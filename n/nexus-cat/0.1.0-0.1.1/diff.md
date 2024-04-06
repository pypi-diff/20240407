# Comparing `tmp/nexus-cat-0.1.0.tar.gz` & `tmp/nexus-cat-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nexus-cat-0.1.0.tar", last modified: Sat Apr  6 21:57:35 2024, max compression
+gzip compressed data, was "nexus-cat-0.1.1.tar", last modified: Sat Apr  6 22:10:49 2024, max compression
```

## Comparing `nexus-cat-0.1.0.tar` & `nexus-cat-0.1.1.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxrwxr-x   0 perraju   (1000) perraju   (1000)        0 2024-04-06 21:57:35.949027 nexus-cat-0.1.0/
--rw-rw-r--   0 perraju   (1000) perraju   (1000)     1076 2024-04-06 13:06:16.000000 nexus-cat-0.1.0/LICENSE
--rw-r--r--   0 perraju   (1000) perraju   (1000)      646 2024-04-06 21:57:35.949027 nexus-cat-0.1.0/PKG-INFO
--rw-rw-r--   0 perraju   (1000) perraju   (1000)     1617 2024-04-06 21:50:39.000000 nexus-cat-0.1.0/README.md
-drwxrwxr-x   0 perraju   (1000) perraju   (1000)        0 2024-04-06 21:57:35.945027 nexus-cat-0.1.0/archive/
--rw-rw-r--   0 perraju   (1000) perraju   (1000)        0 2023-11-25 17:34:16.000000 nexus-cat-0.1.0/archive/__init__.py
--rw-rw-r--   0 perraju   (1000) perraju   (1000)    20635 2024-03-23 11:29:43.000000 nexus-cat-0.1.0/archive/__main__.py
--rw-rw-r--   0 perraju   (1000) perraju   (1000)      283 2023-11-26 11:33:00.000000 nexus-cat-0.1.0/archive/setup.py
-drwxrwxr-x   0 perraju   (1000) perraju   (1000)        0 2024-04-06 21:57:35.945027 nexus-cat-0.1.0/archive/src/
--rw-rw-r--   0 perraju   (1000) perraju   (1000)        0 2023-11-25 17:34:16.000000 nexus-cat-0.1.0/archive/src/__init__.py
-drwxrwxr-x   0 perraju   (1000) perraju   (1000)        0 2024-04-06 21:57:35.945027 nexus-cat-0.1.0/archive/src/analysis/
--rw-rw-r--   0 perraju   (1000) perraju   (1000)        0 2023-11-25 17:34:16.000000 nexus-cat-0.1.0/archive/src/analysis/__init__.py
--rw-rw-r--   0 perraju   (1000) perraju   (1000)    13986 2024-03-23 11:29:43.000000 nexus-cat-0.1.0/archive/src/analysis/cluster_analyzer.py
--rw-rw-r--   0 perraju   (1000) perraju   (1000)     6956 2023-12-10 12:38:53.000000 nexus-cat-0.1.0/archive/src/analysis/percolation_analyzer.py
--rw-rw-r--   0 perraju   (1000) perraju   (1000)     3578 2023-11-25 17:34:16.000000 nexus-cat-0.1.0/archive/src/analysis/structural_analyzer.py
-drwxrwxr-x   0 perraju   (1000) perraju   (1000)        0 2024-04-06 21:57:35.945027 nexus-cat-0.1.0/archive/src/data/
--rw-rw-r--   0 perraju   (1000) perraju   (1000)     7530 2023-12-10 09:10:51.000000 nexus-cat-0.1.0/archive/src/data/__init__.py
-drwxrwxr-x   0 perraju   (1000) perraju   (1000)        0 2024-04-06 21:57:35.945027 nexus-cat-0.1.0/archive/src/io/
--rw-rw-r--   0 perraju   (1000) perraju   (1000)        0 2023-11-25 17:34:16.000000 nexus-cat-0.1.0/archive/src/io/__init__.py
--rw-rw-r--   0 perraju   (1000) perraju   (1000)        0 2023-11-25 17:34:16.000000 nexus-cat-0.1.0/archive/src/io/autodetect.py
--rw-rw-r--   0 perraju   (1000) perraju   (1000)    27489 2024-03-23 11:29:43.000000 nexus-cat-0.1.0/archive/src/io/build_fancy_recaps.py
--rw-rw-r--   0 perraju   (1000) perraju   (1000)        0 2023-11-25 17:34:16.000000 nexus-cat-0.1.0/archive/src/io/cp2k.py
--rw-rw-r--   0 perraju   (1000) perraju   (1000)        0 2023-11-25 17:34:16.000000 nexus-cat-0.1.0/archive/src/io/dftb.py
--rw-rw-r--   0 perraju   (1000) perraju   (1000)        0 2023-11-25 17:34:16.000000 nexus-cat-0.1.0/archive/src/io/dftb_old.py
--rw-rw-r--   0 perraju   (1000) perraju   (1000)        0 2023-11-25 17:34:16.000000 nexus-cat-0.1.0/archive/src/io/imd.py
--rw-rw-r--   0 perraju   (1000) perraju   (1000)     3275 2023-11-25 17:34:16.000000 nexus-cat-0.1.0/archive/src/io/lammps.py
--rw-rw-r--   0 perraju   (1000) perraju   (1000)     3619 2024-01-08 13:04:11.000000 nexus-cat-0.1.0/archive/src/io/xyz.py
-drwxrwxr-x   0 perraju   (1000) perraju   (1000)        0 2024-04-06 21:57:35.945027 nexus-cat-0.1.0/archive/src/settings/
--rw-rw-r--   0 perraju   (1000) perraju   (1000)        0 2023-11-25 17:34:16.000000 nexus-cat-0.1.0/archive/src/settings/__init__.py
--rw-rw-r--   0 perraju   (1000) perraju   (1000)     1234 2023-11-25 17:34:16.000000 nexus-cat-0.1.0/archive/src/settings/parameter.py
--rw-rw-r--   0 perraju   (1000) perraju   (1000)     1916 2023-11-25 17:34:16.000000 nexus-cat-0.1.0/archive/src/settings/parameter_file_reader.py
--rw-rw-r--   0 perraju   (1000) perraju   (1000)     1598 2023-11-25 17:34:16.000000 nexus-cat-0.1.0/archive/src/settings/settings.py
-drwxrwxr-x   0 perraju   (1000) perraju   (1000)        0 2024-04-06 21:57:35.945027 nexus-cat-0.1.0/archive/src/structure/
--rw-rw-r--   0 perraju   (1000) perraju   (1000)        0 2023-11-25 17:34:16.000000 nexus-cat-0.1.0/archive/src/structure/__init__.py
--rw-rw-r--   0 perraju   (1000) perraju   (1000)    12438 2024-02-21 10:29:20.000000 nexus-cat-0.1.0/archive/src/structure/atom.py
--rw-rw-r--   0 perraju   (1000) perraju   (1000)     1800 2024-01-08 13:04:11.000000 nexus-cat-0.1.0/archive/src/structure/box.py
--rw-rw-r--   0 perraju   (1000) perraju   (1000)     9461 2024-03-23 11:29:43.000000 nexus-cat-0.1.0/archive/src/structure/cluster.py
--rw-rw-r--   0 perraju   (1000) perraju   (1000)     8703 2024-03-23 13:25:34.000000 nexus-cat-0.1.0/archive/src/structure/neighbor.py
--rw-rw-r--   0 perraju   (1000) perraju   (1000)     9605 2024-01-08 13:04:11.000000 nexus-cat-0.1.0/archive/src/structure/system.py
-drwxrwxr-x   0 perraju   (1000) perraju   (1000)        0 2024-04-06 21:57:35.949027 nexus-cat-0.1.0/nexus/
--rw-rw-r--   0 perraju   (1000) perraju   (1000)      175 2024-04-06 21:13:47.000000 nexus-cat-0.1.0/nexus/__init__.py
-drwxrwxr-x   0 perraju   (1000) perraju   (1000)        0 2024-04-06 21:57:35.949027 nexus-cat-0.1.0/nexus/core/
--rw-rw-r--   0 perraju   (1000) perraju   (1000)      145 2024-04-06 20:39:23.000000 nexus-cat-0.1.0/nexus/core/__init__.py
--rw-rw-r--   0 perraju   (1000) perraju   (1000)     8816 2024-04-06 21:10:52.000000 nexus-cat-0.1.0/nexus/core/atom.py
--rw-rw-r--   0 perraju   (1000) perraju   (1000)     2616 2024-03-31 10:20:59.000000 nexus-cat-0.1.0/nexus/core/box.py
--rw-rw-r--   0 perraju   (1000) perraju   (1000)    14213 2024-04-06 20:40:34.000000 nexus-cat-0.1.0/nexus/core/cluster.py
--rw-rw-r--   0 perraju   (1000) perraju   (1000)     2141 2024-03-31 11:54:45.000000 nexus-cat-0.1.0/nexus/core/cutoff.py
--rw-rw-r--   0 perraju   (1000) perraju   (1000)    30889 2024-04-06 21:49:13.000000 nexus-cat-0.1.0/nexus/core/system.py
-drwxrwxr-x   0 perraju   (1000) perraju   (1000)        0 2024-04-06 21:57:35.949027 nexus-cat-0.1.0/nexus/data/
--rw-rw-r--   0 perraju   (1000) perraju   (1000)     7530 2024-03-31 11:07:05.000000 nexus-cat-0.1.0/nexus/data/__init__.py
-drwxrwxr-x   0 perraju   (1000) perraju   (1000)        0 2024-04-06 21:57:35.949027 nexus-cat-0.1.0/nexus/extensions/
--rw-rw-r--   0 perraju   (1000) perraju   (1000)     2021 2024-04-06 20:41:19.000000 nexus-cat-0.1.0/nexus/extensions/Na.py
--rw-rw-r--   0 perraju   (1000) perraju   (1000)    14516 2024-04-06 21:08:33.000000 nexus-cat-0.1.0/nexus/extensions/SiOz.py
--rw-rw-r--   0 perraju   (1000) perraju   (1000)       35 2024-04-06 21:21:46.000000 nexus-cat-0.1.0/nexus/extensions/__init__.py
-drwxrwxr-x   0 perraju   (1000) perraju   (1000)        0 2024-04-06 21:57:35.949027 nexus-cat-0.1.0/nexus/io/
--rw-rw-r--   0 perraju   (1000) perraju   (1000)      612 2024-04-06 20:42:58.000000 nexus-cat-0.1.0/nexus/io/__init__.py
--rw-rw-r--   0 perraju   (1000) perraju   (1000)      707 2024-04-05 12:20:44.000000 nexus-cat-0.1.0/nexus/io/make_lines_unique.py
--rw-rw-r--   0 perraju   (1000) perraju   (1000)     4761 2024-04-06 21:49:44.000000 nexus-cat-0.1.0/nexus/io/read_and_create_system.py
--rw-rw-r--   0 perraju   (1000) perraju   (1000)     1032 2024-03-31 11:09:48.000000 nexus-cat-0.1.0/nexus/io/read_lattices_properties.py
--rw-rw-r--   0 perraju   (1000) perraju   (1000)      662 2024-03-31 11:10:34.000000 nexus-cat-0.1.0/nexus/io/read_number_of_configurations.py
--rw-rw-r--   0 perraju   (1000) perraju   (1000)    29013 2024-04-06 20:42:35.000000 nexus-cat-0.1.0/nexus/io/result.py
--rw-rw-r--   0 perraju   (1000) perraju   (1000)      722 2024-04-05 17:39:46.000000 nexus-cat-0.1.0/nexus/io/write_list_of_files.py
--rw-rw-r--   0 perraju   (1000) perraju   (1000)    13679 2024-04-06 21:50:04.000000 nexus-cat-0.1.0/nexus/main.py
-drwxrwxr-x   0 perraju   (1000) perraju   (1000)        0 2024-04-06 21:57:35.949027 nexus-cat-0.1.0/nexus/settings/
--rw-rw-r--   0 perraju   (1000) perraju   (1000)       30 2024-04-06 20:43:10.000000 nexus-cat-0.1.0/nexus/settings/__init__.py
--rw-rw-r--   0 perraju   (1000) perraju   (1000)     5787 2024-04-05 17:06:57.000000 nexus-cat-0.1.0/nexus/settings/parameter.py
--rw-rw-r--   0 perraju   (1000) perraju   (1000)     9113 2024-04-06 21:49:55.000000 nexus-cat-0.1.0/nexus/settings/settings.py
-drwxrwxr-x   0 perraju   (1000) perraju   (1000)        0 2024-04-06 21:57:35.949027 nexus-cat-0.1.0/nexus/utils/
--rw-rw-r--   0 perraju   (1000) perraju   (1000)       97 2024-04-06 20:43:29.000000 nexus-cat-0.1.0/nexus/utils/__init__.py
--rw-rw-r--   0 perraju   (1000) perraju   (1000)     1150 2024-03-31 12:26:32.000000 nexus-cat-0.1.0/nexus/utils/generate_color_gradient.py
--rw-rw-r--   0 perraju   (1000) perraju   (1000)      944 2024-04-03 20:18:53.000000 nexus-cat-0.1.0/nexus/utils/print_title.py
-drwxrwxr-x   0 perraju   (1000) perraju   (1000)        0 2024-04-06 21:57:35.949027 nexus-cat-0.1.0/nexus_cat.egg-info/
--rw-r--r--   0 perraju   (1000) perraju   (1000)      646 2024-04-06 21:57:35.000000 nexus-cat-0.1.0/nexus_cat.egg-info/PKG-INFO
--rw-rw-r--   0 perraju   (1000) perraju   (1000)     1680 2024-04-06 21:57:35.000000 nexus-cat-0.1.0/nexus_cat.egg-info/SOURCES.txt
--rw-rw-r--   0 perraju   (1000) perraju   (1000)        1 2024-04-06 21:57:35.000000 nexus-cat-0.1.0/nexus_cat.egg-info/dependency_links.txt
--rw-rw-r--   0 perraju   (1000) perraju   (1000)       25 2024-04-06 21:57:35.000000 nexus-cat-0.1.0/nexus_cat.egg-info/requires.txt
--rw-rw-r--   0 perraju   (1000) perraju   (1000)       14 2024-04-06 21:57:35.000000 nexus-cat-0.1.0/nexus_cat.egg-info/top_level.txt
--rw-rw-r--   0 perraju   (1000) perraju   (1000)       38 2024-04-06 21:57:35.949027 nexus-cat-0.1.0/setup.cfg
--rw-rw-r--   0 perraju   (1000) perraju   (1000)      751 2024-04-06 21:56:35.000000 nexus-cat-0.1.0/setup.py
+drwxrwxr-x   0 perraju   (1000) perraju   (1000)        0 2024-04-06 22:10:49.627002 nexus-cat-0.1.1/
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)     1076 2024-04-06 13:06:16.000000 nexus-cat-0.1.1/LICENSE
+-rw-r--r--   0 perraju   (1000) perraju   (1000)      646 2024-04-06 22:10:49.627002 nexus-cat-0.1.1/PKG-INFO
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)     1613 2024-04-06 22:00:41.000000 nexus-cat-0.1.1/README.md
+drwxrwxr-x   0 perraju   (1000) perraju   (1000)        0 2024-04-06 22:10:49.623002 nexus-cat-0.1.1/archive/
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)        0 2023-11-25 17:34:16.000000 nexus-cat-0.1.1/archive/__init__.py
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)    20635 2024-03-23 11:29:43.000000 nexus-cat-0.1.1/archive/__main__.py
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)      283 2023-11-26 11:33:00.000000 nexus-cat-0.1.1/archive/setup.py
+drwxrwxr-x   0 perraju   (1000) perraju   (1000)        0 2024-04-06 22:10:49.623002 nexus-cat-0.1.1/archive/src/
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)        0 2023-11-25 17:34:16.000000 nexus-cat-0.1.1/archive/src/__init__.py
+drwxrwxr-x   0 perraju   (1000) perraju   (1000)        0 2024-04-06 22:10:49.623002 nexus-cat-0.1.1/archive/src/analysis/
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)        0 2023-11-25 17:34:16.000000 nexus-cat-0.1.1/archive/src/analysis/__init__.py
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)    13986 2024-03-23 11:29:43.000000 nexus-cat-0.1.1/archive/src/analysis/cluster_analyzer.py
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)     6956 2023-12-10 12:38:53.000000 nexus-cat-0.1.1/archive/src/analysis/percolation_analyzer.py
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)     3578 2023-11-25 17:34:16.000000 nexus-cat-0.1.1/archive/src/analysis/structural_analyzer.py
+drwxrwxr-x   0 perraju   (1000) perraju   (1000)        0 2024-04-06 22:10:49.623002 nexus-cat-0.1.1/archive/src/data/
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)     7530 2023-12-10 09:10:51.000000 nexus-cat-0.1.1/archive/src/data/__init__.py
+drwxrwxr-x   0 perraju   (1000) perraju   (1000)        0 2024-04-06 22:10:49.623002 nexus-cat-0.1.1/archive/src/io/
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)        0 2023-11-25 17:34:16.000000 nexus-cat-0.1.1/archive/src/io/__init__.py
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)        0 2023-11-25 17:34:16.000000 nexus-cat-0.1.1/archive/src/io/autodetect.py
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)    27489 2024-03-23 11:29:43.000000 nexus-cat-0.1.1/archive/src/io/build_fancy_recaps.py
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)        0 2023-11-25 17:34:16.000000 nexus-cat-0.1.1/archive/src/io/cp2k.py
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)        0 2023-11-25 17:34:16.000000 nexus-cat-0.1.1/archive/src/io/dftb.py
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)        0 2023-11-25 17:34:16.000000 nexus-cat-0.1.1/archive/src/io/dftb_old.py
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)        0 2023-11-25 17:34:16.000000 nexus-cat-0.1.1/archive/src/io/imd.py
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)     3275 2023-11-25 17:34:16.000000 nexus-cat-0.1.1/archive/src/io/lammps.py
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)     3619 2024-01-08 13:04:11.000000 nexus-cat-0.1.1/archive/src/io/xyz.py
+drwxrwxr-x   0 perraju   (1000) perraju   (1000)        0 2024-04-06 22:10:49.623002 nexus-cat-0.1.1/archive/src/settings/
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)        0 2023-11-25 17:34:16.000000 nexus-cat-0.1.1/archive/src/settings/__init__.py
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)     1234 2023-11-25 17:34:16.000000 nexus-cat-0.1.1/archive/src/settings/parameter.py
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)     1916 2023-11-25 17:34:16.000000 nexus-cat-0.1.1/archive/src/settings/parameter_file_reader.py
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)     1598 2023-11-25 17:34:16.000000 nexus-cat-0.1.1/archive/src/settings/settings.py
+drwxrwxr-x   0 perraju   (1000) perraju   (1000)        0 2024-04-06 22:10:49.623002 nexus-cat-0.1.1/archive/src/structure/
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)        0 2023-11-25 17:34:16.000000 nexus-cat-0.1.1/archive/src/structure/__init__.py
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)    12438 2024-02-21 10:29:20.000000 nexus-cat-0.1.1/archive/src/structure/atom.py
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)     1800 2024-01-08 13:04:11.000000 nexus-cat-0.1.1/archive/src/structure/box.py
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)     9461 2024-03-23 11:29:43.000000 nexus-cat-0.1.1/archive/src/structure/cluster.py
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)     8703 2024-03-23 13:25:34.000000 nexus-cat-0.1.1/archive/src/structure/neighbor.py
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)     9605 2024-01-08 13:04:11.000000 nexus-cat-0.1.1/archive/src/structure/system.py
+drwxrwxr-x   0 perraju   (1000) perraju   (1000)        0 2024-04-06 22:10:49.623002 nexus-cat-0.1.1/nexus/
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)      175 2024-04-06 22:05:53.000000 nexus-cat-0.1.1/nexus/__init__.py
+drwxrwxr-x   0 perraju   (1000) perraju   (1000)        0 2024-04-06 22:10:49.627002 nexus-cat-0.1.1/nexus/core/
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)      145 2024-04-06 20:39:23.000000 nexus-cat-0.1.1/nexus/core/__init__.py
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)     8816 2024-04-06 21:10:52.000000 nexus-cat-0.1.1/nexus/core/atom.py
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)     2616 2024-03-31 10:20:59.000000 nexus-cat-0.1.1/nexus/core/box.py
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)    14213 2024-04-06 20:40:34.000000 nexus-cat-0.1.1/nexus/core/cluster.py
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)     2141 2024-03-31 11:54:45.000000 nexus-cat-0.1.1/nexus/core/cutoff.py
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)    30889 2024-04-06 21:49:13.000000 nexus-cat-0.1.1/nexus/core/system.py
+drwxrwxr-x   0 perraju   (1000) perraju   (1000)        0 2024-04-06 22:10:49.627002 nexus-cat-0.1.1/nexus/data/
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)     7530 2024-03-31 11:07:05.000000 nexus-cat-0.1.1/nexus/data/__init__.py
+drwxrwxr-x   0 perraju   (1000) perraju   (1000)        0 2024-04-06 22:10:49.627002 nexus-cat-0.1.1/nexus/extensions/
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)     2021 2024-04-06 20:41:19.000000 nexus-cat-0.1.1/nexus/extensions/Na.py
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)    14516 2024-04-06 21:08:33.000000 nexus-cat-0.1.1/nexus/extensions/SiOz.py
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)       35 2024-04-06 21:21:46.000000 nexus-cat-0.1.1/nexus/extensions/__init__.py
+drwxrwxr-x   0 perraju   (1000) perraju   (1000)        0 2024-04-06 22:10:49.627002 nexus-cat-0.1.1/nexus/io/
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)      612 2024-04-06 20:42:58.000000 nexus-cat-0.1.1/nexus/io/__init__.py
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)      707 2024-04-05 12:20:44.000000 nexus-cat-0.1.1/nexus/io/make_lines_unique.py
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)     4761 2024-04-06 21:49:44.000000 nexus-cat-0.1.1/nexus/io/read_and_create_system.py
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)     1032 2024-03-31 11:09:48.000000 nexus-cat-0.1.1/nexus/io/read_lattices_properties.py
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)      662 2024-03-31 11:10:34.000000 nexus-cat-0.1.1/nexus/io/read_number_of_configurations.py
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)    29013 2024-04-06 20:42:35.000000 nexus-cat-0.1.1/nexus/io/result.py
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)      722 2024-04-05 17:39:46.000000 nexus-cat-0.1.1/nexus/io/write_list_of_files.py
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)    13679 2024-04-06 21:50:04.000000 nexus-cat-0.1.1/nexus/main.py
+drwxrwxr-x   0 perraju   (1000) perraju   (1000)        0 2024-04-06 22:10:49.627002 nexus-cat-0.1.1/nexus/settings/
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)       30 2024-04-06 20:43:10.000000 nexus-cat-0.1.1/nexus/settings/__init__.py
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)     5787 2024-04-05 17:06:57.000000 nexus-cat-0.1.1/nexus/settings/parameter.py
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)     9113 2024-04-06 21:49:55.000000 nexus-cat-0.1.1/nexus/settings/settings.py
+drwxrwxr-x   0 perraju   (1000) perraju   (1000)        0 2024-04-06 22:10:49.627002 nexus-cat-0.1.1/nexus/utils/
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)       97 2024-04-06 20:43:29.000000 nexus-cat-0.1.1/nexus/utils/__init__.py
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)     1150 2024-03-31 12:26:32.000000 nexus-cat-0.1.1/nexus/utils/generate_color_gradient.py
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)      927 2024-04-06 22:08:51.000000 nexus-cat-0.1.1/nexus/utils/print_title.py
+drwxrwxr-x   0 perraju   (1000) perraju   (1000)        0 2024-04-06 22:10:49.627002 nexus-cat-0.1.1/nexus_cat.egg-info/
+-rw-r--r--   0 perraju   (1000) perraju   (1000)      646 2024-04-06 22:10:49.000000 nexus-cat-0.1.1/nexus_cat.egg-info/PKG-INFO
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)     1680 2024-04-06 22:10:49.000000 nexus-cat-0.1.1/nexus_cat.egg-info/SOURCES.txt
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)        1 2024-04-06 22:10:49.000000 nexus-cat-0.1.1/nexus_cat.egg-info/dependency_links.txt
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)       25 2024-04-06 22:10:49.000000 nexus-cat-0.1.1/nexus_cat.egg-info/requires.txt
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)       14 2024-04-06 22:10:49.000000 nexus-cat-0.1.1/nexus_cat.egg-info/top_level.txt
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)       38 2024-04-06 22:10:49.627002 nexus-cat-0.1.1/setup.cfg
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)      751 2024-04-06 22:10:06.000000 nexus-cat-0.1.1/setup.py
```

### Comparing `nexus-cat-0.1.0/LICENSE` & `nexus-cat-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nexus-cat-0.1.0/PKG-INFO` & `nexus-cat-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nexus-cat
-Version: 0.1.0
+Version: 0.1.1
 Summary: Nexus is a Cluster Analysing Toolkit package for atomic systems.
 Home-page: https://github.com/JulienPerradin/nexus
 Author: Julien Perradin
 Author-email: julien.perradin@umontpellier.fr
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `nexus-cat-0.1.0/README.md` & `nexus-cat-0.1.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 `nexus-cat` is a package designed to find clusters of connected polyhedra in an atomistic simulation trajectory. It provides functionality to analyze properties of the clusters such as the average cluster size, biggest cluster, gyration radius, and correlation length.
 
 ## Installation
 
 To install `nexus-cat`, first clone this repository as you please, for example with SSH:
 
 ```bash
