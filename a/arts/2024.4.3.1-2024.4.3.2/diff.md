# Comparing `tmp/arts-2024.4.3.1.tar.gz` & `tmp/arts-2024.4.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arts-2024.4.3.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "arts-2024.4.3.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `arts-2024.4.3.1.tar` & `arts-2024.4.3.2.tar`

### file list

```diff
@@ -1,229 +1,229 @@
--rw-r--r--   0        0        0     2175 2023-12-20 10:09:43.709218 arts-2024.4.3.1/.gitignore
--rw-r--r--   0        0        0       46 2024-03-10 10:13:06.948005 arts-2024.4.3.1/README.md
--rw-r--r--   0        0        0      317 2024-02-22 12:02:36.224046 arts-2024.4.3.1/arts/CoolMemory-English/Copyright
--rw-r--r--   0        0        0    10294 2024-03-31 09:22:44.234618 arts-2024.4.3.1/arts/CoolMemory-English/README.md
--rw-r--r--   0        0        0      110 2024-03-06 00:07:28.301653 arts-2024.4.3.1/arts/CoolMemory-English/art.json
--rw-r--r--   0        0        0      393 2023-12-10 08:00:44.000000 arts-2024.4.3.1/arts/CoolMemory-English/licenses/README.md
--rw-r--r--   0        0        0     1586 2023-12-10 08:00:44.000000 arts-2024.4.3.1/arts/CoolMemory-English/licenses/licenses/Chromium/LICENSE
--rw-r--r--   0        0        0    11550 2023-12-10 08:00:44.000000 arts-2024.4.3.1/arts/CoolMemory-English/licenses/licenses/Nuitka/LICENSE
--rw-r--r--   0        0        0    32825 2023-12-10 08:00:44.000000 arts-2024.4.3.1/arts/CoolMemory-English/licenses/licenses/Python/LICENSE
--rw-r--r--   0        0        0     2987 2023-12-10 08:00:44.000000 arts-2024.4.3.1/arts/CoolMemory-English/licenses/licenses/pycryptodome/LICENSE
--rw-r--r--   0        0        0     1166 2023-12-10 08:00:44.000000 arts-2024.4.3.1/arts/CoolMemory-English/licenses/licenses/pyppeteer/LICENSE
--rw-r--r--   0        0        0    11560 2023-12-10 08:00:44.000000 arts-2024.4.3.1/arts/CoolMemory-English/licenses/licenses/tornado/LICENSE
--rw-r--r--   0        0        0      106 2024-03-31 10:18:29.252509 arts-2024.4.3.1/arts/WeChat-Art-Museum/art.json
--rw-r--r--   0        0        0    52568 2024-04-03 07:18:46.648497 arts-2024.4.3.1/arts/WeChat-Art-Museum/index.html
--rw-r--r--   0        0        0        0 2024-02-22 15:47:26.927352 arts-2024.4.3.1/arts/__init__.py
--rw-r--r--   0        0        0     3088 2023-09-24 08:08:30.000000 arts-2024.4.3.1/arts/articles/010-赚钱宝典/010-财富的本质/README.md
--rw-r--r--   0        0        0       44 2023-12-19 10:01:11.532367 arts-2024.4.3.1/arts/articles/010-赚钱宝典/010-财富的本质/art.json
--rw-r--r--   0        0        0     1681 2023-12-20 10:09:07.827303 arts-2024.4.3.1/arts/articles/010-赚钱宝典/020-商业价值/README.md
--rw-r--r--   0        0        0       44 2023-12-19 10:01:11.533332 arts-2024.4.3.1/arts/articles/010-赚钱宝典/020-商业价值/art.json
--rw-r--r--   0        0        0     3552 2023-12-22 07:27:54.636897 arts-2024.4.3.1/arts/articles/010-赚钱宝典/030-财富稳定型社会/README.md
--rw-r--r--   0        0        0       44 2023-12-22 07:26:00.584312 arts-2024.4.3.1/arts/articles/010-赚钱宝典/030-财富稳定型社会/art.json
--rw-r--r--   0        0        0     1812 2024-01-02 20:05:02.520382 arts-2024.4.3.1/arts/articles/075-追英赶美/300-产业升级与失业潮/README.md
--rw-r--r--   0        0        0       44 2024-01-02 20:46:41.567445 arts-2024.4.3.1/arts/articles/075-追英赶美/300-产业升级与失业潮/art.json
--rw-r--r--   0        0        0     1253 2024-01-18 01:49:14.297346 arts-2024.4.3.1/arts/articles/075-追英赶美/600-在ChatGPT冲击下，打造国家级公共知识库迫在眉睫/README.md
--rw-r--r--   0        0        0       44 2024-01-02 20:47:04.916014 arts-2024.4.3.1/arts/articles/075-追英赶美/600-在ChatGPT冲击下，打造国家级公共知识库迫在眉睫/art.json
--rw-r--r--   0        0        0     1559 2023-11-15 13:45:10.000000 arts-2024.4.3.1/arts/articles/150-小民参政/300-广义的民主/README.md
--rw-r--r--   0        0        0       44 2023-12-19 10:02:18.547561 arts-2024.4.3.1/arts/articles/150-小民参政/300-广义的民主/art.json
--rw-r--r--   0        0        0     1499 2023-10-24 11:49:00.000000 arts-2024.4.3.1/arts/articles/150-小民参政/600-年轻人不结婚是文明的进步/README.md
--rw-r--r--   0        0        0       44 2023-12-19 10:02:18.545561 arts-2024.4.3.1/arts/articles/150-小民参政/600-年轻人不结婚是文明的进步/art.json
--rw-r--r--   0        0        0     1450 2023-11-05 04:22:04.000000 arts-2024.4.3.1/arts/articles/300-批判那些伪文艺/200-一元官司有意义吗？/README.md
--rw-r--r--   0        0        0       44 2023-12-19 10:03:07.648073 arts-2024.4.3.1/arts/articles/300-批判那些伪文艺/200-一元官司有意义吗？/art.json
--rw-r--r--   0        0        0     3278 2024-02-25 10:11:51.363950 arts-2024.4.3.1/arts/articles/300-批判那些伪文艺/400-唯有变化是不变的？/README.md
--rw-r--r--   0        0        0       44 2023-12-19 10:03:07.644190 arts-2024.4.3.1/arts/articles/300-批判那些伪文艺/400-唯有变化是不变的？/art.json
--rw-r--r--   0        0        0     1265 2024-03-28 16:30:38.111960 arts-2024.4.3.1/arts/articles/300-批判那些伪文艺/600-未经他人苦，莫劝他人善？/README.md
--rw-r--r--   0        0        0       44 2023-12-19 10:03:07.645220 arts-2024.4.3.1/arts/articles/300-批判那些伪文艺/600-未经他人苦，莫劝他人善？/art.json
--rw-r--r--   0        0        0     1135 2024-03-04 05:13:36.283230 arts-2024.4.3.1/arts/articles/300-批判那些伪文艺/800-务实与务虚/README.md
--rw-r--r--   0        0        0       44 2023-12-19 10:03:07.647184 arts-2024.4.3.1/arts/articles/300-批判那些伪文艺/800-务实与务虚/art.json
--rw-r--r--   0        0        0     2095 2024-01-18 01:48:33.751985 arts-2024.4.3.1/arts/articles/450-万象思考/050-ChatGPT已经有自我意识了/README.md
--rw-r--r--   0        0        0       44 2023-12-19 10:04:00.900873 arts-2024.4.3.1/arts/articles/450-万象思考/050-ChatGPT已经有自我意识了/art.json
--rw-r--r--   0        0        0     1668 2023-11-05 03:35:50.000000 arts-2024.4.3.1/arts/articles/450-万象思考/100-怎么理解「迷信科学」？/README.md
--rw-r--r--   0        0        0       44 2023-12-19 10:04:00.909872 arts-2024.4.3.1/arts/articles/450-万象思考/100-怎么理解「迷信科学」？/art.json
--rw-r--r--   0        0        0     1669 2023-11-15 13:41:24.000000 arts-2024.4.3.1/arts/articles/450-万象思考/150-心理学中个案研究有意义吗？/README.md
--rw-r--r--   0        0        0       44 2023-12-19 10:04:00.903896 arts-2024.4.3.1/arts/articles/450-万象思考/150-心理学中个案研究有意义吗？/art.json
--rw-r--r--   0        0        0     1906 2023-12-27 20:37:35.730568 arts-2024.4.3.1/arts/articles/450-万象思考/200-人工智能会不会统治人类？/README.md
--rw-r--r--   0        0        0       44 2023-12-19 10:04:00.899872 arts-2024.4.3.1/arts/articles/450-万象思考/200-人工智能会不会统治人类？/art.json
--rw-r--r--   0        0        0     1154 2023-11-05 02:49:06.000000 arts-2024.4.3.1/arts/articles/450-万象思考/250-忒修斯之船悖论/README.md
--rw-r--r--   0        0        0       44 2023-12-19 10:04:00.907909 arts-2024.4.3.1/arts/articles/450-万象思考/250-忒修斯之船悖论/art.json
--rw-r--r--   0        0        0     3155 2023-12-27 20:37:10.901781 arts-2024.4.3.1/arts/articles/450-万象思考/300-有无相生，难易相成的启发/README.md
--rw-r--r--   0        0        0       44 2024-01-05 13:23:02.578368 arts-2024.4.3.1/arts/articles/450-万象思考/300-有无相生，难易相成的启发/art.json
--rw-r--r--   0        0        0     1354 2023-11-05 03:42:52.000000 arts-2024.4.3.1/arts/articles/450-万象思考/400-熵增都是坏的，熵减都是好的吗？/README.md
--rw-r--r--   0        0        0       44 2024-01-05 13:30:30.884939 arts-2024.4.3.1/arts/articles/450-万象思考/400-熵增都是坏的，熵减都是好的吗？/art.json
--rw-r--r--   0        0        0     1123 2023-09-10 18:11:18.000000 arts-2024.4.3.1/arts/articles/450-万象思考/500-人们为什么希望拥有后代/README.md
--rw-r--r--   0        0        0       44 2023-12-19 10:04:00.906885 arts-2024.4.3.1/arts/articles/450-万象思考/500-人们为什么希望拥有后代/art.json
--rw-r--r--   0        0        0      708 2023-12-27 20:36:45.425482 arts-2024.4.3.1/arts/articles/450-万象思考/600-万物为什么会遵循着物理定律？/README.md
--rw-r--r--   0        0        0       44 2023-12-19 10:04:00.904897 arts-2024.4.3.1/arts/articles/450-万象思考/600-万物为什么会遵循着物理定律？/art.json
--rw-r--r--   0        0        0     5024 2023-11-15 13:32:28.000000 arts-2024.4.3.1/arts/articles/450-万象思考/700-堕胎自由权/README.md
--rw-r--r--   0        0        0       44 2023-12-19 10:04:00.901873 arts-2024.4.3.1/arts/articles/450-万象思考/700-堕胎自由权/art.json
--rw-r--r--   0        0        0     3701 2023-11-15 13:30:02.000000 arts-2024.4.3.1/arts/articles/450-万象思考/800-人人平等是个伪概念/README.md
--rw-r--r--   0        0        0       44 2023-12-19 10:04:00.910899 arts-2024.4.3.1/arts/articles/450-万象思考/800-人人平等是个伪概念/art.json
--rw-r--r--   0        0        0     3385 2023-12-27 20:36:19.402593 arts-2024.4.3.1/arts/articles/600-时空猜想/200-轮回转世真的存在吗？/README.md
--rw-r--r--   0        0        0       44 2023-12-19 10:04:21.414383 arts-2024.4.3.1/arts/articles/600-时空猜想/200-轮回转世真的存在吗？/art.json
--rw-r--r--   0        0        0     2466 2024-02-25 10:07:00.576902 arts-2024.4.3.1/arts/articles/600-时空猜想/400-我们可能处在人造世界/README.md
--rw-r--r--   0        0        0       44 2023-12-19 10:04:21.399805 arts-2024.4.3.1/arts/articles/600-时空猜想/400-我们可能处在人造世界/art.json
--rw-r--r--   0        0        0     3007 2023-11-04 19:08:36.000000 arts-2024.4.3.1/arts/articles/600-时空猜想/600-占卜真的存在吗？/README.md
--rw-r--r--   0        0        0       44 2023-12-19 10:04:21.412423 arts-2024.4.3.1/arts/articles/600-时空猜想/600-占卜真的存在吗？/art.json
--rw-r--r--   0        0        0     2630 2023-11-04 19:15:30.000000 arts-2024.4.3.1/arts/articles/600-时空猜想/800-“自由意志”其实是“随机意志”/README.md
--rw-r--r--   0        0        0       44 2023-12-19 10:04:21.411378 arts-2024.4.3.1/arts/articles/600-时空猜想/800-“自由意志”其实是“随机意志”/art.json
--rw-r--r--   0        0        0     2038 2023-12-28 02:10:43.748193 arts-2024.4.3.1/arts/articles/700-论时事/300-那些年，我们经历过的历史/README.md
--rw-r--r--   0        0        0       44 2023-12-28 02:02:17.049897 arts-2024.4.3.1/arts/articles/700-论时事/300-那些年，我们经历过的历史/art.json
--rw-r--r--   0        0        0     1742 2024-01-13 20:46:22.292355 arts-2024.4.3.1/arts/articles/700-论时事/600-评价在北京工体冲进场的梅西粉丝/README.md
--rw-r--r--   0        0        0       44 2023-12-19 10:04:35.958057 arts-2024.4.3.1/arts/articles/700-论时事/600-评价在北京工体冲进场的梅西粉丝/art.json
--rw-r--r--   0        0        0     7343 2023-06-23 06:29:18.000000 arts-2024.4.3.1/arts/articles/800-小说/300-陆小凤新传/050-燕山宝藏 第1章/README.md
--rw-r--r--   0        0        0       44 2023-12-19 10:05:12.312457 arts-2024.4.3.1/arts/articles/800-小说/300-陆小凤新传/050-燕山宝藏 第1章/art.json
--rw-r--r--   0        0        0     1652 2023-06-23 06:48:36.000000 arts-2024.4.3.1/arts/articles/800-小说/600-一念天堂/050-被绑架/README.md
--rw-r--r--   0        0        0       44 2023-12-19 10:05:34.053435 arts-2024.4.3.1/arts/articles/800-小说/600-一念天堂/050-被绑架/art.json
--rw-r--r--   0        0        0    11283 2024-02-22 12:02:36.224046 arts-2024.4.3.1/arts/cooltypes/LICENSE
--rw-r--r--   0        0        0      293 2024-03-22 15:18:30.564599 arts-2024.4.3.1/arts/cooltypes/__init__.py
--rw-r--r--   0        0        0     1542 2024-03-31 09:40:29.228723 arts-2024.4.3.1/arts/cooltypes/envname/README.md
--rw-r--r--   0        0        0       62 2024-02-23 04:28:30.402332 arts-2024.4.3.1/arts/cooltypes/envname/__init__.py
--rw-r--r--   0        0        0      409 2024-02-23 04:27:58.084752 arts-2024.4.3.1/arts/cooltypes/envname/_core.py
--rw-r--r--   0        0        0      865 2024-02-23 04:12:59.530774 arts-2024.4.3.1/arts/cooltypes/moduledb/README.md
--rw-r--r--   0        0        0       32 2024-02-23 04:03:44.487797 arts-2024.4.3.1/arts/cooltypes/moduledb/__init__.py
--rw-r--r--   0        0        0     3717 2024-02-23 04:15:35.883622 arts-2024.4.3.1/arts/cooltypes/moduledb/_core.py
--rw-r--r--   0        0        0        0 2024-03-11 20:20:36.445694 arts-2024.4.3.1/arts/cooltypes/modules/coolstr/__init__.py
--rw-r--r--   0        0        0     2181 2024-03-22 15:28:12.579126 arts-2024.4.3.1/arts/cooltypes/modules/coolstr/_core.py
--rw-r--r--   0        0        0     3316 2024-03-31 09:40:29.228723 arts-2024.4.3.1/arts/cooltypes/modules/cooltime/README.md
--rw-r--r--   0        0        0        0 2024-03-11 20:20:55.541076 arts-2024.4.3.1/arts/cooltypes/modules/cooltime/__init__.py
--rw-r--r--   0        0        0       44 2024-02-22 10:39:05.460423 arts-2024.4.3.1/arts/cooltypes/modules/cooltime/_art.json
--rw-r--r--   0        0        0     3665 2024-03-22 15:09:31.411034 arts-2024.4.3.1/arts/cooltypes/modules/cooltime/_core.py
--rw-r--r--   0        0        0     5793 2024-03-22 15:12:37.868753 arts-2024.4.3.1/arts/cooltypes/modules/rslice/README.md
--rw-r--r--   0        0        0        0 2024-03-11 20:26:19.316480 arts-2024.4.3.1/arts/cooltypes/modules/rslice/__init__.py
--rw-r--r--   0        0        0     2801 2024-03-22 15:12:37.864736 arts-2024.4.3.1/arts/cooltypes/modules/rslice/_core.py
--rw-r--r--   0        0        0        0 2024-03-11 20:22:01.981114 arts-2024.4.3.1/arts/cooltypes/modules/vtype/__init__.py
--rw-r--r--   0        0        0    10008 2024-03-22 15:22:10.216978 arts-2024.4.3.1/arts/cooltypes/modules/vtype/_core.py
--rw-r--r--   0        0        0      238 2024-03-22 14:31:42.101320 arts-2024.4.3.1/arts/cooltypes/设计.md
--rw-r--r--   0        0        0    59836 2024-04-06 05:36:30.679243 arts-2024.4.3.1/arts/index.html
--rw-r--r--   0        0        0       44 2024-01-16 13:04:45.523107 arts-2024.4.3.1/arts/life/2018/莆田学院·毕业生留影/art.json
--rw-r--r--   0        0        0      830 2024-02-12 15:02:22.123647 arts-2024.4.3.1/arts/life/2018/莆田学院·毕业生留影/index.html
--rw-r--r--   0        0        0       44 2024-01-17 04:28:07.076300 arts-2024.4.3.1/arts/life/2019/苏州市虎丘山/art.json
--rw-r--r--   0        0        0     1233 2024-03-24 16:39:19.059155 arts-2024.4.3.1/arts/life/2019/苏州市虎丘山/index.html
--rw-r--r--   0        0        0       44 2024-01-17 03:40:13.294365 arts-2024.4.3.1/arts/life/2022/泉州市丰泽区·雨后街道/art.json
--rw-r--r--   0        0        0      969 2024-03-24 16:39:36.018072 arts-2024.4.3.1/arts/life/2022/泉州市丰泽区·雨后街道/index.html
--rw-r--r--   0        0        0       44 2024-01-30 05:00:40.402244 arts-2024.4.3.1/arts/life/2023/更换微信账号了/art.json
--rw-r--r--   0        0        0      898 2024-04-03 03:17:39.386427 arts-2024.4.3.1/arts/life/2023/更换微信账号了/index.html
--rw-r--r--   0        0        0       44 2024-03-24 16:41:15.708702 arts-2024.4.3.1/arts/life/2024/泉州市承天禅寺/art.json
--rw-r--r--   0        0        0     1133 2024-03-25 03:52:07.749983 arts-2024.4.3.1/arts/life/2024/泉州市承天禅寺/index.html
--rw-r--r--   0        0        0    11276 2024-02-22 12:02:36.224046 arts-2024.4.3.1/arts/miumapp/LICENSE
--rw-r--r--   0        0        0     5762 2024-03-31 09:40:29.228723 arts-2024.4.3.1/arts/miumapp/README.md
--rw-r--r--   0        0        0       36 2024-02-12 15:08:38.569224 arts-2024.4.3.1/arts/miumapp/__init__.py
--rw-r--r--   0        0        0     7747 2024-03-25 04:09:08.267200 arts-2024.4.3.1/arts/miumapp/_core.py
--rw-r--r--   0        0        0      111 2024-03-05 23:26:53.659150 arts-2024.4.3.1/arts/miumapp/art.json
--rw-r--r--   0        0        0      245 2023-09-04 06:15:02.000000 arts-2024.4.3.1/arts/miumapp/licenses/README.md
--rw-r--r--   0        0        0     1166 2023-12-10 08:00:44.000000 arts-2024.4.3.1/arts/miumapp/licenses/pyppeteer/LICENSE
--rw-r--r--   0        0        0    11560 2023-12-10 08:00:44.000000 arts-2024.4.3.1/arts/miumapp/licenses/tornado/LICENSE
--rw-r--r--   0        0        0       48 2024-02-12 15:15:42.556195 arts-2024.4.3.1/arts/miumapp/miumapp/__init__.py
--rw-r--r--   0        0        0     4657 2024-02-22 17:30:50.375647 arts-2024.4.3.1/arts/miumapp/miumapp/demo.html
--rw-r--r--   0        0        0     1241 2024-03-25 04:09:36.827762 arts-2024.4.3.1/arts/miumapp/miumapp/demo.py
--rw-r--r--   0        0        0      645 2024-03-12 12:18:10.837369 arts-2024.4.3.1/arts/miumapp/pyproject.toml
--rw-r--r--   0        0        0    11273 2024-03-02 20:20:55.781363 arts-2024.4.3.1/arts/oodb/LICENSE
--rw-r--r--   0        0        0    22563 2024-03-31 09:40:29.216952 arts-2024.4.3.1/arts/oodb/README.md
--rw-r--r--   0        0        0       44 2024-03-06 00:36:04.879589 arts-2024.4.3.1/arts/oodb/__init__.py
--rw-r--r--   0        0        0    19029 2024-03-06 09:46:30.072966 arts-2024.4.3.1/arts/oodb/_core.py
--rw-r--r--   0        0        0       99 2024-03-06 01:01:05.433633 arts-2024.4.3.1/arts/oodb/art.json
--rw-r--r--   0        0        0      245 2023-09-04 06:15:02.000000 arts-2024.4.3.1/arts/oodb/licenses/README.md
--rw-r--r--   0        0        0    11357 2022-11-17 21:35:26.000000 arts-2024.4.3.1/arts/oodb/licenses/pymongo/LICENSE
--rw-r--r--   0        0        0       53 2024-03-06 00:36:04.879589 arts-2024.4.3.1/arts/oodb/oodb.py
--rw-r--r--   0        0        0      626 2024-03-06 09:57:01.274330 arts-2024.4.3.1/arts/oodb/pyproject.toml
--rw-r--r--   0        0        0    11281 2024-03-03 07:09:08.518004 arts-2024.4.3.1/arts/oomongo/LICENSE
--rw-r--r--   0        0        0    17439 2024-03-31 09:40:29.227707 arts-2024.4.3.1/arts/oomongo/README.md
--rw-r--r--   0        0        0       49 2024-03-05 08:01:41.054010 arts-2024.4.3.1/arts/oomongo/__init__.py
--rw-r--r--   0        0        0    27613 2024-03-06 00:34:47.221863 arts-2024.4.3.1/arts/oomongo/_core.py
--rw-r--r--   0        0        0       92 2024-03-06 00:50:10.273786 arts-2024.4.3.1/arts/oomongo/art.json
--rw-r--r--   0        0        0      245 2023-09-04 06:15:02.000000 arts-2024.4.3.1/arts/oomongo/licenses/README.md
--rw-r--r--   0        0        0    11357 2022-10-25 20:46:40.000000 arts-2024.4.3.1/arts/oomongo/licenses/motor/LICENSE
--rw-r--r--   0        0        0    11357 2022-11-17 21:35:26.000000 arts-2024.4.3.1/arts/oomongo/licenses/pymongo/LICENSE
--rw-r--r--   0        0        0       61 2024-03-05 08:01:41.059008 arts-2024.4.3.1/arts/oomongo/oomongo.py
--rw-r--r--   0        0        0      563 2024-03-06 00:09:25.377118 arts-2024.4.3.1/arts/oomongo/pyproject.toml
--rw-r--r--   0        0        0    11281 2024-03-03 07:10:17.933453 arts-2024.4.3.1/arts/oomysql/LICENSE
--rw-r--r--   0        0        0    17139 2024-03-31 09:40:29.228723 arts-2024.4.3.1/arts/oomysql/README.md
--rw-r--r--   0        0        0       45 2024-03-05 08:02:05.322948 arts-2024.4.3.1/arts/oomysql/__init__.py
--rw-r--r--   0        0        0    35301 2024-03-24 00:57:24.021318 arts-2024.4.3.1/arts/oomysql/_core.py
--rw-r--r--   0        0        0       90 2024-03-06 00:10:16.490984 arts-2024.4.3.1/arts/oomysql/art.json
--rw-r--r--   0        0        0      245 2023-09-04 06:15:02.000000 arts-2024.4.3.1/arts/oomysql/licenses/README.md
--rw-r--r--   0        0        0     1070 2022-05-08 19:03:56.000000 arts-2024.4.3.1/arts/oomysql/licenses/aiomysql/LICENSE
--rw-r--r--   0        0        0     1070 2013-11-27 14:43:24.000000 arts-2024.4.3.1/arts/oomysql/licenses/pymysql/LICENSE
--rw-r--r--   0        0        0       57 2024-03-05 08:02:05.335929 arts-2024.4.3.1/arts/oomysql/oomysql.py
--rw-r--r--   0        0        0      641 2024-03-06 00:09:38.203916 arts-2024.4.3.1/arts/oomysql/pyproject.toml
--rw-r--r--   0        0        0    11281 2024-02-22 12:02:36.209038 arts-2024.4.3.1/arts/openai2/LICENSE
--rw-r--r--   0        0        0    13971 2024-03-31 09:40:29.216952 arts-2024.4.3.1/arts/openai2/README.md
--rw-r--r--   0        0        0      167 2023-12-19 12:18:48.792856 arts-2024.4.3.1/arts/openai2/__init__.py
--rw-r--r--   0        0        0     6923 2023-11-15 22:45:46.000000 arts-2024.4.3.1/arts/openai2/_core/GroupChat.py
--rw-r--r--   0        0        0     9298 2024-04-06 05:34:07.115496 arts-2024.4.3.1/arts/openai2/_core/chat.py
--rw-r--r--   0        0        0     2279 2024-02-23 04:06:51.826269 arts-2024.4.3.1/arts/openai2/_core/chat_in_cmd.py
--rw-r--r--   0        0        0       99 2024-03-05 23:28:04.263728 arts-2024.4.3.1/arts/openai2/art.json
--rw-r--r--   0        0        0      245 2023-09-04 06:15:02.000000 arts-2024.4.3.1/arts/openai2/licenses/README.md
--rw-r--r--   0        0        0     1083 2020-12-22 18:45:04.000000 arts-2024.4.3.1/arts/openai2/licenses/openai/LICENSE
--rw-r--r--   0        0        0      203 2024-03-03 10:11:45.701543 arts-2024.4.3.1/arts/openai2/openai2.py
--rw-r--r--   0        0        0      805 2024-04-06 05:38:16.070983 arts-2024.4.3.1/arts/openai2/pyproject.toml
--rw-r--r--   0        0        0      231 2024-02-25 03:34:44.558335 arts-2024.4.3.1/arts/skybox/Copyright
--rw-r--r--   0        0        0      735 2024-02-25 06:24:00.741491 arts-2024.4.3.1/arts/skybox/README.md
--rw-r--r--   0        0        0      320 2024-04-03 06:26:06.014092 arts-2024.4.3.1/arts/skybox/pyproject.toml
--rw-r--r--   0        0        0      231 2024-02-25 03:34:44.558335 arts-2024.4.3.1/arts/skybox/skybox/Copyright
--rw-r--r--   0        0        0      156 2024-02-25 06:24:00.741491 arts-2024.4.3.1/arts/skybox/skybox/__init__.py
--rw-r--r--   0        0        0    12359 2024-04-03 06:25:47.716340 arts-2024.4.3.1/arts/skybox/skybox/files_hashes
--rw-r--r--   0        0        0       44 2023-12-19 10:10:36.391618 arts-2024.4.3.1/arts/thoughts/2022/现代工人的螺丝钉处境/art.json
--rw-r--r--   0        0        0     1374 2024-01-16 22:36:30.326371 arts-2024.4.3.1/arts/thoughts/2022/现代工人的螺丝钉处境/index.html
--rw-r--r--   0        0        0       44 2023-12-19 10:11:02.542208 arts-2024.4.3.1/arts/thoughts/2023/ChatGPT动了学阀的蛋糕/art.json
--rw-r--r--   0        0        0     1346 2024-01-30 04:04:01.359662 arts-2024.4.3.1/arts/thoughts/2023/ChatGPT动了学阀的蛋糕/index.html
--rw-r--r--   0        0        0       44 2023-12-19 10:11:02.562268 arts-2024.4.3.1/arts/thoughts/2023/专利是个公平的赛道/art.json
--rw-r--r--   0        0        0     1340 2024-03-27 02:41:37.370555 arts-2024.4.3.1/arts/thoughts/2023/专利是个公平的赛道/index.html
--rw-r--r--   0        0        0       44 2023-12-19 10:11:02.547209 arts-2024.4.3.1/arts/thoughts/2023/事情的真实性是由度的/art.json
--rw-r--r--   0        0        0     1001 2024-01-16 22:36:30.329386 arts-2024.4.3.1/arts/thoughts/2023/事情的真实性是由度的/index.html
--rw-r--r--   0        0        0       44 2023-12-19 10:11:02.556244 arts-2024.4.3.1/arts/thoughts/2023/人无法摆脱兽性/art.json
--rw-r--r--   0        0        0     1659 2024-01-16 22:36:30.330406 arts-2024.4.3.1/arts/thoughts/2023/人无法摆脱兽性/index.html
--rw-r--r--   0        0        0       44 2023-12-19 10:11:02.551211 arts-2024.4.3.1/arts/thoughts/2023/什么是极端？/art.json
--rw-r--r--   0        0        0      884 2024-01-16 22:36:30.330406 arts-2024.4.3.1/arts/thoughts/2023/什么是极端？/index.html
--rw-r--r--   0        0        0       44 2023-12-19 10:11:02.541243 arts-2024.4.3.1/arts/thoughts/2023/保护好人/art.json
--rw-r--r--   0        0        0      802 2024-01-16 22:36:30.331373 arts-2024.4.3.1/arts/thoughts/2023/保护好人/index.html
--rw-r--r--   0        0        0       44 2023-12-19 10:11:02.554209 arts-2024.4.3.1/arts/thoughts/2023/只筛选，不教化/art.json
--rw-r--r--   0        0        0      853 2024-01-16 22:36:30.331373 arts-2024.4.3.1/arts/thoughts/2023/只筛选，不教化/index.html
--rw-r--r--   0        0        0       44 2023-12-19 10:11:02.549209 arts-2024.4.3.1/arts/thoughts/2023/喊高考加油是刷存在感/art.json
--rw-r--r--   0        0        0     1047 2024-01-16 22:36:30.332406 arts-2024.4.3.1/arts/thoughts/2023/喊高考加油是刷存在感/index.html
--rw-r--r--   0        0        0       44 2023-12-19 10:11:02.552210 arts-2024.4.3.1/arts/thoughts/2023/宣扬出来的宽容是恶的代名词/art.json
--rw-r--r--   0        0        0     1630 2024-01-16 22:36:30.333372 arts-2024.4.3.1/arts/thoughts/2023/宣扬出来的宽容是恶的代名词/index.html
--rw-r--r--   0        0        0       44 2023-12-19 10:11:02.553243 arts-2024.4.3.1/arts/thoughts/2023/对ChatGPT将带来的变革感到不知所措/art.json
--rw-r--r--   0        0        0     2475 2024-01-30 04:03:34.796607 arts-2024.4.3.1/arts/thoughts/2023/对ChatGPT将带来的变革感到不知所措/index.html
--rw-r--r--   0        0        0       44 2023-12-19 10:11:02.561243 arts-2024.4.3.1/arts/thoughts/2023/强人工智能真的出现了，那就是 ChatGPT-4/art.json
--rw-r--r--   0        0        0      833 2024-01-18 01:51:26.994040 arts-2024.4.3.1/arts/thoughts/2023/强人工智能真的出现了，那就是 ChatGPT-4/index.html
--rw-r--r--   0        0        0       44 2023-12-19 10:11:02.545246 arts-2024.4.3.1/arts/thoughts/2023/想去国外了解自己/art.json
--rw-r--r--   0        0        0      966 2024-01-16 22:36:30.335371 arts-2024.4.3.1/arts/thoughts/2023/想去国外了解自己/index.html
--rw-r--r--   0        0        0       44 2023-12-19 10:11:02.548245 arts-2024.4.3.1/arts/thoughts/2023/现代化的分工合作机制/art.json
--rw-r--r--   0        0        0     1668 2024-01-16 22:36:30.335371 arts-2024.4.3.1/arts/thoughts/2023/现代化的分工合作机制/index.html
--rw-r--r--   0        0        0       44 2023-12-19 10:11:02.544210 arts-2024.4.3.1/arts/thoughts/2023/用理性处理简单的事情/art.json
--rw-r--r--   0        0        0     1587 2024-01-16 22:36:30.336371 arts-2024.4.3.1/arts/thoughts/2023/用理性处理简单的事情/index.html
--rw-r--r--   0        0        0       44 2023-12-19 10:11:02.557226 arts-2024.4.3.1/arts/thoughts/2023/真正的问题无法通过花招解决/art.json
--rw-r--r--   0        0        0      977 2024-01-16 22:36:30.336371 arts-2024.4.3.1/arts/thoughts/2023/真正的问题无法通过花招解决/index.html
--rw-r--r--   0        0        0       44 2023-12-19 10:11:02.560208 arts-2024.4.3.1/arts/thoughts/2023/艺术本天成，媒介偶显之/art.json
--rw-r--r--   0        0        0      629 2024-01-16 22:36:30.337410 arts-2024.4.3.1/arts/thoughts/2023/艺术本天成，媒介偶显之/index.html
--rw-r--r--   0        0        0       44 2023-12-19 10:11:02.558244 arts-2024.4.3.1/arts/thoughts/2023/阳光下的美好是以阴影中的丑陋为代价/art.json
--rw-r--r--   0        0        0     1168 2024-01-16 22:36:30.338372 arts-2024.4.3.1/arts/thoughts/2023/阳光下的美好是以阴影中的丑陋为代价/index.html
--rw-r--r--   0        0        0       44 2024-01-13 21:13:40.122707 arts-2024.4.3.1/arts/thoughts/2024/不要害怕犯错/art.json
--rw-r--r--   0        0        0      698 2024-01-16 22:36:30.339373 arts-2024.4.3.1/arts/thoughts/2024/不要害怕犯错/index.html
--rw-r--r--   0        0        0       44 2024-01-01 14:23:12.130009 arts-2024.4.3.1/arts/thoughts/2024/新年题诗/art.json
--rw-r--r--   0        0        0     1152 2024-01-18 06:19:08.705581 arts-2024.4.3.1/arts/thoughts/2024/新年题诗/index.html
--rw-r--r--   0        0        0       44 2024-01-03 04:10:15.709103 arts-2024.4.3.1/arts/thoughts/2024/比特币无法成为取缔实体货币的最终币种/art.json
--rw-r--r--   0        0        0     1270 2024-01-16 22:36:30.341372 arts-2024.4.3.1/arts/thoughts/2024/比特币无法成为取缔实体货币的最终币种/index.html
--rw-r--r--   0        0        0       44 2024-03-24 15:35:39.622105 arts-2024.4.3.1/arts/thoughts/2024/编程语言的进化/art.json
--rw-r--r--   0        0        0     1022 2024-03-24 16:22:12.389078 arts-2024.4.3.1/arts/thoughts/2024/编程语言的进化/example.html
--rw-r--r--   0        0        0     1520 2024-03-25 03:53:51.266590 arts-2024.4.3.1/arts/thoughts/2024/编程语言的进化/index.html
--rw-r--r--   0        0        0       44 2024-01-30 04:08:51.850343 arts-2024.4.3.1/arts/thoughts/2024/萝莉岛事件引发的信任危机/art.json
--rw-r--r--   0        0        0     1077 2024-01-30 04:15:45.681734 arts-2024.4.3.1/arts/thoughts/2024/萝莉岛事件引发的信任危机/index.html
--rw-r--r--   0        0        0       44 2024-01-18 06:20:18.873404 arts-2024.4.3.1/arts/thoughts/2024/霍金去萝莉岛干嘛了/art.json
--rw-r--r--   0        0        0     1174 2024-01-18 06:24:05.339876 arts-2024.4.3.1/arts/thoughts/2024/霍金去萝莉岛干嘛了/index.html
--rw-r--r--   0        0        0      103 2024-03-03 07:12:46.987154 arts-2024.4.3.1/arts/tutorials/150-操作MySQL/art.json
--rw-r--r--   0        0        0      103 2024-03-06 00:50:30.486267 arts-2024.4.3.1/arts/tutorials/225-操作MongoDB/art.json
--rw-r--r--   0        0        0      146 2024-02-25 14:11:14.480558 arts-2024.4.3.1/arts/tutorials/300-开发桌面GUI应用/art.json
--rw-r--r--   0        0        0      103 2024-02-18 14:43:25.042841 arts-2024.4.3.1/arts/tutorials/450-对接ChatGPT/art.json
--rw-r--r--   0        0        0      122 2024-03-22 15:10:08.573597 arts-2024.4.3.1/arts/tutorials/525-时间模块/art.json
--rw-r--r--   0        0        0      100 2024-03-06 01:01:25.689741 arts-2024.4.3.1/arts/tutorials/562-面向对象数据库/art.json
--rw-r--r--   0        0        0     3415 2023-12-20 10:09:07.822297 arts-2024.4.3.1/arts/tutorials/600-用37行代码实现AI五子棋/README.md
--rw-r--r--   0        0        0       44 2023-12-19 10:14:03.255370 arts-2024.4.3.1/arts/tutorials/600-用37行代码实现AI五子棋/art.json
--rw-r--r--   0        0        0     8070 2024-02-25 05:45:21.624081 arts-2024.4.3.1/arts/tutorials/750-正则表达式/README.md
--rw-r--r--   0        0        0       44 2023-12-19 10:13:55.412792 arts-2024.4.3.1/arts/tutorials/750-正则表达式/art.json
--rw-r--r--   0        0        0       44 2024-01-30 03:46:52.790397 arts-2024.4.3.1/arts/videos/200-秦时明月[项羽]·谪居/art.json
--rw-r--r--   0        0        0       44 2023-12-19 10:07:05.944886 arts-2024.4.3.1/arts/videos/400-李连杰[霍元甲]·兰亭序/art.json
--rw-r--r--   0        0        0       44 2023-12-19 10:07:05.933448 arts-2024.4.3.1/arts/videos/600-楚门的世界·五月雨/art.json
--rw-r--r--   0        0        0       44 2024-01-05 13:31:13.729378 arts-2024.4.3.1/arts/videos/800-AI是这样画包拯的/art.json
--rw-r--r--   0        0        0      526 2024-04-06 05:37:48.848464 arts-2024.4.3.1/pyproject.toml
--rw-r--r--   0        0        0      530 1970-01-01 00:00:00.000000 arts-2024.4.3.1/PKG-INFO
+-rw-r--r--   0        0        0     2175 2023-12-20 10:09:43.709218 arts-2024.4.3.2/.gitignore
+-rw-r--r--   0        0        0       46 2024-03-10 10:13:06.948005 arts-2024.4.3.2/README.md
+-rw-r--r--   0        0        0      317 2024-02-22 12:02:36.224046 arts-2024.4.3.2/arts/CoolMemory-English/Copyright
+-rw-r--r--   0        0        0    10294 2024-03-31 09:22:44.234618 arts-2024.4.3.2/arts/CoolMemory-English/README.md
+-rw-r--r--   0        0        0      110 2024-03-06 00:07:28.301653 arts-2024.4.3.2/arts/CoolMemory-English/art.json
+-rw-r--r--   0        0        0      393 2023-12-10 08:00:44.000000 arts-2024.4.3.2/arts/CoolMemory-English/licenses/README.md
+-rw-r--r--   0        0        0     1586 2023-12-10 08:00:44.000000 arts-2024.4.3.2/arts/CoolMemory-English/licenses/licenses/Chromium/LICENSE
+-rw-r--r--   0        0        0    11550 2023-12-10 08:00:44.000000 arts-2024.4.3.2/arts/CoolMemory-English/licenses/licenses/Nuitka/LICENSE
+-rw-r--r--   0        0        0    32825 2023-12-10 08:00:44.000000 arts-2024.4.3.2/arts/CoolMemory-English/licenses/licenses/Python/LICENSE
+-rw-r--r--   0        0        0     2987 2023-12-10 08:00:44.000000 arts-2024.4.3.2/arts/CoolMemory-English/licenses/licenses/pycryptodome/LICENSE
+-rw-r--r--   0        0        0     1166 2023-12-10 08:00:44.000000 arts-2024.4.3.2/arts/CoolMemory-English/licenses/licenses/pyppeteer/LICENSE
+-rw-r--r--   0        0        0    11560 2023-12-10 08:00:44.000000 arts-2024.4.3.2/arts/CoolMemory-English/licenses/licenses/tornado/LICENSE
+-rw-r--r--   0        0        0      106 2024-03-31 10:18:29.252509 arts-2024.4.3.2/arts/WeChat-Art-Museum/art.json
+-rw-r--r--   0        0        0    52568 2024-04-03 07:18:46.648497 arts-2024.4.3.2/arts/WeChat-Art-Museum/index.html
+-rw-r--r--   0        0        0        0 2024-02-22 15:47:26.927352 arts-2024.4.3.2/arts/__init__.py
+-rw-r--r--   0        0        0     3088 2023-09-24 08:08:30.000000 arts-2024.4.3.2/arts/articles/010-赚钱宝典/010-财富的本质/README.md
+-rw-r--r--   0        0        0       44 2023-12-19 10:01:11.532367 arts-2024.4.3.2/arts/articles/010-赚钱宝典/010-财富的本质/art.json
+-rw-r--r--   0        0        0     1681 2023-12-20 10:09:07.827303 arts-2024.4.3.2/arts/articles/010-赚钱宝典/020-商业价值/README.md
+-rw-r--r--   0        0        0       44 2023-12-19 10:01:11.533332 arts-2024.4.3.2/arts/articles/010-赚钱宝典/020-商业价值/art.json
+-rw-r--r--   0        0        0     3552 2023-12-22 07:27:54.636897 arts-2024.4.3.2/arts/articles/010-赚钱宝典/030-财富稳定型社会/README.md
+-rw-r--r--   0        0        0       44 2023-12-22 07:26:00.584312 arts-2024.4.3.2/arts/articles/010-赚钱宝典/030-财富稳定型社会/art.json
+-rw-r--r--   0        0        0     1812 2024-01-02 20:05:02.520382 arts-2024.4.3.2/arts/articles/075-追英赶美/300-产业升级与失业潮/README.md
+-rw-r--r--   0        0        0       44 2024-01-02 20:46:41.567445 arts-2024.4.3.2/arts/articles/075-追英赶美/300-产业升级与失业潮/art.json
+-rw-r--r--   0        0        0     1253 2024-01-18 01:49:14.297346 arts-2024.4.3.2/arts/articles/075-追英赶美/600-在ChatGPT冲击下，打造国家级公共知识库迫在眉睫/README.md
+-rw-r--r--   0        0        0       44 2024-01-02 20:47:04.916014 arts-2024.4.3.2/arts/articles/075-追英赶美/600-在ChatGPT冲击下，打造国家级公共知识库迫在眉睫/art.json
+-rw-r--r--   0        0        0     1559 2023-11-15 13:45:10.000000 arts-2024.4.3.2/arts/articles/150-小民参政/300-广义的民主/README.md
+-rw-r--r--   0        0        0       44 2023-12-19 10:02:18.547561 arts-2024.4.3.2/arts/articles/150-小民参政/300-广义的民主/art.json
+-rw-r--r--   0        0        0     1499 2023-10-24 11:49:00.000000 arts-2024.4.3.2/arts/articles/150-小民参政/600-年轻人不结婚是文明的进步/README.md
+-rw-r--r--   0        0        0       44 2023-12-19 10:02:18.545561 arts-2024.4.3.2/arts/articles/150-小民参政/600-年轻人不结婚是文明的进步/art.json
+-rw-r--r--   0        0        0     1450 2023-11-05 04:22:04.000000 arts-2024.4.3.2/arts/articles/300-批判那些伪文艺/200-一元官司有意义吗？/README.md
+-rw-r--r--   0        0        0       44 2023-12-19 10:03:07.648073 arts-2024.4.3.2/arts/articles/300-批判那些伪文艺/200-一元官司有意义吗？/art.json
+-rw-r--r--   0        0        0     3278 2024-02-25 10:11:51.363950 arts-2024.4.3.2/arts/articles/300-批判那些伪文艺/400-唯有变化是不变的？/README.md
+-rw-r--r--   0        0        0       44 2023-12-19 10:03:07.644190 arts-2024.4.3.2/arts/articles/300-批判那些伪文艺/400-唯有变化是不变的？/art.json
+-rw-r--r--   0        0        0     1265 2024-03-28 16:30:38.111960 arts-2024.4.3.2/arts/articles/300-批判那些伪文艺/600-未经他人苦，莫劝他人善？/README.md
+-rw-r--r--   0        0        0       44 2023-12-19 10:03:07.645220 arts-2024.4.3.2/arts/articles/300-批判那些伪文艺/600-未经他人苦，莫劝他人善？/art.json
+-rw-r--r--   0        0        0     1135 2024-03-04 05:13:36.283230 arts-2024.4.3.2/arts/articles/300-批判那些伪文艺/800-务实与务虚/README.md
+-rw-r--r--   0        0        0       44 2023-12-19 10:03:07.647184 arts-2024.4.3.2/arts/articles/300-批判那些伪文艺/800-务实与务虚/art.json
+-rw-r--r--   0        0        0     2095 2024-01-18 01:48:33.751985 arts-2024.4.3.2/arts/articles/450-万象思考/050-ChatGPT已经有自我意识了/README.md
+-rw-r--r--   0        0        0       44 2023-12-19 10:04:00.900873 arts-2024.4.3.2/arts/articles/450-万象思考/050-ChatGPT已经有自我意识了/art.json
+-rw-r--r--   0        0        0     1668 2023-11-05 03:35:50.000000 arts-2024.4.3.2/arts/articles/450-万象思考/100-怎么理解「迷信科学」？/README.md
+-rw-r--r--   0        0        0       44 2023-12-19 10:04:00.909872 arts-2024.4.3.2/arts/articles/450-万象思考/100-怎么理解「迷信科学」？/art.json
+-rw-r--r--   0        0        0     1669 2023-11-15 13:41:24.000000 arts-2024.4.3.2/arts/articles/450-万象思考/150-心理学中个案研究有意义吗？/README.md
+-rw-r--r--   0        0        0       44 2023-12-19 10:04:00.903896 arts-2024.4.3.2/arts/articles/450-万象思考/150-心理学中个案研究有意义吗？/art.json
+-rw-r--r--   0        0        0     1906 2023-12-27 20:37:35.730568 arts-2024.4.3.2/arts/articles/450-万象思考/200-人工智能会不会统治人类？/README.md
+-rw-r--r--   0        0        0       44 2023-12-19 10:04:00.899872 arts-2024.4.3.2/arts/articles/450-万象思考/200-人工智能会不会统治人类？/art.json
+-rw-r--r--   0        0        0     1154 2023-11-05 02:49:06.000000 arts-2024.4.3.2/arts/articles/450-万象思考/250-忒修斯之船悖论/README.md
+-rw-r--r--   0        0        0       44 2023-12-19 10:04:00.907909 arts-2024.4.3.2/arts/articles/450-万象思考/250-忒修斯之船悖论/art.json
+-rw-r--r--   0        0        0     3155 2023-12-27 20:37:10.901781 arts-2024.4.3.2/arts/articles/450-万象思考/300-有无相生，难易相成的启发/README.md
+-rw-r--r--   0        0        0       44 2024-01-05 13:23:02.578368 arts-2024.4.3.2/arts/articles/450-万象思考/300-有无相生，难易相成的启发/art.json
+-rw-r--r--   0        0        0     1354 2023-11-05 03:42:52.000000 arts-2024.4.3.2/arts/articles/450-万象思考/400-熵增都是坏的，熵减都是好的吗？/README.md
+-rw-r--r--   0        0        0       44 2024-01-05 13:30:30.884939 arts-2024.4.3.2/arts/articles/450-万象思考/400-熵增都是坏的，熵减都是好的吗？/art.json
+-rw-r--r--   0        0        0     1123 2023-09-10 18:11:18.000000 arts-2024.4.3.2/arts/articles/450-万象思考/500-人们为什么希望拥有后代/README.md
+-rw-r--r--   0        0        0       44 2023-12-19 10:04:00.906885 arts-2024.4.3.2/arts/articles/450-万象思考/500-人们为什么希望拥有后代/art.json
+-rw-r--r--   0        0        0      708 2023-12-27 20:36:45.425482 arts-2024.4.3.2/arts/articles/450-万象思考/600-万物为什么会遵循着物理定律？/README.md
+-rw-r--r--   0        0        0       44 2023-12-19 10:04:00.904897 arts-2024.4.3.2/arts/articles/450-万象思考/600-万物为什么会遵循着物理定律？/art.json
+-rw-r--r--   0        0        0     5024 2023-11-15 13:32:28.000000 arts-2024.4.3.2/arts/articles/450-万象思考/700-堕胎自由权/README.md
+-rw-r--r--   0        0        0       44 2023-12-19 10:04:00.901873 arts-2024.4.3.2/arts/articles/450-万象思考/700-堕胎自由权/art.json
+-rw-r--r--   0        0        0     3701 2023-11-15 13:30:02.000000 arts-2024.4.3.2/arts/articles/450-万象思考/800-人人平等是个伪概念/README.md
+-rw-r--r--   0        0        0       44 2023-12-19 10:04:00.910899 arts-2024.4.3.2/arts/articles/450-万象思考/800-人人平等是个伪概念/art.json
+-rw-r--r--   0        0        0     3385 2023-12-27 20:36:19.402593 arts-2024.4.3.2/arts/articles/600-时空猜想/200-轮回转世真的存在吗？/README.md
+-rw-r--r--   0        0        0       44 2023-12-19 10:04:21.414383 arts-2024.4.3.2/arts/articles/600-时空猜想/200-轮回转世真的存在吗？/art.json
+-rw-r--r--   0        0        0     2466 2024-02-25 10:07:00.576902 arts-2024.4.3.2/arts/articles/600-时空猜想/400-我们可能处在人造世界/README.md
+-rw-r--r--   0        0        0       44 2023-12-19 10:04:21.399805 arts-2024.4.3.2/arts/articles/600-时空猜想/400-我们可能处在人造世界/art.json
+-rw-r--r--   0        0        0     3007 2023-11-04 19:08:36.000000 arts-2024.4.3.2/arts/articles/600-时空猜想/600-占卜真的存在吗？/README.md
+-rw-r--r--   0        0        0       44 2023-12-19 10:04:21.412423 arts-2024.4.3.2/arts/articles/600-时空猜想/600-占卜真的存在吗？/art.json
+-rw-r--r--   0        0        0     2630 2023-11-04 19:15:30.000000 arts-2024.4.3.2/arts/articles/600-时空猜想/800-“自由意志”其实是“随机意志”/README.md
+-rw-r--r--   0        0        0       44 2023-12-19 10:04:21.411378 arts-2024.4.3.2/arts/articles/600-时空猜想/800-“自由意志”其实是“随机意志”/art.json
+-rw-r--r--   0        0        0     2038 2023-12-28 02:10:43.748193 arts-2024.4.3.2/arts/articles/700-论时事/300-那些年，我们经历过的历史/README.md
+-rw-r--r--   0        0        0       44 2023-12-28 02:02:17.049897 arts-2024.4.3.2/arts/articles/700-论时事/300-那些年，我们经历过的历史/art.json
+-rw-r--r--   0        0        0     1742 2024-01-13 20:46:22.292355 arts-2024.4.3.2/arts/articles/700-论时事/600-评价在北京工体冲进场的梅西粉丝/README.md
+-rw-r--r--   0        0        0       44 2023-12-19 10:04:35.958057 arts-2024.4.3.2/arts/articles/700-论时事/600-评价在北京工体冲进场的梅西粉丝/art.json
+-rw-r--r--   0        0        0     7343 2023-06-23 06:29:18.000000 arts-2024.4.3.2/arts/articles/800-小说/300-陆小凤新传/050-燕山宝藏 第1章/README.md
+-rw-r--r--   0        0        0       44 2023-12-19 10:05:12.312457 arts-2024.4.3.2/arts/articles/800-小说/300-陆小凤新传/050-燕山宝藏 第1章/art.json
+-rw-r--r--   0        0        0     1652 2023-06-23 06:48:36.000000 arts-2024.4.3.2/arts/articles/800-小说/600-一念天堂/050-被绑架/README.md
+-rw-r--r--   0        0        0       44 2023-12-19 10:05:34.053435 arts-2024.4.3.2/arts/articles/800-小说/600-一念天堂/050-被绑架/art.json
+-rw-r--r--   0        0        0    11283 2024-02-22 12:02:36.224046 arts-2024.4.3.2/arts/cooltypes/LICENSE
+-rw-r--r--   0        0        0      293 2024-03-22 15:18:30.564599 arts-2024.4.3.2/arts/cooltypes/__init__.py
+-rw-r--r--   0        0        0     1542 2024-03-31 09:40:29.228723 arts-2024.4.3.2/arts/cooltypes/envname/README.md
+-rw-r--r--   0        0        0       62 2024-02-23 04:28:30.402332 arts-2024.4.3.2/arts/cooltypes/envname/__init__.py
+-rw-r--r--   0        0        0      409 2024-02-23 04:27:58.084752 arts-2024.4.3.2/arts/cooltypes/envname/_core.py
+-rw-r--r--   0        0        0      865 2024-02-23 04:12:59.530774 arts-2024.4.3.2/arts/cooltypes/moduledb/README.md
+-rw-r--r--   0        0        0       32 2024-02-23 04:03:44.487797 arts-2024.4.3.2/arts/cooltypes/moduledb/__init__.py
+-rw-r--r--   0        0        0     3717 2024-02-23 04:15:35.883622 arts-2024.4.3.2/arts/cooltypes/moduledb/_core.py
+-rw-r--r--   0        0        0        0 2024-03-11 20:20:36.445694 arts-2024.4.3.2/arts/cooltypes/modules/coolstr/__init__.py
+-rw-r--r--   0        0        0     2181 2024-03-22 15:28:12.579126 arts-2024.4.3.2/arts/cooltypes/modules/coolstr/_core.py
+-rw-r--r--   0        0        0     3316 2024-03-31 09:40:29.228723 arts-2024.4.3.2/arts/cooltypes/modules/cooltime/README.md
+-rw-r--r--   0        0        0        0 2024-03-11 20:20:55.541076 arts-2024.4.3.2/arts/cooltypes/modules/cooltime/__init__.py
+-rw-r--r--   0        0        0       44 2024-02-22 10:39:05.460423 arts-2024.4.3.2/arts/cooltypes/modules/cooltime/_art.json
+-rw-r--r--   0        0        0     3665 2024-03-22 15:09:31.411034 arts-2024.4.3.2/arts/cooltypes/modules/cooltime/_core.py
+-rw-r--r--   0        0        0     5793 2024-03-22 15:12:37.868753 arts-2024.4.3.2/arts/cooltypes/modules/rslice/README.md
+-rw-r--r--   0        0        0        0 2024-03-11 20:26:19.316480 arts-2024.4.3.2/arts/cooltypes/modules/rslice/__init__.py
+-rw-r--r--   0        0        0     2801 2024-03-22 15:12:37.864736 arts-2024.4.3.2/arts/cooltypes/modules/rslice/_core.py
+-rw-r--r--   0        0        0        0 2024-03-11 20:22:01.981114 arts-2024.4.3.2/arts/cooltypes/modules/vtype/__init__.py
+-rw-r--r--   0        0        0    10008 2024-03-22 15:22:10.216978 arts-2024.4.3.2/arts/cooltypes/modules/vtype/_core.py
+-rw-r--r--   0        0        0      238 2024-03-22 14:31:42.101320 arts-2024.4.3.2/arts/cooltypes/设计.md
+-rw-r--r--   0        0        0    59836 2024-04-06 05:36:30.679243 arts-2024.4.3.2/arts/index.html
+-rw-r--r--   0        0        0       44 2024-01-16 13:04:45.523107 arts-2024.4.3.2/arts/life/2018/莆田学院·毕业生留影/art.json
+-rw-r--r--   0        0        0      830 2024-02-12 15:02:22.123647 arts-2024.4.3.2/arts/life/2018/莆田学院·毕业生留影/index.html
+-rw-r--r--   0        0        0       44 2024-01-17 04:28:07.076300 arts-2024.4.3.2/arts/life/2019/苏州市虎丘山/art.json
+-rw-r--r--   0        0        0     1233 2024-03-24 16:39:19.059155 arts-2024.4.3.2/arts/life/2019/苏州市虎丘山/index.html
+-rw-r--r--   0        0        0       44 2024-01-17 03:40:13.294365 arts-2024.4.3.2/arts/life/2022/泉州市丰泽区·雨后街道/art.json
+-rw-r--r--   0        0        0      969 2024-03-24 16:39:36.018072 arts-2024.4.3.2/arts/life/2022/泉州市丰泽区·雨后街道/index.html
+-rw-r--r--   0        0        0       44 2024-01-30 05:00:40.402244 arts-2024.4.3.2/arts/life/2023/更换微信账号了/art.json
+-rw-r--r--   0        0        0      898 2024-04-03 03:17:39.386427 arts-2024.4.3.2/arts/life/2023/更换微信账号了/index.html
+-rw-r--r--   0        0        0       44 2024-03-24 16:41:15.708702 arts-2024.4.3.2/arts/life/2024/泉州市承天禅寺/art.json
+-rw-r--r--   0        0        0     1133 2024-03-25 03:52:07.749983 arts-2024.4.3.2/arts/life/2024/泉州市承天禅寺/index.html
+-rw-r--r--   0        0        0    11276 2024-02-22 12:02:36.224046 arts-2024.4.3.2/arts/miumapp/LICENSE
+-rw-r--r--   0        0        0     5762 2024-03-31 09:40:29.228723 arts-2024.4.3.2/arts/miumapp/README.md
+-rw-r--r--   0        0        0       36 2024-02-12 15:08:38.569224 arts-2024.4.3.2/arts/miumapp/__init__.py
+-rw-r--r--   0        0        0     7747 2024-03-25 04:09:08.267200 arts-2024.4.3.2/arts/miumapp/_core.py
+-rw-r--r--   0        0        0      111 2024-03-05 23:26:53.659150 arts-2024.4.3.2/arts/miumapp/art.json
+-rw-r--r--   0        0        0      245 2023-09-04 06:15:02.000000 arts-2024.4.3.2/arts/miumapp/licenses/README.md
+-rw-r--r--   0        0        0     1166 2023-12-10 08:00:44.000000 arts-2024.4.3.2/arts/miumapp/licenses/pyppeteer/LICENSE
+-rw-r--r--   0        0        0    11560 2023-12-10 08:00:44.000000 arts-2024.4.3.2/arts/miumapp/licenses/tornado/LICENSE
+-rw-r--r--   0        0        0       48 2024-02-12 15:15:42.556195 arts-2024.4.3.2/arts/miumapp/miumapp/__init__.py
+-rw-r--r--   0        0        0     4657 2024-02-22 17:30:50.375647 arts-2024.4.3.2/arts/miumapp/miumapp/demo.html
+-rw-r--r--   0        0        0     1241 2024-03-25 04:09:36.827762 arts-2024.4.3.2/arts/miumapp/miumapp/demo.py
+-rw-r--r--   0        0        0      645 2024-03-12 12:18:10.837369 arts-2024.4.3.2/arts/miumapp/pyproject.toml
+-rw-r--r--   0        0        0    11273 2024-03-02 20:20:55.781363 arts-2024.4.3.2/arts/oodb/LICENSE
+-rw-r--r--   0        0        0    22563 2024-03-31 09:40:29.216952 arts-2024.4.3.2/arts/oodb/README.md
+-rw-r--r--   0        0        0       44 2024-03-06 00:36:04.879589 arts-2024.4.3.2/arts/oodb/__init__.py
+-rw-r--r--   0        0        0    19029 2024-03-06 09:46:30.072966 arts-2024.4.3.2/arts/oodb/_core.py
+-rw-r--r--   0        0        0       99 2024-03-06 01:01:05.433633 arts-2024.4.3.2/arts/oodb/art.json
+-rw-r--r--   0        0        0      245 2023-09-04 06:15:02.000000 arts-2024.4.3.2/arts/oodb/licenses/README.md
+-rw-r--r--   0        0        0    11357 2022-11-17 21:35:26.000000 arts-2024.4.3.2/arts/oodb/licenses/pymongo/LICENSE
+-rw-r--r--   0        0        0       53 2024-03-06 00:36:04.879589 arts-2024.4.3.2/arts/oodb/oodb.py
+-rw-r--r--   0        0        0      626 2024-03-06 09:57:01.274330 arts-2024.4.3.2/arts/oodb/pyproject.toml
+-rw-r--r--   0        0        0    11281 2024-03-03 07:09:08.518004 arts-2024.4.3.2/arts/oomongo/LICENSE
+-rw-r--r--   0        0        0    17439 2024-03-31 09:40:29.227707 arts-2024.4.3.2/arts/oomongo/README.md
+-rw-r--r--   0        0        0       49 2024-03-05 08:01:41.054010 arts-2024.4.3.2/arts/oomongo/__init__.py
+-rw-r--r--   0        0        0    27613 2024-03-06 00:34:47.221863 arts-2024.4.3.2/arts/oomongo/_core.py
+-rw-r--r--   0        0        0       92 2024-03-06 00:50:10.273786 arts-2024.4.3.2/arts/oomongo/art.json
+-rw-r--r--   0        0        0      245 2023-09-04 06:15:02.000000 arts-2024.4.3.2/arts/oomongo/licenses/README.md
+-rw-r--r--   0        0        0    11357 2022-10-25 20:46:40.000000 arts-2024.4.3.2/arts/oomongo/licenses/motor/LICENSE
+-rw-r--r--   0        0        0    11357 2022-11-17 21:35:26.000000 arts-2024.4.3.2/arts/oomongo/licenses/pymongo/LICENSE
+-rw-r--r--   0        0        0       61 2024-03-05 08:01:41.059008 arts-2024.4.3.2/arts/oomongo/oomongo.py
+-rw-r--r--   0        0        0      563 2024-03-06 00:09:25.377118 arts-2024.4.3.2/arts/oomongo/pyproject.toml
+-rw-r--r--   0        0        0    11281 2024-03-03 07:10:17.933453 arts-2024.4.3.2/arts/oomysql/LICENSE
+-rw-r--r--   0        0        0    17139 2024-03-31 09:40:29.228723 arts-2024.4.3.2/arts/oomysql/README.md
+-rw-r--r--   0        0        0       45 2024-03-05 08:02:05.322948 arts-2024.4.3.2/arts/oomysql/__init__.py
+-rw-r--r--   0        0        0    35301 2024-03-24 00:57:24.021318 arts-2024.4.3.2/arts/oomysql/_core.py
+-rw-r--r--   0        0        0       90 2024-03-06 00:10:16.490984 arts-2024.4.3.2/arts/oomysql/art.json
+-rw-r--r--   0        0        0      245 2023-09-04 06:15:02.000000 arts-2024.4.3.2/arts/oomysql/licenses/README.md
+-rw-r--r--   0        0        0     1070 2022-05-08 19:03:56.000000 arts-2024.4.3.2/arts/oomysql/licenses/aiomysql/LICENSE
+-rw-r--r--   0        0        0     1070 2013-11-27 14:43:24.000000 arts-2024.4.3.2/arts/oomysql/licenses/pymysql/LICENSE
+-rw-r--r--   0        0        0       57 2024-03-05 08:02:05.335929 arts-2024.4.3.2/arts/oomysql/oomysql.py
+-rw-r--r--   0        0        0      641 2024-03-06 00:09:38.203916 arts-2024.4.3.2/arts/oomysql/pyproject.toml
+-rw-r--r--   0        0        0    11281 2024-02-22 12:02:36.209038 arts-2024.4.3.2/arts/openai2/LICENSE
+-rw-r--r--   0        0        0    13991 2024-04-07 02:46:07.779093 arts-2024.4.3.2/arts/openai2/README.md
+-rw-r--r--   0        0        0      168 2024-04-07 02:56:58.773363 arts-2024.4.3.2/arts/openai2/__init__.py
+-rw-r--r--   0        0        0     9858 2024-04-07 03:08:27.254965 arts-2024.4.3.2/arts/openai2/_core/chat.py
+-rw-r--r--   0        0        0     2285 2024-04-07 02:46:07.785077 arts-2024.4.3.2/arts/openai2/_core/chat_in_cmd.py
+-rw-r--r--   0        0        0     6925 2024-04-07 02:46:07.780076 arts-2024.4.3.2/arts/openai2/_core/group_chat.py
+-rw-r--r--   0        0        0       99 2024-03-05 23:28:04.263728 arts-2024.4.3.2/arts/openai2/art.json
+-rw-r--r--   0        0        0      245 2023-09-04 06:15:02.000000 arts-2024.4.3.2/arts/openai2/licenses/README.md
+-rw-r--r--   0        0        0     1083 2020-12-22 18:45:04.000000 arts-2024.4.3.2/arts/openai2/licenses/openai/LICENSE
+-rw-r--r--   0        0        0      191 2024-04-07 02:57:01.800424 arts-2024.4.3.2/arts/openai2/openai2.py
+-rw-r--r--   0        0        0      805 2024-04-07 03:52:00.773865 arts-2024.4.3.2/arts/openai2/pyproject.toml
+-rw-r--r--   0        0        0      231 2024-02-25 03:34:44.558335 arts-2024.4.3.2/arts/skybox/Copyright
+-rw-r--r--   0        0        0      735 2024-02-25 06:24:00.741491 arts-2024.4.3.2/arts/skybox/README.md
+-rw-r--r--   0        0        0      320 2024-04-03 06:26:06.014092 arts-2024.4.3.2/arts/skybox/pyproject.toml
+-rw-r--r--   0        0        0      231 2024-02-25 03:34:44.558335 arts-2024.4.3.2/arts/skybox/skybox/Copyright
+-rw-r--r--   0        0        0      156 2024-02-25 06:24:00.741491 arts-2024.4.3.2/arts/skybox/skybox/__init__.py
+-rw-r--r--   0        0        0    12359 2024-04-03 06:25:47.716340 arts-2024.4.3.2/arts/skybox/skybox/files_hashes
+-rw-r--r--   0        0        0       44 2023-12-19 10:10:36.391618 arts-2024.4.3.2/arts/thoughts/2022/现代工人的螺丝钉处境/art.json
+-rw-r--r--   0        0        0     1374 2024-01-16 22:36:30.326371 arts-2024.4.3.2/arts/thoughts/2022/现代工人的螺丝钉处境/index.html
+-rw-r--r--   0        0        0       44 2023-12-19 10:11:02.542208 arts-2024.4.3.2/arts/thoughts/2023/ChatGPT动了学阀的蛋糕/art.json
+-rw-r--r--   0        0        0     1346 2024-01-30 04:04:01.359662 arts-2024.4.3.2/arts/thoughts/2023/ChatGPT动了学阀的蛋糕/index.html
+-rw-r--r--   0        0        0       44 2023-12-19 10:11:02.562268 arts-2024.4.3.2/arts/thoughts/2023/专利是个公平的赛道/art.json
+-rw-r--r--   0        0        0     1340 2024-03-27 02:41:37.370555 arts-2024.4.3.2/arts/thoughts/2023/专利是个公平的赛道/index.html
+-rw-r--r--   0        0        0       44 2023-12-19 10:11:02.547209 arts-2024.4.3.2/arts/thoughts/2023/事情的真实性是由度的/art.json
+-rw-r--r--   0        0        0     1001 2024-01-16 22:36:30.329386 arts-2024.4.3.2/arts/thoughts/2023/事情的真实性是由度的/index.html
+-rw-r--r--   0        0        0       44 2023-12-19 10:11:02.556244 arts-2024.4.3.2/arts/thoughts/2023/人无法摆脱兽性/art.json
+-rw-r--r--   0        0        0     1659 2024-01-16 22:36:30.330406 arts-2024.4.3.2/arts/thoughts/2023/人无法摆脱兽性/index.html
+-rw-r--r--   0        0        0       44 2023-12-19 10:11:02.551211 arts-2024.4.3.2/arts/thoughts/2023/什么是极端？/art.json
+-rw-r--r--   0        0        0      884 2024-01-16 22:36:30.330406 arts-2024.4.3.2/arts/thoughts/2023/什么是极端？/index.html
+-rw-r--r--   0        0        0       44 2023-12-19 10:11:02.541243 arts-2024.4.3.2/arts/thoughts/2023/保护好人/art.json
+-rw-r--r--   0        0        0      802 2024-01-16 22:36:30.331373 arts-2024.4.3.2/arts/thoughts/2023/保护好人/index.html
+-rw-r--r--   0        0        0       44 2023-12-19 10:11:02.554209 arts-2024.4.3.2/arts/thoughts/2023/只筛选，不教化/art.json
+-rw-r--r--   0        0        0      853 2024-01-16 22:36:30.331373 arts-2024.4.3.2/arts/thoughts/2023/只筛选，不教化/index.html
+-rw-r--r--   0        0        0       44 2023-12-19 10:11:02.549209 arts-2024.4.3.2/arts/thoughts/2023/喊高考加油是刷存在感/art.json
+-rw-r--r--   0        0        0     1047 2024-01-16 22:36:30.332406 arts-2024.4.3.2/arts/thoughts/2023/喊高考加油是刷存在感/index.html
+-rw-r--r--   0        0        0       44 2023-12-19 10:11:02.552210 arts-2024.4.3.2/arts/thoughts/2023/宣扬出来的宽容是恶的代名词/art.json
+-rw-r--r--   0        0        0     1630 2024-01-16 22:36:30.333372 arts-2024.4.3.2/arts/thoughts/2023/宣扬出来的宽容是恶的代名词/index.html
+-rw-r--r--   0        0        0       44 2023-12-19 10:11:02.553243 arts-2024.4.3.2/arts/thoughts/2023/对ChatGPT将带来的变革感到不知所措/art.json
+-rw-r--r--   0        0        0     2475 2024-01-30 04:03:34.796607 arts-2024.4.3.2/arts/thoughts/2023/对ChatGPT将带来的变革感到不知所措/index.html
+-rw-r--r--   0        0        0       44 2023-12-19 10:11:02.561243 arts-2024.4.3.2/arts/thoughts/2023/强人工智能真的出现了，那就是 ChatGPT-4/art.json
+-rw-r--r--   0        0        0      833 2024-01-18 01:51:26.994040 arts-2024.4.3.2/arts/thoughts/2023/强人工智能真的出现了，那就是 ChatGPT-4/index.html
+-rw-r--r--   0        0        0       44 2023-12-19 10:11:02.545246 arts-2024.4.3.2/arts/thoughts/2023/想去国外了解自己/art.json
+-rw-r--r--   0        0        0      966 2024-01-16 22:36:30.335371 arts-2024.4.3.2/arts/thoughts/2023/想去国外了解自己/index.html
+-rw-r--r--   0        0        0       44 2023-12-19 10:11:02.548245 arts-2024.4.3.2/arts/thoughts/2023/现代化的分工合作机制/art.json
+-rw-r--r--   0        0        0     1668 2024-01-16 22:36:30.335371 arts-2024.4.3.2/arts/thoughts/2023/现代化的分工合作机制/index.html
+-rw-r--r--   0        0        0       44 2023-12-19 10:11:02.544210 arts-2024.4.3.2/arts/thoughts/2023/用理性处理简单的事情/art.json
+-rw-r--r--   0        0        0     1587 2024-01-16 22:36:30.336371 arts-2024.4.3.2/arts/thoughts/2023/用理性处理简单的事情/index.html
+-rw-r--r--   0        0        0       44 2023-12-19 10:11:02.557226 arts-2024.4.3.2/arts/thoughts/2023/真正的问题无法通过花招解决/art.json
+-rw-r--r--   0        0        0      977 2024-01-16 22:36:30.336371 arts-2024.4.3.2/arts/thoughts/2023/真正的问题无法通过花招解决/index.html
+-rw-r--r--   0        0        0       44 2023-12-19 10:11:02.560208 arts-2024.4.3.2/arts/thoughts/2023/艺术本天成，媒介偶显之/art.json
+-rw-r--r--   0        0        0      629 2024-01-16 22:36:30.337410 arts-2024.4.3.2/arts/thoughts/2023/艺术本天成，媒介偶显之/index.html
+-rw-r--r--   0        0        0       44 2023-12-19 10:11:02.558244 arts-2024.4.3.2/arts/thoughts/2023/阳光下的美好是以阴影中的丑陋为代价/art.json
+-rw-r--r--   0        0        0     1168 2024-01-16 22:36:30.338372 arts-2024.4.3.2/arts/thoughts/2023/阳光下的美好是以阴影中的丑陋为代价/index.html
+-rw-r--r--   0        0        0       44 2024-01-13 21:13:40.122707 arts-2024.4.3.2/arts/thoughts/2024/不要害怕犯错/art.json
+-rw-r--r--   0        0        0      698 2024-01-16 22:36:30.339373 arts-2024.4.3.2/arts/thoughts/2024/不要害怕犯错/index.html
+-rw-r--r--   0        0        0       44 2024-01-01 14:23:12.130009 arts-2024.4.3.2/arts/thoughts/2024/新年题诗/art.json
+-rw-r--r--   0        0        0     1152 2024-01-18 06:19:08.705581 arts-2024.4.3.2/arts/thoughts/2024/新年题诗/index.html
+-rw-r--r--   0        0        0       44 2024-01-03 04:10:15.709103 arts-2024.4.3.2/arts/thoughts/2024/比特币无法成为取缔实体货币的最终币种/art.json
+-rw-r--r--   0        0        0     1270 2024-01-16 22:36:30.341372 arts-2024.4.3.2/arts/thoughts/2024/比特币无法成为取缔实体货币的最终币种/index.html
+-rw-r--r--   0        0        0       44 2024-03-24 15:35:39.622105 arts-2024.4.3.2/arts/thoughts/2024/编程语言的进化/art.json
+-rw-r--r--   0        0        0     1022 2024-03-24 16:22:12.389078 arts-2024.4.3.2/arts/thoughts/2024/编程语言的进化/example.html
+-rw-r--r--   0        0        0     1520 2024-03-25 03:53:51.266590 arts-2024.4.3.2/arts/thoughts/2024/编程语言的进化/index.html
+-rw-r--r--   0        0        0       44 2024-01-30 04:08:51.850343 arts-2024.4.3.2/arts/thoughts/2024/萝莉岛事件引发的信任危机/art.json
+-rw-r--r--   0        0        0     1077 2024-01-30 04:15:45.681734 arts-2024.4.3.2/arts/thoughts/2024/萝莉岛事件引发的信任危机/index.html
+-rw-r--r--   0        0        0       44 2024-01-18 06:20:18.873404 arts-2024.4.3.2/arts/thoughts/2024/霍金去萝莉岛干嘛了/art.json
+-rw-r--r--   0        0        0     1174 2024-01-18 06:24:05.339876 arts-2024.4.3.2/arts/thoughts/2024/霍金去萝莉岛干嘛了/index.html
+-rw-r--r--   0        0        0      103 2024-03-03 07:12:46.987154 arts-2024.4.3.2/arts/tutorials/150-操作MySQL/art.json
+-rw-r--r--   0        0        0      103 2024-03-06 00:50:30.486267 arts-2024.4.3.2/arts/tutorials/225-操作MongoDB/art.json
+-rw-r--r--   0        0        0      146 2024-02-25 14:11:14.480558 arts-2024.4.3.2/arts/tutorials/300-开发桌面GUI应用/art.json
+-rw-r--r--   0        0        0      103 2024-02-18 14:43:25.042841 arts-2024.4.3.2/arts/tutorials/450-对接ChatGPT/art.json
+-rw-r--r--   0        0        0      122 2024-03-22 15:10:08.573597 arts-2024.4.3.2/arts/tutorials/525-时间模块/art.json
+-rw-r--r--   0        0        0      100 2024-03-06 01:01:25.689741 arts-2024.4.3.2/arts/tutorials/562-面向对象数据库/art.json
+-rw-r--r--   0        0        0     3415 2023-12-20 10:09:07.822297 arts-2024.4.3.2/arts/tutorials/600-用37行代码实现AI五子棋/README.md
+-rw-r--r--   0        0        0       44 2023-12-19 10:14:03.255370 arts-2024.4.3.2/arts/tutorials/600-用37行代码实现AI五子棋/art.json
+-rw-r--r--   0        0        0     8070 2024-02-25 05:45:21.624081 arts-2024.4.3.2/arts/tutorials/750-正则表达式/README.md
+-rw-r--r--   0        0        0       44 2023-12-19 10:13:55.412792 arts-2024.4.3.2/arts/tutorials/750-正则表达式/art.json
+-rw-r--r--   0        0        0       44 2024-01-30 03:46:52.790397 arts-2024.4.3.2/arts/videos/200-秦时明月[项羽]·谪居/art.json
+-rw-r--r--   0        0        0       44 2023-12-19 10:07:05.944886 arts-2024.4.3.2/arts/videos/400-李连杰[霍元甲]·兰亭序/art.json
+-rw-r--r--   0        0        0       44 2023-12-19 10:07:05.933448 arts-2024.4.3.2/arts/videos/600-楚门的世界·五月雨/art.json
+-rw-r--r--   0        0        0       44 2024-01-05 13:31:13.729378 arts-2024.4.3.2/arts/videos/800-AI是这样画包拯的/art.json
+-rw-r--r--   0        0        0      526 2024-04-07 03:51:45.520838 arts-2024.4.3.2/pyproject.toml
+-rw-r--r--   0        0        0      530 1970-01-01 00:00:00.000000 arts-2024.4.3.2/PKG-INFO
```

