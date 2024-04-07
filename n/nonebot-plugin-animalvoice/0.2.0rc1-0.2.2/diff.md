# Comparing `tmp/nonebot_plugin_animalvoice-0.2.0rc1.tar.gz` & `tmp/nonebot_plugin_animalvoice-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_animalvoice-0.2.0rc1.tar", max compression
+gzip compressed data, was "nonebot_plugin_animalvoice-0.2.2.tar", max compression
```

## Comparing `nonebot_plugin_animalvoice-0.2.0rc1.tar` & `nonebot_plugin_animalvoice-0.2.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    35823 2024-04-06 13:00:03.100114 nonebot_plugin_animalvoice-0.2.0rc1/LICENSE
--rw-r--r--   0        0        0     1623 2024-04-06 13:42:17.990781 nonebot_plugin_animalvoice-0.2.0rc1/nonebot_plugin_animalVoice/__init__.py
--rw-r--r--   0        0        0     2658 2024-04-06 13:28:58.815316 nonebot_plugin_animalvoice-0.2.0rc1/nonebot_plugin_animalVoice/AnimalVoice/__init__.py
--rw-r--r--   0        0        0      290 2024-04-06 13:28:58.777210 nonebot_plugin_animalvoice-0.2.0rc1/nonebot_plugin_animalVoice/AnimalVoice/converter.py
--rw-r--r--   0        0        0     2836 2024-04-06 13:35:17.555281 nonebot_plugin_animalvoice-0.2.0rc1/nonebot_plugin_animalVoice/animalvoice_main.py
--rw-r--r--   0        0        0     1247 2024-04-06 13:28:58.800659 nonebot_plugin_animalvoice-0.2.0rc1/nonebot_plugin_animalVoice/Cheru/__init__.py
--rw-r--r--   0        0        0     2786 2024-04-06 13:35:17.555281 nonebot_plugin_animalvoice-0.2.0rc1/nonebot_plugin_animalVoice/cheru_main.py
--rw-r--r--   0        0        0      452 2024-04-06 13:31:08.659327 nonebot_plugin_animalvoice-0.2.0rc1/nonebot_plugin_animalVoice/config.py
--rw-r--r--   0        0        0      425 2024-04-06 14:03:28.476236 nonebot_plugin_animalvoice-0.2.0rc1/pyproject.toml
--rw-r--r--   0        0        0     3014 2024-04-06 14:01:39.275950 nonebot_plugin_animalvoice-0.2.0rc1/README.md
--rw-r--r--   0        0        0     3753 1970-01-01 00:00:00.000000 nonebot_plugin_animalvoice-0.2.0rc1/setup.py
--rw-r--r--   0        0        0     3522 1970-01-01 00:00:00.000000 nonebot_plugin_animalvoice-0.2.0rc1/PKG-INFO
+-rw-r--r--   0        0        0    35823 2024-04-06 13:00:03.100114 nonebot_plugin_animalvoice-0.2.2/LICENSE
+-rw-r--r--   0        0        0     1981 2024-04-07 01:57:04.741702 nonebot_plugin_animalvoice-0.2.2/nonebot_plugin_animalVoice/__init__.py
+-rw-r--r--   0        0        0     2658 2024-04-06 13:28:58.815316 nonebot_plugin_animalvoice-0.2.2/nonebot_plugin_animalVoice/AnimalVoice/__init__.py
+-rw-r--r--   0        0        0      290 2024-04-06 13:28:58.777210 nonebot_plugin_animalvoice-0.2.2/nonebot_plugin_animalVoice/AnimalVoice/converter.py
+-rw-r--r--   0        0        0     3737 2024-04-07 01:57:04.768086 nonebot_plugin_animalvoice-0.2.2/nonebot_plugin_animalVoice/animalvoice_main.py
+-rw-r--r--   0        0        0     1247 2024-04-06 13:28:58.800659 nonebot_plugin_animalvoice-0.2.2/nonebot_plugin_animalVoice/Cheru/__init__.py
+-rw-r--r--   0        0        0     2803 2024-04-07 01:40:54.805925 nonebot_plugin_animalvoice-0.2.2/nonebot_plugin_animalVoice/cheru_main.py
+-rw-r--r--   0        0        0      452 2024-04-06 13:31:08.659327 nonebot_plugin_animalvoice-0.2.2/nonebot_plugin_animalVoice/config.py
+-rw-r--r--   0        0        0      421 2024-04-07 02:00:34.197815 nonebot_plugin_animalvoice-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     3071 2024-04-07 01:56:03.833588 nonebot_plugin_animalvoice-0.2.2/README.md
+-rw-r--r--   0        0        0     3807 1970-01-01 00:00:00.000000 nonebot_plugin_animalvoice-0.2.2/setup.py
+-rw-r--r--   0        0        0     3625 1970-01-01 00:00:00.000000 nonebot_plugin_animalvoice-0.2.2/PKG-INFO
```

### Comparing `nonebot_plugin_animalvoice-0.2.0rc1/LICENSE` & `nonebot_plugin_animalvoice-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_animalvoice-0.2.0rc1/nonebot_plugin_animalVoice/__init__.py` & `nonebot_plugin_animalvoice-0.2.2/nonebot_plugin_animalVoice/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,45 +1,49 @@
 from . import animalvoice_main, cheru_main
 from nonebot.plugin import PluginMetadata
 
