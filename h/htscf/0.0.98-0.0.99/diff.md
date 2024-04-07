# Comparing `tmp/htscf-0.0.98.tar.gz` & `tmp/htscf-0.0.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "htscf-0.0.98.tar", last modified: Wed Feb 21 12:40:50 2024, max compression
+gzip compressed data, was "htscf-0.0.99.tar", last modified: Wed Feb 21 13:56:36 2024, max compression
```

## Comparing `htscf-0.0.98.tar` & `htscf-0.0.99.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxrwx   0        0        0        0 2024-02-21 12:40:50.567335 htscf-0.0.98/
--rw-rw-rw-   0        0        0     1064 2023-10-25 05:23:47.000000 htscf-0.0.98/LICENSE
--rw-rw-rw-   0        0        0      209 2023-10-25 05:23:48.000000 htscf-0.0.98/MANIFEST.in
--rw-rw-rw-   0        0        0     5033 2024-02-21 12:40:50.566336 htscf-0.0.98/PKG-INFO
--rw-rw-rw-   0        0        0     4225 2024-02-20 09:06:02.000000 htscf-0.0.98/README.md
-drwxrwxrwx   0        0        0        0 2024-02-21 12:40:50.511766 htscf-0.0.98/htscf/
--rw-rw-rw-   0        0        0        0 2023-10-25 05:23:47.000000 htscf-0.0.98/htscf/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-21 12:40:50.541615 htscf-0.0.98/htscf/cli/
--rw-rw-rw-   0        0        0        0 2023-10-25 05:23:47.000000 htscf-0.0.98/htscf/cli/__init__.py
--rw-rw-rw-   0        0        0     1255 2024-02-20 08:14:44.000000 htscf-0.0.98/htscf/cli/bdc.py
--rw-rw-rw-   0        0        0     2269 2024-02-20 08:14:44.000000 htscf-0.0.98/htscf/cli/forceAnalysis.py
--rw-rw-rw-   0        0        0     1465 2024-02-20 08:14:44.000000 htscf-0.0.98/htscf/cli/login.py
--rw-rw-rw-   0        0        0     1370 2024-02-20 08:14:44.000000 htscf-0.0.98/htscf/cli/logout.py
--rw-rw-rw-   0        0        0     1620 2024-02-20 09:06:44.000000 htscf-0.0.98/htscf/cli/main.py
--rw-rw-rw-   0        0        0    25070 2024-02-21 12:40:28.000000 htscf-0.0.98/htscf/cli/pyband.py
--rw-rw-rw-   0        0        0      738 2024-02-20 08:14:44.000000 htscf-0.0.98/htscf/cli/qdelAll.py
--rw-rw-rw-   0        0        0     1173 2024-02-20 08:14:44.000000 htscf-0.0.98/htscf/cli/qstat.py
--rw-rw-rw-   0        0        0      436 2024-02-20 08:14:44.000000 htscf-0.0.98/htscf/cli/remote_sh.py
-drwxrwxrwx   0        0        0        0 2024-02-21 12:40:50.546613 htscf-0.0.98/htscf/core/
--rw-rw-rw-   0        0        0        0 2023-10-25 05:23:47.000000 htscf-0.0.98/htscf/core/__init__.py
--rw-rw-rw-   0        0        0      815 2023-10-25 05:23:47.000000 htscf-0.0.98/htscf/core/createStep.py
--rw-rw-rw-   0        0        0     3071 2023-10-28 10:46:12.000000 htscf-0.0.98/htscf/core/flow.py
-drwxrwxrwx   0        0        0        0 2024-02-21 12:40:50.549614 htscf-0.0.98/htscf/db/
--rw-rw-rw-   0        0        0        0 2023-10-25 05:23:47.000000 htscf-0.0.98/htscf/db/__init__.py
--rw-rw-rw-   0        0        0      257 2023-10-25 05:23:47.000000 htscf-0.0.98/htscf/db/mongo.py
-drwxrwxrwx   0        0        0        0 2024-02-21 12:40:50.552440 htscf-0.0.98/htscf/io/
--rw-rw-rw-   0        0        0        0 2023-10-25 05:23:47.000000 htscf-0.0.98/htscf/io/__init__.py
--rw-rw-rw-   0        0        0     4931 2023-10-25 05:23:47.000000 htscf-0.0.98/htscf/io/vaspIO.py
-drwxrwxrwx   0        0        0        0 2024-02-21 12:40:50.553320 htscf-0.0.98/htscf/test/
--rw-rw-rw-   0        0        0        0 2023-10-25 05:23:47.000000 htscf-0.0.98/htscf/test/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-21 12:40:50.563338 htscf-0.0.98/htscf/utils/
--rw-rw-rw-   0        0        0        0 2023-10-25 05:23:47.000000 htscf-0.0.98/htscf/utils/__init__.py
--rw-rw-rw-   0        0        0     4591 2023-11-02 12:51:57.000000 htscf-0.0.98/htscf/utils/flowHandler.py
--rw-rw-rw-   0        0        0     1972 2023-10-25 14:07:20.000000 htscf-0.0.98/htscf/utils/qsub.py
--rw-rw-rw-   0        0        0     1695 2024-02-21 11:25:18.000000 htscf-0.0.98/htscf/utils/remote_sh.py
--rw-rw-rw-   0        0        0     6929 2023-10-26 10:46:41.000000 htscf-0.0.98/htscf/utils/tools.py
-drwxrwxrwx   0        0        0        0 2024-02-21 12:40:50.565336 htscf-0.0.98/htscf.egg-info/
--rw-rw-rw-   0        0        0     5033 2024-02-21 12:40:48.000000 htscf-0.0.98/htscf.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      777 2024-02-21 12:40:50.000000 htscf-0.0.98/htscf.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-21 12:40:48.000000 htscf-0.0.98/htscf.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2024-02-21 12:40:48.000000 htscf-0.0.98/htscf.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        1 2023-10-25 05:23:48.000000 htscf-0.0.98/htscf.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      113 2024-02-21 12:40:48.000000 htscf-0.0.98/htscf.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-02-21 12:40:48.000000 htscf-0.0.98/htscf.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       80 2023-10-25 05:23:48.000000 htscf-0.0.98/pyproject.toml
--rw-rw-rw-   0        0        0      669 2024-02-21 12:40:50.568348 htscf-0.0.98/setup.cfg
--rw-rw-rw-   0        0        0      190 2023-10-25 05:23:47.000000 htscf-0.0.98/setup.py
+drwxrwxrwx   0        0        0        0 2024-02-21 13:56:36.876193 htscf-0.0.99/
+-rw-rw-rw-   0        0        0     1064 2023-10-25 05:23:47.000000 htscf-0.0.99/LICENSE
+-rw-rw-rw-   0        0        0      209 2023-10-25 05:23:48.000000 htscf-0.0.99/MANIFEST.in
+-rw-rw-rw-   0        0        0     5033 2024-02-21 13:56:36.875195 htscf-0.0.99/PKG-INFO
+-rw-rw-rw-   0        0        0     4225 2024-02-20 09:06:02.000000 htscf-0.0.99/README.md
+drwxrwxrwx   0        0        0        0 2024-02-21 13:56:36.800492 htscf-0.0.99/htscf/
+-rw-rw-rw-   0        0        0        0 2023-10-25 05:23:47.000000 htscf-0.0.99/htscf/__init__.py
+drwxrwxrwx   0        0        0        0 2024-02-21 13:56:36.836475 htscf-0.0.99/htscf/cli/
+-rw-rw-rw-   0        0        0        0 2023-10-25 05:23:47.000000 htscf-0.0.99/htscf/cli/__init__.py
+-rw-rw-rw-   0        0        0     1255 2024-02-20 08:14:44.000000 htscf-0.0.99/htscf/cli/bdc.py
+-rw-rw-rw-   0        0        0     2269 2024-02-20 08:14:44.000000 htscf-0.0.99/htscf/cli/forceAnalysis.py
+-rw-rw-rw-   0        0        0     1465 2024-02-20 08:14:44.000000 htscf-0.0.99/htscf/cli/login.py
+-rw-rw-rw-   0        0        0     1370 2024-02-20 08:14:44.000000 htscf-0.0.99/htscf/cli/logout.py
+-rw-rw-rw-   0        0        0     1620 2024-02-20 09:06:44.000000 htscf-0.0.99/htscf/cli/main.py
+-rw-rw-rw-   0        0        0    25269 2024-02-21 13:52:21.000000 htscf-0.0.99/htscf/cli/pyband.py
+-rw-rw-rw-   0        0        0      738 2024-02-20 08:14:44.000000 htscf-0.0.99/htscf/cli/qdelAll.py
+-rw-rw-rw-   0        0        0     1173 2024-02-20 08:14:44.000000 htscf-0.0.99/htscf/cli/qstat.py
+-rw-rw-rw-   0        0        0      436 2024-02-20 08:14:44.000000 htscf-0.0.99/htscf/cli/remote_sh.py
+drwxrwxrwx   0        0        0        0 2024-02-21 13:56:36.841480 htscf-0.0.99/htscf/core/
+-rw-rw-rw-   0        0        0        0 2023-10-25 05:23:47.000000 htscf-0.0.99/htscf/core/__init__.py
+-rw-rw-rw-   0        0        0      815 2023-10-25 05:23:47.000000 htscf-0.0.99/htscf/core/createStep.py
+-rw-rw-rw-   0        0        0     3071 2023-10-28 10:46:12.000000 htscf-0.0.99/htscf/core/flow.py
+drwxrwxrwx   0        0        0        0 2024-02-21 13:56:36.846483 htscf-0.0.99/htscf/db/
+-rw-rw-rw-   0        0        0        0 2023-10-25 05:23:47.000000 htscf-0.0.99/htscf/db/__init__.py
+-rw-rw-rw-   0        0        0      257 2023-10-25 05:23:47.000000 htscf-0.0.99/htscf/db/mongo.py
+drwxrwxrwx   0        0        0        0 2024-02-21 13:56:36.850479 htscf-0.0.99/htscf/io/
+-rw-rw-rw-   0        0        0        0 2023-10-25 05:23:47.000000 htscf-0.0.99/htscf/io/__init__.py
+-rw-rw-rw-   0        0        0     4931 2023-10-25 05:23:47.000000 htscf-0.0.99/htscf/io/vaspIO.py
+drwxrwxrwx   0        0        0        0 2024-02-21 13:56:36.852478 htscf-0.0.99/htscf/test/
+-rw-rw-rw-   0        0        0        0 2023-10-25 05:23:47.000000 htscf-0.0.99/htscf/test/__init__.py
+drwxrwxrwx   0        0        0        0 2024-02-21 13:56:36.869196 htscf-0.0.99/htscf/utils/
+-rw-rw-rw-   0        0        0        0 2023-10-25 05:23:47.000000 htscf-0.0.99/htscf/utils/__init__.py
+-rw-rw-rw-   0        0        0     4591 2023-11-02 12:51:57.000000 htscf-0.0.99/htscf/utils/flowHandler.py
+-rw-rw-rw-   0        0        0     1972 2023-10-25 14:07:20.000000 htscf-0.0.99/htscf/utils/qsub.py
+-rw-rw-rw-   0        0        0     1695 2024-02-21 11:25:18.000000 htscf-0.0.99/htscf/utils/remote_sh.py
+-rw-rw-rw-   0        0        0     6929 2023-10-26 10:46:41.000000 htscf-0.0.99/htscf/utils/tools.py
+drwxrwxrwx   0        0        0        0 2024-02-21 13:56:36.873202 htscf-0.0.99/htscf.egg-info/
+-rw-rw-rw-   0        0        0     5033 2024-02-21 13:56:34.000000 htscf-0.0.99/htscf.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      777 2024-02-21 13:56:36.000000 htscf-0.0.99/htscf.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-02-21 13:56:34.000000 htscf-0.0.99/htscf.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2024-02-21 13:56:34.000000 htscf-0.0.99/htscf.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        1 2023-10-25 05:23:48.000000 htscf-0.0.99/htscf.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      113 2024-02-21 13:56:34.000000 htscf-0.0.99/htscf.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-02-21 13:56:34.000000 htscf-0.0.99/htscf.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       80 2023-10-25 05:23:48.000000 htscf-0.0.99/pyproject.toml
+-rw-rw-rw-   0        0        0      669 2024-02-21 13:56:36.878195 htscf-0.0.99/setup.cfg
+-rw-rw-rw-   0        0        0      190 2023-10-25 05:23:47.000000 htscf-0.0.99/setup.py
```

### Comparing `htscf-0.0.98/LICENSE` & `htscf-0.0.99/LICENSE`

 * *Files identical despite different names*

### Comparing `htscf-0.0.98/PKG-INFO` & `htscf-0.0.99/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: htscf
-Version: 0.0.98
+Version: 0.0.99
 Summary: High-throughput computing flow
 Home-page: http://zhcloud.top
 Author: Hao Zhao
 Author-email: 601095001@qq.com
 License: OSI Approved :: MIT License
 Platform: Linux/Windows
 Classifier: Programming Language :: Python :: 3
