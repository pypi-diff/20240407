# Comparing `tmp/envo-1.5.1.tar.gz` & `tmp/envo-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "envo-1.5.1.tar", max compression
+gzip compressed data, was "envo-1.5.2.tar", max compression
```

## Comparing `envo-1.5.1.tar` & `envo-1.5.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     3040 2023-10-27 23:33:36.336080 envo-1.5.1/README.rst
--rw-r--r--   0        0        0      612 2024-02-29 10:48:19.341342 envo-1.5.1/envo/__init__.py
--rw-r--r--   0        0        0       40 2023-10-27 23:33:36.340080 envo-1.5.1/envo/__main__.py
--rw-r--r--   0        0        0       12 2023-11-06 15:33:42.150771 envo-1.5.1/envo/comp.py
--rw-r--r--   0        0        0     1739 2023-11-06 15:33:42.150771 envo-1.5.1/envo/const.py
--rw-r--r--   0        0        0     3837 2023-11-06 15:33:42.150771 envo-1.5.1/envo/devops.py
--rw-r--r--   0        0        0     2210 2024-02-29 15:29:07.455477 envo-1.5.1/envo/e2e.py
--rw-r--r--   0        0        0      594 2023-10-27 23:33:36.340080 envo-1.5.1/envo/emergency_env.py
--rw-r--r--   0        0        0    20404 2024-02-29 15:28:23.091067 envo-1.5.1/envo/env.py
--rw-r--r--   0        0        0      410 2023-11-06 15:33:42.150771 envo-1.5.1/envo/environ.py
--rw-r--r--   0        0        0     2303 2024-02-29 02:02:42.771508 envo-1.5.1/envo/exceptions.py
--rw-r--r--   0        0        0     7935 2023-11-06 15:33:42.150771 envo-1.5.1/envo/logs.py
--rw-r--r--   0        0        0     1755 2024-02-29 03:26:52.500838 envo-1.5.1/envo/plugins.py
--rw-r--r--   0        0        0        0 2023-10-27 23:33:36.340080 envo-1.5.1/envo/py.typed
--rwxr-xr-x   0        0        0    13061 2024-02-29 15:34:38.554726 envo-1.5.1/envo/scripts.py
--rw-r--r--   0        0        0    11506 2024-03-29 04:39:02.140775 envo-1.5.1/envo/shell.py
--rw-r--r--   0        0        0     1491 2024-02-29 02:02:04.875013 envo-1.5.1/envo/status.py
--rw-r--r--   0        0        0     2162 2023-11-06 15:33:42.154771 envo-1.5.1/envo/styles.py
--rw-r--r--   0        0        0     1006 2023-10-27 23:33:36.340080 envo-1.5.1/envo/templates/comm_env.py.templ
--rw-r--r--   0        0        0      973 2023-10-27 23:33:36.340080 envo-1.5.1/envo/templates/env.py.templ
--rw-r--r--   0        0        0     5078 2024-02-29 15:34:35.162691 envo-1.5.1/envo/utils.py
--rw-r--r--   0        0        0        0 2023-11-06 15:33:42.154771 envo-1.5.1/envo/vendored/__init__.py
--rw-r--r--   0        0        0    14601 2023-11-06 15:33:42.154771 envo-1.5.1/envo/vendored/colorizer.py
--rw-r--r--   0        0        0     4953 2024-02-29 03:27:04.841256 envo-1.5.1/envo/venv_utils.py
--rw-r--r--   0        0        0     1673 2024-03-29 04:40:34.249172 envo-1.5.1/pyproject.toml
--rw-r--r--   0        0        0     4282 1970-01-01 00:00:00.000000 envo-1.5.1/PKG-INFO
+-rw-r--r--   0        0        0     3040 2023-10-27 23:33:36.336080 envo-1.5.2/README.rst
+-rw-r--r--   0        0        0      612 2024-04-06 10:03:50.564220 envo-1.5.2/envo/__init__.py
+-rw-r--r--   0        0        0       40 2023-10-27 23:33:36.340080 envo-1.5.2/envo/__main__.py
+-rw-r--r--   0        0        0       12 2023-11-06 15:33:42.150771 envo-1.5.2/envo/comp.py
+-rw-r--r--   0        0        0     1739 2023-11-06 15:33:42.150771 envo-1.5.2/envo/const.py
+-rw-r--r--   0        0        0     3837 2023-11-06 15:33:42.150771 envo-1.5.2/envo/devops.py
+-rw-r--r--   0        0        0     2210 2024-04-06 10:03:50.576220 envo-1.5.2/envo/e2e.py
+-rw-r--r--   0        0        0      594 2023-10-27 23:33:36.340080 envo-1.5.2/envo/emergency_env.py
+-rw-r--r--   0        0        0    20267 2024-04-07 11:48:38.500064 envo-1.5.2/envo/env.py
+-rw-r--r--   0        0        0      410 2023-11-06 15:33:42.150771 envo-1.5.2/envo/environ.py
+-rw-r--r--   0        0        0     2303 2024-04-06 10:03:50.536220 envo-1.5.2/envo/exceptions.py
+-rw-r--r--   0        0        0     7935 2023-11-06 15:33:42.150771 envo-1.5.2/envo/logs.py
+-rw-r--r--   0        0        0     1755 2024-04-06 10:03:50.544220 envo-1.5.2/envo/plugins.py
+-rw-r--r--   0        0        0        0 2023-10-27 23:33:36.340080 envo-1.5.2/envo/py.typed
+-rwxr-xr-x   0        0        0    13061 2024-04-06 10:03:50.576220 envo-1.5.2/envo/scripts.py
+-rw-r--r--   0        0        0    11506 2024-04-06 10:05:49.892025 envo-1.5.2/envo/shell.py
+-rw-r--r--   0        0        0     1491 2024-04-06 10:03:50.536220 envo-1.5.2/envo/status.py
+-rw-r--r--   0        0        0     2162 2023-11-06 15:33:42.154771 envo-1.5.2/envo/styles.py
+-rw-r--r--   0        0        0     1006 2023-10-27 23:33:36.340080 envo-1.5.2/envo/templates/comm_env.py.templ
+-rw-r--r--   0        0        0      973 2023-10-27 23:33:36.340080 envo-1.5.2/envo/templates/env.py.templ
+-rw-r--r--   0        0        0     5078 2024-04-06 10:03:50.564220 envo-1.5.2/envo/utils.py
+-rw-r--r--   0        0        0        0 2023-11-06 15:33:42.154771 envo-1.5.2/envo/vendored/__init__.py
+-rw-r--r--   0        0        0    14601 2023-11-06 15:33:42.154771 envo-1.5.2/envo/vendored/colorizer.py
+-rw-r--r--   0        0        0     4953 2024-04-06 10:03:50.544220 envo-1.5.2/envo/venv_utils.py
+-rw-r--r--   0        0        0     1673 2024-04-07 11:49:45.268699 envo-1.5.2/pyproject.toml
+-rw-r--r--   0        0        0     4282 1970-01-01 00:00:00.000000 envo-1.5.2/PKG-INFO
```

### Comparing `envo-1.5.1/README.rst` & `envo-1.5.2/README.rst`

 * *Files identical despite different names*

### Comparing `envo-1.5.1/envo/__init__.py` & `envo-1.5.2/envo/__init__.py`

 * *Files identical despite different names*

### Comparing `envo-1.5.1/envo/const.py` & `envo-1.5.2/envo/const.py`

 * *Files identical despite different names*

### Comparing `envo-1.5.1/envo/devops.py` & `envo-1.5.2/envo/devops.py`

 * *Files identical despite different names*

### Comparing `envo-1.5.1/envo/e2e.py` & `envo-1.5.2/envo/e2e.py`

 * *Files identical despite different names*

### Comparing `envo-1.5.1/envo/emergency_env.py` & `envo-1.5.2/envo/emergency_env.py`

 * *Files identical despite different names*

### Comparing `envo-1.5.1/envo/env.py` & `envo-1.5.2/envo/env.py`

 * *Files 1% similar despite different names*

```diff
@@ -351,19 +351,15 @@
         self.secrets = Env.env_id_to_secrets[self.id] = secrets
 
         self.init()
 
         self.validate()
         self.activate()
 
