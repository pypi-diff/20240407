# Comparing `tmp/anonymous-chatgpt-0.0.1.tar.gz` & `tmp/anonymous-chatgpt-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anonymous-chatgpt-0.0.1.tar", last modified: Sat Apr  6 12:45:26 2024, max compression
+gzip compressed data, was "anonymous-chatgpt-0.0.2.tar", last modified: Sat Apr  6 16:21:20 2024, max compression
```

## Comparing `anonymous-chatgpt-0.0.1.tar` & `anonymous-chatgpt-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 meet      (1000) meet      (1000)        0 2024-04-06 12:45:26.027799 anonymous-chatgpt-0.0.1/
--rw-rw-r--   0 meet      (1000) meet      (1000)     1932 2024-04-06 12:45:26.027799 anonymous-chatgpt-0.0.1/PKG-INFO
--rw-r--r--   0 meet      (1000) meet      (1000)     1308 2024-04-06 12:07:48.000000 anonymous-chatgpt-0.0.1/README.md
-drwxrwxr-x   0 meet      (1000) meet      (1000)        0 2024-04-06 12:45:26.027799 anonymous-chatgpt-0.0.1/anonymous_chatgpt.egg-info/
--rw-rw-r--   0 meet      (1000) meet      (1000)     1932 2024-04-06 12:45:25.000000 anonymous-chatgpt-0.0.1/anonymous_chatgpt.egg-info/PKG-INFO
--rw-rw-r--   0 meet      (1000) meet      (1000)      321 2024-04-06 12:45:25.000000 anonymous-chatgpt-0.0.1/anonymous_chatgpt.egg-info/SOURCES.txt
--rw-rw-r--   0 meet      (1000) meet      (1000)        1 2024-04-06 12:45:25.000000 anonymous-chatgpt-0.0.1/anonymous_chatgpt.egg-info/dependency_links.txt
--rw-rw-r--   0 meet      (1000) meet      (1000)       46 2024-04-06 12:45:25.000000 anonymous-chatgpt-0.0.1/anonymous_chatgpt.egg-info/entry_points.txt
--rw-rw-r--   0 meet      (1000) meet      (1000)        9 2024-04-06 12:45:25.000000 anonymous-chatgpt-0.0.1/anonymous_chatgpt.egg-info/requires.txt
--rw-rw-r--   0 meet      (1000) meet      (1000)        8 2024-04-06 12:45:25.000000 anonymous-chatgpt-0.0.1/anonymous_chatgpt.egg-info/top_level.txt
-drwxrwxr-x   0 meet      (1000) meet      (1000)        0 2024-04-06 12:45:26.027799 anonymous-chatgpt-0.0.1/chatgpt/
--rw-rw-r--   0 meet      (1000) meet      (1000)        0 2024-04-06 11:50:12.000000 anonymous-chatgpt-0.0.1/chatgpt/__init__.py
--rw-r--r--   0 meet      (1000) meet      (1000)       99 2024-04-06 12:37:42.000000 anonymous-chatgpt-0.0.1/chatgpt/__main__.py
--rw-rw-r--   0 meet      (1000) meet      (1000)     2856 2024-04-06 12:41:54.000000 anonymous-chatgpt-0.0.1/chatgpt/app.py
--rw-rw-r--   0 meet      (1000) meet      (1000)       38 2024-04-06 12:45:26.027799 anonymous-chatgpt-0.0.1/setup.cfg
--rw-r--r--   0 meet      (1000) meet      (1000)      882 2024-04-06 12:43:29.000000 anonymous-chatgpt-0.0.1/setup.py
+drwxrwxr-x   0 meet      (1000) meet      (1000)        0 2024-04-06 16:21:20.310142 anonymous-chatgpt-0.0.2/
+-rw-rw-r--   0 meet      (1000) meet      (1000)     1889 2024-04-06 16:21:20.310142 anonymous-chatgpt-0.0.2/PKG-INFO
+-rw-r--r--   0 meet      (1000) meet      (1000)     1540 2024-04-06 16:15:56.000000 anonymous-chatgpt-0.0.2/README.md
+drwxrwxr-x   0 meet      (1000) meet      (1000)        0 2024-04-06 16:21:20.310142 anonymous-chatgpt-0.0.2/anonymous_chatgpt/
+-rw-rw-r--   0 meet      (1000) meet      (1000)       19 2024-04-06 16:17:19.000000 anonymous-chatgpt-0.0.2/anonymous_chatgpt/__init__.py
+-rw-r--r--   0 meet      (1000) meet      (1000)       58 2024-04-06 16:17:00.000000 anonymous-chatgpt-0.0.2/anonymous_chatgpt/__main__.py
+-rw-rw-r--   0 meet      (1000) meet      (1000)     3178 2024-04-06 16:18:36.000000 anonymous-chatgpt-0.0.2/anonymous_chatgpt/app.py
+drwxrwxr-x   0 meet      (1000) meet      (1000)        0 2024-04-06 16:21:20.310142 anonymous-chatgpt-0.0.2/anonymous_chatgpt.egg-info/
+-rw-rw-r--   0 meet      (1000) meet      (1000)     1889 2024-04-06 16:21:20.000000 anonymous-chatgpt-0.0.2/anonymous_chatgpt.egg-info/PKG-INFO
+-rw-rw-r--   0 meet      (1000) meet      (1000)      351 2024-04-06 16:21:20.000000 anonymous-chatgpt-0.0.2/anonymous_chatgpt.egg-info/SOURCES.txt
+-rw-rw-r--   0 meet      (1000) meet      (1000)        1 2024-04-06 16:21:20.000000 anonymous-chatgpt-0.0.2/anonymous_chatgpt.egg-info/dependency_links.txt
+-rw-rw-r--   0 meet      (1000) meet      (1000)       56 2024-04-06 16:21:20.000000 anonymous-chatgpt-0.0.2/anonymous_chatgpt.egg-info/entry_points.txt
+-rw-rw-r--   0 meet      (1000) meet      (1000)        9 2024-04-06 16:21:20.000000 anonymous-chatgpt-0.0.2/anonymous_chatgpt.egg-info/requires.txt
+-rw-rw-r--   0 meet      (1000) meet      (1000)       18 2024-04-06 16:21:20.000000 anonymous-chatgpt-0.0.2/anonymous_chatgpt.egg-info/top_level.txt
+-rw-rw-r--   0 meet      (1000) meet      (1000)       38 2024-04-06 16:21:20.310142 anonymous-chatgpt-0.0.2/setup.cfg
+-rw-r--r--   0 meet      (1000) meet      (1000)      892 2024-04-06 16:20:55.000000 anonymous-chatgpt-0.0.2/setup.py
```

### Comparing `anonymous-chatgpt-0.0.1/PKG-INFO` & `anonymous-chatgpt-0.0.2/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,44 +1,49 @@
-Metadata-Version: 2.1
-Name: anonymous-chatgpt
-Version: 0.0.1
-Summary: A Python Client to interact with OpenAI's ChatGPT(GPT-3) model without authentication
-Home-page: https://github.com/Mr-Destructive/anonymous-chatgpt
-Author: Meet Gor
-Author-email: gormeet711@gmail.com
-License: UNKNOWN
-Description: # Anonymous ChatGPT Client 
-        
-        - Access basic ChatGPT model without authentication
-        
-        OpenAI recently made the ChatGPT model accessible anonymously. You can access it without authentication.
-        Read more about it in the [official docs](https://openai.com/blog/start-using-chatgpt-instantly)
-        
-        ## Installation
-        
-        - Install the package/cli
-        
-        ```bash
-        pip install anonymous-chatgpt
-        ```
-        
-        ## Usage
-        
-        ```bash
-        chatgpt --prompt "hello world"
-        ```
-        
-        
-        ## Process of creating a authentication-less client
-        
-        1. Send the first request to the ChatGPT API i.e. `chat.openai.com`
-        2. The response of that request has cookies for authentication(not user just user-agent and csrf tokens)
-        3. Those cookies are carried in all the upcoming requests
-        4. Send the second request to the [Sential API](https://techcommunity.microsoft.com/t5/manufacturing/introduction-to-openai-and-microsoft-sentinel/ba-p/3761907) i.e. `/backend-anon/sentinel/chat-requirements`
-        5. This request gives us the `sentinel-token` which is the token used for authentication and authorization of the requests (not users).
-        6. We use this token in all the subsequent requests
-        7. The third request is the actual request to the **Anonymous Conversation** endpoint i.e. `/backend-anon/conversation`
-        8. This is a streamed request which returns the response in the form of chunks
-        
-        
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
+# Anonymous ChatGPT Client 
+
+- Access basic ChatGPT model without authentication
+
+OpenAI recently made the ChatGPT model accessible anonymously. You can access it without authentication.
+Read more about it in the [official docs](https://openai.com/blog/start-using-chatgpt-instantly)
+
+## Installation
+
+- Install the package/cli
+
+```bash
+pip install anonymous-chatgpt
+```
+
+## Usage
+
+### CLI
+
+```bash
+chatgpt --prompt "hello world"
+```
+
+#### CLI Demonstration
+
+[Anonymous ChatGPT Demo](https://meetgor-cdn.pages.dev/anonymous-chatgpt-demo.gif)
+
+### Package
+
+```bash
+from anonymous_chatgpt import chat
+
+
+message = chat(prompt="hello world")
+print(message)
+```
+
+
+## Process of creating a authentication-less client
+
+1. Send the first request to the ChatGPT API i.e. `chat.openai.com`
+2. The response of that request has cookies for authentication(not user just user-agent and csrf tokens)
+3. Those cookies are carried in all the upcoming requests
+4. Send the second request to the [Sential API](https://techcommunity.microsoft.com/t5/manufacturing/introduction-to-openai-and-microsoft-sentinel/ba-p/3761907) i.e. `/backend-anon/sentinel/chat-requirements`
+5. This request gives us the `sentinel-token` which is the token used for authentication and authorization of the requests (not users).
+6. We use this token in all the subsequent requests
+7. The third request is the actual request to the **Anonymous Conversation** endpoint i.e. `/backend-anon/conversation`
+8. This is a streamed request which returns the response in the form of chunks
+
```

### Comparing `anonymous-chatgpt-0.0.1/chatgpt/app.py` & `anonymous-chatgpt-0.0.2/anonymous_chatgpt/app.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,26 @@
 import argparse
 import requests
 import json
 import uuid
 
 
-def simple_chat():
+def chat(prompt: str):
     BASE_URL = "https://chat.openai.com"
 
-    args = argparse.ArgumentParser()
-    args.add_argument("--prompt", type=str, required=True)
-    args = args.parse_args()
-
-    prompt = args.prompt
-
     # First request to get the cookies
     headers = {
         "user-agent": "Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/123.0.0.0 Safari/537.36"
     }
+    resp_message = {}
 
     request_client = requests.session()
     response = request_client.get(BASE_URL, headers=headers)
+    if response.status_code != 200:
+        response.raise_for_status()
     set_cookie = response.cookies.get_dict()
 
     cookies = "; ".join([f"{key}={value}" for key, value in set_cookie.items()])
 
     chat_req_url = f"{BASE_URL}/backend-anon/sentinel/chat-requirements"
     headers = {
         "accept": "text/event-stream",
@@ -38,14 +35,16 @@
     }
 
     # second request to get the OpenAI's Sentinel token
     chat_req_res = request_client.post(chat_req_url, headers=headers)
     chat_req_token = ""
     if chat_req_res.status_code == 200:
         chat_req_token = chat_req_res.json().get("token")
+    else:
+        chat_req_res.raise_for_status()
 
 
     # third request to get the response to the prompt
     url = f"{BASE_URL}/backend-anon/conversation"
     headers = {
         **headers,
         "openai-sentinel-chat-requirements-token": chat_req_token,
@@ -74,21 +73,30 @@
         "force_paragen_model_slug": "",
         "force_nulligen": False,
         "force_rate_limit": False,
     }
 
     response = request_client.post(url, headers=headers, json=data)
     if response.status_code != 200:
-        print(response.status_code, response.text)
-        return
+        resp_message["error"] = response.text
+        response.raise_for_status()
     data = response.text
     msgs = data.split("\ndata:")
     if len(msgs) > 1:
         resp = json.loads(msgs[-2])
-        print(resp["message"]["content"]["parts"][0])
+        messages = resp.get("message", {}).get("content", {}).get("parts", [])
+        if len(messages) > 0:
+            resp_message["message"] = messages[0]
+    return resp_message
 
 def main():
-    simple_chat()
+    args = argparse.ArgumentParser()
+    args.add_argument("--prompt", type=str, required=True)
+    args = args.parse_args()
+    prompt = args.prompt
+    response = chat(prompt)
+    print(response)
+
 
 if __name__ == "__main__":
     main()
```

### Comparing `anonymous-chatgpt-0.0.1/setup.py` & `anonymous-chatgpt-0.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pathlib
 from setuptools import setup, find_packages
 
 HERE = pathlib.Path(__file__).parent
 
-VERSION = "0.0.1"
+VERSION = "0.0.2"
 PACKAGE_NAME = "anonymous-chatgpt"
 AUTHOR = "Meet Gor"
 AUTHOR_EMAIL = "gormeet711@gmail.com"
 URL = "https://github.com/Mr-Destructive/anonymous-chatgpt"
 
 DESCRIPTION = (
     "A Python Client to interact with OpenAI's ChatGPT(GPT-3) model without authentication"
@@ -26,10 +26,10 @@
     long_description=README,
     long_description_content_type="text/markdown",
     author=AUTHOR,
     author_email=AUTHOR_EMAIL,
     url=URL,
     install_requires=INSTALL_REQUIRES,
     packages=find_packages(),
-    entry_points={"console_scripts": ["chatgpt = chatgpt.app:main"]},
+    entry_points={"console_scripts": ["chatgpt = anonymous_chatgpt.app:main"]},
 )
```

