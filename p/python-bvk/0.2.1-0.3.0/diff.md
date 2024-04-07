# Comparing `tmp/python-bvk-0.2.1.tar.gz` & `tmp/python-bvk-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-bvk-0.2.1.tar", last modified: Wed Jul  5 09:53:10 2023, max compression
+gzip compressed data, was "python-bvk-0.3.0.tar", last modified: Sun Apr  7 10:10:01 2024, max compression
```

## Comparing `python-bvk-0.2.1.tar` & `python-bvk-0.3.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 dan       (1000) dan       (1000)        0 2023-07-05 09:53:10.060830 python-bvk-0.2.1/
--rw-r--r--   0 dan       (1000) dan       (1000)    11357 2020-08-07 19:27:30.000000 python-bvk-0.2.1/LICENSE
--rw-r--r--   0 dan       (1000) dan       (1000)     3405 2023-07-05 09:53:10.060830 python-bvk-0.2.1/PKG-INFO
--rw-r--r--   0 dan       (1000) dan       (1000)     2919 2021-12-14 21:55:17.000000 python-bvk-0.2.1/README.md
-drwxr-xr-x   0 dan       (1000) dan       (1000)        0 2023-07-05 09:53:10.058830 python-bvk-0.2.1/bvk/
--rw-r--r--   0 dan       (1000) dan       (1000)     1867 2021-12-14 21:50:15.000000 python-bvk-0.2.1/bvk/__init__.py
--rw-r--r--   0 dan       (1000) dan       (1000)      645 2021-09-25 10:08:10.000000 python-bvk-0.2.1/bvk/items.py
--rw-r--r--   0 dan       (1000) dan       (1000)     3263 2020-08-07 19:27:30.000000 python-bvk-0.2.1/bvk/settings.py
-drwxr-xr-x   0 dan       (1000) dan       (1000)        0 2023-07-05 09:53:10.059830 python-bvk-0.2.1/bvk/spiders/
--rw-r--r--   0 dan       (1000) dan       (1000)      161 2020-08-07 19:27:30.000000 python-bvk-0.2.1/bvk/spiders/__init__.py
--rw-r--r--   0 dan       (1000) dan       (1000)     5029 2021-12-14 21:51:07.000000 python-bvk-0.2.1/bvk/spiders/water_consumption.py
-drwxr-xr-x   0 dan       (1000) dan       (1000)        0 2023-07-05 09:53:10.059830 python-bvk-0.2.1/python_bvk.egg-info/
--rw-r--r--   0 dan       (1000) dan       (1000)     3405 2023-07-05 09:53:09.000000 python-bvk-0.2.1/python_bvk.egg-info/PKG-INFO
--rw-r--r--   0 dan       (1000) dan       (1000)      297 2023-07-05 09:53:10.000000 python-bvk-0.2.1/python_bvk.egg-info/SOURCES.txt
--rw-r--r--   0 dan       (1000) dan       (1000)        1 2023-07-05 09:53:09.000000 python-bvk-0.2.1/python_bvk.egg-info/dependency_links.txt
--rw-r--r--   0 dan       (1000) dan       (1000)       23 2023-07-05 09:53:09.000000 python-bvk-0.2.1/python_bvk.egg-info/requires.txt
--rw-r--r--   0 dan       (1000) dan       (1000)        4 2023-07-05 09:53:09.000000 python-bvk-0.2.1/python_bvk.egg-info/top_level.txt
--rw-r--r--   0 dan       (1000) dan       (1000)       38 2023-07-05 09:53:10.060830 python-bvk-0.2.1/setup.cfg
--rw-r--r--   0 dan       (1000) dan       (1000)      785 2023-07-05 09:47:48.000000 python-bvk-0.2.1/setup.py
+drwxr-xr-x   0 dan       (1000) dan       (1000)        0 2024-04-07 10:10:01.717184 python-bvk-0.3.0/
+-rw-r--r--   0 dan       (1000) dan       (1000)    11357 2020-08-07 19:27:30.000000 python-bvk-0.3.0/LICENSE
+-rw-r--r--   0 dan       (1000) dan       (1000)     3405 2024-04-07 10:10:01.717184 python-bvk-0.3.0/PKG-INFO
+-rw-r--r--   0 dan       (1000) dan       (1000)     2919 2021-12-14 21:55:17.000000 python-bvk-0.3.0/README.md
+drwxr-xr-x   0 dan       (1000) dan       (1000)        0 2024-04-07 10:10:01.716184 python-bvk-0.3.0/bvk/
+-rw-r--r--   0 dan       (1000) dan       (1000)     1867 2021-12-14 21:50:15.000000 python-bvk-0.3.0/bvk/__init__.py
+-rw-r--r--   0 dan       (1000) dan       (1000)      645 2021-09-25 10:08:10.000000 python-bvk-0.3.0/bvk/items.py
+-rw-r--r--   0 dan       (1000) dan       (1000)     3263 2020-08-07 19:27:30.000000 python-bvk-0.3.0/bvk/settings.py
+drwxr-xr-x   0 dan       (1000) dan       (1000)        0 2024-04-07 10:10:01.716184 python-bvk-0.3.0/bvk/spiders/
+-rw-r--r--   0 dan       (1000) dan       (1000)      161 2020-08-07 19:27:30.000000 python-bvk-0.3.0/bvk/spiders/__init__.py
+-rw-r--r--   0 dan       (1000) dan       (1000)     5219 2024-04-07 09:56:55.000000 python-bvk-0.3.0/bvk/spiders/water_consumption.py
+drwxr-xr-x   0 dan       (1000) dan       (1000)        0 2024-04-07 10:10:01.717184 python-bvk-0.3.0/python_bvk.egg-info/
+-rw-r--r--   0 dan       (1000) dan       (1000)     3405 2024-04-07 10:10:01.000000 python-bvk-0.3.0/python_bvk.egg-info/PKG-INFO
+-rw-r--r--   0 dan       (1000) dan       (1000)      297 2024-04-07 10:10:01.000000 python-bvk-0.3.0/python_bvk.egg-info/SOURCES.txt
+-rw-r--r--   0 dan       (1000) dan       (1000)        1 2024-04-07 10:10:01.000000 python-bvk-0.3.0/python_bvk.egg-info/dependency_links.txt
+-rw-r--r--   0 dan       (1000) dan       (1000)       23 2024-04-07 10:10:01.000000 python-bvk-0.3.0/python_bvk.egg-info/requires.txt
+-rw-r--r--   0 dan       (1000) dan       (1000)        4 2024-04-07 10:10:01.000000 python-bvk-0.3.0/python_bvk.egg-info/top_level.txt
+-rw-r--r--   0 dan       (1000) dan       (1000)       38 2024-04-07 10:10:01.717184 python-bvk-0.3.0/setup.cfg
+-rw-r--r--   0 dan       (1000) dan       (1000)      785 2024-04-07 09:57:47.000000 python-bvk-0.3.0/setup.py
```

### Comparing `python-bvk-0.2.1/LICENSE` & `python-bvk-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python-bvk-0.2.1/PKG-INFO` & `python-bvk-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-bvk
-Version: 0.2.1
+Version: 0.3.0
 Summary: Python library for tracking water consumption from BVK (Brnenske vodarny a kanalizace, bvk.cz)
 Home-page: https://github.com/dankeder/python-bvk
 Author: Dan Keder
 Author-email: dan.keder@protonmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `python-bvk-0.2.1/README.md` & `python-bvk-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `python-bvk-0.2.1/bvk/__init__.py` & `python-bvk-0.3.0/bvk/__init__.py`

 * *Files identical despite different names*

### Comparing `python-bvk-0.2.1/bvk/items.py` & `python-bvk-0.3.0/bvk/items.py`

 * *Files identical despite different names*

### Comparing `python-bvk-0.2.1/bvk/settings.py` & `python-bvk-0.3.0/bvk/settings.py`

 * *Files identical despite different names*

### Comparing `python-bvk-0.2.1/bvk/spiders/water_consumption.py` & `python-bvk-0.3.0/bvk/spiders/water_consumption.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from datetime import date
-from urllib.parse import urlencode, urljoin
+from urllib.parse import unquote, urlencode, urljoin
 
 import scrapy
 from dateutil import rrule
 from scrapy.loader import ItemLoader
 
 from ..items import WaterConsumptionItem
 
