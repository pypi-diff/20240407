# Comparing `tmp/smawe_tools-0.3.6.tar.gz` & `tmp/smawe_tools-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smawe_tools-0.3.6.tar", last modified: Fri Apr  5 13:58:53 2024, max compression
+gzip compressed data, was "smawe_tools-0.3.7.tar", last modified: Sun Apr  7 14:08:57 2024, max compression
```

## Comparing `smawe_tools-0.3.6.tar` & `smawe_tools-0.3.7.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2024-04-05 13:58:53.009571 smawe_tools-0.3.6/
--rw-rw-rw-   0        0        0     1091 2023-01-15 03:19:33.000000 smawe_tools-0.3.6/LICENSE
--rw-rw-rw-   0        0        0     6784 2024-04-05 13:58:53.007571 smawe_tools-0.3.6/PKG-INFO
--rw-rw-rw-   0        0        0     6207 2024-04-05 13:53:38.000000 smawe_tools-0.3.6/README.md
--rw-rw-rw-   0        0        0       42 2024-04-05 13:58:53.009571 smawe_tools-0.3.6/setup.cfg
--rw-rw-rw-   0        0        0     1092 2023-11-21 11:30:20.000000 smawe_tools-0.3.6/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-05 13:58:52.956571 smawe_tools-0.3.6/smawe_tools/
--rw-rw-rw-   0        0        0      194 2023-11-21 11:27:09.000000 smawe_tools-0.3.6/smawe_tools/__init__.py
--rw-rw-rw-   0        0        0       76 2024-04-05 13:53:38.000000 smawe_tools-0.3.6/smawe_tools/__version__.py
--rw-rw-rw-   0        0        0      394 2023-06-18 06:13:54.000000 smawe_tools-0.3.6/smawe_tools/algorithm.py
--rw-rw-rw-   0        0        0     6799 2023-11-06 11:48:04.000000 smawe_tools-0.3.6/smawe_tools/config.py
-drwxrwxrwx   0        0        0        0 2024-04-05 13:58:52.976571 smawe_tools-0.3.6/smawe_tools/exception/
--rw-rw-rw-   0        0        0       98 2023-04-02 12:50:55.000000 smawe_tools-0.3.6/smawe_tools/exception/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-05 13:58:52.980571 smawe_tools-0.3.6/smawe_tools/net/
--rw-rw-rw-   0        0        0       29 2023-03-29 05:15:59.000000 smawe_tools-0.3.6/smawe_tools/net/__init__.py
--rw-rw-rw-   0        0        0     2887 2023-11-21 11:30:20.000000 smawe_tools-0.3.6/smawe_tools/net/network_tool.py
-drwxrwxrwx   0        0        0        0 2024-04-05 13:58:52.988572 smawe_tools-0.3.6/smawe_tools/retrying/
--rw-rw-rw-   0        0        0       26 2023-04-04 07:07:45.000000 smawe_tools-0.3.6/smawe_tools/retrying/__init__.py
--rw-rw-rw-   0        0        0     3357 2024-04-05 13:53:38.000000 smawe_tools-0.3.6/smawe_tools/retrying/retry.py
--rw-rw-rw-   0        0        0      705 2023-11-08 06:55:39.000000 smawe_tools-0.3.6/smawe_tools/settings.py
-drwxrwxrwx   0        0        0        0 2024-04-05 13:58:52.996571 smawe_tools-0.3.6/smawe_tools/struct/
--rw-rw-rw-   0        0        0      944 2023-11-02 06:42:01.000000 smawe_tools-0.3.6/smawe_tools/struct/__init__.py
--rw-rw-rw-   0        0        0     3077 2023-11-08 00:09:53.000000 smawe_tools-0.3.6/smawe_tools/tool.py
--rw-rw-rw-   0        0        0     1748 2023-11-10 03:37:29.000000 smawe_tools-0.3.6/smawe_tools/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-05 13:58:53.006571 smawe_tools-0.3.6/smawe_tools.egg-info/
--rw-rw-rw-   0        0        0     6784 2024-04-05 13:58:52.000000 smawe_tools-0.3.6/smawe_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      565 2024-04-05 13:58:52.000000 smawe_tools-0.3.6/smawe_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-05 13:58:52.000000 smawe_tools-0.3.6/smawe_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2024-04-05 13:58:52.000000 smawe_tools-0.3.6/smawe_tools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-05 13:58:52.000000 smawe_tools-0.3.6/smawe_tools.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-05 13:58:53.003571 smawe_tools-0.3.6/tests/
--rw-rw-rw-   0        0        0      725 2023-06-25 09:21:46.000000 smawe_tools-0.3.6/tests/test.py
+drwxrwxrwx   0        0        0        0 2024-04-07 14:08:57.883536 smawe_tools-0.3.7/
+-rw-rw-rw-   0        0        0     1091 2023-01-15 03:19:33.000000 smawe_tools-0.3.7/LICENSE
+-rw-rw-rw-   0        0        0     6735 2024-04-07 14:08:57.882537 smawe_tools-0.3.7/PKG-INFO
+-rw-rw-rw-   0        0        0     6158 2024-04-07 14:01:15.000000 smawe_tools-0.3.7/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-07 14:08:57.883536 smawe_tools-0.3.7/setup.cfg
+-rw-rw-rw-   0        0        0     1092 2023-11-21 11:30:20.000000 smawe_tools-0.3.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-07 14:08:57.814535 smawe_tools-0.3.7/smawe_tools/
+-rw-rw-rw-   0        0        0      194 2023-11-21 11:27:09.000000 smawe_tools-0.3.7/smawe_tools/__init__.py
+-rw-rw-rw-   0        0        0       76 2024-04-07 14:01:15.000000 smawe_tools-0.3.7/smawe_tools/__version__.py
+-rw-rw-rw-   0        0        0      394 2023-06-18 06:13:54.000000 smawe_tools-0.3.7/smawe_tools/algorithm.py
+-rw-rw-rw-   0        0        0     6799 2023-11-06 11:48:04.000000 smawe_tools-0.3.7/smawe_tools/config.py
+drwxrwxrwx   0        0        0        0 2024-04-07 14:08:57.837536 smawe_tools-0.3.7/smawe_tools/exception/
+-rw-rw-rw-   0        0        0       98 2023-04-02 12:50:55.000000 smawe_tools-0.3.7/smawe_tools/exception/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-07 14:08:57.855538 smawe_tools-0.3.7/smawe_tools/net/
+-rw-rw-rw-   0        0        0       29 2023-03-29 05:15:59.000000 smawe_tools-0.3.7/smawe_tools/net/__init__.py
+-rw-rw-rw-   0        0        0     2887 2023-11-21 11:30:20.000000 smawe_tools-0.3.7/smawe_tools/net/network_tool.py
+drwxrwxrwx   0        0        0        0 2024-04-07 14:08:57.864535 smawe_tools-0.3.7/smawe_tools/retrying/
+-rw-rw-rw-   0        0        0       26 2023-04-04 07:07:45.000000 smawe_tools-0.3.7/smawe_tools/retrying/__init__.py
+-rw-rw-rw-   0        0        0     3350 2024-04-07 14:06:00.000000 smawe_tools-0.3.7/smawe_tools/retrying/retry.py
+-rw-rw-rw-   0        0        0      705 2023-11-08 06:55:39.000000 smawe_tools-0.3.7/smawe_tools/settings.py
+drwxrwxrwx   0        0        0        0 2024-04-07 14:08:57.870536 smawe_tools-0.3.7/smawe_tools/struct/
+-rw-rw-rw-   0        0        0      944 2023-11-02 06:42:01.000000 smawe_tools-0.3.7/smawe_tools/struct/__init__.py
+-rw-rw-rw-   0        0        0     3077 2023-11-08 00:09:53.000000 smawe_tools-0.3.7/smawe_tools/tool.py
+-rw-rw-rw-   0        0        0     1748 2023-11-10 03:37:29.000000 smawe_tools-0.3.7/smawe_tools/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-07 14:08:57.880537 smawe_tools-0.3.7/smawe_tools.egg-info/
+-rw-rw-rw-   0        0        0     6735 2024-04-07 14:08:57.000000 smawe_tools-0.3.7/smawe_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      565 2024-04-07 14:08:57.000000 smawe_tools-0.3.7/smawe_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-07 14:08:57.000000 smawe_tools-0.3.7/smawe_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2024-04-07 14:08:57.000000 smawe_tools-0.3.7/smawe_tools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-07 14:08:57.000000 smawe_tools-0.3.7/smawe_tools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-07 14:08:57.878537 smawe_tools-0.3.7/tests/
+-rw-rw-rw-   0        0        0      725 2023-06-25 09:21:46.000000 smawe_tools-0.3.7/tests/test.py
```

### Comparing `smawe_tools-0.3.6/LICENSE` & `smawe_tools-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `smawe_tools-0.3.6/PKG-INFO` & `smawe_tools-0.3.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smawe_tools
-Version: 0.3.6
+Version: 0.3.7
 Summary: small tool
 Home-page: https://github.com/Smawexi/SmaweTools
 Author: Samwe
 Author-email: 1281722462@qq.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -12,28 +12,25 @@
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.5.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: colorama
 Requires-Dist: requests
 
-<<<<<<< HEAD
 ### 一个python工具库
 
 ---
 
 ### **安装**
 
 ```text
 pip install smawe-tools
 ```
 ---
 
-=======
->>>>>>> 158d883 (Update)
 ### **核心函数**
 以下函数都可以从smawe_tools包中进行导入  
 例如: from smawe_tools import retry  
 
 - rename(src=""):  
     对src路径指定的目录中的文件进行重命名(支持绝对路径和相对路径)  
     格式为第xxx章
```

