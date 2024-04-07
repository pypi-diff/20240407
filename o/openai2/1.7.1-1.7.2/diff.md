# Comparing `tmp/openai2-1.7.1.tar.gz` & `tmp/openai2-1.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai2-1.7.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "openai2-1.7.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `openai2-1.7.1.tar` & `openai2-1.7.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    11281 2024-02-22 12:02:36.209038 openai2-1.7.1/LICENSE
--rw-r--r--   0        0        0    13971 2024-03-31 09:40:29.216952 openai2-1.7.1/README.md
--rw-r--r--   0        0        0      167 2023-12-19 12:18:48.792856 openai2-1.7.1/__init__.py
--rw-r--r--   0        0        0     6923 2023-11-15 22:45:46.000000 openai2-1.7.1/_core/GroupChat.py
--rw-r--r--   0        0        0     9298 2024-04-06 05:34:07.115496 openai2-1.7.1/_core/chat.py
--rw-r--r--   0        0        0     2279 2024-02-23 04:06:51.826269 openai2-1.7.1/_core/chat_in_cmd.py
--rw-r--r--   0        0        0       99 2024-03-05 23:28:04.263728 openai2-1.7.1/art.json
--rw-r--r--   0        0        0      245 2023-09-04 06:15:02.000000 openai2-1.7.1/licenses/README.md
--rw-r--r--   0        0        0     1083 2020-12-22 18:45:04.000000 openai2-1.7.1/licenses/openai/LICENSE
--rw-r--r--   0        0        0      203 2024-03-03 10:11:45.701543 openai2-1.7.1/openai2.py
--rw-r--r--   0        0        0      805 2024-04-06 05:38:16.070983 openai2-1.7.1/pyproject.toml
--rw-r--r--   0        0        0    14138 1970-01-01 00:00:00.000000 openai2-1.7.1/PKG-INFO
+-rw-r--r--   0        0        0    11281 2024-02-22 12:02:36.209038 openai2-1.7.2/LICENSE
+-rw-r--r--   0        0        0    13991 2024-04-07 02:46:07.779093 openai2-1.7.2/README.md
+-rw-r--r--   0        0        0      168 2024-04-07 02:56:58.773363 openai2-1.7.2/__init__.py
+-rw-r--r--   0        0        0     9858 2024-04-07 03:08:27.254965 openai2-1.7.2/_core/chat.py
+-rw-r--r--   0        0        0     2285 2024-04-07 02:46:07.785077 openai2-1.7.2/_core/chat_in_cmd.py
+-rw-r--r--   0        0        0     6925 2024-04-07 02:46:07.780076 openai2-1.7.2/_core/group_chat.py
+-rw-r--r--   0        0        0       99 2024-03-05 23:28:04.263728 openai2-1.7.2/art.json
+-rw-r--r--   0        0        0      245 2023-09-04 06:15:02.000000 openai2-1.7.2/licenses/README.md
+-rw-r--r--   0        0        0     1083 2020-12-22 18:45:04.000000 openai2-1.7.2/licenses/openai/LICENSE
+-rw-r--r--   0        0        0      191 2024-04-07 02:57:01.800424 openai2-1.7.2/openai2.py
+-rw-r--r--   0        0        0      805 2024-04-07 03:52:00.773865 openai2-1.7.2/pyproject.toml
+-rw-r--r--   0        0        0    14158 1970-01-01 00:00:00.000000 openai2-1.7.2/PKG-INFO
```

### Comparing `openai2-1.7.1/LICENSE` & `openai2-1.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `openai2-1.7.1/README.md` & `openai2-1.7.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -283,20 +283,20 @@
 ]
 ```
 
 ## 限制历史消息数量
 
 ### 限制历史消息数量
 
