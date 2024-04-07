# Comparing `tmp/siunitpy-0.0.2.tar.gz` & `tmp/siunitpy-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "siunitpy-0.0.2.tar", last modified: Sun Jan 14 16:41:23 2024, max compression
+gzip compressed data, was "siunitpy-0.1.1.tar", last modified: Sun Apr  7 14:54:57 2024, max compression
```

## Comparing `siunitpy-0.0.2.tar` & `siunitpy-0.1.1.tar`

### file list

```diff
@@ -1,46 +1,68 @@
-drwxr-xr-x   0 dait      (1000) dait      (1000)        0 2024-01-14 16:41:23.311952 siunitpy-0.0.2/
--rw-r--r--   0 dait      (1000) dait      (1000)    35149 2024-01-13 18:25:13.000000 siunitpy-0.0.2/LICENSE
--rw-r--r--   0 dait      (1000) dait      (1000)     2783 2024-01-14 16:41:23.311952 siunitpy-0.0.2/PKG-INFO
--rw-r--r--   0 dait      (1000) dait      (1000)     2312 2024-01-14 16:15:56.000000 siunitpy-0.0.2/README.md
--rw-r--r--   0 dait      (1000) dait      (1000)      545 2024-01-14 14:18:59.000000 siunitpy-0.0.2/pyproject.toml
--rw-r--r--   0 dait      (1000) dait      (1000)       38 2024-01-14 16:41:23.311952 siunitpy-0.0.2/setup.cfg
-drwxr-xr-x   0 dait      (1000) dait      (1000)        0 2024-01-14 16:41:23.301952 siunitpy-0.0.2/src/
-drwxr-xr-x   0 dait      (1000) dait      (1000)        0 2024-01-14 16:41:23.301952 siunitpy-0.0.2/src/siunitpy/
-drwxr-xr-x   0 dait      (1000) dait      (1000)        0 2024-01-14 16:41:23.301952 siunitpy-0.0.2/src/siunitpy/SI/
--rw-r--r--   0 dait      (1000) dait      (1000)      851 2024-01-13 18:25:13.000000 siunitpy-0.0.2/src/siunitpy/SI/SIprefix.py
--rw-r--r--   0 dait      (1000) dait      (1000)     4561 2024-01-14 15:27:07.000000 siunitpy-0.0.2/src/siunitpy/SI/SIquantity.py
--rw-r--r--   0 dait      (1000) dait      (1000)     3530 2024-01-13 18:25:13.000000 siunitpy-0.0.2/src/siunitpy/SI/SIunit.py
--rw-r--r--   0 dait      (1000) dait      (1000)      113 2024-01-13 18:25:13.000000 siunitpy-0.0.2/src/siunitpy/SI/__init__.py
--rw-r--r--   0 dait      (1000) dait      (1000)      298 2024-01-13 18:25:13.000000 siunitpy-0.0.2/src/siunitpy/__init__.py
--rw-r--r--   0 dait      (1000) dait      (1000)     1167 2024-01-13 18:25:13.000000 siunitpy-0.0.2/src/siunitpy/constant.py
--rw-r--r--   0 dait      (1000) dait      (1000)     2843 2024-01-13 18:25:13.000000 siunitpy-0.0.2/src/siunitpy/dimension.py
--rw-r--r--   0 dait      (1000) dait      (1000)     3400 2024-01-13 18:25:13.000000 siunitpy-0.0.2/src/siunitpy/dimension.pyi
--rw-r--r--   0 dait      (1000) dait      (1000)     1568 2024-01-13 18:25:13.000000 siunitpy-0.0.2/src/siunitpy/dimensionconst.py
--rw-r--r--   0 dait      (1000) dait      (1000)     9403 2024-01-14 16:26:54.000000 siunitpy-0.0.2/src/siunitpy/quantity.py
--rw-r--r--   0 dait      (1000) dait      (1000)     1387 2024-01-13 18:25:13.000000 siunitpy-0.0.2/src/siunitpy/quntity.pyi
--rw-r--r--   0 dait      (1000) dait      (1000)     3026 2024-01-14 16:32:46.000000 siunitpy-0.0.2/src/siunitpy/temperature.py
-drwxr-xr-x   0 dait      (1000) dait      (1000)        0 2024-01-14 16:41:23.311952 siunitpy-0.0.2/src/siunitpy/templatelib/
--rw-r--r--   0 dait      (1000) dait      (1000)      205 2024-01-13 18:25:13.000000 siunitpy-0.0.2/src/siunitpy/templatelib/__init__.py
--rw-r--r--   0 dait      (1000) dait      (1000)     3068 2024-01-13 18:25:13.000000 siunitpy-0.0.2/src/siunitpy/templatelib/compound.py
--rw-r--r--   0 dait      (1000) dait      (1000)     1458 2024-01-13 18:25:13.000000 siunitpy-0.0.2/src/siunitpy/templatelib/compound.pyi
--rw-r--r--   0 dait      (1000) dait      (1000)      836 2024-01-13 18:25:13.000000 siunitpy-0.0.2/src/siunitpy/templatelib/constclass.py
--rw-r--r--   0 dait      (1000) dait      (1000)     4980 2024-01-13 18:25:13.000000 siunitpy-0.0.2/src/siunitpy/templatelib/continuedfraction.py
--rw-r--r--   0 dait      (1000) dait      (1000)     1080 2024-01-13 18:25:13.000000 siunitpy-0.0.2/src/siunitpy/templatelib/continuedfraction.pyi
--rw-r--r--   0 dait      (1000) dait      (1000)     2010 2024-01-13 18:25:13.000000 siunitpy-0.0.2/src/siunitpy/templatelib/utils.py
--rw-r--r--   0 dait      (1000) dait      (1000)      596 2024-01-13 18:25:13.000000 siunitpy-0.0.2/src/siunitpy/templatelib/value.py
--rw-r--r--   0 dait      (1000) dait      (1000)     8201 2024-01-14 13:14:25.000000 siunitpy-0.0.2/src/siunitpy/templatelib/vector.py
--rw-r--r--   0 dait      (1000) dait      (1000)     7307 2024-01-14 10:14:28.000000 siunitpy-0.0.2/src/siunitpy/templatelib/vector.pyi
--rw-r--r--   0 dait      (1000) dait      (1000)     5876 2024-01-14 13:18:29.000000 siunitpy-0.0.2/src/siunitpy/unit.py
--rw-r--r--   0 dait      (1000) dait      (1000)     3361 2024-01-14 08:44:11.000000 siunitpy-0.0.2/src/siunitpy/unit.pyi
--rw-r--r--   0 dait      (1000) dait      (1000)     5833 2024-01-14 13:32:45.000000 siunitpy-0.0.2/src/siunitpy/unit_analysis.py
--rw-r--r--   0 dait      (1000) dait      (1000)     4961 2024-01-14 13:10:39.000000 siunitpy-0.0.2/src/siunitpy/unit_data.py
--rw-r--r--   0 dait      (1000) dait      (1000)     1010 2024-01-13 18:25:13.000000 siunitpy-0.0.2/src/siunitpy/unitconst.py
-drwxr-xr-x   0 dait      (1000) dait      (1000)        0 2024-01-14 16:41:23.311952 siunitpy-0.0.2/src/siunitpy.egg-info/
--rw-r--r--   0 dait      (1000) dait      (1000)     2783 2024-01-14 16:41:23.000000 siunitpy-0.0.2/src/siunitpy.egg-info/PKG-INFO
--rw-r--r--   0 dait      (1000) dait      (1000)     1072 2024-01-14 16:41:23.000000 siunitpy-0.0.2/src/siunitpy.egg-info/SOURCES.txt
--rw-r--r--   0 dait      (1000) dait      (1000)        1 2024-01-14 16:41:23.000000 siunitpy-0.0.2/src/siunitpy.egg-info/dependency_links.txt
--rw-r--r--   0 dait      (1000) dait      (1000)        9 2024-01-14 16:41:23.000000 siunitpy-0.0.2/src/siunitpy.egg-info/top_level.txt
-drwxr-xr-x   0 dait      (1000) dait      (1000)        0 2024-01-14 16:41:23.311952 siunitpy-0.0.2/tests/
--rw-r--r--   0 dait      (1000) dait      (1000)      866 2024-01-14 14:16:06.000000 siunitpy-0.0.2/tests/test_dimension.py
--rw-r--r--   0 dait      (1000) dait      (1000)     1969 2024-01-14 14:02:25.000000 siunitpy-0.0.2/tests/test_unit.py
--rw-r--r--   0 dait      (1000) dait      (1000)     2671 2024-01-14 13:17:54.000000 siunitpy-0.0.2/tests/test_vector.py
+drwxr-xr-x   0 dait      (1000) dait      (1000)        0 2024-04-07 14:54:57.485809 siunitpy-0.1.1/
+-rw-r--r--   0 dait      (1000) dait      (1000)    35149 2024-01-13 18:25:13.000000 siunitpy-0.1.1/LICENSE
+-rw-r--r--   0 dait      (1000) dait      (1000)     2615 2024-04-07 14:54:57.485809 siunitpy-0.1.1/PKG-INFO
+-rw-r--r--   0 dait      (1000) dait      (1000)     2136 2024-04-07 14:42:51.000000 siunitpy-0.1.1/README.md
+-rw-r--r--   0 dait      (1000) dait      (1000)      554 2024-01-16 08:21:41.000000 siunitpy-0.1.1/pyproject.toml
+-rw-r--r--   0 dait      (1000) dait      (1000)       38 2024-04-07 14:54:57.485809 siunitpy-0.1.1/setup.cfg
+drwxr-xr-x   0 dait      (1000) dait      (1000)        0 2024-04-07 14:54:57.475809 siunitpy-0.1.1/src/
+drwxr-xr-x   0 dait      (1000) dait      (1000)        0 2024-04-07 14:54:57.475809 siunitpy-0.1.1/src/siunitpy/
+drwxr-xr-x   0 dait      (1000) dait      (1000)        0 2024-04-07 14:54:57.475809 siunitpy-0.1.1/src/siunitpy/SI/
+-rw-r--r--   0 dait      (1000) dait      (1000)      855 2024-02-03 10:41:47.000000 siunitpy-0.1.1/src/siunitpy/SI/SIprefix.py
+-rw-r--r--   0 dait      (1000) dait      (1000)     4635 2024-04-07 14:22:34.000000 siunitpy-0.1.1/src/siunitpy/SI/SIquantity.py
+-rw-r--r--   0 dait      (1000) dait      (1000)     3438 2024-02-09 09:07:57.000000 siunitpy-0.1.1/src/siunitpy/SI/SIunit.py
+-rw-r--r--   0 dait      (1000) dait      (1000)      113 2024-01-13 18:25:13.000000 siunitpy-0.1.1/src/siunitpy/SI/__init__.py
+-rw-r--r--   0 dait      (1000) dait      (1000)      315 2024-03-30 06:26:48.000000 siunitpy-0.1.1/src/siunitpy/__init__.py
+-rw-r--r--   0 dait      (1000) dait      (1000)      998 2024-04-07 14:26:39.000000 siunitpy-0.1.1/src/siunitpy/constant.py
+-rw-r--r--   0 dait      (1000) dait      (1000)     4636 2024-04-07 14:25:04.000000 siunitpy-0.1.1/src/siunitpy/constant.pyi
+drwxr-xr-x   0 dait      (1000) dait      (1000)        0 2024-04-07 14:54:57.475809 siunitpy-0.1.1/src/siunitpy/deprecated/
+-rw-r--r--   0 dait      (1000) dait      (1000)     1991 2024-02-14 08:30:31.000000 siunitpy-0.1.1/src/siunitpy/deprecated/quantity_unit.py
+-rw-r--r--   0 dait      (1000) dait      (1000)     3034 2024-02-09 08:55:11.000000 siunitpy-0.1.1/src/siunitpy/deprecated/temperature.py
+-rw-r--r--   0 dait      (1000) dait      (1000)      814 2023-08-06 17:17:01.000000 siunitpy-0.1.1/src/siunitpy/deprecated/test_slice.py
+-rw-r--r--   0 dait      (1000) dait      (1000)      610 2024-03-26 10:18:58.000000 siunitpy-0.1.1/src/siunitpy/deprecated/uncertainty.py
+-rw-r--r--   0 dait      (1000) dait      (1000)     3111 2023-07-30 12:18:16.000000 siunitpy-0.1.1/src/siunitpy/deprecated/vectordeprecated.py
+-rw-r--r--   0 dait      (1000) dait      (1000)     2921 2024-04-01 16:06:59.000000 siunitpy-0.1.1/src/siunitpy/dimension.py
+-rw-r--r--   0 dait      (1000) dait      (1000)     3405 2024-03-11 06:33:24.000000 siunitpy-0.1.1/src/siunitpy/dimension.pyi
+-rw-r--r--   0 dait      (1000) dait      (1000)     1942 2024-03-11 06:24:32.000000 siunitpy-0.1.1/src/siunitpy/dimensionconst.py
+-rw-r--r--   0 dait      (1000) dait      (1000)     1826 2024-04-01 16:45:15.000000 siunitpy-0.1.1/src/siunitpy/identity.py
+-rw-r--r--   0 dait      (1000) dait      (1000)     9037 2024-04-01 15:48:24.000000 siunitpy-0.1.1/src/siunitpy/quantity.py
+-rw-r--r--   0 dait      (1000) dait      (1000)     5220 2024-04-07 14:23:38.000000 siunitpy-0.1.1/src/siunitpy/quantity.pyi
+-rw-r--r--   0 dait      (1000) dait      (1000)     7403 2024-04-01 15:39:55.000000 siunitpy-0.1.1/src/siunitpy/unit.py
+-rw-r--r--   0 dait      (1000) dait      (1000)     3521 2024-03-20 13:34:22.000000 siunitpy-0.1.1/src/siunitpy/unit.pyi
+-rw-r--r--   0 dait      (1000) dait      (1000)     3230 2024-03-20 13:36:32.000000 siunitpy-0.1.1/src/siunitpy/unit_analysis.py
+-rw-r--r--   0 dait      (1000) dait      (1000)     6930 2024-03-21 13:05:34.000000 siunitpy-0.1.1/src/siunitpy/unit_archive.py
+-rw-r--r--   0 dait      (1000) dait      (1000)      991 2024-02-13 13:21:51.000000 siunitpy-0.1.1/src/siunitpy/unitconst.py
+-rw-r--r--   0 dait      (1000) dait      (1000)     1947 2024-03-25 13:55:43.000000 siunitpy-0.1.1/src/siunitpy/unitdata.py
+-rw-r--r--   0 dait      (1000) dait      (1000)     3071 2024-04-01 16:47:06.000000 siunitpy-0.1.1/src/siunitpy/unitelement.py
+drwxr-xr-x   0 dait      (1000) dait      (1000)        0 2024-04-07 14:54:57.485809 siunitpy-0.1.1/src/siunitpy/utilcollections/
+-rw-r--r--   0 dait      (1000) dait      (1000)      174 2024-03-30 10:05:39.000000 siunitpy-0.1.1/src/siunitpy/utilcollections/__init__.py
+drwxr-xr-x   0 dait      (1000) dait      (1000)        0 2024-04-07 14:54:57.485809 siunitpy-0.1.1/src/siunitpy/utilcollections/abc/
+-rw-r--r--   0 dait      (1000) dait      (1000)      133 2024-03-26 06:17:24.000000 siunitpy-0.1.1/src/siunitpy/utilcollections/abc/__init__.py
+-rw-r--r--   0 dait      (1000) dait      (1000)     1181 2024-04-07 14:38:27.000000 siunitpy-0.1.1/src/siunitpy/utilcollections/abc/linear.py
+-rw-r--r--   0 dait      (1000) dait      (1000)      959 2024-03-26 06:36:04.000000 siunitpy-0.1.1/src/siunitpy/utilcollections/abc/ordinal.py
+-rw-r--r--   0 dait      (1000) dait      (1000)      334 2024-03-26 06:13:19.000000 siunitpy-0.1.1/src/siunitpy/utilcollections/abc/supports.py
+-rw-r--r--   0 dait      (1000) dait      (1000)      191 2024-02-04 07:50:22.000000 siunitpy-0.1.1/src/siunitpy/utilcollections/abc/valuetype.py
+-rw-r--r--   0 dait      (1000) dait      (1000)     3626 2024-02-13 11:09:03.000000 siunitpy-0.1.1/src/siunitpy/utilcollections/compound.py
+-rw-r--r--   0 dait      (1000) dait      (1000)     1727 2024-02-09 15:01:09.000000 siunitpy-0.1.1/src/siunitpy/utilcollections/compound.pyi
+-rw-r--r--   0 dait      (1000) dait      (1000)      836 2024-01-13 18:25:13.000000 siunitpy-0.1.1/src/siunitpy/utilcollections/constclass.py
+-rw-r--r--   0 dait      (1000) dait      (1000)     4901 2024-02-02 11:05:42.000000 siunitpy-0.1.1/src/siunitpy/utilcollections/continuedfraction.py
+-rw-r--r--   0 dait      (1000) dait      (1000)     1127 2024-02-02 11:06:06.000000 siunitpy-0.1.1/src/siunitpy/utilcollections/continuedfraction.pyi
+-rw-r--r--   0 dait      (1000) dait      (1000)     7549 2024-02-07 12:41:32.000000 siunitpy-0.1.1/src/siunitpy/utilcollections/elementwiselist.py
+-rw-r--r--   0 dait      (1000) dait      (1000)     7302 2024-02-07 12:44:00.000000 siunitpy-0.1.1/src/siunitpy/utilcollections/elementwiselist.pyi
+-rw-r--r--   0 dait      (1000) dait      (1000)     1476 2024-03-26 01:03:31.000000 siunitpy-0.1.1/src/siunitpy/utilcollections/interval.py
+-rw-r--r--   0 dait      (1000) dait      (1000)      844 2024-03-26 01:05:39.000000 siunitpy-0.1.1/src/siunitpy/utilcollections/interval.pyi
+-rw-r--r--   0 dait      (1000) dait      (1000)     2559 2024-03-30 10:07:54.000000 siunitpy-0.1.1/src/siunitpy/utilcollections/utils.py
+-rw-r--r--   0 dait      (1000) dait      (1000)      324 2024-02-12 08:29:15.000000 siunitpy-0.1.1/src/siunitpy/value_archive.py
+-rw-r--r--   0 dait      (1000) dait      (1000)     7312 2024-04-07 14:38:36.000000 siunitpy-0.1.1/src/siunitpy/variable.py
+-rw-r--r--   0 dait      (1000) dait      (1000)     3861 2024-04-07 14:38:33.000000 siunitpy-0.1.1/src/siunitpy/variable.pyi
+drwxr-xr-x   0 dait      (1000) dait      (1000)        0 2024-04-07 14:54:57.485809 siunitpy-0.1.1/src/siunitpy.egg-info/
+-rw-r--r--   0 dait      (1000) dait      (1000)     2615 2024-04-07 14:54:57.000000 siunitpy-0.1.1/src/siunitpy.egg-info/PKG-INFO
+-rw-r--r--   0 dait      (1000) dait      (1000)     1836 2024-04-07 14:54:57.000000 siunitpy-0.1.1/src/siunitpy.egg-info/SOURCES.txt
+-rw-r--r--   0 dait      (1000) dait      (1000)        1 2024-04-07 14:54:57.000000 siunitpy-0.1.1/src/siunitpy.egg-info/dependency_links.txt
+-rw-r--r--   0 dait      (1000) dait      (1000)        9 2024-04-07 14:54:57.000000 siunitpy-0.1.1/src/siunitpy.egg-info/top_level.txt
+drwxr-xr-x   0 dait      (1000) dait      (1000)        0 2024-04-07 14:54:57.485809 siunitpy-0.1.1/tests/
+-rw-r--r--   0 dait      (1000) dait      (1000)      844 2024-03-11 06:26:47.000000 siunitpy-0.1.1/tests/test_dimension.py
+-rw-r--r--   0 dait      (1000) dait      (1000)     2807 2024-02-07 12:35:39.000000 siunitpy-0.1.1/tests/test_elementwiselist.py
+-rw-r--r--   0 dait      (1000) dait      (1000)      453 2024-02-03 10:42:14.000000 siunitpy-0.1.1/tests/test_interval.py
+-rw-r--r--   0 dait      (1000) dait      (1000)      742 2024-02-05 07:54:22.000000 siunitpy-0.1.1/tests/test_linear.py
+-rw-r--r--   0 dait      (1000) dait      (1000)     2018 2024-03-20 08:48:21.000000 siunitpy-0.1.1/tests/test_unit.py
+-rw-r--r--   0 dait      (1000) dait      (1000)     1254 2024-04-07 14:44:15.000000 siunitpy-0.1.1/tests/test_variable.py
```

### Comparing `siunitpy-0.0.2/LICENSE` & `siunitpy-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `siunitpy-0.0.2/PKG-INFO` & `siunitpy-0.1.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: siunitpy
-Version: 0.0.2
-Summary: A package for SI units and uncertainty
+Version: 0.1.1
+Summary: A package for SI unit, quantity and uncertainty
 Author-email: Dait <daitthu@qq.com>
 Project-URL: Homepage, https://github.com/DaitTHU/siunitpy
 Project-URL: Issues, https://github.com/DaitTHU/siunitpy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
@@ -18,15 +18,15 @@
 This package implements [NIST (National Institute of Standards and Technology)](https://www.nist.gov/pml/owm/metric-si/si-units) 
 official unit definitions. 
 
 Moreover, it introduce uncertainty.
 
 ## Installation
 
-pip installable package: [pypi: siunit](https://pypi.org/project/siunitpy/)
+pip installable package: [pypi: siunitpy](https://pypi.org/project/siunitpy/)
 
 ```shell
 pip install siunitpy
 ```
 
 ## Quickstart: module `siunitpy.SI`
 
@@ -35,15 +35,15 @@
 ### `SI`: common physical constants
 
 use physical constants through class `SI`:
 
 ```python
 >>> from siunitpy.SI import SI
 >>> SI.c
