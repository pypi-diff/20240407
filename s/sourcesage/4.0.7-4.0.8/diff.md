# Comparing `tmp/sourcesage-4.0.7.tar.gz` & `tmp/sourcesage-4.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sourcesage-4.0.7.tar", last modified: Sun Apr  7 13:51:27 2024, max compression
+gzip compressed data, was "sourcesage-4.0.8.tar", last modified: Sun Apr  7 13:51:57 2024, max compression
```

## Comparing `sourcesage-4.0.7.tar` & `sourcesage-4.0.8.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2024-04-07 13:51:27.633538 sourcesage-4.0.7/
--rw-rw-rw-   0        0        0     1082 2024-04-04 07:13:56.000000 sourcesage-4.0.7/LICENSE
--rw-rw-rw-   0        0        0    12824 2024-04-07 13:51:27.631551 sourcesage-4.0.7/PKG-INFO
--rw-rw-rw-   0        0        0    12547 2024-04-04 16:38:14.000000 sourcesage-4.0.7/README.md
--rw-rw-rw-   0        0        0       42 2024-04-07 13:51:27.633538 sourcesage-4.0.7/setup.cfg
--rw-rw-rw-   0        0        0      715 2024-04-07 13:49:56.000000 sourcesage-4.0.7/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-07 13:51:27.546308 sourcesage-4.0.7/sourcesage/
--rw-rw-rw-   0        0        0        0 2024-04-04 15:59:17.000000 sourcesage-4.0.7/sourcesage/__init__.py
--rw-rw-rw-   0        0        0     1441 2024-04-07 13:35:31.000000 sourcesage-4.0.7/sourcesage/cli.py
-drwxrwxrwx   0        0        0        0 2024-04-07 13:51:27.586855 sourcesage-4.0.7/sourcesage/config/
--rw-rw-rw-   0        0        0     1751 2024-04-04 15:59:17.000000 sourcesage-4.0.7/sourcesage/config/constants.py
--rw-rw-rw-   0        0        0      590 2024-04-04 15:59:17.000000 sourcesage-4.0.7/sourcesage/config/language_map.json
--rw-rw-rw-   0        0        0     4947 2024-04-07 13:48:15.000000 sourcesage-4.0.7/sourcesage/core.py
-drwxrwxrwx   0        0        0        0 2024-04-07 13:51:27.626119 sourcesage-4.0.7/sourcesage/modules/
--rw-rw-rw-   0        0        0     3885 2024-04-04 15:59:17.000000 sourcesage-4.0.7/sourcesage/modules/ChangelogGenerator.py
--rw-rw-rw-   0        0        0     1440 2024-04-04 15:59:17.000000 sourcesage-4.0.7/sourcesage/modules/ChangelogUtils.py
--rw-rw-rw-   0        0        0     4171 2024-04-04 15:59:17.000000 sourcesage-4.0.7/sourcesage/modules/DiffChangelogGenerator.py
--rw-rw-rw-   0        0        0     1073 2024-04-04 15:59:17.000000 sourcesage-4.0.7/sourcesage/modules/EnvFileHandler.py
--rw-rw-rw-   0        0        0      836 2024-04-04 15:59:17.000000 sourcesage-4.0.7/sourcesage/modules/GitHubIssueRetrieve.py
--rw-rw-rw-   0        0        0     1291 2024-04-04 15:59:17.000000 sourcesage-4.0.7/sourcesage/modules/GitHubUtils.py
--rw-rw-rw-   0        0        0     2227 2024-04-04 15:59:17.000000 sourcesage-4.0.7/sourcesage/modules/IssuesToMarkdown.py
--rw-rw-rw-   0        0        0     3036 2024-04-04 15:59:17.000000 sourcesage-4.0.7/sourcesage/modules/StageInfoGenerator.py
--rw-rw-rw-   0        0        0     2778 2024-04-04 15:59:17.000000 sourcesage-4.0.7/sourcesage/modules/StagedDiffGenerator.py
--rw-rw-rw-   0        0        0        0 2024-04-04 15:59:17.000000 sourcesage-4.0.7/sourcesage/modules/__init__.py
--rw-rw-rw-   0        0        0      930 2024-04-04 15:59:17.000000 sourcesage-4.0.7/sourcesage/modules/file_utils.py
--rw-rw-rw-   0        0        0     3261 2024-04-04 15:59:17.000000 sourcesage-4.0.7/sourcesage/modules/markdown_utils.py
--rw-rw-rw-   0        0        0     1115 2024-04-04 15:59:17.000000 sourcesage-4.0.7/sourcesage/modules/source_sage.py
-drwxrwxrwx   0        0        0        0 2024-04-07 13:51:27.581492 sourcesage-4.0.7/sourcesage.egg-info/
--rw-rw-rw-   0        0        0    12824 2024-04-07 13:51:27.000000 sourcesage-4.0.7/sourcesage.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      877 2024-04-07 13:51:27.000000 sourcesage-4.0.7/sourcesage.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-07 13:51:27.000000 sourcesage-4.0.7/sourcesage.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2024-04-07 13:51:27.000000 sourcesage-4.0.7/sourcesage.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       30 2024-04-07 13:51:27.000000 sourcesage-4.0.7/sourcesage.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-07 13:51:27.000000 sourcesage-4.0.7/sourcesage.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-07 13:51:27.627111 sourcesage-4.0.7/tests/
--rw-rw-rw-   0        0        0     3207 2024-04-07 13:35:05.000000 sourcesage-4.0.7/tests/test_sourcesage.py
+drwxrwxrwx   0        0        0        0 2024-04-07 13:51:57.311168 sourcesage-4.0.8/
+-rw-rw-rw-   0        0        0     1082 2024-04-04 07:13:56.000000 sourcesage-4.0.8/LICENSE
+-rw-rw-rw-   0        0        0    12824 2024-04-07 13:51:57.309152 sourcesage-4.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0    12547 2024-04-04 16:38:14.000000 sourcesage-4.0.8/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-07 13:51:57.311834 sourcesage-4.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      715 2024-04-07 13:51:50.000000 sourcesage-4.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-07 13:51:57.240159 sourcesage-4.0.8/sourcesage/
+-rw-rw-rw-   0        0        0        0 2024-04-04 15:59:17.000000 sourcesage-4.0.8/sourcesage/__init__.py
+-rw-rw-rw-   0        0        0     1441 2024-04-07 13:35:31.000000 sourcesage-4.0.8/sourcesage/cli.py
+drwxrwxrwx   0        0        0        0 2024-04-07 13:51:57.275825 sourcesage-4.0.8/sourcesage/config/
+-rw-rw-rw-   0        0        0     1751 2024-04-04 15:59:17.000000 sourcesage-4.0.8/sourcesage/config/constants.py
+-rw-rw-rw-   0        0        0      590 2024-04-04 15:59:17.000000 sourcesage-4.0.8/sourcesage/config/language_map.json
+-rw-rw-rw-   0        0        0     4932 2024-04-07 13:51:46.000000 sourcesage-4.0.8/sourcesage/core.py
+drwxrwxrwx   0        0        0        0 2024-04-07 13:51:57.304325 sourcesage-4.0.8/sourcesage/modules/
+-rw-rw-rw-   0        0        0     3885 2024-04-04 15:59:17.000000 sourcesage-4.0.8/sourcesage/modules/ChangelogGenerator.py
+-rw-rw-rw-   0        0        0     1440 2024-04-04 15:59:17.000000 sourcesage-4.0.8/sourcesage/modules/ChangelogUtils.py
+-rw-rw-rw-   0        0        0     4171 2024-04-04 15:59:17.000000 sourcesage-4.0.8/sourcesage/modules/DiffChangelogGenerator.py
+-rw-rw-rw-   0        0        0     1073 2024-04-04 15:59:17.000000 sourcesage-4.0.8/sourcesage/modules/EnvFileHandler.py
+-rw-rw-rw-   0        0        0      836 2024-04-04 15:59:17.000000 sourcesage-4.0.8/sourcesage/modules/GitHubIssueRetrieve.py
+-rw-rw-rw-   0        0        0     1291 2024-04-04 15:59:17.000000 sourcesage-4.0.8/sourcesage/modules/GitHubUtils.py
+-rw-rw-rw-   0        0        0     2227 2024-04-04 15:59:17.000000 sourcesage-4.0.8/sourcesage/modules/IssuesToMarkdown.py
+-rw-rw-rw-   0        0        0     3036 2024-04-04 15:59:17.000000 sourcesage-4.0.8/sourcesage/modules/StageInfoGenerator.py
+-rw-rw-rw-   0        0        0     2778 2024-04-04 15:59:17.000000 sourcesage-4.0.8/sourcesage/modules/StagedDiffGenerator.py
+-rw-rw-rw-   0        0        0        0 2024-04-04 15:59:17.000000 sourcesage-4.0.8/sourcesage/modules/__init__.py
+-rw-rw-rw-   0        0        0      930 2024-04-04 15:59:17.000000 sourcesage-4.0.8/sourcesage/modules/file_utils.py
+-rw-rw-rw-   0        0        0     3261 2024-04-04 15:59:17.000000 sourcesage-4.0.8/sourcesage/modules/markdown_utils.py
+-rw-rw-rw-   0        0        0     1115 2024-04-04 15:59:17.000000 sourcesage-4.0.8/sourcesage/modules/source_sage.py
+drwxrwxrwx   0        0        0        0 2024-04-07 13:51:57.272288 sourcesage-4.0.8/sourcesage.egg-info/
+-rw-rw-rw-   0        0        0    12824 2024-04-07 13:51:56.000000 sourcesage-4.0.8/sourcesage.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      877 2024-04-07 13:51:57.000000 sourcesage-4.0.8/sourcesage.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-07 13:51:57.000000 sourcesage-4.0.8/sourcesage.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2024-04-07 13:51:57.000000 sourcesage-4.0.8/sourcesage.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       30 2024-04-07 13:51:57.000000 sourcesage-4.0.8/sourcesage.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-07 13:51:57.000000 sourcesage-4.0.8/sourcesage.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-07 13:51:57.304325 sourcesage-4.0.8/tests/
+-rw-rw-rw-   0        0        0     3207 2024-04-07 13:35:05.000000 sourcesage-4.0.8/tests/test_sourcesage.py
```

### Comparing `sourcesage-4.0.7/LICENSE` & `sourcesage-4.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `sourcesage-4.0.7/PKG-INFO` & `sourcesage-4.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sourcesage
-Version: 4.0.7
+Version: 4.0.8
 Home-page: https://github.com/Sunwood-ai-labs/SourceSage
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: loguru
 Requires-Dist: GitPython
 Requires-Dist: requests
 Requires-Dist: art
```