### Comparing `arts-2024.4.3.1/.gitignore` & `arts-2024.4.3.2/.gitignore`

 * *Files identical despite different names*

### Comparing `arts-2024.4.3.1/arts/CoolMemory-English/README.md` & `arts-2024.4.3.2/arts/CoolMemory-English/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.3.1/arts/CoolMemory-English/licenses/licenses/Chromium/LICENSE` & `arts-2024.4.3.2/arts/CoolMemory-English/licenses/licenses/Chromium/LICENSE`

 * *Files identical despite different names*

### Comparing `arts-2024.4.3.1/arts/CoolMemory-English/licenses/licenses/Nuitka/LICENSE` & `arts-2024.4.3.2/arts/CoolMemory-English/licenses/licenses/Nuitka/LICENSE`

 * *Files identical despite different names*

### Comparing `arts-2024.4.3.1/arts/CoolMemory-English/licenses/licenses/Python/LICENSE` & `arts-2024.4.3.2/arts/CoolMemory-English/licenses/licenses/Python/LICENSE`

 * *Files identical despite different names*

### Comparing `arts-2024.4.3.1/arts/CoolMemory-English/licenses/licenses/pycryptodome/LICENSE` & `arts-2024.4.3.2/arts/CoolMemory-English/licenses/licenses/pycryptodome/LICENSE`

 * *Files identical despite different names*