-from .config import Config
+from .config import plugin_config as Config
 
 Config.customize_cmd_animalconvert
 
 __plugin_meta__ = PluginMetadata(
     name="兽语译者插件",
     description="加密/解密 一句话/图片 为兽语/切噜语",
-    usage="没什么用",
+    usage="发送 /译者帮助 获取帮助",
     homepage="https://github.com/ANGJustinl/nonebot_plugin_animalVoice",
     supported_adapters={"~onebot.v11"},
     type="application",
     config=Config,
     extra={
         "menu_data": [
             {
                 "func": "兽音加密",
                 "trigger_method": "on_cmd",
                 "trigger_condition": "/" + Config.customize_cmd_animalconvert,
                 "brief_des": "将 文字/图片 加密为 兽语",
+                "detail_des": "发送命令激活后再发送要加密内容",
             },
             {
                 "func": "切噜一下加密",
                 "trigger_method": "on_cmd",
                 "trigger_condition": "/" + Config.customize_cmd_cherulizing,
                 "brief_des": "将 文字/图片 加密为 切噜语",
+                "detail_des": "发送命令激活后再发送要加密内容",
             },
             {
                 "func": "兽音解密",
                 "trigger_method": "on_cmd",
                 "trigger_condition": "/" + Config.customize_cmd_animaldeconvert,
                 "brief_des": "将 兽语 解密",
+                "detail_des": "发送命令激活后再发送要解密内容",
             },
             {
                 "func": "切噜～解密",
                 "trigger_method": "on_cmd",
                 "trigger_condition": "/" + Config.customize_cmd_decherulizing,
                 "brief_des": "将 切噜～语 解密",
+                "detail_des": "发送命令激活后再发送要解密内容",
             },
         ],
         "menu_template": "default",
     },
 )
```

### Comparing `nonebot_plugin_animalvoice-0.2.0rc1/nonebot_plugin_animalVoice/AnimalVoice/__init__.py` & `nonebot_plugin_animalvoice-0.2.2/nonebot_plugin_animalVoice/AnimalVoice/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_animalvoice-0.2.0rc1/nonebot_plugin_animalVoice/animalvoice_main.py` & `nonebot_plugin_animalvoice-0.2.2/nonebot_plugin_animalVoice/animalvoice_main.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,27 +1,32 @@
 from nonebot import on_command
 from nonebot.params import Arg
 from nonebot.adapters.onebot.v11 import MessageEvent, Message, Bot
 from nonebot.typing import T_State
 
-from .config import Config
+from .config import plugin_config as Config
 from .AnimalVoice.converter import msg_convert, msg_deconvert
 
 convert = on_command(
     Config.customize_cmd_animalconvert,
     aliases={"animalvoice", "convert"},
     priority=5,
     block=True,
 )
 deconvert = on_command(
     Config.customize_cmd_animaldeconvert,
     aliases={"deanimalvoice", "deconvert"},
     priority=5,
     block=True,
 )
