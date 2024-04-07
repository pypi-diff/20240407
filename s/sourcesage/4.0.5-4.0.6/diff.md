# Comparing `tmp/sourcesage-4.0.5.tar.gz` & `tmp/sourcesage-4.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sourcesage-4.0.5.tar", last modified: Thu Apr  4 16:33:31 2024, max compression
+gzip compressed data, was "sourcesage-4.0.6.tar", last modified: Sun Apr  7 13:48:50 2024, max compression
```

## Comparing `sourcesage-4.0.5.tar` & `sourcesage-4.0.6.tar`

### file list

```diff
@@ -1,33 +1,36 @@
-drwxrwxrwx   0        0        0        0 2024-04-04 16:33:31.591335 sourcesage-4.0.5/
--rw-rw-rw-   0        0        0     1082 2024-04-04 07:13:56.000000 sourcesage-4.0.5/LICENSE
--rw-rw-rw-   0        0        0    12545 2024-04-04 16:33:31.589137 sourcesage-4.0.5/PKG-INFO
--rw-rw-rw-   0        0        0    12288 2024-04-04 16:31:30.000000 sourcesage-4.0.5/README.md
--rw-rw-rw-   0        0        0       42 2024-04-04 16:33:31.591917 sourcesage-4.0.5/setup.cfg
--rw-rw-rw-   0        0        0      632 2024-04-04 16:33:29.000000 sourcesage-4.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-04 16:33:31.512345 sourcesage-4.0.5/sourcesage/
--rw-rw-rw-   0        0        0        0 2024-04-04 15:59:17.000000 sourcesage-4.0.5/sourcesage/__init__.py
--rw-rw-rw-   0        0        0      856 2024-04-04 15:59:17.000000 sourcesage-4.0.5/sourcesage/cli.py
--rw-rw-rw-   0        0        0     4768 2024-04-04 15:59:17.000000 sourcesage-4.0.5/sourcesage/core.py
-drwxrwxrwx   0        0        0        0 2024-04-04 16:33:31.583678 sourcesage-4.0.5/sourcesage/modules/
--rw-rw-rw-   0        0        0     3885 2024-04-04 15:59:17.000000 sourcesage-4.0.5/sourcesage/modules/ChangelogGenerator.py
--rw-rw-rw-   0        0        0     1440 2024-04-04 15:59:17.000000 sourcesage-4.0.5/sourcesage/modules/ChangelogUtils.py
--rw-rw-rw-   0        0        0     4171 2024-04-04 15:59:17.000000 sourcesage-4.0.5/sourcesage/modules/DiffChangelogGenerator.py
--rw-rw-rw-   0        0        0     1073 2024-04-04 15:59:17.000000 sourcesage-4.0.5/sourcesage/modules/EnvFileHandler.py
--rw-rw-rw-   0        0        0      836 2024-04-04 15:59:17.000000 sourcesage-4.0.5/sourcesage/modules/GitHubIssueRetrieve.py
--rw-rw-rw-   0        0        0     1291 2024-04-04 15:59:17.000000 sourcesage-4.0.5/sourcesage/modules/GitHubUtils.py
--rw-rw-rw-   0        0        0     2227 2024-04-04 15:59:17.000000 sourcesage-4.0.5/sourcesage/modules/IssuesToMarkdown.py
--rw-rw-rw-   0        0        0     3036 2024-04-04 15:59:17.000000 sourcesage-4.0.5/sourcesage/modules/StageInfoGenerator.py
--rw-rw-rw-   0        0        0     2778 2024-04-04 15:59:17.000000 sourcesage-4.0.5/sourcesage/modules/StagedDiffGenerator.py
--rw-rw-rw-   0        0        0        0 2024-04-04 15:59:17.000000 sourcesage-4.0.5/sourcesage/modules/__init__.py
--rw-rw-rw-   0        0        0      930 2024-04-04 15:59:17.000000 sourcesage-4.0.5/sourcesage/modules/file_utils.py
--rw-rw-rw-   0        0        0     3261 2024-04-04 15:59:17.000000 sourcesage-4.0.5/sourcesage/modules/markdown_utils.py
--rw-rw-rw-   0        0        0     1115 2024-04-04 15:59:17.000000 sourcesage-4.0.5/sourcesage/modules/source_sage.py
-drwxrwxrwx   0        0        0        0 2024-04-04 16:33:31.545330 sourcesage-4.0.5/sourcesage.egg-info/
--rw-rw-rw-   0        0        0    12545 2024-04-04 16:33:31.000000 sourcesage-4.0.5/sourcesage.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      810 2024-04-04 16:33:31.000000 sourcesage-4.0.5/sourcesage.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-04 16:33:31.000000 sourcesage-4.0.5/sourcesage.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2024-04-04 16:33:31.000000 sourcesage-4.0.5/sourcesage.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       26 2024-04-04 16:33:31.000000 sourcesage-4.0.5/sourcesage.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-04 16:33:31.000000 sourcesage-4.0.5/sourcesage.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-04 16:33:31.586131 sourcesage-4.0.5/tests/
--rw-rw-rw-   0        0        0     2577 2024-04-04 15:59:17.000000 sourcesage-4.0.5/tests/test_sourcesage.py
+drwxrwxrwx   0        0        0        0 2024-04-07 13:48:50.010718 sourcesage-4.0.6/
+-rw-rw-rw-   0        0        0     1082 2024-04-04 07:13:56.000000 sourcesage-4.0.6/LICENSE
+-rw-rw-rw-   0        0        0    12824 2024-04-07 13:48:50.010718 sourcesage-4.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0    12547 2024-04-04 16:38:14.000000 sourcesage-4.0.6/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-07 13:48:50.010718 sourcesage-4.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      715 2024-04-07 13:48:36.000000 sourcesage-4.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-07 13:48:49.921866 sourcesage-4.0.6/sourcesage/
+-rw-rw-rw-   0        0        0        0 2024-04-04 15:59:17.000000 sourcesage-4.0.6/sourcesage/__init__.py
+-rw-rw-rw-   0        0        0     1441 2024-04-07 13:35:31.000000 sourcesage-4.0.6/sourcesage/cli.py
+drwxrwxrwx   0        0        0        0 2024-04-07 13:48:49.958526 sourcesage-4.0.6/sourcesage/config/
+-rw-rw-rw-   0        0        0     1751 2024-04-04 15:59:17.000000 sourcesage-4.0.6/sourcesage/config/constants.py
+-rw-rw-rw-   0        0        0      590 2024-04-04 15:59:17.000000 sourcesage-4.0.6/sourcesage/config/language_map.json
+-rw-rw-rw-   0        0        0     4947 2024-04-07 13:48:15.000000 sourcesage-4.0.6/sourcesage/core.py
+drwxrwxrwx   0        0        0        0 2024-04-07 13:48:50.006792 sourcesage-4.0.6/sourcesage/modules/
+-rw-rw-rw-   0        0        0     3885 2024-04-04 15:59:17.000000 sourcesage-4.0.6/sourcesage/modules/ChangelogGenerator.py
+-rw-rw-rw-   0        0        0     1440 2024-04-04 15:59:17.000000 sourcesage-4.0.6/sourcesage/modules/ChangelogUtils.py
+-rw-rw-rw-   0        0        0     4171 2024-04-04 15:59:17.000000 sourcesage-4.0.6/sourcesage/modules/DiffChangelogGenerator.py
+-rw-rw-rw-   0        0        0     1073 2024-04-04 15:59:17.000000 sourcesage-4.0.6/sourcesage/modules/EnvFileHandler.py
+-rw-rw-rw-   0        0        0      836 2024-04-04 15:59:17.000000 sourcesage-4.0.6/sourcesage/modules/GitHubIssueRetrieve.py
+-rw-rw-rw-   0        0        0     1291 2024-04-04 15:59:17.000000 sourcesage-4.0.6/sourcesage/modules/GitHubUtils.py
+-rw-rw-rw-   0        0        0     2227 2024-04-04 15:59:17.000000 sourcesage-4.0.6/sourcesage/modules/IssuesToMarkdown.py
+-rw-rw-rw-   0        0        0     3036 2024-04-04 15:59:17.000000 sourcesage-4.0.6/sourcesage/modules/StageInfoGenerator.py
+-rw-rw-rw-   0        0        0     2778 2024-04-04 15:59:17.000000 sourcesage-4.0.6/sourcesage/modules/StagedDiffGenerator.py
+-rw-rw-rw-   0        0        0        0 2024-04-04 15:59:17.000000 sourcesage-4.0.6/sourcesage/modules/__init__.py
+-rw-rw-rw-   0        0        0      930 2024-04-04 15:59:17.000000 sourcesage-4.0.6/sourcesage/modules/file_utils.py
+-rw-rw-rw-   0        0        0     3261 2024-04-04 15:59:17.000000 sourcesage-4.0.6/sourcesage/modules/markdown_utils.py
+-rw-rw-rw-   0        0        0     1115 2024-04-04 15:59:17.000000 sourcesage-4.0.6/sourcesage/modules/source_sage.py
+drwxrwxrwx   0        0        0        0 2024-04-07 13:48:49.954448 sourcesage-4.0.6/sourcesage.egg-info/
+-rw-rw-rw-   0        0        0    12824 2024-04-07 13:48:49.000000 sourcesage-4.0.6/sourcesage.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      877 2024-04-07 13:48:49.000000 sourcesage-4.0.6/sourcesage.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-07 13:48:49.000000 sourcesage-4.0.6/sourcesage.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2024-04-07 13:48:49.000000 sourcesage-4.0.6/sourcesage.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       30 2024-04-07 13:48:49.000000 sourcesage-4.0.6/sourcesage.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-07 13:48:49.000000 sourcesage-4.0.6/sourcesage.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-07 13:48:50.009788 sourcesage-4.0.6/tests/
+-rw-rw-rw-   0        0        0     3207 2024-04-07 13:35:05.000000 sourcesage-4.0.6/tests/test_sourcesage.py
```

### Comparing `sourcesage-4.0.5/LICENSE` & `sourcesage-4.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `sourcesage-4.0.5/PKG-INFO` & `sourcesage-4.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,32 @@
 Metadata-Version: 2.1
 Name: sourcesage
-Version: 4.0.5
+Version: 4.0.6
 Home-page: https://github.com/Sunwood-ai-labs/SourceSage
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: loguru
 Requires-Dist: GitPython
 Requires-Dist: requests
+Requires-Dist: art
 
 <p align="center">
 <img src="https://raw.githubusercontent.com/Sunwood-ai-labs/SourceSage/main/docs/icon/SourceSage_icon4.png" width="100%">
 <br>
 <h1 align="center">SourceSage</h1>
 <h2 align="center">
   ～Transforming code for AI～
 
   <br>
   <img alt="PyPI - Version" src="https://img.shields.io/pypi/v/sourcesage">
-  
+  <img alt="PyPI - Format" src="https://img.shields.io/pypi/format/sourcesage">
+  <img alt="PyPI - Implementation" src="https://img.shields.io/pypi/implementation/sourcesage">
+  <img alt="PyPI - Status" src="https://img.shields.io/pypi/status/sourcesage">
+
+
   <br>
 
 </h2>
 
 
 </p>
```