### Comparing `arts-2024.4.3.1/arts/CoolMemory-English/licenses/licenses/pyppeteer/LICENSE` & `arts-2024.4.3.2/arts/CoolMemory-English/licenses/licenses/pyppeteer/LICENSE`

 * *Files identical despite different names*

### Comparing `arts-2024.4.3.1/arts/CoolMemory-English/licenses/licenses/tornado/LICENSE` & `arts-2024.4.3.2/arts/CoolMemory-English/licenses/licenses/tornado/LICENSE`

 * *Files identical despite different names*

### Comparing `arts-2024.4.3.1/arts/WeChat-Art-Museum/index.html` & `arts-2024.4.3.2/arts/WeChat-Art-Museum/index.html`

 * *Files identical despite different names*

### Comparing `arts-2024.4.3.1/arts/articles/010-赚钱宝典/010-财富的本质/README.md` & `arts-2024.4.3.2/arts/articles/010-赚钱宝典/010-财富的本质/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.3.1/arts/articles/010-赚钱宝典/020-商业价值/README.md` & `arts-2024.4.3.2/arts/articles/010-赚钱宝典/020-商业价值/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.3.1/arts/articles/010-赚钱宝典/030-财富稳定型社会/README.md` & `arts-2024.4.3.2/arts/articles/010-赚钱宝典/030-财富稳定型社会/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.3.1/arts/articles/075-追英赶美/300-产业升级与失业潮/README.md` & `arts-2024.4.3.2/arts/articles/075-追英赶美/300-产业升级与失业潮/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.3.1/arts/articles/075-追英赶美/600-在ChatGPT冲击下，打造国家级公共知识库迫在眉睫/README.md` & `arts-2024.4.3.2/arts/articles/075-追英赶美/600-在ChatGPT冲击下，打造国家级公共知识库迫在眉睫/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.3.1/arts/articles/150-小民参政/300-广义的民主/README.md` & `arts-2024.4.3.2/arts/articles/150-小民参政/300-广义的民主/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.3.1/arts/articles/150-小民参政/600-年轻人不结婚是文明的进步/README.md` & `arts-2024.4.3.2/arts/articles/150-小民参政/600-年轻人不结婚是文明的进步/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.3.1/arts/articles/300-批判那些伪文艺/200-一元官司有意义吗？/README.md` & `arts-2024.4.3.2/arts/articles/300-批判那些伪文艺/200-一元官司有意义吗？/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.3.1/arts/articles/300-批判那些伪文艺/400-唯有变化是不变的？/README.md` & `arts-2024.4.3.2/arts/articles/300-批判那些伪文艺/400-唯有变化是不变的？/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.3.1/arts/articles/300-批判那些伪文艺/600-未经他人苦，莫劝他人善？/README.md` & `arts-2024.4.3.2/arts/articles/300-批判那些伪文艺/600-未经他人苦，莫劝他人善？/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.3.1/arts/articles/300-批判那些伪文艺/800-务实与务虚/README.md` & `arts-2024.4.3.2/arts/articles/300-批判那些伪文艺/800-务实与务虚/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.3.1/arts/articles/450-万象思考/050-ChatGPT已经有自我意识了/README.md` & `arts-2024.4.3.2/arts/articles/450-万象思考/050-ChatGPT已经有自我意识了/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.3.1/arts/articles/450-万象思考/100-怎么理解「迷信科学」？/README.md` & `arts-2024.4.3.2/arts/articles/450-万象思考/100-怎么理解「迷信科学」？/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.3.1/arts/articles/450-万象思考/150-心理学中个案研究有意义吗？/README.md` & `arts-2024.4.3.2/arts/articles/450-万象思考/150-心理学中个案研究有意义吗？/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.3.1/arts/articles/450-万象思考/200-人工智能会不会统治人类？/README.md` & `arts-2024.4.3.2/arts/articles/450-万象思考/200-人工智能会不会统治人类？/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.3.1/arts/articles/450-万象思考/250-忒修斯之船悖论/README.md` & `arts-2024.4.3.2/arts/articles/450-万象思考/250-忒修斯之船悖论/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.3.1/arts/articles/450-万象思考/300-有无相生，难易相成的启发/README.md` & `arts-2024.4.3.2/arts/articles/450-万象思考/300-有无相生，难易相成的启发/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.3.1/arts/articles/450-万象思考/400-熵增都是坏的，熵减都是好的吗？/README.md` & `arts-2024.4.3.2/arts/articles/450-万象思考/400-熵增都是坏的，熵减都是好的吗？/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.3.1/arts/articles/450-万象思考/500-人们为什么希望拥有后代/README.md` & `arts-2024.4.3.2/arts/articles/450-万象思考/500-人们为什么希望拥有后代/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.3.1/arts/articles/450-万象思考/600-万物为什么会遵循着物理定律？/README.md` & `arts-2024.4.3.2/arts/articles/450-万象思考/600-万物为什么会遵循着物理定律？/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.3.1/arts/articles/450-万象思考/700-堕胎自由权/README.md` & `arts-2024.4.3.2/arts/articles/450-万象思考/700-堕胎自由权/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.3.1/arts/articles/450-万象思考/800-人人平等是个伪概念/README.md` & `arts-2024.4.3.2/arts/articles/450-万象思考/800-人人平等是个伪概念/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.3.1/arts/articles/600-时空猜想/200-轮回转世真的存在吗？/README.md` & `arts-2024.4.3.2/arts/articles/600-时空猜想/200-轮回转世真的存在吗？/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.3.1/arts/articles/600-时空猜想/400-我们可能处在人造世界/README.md` & `arts-2024.4.3.2/arts/articles/600-时空猜想/400-我们可能处在人造世界/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.3.1/arts/articles/600-时空猜想/600-占卜真的存在吗？/README.md` & `arts-2024.4.3.2/arts/articles/600-时空猜想/600-占卜真的存在吗？/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.3.1/arts/articles/600-时空猜想/800-“自由意志”其实是“随机意志”/README.md` & `arts-2024.4.3.2/arts/articles/600-时空猜想/800-“自由意志”其实是“随机意志”/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.3.1/arts/articles/700-论时事/300-那些年，我们经历过的历史/README.md` & `arts-2024.4.3.2/arts/articles/700-论时事/300-那些年，我们经历过的历史/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.3.1/arts/articles/700-论时事/600-评价在北京工体冲进场的梅西粉丝/README.md` & `arts-2024.4.3.2/arts/articles/700-论时事/600-评价在北京工体冲进场的梅西粉丝/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.3.1/arts/articles/800-小说/300-陆小凤新传/050-燕山宝藏 第1章/README.md` & `arts-2024.4.3.2/arts/articles/800-小说/300-陆小凤新传/050-燕山宝藏 第1章/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.3.1/arts/articles/800-小说/600-一念天堂/050-被绑架/README.md` & `arts-2024.4.3.2/arts/articles/800-小说/600-一念天堂/050-被绑架/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.3.1/arts/cooltypes/LICENSE` & `arts-2024.4.3.2/arts/cooltypes/LICENSE`

 * *Files identical despite different names*

