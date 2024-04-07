# Comparing `tmp/szamlazz.py-1.3.0rc2.tar.gz` & `tmp/szamlazz.py-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "szamlazz.py-1.3.0rc2.tar", last modified: Sun Feb  4 21:18:57 2024, max compression
+gzip compressed data, was "szamlazz.py-1.4.0.tar", last modified: Sun Apr  7 20:43:57 2024, max compression
```

## Comparing `szamlazz.py-1.3.0rc2.tar` & `szamlazz.py-1.4.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 21:18:57.320551 szamlazz.py-1.3.0rc2/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-02-04 21:18:49.000000 szamlazz.py-1.3.0rc2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5695 2024-02-04 21:18:57.320551 szamlazz.py-1.3.0rc2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4756 2024-02-04 21:18:49.000000 szamlazz.py-1.3.0rc2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 21:18:57.316551 szamlazz.py-1.3.0rc2/examples/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-04 21:18:49.000000 szamlazz.py-1.3.0rc2/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      948 2024-02-04 21:18:49.000000 szamlazz.py-1.3.0rc2/examples/delete_pro_forma_invoice.py
--rw-r--r--   0 runner    (1001) docker     (127)     3778 2024-02-04 21:18:49.000000 szamlazz.py-1.3.0rc2/examples/generate_invoice.py
--rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-02-04 21:18:49.000000 szamlazz.py-1.3.0rc2/examples/query_invoice_pdf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-02-04 21:18:49.000000 szamlazz.py-1.3.0rc2/examples/query_invoice_xml.py
--rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-02-04 21:18:49.000000 szamlazz.py-1.3.0rc2/examples/register_credit_entry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-02-04 21:18:49.000000 szamlazz.py-1.3.0rc2/examples/storno.py
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-02-04 21:18:49.000000 szamlazz.py-1.3.0rc2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-04 21:18:57.320551 szamlazz.py-1.3.0rc2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-02-04 21:18:49.000000 szamlazz.py-1.3.0rc2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 21:18:57.320551 szamlazz.py-1.3.0rc2/szamlazz/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-02-04 21:18:49.000000 szamlazz.py-1.3.0rc2/szamlazz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20141 2024-02-04 21:18:49.000000 szamlazz.py-1.3.0rc2/szamlazz/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    10685 2024-02-04 21:18:49.000000 szamlazz.py-1.3.0rc2/szamlazz/models.py
--rw-r--r--   0 runner    (1001) docker     (127)    16505 2024-02-04 21:18:49.000000 szamlazz.py-1.3.0rc2/szamlazz/templates.py
--rw-r--r--   0 runner    (1001) docker     (127)     3276 2024-02-04 21:18:49.000000 szamlazz.py-1.3.0rc2/szamlazz/version.py
--rw-r--r--   0 runner    (1001) docker     (127)    35279 2024-02-04 21:18:49.000000 szamlazz.py-1.3.0rc2/szamlazz/xsd.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 21:18:57.320551 szamlazz.py-1.3.0rc2/szamlazz.py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5695 2024-02-04 21:18:57.000000 szamlazz.py-1.3.0rc2/szamlazz.py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      532 2024-02-04 21:18:57.000000 szamlazz.py-1.3.0rc2/szamlazz.py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-04 21:18:57.000000 szamlazz.py-1.3.0rc2/szamlazz.py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-02-04 21:18:57.000000 szamlazz.py-1.3.0rc2/szamlazz.py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-02-04 21:18:57.000000 szamlazz.py-1.3.0rc2/szamlazz.py.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 20:43:57.768395 szamlazz.py-1.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-07 20:43:53.000000 szamlazz.py-1.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5794 2024-04-07 20:43:57.768395 szamlazz.py-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4756 2024-04-07 20:43:53.000000 szamlazz.py-1.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 20:43:57.768395 szamlazz.py-1.4.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 20:43:53.000000 szamlazz.py-1.4.0/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2024-04-07 20:43:53.000000 szamlazz.py-1.4.0/examples/delete_pro_forma_invoice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3778 2024-04-07 20:43:53.000000 szamlazz.py-1.4.0/examples/generate_invoice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-04-07 20:43:53.000000 szamlazz.py-1.4.0/examples/query_invoice_pdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-04-07 20:43:53.000000 szamlazz.py-1.4.0/examples/query_invoice_xml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-04-07 20:43:53.000000 szamlazz.py-1.4.0/examples/register_credit_entry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-04-07 20:43:53.000000 szamlazz.py-1.4.0/examples/storno.py
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-07 20:43:53.000000 szamlazz.py-1.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 20:43:57.768395 szamlazz.py-1.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-04-07 20:43:53.000000 szamlazz.py-1.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 20:43:57.768395 szamlazz.py-1.4.0/szamlazz/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-07 20:43:53.000000 szamlazz.py-1.4.0/szamlazz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20141 2024-04-07 20:43:53.000000 szamlazz.py-1.4.0/szamlazz/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10685 2024-04-07 20:43:53.000000 szamlazz.py-1.4.0/szamlazz/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16505 2024-04-07 20:43:53.000000 szamlazz.py-1.4.0/szamlazz/templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3276 2024-04-07 20:43:53.000000 szamlazz.py-1.4.0/szamlazz/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35279 2024-04-07 20:43:53.000000 szamlazz.py-1.4.0/szamlazz/xsd.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 20:43:57.768395 szamlazz.py-1.4.0/szamlazz.py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5794 2024-04-07 20:43:57.000000 szamlazz.py-1.4.0/szamlazz.py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-04-07 20:43:57.000000 szamlazz.py-1.4.0/szamlazz.py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 20:43:57.000000 szamlazz.py-1.4.0/szamlazz.py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-07 20:43:57.000000 szamlazz.py-1.4.0/szamlazz.py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-07 20:43:57.000000 szamlazz.py-1.4.0/szamlazz.py.egg-info/top_level.txt
```

### Comparing `szamlazz.py-1.3.0rc2/LICENSE` & `szamlazz.py-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `szamlazz.py-1.3.0rc2/PKG-INFO` & `szamlazz.py-1.4.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 Metadata-Version: 2.1
 Name: szamlazz.py
-Version: 1.3.0rc2
+Version: 1.4.0
 Summary: Python client for Szamlazz.hu :: Számla Agent
 Home-page: https://github.com/theriverman/szamlazz.py
 Author: Kristof Daja (theriverman)
-Author-email: kristof@daja.hu
+Author-email: cowling_benzene0r@icloud.com
 License: MIT License | Copyright (c) 2020 — 2024 Kristof Daja
 Project-URL: Bug Tracker, https://github.com/theriverman/szamlazz.py/issues
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.6
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: Jinja2~=3.1.2
+Requires-Dist: requests>=2.31.0
+Requires-Dist: lxml~=4.9.2
 
 szamlazz.py
 ----
 The **szamlazz.py** package is a Python client (wrapper) for *Szamlazz.hu::Számla Agent*.
 
 # Introduction
 Számla Agent is a non-browser-based interface of the Számlázz.hu system.
```

