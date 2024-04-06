# Comparing `tmp/deltachat_faqbot-0.4.0-py3-none-any.whl.zip` & `tmp/deltachat_faqbot-0.5.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 30681 bytes, number of entries: 11
--rw-r--r--  2.0 unx      164 b- defN 24-Feb-06 05:46 faqbot/__init__.py
--rw-r--r--  2.0 unx       65 b- defN 24-Feb-06 05:46 faqbot/__main__.py
--rw-r--r--  2.0 unx     6818 b- defN 24-Feb-06 05:46 faqbot/hooks.py
--rw-r--r--  2.0 unx     1230 b- defN 24-Feb-06 05:46 faqbot/orm.py
--rw-r--r--  2.0 unx      961 b- defN 24-Feb-06 05:46 faqbot/utils.py
--rw-r--r--  2.0 unx    35141 b- defN 24-Feb-06 05:46 deltachat_faqbot-0.4.0.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx    41888 b- defN 24-Feb-06 05:46 deltachat_faqbot-0.4.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Feb-06 05:46 deltachat_faqbot-0.4.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       39 b- defN 24-Feb-06 05:46 deltachat_faqbot-0.4.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        7 b- defN 24-Feb-06 05:46 deltachat_faqbot-0.4.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      900 b- defN 24-Feb-06 05:46 deltachat_faqbot-0.4.0.dist-info/RECORD
-11 files, 87305 bytes uncompressed, 29151 bytes compressed:  66.6%
+Zip file size: 18187 bytes, number of entries: 11
+-rw-r--r--  2.0 unx      164 b- defN 24-Apr-06 22:46 faqbot/__init__.py
+-rw-r--r--  2.0 unx       65 b- defN 24-Apr-06 22:46 faqbot/__main__.py
+-rw-r--r--  2.0 unx     7026 b- defN 24-Apr-06 22:46 faqbot/hooks.py
+-rw-r--r--  2.0 unx     1250 b- defN 24-Apr-06 22:46 faqbot/orm.py
+-rw-r--r--  2.0 unx      957 b- defN 24-Apr-06 22:46 faqbot/utils.py
+-rw-r--r--  2.0 unx    35141 b- defN 24-Apr-06 22:47 deltachat_faqbot-0.5.0.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx     1441 b- defN 24-Apr-06 22:47 deltachat_faqbot-0.5.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-06 22:47 deltachat_faqbot-0.5.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       39 b- defN 24-Apr-06 22:47 deltachat_faqbot-0.5.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        7 b- defN 24-Apr-06 22:47 deltachat_faqbot-0.5.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      899 b- defN 24-Apr-06 22:47 deltachat_faqbot-0.5.0.dist-info/RECORD
+11 files, 47081 bytes uncompressed, 16657 bytes compressed:  64.6%
```

## zipnote {}

```diff
@@ -9,26 +9,26 @@
 
 Filename: faqbot/orm.py
 Comment: 
 
 Filename: faqbot/utils.py
 Comment: 
 
-Filename: deltachat_faqbot-0.4.0.dist-info/LICENSE.txt
+Filename: deltachat_faqbot-0.5.0.dist-info/LICENSE.txt
 Comment: 
 
-Filename: deltachat_faqbot-0.4.0.dist-info/METADATA
+Filename: deltachat_faqbot-0.5.0.dist-info/METADATA
 Comment: 
 
-Filename: deltachat_faqbot-0.4.0.dist-info/WHEEL
+Filename: deltachat_faqbot-0.5.0.dist-info/WHEEL
 Comment: 
 
-Filename: deltachat_faqbot-0.4.0.dist-info/entry_points.txt
+Filename: deltachat_faqbot-0.5.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: deltachat_faqbot-0.4.0.dist-info/top_level.txt
+Filename: deltachat_faqbot-0.5.0.dist-info/top_level.txt
 Comment: 
 
-Filename: deltachat_faqbot-0.4.0.dist-info/RECORD
+Filename: deltachat_faqbot-0.5.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## faqbot/hooks.py

