# Comparing `tmp/javaobj-py3-0.4.3.tar.gz` & `tmp/javaobj-py3-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\javaobj-py3-0.4.3.tar", last modified: Fri May 14 14:26:42 2021, max compression
+gzip compressed data, was "javaobj-py3-0.4.4.tar", last modified: Sun Apr  7 19:17:40 2024, max compression
```

## Comparing `javaobj-py3-0.4.3.tar` & `javaobj-py3-0.4.4.tar`

### file list

```diff
@@ -1,35 +1,98 @@
-drwxrwxrwx   0        0        0        0 2021-05-14 14:26:42.382599 javaobj-py3-0.4.3/
--rw-rw-rw-   0        0        0      399 2021-05-14 12:06:30.000000 javaobj-py3-0.4.3/AUTHORS
--rw-rw-rw-   0        0        0    11358 2020-01-01 17:58:29.000000 javaobj-py3-0.4.3/LICENSE
--rw-rw-rw-   0        0        0      127 2021-05-14 12:06:30.000000 javaobj-py3-0.4.3/MANIFEST.in
--rw-rw-rw-   0        0        0    21421 2021-05-14 14:26:42.383596 javaobj-py3-0.4.3/PKG-INFO
--rw-rw-rw-   0        0        0    15995 2021-05-14 14:20:12.000000 javaobj-py3-0.4.3/README.md
-drwxrwxrwx   0        0        0        0 2021-05-14 14:26:42.174621 javaobj-py3-0.4.3/javaobj/
--rw-rw-rw-   0        0        0     1659 2021-05-14 14:16:59.000000 javaobj-py3-0.4.3/javaobj/__init__.py
--rw-rw-rw-   0        0        0     4249 2021-05-14 14:16:59.000000 javaobj-py3-0.4.3/javaobj/constants.py
--rw-rw-rw-   0        0        0     7803 2021-05-14 14:16:59.000000 javaobj-py3-0.4.3/javaobj/modifiedutf8.py
--rw-rw-rw-   0        0        0     8165 2021-05-14 14:16:59.000000 javaobj-py3-0.4.3/javaobj/utils.py
-drwxrwxrwx   0        0        0        0 2021-05-14 14:26:42.204599 javaobj-py3-0.4.3/javaobj/v1/
--rw-rw-rw-   0        0        0     1270 2021-05-14 14:16:59.000000 javaobj-py3-0.4.3/javaobj/v1/__init__.py
--rw-rw-rw-   0        0        0     5698 2021-05-14 14:16:59.000000 javaobj-py3-0.4.3/javaobj/v1/beans.py
--rw-rw-rw-   0        0        0     4143 2021-05-14 14:16:59.000000 javaobj-py3-0.4.3/javaobj/v1/core.py
--rw-rw-rw-   0        0        0    18888 2021-05-14 14:16:59.000000 javaobj-py3-0.4.3/javaobj/v1/marshaller.py
--rw-rw-rw-   0        0        0    13228 2021-05-14 14:16:59.000000 javaobj-py3-0.4.3/javaobj/v1/transformers.py
--rw-rw-rw-   0        0        0    28552 2021-05-14 14:16:59.000000 javaobj-py3-0.4.3/javaobj/v1/unmarshaller.py
-drwxrwxrwx   0        0        0        0 2021-05-14 14:26:42.282597 javaobj-py3-0.4.3/javaobj/v2/
--rw-rw-rw-   0        0        0     1548 2021-05-14 14:16:59.000000 javaobj-py3-0.4.3/javaobj/v2/__init__.py
--rw-rw-rw-   0        0        0     3358 2021-05-14 14:16:59.000000 javaobj-py3-0.4.3/javaobj/v2/api.py
--rw-rw-rw-   0        0        0    18059 2021-05-14 14:16:59.000000 javaobj-py3-0.4.3/javaobj/v2/beans.py
--rw-rw-rw-   0        0        0    25773 2021-05-14 14:16:59.000000 javaobj-py3-0.4.3/javaobj/v2/core.py
--rw-rw-rw-   0        0        0     2648 2021-05-14 14:16:01.000000 javaobj-py3-0.4.3/javaobj/v2/main.py
--rw-rw-rw-   0        0        0     4251 2021-05-14 14:16:59.000000 javaobj-py3-0.4.3/javaobj/v2/stream.py
--rw-rw-rw-   0        0        0    15172 2021-05-14 14:16:59.000000 javaobj-py3-0.4.3/javaobj/v2/transformers.py
-drwxrwxrwx   0        0        0        0 2021-05-14 14:26:42.380596 javaobj-py3-0.4.3/javaobj_py3.egg-info/
--rw-rw-rw-   0        0        0    21421 2021-05-14 14:26:41.000000 javaobj-py3-0.4.3/javaobj_py3.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      615 2021-05-14 14:26:41.000000 javaobj-py3-0.4.3/javaobj_py3.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-05-14 14:26:41.000000 javaobj-py3-0.4.3/javaobj_py3.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2021-05-14 14:26:41.000000 javaobj-py3-0.4.3/javaobj_py3.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2021-05-14 14:26:41.000000 javaobj-py3-0.4.3/javaobj_py3.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       30 2021-05-14 12:06:30.000000 javaobj-py3-0.4.3/pyproject.toml
--rw-rw-rw-   0        0        0       74 2021-05-14 14:26:42.393617 javaobj-py3-0.4.3/setup.cfg
--rw-rw-rw-   0        0        0     2899 2021-05-14 14:17:25.000000 javaobj-py3-0.4.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-07 19:17:40.848078 javaobj-py3-0.4.4/
+-rw-rw-rw-   0        0        0       54 2022-03-07 23:05:03.000000 javaobj-py3-0.4.4/.coveragerc
+-rw-rw-rw-   0        0        0      209 2018-06-15 21:52:39.000000 javaobj-py3-0.4.4/.editorconfig
+drwxrwxrwx   0        0        0        0 2024-04-07 19:17:40.696306 javaobj-py3-0.4.4/.github/
+drwxrwxrwx   0        0        0        0 2024-04-07 19:17:40.718331 javaobj-py3-0.4.4/.github/workflows/
+-rw-rw-rw-   0        0        0     1489 2022-03-07 23:05:03.000000 javaobj-py3-0.4.4/.github/workflows/build.yml
+-rw-rw-rw-   0        0        0      437 2020-04-05 10:01:12.000000 javaobj-py3-0.4.4/.gitignore
+-rw-rw-rw-   0        0        0      399 2021-02-02 19:45:11.000000 javaobj-py3-0.4.4/AUTHORS
+-rw-rw-rw-   0        0        0    11560 2016-04-21 21:02:11.000000 javaobj-py3-0.4.4/LICENSE
+-rw-rw-rw-   0        0        0    17678 2024-04-07 19:17:40.847079 javaobj-py3-0.4.4/PKG-INFO
+-rw-rw-rw-   0        0        0    15904 2022-03-07 23:05:03.000000 javaobj-py3-0.4.4/README.md
+drwxrwxrwx   0        0        0        0 2024-04-07 19:17:40.723699 javaobj-py3-0.4.4/javaobj/
+-rw-rw-rw-   0        0        0     1659 2024-04-07 19:17:25.000000 javaobj-py3-0.4.4/javaobj/__init__.py
+-rw-rw-rw-   0        0        0     4249 2024-04-07 19:17:25.000000 javaobj-py3-0.4.4/javaobj/constants.py
+-rw-rw-rw-   0        0        0     7803 2024-04-07 19:17:25.000000 javaobj-py3-0.4.4/javaobj/modifiedutf8.py
+-rw-rw-rw-   0        0        0     8165 2024-04-07 19:17:25.000000 javaobj-py3-0.4.4/javaobj/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-07 19:17:40.745725 javaobj-py3-0.4.4/javaobj/v1/
+-rw-rw-rw-   0        0        0     1270 2024-04-07 19:17:25.000000 javaobj-py3-0.4.4/javaobj/v1/__init__.py
+-rw-rw-rw-   0        0        0     5698 2024-04-07 19:17:25.000000 javaobj-py3-0.4.4/javaobj/v1/beans.py
+-rw-rw-rw-   0        0        0     4143 2024-04-07 19:17:25.000000 javaobj-py3-0.4.4/javaobj/v1/core.py
+-rw-rw-rw-   0        0        0    19097 2024-04-07 19:17:25.000000 javaobj-py3-0.4.4/javaobj/v1/marshaller.py
+-rw-rw-rw-   0        0        0    13228 2024-04-07 19:07:17.000000 javaobj-py3-0.4.4/javaobj/v1/transformers.py
+-rw-rw-rw-   0        0        0    28552 2024-04-07 19:17:25.000000 javaobj-py3-0.4.4/javaobj/v1/unmarshaller.py
+drwxrwxrwx   0        0        0        0 2024-04-07 19:17:40.756238 javaobj-py3-0.4.4/javaobj/v2/
+-rw-rw-rw-   0        0        0     1548 2024-04-07 19:17:25.000000 javaobj-py3-0.4.4/javaobj/v2/__init__.py
+-rw-rw-rw-   0        0        0     4058 2024-04-07 19:17:25.000000 javaobj-py3-0.4.4/javaobj/v2/api.py
+-rw-rw-rw-   0        0        0    18059 2024-04-07 19:17:25.000000 javaobj-py3-0.4.4/javaobj/v2/beans.py
+-rw-rw-rw-   0        0        0    25795 2024-04-07 19:17:25.000000 javaobj-py3-0.4.4/javaobj/v2/core.py
+-rw-rw-rw-   0        0        0     2648 2024-04-07 19:17:25.000000 javaobj-py3-0.4.4/javaobj/v2/main.py
+-rw-rw-rw-   0        0        0     4251 2024-04-07 19:17:25.000000 javaobj-py3-0.4.4/javaobj/v2/stream.py
+-rw-rw-rw-   0        0        0    15243 2024-04-07 19:17:25.000000 javaobj-py3-0.4.4/javaobj/v2/transformers.py
+drwxrwxrwx   0        0        0        0 2024-04-07 19:17:40.846079 javaobj-py3-0.4.4/javaobj_py3.egg-info/
+-rw-rw-rw-   0        0        0    17678 2024-04-07 19:17:40.000000 javaobj-py3-0.4.4/javaobj_py3.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1855 2024-04-07 19:17:40.000000 javaobj-py3-0.4.4/javaobj_py3.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-07 19:17:40.000000 javaobj-py3-0.4.4/javaobj_py3.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2024-04-07 19:17:40.000000 javaobj-py3-0.4.4/javaobj_py3.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-07 19:17:40.000000 javaobj-py3-0.4.4/javaobj_py3.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      127 2020-04-16 19:35:18.000000 javaobj-py3-0.4.4/manifest.in
+-rw-rw-rw-   0        0        0       30 2021-02-02 19:41:47.000000 javaobj-py3-0.4.4/pyproject.toml
+-rw-rw-rw-   0        0        0       58 2020-04-05 10:01:12.000000 javaobj-py3-0.4.4/requirements.txt
+-rw-rw-rw-   0        0        0       74 2024-04-07 19:17:40.849585 javaobj-py3-0.4.4/setup.cfg
+-rw-rw-rw-   0        0        0     3098 2024-04-07 19:17:28.000000 javaobj-py3-0.4.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-07 19:17:40.834958 javaobj-py3-0.4.4/tests/
+-rw-rw-rw-   0        0        0       90 2020-04-05 10:17:20.000000 javaobj-py3-0.4.4/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-07 19:17:40.839509 javaobj-py3-0.4.4/tests/java/
+-rw-rw-rw-   0        0        0      103 2019-03-15 20:53:07.000000 javaobj-py3-0.4.4/tests/java/.gitignore
+drwxrwxrwx   0        0        0        0 2024-04-07 19:17:40.840464 javaobj-py3-0.4.4/tests/java/.settings/
+-rw-rw-rw-   0        0        0       90 2016-04-21 21:01:44.000000 javaobj-py3-0.4.4/tests/java/.settings/org.eclipse.m2e.core.prefs
+-rw-rw-rw-   0        0        0      804 2021-02-02 19:34:54.000000 javaobj-py3-0.4.4/tests/java/pom.xml
+drwxrwxrwx   0        0        0        0 2024-04-07 19:17:40.699811 javaobj-py3-0.4.4/tests/java/src/
+drwxrwxrwx   0        0        0        0 2024-04-07 19:17:40.700818 javaobj-py3-0.4.4/tests/java/src/test/
+drwxrwxrwx   0        0        0        0 2024-04-07 19:17:40.845064 javaobj-py3-0.4.4/tests/java/src/test/java/
+-rw-rw-rw-   0        0        0     1423 2020-04-05 10:17:23.000000 javaobj-py3-0.4.4/tests/java/src/test/java/CollectionsTest.java
+-rw-rw-rw-   0        0        0     4411 2020-04-05 10:17:23.000000 javaobj-py3-0.4.4/tests/java/src/test/java/JFrameTest.java
+-rw-rw-rw-   0        0        0    11482 2022-03-07 23:05:03.000000 javaobj-py3-0.4.4/tests/java/src/test/java/OneTest.java
+-rw-rw-rw-   0        0        0       52 2021-10-03 21:25:14.000000 javaobj-py3-0.4.4/tests/java/testChars.ser.gz
+-rw-rw-rw-   0        0        0      447 2016-04-23 15:00:25.000000 javaobj-py3-0.4.4/tests/jceks_issue_5.ser
+-rw-rw-rw-   0        0        0        8 2016-04-21 21:01:44.000000 javaobj-py3-0.4.4/tests/obj0.ser
+-rw-rw-rw-   0        0        0       14 2016-04-21 21:01:44.000000 javaobj-py3-0.4.4/tests/obj1.ser
+-rw-rw-rw-   0        0        0       16 2016-04-21 21:01:44.000000 javaobj-py3-0.4.4/tests/obj2.ser
+-rw-rw-rw-   0        0        0        7 2016-04-21 21:01:44.000000 javaobj-py3-0.4.4/tests/obj3.ser
+-rw-rw-rw-   0        0        0        7 2016-04-21 21:01:44.000000 javaobj-py3-0.4.4/tests/obj4.ser
+-rw-rw-rw-   0        0        0      129 2016-04-21 21:01:44.000000 javaobj-py3-0.4.4/tests/obj5.ser
+-rw-rw-rw-   0        0        0       37 2016-04-21 21:01:44.000000 javaobj-py3-0.4.4/tests/obj6.ser
+-rw-rw-rw-   0        0        0    20040 2016-04-21 21:01:44.000000 javaobj-py3-0.4.4/tests/obj7.ser
+-rw-rw-rw-   0        0        0      449 2016-04-21 21:01:44.000000 javaobj-py3-0.4.4/tests/objArrays.ser
+-rw-rw-rw-   0        0        0      463 2016-04-23 12:50:57.000000 javaobj-py3-0.4.4/tests/objCollections.ser
+-rw-rw-rw-   0        0        0      190 2016-04-23 12:50:57.000000 javaobj-py3-0.4.4/tests/objEnums.ser
+-rw-rw-rw-   0        0        0     3191 2016-04-23 12:50:57.000000 javaobj-py3-0.4.4/tests/objException.ser
+-rw-rw-rw-   0        0        0      153 2016-04-23 12:50:57.000000 javaobj-py3-0.4.4/tests/objSuper.ser
+-rw-rw-rw-   0        0        0       69 2016-04-21 21:01:44.000000 javaobj-py3-0.4.4/tests/sunExample.ser
+-rw-rw-rw-   0        0        0       85 2022-03-07 23:05:03.000000 javaobj-py3-0.4.4/tests/test2DArray.ser
+-rw-rw-rw-   0        0        0      313 2020-04-05 10:16:14.000000 javaobj-py3-0.4.4/tests/testBoolIntLong-2.ser
+-rw-rw-rw-   0        0        0      279 2020-04-05 10:16:14.000000 javaobj-py3-0.4.4/tests/testBoolIntLong.ser
+-rw-rw-rw-   0        0        0        7 2016-04-23 12:50:57.000000 javaobj-py3-0.4.4/tests/testBoolean.ser
+-rw-rw-rw-   0        0        0        7 2016-04-23 12:50:57.000000 javaobj-py3-0.4.4/tests/testByte.ser
+-rw-rw-rw-   0        0        0       16 2016-04-23 12:50:57.000000 javaobj-py3-0.4.4/tests/testBytes.ser
+-rw-rw-rw-   0        0        0        8 2016-04-23 12:50:57.000000 javaobj-py3-0.4.4/tests/testChar.ser
+-rw-rw-rw-   0        0        0       41 2019-03-15 20:53:07.000000 javaobj-py3-0.4.4/tests/testCharArray.ser
+-rw-rw-rw-   0        0        0       34 2017-02-25 11:16:58.000000 javaobj-py3-0.4.4/tests/testChars.ser
+-rw-rw-rw-   0        0        0       52 2021-10-03 21:25:14.000000 javaobj-py3-0.4.4/tests/testChars.ser.gz
+-rw-rw-rw-   0        0        0       37 2016-04-23 12:50:57.000000 javaobj-py3-0.4.4/tests/testClass.ser
+-rw-rw-rw-   0        0        0      386 2022-03-07 23:05:03.000000 javaobj-py3-0.4.4/tests/testClassArray.ser
+-rw-rw-rw-   0        0        0       81 2017-02-25 11:16:58.000000 javaobj-py3-0.4.4/tests/testClassWithByteArray.ser
+-rw-rw-rw-   0        0        0      220 2020-04-16 16:52:09.000000 javaobj-py3-0.4.4/tests/testCustomWriteObject.ser
+-rw-rw-rw-   0        0        0       14 2016-04-23 12:50:57.000000 javaobj-py3-0.4.4/tests/testDouble.ser
+-rw-rw-rw-   0        0        0        4 2016-04-23 12:50:57.000000 javaobj-py3-0.4.4/tests/testEnums.ser
+-rw-rw-rw-   0        0        0        4 2016-04-23 12:50:57.000000 javaobj-py3-0.4.4/tests/testException.ser
+-rw-rw-rw-   0        0        0      150 2020-04-05 10:16:14.000000 javaobj-py3-0.4.4/tests/testHashSet.ser
+-rw-rw-rw-   0        0        0       16 2020-04-05 10:16:14.000000 javaobj-py3-0.4.4/tests/testJapan.ser
+-rw-rw-rw-   0        0        0      188 2020-04-05 10:16:14.000000 javaobj-py3-0.4.4/tests/testLinkedHashSet.ser
+-rw-rw-rw-   0        0        0        4 2016-04-23 12:50:57.000000 javaobj-py3-0.4.4/tests/testSuper.ser
+-rw-rw-rw-   0        0        0    20062 2016-04-23 12:50:57.000000 javaobj-py3-0.4.4/tests/testSwingObject.ser
+-rw-rw-rw-   0        0        0      231 2020-04-05 10:16:14.000000 javaobj-py3-0.4.4/tests/testTime.ser
+-rw-rw-rw-   0        0        0      143 2020-04-05 10:16:14.000000 javaobj-py3-0.4.4/tests/testTreeSet.ser
+-rw-rw-rw-   0        0        0      129 2016-04-23 12:50:57.000000 javaobj-py3-0.4.4/tests/test_readFields.ser
+-rw-rw-rw-   0        0        0    16578 2024-04-07 19:07:17.000000 javaobj-py3-0.4.4/tests/test_v1.py
+-rw-rw-rw-   0        0        0    21206 2024-04-07 19:07:17.000000 javaobj-py3-0.4.4/tests/test_v2.py
```

### Comparing `javaobj-py3-0.4.3/LICENSE` & `javaobj-py3-0.4.4/LICENSE`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,202 +1,202 @@
-
-                                 Apache License
-                           Version 2.0, January 2004
-                        http://www.apache.org/licenses/
-
-   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
-
-   1. Definitions.
-
-      "License" shall mean the terms and conditions for use, reproduction,
-      and distribution as defined by Sections 1 through 9 of this document.
-
-      "Licensor" shall mean the copyright owner or entity authorized by
-      the copyright owner that is granting the License.
-
-      "Legal Entity" shall mean the union of the acting entity and all
-      other entities that control, are controlled by, or are under common
-      control with that entity. For the purposes of this definition,
-      "control" means (i) the power, direct or indirect, to cause the
-      direction or management of such entity, whether by contract or
-      otherwise, or (ii) ownership of fifty percent (50%) or more of the
-      outstanding shares, or (iii) beneficial ownership of such entity.
-
-      "You" (or "Your") shall mean an individual or Legal Entity
-      exercising permissions granted by this License.
-
-      "Source" form shall mean the preferred form for making modifications,
-      including but not limited to software source code, documentation
-      source, and configuration files.
-
-      "Object" form shall mean any form resulting from mechanical
-      transformation or translation of a Source form, including but
-      not limited to compiled object code, generated documentation,
-      and conversions to other media types.
-
-      "Work" shall mean the work of authorship, whether in Source or
-      Object form, made available under the License, as indicated by a
-      copyright notice that is included in or attached to the work
-      (an example is provided in the Appendix below).
-
-      "Derivative Works" shall mean any work, whether in Source or Object
-      form, that is based on (or derived from) the Work and for which the
-      editorial revisions, annotations, elaborations, or other modifications
-      represent, as a whole, an original work of authorship. For the purposes
-      of this License, Derivative Works shall not include works that remain
-      separable from, or merely link (or bind by name) to the interfaces of,
-      the Work and Derivative Works thereof.
-
-      "Contribution" shall mean any work of authorship, including
-      the original version of the Work and any modifications or additions
-      to that Work or Derivative Works thereof, that is intentionally
-      submitted to Licensor for inclusion in the Work by the copyright owner
-      or by an individual or Legal Entity authorized to submit on behalf of
-      the copyright owner. For the purposes of this definition, "submitted"
-      means any form of electronic, verbal, or written communication sent
-      to the Licensor or its representatives, including but not limited to
-      communication on electronic mailing lists, source code control systems,
-      and issue tracking systems that are managed by, or on behalf of, the
-      Licensor for the purpose of discussing and improving the Work, but
-      excluding communication that is conspicuously marked or otherwise
-      designated in writing by the copyright owner as "Not a Contribution."
-
-      "Contributor" shall mean Licensor and any individual or Legal Entity
-      on behalf of whom a Contribution has been received by Licensor and
-      subsequently incorporated within the Work.
-
-   2. Grant of Copyright License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      copyright license to reproduce, prepare Derivative Works of,
-      publicly display, publicly perform, sublicense, and distribute the
-      Work and such Derivative Works in Source or Object form.
-
-   3. Grant of Patent License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      (except as stated in this section) patent license to make, have made,
-      use, offer to sell, sell, import, and otherwise transfer the Work,
-      where such license applies only to those patent claims licensable
-      by such Contributor that are necessarily infringed by their
-      Contribution(s) alone or by combination of their Contribution(s)
-      with the Work to which such Contribution(s) was submitted. If You
-      institute patent litigation against any entity (including a
-      cross-claim or counterclaim in a lawsuit) alleging that the Work
-      or a Contribution incorporated within the Work constitutes direct
-      or contributory patent infringement, then any patent licenses
-      granted to You under this License for that Work shall terminate
-      as of the date such litigation is filed.
-
-   4. Redistribution. You may reproduce and distribute copies of the
-      Work or Derivative Works thereof in any medium, with or without
-      modifications, and in Source or Object form, provided that You
-      meet the following conditions:
-
-      (a) You must give any other recipients of the Work or
-          Derivative Works a copy of this License; and
-
-      (b) You must cause any modified files to carry prominent notices
-          stating that You changed the files; and
-
-      (c) You must retain, in the Source form of any Derivative Works
-          that You distribute, all copyright, patent, trademark, and
-          attribution notices from the Source form of the Work,
-          excluding those notices that do not pertain to any part of
-          the Derivative Works; and
-
-      (d) If the Work includes a "NOTICE" text file as part of its
-          distribution, then any Derivative Works that You distribute must
-          include a readable copy of the attribution notices contained
-          within such NOTICE file, excluding those notices that do not
-          pertain to any part of the Derivative Works, in at least one
-          of the following places: within a NOTICE text file distributed
-          as part of the Derivative Works; within the Source form or
-          documentation, if provided along with the Derivative Works; or,
-          within a display generated by the Derivative Works, if and
-          wherever such third-party notices normally appear. The contents
-          of the NOTICE file are for informational purposes only and
-          do not modify the License. You may add Your own attribution
-          notices within Derivative Works that You distribute, alongside
-          or as an addendum to the NOTICE text from the Work, provided
-          that such additional attribution notices cannot be construed
-          as modifying the License.
-
-      You may add Your own copyright statement to Your modifications and
-      may provide additional or different license terms and conditions
-      for use, reproduction, or distribution of Your modifications, or
-      for any such Derivative Works as a whole, provided Your use,
-      reproduction, and distribution of the Work otherwise complies with
-      the conditions stated in this License.
-
-   5. Submission of Contributions. Unless You explicitly state otherwise,
-      any Contribution intentionally submitted for inclusion in the Work
-      by You to the Licensor shall be under the terms and conditions of
-      this License, without any additional terms or conditions.
-      Notwithstanding the above, nothing herein shall supersede or modify
-      the terms of any separate license agreement you may have executed
-      with Licensor regarding such Contributions.
-
-   6. Trademarks. This License does not grant permission to use the trade
-      names, trademarks, service marks, or product names of the Licensor,
-      except as required for reasonable and customary use in describing the
-      origin of the Work and reproducing the content of the NOTICE file.
-
-   7. Disclaimer of Warranty. Unless required by applicable law or
-      agreed to in writing, Licensor provides the Work (and each
-      Contributor provides its Contributions) on an "AS IS" BASIS,
-      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
-      implied, including, without limitation, any warranties or conditions
-      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
-      PARTICULAR PURPOSE. You are solely responsible for determining the
-      appropriateness of using or redistributing the Work and assume any
-      risks associated with Your exercise of permissions under this License.
-
-   8. Limitation of Liability. In no event and under no legal theory,
-      whether in tort (including negligence), contract, or otherwise,
-      unless required by applicable law (such as deliberate and grossly
-      negligent acts) or agreed to in writing, shall any Contributor be
-      liable to You for damages, including any direct, indirect, special,
-      incidental, or consequential damages of any character arising as a
-      result of this License or out of the use or inability to use the
-      Work (including but not limited to damages for loss of goodwill,
-      work stoppage, computer failure or malfunction, or any and all
-      other commercial damages or losses), even if such Contributor
-      has been advised of the possibility of such damages.
-
-   9. Accepting Warranty or Additional Liability. While redistributing
-      the Work or Derivative Works thereof, You may choose to offer,
-      and charge a fee for, acceptance of support, warranty, indemnity,
-      or other liability obligations and/or rights consistent with this
-      License. However, in accepting such obligations, You may act only
-      on Your own behalf and on Your sole responsibility, not on behalf
-      of any other Contributor, and only if You agree to indemnify,
-      defend, and hold each Contributor harmless for any liability
-      incurred by, or claims asserted against, such Contributor by reason
-      of your accepting any such warranty or additional liability.
-
-   END OF TERMS AND CONDITIONS
-
-   APPENDIX: How to apply the Apache License to your work.
-
-      To apply the Apache License to your work, attach the following
-      boilerplate notice, with the fields enclosed by brackets "[]"
-      replaced with your own identifying information. (Don't include
-      the brackets!)  The text should be enclosed in the appropriate
-      comment syntax for the file format. We also recommend that a
-      file or class name and description of purpose be included on the
-      same "printed page" as the copyright notice for easier
-      identification within third-party archives.
-
-   Copyright [yyyy] [name of copyright owner]
-
-   Licensed under the Apache License, Version 2.0 (the "License");
-   you may not use this file except in compliance with the License.
-   You may obtain a copy of the License at
-
-       http://www.apache.org/licenses/LICENSE-2.0
-
-   Unless required by applicable law or agreed to in writing, software
-   distributed under the License is distributed on an "AS IS" BASIS,
-   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-   See the License for the specific language governing permissions and
-   limitations under the License.
+
+                                 Apache License
+                           Version 2.0, January 2004
+                        http://www.apache.org/licenses/
+
+   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
+
+   1. Definitions.
+
+      "License" shall mean the terms and conditions for use, reproduction,
+      and distribution as defined by Sections 1 through 9 of this document.
+
+      "Licensor" shall mean the copyright owner or entity authorized by
+      the copyright owner that is granting the License.
+
+      "Legal Entity" shall mean the union of the acting entity and all
+      other entities that control, are controlled by, or are under common
+      control with that entity. For the purposes of this definition,
+      "control" means (i) the power, direct or indirect, to cause the
+      direction or management of such entity, whether by contract or
+      otherwise, or (ii) ownership of fifty percent (50%) or more of the
+      outstanding shares, or (iii) beneficial ownership of such entity.
+
+      "You" (or "Your") shall mean an individual or Legal Entity
+      exercising permissions granted by this License.
+
+      "Source" form shall mean the preferred form for making modifications,
+      including but not limited to software source code, documentation
+      source, and configuration files.
+
+      "Object" form shall mean any form resulting from mechanical
+      transformation or translation of a Source form, including but
+      not limited to compiled object code, generated documentation,
+      and conversions to other media types.
+
+      "Work" shall mean the work of authorship, whether in Source or
+      Object form, made available under the License, as indicated by a
+      copyright notice that is included in or attached to the work
+      (an example is provided in the Appendix below).
+
+      "Derivative Works" shall mean any work, whether in Source or Object
+      form, that is based on (or derived from) the Work and for which the
+      editorial revisions, annotations, elaborations, or other modifications
+      represent, as a whole, an original work of authorship. For the purposes
+      of this License, Derivative Works shall not include works that remain
+      separable from, or merely link (or bind by name) to the interfaces of,
+      the Work and Derivative Works thereof.
+
+      "Contribution" shall mean any work of authorship, including
+      the original version of the Work and any modifications or additions
+      to that Work or Derivative Works thereof, that is intentionally
+      submitted to Licensor for inclusion in the Work by the copyright owner
+      or by an individual or Legal Entity authorized to submit on behalf of
+      the copyright owner. For the purposes of this definition, "submitted"
+      means any form of electronic, verbal, or written communication sent
+      to the Licensor or its representatives, including but not limited to
+      communication on electronic mailing lists, source code control systems,
+      and issue tracking systems that are managed by, or on behalf of, the
+      Licensor for the purpose of discussing and improving the Work, but
+      excluding communication that is conspicuously marked or otherwise
+      designated in writing by the copyright owner as "Not a Contribution."
+
+      "Contributor" shall mean Licensor and any individual or Legal Entity
+      on behalf of whom a Contribution has been received by Licensor and
+      subsequently incorporated within the Work.
+
+   2. Grant of Copyright License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      copyright license to reproduce, prepare Derivative Works of,
+      publicly display, publicly perform, sublicense, and distribute the
+      Work and such Derivative Works in Source or Object form.
+
+   3. Grant of Patent License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      (except as stated in this section) patent license to make, have made,
+      use, offer to sell, sell, import, and otherwise transfer the Work,
+      where such license applies only to those patent claims licensable
+      by such Contributor that are necessarily infringed by their
+      Contribution(s) alone or by combination of their Contribution(s)
+      with the Work to which such Contribution(s) was submitted. If You
+      institute patent litigation against any entity (including a
+      cross-claim or counterclaim in a lawsuit) alleging that the Work
+      or a Contribution incorporated within the Work constitutes direct
+      or contributory patent infringement, then any patent licenses
+      granted to You under this License for that Work shall terminate
+      as of the date such litigation is filed.
+
+   4. Redistribution. You may reproduce and distribute copies of the
+      Work or Derivative Works thereof in any medium, with or without
+      modifications, and in Source or Object form, provided that You
+      meet the following conditions:
+
+      (a) You must give any other recipients of the Work or
+          Derivative Works a copy of this License; and
+
+      (b) You must cause any modified files to carry prominent notices
+          stating that You changed the files; and
+
+      (c) You must retain, in the Source form of any Derivative Works
+          that You distribute, all copyright, patent, trademark, and
+          attribution notices from the Source form of the Work,
+          excluding those notices that do not pertain to any part of
+          the Derivative Works; and
+
+      (d) If the Work includes a "NOTICE" text file as part of its
+          distribution, then any Derivative Works that You distribute must
+          include a readable copy of the attribution notices contained
+          within such NOTICE file, excluding those notices that do not
+          pertain to any part of the Derivative Works, in at least one
+          of the following places: within a NOTICE text file distributed
+          as part of the Derivative Works; within the Source form or
+          documentation, if provided along with the Derivative Works; or,
+          within a display generated by the Derivative Works, if and
+          wherever such third-party notices normally appear. The contents
+          of the NOTICE file are for informational purposes only and
+          do not modify the License. You may add Your own attribution
+          notices within Derivative Works that You distribute, alongside
+          or as an addendum to the NOTICE text from the Work, provided
+          that such additional attribution notices cannot be construed
+          as modifying the License.
+
+      You may add Your own copyright statement to Your modifications and
+      may provide additional or different license terms and conditions
+      for use, reproduction, or distribution of Your modifications, or
+      for any such Derivative Works as a whole, provided Your use,
+      reproduction, and distribution of the Work otherwise complies with
+      the conditions stated in this License.
+
+   5. Submission of Contributions. Unless You explicitly state otherwise,
+      any Contribution intentionally submitted for inclusion in the Work
+      by You to the Licensor shall be under the terms and conditions of
+      this License, without any additional terms or conditions.
+      Notwithstanding the above, nothing herein shall supersede or modify
+      the terms of any separate license agreement you may have executed
+      with Licensor regarding such Contributions.
+
+   6. Trademarks. This License does not grant permission to use the trade
+      names, trademarks, service marks, or product names of the Licensor,
+      except as required for reasonable and customary use in describing the
+      origin of the Work and reproducing the content of the NOTICE file.
+
+   7. Disclaimer of Warranty. Unless required by applicable law or
+      agreed to in writing, Licensor provides the Work (and each
+      Contributor provides its Contributions) on an "AS IS" BASIS,
+      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
+      implied, including, without limitation, any warranties or conditions
+      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
+      PARTICULAR PURPOSE. You are solely responsible for determining the
+      appropriateness of using or redistributing the Work and assume any
+      risks associated with Your exercise of permissions under this License.
+
+   8. Limitation of Liability. In no event and under no legal theory,
+      whether in tort (including negligence), contract, or otherwise,
+      unless required by applicable law (such as deliberate and grossly
+      negligent acts) or agreed to in writing, shall any Contributor be
+      liable to You for damages, including any direct, indirect, special,
+      incidental, or consequential damages of any character arising as a
+      result of this License or out of the use or inability to use the
+      Work (including but not limited to damages for loss of goodwill,
+      work stoppage, computer failure or malfunction, or any and all
+      other commercial damages or losses), even if such Contributor
+      has been advised of the possibility of such damages.
+
+   9. Accepting Warranty or Additional Liability. While redistributing
+      the Work or Derivative Works thereof, You may choose to offer,
+      and charge a fee for, acceptance of support, warranty, indemnity,
+      or other liability obligations and/or rights consistent with this
+      License. However, in accepting such obligations, You may act only
+      on Your own behalf and on Your sole responsibility, not on behalf
+      of any other Contributor, and only if You agree to indemnify,
+      defend, and hold each Contributor harmless for any liability
+      incurred by, or claims asserted against, such Contributor by reason
+      of your accepting any such warranty or additional liability.
+
+   END OF TERMS AND CONDITIONS
+
+   APPENDIX: How to apply the Apache License to your work.
+
+      To apply the Apache License to your work, attach the following
+      boilerplate notice, with the fields enclosed by brackets "[]"
+      replaced with your own identifying information. (Don't include
+      the brackets!)  The text should be enclosed in the appropriate
+      comment syntax for the file format. We also recommend that a
+      file or class name and description of purpose be included on the
+      same "printed page" as the copyright notice for easier
+      identification within third-party archives.
+
+   Copyright [yyyy] [name of copyright owner]
+
+   Licensed under the Apache License, Version 2.0 (the "License");
+   you may not use this file except in compliance with the License.
+   You may obtain a copy of the License at
+
+       http://www.apache.org/licenses/LICENSE-2.0
+
+   Unless required by applicable law or agreed to in writing, software
+   distributed under the License is distributed on an "AS IS" BASIS,
+   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+   See the License for the specific language governing permissions and
+   limitations under the License.
```

