# Comparing `tmp/chat_portal-0.2.7.tar.gz` & `tmp/chat_portal-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chat_portal-0.2.7.tar", max compression
+gzip compressed data, was "chat_portal-0.2.8.tar", max compression
```

## Comparing `chat_portal-0.2.7.tar` & `chat_portal-0.2.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1071 2023-12-20 02:02:24.997703 chat_portal-0.2.7/LICENSE
--rw-r--r--   0        0        0     2235 2024-03-29 17:38:21.051330 chat_portal-0.2.7/README.md
--rw-r--r--   0        0        0      138 2024-03-29 17:35:29.617044 chat_portal-0.2.7/chat_portal/__init__.py
--rw-r--r--   0        0        0     4963 2024-03-29 15:18:21.813160 chat_portal-0.2.7/chat_portal/_database.py
--rw-r--r--   0        0        0     2693 2024-03-31 18:03:53.717025 chat_portal-0.2.7/chat_portal/_entities.py
--rw-r--r--   0        0        0      954 2024-03-31 18:33:14.726979 chat_portal-0.2.7/chat_portal/_logger.py
--rw-r--r--   0        0        0      430 2024-03-27 13:16:48.370825 chat_portal-0.2.7/chat_portal/_models.py
--rw-r--r--   0        0        0     7392 2024-03-31 16:35:19.181428 chat_portal-0.2.7/chat_portal/_portal.py
--rw-r--r--   0        0        0     4374 2024-03-31 16:35:50.151437 chat_portal-0.2.7/chat_portal/interface.py
--rw-r--r--   0        0        0       33 2023-12-21 17:00:55.545635 chat_portal-0.2.7/chat_portal/platforms/__init__.py
--rw-r--r--   0        0        0     4124 2024-03-27 16:04:26.656053 chat_portal-0.2.7/chat_portal/platforms/_instagram.py
--rw-r--r--   0        0        0       34 2024-01-01 13:01:43.063672 chat_portal-0.2.7/chat_portal/portals/__init__.py
--rw-r--r--   0        0        0     4824 2024-03-31 16:21:54.571464 chat_portal-0.2.7/chat_portal/portals/_gpt_portal.py
--rw-r--r--   0        0        0      536 2024-03-31 18:33:41.496978 chat_portal-0.2.7/pyproject.toml
--rw-r--r--   0        0        0     3061 1970-01-01 00:00:00.000000 chat_portal-0.2.7/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-12-20 02:02:24.997703 chat_portal-0.2.8/LICENSE
+-rw-r--r--   0        0        0     2235 2024-03-29 17:38:21.051330 chat_portal-0.2.8/README.md
+-rw-r--r--   0        0        0      138 2024-03-29 17:35:29.617044 chat_portal-0.2.8/chat_portal/__init__.py
+-rw-r--r--   0        0        0     4963 2024-04-07 18:14:19.554879 chat_portal-0.2.8/chat_portal/_database.py
+-rw-r--r--   0        0        0     2693 2024-04-07 18:14:19.554879 chat_portal-0.2.8/chat_portal/_entities.py
+-rw-r--r--   0        0        0      954 2024-03-31 18:33:14.726979 chat_portal-0.2.8/chat_portal/_logger.py
+-rw-r--r--   0        0        0      430 2024-03-27 13:16:48.370825 chat_portal-0.2.8/chat_portal/_models.py
+-rw-r--r--   0        0        0     7392 2024-03-31 16:35:19.181428 chat_portal-0.2.8/chat_portal/_portal.py
+-rw-r--r--   0        0        0     4374 2024-03-31 16:35:50.151437 chat_portal-0.2.8/chat_portal/interface.py
+-rw-r--r--   0        0        0       33 2023-12-21 17:00:55.545635 chat_portal-0.2.8/chat_portal/platforms/__init__.py
+-rw-r--r--   0        0        0     4124 2024-03-27 16:04:26.656053 chat_portal-0.2.8/chat_portal/platforms/_instagram.py
+-rw-r--r--   0        0        0       34 2024-01-01 13:01:43.063672 chat_portal-0.2.8/chat_portal/portals/__init__.py
+-rw-r--r--   0        0        0     4888 2024-04-07 18:16:46.617638 chat_portal-0.2.8/chat_portal/portals/_gpt_portal.py
+-rw-r--r--   0        0        0      536 2024-04-07 18:21:17.267581 chat_portal-0.2.8/pyproject.toml
+-rw-r--r--   0        0        0     3061 1970-01-01 00:00:00.000000 chat_portal-0.2.8/PKG-INFO
```

### Comparing `chat_portal-0.2.7/LICENSE` & `chat_portal-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `chat_portal-0.2.7/README.md` & `chat_portal-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `chat_portal-0.2.7/chat_portal/_database.py` & `chat_portal-0.2.8/chat_portal/_database.py`

 * *Files identical despite different names*

### Comparing `chat_portal-0.2.7/chat_portal/_entities.py` & `chat_portal-0.2.8/chat_portal/_entities.py`

 * *Files identical despite different names*

### Comparing `chat_portal-0.2.7/chat_portal/_logger.py` & `chat_portal-0.2.8/chat_portal/_logger.py`

 * *Files identical despite different names*

### Comparing `chat_portal-0.2.7/chat_portal/_portal.py` & `chat_portal-0.2.8/chat_portal/_portal.py`

 * *Files identical despite different names*

### Comparing `chat_portal-0.2.7/chat_portal/interface.py` & `chat_portal-0.2.8/chat_portal/interface.py`

 * *Files identical despite different names*

### Comparing `chat_portal-0.2.7/chat_portal/platforms/_instagram.py` & `chat_portal-0.2.8/chat_portal/platforms/_instagram.py`

 * *Files identical despite different names*

### Comparing `chat_portal-0.2.7/chat_portal/portals/_gpt_portal.py` & `chat_portal-0.2.8/chat_portal/portals/_gpt_portal.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         self.system_prompt_template = system_prompt_template
 
     def _modifyUnsentMessages(self, received_messages: List[ReceivedMessage], from_thread: Thread, to_thread: Thread):
         if len(received_messages) == 0: return []
         from_user = self.database.fetchUser(from_thread.user_id)
         to_user = self.database.fetchUser(to_thread.user_id)
         assert from_user is not None and to_user is not None