-随着对话次数越来越多，最终上下文长度就会超出 openai 接口限定的最大 token 数量，此时可使用 MsgMaxCount 参数来限制历史消息数量。当消息数量超出 MsgMaxCount 后，程序会自动移除最早的记录，使消息数量减少到恰好等于 MsgMaxCount 。
+随着对话次数越来越多，最终上下文长度就会超出 openai 接口限定的最大 token 数量，此时可使用 msg_max_count 参数来限制历史消息数量。当消息数量超出 msg_max_count 后，程序会自动移除最早的记录，使消息数量减少到恰好等于 msg_max_count 。
 
 ```python
-MsgMaxCount = 6  # 最多保留6条历史消息
+msg_max_count = 6  # 最多保留6条历史消息
 
-Ariel = Chat(api_key=api_key, model="gpt-3.5-turbo", MsgMaxCount=MsgMaxCount)
+Ariel = Chat(api_key=api_key, model="gpt-3.5-turbo", msg_max_count=msg_max_count)
 
 Ariel.request('英国的首都是什么？')  # >>> '伦敦'
 Ariel.request('日本首都是什么？')  # >>> '东京'
 Ariel.request('意大利的首都是什么？')  # >>> '罗马'
 Ariel.request('美国的首都是什么？')  # >>> '华盛顿'
 Ariel.request('世界上国土面积最大的国家是哪个？')  # >>> '俄罗斯'
 Ariel.request('法国的首都叫什么？')  # >>> '巴黎'
@@ -317,17 +317,17 @@
 ```
 
 ### 锁定消息
 
 当程序自动移除消息记录时，也许我们希望某些消息不要被移除，此时可将这些消息锁定。
 
 ```python
-MsgMaxCount = 6
+msg_max_count = 6
 
-Ariel = Chat(api_key=api_key, model="gpt-3.5-turbo", MsgMaxCount=MsgMaxCount)
+Ariel = Chat(api_key=api_key, model="gpt-3.5-turbo", msg_max_count=msg_max_count)
 
 Ariel.request('英国的首都是什么？')  # >>> '伦敦'
 Ariel.request('日本首都是什么？')  # >>> '东京'
 Ariel.request('意大利的首都是什么？')  # >>> '罗马'
 ```
 
 此时共有 6 条消息记录：
@@ -349,15 +349,15 @@
 
 继续请求：
 
 ```python
 Ariel.request('美国的首都是什么？')  # >>> '华盛顿'
 ```
 
-由于设置了 MsgMaxCount = 6，此时共有 6 条消息记录：
+由于设置了 msg_max_count = 6，此时共有 6 条消息记录：
 
 | 消息                 | 正序索引 | 逆序索引 | 锁定状态 |
 | -------------------- | :------: | :------: | :------: |
 | 英国的首都是什么？   |    0    |    -6    |  已锁定  |
 | 东京                 |    1    |    -5    |    -    |
 | 意大利的首都是什么？ |    2    |    -4    |  已锁定  |
 | 罗马                 |    3    |    -3    |  已锁定  |
```

### Comparing `openai2-1.7.1/_core/GroupChat.py` & `openai2-1.7.2/_core/group_chat.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
                     timeout=None,
                     max_retries=None,
                     http_client=None,
                     # request_kwargs
                     model: Literal["gpt-4-1106-preview", "gpt-4-vision-preview", "gpt-4", "gpt-4-0314", "gpt-4-0613",
                                     "gpt-4-32k", "gpt-4-32k-0314", "gpt-4-32k-0613", "gpt-3.5-turbo"] = "gpt-3.5-turbo",
                     # Chat
