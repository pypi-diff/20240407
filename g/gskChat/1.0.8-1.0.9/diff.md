# Comparing `tmp/gskChat-1.0.8.tar.gz` & `tmp/gskChat-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gskChat-1.0.8.tar", last modified: Mon Mar 25 09:32:27 2024, max compression
+gzip compressed data, was "gskChat-1.0.9.tar", last modified: Sun Apr  7 13:59:21 2024, max compression
```

## Comparing `gskChat-1.0.8.tar` & `gskChat-1.0.9.tar`

### file list

```diff
@@ -1,392 +1,393 @@
-drwxrwxrwx   0        0        0        0 2024-03-25 09:32:27.829389 gskChat-1.0.8/
--rw-rw-rw-   0        0        0      224 2024-03-24 15:15:13.000000 gskChat-1.0.8/MANIFEST.in
--rw-rw-rw-   0        0        0     2874 2024-03-25 09:32:27.829389 gskChat-1.0.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-03-25 09:32:27.411320 gskChat-1.0.8/gskChat/
-drwxrwxrwx   0        0        0        0 2024-03-25 09:32:27.450741 gskChat-1.0.8/gskChat/Provider/
--rw-rw-rw-   0        0        0     1607 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/Provider/Aura.py
--rw-rw-rw-   0        0        0    20640 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/Provider/Bing.py
--rw-rw-rw-   0        0        0     2193 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/Provider/BingCreateImages.py
--rw-rw-rw-   0        0        0     2508 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/Provider/ChatForAi.py
--rw-rw-rw-   0        0        0     2653 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/Provider/Chatgpt4Online.py
--rw-rw-rw-   0        0        0     3608 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/Provider/ChatgptAi.py
--rw-rw-rw-   0        0        0     2855 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/Provider/ChatgptFree.py
--rw-rw-rw-   0        0        0     2503 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/Provider/ChatgptNext.py
--rw-rw-rw-   0        0        0     4278 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/Provider/ChatgptX.py
--rw-rw-rw-   0        0        0     3526 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/Provider/DeepInfra.py
--rw-rw-rw-   0        0        0     3196 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/Provider/FlowGpt.py
--rw-rw-rw-   0        0        0     2530 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/Provider/FreeChatgpt.py
--rw-rw-rw-   0        0        0     1791 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/Provider/FreeGpt.py
--rw-rw-rw-   0        0        0     3937 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/Provider/GeminiPro.py
--rw-rw-rw-   0        0        0     2557 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/Provider/GeminiProChat.py
--rw-rw-rw-   0        0        0     3926 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/Provider/GigaChat.py
--rw-rw-rw-   0        0        0     2321 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/Provider/GptTalkRu.py
--rw-rw-rw-   0        0        0     3615 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/Provider/HuggingChat.py
--rw-rw-rw-   0        0        0     2940 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/Provider/HuggingFace.py
--rw-rw-rw-   0        0        0     2485 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/Provider/Koala.py
--rw-rw-rw-   0        0        0     5099 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/Provider/Liaobots.py
--rw-rw-rw-   0        0        0     3105 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/Provider/Llama2.py
--rw-rw-rw-   0        0        0     3951 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/Provider/PerplexityLabs.py
--rw-rw-rw-   0        0        0     2355 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/Provider/Pi.py
--rw-rw-rw-   0        0        0     4027 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/Provider/Vercel.py
--rw-rw-rw-   0        0        0     7243 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/Provider/You.py
--rw-rw-rw-   0        0        0     2047 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/Provider/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-25 09:32:27.476416 gskChat-1.0.8/gskChat/Provider/__pycache__/
--rw-rw-rw-   0        0        0     2618 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/Provider/__pycache__/Aura.cpython-312.pyc
--rw-rw-rw-   0        0        0    20847 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/Provider/__pycache__/Bing.cpython-312.pyc
--rw-rw-rw-   0        0        0     3577 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/Provider/__pycache__/BingCreateImages.cpython-312.pyc
--rw-rw-rw-   0        0        0     3774 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/Provider/__pycache__/ChatForAi.cpython-312.pyc
--rw-rw-rw-   0        0        0     3889 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/Provider/__pycache__/Chatgpt4Online.cpython-312.pyc
--rw-rw-rw-   0        0        0     4740 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/Provider/__pycache__/ChatgptAi.cpython-312.pyc
--rw-rw-rw-   0        0        0     3951 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/Provider/__pycache__/ChatgptFree.cpython-312.pyc
--rw-rw-rw-   0        0        0     3325 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/Provider/__pycache__/ChatgptNext.cpython-312.pyc
--rw-rw-rw-   0        0        0     5386 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/Provider/__pycache__/ChatgptX.cpython-312.pyc
--rw-rw-rw-   0        0        0     4547 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/Provider/__pycache__/DeepInfra.cpython-312.pyc
--rw-rw-rw-   0        0        0     3912 2024-03-24 15:25:24.000000 gskChat-1.0.8/gskChat/Provider/__pycache__/FlowGpt.cpython-312.pyc
--rw-rw-rw-   0        0        0     3552 2024-03-24 15:25:24.000000 gskChat-1.0.8/gskChat/Provider/__pycache__/FreeChatgpt.cpython-312.pyc
--rw-rw-rw-   0        0        0     3089 2024-03-24 15:25:24.000000 gskChat-1.0.8/gskChat/Provider/__pycache__/FreeGpt.cpython-312.pyc
--rw-rw-rw-   0        0        0     5017 2024-03-24 15:25:24.000000 gskChat-1.0.8/gskChat/Provider/__pycache__/GeminiPro.cpython-312.pyc
--rw-rw-rw-   0        0        0     3887 2024-03-24 15:25:24.000000 gskChat-1.0.8/gskChat/Provider/__pycache__/GeminiProChat.cpython-312.pyc
--rw-rw-rw-   0        0        0     5557 2024-03-24 15:25:24.000000 gskChat-1.0.8/gskChat/Provider/__pycache__/GigaChat.cpython-312.pyc
--rw-rw-rw-   0        0        0     4066 2024-03-24 15:25:24.000000 gskChat-1.0.8/gskChat/Provider/__pycache__/GptTalkRu.cpython-312.pyc
--rw-rw-rw-   0        0        0     5345 2024-03-24 15:25:24.000000 gskChat-1.0.8/gskChat/Provider/__pycache__/HuggingChat.cpython-312.pyc
--rw-rw-rw-   0        0        0     4428 2024-03-24 15:25:24.000000 gskChat-1.0.8/gskChat/Provider/__pycache__/HuggingFace.cpython-312.pyc
--rw-rw-rw-   0        0        0     3521 2024-03-24 15:25:24.000000 gskChat-1.0.8/gskChat/Provider/__pycache__/Koala.cpython-312.pyc
--rw-rw-rw-   0        0        0     5673 2024-03-24 15:25:24.000000 gskChat-1.0.8/gskChat/Provider/__pycache__/Liaobots.cpython-312.pyc
--rw-rw-rw-   0        0        0     4082 2024-03-24 15:25:24.000000 gskChat-1.0.8/gskChat/Provider/__pycache__/Llama2.cpython-312.pyc
--rw-rw-rw-   0        0        0     5769 2024-03-24 15:25:24.000000 gskChat-1.0.8/gskChat/Provider/__pycache__/PerplexityLabs.cpython-312.pyc
--rw-rw-rw-   0        0        0     3523 2024-03-24 15:25:24.000000 gskChat-1.0.8/gskChat/Provider/__pycache__/Pi.cpython-312.pyc
--rw-rw-rw-   0        0        0     5112 2024-03-24 15:25:24.000000 gskChat-1.0.8/gskChat/Provider/__pycache__/Vercel.cpython-312.pyc
--rw-rw-rw-   0        0        0     9701 2024-03-24 15:25:24.000000 gskChat-1.0.8/gskChat/Provider/__pycache__/You.cpython-312.pyc
--rw-rw-rw-   0        0        0     2677 2024-03-24 15:25:24.000000 gskChat-1.0.8/gskChat/Provider/__pycache__/__init__.cpython-312.pyc
--rw-rw-rw-   0        0        0      323 2024-03-24 15:25:24.000000 gskChat-1.0.8/gskChat/Provider/__pycache__/base_provider.cpython-312.pyc
--rw-rw-rw-   0        0        0      333 2024-03-24 15:25:24.000000 gskChat-1.0.8/gskChat/Provider/__pycache__/helper.cpython-312.pyc
--rw-rw-rw-   0        0        0       86 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/Provider/base_provider.py
-drwxrwxrwx   0        0        0        0 2024-03-25 09:32:27.478412 gskChat-1.0.8/gskChat/Provider/bing/
--rw-rw-rw-   0        0        0        0 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/Provider/bing/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-25 09:32:27.482401 gskChat-1.0.8/gskChat/Provider/bing/__pycache__/
--rw-rw-rw-   0        0        0      203 2024-03-24 15:25:24.000000 gskChat-1.0.8/gskChat/Provider/bing/__pycache__/__init__.cpython-312.pyc
--rw-rw-rw-   0        0        0     5088 2024-03-24 15:25:24.000000 gskChat-1.0.8/gskChat/Provider/bing/__pycache__/conversation.cpython-312.pyc
--rw-rw-rw-   0        0        0    10876 2024-03-24 15:25:24.000000 gskChat-1.0.8/gskChat/Provider/bing/__pycache__/create_images.cpython-312.pyc
--rw-rw-rw-   0        0        0     6076 2024-03-24 15:25:24.000000 gskChat-1.0.8/gskChat/Provider/bing/__pycache__/upload_image.cpython-312.pyc
--rw-rw-rw-   0        0        0     3468 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/Provider/bing/conversation.py
--rw-rw-rw-   0        0        0     7597 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/Provider/bing/create_images.py
--rw-rw-rw-   0        0        0     4746 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/Provider/bing/upload_image.py
-drwxrwxrwx   0        0        0        0 2024-03-25 09:32:27.510330 gskChat-1.0.8/gskChat/Provider/deprecated/
--rw-rw-rw-   0        0        0     1397 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/Provider/deprecated/Acytoo.py
--rw-rw-rw-   0        0        0     1669 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/Provider/deprecated/AiAsk.py
--rw-rw-rw-   0        0        0     2196 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/Provider/deprecated/AiChatOnline.py
--rw-rw-rw-   0        0        0     1148 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/Provider/deprecated/AiService.py
--rw-rw-rw-   0        0        0     1396 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/Provider/deprecated/Aibn.py
--rw-rw-rw-   0        0        0     2517 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/Provider/deprecated/Aichat.py
--rw-rw-rw-   0        0        0     3358 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/Provider/deprecated/Ails.py
--rw-rw-rw-   0        0        0     2952 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/Provider/deprecated/Aivvm.py
--rw-rw-rw-   0        0        0     2807 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/Provider/deprecated/Berlin.py
--rw-rw-rw-   0        0        0     1934 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/Provider/deprecated/ChatAnywhere.py
--rw-rw-rw-   0        0        0     1303 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/Provider/deprecated/ChatgptDuo.py
--rw-rw-rw-   0        0        0     1873 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/Provider/deprecated/CodeLinkAva.py
--rw-rw-rw-   0        0        0     1356 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/Provider/deprecated/Cromicle.py
--rw-rw-rw-   0        0        0     2498 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/Provider/deprecated/DfeHub.py
--rw-rw-rw-   0        0        0     3398 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/Provider/deprecated/EasyChat.py
--rw-rw-rw-   0        0        0     2755 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/Provider/deprecated/Equing.py
--rw-rw-rw-   0        0        0     4018 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/Provider/deprecated/FakeGpt.py
--rw-rw-rw-   0        0        0     2929 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/Provider/deprecated/FastGpt.py
--rw-rw-rw-   0        0        0     1282 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/Provider/deprecated/Forefront.py
--rw-rw-rw-   0        0        0     3552 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/Provider/deprecated/GPTalk.py
--rw-rw-rw-   0        0        0     2658 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/Provider/deprecated/GeekGpt.py
--rw-rw-rw-   0        0        0     2515 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/Provider/deprecated/GetGpt.py
--rw-rw-rw-   0        0        0     2925 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/Provider/deprecated/H2o.py
--rw-rw-rw-   0        0        0     2674 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/Provider/deprecated/Hashnode.py
--rw-rw-rw-   0        0        0     1700 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/Provider/deprecated/Lockchat.py
--rw-rw-rw-   0        0        0     5050 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/Provider/deprecated/Myshell.py
--rw-rw-rw-   0        0        0     2500 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/Provider/deprecated/NoowAi.py
--rw-rw-rw-   0        0        0     2287 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/Provider/deprecated/Opchatgpts.py
--rw-rw-rw-   0        0        0     5353 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/Provider/deprecated/Phind.py
--rw-rw-rw-   0        0        0     2077 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/Provider/deprecated/V50.py
--rw-rw-rw-   0        0        0    12167 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/Provider/deprecated/Vercel.py
--rw-rw-rw-   0        0        0     1964 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/Provider/deprecated/Vitalentum.py
--rw-rw-rw-   0        0        0     3415 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/Provider/deprecated/VoiGpt.py
--rw-rw-rw-   0        0        0     2464 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/Provider/deprecated/Wewordle.py
--rw-rw-rw-   0        0        0     2020 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/Provider/deprecated/Wuguokai.py
--rw-rw-rw-   0        0        0     1976 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/Provider/deprecated/Ylokh.py
--rw-rw-rw-   0        0        0     1922 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/Provider/deprecated/Yqcloud.py
--rw-rw-rw-   0        0        0     1194 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/Provider/deprecated/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-25 09:32:27.544746 gskChat-1.0.8/gskChat/Provider/deprecated/__pycache__/
--rw-rw-rw-   0        0        0     2523 2024-03-24 15:25:24.000000 gskChat-1.0.8/gskChat/Provider/deprecated/__pycache__/Acytoo.cpython-312.pyc
--rw-rw-rw-   0        0        0     2705 2024-03-24 15:25:24.000000 gskChat-1.0.8/gskChat/Provider/deprecated/__pycache__/AiAsk.cpython-312.pyc
--rw-rw-rw-   0        0        0     3107 2024-03-24 15:25:24.000000 gskChat-1.0.8/gskChat/Provider/deprecated/__pycache__/AiChatOnline.cpython-312.pyc
--rw-rw-rw-   0        0        0     1976 2024-03-24 15:25:24.000000 gskChat-1.0.8/gskChat/Provider/deprecated/__pycache__/AiService.cpython-312.pyc
--rw-rw-rw-   0        0        0     2702 2024-03-24 15:25:24.000000 gskChat-1.0.8/gskChat/Provider/deprecated/__pycache__/Aibn.cpython-312.pyc
--rw-rw-rw-   0        0        0     3337 2024-03-24 15:25:24.000000 gskChat-1.0.8/gskChat/Provider/deprecated/__pycache__/Aichat.cpython-312.pyc
--rw-rw-rw-   0        0        0     4946 2024-03-24 15:25:24.000000 gskChat-1.0.8/gskChat/Provider/deprecated/__pycache__/Ails.cpython-312.pyc
--rw-rw-rw-   0        0        0     3266 2024-03-24 15:25:24.000000 gskChat-1.0.8/gskChat/Provider/deprecated/__pycache__/Aivvm.cpython-312.pyc
--rw-rw-rw-   0        0        0     3969 2024-03-24 15:25:24.000000 gskChat-1.0.8/gskChat/Provider/deprecated/__pycache__/Berlin.cpython-312.pyc
--rw-rw-rw-   0        0        0     2911 2024-03-24 15:25:24.000000 gskChat-1.0.8/gskChat/Provider/deprecated/__pycache__/ChatAnywhere.cpython-312.pyc
--rw-rw-rw-   0        0        0     2243 2024-03-24 15:25:24.000000 gskChat-1.0.8/gskChat/Provider/deprecated/__pycache__/ChatgptDuo.cpython-312.pyc
--rw-rw-rw-   0        0        0     2831 2024-03-24 15:25:24.000000 gskChat-1.0.8/gskChat/Provider/deprecated/__pycache__/CodeLinkAva.cpython-312.pyc
--rw-rw-rw-   0        0        0     2812 2024-03-24 15:25:24.000000 gskChat-1.0.8/gskChat/Provider/deprecated/__pycache__/Cromicle.cpython-312.pyc
--rw-rw-rw-   0        0        0     3098 2024-03-24 15:25:24.000000 gskChat-1.0.8/gskChat/Provider/deprecated/__pycache__/DfeHub.cpython-312.pyc
--rw-rw-rw-   0        0        0     4043 2024-03-24 15:25:24.000000 gskChat-1.0.8/gskChat/Provider/deprecated/__pycache__/EasyChat.cpython-312.pyc
--rw-rw-rw-   0        0        0     3381 2024-03-24 15:25:24.000000 gskChat-1.0.8/gskChat/Provider/deprecated/__pycache__/Equing.cpython-312.pyc
--rw-rw-rw-   0        0        0     5651 2024-03-24 15:25:24.000000 gskChat-1.0.8/gskChat/Provider/deprecated/__pycache__/FakeGpt.cpython-312.pyc
--rw-rw-rw-   0        0        0     3377 2024-03-24 15:25:24.000000 gskChat-1.0.8/gskChat/Provider/deprecated/__pycache__/FastGpt.cpython-312.pyc
--rw-rw-rw-   0        0        0     1953 2024-03-24 15:25:24.000000 gskChat-1.0.8/gskChat/Provider/deprecated/__pycache__/Forefront.cpython-312.pyc
--rw-rw-rw-   0        0        0     5271 2024-03-24 15:25:24.000000 gskChat-1.0.8/gskChat/Provider/deprecated/__pycache__/GPTalk.cpython-312.pyc
--rw-rw-rw-   0        0        0     3197 2024-03-24 15:25:24.000000 gskChat-1.0.8/gskChat/Provider/deprecated/__pycache__/GeekGpt.cpython-312.pyc
--rw-rw-rw-   0        0        0     2831 2024-03-24 15:25:24.000000 gskChat-1.0.8/gskChat/Provider/deprecated/__pycache__/GetGpt.cpython-312.pyc
--rw-rw-rw-   0        0        0     4367 2024-03-24 15:25:24.000000 gskChat-1.0.8/gskChat/Provider/deprecated/__pycache__/H2o.cpython-312.pyc
--rw-rw-rw-   0        0        0     4072 2024-03-24 15:25:24.000000 gskChat-1.0.8/gskChat/Provider/deprecated/__pycache__/Hashnode.cpython-312.pyc
--rw-rw-rw-   0        0        0     2331 2024-03-24 15:25:24.000000 gskChat-1.0.8/gskChat/Provider/deprecated/__pycache__/Lockchat.cpython-312.pyc
--rw-rw-rw-   0        0        0     7947 2024-03-24 15:25:24.000000 gskChat-1.0.8/gskChat/Provider/deprecated/__pycache__/Myshell.cpython-312.pyc
--rw-rw-rw-   0        0        0     3339 2024-03-24 15:25:24.000000 gskChat-1.0.8/gskChat/Provider/deprecated/__pycache__/NoowAi.cpython-312.pyc
--rw-rw-rw-   0        0        0     3166 2024-03-24 15:25:24.000000 gskChat-1.0.8/gskChat/Provider/deprecated/__pycache__/Opchatgpts.cpython-312.pyc
--rw-rw-rw-   0        0        0     7793 2024-03-24 15:25:24.000000 gskChat-1.0.8/gskChat/Provider/deprecated/__pycache__/Phind.cpython-312.pyc
--rw-rw-rw-   0        0        0     2607 2024-03-24 15:25:24.000000 gskChat-1.0.8/gskChat/Provider/deprecated/__pycache__/V50.cpython-312.pyc
--rw-rw-rw-   0        0        0     8348 2024-03-24 15:25:24.000000 gskChat-1.0.8/gskChat/Provider/deprecated/__pycache__/Vercel.cpython-312.pyc
--rw-rw-rw-   0        0        0     3117 2024-03-24 15:25:24.000000 gskChat-1.0.8/gskChat/Provider/deprecated/__pycache__/Vitalentum.cpython-312.pyc
--rw-rw-rw-   0        0        0     3644 2024-03-24 15:25:24.000000 gskChat-1.0.8/gskChat/Provider/deprecated/__pycache__/VoiGpt.cpython-312.pyc
--rw-rw-rw-   0        0        0     3606 2024-03-24 15:25:24.000000 gskChat-1.0.8/gskChat/Provider/deprecated/__pycache__/Wewordle.cpython-312.pyc
--rw-rw-rw-   0        0        0     2702 2024-03-24 15:25:24.000000 gskChat-1.0.8/gskChat/Provider/deprecated/__pycache__/Wuguokai.cpython-312.pyc
--rw-rw-rw-   0        0        0     3036 2024-03-24 15:25:24.000000 gskChat-1.0.8/gskChat/Provider/deprecated/__pycache__/Ylokh.cpython-312.pyc
--rw-rw-rw-   0        0        0     3066 2024-03-24 15:25:24.000000 gskChat-1.0.8/gskChat/Provider/deprecated/__pycache__/Yqcloud.cpython-312.pyc
--rw-rw-rw-   0        0        0     1269 2024-03-24 15:25:24.000000 gskChat-1.0.8/gskChat/Provider/deprecated/__pycache__/__init__.cpython-312.pyc
-drwxrwxrwx   0        0        0        0 2024-03-25 09:32:27.549737 gskChat-1.0.8/gskChat/Provider/gigachat_crt/
--rw-rw-rw-   0        0        0     2056 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/Provider/gigachat_crt/russian_trusted_root_ca_pem.crt
--rw-rw-rw-   0        0        0      111 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/Provider/helper.py
-drwxrwxrwx   0        0        0        0 2024-03-25 09:32:27.555716 gskChat-1.0.8/gskChat/Provider/needs_auth/
--rw-rw-rw-   0        0        0     8145 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/Provider/needs_auth/Gemini.py
--rw-rw-rw-   0        0        0     3309 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/Provider/needs_auth/OpenAssistant.py
--rw-rw-rw-   0        0        0    30868 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/Provider/needs_auth/OpenaiChat.py
--rw-rw-rw-   0        0        0     4289 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/Provider/needs_auth/Poe.py
--rw-rw-rw-   0        0        0     1897 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/Provider/needs_auth/Raycast.py
--rw-rw-rw-   0        0        0     5465 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/Provider/needs_auth/Theb.py
--rw-rw-rw-   0        0        0     2655 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/Provider/needs_auth/ThebApi.py
--rw-rw-rw-   0        0        0      245 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/Provider/needs_auth/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-25 09:32:27.563696 gskChat-1.0.8/gskChat/Provider/needs_auth/__pycache__/
--rw-rw-rw-   0        0        0    12063 2024-03-24 15:25:24.000000 gskChat-1.0.8/gskChat/Provider/needs_auth/__pycache__/Gemini.cpython-312.pyc
--rw-rw-rw-   0        0        0     4902 2024-03-24 15:25:24.000000 gskChat-1.0.8/gskChat/Provider/needs_auth/__pycache__/OpenAssistant.cpython-312.pyc
--rw-rw-rw-   0        0        0    39633 2024-03-24 15:25:24.000000 gskChat-1.0.8/gskChat/Provider/needs_auth/__pycache__/OpenaiChat.cpython-312.pyc
--rw-rw-rw-   0        0        0     5188 2024-03-24 15:25:24.000000 gskChat-1.0.8/gskChat/Provider/needs_auth/__pycache__/Poe.cpython-312.pyc
--rw-rw-rw-   0        0        0     2349 2024-03-24 15:25:24.000000 gskChat-1.0.8/gskChat/Provider/needs_auth/__pycache__/Raycast.cpython-312.pyc
--rw-rw-rw-   0        0        0     6707 2024-03-24 15:25:24.000000 gskChat-1.0.8/gskChat/Provider/needs_auth/__pycache__/Theb.cpython-312.pyc
--rw-rw-rw-   0        0        0     3305 2024-03-24 15:25:24.000000 gskChat-1.0.8/gskChat/Provider/needs_auth/__pycache__/ThebApi.cpython-312.pyc
--rw-rw-rw-   0        0        0      429 2024-03-24 15:25:24.000000 gskChat-1.0.8/gskChat/Provider/needs_auth/__pycache__/__init__.cpython-312.pyc
-drwxrwxrwx   0        0        0        0 2024-03-25 09:32:27.573669 gskChat-1.0.8/gskChat/Provider/not_working/
--rw-rw-rw-   0        0        0     3106 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/Provider/not_working/AItianhu.py
--rw-rw-rw-   0        0        0     1432 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/Provider/not_working/Bestim.py
--rw-rw-rw-   0        0        0     4546 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/Provider/not_working/ChatBase.py
--rw-rw-rw-   0        0        0     2863 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/Provider/not_working/ChatgptDemo.py
--rw-rw-rw-   0        0        0     2062 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/Provider/not_working/ChatgptDemoAi.py
--rw-rw-rw-   0        0        0     3056 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/Provider/not_working/ChatgptLogin.py
--rw-rw-rw-   0        0        0     2245 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/Provider/not_working/Chatxyz.py
--rw-rw-rw-   0        0        0     2243 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/Provider/not_working/Gpt6.py
--rw-rw-rw-   0        0        0     1033 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/Provider/not_working/GptChatly.py
--rw-rw-rw-   0        0        0     3529 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/Provider/not_working/GptForLove.py
--rw-rw-rw-   0        0        0     2480 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/Provider/not_working/GptGo.py
--rw-rw-rw-   0        0        0     2061 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/Provider/not_working/GptGod.py
--rw-rw-rw-   0        0        0     2093 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/Provider/not_working/OnlineGpt.py
--rw-rw-rw-   0        0        0      498 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/Provider/not_working/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-25 09:32:27.586635 gskChat-1.0.8/gskChat/Provider/not_working/__pycache__/
--rw-rw-rw-   0        0        0     3828 2024-03-24 15:25:24.000000 gskChat-1.0.8/gskChat/Provider/not_working/__pycache__/AItianhu.cpython-312.pyc
--rw-rw-rw-   0        0        0     2150 2024-03-24 15:25:24.000000 gskChat-1.0.8/gskChat/Provider/not_working/__pycache__/Bestim.cpython-312.pyc
--rw-rw-rw-   0        0        0     5577 2024-03-24 15:25:24.000000 gskChat-1.0.8/gskChat/Provider/not_working/__pycache__/ChatBase.cpython-312.pyc
--rw-rw-rw-   0        0        0     4629 2024-03-24 15:25:24.000000 gskChat-1.0.8/gskChat/Provider/not_working/__pycache__/ChatgptDemo.cpython-312.pyc
--rw-rw-rw-   0        0        0     3031 2024-03-24 15:25:24.000000 gskChat-1.0.8/gskChat/Provider/not_working/__pycache__/ChatgptDemoAi.cpython-312.pyc
--rw-rw-rw-   0        0        0     4835 2024-03-24 15:25:24.000000 gskChat-1.0.8/gskChat/Provider/not_working/__pycache__/ChatgptLogin.cpython-312.pyc
--rw-rw-rw-   0        0        0     3079 2024-03-24 15:25:24.000000 gskChat-1.0.8/gskChat/Provider/not_working/__pycache__/Chatxyz.cpython-312.pyc
--rw-rw-rw-   0        0        0     3251 2024-03-24 15:25:24.000000 gskChat-1.0.8/gskChat/Provider/not_working/__pycache__/Gpt6.cpython-312.pyc
--rw-rw-rw-   0        0        0     1724 2024-03-24 15:25:24.000000 gskChat-1.0.8/gskChat/Provider/not_working/__pycache__/GptChatly.cpython-312.pyc
--rw-rw-rw-   0        0        0     4841 2024-03-24 15:25:24.000000 gskChat-1.0.8/gskChat/Provider/not_working/__pycache__/GptForLove.cpython-312.pyc
--rw-rw-rw-   0        0        0     3729 2024-03-24 15:25:24.000000 gskChat-1.0.8/gskChat/Provider/not_working/__pycache__/GptGo.cpython-312.pyc
--rw-rw-rw-   0        0        0     3028 2024-03-24 15:25:24.000000 gskChat-1.0.8/gskChat/Provider/not_working/__pycache__/GptGod.cpython-312.pyc
--rw-rw-rw-   0        0        0     3024 2024-03-24 15:25:24.000000 gskChat-1.0.8/gskChat/Provider/not_working/__pycache__/OnlineGpt.cpython-312.pyc
--rw-rw-rw-   0        0        0      632 2024-03-24 15:25:24.000000 gskChat-1.0.8/gskChat/Provider/not_working/__pycache__/__init__.cpython-312.pyc
-drwxrwxrwx   0        0        0        0 2024-03-25 09:32:27.594611 gskChat-1.0.8/gskChat/Provider/npm/
-drwxrwxrwx   0        0        0        0 2024-03-25 09:32:27.598603 gskChat-1.0.8/gskChat/Provider/npm/node_modules/
--rw-rw-rw-   0        0        0      346 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/Provider/npm/node_modules/.package-lock.json
-drwxrwxrwx   0        0        0        0 2024-03-25 09:32:27.628052 gskChat-1.0.8/gskChat/Provider/npm/node_modules/crypto-js/
--rw-rw-rw-   0        0        0     6449 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/Provider/npm/node_modules/crypto-js/README.md
--rw-rw-rw-   0        0        0   219092 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/Provider/npm/node_modules/crypto-js/crypto-js.js
--rw-rw-rw-   0        0        0      698 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/Provider/npm/package-lock.json
--rw-rw-rw-   0        0        0       54 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/Provider/npm/package.json
-drwxrwxrwx   0        0        0        0 2024-03-25 09:32:27.633035 gskChat-1.0.8/gskChat/Provider/selenium/
--rw-rw-rw-   0        0        0     3839 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/Provider/selenium/AItianhuSpace.py
--rw-rw-rw-   0        0        0     2859 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/Provider/selenium/Bard.py
--rw-rw-rw-   0        0        0     2250 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/Provider/selenium/MyShell.py
--rw-rw-rw-   0        0        0     3681 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/Provider/selenium/PerplexityAi.py
--rw-rw-rw-   0        0        0     3655 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/Provider/selenium/Phind.py
--rw-rw-rw-   0        0        0     2678 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/Provider/selenium/TalkAi.py
--rw-rw-rw-   0        0        0      183 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/Provider/selenium/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-25 09:32:27.640015 gskChat-1.0.8/gskChat/Provider/selenium/__pycache__/
--rw-rw-rw-   0        0        0     4847 2024-03-24 15:25:24.000000 gskChat-1.0.8/gskChat/Provider/selenium/__pycache__/AItianhuSpace.cpython-312.pyc
--rw-rw-rw-   0        0        0     3759 2024-03-24 15:25:24.000000 gskChat-1.0.8/gskChat/Provider/selenium/__pycache__/Bard.cpython-312.pyc
--rw-rw-rw-   0        0        0     2914 2024-03-24 15:25:24.000000 gskChat-1.0.8/gskChat/Provider/selenium/__pycache__/MyShell.cpython-312.pyc
--rw-rw-rw-   0        0        0     4525 2024-03-24 15:25:24.000000 gskChat-1.0.8/gskChat/Provider/selenium/__pycache__/PerplexityAi.cpython-312.pyc
--rw-rw-rw-   0        0        0     4649 2024-03-24 15:25:24.000000 gskChat-1.0.8/gskChat/Provider/selenium/__pycache__/Phind.cpython-312.pyc
--rw-rw-rw-   0        0        0     3407 2024-03-24 15:25:24.000000 gskChat-1.0.8/gskChat/Provider/selenium/__pycache__/TalkAi.cpython-312.pyc
--rw-rw-rw-   0        0        0      400 2024-03-24 15:25:24.000000 gskChat-1.0.8/gskChat/Provider/selenium/__pycache__/__init__.cpython-312.pyc
-drwxrwxrwx   0        0        0        0 2024-03-25 09:32:27.643007 gskChat-1.0.8/gskChat/Provider/unfinished/
--rw-rw-rw-   0        0        0     2260 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/Provider/unfinished/AiChatting.py
--rw-rw-rw-   0        0        0     2441 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/Provider/unfinished/ChatAiGpt.py
--rw-rw-rw-   0        0        0     1450 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/Provider/unfinished/Komo.py
--rw-rw-rw-   0        0        0     3298 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/Provider/unfinished/MikuChat.py
--rw-rw-rw-   0        0        0      142 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/Provider/unfinished/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-25 09:32:27.647994 gskChat-1.0.8/gskChat/Provider/unfinished/__pycache__/
--rw-rw-rw-   0        0        0     3349 2024-03-24 15:25:24.000000 gskChat-1.0.8/gskChat/Provider/unfinished/__pycache__/AiChatting.cpython-312.pyc
--rw-rw-rw-   0        0        0     3656 2024-03-24 15:25:24.000000 gskChat-1.0.8/gskChat/Provider/unfinished/__pycache__/ChatAiGpt.cpython-312.pyc
--rw-rw-rw-   0        0        0     2378 2024-03-24 15:25:24.000000 gskChat-1.0.8/gskChat/Provider/unfinished/__pycache__/Komo.cpython-312.pyc
--rw-rw-rw-   0        0        0     5497 2024-03-24 15:25:24.000000 gskChat-1.0.8/gskChat/Provider/unfinished/__pycache__/MikuChat.cpython-312.pyc
--rw-rw-rw-   0        0        0      338 2024-03-24 15:25:24.000000 gskChat-1.0.8/gskChat/Provider/unfinished/__pycache__/__init__.cpython-312.pyc
--rw-rw-rw-   0        0        0    10959 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-25 09:32:27.657969 gskChat-1.0.8/gskChat/__pycache__/
--rw-rw-rw-   0        0        0    12330 2024-03-24 15:25:24.000000 gskChat-1.0.8/gskChat/__pycache__/__init__.cpython-312.pyc
--rw-rw-rw-   0        0        0     2461 2024-03-24 15:25:24.000000 gskChat-1.0.8/gskChat/__pycache__/cli.cpython-312.pyc
--rw-rw-rw-   0        0        0    11637 2024-03-24 15:25:24.000000 gskChat-1.0.8/gskChat/__pycache__/client.cpython-312.pyc
--rw-rw-rw-   0        0        0     4537 2024-03-24 15:25:24.000000 gskChat-1.0.8/gskChat/__pycache__/cookies.cpython-312.pyc
--rw-rw-rw-   0        0        0      478 2024-03-24 15:25:24.000000 gskChat-1.0.8/gskChat/__pycache__/debug.cpython-312.pyc
--rw-rw-rw-   0        0        0     2492 2024-03-24 15:25:24.000000 gskChat-1.0.8/gskChat/__pycache__/errors.cpython-312.pyc
--rw-rw-rw-   0        0        0    11732 2024-03-24 15:25:24.000000 gskChat-1.0.8/gskChat/__pycache__/image.cpython-312.pyc
--rw-rw-rw-   0        0        0     6305 2024-03-24 15:25:24.000000 gskChat-1.0.8/gskChat/__pycache__/models.cpython-312.pyc
--rw-rw-rw-   0        0        0     5533 2024-03-24 15:25:24.000000 gskChat-1.0.8/gskChat/__pycache__/stubs.cpython-312.pyc
--rw-rw-rw-   0        0        0     1152 2024-03-24 15:25:24.000000 gskChat-1.0.8/gskChat/__pycache__/typing.cpython-312.pyc
--rw-rw-rw-   0        0        0     5221 2024-03-24 15:25:24.000000 gskChat-1.0.8/gskChat/__pycache__/version.cpython-312.pyc
--rw-rw-rw-   0        0        0    12909 2024-03-24 15:25:24.000000 gskChat-1.0.8/gskChat/__pycache__/webdriver.cpython-312.pyc
-drwxrwxrwx   0        0        0        0 2024-03-25 09:32:27.660961 gskChat-1.0.8/gskChat/api/
--rw-rw-rw-   0        0        0     5168 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/api/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-25 09:32:27.664949 gskChat-1.0.8/gskChat/api/__pycache__/
--rw-rw-rw-   0        0        0     9054 2024-03-24 15:25:24.000000 gskChat-1.0.8/gskChat/api/__pycache__/__init__.cpython-312.pyc
--rw-rw-rw-   0        0        0     2317 2024-03-24 15:25:24.000000 gskChat-1.0.8/gskChat/api/__pycache__/_logging.cpython-312.pyc
--rw-rw-rw-   0        0        0      195 2024-03-24 15:25:24.000000 gskChat-1.0.8/gskChat/api/__pycache__/_tokenizer.cpython-312.pyc
--rw-rw-rw-   0        0        0      639 2024-03-24 15:25:24.000000 gskChat-1.0.8/gskChat/api/__pycache__/run.cpython-312.pyc
--rw-rw-rw-   0        0        0      893 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/api/_logging.py
--rw-rw-rw-   0        0        0      286 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/api/_tokenizer.py
--rw-rw-rw-   0        0        0      201 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/api/run.py
--rw-rw-rw-   0        0        0     1318 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/cli.py
--rw-rw-rw-   0        0        0     8568 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/client.py
--rw-rw-rw-   0        0        0     3406 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/cookies.py
--rw-rw-rw-   0        0        0      169 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/debug.py
--rw-rw-rw-   0        0        0      712 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/errors.py
-drwxrwxrwx   0        0        0        0 2024-03-25 09:32:27.666944 gskChat-1.0.8/gskChat/gui/
--rw-rw-rw-   0        0        0     1567 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/gui/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-25 09:32:27.669936 gskChat-1.0.8/gskChat/gui/__pycache__/
--rw-rw-rw-   0        0        0     2290 2024-03-24 15:25:24.000000 gskChat-1.0.8/gskChat/gui/__pycache__/__init__.cpython-312.pyc
--rw-rw-rw-   0        0        0     1249 2024-03-24 15:25:24.000000 gskChat-1.0.8/gskChat/gui/__pycache__/run.cpython-312.pyc
--rw-rw-rw-   0        0        0     2080 2024-03-24 15:25:24.000000 gskChat-1.0.8/gskChat/gui/__pycache__/webview.cpython-312.pyc
-drwxrwxrwx   0        0        0        0 2024-03-25 09:32:27.670933 gskChat-1.0.8/gskChat/gui/client/
--rw-rw-rw-   0        0        0        0 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/gui/client/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-25 09:32:27.671930 gskChat-1.0.8/gskChat/gui/client/__pycache__/
--rw-rw-rw-   0        0        0      200 2024-03-24 15:25:24.000000 gskChat-1.0.8/gskChat/gui/client/__pycache__/__init__.cpython-312.pyc
--rw-rw-rw-   0        0        0    25843 2024-03-25 09:31:03.000000 gskChat-1.0.8/gskChat/gui/client/index.html
-drwxrwxrwx   0        0        0        0 2024-03-25 09:32:27.672928 gskChat-1.0.8/gskChat/gui/client/static/
--rw-rw-rw-   0        0        0        0 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/gui/client/static/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-25 09:32:27.672928 gskChat-1.0.8/gskChat/gui/client/static/__pycache__/
--rw-rw-rw-   0        0        0      207 2024-03-24 15:25:24.000000 gskChat-1.0.8/gskChat/gui/client/static/__pycache__/__init__.cpython-312.pyc
-drwxrwxrwx   0        0        0        0 2024-03-25 09:32:27.674924 gskChat-1.0.8/gskChat/gui/client/static/css/
--rw-rw-rw-   0        0        0        0 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/gui/client/static/css/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-25 09:32:27.675920 gskChat-1.0.8/gskChat/gui/client/static/css/__pycache__/
--rw-rw-rw-   0        0        0      211 2024-03-24 15:25:24.000000 gskChat-1.0.8/gskChat/gui/client/static/css/__pycache__/__init__.cpython-312.pyc
--rw-rw-rw-   0        0        0    26422 2024-03-25 09:31:02.000000 gskChat-1.0.8/gskChat/gui/client/static/css/style.css
-drwxrwxrwx   0        0        0        0 2024-03-25 09:32:27.745099 gskChat-1.0.8/gskChat/gui/client/static/img/
--rw-rw-rw-   0        0        0     4286 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/gui/client/static/img/1.png
--rw-rw-rw-   0        0        0        0 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/gui/client/static/img/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-25 09:32:27.746092 gskChat-1.0.8/gskChat/gui/client/static/img/__pycache__/
--rw-rw-rw-   0        0        0      211 2024-03-24 15:25:24.000000 gskChat-1.0.8/gskChat/gui/client/static/img/__pycache__/__init__.cpython-312.pyc
--rw-rw-rw-   0        0        0     8908 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/gui/client/static/img/android-chrome-192x192.png
--rw-rw-rw-   0        0        0    17626 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/gui/client/static/img/android-chrome-512x512.png
--rw-rw-rw-   0        0        0     7984 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/gui/client/static/img/apple-touch-icon.png
--rw-rw-rw-   0        0        0     2258 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/gui/client/static/img/content.png
-drwxrwxrwx   0        0        0        0 2024-03-25 09:32:27.747089 gskChat-1.0.8/gskChat/gui/client/static/img/cursor/
--rw-rw-rw-   0        0        0        0 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/gui/client/static/img/cursor/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-25 09:32:27.748087 gskChat-1.0.8/gskChat/gui/client/static/img/cursor/__pycache__/
--rw-rw-rw-   0        0        0      218 2024-03-24 15:25:24.000000 gskChat-1.0.8/gskChat/gui/client/static/img/cursor/__pycache__/__init__.cpython-312.pyc
--rw-rw-rw-   0        0        0      721 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/gui/client/static/img/favicon-16x16.png
--rw-rw-rw-   0        0        0      499 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/gui/client/static/img/favicon-16x162.png
--rw-rw-rw-   0        0        0     4286 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/gui/client/static/img/favicon-32x32.png
--rw-rw-rw-   0        0        0   501120 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/gui/client/static/img/gpt.png
--rw-rw-rw-   0        0        0     2885 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/gui/client/static/img/gpt1.png
--rw-rw-rw-   0        0        0     2551 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/gui/client/static/img/graphic-designer.png
--rw-rw-rw-   0        0        0  2853419 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/gui/client/static/img/loading-1.gif
--rw-rw-rw-   0        0        0   251420 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/gui/client/static/img/loading-101.gif
--rw-rw-rw-   0        0        0   162448 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/gui/client/static/img/programmer.jpg
--rw-rw-rw-   0        0        0     1783 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/gui/client/static/img/programmer.png
--rw-rw-rw-   0        0        0      447 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/gui/client/static/img/site.webmanifest
--rw-rw-rw-   0        0        0   200333 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/gui/client/static/img/teacher.jpg
--rw-rw-rw-   0        0        0    23088 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/gui/client/static/img/telegram.png
--rw-rw-rw-   0        0        0   175178 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/gui/client/static/img/user.png
--rw-rw-rw-   0        0        0   117644 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/gui/client/static/img/write.jpg
-drwxrwxrwx   0        0        0        0 2024-03-25 09:32:27.788984 gskChat-1.0.8/gskChat/gui/client/static/js/
--rw-rw-rw-   0        0        0        0 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/gui/client/static/js/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-25 09:32:27.789975 gskChat-1.0.8/gskChat/gui/client/static/js/__pycache__/
--rw-rw-rw-   0        0        0      210 2024-03-24 15:25:24.000000 gskChat-1.0.8/gskChat/gui/client/static/js/__pycache__/__init__.cpython-312.pyc
--rw-rw-rw-   0        0        0    33901 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/gui/client/static/js/chat.v1.js
--rw-rw-rw-   0        0        0   118841 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/gui/client/static/js/highlight.min.js
--rw-rw-rw-   0        0        0     1083 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/gui/client/static/js/highlightjs-copy.min.js
--rw-rw-rw-   0        0        0    10865 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/gui/client/static/js/icons.js
--rw-rw-rw-   0        0        0      615 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/gui/run.py
-drwxrwxrwx   0        0        0        0 2024-03-25 09:32:27.794963 gskChat-1.0.8/gskChat/gui/server/
--rw-rw-rw-   0        0        0        0 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/gui/server/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-25 09:32:27.801944 gskChat-1.0.8/gskChat/gui/server/__pycache__/
--rw-rw-rw-   0        0        0      200 2024-03-24 15:25:24.000000 gskChat-1.0.8/gskChat/gui/server/__pycache__/__init__.cpython-312.pyc
--rw-rw-rw-   0        0        0     3366 2024-03-24 15:25:24.000000 gskChat-1.0.8/gskChat/gui/server/__pycache__/android_gallery.cpython-312.pyc
--rw-rw-rw-   0        0        0    12282 2024-03-24 15:25:24.000000 gskChat-1.0.8/gskChat/gui/server/__pycache__/api.cpython-312.pyc
--rw-rw-rw-   0        0        0      577 2024-03-24 15:25:24.000000 gskChat-1.0.8/gskChat/gui/server/__pycache__/app.cpython-312.pyc
--rw-rw-rw-   0        0        0     4568 2024-03-24 15:25:24.000000 gskChat-1.0.8/gskChat/gui/server/__pycache__/backend.cpython-312.pyc
--rw-rw-rw-   0        0        0    14765 2024-03-24 15:25:24.000000 gskChat-1.0.8/gskChat/gui/server/__pycache__/config.cpython-312.pyc
--rw-rw-rw-   0        0        0     7883 2024-03-24 15:25:24.000000 gskChat-1.0.8/gskChat/gui/server/__pycache__/internet.cpython-312.pyc
--rw-rw-rw-   0        0        0     1513 2024-03-24 15:25:24.000000 gskChat-1.0.8/gskChat/gui/server/__pycache__/website.cpython-312.pyc
--rw-rw-rw-   0        0        0     2470 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/gui/server/android_gallery.py
--rw-rw-rw-   0        0        0     9422 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/gui/server/api.py
--rw-rw-rw-   0        0        0      271 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/gui/server/app.py
--rw-rw-rw-   0        0        0     3681 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/gui/server/backend.py
--rw-rw-rw-   0        0        0    15354 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/gui/server/config.py
--rw-rw-rw-   0        0        0     4918 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/gui/server/internet.py
--rw-rw-rw-   0        0        0      839 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/gui/server/website.py
--rw-rw-rw-   0        0        0     1200 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/gui/webview.py
--rw-rw-rw-   0        0        0     8399 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/image.py
-drwxrwxrwx   0        0        0        0 2024-03-25 09:32:27.804940 gskChat-1.0.8/gskChat/local/
--rw-rw-rw-   0        0        0     1405 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/local/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-25 09:32:27.806936 gskChat-1.0.8/gskChat/local/__pycache__/
--rw-rw-rw-   0        0        0     2679 2024-03-24 15:25:24.000000 gskChat-1.0.8/gskChat/local/__pycache__/__init__.cpython-312.pyc
--rw-rw-rw-   0        0        0     3047 2024-03-24 15:25:24.000000 gskChat-1.0.8/gskChat/local/__pycache__/_engine.cpython-312.pyc
--rw-rw-rw-   0        0        0     2179 2024-03-24 15:25:24.000000 gskChat-1.0.8/gskChat/local/__pycache__/_models.cpython-312.pyc
--rw-rw-rw-   0        0        0     1832 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/local/_engine.py
--rw-rw-rw-   0        0        0     2959 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/local/_models.py
--rw-rw-rw-   0        0        0     7633 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/models.py
-drwxrwxrwx   0        0        0        0 2024-03-25 09:32:27.810926 gskChat-1.0.8/gskChat/providers/
--rw-rw-rw-   0        0        0        0 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/providers/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-25 09:32:27.816908 gskChat-1.0.8/gskChat/providers/__pycache__/
--rw-rw-rw-   0        0        0      199 2024-03-24 15:25:24.000000 gskChat-1.0.8/gskChat/providers/__pycache__/__init__.cpython-312.pyc
--rw-rw-rw-   0        0        0    13248 2024-03-24 15:25:24.000000 gskChat-1.0.8/gskChat/providers/__pycache__/base_provider.cpython-312.pyc
--rw-rw-rw-   0        0        0     7555 2024-03-24 15:25:24.000000 gskChat-1.0.8/gskChat/providers/__pycache__/create_images.cpython-312.pyc
--rw-rw-rw-   0        0        0     2745 2024-03-24 15:25:24.000000 gskChat-1.0.8/gskChat/providers/__pycache__/helper.cpython-312.pyc
--rw-rw-rw-   0        0        0     9044 2024-03-24 15:25:24.000000 gskChat-1.0.8/gskChat/providers/__pycache__/retry_provider.cpython-312.pyc
--rw-rw-rw-   0        0        0     4203 2024-03-24 15:25:24.000000 gskChat-1.0.8/gskChat/providers/__pycache__/types.cpython-312.pyc
--rw-rw-rw-   0        0        0     9260 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/providers/base_provider.py
--rw-rw-rw-   0        0        0     6594 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/providers/create_images.py
--rw-rw-rw-   0        0        0     1528 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/providers/helper.py
--rw-rw-rw-   0        0        0     6869 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/providers/retry_provider.py
--rw-rw-rw-   0        0        0     3083 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/providers/types.py
-drwxrwxrwx   0        0        0        0 2024-03-25 09:32:27.819409 gskChat-1.0.8/gskChat/requests/
--rw-rw-rw-   0        0        0     3959 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/requests/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-25 09:32:27.823403 gskChat-1.0.8/gskChat/requests/__pycache__/
--rw-rw-rw-   0        0        0     4981 2024-03-24 15:25:24.000000 gskChat-1.0.8/gskChat/requests/__pycache__/__init__.cpython-312.pyc
--rw-rw-rw-   0        0        0     3226 2024-03-24 15:25:24.000000 gskChat-1.0.8/gskChat/requests/__pycache__/aiohttp.cpython-312.pyc
--rw-rw-rw-   0        0        0     5284 2024-03-24 15:25:24.000000 gskChat-1.0.8/gskChat/requests/__pycache__/curl_cffi.cpython-312.pyc
--rw-rw-rw-   0        0        0     1415 2024-03-24 15:25:24.000000 gskChat-1.0.8/gskChat/requests/__pycache__/defaults.cpython-312.pyc
--rw-rw-rw-   0        0        0     2638 2024-03-24 15:25:24.000000 gskChat-1.0.8/gskChat/requests/__pycache__/raise_for_status.cpython-312.pyc
--rw-rw-rw-   0        0        0     1775 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/requests/aiohttp.py
--rw-rw-rw-   0        0        0     3016 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/requests/curl_cffi.py
--rw-rw-rw-   0        0        0     1091 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/requests/defaults.py
--rw-rw-rw-   0        0        0     1625 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/requests/raise_for_status.py
--rw-rw-rw-   0        0        0     2938 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/stubs.py
--rw-rw-rw-   0        0        0      875 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/typing.py
--rw-rw-rw-   0        0        0     3821 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/version.py
--rw-rw-rw-   0        0        0     9953 2024-03-24 15:25:23.000000 gskChat-1.0.8/gskChat/webdriver.py
-drwxrwxrwx   0        0        0        0 2024-03-25 09:32:27.824400 gskChat-1.0.8/gskChat.egg-info/
--rw-rw-rw-   0        0        0     2874 2024-03-25 09:32:27.000000 gskChat-1.0.8/gskChat.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    15731 2024-03-25 09:32:27.000000 gskChat-1.0.8/gskChat.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-25 09:32:27.000000 gskChat-1.0.8/gskChat.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2024-03-25 09:32:27.000000 gskChat-1.0.8/gskChat.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      621 2024-03-25 09:32:27.000000 gskChat-1.0.8/gskChat.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-03-25 09:32:27.000000 gskChat-1.0.8/gskChat.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-25 09:32:27.830383 gskChat-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0     3200 2024-03-25 09:32:13.000000 gskChat-1.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-07 13:59:21.048525 gskChat-1.0.9/
+-rw-rw-rw-   0        0        0      224 2024-03-24 15:15:13.000000 gskChat-1.0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     2874 2024-04-07 13:59:21.048525 gskChat-1.0.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-07 13:59:20.490163 gskChat-1.0.9/gskChat/
+drwxrwxrwx   0        0        0        0 2024-04-07 13:59:20.530545 gskChat-1.0.9/gskChat/Provider/
+-rw-rw-rw-   0        0        0     1607 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/Aura.py
+-rw-rw-rw-   0        0        0    20640 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/Bing.py
+-rw-rw-rw-   0        0        0     2193 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/BingCreateImages.py
+-rw-rw-rw-   0        0        0     2508 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/ChatForAi.py
+-rw-rw-rw-   0        0        0     2653 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/Chatgpt4Online.py
+-rw-rw-rw-   0        0        0     3608 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/ChatgptAi.py
+-rw-rw-rw-   0        0        0     2855 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/ChatgptFree.py
+-rw-rw-rw-   0        0        0     2503 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/ChatgptNext.py
+-rw-rw-rw-   0        0        0     4278 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/ChatgptX.py
+-rw-rw-rw-   0        0        0     3526 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/DeepInfra.py
+-rw-rw-rw-   0        0        0     3196 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/FlowGpt.py
+-rw-rw-rw-   0        0        0     2530 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/FreeChatgpt.py
+-rw-rw-rw-   0        0        0     1791 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/FreeGpt.py
+-rw-rw-rw-   0        0        0     3937 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/GeminiPro.py
+-rw-rw-rw-   0        0        0     2557 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/GeminiProChat.py
+-rw-rw-rw-   0        0        0     3926 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/GigaChat.py
+-rw-rw-rw-   0        0        0     2321 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/GptTalkRu.py
+-rw-rw-rw-   0        0        0     3615 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/HuggingChat.py
+-rw-rw-rw-   0        0        0     2940 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/HuggingFace.py
+-rw-rw-rw-   0        0        0     2485 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/Koala.py
+-rw-rw-rw-   0        0        0     5099 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/Liaobots.py
+-rw-rw-rw-   0        0        0     3105 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/Llama2.py
+-rw-rw-rw-   0        0        0     3951 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/PerplexityLabs.py
+-rw-rw-rw-   0        0        0     2355 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/Pi.py
+-rw-rw-rw-   0        0        0     4027 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/Vercel.py
+-rw-rw-rw-   0        0        0     7243 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/You.py
+-rw-rw-rw-   0        0        0     2047 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-07 13:59:20.563444 gskChat-1.0.9/gskChat/Provider/__pycache__/
+-rw-rw-rw-   0        0        0     2618 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/__pycache__/Aura.cpython-312.pyc
+-rw-rw-rw-   0        0        0    20847 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/__pycache__/Bing.cpython-312.pyc
+-rw-rw-rw-   0        0        0     3577 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/__pycache__/BingCreateImages.cpython-312.pyc
+-rw-rw-rw-   0        0        0     3774 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/__pycache__/ChatForAi.cpython-312.pyc
+-rw-rw-rw-   0        0        0     3889 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/__pycache__/Chatgpt4Online.cpython-312.pyc
+-rw-rw-rw-   0        0        0     4740 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/__pycache__/ChatgptAi.cpython-312.pyc
+-rw-rw-rw-   0        0        0     3951 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/__pycache__/ChatgptFree.cpython-312.pyc
+-rw-rw-rw-   0        0        0     3325 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/__pycache__/ChatgptNext.cpython-312.pyc
+-rw-rw-rw-   0        0        0     5386 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/__pycache__/ChatgptX.cpython-312.pyc
+-rw-rw-rw-   0        0        0     4547 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/__pycache__/DeepInfra.cpython-312.pyc
+-rw-rw-rw-   0        0        0     3912 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/__pycache__/FlowGpt.cpython-312.pyc
+-rw-rw-rw-   0        0        0     3552 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/__pycache__/FreeChatgpt.cpython-312.pyc
+-rw-rw-rw-   0        0        0     3089 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/__pycache__/FreeGpt.cpython-312.pyc
+-rw-rw-rw-   0        0        0     5017 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/__pycache__/GeminiPro.cpython-312.pyc
+-rw-rw-rw-   0        0        0     3887 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/__pycache__/GeminiProChat.cpython-312.pyc
+-rw-rw-rw-   0        0        0     5557 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/__pycache__/GigaChat.cpython-312.pyc
+-rw-rw-rw-   0        0        0     4066 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/__pycache__/GptTalkRu.cpython-312.pyc
+-rw-rw-rw-   0        0        0     5345 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/__pycache__/HuggingChat.cpython-312.pyc
+-rw-rw-rw-   0        0        0     4428 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/__pycache__/HuggingFace.cpython-312.pyc
+-rw-rw-rw-   0        0        0     3521 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/__pycache__/Koala.cpython-312.pyc
+-rw-rw-rw-   0        0        0     5673 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/__pycache__/Liaobots.cpython-312.pyc
+-rw-rw-rw-   0        0        0     4082 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/__pycache__/Llama2.cpython-312.pyc
+-rw-rw-rw-   0        0        0     5769 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/__pycache__/PerplexityLabs.cpython-312.pyc
+-rw-rw-rw-   0        0        0     3523 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/__pycache__/Pi.cpython-312.pyc
+-rw-rw-rw-   0        0        0     5112 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/__pycache__/Vercel.cpython-312.pyc
+-rw-rw-rw-   0        0        0     9701 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/__pycache__/You.cpython-312.pyc
+-rw-rw-rw-   0        0        0     2677 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/__pycache__/__init__.cpython-312.pyc
+-rw-rw-rw-   0        0        0      323 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/__pycache__/base_provider.cpython-312.pyc
+-rw-rw-rw-   0        0        0      333 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/__pycache__/helper.cpython-312.pyc
+-rw-rw-rw-   0        0        0       86 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/base_provider.py
+drwxrwxrwx   0        0        0        0 2024-04-07 13:59:20.566436 gskChat-1.0.9/gskChat/Provider/bing/
+-rw-rw-rw-   0        0        0        0 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/bing/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-07 13:59:20.570474 gskChat-1.0.9/gskChat/Provider/bing/__pycache__/
+-rw-rw-rw-   0        0        0      203 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/bing/__pycache__/__init__.cpython-312.pyc
+-rw-rw-rw-   0        0        0     5088 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/bing/__pycache__/conversation.cpython-312.pyc
+-rw-rw-rw-   0        0        0    10876 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/bing/__pycache__/create_images.cpython-312.pyc
+-rw-rw-rw-   0        0        0     6076 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/bing/__pycache__/upload_image.cpython-312.pyc
+-rw-rw-rw-   0        0        0     3468 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/bing/conversation.py
+-rw-rw-rw-   0        0        0     7597 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/bing/create_images.py
+-rw-rw-rw-   0        0        0     4746 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/bing/upload_image.py
+drwxrwxrwx   0        0        0        0 2024-04-07 13:59:20.602300 gskChat-1.0.9/gskChat/Provider/deprecated/
+-rw-rw-rw-   0        0        0     1397 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/deprecated/Acytoo.py
+-rw-rw-rw-   0        0        0     1669 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/deprecated/AiAsk.py
+-rw-rw-rw-   0        0        0     2196 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/deprecated/AiChatOnline.py
+-rw-rw-rw-   0        0        0     1148 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/deprecated/AiService.py
+-rw-rw-rw-   0        0        0     1396 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/deprecated/Aibn.py
+-rw-rw-rw-   0        0        0     2517 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/deprecated/Aichat.py
+-rw-rw-rw-   0        0        0     3358 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/deprecated/Ails.py
+-rw-rw-rw-   0        0        0     2952 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/deprecated/Aivvm.py
+-rw-rw-rw-   0        0        0     2807 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/deprecated/Berlin.py
+-rw-rw-rw-   0        0        0     1934 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/deprecated/ChatAnywhere.py
+-rw-rw-rw-   0        0        0     1303 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/deprecated/ChatgptDuo.py
+-rw-rw-rw-   0        0        0     1873 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/deprecated/CodeLinkAva.py
+-rw-rw-rw-   0        0        0     1356 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/deprecated/Cromicle.py
+-rw-rw-rw-   0        0        0     2498 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/deprecated/DfeHub.py
+-rw-rw-rw-   0        0        0     3398 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/deprecated/EasyChat.py
+-rw-rw-rw-   0        0        0     2755 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/deprecated/Equing.py
+-rw-rw-rw-   0        0        0     4018 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/deprecated/FakeGpt.py
+-rw-rw-rw-   0        0        0     2929 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/deprecated/FastGpt.py
+-rw-rw-rw-   0        0        0     1282 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/deprecated/Forefront.py
+-rw-rw-rw-   0        0        0     3552 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/deprecated/GPTalk.py
+-rw-rw-rw-   0        0        0     2658 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/deprecated/GeekGpt.py
+-rw-rw-rw-   0        0        0     2515 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/deprecated/GetGpt.py
+-rw-rw-rw-   0        0        0     2925 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/deprecated/H2o.py
+-rw-rw-rw-   0        0        0     2674 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/deprecated/Hashnode.py
+-rw-rw-rw-   0        0        0     1700 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/deprecated/Lockchat.py
+-rw-rw-rw-   0        0        0     5050 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/deprecated/Myshell.py
+-rw-rw-rw-   0        0        0     2500 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/deprecated/NoowAi.py
+-rw-rw-rw-   0        0        0     2287 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/deprecated/Opchatgpts.py
+-rw-rw-rw-   0        0        0     5353 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/deprecated/Phind.py
+-rw-rw-rw-   0        0        0     2077 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/deprecated/V50.py
+-rw-rw-rw-   0        0        0    12167 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/deprecated/Vercel.py
+-rw-rw-rw-   0        0        0     1964 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/deprecated/Vitalentum.py
+-rw-rw-rw-   0        0        0     3415 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/deprecated/VoiGpt.py
+-rw-rw-rw-   0        0        0     2464 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/deprecated/Wewordle.py
+-rw-rw-rw-   0        0        0     2020 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/deprecated/Wuguokai.py
+-rw-rw-rw-   0        0        0     1976 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/deprecated/Ylokh.py
+-rw-rw-rw-   0        0        0     1922 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/deprecated/Yqcloud.py
+-rw-rw-rw-   0        0        0     1194 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/deprecated/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-07 13:59:20.644472 gskChat-1.0.9/gskChat/Provider/deprecated/__pycache__/
+-rw-rw-rw-   0        0        0     2523 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/deprecated/__pycache__/Acytoo.cpython-312.pyc
+-rw-rw-rw-   0        0        0     2705 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/deprecated/__pycache__/AiAsk.cpython-312.pyc
+-rw-rw-rw-   0        0        0     3107 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/deprecated/__pycache__/AiChatOnline.cpython-312.pyc
+-rw-rw-rw-   0        0        0     1976 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/deprecated/__pycache__/AiService.cpython-312.pyc
+-rw-rw-rw-   0        0        0     2702 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/deprecated/__pycache__/Aibn.cpython-312.pyc
+-rw-rw-rw-   0        0        0     3337 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/deprecated/__pycache__/Aichat.cpython-312.pyc
+-rw-rw-rw-   0        0        0     4946 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/deprecated/__pycache__/Ails.cpython-312.pyc
+-rw-rw-rw-   0        0        0     3266 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/deprecated/__pycache__/Aivvm.cpython-312.pyc
+-rw-rw-rw-   0        0        0     3969 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/deprecated/__pycache__/Berlin.cpython-312.pyc
+-rw-rw-rw-   0        0        0     2911 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/deprecated/__pycache__/ChatAnywhere.cpython-312.pyc
+-rw-rw-rw-   0        0        0     2243 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/deprecated/__pycache__/ChatgptDuo.cpython-312.pyc
+-rw-rw-rw-   0        0        0     2831 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/deprecated/__pycache__/CodeLinkAva.cpython-312.pyc
+-rw-rw-rw-   0        0        0     2812 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/deprecated/__pycache__/Cromicle.cpython-312.pyc
+-rw-rw-rw-   0        0        0     3098 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/deprecated/__pycache__/DfeHub.cpython-312.pyc
+-rw-rw-rw-   0        0        0     4043 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/deprecated/__pycache__/EasyChat.cpython-312.pyc
+-rw-rw-rw-   0        0        0     3381 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/deprecated/__pycache__/Equing.cpython-312.pyc
+-rw-rw-rw-   0        0        0     5651 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/deprecated/__pycache__/FakeGpt.cpython-312.pyc
+-rw-rw-rw-   0        0        0     3377 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/deprecated/__pycache__/FastGpt.cpython-312.pyc
+-rw-rw-rw-   0        0        0     1953 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/deprecated/__pycache__/Forefront.cpython-312.pyc
+-rw-rw-rw-   0        0        0     5271 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/deprecated/__pycache__/GPTalk.cpython-312.pyc
+-rw-rw-rw-   0        0        0     3197 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/deprecated/__pycache__/GeekGpt.cpython-312.pyc
+-rw-rw-rw-   0        0        0     2831 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/deprecated/__pycache__/GetGpt.cpython-312.pyc
+-rw-rw-rw-   0        0        0     4367 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/deprecated/__pycache__/H2o.cpython-312.pyc
+-rw-rw-rw-   0        0        0     4072 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/deprecated/__pycache__/Hashnode.cpython-312.pyc
+-rw-rw-rw-   0        0        0     2331 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/deprecated/__pycache__/Lockchat.cpython-312.pyc
+-rw-rw-rw-   0        0        0     7947 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/deprecated/__pycache__/Myshell.cpython-312.pyc
+-rw-rw-rw-   0        0        0     3339 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/deprecated/__pycache__/NoowAi.cpython-312.pyc
+-rw-rw-rw-   0        0        0     3166 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/deprecated/__pycache__/Opchatgpts.cpython-312.pyc
+-rw-rw-rw-   0        0        0     7793 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/deprecated/__pycache__/Phind.cpython-312.pyc
+-rw-rw-rw-   0        0        0     2607 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/deprecated/__pycache__/V50.cpython-312.pyc
+-rw-rw-rw-   0        0        0     8348 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/deprecated/__pycache__/Vercel.cpython-312.pyc
+-rw-rw-rw-   0        0        0     3117 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/deprecated/__pycache__/Vitalentum.cpython-312.pyc
+-rw-rw-rw-   0        0        0     3644 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/deprecated/__pycache__/VoiGpt.cpython-312.pyc
+-rw-rw-rw-   0        0        0     3606 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/deprecated/__pycache__/Wewordle.cpython-312.pyc
+-rw-rw-rw-   0        0        0     2702 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/deprecated/__pycache__/Wuguokai.cpython-312.pyc
+-rw-rw-rw-   0        0        0     3036 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/deprecated/__pycache__/Ylokh.cpython-312.pyc
+-rw-rw-rw-   0        0        0     3066 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/deprecated/__pycache__/Yqcloud.cpython-312.pyc
+-rw-rw-rw-   0        0        0     1269 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/deprecated/__pycache__/__init__.cpython-312.pyc
+drwxrwxrwx   0        0        0        0 2024-04-07 13:59:20.650520 gskChat-1.0.9/gskChat/Provider/gigachat_crt/
+-rw-rw-rw-   0        0        0     2056 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/gigachat_crt/russian_trusted_root_ca_pem.crt
+-rw-rw-rw-   0        0        0      111 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/helper.py
+drwxrwxrwx   0        0        0        0 2024-04-07 13:59:20.657503 gskChat-1.0.9/gskChat/Provider/needs_auth/
+-rw-rw-rw-   0        0        0     8145 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/needs_auth/Gemini.py
+-rw-rw-rw-   0        0        0     3309 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/needs_auth/OpenAssistant.py
+-rw-rw-rw-   0        0        0    30868 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/needs_auth/OpenaiChat.py
+-rw-rw-rw-   0        0        0     4289 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/needs_auth/Poe.py
+-rw-rw-rw-   0        0        0     1897 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/needs_auth/Raycast.py
+-rw-rw-rw-   0        0        0     5465 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/needs_auth/Theb.py
+-rw-rw-rw-   0        0        0     2655 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/needs_auth/ThebApi.py
+-rw-rw-rw-   0        0        0      245 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/needs_auth/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-07 13:59:20.666530 gskChat-1.0.9/gskChat/Provider/needs_auth/__pycache__/
+-rw-rw-rw-   0        0        0    12063 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/needs_auth/__pycache__/Gemini.cpython-312.pyc
+-rw-rw-rw-   0        0        0     4902 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/needs_auth/__pycache__/OpenAssistant.cpython-312.pyc
+-rw-rw-rw-   0        0        0    39633 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/needs_auth/__pycache__/OpenaiChat.cpython-312.pyc
+-rw-rw-rw-   0        0        0     5188 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/needs_auth/__pycache__/Poe.cpython-312.pyc
+-rw-rw-rw-   0        0        0     2349 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/needs_auth/__pycache__/Raycast.cpython-312.pyc
+-rw-rw-rw-   0        0        0     6707 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/needs_auth/__pycache__/Theb.cpython-312.pyc
+-rw-rw-rw-   0        0        0     3305 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/needs_auth/__pycache__/ThebApi.cpython-312.pyc
+-rw-rw-rw-   0        0        0      429 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/needs_auth/__pycache__/__init__.cpython-312.pyc
+drwxrwxrwx   0        0        0        0 2024-04-07 13:59:20.677914 gskChat-1.0.9/gskChat/Provider/not_working/
+-rw-rw-rw-   0        0        0     3106 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/not_working/AItianhu.py
+-rw-rw-rw-   0        0        0     1432 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/not_working/Bestim.py
+-rw-rw-rw-   0        0        0     4546 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/not_working/ChatBase.py
+-rw-rw-rw-   0        0        0     2863 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/not_working/ChatgptDemo.py
+-rw-rw-rw-   0        0        0     2062 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/not_working/ChatgptDemoAi.py
+-rw-rw-rw-   0        0        0     3056 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/not_working/ChatgptLogin.py
+-rw-rw-rw-   0        0        0     2245 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/not_working/Chatxyz.py
+-rw-rw-rw-   0        0        0     2243 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/not_working/Gpt6.py
+-rw-rw-rw-   0        0        0     1033 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/not_working/GptChatly.py
+-rw-rw-rw-   0        0        0     3529 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/not_working/GptForLove.py
+-rw-rw-rw-   0        0        0     2480 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/not_working/GptGo.py
+-rw-rw-rw-   0        0        0     2061 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/not_working/GptGod.py
+-rw-rw-rw-   0        0        0     2093 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/not_working/OnlineGpt.py
+-rw-rw-rw-   0        0        0      498 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/not_working/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-07 13:59:20.694478 gskChat-1.0.9/gskChat/Provider/not_working/__pycache__/
+-rw-rw-rw-   0        0        0     3828 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/not_working/__pycache__/AItianhu.cpython-312.pyc
+-rw-rw-rw-   0        0        0     2150 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/not_working/__pycache__/Bestim.cpython-312.pyc
+-rw-rw-rw-   0        0        0     5577 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/not_working/__pycache__/ChatBase.cpython-312.pyc
+-rw-rw-rw-   0        0        0     4629 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/not_working/__pycache__/ChatgptDemo.cpython-312.pyc
+-rw-rw-rw-   0        0        0     3031 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/not_working/__pycache__/ChatgptDemoAi.cpython-312.pyc
+-rw-rw-rw-   0        0        0     4835 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/not_working/__pycache__/ChatgptLogin.cpython-312.pyc
+-rw-rw-rw-   0        0        0     3079 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/not_working/__pycache__/Chatxyz.cpython-312.pyc
+-rw-rw-rw-   0        0        0     3251 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/not_working/__pycache__/Gpt6.cpython-312.pyc
+-rw-rw-rw-   0        0        0     1724 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/not_working/__pycache__/GptChatly.cpython-312.pyc
+-rw-rw-rw-   0        0        0     4841 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/not_working/__pycache__/GptForLove.cpython-312.pyc
+-rw-rw-rw-   0        0        0     3729 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/not_working/__pycache__/GptGo.cpython-312.pyc
+-rw-rw-rw-   0        0        0     3028 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/not_working/__pycache__/GptGod.cpython-312.pyc
+-rw-rw-rw-   0        0        0     3024 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/not_working/__pycache__/OnlineGpt.cpython-312.pyc
+-rw-rw-rw-   0        0        0      632 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/not_working/__pycache__/__init__.cpython-312.pyc
+drwxrwxrwx   0        0        0        0 2024-04-07 13:59:20.703535 gskChat-1.0.9/gskChat/Provider/npm/
+drwxrwxrwx   0        0        0        0 2024-04-07 13:59:20.707525 gskChat-1.0.9/gskChat/Provider/npm/node_modules/
+-rw-rw-rw-   0        0        0      346 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/npm/node_modules/.package-lock.json
+drwxrwxrwx   0        0        0        0 2024-04-07 13:59:20.741010 gskChat-1.0.9/gskChat/Provider/npm/node_modules/crypto-js/
+-rw-rw-rw-   0        0        0     6449 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/npm/node_modules/crypto-js/README.md
+-rw-rw-rw-   0        0        0   219092 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/npm/node_modules/crypto-js/crypto-js.js
+-rw-rw-rw-   0        0        0      698 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/npm/package-lock.json
+-rw-rw-rw-   0        0        0       54 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/npm/package.json
+drwxrwxrwx   0        0        0        0 2024-04-07 13:59:20.746996 gskChat-1.0.9/gskChat/Provider/selenium/
+-rw-rw-rw-   0        0        0     3839 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/selenium/AItianhuSpace.py
+-rw-rw-rw-   0        0        0     2859 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/selenium/Bard.py
+-rw-rw-rw-   0        0        0     2250 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/selenium/MyShell.py
+-rw-rw-rw-   0        0        0     3681 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/selenium/PerplexityAi.py
+-rw-rw-rw-   0        0        0     3655 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/selenium/Phind.py
+-rw-rw-rw-   0        0        0     2678 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/selenium/TalkAi.py
+-rw-rw-rw-   0        0        0      183 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/selenium/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-07 13:59:20.754918 gskChat-1.0.9/gskChat/Provider/selenium/__pycache__/
+-rw-rw-rw-   0        0        0     4847 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/selenium/__pycache__/AItianhuSpace.cpython-312.pyc
+-rw-rw-rw-   0        0        0     3759 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/selenium/__pycache__/Bard.cpython-312.pyc
+-rw-rw-rw-   0        0        0     2914 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/selenium/__pycache__/MyShell.cpython-312.pyc
+-rw-rw-rw-   0        0        0     4525 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/selenium/__pycache__/PerplexityAi.cpython-312.pyc
+-rw-rw-rw-   0        0        0     4649 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/selenium/__pycache__/Phind.cpython-312.pyc
+-rw-rw-rw-   0        0        0     3407 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/selenium/__pycache__/TalkAi.cpython-312.pyc
+-rw-rw-rw-   0        0        0      400 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/selenium/__pycache__/__init__.cpython-312.pyc
+drwxrwxrwx   0        0        0        0 2024-04-07 13:59:20.757910 gskChat-1.0.9/gskChat/Provider/unfinished/
+-rw-rw-rw-   0        0        0     2260 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/unfinished/AiChatting.py
+-rw-rw-rw-   0        0        0     2441 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/unfinished/ChatAiGpt.py
+-rw-rw-rw-   0        0        0     1450 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/unfinished/Komo.py
+-rw-rw-rw-   0        0        0     3298 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/unfinished/MikuChat.py
+-rw-rw-rw-   0        0        0      142 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/Provider/unfinished/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-07 13:59:20.764894 gskChat-1.0.9/gskChat/Provider/unfinished/__pycache__/
+-rw-rw-rw-   0        0        0     3349 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/unfinished/__pycache__/AiChatting.cpython-312.pyc
+-rw-rw-rw-   0        0        0     3656 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/unfinished/__pycache__/ChatAiGpt.cpython-312.pyc
+-rw-rw-rw-   0        0        0     2378 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/unfinished/__pycache__/Komo.cpython-312.pyc
+-rw-rw-rw-   0        0        0     5497 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/unfinished/__pycache__/MikuChat.cpython-312.pyc
+-rw-rw-rw-   0        0        0      338 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/Provider/unfinished/__pycache__/__init__.cpython-312.pyc
+-rw-rw-rw-   0        0        0    10959 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-07 13:59:20.779386 gskChat-1.0.9/gskChat/__pycache__/
+-rw-rw-rw-   0        0        0    12330 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/__pycache__/__init__.cpython-312.pyc
+-rw-rw-rw-   0        0        0     2461 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/__pycache__/cli.cpython-312.pyc
+-rw-rw-rw-   0        0        0    11637 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/__pycache__/client.cpython-312.pyc
+-rw-rw-rw-   0        0        0     4537 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/__pycache__/cookies.cpython-312.pyc
+-rw-rw-rw-   0        0        0      478 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/__pycache__/debug.cpython-312.pyc
+-rw-rw-rw-   0        0        0     2492 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/__pycache__/errors.cpython-312.pyc
+-rw-rw-rw-   0        0        0    11732 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/__pycache__/image.cpython-312.pyc
+-rw-rw-rw-   0        0        0     6305 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/__pycache__/models.cpython-312.pyc
+-rw-rw-rw-   0        0        0     5533 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/__pycache__/stubs.cpython-312.pyc
+-rw-rw-rw-   0        0        0     1152 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/__pycache__/typing.cpython-312.pyc
+-rw-rw-rw-   0        0        0     5221 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/__pycache__/version.cpython-312.pyc
+-rw-rw-rw-   0        0        0    12909 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/__pycache__/webdriver.cpython-312.pyc
+drwxrwxrwx   0        0        0        0 2024-04-07 13:59:20.782488 gskChat-1.0.9/gskChat/api/
+-rw-rw-rw-   0        0        0     5168 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/api/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-07 13:59:20.787474 gskChat-1.0.9/gskChat/api/__pycache__/
+-rw-rw-rw-   0        0        0     9054 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/api/__pycache__/__init__.cpython-312.pyc
+-rw-rw-rw-   0        0        0     2317 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/api/__pycache__/_logging.cpython-312.pyc
+-rw-rw-rw-   0        0        0      195 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/api/__pycache__/_tokenizer.cpython-312.pyc
+-rw-rw-rw-   0        0        0      639 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/api/__pycache__/run.cpython-312.pyc
+-rw-rw-rw-   0        0        0      893 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/api/_logging.py
+-rw-rw-rw-   0        0        0      286 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/api/_tokenizer.py
+-rw-rw-rw-   0        0        0      201 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/api/run.py
+-rw-rw-rw-   0        0        0     1318 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/cli.py
+-rw-rw-rw-   0        0        0     8568 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/client.py
+-rw-rw-rw-   0        0        0     3406 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/cookies.py
+-rw-rw-rw-   0        0        0      169 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/debug.py
+-rw-rw-rw-   0        0        0      712 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/errors.py
+drwxrwxrwx   0        0        0        0 2024-04-07 13:59:20.789470 gskChat-1.0.9/gskChat/gui/
+-rw-rw-rw-   0        0        0     1567 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/gui/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-07 13:59:20.792540 gskChat-1.0.9/gskChat/gui/__pycache__/
+-rw-rw-rw-   0        0        0     2290 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/gui/__pycache__/__init__.cpython-312.pyc
+-rw-rw-rw-   0        0        0     1249 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/gui/__pycache__/run.cpython-312.pyc
+-rw-rw-rw-   0        0        0     2080 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/gui/__pycache__/webview.cpython-312.pyc
+drwxrwxrwx   0        0        0        0 2024-04-07 13:59:20.860189 gskChat-1.0.9/gskChat/gui/client/
+-rw-rw-rw-   0        0        0        0 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/gui/client/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-07 13:59:20.861547 gskChat-1.0.9/gskChat/gui/client/__pycache__/
+-rw-rw-rw-   0        0        0      200 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/gui/client/__pycache__/__init__.cpython-312.pyc
+-rw-rw-rw-   0        0        0    25804 2024-04-07 13:04:16.000000 gskChat-1.0.9/gskChat/gui/client/index.html
+drwxrwxrwx   0        0        0        0 2024-04-07 13:59:20.861547 gskChat-1.0.9/gskChat/gui/client/static/
+-rw-rw-rw-   0        0        0        0 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/gui/client/static/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-07 13:59:20.862546 gskChat-1.0.9/gskChat/gui/client/static/__pycache__/
+-rw-rw-rw-   0        0        0      207 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/gui/client/static/__pycache__/__init__.cpython-312.pyc
+drwxrwxrwx   0        0        0        0 2024-04-07 13:59:20.864542 gskChat-1.0.9/gskChat/gui/client/static/css/
+-rw-rw-rw-   0        0        0        0 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/gui/client/static/css/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-07 13:59:20.865539 gskChat-1.0.9/gskChat/gui/client/static/css/__pycache__/
+-rw-rw-rw-   0        0        0      211 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/gui/client/static/css/__pycache__/__init__.cpython-312.pyc
+-rw-rw-rw-   0        0        0    26730 2024-04-07 13:57:33.000000 gskChat-1.0.9/gskChat/gui/client/static/css/style.css
+drwxrwxrwx   0        0        0        0 2024-04-07 13:59:20.957429 gskChat-1.0.9/gskChat/gui/client/static/img/
+-rw-rw-rw-   0        0        0     4286 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/gui/client/static/img/1.png
+-rw-rw-rw-   0        0        0        0 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/gui/client/static/img/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-07 13:59:20.958425 gskChat-1.0.9/gskChat/gui/client/static/img/__pycache__/
+-rw-rw-rw-   0        0        0      211 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/gui/client/static/img/__pycache__/__init__.cpython-312.pyc
+-rw-rw-rw-   0        0        0     8908 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/gui/client/static/img/android-chrome-192x192.png
+-rw-rw-rw-   0        0        0    17626 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/gui/client/static/img/android-chrome-512x512.png
+-rw-rw-rw-   0        0        0     7984 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/gui/client/static/img/apple-touch-icon.png
+-rw-rw-rw-   0        0        0     2258 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/gui/client/static/img/content.png
+drwxrwxrwx   0        0        0        0 2024-04-07 13:59:20.959422 gskChat-1.0.9/gskChat/gui/client/static/img/cursor/
+-rw-rw-rw-   0        0        0        0 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/gui/client/static/img/cursor/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-07 13:59:20.959422 gskChat-1.0.9/gskChat/gui/client/static/img/cursor/__pycache__/
+-rw-rw-rw-   0        0        0      218 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/gui/client/static/img/cursor/__pycache__/__init__.cpython-312.pyc
+-rw-rw-rw-   0        0        0      721 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/gui/client/static/img/favicon-16x16.png
+-rw-rw-rw-   0        0        0      499 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/gui/client/static/img/favicon-16x162.png
+-rw-rw-rw-   0        0        0     4286 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/gui/client/static/img/favicon-32x32.png
+-rw-rw-rw-   0        0        0   501120 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/gui/client/static/img/gpt.png
+-rw-rw-rw-   0        0        0     2885 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/gui/client/static/img/gpt1.png
+-rw-rw-rw-   0        0        0     2551 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/gui/client/static/img/graphic-designer.png
+-rw-rw-rw-   0        0        0  2853419 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/gui/client/static/img/loading-1.gif
+-rw-rw-rw-   0        0        0   251420 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/gui/client/static/img/loading-101.gif
+-rw-rw-rw-   0        0        0   162448 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/gui/client/static/img/programmer.jpg
+-rw-rw-rw-   0        0        0     1783 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/gui/client/static/img/programmer.png
+-rw-rw-rw-   0        0        0      447 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/gui/client/static/img/site.webmanifest
+-rw-rw-rw-   0        0        0   200333 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/gui/client/static/img/teacher.jpg
+-rw-rw-rw-   0        0        0    23088 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/gui/client/static/img/telegram.png
+-rw-rw-rw-   0        0        0   175178 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/gui/client/static/img/user.png
+-rw-rw-rw-   0        0        0   117644 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/gui/client/static/img/write.jpg
+drwxrwxrwx   0        0        0        0 2024-04-07 13:59:21.005483 gskChat-1.0.9/gskChat/gui/client/static/js/
+-rw-rw-rw-   0        0        0        0 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/gui/client/static/js/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-07 13:59:21.006481 gskChat-1.0.9/gskChat/gui/client/static/js/__pycache__/
+-rw-rw-rw-   0        0        0      210 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/gui/client/static/js/__pycache__/__init__.cpython-312.pyc
+-rw-rw-rw-   0        0        0    33901 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/gui/client/static/js/chat.v1.js
+-rw-rw-rw-   0        0        0   118841 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/gui/client/static/js/highlight.min.js
+-rw-rw-rw-   0        0        0     1083 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/gui/client/static/js/highlightjs-copy.min.js
+-rw-rw-rw-   0        0        0    10865 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/gui/client/static/js/icons.js
+-rw-rw-rw-   0        0        0      410 2024-04-07 13:22:40.000000 gskChat-1.0.9/gskChat/gui/client/test.html
+-rw-rw-rw-   0        0        0      615 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/gui/run.py
+drwxrwxrwx   0        0        0        0 2024-04-07 13:59:21.011516 gskChat-1.0.9/gskChat/gui/server/
+-rw-rw-rw-   0        0        0        0 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/gui/server/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-07 13:59:21.020713 gskChat-1.0.9/gskChat/gui/server/__pycache__/
+-rw-rw-rw-   0        0        0      200 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/gui/server/__pycache__/__init__.cpython-312.pyc
+-rw-rw-rw-   0        0        0     3366 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/gui/server/__pycache__/android_gallery.cpython-312.pyc
+-rw-rw-rw-   0        0        0    12282 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/gui/server/__pycache__/api.cpython-312.pyc
+-rw-rw-rw-   0        0        0      577 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/gui/server/__pycache__/app.cpython-312.pyc
+-rw-rw-rw-   0        0        0     4568 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/gui/server/__pycache__/backend.cpython-312.pyc
+-rw-rw-rw-   0        0        0    14765 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/gui/server/__pycache__/config.cpython-312.pyc
+-rw-rw-rw-   0        0        0     7883 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/gui/server/__pycache__/internet.cpython-312.pyc
+-rw-rw-rw-   0        0        0     1513 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/gui/server/__pycache__/website.cpython-312.pyc
+-rw-rw-rw-   0        0        0     2470 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/gui/server/android_gallery.py
+-rw-rw-rw-   0        0        0     9422 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/gui/server/api.py
+-rw-rw-rw-   0        0        0      271 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/gui/server/app.py
+-rw-rw-rw-   0        0        0     3681 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/gui/server/backend.py
+-rw-rw-rw-   0        0        0    15354 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/gui/server/config.py
+-rw-rw-rw-   0        0        0     4918 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/gui/server/internet.py
+-rw-rw-rw-   0        0        0      839 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/gui/server/website.py
+-rw-rw-rw-   0        0        0     1200 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/gui/webview.py
+-rw-rw-rw-   0        0        0     8399 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/image.py
+drwxrwxrwx   0        0        0        0 2024-04-07 13:59:21.021710 gskChat-1.0.9/gskChat/local/
+-rw-rw-rw-   0        0        0     1405 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/local/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-07 13:59:21.024702 gskChat-1.0.9/gskChat/local/__pycache__/
+-rw-rw-rw-   0        0        0     2679 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/local/__pycache__/__init__.cpython-312.pyc
+-rw-rw-rw-   0        0        0     3047 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/local/__pycache__/_engine.cpython-312.pyc
+-rw-rw-rw-   0        0        0     2179 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/local/__pycache__/_models.cpython-312.pyc
+-rw-rw-rw-   0        0        0     1832 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/local/_engine.py
+-rw-rw-rw-   0        0        0     2959 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/local/_models.py
+-rw-rw-rw-   0        0        0     7633 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/models.py
+drwxrwxrwx   0        0        0        0 2024-04-07 13:59:21.029490 gskChat-1.0.9/gskChat/providers/
+-rw-rw-rw-   0        0        0        0 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/providers/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-07 13:59:21.035504 gskChat-1.0.9/gskChat/providers/__pycache__/
+-rw-rw-rw-   0        0        0      199 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/providers/__pycache__/__init__.cpython-312.pyc
+-rw-rw-rw-   0        0        0    13248 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/providers/__pycache__/base_provider.cpython-312.pyc
+-rw-rw-rw-   0        0        0     7555 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/providers/__pycache__/create_images.cpython-312.pyc
+-rw-rw-rw-   0        0        0     2745 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/providers/__pycache__/helper.cpython-312.pyc
+-rw-rw-rw-   0        0        0     9044 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/providers/__pycache__/retry_provider.cpython-312.pyc
+-rw-rw-rw-   0        0        0     4203 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/providers/__pycache__/types.cpython-312.pyc
+-rw-rw-rw-   0        0        0     9260 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/providers/base_provider.py
+-rw-rw-rw-   0        0        0     6594 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/providers/create_images.py
+-rw-rw-rw-   0        0        0     1528 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/providers/helper.py
+-rw-rw-rw-   0        0        0     6869 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/providers/retry_provider.py
+-rw-rw-rw-   0        0        0     3083 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/providers/types.py
+drwxrwxrwx   0        0        0        0 2024-04-07 13:59:21.038497 gskChat-1.0.9/gskChat/requests/
+-rw-rw-rw-   0        0        0     3959 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/requests/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-07 13:59:21.044537 gskChat-1.0.9/gskChat/requests/__pycache__/
+-rw-rw-rw-   0        0        0     4981 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/requests/__pycache__/__init__.cpython-312.pyc
+-rw-rw-rw-   0        0        0     3226 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/requests/__pycache__/aiohttp.cpython-312.pyc
+-rw-rw-rw-   0        0        0     5284 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/requests/__pycache__/curl_cffi.cpython-312.pyc
+-rw-rw-rw-   0        0        0     1415 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/requests/__pycache__/defaults.cpython-312.pyc
+-rw-rw-rw-   0        0        0     2638 2024-03-25 09:33:27.000000 gskChat-1.0.9/gskChat/requests/__pycache__/raise_for_status.cpython-312.pyc
+-rw-rw-rw-   0        0        0     1775 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/requests/aiohttp.py
+-rw-rw-rw-   0        0        0     3016 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/requests/curl_cffi.py
+-rw-rw-rw-   0        0        0     1091 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/requests/defaults.py
+-rw-rw-rw-   0        0        0     1625 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/requests/raise_for_status.py
+-rw-rw-rw-   0        0        0     2938 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/stubs.py
+-rw-rw-rw-   0        0        0      875 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/typing.py
+-rw-rw-rw-   0        0        0     3821 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/version.py
+-rw-rw-rw-   0        0        0     9953 2024-03-25 09:33:26.000000 gskChat-1.0.9/gskChat/webdriver.py
+drwxrwxrwx   0        0        0        0 2024-04-07 13:59:21.045534 gskChat-1.0.9/gskChat.egg-info/
+-rw-rw-rw-   0        0        0     2874 2024-04-07 13:59:20.000000 gskChat-1.0.9/gskChat.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    15760 2024-04-07 13:59:20.000000 gskChat-1.0.9/gskChat.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-07 13:59:20.000000 gskChat-1.0.9/gskChat.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2024-04-07 13:59:20.000000 gskChat-1.0.9/gskChat.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      621 2024-04-07 13:59:20.000000 gskChat-1.0.9/gskChat.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-07 13:59:20.000000 gskChat-1.0.9/gskChat.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-07 13:59:21.050769 gskChat-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     3200 2024-04-07 13:59:12.000000 gskChat-1.0.9/setup.py
```

### Comparing `gskChat-1.0.8/PKG-INFO` & `gskChat-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gskChat
-Version: 1.0.8
+Version: 1.0.9
 Summary: Gsk Chatbot
 Author: tafik
 Author-email: <doneld528@gmail.com>
 Keywords: python,chatbot,reverse-engineering,openai,chatbots,gpt,language-model,gpt-3,gpt3,openai-api,gpt-4,gpt4,chatgpt,chatgpt-api,openai-chatgpt,chatgpt-free,chatgpt-4,chatgpt4,chatgpt4-api,free,free-gpt,gpt4free,g4f
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `gskChat-1.0.8/gskChat/Provider/Aura.py` & `gskChat-1.0.9/gskChat/Provider/Aura.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.8/gskChat/Provider/Bing.py` & `gskChat-1.0.9/gskChat/Provider/Bing.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.8/gskChat/Provider/BingCreateImages.py` & `gskChat-1.0.9/gskChat/Provider/BingCreateImages.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.8/gskChat/Provider/ChatForAi.py` & `gskChat-1.0.9/gskChat/Provider/ChatForAi.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.8/gskChat/Provider/Chatgpt4Online.py` & `gskChat-1.0.9/gskChat/Provider/Chatgpt4Online.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.8/gskChat/Provider/ChatgptAi.py` & `gskChat-1.0.9/gskChat/Provider/ChatgptAi.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.8/gskChat/Provider/ChatgptFree.py` & `gskChat-1.0.9/gskChat/Provider/ChatgptFree.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.8/gskChat/Provider/ChatgptNext.py` & `gskChat-1.0.9/gskChat/Provider/ChatgptNext.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.8/gskChat/Provider/ChatgptX.py` & `gskChat-1.0.9/gskChat/Provider/ChatgptX.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.8/gskChat/Provider/DeepInfra.py` & `gskChat-1.0.9/gskChat/Provider/DeepInfra.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.8/gskChat/Provider/FlowGpt.py` & `gskChat-1.0.9/gskChat/Provider/FlowGpt.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.8/gskChat/Provider/FreeChatgpt.py` & `gskChat-1.0.9/gskChat/Provider/FreeChatgpt.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.8/gskChat/Provider/FreeGpt.py` & `gskChat-1.0.9/gskChat/Provider/FreeGpt.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.8/gskChat/Provider/GeminiPro.py` & `gskChat-1.0.9/gskChat/Provider/GeminiPro.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.8/gskChat/Provider/GeminiProChat.py` & `gskChat-1.0.9/gskChat/Provider/GeminiProChat.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.8/gskChat/Provider/GigaChat.py` & `gskChat-1.0.9/gskChat/Provider/GigaChat.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.8/gskChat/Provider/GptTalkRu.py` & `gskChat-1.0.9/gskChat/Provider/GptTalkRu.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.8/gskChat/Provider/HuggingChat.py` & `gskChat-1.0.9/gskChat/Provider/HuggingChat.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.8/gskChat/Provider/HuggingFace.py` & `gskChat-1.0.9/gskChat/Provider/HuggingFace.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.8/gskChat/Provider/Koala.py` & `gskChat-1.0.9/gskChat/Provider/Koala.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.8/gskChat/Provider/Liaobots.py` & `gskChat-1.0.9/gskChat/Provider/Liaobots.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.8/gskChat/Provider/Llama2.py` & `gskChat-1.0.9/gskChat/Provider/Llama2.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.8/gskChat/Provider/PerplexityLabs.py` & `gskChat-1.0.9/gskChat/Provider/PerplexityLabs.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.8/gskChat/Provider/Pi.py` & `gskChat-1.0.9/gskChat/Provider/Pi.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.8/gskChat/Provider/Vercel.py` & `gskChat-1.0.9/gskChat/Provider/Vercel.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.8/gskChat/Provider/You.py` & `gskChat-1.0.9/gskChat/Provider/You.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.8/gskChat/Provider/__init__.py` & `gskChat-1.0.9/gskChat/Provider/__init__.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.8/gskChat/Provider/__pycache__/Aura.cpython-312.pyc` & `gskChat-1.0.9/gskChat/Provider/__pycache__/Aura.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Sun Mar 24 15:25:23 2024 UTC, .py size: 1607 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: cb0d 0d0a 0000 0000 e345 0066 4706 0000  .........E.fG...
+00000000: cb0d 0d0a 0000 0000 e644 0166 4706 0000  .........D.fG...
 00000010: e300 0000 0000 0000 0000 0000 0005 0000  ................
 00000020: 0000 0000 01f3 6600 0000 9700 6400 6401  ......f.....d.d.
 00000030: 6c00 6d01 5a01 0100 6400 6402 6c02 6d03  l.m.Z...d.d.l.m.
 00000040: 5a03 0100 6403 6404 6c04 6d05 5a05 6d06  Z...d.d.l.m.Z.m.
 00000050: 5a06 0100 6405 6406 6c07 6d08 5a08 0100  Z...d.d.l.m.Z...
 00000060: 6403 6407 6c09 6d0a 5a0a 0100 6403 6408  d.d.l.m.Z...d.d.
 00000070: 6c0b 6d0c 5a0c 0100 0200 4700 6409 8400  l.m.Z.....G.d...
```

