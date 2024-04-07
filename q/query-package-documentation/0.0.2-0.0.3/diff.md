# Comparing `tmp/query-package-documentation-0.0.2.tar.gz` & `tmp/query-package-documentation-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "query-package-documentation-0.0.2.tar", last modified: Fri Jan 26 19:00:02 2024, max compression
+gzip compressed data, was "query-package-documentation-0.0.3.tar", last modified: Sun Apr  7 15:38:22 2024, max compression
```

## Comparing `query-package-documentation-0.0.2.tar` & `query-package-documentation-0.0.3.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 anirban   (1000) anirban   (1000)        0 2024-01-26 19:00:02.776709 query-package-documentation-0.0.2/
--rw-r--r--   0 anirban   (1000) anirban   (1000)     1068 2024-01-26 18:14:33.000000 query-package-documentation-0.0.2/LICENSE
--rw-r--r--   0 anirban   (1000) anirban   (1000)     5643 2024-01-26 19:00:02.776709 query-package-documentation-0.0.2/PKG-INFO
--rw-r--r--   0 anirban   (1000) anirban   (1000)      194 2024-01-26 18:14:33.000000 query-package-documentation-0.0.2/README.md
--rw-r--r--   0 anirban   (1000) anirban   (1000)     5434 2024-01-26 18:58:41.000000 query-package-documentation-0.0.2/pyproject.toml
--rw-r--r--   0 anirban   (1000) anirban   (1000)       38 2024-01-26 19:00:02.776709 query-package-documentation-0.0.2/setup.cfg
-drwxr-xr-x   0 anirban   (1000) anirban   (1000)        0 2024-01-26 19:00:02.756709 query-package-documentation-0.0.2/src/
--rw-r--r--   0 anirban   (1000) anirban   (1000)     5757 2024-01-26 18:14:33.000000 query-package-documentation-0.0.2/src/cli.py
-drwxr-xr-x   0 anirban   (1000) anirban   (1000)        0 2024-01-26 19:00:02.766709 query-package-documentation-0.0.2/src/generative_ai/
--rw-r--r--   0 anirban   (1000) anirban   (1000)     1170 2024-01-26 18:14:33.000000 query-package-documentation-0.0.2/src/generative_ai/__init__.py
-drwxr-xr-x   0 anirban   (1000) anirban   (1000)        0 2024-01-26 19:00:02.766709 query-package-documentation-0.0.2/src/generative_ai/dataset_generation/
--rw-r--r--   0 anirban   (1000) anirban   (1000)      846 2024-01-26 18:14:33.000000 query-package-documentation-0.0.2/src/generative_ai/dataset_generation/__init__.py
--rw-r--r--   0 anirban   (1000) anirban   (1000)     4730 2024-01-26 18:14:33.000000 query-package-documentation-0.0.2/src/generative_ai/dataset_generation/orchestrate_generation.py
--rw-r--r--   0 anirban   (1000) anirban   (1000)    12343 2024-01-26 18:14:33.000000 query-package-documentation-0.0.2/src/generative_ai/dataset_generation/step_1_generation.py
--rw-r--r--   0 anirban   (1000) anirban   (1000)   132462 2024-01-26 18:14:33.000000 query-package-documentation-0.0.2/src/generative_ai/dataset_generation/step_2_generation.py
--rw-r--r--   0 anirban   (1000) anirban   (1000)    17063 2024-01-26 18:14:33.000000 query-package-documentation-0.0.2/src/generative_ai/dataset_generation/utils_generation.py
-drwxr-xr-x   0 anirban   (1000) anirban   (1000)        0 2024-01-26 19:00:02.766709 query-package-documentation-0.0.2/src/generative_ai/information_retrieval/
--rw-r--r--   0 anirban   (1000) anirban   (1000)     1438 2024-01-26 18:14:33.000000 query-package-documentation-0.0.2/src/generative_ai/information_retrieval/__init__.py
--rw-r--r--   0 anirban   (1000) anirban   (1000)     6919 2024-01-26 18:14:33.000000 query-package-documentation-0.0.2/src/generative_ai/information_retrieval/orchestrate_retrieval.py
--rw-r--r--   0 anirban   (1000) anirban   (1000)     2554 2024-01-26 18:14:33.000000 query-package-documentation-0.0.2/src/generative_ai/information_retrieval/step_1_retrieval.py
--rw-r--r--   0 anirban   (1000) anirban   (1000)     5618 2024-01-26 18:14:33.000000 query-package-documentation-0.0.2/src/generative_ai/information_retrieval/step_2_retrieval.py
--rw-r--r--   0 anirban   (1000) anirban   (1000)     2599 2024-01-26 18:14:33.000000 query-package-documentation-0.0.2/src/generative_ai/information_retrieval/step_3_retrieval.py
--rw-r--r--   0 anirban   (1000) anirban   (1000)     2326 2024-01-26 18:14:33.000000 query-package-documentation-0.0.2/src/generative_ai/information_retrieval/utils_retrieval.py
--rw-r--r--   0 anirban   (1000) anirban   (1000)      642 2024-01-26 18:14:33.000000 query-package-documentation-0.0.2/src/generative_ai/metadata.json
--rw-r--r--   0 anirban   (1000) anirban   (1000)        0 2024-01-26 18:14:33.000000 query-package-documentation-0.0.2/src/generative_ai/py.typed
--rw-r--r--   0 anirban   (1000) anirban   (1000)     6568 2024-01-26 18:14:33.000000 query-package-documentation-0.0.2/src/generative_ai/top_level.py
--rw-r--r--   0 anirban   (1000) anirban   (1000)      744 2024-01-26 18:14:33.000000 query-package-documentation-0.0.2/src/generative_ai/utils_top_level.py
--rw-r--r--   0 anirban   (1000) anirban   (1000)    24732 2024-01-26 18:14:33.000000 query-package-documentation-0.0.2/src/gui.py
-drwxr-xr-x   0 anirban   (1000) anirban   (1000)        0 2024-01-26 19:00:02.776709 query-package-documentation-0.0.2/src/query_package_documentation.egg-info/
--rw-r--r--   0 anirban   (1000) anirban   (1000)     5643 2024-01-26 19:00:02.000000 query-package-documentation-0.0.2/src/query_package_documentation.egg-info/PKG-INFO
--rw-r--r--   0 anirban   (1000) anirban   (1000)     1184 2024-01-26 19:00:02.000000 query-package-documentation-0.0.2/src/query_package_documentation.egg-info/SOURCES.txt
--rw-r--r--   0 anirban   (1000) anirban   (1000)        1 2024-01-26 19:00:02.000000 query-package-documentation-0.0.2/src/query_package_documentation.egg-info/dependency_links.txt
--rw-r--r--   0 anirban   (1000) anirban   (1000)       84 2024-01-26 19:00:02.000000 query-package-documentation-0.0.2/src/query_package_documentation.egg-info/entry_points.txt
--rw-r--r--   0 anirban   (1000) anirban   (1000)      921 2024-01-26 19:00:02.000000 query-package-documentation-0.0.2/src/query_package_documentation.egg-info/requires.txt
--rw-r--r--   0 anirban   (1000) anirban   (1000)       22 2024-01-26 19:00:02.000000 query-package-documentation-0.0.2/src/query_package_documentation.egg-info/top_level.txt
+drwxr-xr-x   0 anirban   (1000) anirban   (1000)        0 2024-04-07 15:38:22.249653 query-package-documentation-0.0.3/
+-rw-r--r--   0 anirban   (1000) anirban   (1000)     1073 2024-04-07 15:36:05.000000 query-package-documentation-0.0.3/LICENSE
+-rw-r--r--   0 anirban   (1000) anirban   (1000)     5779 2024-04-07 15:38:22.249653 query-package-documentation-0.0.3/PKG-INFO
+-rw-r--r--   0 anirban   (1000) anirban   (1000)      194 2024-01-26 18:48:33.000000 query-package-documentation-0.0.3/README.md
+-rw-r--r--   0 anirban   (1000) anirban   (1000)     9676 2024-04-07 15:36:05.000000 query-package-documentation-0.0.3/pyproject.toml
+-rw-r--r--   0 anirban   (1000) anirban   (1000)       38 2024-04-07 15:38:22.249653 query-package-documentation-0.0.3/setup.cfg
+drwxr-xr-x   0 anirban   (1000) anirban   (1000)        0 2024-04-07 15:38:22.239653 query-package-documentation-0.0.3/src/
+-rw-r--r--   0 anirban   (1000) anirban   (1000)     5757 2024-01-26 19:33:11.000000 query-package-documentation-0.0.3/src/cli.py
+drwxr-xr-x   0 anirban   (1000) anirban   (1000)        0 2024-04-07 15:38:22.239653 query-package-documentation-0.0.3/src/generative_ai/
+-rw-r--r--   0 anirban   (1000) anirban   (1000)     1170 2024-01-26 19:33:11.000000 query-package-documentation-0.0.3/src/generative_ai/__init__.py
+drwxr-xr-x   0 anirban   (1000) anirban   (1000)        0 2024-04-07 15:38:22.249653 query-package-documentation-0.0.3/src/generative_ai/dataset_generation/
+-rw-r--r--   0 anirban   (1000) anirban   (1000)      846 2024-01-26 19:33:11.000000 query-package-documentation-0.0.3/src/generative_ai/dataset_generation/__init__.py
+-rw-r--r--   0 anirban   (1000) anirban   (1000)     4730 2024-01-26 19:33:11.000000 query-package-documentation-0.0.3/src/generative_ai/dataset_generation/orchestrate_generation.py
+-rw-r--r--   0 anirban   (1000) anirban   (1000)    12343 2024-04-07 08:38:13.000000 query-package-documentation-0.0.3/src/generative_ai/dataset_generation/step_1_generation.py
+-rw-r--r--   0 anirban   (1000) anirban   (1000)   128636 2024-04-07 15:36:05.000000 query-package-documentation-0.0.3/src/generative_ai/dataset_generation/step_2_generation.py
+-rw-r--r--   0 anirban   (1000) anirban   (1000)    14819 2024-04-07 15:36:05.000000 query-package-documentation-0.0.3/src/generative_ai/dataset_generation/utils_generation.py
+drwxr-xr-x   0 anirban   (1000) anirban   (1000)        0 2024-04-07 15:38:22.249653 query-package-documentation-0.0.3/src/generative_ai/information_retrieval/
+-rw-r--r--   0 anirban   (1000) anirban   (1000)     1394 2024-04-07 15:36:05.000000 query-package-documentation-0.0.3/src/generative_ai/information_retrieval/__init__.py
+-rw-r--r--   0 anirban   (1000) anirban   (1000)     6990 2024-04-07 15:36:05.000000 query-package-documentation-0.0.3/src/generative_ai/information_retrieval/orchestrate_retrieval.py
+-rw-r--r--   0 anirban   (1000) anirban   (1000)     2552 2024-04-07 15:36:05.000000 query-package-documentation-0.0.3/src/generative_ai/information_retrieval/step_1_retrieval.py
+-rw-r--r--   0 anirban   (1000) anirban   (1000)     5777 2024-04-07 15:36:05.000000 query-package-documentation-0.0.3/src/generative_ai/information_retrieval/step_2_retrieval.py
+-rw-r--r--   0 anirban   (1000) anirban   (1000)     2652 2024-04-07 15:36:05.000000 query-package-documentation-0.0.3/src/generative_ai/information_retrieval/step_3_retrieval.py
+-rw-r--r--   0 anirban   (1000) anirban   (1000)     2207 2024-04-07 15:36:05.000000 query-package-documentation-0.0.3/src/generative_ai/information_retrieval/utils_retrieval.py
+-rw-r--r--   0 anirban   (1000) anirban   (1000)      642 2024-04-07 15:36:05.000000 query-package-documentation-0.0.3/src/generative_ai/metadata.json
+-rw-r--r--   0 anirban   (1000) anirban   (1000)        0 2023-12-31 10:51:21.000000 query-package-documentation-0.0.3/src/generative_ai/py.typed
+-rw-r--r--   0 anirban   (1000) anirban   (1000)     6568 2024-04-07 08:38:13.000000 query-package-documentation-0.0.3/src/generative_ai/top_level.py
+-rw-r--r--   0 anirban   (1000) anirban   (1000)      744 2024-01-26 19:33:11.000000 query-package-documentation-0.0.3/src/generative_ai/utils_top_level.py
+-rw-r--r--   0 anirban   (1000) anirban   (1000)    24732 2024-02-18 15:03:17.000000 query-package-documentation-0.0.3/src/gui.py
+drwxr-xr-x   0 anirban   (1000) anirban   (1000)        0 2024-04-07 15:38:22.249653 query-package-documentation-0.0.3/src/query_package_documentation.egg-info/
+-rw-r--r--   0 anirban   (1000) anirban   (1000)     5779 2024-04-07 15:38:22.000000 query-package-documentation-0.0.3/src/query_package_documentation.egg-info/PKG-INFO
+-rw-r--r--   0 anirban   (1000) anirban   (1000)     1184 2024-04-07 15:38:22.000000 query-package-documentation-0.0.3/src/query_package_documentation.egg-info/SOURCES.txt
+-rw-r--r--   0 anirban   (1000) anirban   (1000)        1 2024-04-07 15:38:22.000000 query-package-documentation-0.0.3/src/query_package_documentation.egg-info/dependency_links.txt
+-rw-r--r--   0 anirban   (1000) anirban   (1000)       84 2024-04-07 15:38:22.000000 query-package-documentation-0.0.3/src/query_package_documentation.egg-info/entry_points.txt
+-rw-r--r--   0 anirban   (1000) anirban   (1000)      974 2024-04-07 15:38:22.000000 query-package-documentation-0.0.3/src/query_package_documentation.egg-info/requires.txt
+-rw-r--r--   0 anirban   (1000) anirban   (1000)       22 2024-04-07 15:38:22.000000 query-package-documentation-0.0.3/src/query_package_documentation.egg-info/top_level.txt
```

### Comparing `query-package-documentation-0.0.2/LICENSE` & `query-package-documentation-0.0.3/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 Anirban Ray
+Copyright (c) 2023-2024 Anirban Ray
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `query-package-documentation-0.0.2/PKG-INFO` & `query-package-documentation-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: query-package-documentation
-Version: 0.0.2
+Version: 0.0.3
 Summary: A package to explore documentations
 Author-email: Anirban Ray <39331844+yarnabrina@users.noreply.github.com>
 Maintainer-email: Anirban Ray <39331844+yarnabrina@users.noreply.github.com>
 License: MIT License
         
-        Copyright (c) 2023 Anirban Ray
+        Copyright (c) 2023-2024 Anirban Ray
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
         to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
         copies of the Software, and to permit persons to whom the Software is
         furnished to do so, subject to the following conditions:
@@ -47,22 +47,22 @@
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Python: ==3.11.*
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: chromadb<0.5,>=0.4.15
 Requires-Dist: ctransformers<0.3,>=0.2.27
-Requires-Dist: gradio<4.17,>=4.12
-Requires-Dist: jq<1.7,>=1.6
-Requires-Dist: langchain<0.1.5,>=0.1.1
-Requires-Dist: numpydoc<1.7,>=1.6
-Requires-Dist: pydantic<2.6,>=2.4.2
-Requires-Dist: sentence-transformers<2.3,>=2.2.2
-Requires-Dist: transformers<4.38,>=4.36
-Requires-Dist: typer<0.10,>=0.9
+Requires-Dist: gradio<4.26,>=4.19.2
+Requires-Dist: jq<1.8,>=1.6
+Requires-Dist: langchain<0.2,>=0.1.13
+Requires-Dist: numpydoc<1.8,>=1.6
+Requires-Dist: pydantic<2.7,>=2.4.2
+Requires-Dist: sentence-transformers<2.7,>=2.2.2
+Requires-Dist: transformers<4.39,>=4.36
+Requires-Dist: typer-slim<0.13,>=0.12.1
 Provides-Extra: all
 Requires-Dist: autoflake; extra == "all"
 Requires-Dist: bandit; extra == "all"
 Requires-Dist: black; extra == "all"
 Requires-Dist: blacken-docs; extra == "all"
 Requires-Dist: build; extra == "all"
 Requires-Dist: codespell; extra == "all"
@@ -88,22 +88,24 @@
 Requires-Dist: pre-commit; extra == "dev"
 Provides-Extra: doc
 Requires-Dist: furo; extra == "doc"
 Requires-Dist: myst-parser[linkify]; extra == "doc"
 Requires-Dist: Sphinx; extra == "doc"
 Requires-Dist: sphinx-copybutton; extra == "doc"
 Provides-Extra: fine-tuning
-Requires-Dist: accelerate<0.27,>=0.24.1; extra == "fine-tuning"
-Requires-Dist: bitsandbytes<0.43,>=0.41.2; extra == "fine-tuning"
-Requires-Dist: datasets<2.17,>=2.15; extra == "fine-tuning"
-Requires-Dist: peft<0.8,>=0.6.2; extra == "fine-tuning"
+Requires-Dist: accelerate<0.30,>=0.24.1; extra == "fine-tuning"
+Requires-Dist: bitsandbytes<0.44,>=0.41.2; extra == "fine-tuning"
+Requires-Dist: datasets<2.19,>=2.15; extra == "fine-tuning"
+Requires-Dist: evaluate<0.5,>=0.4.1; extra == "fine-tuning"
+Requires-Dist: peft<0.11,>=0.6.2; extra == "fine-tuning"
+Requires-Dist: rouge-score<0.2,>=0.1.2; extra == "fine-tuning"
 Requires-Dist: safetensors<0.5,>=0.4; extra == "fine-tuning"
-Requires-Dist: torch<2.2,>=2.1.1; extra == "fine-tuning"
-Requires-Dist: transformers<4.38,>=4.36; extra == "fine-tuning"
-Requires-Dist: trl<0.8,>=0.7.4; extra == "fine-tuning"
+Requires-Dist: scikit-learn<1.5,>=1.3; extra == "fine-tuning"
+Requires-Dist: torch<2.3,>=2.1.1; extra == "fine-tuning"
+Requires-Dist: trl<0.9,>=0.7.4; extra == "fine-tuning"
 Provides-Extra: format
 Requires-Dist: autoflake; extra == "format"
 Requires-Dist: black; extra == "format"
 Requires-Dist: blacken-docs; extra == "format"
 Requires-Dist: docformatter[tomli]; extra == "format"
 Requires-Dist: isort; extra == "format"
 Requires-Dist: pyproject-fmt; extra == "format"
```

### Comparing `query-package-documentation-0.0.2/src/cli.py` & `query-package-documentation-0.0.3/src/cli.py`

 * *Files identical despite different names*

### Comparing `query-package-documentation-0.0.2/src/generative_ai/__init__.py` & `query-package-documentation-0.0.3/src/generative_ai/__init__.py`

 * *Files identical despite different names*

### Comparing `query-package-documentation-0.0.2/src/generative_ai/dataset_generation/__init__.py` & `query-package-documentation-0.0.3/src/generative_ai/dataset_generation/__init__.py`

 * *Files identical despite different names*

### Comparing `query-package-documentation-0.0.2/src/generative_ai/dataset_generation/orchestrate_generation.py` & `query-package-documentation-0.0.3/src/generative_ai/dataset_generation/orchestrate_generation.py`

 * *Files identical despite different names*

### Comparing `query-package-documentation-0.0.2/src/generative_ai/dataset_generation/step_1_generation.py` & `query-package-documentation-0.0.3/src/generative_ai/dataset_generation/step_1_generation.py`

 * *Files identical despite different names*

### Comparing `query-package-documentation-0.0.2/src/generative_ai/dataset_generation/step_2_generation.py` & `query-package-documentation-0.0.3/src/generative_ai/dataset_generation/step_2_generation.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 """Define functionalities to generate retrieval and tuning sources."""
 
 import inspect