-Constant(value=299792458, unit=m/s, uncertainty=0)
+Constant(value=299792458, uncertainty=0, unit=m/s)
 >>> print(SI.me)
 9.1093837015e-31 ± 2.8e-40 kg
 >>> print(SI.me * SI.c**2)
 8.187105776823886e-14 ± 2.516514500463089e-23 J
 ```
 
 constant class `SI` provide physical constants defined by (or derived from) SI unit system.
@@ -82,32 +82,24 @@
 
 where `F` is a Quantity object, and it has properties:
 
 ```python
 >>> F.value
 1
 >>> F.unit
-Unit(kg·m/s², dim=(1, 1, -2, 0, 0, 0, 0), value=1)
+Unit(kg·m/s², dim=T⁻²LM, value=1)
 >>> F.dimension
-Dimension(L=1, M=1, T=-2, I=0, H=0, N=0, J=0)
+Dimension(T=-2, L=1, M=1, I=0, H=0, N=0, J=0)
 >>> L.uncertainty
 1e-4
 ```
 
 objects in `SI` are also Quantity objects.
 
 Quantity objects can make unit conversion and operate with number or Quantity:
 
 ```python
 >>> print(SI.me.to("keV/c2"))  # unit conversion
 510.99894999616424 ± 1.5706848090652466e-07 keV/c²
 >>> print(F / (1 * si.m)**2)
 1.0 Pa
 ```
-
-Especially, it provides temperature unit system:
-
-```python
->>> from siunitpy import degree
->>> print((100 * degree.F).to(degree.C.unit))
-37.77777777777778 °C
-```
```

### Comparing `siunitpy-0.0.2/README.md` & `siunitpy-0.1.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 This package implements [NIST (National Institute of Standards and Technology)](https://www.nist.gov/pml/owm/metric-si/si-units) 
 official unit definitions. 
 
 Moreover, it introduce uncertainty.
 
 ## Installation
 
