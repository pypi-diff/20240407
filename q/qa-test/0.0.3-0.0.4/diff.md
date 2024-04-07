# Comparing `tmp/qa_test-0.0.3.tar.gz` & `tmp/qa_test-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qa_test-0.0.3.tar", last modified: Sun Apr  7 10:12:27 2024, max compression
+gzip compressed data, was "qa_test-0.0.4.tar", last modified: Sun Apr  7 11:20:51 2024, max compression
```

## Comparing `qa_test-0.0.3.tar` & `qa_test-0.0.4.tar`

### file list

```diff
@@ -1,112 +1,70 @@
-drwxr-xr-x   0 tujianhong   (502) staff       (20)        0 2024-04-07 10:12:27.829890 qa_test-0.0.3/
--rw-r--r--   0 tujianhong   (502) staff       (20)     6897 2024-04-07 07:48:44.000000 qa_test-0.0.3/LICENSE
--rw-r--r--   0 tujianhong   (502) staff       (20)      222 2024-04-07 07:48:44.000000 qa_test-0.0.3/MANIFEST.in
--rw-r--r--   0 tujianhong   (502) staff       (20)      121 2024-04-07 10:12:27.829374 qa_test-0.0.3/PKG-INFO
--rw-r--r--   0 tujianhong   (502) staff       (20)     8736 2024-04-07 07:48:44.000000 qa_test-0.0.3/README.md
-drwxr-xr-x   0 tujianhong   (502) staff       (20)        0 2024-04-07 10:12:27.691504 qa_test-0.0.3/browser_qwen/
--rw-r--r--   0 tujianhong   (502) staff       (20)     1866 2024-04-07 07:48:44.000000 qa_test-0.0.3/browser_qwen/background.js
-drwxr-xr-x   0 tujianhong   (502) staff       (20)        0 2024-04-07 10:12:27.694164 qa_test-0.0.3/browser_qwen/img/
--rw-r--r--   0 tujianhong   (502) staff       (20)     2863 2024-04-07 07:48:44.000000 qa_test-0.0.3/browser_qwen/img/copy.png
--rw-r--r--   0 tujianhong   (502) staff       (20)   732731 2024-04-07 07:48:44.000000 qa_test-0.0.3/browser_qwen/img/logo.png
--rw-r--r--   0 tujianhong   (502) staff       (20)   732731 2024-04-07 07:48:44.000000 qa_test-0.0.3/browser_qwen/img/popup.png
--rw-r--r--   0 tujianhong   (502) staff       (20)      952 2024-04-07 07:48:44.000000 qa_test-0.0.3/browser_qwen/manifest.json
-drwxr-xr-x   0 tujianhong   (502) staff       (20)        0 2024-04-07 10:12:27.697322 qa_test-0.0.3/browser_qwen/src/
--rw-r--r--   0 tujianhong   (502) staff       (20)     2347 2024-04-07 07:48:44.000000 qa_test-0.0.3/browser_qwen/src/content.js
--rw-r--r--   0 tujianhong   (502) staff       (20)     2656 2024-04-07 07:48:44.000000 qa_test-0.0.3/browser_qwen/src/popup.html
--rw-r--r--   0 tujianhong   (502) staff       (20)     2458 2024-04-07 07:48:44.000000 qa_test-0.0.3/browser_qwen/src/popup.js
-drwxr-xr-x   0 tujianhong   (502) staff       (20)        0 2024-04-07 10:12:27.728257 qa_test-0.0.3/examples/
--rw-r--r--   0 tujianhong   (502) staff       (20)        0 2024-04-07 07:48:44.000000 qa_test-0.0.3/examples/__init__.py
--rw-r--r--   0 tujianhong   (502) staff       (20)     2276 2024-04-07 07:48:45.000000 qa_test-0.0.3/examples/assistant_add_custom_tool.py
--rw-r--r--   0 tujianhong   (502) staff       (20)     1213 2024-04-07 07:48:45.000000 qa_test-0.0.3/examples/assistant_angry_girlfriend.py
--rw-r--r--   0 tujianhong   (502) staff       (20)     2164 2024-04-07 07:48:45.000000 qa_test-0.0.3/examples/assistant_growing_girl.py
--rw-r--r--   0 tujianhong   (502) staff       (20)     2168 2024-04-07 07:48:45.000000 qa_test-0.0.3/examples/assistant_weather_bot.py
--rw-r--r--   0 tujianhong   (502) staff       (20)     4209 2024-04-07 07:48:45.000000 qa_test-0.0.3/examples/function_calling.py
--rw-r--r--   0 tujianhong   (502) staff       (20)     5273 2024-04-07 07:48:45.000000 qa_test-0.0.3/examples/gpt_mentions.py
--rw-r--r--   0 tujianhong   (502) staff       (20)     2263 2024-04-07 07:48:45.000000 qa_test-0.0.3/examples/group_chat_chess.py
--rw-r--r--   0 tujianhong   (502) staff       (20)    12466 2024-04-07 07:48:45.000000 qa_test-0.0.3/examples/group_chat_demo.py
--rw-r--r--   0 tujianhong   (502) staff       (20)     2722 2024-04-07 07:48:45.000000 qa_test-0.0.3/examples/llm_riddles.py
--rw-r--r--   0 tujianhong   (502) staff       (20)     2847 2024-04-07 07:48:45.000000 qa_test-0.0.3/examples/llm_vl_mix_text.py
--rw-r--r--   0 tujianhong   (502) staff       (20)     2869 2024-04-07 07:48:45.000000 qa_test-0.0.3/examples/multi_agent_router.py
--rw-r--r--   0 tujianhong   (502) staff       (20)     2303 2024-04-07 07:48:45.000000 qa_test-0.0.3/examples/react_data_analysis.py
--rw-r--r--   0 tujianhong   (502) staff       (20)     3676 2024-04-07 07:48:45.000000 qa_test-0.0.3/examples/visual_storytelling.py
-drwxr-xr-x   0 tujianhong   (502) staff       (20)        0 2024-04-07 10:12:27.731272 qa_test-0.0.3/qa_test.egg-info/
--rw-r--r--   0 tujianhong   (502) staff       (20)      121 2024-04-07 10:12:27.000000 qa_test-0.0.3/qa_test.egg-info/PKG-INFO
--rw-r--r--   0 tujianhong   (502) staff       (20)     2753 2024-04-07 10:12:27.000000 qa_test-0.0.3/qa_test.egg-info/SOURCES.txt
--rw-r--r--   0 tujianhong   (502) staff       (20)        1 2024-04-07 10:12:27.000000 qa_test-0.0.3/qa_test.egg-info/dependency_links.txt
--rw-r--r--   0 tujianhong   (502) staff       (20)      257 2024-04-07 10:12:27.000000 qa_test-0.0.3/qa_test.egg-info/requires.txt
--rw-r--r--   0 tujianhong   (502) staff       (20)       32 2024-04-07 10:12:27.000000 qa_test-0.0.3/qa_test.egg-info/top_level.txt
-drwxr-xr-x   0 tujianhong   (502) staff       (20)        0 2024-04-07 10:12:27.732493 qa_test-0.0.3/qwen_agent/
--rw-r--r--   0 tujianhong   (502) staff       (20)       46 2024-04-07 07:48:45.000000 qa_test-0.0.3/qwen_agent/__init__.py
--rw-r--r--   0 tujianhong   (502) staff       (20)     8672 2024-04-07 07:48:45.000000 qa_test-0.0.3/qwen_agent/agent.py
-drwxr-xr-x   0 tujianhong   (502) staff       (20)        0 2024-04-07 10:12:27.750483 qa_test-0.0.3/qwen_agent/agents/
--rw-r--r--   0 tujianhong   (502) staff       (20)      626 2024-04-07 07:48:45.000000 qa_test-0.0.3/qwen_agent/agents/__init__.py
--rw-r--r--   0 tujianhong   (502) staff       (20)     1598 2024-04-07 07:48:45.000000 qa_test-0.0.3/qwen_agent/agents/article_agent.py
--rw-r--r--   0 tujianhong   (502) staff       (20)     2780 2024-04-07 07:48:45.000000 qa_test-0.0.3/qwen_agent/agents/assistant.py
--rw-r--r--   0 tujianhong   (502) staff       (20)     1766 2024-04-07 07:48:45.000000 qa_test-0.0.3/qwen_agent/agents/docqa_agent.py
--rw-r--r--   0 tujianhong   (502) staff       (20)     4155 2024-04-07 07:48:45.000000 qa_test-0.0.3/qwen_agent/agents/fncall_agent.py
--rw-r--r--   0 tujianhong   (502) staff       (20)    13817 2024-04-07 07:48:45.000000 qa_test-0.0.3/qwen_agent/agents/group_chat.py
--rw-r--r--   0 tujianhong   (502) staff       (20)     3496 2024-04-07 07:48:45.000000 qa_test-0.0.3/qwen_agent/agents/group_chat_auto_router.py
--rw-r--r--   0 tujianhong   (502) staff       (20)     6592 2024-04-07 07:48:45.000000 qa_test-0.0.3/qwen_agent/agents/group_chat_creator.py
--rw-r--r--   0 tujianhong   (502) staff       (20)     7873 2024-04-07 07:48:45.000000 qa_test-0.0.3/qwen_agent/agents/react_chat.py
--rw-r--r--   0 tujianhong   (502) staff       (20)     4204 2024-04-07 07:48:45.000000 qa_test-0.0.3/qwen_agent/agents/router.py
--rw-r--r--   0 tujianhong   (502) staff       (20)      504 2024-04-07 07:48:45.000000 qa_test-0.0.3/qwen_agent/agents/user_agent.py
--rw-r--r--   0 tujianhong   (502) staff       (20)     3956 2024-04-07 07:48:45.000000 qa_test-0.0.3/qwen_agent/agents/write_from_scratch.py
-drwxr-xr-x   0 tujianhong   (502) staff       (20)        0 2024-04-07 10:12:27.759674 qa_test-0.0.3/qwen_agent/llm/
--rw-r--r--   0 tujianhong   (502) staff       (20)     1908 2024-04-07 07:48:45.000000 qa_test-0.0.3/qwen_agent/llm/__init__.py
--rw-r--r--   0 tujianhong   (502) staff       (20)    13188 2024-04-07 07:48:45.000000 qa_test-0.0.3/qwen_agent/llm/base.py
--rw-r--r--   0 tujianhong   (502) staff       (20)    13002 2024-04-07 07:48:45.000000 qa_test-0.0.3/qwen_agent/llm/function_calling.py
--rw-r--r--   0 tujianhong   (502) staff       (20)     4269 2024-04-07 07:48:45.000000 qa_test-0.0.3/qwen_agent/llm/oai.py
--rw-r--r--   0 tujianhong   (502) staff       (20)     6404 2024-04-07 07:48:45.000000 qa_test-0.0.3/qwen_agent/llm/qwen_dashscope.py
--rw-r--r--   0 tujianhong   (502) staff       (20)     3012 2024-04-07 07:48:45.000000 qa_test-0.0.3/qwen_agent/llm/qwenvl_dashscope.py
--rw-r--r--   0 tujianhong   (502) staff       (20)     3322 2024-04-07 07:48:45.000000 qa_test-0.0.3/qwen_agent/llm/schema.py
--rw-r--r--   0 tujianhong   (502) staff       (20)     1596 2024-04-07 07:48:45.000000 qa_test-0.0.3/qwen_agent/llm/text_base.py
--rw-r--r--   0 tujianhong   (502) staff       (20)      599 2024-04-07 07:48:45.000000 qa_test-0.0.3/qwen_agent/log.py
-drwxr-xr-x   0 tujianhong   (502) staff       (20)        0 2024-04-07 10:12:27.761698 qa_test-0.0.3/qwen_agent/memory/
--rw-r--r--   0 tujianhong   (502) staff       (20)       49 2024-04-07 07:48:45.000000 qa_test-0.0.3/qwen_agent/memory/__init__.py
--rw-r--r--   0 tujianhong   (502) staff       (20)     4053 2024-04-07 07:48:45.000000 qa_test-0.0.3/qwen_agent/memory/memory.py
-drwxr-xr-x   0 tujianhong   (502) staff       (20)        0 2024-04-07 10:12:27.769836 qa_test-0.0.3/qwen_agent/prompts/
--rw-r--r--   0 tujianhong   (502) staff       (20)      368 2024-04-07 07:48:45.000000 qa_test-0.0.3/qwen_agent/prompts/__init__.py
--rw-r--r--   0 tujianhong   (502) staff       (20)     1343 2024-04-07 07:48:45.000000 qa_test-0.0.3/qwen_agent/prompts/continue_writing.py
--rw-r--r--   0 tujianhong   (502) staff       (20)     1107 2024-04-07 07:48:45.000000 qa_test-0.0.3/qwen_agent/prompts/doc_qa.py
--rw-r--r--   0 tujianhong   (502) staff       (20)     2248 2024-04-07 07:48:45.000000 qa_test-0.0.3/qwen_agent/prompts/expand_writing.py
--rw-r--r--   0 tujianhong   (502) staff       (20)     3248 2024-04-07 07:48:45.000000 qa_test-0.0.3/qwen_agent/prompts/gen_keyword.py
--rw-r--r--   0 tujianhong   (502) staff       (20)     1495 2024-04-07 07:48:45.000000 qa_test-0.0.3/qwen_agent/prompts/outline_writing.py
-drwxr-xr-x   0 tujianhong   (502) staff       (20)        0 2024-04-07 10:12:27.800797 qa_test-0.0.3/qwen_agent/tools/
--rw-r--r--   0 tujianhong   (502) staff       (20)      714 2024-04-07 07:48:45.000000 qa_test-0.0.3/qwen_agent/tools/__init__.py
--rw-r--r--   0 tujianhong   (502) staff       (20)     2021 2024-04-07 07:48:45.000000 qa_test-0.0.3/qwen_agent/tools/amap_weather.py
--rw-r--r--   0 tujianhong   (502) staff       (20)     3141 2024-04-07 07:48:45.000000 qa_test-0.0.3/qwen_agent/tools/base.py
--rw-r--r--   0 tujianhong   (502) staff       (20)    12040 2024-04-07 07:48:45.000000 qa_test-0.0.3/qwen_agent/tools/code_interpreter.py
--rw-r--r--   0 tujianhong   (502) staff       (20)     5351 2024-04-07 07:48:45.000000 qa_test-0.0.3/qwen_agent/tools/doc_parser.py
--rw-r--r--   0 tujianhong   (502) staff       (20)     1123 2024-04-07 07:48:45.000000 qa_test-0.0.3/qwen_agent/tools/image_gen.py
-drwxr-xr-x   0 tujianhong   (502) staff       (20)        0 2024-04-07 10:12:27.813050 qa_test-0.0.3/qwen_agent/tools/resource/
--rw-r--r--   0 tujianhong   (502) staff       (20)  8559848 2024-04-07 07:48:45.000000 qa_test-0.0.3/qwen_agent/tools/resource/AlibabaPuHuiTi-3-45-Light.ttf
--rw-r--r--   0 tujianhong   (502) staff       (20)     1169 2024-04-07 07:48:45.000000 qa_test-0.0.3/qwen_agent/tools/resource/code_interpreter_init_kernel.py
--rw-r--r--   0 tujianhong   (502) staff       (20)      553 2024-04-07 07:48:45.000000 qa_test-0.0.3/qwen_agent/tools/resource/image_service.py
--rw-r--r--   0 tujianhong   (502) staff       (20)     3627 2024-04-07 07:48:45.000000 qa_test-0.0.3/qwen_agent/tools/retrieval.py
--rw-r--r--   0 tujianhong   (502) staff       (20)     4898 2024-04-07 07:48:45.000000 qa_test-0.0.3/qwen_agent/tools/similarity_search.py
--rw-r--r--   0 tujianhong   (502) staff       (20)     3584 2024-04-07 07:48:45.000000 qa_test-0.0.3/qwen_agent/tools/storage.py
--rw-r--r--   0 tujianhong   (502) staff       (20)     1376 2024-04-07 07:48:45.000000 qa_test-0.0.3/qwen_agent/tools/web_extractor.py
-drwxr-xr-x   0 tujianhong   (502) staff       (20)        0 2024-04-07 10:12:27.820553 qa_test-0.0.3/qwen_agent/utils/
--rw-r--r--   0 tujianhong   (502) staff       (20)        0 2024-04-07 07:48:45.000000 qa_test-0.0.3/qwen_agent/utils/__init__.py
--rw-r--r--   0 tujianhong   (502) staff       (20)     2728 2024-04-07 07:48:45.000000 qa_test-0.0.3/qwen_agent/utils/doc_parser.py
--rw-r--r--   0 tujianhong   (502) staff       (20)  2561218 2024-04-07 07:48:45.000000 qa_test-0.0.3/qwen_agent/utils/qwen.tiktoken
--rw-r--r--   0 tujianhong   (502) staff       (20)    10526 2024-04-07 07:48:45.000000 qa_test-0.0.3/qwen_agent/utils/tokenization_qwen.py
--rw-r--r--   0 tujianhong   (502) staff       (20)     9829 2024-04-07 07:48:45.000000 qa_test-0.0.3/qwen_agent/utils/utils.py
-drwxr-xr-x   0 tujianhong   (502) staff       (20)        0 2024-04-07 10:12:27.825575 qa_test-0.0.3/qwen_server/
--rw-r--r--   0 tujianhong   (502) staff       (20)        0 2024-04-07 07:48:45.000000 qa_test-0.0.3/qwen_server/__init__.py
--rw-r--r--   0 tujianhong   (502) staff       (20)      170 2024-04-07 07:48:45.000000 qa_test-0.0.3/qwen_server/add_qwen_libs.py
--rw-r--r--   0 tujianhong   (502) staff       (20)     5776 2024-04-07 08:34:30.000000 qa_test-0.0.3/qwen_server/assistant_server.py
-drwxr-xr-x   0 tujianhong   (502) staff       (20)        0 2024-04-07 10:12:27.826155 qa_test-0.0.3/qwen_server/css/
--rw-r--r--   0 tujianhong   (502) staff       (20)     2154 2024-04-07 07:48:45.000000 qa_test-0.0.3/qwen_server/css/main.css
--rw-r--r--   0 tujianhong   (502) staff       (20)     4413 2024-04-07 07:48:45.000000 qa_test-0.0.3/qwen_server/database_server.py
-drwxr-xr-x   0 tujianhong   (502) staff       (20)        0 2024-04-07 10:12:27.826575 qa_test-0.0.3/qwen_server/img/
--rw-r--r--   0 tujianhong   (502) staff       (20)   732731 2024-04-07 07:48:45.000000 qa_test-0.0.3/qwen_server/img/logo.png
-drwxr-xr-x   0 tujianhong   (502) staff       (20)        0 2024-04-07 10:12:27.829015 qa_test-0.0.3/qwen_server/js/
--rw-r--r--   0 tujianhong   (502) staff       (20)     1303 2024-04-07 07:48:45.000000 qa_test-0.0.3/qwen_server/js/main.js
--rw-r--r--   0 tujianhong   (502) staff       (20)     4151 2024-04-07 07:48:45.000000 qa_test-0.0.3/qwen_server/output_beautify.py
--rw-r--r--   0 tujianhong   (502) staff       (20)      539 2024-04-07 07:48:45.000000 qa_test-0.0.3/qwen_server/schema.py
--rw-r--r--   0 tujianhong   (502) staff       (20)      610 2024-04-07 07:48:45.000000 qa_test-0.0.3/qwen_server/server_config.json
--rw-r--r--   0 tujianhong   (502) staff       (20)     2620 2024-04-07 07:48:45.000000 qa_test-0.0.3/qwen_server/utils.py
--rw-r--r--   0 tujianhong   (502) staff       (20)    26872 2024-04-07 08:34:30.000000 qa_test-0.0.3/qwen_server/workstation_server.py
--rw-r--r--   0 tujianhong   (502) staff       (20)       38 2024-04-07 10:12:27.829952 qa_test-0.0.3/setup.cfg
--rw-r--r--   0 tujianhong   (502) staff       (20)      501 2024-04-07 10:12:21.000000 qa_test-0.0.3/setup.py
+drwxr-xr-x   0 tujianhong   (502) staff       (20)        0 2024-04-07 11:20:51.045376 qa_test-0.0.4/
+-rw-r--r--   0 tujianhong   (502) staff       (20)     6897 2024-04-07 07:48:44.000000 qa_test-0.0.4/LICENSE
+-rw-r--r--   0 tujianhong   (502) staff       (20)       85 2024-04-07 11:18:25.000000 qa_test-0.0.4/MANIFEST.in
+-rw-r--r--   0 tujianhong   (502) staff       (20)      121 2024-04-07 11:20:51.045129 qa_test-0.0.4/PKG-INFO
+-rw-r--r--   0 tujianhong   (502) staff       (20)     8736 2024-04-07 07:48:44.000000 qa_test-0.0.4/README.md
+drwxr-xr-x   0 tujianhong   (502) staff       (20)        0 2024-04-07 11:20:50.972299 qa_test-0.0.4/qa_test.egg-info/
+-rw-r--r--   0 tujianhong   (502) staff       (20)      121 2024-04-07 11:20:50.000000 qa_test-0.0.4/qa_test.egg-info/PKG-INFO
+-rw-r--r--   0 tujianhong   (502) staff       (20)     1785 2024-04-07 11:20:50.000000 qa_test-0.0.4/qa_test.egg-info/SOURCES.txt
+-rw-r--r--   0 tujianhong   (502) staff       (20)        1 2024-04-07 11:20:50.000000 qa_test-0.0.4/qa_test.egg-info/dependency_links.txt
+-rw-r--r--   0 tujianhong   (502) staff       (20)      257 2024-04-07 11:20:50.000000 qa_test-0.0.4/qa_test.egg-info/requires.txt
+-rw-r--r--   0 tujianhong   (502) staff       (20)       11 2024-04-07 11:20:50.000000 qa_test-0.0.4/qa_test.egg-info/top_level.txt
+drwxr-xr-x   0 tujianhong   (502) staff       (20)        0 2024-04-07 11:20:50.973704 qa_test-0.0.4/qwen_agent/
+-rw-r--r--   0 tujianhong   (502) staff       (20)       46 2024-04-07 07:48:45.000000 qa_test-0.0.4/qwen_agent/__init__.py
+-rw-r--r--   0 tujianhong   (502) staff       (20)     8672 2024-04-07 07:48:45.000000 qa_test-0.0.4/qwen_agent/agent.py
+drwxr-xr-x   0 tujianhong   (502) staff       (20)        0 2024-04-07 11:20:50.980236 qa_test-0.0.4/qwen_agent/agents/
+-rw-r--r--   0 tujianhong   (502) staff       (20)      626 2024-04-07 07:48:45.000000 qa_test-0.0.4/qwen_agent/agents/__init__.py
+-rw-r--r--   0 tujianhong   (502) staff       (20)     1598 2024-04-07 07:48:45.000000 qa_test-0.0.4/qwen_agent/agents/article_agent.py
+-rw-r--r--   0 tujianhong   (502) staff       (20)     2780 2024-04-07 07:48:45.000000 qa_test-0.0.4/qwen_agent/agents/assistant.py
+-rw-r--r--   0 tujianhong   (502) staff       (20)     1766 2024-04-07 07:48:45.000000 qa_test-0.0.4/qwen_agent/agents/docqa_agent.py
+-rw-r--r--   0 tujianhong   (502) staff       (20)     4155 2024-04-07 07:48:45.000000 qa_test-0.0.4/qwen_agent/agents/fncall_agent.py
+-rw-r--r--   0 tujianhong   (502) staff       (20)    13817 2024-04-07 07:48:45.000000 qa_test-0.0.4/qwen_agent/agents/group_chat.py
+-rw-r--r--   0 tujianhong   (502) staff       (20)     3496 2024-04-07 07:48:45.000000 qa_test-0.0.4/qwen_agent/agents/group_chat_auto_router.py
+-rw-r--r--   0 tujianhong   (502) staff       (20)     6592 2024-04-07 07:48:45.000000 qa_test-0.0.4/qwen_agent/agents/group_chat_creator.py
+-rw-r--r--   0 tujianhong   (502) staff       (20)     7873 2024-04-07 07:48:45.000000 qa_test-0.0.4/qwen_agent/agents/react_chat.py
+-rw-r--r--   0 tujianhong   (502) staff       (20)     4204 2024-04-07 07:48:45.000000 qa_test-0.0.4/qwen_agent/agents/router.py
+-rw-r--r--   0 tujianhong   (502) staff       (20)      504 2024-04-07 07:48:45.000000 qa_test-0.0.4/qwen_agent/agents/user_agent.py
+-rw-r--r--   0 tujianhong   (502) staff       (20)     3956 2024-04-07 07:48:45.000000 qa_test-0.0.4/qwen_agent/agents/write_from_scratch.py
+drwxr-xr-x   0 tujianhong   (502) staff       (20)        0 2024-04-07 11:20:50.984320 qa_test-0.0.4/qwen_agent/llm/
+-rw-r--r--   0 tujianhong   (502) staff       (20)     1908 2024-04-07 07:48:45.000000 qa_test-0.0.4/qwen_agent/llm/__init__.py
+-rw-r--r--   0 tujianhong   (502) staff       (20)    13188 2024-04-07 07:48:45.000000 qa_test-0.0.4/qwen_agent/llm/base.py
+-rw-r--r--   0 tujianhong   (502) staff       (20)    13002 2024-04-07 07:48:45.000000 qa_test-0.0.4/qwen_agent/llm/function_calling.py
+-rw-r--r--   0 tujianhong   (502) staff       (20)     4269 2024-04-07 07:48:45.000000 qa_test-0.0.4/qwen_agent/llm/oai.py
+-rw-r--r--   0 tujianhong   (502) staff       (20)     6404 2024-04-07 07:48:45.000000 qa_test-0.0.4/qwen_agent/llm/qwen_dashscope.py
+-rw-r--r--   0 tujianhong   (502) staff       (20)     3012 2024-04-07 07:48:45.000000 qa_test-0.0.4/qwen_agent/llm/qwenvl_dashscope.py
+-rw-r--r--   0 tujianhong   (502) staff       (20)     3322 2024-04-07 07:48:45.000000 qa_test-0.0.4/qwen_agent/llm/schema.py
+-rw-r--r--   0 tujianhong   (502) staff       (20)     1596 2024-04-07 07:48:45.000000 qa_test-0.0.4/qwen_agent/llm/text_base.py
+-rw-r--r--   0 tujianhong   (502) staff       (20)      599 2024-04-07 07:48:45.000000 qa_test-0.0.4/qwen_agent/log.py
+drwxr-xr-x   0 tujianhong   (502) staff       (20)        0 2024-04-07 11:20:50.987227 qa_test-0.0.4/qwen_agent/memory/
+-rw-r--r--   0 tujianhong   (502) staff       (20)       49 2024-04-07 07:48:45.000000 qa_test-0.0.4/qwen_agent/memory/__init__.py
+-rw-r--r--   0 tujianhong   (502) staff       (20)     4053 2024-04-07 07:48:45.000000 qa_test-0.0.4/qwen_agent/memory/memory.py
+drwxr-xr-x   0 tujianhong   (502) staff       (20)        0 2024-04-07 11:20:50.992505 qa_test-0.0.4/qwen_agent/prompts/
+-rw-r--r--   0 tujianhong   (502) staff       (20)      368 2024-04-07 07:48:45.000000 qa_test-0.0.4/qwen_agent/prompts/__init__.py
+-rw-r--r--   0 tujianhong   (502) staff       (20)     1343 2024-04-07 07:48:45.000000 qa_test-0.0.4/qwen_agent/prompts/continue_writing.py
+-rw-r--r--   0 tujianhong   (502) staff       (20)     1107 2024-04-07 07:48:45.000000 qa_test-0.0.4/qwen_agent/prompts/doc_qa.py
+-rw-r--r--   0 tujianhong   (502) staff       (20)     2248 2024-04-07 07:48:45.000000 qa_test-0.0.4/qwen_agent/prompts/expand_writing.py
+-rw-r--r--   0 tujianhong   (502) staff       (20)     3248 2024-04-07 07:48:45.000000 qa_test-0.0.4/qwen_agent/prompts/gen_keyword.py
+-rw-r--r--   0 tujianhong   (502) staff       (20)     1495 2024-04-07 07:48:45.000000 qa_test-0.0.4/qwen_agent/prompts/outline_writing.py
+drwxr-xr-x   0 tujianhong   (502) staff       (20)        0 2024-04-07 11:20:51.002464 qa_test-0.0.4/qwen_agent/tools/
+-rw-r--r--   0 tujianhong   (502) staff       (20)      714 2024-04-07 07:48:45.000000 qa_test-0.0.4/qwen_agent/tools/__init__.py
+-rw-r--r--   0 tujianhong   (502) staff       (20)     2021 2024-04-07 07:48:45.000000 qa_test-0.0.4/qwen_agent/tools/amap_weather.py
+-rw-r--r--   0 tujianhong   (502) staff       (20)     3141 2024-04-07 07:48:45.000000 qa_test-0.0.4/qwen_agent/tools/base.py
+-rw-r--r--   0 tujianhong   (502) staff       (20)    12040 2024-04-07 07:48:45.000000 qa_test-0.0.4/qwen_agent/tools/code_interpreter.py
+-rw-r--r--   0 tujianhong   (502) staff       (20)     5351 2024-04-07 07:48:45.000000 qa_test-0.0.4/qwen_agent/tools/doc_parser.py
+-rw-r--r--   0 tujianhong   (502) staff       (20)     1123 2024-04-07 07:48:45.000000 qa_test-0.0.4/qwen_agent/tools/image_gen.py
+drwxr-xr-x   0 tujianhong   (502) staff       (20)        0 2024-04-07 11:20:51.031212 qa_test-0.0.4/qwen_agent/tools/resource/
+-rw-r--r--   0 tujianhong   (502) staff       (20)  8559848 2024-04-07 07:48:45.000000 qa_test-0.0.4/qwen_agent/tools/resource/AlibabaPuHuiTi-3-45-Light.ttf
+-rw-r--r--   0 tujianhong   (502) staff       (20)     1169 2024-04-07 07:48:45.000000 qa_test-0.0.4/qwen_agent/tools/resource/code_interpreter_init_kernel.py
+-rw-r--r--   0 tujianhong   (502) staff       (20)      553 2024-04-07 07:48:45.000000 qa_test-0.0.4/qwen_agent/tools/resource/image_service.py
+-rw-r--r--   0 tujianhong   (502) staff       (20)     3627 2024-04-07 07:48:45.000000 qa_test-0.0.4/qwen_agent/tools/retrieval.py
+-rw-r--r--   0 tujianhong   (502) staff       (20)     4898 2024-04-07 07:48:45.000000 qa_test-0.0.4/qwen_agent/tools/similarity_search.py
+-rw-r--r--   0 tujianhong   (502) staff       (20)     3584 2024-04-07 07:48:45.000000 qa_test-0.0.4/qwen_agent/tools/storage.py
+-rw-r--r--   0 tujianhong   (502) staff       (20)     1376 2024-04-07 07:48:45.000000 qa_test-0.0.4/qwen_agent/tools/web_extractor.py
+drwxr-xr-x   0 tujianhong   (502) staff       (20)        0 2024-04-07 11:20:51.044485 qa_test-0.0.4/qwen_agent/utils/
+-rw-r--r--   0 tujianhong   (502) staff       (20)        0 2024-04-07 07:48:45.000000 qa_test-0.0.4/qwen_agent/utils/__init__.py
+-rw-r--r--   0 tujianhong   (502) staff       (20)     2728 2024-04-07 07:48:45.000000 qa_test-0.0.4/qwen_agent/utils/doc_parser.py
+-rw-r--r--   0 tujianhong   (502) staff       (20)  2561218 2024-04-07 07:48:45.000000 qa_test-0.0.4/qwen_agent/utils/qwen.tiktoken
+-rw-r--r--   0 tujianhong   (502) staff       (20)    10526 2024-04-07 07:48:45.000000 qa_test-0.0.4/qwen_agent/utils/tokenization_qwen.py
+-rw-r--r--   0 tujianhong   (502) staff       (20)     9829 2024-04-07 07:48:45.000000 qa_test-0.0.4/qwen_agent/utils/utils.py
+-rw-r--r--   0 tujianhong   (502) staff       (20)       38 2024-04-07 11:20:51.045457 qa_test-0.0.4/setup.cfg
+-rw-r--r--   0 tujianhong   (502) staff       (20)      539 2024-04-07 11:20:30.000000 qa_test-0.0.4/setup.py
```

### Comparing `qa_test-0.0.3/LICENSE` & `qa_test-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `qa_test-0.0.3/README.md` & `qa_test-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `qa_test-0.0.3/examples/assistant_weather_bot.py` & `qa_test-0.0.4/qwen_agent/llm/qwenvl_dashscope.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,79 +1,87 @@
-"""A weather forecast assistant implemented by assistant"""
 import os
