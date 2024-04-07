# Comparing `tmp/AsyncKandinsky-0.0.3.tar.gz` & `tmp/AsyncKandinsky-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/AsyncKandinsky-0.0.3.tar", last modified: Sun Apr  7 10:03:53 2024, max compression
+gzip compressed data, was "dist/AsyncKandinsky-0.0.4.tar", last modified: Sun Apr  7 10:27:27 2024, max compression
```

## Comparing `AsyncKandinsky-0.0.3.tar` & `AsyncKandinsky-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 s1rne      (503) staff       (20)        0 2024-04-07 10:03:53.020861 AsyncKandinsky-0.0.3/
-drwxr-xr-x   0 s1rne      (503) staff       (20)        0 2024-04-07 10:03:53.014455 AsyncKandinsky-0.0.3/AsyncKandinsky/
--rw-r--r--   0 s1rne      (503) staff       (20)      346 2024-04-07 09:57:30.000000 AsyncKandinsky-0.0.3/AsyncKandinsky/API_types.py
--rw-r--r--   0 s1rne      (503) staff       (20)      388 2024-04-07 09:57:30.000000 AsyncKandinsky-0.0.3/AsyncKandinsky/URLS.py
--rw-r--r--   0 s1rne      (503) staff       (20)       57 2024-04-07 10:03:51.000000 AsyncKandinsky-0.0.3/AsyncKandinsky/__init__.py
--rw-r--r--   0 s1rne      (503) staff       (20)     3717 2024-04-07 09:57:30.000000 AsyncKandinsky-0.0.3/AsyncKandinsky/api.py
-drwxr-xr-x   0 s1rne      (503) staff       (20)        0 2024-04-07 10:03:53.019568 AsyncKandinsky-0.0.3/AsyncKandinsky.egg-info/
--rw-r--r--   0 s1rne      (503) staff       (20)     1859 2024-04-07 10:03:52.000000 AsyncKandinsky-0.0.3/AsyncKandinsky.egg-info/PKG-INFO
--rw-r--r--   0 s1rne      (503) staff       (20)      317 2024-04-07 10:03:52.000000 AsyncKandinsky-0.0.3/AsyncKandinsky.egg-info/SOURCES.txt
--rw-r--r--   0 s1rne      (503) staff       (20)        1 2024-04-07 10:03:52.000000 AsyncKandinsky-0.0.3/AsyncKandinsky.egg-info/dependency_links.txt
--rw-r--r--   0 s1rne      (503) staff       (20)       30 2024-04-07 10:03:52.000000 AsyncKandinsky-0.0.3/AsyncKandinsky.egg-info/requires.txt
--rw-r--r--   0 s1rne      (503) staff       (20)       15 2024-04-07 10:03:52.000000 AsyncKandinsky-0.0.3/AsyncKandinsky.egg-info/top_level.txt
--rw-r--r--   0 s1rne      (503) staff       (20)     1859 2024-04-07 10:03:53.020530 AsyncKandinsky-0.0.3/PKG-INFO
--rw-r--r--   0 s1rne      (503) staff       (20)     1191 2024-04-07 10:00:00.000000 AsyncKandinsky-0.0.3/README.md
--rw-r--r--   0 s1rne      (503) staff       (20)       38 2024-04-07 10:03:53.022036 AsyncKandinsky-0.0.3/setup.cfg
--rw-r--r--   0 s1rne      (503) staff       (20)      940 2024-04-07 10:03:51.000000 AsyncKandinsky-0.0.3/setup.py
+drwxr-xr-x   0 s1rne      (503) staff       (20)        0 2024-04-07 10:27:27.662423 AsyncKandinsky-0.0.4/
+drwxr-xr-x   0 s1rne      (503) staff       (20)        0 2024-04-07 10:27:27.656975 AsyncKandinsky-0.0.4/AsyncKandinsky/
+-rw-r--r--   0 s1rne      (503) staff       (20)      346 2024-04-07 09:57:30.000000 AsyncKandinsky-0.0.4/AsyncKandinsky/API_types.py
+-rw-r--r--   0 s1rne      (503) staff       (20)      388 2024-04-07 09:57:30.000000 AsyncKandinsky-0.0.4/AsyncKandinsky/URLS.py
+-rw-r--r--   0 s1rne      (503) staff       (20)       57 2024-04-07 10:03:51.000000 AsyncKandinsky-0.0.4/AsyncKandinsky/__init__.py
+-rw-r--r--   0 s1rne      (503) staff       (20)     3715 2024-04-07 10:27:11.000000 AsyncKandinsky-0.0.4/AsyncKandinsky/api.py
+drwxr-xr-x   0 s1rne      (503) staff       (20)        0 2024-04-07 10:27:27.661420 AsyncKandinsky-0.0.4/AsyncKandinsky.egg-info/
+-rw-r--r--   0 s1rne      (503) staff       (20)     2513 2024-04-07 10:27:27.000000 AsyncKandinsky-0.0.4/AsyncKandinsky.egg-info/PKG-INFO
+-rw-r--r--   0 s1rne      (503) staff       (20)      317 2024-04-07 10:27:27.000000 AsyncKandinsky-0.0.4/AsyncKandinsky.egg-info/SOURCES.txt
+-rw-r--r--   0 s1rne      (503) staff       (20)        1 2024-04-07 10:27:27.000000 AsyncKandinsky-0.0.4/AsyncKandinsky.egg-info/dependency_links.txt
+-rw-r--r--   0 s1rne      (503) staff       (20)       30 2024-04-07 10:27:27.000000 AsyncKandinsky-0.0.4/AsyncKandinsky.egg-info/requires.txt
+-rw-r--r--   0 s1rne      (503) staff       (20)       15 2024-04-07 10:27:27.000000 AsyncKandinsky-0.0.4/AsyncKandinsky.egg-info/top_level.txt
+-rw-r--r--   0 s1rne      (503) staff       (20)     2513 2024-04-07 10:27:27.662189 AsyncKandinsky-0.0.4/PKG-INFO
+-rw-r--r--   0 s1rne      (503) staff       (20)     1845 2024-04-07 10:27:11.000000 AsyncKandinsky-0.0.4/README.md
+-rw-r--r--   0 s1rne      (503) staff       (20)       38 2024-04-07 10:27:27.663143 AsyncKandinsky-0.0.4/setup.cfg
+-rw-r--r--   0 s1rne      (503) staff       (20)      940 2024-04-07 10:27:11.000000 AsyncKandinsky-0.0.4/setup.py
```

### Comparing `AsyncKandinsky-0.0.3/AsyncKandinsky/api.py` & `AsyncKandinsky-0.0.4/AsyncKandinsky/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
                 self.api_type = api.type
                 self.urls = WebUrls
             else:
                 raise TypeError("Invalid API")
         else:
             raise TypeError("Invalid API type")
 