-pip installable package: [pypi: siunit](https://pypi.org/project/siunitpy/)
+pip installable package: [pypi: siunitpy](https://pypi.org/project/siunitpy/)
 
 ```shell
 pip install siunitpy
 ```
 
 ## Quickstart: module `siunitpy.SI`
 
@@ -22,15 +22,15 @@
 ### `SI`: common physical constants
 
 use physical constants through class `SI`:
 
 ```python
 >>> from siunitpy.SI import SI
 >>> SI.c
-Constant(value=299792458, unit=m/s, uncertainty=0)
+Constant(value=299792458, uncertainty=0, unit=m/s)
 >>> print(SI.me)
 9.1093837015e-31 ± 2.8e-40 kg
 >>> print(SI.me * SI.c**2)
 8.187105776823886e-14 ± 2.516514500463089e-23 J
 ```
 
 constant class `SI` provide physical constants defined by (or derived from) SI unit system.
@@ -69,32 +69,24 @@
 
 where `F` is a Quantity object, and it has properties:
 
 ```python
 >>> F.value
 1
 >>> F.unit
-Unit(kg·m/s², dim=(1, 1, -2, 0, 0, 0, 0), value=1)
+Unit(kg·m/s², dim=T⁻²LM, value=1)
 >>> F.dimension
-Dimension(L=1, M=1, T=-2, I=0, H=0, N=0, J=0)
+Dimension(T=-2, L=1, M=1, I=0, H=0, N=0, J=0)
 >>> L.uncertainty
 1e-4
 ```
 
 objects in `SI` are also Quantity objects.
 
 Quantity objects can make unit conversion and operate with number or Quantity:
 
 ```python
 >>> print(SI.me.to("keV/c2"))  # unit conversion
 510.99894999616424 ± 1.5706848090652466e-07 keV/c²
 >>> print(F / (1 * si.m)**2)
 1.0 Pa
 ```
-
-Especially, it provides temperature unit system:
-
-```python
->>> from siunitpy import degree
->>> print((100 * degree.F).to(degree.C.unit))
-37.77777777777778 °C
-```
```

### Comparing `siunitpy-0.0.2/pyproject.toml` & `siunitpy-0.1.1/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "siunitpy"
-version = "0.0.2"
+version = "0.1.1"
 authors = [
   { name="Dait", email="daitthu@qq.com" },
 ]
-description = "A package for SI units and uncertainty"
+description = "A package for SI unit, quantity and uncertainty"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
 ]
```

### Comparing `siunitpy-0.0.2/src/siunitpy/SI/SIprefix.py` & `siunitpy-0.1.1/src/siunitpy/SI/SIprefix.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from ..templatelib.constclass import ConstClass
+from ..utilcollections.constclass import ConstClass
 
 __all__ = ['prefix']
 
 
 class prefix(ConstClass):
     # SI prefixes
     Q = quetta = 1e30
```

### Comparing `siunitpy-0.0.2/src/siunitpy/SI/SIquantity.py` & `siunitpy-0.1.1/src/siunitpy/SI/SIquantity.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from ..unit_data import _PI, _WEIN_ZERO
 from ..constant import Constant, constant
-from ..templatelib.constclass import ConstClass
+from ..value_archive import _PI, _WEIN_ZERO, _GRAVITY
+from ..utilcollections.constclass import ConstClass
 from .SIunit import si
 
 __all__ = ['SI']
 
 
 class SI(ConstClass):
     '''This constclass provides common physic constants,
@@ -49,26 +49,26 @@
     # first radiation constant
     c1 = constant((2 * _PI * h * c**2).ito('W.m2'))
     # first radiation constant for spectral radiance
     c1L = constant(c1 / Constant(_PI, 'sr'))
     # second radiation constant
     c2 = constant(h * c / kB)
     # conductance quantum
-    G0 = constant((2 * e**2 / h).isimplify_unit())
+    G0 = constant((2 * e**2 / h).simplify_unit(inplace=True))
     # Josephson constant
     KJ = constant((2 * e / h).ito('Hz/V'))
     # magnetic flux quantum
-    Phi0 = constant((1 / KJ).isimplify_unit())
+    Phi0 = constant((1 / KJ).simplify_unit(inplace=True))
     # von Klitzing constant
-    RK = constant((h / e**2).isimplify_unit())
+    RK = constant((h / e**2).simplify_unit(inplace=True))
 
     ### other defined exact constants
 
     # standard acceleration of gravity
-    g = Constant(9.80665, 'm/s2')
+    g = Constant(_GRAVITY, 'm/s2')
     # standard temperature
     T0 = Constant(273.15, 'K')
     # standard pressure
     p0 = constant(si.atm.to('Pa'))
     # molar volume of ideal gas
     Vm = constant((R * T0 / p0).ito('m3/mol'))
 
@@ -92,15 +92,15 @@
     mu0 = Constant(1.256_637_062_12e-6, 'H/m',
                    0.000_000_000_19e-6)
     # Coulomb constant
     ke = constant(1 / (4 * _PI * epsilon0))
     # magnetic constant
     km = constant(mu0 / (4 * _PI))
     # characteristic impedance of vacuum
-    Z0 = constant((mu0 / epsilon0).isimplify_unit().nthroot(2))
+    Z0 = constant((mu0 / epsilon0).simplify_unit(inplace=True).nthroot(2))
     # fine-structure constant
     alpha = constant(e**2 / (2 * epsilon0 * h * c))
     # inverse fine-structure constant
     alphainv = constant(1 / alpha)
     # particle mass
     me = Constant(9.109_383_7015e-31, 'kg',
                   0.000_000_0028e-31)
@@ -113,15 +113,15 @@
     mmu = Constant(1.883_531_627e-28, 'kg',
                    0.000_000_042e-28)
     mtau = Constant(3.167_54e-27, 'kg',
                     0.000_21e-27)
     # electron charge to mass quotient
     e_me = constant(e / me)
     # Compton wavelength
-    lambdaC = constant((h / (me * c)).isimplify_unit())
+    lambdaC = constant((h / (me * c)).simplify_unit(inplace=True))
     # classical electron radius
     re = constant(alpha * lambdaC / (2 * _PI))
     # Thomson cross section
     sigmae = constant(8 * _PI / 3 * re**2)
     # Bohr radius
     a0 = constant(re / alpha**2)
     # Rydberg constant = alpha**2 / 2 * lambdaC
```

### Comparing `siunitpy-0.0.2/src/siunitpy/SI/SIunit.py` & `siunitpy-0.1.1/src/siunitpy/SI/SIunit.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from ..templatelib.constclass import ConstClass
-from ..unitconst import UnitConst
 from ..constant import Constant
+from ..unitconst import UnitConst
+from ..utilcollections.constclass import ConstClass
 
 __all__ = ['si']
 
 
 def _base(unit: str):
     return lambda prefix: Constant.one(prefix + unit)
 
@@ -55,15 +55,15 @@
     V = Constant.one(UnitConst.VOLT)
     F = Constant.one(UnitConst.FARAD)
     ohm = Constant.one(UnitConst.OHM)
     S = Constant.one(UnitConst.SIEMENS)
     Wb = Constant.one(UnitConst.WEBER)
     T = Constant.one(UnitConst.TESLA)
     H = Constant.one(UnitConst.HENRY)
-    celsius = Constant.one(UnitConst.DEGREE_CELSIUS)
+    # celsius = Constant.one(UnitConst.DEGREE_CELSIUS)
     lm = Constant.one(UnitConst.LUMEN)
     lx = Constant.one(UnitConst.LUX)
     Bq = Constant.one(UnitConst.BECQUEREL)
     Gy = Constant.one(UnitConst.GRAY)
     Sv = Constant.one(UnitConst.SIEVERT)
     kat = Constant.one(UnitConst.KATAL)
     # common prefixed SI unit
@@ -86,10 +86,7 @@
     mL, L = map(_base('L'), 'm ')
     bar = Constant.one('bar')
     atm = Constant.one('atm')
     mmHg = Constant.one('mmHg')
     Wh, kWh = map(_base('Wh'), ' k')
     meV, eV, keV, MeV, GeV, TeV = map(_base('eV'), 'm kMGT')
     cal, kcal = map(_base('cal'), ' k')
-    Ci = Constant.one('Ci')
-    barn = Constant.one('barn')
-    Rontgen = Constant.one('Rontgen')
```

### Comparing `siunitpy-0.0.2/src/siunitpy/dimension.py` & `siunitpy-0.1.1/src/siunitpy/dimension.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,29 @@
-# TODO: add Fraction
-
 import operator
 from fractions import Fraction
 from typing import Callable, Iterable, SupportsIndex
 
-from .templatelib.utils import _inplace, common_rational
+from .utilcollections.utils import _inplace, common_rational
+from .utilcollections.utils import superscript as sup
 
 __all__ = ['Dimension']
 
-_DIM_VAR = ('L', 'M', 'T', 'I', 'H', 'N', 'J')
-_DIM_NUM = len(_DIM_VAR)
+_DIM_SYMBOL = ('T', 'L', 'M', 'I', 'H', 'N', 'J')
+_DIM_NUM = len(_DIM_SYMBOL)
 
 
 def _unpack_vector():
-    def __getter(i): return lambda self: self[i]  # closure
+    def __getter(i: int): return lambda self: self[i]  # closure
     return (property(__getter(i)) for i in range(_DIM_NUM))
 
 
-def _unary_op(op: Callable[[Fraction], Fraction]):
+def _unary(op: Callable[[Fraction], Fraction]):
     '''unary operation: +v, -v.'''
 
-    def __op(self: 'Dimension') -> 'Dimension': 
+    def __op(self: 'Dimension') -> 'Dimension':
         return Dimension.unpack(map(op, self))
     return __op
 
 
 def _vector_add(op: Callable[[Fraction, Fraction], Fraction]):
     '''vector addition: v + u, v - u.'''
 
@@ -40,58 +39,61 @@
         return Dimension.unpack(op(x, c) for x in self)
     return __op, _inplace(__op)
 
 
 class Dimension:
     __slots__ = ('__vector',)
 
-    def __init__(self, L=0, M=0, T=0, I=0, H=0, N=0, J=0) -> None:
-        dimension_vector = (L, M, T, I, H, N, J)
+    def __init__(self, T=0, L=0, M=0, I=0, H=0, N=0, J=0) -> None:
+        dimension_vector = (T, L, M, I, H, N, J)
         self.__vector = tuple(map(common_rational, dimension_vector))
 
     @classmethod
-    def unpack(cls, iterable: dict | Iterable, /): 
+    def unpack(cls, iterable: dict | Iterable, /):
         if isinstance(iterable, dict):
             return cls(**iterable)
         return cls(*iterable)
 
     def __getitem__(self, key: SupportsIndex): return self.__vector[key]
 
     def __iter__(self): return iter(self.__vector)
 
-    L, M, T, I, H, N, J = _unpack_vector()
-    length, mass, time, electric_current, thermodynamic_temperature, \
-        amount_of_substance, luminous_intensity = L, M, T, I, H, N, J
+    T, L, M, I, H, N, J = _unpack_vector()
+    time, length, mass, electric_current, thermodynamic_temperature, \
+        amount_of_substance, luminous_intensity = T, L, M, I, H, N, J
 
     def __repr__(self) -> str:
-        para = ', '.join(f'{var}={val}' for var, val in zip(_DIM_VAR, self))
-        return f'{self.__class__.__name__}({para})'
+        para = ', '.join(f'{s}={v}' for s, v in zip(_DIM_SYMBOL, self))
+        return '{}({})'.format(self.__class__.__name__, para)
 
-    def __str__(self) -> str: return '(' + ', '.join(map(str, self)) + ')'
+    def __str__(self) -> str: 
+        return ''.join(s + sup(v) for s, v in zip(_DIM_SYMBOL, self) if v)
 
     def __len__(self) -> int: return _DIM_NUM
 
     def __hash__(self) -> int: return hash(self.__vector)
 
     def __eq__(self, other: 'Dimension') -> bool:
         return self.__vector == other.__vector
 
-    __pos__ = _unary_op(operator.pos)
-    __neg__ = _unary_op(operator.neg)
+    __pos__ = _unary(operator.pos)
+    __neg__ = _unary(operator.neg)
 
     __add__, __iadd__ = _vector_add(operator.add)
     __sub__, __isub__ = _vector_add(operator.sub)
 
     __mul__, __imul__ = _scalar_mul(operator.mul)
     __rmul__ = __mul__
     __truediv__, __itruediv__ = _scalar_mul(operator.truediv)
-    
+
 
 if __name__ == '__main__':
-    a = '''length
-    mass
+    a = '''
     time
+    length
+    mass
     electric current
     thermodynamic temperature
     amount of substance
-    luminous intensity'''
+    luminous intensity
+    '''
     print(a.replace(' ', '_').upper())
```

### Comparing `siunitpy-0.0.2/src/siunitpy/dimension.pyi` & `siunitpy-0.1.1/src/siunitpy/dimension.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -2,77 +2,80 @@
 from typing import Iterable, Iterator, Literal, SupportsIndex
 
 __all__ = ['Dimension']
 
 
 class Dimension:
     '''`Dimension` is like a 7-len `namedtuple`, the field is
+    - `T`: time
     - `L`: length
     - `M`: mass
-    - `T`: time
     - `I`: electric current
-    - `H`: thermodynamic temperature (Θ)
+    - `H`: thermodynamic temperature (= Θ)
     - `N`: amount of substance
     - `J`: luminous intensity
 
+    It's a kind of immutable sequence.
+
     Get base quantity
     ---
     You can get base quantity property like mass by index, initial 
     or fullname.
     >>> force_dim[0]    # 1
     >>> force_dim.M     # 1
     >>> force_dim.time  # -2
 
     Operation
     ---
     a `Dimension` object is a linear vector in 7-dimension, so the
     operation is the same as vector in linear algebra.
-    >>> -force_dim                              # (-1, -1, 2, 0, ...)
-    >>> power_dim = force_dim + vilocity_dim    # (2, 1, -3, 0, ...)
-    >>> 2 * vilocity_dim                        # (2, 0, -2, ...)
+    >>> -force_dim                              # T⁻²LM
+    >>> power_dim = force_dim + vilocity_dim    # T⁻³L²M
+    >>> 2 * vilocity_dim                        # T⁻²L²
     '''
 
-    def __init__(self, L=0, M=0, T=0, I=0, H=0, N=0, J=0) -> None:
-        '''construct a `Dimension` object using 7 Fraction arguments, 
+    def __init__(self, T=0, L=0, M=0, I=0, H=0, N=0, J=0) -> None:
+        '''construct a `Dimension` object using 7 int/Fraction arguments, 
         default 0.
         >>> time_dim = Dimension(T=1)
-        >>> vilocity_dim = Dimension(1, 0, -1)
+        >>> vilocity_dim = Dimension(-1, 1)
 
         You can also use classmethod `Dimension.unpack` to construct a 
-        `Dimension` object from a `iterable`.
-        >>> force_dim = Dimension.unpack([1, 1, -2])
+        `Dimension` object from a iterable or dict.
+        >>> force_dim = Dimension.unpack([-2, 1, 1])
         >>> charge_dim = Dimension.unpack({'I': 1, 'T': 1})
         '''
 
     @classmethod
-    def unpack(cls, iterable: Iterable[int | float | Fraction] | 
-               dict[Literal['L', 'M', 'T', 'I', 'H', 'N', 'J'], int], /) -> Dimension: ...
+    def unpack(cls, iterable: Iterable[int] |
+               dict[Literal['T', 'L', 'M', 'I', 'H', 'N', 'J'], int], /) -> Dimension: ...
+
     def __getitem__(self, key: SupportsIndex) -> Fraction: ...
     def __iter__(self) -> Iterator[Fraction]: ...
     @property
+    def T(self) -> Fraction: '''time'''
+    @property
     def L(self) -> Fraction: '''length'''
     @property
     def M(self) -> Fraction: '''mass'''
     @property
-    def T(self) -> Fraction: '''time'''
-    @property
     def I(self) -> Fraction: '''electric current'''
     @property
     def H(self) -> Fraction: '''thermodynamic temperature'''
     @property
     def N(self) -> Fraction: '''amount of substance'''
     @property
     def J(self) -> Fraction: '''luminous intensity'''
     @property
+    def time(self) -> Fraction: ...
+    @property
     def length(self) -> Fraction: ...
     @property
     def mass(self) -> Fraction: ...
     @property
-    def time(self) -> Fraction: ...
-    @property
     def electric_current(self) -> Fraction: ...
     @property
     def thermodynamic_temperature(self) -> Fraction: ...
     @property
     def amount_of_substance(self) -> Fraction: ...
     @property
     def luminous_intensity(self) -> Fraction: ...
```

### Comparing `siunitpy-0.0.2/src/siunitpy/dimensionconst.py` & `siunitpy-0.1.1/src/siunitpy/dimensionconst.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,45 +1,59 @@
 from .dimension import Dimension
-from .templatelib.constclass import ConstClass
+from .utilcollections.constclass import ConstClass
 
 __all__ = ['DimensionConst']
 
 
 class DimensionConst(ConstClass):
     '''`DimensionConst` is an constclass containing constant `Dimension`
     objects, like dimensionless, 7 SI base units, and other derived units. 
     Units with different physical meanings sharing the same dimension, 
     like energy and work, have to share the same name `ENERGY`. 
     '''
     DIMENSIONLESS = Dimension()
+    TIME = Dimension(T=1)
     LENGTH = Dimension(L=1)
     MASS = Dimension(M=1)
-    TIME = Dimension(T=1)
     ELECTRIC_CURRENT = Dimension(I=1)
     THERMODYNAMIC_TEMPERATURE = Dimension(H=1)
     AMOUNT_OF_SUBSTANCE = Dimension(N=1)
     LUMINOUS_INTENSITY = Dimension(J=1)
-    # derived
+    # straight derived
+    PLANE_ANGLE = DIMENSIONLESS
+    SOLID_ANGLE = DIMENSIONLESS
     AREA = LENGTH * 2
     VOLUME = LENGTH * 3
     FREQUENCY = -TIME
+    # kinematics and dynamic
     VILOCITY = LENGTH - TIME
     ACCELERATOR = VILOCITY - TIME
     FORCE = MASS + ACCELERATOR
-    PRESSURE = FORCE - AREA  # stress
-    ENERGY = FORCE + LENGTH  # work
+    PRESSURE = FORCE - AREA
+    STRESS = PRESSURE
+    ENERGY = FORCE + LENGTH
+    WORK = ENERGY
+    HEAT = ENERGY
     POWER = ENERGY - TIME
+    HEAT_FLOW_RATE = POWER
     MOMENTUM = MASS + VILOCITY
-    # electirc-magnetic
+    # electrodynamics
     CHARGE = ELECTRIC_CURRENT + TIME
     VOLTAGE = POWER - ELECTRIC_CURRENT
+    ELECTROMOTIVE_FORCE = VOLTAGE
     CAPATITANCE = CHARGE - VOLTAGE
     RESISTANCE = VOLTAGE - ELECTRIC_CURRENT
     CONDUCTANCE = -RESISTANCE
     MAGNETIC_FLUX = VOLTAGE + TIME
-    MAGNETIC_INDUCTION = MAGNETIC_FLUX - AREA
+    MAGNETIC_FLUX_DENSITY = MAGNETIC_FLUX - AREA
+    MAGNETIC_INDUCTION = MAGNETIC_FLUX_DENSITY
     INDUCTANCE = MAGNETIC_FLUX - ELECTRIC_CURRENT
-    # LUMINOUS_FLUX = LUMINOUS_INTENSITY
+    # luminous
+    LUMINOUS_FLUX = LUMINOUS_INTENSITY + SOLID_ANGLE
     ILLUMINANCE = LUMINOUS_INTENSITY - AREA
-    KERMA = ENERGY - MASS  # or dose
+    # nuclear radiation
+    ACTIVITY = FREQUENCY  # of a radionuclide
+    KERMA = ENERGY - MASS
+    DOSE = KERMA
     EXPOSURE = CHARGE - MASS
+    # chemistry
     CATALYTIC_ACTIVITY = AMOUNT_OF_SUBSTANCE - TIME
```

### Comparing `siunitpy-0.0.2/src/siunitpy/quantity.py` & `siunitpy-0.1.1/src/siunitpy/quantity.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,55 +1,64 @@
 import operator
 from copy import copy
-from typing import Callable, Iterable
+from typing import Any, Callable, Generic, TypeVar
 
 from .dimension import Dimension
-from .templatelib.utils import _hypotenuse, _nthroot
+from .identity import Zero, zero
 from .unit import Unit
 from .unitconst import UnitConst
+from .utilcollections.abc import Linear
+from .variable import Variable
 
 __all__ = ['Quantity']
 
+T = TypeVar('T', bound=Linear)
+
+
+def _check_addable(left: 'Quantity', right: 'Quantity'):
+    try:
+        if left.unit.parallel(right.unit):
+            return
+        raise ValueError(f"dimension {left.dimension} != {right.dimension}.")
+    except AttributeError:
+        raise TypeError(f"'{type(right) = }' must be 'Quantity'.")
+
 
 def _comparison(op: Callable[[float, float], bool]):
     def __op(self, other):
         self.addable(other, assertTrue=True)
-        return op(self.value * self.unit.value,
-                  other.value * other.unit.value)
+        return op(self.variable * self.unit.value, other.variable * other.unit.value)
     return __op
 
 
-def _unary_op(op: Callable):
+def _unary(op: Callable):
     def __op(self: 'Quantity'):
-        return Quantity(op(self.value), self.unit, self.uncertainty)
+        return Quantity(op(self.variable), self.unit)
     return __op
 
 
 def _addsub(op: Callable, iop: Callable):
     '''operator: a + b, a - b, where a, b have to share
     the same dimension.
     '''
 
     def __op(self: 'Quantity', other: 'Quantity'):
         if self.is_dimensionless() and not isinstance(other, Quantity):
-            return Quantity(op(self.value, other), self.unit, self.uncertainty)
-        self.addable(other, assertTrue=True)
-        other_value = other.value * other.unit.value_over(self.unit)
-        return Quantity(op(self.value, other_value), self.unit,
-                        _hypotenuse(self.uncertainty, other.uncertainty))
+            return Quantity(op(self.variable, other), self.unit)
+        _check_addable(self, other)
+        other_var = other.variable * other.unit.value_over(self.unit)
+        return Quantity(op(self.variable, other_var), self.unit)
 
     def __iop(self: 'Quantity', other: 'Quantity'):
         if self.is_dimensionless() and not isinstance(other, Quantity):
-            self._value = iop(self.value, other)
+            self._variable = iop(self.variable, other)
             return self
-        self.addable(other, assertTrue=True)
-        other_value = other.value * other.unit.value_over(self.unit)
-        self._value = iop(self.value, other_value)
-        self._uncertainty = _hypotenuse(
-            self.uncertainty, other.uncertainty)
+        _check_addable(self, other)
+        self._variable = iop(self.variable, other.variable *
+                             other.unit.value_over(self.unit))
         return self
 
     return __op, __iop
 
 
 def _muldiv(op: Callable, iop: Callable, unitop: Callable[[Unit, Unit], Unit],
             pm: Callable[[Unit], Unit]):
@@ -57,199 +66,191 @@
 
     when a or b is not a `Quantity` object, which will be treated as a
     dimensionless Quantity.
     '''
 
     def __op(self: 'Quantity', other: 'Quantity'):
         if not isinstance(other, Quantity):
-            return Quantity(op(self.value, other), self.unit,
-                            op(self.uncertainty, abs(other)))
-        new_value = op(self.value, other.value)
+            return Quantity(op(self.variable, other), self.unit)
+        new_variable = op(self.variable, other.variable)
         new_unit = unitop(self.unit, other.unit)
-        if new_unit.parallel(UnitConst.DIMENSIONLESS):
-            new_value *= new_unit.value
+        if new_unit.is_dimensionless():
+            new_variable *= new_unit.value
             new_unit = UnitConst.DIMENSIONLESS
         else:
-            new_unit, factor = new_unit.simplify()
-            new_value *= factor
-        new_uncertainty = new_value * \
-            _hypotenuse(self.uncertainty / self.value,
-                        other.uncertainty / other.value)
-        return Quantity(new_value, new_unit, new_uncertainty)
+            new_unit, factor = new_unit.simplify_with_factor()
+            new_variable *= factor
+        return Quantity(new_variable, new_unit)
 
     def __iop(self: 'Quantity', other: 'Quantity'):
         if not isinstance(other, Quantity):
-            self._value = iop(self.value, other)
-            self._uncertainty = op(self.uncertainty, abs(other))
+            self._variable = iop(self.variable, other)
             return self
-        self._value = iop(self.value, other.value)
+        self._variable = iop(self.variable, other.variable)
         self._unit = unitop(self.unit, other.unit)
-        if self.unit.parallel(UnitConst.DIMENSIONLESS):
-            self._value *= self.unit.value
+        if self.unit.is_dimensionless():
+            self._variable *= self.unit.value
             self._unit = UnitConst.DIMENSIONLESS
         else:
-            self._unit, factor = self.unit.simplify()
-            self._value *= factor
-        self._uncertainty = self.value * \
-            _hypotenuse(self.uncertainty / self.value,
-                        other.uncertainty / other.value)
+            self._unit, factor = self.unit.simplify_with_factor()
+            self._variable *= factor
         return self
 
     def __rop(self: 'Quantity', other):
         '''other is not a `Quantity` object.'''
-        new_value = op(other, self.value)
-        new_uncertainty = new_value * self.uncertainty / self.value
-        return Quantity(new_value, pm(self.unit), new_uncertainty)
+        return Quantity(op(other, self._variable), pm(self.unit))
 
     return __op, __iop, __rop
 
 
-def _unit_deprefix(unit: Unit) -> tuple[Unit, float]: return unit.deprefix()
-def _unit_to_basic(unit: Unit) -> tuple[Unit, float]: return unit.to_basic()
-def _unit_simplify(unit: Unit) -> tuple[Unit, float]: return unit.simplify()
-
+class Quantity(Generic[T]):
+    __slots__ = ('_variable', '_unit')
 
-class Quantity:
-    
-    __slots__ = ('_value', '_unit', '_uncertainty')
-
-    def __init__(self, value: float, /,
+    def __init__(self, value: T | Variable[T], /,
                  unit: str | Unit = UnitConst.DIMENSIONLESS,
-                 uncertainty: float = 0) -> None:
+                 uncertainty: T | Zero = zero) -> None:
         if not isinstance(unit, (str, Unit)):
             raise TypeError(f"{type(unit) = } is not 'str' or 'Unit'.")
-        self._value = value
+        if isinstance(value, Variable):
+            self._variable = value
+        else:
+            self._variable = Variable(value, uncertainty)
         self._unit = Unit.move(unit)
-        self._uncertainty = uncertainty
 
     @classmethod
-    def one(cls, unit: str | Unit): return cls(1, unit, 0)
+    def one(cls, unit: str | Unit): return cls(1, unit)  # type: ignore
 
     @property
-    def value(self) -> float: return self._value
+    def variable(self) -> Variable[T]: return self._variable
     @property
-    def unit(self) -> Unit: return self._unit
+    def value(self) -> T: return self.variable.value
+    @property
+    def uncertainty(self) -> T | Zero: return self.variable.uncertainty
+
+    @property
+    def relative_uncertainty(self) -> T | Zero:
+        return self.variable.relative_uncertainty
+
     @property
-    def dimension(self) -> Dimension: return self._unit.dimension
+    def unit(self) -> Unit: return self._unit
     @property
-    def uncertainty(self) -> float: return self._uncertainty
+    def dimension(self) -> Dimension: return self.unit.dimension
 
     def __repr__(self) -> str:
-        return self.__class__.__name__ \
-            + f'(value={repr(self.value)}, unit={self.unit}, '\
-            f'uncertainty={self.uncertainty})'
+        return '{}(value={}, uncertainty={}, unit={})'.format(
+            self.__class__.__name__, self.value, self.uncertainty, self.unit
+        )
 
     def __str__(self) -> str:
-        value = str(self.value)
-        if not self.is_exact():
-            value += f' ± {self.uncertainty}'
         if self.unit == UnitConst.DIMENSIONLESS:
-            return value
-        return f'{value} {self.unit}'
+            return str(self.variable)
+        return f'{self.variable} {self.unit}'
+
+    def __format__(self, format_spec):
+        if self.unit == UnitConst.DIMENSIONLESS:
+            return format(self.variable, format_spec)
+        return f'{self.variable:{format_spec}} {self.unit}'
 
-    def is_exact(self) -> bool:
-        if isinstance(self.uncertainty, Iterable):
-            return all(unc == 0 for unc in self.uncertainty)
-        return self.uncertainty == 0
+    def is_exact(self) -> bool: return self._variable.is_exact()
 
     def is_dimensionless(self) -> bool:
         return self.unit == UnitConst.DIMENSIONLESS
 
     def copy(self) -> 'Quantity':
-        return Quantity(copy(self.value), self.unit, copy(self.uncertainty))
+        return Quantity(copy(self.variable), self.unit)
 
     def to(self, new_unit: str | Unit, *, assertDimension=True):
         '''unit transform.
         if assertDimension, raise Error when dimension unparallel.'''
         new_unit = Unit.move(new_unit)
-        if assertDimension:
-            self.unit.parallel(new_unit, assertTrue=True)
+        if assertDimension and not self.unit.parallel(new_unit):
+            raise ValueError(
+                f'dimension {self.unit.dimension} != {new_unit.dimension}.')
         factor = self.unit.value_over(new_unit)
-        return Quantity(self.value * factor, new_unit,
-                        self.uncertainty * factor)
+        return Quantity(self.variable * factor, new_unit)
 
     def ito(self, new_unit: str | Unit, *, assertDimension=True):
         '''inplace unit transform'''
         new_unit = Unit.move(new_unit)
-        if assertDimension:
-            self.unit.parallel(new_unit, assertTrue=True)
-        factor = self.unit.value_over(new_unit)
-        self._value *= factor
-        self._uncertainty *= factor
+        if assertDimension and not self.unit.parallel(new_unit):
+            raise ValueError(
+                f'dimension {self.unit.dimension} != {new_unit.dimension}.')
+        self._variable *= self.unit.value_over(new_unit)
         self._unit = new_unit
         return self
 
-    def __change_unit(self, unit_fun: Callable[[Unit], tuple[Unit, float]]):
-        new_unit, factor = unit_fun(self.unit)
-        return Quantity(self.value * factor, new_unit, self.uncertainty * factor)
-
-    def __ichange_unit(self, unit_fun: Callable[[Unit], tuple[Unit, float]]):
-        self._unit, factor = unit_fun(self.unit)
-        self._value *= factor
-        self._uncertainty *= factor
+    def deprefix_unit(self, *, inplace=False):
+        old_unit_value = self.unit.value
+        new_unit = self.unit.deprefix()
+        factor = old_unit_value / new_unit.value
+        if not inplace:
+            return Quantity(self.variable * factor, new_unit)
+        self._unit = new_unit
+        self._variable *= factor
         return self
 
-    def deprefix_unit(self) -> 'Quantity':
-        return self.__change_unit(_unit_deprefix)
-
-    def ideprefix_unit(self) -> 'Quantity':
-        return self.__ichange_unit(_unit_deprefix)
-
-    def to_basic_unit(self) -> 'Quantity':
-        return self.__change_unit(_unit_to_basic)
-
-    def ito_basic_unit(self) -> 'Quantity':
-        return self.__ichange_unit(_unit_to_basic)
-
-    def simplify_unit(self) -> 'Quantity':
-        return self.__change_unit(_unit_simplify)
+    def to_basic_unit(self, *, inplace=False) -> 'Quantity':
+        old_unit_value = self.unit.value
+        new_unit = self.unit.to_basic()
+        factor = old_unit_value / new_unit.value
+        if not inplace:
+            return Quantity(self.variable * factor, new_unit)
+        self._unit = new_unit
+        self._variable *= factor
+        return self
 
-    def isimplify_unit(self) -> 'Quantity':
-        return self.__ichange_unit(_unit_simplify)
+    def simplify_unit(self, *, inplace=False) -> 'Quantity':
+        old_unit_value = self.unit.value
+        new_unit = self.unit.simplify()
+        factor = old_unit_value / new_unit.value
+        if not inplace:
+            return Quantity(self.variable * factor, new_unit)
+        self._unit = new_unit
+        self._variable *= factor
+        return self
 
-    def addable(self, other, /, *, assertTrue=False) -> bool:
-        if not isinstance(other, Quantity):
-            raise TypeError(f"type of '{other}' is not Quantity.")
-        return self.unit.parallel(other.unit, assertTrue=assertTrue)
-    
     def remove_uncertainty(self) -> 'Quantity':
         return Quantity(self.value, self.unit)
 
     __eq__ = _comparison(operator.eq)
     __ne__ = _comparison(operator.ne)
     __gt__ = _comparison(operator.gt)
     __lt__ = _comparison(operator.lt)
     __ge__ = _comparison(operator.ge)
     __le__ = _comparison(operator.le)
 
-    __pos__ = _unary_op(operator.pos)
-    __neg__ = _unary_op(operator.neg)
+    __pos__ = _unary(operator.pos)
+    __neg__ = _unary(operator.neg)
 
     __add__, __iadd__ = _addsub(operator.add, operator.iadd)
     __sub__, __isub__ = _addsub(operator.sub, operator.isub)
 
     __mul__, __imul__, __rmul__ = _muldiv(
         operator.mul, operator.imul, operator.add, operator.pos)
     __matmul__, __imatmul__, __rmatmul__ = _muldiv(
         operator.matmul, operator.imatmul, operator.add, operator.pos)
-    # __floordiv__, __ifloordiv__, __rfloordiv__ = _muldiv(
-    #    operator.floordiv, operator.ifloordiv, operator.sub, operator.neg)
+    __floordiv__, __ifloordiv__, __rfloordiv__ = _muldiv(
+        operator.floordiv, operator.ifloordiv, operator.sub, operator.neg)
     __truediv__, __itruediv__, __rtruediv__ = _muldiv(
         operator.truediv, operator.itruediv, operator.sub, operator.neg)
 
     def __pow__(self, other):
-        new_value = self.value ** other
-        new_uncertainty = new_value * self.uncertainty / self.value
-        return Quantity(new_value, self.unit * other, new_uncertainty)
+        return Quantity(self.variable ** other, self.unit * other)
 
     def __ipow__(self, other):
-        old_value = copy(self._value)
-        self._value **= other
+        self._variable **= other
         self._unit *= other
-        self._uncertainty *= self.value * other / old_value
         return self
 
+    def __rpow__(self, other):
+        if not self.is_dimensionless():
+            raise ValueError("Quantity must be dimensionless as exponent.")
+        return other ** self.value
+
     def nthroot(self, n: int):
-        value = _nthroot(self._value, n)
-        unit = self._unit / n
-        uncertainty = self.uncertainty * value / (n * self.value)
-        return Quantity(value, unit, uncertainty)
+        '''n-th root of Quantity. e.g. square root when n = 2.'''
+        return Quantity(self.variable**(1 / n), self._unit / n)
+
+    __array_priority__ = 1000000000000
+
+    # def __array_ufunc__(self, ufunc, method, *inputs, **kwargs):
+    #     pass
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `siunitpy-0.0.2/src/siunitpy/temperature.py` & `siunitpy-0.1.1/src/siunitpy/deprecated/temperature.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from fractions import Fraction
 from typing import TypeVar, overload
 
-from .quantity import Quantity
-from .templatelib.constclass import ConstClass
-from .unit import Unit
-from .unitconst import UnitConst
+from ..quantity import Quantity
+from ..unit import Unit
+from ..unitconst import UnitConst
+from ..utilcollections.constclass import ConstClass
 
 __all__ = ['Temperature', 'degree']
 
 T = TypeVar('T', int, float)
 
 _ONE = Fraction(1)
 _FIVE_NINTHS = Fraction(5, 9)
```

### Comparing `siunitpy-0.0.2/src/siunitpy/templatelib/compound.py` & `siunitpy-0.1.1/src/siunitpy/utilcollections/compound.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,94 +1,107 @@
 import operator
-from itertools import chain
-from typing import TypeVar, Generic, Iterator, Iterable, Callable
 from fractions import Fraction
+from itertools import chain
+from typing import Callable, Generator, Generic, Iterable, Iterator, TypeVar
 
-from .utils import _inplace
+from .utils import Number, _inplace
+from .utils import common_rational as frac
 
 __all__ = ['Compound']
 
 K = TypeVar('K')
+_ZERO = Fraction(0)
 
 
 def _unary(op: Callable[[Fraction], Fraction]):
     def __op(self):
-        return Compound({key: op(val) for key, val in self.items()})
+        return Compound({k: op(v) for k, v in self.items()}, move_dict=True)
     return __op
 
 
-def _vector_add(op: Callable[[Fraction, Fraction], Fraction]):
+def _vector_add(op: Callable[[Fraction, Number], Fraction]):
     def __op(self, other):
-        dict_gen = ((key, op(self[key], other[key])) 
-                    for key in chain(self, other))
-        return Compound({key: val for key, val in dict_gen if val})
+        return Compound((k, op(self[k], other[k])) for k in chain(self, other))
     return __op, _inplace(__op)
 
 
-def _scalar_mul(op: Callable[[Fraction, Fraction | int], Fraction]):
+def _scalar_mul(op: Callable[[Fraction, Number], Fraction]):
     def __op(self, other):
         if other == 0:
-            return Compound({})
-        return Compound({key: op(val, other) 
-                            for key, val in self.items()})
+            return Compound()
+        return Compound((k, op(v, other)) for k, v in self.items())
     return __op, _inplace(__op)
 
 
 class Compound(Generic[K]):
     '''The class `Compound` is a `dict` whose keys are all the elements 
-    that make up a whole, and whose values are the corresponding 
-    contributions, which can of course be negative.
+    that make up the whole compound, and whose values are the corresponding 
+    contributions, which can be either postive or negative, but never zero.
+
+    Its function is similar to `defaultdict`. 
+    For keys not in the compound, the default values are 0. 
 
-    Its function is similar to `defaultdict`. The keys have a default 
-    value of 0. Moreover, when the value of the key in the `Compound` is 0, 
-    it will be automatically deleted, because elements with a contribution 
-    of 0 should not be taken into account.
+    Moreover, when the value of one key in the compound becomes 0, 
+    the key will be automatically deleted. 
+    Because elements with zero contribution should not be taken into account.
     '''
     __slots__ = ('_elements',)
 
-    def __init__(self, elements: dict[K, Fraction]):
-        '''elements should be a rvalue and guarantee no zero value.'''
-        self._elements = elements
+    def __init__(self, elements: dict[K, Fraction] |
+                 Generator[tuple[K, Number], None, None] = {}, /, *,
+                 move_dict=False):
+        if move_dict and isinstance(elements, dict):
+            self._elements = elements
+            return
+        if isinstance(elements, dict):
+            self._elements = {k: frac(v) for k, v in elements.items() if v}
+        elif isinstance(elements, (Iterable, Generator)):
+            self._elements = {k: frac(v) for k, v in elements if v}
 
     def __contains__(self, key: K) -> bool: return key in self._elements
 
     def __getitem__(self, key: K) -> Fraction:
-        return self._elements[key] if key in self._elements else Fraction(0)
+        return self._elements.get(key, _ZERO)
 
     def __setitem__(self, key: K, value: Fraction) -> None:
         if value == 0:
-            if key in self._elements:
-                del self._elements[key]
+            self._elements.pop(key, _ZERO)
         else:
             self._elements[key] = value
 
     def __delitem__(self, key: K) -> None: del self._elements[key]
 
     def __iter__(self) -> Iterator[K]: return iter(self._elements)
 
-    def __str__(self) -> str: return str(self._elements)
+    def __str__(self) -> str: return '{' \
+        + ', '.join(f'{k}: {v}' for k, v in self._elements.items()) + '}'
+
+    def __repr__(self) -> str: return '{' \
+        + ', '.join(f'{repr(k)}: {v}' for k, v in self._elements.items()) + '}'
 
     def __len__(self) -> int: return len(self._elements)
 
-    def copy(self): return Compound(self._elements.copy())
+    def copy(self): return Compound(self._elements.copy(), move_dict=True)
 
     def keys(self): return self._elements.keys()
 
     def values(self): return self._elements.values()
 
     def items(self): return self._elements.items()
 
     def pop(self, key) -> Fraction: return self._elements.pop(key)
 
-    def __eq__(self, other) -> bool:
+    def clear(self): self._elements.clear()
+
+    def __eq__(self, other: 'Compound') -> bool:
         return self._elements == other._elements
 
     __pos__ = _unary(operator.pos)  # like copy()
     __neg__ = _unary(operator.neg)
 
     __add__, __iadd__ = _vector_add(operator.add)
     __sub__, __isub__ = _vector_add(operator.sub)
 
     __mul__, __imul__ = _scalar_mul(operator.mul)
     __rmul__ = __mul__
     __truediv__, __itruediv__ = _scalar_mul(operator.truediv)
-    #__floordiv__, __ifloordiv__ = _scalar_mul(operator.floordiv)
+    # __floordiv__, __ifloordiv__ = _scalar_mul(operator.floordiv)
```

### Comparing `siunitpy-0.0.2/src/siunitpy/templatelib/compound.pyi` & `siunitpy-0.1.1/src/siunitpy/utilcollections/compound.pyi`

 * *Files 22% similar despite different names*

```diff
@@ -1,28 +1,36 @@
 from fractions import Fraction
-from typing import Generic, Iterator, Iterable, TypeVar, overload
+from typing import Any, Generic, Iterable, Iterator, TypeVar, overload
+
+from .utils import Number
 
 K = TypeVar('K')
 
 
 class Compound(Generic[K]):
-    def __init__(self, elements: dict[K, Fraction]): ...
+    @overload
+    def __init__(self) -> None: ...
+    @overload
+    def __init__(self, iterable: Iterable[tuple[K, Number]], /) -> None: ...
+    @overload
+    def __init__(self, elements: dict[K, Fraction], /, *, move_dict=False) -> None: ...
     def __contains__(self, key: K) -> bool: ...
     def __getitem__(self, key: K) -> Fraction: ...
     def __setitem__(self, key: K, value: Fraction) -> None: ...
     def __delitem__(self, key: K) -> None: ...
     def __iter__(self) -> Iterator[K]: ...
     def __str__(self) -> str: ...
     def __len__(self) -> int: ...
     def copy(self) -> Compound[K]: ...
     def keys(self) -> Iterable[K]: ...
     def values(self) -> Iterable[Fraction]: ...
     def items(self) -> Iterable[tuple[K, Fraction]]: ...
-    def pop(self, key) -> Fraction: ...
-    def __eq__(self, other) -> bool: ...
+    def pop(self, key: K) -> Fraction: ...
+    def clear(self) -> None: ...
+    def __eq__(self, other: Compound[Any]) -> bool: ...
     def __pos__(self) -> Compound[K]: ...
     def __neg__(self) -> Compound[K]: ...
     def __add__(self, other: Compound[K]) -> Compound[K]: ...
     def __sub__(self, other: Compound[K]) -> Compound[K]: ...
     def __mul__(self, other: int | Fraction) -> Compound[K]: ...
     def __truediv__(self, other: int | Fraction) -> Compound[K]: ...
     def __iadd__(self, other: Compound[K]) -> Compound[K]: ...
```

### Comparing `siunitpy-0.0.2/src/siunitpy/templatelib/constclass.py` & `siunitpy-0.1.1/src/siunitpy/utilcollections/constclass.py`

 * *Files identical despite different names*

### Comparing `siunitpy-0.0.2/src/siunitpy/templatelib/continuedfraction.py` & `siunitpy-0.1.1/src/siunitpy/utilcollections/continuedfraction.py`

 * *Files 6% similar despite different names*

```diff
@@ -72,18 +72,18 @@
     >>> ContinuedFraction.from_float(2.718281828)
 
     Moreover, you can set the len_limit and coefficient_limit.
     '''
     __slots__ = ('_coefficients',)
 
     def __init__(self, coefficients: Fraction | Iterable[int],
-                 *, _move_tuple: bool = False) -> None:
+                 *, copy_tuple: bool = True) -> None:
         if isinstance(coefficients, Fraction):
             coefficients = _frac2cfrac(coefficients)