+help = on_command(
+    "译者帮助",
+    priority=5,
+    block=True,
+)
 if_at_sender = Config.at_sender
 
 
 @convert.handle()
 async def _(state: T_State):
     return
 
@@ -91,7 +96,32 @@
                 "uin": bot.self_id,
                 "content": "解密结果\n{}".format(msg),
             },
         }
     )
     await bot.call_api("send_group_forward_msg", group_id=event.group_id, messages=msgs)
     await deconvert.finish()
+
+
+@help.handle()
+async def _(bot: Bot, event: MessageEvent):
+    msgs = []
+    msgs.append(
+        {
+            "type": "node",
+            "data": {
+                "name": "译者bot",
+                "uin": bot.self_id,
+                "content": "指令如下"
+                + "\n兽音加密 /"
+                + Config.customize_cmd_animalconvert
+                + "\n兽音解密 /"
+                + Config.customize_cmd_animaldeconvert
+                + "\n切噜一下加密 /"
+                + Config.customize_cmd_cherulizing
+                + "\n切噜～解密 /"
+                + Config.customize_cmd_decherulizing,
+            },
+        }
+    )
+    await bot.call_api("send_group_forward_msg", group_id=event.group_id, messages=msgs)
+    await help.finish()
```

### Comparing `nonebot_plugin_animalvoice-0.2.0rc1/nonebot_plugin_animalVoice/Cheru/__init__.py` & `nonebot_plugin_animalvoice-0.2.2/nonebot_plugin_animalVoice/Cheru/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_animalvoice-0.2.0rc1/nonebot_plugin_animalVoice/cheru_main.py` & `nonebot_plugin_animalvoice-0.2.2/nonebot_plugin_animalVoice/cheru_main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from nonebot import on_command
 from nonebot.params import Arg
 from nonebot.adapters.onebot.v11 import MessageEvent, Message, Bot
 from nonebot.typing import T_State
 
