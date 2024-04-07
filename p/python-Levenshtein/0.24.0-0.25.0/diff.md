# Comparing `tmp/python-Levenshtein-0.24.0.tar.gz` & `tmp/python-Levenshtein-0.25.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-Levenshtein-0.24.0.tar", last modified: Wed Jan 31 22:43:20 2024, max compression
+gzip compressed data, was "python-Levenshtein-0.25.0.tar", last modified: Sun Feb 11 22:07:24 2024, max compression
```

## Comparing `python-Levenshtein-0.24.0.tar` & `python-Levenshtein-0.25.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 22:43:20.353145 python-Levenshtein-0.24.0/
--rw-r--r--   0 runner    (1001) docker     (127)    18085 2024-01-31 22:43:12.000000 python-Levenshtein-0.24.0/COPYING
--rw-r--r--   0 runner    (1001) docker     (127)     7859 2024-01-31 22:43:12.000000 python-Levenshtein-0.24.0/HISTORY.md
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-31 22:43:12.000000 python-Levenshtein-0.24.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-01-31 22:43:20.353145 python-Levenshtein-0.24.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2835 2024-01-31 22:43:12.000000 python-Levenshtein-0.24.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-01-31 22:43:12.000000 python-Levenshtein-0.24.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 22:43:20.353145 python-Levenshtein-0.24.0/python_Levenshtein.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-01-31 22:43:20.000000 python-Levenshtein-0.24.0/python_Levenshtein.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-01-31 22:43:20.000000 python-Levenshtein-0.24.0/python_Levenshtein.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-31 22:43:20.000000 python-Levenshtein-0.24.0/python_Levenshtein.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-01-31 22:43:20.000000 python-Levenshtein-0.24.0/python_Levenshtein.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-31 22:43:20.000000 python-Levenshtein-0.24.0/python_Levenshtein.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      857 2024-01-31 22:43:20.353145 python-Levenshtein-0.24.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 22:07:24.332229 python-Levenshtein-0.25.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    18085 2024-02-11 22:07:14.000000 python-Levenshtein-0.25.0/COPYING
+-rw-r--r--   0 runner    (1001) docker     (127)     7906 2024-02-11 22:07:14.000000 python-Levenshtein-0.25.0/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-02-11 22:07:14.000000 python-Levenshtein-0.25.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-02-11 22:07:24.332229 python-Levenshtein-0.25.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2835 2024-02-11 22:07:14.000000 python-Levenshtein-0.25.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-02-11 22:07:14.000000 python-Levenshtein-0.25.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 22:07:24.332229 python-Levenshtein-0.25.0/python_Levenshtein.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-02-11 22:07:24.000000 python-Levenshtein-0.25.0/python_Levenshtein.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-02-11 22:07:24.000000 python-Levenshtein-0.25.0/python_Levenshtein.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-11 22:07:24.000000 python-Levenshtein-0.25.0/python_Levenshtein.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-02-11 22:07:24.000000 python-Levenshtein-0.25.0/python_Levenshtein.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-11 22:07:24.000000 python-Levenshtein-0.25.0/python_Levenshtein.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      857 2024-02-11 22:07:24.332229 python-Levenshtein-0.25.0/setup.cfg
```

### Comparing `python-Levenshtein-0.24.0/COPYING` & `python-Levenshtein-0.25.0/COPYING`

 * *Files identical despite different names*

### Comparing `python-Levenshtein-0.24.0/HISTORY.md` & `python-Levenshtein-0.25.0/HISTORY.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 ## Changelog
 
+### v0.25.0
+#### Changed
+- improve type hints
+
 ### v0.24.0
 #### Changed
 - upgrade ``rapidfuzz-cpp`` to ``v3.0.0``
 - drop support for Python 3.7
 
 ### v0.23.0
 #### Changed
```

### Comparing `python-Levenshtein-0.24.0/PKG-INFO` & `python-Levenshtein-0.25.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-Levenshtein
-Version: 0.24.0
+Version: 0.25.0
 Summary: Python extension for computing string edit distances and similarities.
 Home-page: https://github.com/rapidfuzz/python-Levenshtein
 Author: Max Bachmann
 Author-email: pypi@maxbachmann.de
 License: GPL-2.0-or-later
 Keywords: string,Levenshtein,comparison,edit-distance
 Classifier: Programming Language :: Python :: 3
@@ -13,15 +13,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: COPYING
-Requires-Dist: Levenshtein==0.24.0
+Requires-Dist: Levenshtein==0.25.0
 
 # Levenshtein
 
 <p>
   <a href="https://github.com/rapidfuzz/python-Levenshtein/actions">
     <img src="https://github.com/rapidfuzz/python-Levenshtein/workflows/Build/badge.svg"
          alt="Continous Integration">