-        elif _move_tuple and isinstance(coefficients, tuple):
+        elif not copy_tuple and isinstance(coefficients, tuple):
             self._coefficients = coefficients
             return
         self._coefficients = tuple(coefficients)
 
     @property
     def coefficients(self): return self._coefficients
 
@@ -92,60 +92,59 @@
                    coefficient_limit: int = 1000000):
         '''due to flaot precision, coefficients[10:] may have error.'''
         coefficients = _float2cfrac(number, len_limit, coefficient_limit)
         return cls(coefficients)
 
     def __repr__(self) -> str:
         return self.__class__.__name__ \
-            + repr(self._coefficients).replace(',', ';', 1)
+            + repr(self.coefficients).replace(',', ';', 1)
 
     def __str__(self) -> str:
-        return ' + 1/'.join(map(str, self._coefficients))
+        return ' + 1/'.join(map(str, self.coefficients))
 
-    def __len__(self) -> int: return len(self._coefficients)
+    def __len__(self) -> int: return len(self.coefficients)
 
-    def __iter__(self) -> Iterator[int]: return iter(self._coefficients)
+    def __iter__(self) -> Iterator[int]: return iter(self.coefficients)
 
-    def __hash__(self) -> int: return hash(self._coefficients)
+    def __hash__(self) -> int: return hash(self.coefficients)
 
