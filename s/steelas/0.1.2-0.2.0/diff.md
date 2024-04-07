# Comparing `tmp/steelas-0.1.2.tar.gz` & `tmp/steelas-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "steelas-0.1.2.tar", last modified: Wed Mar 13 11:01:21 2024, max compression
+gzip compressed data, was "steelas-0.2.0.tar", last modified: Sun Apr  7 20:55:24 2024, max compression
```

## Comparing `steelas-0.1.2.tar` & `steelas-0.2.0.tar`

### file list

```diff
@@ -1,92 +1,99 @@
-drwxrwxrwx   0        0        0        0 2024-03-13 11:01:21.009411 steelas-0.1.2/
--rw-rw-rw-   0        0        0     1086 2024-02-29 10:08:22.000000 steelas-0.1.2/LICENSE
--rw-rw-rw-   0        0        0      137 2024-03-13 10:58:55.000000 steelas-0.1.2/MANIFEST.in
--rw-rw-rw-   0        0        0     2746 2024-03-13 11:01:21.003073 steelas-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     2074 2024-03-03 10:43:49.000000 steelas-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2024-03-13 11:01:20.275595 steelas-0.1.2/docs/
--rw-rw-rw-   0        0        0     1314 2024-03-03 10:43:49.000000 steelas-0.1.2/docs/index.md
--rw-rw-rw-   0        0        0      857 2024-03-03 10:43:49.000000 steelas-0.1.2/docs/install.md
--rw-rw-rw-   0        0        0      537 2024-03-03 10:43:49.000000 steelas-0.1.2/docs/reference.md
--rw-rw-rw-   0        0        0      839 2024-03-03 10:43:49.000000 steelas-0.1.2/docs/tutorial-1.md
-drwxrwxrwx   0        0        0        0 2024-03-13 11:01:20.281922 steelas-0.1.2/examples/
--rw-rw-rw-   0        0        0      712 2024-03-03 10:43:49.000000 steelas-0.1.2/examples/tutorial_1.py
--rw-rw-rw-   0        0        0      799 2024-03-13 10:51:06.000000 steelas-0.1.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-13 11:01:21.010808 steelas-0.1.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-03-13 11:01:20.192193 steelas-0.1.2/src/
-drwxrwxrwx   0        0        0        0 2024-03-13 11:01:20.287649 steelas-0.1.2/src/steelas/
--rw-rw-rw-   0        0        0       90 2024-03-03 10:43:49.000000 steelas-0.1.2/src/steelas/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-13 11:01:20.351818 steelas-0.1.2/src/steelas/__pycache__/
--rw-rw-rw-   0        0        0      251 2024-03-13 10:51:20.000000 steelas-0.1.2/src/steelas/__pycache__/__init__.cpython-311.pyc
-drwxrwxrwx   0        0        0        0 2024-03-13 11:01:20.412913 steelas-0.1.2/src/steelas/component/
--rw-rw-rw-   0        0        0       61 2024-03-03 10:43:49.000000 steelas-0.1.2/src/steelas/component/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-13 11:01:20.454354 steelas-0.1.2/src/steelas/component/__pycache__/
--rw-rw-rw-   0        0        0      246 2023-01-24 08:41:50.000000 steelas-0.1.2/src/steelas/component/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0    11837 2023-01-24 08:41:51.000000 steelas-0.1.2/src/steelas/component/__pycache__/bolt.cpython-310.pyc
--rw-rw-rw-   0        0        0     5021 2023-01-24 08:41:51.000000 steelas-0.1.2/src/steelas/component/__pycache__/plate.cpython-310.pyc
--rw-rw-rw-   0        0        0     4173 2023-01-24 08:41:51.000000 steelas-0.1.2/src/steelas/component/__pycache__/weld.cpython-310.pyc
--rw-rw-rw-   0        0        0    19938 2024-03-03 10:43:49.000000 steelas-0.1.2/src/steelas/component/bolt.py
--rw-rw-rw-   0        0        0     7550 2024-03-03 10:43:49.000000 steelas-0.1.2/src/steelas/component/plate.py
--rw-rw-rw-   0        0        0     5833 2024-03-03 10:43:49.000000 steelas-0.1.2/src/steelas/component/weld.py
-drwxrwxrwx   0        0        0        0 2024-03-13 11:01:20.483255 steelas-0.1.2/src/steelas/connection/
--rw-rw-rw-   0        0        0    16256 2024-03-03 10:43:49.000000 steelas-0.1.2/src/steelas/connection/FEP.py
--rw-rw-rw-   0        0        0    17910 2024-03-03 10:43:49.000000 steelas-0.1.2/src/steelas/connection/WSP.py
--rw-rw-rw-   0        0        0       90 2024-03-03 10:43:49.000000 steelas-0.1.2/src/steelas/connection/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-13 11:01:20.545987 steelas-0.1.2/src/steelas/connection/__pycache__/
--rw-rw-rw-   0        0        0     7255 2023-07-04 11:48:58.000000 steelas-0.1.2/src/steelas/connection/__pycache__/FEP.cpython-310.pyc
--rw-rw-rw-   0        0        0     8098 2023-06-28 02:50:29.000000 steelas-0.1.2/src/steelas/connection/__pycache__/WSP.cpython-310.pyc
--rw-rw-rw-   0        0        0      281 2023-01-24 11:40:12.000000 steelas-0.1.2/src/steelas/connection/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0     4793 2023-06-28 04:09:48.000000 steelas-0.1.2/src/steelas/connection/__pycache__/featured_member.cpython-310.pyc
--rw-rw-rw-   0        0        0     3987 2023-01-24 11:50:07.000000 steelas-0.1.2/src/steelas/connection/__pycache__/member_stub.cpython-310.pyc
--rw-rw-rw-   0        0        0    11614 2024-03-03 10:43:49.000000 steelas-0.1.2/src/steelas/connection/featured_member.py
-drwxrwxrwx   0        0        0        0 2024-03-13 11:01:20.670492 steelas-0.1.2/src/steelas/data/
--rw-rw-rw-   0        0        0    38804 2024-03-03 10:43:49.000000 steelas-0.1.2/src/steelas/data/ASI_FEP_connection.csv
--rw-rw-rw-   0        0        0   124750 2024-03-03 10:43:49.000000 steelas-0.1.2/src/steelas/data/ASI_WSP_connection.csv
--rw-rw-rw-   0        0        0     4360 2024-03-03 10:43:49.000000 steelas-0.1.2/src/steelas/data/AUS_bolt_groups.csv
--rw-rw-rw-   0        0        0      799 2024-03-03 10:43:49.000000 steelas-0.1.2/src/steelas/data/AUS_bolts.csv
--rw-rw-rw-   0        0        0     2239 2024-03-03 10:43:49.000000 steelas-0.1.2/src/steelas/data/AUS_coped_sections.csv
--rw-rw-rw-   0        0        0    21714 2024-03-03 10:43:49.000000 steelas-0.1.2/src/steelas/data/AUS_hollow_sections.csv
--rw-rw-rw-   0        0        0     6740 2024-03-03 10:43:49.000000 steelas-0.1.2/src/steelas/data/AUS_open_sections.csv
--rw-rw-rw-   0        0        0    14679 2024-03-03 10:43:49.000000 steelas-0.1.2/src/steelas/data/AUS_plates.csv
--rw-rw-rw-   0        0        0     3082 2024-03-03 10:43:49.000000 steelas-0.1.2/src/steelas/data/AUS_tee_sections.csv
--rw-rw-rw-   0        0        0      919 2024-03-03 10:43:49.000000 steelas-0.1.2/src/steelas/data/AUS_welds.csv
--rw-rw-rw-   0        0        0        0 2024-03-03 10:43:49.000000 steelas-0.1.2/src/steelas/data/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-13 11:01:20.682571 steelas-0.1.2/src/steelas/data/__pycache__/
--rw-rw-rw-   0        0        0      181 2024-03-13 10:51:23.000000 steelas-0.1.2/src/steelas/data/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0     1400 2024-03-13 10:51:23.000000 steelas-0.1.2/src/steelas/data/__pycache__/io.cpython-311.pyc
--rw-rw-rw-   0        0        0      685 2024-03-13 10:56:39.000000 steelas-0.1.2/src/steelas/data/io.py
-drwxrwxrwx   0        0        0        0 2024-03-13 11:01:20.759467 steelas-0.1.2/src/steelas/member/
--rw-rw-rw-   0        0        0       90 2024-03-03 10:43:49.000000 steelas-0.1.2/src/steelas/member/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-13 11:01:20.835133 steelas-0.1.2/src/steelas/member/__pycache__/
--rw-rw-rw-   0        0        0      243 2023-01-24 08:41:51.000000 steelas-0.1.2/src/steelas/member/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0      258 2024-03-13 10:51:21.000000 steelas-0.1.2/src/steelas/member/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0     8455 2023-06-28 02:45:20.000000 steelas-0.1.2/src/steelas/member/__pycache__/geometry.cpython-310.pyc
--rw-rw-rw-   0        0        0    15368 2024-03-13 10:51:21.000000 steelas-0.1.2/src/steelas/member/__pycache__/geometry.cpython-311.pyc
--rw-rw-rw-   0        0        0     9220 2023-09-27 06:21:35.000000 steelas-0.1.2/src/steelas/member/__pycache__/material.cpython-310.pyc
--rw-rw-rw-   0        0        0    15059 2023-06-28 02:45:20.000000 steelas-0.1.2/src/steelas/member/__pycache__/member.cpython-310.pyc
--rw-rw-rw-   0        0        0    15873 2023-06-28 02:45:20.000000 steelas-0.1.2/src/steelas/member/__pycache__/slenderness.cpython-310.pyc
--rw-rw-rw-   0        0        0    11060 2024-03-03 10:43:49.000000 steelas-0.1.2/src/steelas/member/geometry.py
--rw-rw-rw-   0        0        0    13805 2024-03-03 10:43:49.000000 steelas-0.1.2/src/steelas/member/material.py
--rw-rw-rw-   0        0        0    17777 2024-03-03 10:43:49.000000 steelas-0.1.2/src/steelas/member/member.py
--rw-rw-rw-   0        0        0    25258 2024-03-03 10:43:49.000000 steelas-0.1.2/src/steelas/member/slenderness.py
-drwxrwxrwx   0        0        0        0 2024-03-13 11:01:20.888972 steelas-0.1.2/src/steelas/shape/
--rw-rw-rw-   0        0        0        0 2024-03-03 10:43:49.000000 steelas-0.1.2/src/steelas/shape/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-13 11:01:20.986255 steelas-0.1.2/src/steelas/shape/__pycache__/
--rw-rw-rw-   0        0        0      182 2024-03-13 10:51:23.000000 steelas-0.1.2/src/steelas/shape/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0     3494 2024-03-13 10:51:23.000000 steelas-0.1.2/src/steelas/shape/__pycache__/circularhollow.cpython-311.pyc
--rw-rw-rw-   0        0        0    10554 2024-03-13 10:51:23.000000 steelas-0.1.2/src/steelas/shape/__pycache__/cshape.cpython-311.pyc
--rw-rw-rw-   0        0        0     7015 2024-03-13 10:51:23.000000 steelas-0.1.2/src/steelas/shape/__pycache__/ishape.cpython-311.pyc
--rw-rw-rw-   0        0        0     2003 2024-03-13 10:51:23.000000 steelas-0.1.2/src/steelas/shape/__pycache__/rectangleplate.cpython-311.pyc
--rw-rw-rw-   0        0        0     8929 2024-03-13 10:51:23.000000 steelas-0.1.2/src/steelas/shape/__pycache__/rectangularhollow.cpython-311.pyc
--rw-rw-rw-   0        0        0     8631 2024-03-13 10:51:23.000000 steelas-0.1.2/src/steelas/shape/__pycache__/tshape.cpython-311.pyc
--rw-rw-rw-   0        0        0     1531 2024-03-03 10:43:49.000000 steelas-0.1.2/src/steelas/shape/circularhollow.py
--rw-rw-rw-   0        0        0     5468 2024-03-03 10:43:49.000000 steelas-0.1.2/src/steelas/shape/cshape.py
--rw-rw-rw-   0        0        0     3311 2024-03-03 10:43:49.000000 steelas-0.1.2/src/steelas/shape/ishape.py
--rw-rw-rw-   0        0        0     2658 2024-03-03 10:43:49.000000 steelas-0.1.2/src/steelas/shape/rectangleplate.py
--rw-rw-rw-   0        0        0     3279 2024-03-03 10:43:49.000000 steelas-0.1.2/src/steelas/shape/rectangularhollow.py
--rw-rw-rw-   0        0        0     4518 2024-03-03 10:43:49.000000 steelas-0.1.2/src/steelas/shape/tshape.py
-drwxrwxrwx   0        0        0        0 2024-03-13 11:01:20.997376 steelas-0.1.2/src/steelas.egg-info/
--rw-rw-rw-   0        0        0     2746 2024-03-13 11:01:20.000000 steelas-0.1.2/src/steelas.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2865 2024-03-13 11:01:20.000000 steelas-0.1.2/src/steelas.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-13 11:01:20.000000 steelas-0.1.2/src/steelas.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2024-03-13 11:01:20.000000 steelas-0.1.2/src/steelas.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-03-13 11:01:20.000000 steelas-0.1.2/src/steelas.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-07 20:55:24.207889 steelas-0.2.0/
+-rw-rw-rw-   0        0        0     1086 2024-02-29 10:08:22.000000 steelas-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0      137 2024-04-07 20:52:52.000000 steelas-0.2.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2746 2024-04-07 20:55:24.206328 steelas-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2074 2024-03-03 10:43:49.000000 steelas-0.2.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-07 20:55:23.947420 steelas-0.2.0/docs/
+-rw-rw-rw-   0        0        0     1676 2024-04-07 20:54:34.000000 steelas-0.2.0/docs/index.md
+-rw-rw-rw-   0        0        0      857 2024-04-07 20:54:34.000000 steelas-0.2.0/docs/install.md
+-rw-rw-rw-   0        0        0      557 2024-04-07 20:54:34.000000 steelas-0.2.0/docs/reference.md
+-rw-rw-rw-   0        0        0     1205 2024-04-07 20:54:34.000000 steelas-0.2.0/docs/tutorial-1.md
+-rw-rw-rw-   0        0        0     3030 2024-04-07 20:54:34.000000 steelas-0.2.0/docs/tutorial-2.md
+-rw-rw-rw-   0        0        0     4656 2024-04-07 20:54:34.000000 steelas-0.2.0/docs/tutorial-3.md
+drwxrwxrwx   0        0        0        0 2024-04-07 20:55:23.957312 steelas-0.2.0/examples/
+-rw-rw-rw-   0        0        0      585 2024-04-07 20:54:34.000000 steelas-0.2.0/examples/tutorial_1.py
+-rw-rw-rw-   0        0        0     2030 2024-04-07 20:54:34.000000 steelas-0.2.0/examples/tutorial_2.py
+-rw-rw-rw-   0        0        0     2936 2024-04-07 20:54:34.000000 steelas-0.2.0/examples/tutorial_3.py
+-rw-rw-rw-   0        0        0      799 2024-04-07 20:54:34.000000 steelas-0.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-07 20:55:24.209692 steelas-0.2.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-07 20:55:23.899066 steelas-0.2.0/src/
+drwxrwxrwx   0        0        0        0 2024-04-07 20:55:23.960369 steelas-0.2.0/src/steelas/
+-rw-rw-rw-   0        0        0       90 2024-03-03 10:43:49.000000 steelas-0.2.0/src/steelas/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-07 20:55:23.978882 steelas-0.2.0/src/steelas/__pycache__/
+-rw-rw-rw-   0        0        0      251 2024-03-13 10:51:20.000000 steelas-0.2.0/src/steelas/__pycache__/__init__.cpython-311.pyc
+drwxrwxrwx   0        0        0        0 2024-04-07 20:55:23.994755 steelas-0.2.0/src/steelas/component/
+-rw-rw-rw-   0        0        0       61 2024-03-03 10:43:49.000000 steelas-0.2.0/src/steelas/component/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-07 20:55:24.009169 steelas-0.2.0/src/steelas/component/__pycache__/
+-rw-rw-rw-   0        0        0      246 2023-01-24 08:41:50.000000 steelas-0.2.0/src/steelas/component/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0    11837 2023-01-24 08:41:51.000000 steelas-0.2.0/src/steelas/component/__pycache__/bolt.cpython-310.pyc
+-rw-rw-rw-   0        0        0     5021 2023-01-24 08:41:51.000000 steelas-0.2.0/src/steelas/component/__pycache__/plate.cpython-310.pyc
+-rw-rw-rw-   0        0        0     4173 2023-01-24 08:41:51.000000 steelas-0.2.0/src/steelas/component/__pycache__/weld.cpython-310.pyc
+-rw-rw-rw-   0        0        0    19938 2024-03-03 10:43:49.000000 steelas-0.2.0/src/steelas/component/bolt.py
+-rw-rw-rw-   0        0        0     7550 2024-03-03 10:43:49.000000 steelas-0.2.0/src/steelas/component/plate.py
+-rw-rw-rw-   0        0        0     5833 2024-03-03 10:43:49.000000 steelas-0.2.0/src/steelas/component/weld.py
+drwxrwxrwx   0        0        0        0 2024-04-07 20:55:24.023628 steelas-0.2.0/src/steelas/connection/
+-rw-rw-rw-   0        0        0    16256 2024-03-03 10:43:49.000000 steelas-0.2.0/src/steelas/connection/FEP.py
+-rw-rw-rw-   0        0        0    17910 2024-03-03 10:43:49.000000 steelas-0.2.0/src/steelas/connection/WSP.py
+-rw-rw-rw-   0        0        0       90 2024-03-03 10:43:49.000000 steelas-0.2.0/src/steelas/connection/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-07 20:55:24.042418 steelas-0.2.0/src/steelas/connection/__pycache__/
+-rw-rw-rw-   0        0        0     7255 2023-07-04 11:48:58.000000 steelas-0.2.0/src/steelas/connection/__pycache__/FEP.cpython-310.pyc
+-rw-rw-rw-   0        0        0     8098 2023-06-28 02:50:29.000000 steelas-0.2.0/src/steelas/connection/__pycache__/WSP.cpython-310.pyc
+-rw-rw-rw-   0        0        0      281 2023-01-24 11:40:12.000000 steelas-0.2.0/src/steelas/connection/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0     4793 2023-06-28 04:09:48.000000 steelas-0.2.0/src/steelas/connection/__pycache__/featured_member.cpython-310.pyc
+-rw-rw-rw-   0        0        0     3987 2023-01-24 11:50:07.000000 steelas-0.2.0/src/steelas/connection/__pycache__/member_stub.cpython-310.pyc
+-rw-rw-rw-   0        0        0    11614 2024-03-03 10:43:49.000000 steelas-0.2.0/src/steelas/connection/featured_member.py
+drwxrwxrwx   0        0        0        0 2024-04-07 20:55:24.089342 steelas-0.2.0/src/steelas/data/
+-rw-rw-rw-   0        0        0    38804 2024-03-03 10:43:49.000000 steelas-0.2.0/src/steelas/data/ASI_FEP_connection.csv
+-rw-rw-rw-   0        0        0   124750 2024-03-03 10:43:49.000000 steelas-0.2.0/src/steelas/data/ASI_WSP_connection.csv
+-rw-rw-rw-   0        0        0     4360 2024-03-03 10:43:49.000000 steelas-0.2.0/src/steelas/data/AUS_bolt_groups.csv
+-rw-rw-rw-   0        0        0      799 2024-03-03 10:43:49.000000 steelas-0.2.0/src/steelas/data/AUS_bolts.csv
+-rw-rw-rw-   0        0        0     2239 2024-03-03 10:43:49.000000 steelas-0.2.0/src/steelas/data/AUS_coped_sections.csv
+-rw-rw-rw-   0        0        0    21714 2024-03-03 10:43:49.000000 steelas-0.2.0/src/steelas/data/AUS_hollow_sections.csv
+-rw-rw-rw-   0        0        0     6740 2024-03-03 10:43:49.000000 steelas-0.2.0/src/steelas/data/AUS_open_sections.csv
+-rw-rw-rw-   0        0        0    14679 2024-03-03 10:43:49.000000 steelas-0.2.0/src/steelas/data/AUS_plates.csv
+-rw-rw-rw-   0        0        0     3082 2024-03-03 10:43:49.000000 steelas-0.2.0/src/steelas/data/AUS_tee_sections.csv
+-rw-rw-rw-   0        0        0      919 2024-03-03 10:43:49.000000 steelas-0.2.0/src/steelas/data/AUS_welds.csv
+-rw-rw-rw-   0        0        0        0 2024-03-03 10:43:49.000000 steelas-0.2.0/src/steelas/data/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-07 20:55:24.094116 steelas-0.2.0/src/steelas/data/__pycache__/
+-rw-rw-rw-   0        0        0      181 2024-03-13 10:51:23.000000 steelas-0.2.0/src/steelas/data/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0     4218 2024-04-07 19:05:46.000000 steelas-0.2.0/src/steelas/data/__pycache__/io.cpython-311.pyc
+-rw-rw-rw-   0        0        0     3656 2024-04-07 20:54:34.000000 steelas-0.2.0/src/steelas/data/io.py
+drwxrwxrwx   0        0        0        0 2024-04-07 20:55:24.109885 steelas-0.2.0/src/steelas/member/
+-rw-rw-rw-   0        0        0       90 2024-03-03 10:43:49.000000 steelas-0.2.0/src/steelas/member/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-07 20:55:24.148816 steelas-0.2.0/src/steelas/member/__pycache__/
+-rw-rw-rw-   0        0        0      243 2023-01-24 08:41:51.000000 steelas-0.2.0/src/steelas/member/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0      258 2024-03-13 10:51:21.000000 steelas-0.2.0/src/steelas/member/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0     8455 2023-06-28 02:45:20.000000 steelas-0.2.0/src/steelas/member/__pycache__/geometry.cpython-310.pyc
+-rw-rw-rw-   0        0        0    16053 2024-04-04 20:53:34.000000 steelas-0.2.0/src/steelas/member/__pycache__/geometry.cpython-311.pyc
+-rw-rw-rw-   0        0        0     9220 2023-09-27 06:21:35.000000 steelas-0.2.0/src/steelas/member/__pycache__/material.cpython-310.pyc
+-rw-rw-rw-   0        0        0    17057 2024-04-02 07:37:01.000000 steelas-0.2.0/src/steelas/member/__pycache__/material.cpython-311.pyc
+-rw-rw-rw-   0        0        0    15059 2023-06-28 02:45:20.000000 steelas-0.2.0/src/steelas/member/__pycache__/member.cpython-310.pyc
+-rw-rw-rw-   0        0        0    25620 2024-04-07 19:04:14.000000 steelas-0.2.0/src/steelas/member/__pycache__/member.cpython-311.pyc
+-rw-rw-rw-   0        0        0    15873 2023-06-28 02:45:20.000000 steelas-0.2.0/src/steelas/member/__pycache__/slenderness.cpython-310.pyc
+-rw-rw-rw-   0        0        0    28445 2024-04-02 06:15:05.000000 steelas-0.2.0/src/steelas/member/__pycache__/slenderness.cpython-311.pyc
+-rw-rw-rw-   0        0        0    11397 2024-04-07 20:54:34.000000 steelas-0.2.0/src/steelas/member/geometry.py
+-rw-rw-rw-   0        0        0    14470 2024-04-07 20:54:34.000000 steelas-0.2.0/src/steelas/member/material.py
+-rw-rw-rw-   0        0        0    18676 2024-04-07 20:54:34.000000 steelas-0.2.0/src/steelas/member/member.py
+-rw-rw-rw-   0        0        0    26914 2024-04-07 20:54:34.000000 steelas-0.2.0/src/steelas/member/slenderness.py
+drwxrwxrwx   0        0        0        0 2024-04-07 20:55:24.172148 steelas-0.2.0/src/steelas/shape/
+-rw-rw-rw-   0        0        0        0 2024-03-03 10:43:49.000000 steelas-0.2.0/src/steelas/shape/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-07 20:55:24.198736 steelas-0.2.0/src/steelas/shape/__pycache__/
+-rw-rw-rw-   0        0        0      182 2024-03-13 10:51:23.000000 steelas-0.2.0/src/steelas/shape/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0     3494 2024-03-13 10:51:23.000000 steelas-0.2.0/src/steelas/shape/__pycache__/circularhollow.cpython-311.pyc
+-rw-rw-rw-   0        0        0    10554 2024-03-13 10:51:23.000000 steelas-0.2.0/src/steelas/shape/__pycache__/cshape.cpython-311.pyc
+-rw-rw-rw-   0        0        0     7015 2024-03-13 10:51:23.000000 steelas-0.2.0/src/steelas/shape/__pycache__/ishape.cpython-311.pyc
+-rw-rw-rw-   0        0        0     2003 2024-03-13 10:51:23.000000 steelas-0.2.0/src/steelas/shape/__pycache__/rectangleplate.cpython-311.pyc
+-rw-rw-rw-   0        0        0     8929 2024-03-13 10:51:23.000000 steelas-0.2.0/src/steelas/shape/__pycache__/rectangularhollow.cpython-311.pyc
+-rw-rw-rw-   0        0        0     8631 2024-03-13 10:51:23.000000 steelas-0.2.0/src/steelas/shape/__pycache__/tshape.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1531 2024-03-03 10:43:49.000000 steelas-0.2.0/src/steelas/shape/circularhollow.py
+-rw-rw-rw-   0        0        0     5468 2024-03-03 10:43:49.000000 steelas-0.2.0/src/steelas/shape/cshape.py
+-rw-rw-rw-   0        0        0     3311 2024-03-03 10:43:49.000000 steelas-0.2.0/src/steelas/shape/ishape.py
+-rw-rw-rw-   0        0        0     2658 2024-03-03 10:43:49.000000 steelas-0.2.0/src/steelas/shape/rectangleplate.py
+-rw-rw-rw-   0        0        0     3279 2024-03-03 10:43:49.000000 steelas-0.2.0/src/steelas/shape/rectangularhollow.py
+-rw-rw-rw-   0        0        0     4518 2024-03-03 10:43:49.000000 steelas-0.2.0/src/steelas/shape/tshape.py
+drwxrwxrwx   0        0        0        0 2024-04-07 20:55:24.202723 steelas-0.2.0/src/steelas.egg-info/
+-rw-rw-rw-   0        0        0     2746 2024-04-07 20:55:23.000000 steelas-0.2.0/src/steelas.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3118 2024-04-07 20:55:23.000000 steelas-0.2.0/src/steelas.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-07 20:55:23.000000 steelas-0.2.0/src/steelas.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       28 2024-04-07 20:55:23.000000 steelas-0.2.0/src/steelas.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-07 20:55:23.000000 steelas-0.2.0/src/steelas.egg-info/top_level.txt
```

### Comparing `steelas-0.1.2/LICENSE` & `steelas-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `steelas-0.1.2/PKG-INFO` & `steelas-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: steelas
-Version: 0.1.2
+Version: 0.2.0
 Summary: steelas is a Python package for the design of steel structures to relevant Australian Standards
 Author-email: Joe Gattas <j.gattas@uq.edu.au>, Yuyu Wang <yuyu.wang@uq.net.au>
 Project-URL: Homepage, https://github.com/Folded-Structures-Lab/steel-as
 Keywords: AS4100,steel structures,structural engineering
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy>=1.25.0
 Requires-Dist: pandas>=2.0.2
 
 # About
 *steelas* is a Python package with tools to support research and design of Australian steel structures. It can be used to determine the material properties, section properties, and design capacities for structural members as per Australian Standard AS4100:2020 (Steel Structures).
```

### Comparing `steelas-0.1.2/README.md` & `steelas-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `steelas-0.1.2/docs/index.md` & `steelas-0.2.0/docs/index.md`

 * *Files 20% similar despite different names*

```diff
@@ -4,26 +4,30 @@
 
 *steelas* is developed by [Yuyu Wang](https://github.com/wyy0990), [Joe Gattas](https://researchers.uq.edu.au/researcher/9443),  and research collaborators at the [University of Queensland](https://civil.uq.edu.au/).
 
 # Contents
 - [Installation](install.md)
 - Tutorials
     - [Quick Start](tutorial-1.md)
+    - [Geometry and Material](tutorial-2.md)
+    - [Tension and Compression Capacity](tutorial-3.md)
 - [API Reference](reference.md)
 
 
 # Support
 Please see the project [Github repository](https://github.com/Folded-Structures-Lab/steel-as) and README file for the latest updates and issues. 
 
 # License
 *steelas* is provided under an MIT License. Please refer to the project Github repository and LICENSE file for more information. 
 
 
 # Acknowledgements
 This package has been developed from research projects supported by the [University of Queensland](https://civil.uq.edu.au/).
 
-If you use *steelas* for projects or scientific publications, please cite our work.
+If you use *steelas* for projects or scientific publications, please consider citing our journal paper:
+> Wang, Y., Bottazzi, V.S., & Gattas, J. M. (2024). A novel framework for set-based steel connection design automation. *Computers and Structures*. [doi:10.1016/j.compstruc.2024.107366](https://doi.org/10.1016/j.compstruc.2024.107366).
+
 
 ## Contributors: 
 
 - [Dr Joe Gattas](https://researchers.uq.edu.au/researcher/9443)
 - [Yuyu Wang](https://github.com/wyy0990)
```