-from .config import Config
+from .config import plugin_config as Config
 from .Cheru import cheru2str, str2cheru
 
 cherulizing = on_command(
     Config.customize_cmd_cherulizing, aliases={"cherulize"}, priority=5, block=True
 )
 decherulizing = on_command(
     Config.customize_cmd_decherulizing, aliases={"decherulize"}, priority=5, block=True
```

### Comparing `nonebot_plugin_animalvoice-0.2.0rc1/README.md` & `nonebot_plugin_animalvoice-0.2.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -60,14 +60,15 @@
 ### 指令表
 | 指令 | 需要@ | 范围 | 说明 |
 |:-----:|:----:|:----:|:----:|
 | [兽音加密]/[convert] | 否 | 群聊/私聊 | 发送需要加密的文字 |
 | [兽音解密]/[deconvert] | 否 | 群聊/私聊 | 发送需要解密的文字 |
 | [切噜一下]/[cherulize] | 否 | 群聊/私聊 | 发送需要解密的文字 |
 | [切噜～]/[decherulize] | 否 | 群聊/私聊 | 发送需要解密的文字 |
+| [译者帮助] | 否 | 群聊/私聊 | 发送帮助 |
 
 **注意**
 默认情况下, 您应该在指令前加上命令前缀, 通常是 /
 
 ## 🛠 配置项
 
 | 配置项 | 类型 | 说明 |
```

#### html2text {}

```diff
@@ -16,15 +16,16 @@
 pyproject.tomléç½®ä¾å¦ï¼ ``` [tool.nonebot] plugin_dirs = ["src/plugins"]
 plugins = ["nonebot_plugin_animalVoice","xxxxx"] ``` ## ð ä½¿ç¨ ###
 æä»¤è¡¨ | æä»¤ | éè¦@ | èå´ | è¯´æ | |:-----:|:----:|:----:|:----:
 | | [å½é³å å¯]/[convert] | å¦ | ç¾¤è/ç§è |
 åééè¦å å¯çæå­ | | [å½é³è§£å¯]/[deconvert] | å¦ | ç¾¤è/
 ç§è | åééè¦è§£å¯çæå­ | | [ååä¸ä¸]/[cherulize] | å¦ |
 ç¾¤è/ç§è | åééè¦è§£å¯çæå­ | | [ååï½]/[decherulize] | å¦
-| ç¾¤è/ç§è | åééè¦è§£å¯çæå­ | **æ³¨æ** é»è®¤æåµä¸,
+| ç¾¤è/ç§è | åééè¦è§£å¯çæå­ | | [è¯èå¸®å©] | å¦ |
+ç¾¤è/ç§è | åéå¸®å© | **æ³¨æ** é»è®¤æåµä¸,
 æ¨åºè¯¥å¨æä»¤åå ä¸å½ä»¤åç¼, éå¸¸æ¯ / ## ð  éç½®é¡¹ |
 éç½®é¡¹ | ç±»å | è¯´æ | |:-----:|:----:|:----:| |
 customize_cmd_animalconvert | str | èªå®ä¹è§¦åå½é³å å¯å½ä»¤ | |
 customize_cmd_animaldeconvert | str | èªå®ä¹è§¦åå½é³è§£å¯å½ä»¤ | |
 customize_cmd_cherulizing | str | èªå®ä¹è§¦åååä¸ä¸å½ä»¤ | |
 customize_cmd_decherulizing | str | èªå®ä¹è§¦åååï½å½ä»¤ | ###
 ð§¡ç¹å«æè°¢ HoshinoBot: https://github.com/Ice-Cirno/HoshinoBot
```

### Comparing `nonebot_plugin_animalvoice-0.2.0rc1/setup.py` & `nonebot_plugin_animalvoice-0.2.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,23 +10,23 @@
 {'': ['*']}
 
 install_requires = \
 ['nonebot2>=2.2.0,<3.0.0']
 
 setup_kwargs = {
     'name': 'nonebot-plugin-animalvoice',
-    'version': '0.2.0rc1',
+    'version': '0.2.2',
     'description': '✨Nonebot兽语译者插件✨',
-    'long_description': '<div align="center">\n  \n  <a href="https://v2.nonebot.dev/store"><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>\n  <br>\n  <p><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText"></p>\n\n\n# nonebot_plugin_animalVoice\n  \n_✨Nonebot兽语译者插件✨_\n\n\n  \n<a href="./LICENSE">\n    <img src="https://img.shields.io/github/license/ANGJustinl/nonebot_plugin_animalVoice" alt="license">\n</a>\n<a href="https://pypi.python.org/pypi/nonebot_plugin_animalVoice">\n    <img src="https://img.shields.io/pypi/v/nonebot_plugin_animalVoice.svg" alt="pypi">\n</a>\n<a href="https://www.python.org">\n    <img src="https://img.shields.io/badge/python-3.7+-blue.svg" alt="python">\n</a>\n<a href="https://github.com/psf/black"><img alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg"></a>\n\n </div> \n  \n## ✔ 使用例\n\n![3`$HP~HVN%SK(IV@2HO7X{M](https://user-images.githubusercontent.com/96008766/210118707-b00e90ff-ce8c-4fdb-bcd9-f3a18c2ebc50.png)\n\n![OYJ5N2~Z@XZ)B6FL %MEIKA](https://user-images.githubusercontent.com/96008766/210118729-8e8a6ff0-f911-4514-aac9-a87f714051e9.png)\n  \n## 💿 安装\n\n### 1. nb-cli安装（推荐）\nbot根目录下打开命令行，执行nb命令安装插件，插件配置会自动添加至配置文件 \n \n```\nnb plugin install nonebot_plugin_animalVoice\n```\n\n### 2. pip安装\n\n```\npip install nonebot_plugin_animalVoice --upgrade\n```  \n\n打开 nonebot2 项目的 ```bot.py``` 文件, 在其中写入  \n```nonebot.load_plugin(\'nonebot_plugin_animalVoice\')```  \n\n或在bot路径```pyproject.toml```的```[tool.nonebot]```的```plugins```中添加```nonebot_plugin_animalVoice```即可  \npyproject.toml配置例如： \n``` \n[tool.nonebot]\nplugin_dirs = ["src/plugins"]\nplugins = ["nonebot_plugin_animalVoice","xxxxx"]\n```\n\n## 🎉 使用\n### 指令表\n| 指令 | 需要@ | 范围 | 说明 |\n|:-----:|:----:|:----:|:----:|\n| [兽音加密]/[convert] | 否 | 群聊/私聊 | 发送需要加密的文字 |\n| [兽音解密]/[deconvert] | 否 | 群聊/私聊 | 发送需要解密的文字 |\n| [切噜一下]/[cherulize] | 否 | 群聊/私聊 | 发送需要解密的文字 |\n| [切噜～]/[decherulize] | 否 | 群聊/私聊 | 发送需要解密的文字 |\n\n**注意**\n默认情况下, 您应该在指令前加上命令前缀, 通常是 /\n\n## 🛠 配置项\n\n| 配置项 | 类型 | 说明 |\n|:-----:|:----:|:----:|\n| customize_cmd_animalconvert | str | 自定义触发兽音加密命令 |\n| customize_cmd_animaldeconvert | str | 自定义触发兽音解密命令 |\n| customize_cmd_cherulizing | str | 自定义触发切噜一下命令 |\n| customize_cmd_decherulizing | str | 自定义触发切噜～命令 |\n\n### 🧡特别感谢 \n\nHoshinoBot: https://github.com/Ice-Cirno/HoshinoBot 提供了切噜切噜的算法\n',
+    'long_description': '<div align="center">\n  \n  <a href="https://v2.nonebot.dev/store"><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>\n  <br>\n  <p><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText"></p>\n\n\n# nonebot_plugin_animalVoice\n  \n_✨Nonebot兽语译者插件✨_\n\n\n  \n<a href="./LICENSE">\n    <img src="https://img.shields.io/github/license/ANGJustinl/nonebot_plugin_animalVoice" alt="license">\n</a>\n<a href="https://pypi.python.org/pypi/nonebot_plugin_animalVoice">\n    <img src="https://img.shields.io/pypi/v/nonebot_plugin_animalVoice.svg" alt="pypi">\n</a>\n<a href="https://www.python.org">\n    <img src="https://img.shields.io/badge/python-3.7+-blue.svg" alt="python">\n</a>\n<a href="https://github.com/psf/black"><img alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg"></a>\n\n </div> \n  \n## ✔ 使用例\n\n![3`$HP~HVN%SK(IV@2HO7X{M](https://user-images.githubusercontent.com/96008766/210118707-b00e90ff-ce8c-4fdb-bcd9-f3a18c2ebc50.png)\n\n![OYJ5N2~Z@XZ)B6FL %MEIKA](https://user-images.githubusercontent.com/96008766/210118729-8e8a6ff0-f911-4514-aac9-a87f714051e9.png)\n  \n## 💿 安装\n\n### 1. nb-cli安装（推荐）\nbot根目录下打开命令行，执行nb命令安装插件，插件配置会自动添加至配置文件 \n \n```\nnb plugin install nonebot_plugin_animalVoice\n```\n\n### 2. pip安装\n\n```\npip install nonebot_plugin_animalVoice --upgrade\n```  \n\n打开 nonebot2 项目的 ```bot.py``` 文件, 在其中写入  \n```nonebot.load_plugin(\'nonebot_plugin_animalVoice\')```  \n\n或在bot路径```pyproject.toml```的```[tool.nonebot]```的```plugins```中添加```nonebot_plugin_animalVoice```即可  \npyproject.toml配置例如： \n``` \n[tool.nonebot]\nplugin_dirs = ["src/plugins"]\nplugins = ["nonebot_plugin_animalVoice","xxxxx"]\n```\n\n## 🎉 使用\n### 指令表\n| 指令 | 需要@ | 范围 | 说明 |\n|:-----:|:----:|:----:|:----:|\n| [兽音加密]/[convert] | 否 | 群聊/私聊 | 发送需要加密的文字 |\n| [兽音解密]/[deconvert] | 否 | 群聊/私聊 | 发送需要解密的文字 |\n| [切噜一下]/[cherulize] | 否 | 群聊/私聊 | 发送需要解密的文字 |\n| [切噜～]/[decherulize] | 否 | 群聊/私聊 | 发送需要解密的文字 |\n| [译者帮助] | 否 | 群聊/私聊 | 发送帮助 |\n\n**注意**\n默认情况下, 您应该在指令前加上命令前缀, 通常是 /\n\n## 🛠 配置项\n\n| 配置项 | 类型 | 说明 |\n|:-----:|:----:|:----:|\n| customize_cmd_animalconvert | str | 自定义触发兽音加密命令 |\n| customize_cmd_animaldeconvert | str | 自定义触发兽音解密命令 |\n| customize_cmd_cherulizing | str | 自定义触发切噜一下命令 |\n| customize_cmd_decherulizing | str | 自定义触发切噜～命令 |\n\n### 🧡特别感谢 \n\nHoshinoBot: https://github.com/Ice-Cirno/HoshinoBot 提供了切噜切噜的算法\n',
     'author': 'angjustinl',
     'author_email': 'angjustin@163.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
-    'python_requires': '>=3.8,<4.0',
+    'python_requires': '>=3.7,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \
 ['nonebot_plugin_animalvoice', 'nonebot_plugin_animalvoice.AnimalVoice',
 'nonebot_plugin_animalvoice.Cheru'] package_data = \ {'': ['*']}
 install_requires = \ ['nonebot2>=2.2.0,<3.0.0'] setup_kwargs = { 'name':
-'nonebot-plugin-animalvoice', 'version': '0.2.0rc1', 'description':
+'nonebot-plugin-animalvoice', 'version': '0.2.2', 'description':
 'â¨Nonebotå½è¯­è¯èæä»¶â¨', 'long_description': '
                          \n \n _[_N_o_n_e_B_o_t_P_l_u_g_i_n_L_o_g_o_]\n
                                       \n
                               [NoneBotPluginText]
 \n\n\n# nonebot_plugin_animalVoice\n \n_â¨Nonebotå½è¯­è¯èæä»¶â¨_\n\n\n
      \n_\_n_ _[_l_i_c_e_n_s_e_]_\_n\n_\_n_ _[_p_y_p_i_]_\_n\n_\_n_ _[_p_y_t_h_o_n_]_\_n\n_[_C_o_d_e_ _s_t_y_l_e_:_ _b_l_a_c_k_]\n\n
 \n \n## â ä½¿ç¨ä¾\n\n![3`$HP~HVN%SK(IV@2HO7X{M](https://user-
@@ -24,20 +24,20 @@
 \npyproject.tomléç½®ä¾å¦ï¼ \n``` \n[tool.nonebot]\nplugin_dirs = ["src/
 plugins"]\nplugins = ["nonebot_plugin_animalVoice","xxxxx"]\n```\n\n## ð
 ä½¿ç¨\n### æä»¤è¡¨\n| æä»¤ | éè¦@ | èå´ | è¯´æ |\n|:-----:|:----:
 |:----:|:----:|\n| [å½é³å å¯]/[convert] | å¦ | ç¾¤è/ç§è |
 åééè¦å å¯çæå­ |\n| [å½é³è§£å¯]/[deconvert] | å¦ | ç¾¤è/
 ç§è | åééè¦è§£å¯çæå­ |\n| [ååä¸ä¸]/[cherulize] | å¦ |
 ç¾¤è/ç§è | åééè¦è§£å¯çæå­ |\n| [ååï½]/[decherulize] |
-å¦ | ç¾¤è/ç§è | åééè¦è§£å¯çæå­
-|\n\n**æ³¨æ**\né»è®¤æåµä¸, æ¨åºè¯¥å¨æä»¤åå ä¸å½ä»¤åç¼,
-éå¸¸æ¯ /\n\n## ð  éç½®é¡¹\n\n| éç½®é¡¹ | ç±»å | è¯´æ |\n|:-----:|:
-----:|:----:|\n| customize_cmd_animalconvert | str |
-èªå®ä¹è§¦åå½é³å å¯å½ä»¤ |\n| customize_cmd_animaldeconvert | str |
-èªå®ä¹è§¦åå½é³è§£å¯å½ä»¤ |\n| customize_cmd_cherulizing | str |
-èªå®ä¹è§¦åååä¸ä¸å½ä»¤ |\n| customize_cmd_decherulizing | str |
-èªå®ä¹è§¦åååï½å½ä»¤ |\n\n### ð§¡ç¹å«æè°¢ \n\nHoshinoBot: https:
-//github.com/Ice-Cirno/HoshinoBot æä¾äºååååçç®æ³\n', 'author':
-'angjustinl', 'author_email': 'angjustin@163.com', 'maintainer': 'None',
-'maintainer_email': 'None', 'url': 'None', 'packages': packages,
-'package_data': package_data, 'install_requires': install_requires,
-'python_requires': '>=3.8,<4.0', } setup(**setup_kwargs)
+å¦ | ç¾¤è/ç§è | åééè¦è§£å¯çæå­ |\n| [è¯èå¸®å©] | å¦ |
+ç¾¤è/ç§è | åéå¸®å© |\n\n**æ³¨æ**\né»è®¤æåµä¸,
+æ¨åºè¯¥å¨æä»¤åå ä¸å½ä»¤åç¼, éå¸¸æ¯ /\n\n## ð  éç½®é¡¹\n\n|
+éç½®é¡¹ | ç±»å | è¯´æ |\n|:-----:|:----:|:----:|\n|
+customize_cmd_animalconvert | str | èªå®ä¹è§¦åå½é³å å¯å½ä»¤ |\n|
+customize_cmd_animaldeconvert | str | èªå®ä¹è§¦åå½é³è§£å¯å½ä»¤ |\n|
+customize_cmd_cherulizing | str | èªå®ä¹è§¦åååä¸ä¸å½ä»¤ |\n|
+customize_cmd_decherulizing | str | èªå®ä¹è§¦åååï½å½ä»¤ |\n\n###
+ð§¡ç¹å«æè°¢ \n\nHoshinoBot: https://github.com/Ice-Cirno/HoshinoBot
+æä¾äºååååçç®æ³\n', 'author': 'angjustinl', 'author_email':
+'angjustin@163.com', 'maintainer': 'None', 'maintainer_email': 'None', 'url':
+'None', 'packages': packages, 'package_data': package_data, 'install_requires':
+install_requires, 'python_requires': '>=3.7,<4.0', } setup(**setup_kwargs)
```

### Comparing `nonebot_plugin_animalvoice-0.2.0rc1/PKG-INFO` & `nonebot_plugin_animalvoice-0.2.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-animalvoice
-Version: 0.2.0rc1
+Version: 0.2.2
 Summary: ✨Nonebot兽语译者插件✨
 License: GPLv3
 Author: angjustinl
 Author-email: angjustin@163.com
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.7,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: nonebot2 (>=2.2.0,<3.0.0)
 Description-Content-Type: text/markdown
 
