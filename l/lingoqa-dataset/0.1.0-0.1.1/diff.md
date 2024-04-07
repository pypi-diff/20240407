# Comparing `tmp/lingoqa_dataset-0.1.0.tar.gz` & `tmp/lingoqa_dataset-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lingoqa_dataset-0.1.0.tar", max compression
+gzip compressed data, was "lingoqa_dataset-0.1.1.tar", max compression
```

## Comparing `lingoqa_dataset-0.1.0.tar` & `lingoqa_dataset-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      864 2024-04-06 17:14:01.838226 lingoqa_dataset-0.1.0/README.md
--rw-r--r--   0        0        0        0 2024-04-06 14:02:23.899843 lingoqa_dataset-0.1.0/lingoqa_dataset/__init__,py
--rw-r--r--   0        0        0     4003 2024-04-06 17:04:48.532592 lingoqa_dataset-0.1.0/lingoqa_dataset/lingoqa_dataset.py
--rw-r--r--   0        0        0      699 2024-04-06 17:12:18.443677 lingoqa_dataset-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1644 1970-01-01 00:00:00.000000 lingoqa_dataset-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      864 2024-04-06 17:14:01.838226 lingoqa_dataset-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2024-04-06 14:02:23.899843 lingoqa_dataset-0.1.1/lingoqa_dataset/__init__,py
+-rw-r--r--   0        0        0     4003 2024-04-06 17:04:48.532592 lingoqa_dataset-0.1.1/lingoqa_dataset/lingoqa_dataset.py
+-rw-r--r--   0        0        0      715 2024-04-06 17:45:46.637238 lingoqa_dataset-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1644 1970-01-01 00:00:00.000000 lingoqa_dataset-0.1.1/PKG-INFO
```

### Comparing `lingoqa_dataset-0.1.0/README.md` & `lingoqa_dataset-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `lingoqa_dataset-0.1.0/lingoqa_dataset/lingoqa_dataset.py` & `lingoqa_dataset-0.1.1/lingoqa_dataset/lingoqa_dataset.py`

 * *Files identical despite different names*

### Comparing `lingoqa_dataset-0.1.0/pyproject.toml` & `lingoqa_dataset-0.1.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lingoqa-dataset"
-version = "0.1.0"
+version = "0.1.1"
 description = "LingoQA dataset for pytorch"
 authors = ["Masaya Kataoka <ms.kataoka@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/hakuturu583"
 repository = "https://github.com/hakuturu583/lingoqa_dataset"
 
 
@@ -22,11 +22,12 @@
 [tool.poetry.group.dev.dependencies]
 flake8 = "^7.0.0"
 black = "^24.3.0"
 isort = "^5.13.2"
 mypy = "^1.9.0"
 pytest = "^8.1.1"
 pre-commit = "^3.7.0"
+lark = "^1.1.9"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `lingoqa_dataset-0.1.0/PKG-INFO` & `lingoqa_dataset-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lingoqa-dataset
-Version: 0.1.0
+Version: 0.1.1
 Summary: LingoQA dataset for pytorch
 Home-page: https://github.com/hakuturu583
 Author: Masaya Kataoka
 Author-email: ms.kataoka@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