```diff
@@ -1,21 +1,23 @@
 """Event Hooks"""
 
 import os
 from argparse import Namespace
 from tempfile import TemporaryDirectory
 
-from deltabot_cli import (
-    AttrDict,
+from deltabot_cli import BotCli
+from deltachat2 import (
     Bot,
-    BotCli,
+    ChatType,
+    CoreEvent,
     EventType,
-    const,
+    Message,
+    MsgData,
+    NewMsgEvent,
     events,
-    is_not_known_command,
 )
 from sqlalchemy.exc import IntegrityError
 from sqlalchemy.future import select
 
 from .orm import FAQ, init, session_scope
 from .utils import get_answer_text, get_faq
 
@@ -25,40 +27,41 @@
 @cli.on_init
 def on_init(bot: Bot, _args: Namespace) -> None:
     for accid in bot.rpc.get_all_account_ids():
         if not bot.rpc.get_config(accid, "displayname"):
             bot.rpc.set_config(accid, "displayname", "FAQ Bot")
             status = "I am a Delta Chat bot, send me /help for more info"
             bot.rpc.set_config(accid, "selfstatus", status)
-            bot.rpc.set_config(accid, "delete_server_after", "1")
+            bot.rpc.set_config(accid, "delete_device_after", str(60 * 60 * 24 * 30))
 
 
 @cli.on_start
 def _on_start(_bot: Bot, args: Namespace) -> None:
     path = os.path.join(args.config_dir, "sqlite.db")
     init(f"sqlite:///{path}")
 
 
 @cli.on(events.RawEvent)
-def log_event(bot: Bot, accid: int, event: AttrDict) -> None:
+def log_event(bot: Bot, accid: int, event: CoreEvent) -> None:
     if event.kind == EventType.INFO:
         bot.logger.info(event.msg)
     elif event.kind == EventType.WARNING:
         bot.logger.warning(event.msg)
     elif event.kind == EventType.ERROR:
         bot.logger.error(event.msg)
     elif event.kind == EventType.SECUREJOIN_INVITER_PROGRESS:
         if event.progress == 1000:
-            bot.logger.debug("QR scanned by contact id=%s", event.contact_id)
-            chatid = bot.rpc.create_chat_by_contact_id(accid, event.contact_id)
-            send_help(bot, accid, chatid)
+            if not bot.rpc.get_contact(accid, event.contact_id).is_bot:
+                bot.logger.debug("QR scanned by contact=%s", event.contact_id)
+                chatid = bot.rpc.create_chat_by_contact_id(accid, event.contact_id)
+                send_help(bot, accid, chatid)
 
 
 @cli.on(events.NewMessage(command="/help"))
-def _help(bot: Bot, accid: int, event: AttrDict) -> None:
+def _help(bot: Bot, accid: int, event: NewMsgEvent) -> None:
     send_help(bot, accid, event.msg.chat_id)
 
 
 def send_help(bot: Bot, accid: int, chat_id: int) -> None:
     text = """**Available commands**
 
 /faq - sends available topics.
@@ -69,57 +72,57 @@
 
 /remove TAG - remove the saved tag/question and its reply
 
 
 **How to use me?**
 
 Add me to a group then you can use the /save and /faq commands there"""
-    bot.rpc.send_msg(accid, chat_id, {"text": text})
+    bot.rpc.send_msg(accid, chat_id, MsgData(text=text))
 
 
 @cli.on(events.NewMessage(command="/faq"))
-def _faq(bot: Bot, accid: int, event: AttrDict) -> None:
+def _faq(bot: Bot, accid: int, event: NewMsgEvent) -> None:
     msg = event.msg
     if reply_to_command_in_dm(bot, accid, msg):
         return
 
     with session_scope() as session:
         text = get_faq(msg.chat_id, session)
-    bot.rpc.send_msg(accid, msg.chat_id, {"text": f"**FAQ**\n\n{text}"})
+    bot.rpc.send_msg(accid, msg.chat_id, MsgData(text=f"**FAQ**\n\n{text}"))
 
 
 @cli.on(events.NewMessage(command="/remove"))
-def _remove(bot: Bot, accid: int, event: AttrDict) -> None:
+def _remove(bot: Bot, accid: int, event: NewMsgEvent) -> None:
     msg = event.msg
     if reply_to_command_in_dm(bot, accid, msg):
         return
 
     question = event.payload
     stmt = select(FAQ).filter(FAQ.chat_id == msg.chat_id, FAQ.question == question)
     with session_scope() as session:
         with session.begin():
             faq = (session.execute(stmt)).scalars().first()
             if faq:
                 session.delete(faq)
-                reply = {"text": "✅ Note removed", "quotedMessageId": msg.id}
+                reply = MsgData(text="✅ Note removed", quoted_message_id=msg.id)
                 bot.rpc.send_msg(accid, msg.chat_id, reply)
 
 
 @cli.on(events.NewMessage(command="/save"))
-def _save(bot: Bot, accid: int, event: AttrDict) -> None:
+def _save(bot: Bot, accid: int, event: NewMsgEvent) -> None:
     msg = event.msg
     if reply_to_command_in_dm(bot, accid, msg):
         return
 
     question = event.payload
-    if question.startswith(const.COMMAND_PREFIX):
-        reply = {
-            "text": f"Invalid text, can not start with {const.COMMAND_PREFIX}",
-            "quotedMessageId": msg.id,
-        }
+    if question.startswith(bot.command_prefix):
+        reply = MsgData(
+            text=f"Invalid text, can not start with {bot.command_prefix}",
+            quoted_message_id=msg.id,
+        )
         bot.rpc.send_msg(accid, msg.chat_id, reply)
         return
     quote = msg.quote
     assert quote
     quote = bot.rpc.get_message(accid, quote.message_id)
     if quote.file:
         with open(quote.file, mode="rb") as attachment:
@@ -135,63 +138,66 @@
                         question=question,
                         answer_text=quote.text,
                         answer_filename=quote.file_name,
                         answer_file=file_bytes,
                         answer_viewtype=quote.view_type,
                     )
                 )
-        reply = {"text": "✅ Saved", "quotedMessageId": msg.id}
+        reply = MsgData(text="✅ Saved", quoted_message_id=msg.id)
     except IntegrityError:
-        reply = {
-            "text": "❌ Error: there is already a saved reply for that tag/question,"
+        reply = MsgData(
+            text="❌ Error: there is already a saved reply for that tag/question,"
             " use /remove first to remove the old reply",
-            "quotedMessageId": msg.id,
-        }
+            quoted_message_id=msg.id,
+        )
     bot.rpc.send_msg(accid, msg.chat_id, reply)
 
 
 @cli.on(events.NewMessage(is_info=False))
-def markseen_commands(bot: Bot, accid: int, event: AttrDict) -> None:
-    if not is_not_known_command(bot, event):
+def markseen_commands(bot: Bot, accid: int, event: NewMsgEvent) -> None:
+    if bot.has_command(event.command):
         bot.rpc.markseen_msgs(accid, [event.msg.id])
 
 
-@cli.on(events.NewMessage(is_info=False, func=is_not_known_command))
-def _answer(bot: Bot, accid: int, event: AttrDict) -> None:
+@cli.on(events.NewMessage(is_info=False))
+def _answer(bot: Bot, accid: int, event: NewMsgEvent) -> None:
+    if bot.has_command(event.command):
+        return
     msg = event.msg
     chat = bot.rpc.get_basic_chat_info(accid, msg.chat_id)
-    if chat.chat_type == const.ChatType.SINGLE:
+    if chat.chat_type == ChatType.SINGLE:
         bot.rpc.markseen_msgs(accid, [msg.id])
         _help(bot, accid, event)
         return
     if event.command or not msg.text:
         return
 
     with session_scope() as session:
         stmt = select(FAQ).filter(FAQ.chat_id == msg.chat_id, FAQ.question == msg.text)
         faq = (session.execute(stmt)).scalars().first()
         if faq:
             quoted_msg_id = msg.quote.message_id if msg.quote else msg.id
-            reply = {
-                "text": get_answer_text(bot, accid, faq, msg, session),
-                "quotedMessageId": quoted_msg_id,
-            }
+            reply = MsgData(
+                text=get_answer_text(bot, accid, faq, msg, session),
+                quoted_message_id=quoted_msg_id,
+            )
             if faq.answer_file:
                 with TemporaryDirectory() as tmp_dir:
                     filename = os.path.join(tmp_dir, faq.answer_filename)
                     with open(filename, mode="wb") as attachment:
                         attachment.write(faq.answer_file)
-                    bot.rpc.send_msg(accid, msg.chat_id, {"file": filename, **reply})
+                    reply.file = filename
+                    bot.rpc.send_msg(accid, msg.chat_id, reply)
             else:
                 bot.rpc.send_msg(accid, msg.chat_id, reply)
 
 
-def reply_to_command_in_dm(bot: Bot, accid: int, msg: AttrDict) -> bool:
+def reply_to_command_in_dm(bot: Bot, accid: int, msg: Message) -> bool:
     chat = bot.rpc.get_basic_chat_info(accid, msg.chat_id)
-    if chat.chat_type == const.ChatType.SINGLE:
-        reply = {
-            "text": "Can't save notes in private, add me to a group and use the command there",
-            "quotedMessageId": msg.id,
-        }
+    if chat.chat_type == ChatType.SINGLE:
+        reply = MsgData(
+            text="Can't save notes in private, add me to a group and use the command there",
+            quoted_message_id=msg.id,
+        )
         bot.rpc.send_msg(accid, msg.chat_id, reply)
         return True
     return False
```