-    def __getitem__(self, i: SupportsIndex): return self._coefficients[i]
+    def __getitem__(self, i: SupportsIndex): return self.coefficients[i]
 
     def __eq__(self, other) -> bool:
         if isinstance(other, ContinuedFraction):
-            return self._coefficients == other._coefficients
+            return self.coefficients == other.coefficients
         raise TypeError(f"comparing ContinuedFraction with {type(other)}.")
 
-    def __int__(self) -> int: return self._coefficients[0]
+    def __int__(self) -> int: return self.coefficients[0]
 
     def truncate(self, end_index: SupportsIndex):
-        return ContinuedFraction(self._coefficients[:end_index],
-                                 _move_tuple=True)
+        return ContinuedFraction(self.coefficients[:end_index], copy_tuple=False)
 
     def to_fraction(self) -> Fraction:
         p, q = 0, 1
-        for coef in reversed(self._coefficients):
+        for coef in reversed(self.coefficients):
             p, q = q, coef * q + p
         return Fraction(q, p)  # reverse again at last
 
     def reciprocal(self):
         '''get 1/fraction.'''
-        coef = self._coefficients[1:] if self._coefficients[0] == 0 \
-            else (0,) + self._coefficients
-        return ContinuedFraction(coef, _move_tuple=True)
+        coef = self.coefficients[1:] if self.coefficients[0] == 0 \
+            else (0,) + self.coefficients
+        return ContinuedFraction(coef, copy_tuple=False)
 