### Comparing `smawe_tools-0.3.6/README.md` & `smawe_tools-0.3.7/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,18 @@
-<<<<<<< HEAD
 ### 一个python工具库
 
 ---
 
 ### **安装**
 
 ```text
 pip install smawe-tools
 ```
 ---
 
-=======
->>>>>>> 158d883 (Update)
 ### **核心函数**
 以下函数都可以从smawe_tools包中进行导入  
 例如: from smawe_tools import retry  
 
 - rename(src=""):  
     对src路径指定的目录中的文件进行重命名(支持绝对路径和相对路径)  
     格式为第xxx章
```

### Comparing `smawe_tools-0.3.6/setup.py` & `smawe_tools-0.3.7/setup.py`

 * *Files identical despite different names*

### Comparing `smawe_tools-0.3.6/smawe_tools/config.py` & `smawe_tools-0.3.7/smawe_tools/config.py`

 * *Files identical despite different names*

### Comparing `smawe_tools-0.3.6/smawe_tools/net/network_tool.py` & `smawe_tools-0.3.7/smawe_tools/net/network_tool.py`

 * *Files identical despite different names*

### Comparing `smawe_tools-0.3.6/smawe_tools/retrying/retry.py` & `smawe_tools-0.3.7/smawe_tools/retrying/retry.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,30 +29,31 @@
         self._wait_random_min = wait_random_min / 1000 if isinstance(wait_random_min, int) else 0
         self._wait_random_max = wait_random_max / 1000 if isinstance(wait_random_max, int) else 1
         if self._wait_random_max <= self._wait_random_min:
             raise ValueError("wait_random_min is greater than or equal to wait_random_max")
 
     def __get__(self, instance, owner=None):
         if isinstance(self._func, (staticmethod, classmethod)):
