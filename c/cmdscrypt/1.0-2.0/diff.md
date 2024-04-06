# Comparing `tmp/cmdscrypt-1.0.tar.gz` & `tmp/cmdscrypt-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmdscrypt-1.0.tar", last modified: Sat Jul 23 15:33:36 2022, max compression
+gzip compressed data, was "cmdscrypt-2.0.tar", last modified: Sat Apr  6 22:05:00 2024, max compression
```

## Comparing `cmdscrypt-1.0.tar` & `cmdscrypt-2.0.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxr-xr-x   0 non       (1000) non       (1000)        0 2022-07-23 15:33:36.686355 cmdscrypt-1.0/
--rw-r--r--   0 non       (1000) non       (1000)      358 2022-07-23 15:33:36.686355 cmdscrypt-1.0/PKG-INFO
--rw-r--r--   0 non       (1000) non       (1000)      316 2022-07-23 15:27:14.000000 cmdscrypt-1.0/README.md
-drwxr-xr-x   0 non       (1000) non       (1000)        0 2022-07-23 15:33:36.686355 cmdscrypt-1.0/cmdscrypt.egg-info/
--rw-r--r--   0 non       (1000) non       (1000)      358 2022-07-23 15:33:36.000000 cmdscrypt-1.0/cmdscrypt.egg-info/PKG-INFO
--rw-r--r--   0 non       (1000) non       (1000)      199 2022-07-23 15:33:36.000000 cmdscrypt-1.0/cmdscrypt.egg-info/SOURCES.txt
--rw-r--r--   0 non       (1000) non       (1000)        1 2022-07-23 15:33:36.000000 cmdscrypt-1.0/cmdscrypt.egg-info/dependency_links.txt
--rw-r--r--   0 non       (1000) non       (1000)       63 2022-07-23 15:33:36.000000 cmdscrypt-1.0/cmdscrypt.egg-info/entry_points.txt
--rw-r--r--   0 non       (1000) non       (1000)       10 2022-07-23 15:33:36.000000 cmdscrypt-1.0/cmdscrypt.egg-info/top_level.txt
--rwxr-x---   0 non       (1000) non       (1000)     1622 2022-07-23 12:11:14.000000 cmdscrypt-1.0/cmdscrypt.py
--rw-r--r--   0 non       (1000) non       (1000)       38 2022-07-23 15:33:36.686355 cmdscrypt-1.0/setup.cfg
--rw-r--r--   0 non       (1000) non       (1000)      496 2022-07-23 15:30:59.000000 cmdscrypt-1.0/setup.py
+drwxr-xr-x   0 non       (1000) non       (1000)        0 2024-04-06 22:05:00.416709 cmdscrypt-2.0/
+-rw-r--r--   0 non       (1000) non       (1000)      696 2024-04-06 22:05:00.416709 cmdscrypt-2.0/PKG-INFO
+-rw-r--r--   0 non       (1000) non       (1000)      368 2024-04-06 22:03:47.000000 cmdscrypt-2.0/README.md
+drwxr-xr-x   0 non       (1000) non       (1000)        0 2024-04-06 22:05:00.416709 cmdscrypt-2.0/cmdscrypt.egg-info/
+-rw-r--r--   0 non       (1000) non       (1000)      696 2024-04-06 22:05:00.000000 cmdscrypt-2.0/cmdscrypt.egg-info/PKG-INFO
+-rw-r--r--   0 non       (1000) non       (1000)      231 2024-04-06 22:05:00.000000 cmdscrypt-2.0/cmdscrypt.egg-info/SOURCES.txt
+-rw-r--r--   0 non       (1000) non       (1000)        1 2024-04-06 22:05:00.000000 cmdscrypt-2.0/cmdscrypt.egg-info/dependency_links.txt
+-rw-r--r--   0 non       (1000) non       (1000)       63 2024-04-06 22:05:00.000000 cmdscrypt-2.0/cmdscrypt.egg-info/entry_points.txt
+-rw-r--r--   0 non       (1000) non       (1000)       13 2024-04-06 22:05:00.000000 cmdscrypt-2.0/cmdscrypt.egg-info/requires.txt
+-rw-r--r--   0 non       (1000) non       (1000)       10 2024-04-06 22:05:00.000000 cmdscrypt-2.0/cmdscrypt.egg-info/top_level.txt
+-rwxrwx---   0 non       (1000) non       (1000)     6000 2024-04-03 20:49:21.000000 cmdscrypt-2.0/cmdscrypt.py
+-rw-r--r--   0 non       (1000) non       (1000)       38 2024-04-06 22:05:00.416709 cmdscrypt-2.0/setup.cfg
+-rw-r--r--   0 non       (1000) non       (1000)      729 2024-04-06 21:45:36.000000 cmdscrypt-2.0/setup.py
```

