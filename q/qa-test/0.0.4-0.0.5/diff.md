# Comparing `tmp/qa_test-0.0.4.tar.gz` & `tmp/qa_test-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qa_test-0.0.4.tar", last modified: Sun Apr  7 11:20:51 2024, max compression
+gzip compressed data, was "qa_test-0.0.5.tar", last modified: Sun Apr  7 11:26:20 2024, max compression
```

## Comparing `qa_test-0.0.4.tar` & `qa_test-0.0.5.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxr-xr-x   0 tujianhong   (502) staff       (20)        0 2024-04-07 11:20:51.045376 qa_test-0.0.4/
--rw-r--r--   0 tujianhong   (502) staff       (20)     6897 2024-04-07 07:48:44.000000 qa_test-0.0.4/LICENSE
--rw-r--r--   0 tujianhong   (502) staff       (20)       85 2024-04-07 11:18:25.000000 qa_test-0.0.4/MANIFEST.in
--rw-r--r--   0 tujianhong   (502) staff       (20)      121 2024-04-07 11:20:51.045129 qa_test-0.0.4/PKG-INFO
--rw-r--r--   0 tujianhong   (502) staff       (20)     8736 2024-04-07 07:48:44.000000 qa_test-0.0.4/README.md
-drwxr-xr-x   0 tujianhong   (502) staff       (20)        0 2024-04-07 11:20:50.972299 qa_test-0.0.4/qa_test.egg-info/
--rw-r--r--   0 tujianhong   (502) staff       (20)      121 2024-04-07 11:20:50.000000 qa_test-0.0.4/qa_test.egg-info/PKG-INFO
--rw-r--r--   0 tujianhong   (502) staff       (20)     1785 2024-04-07 11:20:50.000000 qa_test-0.0.4/qa_test.egg-info/SOURCES.txt
--rw-r--r--   0 tujianhong   (502) staff       (20)        1 2024-04-07 11:20:50.000000 qa_test-0.0.4/qa_test.egg-info/dependency_links.txt
--rw-r--r--   0 tujianhong   (502) staff       (20)      257 2024-04-07 11:20:50.000000 qa_test-0.0.4/qa_test.egg-info/requires.txt
--rw-r--r--   0 tujianhong   (502) staff       (20)       11 2024-04-07 11:20:50.000000 qa_test-0.0.4/qa_test.egg-info/top_level.txt
-drwxr-xr-x   0 tujianhong   (502) staff       (20)        0 2024-04-07 11:20:50.973704 qa_test-0.0.4/qwen_agent/
--rw-r--r--   0 tujianhong   (502) staff       (20)       46 2024-04-07 07:48:45.000000 qa_test-0.0.4/qwen_agent/__init__.py
--rw-r--r--   0 tujianhong   (502) staff       (20)     8672 2024-04-07 07:48:45.000000 qa_test-0.0.4/qwen_agent/agent.py
-drwxr-xr-x   0 tujianhong   (502) staff       (20)        0 2024-04-07 11:20:50.980236 qa_test-0.0.4/qwen_agent/agents/
--rw-r--r--   0 tujianhong   (502) staff       (20)      626 2024-04-07 07:48:45.000000 qa_test-0.0.4/qwen_agent/agents/__init__.py
--rw-r--r--   0 tujianhong   (502) staff       (20)     1598 2024-04-07 07:48:45.000000 qa_test-0.0.4/qwen_agent/agents/article_agent.py
--rw-r--r--   0 tujianhong   (502) staff       (20)     2780 2024-04-07 07:48:45.000000 qa_test-0.0.4/qwen_agent/agents/assistant.py
--rw-r--r--   0 tujianhong   (502) staff       (20)     1766 2024-04-07 07:48:45.000000 qa_test-0.0.4/qwen_agent/agents/docqa_agent.py
--rw-r--r--   0 tujianhong   (502) staff       (20)     4155 2024-04-07 07:48:45.000000 qa_test-0.0.4/qwen_agent/agents/fncall_agent.py
--rw-r--r--   0 tujianhong   (502) staff       (20)    13817 2024-04-07 07:48:45.000000 qa_test-0.0.4/qwen_agent/agents/group_chat.py
--rw-r--r--   0 tujianhong   (502) staff       (20)     3496 2024-04-07 07:48:45.000000 qa_test-0.0.4/qwen_agent/agents/group_chat_auto_router.py
--rw-r--r--   0 tujianhong   (502) staff       (20)     6592 2024-04-07 07:48:45.000000 qa_test-0.0.4/qwen_agent/agents/group_chat_creator.py
--rw-r--r--   0 tujianhong   (502) staff       (20)     7873 2024-04-07 07:48:45.000000 qa_test-0.0.4/qwen_agent/agents/react_chat.py
--rw-r--r--   0 tujianhong   (502) staff       (20)     4204 2024-04-07 07:48:45.000000 qa_test-0.0.4/qwen_agent/agents/router.py
--rw-r--r--   0 tujianhong   (502) staff       (20)      504 2024-04-07 07:48:45.000000 qa_test-0.0.4/qwen_agent/agents/user_agent.py
--rw-r--r--   0 tujianhong   (502) staff       (20)     3956 2024-04-07 07:48:45.000000 qa_test-0.0.4/qwen_agent/agents/write_from_scratch.py
-drwxr-xr-x   0 tujianhong   (502) staff       (20)        0 2024-04-07 11:20:50.984320 qa_test-0.0.4/qwen_agent/llm/
--rw-r--r--   0 tujianhong   (502) staff       (20)     1908 2024-04-07 07:48:45.000000 qa_test-0.0.4/qwen_agent/llm/__init__.py
--rw-r--r--   0 tujianhong   (502) staff       (20)    13188 2024-04-07 07:48:45.000000 qa_test-0.0.4/qwen_agent/llm/base.py
--rw-r--r--   0 tujianhong   (502) staff       (20)    13002 2024-04-07 07:48:45.000000 qa_test-0.0.4/qwen_agent/llm/function_calling.py
--rw-r--r--   0 tujianhong   (502) staff       (20)     4269 2024-04-07 07:48:45.000000 qa_test-0.0.4/qwen_agent/llm/oai.py
--rw-r--r--   0 tujianhong   (502) staff       (20)     6404 2024-04-07 07:48:45.000000 qa_test-0.0.4/qwen_agent/llm/qwen_dashscope.py
--rw-r--r--   0 tujianhong   (502) staff       (20)     3012 2024-04-07 07:48:45.000000 qa_test-0.0.4/qwen_agent/llm/qwenvl_dashscope.py
--rw-r--r--   0 tujianhong   (502) staff       (20)     3322 2024-04-07 07:48:45.000000 qa_test-0.0.4/qwen_agent/llm/schema.py
--rw-r--r--   0 tujianhong   (502) staff       (20)     1596 2024-04-07 07:48:45.000000 qa_test-0.0.4/qwen_agent/llm/text_base.py
--rw-r--r--   0 tujianhong   (502) staff       (20)      599 2024-04-07 07:48:45.000000 qa_test-0.0.4/qwen_agent/log.py
-drwxr-xr-x   0 tujianhong   (502) staff       (20)        0 2024-04-07 11:20:50.987227 qa_test-0.0.4/qwen_agent/memory/
--rw-r--r--   0 tujianhong   (502) staff       (20)       49 2024-04-07 07:48:45.000000 qa_test-0.0.4/qwen_agent/memory/__init__.py
--rw-r--r--   0 tujianhong   (502) staff       (20)     4053 2024-04-07 07:48:45.000000 qa_test-0.0.4/qwen_agent/memory/memory.py
-drwxr-xr-x   0 tujianhong   (502) staff       (20)        0 2024-04-07 11:20:50.992505 qa_test-0.0.4/qwen_agent/prompts/
--rw-r--r--   0 tujianhong   (502) staff       (20)      368 2024-04-07 07:48:45.000000 qa_test-0.0.4/qwen_agent/prompts/__init__.py
--rw-r--r--   0 tujianhong   (502) staff       (20)     1343 2024-04-07 07:48:45.000000 qa_test-0.0.4/qwen_agent/prompts/continue_writing.py
--rw-r--r--   0 tujianhong   (502) staff       (20)     1107 2024-04-07 07:48:45.000000 qa_test-0.0.4/qwen_agent/prompts/doc_qa.py
--rw-r--r--   0 tujianhong   (502) staff       (20)     2248 2024-04-07 07:48:45.000000 qa_test-0.0.4/qwen_agent/prompts/expand_writing.py
--rw-r--r--   0 tujianhong   (502) staff       (20)     3248 2024-04-07 07:48:45.000000 qa_test-0.0.4/qwen_agent/prompts/gen_keyword.py
--rw-r--r--   0 tujianhong   (502) staff       (20)     1495 2024-04-07 07:48:45.000000 qa_test-0.0.4/qwen_agent/prompts/outline_writing.py
-drwxr-xr-x   0 tujianhong   (502) staff       (20)        0 2024-04-07 11:20:51.002464 qa_test-0.0.4/qwen_agent/tools/
--rw-r--r--   0 tujianhong   (502) staff       (20)      714 2024-04-07 07:48:45.000000 qa_test-0.0.4/qwen_agent/tools/__init__.py
--rw-r--r--   0 tujianhong   (502) staff       (20)     2021 2024-04-07 07:48:45.000000 qa_test-0.0.4/qwen_agent/tools/amap_weather.py
--rw-r--r--   0 tujianhong   (502) staff       (20)     3141 2024-04-07 07:48:45.000000 qa_test-0.0.4/qwen_agent/tools/base.py
--rw-r--r--   0 tujianhong   (502) staff       (20)    12040 2024-04-07 07:48:45.000000 qa_test-0.0.4/qwen_agent/tools/code_interpreter.py
--rw-r--r--   0 tujianhong   (502) staff       (20)     5351 2024-04-07 07:48:45.000000 qa_test-0.0.4/qwen_agent/tools/doc_parser.py
--rw-r--r--   0 tujianhong   (502) staff       (20)     1123 2024-04-07 07:48:45.000000 qa_test-0.0.4/qwen_agent/tools/image_gen.py
-drwxr-xr-x   0 tujianhong   (502) staff       (20)        0 2024-04-07 11:20:51.031212 qa_test-0.0.4/qwen_agent/tools/resource/
--rw-r--r--   0 tujianhong   (502) staff       (20)  8559848 2024-04-07 07:48:45.000000 qa_test-0.0.4/qwen_agent/tools/resource/AlibabaPuHuiTi-3-45-Light.ttf
--rw-r--r--   0 tujianhong   (502) staff       (20)     1169 2024-04-07 07:48:45.000000 qa_test-0.0.4/qwen_agent/tools/resource/code_interpreter_init_kernel.py
--rw-r--r--   0 tujianhong   (502) staff       (20)      553 2024-04-07 07:48:45.000000 qa_test-0.0.4/qwen_agent/tools/resource/image_service.py
--rw-r--r--   0 tujianhong   (502) staff       (20)     3627 2024-04-07 07:48:45.000000 qa_test-0.0.4/qwen_agent/tools/retrieval.py
--rw-r--r--   0 tujianhong   (502) staff       (20)     4898 2024-04-07 07:48:45.000000 qa_test-0.0.4/qwen_agent/tools/similarity_search.py
--rw-r--r--   0 tujianhong   (502) staff       (20)     3584 2024-04-07 07:48:45.000000 qa_test-0.0.4/qwen_agent/tools/storage.py
--rw-r--r--   0 tujianhong   (502) staff       (20)     1376 2024-04-07 07:48:45.000000 qa_test-0.0.4/qwen_agent/tools/web_extractor.py
-drwxr-xr-x   0 tujianhong   (502) staff       (20)        0 2024-04-07 11:20:51.044485 qa_test-0.0.4/qwen_agent/utils/
--rw-r--r--   0 tujianhong   (502) staff       (20)        0 2024-04-07 07:48:45.000000 qa_test-0.0.4/qwen_agent/utils/__init__.py
--rw-r--r--   0 tujianhong   (502) staff       (20)     2728 2024-04-07 07:48:45.000000 qa_test-0.0.4/qwen_agent/utils/doc_parser.py
--rw-r--r--   0 tujianhong   (502) staff       (20)  2561218 2024-04-07 07:48:45.000000 qa_test-0.0.4/qwen_agent/utils/qwen.tiktoken
--rw-r--r--   0 tujianhong   (502) staff       (20)    10526 2024-04-07 07:48:45.000000 qa_test-0.0.4/qwen_agent/utils/tokenization_qwen.py
--rw-r--r--   0 tujianhong   (502) staff       (20)     9829 2024-04-07 07:48:45.000000 qa_test-0.0.4/qwen_agent/utils/utils.py
--rw-r--r--   0 tujianhong   (502) staff       (20)       38 2024-04-07 11:20:51.045457 qa_test-0.0.4/setup.cfg
--rw-r--r--   0 tujianhong   (502) staff       (20)      539 2024-04-07 11:20:30.000000 qa_test-0.0.4/setup.py
+drwxr-xr-x   0 tujianhong   (502) staff       (20)        0 2024-04-07 11:26:20.508897 qa_test-0.0.5/
+-rw-r--r--   0 tujianhong   (502) staff       (20)     6897 2024-04-07 07:48:44.000000 qa_test-0.0.5/LICENSE
+-rw-r--r--   0 tujianhong   (502) staff       (20)       85 2024-04-07 11:18:25.000000 qa_test-0.0.5/MANIFEST.in
+-rw-r--r--   0 tujianhong   (502) staff       (20)      121 2024-04-07 11:26:20.508591 qa_test-0.0.5/PKG-INFO
+-rw-r--r--   0 tujianhong   (502) staff       (20)     8736 2024-04-07 07:48:44.000000 qa_test-0.0.5/README.md
+drwxr-xr-x   0 tujianhong   (502) staff       (20)        0 2024-04-07 11:26:20.414545 qa_test-0.0.5/qa_test.egg-info/
+-rw-r--r--   0 tujianhong   (502) staff       (20)      121 2024-04-07 11:26:20.000000 qa_test-0.0.5/qa_test.egg-info/PKG-INFO
+-rw-r--r--   0 tujianhong   (502) staff       (20)     1785 2024-04-07 11:26:20.000000 qa_test-0.0.5/qa_test.egg-info/SOURCES.txt
+-rw-r--r--   0 tujianhong   (502) staff       (20)        1 2024-04-07 11:26:20.000000 qa_test-0.0.5/qa_test.egg-info/dependency_links.txt
+-rw-r--r--   0 tujianhong   (502) staff       (20)      257 2024-04-07 11:26:20.000000 qa_test-0.0.5/qa_test.egg-info/requires.txt
+-rw-r--r--   0 tujianhong   (502) staff       (20)       11 2024-04-07 11:26:20.000000 qa_test-0.0.5/qa_test.egg-info/top_level.txt
+drwxr-xr-x   0 tujianhong   (502) staff       (20)        0 2024-04-07 11:26:20.415591 qa_test-0.0.5/qwen_agent/
+-rw-r--r--   0 tujianhong   (502) staff       (20)       46 2024-04-07 07:48:45.000000 qa_test-0.0.5/qwen_agent/__init__.py
+-rw-r--r--   0 tujianhong   (502) staff       (20)     8672 2024-04-07 07:48:45.000000 qa_test-0.0.5/qwen_agent/agent.py
+drwxr-xr-x   0 tujianhong   (502) staff       (20)        0 2024-04-07 11:26:20.438625 qa_test-0.0.5/qwen_agent/agents/
+-rw-r--r--   0 tujianhong   (502) staff       (20)      626 2024-04-07 07:48:45.000000 qa_test-0.0.5/qwen_agent/agents/__init__.py
+-rw-r--r--   0 tujianhong   (502) staff       (20)     1598 2024-04-07 07:48:45.000000 qa_test-0.0.5/qwen_agent/agents/article_agent.py
+-rw-r--r--   0 tujianhong   (502) staff       (20)     2780 2024-04-07 07:48:45.000000 qa_test-0.0.5/qwen_agent/agents/assistant.py
+-rw-r--r--   0 tujianhong   (502) staff       (20)     1766 2024-04-07 07:48:45.000000 qa_test-0.0.5/qwen_agent/agents/docqa_agent.py
+-rw-r--r--   0 tujianhong   (502) staff       (20)     4155 2024-04-07 07:48:45.000000 qa_test-0.0.5/qwen_agent/agents/fncall_agent.py
+-rw-r--r--   0 tujianhong   (502) staff       (20)    13817 2024-04-07 07:48:45.000000 qa_test-0.0.5/qwen_agent/agents/group_chat.py
+-rw-r--r--   0 tujianhong   (502) staff       (20)     3496 2024-04-07 07:48:45.000000 qa_test-0.0.5/qwen_agent/agents/group_chat_auto_router.py
+-rw-r--r--   0 tujianhong   (502) staff       (20)     6592 2024-04-07 07:48:45.000000 qa_test-0.0.5/qwen_agent/agents/group_chat_creator.py
+-rw-r--r--   0 tujianhong   (502) staff       (20)     7873 2024-04-07 07:48:45.000000 qa_test-0.0.5/qwen_agent/agents/react_chat.py
+-rw-r--r--   0 tujianhong   (502) staff       (20)     4204 2024-04-07 07:48:45.000000 qa_test-0.0.5/qwen_agent/agents/router.py
+-rw-r--r--   0 tujianhong   (502) staff       (20)      504 2024-04-07 07:48:45.000000 qa_test-0.0.5/qwen_agent/agents/user_agent.py
+-rw-r--r--   0 tujianhong   (502) staff       (20)     3956 2024-04-07 07:48:45.000000 qa_test-0.0.5/qwen_agent/agents/write_from_scratch.py
+drwxr-xr-x   0 tujianhong   (502) staff       (20)        0 2024-04-07 11:26:20.443903 qa_test-0.0.5/qwen_agent/llm/
+-rw-r--r--   0 tujianhong   (502) staff       (20)     1908 2024-04-07 07:48:45.000000 qa_test-0.0.5/qwen_agent/llm/__init__.py
+-rw-r--r--   0 tujianhong   (502) staff       (20)    13188 2024-04-07 07:48:45.000000 qa_test-0.0.5/qwen_agent/llm/base.py
+-rw-r--r--   0 tujianhong   (502) staff       (20)    13002 2024-04-07 07:48:45.000000 qa_test-0.0.5/qwen_agent/llm/function_calling.py
+-rw-r--r--   0 tujianhong   (502) staff       (20)     4269 2024-04-07 07:48:45.000000 qa_test-0.0.5/qwen_agent/llm/oai.py
+-rw-r--r--   0 tujianhong   (502) staff       (20)     6404 2024-04-07 07:48:45.000000 qa_test-0.0.5/qwen_agent/llm/qwen_dashscope.py
+-rw-r--r--   0 tujianhong   (502) staff       (20)     3012 2024-04-07 07:48:45.000000 qa_test-0.0.5/qwen_agent/llm/qwenvl_dashscope.py
+-rw-r--r--   0 tujianhong   (502) staff       (20)     3322 2024-04-07 07:48:45.000000 qa_test-0.0.5/qwen_agent/llm/schema.py
+-rw-r--r--   0 tujianhong   (502) staff       (20)     1596 2024-04-07 07:48:45.000000 qa_test-0.0.5/qwen_agent/llm/text_base.py
+-rw-r--r--   0 tujianhong   (502) staff       (20)      599 2024-04-07 07:48:45.000000 qa_test-0.0.5/qwen_agent/log.py
+drwxr-xr-x   0 tujianhong   (502) staff       (20)        0 2024-04-07 11:26:20.445592 qa_test-0.0.5/qwen_agent/memory/
+-rw-r--r--   0 tujianhong   (502) staff       (20)       49 2024-04-07 07:48:45.000000 qa_test-0.0.5/qwen_agent/memory/__init__.py
+-rw-r--r--   0 tujianhong   (502) staff       (20)     4053 2024-04-07 07:48:45.000000 qa_test-0.0.5/qwen_agent/memory/memory.py
+drwxr-xr-x   0 tujianhong   (502) staff       (20)        0 2024-04-07 11:26:20.454958 qa_test-0.0.5/qwen_agent/prompts/
+-rw-r--r--   0 tujianhong   (502) staff       (20)      368 2024-04-07 07:48:45.000000 qa_test-0.0.5/qwen_agent/prompts/__init__.py
+-rw-r--r--   0 tujianhong   (502) staff       (20)     1343 2024-04-07 07:48:45.000000 qa_test-0.0.5/qwen_agent/prompts/continue_writing.py
+-rw-r--r--   0 tujianhong   (502) staff       (20)     1107 2024-04-07 07:48:45.000000 qa_test-0.0.5/qwen_agent/prompts/doc_qa.py
+-rw-r--r--   0 tujianhong   (502) staff       (20)     2248 2024-04-07 07:48:45.000000 qa_test-0.0.5/qwen_agent/prompts/expand_writing.py
+-rw-r--r--   0 tujianhong   (502) staff       (20)     3248 2024-04-07 07:48:45.000000 qa_test-0.0.5/qwen_agent/prompts/gen_keyword.py
+-rw-r--r--   0 tujianhong   (502) staff       (20)     1495 2024-04-07 07:48:45.000000 qa_test-0.0.5/qwen_agent/prompts/outline_writing.py
+drwxr-xr-x   0 tujianhong   (502) staff       (20)        0 2024-04-07 11:26:20.469185 qa_test-0.0.5/qwen_agent/tools/
+-rw-r--r--   0 tujianhong   (502) staff       (20)      714 2024-04-07 07:48:45.000000 qa_test-0.0.5/qwen_agent/tools/__init__.py
+-rw-r--r--   0 tujianhong   (502) staff       (20)     2021 2024-04-07 07:48:45.000000 qa_test-0.0.5/qwen_agent/tools/amap_weather.py
+-rw-r--r--   0 tujianhong   (502) staff       (20)     3141 2024-04-07 07:48:45.000000 qa_test-0.0.5/qwen_agent/tools/base.py
+-rw-r--r--   0 tujianhong   (502) staff       (20)    12040 2024-04-07 07:48:45.000000 qa_test-0.0.5/qwen_agent/tools/code_interpreter.py
+-rw-r--r--   0 tujianhong   (502) staff       (20)     5351 2024-04-07 07:48:45.000000 qa_test-0.0.5/qwen_agent/tools/doc_parser.py
+-rw-r--r--   0 tujianhong   (502) staff       (20)     1123 2024-04-07 07:48:45.000000 qa_test-0.0.5/qwen_agent/tools/image_gen.py
+drwxr-xr-x   0 tujianhong   (502) staff       (20)        0 2024-04-07 11:26:20.499175 qa_test-0.0.5/qwen_agent/tools/resource/
+-rw-r--r--   0 tujianhong   (502) staff       (20)  8559848 2024-04-07 07:48:45.000000 qa_test-0.0.5/qwen_agent/tools/resource/AlibabaPuHuiTi-3-45-Light.ttf
+-rw-r--r--   0 tujianhong   (502) staff       (20)     1169 2024-04-07 07:48:45.000000 qa_test-0.0.5/qwen_agent/tools/resource/code_interpreter_init_kernel.py
+-rw-r--r--   0 tujianhong   (502) staff       (20)      553 2024-04-07 07:48:45.000000 qa_test-0.0.5/qwen_agent/tools/resource/image_service.py
+-rw-r--r--   0 tujianhong   (502) staff       (20)     3627 2024-04-07 07:48:45.000000 qa_test-0.0.5/qwen_agent/tools/retrieval.py
+-rw-r--r--   0 tujianhong   (502) staff       (20)     4898 2024-04-07 07:48:45.000000 qa_test-0.0.5/qwen_agent/tools/similarity_search.py
+-rw-r--r--   0 tujianhong   (502) staff       (20)     3584 2024-04-07 07:48:45.000000 qa_test-0.0.5/qwen_agent/tools/storage.py
+-rw-r--r--   0 tujianhong   (502) staff       (20)     1376 2024-04-07 07:48:45.000000 qa_test-0.0.5/qwen_agent/tools/web_extractor.py
+drwxr-xr-x   0 tujianhong   (502) staff       (20)        0 2024-04-07 11:26:20.507892 qa_test-0.0.5/qwen_agent/utils/
+-rw-r--r--   0 tujianhong   (502) staff       (20)        0 2024-04-07 07:48:45.000000 qa_test-0.0.5/qwen_agent/utils/__init__.py
+-rw-r--r--   0 tujianhong   (502) staff       (20)     2728 2024-04-07 07:48:45.000000 qa_test-0.0.5/qwen_agent/utils/doc_parser.py
+-rw-r--r--   0 tujianhong   (502) staff       (20)  2561218 2024-04-07 07:48:45.000000 qa_test-0.0.5/qwen_agent/utils/qwen.tiktoken
+-rw-r--r--   0 tujianhong   (502) staff       (20)    10526 2024-04-07 07:48:45.000000 qa_test-0.0.5/qwen_agent/utils/tokenization_qwen.py
+-rw-r--r--   0 tujianhong   (502) staff       (20)     9829 2024-04-07 07:48:45.000000 qa_test-0.0.5/qwen_agent/utils/utils.py
+-rw-r--r--   0 tujianhong   (502) staff       (20)       38 2024-04-07 11:26:20.508965 qa_test-0.0.5/setup.cfg
+-rw-r--r--   0 tujianhong   (502) staff       (20)      566 2024-04-07 11:26:19.000000 qa_test-0.0.5/setup.py
```

### Comparing `qa_test-0.0.4/LICENSE` & `qa_test-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `qa_test-0.0.4/README.md` & `qa_test-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `qa_test-0.0.4/qa_test.egg-info/SOURCES.txt` & `qa_test-0.0.5/qa_test.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qa_test-0.0.4/qwen_agent/agent.py` & `qa_test-0.0.5/qwen_agent/agent.py`

 * *Files identical despite different names*

### Comparing `qa_test-0.0.4/qwen_agent/agents/__init__.py` & `qa_test-0.0.5/qwen_agent/agents/__init__.py`

 * *Files identical despite different names*

### Comparing `qa_test-0.0.4/qwen_agent/agents/article_agent.py` & `qa_test-0.0.5/qwen_agent/agents/article_agent.py`

 * *Files identical despite different names*

### Comparing `qa_test-0.0.4/qwen_agent/agents/assistant.py` & `qa_test-0.0.5/qwen_agent/agents/assistant.py`

 * *Files identical despite different names*

### Comparing `qa_test-0.0.4/qwen_agent/agents/docqa_agent.py` & `qa_test-0.0.5/qwen_agent/agents/docqa_agent.py`

 * *Files identical despite different names*

### Comparing `qa_test-0.0.4/qwen_agent/agents/fncall_agent.py` & `qa_test-0.0.5/qwen_agent/agents/fncall_agent.py`

 * *Files identical despite different names*

### Comparing `qa_test-0.0.4/qwen_agent/agents/group_chat.py` & `qa_test-0.0.5/qwen_agent/agents/group_chat.py`

 * *Files identical despite different names*

### Comparing `qa_test-0.0.4/qwen_agent/agents/group_chat_auto_router.py` & `qa_test-0.0.5/qwen_agent/agents/group_chat_auto_router.py`

 * *Files identical despite different names*

### Comparing `qa_test-0.0.4/qwen_agent/agents/group_chat_creator.py` & `qa_test-0.0.5/qwen_agent/agents/group_chat_creator.py`

 * *Files identical despite different names*

### Comparing `qa_test-0.0.4/qwen_agent/agents/react_chat.py` & `qa_test-0.0.5/qwen_agent/agents/react_chat.py`

 * *Files identical despite different names*

### Comparing `qa_test-0.0.4/qwen_agent/agents/router.py` & `qa_test-0.0.5/qwen_agent/agents/router.py`

 * *Files identical despite different names*

### Comparing `qa_test-0.0.4/qwen_agent/agents/write_from_scratch.py` & `qa_test-0.0.5/qwen_agent/agents/write_from_scratch.py`

 * *Files identical despite different names*

### Comparing `qa_test-0.0.4/qwen_agent/llm/__init__.py` & `qa_test-0.0.5/qwen_agent/llm/__init__.py`

 * *Files identical despite different names*

### Comparing `qa_test-0.0.4/qwen_agent/llm/base.py` & `qa_test-0.0.5/qwen_agent/llm/base.py`

 * *Files identical despite different names*

### Comparing `qa_test-0.0.4/qwen_agent/llm/function_calling.py` & `qa_test-0.0.5/qwen_agent/llm/function_calling.py`

 * *Files identical despite different names*

### Comparing `qa_test-0.0.4/qwen_agent/llm/oai.py` & `qa_test-0.0.5/qwen_agent/llm/oai.py`

 * *Files identical despite different names*

### Comparing `qa_test-0.0.4/qwen_agent/llm/qwen_dashscope.py` & `qa_test-0.0.5/qwen_agent/llm/qwen_dashscope.py`

 * *Files identical despite different names*

### Comparing `qa_test-0.0.4/qwen_agent/llm/qwenvl_dashscope.py` & `qa_test-0.0.5/qwen_agent/llm/qwenvl_dashscope.py`

 * *Files identical despite different names*

### Comparing `qa_test-0.0.4/qwen_agent/llm/schema.py` & `qa_test-0.0.5/qwen_agent/llm/schema.py`

 * *Files identical despite different names*

### Comparing `qa_test-0.0.4/qwen_agent/llm/text_base.py` & `qa_test-0.0.5/qwen_agent/llm/text_base.py`

 * *Files identical despite different names*

### Comparing `qa_test-0.0.4/qwen_agent/log.py` & `qa_test-0.0.5/qwen_agent/log.py`

 * *Files identical despite different names*

### Comparing `qa_test-0.0.4/qwen_agent/memory/memory.py` & `qa_test-0.0.5/qwen_agent/memory/memory.py`

 * *Files identical despite different names*

### Comparing `qa_test-0.0.4/qwen_agent/prompts/continue_writing.py` & `qa_test-0.0.5/qwen_agent/prompts/continue_writing.py`

 * *Files identical despite different names*

### Comparing `qa_test-0.0.4/qwen_agent/prompts/doc_qa.py` & `qa_test-0.0.5/qwen_agent/prompts/doc_qa.py`

 * *Files identical despite different names*

### Comparing `qa_test-0.0.4/qwen_agent/prompts/expand_writing.py` & `qa_test-0.0.5/qwen_agent/prompts/expand_writing.py`

 * *Files identical despite different names*

### Comparing `qa_test-0.0.4/qwen_agent/prompts/gen_keyword.py` & `qa_test-0.0.5/qwen_agent/prompts/gen_keyword.py`

 * *Files identical despite different names*

### Comparing `qa_test-0.0.4/qwen_agent/prompts/outline_writing.py` & `qa_test-0.0.5/qwen_agent/prompts/outline_writing.py`

 * *Files identical despite different names*

### Comparing `qa_test-0.0.4/qwen_agent/tools/__init__.py` & `qa_test-0.0.5/qwen_agent/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `qa_test-0.0.4/qwen_agent/tools/amap_weather.py` & `qa_test-0.0.5/qwen_agent/tools/amap_weather.py`

 * *Files identical despite different names*