### Comparing `arts-2024.4.3.1/arts/cooltypes/envname/README.md` & `arts-2024.4.3.2/arts/cooltypes/envname/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.3.1/arts/cooltypes/moduledb/README.md` & `arts-2024.4.3.2/arts/cooltypes/moduledb/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.3.1/arts/cooltypes/moduledb/_core.py` & `arts-2024.4.3.2/arts/cooltypes/moduledb/_core.py`

 * *Files identical despite different names*

### Comparing `arts-2024.4.3.1/arts/cooltypes/modules/coolstr/_core.py` & `arts-2024.4.3.2/arts/cooltypes/modules/coolstr/_core.py`

 * *Files identical despite different names*

### Comparing `arts-2024.4.3.1/arts/cooltypes/modules/cooltime/README.md` & `arts-2024.4.3.2/arts/cooltypes/modules/cooltime/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.3.1/arts/cooltypes/modules/cooltime/_core.py` & `arts-2024.4.3.2/arts/cooltypes/modules/cooltime/_core.py`

 * *Files identical despite different names*

### Comparing `arts-2024.4.3.1/arts/cooltypes/modules/rslice/README.md` & `arts-2024.4.3.2/arts/cooltypes/modules/rslice/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.3.1/arts/cooltypes/modules/rslice/_core.py` & `arts-2024.4.3.2/arts/cooltypes/modules/rslice/_core.py`

 * *Files identical despite different names*

