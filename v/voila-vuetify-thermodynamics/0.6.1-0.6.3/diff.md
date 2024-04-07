# Comparing `tmp/voila-vuetify-thermodynamics-0.6.1.tar.gz` & `tmp/voila-vuetify-thermodynamics-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "voila-vuetify-thermodynamics-0.6.1.tar", last modified: Sat Apr  6 18:13:13 2024, max compression
+gzip compressed data, was "voila-vuetify-thermodynamics-0.6.3.tar", last modified: Sun Apr  7 18:36:43 2024, max compression
```

## Comparing `voila-vuetify-thermodynamics-0.6.1.tar` & `voila-vuetify-thermodynamics-0.6.3.tar`

### file list

```diff
@@ -1,30 +1,13 @@
-drwxr-xr-x   0 lukasbongartz   (501) staff       (20)        0 2024-04-06 18:13:13.653257 voila-vuetify-thermodynamics-0.6.1/
--rw-r--r--   0 lukasbongartz   (501) staff       (20)     1545 2024-04-06 00:47:42.000000 voila-vuetify-thermodynamics-0.6.1/LICENSE
--rw-r--r--   0 lukasbongartz   (501) staff       (20)       16 2024-04-06 00:47:42.000000 voila-vuetify-thermodynamics-0.6.1/MANIFEST.in
--rw-r--r--   0 lukasbongartz   (501) staff       (20)      395 2024-04-06 18:13:13.653165 voila-vuetify-thermodynamics-0.6.1/PKG-INFO
--rw-r--r--   0 lukasbongartz   (501) staff       (20)     1574 2024-04-06 00:47:42.000000 voila-vuetify-thermodynamics-0.6.1/README.md
--rw-r--r--   0 lukasbongartz   (501) staff       (20)      101 2024-04-06 18:13:13.654110 voila-vuetify-thermodynamics-0.6.1/setup.cfg
--rw-r--r--   0 lukasbongartz   (501) staff       (20)     3419 2024-04-06 18:12:41.000000 voila-vuetify-thermodynamics-0.6.1/setup.py
-drwxr-xr-x   0 lukasbongartz   (501) staff       (20)        0 2024-04-06 18:13:13.646936 voila-vuetify-thermodynamics-0.6.1/share/
-drwxr-xr-x   0 lukasbongartz   (501) staff       (20)        0 2024-04-06 18:13:13.647393 voila-vuetify-thermodynamics-0.6.1/share/jupyter/
-drwxr-xr-x   0 lukasbongartz   (501) staff       (20)        0 2024-04-06 18:13:13.647087 voila-vuetify-thermodynamics-0.6.1/share/jupyter/nbconvert/
-drwxr-xr-x   0 lukasbongartz   (501) staff       (20)        0 2024-04-06 18:13:13.647293 voila-vuetify-thermodynamics-0.6.1/share/jupyter/nbconvert/templates/
-drwxr-xr-x   0 lukasbongartz   (501) staff       (20)        0 2024-04-06 18:13:13.650090 voila-vuetify-thermodynamics-0.6.1/share/jupyter/nbconvert/templates/vuetify-base-thermodynamics/
--rw-r--r--   0 lukasbongartz   (501) staff       (20)     7797 2024-04-06 16:17:17.000000 voila-vuetify-thermodynamics-0.6.1/share/jupyter/nbconvert/templates/vuetify-base-thermodynamics/ansi.js
--rw-r--r--   0 lukasbongartz   (501) staff       (20)     1434 2024-04-06 16:17:17.000000 voila-vuetify-thermodynamics-0.6.1/share/jupyter/nbconvert/templates/vuetify-base-thermodynamics/app.html
--rw-r--r--   0 lukasbongartz   (501) staff       (20)       25 2024-04-06 16:17:17.000000 voila-vuetify-thermodynamics-0.6.1/share/jupyter/nbconvert/templates/vuetify-base-thermodynamics/conf.json
--rw-r--r--   0 lukasbongartz   (501) staff       (20)     3179 2024-04-06 16:17:17.000000 voila-vuetify-thermodynamics-0.6.1/share/jupyter/nbconvert/templates/vuetify-base-thermodynamics/index.html.j2
--rw-r--r--   0 lukasbongartz   (501) staff       (20)     7280 2024-04-06 16:17:17.000000 voila-vuetify-thermodynamics-0.6.1/share/jupyter/nbconvert/templates/vuetify-base-thermodynamics/util.js
-drwxr-xr-x   0 lukasbongartz   (501) staff       (20)        0 2024-04-06 18:13:13.650867 voila-vuetify-thermodynamics-0.6.1/share/jupyter/nbconvert/templates/vuetify-default-thermodynamics/
--rw-r--r--   0 lukasbongartz   (501) staff       (20)     5731 2024-04-06 18:03:54.000000 voila-vuetify-thermodynamics-0.6.1/share/jupyter/nbconvert/templates/vuetify-default-thermodynamics/app.html
--rw-r--r--   0 lukasbongartz   (501) staff       (20)       48 2024-04-06 16:23:13.000000 voila-vuetify-thermodynamics-0.6.1/share/jupyter/nbconvert/templates/vuetify-default-thermodynamics/conf.json
-drwxr-xr-x   0 lukasbongartz   (501) staff       (20)        0 2024-04-06 18:13:13.647466 voila-vuetify-thermodynamics-0.6.1/share/jupyter/voila/
-drwxr-xr-x   0 lukasbongartz   (501) staff       (20)        0 2024-04-06 18:13:13.647537 voila-vuetify-thermodynamics-0.6.1/share/jupyter/voila/templates/
-drwxr-xr-x   0 lukasbongartz   (501) staff       (20)        0 2024-04-06 18:13:13.651244 voila-vuetify-thermodynamics-0.6.1/share/jupyter/voila/templates/vuetify-base-thermodynamics/
--rw-r--r--   0 lukasbongartz   (501) staff       (20)     1772 2024-04-06 17:49:52.000000 voila-vuetify-thermodynamics-0.6.1/share/jupyter/voila/templates/vuetify-base-thermodynamics/index.html.j2
-drwxr-xr-x   0 lukasbongartz   (501) staff       (20)        0 2024-04-06 18:13:13.652873 voila-vuetify-thermodynamics-0.6.1/voila_vuetify_thermodynamics.egg-info/
--rw-r--r--   0 lukasbongartz   (501) staff       (20)      395 2024-04-06 18:13:13.000000 voila-vuetify-thermodynamics-0.6.1/voila_vuetify_thermodynamics.egg-info/PKG-INFO
--rw-r--r--   0 lukasbongartz   (501) staff       (20)      887 2024-04-06 18:13:13.000000 voila-vuetify-thermodynamics-0.6.1/voila_vuetify_thermodynamics.egg-info/SOURCES.txt
--rw-r--r--   0 lukasbongartz   (501) staff       (20)        1 2024-04-06 18:13:13.000000 voila-vuetify-thermodynamics-0.6.1/voila_vuetify_thermodynamics.egg-info/dependency_links.txt
--rw-r--r--   0 lukasbongartz   (501) staff       (20)       18 2024-04-06 18:13:13.000000 voila-vuetify-thermodynamics-0.6.1/voila_vuetify_thermodynamics.egg-info/requires.txt
--rw-r--r--   0 lukasbongartz   (501) staff       (20)        6 2024-04-06 18:13:13.000000 voila-vuetify-thermodynamics-0.6.1/voila_vuetify_thermodynamics.egg-info/top_level.txt
+drwxr-xr-x   0 lukasbongartz   (501) staff       (20)        0 2024-04-07 18:36:43.066551 voila-vuetify-thermodynamics-0.6.3/
+-rw-r--r--   0 lukasbongartz   (501) staff       (20)     1545 2024-04-07 17:10:33.000000 voila-vuetify-thermodynamics-0.6.3/LICENSE
+-rw-r--r--   0 lukasbongartz   (501) staff       (20)       16 2024-04-07 17:10:33.000000 voila-vuetify-thermodynamics-0.6.3/MANIFEST.in
+-rw-r--r--   0 lukasbongartz   (501) staff       (20)      322 2024-04-07 18:36:43.066452 voila-vuetify-thermodynamics-0.6.3/PKG-INFO
+-rw-r--r--   0 lukasbongartz   (501) staff       (20)     1574 2024-04-07 17:10:33.000000 voila-vuetify-thermodynamics-0.6.3/README.md
+-rw-r--r--   0 lukasbongartz   (501) staff       (20)      101 2024-04-07 18:36:43.066876 voila-vuetify-thermodynamics-0.6.3/setup.cfg
+-rw-r--r--   0 lukasbongartz   (501) staff       (20)     3340 2024-04-07 18:36:10.000000 voila-vuetify-thermodynamics-0.6.3/setup.py
+drwxr-xr-x   0 lukasbongartz   (501) staff       (20)        0 2024-04-07 18:36:43.066136 voila-vuetify-thermodynamics-0.6.3/voila_vuetify_thermodynamics.egg-info/
+-rw-r--r--   0 lukasbongartz   (501) staff       (20)      322 2024-04-07 18:36:43.000000 voila-vuetify-thermodynamics-0.6.3/voila_vuetify_thermodynamics.egg-info/PKG-INFO
+-rw-r--r--   0 lukasbongartz   (501) staff       (20)      307 2024-04-07 18:36:43.000000 voila-vuetify-thermodynamics-0.6.3/voila_vuetify_thermodynamics.egg-info/SOURCES.txt
+-rw-r--r--   0 lukasbongartz   (501) staff       (20)        1 2024-04-07 18:36:43.000000 voila-vuetify-thermodynamics-0.6.3/voila_vuetify_thermodynamics.egg-info/dependency_links.txt
+-rw-r--r--   0 lukasbongartz   (501) staff       (20)       18 2024-04-07 18:36:43.000000 voila-vuetify-thermodynamics-0.6.3/voila_vuetify_thermodynamics.egg-info/requires.txt
+-rw-r--r--   0 lukasbongartz   (501) staff       (20)        8 2024-04-07 18:36:43.000000 voila-vuetify-thermodynamics-0.6.3/voila_vuetify_thermodynamics.egg-info/top_level.txt
```

### Comparing `voila-vuetify-thermodynamics-0.6.1/LICENSE` & `voila-vuetify-thermodynamics-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `voila-vuetify-thermodynamics-0.6.1/README.md` & `voila-vuetify-thermodynamics-0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `voila-vuetify-thermodynamics-0.6.1/setup.py` & `voila-vuetify-thermodynamics-0.6.3/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -83,21 +83,20 @@
 for (dirpath, dirnames, filenames) in os.walk('share/jupyter/'):
     if filenames:
         data_files.append((dirpath, [os.path.join(dirpath, filename) for filename in filenames]))
 
 
 setup(
     name='voila-vuetify-thermodynamics',
-    version="0.6.1",
-    description="A vuetify template for Voila used for modeling thermodynamics",
+    version="0.6.3",
+    description="A vuetify template for Voila",
     data_files=data_files,
     install_requires=['voila>=0.2.0,<0.5'],
     include_package_data=True,
     author='Lukas Bongartz',
-    author_email='lukasbongartz@outlook.com',
     url='https://github.com/lukasbongartz/voila-vuetify-thermodynamics',
     keywords=[
         'ipython',
         'jupyter',
         'widgets',
         'voila'
     ],
```

