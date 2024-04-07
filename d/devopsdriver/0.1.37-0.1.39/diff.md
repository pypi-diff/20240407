# Comparing `tmp/devopsdriver-0.1.37.tar.gz` & `tmp/devopsdriver-0.1.39.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "devopsdriver-0.1.37.tar", last modified: Sat Apr  6 00:14:02 2024, max compression
+gzip compressed data, was "devopsdriver-0.1.39.tar", last modified: Sat Apr  6 22:18:59 2024, max compression
```

## Comparing `devopsdriver-0.1.37.tar` & `devopsdriver-0.1.39.tar`

### file list

```diff
@@ -1,33 +1,40 @@
-drwxr-xr-x   0 marcp      (501) staff       (20)        0 2024-04-06 00:14:02.739311 devopsdriver-0.1.37/
--rw-r--r--   0 marcp      (501) staff       (20)     1211 2024-03-30 20:53:59.000000 devopsdriver-0.1.37/LICENSE
--rw-r--r--   0 marcp      (501) staff       (20)    10268 2024-04-06 00:14:02.739063 devopsdriver-0.1.37/PKG-INFO
--rw-r--r--   0 marcp      (501) staff       (20)     7672 2024-04-06 00:13:19.000000 devopsdriver-0.1.37/README.md
-drwxr-xr-x   0 marcp      (501) staff       (20)        0 2024-04-06 00:14:02.736329 devopsdriver-0.1.37/devopsdriver/
--rw-r--r--   0 marcp      (501) staff       (20)      207 2024-04-06 00:13:02.000000 devopsdriver-0.1.37/devopsdriver/__init__.py
-drwxr-xr-x   0 marcp      (501) staff       (20)        0 2024-04-06 00:14:02.737197 devopsdriver-0.1.37/devopsdriver/azdo/
--rw-r--r--   0 marcp      (501) staff       (20)      381 2024-04-04 23:50:50.000000 devopsdriver-0.1.37/devopsdriver/azdo/__init__.py
--rw-r--r--   0 marcp      (501) staff       (20)     1866 2024-04-04 23:50:50.000000 devopsdriver-0.1.37/devopsdriver/azdo/clients.py
-drwxr-xr-x   0 marcp      (501) staff       (20)        0 2024-04-06 00:14:02.737756 devopsdriver-0.1.37/devopsdriver/azdo/workitem/
--rw-r--r--   0 marcp      (501) staff       (20)      107 2024-04-04 23:50:50.000000 devopsdriver-0.1.37/devopsdriver/azdo/workitem/__init__.py
--rw-r--r--   0 marcp      (501) staff       (20)     2952 2024-04-04 23:50:50.000000 devopsdriver-0.1.37/devopsdriver/azdo/workitem/client.py
--rw-r--r--   0 marcp      (501) staff       (20)     7791 2024-04-05 02:01:31.000000 devopsdriver-0.1.37/devopsdriver/azdo/workitem/wiql.py
--rw-r--r--   0 marcp      (501) staff       (20)     1445 2024-04-04 23:50:50.000000 devopsdriver-0.1.37/devopsdriver/azdo/workitem/workitem.py
--rw-r--r--   0 marcp      (501) staff       (20)     2998 2024-04-04 23:50:50.000000 devopsdriver-0.1.37/devopsdriver/sendmail.py
--rw-r--r--   0 marcp      (501) staff       (20)    13249 2024-04-05 00:18:06.000000 devopsdriver-0.1.37/devopsdriver/settings.py
--rw-r--r--   0 marcp      (501) staff       (20)     1075 2024-04-06 00:08:39.000000 devopsdriver-0.1.37/devopsdriver/template.py
-drwxr-xr-x   0 marcp      (501) staff       (20)        0 2024-04-06 00:14:02.738864 devopsdriver-0.1.37/devopsdriver.egg-info/
--rw-r--r--   0 marcp      (501) staff       (20)    10268 2024-04-06 00:14:02.000000 devopsdriver-0.1.37/devopsdriver.egg-info/PKG-INFO
--rw-r--r--   0 marcp      (501) staff       (20)      716 2024-04-06 00:14:02.000000 devopsdriver-0.1.37/devopsdriver.egg-info/SOURCES.txt
--rw-r--r--   0 marcp      (501) staff       (20)        1 2024-04-06 00:14:02.000000 devopsdriver-0.1.37/devopsdriver.egg-info/dependency_links.txt
--rw-r--r--   0 marcp      (501) staff       (20)       83 2024-04-06 00:14:02.000000 devopsdriver-0.1.37/devopsdriver.egg-info/requires.txt
--rw-r--r--   0 marcp      (501) staff       (20)       13 2024-04-06 00:14:02.000000 devopsdriver-0.1.37/devopsdriver.egg-info/top_level.txt
--rw-r--r--   0 marcp      (501) staff       (20)     1335 2024-04-06 00:08:39.000000 devopsdriver-0.1.37/pyproject.toml
--rw-r--r--   0 marcp      (501) staff       (20)       38 2024-04-06 00:14:02.739348 devopsdriver-0.1.37/setup.cfg
-drwxr-xr-x   0 marcp      (501) staff       (20)        0 2024-04-06 00:14:02.738698 devopsdriver-0.1.37/tests/
--rw-r--r--   0 marcp      (501) staff       (20)     5342 2024-04-04 23:50:50.000000 devopsdriver-0.1.37/tests/test_azure_clients.py
--rw-r--r--   0 marcp      (501) staff       (20)     4201 2024-04-04 23:50:50.000000 devopsdriver-0.1.37/tests/test_azure_workitem.py
--rw-r--r--   0 marcp      (501) staff       (20)     1740 2024-04-04 23:50:50.000000 devopsdriver-0.1.37/tests/test_azure_workitem_client.py
--rw-r--r--   0 marcp      (501) staff       (20)     2391 2024-04-05 02:01:31.000000 devopsdriver-0.1.37/tests/test_azure_workitem_wiql.py
--rw-r--r--   0 marcp      (501) staff       (20)     4457 2024-04-04 23:59:14.000000 devopsdriver-0.1.37/tests/test_sendmail.py
--rw-r--r--   0 marcp      (501) staff       (20)    11669 2024-04-05 00:09:40.000000 devopsdriver-0.1.37/tests/test_settings.py
--rw-r--r--   0 marcp      (501) staff       (20)      886 2024-04-06 00:08:39.000000 devopsdriver-0.1.37/tests/test_template.py
+drwxr-xr-x   0 marcp      (501) staff       (20)        0 2024-04-06 22:18:59.299766 devopsdriver-0.1.39/
+-rw-r--r--   0 marcp      (501) staff       (20)     1211 2024-03-30 20:53:59.000000 devopsdriver-0.1.39/LICENSE
+-rw-r--r--   0 marcp      (501) staff       (20)    10942 2024-04-06 22:18:59.299525 devopsdriver-0.1.39/PKG-INFO
+-rw-r--r--   0 marcp      (501) staff       (20)     8101 2024-04-06 22:18:27.000000 devopsdriver-0.1.39/README.md
+drwxr-xr-x   0 marcp      (501) staff       (20)        0 2024-04-06 22:18:59.295849 devopsdriver-0.1.39/devopsdriver/
+-rw-r--r--   0 marcp      (501) staff       (20)       87 2024-04-06 22:15:02.000000 devopsdriver-0.1.39/devopsdriver/__init__.py
+drwxr-xr-x   0 marcp      (501) staff       (20)        0 2024-04-06 22:18:59.296963 devopsdriver-0.1.39/devopsdriver/azdo/
+-rw-r--r--   0 marcp      (501) staff       (20)      423 2024-04-06 20:27:22.000000 devopsdriver-0.1.39/devopsdriver/azdo/__init__.py
+-rw-r--r--   0 marcp      (501) staff       (20)     1882 2024-04-06 20:27:22.000000 devopsdriver-0.1.39/devopsdriver/azdo/clients.py
+-rw-r--r--   0 marcp      (501) staff       (20)     2284 2024-04-06 17:54:48.000000 devopsdriver-0.1.39/devopsdriver/azdo/timestamp.py
+drwxr-xr-x   0 marcp      (501) staff       (20)        0 2024-04-06 22:18:59.297490 devopsdriver-0.1.39/devopsdriver/azdo/workitem/
+-rw-r--r--   0 marcp      (501) staff       (20)       29 2024-04-06 20:27:22.000000 devopsdriver-0.1.39/devopsdriver/azdo/workitem/__init__.py
+-rw-r--r--   0 marcp      (501) staff       (20)     2963 2024-04-06 20:27:22.000000 devopsdriver-0.1.39/devopsdriver/azdo/workitem/client.py
+-rw-r--r--   0 marcp      (501) staff       (20)     7792 2024-04-06 20:27:22.000000 devopsdriver-0.1.39/devopsdriver/azdo/workitem/wiql.py
+-rw-r--r--   0 marcp      (501) staff       (20)     1658 2024-04-06 20:27:22.000000 devopsdriver-0.1.39/devopsdriver/azdo/workitem/workitem.py
+-rw-r--r--   0 marcp      (501) staff       (20)     1227 2024-04-06 22:13:48.000000 devopsdriver-0.1.39/devopsdriver/manage_settings.py
+-rw-r--r--   0 marcp      (501) staff       (20)     3002 2024-04-06 20:27:22.000000 devopsdriver-0.1.39/devopsdriver/sendmail.py
+-rw-r--r--   0 marcp      (501) staff       (20)    12276 2024-04-06 22:13:48.000000 devopsdriver-0.1.39/devopsdriver/settings.py
+-rw-r--r--   0 marcp      (501) staff       (20)     1077 2024-04-06 21:50:31.000000 devopsdriver-0.1.39/devopsdriver/template.py
+drwxr-xr-x   0 marcp      (501) staff       (20)        0 2024-04-06 22:18:59.297616 devopsdriver-0.1.39/devopsdriver/templates/
+-rw-r--r--   0 marcp      (501) staff       (20)      483 2024-04-06 22:13:48.000000 devopsdriver-0.1.39/devopsdriver/templates/manage_settings.txt.mako
+drwxr-xr-x   0 marcp      (501) staff       (20)        0 2024-04-06 22:18:59.299060 devopsdriver-0.1.39/devopsdriver.egg-info/
+-rw-r--r--   0 marcp      (501) staff       (20)    10942 2024-04-06 22:18:59.000000 devopsdriver-0.1.39/devopsdriver.egg-info/PKG-INFO
+-rw-r--r--   0 marcp      (501) staff       (20)      926 2024-04-06 22:18:59.000000 devopsdriver-0.1.39/devopsdriver.egg-info/SOURCES.txt
+-rw-r--r--   0 marcp      (501) staff       (20)        1 2024-04-06 22:18:59.000000 devopsdriver-0.1.39/devopsdriver.egg-info/dependency_links.txt
+-rw-r--r--   0 marcp      (501) staff       (20)       63 2024-04-06 22:18:59.000000 devopsdriver-0.1.39/devopsdriver.egg-info/entry_points.txt
+-rw-r--r--   0 marcp      (501) staff       (20)      163 2024-04-06 22:18:59.000000 devopsdriver-0.1.39/devopsdriver.egg-info/requires.txt
+-rw-r--r--   0 marcp      (501) staff       (20)       13 2024-04-06 22:18:59.000000 devopsdriver-0.1.39/devopsdriver.egg-info/top_level.txt
+-rw-r--r--   0 marcp      (501) staff       (20)     1599 2024-04-06 22:13:48.000000 devopsdriver-0.1.39/pyproject.toml
+-rw-r--r--   0 marcp      (501) staff       (20)       38 2024-04-06 22:18:59.299819 devopsdriver-0.1.39/setup.cfg
+drwxr-xr-x   0 marcp      (501) staff       (20)        0 2024-04-06 22:18:59.298749 devopsdriver-0.1.39/tests/
+-rw-r--r--   0 marcp      (501) staff       (20)     5347 2024-04-06 20:27:22.000000 devopsdriver-0.1.39/tests/test_azure_clients.py
+-rw-r--r--   0 marcp      (501) staff       (20)     7779 2024-04-06 17:20:58.000000 devopsdriver-0.1.39/tests/test_azure_timestamp.py
+-rw-r--r--   0 marcp      (501) staff       (20)     4736 2024-04-06 17:54:48.000000 devopsdriver-0.1.39/tests/test_azure_workitem.py
+-rw-r--r--   0 marcp      (501) staff       (20)     1740 2024-04-04 23:50:50.000000 devopsdriver-0.1.39/tests/test_azure_workitem_client.py
+-rw-r--r--   0 marcp      (501) staff       (20)     2391 2024-04-05 02:01:31.000000 devopsdriver-0.1.39/tests/test_azure_workitem_wiql.py
+-rw-r--r--   0 marcp      (501) staff       (20)     2624 2024-04-06 22:13:48.000000 devopsdriver-0.1.39/tests/test_manage_settings.py
+-rw-r--r--   0 marcp      (501) staff       (20)     4466 2024-04-06 20:27:22.000000 devopsdriver-0.1.39/tests/test_sendmail.py
+-rw-r--r--   0 marcp      (501) staff       (20)    10203 2024-04-06 22:13:48.000000 devopsdriver-0.1.39/tests/test_settings.py
+-rw-r--r--   0 marcp      (501) staff       (20)      886 2024-04-06 20:14:20.000000 devopsdriver-0.1.39/tests/test_template.py
```

### Comparing `devopsdriver-0.1.37/LICENSE` & `devopsdriver-0.1.39/LICENSE`

 * *Files identical despite different names*

### Comparing `devopsdriver-0.1.37/PKG-INFO` & `devopsdriver-0.1.39/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: devopsdriver
-Version: 0.1.37
+Version: 0.1.39
 Summary: DevOps tools
 Author-email: Marc Page <marcallenpage@gmail.com>
 License: This is free and unencumbered software released into the public domain.
         
         Anyone is free to copy, modify, publish, use, compile, sell, or
         distribute this software, either in source code form or as a compiled
         binary, for any purpose, commercial or non-commercial, and by any