### Comparing `sourcesage-4.0.5/README.md` & `sourcesage-4.0.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,19 @@
 <br>
 <h1 align="center">SourceSage</h1>
 <h2 align="center">
   ～Transforming code for AI～
 
   <br>
   <img alt="PyPI - Version" src="https://img.shields.io/pypi/v/sourcesage">
-  
+  <img alt="PyPI - Format" src="https://img.shields.io/pypi/format/sourcesage">
+  <img alt="PyPI - Implementation" src="https://img.shields.io/pypi/implementation/sourcesage">
+  <img alt="PyPI - Status" src="https://img.shields.io/pypi/status/sourcesage">
+
+
   <br>
 
 </h2>
 
 
 </p>
```

### Comparing `sourcesage-4.0.5/setup.py` & `sourcesage-4.0.6/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,23 +3,27 @@
 
 # READMEファイルの内容を読み込む
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='sourcesage',
-    version='4.0.5',
+    version='4.0.6',
     packages=find_packages(),
+    package_data={
+        'sourcesage': ['config/*', ],
+    },
     entry_points={
         'console_scripts': [
             'sourcesage=sourcesage.cli:main',
         ],
     },
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Sunwood-ai-labs/SourceSage",
     install_requires=[
         'loguru',
         'GitPython',
         'requests',
+        'art',
     ],
 )