### Comparing `szamlazz.py-1.3.0rc2/README.md` & `szamlazz.py-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `szamlazz.py-1.3.0rc2/examples/delete_pro_forma_invoice.py` & `szamlazz.py-1.4.0/examples/delete_pro_forma_invoice.py`

 * *Files identical despite different names*

### Comparing `szamlazz.py-1.3.0rc2/examples/generate_invoice.py` & `szamlazz.py-1.4.0/examples/generate_invoice.py`

 * *Files identical despite different names*

### Comparing `szamlazz.py-1.3.0rc2/examples/query_invoice_pdf.py` & `szamlazz.py-1.4.0/examples/query_invoice_pdf.py`

 * *Files identical despite different names*

### Comparing `szamlazz.py-1.3.0rc2/examples/query_invoice_xml.py` & `szamlazz.py-1.4.0/examples/query_invoice_xml.py`

 * *Files identical despite different names*

### Comparing `szamlazz.py-1.3.0rc2/examples/register_credit_entry.py` & `szamlazz.py-1.4.0/examples/register_credit_entry.py`

 * *Files identical despite different names*

### Comparing `szamlazz.py-1.3.0rc2/examples/storno.py` & `szamlazz.py-1.4.0/examples/storno.py`

 * *Files identical despite different names*

### Comparing `szamlazz.py-1.3.0rc2/setup.py` & `szamlazz.py-1.4.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     long_description = fh.read()
 
 
 setuptools.setup(
     name="szamlazz.py",
     version=get_git_version(),
     author='Kristof Daja (theriverman)',
-    author_email='kristof@daja.hu',
+    author_email='cowling_benzene0r@icloud.com',
     description='Python client for Szamlazz.hu :: Számla Agent',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/theriverman/szamlazz.py',
     project_urls={
         "Bug Tracker": "https://github.com/theriverman/szamlazz.py/issues",
     },
@@ -26,17 +26,17 @@
     ],
     classifiers=[
         'Environment :: Web Environment',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
         'Programming Language :: Python',
-        'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3.12',
     ],
     packages=setuptools.find_packages(),