```

#### html2text {}

```diff
@@ -1,19 +1,19 @@
-Metadata-Version: 2.1 Name: python-Levenshtein Version: 0.24.0 Summary: Python
+Metadata-Version: 2.1 Name: python-Levenshtein Version: 0.25.0 Summary: Python
 extension for computing string edit distances and similarities. Home-page:
 https://github.com/rapidfuzz/python-Levenshtein Author: Max Bachmann Author-
 email: pypi@maxbachmann.de License: GPL-2.0-or-later Keywords:
 string,Levenshtein,comparison,edit-distance Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Programming Language :: Python :: 3.12 Classifier: License :: OSI Approved ::
 GNU General Public License v2 or later (GPLv2+) Requires-Python: >=3.8
 Description-Content-Type: text/markdown License-File: COPYING Requires-Dist:
-Levenshtein==0.24.0 # Levenshtein
+Levenshtein==0.25.0 # Levenshtein
 _[_C_o_n_t_i_n_o_u_s_ _I_n_t_e_g_r_a_t_i_o_n_]_[_P_y_P_I_ _p_a_c_k_a_g_e_ _v_e_r_s_i_o_n_]_[_P_y_t_h_o_n_ _v_e_r_s_i_o_n_s_]_[_D_o_c_u_m_e_n_t_a_t_i_o_n_]
 _[_G_i_t_H_u_b_ _l_i_c_e_n_s_e_]
 ## Introduction The Levenshtein Python C extension module contains functions
 for fast computation of: * Levenshtein (edit) distance, and edit operations *
 string similarity * approximate median strings, and generally string averaging
 * string sequence and set similarity > :warning: The package was renamed to
 `Levenshtein` and can be found [here](https://github.com/rapidfuzz/
```

### Comparing `python-Levenshtein-0.24.0/README.md` & `python-Levenshtein-0.25.0/README.md`

 * *Files identical despite different names*

### Comparing `python-Levenshtein-0.24.0/python_Levenshtein.egg-info/PKG-INFO` & `python-Levenshtein-0.25.0/python_Levenshtein.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-Levenshtein
-Version: 0.24.0
+Version: 0.25.0
 Summary: Python extension for computing string edit distances and similarities.
 Home-page: https://github.com/rapidfuzz/python-Levenshtein
 Author: Max Bachmann
 Author-email: pypi@maxbachmann.de
 License: GPL-2.0-or-later
 Keywords: string,Levenshtein,comparison,edit-distance
 Classifier: Programming Language :: Python :: 3
@@ -13,15 +13,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: COPYING
-Requires-Dist: Levenshtein==0.24.0
+Requires-Dist: Levenshtein==0.25.0
 
 # Levenshtein
 
 <p>
   <a href="https://github.com/rapidfuzz/python-Levenshtein/actions">
     <img src="https://github.com/rapidfuzz/python-Levenshtein/workflows/Build/badge.svg"
          alt="Continous Integration">
```

#### html2text {}

```diff
@@ -1,19 +1,19 @@
-Metadata-Version: 2.1 Name: python-Levenshtein Version: 0.24.0 Summary: Python
+Metadata-Version: 2.1 Name: python-Levenshtein Version: 0.25.0 Summary: Python
 extension for computing string edit distances and similarities. Home-page:
 https://github.com/rapidfuzz/python-Levenshtein Author: Max Bachmann Author-
 email: pypi@maxbachmann.de License: GPL-2.0-or-later Keywords:
 string,Levenshtein,comparison,edit-distance Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Programming Language :: Python :: 3.12 Classifier: License :: OSI Approved ::
 GNU General Public License v2 or later (GPLv2+) Requires-Python: >=3.8
 Description-Content-Type: text/markdown License-File: COPYING Requires-Dist:
-Levenshtein==0.24.0 # Levenshtein
+Levenshtein==0.25.0 # Levenshtein
 _[_C_o_n_t_i_n_o_u_s_ _I_n_t_e_g_r_a_t_i_o_n_]_[_P_y_P_I_ _p_a_c_k_a_g_e_ _v_e_r_s_i_o_n_]_[_P_y_t_h_o_n_ _v_e_r_s_i_o_n_s_]_[_D_o_c_u_m_e_n_t_a_t_i_o_n_]
 _[_G_i_t_H_u_b_ _l_i_c_e_n_s_e_]
 ## Introduction The Levenshtein Python C extension module contains functions
 for fast computation of: * Levenshtein (edit) distance, and edit operations *
 string similarity * approximate median strings, and generally string averaging
 * string sequence and set similarity > :warning: The package was renamed to
 `Levenshtein` and can be found [here](https://github.com/rapidfuzz/
```

### Comparing `python-Levenshtein-0.24.0/setup.cfg` & `python-Levenshtein-0.25.0/setup.cfg`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = python-Levenshtein
-version = 0.24.0
+version = 0.25.0
 description = Python extension for computing string edit distances and similarities.
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Max Bachmann
 author_email = pypi@maxbachmann.de
 url = https://github.com/rapidfuzz/python-Levenshtein
 license = GPL-2.0-or-later
@@ -17,13 +17,13 @@
 	Programming Language :: Python :: 3.12
 	License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 keywords = string, Levenshtein, comparison, edit-distance
 
 [options]
 python_requires = >=3.8
 install_requires = 
-	Levenshtein==0.24.0
+	Levenshtein==0.25.0
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