```

### Comparing `sourcesage-4.0.5/sourcesage/cli.py` & `sourcesage-4.0.6/sourcesage/cli.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,18 +1,26 @@
 import argparse
 from .core import SourceSage
+import os
 
 def main():
     parser = argparse.ArgumentParser(description='SourceSage CLI')
     parser.add_argument('--config', help='Path to the configuration file', default='sourcesage.yml')
     parser.add_argument('--output', help='Output directory for generated files', default='./')
     parser.add_argument('--repo', help='Path to the repository', default='./')
     parser.add_argument('--owner', help='Owner of the repository', default='Sunwood-ai-labs')  # デフォルト値を設定
     parser.add_argument('--repository', help='Name of the repository', default='SourceSage')  # デフォルト値を設定
+
+    package_root = os.path.dirname(os.path.dirname(os.path.abspath(__file__)))
+    default_ignore_file = os.path.join(package_root, 'sourcesage', 'config', '.SourceSageignore')  # 修正
+    default_language_map = os.path.join(package_root, 'sourcesage', 'config', 'language_map.json')  # 修正
+
+    parser.add_argument('--ignore-file', help='Path to the ignore file', default=default_ignore_file)  # 修正
+    parser.add_argument('--language-map', help='Path to the language map file', default=default_language_map)  # 修正
     
     args = parser.parse_args()
 