```

### Comparing `htscf-0.0.98/README.md` & `htscf-0.0.99/README.md`

 * *Files identical despite different names*

### Comparing `htscf-0.0.98/htscf/cli/bdc.py` & `htscf-0.0.99/htscf/cli/bdc.py`

 * *Files identical despite different names*

### Comparing `htscf-0.0.98/htscf/cli/forceAnalysis.py` & `htscf-0.0.99/htscf/cli/forceAnalysis.py`

 * *Files identical despite different names*

### Comparing `htscf-0.0.98/htscf/cli/login.py` & `htscf-0.0.99/htscf/cli/login.py`

 * *Files identical despite different names*

### Comparing `htscf-0.0.98/htscf/cli/logout.py` & `htscf-0.0.99/htscf/cli/logout.py`

 * *Files identical despite different names*

### Comparing `htscf-0.0.98/htscf/cli/main.py` & `htscf-0.0.99/htscf/cli/main.py`

 * *Files identical despite different names*

### Comparing `htscf-0.0.98/htscf/cli/pyband.py` & `htscf-0.0.99/htscf/cli/pyband.py`

 * *Files 2% similar despite different names*

```diff
@@ -173,14 +173,19 @@
             action='store_true', dest='lsorbit',
             help='Spin orbit coupling on, special treament of PROCAR')
 
         add('-q', '--quiet',
             action='store_true', dest='quiet',
             help='not show the resulting image')
 
