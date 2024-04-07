# Comparing `tmp/scrollablecontainers-2.0.1.tar.gz` & `tmp/scrollablecontainers-2.0.1a0.tar.gz`

## Comparing `scrollablecontainers-2.0.1.tar` & `scrollablecontainers-2.0.1a0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     5174 2020-02-02 00:00:00.000000 scrollablecontainers-2.0.1/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 scrollablecontainers-2.0.1/CONTRIBUTING.md
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 scrollablecontainers-2.0.1/SECURITY.md
--rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 scrollablecontainers-2.0.1/.github/ISSUE_TEMPLATE/bug-report.md
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 scrollablecontainers-2.0.1/.github/ISSUE_TEMPLATE/feature-request.md
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 scrollablecontainers-2.0.1/.github/workflows/build.yml
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 scrollablecontainers-2.0.1/.github/workflows/install.yml
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 scrollablecontainers-2.0.1/.github/workflows/lint.yml
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 scrollablecontainers-2.0.1/examples/README.md
--rwxr-xr-x   0        0        0     1519 2020-02-02 00:00:00.000000 scrollablecontainers-2.0.1/examples/examples_ScrollableAreaQt5.py
--rwxr-xr-x   0        0        0     1519 2020-02-02 00:00:00.000000 scrollablecontainers-2.0.1/examples/examples_ScrollableAreaQt6.py
--rwxr-xr-x   0        0        0     1286 2020-02-02 00:00:00.000000 scrollablecontainers-2.0.1/examples/examples_ScrollableFrameTk.py
--rwxr-xr-x   0        0        0     1350 2020-02-02 00:00:00.000000 scrollablecontainers-2.0.1/examples/examples_ScrollablePanelWx.py
--rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 scrollablecontainers-2.0.1/src/ScrollableContainers/__init__.py
--rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 scrollablecontainers-2.0.1/src/ScrollableContainers/_qt5.py
--rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 scrollablecontainers-2.0.1/src/ScrollableContainers/_qt6.py
--rw-r--r--   0        0        0     6719 2020-02-02 00:00:00.000000 scrollablecontainers-2.0.1/src/ScrollableContainers/_tk.py
--rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 scrollablecontainers-2.0.1/src/ScrollableContainers/_wx.py
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 scrollablecontainers-2.0.1/.gitignore
--rw-r--r--   0        0        0    31917 2020-02-02 00:00:00.000000 scrollablecontainers-2.0.1/COPYING.md
--rw-r--r--   0        0        0     4402 2020-02-02 00:00:00.000000 scrollablecontainers-2.0.1/README.md
--rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 scrollablecontainers-2.0.1/pyproject.toml
--rw-r--r--   0        0        0     5151 2020-02-02 00:00:00.000000 scrollablecontainers-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0     5174 2020-02-02 00:00:00.000000 scrollablecontainers-2.0.1a0/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 scrollablecontainers-2.0.1a0/CONTRIBUTING.md
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 scrollablecontainers-2.0.1a0/SECURITY.md
+-rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 scrollablecontainers-2.0.1a0/.github/ISSUE_TEMPLATE/bug-report.md
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 scrollablecontainers-2.0.1a0/.github/ISSUE_TEMPLATE/feature-request.md
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 scrollablecontainers-2.0.1a0/.github/workflows/build.yml
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 scrollablecontainers-2.0.1a0/.github/workflows/install.yml
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 scrollablecontainers-2.0.1a0/.github/workflows/lint.yml
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 scrollablecontainers-2.0.1a0/examples/README.md
+-rwxr-xr-x   0        0        0     1519 2020-02-02 00:00:00.000000 scrollablecontainers-2.0.1a0/examples/examples_ScrollableAreaQt5.py
+-rwxr-xr-x   0        0        0     1519 2020-02-02 00:00:00.000000 scrollablecontainers-2.0.1a0/examples/examples_ScrollableAreaQt6.py
+-rwxr-xr-x   0        0        0     1286 2020-02-02 00:00:00.000000 scrollablecontainers-2.0.1a0/examples/examples_ScrollableFrameTk.py
+-rwxr-xr-x   0        0        0     1350 2020-02-02 00:00:00.000000 scrollablecontainers-2.0.1a0/examples/examples_ScrollablePanelWx.py
+-rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 scrollablecontainers-2.0.1a0/src/ScrollableContainers/__init__.py
+-rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 scrollablecontainers-2.0.1a0/src/ScrollableContainers/_qt5.py
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 scrollablecontainers-2.0.1a0/src/ScrollableContainers/_qt6.py
+-rw-r--r--   0        0        0     6719 2020-02-02 00:00:00.000000 scrollablecontainers-2.0.1a0/src/ScrollableContainers/_tk.py
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 scrollablecontainers-2.0.1a0/src/ScrollableContainers/_wx.py
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 scrollablecontainers-2.0.1a0/.gitignore
+-rw-r--r--   0        0        0    31917 2020-02-02 00:00:00.000000 scrollablecontainers-2.0.1a0/COPYING.md
+-rw-r--r--   0        0        0     4402 2020-02-02 00:00:00.000000 scrollablecontainers-2.0.1a0/README.md
+-rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 scrollablecontainers-2.0.1a0/pyproject.toml
+-rw-r--r--   0        0        0     5153 2020-02-02 00:00:00.000000 scrollablecontainers-2.0.1a0/PKG-INFO
```

### Comparing `scrollablecontainers-2.0.1/CODE_OF_CONDUCT.md` & `scrollablecontainers-2.0.1a0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `scrollablecontainers-2.0.1/.github/ISSUE_TEMPLATE/bug-report.md` & `scrollablecontainers-2.0.1a0/.github/ISSUE_TEMPLATE/bug-report.md`

 * *Files identical despite different names*