-git clone git@github.com:JulienPerradin/nexus-cat.git
+git clone git@github.com:JulienPerradin/nexus.git
 ```
 Then you can use pip, it will install dependencies and the main package in your Python environment:
 
 ```bash
 pip install nexus-cat
 ```
```

### Comparing `nexus-cat-0.1.0/archive/__main__.py` & `nexus-cat-0.1.1/archive/__main__.py`

 * *Files identical despite different names*

### Comparing `nexus-cat-0.1.0/archive/src/analysis/cluster_analyzer.py` & `nexus-cat-0.1.1/archive/src/analysis/cluster_analyzer.py`

 * *Files identical despite different names*

### Comparing `nexus-cat-0.1.0/archive/src/analysis/percolation_analyzer.py` & `nexus-cat-0.1.1/archive/src/analysis/percolation_analyzer.py`

 * *Files identical despite different names*

### Comparing `nexus-cat-0.1.0/archive/src/analysis/structural_analyzer.py` & `nexus-cat-0.1.1/archive/src/analysis/structural_analyzer.py`

 * *Files identical despite different names*

### Comparing `nexus-cat-0.1.0/archive/src/data/__init__.py` & `nexus-cat-0.1.1/archive/src/data/__init__.py`

 * *Files identical despite different names*

### Comparing `nexus-cat-0.1.0/archive/src/io/build_fancy_recaps.py` & `nexus-cat-0.1.1/archive/src/io/build_fancy_recaps.py`

 * *Files identical despite different names*