### Comparing `gskChat-1.0.8/gskChat/Provider/__pycache__/Bing.cpython-312.pyc` & `gskChat-1.0.9/gskChat/Provider/__pycache__/Bing.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Sun Mar 24 15:25:23 2024 UTC, .py size: 20640 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: cb0d 0d0a 0000 0000 e345 0066 a050 0000  .........E.f.P..
+00000000: cb0d 0d0a 0000 0000 e644 0166 a050 0000  .........D.f.P..
 00000010: e300 0000 0000 0000 0000 0000 0006 0000  ................
 00000020: 0000 0000 01f3 f001 0000 9700 6400 6401  ............d.d.
 00000030: 6c00 6d01 5a01 0100 6400 6402 6c02 5a02  l.m.Z...d.d.l.Z.
 00000040: 6400 6402 6c03 5a03 6400 6402 6c04 5a04  d.d.l.Z.d.d.l.Z.
 00000050: 6400 6402 6c05 5a05 6400 6402 6c06 5a06  d.d.l.Z.d.d.l.Z.
 00000060: 6400 6403 6c07 6d08 5a08 0100 6400 6404  d.d.l.m.Z...d.d.
 00000070: 6c09 6d09 5a09 0100 6400 6405 6c0a 6d0b  l.m.Z...d.d.l.m.
