# Comparing `tmp/ncmlistdownloader-1.0.0.240405a1.tar.gz` & `tmp/ncmlistdownloader-1.0.0.240407b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ncmlistdownloader-1.0.0.240405a1.tar", last modified: Fri Apr  5 14:41:52 2024, max compression
+gzip compressed data, was "ncmlistdownloader-1.0.0.240407b1.tar", last modified: Sun Apr  7 14:49:27 2024, max compression
```

## Comparing `ncmlistdownloader-1.0.0.240405a1.tar` & `ncmlistdownloader-1.0.0.240407b1.tar`

### file list

```diff
@@ -1,28 +1,27 @@
-drwxrwxrwx   0        0        0        0 2024-04-05 14:41:52.256347 ncmlistdownloader-1.0.0.240405a1/
--rw-rw-rw-   0        0        0    35181 2024-02-12 02:33:29.000000 ncmlistdownloader-1.0.0.240405a1/LICENSE
--rw-rw-rw-   0        0        0       18 2024-02-15 05:12:55.000000 ncmlistdownloader-1.0.0.240405a1/MANIFEST.in
--rw-rw-rw-   0        0        0     1399 2024-04-05 14:41:52.253346 ncmlistdownloader-1.0.0.240405a1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-05 14:41:52.179348 ncmlistdownloader-1.0.0.240405a1/ncmlistdownloader/
--rw-rw-rw-   0        0        0     1303 2024-04-05 14:31:49.000000 ncmlistdownloader-1.0.0.240405a1/ncmlistdownloader/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-05 14:41:52.225354 ncmlistdownloader-1.0.0.240405a1/ncmlistdownloader/common/
--rw-rw-rw-   0        0        0     2859 2024-04-05 14:40:44.000000 ncmlistdownloader-1.0.0.240405a1/ncmlistdownloader/common/__init__.py
--rw-rw-rw-   0        0        0     2248 2024-04-05 14:06:36.000000 ncmlistdownloader-1.0.0.240405a1/ncmlistdownloader/common/encode_sec_key.py
--rw-rw-rw-   0        0        0     1785 2024-04-04 13:09:20.000000 ncmlistdownloader-1.0.0.240405a1/ncmlistdownloader/common/global_args.py
--rw-rw-rw-   0        0        0     1784 2024-04-04 13:40:40.000000 ncmlistdownloader-1.0.0.240405a1/ncmlistdownloader/common/thread_test.py
-drwxrwxrwx   0        0        0        0 2024-04-05 14:41:52.229348 ncmlistdownloader-1.0.0.240405a1/ncmlistdownloader/downloader/
--rw-rw-rw-   0        0        0     6526 2024-04-05 14:32:02.000000 ncmlistdownloader-1.0.0.240405a1/ncmlistdownloader/downloader/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-05 14:41:52.232350 ncmlistdownloader-1.0.0.240405a1/ncmlistdownloader/editer/
--rw-rw-rw-   0        0        0     3929 2024-04-04 14:16:10.000000 ncmlistdownloader-1.0.0.240405a1/ncmlistdownloader/editer/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-05 14:41:52.241352 ncmlistdownloader-1.0.0.240405a1/ncmlistdownloader/playlist/
--rw-rw-rw-   0        0        0     1660 2024-04-05 14:22:39.000000 ncmlistdownloader-1.0.0.240405a1/ncmlistdownloader/playlist/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-05 14:41:52.244346 ncmlistdownloader-1.0.0.240405a1/ncmlistdownloader/song/
--rw-rw-rw-   0        0        0     6018 2024-04-05 14:31:02.000000 ncmlistdownloader-1.0.0.240405a1/ncmlistdownloader/song/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-05 14:41:52.250349 ncmlistdownloader-1.0.0.240405a1/ncmlistdownloader.egg-info/
--rw-rw-rw-   0        0        0     1399 2024-04-05 14:41:52.000000 ncmlistdownloader-1.0.0.240405a1/ncmlistdownloader.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      618 2024-04-05 14:41:52.000000 ncmlistdownloader-1.0.0.240405a1/ncmlistdownloader.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-05 14:41:52.000000 ncmlistdownloader-1.0.0.240405a1/ncmlistdownloader.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       70 2024-04-05 14:41:52.000000 ncmlistdownloader-1.0.0.240405a1/ncmlistdownloader.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       37 2024-04-05 14:41:52.000000 ncmlistdownloader-1.0.0.240405a1/ncmlistdownloader.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-04-05 14:41:52.000000 ncmlistdownloader-1.0.0.240405a1/ncmlistdownloader.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-05 14:41:52.257348 ncmlistdownloader-1.0.0.240405a1/setup.cfg
--rw-rw-rw-   0        0        0     1700 2024-04-05 14:41:19.000000 ncmlistdownloader-1.0.0.240405a1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-07 14:49:27.439933 ncmlistdownloader-1.0.0.240407b1/
+-rw-rw-rw-   0        0        0    35181 2024-03-07 09:37:50.000000 ncmlistdownloader-1.0.0.240407b1/LICENSE
+-rw-rw-rw-   0        0        0     1398 2024-04-07 14:49:27.437933 ncmlistdownloader-1.0.0.240407b1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-07 14:49:27.396888 ncmlistdownloader-1.0.0.240407b1/ncmlistdownloader/
+-rw-rw-rw-   0        0        0     1531 2024-04-07 14:32:39.000000 ncmlistdownloader-1.0.0.240407b1/ncmlistdownloader/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-07 14:49:27.421545 ncmlistdownloader-1.0.0.240407b1/ncmlistdownloader/common/
+-rw-rw-rw-   0        0        0     2859 2024-04-06 14:26:30.000000 ncmlistdownloader-1.0.0.240407b1/ncmlistdownloader/common/__init__.py
+-rw-rw-rw-   0        0        0     2248 2024-04-06 14:26:30.000000 ncmlistdownloader-1.0.0.240407b1/ncmlistdownloader/common/encode_sec_key.py
+-rw-rw-rw-   0        0        0     1785 2024-04-02 10:13:15.000000 ncmlistdownloader-1.0.0.240407b1/ncmlistdownloader/common/global_args.py
+-rw-rw-rw-   0        0        0     1784 2024-04-06 14:26:30.000000 ncmlistdownloader-1.0.0.240407b1/ncmlistdownloader/common/thread_test.py
+drwxrwxrwx   0        0        0        0 2024-04-07 14:49:27.424890 ncmlistdownloader-1.0.0.240407b1/ncmlistdownloader/downloader/
+-rw-rw-rw-   0        0        0     6526 2024-04-06 14:26:30.000000 ncmlistdownloader-1.0.0.240407b1/ncmlistdownloader/downloader/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-07 14:49:27.427070 ncmlistdownloader-1.0.0.240407b1/ncmlistdownloader/editer/
+-rw-rw-rw-   0        0        0     3929 2024-04-06 14:26:30.000000 ncmlistdownloader-1.0.0.240407b1/ncmlistdownloader/editer/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-07 14:49:27.431026 ncmlistdownloader-1.0.0.240407b1/ncmlistdownloader/playlist/
+-rw-rw-rw-   0        0        0     1660 2024-04-06 14:26:30.000000 ncmlistdownloader-1.0.0.240407b1/ncmlistdownloader/playlist/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-07 14:49:27.433701 ncmlistdownloader-1.0.0.240407b1/ncmlistdownloader/song/
+-rw-rw-rw-   0        0        0     6091 2024-04-07 14:32:56.000000 ncmlistdownloader-1.0.0.240407b1/ncmlistdownloader/song/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-07 14:49:27.436349 ncmlistdownloader-1.0.0.240407b1/ncmlistdownloader.egg-info/
+-rw-rw-rw-   0        0        0     1398 2024-04-07 14:49:27.000000 ncmlistdownloader-1.0.0.240407b1/ncmlistdownloader.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      606 2024-04-07 14:49:27.000000 ncmlistdownloader-1.0.0.240407b1/ncmlistdownloader.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-07 14:49:27.000000 ncmlistdownloader-1.0.0.240407b1/ncmlistdownloader.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       70 2024-04-07 14:49:27.000000 ncmlistdownloader-1.0.0.240407b1/ncmlistdownloader.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       37 2024-04-07 14:49:27.000000 ncmlistdownloader-1.0.0.240407b1/ncmlistdownloader.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-04-07 14:49:27.000000 ncmlistdownloader-1.0.0.240407b1/ncmlistdownloader.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-07 14:49:27.439933 ncmlistdownloader-1.0.0.240407b1/setup.cfg
+-rw-rw-rw-   0        0        0     1700 2024-04-07 14:33:40.000000 ncmlistdownloader-1.0.0.240407b1/setup.py
```

### Comparing `ncmlistdownloader-1.0.0.240405a1/LICENSE` & `ncmlistdownloader-1.0.0.240407b1/LICENSE`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.0.0.240405a1/PKG-INFO` & `ncmlistdownloader-1.0.0.240407b1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: ncmlistdownloader
-Version: 1.0.0.240405a1
+Version: 1.0.0.240407b1
 Summary: 获取网易云音乐歌单数据，下载音乐，主动添加元信息。
 Home-page: https://gitee.com/Cooooldwind/163ListDownloader_NexT
 Author: CooooldWind_
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Customer Service
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Topic :: Communications :: File Sharing
 Classifier: Topic :: Internet
 Classifier: Topic :: Multimedia
 Classifier: Topic :: Multimedia :: Graphics
```