-            self._func = self._func.__get__(instance, owner)
+            self._f = self._func.__get__(instance, owner)
             return self
 
-        self._func = functools.partial(self._func, instance)
+        self._f = functools.partial(self._func, instance)
+
         return self
 
     def __call__(self, *args, **kwargs):
         current_retry_num = 0
         while True:
             if current_retry_num > self._stop_max_attempt_number:
                 raise _exception.MaxRetryError("Exceeded maximum retry count error")
             try:
                 if current_retry_num:
                     logging.info("\033[1;34mThis is currently the {} retry\033[0m".format(current_retry_num))
                     time.sleep(random.uniform(self._wait_random_min, self._wait_random_max))
-                return self._func(*args, **kwargs)
+                return self._f(*args, **kwargs)
             except self._retry_on_exception:
                 current_retry_num += 1
 
 
 def retry(
     stop_max_attempt_number=None, wait_random_min=None, wait_random_max=None,
     retry_on_exception=None, **kwargs
```

### Comparing `smawe_tools-0.3.6/smawe_tools/settings.py` & `smawe_tools-0.3.7/smawe_tools/settings.py`

 * *Files identical despite different names*

### Comparing `smawe_tools-0.3.6/smawe_tools/struct/__init__.py` & `smawe_tools-0.3.7/smawe_tools/struct/__init__.py`

 * *Files identical despite different names*

### Comparing `smawe_tools-0.3.6/smawe_tools/tool.py` & `smawe_tools-0.3.7/smawe_tools/tool.py`

 * *Files identical despite different names*

### Comparing `smawe_tools-0.3.6/smawe_tools/utils.py` & `smawe_tools-0.3.7/smawe_tools/utils.py`

 * *Files identical despite different names*

### Comparing `smawe_tools-0.3.6/smawe_tools.egg-info/PKG-INFO` & `smawe_tools-0.3.7/smawe_tools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smawe_tools
-Version: 0.3.6
+Version: 0.3.7
 Summary: small tool
 Home-page: https://github.com/Smawexi/SmaweTools
 Author: Samwe
 Author-email: 1281722462@qq.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -12,28 +12,25 @@
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.5.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: colorama
 Requires-Dist: requests
 
-<<<<<<< HEAD
 ### 一个python工具库
 
 ---
 
 ### **安装**
 
 ```text
 pip install smawe-tools
 ```
 ---
 
-=======
->>>>>>> 158d883 (Update)
 ### **核心函数**
 以下函数都可以从smawe_tools包中进行导入  
 例如: from smawe_tools import retry  
 
 - rename(src=""):  
     对src路径指定的目录中的文件进行重命名(支持绝对路径和相对路径)  
     格式为第xxx章
```

### Comparing `smawe_tools-0.3.6/smawe_tools.egg-info/SOURCES.txt` & `smawe_tools-0.3.7/smawe_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `smawe_tools-0.3.6/tests/test.py` & `smawe_tools-0.3.7/tests/test.py`

 * *Files identical despite different names*