+import itertools
 import logging
 import random
 
 import pydantic
 
 from .utils_generation import (
     ClassDetails,
     Dataset,
+    Document,
     EnumDetails,
     FunctionDetails,
     MemberDetails,
     MemberType,
     ModuleDetails,
     PackageDetails,
     SplitName,
@@ -23,47 +25,58 @@
 
 LOGGER = logging.getLogger(__name__)
 
 DEFAULT_SPLIT_PROPORTIONS = SplitProportions(
     train_proportion=0.6, validation_proportion=0.2, test_proportion=0.2
 )
 
+EMPTY_PARAMETER = inspect.Parameter.empty
+EMPTY_SIGNATURE = inspect.Signature.empty
+
 
 @pydantic.validate_call(validate_return=True)
-def allocate_tuning_pairs(
-    tuning_pairs: list[tuple[str, str]],
+def allocate_tuning_triplets(
+    context: str,
+    questions: list[str],
+    answers: list[str],
     split_proportions: SplitProportions = DEFAULT_SPLIT_PROPORTIONS,
-) -> list[tuple[str, str, SplitName]]:
-    """Allocate tuning pairs to different splits.
+) -> list[Document]:
+    """Allocate tuning triplets to different splits.
 
     Parameters
     ----------
-    tuning_pairs : list[tuple[str, str]]
-        question and answer pairs to be allocated to different splits
+    context : str
+        source of information
+    questions : list[str]
+        queries from ``context``
+    answers : list[str]
+        responses based on ``context``
     split_proportions : SplitProportions, optional
         chance of a pair to be allocated to different splits, by default DEFAULT_SPLIT_PROPORTIONS
 
     Returns
     -------
-    list[tuple[str, str, SplitName]]
-        updated tuning pairs with split allocation
+    list[Document]
+        updated tuning triplets with split allocation
     """
+    question_answer_pairs = list(itertools.product(questions, answers))
+
     allocations = random.choices(  # noqa: S311
         [SplitName.TRAIN, SplitName.VALIDATION, SplitName.TEST],
         weights=[
             split_proportions.train_proportion,
             split_proportions.validation_proportion,
             split_proportions.test_proportion,
         ],
-        k=len(tuning_pairs),
+        k=len(question_answer_pairs),
     )
 
     return [
-        (question, answer, allocation)
-        for (question, answer), allocation in zip(tuning_pairs, allocations, strict=True)
+        Document(context=context, question=question, answer=answer, split=allocation)
+        for (question, answer), allocation in zip(question_answer_pairs, allocations, strict=True)
     ]
 
 
 @pydantic.validate_call(validate_return=True)
 def enumerate_array_elements(array: list, attribute: str | None = None) -> str:
     """Store all members of ``array``, or a common property of them.
 
@@ -114,518 +127,452 @@
     """
     package_name = package_contents.package_name
     package_full_name = package_contents.package_qualified_name
 
     package = f"'{package_name}' package"
 
     package_retrieval_chunks: list[str] = [f"'{package_name}' is a Python package."]
-    package_tuning_pairs: list[tuple[str, str, SplitName]] = []
+    package_tuning_documents: list[Document] = []
 
     if (parent_package := package_contents.parent_package_name) is None:
-        root_package_pairs = [
-            ("What is the root package?", f"'{package_name}' is the root package."),
-            (
-                "Can you tell me what the root package is?",
-                f"Sure, the root package is '{package_name}'.",
-            ),
-            (
-                "I'm trying to find out the root package. Can you help?",
-                f"Of course, the root package is '{package_name}'.",
-            ),
-            (
-                "Do you know what the root package is?",
-                f"Yes, the root package is '{package_name}'.",
-            ),
-            (
-                "I'd like to know the root package.",
-                f"The root package you're asking about is '{package_name}'.",
-            ),
-            (
-                "Could you identify the root package?",
-                f"Certainly, '{package_name}' is the root package.",
-            ),
-        ]
-        package_retrieval_chunks.append(f"'{package_name}' is the root package.")
-        package_tuning_pairs.extend(allocate_tuning_pairs(root_package_pairs))
-
-        parent_package_pairs = [
-            (
-                f"Name parent package of '{package_name}'.",
-                f"Being the root package, '{package_name}' has no parent package.",
-            ),
-            (
-                f"What is the parent package of '{package_name}'?",
-                f"The root package '{package_name}' does not have a parent package.",
-            ),
-            (
-                f"Can you tell me the parent package of '{package_name}'?",
-                f"'{package_name}' is a root package and therefore,"
-                " it does not have a parent package.",
-            ),
-            (
-                f"Could you identify the parent package of '{package_name}'?",
-                f"As a root package, '{package_name}' does not possess a parent package.",
-            ),
-            (
-                f"I'm looking for the parent package of '{package_name}'. Can you help?",
-                f"Sure, '{package_name}' is a root package, so it doesn't have a parent package.",
-            ),
-            (
-                f"Do you know the parent package of '{package_name}'?",
-                f"Yes, '{package_name}' is a root package and hence,"
-                " it doesn't have a parent package.",
-            ),
-        ]
-        package_retrieval_chunks.append(f"'{package_name}' has no parent package.")
-        package_tuning_pairs.extend(allocate_tuning_pairs(parent_package_pairs))
-    else:
-        parent_package_pairs = [
-            (
-                f"Name parent package of '{package_name}' sub-package.",
-                f"'{parent_package}' is the full name of its parent package.",
-            ),
-            (
-                f"What is the parent package of the '{package_name}' sub-package?",
-                f"The parent package of '{package_name}' is '{parent_package}'.",
-            ),
-            (
-                f"Could you tell me the parent package of '{package_name}'?",
-                f"Sure, the parent package of '{package_name}' is '{parent_package}'.",
-            ),
-            (
-                f"I need to know the parent package of '{package_name}'.",
-                f"The parent package of '{package_name}' is '{parent_package}'.",
-            ),
-            (
-                f"Identify the parent package for the '{package_name}' sub-package.",
-                f"The parent package for '{package_name}' is identified as '{parent_package}'.",
-            ),
-            (
-                f"Can you name the parent package of the '{package_name}' sub-package?",
-                f"Yes, the parent package of '{package_name}' is '{parent_package}'.",
-            ),
-        ]
-        package_retrieval_chunks.append(
-            f"'{package_name}' is part of parent package '{parent_package}'."
-        )
-        package_tuning_pairs.extend(allocate_tuning_pairs(parent_package_pairs))
-
-        package_full_name_pairs = [
-            (
-                f"Tell the full name of '{package_name}' sub-package.",
-                f"'{package_full_name}' is the fully qualified name of '{package_name}'.",
-            ),
-            (
-                f"What is the fully qualified name of the '{package_name}' sub-package?",
-                f"Fully qualified name of '{package_name}' sub-package is '{package_full_name}'.",
-            ),
-            (
-                f"Could you provide the full name of the '{package_name}' sub-package?",
-                f"Sure, the full name of '{package_name}' sub-package is '{package_full_name}'.",
-            ),
-            (
-                f"I need the full name of the '{package_name}' sub-package. Can you tell me?",
-                f"Of course, full name of '{package_name}' sub-package is '{package_full_name}'.",
-            ),
-            (
-                f"Can you inform me about the full name of the '{package_name}' sub-package?",
-                f"Certainly, full name of '{package_name}' sub-package is '{package_full_name}'.",
-            ),
-            (
-                f"Please, reveal the full name of the '{package_name}' sub-package.",
-                f"Absolutely, full name of '{package_name}' sub-package is '{package_full_name}'.",
-            ),
-        ]
-        package_retrieval_chunks.append(
+        root_package_context = f"'{package_name}' is the root package."
+        root_package_questions = [
+            "What is the root package?",
+            "Can you tell me what the root package is?",
+            "I'm trying to find out the root package. Can you help?",
+            "Do you know what the root package is?",
+            "I'd like to know the root package.",
+            "Could you identify the root package?",
+        ]
+        root_package_answers = [
+            f"'{package_name}' is the root package.",
+            f"The root package is '{package_name}'.",
+            f"The root package you're asking about is '{package_name}'.",
+        ]
+
+        package_retrieval_chunks.append(root_package_context)
+        package_tuning_documents.extend(
+            allocate_tuning_triplets(
+                root_package_context, root_package_questions, root_package_answers
+            )
+        )
+
+        parent_package_context = f"'{package_name}' has no parent package."
+        parent_package_questions = [
+            f"Name parent package of '{package_name}'.",
+            f"What is the parent package of '{package_name}'?",
+            f"Can you tell me the parent package of '{package_name}'?",
+            f"Could you identify the parent package of '{package_name}'?",
+            f"I'm looking for the parent package of '{package_name}'. Can you help?",
+            f"Do you know the parent package of '{package_name}'?",
+        ]
+        parent_package_answers = [
+            f"Being the root package, '{package_name}' has no parent package.",
+            f"The root package '{package_name}' does not have a parent package.",
+            f"'{package_name}' is a root package and therefore it does not have a parent package.",
+            f"As a root package, '{package_name}' does not possess a parent package.",
+            f"'{package_name}' is a root package, so it doesn't have a parent package.",
+            f"'{package_name}' is a root package and hence it doesn't have a parent package.",
+        ]
+
+        package_retrieval_chunks.append(parent_package_context)
+        package_tuning_documents.extend(
+            allocate_tuning_triplets(
+                parent_package_context, parent_package_questions, parent_package_answers
+            )
+        )
+    else:
+        parent_package_context = f"'{package_name}' is part of parent package '{parent_package}'."
+        parent_package_questions = [
+            f"Name parent package of '{package_name}' sub-package.",
+            f"What is the parent package of the '{package_name}' sub-package?",
+            f"Could you tell me the parent package of '{package_name}'?",
+            f"I need to know the parent package of '{package_name}'.",
+            f"Identify the parent package for the '{package_name}' sub-package.",
+            f"Can you name the parent package of the '{package_name}' sub-package?",
+        ]
+        parent_package_answers = [
+            f"'{parent_package}' is the full name of its parent package.",
+            f"The parent package of '{package_name}' is '{parent_package}'.",
+            f"The parent package for '{package_name}' is identified as '{parent_package}'.",
+        ]
+
+        package_retrieval_chunks.append(parent_package_context)
+        package_tuning_documents.extend(
+            allocate_tuning_triplets(
+                parent_package_context, parent_package_questions, parent_package_answers
+            )
+        )
+
+        package_full_name_context = (
             f"Full name of '{package_name}' sub-package is '{package_full_name}'."
         )
-        package_tuning_pairs.extend(allocate_tuning_pairs(package_full_name_pairs))
+        package_full_name_questions = [
+            f"Tell the full name of '{package_name}' sub-package.",
+            f"What is the fully qualified name of the '{package_name}' sub-package?",
+            f"Could you provide the full name of the '{package_name}' sub-package?",
+            f"I need the full name of the '{package_name}' sub-package. Can you tell me?",
+            f"Can you inform me about the full name of the '{package_name}' sub-package?",
+            f"Please, reveal the full name of the '{package_name}' sub-package.",
+        ]
+        package_full_name_answers = [
+            f"'{package_full_name}' is the fully qualified name of '{package_name}'.",
+            f"Fully qualified name of '{package_name}' sub-package is '{package_full_name}'.",
+            f"The full name of '{package_name}' sub-package is '{package_full_name}'.",
+        ]
+
+        package_retrieval_chunks.append(package_full_name_context)
+        package_tuning_documents.extend(
+            allocate_tuning_triplets(
+                package_full_name_context, package_full_name_questions, package_full_name_answers
+            )
+        )
 
         package_hierarchy = enumerate_array_elements(package_contents.package_hierarchy)
-        package_hierarchy_pairs = [
-            (
-                f"What is the hierarchy of {package}?",
-                f"The hierarchy of {package} is as follows: {package_hierarchy}.",
-            ),
-            (
-                f"Can you explain the hierarchy of the {package}?",
-                f"Sure, the hierarchy of the {package} is: {package_hierarchy}.",
-            ),
-            (
-                f"Could you describe the structure of the {package}?",
-                f"Of course, the structure of {package} is: {package_hierarchy}.",
-            ),
-            (
-                f"I need to understand the hierarchy of {package}. Can you help?",
-                f"Absolutely, the hierarchy of {package} is: {package_hierarchy}.",
-            ),
-            (
-                f"Please provide the hierarchy of the {package}.",
-                f"The hierarchy of the {package} is: {package_hierarchy}.",
-            ),
-            (
-                f"I'm interested in the structure of the {package}. What is it?",
-                f"The structure of {package} is as follows: {package_hierarchy}.",
-            ),
-        ]
-        package_retrieval_chunks.append(
-            f"Hierarchy of {package} is as follows: {package_hierarchy}."
+
+        package_hierarchy_context = f"Hierarchy of {package} is as follows: {package_hierarchy}."
+        package_hierarchy_questions = [
+            f"What is the hierarchy of {package}?",
+            f"Can you explain the hierarchy of the {package}?",
+            f"Could you describe the structure of the {package}?",
+            f"I need to understand the hierarchy of {package}. Can you help?",
+            f"Please provide the hierarchy of the {package}.",
+            f"I'm interested in the structure of the {package}. What is it?",
+        ]
+        package_hierarchy_answers = [
+            f"The hierarchy of {package} is as follows: {package_hierarchy}.",
+            f"The hierarchy of {package} is: {package_hierarchy}.",
+            f"The structure of {package} is: {package_hierarchy}.",
+            f"The structure of {package} is as follows: {package_hierarchy}.",
+        ]
+
+        package_retrieval_chunks.append(package_hierarchy_context)
+        package_tuning_documents.extend(
+            allocate_tuning_triplets(
+                package_hierarchy_context, package_hierarchy_questions, package_hierarchy_answers
+            )
         )
-        package_tuning_pairs.extend(allocate_tuning_pairs(package_hierarchy_pairs))
 
     if not (children_sub_packages := package_contents.children_sub_packages_names):
-        package_sub_package_pairs = [
-            (
-                f"List the sub-packages of {package}.",
-                f"{package} does not have any further sub-packages.",
-            ),
-            (
-                f"What are the sub-packages of the {package}?",
-                f"The {package} does not contain any sub-packages.",
-            ),
-            (
-                f"Could you tell me the sub-packages of {package}?",
-                f"I'm sorry, but the {package} doesn't have any sub-packages.",
-            ),
-            (
-                f"I need to know the sub-packages of {package}. Can you list them?",
-                f"Unfortunately, {package} doesn't include any sub-packages.",
-            ),
-            (
-                f"Can you provide a list of sub-packages for the {package}?",
-                f"There are no sub-packages in the {package}.",
-            ),
-            (
-                f"Identify the sub-packages of {package}.",
-                f"No sub-packages are present in the {package}.",
-            ),
-        ]
-        package_retrieval_chunks.append(f"{package} does not have any further sub-packages.")
-        package_tuning_pairs.extend(allocate_tuning_pairs(package_sub_package_pairs))
+        package_sub_package_context = f"{package} does not have any further sub-packages."
+        package_sub_package_questions = [
+            f"List the sub-packages of {package}.",
+            f"What are the sub-packages of the {package}?",
+            f"Could you tell me the sub-packages of {package}?",
+            f"I need to know the sub-packages of {package}. Can you list them?",
+            f"Can you provide a list of sub-packages for the {package}?",
+            f"Identify the sub-packages of {package}.",
+        ]
+        package_sub_package_answers = [
+            f"{package} does not have any further sub-packages.",
+            f"The {package} does not contain any sub-packages.",
+            f"The {package} doesn't have any sub-packages.",
+            f"{package} doesn't include any sub-packages.",
+            f"There are no sub-packages in the {package}.",
+            f"No sub-packages are present in the {package}.",
+        ]
+
+        package_retrieval_chunks.append(package_sub_package_context)
+        package_tuning_documents.extend(
+            allocate_tuning_triplets(
+                package_sub_package_context,
+                package_sub_package_questions,
+                package_sub_package_answers,
+            )
+        )
     else:
         children_sub_packages_count = len(children_sub_packages)
-        children_sub_packages_count_pairs = [
-            (
-                f"How many sub-packages are there in {package}?",
-                f"{package} has {children_sub_packages_count} many sub-packages.",
-            ),
-            (
-                f"What is the count of sub-packages in {package}?",
-                f"The count of sub-packages in {package} is {children_sub_packages_count}.",
-            ),
-            (
-                f"Could you tell me the number of sub-packages available in {package}?",
-                f"{package} has {children_sub_packages_count} sub-packages.",
-            ),
-            (
-                f"Please provide the count of sub-packages for {package}.",
-                f"Number of sub-packages in {package} is {children_sub_packages_count}.",
-            ),
-            (
-                f"Tell me the quantity of sub-packages present in {package}.",
-                f"{package} has {children_sub_packages_count} sub-packages.",
-            ),
-            (
-                f"Would you mind letting me know how many sub-packages {package} contains?",
-                f"{package} contains {children_sub_packages_count} sub-packages.",
-            ),
-        ]
-        package_retrieval_chunks.append(
+
+        children_sub_packages_count_context = (
             f"{package} has {children_sub_packages_count} many sub-packages."
         )
-        package_tuning_pairs.extend(allocate_tuning_pairs(children_sub_packages_count_pairs))
+        children_sub_packages_count_questions = [
+            f"How many sub-packages are there in {package}?",
+            f"What is the count of sub-packages in {package}?",
+            f"Could you tell me the number of sub-packages available in {package}?",
+            f"Please provide the count of sub-packages for {package}.",
+            f"Tell me the quantity of sub-packages present in {package}.",
+            f"Would you mind letting me know how many sub-packages {package} contains?",
+        ]
+        children_sub_packages_count_answers = [
+            f"{package} has {children_sub_packages_count} many sub-packages.",
+            f"The count of sub-packages in {package} is {children_sub_packages_count}.",
+            f"{package} has {children_sub_packages_count} sub-packages.",
+            f"Number of sub-packages in {package} is {children_sub_packages_count}.",
+            f"{package} has {children_sub_packages_count} sub-packages.",
+            f"{package} contains {children_sub_packages_count} sub-packages.",
+        ]
+
+        package_retrieval_chunks.append(children_sub_packages_count_context)
+        package_tuning_documents.extend(
+            allocate_tuning_triplets(
+                children_sub_packages_count_context,
+                children_sub_packages_count_questions,
+                children_sub_packages_count_answers,
+            )
+        )
 
         package_sub_packages = enumerate_array_elements(children_sub_packages)
-        package_sub_package_pairs = [
-            (
-                f"List the sub-packages of {package}.",
-                f"Sub-packages of {package} are as follows: {package_sub_packages}.",
-            ),
-            (
-                f"What are the sub-packages of the {package}?",
-                f"The {package} has the following sub-packages: {package_sub_packages}.",
-            ),
-            (
-                f"Could you tell me the sub-packages of {package}?",
-                f"Sure, the sub-packages of {package} are: {package_sub_packages}.",
-            ),
-            (
-                f"I need to know the sub-packages of {package}. Can you list them?",
-                f"Of course, the sub-packages of {package} are: {package_sub_packages}.",
-            ),
-            (
-                f"Please provide the sub-packages of {package}.",
-                f"The sub-packages of {package} are: {package_sub_packages}.",
-            ),
-            (
-                f"Can you enumerate the sub-packages of {package}?",
-                f"Certainly, the sub-packages of {package} are: {package_sub_packages}.",
-            ),
-        ]
-        package_retrieval_chunks.append(
+
+        package_sub_package_context = (
             f"Sub-packages of {package} are as follows: {package_sub_packages}."
         )
-        package_tuning_pairs.extend(allocate_tuning_pairs(package_sub_package_pairs))
+        package_sub_package_questions = [
+            f"List the sub-packages of {package}.",
+            f"What are the sub-packages of the {package}?",
+            f"Could you tell me the sub-packages of {package}?",
+            f"I need to know the sub-packages of {package}. Can you list them?",
+            f"Please provide the sub-packages of {package}.",
+            f"Can you enumerate the sub-packages of {package}?",
+        ]
+        package_sub_package_answers = [
+            f"Sub-packages of {package} are as follows: {package_sub_packages}.",
+            f"The {package} has the following sub-packages: {package_sub_packages}.",
+            f"The sub-packages of {package} are: {package_sub_packages}.",
+        ]
+
+        package_retrieval_chunks.append(package_sub_package_context)
+        package_tuning_documents.extend(
+            allocate_tuning_triplets(
+                package_sub_package_context,
+                package_sub_package_questions,
+                package_sub_package_answers,
+            )
+        )
 
     if not (children_modules := package_contents.children_modules_names):
-        package_module_pairs = [
-            (
-                f"What are the modules of {package}?",
-                f"{package} does not have any direct modules under itself.",
-            ),
-            (
-                f"Can you list the modules under the {package}?",
-                f"There are no direct modules under the {package}.",
-            ),
-            (
-                f"Does the {package} contain any modules?",
-                f"No, the {package} does not contain any direct modules.",
-            ),
-            (
-                f"I'm looking for the modules of {package}. Can you help?",
-                f"I'm sorry, but {package} does not have any direct modules.",
-            ),
-            (
-                f"Tell me about the modules of {package}.",
-                f"Actually, the {package} does not have any direct modules.",
-            ),
-            (
-                f"Are there any modules under the {package}?",
-                f"No, there aren't any direct modules under the {package}.",
-            ),
-        ]
-        package_retrieval_chunks.append(f"{package} does not have any further modules.")
-        package_tuning_pairs.extend(allocate_tuning_pairs(package_module_pairs))
+        package_module_context = f"{package} does not have any further modules."
+        package_module_questions = [
+            f"What are the modules of {package}?",
+            f"Can you list the modules under the {package}?",
+            f"Does the {package} contain any modules?",
+            f"I'm looking for the modules of {package}. Can you help?",
+            f"Tell me about the modules of {package}.",
+            f"Are there any modules under the {package}?",
+        ]
+        package_module_answers = [
+            f"{package} does not have any direct modules under itself.",
+            f"There are no direct modules under the {package}.",
+            f"No, the {package} does not contain any direct modules.",
+            f"{package} does not have any direct modules.",
+            f"The {package} does not have any direct modules.",
+            f"There aren't any direct modules under the {package}.",
+        ]
+
+        package_retrieval_chunks.append(package_module_context)
+        package_tuning_documents.extend(
+            allocate_tuning_triplets(
+                package_module_context, package_module_questions, package_module_answers
+            )
+        )
     else:
         children_modules_count = len(children_modules)
-        children_modules_count_pairs = [
-            (
-                f"How many modules are there in {package}?",
-                f"{package} has {children_modules_count} many modules.",
-            ),
-            (
-                f"What is the count of modules in {package}?",
-                f"The count of modules in {package} is {children_modules_count}.",
-            ),
-            (
-                f"Could you tell me the number of modules available in {package}?",
-                f"{package} has {children_modules_count} modules.",
-            ),
-            (
-                f"Please provide the count of modules for {package}.",
-                f"The number of modules in {package} is {children_modules_count}.",
-            ),
-            (
-                f"Tell me the quantity of modules present in {package}.",
-                f"{package} has {children_modules_count} modules.",
-            ),
-            (
-                f"Would you mind letting me know how many modules {package} contains?",
-                f"{package} contains {children_modules_count} modules.",
-            ),
-        ]
-        package_retrieval_chunks.append(f"{package} has {children_modules_count} many modules.")
-        package_tuning_pairs.extend(allocate_tuning_pairs(children_modules_count_pairs))
+
+        children_modules_count_context = f"{package} has {children_modules_count} many modules."
+        children_modules_count_questions = [
+            f"How many modules are there in {package}?",
+            f"What is the count of modules in {package}?",
+            f"Could you tell me the number of modules available in {package}?",
+            f"Please provide the count of modules for {package}.",
+            f"Tell me the quantity of modules present in {package}.",
+            f"Would you mind letting me know how many modules {package} contains?",
+        ]
+        children_modules_count_answers = [
+            f"{package} has {children_modules_count} many modules.",
+            f"The count of modules in {package} is {children_modules_count}.",
+            f"{package} has {children_modules_count} modules.",
+            f"The number of modules in {package} is {children_modules_count}.",
+            f"{package} contains {children_modules_count} modules.",
+        ]
+
+        package_retrieval_chunks.append(children_modules_count_context)
+        package_tuning_documents.extend(
+            allocate_tuning_triplets(
+                children_modules_count_context,
+                children_modules_count_questions,
+                children_modules_count_answers,
+            )
+        )
 
         package_modules = enumerate_array_elements(children_modules)
-        package_module_pairs = [
-            (
-                f"What are the modules of {package}?",
-                f"Direct modules under {package} are as follows: {package_modules}.",
-            ),
-            (
-                f"Can you list the modules of the {package}?",
-                f"Sure, the direct modules under {package} are: {package_modules}.",
-            ),
-            (
-                f"I need to know the modules of the {package}.",
-                f"The modules you're looking for in {package} are: {package_modules}.",
-            ),
-            (
-                f"Could you tell me what the modules of the {package} are?",
-                f"Of course, the modules under {package} are: {package_modules}.",
-            ),
-            (
-                f"I'm interested in the modules of the {package}.",
-                f"The modules in {package} are: {package_modules}.",
-            ),
-            (
-                f"What modules does the {package} contain?",
-                f"The {package} contains these modules: {package_modules}.",
-            ),
-        ]
-        package_retrieval_chunks.append(f"Modules of {package} are as follows: {package_modules}.")
-        package_tuning_pairs.extend(allocate_tuning_pairs(package_module_pairs))
+
+        package_module_context = f"Modules of {package} are as follows: {package_modules}."
+        package_module_questions = [
+            f"What are the modules of {package}?",
+            f"Can you list the modules of the {package}?",
+            f"I need to know the modules of the {package}.",
+            f"Could you tell me what the modules of the {package} are?",
+            f"I'm interested in the modules of the {package}.",
+            f"What modules does the {package} contain?",
+        ]
+        package_module_answers = [
+            f"Direct modules under {package} are as follows: {package_modules}.",
+            f"The direct modules under {package} are: {package_modules}.",
+            f"The modules you're looking for in {package} are: {package_modules}.",
+            f"The modules under {package} are: {package_modules}.",
+            f"The modules in {package} are: {package_modules}.",
+            f"The {package} contains these modules: {package_modules}.",
+        ]
+
+        package_retrieval_chunks.append(package_module_context)
+        package_tuning_documents.extend(
+            allocate_tuning_triplets(
+                package_module_context, package_module_questions, package_module_answers
+            )
+        )
 
     if not (package_summary := package_contents.package_summary):
-        package_summary_pairs = [
-            (f"What does {package} do?", f"{package} does not have any documentation."),
-            (
-                f"Can you tell me the functionality of the {package}?",
-                f"Unfortunately, the {package} provides no documentation.",
-            ),
-            (
-                f"I'm curious about what the {package} does. Can you enlighten me?",
-                f"I'm sorry, but the {package} does not come with any documentation.",
-            ),
-            (
-                f"Could you explain the purpose of the {package}?",
-                f"Regrettably, the {package} lacks any form of documentation.",
-            ),
-            (
-                f"What's the role of the {package}?",
-                f"The {package} does not offer any documentation.",
-            ),
-            (
-                f"What functionality does the {package} provide?",
-                f"The {package} does not have any available documentation.",
-            ),
-        ]
-        package_retrieval_chunks.append(
+        package_summary_context = (
             f"Unfortunately, {package} currently does not have any documentation."
         )
-        package_tuning_pairs.extend(allocate_tuning_pairs(package_summary_pairs))
+        package_summary_questions = [
+            f"What does {package} do?",
+            f"Can you tell me the functionality of the {package}?",
+            f"I'm curious about what the {package} does. Can you enlighten me?",
+            f"Could you explain the purpose of the {package}?",
+            f"What's the role of the {package}?",
+            f"What functionality does the {package} provide?",
+        ]
+        package_summary_answers = [
+            f"{package} does not have any documentation.",
+            f"The {package} provides no documentation.",
+            f"The {package} does not come with any documentation.",
+            f"The {package} lacks any form of documentation.",
+            f"The {package} does not offer any documentation.",
+            f"The {package} does not have any available documentation.",
+        ]
+
+        package_retrieval_chunks.append(package_summary_context)
+        package_tuning_documents.extend(
+            allocate_tuning_triplets(
+                package_summary_context, package_summary_questions, package_summary_answers
+            )
+        )
     else:
-        package_summary_pairs = [
-            (f"What does {package} do?", f"Its documentation is as follows: '{package_summary}'."),
-            (
-                f"Can you tell me about the {package}?",
-                f"Sure, here is its documentation: '{package_summary}'.",
-            ),
-            (
-                f"I'd like to know what the {package} does.",
-                f"Of course, here's the documentation for it: '{package_summary}'.",
-            ),
-            (
-                f"Could you explain the functionality of the {package}?",
-                f"Absolutely, the documentation states: '{package_summary}'.",
-            ),
-            (
-                f"What's the purpose of the {package}?",
-                f"The purpose is described in its documentation: '{package_summary}'.",
-            ),
-            (
-                f"I'm curious about the {package}, what does it do?",
-                f"Good question, its documentation reads: '{package_summary}'.",
-            ),
-        ]
-        package_retrieval_chunks.append(
+        package_summary_context = (
             f"The following is the documentation of {package}: '{package_summary}'."
         )
-        package_tuning_pairs.extend(allocate_tuning_pairs(package_summary_pairs))
+        package_summary_questions = [
+            f"What does {package} do?",
+            f"Can you tell me about the {package}?",
+            f"I'd like to know what the {package} does.",
+            f"Could you explain the functionality of the {package}?",
+            f"What's the purpose of the {package}?",
+            f"I'm curious about the {package}, what does it do?",
+        ]
+        package_summary_answers = [
+            f"Its documentation is as follows: '{package_summary}'.",
+            f"Here is its documentation: '{package_summary}'.",
+            f"Here's the documentation for it: '{package_summary}'.",
+            f"The documentation states: '{package_summary}'.",
+            f"The purpose is described in its documentation: '{package_summary}'.",
+            f"Its documentation reads: '{package_summary}'.",
+        ]
+
+        package_retrieval_chunks.append(package_summary_context)
+        package_tuning_documents.extend(
+            allocate_tuning_triplets(
+                package_summary_context, package_summary_questions, package_summary_answers
+            )
+        )
 
     if not (package_exports := package_contents.package_all_exports):
-        package_members_pairs = [
-            (
-                f"What are the public members of the {package}?",
-                f"{package} does not have any public member exported through '__all__'.",
-            ),
-            (
-                f"Can you list the public members of the {package}?",
-                f"The {package} does not export any public members through '__all__'.",
-            ),
-            (
-                f"Are there any public members in the {package}?",
-                f"No, the {package} does not have any public members exported through '__all__'.",
-            ),
-            (
-                f"I'm looking for public members of {package}. Can you help?",
-                f"Sure, but the {package} does not export any public members through '__all__'.",
-            ),
-            (
-                f"Could you tell me the public members of the {package}?",
-                f"Unfortunately, the {package} does not have any public members"
-                " exported through '__all__'.",
-            ),
-            (
-                f"I'd like to know the public members of the {package}."
-                " Can you provide that information?",
-                f"I'm sorry, but the {package} does not have any public members"
-                " exported through '__all__'.",
-            ),
-        ]
-        package_retrieval_chunks.append(
+        package_members_context = (
             f"{package} does not export anything publicly using __all__ variable."
         )
-        package_tuning_pairs.extend(allocate_tuning_pairs(package_members_pairs))
+        package_members_questions = [
+            f"What are the public members of the {package}?",
+            f"Can you list the public members of the {package}?",
+            f"Are there any public members in the {package}?",
+            f"I'm looking for public members of {package}. Can you help?",
+            f"Could you tell me the public members of the {package}?",
+            f"I'd like to know the public members of the {package}."
+            " Can you provide that information?",
+        ]
+        package_members_answers = [
+            f"{package} does not have any public member exported through '__all__'.",
+            f"The {package} does not export any public members through '__all__'.",
+            f"The {package} does not have any public members exported through '__all__'.",
+        ]
+
+        package_retrieval_chunks.append(package_members_context)
+        package_tuning_documents.extend(
+            allocate_tuning_triplets(
+                package_members_context, package_members_questions, package_members_answers
+            )
+        )
     else:
         package_exports_count = len(package_exports)
-        package_exports_count_pairs = [
-            (
-                f"How many objects does {package} export publicly?",
-                f"{package} exports {package_exports_count} many objects using __all__.",
-            ),
-            (
-                f"What is the count of publicly exported objects in {package}?",
-                f"Count of publicly exported objects in {package} is {package_exports_count}.",
-            ),
-            (
-                f"Could you tell me the number of objects publicly exported by {package}?",
-                f"{package} exports {package_exports_count} objects using __all__.",
-            ),
-            (
-                f"Please provide the count of objects publicly exported by {package}.",
-                f"Number of objects publicly exported by {package} is {package_exports_count}.",
-            ),
-            (
-                f"Tell me the quantity of objects that {package} exports publicly.",
-                f"{package} exports {package_exports_count} objects using __all__.",
-            ),
-            (
-                f"Would you mind letting me know how many objects {package} publicly exports?",
-                f"{package} publicly exports {package_exports_count} objects.",
-            ),
-        ]
-        package_retrieval_chunks.append(
+
+        package_exports_count_context = (
             f"{package} has {package_exports_count} many public exports."
         )
-        package_tuning_pairs.extend(allocate_tuning_pairs(package_exports_count_pairs))
+        package_exports_count_questions = [
+            f"How many objects does {package} export publicly?",
+            f"What is the count of publicly exported objects in {package}?",
+            f"Could you tell me the number of objects publicly exported by {package}?",
+            f"Please provide the count of objects publicly exported by {package}.",
+            f"Tell me the quantity of objects that {package} exports publicly.",
+            f"Would you mind letting me know how many objects {package} publicly exports?",
+        ]
+        package_exports_count_answers = [
+            f"{package} exports {package_exports_count} many objects using __all__.",
+            f"Count of publicly exported objects in {package} is {package_exports_count}.",
+            f"{package} exports {package_exports_count} objects using __all__.",
+            f"Number of objects publicly exported by {package} is {package_exports_count}.",
+            f"{package} exports {package_exports_count} objects using __all__.",
+            f"{package} publicly exports {package_exports_count} objects.",
+        ]
+
+        package_retrieval_chunks.append(package_exports_count_context)
+        package_tuning_documents.extend(
+            allocate_tuning_triplets(
+                package_exports_count_context,
+                package_exports_count_questions,
+                package_exports_count_answers,
+            )
+        )
 
         package_public_members = enumerate_array_elements(package_exports)
-        package_members_pairs = [
-            (
-                f"What are the public members of the {package}?",
-                f"{package} publicly exports the following members using '__all__':"
-                f" {package_public_members}.",
-            ),
-            (
-                f"Can you list the public members of the {package}?",
-                f"Sure, the {package} publicly exports these members using '__all__':"
-                f" {package_public_members}.",
-            ),
-            (
-                f"I need to know the public members of the {package}. Can you tell me?",
-                f"Of course, the {package} publicly exports these members using '__all__':"
-                f" {package_public_members}.",
-            ),
-            (
-                f"Could you tell me what the {package} publicly exports?",
-                f"The {package} publicly exports the following members using '__all__':"
-                f" {package_public_members}.",
-            ),
-            (
-                f"I'm interested in the public members of the {package}. What are they?",
-                f"The {package} publicly exports these members using '__all__':"
-                f" {package_public_members}.",
-            ),
-        ]
-        package_retrieval_chunks.append(
+
+        package_members_context = (
             f"{package} exports following public members using __all__: {package_public_members}."
         )
-        package_tuning_pairs.extend(allocate_tuning_pairs(package_members_pairs))
+        package_members_questions = [
+            f"What are the public members of the {package}?",
+            f"Can you list the public members of the {package}?",
+            f"I need to know the public members of the {package}. Can you tell me?",
+            f"Could you tell me what the {package} publicly exports?",
+            f"I'm interested in the public members of the {package}. What are they?",
+        ]
+        package_members_answers = [
+            f"{package} publicly exports the following members using '__all__':"
+            f" {package_public_members}.",
+            f"The {package} publicly exports the following members using '__all__':"
+            f" {package_public_members}.",
+            f"The {package} publicly exports these members using '__all__':"
+            f" {package_public_members}.",
+        ]
+
+        package_retrieval_chunks.append(package_members_context)
+        package_tuning_documents.extend(
+            allocate_tuning_triplets(
+                package_members_context, package_members_questions, package_members_answers
+            )
+        )
 
     package_dataset = Dataset(
-        retrieval_chunks=package_retrieval_chunks, tuning_pairs=package_tuning_pairs
+        retrieval_chunks=package_retrieval_chunks, tuning_documents=package_tuning_documents
     )
 
     return package_dataset
 
 
 @pydantic.validate_call(validate_return=True)
-def generate_module_dataset(module_contents: ModuleDetails) -> Dataset:
+def generate_module_dataset(module_contents: ModuleDetails) -> Dataset:  # noqa: PLR0915
     """Create relevant question and answers based on module details.
 
     Parameters
     ----------
     module_contents : ModuleDetails
         details of a python module
 
@@ -635,318 +582,289 @@
         all documents for retrieval and tuning for querying module documentation
     """
     module_name = module_contents.module_name
     module_full_name = module_contents.module_qualified_name
     module = f"'{module_name}' module"
 
     module_retrieval_chunks: list[str] = [f"'{module_name}' is a Python module."]
-    module_tuning_pairs: list[tuple[str, str, SplitName]] = []
+    module_tuning_documents: list[Document] = []
 
-    module_package_pairs = [
-        (
-            f"Can you tell the the parent package of {module}?",
-            f"'{module_contents.package_name}' is the parent package of {module}.",
-        ),
-        (
-            f"What is the parent package of the {module}?",
-            f"The parent package of {module} is '{module_contents.package_name}'.",
-        ),
-        (
-            f"I'm trying to find the parent package of the {module}. Can you help?",
-            f"Sure, parent package of {module} is '{module_contents.package_name}'.",
-        ),
-        (
-            f"Could you inform me about the parent package of the {module}?",
-            f"Certainly, '{module_contents.package_name}' is the parent package of the {module}.",
-        ),
-        (
-            f"I need to know the parent package of {module}. Can you provide that information?",
-            f"Absolutely, the parent package of the {module} is '{module_contents.package_name}'.",
-        ),
-        (
-            f"Can you identify the parent package for the {module}?",
-            f"Yes, parent package for {module} is '{module_contents.package_name}'.",
-        ),
-    ]
-    module_retrieval_chunks.append(
+    module_package_context = (
         f"{module} is part of parent package '{module_contents.package_name}'."
     )
-    module_tuning_pairs.extend(allocate_tuning_pairs(module_package_pairs))
+    module_package_questions = [
+        f"Can you tell the the parent package of {module}?",
+        f"What is the parent package of the {module}?",
+        f"I'm trying to find the parent package of the {module}. Can you help?",
+        f"Could you inform me about the parent package of the {module}?",
+        f"I need to know the parent package of {module}. Can you provide that information?",
+        f"Can you identify the parent package for the {module}?",
+    ]
+    module_package_answers = [
+        f"'{module_contents.package_name}' is the parent package of {module}.",
+        f"The parent package of {module} is '{module_contents.package_name}'.",
+        f"Parent package of {module} is '{module_contents.package_name}'.",
+        f"'{module_contents.package_name}' is the parent package of the {module}.",
+        f"The parent package of the {module} is '{module_contents.package_name}'.",
+        f"Parent package for {module} is '{module_contents.package_name}'.",
+    ]
+
+    module_retrieval_chunks.append(module_package_context)
+    module_tuning_documents.extend(
+        allocate_tuning_triplets(
+            module_package_context, module_package_questions, module_package_answers
+        )
+    )
 
-    module_full_name_pairs = [
-        (
-            f"Specify the full name of {module}?",
-            f"'{module_full_name}' is fully qualified name for {module}.",
-        ),
-        (
-            f"What is the fully qualified name for the {module}?",
-            f"The fully qualified name for the {module} is '{module_full_name}'.",
-        ),
-        (
-            f"Could you tell me the full name of the {module}?",
-            f"Sure, the full name of the {module} is '{module_full_name}'.",
-        ),
-        (
-            f"I need the full name of the {module}. Can you provide it?",
-            f"Of course, the full name of the {module} is '{module_full_name}'.",
-        ),
-        (
-            f"Can you specify the fully qualified name of the {module}?",
-            f"Yes, fully qualified name of the {module} is '{module_full_name}'.",
-        ),
-        (
-            f"I'm looking for the full name of the {module}. What is it?",
-            f"Full name of the {module} you're looking for is '{module_full_name}'.",
-        ),
+    module_full_name_context = f"Full name of {module} is '{module_full_name}'."
+    module_full_name_questions = [
+        f"Specify the full name of {module}?",
+        f"What is the fully qualified name for the {module}?",
+        f"Could you tell me the full name of the {module}?",
+        f"I need the full name of the {module}. Can you provide it?",
+        f"Can you specify the fully qualified name of the {module}?",
+        f"I'm looking for the full name of the {module}. What is it?",
+    ]
+    module_full_name_answers = [
+        f"'{module_full_name}' is fully qualified name for {module}.",
+        f"The fully qualified name for the {module} is '{module_full_name}'.",
+        f"The full name of the {module} is '{module_full_name}'.",
+        f"Fully qualified name of the {module} is '{module_full_name}'.",
+        f"Full name of the {module} you're looking for is '{module_full_name}'.",
     ]
-    module_retrieval_chunks.append(f"Full name of {module} is '{module_full_name}'.")
-    module_tuning_pairs.extend(allocate_tuning_pairs(module_full_name_pairs))
+
+    module_retrieval_chunks.append(module_full_name_context)
+    module_tuning_documents.extend(
+        allocate_tuning_triplets(
+            module_full_name_context, module_full_name_questions, module_full_name_answers
+        )
+    )
 
     module_hierarchy = enumerate_array_elements(module_contents.module_hierarchy)
-    module_hierarchy_pairs = [
-        (
-            f"What is the hierarchy of {module}?",
-            f"The hierarchy of {module} is as follows: {module_hierarchy}.",
-        ),
-        (
-            f"Can you explain the hierarchy of the {module}?",
-            f"Sure, the hierarchy of the {module} is: {module_hierarchy}.",
-        ),
-        (
-            f"Could you describe the structure of the {module}?",
-            f"Of course, the structure of the {module} is: {module_hierarchy}.",
-        ),
-        (
-            f"I need to understand the hierarchy of the {module}. Can you help?",
-            f"Absolutely, the hierarchy of the {module} is: {module_hierarchy}.",
-        ),
-        (
-            f"Please provide the hierarchy of the {module}.",
-            f"The hierarchy of the {module} is: {module_hierarchy}.",
-        ),
-        (
-            f"What does the hierarchy of the {module} look like?",
-            f"The hierarchy of the {module} looks like this: {module_hierarchy}.",
-        ),
+
+    module_hierarchy_context = f"Hierarchy of {module} is as follows: {module_hierarchy}."
+    module_hierarchy_questions = [
+        f"What is the hierarchy of {module}?",
+        f"Can you explain the hierarchy of the {module}?",
+        f"Could you describe the structure of the {module}?",
+        f"I need to understand the hierarchy of the {module}. Can you help?",
+        f"Please provide the hierarchy of the {module}.",
+        f"What does the hierarchy of the {module} look like?",
+    ]
+    module_hierarchy_answers = [
+        f"The hierarchy of {module} is as follows: {module_hierarchy}.",
+        f"The hierarchy of the {module} is: {module_hierarchy}.",
+        f"The structure of the {module} is: {module_hierarchy}.",
+        f"The hierarchy of the {module} looks like this: {module_hierarchy}.",
     ]
-    module_retrieval_chunks.append(f"Hierarchy of {module} is as follows: {module_hierarchy}.")
-    module_tuning_pairs.extend(allocate_tuning_pairs(module_hierarchy_pairs))
+
+    module_retrieval_chunks.append(module_hierarchy_context)
+    module_tuning_documents.extend(
+        allocate_tuning_triplets(
+            module_hierarchy_context, module_hierarchy_questions, module_hierarchy_answers
+        )
+    )
 
     module_members_count = len(module_contents.module_members)
-    module_members_count_pairs = [
-        (
-            f"How many members does {module} have?",
-            f"{module} has {module_members_count} many members.",
-        ),
-        (
-            f"What is the count of members in {module}?",
-            f"The count of members in {module} is {module_members_count}.",
-        ),
-        (
-            f"Could you tell me the number of members in {module}?",
-            f"{module} has {module_members_count} members.",
-        ),
-        (
-            f"Please provide the count of members for {module}.",
-            f"The number of members in {module} is {module_members_count}.",
-        ),
-        (
-            f"Tell me the quantity of members present in {module}.",
-            f"{module} has {module_members_count} members.",
-        ),
-        (
-            f"Would you mind letting me know how many members {module} contains?",
-            f"{module} contains {module_members_count} members.",
-        ),
+
+    module_members_count_context = f"{module} has {module_members_count} many members."
+    module_members_count_questions = [
+        f"How many members does {module} have?",
+        f"What is the count of members in {module}?",
+        f"Could you tell me the number of members in {module}?",
+        f"Please provide the count of members for {module}.",
+        f"Tell me the quantity of members present in {module}.",
+        f"Would you mind letting me know how many members {module} contains?",
+    ]
+    module_members_count_answers = [
+        f"{module} has {module_members_count} many members.",
+        f"The count of members in {module} is {module_members_count}.",
+        f"{module} has {module_members_count} members.",
+        f"The number of members in {module} is {module_members_count}.",
+        f"{module} contains {module_members_count} members.",
     ]
-    module_retrieval_chunks.append(f"{module} has {module_members_count} many members.")
-    module_tuning_pairs.extend(allocate_tuning_pairs(module_members_count_pairs))
+
+    module_retrieval_chunks.append(module_members_count_context)
+    module_tuning_documents.extend(
+        allocate_tuning_triplets(
+            module_members_count_context,
+            module_members_count_questions,
+            module_members_count_answers,
+        )
+    )
 
     module_member_names = enumerate_array_elements(
         module_contents.module_members, attribute="member_name"
     )
-    module_members_pairs = [
-        (
-            f"List the members of {module}.",
-            f"Members of {module} are as follows: {module_member_names}.",
-        ),
-        (
-            f"What are the members of the {module}?",
-            f"The {module} has the following members: {module_member_names}.",
-        ),
-        (
-            f"Can you tell me the members of the {module}?",
-            f"Sure, the members of the {module} are: {module_member_names}.",
-        ),
-        (
-            f"I need to know the members of the {module}.",
-            f"Members of {module} you asked for are: {module_member_names}.",
-        ),
-        (
-            f"Could you list the members of the {module}?",
-            f"Of course, members of the {module} are: {module_member_names}.",
-        ),
-        (
-            f"Please provide the members of the {module}.",
-            f"Members of {module} you requested are: {module_member_names}.",
-        ),
+
+    module_members_context = f"Members of {module} are as follows: {module_member_names}."
+    module_members_questions = [
+        f"List the members of {module}.",
+        f"What are the members of the {module}?",
+        f"Can you tell me the members of the {module}?",
+        f"I need to know the members of the {module}.",
+        f"Could you list the members of the {module}?",
+        f"Please provide the members of the {module}.",
+    ]
+    module_members_answers = [
+        f"Members of {module} are as follows: {module_member_names}.",
+        f"The {module} has the following members: {module_member_names}.",
+        f"The members of the {module} are: {module_member_names}.",
+        f"Members of {module} you asked for are: {module_member_names}.",
+        f"Members of the {module} are: {module_member_names}.",
+        f"Members of {module} you requested are: {module_member_names}.",
     ]
-    module_retrieval_chunks.append(f"Members of {module} are as follows: {module_member_names}.")
-    module_tuning_pairs.extend(allocate_tuning_pairs(module_members_pairs))
+
+    module_retrieval_chunks.append(module_members_context)
+    module_tuning_documents.extend(
+        allocate_tuning_triplets(
+            module_members_context, module_members_questions, module_members_answers
+        )
+    )
 
     if not (module_summary := module_contents.module_summary):
-        module_summary_pairs = [
-            (f"What is the {module} for?", f"{module} does not have any documentation."),
-            (
-                f"Can you tell me the purpose of the {module}?",
-                f"The {module} lacks any documentation.",
-            ),
-            (
-                f"I'd like to know what the {module} is used for.",
-                f"Unfortunately, there is no documentation for the {module}.",
-            ),
-            (
-                f"Could you explain the function of the {module}?",
-                f"Regrettably, the {module} doesn't come with any documentation.",
-            ),
-            (f"What does the {module} do?", f"The {module} is without any documentation."),
-        ]
-        module_retrieval_chunks.append(
+        module_summary_context = (
             f"Unfortunately, {module} currently does not have any documentation."
         )
-        module_tuning_pairs.extend(allocate_tuning_pairs(module_summary_pairs))
+        module_summary_questions = [
+            f"What is the {module} for?",
+            f"Can you tell me the purpose of the {module}?",
+            f"I'd like to know what the {module} is used for.",
+            f"Could you explain the function of the {module}?",
+            f"What does the {module} do?",
+        ]
+        module_summary_answers = [
+            f"{module} does not have any documentation.",
+            f"The {module} lacks any documentation.",
+            f"There is no documentation for the {module}.",
+            f"The {module} doesn't come with any documentation.",
+            f"The {module} is without any documentation.",
+        ]
+
+        module_retrieval_chunks.append(module_summary_context)
+        module_tuning_documents.extend(
+            allocate_tuning_triplets(
+                module_summary_context, module_summary_questions, module_summary_answers
+            )
+        )
     else:
-        module_summary_pairs = [
-            (
-                f"What is the '{module_name}' module for?",
-                f"{module} documents itself as follows: '{module_summary}'.",
-            ),
-            (
-                f"Can you tell me the purpose of the '{module_name}' module?",
-                f"Purpose of {module} is documented as: '{module_summary}'.",
-            ),
-            (
-                f"I'm curious about the '{module_name}' module. What does it do?",
-                f"The {module} is described as: '{module_summary}'.",
-            ),
-            (
-                f"Could you explain the functionality of the '{module_name}' module?",
-                f"The functionality of the {module} is described as: '{module_summary}'.",
-            ),
-            (
-                f"I'd like to know more about the '{module_name}' module. What's its role?",
-                f"The role of the {module} is: '{module_summary}'.",
-            ),
-            (
-                f"What's the use of the '{module_name}' module?",
-                f"Use of the {module} is documented as: '{module_summary}'.",
-            ),
-        ]
-        module_retrieval_chunks.append(
+        module_summary_context = (
             f"The following is the documentation of {module}: {module_summary}."
         )
-        module_tuning_pairs.extend(allocate_tuning_pairs(module_summary_pairs))
+        module_summary_questions = [
+            f"What is the '{module_name}' module for?",
+            f"Can you tell me the purpose of the '{module_name}' module?",
+            f"I'm curious about the '{module_name}' module. What does it do?",
+            f"Could you explain the functionality of the '{module_name}' module?",
+            f"I'd like to know more about the '{module_name}' module. What's its role?",
+            f"What's the use of the '{module_name}' module?",
+        ]
+        module_summary_answers = [
+            f"{module} documents itself as follows: '{module_summary}'.",
+            f"Purpose of {module} is documented as: '{module_summary}'.",
+            f"The {module} is described as: '{module_summary}'.",
+            f"The functionality of the {module} is described as: '{module_summary}'.",
+            f"The role of the {module} is: '{module_summary}'.",
+            f"Use of the {module} is documented as: '{module_summary}'.",
+        ]
+
+        module_retrieval_chunks.append(module_summary_context)
+        module_tuning_documents.extend(
+            allocate_tuning_triplets(
+                module_summary_context, module_summary_questions, module_summary_answers
+            )
+        )
 
     if not (module_exports := module_contents.module_all_exports):
-        module_exports_pairs = [
-            (
-                f"Tell me the public members of the {module}.",
-                f"{module} lacks any public member exported through '__all__'.",
-            ),
-            (
-                f"What are the public members of the {module}?",
-                "There are no public members exported through '__all__' in the {module}.",
-            ),
-            (
-                f"Could you list the public members of the {module}?",
-                f"Unfortunately, {module} does not export any public members through '__all__'.",
-            ),
-            (
-                f"I need to know the public members of the {module}.",
-                f"The {module} does not have any public members exported through '__all__'.",
-            ),
-            (
-                f"Can you show me the public members of the {module}?",
-                f"The {module} does not contain any public members exported through '__all__'.",
-            ),
-            (
-                f"I'm interested in the public members of the {module}. What are they?",
-                f"{module} does not export any public members through '__all__'.",
-            ),
-        ]
-        module_retrieval_chunks.append(
+        module_exports_context = (
             f"{module} does not export anything publicly using __all__ variable."
         )
-        module_tuning_pairs.extend(allocate_tuning_pairs(module_exports_pairs))
+        module_exports_questions = [
+            f"Tell me the public members of the {module}.",
+            f"What are the public members of the {module}?",
+            f"Could you list the public members of the {module}?",
+            f"I need to know the public members of the {module}.",
+            f"Can you show me the public members of the {module}?",
+            f"I'm interested in the public members of the {module}. What are they?",
+        ]
+        module_exports_answers = [
+            f"{module} lacks any public member exported through '__all__'.",
+            f"There are no public members exported through '__all__' in the {module}.",
+            f"{module} does not export any public members through '__all__'.",
+            f"The {module} does not have any public members exported through '__all__'.",
+            f"The {module} does not contain any public members exported through '__all__'.",
+            f"{module} does not export any public members through '__all__'.",
+        ]
+
+        module_retrieval_chunks.append(module_exports_context)
+        module_tuning_documents.extend(
+            allocate_tuning_triplets(
+                module_exports_context, module_exports_questions, module_exports_answers
+            )
+        )
     else:
         module_exports_count = len(module_exports)
-        module_exports_count_pairs = [
-            (
-                f"How many objects does {module} export publicly?",
-                f"{module} exports {module_exports_count} many objects using __all__.",
-            ),
-            (
-                f"What is the count of publicly exported objects in {module}?",
-                f"The count of publicly exported objects in {module} is {module_exports_count}.",
-            ),
-            (
-                f"Could you tell me the number of objects publicly exported by {module}?",
-                f"{module} exports {module_exports_count} objects using __all__.",
-            ),
-            (
-                f"Please provide the count of objects publicly exported by {module}.",
-                f"The number of objects publicly exported by {module} is {module_exports_count}.",
-            ),
-            (
-                f"Tell me the quantity of objects that {module} exports publicly.",
-                f"{module} exports {module_exports_count} objects using __all__.",
-            ),
-            (
-                f"Would you mind letting me know how many objects {module} publicly exports?",
-                f"{module} publicly exports {module_exports_count} objects.",
-            ),
-        ]
-        module_retrieval_chunks.append(f"{module} has {module_exports_count} many public exports.")
-        module_tuning_pairs.extend(allocate_tuning_pairs(module_exports_count_pairs))
+
+        module_exports_count_context = f"{module} has {module_exports_count} many public exports."
+        module_exports_count_questions = [
+            f"How many objects does {module} export publicly?",
+            f"What is the count of publicly exported objects in {module}?",
+            f"Could you tell me the number of objects publicly exported by {module}?",
+            f"Please provide the count of objects publicly exported by {module}.",
+            f"Tell me the quantity of objects that {module} exports publicly.",
+            f"Would you mind letting me know how many objects {module} publicly exports?",
+        ]
+        module_exports_count_answers = [
+            f"{module} exports {module_exports_count} many objects using __all__.",
+            f"The count of publicly exported objects in {module} is {module_exports_count}.",
+            f"{module} exports {module_exports_count} objects using __all__.",
+            f"The number of objects publicly exported by {module} is {module_exports_count}.",
+            f"{module} exports {module_exports_count} objects using __all__.",
+            f"{module} publicly exports {module_exports_count} objects.",
+        ]
+
+        module_retrieval_chunks.append(module_exports_count_context)
+        module_tuning_documents.extend(
+            allocate_tuning_triplets(
+                module_exports_count_context,
+                module_exports_count_questions,
+                module_exports_count_answers,
+            )
+        )
 
         module_public_exports = enumerate_array_elements(module_exports)
-        module_exports_pairs = [
-            (
-                f"Tell me the public members of the {module}.",
-                f"{module} publicly exports the following members using '__all__':"
-                f" {module_public_exports}.",
-            ),
-            (
-                f"What are the public members of the {module}?",
-                f"The {module} publicly exports the following members using '__all__':"
-                f" {module_public_exports}.",
-            ),
-            (
-                f"Could you list the public members of the {module}?",
-                f"Sure, the {module} publicly exports these members using '__all__':"
-                f" {module_public_exports}.",
-            ),
-            (
-                f"I need to know the public members of the {module}.",
-                f"The {module} publicly exports these members using '__all__':"
-                f" {module_public_exports}.",
-            ),
-            (
-                f"Can you show me the public members of the {module}?",
-                f"Of course, the {module} publicly exports the following members using '__all__':"
-                f" {module_public_exports}.",
-            ),
-        ]
-        module_retrieval_chunks.append(
+
+        module_exports_context = (
             f"{module} exports following members using __all__: {module_public_exports}."
         )
-        module_tuning_pairs.extend(allocate_tuning_pairs(module_exports_pairs))
+        module_exports_questions = [
+            f"Tell me the public members of the {module}.",
+            f"What are the public members of the {module}?",
+            f"Could you list the public members of the {module}?",
+            f"I need to know the public members of the {module}.",
+            f"Can you show me the public members of the {module}?",
+        ]
+        module_exports_answers = [
+            f"{module} publicly exports the following members using '__all__':"
+            f" {module_public_exports}.",
+            f"The {module} publicly exports the following members using '__all__':"
+            f" {module_public_exports}.",
+            f"The {module} publicly exports these members using '__all__':"
+            f" {module_public_exports}.",
+        ]
+
+        module_retrieval_chunks.append(module_exports_context)
+        module_tuning_documents.extend(
+            allocate_tuning_triplets(
+                module_exports_context, module_exports_questions, module_exports_answers
+            )
+        )
 
     module_dataset = Dataset(
-        retrieval_chunks=module_retrieval_chunks, tuning_pairs=module_tuning_pairs
+        retrieval_chunks=module_retrieval_chunks, tuning_documents=module_tuning_documents
     )
 
     return module_dataset
 
 
 @pydantic.validate_call(validate_return=True)
 def generate_enum_member_dataset(
@@ -970,147 +888,131 @@
     list[str]
         only retrieval documents
     """
     enum_member_retrieval_chunks: list[str] = [
         f"{enum_member} is a Python enum.",
         f"{enum_member} has following docstring: {enum_docstring}.",
     ]
-    enum_member_tuning_pairs: list[tuple[str, str, SplitName]] = []
+    enum_member_tuning_documents: list[Document] = []
 
     enum_member_count = len(member_type_details.enum_members)
-    enum_member_count_pairs = [
-        (
-            f"How many members are there in {enum_member}?",
-            f"{enum_member} has {enum_member_count} members.",
-        ),
-        (
-            f"What is the count of members in {enum_member}?",
-            f"The count of members in {enum_member} is {enum_member_count}.",
-        ),
-        (
-            f"Can you tell me the number of members in {enum_member}?",
-            f"Sure, the number of members in {enum_member} is {enum_member_count}.",
-        ),
-        (
-            f"Could you provide the total number of members in {enum_member}?",
-            f"The total number of members in {enum_member} is {enum_member_count}.",
-        ),
-        (
-            f"I need to know the quantity of members in {enum_member}.",
-            f"The quantity of members in {enum_member} is {enum_member_count}.",
-        ),
-        (
-            f"Please inform me about the number of members in {enum_member}.",
-            f"The number of members in {enum_member} is {enum_member_count}.",
-        ),
+
+    enum_member_count_context = f"{enum_member} has {enum_member_count} many members."
+    enum_member_count_questions = [
+        f"How many members are there in {enum_member}?",
+        f"What is the count of members in {enum_member}?",
+        f"Can you tell me the number of members in {enum_member}?",
+        f"Could you provide the total number of members in {enum_member}?",
+        f"I need to know the quantity of members in {enum_member}.",
+        f"Please inform me about the number of members in {enum_member}.",
     ]
-    enum_member_retrieval_chunks.insert(-1, f"{enum_member} has {enum_member_count} many members.")
-    enum_member_tuning_pairs.extend(allocate_tuning_pairs(enum_member_count_pairs))
+    enum_member_count_answers = [
+        f"{enum_member} has {enum_member_count} members.",
+        f"The count of members in {enum_member} is {enum_member_count}.",
+        f"The number of members in {enum_member} is {enum_member_count}.",
+        f"The total number of members in {enum_member} is {enum_member_count}.",
+        f"The quantity of members in {enum_member} is {enum_member_count}.",
+        f"The number of members in {enum_member} is {enum_member_count}.",
+    ]
+
+    enum_member_retrieval_chunks.append(enum_member_count_context)
+    enum_member_tuning_documents.extend(
+        allocate_tuning_triplets(
+            enum_member_count_context, enum_member_count_questions, enum_member_count_answers
+        )
+    )
 
     enum_members = enumerate_array_elements(
         member_type_details.enum_members, attribute="enum_member"
     )
-    enum_members_pairs = [
-        (
-            f"What are the different members of {enum_member}?",
-            f"Different members of {enum_member} are as follows: {enum_members}.",
-        ),
-        (
-            f"Can you list the different members of {enum_member}?",
-            f"Sure, the different members of {enum_member} are: {enum_members}.",
-        ),
-        (
-            f"Could you tell me the different members of {enum_member}?",
-            f"Of course, the different members of {enum_member} include: {enum_members}.",
-        ),
-        (
-            f"I need to know the different members of {enum_member}.",
-            f"The different members of {enum_member} are: {enum_members}.",
-        ),
-        (
-            f"What does {enum_member} consist of?",
-            f"{enum_member} consists of the following members: {enum_members}.",
-        ),
+
+    enum_members_context = f"Members of {enum_member} are as follows: {enum_members}."
+    enum_members_questions = [
+        f"What are the different members of {enum_member}?",
+        f"Can you list the different members of {enum_member}?",
+        f"Could you tell me the different members of {enum_member}?",
+        f"I need to know the different members of {enum_member}.",
+        f"What does {enum_member} consist of?",
     ]
-    enum_member_retrieval_chunks.insert(
-        -1, f"Members of {enum_member} are as follows: {enum_members}."
+    enum_members_answers = [
+        f"Different members of {enum_member} are as follows: {enum_members}.",
+        f"The different members of {enum_member} include: {enum_members}.",
+        f"The different members of {enum_member} are: {enum_members}.",
+        f"{enum_member} consists of the following members: {enum_members}.",
+    ]
+
+    enum_member_retrieval_chunks.append(enum_members_context)
+    enum_member_tuning_documents.extend(
+        allocate_tuning_triplets(
+            enum_members_context, enum_members_questions, enum_members_answers
+        )
     )
-    enum_member_tuning_pairs.extend(allocate_tuning_pairs(enum_members_pairs))
 
     enum_member_names = enumerate_array_elements(
         member_type_details.enum_members, attribute="enum_member_name"
     )
-    enum_member_names_pairs = [
-        (
-            f"List just the names of different members of {enum_member}.",
-            f"Different members of {enum_member} have the following names: {enum_member_names}.",
-        ),
-        (
-            f"Can you provide the names of different members of {enum_member}?",
-            f"Sure, different members of {enum_member} are named as follows: {enum_member_names}.",
-        ),
-        (
-            f"What are the names of different members of {enum_member}?",
-            f"The names of different members of {enum_member} are: {enum_member_names}.",
-        ),
-        (
-            f"I need the names of different members of {enum_member}.",
-            f"The different members of {enum_member} have these names: {enum_member_names}.",
-        ),
-        (
-            f"Could you list the names of different members of {enum_member}?",
-            f"Of course, different members of {enum_member} have these names:"
-            f" {enum_member_names}.",
-        ),
-        (
-            f"Show me the names of different members of {enum_member}.",
-            f"The names of different members of {enum_member} are: {enum_member_names}.",
-        ),
+
+    enum_member_names_context = (
+        f"Names of different members of {enum_member} are as follows: {enum_member_names}."
+    )
+    enum_member_names_questions = [
+        f"List just the names of different members of {enum_member}.",
+        f"Can you provide the names of different members of {enum_member}?",
+        f"What are the names of different members of {enum_member}?",
+        f"I need the names of different members of {enum_member}.",
+        f"Could you list the names of different members of {enum_member}?",
+        f"Show me the names of different members of {enum_member}.",
     ]
-    enum_member_retrieval_chunks.insert(
-        -1, f"Names of different members of {enum_member} are as follows: {enum_member_names}."
+    enum_member_names_answers = [
+        f"Different members of {enum_member} have the following names: {enum_member_names}.",
+        f"Different members of {enum_member} are named as follows: {enum_member_names}.",
+        f"The names of different members of {enum_member} are: {enum_member_names}.",
+        f"Different members of {enum_member} have these names: {enum_member_names}.",
+    ]
+
+    enum_member_retrieval_chunks.append(enum_member_names_context)
+    enum_member_tuning_documents.extend(
+        allocate_tuning_triplets(
+            enum_member_names_context, enum_member_names_questions, enum_member_names_answers
+        )
     )
-    enum_member_tuning_pairs.extend(allocate_tuning_pairs(enum_member_names_pairs))
 
     enum_member_values = enumerate_array_elements(
         member_type_details.enum_members, attribute="enum_member_value"
     )
-    enum_member_values_pairs = [
-        (
-            f"Only show the different values supported by {enum_member}.",
-            f"{enum_member} supports the following values: {enum_member_values}.",
-        ),
-        (
-            f"What are the different values that {enum_member} supports?",
-            f"The different values that {enum_member} supports are: {enum_member_values}.",
-        ),
-        (
-            f"Can you list the values supported by {enum_member}?",
-            f"Sure, {enum_member} supports these values: {enum_member_values}.",
-        ),
-        (
-            f"I need to know the values supported by {enum_member}.",
-            f"{enum_member} supports these values: {enum_member_values}.",
-        ),
-        (
-            f"Could you tell me the values that {enum_member} supports?",
-            f"Of course, the values that {enum_member} supports are: {enum_member_values}.",
-        ),
-        (
-            f"Please provide the values supported by {enum_member}.",
-            f"The values supported by {enum_member} are: {enum_member_values}.",
-        ),
+
+    enum_member_values_context = (
+        f"Values of different members of {enum_member} are as follows: {enum_member_values}."
+    )
+    enum_member_values_questions = [
+        f"Only show the different values supported by {enum_member}.",
+        f"What are the different values that {enum_member} supports?",
+        f"Can you list the values supported by {enum_member}?",
+        f"I need to know the values supported by {enum_member}.",
+        f"Could you tell me the values that {enum_member} supports?",
+        f"Please provide the values supported by {enum_member}.",
+    ]
+    enum_member_values_answers = [
+        f"{enum_member} supports the following values: {enum_member_values}.",
+        f"The different values that {enum_member} supports are: {enum_member_values}.",
+        f"{enum_member} supports these values: {enum_member_values}.",
+        f"The values that {enum_member} supports are: {enum_member_values}.",
+        f"The values supported by {enum_member} are: {enum_member_values}.",
     ]
-    enum_member_retrieval_chunks.insert(
-        -1, f"Values of different members of {enum_member} are as follows: {enum_member_values}."
+
+    enum_member_retrieval_chunks.append(enum_member_values_context)
+    enum_member_tuning_documents.extend(
+        allocate_tuning_triplets(
+            enum_member_values_context, enum_member_values_questions, enum_member_values_answers
+        )
     )
-    enum_member_tuning_pairs.extend(allocate_tuning_pairs(enum_member_values_pairs))
 
     enum_member_dataset = Dataset(
-        retrieval_chunks=enum_member_retrieval_chunks, tuning_pairs=enum_member_tuning_pairs
+        retrieval_chunks=enum_member_retrieval_chunks,
+        tuning_documents=enum_member_tuning_documents,
     )
 
     return enum_member_dataset, enum_member_retrieval_chunks
 
 
 @pydantic.validate_call(validate_return=True)
 def generate_class_member_dataset(  # noqa: C901, PLR0912, PLR0915
@@ -1134,725 +1036,667 @@
     list[str]
         only retrieval documents
     """
     class_member_retrieval_chunks: list[str] = [
         f"{class_member} is a Python class.",
         f"{class_member} has following docstring: {class_docstring}.",
     ]
-    class_member_tuning_pairs: list[tuple[str, str, SplitName]] = []
+    class_member_tuning_documents: list[Document] = []
 
     if not (class_parameters := member_type_details.class_parameters):
-        class_parameters_pairs = [
-            (
-                f"What are the different parameters of {class_member}?",
-                f"{class_member} needs no arguments for instantiation.",
-            ),
-            (
-                f"Can you tell me the parameters required for {class_member}?",
-                f"No parameters are required for instantiating {class_member}.",
-            ),
-            (
-                f"What arguments do I need to instantiate {class_member}?",
-                f"You don't need any arguments to instantiate {class_member}.",
-            ),
-            (
-                f"Do I need any parameters to use {class_member}?",
-                f"{class_member} can be used without any parameters.",
-            ),
-            (
-                f"What should I pass as arguments when creating an instance of {class_member}?",
-                "There's no need to pass any arguments"
-                f" when creating an instance of {class_member}.",
-            ),
-            (
-                f"Are there any parameters needed for the instantiation of {class_member}?",
-                f"The instantiation of {class_member} doesn't require any parameters.",
-            ),
-        ]
-        class_member_retrieval_chunks.append(
-            f"{class_member} requires no arguments for instantiation."
+        class_parameters_context = f"{class_member} requires no arguments for instantiation."
+        class_parameters_questions = [
+            f"What are the different parameters of {class_member}?",
+            f"Can you tell me the parameters required for {class_member}?",
+            f"What arguments do I need to instantiate {class_member}?",
+            f"Do I need any parameters to use {class_member}?",
+            f"What should I pass as arguments when creating an instance of {class_member}?",
+            f"Are there any parameters needed for the instantiation of {class_member}?",
+        ]
+        class_parameters_answers = [
+            f"{class_member} needs no arguments for instantiation.",
+            f"No parameters are required for instantiating {class_member}.",
+            f"Arguments are not needed to instantiate {class_member}.",
+            f"{class_member} can be used without any parameters.",
+            f"There's no need to pass any arguments when creating an instance of {class_member}.",
+            f"The instantiation of {class_member} doesn't require any parameters.",
+        ]
+
+        class_member_retrieval_chunks.append(class_parameters_context)
+        class_member_tuning_documents.extend(
+            allocate_tuning_triplets(
+                class_parameters_context, class_parameters_questions, class_parameters_answers
+            )
         )
-        class_member_tuning_pairs.extend(allocate_tuning_pairs(class_parameters_pairs))
     else:
         class_parameter_names = enumerate_array_elements(
             class_parameters, attribute="parameter_details"
         )
-        class_parameters_pairs = [
-            (
-                f"What are the different parameters of {class_member}?",
-                f"{class_member} supports these arguments to initiate"
-                f" a new instance: {class_parameter_names}.",
-            ),
-            (
-                f"Can you list the parameters for {class_member}?",
-                f"Sure, {class_member} can be initiated with these arguments:"
-                f" {class_parameter_names}.",
-            ),
-            (
-                f"I need to know the parameters of {class_member}.",
-                f"The parameters to initiate a new instance of {class_member} are:"
-                f" {class_parameter_names}.",
-            ),
-            (
-                f"Tell me the parameters that {class_member} supports.",
-                f"{class_member} can be initiated with these arguments: {class_parameter_names}.",
-            ),
-            (
-                f"What arguments does {class_member} take for initialisation?",
-                f"To initialise {class_member}, you can use these arguments:"
-                f" {class_parameter_names}.",
-            ),
-        ]
-        class_member_retrieval_chunks.append(
+
+        class_parameters_context = (
             f"{class_member} requires the following arguments for initialisation:"
             f" {class_parameter_names}"
         )
-        class_member_tuning_pairs.extend(allocate_tuning_pairs(class_parameters_pairs))
+        class_parameters_questions = [
+            f"What are the different parameters of {class_member}?",
+            f"Can you list the parameters for {class_member}?",
+            f"I need to know the parameters of {class_member}.",
+            f"Tell me the parameters that {class_member} supports.",
+            f"What arguments does {class_member} take for initialisation?",
+        ]
+        class_parameters_answers = [
+            f"{class_member} supports these arguments to initiate"
+            f" a new instance: {class_parameter_names}.",
+            f"{class_member} can be initiated with these arguments: {class_parameter_names}.",
+            f"The parameters to initiate a new instance of {class_member} are:"
+            f" {class_parameter_names}.",
+            f"To initialise {class_member}, you can use these arguments: {class_parameter_names}.",
+        ]
+
+        class_member_retrieval_chunks.append(class_parameters_context)
+        class_member_tuning_documents.extend(
+            allocate_tuning_triplets(
+                class_parameters_context, class_parameters_questions, class_parameters_answers
+            )
+        )
 
     for class_parameter in class_parameters:
         parameter_name = class_parameter.parameter_name
         parameter = f"'{parameter_name}' argument in {class_member}"
 
-        if (parameter_default := class_parameter.parameter_default) is inspect._empty:
-            class_parameter_defaults_pairs = [
-                (
-                    f"Tell default value of {parameter}.",
-                    f"{parameter} does not have a default value.",
-                ),
-                (
-                    f"What is the default value of {parameter}?",
-                    f"The {parameter} does not have a default value.",
-                ),
-                (
-                    f"Could you inform me about default value of {parameter}?",
-                    f"Sure, the {parameter} does not have a default value.",
-                ),
-                (
-                    f"I need to know the default value of {parameter}. Can you help?",
-                    f"Of course, the {parameter} does not have a default value.",
-                ),
-                (
-                    f"Can you tell me if {parameter} has default value?",
-                    f"No, the {parameter} does not have a default value.",
-                ),
-                (
-                    f"I'm curious about default value of {parameter}.",
-                    f"Well, the {parameter} does not have a default value.",
-                ),
+        if (parameter_default := class_parameter.parameter_default) is EMPTY_PARAMETER:
+            class_parameter_defaults_context = f"{parameter} does not have a default value."
+            class_parameter_defaults_questions = [
+                f"Tell default value of {parameter}.",
+                f"What is the default value of {parameter}?",
+                f"Could you inform me about default value of {parameter}?",
+                f"I need to know the default value of {parameter}. Can you help?",
+                f"Can you tell me if {parameter} has default value?",
+                f"I'm curious about default value of {parameter}.",
             ]
-            class_member_retrieval_chunks.append(f"{parameter} does not have a default value.")
-            class_member_tuning_pairs.extend(allocate_tuning_pairs(class_parameter_defaults_pairs))
-        else:
-            class_parameter_defaults_pairs = [
-                (
-                    f"Tell default value of {parameter}.",
-                    f"{parameter} takes {parameter_default} by default.",
-                ),
-                (
-                    f"What is the default value of {parameter}?",
-                    f"The default value of {parameter} is {parameter_default}.",
-                ),
-                (
-                    f"Could you inform me about default value of {parameter}?",
-                    f"Sure, the default value of {parameter} is {parameter_default}.",
-                ),
-                (
-                    f"I need to know the default value of {parameter}.",
-                    f"The default value of {parameter} is {parameter_default}.",
-                ),
-                (
-                    f"Can you provide default value of {parameter}?",
-                    f"Yes, default value of {parameter} is {parameter_default}.",
-                ),
-                (
-                    f"Please, disclose default value of {parameter}.",
-                    f"Certainly, the default value of {parameter} is {parameter_default}.",
-                ),
+            class_parameter_defaults_answers = [
+                f"{parameter} does not have a default value.",
+                f"The {parameter} does not have a default value.",
             ]
-            class_member_retrieval_chunks.append(
+
+            class_member_retrieval_chunks.append(class_parameter_defaults_context)
+            class_member_tuning_documents.extend(
+                allocate_tuning_triplets(
+                    class_parameter_defaults_context,
+                    class_parameter_defaults_questions,
+                    class_parameter_defaults_answers,
+                )
+            )
+        else:
+            class_parameter_defaults_context = (
                 f"{parameter_default} is the default value of {parameter}."
             )
-            class_member_tuning_pairs.extend(allocate_tuning_pairs(class_parameter_defaults_pairs))
+            class_parameter_defaults_questions = [
+                f"Tell default value of {parameter}.",
+                f"What is the default value of {parameter}?",
+                f"Could you inform me about default value of {parameter}?",
+                f"I need to know the default value of {parameter}.",
+                f"Can you provide default value of {parameter}?",
+                f"Please, disclose default value of {parameter}.",
+            ]
+            class_parameter_defaults_answers = [
+                f"{parameter} takes {parameter_default} by default.",
+                f"Default value of {parameter} is {parameter_default}.",
+                f"The default value of {parameter} is {parameter_default}.",
+            ]
 
-        if (parameter_annotation := class_parameter.parameter_annotation) is inspect._empty:
-            class_parameter_types_pairs = [
-                (
-                    f"Name type hint for {parameter}.",
-                    f"{parameter} does not have a type annotation.",
-                ),
-                (
-                    f"What is the type hint for {parameter}?",
-                    f"There is no type annotation for the {parameter}.",
-                ),
-                (
-                    f"Can you tell me the type hint for {parameter}?",
-                    f"The {parameter} is not annotated with a type.",
-                ),
-                (
-                    f"I'm looking for the type hint for {parameter}. Can you help?",
-                    f"Sure, the {parameter} does not have a type annotation.",
-                ),
-                (
-                    f"Could you provide the type hint for {parameter}?",
-                    f"Unfortunately, {parameter} does not have type annotation.",
-                ),
-                (
-                    f"I need to know the type hint for {parameter}.",
-                    f"The {parameter} does not come with a type annotation.",
-                ),
+            class_member_retrieval_chunks.append(class_parameter_defaults_context)
+            class_member_tuning_documents.extend(
+                allocate_tuning_triplets(
+                    class_parameter_defaults_context,
+                    class_parameter_defaults_questions,
+                    class_parameter_defaults_answers,
+                )
+            )
+
+        if (parameter_annotation := class_parameter.parameter_annotation) is EMPTY_PARAMETER:
+            class_parameter_types_context = f"Type hint for {parameter} is unavailable."
+            class_parameter_types_questions = [
+                f"Name type hint for {parameter}.",
+                f"What is the type hint for {parameter}?",
+                f"Can you tell me the type hint for {parameter}?",
+                f"I'm looking for the type hint for {parameter}. Can you help?",
+                f"Could you provide the type hint for {parameter}?",
+                f"I need to know the type hint for {parameter}.",
             ]
-            class_member_retrieval_chunks.append(f"Type hint for {parameter} is unavailable.")
-            class_member_tuning_pairs.extend(allocate_tuning_pairs(class_parameter_types_pairs))
-        else:
-            class_parameter_types_pairs = [
-                (
-                    f"Name type hint for {parameter}.",
-                    f"{parameter} has '{parameter_annotation}' as type hint.",
-                ),
-                (
-                    f"What is the type hint for {parameter}?",
-                    f"The type hint for {parameter} is '{parameter_annotation}'.",
-                ),
-                (
-                    f"Could you tell me the type hint for {parameter}?",
-                    f"Sure, the type hint for {parameter} is '{parameter_annotation}'.",
-                ),
-                (
-                    f"I need to know the type hint for {parameter}.",
-                    f"The type hint for {parameter} is '{parameter_annotation}'.",
-                ),
-                (
-                    f"Identify the type hint for {parameter}.",
-                    f"The type hint for {parameter} is '{parameter_annotation}'.",
-                ),
-                (
-                    f"Can you specify the type hint for {parameter}?",
-                    f"Yes, the type hint for {parameter} is '{parameter_annotation}'.",
-                ),
+            class_parameter_types_answers = [
+                f"{parameter} does not have a type annotation.",
+                f"There is no type annotation for the {parameter}.",
+                f"The {parameter} is not annotated with a type.",
+                f"The {parameter} does not have a type annotation.",
+                f"{parameter} does not have type annotation.",
+                f"The {parameter} does not come with a type annotation.",
             ]
-            class_member_retrieval_chunks.append(
+
+            class_member_retrieval_chunks.append(class_parameter_types_context)
+            class_member_tuning_documents.extend(
+                allocate_tuning_triplets(
+                    class_parameter_types_context,
+                    class_parameter_types_questions,
+                    class_parameter_types_answers,
+                )
+            )
+        else:
+            class_parameter_types_context = (
                 f"{parameter} is annotated as '{parameter_annotation}' type."
             )
-            class_member_tuning_pairs.extend(allocate_tuning_pairs(class_parameter_types_pairs))
+            class_parameter_types_questions = [
+                f"Name type hint for {parameter}.",
+                f"What is the type hint for {parameter}?",
+                f"Could you tell me the type hint for {parameter}?",
+                f"I need to know the type hint for {parameter}.",
+                f"Identify the type hint for {parameter}.",
+                f"Can you specify the type hint for {parameter}?",
+            ]
+            class_parameter_types_answers = [
+                f"{parameter} has '{parameter_annotation}' as type hint.",
+                f"The type hint for {parameter} is '{parameter_annotation}'.",
+            ]
+
+            class_member_retrieval_chunks.append(class_parameter_types_context)
+            class_member_tuning_documents.extend(
+                allocate_tuning_triplets(
+                    class_parameter_types_context,
+                    class_parameter_types_questions,
+                    class_parameter_types_answers,
+                )
+            )
 
         if not (parameter_summary := class_parameter.parameter_summary):
-            class_parameter_summary_pairs = [
-                (
-                    f"What does {parameter} do?",
-                    f"Docstring of {class_member} does not describe '{parameter_name}'.",
-                ),
-                (
-                    f"Can you explain the role of {parameter}?",
-                    f"The docstring of {class_member} does not provide any information about"
-                    f" '{parameter_name}'.",
-                ),
-                (
-                    f"I'm trying to understand what {parameter} does. Can you help?",
-                    f"Unfortunately, the docstring of {class_member} does not mention anything"
-                    f" about '{parameter_name}'.",
-                ),
-                (
-                    f"What is the function of {parameter}?",
-                    f"There is no description of '{parameter_name}' in the docstring of"
-                    f" {class_member}.",
-                ),
-                (
-                    f"Could you tell me what '{parameter_name}' does in {class_member}?",
-                    f"The docstring of {class_member} does not contain any details about"
-                    f" '{parameter_name}'.",
-                ),
-                (
-                    f"I'm curious about the purpose of {parameter}. Can you enlighten me?",
-                    f"I'm sorry, but the docstring of {class_member} does not discuss"
-                    f" '{parameter_name}'.",
-                ),
-            ]
-            class_member_retrieval_chunks.append(
+            class_parameter_summary_context = (
                 f"{parameter} lacks any documentation in the docstring."
             )
-            class_member_tuning_pairs.extend(allocate_tuning_pairs(class_parameter_summary_pairs))
-        else:
-            class_parameter_summary_pairs = [
-                (
-                    f"What does {parameter} do?",
-                    f"{class_member} documents role of '{parameter_name}' as follows:"
-                    f" '{parameter_summary}'.",
-                ),
-                (
-                    f"Can you explain the role of {parameter}?",
-                    f"Sure, {class_member} describes '{parameter_name}' as follows:"
-                    f" '{parameter_summary}'.",
-                ),
-                (
-                    f"I'm curious about {parameter}. What does it do?",
-                    f"In {class_member}, '{parameter_name}' is documented as follows:"
-                    f" '{parameter_summary}'.",
-                ),
-                (
-                    f"Could you tell me what {parameter} does?",
-                    f"Of course, {parameter} is described as follows: '{parameter_summary}'.",
-                ),
-                (
-                    f"What's the function of {parameter}?",
-                    f"{class_member} describes the function of '{parameter_name}' as follows:"
-                    f" '{parameter_summary}'.",
-                ),
-                (
-                    f"I'd like to know the purpose of {parameter}.",
-                    f"In {class_member}, the purpose of '{parameter_name}' is defined as follows:"
-                    f" '{parameter_summary}'.",
-                ),
+            class_parameter_summary_questions = [
+                f"What does {parameter} do?",
+                f"Can you explain the role of {parameter}?",
+                f"I'm trying to understand what {parameter} does. Can you help?",
+                f"What is the function of {parameter}?",
+                f"Could you tell me what '{parameter_name}' does in {class_member}?",
+                f"I'm curious about the purpose of {parameter}. Can you enlighten me?",
+            ]
+            class_parameter_summary_answers = [
+                f"Docstring of {class_member} does not describe '{parameter_name}'.",
+                f"The docstring of {class_member} does not provide any information about"
+                f" '{parameter_name}'.",
+                f"The docstring of {class_member} does not mention anything"
+                f" about '{parameter_name}'.",
+                f"There is no description of '{parameter_name}' in the docstring of"
+                f" {class_member}.",
+                f"The docstring of {class_member} does not contain any details about"
+                f" '{parameter_name}'.",
+                f"The docstring of {class_member} does not discuss '{parameter_name}'.",
             ]
-            class_member_retrieval_chunks.append(
+
+            class_member_retrieval_chunks.append(class_parameter_summary_context)
+            class_member_tuning_documents.extend(
+                allocate_tuning_triplets(
+                    class_parameter_summary_context,
+                    class_parameter_summary_questions,
+                    class_parameter_summary_answers,
+                )
+            )
+        else:
+            class_parameter_summary_context = (
                 f"As per docstring, role of {parameter} is: '{parameter_summary}'."
             )
-            class_member_tuning_pairs.extend(allocate_tuning_pairs(class_parameter_summary_pairs))
+            class_parameter_summary_questions = [
+                f"What does {parameter} do?",
+                f"Can you explain the role of {parameter}?",
+                f"I'm curious about {parameter}. What does it do?",
+                f"Could you tell me what {parameter} does?",
+                f"What's the function of {parameter}?",
+                f"I'd like to know the purpose of {parameter}.",
+            ]
+            class_parameter_summary_answers = [
+                f"{class_member} documents role of '{parameter_name}' as follows:"
+                f" '{parameter_summary}'.",
+                f"{class_member} describes '{parameter_name}' as follows: '{parameter_summary}'.",
+                f"In {class_member}, '{parameter_name}' is documented as follows:"
+                f" '{parameter_summary}'.",
+                f"{parameter} is described as follows: '{parameter_summary}'.",
+                f"{class_member} describes the function of '{parameter_name}' as follows:"
+                f" '{parameter_summary}'.",
+                f"In {class_member}, the purpose of '{parameter_name}' is defined as follows:"
+                f" '{parameter_summary}'.",
+            ]
+
+            class_member_retrieval_chunks.append(class_parameter_summary_context)
+            class_member_tuning_documents.extend(
+                allocate_tuning_triplets(
+                    class_parameter_summary_context,
+                    class_parameter_summary_questions,
+                    class_parameter_summary_answers,
+                )
+            )
 
     if not (class_methods := member_type_details.class_methods):
-        class_method_names_pairs = [
-            (
-                f"List names of the public methods of {class_member}.",
-                f"{class_member} does not have any public methods (not starting with '_').",
-            ),
-            (
-                f"Can you provide the names of the public methods for {class_member}?",
-                f"Unfortunately, {class_member} does not have any public methods.",
-            ),
-            (
-                f"What are the public methods of {class_member}?",
-                f"There are no public methods (not starting with '_') in {class_member}.",
-            ),
-            (
-                f"I need to know the public methods of {class_member}. Can you list them?",
-                f"I'm sorry, but {class_member} does not have any public methods.",
-            ),
-            (
-                f"Could you list the public methods of {class_member}?",
-                f"{class_member} does not contain any public methods (not starting with '_').",
-            ),
-            (
-                f"Show me the public methods of {class_member}.",
-                f"It appears that {class_member} does not have any public methods.",
-            ),
-        ]
-        class_member_retrieval_chunks.append(
+        class_method_names_context = (
             f"{class_member} has no public (without _ as the prefix) methods."
         )
-        class_member_tuning_pairs.extend(allocate_tuning_pairs(class_method_names_pairs))
+        class_method_names_questions = [
+            f"List names of the public methods of {class_member}.",
+            f"Can you provide the names of the public methods for {class_member}?",
+            f"What are the public methods of {class_member}?",
+            f"I need to know the public methods of {class_member}. Can you list them?",
+            f"Could you list the public methods of {class_member}?",
+            f"Show me the public methods of {class_member}.",
+        ]
+        class_method_names_answers = [
+            f"{class_member} does not have any public methods (not starting with '_').",
+            f"{class_member} does not have any public methods.",
+            f"There are no public methods (not starting with '_') in {class_member}.",
+            f"{class_member} does not have any public methods.",
+            f"{class_member} does not contain any public methods (not starting with '_').",
+            f"It appears that {class_member} does not have any public methods.",
+        ]
+
+        class_member_retrieval_chunks.append(class_method_names_context)
+        class_member_tuning_documents.extend(
+            allocate_tuning_triplets(
+                class_method_names_context,
+                class_method_names_questions,
+                class_method_names_answers,
+            )
+        )
     else:
         class_methods_count = len(class_methods)
-        class_methods_count_pairs = [
-            (
-                f"How many public methods does {class_member} have?",
-                f"{class_member} has {class_methods_count} many public methods.",
-            ),
-            (
-                f"What is the count of public methods in {class_member}?",
-                f"The count of public methods in {class_member} is {class_methods_count}.",
-            ),
-            (
-                f"Could you tell me the number of public methods in {class_member}?",
-                f"{class_member} has {class_methods_count} public methods.",
-            ),
-            (
-                f"Please provide the count of public methods for {class_member}.",
-                f"The number of public methods in {class_member} is {class_methods_count}.",
-            ),
-            (
-                f"Tell me the quantity of public methods present in {class_member}.",
-                f"{class_member} has {class_methods_count} public methods.",
-            ),
-            (
-                f"Would you mind letting me know how many public methods {class_member} contains?",
-                f"{class_member} contains {class_methods_count} public methods.",
-            ),
-        ]
-        class_member_retrieval_chunks.append(
+
+        class_methods_count_context = (
             f"{class_member} has {class_methods_count} many public methods."
         )
-        class_member_tuning_pairs.extend(allocate_tuning_pairs(class_methods_count_pairs))
+        class_methods_count_questions = [
+            f"How many public methods does {class_member} have?",
+            f"What is the count of public methods in {class_member}?",
+            f"Could you tell me the number of public methods in {class_member}?",
+            f"Please provide the count of public methods for {class_member}.",
+            f"Tell me the quantity of public methods present in {class_member}.",
+            f"Would you mind letting me know how many public methods {class_member} contains?",
+        ]
+        class_methods_count_answers = [
+            f"{class_member} has {class_methods_count} many public methods.",
+            f"The count of public methods in {class_member} is {class_methods_count}.",
+            f"{class_member} has {class_methods_count} public methods.",
+            f"The number of public methods in {class_member} is {class_methods_count}.",
+            f"{class_member} has {class_methods_count} public methods.",
+            f"{class_member} contains {class_methods_count} public methods.",
+        ]
+
+        class_member_retrieval_chunks.append(class_methods_count_context)
+        class_member_tuning_documents.extend(
+            allocate_tuning_triplets(
+                class_methods_count_context,
+                class_methods_count_questions,
+                class_methods_count_answers,
+            )
+        )
 
         class_public_methods = enumerate_array_elements(class_methods, attribute="method_name")
-        class_method_names_pairs = [
-            (
-                f"List names of the public methods of {class_member}.",
-                f"Here are the public methods of {class_member}: {class_public_methods}.",
-            ),
-            (
-                f"Can you provide the names of the public methods for {class_member}?",
-                f"Sure, the public methods of {class_member} that do not start with '_' are:"
-                f" {class_public_methods}.",
-            ),
-            (
-                f"What are the public methods of {class_member}?",
-                f"The public methods of {class_member} (excluding those starting with '_') are:"
-                f" {class_public_methods}.",
-            ),
-            (
-                f"I need to know the public methods of {class_member}.",
-                f"The public methods of {class_member} (those not starting with '_') are:"
-                f" {class_public_methods}.",
-            ),
-            (
-                f"Could you list the public methods of {class_member}?",
-                f"Of course, the public methods of {class_member} (not beginning with '_') are:"
-                f" {class_public_methods}.",
-            ),
-            (
-                f"Please show me the public methods of {class_member}.",
-                f"Here you go, the public methods of {class_member}"
-                f" (excluding those with a prefix '_') are: {class_public_methods}.",
-            ),
-        ]
-        class_member_retrieval_chunks.append(
+
+        class_method_names_context = (
             f"{class_member} has the following public methods: {class_public_methods}"
         )
-        class_member_tuning_pairs.extend(allocate_tuning_pairs(class_method_names_pairs))
+        class_method_names_questions = [
+            f"List names of the public methods of {class_member}.",
+            f"Can you provide the names of the public methods for {class_member}?",
+            f"What are the public methods of {class_member}?",
+            f"I need to know the public methods of {class_member}.",
+            f"Could you list the public methods of {class_member}?",
+            f"Please show me the public methods of {class_member}.",
+        ]
+        class_method_names_answers = [
+            f"Here are the public methods of {class_member}: {class_public_methods}.",
+            f"The public methods of {class_member} that do not start with '_' are:"
+            f" {class_public_methods}.",
+            f"The public methods of {class_member} (excluding those starting with '_') are:"
+            f" {class_public_methods}.",
+            f"The public methods of {class_member} (those not starting with '_') are:"
+            f" {class_public_methods}.",
+            f"The public methods of {class_member} (not beginning with '_') are:"
+            f" {class_public_methods}.",
+            f"The public methods of {class_member} (excluding those with a prefix '_') are:"
+            f" {class_public_methods}.",
+        ]
+
+        class_member_retrieval_chunks.append(class_method_names_context)
+        class_member_tuning_documents.extend(
+            allocate_tuning_triplets(
+                class_method_names_context,
+                class_method_names_questions,
+                class_method_names_answers,
+            )
+        )
 
     for class_method in class_methods:
         method_name = class_method.method_name
         method = f"'{method_name}' method of {class_member}"
 
         if not (method_parameters := class_method.method_parameters):
-            class_method_parameters_pairs = [
-                (f"What arguments do {method} accept?", f"{method} does not take any parameters."),
-                (
-                    f"Can you tell me the parameters that {method} requires?",
-                    f"The {method} does not require any parameters.",
-                ),
-                (
-                    f"What are the inputs for the {method} in {class_member}?",
-                    f"There are no inputs for the {method} in {class_member}.",
-                ),
-                (
-                    f"Does the {method} need any arguments?",
-                    f"No, {method} does not need any arguments.",
-                ),
-                (
-                    f"What parameters should I pass to {method}?",
-                    f"You don't need to pass any parameters to the {method}.",
-                ),
-                (
-                    f"What are required arguments for {method}?",
-                    f"{method} does not require any arguments.",
-                ),
+            class_method_parameters_context = f"{method} takes no arguments."
+            class_method_parameters_questions = [
+                f"What arguments do {method} accept?",
+                f"Can you tell me the parameters that {method} requires?",
+                f"What are the inputs for the {method} in {class_member}?",
+                f"Does the {method} need any arguments?",
+                f"What parameters should I pass to {method}?",
+                f"What are required arguments for {method}?",
+            ]
+            class_method_parameters_answers = [
+                f"{method} does not take any parameters.",
+                f"The {method} does not require any parameters.",
+                f"There are no inputs for the {method} in {class_member}.",
+                f"{method} does not need any arguments.",
+                f"No parameters need to be passed to the {method}.",
+                f"{method} does not require any arguments.",
             ]
-            class_member_retrieval_chunks.append(f"{method} takes no arguments.")
-            class_member_tuning_pairs.extend(allocate_tuning_pairs(class_method_parameters_pairs))
+
+            class_member_retrieval_chunks.append(class_method_parameters_context)
+            class_member_tuning_documents.extend(
+                allocate_tuning_triplets(
+                    class_method_parameters_context,
+                    class_method_parameters_questions,
+                    class_method_parameters_answers,
+                )
+            )
         else:
             class_method_parameters = enumerate_array_elements(method_parameters)
-            class_method_parameters_pairs = [
-                (
-                    f"What arguments do {method} accept?",
-                    f"{method} takes the following parameters: {class_method_parameters}.",
-                ),
-                (
-                    f"Can you tell me the parameters that {method} requires?",
-                    f"Sure, {method} requires these parameters: {class_method_parameters}.",
-                ),
-                (
-                    f"I need to know arguments for {method}.",
-                    f"The {method} has these arguments: {class_method_parameters}.",
-                ),
-                (
-                    f"What are the parameters for '{method}'?",
-                    f"The parameters for {method} are: {class_method_parameters}.",
-                ),
-                (
-                    f"Could you list the arguments that the {method} takes?",
-                    f"Certainly, the {method} takes these arguments: {class_method_parameters}.",
-                ),
-            ]
-            class_member_retrieval_chunks.append(
+
+            class_method_parameters_context = (
                 f"{method} accepts following parameters: {class_method_parameters}"
             )
-            class_member_tuning_pairs.extend(allocate_tuning_pairs(class_method_parameters_pairs))
+            class_method_parameters_questions = [
+                f"What arguments do {method} accept?",
+                f"Can you tell me the parameters that {method} requires?",
+                f"I need to know arguments for {method}.",
+                f"What are the parameters for '{method}'?",
+                f"Could you list the arguments that the {method} takes?",
+            ]
+            class_method_parameters_answers = [
+                f"{method} takes the following parameters: {class_method_parameters}.",
+                f"{method} requires these parameters: {class_method_parameters}.",
+                f"The {method} has these arguments: {class_method_parameters}.",
+                f"The parameters for {method} are: {class_method_parameters}.",
+                f"The {method} takes these arguments: {class_method_parameters}.",
+            ]
+
+            class_member_retrieval_chunks.append(class_method_parameters_context)
+            class_member_tuning_documents.extend(
+                allocate_tuning_triplets(
+                    class_method_parameters_context,
+                    class_method_parameters_questions,
+                    class_method_parameters_answers,
+                )
+            )
 
         if not (method_summary := class_method.method_summary):
-            class_method_summary_pairs = [
-                (f"What does {method} do?", f"Docstring of {method} is missing."),
-                (
-                    f"Can you explain functionality of {method}?",
-                    f"The docstring for {method} is not available.",
-                ),
-                (
-                    f"I'm trying to understand what {method} does. Can you help?",
-                    f"Unfortunately, the docstring for {method} is not provided.",
-                ),
-                (
-                    f"Could you describe the role of {method}?",
-                    f"There is no docstring available for {method}.",
-                ),
-                (
-                    f"I'm not sure what {method} does. Can you clarify?",
-                    f"The {method} lacks a docstring.",
-                ),
-                (f"What's the purpose of {method}?", f"The {method} doesn't have a docstring."),
+            class_method_summary_context = f"Unfortunately, {method} is not documented."
+            class_method_summary_questions = [
+                f"What does {method} do?",
+                f"Can you explain functionality of {method}?",
+                f"I'm trying to understand what {method} does. Can you help?",
+                f"Could you describe the role of {method}?",
+                f"I'm not sure what {method} does. Can you clarify?",
+                f"What's the purpose of {method}?",
             ]
-            class_member_retrieval_chunks.append(f"Unfortunately, {method} is not documented.")
-            class_member_tuning_pairs.extend(allocate_tuning_pairs(class_method_summary_pairs))
-        else:
-            class_method_summary_pairs = [
-                (
-                    f"What does {method} do?",
-                    f"Based on method docstring, its role is to '{method_summary}'.",
-                ),
-                (
-                    f"Can you explain the function of {method}?",
-                    f"Sure, according to method docstring, it is designed to '{method_summary}'.",
-                ),
-                (
-                    f"I'm curious about the {method}. What's its purpose?",
-                    f"Well, if we look at the docstring of {method}, we can see that it's meant to"
-                    f" '{method_summary}'.",
-                ),
-                (
-                    f"Could you tell me what the {method} does?",
-                    f"Of course, the docstring of {method} indicates that its function is to"
-                    f" '{method_summary}'.",
-                ),
-                (
-                    f"I'd like to understand role of {method}.",
-                    f"Certainly, method docstring reveals that its job is to '{method_summary}'.",
-                ),
-                (
-                    f"What's the functionality of the {method}?",
-                    f"As per the method docstring, it's designed to '{method_summary}'.",
-                ),
+            class_method_summary_answers = [
+                f"Docstring of {method} is missing.",
+                f"The docstring for {method} is not available.",
+                f"The docstring for {method} is not provided.",
+                f"There is no docstring available for {method}.",
+                f"The {method} lacks a docstring.",
+                f"The {method} doesn't have a docstring.",
             ]
-            class_member_retrieval_chunks.append(
+
+            class_member_retrieval_chunks.append(class_method_summary_context)
+            class_member_tuning_documents.extend(
+                allocate_tuning_triplets(
+                    class_method_summary_context,
+                    class_method_summary_questions,
+                    class_method_summary_answers,
+                )
+            )
+        else:
+            class_method_summary_context = (
                 f"Based on docstring, {method} has the purpose of '{method_summary}'."
             )
-            class_member_tuning_pairs.extend(allocate_tuning_pairs(class_method_summary_pairs))
+            class_method_summary_questions = [
+                f"What does {method} do?",
+                f"Can you explain the function of {method}?",
+                f"I'm curious about the {method}. What's its purpose?",
+                f"Could you tell me what the {method} does?",
+                f"I'd like to understand role of {method}.",
+                f"What's the functionality of the {method}?",
+            ]
+            class_method_summary_answers = [
+                f"Based on method docstring, its role is to '{method_summary}'.",
+                f"According to method docstring, it is designed to '{method_summary}'.",
+                f"If we look at the docstring of {method}, we can see that it's meant to"
+                f" '{method_summary}'.",
+                f"The docstring of {method} indicates that its function is to '{method_summary}'.",
+                f"Method docstring reveals that its job is to '{method_summary}'.",
+                f"As per the method docstring, it's designed to '{method_summary}'.",
+            ]
+
+            class_member_retrieval_chunks.append(class_method_summary_context)
+            class_member_tuning_documents.extend(
+                allocate_tuning_triplets(
+                    class_method_summary_context,
+                    class_method_summary_questions,
+                    class_method_summary_answers,
+                )
+            )
 
     if not (class_attributes := member_type_details.class_attributes):
-        class_attribute_names_pairs = [
-            (
-                f"Are there any public attributes of {class_member}?",
-                f"{class_member} has no public attributes (not starting with '_').",
-            ),
-            (
-                f"Does {class_member} have any public attributes?",
-                f"No, {class_member} does not have any public attributes.",
-            ),
-            (
-                f"Can you tell me if {class_member} has any public attributes?",
-                f"{class_member} does not have any public attributes (not starting with '_').",
-            ),
-            (
-                f"I'm looking for public attributes of {class_member}. Are there any?",
-                f"There are no public attributes (not starting with '_') for {class_member}.",
-            ),
-            (
-                f"Is it possible to find any public attributes in {class_member}?",
-                f"It's not possible to find any public attributes in {class_member}.",
-            ),
-        ]
-        class_member_retrieval_chunks.append(f"{class_member} has no public attributes.")
-        class_member_tuning_pairs.extend(allocate_tuning_pairs(class_attribute_names_pairs))
+        class_attribute_names_context = f"{class_member} has no public attributes."
+        class_attribute_names_questions = [
+            f"Are there any public attributes of {class_member}?",
+            f"Does {class_member} have any public attributes?",
+            f"Can you tell me if {class_member} has any public attributes?",
+            f"I'm looking for public attributes of {class_member}. Are there any?",
+            f"Is it possible to find any public attributes in {class_member}?",
+        ]
+        class_attribute_names_answers = [
+            f"{class_member} has no public attributes (not starting with '_').",
+            f"{class_member} does not have any public attributes.",
+            f"{class_member} does not have any public attributes (not starting with '_').",
+            f"There are no public attributes (not starting with '_') for {class_member}.",
+            f"It's not possible to find any public attributes in {class_member}.",
+        ]
+
+        class_member_retrieval_chunks.append(class_attribute_names_context)
+        class_member_tuning_documents.extend(
+            allocate_tuning_triplets(
+                class_attribute_names_context,
+                class_attribute_names_questions,
+                class_attribute_names_answers,
+            )
+        )
     else:
         class_attributes_count = len(class_attributes)
-        class_attributes_count_pairs = [
-            (
-                f"How many public attributes does {class_member} have?",
-                f"{class_member} has {class_attributes_count} many public attributes.",
-            ),
-            (
-                f"What is the count of public attributes in {class_member}?",
-                f"The count of public attributes in {class_member} is {class_attributes_count}.",
-            ),
-            (
-                f"Could you tell me the number of public attributes in {class_member}?",
-                f"{class_member} has {class_attributes_count} public attributes.",
-            ),
-            (
-                f"Please provide the count of public attributes for {class_member}.",
-                f"Number of public attributes in {class_member} is {class_attributes_count}.",
-            ),
-            (
-                f"Tell me the quantity of public attributes present in {class_member}.",
-                f"{class_member} has {class_attributes_count} public attributes.",
-            ),
-            (
-                f"Would you mind letting me know how many public attributes {class_member}"
-                " contains?",
-                f"{class_member} contains {class_attributes_count} public attributes.",
-            ),
-        ]
-        class_member_retrieval_chunks.append(
+
+        class_attributes_count_context = (
             f"{class_member} has {class_attributes_count} many public attributes."
         )
-        class_member_tuning_pairs.extend(allocate_tuning_pairs(class_attributes_count_pairs))
+        class_attributes_count_questions = [
+            f"How many public attributes does {class_member} have?",
+            f"What is the count of public attributes in {class_member}?",
+            f"Could you tell me the number of public attributes in {class_member}?",
+            f"Please provide the count of public attributes for {class_member}.",
+            f"Tell me the quantity of public attributes present in {class_member}.",
+            f"Would you mind letting me know how many public attributes {class_member} contains?",
+        ]
+        class_attributes_count_answers = [
+            f"{class_member} has {class_attributes_count} many public attributes.",
+            f"The count of public attributes in {class_member} is {class_attributes_count}.",
+            f"{class_member} has {class_attributes_count} public attributes.",
+            f"Number of public attributes in {class_member} is {class_attributes_count}.",
+            f"{class_member} has {class_attributes_count} public attributes.",
+            f"{class_member} contains {class_attributes_count} public attributes.",
+        ]
+
+        class_member_retrieval_chunks.append(class_attributes_count_context)
+        class_member_tuning_documents.extend(
+            allocate_tuning_triplets(
+                class_attributes_count_context,
+                class_attributes_count_questions,
+                class_attributes_count_answers,
+            )
+        )
 
         class_public_attributes = enumerate_array_elements(
             class_attributes, attribute="attribute_name"
         )
-        class_attribute_names_pairs = [
-            (
-                f"Are there any public attributes of {class_member}?",
-                f"These are the public attributes of {class_member}: {class_public_attributes}.",
-            ),
-            (
-                f"Can you list the public attributes of {class_member}?",
-                f"{class_member} has the following public attributes (not starting with '_'):"
-                f" {class_public_attributes}.",
-            ),
-            (
-                f"What are the public attributes of {class_member}?",
-                f"The public attributes of {class_member} (those not starting with '_') are:"
-                f" {class_public_attributes}.",
-            ),
-            (
-                f"I need to know the public attributes of {class_member}.",
-                f"Sure, the public attributes of {class_member} are: {class_public_attributes}.",
-            ),
-            (
-                f"Could you tell me the public attributes of {class_member}?",
-                f"Of course, public attributes of {class_member} (not starting with '_') are:"
-                f" {class_public_attributes}.",
-            ),
-        ]
-        class_member_retrieval_chunks.append(
+
+        class_attribute_names_context = (
             f"{class_member} has following public attributes: {class_public_attributes}"
         )
-        class_member_tuning_pairs.extend(allocate_tuning_pairs(class_attribute_names_pairs))
+        class_attribute_names_questions = [
+            f"Are there any public attributes of {class_member}?",
+            f"Can you list the public attributes of {class_member}?",
+            f"What are the public attributes of {class_member}?",
+            f"I need to know the public attributes of {class_member}.",
+            f"Could you tell me the public attributes of {class_member}?",
+        ]
+        class_attribute_names_answers = [
+            f"These are the public attributes of {class_member}: {class_public_attributes}.",
+            f"{class_member} has the following public attributes (not starting with '_'):"
+            f" {class_public_attributes}.",
+            f"The public attributes of {class_member} (those not starting with '_') are:"
+            f" {class_public_attributes}.",
+            f"The public attributes of {class_member} are: {class_public_attributes}.",
+            f"Public attributes of {class_member} (not starting with '_') are:"
+            f" {class_public_attributes}.",
+        ]
+
+        class_member_retrieval_chunks.append(class_attribute_names_context)
+        class_member_tuning_documents.extend(
+            allocate_tuning_triplets(
+                class_attribute_names_context,
+                class_attribute_names_questions,
+                class_attribute_names_answers,
+            )
+        )
 
     if not (class_summary := member_type_details.class_summary):
-        class_summary_pairs = [
-            (
-                f"What does {class_member} do in short?",
-                f"Docstring of {class_member} lacks a summary of its objective.",
-            ),
-            (
-                f"Can you briefly explain the function of {class_member}?",
-                f"Docstring of {class_member} doesn't provide a concise summary of its purpose.",
-            ),
-            (
-                f"Could you tell me what {class_member} is used for?",
-                f"Unfortunately, the docstring of {class_member} doesn't contain"
-                " a brief description of its function.",
-            ),
-            (
-                f"I'm not sure what {class_member} does. Can you clarify?",
-                f"The docstring of {class_member} doesn't succinctly explain its role.",
-            ),
-            (
-                f"What's the purpose of {class_member}?",
-                f"Docstring of {class_member} doesn't have any explanation of its objective.",
-            ),
-        ]
-        class_member_retrieval_chunks.append(
-            f"Unfortunately, {class_member} does not document its objective."
-        )
-        class_member_tuning_pairs.extend(allocate_tuning_pairs(class_summary_pairs))
-    else:
-        class_summary_pairs = [
-            (
-                f"What does {class_member} do in short?",
-                f"Based on documentation, objective of {class_member} is to: '{class_summary}'.",
-            ),
-            (
-                f"Can you briefly explain the function of {class_member}?",
-                f"Sure, according to the documentation, {class_member} is designed to:"
-                f" '{class_summary}'.",
-            ),
-            (
-                f"I'm curious about {class_member}, what's its purpose?",
-                f"Well, as per the documentation, {class_member} aims to: '{class_summary}'.",
-            ),
-            (
-                f"Could you give me a quick rundown on what {class_member} does?",
-                f"Absolutely, the documentation states that the role of {class_member} is to:"
-                f" '{class_summary}'.",
-            ),
-            (
-                f"What's the role of {class_member} in a nutshell?",
-                f"The documentation indicates that the purpose of {class_member} is to:"
-                f" '{class_summary}'.",
-            ),
-            (
-                f"Can you summarise the function of {class_member}?",
-                f"Of course, the documentation outlines that {class_member} is intended to:"
-                f" '{class_summary}'.",
-            ),
-        ]
-        class_member_retrieval_chunks.append(
+        class_summary_context = f"Unfortunately, {class_member} does not document its objective."
+        class_summary_questions = [
+            f"What does {class_member} do in short?",
+            f"Can you briefly explain the function of {class_member}?",
+            f"Could you tell me what {class_member} is used for?",
+            f"I'm not sure what {class_member} does. Can you clarify?",
+            f"What's the purpose of {class_member}?",
+        ]
+        class_summary_answers = [
+            f"Docstring of {class_member} lacks a summary of its objective.",
+            f"Docstring of {class_member} doesn't provide a concise summary of its purpose.",
+            f"The docstring of {class_member} doesn't contain"
+            " a brief description of its function.",
+            f"The docstring of {class_member} doesn't succinctly explain its role.",
+            f"Docstring of {class_member} doesn't have any explanation of its objective.",
+        ]
+
+        class_member_retrieval_chunks.append(class_summary_context)
+        class_member_tuning_documents.extend(
+            allocate_tuning_triplets(
+                class_summary_context, class_summary_questions, class_summary_answers
+            )
+        )
+    else:
+        class_summary_context = (
             f"{class_member} documents its purpose as follows: '{class_summary}'."
         )
-        class_member_tuning_pairs.extend(allocate_tuning_pairs(class_summary_pairs))
+        class_summary_questions = [
+            f"What does {class_member} do in short?",
+            f"Can you briefly explain the function of {class_member}?",
+            f"I'm curious about {class_member}, what's its purpose?",
+            f"Could you give me a quick rundown on what {class_member} does?",
+            f"What's the role of {class_member} in a nutshell?",
+            f"Can you summarise the function of {class_member}?",
+        ]
+        class_summary_answers = [
+            f"Based on documentation, objective of {class_member} is to: '{class_summary}'.",
+            f"According to the documentation, {class_member} is designed to: '{class_summary}'.",
+            f"As per the documentation, {class_member} aims to: '{class_summary}'.",
+            f"The documentation states that the role of {class_member} is to: '{class_summary}'.",
+            f"The documentation indicates that the purpose of {class_member} is to:"
+            f" '{class_summary}'.",
+            f"The documentation outlines that {class_member} is intended to: '{class_summary}'.",
+        ]
+
+        class_member_retrieval_chunks.append(class_summary_context)
+        class_member_tuning_documents.extend(
+            allocate_tuning_triplets(
+                class_summary_context, class_summary_questions, class_summary_answers
+            )
+        )
 
     if not (class_notes := member_type_details.class_notes):
-        class_notes_pairs = [
-            (
-                f"Mention any specific details for {class_member} to be aware of.",
-                f"Docstring of {class_member} does not note on specific details.",
-            ),
-            (
-                f"What are the specific details to be aware of for {class_member}?",
-                f"There are no specific details noted in the docstring of {class_member}.",
-            ),
-            (
-                f"Could you tell me any specifics for {class_member} that I should be aware of?",
-                f"The docstring of {class_member} doesn't highlight any details.",
-            ),
-            (
-                f"Are there any specific details for {class_member} that I need to know?",
-                f"No specific details are mentioned in the docstring of {class_member}.",
-            ),
-            (
-                f"I need to know the specific details for {class_member}. Can you provide them?",
-                f"Unfortunately, the docstring of {class_member} does not contain any details.",
-            ),
-            (
-                f"Can you specify any details for {class_member} that I should be aware of?",
-                f"The docstring of {class_member} does not specify any details to be aware of.",
-            ),
-        ]
-        class_member_retrieval_chunks.append(
+        class_notes_context = (
             f"Docstring of {class_member} has contains no specific implementation details."
         )
-        class_member_tuning_pairs.extend(allocate_tuning_pairs(class_notes_pairs))
+        class_notes_questions = [
+            f"Mention any specific details for {class_member} to be aware of.",
+            f"What are the specific details to be aware of for {class_member}?",
+            f"Could you tell me any specifics for {class_member} that I should be aware of?",
+            f"Are there any specific details for {class_member} that I need to know?",
+            f"I need to know the specific details for {class_member}. Can you provide them?",
+            f"Can you specify any details for {class_member} that I should be aware of?",
+        ]
+        class_notes_answers = [
+            f"Docstring of {class_member} does not note on specific details.",
+            f"There are no specific details noted in the docstring of {class_member}.",
+            f"The docstring of {class_member} doesn't highlight any details.",
+            f"No specific details are mentioned in the docstring of {class_member}.",
+            f"The docstring of {class_member} does not contain any details.",
+            f"The docstring of {class_member} does not specify any details to be aware of.",
+        ]
+
+        class_member_retrieval_chunks.append(class_notes_context)
+        class_member_tuning_documents.extend(
+            allocate_tuning_triplets(
+                class_notes_context, class_notes_questions, class_notes_answers
+            )
+        )
     else:
-        class_notes_pairs = [
-            (
-                f"Mention any specific details for {class_member} to be aware of.",
-                f"The {class_member} docstring highlights the following: '{class_notes}'.",
-            ),
-            (
-                f"What are specifics that I should be aware of before using {class_member}?",
-                f"The details you should know to use {class_member} are highlighted in docstring:"
-                f" '{class_notes}'.",
-            ),
-            (
-                f"Could you specify the details for {class_member} to take note of?",
-                f"Sure, the docstring for {class_member} specifies the following details:"
-                f" '{class_notes}'.",
-            ),
-            (
-                f"Can you list the details for {class_member} to keep in mind?",
-                f"Certainly, the docstring for {class_member} lists the following details:"
-                f" '{class_notes}'.",
-            ),
-            (
-                f"What should users of {class_member} be mindful of?",
-                f"The docstring for {class_member} mentions the following points to be mindful of:"
-                f" '{class_notes}'.",
-            ),
-            (
-                f"What details does the user of {class_member} need to know?",
-                f"User of {class_member} needs to know the following details: '{class_notes}'.",
-            ),
-        ]
-        class_member_retrieval_chunks.append(
+        class_notes_context = (
             f"In docstring, {class_member} specifies the following: '{class_notes}'."
         )
-        class_member_tuning_pairs.extend(allocate_tuning_pairs(class_notes_pairs))
+        class_notes_questions = [
+            f"Mention any specific details for {class_member} to be aware of.",
+            f"What are specifics that I should be aware of before using {class_member}?",
+            f"Could you specify the details for {class_member} to take note of?",
+            f"Can you list the details for {class_member} to keep in mind?",
+            f"What should users of {class_member} be mindful of?",
+            f"What details does the user of {class_member} need to know?",
+        ]
+        class_notes_answers = [
+            f"The {class_member} docstring highlights the following: '{class_notes}'.",
+            f"The details you should know to use {class_member} are highlighted in docstring:"
+            f" '{class_notes}'.",
+            f"The docstring for {class_member} specifies the following details: '{class_notes}'.",
+            f"The docstring for {class_member} lists the following details: '{class_notes}'.",
+            f"The docstring for {class_member} mentions the following points to be mindful of:"
+            f" '{class_notes}'.",
+            f"User of {class_member} needs to know the following details: '{class_notes}'.",
+        ]
+
+        class_member_retrieval_chunks.append(class_notes_context)
+        class_member_tuning_documents.extend(
+            allocate_tuning_triplets(
+                class_notes_context, class_notes_questions, class_notes_answers
+            )
+        )
 
     class_member_dataset = Dataset(
-        retrieval_chunks=class_member_retrieval_chunks[:2], tuning_pairs=class_member_tuning_pairs
+        retrieval_chunks=class_member_retrieval_chunks[:2],
+        tuning_documents=class_member_tuning_documents,
     )
 
     return class_member_dataset, class_member_retrieval_chunks
 
 
 @pydantic.validate_call(validate_return=True)
 def generate_function_member_dataset(  # noqa: C901, PLR0912, PLR0915
@@ -1876,856 +1720,766 @@
     list[str]
         only retrieval documents
     """
     function_member_retrieval_chunks: list[str] = [
         f"{function_member} is a Python function.",
         f"{function_member} has following docstring: {function_docstring}.",
     ]
-    function_member_tuning_pairs: list[tuple[str, str, SplitName]] = []
+    function_member_tuning_documents: list[Document] = []
 
     if not (function_parameters := member_type_details.function_parameters):
-        function_parameters_pairs = [
-            (
-                f"List various parameters of {function_member}.",
-                f"{function_member} does not take any parameters.",
-            ),
-            (
-                f"What are the parameters of {function_member}?",
-                f"{function_member} has no parameters.",
-            ),
-            (
-                f"Could you tell me the parameters that {function_member} takes?",
-                f"{function_member} doesn't require any parameters.",
-            ),
-            (
-                f"I need to know the parameters for {function_member}.",
-                f"There are no parameters for {function_member}.",
-            ),
-            (
-                f"Can you list the parameters for {function_member}?",
-                f"Actually, {function_member} doesn't have any parameters.",
-            ),
-            (
-                f"Please provide the parameters of {function_member}.",
-                f"Sorry, but {function_member} does not have any parameters.",
-            ),
-        ]
-        function_member_retrieval_chunks.append(f"{function_member} takes no parameters.")
-        function_member_tuning_pairs.extend(allocate_tuning_pairs(function_parameters_pairs))
+        function_parameters_context = f"{function_member} takes no parameters."
+        function_parameters_questions = [
+            f"List various parameters of {function_member}.",
+            f"What are the parameters of {function_member}?",
+            f"Could you tell me the parameters that {function_member} takes?",
+            f"I need to know the parameters for {function_member}.",
+            f"Can you list the parameters for {function_member}?",
+            f"Please provide the parameters of {function_member}.",
+        ]
+        function_parameters_answers = [
+            f"{function_member} does not take any parameters.",
+            f"{function_member} has no parameters.",
+            f"{function_member} doesn't require any parameters.",
+            f"There are no parameters for {function_member}.",
+            f"Actually, {function_member} doesn't have any parameters.",
+            f"Sorry, but {function_member} does not have any parameters.",
+        ]
+
+        function_member_retrieval_chunks.append(function_parameters_context)
+        function_member_tuning_documents.extend(
+            allocate_tuning_triplets(
+                function_parameters_context,
+                function_parameters_questions,
+                function_parameters_answers,
+            )
+        )
     else:
         function_parameter_names = enumerate_array_elements(
             function_parameters, attribute="parameter_details"
         )
-        function_parameters_pairs = [
-            (
-                f"List various parameters of {function_member}.",
-                f"Different parameters of {function_member} are as follows:"
-                f" {function_parameter_names}.",
-            ),
-            (
-                f"What are the different parameters of {function_member}?",
-                f"{function_member} has the following parameters: {function_parameter_names}.",
-            ),
-            (
-                f"Could you tell me the parameters of {function_member}?",
-                f"Sure, the parameters of {function_member} are: {function_parameter_names}.",
-            ),
-            (
-                f"I need to know the parameters of {function_member}.",
-                f"The parameters of {function_member} are: {function_parameter_names}.",
-            ),
-            (
-                f"Can you list the parameters for {function_member}?",
-                f"Yes, the parameters for {function_member} are: {function_parameter_names}.",
-            ),
-            (
-                f"Please provide the parameters of {function_member}.",
-                f"Parameters of {function_member} are as follows: {function_parameter_names}.",
-            ),
-        ]
-        function_member_retrieval_chunks.append(
+
+        function_parameters_context = (
             f"{function_member} takes the following parameters: {function_parameter_names}"
         )
-        function_member_tuning_pairs.extend(allocate_tuning_pairs(function_parameters_pairs))
+        function_parameters_questions = [
+            f"List various parameters of {function_member}.",
+            f"What are the different parameters of {function_member}?",
+            f"Could you tell me the parameters of {function_member}?",
+            f"I need to know the parameters of {function_member}.",
+            f"Can you list the parameters for {function_member}?",
+            f"Please provide the parameters of {function_member}.",
+        ]
+        function_parameters_answers = [
+            f"Different parameters of {function_member} are as follows:"
+            f" {function_parameter_names}.",
+            f"{function_member} has the following parameters: {function_parameter_names}.",
+            f"The parameters of {function_member} are: {function_parameter_names}.",
+            f"Yes, the parameters for {function_member} are: {function_parameter_names}.",
+            f"Parameters of {function_member} are as follows: {function_parameter_names}.",
+        ]
+
+        function_member_retrieval_chunks.append(function_parameters_context)
+        function_member_tuning_documents.extend(
+            allocate_tuning_triplets(
+                function_parameters_context,
+                function_parameters_questions,
+                function_parameters_answers,
+            )
+        )
 
     for function_parameter in function_parameters:
         parameter_name = function_parameter.parameter_name
         parameter = f"'{parameter_name}' argument in {function_member}"
 
-        if (parameter_default := function_parameter.parameter_default) is inspect._empty:
-            function_parameter_defaults_pairs = [
-                (f"Default value of {parameter}?", f"{parameter} does not have a default value."),
-                (
-                    f"What is the default value for {parameter}?",
-                    f"The {parameter} does not come with a default value.",
-                ),
-                (
-                    f"Could you tell me default value of {parameter}?",
-                    f"Sure, the {parameter} does not possess a default value.",
-                ),
-                (
-                    f"I'm curious about default value of {parameter}.",
-                    f"In response to your curiosity, {parameter} is not assigned a default value.",
-                ),
-                (
-                    f"I'd like to know the default value of {parameter}.",
-                    f"To answer your query, {parameter} does not hold a default value.",
-                ),
-                (
-                    f"Can you inform me about the default value of {parameter}?",
-                    f"Certainly, {parameter} does not contain a default value.",
-                ),
-            ]
-            function_member_retrieval_chunks.append(f"{parameter} has no default value.")
-            function_member_tuning_pairs.extend(
-                allocate_tuning_pairs(function_parameter_defaults_pairs)
+        if (parameter_default := function_parameter.parameter_default) is EMPTY_PARAMETER:
+            function_parameter_defaults_context = f"{parameter} has no default value."
+            function_parameter_defaults_questions = [
+                f"Default value of {parameter}?",
+                f"What is the default value for {parameter}?",
+                f"Could you tell me default value of {parameter}?",
+                f"I'm curious about default value of {parameter}.",
+                f"I'd like to know the default value of {parameter}.",
+                f"Can you inform me about the default value of {parameter}?",
+            ]
+            function_parameter_defaults_answers = [
+                f"{parameter} does not have a default value."
+                f"The {parameter} does not come with a default value.",
+                f"The {parameter} does not possess a default value.",
+                f"In response to your curiosity, {parameter} is not assigned a default value.",
+                f"To answer your query, {parameter} does not hold a default value.",
+                f"{parameter} does not contain a default value.",
+            ]
+
+            function_member_retrieval_chunks.append(function_parameter_defaults_context)
+            function_member_tuning_documents.extend(
+                allocate_tuning_triplets(
+                    function_parameter_defaults_context,
+                    function_parameter_defaults_questions,
+                    function_parameter_defaults_answers,
+                )
             )
         else:
-            function_parameter_defaults_pairs = [
-                (
-                    f"Default value of {parameter}?",
-                    f"{parameter} has default value of {parameter_default}.",
-                ),
-                (
-                    f"What is the default value for {parameter}?",
-                    f"The default value for {parameter} is {parameter_default}.",
-                ),
-                (
-                    f"Could you tell me default value of {parameter}?",
-                    f"Sure, the default value of {parameter} is {parameter_default}.",
-                ),
-                (
-                    f"I would like to know the default value of {parameter}.",
-                    f"The {parameter} has a default value of {parameter_default}.",
-                ),
-                (
-                    f"Can you inform me about the default value of {parameter}?",
-                    f"Of course, the {parameter} defaults to {parameter_default}.",
-                ),
-                (
-                    f"I'm interested in default value of {parameter}.",
-                    f"The default value of the {parameter} is {parameter_default}.",
-                ),
-            ]
-            function_member_retrieval_chunks.append(
+            function_parameter_defaults_context = (
                 f"{parameter} has the default value of {parameter_default}."
             )
-            function_member_tuning_pairs.extend(
-                allocate_tuning_pairs(function_parameter_defaults_pairs)
+            function_parameter_defaults_questions = [
+                f"Default value of {parameter}?",
+                f"What is the default value for {parameter}?",
+                f"Could you tell me default value of {parameter}?",
+                f"I would like to know the default value of {parameter}.",
+                f"Can you inform me about the default value of {parameter}?",
+                f"I'm interested in default value of {parameter}.",
+            ]
+            function_parameter_defaults_answers = [
+                f"{parameter} has default value of {parameter_default}.",
+                f"The default value for {parameter} is {parameter_default}.",
+                f"The default value of {parameter} is {parameter_default}.",
+                f"The {parameter} has a default value of {parameter_default}.",
+                f"The {parameter} defaults to {parameter_default}.",
+                f"The default value of the {parameter} is {parameter_default}.",
+            ]
+
+            function_member_retrieval_chunks.append(function_parameter_defaults_context)
+            function_member_tuning_documents.extend(
+                allocate_tuning_triplets(
+                    function_parameter_defaults_context,
+                    function_parameter_defaults_questions,
+                    function_parameter_defaults_answers,
+                )
             )
 
-        if (parameter_annotation := function_parameter.parameter_annotation) is inspect._empty:
-            function_parameter_types_pairs = [
-                (
-                    f"What is type annotation of {parameter}?",
-                    f"{parameter} does not have a type annotation.",
-                ),
-                (
-                    f"Can you tell me type annotation of {parameter}?",
-                    f"The {parameter} does not have a type annotation.",
-                ),
-                (
-                    f"I'm curious about the type annotation of {parameter}."
-                    " Can you provide some information?",
-                    f"Sure, the {parameter} does not have a type annotation.",
-                ),
-                (
-                    f"Do you have any information on the type annotation of {parameter}?",
-                    f"Yes, the {parameter} does not have a type annotation.",
-                ),
-                (
-                    f"Could you inform me about the type annotation of {parameter}?",
-                    f"Certainly, {parameter} does not have a type annotation.",
-                ),
-                (
-                    f"I'd like to know the type annotation of {parameter}.",
-                    f"The {parameter} you're asking about does not have a type annotation.",
-                ),
-            ]
-            function_member_retrieval_chunks.append(
+        if (parameter_annotation := function_parameter.parameter_annotation) is EMPTY_PARAMETER:
+            function_parameter_types_context = (
                 f"Unfortunately, type hint for {parameter} is missing."
             )
-            function_member_tuning_pairs.extend(
-                allocate_tuning_pairs(function_parameter_types_pairs)
+            function_parameter_types_questions = [
+                f"What is type annotation of {parameter}?",
+                f"Can you tell me type annotation of {parameter}?",
+                f"I'm curious about the type annotation of {parameter}."
+                " Can you provide some information?",
+                f"Do you have any information on the type annotation of {parameter}?",
+                f"Could you inform me about the type annotation of {parameter}?",
+                f"I'd like to know the type annotation of {parameter}.",
+            ]
+            function_parameter_types_answers = [
+                f"{parameter} does not have a type annotation.",
+                f"The {parameter} does not have a type annotation.",
+                f"{parameter} does not have a type annotation.",
+                f"The {parameter} you're asking about does not have a type annotation.",
+            ]
+
+            function_member_retrieval_chunks.append(function_parameter_types_context)
+            function_member_tuning_documents.extend(
+                allocate_tuning_triplets(
+                    function_parameter_types_context,
+                    function_parameter_types_questions,
+                    function_parameter_types_answers,
+                )
             )
         else:
-            function_parameter_types_pairs = [
-                (
-                    f"What is type annotation of {parameter}?",
-                    f"Type annotation of {parameter} is '{parameter_annotation}'.",
-                ),
-                (
-                    f"Can you tell me type annotation of {parameter}?",
-                    f"Sure, the type annotation of {parameter} is '{parameter_annotation}'.",
-                ),
-                (
-                    f"I'm curious about the type annotation of {parameter}. What is it?",
-                    f"The type annotation of {parameter} is '{parameter_annotation}'.",
-                ),
-                (
-                    f"Do you know type annotation of {parameter}?",
-                    f"Yes, the type annotation of {parameter} is '{parameter_annotation}'.",
-                ),
-                (
-                    f"Could you inform me about the type annotation of {parameter}?",
-                    f"Of course, the type annotation of {parameter} is '{parameter_annotation}'.",
-                ),
-                (
-                    f"What's the type annotation for {parameter}?",
-                    f"The type annotation for {parameter} is '{parameter_annotation}'.",
-                ),
-            ]
-            function_member_retrieval_chunks.append(
+            function_parameter_types_context = (
                 f"{parameter} has '{parameter_annotation}' as type annotation."
             )
-            function_member_tuning_pairs.extend(
-                allocate_tuning_pairs(function_parameter_types_pairs)
+            function_parameter_types_questions = [
+                f"What is type annotation of {parameter}?",
+                f"Can you tell me type annotation of {parameter}?",
+                f"I'm curious about the type annotation of {parameter}. What is it?",
+                f"Do you know type annotation of {parameter}?",
+                f"Could you inform me about the type annotation of {parameter}?",
+                f"What's the type annotation for {parameter}?",
+            ]
+            function_parameter_types_answers = [
+                f"Type annotation of {parameter} is '{parameter_annotation}'.",
+                f"The type annotation of {parameter} is '{parameter_annotation}'.",
+                f"The type annotation for {parameter} is '{parameter_annotation}'.",
+            ]
+
+            function_member_retrieval_chunks.append(function_parameter_types_context)
+            function_member_tuning_documents.extend(
+                allocate_tuning_triplets(
+                    function_parameter_types_context,
+                    function_parameter_types_questions,
+                    function_parameter_types_answers,
+                )
             )
 
         if not (parameter_summary := function_parameter.parameter_summary):
-            function_parameter_summary_pairs = [
-                (
-                    f"What is {parameter} for?",
-                    f"Docstring of {function_member} lacks a description for '{parameter_name}'.",
-                ),
-                (
-                    f"Can you explain the purpose of {parameter}?",
-                    f"The docstring of {function_member} doesn't provide a description.",
-                ),
-                (
-                    f"I'm not sure what {parameter} does. Can you help?",
-                    f"Unfortunately, the docstring of {function_member} doesn't include"
-                    " a description.",
-                ),
-                (
-                    f"Could you clarify the role of {parameter}?",
-                    f"The description is missing in the docstring of {function_member}.",
-                ),
-                (
-                    f"I'm confused about the {parameter}. What does it do?",
-                    f"The docstring of {function_member} doesn't contain a description.",
-                ),
-                (
-                    f"What does {parameter} do?",
-                    f"There's no description in the docstring of {function_member}.",
-                ),
+            function_parameter_summary_context = f"{parameter} is not documented in the docstring."
+            function_parameter_summary_questions = [
+                f"What is {parameter} for?",
+                f"Can you explain the purpose of {parameter}?",
+                f"I'm not sure what {parameter} does. Can you help?",
+                f"Could you clarify the role of {parameter}?",
+                f"I'm confused about the {parameter}. What does it do?",
+                f"What does {parameter} do?",
             ]
-            function_member_retrieval_chunks.append(
-                f"{parameter} is not documented in the docstring."
-            )
-            function_member_tuning_pairs.extend(
-                allocate_tuning_pairs(function_parameter_summary_pairs)
+            function_parameter_summary_answers = [
+                f"Docstring of {function_member} lacks a description for '{parameter_name}'.",
+                f"The docstring of {function_member} doesn't provide a description.",
+                f"Unfortunately, the docstring of {function_member} doesn't include"
+                " a description.",
+                f"The description is missing in the docstring of {function_member}.",
+                f"The docstring of {function_member} doesn't contain a description.",
+                f"There's no description in the docstring of {function_member}.",
+            ]
+
+            function_member_retrieval_chunks.append(function_parameter_summary_context)
+            function_member_tuning_documents.extend(
+                allocate_tuning_triplets(
+                    function_parameter_summary_context,
+                    function_parameter_summary_questions,
+                    function_parameter_summary_answers,
+                )
             )
         else:
-            function_parameter_summary_pairs = [
-                (
-                    f"What is {parameter} for?",
-                    f"Based on {function_member} docstring, its role is '{parameter_summary}'.",
-                ),
-                (
-                    f"Can you explain the role of {parameter}?",
-                    f"Sure, according to the docstring of {function_member},"
-                    f" '{parameter_name}' is used for '{parameter_summary}'.",
-                ),
-                (
-                    f"I'm curious about the {parameter}. What does it do?",
-                    f"Well, if you look at the docstring of {function_member}, you'll see that"
-                    f" '{parameter_name}' is responsible for '{parameter_summary}'.",
-                ),
-                (
-                    f"Could you tell me the purpose of {parameter}?",
-                    f"Of course, the docstring of {function_member} indicates that"
-                    f" '{parameter_name}' serves the purpose of '{parameter_summary}'.",
-                ),
-                (
-                    f"What's the function of {parameter}?",
-                    f"As per the docstring of {function_member}, '{parameter_name}' functions as:"
-                    f" '{parameter_summary}'.",
-                ),
-                (
-                    f"I'd like to know what '{parameter_name}' does in {function_member}.",
-                    f"Sure thing, the docstring of {function_member} states that"
-                    f" '{parameter_name}' does '{parameter_summary}'.",
-                ),
-            ]
-            function_member_retrieval_chunks.append(
+            function_parameter_summary_context = (
                 f"In the docstring, {parameter} is described as '{parameter_summary}'."
             )
-            function_member_tuning_pairs.extend(
-                allocate_tuning_pairs(function_parameter_summary_pairs)
+            function_parameter_summary_questions = [
+                f"What is {parameter} for?",
+                f"Can you explain the role of {parameter}?",
+                f"I'm curious about the {parameter}. What does it do?",
+                f"Could you tell me the purpose of {parameter}?",
+                f"What's the function of {parameter}?",
+                f"I'd like to know what '{parameter_name}' does in {function_member}.",
+            ]
+            function_parameter_summary_answers = [
+                f"Based on {function_member} docstring, its role is '{parameter_summary}'.",
+                f"According to the docstring of {function_member},"
+                f"'{parameter_name}' is used for '{parameter_summary}'.",
+                f"If you look at the docstring of {function_member}, you'll see that"
+                f" '{parameter_name}' is responsible for '{parameter_summary}'.",
+                f"The docstring of {function_member} indicates that"
+                f" '{parameter_name}' serves the purpose of '{parameter_summary}'.",
+                f"As per the docstring of {function_member}, '{parameter_name}' functions as:"
+                f" '{parameter_summary}'.",
+                f"The docstring of {function_member} states that"
+                f" '{parameter_name}' does '{parameter_summary}'.",
+            ]
+
+            function_member_retrieval_chunks.append(function_parameter_summary_context)
+            function_member_tuning_documents.extend(
+                allocate_tuning_triplets(
+                    function_parameter_summary_context,
+                    function_parameter_summary_questions,
+                    function_parameter_summary_answers,
+                )
             )
 
     if (
         returns_annotation := member_type_details.function_returns.returns_annotation
-    ) is inspect._empty:
-        function_return_type_pairs = [
-            (
-                f"What is the return type annotation of {function_member}?",
-                f"{function_member} lacks a return type annotation. It may still return though.",
-            ),
-            (
-                f"Can you tell me the return type annotation of {function_member}?",
-                f"The function {function_member} does not have a return type annotation."
-                " However, it may still return.",
-            ),
-            (
-                f"I'm curious about return type annotation of {function_member}. What is it?",
-                f"Well, {function_member} doesn't have a return type annotation."
-                " But, it could still return.",
-            ),
-            (
-                f"Do you know the return type annotation of {function_member}?",
-                f"Actually, {function_member} doesn't come with a return type annotation."
-                " It's possible that it still returns though.",
-            ),
-            (
-                f"Could you inform me about the return type annotation of {function_member}?",
-                f"Sure, {function_member} is missing a return type annotation."
-                " It might still return though.",
-            ),
-            (
-                f"What's the return type annotation for {function_member}?",
-                f"It appears that {function_member} is without a return type annotation."
-                " It may still have a return.",
-            ),
-        ]
-        function_member_retrieval_chunks.append(
+    ) is EMPTY_SIGNATURE:
+        function_return_type_context = (
             f"{function_member} has no return annotation, but its return can still be non-null."
         )
-        function_member_tuning_pairs.extend(allocate_tuning_pairs(function_return_type_pairs))
+        function_return_type_questions = [
+            f"What is the return type annotation of {function_member}?",
+            f"Can you tell me the return type annotation of {function_member}?",
+            f"I'm curious about return type annotation of {function_member}. What is it?",
+            f"Do you know the return type annotation of {function_member}?",
+            f"Could you inform me about the return type annotation of {function_member}?",
+            f"What's the return type annotation for {function_member}?",
+        ]
+        function_return_type_answers = [
+            f"{function_member} lacks a return type annotation. It may still return though.",
+            f"The function {function_member} does not have a return type annotation."
+            " However, it may still return.",
+            f"{function_member} doesn't have a return type annotation."
+            " But, it could still return.",
+            f"Actually, {function_member} doesn't come with a return type annotation."
+            " It's possible that it still returns though.",
+            f"Sure, {function_member} is missing a return type annotation."
+            " It might still return though.",
+            f"It appears that {function_member} is without a return type annotation."
+            " It may still have a return.",
+        ]
+
+        function_member_retrieval_chunks.append(function_return_type_context)
+        function_member_tuning_documents.extend(
+            allocate_tuning_triplets(
+                function_return_type_context,
+                function_return_type_questions,
+                function_return_type_answers,
+            )
+        )
     else:
-        function_return_type_pairs = [
-            (
-                f"What is the return type annotation of {function_member}?",
-                f"Return type annotation for {function_member} is '{returns_annotation}'.",
-            ),
-            (
-                f"Can you tell me the return type annotation of {function_member}?",
-                f"Sure, return type annotation for {function_member} is '{returns_annotation}'.",
-            ),
-            (
-                f"I need to know the return type annotation of {function_member}.",
-                f"The return type annotation for {function_member} is '{returns_annotation}'.",
-            ),
-            (
-                f"Do you know the return type annotation of {function_member}?",
-                f"Yes, return type annotation for {function_member} is '{returns_annotation}'.",
-            ),
-            (
-                f"Could you inform me about the return type annotation of {function_member}?",
-                f"Of course, the return type for {function_member} is '{returns_annotation}'.",
-            ),
-            (
-                f"I'm curious about the return type annotation of {function_member}.",
-                f"The return type annotation for {function_member} is '{returns_annotation}'.",
-            ),
-        ]
-        function_member_retrieval_chunks.append(
+        function_return_type_context = (
             f"Return of {function_member} is annotated as '{returns_annotation}'."
         )
-        function_member_tuning_pairs.extend(allocate_tuning_pairs(function_return_type_pairs))
+        function_return_type_questions = [
+            f"What is the return type annotation of {function_member}?",
+            f"Can you tell me the return type annotation of {function_member}?",
+            f"I need to know the return type annotation of {function_member}.",
+            f"Do you know the return type annotation of {function_member}?",
+            f"Could you inform me about the return type annotation of {function_member}?",
+            f"I'm curious about the return type annotation of {function_member}.",
+        ]
+        function_return_type_answers = [
+            f"Return type annotation for {function_member} is '{returns_annotation}'.",
+            f"The return type annotation for {function_member} is '{returns_annotation}'.",
+            f"The return type for {function_member} is '{returns_annotation}'.",
+        ]
+
+        function_member_retrieval_chunks.append(function_return_type_context)
+        function_member_tuning_documents.extend(
+            allocate_tuning_triplets(
+                function_return_type_context,
+                function_return_type_questions,
+                function_return_type_answers,
+            )
+        )
 
     if not (returns_summary := member_type_details.function_returns.returns_summary):
-        function_return_summary_pairs = [
-            (
-                f"What does {function_member} return?",
-                f"Docstring of {function_member} does not describe its return.",
-            ),
-            (
-                f"Can you tell me what {function_member} returns?",
-                f"Docstring of {function_member} doesn't provide information about its return.",
-            ),
-            (
-                f"Do you know the return of {function_member}?",
-                f"Unfortunately, docstring of {function_member} doesn't specify what it returns.",
-            ),
-            (
-                f"I'm curious about what {function_member} returns. Can you help?",
-                f"I'm sorry, but the docstring of {function_member} doesn't clarify its return.",
-            ),
-            (
-                f"What's the return of {function_member}?",
-                f"The return of {function_member} is not described in its docstring.",
-            ),
-            (
-                f"Could you inform me about the return of {function_member}?",
-                f"Regrettably, the docstring of {function_member} doesn't detail its return.",
-            ),
-        ]
-        function_member_retrieval_chunks.append(f"{function_member} does not document its return.")
-        function_member_tuning_pairs.extend(allocate_tuning_pairs(function_return_summary_pairs))
-    else:
-        function_return_summary_pairs = [
-            (
-                f"What does {function_member} return?",
-                f"Based on {function_member} docstring, the return contains: '{returns_summary}'.",
-            ),
-            (
-                f"Can you tell me what {function_member} returns?",
-                f"Sure, as per docstring of {function_member}, it returns: '{returns_summary}'.",
-            ),
-            (
-                f"I'm curious about what {function_member} returns. Can you help?",
-                f"Absolutely! The docstring of {function_member} indicates that it returns:"
-                f" '{returns_summary}'.",
-            ),
-            (
-                f"Do you know what {function_member} returns?",
-                f"Yes, the docstring of {function_member} states that it returns:"
-                f" '{returns_summary}'.",
-            ),
-            (
-                f"I'd like to know what {function_member} returns.",
-                f"Of course, the docstring of {function_member} reveals that its return contains:"
-                f" '{returns_summary}'.",
-            ),
-            (
-                f"Could you inform me about the return of {function_member}?",
-                f"Certainly, the docstring of {function_member} specifies that it returns:"
-                f" '{returns_summary}'.",
-            ),
-        ]
-        function_member_retrieval_chunks.append(
+        function_return_summary_context = f"{function_member} does not document its return."
+        function_return_summary_questions = [
+            f"What does {function_member} return?",
+            f"Can you tell me what {function_member} returns?",
+            f"Do you know the return of {function_member}?",
+            f"I'm curious about what {function_member} returns. Can you help?",
+            f"What's the return of {function_member}?",
+            f"Could you inform me about the return of {function_member}?",
+        ]
+        function_return_summary_answers = [
+            f"Docstring of {function_member} does not describe its return.",
+            f"Docstring of {function_member} doesn't provide information about its return.",
+            f"Docstring of {function_member} doesn't specify what it returns.",
+            f"The docstring of {function_member} doesn't clarify its return.",
+            f"The return of {function_member} is not described in its docstring.",
+            f"The docstring of {function_member} doesn't detail its return.",
+        ]
+
+        function_member_retrieval_chunks.append(function_return_summary_context)
+        function_member_tuning_documents.extend(
+            allocate_tuning_triplets(
+                function_return_summary_context,
+                function_return_summary_questions,
+                function_return_summary_answers,
+            )
+        )
+    else:
+        function_return_summary_context = (
             f"Based on docstring, return of {function_member} is as follows: '{returns_summary}'."
         )
-        function_member_tuning_pairs.extend(allocate_tuning_pairs(function_return_summary_pairs))
+        function_return_summary_questions = [
+            f"What does {function_member} return?",
+            f"Can you tell me what {function_member} returns?",
+            f"I'm curious about what {function_member} returns. Can you help?",
+            f"Do you know what {function_member} returns?",
+            f"I'd like to know what {function_member} returns.",
+            f"Could you inform me about the return of {function_member}?",
+        ]
+        function_return_summary_answers = [
+            f"Based on {function_member} docstring, the return contains: '{returns_summary}'.",
+            f"As per docstring of {function_member}, it returns: '{returns_summary}'.",
+            f"The docstring of {function_member} indicates that it returns: '{returns_summary}'.",
+            f"The docstring of {function_member} states that it returns: '{returns_summary}'.",
+            f"The docstring of {function_member} reveals that its return contains:"
+            f" '{returns_summary}'.",
+            f"The docstring of {function_member} specifies that it returns: '{returns_summary}'.",
+        ]
+
+        function_member_retrieval_chunks.append(function_return_summary_context)
+        function_member_tuning_documents.extend(
+            allocate_tuning_triplets(
+                function_return_summary_context,
+                function_return_summary_questions,
+                function_return_summary_answers,
+            )
+        )
 
     if not (function_summary := member_type_details.function_summary):
-        function_summary_pairs = [
-            (
-                f"Summarise role of {function_member} in short.",
-                f"{function_member} docstring lacks a summary of its objective.",
-            ),
-            (
-                f"Can you briefly explain the role of {function_member}?",
-                f"The docstring of {function_member} doesn't provide its purpose.",
-            ),
-            (
-                f"What is the purpose of {function_member} as per its docstring?",
-                f"The docstring of {function_member} doesn't clearly state its purpose.",
-            ),
-            (
-                f"Could you provide a summary of objective of {function_member}?",
-                f"The objective of {function_member} is not summarised in its docstring.",
-            ),
-            (
-                f"What does {function_member} do according to its docstring?",
-                f"According to its docstring, role of {function_member} is not summarised.",
-            ),
-        ]
-        function_member_retrieval_chunks.append(f"Documentation for {function_member} is missing.")
-        function_member_tuning_pairs.extend(allocate_tuning_pairs(function_summary_pairs))
-    else:
-        function_summary_pairs = [
-            (
-                f"Summarise role of {function_member} in short.",
-                f"Based on docstring, objective of {function_member} is to: '{function_summary}'.",
-            ),
-            (
-                f"Can you briefly explain the role of {function_member}?",
-                f"Sure, according to the docstring, the purpose of {function_member} is:"
-                f" '{function_summary}'.",
-            ),
-            (
-                f"What does {function_member} do, in a nutshell?",
-                f"In a nutshell, {function_member} is designed to: '{function_summary}'.",
-            ),
-            (
-                f"Could you provide a short summary of role of {function_member}?",
-                f"Certainly, from docstring, {function_member} aims to: '{function_summary}'.",
-            ),
-            (
-                f"I need a brief explanation of what {function_member} does.",
-                f"Of course, {function_member} is intended to: '{function_summary}'.",
-            ),
-            (
-                f"In brief, what is the role of {function_member}?",
-                f"Briefly, the role of {function_member} is to: '{function_summary}',"
-                " according to the docstring.",
-            ),
-        ]
-        function_member_retrieval_chunks.append(
+        function_summary_context = f"Documentation for {function_member} is missing."
+        function_summary_questions = [
+            f"Summarise role of {function_member} in short.",
+            f"Can you briefly explain the role of {function_member}?",
+            f"What is the purpose of {function_member} as per its docstring?",
+            f"Could you provide a summary of objective of {function_member}?",
+            f"What does {function_member} do according to its docstring?",
+        ]
+        function_summary_answers = [
+            f"{function_member} docstring lacks a summary of its objective.",
+            f"The docstring of {function_member} doesn't provide its purpose.",
+            f"The docstring of {function_member} doesn't clearly state its purpose.",
+            f"The objective of {function_member} is not summarised in its docstring.",
+            f"According to its docstring, role of {function_member} is not summarised.",
+        ]
+
+        function_member_retrieval_chunks.append(function_summary_context)
+        function_member_tuning_documents.extend(
+            allocate_tuning_triplets(
+                function_summary_context, function_summary_questions, function_summary_answers
+            )
+        )
+    else:
+        function_summary_context = (
             f"{function_member} documents itself as follows: '{function_summary}'."
         )
-        function_member_tuning_pairs.extend(allocate_tuning_pairs(function_summary_pairs))
+        function_summary_questions = [
+            f"Summarise role of {function_member} in short.",
+            f"Can you briefly explain the role of {function_member}?",
+            f"What does {function_member} do, in a nutshell?",
+            f"Could you provide a short summary of role of {function_member}?",
+            f"I need a brief explanation of what {function_member} does.",
+            f"In brief, what is the role of {function_member}?",
+        ]
+        function_summary_answers = [
+            f"Based on docstring, objective of {function_member} is to: '{function_summary}'.",
+            f"According to the docstring, the purpose of {function_member} is:"
+            f" '{function_summary}'.",
+            f"In a nutshell, {function_member} is designed to: '{function_summary}'.",
+            f"From docstring, {function_member} aims to: '{function_summary}'.",
+            f"{function_member} is intended to: '{function_summary}'.",
+            f"The role of {function_member} is to: '{function_summary}',"
+            " according to the docstring.",
+        ]
+
+        function_member_retrieval_chunks.append(function_summary_context)
+        function_member_tuning_documents.extend(
+            allocate_tuning_triplets(
+                function_summary_context, function_summary_questions, function_summary_answers
+            )
+        )
 
     if not (function_raises := member_type_details.function_raises):
-        function_raise_types_pairs = [
-            (
-                f"Does {function_member} raise any specific exception?",
-                f"Docstring of {function_member} does not mention any specific exceptions.",
-            ),
-            (
-                f"Are there any specific exceptions that {function_member} raises?",
-                f"No specific exceptions are mentioned in the docstring of {function_member}.",
-            ),
-            (
-                f"Can you tell me if {function_member} raises any specific exceptions?",
-                f"According to docstring, {function_member} does not raise exceptions.",
-            ),
-            (
-                f"I want to know if {function_member} raises any specific exceptions."
-                " Can you confirm?",
-                f"I can confirm that docstring of {function_member} does not mention exceptions.",
-            ),
-            (
-                f"Could {function_member} possibly raise any specific exceptions?",
-                f"The docstring of {function_member} does not indicate that"
-                " it raises any specific exceptions.",
-            ),
-            (
-                f"Is it possible for {function_member} to raise any specific exceptions?",
-                f"The docstring of {function_member} does not suggest that"
-                " it raises any specific exceptions.",
-            ),
-        ]
-        function_member_retrieval_chunks.append(
+        function_raise_types_context = (
             f"{function_member} does not document any specific exceptions in the docstring."
         )
-        function_member_tuning_pairs.extend(allocate_tuning_pairs(function_raise_types_pairs))
+        function_raise_types_questions = [
+            f"Does {function_member} raise any specific exception?",
+            f"Are there any specific exceptions that {function_member} raises?",
+            f"Can you tell me if {function_member} raises any specific exceptions?",
+            f"I want to know if {function_member} raises any specific exceptions."
+            " Can you confirm?",
+            f"Could {function_member} possibly raise any specific exceptions?",
+            f"Is it possible for {function_member} to raise any specific exceptions?",
+        ]
+        function_raise_types_answers = [
+            f"Docstring of {function_member} does not mention any specific exceptions.",
+            f"No specific exceptions are mentioned in the docstring of {function_member}.",
+            f"According to docstring, {function_member} does not raise exceptions.",
+            f"Docstring of {function_member} does not mention exceptions.",
+            f"The docstring of {function_member} does not indicate that"
+            " it raises any specific exceptions.",
+            f"The docstring of {function_member} does not suggest that"
+            " it raises any specific exceptions.",
+        ]
+
+        function_member_retrieval_chunks.append(function_raise_types_context)
+        function_member_tuning_documents.extend(
+            allocate_tuning_triplets(
+                function_raise_types_context,
+                function_raise_types_questions,
+                function_raise_types_answers,
+            )
+        )
     else:
         function_raise_types = enumerate_array_elements(
             function_raises, attribute="raises_details"
         )
-        function_raise_types_pairs = [
-            (
-                f"Does {function_member} raise any specific exception?",
-                f"Based on docstring of {function_member}, it can raise the following:"
-                f" {function_raise_types}.",
-            ),
-            (
-                f"Can you tell me if {function_member} raises any specific exceptions?",
-                f"Yes, according to docstring of {function_member}, it can raise these exceptions:"
-                f" {function_raise_types}.",
-            ),
-            (
-                f"What exceptions, if any, does {function_member} raise?",
-                f"{function_member} can raise these exceptions as per its docstring:"
-                f" {function_raise_types}.",
-            ),
-            (
-                f"I need to know if {function_member} throws any specific exceptions."
-                " Can you help?",
-                f"Sure, {function_member} can throw following exceptions according to docstring:"
-                f" {function_raise_types}.",
-            ),
-            (
-                f"Could you inform me about any specific exceptions that"
-                f" {function_member} might raise?",
-                f"Certainly, the docstring of {function_member} indicates that"
-                f" it can raise these exceptions: {function_raise_types}.",
-            ),
-            (
-                f"I'm curious about the exceptions that {function_member} might throw."
-                " Do you have any information?",
-                f"Yes, the docstring of {function_member} suggests that"
-                f" it can throw the following exceptions: {function_raise_types}.",
-            ),
-        ]
-        function_member_retrieval_chunks.append(
+
+        function_raise_types_context = (
             f"From docstring, {function_member} can raise the following: {function_raise_types}"
         )
-        function_member_tuning_pairs.extend(allocate_tuning_pairs(function_raise_types_pairs))
+        function_raise_types_questions = [
+            f"Does {function_member} raise any specific exception?",
+            f"Can you tell me if {function_member} raises any specific exceptions?",
+            f"What exceptions, if any, does {function_member} raise?",
+            f"I need to know if {function_member} throws any specific exceptions. Can you help?",
+            f"Could you inform me about any specific exceptions that"
+            f" {function_member} might raise?",
+            f"I'm curious about the exceptions that {function_member} might throw."
+            " Do you have any information?",
+        ]
+        function_raise_types_answers = [
+            f"Based on docstring of {function_member}, it can raise the following:"
+            f" {function_raise_types}.",
+            f"According to docstring of {function_member}, it can raise these exceptions:"
+            f" {function_raise_types}.",
+            f"{function_member} can raise these exceptions as per its docstring:"
+            f" {function_raise_types}.",
+            f"{function_member} can throw following exceptions according to docstring:"
+            f" {function_raise_types}.",
+            f"The docstring of {function_member} indicates that"
+            f" it can raise these exceptions: {function_raise_types}.",
+            f"The docstring of {function_member} suggests that"
+            f" it can throw the following exceptions: {function_raise_types}.",
+        ]
+
+        function_member_retrieval_chunks.append(function_raise_types_context)
+        function_member_tuning_documents.extend(
+            allocate_tuning_triplets(
+                function_raise_types_context,
+                function_raise_types_questions,
+                function_raise_types_answers,
+            )
+        )
 
     if not (function_warns := member_type_details.function_warns):
-        function_warn_types_pairs = [
-            (
-                f"Does {function_member} throw any specific warnings?",
-                f"Docstring of {function_member} lacks any mention of specific warnings.",
-            ),
-            (
-                f"Are there any specific warnings that {function_member} throws?",
-                f"There are no specific warnings mentioned in docstring of {function_member}.",
-            ),
-            (
-                f"Can you tell me if {function_member} throws any specific warnings?",
-                f"According to the docstring of {function_member},"
-                " it doesn't throw any specific warnings.",
-            ),
-            (
-                f"I want to know if {function_member} throws any specific warnings."
-                " Can you help?",
-                f"Sure, I checked the docstring of {function_member} and"
-                " found no mention of specific warnings.",
-            ),
-            (
-                f"Could you check if {function_member} throws any specific warnings?",
-                f"I've checked the docstring of {function_member} and"
-                " it doesn't mention any specific warnings.",
-            ),
-            (
-                f"Is it possible that {function_member} throws any specific warnings?",
-                f"Based on the docstring of {function_member},"
-                " it doesn't seem to throw any specific warnings.",
-            ),
-        ]
-        function_member_retrieval_chunks.append(
+        function_warn_types_context = (
             f"Mention of any warnings is missing in docstring of {function_member}."
         )
-        function_member_tuning_pairs.extend(allocate_tuning_pairs(function_warn_types_pairs))
+        function_warn_types_questions = [
+            f"Does {function_member} throw any specific warnings?",
+            f"Are there any specific warnings that {function_member} throws?",
+            f"Can you tell me if {function_member} throws any specific warnings?",
+            f"I want to know if {function_member} throws any specific warnings. Can you help?",
+            f"Could you check if {function_member} throws any specific warnings?",
+            f"Is it possible that {function_member} throws any specific warnings?",
+        ]
+        function_warn_types_answers = [
+            f"Docstring of {function_member} lacks any mention of specific warnings.",
+            f"There are no specific warnings mentioned in docstring of {function_member}.",
+            f"According to the docstring of {function_member},"
+            " it doesn't throw any specific warnings.",
+            f"No mention of specific warnings are found in the docstring of {function_member}.",
+            f"Based on the docstring of {function_member},"
+            " it doesn't seem to throw any specific warnings.",
+        ]
+
+        function_member_retrieval_chunks.append(function_warn_types_context)
+        function_member_tuning_documents.extend(
+            allocate_tuning_triplets(
+                function_warn_types_context,
+                function_warn_types_questions,
+                function_warn_types_answers,
+            )
+        )
     else:
         function_warn_types = enumerate_array_elements(function_warns, attribute="warns_details")
-        function_warn_types_pairs = [
-            (
-                f"Does {function_member} throw any specific warnings?",
-                f"Based on the docstring, {function_member} can throw the following warnings:"
-                f" {function_warn_types}.",
-            ),
-            (
-                f"Can you tell me if {function_member} throws any specific warnings?",
-                f"Yes, according to docstring, {function_member} may throw these warnings:"
-                f" {function_warn_types}.",
-            ),
-            (
-                f"I'm curious, does {function_member} generate any particular warnings?",
-                f"Indeed, docstring indicates that {function_member} can generate these warnings:"
-                f" {function_warn_types}.",
-            ),
-            (
-                f"What specific warnings, if any, does {function_member} throw?",
-                f"{function_member} throws the following warnings as per the docstring:"
-                f" {function_warn_types}.",
-            ),
-            (
-                f"Could {function_member} possibly throw any specific warnings?",
-                f"Yes, it could. Docstring of {function_member} mentions these specific warnings:"
-                f" {function_warn_types}.",
-            ),
-            (
-                f"Are there any specific warnings that {function_member} throws?",
-                f"Yes, there are. The docstring for {function_member} lists following warnings:"
-                f" {function_warn_types}.",
-            ),
-        ]
-        function_member_retrieval_chunks.append(
+
+        function_warn_types_context = (
             f"{function_member} documents the following warnings: {function_warn_types}"
         )
-        function_member_tuning_pairs.extend(allocate_tuning_pairs(function_warn_types_pairs))
+        function_warn_types_questions = [
+            f"Does {function_member} throw any specific warnings?",
+            f"Can you tell me if {function_member} throws any specific warnings?",
+            f"I'm curious, does {function_member} generate any particular warnings?",
+            f"What specific warnings, if any, does {function_member} throw?",
+            f"Could {function_member} possibly throw any specific warnings?",
+            f"Are there any specific warnings that {function_member} throws?",
+        ]
+        function_warn_types_answers = [
+            f"Based on the docstring, {function_member} can throw the following warnings:"
+            f" {function_warn_types}.",
+            f"According to docstring, {function_member} may throw these warnings:"
+            f" {function_warn_types}.",
+            f"Docstring indicates that {function_member} can generate these warnings:"
+            f" {function_warn_types}.",
+            f"{function_member} throws the following warnings as per the docstring:"
+            f" {function_warn_types}.",
+            f"Docstring of {function_member} mentions these specific warnings:"
+            f" {function_warn_types}.",
+            f"The docstring for {function_member} lists following warnings:"
+            f" {function_warn_types}.",
+        ]
+
+        function_member_retrieval_chunks.append(function_warn_types_context)
+        function_member_tuning_documents.extend(
+            allocate_tuning_triplets(
+                function_warn_types_context,
+                function_warn_types_questions,
+                function_warn_types_answers,
+            )
+        )
 
     if not (function_notes := member_type_details.function_notes):
-        function_notes_pairs = [
-            (
-                f"Is there any specific details for {function_member} to be aware of?",
-                f"Docstring of {function_member} lacks any notes on specific details.",
-            ),
-            (
-                f"Are there any particular details I should know about {function_member}?",
-                f"There are no specific details noted in the docstring of {function_member}.",
-            ),
-            (
-                f"What should I be aware of when using {function_member}?",
-                f"The docstring of {function_member} does not contain any details to be aware of.",
-            ),
-            (
-                f"Could you tell me if there are any specific details for {function_member}?",
-                f"No specific details are mentioned in the docstring of {function_member}.",
-            ),
-            (
-                f"I'm curious if there are any specific details about {function_member}?",
-                f"The docstring of {function_member} does not provide any specific details.",
-            ),
-            (
-                f"Do I need to be aware of any specific details for {function_member}?",
-                f"The docstring of {function_member} does not include any specific details.",
-            ),
-        ]
-        function_member_retrieval_chunks.append(
-            f"{function_member} has no specific notes in the docstring."
-        )
-        function_member_tuning_pairs.extend(allocate_tuning_pairs(function_notes_pairs))
-    else:
-        function_notes_pairs = [
-            (
-                f"Is there any specific details for {function_member} to be aware of?",
-                f"Docstring of {function_member} highlights the following: '{function_notes}'.",
-            ),
-            (
-                f"What should I know about {function_member}?",
-                "You should be aware that docstring includes the following details:"
-                f" '{function_notes}'.",
-            ),
-            (
-                f"Could you provide some details about {function_member}?",
-                f"Sure, the docstring of {function_member} provides the following information:"
-                f" '{function_notes}'.",
-            ),
-            (
-                f"What are the important details of {function_member}?",
-                f"The important details of {function_member} are highlighted in its docstring:"
-                f" '{function_notes}'.",
-            ),
-            (
-                f"Can you tell me more about {function_member}?",
-                f"Of course, the docstring of {function_member} contains the following details:"
-                f" '{function_notes}'.",
-            ),
-            (
-                f"I need information about {function_member}.",
-                f"The docstring of {function_member} contains the following information:"
-                f" '{function_notes}'.",
-            ),
-        ]
-        function_member_retrieval_chunks.append(
+        function_notes_context = f"{function_member} has no specific notes in the docstring."
+        function_notes_questions = [
+            f"Is there any specific details for {function_member} to be aware of?",
+            f"Are there any particular details I should know about {function_member}?",
+            f"What should I be aware of when using {function_member}?",
+            f"Could you tell me if there are any specific details for {function_member}?",
+            f"I'm curious if there are any specific details about {function_member}?",
+            f"Do I need to be aware of any specific details for {function_member}?",
+        ]
+        function_notes_answers = [
+            f"Docstring of {function_member} lacks any notes on specific details.",
+            f"There are no specific details noted in the docstring of {function_member}.",
+            f"The docstring of {function_member} does not contain any details to be aware of.",
+            f"No specific details are mentioned in the docstring of {function_member}.",
+            f"The docstring of {function_member} does not provide any specific details.",
+            f"The docstring of {function_member} does not include any specific details.",
+        ]
+
+        function_member_retrieval_chunks.append(function_notes_context)
+        function_member_tuning_documents.extend(
+            allocate_tuning_triplets(
+                function_notes_context, function_notes_questions, function_notes_answers
+            )
+        )
+    else:
+        function_notes_context = (
             f"Docstring for {function_member} has following notes: '{function_notes}'."
         )
-        function_member_tuning_pairs.extend(allocate_tuning_pairs(function_notes_pairs))
+        function_notes_questions = [
+            f"Is there any specific details for {function_member} to be aware of?",
+            f"What should I know about {function_member}?",
+            f"Could you provide some details about {function_member}?",
+            f"What are the important details of {function_member}?",
+            f"Can you tell me more about {function_member}?",
+            f"I need information about {function_member}.",
+        ]
+        function_notes_answers = [
+            f"Docstring of {function_member} highlights the following: '{function_notes}'.",
+            "Users should be aware that docstring includes the following details:"
+            f" '{function_notes}'.",
+            f"The docstring of {function_member} provides the following information:"
+            f" '{function_notes}'.",
+            f"The important details of {function_member} are highlighted in its docstring:"
+            f" '{function_notes}'.",
+            f"The docstring of {function_member} contains the following details:"
+            f" '{function_notes}'.",
+            f"The docstring of {function_member} contains the following information:"
+            f" '{function_notes}'.",
+        ]
+
+        function_member_retrieval_chunks.append(function_notes_context)
+        function_member_tuning_documents.extend(
+            allocate_tuning_triplets(
+                function_notes_context, function_notes_questions, function_notes_answers
+            )
+        )
 
     if not (function_references := member_type_details.function_references):
-        function_references_pairs = [
-            (
-                f"Is there any reference for {function_member}?",
-                f"Documentation for {function_member} contains no references.",
-            ),
-            (
-                f"Can I find any references in the documentation for {function_member}?",
-                f"No, the documentation for {function_member} does not contain any references.",
-            ),
-            (
-                f"Does the documentation for {function_member} include any references?",
-                f"No, there are no references in the documentation for {function_member}.",
-            ),
-            (
-                f"Are there references available in the {function_member} documentation?",
-                f"No, the {function_member} documentation does not include any references.",
-            ),
-            (
-                f"I'm looking for references in {function_member} documentation. Are there any?",
-                f"Unfortunately, the documentation for {function_member} contains no references.",
-            ),
-            (
-                f"Could you tell me if there are any references for {function_member}?",
-                f"I'm sorry, but documentation for {function_member} lacks any references.",
-            ),
-        ]
-        function_member_retrieval_chunks.append(
+        function_references_context = (
             f"{function_member} documents no references in its docstring."
         )
-        function_member_tuning_pairs.extend(allocate_tuning_pairs(function_references_pairs))
+        function_references_questions = [
+            f"Is there any reference for {function_member}?",
+            f"Can I find any references in the documentation for {function_member}?",
+            f"Does the documentation for {function_member} include any references?",
+            f"Are there references available in the {function_member} documentation?",
+            f"I'm looking for references in {function_member} documentation. Are there any?",
+            f"Could you tell me if there are any references for {function_member}?",
+        ]
+        function_references_answers = [
+            f"Documentation for {function_member} contains no references.",
+            f"The documentation for {function_member} does not contain any references.",
+            f"There are no references in the documentation for {function_member}.",
+            f"The {function_member} documentation does not include any references.",
+            f"The documentation for {function_member} contains no references.",
+            f"Documentation for {function_member} lacks any references.",
+        ]
+
+        function_member_retrieval_chunks.append(function_references_context)
+        function_member_tuning_documents.extend(
+            allocate_tuning_triplets(
+                function_references_context,
+                function_references_questions,
+                function_references_answers,
+            )
+        )
     else:
-        function_references_pairs = [
-            (
-                f"Is there any reference for {function_member}?",
-                f"The docstring links the following: '{function_references}'.",
-            ),
-            (
-                f"Can you provide a reference for {function_member}?",
-                f"Sure, the docstring provides the following reference: '{function_references}'.",
-            ),
-            (
-                f"Where can I find a reference for {function_member}?",
-                f"You can find it in the docstring, which links to: '{function_references}'.",
-            ),
-            (
-                f"Could you point me to the reference for {function_member}?",
-                f"Of course, the docstring points to these reference: '{function_references}'.",
-            ),
-            (
-                f"I'm looking for a reference for {function_member}. Can you help?",
-                f"Absolutely, the docstring links to this reference: '{function_references}'.",
-            ),
-            (
-                f"What's the reference for {function_member}?",
-                f"The reference for that is in the docstring: '{function_references}'.",
-            ),
-        ]
-        function_member_retrieval_chunks.append(
+        function_references_context = (
             f"{function_member} list the following references: {function_references}"
         )
-        function_member_tuning_pairs.extend(allocate_tuning_pairs(function_references_pairs))
+        function_references_questions = [
+            f"Is there any reference for {function_member}?",
+            f"Can you provide a reference for {function_member}?",
+            f"Where can I find a reference for {function_member}?",
+            f"Could you point me to the reference for {function_member}?",
+            f"I'm looking for a reference for {function_member}. Can you help?",
+            f"What's the reference for {function_member}?",
+        ]
+        function_references_answers = [
+            f"The docstring links the following: '{function_references}'.",
+            f"The docstring provides the following reference: '{function_references}'.",
+            f"The docstring links to: '{function_references}'.",
+            f"The docstring points to these reference: '{function_references}'.",
+            f"The docstring links to this reference: '{function_references}'.",
+            f"The reference for that is in the docstring: '{function_references}'.",
+        ]
+
+        function_member_retrieval_chunks.append(function_references_context)
+        function_member_tuning_documents.extend(
+            allocate_tuning_triplets(
+                function_references_context,
+                function_references_questions,
+                function_references_answers,
+            )
+        )
 
     if not (function_examples := member_type_details.function_examples):
-        function_examples_pairs = [
-            (
-                f"Is there any example for {function_member}?",
-                f"Docstring for {function_member} lacks any examples.",
-            ),
-            (
-                f"Can I find an example for {function_member} in the docstring?",
-                f"Unfortunately, docstring for {function_member} does not contain any examples.",
-            ),
-            (
-                f"Does the docstring for {function_member} include any examples?",
-                f"No, the docstring for {function_member} does not include any examples.",
-            ),
-            (
-                f"I'm looking for an example of {function_member} in docstring, is there one?",
-                f"I'm sorry, but docstring for {function_member} does not provide any examples.",
-            ),
-            (
-                f"Are there any examples provided in the docstring for {function_member}?",
-                f"No examples are provided in the docstring for {function_member}.",
-            ),
-            (
-                f"Could you tell me if there's an example for {function_member} in docstring?",
-                f"I regret to inform you that {function_member} documents no examples.",
-            ),
-        ]
-        function_member_retrieval_chunks.append(
-            f"Documentation of {function_member} lacks any examples."
-        )
-        function_member_tuning_pairs.extend(allocate_tuning_pairs(function_examples_pairs))
-    else:
-        function_examples_pairs = [
-            (
-                f"Is there any example for {function_member}?",
-                f"Documentation of {function_member} contains these examples:"
-                f" '{function_examples}'.",
-            ),
-            (
-                f"Can you provide an example of {function_member}?",
-                f"Sure, you can find examples of {function_member} in its documentation:"
-                f" '{function_examples}'.",
-            ),
-            (
-                f"I'm looking for examples of {function_member}, can you help?",
-                f"Absolutely, examples for {function_member} are available in its documentation:"
-                f" '{function_examples}'.",
-            ),
-            (
-                f"Where can I find examples for {function_member}?",
-                f"You can find examples for {function_member} in its documentation:"
-                f" '{function_examples}'.",
-            ),
-            (
-                f"Could you show me some examples of {function_member}?",
-                f"Of course, the documentation of {function_member} includes these examples:"
-                f" '{function_examples}'.",
-            ),
-            (
-                f"I need examples for {function_member}, where can I find them?",
-                f"You can find examples for {function_member} in its documentation:"
-                f" '{function_examples}'.",
-            ),
-        ]
-        function_member_retrieval_chunks.append(
+        function_examples_context = f"Documentation of {function_member} lacks any examples."
+        function_examples_questions = [
+            f"Is there any example for {function_member}?",
+            f"Can I find an example for {function_member} in the docstring?",
+            f"Does the docstring for {function_member} include any examples?",
+            f"I'm looking for an example of {function_member} in docstring, is there one?",
+            f"Are there any examples provided in the docstring for {function_member}?",
+            f"Could you tell me if there's an example for {function_member} in docstring?",
+        ]
+        function_examples_answers = [
+            f"Docstring for {function_member} lacks any examples.",
+            f"Docstring for {function_member} does not contain any examples.",
+            f"The docstring for {function_member} does not include any examples.",
+            f"Docstring for {function_member} does not provide any examples.",
+            f"No examples are provided in the docstring for {function_member}.",
+            f"{function_member} documents no examples.",
+        ]
+
+        function_member_retrieval_chunks.append(function_examples_context)
+        function_member_tuning_documents.extend(
+            allocate_tuning_triplets(
+                function_examples_context, function_examples_questions, function_examples_answers
+            )
+        )
+    else:
+        function_examples_context = (
             f"Docstring of {function_member} contains following examples: '{function_examples}'."
         )
-        function_member_tuning_pairs.extend(allocate_tuning_pairs(function_examples_pairs))
+        function_examples_questions = [
+            f"Is there any example for {function_member}?",
+            f"Can you provide an example of {function_member}?",
+            f"I'm looking for examples of {function_member}, can you help?",
+            f"Where can I find examples for {function_member}?",
+            f"Could you show me some examples of {function_member}?",
+            f"I need examples for {function_member}, where can I find them?",
+        ]
+        function_examples_answers = [
+            f"Documentation of {function_member} contains these examples: '{function_examples}'.",
+            f"In documentation of {function_member}, these examples can be found:"
+            f" '{function_examples}'.",
+            f"Examples for {function_member} are available in its documentation:"
+            f" '{function_examples}'.",
+            f"In documentation for {function_member}, these examples can be found:"
+            f" '{function_examples}'.",
+            f"The documentation of {function_member} includes these examples:"
+            f" '{function_examples}'.",
+        ]
+
+        function_member_retrieval_chunks.append(function_examples_context)
+        function_member_tuning_documents.extend(
+            allocate_tuning_triplets(
+                function_examples_context, function_examples_questions, function_examples_answers
+            )
+        )
 
     function_member_dataset = Dataset(
         retrieval_chunks=function_member_retrieval_chunks[:2],
-        tuning_pairs=function_member_tuning_pairs,
+        tuning_documents=function_member_tuning_documents,
     )
 
     return function_member_dataset, function_member_retrieval_chunks
 
 
 @pydantic.validate_call(validate_return=True)
-def generate_member_dataset(member_details: MemberDetails) -> tuple[Dataset, ...]:
+def generate_member_dataset(member_details: MemberDetails) -> tuple[Dataset, ...]:  # noqa: PLR0915
     """Create a dataset for a member.
 
     Parameters
     ----------
     member_details : MemberDetails
         all details of the member
 
     Returns
     -------
     tuple[Dataset, ...]
-        all documents for retrieval and tuning pairs for querying member documentation
+        all documents for retrieval and tuning for querying member documentation
 
     Raises
     ------
     ValueError
         if the member type is not supported
 
     Notes
@@ -2734,196 +2488,171 @@
     * Otherwise, there will be two returns, one for the member and one for the member type.
     """
     member_name = member_details.member_name
     member_full_name = member_details.member_qualified_name
     member = f"'{member_name}' object"
 
     member_retrieval_chunks: list[str] = []
-    member_tuning_pairs: list[tuple[str, str, SplitName]] = []
+    member_tuning_documents: list[Document] = []
+
+    module_parent_context = f"{member} is part of parent module {member_details.member_module}."
+    module_parent_questions = [
+        f"What is the parent module of {member}?",
+        f"Can you tell me the parent module of {member}?",
+        f"I'm trying to find the parent module of {member}, can you help?",
+        f"Do you know the parent module of {member}?",
+        f"I need to know the parent module of {member}, can you provide that?",
+        f"Could you inform me about the parent module of {member}?",
+    ]
+    module_parent_answers = [
+        f"'{member_details.member_module}' is the name of its parent module.",
+        f"The parent module of {member} is '{member_details.member_module}'.",
+        f"Parent module of {member} is '{member_details.member_module}'.",
+        f"'{member_details.member_module}' is parent module of {member}.",
+    ]
+
+    member_retrieval_chunks.append(module_parent_context)
+    member_tuning_documents.extend(
+        allocate_tuning_triplets(
+            module_parent_context, module_parent_questions, module_parent_answers
+        )
+    )
 
-    module_parent_pairs = [
-        (
-            f"What is the parent module of {member}?",
-            f"'{member_details.member_module}' is the name of its parent module.",
-        ),
-        (
-            f"Can you tell me the parent module of {member}?",
-            f"Sure, the parent module of {member} is '{member_details.member_module}'.",
-        ),
-        (
-            f"I'm trying to find the parent module of {member}, can you help?",
-            f"Of course, parent module of {member} is '{member_details.member_module}'.",
-        ),
-        (
-            f"Do you know the parent module of {member}?",
-            f"Yes, the parent module of {member} is '{member_details.member_module}'.",
-        ),
-        (
-            f"I need to know the parent module of {member}, can you provide that?",
-            f"Absolutely, parent module of {member} is '{member_details.member_module}'.",
-        ),
-        (
-            f"Could you inform me about the parent module of {member}?",
-            f"Certainly, '{member_details.member_module}' is parent module of {member}.",
-        ),
-    ]
-    member_retrieval_chunks.append(
-        f"{member} is part of parent module {member_details.member_module}."
-    )
-    member_tuning_pairs.extend(allocate_tuning_pairs(module_parent_pairs))
-
-    member_full_name_pairs = [
-        (
-            f"What is the full name of {member}?",
-            f"'{member_full_name}' is its fully qualified name.",
-        ),
-        (
-            f"Can you tell me the full name of the {member}?",
-            f"Sure, the fully qualified name of {member} is '{member_full_name}'.",
-        ),
-        (
-            f"I need to know the full name of {member}. Can you help?",
-            f"Of course, the full name of {member} is '{member_full_name}'.",
-        ),
-        (
-            f"What's the fully qualified name for the {member}?",
-            f"The fully qualified name for {member} is '{member_full_name}'.",
-        ),
-        (
-            f"Could you provide the full name of the {member}?",
-            f"Certainly, the full name of the {member} is '{member_full_name}'.",
-        ),
-        (
-            f"I'm looking for the full name of {member}. What is it?",
-            f"The full name of {member} is '{member_full_name}'.",
-        ),
+    member_full_name_context = f"Full name of {member} is '{member_full_name}'."
+    member_full_name_questions = [
+        f"What is the full name of {member}?",
+        f"Can you tell me the full name of the {member}?",
+        f"I need to know the full name of {member}. Can you help?",
+        f"What's the fully qualified name for the {member}?",
+        f"Could you provide the full name of the {member}?",
+        f"I'm looking for the full name of {member}. What is it?",
+    ]
+    member_full_name_answers = [
+        f"'{member_full_name}' is its fully qualified name.",
+        f"The fully qualified name of {member} is '{member_full_name}'.",
+        f"The full name of {member} is '{member_full_name}'.",
+        f"The fully qualified name for {member} is '{member_full_name}'.",
+        f"The full name of the {member} is '{member_full_name}'.",
     ]
-    member_retrieval_chunks.append(f"Full name of {member} is '{member_full_name}'.")
-    member_tuning_pairs.extend(allocate_tuning_pairs(member_full_name_pairs))
+
+    member_retrieval_chunks.append(member_full_name_context)
+    member_tuning_documents.extend(
+        allocate_tuning_triplets(
+            member_full_name_context, member_full_name_questions, member_full_name_answers
+        )
+    )
 
     member_hierarchy = enumerate_array_elements(member_details.member_hierarchy)
-    member_hierarchy_pairs = [
-        (
-            f"What is the hierarchy of {member}?",
-            f"The hierarchy of {member} is as follows: {member_hierarchy}.",
-        ),
-        (
-            f"Can you explain the hierarchy of the {member}?",
-            f"Sure, the hierarchy of the {member} is: {member_hierarchy}.",
-        ),
-        (
-            f"Could you tell me the hierarchy of {member}?",
-            f"Of course, the hierarchy of {member} is: {member_hierarchy}.",
-        ),
-        (
-            f"I would like to know the hierarchy of {member}. Can you provide that?",
-            f"Absolutely, the hierarchy of {member} is: {member_hierarchy}.",
-        ),
-        (
-            f"Please provide the hierarchy of {member}.",
-            f"The hierarchy of {member} is: {member_hierarchy}.",
-        ),
-        (
-            f"I'm interested in the hierarchy of {member}. Could you share it?",
-            f"Sure, the hierarchy of {member} is: {member_hierarchy}.",
-        ),
+
+    member_hierarchy_context = f"Hierarchy of {member} is as follows: {member_hierarchy}."
+    member_hierarchy_questions = [
+        f"What is the hierarchy of {member}?",
+        f"Can you explain the hierarchy of the {member}?",
+        f"Could you tell me the hierarchy of {member}?",
+        f"I would like to know the hierarchy of {member}. Can you provide that?",
+        f"Please provide the hierarchy of {member}.",
+        f"I'm interested in the hierarchy of {member}. Could you share it?",
+    ]
+    member_hierarchy_answers = [
+        f"The hierarchy of {member} is as follows: {member_hierarchy}.",
+        f"The hierarchy of the {member} is: {member_hierarchy}.",
+        f"The hierarchy of {member} is: {member_hierarchy}.",
     ]
-    member_retrieval_chunks.append(f"Hierarchy of {member} is as follows: {member_hierarchy}.")
-    member_tuning_pairs.extend(allocate_tuning_pairs(member_hierarchy_pairs))
+
+    member_retrieval_chunks.append(member_hierarchy_context)
+    member_tuning_documents.extend(
+        allocate_tuning_triplets(
+            member_hierarchy_context, member_hierarchy_questions, member_hierarchy_answers
+        )
+    )
 
     if not (member_docstring := member_details.member_docstring):
-        member_documentation_pairs = [
-            (
-                f"What is the documentation of {member}?",
-                f"{member} does not have any documentation.",
-            ),
-            (
-                f"Can you provide the documentation for the {member}?",
-                f"Sorry, the {member} does not have any documentation.",
-            ),
-            (
-                f"Is there any documentation available for the {member}?",
-                f"No, there is no documentation available for the {member}.",
-            ),
-            (
-                f"Could you show me the documentation of the {member}?",
-                f"Unfortunately, the {member} does not have any documentation.",
-            ),
-            (
-                f"I'm looking for the documentation of {member}. Can you help?",
-                f"I'm sorry, but the {member} does not have any documentation.",
-            ),
-        ]
-        member_retrieval_chunks.append(
+        member_documentation_context = (
             f"Unfortunately, {member} currently does not have any documentation."
         )
-        member_tuning_pairs.extend(allocate_tuning_pairs(member_documentation_pairs))
+        member_documentation_questions = [
+            f"What is the documentation of {member}?",
+            f"Can you provide the documentation for the {member}?",
+            f"Is there any documentation available for the {member}?",
+            f"Could you show me the documentation of the {member}?",
+            f"I'm looking for the documentation of {member}. Can you help?",
+        ]
+        member_documentation_answers = [
+            f"{member} does not have any documentation.",
+            f"The {member} does not have any documentation.",
+            f"There is no documentation available for the {member}.",
+        ]
+
+        member_retrieval_chunks.append(member_documentation_context)
+        member_tuning_documents.extend(
+            allocate_tuning_triplets(
+                member_documentation_context,
+                member_documentation_questions,
+                member_documentation_answers,
+            )
+        )
     else:
-        member_documentation_pairs = [
-            (f"What does {member} do?", f"Its documentation is as follows: '{member_docstring}'."),
-            (
-                f"Can you explain the function of the {member}?",
-                f"Sure, here is its documentation: '{member_docstring}'.",
-            ),
-            (
-                f"I'm not sure what {member} does. Can you clarify?",
-                f"Of course, here's its documentation for clarification: '{member_docstring}'.",
-            ),
-            (
-                f"Could you tell me about the {member}?",
-                f"Certainly, its documentation is: '{member_docstring}'.",
-            ),
-            (
-                f"I need information on the {member}.",
-                f"Here's the documentation you need: '{member_docstring}'.",
-            ),
-            (
-                f"What's the purpose of the {member}?",
-                f"The purpose is described in its documentation: '{member_docstring}'.",
-            ),
-        ]
-        member_retrieval_chunks.append(
+        member_documentation_context = (
             f"The following is the documentation of {member}: '{member_docstring}'."
         )
-        member_tuning_pairs.extend(allocate_tuning_pairs(member_documentation_pairs))
+        member_documentation_questions = [
+            f"What does {member} do?",
+            f"Can you explain the function of the {member}?",
+            f"I'm not sure what {member} does. Can you clarify?",
+            f"Could you tell me about the {member}?",
+            f"I need information on the {member}.",
+            f"What's the purpose of the {member}?",
+        ]
+        member_documentation_answers = [
+            f"Its documentation is as follows: '{member_docstring}'.",
+            f"Here is its documentation: '{member_docstring}'.",
+            f"Here's its documentation for clarification: '{member_docstring}'.",
+            f"Its documentation is: '{member_docstring}'.",
+            f"Here's the documentation you need: '{member_docstring}'.",
+            f"The purpose is described in its documentation: '{member_docstring}'.",
+        ]
+
+        member_retrieval_chunks.append(member_documentation_context)
+        member_tuning_documents.extend(
+            allocate_tuning_triplets(
+                member_documentation_context,
+                member_documentation_questions,
+                member_documentation_answers,
+            )
+        )
 
     if (member_type_details := member_details.member_type_details) is not None:
         member_type = member_type_details.member_type
 
-        member_type_pairs = [
-            (f"What is the type of {member}?", f"{member} is of '{member_type.value}' type."),
-            (
-                f"Can you tell me the type of the {member}?",
-                f"Sure, the {member} is of '{member_type.value}' type.",
-            ),
-            (
-                f"I would like to know the type of {member}. Can you help?",
-                f"Absolutely, the {member} is of '{member_type.value}' type.",
-            ),
-            (
-                f"Do you know the type of {member}?",
-                f"Yes, the {member} is of '{member_type.value}' type.",
-            ),
-            (
-                f"Could you inform me about the type of {member}?",
-                f"Of course, the {member} is of '{member_type.value}' type.",
-            ),
-            (
-                f"I'm curious about type of {member}. Can you provide some information?",
-                f"Certainly, the {member} is of '{member_type.value}' type.",
-            ),
-        ]
-        member_retrieval_chunks.insert(-1, f"'{member_name}' is a Python {member_type.value}.")
-        member_tuning_pairs.extend(allocate_tuning_pairs(member_type_pairs))
+        member_type_context = f"'{member_name}' is a Python {member_type.value}."
+        member_type_questions = [
+            f"What is the type of {member}?",
+            f"Can you tell me the type of the {member}?",
+            f"I would like to know the type of {member}. Can you help?",
+            f"Do you know the type of {member}?",
+            f"Could you inform me about the type of {member}?",
+            f"I'm curious about type of {member}. Can you provide some information?",
+        ]
+        member_type_answers = [
+            f"{member} is of '{member_type.value}' type.",
+            f"The {member} is of '{member_type.value}' type.",
+        ]
+
+        member_retrieval_chunks.append(member_type_context)
+        member_tuning_documents.extend(
+            allocate_tuning_triplets(
+                member_type_context, member_type_questions, member_type_answers
+            )
+        )
 
     if member_type_details is None:
         member_retrieval_chunks.insert(0, f"'{member_name}' is a Python object.")
 
         member_dataset = Dataset(
-            retrieval_chunks=member_retrieval_chunks, tuning_pairs=member_tuning_pairs
+            retrieval_chunks=member_retrieval_chunks, tuning_documents=member_tuning_documents
         )
 
         return (member_dataset,)
 
     match member_type:
         case MemberType.ENUM:
             member_type_dataset, member_type_retrieval_chunks = generate_enum_member_dataset(
@@ -2940,15 +2669,15 @@
         case _:
             LOGGER.critical(f"Received unsupported {member_type=}")
 
             raise ValueError("Unexpected member type: supports 'enum', 'class', 'function'")
 
     member_dataset = Dataset(
         retrieval_chunks=member_retrieval_chunks + member_type_retrieval_chunks,
-        tuning_pairs=member_tuning_pairs,
+        tuning_documents=member_tuning_documents,
     )
 
     return (member_dataset, member_type_dataset)
 
 
 __all__ = [
     "enumerate_array_elements",
```

### Comparing `query-package-documentation-0.0.2/src/generative_ai/dataset_generation/utils_generation.py` & `query-package-documentation-0.0.3/src/generative_ai/dataset_generation/utils_generation.py`

 * *Files 17% similar despite different names*

```diff
@@ -435,86 +435,28 @@
     """
 
     context: str
     question: str
     answer: str
     split: SplitName
 
-    @pydantic.computed_field
-    @functools.cached_property
-    def instruction_with_context(self: "Document") -> str:
-        """Store tuning prompt for the document using context, question and answer.
-
-        Returns
-        -------
-        str
-            tuning prompt for the document using context, question and answer
-        """
-        system_instruction = (
-            "Below is a question that can be answered using the following context. "
-            "Write an answer for the question appropriately without using any additional data."
-        )
-
-        return " ".join(
-            [
-                "<s>",
-                f"[INST] {system_instruction} [/INST]",
-                f"[INST] Context: {self.context} [/INST]",
-                f"[INST] Question: {self.question} [/INST]",
-                f"[INST] Answer: {self.answer} [/INST]",
-                "</s>",
-            ]
-        )
-
-    @pydantic.computed_field
-    @functools.cached_property
-    def instruction_without_context(self: "Document") -> str:
-        """Store tuning prompt for the document using question and answer.
-
-        Returns
-        -------
-        str
-            tuning prompt for the document using question and answer
-        """
-        return f"<s>[INST] {self.question} [/INST] {self.answer} </s>"
-
 
 class Dataset(pydantic.BaseModel):
     """Store details of a dataset.
 
     Attributes
     ----------
     retrieval_chunks : list[str]
         chunks of text to be used for retrieval
-    tuning_pairs : list[tuple[str, str, SplitName]]
+    tuning_triplets : list[tuple[str, str, SplitName]]
         pairs of question and answer to be used for tuning and their split allocation
     """
 
     retrieval_chunks: list[str]
-    tuning_pairs: list[tuple[str, str, SplitName]]
-
-    @pydantic.computed_field
-    @functools.cached_property
-    def tuning_documents(self: "Dataset") -> list[Document]:
-        """Store tuning documents using concatenated retrieval sources, questions and answers.
-
-        Returns
-        -------
-        list[Document]
-            tuning documents using concatenated retrieval sources, questions and answers
-        """
-        return [
-            Document(
-                context=" ".join(self.retrieval_chunks),
-                question=question,
-                answer=answer,
-                split=split,
-            )
-            for question, answer, split in self.tuning_pairs
-        ]
+    tuning_documents: list[Document]
 
 
 class JSONDocument(pydantic.BaseModel):
     """Store details of a document in JSON format.
 
     Attributes
     ----------
@@ -522,26 +464,20 @@
         details containing the description
     question : str
         question to be answered or instructions to follow using the ``context``
     answer : str
         answer to the question or instruction based on the ``context``
     split : SplitName
         split allocation of the document
-    instruction_with_context : str
-        tuning prompt for the document using context, question and answer
-    instruction_without_context : str
-        tuning prompt for the document using question and answer
     """
 
     context: str
     question: str
     answer: str
     split: SplitName
-    instruction_with_context: str
-    instruction_without_context: str
 
 
 class JSONDataset(pydantic.BaseModel):
     """Store all details for querying a package documentation in JSON format.
 
     Attributes
     ----------
```

### Comparing `query-package-documentation-0.0.2/src/generative_ai/information_retrieval/__init__.py` & `query-package-documentation-0.0.3/src/generative_ai/information_retrieval/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,27 +21,25 @@
     LanguageModel,
     LanguageModelAdapter,
     PipelineType,
     QuantisedModel,
     RetrievalType,
     StandardModel,
     TransformerType,
-    ValidatedChroma,
 )
 
 __all__ = [
     "CaptureDetailsCallback",
     "LanguageModel",
     "LanguageModelAdapter",
     "PipelineType",
     "QuantisedModel",
     "RetrievalType",
     "StandardModel",
     "TransformerType",
-    "ValidatedChroma",
     "configure_language_model",
     "create_database_retriever",
     "create_document_embedder",
     "create_embedding_database",
     "create_llm",
     "create_vector_store",
     "generate_retrieval_chain",
```

### Comparing `query-package-documentation-0.0.2/src/generative_ai/information_retrieval/orchestrate_retrieval.py` & `query-package-documentation-0.0.3/src/generative_ai/information_retrieval/orchestrate_retrieval.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 """Define functionalities to orchestrate information retrieval."""
 
-import pathlib
+import typing
 
 import pydantic
-from langchain.docstore.document import Document
-from langchain.schema.runnable import RunnableSerializable
 
 from .step_1_retrieval import (
     create_document_embedder,
     create_vector_store,
     load_json_documents,
     partition_documents,
 )
@@ -16,19 +14,25 @@
 from .step_3_retrieval import CaptureDetailsCallback
 from .utils_retrieval import (
     LanguageModel,
     LanguageModelAdapter,
     PipelineType,
     RetrievalType,
     TransformerType,
-    ValidatedChroma,
 )
 
+if typing.TYPE_CHECKING:
+    import pathlib
 
-def load_source_documents(file_path: pathlib.Path) -> list[Document]:
+    from langchain.docstore.document import Document
+    from langchain.schema.runnable import RunnableSerializable
+    from langchain.vectorstores.chroma import Chroma
+
+
+def load_source_documents(file_path: "pathlib.Path") -> list["Document"]:
     """Load and partition source documents.
 
     Parameters
     ----------
     file_path : pathlib.Path
         path storing JSON dataset
 
@@ -40,16 +44,16 @@
     raw_documents = load_json_documents(file_path)
     partitioned_documents = partition_documents(raw_documents)
 
     return partitioned_documents
 
 
 def create_embedding_database(
-    embedding_model: str, directory_path: pathlib.Path, source_documents: list[Document]
-) -> ValidatedChroma:
+    embedding_model: str, directory_path: "pathlib.Path", source_documents: list["Document"]
+) -> "Chroma":
     """Prepare an embedding database.
 
     Parameters
     ----------
     embedding_model : str
         name of Sentence Transformers model from Hugging Face
     directory_path : pathlib.Path
@@ -66,26 +70,26 @@
 
     vector_store = create_vector_store(document_embedder, directory_path)
     vector_store.add_documents(source_documents)
 
     return vector_store
 
 
-def store_embedding_database(vector_store: ValidatedChroma) -> None:
+def store_embedding_database(vector_store: "Chroma") -> None:
     """Dump vector store to disk into configured directory.
 
     Parameters
     ----------
     vector_store : Chroma
         vector store
     """
     vector_store.persist()
 
 
-def load_embedding_database(embedding_model: str, directory_path: pathlib.Path) -> ValidatedChroma:
+def load_embedding_database(embedding_model: str, directory_path: "pathlib.Path") -> "Chroma":
     """Load vector store from disk from configured directory.
 
     Parameters
     ----------
     embedding_model : str
         name of Sentence Transformers model from Hugging Face
     directory_path : pathlib.Path
@@ -164,21 +168,21 @@
         case _:
             raise ValueError("Unexpected language model type")
 
     return LanguageModelAdapter.validate_python(language_model)
 
 
 def prepare_question_answer_chain(  # noqa: PLR0913
-    embedding_database: ValidatedChroma,
+    embedding_database: "Chroma",
     search_type: RetrievalType,
     number_of_documents: int,
     initial_number_of_documents: int,
     diversity_level: float,
     language_model: LanguageModel,
-) -> RunnableSerializable:
+) -> "RunnableSerializable":
     """Prepare a question answering pipeline.
 
     Parameters
     ----------
     embedding_database : Chroma
         vector store
     search_type : RetrievalType
@@ -208,15 +212,15 @@
 
     question_answer_chain = generate_retrieval_chain(database_retriever, llm)
 
     return question_answer_chain
 
 
 def run_question_answer_chain(
-    question_answer_chain: RunnableSerializable, question: str
+    question_answer_chain: "RunnableSerializable", question: str
 ) -> tuple[dict, CaptureDetailsCallback]:
     """Run question answering pipeline for user input.
 
     Parameters
     ----------
     question_answer_chain : RunnableSerializable
         question answering pipeline
```

### Comparing `query-package-documentation-0.0.2/src/generative_ai/information_retrieval/step_1_retrieval.py` & `query-package-documentation-0.0.3/src/generative_ai/information_retrieval/step_1_retrieval.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 """Define functionalities to store document embeddings."""
 
-import pathlib
+import typing
 
-from langchain.docstore.document import Document
 from langchain.text_splitter import RecursiveCharacterTextSplitter
 from langchain.vectorstores.chroma import Chroma
 from langchain_community.document_loaders import JSONLoader
 from langchain_community.embeddings import HuggingFaceEmbeddings
 
-from .utils_retrieval import ValidatedChroma
+if typing.TYPE_CHECKING:
+    import pathlib
 
+    from langchain.docstore.document import Document
 
-def load_json_documents(file_path: pathlib.Path) -> list[Document]:
+
+def load_json_documents(file_path: "pathlib.Path") -> list["Document"]:
     """Load retrieval documents from a JSON file.
 
     Parameters
     ----------
     file_path : pathlib.Path
         path to JSON file
 
@@ -26,15 +28,15 @@
     """
     json_loader = JSONLoader(file_path, ".retrieval_documents[]")
     raw_documents = json_loader.load()
 
     return raw_documents
 
 
-def partition_documents(raw_documents: list[Document]) -> list[Document]:
+def partition_documents(raw_documents: list["Document"]) -> list["Document"]:
     """Partition retrieval documents into chunks.
 
     Parameters
     ----------
     raw_documents : list[Document]
         retrieval documents
 
@@ -68,17 +70,15 @@
         document embedder
     """
     embedder = HuggingFaceEmbeddings(model_name=embedding_model)
 
     return embedder
 
 
-def create_vector_store(
-    embedder: HuggingFaceEmbeddings, directory_path: pathlib.Path
-) -> ValidatedChroma:
+def create_vector_store(embedder: HuggingFaceEmbeddings, directory_path: "pathlib.Path") -> Chroma:
     """Initialise a Chroma vector store.
 
     Parameters
     ----------
     embedder : HuggingFaceEmbeddings
         document embedder
     directory_path : pathlib.Path
```

### Comparing `query-package-documentation-0.0.2/src/generative_ai/information_retrieval/step_2_retrieval.py` & `query-package-documentation-0.0.3/src/generative_ai/information_retrieval/step_2_retrieval.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,32 @@
 """Define functionalities to fetch and use relevant information from database."""
 
+import typing
+
 import transformers
 from langchain.chains import RetrievalQA
-from langchain.chains.retrieval_qa.base import BaseRetrievalQA
 from langchain.llms.ctransformers import CTransformers
 from langchain.llms.huggingface_pipeline import HuggingFacePipeline
 from langchain.prompts import PromptTemplate
-from langchain.schema.vectorstore import VectorStoreRetriever
 
-from .utils_retrieval import LanguageModel, RetrievalType, TransformerType, ValidatedChroma
+from .utils_retrieval import LanguageModel, RetrievalType, TransformerType
+
+if typing.TYPE_CHECKING:
+    from langchain.chains.retrieval_qa.base import BaseRetrievalQA
+    from langchain.schema.vectorstore import VectorStoreRetriever
+    from langchain.vectorstores.chroma import Chroma
 
 
 def create_database_retriever(
-    embedding_database: ValidatedChroma,
+    embedding_database: "Chroma",
     search_type: RetrievalType,
     number_of_documents: int,
     initial_number_of_documents: int,
     diversity_level: float,
-) -> VectorStoreRetriever:
+) -> "VectorStoreRetriever":
     """Prepare a vector store retriever for the retrieval database.
 
     Parameters
     ----------
     embedding_database : Chroma
         vector store
     search_type : RetrievalType
@@ -103,14 +108,15 @@
             common_parameters.update({"do_sample": True, "top_k": 1})
 
             tokeniser = transformers.AutoTokenizer.from_pretrained(
                 language_model.standard_model_name,
                 use_fast=True,
                 padding="max_length",
                 truncation=True,
+                padding_side="left",
             )
             tokeniser.pad_token = tokeniser.eos_token
 
             pipeline = transformers.pipeline(
                 task=language_model.standard_pipeline_type,
                 model=language_model.standard_model_name,
                 tokenizer=tokeniser,
@@ -130,16 +136,16 @@
         case _:
             raise ValueError("Unexpected language model type")
 
     return llm
 
 
 def generate_retrieval_chain(
-    database_retriever: VectorStoreRetriever, llm: CTransformers | HuggingFacePipeline
-) -> BaseRetrievalQA:
+    database_retriever: "VectorStoreRetriever", llm: CTransformers | HuggingFacePipeline
+) -> "BaseRetrievalQA":
     """Prepare a retrieval chain for question answering.
 
     Parameters
     ----------
     database_retriever : VectorStoreRetriever
         vector store retriever
     llm : CTransformers | HuggingFacePipeline
@@ -151,33 +157,27 @@
         retrieval chain
 
     Notes
     -----
     * The prompt template instructs the model to not answer if it is missing in the context.
     * It also instructs the model to keep the answer as concise as possible.
     """
-    prompt_template = """You are a chat assistant for question answering tasks.
-
-Use the following retrieved context to answer the given question.
-
-If the answer is not in the context, say "I do not know.".
-
-Keep your answer as concise as possible.
-
-Context
+    prompt_template = """You are an assistant for question answering tasks.
 
-{context}
+### Instructions
 
-Question
+1. Use only the following retrieved context to answer the given question.
+2. If the answer is not in the context, say "I do not know.".
+3. Keep your answer as concise as possible.
 
-{question}
+### Context: {context}
 
-Answer
+### Question: {question}
 
-"""
+### Answer: """
 
     prompt = PromptTemplate.from_template(prompt_template)
 
     retrieval_chain = RetrievalQA.from_chain_type(
         llm,
         chain_type_kwargs={"prompt": prompt},
         retriever=database_retriever,
```

### Comparing `query-package-documentation-0.0.2/src/generative_ai/information_retrieval/step_3_retrieval.py` & `query-package-documentation-0.0.3/src/generative_ai/information_retrieval/step_3_retrieval.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,44 +1,47 @@
 """Define functionalities to debug large language model generation process."""
 
 import time
 import typing
-import uuid
 
 from langchain.callbacks.base import BaseCallbackHandler
-from langchain_core.outputs import LLMResult
+
+if typing.TYPE_CHECKING:
+    import uuid
+
+    from langchain_core.outputs import LLMResult
 
 
 class CaptureDetailsCallback(BaseCallbackHandler):
     """Capture details of question answering pipeline.
 
     Attributes
     ----------
     effective_prompt : str | None
         exact prompt passed to large language model after successful retrieval
     effective_duration : float | None
         time taken (in seconds) for large language model to generate response
     """
 
-    def __init__(self: "CaptureDetailsCallback") -> None:  # numpydoc ignore=GL08
+    def __init__(self: "CaptureDetailsCallback") -> None:
         super().__init__()
 
         self.effective_prompt: str | None = None
         self.effective_duration: float | None = None
 
     def on_llm_start(  # noqa: PLR0913, numpydoc ignore=PR01
         self: "CaptureDetailsCallback",
         serialized: dict,
         prompts: list[str],
         *,
-        run_id: uuid.UUID,
-        parent_run_id: uuid.UUID | None = None,
+        run_id: "uuid.UUID",
+        parent_run_id: "uuid.UUID | None" = None,
         tags: list[str] | None = None,
         metadata: dict | None = None,
-        **kwargs: typing.Any,
+        **kwargs: typing.Any,  # noqa: ANN401
     ) -> None:
         """Run when large language model starts generating response.
 
         Notes
         -----
         * This method only uses ``prompts`` argument, and rest are ignored.
         * This modifies ``self.effective_prompt`` and ``self.effective_duration`` attributes.
@@ -54,19 +57,19 @@
         del kwargs
 
         self.effective_prompt = prompts[0]
         self.effective_duration = time.perf_counter()
 
     def on_llm_end(  # numpydoc ignore=PR01
         self: "CaptureDetailsCallback",
-        response: LLMResult,
+        response: "LLMResult",
         *,
-        run_id: uuid.UUID,
-        parent_run_id: uuid.UUID | None = None,
-        **kwargs: typing.Any,
+        run_id: "uuid.UUID",
+        parent_run_id: "uuid.UUID | None" = None,
+        **kwargs: typing.Any,  # noqa: ANN401
     ) -> None:
         """Run when large language model finishes generating response.
 
         Notes
         -----
         * This method ignores all of its arguments.
         * This modifies ``self.effective_duration`` attribute.
```

### Comparing `query-package-documentation-0.0.2/src/generative_ai/information_retrieval/utils_retrieval.py` & `query-package-documentation-0.0.3/src/generative_ai/information_retrieval/utils_retrieval.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """Define functionalities for type annotations in information retrieval step."""
 
 import enum
 import typing
 
 import pydantic
-from langchain.vectorstores.chroma import Chroma
 
 
 class RetrievalType(str, enum.Enum):
     """Define supported retrieval types."""
 
     MMR = "mmr"
     SIMILARITY = "similarity"
@@ -68,20 +67,17 @@
 
 
 LanguageModel = typing.Annotated[
     QuantisedModel | StandardModel, pydantic.Field(discriminator="language_model_type")
 ]
 LanguageModelAdapter = pydantic.TypeAdapter(LanguageModel)
 
-ValidatedChroma = pydantic.InstanceOf[Chroma]
-
 
 __all__ = [
     "LanguageModel",
     "LanguageModelAdapter",
     "TransformerType",
     "PipelineType",
     "QuantisedModel",
     "RetrievalType",
     "StandardModel",
-    "ValidatedChroma",
 ]
```

### Comparing `query-package-documentation-0.0.2/src/generative_ai/metadata.json` & `query-package-documentation-0.0.3/src/generative_ai/metadata.json`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9375%*

 * *Differences: {"'Version'": "'0.0.3'"}*

```diff
@@ -13,9 +13,9 @@
         "Documentation": "https://query-package-documentation.readthedocs.io",
         "Source Code": "https://github.com/yarnabrina/query-package-documentation"
     },
     "Maintainers": [
         "Anirban Ray <39331844+yarnabrina@users.noreply.github.com>"
     ],
     "Name": "query-package-documentation",
-    "Version": "0.0.2"
+    "Version": "0.0.3"
 }
```

### Comparing `query-package-documentation-0.0.2/src/generative_ai/top_level.py` & `query-package-documentation-0.0.3/src/generative_ai/top_level.py`

 * *Files identical despite different names*

### Comparing `query-package-documentation-0.0.2/src/generative_ai/utils_top_level.py` & `query-package-documentation-0.0.3/src/generative_ai/utils_top_level.py`

 * *Files identical despite different names*

### Comparing `query-package-documentation-0.0.2/src/gui.py` & `query-package-documentation-0.0.3/src/gui.py`

 * *Files identical despite different names*

### Comparing `query-package-documentation-0.0.2/src/query_package_documentation.egg-info/PKG-INFO` & `query-package-documentation-0.0.3/src/query_package_documentation.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: query-package-documentation
-Version: 0.0.2
+Version: 0.0.3
 Summary: A package to explore documentations
 Author-email: Anirban Ray <39331844+yarnabrina@users.noreply.github.com>
 Maintainer-email: Anirban Ray <39331844+yarnabrina@users.noreply.github.com>
 License: MIT License
         
-        Copyright (c) 2023 Anirban Ray
+        Copyright (c) 2023-2024 Anirban Ray
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
         to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
         copies of the Software, and to permit persons to whom the Software is
         furnished to do so, subject to the following conditions:
@@ -47,22 +47,22 @@
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Python: ==3.11.*
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: chromadb<0.5,>=0.4.15
 Requires-Dist: ctransformers<0.3,>=0.2.27
-Requires-Dist: gradio<4.17,>=4.12
-Requires-Dist: jq<1.7,>=1.6
-Requires-Dist: langchain<0.1.5,>=0.1.1
-Requires-Dist: numpydoc<1.7,>=1.6
-Requires-Dist: pydantic<2.6,>=2.4.2
-Requires-Dist: sentence-transformers<2.3,>=2.2.2
-Requires-Dist: transformers<4.38,>=4.36
-Requires-Dist: typer<0.10,>=0.9
+Requires-Dist: gradio<4.26,>=4.19.2
+Requires-Dist: jq<1.8,>=1.6
+Requires-Dist: langchain<0.2,>=0.1.13
+Requires-Dist: numpydoc<1.8,>=1.6
+Requires-Dist: pydantic<2.7,>=2.4.2
+Requires-Dist: sentence-transformers<2.7,>=2.2.2
+Requires-Dist: transformers<4.39,>=4.36
+Requires-Dist: typer-slim<0.13,>=0.12.1
 Provides-Extra: all
 Requires-Dist: autoflake; extra == "all"
 Requires-Dist: bandit; extra == "all"
 Requires-Dist: black; extra == "all"
 Requires-Dist: blacken-docs; extra == "all"
 Requires-Dist: build; extra == "all"
 Requires-Dist: codespell; extra == "all"
@@ -88,22 +88,24 @@
 Requires-Dist: pre-commit; extra == "dev"
 Provides-Extra: doc
 Requires-Dist: furo; extra == "doc"
 Requires-Dist: myst-parser[linkify]; extra == "doc"
 Requires-Dist: Sphinx; extra == "doc"
 Requires-Dist: sphinx-copybutton; extra == "doc"
 Provides-Extra: fine-tuning
-Requires-Dist: accelerate<0.27,>=0.24.1; extra == "fine-tuning"
-Requires-Dist: bitsandbytes<0.43,>=0.41.2; extra == "fine-tuning"
-Requires-Dist: datasets<2.17,>=2.15; extra == "fine-tuning"
-Requires-Dist: peft<0.8,>=0.6.2; extra == "fine-tuning"
+Requires-Dist: accelerate<0.30,>=0.24.1; extra == "fine-tuning"
+Requires-Dist: bitsandbytes<0.44,>=0.41.2; extra == "fine-tuning"
+Requires-Dist: datasets<2.19,>=2.15; extra == "fine-tuning"
+Requires-Dist: evaluate<0.5,>=0.4.1; extra == "fine-tuning"
+Requires-Dist: peft<0.11,>=0.6.2; extra == "fine-tuning"
+Requires-Dist: rouge-score<0.2,>=0.1.2; extra == "fine-tuning"
 Requires-Dist: safetensors<0.5,>=0.4; extra == "fine-tuning"
-Requires-Dist: torch<2.2,>=2.1.1; extra == "fine-tuning"
-Requires-Dist: transformers<4.38,>=4.36; extra == "fine-tuning"
-Requires-Dist: trl<0.8,>=0.7.4; extra == "fine-tuning"
+Requires-Dist: scikit-learn<1.5,>=1.3; extra == "fine-tuning"
+Requires-Dist: torch<2.3,>=2.1.1; extra == "fine-tuning"
+Requires-Dist: trl<0.9,>=0.7.4; extra == "fine-tuning"
 Provides-Extra: format
 Requires-Dist: autoflake; extra == "format"
 Requires-Dist: black; extra == "format"
 Requires-Dist: blacken-docs; extra == "format"
 Requires-Dist: docformatter[tomli]; extra == "format"
 Requires-Dist: isort; extra == "format"
 Requires-Dist: pyproject-fmt; extra == "format"
```

### Comparing `query-package-documentation-0.0.2/src/query_package_documentation.egg-info/SOURCES.txt` & `query-package-documentation-0.0.3/src/query_package_documentation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `query-package-documentation-0.0.2/src/query_package_documentation.egg-info/requires.txt` & `query-package-documentation-0.0.3/src/query_package_documentation.egg-info/requires.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 chromadb<0.5,>=0.4.15
 ctransformers<0.3,>=0.2.27
-gradio<4.17,>=4.12
-jq<1.7,>=1.6
-langchain<0.1.5,>=0.1.1
-numpydoc<1.7,>=1.6
-pydantic<2.6,>=2.4.2
-sentence-transformers<2.3,>=2.2.2
-transformers<4.38,>=4.36
-typer<0.10,>=0.9
+gradio<4.26,>=4.19.2
+jq<1.8,>=1.6
+langchain<0.2,>=0.1.13
+numpydoc<1.8,>=1.6
+pydantic<2.7,>=2.4.2
+sentence-transformers<2.7,>=2.2.2
+transformers<4.39,>=4.36
+typer-slim<0.13,>=0.12.1
 
 [all]
 autoflake
 bandit
 black
 blacken-docs
 build
@@ -41,22 +41,24 @@
 [doc]
 furo
 myst-parser[linkify]
 Sphinx
 sphinx-copybutton
 
 [fine-tuning]
-accelerate<0.27,>=0.24.1
-bitsandbytes<0.43,>=0.41.2
-datasets<2.17,>=2.15
-peft<0.8,>=0.6.2
+accelerate<0.30,>=0.24.1
+bitsandbytes<0.44,>=0.41.2
+datasets<2.19,>=2.15
+evaluate<0.5,>=0.4.1
+peft<0.11,>=0.6.2
+rouge-score<0.2,>=0.1.2
 safetensors<0.5,>=0.4
-torch<2.2,>=2.1.1
-transformers<4.38,>=4.36
-trl<0.8,>=0.7.4
+scikit-learn<1.5,>=1.3
+torch<2.3,>=2.1.1
+trl<0.9,>=0.7.4
 
 [format]
 autoflake
 black
 blacken-docs
 docformatter[tomli]
 isort
```

