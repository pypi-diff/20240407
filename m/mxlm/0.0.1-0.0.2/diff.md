# Comparing `tmp/mxlm-0.0.1.tar.gz` & `tmp/mxlm-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mxlm-0.0.1.tar", last modified: Sat Mar 30 09:35:35 2024, max compression
+gzip compressed data, was "mxlm-0.0.2.tar", last modified: Sun Apr  7 12:50:58 2024, max compression
```

## Comparing `mxlm-0.0.1.tar` & `mxlm-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 yl        (1000) yl        (1000)        0 2024-03-30 09:35:35.277701 mxlm-0.0.1/
--rw-rw-r--   0 yl        (1000) yl        (1000)       35 2024-03-21 10:12:22.000000 mxlm-0.0.1/MANIFEST.in
--rw-r--r--   0 yl        (1000) yl        (1000)      481 2024-03-30 09:35:35.277701 mxlm-0.0.1/PKG-INFO
--rw-rw-r--   0 yl        (1000) yl        (1000)      601 2024-03-30 08:36:12.000000 mxlm-0.0.1/README.md
-drwxrwxr-x   0 yl        (1000) yl        (1000)        0 2024-03-30 09:35:35.277701 mxlm-0.0.1/mxlm/
--rw-rw-r--   0 yl        (1000) yl        (1000)      585 2024-03-30 08:38:20.000000 mxlm-0.0.1/mxlm/__info__.py
--rw-rw-r--   0 yl        (1000) yl        (1000)      128 2024-03-29 08:26:32.000000 mxlm-0.0.1/mxlm/__init__.py
--rw-rw-r--   0 yl        (1000) yl        (1000)     2611 2024-03-30 08:05:51.000000 mxlm-0.0.1/mxlm/chat_api.py
--rw-rw-r--   0 yl        (1000) yl        (1000)     1983 2024-03-30 07:21:31.000000 mxlm-0.0.1/mxlm/chatmd_utils.py
-drwxrwxr-x   0 yl        (1000) yl        (1000)        0 2024-03-30 09:35:35.277701 mxlm-0.0.1/mxlm.egg-info/
--rw-r--r--   0 yl        (1000) yl        (1000)      481 2024-03-30 09:35:35.000000 mxlm-0.0.1/mxlm.egg-info/PKG-INFO
--rw-rw-r--   0 yl        (1000) yl        (1000)      258 2024-03-30 09:35:35.000000 mxlm-0.0.1/mxlm.egg-info/SOURCES.txt
--rw-rw-r--   0 yl        (1000) yl        (1000)        1 2024-03-30 09:35:35.000000 mxlm-0.0.1/mxlm.egg-info/dependency_links.txt
--rw-rw-r--   0 yl        (1000) yl        (1000)        7 2024-03-30 09:35:35.000000 mxlm-0.0.1/mxlm.egg-info/requires.txt
--rw-rw-r--   0 yl        (1000) yl        (1000)        5 2024-03-30 09:35:35.000000 mxlm-0.0.1/mxlm.egg-info/top_level.txt
--rw-rw-r--   0 yl        (1000) yl        (1000)        8 2024-03-24 13:30:54.000000 mxlm-0.0.1/requirements.txt
--rw-rw-r--   0 yl        (1000) yl        (1000)       38 2024-03-30 09:35:35.277701 mxlm-0.0.1/setup.cfg
--rw-rw-r--   0 yl        (1000) yl        (1000)      962 2024-03-24 13:17:50.000000 mxlm-0.0.1/setup.py
+drwxrwxr-x   0 yl        (1000) yl        (1000)        0 2024-04-07 12:50:58.875848 mxlm-0.0.2/
+-rw-rw-r--   0 yl        (1000) yl        (1000)       35 2024-03-21 10:12:22.000000 mxlm-0.0.2/MANIFEST.in
+-rw-r--r--   0 yl        (1000) yl        (1000)      481 2024-04-07 12:50:58.875848 mxlm-0.0.2/PKG-INFO
+-rw-rw-r--   0 yl        (1000) yl        (1000)      601 2024-03-30 08:36:12.000000 mxlm-0.0.2/README.md
+drwxrwxr-x   0 yl        (1000) yl        (1000)        0 2024-04-07 12:50:58.875848 mxlm-0.0.2/mxlm/
+-rw-rw-r--   0 yl        (1000) yl        (1000)      585 2024-04-07 12:47:58.000000 mxlm-0.0.2/mxlm/__info__.py
+-rw-rw-r--   0 yl        (1000) yl        (1000)      128 2024-03-29 08:26:32.000000 mxlm-0.0.2/mxlm/__init__.py
+-rw-rw-r--   0 yl        (1000) yl        (1000)     2709 2024-04-07 12:49:51.000000 mxlm-0.0.2/mxlm/chat_api.py
+-rw-rw-r--   0 yl        (1000) yl        (1000)     2023 2024-04-07 12:48:14.000000 mxlm-0.0.2/mxlm/chatmd_utils.py
+drwxrwxr-x   0 yl        (1000) yl        (1000)        0 2024-04-07 12:50:58.875848 mxlm-0.0.2/mxlm.egg-info/
+-rw-r--r--   0 yl        (1000) yl        (1000)      481 2024-04-07 12:50:58.000000 mxlm-0.0.2/mxlm.egg-info/PKG-INFO
+-rw-rw-r--   0 yl        (1000) yl        (1000)      258 2024-04-07 12:50:58.000000 mxlm-0.0.2/mxlm.egg-info/SOURCES.txt
+-rw-rw-r--   0 yl        (1000) yl        (1000)        1 2024-04-07 12:50:58.000000 mxlm-0.0.2/mxlm.egg-info/dependency_links.txt
+-rw-rw-r--   0 yl        (1000) yl        (1000)        7 2024-04-07 12:50:58.000000 mxlm-0.0.2/mxlm.egg-info/requires.txt
+-rw-rw-r--   0 yl        (1000) yl        (1000)        5 2024-04-07 12:50:58.000000 mxlm-0.0.2/mxlm.egg-info/top_level.txt
+-rw-rw-r--   0 yl        (1000) yl        (1000)        8 2024-03-24 13:30:54.000000 mxlm-0.0.2/requirements.txt
+-rw-rw-r--   0 yl        (1000) yl        (1000)       38 2024-04-07 12:50:58.875848 mxlm-0.0.2/setup.cfg
+-rw-rw-r--   0 yl        (1000) yl        (1000)      962 2024-03-24 13:17:50.000000 mxlm-0.0.2/setup.py
```

### Comparing `mxlm-0.0.1/README.md` & `mxlm-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `mxlm-0.0.1/mxlm/__info__.py` & `mxlm-0.0.2/mxlm/__info__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.0.1"
+__version__ = "0.0.2"
 __description__ = "Language Model Utils"
 __license__ = "MIT"
 __author__ = "DIYer22"
 __author_email__ = "ylxx@live.com"
 __maintainer__ = "DIYer22"
 __maintainer_email__ = "ylxx@live.com"
 __github_username__ = "DIYer22"
```