### Comparing `arts-2024.4.3.1/arts/cooltypes/modules/vtype/_core.py` & `arts-2024.4.3.2/arts/cooltypes/modules/vtype/_core.py`

 * *Files identical despite different names*

### Comparing `arts-2024.4.3.1/arts/index.html` & `arts-2024.4.3.2/arts/index.html`

 * *Files identical despite different names*

### Comparing `arts-2024.4.3.1/arts/life/2018/莆田学院·毕业生留影/index.html` & `arts-2024.4.3.2/arts/life/2018/莆田学院·毕业生留影/index.html`

 * *Files identical despite different names*

### Comparing `arts-2024.4.3.1/arts/life/2019/苏州市虎丘山/index.html` & `arts-2024.4.3.2/arts/life/2019/苏州市虎丘山/index.html`

 * *Files identical despite different names*

### Comparing `arts-2024.4.3.1/arts/life/2022/泉州市丰泽区·雨后街道/index.html` & `arts-2024.4.3.2/arts/life/2022/泉州市丰泽区·雨后街道/index.html`

 * *Files identical despite different names*

### Comparing `arts-2024.4.3.1/arts/life/2023/更换微信账号了/index.html` & `arts-2024.4.3.2/arts/life/2023/更换微信账号了/index.html`

 * *Files identical despite different names*

