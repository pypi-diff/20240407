# Comparing `tmp/thulearn2018-2.4.2.tar.gz` & `tmp/thulearn2018-2.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thulearn2018-2.4.2.tar", last modified: Mon Mar 25 15:09:58 2024, max compression
+gzip compressed data, was "thulearn2018-2.4.3.tar", last modified: Sun Apr  7 11:24:18 2024, max compression
```

## Comparing `thulearn2018-2.4.2.tar` & `thulearn2018-2.4.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-x---   0 hyr       (1000) hyr       (1000)        0 2024-03-25 15:09:58.626322 thulearn2018-2.4.2/
--rw-r--r--   0 hyr       (1000) hyr       (1000)       75 2023-09-13 09:31:57.000000 thulearn2018-2.4.2/.gitignore
--rw-r--r--   0 hyr       (1000) hyr       (1000)     1074 2023-09-13 09:31:57.000000 thulearn2018-2.4.2/LICENSE
--rw-r--r--   0 hyr       (1000) hyr       (1000)      716 2024-03-25 15:09:58.626322 thulearn2018-2.4.2/PKG-INFO
--rw-r-----   0 hyr       (1000) hyr       (1000)     5277 2024-03-24 16:37:48.000000 thulearn2018-2.4.2/README.md
--rw-r-----   0 hyr       (1000) hyr       (1000)       38 2024-03-25 15:09:58.626322 thulearn2018-2.4.2/setup.cfg
--rw-r--r--   0 hyr       (1000) hyr       (1000)     2540 2024-03-25 15:09:54.000000 thulearn2018-2.4.2/setup.py
-drwxr-x---   0 hyr       (1000) hyr       (1000)        0 2024-03-25 15:09:58.622322 thulearn2018-2.4.2/thulearn2018/
--rw-r--r--   0 hyr       (1000) hyr       (1000)       22 2023-09-13 09:31:57.000000 thulearn2018-2.4.2/thulearn2018/__init__.py
--rw-r-----   0 hyr       (1000) hyr       (1000)    10558 2024-03-25 15:06:19.000000 thulearn2018-2.4.2/thulearn2018/browser.py
--rw-r-----   0 hyr       (1000) hyr       (1000)     5708 2024-03-25 14:56:30.000000 thulearn2018-2.4.2/thulearn2018/filemanager.py
--rw-r--r--   0 hyr       (1000) hyr       (1000)      415 2023-10-20 16:40:42.000000 thulearn2018-2.4.2/thulearn2018/jsonhelper.py
--rw-r--r--   0 hyr       (1000) hyr       (1000)     3596 2023-11-28 10:16:52.000000 thulearn2018-2.4.2/thulearn2018/learn.py
--rw-r--r--   0 hyr       (1000) hyr       (1000)     3207 2023-11-28 10:29:46.000000 thulearn2018-2.4.2/thulearn2018/settings.py
--rw-r-----   0 hyr       (1000) hyr       (1000)     3941 2024-03-25 12:36:49.000000 thulearn2018-2.4.2/thulearn2018/soup.py
--rw-r--r--   0 hyr       (1000) hyr       (1000)     1105 2023-11-28 10:17:17.000000 thulearn2018-2.4.2/thulearn2018/utils.py
-drwxr-x---   0 hyr       (1000) hyr       (1000)        0 2024-03-25 15:09:58.626322 thulearn2018-2.4.2/thulearn2018.egg-info/
--rw-r--r--   0 hyr       (1000) hyr       (1000)      716 2024-03-25 15:09:58.000000 thulearn2018-2.4.2/thulearn2018.egg-info/PKG-INFO
--rw-r--r--   0 hyr       (1000) hyr       (1000)      449 2024-03-25 15:09:58.000000 thulearn2018-2.4.2/thulearn2018.egg-info/SOURCES.txt
--rw-r--r--   0 hyr       (1000) hyr       (1000)        1 2024-03-25 15:09:58.000000 thulearn2018-2.4.2/thulearn2018.egg-info/dependency_links.txt
--rw-r--r--   0 hyr       (1000) hyr       (1000)       50 2024-03-25 15:09:58.000000 thulearn2018-2.4.2/thulearn2018.egg-info/entry_points.txt
--rw-r--r--   0 hyr       (1000) hyr       (1000)       79 2024-03-25 15:09:58.000000 thulearn2018-2.4.2/thulearn2018.egg-info/requires.txt
--rw-r--r--   0 hyr       (1000) hyr       (1000)       13 2024-03-25 15:09:58.000000 thulearn2018-2.4.2/thulearn2018.egg-info/top_level.txt
+drwxr-x---   0 hyr       (1000) hyr       (1000)        0 2024-04-07 11:24:18.585221 thulearn2018-2.4.3/
+-rw-r--r--   0 hyr       (1000) hyr       (1000)       75 2023-09-13 09:31:57.000000 thulearn2018-2.4.3/.gitignore
+-rw-r--r--   0 hyr       (1000) hyr       (1000)     1074 2023-09-13 09:31:57.000000 thulearn2018-2.4.3/LICENSE
+-rw-r--r--   0 hyr       (1000) hyr       (1000)      716 2024-04-07 11:24:18.585221 thulearn2018-2.4.3/PKG-INFO
+-rw-r-----   0 hyr       (1000) hyr       (1000)     5277 2024-04-07 05:13:15.000000 thulearn2018-2.4.3/README.md
+-rw-r-----   0 hyr       (1000) hyr       (1000)       38 2024-04-07 11:24:18.585221 thulearn2018-2.4.3/setup.cfg
+-rw-r-----   0 hyr       (1000) hyr       (1000)     2540 2024-04-07 11:21:35.000000 thulearn2018-2.4.3/setup.py
+drwxr-x---   0 hyr       (1000) hyr       (1000)        0 2024-04-07 11:24:18.585221 thulearn2018-2.4.3/thulearn2018/
+-rw-r--r--   0 hyr       (1000) hyr       (1000)       22 2023-09-13 09:31:57.000000 thulearn2018-2.4.3/thulearn2018/__init__.py
+-rw-r-----   0 hyr       (1000) hyr       (1000)    10580 2024-04-07 11:23:07.000000 thulearn2018-2.4.3/thulearn2018/browser.py
+-rw-r-----   0 hyr       (1000) hyr       (1000)     5708 2024-04-07 05:13:21.000000 thulearn2018-2.4.3/thulearn2018/filemanager.py
+-rw-r-----   0 hyr       (1000) hyr       (1000)      415 2024-04-07 05:12:59.000000 thulearn2018-2.4.3/thulearn2018/jsonhelper.py
+-rw-r-----   0 hyr       (1000) hyr       (1000)     3596 2024-04-07 05:13:14.000000 thulearn2018-2.4.3/thulearn2018/learn.py
+-rw-r-----   0 hyr       (1000) hyr       (1000)     3207 2024-04-07 05:13:14.000000 thulearn2018-2.4.3/thulearn2018/settings.py
+-rw-r-----   0 hyr       (1000) hyr       (1000)     3941 2024-04-07 05:13:20.000000 thulearn2018-2.4.3/thulearn2018/soup.py
+-rw-r-----   0 hyr       (1000) hyr       (1000)     1263 2024-04-07 10:52:59.000000 thulearn2018-2.4.3/thulearn2018/utils.py
+drwxr-x---   0 hyr       (1000) hyr       (1000)        0 2024-04-07 11:24:18.585221 thulearn2018-2.4.3/thulearn2018.egg-info/
+-rw-r--r--   0 hyr       (1000) hyr       (1000)      716 2024-04-07 11:24:18.000000 thulearn2018-2.4.3/thulearn2018.egg-info/PKG-INFO
+-rw-r--r--   0 hyr       (1000) hyr       (1000)      449 2024-04-07 11:24:18.000000 thulearn2018-2.4.3/thulearn2018.egg-info/SOURCES.txt
+-rw-r--r--   0 hyr       (1000) hyr       (1000)        1 2024-04-07 11:24:18.000000 thulearn2018-2.4.3/thulearn2018.egg-info/dependency_links.txt
+-rw-r--r--   0 hyr       (1000) hyr       (1000)       50 2024-04-07 11:24:18.000000 thulearn2018-2.4.3/thulearn2018.egg-info/entry_points.txt
+-rw-r--r--   0 hyr       (1000) hyr       (1000)       79 2024-04-07 11:24:18.000000 thulearn2018-2.4.3/thulearn2018.egg-info/requires.txt
+-rw-r--r--   0 hyr       (1000) hyr       (1000)       13 2024-04-07 11:24:18.000000 thulearn2018-2.4.3/thulearn2018.egg-info/top_level.txt
```

### Comparing `thulearn2018-2.4.2/LICENSE` & `thulearn2018-2.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `thulearn2018-2.4.2/PKG-INFO` & `thulearn2018-2.4.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thulearn2018
-Version: 2.4.2
+Version: 2.4.3
 Summary: Tools for Web Learning of Tsinghua University
 Home-page: https://github.com/euxcet/thulearn2018
 Author: Chengchi Zhou, Yingtian Liu, Yurui Hong
 Author-email: zcc16@mails.tsinghua.edu.cn, liu-yt16@mails.tsinghua.edu.cn,yuruihong02@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `thulearn2018-2.4.2/README.md` & `thulearn2018-2.4.3/README.md`

 * *Files identical despite different names*

### Comparing `thulearn2018-2.4.2/setup.py` & `thulearn2018-2.4.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="thulearn2018",
-    version="2.4.2",
+    version="2.4.3",
     author="Chengchi Zhou, Yingtian Liu, Yurui Hong",
     author_email="zcc16@mails.tsinghua.edu.cn, liu-yt16@mails.tsinghua.edu.cn,"
                  "yuruihong02@outlook.com",
     description="Tools for Web Learning of Tsinghua University",
     long_description="Tools for Web Learning of Tsinghua University",
     long_description_content_type="text/markdown",
     url="https://github.com/euxcet/thulearn2018",
