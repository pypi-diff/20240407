# Comparing `tmp/sourcesage-4.0.9.tar.gz` & `tmp/sourcesage-4.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sourcesage-4.0.9.tar", last modified: Sun Apr  7 13:54:47 2024, max compression
+gzip compressed data, was "sourcesage-4.1.1.tar", last modified: Sun Apr  7 15:38:08 2024, max compression
```

## Comparing `sourcesage-4.0.9.tar` & `sourcesage-4.1.1.tar`

### file list

```diff
@@ -1,43 +1,44 @@
-drwxrwxrwx   0        0        0        0 2024-04-07 13:54:47.327708 sourcesage-4.0.9/
--rw-rw-rw-   0        0        0     1082 2024-04-04 07:13:56.000000 sourcesage-4.0.9/LICENSE
--rw-rw-rw-   0        0        0    12824 2024-04-07 13:54:47.327708 sourcesage-4.0.9/PKG-INFO
--rw-rw-rw-   0        0        0    12547 2024-04-04 16:38:14.000000 sourcesage-4.0.9/README.md
--rw-rw-rw-   0        0        0       42 2024-04-07 13:54:47.327708 sourcesage-4.0.9/setup.cfg
--rw-rw-rw-   0        0        0      719 2024-04-07 13:54:44.000000 sourcesage-4.0.9/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-07 13:54:47.242457 sourcesage-4.0.9/sourcesage/
--rw-rw-rw-   0        0        0        0 2024-04-04 15:59:17.000000 sourcesage-4.0.9/sourcesage/__init__.py
--rw-rw-rw-   0        0        0     1441 2024-04-07 13:35:31.000000 sourcesage-4.0.9/sourcesage/cli.py
-drwxrwxrwx   0        0        0        0 2024-04-07 13:54:47.284473 sourcesage-4.0.9/sourcesage/config/
-drwxrwxrwx   0        0        0        0 2024-04-07 13:54:47.286728 sourcesage-4.0.9/sourcesage/config/ISSUES_RESOLVE/
--rw-rw-rw-   0        0        0     1113 2024-04-04 15:59:17.000000 sourcesage-4.0.9/sourcesage/config/ISSUES_RESOLVE/ISSUES_RESOLVE_TEMPLATE.md
-drwxrwxrwx   0        0        0        0 2024-04-07 13:54:47.286728 sourcesage-4.0.9/sourcesage/config/STAGE_INFO/
--rw-rw-rw-   0        0        0     1319 2024-04-04 15:59:17.000000 sourcesage-4.0.9/sourcesage/config/STAGE_INFO/STAGE_INFO_AND_ISSUES_TEMPLATE.md
--rw-rw-rw-   0        0        0     1127 2024-04-04 15:59:17.000000 sourcesage-4.0.9/sourcesage/config/STAGE_INFO/STAGE_INFO_TEMPLATE.md
-drwxrwxrwx   0        0        0        0 2024-04-07 13:54:47.292993 sourcesage-4.0.9/sourcesage/config/__pycache__/
--rw-rw-rw-   0        0        0     3229 2024-04-04 16:07:17.000000 sourcesage-4.0.9/sourcesage/config/__pycache__/constants.cpython-311.pyc
--rw-rw-rw-   0        0        0     1751 2024-04-04 15:59:17.000000 sourcesage-4.0.9/sourcesage/config/constants.py
--rw-rw-rw-   0        0        0      590 2024-04-04 15:59:17.000000 sourcesage-4.0.9/sourcesage/config/language_map.json
--rw-rw-rw-   0        0        0     4932 2024-04-07 13:51:46.000000 sourcesage-4.0.9/sourcesage/core.py
-drwxrwxrwx   0        0        0        0 2024-04-07 13:54:47.326214 sourcesage-4.0.9/sourcesage/modules/
--rw-rw-rw-   0        0        0     3885 2024-04-04 15:59:17.000000 sourcesage-4.0.9/sourcesage/modules/ChangelogGenerator.py
--rw-rw-rw-   0        0        0     1440 2024-04-04 15:59:17.000000 sourcesage-4.0.9/sourcesage/modules/ChangelogUtils.py
--rw-rw-rw-   0        0        0     4171 2024-04-04 15:59:17.000000 sourcesage-4.0.9/sourcesage/modules/DiffChangelogGenerator.py
--rw-rw-rw-   0        0        0     1073 2024-04-04 15:59:17.000000 sourcesage-4.0.9/sourcesage/modules/EnvFileHandler.py
--rw-rw-rw-   0        0        0      836 2024-04-04 15:59:17.000000 sourcesage-4.0.9/sourcesage/modules/GitHubIssueRetrieve.py
--rw-rw-rw-   0        0        0     1291 2024-04-04 15:59:17.000000 sourcesage-4.0.9/sourcesage/modules/GitHubUtils.py
--rw-rw-rw-   0        0        0     2227 2024-04-04 15:59:17.000000 sourcesage-4.0.9/sourcesage/modules/IssuesToMarkdown.py
--rw-rw-rw-   0        0        0     3036 2024-04-04 15:59:17.000000 sourcesage-4.0.9/sourcesage/modules/StageInfoGenerator.py
--rw-rw-rw-   0        0        0     2778 2024-04-04 15:59:17.000000 sourcesage-4.0.9/sourcesage/modules/StagedDiffGenerator.py
--rw-rw-rw-   0        0        0        0 2024-04-04 15:59:17.000000 sourcesage-4.0.9/sourcesage/modules/__init__.py
--rw-rw-rw-   0        0        0      930 2024-04-04 15:59:17.000000 sourcesage-4.0.9/sourcesage/modules/file_utils.py
--rw-rw-rw-   0        0        0     3261 2024-04-04 15:59:17.000000 sourcesage-4.0.9/sourcesage/modules/markdown_utils.py
--rw-rw-rw-   0        0        0     1115 2024-04-04 15:59:17.000000 sourcesage-4.0.9/sourcesage/modules/source_sage.py
-drwxrwxrwx   0        0        0        0 2024-04-07 13:54:47.276432 sourcesage-4.0.9/sourcesage.egg-info/
--rw-rw-rw-   0        0        0    12824 2024-04-07 13:54:47.000000 sourcesage-4.0.9/sourcesage.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1108 2024-04-07 13:54:47.000000 sourcesage-4.0.9/sourcesage.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-07 13:54:47.000000 sourcesage-4.0.9/sourcesage.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2024-04-07 13:54:47.000000 sourcesage-4.0.9/sourcesage.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       30 2024-04-07 13:54:47.000000 sourcesage-4.0.9/sourcesage.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-07 13:54:47.000000 sourcesage-4.0.9/sourcesage.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-07 13:54:47.327708 sourcesage-4.0.9/tests/
--rw-rw-rw-   0        0        0     3207 2024-04-07 13:35:05.000000 sourcesage-4.0.9/tests/test_sourcesage.py
+drwxrwxrwx   0        0        0        0 2024-04-07 15:38:08.562589 sourcesage-4.1.1/
+-rw-rw-rw-   0        0        0     1082 2024-04-04 07:13:56.000000 sourcesage-4.1.1/LICENSE
+-rw-rw-rw-   0        0        0    15634 2024-04-07 15:38:08.562589 sourcesage-4.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0    15236 2024-04-07 15:35:50.000000 sourcesage-4.1.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-07 15:38:08.562589 sourcesage-4.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      915 2024-04-07 15:38:06.000000 sourcesage-4.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-07 15:38:08.476258 sourcesage-4.1.1/sourcesage/
+-rw-rw-rw-   0        0        0        0 2024-04-04 15:59:17.000000 sourcesage-4.1.1/sourcesage/__init__.py
+-rw-rw-rw-   0        0        0     1441 2024-04-07 15:31:18.000000 sourcesage-4.1.1/sourcesage/cli.py
+drwxrwxrwx   0        0        0        0 2024-04-07 15:38:08.507960 sourcesage-4.1.1/sourcesage/config/
+-rw-rw-rw-   0        0        0      306 2024-04-07 15:31:18.000000 sourcesage-4.1.1/sourcesage/config/.SourceSageignore
+drwxrwxrwx   0        0        0        0 2024-04-07 15:38:08.508962 sourcesage-4.1.1/sourcesage/config/ISSUES_RESOLVE/
+-rw-rw-rw-   0        0        0     1113 2024-04-04 15:59:17.000000 sourcesage-4.1.1/sourcesage/config/ISSUES_RESOLVE/ISSUES_RESOLVE_TEMPLATE.md
+drwxrwxrwx   0        0        0        0 2024-04-07 15:38:08.510568 sourcesage-4.1.1/sourcesage/config/STAGE_INFO/
+-rw-rw-rw-   0        0        0     1319 2024-04-04 15:59:17.000000 sourcesage-4.1.1/sourcesage/config/STAGE_INFO/STAGE_INFO_AND_ISSUES_TEMPLATE.md
+-rw-rw-rw-   0        0        0     1127 2024-04-04 15:59:17.000000 sourcesage-4.1.1/sourcesage/config/STAGE_INFO/STAGE_INFO_TEMPLATE.md
+drwxrwxrwx   0        0        0        0 2024-04-07 15:38:08.510568 sourcesage-4.1.1/sourcesage/config/__pycache__/
+-rw-rw-rw-   0        0        0     3229 2024-04-04 16:07:17.000000 sourcesage-4.1.1/sourcesage/config/__pycache__/constants.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1773 2024-04-07 15:31:18.000000 sourcesage-4.1.1/sourcesage/config/constants.py
+-rw-rw-rw-   0        0        0      590 2024-04-04 15:59:17.000000 sourcesage-4.1.1/sourcesage/config/language_map.json
+-rw-rw-rw-   0        0        0     4932 2024-04-07 15:31:18.000000 sourcesage-4.1.1/sourcesage/core.py
+drwxrwxrwx   0        0        0        0 2024-04-07 15:38:08.562589 sourcesage-4.1.1/sourcesage/modules/
+-rw-rw-rw-   0        0        0     3915 2024-04-07 15:37:34.000000 sourcesage-4.1.1/sourcesage/modules/ChangelogGenerator.py
+-rw-rw-rw-   0        0        0     1440 2024-04-04 15:59:17.000000 sourcesage-4.1.1/sourcesage/modules/ChangelogUtils.py
+-rw-rw-rw-   0        0        0     4171 2024-04-04 15:59:17.000000 sourcesage-4.1.1/sourcesage/modules/DiffChangelogGenerator.py
+-rw-rw-rw-   0        0        0     1073 2024-04-04 15:59:17.000000 sourcesage-4.1.1/sourcesage/modules/EnvFileHandler.py
+-rw-rw-rw-   0        0        0      836 2024-04-04 15:59:17.000000 sourcesage-4.1.1/sourcesage/modules/GitHubIssueRetrieve.py
+-rw-rw-rw-   0        0        0     1291 2024-04-04 15:59:17.000000 sourcesage-4.1.1/sourcesage/modules/GitHubUtils.py
+-rw-rw-rw-   0        0        0     2227 2024-04-04 15:59:17.000000 sourcesage-4.1.1/sourcesage/modules/IssuesToMarkdown.py
+-rw-rw-rw-   0        0        0     3036 2024-04-04 15:59:17.000000 sourcesage-4.1.1/sourcesage/modules/StageInfoGenerator.py
+-rw-rw-rw-   0        0        0     2778 2024-04-04 15:59:17.000000 sourcesage-4.1.1/sourcesage/modules/StagedDiffGenerator.py
+-rw-rw-rw-   0        0        0        0 2024-04-04 15:59:17.000000 sourcesage-4.1.1/sourcesage/modules/__init__.py
+-rw-rw-rw-   0        0        0      930 2024-04-04 15:59:17.000000 sourcesage-4.1.1/sourcesage/modules/file_utils.py
+-rw-rw-rw-   0        0        0     3261 2024-04-04 15:59:17.000000 sourcesage-4.1.1/sourcesage/modules/markdown_utils.py
+-rw-rw-rw-   0        0        0     1115 2024-04-04 15:59:17.000000 sourcesage-4.1.1/sourcesage/modules/source_sage.py
+drwxrwxrwx   0        0        0        0 2024-04-07 15:38:08.501970 sourcesage-4.1.1/sourcesage.egg-info/
+-rw-rw-rw-   0        0        0    15634 2024-04-07 15:38:08.000000 sourcesage-4.1.1/sourcesage.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1144 2024-04-07 15:38:08.000000 sourcesage-4.1.1/sourcesage.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-07 15:38:08.000000 sourcesage-4.1.1/sourcesage.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2024-04-07 15:38:08.000000 sourcesage-4.1.1/sourcesage.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       30 2024-04-07 15:38:08.000000 sourcesage-4.1.1/sourcesage.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-07 15:38:08.000000 sourcesage-4.1.1/sourcesage.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-07 15:38:08.562589 sourcesage-4.1.1/tests/
+-rw-rw-rw-   0        0        0     3207 2024-04-07 15:31:18.000000 sourcesage-4.1.1/tests/test_sourcesage.py
```

### Comparing `sourcesage-4.0.9/LICENSE` & `sourcesage-4.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sourcesage-4.0.9/setup.py` & `sourcesage-4.1.1/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,18 +3,24 @@
 
 # READMEファイルの内容を読み込む
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='sourcesage',
-    version='4.0.9',
+    version='4.1.1',
     packages=find_packages(),