@@ -39,34 +39,36 @@
     def start_requests(self):
         url = "https://zis.bvk.cz/"
         yield scrapy.Request(url=url, callback=self.handle_login)
 
     def handle_login(self, response):
         return scrapy.FormRequest.from_response(
             response,
-            formid="aspnetForm",
+            formid="ctl00_ctl00_lvLoginForm_LoginDialog1_PanelLogin",
             headers={"X-MicrosoftAjax": "Delta=true"},
             formdata={
-                "ctl00$lvLoginForm$LoginDialog1$edEmail": self._bvk_username,
-                "ctl00$lvLoginForm$LoginDialog1$edPassword": self._bvk_password,
-                "ctl00$lvLoginForm$LoginDialog1$btnLogin": "Login",
+                "ctl00$ctl00$lvLoginForm$LoginDialog1$edEmail": self._bvk_username,
+                "ctl00$ctl00$lvLoginForm$LoginDialog1$edPassword": self._bvk_password,
+                "ctl00$ctl00$lvLoginForm$LoginDialog1$btnLogin": "Login",
             },
             callback=self.handle_login_response,
         )
 
     def handle_login_response(self, response):
-        if "pageRedirect" in response.text:
-            main_info_url = urljoin(response.url, "/Userdata/MainInfo.aspx")
+        response_parts = response.text.split('|')
+        if response_parts[5] == "pageRedirect":
+            redirect_url = "/Userdata/MainInfo.aspx"
+            main_info_url = urljoin(response.url, redirect_url)
             return scrapy.Request(url=main_info_url, callback=self.handle_main_info_response)
         else:
             raise Exception(f"Login to BVK failed (status {response.status}): {response.text}")
 
     def handle_main_info_response(self, response):
         suezsmartsolutions_login_url = response.css(
-            "a#ctl00_ctl00_ContentPlaceHolder1_UserDataContentPlaceHolder_btnPortalEmis"
+            "a#ctl00_ctl00_ctl00_ContentPlaceHolder1Common_ContentPlaceHolder1_UserDataContentPlaceHolder_btnPortalEmis"
         ).attrib["href"]
         return scrapy.Request(url=suezsmartsolutions_login_url, callback=self.handle_suezsmartsolutions_login_response)
 
     def handle_suezsmartsolutions_login_response(self, response):
         # Iterate over years/months between `date_from` and `date_to` and get
         # the daily consumption for the respective months
         #
```

### Comparing `python-bvk-0.2.1/python_bvk.egg-info/PKG-INFO` & `python-bvk-0.3.0/python_bvk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-bvk
-Version: 0.2.1
+Version: 0.3.0
 Summary: Python library for tracking water consumption from BVK (Brnenske vodarny a kanalizace, bvk.cz)
 Home-page: https://github.com/dankeder/python-bvk
 Author: Dan Keder
 Author-email: dan.keder@protonmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `python-bvk-0.2.1/setup.py` & `python-bvk-0.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 install_requires = ["scrapy", "python-dateutil"]
 
 setuptools.setup(
     name="python-bvk",
-    version="0.2.1",
+    version="0.3.0",
     author="Dan Keder",
     author_email="dan.keder@protonmail.com",
     description="Python library for tracking water consumption from BVK (Brnenske vodarny a kanalizace, bvk.cz)",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/dankeder/python-bvk",
     packages=setuptools.find_packages(),
```