@@ -47,17 +47,24 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: PyYAML==6.0.1
 Requires-Dist: keyring==25.0.0
 Requires-Dist: setuptools==69.0.2
 Requires-Dist: azure-devops==7.1.0b4
 Requires-Dist: Mako==1.3.2
+Provides-Extra: dev
+Requires-Dist: black>=24.3.0; extra == "dev"
+Requires-Dist: pylint>=3.1.0; extra == "dev"
+Provides-Extra: test
+Requires-Dist: pytest>=8.1.1; extra == "test"
+Requires-Dist: coverage>=7.4.4; extra == "test"
+Provides-Extra: doc
 
 ![status sheild](https://img.shields.io/static/v1?label=status&message=beta&color=blue&style=plastic)
-[![status sheild](https://img.shields.io/static/v1?label=released&message=v0.1.37&color=active&style=plastic)](https://pypi.org/project/devopsdriver/0.1.37/)
+[![status sheild](https://img.shields.io/static/v1?label=released&message=v0.1.39&color=active&style=plastic)](https://pypi.org/project/devopsdriver/0.1.39/)
 [![GitHub](https://img.shields.io/github/license/marcpage/devops-driver?style=plastic)](https://github.com/marcpage/devops-driver?tab=Unlicense-1-ov-file#readme)
 [![GitHub contributors](https://img.shields.io/github/contributors/marcpage/devops-driver?style=flat)](https://github.com/marcpage/devops-driver/graphs/contributors)
 [![PR's Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat)](http://makeapullrequest.com)
 
 [![commit sheild](https://img.shields.io/github/last-commit/marcpage/devops-driver?style=plastic)](https://github.com/marcpage/devops-driver/commits)
 [![activity sheild](https://img.shields.io/github/commit-activity/m/marcpage/devops-driver?style=plastic)](https://github.com/marcpage/devops-driver/commits)
 [![GitHub top language](https://img.shields.io/github/languages/top/marcpage/devops-driver?style=plastic)](https://github.com/marcpage/devops-driver)
@@ -80,15 +87,24 @@
 [![macOS](https://img.shields.io/static/v1?label=&message=macOS&color=white&logoColor=black&style=plastic&logo=apple)](https://apple.com/)
 [![Linux](https://img.shields.io/static/v1?label=&message=Linux&color=seashell&logoColor=black&style=plastic&logo=linux)](https://linux.org/)
 
 # devops-driver
 
 Devops-driver is a collection of tools to help streamline developer's experience and gain insights into various processes.
 
-## Access to secrets
+## Tools
+
+devopsdriver is a toolbox that helps to quickly put together reports. Some of the items in the toolbox are:
+
+- **Settings**: store data, constants, settings, keys, tokens, etc. both in and out of the repository
+- **send_email**: send emails over SMTP (including SSL), using `Settings` to store credentials
+- **Template**: Simplify generating reports using `.mako` templates
+- **Azure.workitem**: Search for and inspect Azure DevOps work items
+
+## Example use-case
 
 To allow seamless work in both pipelines as well as in the development environment, the `Settings` object gives you access to common settings among multiple scripts, secrets, and configuration constants in a way the helps keep secrets out of the repository but runs just as well in the pipeline as your machine.
 
 Say you want a pipeline that looks for User Stories that are newer than 3 days and send out an email.
 
 ### \<platform dependent path\>/devopsdriver.yml
 ```yaml
@@ -97,42 +113,43 @@
 
 secrets:
     azure.token: azure/token
     smtp.password: smtp/password
 ```
 
 This file is in a global place (location varies by OS) and stores information that you may not want in your repository or is specific to development. 
-The `secrets` are extra sensative and are stored in the OS keychain.
 
 | Platform | Global Directory       |
 |----------|------------------------|
 | Windows  | %APPDATA%\             |
 | Linux    | ~/.devopsdriver/       |
 | macOS    | ~/Library/Preferences/ |
 
+The `secrets` are extra sensative and are stored in the OS keychain.
+
 ### Set secrets in the keychain
 ```bash
 $ python3 -m venv .venv
 $ source .venv/bin/activate
 $ pip install devopsdriver
-$ python -m devopsdriver.settings --secrets
+$ settings --secrets
 secret: smtp.password  key: smtp/password
 smtp.password (smtp/password): ****
 secret: azure.token  key: azure/token
 smtp.password (azure/token): ****
-$ python -m devopsdriver.settings --secrets
+$ settings --secrets
 secret: azure.token  key: azure/token
 	Value set
 secret: smtp.password  key: smtp/password
 	Value set
 $
 ```
-The first call to `devopsdriver.settings` will look for every secret and check if they are already set in the keychain.
+The first call to `settings` will look for every secret and check if they are already set in the keychain.
 For any secret that has not been set in the keychain, you will be prompted to enter the password to store.
-The second call to `devopsdriver.settings` will verify that all the values have been set in the keychain.
+The second call to `settings` will verify that all the values have been set in the keychain.
 
 ### devopsdriver.yml
 ```yaml
 azure:
     url: https://dev.azure.com/MyCompany
 
 smtp:
@@ -170,14 +187,16 @@
 <ul>
     % for story in stories:
     <li>${story.id} ${story.title}</li>
     % endfor
 </ul>
 ```
 
+This file is the template for the email body.
+
 ### new_stories.py
 ```python
 from datetime import date, timedelta
 
 from devopsdriver import Settings, Azure, send_email, Template
 from devopsdriver.azdo import Wiql, GreaterThan
```

### Comparing `devopsdriver-0.1.37/README.md` & `devopsdriver-0.1.39/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ![status sheild](https://img.shields.io/static/v1?label=status&message=beta&color=blue&style=plastic)
-[![status sheild](https://img.shields.io/static/v1?label=released&message=v0.1.37&color=active&style=plastic)](https://pypi.org/project/devopsdriver/0.1.37/)
+[![status sheild](https://img.shields.io/static/v1?label=released&message=v0.1.39&color=active&style=plastic)](https://pypi.org/project/devopsdriver/0.1.39/)
 [![GitHub](https://img.shields.io/github/license/marcpage/devops-driver?style=plastic)](https://github.com/marcpage/devops-driver?tab=Unlicense-1-ov-file#readme)
 [![GitHub contributors](https://img.shields.io/github/contributors/marcpage/devops-driver?style=flat)](https://github.com/marcpage/devops-driver/graphs/contributors)
 [![PR's Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat)](http://makeapullrequest.com)
 
 [![commit sheild](https://img.shields.io/github/last-commit/marcpage/devops-driver?style=plastic)](https://github.com/marcpage/devops-driver/commits)
 [![activity sheild](https://img.shields.io/github/commit-activity/m/marcpage/devops-driver?style=plastic)](https://github.com/marcpage/devops-driver/commits)
 [![GitHub top language](https://img.shields.io/github/languages/top/marcpage/devops-driver?style=plastic)](https://github.com/marcpage/devops-driver)
@@ -26,15 +26,24 @@
 [![macOS](https://img.shields.io/static/v1?label=&message=macOS&color=white&logoColor=black&style=plastic&logo=apple)](https://apple.com/)
 [![Linux](https://img.shields.io/static/v1?label=&message=Linux&color=seashell&logoColor=black&style=plastic&logo=linux)](https://linux.org/)
 
 # devops-driver
 
 Devops-driver is a collection of tools to help streamline developer's experience and gain insights into various processes.
 
-## Access to secrets
+## Tools
+
+devopsdriver is a toolbox that helps to quickly put together reports. Some of the items in the toolbox are:
+
+- **Settings**: store data, constants, settings, keys, tokens, etc. both in and out of the repository
+- **send_email**: send emails over SMTP (including SSL), using `Settings` to store credentials
+- **Template**: Simplify generating reports using `.mako` templates
+- **Azure.workitem**: Search for and inspect Azure DevOps work items
+
+## Example use-case
 
 To allow seamless work in both pipelines as well as in the development environment, the `Settings` object gives you access to common settings among multiple scripts, secrets, and configuration constants in a way the helps keep secrets out of the repository but runs just as well in the pipeline as your machine.
 
 Say you want a pipeline that looks for User Stories that are newer than 3 days and send out an email.
 
 ### \<platform dependent path\>/devopsdriver.yml
 ```yaml
@@ -43,42 +52,43 @@
 
 secrets:
     azure.token: azure/token
     smtp.password: smtp/password
 ```
 
 This file is in a global place (location varies by OS) and stores information that you may not want in your repository or is specific to development. 
-The `secrets` are extra sensative and are stored in the OS keychain.
 
 | Platform | Global Directory       |
 |----------|------------------------|
 | Windows  | %APPDATA%\             |
 | Linux    | ~/.devopsdriver/       |
 | macOS    | ~/Library/Preferences/ |
 
+The `secrets` are extra sensative and are stored in the OS keychain.
+
 ### Set secrets in the keychain
 ```bash
 $ python3 -m venv .venv
 $ source .venv/bin/activate
 $ pip install devopsdriver
-$ python -m devopsdriver.settings --secrets
+$ settings --secrets
 secret: smtp.password  key: smtp/password
 smtp.password (smtp/password): ****
 secret: azure.token  key: azure/token
 smtp.password (azure/token): ****
-$ python -m devopsdriver.settings --secrets
+$ settings --secrets
 secret: azure.token  key: azure/token
 	Value set
 secret: smtp.password  key: smtp/password
 	Value set
 $
 ```
-The first call to `devopsdriver.settings` will look for every secret and check if they are already set in the keychain.
+The first call to `settings` will look for every secret and check if they are already set in the keychain.
 For any secret that has not been set in the keychain, you will be prompted to enter the password to store.
-The second call to `devopsdriver.settings` will verify that all the values have been set in the keychain.
+The second call to `settings` will verify that all the values have been set in the keychain.
 
 ### devopsdriver.yml
 ```yaml
 azure:
     url: https://dev.azure.com/MyCompany
 
 smtp:
@@ -116,14 +126,16 @@
 <ul>
     % for story in stories:
     <li>${story.id} ${story.title}</li>
     % endfor
 </ul>
 ```
 
+This file is the template for the email body.
+
 ### new_stories.py
 ```python
 from datetime import date, timedelta
 
 from devopsdriver import Settings, Azure, send_email, Template
 from devopsdriver.azdo import Wiql, GreaterThan
```

### Comparing `devopsdriver-0.1.37/devopsdriver/azdo/clients.py` & `devopsdriver-0.1.39/devopsdriver/azdo/clients.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,20 +3,23 @@
 
 """ Establish a connection to Azure Devops 
 
 API Documented here:
 https://github.com/microsoft/azure-devops-python-api
 """
 
+
 from azure.devops.connection import Connection as AzureConnection
 from msrest.authentication import BasicAuthentication as MSBasicAuthentication
 
 from devopsdriver.settings import Settings
 from devopsdriver.azdo.workitem.client import Client as WIClient
 
+
+# for testing
 CONNECTION = AzureConnection
 AUTHENTICATION = MSBasicAuthentication
 
 
 class Azure:  # pylint: disable=too-few-public-methods
     """A connection to Azure clients"""
```

### Comparing `devopsdriver-0.1.37/devopsdriver/azdo/workitem/client.py` & `devopsdriver-0.1.39/devopsdriver/azdo/workitem/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 #!/usr/bin/env python3
 
+
 """ Azure WorkItem Client """
 
+
 from azure.devops.v7_1.work_item_tracking.models import Wiql as AzureWiql
 from azure.devops.v7_1.work_item_tracking.models import WorkItem as AzureWorkItem
 from azure.devops.v7_1.work_item_tracking.models import TeamContext
 from azure.devops.v7_1.work_item_tracking.models import WorkItemQueryResult
-from devopsdriver.azdo.workitem import WorkItem
+from devopsdriver.azdo.workitem.workitem import WorkItem
 from devopsdriver.azdo.workitem.wiql import Wiql
 
 
 class Client:
     """Wraps work item client"""
 
     def __init__(self, client):
```

### Comparing `devopsdriver-0.1.37/devopsdriver/azdo/workitem/wiql.py` & `devopsdriver-0.1.39/devopsdriver/azdo/workitem/wiql.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 #!/usr/bin/env python3
 
+
 """ Builds a WIQL query
 https://learn.microsoft.com/en-us/azure/devops/boards/queries/wiql-syntax?view=azure-devops
 
 SELECT
     [System.Id],
     [System.AssignedTo],
     [System.State],
```

### Comparing `devopsdriver-0.1.37/devopsdriver/sendmail.py` & `devopsdriver-0.1.39/devopsdriver/sendmail.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 #!/usr/bin/env python3
 
+
 """ Ability to send emails with embedded images """
+
+
 from smtplib import SMTP as OS_SMTP, SMTP_SSL as OS_SMTP_SSL
 from email.mime.multipart import MIMEMultipart as OS_MIMEMultipart
 from email.mime.text import MIMEText as OS_MIMEText
 from email.mime.image import MIMEImage as OS_MIMEImage
 
 from devopsdriver.settings import Settings
 
+
 IMAGE_HEADERS = {".png": b"\x89PNG\r\n\x1a\n", ".jpg": b"\xff\xd8\xff"}
 
 # for testing
 MIMEMULTIPART = OS_MIMEMultipart
 MIMETEXT = OS_MIMEText
 MIMEIMAGE = OS_MIMEImage
 SMTP = OS_SMTP
```

### Comparing `devopsdriver-0.1.37/devopsdriver/settings.py` & `devopsdriver-0.1.39/devopsdriver/settings.py`

 * *Files 4% similar despite different names*

```diff
@@ -82,14 +82,16 @@
 from re import compile as regex
 from platform import system as os_system
 from sys import argv as sys_argv
 from getpass import getpass as os_getpass
 
 from yaml import safe_load
 from keyring import get_password, set_password
+from keyring.backends import fail
+
 
 # for testing
 ENVIRON = os_environ
 ARGV = sys_argv
 SYSTEM = os_system
 MAKEDIRS = os_makedirs
 SHARED = "devopsdriver"
@@ -262,15 +264,15 @@
                 if e_key.lower() == self.environ[key].lower():
                     return True if check else ENVIRON[e_key]
 
         # Settings in the keychain are next
         if key in self.secrets:
             value = GET_PASSWORD(*Settings.split_key(self.secrets[key]))
 
-            if value is not None:
+            if value is not None and not isinstance(value, fail.Keyring):
                 return True if check else value
 
         # Last check the files for settings
         keys = key.split(".")
         level = self.settings
 
         for key_part in keys[:-1]:
@@ -353,42 +355,7 @@
         settings = {}
 
         for extension, name, directory, loader in search_info:
             contents = loader(join(directory, name + extension))
             Settings.__merge(settings, contents)
 
         return settings
-
-
-def main() -> None:
-    """Get settings values"""
-    args = list(ARGV[1:])
-
-    if not args or "--help" in args or "-h" in args:
-        PRINT("pass in settings to see if they are set and to what value")
-        PRINT("You can pass dotted names to get inner values, like smpt.server")
-        PRINT("You can pass --secrets to set keychain values that have not been set")
-        PRINT("You can also pass --help or -h to get this message")
-        return
-
-    settings = Settings(__file__, dirname(dirname(__file__))).key("secrets")
-
-    if "--secrets" in args:
-        args.remove("--secrets")
-
-        for secret, key in settings.secrets.items():
-            PRINT(f"secret: {secret}  key: {key}")
-
-            if not settings.has(secret):
-                value = GET_PASS(f"{secret} ({key}): ")
-
-                if value:
-                    SET_PASSWORD(*Settings.split_key(key), value)
-            else:
-                PRINT("\tValue set")
-
-    for arg in args:
-        PRINT(f"{settings.get(arg)}")
-
-
-if __name__ == "__main__":
-    main()
```

### Comparing `devopsdriver-0.1.37/devopsdriver/template.py` & `devopsdriver-0.1.39/devopsdriver/template.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 #!/usr/bin/env python3
 
+
 """ Module Doc """
 
+
 from os.path import dirname, basename, splitext
 
 from mako.lookup import TemplateLookup
 
 
 class Template:  # pylint: disable=too-few-public-methods
     """render template files"""
```

### Comparing `devopsdriver-0.1.37/devopsdriver.egg-info/PKG-INFO` & `devopsdriver-0.1.39/devopsdriver.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: devopsdriver
-Version: 0.1.37
+Version: 0.1.39
 Summary: DevOps tools
 Author-email: Marc Page <marcallenpage@gmail.com>
 License: This is free and unencumbered software released into the public domain.
         
         Anyone is free to copy, modify, publish, use, compile, sell, or
         distribute this software, either in source code form or as a compiled
         binary, for any purpose, commercial or non-commercial, and by any
@@ -47,17 +47,24 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: PyYAML==6.0.1
 Requires-Dist: keyring==25.0.0
 Requires-Dist: setuptools==69.0.2
 Requires-Dist: azure-devops==7.1.0b4
 Requires-Dist: Mako==1.3.2
+Provides-Extra: dev
+Requires-Dist: black>=24.3.0; extra == "dev"
+Requires-Dist: pylint>=3.1.0; extra == "dev"
+Provides-Extra: test
+Requires-Dist: pytest>=8.1.1; extra == "test"
+Requires-Dist: coverage>=7.4.4; extra == "test"
+Provides-Extra: doc
 
 ![status sheild](https://img.shields.io/static/v1?label=status&message=beta&color=blue&style=plastic)
-[![status sheild](https://img.shields.io/static/v1?label=released&message=v0.1.37&color=active&style=plastic)](https://pypi.org/project/devopsdriver/0.1.37/)
+[![status sheild](https://img.shields.io/static/v1?label=released&message=v0.1.39&color=active&style=plastic)](https://pypi.org/project/devopsdriver/0.1.39/)
 [![GitHub](https://img.shields.io/github/license/marcpage/devops-driver?style=plastic)](https://github.com/marcpage/devops-driver?tab=Unlicense-1-ov-file#readme)
 [![GitHub contributors](https://img.shields.io/github/contributors/marcpage/devops-driver?style=flat)](https://github.com/marcpage/devops-driver/graphs/contributors)
 [![PR's Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat)](http://makeapullrequest.com)
 
 [![commit sheild](https://img.shields.io/github/last-commit/marcpage/devops-driver?style=plastic)](https://github.com/marcpage/devops-driver/commits)
 [![activity sheild](https://img.shields.io/github/commit-activity/m/marcpage/devops-driver?style=plastic)](https://github.com/marcpage/devops-driver/commits)
 [![GitHub top language](https://img.shields.io/github/languages/top/marcpage/devops-driver?style=plastic)](https://github.com/marcpage/devops-driver)
@@ -80,15 +87,24 @@
 [![macOS](https://img.shields.io/static/v1?label=&message=macOS&color=white&logoColor=black&style=plastic&logo=apple)](https://apple.com/)
 [![Linux](https://img.shields.io/static/v1?label=&message=Linux&color=seashell&logoColor=black&style=plastic&logo=linux)](https://linux.org/)
 
 # devops-driver
 
 Devops-driver is a collection of tools to help streamline developer's experience and gain insights into various processes.
 
-## Access to secrets
+## Tools
+
+devopsdriver is a toolbox that helps to quickly put together reports. Some of the items in the toolbox are:
+
+- **Settings**: store data, constants, settings, keys, tokens, etc. both in and out of the repository
+- **send_email**: send emails over SMTP (including SSL), using `Settings` to store credentials
+- **Template**: Simplify generating reports using `.mako` templates
+- **Azure.workitem**: Search for and inspect Azure DevOps work items
+
+## Example use-case
 
 To allow seamless work in both pipelines as well as in the development environment, the `Settings` object gives you access to common settings among multiple scripts, secrets, and configuration constants in a way the helps keep secrets out of the repository but runs just as well in the pipeline as your machine.
 
 Say you want a pipeline that looks for User Stories that are newer than 3 days and send out an email.
 
 ### \<platform dependent path\>/devopsdriver.yml
 ```yaml
@@ -97,42 +113,43 @@
 
 secrets:
     azure.token: azure/token
     smtp.password: smtp/password
 ```
 
 This file is in a global place (location varies by OS) and stores information that you may not want in your repository or is specific to development. 
-The `secrets` are extra sensative and are stored in the OS keychain.
 
 | Platform | Global Directory       |
 |----------|------------------------|
 | Windows  | %APPDATA%\             |
 | Linux    | ~/.devopsdriver/       |
 | macOS    | ~/Library/Preferences/ |
 
+The `secrets` are extra sensative and are stored in the OS keychain.
+
 ### Set secrets in the keychain
 ```bash
 $ python3 -m venv .venv
 $ source .venv/bin/activate
 $ pip install devopsdriver
-$ python -m devopsdriver.settings --secrets
+$ settings --secrets
 secret: smtp.password  key: smtp/password
 smtp.password (smtp/password): ****
 secret: azure.token  key: azure/token
 smtp.password (azure/token): ****
-$ python -m devopsdriver.settings --secrets
+$ settings --secrets
 secret: azure.token  key: azure/token
 	Value set
 secret: smtp.password  key: smtp/password
 	Value set
 $
 ```
-The first call to `devopsdriver.settings` will look for every secret and check if they are already set in the keychain.
+The first call to `settings` will look for every secret and check if they are already set in the keychain.
 For any secret that has not been set in the keychain, you will be prompted to enter the password to store.
-The second call to `devopsdriver.settings` will verify that all the values have been set in the keychain.
+The second call to `settings` will verify that all the values have been set in the keychain.
 
 ### devopsdriver.yml
 ```yaml
 azure:
     url: https://dev.azure.com/MyCompany
 
 smtp:
@@ -170,14 +187,16 @@
 <ul>
     % for story in stories:
     <li>${story.id} ${story.title}</li>
     % endfor
 </ul>
 ```
 
+This file is the template for the email body.
+
 ### new_stories.py
 ```python
 from datetime import date, timedelta
 
 from devopsdriver import Settings, Azure, send_email, Template
 from devopsdriver.azdo import Wiql, GreaterThan
```

### Comparing `devopsdriver-0.1.37/devopsdriver.egg-info/SOURCES.txt` & `devopsdriver-0.1.39/devopsdriver.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,31 @@
 LICENSE
 README.md
 pyproject.toml
 devopsdriver/__init__.py
+devopsdriver/manage_settings.py
 devopsdriver/sendmail.py
 devopsdriver/settings.py
 devopsdriver/template.py
 devopsdriver.egg-info/PKG-INFO
 devopsdriver.egg-info/SOURCES.txt
 devopsdriver.egg-info/dependency_links.txt
+devopsdriver.egg-info/entry_points.txt
 devopsdriver.egg-info/requires.txt
 devopsdriver.egg-info/top_level.txt
 devopsdriver/azdo/__init__.py
 devopsdriver/azdo/clients.py
+devopsdriver/azdo/timestamp.py
 devopsdriver/azdo/workitem/__init__.py
 devopsdriver/azdo/workitem/client.py
 devopsdriver/azdo/workitem/wiql.py
 devopsdriver/azdo/workitem/workitem.py
+devopsdriver/templates/manage_settings.txt.mako
 tests/test_azure_clients.py
+tests/test_azure_timestamp.py
 tests/test_azure_workitem.py
 tests/test_azure_workitem_client.py
 tests/test_azure_workitem_wiql.py
+tests/test_manage_settings.py
 tests/test_sendmail.py
 tests/test_settings.py
 tests/test_template.py
```

### Comparing `devopsdriver-0.1.37/pyproject.toml` & `devopsdriver-0.1.39/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -24,14 +24,31 @@
     "Topic :: Utilities",
     "Topic :: Software Development",
 ]
 authors = [
   {name = "Marc Page", email = "marcallenpage@gmail.com"},
 ]
 
+[project.scripts]
+settings = "devopsdriver.manage_settings:main"
+
+[tool.setuptools.package-data]
+"*" = ["*.mako"]
+
+[project.optional-dependencies]
+dev = [
+    "black>=24.3.0",
+    "pylint>=3.1.0",
+]
+test = [
+    "pytest>=8.1.1",
+    "coverage>=7.4.4",
+]
+doc = []
+
 [project.urls]
 Homepage = "https://github.com/marcpage/devops-driver"
 Documentation = "https://github.com/marcpage/devops-driver"
 Repository = "https://github.com/marcpage/devops-driver.git"
 Issues = "https://github.com/marcpage/devops-driver/issues"
 Changelog = "https://github.com/marcpage/devops-driver"
```

### Comparing `devopsdriver-0.1.37/tests/test_azure_clients.py` & `devopsdriver-0.1.39/tests/test_azure_clients.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 from tempfile import TemporaryDirectory
 from types import SimpleNamespace
 from os.path import join
 
 from helpers import setup_settings, write
 
-from devopsdriver import Azure
+from devopsdriver.azdo import Azure
 from devopsdriver.azdo import clients
 
 
 class MockConnection:  # pylint: disable=too-few-public-methods
     """Fakes an Azure connection"""
 
     def __init__(self, base_url: str, creds: SimpleNamespace):
```

### Comparing `devopsdriver-0.1.37/tests/test_azure_workitem.py` & `devopsdriver-0.1.39/tests/test_azure_workitem.py`

 * *Files 20% similar despite different names*

```diff
@@ -17,15 +17,15 @@
             + "_apis/wit/workItems/5/revisions/1",
             "fields": {
                 "System.WorkItemType": "User Story",
                 "System.State": "New",
                 "System.Reason": "New",
                 "System.CreatedDate": "2023-11-16T03:12:32.94Z",
                 "System.CreatedBy": {
-                    "displayName": "Edna Johnson",
+                    "displayName": "Edna Johnson Z",
                     "url": "https://spsprodcus5.vssps.visualstudio.com/"
                     + "A3eb27a26-75f2-40f9-87dc-cc10e8e565e4/_apis/Identities"
                     + "/45fcf770-0670-69d4-8e48-3ae6e0bf9b5c",
                     "_links": {
                         "avatar": {
                             "href": "https://dev.azure.com/MyOrg/_apis/GraphProfile/"
                             + "MemberAvatars/aad.NDVmY2Y3NzAtMDY3MC03OWQ0LThlNDgtM2FlNmUwYmY5YjVj"
@@ -36,15 +36,16 @@
                     "imageUrl": "https://dev.azure.com/MyOrg/_apis/GraphProfile/"
                     + "MemberAvatars/aad.NDVmY2Y3NzAtMDY3MC03OWQ0LThlNDgtM2FlNmUwYmY5YjVj",
                     "inactive": True,
                     "descriptor": "aad.NDVmY2Y3NzAtMDY3MC03OWQ0LThlNDgtM2FlNmUwYmY5YjVj",
                 },
                 "System.ChangedDate": "2023-11-16T03:12:32.94Z",
                 "System.ChangedBy": {
-                    "displayName": "Edna Johnson",
+                    "displayName": "Edna Johnson .Z",
+                    "changedOn": "2023-11-16T03:12:32.94Z",
                     "url": "https://spsprodcus5.vssps.visualstudio.com/"
                     + "A3eb27a26-75f2-40f9-87dc-cc10e8e565e4/_apis/Identities/"
                     + "45fcf770-0670-69d4-8e48-3ae6e0bf9b5c",
                     "_links": {
                         "avatar": {
                             "href": "https://dev.azure.com/MyOrg/_apis/GraphProfile/"
                             + "MemberAvatars/aad.NDVmY2Y3NzAtMDY3MC03OWQ0LThlNDgtM2FlNmUwYmY5YjVj"
@@ -56,15 +57,15 @@
                     + "MemberAvatars/aad.NDVmY2Y3NzAtMDY3MC03OWQ0LThlNDgtM2FlNmUwYmY5YjVj",
                     "inactive": True,
                     "descriptor": "aad.NDVmY2Y3NzAtMDY3MC03OWQ0LThlNDgtM2FlNmUwYmY5YjVj",
                 },
                 "System.CommentCount": 0,
                 "System.TeamProject": "Creative",
                 "System.AreaPath": "Creative",
-                "System.IterationPath": "Creative\\November 2 2023",
+                "System.IterationPath": "2023-11-16T03:12:32.alphaZ",
                 "System.Title": "test",
                 "Microsoft.VSTS.Common.Priority": 2,
                 "Microsoft.VSTS.Common.ValueArea": "Business",
                 "WEF_FBFB2B85F9CD4A7C9AA907EBB29D5863_Kanban.Column": "To Do",
                 "WEF_FBFB2B85F9CD4A7C9AA907EBB29D5863_Kanban.Column.Done": False,
                 "System.BoardColumn": "To Do",
                 "System.BoardColumnDone": False,
@@ -76,20 +77,28 @@
 def test_workitem() -> None:
     """test basic work item"""
     wi = WorkItem(MockAzureWorkItem())
     assert wi.id == 5, wi.id
     assert wi.ID == 5, wi.ID
     assert wi.workitemtype == "User Story", wi.workitemtype
     assert wi.system_workitemtype == "User Story", wi.system_workitemtype
-    assert wi.ChangedBy["displayName"] == "Edna Johnson", wi.changedBy
-    assert wi.changedby.displayname == "Edna Johnson", wi.changedby.displayname
     assert wi.microsoft_vsts_common_priority == 2, wi.microsoft_vsts_common_priority
+    assert wi.not_a_field is None, wi.not_a_field
 
-    try:
-        _ = wi.not_a_field
 
-    except AttributeError as error:
-        assert "not_a_field" in str(error)
+def test_timestamp() -> None:
+    """test timestamps"""
+    wi = WorkItem(MockAzureWorkItem())
+    assert wi.StateChangeDate.to_string() == "2023-11-16T03:12:32.94Z"
+    assert wi.CreatedDate.to_string() == "2023-11-16T03:12:32.94Z"
+    assert wi.ChangedDate.to_string() == "2023-11-16T03:12:32.94Z"
+    assert wi.IterationPath == "2023-11-16T03:12:32.alphaZ", wi.IterationPath
+    assert wi.ChangedBy["displayName"] == "Edna Johnson .Z", wi.changedBy["displayName"]
+    assert wi.createdBy.displayName == "Edna Johnson Z", wi.createdBy.displayName
+    assert (
+        wi.changedBy.changedOn.to_string() == "2023-11-16T03:12:32.94Z"
+    ), wi.changedBy.changedOn
 
 
 if __name__ == "__main__":
+    test_timestamp()
     test_workitem()
```

### Comparing `devopsdriver-0.1.37/tests/test_azure_workitem_client.py` & `devopsdriver-0.1.39/tests/test_azure_workitem_client.py`

 * *Files identical despite different names*

### Comparing `devopsdriver-0.1.37/tests/test_azure_workitem_wiql.py` & `devopsdriver-0.1.39/tests/test_azure_workitem_wiql.py`

 * *Files identical despite different names*

### Comparing `devopsdriver-0.1.37/tests/test_sendmail.py` & `devopsdriver-0.1.39/tests/test_sendmail.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python3
 
 """ Test sendmail """
 
 from devopsdriver import sendmail  # for debugging
-from devopsdriver import send_email
+from devopsdriver.sendmail import send_email
 
 
 class MockMultipart(dict):
     """Mock mime multipart"""
 
     def __init__(self):
         self.objects = []
```

### Comparing `devopsdriver-0.1.37/tests/test_settings.py` & `devopsdriver-0.1.39/tests/test_settings.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from os.path import join
 from string import ascii_lowercase
 from itertools import product
 
 from helpers import setup_settings, ensure, write
 
 from devopsdriver import settings  # debug access
-from devopsdriver import Settings
+from devopsdriver.settings import Settings
 
 
 def __setup_files(directory: str, dir1: str, dir2: str) -> None:
     """
     Priorities:
         <dir>/main.yml a
         <dir>/main.yaml b
@@ -234,32 +234,14 @@
         }
         opts = Settings(join(base_dir, "main.py"), aa="code aa").cli("cli").env("env")
         assert opts["output"] == "sweet home/reports", opts["output"]
         assert opts["settings"] == "app data dir/settings.json", opts["settings"]
         assert opts["value"] == "testing ${noenv} for noenv", opts["value"]
 
 
-def test_main():
-    """test the main entry point"""
-    with TemporaryDirectory() as working_dir:
-        setup_settings(shared="test", Linux=join(working_dir, "Linux"))
-        settings.ARGV = ["ignore", "test"]
-        write(join(working_dir, "Linux", "test.yml"), test=3)
-        settings.main()
-
-
-def test_main_help():
-    """test the main entry point"""
-    with TemporaryDirectory() as working_dir:
-        setup_settings(shared="test", Linux=join(working_dir, "Linux"))
-        settings.ARGV = ["ignore", "--help"]
-        write(join(working_dir, "Linux", "test.yml"), test=3)
-        settings.main()
-
-
 def test_secret():
     """test os secret storage"""
     with TemporaryDirectory() as working_dir:
         base_dir = join(working_dir, "base")
         passwords = {"system": {"john": "setec astronomy"}}
         setup_settings(
             os="Linux",
@@ -270,37 +252,12 @@
         )
         settings.GET_PASSWORD = lambda s, e: passwords.get(s, {}).get(e, None)
         write(join(base_dir, "main.yml"), password="main")
         opts = Settings(join(base_dir, "main.py")).key("password", "system/john")
         assert opts["password"] == "setec astronomy", opts["password"]
 
 
-def test_main_set_secret():
-    """test the main entry point when settings keychain secrets"""
-
-    def set_password(s, n, p):
-        assert (
-            s in ("azure", "jira") and n == "token" and p == "setec astronomy"
-        ), f"{s} {n} {p}"
-
-    with TemporaryDirectory() as working_dir:
-        setup_settings(shared="test", Linux=join(working_dir, "Linux"))
-        settings.ARGV = ["ignore", "--secrets"]
-        settings.GET_PASSWORD = lambda s, n: (
-            "password" if f"{s}/{n}" == "azure/token" else None
-        )
-        settings.GET_PASS = lambda p: "setec astronomy"
-        settings.SET_PASSWORD = set_password
-        write(
-            join(working_dir, "Linux", "test.yml"),
-            secrets={"azure.token": "azure/token", "jira.token": "jira/token"},
-        )
-        settings.main()
-
-
 if __name__ == "__main__":
-    test_main_set_secret()
     test_secret()
-    test_main()
     test_environ_values()
     test_cli_env_in_yaml()
     test_basic()
```

### Comparing `devopsdriver-0.1.37/tests/test_template.py` & `devopsdriver-0.1.39/tests/test_template.py`

 * *Files identical despite different names*