### Comparing `steelas-0.1.2/docs/install.md` & `steelas-0.2.0/docs/install.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 This page will guide you through the installation process for *steelas*.
 
 ## Prerequisites
 
 Before you begin, ensure:
 
-- You have installed Python 3.10+.
+- You have installed Python 3.11+.
 - You have a basic understanding of Python programming.
 
 ## Installation
 
 *steelas* and its required dependencies can be installed from the Python Package index using pip:
 ```
 pip install steelas
```

### Comparing `steelas-0.1.2/docs/reference.md` & `steelas-0.2.0/docs/reference.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 
 # API
-<!-- 
+
 ## Members
 
+Coming Soon!
+
+<!-- 
+
 ### *geometry* Module
 
 :::steelas.member.geometry
 
 ### *material* Module
 
 :::steelas.member.material
```

### Comparing `steelas-0.1.2/pyproject.toml` & `steelas-0.2.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "steelas"
-version = "0.1.2"
+version = "0.2.0"
 authors = [
   { name="Joe Gattas", email="j.gattas@uq.edu.au" },
   { name="Yuyu Wang", email="yuyu.wang@uq.net.au"},
 ]
 description = "steelas is a Python package for the design of steel structures to relevant Australian Standards"
 readme = "README.md"
-requires-python = ">=3.10"
+requires-python = ">=3.11"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 keywords = ["AS4100", "steel structures", "structural engineering"]
 dependencies = [
```

### Comparing `steelas-0.1.2/src/steelas/component/__pycache__/bolt.cpython-310.pyc` & `steelas-0.2.0/src/steelas/component/__pycache__/bolt.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `steelas-0.1.2/src/steelas/component/__pycache__/plate.cpython-310.pyc` & `steelas-0.2.0/src/steelas/component/__pycache__/plate.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `steelas-0.1.2/src/steelas/component/__pycache__/weld.cpython-310.pyc` & `steelas-0.2.0/src/steelas/component/__pycache__/weld.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `steelas-0.1.2/src/steelas/component/bolt.py` & `steelas-0.2.0/src/steelas/component/bolt.py`

 * *Files identical despite different names*

### Comparing `steelas-0.1.2/src/steelas/component/plate.py` & `steelas-0.2.0/src/steelas/component/plate.py`

 * *Files identical despite different names*

### Comparing `steelas-0.1.2/src/steelas/component/weld.py` & `steelas-0.2.0/src/steelas/component/weld.py`

 * *Files identical despite different names*

### Comparing `steelas-0.1.2/src/steelas/connection/FEP.py` & `steelas-0.2.0/src/steelas/connection/FEP.py`

 * *Files identical despite different names*

### Comparing `steelas-0.1.2/src/steelas/connection/WSP.py` & `steelas-0.2.0/src/steelas/connection/WSP.py`

 * *Files identical despite different names*

### Comparing `steelas-0.1.2/src/steelas/connection/__pycache__/FEP.cpython-310.pyc` & `steelas-0.2.0/src/steelas/connection/__pycache__/FEP.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `steelas-0.1.2/src/steelas/connection/__pycache__/WSP.cpython-310.pyc` & `steelas-0.2.0/src/steelas/connection/__pycache__/WSP.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `steelas-0.1.2/src/steelas/connection/__pycache__/featured_member.cpython-310.pyc` & `steelas-0.2.0/src/steelas/connection/__pycache__/featured_member.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `steelas-0.1.2/src/steelas/connection/__pycache__/member_stub.cpython-310.pyc` & `steelas-0.2.0/src/steelas/connection/__pycache__/member_stub.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `steelas-0.1.2/src/steelas/connection/featured_member.py` & `steelas-0.2.0/src/steelas/connection/featured_member.py`

 * *Files identical despite different names*

### Comparing `steelas-0.1.2/src/steelas/data/ASI_FEP_connection.csv` & `steelas-0.2.0/src/steelas/data/ASI_FEP_connection.csv`

 * *Files identical despite different names*

### Comparing `steelas-0.1.2/src/steelas/data/ASI_WSP_connection.csv` & `steelas-0.2.0/src/steelas/data/ASI_WSP_connection.csv`

 * *Files identical despite different names*

### Comparing `steelas-0.1.2/src/steelas/data/AUS_bolt_groups.csv` & `steelas-0.2.0/src/steelas/data/AUS_bolt_groups.csv`

 * *Files identical despite different names*

### Comparing `steelas-0.1.2/src/steelas/data/AUS_bolts.csv` & `steelas-0.2.0/src/steelas/data/AUS_bolts.csv`

 * *Files identical despite different names*

### Comparing `steelas-0.1.2/src/steelas/data/AUS_coped_sections.csv` & `steelas-0.2.0/src/steelas/data/AUS_coped_sections.csv`

 * *Files identical despite different names*

### Comparing `steelas-0.1.2/src/steelas/data/AUS_hollow_sections.csv` & `steelas-0.2.0/src/steelas/data/AUS_hollow_sections.csv`

 * *Files identical despite different names*

### Comparing `steelas-0.1.2/src/steelas/data/AUS_open_sections.csv` & `steelas-0.2.0/src/steelas/data/AUS_open_sections.csv`

 * *Files identical despite different names*

### Comparing `steelas-0.1.2/src/steelas/data/AUS_plates.csv` & `steelas-0.2.0/src/steelas/data/AUS_plates.csv`

 * *Files identical despite different names*

### Comparing `steelas-0.1.2/src/steelas/data/AUS_tee_sections.csv` & `steelas-0.2.0/src/steelas/data/AUS_tee_sections.csv`

 * *Files identical despite different names*

### Comparing `steelas-0.1.2/src/steelas/data/AUS_welds.csv` & `steelas-0.2.0/src/steelas/data/AUS_welds.csv`

 * *Files identical despite different names*

### Comparing `steelas-0.1.2/src/steelas/member/__pycache__/geometry.cpython-310.pyc` & `steelas-0.2.0/src/steelas/member/__pycache__/geometry.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `steelas-0.1.2/src/steelas/member/__pycache__/geometry.cpython-311.pyc` & `steelas-0.2.0/src/steelas/member/__pycache__/geometry.cpython-311.pyc`

 * *Files 8% similar despite different names*

#### Python bytecode

```diff
@@ -1,25 +1,27 @@
 magic:    0xa70d0d0a
-moddate:  0x6554e465 (Sun Mar  3 10:43:49 2024 UTC)
-files sz: 11060
+moddate:  0x03090f66 (Thu Apr  4 20:09:39 2024 UTC)
+files sz: 11397
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 16777216
    code
       0x970064005a00640164026c016d025a020100640164036c036d045a046d
       055a056d065a060100640164046c076d085a086d095a090100640164056c
-      0a5a0b640164066c0c6d0d5a0d6d0e5a0e6d0f5a0f6d105a106d115a116d
-      125a120100020065086407ac08a6010000ab010000000000000000020047
-      0064098400640aa6020000ab020000000000000000a6000000ab00000000
-      00000000005a1364055300
+      0a6d0b5a0b0100640164066c0c5a0d640164076c0e6d0f5a0f6d105a106d
+      115a116d125a126d135a136d145a140100640164086c156d165a16010002
+      00470064098400640a650ba6030000ab0300000000000000005a17020065
+      08640bac0ca6010000ab01000000000000000002004700640d8400640ea6
+      020000ab020000000000000000a6000000ab0000000000000000005a1864
+      065300
      0           0 RESUME                   0
    
-     3           2 LOAD_CONST               0 ('\nThis module provides classes and functions to manage steel sections and their geometric properties.\n\nClasses:    \n    SectionGeometry: TODO. \n\nFunctions:\n    import_section_library(): Returns a DataFrame containing the section library defined\n    in steelas/data/\n\n')
+     3           2 LOAD_CONST               0 ('\nThis module provides classes and functions to manage steel sections and their geometric properties.\n\nClasses:\n    SectionGeometry: TODO.\n\nFunctions:\n    import_section_library(): Returns a DataFrame containing the section library defined\n    in steelas/data/\n\n')
                  4 STORE_NAME               0 (__doc__)
    
     15           6 LOAD_CONST               1 (0)
                  8 LOAD_CONST               2 (('annotations',))
                 10 IMPORT_NAME              1 (__future__)
                 12 IMPORT_FROM              2 (annotations)
                 14 STORE_NAME               2 (annotations)
@@ -42,64 +44,157 @@
                 44 IMPORT_FROM              8 (dataclass)
                 46 STORE_NAME               8 (dataclass)
                 48 IMPORT_FROM              9 (field)
                 50 STORE_NAME               9 (field)
                 52 POP_TOP
    
     19          54 LOAD_CONST               1 (0)
-                56 LOAD_CONST               5 (None)
-                58 IMPORT_NAME             10 (numpy)
-                60 STORE_NAME              11 (np)
+                56 LOAD_CONST               5 (('StrEnum',))
+                58 IMPORT_NAME             10 (enum)
+                60 IMPORT_FROM             11 (StrEnum)
+                62 STORE_NAME              11 (StrEnum)
+                64 POP_TOP
    
-    21          62 LOAD_CONST               1 (0)
-                64 LOAD_CONST               6 (('circularhollow', 'rectangularhollow', 'ishape', 'cshape', 'tshape', 'rectangleplate'))
-                66 IMPORT_NAME             12 (steelas.shape)
-                68 IMPORT_FROM             13 (circularhollow)
-                70 STORE_NAME              13 (circularhollow)
-                72 IMPORT_FROM             14 (rectangularhollow)
-                74 STORE_NAME              14 (rectangularhollow)
-                76 IMPORT_FROM             15 (ishape)
-                78 STORE_NAME              15 (ishape)
-                80 IMPORT_FROM             16 (cshape)
-                82 STORE_NAME              16 (cshape)
-                84 IMPORT_FROM             17 (tshape)
-                86 STORE_NAME              17 (tshape)
-                88 IMPORT_FROM             18 (rectangleplate)
-                90 STORE_NAME              18 (rectangleplate)
-                92 POP_TOP
+    20          66 LOAD_CONST               1 (0)
+                68 LOAD_CONST               6 (None)
+                70 IMPORT_NAME             12 (numpy)
+                72 STORE_NAME              13 (np)
    
-    39          94 PUSH_NULL
-                96 LOAD_NAME                8 (dataclass)
-                98 LOAD_CONST               7 (True)
-               100 KW_NAMES                 8
-               102 PRECALL                  1
-               106 CALL                     1
+    22          74 LOAD_CONST               1 (0)
+                76 LOAD_CONST               7 (('circularhollow', 'rectangularhollow', 'ishape', 'cshape', 'tshape', 'rectangleplate'))
+                78 IMPORT_NAME             14 (steelas.shape)
+                80 IMPORT_FROM             15 (circularhollow)
+                82 STORE_NAME              15 (circularhollow)
+                84 IMPORT_FROM             16 (rectangularhollow)
+                86 STORE_NAME              16 (rectangularhollow)
+                88 IMPORT_FROM             17 (ishape)
+                90 STORE_NAME              17 (ishape)
+                92 IMPORT_FROM             18 (cshape)
+                94 STORE_NAME              18 (cshape)
+                96 IMPORT_FROM             19 (tshape)
+                98 STORE_NAME              19 (tshape)
+               100 IMPORT_FROM             20 (rectangleplate)
+               102 STORE_NAME              20 (rectangleplate)
+               104 POP_TOP
    
-    40         116 PUSH_NULL
-               118 LOAD_BUILD_CLASS
-               120 LOAD_CONST               9 (<code object SectionGeometry, file "C:\Users\uqjgatta\Documents\GitHub\steel-as\src\steelas\member\geometry.py", line 39>)
-               122 MAKE_FUNCTION            0
-               124 LOAD_CONST              10 ('SectionGeometry')
-               126 PRECALL                  2
-               130 CALL                     2
+    31         106 LOAD_CONST               1 (0)
+               108 LOAD_CONST               8 (('report',))
+               110 IMPORT_NAME             21 (steelas.data.io)
+               112 IMPORT_FROM             22 (report)
+               114 STORE_NAME              22 (report)
+               116 POP_TOP
    
-    39         140 PRECALL                  0
-               144 CALL                     0
+    34         118 PUSH_NULL
+               120 LOAD_BUILD_CLASS
+               122 LOAD_CONST               9 (<code object SectionType, file "C:\Users\uqjgatta\Documents\GitHub\steel-as\src\steelas\member\geometry.py", line 34>)
+               124 MAKE_FUNCTION            0
+               126 LOAD_CONST              10 ('SectionType')
+               128 LOAD_NAME               11 (StrEnum)
+               130 PRECALL                  3
+               134 CALL                     3
+               144 STORE_NAME              23 (SectionType)
    
-    40         154 STORE_NAME              19 (SectionGeometry)
-               156 LOAD_CONST               5 (None)
-               158 RETURN_VALUE
+    55         146 PUSH_NULL
+               148 LOAD_NAME                8 (dataclass)
+               150 LOAD_CONST              11 (True)
+               152 KW_NAMES                12
+               154 PRECALL                  1
+               158 CALL                     1
+   
+    56         168 PUSH_NULL
+               170 LOAD_BUILD_CLASS
+               172 LOAD_CONST              13 (<code object SectionGeometry, file "C:\Users\uqjgatta\Documents\GitHub\steel-as\src\steelas\member\geometry.py", line 55>)
+               174 MAKE_FUNCTION            0
+               176 LOAD_CONST              14 ('SectionGeometry')
+               178 PRECALL                  2
+               182 CALL                     2
+   
+    55         192 PRECALL                  0
+               196 CALL                     0
+   
+    56         206 STORE_NAME              24 (SectionGeometry)
+               208 LOAD_CONST               6 (None)
+               210 RETURN_VALUE
    consts
-      '\nThis module provides classes and functions to manage steel sections and their geometric properties.\n\nClasses:    \n    SectionGeometry: TODO. \n\nFunctions:\n    import_section_library(): Returns a DataFrame containing the section library defined\n    in steelas/data/\n\n'
+      '\nThis module provides classes and functions to manage steel sections and their geometric properties.\n\nClasses:\n    SectionGeometry: TODO.\n\nFunctions:\n    import_section_library(): Returns a DataFrame containing the section library defined\n    in steelas/data/\n\n'
       0
       ('annotations',)
       ('floor', 'log10', 'isnan')
       ('dataclass', 'field')
+      ('StrEnum',)
       None
       ('circularhollow', 'rectangularhollow', 'ishape', 'cshape', 'tshape', 'rectangleplate')
+      ('report',)
+      code
+         argcount  : 0
+         nlocals   : 0
+         stacksize : 1
+         flags     : 16777216
+         code
+            0x970065005a0164005a0264015a0364025a0464035a0564045a0664055a
+            0764065a0864075a0964085a0a64095a0b640a5a0c640b5300
+          34           0 RESUME                   0
+                       2 LOAD_NAME                0 (__name__)
+                       4 STORE_NAME               1 (__module__)
+                       6 LOAD_CONST               0 ('SectionType')
+                       8 STORE_NAME               2 (__qualname__)
+         
+          35          10 LOAD_CONST               1 ('CHS')
+                      12 STORE_NAME               3 (CHS)
+         
+          36          14 LOAD_CONST               2 ('RHS')
+                      16 STORE_NAME               4 (RHS)
+         
+          37          18 LOAD_CONST               3 ('SHS')
+                      20 STORE_NAME               5 (SHS)
+         
+          38          22 LOAD_CONST               4 ('WB')
+                      24 STORE_NAME               6 (WB)
+         
+          39          26 LOAD_CONST               5 ('UB')
+                      28 STORE_NAME               7 (UB)
+         
+          40          30 LOAD_CONST               6 ('UC')
+                      32 STORE_NAME               8 (UC)
+         
+          41          34 LOAD_CONST               7 ('PFC')
+                      36 STORE_NAME               9 (PFC)
+         
+          42          38 LOAD_CONST               8 ('BT')
+                      40 STORE_NAME              10 (BT)
+         
+          43          42 LOAD_CONST               9 ('CT')
+                      44 STORE_NAME              11 (CT)
+         
+          44          46 LOAD_CONST              10 ('RectPlate')
+                      48 STORE_NAME              12 (RectPlate)
+                      50 LOAD_CONST              11 (None)
+                      52 RETURN_VALUE
+         consts
+            'SectionType'
+            'CHS'
+            'RHS'
+            'SHS'
+            'WB'
+            'UB'
+            'UC'
+            'PFC'
+            'BT'
+            'CT'
+            'RectPlate'
+            None
+         names      ('__name__', '__module__', '__qualname__', 'CHS', 'RHS', 'SHS', 'WB', 'UB', 'UC', 'PFC', 'BT', 'CT', 'RectPlate')
+         varnames   ()
+         freevars   ()
+         cellvars   ()
+         filename   'C:\\Users\\uqjgatta\\Documents\\GitHub\\steel-as\\src\\steelas\\member\\geometry.py'
+         name       'SectionType'
+         firstlineno 34
+         lnotab 0x0a01040104010401040104010401040104010401
+      'SectionType'
       True
       ('kw_only',)
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 4
          flags     : 16777216
@@ -120,377 +215,381 @@
             153c00000065086a0900000000000000005a186407650564163c00000065
             086a0900000000000000005a196407650564173c00000065086a09000000
             00000000005a1a6407650564183c00000065086a0900000000000000005a
             1b6407650564193c00000065086a0900000000000000005a1c6407650564
             1a3c00000065086a0900000000000000005a1d64076505641b3c00000064
             1c5a1e64076505641d3c000000641c5a1f64076505641e3c000000020065
             20641f6420ac21a6020000ab0200000000000000005a216422650564233c
-            000000642484005a22642584005a236436642784045a246436642884045a
-            256436642984045a266436642a84045a276528642b8400a6000000ab0000
-            000000000000005a296528642c8400a6000000ab0000000000000000005a
-            2a652b642d8400a6000000ab0000000000000000005a2c6528642e8400a6
-            000000ab0000000000000000005a2d65286436642f8404a6000000ab0000
-            000000000000005a2e652864308400a6000000ab0000000000000000005a
-            2f652864318400a6000000ab0000000000000000005a30652864328400a6
-            000000ab0000000000000000005a316528643664338404a6000000ab0000
-            000000000000005a326528643664348404a6000000ab0000000000000000
-            005a3364355300
-          39           0 RESUME                   0
+            000000642484005a22642584005a23642684005a246437642884045a2564
+            37642984045a266437642a84045a276437642b84045a286529642c8400a6
+            000000ab0000000000000000005a2a6529642d8400a6000000ab00000000
+            00000000005a2b652c642e8400a6000000ab0000000000000000005a2d65
+            29642f8400a6000000ab0000000000000000005a2e6529643764308404a6
+            000000ab0000000000000000005a2f652964318400a6000000ab00000000
+            00000000005a30652964328400a6000000ab0000000000000000005a3165
+            2964338400a6000000ab0000000000000000005a326529643764348404a6
+            000000ab0000000000000000005a336529643764358404a6000000ab0000
+            000000000000005a3464365300
+          55           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('SectionGeometry')
                        8 STORE_NAME               2 (__qualname__)
                       10 SETUP_ANNOTATIONS
          
-          41          12 LOAD_CONST               1 ('\n    Represents the geometric properties of a structural section.\n\n    This class encapsulates the geometric dimensions and derived properties of various structural section types, \n    such as I-shapes (WB, WC, UB, UC), Channels (PFC), Hollow Sections (RHS, SHS, CHS), and Plates. It provides \n    functionality to calculate sectional properties based on the specified geometry, including area, moment of \n    inertia, section modulus, and radius of gyration, among others.\n\n    Attributes:\n        name (str): A descriptive name for the section.\n        section (str): The specific section designation.\n        sec_type (str): The type of section (e.g., CHS, RHS, UB).\n        d, b, t_f, t_w, t, r_1, r_2, alpha, r_o: Geometric dimensions of the section.\n        A_g (float): Gross area of the section.\n        I_x, I_y (float): Second moment of area about the x-axis and y-axis, respectively.\n        S_x, S_y (float): Elastic section modulus about the x-axis and y-axis, respectively.\n        Z_x, Z_y (float): Plastic section modulus about the x-axis and y-axis, respectively.\n        r_x, r_y (float): Radius of gyration about the x-axis and y-axis, respectively.\n        I_w (float): Warping constant.\n        J (float): Torsional constant.\n        x_c, y_c (float): Coordinates of the centroid, default to 0.\n        sig_figs (int): Number of significant figures for rounding calculations, defaults to 4.\n    ')
+          57          12 LOAD_CONST               1 ('\n    Represents the geometric properties of a structural section.\n\n    This class encapsulates the geometric dimensions and derived properties of various structural section types,\n    such as I-shapes (WB, WC, UB, UC), Channels (PFC), Hollow Sections (RHS, SHS, CHS), and Plates. It provides\n    functionality to calculate sectional properties based on the specified geometry, including area, moment of\n    inertia, section modulus, and radius of gyration, among others.\n\n    Attributes:\n        name (str): A descriptive name for the section.\n        section (str): The specific section designation.\n        sec_type (str): The type of section (e.g., CHS, RHS, UB).\n        d, b, t_f, t_w, t, r_1, r_2, alpha, r_o: Geometric dimensions of the section.\n        A_g (float): Gross area of the section.\n        I_x, I_y (float): Second moment of area about the x-axis and y-axis, respectively.\n        S_x, S_y (float): Elastic section modulus about the x-axis and y-axis, respectively.\n        Z_x, Z_y (float): Plastic section modulus about the x-axis and y-axis, respectively.\n        r_x, r_y (float): Radius of gyration about the x-axis and y-axis, respectively.\n        I_w (float): Warping constant.\n        J (float): Torsional constant.\n        x_c, y_c (float): Coordinates of the centroid, default to 0.\n        sig_figs (int): Number of significant figures for rounding calculations, defaults to 4.\n    ')
                       14 STORE_NAME               3 (__doc__)
          
-          64          16 LOAD_CONST               2 ('')
+          81          16 LOAD_CONST               2 ('')
                       18 STORE_NAME               4 (name)
                       20 LOAD_CONST               3 ('str')
                       22 LOAD_NAME                5 (__annotations__)
                       24 LOAD_CONST               4 ('name')
                       26 STORE_SUBSCR
          
-          65          30 LOAD_CONST               2 ('')
+          82          30 LOAD_CONST               2 ('')
                       32 STORE_NAME               6 (section)
                       34 LOAD_CONST               3 ('str')
                       36 LOAD_NAME                5 (__annotations__)
                       38 LOAD_CONST               5 ('section')
                       40 STORE_SUBSCR
          
-          66          44 LOAD_CONST               2 ('')
+          83          44 LOAD_CONST               2 ('')
                       46 STORE_NAME               7 (sec_type)
                       48 LOAD_CONST               3 ('str')
                       50 LOAD_NAME                5 (__annotations__)
                       52 LOAD_CONST               6 ('sec_type')
                       54 STORE_SUBSCR
          
-          68          58 LOAD_NAME                8 (np)
+          85          58 LOAD_NAME                8 (np)
                       60 LOAD_ATTR                9 (nan)
                       70 STORE_NAME              10 (d)
                       72 LOAD_CONST               7 ('float')
                       74 LOAD_NAME                5 (__annotations__)
                       76 LOAD_CONST               8 ('d')
                       78 STORE_SUBSCR
          
-          69          82 LOAD_NAME                8 (np)
+          86          82 LOAD_NAME                8 (np)
                       84 LOAD_ATTR                9 (nan)
                       94 STORE_NAME              11 (b)
                       96 LOAD_CONST               7 ('float')
                       98 LOAD_NAME                5 (__annotations__)
                      100 LOAD_CONST               9 ('b')
                      102 STORE_SUBSCR
          
-          70         106 LOAD_NAME                8 (np)
+          87         106 LOAD_NAME                8 (np)
                      108 LOAD_ATTR                9 (nan)
                      118 STORE_NAME              12 (t_f)
                      120 LOAD_CONST               7 ('float')
                      122 LOAD_NAME                5 (__annotations__)
                      124 LOAD_CONST              10 ('t_f')
                      126 STORE_SUBSCR
          
-          71         130 LOAD_NAME                8 (np)
+          88         130 LOAD_NAME                8 (np)
                      132 LOAD_ATTR                9 (nan)
                      142 STORE_NAME              13 (t_w)
                      144 LOAD_CONST               7 ('float')
                      146 LOAD_NAME                5 (__annotations__)
                      148 LOAD_CONST              11 ('t_w')
                      150 STORE_SUBSCR
          
-          72         154 LOAD_NAME                8 (np)
+          89         154 LOAD_NAME                8 (np)
                      156 LOAD_ATTR                9 (nan)
                      166 STORE_NAME              14 (t)
                      168 LOAD_CONST               7 ('float')
                      170 LOAD_NAME                5 (__annotations__)
                      172 LOAD_CONST              12 ('t')
                      174 STORE_SUBSCR
          
-          73         178 LOAD_NAME                8 (np)
+          90         178 LOAD_NAME                8 (np)
                      180 LOAD_ATTR                9 (nan)
                      190 STORE_NAME              15 (r_1)
                      192 LOAD_CONST               7 ('float')
                      194 LOAD_NAME                5 (__annotations__)
                      196 LOAD_CONST              13 ('r_1')
                      198 STORE_SUBSCR
          
-          74         202 LOAD_NAME                8 (np)
+          91         202 LOAD_NAME                8 (np)
                      204 LOAD_ATTR                9 (nan)
                      214 STORE_NAME              16 (r_2)
                      216 LOAD_CONST               7 ('float')
                      218 LOAD_NAME                5 (__annotations__)
                      220 LOAD_CONST              14 ('r_2')
                      222 STORE_SUBSCR
          
-          75         226 LOAD_NAME                8 (np)
+          92         226 LOAD_NAME                8 (np)
                      228 LOAD_ATTR                9 (nan)
                      238 STORE_NAME              17 (alpha)
                      240 LOAD_CONST               7 ('float')
                      242 LOAD_NAME                5 (__annotations__)
                      244 LOAD_CONST              15 ('alpha')
                      246 STORE_SUBSCR
          
-          76         250 LOAD_NAME                8 (np)
+          93         250 LOAD_NAME                8 (np)
                      252 LOAD_ATTR                9 (nan)
                      262 STORE_NAME              18 (r_o)
                      264 LOAD_CONST               7 ('float')
                      266 LOAD_NAME                5 (__annotations__)
                      268 LOAD_CONST              16 ('r_o')
                      270 STORE_SUBSCR
          
-          78         274 LOAD_NAME                8 (np)
+          95         274 LOAD_NAME                8 (np)
                      276 LOAD_ATTR                9 (nan)
                      286 STORE_NAME              19 (A_g)
                      288 LOAD_CONST               7 ('float')
                      290 LOAD_NAME                5 (__annotations__)
                      292 LOAD_CONST              17 ('A_g')
                      294 STORE_SUBSCR
          
-          79         298 LOAD_NAME                8 (np)
+          96         298 LOAD_NAME                8 (np)
                      300 LOAD_ATTR                9 (nan)
                      310 STORE_NAME              20 (I_x)
                      312 LOAD_CONST               7 ('float')
                      314 LOAD_NAME                5 (__annotations__)
                      316 LOAD_CONST              18 ('I_x')
                      318 STORE_SUBSCR
          
-          80         322 LOAD_NAME                8 (np)
+          97         322 LOAD_NAME                8 (np)
                      324 LOAD_ATTR                9 (nan)
                      334 STORE_NAME              21 (I_y)
                      336 LOAD_CONST               7 ('float')
                      338 LOAD_NAME                5 (__annotations__)
                      340 LOAD_CONST              19 ('I_y')
                      342 STORE_SUBSCR
          
-          81         346 LOAD_NAME                8 (np)
+          98         346 LOAD_NAME                8 (np)
                      348 LOAD_ATTR                9 (nan)
                      358 STORE_NAME              22 (S_x)
                      360 LOAD_CONST               7 ('float')
                      362 LOAD_NAME                5 (__annotations__)
                      364 LOAD_CONST              20 ('S_x')
                      366 STORE_SUBSCR
          
-          82         370 LOAD_NAME                8 (np)
+          99         370 LOAD_NAME                8 (np)
                      372 LOAD_ATTR                9 (nan)
                      382 STORE_NAME              23 (S_y)
                      384 LOAD_CONST               7 ('float')
                      386 LOAD_NAME                5 (__annotations__)
                      388 LOAD_CONST              21 ('S_y')
                      390 STORE_SUBSCR
          
-          83         394 LOAD_NAME                8 (np)
+         100         394 LOAD_NAME                8 (np)
                      396 LOAD_ATTR                9 (nan)
                      406 STORE_NAME              24 (Z_x)
                      408 LOAD_CONST               7 ('float')
                      410 LOAD_NAME                5 (__annotations__)
                      412 LOAD_CONST              22 ('Z_x')
                      414 STORE_SUBSCR
          
-          84         418 LOAD_NAME                8 (np)
+         101         418 LOAD_NAME                8 (np)
                      420 LOAD_ATTR                9 (nan)
                      430 STORE_NAME              25 (Z_y)
                      432 LOAD_CONST               7 ('float')
                      434 LOAD_NAME                5 (__annotations__)
                      436 LOAD_CONST              23 ('Z_y')
                      438 STORE_SUBSCR
          
-          85         442 LOAD_NAME                8 (np)
+         102         442 LOAD_NAME                8 (np)
                      444 LOAD_ATTR                9 (nan)
                      454 STORE_NAME              26 (r_x)
                      456 LOAD_CONST               7 ('float')
                      458 LOAD_NAME                5 (__annotations__)
                      460 LOAD_CONST              24 ('r_x')
                      462 STORE_SUBSCR
          
-          86         466 LOAD_NAME                8 (np)
+         103         466 LOAD_NAME                8 (np)
                      468 LOAD_ATTR                9 (nan)
                      478 STORE_NAME              27 (r_y)
                      480 LOAD_CONST               7 ('float')
                      482 LOAD_NAME                5 (__annotations__)
                      484 LOAD_CONST              25 ('r_y')
                      486 STORE_SUBSCR
          
-          87         490 LOAD_NAME                8 (np)
+         104         490 LOAD_NAME                8 (np)
                      492 LOAD_ATTR                9 (nan)
                      502 STORE_NAME              28 (I_w)
                      504 LOAD_CONST               7 ('float')
                      506 LOAD_NAME                5 (__annotations__)
                      508 LOAD_CONST              26 ('I_w')
                      510 STORE_SUBSCR
          
-          88         514 LOAD_NAME                8 (np)
+         105         514 LOAD_NAME                8 (np)
                      516 LOAD_ATTR                9 (nan)
                      526 STORE_NAME              29 (J)
                      528 LOAD_CONST               7 ('float')
                      530 LOAD_NAME                5 (__annotations__)
                      532 LOAD_CONST              27 ('J')
                      534 STORE_SUBSCR
          
-          90         538 LOAD_CONST              28 (0)
+         107         538 LOAD_CONST              28 (0)
                      540 STORE_NAME              30 (x_c)
                      542 LOAD_CONST               7 ('float')
                      544 LOAD_NAME                5 (__annotations__)
                      546 LOAD_CONST              29 ('x_c')
                      548 STORE_SUBSCR
          
-          91         552 LOAD_CONST              28 (0)
+         108         552 LOAD_CONST              28 (0)
                      554 STORE_NAME              31 (y_c)
                      556 LOAD_CONST               7 ('float')
                      558 LOAD_NAME                5 (__annotations__)
                      560 LOAD_CONST              30 ('y_c')
                      562 STORE_SUBSCR
          
-          94         566 PUSH_NULL
+         111         566 PUSH_NULL
                      568 LOAD_NAME               32 (field)
                      570 LOAD_CONST              31 (False)
                      572 LOAD_CONST              32 (4)
                      574 KW_NAMES                33
                      576 PRECALL                  2
                      580 CALL                     2
                      590 STORE_NAME              33 (sig_figs)
                      592 LOAD_CONST              34 ('int')
                      594 LOAD_NAME                5 (__annotations__)
                      596 LOAD_CONST              35 ('sig_figs')
                      598 STORE_SUBSCR
          
-          96         602 LOAD_CONST              36 (<code object __post_init__, file "C:\Users\uqjgatta\Documents\GitHub\steel-as\src\steelas\member\geometry.py", line 96>)
+         113         602 LOAD_CONST              36 (<code object __post_init__, file "C:\Users\uqjgatta\Documents\GitHub\steel-as\src\steelas\member\geometry.py", line 113>)
                      604 MAKE_FUNCTION            0
                      606 STORE_NAME              34 (__post_init__)
          
-         100         608 LOAD_CONST              37 (<code object solve_shape, file "C:\Users\uqjgatta\Documents\GitHub\steel-as\src\steelas\member\geometry.py", line 100>)
+         117         608 LOAD_CONST              37 (<code object report, file "C:\Users\uqjgatta\Documents\GitHub\steel-as\src\steelas\member\geometry.py", line 117>)
                      610 MAKE_FUNCTION            0
-                     612 STORE_NAME              35 (solve_shape)
+                     612 STORE_NAME              35 (report)
+         
+         120         614 LOAD_CONST              38 (<code object solve_shape, file "C:\Users\uqjgatta\Documents\GitHub\steel-as\src\steelas\member\geometry.py", line 120>)
+                     616 MAKE_FUNCTION            0
+                     618 STORE_NAME              36 (solve_shape)
          
-         141         614 LOAD_CONST              54 (('return', 'float'))
-                     616 LOAD_CONST              39 (<code object _Z_x, file "C:\Users\uqjgatta\Documents\GitHub\steel-as\src\steelas\member\geometry.py", line 141>)
-                     618 MAKE_FUNCTION            4 (annotations)
-                     620 STORE_NAME              36 (_Z_x)
+         161         620 LOAD_CONST              55 (('return', 'float'))
+                     622 LOAD_CONST              40 (<code object _Z_x, file "C:\Users\uqjgatta\Documents\GitHub\steel-as\src\steelas\member\geometry.py", line 161>)
+                     624 MAKE_FUNCTION            4 (annotations)
+                     626 STORE_NAME              37 (_Z_x)
          
-         144         622 LOAD_CONST              54 (('return', 'float'))
-                     624 LOAD_CONST              40 (<code object _Z_y, file "C:\Users\uqjgatta\Documents\GitHub\steel-as\src\steelas\member\geometry.py", line 144>)
-                     626 MAKE_FUNCTION            4 (annotations)
-                     628 STORE_NAME              37 (_Z_y)
+         164         628 LOAD_CONST              55 (('return', 'float'))
+                     630 LOAD_CONST              41 (<code object _Z_y, file "C:\Users\uqjgatta\Documents\GitHub\steel-as\src\steelas\member\geometry.py", line 164>)
+                     632 MAKE_FUNCTION            4 (annotations)
+                     634 STORE_NAME              38 (_Z_y)
          
-         147         630 LOAD_CONST              54 (('return', 'float'))
-                     632 LOAD_CONST              41 (<code object _r_x, file "C:\Users\uqjgatta\Documents\GitHub\steel-as\src\steelas\member\geometry.py", line 147>)
-                     634 MAKE_FUNCTION            4 (annotations)
-                     636 STORE_NAME              38 (_r_x)
+         167         636 LOAD_CONST              55 (('return', 'float'))
+                     638 LOAD_CONST              42 (<code object _r_x, file "C:\Users\uqjgatta\Documents\GitHub\steel-as\src\steelas\member\geometry.py", line 167>)
+                     640 MAKE_FUNCTION            4 (annotations)
+                     642 STORE_NAME              39 (_r_x)
          
-         150         638 LOAD_CONST              54 (('return', 'float'))
-                     640 LOAD_CONST              42 (<code object _r_y, file "C:\Users\uqjgatta\Documents\GitHub\steel-as\src\steelas\member\geometry.py", line 150>)
-                     642 MAKE_FUNCTION            4 (annotations)
-                     644 STORE_NAME              39 (_r_y)
+         170         644 LOAD_CONST              55 (('return', 'float'))
+                     646 LOAD_CONST              43 (<code object _r_y, file "C:\Users\uqjgatta\Documents\GitHub\steel-as\src\steelas\member\geometry.py", line 170>)
+                     648 MAKE_FUNCTION            4 (annotations)
+                     650 STORE_NAME              40 (_r_y)
          
-         153         646 LOAD_NAME               40 (property)
+         173         652 LOAD_NAME               41 (property)
          
-         154         648 LOAD_CONST              43 (<code object x_max, file "C:\Users\uqjgatta\Documents\GitHub\steel-as\src\steelas\member\geometry.py", line 153>)
-                     650 MAKE_FUNCTION            0
+         174         654 LOAD_CONST              44 (<code object x_max, file "C:\Users\uqjgatta\Documents\GitHub\steel-as\src\steelas\member\geometry.py", line 173>)
+                     656 MAKE_FUNCTION            0
          
-         153         652 PRECALL                  0
-                     656 CALL                     0
+         173         658 PRECALL                  0
+                     662 CALL                     0
          
-         154         666 STORE_NAME              41 (x_max)
+         174         672 STORE_NAME              42 (x_max)
          
-         165         668 LOAD_NAME               40 (property)
+         185         674 LOAD_NAME               41 (property)
          
-         166         670 LOAD_CONST              44 (<code object y_max, file "C:\Users\uqjgatta\Documents\GitHub\steel-as\src\steelas\member\geometry.py", line 165>)
-                     672 MAKE_FUNCTION            0
+         186         676 LOAD_CONST              45 (<code object y_max, file "C:\Users\uqjgatta\Documents\GitHub\steel-as\src\steelas\member\geometry.py", line 185>)
+                     678 MAKE_FUNCTION            0
          
-         165         674 PRECALL                  0
-                     678 CALL                     0
+         185         680 PRECALL                  0
+                     684 CALL                     0
          
-         166         688 STORE_NAME              42 (y_max)
+         186         694 STORE_NAME              43 (y_max)
          
-         174         690 LOAD_NAME               43 (classmethod)
+         194         696 LOAD_NAME               44 (classmethod)
          
-         175         692 LOAD_CONST              45 (<code object from_dict, file "C:\Users\uqjgatta\Documents\GitHub\steel-as\src\steelas\member\geometry.py", line 174>)
-                     694 MAKE_FUNCTION            0
+         195         698 LOAD_CONST              46 (<code object from_dict, file "C:\Users\uqjgatta\Documents\GitHub\steel-as\src\steelas\member\geometry.py", line 194>)
+                     700 MAKE_FUNCTION            0
          
-         174         696 PRECALL                  0
-                     700 CALL                     0
+         194         702 PRECALL                  0
+                     706 CALL                     0
          
-         175         710 STORE_NAME              44 (from_dict)
+         195         716 STORE_NAME              45 (from_dict)
          
-         188         712 LOAD_NAME               40 (property)
+         208         718 LOAD_NAME               41 (property)
          
-         189         714 LOAD_CONST              46 (<code object d_1, file "C:\Users\uqjgatta\Documents\GitHub\steel-as\src\steelas\member\geometry.py", line 188>)
-                     716 MAKE_FUNCTION            0
+         209         720 LOAD_CONST              47 (<code object d_1, file "C:\Users\uqjgatta\Documents\GitHub\steel-as\src\steelas\member\geometry.py", line 208>)
+                     722 MAKE_FUNCTION            0
          
-         188         718 PRECALL                  0
-                     722 CALL                     0
+         208         724 PRECALL                  0
+                     728 CALL                     0
          
-         189         732 STORE_NAME              45 (d_1)
+         209         738 STORE_NAME              46 (d_1)
          
-         209         734 LOAD_NAME               40 (property)
+         229         740 LOAD_NAME               41 (property)
          
-         210         736 LOAD_CONST              54 (('return', 'float'))
-                     738 LOAD_CONST              47 (<code object A_w, file "C:\Users\uqjgatta\Documents\GitHub\steel-as\src\steelas\member\geometry.py", line 209>)
-                     740 MAKE_FUNCTION            4 (annotations)
+         230         742 LOAD_CONST              55 (('return', 'float'))
+                     744 LOAD_CONST              48 (<code object A_w, file "C:\Users\uqjgatta\Documents\GitHub\steel-as\src\steelas\member\geometry.py", line 229>)
+                     746 MAKE_FUNCTION            4 (annotations)
          
-         209         742 PRECALL                  0
-                     746 CALL                     0
+         229         748 PRECALL                  0
+                     752 CALL                     0
          
-         210         756 STORE_NAME              46 (A_w)
+         230         762 STORE_NAME              47 (A_w)
          
-         230         758 LOAD_NAME               40 (property)
+         250         764 LOAD_NAME               41 (property)
          
-         231         760 LOAD_CONST              48 (<code object d_w, file "C:\Users\uqjgatta\Documents\GitHub\steel-as\src\steelas\member\geometry.py", line 230>)
-                     762 MAKE_FUNCTION            0
+         251         766 LOAD_CONST              49 (<code object d_w, file "C:\Users\uqjgatta\Documents\GitHub\steel-as\src\steelas\member\geometry.py", line 250>)
+                     768 MAKE_FUNCTION            0
          
-         230         764 PRECALL                  0
-                     768 CALL                     0
+         250         770 PRECALL                  0
+                     774 CALL                     0
          
-         231         778 STORE_NAME              47 (d_w)
+         251         784 STORE_NAME              48 (d_w)
          
-         248         780 LOAD_NAME               40 (property)
+         268         786 LOAD_NAME               41 (property)
          
-         249         782 LOAD_CONST              49 (<code object d_p, file "C:\Users\uqjgatta\Documents\GitHub\steel-as\src\steelas\member\geometry.py", line 248>)
-                     784 MAKE_FUNCTION            0
+         269         788 LOAD_CONST              50 (<code object d_p, file "C:\Users\uqjgatta\Documents\GitHub\steel-as\src\steelas\member\geometry.py", line 268>)
+                     790 MAKE_FUNCTION            0
          
-         248         786 PRECALL                  0
-                     790 CALL                     0
+         268         792 PRECALL                  0
+                     796 CALL                     0
          
-         249         800 STORE_NAME              48 (d_p)
+         269         806 STORE_NAME              49 (d_p)
          
-         256         802 LOAD_NAME               40 (property)
+         276         808 LOAD_NAME               41 (property)
          
-         257         804 LOAD_CONST              50 (<code object b_ff, file "C:\Users\uqjgatta\Documents\GitHub\steel-as\src\steelas\member\geometry.py", line 256>)
-                     806 MAKE_FUNCTION            0
+         277         810 LOAD_CONST              51 (<code object b_ff, file "C:\Users\uqjgatta\Documents\GitHub\steel-as\src\steelas\member\geometry.py", line 276>)
+                     812 MAKE_FUNCTION            0
          
-         256         808 PRECALL                  0
-                     812 CALL                     0
+         276         814 PRECALL                  0
+                     818 CALL                     0
          
-         257         822 STORE_NAME              49 (b_ff)
+         277         828 STORE_NAME              50 (b_ff)
          
-         273         824 LOAD_NAME               40 (property)
+         293         830 LOAD_NAME               41 (property)
          
-         274         826 LOAD_CONST              54 (('return', 'float'))
-                     828 LOAD_CONST              51 (<code object Q_c, file "C:\Users\uqjgatta\Documents\GitHub\steel-as\src\steelas\member\geometry.py", line 273>)
-                     830 MAKE_FUNCTION            4 (annotations)
+         294         832 LOAD_CONST              55 (('return', 'float'))
+                     834 LOAD_CONST              52 (<code object Q_c, file "C:\Users\uqjgatta\Documents\GitHub\steel-as\src\steelas\member\geometry.py", line 293>)
+                     836 MAKE_FUNCTION            4 (annotations)
          
-         273         832 PRECALL                  0
-                     836 CALL                     0
+         293         838 PRECALL                  0
+                     842 CALL                     0
          
-         274         846 STORE_NAME              50 (Q_c)
+         294         852 STORE_NAME              51 (Q_c)
          
-         307         848 LOAD_NAME               40 (property)
+         327         854 LOAD_NAME               41 (property)
          
-         308         850 LOAD_CONST              54 (('return', 'float'))
-                     852 LOAD_CONST              52 (<code object shear_stress_uniformity, file "C:\Users\uqjgatta\Documents\GitHub\steel-as\src\steelas\member\geometry.py", line 307>)
-                     854 MAKE_FUNCTION            4 (annotations)
+         328         856 LOAD_CONST              55 (('return', 'float'))
+                     858 LOAD_CONST              53 (<code object shear_stress_uniformity, file "C:\Users\uqjgatta\Documents\GitHub\steel-as\src\steelas\member\geometry.py", line 327>)
+                     860 MAKE_FUNCTION            4 (annotations)
          
-         307         856 PRECALL                  0
-                     860 CALL                     0
+         327         862 PRECALL                  0
+                     866 CALL                     0
          
-         308         870 STORE_NAME              51 (shear_stress_uniformity)
-                     872 LOAD_CONST              53 (None)
-                     874 RETURN_VALUE
+         328         876 STORE_NAME              52 (shear_stress_uniformity)
+                     878 LOAD_CONST              54 (None)
+                     880 RETURN_VALUE
          consts
             'SectionGeometry'
-            '\n    Represents the geometric properties of a structural section.\n\n    This class encapsulates the geometric dimensions and derived properties of various structural section types, \n    such as I-shapes (WB, WC, UB, UC), Channels (PFC), Hollow Sections (RHS, SHS, CHS), and Plates. It provides \n    functionality to calculate sectional properties based on the specified geometry, including area, moment of \n    inertia, section modulus, and radius of gyration, among others.\n\n    Attributes:\n        name (str): A descriptive name for the section.\n        section (str): The specific section designation.\n        sec_type (str): The type of section (e.g., CHS, RHS, UB).\n        d, b, t_f, t_w, t, r_1, r_2, alpha, r_o: Geometric dimensions of the section.\n        A_g (float): Gross area of the section.\n        I_x, I_y (float): Second moment of area about the x-axis and y-axis, respectively.\n        S_x, S_y (float): Elastic section modulus about the x-axis and y-axis, respectively.\n        Z_x, Z_y (float): Plastic section modulus about the x-axis and y-axis, respectively.\n        r_x, r_y (float): Radius of gyration about the x-axis and y-axis, respectively.\n        I_w (float): Warping constant.\n        J (float): Torsional constant.\n        x_c, y_c (float): Coordinates of the centroid, default to 0.\n        sig_figs (int): Number of significant figures for rounding calculations, defaults to 4.\n    '
+            '\n    Represents the geometric properties of a structural section.\n\n    This class encapsulates the geometric dimensions and derived properties of various structural section types,\n    such as I-shapes (WB, WC, UB, UC), Channels (PFC), Hollow Sections (RHS, SHS, CHS), and Plates. It provides\n    functionality to calculate sectional properties based on the specified geometry, including area, moment of\n    inertia, section modulus, and radius of gyration, among others.\n\n    Attributes:\n        name (str): A descriptive name for the section.\n        section (str): The specific section designation.\n        sec_type (str): The type of section (e.g., CHS, RHS, UB).\n        d, b, t_f, t_w, t, r_1, r_2, alpha, r_o: Geometric dimensions of the section.\n        A_g (float): Gross area of the section.\n        I_x, I_y (float): Second moment of area about the x-axis and y-axis, respectively.\n        S_x, S_y (float): Elastic section modulus about the x-axis and y-axis, respectively.\n        Z_x, Z_y (float): Plastic section modulus about the x-axis and y-axis, respectively.\n        r_x, r_y (float): Radius of gyration about the x-axis and y-axis, respectively.\n        I_w (float): Warping constant.\n        J (float): Torsional constant.\n        x_c, y_c (float): Coordinates of the centroid, default to 0.\n        sig_figs (int): Number of significant figures for rounding calculations, defaults to 4.\n    '
             ''
             'str'
             'name'
             'section'
             'sec_type'
             'float'
             'd'
@@ -526,45 +625,71 @@
                nlocals   : 1
                stacksize : 2
                flags     : 16777219
                code
                   0x97007c006a00000000000000000064016b030000000072167c00a00100
                   00000000000000000000000000000000000000a6000000ab000000000000
                   00000001006400530064005300
-                96           0 RESUME                   0
+               113           0 RESUME                   0
                
-                97           2 LOAD_FAST                0 (self)
+               114           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (sec_type)
                             14 LOAD_CONST               1 ('')
                             16 COMPARE_OP               3 (!=)
                             22 POP_JUMP_FORWARD_IF_FALSE    22 (to 68)
                
-                98          24 LOAD_FAST                0 (self)
+               115          24 LOAD_FAST                0 (self)
                             26 LOAD_METHOD              1 (solve_shape)
                             48 PRECALL                  0
                             52 CALL                     0
                             62 POP_TOP
                             64 LOAD_CONST               0 (None)
                             66 RETURN_VALUE
                
-                97     >>   68 LOAD_CONST               0 (None)
+               114     >>   68 LOAD_CONST               0 (None)
                             70 RETURN_VALUE
                consts
                   None
                   ''
                names      ('sec_type', 'solve_shape')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'C:\\Users\\uqjgatta\\Documents\\GitHub\\steel-as\\src\\steelas\\member\\geometry.py'
                name       '__post_init__'
-               firstlineno 96
+               firstlineno 113
                lnotab 0x020116012cff
             code
                argcount  : 1
+               nlocals   : 2
+               stacksize : 5
+               flags     : 16777227
+               code 0x97007401000000000000000000007c00660169007c01a4018e015300
+               117           0 RESUME                   0
+               
+               118           2 LOAD_GLOBAL              1 (NULL + report)
+                            14 LOAD_FAST                0 (self)
+                            16 BUILD_TUPLE              1
+                            18 BUILD_MAP                0
+                            20 LOAD_FAST                1 (kwargs)
+                            22 DICT_MERGE               1
+                            24 CALL_FUNCTION_EX         1
+                            26 RETURN_VALUE
+               consts
+                  None
+               names      ('report',)
+               varnames   ('self', 'kwargs')
+               freevars   ()
+               cellvars   ()
+               filename   'C:\\Users\\uqjgatta\\Documents\\GitHub\\steel-as\\src\\steelas\\member\\geometry.py'
+               name       'report'
+               firstlineno 117
+               lnotab 0x0201
+            code
+               argcount  : 1
                nlocals   : 4
                stacksize : 18
                flags     : 16777219
                code
                   0x97007c006a000000000000000000640176007208740200000000000000
                   0000007d016ea17c006a0000000000000000006402760072087404000000
                   000000000000007d016e907c006a00000000000000000064037600720874
@@ -605,208 +730,208 @@
                   0364096b0300000000725e7443000000000000000000007c007c02744500
                   0000000000000000007c037c006a190000000000000000743f0000000000
                   000000000074470000000000000000000074490000000000000000000074
                   4b000000000000000000007c03a6010000ab010000000000000000a60100
                   00ab010000000000000000a6010000ab010000000000000000a6010000ab
                   0100000000000000007a0a0000640a7a0a0000a6020000ab020000000000
                   000000a6030000ab03000000000000000001008c956400530064005300
-               100           0 RESUME                   0
+               120           0 RESUME                   0
                
-               101           2 LOAD_FAST                0 (self)
+               121           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (sec_type)
                             14 LOAD_CONST               1 (('CHS',))
                             16 CONTAINS_OP              0
                             18 POP_JUMP_FORWARD_IF_FALSE     8 (to 36)
                
-               102          20 LOAD_GLOBAL              2 (circularhollow)
+               122          20 LOAD_GLOBAL              2 (circularhollow)
                             32 STORE_FAST               1 (shape_fn)
                             34 JUMP_FORWARD           161 (to 358)
                
-               103     >>   36 LOAD_FAST                0 (self)
+               123     >>   36 LOAD_FAST                0 (self)
                             38 LOAD_ATTR                0 (sec_type)
                             48 LOAD_CONST               2 (('RHS', 'SHS'))
                             50 CONTAINS_OP              0
                             52 POP_JUMP_FORWARD_IF_FALSE     8 (to 70)
                
-               104          54 LOAD_GLOBAL              4 (rectangularhollow)
+               124          54 LOAD_GLOBAL              4 (rectangularhollow)
                             66 STORE_FAST               1 (shape_fn)
                             68 JUMP_FORWARD           144 (to 358)
                
-               105     >>   70 LOAD_FAST                0 (self)
+               125     >>   70 LOAD_FAST                0 (self)
                             72 LOAD_ATTR                0 (sec_type)
                             82 LOAD_CONST               3 (('WB', 'WC', 'UB', 'UC'))
                             84 CONTAINS_OP              0
                             86 POP_JUMP_FORWARD_IF_FALSE     8 (to 104)
                
-               106          88 LOAD_GLOBAL              6 (ishape)
+               126          88 LOAD_GLOBAL              6 (ishape)
                            100 STORE_FAST               1 (shape_fn)
                            102 JUMP_FORWARD           127 (to 358)
                
-               107     >>  104 LOAD_FAST                0 (self)
+               127     >>  104 LOAD_FAST                0 (self)
                            106 LOAD_ATTR                0 (sec_type)
                            116 LOAD_CONST               4 (('PFC',))
                            118 CONTAINS_OP              0
                            120 POP_JUMP_FORWARD_IF_FALSE    34 (to 190)
                
-               108         122 LOAD_GLOBAL              8 (cshape)
+               128         122 LOAD_GLOBAL              8 (cshape)
                            134 STORE_FAST               1 (shape_fn)
                
-               109         136 LOAD_FAST                1 (shape_fn)
+               129         136 LOAD_FAST                1 (shape_fn)
                            138 LOAD_METHOD              5 (x_c)
                            160 LOAD_FAST                0 (self)
                            162 PRECALL                  1
                            166 CALL                     1
                            176 LOAD_FAST                0 (self)
                            178 STORE_ATTR               5 (x_c)
                            188 JUMP_FORWARD            84 (to 358)
                
-               110     >>  190 LOAD_FAST                0 (self)
+               130     >>  190 LOAD_FAST                0 (self)
                            192 LOAD_ATTR                0 (sec_type)
                            202 LOAD_CONST               5 (('BT', 'CT'))
                            204 CONTAINS_OP              0
                            206 POP_JUMP_FORWARD_IF_FALSE    34 (to 276)
                
-               111         208 LOAD_GLOBAL             12 (tshape)
+               131         208 LOAD_GLOBAL             12 (tshape)
                            220 STORE_FAST               1 (shape_fn)
                
-               112         222 LOAD_FAST                1 (shape_fn)
+               132         222 LOAD_FAST                1 (shape_fn)
                            224 LOAD_METHOD              7 (y_c)
                            246 LOAD_FAST                0 (self)
                            248 PRECALL                  1
                            252 CALL                     1
                            262 LOAD_FAST                0 (self)
                            264 STORE_ATTR               7 (y_c)
                            274 JUMP_FORWARD            41 (to 358)
                
-               113     >>  276 LOAD_FAST                0 (self)
+               133     >>  276 LOAD_FAST                0 (self)
                            278 LOAD_ATTR                0 (sec_type)
                            288 LOAD_CONST               6 (('RectPlate',))
                            290 CONTAINS_OP              0
                            292 POP_JUMP_FORWARD_IF_FALSE     8 (to 310)
                
-               114         294 LOAD_GLOBAL             16 (rectangleplate)
+               134         294 LOAD_GLOBAL             16 (rectangleplate)
                            306 STORE_FAST               1 (shape_fn)
                            308 JUMP_FORWARD            24 (to 358)
                
-               116     >>  310 LOAD_GLOBAL             19 (NULL + NotImplementedError)
+               136     >>  310 LOAD_GLOBAL             19 (NULL + NotImplementedError)
                
-               117         322 LOAD_CONST               7 ('section type: ')
+               137         322 LOAD_CONST               7 ('section type: ')
                            324 LOAD_FAST                0 (self)
                            326 LOAD_ATTR                0 (sec_type)
                            336 FORMAT_VALUE             0
                            338 LOAD_CONST               8 (' has no shape function')
                            340 BUILD_STRING             3
                
-               116         342 PRECALL                  1
+               136         342 PRECALL                  1
                            346 CALL                     1
                            356 RAISE_VARARGS            1
                
-               120     >>  358 LOAD_FAST                1 (shape_fn)
+               140     >>  358 LOAD_FAST                1 (shape_fn)
                            360 LOAD_METHOD             10 (A_g)
                            382 LOAD_FAST                0 (self)
                            384 PRECALL                  1
                            388 CALL                     1
                            398 LOAD_FAST                0 (self)
                            400 STORE_ATTR              10 (A_g)
                
-               121         410 LOAD_FAST                1 (shape_fn)
+               141         410 LOAD_FAST                1 (shape_fn)
                            412 LOAD_METHOD             11 (I_x)
                            434 LOAD_FAST                0 (self)
                            436 PRECALL                  1
                            440 CALL                     1
                            450 LOAD_FAST                0 (self)
                            452 STORE_ATTR              11 (I_x)
                
-               122         462 LOAD_FAST                1 (shape_fn)
+               142         462 LOAD_FAST                1 (shape_fn)
                            464 LOAD_METHOD             12 (I_y)
                            486 LOAD_FAST                0 (self)
                            488 PRECALL                  1
                            492 CALL                     1
                            502 LOAD_FAST                0 (self)
                            504 STORE_ATTR              12 (I_y)
                
-               123         514 LOAD_FAST                1 (shape_fn)
+               143         514 LOAD_FAST                1 (shape_fn)
                            516 LOAD_METHOD             13 (S_x)
                            538 LOAD_FAST                0 (self)
                            540 PRECALL                  1
                            544 CALL                     1
                            554 LOAD_FAST                0 (self)
                            556 STORE_ATTR              13 (S_x)
                
-               124         566 LOAD_FAST                1 (shape_fn)
+               144         566 LOAD_FAST                1 (shape_fn)
                            568 LOAD_METHOD             14 (S_y)
                            590 LOAD_FAST                0 (self)
                            592 PRECALL                  1
                            596 CALL                     1
                            606 LOAD_FAST                0 (self)
                            608 STORE_ATTR              14 (S_y)
                
-               125         618 LOAD_FAST                1 (shape_fn)
+               145         618 LOAD_FAST                1 (shape_fn)
                            620 LOAD_METHOD             15 (J)
                            642 LOAD_FAST                0 (self)
                            644 PRECALL                  1
                            648 CALL                     1
                            658 LOAD_FAST                0 (self)
                            660 STORE_ATTR              15 (J)
                
-               126         670 LOAD_FAST                1 (shape_fn)
+               146         670 LOAD_FAST                1 (shape_fn)
                            672 LOAD_METHOD             16 (I_w)
                            694 LOAD_FAST                0 (self)
                            696 PRECALL                  1
                            700 CALL                     1
                            710 LOAD_FAST                0 (self)
                            712 STORE_ATTR              16 (I_w)
                
-               128         722 LOAD_FAST                0 (self)
+               148         722 LOAD_FAST                0 (self)
                            724 LOAD_METHOD             17 (_Z_x)
                            746 PRECALL                  0
                            750 CALL                     0
                            760 LOAD_FAST                0 (self)
                            762 STORE_ATTR              18 (Z_x)
                
-               129         772 LOAD_FAST                0 (self)
+               149         772 LOAD_FAST                0 (self)
                            774 LOAD_METHOD             19 (_Z_y)
                            796 PRECALL                  0
                            800 CALL                     0
                            810 LOAD_FAST                0 (self)
                            812 STORE_ATTR              20 (Z_y)
                
-               130         822 LOAD_FAST                0 (self)
+               150         822 LOAD_FAST                0 (self)
                            824 LOAD_METHOD             21 (_r_x)
                            846 PRECALL                  0
                            850 CALL                     0
                            860 LOAD_FAST                0 (self)
                            862 STORE_ATTR              22 (r_x)
                
-               131         872 LOAD_FAST                0 (self)
+               151         872 LOAD_FAST                0 (self)
                            874 LOAD_METHOD             23 (_r_y)
                            896 PRECALL                  0
                            900 CALL                     0
                            910 LOAD_FAST                0 (self)
                            912 STORE_ATTR              24 (r_y)
                
-               134         922 LOAD_FAST                0 (self)
+               154         922 LOAD_FAST                0 (self)
                            924 LOAD_ATTR               25 (sig_figs)
                            934 POP_JUMP_FORWARD_IF_FALSE   187 (to 1310)
                
-               135         936 LOAD_GLOBAL             53 (NULL + list)
+               155         936 LOAD_GLOBAL             53 (NULL + list)
                            948 LOAD_FAST                0 (self)
                            950 LOAD_ATTR               27 (__dict__)
                            960 LOAD_METHOD             28 (items)
                            982 PRECALL                  0
                            986 CALL                     0
                            996 PRECALL                  1
                           1000 CALL                     1
                           1010 GET_ITER
                        >> 1012 FOR_ITER               150 (to 1314)
                           1014 UNPACK_SEQUENCE          2
                           1018 STORE_FAST               2 (k)
                           1020 STORE_FAST               3 (v)
                
-               136        1022 LOAD_GLOBAL             59 (NULL + isinstance)
+               156        1022 LOAD_GLOBAL             59 (NULL + isinstance)
                           1034 LOAD_FAST                3 (v)
                           1036 LOAD_GLOBAL             60 (float)
                           1048 LOAD_GLOBAL             62 (int)
                           1060 BUILD_TUPLE              2
                           1062 PRECALL                  2
                           1066 CALL                     2
                           1076 POP_JUMP_FORWARD_IF_FALSE   115 (to 1308)
@@ -816,17 +941,17 @@
                           1096 CALL                     1
                           1106 POP_JUMP_FORWARD_IF_TRUE   100 (to 1308)
                           1108 LOAD_FAST                3 (v)
                           1110 LOAD_CONST               9 (0)
                           1112 COMPARE_OP               3 (!=)
                           1118 POP_JUMP_FORWARD_IF_FALSE    94 (to 1308)
                
-               137        1120 LOAD_GLOBAL             67 (NULL + setattr)
+               157        1120 LOAD_GLOBAL             67 (NULL + setattr)
                
-               138        1132 LOAD_FAST                0 (self)
+               158        1132 LOAD_FAST                0 (self)
                           1134 LOAD_FAST                2 (k)
                           1136 LOAD_GLOBAL             69 (NULL + round)
                           1148 LOAD_FAST                3 (v)
                           1150 LOAD_FAST                0 (self)
                           1152 LOAD_ATTR               25 (sig_figs)
                           1162 LOAD_GLOBAL             63 (NULL + int)
                           1174 LOAD_GLOBAL             71 (NULL + floor)
@@ -843,23 +968,23 @@
                           1258 CALL                     1
                           1268 BINARY_OP               10 (-)
                           1272 LOAD_CONST              10 (1)
                           1274 BINARY_OP               10 (-)
                           1278 PRECALL                  2
                           1282 CALL                     2
                
-               137        1292 PRECALL                  3
+               157        1292 PRECALL                  3
                           1296 CALL                     3
                           1306 POP_TOP
                        >> 1308 JUMP_BACKWARD          149 (to 1012)
                
-               134     >> 1310 LOAD_CONST               0 (None)
+               154     >> 1310 LOAD_CONST               0 (None)
                           1312 RETURN_VALUE
                
-               135     >> 1314 LOAD_CONST               0 (None)
+               155     >> 1314 LOAD_CONST               0 (None)
                           1316 RETURN_VALUE
                consts
                   None
                   ('CHS',)
                   ('RHS', 'SHS')
                   ('WB', 'WC', 'UB', 'UC')
                   ('PFC',)
@@ -871,83 +996,83 @@
                   1
                names      ('sec_type', 'circularhollow', 'rectangularhollow', 'ishape', 'cshape', 'x_c', 'tshape', 'y_c', 'rectangleplate', 'NotImplementedError', 'A_g', 'I_x', 'I_y', 'S_x', 'S_y', 'J', 'I_w', '_Z_x', 'Z_x', '_Z_y', 'Z_y', '_r_x', 'r_x', '_r_y', 'r_y', 'sig_figs', 'list', '__dict__', 'items', 'isinstance', 'float', 'int', 'isnan', 'setattr', 'round', 'floor', 'log10', 'abs')
                varnames   ('self', 'shape_fn', 'k', 'v')
                freevars   ()
                cellvars   ()
                filename   'C:\\Users\\uqjgatta\\Documents\\GitHub\\steel-as\\src\\steelas\\member\\geometry.py'
                name       'solve_shape'
-               firstlineno 100
+               firstlineno 120
                lnotab
                   0x020112011001120110011201100112010e01360112010e013601120110
                   020c0114ff1004340134013401340134013401340232013201320132030e
                   01560162010c01a0ff12fd0401
             'return'
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 16777219
                code
                   0x97007c006a0000000000000000007c006a0100000000000000007a0b00
                   005300
-               141           0 RESUME                   0
+               161           0 RESUME                   0
                
-               142           2 LOAD_FAST                0 (self)
+               162           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (I_x)
                             14 LOAD_FAST                0 (self)
                             16 LOAD_ATTR                1 (y_max)
                             26 BINARY_OP               11 (/)
                             30 RETURN_VALUE
                consts
                   None
                names      ('I_x', 'y_max')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'C:\\Users\\uqjgatta\\Documents\\GitHub\\steel-as\\src\\steelas\\member\\geometry.py'
                name       '_Z_x'
-               firstlineno 141
+               firstlineno 161
                lnotab 0x0201
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 16777219
                code
                   0x97007c006a0000000000000000007c006a0100000000000000007a0b00
                   005300
-               144           0 RESUME                   0
+               164           0 RESUME                   0
                
-               145           2 LOAD_FAST                0 (self)
+               165           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (I_y)
                             14 LOAD_FAST                0 (self)
                             16 LOAD_ATTR                1 (x_max)
                             26 BINARY_OP               11 (/)
                             30 RETURN_VALUE
                consts
                   None
                names      ('I_y', 'x_max')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'C:\\Users\\uqjgatta\\Documents\\GitHub\\steel-as\\src\\steelas\\member\\geometry.py'
                name       '_Z_y'
-               firstlineno 144
+               firstlineno 164
                lnotab 0x0201
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 16777219
                code
                   0x97007c006a0000000000000000007c006a0100000000000000007a0b00
                   0064017a0800005300
-               147           0 RESUME                   0
+               167           0 RESUME                   0
                
-               148           2 LOAD_FAST                0 (self)
+               168           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (I_x)
                             14 LOAD_FAST                0 (self)
                             16 LOAD_ATTR                1 (A_g)
                             26 BINARY_OP               11 (/)
                             30 LOAD_CONST               1 (0.5)
                             32 BINARY_OP                8 (**)
                             36 RETURN_VALUE
@@ -956,27 +1081,27 @@
                   0.5
                names      ('I_x', 'A_g')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'C:\\Users\\uqjgatta\\Documents\\GitHub\\steel-as\\src\\steelas\\member\\geometry.py'
                name       '_r_x'
-               firstlineno 147
+               firstlineno 167
                lnotab 0x0201
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 16777219
                code
                   0x97007c006a0000000000000000007c006a0100000000000000007a0b00
                   0064017a0800005300
-               150           0 RESUME                   0
+               170           0 RESUME                   0
                
-               151           2 LOAD_FAST                0 (self)
+               171           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (I_y)
                             14 LOAD_FAST                0 (self)
                             16 LOAD_ATTR                1 (A_g)
                             26 BINARY_OP               11 (/)
                             30 LOAD_CONST               1 (0.5)
                             32 BINARY_OP                8 (**)
                             36 RETURN_VALUE
@@ -985,66 +1110,66 @@
                   0.5
                names      ('I_y', 'A_g')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'C:\\Users\\uqjgatta\\Documents\\GitHub\\steel-as\\src\\steelas\\member\\geometry.py'
                name       '_r_y'
-               firstlineno 150
+               firstlineno 170
                lnotab 0x0201
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 5
                flags     : 16777219
                code
                   0x97007c006a00000000000000000064017600720a7c006a010000000000
                   00000064027a0b000053007c006a00000000000000000064037600722c74
                   05000000000000000000006a0300000000000000007c00a6010000ab0100
                   000000000000007d017409000000000000000000007c017c006a05000000
                   00000000007c017a0a0000a6020000ab02000000000000000053007c006a
                   05000000000000000064027a0b00005300
-               153           0 RESUME                   0
+               173           0 RESUME                   0
                
-               157           2 LOAD_FAST                0 (self)
+               177           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (sec_type)
                             14 LOAD_CONST               1 (('CHS',))
                             16 CONTAINS_OP              0
                             18 POP_JUMP_FORWARD_IF_FALSE    10 (to 40)
                
-               158          20 LOAD_FAST                0 (self)
+               178          20 LOAD_FAST                0 (self)
                             22 LOAD_ATTR                1 (d)
                             32 LOAD_CONST               2 (2)
                             34 BINARY_OP               11 (/)
                             38 RETURN_VALUE
                
-               159     >>   40 LOAD_FAST                0 (self)
+               179     >>   40 LOAD_FAST                0 (self)
                             42 LOAD_ATTR                0 (sec_type)
                             52 LOAD_CONST               3 (('PFC',))
                             54 CONTAINS_OP              0
                             56 POP_JUMP_FORWARD_IF_FALSE    44 (to 146)
                
-               160          58 LOAD_GLOBAL              5 (NULL + cshape)
+               180          58 LOAD_GLOBAL              5 (NULL + cshape)
                             70 LOAD_ATTR                3 (x_c)
                             80 LOAD_FAST                0 (self)
                             82 PRECALL                  1
                             86 CALL                     1
                             96 STORE_FAST               1 (x_c)
                
-               161          98 LOAD_GLOBAL              9 (NULL + max)
+               181          98 LOAD_GLOBAL              9 (NULL + max)
                            110 LOAD_FAST                1 (x_c)
                            112 LOAD_FAST                0 (self)
                            114 LOAD_ATTR                5 (b)
                            124 LOAD_FAST                1 (x_c)
                            126 BINARY_OP               10 (-)
                            130 PRECALL                  2
                            134 CALL                     2
                            144 RETURN_VALUE
                
-               163     >>  146 LOAD_FAST                0 (self)
+               183     >>  146 LOAD_FAST                0 (self)
                            148 LOAD_ATTR                5 (b)
                            158 LOAD_CONST               2 (2)
                            160 BINARY_OP               11 (/)
                            164 RETURN_VALUE
                consts
                   None
                   ('CHS',)
@@ -1052,68 +1177,68 @@
                   ('PFC',)
                names      ('sec_type', 'd', 'cshape', 'x_c', 'max', 'b')
                varnames   ('self', 'x_c')
                freevars   ()
                cellvars   ()
                filename   'C:\\Users\\uqjgatta\\Documents\\GitHub\\steel-as\\src\\steelas\\member\\geometry.py'
                name       'x_max'
-               firstlineno 153
+               firstlineno 173
                lnotab 0x020412011401120128013002
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 5
                flags     : 16777219
                code
                   0x97007c006a00000000000000000064017600722c740300000000000000
                   0000006a0200000000000000007c00a6010000ab0100000000000000007d
                   017407000000000000000000007c017c006a0400000000000000007c017a
                   0a0000a6020000ab02000000000000000053007c006a0400000000000000
                   0064027a0b00005300
-               165           0 RESUME                   0
+               185           0 RESUME                   0
                
-               168           2 LOAD_FAST                0 (self)
+               188           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (sec_type)
                             14 LOAD_CONST               1 (('BT', 'CT'))
                             16 CONTAINS_OP              0
                             18 POP_JUMP_FORWARD_IF_FALSE    44 (to 108)
                
-               169          20 LOAD_GLOBAL              3 (NULL + tshape)
+               189          20 LOAD_GLOBAL              3 (NULL + tshape)
                             32 LOAD_ATTR                2 (y_c)
                             42 LOAD_FAST                0 (self)
                             44 PRECALL                  1
                             48 CALL                     1
                             58 STORE_FAST               1 (y_c)
                
-               170          60 LOAD_GLOBAL              7 (NULL + max)
+               190          60 LOAD_GLOBAL              7 (NULL + max)
                             72 LOAD_FAST                1 (y_c)
                             74 LOAD_FAST                0 (self)
                             76 LOAD_ATTR                4 (d)
                             86 LOAD_FAST                1 (y_c)
                             88 BINARY_OP               10 (-)
                             92 PRECALL                  2
                             96 CALL                     2
                            106 RETURN_VALUE
                
-               172     >>  108 LOAD_FAST                0 (self)
+               192     >>  108 LOAD_FAST                0 (self)
                            110 LOAD_ATTR                4 (d)
                            120 LOAD_CONST               2 (2)
                            122 BINARY_OP               11 (/)
                            126 RETURN_VALUE
                consts
                   None
                   ('BT', 'CT')
                   2
                names      ('sec_type', 'tshape', 'y_c', 'max', 'd')
                varnames   ('self', 'y_c')
                freevars   ()
                cellvars   ()
                filename   'C:\\Users\\uqjgatta\\Documents\\GitHub\\steel-as\\src\\steelas\\member\\geometry.py'
                name       'y_max'
-               firstlineno 165
+               firstlineno 185
                lnotab 0x0203120128013002
             code
                argcount  : 1
                nlocals   : 5
                stacksize : 6
                flags     : 16777227
                code
@@ -1121,72 +1246,72 @@
                   0000000000000000000000000000000000a6000000ab0000000000000000
                   0044005d265c0200007d037d047403000000000000000000007c027c03a6
                   020000ab02000000000000000072117405000000000000000000007c027c
                   037c04a6030000ab03000000000000000001008c27740700000000000000
                   0000007c026a040000000000000000a6010000ab01000000000000000072
                   147c02a0050000000000000000000000000000000000000000a6000000ab
                   00000000000000000001007c025300
-               174           0 RESUME                   0
+               194           0 RESUME                   0
                
-               176           2 PUSH_NULL
+               196           2 PUSH_NULL
                              4 LOAD_FAST                0 (cls)
                              6 PRECALL                  0
                             10 CALL                     0
                             20 STORE_FAST               2 (o)
                
-               178          22 LOAD_FAST                1 (kwargs)
+               198          22 LOAD_FAST                1 (kwargs)
                             24 LOAD_METHOD              0 (items)
                             46 PRECALL                  0
                             50 CALL                     0
                             60 GET_ITER
                        >>   62 FOR_ITER                38 (to 140)
                             64 UNPACK_SEQUENCE          2
                             68 STORE_FAST               3 (k)
                             70 STORE_FAST               4 (v)
                
-               180          72 LOAD_GLOBAL              3 (NULL + hasattr)
+               200          72 LOAD_GLOBAL              3 (NULL + hasattr)
                             84 LOAD_FAST                2 (o)
                             86 LOAD_FAST                3 (k)
                             88 PRECALL                  2
                             92 CALL                     2
                            102 POP_JUMP_FORWARD_IF_FALSE    17 (to 138)
                
-               181         104 LOAD_GLOBAL              5 (NULL + setattr)
+               201         104 LOAD_GLOBAL              5 (NULL + setattr)
                            116 LOAD_FAST                2 (o)
                            118 LOAD_FAST                3 (k)
                            120 LOAD_FAST                4 (v)
                            122 PRECALL                  3
                            126 CALL                     3
                            136 POP_TOP
                        >>  138 JUMP_BACKWARD           39 (to 62)
                
-               183     >>  140 LOAD_GLOBAL              7 (NULL + isnan)
+               203     >>  140 LOAD_GLOBAL              7 (NULL + isnan)
                            152 LOAD_FAST                2 (o)
                            154 LOAD_ATTR                4 (A_g)
                            164 PRECALL                  1
                            168 CALL                     1
                            178 POP_JUMP_FORWARD_IF_FALSE    20 (to 220)
                
-               185         180 LOAD_FAST                2 (o)
+               205         180 LOAD_FAST                2 (o)
                            182 LOAD_METHOD              5 (solve_shape)
                            204 PRECALL                  0
                            208 CALL                     0
                            218 POP_TOP
                
-               186     >>  220 LOAD_FAST                2 (o)
+               206     >>  220 LOAD_FAST                2 (o)
                            222 RETURN_VALUE
                consts
                   None
                names      ('items', 'hasattr', 'setattr', 'isnan', 'A_g', 'solve_shape')
                varnames   ('cls', 'kwargs', 'o', 'k', 'v')
                freevars   ()
                cellvars   ()
                filename   'C:\\Users\\uqjgatta\\Documents\\GitHub\\steel-as\\src\\steelas\\member\\geometry.py'
                name       'from_dict'
-               firstlineno 174
+               firstlineno 194
                lnotab 0x0202140232022001240228022801
             code
                argcount  : 1
                nlocals   : 3
                stacksize : 4
                flags     : 16777219
                code
@@ -1200,20 +1325,20 @@
                   020000000072016e0201006e15010001007c006a01000000000000000064
                   057c006a0200000000000000007a0500007a0a00007d016e457801780164
                   0a6b020000000072016e097801640b6b020000000072016e0201006e1501
                   0001007c006a01000000000000000064057c006a0300000000000000007a
                   0500007a0a00007d016e1f7801640c6b0200000000720901007c006a0100
                   000000000000007d016e107d02740900000000000000000000640da60100
                   00ab01000000000000000082017c015300
-               188           0 RESUME                   0
+               208           0 RESUME                   0
                
-               191           2 LOAD_FAST                0 (self)
+               211           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (sec_type)
                
-               192          14 COPY                     1
+               212          14 COPY                     1
                             16 COPY                     1
                             18 LOAD_CONST               1 ('UB')
                             20 COMPARE_OP               2 (==)
                             26 POP_JUMP_FORWARD_IF_FALSE     1 (to 30)
                             28 JUMP_FORWARD            23 (to 76)
                        >>   30 COPY                     1
                             32 LOAD_CONST               2 ('UC')
@@ -1231,25 +1356,25 @@
                             68 POP_JUMP_FORWARD_IF_FALSE     1 (to 72)
                             70 JUMP_FORWARD             2 (to 76)
                        >>   72 POP_TOP
                             74 JUMP_FORWARD            21 (to 118)
                        >>   76 POP_TOP
                             78 POP_TOP
                
-               195          80 LOAD_FAST                0 (self)
+               215          80 LOAD_FAST                0 (self)
                             82 LOAD_ATTR                1 (d)
                             92 LOAD_CONST               5 (2)
                             94 LOAD_FAST                0 (self)
                             96 LOAD_ATTR                2 (t_f)
                            106 BINARY_OP                5 (*)
                            110 BINARY_OP               10 (-)
                            114 STORE_FAST               1 (d)
                            116 JUMP_FORWARD           142 (to 402)
                
-               196     >>  118 COPY                     1
+               216     >>  118 COPY                     1
                            120 COPY                     1
                            122 LOAD_CONST               6 ('BT')
                            124 COMPARE_OP               2 (==)
                            130 POP_JUMP_FORWARD_IF_FALSE     1 (to 134)
                            132 JUMP_FORWARD             9 (to 152)
                        >>  134 COPY                     1
                            136 LOAD_CONST               7 ('CT')
@@ -1257,23 +1382,23 @@
                            144 POP_JUMP_FORWARD_IF_FALSE     1 (to 148)
                            146 JUMP_FORWARD             2 (to 152)
                        >>  148 POP_TOP
                            150 JUMP_FORWARD            18 (to 188)
                        >>  152 POP_TOP
                            154 POP_TOP
                
-               197         156 LOAD_FAST                0 (self)
+               217         156 LOAD_FAST                0 (self)
                            158 LOAD_ATTR                1 (d)
                            168 LOAD_FAST                0 (self)
                            170 LOAD_ATTR                2 (t_f)
                            180 BINARY_OP               10 (-)
                            184 STORE_FAST               1 (d)
                            186 JUMP_FORWARD           107 (to 402)
                
-               198     >>  188 COPY                     1
+               218     >>  188 COPY                     1
                            190 COPY                     1
                            192 LOAD_CONST               8 ('WB')
                            194 COMPARE_OP               2 (==)
                            200 POP_JUMP_FORWARD_IF_FALSE     1 (to 204)
                            202 JUMP_FORWARD             9 (to 222)
                        >>  204 COPY                     1
                            206 LOAD_CONST               9 ('WC')
@@ -1281,25 +1406,25 @@
                            214 POP_JUMP_FORWARD_IF_FALSE     1 (to 218)
                            216 JUMP_FORWARD             2 (to 222)
                        >>  218 POP_TOP
                            220 JUMP_FORWARD            21 (to 264)
                        >>  222 POP_TOP
                            224 POP_TOP
                
-               199         226 LOAD_FAST                0 (self)
+               219         226 LOAD_FAST                0 (self)
                            228 LOAD_ATTR                1 (d)
                            238 LOAD_CONST               5 (2)
                            240 LOAD_FAST                0 (self)
                            242 LOAD_ATTR                2 (t_f)
                            252 BINARY_OP                5 (*)
                            256 BINARY_OP               10 (-)
                            260 STORE_FAST               1 (d)
                            262 JUMP_FORWARD            69 (to 402)
                
-               200     >>  264 COPY                     1
+               220     >>  264 COPY                     1
                            266 COPY                     1
                            268 LOAD_CONST              10 ('SHS')
                            270 COMPARE_OP               2 (==)
                            276 POP_JUMP_FORWARD_IF_FALSE     1 (to 280)
                            278 JUMP_FORWARD             9 (to 298)
                        >>  280 COPY                     1
                            282 LOAD_CONST              11 ('RHS')
@@ -1307,44 +1432,44 @@
                            290 POP_JUMP_FORWARD_IF_FALSE     1 (to 294)
                            292 JUMP_FORWARD             2 (to 298)
                        >>  294 POP_TOP
                            296 JUMP_FORWARD            21 (to 340)
                        >>  298 POP_TOP
                            300 POP_TOP
                
-               201         302 LOAD_FAST                0 (self)
+               221         302 LOAD_FAST                0 (self)
                            304 LOAD_ATTR                1 (d)
                            314 LOAD_CONST               5 (2)
                            316 LOAD_FAST                0 (self)
                            318 LOAD_ATTR                3 (t)
                            328 BINARY_OP                5 (*)
                            332 BINARY_OP               10 (-)
                            336 STORE_FAST               1 (d)
                            338 JUMP_FORWARD            31 (to 402)
                
-               202     >>  340 COPY                     1
+               222     >>  340 COPY                     1
                            342 LOAD_CONST              12 ('RectPlate')
                            344 COMPARE_OP               2 (==)
                            350 POP_JUMP_FORWARD_IF_FALSE     9 (to 370)
                            352 POP_TOP
                
-               203         354 LOAD_FAST                0 (self)
+               223         354 LOAD_FAST                0 (self)
                            356 LOAD_ATTR                1 (d)
                            366 STORE_FAST               1 (d)
                            368 JUMP_FORWARD            16 (to 402)
                
-               204     >>  370 STORE_FAST               2 (other)
+               224     >>  370 STORE_FAST               2 (other)
                
-               205         372 LOAD_GLOBAL              9 (NULL + ValueError)
+               225         372 LOAD_GLOBAL              9 (NULL + ValueError)
                            384 LOAD_CONST              13 ('unknown section type')
                            386 PRECALL                  1
                            390 CALL                     1
                            400 RAISE_VARARGS            1
                
-               207     >>  402 LOAD_FAST                1 (d)
+               227     >>  402 LOAD_FAST                1 (d)
                            404 RETURN_VALUE
                consts
                   'clear depth between flanges for open sections, ignoring fillets or welds'
                   'UB'
                   'UC'
                   'PFC'
                   'TFB'
@@ -1359,15 +1484,15 @@
                   'unknown section type'
                names      ('sec_type', 'd', 't_f', 't', 'ValueError')
                varnames   ('self', 'd', 'other')
                freevars   ()
                cellvars   ()
                filename   'C:\\Users\\uqjgatta\\Documents\\GitHub\\steel-as\\src\\steelas\\member\\geometry.py'
                name       'd_1'
-               firstlineno 188
+               firstlineno 208
                lnotab 0x02030c01420326012601200126012601260126010e01100102011e02
             code
                argcount  : 1
                nlocals   : 3
                stacksize : 4
                flags     : 16777219
                code
@@ -1380,20 +1505,20 @@
                   006a0100000000000000007c006a0200000000000000007a0500007d016e
                   557801780164096b020000000072016e097801640a6b020000000072016e
                   0201006e1501000100640b7c006a0300000000000000007a0500007c006a
                   0400000000000000007a0500007d016e2f7801640c6b0200000000721101
                   007c006a0500000000000000007c006a0600000000000000007a0500007d
                   016e187d02740f00000000000000000000640d7c006a0000000000000000
                   009b009d02a6010000ab01000000000000000082017c015300
-               209           0 RESUME                   0
+               229           0 RESUME                   0
                
-               212           2 LOAD_FAST                0 (self)
+               232           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (sec_type)
                
-               213          14 COPY                     1
+               233          14 COPY                     1
                             16 COPY                     1
                             18 LOAD_CONST               1 ('UB')
                             20 COMPARE_OP               2 (==)
                             26 POP_JUMP_FORWARD_IF_FALSE     1 (to 30)
                             28 JUMP_FORWARD            37 (to 104)
                        >>   30 COPY                     1
                             32 LOAD_CONST               2 ('UC')
@@ -1421,23 +1546,23 @@
                             96 POP_JUMP_FORWARD_IF_FALSE     1 (to 100)
                             98 JUMP_FORWARD             2 (to 104)
                        >>  100 POP_TOP
                            102 JUMP_FORWARD            18 (to 140)
                        >>  104 POP_TOP
                            106 POP_TOP
                
-               214         108 LOAD_FAST                0 (self)
+               234         108 LOAD_FAST                0 (self)
                            110 LOAD_ATTR                1 (d_w)
                            120 LOAD_FAST                0 (self)
                            122 LOAD_ATTR                2 (t_w)
                            132 BINARY_OP                5 (*)
                            136 STORE_FAST               1 (a)
                            138 JUMP_FORWARD           120 (to 380)
                
-               215     >>  140 COPY                     1
+               235     >>  140 COPY                     1
                            142 COPY                     1
                            144 LOAD_CONST               7 ('BT')
                            146 COMPARE_OP               2 (==)
                            152 POP_JUMP_FORWARD_IF_FALSE     1 (to 156)
                            154 JUMP_FORWARD             9 (to 174)
                        >>  156 COPY                     1
                            158 LOAD_CONST               8 ('CT')
@@ -1445,23 +1570,23 @@
                            166 POP_JUMP_FORWARD_IF_FALSE     1 (to 170)
                            168 JUMP_FORWARD             2 (to 174)
                        >>  170 POP_TOP
                            172 JUMP_FORWARD            18 (to 210)
                        >>  174 POP_TOP
                            176 POP_TOP
                
-               219         178 LOAD_FAST                0 (self)
+               239         178 LOAD_FAST                0 (self)
                            180 LOAD_ATTR                1 (d_w)
                            190 LOAD_FAST                0 (self)
                            192 LOAD_ATTR                2 (t_w)
                            202 BINARY_OP                5 (*)
                            206 STORE_FAST               1 (a)
                            208 JUMP_FORWARD            85 (to 380)
                
-               220     >>  210 COPY                     1
+               240     >>  210 COPY                     1
                            212 COPY                     1
                            214 LOAD_CONST               9 ('SHS')
                            216 COMPARE_OP               2 (==)
                            222 POP_JUMP_FORWARD_IF_FALSE     1 (to 226)
                            224 JUMP_FORWARD             9 (to 244)
                        >>  226 COPY                     1
                            228 LOAD_CONST              10 ('RHS')
@@ -1469,53 +1594,53 @@
                            236 POP_JUMP_FORWARD_IF_FALSE     1 (to 240)
                            238 JUMP_FORWARD             2 (to 244)
                        >>  240 POP_TOP
                            242 JUMP_FORWARD            21 (to 286)
                        >>  244 POP_TOP
                            246 POP_TOP
                
-               221         248 LOAD_CONST              11 (2)
+               241         248 LOAD_CONST              11 (2)
                            250 LOAD_FAST                0 (self)
                            252 LOAD_ATTR                3 (d_p)
                            262 BINARY_OP                5 (*)
                            266 LOAD_FAST                0 (self)
                            268 LOAD_ATTR                4 (t)
                            278 BINARY_OP                5 (*)
                            282 STORE_FAST               1 (a)
                            284 JUMP_FORWARD            47 (to 380)
                
-               222     >>  286 COPY                     1
+               242     >>  286 COPY                     1
                            288 LOAD_CONST              12 ('RectPlate')
                            290 COMPARE_OP               2 (==)
                            296 POP_JUMP_FORWARD_IF_FALSE    17 (to 332)
                            298 POP_TOP
                
-               223         300 LOAD_FAST                0 (self)
+               243         300 LOAD_FAST                0 (self)
                            302 LOAD_ATTR                5 (d)
                            312 LOAD_FAST                0 (self)
                            314 LOAD_ATTR                6 (b)
                            324 BINARY_OP                5 (*)
                            328 STORE_FAST               1 (a)
                            330 JUMP_FORWARD            24 (to 380)
                
-               224     >>  332 STORE_FAST               2 (other)
+               244     >>  332 STORE_FAST               2 (other)
                
-               225         334 LOAD_GLOBAL             15 (NULL + NotImplementedError)
+               245         334 LOAD_GLOBAL             15 (NULL + NotImplementedError)
                
-               226         346 LOAD_CONST              13 ('A_w not implemented for section type ')
+               246         346 LOAD_CONST              13 ('A_w not implemented for section type ')
                            348 LOAD_FAST                0 (self)
                            350 LOAD_ATTR                0 (sec_type)
                            360 FORMAT_VALUE             0
                            362 BUILD_STRING             2
                
-               225         364 PRECALL                  1
+               245         364 PRECALL                  1
                            368 CALL                     1
                            378 RAISE_VARARGS            1
                
-               228     >>  380 LOAD_FAST                1 (a)
+               248     >>  380 LOAD_FAST                1 (a)
                            382 RETURN_VALUE
                consts
                   'area of web elements'
                   'UB'
                   'UC'
                   'WB'
                   'WC'
@@ -1530,15 +1655,15 @@
                   'A_w not implemented for section type '
                names      ('sec_type', 'd_w', 't_w', 'd_p', 't', 'd', 'b', 'NotImplementedError')
                varnames   ('self', 'a', 'other')
                freevars   ()
                cellvars   ()
                filename   'C:\\Users\\uqjgatta\\Documents\\GitHub\\steel-as\\src\\steelas\\member\\geometry.py'
                name       'A_w'
-               firstlineno 209
+               firstlineno 229
                lnotab 0x02030c015e01200126042001260126010e01200102010c0112ff1003
             code
                argcount  : 1
                nlocals   : 3
                stacksize : 4
                flags     : 16777219
                code
@@ -1551,20 +1676,20 @@
                   0164096b020000000072016e097801640a6b020000000072016e0201006e
                   0a010001007c006a0100000000000000007d016e4578017801640b6b0200
                   00000072016e097801640c6b020000000072016e0201006e15010001007c
                   006a01000000000000000064037c006a0300000000000000007a0500007a
                   0a00007d016e1f7801640d6b0200000000720901007c006a010000000000
                   0000007d016e107d02740900000000000000000000640ea6010000ab0100
                   0000000000000082017c015300
-               230           0 RESUME                   0
+               250           0 RESUME                   0
                
-               233           2 LOAD_FAST                0 (self)
+               253           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (sec_type)
                
-               234          14 COPY                     1
+               254          14 COPY                     1
                             16 COPY                     1
                             18 LOAD_CONST               1 ('RHS')
                             20 COMPARE_OP               2 (==)
                             26 POP_JUMP_FORWARD_IF_FALSE     1 (to 30)
                             28 JUMP_FORWARD             9 (to 48)
                        >>   30 COPY                     1
                             32 LOAD_CONST               2 ('SHS')
@@ -1572,36 +1697,36 @@
                             40 POP_JUMP_FORWARD_IF_FALSE     1 (to 44)
                             42 JUMP_FORWARD             2 (to 48)
                        >>   44 POP_TOP
                             46 JUMP_FORWARD            21 (to 90)
                        >>   48 POP_TOP
                             50 POP_TOP
                
-               235          52 LOAD_FAST                0 (self)
+               255          52 LOAD_FAST                0 (self)
                             54 LOAD_ATTR                1 (d)
                             64 LOAD_CONST               3 (2)
                             66 LOAD_FAST                0 (self)
                             68 LOAD_ATTR                2 (t)
                             78 BINARY_OP                5 (*)
                             82 BINARY_OP               10 (-)
                             86 STORE_FAST               1 (d)
                             88 JUMP_FORWARD           139 (to 368)
                
-               236     >>   90 COPY                     1
+               256     >>   90 COPY                     1
                             92 LOAD_CONST               4 ('CHS')
                             94 COMPARE_OP               2 (==)
                            100 POP_JUMP_FORWARD_IF_FALSE     9 (to 120)
                            102 POP_TOP
                
-               237         104 LOAD_FAST                0 (self)
+               257         104 LOAD_FAST                0 (self)
                            106 LOAD_ATTR                1 (d)
                            116 STORE_FAST               1 (d)
                            118 JUMP_FORWARD           124 (to 368)
                
-               238     >>  120 COPY                     1
+               258     >>  120 COPY                     1
                            122 COPY                     1
                            124 LOAD_CONST               5 ('UB')
                            126 COMPARE_OP               2 (==)
                            132 POP_JUMP_FORWARD_IF_FALSE     1 (to 136)
                            134 JUMP_FORWARD            37 (to 210)
                        >>  136 COPY                     1
                            138 LOAD_CONST               6 ('UC')
@@ -1629,20 +1754,20 @@
                            202 POP_JUMP_FORWARD_IF_FALSE     1 (to 206)
                            204 JUMP_FORWARD             2 (to 210)
                        >>  206 POP_TOP
                            208 JUMP_FORWARD            10 (to 230)
                        >>  210 POP_TOP
                            212 POP_TOP
                
-               239         214 LOAD_FAST                0 (self)
+               259         214 LOAD_FAST                0 (self)
                            216 LOAD_ATTR                1 (d)
                            226 STORE_FAST               1 (d)
                            228 JUMP_FORWARD            69 (to 368)
                
-               240     >>  230 COPY                     1
+               260     >>  230 COPY                     1
                            232 COPY                     1
                            234 LOAD_CONST              11 ('WB')
                            236 COMPARE_OP               2 (==)
                            242 POP_JUMP_FORWARD_IF_FALSE     1 (to 246)
                            244 JUMP_FORWARD             9 (to 264)
                        >>  246 COPY                     1
                            248 LOAD_CONST              12 ('WC')
@@ -1650,44 +1775,44 @@
                            256 POP_JUMP_FORWARD_IF_FALSE     1 (to 260)
                            258 JUMP_FORWARD             2 (to 264)
                        >>  260 POP_TOP
                            262 JUMP_FORWARD            21 (to 306)
                        >>  264 POP_TOP
                            266 POP_TOP
                
-               241         268 LOAD_FAST                0 (self)
+               261         268 LOAD_FAST                0 (self)
                            270 LOAD_ATTR                1 (d)
                            280 LOAD_CONST               3 (2)
                            282 LOAD_FAST                0 (self)
                            284 LOAD_ATTR                3 (t_f)
                            294 BINARY_OP                5 (*)
                            298 BINARY_OP               10 (-)
                            302 STORE_FAST               1 (d)
                            304 JUMP_FORWARD            31 (to 368)
                
-               242     >>  306 COPY                     1
+               262     >>  306 COPY                     1
                            308 LOAD_CONST              13 ('RectPlate')
                            310 COMPARE_OP               2 (==)
                            316 POP_JUMP_FORWARD_IF_FALSE     9 (to 336)
                            318 POP_TOP
                
-               243         320 LOAD_FAST                0 (self)
+               263         320 LOAD_FAST                0 (self)
                            322 LOAD_ATTR                1 (d)
                            332 STORE_FAST               1 (d)
                            334 JUMP_FORWARD            16 (to 368)
                
-               244     >>  336 STORE_FAST               2 (other)
+               264     >>  336 STORE_FAST               2 (other)
                
-               245         338 LOAD_GLOBAL              9 (NULL + ValueError)
+               265         338 LOAD_GLOBAL              9 (NULL + ValueError)
                            350 LOAD_CONST              14 ('unknown section type')
                            352 PRECALL                  1
                            356 CALL                     1
                            366 RAISE_VARARGS            1
                
-               246     >>  368 LOAD_FAST                1 (d)
+               266     >>  368 LOAD_FAST                1 (d)
                            370 RETURN_VALUE
                consts
                   'clear depth between flanges for RHS, SHS sections, ignoring radii'
                   'RHS'
                   'SHS'
                   2
                   'CHS'
@@ -1703,49 +1828,49 @@
                   'unknown section type'
                names      ('sec_type', 'd', 't', 't_f', 'ValueError')
                varnames   ('self', 'd', 'other')
                freevars   ()
                cellvars   ()
                filename   'C:\\Users\\uqjgatta\\Documents\\GitHub\\steel-as\\src\\steelas\\member\\geometry.py'
                name       'd_w'
-               firstlineno 230
+               firstlineno 250
                lnotab 0x02030c01260126010e0110015e011001260126010e01100102011e01
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 16777219
                code
                   0x97007c006a0000000000000000006401760072077c006a010000000000
                   00000053007c006a0200000000000000005300
-               248           0 RESUME                   0
+               268           0 RESUME                   0
                
-               251           2 LOAD_FAST                0 (self)
+               271           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (sec_type)
                             14 LOAD_CONST               1 (('UB', 'UC', 'PFC', 'TFB', 'WB', 'WC', 'BT', 'CT'))
                             16 CONTAINS_OP              0
                             18 POP_JUMP_FORWARD_IF_FALSE     7 (to 34)
                
-               252          20 LOAD_FAST                0 (self)
+               272          20 LOAD_FAST                0 (self)
                             22 LOAD_ATTR                1 (d_1)
                             32 RETURN_VALUE
                
-               254     >>   34 LOAD_FAST                0 (self)
+               274     >>   34 LOAD_FAST                0 (self)
                             36 LOAD_ATTR                2 (d_w)
                             46 RETURN_VALUE
                consts
                   'clear transverse dimension of a web panel'
                   ('UB', 'UC', 'PFC', 'TFB', 'WB', 'WC', 'BT', 'CT')
                names      ('sec_type', 'd_1', 'd_w')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'C:\\Users\\uqjgatta\\Documents\\GitHub\\steel-as\\src\\steelas\\member\\geometry.py'
                name       'd_p'
-               firstlineno 248
+               firstlineno 268
                lnotab 0x020312010e02
             code
                argcount  : 1
                nlocals   : 3
                stacksize : 4
                flags     : 16777219
                code
@@ -1757,20 +1882,20 @@
                   0164086b020000000072016e10780164096b020000000072016e09780164
                   0a6b020000000072016e0201006e15010001007c006a0100000000000000
                   007c006a0300000000000000007a0a000064037a0b00007d016e34780164
                   0b6b0200000000721401007c006a0100000000000000007c006a03000000
                   00000000007a0a000064037a0b00007d016e1a7801640c6b020000000072
                   040100640d7d016e107d02740900000000000000000000640ea6010000ab
                   01000000000000000082017c015300
-               256           0 RESUME                   0
+               276           0 RESUME                   0
                
-               259           2 LOAD_FAST                0 (self)
+               279           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (sec_type)
                
-               260          14 COPY                     1
+               280          14 COPY                     1
                             16 COPY                     1
                             18 LOAD_CONST               1 ('RHS')
                             20 COMPARE_OP               2 (==)
                             26 POP_JUMP_FORWARD_IF_FALSE     1 (to 30)
                             28 JUMP_FORWARD             9 (to 48)
                        >>   30 COPY                     1
                             32 LOAD_CONST               2 ('SHS')
@@ -1778,25 +1903,25 @@
                             40 POP_JUMP_FORWARD_IF_FALSE     1 (to 44)
                             42 JUMP_FORWARD             2 (to 48)
                        >>   44 POP_TOP
                             46 JUMP_FORWARD            21 (to 90)
                        >>   48 POP_TOP
                             50 POP_TOP
                
-               261          52 LOAD_FAST                0 (self)
+               281          52 LOAD_FAST                0 (self)
                             54 LOAD_ATTR                1 (b)
                             64 LOAD_CONST               3 (2)
                             66 LOAD_FAST                0 (self)
                             68 LOAD_ATTR                2 (t)
                             78 BINARY_OP                5 (*)
                             82 BINARY_OP               10 (-)
                             86 STORE_FAST               1 (d)
                             88 JUMP_FORWARD           125 (to 340)
                
-               262     >>   90 COPY                     1
+               282     >>   90 COPY                     1
                             92 COPY                     1
                             94 LOAD_CONST               4 ('UB')
                             96 COMPARE_OP               2 (==)
                            102 POP_JUMP_FORWARD_IF_FALSE     1 (to 106)
                            104 JUMP_FORWARD            44 (to 194)
                        >>  106 COPY                     1
                            108 LOAD_CONST               5 ('UC')
@@ -1829,59 +1954,59 @@
                            186 POP_JUMP_FORWARD_IF_FALSE     1 (to 190)
                            188 JUMP_FORWARD             2 (to 194)
                        >>  190 POP_TOP
                            192 JUMP_FORWARD            21 (to 236)
                        >>  194 POP_TOP
                            196 POP_TOP
                
-               263         198 LOAD_FAST                0 (self)
+               283         198 LOAD_FAST                0 (self)
                            200 LOAD_ATTR                1 (b)
                            210 LOAD_FAST                0 (self)
                            212 LOAD_ATTR                3 (t_w)
                            222 BINARY_OP               10 (-)
                            226 LOAD_CONST               3 (2)
                            228 BINARY_OP               11 (/)
                            232 STORE_FAST               1 (d)
                            234 JUMP_FORWARD            52 (to 340)
                
-               264     >>  236 COPY                     1
+               284     >>  236 COPY                     1
                            238 LOAD_CONST              11 ('PFC')
                            240 COMPARE_OP               2 (==)
                            246 POP_JUMP_FORWARD_IF_FALSE    20 (to 288)
                            248 POP_TOP
                
-               266         250 LOAD_FAST                0 (self)
+               286         250 LOAD_FAST                0 (self)
                            252 LOAD_ATTR                1 (b)
                            262 LOAD_FAST                0 (self)
                            264 LOAD_ATTR                3 (t_w)
                            274 BINARY_OP               10 (-)
                            278 LOAD_CONST               3 (2)
                            280 BINARY_OP               11 (/)
                            284 STORE_FAST               1 (d)
                            286 JUMP_FORWARD            26 (to 340)
                
-               267     >>  288 COPY                     1
+               287     >>  288 COPY                     1
                            290 LOAD_CONST              12 ('RectPlate')
                            292 COMPARE_OP               2 (==)
                            298 POP_JUMP_FORWARD_IF_FALSE     4 (to 308)
                            300 POP_TOP
                
-               268         302 LOAD_CONST              13 (0)
+               288         302 LOAD_CONST              13 (0)
                            304 STORE_FAST               1 (d)
                            306 JUMP_FORWARD            16 (to 340)
                
-               269     >>  308 STORE_FAST               2 (other)
+               289     >>  308 STORE_FAST               2 (other)
                
-               270         310 LOAD_GLOBAL              9 (NULL + ValueError)
+               290         310 LOAD_GLOBAL              9 (NULL + ValueError)
                            322 LOAD_CONST              14 ('unknown section type')
                            324 PRECALL                  1
                            328 CALL                     1
                            338 RAISE_VARARGS            1
                
-               271     >>  340 LOAD_FAST                1 (d)
+               291     >>  340 LOAD_FAST                1 (d)
                            342 RETURN_VALUE
                consts
                   'clear width of flange for steel sections'
                   'RHS'
                   'SHS'
                   2
                   'UB'
@@ -1897,15 +2022,15 @@
                   'unknown section type'
                names      ('sec_type', 'b', 't', 't_w', 'ValueError')
                varnames   ('self', 'd', 'other')
                freevars   ()
                cellvars   ()
                filename   'C:\\Users\\uqjgatta\\Documents\\GitHub\\steel-as\\src\\steelas\\member\\geometry.py'
                name       'b_ff'
-               firstlineno 256
+               firstlineno 276
                lnotab 0x02030c01260126016c0126010e0226010e01060102011e01
             code
                argcount  : 1
                nlocals   : 3
                stacksize : 5
                flags     : 16777219
                code
@@ -1926,20 +2051,20 @@
                   0000007c006a0100000000000000007c006a0200000000000000007a0a00
                   0064057a0800007a05000064057a0b00007a0000007d016e44740d000000
                   000000000000006407a6010000ab0100000000000000008201780164086b
                   0200000000721701007c006a0400000000000000007c006a070000000000
                   00000064057a0800007a05000064097a0b00007d016e187d027411000000
                   00000000000000640a7c006a0000000000000000009b009d02a6010000ab
                   01000000000000000082017c015300
-               273           0 RESUME                   0
+               293           0 RESUME                   0
                
-               275           2 LOAD_FAST                0 (self)
+               295           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (sec_type)
                
-               276          14 COPY                     1
+               296          14 COPY                     1
                             16 COPY                     1
                             18 LOAD_CONST               1 ('BT')
                             20 COMPARE_OP               2 (==)
                             26 POP_JUMP_FORWARD_IF_FALSE     1 (to 30)
                             28 JUMP_FORWARD             9 (to 48)
                        >>   30 COPY                     1
                             32 LOAD_CONST               2 ('CT')
@@ -1947,160 +2072,160 @@
                             40 POP_JUMP_FORWARD_IF_FALSE     1 (to 44)
                             42 JUMP_FORWARD             2 (to 48)
                        >>   44 POP_TOP
                             46 JUMP_FORWARD           228 (to 504)
                        >>   48 POP_TOP
                             50 POP_TOP
                
-               277          52 LOAD_FAST                0 (self)
+               297          52 LOAD_FAST                0 (self)
                             54 LOAD_ATTR                1 (y_c)
                             64 LOAD_FAST                0 (self)
                             66 LOAD_ATTR                2 (t_f)
                             76 LOAD_FAST                0 (self)
                             78 LOAD_ATTR                3 (r_1)
                             88 BINARY_OP                0 (+)
                             92 COMPARE_OP               5 (>=)
                             98 POP_JUMP_FORWARD_IF_FALSE   106 (to 312)
                
-               279         100 LOAD_FAST                0 (self)
+               299         100 LOAD_FAST                0 (self)
                            102 LOAD_ATTR                4 (b)
                            112 LOAD_FAST                0 (self)
                            114 LOAD_ATTR                2 (t_f)
                            124 BINARY_OP                5 (*)
                            128 LOAD_FAST                0 (self)
                            130 LOAD_ATTR                1 (y_c)
                            140 LOAD_CONST               3 (0.5)
                            142 LOAD_FAST                0 (self)
                            144 LOAD_ATTR                2 (t_f)
                            154 BINARY_OP                5 (*)
                            158 BINARY_OP               10 (-)
                            162 BINARY_OP                5 (*)
                
-               280         166 LOAD_CONST               4 (0.4292)
+               300         166 LOAD_CONST               4 (0.4292)
                
-               281         168 LOAD_FAST                0 (self)
+               301         168 LOAD_FAST                0 (self)
                            170 LOAD_ATTR                3 (r_1)
                            180 LOAD_CONST               5 (2)
                            182 BINARY_OP                8 (**)
                
-               280         186 BINARY_OP                5 (*)
+               300         186 BINARY_OP                5 (*)
                
-               282         190 LOAD_FAST                0 (self)
+               302         190 LOAD_FAST                0 (self)
                            192 LOAD_ATTR                1 (y_c)
                            202 LOAD_FAST                0 (self)
                            204 LOAD_ATTR                2 (t_f)
                            214 BINARY_OP               10 (-)
                            218 LOAD_CONST               6 (0.223)
                            220 LOAD_FAST                0 (self)
                            222 LOAD_ATTR                3 (r_1)
                            232 BINARY_OP                5 (*)
                            236 BINARY_OP               10 (-)
                
-               280         240 BINARY_OP                5 (*)
+               300         240 BINARY_OP                5 (*)
                
-               279         244 BINARY_OP                0 (+)
+               299         244 BINARY_OP                0 (+)
                
-               283         248 LOAD_FAST                0 (self)
+               303         248 LOAD_FAST                0 (self)
                            250 LOAD_ATTR                5 (t_w)
                            260 LOAD_FAST                0 (self)
                            262 LOAD_ATTR                1 (y_c)
                            272 LOAD_FAST                0 (self)
                            274 LOAD_ATTR                2 (t_f)
                            284 BINARY_OP               10 (-)
                            288 LOAD_CONST               5 (2)
                            290 BINARY_OP                8 (**)
                            294 BINARY_OP                5 (*)
                            298 LOAD_CONST               5 (2)
                            300 BINARY_OP               11 (/)
                
-               279         304 BINARY_OP                0 (+)
+               299         304 BINARY_OP                0 (+)
                
-               278         308 STORE_FAST               1 (q)
+               298         308 STORE_FAST               1 (q)
                            310 JUMP_FORWARD           149 (to 610)
                
-               285     >>  312 LOAD_FAST                0 (self)
+               305     >>  312 LOAD_FAST                0 (self)
                            314 LOAD_ATTR                1 (y_c)
                            324 LOAD_FAST                0 (self)
                            326 LOAD_ATTR                2 (t_f)
                            336 COMPARE_OP               5 (>=)
                            342 POP_JUMP_FORWARD_IF_FALSE    65 (to 474)
                
-               287         344 LOAD_FAST                0 (self)
+               307         344 LOAD_FAST                0 (self)
                            346 LOAD_ATTR                4 (b)
                            356 LOAD_FAST                0 (self)
                            358 LOAD_ATTR                2 (t_f)
                            368 BINARY_OP                5 (*)
                            372 LOAD_FAST                0 (self)
                            374 LOAD_ATTR                1 (y_c)
                            384 LOAD_CONST               3 (0.5)
                            386 LOAD_FAST                0 (self)
                            388 LOAD_ATTR                2 (t_f)
                            398 BINARY_OP                5 (*)
                            402 BINARY_OP               10 (-)
                            406 BINARY_OP                5 (*)
                
-               288         410 LOAD_FAST                0 (self)
+               308         410 LOAD_FAST                0 (self)
                            412 LOAD_ATTR                5 (t_w)
                            422 LOAD_FAST                0 (self)
                            424 LOAD_ATTR                1 (y_c)
                            434 LOAD_FAST                0 (self)
                            436 LOAD_ATTR                2 (t_f)
                            446 BINARY_OP               10 (-)
                            450 LOAD_CONST               5 (2)
                            452 BINARY_OP                8 (**)
                            456 BINARY_OP                5 (*)
                            460 LOAD_CONST               5 (2)
                            462 BINARY_OP               11 (/)
                
-               287         466 BINARY_OP                0 (+)
+               307         466 BINARY_OP                0 (+)
                
-               286         470 STORE_FAST               1 (q)
+               306         470 STORE_FAST               1 (q)
                            472 JUMP_FORWARD            68 (to 610)
                
-               293     >>  474 LOAD_GLOBAL             13 (NULL + NotImplementedError)
+               313     >>  474 LOAD_GLOBAL             13 (NULL + NotImplementedError)
                
-               294         486 LOAD_CONST               7 ('Q_c calculation for n.a. within flange of tee-section not implemented')
+               314         486 LOAD_CONST               7 ('Q_c calculation for n.a. within flange of tee-section not implemented')
                
-               293         488 PRECALL                  1
+               313         488 PRECALL                  1
                            492 CALL                     1
                            502 RAISE_VARARGS            1
                
-               299     >>  504 COPY                     1
+               319     >>  504 COPY                     1
                            506 LOAD_CONST               8 ('RectPlate')
                            508 COMPARE_OP               2 (==)
                            514 POP_JUMP_FORWARD_IF_FALSE    23 (to 562)
                            516 POP_TOP
                
-               300         518 LOAD_FAST                0 (self)
+               320         518 LOAD_FAST                0 (self)
                            520 LOAD_ATTR                4 (b)
                            530 LOAD_FAST                0 (self)
                            532 LOAD_ATTR                7 (d)
                            542 LOAD_CONST               5 (2)
                            544 BINARY_OP                8 (**)
                            548 BINARY_OP                5 (*)
                            552 LOAD_CONST               9 (8)
                            554 BINARY_OP               11 (/)
                            558 STORE_FAST               1 (q)
                            560 JUMP_FORWARD            24 (to 610)
                
-               301     >>  562 STORE_FAST               2 (other)
+               321     >>  562 STORE_FAST               2 (other)
                
-               302         564 LOAD_GLOBAL             17 (NULL + ValueError)
+               322         564 LOAD_GLOBAL             17 (NULL + ValueError)
                
-               303         576 LOAD_CONST              10 ('Q_c not implemented for section type ')
+               323         576 LOAD_CONST              10 ('Q_c not implemented for section type ')
                            578 LOAD_FAST                0 (self)
                            580 LOAD_ATTR                0 (sec_type)
                            590 FORMAT_VALUE             0
                            592 BUILD_STRING             2
                
-               302         594 PRECALL                  1
+               322         594 PRECALL                  1
                            598 CALL                     1
                            608 RAISE_VARARGS            1
                
-               305     >>  610 LOAD_FAST                1 (q)
+               325     >>  610 LOAD_FAST                1 (q)
                            612 RETURN_VALUE
                consts
                   None
                   'BT'
                   'CT'
                   0.5
                   0.4292
@@ -2112,15 +2237,15 @@
                   'Q_c not implemented for section type '
                names      ('sec_type', 'y_c', 't_f', 'r_1', 'b', 't_w', 'NotImplementedError', 'd', 'ValueError')
                varnames   ('self', 'q', 'other')
                freevars   ()
                cellvars   ()
                filename   'C:\\Users\\uqjgatta\\Documents\\GitHub\\steel-as\\src\\steelas\\member\\geometry.py'
                name       'Q_c'
-               firstlineno 273
+               firstlineno 293
                lnotab
                   0x02020c01260130024201020112ff040232fe04ff040438fc04ff040720
                   02420138ff04ff04070c0102ff10060e012c0102010c0112ff1003
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 4
@@ -2134,20 +2259,20 @@
                   00640a530078017801640b6b020000000072016e097801640c6b02000000
                   0072016e0201006e19010001007c006a0100000000000000007c006a0200
                   000000000000007a0500007c006a0300000000000000007a0b0000530078
                   01640d6b0200000000721801007c006a0100000000000000007c006a0400
                   000000000000007a0500007c006a0300000000000000007a0b000053007d
                   01740b00000000000000000000640e7c006a0000000000000000009b009d
                   02a6010000ab0100000000000000008201
-               307           0 RESUME                   0
+               327           0 RESUME                   0
                
-               309           2 LOAD_FAST                0 (self)
+               329           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (sec_type)
                
-               310          14 COPY                     1
+               330          14 COPY                     1
                             16 COPY                     1
                             18 LOAD_CONST               1 ('RHS')
                             20 COMPARE_OP               2 (==)
                             26 POP_JUMP_FORWARD_IF_FALSE     1 (to 30)
                             28 JUMP_FORWARD            58 (to 146)
                        >>   30 COPY                     1
                             32 LOAD_CONST               2 ('SHS')
@@ -2190,18 +2315,18 @@
                            138 POP_JUMP_FORWARD_IF_FALSE     1 (to 142)
                            140 JUMP_FORWARD             2 (to 146)
                        >>  142 POP_TOP
                            144 JUMP_FORWARD             4 (to 154)
                        >>  146 POP_TOP
                            148 POP_TOP
                
-               311         150 LOAD_CONST              10 (1.0)
+               331         150 LOAD_CONST              10 (1.0)
                            152 RETURN_VALUE
                
-               312     >>  154 COPY                     1
+               332     >>  154 COPY                     1
                            156 COPY                     1
                            158 LOAD_CONST              11 ('BT')
                            160 COMPARE_OP               2 (==)
                            166 POP_JUMP_FORWARD_IF_FALSE     1 (to 170)
                            168 JUMP_FORWARD             9 (to 188)
                        >>  170 COPY                     1
                            172 LOAD_CONST              12 ('CT')
@@ -2209,51 +2334,51 @@
                            180 POP_JUMP_FORWARD_IF_FALSE     1 (to 184)
                            182 JUMP_FORWARD             2 (to 188)
                        >>  184 POP_TOP
                            186 JUMP_FORWARD            25 (to 238)
                        >>  188 POP_TOP
                            190 POP_TOP
                
-               313         192 LOAD_FAST                0 (self)
+               333         192 LOAD_FAST                0 (self)
                            194 LOAD_ATTR                1 (Q_c)
                            204 LOAD_FAST                0 (self)
                            206 LOAD_ATTR                2 (d_1)
                            216 BINARY_OP                5 (*)
                            220 LOAD_FAST                0 (self)
                            222 LOAD_ATTR                3 (I_x)
                            232 BINARY_OP               11 (/)
                            236 RETURN_VALUE
                
-               314     >>  238 COPY                     1
+               334     >>  238 COPY                     1
                            240 LOAD_CONST              13 ('RectPlate')
                            242 COMPARE_OP               2 (==)
                            248 POP_JUMP_FORWARD_IF_FALSE    24 (to 298)
                            250 POP_TOP
                
-               316         252 LOAD_FAST                0 (self)
+               336         252 LOAD_FAST                0 (self)
                            254 LOAD_ATTR                1 (Q_c)
                            264 LOAD_FAST                0 (self)
                            266 LOAD_ATTR                4 (d)
                            276 BINARY_OP                5 (*)
                            280 LOAD_FAST                0 (self)
                            282 LOAD_ATTR                3 (I_x)
                            292 BINARY_OP               11 (/)
                            296 RETURN_VALUE
                
-               318     >>  298 STORE_FAST               1 (other)
+               338     >>  298 STORE_FAST               1 (other)
                
-               319         300 LOAD_GLOBAL             11 (NULL + ValueError)
+               339         300 LOAD_GLOBAL             11 (NULL + ValueError)
                
-               320         312 LOAD_CONST              14 ('unknown shear stress distribution for section type ')
+               340         312 LOAD_CONST              14 ('unknown shear stress distribution for section type ')
                            314 LOAD_FAST                0 (self)
                            316 LOAD_ATTR                0 (sec_type)
                            326 FORMAT_VALUE             0
                            328 BUILD_STRING             2
                
-               319         330 PRECALL                  1
+               339         330 PRECALL                  1
                            334 CALL                     1
                            344 RAISE_VARARGS            1
                consts
                   None
                   'RHS'
                   'SHS'
                   'UB'
@@ -2270,33 +2395,33 @@
                   'unknown shear stress distribution for section type '
                names      ('sec_type', 'Q_c', 'd_1', 'I_x', 'd', 'ValueError')
                varnames   ('self', 'other')
                freevars   ()
                cellvars   ()
                filename   'C:\\Users\\uqjgatta\\Documents\\GitHub\\steel-as\\src\\steelas\\member\\geometry.py'
                name       'shear_stress_uniformity'
-               firstlineno 307
+               firstlineno 327
                lnotab 0x02020c018801040126012e010e022e0202010c0112ff
             None
             ('return', 'float')
-         names      ('__name__', '__module__', '__qualname__', '__doc__', 'name', '__annotations__', 'section', 'sec_type', 'np', 'nan', 'd', 'b', 't_f', 't_w', 't', 'r_1', 'r_2', 'alpha', 'r_o', 'A_g', 'I_x', 'I_y', 'S_x', 'S_y', 'Z_x', 'Z_y', 'r_x', 'r_y', 'I_w', 'J', 'x_c', 'y_c', 'field', 'sig_figs', '__post_init__', 'solve_shape', '_Z_x', '_Z_y', '_r_x', '_r_y', 'property', 'x_max', 'y_max', 'classmethod', 'from_dict', 'd_1', 'A_w', 'd_w', 'd_p', 'b_ff', 'Q_c', 'shear_stress_uniformity')
+         names      ('__name__', '__module__', '__qualname__', '__doc__', 'name', '__annotations__', 'section', 'sec_type', 'np', 'nan', 'd', 'b', 't_f', 't_w', 't', 'r_1', 'r_2', 'alpha', 'r_o', 'A_g', 'I_x', 'I_y', 'S_x', 'S_y', 'Z_x', 'Z_y', 'r_x', 'r_y', 'I_w', 'J', 'x_c', 'y_c', 'field', 'sig_figs', '__post_init__', 'report', 'solve_shape', '_Z_x', '_Z_y', '_r_x', '_r_y', 'property', 'x_max', 'y_max', 'classmethod', 'from_dict', 'd_1', 'A_w', 'd_w', 'd_p', 'b_ff', 'Q_c', 'shear_stress_uniformity')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'C:\\Users\\uqjgatta\\Documents\\GitHub\\steel-as\\src\\steelas\\member\\geometry.py'
          name       'SectionGeometry'
-         firstlineno 39
+         firstlineno 55
          lnotab
-            0x0c0204170e010e010e0218011801180118011801180118011801180218
+            0x0c0204180e010e010e0218011801180118011801180118011801180218
             0118011801180118011801180118011801180118020e010e032402060406
-            290803080308030803020104ff0e01020b020104ff0e010208020104ff0e
-            01020d020104ff0e010214020106ff0e010214020104ff0e010211020104
-            ff0e010207020104ff0e010210020106ff0e010221020106ff0e01
+            0306290803080308030803020104ff0e01020b020104ff0e010208020104
+            ff0e01020d020104ff0e010214020106ff0e010214020104ff0e01021102
+            0104ff0e010207020104ff0e010210020106ff0e010221020106ff0e01
       'SectionGeometry'
-   names      ('__doc__', '__future__', 'annotations', 'math', 'floor', 'log10', 'isnan', 'dataclasses', 'dataclass', 'field', 'numpy', 'np', 'steelas.shape', 'circularhollow', 'rectangularhollow', 'ishape', 'cshape', 'tshape', 'rectangleplate', 'SectionGeometry')
+   names      ('__doc__', '__future__', 'annotations', 'math', 'floor', 'log10', 'isnan', 'dataclasses', 'dataclass', 'field', 'enum', 'StrEnum', 'numpy', 'np', 'steelas.shape', 'circularhollow', 'rectangularhollow', 'ishape', 'cshape', 'tshape', 'rectangleplate', 'steelas.data.io', 'report', 'SectionType', 'SectionGeometry')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   'C:\\Users\\uqjgatta\\Documents\\GitHub\\steel-as\\src\\steelas\\member\\geometry.py'
    name       '<module>'
    firstlineno 1
-   lnotab 0x00ff0203040c0c021401100108022012160118ff0e01
+   lnotab 0x00ff0203040c0c02140110010c01080220090c031c15160118ff0e01
```

### Comparing `steelas-0.1.2/src/steelas/member/__pycache__/material.cpython-310.pyc` & `steelas-0.2.0/src/steelas/member/__pycache__/material.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `steelas-0.1.2/src/steelas/member/__pycache__/member.cpython-310.pyc` & `steelas-0.2.0/src/steelas/member/__pycache__/member.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `steelas-0.1.2/src/steelas/member/__pycache__/slenderness.cpython-310.pyc` & `steelas-0.2.0/src/steelas/member/__pycache__/slenderness.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `steelas-0.1.2/src/steelas/member/geometry.py` & `steelas-0.2.0/src/steelas/member/geometry.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,53 +1,69 @@
 # -*- coding: utf-8 -*-
 
 """
 This module provides classes and functions to manage steel sections and their geometric properties.
 
-Classes:    
-    SectionGeometry: TODO. 
+Classes:
+    SectionGeometry: TODO.
 
 Functions:
     import_section_library(): Returns a DataFrame containing the section library defined
     in steelas/data/
 
 """
 
 from __future__ import annotations
 
 from math import floor, log10, isnan
 from dataclasses import dataclass, field
+from enum import StrEnum
 import numpy as np
 
 from steelas.shape import (
     circularhollow,
     rectangularhollow,
     ishape,
     cshape,
     tshape,
     rectangleplate,
 )
 
+from steelas.data.io import report
+
+
+class SectionType(StrEnum):
+    CHS = "CHS"
+    RHS = "RHS"
+    SHS = "SHS"
+    WB = "WB"
+    UB = "UB"
+    UC = "UC"
+    PFC = "PFC"
+    BT = "BT"
+    CT = "CT"
+    RectPlate = "RectPlate"
+
 
 # list section property keys
 # open_section_keys = ['d', 'b', 't_f', 't_w', 'r']
 # tfb_keys = ['d', 'b', 't_f', 't_w', 'r_r', 'r_f', 'alpha']
 # rhs_keys = ['d', 'b', 't', 'r_out']
 # chs_keys = ['d', 't']
 # plate_keys = ['b', 'd']
 
 
 @dataclass(kw_only=True)
 class SectionGeometry:
     """
     Represents the geometric properties of a structural section.
 
-    This class encapsulates the geometric dimensions and derived properties of various structural section types, 
-    such as I-shapes (WB, WC, UB, UC), Channels (PFC), Hollow Sections (RHS, SHS, CHS), and Plates. It provides 
-    functionality to calculate sectional properties based on the specified geometry, including area, moment of 
+    This class encapsulates the geometric dimensions and derived properties of various structural section types,
+    such as I-shapes (WB, WC, UB, UC), Channels (PFC), Hollow Sections (RHS, SHS, CHS), and Plates. It provides
+    functionality to calculate sectional properties based on the specified geometry, including area, moment of
     inertia, section modulus, and radius of gyration, among others.
 
     Attributes:
         name (str): A descriptive name for the section.
         section (str): The specific section designation.
         sec_type (str): The type of section (e.g., CHS, RHS, UB).
         d, b, t_f, t_w, t, r_1, r_2, alpha, r_o: Geometric dimensions of the section.
@@ -57,14 +73,15 @@
         Z_x, Z_y (float): Plastic section modulus about the x-axis and y-axis, respectively.
         r_x, r_y (float): Radius of gyration about the x-axis and y-axis, respectively.
         I_w (float): Warping constant.
         J (float): Torsional constant.
         x_c, y_c (float): Coordinates of the centroid, default to 0.
         sig_figs (int): Number of significant figures for rounding calculations, defaults to 4.
     """
+
     name: str = ""
     section: str = ""
     sec_type: str = ""
 
     d: float = np.nan
     b: float = np.nan
     t_f: float = np.nan
@@ -93,14 +110,17 @@
     # round values to a number of significant figures
     sig_figs: int = field(repr=False, default=4)
 
     def __post_init__(self):
         if self.sec_type != "":
             self.solve_shape()
 
+    def report(self, **kwargs):
+        return report(self, **kwargs)
+
     def solve_shape(self):
         if self.sec_type in ["CHS"]:
             shape_fn = circularhollow
         elif self.sec_type in ["RHS", "SHS"]:
             shape_fn = rectangularhollow
         elif self.sec_type in ["WB", "WC", "UB", "UC"]:
             shape_fn = ishape
```

### Comparing `steelas-0.1.2/src/steelas/member/material.py` & `steelas-0.2.0/src/steelas/member/material.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,14 +3,41 @@
 """
 
 import numpy as np
 from math import isnan
 from dataclasses import dataclass
 from typing import Callable
 
+from steelas.data.io import report
+
+from enum import StrEnum
+
+
+class SteelMaterialType(StrEnum):
+    HotRolledSection = "HotRolledSection"
+    HollowSection = "HollowSection"
+    HotRolledPlate = "HotRolledPlate"
+    WeldedSection = "WeldedSection"
+
+
+class SteelGrade(StrEnum):
+    C450 = "C450"
+    C350 = "C350"
+    C250 = "C250"
+    GR450 = "GR450"
+    GR400 = "GR400"
+    GR350 = "GR350"
+    GR300 = "GR300"
+    WR350 = "WR350"
+    GR250 = "GR250"
+    GR200 = "GR200"
+    PR500 = "PR500"
+    PR600 = "PR600"
+    PR700 = "PR700"
+
 
 @dataclass(kw_only=True)
 class SteelMaterial:
     """
     Represents the material properties of steel used in structural engineering design.
 
     This class encapsulates the essential characteristics and mechanical properties of steel materials,
@@ -27,17 +54,18 @@
         f_u (float): Tensile strength used in design, dynamically calculated.
         res_stress (str): Designator for the type of residual stress category, e.g., 'HR' for hot-rolled.
         t (float): Plate thickness, applicable for closed sections.
         t_f (float): Flange thickness, applicable for open sections.
         t_w (float): Web thickness, applicable for open sections.
         f_yw (float): Web yield stress, dynamically calculated based on web thickness.
     """
-    grade: str = "GR300"
-    mat_type: str = "HotRolledSection"
+
     name: str = ""
+    grade: str | SteelGrade = "GR300"
+    mat_type: str | SteelMaterialType = "HotRolledSection"
     f_y: float = 0  # yield stress used in design
     f_u: float = 0  # tensile strength used in design
 
     res_stress: str = "HR"
 
     # attr for closed sections
     t: float = np.nan  # plate thickness
@@ -57,19 +85,22 @@
             self.f_y = self._f_y(self.t_f)
         if not isnan(self.t_w):
             self.f_yw = self._f_y(self.t_w)
 
         self.f_u = self._f_u()
         self.res_stress = self._res_stress()
 
+    def report(self, **kwargs):
+        return report(self, **kwargs)
+
     @property
     def density(self) -> int:
         """Density of Steel, kg/m^3"""
         return 7850
-    
+
     @property
     def E(self) -> int:
         """Modulus of Elasticity, AS4100 Cl 2.2.4"""
         return 200000
 
     @property
     def G(self) -> int:
```

### Comparing `steelas-0.1.2/src/steelas/member/member.py` & `steelas-0.2.0/src/steelas/member/member.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,39 +2,47 @@
 # Script to calculate the capacity of few different steel sections
 
 # for pi in member buckling
 import numpy as np
 from dataclasses import dataclass, field
 from math import isnan, floor, log10
 
-
+from steelas.data.io import get_section_from_library, MemberLibrary
 from steelas.member.material import SteelMaterial
 from steelas.member.geometry import SectionGeometry
 from steelas.member.slenderness import SteelSlenderness
+from steelas.data.io import report
 
 
 def reference_buckling_moment(section: SteelSection, l_eb: int) -> float:
-    if section.sec_type in ['UB', 'UC', 'WB', 'WC', 'PFC']:
+    if section.sec_type in ["UB", "UC", "WB", "WC", "PFC"]:
         # AS4100 Cl5.6.1.1 open section with equal flanges
         # Eq 5.6.1.1(3)
-        M_o = ((np.pi**2 * section.mat.E * section.geom.I_y/l_eb**2) *
-               (section.mat.G*section.geom.J + (np.pi**2 * section.mat.E * section.geom.I_w/l_eb**2)))**0.5
-    elif section.sec_type in ['RHS', 'SHS', 'CHS']:
+        M_o = (
+            (np.pi**2 * section.mat.E * section.geom.I_y / l_eb**2)
+            * (
+                section.mat.G * section.geom.J
+                + (np.pi**2 * section.mat.E * section.geom.I_w / l_eb**2)
+            )
+        ) ** 0.5
+    elif section.sec_type in ["RHS", "SHS", "CHS"]:
         # AS4100 Cl5.6.1.4 hollow sections, I_w = 0 #NOTE - THIS IS SAME FORMULA AS ABOVE BUT WITH I_w =0
-        M_o = ((np.pi**2 * section.mat.E * section.geom.I_y/l_eb**2) *
-               (section.mat.G*section.geom.J))**0.5
+        M_o = (
+            (np.pi**2 * section.mat.E * section.geom.I_y / l_eb**2)
+            * (section.mat.G * section.geom.J)
+        ) ** 0.5
     else:
         raise NotImplementedError
         # angle sections Cl 5.6.1.3
-    #Nmm_to_kn_m = 1/1e6
+    # Nmm_to_kn_m = 1/1e6
     return M_o  # * Nmm_to_kn_m
 
 
 @dataclass(kw_only=True)
-class SteelSection():
+class SteelSection:
     geom: SectionGeometry | dict
     mat: SteelMaterial | dict
     slenderness: SteelSlenderness | dict | None
 
     # TODO solve steel slenderness if not provided?
     def __post_init__(self):
         if type(self.geom) is dict:
@@ -44,102 +52,146 @@
         if type(self.slenderness) is dict:
             self.slenderness = SteelSlenderness.from_dict(**self.slenderness)
 
         if self.slenderness is None:
             self.slenderness = SteelSlenderness(geom=self.geom, mat=self.mat)
         self.slenderness.geom = self.geom
         self.slenderness.mat = self.mat
+
+    def report(self, **kwargs) -> None:
+        report(self.geom, **kwargs)
+        report(self.mat, **kwargs)
+        report(
+            self.slenderness,
+            exclude_attribute_names=[
+                "geom",
+                "mat",
+                "components_x",
+                "components_y",
+                "components_c",
+            ],
+            **kwargs,
+        )
+
     # ----------------
     # Geometry Attrs
     # ----------------
     @property
-    def sec_type(self): return self.geom.sec_type
+    def sec_type(self):
+        return self.geom.sec_type
 
     @property
-    def A_g(self): return self.geom.A_g
+    def A_g(self):
+        return self.geom.A_g
 
     @property
     def A_n(self):
         return self._A_n()
 
     def _A_n(self):
         return self.geom.A_g
 
     @property
-    def A_w(self): return self.geom.A_w
+    def A_w(self):
+        return self.geom.A_w
 
     @property
-    def r_x(self): return self.geom.r_x
+    def r_x(self):
+        return self.geom.r_x
 
     @property
-    def r_y(self): return self.geom.r_y
+    def r_y(self):
+        return self.geom.r_y
 
     # ----------------
     # Material Attrs
     # ----------------
     #  f_u f_y f_yw k_f
     @property
-    def f_u(self): return self.mat.f_u
+    def f_u(self):
+        return self.mat.f_u
 
     @property
-    def f_y(self): return self.mat.f_y
+    def f_y(self):
+        return self.mat.f_y
 
     @property
-    def f_yw(self): return self.mat.f_yw
+    def f_yw(self):
+        return self.mat.f_yw
 
-    @property
-    def k_f(self): return self.mat.k_f
+    # @property
+    # def k_f(self):
+    #     return self.mat.k_f
 
     # ----------------
     # Slenderness Attrs
     # ----------------
     # Z_ex Z_ey k_f alpha_b web_shear_yield_governs alpha_v
 
     @property
-    def section_name(self): return self.slenderness.section
+    def section_name(self):
+        return self.slenderness.section
 
     @property
-    def material_name(self): return self.slenderness.grade
+    def material_name(self):
+        return self.slenderness.grade
 
     @property
-    def Z_ex(self): return self.slenderness.Z_ex
+    def Z_ex(self):
+        return self.slenderness.Z_ex
 
     @property
-    def Z_ey(self): return self.slenderness.Z_ey
+    def Z_ey(self):
+        return self.slenderness.Z_ey
 
     @property
-    def k_f(self): return self.slenderness.k_f
+    def k_f(self):
+        return self.slenderness.k_f
 
     @property
-    def alpha_b(self): return self.slenderness.alpha_b
+    def alpha_b(self):
+        return self.slenderness.alpha_b
 
     @property
-    def web_shear_yield_governs(
-        self): return self.slenderness.web_shear_yield_governs
+    def web_shear_yield_governs(self):
+        return self.slenderness.web_shear_yield_governs
 
     @property
-    def alpha_v(self): return self.slenderness.alpha_v
+    def alpha_v(self):
+        return self.slenderness.alpha_v
 
     @property
-    def shear_stress_uniformity(self): return self.geom.shear_stress_uniformity
+    def shear_stress_uniformity(self):
+        return self.geom.shear_stress_uniformity
+
+    @classmethod
+    def from_library(
+        cls, library: MemberLibrary, lookup_val: str, lookup_col: str = "name"
+    ) -> SteelSection:
+        section_dict = get_section_from_library(
+            library, lookup_val=lookup_val, lookup_col=lookup_col
+        )
+        return cls.from_section_dict(section_dict)
+
+    """creates a new SteelSection from library import"""
 
     @classmethod
     def from_section_dict(cls, section_dict: dict):
-        '''builds geometry, material, and section classes from section_dict'''
+        """builds geometry, material, and section classes from section_dict"""
         geom = SectionGeometry.from_dict(**section_dict)
         mat = SteelMaterial.from_dict(**section_dict)
         return cls(geom=geom, mat=mat, slenderness=None)
 
 
 @dataclass
-class SteelMember():
+class SteelMember:
     section: SteelSection  # includes geom and material and slenderness attrs
-    name: str = field(init=False, default='')
-    section_name: str = ''  # temp
-    material_name: str = ''  # temp
+    name: str = field(init=False, default="")
+    section_name: str = ""  # temp
+    material_name: str = ""  # temp
     l_ex: float = 0
     l_ey: float = 0
     l_eb: float = 0
 
     end_i_restraint: bool = True  # True if end is full or partially restraint
     end_j_restraint: bool = True  # True if end is full or partially restraint
 
@@ -172,19 +224,18 @@
     phiM_x: float = 0
     phiM_y: float = 0
 
     # round values to a number of significant figures
     sig_figs: int = 3
 
     def __post_init__(self):
-        N_to_kN = 1/1e3
-        Nmm_to_kn_m = 1/1e6
+        N_to_kN = 1 / 1e3
+        Nmm_to_kn_m = 1 / 1e6
 
-        self.name = self.section.section_name + \
-            ' (' + self.section.material_name + ')'
+        self.name = self.section.section_name + " (" + self.section.material_name + ")"
 
         self.section_name = self.section.section_name
         self.material_name = self.section.material_name
 
         self.M_sx = self._M_sx() * Nmm_to_kn_m
         self.M_bx = self._M_bx() * Nmm_to_kn_m
         self.M_sy = self._M_sy() * Nmm_to_kn_m
@@ -197,264 +248,296 @@
 
         self.N_t = self._N_t() * N_to_kN
 
         self.phiN_s = self.phi * self.N_s
         self.phiN_t = self.phi * self.N_t
         self.phiV_v = self.phi * self.V_v
         self.phiM_bx = self.phi * min(self.M_bx, self.M_sx)
-        #self.phiM_bx = self.phi * self.M_bx
+        # self.phiM_bx = self.phi * self.M_bx
         self.phiM_y = self.phi * self.M_sy
         self.phiM_sx = self.phi * self.M_sx
         self.phiM_sy = self.phi * self.M_sy
 
         self.phiN_c = self.phi * min(self.N_s, self.N_cx, self.N_cy)
 
         # round to sig figs
         if self.sig_figs:
             for k, v in list(self.__dict__.items()):
                 if isinstance(v, (float, int)) and (not isnan(v)) and (v != 0):
-                    setattr(self, k, round(v, self.sig_figs -
-                            int(floor(log10(abs(v))))-1))
+                    setattr(
+                        self, k, round(v, self.sig_figs - int(floor(log10(abs(v)))) - 1)
+                    )
+
+    def report(self, **kwargs) -> None:
+        report(self, exclude_attribute_names=["section"], **kwargs)
 
     # ------------------------------------------------------------------------
     # AS4100 Section 5 Members Subject to Bending ----------------------------
     # ------------------------------------------------------------------------
 
     def _M_sx(self) -> float:
-        '''AS4100 Cl 5.2.1 Ms nominal section moment capacity'''
+        """AS4100 Cl 5.2.1 Ms nominal section moment capacity"""
         return self.section.Z_ex * self.section.f_y
 
     def _M_sy(self) -> float:
-        '''AS4100 Cl 5.2.1 Ms nominal section moment capacity'''
+        """AS4100 Cl 5.2.1 Ms nominal section moment capacity"""
         return self.section.Z_ey * self.section.f_y
 
     def _M_bx(self) -> float:
-        '''AS4100 Cl 5.6, member capacity of segments without full lateral restraint'''
+        """AS4100 Cl 5.6, member capacity of segments without full lateral restraint"""
         if self.l_eb > 0:
             if self.end_i_restraint and self.end_j_restraint:
                 # AS4100 Cl 5.6.1 boths ends are fully or partially restrained
                 return min(self.alpha_m * self.alpha_sx * self._M_sx(), self._M_sx())
             elif self.end_i_restraint or self.end_j_restraint:
                 # AS4100 Cl 5.6.2 only one end is fully or partially restrained
                 raise NotImplementedError
                 # return min(self.alpha_sx * self.M_sx, self.M_sx)
             else:
-                raise ValueError('both ends are unrestrained')
+                raise ValueError("both ends are unrestrained")
         else:
             return self._M_sx()
 
     # @property
     def alpha_s(self, M_s: float, M_oa: float) -> float:
-        '''AS4100 Cl 5.6.1.1(iv) slenderness reduction factor, section of constant cross-section'''
-        return 0.6 * (((M_s/M_oa)**2 + 3)**0.5 - M_s/M_oa)
+        """AS4100 Cl 5.6.1.1(iv) slenderness reduction factor, section of constant cross-section"""
+        return 0.6 * (((M_s / M_oa) ** 2 + 3) ** 0.5 - M_s / M_oa)
         # return slenderness_reduction_factor(self.section, M_s, M_oa)
 
     @property
     def alpha_sx(self) -> float:
-        ''' AS4100 Cl 6.6.1.1(iv) slenderness reduction factor'''
+        """AS4100 Cl 6.6.1.1(iv) slenderness reduction factor"""
         return self.alpha_s(self._M_sx(), self.M_oa)
 
     @property
     def M_oa(self) -> float:
-        ''' AS4100 Cl 5.6.1.1(iv) M_oa = M_o or value determined from elastic buckling analysis'''
+        """AS4100 Cl 5.6.1.1(iv) M_oa = M_o or value determined from elastic buckling analysis"""
         return self.M_o
 
     @property
     def M_o(self) -> float:
-        ''' AS4100 Cl 5.6.1 M_o reference buckling moment'''
+        """AS4100 Cl 5.6.1 M_o reference buckling moment"""
         return reference_buckling_moment(self.section, self.l_eb)
 
     # ------------------------------------------------------------------------
     # AS4100 Section 6 Members subject to axial compression
     # ------------------------------------------------------------------------M_bx
 
     def _N_s(self) -> float:
-        '''AS4100 Cl 6.2.1 Nominal section capacity'''
+        """AS4100 Cl 6.2.1 Nominal section capacity"""
         return self.section.k_f * self.section.A_n * self.section.f_y
 
     def _N_cx(self) -> float:
-        '''AS4100 Cl 6.3.3 Nominal section capacity (x axis) of a member of constant cross-section subject to flexural bending'''
+        """AS4100 Cl 6.3.3 Nominal section capacity (x axis) of a member of constant cross-section subject to flexural bending"""
         if self.l_ex > 0:
             return self.alpha_cx * self._N_s()
         else:
             return self._N_s()
 
     def _N_cy(self) -> float:
-        '''AS4100 Cl 6.3.3 Nominal section capacity (y axis) of a member of constant cross-section subject to flexural bending'''
+        """AS4100 Cl 6.3.3 Nominal section capacity (y axis) of a member of constant cross-section subject to flexural bending"""
         if self.l_ey > 0:
             return self.alpha_cy * self._N_s()
         else:
             return self._N_s()
 
     @staticmethod
     def alpha_c(xi: float, lam: float) -> float:
-        '''AS4100 Cl 6.3.3 member slenderness reduction factor, compression'''
-        return xi*(1-(1-(90/(xi*lam))**2)**0.5)
+        """AS4100 Cl 6.3.3 member slenderness reduction factor, compression"""
+        return xi * (1 - (1 - (90 / (xi * lam)) ** 2) ** 0.5)
 
     @property
     def alpha_cx(self) -> float:
-        '''AS4100 Cl 6.3.3 member slenderness reduction factor, compression x-axis'''
+        """AS4100 Cl 6.3.3 member slenderness reduction factor, compression x-axis"""
         return self.alpha_c(self.xi_x, self.lam_x)
 
     @property
     def alpha_cy(self) -> float:
-        '''AS4100 Cl 6.3.3 member slenderness reduction factor, compression y-axis'''
+        """AS4100 Cl 6.3.3 member slenderness reduction factor, compression y-axis"""
         return self.alpha_c(self.xi_y, self.lam_y)
 
     @staticmethod
     def xi(lam: float, eta: float) -> float:
-        '''AS4100 Cl 6.3.3 calculation parameter'''
+        """AS4100 Cl 6.3.3 calculation parameter"""
         # NOTE (2*(lam/90)**2) is equal to zero if lam = 0
         # lam = 0 if l_ex or l_ey = 0
         # length != 0 checked in _N_cx and _N_cy
-        return ((lam/90)**2 + 1 + eta)/(2*(lam/90)**2)
+        return ((lam / 90) ** 2 + 1 + eta) / (2 * (lam / 90) ** 2)
 
     @property
     def xi_x(self) -> float:
-        '''AS4100 Cl 6.3.3 calculation parameter, x-axis'''
+        """AS4100 Cl 6.3.3 calculation parameter, x-axis"""
         eta_x = self.eta(self.lam_x)
         return self.xi(self.lam_x, eta_x)
 
     @property
     def xi_y(self):
-        '''AS4100 Cl 6.3.3 calculation parameter, y-axis'''
+        """AS4100 Cl 6.3.3 calculation parameter, y-axis"""
         eta_y = self.eta(self.lam_y)
         return self.xi(self.lam_y, eta_y)
 
     @staticmethod
     def eta(lam: float) -> float:
-        '''AS4100 Cl 6.3.3 calculation parameter'''
-        return max(0.00326*(lam - 13.5), 0)
+        """AS4100 Cl 6.3.3 calculation parameter"""
+        return max(0.00326 * (lam - 13.5), 0)
 
     @property
     def lam_x(self) -> float:
-        '''AS4100 Cl 6.3.3 slenderness reduction parameter, x-axis'''
+        """AS4100 Cl 6.3.3 slenderness reduction parameter, x-axis"""
         alpha_ax = self.alpha_a(self.lam_nx)
         return self.lam_nx + alpha_ax * self.section.alpha_b
 
     @property
     def lam_y(self) -> float:
-        '''AS4100 Cl 6.3.3 slenderness reduction parameter, y-axis'''
+        """AS4100 Cl 6.3.3 slenderness reduction parameter, y-axis"""
         alpha_ay = self.alpha_a(self.lam_ny)
         return self.lam_ny + alpha_ay * self.section.alpha_b
 
     @property
     def lam_nx(self) -> float:
-        '''AS4100 Cl 6.3.3 modified member slenderness, x-axis'''
-        l = (self.l_ex/self.section.r_x) * \
-            (self.section.k_f * self.section.f_y/250)**0.5
+        """AS4100 Cl 6.3.3 modified member slenderness, x-axis"""
+        l = (self.l_ex / self.section.r_x) * (
+            self.section.k_f * self.section.f_y / 250
+        ) ** 0.5
         return l
 
     @property
     def lam_ny(self) -> float:
-        '''AS4100 Cl 6.3.3 modified member slenderness, y-axis'''
-        return (self.l_ey/self.section.r_y) * (self.section.k_f * self.section.f_y/250)**0.5
+        """AS4100 Cl 6.3.3 modified member slenderness, y-axis"""
+        return (self.l_ey / self.section.r_y) * (
+            self.section.k_f * self.section.f_y / 250
+        ) ** 0.5
 
     @staticmethod
     def alpha_a(lam_n: float) -> float:
-        '''AS4100 Cl 6.3.3 calculation parameter'''
-        return 2100*(lam_n - 13.5)/(lam_n**2 - 15.3*lam_n + 2050)
+        """AS4100 Cl 6.3.3 calculation parameter"""
+        return 2100 * (lam_n - 13.5) / (lam_n**2 - 15.3 * lam_n + 2050)
 
     # ------------------------------------------------------------------------
     # AS4100 Section 7 Members subject to axial tension-----------------------
     # ------------------------------------------------------------------------
 
+    @property
+    def _N_ty(self) -> float:
+        """AS4100 Cl 7.2 - tension yield capacity"""
+        return self.section.A_g * self.section.f_y
+
+    @property
+    def _N_tf(self) -> float:
+        """AS4100 Cl 7.2 - tension fracture capacity"""
+        return 0.85 * self.k_t * self.section.A_n * self.section.f_u
+
     def _N_t(self) -> float:
-        ''' AS4100 Cl 7.2 Nominal section capacity, axial tension'''
-        N_t = min(self.section.A_g * self.section.f_y, 0.85 *
-                  self.k_t * self.section.A_n*self.section.f_u)
+        """AS4100 Cl 7.2 Nominal section capacity, axial tension"""
+        N_t = min(
+            self._N_ty,
+            self._N_tf,
+        )
         return N_t
 
     # ------------------------------------------------------------------------
     # AS4100 Section combined actions ---------
     # ------------------------------------------------------------------------
 
     def M_ix(self, N_star, l_ex):
         if N_star <= 0:
-            return self.M_sx()*(1 + N_star/(self.phi["N_c"] * self.N_cx(l_ex)))
+            return self.M_sx() * (1 + N_star / (self.phi["N_c"] * self.N_cx(l_ex)))
         else:
             return None
 
     def M_iy(self, N_star, l_ey):
         if N_star <= 0:
-            return self.M_sy()*(1 + N_star/(self.phi["N_c"] * self.N_cy(l_ey)))
+            return self.M_sy() * (1 + N_star / (self.phi["N_c"] * self.N_cy(l_ey)))
         else:
             return None
 
     def M_rx(self, N_star):
-        return self.M_sx() * (1 - abs(N_star)/(self.phi["N_s"] * self.N_t()))
+        return self.M_sx() * (1 - abs(N_star) / (self.phi["N_s"] * self.N_t()))
 
     def M_ox(self, N_star, l_eb, l_ey, alpha_m):
         if N_star <= 0:
             # compression
-            return self.M_bx(l_eb, alpha_m)*(1 + N_star/(self.phi["N_c"] * self.N_cy(l_ey)))
+            return self.M_bx(l_eb, alpha_m) * (
+                1 + N_star / (self.phi["N_c"] * self.N_cy(l_ey))
+            )
         else:
             # tension
-            return min(self.M_bx(l_eb, alpha_m)*(1 + N_star/(self.phi["N_c"] * self.N_t())), self.M_rx(N_star))
+            return min(
+                self.M_bx(l_eb, alpha_m)
+                * (1 + N_star / (self.phi["N_c"] * self.N_t())),
+                self.M_rx(N_star),
+            )
 
     def M_cx(self, N_star, l_ex, l_ey, l_eb, alpha_m):
         try:
             return min(self.M_ix(N_star, l_ey), self.M_ox(N_star, l_eb, l_ey, alpha_m))
         except:
             return self.M_ox(N_star, l_eb, l_ey, alpha_m)
 
     # shear calculations -----------------------------------------------------
 
     # shear calcs depend on the section shape so it can't be generic
     # def V_v(self): # pragma: no cover
     #     raise NotImplementedError
 
     def _V_v(self):
-        ''' AS4100 Cl 5.11.1 shear capacity of web  '''
+        """AS4100 Cl 5.11.1 shear capacity of web"""
         if self.section.shear_stress_uniformity == 1:
             # approximately uniform shear stress distribution
             return self.V_u
         else:
             # non-uniform shear stress distribution
             return self.V_nu
 
     @property
     def V_u(self):
-        '''Cl 5.11.2 approximately uniform shear stress distribution'''
+        """Cl 5.11.2 approximately uniform shear stress distribution"""
         if self.section.web_shear_yield_governs:
             return self.V_w
         else:
             return self.V_b
 
     @property
     def V_nu(self):
-        '''Cl 5.11.3 non-uniform shear stress distribution'''
+        """Cl 5.11.3 non-uniform shear stress distribution"""
         v_u = self.V_u
         v_nu = 2 * v_u / (0.9 + self.section.shear_stress_uniformity)
         return min(v_u, v_nu)
 
     @property
     def V_w(self) -> float:
-        '''AS4100 Cl 5.11.4 shear yield capacity'''
-        if self.section.sec_type == 'CHS':
+        """AS4100 Cl 5.11.4 shear yield capacity"""
+        if self.section.sec_type == "CHS":
             A_e = self.section.A_g
             return 0.36 * self.section.f_y * A_e
         else:
             # TODO: improve this - embed in SteelSection?
-            if 'f_yw' in self.section.mat.__dict__:
-                return 0.6*self.section.f_yw * self.section.A_w
+            if "f_yw" in self.section.mat.__dict__:
+                return 0.6 * self.section.f_yw * self.section.A_w
             else:
-                return 0.6*self.section.f_y * self.section.A_w
+                return 0.6 * self.section.f_y * self.section.A_w
 
     @property
     def V_b(self) -> float:
-        '''AS4100 Cl 5.11.5 shear buckling capacity'''
+        """AS4100 Cl 5.11.5 shear buckling capacity"""
         # NOTE: only implemented for unstiffened web
         return self.section.alpha_v * self.V_w
 
     @classmethod
     def column_order(cls):
-        n = ['name',   # 'l_ex', 'l_ey',
-             'phiN_s', 'phiN_t',
-             'phiM_sx', 'phiM_sy', 'phiV_v', 'section_name', 'material_name']
+        n = [
+            "name",  # 'l_ex', 'l_ey',
+            "phiN_s",
+            "phiN_t",
+            "phiM_sx",
+            "phiM_sy",
+            "phiV_v",
+            "section_name",
+            "material_name",
+        ]
         return n
 
     # @classmethod
     # #def from_dict(cls, attr_dict):
     # def from_dict(cls, **kwargs):
     #     o = cls()
     #     for k, v in kwargs.items():
@@ -472,39 +555,12 @@
     #                 # this is limited to I-section
     #                 setattr(o, k, SteelISection.from_dict(**v))
     #             else:
     #                 setattr(o, k, v)
     #     return o
 
 
-def main():
-    from pathlib import Path
-    import pandas as pd
-    path = Path(__file__)
-    input_data = str(path.parent.parent)+'\\input_data\\AUS_open_sections.csv'
-
-    section_df = pd.read_csv(input_data, skiprows=[1])
-    section_df = section_df.apply(pd.to_numeric, errors='ignore').fillna(0)
-    section_dict = section_df.iloc[1].to_dict()
-    ss = SteelSection.from_section_dict(section_dict)
-    print('\nSteel section (container class for all section attributes):')
-    print(ss)
-
-    sm = SteelMember(section=ss)
-    print('\nSteel member with section capacities calculated as per AS4100')
-    print(sm)
-
-    sm = SteelMember(section=ss, l_ex=21000, l_ey=0, l_eb=0, alpha_m = 1)
-
-    print('\nSteel member with member capacities calculated as per AS4100')
-    print(sm)
-    #ss.k_f = 0.825 -> #OK
-    #ss.alpha_b = 0.5 #OK
-    print(sm.phiN_c)
-    ...
-    #calc value = 10500.0
-    #verif value = 9700
-    #error = 8.2475
+def main(): ...
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `steelas-0.1.2/src/steelas/member/slenderness.py` & `steelas-0.2.0/src/steelas/member/slenderness.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,37 +11,35 @@
 from typing import Tuple
 import numpy as np
 from math import pi, isnan, floor, log10
 
 # from structuraldesigntoolbox.
 from steelas.member.material import SteelMaterial
 from steelas.member.geometry import SectionGeometry
+from steelas.data.io import report
 
 
 @dataclass(kw_only=True)
-class SteelSlenderness():
+class SteelSlenderness:
     # AS4100 Cl 5.2.2, 5.2.3, 5.2.5, 5.2.5
     geom: SectionGeometry | None = None
     mat: SteelMaterial | None = None
     # TODO - don't store geom and mat as attrs?
 
-    name: str = ''  # section name  (shape + material)
-    section: str = ''  # section shape
-    grade: str = ''  # material
-
-    components_x: list[PlateComponent] = field(
-        default_factory=list, repr=False)
-    components_y: list[PlateComponent] = field(
-        default_factory=list, repr=False)
+    name: str = ""  # section name  (shape + material)
+    section: str = ""  # section shape
+    grade: str = ""  # material
+
+    components_x: list[PlateComponent] = field(default_factory=list, repr=False)
+    components_y: list[PlateComponent] = field(default_factory=list, repr=False)
     # compression components
-    components_c: list[PlateComponent] = field(
-        default_factory=list, repr=False)
+    components_c: list[PlateComponent] = field(default_factory=list, repr=False)
 
-    compact_x: str = field(repr=False, default='')
-    compact_y: str = field(repr=False, default='')
+    compact_x: str = field(repr=False, default="")
+    compact_y: str = field(repr=False, default="")
 
     lam_s_x: float = field(repr=False, default=0)  # section slenderness
     lam_sp_x: float = field(repr=False, default=0)  # section slenderness
     lam_sy_x: float = field(repr=False, default=0)  # section slenderness
 
     lam_s_y: float = field(repr=False, default=0)  # section slenderness
     lam_sp_y: float = field(repr=False, default=0)  # section slenderness
@@ -63,39 +61,44 @@
 
     def __post_init__(self):
         if self.geom is not None and self.mat is not None:
             self.name = self.geom.name
             self.grade = self.mat.grade
             self.section = self.geom.section
             match self.geom.sec_type:
-                case 'UB' | 'UC' | 'WB' | 'WC':
+                case "UB" | "UC" | "WB" | "WC":
                     components_method = i_section_components
-                case 'PFC' | 'TFB':
+                case "PFC" | "TFB":
                     components_method = c_section_components
-                case 'SHS' | 'RHS':
+                case "SHS" | "RHS":
                     components_method = rhs_section_components
-                case 'CHS':
+                case "CHS":
                     components_method = chs_section_components
-                case 'BT' | 'CT':
+                case "BT" | "CT":
                     components_method = t_section_components
-                case 'RectPlate':
+                case "RectPlate":
                     components_method = rect_section_components
                 case other:
                     raise NotImplementedError(
-                        f'section type {self.geom.sec_type} not available')
+                        f"section type {self.geom.sec_type} not available"
+                    )
             self.components_x, self.components_y, self.components_c = components_method(
-                self.geom, self.mat)
+                self.geom, self.mat
+            )
             self.solve_slenderness()
 
             # round to sig figs
             if self.sig_figs:
                 for k, v in list(self.__dict__.items()):
                     if isinstance(v, (float, int)) and (not isnan(v)) and (v != 0):
-                        setattr(self, k, round(v, self.sig_figs -
-                                int(floor(log10(abs(v))))-1))
+                        setattr(
+                            self,
+                            k,
+                            round(v, self.sig_figs - int(floor(log10(abs(v)))) - 1),
+                        )
 
     def solve_slenderness(self):
         # compact_x
         # compact_y
 
         # AS4100 Cl5.2.2.
         # lam_sp and lam_sy are values from element with greatest lam_s = lem_e/lam_ey
@@ -105,15 +108,15 @@
                 max_lam_e_ratio = p.lam_e_ratio
                 self.lam_s_x = p.lam_e
                 self.lam_sp_x = p.lam_ep
                 self.lam_sy_x = p.lam_ey
 
                 if isinstance(p, RingComponent):
                     self.slender_section_type_x = 3
-                elif p.edge_sup == 'One' and p.load_type == 'CompToTens':
+                elif p.edge_sup == "One" and p.load_type == "CompToTens":
                     self.slender_section_type_x = 2
                 else:
                     self.slender_section_type_x = 1
 
         max_lam_e_ratio = 0
         for p in self.components_y:
             if p.lam_e_ratio > max_lam_e_ratio:
@@ -128,416 +131,578 @@
         self.Z_ey = self._Z_ey()
         self.A_e = self._A_e()
         self.k_f = self._k_f()
         self.alpha_b = self._alpha_b()
         self.web_shear_yield_governs = self._web_shear_yield_governs()
         self.alpha_v = self._alpha_v()
 
+    def report(self, **kwargs) -> None:
+        report(
+            self,
+            exclude_attribute_names=[
+                "geom",
+                "mat",
+                "components_x",
+                "components_y",
+                "components_c",
+            ],
+            **kwargs,
+        )
+
     def _A_e(self):
         A_e = 0
         A_e += self.geom.A_g
         for p in self.components_c:
             A_e -= p.A_v
         #    A_e += p.A_e
         return A_e
 
     def _k_f(self) -> float:
-        return self.A_e/self.geom.A_g
+        return self.A_e / self.geom.A_g
 
     def _Z_ex(self) -> float:
         # AS4100 Cl5.2
         if self.lam_s_x <= self.lam_sp_x:
-            self.compact_x = 'C'
+            self.compact_x = "C"
             return self._Z_excompact
         elif self.lam_s_x <= self.lam_sy_x:
-            self.compact_x = 'N'
+            self.compact_x = "N"
             return self._Z_exnoncompact
         else:
-            self.compact_x = 'S'
+            self.compact_x = "S"
             return self._Z_exslender
 
     def _Z_ey(self) -> float:
         # AS4100 Cl 5.2
         if self.lam_s_y <= self.lam_sp_y:
-            self.compact_y = 'C'
+            self.compact_y = "C"
             return self._Z_eycompact
         elif self.lam_s_y <= self.lam_sy_y:
-            self.compact_y = 'N'
+            self.compact_y = "N"
             return self._Z_eynoncompact
         else:
-            self.compact_y = 'S'
+            self.compact_y = "S"
             return self._Z_eyslender
 
     @property
     def _Z_excompact(self) -> float:
         # AS4100 Cl 5.2.3
-        return min(self.geom.S_x, 1.5*self.geom.Z_x)
+        return min(self.geom.S_x, 1.5 * self.geom.Z_x)
 
     @property
     def _Z_eycompact(self) -> float:
         # AS4100 Cl 5.2.3
-        return min(self.geom.S_y, 1.5*self.geom.Z_y)
+        return min(self.geom.S_y, 1.5 * self.geom.Z_y)
 
     @property
     def _Z_exnoncompact(self) -> float:
         # AS4100 Cl 5.2.4
-        return self.geom.Z_x + \
-            (self.lam_sy_x - self.lam_s_x)/(self.lam_sy_x - self.lam_sp_x) * \
-            (self._Z_excompact - self.geom.Z_x)
+        return self.geom.Z_x + (self.lam_sy_x - self.lam_s_x) / (
+            self.lam_sy_x - self.lam_sp_x
+        ) * (self._Z_excompact - self.geom.Z_x)
 
     @property
     def _Z_eynoncompact(self) -> float:
         # AS4100 Cl 5.2.4
-        return self.geom.Z_y + \
-            (self.lam_sy_y - self.lam_s_y)/(self.lam_sy_y - self.lam_sp_y) * \
-            (self._Z_eycompact - self.geom.Z_y)
+        return self.geom.Z_y + (self.lam_sy_y - self.lam_s_y) / (
+            self.lam_sy_y - self.lam_sp_y
+        ) * (self._Z_eycompact - self.geom.Z_y)
 
     @property
     def _Z_exslender(self) -> float:
         # AS4100 Cl 5.2.5
         # TODO - do this properly
         if self.slender_section_type_x == 1:
-            if self.geom.sec_type not in ['RHS', 'SHS']:
-                z = self.geom.Z_x * self.lam_sy_x/self.lam_s_x
+            if self.geom.sec_type not in ["RHS", "SHS"]:
+                z = self.geom.Z_x * self.lam_sy_x / self.lam_s_x
             else:
-                #https://www.steelforlifebluebook.co.uk/explanatory-notes/bs5950/effective-properties/
-                #BS 5950-1 3.6.2.2?
+                # https://www.steelforlifebluebook.co.uk/explanatory-notes/bs5950/effective-properties/
+                # BS 5950-1 3.6.2.2?
                 d = self.geom.d
                 b = self.geom.b
                 t = self.geom.t
                 A = self.geom.A_g
 
-                eps	= (275/self.mat.f_y)**0.5
+                eps = (275 / self.mat.f_y) ** 0.5
 
-                k = (b-35*t*eps-5*t)
+                k = b - 35 * t * eps - 5 * t
 
-                y_xeff = (A*d - k*t**2)/(2*(A-k*t))
-                A_eff = A - k*t
-                I_ex = self.geom.I_x - k * t**3/12 - k*t*(d/2-t/2)**2-A_eff*(y_xeff-d/2)**2 
+                y_xeff = (A * d - k * t**2) / (2 * (A - k * t))
+                A_eff = A - k * t
+                I_ex = (
+                    self.geom.I_x
+                    - k * t**3 / 12
+                    - k * t * (d / 2 - t / 2) ** 2
+                    - A_eff * (y_xeff - d / 2) ** 2
+                )
 
-                z = I_ex/y_xeff
+                z = I_ex / y_xeff
 
         elif self.slender_section_type_x == 2:
-            z = self.geom.Z_x * (self.lam_sy_x/self.lam_s_x)**2
+            z = self.geom.Z_x * (self.lam_sy_x / self.lam_s_x) ** 2
         elif self._web_shear_slenderness_ratio == 3:
-            raise NotImplementedError('Slender CHS sections not implemented')
+            raise NotImplementedError("Slender CHS sections not implemented")
         return z
 
     @property
     def _Z_eyslender(self) -> float:
         # AS4100 Cl 5.2.5
         # TODO - do this properly
-        if self.geom.sec_type not in ['RHS', 'SHS']:
-            Z_ey= self.geom.Z_y * self.lam_sy_y/self.lam_s_y
+        if self.geom.sec_type not in ["RHS", "SHS"]:
+            Z_ey = self.geom.Z_y * self.lam_sy_y / self.lam_s_y
         else:
-            #https://www.steelforlifebluebook.co.uk/explanatory-notes/bs5950/effective-properties/
-            #BS 5950-1 3.6.2.2?
+            # https://www.steelforlifebluebook.co.uk/explanatory-notes/bs5950/effective-properties/
+            # BS 5950-1 3.6.2.2?
             d = self.geom.d
             b = self.geom.b
             t = self.geom.t
             A = self.geom.A_g
 
-            eps	= (275/self.mat.f_y)**0.5
-            k = (d-35*t*eps-5*t)
+            eps = (275 / self.mat.f_y) ** 0.5
+            k = d - 35 * t * eps - 5 * t
+
+            x_xeff = (A * b - k * t**2) / (2 * (A - k * t))
+            A_eff = A - k * t
+            I_ey = (
+                self.geom.I_y
+                - k * t**3 / 12
+                - k * t * (b / 2 - t / 2) ** 2
+                - A_eff * (x_xeff - b / 2) ** 2
+            )
 
-            x_xeff = (A*b - k*t**2)/(2*(A-k*t))
-            A_eff = A - k*t
-            I_ey = self.geom.I_y - k * t**3/12 - k*t*(b/2-t/2)**2-A_eff*(x_xeff-b/2)**2 
+            Z_ey = I_ey / x_xeff
 
-            Z_ey = I_ey/x_xeff
-            
         return Z_ey
 
     def _alpha_b(self) -> float:
-        '''AS4100 Table 6.3.3A, member section constant'''
+        """AS4100 Table 6.3.3A, member section constant"""
         return self._member_section_constant(geom=self.geom, k_f=self.k_f)
 
     @staticmethod
     def _member_section_constant(geom: SectionGeometry, k_f: float = 0) -> float:
-        '''AS4100 Table 6.3.3(A) and 6.3.3(B) '''
+        """AS4100 Table 6.3.3(A) and 6.3.3(B)"""
         if k_f < 1:
             # T6.3.3(B)
             match geom.sec_type:
-                case 'SHS' | 'RHS' | 'CHS':
+                case "SHS" | "RHS" | "CHS":
                     a = -0.5
-                case 'UB' | 'UC':
+                case "UB" | "UC":
                     t_f = geom.t_f
                     a = 0 if t_f <= 40 else 0.5
-                case 'WB' | 'WC':
+                case "WB" | "WC":
                     t_f = geom.t_f
                     a = 0.5 if t_f <= 40 else 1.0
                 case other:
                     a = 1.0
         else:  # k_f = 1
             # T6.3.3(A)
             match geom.sec_type:
-                case 'SHS' | 'RHS' | 'CHS':
+                case "SHS" | "RHS" | "CHS":
                     a = -1
                     # NOTE: stress relief considerations not implemented
-                case 'UB' | 'UC' | 'TFB':
+                case "UB" | "UC" | "TFB":
                     t_f = geom.t_f
                     a = 0 if t_f <= 40 else 1.0
-                case 'PFC' | 'BT' | 'CT':
+                case "PFC" | "BT" | "CT":
                     a = 0.5
-                case 'WB' | 'WC':
-                    a = 0.0 #AISC Des. Cap. Tables T6.1
-                    #t_f = geom.t_f
-                    #a = 0.5 if t_f <= 40 else 1.0
+                case "WB" | "WC":
+                    a = 0.0  # AISC Des. Cap. Tables T6.1
+                    # t_f = geom.t_f
+                    # a = 0.5 if t_f <= 40 else 1.0
                 case other:
                     a = 0.5
                     # raise NotImplementedError(
                     #    f'section {geom.sec_type} not implemented for alpha_b - See T6.3.3(A)')
         return a
 
     def _web_shear_yield_governs(self) -> bool:
-        '''AS4100 Cl 5.11.2 web shear slenderness limit check for sections with approximatly uniform web shear stress distribution'''
+        """AS4100 Cl 5.11.2 web shear slenderness limit check for sections with approximatly uniform web shear stress distribution"""
         web_shear_slenderness_ratio = self._web_shear_slenderness_ratio()
 
         if web_shear_slenderness_ratio <= 1:
             return False
         else:
             return True
 
     def _web_shear_slenderness_ratio(self) -> bool:
-        '''AS4100 Cl 5.11.2 web shear slenderness ratio for sections with approximatly uniform web shear stress distribution'''
-        r1 = self.geom.d_p/self.geom.t_w
-        if 'f_yw' in self.mat.__dict__:
-            r2 = 82/(self.mat.f_yw/250)**0.5
+        """AS4100 Cl 5.11.2 web shear slenderness ratio for sections with approximatly uniform web shear stress distribution"""
+        r1 = self.geom.d_p / self.geom.t_w
+        if "f_yw" in self.mat.__dict__:
+            r2 = 82 / (self.mat.f_yw / 250) ** 0.5
         else:
-            r2 = 82/(self.mat.f_y/250)**0.5
+            r2 = 82 / (self.mat.f_y / 250) ** 0.5
         return r2 / r1
 
     def _alpha_v(self) -> float:
-        '''AS4100 5.11.5.1 unstiffened web shear buckling reduction factor'''
-        return min((self._web_shear_slenderness_ratio())**2, 1)
+        """AS4100 5.11.5.1 unstiffened web shear buckling reduction factor"""
+        return min((self._web_shear_slenderness_ratio()) ** 2, 1)
 
     @classmethod
     def column_order(cls) -> list[str]:
-        '''specifies the reported attributes when output to dataframe'''
+        """specifies the reported attributes when output to dataframe"""
         k = list(cls.__annotations__.keys())
 
         # lam_s_x,  lam_sp_x,  lam_sy_x,  lam_s_y,  lam_sp_y, lam_sy_y,
 
-        n = ['section', 'grade', 'compact_x', 'compact_y', 'Z_ex', 'Z_ey', 'k_f', 'A_e',
-             #'lam_s_x', 'lam_sp_x',  'lam_sy_x',  'lam_s_y',  'lam_sp_y', 'lam_sy_y',
-             'alpha_b', 'web_shear_yield_governs', 'alpha_v']
+        n = [
+            "section",
+            "grade",
+            "compact_x",
+            "compact_y",
+            "Z_ex",
+            "Z_ey",
+            "k_f",
+            "A_e",
+            #'lam_s_x', 'lam_sp_x',  'lam_sy_x',  'lam_s_y',  'lam_sp_y', 'lam_sy_y',
+            "alpha_b",
+            "web_shear_yield_governs",
+            "alpha_v",
+        ]
         return n  # + [x for x in k if x not in n]
 
     @classmethod
     def from_dict(cls, **kwargs):
         o = cls()
-        #all_ann = cls.__annotations__
+        # all_ann = cls.__annotations__
         for k, v in kwargs.items():
             # note - @property items are in hasattr but not in __annotations__)
             if hasattr(o, k):  # and (k in cls.__annotations__):
                 setattr(o, k, v)
         return o
 
 
 def i_section_components(geom: SectionGeometry, mat: SteelMaterial):
-    '''populate components required for slenderness evaluation'''
+    """populate components required for slenderness evaluation"""
 
     # major axis bending
-    c_flange_x = PlateComponent(b=geom.b_ff,  t=geom.t_f, f_y=mat.f_y,
-                                edge_sup='One', load_type='UniformComp', res_stress=mat.res_stress)
+    c_flange_x = PlateComponent(
+        b=geom.b_ff,
+        t=geom.t_f,
+        f_y=mat.f_y,
+        edge_sup="One",
+        load_type="UniformComp",
+        res_stress=mat.res_stress,
+    )
     # TODO - ask ASI about f_y vs f_yf in web slenderness check
     # verification data uses f_y
     # c_web_x = PlateComponent(b=geom.d_1,  t=geom.t_w, f_y=mat.f_yw,
     #                         edge_sup='Both', load_type='CompToTens', res_stress=mat.res_stress)
-    c_web_x = PlateComponent(b=geom.d_1,  t=geom.t_w, f_y=mat.f_y,
-                             edge_sup='Both', load_type='CompToTens', res_stress=mat.res_stress)
+    c_web_x = PlateComponent(
+        b=geom.d_1,
+        t=geom.t_w,
+        f_y=mat.f_y,
+        edge_sup="Both",
+        load_type="CompToTens",
+        res_stress=mat.res_stress,
+    )
     components_x = [c_flange_x, c_web_x]
 
     # minor axis bending
-    c_flange_y = PlateComponent(b=geom.b_ff,  t=geom.t_f, f_y=mat.f_y,
-                                edge_sup='One', load_type='CompToTens', res_stress=mat.res_stress)
+    c_flange_y = PlateComponent(
+        b=geom.b_ff,
+        t=geom.t_f,
+        f_y=mat.f_y,
+        edge_sup="One",
+        load_type="CompToTens",
+        res_stress=mat.res_stress,
+    )
     # note - web never governs as unsupported outstand width is zero
-    #c_web_y = PlateComponent(b=0,  t=self.t_w, f_y = self.f_yw, edge_sup = 'Both', load_type = 'CompToTens', res_stress = self.res_stress)
+    # c_web_y = PlateComponent(b=0,  t=self.t_w, f_y = self.f_yw, edge_sup = 'Both', load_type = 'CompToTens', res_stress = self.res_stress)
     components_y = [c_flange_y]  # , c_web_y]
 
     # compression
-    c_flange_c = PlateComponent(b=geom.b_ff,  t=geom.t_f, f_y=mat.f_y,
-                                edge_sup='One', load_type='UniformComp', res_stress=mat.res_stress)
+    c_flange_c = PlateComponent(
+        b=geom.b_ff,
+        t=geom.t_f,
+        f_y=mat.f_y,
+        edge_sup="One",
+        load_type="UniformComp",
+        res_stress=mat.res_stress,
+    )
     # TODO - as above, f_y vs f_yw in web slenderness check
-    c_web_c = PlateComponent(b=geom.d_1,  t=geom.t_w, f_y=mat.f_y,
-                             edge_sup='Both', load_type='UniformComp', res_stress=mat.res_stress)
+    c_web_c = PlateComponent(
+        b=geom.d_1,
+        t=geom.t_w,
+        f_y=mat.f_y,
+        edge_sup="Both",
+        load_type="UniformComp",
+        res_stress=mat.res_stress,
+    )
     components_c = [c_web_c] + [c_flange_c] * 4
 
     return components_x, components_y, components_c
 
 
 def c_section_components(geom: SectionGeometry, mat: SteelMaterial):
-    '''populate components required for Cee section slenderness evaluation'''
+    """populate components required for Cee section slenderness evaluation"""
 
     # major axis bending
-    c_flange_x = PlateComponent(b=geom.b_ff,  t=geom.t_f, f_y=mat.f_y,
-                                edge_sup='One', load_type='UniformComp', res_stress=mat.res_stress)
+    c_flange_x = PlateComponent(
+        b=geom.b_ff,
+        t=geom.t_f,
+        f_y=mat.f_y,
+        edge_sup="One",
+        load_type="UniformComp",
+        res_stress=mat.res_stress,
+    )
     # TODO - ask ASI about f_y vs f_yf in web slenderness check
     # verification data uses f_y
     # c_web_x = PlateComponent(b=geom.d_1,  t=geom.t_w, f_y=mat.f_yw,
     #                         edge_sup='Both', load_type='CompToTens', res_stress=mat.res_stress)
-    c_web_x = PlateComponent(b=geom.d_1,  t=geom.t_w, f_y=mat.f_y,
-                             edge_sup='Both', load_type='CompToTens', res_stress=mat.res_stress)
+    c_web_x = PlateComponent(
+        b=geom.d_1,
+        t=geom.t_w,
+        f_y=mat.f_y,
+        edge_sup="Both",
+        load_type="CompToTens",
+        res_stress=mat.res_stress,
+    )
     components_x = [c_flange_x, c_web_x]
 
     # minor axis bending
-    c_flange_y = PlateComponent(b=geom.b_ff,  t=geom.t_f, f_y=mat.f_y,
-                                edge_sup='One', load_type='CompToTens', res_stress=mat.res_stress)
+    c_flange_y = PlateComponent(
+        b=geom.b_ff,
+        t=geom.t_f,
+        f_y=mat.f_y,
+        edge_sup="One",
+        load_type="CompToTens",
+        res_stress=mat.res_stress,
+    )
     # note - web never governs as unsupported outstand width is zero
     # f_yw, or f_y
     # note - c_section dir_1 assumed as tension in the web element
     # c_web_y = PlateComponent(b=geom.d_1,  t=geom.t_w, f_y=mat.f_y,
     #                         edge_sup='Both', load_type='UniformComp', res_stress=mat.res_stress)
     components_y = [c_flange_y]  # , c_web_y]
 
     # compression
-    c_flange_c = PlateComponent(b=geom.b_ff,  t=geom.t_f, f_y=mat.f_y,
-                                edge_sup='One', load_type='UniformComp', res_stress=mat.res_stress)
+    c_flange_c = PlateComponent(
+        b=geom.b_ff,
+        t=geom.t_f,
+        f_y=mat.f_y,
+        edge_sup="One",
+        load_type="UniformComp",
+        res_stress=mat.res_stress,
+    )
     # TODO - as above, f_y vs f_yw in web slenderness check
-    c_web_c = PlateComponent(b=geom.d_1,  t=geom.t_w, f_y=mat.f_y,
-                             edge_sup='Both', load_type='UniformComp', res_stress=mat.res_stress)
+    c_web_c = PlateComponent(
+        b=geom.d_1,
+        t=geom.t_w,
+        f_y=mat.f_y,
+        edge_sup="Both",
+        load_type="UniformComp",
+        res_stress=mat.res_stress,
+    )
     components_c = [c_web_c] + [c_flange_c] * 2
 
     return components_x, components_y, components_c
 
 
 def t_section_components(geom: SectionGeometry, mat: SteelMaterial):
-    '''populate components required for t-section (stem up) slenderness evaluation'''
+    """populate components required for t-section (stem up) slenderness evaluation"""
 
     # major axis bending
     # c_flange_x = PlateComponent(b=geom.b_ff,  t=geom.t_f, f_y=mat.f_y,
     #                            edge_sup='One', load_type='UniformComp', res_stress=mat.res_stress)
-    c_web_x = PlateComponent(b=geom.d_1,  t=geom.t_w, f_y=mat.f_y,
-                             edge_sup='One', load_type='CompToTens', res_stress=mat.res_stress)
+    c_web_x = PlateComponent(
+        b=geom.d_1,
+        t=geom.t_w,
+        f_y=mat.f_y,
+        edge_sup="One",
+        load_type="CompToTens",
+        res_stress=mat.res_stress,
+    )
     components_x = [c_web_x]
 
     # minor axis bending
-    c_flange_y = PlateComponent(b=geom.b_ff,  t=geom.t_f, f_y=mat.f_y,
-                                edge_sup='One', load_type='CompToTens', res_stress=mat.res_stress)
+    c_flange_y = PlateComponent(
+        b=geom.b_ff,
+        t=geom.t_f,
+        f_y=mat.f_y,
+        edge_sup="One",
+        load_type="CompToTens",
+        res_stress=mat.res_stress,
+    )
     components_y = [c_flange_y]  # , c_web_y]
 
     # compression
-    c_flange_c = PlateComponent(b=geom.b_ff,  t=geom.t_f, f_y=mat.f_y,
-                                edge_sup='One', load_type='UniformComp', res_stress=mat.res_stress)
+    c_flange_c = PlateComponent(
+        b=geom.b_ff,
+        t=geom.t_f,
+        f_y=mat.f_y,
+        edge_sup="One",
+        load_type="UniformComp",
+        res_stress=mat.res_stress,
+    )
     # TODO - as above, f_y vs f_yw in web slenderness check
-    c_web_c = PlateComponent(b=geom.d_1,  t=geom.t_w, f_y=mat.f_y,
-                             edge_sup='One', load_type='UniformComp', res_stress=mat.res_stress)
+    c_web_c = PlateComponent(
+        b=geom.d_1,
+        t=geom.t_w,
+        f_y=mat.f_y,
+        edge_sup="One",
+        load_type="UniformComp",
+        res_stress=mat.res_stress,
+    )
     components_c = [c_web_c] + [c_flange_c] * 2
 
     return components_x, components_y, components_c
 
 
 def rhs_section_components(geom: SectionGeometry, mat: SteelMaterial):
     # solve slenderness
-    c_flange_x = PlateComponent(b=geom.b_ff,  t=geom.t, f_y=mat.f_y,
-                                edge_sup='Both', load_type='UniformComp', res_stress=mat.res_stress)
-    c_web_x = PlateComponent(b=geom.d_1,  t=geom.t, f_y=mat.f_y,
-                             edge_sup='Both', load_type='CompToTens', res_stress=mat.res_stress)
+    c_flange_x = PlateComponent(
+        b=geom.b_ff,
+        t=geom.t,
+        f_y=mat.f_y,
+        edge_sup="Both",
+        load_type="UniformComp",
+        res_stress=mat.res_stress,
+    )
+    c_web_x = PlateComponent(
+        b=geom.d_1,
+        t=geom.t,
+        f_y=mat.f_y,
+        edge_sup="Both",
+        load_type="CompToTens",
+        res_stress=mat.res_stress,
+    )
     components_x = [c_flange_x, c_web_x]
 
-    c_flange_y = PlateComponent(b=geom.b_ff,  t=geom.t, f_y=mat.f_y,
-                                edge_sup='Both', load_type='CompToTens', res_stress=mat.res_stress)
-    c_web_y = PlateComponent(b=geom.d_1,  t=geom.t, f_y=mat.f_y,
-                             edge_sup='Both', load_type='UniformComp', res_stress=mat.res_stress)
+    c_flange_y = PlateComponent(
+        b=geom.b_ff,
+        t=geom.t,
+        f_y=mat.f_y,
+        edge_sup="Both",
+        load_type="CompToTens",
+        res_stress=mat.res_stress,
+    )
+    c_web_y = PlateComponent(
+        b=geom.d_1,
+        t=geom.t,
+        f_y=mat.f_y,
+        edge_sup="Both",
+        load_type="UniformComp",
+        res_stress=mat.res_stress,
+    )
     components_y = [c_flange_y, c_web_y]
 
     # compression
     # PlateComponent(b=self.b_ff,  t=self.t, f_y = self.f_y, edge_sup = 'Both', load_type = 'UniformComp', res_stress = self.res_stress)
     c_flange_c = c_flange_x
     # PlateComponent(b=self.d_1,  t=self.t_w, f_y = self.f_yw, edge_sup = 'Both', load_type = 'UniformComp', res_stress = self.res_stress)
     c_web_c = c_web_y
     components_c = [c_web_c] * 2 + [c_flange_c] * 2
 
     return components_x, components_y, components_c
 
 
 def rect_section_components(geom: SectionGeometry, mat: SteelMaterial):
     # solve slenderness
-    print('NOTE: AS 4100 does not contain provisions for slenderness of rectangular plates unsupported at both ends - slenderness is not checked (section assumed as compact and k_f =1)')
+    print(
+        "NOTE: AS 4100 does not contain provisions for slenderness of rectangular plates unsupported at both ends - slenderness is not checked (section assumed as compact and k_f =1)"
+    )
     components_x = []
     components_y = []
     components_c = []
 
     return components_x, components_y, components_c
 
 
-def chs_section_components(geom: SectionGeometry, mat: SteelMaterial) -> Tuple[list[RingComponent], list[RingComponent], list[RingComponent]]:
+def chs_section_components(
+    geom: SectionGeometry, mat: SteelMaterial
+) -> Tuple[list[RingComponent], list[RingComponent], list[RingComponent]]:
     # solve slenderness
-    c_ring = RingComponent(d_o=geom.d,  t=geom.t,
-                           f_y=mat.f_y, res_stress=mat.res_stress)
+    c_ring = RingComponent(d_o=geom.d, t=geom.t, f_y=mat.f_y, res_stress=mat.res_stress)
     components_x = [c_ring]
     components_y = [c_ring]
     components_c = [c_ring]
 
     return components_x, components_y, components_c
 
 
-def plate_element_slenderness_limit(edge_support: str, load_type: str, res_stress: str) -> Tuple(float, float, float):
-    '''
+def plate_element_slenderness_limit(
+    edge_support: str, load_type: str, res_stress: str
+) -> Tuple(float, float, float):
+    """
     AS4100 Table 5.2 and 6.2.4 - Values of plate element slenderness limits
     Returns:
-        lam_ep plasticity limit, 
-        lam_ey yield limit bending, 
-        lam_ed deformation limit 
+        lam_ep plasticity limit,
+        lam_ey yield limit bending,
+        lam_ed deformation limit
 
 
     Parameters:
     edge_support = 'One' or 'Both'
     load_type = 'UniformComp', 'CompToTens', or 'CHS'
     res_stress = 'SR', HR', 'LW', 'CF', or 'HW'
-    '''
+    """
     # TODO -> make this a static method of PlateElement?
-    if edge_support == 'One':
-        if load_type == 'UniformComp':
+    if edge_support == "One":
+        if load_type == "UniformComp":
             match res_stress:
-                case 'SR': val = (10, 16, 35)
-                case 'HR': val = (9, 16, 35)
-                case 'LW' | 'CF': val = (8, 15, 35)
-                case 'HW': val = (8, 14, 34)
-        elif load_type == 'CompToTens':
+                case "SR":
+                    val = (10, 16, 35)
+                case "HR":
+                    val = (9, 16, 35)
+                case "LW" | "CF":
+                    val = (8, 15, 35)
+                case "HW":
+                    val = (8, 14, 34)
+        elif load_type == "CompToTens":
             match res_stress:
-                case 'SR': val = (10, 25, np.nan)
-                case 'HR': val = (9, 25, np.nan)
-                case 'LW' | 'CF' | 'HW': val = (8, 22, np.nan)
-    elif edge_support == 'Both':
-        if load_type == 'UniformComp':
+                case "SR":
+                    val = (10, 25, np.nan)
+                case "HR":
+                    val = (9, 25, np.nan)
+                case "LW" | "CF" | "HW":
+                    val = (8, 22, np.nan)
+    elif edge_support == "Both":
+        if load_type == "UniformComp":
             match res_stress:
-                case 'SR' | 'HR': val = (30, 45, 90)
-                case 'LW' | 'CF': val = (30, 40, 90)
-                case 'HW': val = (30, 35, 90)
-        elif load_type == 'CompToTens':
+                case "SR" | "HR":
+                    val = (30, 45, 90)
+                case "LW" | "CF":
+                    val = (30, 40, 90)
+                case "HW":
+                    val = (30, 35, 90)
+        elif load_type == "CompToTens":
             val = (82, 115, np.nan)
     return val
 
 
-def ring_element_slenderness_limit(res_stress: str) -> Tuple(float, float, float, float):
-    '''
+def ring_element_slenderness_limit(res_stress: str) -> Tuple(
+    float, float, float, float
+):
+    """
     AS4100 Table 5.2 - Values of chs element slenderness limits
     Returns:
-        lam_ep plasticity limit, 
-        lam_ey yield limit, 
+        lam_ep plasticity limit,
+        lam_ey yield limit,
         lam_eyc yield limit compression,
         lam_ed -> not implemented
 
     Parameters:
     res_stress = 'SR', HR', 'LW', 'CF', or 'HW'
-    '''
+    """
     # TODO -> make this a static method of RingElement?
     # NOTE Table 5.2 and 6.2.4 lam_ey different for CHS sections
     match res_stress:
-        case 'SR' | 'HR' | 'CF': val = (50, 120, 82, np.nan)
-        case 'LW' | 'HW': val = (42, 120, 82, np.nan)
+        case "SR" | "HR" | "CF":
+            val = (50, 120, 82, np.nan)
+        case "LW" | "HW":
+            val = (42, 120, 82, np.nan)
     return val
 
 
 @dataclass(kw_only=True)
-class PlateComponent():
-    '''AS4100 Cl5.2.2 Section slenderness - plate components
-       AS4100 Cl 6.2.3 Plate element slenderness for compression
-    '''
+class PlateComponent:
+    """AS4100 Cl5.2.2 Section slenderness - plate components
+    AS4100 Cl 6.2.3 Plate element slenderness for compression
+    """
+
     b: float  # clear width of element from supported edge/edges
     t: float  # element thickness
     f_y: float  # element yield stress
     edge_sup: str  # element edge support
     res_stress: str  # section residual stress type
     load_type: str  # element load type
 
@@ -548,80 +713,84 @@
 
     b_e: float = field(init=False)  # plate element effective width Cl 6.2.4
     A_v: float = field(init=False)
     A_e: float = field(init=False)
 
     def __post_init__(self):
         self.lam_ep, self.lam_ey, _ = plate_element_slenderness_limit(
-            self.edge_sup, self.load_type, self.res_stress)
-        self.lam_e = float(self.b / self.t * (self.f_y/250)**0.5)
-        self.lam_e_ratio = self.lam_e/self.lam_ey
+            self.edge_sup, self.load_type, self.res_stress
+        )
+        self.lam_e = float(self.b / self.t * (self.f_y / 250) ** 0.5)
+        self.lam_e_ratio = self.lam_e / self.lam_ey
 
         # AS4100 Cl 6.2.4
         self.b_e = min(1, self.lam_ey / self.lam_e) * self.b
         self.A_e = self.b_e * self.t
         self.A_v = (self.b - self.b_e) * self.t
         # CHS -> Not implemented
 
 
 @dataclass(kw_only=True)