-    def represente(self, width: int | None = None) -> None:
+    def represent(self, width: int = -1) -> None:
         '''print
 
         a0 + _________1__________
              a1 + _______1_______
                   a2 + ____1_____
                        ... + 1/an
         '''
-        if len(self._coefficients) <= 1:
-            return print(self._coefficients[0])
-        cstrs = [str(c) + ' + ' for c in self._coefficients[:-1]]
-        cstrs[-1] += '1/' + str(self._coefficients[-1])
-        clens = list(accumulate(map(len, cstrs)))
-        width = clens[-1] if width is None else width
-        for cstr, clen in zip(cstrs, clens):
-            fline = f'{1:_^{clens[-1] - clen}}'
-            print((cstr + fline if len(fline) > 1 else cstr).rjust(width))
+        if len(self.coefficients) <= 1:
+            return print(self.coefficients[0])
+        coefs = [str(c) + ' + ' for c in self.coefficients[:-1]]
+        coefs[-1] += '1/' + str(self.coefficients[-1])
+        clens = list(accumulate(map(len, coefs)))
+        width = max(width, clens[-1])
+        for coef, clen in zip(coefs, clens):
+            line = f'{1:_^{clens[-1] - clen}}'
+            print((coef + line if len(line) > 1 else coef).rjust(width))
```

### Comparing `siunitpy-0.0.2/src/siunitpy/templatelib/continuedfraction.pyi` & `siunitpy-0.1.1/src/siunitpy/utilcollections/continuedfraction.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -5,16 +5,19 @@
 
 
 class ContinuedFraction:
     @overload
     def __init__(self, fraction: Fraction) -> None: ...
 
     @overload
-    def __init__(self, coefficients: Iterable[int],  
-                 *, _move_tuple: bool = False) -> None: ...
+    def __init__(self, coefficients: Iterable[int],
+                 *, copy_tuple: bool = True) -> None: ...
+
+    @property
+    def coefficients(self) -> tuple[int]: ...
 
     @classmethod
     def from_float(cls, number: float, *, len_limit: int = 10,
                    coefficient_limit: int = 1000000) -> ContinuedFraction: ...
 
     def __repr__(self) -> str: ...
     def __str__(self) -> str: ...
@@ -23,8 +26,8 @@
     def __hash__(self) -> int: ...
     def __getitem__(self, i: SupportsIndex) -> int: ...
     def __eq__(self, other: ContinuedFraction) -> bool: ...
     def __int__(self) -> int: ...
     def truncate(self, end_index: SupportsIndex) -> ContinuedFraction: ...
     def to_fraction(self) -> Fraction: ...
     def reciprocal(self) -> ContinuedFraction: ...
-    def represente(self, width: int | None = None) -> None: ...
+    def represent(self, width: int = -1) -> None: ...
```

### Comparing `siunitpy-0.0.2/src/siunitpy/templatelib/vector.py` & `siunitpy-0.1.1/src/siunitpy/utilcollections/elementwiselist.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,119 +1,127 @@
 # TODO: optimize __setitem__ and __delitem_
 
-# from __future__ import annotations
-
 import operator
-from typing import Callable, Iterable, Sequence, TypeVar
+from typing import (Callable, Generator, Iterable, Sequence, SupportsIndex,
+                    TypeVar)
 
-__all__ = ['Vector', 'VectorMatchError']
+__all__ = ['ElementWiseList']
 
 T = TypeVar('T')
 
 
 def _unary(op: Callable):
-    '''unary operation: +v, -v, not v, ~v...'''
+    '''4 unary operation: +v, -v, not v, ~v'''
 
-    def __op(self): return Vector(op(x) for x in self)
+    def __op(self): return ElementWiseList(op(x) for x in self)
     return __op
 
 
+def _length_equal(left, right):
+    try:
+        return isinstance(right, Sequence) and len(left) == len(right)
+    except TypeError:
+        raise TypeError('object to operator must be sequence.')
+
+
 def _comparison(op: Callable):
     def __op(self, other):
-        if Vector.match_length(self, other):
-            return Vector(op(x, y) for x, y in zip(self, other))
+        if _length_equal(self, other):
+            return ElementWiseList(op(x, y) for x, y in zip(self, other))
         else:
-            return Vector(op(x, other) for x in self)
+            return ElementWiseList(op(x, other) for x in self)
     return __op
 
 
 def _binary(op: Callable):
     '''binary operation: all are elementwise
-    - comparison: v > u, v == 0... (return Vector, not bool)
+    - comparison: v > u, v == 0... (return ElementWiseList[bool], not bool)
     - other binary operation: v + u, 2 * v...
     '''
 
     def __op(self, other):
-        if Vector.match_length(self, other):
-            return Vector(op(x, y) for x, y in zip(self, other))
+        if _length_equal(self, other):
+            return ElementWiseList(op(x, y) for x, y in zip(self, other))
         else:
-            return Vector(op(x, other) for x in self)
+            return ElementWiseList(op(x, other) for x in self)
 
     def __iop(self, other):
-        if Vector.match_length(self, other):
+        if _length_equal(self, other):
             for i in range(len(self)):
                 self[i] = op(self[i], other[i])
         else:
             for i in range(len(self)):
                 self[i] = op(self[i], other)
         return self
 
     def __rop(self, other):
-        if Vector.match_length(self, other):
-            return Vector(op(y, x) for x, y in zip(self, other))
+        if len(self) == len(other):
+            return ElementWiseList(op(y, x) for x, y in zip(self, other))
         else:
-            return Vector(op(other, x) for x in self)
+            return ElementWiseList(op(other, x) for x in self)
 
     return __op, __iop, __rop
 
 
-class Vector(list[T]):
+class ElementWiseList(list[T]):
 
     def __init__(self, iterable: Iterable[T] = (), /) -> None:
-        '''Construct a `Vector`
+        '''Construct a `ElementWiseList`
 
-        If no argument is given, the constructor creates a new empty Vector:
-        >>> Vector()  # []
+        If no argument is given, the constructor creates a new empty List:
+        >>> ElementWiseList()  # []
 
         The argument must be an iterable if specified:
-        >>> Vector([0, 1, 2, 3])  # [0, 1, 2, 3] 
-        >>> Vector(range(4))      # [0, 1, 2, 3]
+        >>> ElementWiseList([0, 1, 2, 3])  # [0, 1, 2, 3] 
+        >>> ElementWiseList(range(4))      # [0, 1, 2, 3]
 
-        If you want to packup multiple non-iterable elements as a `Vector`, 
-        use classmethod `Vector.packup(*args)`:
-        >>> Vector.packup(0, 1, 2, 3)  # [0, 1, 2, 3]
+        If you want to packup multiple non-iterable elements, 
+        use classmethod `cls.packup(*args)`:
+        >>> ElementWiseList.packup(0, 1, 2, 3)  # [0, 1, 2, 3]
         '''
         super().__init__(iterable)
 
     @classmethod
-    def packup(cls, *args: T):
-        return cls(args)
+    def packup(cls, *args: T): return cls(args)
 
     def __getitem__(self, index):
+        cls = self.__class__
         getter = super().__getitem__
         # get item
-        if isinstance(index, int):
+        if isinstance(index, SupportsIndex):
             return getter(index)
-        # get sub-Vector
+        # get sub-sequence
         if isinstance(index, slice):
-            return Vector(getter(index))
+            return cls(getter(index))
         # not an index
         if not isinstance(index, Iterable):
             raise TypeError(f'Inappropriate index type: {type(index)}')
         # boolean indexing
         if all(isinstance(idx, bool) for idx in index):
-            return Vector(getter(i) for i, idx in enumerate(index) if idx)
+            return cls(getter(i) for i, idx in enumerate(index) if idx)
         # advanced indexing
-        return Vector(getter(idx) for idx in index)
+        return cls(getter(idx) for idx in index)
 
     def __setitem__(self, index, value):
         setter = super().__setitem__
         # set element
-        if isinstance(index, int):
+        if isinstance(index, SupportsIndex):
             return setter(index, value)
-        # set sub-Vector
+        # set sub-sequence
         if isinstance(index, slice):
             if isinstance(value, Iterable):
                 return setter(index, value)
             for idx in range(len(self))[index]:
                 setter(idx, value)
             return
         # not an index
         if not isinstance(index, Iterable):
             raise TypeError(f'Inappropriate index type: {type(index)}')
+        elif isinstance(index, Generator):
+            index = tuple(index)
         # boolean indexing
         if all(isinstance(idx, bool) for idx in index):
             if isinstance(value, Iterable):
                 for i, (idx, val) in enumerate(zip(index, value)):
                     if idx:
                         setter(i, val)
             else:
@@ -127,97 +135,76 @@
                 setter(idx, val)
         else:
             for idx in index:
                 setter(idx, value)
 
     def __delitem__(self, index):
         killer = super().__delitem__
-        # delete item or sub-Vector
-        if isinstance(index, (int, slice)):
+        # delete item or sub-sequence
+        if isinstance(index, (SupportsIndex, slice)):
             return killer(index)
         # not an index
         if not isinstance(index, Iterable):
             raise TypeError(f'Inappropriate index type: {type(index)}')
+        elif isinstance(index, Generator):
+            index = tuple(index)
         # boolean indexing
         if all(isinstance(idx, bool) for idx in index):
             for i, idx in reversed(list(enumerate(index))):
                 if idx:
                     killer(i)
             return
         # advanced indexing
         for idx in sorted(index, reverse=True):
             killer(idx)
 
     @classmethod
     def cat(cls, left: Iterable, /, *rights):
-        '''concatenat Vectors, same as `sum(list)`'''
+        '''concatenat Lists, same as `sum(list)`'''
         result = list(left)
         for right in rights:
             result.extend(right)
         return cls(result)
 
     def repeat(self, repeat_time: int, /):
-        return Vector(super().__mul__(repeat_time))
+        return ElementWiseList(super().__mul__(repeat_time))
 
     def irepeat(self, repeat_time: int, /):
         '''inplacement repeat, same as `list` `*=`'''
         self = super().__imul__(repeat_time)
         return self
 
     def erepeat(self, repeat_time: int, /):
         '''element repeat, 