-from typing import Optional
-
-from qwen_agent.agents import Assistant
-
-ROOT_RESOURCE = os.path.join(os.path.dirname(__file__), 'resource')
-
-
-def init_agent_service():
-    llm_cfg = {'model': 'qwen-max'}
-    system = (
-        '你扮演一个天气预报助手，你具有查询天气和画图能力。'
-        '你需要查询相应地区的天气，然后调用给你的画图工具绘制一张城市的图，并从给定的诗词文档中选一首相关的诗词来描述天气，不要说文档以外的诗词。')
-
-    tools = ['image_gen', 'amap_weather']
-    bot = Assistant(llm=llm_cfg, system_message=system, function_list=tools)
-
-    return bot
-
-
-def app():
-    # Define the agent
-    bot = init_agent_service()
-
-    # Chat
-    messages = []
-    while True:
-        # Query example: 海淀区天气
-        query = input('user question: ')
-        # File example: resource/poem.pdf
-        file = input('file url (press enter if no file): ').strip()
-        if not query:
-            print('user question cannot be empty！')
-            continue
-        if not file:
-            messages.append({'role': 'user', 'content': query})
+from http import HTTPStatus
+from pprint import pformat
+from typing import Dict, Iterator, List, Optional
+
+import dashscope
+
+from qwen_agent.llm.base import ModelServiceError, register_llm
+from qwen_agent.llm.function_calling import BaseFnCallModel
+from qwen_agent.llm.text_base import format_as_text_messages
+from qwen_agent.log import logger
+
+from .schema import ContentItem, Message
+
+
+@register_llm('qwenvl_dashscope')
+class QwenVLChatAtDS(BaseFnCallModel):
+
+    def __init__(self, cfg: Optional[Dict] = None):
+        super().__init__(cfg)
+        self.model = self.model or 'qwen-vl-max'
+
+        cfg = cfg or {}
+        api_key = cfg.get('api_key', '')
+        if not api_key:
+            api_key = os.getenv('DASHSCOPE_API_KEY', 'EMPTY')
+        api_key = api_key.strip()
+        dashscope.api_key = api_key
+
+    def _chat_stream(
+        self,
+        messages: List[Message],
+        delta_stream: bool = False,
+    ) -> Iterator[List[Message]]:
+        if delta_stream:
+            raise NotImplementedError
+
+        messages = [msg.model_dump() for msg in messages]
+        logger.debug(f'*{pformat(messages, indent=2)}*')
+        response = dashscope.MultiModalConversation.call(
+            model=self.model,
+            messages=messages,
+            result_format='message',
+            stream=True,
+            **self.generate_cfg)
+
+        for trunk in response:
+            if trunk.status_code == HTTPStatus.OK:
+                yield _extract_vl_response(trunk)
+            else:
+                raise ModelServiceError(code=trunk.code, message=trunk.message)
+
+    def _chat_no_stream(
+        self,
+        messages: List[Message],
+    ) -> List[Message]:
+        messages = [msg.model_dump() for msg in messages]
+        logger.debug(f'*{pformat(messages, indent=2)}*')
+        response = dashscope.MultiModalConversation.call(
+            model=self.model,
+            messages=messages,
+            result_format='message',
+            stream=False,
+            **self.generate_cfg)
+        if response.status_code == HTTPStatus.OK:
+            return _extract_vl_response(response=response)
         else:
-            messages.append({
-                'role': 'user',
-                'content': [{
-                    'text': query
-                }, {
-                    'file': file
-                }]
-            })
-
-        response = []
-        for response in bot.run(messages):
-            print('bot response:', response)
-        messages.extend(response)
-
-
-def test(query='海淀区天气',
-         file: Optional[str] = os.path.join(ROOT_RESOURCE, 'poem.pdf')):
-    # Define the agent
-    bot = init_agent_service()
-
-    # Chat
-    messages = []
-
-    if not file:
-        messages.append({'role': 'user', 'content': query})
-    else:
-        messages.append({
-            'role': 'user',
-            'content': [{
-                'text': query
-            }, {
-                'file': file
-            }]
-        })
-
-    for response in bot.run(messages):
-        print('bot response:', response)
-
+            raise ModelServiceError(code=response.code,
+                                    message=response.message)
 
-if __name__ == '__main__':
-    app()
+    def _postprocess_messages(self, messages: List[Message],
+                              fncall_mode: bool) -> List[Message]:
+        messages = super()._postprocess_messages(messages,
+                                                 fncall_mode=fncall_mode)
+        # Make VL return the same format as text models for easy usage
+        messages = format_as_text_messages(messages)
+        return messages
+
+
+def _extract_vl_response(response) -> List[Message]:
+    output = response.output.choices[0].message
+    text_content = []
+    for item in output.content:
+        for k, v in item.items():
+            if k in ('text', 'box'):
+                text_content.append(ContentItem(text=v))
+    return [Message(role=output.role, content=text_content)]
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `qa_test-0.0.3/qwen_agent/agent.py` & `qa_test-0.0.4/qwen_agent/agent.py`

 * *Files identical despite different names*