-    async def get_styles(self) -> ApiApi:
+    async def get_styles(self) -> dict:
         async with aiohttp.ClientSession() as session:
             n_url = self.url_get_styles.replace("$api_type", self.api_type)
             async with session.get(n_url) as response:
                 return await response.json()
 
     async def text2image(self,
                          prompt: str = "",
```

### Comparing `AsyncKandinsky-0.0.3/AsyncKandinsky.egg-info/PKG-INFO` & `AsyncKandinsky-0.0.4/AsyncKandinsky.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AsyncKandinsky
-Version: 0.0.3
+Version: 0.0.4
 Summary: This module is designed for asynchronous use of the kandinsky neural network and easy integration into your project.
 Home-page: https://github.com/s1rne/kandinsky-async-api
 Author: s1rne
 Author-email: s.simaranov8@gmail.com
 Project-URL: GitHub, https://github.com/s1rne/kandinsky-async-api
 Keywords: kandinsky text2img async api
 Classifier: Programming Language :: Python :: 3.9
@@ -13,25 +13,33 @@
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Requires-Dist: aiohttp>=3.8.4
 Requires-Dist: Pillow>=10.0.0
 
 # kandinsky-api-requests
 
-**Асионхронное** api для использования нейросети kandinsky 3.0
+**Асинхронное** api для использования kandinsky 3.0
 
-ВНИМАНИЕ: После изменнеия структуры сайта, сделана работа только для api версии. Планируется "взломать" использование web версии программно.
+ВНИМАНИЕ: После изменения структуры сайта, сделана api только по их ключам. Планируется отревёрсить использование web версии программно.
+
+### **Как использовать:**
+##### Установка: pip install AsyncKandinsky
+
+### Для инициализации FusionBrainApi можно использовать keys или данные аккаунта:
+ + api_key и secret_key - их надо создать во вкладе api (https://fusionbrain.ai/keys/):
+   + быстрый и простой способ генерации 
+ + почта и пароль - данные от уже созданного аккаунта {пока в разработке}:
+   + в такой версии будет доступна генерация: **видео / анимации / больше стилей**
+###### *Полный пример можно посмотреть в tests.py (GitHub)*
 
-**Как использовать:**
-###### *полный пример можно посмотреть в tests.py*
 
 ### 1. text2image
 
 ```
-model = FusionBrainApi()
+model = FusionBrainApi(ApiApi(api_key, secret_key))
 
 
 async def generate():
     result = await model.text2image("котик", style="ANIME")
     if result["error"]:
         print("Error:")
         print(result["data"])
```

### Comparing `AsyncKandinsky-0.0.3/PKG-INFO` & `AsyncKandinsky-0.0.4/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AsyncKandinsky
-Version: 0.0.3
+Version: 0.0.4
 Summary: This module is designed for asynchronous use of the kandinsky neural network and easy integration into your project.
 Home-page: https://github.com/s1rne/kandinsky-async-api
 Author: s1rne
 Author-email: s.simaranov8@gmail.com
 Project-URL: GitHub, https://github.com/s1rne/kandinsky-async-api
 Keywords: kandinsky text2img async api
 Classifier: Programming Language :: Python :: 3.9
@@ -13,25 +13,33 @@
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Requires-Dist: aiohttp>=3.8.4
 Requires-Dist: Pillow>=10.0.0
 
 # kandinsky-api-requests
 
-**Асионхронное** api для использования нейросети kandinsky 3.0
+**Асинхронное** api для использования kandinsky 3.0
 
-ВНИМАНИЕ: После изменнеия структуры сайта, сделана работа только для api версии. Планируется "взломать" использование web версии программно.
+ВНИМАНИЕ: После изменения структуры сайта, сделана api только по их ключам. Планируется отревёрсить использование web версии программно.
+
+### **Как использовать:**
+##### Установка: pip install AsyncKandinsky
+
+### Для инициализации FusionBrainApi можно использовать keys или данные аккаунта:
+ + api_key и secret_key - их надо создать во вкладе api (https://fusionbrain.ai/keys/):
+   + быстрый и простой способ генерации 
+ + почта и пароль - данные от уже созданного аккаунта {пока в разработке}:
+   + в такой версии будет доступна генерация: **видео / анимации / больше стилей**
+###### *Полный пример можно посмотреть в tests.py (GitHub)*
 
-**Как использовать:**
-###### *полный пример можно посмотреть в tests.py*
 
 ### 1. text2image
 
 ```
-model = FusionBrainApi()
+model = FusionBrainApi(ApiApi(api_key, secret_key))
 
 
 async def generate():
     result = await model.text2image("котик", style="ANIME")
     if result["error"]:
         print("Error:")
         print(result["data"])
```

### Comparing `AsyncKandinsky-0.0.3/setup.py` & `AsyncKandinsky-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def readme():
     with open('README.md', 'r') as f:
         return f.read()
 
 
 setup(
     name='AsyncKandinsky',
-    version='0.0.3',
+    version='0.0.4',
     author='s1rne',
     author_email='s.simaranov8@gmail.com',
     description='This module is designed for asynchronous use of the kandinsky neural network and easy integration into your project.',
     long_description=readme(),
     long_description_content_type='text/markdown',
     url='https://github.com/s1rne/kandinsky-async-api',
     packages=find_packages(),
```