```

### Comparing `gskChat-1.0.8/gskChat/Provider/__pycache__/BingCreateImages.cpython-312.pyc` & `gskChat-1.0.9/gskChat/Provider/__pycache__/BingCreateImages.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Sun Mar 24 15:25:23 2024 UTC, .py size: 2193 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: cb0d 0d0a 0000 0000 e345 0066 9108 0000  .........E.f....
+00000000: cb0d 0d0a 0000 0000 e644 0166 9108 0000  .........D.f....
 00000010: e300 0000 0000 0000 0000 0000 0004 0000  ................
 00000020: 0000 0000 01f3 8c00 0000 9700 6400 6401  ............d.d.
 00000030: 6c00 6d01 5a01 0100 6400 6402 6c02 5a02  l.m.Z...d.d.l.Z.
 00000040: 6400 6402 6c03 5a03 6400 6403 6c04 6d05  d.d.l.Z.d.d.l.m.
 00000050: 5a05 6d06 5a06 0100 6404 6405 6c07 6d08  Z.m.Z...d.d.l.m.
 00000060: 5a08 0100 6404 6406 6c09 6d0a 5a0a 0100  Z...d.d.l.m.Z...
 00000070: 6404 6407 6c0b 6d0c 5a0c 6d0d 5a0d 0100  d.d.l.m.Z.m.Z...
```

### Comparing `gskChat-1.0.8/gskChat/Provider/__pycache__/ChatForAi.cpython-312.pyc` & `gskChat-1.0.9/gskChat/Provider/__pycache__/ChatForAi.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Sun Mar 24 15:25:23 2024 UTC, .py size: 2508 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: cb0d 0d0a 0000 0000 e345 0066 cc09 0000  .........E.f....
+00000000: cb0d 0d0a 0000 0000 e644 0166 cc09 0000  .........D.f....
 00000010: e300 0000 0000 0000 0000 0000 0006 0000  ................
 00000020: 0000 0000 01f3 8000 0000 9700 6400 6401  ............d.d.
 00000030: 6c00 6d01 5a01 0100 6400 6402 6c02 5a02  l.m.Z...d.d.l.Z.
 00000040: 6400 6402 6c03 5a03 6400 6402 6c04 5a04  d.d.l.Z.d.d.l.Z.
 00000050: 6403 6404 6c05 6d06 5a06 6d07 5a07 0100  d.d.l.m.Z.m.Z...
 00000060: 6403 6405 6c08 6d09 5a09 0100 6403 6406  d.d.l.m.Z...d.d.
 00000070: 6c0a 6d0b 5a0b 0100 6407 6408 6c0c 6d0d  l.m.Z...d.d.l.m.
```

### Comparing `gskChat-1.0.8/gskChat/Provider/__pycache__/Chatgpt4Online.cpython-312.pyc` & `gskChat-1.0.9/gskChat/Provider/__pycache__/Chatgpt4Online.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Sun Mar 24 15:25:23 2024 UTC, .py size: 2653 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: cb0d 0d0a 0000 0000 e345 0066 5d0a 0000  .........E.f]...
+00000000: cb0d 0d0a 0000 0000 e644 0166 5d0a 0000  .........D.f]...
 00000010: e300 0000 0000 0000 0000 0000 0005 0000  ................
 00000020: 0000 0000 01f3 7600 0000 9700 6400 6401  ......v.....d.d.
 00000030: 6c00 6d01 5a01 0100 6400 6402 6c02 5a02  l.m.Z...d.d.l.Z.
 00000040: 6400 6402 6c03 5a03 6400 6403 6c04 6d05  d.d.l.Z.d.d.l.m.
 00000050: 5a05 0100 6404 6405 6c06 6d07 5a07 6d08  Z...d.d.l.m.Z.m.
 00000060: 5a08 0100 6404 6406 6c09 6d0a 5a0a 0100  Z...d.d.l.m.Z...
 00000070: 6407 6408 6c0b 6d0c 5a0c 0100 6407 6409  d.d.l.m.Z...d.d.
```

### Comparing `gskChat-1.0.8/gskChat/Provider/__pycache__/ChatgptAi.cpython-312.pyc` & `gskChat-1.0.9/gskChat/Provider/__pycache__/ChatgptAi.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Sun Mar 24 15:25:23 2024 UTC, .py size: 3608 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: cb0d 0d0a 0000 0000 e345 0066 180e 0000  .........E.f....
+00000000: cb0d 0d0a 0000 0000 e644 0166 180e 0000  .........D.f....
 00000010: e300 0000 0000 0000 0000 0000 0005 0000  ................
 00000020: 0000 0000 01f3 8e00 0000 9700 6400 6401  ............d.d.
 00000030: 6c00 6d01 5a01 0100 6400 6402 6c02 5a02  l.m.Z...d.d.l.Z.
 00000040: 6400 6402 6c03 5a03 6400 6402 6c04 5a04  d.d.l.Z.d.d.l.Z.
 00000050: 6400 6402 6c05 5a05 6400 6402 6c06 5a06  d.d.l.Z.d.d.l.Z.
 00000060: 6400 6403 6c07 6d08 5a08 0100 6404 6405  d.d.l.m.Z...d.d.
 00000070: 6c09 6d0a 5a0a 6d0b 5a0b 0100 6404 6406  l.m.Z.m.Z...d.d.
```

### Comparing `gskChat-1.0.8/gskChat/Provider/__pycache__/ChatgptFree.cpython-312.pyc` & `gskChat-1.0.9/gskChat/Provider/__pycache__/ChatgptFree.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Sun Mar 24 15:25:23 2024 UTC, .py size: 2855 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: cb0d 0d0a 0000 0000 e345 0066 270b 0000  .........E.f'...
+00000000: cb0d 0d0a 0000 0000 e644 0166 270b 0000  .........D.f'...
 00000010: e300 0000 0000 0000 0000 0000 0005 0000  ................
 00000020: 0000 0000 01f3 5e00 0000 9700 6400 6401  ......^.....d.d.
 00000030: 6c00 6d01 5a01 0100 6400 6402 6c02 5a02  l.m.Z...d.d.l.Z.
 00000040: 6403 6404 6c03 6d04 5a04 0100 6403 6405  d.d.l.m.Z...d.d.
 00000050: 6c05 6d06 5a06 0100 6406 6407 6c07 6d08  l.m.Z...d.d.l.m.
 00000060: 5a08 0100 6406 6408 6c09 6d0a 5a0a 0100  Z...d.d.l.m.Z...
 00000070: 0200 4700 6409 8400 640a 6508 ab03 0000  ..G.d...d.e.....
```

### Comparing `gskChat-1.0.8/gskChat/Provider/__pycache__/ChatgptNext.cpython-312.pyc` & `gskChat-1.0.9/gskChat/Provider/__pycache__/ChatgptNext.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Sun Mar 24 15:25:23 2024 UTC, .py size: 2503 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: cb0d 0d0a 0000 0000 e345 0066 c709 0000  .........E.f....
+00000000: cb0d 0d0a 0000 0000 e644 0166 c709 0000  .........D.f....
 00000010: e300 0000 0000 0000 0000 0000 0005 0000  ................
 00000020: 0000 0000 01f3 5600 0000 9700 6400 6401  ......V.....d.d.
 00000030: 6c00 6d01 5a01 0100 6400 6402 6c02 5a02  l.m.Z...d.d.l.Z.
 00000040: 6400 6403 6c03 6d04 5a04 0100 6404 6405  d.d.l.m.Z...d.d.
 00000050: 6c05 6d06 5a06 6d07 5a07 0100 6406 6407  l.m.Z.m.Z...d.d.
 00000060: 6c08 6d09 5a09 0100 0200 4700 6408 8400  l.m.Z.....G.d...
 00000070: 6409 6509 ab03 0000 0000 0000 5a0a 7902  d.e.........Z.y.
```

### Comparing `gskChat-1.0.8/gskChat/Provider/__pycache__/ChatgptX.cpython-312.pyc` & `gskChat-1.0.9/gskChat/Provider/__pycache__/ChatgptX.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Sun Mar 24 15:25:23 2024 UTC, .py size: 4278 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: cb0d 0d0a 0000 0000 e345 0066 b610 0000  .........E.f....
+00000000: cb0d 0d0a 0000 0000 e644 0166 b610 0000  .........D.f....
 00000010: e300 0000 0000 0000 0000 0000 0005 0000  ................
 00000020: 0000 0000 01f3 7600 0000 9700 6400 6401  ......v.....d.d.
 00000030: 6c00 6d01 5a01 0100 6400 6402 6c02 5a02  l.m.Z...d.d.l.Z.
 00000040: 6400 6402 6c03 5a03 6400 6403 6c04 6d05  d.d.l.Z.d.d.l.m.
 00000050: 5a05 0100 6404 6405 6c06 6d07 5a07 6d08  Z...d.d.l.m.Z.m.
 00000060: 5a08 0100 6406 6407 6c09 6d0a 5a0a 0100  Z...d.d.l.m.Z...
 00000070: 6406 6408 6c0b 6d0c 5a0c 0100 6404 6409  d.d.l.m.Z...d.d.
```

### Comparing `gskChat-1.0.8/gskChat/Provider/__pycache__/DeepInfra.cpython-312.pyc` & `gskChat-1.0.9/gskChat/Provider/__pycache__/DeepInfra.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Sun Mar 24 15:25:23 2024 UTC, .py size: 3526 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: cb0d 0d0a 0000 0000 e345 0066 c60d 0000  .........E.f....
+00000000: cb0d 0d0a 0000 0000 e644 0166 c60d 0000  .........D.f....
 00000010: e300 0000 0000 0000 0000 0000 0006 0000  ................
 00000020: 0000 0000 01f3 6400 0000 9700 6400 6401  ......d.....d.d.
 00000030: 6c00 6d01 5a01 0100 6400 6402 6c02 5a02  l.m.Z...d.d.l.Z.
 00000040: 6400 6402 6c03 5a03 6403 6404 6c04 6d05  d.d.l.Z.d.d.l.m.
 00000050: 5a05 6d06 5a06 0100 6405 6406 6c07 6d08  Z.m.Z...d.d.l.m.
 00000060: 5a08 6d09 5a09 0100 6403 6407 6c03 6d0a  Z.m.Z...d.d.l.m.
 00000070: 5a0a 0100 0200 4700 6408 8400 6409 6508  Z.....G.d...d.e.
```

### Comparing `gskChat-1.0.8/gskChat/Provider/__pycache__/FlowGpt.cpython-312.pyc` & `gskChat-1.0.9/gskChat/Provider/__pycache__/FlowGpt.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Sun Mar 24 15:25:23 2024 UTC, .py size: 3196 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: cb0d 0d0a 0000 0000 e345 0066 7c0c 0000  .........E.f|...
+00000000: cb0d 0d0a 0000 0000 e644 0166 7c0c 0000  .........D.f|...
 00000010: e300 0000 0000 0000 0000 0000 0006 0000  ................
 00000020: 0000 0000 01f3 6800 0000 9700 6400 6401  ......h.....d.d.
 00000030: 6c00 6d01 5a01 0100 6400 6402 6c02 5a02  l.m.Z...d.d.l.Z.
 00000040: 6400 6403 6c03 6d04 5a04 0100 6404 6405  d.d.l.m.Z...d.d.
 00000050: 6c05 6d06 5a06 6d07 5a07 0100 6406 6407  l.m.Z.m.Z...d.d.
 00000060: 6c08 6d09 5a09 6d0a 5a0a 0100 6404 6408  l.m.Z.m.Z...d.d.
 00000070: 6c0b 6d0c 5a0c 0100 0200 4700 6409 8400  l.m.Z.....G.d...
