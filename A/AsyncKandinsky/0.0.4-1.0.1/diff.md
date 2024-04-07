# Comparing `tmp/AsyncKandinsky-0.0.4.tar.gz` & `tmp/AsyncKandinsky-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/AsyncKandinsky-0.0.4.tar", last modified: Sun Apr  7 10:27:27 2024, max compression
+gzip compressed data, was "dist/AsyncKandinsky-1.0.1.tar", last modified: Sun Apr  7 16:14:28 2024, max compression
```

## Comparing `AsyncKandinsky-0.0.4.tar` & `AsyncKandinsky-1.0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 s1rne      (503) staff       (20)        0 2024-04-07 10:27:27.662423 AsyncKandinsky-0.0.4/
-drwxr-xr-x   0 s1rne      (503) staff       (20)        0 2024-04-07 10:27:27.656975 AsyncKandinsky-0.0.4/AsyncKandinsky/
--rw-r--r--   0 s1rne      (503) staff       (20)      346 2024-04-07 09:57:30.000000 AsyncKandinsky-0.0.4/AsyncKandinsky/API_types.py
--rw-r--r--   0 s1rne      (503) staff       (20)      388 2024-04-07 09:57:30.000000 AsyncKandinsky-0.0.4/AsyncKandinsky/URLS.py
--rw-r--r--   0 s1rne      (503) staff       (20)       57 2024-04-07 10:03:51.000000 AsyncKandinsky-0.0.4/AsyncKandinsky/__init__.py
--rw-r--r--   0 s1rne      (503) staff       (20)     3715 2024-04-07 10:27:11.000000 AsyncKandinsky-0.0.4/AsyncKandinsky/api.py
-drwxr-xr-x   0 s1rne      (503) staff       (20)        0 2024-04-07 10:27:27.661420 AsyncKandinsky-0.0.4/AsyncKandinsky.egg-info/
--rw-r--r--   0 s1rne      (503) staff       (20)     2513 2024-04-07 10:27:27.000000 AsyncKandinsky-0.0.4/AsyncKandinsky.egg-info/PKG-INFO
--rw-r--r--   0 s1rne      (503) staff       (20)      317 2024-04-07 10:27:27.000000 AsyncKandinsky-0.0.4/AsyncKandinsky.egg-info/SOURCES.txt
--rw-r--r--   0 s1rne      (503) staff       (20)        1 2024-04-07 10:27:27.000000 AsyncKandinsky-0.0.4/AsyncKandinsky.egg-info/dependency_links.txt
--rw-r--r--   0 s1rne      (503) staff       (20)       30 2024-04-07 10:27:27.000000 AsyncKandinsky-0.0.4/AsyncKandinsky.egg-info/requires.txt
--rw-r--r--   0 s1rne      (503) staff       (20)       15 2024-04-07 10:27:27.000000 AsyncKandinsky-0.0.4/AsyncKandinsky.egg-info/top_level.txt
--rw-r--r--   0 s1rne      (503) staff       (20)     2513 2024-04-07 10:27:27.662189 AsyncKandinsky-0.0.4/PKG-INFO
--rw-r--r--   0 s1rne      (503) staff       (20)     1845 2024-04-07 10:27:11.000000 AsyncKandinsky-0.0.4/README.md
--rw-r--r--   0 s1rne      (503) staff       (20)       38 2024-04-07 10:27:27.663143 AsyncKandinsky-0.0.4/setup.cfg
--rw-r--r--   0 s1rne      (503) staff       (20)      940 2024-04-07 10:27:11.000000 AsyncKandinsky-0.0.4/setup.py
+drwxr-xr-x   0 s1rne      (503) staff       (20)        0 2024-04-07 16:14:28.240215 AsyncKandinsky-1.0.1/
+drwxr-xr-x   0 s1rne      (503) staff       (20)        0 2024-04-07 16:14:28.235658 AsyncKandinsky-1.0.1/AsyncKandinsky/
+-rw-r--r--   0 s1rne      (503) staff       (20)     2198 2024-04-07 16:02:44.000000 AsyncKandinsky-1.0.1/AsyncKandinsky/API_types.py
+-rw-r--r--   0 s1rne      (503) staff       (20)      683 2024-04-07 16:01:35.000000 AsyncKandinsky-1.0.1/AsyncKandinsky/URLS.py
+-rw-r--r--   0 s1rne      (503) staff       (20)       57 2024-04-07 10:03:51.000000 AsyncKandinsky-1.0.1/AsyncKandinsky/__init__.py
+-rw-r--r--   0 s1rne      (503) staff       (20)     3135 2024-04-07 16:12:43.000000 AsyncKandinsky-1.0.1/AsyncKandinsky/api.py
+drwxr-xr-x   0 s1rne      (503) staff       (20)        0 2024-04-07 16:14:28.239209 AsyncKandinsky-1.0.1/AsyncKandinsky.egg-info/
+-rw-r--r--   0 s1rne      (503) staff       (20)     2870 2024-04-07 16:14:28.000000 AsyncKandinsky-1.0.1/AsyncKandinsky.egg-info/PKG-INFO
+-rw-r--r--   0 s1rne      (503) staff       (20)      317 2024-04-07 16:14:28.000000 AsyncKandinsky-1.0.1/AsyncKandinsky.egg-info/SOURCES.txt
+-rw-r--r--   0 s1rne      (503) staff       (20)        1 2024-04-07 16:14:28.000000 AsyncKandinsky-1.0.1/AsyncKandinsky.egg-info/dependency_links.txt
+-rw-r--r--   0 s1rne      (503) staff       (20)       30 2024-04-07 16:14:28.000000 AsyncKandinsky-1.0.1/AsyncKandinsky.egg-info/requires.txt
+-rw-r--r--   0 s1rne      (503) staff       (20)       15 2024-04-07 16:14:28.000000 AsyncKandinsky-1.0.1/AsyncKandinsky.egg-info/top_level.txt
+-rw-r--r--   0 s1rne      (503) staff       (20)     2870 2024-04-07 16:14:28.239924 AsyncKandinsky-1.0.1/PKG-INFO
+-rw-r--r--   0 s1rne      (503) staff       (20)     2202 2024-04-07 16:12:43.000000 AsyncKandinsky-1.0.1/README.md
+-rw-r--r--   0 s1rne      (503) staff       (20)       38 2024-04-07 16:14:28.241047 AsyncKandinsky-1.0.1/setup.cfg
+-rw-r--r--   0 s1rne      (503) staff       (20)      940 2024-04-07 16:14:25.000000 AsyncKandinsky-1.0.1/setup.py
```

### Comparing `AsyncKandinsky-0.0.4/AsyncKandinsky/api.py` & `AsyncKandinsky-1.0.1/AsyncKandinsky/api.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,53 +4,32 @@
 import base64
 import json
 import time
 from io import BytesIO
 
 import aiohttp
 