-    sourcesage = SourceSage(args.config, args.output, args.repo, args.owner, args.repository)
+    sourcesage = SourceSage(args.config, args.output, args.repo, args.owner, args.repository, args.ignore_file, args.language_map)
     sourcesage.run()
 
 if __name__ == '__main__':
     main()
```

### Comparing `sourcesage-4.0.5/sourcesage/core.py` & `sourcesage-4.0.6/sourcesage/core.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,51 +5,57 @@
 from .modules.StageInfoGenerator import StageInfoGenerator
 from .modules.GitHubIssueRetrieve import GitHubIssueRetriever
 from .modules.StagedDiffGenerator import StagedDiffGenerator
 from .modules.IssuesToMarkdown import IssuesToMarkdown
 
 from .config.constants import Constants
 
+from art import *
+
 class SourceSage:
-    def __init__(self, config_path, output_dir, repo_path, owner, repository):
+    def __init__(self, config_path, output_dir, repo_path, owner, repository, ignore_file, language_map_file):
         self.config_path = config_path
         self.output_dir = output_dir
         self.repo_path = repo_path
+        self.ignore_file = ignore_file
+        self.language_map_file = language_map_file
 
         self.constants = Constants(output_dir, owner, repository) 
 
     def run(self):
+        tprint("SourceSage", font="rnd-medium")
+        raise
         print("Running SourceSage...")
         
         # Load configuration
         config = self.load_config()
 
         # Create necessary directories
         os.makedirs(self.constants.ISSUE_LOG_DIR, exist_ok=True)
         os.makedirs(self.constants.ISSUES_RESOLVE_DIR, exist_ok=True)
         os.makedirs(self.constants.STAGE_INFO_DIR, exist_ok=True)
         
         # Generate SourceSage markdown
-        sourcesage_module = SourceSageModule(folders=[self.repo_path], ignore_file=self.constants.IGNORE_FILE,
+        sourcesage_module = SourceSageModule(folders=[self.repo_path], ignore_file=self.ignore_file,
                                              output_file=os.path.join(self.constants.SOURCE_SAGE_ASSETS_DIR, self.constants.SOURCE_SAGE_MD),
-                                             language_map_file=self.constants.LANGUAGE_MAP_FILE)
+                                             language_map_file=self.language_map_file)
         sourcesage_module.generate_markdown()
 
         # Generate changelog
         changelog_generator = ChangelogGenerator(self.repo_path, os.path.join(self.constants.SOURCE_SAGE_ASSETS_DIR, self.constants.CHANGELOG_DIR))
         changelog_generator.generate_changelog_for_all_branches()
         changelog_generator.integrate_changelogs()
 
         # Retrieve GitHub issues
         issue_retriever = GitHubIssueRetriever(self.constants.OWNER, self.constants.REPOSITORY, self.constants.ISSUE_LOG_DIR, self.constants.ISSUES_FILE_NAME)
         issue_retriever.run()
 
         # Generate staged diff
         diff_generator = StagedDiffGenerator(repo_path=self.repo_path, output_dir=self.constants.SOURCE_SAGE_ASSETS_DIR,
-                                             language_map_file=self.constants.LANGUAGE_MAP_FILE)
+                                             language_map_file=self.language_map_file)
         diff_generator.run()
 
         # Generate stage info and issues
         stage_info_generator = StageInfoGenerator(issue_file_path=os.path.join(self.constants.ISSUE_LOG_DIR, self.constants.ISSUES_FILE_NAME),
                                                   stage_diff_file_path=os.path.join(self.constants.SOURCE_SAGE_ASSETS_DIR, self.constants.STAGED_DIFF_MD),
                                                   template_file_path=os.path.join(self.constants.DOCS_DIR, self.constants.TEMPLATE_STAGE_INFO_DIR, self.constants.STAGE_INFO_TEMPLATE_MD),
                                                   output_file_path=os.path.join(self.constants.STAGE_INFO_DIR, self.constants.STAGE_INFO_OUTPUT_MD))