## faqbot/orm.py

```diff
@@ -1,23 +1,25 @@
 """database"""
 
 from contextlib import contextmanager
 from threading import Lock
+from typing import Any
 
 from sqlalchemy import Column, Integer, LargeBinary, String, create_engine
 from sqlalchemy.ext.declarative import declarative_base
 from sqlalchemy.orm import sessionmaker
 
-Base = declarative_base()
+Base: Any = declarative_base()
 _Session = sessionmaker()
 _lock = Lock()
-_session = None  # noqa
 
 
-class FAQ(Base):  # noqa
+class FAQ(Base):
+    """A FAQ entry."""
+
     __tablename__ = "faq"
     chat_id = Column(Integer, primary_key=True)
     question = Column(String, primary_key=True)
     answer_text = Column(String)
     answer_html = Column(String)
     answer_file = Column(LargeBinary)
     answer_filename = Column(String)
```

## faqbot/utils.py

```diff
@@ -1,25 +1,25 @@
 """Utilities"""
 
-from deltabot_cli import AttrDict, Bot
+from deltachat2 import Bot, Message
 from sqlalchemy.future import select
 
 from .orm import FAQ
 
 
 def get_faq(chat_id: int, session) -> str:
     """Get the FAQ list as a markdown list."""
     text = ""
     stmt = select(FAQ).filter(FAQ.chat_id == chat_id)
     for faq in session.execute(stmt).scalars().all():
         text += f"* {faq.question}\n"
     return text
 
 
-def get_answer_text(bot: Bot, accid: int, faq: FAQ, msg: AttrDict, session) -> str:
+def get_answer_text(bot: Bot, accid: int, faq: FAQ, msg: Message, session) -> str:
     """Generate the answer from the given FAQ entry's template answer."""
     if not faq.answer_text:
         return ""
     kwargs = {}
     if msg.quote:
         kwargs["name"] = msg.quote.override_sender_name or msg.quote.author_display_name
     else:
```