```

### Comparing `gskChat-1.0.8/gskChat/Provider/__pycache__/FreeChatgpt.cpython-312.pyc` & `gskChat-1.0.9/gskChat/Provider/__pycache__/FreeChatgpt.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Sun Mar 24 15:25:23 2024 UTC, .py size: 2530 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: cb0d 0d0a 0000 0000 e345 0066 e209 0000  .........E.f....
+00000000: cb0d 0d0a 0000 0000 e644 0166 e209 0000  .........D.f....
 00000010: e300 0000 0000 0000 0000 0000 0006 0000  ................
 00000020: 0000 0000 01f3 6000 0000 9700 6400 6401  ......`.....d.d.
 00000030: 6c00 6d01 5a01 0100 6400 6402 6c02 5a02  l.m.Z...d.d.l.Z.
 00000040: 6400 6403 6c03 6d04 5a04 6d05 5a05 0100  d.d.l.m.Z.m.Z...
 00000050: 6404 6405 6c06 6d07 5a07 6d08 5a08 0100  d.d.l.m.Z.m.Z...
 00000060: 6406 6407 6c09 6d0a 5a0a 6d0b 5a0b 0100  d.d.l.m.Z.m.Z...
 00000070: 0200 4700 6408 8400 6409 650a 650b ab04  ..G.d...d.e.e...
```

### Comparing `gskChat-1.0.8/gskChat/Provider/__pycache__/FreeGpt.cpython-312.pyc` & `gskChat-1.0.9/gskChat/Provider/__pycache__/FreeGpt.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Sun Mar 24 15:25:23 2024 UTC, .py size: 1791 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: cb0d 0d0a 0000 0000 e345 0066 ff06 0000  .........E.f....
+00000000: cb0d 0d0a 0000 0000 e644 0166 ff06 0000  .........D.f....
 00000010: e300 0000 0000 0000 0000 0000 0005 0000  ................
 00000020: 0000 0000 01f3 8400 0000 9700 6400 6401  ............d.d.
 00000030: 6c00 6d01 5a01 0100 6400 6402 6c02 5a02  l.m.Z...d.d.l.Z.
 00000040: 6400 6402 6c03 5a03 6400 6402 6c04 5a04  d.d.l.Z.d.d.l.Z.
 00000050: 6403 6404 6c05 6d06 5a06 6d07 5a07 0100  d.d.l.m.Z.m.Z...
 00000060: 6403 6405 6c08 6d09 5a09 0100 6406 6407  d.d.l.m.Z...d.d.
 00000070: 6c0a 6d0b 5a0b 0100 6403 6408 6c0c 6d0d  l.m.Z...d.d.l.m.
```

### Comparing `gskChat-1.0.8/gskChat/Provider/__pycache__/GeminiPro.cpython-312.pyc` & `gskChat-1.0.9/gskChat/Provider/__pycache__/GeminiPro.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Sun Mar 24 15:25:23 2024 UTC, .py size: 3937 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: cb0d 0d0a 0000 0000 e345 0066 610f 0000  .........E.fa...
+00000000: cb0d 0d0a 0000 0000 e644 0166 610f 0000  .........D.fa...
 00000010: e300 0000 0000 0000 0000 0000 0006 0000  ................
 00000020: 0000 0000 01f3 9400 0000 9700 6400 6401  ............d.d.
 00000030: 6c00 6d01 5a01 0100 6400 6402 6c02 5a02  l.m.Z...d.d.l.Z.
 00000040: 6400 6402 6c03 5a03 6400 6403 6c04 6d05  d.d.l.Z.d.d.l.m.
 00000050: 5a05 6d06 5a06 0100 6404 6405 6c07 6d08  Z.m.Z...d.d.l.m.
 00000060: 5a08 6d09 5a09 6d0a 5a0a 0100 6406 6407  Z.m.Z.m.Z...d.d.
 00000070: 6c0b 6d0c 5a0c 6d0d 5a0d 0100 6404 6408  l.m.Z.m.Z...d.d.
```

### Comparing `gskChat-1.0.8/gskChat/Provider/__pycache__/GeminiProChat.cpython-312.pyc` & `gskChat-1.0.9/gskChat/Provider/__pycache__/GeminiProChat.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Sun Mar 24 15:25:23 2024 UTC, .py size: 2557 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: cb0d 0d0a 0000 0000 e345 0066 fd09 0000  .........E.f....
+00000000: cb0d 0d0a 0000 0000 e644 0166 fd09 0000  .........D.f....
 00000010: e300 0000 0000 0000 0000 0000 0005 0000  ................
 00000020: 0000 0000 01f3 9400 0000 9700 6400 6401  ............d.d.
 00000030: 6c00 6d01 5a01 0100 6400 6402 6c02 5a02  l.m.Z...d.d.l.Z.
 00000040: 6400 6403 6c03 6d04 5a04 0100 6400 6404  d.d.l.m.Z...d.d.
 00000050: 6c05 6d06 5a06 6d07 5a07 0100 6405 6406  l.m.Z.m.Z...d.d.
 00000060: 6c08 6d09 5a09 6d0a 5a0a 0100 6407 6408  l.m.Z.m.Z...d.d.
 00000070: 6c0b 6d0c 5a0c 0100 6405 6409 6c0d 6d0e  l.m.Z...d.d.l.m.
```

### Comparing `gskChat-1.0.8/gskChat/Provider/__pycache__/GigaChat.cpython-312.pyc` & `gskChat-1.0.9/gskChat/Provider/__pycache__/GigaChat.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Sun Mar 24 15:25:23 2024 UTC, .py size: 3926 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: cb0d 0d0a 0000 0000 e345 0066 560f 0000  .........E.fV...
+00000000: cb0d 0d0a 0000 0000 e644 0166 560f 0000  .........D.fV...
 00000010: e300 0000 0000 0000 0000 0000 0006 0000  ................
 00000020: 0000 0000 01f3 b000 0000 9700 6400 6401  ............d.d.
 00000030: 6c00 6d01 5a01 0100 6400 6402 6c02 5a02  l.m.Z...d.d.l.Z.
 00000040: 6400 6402 6c03 5a03 6400 6402 6c04 5a04  d.d.l.Z.d.d.l.Z.
 00000050: 6400 6402 6c05 5a05 6400 6402 6c06 5a06  d.d.l.Z.d.d.l.Z.
 00000060: 6400 6403 6c07 6d08 5a08 6d09 5a09 6d0a  d.d.l.m.Z.m.Z.m.
 00000070: 5a0a 0100 6400 6404 6c0b 6d0c 5a0c 0100  Z...d.d.l.m.Z...
```

### Comparing `gskChat-1.0.8/gskChat/Provider/__pycache__/GptTalkRu.cpython-312.pyc` & `gskChat-1.0.9/gskChat/Provider/__pycache__/GptTalkRu.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Sun Mar 24 15:25:23 2024 UTC, .py size: 2321 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: cb0d 0d0a 0000 0000 e345 0066 1109 0000  .........E.f....
+00000000: cb0d 0d0a 0000 0000 e644 0166 1109 0000  .........D.f....
 00000010: e300 0000 0000 0000 0000 0000 0005 0000  ................
 00000020: 0000 0000 01f3 9600 0000 9700 6400 6401  ............d.d.
 00000030: 6c00 6d01 5a01 0100 6400 6402 6c02 6d03  l.m.Z...d.d.l.m.
 00000040: 5a03 6d04 5a04 0100 6403 6404 6c05 6d06  Z.m.Z...d.d.l.m.
 00000050: 5a06 6d07 5a07 0100 6405 6406 6c08 6d09  Z.m.Z...d.d.l.m.
 00000060: 5a09 0100 6405 6407 6c0a 6d0b 5a0b 6d0c  Z...d.d.l.m.Z.m.
 00000070: 5a0c 0100 6403 6408 6c0d 6d0e 5a0e 6d0f  Z...d.d.l.m.Z.m.
```

### Comparing `gskChat-1.0.8/gskChat/Provider/__pycache__/HuggingChat.cpython-312.pyc` & `gskChat-1.0.9/gskChat/Provider/__pycache__/HuggingChat.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Sun Mar 24 15:25:23 2024 UTC, .py size: 3615 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: cb0d 0d0a 0000 0000 e345 0066 1f0e 0000  .........E.f....
+00000000: cb0d 0d0a 0000 0000 e644 0166 1f0e 0000  .........D.f....
 00000010: e300 0000 0000 0000 0000 0000 0006 0000  ................
 00000020: 0000 0000 01f3 7000 0000 9700 6400 6401  ......p.....d.d.
 00000030: 6c00 6d01 5a01 0100 6400 6402 6c02 5a02  l.m.Z...d.d.l.Z.
 00000040: 6400 6403 6c03 6d04 5a04 6d05 5a05 0100  d.d.l.m.Z.m.Z...
 00000050: 6404 6405 6c06 6d07 5a07 6d08 5a08 0100  d.d.l.m.Z.m.Z...
 00000060: 6406 6407 6c09 6d0a 5a0a 6d0b 5a0b 0100  d.d.l.m.Z.m.Z...
 00000070: 6406 6408 6c0c 6d0d 5a0d 6d0e 5a0e 0100  d.d.l.m.Z.m.Z...
```

### Comparing `gskChat-1.0.8/gskChat/Provider/__pycache__/HuggingFace.cpython-312.pyc` & `gskChat-1.0.9/gskChat/Provider/__pycache__/HuggingFace.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Sun Mar 24 15:25:23 2024 UTC, .py size: 2940 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: cb0d 0d0a 0000 0000 e345 0066 7c0b 0000  .........E.f|...
+00000000: cb0d 0d0a 0000 0000 e644 0166 7c0b 0000  .........D.f|...
 00000010: e300 0000 0000 0000 0000 0000 0006 0000  ................
 00000020: 0000 0000 01f3 9000 0000 9700 6400 6401  ............d.d.
 00000030: 6c00 6d01 5a01 0100 6400 6402 6c02 5a02  l.m.Z...d.d.l.Z.
 00000040: 6400 6403 6c03 6d04 5a04 6d05 5a05 0100  d.d.l.m.Z.m.Z...
 00000050: 6404 6405 6c06 6d07 5a07 6d08 5a08 0100  d.d.l.m.Z.m.Z...
 00000060: 6406 6407 6c09 6d0a 5a0a 6d0b 5a0b 0100  d.d.l.m.Z.m.Z...
 00000070: 6406 6408 6c0c 6d0d 5a0d 0100 6404 6409  d.d.l.m.Z...d.d.
```

### Comparing `gskChat-1.0.8/gskChat/Provider/__pycache__/Koala.cpython-312.pyc` & `gskChat-1.0.9/gskChat/Provider/__pycache__/Koala.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Sun Mar 24 15:25:23 2024 UTC, .py size: 2485 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: cb0d 0d0a 0000 0000 e345 0066 b509 0000  .........E.f....
+00000000: cb0d 0d0a 0000 0000 e644 0166 b509 0000  .........D.f....
 00000010: e300 0000 0000 0000 0000 0000 0005 0000  ................
 00000020: 0000 0000 01f3 7600 0000 9700 6400 6401  ......v.....d.d.
 00000030: 6c00 6d01 5a01 0100 6400 6402 6c02 5a02  l.m.Z...d.d.l.Z.
 00000040: 6400 6403 6c03 6d04 5a04 6d05 5a05 0100  d.d.l.m.Z.m.Z...
 00000050: 6404 6405 6c06 6d07 5a07 6d08 5a08 0100  d.d.l.m.Z.m.Z...
 00000060: 6406 6407 6c09 6d0a 5a0a 0100 6406 6408  d.d.l.m.Z...d.d.
 00000070: 6c0b 6d0c 5a0c 6d0d 5a0d 0100 6404 6409  l.m.Z.m.Z...d.d.
```

### Comparing `gskChat-1.0.8/gskChat/Provider/__pycache__/Liaobots.cpython-312.pyc` & `gskChat-1.0.9/gskChat/Provider/__pycache__/Liaobots.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Sun Mar 24 15:25:23 2024 UTC, .py size: 5099 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: cb0d 0d0a 0000 0000 e345 0066 eb13 0000  .........E.f....
+00000000: cb0d 0d0a 0000 0000 e644 0166 eb13 0000  .........D.f....
 00000010: e300 0000 0000 0000 0000 0000 000f 0000  ................
 00000020: 0000 0000 01f3 0a01 0000 9700 6400 6401  ............d.d.
 00000030: 6c00 6d01 5a01 0100 6400 6402 6c02 5a02  l.m.Z...d.d.l.Z.
 00000040: 6400 6403 6c03 6d04 5a04 6d05 5a05 0100  d.d.l.m.Z.m.Z...
 00000050: 6404 6405 6c06 6d07 5a07 6d08 5a08 0100  d.d.l.m.Z.m.Z...
 00000060: 6406 6407 6c09 6d0a 5a0a 6d0b 5a0b 0100  d.d.l.m.Z.m.Z...
 00000070: 6406 6408 6c0c 6d0d 5a0d 0100 6404 6409  d.d.l.m.Z...d.d.
```

### Comparing `gskChat-1.0.8/gskChat/Provider/__pycache__/Llama2.cpython-312.pyc` & `gskChat-1.0.9/gskChat/Provider/__pycache__/Llama2.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Sun Mar 24 15:25:23 2024 UTC, .py size: 3105 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: cb0d 0d0a 0000 0000 e345 0066 210c 0000  .........E.f!...
+00000000: cb0d 0d0a 0000 0000 e644 0166 210c 0000  .........D.f!...
 00000010: e300 0000 0000 0000 0000 0000 0006 0000  ................
 00000020: 0000 0000 01f3 5c00 0000 9700 6400 6401  ......\.....d.d.
 00000030: 6c00 6d01 5a01 0100 6400 6402 6c02 6d03  l.m.Z...d.d.l.m.
 00000040: 5a03 0100 6403 6404 6c04 6d05 5a05 6d06  Z...d.d.l.m.Z.m.
 00000050: 5a06 0100 6405 6406 6c07 6d08 5a08 6d09  Z...d.d.l.m.Z.m.
 00000060: 5a09 0100 0200 4700 6407 8400 6408 6508  Z.....G.d...d.e.
 00000070: 6509 ab04 0000 0000 0000 5a0a 640b 6409  e.........Z.d.d.
```

### Comparing `gskChat-1.0.8/gskChat/Provider/__pycache__/PerplexityLabs.cpython-312.pyc` & `gskChat-1.0.9/gskChat/Provider/__pycache__/PerplexityLabs.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Sun Mar 24 15:25:23 2024 UTC, .py size: 3951 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: cb0d 0d0a 0000 0000 e345 0066 6f0f 0000  .........E.fo...
+00000000: cb0d 0d0a 0000 0000 e644 0166 6f0f 0000  .........D.fo...
 00000010: e300 0000 0000 0000 0000 0000 0006 0000  ................
 00000020: 0000 0000 01f3 7c00 0000 9700 6400 6401  ......|.....d.d.
 00000030: 6c00 6d01 5a01 0100 6400 6402 6c02 5a02  l.m.Z...d.d.l.Z.
 00000040: 6400 6402 6c03 5a03 6400 6403 6c04 6d05  d.d.l.Z.d.d.l.m.
 00000050: 5a05 6d06 5a06 0100 6404 6405 6c07 6d08  Z.m.Z...d.d.l.m.
 00000060: 5a08 6d09 5a09 0100 6406 6407 6c0a 6d0b  Z.m.Z...d.d.l.m.
 00000070: 5a0b 6d0c 5a0c 0100 6406 6408 6c0d 6d0e  Z.m.Z...d.d.l.m.
```

### Comparing `gskChat-1.0.8/gskChat/Provider/__pycache__/Pi.cpython-312.pyc` & `gskChat-1.0.9/gskChat/Provider/__pycache__/Pi.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Sun Mar 24 15:25:23 2024 UTC, .py size: 2355 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: cb0d 0d0a 0000 0000 e345 0066 3309 0000  .........E.f3...
+00000000: cb0d 0d0a 0000 0000 e644 0166 3309 0000  .........D.f3...
 00000010: e300 0000 0000 0000 0000 0000 0005 0000  ................
 00000020: 0000 0000 01f3 6200 0000 9700 6400 6401  ......b.....d.d.
 00000030: 6c00 6d01 5a01 0100 6400 6402 6c02 5a02  l.m.Z...d.d.l.Z.
 00000040: 6403 6404 6c03 6d04 5a04 6d05 5a05 0100  d.d.l.m.Z.m.Z...
 00000050: 6405 6406 6c06 6d07 5a07 6d08 5a08 0100  d.d.l.m.Z.m.Z...
 00000060: 6403 6407 6c09 6d0a 5a0a 6d0b 5a0b 6d0c  d.d.l.m.Z.m.Z.m.
 00000070: 5a0c 0100 0200 4700 6408 8400 6409 6507  Z.....G.d...d.e.
```

### Comparing `gskChat-1.0.8/gskChat/Provider/__pycache__/Vercel.cpython-312.pyc` & `gskChat-1.0.9/gskChat/Provider/__pycache__/Vercel.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Sun Mar 24 15:25:23 2024 UTC, .py size: 4027 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: cb0d 0d0a 0000 0000 e345 0066 bb0f 0000  .........E.f....
+00000000: cb0d 0d0a 0000 0000 e644 0166 bb0f 0000  .........D.f....
 00000010: e300 0000 0000 0000 0000 0000 0005 0000  ................
 00000020: 0000 0000 01f3 ba00 0000 9700 6400 6401  ............d.d.
 00000030: 6c00 6d01 5a01 0100 6400 6402 6c02 5a02  l.m.Z...d.d.l.Z.
 00000040: 6400 6402 6c03 5a03 6400 6402 6c04 5a04  d.d.l.Z.d.d.l.Z.
 00000050: 6400 6402 6c05 5a05 6400 6402 6c06 5a06  d.d.l.Z.d.d.l.Z.
 00000060: 0900 6400 6402 6c07 5a07 6403 5a08 6405  ..d.d.l.Z.d.Z.d.
 00000070: 6406 6c0a 6d0b 5a0b 6d0c 5a0c 0100 6407  d.l.m.Z.m.Z...d.
```

### Comparing `gskChat-1.0.8/gskChat/Provider/__pycache__/You.cpython-312.pyc` & `gskChat-1.0.9/gskChat/Provider/__pycache__/You.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Sun Mar 24 15:25:23 2024 UTC, .py size: 7243 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: cb0d 0d0a 0000 0000 e345 0066 4b1c 0000  .........E.fK...
+00000000: cb0d 0d0a 0000 0000 e644 0166 4b1c 0000  .........D.fK...
 00000010: e300 0000 0000 0000 0000 0000 0006 0000  ................
 00000020: 0000 0000 01f3 d400 0000 9700 6400 6401  ............d.d.
 00000030: 6c00 6d01 5a01 0100 6400 6402 6c02 5a02  l.m.Z...d.d.l.Z.
 00000040: 6400 6402 6c03 5a03 6400 6402 6c04 5a04  d.d.l.Z.d.d.l.Z.
 00000050: 6400 6402 6c05 5a05 0900 6403 6404 6c06  d.d.l.Z...d.d.l.
 00000060: 6d07 5a07 0100 6405 5a08 6403 6407 6c0a  m.Z...d.Z.d.d.l.
 00000070: 6d0b 5a0b 6d0c 5a0c 6d0d 5a0d 6d0e 5a0e  m.Z.m.Z.m.Z.m.Z.
```

### Comparing `gskChat-1.0.8/gskChat/Provider/__pycache__/__init__.cpython-312.pyc` & `gskChat-1.0.9/gskChat/Provider/__pycache__/__init__.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Sun Mar 24 15:25:23 2024 UTC, .py size: 2047 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: cb0d 0d0a 0000 0000 e345 0066 ff07 0000  .........E.f....
+00000000: cb0d 0d0a 0000 0000 e644 0166 ff07 0000  .........D.f....
 00000010: e300 0000 0000 0000 0000 0000 0007 0000  ................
 00000020: 0000 0000 01f3 5403 0000 9700 5500 6400  ......T.....U.d.
 00000030: 6401 6c00 6d01 5a01 0100 6402 6403 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 6d04 5a04 0100 6402 6404 6c05  m.Z.m.Z...d.d.l.
 00000050: 6d06 5a06 6d07 5a07 0100 6402 6405 6c08  m.Z.m.Z...d.d.l.
 00000060: 6d09 5a09 6d0a 5a0a 0100 6402 6406 6c0b  m.Z.m.Z...d.d.l.
 00000070: 6d0c 5a0c 0100 6407 6408 6c0d ad02 0100  m.Z...d.d.l.....
```

### Comparing `gskChat-1.0.8/gskChat/Provider/bing/__pycache__/conversation.cpython-312.pyc` & `gskChat-1.0.9/gskChat/Provider/bing/__pycache__/conversation.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Sun Mar 24 15:25:23 2024 UTC, .py size: 3468 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: cb0d 0d0a 0000 0000 e345 0066 8c0d 0000  .........E.f....
+00000000: cb0d 0d0a 0000 0000 e644 0166 8c0d 0000  .........D.f....
 00000010: e300 0000 0000 0000 0000 0000 0004 0000  ................
 00000020: 0000 0000 01f3 6000 0000 9700 6400 6401  ......`.....d.d.
 00000030: 6c00 6d01 5a01 0100 6400 6402 6c02 6d03  l.m.Z...d.d.l.m.
 00000040: 5a03 0100 6403 6404 6c04 6d05 5a05 0100  Z...d.d.l.m.Z...
 00000050: 6403 6405 6c06 6d07 5a07 0100 0200 4700  d.d.l.m.Z.....G.
 00000060: 6406 8400 6407 ab02 0000 0000 0000 5a08  d...d.........Z.
 00000070: 640c 6408 8404 5a09 640d 6409 8404 5a0a  d.d...Z.d.d...Z.
```

### Comparing `gskChat-1.0.8/gskChat/Provider/bing/__pycache__/create_images.cpython-312.pyc` & `gskChat-1.0.9/gskChat/Provider/bing/__pycache__/create_images.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Sun Mar 24 15:25:23 2024 UTC, .py size: 7597 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: cb0d 0d0a 0000 0000 e345 0066 ad1d 0000  .........E.f....
+00000000: cb0d 0d0a 0000 0000 e644 0166 ad1d 0000  .........D.f....
 00000010: e300 0000 0000 0000 0000 0000 0004 0000  ................
 00000020: 0000 0000 01f3 2601 0000 9700 6400 5a00  ......&.....d.Z.
 00000030: 6401 6402 6c01 6d02 5a02 0100 6401 6403  d.d.l.m.Z...d.d.
 00000040: 6c03 5a03 6401 6403 6c04 5a04 6401 6403  l.Z.d.d.l.Z.d.d.
 00000050: 6c05 5a05 6401 6404 6c06 6d07 5a07 6d08  l.Z.d.d.l.m.Z.m.
 00000060: 5a08 0100 6401 6405 6c09 6d0a 5a0a 0100  Z...d.d.l.m.Z...
 00000070: 6401 6406 6c0b 6d0c 5a0c 6d0d 5a0d 0100  d.d.l.m.Z.m.Z...
```

### Comparing `gskChat-1.0.8/gskChat/Provider/bing/__pycache__/upload_image.cpython-312.pyc` & `gskChat-1.0.9/gskChat/Provider/bing/__pycache__/upload_image.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Sun Mar 24 15:25:23 2024 UTC, .py size: 4746 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: cb0d 0d0a 0000 0000 e345 0066 8a12 0000  .........E.f....
+00000000: cb0d 0d0a 0000 0000 e644 0166 8a12 0000  .........D.f....
 00000010: e300 0000 0000 0000 0000 0000 0004 0000  ................
 00000020: 0000 0000 01f3 bc00 0000 9700 6400 5a00  ............d.Z.
 00000030: 6401 6402 6c01 6d02 5a02 0100 6401 6403  d.d.l.m.Z...d.d.
 00000040: 6c03 5a03 6401 6403 6c04 5a04 6401 6404  l.Z.d.d.l.Z.d.d.
 00000050: 6c05 6d06 5a06 6d07 5a07 0100 6405 6406  l.m.Z.m.Z...d.d.
 00000060: 6c08 6d09 5a09 6d0a 5a0a 0100 6405 6407  l.m.Z.m.Z...d.d.
 00000070: 6c0b 6d0c 5a0c 6d0d 5a0d 6d0e 5a0e 6d0f  l.m.Z.m.Z.m.Z.m.
```

### Comparing `gskChat-1.0.8/gskChat/Provider/bing/conversation.py` & `gskChat-1.0.9/gskChat/Provider/bing/conversation.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.8/gskChat/Provider/bing/create_images.py` & `gskChat-1.0.9/gskChat/Provider/bing/create_images.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.8/gskChat/Provider/bing/upload_image.py` & `gskChat-1.0.9/gskChat/Provider/bing/upload_image.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.8/gskChat/Provider/deprecated/Acytoo.py` & `gskChat-1.0.9/gskChat/Provider/deprecated/Acytoo.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.8/gskChat/Provider/deprecated/AiAsk.py` & `gskChat-1.0.9/gskChat/Provider/deprecated/AiAsk.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.8/gskChat/Provider/deprecated/AiChatOnline.py` & `gskChat-1.0.9/gskChat/Provider/deprecated/AiChatOnline.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.8/gskChat/Provider/deprecated/AiService.py` & `gskChat-1.0.9/gskChat/Provider/deprecated/AiService.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.8/gskChat/Provider/deprecated/Aibn.py` & `gskChat-1.0.9/gskChat/Provider/deprecated/Aibn.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.8/gskChat/Provider/deprecated/Aichat.py` & `gskChat-1.0.9/gskChat/Provider/deprecated/Aichat.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.8/gskChat/Provider/deprecated/Ails.py` & `gskChat-1.0.9/gskChat/Provider/deprecated/Ails.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.8/gskChat/Provider/deprecated/Aivvm.py` & `gskChat-1.0.9/gskChat/Provider/deprecated/Aivvm.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.8/gskChat/Provider/deprecated/Berlin.py` & `gskChat-1.0.9/gskChat/Provider/deprecated/Berlin.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.8/gskChat/Provider/deprecated/ChatAnywhere.py` & `gskChat-1.0.9/gskChat/Provider/deprecated/ChatAnywhere.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.8/gskChat/Provider/deprecated/ChatgptDuo.py` & `gskChat-1.0.9/gskChat/Provider/deprecated/ChatgptDuo.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.8/gskChat/Provider/deprecated/CodeLinkAva.py` & `gskChat-1.0.9/gskChat/Provider/deprecated/CodeLinkAva.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.8/gskChat/Provider/deprecated/Cromicle.py` & `gskChat-1.0.9/gskChat/Provider/deprecated/Cromicle.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.8/gskChat/Provider/deprecated/DfeHub.py` & `gskChat-1.0.9/gskChat/Provider/deprecated/DfeHub.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.8/gskChat/Provider/deprecated/EasyChat.py` & `gskChat-1.0.9/gskChat/Provider/deprecated/EasyChat.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.8/gskChat/Provider/deprecated/Equing.py` & `gskChat-1.0.9/gskChat/Provider/deprecated/Equing.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.8/gskChat/Provider/deprecated/FakeGpt.py` & `gskChat-1.0.9/gskChat/Provider/deprecated/FakeGpt.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.8/gskChat/Provider/deprecated/FastGpt.py` & `gskChat-1.0.9/gskChat/Provider/deprecated/FastGpt.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.8/gskChat/Provider/deprecated/Forefront.py` & `gskChat-1.0.9/gskChat/Provider/deprecated/Forefront.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.8/gskChat/Provider/deprecated/GPTalk.py` & `gskChat-1.0.9/gskChat/Provider/deprecated/GPTalk.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.8/gskChat/Provider/deprecated/GeekGpt.py` & `gskChat-1.0.9/gskChat/Provider/deprecated/GeekGpt.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.8/gskChat/Provider/deprecated/GetGpt.py` & `gskChat-1.0.9/gskChat/Provider/deprecated/GetGpt.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.8/gskChat/Provider/deprecated/H2o.py` & `gskChat-1.0.9/gskChat/Provider/deprecated/H2o.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.8/gskChat/Provider/deprecated/Hashnode.py` & `gskChat-1.0.9/gskChat/Provider/deprecated/Hashnode.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.8/gskChat/Provider/deprecated/Lockchat.py` & `gskChat-1.0.9/gskChat/Provider/deprecated/Lockchat.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.8/gskChat/Provider/deprecated/Myshell.py` & `gskChat-1.0.9/gskChat/Provider/deprecated/Myshell.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.8/gskChat/Provider/deprecated/NoowAi.py` & `gskChat-1.0.9/gskChat/Provider/deprecated/NoowAi.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.8/gskChat/Provider/deprecated/Opchatgpts.py` & `gskChat-1.0.9/gskChat/Provider/deprecated/Opchatgpts.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.8/gskChat/Provider/deprecated/Phind.py` & `gskChat-1.0.9/gskChat/Provider/deprecated/Phind.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.8/gskChat/Provider/deprecated/V50.py` & `gskChat-1.0.9/gskChat/Provider/deprecated/V50.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.8/gskChat/Provider/deprecated/Vercel.py` & `gskChat-1.0.9/gskChat/Provider/deprecated/Vercel.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.8/gskChat/Provider/deprecated/Vitalentum.py` & `gskChat-1.0.9/gskChat/Provider/deprecated/Vitalentum.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.8/gskChat/Provider/deprecated/VoiGpt.py` & `gskChat-1.0.9/gskChat/Provider/deprecated/VoiGpt.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.8/gskChat/Provider/deprecated/Wewordle.py` & `gskChat-1.0.9/gskChat/Provider/deprecated/Wewordle.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.8/gskChat/Provider/deprecated/Wuguokai.py` & `gskChat-1.0.9/gskChat/Provider/deprecated/Wuguokai.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.8/gskChat/Provider/deprecated/Ylokh.py` & `gskChat-1.0.9/gskChat/Provider/deprecated/Ylokh.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.8/gskChat/Provider/deprecated/Yqcloud.py` & `gskChat-1.0.9/gskChat/Provider/deprecated/Yqcloud.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.8/gskChat/Provider/deprecated/__init__.py` & `gskChat-1.0.9/gskChat/Provider/deprecated/__init__.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.8/gskChat/Provider/deprecated/__pycache__/Acytoo.cpython-312.pyc` & `gskChat-1.0.9/gskChat/Provider/deprecated/__pycache__/Acytoo.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Sun Mar 24 15:25:23 2024 UTC, .py size: 1397 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: cb0d 0d0a 0000 0000 e345 0066 7505 0000  .........E.fu...
+00000000: cb0d 0d0a 0000 0000 e644 0166 7505 0000  .........D.fu...
 00000010: e300 0000 0000 0000 0000 0000 0005 0000  ................
 00000020: 0000 0000 01f3 5e00 0000 9700 6400 6401  ......^.....d.d.
 00000030: 6c00 6d01 5a01 0100 6400 6402 6c02 6d03  l.m.Z...d.d.l.m.
 00000040: 5a03 0100 6403 6404 6c04 6d05 5a05 6d06  Z...d.d.l.m.Z.m.
 00000050: 5a06 0100 6405 6406 6c07 6d08 5a08 0100  Z...d.d.l.m.Z...
 00000060: 0200 4700 6407 8400 6408 6508 ab03 0000  ..G.d...d.e.....
 00000070: 0000 0000 5a09 6409 8400 5a0a 640c 640d  ....Z.d...Z.d.d.
```

### Comparing `gskChat-1.0.8/gskChat/Provider/deprecated/__pycache__/AiAsk.cpython-312.pyc` & `gskChat-1.0.9/gskChat/Provider/deprecated/__pycache__/AiAsk.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Sun Mar 24 15:25:23 2024 UTC, .py size: 1669 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: cb0d 0d0a 0000 0000 e345 0066 8506 0000  .........E.f....
+00000000: cb0d 0d0a 0000 0000 e644 0166 8506 0000  .........D.f....
 00000010: e300 0000 0000 0000 0000 0000 0005 0000  ................
 00000020: 0000 0000 01f3 4e00 0000 9700 6400 6401  ......N.....d.d.
 00000030: 6c00 6d01 5a01 0100 6400 6402 6c02 6d03  l.m.Z...d.d.l.m.
 00000040: 5a03 0100 6403 6404 6c04 6d05 5a05 6d06  Z...d.d.l.m.Z.m.
 00000050: 5a06 0100 6405 6406 6c07 6d08 5a08 0100  Z...d.d.l.m.Z...
 00000060: 0200 4700 6407 8400 6408 6508 ab03 0000  ..G.d...d.e.....
 00000070: 0000 0000 5a09 7909 290a e900 0000 0029  ....Z.y.)......)
```

### Comparing `gskChat-1.0.8/gskChat/Provider/deprecated/__pycache__/AiChatOnline.cpython-312.pyc` & `gskChat-1.0.9/gskChat/Provider/deprecated/__pycache__/AiChatOnline.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Sun Mar 24 15:25:23 2024 UTC, .py size: 2196 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: cb0d 0d0a 0000 0000 e345 0066 9408 0000  .........E.f....
+00000000: cb0d 0d0a 0000 0000 e644 0166 9408 0000  .........D.f....
 00000010: e300 0000 0000 0000 0000 0000 0005 0000  ................
 00000020: 0000 0000 01f3 6200 0000 9700 6400 6401  ......b.....d.d.
 00000030: 6c00 6d01 5a01 0100 6400 6402 6c02 5a02  l.m.Z...d.d.l.Z.
 00000040: 6400 6403 6c03 6d04 5a04 0100 6404 6405  d.d.l.m.Z...d.d.
 00000050: 6c05 6d06 5a06 6d07 5a07 0100 6406 6407  l.m.Z.m.Z...d.d.
 00000060: 6c08 6d09 5a09 0100 6406 6408 6c0a 6d0b  l.m.Z...d.d.l.m.
 00000070: 5a0b 0100 0200 4700 6409 8400 640a 6509  Z.....G.d...d.e.
```

### Comparing `gskChat-1.0.8/gskChat/Provider/deprecated/__pycache__/AiService.cpython-312.pyc` & `gskChat-1.0.9/gskChat/Provider/deprecated/__pycache__/AiService.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Sun Mar 24 15:25:23 2024 UTC, .py size: 1148 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: cb0d 0d0a 0000 0000 e345 0066 7c04 0000  .........E.f|...
+00000000: cb0d 0d0a 0000 0000 e644 0166 7c04 0000  .........D.f|...
 00000010: e300 0000 0000 0000 0000 0000 0005 0000  ................
 00000020: 0000 0000 01f3 4e00 0000 9700 6400 6401  ......N.....d.d.
 00000030: 6c00 6d01 5a01 0100 6400 6402 6c02 5a02  l.m.Z...d.d.l.Z.
 00000040: 6403 6404 6c03 6d04 5a04 6d05 5a05 6d06  d.d.l.m.Z.m.Z.m.
 00000050: 5a06 0100 6405 6406 6c07 6d08 5a08 0100  Z...d.d.l.m.Z...
 00000060: 0200 4700 6407 8400 6408 6508 ab03 0000  ..G.d...d.e.....
 00000070: 0000 0000 5a09 7902 2909 e900 0000 0029  ....Z.y.)......)
```

### Comparing `gskChat-1.0.8/gskChat/Provider/deprecated/__pycache__/Aibn.cpython-312.pyc` & `gskChat-1.0.9/gskChat/Provider/deprecated/__pycache__/Aibn.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Sun Mar 24 15:25:23 2024 UTC, .py size: 1396 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: cb0d 0d0a 0000 0000 e345 0066 7405 0000  .........E.ft...
+00000000: cb0d 0d0a 0000 0000 e644 0166 7405 0000  .........D.ft...
 00000010: e300 0000 0000 0000 0000 0000 0005 0000  ................
 00000020: 0000 0000 01f3 6800 0000 9700 6400 6401  ......h.....d.d.
 00000030: 6c00 6d01 5a01 0100 6400 6402 6c02 5a02  l.m.Z...d.d.l.Z.
 00000040: 6400 6402 6c03 5a03 6403 6404 6c04 6d05  d.d.l.Z.d.d.l.m.
 00000050: 5a05 6d06 5a06 0100 6403 6405 6c07 6d08  Z.m.Z...d.d.l.m.
 00000060: 5a08 0100 6406 6407 6c09 6d0a 5a0a 0100  Z...d.d.l.m.Z...
 00000070: 0200 4700 6408 8400 6409 650a ab03 0000  ..G.d...d.e.....