@@ -77,14 +78,15 @@
 ### 指令表
 | 指令 | 需要@ | 范围 | 说明 |
 |:-----:|:----:|:----:|:----:|
 | [兽音加密]/[convert] | 否 | 群聊/私聊 | 发送需要加密的文字 |
 | [兽音解密]/[deconvert] | 否 | 群聊/私聊 | 发送需要解密的文字 |
 | [切噜一下]/[cherulize] | 否 | 群聊/私聊 | 发送需要解密的文字 |
 | [切噜～]/[decherulize] | 否 | 群聊/私聊 | 发送需要解密的文字 |
+| [译者帮助] | 否 | 群聊/私聊 | 发送帮助 |
 
 **注意**
 默认情况下, 您应该在指令前加上命令前缀, 通常是 /
 
 ## 🛠 配置项
 
 | 配置项 | 类型 | 说明 |
```

#### html2text {}

```diff
@@ -1,15 +1,16 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-animalvoice Version: 0.2.0rc1
-Summary: â¨Nonebotå½è¯­è¯èæä»¶â¨ License: GPLv3 Author: angjustinl
-Author-email: angjustin@163.com Requires-Python: >=3.8,<4.0 Classifier: License
-:: Other/Proprietary License Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
-Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11 Requires-Dist: nonebot2
-(>=2.2.0,<3.0.0) Description-Content-Type: text/markdown
+Metadata-Version: 2.1 Name: nonebot-plugin-animalvoice Version: 0.2.2 Summary:
+â¨Nonebotå½è¯­è¯èæä»¶â¨ License: GPLv3 Author: angjustinl Author-email:
+angjustin@163.com Requires-Python: >=3.7,<4.0 Classifier: License :: Other/
+Proprietary License Classifier: Programming Language :: Python :: 3 Classifier:
+Programming Language :: Python :: 3.7 Classifier: Programming Language ::
+Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
+Programming Language :: Python :: 3.10 Classifier: Programming Language ::
+Python :: 3.11 Requires-Dist: nonebot2 (>=2.2.0,<3.0.0) Description-Content-
+Type: text/markdown
                               _[_N_o_n_e_B_o_t_P_l_u_g_i_n_L_o_g_o_]
                               [NoneBotPluginText]
  # nonebot_plugin_animalVoice _â¨Nonebotå½è¯­è¯èæä»¶â¨__[_l_i_c_e_n_s_e_]_[_p_y_p_i_]
                           _[_p_y_t_h_o_n_]_[_C_o_d_e_ _s_t_y_l_e_:_ _b_l_a_c_k_]
 ## â ä½¿ç¨ä¾ ![3`$HP~HVN%SK(IV@2HO7X{M](https://user-
 images.githubusercontent.com/96008766/210118707-b00e90ff-ce8c-4fdb-bcd9-
 f3a18c2ebc50.png) ![OYJ5N2~Z@XZ)B6FL %MEIKA](https://user-
@@ -24,15 +25,16 @@
 pyproject.tomléç½®ä¾å¦ï¼ ``` [tool.nonebot] plugin_dirs = ["src/plugins"]
 plugins = ["nonebot_plugin_animalVoice","xxxxx"] ``` ## ð ä½¿ç¨ ###
 æä»¤è¡¨ | æä»¤ | éè¦@ | èå´ | è¯´æ | |:-----:|:----:|:----:|:----:
 | | [å½é³å å¯]/[convert] | å¦ | ç¾¤è/ç§è |
 åééè¦å å¯çæå­ | | [å½é³è§£å¯]/[deconvert] | å¦ | ç¾¤è/
 ç§è | åééè¦è§£å¯çæå­ | | [ååä¸ä¸]/[cherulize] | å¦ |
 ç¾¤è/ç§è | åééè¦è§£å¯çæå­ | | [ååï½]/[decherulize] | å¦
-| ç¾¤è/ç§è | åééè¦è§£å¯çæå­ | **æ³¨æ** é»è®¤æåµä¸,
+| ç¾¤è/ç§è | åééè¦è§£å¯çæå­ | | [è¯èå¸®å©] | å¦ |
+ç¾¤è/ç§è | åéå¸®å© | **æ³¨æ** é»è®¤æåµä¸,
 æ¨åºè¯¥å¨æä»¤åå ä¸å½ä»¤åç¼, éå¸¸æ¯ / ## ð  éç½®é¡¹ |
 éç½®é¡¹ | ç±»å | è¯´æ | |:-----:|:----:|:----:| |
 customize_cmd_animalconvert | str | èªå®ä¹è§¦åå½é³å å¯å½ä»¤ | |
 customize_cmd_animaldeconvert | str | èªå®ä¹è§¦åå½é³è§£å¯å½ä»¤ | |
 customize_cmd_cherulizing | str | èªå®ä¹è§¦åååä¸ä¸å½ä»¤ | |
 customize_cmd_decherulizing | str | èªå®ä¹è§¦åååï½å½ä»¤ | ###
 ð§¡ç¹å«æè°¢ HoshinoBot: https://github.com/Ice-Cirno/HoshinoBot
```

