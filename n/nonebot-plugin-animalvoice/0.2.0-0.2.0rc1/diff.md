# Comparing `tmp/nonebot_plugin_animalvoice-0.2.0.tar.gz` & `tmp/nonebot_plugin_animalvoice-0.2.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_animalvoice-0.2.0.tar", max compression
+gzip compressed data, was "nonebot_plugin_animalvoice-0.2.0rc1.tar", max compression
```

## Comparing `nonebot_plugin_animalvoice-0.2.0.tar` & `nonebot_plugin_animalvoice-0.2.0rc1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    35823 2024-04-06 13:00:03.100114 nonebot_plugin_animalvoice-0.2.0/LICENSE
--rw-r--r--   0        0        0     1623 2024-04-06 13:42:17.990781 nonebot_plugin_animalvoice-0.2.0/nonebot_plugin_animalVoice/__init__.py
--rw-r--r--   0        0        0     2658 2024-04-06 13:28:58.815316 nonebot_plugin_animalvoice-0.2.0/nonebot_plugin_animalVoice/AnimalVoice/__init__.py
--rw-r--r--   0        0        0      290 2024-04-06 13:28:58.777210 nonebot_plugin_animalvoice-0.2.0/nonebot_plugin_animalVoice/AnimalVoice/converter.py
--rw-r--r--   0        0        0     2836 2024-04-06 13:35:17.555281 nonebot_plugin_animalvoice-0.2.0/nonebot_plugin_animalVoice/animalvoice_main.py
--rw-r--r--   0        0        0     1247 2024-04-06 13:28:58.800659 nonebot_plugin_animalvoice-0.2.0/nonebot_plugin_animalVoice/Cheru/__init__.py
--rw-r--r--   0        0        0     2786 2024-04-06 13:35:17.555281 nonebot_plugin_animalvoice-0.2.0/nonebot_plugin_animalVoice/cheru_main.py
--rw-r--r--   0        0        0      452 2024-04-06 13:31:08.659327 nonebot_plugin_animalvoice-0.2.0/nonebot_plugin_animalVoice/config.py
--rw-r--r--   0        0        0      421 2024-04-06 13:57:03.661347 nonebot_plugin_animalvoice-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     2525 2024-04-06 13:00:03.102760 nonebot_plugin_animalvoice-0.2.0/README.md
--rw-r--r--   0        0        0     3261 1970-01-01 00:00:00.000000 nonebot_plugin_animalvoice-0.2.0/setup.py
--rw-r--r--   0        0        0     3031 1970-01-01 00:00:00.000000 nonebot_plugin_animalvoice-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    35823 2024-04-06 13:00:03.100114 nonebot_plugin_animalvoice-0.2.0rc1/LICENSE
+-rw-r--r--   0        0        0     1623 2024-04-06 13:42:17.990781 nonebot_plugin_animalvoice-0.2.0rc1/nonebot_plugin_animalVoice/__init__.py
+-rw-r--r--   0        0        0     2658 2024-04-06 13:28:58.815316 nonebot_plugin_animalvoice-0.2.0rc1/nonebot_plugin_animalVoice/AnimalVoice/__init__.py
+-rw-r--r--   0        0        0      290 2024-04-06 13:28:58.777210 nonebot_plugin_animalvoice-0.2.0rc1/nonebot_plugin_animalVoice/AnimalVoice/converter.py
+-rw-r--r--   0        0        0     2836 2024-04-06 13:35:17.555281 nonebot_plugin_animalvoice-0.2.0rc1/nonebot_plugin_animalVoice/animalvoice_main.py
+-rw-r--r--   0        0        0     1247 2024-04-06 13:28:58.800659 nonebot_plugin_animalvoice-0.2.0rc1/nonebot_plugin_animalVoice/Cheru/__init__.py
+-rw-r--r--   0        0        0     2786 2024-04-06 13:35:17.555281 nonebot_plugin_animalvoice-0.2.0rc1/nonebot_plugin_animalVoice/cheru_main.py
+-rw-r--r--   0        0        0      452 2024-04-06 13:31:08.659327 nonebot_plugin_animalvoice-0.2.0rc1/nonebot_plugin_animalVoice/config.py
+-rw-r--r--   0        0        0      425 2024-04-06 14:03:28.476236 nonebot_plugin_animalvoice-0.2.0rc1/pyproject.toml
+-rw-r--r--   0        0        0     3014 2024-04-06 14:01:39.275950 nonebot_plugin_animalvoice-0.2.0rc1/README.md
+-rw-r--r--   0        0        0     3753 1970-01-01 00:00:00.000000 nonebot_plugin_animalvoice-0.2.0rc1/setup.py
+-rw-r--r--   0        0        0     3522 1970-01-01 00:00:00.000000 nonebot_plugin_animalvoice-0.2.0rc1/PKG-INFO
```

### Comparing `nonebot_plugin_animalvoice-0.2.0/LICENSE` & `nonebot_plugin_animalvoice-0.2.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_animalvoice-0.2.0/nonebot_plugin_animalVoice/__init__.py` & `nonebot_plugin_animalvoice-0.2.0rc1/nonebot_plugin_animalVoice/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_animalvoice-0.2.0/nonebot_plugin_animalVoice/AnimalVoice/__init__.py` & `nonebot_plugin_animalvoice-0.2.0rc1/nonebot_plugin_animalVoice/AnimalVoice/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_animalvoice-0.2.0/nonebot_plugin_animalVoice/animalvoice_main.py` & `nonebot_plugin_animalvoice-0.2.0rc1/nonebot_plugin_animalVoice/animalvoice_main.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_animalvoice-0.2.0/nonebot_plugin_animalVoice/Cheru/__init__.py` & `nonebot_plugin_animalvoice-0.2.0rc1/nonebot_plugin_animalVoice/Cheru/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_animalvoice-0.2.0/nonebot_plugin_animalVoice/cheru_main.py` & `nonebot_plugin_animalvoice-0.2.0rc1/nonebot_plugin_animalVoice/cheru_main.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_animalvoice-0.2.0/setup.py` & `nonebot_plugin_animalvoice-0.2.0rc1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,17 +10,17 @@
 {'': ['*']}
 
 install_requires = \
 ['nonebot2>=2.2.0,<3.0.0']
 
 setup_kwargs = {
     'name': 'nonebot-plugin-animalvoice',
-    'version': '0.2.0',
+    'version': '0.2.0rc1',
     'description': '✨Nonebot兽语译者插件✨',
-    'long_description': '<div align="center">\n  \n  <a href="https://v2.nonebot.dev/store"><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>\n  <br>\n  <p><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText"></p>\n\n\n# nonebot_plugin_animalVoice\n  \n_✨Nonebot兽语译者插件✨_\n\n---\n  \n<a href="./LICENSE">\n    <img src="https://img.shields.io/github/license/ANGJustinl/nonebot_plugin_animalVoice" alt="license">\n</a>\n<a href="https://pypi.python.org/pypi/nonebot_plugin_animalVoice">\n    <img src="https://img.shields.io/pypi/v/nonebot_plugin_animalVoice.svg" alt="pypi">\n</a>\n<a href="https://www.python.org">\n    <img src="https://img.shields.io/badge/python-3.7+-blue.svg" alt="python">\n</a>\n\n---  \n </div> \n  \n## ✔ 使用例\n\n![3`$HP~HVN%SK(IV@2HO7X{M](https://user-images.githubusercontent.com/96008766/210118707-b00e90ff-ce8c-4fdb-bcd9-f3a18c2ebc50.png)\n\n![OYJ5N2~Z@XZ)B6FL %MEIKA](https://user-images.githubusercontent.com/96008766/210118729-8e8a6ff0-f911-4514-aac9-a87f714051e9.png)\n  \n## 💿 安装\n\n### 1. nb-cli安装（推荐）\nbot根目录下打开命令行，执行nb命令安装插件，插件配置会自动添加至配置文件 \n \n```\nnb plugin install nonebot_plugin_animalVoice\n```\n\n### 2. pip安装\n\n```\npip install nonebot_plugin_animalVoice --upgrade\n\n```  \n\n打开 nonebot2 项目的 ```bot.py``` 文件, 在其中写入  \n```nonebot.load_plugin(\'nonebot_plugin_animalVoice\')```  \n  \n或在bot路径```pyproject.toml```的```[tool.nonebot]```的```plugins```中添加```nonebot_plugin_animalVoice```即可  \npyproject.toml配置例如： \n\n``` \n\n[tool.nonebot]\nplugin_dirs = ["src/plugins"]\nplugins = ["nonebot_plugin_animalVoice","xxxxx"]\n\n```\n\n\n## 🎉 使用\n### 指令表\n| 指令 | 需要@ | 范围 | 说明 |\n|:-----:|:----:|:----:|:----:|\n| [兽音加密]/[convert] | 否 | 群聊/私聊 | 发送需要加密的文字 |\n| [兽音解密]/[deconvert] | 否 | 群聊/私聊 | 发送需要解密的文字 |\n| [切噜一下]/[cherulize] | 否 | 群聊/私聊 | 发送需要解密的文字 |\n| [切噜～]/[decherulize] | 否 | 群聊/私聊 | 发送需要解密的文字 |\n\n\n**注意**\n\n默认情况下, 您应该在指令前加上命令前缀, 通常是 /\n\n\n### 🧡特别感谢 \n\nHoshinoBot: https://github.com/Ice-Cirno/HoshinoBot 提供了切噜切噜的算法\n',
+    'long_description': '<div align="center">\n  \n  <a href="https://v2.nonebot.dev/store"><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>\n  <br>\n  <p><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText"></p>\n\n\n# nonebot_plugin_animalVoice\n  \n_✨Nonebot兽语译者插件✨_\n\n\n  \n<a href="./LICENSE">\n    <img src="https://img.shields.io/github/license/ANGJustinl/nonebot_plugin_animalVoice" alt="license">\n</a>\n<a href="https://pypi.python.org/pypi/nonebot_plugin_animalVoice">\n    <img src="https://img.shields.io/pypi/v/nonebot_plugin_animalVoice.svg" alt="pypi">\n</a>\n<a href="https://www.python.org">\n    <img src="https://img.shields.io/badge/python-3.7+-blue.svg" alt="python">\n</a>\n<a href="https://github.com/psf/black"><img alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg"></a>\n\n </div> \n  \n## ✔ 使用例\n\n![3`$HP~HVN%SK(IV@2HO7X{M](https://user-images.githubusercontent.com/96008766/210118707-b00e90ff-ce8c-4fdb-bcd9-f3a18c2ebc50.png)\n\n![OYJ5N2~Z@XZ)B6FL %MEIKA](https://user-images.githubusercontent.com/96008766/210118729-8e8a6ff0-f911-4514-aac9-a87f714051e9.png)\n  \n## 💿 安装\n\n### 1. nb-cli安装（推荐）\nbot根目录下打开命令行，执行nb命令安装插件，插件配置会自动添加至配置文件 \n \n```\nnb plugin install nonebot_plugin_animalVoice\n```\n\n### 2. pip安装\n\n```\npip install nonebot_plugin_animalVoice --upgrade\n```  \n\n打开 nonebot2 项目的 ```bot.py``` 文件, 在其中写入  \n```nonebot.load_plugin(\'nonebot_plugin_animalVoice\')```  \n\n或在bot路径```pyproject.toml```的```[tool.nonebot]```的```plugins```中添加```nonebot_plugin_animalVoice```即可  \npyproject.toml配置例如： \n``` \n[tool.nonebot]\nplugin_dirs = ["src/plugins"]\nplugins = ["nonebot_plugin_animalVoice","xxxxx"]\n```\n\n## 🎉 使用\n### 指令表\n| 指令 | 需要@ | 范围 | 说明 |\n|:-----:|:----:|:----:|:----:|\n| [兽音加密]/[convert] | 否 | 群聊/私聊 | 发送需要加密的文字 |\n| [兽音解密]/[deconvert] | 否 | 群聊/私聊 | 发送需要解密的文字 |\n| [切噜一下]/[cherulize] | 否 | 群聊/私聊 | 发送需要解密的文字 |\n| [切噜～]/[decherulize] | 否 | 群聊/私聊 | 发送需要解密的文字 |\n\n**注意**\n默认情况下, 您应该在指令前加上命令前缀, 通常是 /\n\n## 🛠 配置项\n\n| 配置项 | 类型 | 说明 |\n|:-----:|:----:|:----:|\n| customize_cmd_animalconvert | str | 自定义触发兽音加密命令 |\n| customize_cmd_animaldeconvert | str | 自定义触发兽音解密命令 |\n| customize_cmd_cherulizing | str | 自定义触发切噜一下命令 |\n| customize_cmd_decherulizing | str | 自定义触发切噜～命令 |\n\n### 🧡特别感谢 \n\nHoshinoBot: https://github.com/Ice-Cirno/HoshinoBot 提供了切噜切噜的算法\n',
     'author': 'angjustinl',
     'author_email': 'angjustin@163.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

#### html2text {}

```diff
@@ -1,39 +1,43 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \
 ['nonebot_plugin_animalvoice', 'nonebot_plugin_animalvoice.AnimalVoice',
 'nonebot_plugin_animalvoice.Cheru'] package_data = \ {'': ['*']}
 install_requires = \ ['nonebot2>=2.2.0,<3.0.0'] setup_kwargs = { 'name':
-'nonebot-plugin-animalvoice', 'version': '0.2.0', 'description':
+'nonebot-plugin-animalvoice', 'version': '0.2.0rc1', 'description':
 'â¨Nonebotå½è¯­è¯èæä»¶â¨', 'long_description': '
                          \n \n _[_N_o_n_e_B_o_t_P_l_u_g_i_n_L_o_g_o_]\n
                                       \n
                               [NoneBotPluginText]
-\n\n\n# nonebot_plugin_animalVoice\n \n_â¨Nonebotå½è¯­è¯èæä»¶â¨_\n\n---
-           \n \n_\_n_ _[_l_i_c_e_n_s_e_]_\_n\n_\_n_ _[_p_y_p_i_]_\_n\n_\_n_ _[_p_y_t_h_o_n_]_\_n\n\n--- \n
+\n\n\n# nonebot_plugin_animalVoice\n \n_â¨Nonebotå½è¯­è¯èæä»¶â¨_\n\n\n
+     \n_\_n_ _[_l_i_c_e_n_s_e_]_\_n\n_\_n_ _[_p_y_p_i_]_\_n\n_\_n_ _[_p_y_t_h_o_n_]_\_n\n_[_C_o_d_e_ _s_t_y_l_e_:_ _b_l_a_c_k_]\n\n
 \n \n## â ä½¿ç¨ä¾\n\n![3`$HP~HVN%SK(IV@2HO7X{M](https://user-
 images.githubusercontent.com/96008766/210118707-b00e90ff-ce8c-4fdb-bcd9-
 f3a18c2ebc50.png)\n\n![OYJ5N2~Z@XZ)B6FL %MEIKA](https://user-
 images.githubusercontent.com/96008766/210118729-8e8a6ff0-f911-4514-aac9-
 a87f714051e9.png)\n \n## ð¿ å®è£\n\n### 1. nb-
 cliå®è£ï¼æ¨èï¼\nbotæ ¹ç®å½ä¸æå¼å½ä»¤è¡ï¼æ§è¡nbå½ä»¤å®è£æä»¶ï¼æä»¶éç½®ä¼èªå¨æ·»å è³éç½®æä»¶
 \n \n```\nnb plugin install nonebot_plugin_animalVoice\n```\n\n### 2.
-pipå®è£\n\n```\npip install nonebot_plugin_animalVoice --upgrade\n\n```
+pipå®è£\n\n```\npip install nonebot_plugin_animalVoice --upgrade\n```
 \n\næå¼ nonebot2 é¡¹ç®ç ```bot.py``` æä»¶, å¨å¶ä¸­åå¥
-\n```nonebot.load_plugin(\'nonebot_plugin_animalVoice\')``` \n
-\næå¨botè·¯å¾```pyproject.toml```ç```
+\n```nonebot.load_plugin(\'nonebot_plugin_animalVoice\')```
+\n\næå¨botè·¯å¾```pyproject.toml```ç```
 [tool.nonebot]```ç```plugins```ä¸­æ·»å ```nonebot_plugin_animalVoice```å³å¯
-\npyproject.tomléç½®ä¾å¦ï¼ \n\n``` \n\n[tool.nonebot]\nplugin_dirs =
-["src/plugins"]\nplugins =
-["nonebot_plugin_animalVoice","xxxxx"]\n\n```\n\n\n## ð ä½¿ç¨\n###
-æä»¤è¡¨\n| æä»¤ | éè¦@ | èå´ | è¯´æ |\n|:-----:|:----:|:----:|:---
--:|\n| [å½é³å å¯]/[convert] | å¦ | ç¾¤è/ç§è |
+\npyproject.tomléç½®ä¾å¦ï¼ \n``` \n[tool.nonebot]\nplugin_dirs = ["src/
+plugins"]\nplugins = ["nonebot_plugin_animalVoice","xxxxx"]\n```\n\n## ð
+ä½¿ç¨\n### æä»¤è¡¨\n| æä»¤ | éè¦@ | èå´ | è¯´æ |\n|:-----:|:----:
+|:----:|:----:|\n| [å½é³å å¯]/[convert] | å¦ | ç¾¤è/ç§è |
 åééè¦å å¯çæå­ |\n| [å½é³è§£å¯]/[deconvert] | å¦ | ç¾¤è/
 ç§è | åééè¦è§£å¯çæå­ |\n| [ååä¸ä¸]/[cherulize] | å¦ |
 ç¾¤è/ç§è | åééè¦è§£å¯çæå­ |\n| [ååï½]/[decherulize] |
 å¦ | ç¾¤è/ç§è | åééè¦è§£å¯çæå­
-|\n\n\n**æ³¨æ**\n\né»è®¤æåµä¸, æ¨åºè¯¥å¨æä»¤åå ä¸å½ä»¤åç¼,
-éå¸¸æ¯ /\n\n\n### ð§¡ç¹å«æè°¢ \n\nHoshinoBot: https://github.com/Ice-
-Cirno/HoshinoBot æä¾äºååååçç®æ³\n', 'author': 'angjustinl',
-'author_email': 'angjustin@163.com', 'maintainer': 'None', 'maintainer_email':
-'None', 'url': 'None', 'packages': packages, 'package_data': package_data,
-'install_requires': install_requires, 'python_requires': '>=3.8,<4.0', } setup
-(**setup_kwargs)
+|\n\n**æ³¨æ**\né»è®¤æåµä¸, æ¨åºè¯¥å¨æä»¤åå ä¸å½ä»¤åç¼,
+éå¸¸æ¯ /\n\n## ð  éç½®é¡¹\n\n| éç½®é¡¹ | ç±»å | è¯´æ |\n|:-----:|:
+----:|:----:|\n| customize_cmd_animalconvert | str |
+èªå®ä¹è§¦åå½é³å å¯å½ä»¤ |\n| customize_cmd_animaldeconvert | str |
+èªå®ä¹è§¦åå½é³è§£å¯å½ä»¤ |\n| customize_cmd_cherulizing | str |
+èªå®ä¹è§¦åååä¸ä¸å½ä»¤ |\n| customize_cmd_decherulizing | str |
+èªå®ä¹è§¦åååï½å½ä»¤ |\n\n### ð§¡ç¹å«æè°¢ \n\nHoshinoBot: https:
+//github.com/Ice-Cirno/HoshinoBot æä¾äºååååçç®æ³\n', 'author':
+'angjustinl', 'author_email': 'angjustin@163.com', 'maintainer': 'None',
+'maintainer_email': 'None', 'url': 'None', 'packages': packages,
+'package_data': package_data, 'install_requires': install_requires,
+'python_requires': '>=3.8,<4.0', } setup(**setup_kwargs)
```

### Comparing `nonebot_plugin_animalvoice-0.2.0/PKG-INFO` & `nonebot_plugin_animalvoice-0.2.0rc1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-animalvoice
-Version: 0.2.0
+Version: 0.2.0rc1
 Summary: ✨Nonebot兽语译者插件✨
 License: GPLv3
 Author: angjustinl
 Author-email: angjustin@163.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
