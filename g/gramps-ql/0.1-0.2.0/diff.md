# Comparing `tmp/gramps-ql-0.1.tar.gz` & `tmp/gramps-ql-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gramps-ql-0.1.tar", last modified: Thu Apr  4 19:40:38 2024, max compression
+gzip compressed data, was "gramps-ql-0.2.0.tar", last modified: Sun Apr  7 19:10:54 2024, max compression
```

## Comparing `gramps-ql-0.1.tar` & `gramps-ql-0.2.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:40:38.335069 gramps-ql-0.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:40:38.331069 gramps-ql-0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:40:38.331069 gramps-ql-0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-04 19:40:33.000000 gramps-ql-0.1/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      856 2024-04-04 19:40:33.000000 gramps-ql-0.1/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-04 19:40:33.000000 gramps-ql-0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-04 19:40:33.000000 gramps-ql-0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      933 2024-04-04 19:40:38.335069 gramps-ql-0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      523 2024-04-04 19:40:33.000000 gramps-ql-0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-04 19:40:33.000000 gramps-ql-0.1/mypy.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      728 2024-04-04 19:40:33.000000 gramps-ql-0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 19:40:38.335069 gramps-ql-0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-04 19:40:33.000000 gramps-ql-0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:40:38.331069 gramps-ql-0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:40:38.335069 gramps-ql-0.1/src/gramps_ql/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-04 19:40:33.000000 gramps-ql-0.1/src/gramps_ql/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-04 19:40:33.000000 gramps-ql-0.1/src/gramps_ql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-04-04 19:40:38.000000 gramps-ql-0.1/src/gramps_ql/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     5403 2024-04-04 19:40:33.000000 gramps-ql-0.1/src/gramps_ql/gql.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:40:38.335069 gramps-ql-0.1/src/gramps_ql.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      933 2024-04-04 19:40:38.000000 gramps-ql-0.1/src/gramps_ql.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      496 2024-04-04 19:40:38.000000 gramps-ql-0.1/src/gramps_ql.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 19:40:38.000000 gramps-ql-0.1/src/gramps_ql.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-04 19:40:38.000000 gramps-ql-0.1/src/gramps_ql.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-04 19:40:38.000000 gramps-ql-0.1/src/gramps_ql.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:40:38.331069 gramps-ql-0.1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:40:38.335069 gramps-ql-0.1/tests/gramps_ql/
--rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-04-04 19:40:33.000000 gramps-ql-0.1/tests/gramps_ql/test_iter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-04-04 19:40:33.000000 gramps-ql-0.1/tests/gramps_ql/test_match.py
--rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-04-04 19:40:33.000000 gramps-ql-0.1/tests/gramps_ql/test_parse.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 19:10:54.854777 gramps-ql-0.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 19:10:54.850777 gramps-ql-0.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 19:10:54.850777 gramps-ql-0.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-07 19:10:44.000000 gramps-ql-0.2.0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-04-07 19:10:44.000000 gramps-ql-0.2.0/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-07 19:10:44.000000 gramps-ql-0.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-07 19:10:44.000000 gramps-ql-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    11888 2024-04-07 19:10:54.854777 gramps-ql-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11477 2024-04-07 19:10:44.000000 gramps-ql-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-07 19:10:44.000000 gramps-ql-0.2.0/mypy.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-04-07 19:10:44.000000 gramps-ql-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 19:10:54.854777 gramps-ql-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-07 19:10:44.000000 gramps-ql-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 19:10:54.850777 gramps-ql-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 19:10:54.854777 gramps-ql-0.2.0/src/gramps_ql/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-07 19:10:44.000000 gramps-ql-0.2.0/src/gramps_ql/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-07 19:10:44.000000 gramps-ql-0.2.0/src/gramps_ql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-07 19:10:54.000000 gramps-ql-0.2.0/src/gramps_ql/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6909 2024-04-07 19:10:44.000000 gramps-ql-0.2.0/src/gramps_ql/gql.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 19:10:54.854777 gramps-ql-0.2.0/src/gramps_ql.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11888 2024-04-07 19:10:54.000000 gramps-ql-0.2.0/src/gramps_ql.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-04-07 19:10:54.000000 gramps-ql-0.2.0/src/gramps_ql.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 19:10:54.000000 gramps-ql-0.2.0/src/gramps_ql.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-07 19:10:54.000000 gramps-ql-0.2.0/src/gramps_ql.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-07 19:10:54.000000 gramps-ql-0.2.0/src/gramps_ql.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 19:10:54.850777 gramps-ql-0.2.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 19:10:54.854777 gramps-ql-0.2.0/tests/gramps_ql/
+-rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-04-07 19:10:44.000000 gramps-ql-0.2.0/tests/gramps_ql/test_iter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3640 2024-04-07 19:10:44.000000 gramps-ql-0.2.0/tests/gramps_ql/test_match.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-04-07 19:10:44.000000 gramps-ql-0.2.0/tests/gramps_ql/test_parse.py
```

### Comparing `gramps-ql-0.1/.github/workflows/python-publish.yml` & `gramps-ql-0.2.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `gramps-ql-0.1/.github/workflows/test.yml` & `gramps-ql-0.2.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `gramps-ql-0.1/LICENSE` & `gramps-ql-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gramps-ql-0.1/pyproject.toml` & `gramps-ql-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gramps-ql-0.1/src/gramps_ql/gql.py` & `gramps-ql-0.2.0/src/gramps_ql/gql.py`

 * *Files 21% similar despite different names*

```diff
@@ -127,29 +127,66 @@
         if not parsed:
             raise ValueError(f"Unable to parse left-hand side: {lhs}")
         for i, part in enumerate(parsed):
             if i == 0:
                 result = obj.get(parsed[0])
             elif part in ["[", "]", "."]:
                 continue