-        >>> Vector(range(2)).erepeat(3)
+        >>> ElementWiseList([0, 1]).erepeat(3)
         [0, 0, 0, 1, 1, 1]
         '''
-        return Vector(item for self_clone in zip(*([self] * repeat_time))
-                      for item in self_clone)
+        return self.__class__(item for self_clone in zip(*([self] * repeat_time))
+                              for item in self_clone)
 
-    @staticmethod
-    def zeros(length: int, /): return Vector([0]).irepeat(length)
+    @classmethod
+    def zeros(cls, length: int, /): return cls([0]).irepeat(length)
 
-    @staticmethod
-    def ones(length: int, /): return Vector([1]).irepeat(length)
+    @classmethod
+    def ones(cls, length: int, /): return cls([1]).irepeat(length)
 
-    def copy(self): return Vector(self)
+    def copy(self): return self.__class__(self)
 
     __pos__ = _unary(operator.pos)
     __neg__ = _unary(operator.neg)
     __not__ = _unary(operator.not_)
     __invert__ = _unary(operator.invert)
     __abs__ = _unary(operator.abs)
-
-    @staticmethod
-    def set_match_check(*, enable: bool) -> None:
-        '''If enabled, the match check mode will automatically check 
-        whether the two lengths are matched whenever the `Vector` are 
-        operated with the `Sequence`, and will raise `VectorMatchError`
-        if the lengths do not match.
-
-        If disabled, the check process will be omitted, but it may be
-        dangerous.
-        '''
-        VectorMatch._match_check = enable
-
-    @staticmethod
-    def match_length(left, right) -> bool:
-        '''see staticmethod Vector.set_match_check.'''
-        if not isinstance(right, Sequence):
-            return False
-        if VectorMatch._match_check and len(left) != len(right):
-            raise VectorMatchError(
-                f'Length ({len(left)}, {len(right)}) do not match.')
-        return True
-
     # comparison
-    __eq__ = _comparison(operator.eq)
-    __ne__ = _comparison(operator.ne)
-    __gt__ = _comparison(operator.gt)
-    __lt__ = _comparison(operator.lt)
-    __ge__ = _comparison(operator.ge)
-    __le__ = _comparison(operator.le)
+    __eq__ = _comparison(operator.eq)  # type: ignore
+    __ne__ = _comparison(operator.ne)  # type: ignore
+    __gt__ = _comparison(operator.gt)  # type: ignore
+    __lt__ = _comparison(operator.lt)  # type: ignore
+    __ge__ = _comparison(operator.ge)  # type: ignore
+    __le__ = _comparison(operator.le)  # type: ignore
     # operation
     __add__, __iadd__, __radd__ = _binary(operator.add)
     __sub__, __isub__, __rsub__ = _binary(operator.sub)
     __mul__, __imul__, __rmul__ = _binary(operator.mul)
     __matmul__, __imatmul__, __rmatmul__ = _binary(operator.matmul)
     __pow__, __ipow__, __rpow__ = _binary(operator.pow)
     __floordiv__, __ifloordiv__, __rfloordiv__ = _binary(operator.floordiv)
@@ -225,25 +212,7 @@
     __mod__, __imod__, __rmod__ = _binary(operator.mod)
     # bit
     __and__, __iand__, __rand__ = _binary(operator.and_)
     __or__, __ior__, __ror__ = _binary(operator.or_)
     __xor__, __ixor__, __rxor__ = _binary(operator.xor)
     __lshift__, __ilshift__, __rlshift__ = _binary(operator.lshift)
     __rshift__, __irshift__, __rrshift__ = _binary(operator.rshift)
-
-    @staticmethod
-    def equal(left, right) -> bool:
-        '''since `v == u` returns a `Vector`, the `Vector.equal(v, u)` assumes 
-        the function of determining whether `v`, `u` are equal or not.
-        '''
-        for l, r in zip(left, right, strict=True):
-            if l != r:
-                return False
-        return True
-
-
-class VectorMatch:
-    _match_check = True
-
-
-class VectorMatchError(Exception):
-    pass
```

### Comparing `siunitpy-0.0.2/src/siunitpy/unit.py` & `siunitpy-0.1.1/src/siunitpy/unit.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,28 @@
 import operator
 from fractions import Fraction
 from itertools import product
-from typing import Callable, Optional, Union, overload
+from math import prod
+from typing import Callable, Optional, overload
 
 from .dimension import Dimension
 from .dimensionconst import DimensionConst
-from .templatelib.compound import Compound
-from .templatelib.utils import _inplace, _nthroot
-from .unit_analysis import _combine, _deprefix, _resolve
-from .unit_data import _BASIC_SI, _UNIT_STD
+from .unit_analysis import _combine, _combine_fullname, _resolve
+from .unit_archive import _BASIC_SI, _PREFIX_DATA, _UNIT_DATA, _UNIT_STD
+from .unitelement import UnitElement
+from .utilcollections.compound import Compound
+from .utilcollections.utils import _inplace
 
-__all__ = ['Unit', 'UnitDimensionError', '_DIMENSIONLESS_UNIT']
+__all__ = ['Unit']
+
+_ONE, _TWO = Fraction(1), Fraction(2)
+_SIMPLE_EXPONENT = (-_ONE, _TWO, -_TWO)
+
+
+def _nthroot(a, b): return a ** (1 / b)
 
 
 def _vector_add(op: Callable, valop: Callable):
     '''vector addition: v + u, v - u.'''
 
     def __op(self: 'Unit', other: 'Unit'):
         return Unit(op(self._elements, other._elements),
@@ -25,129 +33,164 @@
 
 
 def _scalar_mul(op: Callable, valop: Callable):
     '''scalar multiplication: c * v, v / c.'''
 
     def __op(self: 'Unit', c):
         if c == 0:
-            return _DIMENSIONLESS_UNIT
+            return _UNIT_SIMPLE['']
         return Unit(op(self._elements, c),
                     dimension=op(self.dimension, c),
                     value=valop(self.value, c))
 
     return __op, _inplace(__op)
 
 
 class Unit:
-
-    __slots__ = ('_elements', '_dimension', '_value', '_symbol')
+    __slots__ = ('_elements', '_dimension', '_value')
 
     @overload
     def __init__(self, symbol: str) -> None: ...
 
     @overload
-    def __init__(self, elements: Compound[str],
+    def __init__(self, elements: Compound[UnitElement],
                  dimension: Dimension, value: float) -> None:
         '''The constructor is designed for private use, 
         please do NOT call it.
         '''
 
-    def __init__(self, symbol: str | Compound[str], /,  # type: ignore
+    def __init__(self, symbol: str | Compound[UnitElement], /,  # type: ignore
                  dimension: Optional[Dimension] = None,
                  value: float = 1) -> None:
         if isinstance(symbol, str):
-            self._elements, self._dimension, self._value = _resolve(symbol)
-            self._symbol = _combine(self._elements)
+            self._elements = _resolve(symbol)
+            dim_gen = (u.dimension * e for u, e in self._elements.items())
+            self._dimension = sum(dim_gen, start=DimensionConst.DIMENSIONLESS)
+            self._value = prod(u.value**e for u, e in self._elements.items())
+            if self.is_dimensionless() and self.value == 1:  # like "C²/F·J"
+                self._elements.clear()
+            if isinstance(self.value, float) and self.value.is_integer():
+                self._value = int(self.value)
             return
         elif dimension is None:
             raise TypeError(f"{type(symbol) = } must be 'str'.")
-        # developer mode, make sure type(symbol) is Compound[str]
-        if dimension == DimensionConst.DIMENSIONLESS:  # like 'C2/F·J'
-            self._elements: Compound[str] = Compound({})
-        else:
+        # developer mode, make sure type(symbol) is Compound
+        if dimension == DimensionConst.DIMENSIONLESS and value == 1:
+            self._elements: Compound[UnitElement] = Compound()
+        elif isinstance(symbol, Compound):
             self._elements = symbol  # no copy
+        else:
+            raise TypeError("Constructor takes only one argument.")
         self._dimension = dimension
         self._value = value
-        self._symbol = _combine(self._elements)
 
     @property
-    def symbol(self) -> str: return self._symbol
+    def symbol(self) -> str: return _combine(self._elements)
+    @property
+    def fullname(self) -> str: return _combine_fullname(self._elements)
     @property
     def dimension(self) -> Dimension: return self._dimension
     @property
     def value(self) -> float: return self._value
 
     def __repr__(self) -> str:
-        return self.__class__.__name__ + f'({self.symbol}, ' \
-            f'dim={self.dimension}, value={self.value})'
+        return '{}({}, dim={}, value={})'.format(
+            self.__class__.__name__, self.symbol, self.dimension, self.value
+        )
 
     def __str__(self) -> str: return self.symbol
 
-    def __hash__(self) -> int: return hash(self.symbol)
+    @staticmethod
+    def simple(symbol):
+        if symbol in _UNIT_SIMPLE:
+            return _UNIT_SIMPLE[symbol]
+        return Unit(symbol)
 
     @classmethod
-    def move(cls, unit: Union['Unit', str]) -> 'Unit':
-        '''type(unit) must be str or Unit'''
-        return Unit(unit) if isinstance(unit, str) else unit
-
-    def deprefix(self) -> tuple['Unit', float]:
-        '''return a new unit that remove all the prefix, 
-        and pop out the factor.
-        '''
-        elements, factor = _deprefix(self._elements)
-        deprefixed_unit = \
-            Unit(elements, self.dimension, self.value / factor)
-        return deprefixed_unit, factor
-
-    def to_basic(self) -> tuple['Unit', float]:
-        '''return a combination of `_BASIC_SI` unit with the same dimension, 
-        whose value = 1, thus the factor is self.value.
-        '''
-        elements = Compound(
-            {unit: e for unit, e in zip(_BASIC_SI, self.dimension) if e})
-        basic_unit = Unit(elements, self.dimension, 1)
-        return basic_unit, self.value
-
-    def simplify(self) -> tuple['Unit', float]:
-        '''if the complex unit can be simplified as m, m-1, m2, m-2, 
-        where m represents a `_BASIC_SI` unit. 
-        e.g. 
+    def move(cls, unit):
+        '''transform either str or Unit object to a Unit object.'''
+        if isinstance(unit, cls):
+            return unit
+        if isinstance(unit, str):
+            return cls(unit)
+        raise TypeError(f"{type(unit) = } must be 'str' or 'Unit'.")
+
+    def deprefix_with_factor(self):
+        elements = self._elements
+        factor = 1
+        for unit in self._elements:
+            if unit.symbol in _UNIT_DATA:  # not prefixed
+                continue
+            if elements is self._elements:
+                elements = self._elements.copy()
+            e = elements.pop(unit)
+            factor *= _PREFIX_DATA[unit.prefix].value ** e
+            if unit.base:  # not a single prefix
+                elements[unit.deprefix()] += e
+        return Unit(elements, self.dimension, self.value / factor), factor
+
+    def deprefix(self):
+        '''return a new unit that remove all the prefix.'''
+        return self.deprefix_with_factor()[0]
+
+    def to_basic_with_factor(self):
+        elements = Compound({UnitElement(unit): e for unit, e in
+                             zip(_BASIC_SI, self.dimension) if e}, move_dict=True)
+        return Unit(elements, self.dimension, 1), self.value
+
+    def to_basic(self):
+        '''return a combination of basic SI unit 
+        (i.e. m, kg, s, A, K, mol, cd) 
+        with the same dimension.
         '''
+        return self.to_basic_with_factor()[0]
+
+    def simplify_with_factor(self):
         if len(self._elements) < 2:
             return self, 1
         if self.dimension in _UNIT_STD:
             return Unit(_UNIT_STD[self.dimension]), self.value
-        for (dim, symbol), expo in product(_UNIT_STD.items(), (-1, 2, -2)):
+        for (dim, symbol), expo in product(_UNIT_STD.items(), _SIMPLE_EXPONENT):
             if dim * expo != self.dimension:
                 continue
-            return Unit(Compound({symbol: Fraction(expo)}),
-                        self.dimension, self.value), self.value
+            elements = Compound({UnitElement(symbol): expo}, move_dict=True)
+            return Unit(elements, self.dimension, 1), self.value
         return self, 1
 
+    def simplify(self):
+        '''if the complex unit can be simplified as m, m⁻¹, m², m⁻², 
+        where m represents a standard SI unit. 
+
+        e.g. the standard unit of voltage is V.
+        '''
+        return self.simplify_with_factor()[0]
+    
+    def __hash__(self) -> int:
+        return hash((self.dimension, self.value))
+
     def __eq__(self, other: 'Unit') -> bool:
         '''e.g. N == kg·m/s2'''
-        return self.dimension == other.dimension \
-            and self.value == other.value
+        return self.dimension == other.dimension and self.value == other.value
 
     def same_as(self, other: 'Unit') -> bool:
         '''e.g. N and kg.m/s2 are not the same element.'''
         return self._elements == other._elements
 
-    def parallel(self, other: 'Unit', /, *, assertTrue=False) -> bool:
-        '''if assertTrue, raise Error when dimension unparallel.'''
+    def parallel(self, other: 'Unit', /) -> bool:
+        '''two units parallel means their dimensions are the same.'''
         try:
             if self.dimension == other.dimension:
                 return True
         except AttributeError:
-            raise TypeError("parameter must be 'Unit' or 'Quantity'.")
-        if assertTrue:
-            raise UnitDimensionError(
-                f"dimension {self.dimension} != {other.dimension}.")
+            raise TypeError(f"{type(other) = } must be 'Unit' or 'Quantity'.")
         return False
 
+    def is_dimensionless(self) -> bool:
+        return self.dimension == DimensionConst.DIMENSIONLESS
+
     def value_over(self, other: 'Unit', /) -> float:
         '''return self.value / other.value.'''
         return self.value / other.value
 
     def __pos__(self): return self
 
     def __neg__(self):
@@ -158,12 +201,10 @@
     __sub__, __isub__ = _vector_add(operator.sub, operator.truediv)
 
     __mul__, __imul__ = _scalar_mul(operator.mul, operator.pow)
     __rmul__ = __mul__
     __truediv__, __itruediv__ = _scalar_mul(operator.truediv, _nthroot)
 
 
-_DIMENSIONLESS_UNIT = Unit('')
-
-
-class UnitDimensionError(Exception):
-    pass
+_UNIT_SIMPLE: dict[str, Unit] = {
+    symbol: Unit(symbol) for symbol in _UNIT_DATA
+}
```

### Comparing `siunitpy-0.0.2/src/siunitpy/unit.pyi` & `siunitpy-0.1.1/src/siunitpy/unit.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from fractions import Fraction
 from typing import Iterable
 
 from .dimension import Dimension
 
-__all__ = ['Unit', 'UnitDimensionError', '_DIMENSIONLESS_UNIT']
+__all__ = ['Unit']
 
 
 class Unit:
     '''`Unit` is a immutable object:
     - `symbol`: string expression of the unit.
     - `dimension`: `Dimension`, dimension of the unit.
     - `value`: 1 unit = ? standard-unit.
@@ -57,45 +57,48 @@
         >>> Unit('kg.m/s2')
         >>> Unit('MeV/c2')
         >>> Unit('T.W/m2.K4')
 
         - illegal expression example: 
 
         >>> Unit('x')   # UnitSymbolError: 'x' is not a valid unit.
-        >>> Unit('m+m') # 'm', because only substr before '+' is element
+        >>> Unit('m+m') # UnitSymbolError: 'm+m' is not a valid element unit.
         '''
     
     @property
     def symbol(self) -> str: ...
     @property
+    def fullname(self) -> str: ...
+    @property
     def dimension(self) -> Dimension: ...
     @property
     def value(self) -> float: ...
     def __repr__(self) -> str: ...
     def __str__(self) -> str: ...
     def __hash__(self) -> int: ...
+    @staticmethod
+    def simple(symbol: str) -> Unit: ...
     @classmethod
     def move(cls, unit: Unit | str) -> Unit: ...
-    def deprefix(self) -> tuple[Unit, float]: ...
-    def to_basic(self) -> tuple[Unit, float]: ...
-    def simplify(self) -> tuple[Unit, float]: ...
+    def deprefix_with_factor(self) -> tuple[Unit, float]: ...
+    def to_basic_with_factor(self) -> tuple[Unit, float]: ...
+    def simplify_with_factor(self) -> tuple[Unit, float]: ...
+    def deprefix(self) -> Unit: ...
+    def to_basic(self) -> Unit: ...
+    def simplify(self) -> Unit: ...
     def __eq__(self, other: Unit) -> bool: ...
     def same_as(self, other: Unit) -> bool: ...