### Comparing `qa_test-0.0.3/qwen_agent/agents/__init__.py` & `qa_test-0.0.4/qwen_agent/agents/__init__.py`

 * *Files identical despite different names*

### Comparing `qa_test-0.0.3/qwen_agent/agents/article_agent.py` & `qa_test-0.0.4/qwen_agent/agents/article_agent.py`

 * *Files identical despite different names*

### Comparing `qa_test-0.0.3/qwen_agent/agents/assistant.py` & `qa_test-0.0.4/qwen_agent/agents/assistant.py`

 * *Files identical despite different names*

### Comparing `qa_test-0.0.3/qwen_agent/agents/docqa_agent.py` & `qa_test-0.0.4/qwen_agent/agents/docqa_agent.py`

 * *Files identical despite different names*

### Comparing `qa_test-0.0.3/qwen_agent/agents/fncall_agent.py` & `qa_test-0.0.4/qwen_agent/agents/fncall_agent.py`

 * *Files identical despite different names*

### Comparing `qa_test-0.0.3/qwen_agent/agents/group_chat.py` & `qa_test-0.0.4/qwen_agent/agents/group_chat.py`

 * *Files identical despite different names*

### Comparing `qa_test-0.0.3/qwen_agent/agents/group_chat_auto_router.py` & `qa_test-0.0.4/qwen_agent/agents/group_chat_auto_router.py`

 * *Files identical despite different names*