### Comparing `ncmlistdownloader-1.0.0.240405a1/ncmlistdownloader/__init__.py` & `ncmlistdownloader-1.0.0.240407b1/ncmlistdownloader/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 '''
 ncmlistdownloader/__init__.py
-Core.Ver.1.0.0.240404b4-2
+Core.Ver.1.0.0.240407b1
 Author: CooooldWind_
 '''
 from ncmlistdownloader.playlist import *
+from ncmlistdownloader.common import *
 
 def main():
     print("163ListDownloader CMD Ver.")
-    print("Core.Ver.1.0.0.240404b4 / Made by CooooldWind_")
+    print("Core.Ver.1.0.0.240407b1 / Made by CooooldWind_")
     print("Warning: It's an Beta Version. It may has a lot of bugs.")
     print("If you met them, click the links below:")
     print("Gitee: https://gitee.com/CooooldWind/163ListDownloader_NexT/issues")
     print("GitHub: https://github.com/CooooldWind/163ListDownloader_NexT/issues")
     id = str(input("ID: "))
     p = Playlist(id)
     p.get_info()
@@ -22,19 +23,21 @@
         d = '%USERPROFILE%/Downloads/ncmlistdownloader/'
     fnf = str(input("Filename format: "))
     if fnf == '':
         fnf = '$title$ - $artist$'
     if d[-1] != '/' and d[-1] != '\\':
         d += '/'
     d = d.replace('\\', '/')
+    auto_mkdir(d)
     for i in p.track:
         i.filename_format = d + fnf
-        j = i.song_download()
-        if j == -1:
+        music_filename = i.song_download()
+        if music_filename == -1:
             print(i.title + 'cannot download.')
             continue
-        i.cover_download()
-        i.lyric_get()
-        i.attribute_write()
-        i.cover_write()
-        i.lyric_write()
+        cover_filename = i.cover_download()
+        lyric_filename = i.lyric_get()
+        i.attribute_write(music_filename)
+        i.cover_write(music_filename, cover_filename)
+        i.lyric_write(music_filename, lyric_filename)
+        print(i.title + 'Succeed.')
     print('Succeed.')
```

### Comparing `ncmlistdownloader-1.0.0.240405a1/ncmlistdownloader/common/__init__.py` & `ncmlistdownloader-1.0.0.240407b1/ncmlistdownloader/common/__init__.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.0.0.240405a1/ncmlistdownloader/common/encode_sec_key.py` & `ncmlistdownloader-1.0.0.240407b1/ncmlistdownloader/common/encode_sec_key.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.0.0.240405a1/ncmlistdownloader/common/global_args.py` & `ncmlistdownloader-1.0.0.240407b1/ncmlistdownloader/common/global_args.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.0.0.240405a1/ncmlistdownloader/common/thread_test.py` & `ncmlistdownloader-1.0.0.240407b1/ncmlistdownloader/common/thread_test.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.0.0.240405a1/ncmlistdownloader/downloader/__init__.py` & `ncmlistdownloader-1.0.0.240407b1/ncmlistdownloader/downloader/__init__.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.0.0.240405a1/ncmlistdownloader/editer/__init__.py` & `ncmlistdownloader-1.0.0.240407b1/ncmlistdownloader/editer/__init__.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.0.0.240405a1/ncmlistdownloader/playlist/__init__.py` & `ncmlistdownloader-1.0.0.240407b1/ncmlistdownloader/playlist/__init__.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.0.0.240405a1/ncmlistdownloader/song/__init__.py` & `ncmlistdownloader-1.0.0.240407b1/ncmlistdownloader/song/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 '''
 ncmlistdownloader/Song/__init__.py