### Comparing `mxlm-0.0.1/mxlm/chat_api.py` & `mxlm-0.0.2/mxlm/chat_api.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,42 +1,46 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
-from openai import OpenAI
 
 
 class ChatAPI:
     default_messages = [
         {"role": "system", "content": "You are a helpful assistant."},
         {"role": "user", "content": "Just repeat `mxlm`."},
     ]
     default_base_url = None
 
     def __init__(self, base_url=None, api_key="sk-NoneKey", **default_argkws):
+        from openai import OpenAI
+
         self.base_url = base_url or self.default_base_url
         self.api_key = api_key
-        self.client = OpenAI(api_key=api_key, base_url=base_url)
+        self.client = OpenAI(api_key=self.api_key, base_url=self.base_url)
         self.default_argkws = dict(
-            model=self.get_model_list()[-1]["id"],
+            model=self.get_default_model(),
             max_tokens=1024,
             top_p=0.9,
             temperature=0.5,
         )
         self.default_argkws.update(default_argkws)
 
     def get_model_list(self):
         return self.client.models.list().dict()["data"]
 
+    def get_default_model(self):
+        return self.get_model_list()[-1]["id"]
+
     def __call__(
         self, messages=None, return_messages=False, return_dict=False, **argkws_
     ):
         """
         Returns new message.content by default
         """
         messages = messages or self.default_messages
-        argkws = self.default_argkws
+        argkws = self.default_argkws.copy()
         argkws.update(argkws_)
         response = self.client.chat.completions.create(messages=messages, **argkws)
 
         if argkws.get("stream"):
             content = ""
             for chunki, chunk in enumerate(response):
                 if not chunki:
@@ -63,15 +67,17 @@
 
     def __str__(self):
         import json
 
         argkws_str = json.dumps(self.default_argkws, indent=2)
         return f"mxlm.ChatAPI{tuple([self.base_url])}:\n{argkws_str[2:-2]}"
 
+    __repr__ = __str__
+
 
 if __name__ == "__main__":
     from boxx import *
 
-    client = ChatAPI("http://127.0.0.1:9200/v1")
+    client = ChatAPI()
     print(client)
     msg = client(stream=True)
     # print(msg)
```

### Comparing `mxlm-0.0.1/mxlm/chatmd_utils.py` & `mxlm-0.0.2/mxlm/chatmd_utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -39,40 +39,40 @@
         }
         tag = match.group("tag")
         if tag:
             # Revert to json if tag is json
             is_dict = tag[0] == "{" and tag[-1] == "}" and ":" in tag
             is_list = tag[0] == "[" and tag[-1] == "]"
             if is_dict or is_list:
-                print(tag)
                 tag = json.loads(tag)
             msg["tag"] = tag
         messages.append(msg)
     return messages
 
 
 if __name__ == "__main__":
     chatmd_example = """
 
-<!--<|BOT|>--><hr></hr><hr></hr> tag must be one line. Could be str or json
+<!--<|BOT|>--><hr></hr><hr></hr> Here you can put the `tag`, must be one line. Could be str or JSON.
 ## system
 You are a helpful assistant.
 
-<!--<|BOT|>--><hr></hr><hr></hr> {"role": "del", "content": "Thank you, doctor2!"}
+<!--<|BOT|>--><hr></hr><hr></hr> {"url":"XXX.html", "title":"XXX"}
 ## context
-None
+{text from url}
 
 <!--<|BOT|>--><hr></hr><hr></hr>
 ## comment
-Multi-line comments 
-that will not be seen by model
+Multi-line comments.  
+Visible to humans but invisible to models.
 
 <!--<|BOT|>--><hr></hr><hr></hr>
 ## user  
-Thank you, doctor2!
+Summarize the content in this url: 
+https://XXX.html
 """
     msgs = chatmd_to_messages(chatmd_example)
     for msg in msgs:
         print(msg)
 
     chatmd = messages_to_chatmd(msgs)
     print(chatmd)
```

### Comparing `mxlm-0.0.1/setup.py` & `mxlm-0.0.2/setup.py`

 * *Files identical despite different names*