### Comparing `nexus-cat-0.1.0/archive/src/io/lammps.py` & `nexus-cat-0.1.1/archive/src/io/lammps.py`

 * *Files identical despite different names*

### Comparing `nexus-cat-0.1.0/archive/src/io/xyz.py` & `nexus-cat-0.1.1/archive/src/io/xyz.py`

 * *Files identical despite different names*

### Comparing `nexus-cat-0.1.0/archive/src/settings/parameter.py` & `nexus-cat-0.1.1/archive/src/settings/parameter.py`

 * *Files identical despite different names*

### Comparing `nexus-cat-0.1.0/archive/src/settings/parameter_file_reader.py` & `nexus-cat-0.1.1/archive/src/settings/parameter_file_reader.py`

 * *Files identical despite different names*

### Comparing `nexus-cat-0.1.0/archive/src/settings/settings.py` & `nexus-cat-0.1.1/archive/src/settings/settings.py`

 * *Files identical despite different names*

### Comparing `nexus-cat-0.1.0/archive/src/structure/atom.py` & `nexus-cat-0.1.1/archive/src/structure/atom.py`

 * *Files identical despite different names*

### Comparing `nexus-cat-0.1.0/archive/src/structure/box.py` & `nexus-cat-0.1.1/archive/src/structure/box.py`

 * *Files identical despite different names*