### Comparing `javaobj-py3-0.4.3/README.md` & `javaobj-py3-0.4.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,13 @@
 # javaobj-py3
 
-<p>
-    <a href="https://pypi.python.org/pypi/javaobj-py3/">
-        <img src="https://img.shields.io/pypi/v/javaobj-py3.svg" alt="Latest Version" />
-        <img src="https://img.shields.io/pypi/l/javaobj-py3.svg" alt="License" />
-    </a>
-    <a href="https://travis-ci.org/tcalmant/python-javaobj">
-    <img src="https://travis-ci.org/tcalmant/python-javaobj.svg?branch=master"
-        alt="Travis-CI status" />
-    </a>
-    <a href="https://coveralls.io/r/tcalmant/python-javaobj?branch=master">
-        <img src="https://coveralls.io/repos/tcalmant/python-javaobj/badge.svg?branch=master"
-            alt="Coveralls status" />
-    </a>
-</p>
+[![Latest Version](https://img.shields.io/pypi/v/javaobj-py3.svg)](https://pypi.python.org/pypi/javaobj-py3/)
+[![License](https://img.shields.io/pypi/l/javaobj-py3.svg)](https://pypi.python.org/pypi/javaobj-py3/)
+[![CI Build](https://github.com/tcalmant/python-javaobj/actions/workflows/build.yml/badge.svg?branch=master)](https://github.com/tcalmant/python-javaobj/actions/workflows/build.yml)
+[![Coveralls status](https://coveralls.io/repos/tcalmant/python-javaobj/badge.svg?branch=master)](https://coveralls.io/r/tcalmant/python-javaobj?branch=master)
 
 *python-javaobj* is a python library that provides functions for reading and
 writing (writing is WIP currently) Java objects serialized or will be
 deserialized by `ObjectOutputStream`. This form of object representation is a
 standard data interchange format in Java world.
 
 The `javaobj` module exposes an API familiar to users of the standard library
```

### Comparing `javaobj-py3-0.4.3/javaobj/__init__.py` & `javaobj-py3-0.4.4/javaobj/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,20 +9,20 @@
 marshal, pickle and json modules.
 
 See:
 http://download.oracle.com/javase/6/docs/platform/serialization/spec/protocol.html
 
 :authors: Volodymyr Buell, Thomas Calmant
 :license: Apache License 2.0
-:version: 0.4.3
+:version: 0.4.4
 :status: Alpha
 
 ..
 
-    Copyright 2021 Thomas Calmant
+    Copyright 2024 Thomas Calmant
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
 
@@ -37,12 +37,12 @@
 from javaobj.v1.beans import *  # noqa: F401,F403
 from javaobj.v1.core import *  # noqa: F401,F403
 from javaobj.v1.transformers import *  # noqa: F401,F403
 
 # ------------------------------------------------------------------------------
 
 # Module version
-__version_info__ = (0, 4, 3)
+__version_info__ = (0, 4, 4)
 __version__ = ".".join(str(x) for x in __version_info__)
 
 # Documentation strings format
 __docformat__ = "restructuredtext en"
```

### Comparing `javaobj-py3-0.4.3/javaobj/constants.py` & `javaobj-py3-0.4.4/javaobj/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 #!/usr/bin/env python3
 """
 Definition of the constants used in the deserialization process
 
 :authors: Thomas Calmant
 :license: Apache License 2.0
-:version: 0.4.3
+:version: 0.4.4
 :status: Alpha
 
 ..
 
-    Copyright 2021 Thomas Calmant
+    Copyright 2024 Thomas Calmant
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
 
@@ -34,15 +34,15 @@
     "TerminalCode",
     "ClassDescFlags",
     "TypeCode",
     "StreamCodeDebug",
 )
 
 # Module version
-__version_info__ = (0, 4, 3)
+__version_info__ = (0, 4, 4)
 __version__ = ".".join(str(x) for x in __version_info__)
 
 # Documentation strings format
 __docformat__ = "restructuredtext en"
 
 # ------------------------------------------------------------------------------
```

### Comparing `javaobj-py3-0.4.3/javaobj/modifiedutf8.py` & `javaobj-py3-0.4.4/javaobj/modifiedutf8.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,25 +7,25 @@
 `@guywithface <https://github.com/guywithface>`_.
 
 The project the original file comes from is available at:
 https://github.com/swstephe/py2jdbc/
 
 :authors: Scott Stephens (@swstephe), @guywithface
 :license: Apache License 2.0
-:version: 0.4.3
+:version: 0.4.4
 :status: Alpha
 """
 
 from __future__ import unicode_literals
 
 import sys
 
 
 # Module version
-__version_info__ = (0, 4, 3)
+__version_info__ = (0, 4, 4)
 __version__ = ".".join(str(x) for x in __version_info__)
 
 # Documentation strings format
 __docformat__ = "restructuredtext en"
 
 # Encoding name: not cesu-8, which uses a different zero-byte
 NAME = "mutf8"
```

### Comparing `javaobj-py3-0.4.3/javaobj/utils.py` & `javaobj-py3-0.4.4/javaobj/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,20 +3,20 @@
 """
 Provides utility methods used by the core implementation of javaobj.
 
 Namely: logging methods, bytes/str/unicode converters
 
 :authors: Thomas Calmant
 :license: Apache License 2.0
-:version: 0.4.3
+:version: 0.4.4
 :status: Alpha
 
 ..
 
-    Copyright 2021 Thomas Calmant
+    Copyright 2024 Thomas Calmant
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
 
@@ -39,15 +39,15 @@
 
 # Modified UTF-8 parser
 from .modifiedutf8 import byte_to_int, decode_modified_utf8
 
 # ------------------------------------------------------------------------------
 
 # Module version
-__version_info__ = (0, 4, 3)
+__version_info__ = (0, 4, 4)
 __version__ = ".".join(str(x) for x in __version_info__)
 
 # Documentation strings format
 __docformat__ = "restructuredtext en"
 
 # ------------------------------------------------------------------------------
```

### Comparing `javaobj-py3-0.4.3/javaobj/v1/__init__.py` & `javaobj-py3-0.4.4/javaobj/v1/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 #!/usr/bin/env python
 """
 First version of the un-marshalling process of javaobj.
 
 :authors: Thomas Calmant
 :license: Apache License 2.0
-:version: 0.4.3
+:version: 0.4.4
 :status: Alpha
 
 ..
 
-    Copyright 2021 Thomas Calmant
+    Copyright 2024 Thomas Calmant
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
 
@@ -33,12 +33,12 @@
     JavaObjectUnmarshaller,
 )
 from .transformers import DefaultObjectTransformer  # noqa: F401
 
 # ------------------------------------------------------------------------------
 
 # Module version
-__version_info__ = (0, 4, 3)
+__version_info__ = (0, 4, 4)
 __version__ = ".".join(str(x) for x in __version_info__)
 
 # Documentation strings format
 __docformat__ = "restructuredtext en"
```

### Comparing `javaobj-py3-0.4.3/javaobj/v1/beans.py` & `javaobj-py3-0.4.4/javaobj/v1/beans.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 #!/usr/bin/python
 # -- Content-Encoding: utf-8 --
 """
 Definition of the beans of the v1 parser
 
 :authors: Volodymyr Buell, Thomas Calmant
 :license: Apache License 2.0
-:version: 0.4.3
+:version: 0.4.4
 :status: Alpha
 
 ..
 
-    Copyright 2021 Thomas Calmant
+    Copyright 2024 Thomas Calmant
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
 
@@ -40,15 +40,15 @@
     "JavaClass",
     "JavaEnum",
     "JavaObject",
     "JavaString",
 )
 
 # Module version
-__version_info__ = (0, 4, 3)
+__version_info__ = (0, 4, 4)
 __version__ = ".".join(str(x) for x in __version_info__)
 
 # Documentation strings format
 __docformat__ = "restructuredtext en"
 
 # ------------------------------------------------------------------------------
```

### Comparing `javaobj-py3-0.4.3/javaobj/v1/core.py` & `javaobj-py3-0.4.4/javaobj/v1/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,20 +9,20 @@
 marshal, pickle and json modules.
 
 See:
 http://download.oracle.com/javase/6/docs/platform/serialization/spec/protocol.html
 
 :authors: Volodymyr Buell, Thomas Calmant
 :license: Apache License 2.0
-:version: 0.4.3
+:version: 0.4.4
 :status: Alpha
 
 ..
 
-    Copyright 2021 Thomas Calmant
+    Copyright 2024 Thomas Calmant
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
 
@@ -58,15 +58,15 @@
     "JavaObjectUnmarshaller",
     "dumps",
     "load",
     "loads",
 )
 
 # Module version
-__version_info__ = (0, 4, 3)
+__version_info__ = (0, 4, 4)
 __version__ = ".".join(str(x) for x in __version_info__)
 
 # Documentation strings format
 __docformat__ = "restructuredtext en"
 
 # ------------------------------------------------------------------------------
```

### Comparing `javaobj-py3-0.4.3/javaobj/v1/marshaller.py` & `javaobj-py3-0.4.4/javaobj/v1/marshaller.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,20 +9,20 @@
 marshal, pickle and json modules.
 
 See:
 http://download.oracle.com/javase/6/docs/platform/serialization/spec/protocol.html
 
 :authors: Volodymyr Buell, Thomas Calmant
 :license: Apache License 2.0
-:version: 0.4.3
+:version: 0.4.4
 :status: Alpha
 
 ..
 
-    Copyright 2021 Thomas Calmant
+    Copyright 2024 Thomas Calmant
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
 
@@ -72,15 +72,15 @@
 
 # ------------------------------------------------------------------------------
 
 __all__ = ("JavaObjectMarshaller",)
 
 
 # Module version
-__version_info__ = (0, 4, 3)
+__version_info__ = (0, 4, 4)
 __version__ = ".".join(str(x) for x in __version_info__)
 
 # Documentation strings format
 __docformat__ = "restructuredtext en"
 
 # ------------------------------------------------------------------------------
 
@@ -137,14 +137,17 @@
         :param obj: A string or a deserialized Java object
         :raise RuntimeError: Unsupported type
         """
         log_debug("Writing object of type {0}".format(type(obj).__name__))
         if isinstance(obj, JavaArray):
             # Deserialized Java array
             self.write_array(obj)
+        elif isinstance(obj, JavaByteArray):
+            # Deserialized Java byte array
+            self.write_array(obj)
         elif isinstance(obj, JavaEnum):
             # Deserialized Java Enum
             self.write_enum(obj)
         elif isinstance(obj, JavaObject):
             # Deserialized Java object
             self.write_object(obj)
         elif isinstance(obj, JavaString):
@@ -533,14 +536,16 @@
                 self.write_enum(value)
             elif isinstance(value, (JavaArray, JavaByteArray)):
                 self.write_array(value)
             elif isinstance(value, JavaObject):
                 self.write_object(value)
             elif isinstance(value, JavaString):
                 self.write_string(value)
+            elif isinstance(value, JavaClass):
+                self.write_class(value)
             elif isinstance(value, (BYTES_TYPE, UNICODE_TYPE)):
                 self.write_blockdata(value)
             else:
                 raise RuntimeError("Unknown typecode: {0}".format(field_type))
         else:
             raise RuntimeError("Unknown typecode: {0}".format(field_type))
```

### Comparing `javaobj-py3-0.4.3/javaobj/v1/transformers.py` & `javaobj-py3-0.4.4/javaobj/v1/transformers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 #!/usr/bin/python
 # -- Content-Encoding: utf-8 --
 """
 Implementation of the object transformers in v1 parser
 
 :authors: Volodymyr Buell, Thomas Calmant
 :license: Apache License 2.0
-:version: 0.4.3
+:version: 0.4.4
 :status: Alpha
 
 ..
 
-    Copyright 2021 Thomas Calmant
+    Copyright 2024 Thomas Calmant
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `javaobj-py3-0.4.3/javaobj/v1/unmarshaller.py` & `javaobj-py3-0.4.4/javaobj/v1/unmarshaller.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,20 +9,20 @@
 marshal, pickle and json modules.
 
 See:
 http://download.oracle.com/javase/6/docs/platform/serialization/spec/protocol.html
 
 :authors: Volodymyr Buell, Thomas Calmant
 :license: Apache License 2.0
-:version: 0.4.3
+:version: 0.4.4
 :status: Alpha
 
 ..
 
-    Copyright 2021 Thomas Calmant
+    Copyright 2024 Thomas Calmant
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
 
@@ -68,15 +68,15 @@
 numpy = None  # Imported only when really used
 
 # ------------------------------------------------------------------------------
 
 __all__ = ("JavaObjectUnmarshaller",)
 
 # Module version
-__version_info__ = (0, 4, 3)
+__version_info__ = (0, 4, 4)
 __version__ = ".".join(str(x) for x in __version_info__)
 
 # Documentation strings format
 __docformat__ = "restructuredtext en"
 
 # ------------------------------------------------------------------------------
```

### Comparing `javaobj-py3-0.4.3/javaobj/v2/__init__.py` & `javaobj-py3-0.4.4/javaobj/v2/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,20 +11,20 @@
 approach.
 
 This package should handle more files than before, in read-only mode.
 The writing mode should be handled by the "classic" javaobj code.
 
 :authors: Thomas Calmant
 :license: Apache License 2.0
-:version: 0.4.3
+:version: 0.4.4
 :status: Alpha
 
 ..
 
-    Copyright 2021 Thomas Calmant
+    Copyright 2024 Thomas Calmant
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
 
@@ -37,12 +37,12 @@
 
 from . import api, beans, core, main, stream, transformers  # noqa: 401
 from .main import load, loads  # noqa: 401
 
 # ------------------------------------------------------------------------------
 
 # Module version
-__version_info__ = (0, 4, 3)
+__version_info__ = (0, 4, 4)
 __version__ = ".".join(str(x) for x in __version_info__)
 
 # Documentation strings format
 __docformat__ = "restructuredtext en"
```

### Comparing `javaobj-py3-0.4.3/javaobj/v2/api.py` & `javaobj-py3-0.4.4/javaobj/v2/api.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 #!/usr/bin/env python3
 """
 Definition of the object transformer API
 
 :authors: Thomas Calmant
 :license: Apache License 2.0
-:version: 0.4.3
+:version: 0.4.4
 :status: Alpha
 
 ..
 
-    Copyright 2021 Thomas Calmant
+    Copyright 2024 Thomas Calmant
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
 
@@ -22,32 +22,62 @@
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 """
 
 from __future__ import absolute_import
 
-from typing import Optional
+from typing import List, Optional
 
-from .beans import JavaClassDesc, JavaInstance  # pylint:disable=W0611
-from .stream import DataStreamReader  # pylint:disable=W0611
 from ..constants import TypeCode  # pylint:disable=W0611
+from .beans import (  # pylint:disable=W0611
+    JavaClassDesc,
+    JavaInstance,
+    ParsedJavaContent,
+)
+from .stream import DataStreamReader  # pylint:disable=W0611
 
 # ------------------------------------------------------------------------------
 
 # Module version
-__version_info__ = (0, 4, 3)
+__version_info__ = (0, 4, 4)
 __version__ = ".".join(str(x) for x in __version_info__)
 
 # Documentation strings format
 __docformat__ = "restructuredtext en"
 
 # ------------------------------------------------------------------------------
 
 
+class IJavaStreamParser:
+    """
+    API of the Java stream parser
+    """
+
+    def run(self):
+        # type: () -> List[ParsedJavaContent]
+        """
+        Parses the input stream
+        """
+        raise NotImplementedError
+
+    def dump(self, content):
+        # type: (List[ParsedJavaContent]) -> str
+        """
+        Dumps to a string the given objects
+        """
+        raise NotImplementedError
+
+    def _read_content(self, type_code, block_data, class_desc=None):
+        # type: (int, bool, Optional[JavaClassDesc]) -> ParsedJavaContent
+        """
+        Parses the next content. Use with care (use only in a transformer)
+        """
+
+
 class ObjectTransformer(object):  # pylint:disable=R0205
     """
     Representation of an object transformer
     """
 
     def create_instance(self, classdesc):  # pylint:disable=W0613,R0201
         # type: (JavaClassDesc) -> Optional[JavaInstance]
@@ -80,15 +110,15 @@
         :param size: Number of elements in the array
         """
         return None
 
     def load_custom_writeObject(
         self, parser, reader, name
     ):  # pylint:disable=W0613,R0201
-        # type: (JavaStreamParser, DataStreamReader, str) -> Optional[JavaClassDesc]
+        # type: (IJavaStreamParser, DataStreamReader, str) -> Optional[JavaClassDesc]
         """
         Reads content stored from a custom writeObject.
 
         This method is called only if the class description has both the
         ``SC_SERIALIZABLE`` and ``SC_WRITE_METHOD`` flags set.
 
         The stream parsing will stop and fail if this method returns None.
```

### Comparing `javaobj-py3-0.4.3/javaobj/v2/beans.py` & `javaobj-py3-0.4.4/javaobj/v2/beans.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 #!/usr/bin/env python3
 """
 Definition of the beans used to represent the parsed objects
 
 :authors: Thomas Calmant
 :license: Apache License 2.0
-:version: 0.4.3
+:version: 0.4.4
 :status: Alpha
 
 ..
 
-    Copyright 2021 Thomas Calmant
+    Copyright 2024 Thomas Calmant
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
 
@@ -22,26 +22,26 @@
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 """
 
 from __future__ import absolute_import
 
+import logging
 from enum import IntEnum
 from typing import Any, Dict, List, Optional, Set
-import logging
 
 from ..constants import ClassDescFlags, TypeCode
-from ..modifiedutf8 import decode_modified_utf8, byte_to_int
+from ..modifiedutf8 import byte_to_int, decode_modified_utf8
 from ..utils import UNICODE_TYPE
 
 # ------------------------------------------------------------------------------
 
 # Module version
-__version_info__ = (0, 4, 3)
+__version_info__ = (0, 4, 4)
 __version__ = ".".join(str(x) for x in __version_info__)
 
 # Documentation strings format
 __docformat__ = "restructuredtext en"
 
 # ------------------------------------------------------------------------------
```

### Comparing `javaobj-py3-0.4.3/javaobj/v2/core.py` & `javaobj-py3-0.4.4/javaobj/v2/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 #!/usr/bin/env python3
 """
 Second parsing approach for javaobj, using the same approach as jdeserialize
 See: https://github.com/frohoff/jdeserialize
 
 :authors: Thomas Calmant
 :license: Apache License 2.0
-:version: 0.4.3
+:version: 0.4.4
 :status: Alpha
 
 ..
 
-    Copyright 2021 Thomas Calmant
+    Copyright 2024 Thomas Calmant
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
 
@@ -23,68 +23,67 @@
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 """
 
 from __future__ import absolute_import
 
-from typing import (
+import logging
+import os
+from typing import (  # pylint:disable=W0611
+    IO,
     Any,
     Callable,
     Dict,
-    IO,
     List,
     Optional,
-)  # pylint:disable=W0611
-import logging
-import os
+)
 
+from ..constants import (
+    PRIMITIVE_TYPES,
+    StreamConstants,
+    TerminalCode,
+    TypeCode,
+)
+from ..modifiedutf8 import (  # pylint:disable=W0611  # noqa: F401
+    decode_modified_utf8,
+)
 from . import api  # pylint:disable=W0611
 from .beans import (
-    ParsedJavaContent,
     BlockData,
-    JavaClassDesc,
-    JavaClass,
+    ClassDataType,
+    ClassDescType,
+    ExceptionRead,
+    ExceptionState,
+    FieldType,
     JavaArray,
+    JavaClass,
+    JavaClassDesc,
     JavaEnum,
     JavaField,
     JavaInstance,
     JavaString,
-    ExceptionState,
-    ExceptionRead,
-    ClassDescType,
-    FieldType,
-    ClassDataType,
+    ParsedJavaContent,
 )
 from .stream import DataStreamReader
 from .transformers import DefaultObjectTransformer
-from ..constants import (
-    StreamConstants,
-    TerminalCode,
-    TypeCode,
-    PRIMITIVE_TYPES,
-)
-
-from ..modifiedutf8 import (
-    decode_modified_utf8,
-)  # pylint:disable=W0611  # noqa: F401
 
 # ------------------------------------------------------------------------------
 
 # Module version
-__version_info__ = (0, 4, 3)
+__version_info__ = (0, 4, 4)
 __version__ = ".".join(str(x) for x in __version_info__)
 
 # Documentation strings format
 __docformat__ = "restructuredtext en"
 
 # ------------------------------------------------------------------------------
 
 
-class JavaStreamParser:
+class JavaStreamParser(api.IJavaStreamParser):
     """
     Parses a Java stream
     """
 
     def __init__(self, fd, transformers):
         # type: (IO[bytes], List[api.ObjectTransformer]) -> None
         """
```

### Comparing `javaobj-py3-0.4.3/javaobj/v2/main.py` & `javaobj-py3-0.4.4/javaobj/v2/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 #!/usr/bin/env python3
 """
 Mimics the core API with the new deserializer
 """
 
 from __future__ import absolute_import
 
-from typing import Any, IO  # pylint:disable=W0611
+from typing import IO, Any  # pylint:disable=W0611
 
 try:
     # Python 2
     from StringIO import StringIO as BytesIO
 except ImportError:
     # Python 3+
     from io import BytesIO
 
+from ..utils import java_data_fd
 from .api import ObjectTransformer  # pylint:disable=W0611
 from .core import JavaStreamParser
 from .transformers import DefaultObjectTransformer, NumpyArrayTransformer
-from ..utils import java_data_fd
 
 # ------------------------------------------------------------------------------
 
 # Module version
-__version_info__ = (0, 4, 3)
+__version_info__ = (0, 4, 4)
 __version__ = ".".join(str(x) for x in __version_info__)
 
 # Documentation strings format
 __docformat__ = "restructuredtext en"
 
 # ------------------------------------------------------------------------------
```

### Comparing `javaobj-py3-0.4.3/javaobj/v2/stream.py` & `javaobj-py3-0.4.4/javaobj/v2/stream.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 #!/usr/bin/env python3
 """
 Utility module to handle streams like in Java
 
 :authors: Thomas Calmant
 :license: Apache License 2.0
-:version: 0.4.3
+:version: 0.4.4
 :status: Alpha
 
 ..
 
-    Copyright 2021 Thomas Calmant
+    Copyright 2024 Thomas Calmant
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
 
@@ -22,24 +22,24 @@
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 """
 
 from __future__ import absolute_import
 
-from typing import Any, IO, Tuple  # pylint:disable=W0611
 import struct
+from typing import IO, Any, Tuple  # pylint:disable=W0611
 
 from ..modifiedutf8 import decode_modified_utf8
-from ..utils import unicode_char, UNICODE_TYPE  # pylint:disable=W0611
+from ..utils import UNICODE_TYPE, unicode_char  # pylint:disable=W0611
 
 # ------------------------------------------------------------------------------
 
 # Module version
-__version_info__ = (0, 4, 3)
+__version_info__ = (0, 4, 4)
 __version__ = ".".join(str(x) for x in __version_info__)
 
 # Documentation strings format
 __docformat__ = "restructuredtext en"
 
 # ------------------------------------------------------------------------------
```

### Comparing `javaobj-py3-0.4.3/javaobj/v2/transformers.py` & `javaobj-py3-0.4.4/javaobj/v2/transformers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 #!/usr/bin/env python3
 """
 Defines the default object transformers
 
 :authors: Thomas Calmant
 :license: Apache License 2.0
-:version: 0.4.3
+:version: 0.4.4
 :status: Alpha
 
 ..
 
-    Copyright 2021 Thomas Calmant
+    Copyright 2024 Thomas Calmant
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
 
@@ -21,38 +21,38 @@
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 """
 
 # Standard library
-from typing import List, Optional, Tuple
 import functools
+from typing import List, Optional, Tuple
 
 # Numpy (optional)
 try:
     import numpy
 except ImportError:
-    numpy = None
-
+    numpy = None  # type: ignore
 
 # Javaobj
-from .api import ObjectTransformer
-from .beans import (
-    JavaInstance,
-    JavaClassDesc,
-    BlockData,
-)  # pylint:disable=W0611
 from ..constants import TerminalCode, TypeCode
-from ..utils import to_bytes, log_error, log_debug, read_struct, read_string
+from ..utils import log_debug, log_error, read_string, read_struct, to_bytes
+from .api import IJavaStreamParser, ObjectTransformer
+from .beans import ( # pylint:disable=W0611
+    BlockData,
+    JavaClassDesc,
+    JavaInstance,
+)
+from .stream import DataStreamReader
 
 # ------------------------------------------------------------------------------
 
 # Module version
-__version_info__ = (0, 4, 3)
+__version_info__ = (0, 4, 4)
 __version__ = ".".join(str(x) for x in __version_info__)
 
 # Documentation strings format
 __docformat__ = "restructuredtext en"
 
 # ------------------------------------------------------------------------------
 
@@ -179,15 +179,15 @@
     """
     Linked has map are handled with a specific block data
     """
 
     HANDLED_CLASSES = ("java.util.LinkedHashMap",)
 
     def load_from_blockdata(self, parser, reader, indent=0):
-        # type: (JavaStreamParser, DataStreamReader, int) -> bool
+        # type: (IJavaStreamParser, DataStreamReader, int) -> bool
         """
         Loads the content of the map, written with a custom implementation
         """
         # Read HashMap fields
         self.buckets = reader.read_int()
         self.size = reader.read_int()
```

### Comparing `javaobj-py3-0.4.3/setup.py` & `javaobj-py3-0.4.4/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,20 +3,20 @@
 pickle and json modules.
 
 See:
 http://download.oracle.com/javase/6/docs/platform/serialization/spec/protocol.html
 
 :authors: Volodymyr Buell, Thomas Calmant
 :license: Apache License 2.0
-:version: 0.4.3
+:version: 0.4.4
 :status: Alpha
 
 ..
 
-    Copyright 2021 Thomas Calmant
+    Copyright 2024 Thomas Calmant
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
 
@@ -33,15 +33,15 @@
     from setuptools import setup
 except ImportError:
     from distutils.core import setup
 
 # ------------------------------------------------------------------------------
 
 # Module version
-__version_info__ = (0, 4, 3)
+__version_info__ = (0, 4, 4)
 __version__ = ".".join(str(x) for x in __version_info__)
 
 # Documentation strings format
 __docformat__ = "restructuredtext en"
 
 # ------------------------------------------------------------------------------
 
@@ -83,10 +83,14 @@
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 2.7",
         "Programming Language :: Python :: 3.4",
         "Programming Language :: Python :: 3.5",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
         "Topic :: Software Development :: Libraries :: Python Modules",
     ],
 )
```

