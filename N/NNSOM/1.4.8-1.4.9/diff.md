# Comparing `tmp/nnsom-1.4.8.tar.gz` & `tmp/nnsom-1.4.9.tar.gz`

## Comparing `nnsom-1.4.8.tar` & `nnsom-1.4.9.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    76901 2020-02-02 00:00:00.000000 nnsom-1.4.8/src/NNSOM/plots.py
--rw-r--r--   0        0        0    10369 2020-02-02 00:00:00.000000 nnsom-1.4.8/src/NNSOM/som.py
--rw-r--r--   0        0        0    22430 2020-02-02 00:00:00.000000 nnsom-1.4.8/src/NNSOM/utils.py
--rw-r--r--   0        0        0    16114 2020-02-02 00:00:00.000000 nnsom-1.4.8/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nnsom-1.4.8/LICENSE
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 nnsom-1.4.8/README.md
--rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 nnsom-1.4.8/pyproject.toml
--rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 nnsom-1.4.8/PKG-INFO
+-rw-r--r--   0        0        0    76901 2020-02-02 00:00:00.000000 nnsom-1.4.9/src/NNSOM/plots.py
+-rw-r--r--   0        0        0    10369 2020-02-02 00:00:00.000000 nnsom-1.4.9/src/NNSOM/som.py
+-rw-r--r--   0        0        0    22430 2020-02-02 00:00:00.000000 nnsom-1.4.9/src/NNSOM/utils.py
+-rw-r--r--   0        0        0    16114 2020-02-02 00:00:00.000000 nnsom-1.4.9/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nnsom-1.4.9/LICENSE
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 nnsom-1.4.9/README.md
+-rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 nnsom-1.4.9/pyproject.toml
+-rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 nnsom-1.4.9/PKG-INFO
```

### Comparing `nnsom-1.4.8/src/NNSOM/plots.py` & `nnsom-1.4.9/src/NNSOM/plots.py`

 * *Files 0% similar despite different names*

```diff
@@ -1632,15 +1632,15 @@
                 # =============================================
 
                 # Call the pie plot
                 return selected_plot(sizes, **kwargs)
 
             elif plot_type == 'stem':
                 # Extract Align
-                if use_add_1darray:
+                if use_add_2darray:
                     align = [i for i in range(sizes.shape[1])]
                 else:
                     align = [i for i in range(len(np.unique(target)))]
                 # Call the stem plot
                 return selected_plot(align, sizes, **kwargs)
 
         elif plot_type in ['hist']:
```

### Comparing `nnsom-1.4.8/src/NNSOM/som.py` & `nnsom-1.4.9/src/NNSOM/som.py`

 * *Files identical despite different names*

### Comparing `nnsom-1.4.8/src/NNSOM/utils.py` & `nnsom-1.4.9/src/NNSOM/utils.py`

 * *Files identical despite different names*

### Comparing `nnsom-1.4.8/.gitignore` & `nnsom-1.4.9/.gitignore`

 * *Files identical despite different names*

### Comparing `nnsom-1.4.8/pyproject.toml` & `nnsom-1.4.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [tool.hatch.build.targets.sdist]
-include = ["src/NNSOM/**"]
+include = ["src/NNSOM/*.py"]
 
 [tool.hatch.build.targets.wheel]
 packages = ["src/NNSOM"]
 
 [project]
 name = "NNSOM"
-version = "1.4.8"
+version = "1.4.9"
 description = "A SOM package"
 readme = "README.md"
 requires-python = ">=3.8"
 license = { file = "LICENSE" }
 authors = [
   { name = "Dr. Hagan" },
   { name = "Dr. Amir Jafari", email = "amir.h.jafari@okstate.edu" },
```

### Comparing `nnsom-1.4.8/PKG-INFO` & `nnsom-1.4.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: NNSOM
-Version: 1.4.8
+Version: 1.4.9
 Summary: A SOM package
 Project-URL: Repository, https://github.com/amir-jafari/SOM
 Project-URL: Issues, https://github.com/amir-jafari/SOM/issues
 Author: Dr. Hagan, Lakshmi Sravya Chalapati, Ei Tanaka
 Author-email: "Dr. Amir Jafari" <amir.h.jafari@okstate.edu>
 Maintainer-email: "Dr. Amir Jafari" <amir.h.jafari@okstate.edu>
 License-File: LICENSE
```