-    def parallel(self, other: Unit, /, *, assertTrue=False) -> bool: ...
+    def parallel(self, other: Unit, /) -> bool: ...
+    def is_dimensionless(self) -> bool: ...
     def value_over(self, other: Unit, /) -> float: ...
     def __pos__(self): ...
     def __neg__(self): ...
     def __add__(self, other: Unit) -> Unit: ...
     def __sub__(self, other: Unit) -> Unit: ...
     def __mul__(self, other: int | Fraction) -> Unit: ...
     def __truediv__(self, other: int | Fraction) -> Unit: ...
     def __iadd__(self, other: Unit) -> Unit: ...
     def __isub__(self, other: Unit) -> Unit: ...
     def __imul__(self, other: int | Fraction) -> Unit: ...
     def __itruediv__(self, other: int | Fraction) -> Unit: ...
     def __rmul__(self, other: int | Fraction) -> Unit: ...
 
-
-_DIMENSIONLESS_UNIT = Unit('')
-
-
-class UnitDimensionError(Exception): ...
```

### Comparing `siunitpy-0.0.2/src/siunitpy/unitconst.py` & `siunitpy-0.1.1/src/siunitpy/unitconst.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-from .templatelib.constclass import ConstClass
-from .unit import _DIMENSIONLESS_UNIT, Unit
+from .unit import Unit
+from .utilcollections.constclass import ConstClass
 
 __all__ = ['UnitConst']
 
 
 class UnitConst(ConstClass):
     '''`UnitConst` is an constclass containing constant `Unit`
     objects, like dimensionless unit, 7 SI base units
     '''
-    DIMENSIONLESS = _DIMENSIONLESS_UNIT
+    DIMENSIONLESS = Unit.simple('')
     METER = Unit('m')
     KILOGRAM = Unit('kg')
     SECOND = Unit('s')
     AMPERE = Unit('A')
     KELVIN = Unit('K')
     MOLE = Unit('mol')
     CANDELA = Unit('cd')
@@ -28,14 +28,14 @@
     VOLT = Unit('V')
     FARAD = Unit('F')
     OHM = Unit('Ω')
     SIEMENS = Unit('S')
     WEBER = Unit('Wb')
     TESLA = Unit('T')
     HENRY = Unit('H')
-    DEGREE_CELSIUS = Unit('°C')
+    # DEGREE_CELSIUS = Unit('°C')
     LUMEN = Unit('lm')
     LUX = Unit('lx')
     BECQUEREL = Unit('Bq')
     GRAY = Unit('Gy')
     SIEVERT = Unit('Sv')
     KATAL = Unit('kat')
```

### Comparing `siunitpy-0.0.2/src/siunitpy.egg-info/PKG-INFO` & `siunitpy-0.1.1/src/siunitpy.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: siunitpy
-Version: 0.0.2
-Summary: A package for SI units and uncertainty
+Version: 0.1.1
+Summary: A package for SI unit, quantity and uncertainty
 Author-email: Dait <daitthu@qq.com>
 Project-URL: Homepage, https://github.com/DaitTHU/siunitpy
 Project-URL: Issues, https://github.com/DaitTHU/siunitpy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
@@ -18,15 +18,15 @@
 This package implements [NIST (National Institute of Standards and Technology)](https://www.nist.gov/pml/owm/metric-si/si-units) 
 official unit definitions. 
 
 Moreover, it introduce uncertainty.
 
 ## Installation
 
-pip installable package: [pypi: siunit](https://pypi.org/project/siunitpy/)
+pip installable package: [pypi: siunitpy](https://pypi.org/project/siunitpy/)
 
 ```shell
 pip install siunitpy
 ```
 
 ## Quickstart: module `siunitpy.SI`
 
@@ -35,15 +35,15 @@
 ### `SI`: common physical constants
 
 use physical constants through class `SI`:
 
 ```python
 >>> from siunitpy.SI import SI
 >>> SI.c
-Constant(value=299792458, unit=m/s, uncertainty=0)
+Constant(value=299792458, uncertainty=0, unit=m/s)
 >>> print(SI.me)
 9.1093837015e-31 ± 2.8e-40 kg
 >>> print(SI.me * SI.c**2)
 8.187105776823886e-14 ± 2.516514500463089e-23 J
 ```
 
 constant class `SI` provide physical constants defined by (or derived from) SI unit system.
@@ -82,32 +82,24 @@
 
 where `F` is a Quantity object, and it has properties:
 
 ```python
 >>> F.value
 1
 >>> F.unit
-Unit(kg·m/s², dim=(1, 1, -2, 0, 0, 0, 0), value=1)
+Unit(kg·m/s², dim=T⁻²LM, value=1)
 >>> F.dimension
-Dimension(L=1, M=1, T=-2, I=0, H=0, N=0, J=0)
+Dimension(T=-2, L=1, M=1, I=0, H=0, N=0, J=0)
 >>> L.uncertainty
 1e-4
 ```
 
 objects in `SI` are also Quantity objects.
 
 Quantity objects can make unit conversion and operate with number or Quantity:
 
 ```python
 >>> print(SI.me.to("keV/c2"))  # unit conversion
 510.99894999616424 ± 1.5706848090652466e-07 keV/c²
 >>> print(F / (1 * si.m)**2)
 1.0 Pa
 ```
-
-Especially, it provides temperature unit system:
-
-```python
->>> from siunitpy import degree
->>> print((100 * degree.F).to(degree.C.unit))
-37.77777777777778 °C
-```
```

### Comparing `siunitpy-0.0.2/tests/test_dimension.py` & `siunitpy-0.1.1/tests/test_dimension.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,26 @@
-import unittest
 import sys
+import unittest
+
 from src.siunitpy import Dimension, DimensionConst
 
 
 @unittest.skipIf(sys.version_info < (3, 9), 'only support 3.9+.')
 class TestDimension(unittest.TestCase):
     def test_init(self):
-        v = Dimension(1, 0, -1, 0, 0, 0, 0)
+        v = Dimension(-1, 1, 0, 0, 0, 0, 0)
         self.assertEqual(
-            repr(v), 'Dimension(L=1, M=0, T=-1, I=0, H=0, N=0, J=0)')
-        self.assertEqual(str(v), '(1, 0, -1, 0, 0, 0, 0)')
+            repr(v), 'Dimension(T=-1, L=1, M=0, I=0, H=0, N=0, J=0)')
+        self.assertEqual(str(v), 'T⁻¹L')
         self.assertEqual(v.L, 1)
         self.assertEqual(v.mass, 0)
         self.assertEqual(v.time, -1)
 
     def test_operation(self):
         dl = DimensionConst.LENGTH
         dm = DimensionConst.MASS
         dt = DimensionConst.TIME
         dv = DimensionConst.VILOCITY
         df = DimensionConst.FORCE
-        self.assertEqual(str(-df), '(-1, -1, 2, 0, 0, 0, 0)')
+        self.assertEqual(str(-df), 'T²L⁻¹M⁻¹')
         self.assertEqual(dl - dt, dv)
         self.assertEqual(dm + dl - dt * 2, df)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `siunitpy-0.0.2/tests/test_unit.py` & `siunitpy-0.1.1/tests/test_unit.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,44 +1,44 @@
-import unittest
 import sys
+import unittest
+
 from src.siunitpy import Dimension, DimensionConst, Unit, UnitConst
 
 
 @unittest.skipIf(sys.version_info < (3, 9), 'only support 3.9+.')
 class TestUnit(unittest.TestCase):
     def test_init(self):
         u0 = Unit('kg.m/s2')
-        self.assertEqual(
-            repr(u0), 'Unit(kg·m/s², dim=(1, 1, -2, 0, 0, 0, 0), value=1)')
+        self.assertEqual(repr(u0), 'Unit(kg·m/s², dim=T⁻²LM, value=1)')
         self.assertEqual(u0.symbol, 'kg·m/s²')
         self.assertEqual(u0.dimension, DimensionConst.FORCE)
         self.assertEqual(u0.value, 1)
-        u1 = Unit('kg.m/s²')
+        u1 = Unit('kilogram.meter/second2')
         self.assertEqual(repr(u1), repr(u0))
         u2 = Unit('MeV/c2')
         self.assertEqual(u2.symbol, 'MeV/c²')
         self.assertEqual(u2.dimension, DimensionConst.MASS)
         self.assertEqual(u2.value, 1.7826619216278976e-30)
-        u3 = Unit('MeV/c²')
+        u3 = Unit('megaelectronvolt/speed-of-light2')
         self.assertEqual(repr(u3), repr(u3))
         u4 = Unit('T.W/m2.K4')
         self.assertEqual(u4.symbol, 'T·W/m²·K⁴')
-        self.assertEqual(u4.dimension, Dimension(0, 2, -5, -1, -4, 0, 0))
+        self.assertEqual(u4.dimension, Dimension(-5, 0, 2, -1, -4, 0, 0))
         self.assertEqual(u4.value, 1)
 
     def test_operation(self):
         u0 = Unit("MeV/c")
-        u1, factor1 = u0.deprefix()
+        u1, factor1 = u0.deprefix_with_factor()
         self.assertEqual(u1.symbol, "eV/c")
         self.assertEqual(factor1, 1000_000)
-        u2, factor2 = u0.to_basic()
+        u2, factor2 = u0.to_basic_with_factor()
         self.assertEqual(u2.symbol, "m·kg/s")
         self.assertEqual(factor2, 5.3442859926783075e-22)
         self.assertEqual(u0.value_over(Unit(u2.symbol)), factor2)
-        u3, factor3 = Unit("V/mA").simplify()
+        u3, factor3 = Unit("V/mA").simplify_with_factor()
         self.assertEqual(u3.symbol, "Ω")
         self.assertEqual(factor3, 1000)
         um = UnitConst.METER
         ukg = UnitConst.KILOGRAM
         us = UnitConst.SECOND
         self.assertEqual((ukg + um - us * 2).symbol, "kg·m/s²")
```

### Comparing `siunitpy-0.0.2/tests/test_vector.py` & `siunitpy-0.1.1/tests/test_elementwiselist.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,78 +1,79 @@
-import unittest
 import sys
-from src.siunitpy.templatelib import Vector
+import unittest
+
+from src.siunitpy.utilcollections import ElementWiseList
 
 
 @unittest.skipIf(sys.version_info < (3, 9), 'only support 3.9+.')
-class TestVector(unittest.TestCase):
+class TestElementWiseList(unittest.TestCase):
     def test_init(self):
-        v0 = Vector()
+        v0 = ElementWiseList()
         self.assertEqual(repr(v0), '[]')
         self.assertEqual(len(v0), 0)
-        v1 = Vector([0, 1, 2, 3])
+        v1 = ElementWiseList([0, 1, 2, 3])
         self.assertEqual(repr(v1), '[0, 1, 2, 3]')
         self.assertEqual(str(v1), '[0, 1, 2, 3]')
         self.assertEqual(len(v1), 4)
-        v2 = Vector(range(4))
+        v2 = ElementWiseList(range(4))
         self.assertEqual(repr(v2), '[0, 1, 2, 3]')
         self.assertEqual(len(v2), 4)
-        v3 = Vector.packup(0, 1, 2, 3)
+        v3 = ElementWiseList.packup(0, 1, 2, 3)
         self.assertEqual(repr(v3), '[0, 1, 2, 3]')
         self.assertEqual(len(v3), 4)
 
     def test_getitem(self):
-        v0 = Vector(range(4))
+        v0 = ElementWiseList(range(4))
         self.assertEqual(v0[3], 3)
         self.assertEqual(v0[-1], 3)
         self.assertEqual(repr(v0[:2]), '[0, 1]')
         self.assertEqual(repr(v0[0, -1, 2]), '[0, 3, 2]')
         self.assertEqual(repr(v0[True, False, True]), '[0, 2]')
 
     def test_setitem(self):
-        v0 = Vector(range(4))
+        v0 = ElementWiseList(range(4))
         v0[:2] = range(1, 3)
         self.assertEqual(repr(v0), '[1, 2, 2, 3]')
         v0[v0 > 1] = 0
         self.assertEqual(repr(v0), '[1, 0, 0, 0]')
         v0[1:] = range(4)
         self.assertEqual(repr(v0), '[1, 0, 1, 2, 3]')
 
     def test_delitem(self):
-        v0 = Vector(range(10))
+        v0 = ElementWiseList(range(10))
         del v0[2:5]
         self.assertEqual(repr(v0), '[0, 1, 5, 6, 7, 8, 9]')
         del v0[v0 > 7]
         self.assertEqual(repr(v0), '[0, 1, 5, 6, 7]')
         if sys.version_info >= (3, 12):
             del v0[1, 4, 3]
             self.assertEqual(repr(v0), '[0, 5]')
 
 
     def test_operation(self):
-        v0 = Vector(range(4))
+        v0 = ElementWiseList(range(4))
         self.assertEqual(repr(-v0), '[0, -1, -2, -3]')
         self.assertEqual(repr(v0 * 3), '[0, 3, 6, 9]')
         v1 = v0 - 1
         self.assertEqual(repr(v1), '[-1, 0, 1, 2]')
         self.assertEqual(repr(abs(v1)), '[1, 0, 1, 2]')
         v2 = v0 * (v0 + 1)
         self.assertEqual(repr(v2), '[0, 2, 6, 12]')
         self.assertEqual(repr(v0 == v2 / 2), '[True, True, False, False]')
 
     def test_inplace_operation(self):
-        v0 = Vector(range(4))
+        v0 = ElementWiseList(range(4))
         v0 *= 2
         self.assertEqual(repr(v0), '[0, 2, 4, 6]')
         v0 <<= 3
         self.assertEqual(repr(v0), '[0, 16, 32, 48]')
     
     def test_replaced_operation(self):
-        v0 = Vector(range(3))
-        self.assertEqual(repr(Vector.cat(v0, v0 + 1)), '[0, 1, 2, 1, 2, 3]')
+        v0 = ElementWiseList(range(3))
+        self.assertEqual(repr(ElementWiseList.cat(v0, v0 + 1)), '[0, 1, 2, 1, 2, 3]')
         self.assertEqual(repr(v0.repeat(2)), '[0, 1, 2, 0, 1, 2]')
-        self.assertEqual(Vector.equal(v0, range(3)), True)
+        self.assertEqual(all(v0 == ElementWiseList([0, 1, 2, 3])), True)
         v0.extend(v0 - 1)
         self.assertEqual(repr(v0), '[0, 1, 2, -1, 0, 1]')
```