```

### Comparing `gskChat-1.0.8/gskChat/Provider/deprecated/__pycache__/Aichat.cpython-312.pyc` & `gskChat-1.0.9/gskChat/Provider/deprecated/__pycache__/Aichat.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Sun Mar 24 15:25:23 2024 UTC, .py size: 2517 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: cb0d 0d0a 0000 0000 e345 0066 d509 0000  .........E.f....
+00000000: cb0d 0d0a 0000 0000 e644 0166 d509 0000  .........D.f....
 00000010: e300 0000 0000 0000 0000 0000 0005 0000  ................
 00000020: 0000 0000 01f3 5a00 0000 9700 6400 6401  ......Z.....d.d.
 00000030: 6c00 6d01 5a01 0100 6402 6403 6c02 6d03  l.m.Z...d.d.l.m.
 00000040: 5a03 0100 6404 6405 6c04 6d05 5a05 6d06  Z...d.d.l.m.Z.m.
 00000050: 5a06 0100 6404 6406 6c07 6d08 5a08 0100  Z...d.d.l.m.Z...
 00000060: 6402 6407 6c09 6d0a 5a0a 0100 0200 4700  d.d.l.m.Z.....G.
 00000070: 6408 8400 6409 6505 ab03 0000 0000 0000  d...d.e.........
```

### Comparing `gskChat-1.0.8/gskChat/Provider/deprecated/__pycache__/Ails.cpython-312.pyc` & `gskChat-1.0.9/gskChat/Provider/deprecated/__pycache__/Ails.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Sun Mar 24 15:25:23 2024 UTC, .py size: 3358 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: cb0d 0d0a 0000 0000 e345 0066 1e0d 0000  .........E.f....
+00000000: cb0d 0d0a 0000 0000 e644 0166 1e0d 0000  .........D.f....
 00000010: e300 0000 0000 0000 0000 0000 0005 0000  ................
 00000020: 0000 0000 01f3 8e00 0000 9700 6400 6401  ............d.d.
 00000030: 6c00 6d01 5a01 0100 6400 6402 6c02 5a02  l.m.Z...d.d.l.Z.
 00000040: 6400 6402 6c03 5a03 6400 6402 6c04 5a04  d.d.l.Z.d.d.l.Z.
 00000050: 6400 6402 6c05 5a05 6400 6403 6c06 6d06  d.d.l.Z.d.d.l.m.
 00000060: 5a06 0100 6400 6404 6c07 6d08 5a08 0100  Z...d.d.l.m.Z...
 00000070: 6405 6406 6c09 6d0a 5a0a 6d0b 5a0b 6d0c  d.d.l.m.Z.m.Z.m.
```

### Comparing `gskChat-1.0.8/gskChat/Provider/deprecated/__pycache__/Aivvm.cpython-312.pyc` & `gskChat-1.0.9/gskChat/Provider/deprecated/__pycache__/Aivvm.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Sun Mar 24 15:25:23 2024 UTC, .py size: 2952 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: cb0d 0d0a 0000 0000 e345 0066 880b 0000  .........E.f....
+00000000: cb0d 0d0a 0000 0000 e644 0166 880b 0000  .........D.f....
 00000010: e300 0000 0000 0000 0000 0000 000a 0000  ................
 00000020: 0000 0000 01f3 9800 0000 9700 6400 6401  ............d.d.
 00000030: 6c00 6d01 5a01 0100 6400 6402 6c02 5a02  l.m.Z...d.d.l.Z.
 00000040: 6400 6402 6c03 5a03 6403 6404 6c04 6d05  d.d.l.Z.d.d.l.m.
 00000050: 5a05 0100 6405 6406 6c06 6d07 5a07 6d08  Z...d.d.l.m.Z.m.
 00000060: 5a08 0100 6407 6408 6409 9c02 640a 640b  Z...d.d.d...d.d.
 00000070: 6409 9c02 640c 640d 6409 9c02 640e 640f  d...d.d.d...d.d.
```

### Comparing `gskChat-1.0.8/gskChat/Provider/deprecated/__pycache__/Berlin.cpython-312.pyc` & `gskChat-1.0.9/gskChat/Provider/deprecated/__pycache__/Berlin.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Sun Mar 24 15:25:23 2024 UTC, .py size: 2807 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: cb0d 0d0a 0000 0000 e345 0066 f70a 0000  .........E.f....
+00000000: cb0d 0d0a 0000 0000 e644 0166 f70a 0000  .........D.f....
 00000010: e300 0000 0000 0000 0000 0000 0005 0000  ................
 00000020: 0000 0000 01f3 7200 0000 9700 6400 6401  ......r.....d.d.
 00000030: 6c00 6d01 5a01 0100 6400 6402 6c02 5a02  l.m.Z...d.d.l.Z.
 00000040: 6400 6402 6c03 5a03 6400 6402 6c04 5a04  d.d.l.Z.d.d.l.Z.
 00000050: 6400 6403 6c05 6d06 5a06 0100 6404 6405  d.d.l.m.Z...d.d.
 00000060: 6c07 6d08 5a08 6d09 5a09 0100 6406 6407  l.m.Z.m.Z...d.d.
 00000070: 6c0a 6d0b 5a0b 0100 6406 6408 6c0c 6d0d  l.m.Z...d.d.l.m.
```

### Comparing `gskChat-1.0.8/gskChat/Provider/deprecated/__pycache__/ChatAnywhere.cpython-312.pyc` & `gskChat-1.0.9/gskChat/Provider/deprecated/__pycache__/ChatAnywhere.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Sun Mar 24 15:25:23 2024 UTC, .py size: 1934 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: cb0d 0d0a 0000 0000 e345 0066 8e07 0000  .........E.f....
+00000000: cb0d 0d0a 0000 0000 e644 0166 8e07 0000  .........D.f....
 00000010: e300 0000 0000 0000 0000 0000 0005 0000  ................
 00000020: 0000 0000 01f3 5200 0000 9700 6400 6401  ......R.....d.d.
 00000030: 6c00 6d01 5a01 0100 6400 6402 6c02 6d03  l.m.Z...d.d.l.m.
 00000040: 5a03 6d04 5a04 0100 6403 6404 6c05 6d06  Z.m.Z...d.d.l.m.
 00000050: 5a06 6d07 5a07 0100 6405 6406 6c08 6d09  Z.m.Z...d.d.l.m.
 00000060: 5a09 0100 0200 4700 6407 8400 6408 6509  Z.....G.d...d.e.
 00000070: ab03 0000 0000 0000 5a0a 7909 290a e900  ........Z.y.)...
```

### Comparing `gskChat-1.0.8/gskChat/Provider/deprecated/__pycache__/ChatgptDuo.cpython-312.pyc` & `gskChat-1.0.9/gskChat/Provider/deprecated/__pycache__/ChatgptDuo.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Sun Mar 24 15:25:23 2024 UTC, .py size: 1303 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: cb0d 0d0a 0000 0000 e345 0066 1705 0000  .........E.f....
+00000000: cb0d 0d0a 0000 0000 e644 0166 1705 0000  .........D.f....
 00000010: e300 0000 0000 0000 0000 0000 0005 0000  ................
 00000020: 0000 0000 01f3 4e00 0000 9700 6400 6401  ......N.....d.d.
 00000030: 6c00 6d01 5a01 0100 6402 6403 6c02 6d03  l.m.Z...d.d.l.m.
 00000040: 5a03 0100 6402 6404 6c04 6d05 5a05 0100  Z...d.d.l.m.Z...
 00000050: 6405 6406 6c06 6d07 5a07 6d08 5a08 0100  d.d.l.m.Z.m.Z...
 00000060: 0200 4700 6407 8400 6408 6507 ab03 0000  ..G.d...d.e.....
 00000070: 0000 0000 5a09 7909 290a e900 0000 0029  ....Z.y.)......)
```

### Comparing `gskChat-1.0.8/gskChat/Provider/deprecated/__pycache__/CodeLinkAva.cpython-312.pyc` & `gskChat-1.0.9/gskChat/Provider/deprecated/__pycache__/CodeLinkAva.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Sun Mar 24 15:25:23 2024 UTC, .py size: 1873 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: cb0d 0d0a 0000 0000 e345 0066 5107 0000  .........E.fQ...
+00000000: cb0d 0d0a 0000 0000 e644 0166 5107 0000  .........D.fQ...
 00000010: e300 0000 0000 0000 0000 0000 0005 0000  ................
 00000020: 0000 0000 01f3 5200 0000 9700 6400 6401  ......R.....d.d.
 00000030: 6c00 6d01 5a01 0100 6400 6402 6c02 6d03  l.m.Z...d.d.l.m.
 00000040: 5a03 0100 6400 6403 6c04 5a04 6404 6405  Z...d.d.l.Z.d.d.
 00000050: 6c05 6d06 5a06 0100 6406 6407 6c07 6d08  l.m.Z...d.d.l.m.
 00000060: 5a08 0100 0200 4700 6408 8400 6409 6508  Z.....G.d...d.e.
 00000070: ab03 0000 0000 0000 5a09 7903 290a e900  ........Z.y.)...
```

### Comparing `gskChat-1.0.8/gskChat/Provider/deprecated/__pycache__/Cromicle.cpython-312.pyc` & `gskChat-1.0.9/gskChat/Provider/deprecated/__pycache__/Cromicle.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Sun Mar 24 15:25:23 2024 UTC, .py size: 1356 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: cb0d 0d0a 0000 0000 e345 0066 4c05 0000  .........E.fL...
+00000000: cb0d 0d0a 0000 0000 e644 0166 4c05 0000  .........D.fL...
 00000010: e300 0000 0000 0000 0000 0000 0005 0000  ................
 00000020: 0000 0000 01f3 7a00 0000 9700 6400 6401  ......z.....d.d.
 00000030: 6c00 6d01 5a01 0100 6400 6402 6c02 6d03  l.m.Z...d.d.l.m.
 00000040: 5a03 0100 6400 6403 6c04 6d05 5a05 0100  Z...d.d.l.m.Z...
 00000050: 6404 6405 6c06 6d07 5a07 6d08 5a08 6d09  d.d.l.m.Z.m.Z.m.
 00000060: 5a09 0100 6406 6407 6c0a 6d0b 5a0b 0100  Z...d.d.l.m.Z...
 00000070: 6406 6408 6c0c 6d0d 5a0d 0100 0200 4700  d.d.l.m.Z.....G.
```

### Comparing `gskChat-1.0.8/gskChat/Provider/deprecated/__pycache__/DfeHub.cpython-312.pyc` & `gskChat-1.0.9/gskChat/Provider/deprecated/__pycache__/DfeHub.cpython-312.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xcb0d0d0a
-moddate:  0xe3450066 (Sun Mar 24 15:25:23 2024 UTC)
+moddate:  0xe6440166 (Mon Mar 25 09:33:26 2024 UTC)
 files sz: 2498
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 16777216
    code
```

### Comparing `gskChat-1.0.8/gskChat/Provider/deprecated/__pycache__/EasyChat.cpython-312.pyc` & `gskChat-1.0.9/gskChat/Provider/deprecated/__pycache__/EasyChat.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Sun Mar 24 15:25:23 2024 UTC, .py size: 3398 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: cb0d 0d0a 0000 0000 e345 0066 460d 0000  .........E.fF...
+00000000: cb0d 0d0a 0000 0000 e644 0166 460d 0000  .........D.fF...
 00000010: e300 0000 0000 0000 0000 0000 0005 0000  ................
 00000020: 0000 0000 01f3 5a00 0000 9700 6400 6401  ......Z.....d.d.
 00000030: 6c00 6d01 5a01 0100 6400 6402 6c02 5a02  l.m.Z...d.d.l.Z.
 00000040: 6400 6402 6c03 5a03 6400 6402 6c04 5a04  d.d.l.Z.d.d.l.Z.
 00000050: 6403 6404 6c05 6d06 5a06 6d07 5a07 0100  d.d.l.m.Z.m.Z...
 00000060: 6405 6406 6c08 6d09 5a09 0100 0200 4700  d.d.l.m.Z.....G.
 00000070: 6407 8400 6408 6509 ab03 0000 0000 0000  d...d.e.........
```

### Comparing `gskChat-1.0.8/gskChat/Provider/deprecated/__pycache__/Equing.cpython-312.pyc` & `gskChat-1.0.9/gskChat/Provider/deprecated/__pycache__/Equing.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Sun Mar 24 15:25:23 2024 UTC, .py size: 2755 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: cb0d 0d0a 0000 0000 e345 0066 c30a 0000  .........E.f....
+00000000: cb0d 0d0a 0000 0000 e644 0166 c30a 0000  .........D.f....
 00000010: e300 0000 0000 0000 0000 0000 0005 0000  ................
 00000020: 0000 0000 01f3 6200 0000 9700 6400 6401  ......b.....d.d.
 00000030: 6c00 6d01 5a01 0100 6400 6402 6c02 5a02  l.m.Z...d.d.l.Z.
 00000040: 6400 6403 6c03 6d04 5a04 6d05 5a05 0100  d.d.l.m.Z.m.Z...
 00000050: 6400 6402 6c06 5a06 6404 6405 6c07 6d08  d.d.l.Z.d.d.l.m.
 00000060: 5a08 6d09 5a09 0100 6406 6407 6c0a 6d0b  Z.m.Z...d.d.l.m.
 00000070: 5a0b 0100 0200 4700 6408 8400 6409 650b  Z.....G.d...d.e.
```

### Comparing `gskChat-1.0.8/gskChat/Provider/deprecated/__pycache__/FakeGpt.cpython-312.pyc` & `gskChat-1.0.9/gskChat/Provider/deprecated/__pycache__/FakeGpt.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Sun Mar 24 15:25:23 2024 UTC, .py size: 4018 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: cb0d 0d0a 0000 0000 e345 0066 b20f 0000  .........E.f....
+00000000: cb0d 0d0a 0000 0000 e644 0166 b20f 0000  .........D.f....
 00000010: e300 0000 0000 0000 0000 0000 0005 0000  ................
 00000020: 0000 0000 01f3 7e00 0000 9700 6400 6401  ......~.....d.d.
 00000030: 6c00 6d01 5a01 0100 6400 6402 6c02 5a02  l.m.Z...d.d.l.Z.
 00000040: 6400 6402 6c03 5a03 6400 6402 6c04 5a04  d.d.l.Z.d.d.l.Z.
 00000050: 6400 6402 6c05 5a05 6400 6403 6c06 6d07  d.d.l.Z.d.d.l.m.
 00000060: 5a07 0100 6404 6405 6c08 6d09 5a09 6d0a  Z...d.d.l.m.Z.m.
 00000070: 5a0a 0100 6406 6407 6c0b 6d0c 5a0c 0100  Z...d.d.l.m.Z...
```

### Comparing `gskChat-1.0.8/gskChat/Provider/deprecated/__pycache__/FastGpt.cpython-312.pyc` & `gskChat-1.0.9/gskChat/Provider/deprecated/__pycache__/FastGpt.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Sun Mar 24 15:25:23 2024 UTC, .py size: 2929 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: cb0d 0d0a 0000 0000 e345 0066 710b 0000  .........E.fq...
+00000000: cb0d 0d0a 0000 0000 e644 0166 710b 0000  .........D.fq...
 00000010: e300 0000 0000 0000 0000 0000 0005 0000  ................
 00000020: 0000 0000 01f3 5a00 0000 9700 6400 6401  ......Z.....d.d.
 00000030: 6c00 6d01 5a01 0100 6400 6402 6c02 5a02  l.m.Z...d.d.l.Z.
 00000040: 6400 6402 6c03 5a03 6400 6402 6c04 5a04  d.d.l.Z.d.d.l.Z.
 00000050: 6403 6404 6c05 6d06 5a06 6d07 5a07 0100  d.d.l.m.Z.m.Z...
 00000060: 6405 6406 6c08 6d09 5a09 0100 0200 4700  d.d.l.m.Z.....G.
 00000070: 6407 8400 6408 6509 ab03 0000 0000 0000  d...d.e.........
```

### Comparing `gskChat-1.0.8/gskChat/Provider/deprecated/__pycache__/Forefront.cpython-312.pyc` & `gskChat-1.0.9/gskChat/Provider/deprecated/__pycache__/Forefront.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Sun Mar 24 15:25:23 2024 UTC, .py size: 1282 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: cb0d 0d0a 0000 0000 e345 0066 0205 0000  .........E.f....
+00000000: cb0d 0d0a 0000 0000 e644 0166 0205 0000  .........D.f....
 00000010: e300 0000 0000 0000 0000 0000 0005 0000  ................
 00000020: 0000 0000 01f3 5200 0000 9700 6400 6401  ......R.....d.d.
 00000030: 6c00 6d01 5a01 0100 6400 6402 6c02 5a02  l.m.Z...d.d.l.Z.
 00000040: 6400 6402 6c03 5a03 6403 6404 6c04 6d05  d.d.l.Z.d.d.l.m.
 00000050: 5a05 6d06 5a06 0100 6405 6406 6c07 6d08  Z.m.Z...d.d.l.m.
 00000060: 5a08 0100 0200 4700 6407 8400 6408 6508  Z.....G.d...d.e.
 00000070: ab03 0000 0000 0000 5a09 7902 2909 e900  ........Z.y.)...
```

### Comparing `gskChat-1.0.8/gskChat/Provider/deprecated/__pycache__/GPTalk.cpython-312.pyc` & `gskChat-1.0.9/gskChat/Provider/deprecated/__pycache__/GPTalk.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Sun Mar 24 15:25:23 2024 UTC, .py size: 3552 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: cb0d 0d0a 0000 0000 e345 0066 e00d 0000  .........E.f....
+00000000: cb0d 0d0a 0000 0000 e644 0166 e00d 0000  .........D.f....
 00000010: e300 0000 0000 0000 0000 0000 0005 0000  ................
 00000020: 0000 0000 01f3 7200 0000 9700 6400 6401  ......r.....d.d.
 00000030: 6c00 6d01 5a01 0100 6400 6402 6c02 5a02  l.m.Z...d.d.l.Z.
 00000040: 6400 6402 6c03 5a03 6400 6402 6c04 5a04  d.d.l.Z.d.d.l.Z.
 00000050: 6400 6403 6c05 6d06 5a06 0100 6404 6405  d.d.l.m.Z...d.d.
 00000060: 6c07 6d08 5a08 6d09 5a09 0100 6406 6407  l.m.Z.m.Z...d.d.
 00000070: 6c0a 6d0b 5a0b 0100 6406 6408 6c0c 6d0d  l.m.Z...d.d.l.m.
```

### Comparing `gskChat-1.0.8/gskChat/Provider/deprecated/__pycache__/GeekGpt.cpython-312.pyc` & `gskChat-1.0.9/gskChat/Provider/deprecated/__pycache__/GeekGpt.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Sun Mar 24 15:25:23 2024 UTC, .py size: 2658 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: cb0d 0d0a 0000 0000 e345 0066 620a 0000  .........E.fb...
+00000000: cb0d 0d0a 0000 0000 e644 0166 620a 0000  .........D.fb...
 00000010: e300 0000 0000 0000 0000 0000 0005 0000  ................
 00000020: 0000 0000 01f3 5e00 0000 9700 6400 6401  ......^.....d.d.
 00000030: 6c00 6d01 5a01 0100 6400 6402 6c02 5a02  l.m.Z...d.d.l.Z.
 00000040: 6400 6402 6c03 5a03 6403 6404 6c04 6d05  d.d.l.Z.d.d.l.m.
 00000050: 5a05 0100 6405 6406 6c06 6d07 5a07 6d08  Z...d.d.l.m.Z.m.
 00000060: 5a08 0100 6400 6407 6c03 6d09 5a09 0100  Z...d.d.l.m.Z...
 00000070: 0200 4700 6408 8400 6409 6505 ab03 0000  ..G.d...d.e.....
```

### Comparing `gskChat-1.0.8/gskChat/Provider/deprecated/__pycache__/GetGpt.cpython-312.pyc` & `gskChat-1.0.9/gskChat/Provider/deprecated/__pycache__/GetGpt.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Sun Mar 24 15:25:23 2024 UTC, .py size: 2515 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: cb0d 0d0a 0000 0000 e345 0066 d309 0000  .........E.f....
+00000000: cb0d 0d0a 0000 0000 e644 0166 d309 0000  .........D.f....
 00000010: e300 0000 0000 0000 0000 0000 0005 0000  ................
 00000020: 0000 0000 01f3 7200 0000 9700 6400 6401  ......r.....d.d.
 00000030: 6c00 6d01 5a01 0100 6400 6402 6c02 5a02  l.m.Z...d.d.l.Z.
 00000040: 6400 6402 6c03 5a03 6400 6402 6c04 5a04  d.d.l.Z.d.d.l.Z.
 00000050: 6400 6402 6c05 5a05 6403 6404 6c06 6d07  d.d.l.Z.d.d.l.m.
 00000060: 5a07 6d08 5a08 0100 6405 6406 6c09 6d0a  Z.m.Z...d.d.l.m.
 00000070: 5a0a 0100 0200 4700 6407 8400 6408 650a  Z.....G.d...d.e.
```

### Comparing `gskChat-1.0.8/gskChat/Provider/deprecated/__pycache__/H2o.cpython-312.pyc` & `gskChat-1.0.9/gskChat/Provider/deprecated/__pycache__/H2o.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Sun Mar 24 15:25:23 2024 UTC, .py size: 2925 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: cb0d 0d0a 0000 0000 e345 0066 6d0b 0000  .........E.fm...
+00000000: cb0d 0d0a 0000 0000 e644 0166 6d0b 0000  .........D.fm...
 00000010: e300 0000 0000 0000 0000 0000 0005 0000  ................
 00000020: 0000 0000 01f3 6200 0000 9700 6400 6401  ......b.....d.d.
 00000030: 6c00 6d01 5a01 0100 6400 6402 6c02 5a02  l.m.Z...d.d.l.Z.
 00000040: 6400 6402 6c03 5a03 6400 6403 6c04 6d05  d.d.l.Z.d.d.l.m.
 00000050: 5a05 0100 6404 6405 6c06 6d07 5a07 6d08  Z...d.d.l.m.Z.m.
 00000060: 5a08 0100 6406 6407 6c09 6d0a 5a0a 6d0b  Z...d.d.l.m.Z.m.
 00000070: 5a0b 0100 0200 4700 6408 8400 6409 650a  Z.....G.d...d.e.
```

### Comparing `gskChat-1.0.8/gskChat/Provider/deprecated/__pycache__/Hashnode.cpython-312.pyc` & `gskChat-1.0.9/gskChat/Provider/deprecated/__pycache__/Hashnode.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Sun Mar 24 15:25:23 2024 UTC, .py size: 2674 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: cb0d 0d0a 0000 0000 e345 0066 720a 0000  .........E.fr...
+00000000: cb0d 0d0a 0000 0000 e644 0166 720a 0000  .........D.fr...
 00000010: e300 0000 0000 0000 0000 0000 0005 0000  ................
 00000020: 0000 0000 01f3 6e00 0000 9700 6400 6401  ......n.....d.d.
 00000030: 6c00 6d01 5a01 0100 6400 6402 6c02 6d03  l.m.Z...d.d.l.m.
 00000040: 5a03 0100 6403 6404 6c04 6d05 5a05 6d06  Z...d.d.l.m.Z.m.
 00000050: 5a06 0100 6405 6406 6c07 6d08 5a08 0100  Z...d.d.l.m.Z...
 00000060: 6405 6407 6c09 6d0a 5a0a 0100 0200 4700  d.d.l.m.Z.....G.
 00000070: 6408 8400 6409 ab02 0000 0000 0000 5a0b  d...d.........Z.
```

### Comparing `gskChat-1.0.8/gskChat/Provider/deprecated/__pycache__/Lockchat.cpython-312.pyc` & `gskChat-1.0.9/gskChat/Provider/deprecated/__pycache__/Lockchat.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Sun Mar 24 15:25:23 2024 UTC, .py size: 1700 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: cb0d 0d0a 0000 0000 e345 0066 a406 0000  .........E.f....
+00000000: cb0d 0d0a 0000 0000 e644 0166 a406 0000  .........D.f....
 00000010: e300 0000 0000 0000 0000 0000 0005 0000  ................
 00000020: 0000 0000 01f3 5200 0000 9700 6400 6401  ......R.....d.d.
 00000030: 6c00 6d01 5a01 0100 6400 6402 6c02 5a02  l.m.Z...d.d.l.Z.
 00000040: 6400 6402 6c03 5a03 6403 6404 6c04 6d05  d.d.l.Z.d.d.l.m.
 00000050: 5a05 6d06 5a06 0100 6405 6406 6c07 6d08  Z.m.Z...d.d.l.m.
 00000060: 5a08 0100 0200 4700 6407 8400 6408 6508  Z.....G.d...d.e.
 00000070: ab03 0000 0000 0000 5a09 7902 2909 e900  ........Z.y.)...
```

### Comparing `gskChat-1.0.8/gskChat/Provider/deprecated/__pycache__/Myshell.cpython-312.pyc` & `gskChat-1.0.9/gskChat/Provider/deprecated/__pycache__/Myshell.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Sun Mar 24 15:25:23 2024 UTC, .py size: 5050 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: cb0d 0d0a 0000 0000 e345 0066 ba13 0000  .........E.f....
+00000000: cb0d 0d0a 0000 0000 e644 0166 ba13 0000  .........D.f....
 00000010: e300 0000 0000 0000 0000 0000 0005 0000  ................
 00000020: 0000 0000 01f3 c200 0000 9700 6400 6401  ............d.d.
 00000030: 6c00 6d01 5a01 0100 6400 6402 6c02 5a02  l.m.Z...d.d.l.Z.
 00000040: 6400 6402 6c03 5a03 6400 6402 6c04 5a04  d.d.l.Z.d.d.l.Z.
 00000050: 6400 6402 6c05 5a05 6400 6402 6c06 5a06  d.d.l.Z.d.d.l.Z.
 00000060: 6400 6403 6c07 6d08 5a08 0100 6400 6404  d.d.l.m.Z...d.d.
 00000070: 6c09 6d0a 5a0a 0100 6400 6402 6c0b 5a0b  l.m.Z...d.d.l.Z.
```

### Comparing `gskChat-1.0.8/gskChat/Provider/deprecated/__pycache__/NoowAi.cpython-312.pyc` & `gskChat-1.0.9/gskChat/Provider/deprecated/__pycache__/NoowAi.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Sun Mar 24 15:25:23 2024 UTC, .py size: 2500 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: cb0d 0d0a 0000 0000 e345 0066 c409 0000  .........E.f....
+00000000: cb0d 0d0a 0000 0000 e644 0166 c409 0000  .........D.f....
 00000010: e300 0000 0000 0000 0000 0000 0005 0000  ................
 00000020: 0000 0000 01f3 6200 0000 9700 6400 6401  ......b.....d.d.
 00000030: 6c00 6d01 5a01 0100 6400 6402 6c02 5a02  l.m.Z...d.d.l.Z.
 00000040: 6400 6403 6c03 6d04 5a04 0100 6404 6405  d.d.l.m.Z...d.d.
 00000050: 6c05 6d06 5a06 6d07 5a07 0100 6406 6407  l.m.Z.m.Z...d.d.
 00000060: 6c08 6d09 5a09 0100 6406 6408 6c0a 6d0b  l.m.Z...d.d.l.m.
 00000070: 5a0b 0100 0200 4700 6409 8400 640a 6509  Z.....G.d...d.e.
```

### Comparing `gskChat-1.0.8/gskChat/Provider/deprecated/__pycache__/Opchatgpts.cpython-312.pyc` & `gskChat-1.0.9/gskChat/Provider/deprecated/__pycache__/Opchatgpts.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Sun Mar 24 15:25:23 2024 UTC, .py size: 2287 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: cb0d 0d0a 0000 0000 e345 0066 ef08 0000  .........E.f....
+00000000: cb0d 0d0a 0000 0000 e644 0166 ef08 0000  .........D.f....
 00000010: e300 0000 0000 0000 0000 0000 0005 0000  ................
 00000020: 0000 0000 01f3 7200 0000 9700 6400 6401  ......r.....d.d.
 00000030: 6c00 6d01 5a01 0100 6400 6402 6c02 5a02  l.m.Z...d.d.l.Z.
 00000040: 6400 6402 6c03 5a03 6400 6402 6c04 5a04  d.d.l.Z.d.d.l.Z.
 00000050: 6400 6403 6c05 6d06 5a06 0100 6404 6405  d.d.l.m.Z...d.d.
 00000060: 6c07 6d08 5a08 6d09 5a09 0100 6406 6407  l.m.Z.m.Z...d.d.
 00000070: 6c0a 6d0b 5a0b 0100 6406 6408 6c0c 6d0d  l.m.Z...d.d.l.m.
```

### Comparing `gskChat-1.0.8/gskChat/Provider/deprecated/__pycache__/Phind.cpython-312.pyc` & `gskChat-1.0.9/gskChat/Provider/deprecated/__pycache__/Phind.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Sun Mar 24 15:25:23 2024 UTC, .py size: 5353 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: cb0d 0d0a 0000 0000 e345 0066 e914 0000  .........E.f....
+00000000: cb0d 0d0a 0000 0000 e644 0166 e914 0000  .........D.f....
 00000010: e300 0000 0000 0000 0000 0000 0005 0000  ................
 00000020: 0000 0000 01f3 9400 0000 9700 6400 6401  ............d.d.
 00000030: 6c00 6d01 5a01 0100 6400 6402 6c02 5a02  l.m.Z...d.d.l.Z.
 00000040: 6400 6402 6c03 5a03 6400 6403 6c04 6d05  d.d.l.Z.d.d.l.m.
 00000050: 5a05 0100 6400 6404 6c06 6d06 5a06 0100  Z...d.d.l.m.Z...
 00000060: 6405 6406 6c07 6d08 5a08 6d09 5a09 0100  d.d.l.m.Z.m.Z...
 00000070: 6407 6408 6c0a 6d0b 5a0b 0100 6405 6409  d.d.l.m.Z...d.d.
```

### Comparing `gskChat-1.0.8/gskChat/Provider/deprecated/__pycache__/V50.cpython-312.pyc` & `gskChat-1.0.9/gskChat/Provider/deprecated/__pycache__/V50.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Sun Mar 24 15:25:23 2024 UTC, .py size: 2077 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: cb0d 0d0a 0000 0000 e345 0066 1d08 0000  .........E.f....
+00000000: cb0d 0d0a 0000 0000 e644 0166 1d08 0000  .........D.f....
 00000010: e300 0000 0000 0000 0000 0000 0005 0000  ................
 00000020: 0000 0000 01f3 5200 0000 9700 6400 6401  ......R.....d.d.
 00000030: 6c00 6d01 5a01 0100 6400 6402 6c02 5a02  l.m.Z...d.d.l.Z.
 00000040: 6400 6402 6c03 5a03 6403 6404 6c04 6d05  d.d.l.Z.d.d.l.m.
 00000050: 5a05 6d06 5a06 0100 6405 6406 6c07 6d08  Z.m.Z...d.d.l.m.
 00000060: 5a08 0100 0200 4700 6407 8400 6408 6508  Z.....G.d...d.e.
 00000070: ab03 0000 0000 0000 5a09 7902 2909 e900  ........Z.y.)...
```

### Comparing `gskChat-1.0.8/gskChat/Provider/deprecated/__pycache__/Vercel.cpython-312.pyc` & `gskChat-1.0.9/gskChat/Provider/deprecated/__pycache__/Vercel.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Sun Mar 24 15:25:23 2024 UTC, .py size: 12167 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: cb0d 0d0a 0000 0000 e345 0066 872f 0000  .........E.f./..
+00000000: cb0d 0d0a 0000 0000 e644 0166 872f 0000  .........D.f./..
 00000010: e300 0000 0000 0000 0000 0000 000c 0000  ................
 00000020: 0000 0000 01f3 d602 0000 9700 5500 6400  ............U.d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 5a02 6400 6402 6c03 5a03 6400 6402 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 5a04 6400 6402 6c05 5a05 6400 6402 6c06  Z.d.d.l.Z.d.d.l.
 00000060: 5a06 0900 6400 6402 6c07 5a07 6403 5a08  Z...d.d.l.Z.d.Z.
 00000070: 6405 6406 6c0a 6d0b 5a0b 6d0c 5a0c 6d0d  d.d.l.m.Z.m.Z.m.
```

### Comparing `gskChat-1.0.8/gskChat/Provider/deprecated/__pycache__/Vitalentum.cpython-312.pyc` & `gskChat-1.0.9/gskChat/Provider/deprecated/__pycache__/Vitalentum.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Sun Mar 24 15:25:23 2024 UTC, .py size: 1964 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: cb0d 0d0a 0000 0000 e345 0066 ac07 0000  .........E.f....
+00000000: cb0d 0d0a 0000 0000 e644 0166 ac07 0000  .........D.f....
 00000010: e300 0000 0000 0000 0000 0000 0005 0000  ................
 00000020: 0000 0000 01f3 5600 0000 9700 6400 6401  ......V.....d.d.
 00000030: 6c00 6d01 5a01 0100 6400 6402 6c02 5a02  l.m.Z...d.d.l.Z.
 00000040: 6400 6403 6c03 6d04 5a04 0100 6404 6405  d.d.l.m.Z...d.d.
 00000050: 6c05 6d06 5a06 0100 6406 6407 6c07 6d08  l.m.Z...d.d.l.m.
 00000060: 5a08 6d09 5a09 0100 0200 4700 6408 8400  Z.m.Z.....G.d...
 00000070: 6409 6506 ab03 0000 0000 0000 5a0a 7902  d.e.........Z.y.
```

### Comparing `gskChat-1.0.8/gskChat/Provider/deprecated/__pycache__/VoiGpt.cpython-312.pyc` & `gskChat-1.0.9/gskChat/Provider/deprecated/__pycache__/VoiGpt.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Sun Mar 24 15:25:23 2024 UTC, .py size: 3415 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: cb0d 0d0a 0000 0000 e345 0066 570d 0000  .........E.fW...
+00000000: cb0d 0d0a 0000 0000 e644 0166 570d 0000  .........D.fW...
 00000010: e300 0000 0000 0000 0000 0000 0005 0000  ................
 00000020: 0000 0000 01f3 5200 0000 9700 6400 6401  ......R.....d.d.
 00000030: 6c00 6d01 5a01 0100 6400 6402 6c02 5a02  l.m.Z...d.d.l.Z.
 00000040: 6400 6402 6c03 5a03 6403 6404 6c04 6d05  d.d.l.Z.d.d.l.m.
 00000050: 5a05 0100 6405 6406 6c06 6d07 5a07 6d08  Z...d.d.l.m.Z.m.
 00000060: 5a08 0100 0200 4700 6407 8400 6408 6505  Z.....G.d...d.e.
 00000070: ab03 0000 0000 0000 5a09 7902 2909 e900  ........Z.y.)...
```

### Comparing `gskChat-1.0.8/gskChat/Provider/deprecated/__pycache__/Wewordle.cpython-312.pyc` & `gskChat-1.0.9/gskChat/Provider/deprecated/__pycache__/Wewordle.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Sun Mar 24 15:25:23 2024 UTC, .py size: 2464 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: cb0d 0d0a 0000 0000 e345 0066 a009 0000  .........E.f....
+00000000: cb0d 0d0a 0000 0000 e644 0166 a009 0000  .........D.f....
 00000010: e300 0000 0000 0000 0000 0000 0005 0000  ................
 00000020: 0000 0000 01f3 5600 0000 9700 6400 6401  ......V.....d.d.
 00000030: 6c00 6d01 5a01 0100 6400 6402 6c02 5a02  l.m.Z...d.d.l.Z.
 00000040: 6400 6402 6c03 5a03 6400 6402 6c04 5a04  d.d.l.Z.d.d.l.Z.
 00000050: 6400 6403 6c05 6d06 5a06 0100 6404 6405  d.d.l.m.Z...d.d.
 00000060: 6c07 6d08 5a08 0100 0200 4700 6406 8400  l.m.Z.....G.d...
 00000070: 6407 6508 ab03 0000 0000 0000 5a09 7902  d.e.........Z.y.
```

### Comparing `gskChat-1.0.8/gskChat/Provider/deprecated/__pycache__/Wuguokai.cpython-312.pyc` & `gskChat-1.0.9/gskChat/Provider/deprecated/__pycache__/Wuguokai.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Sun Mar 24 15:25:23 2024 UTC, .py size: 2020 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: cb0d 0d0a 0000 0000 e345 0066 e407 0000  .........E.f....
+00000000: cb0d 0d0a 0000 0000 e644 0166 e407 0000  .........D.f....
 00000010: e300 0000 0000 0000 0000 0000 0005 0000  ................
 00000020: 0000 0000 01f3 5600 0000 9700 6400 6401  ......V.....d.d.
 00000030: 6c00 6d01 5a01 0100 6400 6402 6c02 5a02  l.m.Z...d.d.l.Z.
 00000040: 6400 6402 6c03 5a03 6403 6404 6c04 6d05  d.d.l.Z.d.d.l.m.
 00000050: 5a05 6d06 5a06 0100 6405 6406 6c07 6d08  Z.m.Z...d.d.l.m.
 00000060: 5a08 6d09 5a09 0100 0200 4700 6407 8400  Z.m.Z.....G.d...
 00000070: 6408 6508 ab03 0000 0000 0000 5a0a 7902  d.e.........Z.y.