```

### Comparing `thulearn2018-2.4.2/thulearn2018/browser.py` & `thulearn2018-2.4.3/thulearn2018/browser.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,18 +83,16 @@
                        settings.local_file_path)
         self.local = self.fm.get_local()
 
     # -------------------------------------------------------------------------
     def get_lessons(self, exclude=[], include=[]):
         content = self.jh.loads(self.post(settings.lessons_url(self.semester)))
         # first sort by lesson name, then sort by teacher name
-        lessons = [[x["wlkcid"], x["kcm"], x["jsm"], x["kch"]]
-                   for x in content["resultList"] if x["kcm"] not in exclude]
-        if include != []:
-            lessons = [lesson for lesson in lessons if lesson[1] in include]
+        lessons = [[x["wlkcid"], utils.escape_str(x["kcm"]), x["jsm"], x["kch"]]
+                   for x in content["resultList"] if (x["kcm"] not in exclude) and (include == [] or x["kcm"] in include or utils.escape_str(x["kcm"]) in include)]
 
         lessons.sort(key=lambda x: (x[1], x[2]))
 
         # create a helper function to determine the folder name
         for i in range(len(lessons)):
             _, kcm, jsm, kch = lessons[i]
 
@@ -102,23 +100,21 @@
             # determine the naming method of the current lesson
             prev_lesson = lessons[i-1] if i-1 >= 0 else None
             next_lesson = lessons[i+1] if i+1 < len(lessons) else None
 
             if (prev_lesson is None or prev_lesson[1] != kcm) and \
                (next_lesson is None or next_lesson[1] != kcm):
                 lessons[i].append(kcm)