### Comparing `qa_test-0.0.3/qwen_agent/agents/group_chat_creator.py` & `qa_test-0.0.4/qwen_agent/agents/group_chat_creator.py`

 * *Files identical despite different names*

### Comparing `qa_test-0.0.3/qwen_agent/agents/react_chat.py` & `qa_test-0.0.4/qwen_agent/agents/react_chat.py`

 * *Files identical despite different names*

### Comparing `qa_test-0.0.3/qwen_agent/agents/router.py` & `qa_test-0.0.4/qwen_agent/agents/router.py`

 * *Files identical despite different names*

### Comparing `qa_test-0.0.3/qwen_agent/agents/write_from_scratch.py` & `qa_test-0.0.4/qwen_agent/agents/write_from_scratch.py`

 * *Files identical despite different names*

### Comparing `qa_test-0.0.3/qwen_agent/llm/__init__.py` & `qa_test-0.0.4/qwen_agent/llm/__init__.py`

 * *Files identical despite different names*

### Comparing `qa_test-0.0.3/qwen_agent/llm/base.py` & `qa_test-0.0.4/qwen_agent/llm/base.py`

 * *Files identical despite different names*

### Comparing `qa_test-0.0.3/qwen_agent/llm/function_calling.py` & `qa_test-0.0.4/qwen_agent/llm/function_calling.py`

 * *Files identical despite different names*