### Comparing `arts-2024.4.3.1/arts/life/2024/泉州市承天禅寺/index.html` & `arts-2024.4.3.2/arts/life/2024/泉州市承天禅寺/index.html`

 * *Files identical despite different names*

### Comparing `arts-2024.4.3.1/arts/miumapp/LICENSE` & `arts-2024.4.3.2/arts/miumapp/LICENSE`

 * *Files identical despite different names*

### Comparing `arts-2024.4.3.1/arts/miumapp/README.md` & `arts-2024.4.3.2/arts/miumapp/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.3.1/arts/miumapp/_core.py` & `arts-2024.4.3.2/arts/miumapp/_core.py`

 * *Files identical despite different names*

### Comparing `arts-2024.4.3.1/arts/miumapp/licenses/pyppeteer/LICENSE` & `arts-2024.4.3.2/arts/miumapp/licenses/pyppeteer/LICENSE`

 * *Files identical despite different names*

### Comparing `arts-2024.4.3.1/arts/miumapp/licenses/tornado/LICENSE` & `arts-2024.4.3.2/arts/miumapp/licenses/tornado/LICENSE`

 * *Files identical despite different names*

### Comparing `arts-2024.4.3.1/arts/miumapp/miumapp/demo.html` & `arts-2024.4.3.2/arts/miumapp/miumapp/demo.html`

 * *Files identical despite different names*