```

### Comparing `gskChat-1.0.8/gskChat/Provider/deprecated/__pycache__/Ylokh.cpython-312.pyc` & `gskChat-1.0.9/gskChat/Provider/deprecated/__pycache__/Ylokh.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Sun Mar 24 15:25:23 2024 UTC, .py size: 1976 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: cb0d 0d0a 0000 0000 e345 0066 b807 0000  .........E.f....
+00000000: cb0d 0d0a 0000 0000 e644 0166 b807 0000  .........D.f....
 00000010: e300 0000 0000 0000 0000 0000 0005 0000  ................
 00000020: 0000 0000 01f3 5600 0000 9700 6400 6401  ......V.....d.d.
 00000030: 6c00 6d01 5a01 0100 6400 6402 6c02 5a02  l.m.Z...d.d.l.Z.
 00000040: 6403 6404 6c03 6d04 5a04 0100 6405 6406  d.d.l.m.Z...d.d.
 00000050: 6c05 6d06 5a06 0100 6403 6407 6c07 6d08  l.m.Z...d.d.l.m.
 00000060: 5a08 6d09 5a09 0100 0200 4700 6408 8400  Z.m.Z.....G.d...
 00000070: 6409 6506 ab03 0000 0000 0000 5a0a 7902  d.e.........Z.y.
```

### Comparing `gskChat-1.0.8/gskChat/Provider/deprecated/__pycache__/Yqcloud.cpython-312.pyc` & `gskChat-1.0.9/gskChat/Provider/deprecated/__pycache__/Yqcloud.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Sun Mar 24 15:25:23 2024 UTC, .py size: 1922 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: cb0d 0d0a 0000 0000 e345 0066 8207 0000  .........E.f....
+00000000: cb0d 0d0a 0000 0000 e644 0166 8207 0000  .........D.f....
 00000010: e300 0000 0000 0000 0000 0000 0005 0000  ................
 00000020: 0000 0000 01f3 7800 0000 9700 6400 6401  ......x.....d.d.
 00000030: 6c00 6d01 5a01 0100 6400 6402 6c02 5a02  l.m.Z...d.d.l.Z.
 00000040: 6403 6404 6c03 6d04 5a04 0100 6403 6405  d.d.l.m.Z...d.d.
 00000050: 6c05 6d06 5a06 6d07 5a07 0100 6406 6407  l.m.Z.m.Z...d.d.
 00000060: 6c08 6d09 5a09 6d0a 5a0a 0100 0200 4700  l.m.Z.m.Z.....G.
 00000070: 6408 8400 6409 6509 ab03 0000 0000 0000  d...d.e.........
```

### Comparing `gskChat-1.0.8/gskChat/Provider/deprecated/__pycache__/__init__.cpython-312.pyc` & `gskChat-1.0.9/gskChat/Provider/deprecated/__pycache__/__init__.cpython-312.pyc`

 * *Files 12% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xcb0d0d0a
-moddate:  0xe3450066 (Sun Mar 24 15:25:23 2024 UTC)
+moddate:  0xe6440166 (Mon Mar 25 09:33:26 2024 UTC)
 files sz: 1194
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 2
    flags     : 0
    code
```

### Comparing `gskChat-1.0.8/gskChat/Provider/gigachat_crt/russian_trusted_root_ca_pem.crt` & `gskChat-1.0.9/gskChat/Provider/gigachat_crt/russian_trusted_root_ca_pem.crt`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.8/gskChat/Provider/needs_auth/Gemini.py` & `gskChat-1.0.9/gskChat/Provider/needs_auth/Gemini.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.8/gskChat/Provider/needs_auth/OpenAssistant.py` & `gskChat-1.0.9/gskChat/Provider/needs_auth/OpenAssistant.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.8/gskChat/Provider/needs_auth/OpenaiChat.py` & `gskChat-1.0.9/gskChat/Provider/needs_auth/OpenaiChat.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.8/gskChat/Provider/needs_auth/Poe.py` & `gskChat-1.0.9/gskChat/Provider/needs_auth/Poe.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.8/gskChat/Provider/needs_auth/Raycast.py` & `gskChat-1.0.9/gskChat/Provider/needs_auth/Raycast.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.8/gskChat/Provider/needs_auth/Theb.py` & `gskChat-1.0.9/gskChat/Provider/needs_auth/Theb.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.8/gskChat/Provider/needs_auth/ThebApi.py` & `gskChat-1.0.9/gskChat/Provider/needs_auth/ThebApi.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.8/gskChat/Provider/needs_auth/__pycache__/Gemini.cpython-312.pyc` & `gskChat-1.0.9/gskChat/Provider/needs_auth/__pycache__/Gemini.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Sun Mar 24 15:25:23 2024 UTC, .py size: 8145 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: cb0d 0d0a 0000 0000 e345 0066 d11f 0000  .........E.f....
+00000000: cb0d 0d0a 0000 0000 e644 0166 d11f 0000  .........D.f....
 00000010: e300 0000 0000 0000 0000 0000 000d 0000  ................
 00000020: 0000 0000 01f3 2c01 0000 9700 6400 6401  ......,.....d.d.
 00000030: 6c00 6d01 5a01 0100 6400 6402 6c02 5a02  l.m.Z...d.d.l.Z.
 00000040: 6400 6402 6c03 5a03 6400 6402 6c04 5a04  d.d.l.Z.d.d.l.Z.
 00000050: 6400 6402 6c05 5a05 6400 6403 6c06 6d07  d.d.l.Z.d.d.l.m.
 00000060: 5a07 0100 0900 6400 6404 6c08 6d09 5a09  Z.....d.d.l.m.Z.
 00000070: 0100 6400 6405 6c0a 6d0b 5a0b 0100 6400  ..d.d.l.m.Z...d.
```

### Comparing `gskChat-1.0.8/gskChat/Provider/needs_auth/__pycache__/OpenAssistant.cpython-312.pyc` & `gskChat-1.0.9/gskChat/Provider/needs_auth/__pycache__/OpenAssistant.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Sun Mar 24 15:25:23 2024 UTC, .py size: 3309 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: cb0d 0d0a 0000 0000 e345 0066 ed0c 0000  .........E.f....
+00000000: cb0d 0d0a 0000 0000 e644 0166 ed0c 0000  .........D.f....
 00000010: e300 0000 0000 0000 0000 0000 0005 0000  ................
 00000020: 0000 0000 01f3 6600 0000 9700 6400 6401  ......f.....d.d.
 00000030: 6c00 6d01 5a01 0100 6400 6402 6c02 5a02  l.m.Z...d.d.l.Z.
 00000040: 6400 6403 6c03 6d04 5a04 0100 6404 6405  d.d.l.m.Z...d.d.
 00000050: 6c05 6d06 5a06 6d07 5a07 0100 6406 6407  l.m.Z.m.Z...d.d.
 00000060: 6c08 6d09 5a09 0100 6406 6408 6c0a 6d0b  l.m.Z...d.d.l.m.
 00000070: 5a0b 6d0c 5a0c 0100 0200 4700 6409 8400  Z.m.Z.....G.d...
```

### Comparing `gskChat-1.0.8/gskChat/Provider/needs_auth/__pycache__/OpenaiChat.cpython-312.pyc` & `gskChat-1.0.9/gskChat/Provider/needs_auth/__pycache__/OpenaiChat.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Sun Mar 24 15:25:23 2024 UTC, .py size: 30868 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: cb0d 0d0a 0000 0000 e345 0066 9478 0000  .........E.f.x..
+00000000: cb0d 0d0a 0000 0000 e644 0166 9478 0000  .........D.f.x..
 00000010: e300 0000 0000 0000 0000 0000 0006 0000  ................
 00000020: 0000 0000 01f3 b801 0000 9700 6400 6401  ............d.d.
 00000030: 6c00 6d01 5a01 0100 6400 6402 6c02 5a02  l.m.Z...d.d.l.Z.
 00000040: 6400 6402 6c03 5a03 6400 6402 6c04 5a04  d.d.l.Z.d.d.l.Z.
 00000050: 6400 6402 6c05 5a05 6400 6402 6c06 5a06  d.d.l.Z.d.d.l.Z.
 00000060: 6400 6402 6c07 5a07 6400 6403 6c08 6d09  d.d.l.Z.d.d.l.m.
 00000070: 5a09 0100 0900 6400 6404 6c0a 6d0b 5a0b  Z.....d.d.l.m.Z.
```

### Comparing `gskChat-1.0.8/gskChat/Provider/needs_auth/__pycache__/Poe.cpython-312.pyc` & `gskChat-1.0.9/gskChat/Provider/needs_auth/__pycache__/Poe.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Sun Mar 24 15:25:23 2024 UTC, .py size: 4289 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: cb0d 0d0a 0000 0000 e345 0066 c110 0000  .........E.f....
+00000000: cb0d 0d0a 0000 0000 e644 0166 c110 0000  .........D.f....
 00000010: e300 0000 0000 0000 0000 0000 000b 0000  ................
 00000020: 0000 0000 01f3 ac00 0000 9700 6400 6401  ............d.d.
 00000030: 6c00 6d01 5a01 0100 6400 6402 6c02 5a02  l.m.Z...d.d.l.Z.
 00000040: 6403 6404 6c03 6d04 5a04 6d05 5a05 0100  d.d.l.m.Z.m.Z...
 00000050: 6405 6406 6c06 6d07 5a07 0100 6405 6407  d.d.l.m.Z...d.d.
 00000060: 6c08 6d09 5a09 0100 6403 6408 6c0a 6d0b  l.m.Z...d.d.l.m.
 00000070: 5a0b 6d0c 5a0c 6d0d 5a0d 0100 6409 640a  Z.m.Z.m.Z...d.d.
```

### Comparing `gskChat-1.0.8/gskChat/Provider/needs_auth/__pycache__/Raycast.cpython-312.pyc` & `gskChat-1.0.9/gskChat/Provider/needs_auth/__pycache__/Raycast.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Sun Mar 24 15:25:23 2024 UTC, .py size: 1897 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: cb0d 0d0a 0000 0000 e345 0066 6907 0000  .........E.fi...
+00000000: cb0d 0d0a 0000 0000 e644 0166 6907 0000  .........D.fi...
 00000010: e300 0000 0000 0000 0000 0000 0005 0000  ................
 00000020: 0000 0000 01f3 5200 0000 9700 6400 6401  ......R.....d.d.
 00000030: 6c00 6d01 5a01 0100 6400 6402 6c02 5a02  l.m.Z...d.d.l.Z.
 00000040: 6400 6402 6c03 5a03 6403 6404 6c04 6d05  d.d.l.Z.d.d.l.m.
 00000050: 5a05 6d06 5a06 0100 6405 6406 6c07 6d08  Z.m.Z...d.d.l.m.
 00000060: 5a08 0100 0200 4700 6407 8400 6408 6508  Z.....G.d...d.e.
 00000070: ab03 0000 0000 0000 5a09 7902 2909 e900  ........Z.y.)...
```

### Comparing `gskChat-1.0.8/gskChat/Provider/needs_auth/__pycache__/Theb.cpython-312.pyc` & `gskChat-1.0.9/gskChat/Provider/needs_auth/__pycache__/Theb.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Sun Mar 24 15:25:23 2024 UTC, .py size: 5465 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: cb0d 0d0a 0000 0000 e345 0066 5915 0000  .........E.fY...
+00000000: cb0d 0d0a 0000 0000 e644 0166 5915 0000  .........D.fY...
 00000010: e300 0000 0000 0000 0000 0000 0006 0000  ................
 00000020: 0000 0000 01f3 e200 0000 9700 6400 6401  ............d.d.
 00000030: 6c00 6d01 5a01 0100 6400 6402 6c02 5a02  l.m.Z...d.d.l.Z.
 00000040: 6403 6404 6c03 6d04 5a04 6d05 5a05 0100  d.d.l.m.Z.m.Z...
 00000050: 6405 6406 6c06 6d07 5a07 0100 6405 6407  d.d.l.m.Z...d.d.
 00000060: 6c08 6d09 5a09 0100 6403 6408 6c0a 6d0b  l.m.Z...d.d.l.m.
 00000070: 5a0b 6d0c 5a0c 6d0d 5a0d 0100 6900 6409  Z.m.Z.m.Z...i.d.
```

### Comparing `gskChat-1.0.8/gskChat/Provider/needs_auth/__pycache__/ThebApi.cpython-312.pyc` & `gskChat-1.0.9/gskChat/Provider/needs_auth/__pycache__/ThebApi.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Sun Mar 24 15:25:23 2024 UTC, .py size: 2655 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: cb0d 0d0a 0000 0000 e345 0066 5f0a 0000  .........E.f_...
+00000000: cb0d 0d0a 0000 0000 e644 0166 5f0a 0000  .........D.f_...
 00000010: e300 0000 0000 0000 0000 0000 0006 0000  ................
 00000020: 0000 0000 01f3 d800 0000 9700 6400 6401  ............d.d.
 00000030: 6c00 6d01 5a01 0100 6400 6402 6c02 5a02  l.m.Z...d.d.l.Z.
 00000040: 6403 6404 6c03 6d04 5a04 6d05 5a05 6d06  d.d.l.m.Z.m.Z.m.
 00000050: 5a06 0100 6405 6406 6c07 6d08 5a08 6d09  Z...d.d.l.m.Z.m.
 00000060: 5a09 0100 6403 6407 6c0a 6d0b 5a0b 0100  Z...d.d.l.m.Z...
 00000070: 6900 6408 6409 9301 640a 640b 9301 640c  i.d.d...d.d...d.
```

### Comparing `gskChat-1.0.8/gskChat/Provider/not_working/AItianhu.py` & `gskChat-1.0.9/gskChat/Provider/not_working/AItianhu.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.8/gskChat/Provider/not_working/Bestim.py` & `gskChat-1.0.9/gskChat/Provider/not_working/Bestim.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.8/gskChat/Provider/not_working/ChatBase.py` & `gskChat-1.0.9/gskChat/Provider/not_working/ChatBase.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.8/gskChat/Provider/not_working/ChatgptDemo.py` & `gskChat-1.0.9/gskChat/Provider/not_working/ChatgptDemo.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.8/gskChat/Provider/not_working/ChatgptDemoAi.py` & `gskChat-1.0.9/gskChat/Provider/not_working/ChatgptDemoAi.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.8/gskChat/Provider/not_working/ChatgptLogin.py` & `gskChat-1.0.9/gskChat/Provider/not_working/ChatgptLogin.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.8/gskChat/Provider/not_working/Chatxyz.py` & `gskChat-1.0.9/gskChat/Provider/not_working/Chatxyz.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.8/gskChat/Provider/not_working/Gpt6.py` & `gskChat-1.0.9/gskChat/Provider/not_working/Gpt6.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.8/gskChat/Provider/not_working/GptChatly.py` & `gskChat-1.0.9/gskChat/Provider/not_working/GptChatly.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.8/gskChat/Provider/not_working/GptForLove.py` & `gskChat-1.0.9/gskChat/Provider/not_working/GptForLove.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.8/gskChat/Provider/not_working/GptGo.py` & `gskChat-1.0.9/gskChat/Provider/not_working/GptGo.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.8/gskChat/Provider/not_working/GptGod.py` & `gskChat-1.0.9/gskChat/Provider/not_working/GptGod.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.8/gskChat/Provider/not_working/OnlineGpt.py` & `gskChat-1.0.9/gskChat/Provider/not_working/OnlineGpt.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.8/gskChat/Provider/not_working/__pycache__/AItianhu.cpython-312.pyc` & `gskChat-1.0.9/gskChat/Provider/not_working/__pycache__/AItianhu.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Sun Mar 24 15:25:23 2024 UTC, .py size: 3106 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: cb0d 0d0a 0000 0000 e345 0066 220c 0000  .........E.f"...
+00000000: cb0d 0d0a 0000 0000 e644 0166 220c 0000  .........D.f"...
 00000010: e300 0000 0000 0000 0000 0000 0005 0000  ................
 00000020: 0000 0000 01f3 5e00 0000 9700 6400 6401  ......^.....d.d.
 00000030: 6c00 6d01 5a01 0100 6400 6402 6c02 5a02  l.m.Z...d.d.l.Z.
 00000040: 6403 6404 6c03 6d04 5a04 6d05 5a05 0100  d.d.l.m.Z.m.Z...
 00000050: 6403 6405 6c06 6d07 5a07 0100 6406 6407  d.d.l.m.Z...d.d.
 00000060: 6c08 6d09 5a09 6d0a 5a0a 6d0b 5a0b 0100  l.m.Z.m.Z.m.Z...
 00000070: 0200 4700 6408 8400 6409 6509 ab03 0000  ..G.d...d.e.....
```

### Comparing `gskChat-1.0.8/gskChat/Provider/not_working/__pycache__/Bestim.cpython-312.pyc` & `gskChat-1.0.9/gskChat/Provider/not_working/__pycache__/Bestim.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Sun Mar 24 15:25:23 2024 UTC, .py size: 1432 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: cb0d 0d0a 0000 0000 e345 0066 9805 0000  .........E.f....
+00000000: cb0d 0d0a 0000 0000 e644 0166 9805 0000  .........D.f....
 00000010: e300 0000 0000 0000 0000 0000 0005 0000  ................
 00000020: 0000 0000 01f3 5a00 0000 9700 6400 6401  ......Z.....d.d.
 00000030: 6c00 6d01 5a01 0100 6402 6403 6c02 6d03  l.m.Z...d.d.l.m.
 00000040: 5a03 0100 6404 6405 6c04 6d05 5a05 6d06  Z...d.d.l.m.Z.m.
 00000050: 5a06 0100 6402 6406 6c07 6d08 5a08 0100  Z...d.d.l.m.Z...
 00000060: 6400 6407 6c09 6d0a 5a0a 0100 0200 4700  d.d.l.m.Z.....G.
 00000070: 6408 8400 6409 6505 ab03 0000 0000 0000  d...d.e.........
```

### Comparing `gskChat-1.0.8/gskChat/Provider/not_working/__pycache__/ChatBase.cpython-312.pyc` & `gskChat-1.0.9/gskChat/Provider/not_working/__pycache__/ChatBase.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Sun Mar 24 15:25:23 2024 UTC, .py size: 4546 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: cb0d 0d0a 0000 0000 e345 0066 c211 0000  .........E.f....
+00000000: cb0d 0d0a 0000 0000 e644 0166 c211 0000  .........D.f....
 00000010: e300 0000 0000 0000 0000 0000 0005 0000  ................
 00000020: 0000 0000 01f3 4e00 0000 9700 6400 6401  ......N.....d.d.
 00000030: 6c00 6d01 5a01 0100 6400 6402 6c02 6d03  l.m.Z...d.d.l.m.
 00000040: 5a03 0100 6403 6404 6c04 6d05 5a05 6d06  Z...d.d.l.m.Z.m.
 00000050: 5a06 0100 6405 6406 6c07 6d08 5a08 0100  Z...d.d.l.m.Z...
 00000060: 0200 4700 6407 8400 6408 6508 ab03 0000  ..G.d...d.e.....
 00000070: 0000 0000 5a09 7909 290a e900 0000 0029  ....Z.y.)......)
```

### Comparing `gskChat-1.0.8/gskChat/Provider/not_working/__pycache__/ChatgptDemo.cpython-312.pyc` & `gskChat-1.0.9/gskChat/Provider/not_working/__pycache__/ChatgptDemo.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Sun Mar 24 15:25:23 2024 UTC, .py size: 2863 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: cb0d 0d0a 0000 0000 e345 0066 2f0b 0000  .........E.f/...
+00000000: cb0d 0d0a 0000 0000 e644 0166 2f0b 0000  .........D.f/...
 00000010: e300 0000 0000 0000 0000 0000 0005 0000  ................
 00000020: 0000 0000 01f3 8600 0000 9700 6400 6401  ............d.d.
 00000030: 6c00 6d01 5a01 0100 6400 6402 6c02 5a02  l.m.Z...d.d.l.Z.
 00000040: 6400 6402 6c03 5a03 6400 6402 6c04 5a04  d.d.l.Z.d.d.l.Z.
 00000050: 6400 6402 6c05 5a05 6400 6403 6c06 6d07  d.d.l.Z.d.d.l.m.
 00000060: 5a07 0100 6404 6405 6c08 6d09 5a09 6d0a  Z...d.d.l.m.Z.m.
 00000070: 5a0a 0100 6404 6406 6c0b 6d0c 5a0c 0100  Z...d.d.l.m.Z...
```

### Comparing `gskChat-1.0.8/gskChat/Provider/not_working/__pycache__/ChatgptDemoAi.cpython-312.pyc` & `gskChat-1.0.9/gskChat/Provider/not_working/__pycache__/ChatgptDemoAi.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Sun Mar 24 15:25:23 2024 UTC, .py size: 2062 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: cb0d 0d0a 0000 0000 e345 0066 0e08 0000  .........E.f....
+00000000: cb0d 0d0a 0000 0000 e644 0166 0e08 0000  .........D.f....
 00000010: e300 0000 0000 0000 0000 0000 0005 0000  ................
 00000020: 0000 0000 01f3 6200 0000 9700 6400 6401  ......b.....d.d.
 00000030: 6c00 6d01 5a01 0100 6400 6402 6c02 5a02  l.m.Z...d.d.l.Z.
 00000040: 6400 6403 6c03 6d04 5a04 0100 6404 6405  d.d.l.m.Z...d.d.
 00000050: 6c05 6d06 5a06 6d07 5a07 0100 6406 6407  l.m.Z.m.Z...d.d.
 00000060: 6c08 6d09 5a09 0100 6406 6408 6c0a 6d0b  l.m.Z...d.d.l.m.
 00000070: 5a0b 0100 0200 4700 6409 8400 640a 6509  Z.....G.d...d.e.
```

### Comparing `gskChat-1.0.8/gskChat/Provider/not_working/__pycache__/ChatgptLogin.cpython-312.pyc` & `gskChat-1.0.9/gskChat/Provider/not_working/__pycache__/ChatgptLogin.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Sun Mar 24 15:25:23 2024 UTC, .py size: 3056 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: cb0d 0d0a 0000 0000 e345 0066 f00b 0000  .........E.f....
+00000000: cb0d 0d0a 0000 0000 e644 0166 f00b 0000  .........D.f....
 00000010: e300 0000 0000 0000 0000 0000 0005 0000  ................
 00000020: 0000 0000 01f3 7200 0000 9700 6400 6401  ......r.....d.d.
 00000030: 6c00 6d01 5a01 0100 6400 6402 6c02 5a02  l.m.Z...d.d.l.Z.
 00000040: 6400 6402 6c03 5a03 6400 6402 6c04 5a04  d.d.l.Z.d.d.l.Z.
 00000050: 6400 6403 6c05 6d06 5a06 0100 6404 6405  d.d.l.m.Z...d.d.
 00000060: 6c07 6d08 5a08 6d09 5a09 0100 6406 6407  l.m.Z.m.Z...d.d.
 00000070: 6c0a 6d0b 5a0b 0100 6406 6408 6c0c 6d0d  l.m.Z...d.d.l.m.
```

### Comparing `gskChat-1.0.8/gskChat/Provider/not_working/__pycache__/Chatxyz.cpython-312.pyc` & `gskChat-1.0.9/gskChat/Provider/not_working/__pycache__/Chatxyz.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Sun Mar 24 15:25:23 2024 UTC, .py size: 2245 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: cb0d 0d0a 0000 0000 e345 0066 c508 0000  .........E.f....
+00000000: cb0d 0d0a 0000 0000 e644 0166 c508 0000  .........D.f....
 00000010: e300 0000 0000 0000 0000 0000 0005 0000  ................
 00000020: 0000 0000 01f3 5600 0000 9700 6400 6401  ......V.....d.d.
 00000030: 6c00 6d01 5a01 0100 6400 6402 6c02 5a02  l.m.Z...d.d.l.Z.
 00000040: 6400 6403 6c03 6d04 5a04 0100 6404 6405  d.d.l.m.Z...d.d.
 00000050: 6c05 6d06 5a06 6d07 5a07 0100 6406 6407  l.m.Z.m.Z...d.d.
 00000060: 6c08 6d09 5a09 0100 0200 4700 6408 8400  l.m.Z.....G.d...
 00000070: 6409 6509 ab03 0000 0000 0000 5a0a 7902  d.e.........Z.y.
```

### Comparing `gskChat-1.0.8/gskChat/Provider/not_working/__pycache__/Gpt6.cpython-312.pyc` & `gskChat-1.0.9/gskChat/Provider/not_working/__pycache__/Gpt6.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Sun Mar 24 15:25:23 2024 UTC, .py size: 2243 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: cb0d 0d0a 0000 0000 e345 0066 c308 0000  .........E.f....
+00000000: cb0d 0d0a 0000 0000 e644 0166 c308 0000  .........D.f....
 00000010: e300 0000 0000 0000 0000 0000 0005 0000  ................
 00000020: 0000 0000 01f3 5600 0000 9700 6400 6401  ......V.....d.d.
 00000030: 6c00 6d01 5a01 0100 6400 6402 6c02 5a02  l.m.Z...d.d.l.Z.
 00000040: 6400 6403 6c03 6d04 5a04 0100 6404 6405  d.d.l.m.Z...d.d.
 00000050: 6c05 6d06 5a06 6d07 5a07 0100 6406 6407  l.m.Z.m.Z...d.d.
 00000060: 6c08 6d09 5a09 0100 0200 4700 6408 8400  l.m.Z.....G.d...
 00000070: 6409 6509 ab03 0000 0000 0000 5a0a 7902  d.e.........Z.y.
```

### Comparing `gskChat-1.0.8/gskChat/Provider/not_working/__pycache__/GptChatly.cpython-312.pyc` & `gskChat-1.0.9/gskChat/Provider/not_working/__pycache__/GptChatly.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Sun Mar 24 15:25:23 2024 UTC, .py size: 1033 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: cb0d 0d0a 0000 0000 e345 0066 0904 0000  .........E.f....
+00000000: cb0d 0d0a 0000 0000 e644 0166 0904 0000  .........D.f....
 00000010: e300 0000 0000 0000 0000 0000 0005 0000  ................
 00000020: 0000 0000 01f3 4e00 0000 9700 6400 6401  ......N.....d.d.
 00000030: 6c00 6d01 5a01 0100 6402 6403 6c02 6d03  l.m.Z...d.d.l.m.
 00000040: 5a03 6d04 5a04 0100 6402 6404 6c05 6d06  Z.m.Z...d.d.l.m.
 00000050: 5a06 0100 6405 6406 6c07 6d08 5a08 0100  Z...d.d.l.m.Z...
 00000060: 0200 4700 6407 8400 6408 6508 ab03 0000  ..G.d...d.e.....
 00000070: 0000 0000 5a09 7909 290a e900 0000 0029  ....Z.y.)......)
```

### Comparing `gskChat-1.0.8/gskChat/Provider/not_working/__pycache__/GptForLove.cpython-312.pyc` & `gskChat-1.0.9/gskChat/Provider/not_working/__pycache__/GptForLove.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Sun Mar 24 15:25:23 2024 UTC, .py size: 3529 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: cb0d 0d0a 0000 0000 e345 0066 c90d 0000  .........E.f....
+00000000: cb0d 0d0a 0000 0000 e644 0166 c90d 0000  .........D.f....
 00000010: e300 0000 0000 0000 0000 0000 0005 0000  ................
 00000020: 0000 0000 01f3 a600 0000 9700 6400 6401  ............d.d.
 00000030: 6c00 6d01 5a01 0100 6400 6402 6c02 6d03  l.m.Z...d.d.l.m.
 00000040: 5a03 0100 6400 6403 6c04 5a04 6400 6403  Z...d.d.l.Z.d.d.
 00000050: 6c05 5a05 0900 6400 6403 6c06 5a06 6404  l.Z...d.d.l.Z.d.
 00000060: 5a07 6406 6407 6c09 6d0a 5a0a 6d0b 5a0b  Z.d.d.l.m.Z.m.Z.
 00000070: 0100 6408 6409 6c0c 6d0d 5a0d 0100 6408  ..d.d.l.m.Z...d.
```

### Comparing `gskChat-1.0.8/gskChat/Provider/not_working/__pycache__/GptGo.cpython-312.pyc` & `gskChat-1.0.9/gskChat/Provider/not_working/__pycache__/GptGo.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Sun Mar 24 15:25:23 2024 UTC, .py size: 2480 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: cb0d 0d0a 0000 0000 e345 0066 b009 0000  .........E.f....
+00000000: cb0d 0d0a 0000 0000 e644 0166 b009 0000  .........D.f....
 00000010: e300 0000 0000 0000 0000 0000 0005 0000  ................
 00000020: 0000 0000 01f3 6200 0000 9700 6400 6401  ......b.....d.d.
 00000030: 6c00 6d01 5a01 0100 6400 6402 6c02 6d03  l.m.Z...d.d.l.m.
 00000040: 5a03 0100 6400 6403 6c04 5a04 6400 6403  Z...d.d.l.Z.d.d.
 00000050: 6c05 5a05 6404 6405 6c06 6d07 5a07 6d08  l.Z.d.d.l.m.Z.m.
 00000060: 5a08 0100 6406 6407 6c09 6d0a 5a0a 6d0b  Z...d.d.l.m.Z.m.
 00000070: 5a0b 0100 0200 4700 6408 8400 6409 650a  Z.....G.d...d.e.
```

### Comparing `gskChat-1.0.8/gskChat/Provider/not_working/__pycache__/GptGod.cpython-312.pyc` & `gskChat-1.0.9/gskChat/Provider/not_working/__pycache__/GptGod.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Sun Mar 24 15:25:23 2024 UTC, .py size: 2061 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: cb0d 0d0a 0000 0000 e345 0066 0d08 0000  .........E.f....
+00000000: cb0d 0d0a 0000 0000 e644 0166 0d08 0000  .........D.f....
 00000010: e300 0000 0000 0000 0000 0000 0005 0000  ................
 00000020: 0000 0000 01f3 6a00 0000 9700 6400 6401  ......j.....d.d.
 00000030: 6c00 6d01 5a01 0100 6400 6402 6c02 5a02  l.m.Z...d.d.l.Z.
 00000040: 6400 6402 6c03 5a03 6400 6403 6c04 6d05  d.d.l.Z.d.d.l.m.
 00000050: 5a05 0100 6404 6405 6c06 6d07 5a07 6d08  Z...d.d.l.m.Z.m.
 00000060: 5a08 0100 6406 6407 6c09 6d0a 5a0a 0100  Z...d.d.l.m.Z...
 00000070: 6406 6408 6c0b 6d0c 5a0c 0100 0200 4700  d.d.l.m.Z.....G.
```

### Comparing `gskChat-1.0.8/gskChat/Provider/not_working/__pycache__/OnlineGpt.cpython-312.pyc` & `gskChat-1.0.9/gskChat/Provider/not_working/__pycache__/OnlineGpt.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Sun Mar 24 15:25:23 2024 UTC, .py size: 2093 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: cb0d 0d0a 0000 0000 e345 0066 2d08 0000  .........E.f-...
+00000000: cb0d 0d0a 0000 0000 e644 0166 2d08 0000  .........D.f-...
 00000010: e300 0000 0000 0000 0000 0000 0005 0000  ................
 00000020: 0000 0000 01f3 6200 0000 9700 6400 6401  ......b.....d.d.
 00000030: 6c00 6d01 5a01 0100 6400 6402 6c02 5a02  l.m.Z...d.d.l.Z.
 00000040: 6400 6403 6c03 6d04 5a04 0100 6404 6405  d.d.l.m.Z...d.d.
 00000050: 6c05 6d06 5a06 6d07 5a07 0100 6406 6407  l.m.Z.m.Z...d.d.
 00000060: 6c08 6d09 5a09 0100 6406 6408 6c0a 6d0b  l.m.Z...d.d.l.m.
 00000070: 5a0b 0100 0200 4700 6409 8400 640a 6509  Z.....G.d...d.e.
```

### Comparing `gskChat-1.0.8/gskChat/Provider/not_working/__pycache__/__init__.cpython-312.pyc` & `gskChat-1.0.9/gskChat/Provider/not_working/__pycache__/__init__.cpython-312.pyc`

 * *Files 2% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xcb0d0d0a
-moddate:  0xe3450066 (Sun Mar 24 15:25:23 2024 UTC)
+moddate:  0xe6440166 (Mon Mar 25 09:33:26 2024 UTC)
 files sz: 498
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 2
    flags     : 0
    code
```

### Comparing `gskChat-1.0.8/gskChat/Provider/npm/node_modules/crypto-js/README.md` & `gskChat-1.0.9/gskChat/Provider/npm/node_modules/crypto-js/README.md`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.8/gskChat/Provider/npm/node_modules/crypto-js/crypto-js.js` & `gskChat-1.0.9/gskChat/Provider/npm/node_modules/crypto-js/crypto-js.js`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.8/gskChat/Provider/npm/package-lock.json` & `gskChat-1.0.9/gskChat/Provider/npm/package-lock.json`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.8/gskChat/Provider/selenium/AItianhuSpace.py` & `gskChat-1.0.9/gskChat/Provider/selenium/AItianhuSpace.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.8/gskChat/Provider/selenium/Bard.py` & `gskChat-1.0.9/gskChat/Provider/selenium/Bard.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.8/gskChat/Provider/selenium/MyShell.py` & `gskChat-1.0.9/gskChat/Provider/selenium/MyShell.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.8/gskChat/Provider/selenium/PerplexityAi.py` & `gskChat-1.0.9/gskChat/Provider/selenium/PerplexityAi.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.8/gskChat/Provider/selenium/Phind.py` & `gskChat-1.0.9/gskChat/Provider/selenium/Phind.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.8/gskChat/Provider/selenium/TalkAi.py` & `gskChat-1.0.9/gskChat/Provider/selenium/TalkAi.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.8/gskChat/Provider/selenium/__pycache__/AItianhuSpace.cpython-312.pyc` & `gskChat-1.0.9/gskChat/Provider/selenium/__pycache__/AItianhuSpace.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Sun Mar 24 15:25:23 2024 UTC, .py size: 3839 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: cb0d 0d0a 0000 0000 e345 0066 ff0e 0000  .........E.f....
+00000000: cb0d 0d0a 0000 0000 e644 0166 ff0e 0000  .........D.f....
 00000010: e300 0000 0000 0000 0000 0000 0005 0000  ................
 00000020: 0000 0000 01f3 8200 0000 9700 6400 6401  ............d.d.
 00000030: 6c00 6d01 5a01 0100 6400 6402 6c02 5a02  l.m.Z...d.d.l.Z.
 00000040: 6400 6402 6c03 5a03 6403 6404 6c04 6d05  d.d.l.Z.d.d.l.m.
 00000050: 5a05 6d06 5a06 0100 6405 6406 6c07 6d08  Z.m.Z...d.d.l.m.
 00000060: 5a08 0100 6405 6407 6c09 6d0a 5a0a 6d0b  Z...d.d.l.m.Z.m.
 00000070: 5a0b 0100 6403 6408 6c0c 6d0d 5a0d 6d0e  Z...d.d.l.m.Z.m.
```

### Comparing `gskChat-1.0.8/gskChat/Provider/selenium/__pycache__/Bard.cpython-312.pyc` & `gskChat-1.0.9/gskChat/Provider/selenium/__pycache__/Bard.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Sun Mar 24 15:25:23 2024 UTC, .py size: 2859 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: cb0d 0d0a 0000 0000 e345 0066 2b0b 0000  .........E.f+...
+00000000: cb0d 0d0a 0000 0000 e644 0166 2b0b 0000  .........D.f+...
 00000010: e300 0000 0000 0000 0000 0000 0005 0000  ................
 00000020: 0000 0000 01f3 ae00 0000 9700 6400 6401  ............d.d.
 00000030: 6c00 6d01 5a01 0100 6400 6402 6c02 5a02  l.m.Z...d.d.l.Z.
 00000040: 6400 6402 6c03 5a03 0900 6400 6403 6c04  d.d.l.Z...d.d.l.
 00000050: 6d05 5a05 0100 6400 6404 6c06 6d07 5a07  m.Z...d.d.l.m.Z.
 00000060: 0100 6400 6405 6c08 6d09 5a0a 0100 6406  ..d.d.l.m.Z...d.
 00000070: 6407 6c0c 6d0d 5a0d 6d0e 5a0e 0100 6408  d.l.m.Z.m.Z...d.