### Comparing `qa_test-0.0.3/qwen_agent/llm/oai.py` & `qa_test-0.0.4/qwen_agent/llm/oai.py`

 * *Files identical despite different names*

### Comparing `qa_test-0.0.3/qwen_agent/llm/qwen_dashscope.py` & `qa_test-0.0.4/qwen_agent/llm/qwen_dashscope.py`

 * *Files identical despite different names*

### Comparing `qa_test-0.0.3/qwen_agent/llm/schema.py` & `qa_test-0.0.4/qwen_agent/llm/schema.py`

 * *Files identical despite different names*

### Comparing `qa_test-0.0.3/qwen_agent/llm/text_base.py` & `qa_test-0.0.4/qwen_agent/llm/text_base.py`

 * *Files identical despite different names*

### Comparing `qa_test-0.0.3/qwen_agent/log.py` & `qa_test-0.0.4/qwen_agent/log.py`

 * *Files identical despite different names*

### Comparing `qa_test-0.0.3/qwen_agent/memory/memory.py` & `qa_test-0.0.4/qwen_agent/memory/memory.py`

 * *Files identical despite different names*

### Comparing `qa_test-0.0.3/qwen_agent/prompts/continue_writing.py` & `qa_test-0.0.4/qwen_agent/prompts/continue_writing.py`

 * *Files identical despite different names*