### Comparing `nexus-cat-0.1.0/archive/src/structure/cluster.py` & `nexus-cat-0.1.1/archive/src/structure/cluster.py`

 * *Files identical despite different names*

### Comparing `nexus-cat-0.1.0/archive/src/structure/neighbor.py` & `nexus-cat-0.1.1/archive/src/structure/neighbor.py`

 * *Files identical despite different names*

### Comparing `nexus-cat-0.1.0/archive/src/structure/system.py` & `nexus-cat-0.1.1/archive/src/structure/system.py`

 * *Files identical despite different names*

### Comparing `nexus-cat-0.1.0/nexus/core/atom.py` & `nexus-cat-0.1.1/nexus/core/atom.py`

 * *Files identical despite different names*

### Comparing `nexus-cat-0.1.0/nexus/core/box.py` & `nexus-cat-0.1.1/nexus/core/box.py`

 * *Files identical despite different names*

### Comparing `nexus-cat-0.1.0/nexus/core/cluster.py` & `nexus-cat-0.1.1/nexus/core/cluster.py`

 * *Files identical despite different names*

### Comparing `nexus-cat-0.1.0/nexus/core/cutoff.py` & `nexus-cat-0.1.1/nexus/core/cutoff.py`

 * *Files identical despite different names*

### Comparing `nexus-cat-0.1.0/nexus/core/system.py` & `nexus-cat-0.1.1/nexus/core/system.py`

 * *Files identical despite different names*