### Comparing `arts-2024.4.3.1/arts/miumapp/miumapp/demo.py` & `arts-2024.4.3.2/arts/miumapp/miumapp/demo.py`

 * *Files identical despite different names*

### Comparing `arts-2024.4.3.1/arts/miumapp/pyproject.toml` & `arts-2024.4.3.2/arts/miumapp/pyproject.toml`

 * *Files identical despite different names*

### Comparing `arts-2024.4.3.1/arts/oodb/LICENSE` & `arts-2024.4.3.2/arts/oodb/LICENSE`

 * *Files identical despite different names*

### Comparing `arts-2024.4.3.1/arts/oodb/README.md` & `arts-2024.4.3.2/arts/oodb/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.3.1/arts/oodb/_core.py` & `arts-2024.4.3.2/arts/oodb/_core.py`

 * *Files identical despite different names*

### Comparing `arts-2024.4.3.1/arts/oodb/licenses/pymongo/LICENSE` & `arts-2024.4.3.2/arts/oodb/licenses/pymongo/LICENSE`

 * *Files identical despite different names*

### Comparing `arts-2024.4.3.1/arts/oodb/pyproject.toml` & `arts-2024.4.3.2/arts/oodb/pyproject.toml`

 * *Files identical despite different names*

### Comparing `arts-2024.4.3.1/arts/oomongo/LICENSE` & `arts-2024.4.3.2/arts/oomongo/LICENSE`

 * *Files identical despite different names*

### Comparing `arts-2024.4.3.1/arts/oomongo/README.md` & `arts-2024.4.3.2/arts/oomongo/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.3.1/arts/oomongo/_core.py` & `arts-2024.4.3.2/arts/oomongo/_core.py`

 * *Files identical despite different names*

### Comparing `arts-2024.4.3.1/arts/oomongo/licenses/motor/LICENSE` & `arts-2024.4.3.2/arts/oomongo/licenses/motor/LICENSE`

 * *Files identical despite different names*

### Comparing `arts-2024.4.3.1/arts/oomongo/licenses/pymongo/LICENSE` & `arts-2024.4.3.2/arts/oomongo/licenses/pymongo/LICENSE`

 * *Files identical despite different names*

### Comparing `arts-2024.4.3.1/arts/oomongo/pyproject.toml` & `arts-2024.4.3.2/arts/oomongo/pyproject.toml`

 * *Files identical despite different names*

### Comparing `arts-2024.4.3.1/arts/oomysql/LICENSE` & `arts-2024.4.3.2/arts/oomysql/LICENSE`

 * *Files identical despite different names*

### Comparing `arts-2024.4.3.1/arts/oomysql/README.md` & `arts-2024.4.3.2/arts/oomysql/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.3.1/arts/oomysql/_core.py` & `arts-2024.4.3.2/arts/oomysql/_core.py`

 * *Files identical despite different names*

### Comparing `arts-2024.4.3.1/arts/oomysql/licenses/aiomysql/LICENSE` & `arts-2024.4.3.2/arts/oomysql/licenses/aiomysql/LICENSE`

 * *Files identical despite different names*

### Comparing `arts-2024.4.3.1/arts/oomysql/licenses/pymysql/LICENSE` & `arts-2024.4.3.2/arts/oomysql/licenses/pymysql/LICENSE`

 * *Files identical despite different names*

### Comparing `arts-2024.4.3.1/arts/oomysql/pyproject.toml` & `arts-2024.4.3.2/arts/oomysql/pyproject.toml`

 * *Files identical despite different names*

### Comparing `arts-2024.4.3.1/arts/openai2/LICENSE` & `arts-2024.4.3.2/arts/openai2/LICENSE`

 * *Files identical despite different names*

### Comparing `arts-2024.4.3.1/arts/openai2/README.md` & `arts-2024.4.3.2/arts/openai2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -283,20 +283,20 @@
 ]
 ```
 
 ## 限制历史消息数量
 
 ### 限制历史消息数量
 
-随着对话次数越来越多，最终上下文长度就会超出 openai 接口限定的最大 token 数量，此时可使用 MsgMaxCount 参数来限制历史消息数量。当消息数量超出 MsgMaxCount 后，程序会自动移除最早的记录，使消息数量减少到恰好等于 MsgMaxCount 。
+随着对话次数越来越多，最终上下文长度就会超出 openai 接口限定的最大 token 数量，此时可使用 msg_max_count 参数来限制历史消息数量。当消息数量超出 msg_max_count 后，程序会自动移除最早的记录，使消息数量减少到恰好等于 msg_max_count 。
 
 ```python
-MsgMaxCount = 6  # 最多保留6条历史消息
+msg_max_count = 6  # 最多保留6条历史消息
 
-Ariel = Chat(api_key=api_key, model="gpt-3.5-turbo", MsgMaxCount=MsgMaxCount)
+Ariel = Chat(api_key=api_key, model="gpt-3.5-turbo", msg_max_count=msg_max_count)
 
 Ariel.request('英国的首都是什么？')  # >>> '伦敦'
 Ariel.request('日本首都是什么？')  # >>> '东京'
 Ariel.request('意大利的首都是什么？')  # >>> '罗马'
 Ariel.request('美国的首都是什么？')  # >>> '华盛顿'
 Ariel.request('世界上国土面积最大的国家是哪个？')  # >>> '俄罗斯'
 Ariel.request('法国的首都叫什么？')  # >>> '巴黎'
@@ -317,17 +317,17 @@
 ```
 
 ### 锁定消息
 
 当程序自动移除消息记录时，也许我们希望某些消息不要被移除，此时可将这些消息锁定。
 
 ```python
-MsgMaxCount = 6
+msg_max_count = 6
 
-Ariel = Chat(api_key=api_key, model="gpt-3.5-turbo", MsgMaxCount=MsgMaxCount)
+Ariel = Chat(api_key=api_key, model="gpt-3.5-turbo", msg_max_count=msg_max_count)
 
 Ariel.request('英国的首都是什么？')  # >>> '伦敦'
 Ariel.request('日本首都是什么？')  # >>> '东京'
 Ariel.request('意大利的首都是什么？')  # >>> '罗马'
 ```
 
 此时共有 6 条消息记录：
@@ -349,15 +349,15 @@
 
 继续请求：
 
 ```python
 Ariel.request('美国的首都是什么？')  # >>> '华盛顿'
 ```
 
-由于设置了 MsgMaxCount = 6，此时共有 6 条消息记录：
+由于设置了 msg_max_count = 6，此时共有 6 条消息记录：
 
 | 消息                 | 正序索引 | 逆序索引 | 锁定状态 |
 | -------------------- | :------: | :------: | :------: |
 | 英国的首都是什么？   |    0    |    -6    |  已锁定  |
 | 东京                 |    1    |    -5    |    -    |
 | 意大利的首都是什么？ |    2    |    -4    |  已锁定  |
 | 罗马                 |    3    |    -3    |  已锁定  |
```

### Comparing `arts-2024.4.3.1/arts/openai2/_core/GroupChat.py` & `arts-2024.4.3.2/arts/openai2/_core/group_chat.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
                     timeout=None,
                     max_retries=None,
                     http_client=None,
                     # request_kwargs
                     model: Literal["gpt-4-1106-preview", "gpt-4-vision-preview", "gpt-4", "gpt-4-0314", "gpt-4-0613",
                                     "gpt-4-32k", "gpt-4-32k-0314", "gpt-4-32k-0613", "gpt-3.5-turbo"] = "gpt-3.5-turbo",
                     # Chat