+    classifiers=[
+        "Development Status :: 4 - Beta",
+        "Intended Audience :: Developers",
+        "Topic :: Utilities",
+    ],
     package_data={
-        'sourcesage': ['config/**/**', ],
+        'sourcesage': ['config/**/**', 
+                       'config/.SourceSageignore'],
     },
     entry_points={
         'console_scripts': [
             'sourcesage=sourcesage.cli:main',
         ],
     },
     long_description=long_description,
```

### Comparing `sourcesage-4.0.9/sourcesage/cli.py` & `sourcesage-4.1.1/sourcesage/cli.py`

 * *Files identical despite different names*

### Comparing `sourcesage-4.0.9/sourcesage/config/ISSUES_RESOLVE/ISSUES_RESOLVE_TEMPLATE.md` & `sourcesage-4.1.1/sourcesage/config/ISSUES_RESOLVE/ISSUES_RESOLVE_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `sourcesage-4.0.9/sourcesage/config/STAGE_INFO/STAGE_INFO_AND_ISSUES_TEMPLATE.md` & `sourcesage-4.1.1/sourcesage/config/STAGE_INFO/STAGE_INFO_AND_ISSUES_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `sourcesage-4.0.9/sourcesage/config/STAGE_INFO/STAGE_INFO_TEMPLATE.md` & `sourcesage-4.1.1/sourcesage/config/STAGE_INFO/STAGE_INFO_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `sourcesage-4.0.9/sourcesage/config/__pycache__/constants.cpython-311.pyc` & `sourcesage-4.1.1/sourcesage/config/__pycache__/constants.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `sourcesage-4.0.9/sourcesage/config/constants.py` & `sourcesage-4.1.1/sourcesage/config/constants.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,25 +10,25 @@
         self.REPO_PATH = self.BASE_DIR
         self.CONFIG_DIR = os.path.join(self.BASE_DIR, 'config')
         self.DOCS_DIR = os.path.join(self.BASE_DIR, "config")
 
         self.LANGUAGE_MAP_FILE = os.path.join(self.CONFIG_DIR, 'language_map.json')
         self.IGNORE_FILE = os.path.join(self.CONFIG_DIR, '.SourceSageignore')
 
