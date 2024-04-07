# Comparing `tmp/croco_selenium-0.1.5.tar.gz` & `tmp/croco_selenium-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "croco_selenium-0.1.5.tar", max compression
+gzip compressed data, was "croco_selenium-0.1.6.tar", max compression
```

## Comparing `croco_selenium-0.1.5.tar` & `croco_selenium-0.1.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1062 2023-12-19 17:17:43.274155 croco_selenium-0.1.5/LICENSE
--rw-r--r--   0        0        0     9360 2023-12-19 17:22:28.682487 croco_selenium-0.1.5/README.md
--rw-r--r--   0        0        0     1420 2023-12-19 17:17:43.275342 croco_selenium-0.1.5/croco_selenium/__init__.py
--rw-r--r--   0        0        0     1354 2023-12-19 17:17:43.275566 croco_selenium-0.1.5/croco_selenium/_croco_driver.py
--rw-r--r--   0        0        0     8536 2024-03-12 21:32:47.289257 croco_selenium-0.1.5/croco_selenium/action_performer.py
--rw-r--r--   0        0        0    10440 2024-03-12 21:32:47.295576 croco_selenium-0.1.5/croco_selenium/actions.py
--rw-r--r--   0        0        0     1161 2023-12-19 17:17:43.277576 croco_selenium-0.1.5/croco_selenium/chrome_driver.py
--rw-r--r--   0        0        0     4746 2024-03-13 16:49:55.931526 croco_selenium-0.1.5/croco_selenium/decorators.py
--rw-r--r--   0        0        0      358 2023-12-19 17:17:43.278188 croco_selenium-0.1.5/croco_selenium/exceptions.py
--rw-r--r--   0        0        0      388 2024-02-28 16:44:41.196772 croco_selenium-0.1.5/croco_selenium/types.py
--rw-r--r--   0        0        0      449 2024-02-28 16:44:34.572195 croco_selenium-0.1.5/croco_selenium/utils.py
--rw-r--r--   0        0        0     1096 2024-03-13 16:49:55.937275 croco_selenium-0.1.5/pyproject.toml
--rw-r--r--   0        0        0    10396 1970-01-01 00:00:00.000000 croco_selenium-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-12-19 17:17:43.274155 croco_selenium-0.1.6/LICENSE
+-rw-r--r--   0        0        0     9360 2023-12-19 17:22:28.682487 croco_selenium-0.1.6/README.md
+-rw-r--r--   0        0        0     1420 2023-12-19 17:17:43.275342 croco_selenium-0.1.6/croco_selenium/__init__.py
+-rw-r--r--   0        0        0     1354 2023-12-19 17:17:43.275566 croco_selenium-0.1.6/croco_selenium/_croco_driver.py
+-rw-r--r--   0        0        0     8536 2024-03-12 21:32:47.289257 croco_selenium-0.1.6/croco_selenium/action_performer.py
+-rw-r--r--   0        0        0    10483 2024-04-07 01:49:09.609532 croco_selenium-0.1.6/croco_selenium/actions.py
+-rw-r--r--   0        0        0     1161 2023-12-19 17:17:43.277576 croco_selenium-0.1.6/croco_selenium/chrome_driver.py
+-rw-r--r--   0        0        0     4746 2024-03-13 16:49:55.931526 croco_selenium-0.1.6/croco_selenium/decorators.py
+-rw-r--r--   0        0        0      358 2023-12-19 17:17:43.278188 croco_selenium-0.1.6/croco_selenium/exceptions.py
+-rw-r--r--   0        0        0      388 2024-02-28 16:44:41.196772 croco_selenium-0.1.6/croco_selenium/types.py
+-rw-r--r--   0        0        0      449 2024-02-28 16:44:34.572195 croco_selenium-0.1.6/croco_selenium/utils.py
+-rw-r--r--   0        0        0     1096 2024-04-07 01:49:09.614520 croco_selenium-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0    10396 1970-01-01 00:00:00.000000 croco_selenium-0.1.6/PKG-INFO
```

### Comparing `croco_selenium-0.1.5/LICENSE` & `croco_selenium-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `croco_selenium-0.1.5/README.md` & `croco_selenium-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `croco_selenium-0.1.5/croco_selenium/__init__.py` & `croco_selenium-0.1.6/croco_selenium/__init__.py`

 * *Files identical despite different names*

### Comparing `croco_selenium-0.1.5/croco_selenium/_croco_driver.py` & `croco_selenium-0.1.6/croco_selenium/_croco_driver.py`

 * *Files identical despite different names*

### Comparing `croco_selenium-0.1.5/croco_selenium/action_performer.py` & `croco_selenium-0.1.6/croco_selenium/action_performer.py`

 * *Files identical despite different names*

### Comparing `croco_selenium-0.1.5/croco_selenium/actions.py` & `croco_selenium-0.1.6/croco_selenium/actions.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,16 @@
     Switches to a different window from current window in browser
     :param driver: A driver to be interacted
     :param timeout: Number of seconds before timing out
 
     :return: str
     """
     original_window_handle = driver.current_window_handle
-    WebDriverWait(driver, timeout).until(EC.number_of_windows_to_be(2))
+    if len(driver.window_handles) < 2:
+        WebDriverWait(driver, timeout).until(EC.number_of_windows_to_be(2))
 
     for window_handle in driver.window_handles:
         if window_handle != original_window_handle:
             driver.switch_to.window(window_handle)
             break
```

### Comparing `croco_selenium-0.1.5/croco_selenium/chrome_driver.py` & `croco_selenium-0.1.6/croco_selenium/chrome_driver.py`

 * *Files identical despite different names*

### Comparing `croco_selenium-0.1.5/croco_selenium/decorators.py` & `croco_selenium-0.1.6/croco_selenium/decorators.py`

 * *Files identical despite different names*

### Comparing `croco_selenium-0.1.5/pyproject.toml` & `croco_selenium-0.1.6/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = 'croco_selenium'
-version = '0.1.5'
+version = '0.1.6'
 description = 'The package providing ways to interact with Selenium Web Driver actions, such as clicking, sending keys etc.'
 authors = ['Alexey <abelenkov2006@gmail.com>']
 license = 'MIT'
 readme = 'README.md'
 repository = 'https://github.com/blnkoff/croco-selenium'
 homepage = 'https://github.com/blnkoff/croco-selenium'
 classifiers = [
```

### Comparing `croco_selenium-0.1.5/PKG-INFO` & `croco_selenium-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: croco_selenium
-Version: 0.1.5
+Version: 0.1.6
 Summary: The package providing ways to interact with Selenium Web Driver actions, such as clicking, sending keys etc.
 Home-page: https://github.com/blnkoff/croco-selenium
 License: MIT
 Author: Alexey
 Author-email: abelenkov2006@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 4 - Beta
```