-                    MsgMaxCount=None,
+                    msg_max_count=None,
                     # kwargs
                     **kwargs,
                     ):
             ...
     
     def add_dialog(self, speaker:str, audiences:list, remark:str):
         '''
```

### Comparing `arts-2024.4.3.1/arts/openai2/_core/chat.py` & `arts-2024.4.3.2/arts/openai2/_core/chat.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from json import dumps as jsonDumps
 from json import loads as jsonLoads
 from pathlib import Path
-from typing import Union, List, Literal
+from typing import List, Literal
 from openai import OpenAI, AsyncOpenAI
 
 
 class AKPool:
     """ 轮询获取api_key """
 
     def __init__(self, apikeys: list):
@@ -80,17 +80,17 @@
 
     def copy(self):
         que = self.__class__(maxlen=self.maxlen)
         que.core = self.core.copy()
         return que
 
     def deepcopy(self):
-        ...  # 创建这个方法是为了提醒用户: copy 方法是浅拷贝
+        ...  # 创建这个方法是为了以代码提示的方式提醒用户: copy 方法是浅拷贝
 
-    def __add__(self, obj: Union[list, "Temque"]):
+    def __add__(self, obj: 'list|Temque'):
         que = self.copy()
         if isinstance(obj, self.__class__):
             que.core += obj.core
             que._trim()
         else:
             que.add_many(*obj)
         return que
@@ -105,40 +105,43 @@
     * [获取链接2](https://www.baidu.com/s?wd=%E8%8E%B7%E5%8F%96%20openai%20api_key)
     """
     
     recently_request_data: dict  # 最近一次请求所用的参数
 
     def __init__(self,
                  # kwargs
-                 api_key: Union[str, AKPool],
+                 api_key: str|AKPool,
                  base_url: str = None,  # base_url 参数用于修改基础URL
                  timeout=None,
                  max_retries=None,
                  http_client=None,
                  # request_kwargs
                  model: Literal["gpt-4-1106-preview", "gpt-4-vision-preview", "gpt-4", "gpt-4-0314", "gpt-4-0613",
                                 "gpt-4-32k", "gpt-4-32k-0314", "gpt-4-32k-0613", "gpt-3.5-turbo"] = "gpt-3.5-turbo",
                  # Chat
-                 MsgMaxCount=None,
+                 msg_max_count: int=None,
                  # kwargs
                  **kwargs,
                  ):
         api_base = kwargs.pop('api_base', None)
+        base_url = base_url or api_base
+        MsgMaxCount = kwargs.pop('MsgMaxCount', None)
+        msg_max_count = msg_max_count or MsgMaxCount
 
-        if base_url or api_base: kwargs["base_url"] = base_url or api_base
+        if base_url: kwargs["base_url"] = base_url
         if timeout: kwargs["timeout"] = timeout
         if max_retries: kwargs["max_retries"] = max_retries
         if http_client: kwargs["http_client"] = http_client
 
         self.reset_api_key(api_key)
         self._kwargs = kwargs
         self._request_kwargs = {'model':model}
-        self._messages = Temque(maxlen=MsgMaxCount)
+        self._messages = Temque(maxlen=msg_max_count)
     
-    def reset_api_key(self, api_key: Union[str, AKPool]):
+    def reset_api_key(self, api_key: str|AKPool):
         if isinstance(api_key, AKPool):
             self._akpool = api_key
         else:
             self._akpool = AKPool([api_key])
 
     def request(self, text: str=None, **kwargs):
         messages = [{"role": "user", "content": text}]
@@ -211,47 +214,64 @@
         async for chunk in completion:
             if chunk.choices and (content := chunk.choices[0].delta.content):
                 answer += content
                 yield content
         self._messages.add_many(*messages, {"role": "assistant", "content": answer})
 
     def rollback(self, n=1):
+        '''
+        回滚对话
+        '''
         self._messages.core[-2 * n :] = []
         for x in self._messages.core[-2:]:
             x = x["obj"]
             print(f"[{x['role']}]:{x['content']}")
 
     def pin_messages(self, *indexes):
+        '''
+        锁定历史消息
+        '''
         self._messages.pin(*indexes)
 
     def unpin_messages(self, *indexes):
+        '''
+        解锁历史消息
+        '''
         self._messages.unpin(*indexes)
     
     def fetch_messages(self):
         return list(self._messages)
     
-    def add_dialogs(self, *ms: Union[system_msg, user_msg, assistant_msg, dict]):
+    def add_dialogs(self, *ms: dict|system_msg|user_msg|assistant_msg):
         '''
         添加历史对话
         '''
         messages = [dict(x) for x in ms]
         self._messages.add_many(*messages)
-    
-    asy_request = async_request  # 兼容旧代码
-
-    forge = add_dialogs  # 兼容旧代码
+        
+    def __getattr__(self, name):
+        match name:  # 兼容旧代码
+            case 'asy_request':
+                return self.async_request
+            case 'forge':
+                return self.add_dialogs
+            case 'pin':
+                return self.pin_messages
+            case 'unpin':
+                return self.unpin_messages
+            case 'dump':
+                return self._dump
+            case 'load':
+                return self._load
+        raise AttributeError(name)
 
-    pin = pin_messages  # 兼容旧代码
-
-    unpin = unpin_messages  # 兼容旧代码
-    
-    def dump(self, fpath: str):  # 兼容旧代码
+    def _dump(self, fpath: str):
         """ 存档 """
         jt = jsonDumps(self.fetch_messages(), ensure_ascii=False)
         Path(fpath).write_text(jt, encoding="utf8")
         return True
     
-    def load(self, fpath: str):  # 兼容旧代码
+    def _load(self, fpath: str):
         """ 载入存档 """
         jt = Path(fpath).read_text(encoding="utf8")
         self._messages.add_many(*jsonLoads(jt))
         return True
```

### Comparing `arts-2024.4.3.1/arts/openai2/_core/chat_in_cmd.py` & `arts-2024.4.3.2/arts/openai2/_core/chat_in_cmd.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 mdb = moduledb.DB(openai2, depth=3)['chat_in_cmd']
 apikeys: moduledb.File = mdb['apikeys']['data_1']
 apikeys.setdefault('list', [])
 record: moduledb.File = mdb['records']['chat_1']
 record.setdefault('messages', [])
 
 
-def chat_in_cmd(apikeys:list, newchat=False, model='gpt-4-1106-preview', MsgMaxCount=30):
+def chat_in_cmd(apikeys:list, newchat=False, model='gpt-4-1106-preview', msg_max_count=30):
     print(f"\n\033[0m您已进入命令行聊天模式, 当前使用'{model}'模型, 请确保您的apikey支持该模型.", end='')
-    gpt = Chat(api_key=AKPool(apikeys), model=model, MsgMaxCount=MsgMaxCount)
+    gpt = Chat(api_key=AKPool(apikeys), model=model, msg_max_count=msg_max_count)
     if not newchat:
         gpt.add_dialogs(*record['messages'])
     while True:
         user = input('\n\n\033[32;1m:')
         print('\033[0m')
         for x in gpt.stream_request(user):
             print(x, end='', flush=True)
```

### Comparing `arts-2024.4.3.1/arts/openai2/licenses/openai/LICENSE` & `arts-2024.4.3.2/arts/openai2/licenses/openai/LICENSE`

 * *Files identical despite different names*

### Comparing `arts-2024.4.3.1/arts/openai2/pyproject.toml` & `arts-2024.4.3.2/arts/openai2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "openai2"
-version = "1.7.1"
+version = "1.7.2"
 description = "ChatGPT 工具包，支持连续对话、流式对话（逐字显示）、对话存档与载入、对话回滚、对话伪造、轮询 api_key 池、群聊多角色模拟、在命令行对话、限制历史消息数量、异步请求。"
-dependencies = ["arts>=2024.4.3.1"]
+dependencies = ["arts>=2024.4.3.2"]
 keywords = ["openai", "chatgpt", "openai2"]
 
 
 readme = "README.md"
 authors = [{name = "江南雨上", email = "lcctoor@outlook.com"}]
 license = {file = "LICENSE"}
 classifiers = ["License :: OSI Approved :: Apache Software License"]
```

### Comparing `arts-2024.4.3.1/arts/skybox/README.md` & `arts-2024.4.3.2/arts/skybox/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.3.1/arts/skybox/skybox/files_hashes` & `arts-2024.4.3.2/arts/skybox/skybox/files_hashes`

 * *Files identical despite different names*

### Comparing `arts-2024.4.3.1/arts/thoughts/2022/现代工人的螺丝钉处境/index.html` & `arts-2024.4.3.2/arts/thoughts/2022/现代工人的螺丝钉处境/index.html`

 * *Files identical despite different names*

### Comparing `arts-2024.4.3.1/arts/thoughts/2023/ChatGPT动了学阀的蛋糕/index.html` & `arts-2024.4.3.2/arts/thoughts/2023/ChatGPT动了学阀的蛋糕/index.html`

 * *Files identical despite different names*

### Comparing `arts-2024.4.3.1/arts/thoughts/2023/专利是个公平的赛道/index.html` & `arts-2024.4.3.2/arts/thoughts/2023/专利是个公平的赛道/index.html`

 * *Files identical despite different names*

### Comparing `arts-2024.4.3.1/arts/thoughts/2023/事情的真实性是由度的/index.html` & `arts-2024.4.3.2/arts/thoughts/2023/事情的真实性是由度的/index.html`

 * *Files identical despite different names*

### Comparing `arts-2024.4.3.1/arts/thoughts/2023/人无法摆脱兽性/index.html` & `arts-2024.4.3.2/arts/thoughts/2023/人无法摆脱兽性/index.html`

 * *Files identical despite different names*

### Comparing `arts-2024.4.3.1/arts/thoughts/2023/什么是极端？/index.html` & `arts-2024.4.3.2/arts/thoughts/2023/什么是极端？/index.html`

 * *Files identical despite different names*

### Comparing `arts-2024.4.3.1/arts/thoughts/2023/保护好人/index.html` & `arts-2024.4.3.2/arts/thoughts/2023/保护好人/index.html`

 * *Files identical despite different names*

### Comparing `arts-2024.4.3.1/arts/thoughts/2023/只筛选，不教化/index.html` & `arts-2024.4.3.2/arts/thoughts/2023/只筛选，不教化/index.html`

 * *Files identical despite different names*

### Comparing `arts-2024.4.3.1/arts/thoughts/2023/喊高考加油是刷存在感/index.html` & `arts-2024.4.3.2/arts/thoughts/2023/喊高考加油是刷存在感/index.html`

 * *Files identical despite different names*

### Comparing `arts-2024.4.3.1/arts/thoughts/2023/宣扬出来的宽容是恶的代名词/index.html` & `arts-2024.4.3.2/arts/thoughts/2023/宣扬出来的宽容是恶的代名词/index.html`

 * *Files identical despite different names*

### Comparing `arts-2024.4.3.1/arts/thoughts/2023/对ChatGPT将带来的变革感到不知所措/index.html` & `arts-2024.4.3.2/arts/thoughts/2023/对ChatGPT将带来的变革感到不知所措/index.html`

 * *Files identical despite different names*

### Comparing `arts-2024.4.3.1/arts/thoughts/2023/强人工智能真的出现了，那就是 ChatGPT-4/index.html` & `arts-2024.4.3.2/arts/thoughts/2023/强人工智能真的出现了，那就是 ChatGPT-4/index.html`

 * *Files identical despite different names*

### Comparing `arts-2024.4.3.1/arts/thoughts/2023/想去国外了解自己/index.html` & `arts-2024.4.3.2/arts/thoughts/2023/想去国外了解自己/index.html`

 * *Files identical despite different names*

### Comparing `arts-2024.4.3.1/arts/thoughts/2023/现代化的分工合作机制/index.html` & `arts-2024.4.3.2/arts/thoughts/2023/现代化的分工合作机制/index.html`

 * *Files identical despite different names*

### Comparing `arts-2024.4.3.1/arts/thoughts/2023/用理性处理简单的事情/index.html` & `arts-2024.4.3.2/arts/thoughts/2023/用理性处理简单的事情/index.html`

 * *Files identical despite different names*

### Comparing `arts-2024.4.3.1/arts/thoughts/2023/真正的问题无法通过花招解决/index.html` & `arts-2024.4.3.2/arts/thoughts/2023/真正的问题无法通过花招解决/index.html`

 * *Files identical despite different names*

### Comparing `arts-2024.4.3.1/arts/thoughts/2023/艺术本天成，媒介偶显之/index.html` & `arts-2024.4.3.2/arts/thoughts/2023/艺术本天成，媒介偶显之/index.html`

 * *Files identical despite different names*

### Comparing `arts-2024.4.3.1/arts/thoughts/2023/阳光下的美好是以阴影中的丑陋为代价/index.html` & `arts-2024.4.3.2/arts/thoughts/2023/阳光下的美好是以阴影中的丑陋为代价/index.html`

 * *Files identical despite different names*

### Comparing `arts-2024.4.3.1/arts/thoughts/2024/不要害怕犯错/index.html` & `arts-2024.4.3.2/arts/thoughts/2024/不要害怕犯错/index.html`

 * *Files identical despite different names*

### Comparing `arts-2024.4.3.1/arts/thoughts/2024/新年题诗/index.html` & `arts-2024.4.3.2/arts/thoughts/2024/新年题诗/index.html`

 * *Files identical despite different names*

### Comparing `arts-2024.4.3.1/arts/thoughts/2024/比特币无法成为取缔实体货币的最终币种/index.html` & `arts-2024.4.3.2/arts/thoughts/2024/比特币无法成为取缔实体货币的最终币种/index.html`

 * *Files identical despite different names*

### Comparing `arts-2024.4.3.1/arts/thoughts/2024/编程语言的进化/example.html` & `arts-2024.4.3.2/arts/thoughts/2024/编程语言的进化/example.html`

 * *Files identical despite different names*

### Comparing `arts-2024.4.3.1/arts/thoughts/2024/编程语言的进化/index.html` & `arts-2024.4.3.2/arts/thoughts/2024/编程语言的进化/index.html`

 * *Files identical despite different names*

### Comparing `arts-2024.4.3.1/arts/thoughts/2024/萝莉岛事件引发的信任危机/index.html` & `arts-2024.4.3.2/arts/thoughts/2024/萝莉岛事件引发的信任危机/index.html`

 * *Files identical despite different names*

### Comparing `arts-2024.4.3.1/arts/thoughts/2024/霍金去萝莉岛干嘛了/index.html` & `arts-2024.4.3.2/arts/thoughts/2024/霍金去萝莉岛干嘛了/index.html`

 * *Files identical despite different names*

### Comparing `arts-2024.4.3.1/arts/tutorials/600-用37行代码实现AI五子棋/README.md` & `arts-2024.4.3.2/arts/tutorials/600-用37行代码实现AI五子棋/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.3.1/arts/tutorials/750-正则表达式/README.md` & `arts-2024.4.3.2/arts/tutorials/750-正则表达式/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.3.1/pyproject.toml` & `arts-2024.4.3.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "arts"
-version = "2024.4.3.1"
+version = "2024.4.3.2"
 description = "对 Python 开发中常用功能的封装"
 dependencies = ["openai>=1.2.4", "numpy", "pymysql", "aiomysql", "pymongo", "motor", "pyppeteer>=2.0.0", "tornado"]
 
 
 requires-python = ">=3.10"
 readme = "README.md"
 authors = [{name = "江南雨上", email = "lcctoor@outlook.com"}]
```

### Comparing `arts-2024.4.3.1/PKG-INFO` & `arts-2024.4.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arts
-Version: 2024.4.3.1
+Version: 2024.4.3.2
 Summary: 对 Python 开发中常用功能的封装
 Author-email: 江南雨上 <lcctoor@outlook.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: openai>=1.2.4
 Requires-Dist: numpy
 Requires-Dist: pymysql
```