-        self.SOURCE_SAGE_MD = "SourceSage.md"
+        self.SOURCE_SAGE_MD = "DocuMind.md"
         self.CHANGELOG_DIR = "Changelog"
         self.STAGED_DIFF_MD = "STAGED_DIFF.md"
 
         self.set_output_dir(output_dir)
 
     def set_output_dir(self, output_dir):
         self.SOURCE_SAGE_ASSETS_DIR = os.path.join(output_dir, "SourceSageAssets")
         self.ISSUE_LOG_DIR = os.path.join(self.SOURCE_SAGE_ASSETS_DIR, "ISSUE_LOG")
-        self.ISSUES_RESOLVE_DIR = os.path.join(self.SOURCE_SAGE_ASSETS_DIR, "ISSUES_RESOLVE")
-        self.STAGE_INFO_DIR = os.path.join(self.SOURCE_SAGE_ASSETS_DIR, "STAGE_INFO")
+        self.ISSUES_RESOLVE_DIR = os.path.join(self.SOURCE_SAGE_ASSETS_DIR, "ISSUE_WISE/ISSUES_RESOLVE")
+        self.STAGE_INFO_DIR = os.path.join(self.SOURCE_SAGE_ASSETS_DIR, "COMMIT_CRAFT/STAGE_INFO")
 
         self.TEMPLATE_ISSUES_RESOLVE_DIR = os.path.join(self.DOCS_DIR, "ISSUES_RESOLVE")
         self.ISSUES_RESOLVE_TEMPLATE_MD = "ISSUES_RESOLVE_TEMPLATE.md"
 
         self.TEMPLATE_STAGE_INFO_DIR = os.path.join(self.DOCS_DIR, "STAGE_INFO")
         self.STAGE_INFO_OUTPUT_MD = "STAGE_INFO_AND_ISSUES_AND_PROMT.md"
         self.STAGE_INFO_TEMPLATE_MD = "STAGE_INFO_AND_ISSUES_TEMPLATE.md"