-        for c in reversed(self.__class__.__mro__):
-            if not issubclass(c, BaseEnv):
-                continue
-
-            getattr(c, "post_init")(self)
+        self.post_init()
 
     def _get_path_delimiter(self) -> str:
         if utils.is_linux() or utils.is_darwin():
             return ":"
         elif utils.is_windows():
             return ";"
         else:
```

### Comparing `envo-1.5.1/envo/exceptions.py` & `envo-1.5.2/envo/exceptions.py`

 * *Files identical despite different names*

### Comparing `envo-1.5.1/envo/logs.py` & `envo-1.5.2/envo/logs.py`

 * *Files identical despite different names*

### Comparing `envo-1.5.1/envo/plugins.py` & `envo-1.5.2/envo/plugins.py`

 * *Files identical despite different names*

### Comparing `envo-1.5.1/envo/scripts.py` & `envo-1.5.2/envo/scripts.py`

 * *Files identical despite different names*

### Comparing `envo-1.5.1/envo/shell.py` & `envo-1.5.2/envo/shell.py`

 * *Files identical despite different names*

### Comparing `envo-1.5.1/envo/status.py` & `envo-1.5.2/envo/status.py`

 * *Files identical despite different names*

### Comparing `envo-1.5.1/envo/styles.py` & `envo-1.5.2/envo/styles.py`

 * *Files identical despite different names*

### Comparing `envo-1.5.1/envo/templates/comm_env.py.templ` & `envo-1.5.2/envo/templates/comm_env.py.templ`

 * *Files identical despite different names*

### Comparing `envo-1.5.1/envo/templates/env.py.templ` & `envo-1.5.2/envo/templates/env.py.templ`

 * *Files identical despite different names*

### Comparing `envo-1.5.1/envo/utils.py` & `envo-1.5.2/envo/utils.py`

 * *Files identical despite different names*

### Comparing `envo-1.5.1/envo/vendored/colorizer.py` & `envo-1.5.2/envo/vendored/colorizer.py`

 * *Files identical despite different names*

### Comparing `envo-1.5.1/envo/venv_utils.py` & `envo-1.5.2/envo/venv_utils.py`

 * *Files identical despite different names*

### Comparing `envo-1.5.1/pyproject.toml` & `envo-1.5.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "envo"
-version = "1.5.1"
+version = "1.5.2"
 description = "Smart Environments handling - Define command hooks, file hooks and env variables in python and activate hot reloaded shells."
 authors = ["Damian Krystkiewicz <damian.krystkiewicz@gmail.com>"]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Environment :: Console",
```

### Comparing `envo-1.5.1/PKG-INFO` & `envo-1.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: envo
-Version: 1.5.1
+Version: 1.5.2
 Summary: Smart Environments handling - Define command hooks, file hooks and env variables in python and activate hot reloaded shells.
 License: Apache 2.0
 Author: Damian Krystkiewicz
 Author-email: damian.krystkiewicz@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