```

### Comparing `gskChat-1.0.8/gskChat/Provider/selenium/__pycache__/MyShell.cpython-312.pyc` & `gskChat-1.0.9/gskChat/Provider/selenium/__pycache__/MyShell.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Sun Mar 24 15:25:23 2024 UTC, .py size: 2250 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: cb0d 0d0a 0000 0000 e345 0066 ca08 0000  .........E.f....
+00000000: cb0d 0d0a 0000 0000 e644 0166 ca08 0000  .........D.f....
 00000010: e300 0000 0000 0000 0000 0000 0005 0000  ................
 00000020: 0000 0000 01f3 7200 0000 9700 6400 6401  ......r.....d.d.
 00000030: 6c00 6d01 5a01 0100 6400 6402 6c02 5a02  l.m.Z...d.d.l.Z.
 00000040: 6400 6402 6c03 5a03 6403 6404 6c04 6d05  d.d.l.Z.d.d.l.m.
 00000050: 5a05 6d06 5a06 0100 6405 6406 6c07 6d08  Z.m.Z...d.d.l.m.
 00000060: 5a08 0100 6405 6407 6c09 6d0a 5a0a 0100  Z...d.d.l.m.Z...
 00000070: 6403 6408 6c0b 6d0c 5a0c 6d0d 5a0d 6d0e  d.d.l.m.Z.m.Z.m.
```

### Comparing `gskChat-1.0.8/gskChat/Provider/selenium/__pycache__/PerplexityAi.cpython-312.pyc` & `gskChat-1.0.9/gskChat/Provider/selenium/__pycache__/PerplexityAi.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Sun Mar 24 15:25:23 2024 UTC, .py size: 3681 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: cb0d 0d0a 0000 0000 e345 0066 610e 0000  .........E.fa...
+00000000: cb0d 0d0a 0000 0000 e644 0166 610e 0000  .........D.fa...
 00000010: e300 0000 0000 0000 0000 0000 0005 0000  ................
 00000020: 0000 0000 01f3 a600 0000 9700 6400 6401  ............d.d.
 00000030: 6c00 6d01 5a01 0100 6400 6402 6c02 5a02  l.m.Z...d.d.l.Z.
 00000040: 0900 6400 6403 6c03 6d04 5a04 0100 6400  ..d.d.l.m.Z...d.
 00000050: 6404 6c05 6d06 5a06 0100 6400 6405 6c07  d.l.m.Z...d.d.l.
 00000060: 6d08 5a09 0100 6406 6407 6c0b 6d0c 5a0c  m.Z...d.d.l.m.Z.
 00000070: 6d0d 5a0d 0100 6408 6409 6c0e 6d0f 5a0f  m.Z...d.d.l.m.Z.
```

### Comparing `gskChat-1.0.8/gskChat/Provider/selenium/__pycache__/Phind.cpython-312.pyc` & `gskChat-1.0.9/gskChat/Provider/selenium/__pycache__/Phind.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Sun Mar 24 15:25:23 2024 UTC, .py size: 3655 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: cb0d 0d0a 0000 0000 e345 0066 470e 0000  .........E.fG...
+00000000: cb0d 0d0a 0000 0000 e644 0166 470e 0000  .........D.fG...
 00000010: e300 0000 0000 0000 0000 0000 0005 0000  ................
 00000020: 0000 0000 01f3 7200 0000 9700 6400 6401  ......r.....d.d.
 00000030: 6c00 6d01 5a01 0100 6400 6402 6c02 5a02  l.m.Z...d.d.l.Z.
 00000040: 6400 6403 6c03 6d04 5a04 0100 6404 6405  d.d.l.m.Z...d.d.
 00000050: 6c05 6d06 5a06 6d07 5a07 0100 6406 6407  l.m.Z.m.Z...d.d.
 00000060: 6c08 6d09 5a09 0100 6406 6408 6c0a 6d0b  l.m.Z...d.d.l.m.
 00000070: 5a0b 0100 6404 6409 6c0c 6d0d 5a0d 6d0e  Z...d.d.l.m.Z.m.
```

### Comparing `gskChat-1.0.8/gskChat/Provider/selenium/__pycache__/TalkAi.cpython-312.pyc` & `gskChat-1.0.9/gskChat/Provider/selenium/__pycache__/TalkAi.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Sun Mar 24 15:25:23 2024 UTC, .py size: 2678 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: cb0d 0d0a 0000 0000 e345 0066 760a 0000  .........E.fv...
+00000000: cb0d 0d0a 0000 0000 e644 0166 760a 0000  .........D.fv...
 00000010: e300 0000 0000 0000 0000 0000 0005 0000  ................
 00000020: 0000 0000 01f3 6a00 0000 9700 6400 6401  ......j.....d.d.
 00000030: 6c00 6d01 5a01 0100 6400 6402 6c02 5a02  l.m.Z...d.d.l.Z.
 00000040: 6400 6402 6c03 5a03 6400 6402 6c02 5a02  d.d.l.Z.d.d.l.Z.
 00000050: 6403 6404 6c04 6d05 5a05 6d06 5a06 0100  d.d.l.m.Z.m.Z...
 00000060: 6405 6406 6c07 6d08 5a08 0100 6403 6407  d.d.l.m.Z...d.d.
 00000070: 6c09 6d0a 5a0a 6d0b 5a0b 0100 0200 4700  l.m.Z.m.Z.....G.
```

### Comparing `gskChat-1.0.8/gskChat/Provider/unfinished/AiChatting.py` & `gskChat-1.0.9/gskChat/Provider/unfinished/AiChatting.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.8/gskChat/Provider/unfinished/ChatAiGpt.py` & `gskChat-1.0.9/gskChat/Provider/unfinished/ChatAiGpt.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.8/gskChat/Provider/unfinished/Komo.py` & `gskChat-1.0.9/gskChat/Provider/unfinished/Komo.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.8/gskChat/Provider/unfinished/MikuChat.py` & `gskChat-1.0.9/gskChat/Provider/unfinished/MikuChat.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.8/gskChat/Provider/unfinished/__pycache__/AiChatting.cpython-312.pyc` & `gskChat-1.0.9/gskChat/Provider/unfinished/__pycache__/AiChatting.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Sun Mar 24 15:25:23 2024 UTC, .py size: 2260 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: cb0d 0d0a 0000 0000 e345 0066 d408 0000  .........E.f....
+00000000: cb0d 0d0a 0000 0000 e644 0166 d408 0000  .........D.f....
 00000010: e300 0000 0000 0000 0000 0000 0005 0000  ................
 00000020: 0000 0000 01f3 6a00 0000 9700 6400 6401  ......j.....d.d.
 00000030: 6c00 6d01 5a01 0100 6400 6402 6c02 6d03  l.m.Z...d.d.l.m.
 00000040: 5a03 0100 6403 6404 6c04 6d05 5a05 6d06  Z...d.d.l.m.Z.m.
 00000050: 5a06 0100 6405 6406 6c07 6d08 5a08 0100  Z...d.d.l.m.Z...
 00000060: 6403 6407 6c09 6d0a 5a0a 0100 6403 6408  d.d.l.m.Z...d.d.
 00000070: 6c0b 6d0c 5a0c 6d0d 5a0d 0100 0200 4700  l.m.Z.m.Z.....G.
```

### Comparing `gskChat-1.0.8/gskChat/Provider/unfinished/__pycache__/ChatAiGpt.cpython-312.pyc` & `gskChat-1.0.9/gskChat/Provider/unfinished/__pycache__/ChatAiGpt.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Sun Mar 24 15:25:23 2024 UTC, .py size: 2441 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: cb0d 0d0a 0000 0000 e345 0066 8909 0000  .........E.f....
+00000000: cb0d 0d0a 0000 0000 e644 0166 8909 0000  .........D.f....
 00000010: e300 0000 0000 0000 0000 0000 0005 0000  ................
 00000020: 0000 0000 01f3 6200 0000 9700 6400 6401  ......b.....d.d.
 00000030: 6c00 6d01 5a01 0100 6400 6402 6c02 5a02  l.m.Z...d.d.l.Z.
 00000040: 6400 6403 6c03 6d04 5a04 0100 6404 6405  d.d.l.m.Z...d.d.
 00000050: 6c05 6d06 5a06 6d07 5a07 0100 6406 6407  l.m.Z.m.Z...d.d.
 00000060: 6c08 6d09 5a09 0100 6406 6408 6c0a 6d0b  l.m.Z...d.d.l.m.
 00000070: 5a0b 0100 0200 4700 6409 8400 640a 6509  Z.....G.d...d.e.
```

### Comparing `gskChat-1.0.8/gskChat/Provider/unfinished/__pycache__/Komo.cpython-312.pyc` & `gskChat-1.0.9/gskChat/Provider/unfinished/__pycache__/Komo.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Sun Mar 24 15:25:23 2024 UTC, .py size: 1450 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: cb0d 0d0a 0000 0000 e345 0066 aa05 0000  .........E.f....
+00000000: cb0d 0d0a 0000 0000 e644 0166 aa05 0000  .........D.f....
 00000010: e300 0000 0000 0000 0000 0000 0005 0000  ................
 00000020: 0000 0000 01f3 5600 0000 9700 6400 6401  ......V.....d.d.
 00000030: 6c00 6d01 5a01 0100 6400 6402 6c02 5a02  l.m.Z...d.d.l.Z.
 00000040: 6403 6404 6c03 6d04 5a04 0100 6403 6405  d.d.l.m.Z...d.d.
 00000050: 6c05 6d06 5a06 0100 6406 6407 6c07 6d08  l.m.Z...d.d.l.m.
 00000060: 5a08 6d09 5a09 0100 0200 4700 6408 8400  Z.m.Z.....G.d...
 00000070: 6409 6508 ab03 0000 0000 0000 5a0a 7902  d.e.........Z.y.
```

### Comparing `gskChat-1.0.8/gskChat/Provider/unfinished/__pycache__/MikuChat.cpython-312.pyc` & `gskChat-1.0.9/gskChat/Provider/unfinished/__pycache__/MikuChat.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Sun Mar 24 15:25:23 2024 UTC, .py size: 3298 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: cb0d 0d0a 0000 0000 e345 0066 e20c 0000  .........E.f....
+00000000: cb0d 0d0a 0000 0000 e644 0166 e20c 0000  .........D.f....
 00000010: e300 0000 0000 0000 0000 0000 0005 0000  ................
 00000020: 0000 0000 01f3 7e00 0000 9700 6400 6401  ......~.....d.d.
 00000030: 6c00 6d01 5a01 0100 6400 6402 6c02 5a02  l.m.Z...d.d.l.Z.
 00000040: 6400 6402 6c03 5a03 6400 6403 6c04 6d04  d.d.l.Z.d.d.l.m.
 00000050: 5a04 0100 6404 6405 6c05 6d06 5a06 0100  Z...d.d.l.m.Z...
 00000060: 6404 6406 6c07 6d08 5a08 0100 6407 6408  d.d.l.m.Z...d.d.
 00000070: 6c09 6d0a 5a0a 0100 0200 4700 6409 8400  l.m.Z.....G.d...
```

### Comparing `gskChat-1.0.8/gskChat/__init__.py` & `gskChat-1.0.9/gskChat/__init__.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.8/gskChat/__pycache__/__init__.cpython-312.pyc` & `gskChat-1.0.9/gskChat/__pycache__/__init__.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Sun Mar 24 15:25:23 2024 UTC, .py size: 10959 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: cb0d 0d0a 0000 0000 e345 0066 cf2a 0000  .........E.f.*..
+00000000: cb0d 0d0a 0000 0000 e644 0166 cf2a 0000  .........D.f.*..
 00000010: e300 0000 0000 0000 0000 0000 0004 0000  ................
 00000020: 0000 0000 01f3 fa00 0000 9700 6400 6401  ............d.d.
 00000030: 6c00 6d01 5a01 0100 6400 6402 6c02 5a02  l.m.Z...d.d.l.Z.
 00000040: 6403 6404 6c03 ad02 0100 6403 6405 6c04  d.d.l.....d.d.l.
 00000050: 6d05 5a05 6d06 5a06 0100 6403 6406 6c07  m.Z.m.Z...d.d.l.
 00000060: 6d08 5a08 6d09 5a09 0100 6403 6407 6c0a  m.Z.m.Z...d.d.l.
 00000070: 6d0b 5a0b 6d0c 5a0c 6d0d 5a0d 6d0e 5a0e  m.Z.m.Z.m.Z.m.Z.
```

### Comparing `gskChat-1.0.8/gskChat/__pycache__/cli.cpython-312.pyc` & `gskChat-1.0.9/gskChat/__pycache__/cli.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Sun Mar 24 15:25:23 2024 UTC, .py size: 1318 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: cb0d 0d0a 0000 0000 e345 0066 2605 0000  .........E.f&...
+00000000: cb0d 0d0a 0000 0000 e644 0166 2605 0000  .........D.f&...
 00000010: e300 0000 0000 0000 0000 0000 0002 0000  ................
 00000020: 0000 0000 00f3 6200 0000 9700 6400 6401  ......b.....d.d.
 00000030: 6c00 5a00 6400 6402 6c01 6d02 5a02 0100  l.Z.d.d.l.m.Z...
 00000040: 6400 6401 6c03 5a03 6400 6403 6c03 6d04  d.d.l.Z.d.d.l.m.
 00000050: 5a04 0100 6400 6404 6c05 6d06 5a06 6d07  Z...d.d.l.m.Z.m.
 00000060: 5a07 0100 6405 8400 5a08 6406 8400 5a09  Z...d...Z.d...Z.
 00000070: 650a 6407 6b28 0000 7208 0200 6509 ab00  e.d.k(..r...e...
```

### Comparing `gskChat-1.0.8/gskChat/__pycache__/client.cpython-312.pyc` & `gskChat-1.0.9/gskChat/__pycache__/client.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Sun Mar 24 15:25:23 2024 UTC, .py size: 8568 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: cb0d 0d0a 0000 0000 e345 0066 7821 0000  .........E.fx!..
+00000000: cb0d 0d0a 0000 0000 e644 0166 7821 0000  .........D.fx!..
 00000010: e300 0000 0000 0000 0000 0000 0004 0000  ................
 00000020: 0000 0000 01f3 b201 0000 9700 6400 6401  ............d.d.
 00000030: 6c00 6d01 5a01 0100 6400 6402 6c02 5a02  l.m.Z...d.d.l.Z.
 00000040: 6400 6402 6c03 5a03 6400 6402 6c04 5a04  d.d.l.Z.d.d.l.Z.
 00000050: 6400 6402 6c05 5a05 6400 6402 6c06 5a06  d.d.l.Z.d.d.l.Z.
 00000060: 6403 6404 6c07 6d08 5a08 6d09 5a09 6d0a  d.d.l.m.Z.m.Z.m.
 00000070: 5a0a 6d0b 5a0b 0100 6403 6405 6c0c 6d0d  Z.m.Z...d.d.l.m.
```

### Comparing `gskChat-1.0.8/gskChat/__pycache__/cookies.cpython-312.pyc` & `gskChat-1.0.9/gskChat/__pycache__/cookies.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Sun Mar 24 15:25:23 2024 UTC, .py size: 3406 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: cb0d 0d0a 0000 0000 e345 0066 4e0d 0000  .........E.fN...
+00000000: cb0d 0d0a 0000 0000 e644 0166 4e0d 0000  .........D.fN...
 00000010: e300 0000 0000 0000 0000 0000 0004 0000  ................
 00000020: 0000 0000 01f3 4a01 0000 9700 5500 6400  ......J.....U.d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 5a02 6400 6402 6c03 5a03 0900 6400 6403  Z.d.d.l.Z...d.d.
 00000050: 6c04 6d05 5a05 0100 6404 5a06 0900 6400  l.m.Z...d.Z...d.
 00000060: 6406 6c08 6d09 5a09 6d0a 5a0a 6d0b 5a0b  d.l.m.Z.m.Z.m.Z.
 00000070: 6d0c 5a0c 6d0d 5a0d 6d0e 5a0e 6d0f 5a0f  m.Z.m.Z.m.Z.m.Z.
```

### Comparing `gskChat-1.0.8/gskChat/__pycache__/errors.cpython-312.pyc` & `gskChat-1.0.9/gskChat/__pycache__/errors.cpython-312.pyc`

 * *Files 4% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xcb0d0d0a
-moddate:  0xe3450066 (Sun Mar 24 15:25:23 2024 UTC)
+moddate:  0xe6440166 (Mon Mar 25 09:33:26 2024 UTC)
 files sz: 712
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
```

### Comparing `gskChat-1.0.8/gskChat/__pycache__/image.cpython-312.pyc` & `gskChat-1.0.9/gskChat/__pycache__/image.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Sun Mar 24 15:25:23 2024 UTC, .py size: 8399 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: cb0d 0d0a 0000 0000 e345 0066 cf20 0000  .........E.f. ..
+00000000: cb0d 0d0a 0000 0000 e644 0166 cf20 0000  .........D.f. ..
 00000010: e300 0000 0000 0000 0000 0000 0004 0000  ................
 00000020: 0000 0000 01f3 1801 0000 9700 6400 6401  ............d.d.
 00000030: 6c00 6d01 5a01 0100 6400 6402 6c02 5a02  l.m.Z...d.d.l.Z.
 00000040: 6400 6403 6c03 6d04 5a04 0100 6400 6402  d.d.l.m.Z...d.d.
 00000050: 6c05 5a05 6404 6405 6c06 6d07 5a07 6d08  l.Z.d.d.l.m.Z.m.
 00000060: 5a08 6d09 5a09 0100 0900 6400 6406 6c0a  Z.m.Z.....d.d.l.
 00000070: 6d0b 5a0c 6d0d 5a0e 0100 6400 6407 6c0a  m.Z.m.Z...d.d.l.
```

### Comparing `gskChat-1.0.8/gskChat/__pycache__/models.cpython-312.pyc` & `gskChat-1.0.9/gskChat/__pycache__/models.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Sun Mar 24 15:25:23 2024 UTC, .py size: 7633 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: cb0d 0d0a 0000 0000 e345 0066 d11d 0000  .........E.f....
+00000000: cb0d 0d0a 0000 0000 e644 0166 d11d 0000  .........D.f....
 00000010: e300 0000 0000 0000 0000 0000 000c 0000  ................
 00000020: 0000 0000 01f3 4805 0000 9700 6400 6401  ......H.....d.d.
 00000030: 6c00 6d01 5a01 0100 6400 6402 6c02 6d03  l.m.Z...d.d.l.m.
 00000040: 5a03 0100 6403 6404 6c04 6d05 5a05 6d06  Z...d.d.l.m.Z.m.
 00000050: 5a06 0100 6403 6405 6c04 6d07 5a07 6d08  Z...d.d.l.m.Z.m.
 00000060: 5a08 6d09 5a09 6d0a 5a0a 6d0b 5a0b 6d0c  Z.m.Z.m.Z.m.Z.m.
 00000070: 5a0c 6d0d 5a0d 6d0e 5a0e 6d0f 5a0f 6d10  Z.m.Z.m.Z.m.Z.m.
```

### Comparing `gskChat-1.0.8/gskChat/__pycache__/stubs.cpython-312.pyc` & `gskChat-1.0.9/gskChat/__pycache__/stubs.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Sun Mar 24 15:25:23 2024 UTC, .py size: 2938 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: cb0d 0d0a 0000 0000 e345 0066 7a0b 0000  .........E.fz...
+00000000: cb0d 0d0a 0000 0000 e644 0166 7a0b 0000  .........D.fz...
 00000010: e300 0000 0000 0000 0000 0000 0005 0000  ................
 00000020: 0000 0000 01f3 e000 0000 9700 6400 6401  ............d.d.
 00000030: 6c00 6d01 5a01 0100 6400 6402 6c02 6d03  l.m.Z...d.d.l.m.
 00000040: 5a03 0100 0200 4700 6403 8400 6404 ab02  Z.....G.d...d...
 00000050: 0000 0000 0000 5a04 0200 4700 6405 8400  ......Z...G.d...
 00000060: 6406 6504 ab03 0000 0000 0000 5a05 0200  d.e.........Z...
 00000070: 4700 6407 8400 6408 6504 ab03 0000 0000  G.d...d.e.......
```

### Comparing `gskChat-1.0.8/gskChat/__pycache__/typing.cpython-312.pyc` & `gskChat-1.0.9/gskChat/__pycache__/typing.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Sun Mar 24 15:25:23 2024 UTC, .py size: 875 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: cb0d 0d0a 0000 0000 e345 0066 6b03 0000  .........E.fk...
+00000000: cb0d 0d0a 0000 0000 e644 0166 6b03 0000  .........D.fk...
 00000010: e300 0000 0000 0000 0000 0000 0006 0000  ................
 00000020: 0000 0000 00f3 1401 0000 9700 6400 6401  ............d.d.
 00000030: 6c00 5a00 6400 6402 6c01 6d02 5a02 6d03  l.Z.d.d.l.m.Z.m.
 00000040: 5a03 6d04 5a04 6d05 5a05 6d06 5a06 6d07  Z.m.Z.m.Z.m.Z.m.
 00000050: 5a07 6d08 5a08 6d09 5a09 6d0a 5a0a 6d0b  Z.m.Z.m.Z.m.Z.m.
 00000060: 5a0b 6d0c 5a0c 6d0d 5a0d 6d0e 5a0e 0100  Z.m.Z.m.Z.m.Z...
 00000070: 0900 6400 6403 6c0f 6d10 5a10 0100 6500  ..d.d.l.m.Z...e.
```

### Comparing `gskChat-1.0.8/gskChat/__pycache__/version.cpython-312.pyc` & `gskChat-1.0.9/gskChat/__pycache__/version.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Sun Mar 24 15:25:23 2024 UTC, .py size: 3821 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: cb0d 0d0a 0000 0000 e345 0066 ed0e 0000  .........E.f....
+00000000: cb0d 0d0a 0000 0000 e644 0166 ed0e 0000  .........D.f....
 00000010: e300 0000 0000 0000 0000 0000 0004 0000  ................
 00000020: 0000 0000 01f3 a200 0000 9700 6400 6401  ............d.d.
 00000030: 6c00 6d01 5a01 0100 6400 6402 6c02 6d03  l.m.Z...d.d.l.m.
 00000040: 5a03 0100 6400 6403 6c04 5a04 6400 6404  Z...d.d.l.Z.d.d.
 00000050: 6c05 6d06 5a06 0100 6400 6405 6c07 6d08  l.m.Z...d.d.l.m.
 00000060: 5a09 6d0a 5a0a 0100 6400 6406 6c0b 6d0c  Z.m.Z...d.d.l.m.
 00000070: 5a0c 6d0d 5a0d 6d0e 5a0e 0100 6407 6408  Z.m.Z.m.Z...d.d.
```

### Comparing `gskChat-1.0.8/gskChat/__pycache__/webdriver.cpython-312.pyc` & `gskChat-1.0.9/gskChat/__pycache__/webdriver.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Sun Mar 24 15:25:23 2024 UTC, .py size: 9953 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: cb0d 0d0a 0000 0000 e345 0066 e126 0000  .........E.f.&..
+00000000: cb0d 0d0a 0000 0000 e644 0166 e126 0000  .........D.f.&..
 00000010: e300 0000 0000 0000 0000 0000 0007 0000  ................
 00000020: 0000 0000 01f3 d201 0000 9700 6400 6401  ............d.d.
 00000030: 6c00 6d01 5a01 0100 0900 6400 6402 6c02  l.m.Z.....d.d.l.
 00000040: 6d03 5a03 0100 6400 6403 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 6d06 5a06 6d07 5a07 0100 6400 6404 6c08  m.Z.m.Z...d.d.l.
 00000060: 6d09 5a09 0100 6400 6405 6c0a 6d0b 5a0b  m.Z...d.d.l.m.Z.
 00000070: 0100 6400 6406 6c0c 6d0d 5a0d 0100 6400  ..d.d.l.m.Z...d.
```

### Comparing `gskChat-1.0.8/gskChat/api/__init__.py` & `gskChat-1.0.9/gskChat/api/__init__.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.8/gskChat/api/__pycache__/__init__.cpython-312.pyc` & `gskChat-1.0.9/gskChat/api/__pycache__/__init__.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Sun Mar 24 15:25:23 2024 UTC, .py size: 5168 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: cb0d 0d0a 0000 0000 e345 0066 3014 0000  .........E.f0...
+00000000: cb0d 0d0a 0000 0000 e644 0166 3014 0000  .........D.f0...
 00000010: e300 0000 0000 0000 0000 0000 0009 0000  ................
 00000020: 0000 0000 00f3 ec00 0000 9700 6400 6401  ............d.d.
 00000030: 6c00 5a00 6400 6401 6c01 5a01 6400 6401  l.Z.d.d.l.Z.d.d.
 00000040: 6c02 5a02 6400 6401 6c03 5a03 6400 6402  l.Z.d.d.l.Z.d.d.
 00000050: 6c04 6d05 5a05 6d06 5a06 6d07 5a07 0100  l.m.Z.m.Z.m.Z...
 00000060: 6400 6403 6c08 6d09 5a09 6d0a 5a0a 6d0b  d.d.l.m.Z.m.Z.m.
 00000070: 5a0b 6d0c 5a0c 0100 6400 6404 6c0d 6d0e  Z.m.Z...d.d.l.m.
```

### Comparing `gskChat-1.0.8/gskChat/api/__pycache__/_logging.cpython-312.pyc` & `gskChat-1.0.9/gskChat/api/__pycache__/_logging.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Sun Mar 24 15:25:23 2024 UTC, .py size: 893 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: cb0d 0d0a 0000 0000 e345 0066 7d03 0000  .........E.f}...
+00000000: cb0d 0d0a 0000 0000 e644 0166 7d03 0000  .........D.f}...
 00000010: e300 0000 0000 0000 0000 0000 0005 0000  ................
 00000020: 0000 0000 00f3 5c00 0000 9700 6400 6401  ......\.....d.d.
 00000030: 6c00 5a00 6400 6401 6c01 5a01 6400 6402  l.Z.d.d.l.Z.d.d.
 00000040: 6c02 6d03 5a03 0100 6403 8400 5a04 0200  l.m.Z...d...Z...
 00000050: 4700 6404 8400 6405 6501 6a0a 0000 0000  G.d...d.e.j.....
 00000060: 0000 0000 0000 0000 0000 0000 0000 ab03  ................
 00000070: 0000 0000 0000 5a06 6406 8400 5a07 6407  ......Z.d...Z.d.
```

### Comparing `gskChat-1.0.8/gskChat/api/__pycache__/run.cpython-312.pyc` & `gskChat-1.0.9/gskChat/api/__pycache__/run.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Sun Mar 24 15:25:23 2024 UTC, .py size: 201 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: cb0d 0d0a 0000 0000 e345 0066 c900 0000  .........E.f....
+00000000: cb0d 0d0a 0000 0000 e644 0166 c900 0000  .........D.f....
 00000010: e300 0000 0000 0000 0000 0000 0005 0000  ................
 00000020: 0000 0000 00f3 ce00 0000 9700 6400 6401  ............d.d.
 00000030: 6c00 5a00 6400 6401 6c01 5a00 6502 6402  l.Z.d.d.l.Z.e.d.
 00000040: 6b28 0000 7258 0200 6503 6403 6500 6a08  k(..rX..e.d.e.j.
 00000050: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000060: 0000 6a0a 0000 0000 0000 0000 0000 0000  ..j.............
 00000070: 0000 0000 0000 6a0c 0000 0000 0000 0000  ......j.........
```

### Comparing `gskChat-1.0.8/gskChat/api/_logging.py` & `gskChat-1.0.9/gskChat/api/_logging.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.8/gskChat/cli.py` & `gskChat-1.0.9/gskChat/cli.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.8/gskChat/client.py` & `gskChat-1.0.9/gskChat/client.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.8/gskChat/cookies.py` & `gskChat-1.0.9/gskChat/cookies.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.8/gskChat/errors.py` & `gskChat-1.0.9/gskChat/errors.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.8/gskChat/gui/__init__.py` & `gskChat-1.0.9/gskChat/gui/__init__.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.8/gskChat/gui/__pycache__/__init__.cpython-312.pyc` & `gskChat-1.0.9/gskChat/gui/__pycache__/__init__.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Sun Mar 24 15:25:23 2024 UTC, .py size: 1567 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: cb0d 0d0a 0000 0000 e345 0066 1f06 0000  .........E.f....
+00000000: cb0d 0d0a 0000 0000 e644 0166 1f06 0000  .........D.f....
 00000010: e300 0000 0000 0000 0000 0000 0009 0000  ................
 00000020: 0000 0000 00f3 5000 0000 9700 6400 6401  ......P.....d.d.
 00000030: 6c00 6d01 5a01 0100 6400 6402 6c02 5a02  l.m.Z...d.d.l.Z.
 00000040: 6400 6403 6c03 6d04 5a04 0100 6400 6404  d.d.l.m.Z...d.d.
 00000050: 6c03 6d05 5a05 0100 6405 8400 5a06 640b  l.m.Z...d...Z.d.
 00000060: 6406 6507 6407 6508 6408 6509 6409 6402  d.e.d.e.d.e.d.d.
 00000070: 6608 640a 8405 5a0a 7902 290c e900 0000  f.d...Z.y.).....