-class RingComponent():
-    '''AS4100 Cl 5.2.2 Section slenderness - chs components
-       AS4100 Cl 6.2.3 chs element slenderness for compression
-    '''
+class RingComponent:
+    """AS4100 Cl 5.2.2 Section slenderness - chs components
+    AS4100 Cl 6.2.3 chs element slenderness for compression
+    """
+
     d_o: float  # clear width of element from supported edge/edges
     t: float  # element thickness
     f_y: float  # element yield stress
     res_stress: str  # section residual stress type
 
     lam_ey: float = field(init=False)  # element yield limit, bending
     lam_eyc: float = field(init=False)  # element yield limit, compression
     lam_ep: float = field(init=False)  # element plasticity limit
     lam_e: float = field(init=False)  # component slenderness limit
     lam_e_ratio: float = field(init=False)  # component slenderness ratio
 
     d_e: float = field(init=False)  # plate element effective width Cl 6.2.4
-    #A_v: float = field(init=False)
-    #A_e: float = field(init=False)
+    # A_v: float = field(init=False)
+    # A_e: float = field(init=False)
 
     def __post_init__(self):
         self.lam_ep, self.lam_ey, self.lam_eyc, _ = ring_element_slenderness_limit(
-            self.res_stress)
-        self.lam_e = float(self.d_o / self.t * (self.f_y/250))
-        self.lam_e_ratio = self.lam_e/self.lam_ey
+            self.res_stress
+        )
+        self.lam_e = float(self.d_o / self.t * (self.f_y / 250))
+        self.lam_e_ratio = self.lam_e / self.lam_ey
 
         # AS4100 Cl 6.2.4