-Core.Ver.1.0.0.240404b4-2
+Core.Ver.1.0.0.240407b1
 Author: CooooldWind_
 '''
 
 from ncmlistdownloader.common import *
 from ncmlistdownloader.common.encode_sec_key import *
 from ncmlistdownloader.common.thread_test import best_thread
 from ncmlistdownloader.downloader import *
@@ -112,30 +112,33 @@
 
     def song_download(self):
         filename = self.get_formated_filename('mp3')
         file_origin = OriginFile(self.url_info['song_file'])
         if file_origin.total_size <= 0:
             return -1
         file_origin.single_thread_start(filename = filename)
+        return filename
 
     def cover_download(self):
         filename = self.get_formated_filename('jpg')
         file_origin = OriginFile(self.url_info['album_pic'])
         if file_origin.total_size == -1:
             return -1
         file_origin.auto_start(filename = filename)
+        return filename
 
     def lyric_get(self):
         self.lyric = NeteaseParams(
             url = LYRIC_API,
             encode_data = self.lyric_encode_data
         ).get_resource()['lrc']['lyric'].replace("\n", '\n')
         filename = self.get_formated_filename('lrc')
         with open(file = filename, mode = 'w+', encoding = 'UTF-8') as file:
             file.write(self.lyric)
+        return filename
 
     def attribute_write(self, filename = 'No filename'):
         '''
         往文件里面写入歌曲信息
         ----------
         参数: 
         1. `filename`: 文件名，字符串，仅mp3/flac格式