-                    MsgMaxCount=None,
+                    msg_max_count=None,
                     # kwargs
                     **kwargs,
                     ):
             ...
     
     def add_dialog(self, speaker:str, audiences:list, remark:str):
         '''
```

### Comparing `openai2-1.7.1/_core/chat.py` & `openai2-1.7.2/_core/chat.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from json import dumps as jsonDumps
 from json import loads as jsonLoads
 from pathlib import Path
-from typing import Union, List, Literal
+from typing import List, Literal
 from openai import OpenAI, AsyncOpenAI
 
 
 class AKPool:
     """ 轮询获取api_key """
 
     def __init__(self, apikeys: list):
@@ -80,17 +80,17 @@
 
     def copy(self):
         que = self.__class__(maxlen=self.maxlen)
         que.core = self.core.copy()
         return que
 
     def deepcopy(self):
-        ...  # 创建这个方法是为了提醒用户: copy 方法是浅拷贝
+        ...  # 创建这个方法是为了以代码提示的方式提醒用户: copy 方法是浅拷贝
 
-    def __add__(self, obj: Union[list, "Temque"]):
+    def __add__(self, obj: 'list|Temque'):
         que = self.copy()
         if isinstance(obj, self.__class__):
             que.core += obj.core
             que._trim()
         else:
             que.add_many(*obj)
         return que
@@ -105,40 +105,43 @@
     * [获取链接2](https://www.baidu.com/s?wd=%E8%8E%B7%E5%8F%96%20openai%20api_key)
     """
     
     recently_request_data: dict  # 最近一次请求所用的参数
 
     def __init__(self,
                  # kwargs
-                 api_key: Union[str, AKPool],
+                 api_key: str|AKPool,
                  base_url: str = None,  # base_url 参数用于修改基础URL
                  timeout=None,
                  max_retries=None,
                  http_client=None,
                  # request_kwargs
                  model: Literal["gpt-4-1106-preview", "gpt-4-vision-preview", "gpt-4", "gpt-4-0314", "gpt-4-0613",
                                 "gpt-4-32k", "gpt-4-32k-0314", "gpt-4-32k-0613", "gpt-3.5-turbo"] = "gpt-3.5-turbo",
                  # Chat
-                 MsgMaxCount=None,
+                 msg_max_count: int=None,
                  # kwargs
                  **kwargs,
                  ):
         api_base = kwargs.pop('api_base', None)
+        base_url = base_url or api_base
+        MsgMaxCount = kwargs.pop('MsgMaxCount', None)
+        msg_max_count = msg_max_count or MsgMaxCount
 
-        if base_url or api_base: kwargs["base_url"] = base_url or api_base
+        if base_url: kwargs["base_url"] = base_url
         if timeout: kwargs["timeout"] = timeout
         if max_retries: kwargs["max_retries"] = max_retries
         if http_client: kwargs["http_client"] = http_client
 
         self.reset_api_key(api_key)
         self._kwargs = kwargs
         self._request_kwargs = {'model':model}
-        self._messages = Temque(maxlen=MsgMaxCount)
+        self._messages = Temque(maxlen=msg_max_count)
     
-    def reset_api_key(self, api_key: Union[str, AKPool]):
+    def reset_api_key(self, api_key: str|AKPool):
         if isinstance(api_key, AKPool):
             self._akpool = api_key
         else:
             self._akpool = AKPool([api_key])
 
     def request(self, text: str=None, **kwargs):
         messages = [{"role": "user", "content": text}]
@@ -211,47 +214,64 @@
         async for chunk in completion:
             if chunk.choices and (content := chunk.choices[0].delta.content):
                 answer += content
                 yield content
         self._messages.add_many(*messages, {"role": "assistant", "content": answer})
 
     def rollback(self, n=1):
+        '''
+        回滚对话
+        '''
         self._messages.core[-2 * n :] = []
         for x in self._messages.core[-2:]:
             x = x["obj"]
             print(f"[{x['role']}]:{x['content']}")
 
     def pin_messages(self, *indexes):
+        '''
+        锁定历史消息
+        '''
         self._messages.pin(*indexes)
 
     def unpin_messages(self, *indexes):
+        '''
+        解锁历史消息
+        '''
         self._messages.unpin(*indexes)
     
     def fetch_messages(self):
         return list(self._messages)
     
-    def add_dialogs(self, *ms: Union[system_msg, user_msg, assistant_msg, dict]):
+    def add_dialogs(self, *ms: dict|system_msg|user_msg|assistant_msg):
         '''
         添加历史对话
         '''
         messages = [dict(x) for x in ms]
         self._messages.add_many(*messages)
-    
-    asy_request = async_request  # 兼容旧代码
-
-    forge = add_dialogs  # 兼容旧代码
+        
+    def __getattr__(self, name):
+        match name:  # 兼容旧代码
+            case 'asy_request':
+                return self.async_request
+            case 'forge':
+                return self.add_dialogs
+            case 'pin':
+                return self.pin_messages
+            case 'unpin':
+                return self.unpin_messages
+            case 'dump':
+                return self._dump
+            case 'load':
+                return self._load
+        raise AttributeError(name)
 
-    pin = pin_messages  # 兼容旧代码
-
-    unpin = unpin_messages  # 兼容旧代码
-    
-    def dump(self, fpath: str):  # 兼容旧代码
+    def _dump(self, fpath: str):
         """ 存档 """
         jt = jsonDumps(self.fetch_messages(), ensure_ascii=False)
         Path(fpath).write_text(jt, encoding="utf8")
         return True
     
-    def load(self, fpath: str):  # 兼容旧代码
+    def _load(self, fpath: str):
         """ 载入存档 """
         jt = Path(fpath).read_text(encoding="utf8")
         self._messages.add_many(*jsonLoads(jt))
         return True
```

### Comparing `openai2-1.7.1/_core/chat_in_cmd.py` & `openai2-1.7.2/_core/chat_in_cmd.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 mdb = moduledb.DB(openai2, depth=3)['chat_in_cmd']
 apikeys: moduledb.File = mdb['apikeys']['data_1']
 apikeys.setdefault('list', [])
 record: moduledb.File = mdb['records']['chat_1']
 record.setdefault('messages', [])
 
 
-def chat_in_cmd(apikeys:list, newchat=False, model='gpt-4-1106-preview', MsgMaxCount=30):
+def chat_in_cmd(apikeys:list, newchat=False, model='gpt-4-1106-preview', msg_max_count=30):
     print(f"\n\033[0m您已进入命令行聊天模式, 当前使用'{model}'模型, 请确保您的apikey支持该模型.", end='')
-    gpt = Chat(api_key=AKPool(apikeys), model=model, MsgMaxCount=MsgMaxCount)
+    gpt = Chat(api_key=AKPool(apikeys), model=model, msg_max_count=msg_max_count)
     if not newchat:
         gpt.add_dialogs(*record['messages'])
     while True:
         user = input('\n\n\033[32;1m:')
         print('\033[0m')
         for x in gpt.stream_request(user):
             print(x, end='', flush=True)
```

### Comparing `openai2-1.7.1/licenses/openai/LICENSE` & `openai2-1.7.2/licenses/openai/LICENSE`

 * *Files identical despite different names*

### Comparing `openai2-1.7.1/pyproject.toml` & `openai2-1.7.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "openai2"
-version = "1.7.1"
+version = "1.7.2"
 description = "ChatGPT 工具包，支持连续对话、流式对话（逐字显示）、对话存档与载入、对话回滚、对话伪造、轮询 api_key 池、群聊多角色模拟、在命令行对话、限制历史消息数量、异步请求。"
-dependencies = ["arts>=2024.4.3.1"]
+dependencies = ["arts>=2024.4.3.2"]
 keywords = ["openai", "chatgpt", "openai2"]
 
 
 readme = "README.md"
 authors = [{name = "江南雨上", email = "lcctoor@outlook.com"}]
 license = {file = "LICENSE"}
 classifiers = ["License :: OSI Approved :: Apache Software License"]
```

### Comparing `openai2-1.7.1/PKG-INFO` & `openai2-1.7.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: openai2
-Version: 1.7.1
+Version: 1.7.2
 Summary: ChatGPT 工具包，支持连续对话、流式对话（逐字显示）、对话存档与载入、对话回滚、对话伪造、轮询 api_key 池、群聊多角色模拟、在命令行对话、限制历史消息数量、异步请求。
 Keywords: openai,chatgpt,openai2
 Author-email: 江南雨上 <lcctoor@outlook.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
-Requires-Dist: arts>=2024.4.3.1
+Requires-Dist: arts>=2024.4.3.2
 Project-URL: HomePage, https://github.com/lcctoor/arts/tree/main/arts/openai2
 
 # 项目描述
 
 ChatGPT 工具包，支持连续对话、流式对话（逐字显示）、对话存档与载入、对话回滚、对话伪造、轮询 api_key 池、群聊多角色模拟、在命令行对话、限制历史消息数量、异步请求。
 
 # 作者
@@ -294,20 +294,20 @@
 ]
 ```
 
 ## 限制历史消息数量
 
 ### 限制历史消息数量
 
-随着对话次数越来越多，最终上下文长度就会超出 openai 接口限定的最大 token 数量，此时可使用 MsgMaxCount 参数来限制历史消息数量。当消息数量超出 MsgMaxCount 后，程序会自动移除最早的记录，使消息数量减少到恰好等于 MsgMaxCount 。
+随着对话次数越来越多，最终上下文长度就会超出 openai 接口限定的最大 token 数量，此时可使用 msg_max_count 参数来限制历史消息数量。当消息数量超出 msg_max_count 后，程序会自动移除最早的记录，使消息数量减少到恰好等于 msg_max_count 。
 
 ```python
-MsgMaxCount = 6  # 最多保留6条历史消息
+msg_max_count = 6  # 最多保留6条历史消息
 
-Ariel = Chat(api_key=api_key, model="gpt-3.5-turbo", MsgMaxCount=MsgMaxCount)
+Ariel = Chat(api_key=api_key, model="gpt-3.5-turbo", msg_max_count=msg_max_count)
 
 Ariel.request('英国的首都是什么？')  # >>> '伦敦'
 Ariel.request('日本首都是什么？')  # >>> '东京'
 Ariel.request('意大利的首都是什么？')  # >>> '罗马'
 Ariel.request('美国的首都是什么？')  # >>> '华盛顿'
 Ariel.request('世界上国土面积最大的国家是哪个？')  # >>> '俄罗斯'
 Ariel.request('法国的首都叫什么？')  # >>> '巴黎'
@@ -328,17 +328,17 @@
 ```
 
 ### 锁定消息
 
 当程序自动移除消息记录时，也许我们希望某些消息不要被移除，此时可将这些消息锁定。
 
 ```python
-MsgMaxCount = 6
+msg_max_count = 6
 
-Ariel = Chat(api_key=api_key, model="gpt-3.5-turbo", MsgMaxCount=MsgMaxCount)
+Ariel = Chat(api_key=api_key, model="gpt-3.5-turbo", msg_max_count=msg_max_count)
 
 Ariel.request('英国的首都是什么？')  # >>> '伦敦'
 Ariel.request('日本首都是什么？')  # >>> '东京'
 Ariel.request('意大利的首都是什么？')  # >>> '罗马'
 ```
 
 此时共有 6 条消息记录：
@@ -360,15 +360,15 @@
 
 继续请求：
 
 ```python
 Ariel.request('美国的首都是什么？')  # >>> '华盛顿'
 ```
 
-由于设置了 MsgMaxCount = 6，此时共有 6 条消息记录：
+由于设置了 msg_max_count = 6，此时共有 6 条消息记录：
 
 | 消息                 | 正序索引 | 逆序索引 | 锁定状态 |
 | -------------------- | :------: | :------: | :------: |
 | 英国的首都是什么？   |    0    |    -6    |  已锁定  |
 | 东京                 |    1    |    -5    |    -    |
 | 意大利的首都是什么？ |    2    |    -4    |  已锁定  |
 | 罗马                 |    3    |    -3    |  已锁定  |
```

