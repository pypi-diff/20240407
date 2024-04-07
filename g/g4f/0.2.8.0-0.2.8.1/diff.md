# Comparing `tmp/g4f-0.2.8.0.tar.gz` & `tmp/g4f-0.2.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "g4f-0.2.8.0.tar", last modified: Fri Apr  5 19:04:54 2024, max compression
+gzip compressed data, was "g4f-0.2.8.1.tar", last modified: Sun Apr  7 09:30:48 2024, max compression
```

## Comparing `g4f-0.2.8.0.tar` & `g4f-0.2.8.1.tar`

### file list

```diff
@@ -1,207 +1,226 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:04:54.054947 g4f-0.2.8.0/
--rw-r--r--   0 runner    (1001) docker     (127)    35148 2024-04-05 19:04:50.000000 g4f-0.2.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-05 19:04:50.000000 g4f-0.2.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    42097 2024-04-05 19:04:54.050947 g4f-0.2.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    38981 2024-04-05 19:04:50.000000 g4f-0.2.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:04:54.018947 g4f-0.2.8.0/g4f/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:04:54.026946 g4f-0.2.8.0/g4f/Provider/
--rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/Provider/Aura.py
--rw-r--r--   0 runner    (1001) docker     (127)    20635 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/Provider/Bing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2193 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/Provider/BingCreateImages.py
--rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/Provider/ChatForAi.py
--rw-r--r--   0 runner    (1001) docker     (127)     2653 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/Provider/Chatgpt4Online.py
--rw-r--r--   0 runner    (1001) docker     (127)     3608 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/Provider/ChatgptAi.py
--rw-r--r--   0 runner    (1001) docker     (127)     2855 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/Provider/ChatgptFree.py
--rw-r--r--   0 runner    (1001) docker     (127)     2503 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/Provider/ChatgptNext.py
--rw-r--r--   0 runner    (1001) docker     (127)     4278 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/Provider/ChatgptX.py
--rw-r--r--   0 runner    (1001) docker     (127)     3526 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/Provider/DeepInfra.py
--rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/Provider/FlowGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/Provider/FreeChatgpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/Provider/FreeGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     3937 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/Provider/GeminiPro.py
--rw-r--r--   0 runner    (1001) docker     (127)     2557 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/Provider/GeminiProChat.py
--rw-r--r--   0 runner    (1001) docker     (127)     3922 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/Provider/GigaChat.py
--rw-r--r--   0 runner    (1001) docker     (127)     2321 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/Provider/GptTalkRu.py
--rw-r--r--   0 runner    (1001) docker     (127)     3948 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/Provider/HuggingChat.py
--rw-r--r--   0 runner    (1001) docker     (127)     2940 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/Provider/HuggingFace.py
--rw-r--r--   0 runner    (1001) docker     (127)     2485 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/Provider/Koala.py
--rw-r--r--   0 runner    (1001) docker     (127)     5086 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/Provider/Liaobots.py
--rw-r--r--   0 runner    (1001) docker     (127)     3105 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/Provider/Llama2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3951 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/Provider/PerplexityLabs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/Provider/Pi.py
--rw-r--r--   0 runner    (1001) docker     (127)     4027 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/Provider/Vercel.py
--rw-r--r--   0 runner    (1001) docker     (127)     7243 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/Provider/You.py
--rw-r--r--   0 runner    (1001) docker     (127)     2047 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/Provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/Provider/base_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:04:54.026946 g4f-0.2.8.0/g4f/Provider/bing/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/Provider/bing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3541 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/Provider/bing/conversation.py
--rw-r--r--   0 runner    (1001) docker     (127)     7597 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/Provider/bing/create_images.py
--rw-r--r--   0 runner    (1001) docker     (127)     4746 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/Provider/bing/upload_image.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:04:54.034947 g4f-0.2.8.0/g4f/Provider/deprecated/
--rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/Provider/deprecated/Acytoo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/Provider/deprecated/AiAsk.py
--rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/Provider/deprecated/AiChatOnline.py
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/Provider/deprecated/AiService.py
--rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/Provider/deprecated/Aibn.py
--rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/Provider/deprecated/Aichat.py
--rw-r--r--   0 runner    (1001) docker     (127)     3358 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/Provider/deprecated/Ails.py
--rw-r--r--   0 runner    (1001) docker     (127)     2952 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/Provider/deprecated/Aivvm.py
--rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/Provider/deprecated/Berlin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/Provider/deprecated/ChatAnywhere.py
--rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/Provider/deprecated/ChatgptDuo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/Provider/deprecated/CodeLinkAva.py
--rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/Provider/deprecated/Cromicle.py
--rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/Provider/deprecated/DfeHub.py
--rw-r--r--   0 runner    (1001) docker     (127)     3398 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/Provider/deprecated/EasyChat.py
--rw-r--r--   0 runner    (1001) docker     (127)     2755 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/Provider/deprecated/Equing.py
--rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/Provider/deprecated/FakeGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/Provider/deprecated/FastGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/Provider/deprecated/Forefront.py
--rw-r--r--   0 runner    (1001) docker     (127)     3552 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/Provider/deprecated/GPTalk.py
--rw-r--r--   0 runner    (1001) docker     (127)     2658 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/Provider/deprecated/GeekGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/Provider/deprecated/GetGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2925 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/Provider/deprecated/H2o.py
--rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/Provider/deprecated/Hashnode.py
--rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/Provider/deprecated/Lockchat.py
--rw-r--r--   0 runner    (1001) docker     (127)     5050 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/Provider/deprecated/Myshell.py
--rw-r--r--   0 runner    (1001) docker     (127)     2500 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/Provider/deprecated/NoowAi.py
--rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/Provider/deprecated/Opchatgpts.py
--rw-r--r--   0 runner    (1001) docker     (127)     5353 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/Provider/deprecated/Phind.py
--rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/Provider/deprecated/V50.py
--rw-r--r--   0 runner    (1001) docker     (127)    12167 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/Provider/deprecated/Vercel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/Provider/deprecated/Vitalentum.py
--rw-r--r--   0 runner    (1001) docker     (127)     3415 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/Provider/deprecated/VoiGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2464 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/Provider/deprecated/Wewordle.py
--rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/Provider/deprecated/Wuguokai.py
--rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/Provider/deprecated/Ylokh.py
--rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/Provider/deprecated/Yqcloud.py
--rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/Provider/deprecated/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:04:54.034947 g4f-0.2.8.0/g4f/Provider/gigachat_crt/
--rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/Provider/gigachat_crt/russian_trusted_root_ca_pem.crt
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/Provider/helper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:04:54.034947 g4f-0.2.8.0/g4f/Provider/needs_auth/
--rw-r--r--   0 runner    (1001) docker     (127)     8625 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/Provider/needs_auth/Gemini.py
--rw-r--r--   0 runner    (1001) docker     (127)     3309 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/Provider/needs_auth/OpenAssistant.py
--rw-r--r--   0 runner    (1001) docker     (127)    30021 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/Provider/needs_auth/OpenaiChat.py
--rw-r--r--   0 runner    (1001) docker     (127)     4289 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/Provider/needs_auth/Poe.py
--rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/Provider/needs_auth/Raycast.py
--rw-r--r--   0 runner    (1001) docker     (127)     5465 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/Provider/needs_auth/Theb.py
--rw-r--r--   0 runner    (1001) docker     (127)     2655 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/Provider/needs_auth/ThebApi.py
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/Provider/needs_auth/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:04:54.038946 g4f-0.2.8.0/g4f/Provider/not_working/
--rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/Provider/not_working/AItianhu.py
--rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/Provider/not_working/Bestim.py
--rw-r--r--   0 runner    (1001) docker     (127)     4546 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/Provider/not_working/ChatBase.py
--rw-r--r--   0 runner    (1001) docker     (127)     2863 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/Provider/not_working/ChatgptDemo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/Provider/not_working/ChatgptDemoAi.py
--rw-r--r--   0 runner    (1001) docker     (127)     3056 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/Provider/not_working/ChatgptLogin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/Provider/not_working/Chatxyz.py
--rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/Provider/not_working/Gpt6.py
--rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/Provider/not_working/GptChatly.py
--rw-r--r--   0 runner    (1001) docker     (127)     3529 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/Provider/not_working/GptForLove.py
--rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/Provider/not_working/GptGo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/Provider/not_working/GptGod.py
--rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/Provider/not_working/OnlineGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/Provider/not_working/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:04:54.038946 g4f-0.2.8.0/g4f/Provider/npm/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:04:54.038946 g4f-0.2.8.0/g4f/Provider/npm/node_modules/
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/Provider/npm/node_modules/.package-lock.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:04:54.038946 g4f-0.2.8.0/g4f/Provider/npm/node_modules/crypto-js/
--rw-r--r--   0 runner    (1001) docker     (127)     6449 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/Provider/npm/node_modules/crypto-js/README.md
--rw-r--r--   0 runner    (1001) docker     (127)   219092 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/Provider/npm/node_modules/crypto-js/crypto-js.js
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/Provider/npm/package-lock.json
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/Provider/npm/package.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:04:54.038946 g4f-0.2.8.0/g4f/Provider/openai/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/Provider/openai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/Provider/openai/crypt.py
--rw-r--r--   0 runner    (1001) docker     (127)     4649 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/Provider/openai/har_file.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:04:54.038946 g4f-0.2.8.0/g4f/Provider/selenium/
--rw-r--r--   0 runner    (1001) docker     (127)     3839 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/Provider/selenium/AItianhuSpace.py
--rw-r--r--   0 runner    (1001) docker     (127)     2859 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/Provider/selenium/Bard.py
--rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/Provider/selenium/MyShell.py
--rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/Provider/selenium/PerplexityAi.py
--rw-r--r--   0 runner    (1001) docker     (127)     3655 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/Provider/selenium/Phind.py
--rw-r--r--   0 runner    (1001) docker     (127)     2678 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/Provider/selenium/TalkAi.py
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/Provider/selenium/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:04:54.038946 g4f-0.2.8.0/g4f/Provider/unfinished/
--rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/Provider/unfinished/AiChatting.py
--rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/Provider/unfinished/ChatAiGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/Provider/unfinished/Komo.py
--rw-r--r--   0 runner    (1001) docker     (127)     3298 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/Provider/unfinished/MikuChat.py
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/Provider/unfinished/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10959 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:04:54.042946 g4f-0.2.8.0/g4f/api/
--rw-r--r--   0 runner    (1001) docker     (127)     5168 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      893 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/api/_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/api/_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/api/run.py
--rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     8568 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3406 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/cookies.py
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/debug.py
--rw-r--r--   0 runner    (1001) docker     (127)      753 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:04:54.042946 g4f-0.2.8.0/g4f/gui/
--rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/gui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:04:54.042946 g4f-0.2.8.0/g4f/gui/client/
--rw-r--r--   0 runner    (1001) docker     (127)     9843 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/gui/client/index.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:04:54.014946 g4f-0.2.8.0/g4f/gui/client/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:04:54.042946 g4f-0.2.8.0/g4f/gui/client/static/css/
--rw-r--r--   0 runner    (1001) docker     (127)    20099 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/gui/client/static/css/style.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:04:54.042946 g4f-0.2.8.0/g4f/gui/client/static/img/
--rw-r--r--   0 runner    (1001) docker     (127)     8908 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/gui/client/static/img/android-chrome-192x192.png
--rw-r--r--   0 runner    (1001) docker     (127)    17626 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/gui/client/static/img/android-chrome-512x512.png
--rw-r--r--   0 runner    (1001) docker     (127)     7984 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/gui/client/static/img/apple-touch-icon.png
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/gui/client/static/img/favicon-16x16.png
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/gui/client/static/img/favicon-32x32.png
--rw-r--r--   0 runner    (1001) docker     (127)     2885 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/gui/client/static/img/gpt.png
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/gui/client/static/img/site.webmanifest
--rw-r--r--   0 runner    (1001) docker     (127)    17004 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/gui/client/static/img/user.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:04:54.042946 g4f-0.2.8.0/g4f/gui/client/static/js/
--rw-r--r--   0 runner    (1001) docker     (127)    34997 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/gui/client/static/js/chat.v1.js
--rw-r--r--   0 runner    (1001) docker     (127)   118841 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/gui/client/static/js/highlight.min.js
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/gui/client/static/js/highlightjs-copy.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    10865 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/gui/client/static/js/icons.js
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/gui/run.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:04:54.046947 g4f-0.2.8.0/g4f/gui/server/
--rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/gui/server/android_gallery.py
--rw-r--r--   0 runner    (1001) docker     (127)     9675 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/gui/server/api.py
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/gui/server/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     3688 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/gui/server/backend.py
--rw-r--r--   0 runner    (1001) docker     (127)    15354 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/gui/server/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4918 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/gui/server/internet.py
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/gui/server/website.py
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/gui/webview.py
--rw-r--r--   0 runner    (1001) docker     (127)     8399 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/image.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:04:54.046947 g4f-0.2.8.0/g4f/local/
--rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/local/_engine.py
--rw-r--r--   0 runner    (1001) docker     (127)     2959 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/local/_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     7472 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:04:54.046947 g4f-0.2.8.0/g4f/providers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9260 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/providers/base_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/providers/conversation.py
--rw-r--r--   0 runner    (1001) docker     (127)     6594 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/providers/create_images.py
--rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/providers/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     6869 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/providers/retry_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     3083 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/providers/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:04:54.046947 g4f-0.2.8.0/g4f/requests/
--rw-r--r--   0 runner    (1001) docker     (127)     3959 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/requests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/requests/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (127)     3016 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/requests/curl_cffi.py
--rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/requests/defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/requests/raise_for_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     2938 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/stubs.py
--rw-r--r--   0 runner    (1001) docker     (127)      875 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/typing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3855 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     9961 2024-04-05 19:04:50.000000 g4f-0.2.8.0/g4f/webdriver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:04:54.046947 g4f-0.2.8.0/g4f.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    42097 2024-04-05 19:04:53.000000 g4f-0.2.8.0/g4f.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5452 2024-04-05 19:04:54.000000 g4f-0.2.8.0/g4f.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 19:04:53.000000 g4f-0.2.8.0/g4f.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-05 19:04:53.000000 g4f-0.2.8.0/g4f.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-05 19:04:53.000000 g4f-0.2.8.0/g4f.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-05 19:04:53.000000 g4f-0.2.8.0/g4f.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 19:04:54.054947 g4f-0.2.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3646 2024-04-05 19:04:50.000000 g4f-0.2.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 09:30:48.404399 g4f-0.2.8.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    35148 2024-04-07 09:30:44.000000 g4f-0.2.8.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-07 09:30:44.000000 g4f-0.2.8.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    49027 2024-04-07 09:30:48.404399 g4f-0.2.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    45911 2024-04-07 09:30:44.000000 g4f-0.2.8.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 09:30:48.372399 g4f-0.2.8.1/g4f/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 09:30:48.376399 g4f-0.2.8.1/g4f/Provider/
+-rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-04-07 09:30:44.000000 g4f-0.2.8.1/g4f/Provider/Aura.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20635 2024-04-07 09:30:44.000000 g4f-0.2.8.1/g4f/Provider/Bing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2193 2024-04-07 09:30:44.000000 g4f-0.2.8.1/g4f/Provider/BingCreateImages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-04-07 09:30:44.000000 g4f-0.2.8.1/g4f/Provider/ChatForAi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2653 2024-04-07 09:30:44.000000 g4f-0.2.8.1/g4f/Provider/Chatgpt4Online.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3608 2024-04-07 09:30:44.000000 g4f-0.2.8.1/g4f/Provider/ChatgptAi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2866 2024-04-07 09:30:44.000000 g4f-0.2.8.1/g4f/Provider/ChatgptFree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2503 2024-04-07 09:30:44.000000 g4f-0.2.8.1/g4f/Provider/ChatgptNext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4278 2024-04-07 09:30:44.000000 g4f-0.2.8.1/g4f/Provider/ChatgptX.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-04-07 09:30:44.000000 g4f-0.2.8.1/g4f/Provider/DeepInfra.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3116 2024-04-07 09:30:44.000000 g4f-0.2.8.1/g4f/Provider/FlowGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-04-07 09:30:44.000000 g4f-0.2.8.1/g4f/Provider/FreeChatgpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-04-07 09:30:44.000000 g4f-0.2.8.1/g4f/Provider/FreeGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3985 2024-04-07 09:30:44.000000 g4f-0.2.8.1/g4f/Provider/GeminiPro.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2572 2024-04-07 09:30:44.000000 g4f-0.2.8.1/g4f/Provider/GeminiProChat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3922 2024-04-07 09:30:44.000000 g4f-0.2.8.1/g4f/Provider/GigaChat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-04-07 09:30:44.000000 g4f-0.2.8.1/g4f/Provider/GptTalkRu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3998 2024-04-07 09:30:44.000000 g4f-0.2.8.1/g4f/Provider/HuggingChat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2940 2024-04-07 09:30:44.000000 g4f-0.2.8.1/g4f/Provider/HuggingFace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2485 2024-04-07 09:30:44.000000 g4f-0.2.8.1/g4f/Provider/Koala.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5006 2024-04-07 09:30:44.000000 g4f-0.2.8.1/g4f/Provider/Liaobots.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3234 2024-04-07 09:30:44.000000 g4f-0.2.8.1/g4f/Provider/Llama2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-04-07 09:30:44.000000 g4f-0.2.8.1/g4f/Provider/Local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3951 2024-04-07 09:30:44.000000 g4f-0.2.8.1/g4f/Provider/PerplexityLabs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-04-07 09:30:44.000000 g4f-0.2.8.1/g4f/Provider/Pi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4042 2024-04-07 09:30:44.000000 g4f-0.2.8.1/g4f/Provider/Vercel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7450 2024-04-07 09:30:44.000000 g4f-0.2.8.1/g4f/Provider/You.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-04-07 09:30:44.000000 g4f-0.2.8.1/g4f/Provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-07 09:30:44.000000 g4f-0.2.8.1/g4f/Provider/base_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 09:30:48.380399 g4f-0.2.8.1/g4f/Provider/bing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 09:30:44.000000 g4f-0.2.8.1/g4f/Provider/bing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3541 2024-04-07 09:30:44.000000 g4f-0.2.8.1/g4f/Provider/bing/conversation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7597 2024-04-07 09:30:44.000000 g4f-0.2.8.1/g4f/Provider/bing/create_images.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4746 2024-04-07 09:30:44.000000 g4f-0.2.8.1/g4f/Provider/bing/upload_image.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 09:30:48.384399 g4f-0.2.8.1/g4f/Provider/deprecated/
+-rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-04-07 09:30:44.000000 g4f-0.2.8.1/g4f/Provider/deprecated/Acytoo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-04-07 09:30:44.000000 g4f-0.2.8.1/g4f/Provider/deprecated/AiAsk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-04-07 09:30:44.000000 g4f-0.2.8.1/g4f/Provider/deprecated/AiChatOnline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-04-07 09:30:45.000000 g4f-0.2.8.1/g4f/Provider/deprecated/AiService.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-04-07 09:30:45.000000 g4f-0.2.8.1/g4f/Provider/deprecated/Aibn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-04-07 09:30:45.000000 g4f-0.2.8.1/g4f/Provider/deprecated/Aichat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3358 2024-04-07 09:30:45.000000 g4f-0.2.8.1/g4f/Provider/deprecated/Ails.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2952 2024-04-07 09:30:45.000000 g4f-0.2.8.1/g4f/Provider/deprecated/Aivvm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-04-07 09:30:45.000000 g4f-0.2.8.1/g4f/Provider/deprecated/Berlin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-04-07 09:30:45.000000 g4f-0.2.8.1/g4f/Provider/deprecated/ChatAnywhere.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-04-07 09:30:45.000000 g4f-0.2.8.1/g4f/Provider/deprecated/ChatgptDuo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-04-07 09:30:45.000000 g4f-0.2.8.1/g4f/Provider/deprecated/CodeLinkAva.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-04-07 09:30:45.000000 g4f-0.2.8.1/g4f/Provider/deprecated/Cromicle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-04-07 09:30:45.000000 g4f-0.2.8.1/g4f/Provider/deprecated/DfeHub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3398 2024-04-07 09:30:45.000000 g4f-0.2.8.1/g4f/Provider/deprecated/EasyChat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2755 2024-04-07 09:30:45.000000 g4f-0.2.8.1/g4f/Provider/deprecated/Equing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-04-07 09:30:45.000000 g4f-0.2.8.1/g4f/Provider/deprecated/FakeGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-04-07 09:30:45.000000 g4f-0.2.8.1/g4f/Provider/deprecated/FastGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-07 09:30:45.000000 g4f-0.2.8.1/g4f/Provider/deprecated/Forefront.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3552 2024-04-07 09:30:45.000000 g4f-0.2.8.1/g4f/Provider/deprecated/GPTalk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2658 2024-04-07 09:30:45.000000 g4f-0.2.8.1/g4f/Provider/deprecated/GeekGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-04-07 09:30:45.000000 g4f-0.2.8.1/g4f/Provider/deprecated/GetGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2925 2024-04-07 09:30:45.000000 g4f-0.2.8.1/g4f/Provider/deprecated/H2o.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-04-07 09:30:45.000000 g4f-0.2.8.1/g4f/Provider/deprecated/Hashnode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-04-07 09:30:45.000000 g4f-0.2.8.1/g4f/Provider/deprecated/Lockchat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5050 2024-04-07 09:30:45.000000 g4f-0.2.8.1/g4f/Provider/deprecated/Myshell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2500 2024-04-07 09:30:45.000000 g4f-0.2.8.1/g4f/Provider/deprecated/NoowAi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-04-07 09:30:45.000000 g4f-0.2.8.1/g4f/Provider/deprecated/Opchatgpts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3308 2024-04-07 09:30:45.000000 g4f-0.2.8.1/g4f/Provider/deprecated/OpenAssistant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5353 2024-04-07 09:30:45.000000 g4f-0.2.8.1/g4f/Provider/deprecated/Phind.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-04-07 09:30:45.000000 g4f-0.2.8.1/g4f/Provider/deprecated/V50.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12167 2024-04-07 09:30:45.000000 g4f-0.2.8.1/g4f/Provider/deprecated/Vercel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-04-07 09:30:45.000000 g4f-0.2.8.1/g4f/Provider/deprecated/Vitalentum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3415 2024-04-07 09:30:45.000000 g4f-0.2.8.1/g4f/Provider/deprecated/VoiGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2464 2024-04-07 09:30:45.000000 g4f-0.2.8.1/g4f/Provider/deprecated/Wewordle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-04-07 09:30:45.000000 g4f-0.2.8.1/g4f/Provider/deprecated/Wuguokai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-04-07 09:30:45.000000 g4f-0.2.8.1/g4f/Provider/deprecated/Ylokh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-04-07 09:30:45.000000 g4f-0.2.8.1/g4f/Provider/deprecated/Yqcloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-07 09:30:45.000000 g4f-0.2.8.1/g4f/Provider/deprecated/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 09:30:48.384399 g4f-0.2.8.1/g4f/Provider/gigachat_crt/
+-rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-04-07 09:30:45.000000 g4f-0.2.8.1/g4f/Provider/gigachat_crt/russian_trusted_root_ca_pem.crt
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-07 09:30:45.000000 g4f-0.2.8.1/g4f/Provider/helper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 09:30:48.384399 g4f-0.2.8.1/g4f/Provider/needs_auth/
+-rw-r--r--   0 runner    (1001) docker     (127)     8802 2024-04-07 09:30:45.000000 g4f-0.2.8.1/g4f/Provider/needs_auth/Gemini.py
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-04-07 09:30:45.000000 g4f-0.2.8.1/g4f/Provider/needs_auth/Groq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4173 2024-04-07 09:30:45.000000 g4f-0.2.8.1/g4f/Provider/needs_auth/Openai.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30021 2024-04-07 09:30:45.000000 g4f-0.2.8.1/g4f/Provider/needs_auth/OpenaiChat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4289 2024-04-07 09:30:45.000000 g4f-0.2.8.1/g4f/Provider/needs_auth/Poe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-04-07 09:30:45.000000 g4f-0.2.8.1/g4f/Provider/needs_auth/Raycast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5465 2024-04-07 09:30:45.000000 g4f-0.2.8.1/g4f/Provider/needs_auth/Theb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-04-07 09:30:45.000000 g4f-0.2.8.1/g4f/Provider/needs_auth/ThebApi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-07 09:30:45.000000 g4f-0.2.8.1/g4f/Provider/needs_auth/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 09:30:48.388399 g4f-0.2.8.1/g4f/Provider/not_working/
+-rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-04-07 09:30:45.000000 g4f-0.2.8.1/g4f/Provider/not_working/AItianhu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-04-07 09:30:45.000000 g4f-0.2.8.1/g4f/Provider/not_working/Bestim.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4546 2024-04-07 09:30:45.000000 g4f-0.2.8.1/g4f/Provider/not_working/ChatBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2863 2024-04-07 09:30:45.000000 g4f-0.2.8.1/g4f/Provider/not_working/ChatgptDemo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-04-07 09:30:45.000000 g4f-0.2.8.1/g4f/Provider/not_working/ChatgptDemoAi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3056 2024-04-07 09:30:45.000000 g4f-0.2.8.1/g4f/Provider/not_working/ChatgptLogin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-04-07 09:30:45.000000 g4f-0.2.8.1/g4f/Provider/not_working/Chatxyz.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-04-07 09:30:45.000000 g4f-0.2.8.1/g4f/Provider/not_working/Gpt6.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-04-07 09:30:45.000000 g4f-0.2.8.1/g4f/Provider/not_working/GptChatly.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3529 2024-04-07 09:30:45.000000 g4f-0.2.8.1/g4f/Provider/not_working/GptForLove.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-04-07 09:30:45.000000 g4f-0.2.8.1/g4f/Provider/not_working/GptGo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-04-07 09:30:45.000000 g4f-0.2.8.1/g4f/Provider/not_working/GptGod.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-04-07 09:30:45.000000 g4f-0.2.8.1/g4f/Provider/not_working/OnlineGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-07 09:30:45.000000 g4f-0.2.8.1/g4f/Provider/not_working/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 09:30:48.388399 g4f-0.2.8.1/g4f/Provider/npm/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 09:30:48.388399 g4f-0.2.8.1/g4f/Provider/npm/node_modules/
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-07 09:30:45.000000 g4f-0.2.8.1/g4f/Provider/npm/node_modules/.package-lock.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 09:30:48.388399 g4f-0.2.8.1/g4f/Provider/npm/node_modules/crypto-js/
+-rw-r--r--   0 runner    (1001) docker     (127)     6449 2024-04-07 09:30:45.000000 g4f-0.2.8.1/g4f/Provider/npm/node_modules/crypto-js/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)   219092 2024-04-07 09:30:45.000000 g4f-0.2.8.1/g4f/Provider/npm/node_modules/crypto-js/crypto-js.js
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-07 09:30:45.000000 g4f-0.2.8.1/g4f/Provider/npm/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-07 09:30:45.000000 g4f-0.2.8.1/g4f/Provider/npm/package.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 09:30:48.388399 g4f-0.2.8.1/g4f/Provider/openai/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 09:30:45.000000 g4f-0.2.8.1/g4f/Provider/openai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-04-07 09:30:45.000000 g4f-0.2.8.1/g4f/Provider/openai/crypt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4649 2024-04-07 09:30:45.000000 g4f-0.2.8.1/g4f/Provider/openai/har_file.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 09:30:48.392399 g4f-0.2.8.1/g4f/Provider/selenium/
+-rw-r--r--   0 runner    (1001) docker     (127)     3839 2024-04-07 09:30:45.000000 g4f-0.2.8.1/g4f/Provider/selenium/AItianhuSpace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2859 2024-04-07 09:30:45.000000 g4f-0.2.8.1/g4f/Provider/selenium/Bard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-04-07 09:30:45.000000 g4f-0.2.8.1/g4f/Provider/selenium/MyShell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-04-07 09:30:45.000000 g4f-0.2.8.1/g4f/Provider/selenium/PerplexityAi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3655 2024-04-07 09:30:45.000000 g4f-0.2.8.1/g4f/Provider/selenium/Phind.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2678 2024-04-07 09:30:45.000000 g4f-0.2.8.1/g4f/Provider/selenium/TalkAi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-07 09:30:45.000000 g4f-0.2.8.1/g4f/Provider/selenium/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 09:30:48.392399 g4f-0.2.8.1/g4f/Provider/unfinished/
+-rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-04-07 09:30:45.000000 g4f-0.2.8.1/g4f/Provider/unfinished/AiChatting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-04-07 09:30:45.000000 g4f-0.2.8.1/g4f/Provider/unfinished/ChatAiGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-04-07 09:30:45.000000 g4f-0.2.8.1/g4f/Provider/unfinished/Komo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3298 2024-04-07 09:30:45.000000 g4f-0.2.8.1/g4f/Provider/unfinished/MikuChat.py
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-07 09:30:45.000000 g4f-0.2.8.1/g4f/Provider/unfinished/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 09:30:48.392399 g4f-0.2.8.1/g4f/Provider/you/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 09:30:45.000000 g4f-0.2.8.1/g4f/Provider/you/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2451 2024-04-07 09:30:45.000000 g4f-0.2.8.1/g4f/Provider/you/har_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6848 2024-04-07 09:30:45.000000 g4f-0.2.8.1/g4f/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 09:30:48.392399 g4f-0.2.8.1/g4f/api/
+-rw-r--r--   0 runner    (1001) docker     (127)     6084 2024-04-07 09:30:45.000000 g4f-0.2.8.1/g4f/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2024-04-07 09:30:45.000000 g4f-0.2.8.1/g4f/api/_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-07 09:30:45.000000 g4f-0.2.8.1/g4f/api/_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-07 09:30:45.000000 g4f-0.2.8.1/g4f/api/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-04-07 09:30:45.000000 g4f-0.2.8.1/g4f/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 09:30:48.392399 g4f-0.2.8.1/g4f/client/
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-07 09:30:45.000000 g4f-0.2.8.1/g4f/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7397 2024-04-07 09:30:45.000000 g4f-0.2.8.1/g4f/client/async_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6378 2024-04-07 09:30:45.000000 g4f-0.2.8.1/g4f/client/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-07 09:30:45.000000 g4f-0.2.8.1/g4f/client/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-07 09:30:45.000000 g4f-0.2.8.1/g4f/client/image_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4500 2024-04-07 09:30:45.000000 g4f-0.2.8.1/g4f/client/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2938 2024-04-07 09:30:45.000000 g4f-0.2.8.1/g4f/client/stubs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-04-07 09:30:45.000000 g4f-0.2.8.1/g4f/client/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3406 2024-04-07 09:30:45.000000 g4f-0.2.8.1/g4f/cookies.py
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-07 09:30:45.000000 g4f-0.2.8.1/g4f/debug.py
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-07 09:30:45.000000 g4f-0.2.8.1/g4f/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 09:30:48.392399 g4f-0.2.8.1/g4f/gui/
+-rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-04-07 09:30:45.000000 g4f-0.2.8.1/g4f/gui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 09:30:48.392399 g4f-0.2.8.1/g4f/gui/client/
+-rw-r--r--   0 runner    (1001) docker     (127)    10964 2024-04-07 09:30:45.000000 g4f-0.2.8.1/g4f/gui/client/index.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 09:30:48.368399 g4f-0.2.8.1/g4f/gui/client/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 09:30:48.392399 g4f-0.2.8.1/g4f/gui/client/static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)    20915 2024-04-07 09:30:45.000000 g4f-0.2.8.1/g4f/gui/client/static/css/style.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 09:30:48.396399 g4f-0.2.8.1/g4f/gui/client/static/img/
+-rw-r--r--   0 runner    (1001) docker     (127)     8908 2024-04-07 09:30:45.000000 g4f-0.2.8.1/g4f/gui/client/static/img/android-chrome-192x192.png
+-rw-r--r--   0 runner    (1001) docker     (127)    17626 2024-04-07 09:30:45.000000 g4f-0.2.8.1/g4f/gui/client/static/img/android-chrome-512x512.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7984 2024-04-07 09:30:45.000000 g4f-0.2.8.1/g4f/gui/client/static/img/apple-touch-icon.png
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-07 09:30:45.000000 g4f-0.2.8.1/g4f/gui/client/static/img/favicon-16x16.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-04-07 09:30:45.000000 g4f-0.2.8.1/g4f/gui/client/static/img/favicon-32x32.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2885 2024-04-07 09:30:45.000000 g4f-0.2.8.1/g4f/gui/client/static/img/gpt.png
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-07 09:30:45.000000 g4f-0.2.8.1/g4f/gui/client/static/img/site.webmanifest
+-rw-r--r--   0 runner    (1001) docker     (127)    17004 2024-04-07 09:30:45.000000 g4f-0.2.8.1/g4f/gui/client/static/img/user.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 09:30:48.396399 g4f-0.2.8.1/g4f/gui/client/static/js/
+-rw-r--r--   0 runner    (1001) docker     (127)    34997 2024-04-07 09:30:45.000000 g4f-0.2.8.1/g4f/gui/client/static/js/chat.v1.js
+-rw-r--r--   0 runner    (1001) docker     (127)   118841 2024-04-07 09:30:45.000000 g4f-0.2.8.1/g4f/gui/client/static/js/highlight.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-07 09:30:45.000000 g4f-0.2.8.1/g4f/gui/client/static/js/highlightjs-copy.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    10865 2024-04-07 09:30:45.000000 g4f-0.2.8.1/g4f/gui/client/static/js/icons.js
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-07 09:30:45.000000 g4f-0.2.8.1/g4f/gui/gui_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-07 09:30:45.000000 g4f-0.2.8.1/g4f/gui/run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 09:30:48.396399 g4f-0.2.8.1/g4f/gui/server/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 09:30:45.000000 g4f-0.2.8.1/g4f/gui/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-04-07 09:30:45.000000 g4f-0.2.8.1/g4f/gui/server/android_gallery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6101 2024-04-07 09:30:45.000000 g4f-0.2.8.1/g4f/gui/server/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-07 09:30:45.000000 g4f-0.2.8.1/g4f/gui/server/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3688 2024-04-07 09:30:45.000000 g4f-0.2.8.1/g4f/gui/server/backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15354 2024-04-07 09:30:45.000000 g4f-0.2.8.1/g4f/gui/server/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4918 2024-04-07 09:30:45.000000 g4f-0.2.8.1/g4f/gui/server/internet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3268 2024-04-07 09:30:45.000000 g4f-0.2.8.1/g4f/gui/server/js_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-04-07 09:30:45.000000 g4f-0.2.8.1/g4f/gui/server/website.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-04-07 09:30:45.000000 g4f-0.2.8.1/g4f/gui/webview.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8399 2024-04-07 09:30:45.000000 g4f-0.2.8.1/g4f/image.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 09:30:48.396399 g4f-0.2.8.1/g4f/local/
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-04-07 09:30:45.000000 g4f-0.2.8.1/g4f/local/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 09:30:48.396399 g4f-0.2.8.1/g4f/locals/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 09:30:45.000000 g4f-0.2.8.1/g4f/locals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-04-07 09:30:45.000000 g4f-0.2.8.1/g4f/locals/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2710 2024-04-07 09:30:45.000000 g4f-0.2.8.1/g4f/locals/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7472 2024-04-07 09:30:45.000000 g4f-0.2.8.1/g4f/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 09:30:48.400399 g4f-0.2.8.1/g4f/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 09:30:45.000000 g4f-0.2.8.1/g4f/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9347 2024-04-07 09:30:45.000000 g4f-0.2.8.1/g4f/providers/base_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-07 09:30:45.000000 g4f-0.2.8.1/g4f/providers/conversation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6594 2024-04-07 09:30:45.000000 g4f-0.2.8.1/g4f/providers/create_images.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-04-07 09:30:45.000000 g4f-0.2.8.1/g4f/providers/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6869 2024-04-07 09:30:45.000000 g4f-0.2.8.1/g4f/providers/retry_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3217 2024-04-07 09:30:45.000000 g4f-0.2.8.1/g4f/providers/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 09:30:48.400399 g4f-0.2.8.1/g4f/requests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3959 2024-04-07 09:30:45.000000 g4f-0.2.8.1/g4f/requests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-04-07 09:30:45.000000 g4f-0.2.8.1/g4f/requests/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3016 2024-04-07 09:30:45.000000 g4f-0.2.8.1/g4f/requests/curl_cffi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-04-07 09:30:45.000000 g4f-0.2.8.1/g4f/requests/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-04-07 09:30:45.000000 g4f-0.2.8.1/g4f/requests/raise_for_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2938 2024-04-07 09:30:45.000000 g4f-0.2.8.1/g4f/stubs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      875 2024-04-07 09:30:45.000000 g4f-0.2.8.1/g4f/typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3855 2024-04-07 09:30:45.000000 g4f-0.2.8.1/g4f/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9961 2024-04-07 09:30:45.000000 g4f-0.2.8.1/g4f/webdriver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 09:30:48.400399 g4f-0.2.8.1/g4f.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    49027 2024-04-07 09:30:48.000000 g4f-0.2.8.1/g4f.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5864 2024-04-07 09:30:48.000000 g4f-0.2.8.1/g4f.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 09:30:48.000000 g4f-0.2.8.1/g4f.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-07 09:30:48.000000 g4f-0.2.8.1/g4f.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-07 09:30:48.000000 g4f-0.2.8.1/g4f.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-07 09:30:48.000000 g4f-0.2.8.1/g4f.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 09:30:48.404399 g4f-0.2.8.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3646 2024-04-07 09:30:45.000000 g4f-0.2.8.1/setup.py
```

### Comparing `g4f-0.2.8.0/LICENSE` & `g4f-0.2.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.0/PKG-INFO` & `g4f-0.2.8.1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,83 +1,7 @@
-Metadata-Version: 2.1
-Name: g4f
-Version: 0.2.8.0
-Summary: The official gpt4free repository | various collection of powerful language models
-Home-page: https://github.com/xtekky/gpt4free
-Author: Tekky
-Author-email: <support@g4f.ai>
-Project-URL: Source Code, https://github.com/xtekky/gpt4free
-Project-URL: Bug Tracker, https://github.com/xtekky/gpt4free/issues
-Keywords: python,chatbot,reverse-engineering,openai,chatbots,gpt,language-model,gpt-3,gpt3,openai-api,gpt-4,gpt4,chatgpt,chatgpt-api,openai-chatgpt,chatgpt-free,chatgpt-4,chatgpt4,chatgpt4-api,free,free-gpt,gpt4free,g4f
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: Unix
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: Microsoft :: Windows
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: requests
-Requires-Dist: aiohttp
-Requires-Dist: brotli
-Requires-Dist: pycryptodome
-Provides-Extra: all
-Requires-Dist: curl_cffi>=0.6.2; extra == "all"
-Requires-Dist: certifi; extra == "all"
-Requires-Dist: browser_cookie3; extra == "all"
-Requires-Dist: PyExecJS; extra == "all"
-Requires-Dist: duckduckgo-search>=5.0; extra == "all"
-Requires-Dist: beautifulsoup4; extra == "all"
-Requires-Dist: brotli; extra == "all"
-Requires-Dist: pywebview; extra == "all"
-Requires-Dist: platformdirs; extra == "all"
-Requires-Dist: plyer; extra == "all"
-Requires-Dist: cryptography; extra == "all"
-Requires-Dist: aiohttp_socks; extra == "all"
-Requires-Dist: pillow; extra == "all"
-Requires-Dist: cairosvg; extra == "all"
-Requires-Dist: werkzeug; extra == "all"
-Requires-Dist: flask; extra == "all"
-Requires-Dist: loguru; extra == "all"
-Requires-Dist: fastapi; extra == "all"
-Requires-Dist: uvicorn; extra == "all"
-Requires-Dist: nest_asyncio; extra == "all"
-Requires-Dist: pycryptodome; extra == "all"
-Provides-Extra: image
-Requires-Dist: pillow; extra == "image"
-Requires-Dist: cairosvg; extra == "image"
-Requires-Dist: beautifulsoup4; extra == "image"
-Provides-Extra: webdriver
-Requires-Dist: platformdirs; extra == "webdriver"
-Requires-Dist: undetected-chromedriver>=3.5.5; extra == "webdriver"
-Requires-Dist: setuptools; extra == "webdriver"
-Requires-Dist: selenium-wire; extra == "webdriver"
-Provides-Extra: webview
-Requires-Dist: webview; extra == "webview"
-Requires-Dist: platformdirs; extra == "webview"
-Requires-Dist: plyer; extra == "webview"
-Requires-Dist: cryptography; extra == "webview"
-Provides-Extra: openai
-Requires-Dist: pycryptodome; extra == "openai"
-Provides-Extra: api
-Requires-Dist: loguru; extra == "api"
-Requires-Dist: fastapi; extra == "api"
-Requires-Dist: uvicorn; extra == "api"
-Requires-Dist: nest_asyncio; extra == "api"
-Provides-Extra: gui
-Requires-Dist: werkzeug; extra == "gui"
-Requires-Dist: flask; extra == "gui"
-Requires-Dist: beautifulsoup4; extra == "gui"
-Requires-Dist: pillow; extra == "gui"
-Requires-Dist: duckduckgo-search>=5.0; extra == "gui"
-Requires-Dist: browser_cookie3; extra == "gui"
-Provides-Extra: local
-Requires-Dist: gpt4all; extra == "local"
-
-
 ![248433934-7886223b-c1d1-4260-82aa-da5741f303bb](https://github.com/xtekky/gpt4free/assets/98614666/ea012c87-76e0-496a-8ac4-e2de090cc6c9)
 
 <a href="https://trendshift.io/repositories/1692" target="_blank"><img src="https://trendshift.io/api/badge/repositories/1692" alt="xtekky%2Fgpt4free | Trendshift" style="width: 250px; height: 55px;" width="250" height="55"/></a>
 
 Written by [@xtekky](https://github.com/hlohaus) & maintained by [@hlohaus](https://github.com/hlohaus)
 
 <div id="top"></div>
@@ -96,43 +20,43 @@
 ```
 ```sh
 docker pull hlohaus789/g4f
 ```
 
 ## 🆕 What's New
 
-- Check out a more in depth local inference @ https://github.com/gpt4free/gpt4local
-- Join our Telegram Channel: [t.me/g4f_channel](https://telegram.me/g4f_channel)
-- Join our Discord Group: [discord.gg/XfybzPXPH5](https://discord.gg/XfybzPXPH5)
-- `g4f` now supports 100% local inference: [local-docs](https://g4f.mintlify.app/docs/core/usage/local)
+- Installation Guide for Windows (.exe): 💻 [#installation-guide-for-windows](#installation-guide-for-windows-exe)
+- Join our Telegram Channel: 📨 [telegram.me/g4f_channel](https://telegram.me/g4f_channel)
+- Join our Discord Group: 💬 [discord.gg/XfybzPXPH5](https://discord.gg/XfybzPXPH5)
+- `g4f` now supports 100% local inference: 🧠 [local-docs](https://g4f.mintlify.app/docs/core/usage/local)
 
 ## 🔻 Site Takedown
-Is your site on this repository and you want to take it down? Send an email to takedown@g4f.ai with proof it is yours and it will be removed as fast as possible. To prevent reproduction please secure your API ;)
+Is your site on this repository and you want to take it down? Send an email to takedown@g4f.ai with proof it is yours and it will be removed as fast as possible. To prevent reproduction please secure your API. 😉
 
 ## 🚀  Feedback and Todo
 You can always leave some feedback here: https://forms.gle/FeWV9RLEedfdkmFN6
 
 As per the survey, here is a list of improvements to come
 - [x] Update the repository to include the new openai library syntax (ex: `Openai()` class) | completed, use `g4f.client.Client`
 - [ ] Golang implementation
 - [ ] 🚧 Improve Documentation (in /docs & Guides, Howtos, & Do video tutorials)
 - [x] Improve the provider status list & updates
 - [ ] Tutorials on how to reverse sites to write your own wrapper (PoC only ofc)
 - [x] Improve the Bing wrapper. (Wait and Retry or reuse conversation)
-- [ ] Write a standard provider performance test to improve the stability
+- [ ] 🚧 Write a standard provider performance test to improve the stability
 - [ ] Potential support and development of local models
 - [ ] 🚧 Improve compatibility and error handling
 
 ## 📚 Table of Contents
 
 - [🆕 What's New](#-whats-new)
 - [📚 Table of Contents](#-table-of-contents)
 - [🛠️ Getting Started](#-getting-started)
-    + [Docker container](#docker-container)
-      - [Quick start](#quick-start)
+    + [Docker Container Guide](#docker-container-guide)
+    + [Installation Guide for Windows (.exe)](#installation-guide-for-windows-exe)
     + [Use python](#use-python)
       - [Prerequisites](#prerequisites)
       - [Install using PyPI package:](#install-using-pypi-package)
       - [Install from source:](#install-from-source)
       - [Install using Docker:](#install-using-docker)
 - [💡 Usage](#-usage)
   * [Text Generation](#text-generation)
@@ -152,28 +76,49 @@
 - [🙌 Contributors](#-contributors)
 - [©️ Copyright](#-copyright)
 - [⭐ Star History](#-star-history)
 - [📄 License](#-license)
 
 ## 🛠️ Getting Started
 
-#### Docker container
+#### Docker Container Guide
+
+##### Getting Started Quickly:
 
-##### Quick start:
+1. **Install Docker:** Begin by [downloading and installing Docker](https://docs.docker.com/get-docker/).
 
-1. [Download and install Docker](https://docs.docker.com/get-docker/)
-2. Pull latest image and run the container:
+2. **Set Up the Container:**
+   Use the following commands to pull the latest image and start the container:
 
 ```sh
 docker pull hlohaus789/g4f
 docker run -p 8080:8080 -p 1337:1337 -p 7900:7900 --shm-size="2g" -v ${PWD}/hardir:/app/hardir hlohaus789/g4f:latest
 ```
-3. Open the included client on: [http://localhost:8080/chat/](http://localhost:8080/chat/)
-or set the API base in your client to: [http://localhost:1337/v1](http://localhost:1337/v1)
-4. (Optional) If you need to log in to a provider, you can view the desktop from the container here: http://localhost:7900/?autoconnect=1&resize=scale&password=secret.
+
+3. **Access the Client:** 
+   - To use the included client, navigate to: [http://localhost:8080/chat/](http://localhost:8080/chat/)
+   - Or set the API base for your client to: [http://localhost:1337/v1](http://localhost:1337/v1)
+
+4. **(Optional) Provider Login:**
+   If required, you can access the container's desktop here: http://localhost:7900/?autoconnect=1&resize=scale&password=secret for provider login purposes.
+
+#### Installation Guide for Windows (.exe)
+To ensure the seamless operation of our application, please follow the instructions below. These steps are designed to guide you through the installation process on Windows operating systems.
+##### Prerequisites
+1. **WebView2 Runtime**: Our application requires the *WebView2 Runtime* to be installed on your system. If you do not have it installed, please download and install it from the [Microsoft Developer Website](https://developer.microsoft.com/en-us/microsoft-edge/webview2/). If you already have *WebView2 Runtime* installed but are encountering issues, navigate to *Installed Windows Apps*, select *WebView2*, and opt for the repair option.
+##### Installation Steps
+2. **Download the Application**: Visit our [latest releases page](https://github.com/xtekky/gpt4free/releases/latest) and download the most recent version of the application, named `g4f.webview.*.exe`.
+3. **File Placement**: Once downloaded, transfer the `.exe` file from your downloads folder to a directory of your choice on your system, and then execute it to run the app.
+##### Post-Installation Adjustment
+4. **Firewall Configuration (Hotfix)**: Upon installation, it may be necessary to adjust your Windows Firewall settings to allow the application to operate correctly. To do this, access your Windows Firewall settings and allow the application.
+
+By following these steps, you should be able to successfully install and run the application on your Windows system. If you encounter any issues during the installation process, please refer to our Issue Tracker or try to get contact over Discord for assistance.
+
+Run the **Webview UI** on other Platfroms:
+- [/docs/guides/webview](/docs/webview.md)
 
 ##### Use your smartphone:
 
 Run the Web UI on Your Smartphone:
 - [/docs/guides/phone](/docs/guides/phone.md)
 
 #### Use python
@@ -242,59 +187,34 @@
 [![Image with cat](/docs/cat.jpeg)](/docs/client.md)
 
 **Full Documentation for Python API**
 
 - New Client API like the OpenAI Python library: [/docs/client](/docs/client.md)
 - Legacy API with python modules: [/docs/legacy](/docs/legacy.md)
 
-### Webview GUI
-
-Open the GUI in a window of your OS. Runs on a local/static/ssl server and use a JavaScript API.
-Supports login into the OpenAI Chat, Image Upload and streamed Text Generation.
-
-Supports all platforms, but only Linux tested.
-
-1. Install all requirements with:
-
-```bash
-pip install g4f[webview]
-```
-
-2. Follow the OS specific steps here:
- [pywebview installation](https://pywebview.flowrl.com/guide/installation.html#dependencies)
-
-3. Run the app with:
-
-```python
-from g4f.gui.webview import run_webview
-run_webview(debug=True)
-```
-or execute the following command:
-```bash
-python -m g4f.gui.webview -debug
-```
-
-#### Webserver
+#### Web UI
 
 To start the web interface, type the following codes in python:
 
 ```python
 from g4f.gui import run_gui
 run_gui()
 ```
 or execute the following command:
 ```bash
 python -m g4f.cli gui -port 8080 -debug
 ```
 
-### Interference API
+#### Interference API
 
 You can use the Interference API to serve other OpenAI integrations with G4F.
 
-See: [/docs/interference](/docs/interference.md)
+See docs: [/docs/interference](/docs/interference.md)
+
+Access with: http://localhost:1337/v1
 
 ### Configuration
 
 #### Cookies
 
 You need cookies for BingCreateImages and the Gemini Provider.
 From Bing you need the "_U" cookie and from Gemini you need the "__Secure-1PSID" cookie.
@@ -319,15 +239,15 @@
 
 To utilize the OpenaiChat provider, a .har file is required from https://chat.openai.com/. Follow the steps below to create a valid .har file:
 
 1. Navigate to https://chat.openai.com/ using your preferred web browser and log in with your credentials.
 2. Access the Developer Tools in your browser. This can typically be done by right-clicking the page and selecting "Inspect," or by pressing F12 or Ctrl+Shift+I (Cmd+Option+I on a Mac).
 3. With the Developer Tools open, switch to the "Network" tab.
 4. Reload the website to capture the loading process within the Network tab.
-5. Initiate an action in the chat which can be capture in the .har file.
+5. Initiate an action in the chat which can be captured in the .har file.
 6. Right-click any of the network activities listed and select "Save all as HAR with content" to export the .har file.
 
 ##### Storing the .HAR File
 
 - Place the exported .har file in the `./hardir` directory if you are using Docker. Alternatively, you can store it in any preferred location within your current working directory.
 
 Note: Ensure that your .har file is stored securely, as it may contain sensitive information.
@@ -852,17 +772,58 @@
 
 ###### Guide: How can AI help me with writing code?
 
  - Read: [/docs/guides/help_me](/docs/guides/help_me.md)
 
 ## 🙌 Contributors
 
-A list of all contributors is available [here](https://github.com/xtekky/gpt4free/graphs/contributors)   
-The [`Vercel.py`](https://github.com/xtekky/gpt4free/blob/main/g4f/Provider/Vercel.py) file contains code from [vercel-llm-api](https://github.com/ading2210/vercel-llm-api) by [@ading2210](https://github.com/ading2210), which is licensed under the [GNU GPL v3](https://www.gnu.org/licenses/gpl-3.0.txt)   
-Top 1 Contributor: [@hlohaus](https://github.com/hlohaus)
+A list of all contributors is available [here](https://github.com/xtekky/gpt4free/graphs/contributors)
+
+<a href="https://github.com/xtekky" target="_blank"><img src="https://avatars.githubusercontent.com/u/98614666?v=4&s=45" width="45" title="xtekky"></a>
+<a href="https://github.com/hlohaus" target="_blank"><img src="https://avatars.githubusercontent.com/u/983577?v=4&s=45" width="45" title="hlohaus"></a>
+<a href="https://github.com/bagusindrayana" target="_blank"><img src="https://avatars.githubusercontent.com/u/36830534?v=4&s=45" width="45" title="bagusindrayana"></a>
+<a href="https://github.com/sudouser777" target="_blank"><img src="https://avatars.githubusercontent.com/u/22415463?v=4&s=45" width="45" title="sudouser777"></a>
+<a href="https://github.com/thatlukinhasguy1" target="_blank"><img src="https://avatars.githubusercontent.com/u/139662282?v=4&s=45" width="45" title="thatlukinhasguy1"></a>
+<a href="https://github.com/Commenter123321" target="_blank"><img src="https://avatars.githubusercontent.com/u/36051603?v=4&s=45" width="45" title="Commenter123321"></a>
+<a href="https://github.com/DanielShemesh" target="_blank"><img src="https://avatars.githubusercontent.com/u/20585236?v=4&s=45" width="45" title="DanielShemesh"></a>
+<a href="https://github.com/Luneye" target="_blank"><img src="https://avatars.githubusercontent.com/u/73485421?v=4&s=45" width="45" title="Luneye"></a>
+<a href="https://github.com/enganese" target="_blank"><img src="https://avatars.githubusercontent.com/u/69082498?v=4&s=45" width="45" title="enganese"></a>
+<a href="https://github.com/ezerinz" target="_blank"><img src="https://avatars.githubusercontent.com/u/100193740?v=4&s=45" width="45" title="ezerinz"></a>
+<a href="https://github.com/Lin-jun-xiang" target="_blank"><img src="https://avatars.githubusercontent.com/u/63782903?v=4&s=45" width="45" title="Lin-jun-xiang"></a>
+<a href="https://github.com/nullstreak" target="_blank"><img src="https://avatars.githubusercontent.com/u/139914347?v=4&s=45" width="45" title="nullstreak"></a>
+<a href="https://github.com/valerii-chirkov" target="_blank"><img src="https://avatars.githubusercontent.com/u/81074936?v=4&s=45" width="45" title="valerii-chirkov"></a>
+<a href="https://github.com/MIDORIBIN" target="_blank"><img src="https://avatars.githubusercontent.com/u/25425217?v=4&s=45" width="45" title="MIDORIBIN"></a>
+<a href="https://github.com/repollo" target="_blank"><img src="https://avatars.githubusercontent.com/u/2671466?v=4&s=45" width="45" title="repollo"></a>
+<a href="https://github.com/hpsj" target="_blank"><img src="https://avatars.githubusercontent.com/u/54535414?v=4&s=45" width="45" title="hpsj"></a>
+<a href="https://github.com/taiyi747" target="_blank"><img src="https://avatars.githubusercontent.com/u/63543716?v=4&s=45" width="45" title="taiyi747"></a>
+<a href="https://github.com/ostix360" target="_blank"><img src="https://avatars.githubusercontent.com/u/55257054?v=4&s=45" width="45" title="ostix360"></a>
+<a href="https://github.com/WdR-Tech" target="_blank"><img src="https://avatars.githubusercontent.com/u/143020293?v=4&s=45" width="45" title="WdR-Tech"></a>
+<a href="https://github.com/HexyeDEV" target="_blank"><img src="https://avatars.githubusercontent.com/u/65314629?v=4&s=45" width="45" title="HexyeDEV"></a>
+<a href="https://github.com/9fo" target="_blank"><img src="https://avatars.githubusercontent.com/u/71867245?v=4&s=45" width="45" title="9fo"></a>
+<a href="https://github.com/eltociear" target="_blank"><img src="https://avatars.githubusercontent.com/u/22633385?v=4&s=45" width="45" title="eltociear"></a>
+<a href="https://github.com/ramonvc" target="_blank"><img src="https://avatars.githubusercontent.com/u/13617054?v=4&s=45" width="45" title="ramonvc"></a>
+<a href="https://github.com/naa7" target="_blank"><img src="https://avatars.githubusercontent.com/u/44613678?v=4&s=45" width="45" title="naa7"></a>
+<a href="https://github.com/zeng-rr" target="_blank"><img src="https://avatars.githubusercontent.com/u/47846202?v=4&s=45" width="45" title="zeng-rr"></a>
+<a href="https://github.com/editor-syntax" target="_blank"><img src="https://avatars.githubusercontent.com/u/109844019?v=4&s=45" width="45" title="editor-syntax"></a>
+<a href="https://github.com/devAdityaa" target="_blank"><img src="https://avatars.githubusercontent.com/u/77636021?v=4&s=45" width="45" title="devAdityaa"></a>
+<a href="https://github.com/kggn" target="_blank"><img src="https://avatars.githubusercontent.com/u/95663228?v=4&s=45" width="45" title="kggn"></a>
+<a href="https://github.com/xiangsx" target="_blank"><img src="https://avatars.githubusercontent.com/u/29322721?v=4&s=45" width="45" title="xiangsx"></a>
+<a href="https://github.com/ggindinson" target="_blank"><img src="https://avatars.githubusercontent.com/u/97807772?v=4&s=45" width="45" title="ggindinson"></a>
+<span></span>
+<img src="https://avatars.githubusercontent.com/u/71154407?s=45&v=4" width="45" title="ading2210">
+<img src="https://avatars.githubusercontent.com/u/12299238?s=45&v=4" width="45" title="xqdoo00o">
+<img src="https://avatars.githubusercontent.com/u/97126670?s=45&v=4" width="45" title="nathanrchn">
+<img src="https://avatars.githubusercontent.com/u/81407603?v=4&s=45" width="45" title="dsdanielpark">
+
+- The [`Vercel.py`](g4f/Provider/Vercel.py) file contains code from [vercel-llm-api](https://github.com/ading2210/vercel-llm-api) by [@ading2210](https://github.com/ading2210)
+- The [`har_file.py`](g4f/Provider/openai/har_file.py) has input from [xqdoo00o/ChatGPT-to-API](https://github.com/xqdoo00o/ChatGPT-to-API)
+- The [`PerplexityLabs.py`](g4f/Provider/openai/har_file.py) has input from [nathanrchn/perplexityai](https://github.com/nathanrchn/perplexityai)
+- The [`Gemini.py`](g4f/Provider/needs_auth/Gemini.py) has input from [dsdanielpark/Gemini-API](https://github.com/dsdanielpark/Gemini-API)
+
+*Having input implies that the AI's code generation utilized it as one of many sources.*
 
 ## ©️ Copyright
 
 This program is licensed under the [GNU GPL v3](https://www.gnu.org/licenses/gpl-3.0.txt)
 
 ```
 xtekky/gpt4free: Copyright (C) 2023 xtekky
```

#### html2text {}

```diff
@@ -1,52 +1,11 @@
-Metadata-Version: 2.1 Name: g4f Version: 0.2.8.0 Summary: The official gpt4free
-repository | various collection of powerful language models Home-page: https://
-github.com/xtekky/gpt4free Author: Tekky Author-email:
-g4f.ai> Project-URL: Source Code, https://github.com/xtekky/gpt4free Project-
-URL: Bug Tracker, https://github.com/xtekky/gpt4free/issues Keywords:
-python,chatbot,reverse-engineering,openai,chatbots,gpt,language-model,gpt-
-3,gpt3,openai-api,gpt-4,gpt4,chatgpt,chatgpt-api,openai-chatgpt,chatgpt-
-free,chatgpt-4,chatgpt4,chatgpt4-api,free,free-gpt,gpt4free,g4f Classifier:
-Development Status :: 2 - Pre-Alpha Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3 Classifier: Operating System ::
-Unix Classifier: Operating System :: MacOS :: MacOS X Classifier: Operating
-System :: Microsoft :: Windows Description-Content-Type: text/markdown License-
-File: LICENSE Requires-Dist: requests Requires-Dist: aiohttp Requires-Dist:
-brotli Requires-Dist: pycryptodome Provides-Extra: all Requires-Dist:
-curl_cffi>=0.6.2; extra == "all" Requires-Dist: certifi; extra == "all"
-Requires-Dist: browser_cookie3; extra == "all" Requires-Dist: PyExecJS; extra
-== "all" Requires-Dist: duckduckgo-search>=5.0; extra == "all" Requires-Dist:
-beautifulsoup4; extra == "all" Requires-Dist: brotli; extra == "all" Requires-
-Dist: pywebview; extra == "all" Requires-Dist: platformdirs; extra == "all"
-Requires-Dist: plyer; extra == "all" Requires-Dist: cryptography; extra ==
-"all" Requires-Dist: aiohttp_socks; extra == "all" Requires-Dist: pillow; extra
-== "all" Requires-Dist: cairosvg; extra == "all" Requires-Dist: werkzeug; extra
-== "all" Requires-Dist: flask; extra == "all" Requires-Dist: loguru; extra ==
-"all" Requires-Dist: fastapi; extra == "all" Requires-Dist: uvicorn; extra ==
-"all" Requires-Dist: nest_asyncio; extra == "all" Requires-Dist: pycryptodome;
-extra == "all" Provides-Extra: image Requires-Dist: pillow; extra == "image"
-Requires-Dist: cairosvg; extra == "image" Requires-Dist: beautifulsoup4; extra
-== "image" Provides-Extra: webdriver Requires-Dist: platformdirs; extra ==
-"webdriver" Requires-Dist: undetected-chromedriver>=3.5.5; extra == "webdriver"
-Requires-Dist: setuptools; extra == "webdriver" Requires-Dist: selenium-wire;
-extra == "webdriver" Provides-Extra: webview Requires-Dist: webview; extra ==
-"webview" Requires-Dist: platformdirs; extra == "webview" Requires-Dist: plyer;
-extra == "webview" Requires-Dist: cryptography; extra == "webview" Provides-
-Extra: openai Requires-Dist: pycryptodome; extra == "openai" Provides-Extra:
-api Requires-Dist: loguru; extra == "api" Requires-Dist: fastapi; extra ==
-"api" Requires-Dist: uvicorn; extra == "api" Requires-Dist: nest_asyncio; extra
-== "api" Provides-Extra: gui Requires-Dist: werkzeug; extra == "gui" Requires-
-Dist: flask; extra == "gui" Requires-Dist: beautifulsoup4; extra == "gui"
-Requires-Dist: pillow; extra == "gui" Requires-Dist: duckduckgo-search>=5.0;
-extra == "gui" Requires-Dist: browser_cookie3; extra == "gui" Provides-Extra:
-local Requires-Dist: gpt4all; extra == "local" ![248433934-7886223b-c1d1-4260-
-82aa-da5741f303bb](https://github.com/xtekky/gpt4free/assets/98614666/ea012c87-
-76e0-496a-8ac4-e2de090cc6c9) _[_x_t_e_k_k_y_%_2_F_g_p_t_4_f_r_e_e_ _|_ _T_r_e_n_d_s_h_i_f_t_]Written by
-[@xtekky](https://github.com/hlohaus) & maintained by [@hlohaus](https://
-github.com/hlohaus)
+![248433934-7886223b-c1d1-4260-82aa-da5741f303bb](https://github.com/xtekky/
+gpt4free/assets/98614666/ea012c87-76e0-496a-8ac4-e2de090cc6c9)
+_[_x_t_e_k_k_y_%_2_F_g_p_t_4_f_r_e_e_ _|_ _T_r_e_n_d_s_h_i_f_t_]Written by [@xtekky](https://github.com/
+hlohaus) & maintained by [@hlohaus](https://github.com/hlohaus)
 > By using this repository or any code related to it, you agree to the [legal
 notice](LEGAL_NOTICE.md). The author is **not responsible for the usage of this
 repository nor endorses it**, nor is the author responsible for any copies,
 forks, re-uploads made by other users, or anything else related to GPT4Free.
 This is the author's only account and repository. To prevent impersonation or
 irresponsible actions, please comply with the GNU GPL license this Repository
 uses. > [!Warning] *"gpt4free"* serves as a **PoC** (proof of concept),
@@ -54,139 +13,159 @@
 with features like timeouts, load balance and flow control. > [!Note] LLaasstteett
 vveerrssiioonn:: [![PyPI version](https://img.shields.io/pypi/v/g4f?color=blue)](https:
 //pypi.org/project/g4f) [![Docker version](https://img.shields.io/docker/v/
 hlohaus789/g4f?label=docker&color=blue)](https://hub.docker.com/r/hlohaus789/
 g4f) > SSttaattss:: [![Downloads](https://static.pepy.tech/badge/g4f)](https://
 pepy.tech/project/g4f) [![Downloads](https://static.pepy.tech/badge/g4f/month)]
 (https://pepy.tech/project/g4f) ```sh pip install -U g4f ``` ```sh docker pull
-hlohaus789/g4f ``` ## ð What's New - Check out a more in depth local
-inference @ https://github.com/gpt4free/gpt4local - Join our Telegram Channel:
-[t.me/g4f_channel](https://telegram.me/g4f_channel) - Join our Discord Group:
-[discord.gg/XfybzPXPH5](https://discord.gg/XfybzPXPH5) - `g4f` now supports
-100% local inference: [local-docs](https://g4f.mintlify.app/docs/core/usage/
-local) ## ð» Site Takedown Is your site on this repository and you want to
-take it down? Send an email to takedown@g4f.ai with proof it is yours and it
-will be removed as fast as possible. To prevent reproduction please secure your
-API ;) ## ð Feedback and Todo You can always leave some feedback here:
-https://forms.gle/FeWV9RLEedfdkmFN6 As per the survey, here is a list of
-improvements to come - [x] Update the repository to include the new openai
-library syntax (ex: `Openai()` class) | completed, use `g4f.client.Client` -
-[ ] Golang implementation - [ ] ð§ Improve Documentation (in /docs & Guides,
-Howtos, & Do video tutorials) - [x] Improve the provider status list & updates
-- [ ] Tutorials on how to reverse sites to write your own wrapper (PoC only
-ofc) - [x] Improve the Bing wrapper. (Wait and Retry or reuse conversation) -
-[ ] Write a standard provider performance test to improve the stability - [ ]
-Potential support and development of local models - [ ] ð§ Improve
-compatibility and error handling ## ð Table of Contents - [ð What's New]
-(#-whats-new) - [ð Table of Contents](#-table-of-contents) - [ð ï¸
-Getting Started](#-getting-started) + [Docker container](#docker-container) -
-[Quick start](#quick-start) + [Use python](#use-python) - [Prerequisites]
-(#prerequisites) - [Install using PyPI package:](#install-using-pypi-package) -
-[Install from source:](#install-from-source) - [Install using Docker:]
-(#install-using-docker) - [ð¡ Usage](#-usage) * [Text Generation](#text-
-generation) * [Image Generation](#image-generation) * [Web UI](#web-ui) *
-[Interference API](#interference-api) * [Configuration](#configuration) - [ð
-Providers and Models](#-providers-and-models) * [GPT-4](#gpt-4) * [GPT-3.5]
-(#gpt-35) * [Other](#other) * [Models](#models) - [ð Powered by gpt4free](#-
-powered-by-gpt4free) - [ð¤ Contribute](#-contribute) + [How do i create a new
-Provider?](#guide-how-do-i-create-a-new-provider) + [How can AI help me with
-writing code?](#guide-how-can-ai-help-me-with-writing-code) - [ð
-Contributors](#-contributors) - [Â©ï¸ Copyright](#-copyright) - [â­ Star
-History](#-star-history) - [ð License](#-license) ## ð ï¸ Getting Started
-#### Docker container ##### Quick start: 1. [Download and install Docker]
-(https://docs.docker.com/get-docker/) 2. Pull latest image and run the
+hlohaus789/g4f ``` ## ð What's New - Installation Guide for Windows (.exe):
+ð» [#installation-guide-for-windows](#installation-guide-for-windows-exe) -
+Join our Telegram Channel: ð¨ [telegram.me/g4f_channel](https://telegram.me/
+g4f_channel) - Join our Discord Group: ð¬ [discord.gg/XfybzPXPH5](https://
+discord.gg/XfybzPXPH5) - `g4f` now supports 100% local inference: ð§  [local-
+docs](https://g4f.mintlify.app/docs/core/usage/local) ## ð» Site Takedown Is
+your site on this repository and you want to take it down? Send an email to
+takedown@g4f.ai with proof it is yours and it will be removed as fast as
+possible. To prevent reproduction please secure your API. ð ## ð Feedback
+and Todo You can always leave some feedback here: https://forms.gle/
+FeWV9RLEedfdkmFN6 As per the survey, here is a list of improvements to come -
+[x] Update the repository to include the new openai library syntax (ex: `Openai
+()` class) | completed, use `g4f.client.Client` - [ ] Golang implementation -
+[ ] ð§ Improve Documentation (in /docs & Guides, Howtos, & Do video
+tutorials) - [x] Improve the provider status list & updates - [ ] Tutorials on
+how to reverse sites to write your own wrapper (PoC only ofc) - [x] Improve the
+Bing wrapper. (Wait and Retry or reuse conversation) - [ ] ð§ Write a
+standard provider performance test to improve the stability - [ ] Potential
+support and development of local models - [ ] ð§ Improve compatibility and
+error handling ## ð Table of Contents - [ð What's New](#-whats-new) -
+[ð Table of Contents](#-table-of-contents) - [ð ï¸ Getting Started](#-
+getting-started) + [Docker Container Guide](#docker-container-guide) +
+[Installation Guide for Windows (.exe)](#installation-guide-for-windows-exe) +
+[Use python](#use-python) - [Prerequisites](#prerequisites) - [Install using
+PyPI package:](#install-using-pypi-package) - [Install from source:](#install-
+from-source) - [Install using Docker:](#install-using-docker) - [ð¡ Usage](#-
+usage) * [Text Generation](#text-generation) * [Image Generation](#image-
+generation) * [Web UI](#web-ui) * [Interference API](#interference-api) *
+[Configuration](#configuration) - [ð Providers and Models](#-providers-and-
+models) * [GPT-4](#gpt-4) * [GPT-3.5](#gpt-35) * [Other](#other) * [Models]
+(#models) - [ð Powered by gpt4free](#-powered-by-gpt4free) - [ð¤
+Contribute](#-contribute) + [How do i create a new Provider?](#guide-how-do-i-
+create-a-new-provider) + [How can AI help me with writing code?](#guide-how-
+can-ai-help-me-with-writing-code) - [ð Contributors](#-contributors) -
+[Â©ï¸ Copyright](#-copyright) - [â­ Star History](#-star-history) - [ð
+License](#-license) ## ð ï¸ Getting Started #### Docker Container Guide
+##### Getting Started Quickly: 1. **Install Docker:** Begin by [downloading and
+installing Docker](https://docs.docker.com/get-docker/). 2. **Set Up the
+Container:** Use the following commands to pull the latest image and start the
 container: ```sh docker pull hlohaus789/g4f docker run -p 8080:8080 -p 1337:
 1337 -p 7900:7900 --shm-size="2g" -v ${PWD}/hardir:/app/hardir hlohaus789/g4f:
-latest ``` 3. Open the included client on: [http://localhost:8080/chat/](http:/
-/localhost:8080/chat/) or set the API base in your client to: [http://
-localhost:1337/v1](http://localhost:1337/v1) 4. (Optional) If you need to log
-in to a provider, you can view the desktop from the container here: http://
-localhost:7900/?autoconnect=1&resize=scale&password=secret. ##### Use your
-smartphone: Run the Web UI on Your Smartphone: - [/docs/guides/phone](/docs/
-guides/phone.md) #### Use python ##### Prerequisites: 1. [Download and install
-Python](https://www.python.org/downloads/) (Version 3.10+ is recommended). 2.
-[Install Google Chrome](https://www.google.com/chrome/) for providers with
-webdriver ##### Install using PyPI package: ``` pip install -U g4f[all] ``` How
-do I install only parts or do disable parts? Use partial requirements: [/docs/
-requirements](/docs/requirements.md) ##### Install from source: How do I load
-the project using git and installing the project requirements? Read this
-tutorial and follow it step by step: [/docs/git](/docs/git.md) ##### Install
-using Docker: How do I build and run composer image from source? Use docker-
-compose: [/docs/docker](/docs/docker.md) ## ð¡ Usage #### Text Generation
-```python from g4f.client import Client client = Client() response =
+latest ``` 3. **Access the Client:** - To use the included client, navigate to:
+[http://localhost:8080/chat/](http://localhost:8080/chat/) - Or set the API
+base for your client to: [http://localhost:1337/v1](http://localhost:1337/v1)
+4. **(Optional) Provider Login:** If required, you can access the container's
+desktop here: http://localhost:7900/?autoconnect=1&resize=scale&password=secret
+for provider login purposes. #### Installation Guide for Windows (.exe) To
+ensure the seamless operation of our application, please follow the
+instructions below. These steps are designed to guide you through the
+installation process on Windows operating systems. ##### Prerequisites 1.
+**WebView2 Runtime**: Our application requires the *WebView2 Runtime* to be
+installed on your system. If you do not have it installed, please download and
+install it from the [Microsoft Developer Website](https://
+developer.microsoft.com/en-us/microsoft-edge/webview2/). If you already have
+*WebView2 Runtime* installed but are encountering issues, navigate to
+*Installed Windows Apps*, select *WebView2*, and opt for the repair option.
+##### Installation Steps 2. **Download the Application**: Visit our [latest
+releases page](https://github.com/xtekky/gpt4free/releases/latest) and download
+the most recent version of the application, named `g4f.webview.*.exe`. 3.
+**File Placement**: Once downloaded, transfer the `.exe` file from your
+downloads folder to a directory of your choice on your system, and then execute
+it to run the app. ##### Post-Installation Adjustment 4. **Firewall
+Configuration (Hotfix)**: Upon installation, it may be necessary to adjust your
+Windows Firewall settings to allow the application to operate correctly. To do
+this, access your Windows Firewall settings and allow the application. By
+following these steps, you should be able to successfully install and run the
+application on your Windows system. If you encounter any issues during the
+installation process, please refer to our Issue Tracker or try to get contact
+over Discord for assistance. Run the **Webview UI** on other Platfroms: - [/
+docs/guides/webview](/docs/webview.md) ##### Use your smartphone: Run the Web
+UI on Your Smartphone: - [/docs/guides/phone](/docs/guides/phone.md) #### Use
+python ##### Prerequisites: 1. [Download and install Python](https://
+www.python.org/downloads/) (Version 3.10+ is recommended). 2. [Install Google
+Chrome](https://www.google.com/chrome/) for providers with webdriver #####
+Install using PyPI package: ``` pip install -U g4f[all] ``` How do I install
+only parts or do disable parts? Use partial requirements: [/docs/requirements]
+(/docs/requirements.md) ##### Install from source: How do I load the project
+using git and installing the project requirements? Read this tutorial and
+follow it step by step: [/docs/git](/docs/git.md) ##### Install using Docker:
+How do I build and run composer image from source? Use docker-compose: [/docs/
+docker](/docs/docker.md) ## ð¡ Usage #### Text Generation ```python from
+g4f.client import Client client = Client() response =
 client.chat.completions.create( model="gpt-3.5-turbo", messages=[{"role":
 "user", "content": "Hello"}], ... ) print(response.choices[0].message.content)
 ``` ``` Hello! How can I assist you today? ``` #### Image Generation ```python
 from g4f.client import Client client = Client() response =
 client.images.generate( model="gemini", prompt="a white siamese cat", ... )
 image_url = response.data[0].url ``` [![Image with cat](/docs/cat.jpeg)](/docs/
 client.md) **Full Documentation for Python API** - New Client API like the
 OpenAI Python library: [/docs/client](/docs/client.md) - Legacy API with python
-modules: [/docs/legacy](/docs/legacy.md) ### Webview GUI Open the GUI in a
-window of your OS. Runs on a local/static/ssl server and use a JavaScript API.
-Supports login into the OpenAI Chat, Image Upload and streamed Text Generation.
-Supports all platforms, but only Linux tested. 1. Install all requirements
-with: ```bash pip install g4f[webview] ``` 2. Follow the OS specific steps
-here: [pywebview installation](https://pywebview.flowrl.com/guide/
-installation.html#dependencies) 3. Run the app with: ```python from
-g4f.gui.webview import run_webview run_webview(debug=True) ``` or execute the
-following command: ```bash python -m g4f.gui.webview -debug ``` #### Webserver
-To start the web interface, type the following codes in python: ```python from
-g4f.gui import run_gui run_gui() ``` or execute the following command: ```bash
-python -m g4f.cli gui -port 8080 -debug ``` ### Interference API You can use
-the Interference API to serve other OpenAI integrations with G4F. See: [/docs/
-interference](/docs/interference.md) ### Configuration #### Cookies You need
-cookies for BingCreateImages and the Gemini Provider. From Bing you need the
-"_U" cookie and from Gemini you need the "__Secure-1PSID" cookie. Sometimes you
-doesn't need the "__Secure-1PSID" cookie, but some other auth cookies. You can
-pass the cookies in the create function or you use the `set_cookies` setter
-before you run G4F: ```python from g4f.cookies import set_cookies set_cookies
-(".bing.com", { "_U": "cookie value" }) set_cookies(".google.com", { "__Secure-
-1PSID": "cookie value" }) ... ``` #### .HAR File for OpenaiChat Provider #####
-Generating a .HAR File To utilize the OpenaiChat provider, a .har file is
-required from https://chat.openai.com/. Follow the steps below to create a
-valid .har file: 1. Navigate to https://chat.openai.com/ using your preferred
-web browser and log in with your credentials. 2. Access the Developer Tools in
-your browser. This can typically be done by right-clicking the page and
-selecting "Inspect," or by pressing F12 or Ctrl+Shift+I (Cmd+Option+I on a
-Mac). 3. With the Developer Tools open, switch to the "Network" tab. 4. Reload
-the website to capture the loading process within the Network tab. 5. Initiate
-an action in the chat which can be capture in the .har file. 6. Right-click any
-of the network activities listed and select "Save all as HAR with content" to
-export the .har file. ##### Storing the .HAR File - Place the exported .har
-file in the `./hardir` directory if you are using Docker. Alternatively, you
-can store it in any preferred location within your current working directory.
-Note: Ensure that your .har file is stored securely, as it may contain
-sensitive information. #### Using Proxy If you want to hide or change your IP
-address for the providers, you can set a proxy globally via an environment
-variable: - On macOS and Linux: ```bash export G4F_PROXY="http://host:port" ```
-- On Windows: ```bash set G4F_PROXY=http://host:port ``` ## ð Providers and
-Models ### GPT-4 | Website | Provider | GPT-3.5 | GPT-4 | Stream | Status |
-Auth | | ------ | ------- | ------- | ----- | ------ | ------ | ---- | |
-[bing.com](https://bing.com/chat) | `g4f.Provider.Bing` | â | âï¸ | âï¸
-| ![Unknown](https://img.shields.io/badge/Unknown-grey) | â | | [chatgpt.ai]
-(https://chatgpt.ai) | `g4f.Provider.ChatgptAi` | â | âï¸ | âï¸ | !
-[Active](https://img.shields.io/badge/Active-brightgreen) | â | |
-[liaobots.site](https://liaobots.site) | `g4f.Provider.Liaobots` | âï¸ |
-âï¸ | âï¸ | ![Active](https://img.shields.io/badge/Active-brightgreen) |
-â | | [chat.openai.com](https://chat.openai.com) | `g4f.Provider.OpenaiChat`
-| âï¸ | â | âï¸ | ![Unknown](https://img.shields.io/badge/Unknown-grey)
-| âï¸ | | [raycast.com](https://raycast.com) | `g4f.Provider.Raycast` |
-âï¸ | âï¸ | âï¸ | ![Unknown](https://img.shields.io/badge/Unknown-
-grey) | âï¸ | | [beta.theb.ai](https://beta.theb.ai) | `g4f.Provider.Theb` |
-âï¸ | âï¸ | âï¸ | ![Unknown](https://img.shields.io/badge/Unknown-
-grey) | â | | [you.com](https://you.com) | `g4f.Provider.You` | âï¸ |
-âï¸ | âï¸ | ![Unknown](https://img.shields.io/badge/Unknown-grey) | â |
-### GPT-3.5 | Website | Provider | GPT-3.5 | GPT-4 | Stream | Status | Auth | |
------- | ------- | ------- | ----- | ------ | ------ | ---- | |
-[chat3.aiyunos.top](https://chat3.aiyunos.top/) | `g4f.Provider.AItianhuSpace`
-| âï¸ | â | âï¸ | ![Unknown](https://img.shields.io/badge/Unknown-grey)
-| â | | [chatforai.store](https://chatforai.store) | `g4f.Provider.ChatForAi`
-| âï¸ | â | âï¸ | ![Active](https://img.shields.io/badge/Active-
-brightgreen) | â | | [chatgpt4online.org](https://chatgpt4online.org) |
+modules: [/docs/legacy](/docs/legacy.md) #### Web UI To start the web
+interface, type the following codes in python: ```python from g4f.gui import
+run_gui run_gui() ``` or execute the following command: ```bash python -
+m g4f.cli gui -port 8080 -debug ``` #### Interference API You can use the
+Interference API to serve other OpenAI integrations with G4F. See docs: [/docs/
+interference](/docs/interference.md) Access with: http://localhost:1337/v1 ###
+Configuration #### Cookies You need cookies for BingCreateImages and the Gemini
+Provider. From Bing you need the "_U" cookie and from Gemini you need the
+"__Secure-1PSID" cookie. Sometimes you doesn't need the "__Secure-1PSID"
+cookie, but some other auth cookies. You can pass the cookies in the create
+function or you use the `set_cookies` setter before you run G4F: ```python from
+g4f.cookies import set_cookies set_cookies(".bing.com", { "_U": "cookie value"
+}) set_cookies(".google.com", { "__Secure-1PSID": "cookie value" }) ... ```
+#### .HAR File for OpenaiChat Provider ##### Generating a .HAR File To utilize
+the OpenaiChat provider, a .har file is required from https://chat.openai.com/.
+Follow the steps below to create a valid .har file: 1. Navigate to https://
+chat.openai.com/ using your preferred web browser and log in with your
+credentials. 2. Access the Developer Tools in your browser. This can typically
+be done by right-clicking the page and selecting "Inspect," or by pressing F12
+or Ctrl+Shift+I (Cmd+Option+I on a Mac). 3. With the Developer Tools open,
+switch to the "Network" tab. 4. Reload the website to capture the loading
+process within the Network tab. 5. Initiate an action in the chat which can be
+captured in the .har file. 6. Right-click any of the network activities listed
+and select "Save all as HAR with content" to export the .har file. #####
+Storing the .HAR File - Place the exported .har file in the `./hardir`
+directory if you are using Docker. Alternatively, you can store it in any
+preferred location within your current working directory. Note: Ensure that
+your .har file is stored securely, as it may contain sensitive information.
+#### Using Proxy If you want to hide or change your IP address for the
+providers, you can set a proxy globally via an environment variable: - On macOS
+and Linux: ```bash export G4F_PROXY="http://host:port" ``` - On Windows:
+```bash set G4F_PROXY=http://host:port ``` ## ð Providers and Models ###
+GPT-4 | Website | Provider | GPT-3.5 | GPT-4 | Stream | Status | Auth | | -----
+- | ------- | ------- | ----- | ------ | ------ | ---- | | [bing.com](https://
+bing.com/chat) | `g4f.Provider.Bing` | â | âï¸ | âï¸ | ![Unknown]
+(https://img.shields.io/badge/Unknown-grey) | â | | [chatgpt.ai](https://
+chatgpt.ai) | `g4f.Provider.ChatgptAi` | â | âï¸ | âï¸ | ![Active]
+(https://img.shields.io/badge/Active-brightgreen) | â | | [liaobots.site]
+(https://liaobots.site) | `g4f.Provider.Liaobots` | âï¸ | âï¸ | âï¸ |
+![Active](https://img.shields.io/badge/Active-brightgreen) | â | |
+[chat.openai.com](https://chat.openai.com) | `g4f.Provider.OpenaiChat` | âï¸
+| â | âï¸ | ![Unknown](https://img.shields.io/badge/Unknown-grey) | âï¸
+| | [raycast.com](https://raycast.com) | `g4f.Provider.Raycast` | âï¸ |
+âï¸ | âï¸ | ![Unknown](https://img.shields.io/badge/Unknown-grey) |
+âï¸ | | [beta.theb.ai](https://beta.theb.ai) | `g4f.Provider.Theb` | âï¸
+| âï¸ | âï¸ | ![Unknown](https://img.shields.io/badge/Unknown-grey) | â
+| | [you.com](https://you.com) | `g4f.Provider.You` | âï¸ | âï¸ | âï¸
+| ![Unknown](https://img.shields.io/badge/Unknown-grey) | â | ### GPT-3.5 |
+Website | Provider | GPT-3.5 | GPT-4 | Stream | Status | Auth | | ------ | ----
+--- | ------- | ----- | ------ | ------ | ---- | | [chat3.aiyunos.top](https://
+chat3.aiyunos.top/) | `g4f.Provider.AItianhuSpace` | âï¸ | â | âï¸ | !
+[Unknown](https://img.shields.io/badge/Unknown-grey) | â | |
+[chatforai.store](https://chatforai.store) | `g4f.Provider.ChatForAi` | âï¸
+| â | âï¸ | ![Active](https://img.shields.io/badge/Active-brightgreen) |
+â | | [chatgpt4online.org](https://chatgpt4online.org) |
 `g4f.Provider.Chatgpt4Online` | âï¸ | â | âï¸ | ![Active](https://
 img.shields.io/badge/Active-brightgreen) | â | | [chatgpt-free.cc](https://
 www.chatgpt-free.cc) | `g4f.Provider.ChatgptNext` | âï¸ | â | âï¸ | !
 [Active](https://img.shields.io/badge/Active-brightgreen) | â | |
 [chatgptx.de](https://chatgptx.de) | `g4f.Provider.ChatgptX` | âï¸ | â |
 âï¸ | ![Active](https://img.shields.io/badge/Active-brightgreen) | â | |
 [flowgpt.com](https://flowgpt.com/chat) | `g4f.Provider.FlowGpt` | âï¸ | â
@@ -319,30 +298,68 @@
 improvements, your input is valued. Creating a pull request is all it takes â
 our co-pilot will handle the code review process. Once all changes have been
 addressed, we'll merge the pull request into the main branch and release the
 updates at a later time. ###### Guide: How do i create a new Provider? - Read:
 [/docs/guides/create_provider](/docs/guides/create_provider.md) ###### Guide:
 How can AI help me with writing code? - Read: [/docs/guides/help_me](/docs/
 guides/help_me.md) ## ð Contributors A list of all contributors is available
-[here](https://github.com/xtekky/gpt4free/graphs/contributors) The
-[`Vercel.py`](https://github.com/xtekky/gpt4free/blob/main/g4f/Provider/
-Vercel.py) file contains code from [vercel-llm-api](https://github.com/
-ading2210/vercel-llm-api) by [@ading2210](https://github.com/ading2210), which
-is licensed under the [GNU GPL v3](https://www.gnu.org/licenses/gpl-3.0.txt)
-Top 1 Contributor: [@hlohaus](https://github.com/hlohaus) ## Â©ï¸ Copyright
-This program is licensed under the [GNU GPL v3](https://www.gnu.org/licenses/
-gpl-3.0.txt) ``` xtekky/gpt4free: Copyright (C) 2023 xtekky This program is
-free software: you can redistribute it and/or modify it under the terms of the
-GNU General Public License as published by the Free Software Foundation, either
-version 3 of the License, or (at your option) any later version. This program
-is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
-without even the implied warranty of MERCHANTABILITY or FITNESS FOR A
-PARTICULAR PURPOSE. See the GNU General Public License for more details. You
-should have received a copy of the GNU General Public License along with this
-program. If not, see
+[here](https://github.com/xtekky/gpt4free/graphs/contributors) _[_h_t_t_p_s_:_/_/
+_a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_9_8_6_1_4_6_6_6_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
+_a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_9_8_3_5_7_7_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
+_a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_3_6_8_3_0_5_3_4_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
+_a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_2_2_4_1_5_4_6_3_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
+_a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_1_3_9_6_6_2_2_8_2_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
+_a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_3_6_0_5_1_6_0_3_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
+_a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_2_0_5_8_5_2_3_6_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
+_a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_7_3_4_8_5_4_2_1_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
+_a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_6_9_0_8_2_4_9_8_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
+_a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_1_0_0_1_9_3_7_4_0_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
+_a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_6_3_7_8_2_9_0_3_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
+_a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_1_3_9_9_1_4_3_4_7_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
+_a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_8_1_0_7_4_9_3_6_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
+_a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_2_5_4_2_5_2_1_7_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
+_a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_2_6_7_1_4_6_6_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
+_a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_5_4_5_3_5_4_1_4_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
+_a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_6_3_5_4_3_7_1_6_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
+_a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_5_5_2_5_7_0_5_4_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
+_a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_1_4_3_0_2_0_2_9_3_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
+_a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_6_5_3_1_4_6_2_9_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
+_a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_7_1_8_6_7_2_4_5_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
+_a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_2_2_6_3_3_3_8_5_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
+_a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_1_3_6_1_7_0_5_4_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
+_a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_4_4_6_1_3_6_7_8_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
+_a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_4_7_8_4_6_2_0_2_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
+_a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_1_0_9_8_4_4_0_1_9_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
+_a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_7_7_6_3_6_0_2_1_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
+_a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_9_5_6_6_3_2_2_8_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
+_a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_2_9_3_2_2_7_2_1_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
+_a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_9_7_8_0_7_7_7_2_?_v_=_4_&_s_=_4_5_][https://
+avatars.githubusercontent.com/u/71154407?s=45&v=4][https://
+avatars.githubusercontent.com/u/12299238?s=45&v=4][https://
+avatars.githubusercontent.com/u/97126670?s=45&v=4][https://
+avatars.githubusercontent.com/u/81407603?v=4&s=45]- The [`Vercel.py`](g4f/
+Provider/Vercel.py) file contains code from [vercel-llm-api](https://
+github.com/ading2210/vercel-llm-api) by [@ading2210](https://github.com/
+ading2210) - The [`har_file.py`](g4f/Provider/openai/har_file.py) has input
+from [xqdoo00o/ChatGPT-to-API](https://github.com/xqdoo00o/ChatGPT-to-API) -
+The [`PerplexityLabs.py`](g4f/Provider/openai/har_file.py) has input from
+[nathanrchn/perplexityai](https://github.com/nathanrchn/perplexityai) - The
+[`Gemini.py`](g4f/Provider/needs_auth/Gemini.py) has input from [dsdanielpark/
+Gemini-API](https://github.com/dsdanielpark/Gemini-API) *Having input implies
+that the AI's code generation utilized it as one of many sources.* ## Â©ï¸
+Copyright This program is licensed under the [GNU GPL v3](https://www.gnu.org/
+licenses/gpl-3.0.txt) ``` xtekky/gpt4free: Copyright (C) 2023 xtekky This
+program is free software: you can redistribute it and/or modify it under the
+terms of the GNU General Public License as published by the Free Software
+Foundation, either version 3 of the License, or (at your option) any later
+version. This program is distributed in the hope that it will be useful, but
+WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or
+FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more
+details. You should have received a copy of the GNU General Public License
+along with this program. If not, see
 www.gnu.org/licenses/>. ``` ## â­ Star History _[_S_t_a_r_ _H_i_s_t_o_r_y_ _C_h_a_r_t_]## ð
 License
 [https://upload.wikimedia.org/wikipedia/ [https://img.shields.io/badge/License-
    commons/thumb/9/93/GPLv3_Logo.svg/    GNU_GPL_v3.0-red.svg]
        1200px-GPLv3_Logo.svg.png]        This project is licensed under
                                          _G_N_U___G_P_L___v_3_._0.
                                                              (_ð___¼_ _B_a_c_k_ _t_o_ _t_o_p)
```

### Comparing `g4f-0.2.8.0/README.md` & `g4f-0.2.8.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,83 @@
+Metadata-Version: 2.1
+Name: g4f
+Version: 0.2.8.1
+Summary: The official gpt4free repository | various collection of powerful language models
+Home-page: https://github.com/xtekky/gpt4free
+Author: Tekky
+Author-email: <support@g4f.ai>
+Project-URL: Source Code, https://github.com/xtekky/gpt4free
+Project-URL: Bug Tracker, https://github.com/xtekky/gpt4free/issues
+Keywords: python,chatbot,reverse-engineering,openai,chatbots,gpt,language-model,gpt-3,gpt3,openai-api,gpt-4,gpt4,chatgpt,chatgpt-api,openai-chatgpt,chatgpt-free,chatgpt-4,chatgpt4,chatgpt4-api,free,free-gpt,gpt4free,g4f
+Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: Unix
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: Microsoft :: Windows
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: requests
+Requires-Dist: aiohttp
+Requires-Dist: brotli
+Requires-Dist: pycryptodome
+Provides-Extra: all
+Requires-Dist: curl_cffi>=0.6.2; extra == "all"
+Requires-Dist: certifi; extra == "all"
+Requires-Dist: browser_cookie3; extra == "all"
+Requires-Dist: PyExecJS; extra == "all"
+Requires-Dist: duckduckgo-search>=5.0; extra == "all"
+Requires-Dist: beautifulsoup4; extra == "all"
+Requires-Dist: brotli; extra == "all"
+Requires-Dist: pywebview; extra == "all"
+Requires-Dist: platformdirs; extra == "all"
+Requires-Dist: plyer; extra == "all"
+Requires-Dist: cryptography; extra == "all"
+Requires-Dist: aiohttp_socks; extra == "all"
+Requires-Dist: pillow; extra == "all"
+Requires-Dist: cairosvg; extra == "all"
+Requires-Dist: werkzeug; extra == "all"
+Requires-Dist: flask; extra == "all"
+Requires-Dist: loguru; extra == "all"
+Requires-Dist: fastapi; extra == "all"
+Requires-Dist: uvicorn; extra == "all"
+Requires-Dist: nest_asyncio; extra == "all"
+Requires-Dist: pycryptodome; extra == "all"
+Provides-Extra: image
+Requires-Dist: pillow; extra == "image"
+Requires-Dist: cairosvg; extra == "image"
+Requires-Dist: beautifulsoup4; extra == "image"
+Provides-Extra: webdriver
+Requires-Dist: platformdirs; extra == "webdriver"
+Requires-Dist: undetected-chromedriver>=3.5.5; extra == "webdriver"
+Requires-Dist: setuptools; extra == "webdriver"
+Requires-Dist: selenium-wire; extra == "webdriver"
+Provides-Extra: webview
+Requires-Dist: webview; extra == "webview"
+Requires-Dist: platformdirs; extra == "webview"
+Requires-Dist: plyer; extra == "webview"
+Requires-Dist: cryptography; extra == "webview"
+Provides-Extra: openai
+Requires-Dist: pycryptodome; extra == "openai"
+Provides-Extra: api
+Requires-Dist: loguru; extra == "api"
+Requires-Dist: fastapi; extra == "api"
+Requires-Dist: uvicorn; extra == "api"
+Requires-Dist: nest_asyncio; extra == "api"
+Provides-Extra: gui
+Requires-Dist: werkzeug; extra == "gui"
+Requires-Dist: flask; extra == "gui"
+Requires-Dist: beautifulsoup4; extra == "gui"
+Requires-Dist: pillow; extra == "gui"
+Requires-Dist: duckduckgo-search>=5.0; extra == "gui"
+Requires-Dist: browser_cookie3; extra == "gui"
+Provides-Extra: local
+Requires-Dist: gpt4all; extra == "local"
+
+
 ![248433934-7886223b-c1d1-4260-82aa-da5741f303bb](https://github.com/xtekky/gpt4free/assets/98614666/ea012c87-76e0-496a-8ac4-e2de090cc6c9)
 
 <a href="https://trendshift.io/repositories/1692" target="_blank"><img src="https://trendshift.io/api/badge/repositories/1692" alt="xtekky%2Fgpt4free | Trendshift" style="width: 250px; height: 55px;" width="250" height="55"/></a>
 
 Written by [@xtekky](https://github.com/hlohaus) & maintained by [@hlohaus](https://github.com/hlohaus)
 
 <div id="top"></div>
@@ -20,43 +96,43 @@
 ```
 ```sh
 docker pull hlohaus789/g4f
 ```
 
 ## 🆕 What's New
 
-- Check out a more in depth local inference @ https://github.com/gpt4free/gpt4local
-- Join our Telegram Channel: [t.me/g4f_channel](https://telegram.me/g4f_channel)
-- Join our Discord Group: [discord.gg/XfybzPXPH5](https://discord.gg/XfybzPXPH5)
-- `g4f` now supports 100% local inference: [local-docs](https://g4f.mintlify.app/docs/core/usage/local)
+- Installation Guide for Windows (.exe): 💻 [#installation-guide-for-windows](#installation-guide-for-windows-exe)
+- Join our Telegram Channel: 📨 [telegram.me/g4f_channel](https://telegram.me/g4f_channel)
+- Join our Discord Group: 💬 [discord.gg/XfybzPXPH5](https://discord.gg/XfybzPXPH5)
+- `g4f` now supports 100% local inference: 🧠 [local-docs](https://g4f.mintlify.app/docs/core/usage/local)
 
 ## 🔻 Site Takedown
-Is your site on this repository and you want to take it down? Send an email to takedown@g4f.ai with proof it is yours and it will be removed as fast as possible. To prevent reproduction please secure your API ;)
+Is your site on this repository and you want to take it down? Send an email to takedown@g4f.ai with proof it is yours and it will be removed as fast as possible. To prevent reproduction please secure your API. 😉
 
 ## 🚀  Feedback and Todo
 You can always leave some feedback here: https://forms.gle/FeWV9RLEedfdkmFN6
 
 As per the survey, here is a list of improvements to come
 - [x] Update the repository to include the new openai library syntax (ex: `Openai()` class) | completed, use `g4f.client.Client`
 - [ ] Golang implementation
 - [ ] 🚧 Improve Documentation (in /docs & Guides, Howtos, & Do video tutorials)
 - [x] Improve the provider status list & updates
 - [ ] Tutorials on how to reverse sites to write your own wrapper (PoC only ofc)
 - [x] Improve the Bing wrapper. (Wait and Retry or reuse conversation)
-- [ ] Write a standard provider performance test to improve the stability
+- [ ] 🚧 Write a standard provider performance test to improve the stability
 - [ ] Potential support and development of local models
 - [ ] 🚧 Improve compatibility and error handling
 
 ## 📚 Table of Contents
 
 - [🆕 What's New](#-whats-new)
 - [📚 Table of Contents](#-table-of-contents)
 - [🛠️ Getting Started](#-getting-started)
-    + [Docker container](#docker-container)
-      - [Quick start](#quick-start)
+    + [Docker Container Guide](#docker-container-guide)
+    + [Installation Guide for Windows (.exe)](#installation-guide-for-windows-exe)
     + [Use python](#use-python)
       - [Prerequisites](#prerequisites)
       - [Install using PyPI package:](#install-using-pypi-package)
       - [Install from source:](#install-from-source)
       - [Install using Docker:](#install-using-docker)
 - [💡 Usage](#-usage)
   * [Text Generation](#text-generation)
@@ -76,28 +152,49 @@
 - [🙌 Contributors](#-contributors)
 - [©️ Copyright](#-copyright)
 - [⭐ Star History](#-star-history)
 - [📄 License](#-license)
 
 ## 🛠️ Getting Started
 
-#### Docker container
+#### Docker Container Guide
+
+##### Getting Started Quickly:
 
-##### Quick start:
+1. **Install Docker:** Begin by [downloading and installing Docker](https://docs.docker.com/get-docker/).
 
-1. [Download and install Docker](https://docs.docker.com/get-docker/)
-2. Pull latest image and run the container:
+2. **Set Up the Container:**
+   Use the following commands to pull the latest image and start the container:
 
 ```sh
 docker pull hlohaus789/g4f
 docker run -p 8080:8080 -p 1337:1337 -p 7900:7900 --shm-size="2g" -v ${PWD}/hardir:/app/hardir hlohaus789/g4f:latest
 ```
-3. Open the included client on: [http://localhost:8080/chat/](http://localhost:8080/chat/)
-or set the API base in your client to: [http://localhost:1337/v1](http://localhost:1337/v1)
-4. (Optional) If you need to log in to a provider, you can view the desktop from the container here: http://localhost:7900/?autoconnect=1&resize=scale&password=secret.
+
+3. **Access the Client:** 
+   - To use the included client, navigate to: [http://localhost:8080/chat/](http://localhost:8080/chat/)
+   - Or set the API base for your client to: [http://localhost:1337/v1](http://localhost:1337/v1)
+
+4. **(Optional) Provider Login:**
+   If required, you can access the container's desktop here: http://localhost:7900/?autoconnect=1&resize=scale&password=secret for provider login purposes.
+
+#### Installation Guide for Windows (.exe)
+To ensure the seamless operation of our application, please follow the instructions below. These steps are designed to guide you through the installation process on Windows operating systems.
+##### Prerequisites
+1. **WebView2 Runtime**: Our application requires the *WebView2 Runtime* to be installed on your system. If you do not have it installed, please download and install it from the [Microsoft Developer Website](https://developer.microsoft.com/en-us/microsoft-edge/webview2/). If you already have *WebView2 Runtime* installed but are encountering issues, navigate to *Installed Windows Apps*, select *WebView2*, and opt for the repair option.
+##### Installation Steps
+2. **Download the Application**: Visit our [latest releases page](https://github.com/xtekky/gpt4free/releases/latest) and download the most recent version of the application, named `g4f.webview.*.exe`.
+3. **File Placement**: Once downloaded, transfer the `.exe` file from your downloads folder to a directory of your choice on your system, and then execute it to run the app.
+##### Post-Installation Adjustment
+4. **Firewall Configuration (Hotfix)**: Upon installation, it may be necessary to adjust your Windows Firewall settings to allow the application to operate correctly. To do this, access your Windows Firewall settings and allow the application.
+
+By following these steps, you should be able to successfully install and run the application on your Windows system. If you encounter any issues during the installation process, please refer to our Issue Tracker or try to get contact over Discord for assistance.
+
+Run the **Webview UI** on other Platfroms:
+- [/docs/guides/webview](/docs/webview.md)
 
 ##### Use your smartphone:
 
 Run the Web UI on Your Smartphone:
 - [/docs/guides/phone](/docs/guides/phone.md)
 
 #### Use python
@@ -166,59 +263,34 @@
 [![Image with cat](/docs/cat.jpeg)](/docs/client.md)
 
 **Full Documentation for Python API**
 
 - New Client API like the OpenAI Python library: [/docs/client](/docs/client.md)
 - Legacy API with python modules: [/docs/legacy](/docs/legacy.md)
 
-### Webview GUI
-
-Open the GUI in a window of your OS. Runs on a local/static/ssl server and use a JavaScript API.
-Supports login into the OpenAI Chat, Image Upload and streamed Text Generation.
-
-Supports all platforms, but only Linux tested.
-
-1. Install all requirements with:
-
-```bash
-pip install g4f[webview]
-```
-
-2. Follow the OS specific steps here:
- [pywebview installation](https://pywebview.flowrl.com/guide/installation.html#dependencies)
-
-3. Run the app with:
-
-```python
-from g4f.gui.webview import run_webview
-run_webview(debug=True)
-```
-or execute the following command:
-```bash
-python -m g4f.gui.webview -debug
-```
-
-#### Webserver
+#### Web UI
 
 To start the web interface, type the following codes in python:
 
 ```python
 from g4f.gui import run_gui
 run_gui()
 ```
 or execute the following command:
 ```bash
 python -m g4f.cli gui -port 8080 -debug
 ```
 
-### Interference API
+#### Interference API
 
 You can use the Interference API to serve other OpenAI integrations with G4F.
 
-See: [/docs/interference](/docs/interference.md)
+See docs: [/docs/interference](/docs/interference.md)
+
+Access with: http://localhost:1337/v1
 
 ### Configuration
 
 #### Cookies
 
 You need cookies for BingCreateImages and the Gemini Provider.
 From Bing you need the "_U" cookie and from Gemini you need the "__Secure-1PSID" cookie.
@@ -243,15 +315,15 @@
 
 To utilize the OpenaiChat provider, a .har file is required from https://chat.openai.com/. Follow the steps below to create a valid .har file:
 
 1. Navigate to https://chat.openai.com/ using your preferred web browser and log in with your credentials.
 2. Access the Developer Tools in your browser. This can typically be done by right-clicking the page and selecting "Inspect," or by pressing F12 or Ctrl+Shift+I (Cmd+Option+I on a Mac).
 3. With the Developer Tools open, switch to the "Network" tab.
 4. Reload the website to capture the loading process within the Network tab.
-5. Initiate an action in the chat which can be capture in the .har file.
+5. Initiate an action in the chat which can be captured in the .har file.
 6. Right-click any of the network activities listed and select "Save all as HAR with content" to export the .har file.
 
 ##### Storing the .HAR File
 
 - Place the exported .har file in the `./hardir` directory if you are using Docker. Alternatively, you can store it in any preferred location within your current working directory.
 
 Note: Ensure that your .har file is stored securely, as it may contain sensitive information.
@@ -776,17 +848,58 @@
 
 ###### Guide: How can AI help me with writing code?
 
  - Read: [/docs/guides/help_me](/docs/guides/help_me.md)
 
 ## 🙌 Contributors
 
-A list of all contributors is available [here](https://github.com/xtekky/gpt4free/graphs/contributors)   
-The [`Vercel.py`](https://github.com/xtekky/gpt4free/blob/main/g4f/Provider/Vercel.py) file contains code from [vercel-llm-api](https://github.com/ading2210/vercel-llm-api) by [@ading2210](https://github.com/ading2210), which is licensed under the [GNU GPL v3](https://www.gnu.org/licenses/gpl-3.0.txt)   
-Top 1 Contributor: [@hlohaus](https://github.com/hlohaus)
+A list of all contributors is available [here](https://github.com/xtekky/gpt4free/graphs/contributors)
+
+<a href="https://github.com/xtekky" target="_blank"><img src="https://avatars.githubusercontent.com/u/98614666?v=4&s=45" width="45" title="xtekky"></a>
+<a href="https://github.com/hlohaus" target="_blank"><img src="https://avatars.githubusercontent.com/u/983577?v=4&s=45" width="45" title="hlohaus"></a>
+<a href="https://github.com/bagusindrayana" target="_blank"><img src="https://avatars.githubusercontent.com/u/36830534?v=4&s=45" width="45" title="bagusindrayana"></a>
+<a href="https://github.com/sudouser777" target="_blank"><img src="https://avatars.githubusercontent.com/u/22415463?v=4&s=45" width="45" title="sudouser777"></a>
+<a href="https://github.com/thatlukinhasguy1" target="_blank"><img src="https://avatars.githubusercontent.com/u/139662282?v=4&s=45" width="45" title="thatlukinhasguy1"></a>
+<a href="https://github.com/Commenter123321" target="_blank"><img src="https://avatars.githubusercontent.com/u/36051603?v=4&s=45" width="45" title="Commenter123321"></a>
+<a href="https://github.com/DanielShemesh" target="_blank"><img src="https://avatars.githubusercontent.com/u/20585236?v=4&s=45" width="45" title="DanielShemesh"></a>
+<a href="https://github.com/Luneye" target="_blank"><img src="https://avatars.githubusercontent.com/u/73485421?v=4&s=45" width="45" title="Luneye"></a>
+<a href="https://github.com/enganese" target="_blank"><img src="https://avatars.githubusercontent.com/u/69082498?v=4&s=45" width="45" title="enganese"></a>
+<a href="https://github.com/ezerinz" target="_blank"><img src="https://avatars.githubusercontent.com/u/100193740?v=4&s=45" width="45" title="ezerinz"></a>
+<a href="https://github.com/Lin-jun-xiang" target="_blank"><img src="https://avatars.githubusercontent.com/u/63782903?v=4&s=45" width="45" title="Lin-jun-xiang"></a>
+<a href="https://github.com/nullstreak" target="_blank"><img src="https://avatars.githubusercontent.com/u/139914347?v=4&s=45" width="45" title="nullstreak"></a>
+<a href="https://github.com/valerii-chirkov" target="_blank"><img src="https://avatars.githubusercontent.com/u/81074936?v=4&s=45" width="45" title="valerii-chirkov"></a>
+<a href="https://github.com/MIDORIBIN" target="_blank"><img src="https://avatars.githubusercontent.com/u/25425217?v=4&s=45" width="45" title="MIDORIBIN"></a>
+<a href="https://github.com/repollo" target="_blank"><img src="https://avatars.githubusercontent.com/u/2671466?v=4&s=45" width="45" title="repollo"></a>
+<a href="https://github.com/hpsj" target="_blank"><img src="https://avatars.githubusercontent.com/u/54535414?v=4&s=45" width="45" title="hpsj"></a>
+<a href="https://github.com/taiyi747" target="_blank"><img src="https://avatars.githubusercontent.com/u/63543716?v=4&s=45" width="45" title="taiyi747"></a>
+<a href="https://github.com/ostix360" target="_blank"><img src="https://avatars.githubusercontent.com/u/55257054?v=4&s=45" width="45" title="ostix360"></a>
+<a href="https://github.com/WdR-Tech" target="_blank"><img src="https://avatars.githubusercontent.com/u/143020293?v=4&s=45" width="45" title="WdR-Tech"></a>
+<a href="https://github.com/HexyeDEV" target="_blank"><img src="https://avatars.githubusercontent.com/u/65314629?v=4&s=45" width="45" title="HexyeDEV"></a>
+<a href="https://github.com/9fo" target="_blank"><img src="https://avatars.githubusercontent.com/u/71867245?v=4&s=45" width="45" title="9fo"></a>
+<a href="https://github.com/eltociear" target="_blank"><img src="https://avatars.githubusercontent.com/u/22633385?v=4&s=45" width="45" title="eltociear"></a>
+<a href="https://github.com/ramonvc" target="_blank"><img src="https://avatars.githubusercontent.com/u/13617054?v=4&s=45" width="45" title="ramonvc"></a>
+<a href="https://github.com/naa7" target="_blank"><img src="https://avatars.githubusercontent.com/u/44613678?v=4&s=45" width="45" title="naa7"></a>
+<a href="https://github.com/zeng-rr" target="_blank"><img src="https://avatars.githubusercontent.com/u/47846202?v=4&s=45" width="45" title="zeng-rr"></a>
+<a href="https://github.com/editor-syntax" target="_blank"><img src="https://avatars.githubusercontent.com/u/109844019?v=4&s=45" width="45" title="editor-syntax"></a>
+<a href="https://github.com/devAdityaa" target="_blank"><img src="https://avatars.githubusercontent.com/u/77636021?v=4&s=45" width="45" title="devAdityaa"></a>
+<a href="https://github.com/kggn" target="_blank"><img src="https://avatars.githubusercontent.com/u/95663228?v=4&s=45" width="45" title="kggn"></a>
+<a href="https://github.com/xiangsx" target="_blank"><img src="https://avatars.githubusercontent.com/u/29322721?v=4&s=45" width="45" title="xiangsx"></a>
+<a href="https://github.com/ggindinson" target="_blank"><img src="https://avatars.githubusercontent.com/u/97807772?v=4&s=45" width="45" title="ggindinson"></a>
+<span></span>
+<img src="https://avatars.githubusercontent.com/u/71154407?s=45&v=4" width="45" title="ading2210">
+<img src="https://avatars.githubusercontent.com/u/12299238?s=45&v=4" width="45" title="xqdoo00o">
+<img src="https://avatars.githubusercontent.com/u/97126670?s=45&v=4" width="45" title="nathanrchn">
+<img src="https://avatars.githubusercontent.com/u/81407603?v=4&s=45" width="45" title="dsdanielpark">
+
+- The [`Vercel.py`](g4f/Provider/Vercel.py) file contains code from [vercel-llm-api](https://github.com/ading2210/vercel-llm-api) by [@ading2210](https://github.com/ading2210)
+- The [`har_file.py`](g4f/Provider/openai/har_file.py) has input from [xqdoo00o/ChatGPT-to-API](https://github.com/xqdoo00o/ChatGPT-to-API)
+- The [`PerplexityLabs.py`](g4f/Provider/openai/har_file.py) has input from [nathanrchn/perplexityai](https://github.com/nathanrchn/perplexityai)
+- The [`Gemini.py`](g4f/Provider/needs_auth/Gemini.py) has input from [dsdanielpark/Gemini-API](https://github.com/dsdanielpark/Gemini-API)
+
+*Having input implies that the AI's code generation utilized it as one of many sources.*
 
 ## ©️ Copyright
 
 This program is licensed under the [GNU GPL v3](https://www.gnu.org/licenses/gpl-3.0.txt)
 
 ```
 xtekky/gpt4free: Copyright (C) 2023 xtekky
```

#### html2text {}

```diff
@@ -1,11 +1,52 @@
-![248433934-7886223b-c1d1-4260-82aa-da5741f303bb](https://github.com/xtekky/
-gpt4free/assets/98614666/ea012c87-76e0-496a-8ac4-e2de090cc6c9)
-_[_x_t_e_k_k_y_%_2_F_g_p_t_4_f_r_e_e_ _|_ _T_r_e_n_d_s_h_i_f_t_]Written by [@xtekky](https://github.com/
-hlohaus) & maintained by [@hlohaus](https://github.com/hlohaus)
+Metadata-Version: 2.1 Name: g4f Version: 0.2.8.1 Summary: The official gpt4free
+repository | various collection of powerful language models Home-page: https://
+github.com/xtekky/gpt4free Author: Tekky Author-email:
+g4f.ai> Project-URL: Source Code, https://github.com/xtekky/gpt4free Project-
+URL: Bug Tracker, https://github.com/xtekky/gpt4free/issues Keywords:
+python,chatbot,reverse-engineering,openai,chatbots,gpt,language-model,gpt-
+3,gpt3,openai-api,gpt-4,gpt4,chatgpt,chatgpt-api,openai-chatgpt,chatgpt-
+free,chatgpt-4,chatgpt4,chatgpt4-api,free,free-gpt,gpt4free,g4f Classifier:
+Development Status :: 2 - Pre-Alpha Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python :: 3 Classifier: Operating System ::
+Unix Classifier: Operating System :: MacOS :: MacOS X Classifier: Operating
+System :: Microsoft :: Windows Description-Content-Type: text/markdown License-
+File: LICENSE Requires-Dist: requests Requires-Dist: aiohttp Requires-Dist:
+brotli Requires-Dist: pycryptodome Provides-Extra: all Requires-Dist:
+curl_cffi>=0.6.2; extra == "all" Requires-Dist: certifi; extra == "all"
+Requires-Dist: browser_cookie3; extra == "all" Requires-Dist: PyExecJS; extra
+== "all" Requires-Dist: duckduckgo-search>=5.0; extra == "all" Requires-Dist:
+beautifulsoup4; extra == "all" Requires-Dist: brotli; extra == "all" Requires-
+Dist: pywebview; extra == "all" Requires-Dist: platformdirs; extra == "all"
+Requires-Dist: plyer; extra == "all" Requires-Dist: cryptography; extra ==
+"all" Requires-Dist: aiohttp_socks; extra == "all" Requires-Dist: pillow; extra
+== "all" Requires-Dist: cairosvg; extra == "all" Requires-Dist: werkzeug; extra
+== "all" Requires-Dist: flask; extra == "all" Requires-Dist: loguru; extra ==
+"all" Requires-Dist: fastapi; extra == "all" Requires-Dist: uvicorn; extra ==
+"all" Requires-Dist: nest_asyncio; extra == "all" Requires-Dist: pycryptodome;
+extra == "all" Provides-Extra: image Requires-Dist: pillow; extra == "image"
+Requires-Dist: cairosvg; extra == "image" Requires-Dist: beautifulsoup4; extra
+== "image" Provides-Extra: webdriver Requires-Dist: platformdirs; extra ==
+"webdriver" Requires-Dist: undetected-chromedriver>=3.5.5; extra == "webdriver"
+Requires-Dist: setuptools; extra == "webdriver" Requires-Dist: selenium-wire;
+extra == "webdriver" Provides-Extra: webview Requires-Dist: webview; extra ==
+"webview" Requires-Dist: platformdirs; extra == "webview" Requires-Dist: plyer;
+extra == "webview" Requires-Dist: cryptography; extra == "webview" Provides-
+Extra: openai Requires-Dist: pycryptodome; extra == "openai" Provides-Extra:
+api Requires-Dist: loguru; extra == "api" Requires-Dist: fastapi; extra ==
+"api" Requires-Dist: uvicorn; extra == "api" Requires-Dist: nest_asyncio; extra
+== "api" Provides-Extra: gui Requires-Dist: werkzeug; extra == "gui" Requires-
+Dist: flask; extra == "gui" Requires-Dist: beautifulsoup4; extra == "gui"
+Requires-Dist: pillow; extra == "gui" Requires-Dist: duckduckgo-search>=5.0;
+extra == "gui" Requires-Dist: browser_cookie3; extra == "gui" Provides-Extra:
+local Requires-Dist: gpt4all; extra == "local" ![248433934-7886223b-c1d1-4260-
+82aa-da5741f303bb](https://github.com/xtekky/gpt4free/assets/98614666/ea012c87-
+76e0-496a-8ac4-e2de090cc6c9) _[_x_t_e_k_k_y_%_2_F_g_p_t_4_f_r_e_e_ _|_ _T_r_e_n_d_s_h_i_f_t_]Written by
+[@xtekky](https://github.com/hlohaus) & maintained by [@hlohaus](https://
+github.com/hlohaus)
 > By using this repository or any code related to it, you agree to the [legal
 notice](LEGAL_NOTICE.md). The author is **not responsible for the usage of this
 repository nor endorses it**, nor is the author responsible for any copies,
 forks, re-uploads made by other users, or anything else related to GPT4Free.
 This is the author's only account and repository. To prevent impersonation or
 irresponsible actions, please comply with the GNU GPL license this Repository
 uses. > [!Warning] *"gpt4free"* serves as a **PoC** (proof of concept),
@@ -13,139 +54,159 @@
 with features like timeouts, load balance and flow control. > [!Note] LLaasstteett
 vveerrssiioonn:: [![PyPI version](https://img.shields.io/pypi/v/g4f?color=blue)](https:
 //pypi.org/project/g4f) [![Docker version](https://img.shields.io/docker/v/
 hlohaus789/g4f?label=docker&color=blue)](https://hub.docker.com/r/hlohaus789/
 g4f) > SSttaattss:: [![Downloads](https://static.pepy.tech/badge/g4f)](https://
 pepy.tech/project/g4f) [![Downloads](https://static.pepy.tech/badge/g4f/month)]
 (https://pepy.tech/project/g4f) ```sh pip install -U g4f ``` ```sh docker pull
-hlohaus789/g4f ``` ## ð What's New - Check out a more in depth local
-inference @ https://github.com/gpt4free/gpt4local - Join our Telegram Channel:
-[t.me/g4f_channel](https://telegram.me/g4f_channel) - Join our Discord Group:
-[discord.gg/XfybzPXPH5](https://discord.gg/XfybzPXPH5) - `g4f` now supports
-100% local inference: [local-docs](https://g4f.mintlify.app/docs/core/usage/
-local) ## ð» Site Takedown Is your site on this repository and you want to
-take it down? Send an email to takedown@g4f.ai with proof it is yours and it
-will be removed as fast as possible. To prevent reproduction please secure your
-API ;) ## ð Feedback and Todo You can always leave some feedback here:
-https://forms.gle/FeWV9RLEedfdkmFN6 As per the survey, here is a list of
-improvements to come - [x] Update the repository to include the new openai
-library syntax (ex: `Openai()` class) | completed, use `g4f.client.Client` -
-[ ] Golang implementation - [ ] ð§ Improve Documentation (in /docs & Guides,
-Howtos, & Do video tutorials) - [x] Improve the provider status list & updates
-- [ ] Tutorials on how to reverse sites to write your own wrapper (PoC only
-ofc) - [x] Improve the Bing wrapper. (Wait and Retry or reuse conversation) -
-[ ] Write a standard provider performance test to improve the stability - [ ]
-Potential support and development of local models - [ ] ð§ Improve
-compatibility and error handling ## ð Table of Contents - [ð What's New]
-(#-whats-new) - [ð Table of Contents](#-table-of-contents) - [ð ï¸
-Getting Started](#-getting-started) + [Docker container](#docker-container) -
-[Quick start](#quick-start) + [Use python](#use-python) - [Prerequisites]
-(#prerequisites) - [Install using PyPI package:](#install-using-pypi-package) -
-[Install from source:](#install-from-source) - [Install using Docker:]
-(#install-using-docker) - [ð¡ Usage](#-usage) * [Text Generation](#text-
-generation) * [Image Generation](#image-generation) * [Web UI](#web-ui) *
-[Interference API](#interference-api) * [Configuration](#configuration) - [ð
-Providers and Models](#-providers-and-models) * [GPT-4](#gpt-4) * [GPT-3.5]
-(#gpt-35) * [Other](#other) * [Models](#models) - [ð Powered by gpt4free](#-
-powered-by-gpt4free) - [ð¤ Contribute](#-contribute) + [How do i create a new
-Provider?](#guide-how-do-i-create-a-new-provider) + [How can AI help me with
-writing code?](#guide-how-can-ai-help-me-with-writing-code) - [ð
-Contributors](#-contributors) - [Â©ï¸ Copyright](#-copyright) - [â­ Star
-History](#-star-history) - [ð License](#-license) ## ð ï¸ Getting Started
-#### Docker container ##### Quick start: 1. [Download and install Docker]
-(https://docs.docker.com/get-docker/) 2. Pull latest image and run the
+hlohaus789/g4f ``` ## ð What's New - Installation Guide for Windows (.exe):
+ð» [#installation-guide-for-windows](#installation-guide-for-windows-exe) -
+Join our Telegram Channel: ð¨ [telegram.me/g4f_channel](https://telegram.me/
+g4f_channel) - Join our Discord Group: ð¬ [discord.gg/XfybzPXPH5](https://
+discord.gg/XfybzPXPH5) - `g4f` now supports 100% local inference: ð§  [local-
+docs](https://g4f.mintlify.app/docs/core/usage/local) ## ð» Site Takedown Is
+your site on this repository and you want to take it down? Send an email to
+takedown@g4f.ai with proof it is yours and it will be removed as fast as
+possible. To prevent reproduction please secure your API. ð ## ð Feedback
+and Todo You can always leave some feedback here: https://forms.gle/
+FeWV9RLEedfdkmFN6 As per the survey, here is a list of improvements to come -
+[x] Update the repository to include the new openai library syntax (ex: `Openai
+()` class) | completed, use `g4f.client.Client` - [ ] Golang implementation -
+[ ] ð§ Improve Documentation (in /docs & Guides, Howtos, & Do video
+tutorials) - [x] Improve the provider status list & updates - [ ] Tutorials on
+how to reverse sites to write your own wrapper (PoC only ofc) - [x] Improve the
+Bing wrapper. (Wait and Retry or reuse conversation) - [ ] ð§ Write a
+standard provider performance test to improve the stability - [ ] Potential
+support and development of local models - [ ] ð§ Improve compatibility and
+error handling ## ð Table of Contents - [ð What's New](#-whats-new) -
+[ð Table of Contents](#-table-of-contents) - [ð ï¸ Getting Started](#-
+getting-started) + [Docker Container Guide](#docker-container-guide) +
+[Installation Guide for Windows (.exe)](#installation-guide-for-windows-exe) +
+[Use python](#use-python) - [Prerequisites](#prerequisites) - [Install using
+PyPI package:](#install-using-pypi-package) - [Install from source:](#install-
+from-source) - [Install using Docker:](#install-using-docker) - [ð¡ Usage](#-
+usage) * [Text Generation](#text-generation) * [Image Generation](#image-
+generation) * [Web UI](#web-ui) * [Interference API](#interference-api) *
+[Configuration](#configuration) - [ð Providers and Models](#-providers-and-
+models) * [GPT-4](#gpt-4) * [GPT-3.5](#gpt-35) * [Other](#other) * [Models]
+(#models) - [ð Powered by gpt4free](#-powered-by-gpt4free) - [ð¤
+Contribute](#-contribute) + [How do i create a new Provider?](#guide-how-do-i-
+create-a-new-provider) + [How can AI help me with writing code?](#guide-how-
+can-ai-help-me-with-writing-code) - [ð Contributors](#-contributors) -
+[Â©ï¸ Copyright](#-copyright) - [â­ Star History](#-star-history) - [ð
+License](#-license) ## ð ï¸ Getting Started #### Docker Container Guide
+##### Getting Started Quickly: 1. **Install Docker:** Begin by [downloading and
+installing Docker](https://docs.docker.com/get-docker/). 2. **Set Up the
+Container:** Use the following commands to pull the latest image and start the
 container: ```sh docker pull hlohaus789/g4f docker run -p 8080:8080 -p 1337:
 1337 -p 7900:7900 --shm-size="2g" -v ${PWD}/hardir:/app/hardir hlohaus789/g4f:
-latest ``` 3. Open the included client on: [http://localhost:8080/chat/](http:/
-/localhost:8080/chat/) or set the API base in your client to: [http://
-localhost:1337/v1](http://localhost:1337/v1) 4. (Optional) If you need to log
-in to a provider, you can view the desktop from the container here: http://
-localhost:7900/?autoconnect=1&resize=scale&password=secret. ##### Use your
-smartphone: Run the Web UI on Your Smartphone: - [/docs/guides/phone](/docs/
-guides/phone.md) #### Use python ##### Prerequisites: 1. [Download and install
-Python](https://www.python.org/downloads/) (Version 3.10+ is recommended). 2.
-[Install Google Chrome](https://www.google.com/chrome/) for providers with
-webdriver ##### Install using PyPI package: ``` pip install -U g4f[all] ``` How
-do I install only parts or do disable parts? Use partial requirements: [/docs/
-requirements](/docs/requirements.md) ##### Install from source: How do I load
-the project using git and installing the project requirements? Read this
-tutorial and follow it step by step: [/docs/git](/docs/git.md) ##### Install
-using Docker: How do I build and run composer image from source? Use docker-
-compose: [/docs/docker](/docs/docker.md) ## ð¡ Usage #### Text Generation
-```python from g4f.client import Client client = Client() response =
+latest ``` 3. **Access the Client:** - To use the included client, navigate to:
+[http://localhost:8080/chat/](http://localhost:8080/chat/) - Or set the API
+base for your client to: [http://localhost:1337/v1](http://localhost:1337/v1)
+4. **(Optional) Provider Login:** If required, you can access the container's
+desktop here: http://localhost:7900/?autoconnect=1&resize=scale&password=secret
+for provider login purposes. #### Installation Guide for Windows (.exe) To
+ensure the seamless operation of our application, please follow the
+instructions below. These steps are designed to guide you through the
+installation process on Windows operating systems. ##### Prerequisites 1.
+**WebView2 Runtime**: Our application requires the *WebView2 Runtime* to be
+installed on your system. If you do not have it installed, please download and
+install it from the [Microsoft Developer Website](https://
+developer.microsoft.com/en-us/microsoft-edge/webview2/). If you already have
+*WebView2 Runtime* installed but are encountering issues, navigate to
+*Installed Windows Apps*, select *WebView2*, and opt for the repair option.
+##### Installation Steps 2. **Download the Application**: Visit our [latest
+releases page](https://github.com/xtekky/gpt4free/releases/latest) and download
+the most recent version of the application, named `g4f.webview.*.exe`. 3.
+**File Placement**: Once downloaded, transfer the `.exe` file from your
+downloads folder to a directory of your choice on your system, and then execute
+it to run the app. ##### Post-Installation Adjustment 4. **Firewall
+Configuration (Hotfix)**: Upon installation, it may be necessary to adjust your
+Windows Firewall settings to allow the application to operate correctly. To do
+this, access your Windows Firewall settings and allow the application. By
+following these steps, you should be able to successfully install and run the
+application on your Windows system. If you encounter any issues during the
+installation process, please refer to our Issue Tracker or try to get contact
+over Discord for assistance. Run the **Webview UI** on other Platfroms: - [/
+docs/guides/webview](/docs/webview.md) ##### Use your smartphone: Run the Web
+UI on Your Smartphone: - [/docs/guides/phone](/docs/guides/phone.md) #### Use
+python ##### Prerequisites: 1. [Download and install Python](https://
+www.python.org/downloads/) (Version 3.10+ is recommended). 2. [Install Google
+Chrome](https://www.google.com/chrome/) for providers with webdriver #####
+Install using PyPI package: ``` pip install -U g4f[all] ``` How do I install
+only parts or do disable parts? Use partial requirements: [/docs/requirements]
+(/docs/requirements.md) ##### Install from source: How do I load the project
+using git and installing the project requirements? Read this tutorial and
+follow it step by step: [/docs/git](/docs/git.md) ##### Install using Docker:
+How do I build and run composer image from source? Use docker-compose: [/docs/
+docker](/docs/docker.md) ## ð¡ Usage #### Text Generation ```python from
+g4f.client import Client client = Client() response =
 client.chat.completions.create( model="gpt-3.5-turbo", messages=[{"role":
 "user", "content": "Hello"}], ... ) print(response.choices[0].message.content)
 ``` ``` Hello! How can I assist you today? ``` #### Image Generation ```python
 from g4f.client import Client client = Client() response =
 client.images.generate( model="gemini", prompt="a white siamese cat", ... )
 image_url = response.data[0].url ``` [![Image with cat](/docs/cat.jpeg)](/docs/
 client.md) **Full Documentation for Python API** - New Client API like the
 OpenAI Python library: [/docs/client](/docs/client.md) - Legacy API with python
-modules: [/docs/legacy](/docs/legacy.md) ### Webview GUI Open the GUI in a
-window of your OS. Runs on a local/static/ssl server and use a JavaScript API.
-Supports login into the OpenAI Chat, Image Upload and streamed Text Generation.
-Supports all platforms, but only Linux tested. 1. Install all requirements
-with: ```bash pip install g4f[webview] ``` 2. Follow the OS specific steps
-here: [pywebview installation](https://pywebview.flowrl.com/guide/
-installation.html#dependencies) 3. Run the app with: ```python from
-g4f.gui.webview import run_webview run_webview(debug=True) ``` or execute the
-following command: ```bash python -m g4f.gui.webview -debug ``` #### Webserver
-To start the web interface, type the following codes in python: ```python from
-g4f.gui import run_gui run_gui() ``` or execute the following command: ```bash
-python -m g4f.cli gui -port 8080 -debug ``` ### Interference API You can use
-the Interference API to serve other OpenAI integrations with G4F. See: [/docs/
-interference](/docs/interference.md) ### Configuration #### Cookies You need
-cookies for BingCreateImages and the Gemini Provider. From Bing you need the
-"_U" cookie and from Gemini you need the "__Secure-1PSID" cookie. Sometimes you
-doesn't need the "__Secure-1PSID" cookie, but some other auth cookies. You can
-pass the cookies in the create function or you use the `set_cookies` setter
-before you run G4F: ```python from g4f.cookies import set_cookies set_cookies
-(".bing.com", { "_U": "cookie value" }) set_cookies(".google.com", { "__Secure-
-1PSID": "cookie value" }) ... ``` #### .HAR File for OpenaiChat Provider #####
-Generating a .HAR File To utilize the OpenaiChat provider, a .har file is
-required from https://chat.openai.com/. Follow the steps below to create a
-valid .har file: 1. Navigate to https://chat.openai.com/ using your preferred
-web browser and log in with your credentials. 2. Access the Developer Tools in
-your browser. This can typically be done by right-clicking the page and
-selecting "Inspect," or by pressing F12 or Ctrl+Shift+I (Cmd+Option+I on a
-Mac). 3. With the Developer Tools open, switch to the "Network" tab. 4. Reload
-the website to capture the loading process within the Network tab. 5. Initiate
-an action in the chat which can be capture in the .har file. 6. Right-click any
-of the network activities listed and select "Save all as HAR with content" to
-export the .har file. ##### Storing the .HAR File - Place the exported .har
-file in the `./hardir` directory if you are using Docker. Alternatively, you
-can store it in any preferred location within your current working directory.
-Note: Ensure that your .har file is stored securely, as it may contain
-sensitive information. #### Using Proxy If you want to hide or change your IP
-address for the providers, you can set a proxy globally via an environment
-variable: - On macOS and Linux: ```bash export G4F_PROXY="http://host:port" ```
-- On Windows: ```bash set G4F_PROXY=http://host:port ``` ## ð Providers and
-Models ### GPT-4 | Website | Provider | GPT-3.5 | GPT-4 | Stream | Status |
-Auth | | ------ | ------- | ------- | ----- | ------ | ------ | ---- | |
-[bing.com](https://bing.com/chat) | `g4f.Provider.Bing` | â | âï¸ | âï¸
-| ![Unknown](https://img.shields.io/badge/Unknown-grey) | â | | [chatgpt.ai]
-(https://chatgpt.ai) | `g4f.Provider.ChatgptAi` | â | âï¸ | âï¸ | !
-[Active](https://img.shields.io/badge/Active-brightgreen) | â | |
-[liaobots.site](https://liaobots.site) | `g4f.Provider.Liaobots` | âï¸ |
-âï¸ | âï¸ | ![Active](https://img.shields.io/badge/Active-brightgreen) |
-â | | [chat.openai.com](https://chat.openai.com) | `g4f.Provider.OpenaiChat`
-| âï¸ | â | âï¸ | ![Unknown](https://img.shields.io/badge/Unknown-grey)
-| âï¸ | | [raycast.com](https://raycast.com) | `g4f.Provider.Raycast` |
-âï¸ | âï¸ | âï¸ | ![Unknown](https://img.shields.io/badge/Unknown-
-grey) | âï¸ | | [beta.theb.ai](https://beta.theb.ai) | `g4f.Provider.Theb` |
-âï¸ | âï¸ | âï¸ | ![Unknown](https://img.shields.io/badge/Unknown-
-grey) | â | | [you.com](https://you.com) | `g4f.Provider.You` | âï¸ |
-âï¸ | âï¸ | ![Unknown](https://img.shields.io/badge/Unknown-grey) | â |
-### GPT-3.5 | Website | Provider | GPT-3.5 | GPT-4 | Stream | Status | Auth | |
------- | ------- | ------- | ----- | ------ | ------ | ---- | |
-[chat3.aiyunos.top](https://chat3.aiyunos.top/) | `g4f.Provider.AItianhuSpace`
-| âï¸ | â | âï¸ | ![Unknown](https://img.shields.io/badge/Unknown-grey)
-| â | | [chatforai.store](https://chatforai.store) | `g4f.Provider.ChatForAi`
-| âï¸ | â | âï¸ | ![Active](https://img.shields.io/badge/Active-
-brightgreen) | â | | [chatgpt4online.org](https://chatgpt4online.org) |
+modules: [/docs/legacy](/docs/legacy.md) #### Web UI To start the web
+interface, type the following codes in python: ```python from g4f.gui import
+run_gui run_gui() ``` or execute the following command: ```bash python -
+m g4f.cli gui -port 8080 -debug ``` #### Interference API You can use the
+Interference API to serve other OpenAI integrations with G4F. See docs: [/docs/
+interference](/docs/interference.md) Access with: http://localhost:1337/v1 ###
+Configuration #### Cookies You need cookies for BingCreateImages and the Gemini
+Provider. From Bing you need the "_U" cookie and from Gemini you need the
+"__Secure-1PSID" cookie. Sometimes you doesn't need the "__Secure-1PSID"
+cookie, but some other auth cookies. You can pass the cookies in the create
+function or you use the `set_cookies` setter before you run G4F: ```python from
+g4f.cookies import set_cookies set_cookies(".bing.com", { "_U": "cookie value"
+}) set_cookies(".google.com", { "__Secure-1PSID": "cookie value" }) ... ```
+#### .HAR File for OpenaiChat Provider ##### Generating a .HAR File To utilize
+the OpenaiChat provider, a .har file is required from https://chat.openai.com/.
+Follow the steps below to create a valid .har file: 1. Navigate to https://
+chat.openai.com/ using your preferred web browser and log in with your
+credentials. 2. Access the Developer Tools in your browser. This can typically
+be done by right-clicking the page and selecting "Inspect," or by pressing F12
+or Ctrl+Shift+I (Cmd+Option+I on a Mac). 3. With the Developer Tools open,
+switch to the "Network" tab. 4. Reload the website to capture the loading
+process within the Network tab. 5. Initiate an action in the chat which can be
+captured in the .har file. 6. Right-click any of the network activities listed
+and select "Save all as HAR with content" to export the .har file. #####
+Storing the .HAR File - Place the exported .har file in the `./hardir`
+directory if you are using Docker. Alternatively, you can store it in any
+preferred location within your current working directory. Note: Ensure that
+your .har file is stored securely, as it may contain sensitive information.
+#### Using Proxy If you want to hide or change your IP address for the
+providers, you can set a proxy globally via an environment variable: - On macOS
+and Linux: ```bash export G4F_PROXY="http://host:port" ``` - On Windows:
+```bash set G4F_PROXY=http://host:port ``` ## ð Providers and Models ###
+GPT-4 | Website | Provider | GPT-3.5 | GPT-4 | Stream | Status | Auth | | -----
+- | ------- | ------- | ----- | ------ | ------ | ---- | | [bing.com](https://
+bing.com/chat) | `g4f.Provider.Bing` | â | âï¸ | âï¸ | ![Unknown]
+(https://img.shields.io/badge/Unknown-grey) | â | | [chatgpt.ai](https://
+chatgpt.ai) | `g4f.Provider.ChatgptAi` | â | âï¸ | âï¸ | ![Active]
+(https://img.shields.io/badge/Active-brightgreen) | â | | [liaobots.site]
+(https://liaobots.site) | `g4f.Provider.Liaobots` | âï¸ | âï¸ | âï¸ |
+![Active](https://img.shields.io/badge/Active-brightgreen) | â | |
+[chat.openai.com](https://chat.openai.com) | `g4f.Provider.OpenaiChat` | âï¸
+| â | âï¸ | ![Unknown](https://img.shields.io/badge/Unknown-grey) | âï¸
+| | [raycast.com](https://raycast.com) | `g4f.Provider.Raycast` | âï¸ |
+âï¸ | âï¸ | ![Unknown](https://img.shields.io/badge/Unknown-grey) |
+âï¸ | | [beta.theb.ai](https://beta.theb.ai) | `g4f.Provider.Theb` | âï¸
+| âï¸ | âï¸ | ![Unknown](https://img.shields.io/badge/Unknown-grey) | â
+| | [you.com](https://you.com) | `g4f.Provider.You` | âï¸ | âï¸ | âï¸
+| ![Unknown](https://img.shields.io/badge/Unknown-grey) | â | ### GPT-3.5 |
+Website | Provider | GPT-3.5 | GPT-4 | Stream | Status | Auth | | ------ | ----
+--- | ------- | ----- | ------ | ------ | ---- | | [chat3.aiyunos.top](https://
+chat3.aiyunos.top/) | `g4f.Provider.AItianhuSpace` | âï¸ | â | âï¸ | !
+[Unknown](https://img.shields.io/badge/Unknown-grey) | â | |
+[chatforai.store](https://chatforai.store) | `g4f.Provider.ChatForAi` | âï¸
+| â | âï¸ | ![Active](https://img.shields.io/badge/Active-brightgreen) |
+â | | [chatgpt4online.org](https://chatgpt4online.org) |
 `g4f.Provider.Chatgpt4Online` | âï¸ | â | âï¸ | ![Active](https://
 img.shields.io/badge/Active-brightgreen) | â | | [chatgpt-free.cc](https://
 www.chatgpt-free.cc) | `g4f.Provider.ChatgptNext` | âï¸ | â | âï¸ | !
 [Active](https://img.shields.io/badge/Active-brightgreen) | â | |
 [chatgptx.de](https://chatgptx.de) | `g4f.Provider.ChatgptX` | âï¸ | â |
 âï¸ | ![Active](https://img.shields.io/badge/Active-brightgreen) | â | |
 [flowgpt.com](https://flowgpt.com/chat) | `g4f.Provider.FlowGpt` | âï¸ | â
@@ -278,30 +339,68 @@
 improvements, your input is valued. Creating a pull request is all it takes â
 our co-pilot will handle the code review process. Once all changes have been
 addressed, we'll merge the pull request into the main branch and release the
 updates at a later time. ###### Guide: How do i create a new Provider? - Read:
 [/docs/guides/create_provider](/docs/guides/create_provider.md) ###### Guide:
 How can AI help me with writing code? - Read: [/docs/guides/help_me](/docs/
 guides/help_me.md) ## ð Contributors A list of all contributors is available
-[here](https://github.com/xtekky/gpt4free/graphs/contributors) The
-[`Vercel.py`](https://github.com/xtekky/gpt4free/blob/main/g4f/Provider/
-Vercel.py) file contains code from [vercel-llm-api](https://github.com/
-ading2210/vercel-llm-api) by [@ading2210](https://github.com/ading2210), which
-is licensed under the [GNU GPL v3](https://www.gnu.org/licenses/gpl-3.0.txt)
-Top 1 Contributor: [@hlohaus](https://github.com/hlohaus) ## Â©ï¸ Copyright
-This program is licensed under the [GNU GPL v3](https://www.gnu.org/licenses/
-gpl-3.0.txt) ``` xtekky/gpt4free: Copyright (C) 2023 xtekky This program is
-free software: you can redistribute it and/or modify it under the terms of the
-GNU General Public License as published by the Free Software Foundation, either
-version 3 of the License, or (at your option) any later version. This program
-is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
-without even the implied warranty of MERCHANTABILITY or FITNESS FOR A
-PARTICULAR PURPOSE. See the GNU General Public License for more details. You
-should have received a copy of the GNU General Public License along with this
-program. If not, see
+[here](https://github.com/xtekky/gpt4free/graphs/contributors) _[_h_t_t_p_s_:_/_/
+_a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_9_8_6_1_4_6_6_6_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
+_a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_9_8_3_5_7_7_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
+_a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_3_6_8_3_0_5_3_4_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
+_a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_2_2_4_1_5_4_6_3_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
+_a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_1_3_9_6_6_2_2_8_2_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
+_a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_3_6_0_5_1_6_0_3_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
+_a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_2_0_5_8_5_2_3_6_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
+_a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_7_3_4_8_5_4_2_1_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
+_a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_6_9_0_8_2_4_9_8_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
+_a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_1_0_0_1_9_3_7_4_0_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
+_a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_6_3_7_8_2_9_0_3_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
+_a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_1_3_9_9_1_4_3_4_7_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
+_a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_8_1_0_7_4_9_3_6_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
+_a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_2_5_4_2_5_2_1_7_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
+_a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_2_6_7_1_4_6_6_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
+_a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_5_4_5_3_5_4_1_4_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
+_a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_6_3_5_4_3_7_1_6_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
+_a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_5_5_2_5_7_0_5_4_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
+_a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_1_4_3_0_2_0_2_9_3_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
+_a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_6_5_3_1_4_6_2_9_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
+_a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_7_1_8_6_7_2_4_5_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
+_a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_2_2_6_3_3_3_8_5_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
+_a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_1_3_6_1_7_0_5_4_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
+_a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_4_4_6_1_3_6_7_8_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
+_a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_4_7_8_4_6_2_0_2_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
+_a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_1_0_9_8_4_4_0_1_9_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
+_a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_7_7_6_3_6_0_2_1_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
+_a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_9_5_6_6_3_2_2_8_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
+_a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_2_9_3_2_2_7_2_1_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
+_a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_9_7_8_0_7_7_7_2_?_v_=_4_&_s_=_4_5_][https://
+avatars.githubusercontent.com/u/71154407?s=45&v=4][https://
+avatars.githubusercontent.com/u/12299238?s=45&v=4][https://
+avatars.githubusercontent.com/u/97126670?s=45&v=4][https://
+avatars.githubusercontent.com/u/81407603?v=4&s=45]- The [`Vercel.py`](g4f/
+Provider/Vercel.py) file contains code from [vercel-llm-api](https://
+github.com/ading2210/vercel-llm-api) by [@ading2210](https://github.com/
+ading2210) - The [`har_file.py`](g4f/Provider/openai/har_file.py) has input
+from [xqdoo00o/ChatGPT-to-API](https://github.com/xqdoo00o/ChatGPT-to-API) -
+The [`PerplexityLabs.py`](g4f/Provider/openai/har_file.py) has input from
+[nathanrchn/perplexityai](https://github.com/nathanrchn/perplexityai) - The
+[`Gemini.py`](g4f/Provider/needs_auth/Gemini.py) has input from [dsdanielpark/
+Gemini-API](https://github.com/dsdanielpark/Gemini-API) *Having input implies
+that the AI's code generation utilized it as one of many sources.* ## Â©ï¸
+Copyright This program is licensed under the [GNU GPL v3](https://www.gnu.org/
+licenses/gpl-3.0.txt) ``` xtekky/gpt4free: Copyright (C) 2023 xtekky This
+program is free software: you can redistribute it and/or modify it under the
+terms of the GNU General Public License as published by the Free Software
+Foundation, either version 3 of the License, or (at your option) any later
+version. This program is distributed in the hope that it will be useful, but
+WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or
+FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more
+details. You should have received a copy of the GNU General Public License
+along with this program. If not, see
 www.gnu.org/licenses/>. ``` ## â­ Star History _[_S_t_a_r_ _H_i_s_t_o_r_y_ _C_h_a_r_t_]## ð
 License
 [https://upload.wikimedia.org/wikipedia/ [https://img.shields.io/badge/License-
    commons/thumb/9/93/GPLv3_Logo.svg/    GNU_GPL_v3.0-red.svg]
        1200px-GPLv3_Logo.svg.png]        This project is licensed under
                                          _G_N_U___G_P_L___v_3_._0.
                                                              (_ð___¼_ _B_a_c_k_ _t_o_ _t_o_p)
```

### Comparing `g4f-0.2.8.0/g4f/Provider/Aura.py` & `g4f-0.2.8.1/g4f/Provider/Aura.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,14 +13,16 @@
 
     @classmethod
     async def create_async_generator(
         cls,
         model: str,
         messages: Messages,
         proxy: str = None,
+        temperature: float = 0.5,
+        max_tokens: int = 8192,
         webdriver: WebDriver = None,
         **kwargs
     ) -> AsyncResult:
         args = get_args_from_browser(cls.url, webdriver, proxy)
         async with ClientSession(**args) as session:
             new_messages = []
             system_message = []
@@ -30,18 +32,18 @@
                 else:
                     new_messages.append(message)
             data = {
                 "model": {
                     "id": "openchat_v3.2_mistral",
                     "name": "OpenChat Aura",
                     "maxLength": 24576,
-                    "tokenLimit": 8192
+                    "tokenLimit": max_tokens
                 },
                 "messages": new_messages,
                 "key": "",
                 "prompt": "\n".join(system_message),
-                "temperature": 0.5
+                "temperature": temperature
             }
             async with session.post(f"{cls.url}/api/chat", json=data, proxy=proxy) as response:
                 response.raise_for_status()
                 async for chunk in response.content.iter_any():
-                    yield chunk.decode()
+                    yield chunk.decode(error="ignore")
```

### Comparing `g4f-0.2.8.0/g4f/Provider/Bing.py` & `g4f-0.2.8.1/g4f/Provider/Bing.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.0/g4f/Provider/BingCreateImages.py` & `g4f-0.2.8.1/g4f/Provider/BingCreateImages.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.0/g4f/Provider/ChatForAi.py` & `g4f-0.2.8.1/g4f/Provider/ChatForAi.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 import time
 import hashlib
 import uuid
 
 from ..typing import AsyncResult, Messages
-from ..requests import StreamSession
+from ..requests import StreamSession, raise_for_status
 from ..errors import RateLimitError
 from .base_provider import AsyncGeneratorProvider, ProviderModelMixin
 
 class ChatForAi(AsyncGeneratorProvider, ProviderModelMixin):
     url = "https://chatforai.store"
     working = True
     default_model = "gpt-3.5-turbo"
@@ -50,19 +50,17 @@
                 },
                 "prompt": "",
                 "messages": messages,
                 "timestamp": timestamp,
                 "sign": generate_signature(timestamp, "", conversation_id)
             }
             async with session.post(f"{cls.url}/api/handle/provider-openai", json=data) as response:
-                if response.status == 429:
-                    raise RateLimitError("Rate limit reached")
-                response.raise_for_status()
+                await raise_for_status(response)
                 async for chunk in response.iter_content():
                     if b"https://chatforai.store" in chunk:
-                        raise RuntimeError(f"Response: {chunk.decode()}")
-                    yield chunk.decode()
+                        raise RuntimeError(f"Response: {chunk.decode(errors='ignore')}")
+                    yield chunk.decode(errors="ignore")
 
     
 def generate_signature(timestamp: int, message: str, id: str):
     buffer = f"{id}:{timestamp}:{message}:h496Jd6b"
     return hashlib.sha256(buffer.encode()).hexdigest()
```

### Comparing `g4f-0.2.8.0/g4f/Provider/Chatgpt4Online.py` & `g4f-0.2.8.1/g4f/Provider/Chatgpt4Online.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.0/g4f/Provider/ChatgptAi.py` & `g4f-0.2.8.1/g4f/Provider/ChatgptAi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.0/g4f/Provider/ChatgptFree.py` & `g4f-0.2.8.1/g4f/Provider/ChatgptFree.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 import re
 
-from ..requests import StreamSession
+from ..requests import StreamSession, raise_for_status
 from ..typing import Messages
 from .base_provider import AsyncProvider
 from .helper import format_prompt
 
 class ChatgptFree(AsyncProvider):
     url                   = "https://chatgptfree.ai"
     supports_gpt_35_turbo = True
@@ -38,23 +38,23 @@
             'sec-fetch-site': 'same-origin',
             'user-agent': 'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/118.0.0.0 Safari/537.36',
         }
 
         async with StreamSession(
                 headers=headers,
                 cookies=cookies,
-                impersonate="chrome107",
-                proxies={"https": proxy},
+                impersonate="chrome",
+                proxies={"all": proxy},
                 timeout=timeout
             ) as session:
-            
+
             if not cls._nonce:
                 async with session.get(f"{cls.url}/") as response:
                     
-                    response.raise_for_status()
+                    await raise_for_status(response)
                     response = await response.text()
 
                     result = re.search(r'data-post-id="([0-9]+)"', response)
                     if not result:
                         raise RuntimeError("No post id found")
                     cls._post_id = result.group(1)
 
@@ -71,9 +71,9 @@
                 "post_id": cls._post_id,
                 "url": cls.url,
                 "action": "wpaicg_chat_shortcode_message",
                 "message": prompt,
                 "bot_id": "0"
             }
             async with session.post(f"{cls.url}/wp-admin/admin-ajax.php", data=data, cookies=cookies) as response:
-                response.raise_for_status()
+                await raise_for_status(response)
                 return (await response.json())["data"]
```

### Comparing `g4f-0.2.8.0/g4f/Provider/ChatgptNext.py` & `g4f-0.2.8.1/g4f/Provider/ChatgptNext.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.0/g4f/Provider/ChatgptX.py` & `g4f-0.2.8.1/g4f/Provider/ChatgptX.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.0/g4f/Provider/DeepInfra.py` & `g4f-0.2.8.1/g4f/Provider/deprecated/Aichat.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,89 +1,64 @@
 from __future__ import annotations
 
-import json
-import requests
-from ..typing       import AsyncResult, Messages
-from .base_provider import AsyncGeneratorProvider, ProviderModelMixin
-from ..requests     import StreamSession
-
-class DeepInfra(AsyncGeneratorProvider, ProviderModelMixin):
-    url = "https://deepinfra.com"
-    working = True
-    supports_stream = True
-    supports_message_history = True
-    default_model = 'meta-llama/Llama-2-70b-chat-hf'
-    
-    @classmethod
-    def get_models(cls):
-        if not cls.models:
-            url = 'https://api.deepinfra.com/models/featured'
-            models = requests.get(url).json()
-            cls.models = [model['model_name'] for model in models]
-        return cls.models
-
-    @classmethod
-    async def create_async_generator(
-        cls,
+from ...typing import Messages
+from ..base_provider import AsyncProvider, format_prompt
+from ..helper import get_cookies
+from ...requests import StreamSession
+
+class Aichat(AsyncProvider):
+    url = "https://chat-gpt.org/chat"
+    working = False
+    supports_gpt_35_turbo = True
+
+    @staticmethod
+    async def create_async(
         model: str,
         messages: Messages,
-        stream: bool,
-        proxy: str = None,
-        timeout: int = 120,
-        auth: str = None,
-        **kwargs
-    ) -> AsyncResult:
+        proxy: str = None, **kwargs) -> str:
+        
+        cookies = get_cookies('chat-gpt.org') if not kwargs.get('cookies') else kwargs.get('cookies')
+        if not cookies:
+            raise RuntimeError(
+                "g4f.provider.Aichat requires cookies, [refresh https://chat-gpt.org on chrome]"
+            )
+
         headers = {
-            'Accept-Encoding': 'gzip, deflate, br',
-            'Accept-Language': 'en-US',
-            'Connection': 'keep-alive',
-            'Content-Type': 'application/json',
-            'Origin': 'https://deepinfra.com',
-            'Referer': 'https://deepinfra.com/',
-            'Sec-Fetch-Dest': 'empty',
-            'Sec-Fetch-Mode': 'cors',
-            'Sec-Fetch-Site': 'same-site',
-            'User-Agent': 'Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/119.0.0.0 Safari/537.36',
-            'X-Deepinfra-Source': 'web-embed',
-            'accept': 'text/event-stream',
-            'sec-ch-ua': '"Google Chrome";v="119", "Chromium";v="119", "Not?A_Brand";v="24"',
+            'authority': 'chat-gpt.org',
+            'accept': '*/*',
+            'accept-language': 'en,fr-FR;q=0.9,fr;q=0.8,es-ES;q=0.7,es;q=0.6,en-US;q=0.5,am;q=0.4,de;q=0.3',
+            'content-type': 'application/json',
+            'origin': 'https://chat-gpt.org',
+            'referer': 'https://chat-gpt.org/chat',
+            'sec-ch-ua': '"Chromium";v="118", "Google Chrome";v="118", "Not=A?Brand";v="99"',
             'sec-ch-ua-mobile': '?0',
             'sec-ch-ua-platform': '"macOS"',
+            'sec-fetch-dest': 'empty',
+            'sec-fetch-mode': 'cors',
+            'sec-fetch-site': 'same-origin',
+            'user-agent': 'Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/118.0.0.0 Safari/537.36',
         }
-        if auth:
-            headers['Authorization'] = f"bearer {auth}" 
-            
+
         async with StreamSession(headers=headers,
-            timeout=timeout,
-            proxies={"https": proxy},
-            impersonate="chrome110"
-        ) as session:
+                                    cookies=cookies,
+                                    timeout=6,
+                                    proxies={"https": proxy} if proxy else None,
+                                    impersonate="chrome110", verify=False) as session:
+
             json_data = {
-                'model'   : cls.get_model(model),
-                'messages': messages,
-                'temperature': kwargs.get("temperature", 0.7),
-                'max_tokens': kwargs.get("max_tokens", 512),
-                'stop': kwargs.get("stop", []),
-                'stream'  : True
+                "message": format_prompt(messages),
+                "temperature": kwargs.get('temperature', 0.5),
+                "presence_penalty": 0,
+                "top_p": kwargs.get('top_p', 1),
+                "frequency_penalty": 0,
             }
-            async with session.post('https://api.deepinfra.com/v1/openai/chat/completions',
+
+            async with session.post("https://chat-gpt.org/api/text",
                                     json=json_data) as response:
+
                 response.raise_for_status()
-                first = True
-                async for line in response.iter_lines():
-                    if not line.startswith(b"data: "):
-                        continue
-                    try:
-                        json_line = json.loads(line[6:])
-                        choices = json_line.get("choices", [{}])
-                        finish_reason = choices[0].get("finish_reason")
-                        if finish_reason:
-                            break
-                        token = choices[0].get("delta", {}).get("content")
-                        if token:
-                            if first:
-                                token = token.lstrip()
-                            if token:
-                                first = False
-                                yield token
-                    except Exception:
-                        raise RuntimeError(f"Response: {line}")
+                result = await response.json()
+
+                if not result['response']:
+                    raise Exception(f"Error Response: {result}")
+
+                return result["message"]
```

### Comparing `g4f-0.2.8.0/g4f/Provider/FlowGpt.py` & `g4f-0.2.8.1/g4f/Provider/FlowGpt.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 import json
 from aiohttp import ClientSession
 
 from ..typing import AsyncResult, Messages
 from .base_provider import AsyncGeneratorProvider, ProviderModelMixin
-from ..errors import RateLimitError
+from ..requests.raise_for_status import raise_for_status
 
 class FlowGpt(AsyncGeneratorProvider, ProviderModelMixin):
     url = "https://flowgpt.com/chat"
     working = True
     supports_gpt_35_turbo = True
     supports_message_history = True
     supports_system_message = True
@@ -66,17 +66,15 @@
                 "promptId": f"model-{model}",
                 "documentIds": [],
                 "chatFileDocumentIds": [],
                 "generateImage": False,
                 "generateAudio": False
             }
             async with session.post("https://backend-k8s.flowgpt.com/v2/chat-anonymous", json=data, proxy=proxy) as response:
-                if response.status == 429:
-                    raise RateLimitError("Rate limit reached")
-                response.raise_for_status()
+                await raise_for_status(response)
                 async for chunk in response.content:
                     if chunk.strip():
                         message = json.loads(chunk)
                         if "event" not in message:
                             continue
                         if message["event"] == "text":
                             yield message["data"]
```

### Comparing `g4f-0.2.8.0/g4f/Provider/FreeChatgpt.py` & `g4f-0.2.8.1/g4f/Provider/FreeChatgpt.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 
 import json
 from aiohttp import ClientSession, ClientTimeout
 
 from ..typing import AsyncResult, Messages
 from .base_provider import AsyncGeneratorProvider, ProviderModelMixin
+from ..requests.raise_for_status import raise_for_status
 
 class FreeChatgpt(AsyncGeneratorProvider, ProviderModelMixin):
     url = "https://free.chatgpt.org.uk"
     working = True
     supports_message_history = True
     default_model = "google-gemini-pro"
 
@@ -41,15 +42,15 @@
                 "model": cls.get_model(""),
                 "temperature": kwargs.get("temperature", 0.5),
                 "presence_penalty": kwargs.get("presence_penalty", 0),
                 "frequency_penalty": kwargs.get("frequency_penalty", 0),
                 "top_p": kwargs.get("top_p", 1)
             }
             async with session.post(f'{cls.url}/api/openai/v1/chat/completions', json=data, proxy=proxy) as response:
-                response.raise_for_status()
+                await raise_for_status(response)
                 started = False
                 async for line in response.content:
                     if line.startswith(b"data: [DONE]"):
                         break
                     elif line.startswith(b"data: "):
                         line = json.loads(line[6:])
                         if(line["choices"]==[]):
```

### Comparing `g4f-0.2.8.0/g4f/Provider/FreeGpt.py` & `g4f-0.2.8.1/g4f/Provider/deprecated/Aibn.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,55 +1,46 @@
 from __future__ import annotations
 
-import time, hashlib, random
+import time
+import hashlib
 
-from ..typing import AsyncResult, Messages
-from ..requests import StreamSession
-from .base_provider import AsyncGeneratorProvider
-from ..errors import RateLimitError
-
-domains = [
-    "https://s.aifree.site",
-    "https://v.aifree.site/"
-]
-
-class FreeGpt(AsyncGeneratorProvider):
-    url = "https://freegptsnav.aifree.site"
-    working = True
+from ...typing import AsyncResult, Messages
+from ...requests import StreamSession
+from ..base_provider import AsyncGeneratorProvider
+
+
+class Aibn(AsyncGeneratorProvider):
+    url = "https://aibn.cc"
+    working = False
     supports_message_history = True
-    supports_system_message = True
     supports_gpt_35_turbo = True
 
     @classmethod
     async def create_async_generator(
         cls,
         model: str,
         messages: Messages,
         proxy: str = None,
         timeout: int = 120,
         **kwargs
     ) -> AsyncResult:
         async with StreamSession(
             impersonate="chrome107",
-            timeout=timeout,
-            proxies={"https": proxy}
+            proxies={"https": proxy},
+            timeout=timeout
         ) as session:
-            prompt = messages[-1]["content"]
             timestamp = int(time.time())
             data = {
                 "messages": messages,
-                "time": timestamp,
                 "pass": None,
-                "sign": generate_signature(timestamp, prompt)
+                "sign": generate_signature(timestamp, messages[-1]["content"]),
+                "time": timestamp
             }
-            domain = random.choice(domains)
-            async with session.post(f"{domain}/api/generate", json=data) as response:
+            async with session.post(f"{cls.url}/api/generate", json=data) as response:
                 response.raise_for_status()
                 async for chunk in response.iter_content():
-                    chunk = chunk.decode()
-                    if chunk == "当前地区当日额度已消耗完":
-                        raise RateLimitError("Rate limit reached")
-                    yield chunk
+                    yield chunk.decode()
     
-def generate_signature(timestamp: int, message: str, secret: str = ""):
+
+def generate_signature(timestamp: int, message: str, secret: str = "undefined"):
     data = f"{timestamp}:{message}:{secret}"
-    return hashlib.sha256(data.encode()).hexdigest()
+    return hashlib.sha256(data.encode()).hexdigest()
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `g4f-0.2.8.0/g4f/Provider/GeminiPro.py` & `g4f-0.2.8.1/g4f/Provider/GeminiPro.py`

 * *Files 6% similar despite different names*

```diff
@@ -72,27 +72,27 @@
                     "topK": kwargs.get("top_k"),
                 }
             }
             async with session.post(url, params=params, json=data) as response:
                 if not response.ok:
                     data = await response.json()
                     data = data[0] if isinstance(data, list) else data
-                    raise RuntimeError(data["error"]["message"])
+                    raise RuntimeError(f"Response {response.status}: {data['error']['message']}")
                 if stream:
                     lines = []
                     async for chunk in response.content:
                         if chunk == b"[{\n":
                             lines = [b"{\n"]
                         elif chunk == b",\r\n" or chunk == b"]":
                             try:
                                 data = b"".join(lines)
                                 data = json.loads(data)
                                 yield data["candidates"][0]["content"]["parts"][0]["text"]
                             except:
-                                data = data.decode() if isinstance(data, bytes) else data
+                                data = data.decode(errors="ignore") if isinstance(data, bytes) else data
                                 raise RuntimeError(f"Read chunk failed: {data}")
                             lines = []
                         else:
                             lines.append(chunk)
                 else:
                     data = await response.json()
                     yield data["candidates"][0]["content"]["parts"][0]["text"]
```

### Comparing `g4f-0.2.8.0/g4f/Provider/GeminiProChat.py` & `g4f-0.2.8.1/g4f/Provider/GeminiProChat.py`

 * *Files 8% similar despite different names*

```diff
@@ -51,13 +51,13 @@
             }
             async with session.post(f"{cls.url}/api/generate", json=data, proxy=proxy) as response:
                 if response.status == 500:
                     if "Quota exceeded" in await response.text():
                         raise RateLimitError(f"Response {response.status}: Rate limit reached")
                 await raise_for_status(response)
                 async for chunk in response.content.iter_any():
-                    yield chunk.decode()
+                    yield chunk.decode(errors="ignore")
                         
 def generate_signature(time: int, text: str, secret: str = ""):
     message = f'{time}:{text}:{secret}';
     return sha256(message.encode()).hexdigest()
```

### Comparing `g4f-0.2.8.0/g4f/Provider/GigaChat.py` & `g4f-0.2.8.1/g4f/Provider/GigaChat.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.0/g4f/Provider/GptTalkRu.py` & `g4f-0.2.8.1/g4f/Provider/GptTalkRu.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,15 @@
                     "randomMessage": random_string,
                     "shifrText": encrypt(public_key, random_string)
                 }
             }
             async with session.post(f"{cls.url}/gpt2", json=data, proxy=proxy) as response:
                 await raise_for_status(response)
                 async for chunk in response.content.iter_any():
-                   yield chunk.decode()
+                   yield chunk.decode(errors="ignore")
 
 def encrypt(public_key: str, value: str) -> str:
     from Crypto.Cipher import PKCS1_v1_5
     from Crypto.PublicKey import RSA
     import base64
     rsa_key = RSA.importKey(public_key)
     cipher = PKCS1_v1_5.new(rsa_key)
```

### Comparing `g4f-0.2.8.0/g4f/Provider/HuggingChat.py` & `g4f-0.2.8.1/g4f/Provider/HuggingChat.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from __future__ import annotations
 
 import json
 import requests
 from aiohttp import ClientSession, BaseConnector
 
 from ..typing import AsyncResult, Messages
+from ..requests.raise_for_status import raise_for_status
 from .base_provider import AsyncGeneratorProvider, ProviderModelMixin
 from .helper import format_prompt, get_connector
 
-
 class HuggingChat(AsyncGeneratorProvider, ProviderModelMixin):
     url = "https://huggingface.co/chat"
     working = True
     default_model = "meta-llama/Llama-2-70b-chat-hf"
     models = [
         "mistralai/Mixtral-8x7B-Instruct-v0.1",
         "google/gemma-7b-it",
@@ -56,40 +56,40 @@
             'User-Agent': 'Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/111.0.0.0 Safari/537.36',
         }
         async with ClientSession(
             cookies=cookies,
             headers=headers,
             connector=get_connector(connector, proxy)
         ) as session:
-            async with session.post(f"{cls.url}/conversation", json=options, proxy=proxy) as response:
-                response.raise_for_status()
+            async with session.post(f"{cls.url}/conversation", json=options) as response:
+                await raise_for_status(response)
                 conversation_id = (await response.json())["conversationId"]
             async with session.get(f"{cls.url}/conversation/{conversation_id}/__data.json") as response:
-                response.raise_for_status()
+                await raise_for_status(response)
                 data: list = (await response.json())["nodes"][1]["data"]
                 keys: list[int] = data[data[0]["messages"]]
                 message_keys: dict = data[keys[0]]
                 message_id: str = data[message_keys["id"]]
             options = {
                 "id": message_id,
                 "inputs": format_prompt(messages),
                 "is_continue": False,
                 "is_retry": False,
                 "web_search": web_search
             }
             async with session.post(f"{cls.url}/conversation/{conversation_id}", json=options) as response:
                 first_token = True
                 async for line in response.content:
-                    response.raise_for_status()
+                    await raise_for_status(response)
                     line = json.loads(line)
                     if "type" not in line:
                         raise RuntimeError(f"Response: {line}")
                     elif line["type"] == "stream":
                         token = line["token"]
                         if first_token:
                             token = token.lstrip()
                             first_token = False
                         yield token
                     elif line["type"] == "finalAnswer":
                         break
-            async with session.delete(f"{cls.url}/conversation/{conversation_id}", proxy=proxy) as response:
-                response.raise_for_status()
+            async with session.delete(f"{cls.url}/conversation/{conversation_id}") as response:
+                await raise_for_status(response)
```

### Comparing `g4f-0.2.8.0/g4f/Provider/HuggingFace.py` & `g4f-0.2.8.1/g4f/Provider/HuggingFace.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.0/g4f/Provider/Koala.py` & `g4f-0.2.8.1/g4f/Provider/Koala.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.0/g4f/Provider/Liaobots.py` & `g4f-0.2.8.1/g4f/Provider/Liaobots.py`

 * *Files 2% similar despite different names*

```diff
@@ -120,22 +120,20 @@
             cookie_jar=cls._cookie_jar,
             connector=get_connector(connector, proxy, True)
         ) as session:
             cls._auth_code = auth if isinstance(auth, str) else cls._auth_code
             if not cls._auth_code:
                 async with session.post(
                     "https://liaobots.work/recaptcha/api/login",
-                    proxy=proxy,
                     data={"token": "abcdefghijklmnopqrst"},
                     verify_ssl=False
                 ) as response:
                     await raise_for_status(response)
                 async with session.post(
                     "https://liaobots.work/api/user",
-                    proxy=proxy,
                     json={"authcode": ""},
                     verify_ssl=False
                 ) as response:
                     await raise_for_status(response)
                     cls._auth_code = (await response.json(content_type=None))["authCode"]
                     cls._cookie_jar = session.cookie_jar
 
@@ -144,18 +142,17 @@
                 "model": models[cls.get_model(model)],
                 "messages": messages,
                 "key": "",
                 "prompt": kwargs.get("system_message", "You are ChatGPT, a large language model trained by OpenAI. Follow the user's instructions carefully."),
             }
             async with session.post(
                 "https://liaobots.work/api/chat",
-                proxy=proxy,
                 json=data,
                 headers={"x-auth-code": cls._auth_code},
                 verify_ssl=False
             ) as response:
                 await raise_for_status(response)
                 async for chunk in response.content.iter_any():
                     if b"<html coupert-item=" in chunk:
                         raise RuntimeError("Invalid session")
                     if chunk:
-                        yield chunk.decode()
+                        yield chunk.decode(errors="ignore")
```

### Comparing `g4f-0.2.8.0/g4f/Provider/Llama2.py` & `g4f-0.2.8.1/g4f/Provider/Llama2.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 
 from aiohttp import ClientSession
 
 from ..typing import AsyncResult, Messages
+from ..requests.raise_for_status import raise_for_status
 from .base_provider import AsyncGeneratorProvider, ProviderModelMixin
 
 
 class Llama2(AsyncGeneratorProvider, ProviderModelMixin):
     url = "https://www.llama2.ai"
     working = True
     supports_message_history = True
@@ -63,16 +64,18 @@
                 "temperature": temperature,
                 "topP": top_p,
                 "maxTokens": max_tokens,
                 "image": None
             }
             started = False
             async with session.post(f"{cls.url}/api", json=data, proxy=proxy) as response:
-                response.raise_for_status()
+                await raise_for_status(response)
                 async for chunk in response.content.iter_any():
+                    if not chunk:
+                        continue
                     if not started:
                         chunk = chunk.lstrip()
                         started = True
                     yield chunk.decode(errors="ignore")
             
 def format_prompt(messages: Messages):
     messages = [
```

### Comparing `g4f-0.2.8.0/g4f/Provider/PerplexityLabs.py` & `g4f-0.2.8.1/g4f/Provider/PerplexityLabs.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.0/g4f/Provider/Pi.py` & `g4f-0.2.8.1/g4f/Provider/Pi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.0/g4f/Provider/Vercel.py` & `g4f-0.2.8.1/g4f/Provider/Vercel.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,15 @@
         for _ in range(max_retries):
             response = requests.post('https://chat.vercel.ai/api/chat', 
                                     headers=headers, json=json_data, stream=True, proxies={"https": proxy})
             if not response.ok:
                 continue
             for token in response.iter_content(chunk_size=None):
                 try:
-                    yield token.decode()
+                    yield token.decode(errors="ignore")
                 except UnicodeDecodeError:
                     pass
             break
         raise_for_status(response)
 
 def get_anti_bot_token() -> str:
     headers = {
```

### Comparing `g4f-0.2.8.0/g4f/Provider/You.py` & `g4f-0.2.8.1/g4f/Provider/You.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,14 +13,16 @@
 from ..typing import AsyncResult, Messages, ImageType, Cookies
 from .base_provider import AsyncGeneratorProvider, ProviderModelMixin
 from .helper import format_prompt
 from ..image import to_bytes, ImageResponse
 from ..requests import StreamSession, raise_for_status
 from ..errors import MissingRequirementsError
 
+from .you.har_file import get_dfp_telemetry_id
+
 class You(AsyncGeneratorProvider, ProviderModelMixin):
     url = "https://you.com"
     working = True
     supports_gpt_35_turbo = True
     supports_gpt_4 = True
     default_model = "gpt-3.5-turbo"
     models = [
@@ -41,26 +43,27 @@
     _cookies_used = 0
 
     @classmethod
     async def create_async_generator(
         cls,
         model: str,
         messages: Messages,
+        stream: bool = True,
         image: ImageType = None,
         image_name: str = None,
         proxy: str = None,
         chat_mode: str = "default",
         **kwargs,
     ) -> AsyncResult:
         if not has_curl_cffi:
             raise MissingRequirementsError('Install "curl_cffi" package')
         if image is not None:
             chat_mode = "agent"
         elif not model or model == cls.default_model:
-            chat_mode = "default"
+            ...
         elif model.startswith("dall-e"):
             chat_mode = "create"
         else:
             chat_mode = "custom"
             model = cls.get_model(model)
         async with StreamSession(
             proxy=proxy,
@@ -104,15 +107,15 @@
                     if line.startswith(b'event: '):
                         event = line[7:].decode()
                     elif line.startswith(b'data: '):
                         if event in ["youChatUpdate", "youChatToken"]:
                             data = json.loads(line[6:])
                         if event == "youChatToken" and event in data:
                             yield data[event]
-                        elif event == "youChatUpdate" and "t" in data:
+                        elif event == "youChatUpdate" and "t" in data and data["t"] is not None:
                             match = re.search(r"!\[fig\]\((.+?)\)", data["t"])
                             if match:
                                 yield ImageResponse(match.group(1), messages[-1]["content"])
                             else:
                                 yield data["t"]                         
 
     @classmethod
@@ -173,20 +176,22 @@
             "https://web.stytch.com/sdk/v1/passwords",
             headers={
                 "Authorization": cls.get_auth(),
                 "X-SDK-Client": cls.get_sdk(),
                 "X-SDK-Parent-Host": cls.url
             },
             json={
+                "dfp_telemetry_id": await get_dfp_telemetry_id(),
                 "email": f"{user_uuid}@gmail.com",
                 "password": f"{user_uuid}#{user_uuid}",
+                "dfp_telemetry_id": f"{uuid.uuid4()}",
                 "session_duration_minutes": 129600
             }
         ) as response:
             await raise_for_status(response)
             session = (await response.json())["data"]
         return {
             "stytch_session": session["session_token"],
             'stytch_session_jwt': session["session_jwt"],
             'ydc_stytch_session': session["session_token"],
             'ydc_stytch_session_jwt': session["session_jwt"],
-        }
+        }
```

### Comparing `g4f-0.2.8.0/g4f/Provider/__init__.py` & `g4f-0.2.8.1/g4f/Provider/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 from .GeminiProChat    import GeminiProChat
 from .GptTalkRu        import GptTalkRu
 from .HuggingChat      import HuggingChat
 from .HuggingFace      import HuggingFace
 from .Koala            import Koala
 from .Liaobots         import Liaobots
 from .Llama2           import Llama2
+from .Local            import Local
 from .PerplexityLabs   import PerplexityLabs
 from .Pi               import Pi
 from .Vercel           import Vercel
 from .You              import You
 
 import sys
```

### Comparing `g4f-0.2.8.0/g4f/Provider/bing/conversation.py` & `g4f-0.2.8.1/g4f/Provider/bing/conversation.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.0/g4f/Provider/bing/create_images.py` & `g4f-0.2.8.1/g4f/Provider/bing/create_images.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.0/g4f/Provider/bing/upload_image.py` & `g4f-0.2.8.1/g4f/Provider/bing/upload_image.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.0/g4f/Provider/deprecated/Acytoo.py` & `g4f-0.2.8.1/g4f/Provider/deprecated/Acytoo.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.0/g4f/Provider/deprecated/AiAsk.py` & `g4f-0.2.8.1/g4f/Provider/deprecated/AiAsk.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.0/g4f/Provider/deprecated/AiChatOnline.py` & `g4f-0.2.8.1/g4f/Provider/deprecated/AiChatOnline.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.0/g4f/Provider/deprecated/AiService.py` & `g4f-0.2.8.1/g4f/Provider/deprecated/AiService.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.0/g4f/Provider/deprecated/Aibn.py` & `g4f-0.2.8.1/g4f/Provider/not_working/GptChatly.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,46 +1,35 @@
 from __future__ import annotations
 
-import time
-import hashlib
+from ...requests import Session, get_session_from_browser
+from ...typing       import Messages
+from ..base_provider import AsyncProvider
 
-from ...typing import AsyncResult, Messages
-from ...requests import StreamSession
-from ..base_provider import AsyncGeneratorProvider
 
-
-class Aibn(AsyncGeneratorProvider):
-    url = "https://aibn.cc"
+class GptChatly(AsyncProvider):
+    url = "https://gptchatly.com"
     working = False
     supports_message_history = True
     supports_gpt_35_turbo = True
 
     @classmethod
-    async def create_async_generator(
+    async def create_async(
         cls,
         model: str,
         messages: Messages,
         proxy: str = None,
         timeout: int = 120,
+        session: Session = None,
         **kwargs
-    ) -> AsyncResult:
-        async with StreamSession(
-            impersonate="chrome107",
-            proxies={"https": proxy},
-            timeout=timeout
-        ) as session:
-            timestamp = int(time.time())
-            data = {
-                "messages": messages,
-                "pass": None,
-                "sign": generate_signature(timestamp, messages[-1]["content"]),
-                "time": timestamp
-            }
-            async with session.post(f"{cls.url}/api/generate", json=data) as response:
-                response.raise_for_status()
-                async for chunk in response.iter_content():
-                    yield chunk.decode()
-    
-
-def generate_signature(timestamp: int, message: str, secret: str = "undefined"):
-    data = f"{timestamp}:{message}:{secret}"
-    return hashlib.sha256(data.encode()).hexdigest()
+    ) -> str:
+        if not session:
+            session = get_session_from_browser(cls.url, proxy=proxy, timeout=timeout)
+        if model.startswith("gpt-4"):
+            chat_url = f"{cls.url}/fetch-gpt4-response"
+        else:
+            chat_url = f"{cls.url}/felch-response"
+        data = {
+            "past_conversations": messages
+        }
+        response = session.post(chat_url, json=data)
+        response.raise_for_status()
+        return response.json()["chatGPTResponse"]
```

### Comparing `g4f-0.2.8.0/g4f/Provider/deprecated/Aichat.py` & `g4f-0.2.8.1/g4f/Provider/not_working/AItianhu.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,64 +1,79 @@
 from __future__ import annotations
 
-from ...typing import Messages
-from ..base_provider import AsyncProvider, format_prompt
-from ..helper import get_cookies
+import json
+
+from ...typing import AsyncResult, Messages
 from ...requests import StreamSession
+from ..base_provider import AsyncGeneratorProvider, format_prompt, get_cookies
+
 
-class Aichat(AsyncProvider):
-    url = "https://chat-gpt.org/chat"
+class AItianhu(AsyncGeneratorProvider):
+    url = "https://www.aitianhu.com"
     working = False
     supports_gpt_35_turbo = True
 
-    @staticmethod
-    async def create_async(
+    @classmethod
+    async def create_async_generator(
+        cls,
         model: str,
         messages: Messages,
-        proxy: str = None, **kwargs) -> str:
+        proxy: str = None,
+        cookies: dict = None,
+        timeout: int = 120, **kwargs) -> AsyncResult:
         
-        cookies = get_cookies('chat-gpt.org') if not kwargs.get('cookies') else kwargs.get('cookies')
         if not cookies:
-            raise RuntimeError(
-                "g4f.provider.Aichat requires cookies, [refresh https://chat-gpt.org on chrome]"
-            )
+            cookies = get_cookies(domain_name='www.aitianhu.com')
+        if not cookies:
+            raise RuntimeError(f"g4f.provider.{cls.__name__} requires cookies [refresh https://www.aitianhu.com on chrome]")
+
+        data = {
+            "prompt": format_prompt(messages),
+            "options": {},
+            "systemMessage": "You are ChatGPT, a large language model trained by OpenAI. Follow the user's instructions carefully.",
+            "temperature": 0.8,
+            "top_p": 1,
+            **kwargs
+        }
 
         headers = {
-            'authority': 'chat-gpt.org',
-            'accept': '*/*',
+            'authority': 'www.aitianhu.com',
+            'accept': 'application/json, text/plain, */*',
             'accept-language': 'en,fr-FR;q=0.9,fr;q=0.8,es-ES;q=0.7,es;q=0.6,en-US;q=0.5,am;q=0.4,de;q=0.3',
             'content-type': 'application/json',
-            'origin': 'https://chat-gpt.org',
-            'referer': 'https://chat-gpt.org/chat',
+            'origin': 'https://www.aitianhu.com',
+            'referer': 'https://www.aitianhu.com/',
             'sec-ch-ua': '"Chromium";v="118", "Google Chrome";v="118", "Not=A?Brand";v="99"',
             'sec-ch-ua-mobile': '?0',
             'sec-ch-ua-platform': '"macOS"',
             'sec-fetch-dest': 'empty',
             'sec-fetch-mode': 'cors',
             'sec-fetch-site': 'same-origin',
             'user-agent': 'Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/118.0.0.0 Safari/537.36',
         }
 
         async with StreamSession(headers=headers,
-                                    cookies=cookies,
-                                    timeout=6,
-                                    proxies={"https": proxy} if proxy else None,
-                                    impersonate="chrome110", verify=False) as session:
-
-            json_data = {
-                "message": format_prompt(messages),
-                "temperature": kwargs.get('temperature', 0.5),
-                "presence_penalty": 0,
-                "top_p": kwargs.get('top_p', 1),
-                "frequency_penalty": 0,
-            }
-
-            async with session.post("https://chat-gpt.org/api/text",
-                                    json=json_data) as response:
-
+                                        cookies=cookies,
+                                        timeout=timeout,
+                                        proxies={"https": proxy},
+                                        impersonate="chrome107", verify=False) as session:
+            
+            async with session.post(f"{cls.url}/api/chat-process", json=data) as response:
                 response.raise_for_status()
-                result = await response.json()
-
-                if not result['response']:
-                    raise Exception(f"Error Response: {result}")
 
-                return result["message"]
+                async for line in response.iter_lines():
+                    if line == b"<script>":
+                        raise RuntimeError("Solve challenge and pass cookies")
+
+                    if b"platform's risk control" in line:
+                        raise RuntimeError("Platform's Risk Control")
+
+                    line = json.loads(line)
+
+                    if "detail" not in line:
+                        raise RuntimeError(f"Response: {line}")
+
+                    content = line["detail"]["choices"][0]["delta"].get(
+                        "content"
+                    )
+                    if content:
+                        yield content
```

### Comparing `g4f-0.2.8.0/g4f/Provider/deprecated/Ails.py` & `g4f-0.2.8.1/g4f/Provider/deprecated/Ails.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.0/g4f/Provider/deprecated/Aivvm.py` & `g4f-0.2.8.1/g4f/Provider/deprecated/Aivvm.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.0/g4f/Provider/deprecated/Berlin.py` & `g4f-0.2.8.1/g4f/Provider/deprecated/Berlin.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.0/g4f/Provider/deprecated/ChatAnywhere.py` & `g4f-0.2.8.1/g4f/Provider/deprecated/ChatAnywhere.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.0/g4f/Provider/deprecated/ChatgptDuo.py` & `g4f-0.2.8.1/g4f/Provider/deprecated/ChatgptDuo.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.0/g4f/Provider/deprecated/CodeLinkAva.py` & `g4f-0.2.8.1/g4f/Provider/deprecated/CodeLinkAva.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.0/g4f/Provider/deprecated/Cromicle.py` & `g4f-0.2.8.1/g4f/Provider/deprecated/Cromicle.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.0/g4f/Provider/deprecated/DfeHub.py` & `g4f-0.2.8.1/g4f/Provider/deprecated/DfeHub.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.0/g4f/Provider/deprecated/EasyChat.py` & `g4f-0.2.8.1/g4f/Provider/deprecated/EasyChat.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.0/g4f/Provider/deprecated/Equing.py` & `g4f-0.2.8.1/g4f/Provider/deprecated/Equing.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.0/g4f/Provider/deprecated/FakeGpt.py` & `g4f-0.2.8.1/g4f/Provider/deprecated/FakeGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.0/g4f/Provider/deprecated/FastGpt.py` & `g4f-0.2.8.1/g4f/Provider/deprecated/FastGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.0/g4f/Provider/deprecated/Forefront.py` & `g4f-0.2.8.1/g4f/Provider/deprecated/Forefront.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.0/g4f/Provider/deprecated/GPTalk.py` & `g4f-0.2.8.1/g4f/Provider/deprecated/GPTalk.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.0/g4f/Provider/deprecated/GeekGpt.py` & `g4f-0.2.8.1/g4f/Provider/deprecated/GeekGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.0/g4f/Provider/deprecated/GetGpt.py` & `g4f-0.2.8.1/g4f/Provider/deprecated/GetGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.0/g4f/Provider/deprecated/H2o.py` & `g4f-0.2.8.1/g4f/Provider/deprecated/H2o.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.0/g4f/Provider/deprecated/Hashnode.py` & `g4f-0.2.8.1/g4f/Provider/deprecated/Hashnode.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.0/g4f/Provider/deprecated/Lockchat.py` & `g4f-0.2.8.1/g4f/Provider/deprecated/Lockchat.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.0/g4f/Provider/deprecated/Myshell.py` & `g4f-0.2.8.1/g4f/Provider/deprecated/Myshell.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.0/g4f/Provider/deprecated/NoowAi.py` & `g4f-0.2.8.1/g4f/Provider/deprecated/NoowAi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.0/g4f/Provider/deprecated/Opchatgpts.py` & `g4f-0.2.8.1/g4f/Provider/deprecated/Opchatgpts.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.0/g4f/Provider/deprecated/Phind.py` & `g4f-0.2.8.1/g4f/Provider/deprecated/Phind.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.0/g4f/Provider/deprecated/V50.py` & `g4f-0.2.8.1/g4f/Provider/deprecated/V50.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.0/g4f/Provider/deprecated/Vercel.py` & `g4f-0.2.8.1/g4f/Provider/deprecated/Vercel.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.0/g4f/Provider/deprecated/Vitalentum.py` & `g4f-0.2.8.1/g4f/Provider/deprecated/Vitalentum.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.0/g4f/Provider/deprecated/VoiGpt.py` & `g4f-0.2.8.1/g4f/Provider/deprecated/VoiGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.0/g4f/Provider/deprecated/Wewordle.py` & `g4f-0.2.8.1/g4f/Provider/deprecated/Wewordle.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.0/g4f/Provider/deprecated/Wuguokai.py` & `g4f-0.2.8.1/g4f/Provider/deprecated/Wuguokai.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.0/g4f/Provider/deprecated/Ylokh.py` & `g4f-0.2.8.1/g4f/Provider/deprecated/Ylokh.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.0/g4f/Provider/deprecated/Yqcloud.py` & `g4f-0.2.8.1/g4f/Provider/deprecated/Yqcloud.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.0/g4f/Provider/deprecated/__init__.py` & `g4f-0.2.8.1/g4f/Provider/deprecated/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -27,8 +27,9 @@
 from .AiAsk         import AiAsk
 from .AiChatOnline  import AiChatOnline
 from .ChatAnywhere  import ChatAnywhere
 from .FakeGpt       import FakeGpt
 from .GeekGpt       import GeekGpt
 from .GPTalk        import GPTalk
 from .Hashnode      import Hashnode
-from .Ylokh         import Ylokh
+from .Ylokh         import Ylokh
+from .OpenAssistant import OpenAssistant
```

### Comparing `g4f-0.2.8.0/g4f/Provider/gigachat_crt/russian_trusted_root_ca_pem.crt` & `g4f-0.2.8.1/g4f/Provider/gigachat_crt/russian_trusted_root_ca_pem.crt`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.0/g4f/Provider/needs_auth/Gemini.py` & `g4f-0.2.8.1/g4f/Provider/needs_auth/Gemini.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     from selenium.webdriver.support import expected_conditions as EC
 except ImportError:
     pass
 
 from ...typing import Messages, Cookies, ImageType, AsyncResult
 from ..base_provider import AsyncGeneratorProvider
 from ..helper import format_prompt, get_cookies
+from ...requests.raise_for_status import raise_for_status
 from ...errors import MissingAuthError, MissingRequirementsError
 from ...image import to_bytes, ImageResponse
 from ...webdriver import get_browser, get_driver_cookies
 
 REQUEST_HEADERS = {
     "authority": "gemini.google.com",
     "origin": "https://gemini.google.com",
@@ -124,14 +125,15 @@
                     ))])
                 }
                 async with client.post(
                     REQUEST_URL,
                     data=data,
                     params=params,
                 ) as response:
+                    await raise_for_status(response)
                     response = await response.text()
                     response_part = json.loads(json.loads(response.splitlines()[-5])[0][2])
                     if response_part[4] is None:
                         response_part = json.loads(json.loads(response.splitlines()[-7])[0][2])
 
                     content = response_part[4][0][1][0]
                     image_prompt = None
@@ -181,38 +183,39 @@
 
     async def upload_image(connector: BaseConnector, image: bytes, image_name: str = None):
         async with ClientSession(
             headers=UPLOAD_IMAGE_HEADERS,
             connector=connector
         ) as session:
             async with session.options(UPLOAD_IMAGE_URL) as reponse:
-                reponse.raise_for_status()
+                await raise_for_status(response)
 
             headers = {
                 "size": str(len(image)),
                 "x-goog-upload-command": "start"
             }
             data = f"File name: {image_name}" if image_name else None
             async with session.post(
                 UPLOAD_IMAGE_URL, headers=headers, data=data
             ) as response:
-                response.raise_for_status()
+                await raise_for_status(response)
                 upload_url = response.headers["X-Goog-Upload-Url"]
 
             async with session.options(upload_url, headers=headers) as response:
-                response.raise_for_status()
+                await raise_for_status(response)
 
             headers["x-goog-upload-command"] = "upload, finalize"
             headers["X-Goog-Upload-Offset"] = "0"
             async with session.post(
                 upload_url, headers=headers, data=image
             ) as response:
-                response.raise_for_status()
+                await raise_for_status(response)
                 return await response.text()
 
     @classmethod
     async def fetch_snlm0e(cls, session: ClientSession, cookies: Cookies):
         async with session.get(cls.url, cookies=cookies) as response:
+            await raise_for_status(response)
             text = await response.text()
         match = re.search(r'SNlM0e\":\"(.*?)\"', text)
         if match:
             return match.group(1)
```

### Comparing `g4f-0.2.8.0/g4f/Provider/needs_auth/OpenAssistant.py` & `g4f-0.2.8.1/g4f/Provider/deprecated/OpenAssistant.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 
 from aiohttp import ClientSession
 
 from ...typing import AsyncResult, Messages
 from ..base_provider import AsyncGeneratorProvider
 from ..helper import format_prompt, get_cookies
 
-
 class OpenAssistant(AsyncGeneratorProvider):
     url = "https://open-assistant.io/chat"
     needs_auth = True
     working = False
     model = "OA_SFT_Llama_30B_6"
 
     @classmethod
```

### Comparing `g4f-0.2.8.0/g4f/Provider/needs_auth/OpenaiChat.py` & `g4f-0.2.8.1/g4f/Provider/needs_auth/OpenaiChat.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.0/g4f/Provider/needs_auth/Poe.py` & `g4f-0.2.8.1/g4f/Provider/needs_auth/Poe.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.0/g4f/Provider/needs_auth/Raycast.py` & `g4f-0.2.8.1/g4f/Provider/needs_auth/Raycast.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.0/g4f/Provider/needs_auth/Theb.py` & `g4f-0.2.8.1/g4f/Provider/needs_auth/Theb.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.0/g4f/Provider/not_working/Bestim.py` & `g4f-0.2.8.1/g4f/Provider/not_working/Bestim.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.0/g4f/Provider/not_working/ChatBase.py` & `g4f-0.2.8.1/g4f/Provider/not_working/ChatBase.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.0/g4f/Provider/not_working/ChatgptDemo.py` & `g4f-0.2.8.1/g4f/Provider/not_working/ChatgptDemo.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.0/g4f/Provider/not_working/ChatgptDemoAi.py` & `g4f-0.2.8.1/g4f/Provider/not_working/ChatgptDemoAi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.0/g4f/Provider/not_working/ChatgptLogin.py` & `g4f-0.2.8.1/g4f/Provider/not_working/ChatgptLogin.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.0/g4f/Provider/not_working/Chatxyz.py` & `g4f-0.2.8.1/g4f/Provider/not_working/Chatxyz.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.0/g4f/Provider/not_working/Gpt6.py` & `g4f-0.2.8.1/g4f/Provider/not_working/Gpt6.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.0/g4f/Provider/not_working/GptForLove.py` & `g4f-0.2.8.1/g4f/Provider/not_working/GptForLove.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.0/g4f/Provider/not_working/GptGo.py` & `g4f-0.2.8.1/g4f/Provider/not_working/GptGo.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.0/g4f/Provider/not_working/GptGod.py` & `g4f-0.2.8.1/g4f/Provider/not_working/GptGod.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.0/g4f/Provider/not_working/OnlineGpt.py` & `g4f-0.2.8.1/g4f/Provider/not_working/OnlineGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.0/g4f/Provider/npm/node_modules/crypto-js/README.md` & `g4f-0.2.8.1/g4f/Provider/npm/node_modules/crypto-js/README.md`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.0/g4f/Provider/npm/node_modules/crypto-js/crypto-js.js` & `g4f-0.2.8.1/g4f/Provider/npm/node_modules/crypto-js/crypto-js.js`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.0/g4f/Provider/npm/package-lock.json` & `g4f-0.2.8.1/g4f/Provider/npm/package-lock.json`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.0/g4f/Provider/openai/crypt.py` & `g4f-0.2.8.1/g4f/Provider/openai/crypt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.0/g4f/Provider/openai/har_file.py` & `g4f-0.2.8.1/g4f/Provider/openai/har_file.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.0/g4f/Provider/selenium/AItianhuSpace.py` & `g4f-0.2.8.1/g4f/Provider/selenium/AItianhuSpace.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.0/g4f/Provider/selenium/Bard.py` & `g4f-0.2.8.1/g4f/Provider/selenium/Bard.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.0/g4f/Provider/selenium/MyShell.py` & `g4f-0.2.8.1/g4f/Provider/selenium/MyShell.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.0/g4f/Provider/selenium/PerplexityAi.py` & `g4f-0.2.8.1/g4f/Provider/selenium/PerplexityAi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.0/g4f/Provider/selenium/Phind.py` & `g4f-0.2.8.1/g4f/Provider/selenium/Phind.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.0/g4f/Provider/selenium/TalkAi.py` & `g4f-0.2.8.1/g4f/Provider/selenium/TalkAi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.0/g4f/Provider/unfinished/AiChatting.py` & `g4f-0.2.8.1/g4f/Provider/unfinished/AiChatting.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.0/g4f/Provider/unfinished/ChatAiGpt.py` & `g4f-0.2.8.1/g4f/Provider/unfinished/ChatAiGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.0/g4f/Provider/unfinished/Komo.py` & `g4f-0.2.8.1/g4f/Provider/unfinished/Komo.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.0/g4f/Provider/unfinished/MikuChat.py` & `g4f-0.2.8.1/g4f/Provider/unfinished/MikuChat.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.0/g4f/api/__init__.py` & `g4f-0.2.8.1/g4f/api/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 import logging
 import json
 import uvicorn
 import nest_asyncio
 
-from fastapi           import FastAPI, Response, Request
+from fastapi import FastAPI, Response, Request
 from fastapi.responses import StreamingResponse, RedirectResponse, HTMLResponse, JSONResponse
-from pydantic          import BaseModel
-from typing            import List, Union
+from fastapi.exceptions import RequestValidationError
+from starlette.status import HTTP_422_UNPROCESSABLE_ENTITY
+from fastapi.encoders import jsonable_encoder
+from pydantic import BaseModel
+from typing import List, Union
 
 import g4f
 import g4f.debug
 from g4f.client import Client
 from g4f.typing import Messages
 
 class ChatCompletionsConfig(BaseModel):
@@ -35,14 +38,33 @@
             g4f.debug.logging = True
         self.client = Client()
 
         nest_asyncio.apply()
         self.app = FastAPI()
 
         self.routes()
+        self.register_validation_exception_handler()
+
+    def register_validation_exception_handler(self):
+        @self.app.exception_handler(RequestValidationError)
+        async def validation_exception_handler(request: Request, exc: RequestValidationError):
+            details = exc.errors()
+            modified_details = []
+            for error in details:
+                modified_details.append(
+                    {
+                        "loc": error["loc"],
+                        "message": error["msg"],
+                        "type": error["type"],
+                    }
+                )
+            return JSONResponse(
+                status_code=HTTP_422_UNPROCESSABLE_ENTITY,
+                content=jsonable_encoder({"detail": modified_details}),
+            )
 
     def routes(self):
         @self.app.get("/")
         async def read_root():
             return RedirectResponse("/v1", 302)
 
         @self.app.get("/v1")
```

### Comparing `g4f-0.2.8.0/g4f/api/_logging.py` & `g4f-0.2.8.1/g4f/api/_logging.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.0/g4f/cli.py` & `g4f-0.2.8.1/g4f/cli.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.0/g4f/client.py` & `g4f-0.2.8.1/g4f/client/async_client.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,240 +1,202 @@
 from __future__ import annotations
 
-import re
-import os
 import time
 import random
 import string
 
-from .stubs import ChatCompletion, ChatCompletionChunk, Image, ImagesResponse
-from .typing import Union, Iterator, Messages, ImageType
-from .providers.types import BaseProvider, ProviderType
-from .image import ImageResponse as ImageProviderResponse
-from .errors import NoImageResponseError, RateLimitError, MissingAuthError
-from . import get_model_and_provider, get_last_provider
-
-from .Provider.BingCreateImages import BingCreateImages
-from .Provider.needs_auth import Gemini, OpenaiChat
-from .Provider.You import You
-
-ImageProvider = Union[BaseProvider, object]
-Proxies = Union[dict, str]
-IterResponse = Iterator[Union[ChatCompletion, ChatCompletionChunk]]
-
-def read_json(text: str) -> dict:
-    """
-    Parses JSON code block from a string.
-
-    Args:
-        text (str): A string containing a JSON code block.
-
-    Returns:
-        dict: A dictionary parsed from the JSON code block.
-    """
-    match = re.search(r"```(json|)\n(?P<code>[\S\s]+?)\n```", text)
-    if match:
-        return match.group("code")
-    return text
+from .types import Client as BaseClient
+from .types import ProviderType, FinishReason
+from .stubs import ChatCompletion, ChatCompletionChunk, ImagesResponse, Image
+from .types import AsyncIterResponse, ImageProvider
+from .image_models import ImageModels
+from .helper import filter_json, find_stop, filter_none, cast_iter_async
+from .service import get_last_provider, get_model_and_provider
+from ..typing import Union, Iterator, Messages, AsyncIterator, ImageType
+from ..errors import NoImageResponseError
+from ..image import ImageResponse as ImageProviderResponse
+from ..providers.base_provider import AsyncGeneratorProvider
 
-def iter_response(
-    response: iter[str],
+async def iter_response(
+    response: AsyncIterator[str],
     stream: bool,
     response_format: dict = None,
     max_tokens: int = None,
     stop: list = None
-) -> IterResponse:
+) -> AsyncIterResponse:
     content = ""
     finish_reason = None
     completion_id = ''.join(random.choices(string.ascii_letters + string.digits, k=28))
-    for idx, chunk in enumerate(response):
+    count: int = 0
+    async for chunk in response:
+        if isinstance(chunk, FinishReason):
+            finish_reason = chunk.reason
+            break
         content += str(chunk)
-        if max_tokens is not None and idx + 1 >= max_tokens:
+        count += 1
+        if max_tokens is not None and count >= max_tokens:
             finish_reason = "length"
-        first = -1
-        word = None
-        if stop is not None:
-            for word in list(stop):
-                first = content.find(word)
-                if first != -1:
-                    content = content[:first]
-                    break
-            if stream and first != -1:
-                first = chunk.find(word)
-                if first != -1:
-                    chunk = chunk[:first]
-                else:
-                    first = 0
+        first, content, chunk = find_stop(stop, content, chunk)
         if first != -1:
             finish_reason = "stop"
         if stream:
             yield ChatCompletionChunk(chunk, None, completion_id, int(time.time()))
         if finish_reason is not None:
             break
     finish_reason = "stop" if finish_reason is None else finish_reason
     if stream:
         yield ChatCompletionChunk(None, finish_reason, completion_id, int(time.time()))
     else:
         if response_format is not None and "type" in response_format:
             if response_format["type"] == "json_object":
-                content = read_json(content)
+                content = filter_json(content)
         yield ChatCompletion(content, finish_reason, completion_id, int(time.time()))
 
-def iter_append_model_and_provider(response: IterResponse) -> IterResponse:
+async def iter_append_model_and_provider(response: AsyncIterResponse) -> AsyncIterResponse:
     last_provider = None
-    for chunk in response:
+    async for chunk in response:
         last_provider = get_last_provider(True) if last_provider is None else last_provider
         chunk.model = last_provider.get("model")
         chunk.provider =  last_provider.get("name")
         yield chunk
 
-class Client():
-
+class AsyncClient(BaseClient):
     def __init__(
         self,
-        api_key: str = None,
-        proxies: Proxies = None,
         provider: ProviderType = None,
         image_provider: ImageProvider = None,
         **kwargs
-    ) -> None:
-        self.api_key: str = api_key
-        self.proxies: Proxies = proxies
+    ):
+        super().__init__(**kwargs)
         self.chat: Chat = Chat(self, provider)
         self.images: Images = Images(self, image_provider)
 
-    def get_proxy(self) -> Union[str, None]:
-        if isinstance(self.proxies, str):
-            return self.proxies
-        elif self.proxies is None:
-            return os.environ.get("G4F_PROXY")
-        elif "all" in self.proxies:
-            return self.proxies["all"]
-        elif "https" in self.proxies:
-            return self.proxies["https"]
-
-def filter_none(**kwargs):
-    for key in list(kwargs.keys()):
-        if kwargs[key] is None:
-            del kwargs[key]
-    return kwargs
+def create_response(
+    messages: Messages,
+    model: str,
+    provider: ProviderType = None,
+    stream: bool = False,
+    proxy: str = None,
+    max_tokens: int = None,
+    stop: list[str] = None,
+    api_key: str = None,
+    **kwargs
+):
+    has_asnyc = isinstance(provider, type) and issubclass(provider, AsyncGeneratorProvider)
+    if has_asnyc:
+        create = provider.create_async_generator
+    else:
+        create = provider.create_completion
+    response = create(
+        model, messages, stream,            
+        **filter_none(
+            proxy=proxy,
+            max_tokens=max_tokens,
+            stop=stop,
+            api_key=api_key
+        ),
+        **kwargs
+    )
+    if not has_asnyc:
+        response = cast_iter_async(response)
+    return response
 
 class Completions():
-    def __init__(self, client: Client, provider: ProviderType = None):
-        self.client: Client = client
+    def __init__(self, client: AsyncClient, provider: ProviderType = None):
+        self.client: AsyncClient = client
         self.provider: ProviderType = provider
 
     def create(
         self,
         messages: Messages,
         model: str,
         provider: ProviderType = None,
         stream: bool = False,
-        response_format: dict = None,
+        proxy: str = None,
         max_tokens: int = None,
         stop: Union[list[str], str] = None,
         api_key: str = None,
+        response_format: dict = None,
         ignored  : list[str] = None,
         ignore_working: bool = False,
         ignore_stream: bool = False,
         **kwargs
-    ) -> Union[ChatCompletion, Iterator[ChatCompletionChunk]]:
+    ) -> Union[ChatCompletion, AsyncIterator[ChatCompletionChunk]]:
         model, provider = get_model_and_provider(
             model,
             self.provider if provider is None else provider,
             stream,
             ignored,
             ignore_working,
-            ignore_stream,
-            **kwargs
+            ignore_stream
         )
         stop = [stop] if isinstance(stop, str) else stop
-        response = provider.create_completion(
-            model, messages, stream,            
-            **filter_none(
-                proxy=self.client.get_proxy(),
-                max_tokens=max_tokens,
-                stop=stop,
-                api_key=self.client.api_key if api_key is None else api_key
-            ),
+        response = create_response(
+            messages, model,
+            provider, stream,
+            proxy=self.client.get_proxy() if proxy is None else proxy,
+            max_tokens=max_tokens,
+            stop=stop,
+            api_key=self.client.api_key if api_key is None else api_key
             **kwargs
         )
         response = iter_response(response, stream, response_format, max_tokens, stop)
         response = iter_append_model_and_provider(response)
-        return response if stream else next(response)
+        return response if stream else anext(response)
 
 class Chat():
     completions: Completions
 
-    def __init__(self, client: Client, provider: ProviderType = None):
+    def __init__(self, client: AsyncClient, provider: ProviderType = None):
         self.completions = Completions(client, provider)
 
-class ImageModels():
-    gemini = Gemini
-    openai = OpenaiChat
-    you = You
-
-    def __init__(self, client: Client) -> None:
-        self.client = client
-        self.default = BingCreateImages(proxy=self.client.get_proxy())
-
-    def get(self, name: str, default: ImageProvider = None) -> ImageProvider:
-        return getattr(self, name) if hasattr(self, name) else default or self.default
-
-def iter_image_response(response: Iterator) -> Union[ImagesResponse, None]:
-    for chunk in list(response):
+async def iter_image_response(response: Iterator) -> Union[ImagesResponse, None]:
+    async for chunk in response:
         if isinstance(chunk, ImageProviderResponse):
             return ImagesResponse([Image(image) for image in chunk.get_list()])
 
-def create_image(client: Client, provider: ProviderType, prompt: str, model: str = "", **kwargs) -> Iterator:
+def create_image(client: AsyncClient, provider: ProviderType, prompt: str, model: str = "", **kwargs) -> AsyncIterator:
     prompt = f"create a image with: {prompt}"
-    return provider.create_completion(
+    if provider.__name__ == "You":
+        kwargs["chat_mode"] = "create"
+    return provider.create_async_generator(
         model,
         [{"role": "user", "content": prompt}],
-        True,
+        stream=True,
         proxy=client.get_proxy(),
         **kwargs
     )
 
 class Images():
-    def __init__(self, client: Client, provider: ImageProvider = None):
-        self.client: Client = client
+    def __init__(self, client: AsyncClient, provider: ImageProvider = None):
+        self.client: AsyncClient = client
         self.provider: ImageProvider = provider
         self.models: ImageModels = ImageModels(client)
 
-    def generate(self, prompt, model: str = None, **kwargs) -> ImagesResponse:
+    async def generate(self, prompt, model: str = "", **kwargs) -> ImagesResponse:
         provider = self.models.get(model, self.provider)
-        if isinstance(provider, type) and issubclass(provider, BaseProvider):
+        if isinstance(provider, type) and issubclass(provider, AsyncGeneratorProvider):
             response = create_image(self.client, provider, prompt, **kwargs)
         else:
-            try:
-                response = list(provider.create(prompt))
-            except (RateLimitError, MissingAuthError) as e:
-                # Fallback for default provider
-                if self.provider is None:
-                    response = create_image(self.client, self.models.you, prompt, model or "dall-e", **kwargs)
-                else:
-                    raise e
-        image = iter_image_response(response)
+            response = await provider.create_async(prompt)
+            return ImagesResponse([Image(image) for image in response.get_list()])
+        image = await iter_image_response(response)
         if image is None:
             raise NoImageResponseError()
         return image
 
-    def create_variation(self, image: ImageType, model: str = None, **kwargs):
+    async def create_variation(self, image: ImageType, model: str = None, **kwargs):
         provider = self.models.get(model, self.provider)
         result = None
-        if isinstance(provider, type) and issubclass(provider, BaseProvider):
-            response = provider.create_completion(
+        if isinstance(provider, type) and issubclass(provider, AsyncGeneratorProvider):
+            response = provider.create_async_generator(
                 "",
                 [{"role": "user", "content": "create a image like this"}],
                 True,
                 image=image,
                 proxy=self.client.get_proxy(),
                 **kwargs
             )
-            for chunk in response:
-                if isinstance(chunk, ImageProviderResponse):
-                    result = ([chunk.images] if isinstance(chunk.images, str) else chunk.images)
-                    result = ImagesResponse([Image(image)for image in result])
+            result = iter_image_response(response)
         if result is None:
             raise NoImageResponseError()
         return result
```

### Comparing `g4f-0.2.8.0/g4f/cookies.py` & `g4f-0.2.8.1/g4f/cookies.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.0/g4f/errors.py` & `g4f-0.2.8.1/g4f/errors.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,23 +18,23 @@
 
 class RetryNoProviderError(Exception):
     ...
 
 class VersionNotFoundError(Exception):
     ...
 
-class NestAsyncioError(Exception):
-    ...
-
 class ModelNotSupportedError(Exception):
     ...
 
 class MissingRequirementsError(Exception):
     ...
 
+class NestAsyncioError(MissingRequirementsError):
+    ...
+
 class MissingAuthError(Exception):
     ...
 
 class NoImageResponseError(Exception):
     ...
 
 class RateLimitError(Exception):
```

### Comparing `g4f-0.2.8.0/g4f/gui/client/index.html` & `g4f-0.2.8.1/g4f/gui/client/index.html`

 * *Files 20% similar despite different names*

```diff
@@ -37,56 +37,23 @@
         import llamaTokenizer from "llama-tokenizer-js"
     </script>
     <script src="https://unpkg.com/gpt-tokenizer/dist/cl100k_base.js" async></script>
     <script>
         const user_image = '<img src="/static/img/user.png" alt="your avatar">';
         const gpt_image = '<img src="/static/img/gpt.png" alt="your avatar">';
     </script>
-    <style>
-        .hljs {
-            color: #e9e9f4;
-            background: #28293629;
-            border-radius: var(--border-radius-1);
-            border: 1px solid var(--blur-border);
-            font-size: 15px;
-        }
-
-        #message-input {
-            height: 82px;
-            margin-left: 20px;
-        }
-
-        #message-input::-webkit-scrollbar {
-            width: 5px;
-        }
-
-        /* Track */
-        #message-input::-webkit-scrollbar-track {
-            background: #f1f1f1;
-        }
-
-        /* Handle */
-        #message-input::-webkit-scrollbar-thumb {
-            background: #c7a2ff;
-        }
-
-        /* Handle on hover */
-        #message-input::-webkit-scrollbar-thumb:hover {
-            background: #8b3dff;
-        }
-    </style>
     <script src="/static/js/highlight.min.js"></script>
     <script>window.conversation_id = "{{chat_id}}"</script>
     <title>g4f - gui</title>
 </head>
 
 <body>
     <div class="gradient"></div>
     <div class="row">
-        <div class="box conversations">
+        <div class="box conversations hidden">
             <div class="top">
                 <button class="new_convo" onclick="new_conversation()">
                     <i class="fa-regular fa-plus"></i>
                     <span>New Conversation</span>
                 </button>
             </div>
             <div class="bottom_buttons">
@@ -105,14 +72,45 @@
                 </div>
                 <div class="info">
                     <i class="fa-solid fa-star"></i>
                     <span id="version_text" class="convo-title"></span>
                 </div>
             </div>
         </div>
+        <div class="settings">
+            <div class="field box">
+                <label for="OpenaiChat-api_key" class="label" title="">OpenaiChat: access_token</label>
+                <textarea id="OpenaiChat-api_key" name="OpenaiChat[api_key]" placeholder="..."></textarea>
+            </div>
+            <div class="field">
+                <span class="label">OpenaiChat: Auto continue</span>
+                <input id="OpenaiChat-auto_continue" type="checkbox" name="OpenaiChat[auto_continue]" checked/>
+                <label for="OpenaiChat-auto_continue" class="toogle" title=""></label>
+            </div>
+            <div class="field box">
+                <label for="Bing-api_key" class="label" title="">Bing: "_U" cookie</label>
+                <textarea id="Bing-api_key" name="Bing[api_key]" placeholder="..."></textarea>
+            </div>
+            <div class="field box">
+                <label for="Gemini-api_key" class="label" title="">Gemini: Auth cookies</label>
+                <textarea id="Gemini-api_key" name="Gemini[api_key]" placeholder="..."></textarea>
+            </div>
+            <div class="field box">
+                <label for="Openai-api_key" class="label" title="">Openai: api_key</label>
+                <textarea id="Openai-api_key" name="Openai[api_key]" placeholder="..."></textarea>
+            </div>
+            <div class="field box">
+                <label for="GeminiPro-api_key" class="label" title="">GeminiPro: api_key</label>
+                <textarea id="GeminiPro-api_key" name="GeminiPro[api_key]" placeholder="..."></textarea>
+            </div>
+            <div class="field box">
+                <label for="HuggingFace-api_key" class="label" title="">HuggingFace: api_key</label>
+                <textarea id="HuggingFace-api_key" name="HuggingFace[api_key]" placeholder="..."></textarea>
+            </div>
+        </div>
         <div class="conversation">
             <textarea id="systemPrompt" class="box" placeholder="System prompt"></textarea>    
             <div id="messages" class="box"></div>
             <div class="toolbar">
                 <div id="input-count" class="">
                     &nbsp;
                 </div>
```

#### html2text {}

```diff
@@ -1,10 +1,11 @@
 New Conversation
 Clear Conversations Export Conversations
 github ~ _@_g_p_t_4_f_r_e_e
+OpenaiChat: Auto continue
  
 Stop Generating
 Regenerate
 [File][File][File]
 [One of: Set Jailbreak/math 1.0/dude 1.0/dan 1.0/dan 2.0/dev 2.0/evil 1.0]
 [One of: Provider: Auto/Bing/OpenaiChat/Gemini/Liaobots/You/----]
 ??Web Access
```

### Comparing `g4f-0.2.8.0/g4f/gui/client/static/css/style.css` & `g4f-0.2.8.1/g4f/gui/client/static/css/style.css`

 * *Files 2% similar despite different names*

```diff
@@ -508,21 +508,23 @@
 
 @media (pointer:none), (pointer:coarse) {
     label[for="camera"] {
         display: block;
     }
 }
 
-.buttons input[type="checkbox"] {
+.buttons input[type="checkbox"],
+.settings input[type="checkbox"] {
     height: 0;
     width: 0;
     display: none;
 }
 
-.buttons label {
+.buttons label,
+.settings label.toogle {
     cursor: pointer;
     text-indent: -9999px;
     width: 50px;
     height: 30px;
     backdrop-filter: blur(20px);
     -webkit-backdrop-filter: blur(20px);
     background-color: var(--blur-bg);
@@ -531,28 +533,30 @@
     display: block;
     border-radius: 100px;
     position: relative;
     overflow: hidden;
     transition: 0.33s;
 }
 
-.buttons label:after {
+.buttons label:after,
+.settings label.toogle:after {
     content: "";
     position: absolute;
     top: 50%;
     transform: translateY(-50%);
     left: 5px;
     width: 20px;
     height: 20px;
     background: var(--colour-3);
     border-radius: 90px;
     transition: 0.33s;
 }
 
-.buttons input:checked+label {
+.buttons input:checked+label,
+.settings input:checked+label {
     background: var(--accent);
 }
 
 .buttons input:checked+label:after {
     left: calc(100% - 5px - 20px);
 }
 
@@ -872,15 +876,14 @@
     height: 1px;
     overflow: hidden;
     position: absolute;
     white-space: nowrap;
     width: 1px;
 }
 
-
 .color-picker>fieldset {
     border: 0;
     display: flex;
     width: fit-content;
     background: var(--colour-1);
     margin-inline: auto;
     border-radius: 8px;
@@ -1006,31 +1009,72 @@
     right: 8px;
 }
 
 #send-button:hover {
     border: 1px solid #e4d4ffc9;
 }
 
-#systemPrompt {
+#systemPrompt, .settings textarea {
     font-size: 15px;
     width: 100%;
     color: var(--colour-3);
-    min-height: 59px;
-    height: 59px;
+    min-height: 50px;
+    height: 50px;
     outline: none;
     padding: var(--inner-gap) var(--section-gap);
     resize: vertical;
 }
 
+.settings {
+    width: 100%;
+    display: none;
+}
+
+.settings .field {
+    margin: var(--inner-gap) 0;
+}
+
+.settings textarea {
+    background-color: transparent;
+    border: none;
+    padding: var(--inner-gap) 0;
+}
+
+.settings .label {
+    font-size: 15px;
+    padding: var(--inner-gap) 0;
+    width: fit-content;
+    min-width: 190px;
+    margin-left: var(--section-gap);
+    white-space:nowrap;
+}
+
 ::-webkit-scrollbar {
     width: 10px;
 }
 ::-webkit-scrollbar-track {
     background: var(--colour-3);
 }
 ::-webkit-scrollbar-thumb {
     background: var(--blur-bg);
     border-radius: 5px;
 }
 ::-webkit-scrollbar-thumb:hover {
     background: var(--accent)
+}
+
+.hljs {
+    color: #e9e9f4;
+    background: #28293629;
+    border-radius: var(--border-radius-1);
+    border: 1px solid var(--blur-border);
+    font-size: 15px;
+}
+
+#message-input {
+    height: 82px;
+    margin-left: 20px;
+}
+
+#message-input::-webkit-scrollbar {
+    width: 5px;
 }
```

### Comparing `g4f-0.2.8.0/g4f/gui/client/static/img/android-chrome-192x192.png` & `g4f-0.2.8.1/g4f/gui/client/static/img/android-chrome-192x192.png`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.0/g4f/gui/client/static/img/android-chrome-512x512.png` & `g4f-0.2.8.1/g4f/gui/client/static/img/android-chrome-512x512.png`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.0/g4f/gui/client/static/img/apple-touch-icon.png` & `g4f-0.2.8.1/g4f/gui/client/static/img/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.0/g4f/gui/client/static/img/favicon-32x32.png` & `g4f-0.2.8.1/g4f/gui/client/static/img/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.0/g4f/gui/client/static/img/gpt.png` & `g4f-0.2.8.1/g4f/gui/client/static/img/gpt.png`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.0/g4f/gui/client/static/img/user.png` & `g4f-0.2.8.1/g4f/gui/client/static/img/user.png`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.0/g4f/gui/client/static/js/chat.v1.js` & `g4f-0.2.8.1/g4f/gui/client/static/js/chat.v1.js`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.0/g4f/gui/client/static/js/highlight.min.js` & `g4f-0.2.8.1/g4f/gui/client/static/js/highlight.min.js`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.0/g4f/gui/client/static/js/highlightjs-copy.min.js` & `g4f-0.2.8.1/g4f/gui/client/static/js/highlightjs-copy.min.js`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.0/g4f/gui/client/static/js/icons.js` & `g4f-0.2.8.1/g4f/gui/client/static/js/icons.js`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.0/g4f/gui/server/android_gallery.py` & `g4f-0.2.8.1/g4f/gui/server/android_gallery.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.0/g4f/gui/server/backend.py` & `g4f-0.2.8.1/g4f/gui/server/backend.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.0/g4f/gui/server/config.py` & `g4f-0.2.8.1/g4f/gui/server/config.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.0/g4f/gui/server/internet.py` & `g4f-0.2.8.1/g4f/gui/server/internet.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.0/g4f/gui/server/website.py` & `g4f-0.2.8.1/g4f/gui/server/website.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.0/g4f/image.py` & `g4f-0.2.8.1/g4f/image.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.0/g4f/local/__init__.py` & `g4f-0.2.8.1/g4f/local/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,36 +1,37 @@
-from ..typing import Union, Iterator, Messages
-from ..stubs  import ChatCompletion, ChatCompletionChunk
-from ._engine import LocalProvider
-from ._models import models
-from ..client import iter_response, filter_none, IterResponse
+from __future__ import annotations
+
+from ..typing import Union, Messages
+from ..locals.provider import LocalProvider
+from ..locals.models import get_models
+from ..client.client import iter_response, filter_none
+from ..client.types import IterResponse
 
 class LocalClient():
     def __init__(self, **kwargs) -> None:
         self.chat: Chat = Chat(self)
-    
+
     @staticmethod
     def list_models():
-        return list(models.keys())
-        
+        return list(get_models())
+
 class Completions():
     def __init__(self, client: LocalClient):
         self.client: LocalClient = client
 
     def create(
         self,
         messages: Messages,
         model: str,
         stream: bool = False,
         response_format: dict = None,
         max_tokens: int = None,
         stop: Union[list[str], str] = None,
         **kwargs
-    ) -> Union[ChatCompletion, Iterator[ChatCompletionChunk]]:
-
+    ) -> IterResponse:
         stop = [stop] if isinstance(stop, str) else stop
         response = LocalProvider.create_completion(
             model, messages, stream,            
             **filter_none(
                 max_tokens=max_tokens,
                 stop=stop,
             ),
```

### Comparing `g4f-0.2.8.0/g4f/models.py` & `g4f-0.2.8.1/g4f/models.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.0/g4f/providers/base_provider.py` & `g4f-0.2.8.1/g4f/providers/base_provider.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,40 +2,47 @@
 
 import sys
 import asyncio
 from asyncio import AbstractEventLoop
 from concurrent.futures import ThreadPoolExecutor
 from abc import abstractmethod
 from inspect import signature, Parameter
-from ..typing import CreateResult, AsyncResult, Messages, Union
-from .types import BaseProvider
+from typing import Callable, Union
+from ..typing import CreateResult, AsyncResult, Messages
+from .types import BaseProvider, FinishReason
 from ..errors import NestAsyncioError, ModelNotSupportedError
 from .. import debug
 
 if sys.version_info < (3, 10):
     NoneType = type(None)
 else:
     from types import NoneType
 
 # Set Windows event loop policy for better compatibility with asyncio and curl_cffi
 if sys.platform == 'win32':
     if isinstance(asyncio.get_event_loop_policy(), asyncio.WindowsProactorEventLoopPolicy):
         asyncio.set_event_loop_policy(asyncio.WindowsSelectorEventLoopPolicy())
 
-def get_running_loop() -> Union[AbstractEventLoop, None]:
+def get_running_loop(check_nested: bool) -> Union[AbstractEventLoop, None]:
     try:
         loop = asyncio.get_running_loop()
-        if not hasattr(loop.__class__, "_nest_patched"):
-            raise NestAsyncioError(
-                'Use "create_async" instead of "create" function in a running event loop. Or use "nest_asyncio" package.'
-            )
+        if check_nested and not hasattr(loop.__class__, "_nest_patched"):
+            try:
+                import nest_asyncio
+                nest_asyncio.apply(loop)
+            except ImportError:
+                raise NestAsyncioError('Install "nest_asyncio" package')
         return loop
     except RuntimeError:
         pass
 
+# Fix for RuntimeError: async generator ignored GeneratorExit
+async def await_callback(callback: Callable):
+    return await callback()
+
 class AbstractProvider(BaseProvider):
     """
     Abstract class for providing asynchronous functionality to derived classes.
     """
 
     @classmethod
     async def create_async(
@@ -128,15 +135,15 @@
             stream (bool): Indicates whether to stream the results. Defaults to False.
             loop (AbstractEventLoop, optional): The event loop to use. Defaults to None.
             **kwargs: Additional keyword arguments.
 
         Returns:
             CreateResult: The result of the completion creation.
         """
-        get_running_loop()
+        get_running_loop(check_nested=True)
         yield asyncio.run(cls.create_async(model, messages, **kwargs))
 
     @staticmethod
     @abstractmethod
     async def create_async(
         model: str,
         messages: Messages,
@@ -154,15 +161,14 @@
             NotImplementedError: If this method is not overridden in derived classes.
 
         Returns:
             str: The created result as a string.
         """
         raise NotImplementedError()
 
-
 class AsyncGeneratorProvider(AsyncProvider):
     """
     Provides asynchronous generator functionality for streaming results.
     """
     supports_stream = True
 
     @classmethod
@@ -183,34 +189,29 @@
             stream (bool): Indicates whether to stream the results. Defaults to True.
             loop (AbstractEventLoop, optional): The event loop to use. Defaults to None.
             **kwargs: Additional keyword arguments.
 
         Returns:
             CreateResult: The result of the streaming completion creation.
         """
-        loop = get_running_loop()
+        loop = get_running_loop(check_nested=True)
         new_loop = False
-        if not loop:
+        if loop is None:
             loop = asyncio.new_event_loop()
             asyncio.set_event_loop(loop)
             new_loop = True
 
         generator = cls.create_async_generator(model, messages, stream=stream, **kwargs)
         gen = generator.__aiter__()
 
-        # Fix for RuntimeError: async generator ignored GeneratorExit
-        async def await_callback(callback):
-            return await callback()
-
         try:
             while True:
                 yield loop.run_until_complete(await_callback(gen.__anext__))
         except StopAsyncIteration:
             ...
-        # Fix for: ResourceWarning: unclosed event loop
         finally:
             if new_loop:
                 loop.close()
                 asyncio.set_event_loop(None)
 
     @classmethod
     async def create_async(
@@ -229,15 +230,15 @@
             **kwargs: Additional keyword arguments.
 
         Returns:
             str: The created result as a string.
         """
         return "".join([
             chunk async for chunk in cls.create_async_generator(model, messages, stream=False, **kwargs) 
-            if not isinstance(chunk, Exception)
+            if not isinstance(chunk, (Exception, FinishReason))
         ])
 
     @staticmethod
     @abstractmethod
     async def create_async_generator(
         model: str,
         messages: Messages,
```

### Comparing `g4f-0.2.8.0/g4f/providers/create_images.py` & `g4f-0.2.8.1/g4f/providers/create_images.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.0/g4f/providers/helper.py` & `g4f-0.2.8.1/g4f/providers/helper.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.0/g4f/providers/retry_provider.py` & `g4f-0.2.8.1/g4f/providers/retry_provider.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.0/g4f/providers/types.py` & `g4f-0.2.8.1/g4f/providers/types.py`

 * *Files 3% similar despite different names*

```diff
@@ -92,9 +92,14 @@
         shuffle (bool): Whether to shuffle the providers list.
         exceptions (Dict[str, Exception]): Dictionary of exceptions encountered.
         last_provider (Type[BaseProvider]): The last provider used.
     """
 
     __name__: str = "RetryProvider"
     supports_stream: bool = True
+    last_provider: Type[BaseProvider] = None
 
-ProviderType = Union[Type[BaseProvider], BaseRetryProvider]
+ProviderType = Union[Type[BaseProvider], BaseRetryProvider]
+
+class FinishReason():
+    def __init__(self, reason: str):
+        self.reason = reason
```

### Comparing `g4f-0.2.8.0/g4f/requests/__init__.py` & `g4f-0.2.8.1/g4f/requests/__init__.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.0/g4f/requests/aiohttp.py` & `g4f-0.2.8.1/g4f/requests/aiohttp.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,29 +11,37 @@
         async for line in self.content:
             yield line.rstrip(b"\r\n")
 
     async def iter_content(self) -> AsyncIterator[bytes]:
         async for chunk in self.content.iter_any():
             yield chunk
 
-    async def json(self) -> Any:
-        return await super().json(content_type=None)
+    async def json(self, content_type: str = None) -> Any:
+        return await super().json(content_type=content_type)
 
 class StreamSession(ClientSession):
-    def __init__(self, headers: dict = {}, timeout: int = None, proxies: dict = {}, impersonate = None, **kwargs):
+    def __init__(
+        self,
+        headers: dict = {},
+        timeout: int = None,
+        connector: BaseConnector = None,
+        proxies: dict = {},
+        impersonate = None,
+        **kwargs
+    ):
         if impersonate:
             headers = {
                 **DEFAULT_HEADERS,
                 **headers
             }
         super().__init__(
             **kwargs,
             timeout=ClientTimeout(timeout) if timeout else None,
             response_class=StreamResponse,
-            connector=get_connector(kwargs.get("connector"), proxies.get("https")),
+            connector=get_connector(connector, proxies.get("all", proxies.get("https"))),
             headers=headers
         )
 
 def get_connector(connector: BaseConnector = None, proxy: str = None, rdns: bool = False) -> Optional[BaseConnector]:
     if proxy and not connector:
         try:
             from aiohttp_socks import ProxyConnector
```

### Comparing `g4f-0.2.8.0/g4f/requests/curl_cffi.py` & `g4f-0.2.8.1/g4f/requests/curl_cffi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.0/g4f/requests/defaults.py` & `g4f-0.2.8.1/g4f/requests/defaults.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.0/g4f/requests/raise_for_status.py` & `g4f-0.2.8.1/g4f/requests/raise_for_status.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.0/g4f/stubs.py` & `g4f-0.2.8.1/g4f/stubs.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.0/g4f/typing.py` & `g4f-0.2.8.1/g4f/typing.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.0/g4f/version.py` & `g4f-0.2.8.1/g4f/version.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.0/g4f/webdriver.py` & `g4f-0.2.8.1/g4f/webdriver.py`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.0/g4f.egg-info/PKG-INFO` & `g4f-0.2.8.1/g4f.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: g4f
-Version: 0.2.8.0
+Version: 0.2.8.1
 Summary: The official gpt4free repository | various collection of powerful language models
 Home-page: https://github.com/xtekky/gpt4free
 Author: Tekky
 Author-email: <support@g4f.ai>
 Project-URL: Source Code, https://github.com/xtekky/gpt4free
 Project-URL: Bug Tracker, https://github.com/xtekky/gpt4free/issues
 Keywords: python,chatbot,reverse-engineering,openai,chatbots,gpt,language-model,gpt-3,gpt3,openai-api,gpt-4,gpt4,chatgpt,chatgpt-api,openai-chatgpt,chatgpt-free,chatgpt-4,chatgpt4,chatgpt4-api,free,free-gpt,gpt4free,g4f
@@ -96,43 +96,43 @@
 ```
 ```sh
 docker pull hlohaus789/g4f
 ```
 
 ## 🆕 What's New
 
-- Check out a more in depth local inference @ https://github.com/gpt4free/gpt4local
-- Join our Telegram Channel: [t.me/g4f_channel](https://telegram.me/g4f_channel)
-- Join our Discord Group: [discord.gg/XfybzPXPH5](https://discord.gg/XfybzPXPH5)
-- `g4f` now supports 100% local inference: [local-docs](https://g4f.mintlify.app/docs/core/usage/local)
+- Installation Guide for Windows (.exe): 💻 [#installation-guide-for-windows](#installation-guide-for-windows-exe)
+- Join our Telegram Channel: 📨 [telegram.me/g4f_channel](https://telegram.me/g4f_channel)
+- Join our Discord Group: 💬 [discord.gg/XfybzPXPH5](https://discord.gg/XfybzPXPH5)
+- `g4f` now supports 100% local inference: 🧠 [local-docs](https://g4f.mintlify.app/docs/core/usage/local)
 
 ## 🔻 Site Takedown
-Is your site on this repository and you want to take it down? Send an email to takedown@g4f.ai with proof it is yours and it will be removed as fast as possible. To prevent reproduction please secure your API ;)
+Is your site on this repository and you want to take it down? Send an email to takedown@g4f.ai with proof it is yours and it will be removed as fast as possible. To prevent reproduction please secure your API. 😉
 
 ## 🚀  Feedback and Todo
 You can always leave some feedback here: https://forms.gle/FeWV9RLEedfdkmFN6
 
 As per the survey, here is a list of improvements to come
 - [x] Update the repository to include the new openai library syntax (ex: `Openai()` class) | completed, use `g4f.client.Client`
 - [ ] Golang implementation
 - [ ] 🚧 Improve Documentation (in /docs & Guides, Howtos, & Do video tutorials)
 - [x] Improve the provider status list & updates
 - [ ] Tutorials on how to reverse sites to write your own wrapper (PoC only ofc)
 - [x] Improve the Bing wrapper. (Wait and Retry or reuse conversation)
-- [ ] Write a standard provider performance test to improve the stability
+- [ ] 🚧 Write a standard provider performance test to improve the stability
 - [ ] Potential support and development of local models
 - [ ] 🚧 Improve compatibility and error handling
 
 ## 📚 Table of Contents
 
 - [🆕 What's New](#-whats-new)
 - [📚 Table of Contents](#-table-of-contents)
 - [🛠️ Getting Started](#-getting-started)
-    + [Docker container](#docker-container)
-      - [Quick start](#quick-start)
+    + [Docker Container Guide](#docker-container-guide)
+    + [Installation Guide for Windows (.exe)](#installation-guide-for-windows-exe)
     + [Use python](#use-python)
       - [Prerequisites](#prerequisites)
       - [Install using PyPI package:](#install-using-pypi-package)
       - [Install from source:](#install-from-source)
       - [Install using Docker:](#install-using-docker)
 - [💡 Usage](#-usage)
   * [Text Generation](#text-generation)
@@ -152,28 +152,49 @@
 - [🙌 Contributors](#-contributors)
 - [©️ Copyright](#-copyright)
 - [⭐ Star History](#-star-history)
 - [📄 License](#-license)
 
 ## 🛠️ Getting Started
 
-#### Docker container
+#### Docker Container Guide
 
-##### Quick start:
+##### Getting Started Quickly:
 
-1. [Download and install Docker](https://docs.docker.com/get-docker/)
-2. Pull latest image and run the container:
+1. **Install Docker:** Begin by [downloading and installing Docker](https://docs.docker.com/get-docker/).
+
+2. **Set Up the Container:**
+   Use the following commands to pull the latest image and start the container:
 
 ```sh
 docker pull hlohaus789/g4f
 docker run -p 8080:8080 -p 1337:1337 -p 7900:7900 --shm-size="2g" -v ${PWD}/hardir:/app/hardir hlohaus789/g4f:latest
 ```
-3. Open the included client on: [http://localhost:8080/chat/](http://localhost:8080/chat/)
-or set the API base in your client to: [http://localhost:1337/v1](http://localhost:1337/v1)
-4. (Optional) If you need to log in to a provider, you can view the desktop from the container here: http://localhost:7900/?autoconnect=1&resize=scale&password=secret.
+
+3. **Access the Client:** 
+   - To use the included client, navigate to: [http://localhost:8080/chat/](http://localhost:8080/chat/)
+   - Or set the API base for your client to: [http://localhost:1337/v1](http://localhost:1337/v1)
+
+4. **(Optional) Provider Login:**
+   If required, you can access the container's desktop here: http://localhost:7900/?autoconnect=1&resize=scale&password=secret for provider login purposes.
+
+#### Installation Guide for Windows (.exe)
+To ensure the seamless operation of our application, please follow the instructions below. These steps are designed to guide you through the installation process on Windows operating systems.
+##### Prerequisites
+1. **WebView2 Runtime**: Our application requires the *WebView2 Runtime* to be installed on your system. If you do not have it installed, please download and install it from the [Microsoft Developer Website](https://developer.microsoft.com/en-us/microsoft-edge/webview2/). If you already have *WebView2 Runtime* installed but are encountering issues, navigate to *Installed Windows Apps*, select *WebView2*, and opt for the repair option.
+##### Installation Steps
+2. **Download the Application**: Visit our [latest releases page](https://github.com/xtekky/gpt4free/releases/latest) and download the most recent version of the application, named `g4f.webview.*.exe`.
+3. **File Placement**: Once downloaded, transfer the `.exe` file from your downloads folder to a directory of your choice on your system, and then execute it to run the app.
+##### Post-Installation Adjustment
+4. **Firewall Configuration (Hotfix)**: Upon installation, it may be necessary to adjust your Windows Firewall settings to allow the application to operate correctly. To do this, access your Windows Firewall settings and allow the application.
+
+By following these steps, you should be able to successfully install and run the application on your Windows system. If you encounter any issues during the installation process, please refer to our Issue Tracker or try to get contact over Discord for assistance.
+
+Run the **Webview UI** on other Platfroms:
+- [/docs/guides/webview](/docs/webview.md)
 
 ##### Use your smartphone:
 
 Run the Web UI on Your Smartphone:
 - [/docs/guides/phone](/docs/guides/phone.md)
 
 #### Use python
@@ -242,59 +263,34 @@
 [![Image with cat](/docs/cat.jpeg)](/docs/client.md)
 
 **Full Documentation for Python API**
 
 - New Client API like the OpenAI Python library: [/docs/client](/docs/client.md)
 - Legacy API with python modules: [/docs/legacy](/docs/legacy.md)
 
-### Webview GUI
-
-Open the GUI in a window of your OS. Runs on a local/static/ssl server and use a JavaScript API.
-Supports login into the OpenAI Chat, Image Upload and streamed Text Generation.
-
-Supports all platforms, but only Linux tested.
-
-1. Install all requirements with:
-
-```bash
-pip install g4f[webview]
-```
-
-2. Follow the OS specific steps here:
- [pywebview installation](https://pywebview.flowrl.com/guide/installation.html#dependencies)
-
-3. Run the app with:
-
-```python
-from g4f.gui.webview import run_webview
-run_webview(debug=True)
-```
-or execute the following command:
-```bash
-python -m g4f.gui.webview -debug
-```
-
-#### Webserver
+#### Web UI
 
 To start the web interface, type the following codes in python:
 
 ```python
 from g4f.gui import run_gui
 run_gui()
 ```
 or execute the following command:
 ```bash
 python -m g4f.cli gui -port 8080 -debug
 ```
 
-### Interference API
+#### Interference API
 
 You can use the Interference API to serve other OpenAI integrations with G4F.
 
-See: [/docs/interference](/docs/interference.md)
+See docs: [/docs/interference](/docs/interference.md)
+
+Access with: http://localhost:1337/v1
 
 ### Configuration
 
 #### Cookies
 
 You need cookies for BingCreateImages and the Gemini Provider.
 From Bing you need the "_U" cookie and from Gemini you need the "__Secure-1PSID" cookie.
@@ -319,15 +315,15 @@
 
 To utilize the OpenaiChat provider, a .har file is required from https://chat.openai.com/. Follow the steps below to create a valid .har file:
 
 1. Navigate to https://chat.openai.com/ using your preferred web browser and log in with your credentials.
 2. Access the Developer Tools in your browser. This can typically be done by right-clicking the page and selecting "Inspect," or by pressing F12 or Ctrl+Shift+I (Cmd+Option+I on a Mac).
 3. With the Developer Tools open, switch to the "Network" tab.
 4. Reload the website to capture the loading process within the Network tab.
-5. Initiate an action in the chat which can be capture in the .har file.
+5. Initiate an action in the chat which can be captured in the .har file.
 6. Right-click any of the network activities listed and select "Save all as HAR with content" to export the .har file.
 
 ##### Storing the .HAR File
 
 - Place the exported .har file in the `./hardir` directory if you are using Docker. Alternatively, you can store it in any preferred location within your current working directory.
 
 Note: Ensure that your .har file is stored securely, as it may contain sensitive information.
@@ -852,17 +848,58 @@
 
 ###### Guide: How can AI help me with writing code?
 
  - Read: [/docs/guides/help_me](/docs/guides/help_me.md)
 
 ## 🙌 Contributors
 
-A list of all contributors is available [here](https://github.com/xtekky/gpt4free/graphs/contributors)   
-The [`Vercel.py`](https://github.com/xtekky/gpt4free/blob/main/g4f/Provider/Vercel.py) file contains code from [vercel-llm-api](https://github.com/ading2210/vercel-llm-api) by [@ading2210](https://github.com/ading2210), which is licensed under the [GNU GPL v3](https://www.gnu.org/licenses/gpl-3.0.txt)   
-Top 1 Contributor: [@hlohaus](https://github.com/hlohaus)
+A list of all contributors is available [here](https://github.com/xtekky/gpt4free/graphs/contributors)
+
+<a href="https://github.com/xtekky" target="_blank"><img src="https://avatars.githubusercontent.com/u/98614666?v=4&s=45" width="45" title="xtekky"></a>
+<a href="https://github.com/hlohaus" target="_blank"><img src="https://avatars.githubusercontent.com/u/983577?v=4&s=45" width="45" title="hlohaus"></a>
+<a href="https://github.com/bagusindrayana" target="_blank"><img src="https://avatars.githubusercontent.com/u/36830534?v=4&s=45" width="45" title="bagusindrayana"></a>
+<a href="https://github.com/sudouser777" target="_blank"><img src="https://avatars.githubusercontent.com/u/22415463?v=4&s=45" width="45" title="sudouser777"></a>
+<a href="https://github.com/thatlukinhasguy1" target="_blank"><img src="https://avatars.githubusercontent.com/u/139662282?v=4&s=45" width="45" title="thatlukinhasguy1"></a>
+<a href="https://github.com/Commenter123321" target="_blank"><img src="https://avatars.githubusercontent.com/u/36051603?v=4&s=45" width="45" title="Commenter123321"></a>
+<a href="https://github.com/DanielShemesh" target="_blank"><img src="https://avatars.githubusercontent.com/u/20585236?v=4&s=45" width="45" title="DanielShemesh"></a>
+<a href="https://github.com/Luneye" target="_blank"><img src="https://avatars.githubusercontent.com/u/73485421?v=4&s=45" width="45" title="Luneye"></a>
+<a href="https://github.com/enganese" target="_blank"><img src="https://avatars.githubusercontent.com/u/69082498?v=4&s=45" width="45" title="enganese"></a>
+<a href="https://github.com/ezerinz" target="_blank"><img src="https://avatars.githubusercontent.com/u/100193740?v=4&s=45" width="45" title="ezerinz"></a>
+<a href="https://github.com/Lin-jun-xiang" target="_blank"><img src="https://avatars.githubusercontent.com/u/63782903?v=4&s=45" width="45" title="Lin-jun-xiang"></a>
+<a href="https://github.com/nullstreak" target="_blank"><img src="https://avatars.githubusercontent.com/u/139914347?v=4&s=45" width="45" title="nullstreak"></a>
+<a href="https://github.com/valerii-chirkov" target="_blank"><img src="https://avatars.githubusercontent.com/u/81074936?v=4&s=45" width="45" title="valerii-chirkov"></a>
+<a href="https://github.com/MIDORIBIN" target="_blank"><img src="https://avatars.githubusercontent.com/u/25425217?v=4&s=45" width="45" title="MIDORIBIN"></a>
+<a href="https://github.com/repollo" target="_blank"><img src="https://avatars.githubusercontent.com/u/2671466?v=4&s=45" width="45" title="repollo"></a>
+<a href="https://github.com/hpsj" target="_blank"><img src="https://avatars.githubusercontent.com/u/54535414?v=4&s=45" width="45" title="hpsj"></a>
+<a href="https://github.com/taiyi747" target="_blank"><img src="https://avatars.githubusercontent.com/u/63543716?v=4&s=45" width="45" title="taiyi747"></a>
+<a href="https://github.com/ostix360" target="_blank"><img src="https://avatars.githubusercontent.com/u/55257054?v=4&s=45" width="45" title="ostix360"></a>
+<a href="https://github.com/WdR-Tech" target="_blank"><img src="https://avatars.githubusercontent.com/u/143020293?v=4&s=45" width="45" title="WdR-Tech"></a>
+<a href="https://github.com/HexyeDEV" target="_blank"><img src="https://avatars.githubusercontent.com/u/65314629?v=4&s=45" width="45" title="HexyeDEV"></a>
+<a href="https://github.com/9fo" target="_blank"><img src="https://avatars.githubusercontent.com/u/71867245?v=4&s=45" width="45" title="9fo"></a>
+<a href="https://github.com/eltociear" target="_blank"><img src="https://avatars.githubusercontent.com/u/22633385?v=4&s=45" width="45" title="eltociear"></a>
+<a href="https://github.com/ramonvc" target="_blank"><img src="https://avatars.githubusercontent.com/u/13617054?v=4&s=45" width="45" title="ramonvc"></a>
+<a href="https://github.com/naa7" target="_blank"><img src="https://avatars.githubusercontent.com/u/44613678?v=4&s=45" width="45" title="naa7"></a>
+<a href="https://github.com/zeng-rr" target="_blank"><img src="https://avatars.githubusercontent.com/u/47846202?v=4&s=45" width="45" title="zeng-rr"></a>
+<a href="https://github.com/editor-syntax" target="_blank"><img src="https://avatars.githubusercontent.com/u/109844019?v=4&s=45" width="45" title="editor-syntax"></a>
+<a href="https://github.com/devAdityaa" target="_blank"><img src="https://avatars.githubusercontent.com/u/77636021?v=4&s=45" width="45" title="devAdityaa"></a>
+<a href="https://github.com/kggn" target="_blank"><img src="https://avatars.githubusercontent.com/u/95663228?v=4&s=45" width="45" title="kggn"></a>
+<a href="https://github.com/xiangsx" target="_blank"><img src="https://avatars.githubusercontent.com/u/29322721?v=4&s=45" width="45" title="xiangsx"></a>
+<a href="https://github.com/ggindinson" target="_blank"><img src="https://avatars.githubusercontent.com/u/97807772?v=4&s=45" width="45" title="ggindinson"></a>
+<span></span>
+<img src="https://avatars.githubusercontent.com/u/71154407?s=45&v=4" width="45" title="ading2210">
+<img src="https://avatars.githubusercontent.com/u/12299238?s=45&v=4" width="45" title="xqdoo00o">
+<img src="https://avatars.githubusercontent.com/u/97126670?s=45&v=4" width="45" title="nathanrchn">
+<img src="https://avatars.githubusercontent.com/u/81407603?v=4&s=45" width="45" title="dsdanielpark">
+
+- The [`Vercel.py`](g4f/Provider/Vercel.py) file contains code from [vercel-llm-api](https://github.com/ading2210/vercel-llm-api) by [@ading2210](https://github.com/ading2210)
+- The [`har_file.py`](g4f/Provider/openai/har_file.py) has input from [xqdoo00o/ChatGPT-to-API](https://github.com/xqdoo00o/ChatGPT-to-API)
+- The [`PerplexityLabs.py`](g4f/Provider/openai/har_file.py) has input from [nathanrchn/perplexityai](https://github.com/nathanrchn/perplexityai)
+- The [`Gemini.py`](g4f/Provider/needs_auth/Gemini.py) has input from [dsdanielpark/Gemini-API](https://github.com/dsdanielpark/Gemini-API)
+
+*Having input implies that the AI's code generation utilized it as one of many sources.*
 
 ## ©️ Copyright
 
 This program is licensed under the [GNU GPL v3](https://www.gnu.org/licenses/gpl-3.0.txt)
 
 ```
 xtekky/gpt4free: Copyright (C) 2023 xtekky
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: g4f Version: 0.2.8.0 Summary: The official gpt4free
+Metadata-Version: 2.1 Name: g4f Version: 0.2.8.1 Summary: The official gpt4free
 repository | various collection of powerful language models Home-page: https://
 github.com/xtekky/gpt4free Author: Tekky Author-email:
 g4f.ai> Project-URL: Source Code, https://github.com/xtekky/gpt4free Project-
 URL: Bug Tracker, https://github.com/xtekky/gpt4free/issues Keywords:
 python,chatbot,reverse-engineering,openai,chatbots,gpt,language-model,gpt-
 3,gpt3,openai-api,gpt-4,gpt4,chatgpt,chatgpt-api,openai-chatgpt,chatgpt-
 free,chatgpt-4,chatgpt4,chatgpt4-api,free,free-gpt,gpt4free,g4f Classifier:
@@ -54,139 +54,159 @@
 with features like timeouts, load balance and flow control. > [!Note] LLaasstteett
 vveerrssiioonn:: [![PyPI version](https://img.shields.io/pypi/v/g4f?color=blue)](https:
 //pypi.org/project/g4f) [![Docker version](https://img.shields.io/docker/v/
 hlohaus789/g4f?label=docker&color=blue)](https://hub.docker.com/r/hlohaus789/
 g4f) > SSttaattss:: [![Downloads](https://static.pepy.tech/badge/g4f)](https://
 pepy.tech/project/g4f) [![Downloads](https://static.pepy.tech/badge/g4f/month)]
 (https://pepy.tech/project/g4f) ```sh pip install -U g4f ``` ```sh docker pull
-hlohaus789/g4f ``` ## ð What's New - Check out a more in depth local
-inference @ https://github.com/gpt4free/gpt4local - Join our Telegram Channel:
-[t.me/g4f_channel](https://telegram.me/g4f_channel) - Join our Discord Group:
-[discord.gg/XfybzPXPH5](https://discord.gg/XfybzPXPH5) - `g4f` now supports
-100% local inference: [local-docs](https://g4f.mintlify.app/docs/core/usage/
-local) ## ð» Site Takedown Is your site on this repository and you want to
-take it down? Send an email to takedown@g4f.ai with proof it is yours and it
-will be removed as fast as possible. To prevent reproduction please secure your
-API ;) ## ð Feedback and Todo You can always leave some feedback here:
-https://forms.gle/FeWV9RLEedfdkmFN6 As per the survey, here is a list of
-improvements to come - [x] Update the repository to include the new openai
-library syntax (ex: `Openai()` class) | completed, use `g4f.client.Client` -
-[ ] Golang implementation - [ ] ð§ Improve Documentation (in /docs & Guides,
-Howtos, & Do video tutorials) - [x] Improve the provider status list & updates
-- [ ] Tutorials on how to reverse sites to write your own wrapper (PoC only
-ofc) - [x] Improve the Bing wrapper. (Wait and Retry or reuse conversation) -
-[ ] Write a standard provider performance test to improve the stability - [ ]
-Potential support and development of local models - [ ] ð§ Improve
-compatibility and error handling ## ð Table of Contents - [ð What's New]
-(#-whats-new) - [ð Table of Contents](#-table-of-contents) - [ð ï¸
-Getting Started](#-getting-started) + [Docker container](#docker-container) -
-[Quick start](#quick-start) + [Use python](#use-python) - [Prerequisites]
-(#prerequisites) - [Install using PyPI package:](#install-using-pypi-package) -
-[Install from source:](#install-from-source) - [Install using Docker:]
-(#install-using-docker) - [ð¡ Usage](#-usage) * [Text Generation](#text-
-generation) * [Image Generation](#image-generation) * [Web UI](#web-ui) *
-[Interference API](#interference-api) * [Configuration](#configuration) - [ð
-Providers and Models](#-providers-and-models) * [GPT-4](#gpt-4) * [GPT-3.5]
-(#gpt-35) * [Other](#other) * [Models](#models) - [ð Powered by gpt4free](#-
-powered-by-gpt4free) - [ð¤ Contribute](#-contribute) + [How do i create a new
-Provider?](#guide-how-do-i-create-a-new-provider) + [How can AI help me with
-writing code?](#guide-how-can-ai-help-me-with-writing-code) - [ð
-Contributors](#-contributors) - [Â©ï¸ Copyright](#-copyright) - [â­ Star
-History](#-star-history) - [ð License](#-license) ## ð ï¸ Getting Started
-#### Docker container ##### Quick start: 1. [Download and install Docker]
-(https://docs.docker.com/get-docker/) 2. Pull latest image and run the
+hlohaus789/g4f ``` ## ð What's New - Installation Guide for Windows (.exe):
+ð» [#installation-guide-for-windows](#installation-guide-for-windows-exe) -
+Join our Telegram Channel: ð¨ [telegram.me/g4f_channel](https://telegram.me/
+g4f_channel) - Join our Discord Group: ð¬ [discord.gg/XfybzPXPH5](https://
+discord.gg/XfybzPXPH5) - `g4f` now supports 100% local inference: ð§  [local-
+docs](https://g4f.mintlify.app/docs/core/usage/local) ## ð» Site Takedown Is
+your site on this repository and you want to take it down? Send an email to
+takedown@g4f.ai with proof it is yours and it will be removed as fast as
+possible. To prevent reproduction please secure your API. ð ## ð Feedback
+and Todo You can always leave some feedback here: https://forms.gle/
+FeWV9RLEedfdkmFN6 As per the survey, here is a list of improvements to come -
+[x] Update the repository to include the new openai library syntax (ex: `Openai
+()` class) | completed, use `g4f.client.Client` - [ ] Golang implementation -
+[ ] ð§ Improve Documentation (in /docs & Guides, Howtos, & Do video
+tutorials) - [x] Improve the provider status list & updates - [ ] Tutorials on
+how to reverse sites to write your own wrapper (PoC only ofc) - [x] Improve the
+Bing wrapper. (Wait and Retry or reuse conversation) - [ ] ð§ Write a
+standard provider performance test to improve the stability - [ ] Potential
+support and development of local models - [ ] ð§ Improve compatibility and
+error handling ## ð Table of Contents - [ð What's New](#-whats-new) -
+[ð Table of Contents](#-table-of-contents) - [ð ï¸ Getting Started](#-
+getting-started) + [Docker Container Guide](#docker-container-guide) +
+[Installation Guide for Windows (.exe)](#installation-guide-for-windows-exe) +
+[Use python](#use-python) - [Prerequisites](#prerequisites) - [Install using
+PyPI package:](#install-using-pypi-package) - [Install from source:](#install-
+from-source) - [Install using Docker:](#install-using-docker) - [ð¡ Usage](#-
+usage) * [Text Generation](#text-generation) * [Image Generation](#image-
+generation) * [Web UI](#web-ui) * [Interference API](#interference-api) *
+[Configuration](#configuration) - [ð Providers and Models](#-providers-and-
+models) * [GPT-4](#gpt-4) * [GPT-3.5](#gpt-35) * [Other](#other) * [Models]
+(#models) - [ð Powered by gpt4free](#-powered-by-gpt4free) - [ð¤
+Contribute](#-contribute) + [How do i create a new Provider?](#guide-how-do-i-
+create-a-new-provider) + [How can AI help me with writing code?](#guide-how-
+can-ai-help-me-with-writing-code) - [ð Contributors](#-contributors) -
+[Â©ï¸ Copyright](#-copyright) - [â­ Star History](#-star-history) - [ð
+License](#-license) ## ð ï¸ Getting Started #### Docker Container Guide
+##### Getting Started Quickly: 1. **Install Docker:** Begin by [downloading and
+installing Docker](https://docs.docker.com/get-docker/). 2. **Set Up the
+Container:** Use the following commands to pull the latest image and start the
 container: ```sh docker pull hlohaus789/g4f docker run -p 8080:8080 -p 1337:
 1337 -p 7900:7900 --shm-size="2g" -v ${PWD}/hardir:/app/hardir hlohaus789/g4f:
-latest ``` 3. Open the included client on: [http://localhost:8080/chat/](http:/
-/localhost:8080/chat/) or set the API base in your client to: [http://
-localhost:1337/v1](http://localhost:1337/v1) 4. (Optional) If you need to log
-in to a provider, you can view the desktop from the container here: http://
-localhost:7900/?autoconnect=1&resize=scale&password=secret. ##### Use your
-smartphone: Run the Web UI on Your Smartphone: - [/docs/guides/phone](/docs/
-guides/phone.md) #### Use python ##### Prerequisites: 1. [Download and install
-Python](https://www.python.org/downloads/) (Version 3.10+ is recommended). 2.
-[Install Google Chrome](https://www.google.com/chrome/) for providers with
-webdriver ##### Install using PyPI package: ``` pip install -U g4f[all] ``` How
-do I install only parts or do disable parts? Use partial requirements: [/docs/
-requirements](/docs/requirements.md) ##### Install from source: How do I load
-the project using git and installing the project requirements? Read this
-tutorial and follow it step by step: [/docs/git](/docs/git.md) ##### Install
-using Docker: How do I build and run composer image from source? Use docker-
-compose: [/docs/docker](/docs/docker.md) ## ð¡ Usage #### Text Generation
-```python from g4f.client import Client client = Client() response =
+latest ``` 3. **Access the Client:** - To use the included client, navigate to:
+[http://localhost:8080/chat/](http://localhost:8080/chat/) - Or set the API
+base for your client to: [http://localhost:1337/v1](http://localhost:1337/v1)
+4. **(Optional) Provider Login:** If required, you can access the container's
+desktop here: http://localhost:7900/?autoconnect=1&resize=scale&password=secret
+for provider login purposes. #### Installation Guide for Windows (.exe) To
+ensure the seamless operation of our application, please follow the
+instructions below. These steps are designed to guide you through the
+installation process on Windows operating systems. ##### Prerequisites 1.
+**WebView2 Runtime**: Our application requires the *WebView2 Runtime* to be
+installed on your system. If you do not have it installed, please download and
+install it from the [Microsoft Developer Website](https://
+developer.microsoft.com/en-us/microsoft-edge/webview2/). If you already have
+*WebView2 Runtime* installed but are encountering issues, navigate to
+*Installed Windows Apps*, select *WebView2*, and opt for the repair option.
+##### Installation Steps 2. **Download the Application**: Visit our [latest
+releases page](https://github.com/xtekky/gpt4free/releases/latest) and download
+the most recent version of the application, named `g4f.webview.*.exe`. 3.
+**File Placement**: Once downloaded, transfer the `.exe` file from your
+downloads folder to a directory of your choice on your system, and then execute
+it to run the app. ##### Post-Installation Adjustment 4. **Firewall
+Configuration (Hotfix)**: Upon installation, it may be necessary to adjust your
+Windows Firewall settings to allow the application to operate correctly. To do
+this, access your Windows Firewall settings and allow the application. By
+following these steps, you should be able to successfully install and run the
+application on your Windows system. If you encounter any issues during the
+installation process, please refer to our Issue Tracker or try to get contact
+over Discord for assistance. Run the **Webview UI** on other Platfroms: - [/
+docs/guides/webview](/docs/webview.md) ##### Use your smartphone: Run the Web
+UI on Your Smartphone: - [/docs/guides/phone](/docs/guides/phone.md) #### Use
+python ##### Prerequisites: 1. [Download and install Python](https://
+www.python.org/downloads/) (Version 3.10+ is recommended). 2. [Install Google
+Chrome](https://www.google.com/chrome/) for providers with webdriver #####
+Install using PyPI package: ``` pip install -U g4f[all] ``` How do I install
+only parts or do disable parts? Use partial requirements: [/docs/requirements]
+(/docs/requirements.md) ##### Install from source: How do I load the project
+using git and installing the project requirements? Read this tutorial and
+follow it step by step: [/docs/git](/docs/git.md) ##### Install using Docker:
+How do I build and run composer image from source? Use docker-compose: [/docs/
+docker](/docs/docker.md) ## ð¡ Usage #### Text Generation ```python from
+g4f.client import Client client = Client() response =
 client.chat.completions.create( model="gpt-3.5-turbo", messages=[{"role":
 "user", "content": "Hello"}], ... ) print(response.choices[0].message.content)
 ``` ``` Hello! How can I assist you today? ``` #### Image Generation ```python
 from g4f.client import Client client = Client() response =
 client.images.generate( model="gemini", prompt="a white siamese cat", ... )
 image_url = response.data[0].url ``` [![Image with cat](/docs/cat.jpeg)](/docs/
 client.md) **Full Documentation for Python API** - New Client API like the
 OpenAI Python library: [/docs/client](/docs/client.md) - Legacy API with python
-modules: [/docs/legacy](/docs/legacy.md) ### Webview GUI Open the GUI in a
-window of your OS. Runs on a local/static/ssl server and use a JavaScript API.
-Supports login into the OpenAI Chat, Image Upload and streamed Text Generation.
-Supports all platforms, but only Linux tested. 1. Install all requirements
-with: ```bash pip install g4f[webview] ``` 2. Follow the OS specific steps
-here: [pywebview installation](https://pywebview.flowrl.com/guide/
-installation.html#dependencies) 3. Run the app with: ```python from
-g4f.gui.webview import run_webview run_webview(debug=True) ``` or execute the
-following command: ```bash python -m g4f.gui.webview -debug ``` #### Webserver
-To start the web interface, type the following codes in python: ```python from
-g4f.gui import run_gui run_gui() ``` or execute the following command: ```bash
-python -m g4f.cli gui -port 8080 -debug ``` ### Interference API You can use
-the Interference API to serve other OpenAI integrations with G4F. See: [/docs/
-interference](/docs/interference.md) ### Configuration #### Cookies You need
-cookies for BingCreateImages and the Gemini Provider. From Bing you need the
-"_U" cookie and from Gemini you need the "__Secure-1PSID" cookie. Sometimes you
-doesn't need the "__Secure-1PSID" cookie, but some other auth cookies. You can
-pass the cookies in the create function or you use the `set_cookies` setter
-before you run G4F: ```python from g4f.cookies import set_cookies set_cookies
-(".bing.com", { "_U": "cookie value" }) set_cookies(".google.com", { "__Secure-
-1PSID": "cookie value" }) ... ``` #### .HAR File for OpenaiChat Provider #####
-Generating a .HAR File To utilize the OpenaiChat provider, a .har file is
-required from https://chat.openai.com/. Follow the steps below to create a
-valid .har file: 1. Navigate to https://chat.openai.com/ using your preferred
-web browser and log in with your credentials. 2. Access the Developer Tools in
-your browser. This can typically be done by right-clicking the page and
-selecting "Inspect," or by pressing F12 or Ctrl+Shift+I (Cmd+Option+I on a
-Mac). 3. With the Developer Tools open, switch to the "Network" tab. 4. Reload
-the website to capture the loading process within the Network tab. 5. Initiate
-an action in the chat which can be capture in the .har file. 6. Right-click any
-of the network activities listed and select "Save all as HAR with content" to
-export the .har file. ##### Storing the .HAR File - Place the exported .har
-file in the `./hardir` directory if you are using Docker. Alternatively, you
-can store it in any preferred location within your current working directory.
-Note: Ensure that your .har file is stored securely, as it may contain
-sensitive information. #### Using Proxy If you want to hide or change your IP
-address for the providers, you can set a proxy globally via an environment
-variable: - On macOS and Linux: ```bash export G4F_PROXY="http://host:port" ```
-- On Windows: ```bash set G4F_PROXY=http://host:port ``` ## ð Providers and
-Models ### GPT-4 | Website | Provider | GPT-3.5 | GPT-4 | Stream | Status |
-Auth | | ------ | ------- | ------- | ----- | ------ | ------ | ---- | |
-[bing.com](https://bing.com/chat) | `g4f.Provider.Bing` | â | âï¸ | âï¸
-| ![Unknown](https://img.shields.io/badge/Unknown-grey) | â | | [chatgpt.ai]
-(https://chatgpt.ai) | `g4f.Provider.ChatgptAi` | â | âï¸ | âï¸ | !
-[Active](https://img.shields.io/badge/Active-brightgreen) | â | |
-[liaobots.site](https://liaobots.site) | `g4f.Provider.Liaobots` | âï¸ |
-âï¸ | âï¸ | ![Active](https://img.shields.io/badge/Active-brightgreen) |
-â | | [chat.openai.com](https://chat.openai.com) | `g4f.Provider.OpenaiChat`
-| âï¸ | â | âï¸ | ![Unknown](https://img.shields.io/badge/Unknown-grey)
-| âï¸ | | [raycast.com](https://raycast.com) | `g4f.Provider.Raycast` |
-âï¸ | âï¸ | âï¸ | ![Unknown](https://img.shields.io/badge/Unknown-
-grey) | âï¸ | | [beta.theb.ai](https://beta.theb.ai) | `g4f.Provider.Theb` |
-âï¸ | âï¸ | âï¸ | ![Unknown](https://img.shields.io/badge/Unknown-
-grey) | â | | [you.com](https://you.com) | `g4f.Provider.You` | âï¸ |
-âï¸ | âï¸ | ![Unknown](https://img.shields.io/badge/Unknown-grey) | â |
-### GPT-3.5 | Website | Provider | GPT-3.5 | GPT-4 | Stream | Status | Auth | |
------- | ------- | ------- | ----- | ------ | ------ | ---- | |
-[chat3.aiyunos.top](https://chat3.aiyunos.top/) | `g4f.Provider.AItianhuSpace`
-| âï¸ | â | âï¸ | ![Unknown](https://img.shields.io/badge/Unknown-grey)
-| â | | [chatforai.store](https://chatforai.store) | `g4f.Provider.ChatForAi`
-| âï¸ | â | âï¸ | ![Active](https://img.shields.io/badge/Active-
-brightgreen) | â | | [chatgpt4online.org](https://chatgpt4online.org) |
+modules: [/docs/legacy](/docs/legacy.md) #### Web UI To start the web
+interface, type the following codes in python: ```python from g4f.gui import
+run_gui run_gui() ``` or execute the following command: ```bash python -
+m g4f.cli gui -port 8080 -debug ``` #### Interference API You can use the
+Interference API to serve other OpenAI integrations with G4F. See docs: [/docs/
+interference](/docs/interference.md) Access with: http://localhost:1337/v1 ###
+Configuration #### Cookies You need cookies for BingCreateImages and the Gemini
+Provider. From Bing you need the "_U" cookie and from Gemini you need the
+"__Secure-1PSID" cookie. Sometimes you doesn't need the "__Secure-1PSID"
+cookie, but some other auth cookies. You can pass the cookies in the create
+function or you use the `set_cookies` setter before you run G4F: ```python from
+g4f.cookies import set_cookies set_cookies(".bing.com", { "_U": "cookie value"
+}) set_cookies(".google.com", { "__Secure-1PSID": "cookie value" }) ... ```
+#### .HAR File for OpenaiChat Provider ##### Generating a .HAR File To utilize
+the OpenaiChat provider, a .har file is required from https://chat.openai.com/.
+Follow the steps below to create a valid .har file: 1. Navigate to https://
+chat.openai.com/ using your preferred web browser and log in with your
+credentials. 2. Access the Developer Tools in your browser. This can typically
+be done by right-clicking the page and selecting "Inspect," or by pressing F12
+or Ctrl+Shift+I (Cmd+Option+I on a Mac). 3. With the Developer Tools open,
+switch to the "Network" tab. 4. Reload the website to capture the loading
+process within the Network tab. 5. Initiate an action in the chat which can be
+captured in the .har file. 6. Right-click any of the network activities listed
+and select "Save all as HAR with content" to export the .har file. #####
+Storing the .HAR File - Place the exported .har file in the `./hardir`
+directory if you are using Docker. Alternatively, you can store it in any
+preferred location within your current working directory. Note: Ensure that
+your .har file is stored securely, as it may contain sensitive information.
+#### Using Proxy If you want to hide or change your IP address for the
+providers, you can set a proxy globally via an environment variable: - On macOS
+and Linux: ```bash export G4F_PROXY="http://host:port" ``` - On Windows:
+```bash set G4F_PROXY=http://host:port ``` ## ð Providers and Models ###
+GPT-4 | Website | Provider | GPT-3.5 | GPT-4 | Stream | Status | Auth | | -----
+- | ------- | ------- | ----- | ------ | ------ | ---- | | [bing.com](https://
+bing.com/chat) | `g4f.Provider.Bing` | â | âï¸ | âï¸ | ![Unknown]
+(https://img.shields.io/badge/Unknown-grey) | â | | [chatgpt.ai](https://
+chatgpt.ai) | `g4f.Provider.ChatgptAi` | â | âï¸ | âï¸ | ![Active]
+(https://img.shields.io/badge/Active-brightgreen) | â | | [liaobots.site]
+(https://liaobots.site) | `g4f.Provider.Liaobots` | âï¸ | âï¸ | âï¸ |
+![Active](https://img.shields.io/badge/Active-brightgreen) | â | |
+[chat.openai.com](https://chat.openai.com) | `g4f.Provider.OpenaiChat` | âï¸
+| â | âï¸ | ![Unknown](https://img.shields.io/badge/Unknown-grey) | âï¸
+| | [raycast.com](https://raycast.com) | `g4f.Provider.Raycast` | âï¸ |
+âï¸ | âï¸ | ![Unknown](https://img.shields.io/badge/Unknown-grey) |
+âï¸ | | [beta.theb.ai](https://beta.theb.ai) | `g4f.Provider.Theb` | âï¸
+| âï¸ | âï¸ | ![Unknown](https://img.shields.io/badge/Unknown-grey) | â
+| | [you.com](https://you.com) | `g4f.Provider.You` | âï¸ | âï¸ | âï¸
+| ![Unknown](https://img.shields.io/badge/Unknown-grey) | â | ### GPT-3.5 |
+Website | Provider | GPT-3.5 | GPT-4 | Stream | Status | Auth | | ------ | ----
+--- | ------- | ----- | ------ | ------ | ---- | | [chat3.aiyunos.top](https://
+chat3.aiyunos.top/) | `g4f.Provider.AItianhuSpace` | âï¸ | â | âï¸ | !
+[Unknown](https://img.shields.io/badge/Unknown-grey) | â | |
+[chatforai.store](https://chatforai.store) | `g4f.Provider.ChatForAi` | âï¸
+| â | âï¸ | ![Active](https://img.shields.io/badge/Active-brightgreen) |
+â | | [chatgpt4online.org](https://chatgpt4online.org) |
 `g4f.Provider.Chatgpt4Online` | âï¸ | â | âï¸ | ![Active](https://
 img.shields.io/badge/Active-brightgreen) | â | | [chatgpt-free.cc](https://
 www.chatgpt-free.cc) | `g4f.Provider.ChatgptNext` | âï¸ | â | âï¸ | !
 [Active](https://img.shields.io/badge/Active-brightgreen) | â | |
 [chatgptx.de](https://chatgptx.de) | `g4f.Provider.ChatgptX` | âï¸ | â |
 âï¸ | ![Active](https://img.shields.io/badge/Active-brightgreen) | â | |
 [flowgpt.com](https://flowgpt.com/chat) | `g4f.Provider.FlowGpt` | âï¸ | â
@@ -319,30 +339,68 @@
 improvements, your input is valued. Creating a pull request is all it takes â
 our co-pilot will handle the code review process. Once all changes have been
 addressed, we'll merge the pull request into the main branch and release the
 updates at a later time. ###### Guide: How do i create a new Provider? - Read:
 [/docs/guides/create_provider](/docs/guides/create_provider.md) ###### Guide:
 How can AI help me with writing code? - Read: [/docs/guides/help_me](/docs/
 guides/help_me.md) ## ð Contributors A list of all contributors is available
-[here](https://github.com/xtekky/gpt4free/graphs/contributors) The
-[`Vercel.py`](https://github.com/xtekky/gpt4free/blob/main/g4f/Provider/
-Vercel.py) file contains code from [vercel-llm-api](https://github.com/
-ading2210/vercel-llm-api) by [@ading2210](https://github.com/ading2210), which
-is licensed under the [GNU GPL v3](https://www.gnu.org/licenses/gpl-3.0.txt)
-Top 1 Contributor: [@hlohaus](https://github.com/hlohaus) ## Â©ï¸ Copyright
-This program is licensed under the [GNU GPL v3](https://www.gnu.org/licenses/
-gpl-3.0.txt) ``` xtekky/gpt4free: Copyright (C) 2023 xtekky This program is
-free software: you can redistribute it and/or modify it under the terms of the
-GNU General Public License as published by the Free Software Foundation, either
-version 3 of the License, or (at your option) any later version. This program
-is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
-without even the implied warranty of MERCHANTABILITY or FITNESS FOR A
-PARTICULAR PURPOSE. See the GNU General Public License for more details. You
-should have received a copy of the GNU General Public License along with this
-program. If not, see
+[here](https://github.com/xtekky/gpt4free/graphs/contributors) _[_h_t_t_p_s_:_/_/
+_a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_9_8_6_1_4_6_6_6_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
+_a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_9_8_3_5_7_7_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
+_a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_3_6_8_3_0_5_3_4_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
+_a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_2_2_4_1_5_4_6_3_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
+_a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_1_3_9_6_6_2_2_8_2_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
+_a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_3_6_0_5_1_6_0_3_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
+_a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_2_0_5_8_5_2_3_6_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
+_a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_7_3_4_8_5_4_2_1_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
+_a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_6_9_0_8_2_4_9_8_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
+_a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_1_0_0_1_9_3_7_4_0_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
+_a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_6_3_7_8_2_9_0_3_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
+_a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_1_3_9_9_1_4_3_4_7_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
+_a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_8_1_0_7_4_9_3_6_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
+_a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_2_5_4_2_5_2_1_7_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
+_a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_2_6_7_1_4_6_6_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
+_a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_5_4_5_3_5_4_1_4_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
+_a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_6_3_5_4_3_7_1_6_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
+_a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_5_5_2_5_7_0_5_4_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
+_a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_1_4_3_0_2_0_2_9_3_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
+_a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_6_5_3_1_4_6_2_9_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
+_a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_7_1_8_6_7_2_4_5_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
+_a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_2_2_6_3_3_3_8_5_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
+_a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_1_3_6_1_7_0_5_4_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
+_a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_4_4_6_1_3_6_7_8_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
+_a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_4_7_8_4_6_2_0_2_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
+_a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_1_0_9_8_4_4_0_1_9_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
+_a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_7_7_6_3_6_0_2_1_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
+_a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_9_5_6_6_3_2_2_8_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
+_a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_2_9_3_2_2_7_2_1_?_v_=_4_&_s_=_4_5_]_[_h_t_t_p_s_:_/_/
+_a_v_a_t_a_r_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_u_/_9_7_8_0_7_7_7_2_?_v_=_4_&_s_=_4_5_][https://
+avatars.githubusercontent.com/u/71154407?s=45&v=4][https://
+avatars.githubusercontent.com/u/12299238?s=45&v=4][https://
+avatars.githubusercontent.com/u/97126670?s=45&v=4][https://
+avatars.githubusercontent.com/u/81407603?v=4&s=45]- The [`Vercel.py`](g4f/
+Provider/Vercel.py) file contains code from [vercel-llm-api](https://
+github.com/ading2210/vercel-llm-api) by [@ading2210](https://github.com/
+ading2210) - The [`har_file.py`](g4f/Provider/openai/har_file.py) has input
+from [xqdoo00o/ChatGPT-to-API](https://github.com/xqdoo00o/ChatGPT-to-API) -
+The [`PerplexityLabs.py`](g4f/Provider/openai/har_file.py) has input from
+[nathanrchn/perplexityai](https://github.com/nathanrchn/perplexityai) - The
+[`Gemini.py`](g4f/Provider/needs_auth/Gemini.py) has input from [dsdanielpark/
+Gemini-API](https://github.com/dsdanielpark/Gemini-API) *Having input implies
+that the AI's code generation utilized it as one of many sources.* ## Â©ï¸
+Copyright This program is licensed under the [GNU GPL v3](https://www.gnu.org/
+licenses/gpl-3.0.txt) ``` xtekky/gpt4free: Copyright (C) 2023 xtekky This
+program is free software: you can redistribute it and/or modify it under the
+terms of the GNU General Public License as published by the Free Software
+Foundation, either version 3 of the License, or (at your option) any later
+version. This program is distributed in the hope that it will be useful, but
+WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or
+FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more
+details. You should have received a copy of the GNU General Public License
+along with this program. If not, see
 www.gnu.org/licenses/>. ``` ## â­ Star History _[_S_t_a_r_ _H_i_s_t_o_r_y_ _C_h_a_r_t_]## ð
 License
 [https://upload.wikimedia.org/wikipedia/ [https://img.shields.io/badge/License-
    commons/thumb/9/93/GPLv3_Logo.svg/    GNU_GPL_v3.0-red.svg]
        1200px-GPLv3_Logo.svg.png]        This project is licensed under
                                          _G_N_U___G_P_L___v_3_._0.
                                                              (_ð___¼_ _B_a_c_k_ _t_o_ _t_o_p)
```

### Comparing `g4f-0.2.8.0/g4f.egg-info/SOURCES.txt` & `g4f-0.2.8.1/g4f.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 LICENSE
 MANIFEST.in
 README.md
 setup.py
 g4f/__init__.py
 g4f/cli.py
-g4f/client.py
 g4f/cookies.py
 g4f/debug.py
 g4f/errors.py
 g4f/image.py
 g4f/models.py
 g4f/stubs.py
 g4f/typing.py
@@ -38,14 +37,15 @@
 g4f/Provider/GigaChat.py
 g4f/Provider/GptTalkRu.py
 g4f/Provider/HuggingChat.py
 g4f/Provider/HuggingFace.py
 g4f/Provider/Koala.py
 g4f/Provider/Liaobots.py
 g4f/Provider/Llama2.py
+g4f/Provider/Local.py
 g4f/Provider/PerplexityLabs.py
 g4f/Provider/Pi.py
 g4f/Provider/Vercel.py
 g4f/Provider/You.py
 g4f/Provider/__init__.py
 g4f/Provider/base_provider.py
 g4f/Provider/helper.py
@@ -77,27 +77,29 @@
 g4f/Provider/deprecated/GetGpt.py
 g4f/Provider/deprecated/H2o.py
 g4f/Provider/deprecated/Hashnode.py
 g4f/Provider/deprecated/Lockchat.py
 g4f/Provider/deprecated/Myshell.py
 g4f/Provider/deprecated/NoowAi.py
 g4f/Provider/deprecated/Opchatgpts.py
+g4f/Provider/deprecated/OpenAssistant.py
 g4f/Provider/deprecated/Phind.py
 g4f/Provider/deprecated/V50.py
 g4f/Provider/deprecated/Vercel.py
 g4f/Provider/deprecated/Vitalentum.py
 g4f/Provider/deprecated/VoiGpt.py
 g4f/Provider/deprecated/Wewordle.py
 g4f/Provider/deprecated/Wuguokai.py
 g4f/Provider/deprecated/Ylokh.py
 g4f/Provider/deprecated/Yqcloud.py
 g4f/Provider/deprecated/__init__.py
 g4f/Provider/gigachat_crt/russian_trusted_root_ca_pem.crt
 g4f/Provider/needs_auth/Gemini.py
-g4f/Provider/needs_auth/OpenAssistant.py
+g4f/Provider/needs_auth/Groq.py
+g4f/Provider/needs_auth/Openai.py
 g4f/Provider/needs_auth/OpenaiChat.py
 g4f/Provider/needs_auth/Poe.py
 g4f/Provider/needs_auth/Raycast.py
 g4f/Provider/needs_auth/Theb.py
 g4f/Provider/needs_auth/ThebApi.py
 g4f/Provider/needs_auth/__init__.py
 g4f/Provider/not_working/AItianhu.py
@@ -130,19 +132,30 @@
 g4f/Provider/selenium/TalkAi.py
 g4f/Provider/selenium/__init__.py
 g4f/Provider/unfinished/AiChatting.py
 g4f/Provider/unfinished/ChatAiGpt.py
 g4f/Provider/unfinished/Komo.py
 g4f/Provider/unfinished/MikuChat.py
 g4f/Provider/unfinished/__init__.py
+g4f/Provider/you/__init__.py
+g4f/Provider/you/har_file.py
 g4f/api/__init__.py
 g4f/api/_logging.py
 g4f/api/_tokenizer.py
 g4f/api/run.py
+g4f/client/__init__.py
+g4f/client/async_client.py
+g4f/client/client.py
+g4f/client/helper.py
+g4f/client/image_models.py
+g4f/client/service.py
+g4f/client/stubs.py
+g4f/client/types.py
 g4f/gui/__init__.py
+g4f/gui/gui_parser.py
 g4f/gui/run.py
 g4f/gui/webview.py
 g4f/gui/client/index.html
 g4f/gui/client/static/css/style.css
 g4f/gui/client/static/img/android-chrome-192x192.png
 g4f/gui/client/static/img/android-chrome-512x512.png
 g4f/gui/client/static/img/apple-touch-icon.png
@@ -151,24 +164,27 @@
 g4f/gui/client/static/img/gpt.png
 g4f/gui/client/static/img/site.webmanifest
 g4f/gui/client/static/img/user.png
 g4f/gui/client/static/js/chat.v1.js
 g4f/gui/client/static/js/highlight.min.js
 g4f/gui/client/static/js/highlightjs-copy.min.js
 g4f/gui/client/static/js/icons.js
+g4f/gui/server/__init__.py
 g4f/gui/server/android_gallery.py
 g4f/gui/server/api.py
 g4f/gui/server/app.py
 g4f/gui/server/backend.py
 g4f/gui/server/config.py
 g4f/gui/server/internet.py
+g4f/gui/server/js_api.py
 g4f/gui/server/website.py
 g4f/local/__init__.py
-g4f/local/_engine.py
-g4f/local/_models.py
+g4f/locals/__init__.py
+g4f/locals/models.py
+g4f/locals/provider.py
 g4f/providers/__init__.py
 g4f/providers/base_provider.py
 g4f/providers/conversation.py
 g4f/providers/create_images.py
 g4f/providers/helper.py
 g4f/providers/retry_provider.py
 g4f/providers/types.py
```

### Comparing `g4f-0.2.8.0/g4f.egg-info/requires.txt` & `g4f-0.2.8.1/g4f.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `g4f-0.2.8.0/setup.py` & `g4f-0.2.8.1/setup.py`

 * *Files identical despite different names*