+        add('--xlabel',
+            action='store', type=str,
+            dest='xlabel', default=None,
+            help='设置x坐标描述')
+
     @staticmethod
     def run(args, parser):
 
         if args.occ:
 
             Nocc = len(args.occ)
             occM = ['o' for ii in range(Nocc)]
@@ -574,14 +579,16 @@
     for xx in opts.hlines:
         ax.axhline(y=xx, ls=':', color='k', lw=0.5, alpha=0.5)
     for yy in opts.vlines:
         ax.axhline(x=yy, ls=':', color='k', lw=0.5, alpha=0.5)
 
     ax.set_ylabel('Energy (eV)',  # fontsize='small',
                   labelpad=5)
+    if opts.xlabel:
+        ax.set_xlabel(opts.xlabel)
     ax.set_ylim(ymin, ymax)
     ax.set_xlim(kpath.min(), kpath.max())
 
     ax.set_xticks(kpt_bounds)
     if opts.kpts:
         kname = [x.upper() for x in opts.kpts]
         for ii in range(len(kname)):
```

### Comparing `htscf-0.0.98/htscf/cli/qdelAll.py` & `htscf-0.0.99/htscf/cli/qdelAll.py`

 * *Files identical despite different names*

### Comparing `htscf-0.0.98/htscf/cli/qstat.py` & `htscf-0.0.99/htscf/cli/qstat.py`

 * *Files identical despite different names*

### Comparing `htscf-0.0.98/htscf/core/createStep.py` & `htscf-0.0.99/htscf/core/createStep.py`

 * *Files identical despite different names*

### Comparing `htscf-0.0.98/htscf/core/flow.py` & `htscf-0.0.99/htscf/core/flow.py`

 * *Files identical despite different names*

### Comparing `htscf-0.0.98/htscf/io/vaspIO.py` & `htscf-0.0.99/htscf/io/vaspIO.py`

 * *Files identical despite different names*

### Comparing `htscf-0.0.98/htscf/utils/flowHandler.py` & `htscf-0.0.99/htscf/utils/flowHandler.py`

 * *Files identical despite different names*

### Comparing `htscf-0.0.98/htscf/utils/qsub.py` & `htscf-0.0.99/htscf/utils/qsub.py`

 * *Files identical despite different names*

### Comparing `htscf-0.0.98/htscf/utils/remote_sh.py` & `htscf-0.0.99/htscf/utils/remote_sh.py`

 * *Files identical despite different names*

### Comparing `htscf-0.0.98/htscf/utils/tools.py` & `htscf-0.0.99/htscf/utils/tools.py`

 * *Files identical despite different names*

### Comparing `htscf-0.0.98/htscf.egg-info/PKG-INFO` & `htscf-0.0.99/htscf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: htscf
-Version: 0.0.98
+Version: 0.0.99
 Summary: High-throughput computing flow
 Home-page: http://zhcloud.top
 Author: Hao Zhao
 Author-email: 601095001@qq.com
 License: OSI Approved :: MIT License
 Platform: Linux/Windows
 Classifier: Programming Language :: Python :: 3
```

### Comparing `htscf-0.0.98/htscf.egg-info/SOURCES.txt` & `htscf-0.0.99/htscf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `htscf-0.0.98/setup.cfg` & `htscf-0.0.99/setup.cfg`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2068 7473 6366 0d0a 7665 7273 696f   = htscf..versio
-00000020: 6e20 3d20 302e 302e 3938 0d0a 6465 7363  n = 0.0.98..desc
+00000020: 6e20 3d20 302e 302e 3939 0d0a 6465 7363  n = 0.0.99..desc
 00000030: 7269 7074 696f 6e20 3d20 4869 6768 2d74  ription = High-t
 00000040: 6872 6f75 6768 7075 7420 636f 6d70 7574  hroughput comput
 00000050: 696e 6720 666c 6f77 0d0a 6c6f 6e67 5f64  ing flow..long_d
 00000060: 6573 6372 6970 7469 6f6e 203d 2066 696c  escription = fil
 00000070: 653a 2052 4541 444d 452e 6d64 0d0a 6c6f  e: README.md..lo
 00000080: 6e67 5f64 6573 6372 6970 7469 6f6e 5f63  ng_description_c
 00000090: 6f6e 7465 6e74 5f74 7970 6520 3d20 7465  ontent_type = te
```