### Comparing `qa_test-0.0.4/qwen_agent/tools/base.py` & `qa_test-0.0.5/qwen_agent/tools/base.py`

 * *Files identical despite different names*

### Comparing `qa_test-0.0.4/qwen_agent/tools/code_interpreter.py` & `qa_test-0.0.5/qwen_agent/tools/code_interpreter.py`

 * *Files identical despite different names*

### Comparing `qa_test-0.0.4/qwen_agent/tools/doc_parser.py` & `qa_test-0.0.5/qwen_agent/tools/doc_parser.py`

 * *Files identical despite different names*

### Comparing `qa_test-0.0.4/qwen_agent/tools/image_gen.py` & `qa_test-0.0.5/qwen_agent/tools/image_gen.py`

 * *Files identical despite different names*

### Comparing `qa_test-0.0.4/qwen_agent/tools/resource/AlibabaPuHuiTi-3-45-Light.ttf` & `qa_test-0.0.5/qwen_agent/tools/resource/AlibabaPuHuiTi-3-45-Light.ttf`

 * *Files identical despite different names*

### Comparing `qa_test-0.0.4/qwen_agent/tools/resource/code_interpreter_init_kernel.py` & `qa_test-0.0.5/qwen_agent/tools/resource/code_interpreter_init_kernel.py`

 * *Files identical despite different names*