```

### Comparing `sourcesage-4.0.9/sourcesage/config/language_map.json` & `sourcesage-4.1.1/sourcesage/config/language_map.json`

 * *Files identical despite different names*

### Comparing `sourcesage-4.0.9/sourcesage/core.py` & `sourcesage-4.1.1/sourcesage/core.py`

 * *Files identical despite different names*

### Comparing `sourcesage-4.0.9/sourcesage/modules/ChangelogGenerator.py` & `sourcesage-4.1.1/sourcesage/modules/ChangelogGenerator.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
         print(branches)
 
         feature_branches = [branch for branch in branches if 'feature/' in branch]
         other_branches = [branch for branch in branches if 'feature/' not in branch]
 
         for branch in other_branches:
             branch_name = branch.replace('origin/', '')
-            output_file = os.path.join(self.output_dir, f"CHANGELOG_{branch_name}.md").replace("release/", "release_")
+            output_file = os.path.join(self.output_dir, f"CHANGELOG_{branch_name}.md").replace("release/", "release_").replace("bugfix/", "bugfix_")
             logger.info(f"Generating changelog for branch '{branch_name}'...")
             self.generate_changelog(branch_name, output_file)
 
         if feature_branches:
             output_file = os.path.join(self.output_dir, "CHANGELOG_features.md")
             with open(output_file, 'w', encoding='utf-8') as f:
                 f.write(f"# Changelog - Features\n\n")