```

### Comparing `ncmlistdownloader-1.0.0.240405a1/ncmlistdownloader.egg-info/PKG-INFO` & `ncmlistdownloader-1.0.0.240407b1/ncmlistdownloader.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: ncmlistdownloader
-Version: 1.0.0.240405a1
+Version: 1.0.0.240407b1
 Summary: 获取网易云音乐歌单数据，下载音乐，主动添加元信息。
 Home-page: https://gitee.com/Cooooldwind/163ListDownloader_NexT
 Author: CooooldWind_
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Customer Service
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Topic :: Communications :: File Sharing
 Classifier: Topic :: Internet
 Classifier: Topic :: Multimedia
 Classifier: Topic :: Multimedia :: Graphics
```

### Comparing `ncmlistdownloader-1.0.0.240405a1/ncmlistdownloader.egg-info/SOURCES.txt` & `ncmlistdownloader-1.0.0.240407b1/ncmlistdownloader.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 LICENSE
-MANIFEST.in
 setup.py
 ncmlistdownloader/__init__.py
 ncmlistdownloader.egg-info/PKG-INFO
 ncmlistdownloader.egg-info/SOURCES.txt
 ncmlistdownloader.egg-info/dependency_links.txt
 ncmlistdownloader.egg-info/entry_points.txt
 ncmlistdownloader.egg-info/requires.txt
```

### Comparing `ncmlistdownloader-1.0.0.240405a1/setup.py` & `ncmlistdownloader-1.0.0.240407b1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 setup(
     classifiers = [
         # 发展时期
-        'Development Status :: 3 - Alpha',
-        # 'Development Status :: 4 - Beta',
+        # 'Development Status :: 3 - Alpha',
+        'Development Status :: 4 - Beta',
         # 开发的目标用户
         'Intended Audience :: Customer Service',
         'Intended Audience :: Developers',
         'Intended Audience :: End Users/Desktop',
         # 属于什么类型
         'Topic :: Communications :: File Sharing',
         'Topic :: Internet',
@@ -25,15 +25,15 @@
 		'Programming Language :: Python :: 3.8',
 		'Programming Language :: Python :: 3.9',
 		'Programming Language :: Python :: 3.10',
 		'Programming Language :: Python :: 3.11',
 		'Programming Language :: Python :: 3.12',
     ],
     name = 'ncmlistdownloader',
-    version = "1.0.0.240405a1",
+    version = "1.0.0.240407b1",
     description = '获取网易云音乐歌单数据，下载音乐，主动添加元信息。',
     author = 'CooooldWind_',
     url = 'https://gitee.com/Cooooldwind/163ListDownloader_NexT',
     packages = find_packages(),
     install_requires = ['pycryptodome','pillow','mutagen','requests',],
     entry_points = {'console_scripts': ['ncmlistdownloader = ncmlistdownloader.__init__:main']},
 )
```