-
-            if (prev_lesson is None or prev_lesson[1] != kcm or
+            elif (prev_lesson is None or prev_lesson[1] != kcm or
                prev_lesson[2] != jsm) and \
                (next_lesson is None or next_lesson[1] != kcm or
                next_lesson[2] != jsm):
                 lessons[i].append(f"{kcm}_{jsm}")
-
-            lessons[i].append(f"{kcm}_{kch}")
-
+            else:
+                lessons[i].append(f"{kcm}_{kch}")
         return lessons
 
     def init_lessons(self, exclude, include):
         lessons = self.get_lessons(exclude=exclude, include=include)
 
         for i in range(len(lessons)):
             self.fm.mkdirl(os.path.join(self.path, lessons[i][4]))
```

### Comparing `thulearn2018-2.4.2/thulearn2018/filemanager.py` & `thulearn2018-2.4.3/thulearn2018/filemanager.py`

 * *Files identical despite different names*

### Comparing `thulearn2018-2.4.2/thulearn2018/learn.py` & `thulearn2018-2.4.3/thulearn2018/learn.py`

 * *Files identical despite different names*

### Comparing `thulearn2018-2.4.2/thulearn2018/settings.py` & `thulearn2018-2.4.3/thulearn2018/settings.py`

 * *Files identical despite different names*

### Comparing `thulearn2018-2.4.2/thulearn2018/soup.py` & `thulearn2018-2.4.3/thulearn2018/soup.py`

 * *Files identical despite different names*

### Comparing `thulearn2018-2.4.2/thulearn2018/utils.py` & `thulearn2018-2.4.3/thulearn2018/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -32,7 +32,17 @@
     delta = datetime.datetime(tl[0], tl[1], tl[2], tl[3], tl[4], 0, 0) - \
         (datetime.datetime.utcnow() + datetime.timedelta(hours=8))
     return seconds_to_string(delta.days*24*60*60+delta.seconds)
 
 
 def expired(timeStr):
     return timeStr < datetime.datetime.now().strftime("%Y-%m-%d %H:%M:%S")
+
+
+def escape_str(s):
+    rules = {
+        '/': '、',
+        '&mdash;' : '—'
+    }
+    for k, v in rules.items():
+        s = s.replace(k, v)
+    return s
```

### Comparing `thulearn2018-2.4.2/thulearn2018.egg-info/PKG-INFO` & `thulearn2018-2.4.3/thulearn2018.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thulearn2018
-Version: 2.4.2
+Version: 2.4.3
 Summary: Tools for Web Learning of Tsinghua University
 Home-page: https://github.com/euxcet/thulearn2018
 Author: Chengchi Zhou, Yingtian Liu, Yurui Hong
 Author-email: zcc16@mails.tsinghua.edu.cn, liu-yt16@mails.tsinghua.edu.cn,yuruihong02@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