```

### Comparing `sourcesage-4.0.9/sourcesage/modules/ChangelogUtils.py` & `sourcesage-4.1.1/sourcesage/modules/ChangelogUtils.py`

 * *Files identical despite different names*

### Comparing `sourcesage-4.0.9/sourcesage/modules/DiffChangelogGenerator.py` & `sourcesage-4.1.1/sourcesage/modules/DiffChangelogGenerator.py`

 * *Files identical despite different names*

### Comparing `sourcesage-4.0.9/sourcesage/modules/EnvFileHandler.py` & `sourcesage-4.1.1/sourcesage/modules/EnvFileHandler.py`

 * *Files identical despite different names*

### Comparing `sourcesage-4.0.9/sourcesage/modules/GitHubIssueRetrieve.py` & `sourcesage-4.1.1/sourcesage/modules/GitHubIssueRetrieve.py`

 * *Files identical despite different names*

### Comparing `sourcesage-4.0.9/sourcesage/modules/GitHubUtils.py` & `sourcesage-4.1.1/sourcesage/modules/GitHubUtils.py`

 * *Files identical despite different names*

### Comparing `sourcesage-4.0.9/sourcesage/modules/IssuesToMarkdown.py` & `sourcesage-4.1.1/sourcesage/modules/IssuesToMarkdown.py`

 * *Files identical despite different names*

### Comparing `sourcesage-4.0.9/sourcesage/modules/StageInfoGenerator.py` & `sourcesage-4.1.1/sourcesage/modules/StageInfoGenerator.py`

 * *Files identical despite different names*

### Comparing `sourcesage-4.0.9/sourcesage/modules/StagedDiffGenerator.py` & `sourcesage-4.1.1/sourcesage/modules/StagedDiffGenerator.py`

 * *Files identical despite different names*

### Comparing `sourcesage-4.0.9/sourcesage/modules/file_utils.py` & `sourcesage-4.1.1/sourcesage/modules/file_utils.py`

 * *Files identical despite different names*

### Comparing `sourcesage-4.0.9/sourcesage/modules/markdown_utils.py` & `sourcesage-4.1.1/sourcesage/modules/markdown_utils.py`

 * *Files identical despite different names*

### Comparing `sourcesage-4.0.9/sourcesage/modules/source_sage.py` & `sourcesage-4.1.1/sourcesage/modules/source_sage.py`

 * *Files identical despite different names*

### Comparing `sourcesage-4.0.9/sourcesage.egg-info/SOURCES.txt` & `sourcesage-4.1.1/sourcesage.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 sourcesage/core.py
 sourcesage.egg-info/PKG-INFO
 sourcesage.egg-info/SOURCES.txt
 sourcesage.egg-info/dependency_links.txt
 sourcesage.egg-info/entry_points.txt
 sourcesage.egg-info/requires.txt
 sourcesage.egg-info/top_level.txt
+sourcesage/config/.SourceSageignore
 sourcesage/config/constants.py
 sourcesage/config/language_map.json
 sourcesage/config/ISSUES_RESOLVE/ISSUES_RESOLVE_TEMPLATE.md
 sourcesage/config/STAGE_INFO/STAGE_INFO_AND_ISSUES_TEMPLATE.md
 sourcesage/config/STAGE_INFO/STAGE_INFO_TEMPLATE.md
 sourcesage/config/__pycache__/constants.cpython-311.pyc
 sourcesage/modules/ChangelogGenerator.py
```

### Comparing `sourcesage-4.0.9/tests/test_sourcesage.py` & `sourcesage-4.1.1/tests/test_sourcesage.py`

 * *Files identical despite different names*