-    python_requires=">=3.6",
+    python_requires=">=3.8",
     license=f'MIT License | Copyright (c) 2020 — {datetime.now().year} Kristof Daja',
 )
```

### Comparing `szamlazz.py-1.3.0rc2/szamlazz/client.py` & `szamlazz.py-1.4.0/szamlazz/client.py`

 * *Files identical despite different names*

### Comparing `szamlazz.py-1.3.0rc2/szamlazz/models.py` & `szamlazz.py-1.4.0/szamlazz/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -144,15 +144,15 @@
                  response: Response,
                  xml_namespace: str,
                  ):
         self.xml_namespace = xml_namespace
         self.__response = response
         self.__action_success: bool = False
         content_type = response.headers.get("Content-Type")
-        if content_type == "application/octet-stream":
+        if "application/octet-stream" in content_type:
             # Parse XML and map into class members
             root = ET.fromstring(self.__response.text)
             self.__pdf: str = self.__get_tag_text(root, "pdf")
             self.__pdf_bytes: bytes = b""
             self.__action_success: bool = True if (self.__get_tag_text(root, "sikeres") == "true") else False
         else:
             self.__pdf_bytes: bytes = response.content
```

### Comparing `szamlazz.py-1.3.0rc2/szamlazz/templates.py` & `szamlazz.py-1.4.0/szamlazz/templates.py`

 * *Files identical despite different names*

### Comparing `szamlazz.py-1.3.0rc2/szamlazz/version.py` & `szamlazz.py-1.4.0/szamlazz/version.py`

 * *Files identical despite different names*

### Comparing `szamlazz.py-1.3.0rc2/szamlazz/xsd.py` & `szamlazz.py-1.4.0/szamlazz/xsd.py`

 * *Files identical despite different names*

### Comparing `szamlazz.py-1.3.0rc2/szamlazz.py.egg-info/PKG-INFO` & `szamlazz.py-1.4.0/szamlazz.py.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 Metadata-Version: 2.1
 Name: szamlazz.py
-Version: 1.3.0rc2
+Version: 1.4.0
 Summary: Python client for Szamlazz.hu :: Számla Agent
 Home-page: https://github.com/theriverman/szamlazz.py
 Author: Kristof Daja (theriverman)
-Author-email: kristof@daja.hu
+Author-email: cowling_benzene0r@icloud.com
 License: MIT License | Copyright (c) 2020 — 2024 Kristof Daja
 Project-URL: Bug Tracker, https://github.com/theriverman/szamlazz.py/issues
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.6
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: Jinja2~=3.1.2
+Requires-Dist: requests>=2.31.0
+Requires-Dist: lxml~=4.9.2
 
 szamlazz.py
 ----
 The **szamlazz.py** package is a Python client (wrapper) for *Szamlazz.hu::Számla Agent*.
 
 # Introduction
 Számla Agent is a non-browser-based interface of the Számlázz.hu system.
```

### Comparing `szamlazz.py-1.3.0rc2/szamlazz.py.egg-info/SOURCES.txt` & `szamlazz.py-1.4.0/szamlazz.py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