### Comparing `qa_test-0.0.3/qwen_agent/prompts/doc_qa.py` & `qa_test-0.0.4/qwen_agent/prompts/doc_qa.py`

 * *Files identical despite different names*

### Comparing `qa_test-0.0.3/qwen_agent/prompts/expand_writing.py` & `qa_test-0.0.4/qwen_agent/prompts/expand_writing.py`

 * *Files identical despite different names*

### Comparing `qa_test-0.0.3/qwen_agent/prompts/gen_keyword.py` & `qa_test-0.0.4/qwen_agent/prompts/gen_keyword.py`

 * *Files identical despite different names*

### Comparing `qa_test-0.0.3/qwen_agent/prompts/outline_writing.py` & `qa_test-0.0.4/qwen_agent/prompts/outline_writing.py`

 * *Files identical despite different names*

### Comparing `qa_test-0.0.3/qwen_agent/tools/__init__.py` & `qa_test-0.0.4/qwen_agent/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `qa_test-0.0.3/qwen_agent/tools/amap_weather.py` & `qa_test-0.0.4/qwen_agent/tools/amap_weather.py`

 * *Files identical despite different names*

### Comparing `qa_test-0.0.3/qwen_agent/tools/base.py` & `qa_test-0.0.4/qwen_agent/tools/base.py`

 * *Files identical despite different names*