-        self.d_e = self.d_o * min(1,
-                                  (self.lam_eyc / self.lam_e)**0.5,
-                                  (3 * self.lam_eyc / self.lam_e)**2)
+        self.d_e = self.d_o * min(
+            1, (self.lam_eyc / self.lam_e) ** 0.5, (3 * self.lam_eyc / self.lam_e) ** 2
+        )
 
         # NOTE: unsure if this is the correct effective area calculation
-        r_o = self.d_o/2
+        r_o = self.d_o / 2
         r_i = r_o - self.t
-        A_n = pi*(r_o + r_i) * (r_o - r_i)
+        A_n = pi * (r_o + r_i) * (r_o - r_i)
 
         r_e = self.d_e / 2
         r_ie = r_e - self.t
-        self.A_e = pi*(r_e + r_ie) * (r_e - r_ie)
+        self.A_e = pi * (r_e + r_ie) * (r_e - r_ie)
         self.A_v = A_n - self.A_e
 
 
 def main():
     from pathlib import Path
     import pandas as pd
+
     path = Path(__file__)
-    input_data = str(path.parent.parent)+'\\input_data\\AUS_open_sections.csv'
+    input_data = str(path.parent.parent) + "\\input_data\\AUS_open_sections.csv"
 
     section_df = pd.read_csv(input_data, skiprows=[1])