### Comparing `nexus-cat-0.1.0/nexus/data/__init__.py` & `nexus-cat-0.1.1/nexus/data/__init__.py`

 * *Files identical despite different names*

### Comparing `nexus-cat-0.1.0/nexus/extensions/Na.py` & `nexus-cat-0.1.1/nexus/extensions/Na.py`

 * *Files identical despite different names*

### Comparing `nexus-cat-0.1.0/nexus/extensions/SiOz.py` & `nexus-cat-0.1.1/nexus/extensions/SiOz.py`

 * *Files identical despite different names*

### Comparing `nexus-cat-0.1.0/nexus/io/__init__.py` & `nexus-cat-0.1.1/nexus/io/__init__.py`

 * *Files identical despite different names*

### Comparing `nexus-cat-0.1.0/nexus/io/make_lines_unique.py` & `nexus-cat-0.1.1/nexus/io/make_lines_unique.py`

 * *Files identical despite different names*

### Comparing `nexus-cat-0.1.0/nexus/io/read_and_create_system.py` & `nexus-cat-0.1.1/nexus/io/read_and_create_system.py`

 * *Files identical despite different names*

### Comparing `nexus-cat-0.1.0/nexus/io/read_lattices_properties.py` & `nexus-cat-0.1.1/nexus/io/read_lattices_properties.py`

 * *Files identical despite different names*