### Comparing `scrollablecontainers-2.0.1/.github/ISSUE_TEMPLATE/feature-request.md` & `scrollablecontainers-2.0.1a0/.github/ISSUE_TEMPLATE/feature-request.md`

 * *Files identical despite different names*

### Comparing `scrollablecontainers-2.0.1/examples/examples_ScrollableAreaQt5.py` & `scrollablecontainers-2.0.1a0/examples/examples_ScrollableAreaQt5.py`

 * *Files identical despite different names*

### Comparing `scrollablecontainers-2.0.1/examples/examples_ScrollableAreaQt6.py` & `scrollablecontainers-2.0.1a0/examples/examples_ScrollableAreaQt6.py`

 * *Files identical despite different names*

### Comparing `scrollablecontainers-2.0.1/examples/examples_ScrollableFrameTk.py` & `scrollablecontainers-2.0.1a0/examples/examples_ScrollableFrameTk.py`

 * *Files identical despite different names*

### Comparing `scrollablecontainers-2.0.1/examples/examples_ScrollablePanelWx.py` & `scrollablecontainers-2.0.1a0/examples/examples_ScrollablePanelWx.py`

 * *Files identical despite different names*

### Comparing `scrollablecontainers-2.0.1/src/ScrollableContainers/_qt5.py` & `scrollablecontainers-2.0.1a0/src/ScrollableContainers/_qt5.py`

 * *Files identical despite different names*

### Comparing `scrollablecontainers-2.0.1/src/ScrollableContainers/_qt6.py` & `scrollablecontainers-2.0.1a0/src/ScrollableContainers/_qt6.py`

 * *Files identical despite different names*

### Comparing `scrollablecontainers-2.0.1/src/ScrollableContainers/_tk.py` & `scrollablecontainers-2.0.1a0/src/ScrollableContainers/_tk.py`

 * *Files identical despite different names*

### Comparing `scrollablecontainers-2.0.1/src/ScrollableContainers/_wx.py` & `scrollablecontainers-2.0.1a0/src/ScrollableContainers/_wx.py`

 * *Files identical despite different names*

### Comparing `scrollablecontainers-2.0.1/COPYING.md` & `scrollablecontainers-2.0.1a0/COPYING.md`

 * *Files identical despite different names*

### Comparing `scrollablecontainers-2.0.1/README.md` & `scrollablecontainers-2.0.1a0/README.md`

 * *Files identical despite different names*

### Comparing `scrollablecontainers-2.0.1/pyproject.toml` & `scrollablecontainers-2.0.1a0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "ScrollableContainers"
-version = "2.0.1"
+version = "2.0.1a0"
 authors = [
     { name = "Vishal Pankaj Chandratreya" },
 ]
 description = "Scrollable containers for Tkinter, wxPython, PyQt5 and PyQt6"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `scrollablecontainers-2.0.1/PKG-INFO` & `scrollablecontainers-2.0.1a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: ScrollableContainers
-Version: 2.0.1
+Version: 2.0.1a0
 Summary: Scrollable containers for Tkinter, wxPython, PyQt5 and PyQt6
 Project-URL: Homepage, https://github.com/tfpf/ScrollableContainers
 Project-URL: Bug Tracker, https://github.com/tfpf/ScrollableContainers/issues
 Author: Vishal Pankaj Chandratreya
 License-File: COPYING.md
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