### Comparing `qa_test-0.0.3/qwen_agent/tools/code_interpreter.py` & `qa_test-0.0.4/qwen_agent/tools/code_interpreter.py`

 * *Files identical despite different names*

### Comparing `qa_test-0.0.3/qwen_agent/tools/doc_parser.py` & `qa_test-0.0.4/qwen_agent/tools/doc_parser.py`

 * *Files identical despite different names*

### Comparing `qa_test-0.0.3/qwen_agent/tools/image_gen.py` & `qa_test-0.0.4/qwen_agent/tools/image_gen.py`

 * *Files identical despite different names*

### Comparing `qa_test-0.0.3/qwen_agent/tools/resource/AlibabaPuHuiTi-3-45-Light.ttf` & `qa_test-0.0.4/qwen_agent/tools/resource/AlibabaPuHuiTi-3-45-Light.ttf`

 * *Files identical despite different names*

### Comparing `qa_test-0.0.3/qwen_agent/tools/resource/code_interpreter_init_kernel.py` & `qa_test-0.0.4/qwen_agent/tools/resource/code_interpreter_init_kernel.py`

 * *Files identical despite different names*

### Comparing `qa_test-0.0.3/qwen_agent/tools/resource/image_service.py` & `qa_test-0.0.4/qwen_agent/tools/resource/image_service.py`

 * *Files identical despite different names*

### Comparing `qa_test-0.0.3/qwen_agent/tools/retrieval.py` & `qa_test-0.0.4/qwen_agent/tools/retrieval.py`

 * *Files identical despite different names*

### Comparing `qa_test-0.0.3/qwen_agent/tools/similarity_search.py` & `qa_test-0.0.4/qwen_agent/tools/similarity_search.py`

 * *Files identical despite different names*

### Comparing `qa_test-0.0.3/qwen_agent/tools/storage.py` & `qa_test-0.0.4/qwen_agent/tools/storage.py`

 * *Files identical despite different names*

### Comparing `qa_test-0.0.3/qwen_agent/tools/web_extractor.py` & `qa_test-0.0.4/qwen_agent/tools/web_extractor.py`

 * *Files identical despite different names*

### Comparing `qa_test-0.0.3/qwen_agent/utils/doc_parser.py` & `qa_test-0.0.4/qwen_agent/utils/doc_parser.py`

 * *Files identical despite different names*

### Comparing `qa_test-0.0.3/qwen_agent/utils/qwen.tiktoken` & `qa_test-0.0.4/qwen_agent/utils/qwen.tiktoken`

 * *Files identical despite different names*

### Comparing `qa_test-0.0.3/qwen_agent/utils/tokenization_qwen.py` & `qa_test-0.0.4/qwen_agent/utils/tokenization_qwen.py`

 * *Files identical despite different names*

### Comparing `qa_test-0.0.3/qwen_agent/utils/utils.py` & `qa_test-0.0.4/qwen_agent/utils/utils.py`

 * *Files identical despite different names*