@@ -22,27 +22,27 @@
   <p><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText"></p>
 
 
 # nonebot_plugin_animalVoice
   
 _✨Nonebot兽语译者插件✨_
 
----
+
   
 <a href="./LICENSE">
     <img src="https://img.shields.io/github/license/ANGJustinl/nonebot_plugin_animalVoice" alt="license">
 </a>
 <a href="https://pypi.python.org/pypi/nonebot_plugin_animalVoice">
     <img src="https://img.shields.io/pypi/v/nonebot_plugin_animalVoice.svg" alt="pypi">
 </a>
 <a href="https://www.python.org">
     <img src="https://img.shields.io/badge/python-3.7+-blue.svg" alt="python">
 </a>
+<a href="https://github.com/psf/black"><img alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg"></a>
 
----  
  </div> 
   
 ## ✔ 使用例
 
 ![3`$HP~HVN%SK(IV@2HO7X{M](https://user-images.githubusercontent.com/96008766/210118707-b00e90ff-ce8c-4fdb-bcd9-f3a18c2ebc50.png)
 
 ![OYJ5N2~Z@XZ)B6FL %MEIKA](https://user-images.githubusercontent.com/96008766/210118729-8e8a6ff0-f911-4514-aac9-a87f714051e9.png)
@@ -56,44 +56,45 @@
 nb plugin install nonebot_plugin_animalVoice
 ```
 
 ### 2. pip安装
 
 ```
 pip install nonebot_plugin_animalVoice --upgrade
-
 ```  
 
 打开 nonebot2 项目的 ```bot.py``` 文件, 在其中写入  
 ```nonebot.load_plugin('nonebot_plugin_animalVoice')```  
-  
+
 或在bot路径```pyproject.toml```的```[tool.nonebot]```的```plugins```中添加```nonebot_plugin_animalVoice```即可  
 pyproject.toml配置例如： 
-
 ``` 
-
 [tool.nonebot]
 plugin_dirs = ["src/plugins"]
 plugins = ["nonebot_plugin_animalVoice","xxxxx"]
-
 ```
 
-
 ## 🎉 使用
 ### 指令表
 | 指令 | 需要@ | 范围 | 说明 |
 |:-----:|:----:|:----:|:----:|
 | [兽音加密]/[convert] | 否 | 群聊/私聊 | 发送需要加密的文字 |
 | [兽音解密]/[deconvert] | 否 | 群聊/私聊 | 发送需要解密的文字 |
 | [切噜一下]/[cherulize] | 否 | 群聊/私聊 | 发送需要解密的文字 |
 | [切噜～]/[decherulize] | 否 | 群聊/私聊 | 发送需要解密的文字 |
 
-
 **注意**
-
 默认情况下, 您应该在指令前加上命令前缀, 通常是 /
 
+## 🛠 配置项
+
+| 配置项 | 类型 | 说明 |
+|:-----:|:----:|:----:|
+| customize_cmd_animalconvert | str | 自定义触发兽音加密命令 |
+| customize_cmd_animaldeconvert | str | 自定义触发兽音解密命令 |
+| customize_cmd_cherulizing | str | 自定义触发切噜一下命令 |
+| customize_cmd_decherulizing | str | 自定义触发切噜～命令 |
 
 ### 🧡特别感谢 
 
 HoshinoBot: https://github.com/Ice-Cirno/HoshinoBot 提供了切噜切噜的算法
```

#### html2text {}

```diff
@@ -1,19 +1,19 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-animalvoice Version: 0.2.0 Summary:
-â¨Nonebotå½è¯­è¯èæä»¶â¨ License: GPLv3 Author: angjustinl Author-email:
-angjustin@163.com Requires-Python: >=3.8,<4.0 Classifier: License :: Other/
-Proprietary License Classifier: Programming Language :: Python :: 3 Classifier:
-Programming Language :: Python :: 3.8 Classifier: Programming Language ::
-Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
-Programming Language :: Python :: 3.11 Requires-Dist: nonebot2 (>=2.2.0,<3.0.0)
-Description-Content-Type: text/markdown
+Metadata-Version: 2.1 Name: nonebot-plugin-animalvoice Version: 0.2.0rc1
+Summary: â¨Nonebotå½è¯­è¯èæä»¶â¨ License: GPLv3 Author: angjustinl
+Author-email: angjustin@163.com Requires-Python: >=3.8,<4.0 Classifier: License
+:: Other/Proprietary License Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Requires-Dist: nonebot2
+(>=2.2.0,<3.0.0) Description-Content-Type: text/markdown
                               _[_N_o_n_e_B_o_t_P_l_u_g_i_n_L_o_g_o_]
                               [NoneBotPluginText]
- # nonebot_plugin_animalVoice _â¨Nonebotå½è¯­è¯èæä»¶â¨_ --- _[_l_i_c_e_n_s_e_]
-                               _[_p_y_p_i_]_[_p_y_t_h_o_n_]---
+ # nonebot_plugin_animalVoice _â¨Nonebotå½è¯­è¯èæä»¶â¨__[_l_i_c_e_n_s_e_]_[_p_y_p_i_]
+                          _[_p_y_t_h_o_n_]_[_C_o_d_e_ _s_t_y_l_e_:_ _b_l_a_c_k_]
 ## â ä½¿ç¨ä¾ ![3`$HP~HVN%SK(IV@2HO7X{M](https://user-
 images.githubusercontent.com/96008766/210118707-b00e90ff-ce8c-4fdb-bcd9-
 f3a18c2ebc50.png) ![OYJ5N2~Z@XZ)B6FL %MEIKA](https://user-
 images.githubusercontent.com/96008766/210118729-8e8a6ff0-f911-4514-aac9-
 a87f714051e9.png) ## ð¿ å®è£ ### 1. nb-cliå®è£ï¼æ¨èï¼
 botæ ¹ç®å½ä¸æå¼å½ä»¤è¡ï¼æ§è¡nbå½ä»¤å®è£æä»¶ï¼æä»¶éç½®ä¼èªå¨æ·»å è³éç½®æä»¶
 ``` nb plugin install nonebot_plugin_animalVoice ``` ### 2. pipå®è£ ``` pip