+            elif part == "length":
+                result = len(result)
+            elif part in ["all", "any"]:
+                if i + 1 == len(parsed):  # last item
+                    results = [
+                        self._match_values(item, operator, rhs) for item in result
+                    ]
+                elif len(parsed) > i + 1 and parsed[i + 1] == ".":
+                    lhs_rest = "".join(parsed[i + 2 :])
+                    results = [
+                        self._match_single(item, lhs_rest, operator, rhs)
+                        for item in result
+                    ]
+                else:
+                    raise ValueError(f"'any' cannot be followed by {parsed[i + 1]}")
+                try:
+                    if part == "all":
+                        return results and all(results)  # because all([]) is True
+                    else:
+                        return any(results)
+                except TypeError:
+                    return False
             else:
                 try:
                     result = result[part]
                 except (KeyError, IndexError):
                     return False
             if result is None:
                 return False
+        return self._match_values(result, operator, rhs)
+
+    def _match_values(self, result, operator: str = "", rhs: str = "") -> bool:
+        """Match two values."""
         if not operator:
             return bool(result)
         if isinstance(rhs, str):
-            rhs = rhs.strip("\"'")
+            if rhs.isdigit():
+                rhs = int(rhs)
+            else:
+                rhs = rhs.strip("\"'")
         if operator == "=":
             return result == rhs
         if operator == "!=":
             return result != rhs
+        if operator == "~":
+            if isinstance(result, str):
+                rhs = str(rhs)
+            return rhs in result
+        if operator == "!~":
+            if isinstance(result, str):
+                rhs = str(rhs)
+            return rhs not in result
         try:
             if operator == "<":
                 return result < rhs
             if operator == ">":
                 return result > rhs
             if operator == "<=":
                 return result <= rhs
```

### Comparing `gramps-ql-0.1/tests/gramps_ql/test_iter.py` & `gramps-ql-0.2.0/tests/gramps_ql/test_iter.py`

 * *Files identical despite different names*

### Comparing `gramps-ql-0.1/tests/gramps_ql/test_parse.py` & `gramps-ql-0.2.0/tests/gramps_ql/test_parse.py`

 * *Files identical despite different names*