### Comparing `nexus-cat-0.1.0/nexus/io/read_number_of_configurations.py` & `nexus-cat-0.1.1/nexus/io/read_number_of_configurations.py`

 * *Files identical despite different names*

### Comparing `nexus-cat-0.1.0/nexus/io/result.py` & `nexus-cat-0.1.1/nexus/io/result.py`

 * *Files identical despite different names*

### Comparing `nexus-cat-0.1.0/nexus/io/write_list_of_files.py` & `nexus-cat-0.1.1/nexus/io/write_list_of_files.py`

 * *Files identical despite different names*

### Comparing `nexus-cat-0.1.0/nexus/main.py` & `nexus-cat-0.1.1/nexus/main.py`

 * *Files identical despite different names*

### Comparing `nexus-cat-0.1.0/nexus/settings/parameter.py` & `nexus-cat-0.1.1/nexus/settings/parameter.py`

 * *Files identical despite different names*

### Comparing `nexus-cat-0.1.0/nexus/settings/settings.py` & `nexus-cat-0.1.1/nexus/settings/settings.py`

 * *Files identical despite different names*

### Comparing `nexus-cat-0.1.0/nexus/utils/generate_color_gradient.py` & `nexus-cat-0.1.1/nexus/utils/generate_color_gradient.py`

 * *Files identical despite different names*