-        sys_prompt = self._sysPrompt(from_user, to_user)
+        sys_prompt = self._sysPrompt(from_thread, to_thread, from_user, to_user)
         user_prompt = self._messagesToGptPrompt(received_messages, to_thread, from_user, to_user)
         gpt_messages = self._messagesToModified(received_messages, sys_prompt, user_prompt)
         return self._toModifiedMessageList(gpt_messages, received_messages, to_thread)
 
     def _messagesToGptPrompt(self, received_messages: List[ReceivedMessage], to_thread: Thread, from_user: User, to_user: User) -> str:
         first_timestamp = min(map(lambda msg: msg.timestamp, received_messages))
         conversation = self.database.conversationHistory(to_thread.id, first_timestamp, MAX_CONTEXT_MESSAGES)
@@ -72,15 +72,15 @@
                 for i, processed_message in enumerate(gpt_messages)
             ]
         return [
             ModifiedMessage(received_message.id, to_thread.id, processed_message, received_message.timestamp)
             for received_message, processed_message in zip(received_messages, gpt_messages)
         ]
 
-    def _sysPrompt(self, from_user: User, to_user: User) -> str:
+    def _sysPrompt(self, from_thread: Thread, to_thread: Thread, from_user: User, to_user: User) -> str:
         return self.system_prompt_template.format(
             from_name=GptPortal._determineName(from_user),
             to_name=GptPortal._determineName(to_user)
         )
 
     @staticmethod
     def _determineName(user: User) -> str:
```

### Comparing `chat_portal-0.2.7/pyproject.toml` & `chat_portal-0.2.8/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "chat-portal"
-version = "0.2.7"
+version = "0.2.8"
 description = "Pair a profile's message contacts and transport modified messages that pretend to come from the initial profile"
 authors = ["kuco23 <nseverkar@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/kuco23/chat-portal/"
 
 [tool.poetry.dependencies]
```

### Comparing `chat_portal-0.2.7/PKG-INFO` & `chat_portal-0.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chat-portal
-Version: 0.2.7
+Version: 0.2.8
 Summary: Pair a profile's message contacts and transport modified messages that pretend to come from the initial profile
 Home-page: https://github.com/kuco23/chat-portal/
 License: MIT
 Author: kuco23
 Author-email: nseverkar@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

