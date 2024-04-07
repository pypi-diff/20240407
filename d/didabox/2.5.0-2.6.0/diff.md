# Comparing `tmp/didabox-2.5.0.tar.gz` & `tmp/didabox-2.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "didabox-2.5.0.tar", max compression
+gzip compressed data, was "didabox-2.6.0.tar", max compression
```

## Comparing `didabox-2.5.0.tar` & `didabox-2.6.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1082 2024-03-29 03:41:43.513060 didabox-2.5.0/LICENSE
--rw-r--r--   0        0        0      350 2024-04-03 08:52:11.021744 didabox-2.5.0/pyproject.toml
--rw-r--r--   0        0        0      107 2024-03-29 03:41:43.514059 didabox-2.5.0/README.md
--rw-r--r--   0        0        0      146 2024-03-29 03:41:43.515059 didabox-2.5.0/src/didabox/__init__.py
--rw-r--r--   0        0        0      712 2024-03-29 03:41:43.516059 didabox-2.5.0/src/didabox/check.py
--rw-r--r--   0        0        0      600 2024-04-03 05:26:21.967501 didabox-2.5.0/src/didabox/info.py
--rw-r--r--   0        0        0      591 2024-03-29 03:41:43.516059 didabox-2.5.0/src/didabox/login.py
--rw-r--r--   0        0        0     2136 2024-04-03 08:51:54.701507 didabox-2.5.0/src/didabox/main.py
--rw-r--r--   0        0        0     1412 2024-03-29 03:41:43.516059 didabox-2.5.0/src/didabox/request.py
--rw-r--r--   0        0        0     2674 2024-04-03 08:37:31.015779 didabox-2.5.0/src/didabox/task.py
--rw-r--r--   0        0        0     1999 2024-03-29 03:41:43.517060 didabox-2.5.0/src/didabox/utils.py
--rw-r--r--   0        0        0      826 1970-01-01 00:00:00.000000 didabox-2.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1082 2024-03-29 03:41:43.513060 didabox-2.6.0/LICENSE
+-rw-r--r--   0        0        0      350 2024-04-07 05:02:44.008828 didabox-2.6.0/pyproject.toml
+-rw-r--r--   0        0        0      107 2024-03-29 03:41:43.514059 didabox-2.6.0/README.md
+-rw-r--r--   0        0        0      146 2024-03-29 03:41:43.515059 didabox-2.6.0/src/didabox/__init__.py
+-rw-r--r--   0        0        0      712 2024-03-29 03:41:43.516059 didabox-2.6.0/src/didabox/check.py
+-rw-r--r--   0        0        0      600 2024-04-03 05:26:21.967501 didabox-2.6.0/src/didabox/info.py
+-rw-r--r--   0        0        0      591 2024-03-29 03:41:43.516059 didabox-2.6.0/src/didabox/login.py
+-rw-r--r--   0        0        0     2286 2024-04-07 03:39:08.181056 didabox-2.6.0/src/didabox/main.py
+-rw-r--r--   0        0        0     1412 2024-03-29 03:41:43.516059 didabox-2.6.0/src/didabox/request.py
+-rw-r--r--   0        0        0     2897 2024-04-07 03:35:13.461196 didabox-2.6.0/src/didabox/task.py
+-rw-r--r--   0        0        0     1999 2024-03-29 03:41:43.517060 didabox-2.6.0/src/didabox/utils.py
+-rw-r--r--   0        0        0      826 1970-01-01 00:00:00.000000 didabox-2.6.0/PKG-INFO
```

### Comparing `didabox-2.5.0/LICENSE` & `didabox-2.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `didabox-2.5.0/src/didabox/check.py` & `didabox-2.6.0/src/didabox/check.py`

 * *Files identical despite different names*

### Comparing `didabox-2.5.0/src/didabox/info.py` & `didabox-2.6.0/src/didabox/info.py`

 * *Files identical despite different names*

### Comparing `didabox-2.5.0/src/didabox/login.py` & `didabox-2.6.0/src/didabox/login.py`

 * *Files identical despite different names*

### Comparing `didabox-2.5.0/src/didabox/main.py` & `didabox-2.6.0/src/didabox/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -61,8 +61,11 @@
         获取已完成的任务
         :param to_date: 格式 2024-03-28 00:57:26
         :param from_date:
         :param limit:
         """
         return self.task_box.all_completed(from_date=from_date, to_date=to_date, limit=limit)
 
+    def search(self, keywords: str) -> Response:
+        """根据关键词查询相关任务"""
+        return self.task_box.search_all(keywords)
     # -- 清单任务维度 --
```

### Comparing `didabox-2.5.0/src/didabox/request.py` & `didabox-2.6.0/src/didabox/request.py`

 * *Files identical despite different names*

### Comparing `didabox-2.5.0/src/didabox/task.py` & `didabox-2.6.0/src/didabox/task.py`

 * *Files 12% similar despite different names*

```diff
@@ -74,7 +74,13 @@
             "to": to_date,
             "limit": str(limit)
         }
         # 冒号不能转义 (= =)
         encoded_params = urlencode(params, safe=":")
         response = self.req.get("https://api.dida365.com/api/v2/project/all/completed/?" + encoded_params, params={})
         return response
+
+    def search_all(self, keyword: str):
+        """搜索"""
+        params = {'keywords': keyword}
+        response = self.req.get('https://api.dida365.com/api/v2/search/all', params=params)
+        return response
```

### Comparing `didabox-2.5.0/src/didabox/utils.py` & `didabox-2.6.0/src/didabox/utils.py`

 * *Files identical despite different names*

### Comparing `didabox-2.5.0/PKG-INFO` & `didabox-2.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: didabox
-Version: 2.5.0
+Version: 2.6.0
 Summary: dida api
 License: MIT
 Author: luke9012
 Author-email: luke781520097@163.com
 Requires-Python: >=3.6
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