-    section_df = section_df.apply(pd.to_numeric, errors='ignore').fillna(0)
+    section_df = section_df.apply(pd.to_numeric, errors="ignore").fillna(0)
     section_dict = section_df.iloc[2].to_dict()
 
     geom = SectionGeometry._solve_new(section_dict)
     mat = SteelMaterial.from_dict(**section_dict)
 
     slenderness = SteelSlenderness(geom=geom, mat=mat)
-    print('\nSlenderness attributes for a given section, as per AS4100:')
+    print("\nSlenderness attributes for a given section, as per AS4100:")
     print(slenderness)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `steelas-0.1.2/src/steelas/shape/__pycache__/circularhollow.cpython-311.pyc` & `steelas-0.2.0/src/steelas/shape/__pycache__/circularhollow.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `steelas-0.1.2/src/steelas/shape/__pycache__/cshape.cpython-311.pyc` & `steelas-0.2.0/src/steelas/shape/__pycache__/cshape.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `steelas-0.1.2/src/steelas/shape/__pycache__/ishape.cpython-311.pyc` & `steelas-0.2.0/src/steelas/shape/__pycache__/ishape.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `steelas-0.1.2/src/steelas/shape/__pycache__/rectangleplate.cpython-311.pyc` & `steelas-0.2.0/src/steelas/shape/__pycache__/rectangleplate.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `steelas-0.1.2/src/steelas/shape/__pycache__/rectangularhollow.cpython-311.pyc` & `steelas-0.2.0/src/steelas/shape/__pycache__/rectangularhollow.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `steelas-0.1.2/src/steelas/shape/__pycache__/tshape.cpython-311.pyc` & `steelas-0.2.0/src/steelas/shape/__pycache__/tshape.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `steelas-0.1.2/src/steelas/shape/circularhollow.py` & `steelas-0.2.0/src/steelas/shape/circularhollow.py`

 * *Files identical despite different names*