### Comparing `sourcesage-4.0.7/README.md` & `sourcesage-4.0.8/README.md`

 * *Files identical despite different names*

### Comparing `sourcesage-4.0.7/setup.py` & `sourcesage-4.0.8/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 # READMEファイルの内容を読み込む
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='sourcesage',
-    version='4.0.7',
+    version='4.0.8',
     packages=find_packages(),
     package_data={
         'sourcesage': ['config/*', ],
     },
     entry_points={
         'console_scripts': [
             'sourcesage=sourcesage.cli:main',
```

### Comparing `sourcesage-4.0.7/sourcesage/cli.py` & `sourcesage-4.0.8/sourcesage/cli.py`

 * *Files identical despite different names*

### Comparing `sourcesage-4.0.7/sourcesage/config/constants.py` & `sourcesage-4.0.8/sourcesage/config/constants.py`

 * *Files identical despite different names*

### Comparing `sourcesage-4.0.7/sourcesage/config/language_map.json` & `sourcesage-4.0.8/sourcesage/config/language_map.json`

 * *Files identical despite different names*

### Comparing `sourcesage-4.0.7/sourcesage/core.py` & `sourcesage-4.0.8/sourcesage/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,14 @@
         self.ignore_file = ignore_file
         self.language_map_file = language_map_file
 
         self.constants = Constants(output_dir, owner, repository) 
 
     def run(self):
         tprint("SourceSage", font="rnd-medium")
-        raise
         print("Running SourceSage...")
         
         # Load configuration
         config = self.load_config()
 
         # Create necessary directories
         os.makedirs(self.constants.ISSUE_LOG_DIR, exist_ok=True)
```

### Comparing `sourcesage-4.0.7/sourcesage/modules/ChangelogGenerator.py` & `sourcesage-4.0.8/sourcesage/modules/ChangelogGenerator.py`

 * *Files identical despite different names*

### Comparing `sourcesage-4.0.7/sourcesage/modules/ChangelogUtils.py` & `sourcesage-4.0.8/sourcesage/modules/ChangelogUtils.py`

 * *Files identical despite different names*

### Comparing `sourcesage-4.0.7/sourcesage/modules/DiffChangelogGenerator.py` & `sourcesage-4.0.8/sourcesage/modules/DiffChangelogGenerator.py`

 * *Files identical despite different names*

### Comparing `sourcesage-4.0.7/sourcesage/modules/EnvFileHandler.py` & `sourcesage-4.0.8/sourcesage/modules/EnvFileHandler.py`

 * *Files identical despite different names*

### Comparing `sourcesage-4.0.7/sourcesage/modules/GitHubIssueRetrieve.py` & `sourcesage-4.0.8/sourcesage/modules/GitHubIssueRetrieve.py`

 * *Files identical despite different names*

### Comparing `sourcesage-4.0.7/sourcesage/modules/GitHubUtils.py` & `sourcesage-4.0.8/sourcesage/modules/GitHubUtils.py`

 * *Files identical despite different names*

### Comparing `sourcesage-4.0.7/sourcesage/modules/IssuesToMarkdown.py` & `sourcesage-4.0.8/sourcesage/modules/IssuesToMarkdown.py`

 * *Files identical despite different names*

### Comparing `sourcesage-4.0.7/sourcesage/modules/StageInfoGenerator.py` & `sourcesage-4.0.8/sourcesage/modules/StageInfoGenerator.py`

 * *Files identical despite different names*

### Comparing `sourcesage-4.0.7/sourcesage/modules/StagedDiffGenerator.py` & `sourcesage-4.0.8/sourcesage/modules/StagedDiffGenerator.py`

 * *Files identical despite different names*

### Comparing `sourcesage-4.0.7/sourcesage/modules/file_utils.py` & `sourcesage-4.0.8/sourcesage/modules/file_utils.py`

 * *Files identical despite different names*

### Comparing `sourcesage-4.0.7/sourcesage/modules/markdown_utils.py` & `sourcesage-4.0.8/sourcesage/modules/markdown_utils.py`

 * *Files identical despite different names*

### Comparing `sourcesage-4.0.7/sourcesage/modules/source_sage.py` & `sourcesage-4.0.8/sourcesage/modules/source_sage.py`

 * *Files identical despite different names*

### Comparing `sourcesage-4.0.7/sourcesage.egg-info/PKG-INFO` & `sourcesage-4.0.8/sourcesage.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sourcesage
-Version: 4.0.7
+Version: 4.0.8
 Home-page: https://github.com/Sunwood-ai-labs/SourceSage
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: loguru
 Requires-Dist: GitPython
 Requires-Dist: requests
 Requires-Dist: art
```

### Comparing `sourcesage-4.0.7/sourcesage.egg-info/SOURCES.txt` & `sourcesage-4.0.8/sourcesage.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sourcesage-4.0.7/tests/test_sourcesage.py` & `sourcesage-4.0.8/tests/test_sourcesage.py`

 * *Files identical despite different names*