```

### Comparing `gskChat-1.0.8/gskChat/gui/__pycache__/run.cpython-312.pyc` & `gskChat-1.0.9/gskChat/gui/__pycache__/run.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Sun Mar 24 15:25:23 2024 UTC, .py size: 615 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: cb0d 0d0a 0000 0000 e345 0066 6702 0000  .........E.fg...
+00000000: cb0d 0d0a 0000 0000 e644 0166 6702 0000  .........D.fg...
 00000010: e300 0000 0000 0000 0000 0000 0003 0000  ................
 00000020: 0000 0000 00f3 6600 0000 9700 6400 6401  ......f.....d.d.
 00000030: 6c00 6d01 5a01 0100 6402 8400 5a02 6403  l.m.Z...d...Z.d.
 00000040: 8400 5a03 6504 6404 6b28 0000 7220 0200  ..Z.e.d.k(..r ..
 00000050: 6502 ab00 0000 0000 0000 5a05 6505 6a0d  e.........Z.e.j.
 00000060: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000070: 0000 ab00 0000 0000 0000 5a07 0200 6503  ..........Z...e.
```

### Comparing `gskChat-1.0.8/gskChat/gui/__pycache__/webview.cpython-312.pyc` & `gskChat-1.0.9/gskChat/gui/__pycache__/webview.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Sun Mar 24 15:25:23 2024 UTC, .py size: 1200 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: cb0d 0d0a 0000 0000 e345 0066 b004 0000  .........E.f....
+00000000: cb0d 0d0a 0000 0000 e644 0166 b004 0000  .........D.f....
 00000010: e300 0000 0000 0000 0000 0000 0004 0000  ................
 00000020: 0000 0000 01f3 2801 0000 9700 6400 6401  ......(.....d.d.
 00000030: 6c00 6d01 5a01 0100 6400 6402 6c02 5a02  l.m.Z...d.d.l.Z.
 00000040: 6400 6402 6c03 5a04 6400 6402 6c05 5a05  d.d.l.Z.d.d.l.Z.
 00000050: 0900 6400 6403 6c06 6d07 5a07 0100 6404  ..d.d.l.m.Z...d.
 00000060: 5a08 6400 6406 6c0a 6d0b 5a0b 0100 6400  Z.d.d.l.m.Z...d.
 00000070: 6407 6c0c 6d0d 5a0d 0100 6400 6402 6c0e  d.l.m.Z...d.d.l.
```

### Comparing `gskChat-1.0.8/gskChat/gui/client/index.html` & `gskChat-1.0.9/gskChat/gui/client/index.html`

 * *Files 1% similar despite different names*

```diff
@@ -120,23 +120,23 @@
           </script>
         </div>
         <div class="secondPrev">
             <div class="contentPrev">
                 <div class="titleContent"><h2 class="hTitle">Выбери своего бота</h2></div>
                 <div class="selectAutor" id="programmer">
                   <div class="logoAutor"><img src="/static/img/programmer.jpg" alt="logoAutor"></div>
-                  <div class="contentAutor"><h3>Лучший программист</h3> <span id="spanPer">┕</span> <span> Ответит на любой вопрос касательно программирования, а так же может написать любой код</span></div>
+                  <div class="contentAutor"><h3>Программист</h3> <span id="spanPer">┕</span> <span> Ответит на любой вопрос касательно программирования, а так же может написать любой код</span></div>
                 </div>
                 <div class="selectAutor" id="teacher">
                   <div class="logoAutor"><img src="/static/img/teacher.jpg" alt="logoAutor"></div>
-                  <div class="contentAutor"><h3>Лучший учитель</h3> <span id="spanPer">┕</span> <span> Знает всё на свете. Хочешь научиться чему-то? Не знаешь чего-то? Тебе сюда</span></div>
+                  <div class="contentAutor"><h3>Учитель</h3> <span id="spanPer">┕</span> <span> Знает всё на свете. Хочешь научиться чему-то? Не знаешь чего-то? Тебе сюда</span></div>
                 </div>
                 <div class="selectAutor" id="writer">
                   <div class="logoAutor"><img src="/static/img/write.jpg" alt="logoAutor"></div>
-                  <div class="contentAutor"><h3>Писатель</h3><span id="spanPer">┕</span><span> Лучший философ. Нужен текст для лекции? Написать  Хочешь придумать стих? тебе сюда</span></div>
+                  <div class="contentAutor"><h3>Писатель</h3><span id="spanPer">┕</span><span> Философ. Нужен текст для лекции? Написать  Хочешь придумать стих? тебе сюда</span></div>
                 </div>
             </div>
         </div>
       </div>
         <div class="row" >
             <div class="box conversations">
               <div class="avtoLogo">
```

#### html2text {}

```diff
@@ -1,19 +1,18 @@
 ********** ?В?ы?б?е?р?и ?с?в?о?е?г?о ?б?о?т?а **********
 [logoAutor]
-******** ?Л?у?ч?ш?и?й ?п?р?о?г?р?а?м?м?и?с?т ********
+******** ?П?р?о?г?р?а?м?м?и?с?т ********
 ┕ Ответит на любой вопрос касательно программирования, а так же может написать
 любой код
 [logoAutor]
-******** ?Л?у?ч?ш?и?й ?у?ч?и?т?е?л?ь ********
+******** ?У?ч?и?т?е?л?ь ********
 ┕ Знает всё на свете. Хочешь научиться чему-то? Не знаешь чего-то? Тебе сюда
 [logoAutor]
 ******** ?П?и?с?а?т?е?л?ь ********
-┕ Лучший философ. Нужен текст для лекции? Написать Хочешь придумать стих? тебе
-сюда
+┕ Философ. Нужен текст для лекции? Написать Хочешь придумать стих? тебе сюда
 Сменить бота
 Новая беседа
 Удалить беседу Выгрузить чат
 АВТОРЫ *ТЫК*
     * _@_t_a_f_i_k_2_3_ _-_ _Ф_а_л_ю_ш_и_н_ _А_._С_ _(_П_р_о_г_р_а_м_м_и_с_т_)
     * _@_f_p_p_z_l_x_l_a_c_ _-_ _С_у_с_л_о_в_а_ _А_._С_ _(_Д_и_з_а_й_н_е_р_)
     * _@_D_a_n_i_a_g_0_ _-_ _М_а_л_и_н_и_н_ _Д_._Д_ _(_К_о_н_т_е_н_т_)
```

### Comparing `gskChat-1.0.8/gskChat/gui/client/static/css/style.css` & `gskChat-1.0.9/gskChat/gui/client/static/css/style.css`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 @import url("https://fonts.googleapis.com/css2?family=Inter:wght@100;200;300;400;500;600;700;800;900&display=swap");
 
 .avtoLogo {
     padding: 5px;
     width: 100%;
-    
+    transition: 250ms;
     justify-content: center;
     height: 165px;
 }
 .avtoLogo:hover {
+    transition: 250ms;
     border-radius: 2em;
-    box-shadow: 2px 2px 12px 2px black;
-    border: 1px solid paleturquoise;
+    box-shadow: 2px 2px 12px 2px rgb(0, 24, 34);
 }
 #smenAutor { 
     font-size: 20px;
     transition: 200ms;
     font-weight: 400;
     margin-top: 5px;
     
@@ -71,15 +71,14 @@
     transition: 100ms;
 }
 .modal-content ul li a span {
     color: #1ba8d3;
 }
 .modal-content ul li a:hover {
     box-shadow: 8px 5px 22px 2px black;
-font-size: 27px;
 transition: 100ms;
 }
 .modal-content ul {
     list-style: none;
 }
 .modal-content a {
     padding: 5px;
@@ -336,15 +335,15 @@
     font-weight: 900;
 }
 .secondPrev {
     margin-top: 50px;
     display: flex;
     justify-content: center;
     width: 100%;
-    height: 100%;
+    height: 80%;
 }
 .selectAutor {
     
     transition: 650ms;
     background-color: #0a1616;
     border-radius: 2em;
     border: 1px dashed black;
@@ -386,16 +385,17 @@
     z-index: 9999;
 }
 .contentPrev {
     border-radius: 20px;
     border: 2px solid rgb(0, 0, 0);
     background-color: rgba(0, 0, 0, 0.9);
     width: 50%;
-    height: 750px;
+    height: 100%;
     box-shadow: 22px 22px 20px 2px black;
+    overflow: auto;
 }
 #title i, #title span{
     text-decoration:double;
     font-family: "Source Code Pro", monospace;
     font-optical-sizing: auto;
     font-weight: 200;
     font-style: italic;
@@ -406,19 +406,20 @@
     line-height: 2;
     color: rgb(13, 238, 182);
 
 }
 .box {
     backdrop-filter: blur(5px);
     -webkit-backdrop-filter: blur(20px);
+    box-shadow: 1px 1px 8px 1px rgba(0, 183, 255, 0.3);
     background-color: var(--blur-bg);
     height: 100%;
     width: 100%;
     border-radius: var(--border-radius-1);
-    border: 1px solid rgba(255, 187, 0, 0.3);
+    border: 1px solid rgba(0, 183, 255, 0.3);
 }
 
 .hidden {
     display: none;
 }
 
 .conversations {
@@ -506,15 +507,15 @@
 .conversations .convo {
     padding: 8px 12px;
     display: flex;
     gap: 10px;
     align-items: center;
     user-select: none;
     justify-content: space-between;
-    border: 1px dashed var(--conversations);
+    border: 1px dashed rgba(0, 183, 255, 0.3);
     border-radius: var(--border-radius-1);
 }
 
 .conversations .convo .left {
 
     display: flex;
     align-items: center;
@@ -524,15 +525,15 @@
 .conversations .convo .choise {
     position: absolute;
     right: 8px;
     background-color: var(--blur-bg);
 }
 
 .conversations i {
-    color: var(--conversations);
+    color: rgba(0, 183, 255, 0.3);
 
 }
 
 .convo-title {
     color: var(--colour-3);
     font-size: 14px;
     text-overflow: ellipsis;
@@ -676,21 +677,21 @@
     padding: 8px 12px;
     display: flex;
     gap: 18px;
     align-items: center;
 
     user-select: none;
     background: transparent;
-    border: 1px solid var(--conversations);
+    border: 1px solid rgba(0, 183, 255, 0.3);
     border-radius: var(--border-radius-1);
     transition: all 0.2s ease;
 }
 
 .new_convo:hover {
-    box-shadow: inset 0px 0px 20px var(--conversations-hover);
+    box-shadow: inset 0px 0px 20px rgba(0, 183, 255, 0.3);
 }
 
 .new_convo span {
     color: var(--colour-3);
     font-size: 14px;
 }
 
@@ -851,15 +852,15 @@
     height: 20px;
     background: var(--colour-3);
     border-radius: 90px;
     transition: 0.33s;
 }
 
 .buttons input:checked+label {
-    background: #86880a;
+    background: rgba(0, 183, 255, 0.3);
 }
 
 .buttons input:checked+label:after {
     left: calc(100% - 5px - 20px);
 }
 
 .buttons {
@@ -925,38 +926,39 @@
     gap: 18px;
     align-items: center;
     user-select: none;
     background: transparent;
     border-radius: var(--border-radius-1);
     width: 100%;
     cursor: default;
-    border: 1px dashed var(--conversations)
+    border: 1px dashed rgba(0, 183, 255, 0.3);
 }
 
 .bottom_buttons {
     width: 100%;
     display: flex;
     flex-direction: column;
     gap: 10px;
 }
 .bottom_buttons button:hover {
-    transition: 100ms;
-    box-shadow: inset 0px 0px 20px var(--conversations-hover);
+    transition: 200ms;
+    box-shadow: inset 0px 0px 20px rgba(0, 183, 255, 0.3);
 }
 
 .bottom_buttons button {
-    transition: 100ms;
+    box-shadow: 1px 1px 8px 1px rgba(0, 183, 255, 0.3);
+    transition: 200ms;
     padding: 8px 12px;
     display: flex;
     gap: 18px;
     align-items: center;
 
     user-select: none;
     background: transparent;
-    border: 1px solid var(--conversations);
+    border: 1px solid rgba(0, 183, 255, 0.3);
     border-radius: var(--border-radius-1);
     width: 100%;
 }
 
 .bottom_buttons button a,
 .bottom_buttons button span,
 .bottom_buttons .info a,
@@ -1328,33 +1330,40 @@
 
 :root:has(#dark:checked) {
     --colour-1: hsl(209 50% 10%);
     --clr-card-bg: hsl(209 50% 5%);
     --colour-3: hsl(209 50% 90%);
     --conversations: hsl(209 50% 80%);
 }
-
+.fa-paper-plane-top {
+    width: 100%;
+   
+margin-top: 2em;
+    text-align: center;
+}
 #send-button {
-    margin-bottom: 1em;
-    border: 1px dashed #e4d4ffa6;
-    border-radius: 4px;
-
-    padding-left: 8px;
-    padding-right: 5px;
-    padding-top: 2px;
-    padding-bottom: 2px;
+    transition: 300ms;
+    border-radius: 0px 8px 8px 0px;
     position: absolute;
-    bottom: 8px;
-    right: 8px;
+    right: -1px;
+    height: 100%;
+    width: 3%;
+    background: rgba(0, 183, 255, 0.6);
 }
 #version_text {
     display: none;
 }
 #send-button:hover {
-    border: 1px solid #e4d4ffc9;
+    transition: 300ms;
+    border-radius: 0px 8px 8px 0px;
+    position: absolute;
+    right: -1px;
+    height: 100%;
+    width: 4%;
+    background: rgba(0, 183, 255, 0.9);
 }
 
 #systemPrompt {
     display: none;
     font-size: 15px;
     width: 100%;
     color: var(--colour-3);
```

### Comparing `gskChat-1.0.8/gskChat/gui/client/static/img/1.png` & `gskChat-1.0.9/gskChat/gui/client/static/img/1.png`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.8/gskChat/gui/client/static/img/android-chrome-192x192.png` & `gskChat-1.0.9/gskChat/gui/client/static/img/android-chrome-192x192.png`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.8/gskChat/gui/client/static/img/android-chrome-512x512.png` & `gskChat-1.0.9/gskChat/gui/client/static/img/android-chrome-512x512.png`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.8/gskChat/gui/client/static/img/apple-touch-icon.png` & `gskChat-1.0.9/gskChat/gui/client/static/img/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.8/gskChat/gui/client/static/img/content.png` & `gskChat-1.0.9/gskChat/gui/client/static/img/content.png`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.8/gskChat/gui/client/static/img/favicon-16x16.png` & `gskChat-1.0.9/gskChat/gui/client/static/img/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.8/gskChat/gui/client/static/img/favicon-32x32.png` & `gskChat-1.0.9/gskChat/gui/client/static/img/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.8/gskChat/gui/client/static/img/gpt.png` & `gskChat-1.0.9/gskChat/gui/client/static/img/gpt.png`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.8/gskChat/gui/client/static/img/gpt1.png` & `gskChat-1.0.9/gskChat/gui/client/static/img/gpt1.png`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.8/gskChat/gui/client/static/img/graphic-designer.png` & `gskChat-1.0.9/gskChat/gui/client/static/img/graphic-designer.png`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.8/gskChat/gui/client/static/img/loading-1.gif` & `gskChat-1.0.9/gskChat/gui/client/static/img/loading-1.gif`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.8/gskChat/gui/client/static/img/loading-101.gif` & `gskChat-1.0.9/gskChat/gui/client/static/img/loading-101.gif`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.8/gskChat/gui/client/static/img/programmer.jpg` & `gskChat-1.0.9/gskChat/gui/client/static/img/programmer.jpg`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.8/gskChat/gui/client/static/img/programmer.png` & `gskChat-1.0.9/gskChat/gui/client/static/img/programmer.png`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.8/gskChat/gui/client/static/img/teacher.jpg` & `gskChat-1.0.9/gskChat/gui/client/static/img/teacher.jpg`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.8/gskChat/gui/client/static/img/telegram.png` & `gskChat-1.0.9/gskChat/gui/client/static/img/telegram.png`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.8/gskChat/gui/client/static/img/user.png` & `gskChat-1.0.9/gskChat/gui/client/static/img/user.png`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.8/gskChat/gui/client/static/img/write.jpg` & `gskChat-1.0.9/gskChat/gui/client/static/img/write.jpg`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.8/gskChat/gui/client/static/js/chat.v1.js` & `gskChat-1.0.9/gskChat/gui/client/static/js/chat.v1.js`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.8/gskChat/gui/client/static/js/highlight.min.js` & `gskChat-1.0.9/gskChat/gui/client/static/js/highlight.min.js`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.8/gskChat/gui/client/static/js/highlightjs-copy.min.js` & `gskChat-1.0.9/gskChat/gui/client/static/js/highlightjs-copy.min.js`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.8/gskChat/gui/client/static/js/icons.js` & `gskChat-1.0.9/gskChat/gui/client/static/js/icons.js`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.8/gskChat/gui/run.py` & `gskChat-1.0.9/gskChat/gui/run.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.8/gskChat/gui/server/__pycache__/android_gallery.cpython-312.pyc` & `gskChat-1.0.9/gskChat/gui/server/__pycache__/android_gallery.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Sun Mar 24 15:25:23 2024 UTC, .py size: 2470 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: cb0d 0d0a 0000 0000 e345 0066 a609 0000  .........E.f....
+00000000: cb0d 0d0a 0000 0000 e644 0166 a609 0000  .........D.f....
 00000010: e300 0000 0000 0000 0000 0000 0003 0000  ................
 00000020: 0000 0000 00f3 8e00 0000 9700 6400 6401  ............d.d.
 00000030: 6c00 6d01 5a01 0100 6400 6402 6c02 6d03  l.m.Z...d.d.l.m.
 00000040: 5a03 0100 6400 6403 6c04 6d05 5a05 0100  Z...d.d.l.m.Z...
 00000050: 6400 6404 6c04 6d06 5a06 0100 6400 6405  d.d.l.m.Z...d.d.
 00000060: 6c07 6d08 5a08 0100 0200 6505 6406 ab01  l.m.Z.....e.d...
 00000070: 0000 0000 0000 5a09 0200 6505 6407 ab01  ......Z...e.d...
```

### Comparing `gskChat-1.0.8/gskChat/gui/server/__pycache__/api.cpython-312.pyc` & `gskChat-1.0.9/gskChat/gui/server/__pycache__/api.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Sun Mar 24 15:25:23 2024 UTC, .py size: 9422 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: cb0d 0d0a 0000 0000 e345 0066 ce24 0000  .........E.f.$..
+00000000: cb0d 0d0a 0000 0000 e644 0166 ce24 0000  .........D.f.$..
 00000010: e300 0000 0000 0000 0000 0000 0006 0000  ................
 00000020: 0000 0000 01f3 1602 0000 9700 5500 6400  ............U.d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 5a02 6400 6402 6c03 5a03 6400 6402 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 5a05 6400 6403 6c06 6d07 5a07 0100 6400  Z.d.d.l.m.Z...d.
 00000060: 6404 6c08 6d09 5a09 0100 6400 6405 6c0a  d.l.m.Z...d.d.l.
 00000070: 6d0b 5a0b 0100 0900 6400 6402 6c0c 5a0c  m.Z.....d.d.l.Z.
```

### Comparing `gskChat-1.0.8/gskChat/gui/server/__pycache__/app.cpython-312.pyc` & `gskChat-1.0.9/gskChat/gui/server/__pycache__/app.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Sun Mar 24 15:25:23 2024 UTC, .py size: 271 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: cb0d 0d0a 0000 0000 e345 0066 0f01 0000  .........E.f....
+00000000: cb0d 0d0a 0000 0000 e644 0166 0f01 0000  .........D.f....
 00000010: e300 0000 0000 0000 0000 0000 0006 0000  ................
 00000020: 0000 0000 00f3 a200 0000 9700 6400 6401  ............d.d.
 00000030: 6c00 5a00 6400 6401 6c01 5a01 6400 6402  l.Z.d.d.l.Z.d.d.
 00000040: 6c02 6d03 5a03 0100 0200 6504 6500 6403  l.m.Z.....e.e.d.
 00000050: 6404 ab03 0000 0000 0000 7227 6501 6a0a  d.........r'e.j.
 00000060: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000070: 0000 6a0d 0000 0000 0000 0000 0000 0000  ..j.............
```

### Comparing `gskChat-1.0.8/gskChat/gui/server/__pycache__/backend.cpython-312.pyc` & `gskChat-1.0.9/gskChat/gui/server/__pycache__/backend.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Sun Mar 24 15:25:23 2024 UTC, .py size: 3681 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: cb0d 0d0a 0000 0000 e345 0066 610e 0000  .........E.fa...
+00000000: cb0d 0d0a 0000 0000 e644 0166 610e 0000  .........D.fa...
 00000010: e300 0000 0000 0000 0000 0000 0005 0000  ................
 00000020: 0000 0000 00f3 4e00 0000 9700 6400 6401  ......N.....d.d.
 00000030: 6c00 5a00 6400 6402 6c01 6d02 5a02 6d03  l.Z.d.d.l.m.Z.m.
 00000040: 5a03 0100 6400 6403 6c04 6d05 5a05 6d06  Z...d.d.l.m.Z.m.
 00000050: 5a06 0100 6404 6405 6c07 6d08 5a08 0100  Z...d.d.l.m.Z...
 00000060: 0200 4700 6406 8400 6407 6508 ab03 0000  ..G.d...d.e.....
 00000070: 0000 0000 5a09 7901 2908 e900 0000 004e  ....Z.y.)......N
```

### Comparing `gskChat-1.0.8/gskChat/gui/server/__pycache__/config.cpython-312.pyc` & `gskChat-1.0.9/gskChat/gui/server/__pycache__/config.cpython-312.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xcb0d0d0a
-moddate:  0xe3450066 (Sun Mar 24 15:25:23 2024 UTC)
+moddate:  0xe6440166 (Mon Mar 25 09:33:26 2024 UTC)
 files sz: 15354
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 10
    flags     : 0
    code
```

### Comparing `gskChat-1.0.8/gskChat/gui/server/__pycache__/internet.cpython-312.pyc` & `gskChat-1.0.9/gskChat/gui/server/__pycache__/internet.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Sun Mar 24 15:25:23 2024 UTC, .py size: 4918 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: cb0d 0d0a 0000 0000 e345 0066 3613 0000  .........E.f6...
+00000000: cb0d 0d0a 0000 0000 e644 0166 3613 0000  .........D.f6...
 00000010: e300 0000 0000 0000 0000 0000 0004 0000  ................
 00000020: 0000 0000 01f3 ba00 0000 9700 6400 6401  ............d.d.
 00000030: 6c00 6d01 5a01 0100 6400 6402 6c02 6d03  l.m.Z...d.d.l.m.
 00000040: 5a03 6d04 5a04 0100 0900 6400 6403 6c05  Z.m.Z.....d.d.l.
 00000050: 6d06 5a06 0100 6400 6404 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
 00000060: 0100 6405 5a09 6407 6408 6c0b 6d0c 5a0c  ..d.Z.d.d.l.m.Z.
 00000070: 0100 6400 6409 6c0d 5a0d 0200 4700 640a  ..d.d.l.Z...G.d.
```

### Comparing `gskChat-1.0.8/gskChat/gui/server/__pycache__/website.cpython-312.pyc` & `gskChat-1.0.9/gskChat/gui/server/__pycache__/website.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Sun Mar 24 15:25:23 2024 UTC, .py size: 839 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: cb0d 0d0a 0000 0000 e345 0066 4703 0000  .........E.fG...
+00000000: cb0d 0d0a 0000 0000 e644 0166 4703 0000  .........D.fG...
 00000010: e300 0000 0000 0000 0000 0000 0004 0000  ................
 00000020: 0000 0000 00f3 3000 0000 9700 6400 6401  ......0.....d.d.
 00000030: 6c00 5a00 6400 6402 6c01 6d02 5a02 6d03  l.Z.d.d.l.m.Z.m.
 00000040: 5a03 0100 0200 4700 6403 8400 6404 ab02  Z.....G.d...d...
 00000050: 0000 0000 0000 5a04 7901 2905 e900 0000  ......Z.y.).....
 00000060: 004e 2902 da0f 7265 6e64 6572 5f74 656d  .N)...render_tem
 00000070: 706c 6174 65da 0872 6564 6972 6563 7463  plate..redirectc
```

### Comparing `gskChat-1.0.8/gskChat/gui/server/android_gallery.py` & `gskChat-1.0.9/gskChat/gui/server/android_gallery.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.8/gskChat/gui/server/api.py` & `gskChat-1.0.9/gskChat/gui/server/api.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.8/gskChat/gui/server/backend.py` & `gskChat-1.0.9/gskChat/gui/server/backend.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.8/gskChat/gui/server/config.py` & `gskChat-1.0.9/gskChat/gui/server/config.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.8/gskChat/gui/server/internet.py` & `gskChat-1.0.9/gskChat/gui/server/internet.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.8/gskChat/gui/server/website.py` & `gskChat-1.0.9/gskChat/gui/server/website.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.8/gskChat/gui/webview.py` & `gskChat-1.0.9/gskChat/gui/webview.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.8/gskChat/image.py` & `gskChat-1.0.9/gskChat/image.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.8/gskChat/local/__init__.py` & `gskChat-1.0.9/gskChat/local/__init__.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.8/gskChat/local/__pycache__/__init__.cpython-312.pyc` & `gskChat-1.0.9/gskChat/local/__pycache__/__init__.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Sun Mar 24 15:25:23 2024 UTC, .py size: 1405 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: cb0d 0d0a 0000 0000 e345 0066 7d05 0000  .........E.f}...
+00000000: cb0d 0d0a 0000 0000 e644 0166 7d05 0000  .........D.f}...
 00000010: e300 0000 0000 0000 0000 0000 0004 0000  ................
 00000020: 0000 0000 00f3 9000 0000 9700 6400 6401  ............d.d.
 00000030: 6c00 6d01 5a01 6d02 5a02 6d03 5a03 0100  l.m.Z.m.Z.m.Z...
 00000040: 6400 6402 6c04 6d05 5a05 6d06 5a06 0100  d.d.l.m.Z.m.Z...
 00000050: 6403 6404 6c07 6d08 5a08 0100 6403 6405  d.d.l.m.Z...d.d.
 00000060: 6c09 6d0a 5a0a 0100 6400 6406 6c0b 6d0c  l.m.Z...d.d.l.m.
 00000070: 5a0c 6d0d 5a0d 6d0e 5a0e 0100 0200 4700  Z.m.Z.m.Z.....G.
```

### Comparing `gskChat-1.0.8/gskChat/local/__pycache__/_engine.cpython-312.pyc` & `gskChat-1.0.9/gskChat/local/__pycache__/_engine.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Sun Mar 24 15:25:23 2024 UTC, .py size: 1832 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: cb0d 0d0a 0000 0000 e345 0066 2807 0000  .........E.f(...
+00000000: cb0d 0d0a 0000 0000 e644 0166 2807 0000  .........D.f(...
 00000010: e300 0000 0000 0000 0000 0000 0004 0000  ................
 00000020: 0000 0000 00f3 3800 0000 9700 6400 6401  ......8.....d.d.
 00000030: 6c00 5a00 6400 6402 6c01 6d02 5a02 0100  l.Z.d.d.l.m.Z...
 00000040: 6403 6404 6c03 6d04 5a04 0100 0200 4700  d.d.l.m.Z.....G.
 00000050: 6405 8400 6406 ab02 0000 0000 0000 5a05  d...d.........Z.
 00000060: 7901 2907 e900 0000 004e 2901 da07 4750  y.)......N)...GP
 00000070: 5434 416c 6ce9 0100 0000 2901 da06 6d6f  T4All.....)...mo
```

### Comparing `gskChat-1.0.8/gskChat/local/__pycache__/_models.cpython-312.pyc` & `gskChat-1.0.9/gskChat/local/__pycache__/_models.cpython-312.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xcb0d0d0a
-moddate:  0xe3450066 (Sun Mar 24 15:25:23 2024 UTC)
+moddate:  0xe6440166 (Mon Mar 25 09:33:26 2024 UTC)
 files sz: 2959
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 18
    flags     : 0
    code
```

### Comparing `gskChat-1.0.8/gskChat/local/_engine.py` & `gskChat-1.0.9/gskChat/local/_engine.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.8/gskChat/local/_models.py` & `gskChat-1.0.9/gskChat/local/_models.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.8/gskChat/models.py` & `gskChat-1.0.9/gskChat/models.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.8/gskChat/providers/__pycache__/base_provider.cpython-312.pyc` & `gskChat-1.0.9/gskChat/providers/__pycache__/base_provider.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Sun Mar 24 15:25:23 2024 UTC, .py size: 9260 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: cb0d 0d0a 0000 0000 e345 0066 2c24 0000  .........E.f,$..
+00000000: cb0d 0d0a 0000 0000 e644 0166 2c24 0000  .........D.f,$..
 00000010: e300 0000 0000 0000 0000 0000 0005 0000  ................
 00000020: 0000 0000 01f3 d201 0000 9700 6400 6401  ............d.d.
 00000030: 6c00 6d01 5a01 0100 6400 6402 6c02 5a02  l.m.Z...d.d.l.Z.
 00000040: 6400 6402 6c03 5a03 6400 6403 6c03 6d04  d.d.l.Z.d.d.l.m.
 00000050: 5a04 0100 6400 6404 6c05 6d06 5a06 0100  Z...d.d.l.m.Z...
 00000060: 6400 6405 6c07 6d08 5a08 0100 6400 6406  d.d.l.m.Z...d.d.
 00000070: 6c09 6d0a 5a0a 6d0b 5a0b 0100 6407 6408  l.m.Z.m.Z...d.d.
```

### Comparing `gskChat-1.0.8/gskChat/providers/__pycache__/create_images.cpython-312.pyc` & `gskChat-1.0.9/gskChat/providers/__pycache__/create_images.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Sun Mar 24 15:25:23 2024 UTC, .py size: 6594 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: cb0d 0d0a 0000 0000 e345 0066 c219 0000  .........E.f....
+00000000: cb0d 0d0a 0000 0000 e644 0166 c219 0000  .........D.f....
 00000010: e300 0000 0000 0000 0000 0000 0005 0000  ................
 00000020: 0000 0000 01f3 7200 0000 9700 6400 6401  ......r.....d.d.
 00000030: 6c00 6d01 5a01 0100 6400 6402 6c02 5a02  l.m.Z...d.d.l.Z.
 00000040: 6400 6402 6c03 5a03 6403 6404 6c04 6d05  d.d.l.Z.d.d.l.m.
 00000050: 5a05 0100 6403 6405 6c06 6d07 5a07 6d08  Z...d.d.l.m.Z.m.
 00000060: 5a08 0100 6406 6407 6c09 6d0a 5a0a 6d0b  Z...d.d.l.m.Z.m.
 00000070: 5a0b 0100 6403 6408 6c0c 6d0d 5a0d 0100  Z...d.d.l.m.Z...
```

### Comparing `gskChat-1.0.8/gskChat/providers/__pycache__/helper.cpython-312.pyc` & `gskChat-1.0.9/gskChat/providers/__pycache__/helper.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Sun Mar 24 15:25:23 2024 UTC, .py size: 1528 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: cb0d 0d0a 0000 0000 e345 0066 f805 0000  .........E.f....
+00000000: cb0d 0d0a 0000 0000 e644 0166 f805 0000  .........D.f....
 00000010: e300 0000 0000 0000 0000 0000 0003 0000  ................
 00000020: 0000 0000 01f3 4a00 0000 9700 6400 6401  ......J.....d.d.
 00000030: 6c00 6d01 5a01 0100 6400 6402 6c02 5a02  l.m.Z...d.d.l.Z.
 00000040: 6400 6402 6c03 5a03 6403 6404 6c04 6d05  d.d.l.Z.d.d.l.m.
 00000050: 5a05 0100 6408 6409 6405 8405 5a06 640a  Z...d.d.d...Z.d.
 00000060: 640b 6406 8405 5a07 640c 640b 6407 8405  d.d...Z.d.d.d...
 00000070: 5a08 7902 290d e900 0000 0029 01da 0b61  Z.y.)......)...a
```

### Comparing `gskChat-1.0.8/gskChat/providers/__pycache__/retry_provider.cpython-312.pyc` & `gskChat-1.0.9/gskChat/providers/__pycache__/retry_provider.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Sun Mar 24 15:25:23 2024 UTC, .py size: 6869 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: cb0d 0d0a 0000 0000 e345 0066 d51a 0000  .........E.f....
+00000000: cb0d 0d0a 0000 0000 e644 0166 d51a 0000  .........D.f....
 00000010: e300 0000 0000 0000 0000 0000 0005 0000  ................
 00000020: 0000 0000 01f3 9c00 0000 9700 6400 6401  ............d.d.
 00000030: 6c00 6d01 5a01 0100 6400 6402 6c02 5a02  l.m.Z...d.d.l.Z.
 00000040: 6400 6402 6c03 5a03 6403 6404 6c04 6d05  d.d.l.Z.d.d.l.m.
 00000050: 5a05 6d06 5a06 6d07 5a07 6d08 5a08 6d09  Z.m.Z.m.Z.m.Z.m.
 00000060: 5a09 0100 6405 6406 6c0a 6d0b 5a0b 6d0c  Z...d.d.l.m.Z.m.
 00000070: 5a0c 0100 6403 6407 6c0d 6d0e 5a0e 0100  Z...d.d.l.m.Z...
```

### Comparing `gskChat-1.0.8/gskChat/providers/__pycache__/types.cpython-312.pyc` & `gskChat-1.0.9/gskChat/providers/__pycache__/types.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Sun Mar 24 15:25:23 2024 UTC, .py size: 3083 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: cb0d 0d0a 0000 0000 e345 0066 0b0c 0000  .........E.f....
+00000000: cb0d 0d0a 0000 0000 e644 0166 0b0c 0000  .........D.f....
 00000010: e300 0000 0000 0000 0000 0000 0005 0000  ................
 00000020: 0000 0000 01f3 8400 0000 9700 6400 6401  ............d.d.
 00000030: 6c00 6d01 5a01 0100 6400 6402 6c02 6d03  l.m.Z...d.d.l.m.
 00000040: 5a03 6d04 5a04 0100 6400 6403 6c05 6d06  Z.m.Z...d.d.l.m.
 00000050: 5a06 6d07 5a07 6d08 5a08 0100 6404 6405  Z.m.Z.m.Z...d.d.
 00000060: 6c05 6d09 5a09 6d0a 5a0a 0100 0200 4700  l.m.Z.m.Z.....G.
 00000070: 6406 8400 6407 6503 ab03 0000 0000 0000  d...d.e.........
```

### Comparing `gskChat-1.0.8/gskChat/providers/base_provider.py` & `gskChat-1.0.9/gskChat/providers/base_provider.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.8/gskChat/providers/create_images.py` & `gskChat-1.0.9/gskChat/providers/create_images.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.8/gskChat/providers/helper.py` & `gskChat-1.0.9/gskChat/providers/helper.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.8/gskChat/providers/retry_provider.py` & `gskChat-1.0.9/gskChat/providers/retry_provider.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.8/gskChat/providers/types.py` & `gskChat-1.0.9/gskChat/providers/types.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.8/gskChat/requests/__init__.py` & `gskChat-1.0.9/gskChat/requests/__init__.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.8/gskChat/requests/__pycache__/__init__.cpython-312.pyc` & `gskChat-1.0.9/gskChat/requests/__pycache__/__init__.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Sun Mar 24 15:25:23 2024 UTC, .py size: 3959 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: cb0d 0d0a 0000 0000 e345 0066 770f 0000  .........E.fw...
+00000000: cb0d 0d0a 0000 0000 e644 0166 770f 0000  .........D.fw...
 00000010: e300 0000 0000 0000 0000 0000 0004 0000  ................
 00000020: 0000 0000 01f3 3001 0000 9700 6400 6401  ......0.....d.d.
 00000030: 6c00 6d01 5a01 0100 0900 6400 6402 6c02  l.m.Z.....d.d.l.
 00000040: 6d03 5a03 6d04 5a04 0100 6403 6404 6c05  m.Z.m.Z...d.d.l.
 00000050: 6d06 5a06 6d07 5a07 6d08 5a08 0100 6405  m.Z.m.Z.m.Z...d.
 00000060: 5a09 0900 6400 6408 6c0e 5a0e 6400 6408  Z...d.d.l.Z.d.d.
 00000070: 6c0f 5a0f 6405 5a10 6403 6409 6c11 6d11  l.Z.d.Z.d.d.l.m.
```

### Comparing `gskChat-1.0.8/gskChat/requests/__pycache__/aiohttp.cpython-312.pyc` & `gskChat-1.0.9/gskChat/requests/__pycache__/aiohttp.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Sun Mar 24 15:25:23 2024 UTC, .py size: 1775 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: cb0d 0d0a 0000 0000 e345 0066 ef06 0000  .........E.f....
+00000000: cb0d 0d0a 0000 0000 e644 0166 ef06 0000  .........D.f....
 00000010: e300 0000 0000 0000 0000 0000 0005 0000  ................
 00000020: 0000 0000 01f3 8e00 0000 9700 6400 6401  ............d.d.
 00000030: 6c00 6d01 5a01 0100 6400 6402 6c02 6d03  l.m.Z...d.d.l.m.
 00000040: 5a03 6d04 5a04 6d05 5a05 6d06 5a06 6d07  Z.m.Z.m.Z.m.Z.m.
 00000050: 5a07 0100 6400 6403 6c08 6d09 5a09 6d0a  Z...d.d.l.m.Z.m.
 00000060: 5a0a 6d0b 5a0b 0100 6404 6405 6c0c 6d0d  Z.m.Z...d.d.l.m.
 00000070: 5a0d 0100 6406 6407 6c0e 6d0f 5a0f 0100  Z...d.d.l.m.Z...
```

### Comparing `gskChat-1.0.8/gskChat/requests/__pycache__/curl_cffi.cpython-312.pyc` & `gskChat-1.0.9/gskChat/requests/__pycache__/curl_cffi.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Sun Mar 24 15:25:23 2024 UTC, .py size: 3016 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: cb0d 0d0a 0000 0000 e345 0066 c80b 0000  .........E.f....
+00000000: cb0d 0d0a 0000 0000 e644 0166 c80b 0000  .........D.f....
 00000010: e300 0000 0000 0000 0000 0000 0005 0000  ................
 00000020: 0000 0000 01f3 8800 0000 9700 6400 6401  ............d.d.
 00000030: 6c00 6d01 5a01 0100 6400 6402 6c02 6d03  l.m.Z...d.d.l.m.
 00000040: 5a03 6d04 5a04 6d05 5a05 0100 6400 6403  Z.m.Z.m.Z...d.d.
 00000050: 6c06 6d07 5a07 6d08 5a08 0100 6400 6404  l.m.Z.m.Z...d.d.
 00000060: 6c09 6d0a 5a0a 0100 6400 6405 6c0b 5a0b  l.m.Z...d.d.l.Z.
 00000070: 0200 4700 6406 8400 6407 ab02 0000 0000  ..G.d...d.......
```

### Comparing `gskChat-1.0.8/gskChat/requests/__pycache__/defaults.cpython-312.pyc` & `gskChat-1.0.9/gskChat/requests/__pycache__/defaults.cpython-312.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xcb0d0d0a
-moddate:  0xe3450066 (Sun Mar 24 15:25:23 2024 UTC)
+moddate:  0xe6440166 (Mon Mar 25 09:33:26 2024 UTC)
 files sz: 1091
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 9
    flags     : 0
    code
```

### Comparing `gskChat-1.0.8/gskChat/requests/__pycache__/raise_for_status.cpython-312.pyc` & `gskChat-1.0.9/gskChat/requests/__pycache__/raise_for_status.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Sun Mar 24 15:25:23 2024 UTC, .py size: 1625 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: cb0d 0d0a 0000 0000 e345 0066 5906 0000  .........E.fY...
+00000000: cb0d 0d0a 0000 0000 e644 0166 5906 0000  .........D.fY...
 00000010: e300 0000 0000 0000 0000 0000 0005 0000  ................
 00000020: 0000 0000 01f3 8600 0000 9700 6400 6401  ............d.d.
 00000030: 6c00 6d01 5a01 0100 6400 6402 6c02 6d03  l.m.Z...d.d.l.m.
 00000040: 5a03 0100 6400 6403 6c04 6d05 5a05 0100  Z...d.d.l.m.Z...
 00000050: 6400 6404 6c06 6d07 5a08 0100 6405 6406  d.d.l.m.Z...d.d.
 00000060: 6c09 6d0a 5a0a 6d0b 5a0b 0100 6407 6408  l.m.Z.m.Z...d.d.
 00000070: 6c0c 6d07 5a07 6d0d 5a0d 0100 0200 4700  l.m.Z.m.Z.....G.
```

### Comparing `gskChat-1.0.8/gskChat/requests/aiohttp.py` & `gskChat-1.0.9/gskChat/requests/aiohttp.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.8/gskChat/requests/curl_cffi.py` & `gskChat-1.0.9/gskChat/requests/curl_cffi.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.8/gskChat/requests/defaults.py` & `gskChat-1.0.9/gskChat/requests/defaults.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.8/gskChat/requests/raise_for_status.py` & `gskChat-1.0.9/gskChat/requests/raise_for_status.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.8/gskChat/stubs.py` & `gskChat-1.0.9/gskChat/stubs.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.8/gskChat/typing.py` & `gskChat-1.0.9/gskChat/typing.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.8/gskChat/version.py` & `gskChat-1.0.9/gskChat/version.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.8/gskChat/webdriver.py` & `gskChat-1.0.9/gskChat/webdriver.py`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.8/gskChat.egg-info/PKG-INFO` & `gskChat-1.0.9/gskChat.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gskChat
-Version: 1.0.8
+Version: 1.0.9
 Summary: Gsk Chatbot
 Author: tafik
 Author-email: <doneld528@gmail.com>
 Keywords: python,chatbot,reverse-engineering,openai,chatbots,gpt,language-model,gpt-3,gpt3,openai-api,gpt-4,gpt4,chatgpt,chatgpt-api,openai-chatgpt,chatgpt-free,chatgpt-4,chatgpt4,chatgpt4-api,free,free-gpt,gpt4free,g4f
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `gskChat-1.0.8/gskChat.egg-info/SOURCES.txt` & `gskChat-1.0.9/gskChat.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -259,14 +259,15 @@
 gskChat/gui/run.py
 gskChat/gui/webview.py
 gskChat/gui/__pycache__/__init__.cpython-312.pyc
 gskChat/gui/__pycache__/run.cpython-312.pyc
 gskChat/gui/__pycache__/webview.cpython-312.pyc
 gskChat/gui/client/__init__.py
 gskChat/gui/client/index.html
+gskChat/gui/client/test.html
 gskChat/gui/client/__pycache__/__init__.cpython-312.pyc
 gskChat/gui/client/static/__init__.py
 gskChat/gui/client/static/__pycache__/__init__.cpython-312.pyc
 gskChat/gui/client/static/css/__init__.py
 gskChat/gui/client/static/css/style.css
 gskChat/gui/client/static/css/__pycache__/__init__.cpython-312.pyc
 gskChat/gui/client/static/img/1.png
```

### Comparing `gskChat-1.0.8/gskChat.egg-info/requires.txt` & `gskChat-1.0.9/gskChat.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `gskChat-1.0.8/setup.py` & `gskChat-1.0.9/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -67,15 +67,15 @@
 DESCRIPTION = (
     "Gsk Chatbot"
 )
 
 # Setting up
 setup(
     name='gskChat',
-    version="1.0.8",
+    version="1.0.9",
     author='tafik',
     author_email='<doneld528@gmail.com>',
     description=DESCRIPTION,
     long_description_content_type='text/markdown',
     long_description="Gsk Chatbot",
     packages=find_packages(),
     package_data={
```