### Comparing `steelas-0.1.2/src/steelas/shape/cshape.py` & `steelas-0.2.0/src/steelas/shape/cshape.py`

 * *Files identical despite different names*

### Comparing `steelas-0.1.2/src/steelas/shape/ishape.py` & `steelas-0.2.0/src/steelas/shape/ishape.py`

 * *Files identical despite different names*

### Comparing `steelas-0.1.2/src/steelas/shape/rectangleplate.py` & `steelas-0.2.0/src/steelas/shape/rectangleplate.py`

 * *Files identical despite different names*

### Comparing `steelas-0.1.2/src/steelas/shape/rectangularhollow.py` & `steelas-0.2.0/src/steelas/shape/rectangularhollow.py`

 * *Files identical despite different names*

### Comparing `steelas-0.1.2/src/steelas/shape/tshape.py` & `steelas-0.2.0/src/steelas/shape/tshape.py`

 * *Files identical despite different names*

### Comparing `steelas-0.1.2/src/steelas.egg-info/PKG-INFO` & `steelas-0.2.0/src/steelas.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: steelas
-Version: 0.1.2
+Version: 0.2.0
 Summary: steelas is a Python package for the design of steel structures to relevant Australian Standards
 Author-email: Joe Gattas <j.gattas@uq.edu.au>, Yuyu Wang <yuyu.wang@uq.net.au>
 Project-URL: Homepage, https://github.com/Folded-Structures-Lab/steel-as
 Keywords: AS4100,steel structures,structural engineering
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy>=1.25.0
 Requires-Dist: pandas>=2.0.2
 
 # About
 *steelas* is a Python package with tools to support research and design of Australian steel structures. It can be used to determine the material properties, section properties, and design capacities for structural members as per Australian Standard AS4100:2020 (Steel Structures).