```

### Comparing `sourcesage-4.0.5/sourcesage/modules/ChangelogGenerator.py` & `sourcesage-4.0.6/sourcesage/modules/ChangelogGenerator.py`

 * *Files identical despite different names*

### Comparing `sourcesage-4.0.5/sourcesage/modules/ChangelogUtils.py` & `sourcesage-4.0.6/sourcesage/modules/ChangelogUtils.py`

 * *Files identical despite different names*

### Comparing `sourcesage-4.0.5/sourcesage/modules/DiffChangelogGenerator.py` & `sourcesage-4.0.6/sourcesage/modules/DiffChangelogGenerator.py`

 * *Files identical despite different names*

### Comparing `sourcesage-4.0.5/sourcesage/modules/EnvFileHandler.py` & `sourcesage-4.0.6/sourcesage/modules/EnvFileHandler.py`

 * *Files identical despite different names*

### Comparing `sourcesage-4.0.5/sourcesage/modules/GitHubIssueRetrieve.py` & `sourcesage-4.0.6/sourcesage/modules/GitHubIssueRetrieve.py`

 * *Files identical despite different names*

### Comparing `sourcesage-4.0.5/sourcesage/modules/GitHubUtils.py` & `sourcesage-4.0.6/sourcesage/modules/GitHubUtils.py`

 * *Files identical despite different names*

### Comparing `sourcesage-4.0.5/sourcesage/modules/IssuesToMarkdown.py` & `sourcesage-4.0.6/sourcesage/modules/IssuesToMarkdown.py`

 * *Files identical despite different names*

### Comparing `sourcesage-4.0.5/sourcesage/modules/StageInfoGenerator.py` & `sourcesage-4.0.6/sourcesage/modules/StageInfoGenerator.py`

 * *Files identical despite different names*

### Comparing `sourcesage-4.0.5/sourcesage/modules/StagedDiffGenerator.py` & `sourcesage-4.0.6/sourcesage/modules/StagedDiffGenerator.py`

 * *Files identical despite different names*

### Comparing `sourcesage-4.0.5/sourcesage/modules/file_utils.py` & `sourcesage-4.0.6/sourcesage/modules/file_utils.py`

 * *Files identical despite different names*

### Comparing `sourcesage-4.0.5/sourcesage/modules/markdown_utils.py` & `sourcesage-4.0.6/sourcesage/modules/markdown_utils.py`

 * *Files identical despite different names*

### Comparing `sourcesage-4.0.5/sourcesage/modules/source_sage.py` & `sourcesage-4.0.6/sourcesage/modules/source_sage.py`

 * *Files identical despite different names*

### Comparing `sourcesage-4.0.5/sourcesage.egg-info/PKG-INFO` & `sourcesage-4.0.6/sourcesage.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,32 @@
 Metadata-Version: 2.1
 Name: sourcesage
-Version: 4.0.5
+Version: 4.0.6
 Home-page: https://github.com/Sunwood-ai-labs/SourceSage
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: loguru
 Requires-Dist: GitPython
 Requires-Dist: requests
+Requires-Dist: art
 
 <p align="center">
 <img src="https://raw.githubusercontent.com/Sunwood-ai-labs/SourceSage/main/docs/icon/SourceSage_icon4.png" width="100%">
 <br>
 <h1 align="center">SourceSage</h1>
 <h2 align="center">
   ～Transforming code for AI～
 
   <br>
   <img alt="PyPI - Version" src="https://img.shields.io/pypi/v/sourcesage">
