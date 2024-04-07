# Comparing `tmp/commits2pdf-1.0.5.tar.gz` & `tmp/commits2pdf-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "commits2pdf-1.0.5.tar", last modified: Fri Mar 29 22:49:07 2024, max compression
+gzip compressed data, was "commits2pdf-1.1.5.tar", last modified: Sun Apr  7 11:37:24 2024, max compression
```

## Comparing `commits2pdf-1.0.5.tar` & `commits2pdf-1.1.5.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-03-29 22:49:07.497520 commits2pdf-1.0.5/
--rw-rw-rw-   0        0        0     1086 2024-03-28 09:30:12.000000 commits2pdf-1.0.5/LICENCE.md
--rw-rw-rw-   0        0        0     3072 2024-03-29 22:49:07.495525 commits2pdf-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     2256 2024-03-29 22:47:21.000000 commits2pdf-1.0.5/README.md
-drwxrwxrwx   0        0        0        0 2024-03-29 22:49:07.469595 commits2pdf-1.0.5/commits2pdf/
--rw-rw-rw-   0        0        0       21 2024-03-29 18:15:07.000000 commits2pdf-1.0.5/commits2pdf/__init__.py
--rw-rw-rw-   0        0        0     5194 2024-03-29 22:04:13.000000 commits2pdf-1.0.5/commits2pdf/cli.py
--rw-rw-rw-   0        0        0     4747 2024-03-29 21:53:43.000000 commits2pdf-1.0.5/commits2pdf/commits.py
--rw-rw-rw-   0        0        0      549 2024-03-29 20:20:06.000000 commits2pdf-1.0.5/commits2pdf/constants.py
--rw-rw-rw-   0        0        0      284 2024-03-29 21:52:02.000000 commits2pdf-1.0.5/commits2pdf/logger.py
--rw-rw-rw-   0        0        0     4740 2024-03-29 22:00:43.000000 commits2pdf-1.0.5/commits2pdf/render.py
-drwxrwxrwx   0        0        0        0 2024-03-29 22:49:07.494527 commits2pdf-1.0.5/commits2pdf.egg-info/
--rw-rw-rw-   0        0        0     3072 2024-03-29 22:49:07.000000 commits2pdf-1.0.5/commits2pdf.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      376 2024-03-29 22:49:07.000000 commits2pdf-1.0.5/commits2pdf.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-29 22:49:07.000000 commits2pdf-1.0.5/commits2pdf.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2024-03-29 22:49:07.000000 commits2pdf-1.0.5/commits2pdf.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       18 2024-03-29 22:49:07.000000 commits2pdf-1.0.5/commits2pdf.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-03-29 22:49:07.000000 commits2pdf-1.0.5/commits2pdf.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-29 22:49:07.497520 commits2pdf-1.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1153 2024-03-29 19:48:18.000000 commits2pdf-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-07 11:37:24.366410 commits2pdf-1.1.5/
+-rw-rw-rw-   0        0        0     1086 2024-03-28 09:30:12.000000 commits2pdf-1.1.5/LICENCE.md
+-rw-rw-rw-   0        0        0     7912 2024-04-07 11:37:24.365414 commits2pdf-1.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     7026 2024-04-07 11:27:11.000000 commits2pdf-1.1.5/README.md
+drwxrwxrwx   0        0        0        0 2024-04-07 11:37:24.346462 commits2pdf-1.1.5/commits2pdf/
+-rw-rw-rw-   0        0        0       21 2024-03-29 18:15:07.000000 commits2pdf-1.1.5/commits2pdf/__init__.py
+-rw-rw-rw-   0        0        0    10679 2024-04-07 10:52:13.000000 commits2pdf-1.1.5/commits2pdf/cli.py
+-rw-rw-rw-   0        0        0    12788 2024-04-07 09:56:11.000000 commits2pdf-1.1.5/commits2pdf/commits.py
+-rw-rw-rw-   0        0        0     3037 2024-04-07 10:09:48.000000 commits2pdf-1.1.5/commits2pdf/constants.py
+-rw-rw-rw-   0        0        0      308 2024-04-07 03:56:00.000000 commits2pdf-1.1.5/commits2pdf/logger.py
+-rw-rw-rw-   0        0        0     7100 2024-04-07 10:55:21.000000 commits2pdf-1.1.5/commits2pdf/render_cairo.py
+-rw-rw-rw-   0        0        0     9646 2024-04-07 11:29:41.000000 commits2pdf-1.1.5/commits2pdf/render_fpdf.py
+drwxrwxrwx   0        0        0        0 2024-04-07 11:37:24.364415 commits2pdf-1.1.5/commits2pdf.egg-info/
+-rw-rw-rw-   0        0        0     7912 2024-04-07 11:37:24.000000 commits2pdf-1.1.5/commits2pdf.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      409 2024-04-07 11:37:24.000000 commits2pdf-1.1.5/commits2pdf.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-07 11:37:24.000000 commits2pdf-1.1.5/commits2pdf.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2024-04-07 11:37:24.000000 commits2pdf-1.1.5/commits2pdf.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       23 2024-04-07 11:37:24.000000 commits2pdf-1.1.5/commits2pdf.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-07 11:37:24.000000 commits2pdf-1.1.5/commits2pdf.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-07 11:37:24.366410 commits2pdf-1.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     1223 2024-04-07 11:37:20.000000 commits2pdf-1.1.5/setup.py
```

### Comparing `commits2pdf-1.0.5/LICENCE.md` & `commits2pdf-1.1.5/LICENCE.md`

 * *Files identical despite different names*

### Comparing `commits2pdf-1.0.5/setup.py` & `commits2pdf-1.1.5/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,39 +1,41 @@
 from setuptools import setup, find_packages
 
 with open("README.md") as f:
     LONG_DESCRIPTION = f.read()
 
 setup(
     name="commits2pdf",
-    version="1.0.5",
+    version="1.1.5",
     author="Tomas Vana",
     url="https://github.com/tomasvana10/commits2pdf",
-    description="View commit history through a PDF",
+    description="View a filtered commit history in PDF form.",
     long_description=LONG_DESCRIPTION,
+    long_description_content_type="text/markdown",
     packages=find_packages(),
     license="MIT",
+    platforms="any",
     install_requires=[
         "GitPython",
-        "pycairo"
+        "pycairo",
+        "fpdf"
     ],
+    entry_points={
+        "console_scripts": [
+            "c2p = commits2pdf.cli:main"
+        ]
+    },
     classifiers=[
         "Topic :: Multimedia",
         "Development Status :: 5 - Production/Stable",
         "Environment :: Console",
         "Intended Audience :: End Users/Desktop",
         "Intended Audience :: Developers",
         "Intended Audience :: Education",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Topic :: Education",
         "Topic :: Office/Business",
-    ],
-    platforms="any",
-    entry_points={
-        "console_scripts": [
-            "commits2pdf = commits2pdf.cli:main"
-        ],
-    }
+    ]
 )
```