```

### Comparing `steelas-0.1.2/src/steelas.egg-info/SOURCES.txt` & `steelas-0.2.0/src/steelas.egg-info/SOURCES.txt`

 * *Files 25% similar despite different names*

```diff
@@ -2,15 +2,19 @@
 MANIFEST.in
 README.md
 pyproject.toml
 docs/index.md
 docs/install.md
 docs/reference.md
 docs/tutorial-1.md
+docs/tutorial-2.md
+docs/tutorial-3.md
 examples/tutorial_1.py
+examples/tutorial_2.py
+examples/tutorial_3.py
 src/steelas/__init__.py
 src/steelas.egg-info/PKG-INFO
 src/steelas.egg-info/SOURCES.txt
 src/steelas.egg-info/dependency_links.txt
 src/steelas.egg-info/requires.txt
 src/steelas.egg-info/top_level.txt
 src/steelas/__pycache__/__init__.cpython-311.pyc
@@ -51,16 +55,19 @@
 src/steelas/member/member.py
 src/steelas/member/slenderness.py
 src/steelas/member/__pycache__/__init__.cpython-310.pyc
 src/steelas/member/__pycache__/__init__.cpython-311.pyc
 src/steelas/member/__pycache__/geometry.cpython-310.pyc
 src/steelas/member/__pycache__/geometry.cpython-311.pyc
 src/steelas/member/__pycache__/material.cpython-310.pyc
+src/steelas/member/__pycache__/material.cpython-311.pyc
 src/steelas/member/__pycache__/member.cpython-310.pyc
+src/steelas/member/__pycache__/member.cpython-311.pyc
 src/steelas/member/__pycache__/slenderness.cpython-310.pyc
+src/steelas/member/__pycache__/slenderness.cpython-311.pyc
 src/steelas/shape/__init__.py
 src/steelas/shape/circularhollow.py
 src/steelas/shape/cshape.py
 src/steelas/shape/ishape.py
 src/steelas/shape/rectangleplate.py
 src/steelas/shape/rectangularhollow.py
 src/steelas/shape/tshape.py
```