## Comparing `deltachat_faqbot-0.4.0.dist-info/LICENSE.txt` & `deltachat_faqbot-0.5.0.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `deltachat_faqbot-0.4.0.dist-info/RECORD` & `deltachat_faqbot-0.5.0.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 faqbot/__init__.py,sha256=HQDDaYy2LJKcpbyq3SCzQ6LLYe8elUMIC6ORVAgMt_4,164
 faqbot/__main__.py,sha256=M7jcIQ0wYwLot7bzOqMQUEJv_190nXbdctI6hrTINbA,65
-faqbot/hooks.py,sha256=IVqcvjjw8XIPdhE3c3laPQbbSpeLR1cbQwViPTMz2Z0,6818
-faqbot/orm.py,sha256=zRiojuDSQ03qULlDmfmPgi35E0x_ed8QHrXNZZ_usmE,1230
-faqbot/utils.py,sha256=5gN_z1Ltg2iB1dH7Y1GYW4aq91zVI2JLv-012CNfjos,961
-deltachat_faqbot-0.4.0.dist-info/LICENSE.txt,sha256=WJ7YI-moTFb-uVrFjnzzhGJrnL9P2iqQe8NuED3hutI,35141
-deltachat_faqbot-0.4.0.dist-info/METADATA,sha256=7C2AibSbry2aW-feaY4TeKqh-7IHfUFqMq0REgfyU3g,41888
-deltachat_faqbot-0.4.0.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
-deltachat_faqbot-0.4.0.dist-info/entry_points.txt,sha256=LPihtLfVtOY_74CMHDuB2b-o-S4mxY8J32JNubC7uVc,39
-deltachat_faqbot-0.4.0.dist-info/top_level.txt,sha256=owc81PC21g6sHQ1ESOzXn8ZV_85OmuEq4RplpAErzd8,7
-deltachat_faqbot-0.4.0.dist-info/RECORD,,
+faqbot/hooks.py,sha256=dC6q9wI4iAsXGN56CrAH13aG55kotAw8vg5pkxoeHPA,7026
+faqbot/orm.py,sha256=01QrRfYB3nk6nx9V0CEWkBhrebz3nC0O06q-6aHUu9U,1250
+faqbot/utils.py,sha256=HPMshutjdZMoUnwiUUqQ2CGMqyCqfR6aSMlzsB8DP8U,957
+deltachat_faqbot-0.5.0.dist-info/LICENSE.txt,sha256=WJ7YI-moTFb-uVrFjnzzhGJrnL9P2iqQe8NuED3hutI,35141
+deltachat_faqbot-0.5.0.dist-info/METADATA,sha256=up_98IafGq2KUNj16y7HmOU4YlQk5C-pDbBv4G1ftME,1441
+deltachat_faqbot-0.5.0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+deltachat_faqbot-0.5.0.dist-info/entry_points.txt,sha256=LPihtLfVtOY_74CMHDuB2b-o-S4mxY8J32JNubC7uVc,39
+deltachat_faqbot-0.5.0.dist-info/top_level.txt,sha256=owc81PC21g6sHQ1ESOzXn8ZV_85OmuEq4RplpAErzd8,7
+deltachat_faqbot-0.5.0.dist-info/RECORD,,
```