-from API_types import ApiApi, ApiWeb
-from URLS import ApiUrls, WebUrls
+from .API_types import ApiApi, ApiWeb
 
 
 class FusionBrainApi:
     url_get_styles = "https://cdn.fusionbrain.ai/static/styles/$api_type"
 
-    models_api_type = {
-        "api": {
-            "3.0": "4"
-        },
-        "web": {
-            "3.0": "1"
-        }
-    }
-
     def __init__(self, api: ApiApi | ApiWeb):
         if hasattr(api, "type"):
-            if api.type == "api":
-                self.api_headers = {
-                    "X-Key": f"Key {api.api_key}",
-                    "X-Secret": f"Secret {api.secret_key}",
-                }
-                self.api_type = api.type
-                self.urls = ApiUrls
-            elif api.type == "web":
-                self.api_headers = {
-                    "Authorization": api.authorization
-                }
-                self.api_type = api.type
-                self.urls = WebUrls
+            if api.type not in [ApiApi.type, ApiWeb.type]:
+                raise TypeError("Invalid API type")
             else:
-                raise TypeError("Invalid API")
+                self.api = api
         else:
-            raise TypeError("Invalid API type")
+            raise TypeError("Invalid API structure")
 
     async def get_styles(self) -> dict:
         async with aiohttp.ClientSession() as session:
-            n_url = self.url_get_styles.replace("$api_type", self.api_type)
+            n_url = self.url_get_styles.replace("$api_type", self.api.type)
             async with session.get(n_url) as response:
                 return await response.json()
 
     async def text2image(self,
                          prompt: str = "",
                          negative_prompt: str = "",
                          style: str = "DEFAULT",
@@ -71,32 +50,31 @@
         }
 
         data = aiohttp.FormData()
         data.add_field("params",
                        json.dumps(params),
                        content_type="application/json",
                        )
-        data.add_field("model_id", self.models_api_type[self.api_type][model])
+        data.add_field("model_id", self.api.model_numbers[model])
 
         async with aiohttp.ClientSession() as session:
-            n_url = self.urls.url_text2image_run
-            async with session.post(n_url, data=data, headers=self.api_headers) as resp:
+            n_url = self.api.urls.url_text2image_run
+            async with session.post(n_url, data=data, headers=await self.api.get_headers()) as resp:
                 result = await resp.json()
 
         if "error" in result:
             return {"error": True, "data": result}
 
         uuid = result["uuid"]
         start_time = time.time()
         while time.time() - (start_time + max_time) < 0:
             async with aiohttp.ClientSession() as session:
-                n_url = self.urls.url_text2_image_status.replace("$uuid", uuid)
-                async with session.get(n_url, headers=self.api_headers) as resp:
+                n_url = self.api.urls.url_text2_image_status.replace("$uuid", uuid)
+                async with session.get(n_url, headers=await self.api.get_headers()) as resp:
                     result = await resp.json()
-                    print(result)
                     if result["status"] == "DONE":
                         if result["censored"]:
                             return {"error": True, "data": "censored: is True"}
                         else:
                             return {"error": False, "data": BytesIO(base64.b64decode(result["images"][0]))}
                     elif result["status"] == "FAIL":
                         return {"error": True, "data": f"status is FAIL: {result['status']}"}
```

### Comparing `AsyncKandinsky-0.0.4/AsyncKandinsky.egg-info/PKG-INFO` & `AsyncKandinsky-1.0.1/AsyncKandinsky.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AsyncKandinsky
-Version: 0.0.4
+Version: 1.0.1
 Summary: This module is designed for asynchronous use of the kandinsky neural network and easy integration into your project.
 Home-page: https://github.com/s1rne/kandinsky-async-api
 Author: s1rne
 Author-email: s.simaranov8@gmail.com
 Project-URL: GitHub, https://github.com/s1rne/kandinsky-async-api
 Keywords: kandinsky text2img async api
 Classifier: Programming Language :: Python :: 3.9
@@ -18,28 +18,34 @@
 # kandinsky-api-requests
 
 **Асинхронное** api для использования kandinsky 3.0
 
 ВНИМАНИЕ: После изменения структуры сайта, сделана api только по их ключам. Планируется отревёрсить использование web версии программно.
 
 ### **Как использовать:**
-##### Установка: pip install AsyncKandinsky
+##### Установка: `pip install AsyncKandinsky`
 
 ### Для инициализации FusionBrainApi можно использовать keys или данные аккаунта:
- + api_key и secret_key - их надо создать во вкладе api (https://fusionbrain.ai/keys/):
+ + api_key и secret_key:
+   + **!!! Ключи создаются в вкладке api (https://fusionbrain.ai/keys/)**
    + быстрый и простой способ генерации 
- + почта и пароль - данные от уже созданного аккаунта {пока в разработке}:
-   + в такой версии будет доступна генерация: **видео / анимации / больше стилей**
+   + не самое лучше качество генерации
+ + почта и пароль - данные от уже созданного аккаунта:
+   + **!!! Обязательно нужен уже зарегистрированный аккаунт**
+   + в такой версии будет доступна генерация: **видео / анимации / больше стилей** {В процесса разработки}
+   + лучшее качество генерации
 ###### *Полный пример можно посмотреть в tests.py (GitHub)*
 
 
 ### 1. text2image
 
 ```
 model = FusionBrainApi(ApiApi(api_key, secret_key))
+# Любой способ на выбор
+model = FusionBrainApi(ApiWeb("Ваша почта", "Ваш пароль"))
 
 
 async def generate():
     result = await model.text2image("котик", style="ANIME")
     if result["error"]:
         print("Error:")
         print(result["data"])
@@ -54,11 +60,11 @@
 ```
 
 Все стили можно посмотреть в `await FusionBrainApi().get_styles()`:
 
 ```
 async def read_styles():
     for style in await model.get_styles():
-        print(style, end="\n\n")
+        print(style)
 ```
 
 ![Пример генерации](https://github.com/s1rne/kandinsky-async-api/blob/main/cat_anime.jpg)
```

### Comparing `AsyncKandinsky-0.0.4/PKG-INFO` & `AsyncKandinsky-1.0.1/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AsyncKandinsky
-Version: 0.0.4
+Version: 1.0.1
 Summary: This module is designed for asynchronous use of the kandinsky neural network and easy integration into your project.
 Home-page: https://github.com/s1rne/kandinsky-async-api
 Author: s1rne
 Author-email: s.simaranov8@gmail.com
 Project-URL: GitHub, https://github.com/s1rne/kandinsky-async-api
 Keywords: kandinsky text2img async api
 Classifier: Programming Language :: Python :: 3.9
@@ -18,28 +18,34 @@
 # kandinsky-api-requests
 
 **Асинхронное** api для использования kandinsky 3.0
 
 ВНИМАНИЕ: После изменения структуры сайта, сделана api только по их ключам. Планируется отревёрсить использование web версии программно.
 
 ### **Как использовать:**
-##### Установка: pip install AsyncKandinsky
+##### Установка: `pip install AsyncKandinsky`
 
 ### Для инициализации FusionBrainApi можно использовать keys или данные аккаунта:
- + api_key и secret_key - их надо создать во вкладе api (https://fusionbrain.ai/keys/):
+ + api_key и secret_key:
+   + **!!! Ключи создаются в вкладке api (https://fusionbrain.ai/keys/)**
    + быстрый и простой способ генерации 
- + почта и пароль - данные от уже созданного аккаунта {пока в разработке}:
-   + в такой версии будет доступна генерация: **видео / анимации / больше стилей**
+   + не самое лучше качество генерации
+ + почта и пароль - данные от уже созданного аккаунта:
+   + **!!! Обязательно нужен уже зарегистрированный аккаунт**
+   + в такой версии будет доступна генерация: **видео / анимации / больше стилей** {В процесса разработки}
+   + лучшее качество генерации
 ###### *Полный пример можно посмотреть в tests.py (GitHub)*
 
 
 ### 1. text2image
 
 ```
 model = FusionBrainApi(ApiApi(api_key, secret_key))
+# Любой способ на выбор
+model = FusionBrainApi(ApiWeb("Ваша почта", "Ваш пароль"))
 
 
 async def generate():
     result = await model.text2image("котик", style="ANIME")
     if result["error"]:
         print("Error:")
         print(result["data"])
@@ -54,11 +60,11 @@
 ```
 
 Все стили можно посмотреть в `await FusionBrainApi().get_styles()`:
 
 ```
 async def read_styles():
     for style in await model.get_styles():
-        print(style, end="\n\n")
+        print(style)
 ```
 
 ![Пример генерации](https://github.com/s1rne/kandinsky-async-api/blob/main/cat_anime.jpg)
```

### Comparing `AsyncKandinsky-0.0.4/README.md` & `AsyncKandinsky-1.0.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,34 @@
 # kandinsky-api-requests
 
 **Асинхронное** api для использования kandinsky 3.0
 
 ВНИМАНИЕ: После изменения структуры сайта, сделана api только по их ключам. Планируется отревёрсить использование web версии программно.
 
 ### **Как использовать:**
-##### Установка: pip install AsyncKandinsky
+##### Установка: `pip install AsyncKandinsky`
 
 ### Для инициализации FusionBrainApi можно использовать keys или данные аккаунта:
- + api_key и secret_key - их надо создать во вкладе api (https://fusionbrain.ai/keys/):
+ + api_key и secret_key:
+   + **!!! Ключи создаются в вкладке api (https://fusionbrain.ai/keys/)**
    + быстрый и простой способ генерации 
- + почта и пароль - данные от уже созданного аккаунта {пока в разработке}:
-   + в такой версии будет доступна генерация: **видео / анимации / больше стилей**
+   + не самое лучше качество генерации
+ + почта и пароль - данные от уже созданного аккаунта:
+   + **!!! Обязательно нужен уже зарегистрированный аккаунт**
+   + в такой версии будет доступна генерация: **видео / анимации / больше стилей** {В процесса разработки}
+   + лучшее качество генерации
 ###### *Полный пример можно посмотреть в tests.py (GitHub)*
 
 
 ### 1. text2image
 
 ```
 model = FusionBrainApi(ApiApi(api_key, secret_key))
+# Любой способ на выбор
+model = FusionBrainApi(ApiWeb("Ваша почта", "Ваш пароль"))
 
 
 async def generate():
     result = await model.text2image("котик", style="ANIME")
     if result["error"]:
         print("Error:")
         print(result["data"])
@@ -37,11 +43,11 @@
 ```
 
 Все стили можно посмотреть в `await FusionBrainApi().get_styles()`:
 
 ```
 async def read_styles():
     for style in await model.get_styles():
-        print(style, end="\n\n")
+        print(style)
 ```
 
 ![Пример генерации](https://github.com/s1rne/kandinsky-async-api/blob/main/cat_anime.jpg)
```

### Comparing `AsyncKandinsky-0.0.4/setup.py` & `AsyncKandinsky-1.0.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def readme():
     with open('README.md', 'r') as f:
         return f.read()
 
 
 setup(
     name='AsyncKandinsky',
-    version='0.0.4',
+    version='1.0.1',
     author='s1rne',
     author_email='s.simaranov8@gmail.com',
     description='This module is designed for asynchronous use of the kandinsky neural network and easy integration into your project.',
     long_description=readme(),
     long_description_content_type='text/markdown',
     url='https://github.com/s1rne/kandinsky-async-api',
     packages=find_packages(),
```

