# Comparing `tmp/discordanalytics-0.0.2.tar.gz` & `tmp/discordanalytics-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discordanalytics-0.0.2.tar", last modified: Sat Apr  6 18:30:20 2024, max compression
+gzip compressed data, was "discordanalytics-0.0.3.tar", last modified: Sat Apr  6 18:41:14 2024, max compression
```

## Comparing `discordanalytics-0.0.2.tar` & `discordanalytics-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-06 18:30:20.963501 discordanalytics-0.0.2/
--rw-rw-rw-   0        0        0     1095 2024-04-06 18:05:32.000000 discordanalytics-0.0.2/LICENSE
--rw-rw-rw-   0        0        0      386 2024-04-06 18:30:20.961501 discordanalytics-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      680 2024-04-06 16:58:50.000000 discordanalytics-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-06 18:30:20.895342 discordanalytics-0.0.2/discordanalytics/
--rw-rw-rw-   0        0        0      125 2024-04-06 17:54:05.000000 discordanalytics-0.0.2/discordanalytics/__init__.py
--rw-rw-rw-   0        0        0     7065 2024-04-06 17:13:40.000000 discordanalytics-0.0.2/discordanalytics/client.py
-drwxrwxrwx   0        0        0        0 2024-04-06 18:30:20.959501 discordanalytics-0.0.2/discordanalytics.egg-info/
--rw-rw-rw-   0        0        0      386 2024-04-06 18:30:20.000000 discordanalytics-0.0.2/discordanalytics.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      248 2024-04-06 18:30:20.000000 discordanalytics-0.0.2/discordanalytics.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-06 18:30:20.000000 discordanalytics-0.0.2/discordanalytics.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-04-06 18:30:20.000000 discordanalytics-0.0.2/discordanalytics.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      473 2024-04-06 18:29:40.000000 discordanalytics-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-06 18:30:20.963501 discordanalytics-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 18:41:14.417436 discordanalytics-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-06 18:41:09.000000 discordanalytics-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-04-06 18:41:14.417436 discordanalytics-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-06 18:41:09.000000 discordanalytics-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 18:41:14.413436 discordanalytics-0.0.3/discordanalytics/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-06 18:41:09.000000 discordanalytics-0.0.3/discordanalytics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6853 2024-04-06 18:41:09.000000 discordanalytics-0.0.3/discordanalytics/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 18:41:14.417436 discordanalytics-0.0.3/discordanalytics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-04-06 18:41:14.000000 discordanalytics-0.0.3/discordanalytics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-06 18:41:14.000000 discordanalytics-0.0.3/discordanalytics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 18:41:14.000000 discordanalytics-0.0.3/discordanalytics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-06 18:41:14.000000 discordanalytics-0.0.3/discordanalytics.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-04-06 18:41:09.000000 discordanalytics-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 18:41:14.417436 discordanalytics-0.0.3/setup.cfg
```