@@ -25,10 +25,15 @@
 plugins = ["nonebot_plugin_animalVoice","xxxxx"] ``` ## ð ä½¿ç¨ ###
 æä»¤è¡¨ | æä»¤ | éè¦@ | èå´ | è¯´æ | |:-----:|:----:|:----:|:----:
 | | [å½é³å å¯]/[convert] | å¦ | ç¾¤è/ç§è |
 åééè¦å å¯çæå­ | | [å½é³è§£å¯]/[deconvert] | å¦ | ç¾¤è/
 ç§è | åééè¦è§£å¯çæå­ | | [ååä¸ä¸]/[cherulize] | å¦ |
 ç¾¤è/ç§è | åééè¦è§£å¯çæå­ | | [ååï½]/[decherulize] | å¦
 | ç¾¤è/ç§è | åééè¦è§£å¯çæå­ | **æ³¨æ** é»è®¤æåµä¸,
-æ¨åºè¯¥å¨æä»¤åå ä¸å½ä»¤åç¼, éå¸¸æ¯ / ### ð§¡ç¹å«æè°¢
-HoshinoBot: https://github.com/Ice-Cirno/HoshinoBot
+æ¨åºè¯¥å¨æä»¤åå ä¸å½ä»¤åç¼, éå¸¸æ¯ / ## ð  éç½®é¡¹ |
+éç½®é¡¹ | ç±»å | è¯´æ | |:-----:|:----:|:----:| |
+customize_cmd_animalconvert | str | èªå®ä¹è§¦åå½é³å å¯å½ä»¤ | |
+customize_cmd_animaldeconvert | str | èªå®ä¹è§¦åå½é³è§£å¯å½ä»¤ | |
+customize_cmd_cherulizing | str | èªå®ä¹è§¦åååä¸ä¸å½ä»¤ | |
+customize_cmd_decherulizing | str | èªå®ä¹è§¦åååï½å½ä»¤ | ###
+ð§¡ç¹å«æè°¢ HoshinoBot: https://github.com/Ice-Cirno/HoshinoBot
 æä¾äºååååçç®æ³
```