### Comparing `nexus-cat-0.1.0/nexus/utils/print_title.py` & `nexus-cat-0.1.1/nexus/utils/print_title.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,22 +3,22 @@
     Prints the title and the version of the package.
     
     Returns:
     --------
       - None.
     """
     title = r'''
-                                                           
-                                                           
-      .g8"""bgd `7MMF'       .M"""bgd MMP""MM""YMM `7MM"""Mq.  
-    .dP'     `M   MM        ,MI    "Y P'   MM   `7   MM   `MM. 
-    dM'       `   MM        `MMb.          MM        MM   ,M9  
-    MM            MM          `YMMNq.      MM        MMmmdM9   
-    MM.           MM      , .     `MM      MM        MM  YM.   
-    `Mb.     ,'   MM     ,M Mb     dM      MM        MM   `Mb. 
-      `"bmmmd'  .JMMmmmmMMM P"Ybmmd"     .JMML.    .JMML. .JMM.
-                                                           
-                                                           
+                                                            
+                                                            
+`7MN.   `7MF'`7MM"""YMM  `YMM'   `MP'`7MMF'   `7MF'.M"""bgd 
+  MMN.    M    MM    `7    VMb.  ,P    MM       M ,MI    "Y 
+  M YMb   M    MM   d       `MM.M'     MM       M `MMb.     
+  M  `MN. M    MMmmMM         MMb      MM       M   `YMMNq. 
+  M   `MM.M    MM   Y  ,    ,M'`Mb.    MM       M .     `MM 
+  M     YMM    MM     ,M   ,P   `MM.   YM.     ,M Mb     dM 
+.JML.    YM  .JMMmmmmMMM .MM:.  .:MMa.  `bmmmmd"' P"Ybmmd"  
+                                                            
+                                                            
     '''
     print(title)
     print(f"__version__ \u279c\t {__version__}\n")
     return
```

### Comparing `nexus-cat-0.1.0/nexus_cat.egg-info/PKG-INFO` & `nexus-cat-0.1.1/nexus_cat.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nexus-cat
-Version: 0.1.0
+Version: 0.1.1
 Summary: Nexus is a Cluster Analysing Toolkit package for atomic systems.
 Home-page: https://github.com/JulienPerradin/nexus
 Author: Julien Perradin
 Author-email: julien.perradin@umontpellier.fr
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `nexus-cat-0.1.0/nexus_cat.egg-info/SOURCES.txt` & `nexus-cat-0.1.1/nexus_cat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nexus-cat-0.1.0/setup.py` & `nexus-cat-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='nexus-cat',
-    version='0.1.0',
+    version='0.1.1',
     description='Nexus is a Cluster Analysing Toolkit package for atomic systems.',
     author='Julien Perradin',
     author_email='julien.perradin@umontpellier.fr',
     url='https://github.com/JulienPerradin/nexus',
     packages=find_packages(),
     install_requires=[
         'numpy',
```