-  
+  <img alt="PyPI - Format" src="https://img.shields.io/pypi/format/sourcesage">
+  <img alt="PyPI - Implementation" src="https://img.shields.io/pypi/implementation/sourcesage">
+  <img alt="PyPI - Status" src="https://img.shields.io/pypi/status/sourcesage">
+
+
   <br>
 
 </h2>
 
 
 </p>
```

### Comparing `sourcesage-4.0.5/sourcesage.egg-info/SOURCES.txt` & `sourcesage-4.0.6/sourcesage.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 sourcesage/core.py
 sourcesage.egg-info/PKG-INFO
 sourcesage.egg-info/SOURCES.txt
 sourcesage.egg-info/dependency_links.txt
 sourcesage.egg-info/entry_points.txt
 sourcesage.egg-info/requires.txt
 sourcesage.egg-info/top_level.txt
+sourcesage/config/constants.py
+sourcesage/config/language_map.json
 sourcesage/modules/ChangelogGenerator.py
 sourcesage/modules/ChangelogUtils.py
 sourcesage/modules/DiffChangelogGenerator.py
 sourcesage/modules/EnvFileHandler.py
 sourcesage/modules/GitHubIssueRetrieve.py
 sourcesage/modules/GitHubUtils.py
 sourcesage/modules/IssuesToMarkdown.py
```

### Comparing `sourcesage-4.0.5/tests/test_sourcesage.py` & `sourcesage-4.0.6/tests/test_sourcesage.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,15 +16,18 @@
     config_path = os.path.join(temp_dir, 'sourcesage.yml')
     with open(config_path, 'w') as f:
         f.write('exclude_patterns:\n  - "*.pyc"\n  - "__pycache__"\n')
 
     # パッケージのルートディレクトリを取得
     package_root = os.path.dirname(os.path.dirname(os.path.abspath(__file__)))
 
-    sys.argv = ['sourcesage', '--config', config_path, '--output', temp_dir, '--repo', package_root]
+    ignore_file_path = os.path.join(package_root, 'sourcesage', 'config', '.SourceSageignore')  # 修正
+    language_map_path = os.path.join(package_root, 'sourcesage', 'config', 'language_map.json')  # 修正
+
+    sys.argv = ['sourcesage', '--config', config_path, '--output', temp_dir, '--repo', package_root, '--owner', 'Sunwood-ai-labs', '--repository', 'SourceSage', '--ignore-file', ignore_file_path, '--language-map', language_map_path]
     main()
 
     # 出力を確認
     captured = capsys.readouterr()
     assert 'Running SourceSage...' in captured.out
     assert 'SourceSage completed successfully.' in captured.out
 
@@ -42,22 +45,25 @@
     config_path = os.path.join(temp_dir, 'sourcesage.yml')
     with open(config_path, 'w') as f:
         f.write('exclude_patterns:\n  - "*.pyc"\n  - "__pycache__"\n')
 
     # パッケージのルートディレクトリを取得
     package_root = os.path.dirname(os.path.dirname(os.path.abspath(__file__)))
 
+    ignore_file_path = os.path.join(package_root, 'sourcesage', 'config', '.SourceSageignore')  # 修正
+    language_map_path = os.path.join(package_root, 'sourcesage', 'config', 'language_map.json')  # 修正
+
     # 必要なディレクトリを作成
     necessary_dirs = ['SourceSageAssets/Changelog', 'SourceSageAssets/ISSUE_LOG', 'SourceSageAssets/ISSUES_RESOLVE', 'SourceSageAssets/STAGE_INFO']
     for dir_path in necessary_dirs:
         os.makedirs(os.path.join(temp_dir, dir_path), exist_ok=True)
 
     # SourceSageクラスを直接インスタンス化して実行
-    sourcesage = SourceSage(config_path, temp_dir, package_root)
+    sourcesage = SourceSage(config_path, temp_dir, package_root, 'Sunwood-ai-labs', 'SourceSage', ignore_file_path, language_map_path)
     sourcesage.run()
 
     # 出力ファイルが生成されたことを確認
     output_file = os.path.join(temp_dir, 'SourceSage.md')
     # assert os.path.exists(output_file)
 
     # 出力ファイルの保存場所を表示
-    print(f"Output file saved at: {output_file}")
+    print(f"Output file saved at: {output_file}")
```