### Comparing `qa_test-0.0.4/qwen_agent/tools/resource/image_service.py` & `qa_test-0.0.5/qwen_agent/tools/resource/image_service.py`

 * *Files identical despite different names*

### Comparing `qa_test-0.0.4/qwen_agent/tools/retrieval.py` & `qa_test-0.0.5/qwen_agent/tools/retrieval.py`

 * *Files identical despite different names*

### Comparing `qa_test-0.0.4/qwen_agent/tools/similarity_search.py` & `qa_test-0.0.5/qwen_agent/tools/similarity_search.py`

 * *Files identical despite different names*

### Comparing `qa_test-0.0.4/qwen_agent/tools/storage.py` & `qa_test-0.0.5/qwen_agent/tools/storage.py`

 * *Files identical despite different names*

### Comparing `qa_test-0.0.4/qwen_agent/tools/web_extractor.py` & `qa_test-0.0.5/qwen_agent/tools/web_extractor.py`

 * *Files identical despite different names*

### Comparing `qa_test-0.0.4/qwen_agent/utils/doc_parser.py` & `qa_test-0.0.5/qwen_agent/utils/doc_parser.py`

 * *Files identical despite different names*

### Comparing `qa_test-0.0.4/qwen_agent/utils/qwen.tiktoken` & `qa_test-0.0.5/qwen_agent/utils/qwen.tiktoken`

 * *Files identical despite different names*

### Comparing `qa_test-0.0.4/qwen_agent/utils/tokenization_qwen.py` & `qa_test-0.0.5/qwen_agent/utils/tokenization_qwen.py`

 * *Files identical despite different names*

### Comparing `qa_test-0.0.4/qwen_agent/utils/utils.py` & `qa_test-0.0.5/qwen_agent/utils/utils.py`

 * *Files identical despite different names*

### Comparing `qa_test-0.0.4/setup.py` & `qa_test-0.0.5/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,15 +6,15 @@
         content = req.read()
         requirements = content.split('\n')
     return requirements
 
 
 setup(
     name='qa_test',
-    version='0.0.4',
+    version='0.0.5',
     packages=find_packages(exclude=['examples', 'examples.*', 'qwen_server', 'qwen_server.*']),
     package_data={
-        'qwen_agent': ['utils/qwen.tiktoken', 'tools/resource/*'],
+        'qwen_agent': ['utils/qwen.tiktoken', 'tools/resource/*.ttf', 'tools/resource/*.py'],
     },
     install_requires=read_requirements(),
     url='https://github.com/QwenLM/Qwen-Agent'
 )
```

