# Comparing `tmp/azure-mgmt-hdinsightcontainers-1.0.0b1.tar.gz` & `tmp/azure-mgmt-hdinsightcontainers-1.0.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "azure-mgmt-hdinsightcontainers-1.0.0b1.tar", last modified: Tue Aug 22 04:59:56 2023, max compression
+gzip compressed data, was "azure-mgmt-hdinsightcontainers-1.0.0b2.tar", last modified: Sun Apr  7 03:34:25 2024, max compression
```

## Comparing `azure-mgmt-hdinsightcontainers-1.0.0b1.tar` & `azure-mgmt-hdinsightcontainers-1.0.0b2.tar`

### file list

```diff
@@ -1,59 +1,63 @@
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-08-22 04:59:56.279952 azure-mgmt-hdinsightcontainers-1.0.0b1/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       62 2023-08-22 04:58:58.000000 azure-mgmt-hdinsightcontainers-1.0.0b1/CHANGELOG.md
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1074 2023-08-22 04:58:58.000000 azure-mgmt-hdinsightcontainers-1.0.0b1/LICENSE
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      225 2023-08-22 04:58:58.000000 azure-mgmt-hdinsightcontainers-1.0.0b1/MANIFEST.in
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3191 2023-08-22 04:59:56.279952 azure-mgmt-hdinsightcontainers-1.0.0b1/PKG-INFO
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2216 2023-08-22 04:58:58.000000 azure-mgmt-hdinsightcontainers-1.0.0b1/README.md
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      696 2023-08-22 04:58:58.000000 azure-mgmt-hdinsightcontainers-1.0.0b1/_meta.json
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-08-22 04:59:56.275952 azure-mgmt-hdinsightcontainers-1.0.0b1/azure/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       65 2023-08-22 04:58:58.000000 azure-mgmt-hdinsightcontainers-1.0.0b1/azure/__init__.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-08-22 04:59:56.275952 azure-mgmt-hdinsightcontainers-1.0.0b1/azure/mgmt/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       65 2023-08-22 04:58:58.000000 azure-mgmt-hdinsightcontainers-1.0.0b1/azure/mgmt/__init__.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-08-22 04:59:56.275952 azure-mgmt-hdinsightcontainers-1.0.0b1/azure/mgmt/hdinsightcontainers/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      929 2023-08-22 04:58:58.000000 azure-mgmt-hdinsightcontainers-1.0.0b1/azure/mgmt/hdinsightcontainers/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3562 2023-08-22 04:58:58.000000 azure-mgmt-hdinsightcontainers-1.0.0b1/azure/mgmt/hdinsightcontainers/_configuration.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6109 2023-08-22 04:58:58.000000 azure-mgmt-hdinsightcontainers-1.0.0b1/azure/mgmt/hdinsightcontainers/_hd_insight_containers_mgmt_client.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2023-08-22 04:58:58.000000 azure-mgmt-hdinsightcontainers-1.0.0b1/azure/mgmt/hdinsightcontainers/_patch.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    79289 2023-08-22 04:58:58.000000 azure-mgmt-hdinsightcontainers-1.0.0b1/azure/mgmt/hdinsightcontainers/_serialization.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      778 2023-08-22 04:58:58.000000 azure-mgmt-hdinsightcontainers-1.0.0b1/azure/mgmt/hdinsightcontainers/_vendor.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      488 2023-08-22 04:58:58.000000 azure-mgmt-hdinsightcontainers-1.0.0b1/azure/mgmt/hdinsightcontainers/_version.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-08-22 04:59:56.275952 azure-mgmt-hdinsightcontainers-1.0.0b1/azure/mgmt/hdinsightcontainers/aio/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      876 2023-08-22 04:58:58.000000 azure-mgmt-hdinsightcontainers-1.0.0b1/azure/mgmt/hdinsightcontainers/aio/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3610 2023-08-22 04:58:58.000000 azure-mgmt-hdinsightcontainers-1.0.0b1/azure/mgmt/hdinsightcontainers/aio/_configuration.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6269 2023-08-22 04:58:58.000000 azure-mgmt-hdinsightcontainers-1.0.0b1/azure/mgmt/hdinsightcontainers/aio/_hd_insight_containers_mgmt_client.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2023-08-22 04:58:58.000000 azure-mgmt-hdinsightcontainers-1.0.0b1/azure/mgmt/hdinsightcontainers/aio/_patch.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-08-22 04:59:56.279952 azure-mgmt-hdinsightcontainers-1.0.0b1/azure/mgmt/hdinsightcontainers/aio/operations/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1374 2023-08-22 04:58:58.000000 azure-mgmt-hdinsightcontainers-1.0.0b1/azure/mgmt/hdinsightcontainers/aio/operations/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6293 2023-08-22 04:58:58.000000 azure-mgmt-hdinsightcontainers-1.0.0b1/azure/mgmt/hdinsightcontainers/aio/operations/_available_cluster_pool_versions_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6250 2023-08-22 04:58:58.000000 azure-mgmt-hdinsightcontainers-1.0.0b1/azure/mgmt/hdinsightcontainers/aio/operations/_available_cluster_versions_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    18375 2023-08-22 04:58:58.000000 azure-mgmt-hdinsightcontainers-1.0.0b1/azure/mgmt/hdinsightcontainers/aio/operations/_cluster_jobs_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    41009 2023-08-22 04:58:58.000000 azure-mgmt-hdinsightcontainers-1.0.0b1/azure/mgmt/hdinsightcontainers/aio/operations/_cluster_pools_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    62662 2023-08-22 04:58:58.000000 azure-mgmt-hdinsightcontainers-1.0.0b1/azure/mgmt/hdinsightcontainers/aio/operations/_clusters_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     7945 2023-08-22 04:58:58.000000 azure-mgmt-hdinsightcontainers-1.0.0b1/azure/mgmt/hdinsightcontainers/aio/operations/_locations_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5785 2023-08-22 04:58:58.000000 azure-mgmt-hdinsightcontainers-1.0.0b1/azure/mgmt/hdinsightcontainers/aio/operations/_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2023-08-22 04:58:58.000000 azure-mgmt-hdinsightcontainers-1.0.0b1/azure/mgmt/hdinsightcontainers/aio/operations/_patch.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-08-22 04:59:56.279952 azure-mgmt-hdinsightcontainers-1.0.0b1/azure/mgmt/hdinsightcontainers/models/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     8863 2023-08-22 04:58:58.000000 azure-mgmt-hdinsightcontainers-1.0.0b1/azure/mgmt/hdinsightcontainers/models/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3584 2023-08-22 04:58:58.000000 azure-mgmt-hdinsightcontainers-1.0.0b1/azure/mgmt/hdinsightcontainers/models/_hd_insight_containers_mgmt_client_enums.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)   177321 2023-08-22 04:58:58.000000 azure-mgmt-hdinsightcontainers-1.0.0b1/azure/mgmt/hdinsightcontainers/models/_models_py3.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2023-08-22 04:58:58.000000 azure-mgmt-hdinsightcontainers-1.0.0b1/azure/mgmt/hdinsightcontainers/models/_patch.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-08-22 04:59:56.279952 azure-mgmt-hdinsightcontainers-1.0.0b1/azure/mgmt/hdinsightcontainers/operations/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1374 2023-08-22 04:58:58.000000 azure-mgmt-hdinsightcontainers-1.0.0b1/azure/mgmt/hdinsightcontainers/operations/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     7396 2023-08-22 04:58:58.000000 azure-mgmt-hdinsightcontainers-1.0.0b1/azure/mgmt/hdinsightcontainers/operations/_available_cluster_pool_versions_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     7354 2023-08-22 04:58:58.000000 azure-mgmt-hdinsightcontainers-1.0.0b1/azure/mgmt/hdinsightcontainers/operations/_available_cluster_versions_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    21285 2023-08-22 04:58:58.000000 azure-mgmt-hdinsightcontainers-1.0.0b1/azure/mgmt/hdinsightcontainers/operations/_cluster_jobs_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    48501 2023-08-22 04:58:58.000000 azure-mgmt-hdinsightcontainers-1.0.0b1/azure/mgmt/hdinsightcontainers/operations/_cluster_pools_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    75789 2023-08-22 04:58:58.000000 azure-mgmt-hdinsightcontainers-1.0.0b1/azure/mgmt/hdinsightcontainers/operations/_clusters_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     9323 2023-08-22 04:58:58.000000 azure-mgmt-hdinsightcontainers-1.0.0b1/azure/mgmt/hdinsightcontainers/operations/_locations_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6485 2023-08-22 04:58:58.000000 azure-mgmt-hdinsightcontainers-1.0.0b1/azure/mgmt/hdinsightcontainers/operations/_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2023-08-22 04:58:58.000000 azure-mgmt-hdinsightcontainers-1.0.0b1/azure/mgmt/hdinsightcontainers/operations/_patch.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       26 2023-08-22 04:58:58.000000 azure-mgmt-hdinsightcontainers-1.0.0b1/azure/mgmt/hdinsightcontainers/py.typed
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-08-22 04:59:56.279952 azure-mgmt-hdinsightcontainers-1.0.0b1/azure_mgmt_hdinsightcontainers.egg-info/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3191 2023-08-22 04:59:56.000000 azure-mgmt-hdinsightcontainers-1.0.0b1/azure_mgmt_hdinsightcontainers.egg-info/PKG-INFO
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2508 2023-08-22 04:59:56.000000 azure-mgmt-hdinsightcontainers-1.0.0b1/azure_mgmt_hdinsightcontainers.egg-info/SOURCES.txt
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        1 2023-08-22 04:59:56.000000 azure-mgmt-hdinsightcontainers-1.0.0b1/azure_mgmt_hdinsightcontainers.egg-info/dependency_links.txt
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        1 2023-08-22 04:59:56.000000 azure-mgmt-hdinsightcontainers-1.0.0b1/azure_mgmt_hdinsightcontainers.egg-info/not-zip-safe
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      124 2023-08-22 04:59:56.000000 azure-mgmt-hdinsightcontainers-1.0.0b1/azure_mgmt_hdinsightcontainers.egg-info/requires.txt
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        6 2023-08-22 04:59:56.000000 azure-mgmt-hdinsightcontainers-1.0.0b1/azure_mgmt_hdinsightcontainers.egg-info/top_level.txt
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       38 2023-08-22 04:59:56.279952 azure-mgmt-hdinsightcontainers-1.0.0b1/setup.cfg
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2864 2023-08-22 04:58:58.000000 azure-mgmt-hdinsightcontainers-1.0.0b1/setup.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-07 03:34:25.165396 azure-mgmt-hdinsightcontainers-1.0.0b2/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5504 2024-04-07 03:33:17.000000 azure-mgmt-hdinsightcontainers-1.0.0b2/CHANGELOG.md
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1074 2024-04-07 03:33:17.000000 azure-mgmt-hdinsightcontainers-1.0.0b2/LICENSE
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      225 2024-04-07 03:33:17.000000 azure-mgmt-hdinsightcontainers-1.0.0b2/MANIFEST.in
+-rw-r--r--   0 cloudtest  (1000) cloudtest  (1000)     8586 2024-04-07 03:34:25.165396 azure-mgmt-hdinsightcontainers-1.0.0b2/PKG-INFO
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2067 2024-04-07 03:33:17.000000 azure-mgmt-hdinsightcontainers-1.0.0b2/README.md
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      728 2024-04-07 03:33:17.000000 azure-mgmt-hdinsightcontainers-1.0.0b2/_meta.json
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-07 03:34:25.157395 azure-mgmt-hdinsightcontainers-1.0.0b2/azure/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       65 2024-04-07 03:33:17.000000 azure-mgmt-hdinsightcontainers-1.0.0b2/azure/__init__.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-07 03:34:25.157395 azure-mgmt-hdinsightcontainers-1.0.0b2/azure/mgmt/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       65 2024-04-07 03:33:17.000000 azure-mgmt-hdinsightcontainers-1.0.0b2/azure/mgmt/__init__.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-07 03:34:25.157395 azure-mgmt-hdinsightcontainers-1.0.0b2/azure/mgmt/hdinsightcontainers/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      929 2024-04-07 03:33:17.000000 azure-mgmt-hdinsightcontainers-1.0.0b2/azure/mgmt/hdinsightcontainers/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3494 2024-04-07 03:33:17.000000 azure-mgmt-hdinsightcontainers-1.0.0b2/azure/mgmt/hdinsightcontainers/_configuration.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     8016 2024-04-07 03:33:17.000000 azure-mgmt-hdinsightcontainers-1.0.0b2/azure/mgmt/hdinsightcontainers/_hd_insight_containers_mgmt_client.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-04-07 03:33:17.000000 azure-mgmt-hdinsightcontainers-1.0.0b2/azure/mgmt/hdinsightcontainers/_patch.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    78873 2024-04-07 03:33:17.000000 azure-mgmt-hdinsightcontainers-1.0.0b2/azure/mgmt/hdinsightcontainers/_serialization.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      778 2024-04-07 03:33:17.000000 azure-mgmt-hdinsightcontainers-1.0.0b2/azure/mgmt/hdinsightcontainers/_vendor.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      488 2024-04-07 03:33:17.000000 azure-mgmt-hdinsightcontainers-1.0.0b2/azure/mgmt/hdinsightcontainers/_version.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-07 03:34:25.157395 azure-mgmt-hdinsightcontainers-1.0.0b2/azure/mgmt/hdinsightcontainers/aio/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      876 2024-04-07 03:33:17.000000 azure-mgmt-hdinsightcontainers-1.0.0b2/azure/mgmt/hdinsightcontainers/aio/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3542 2024-04-07 03:33:17.000000 azure-mgmt-hdinsightcontainers-1.0.0b2/azure/mgmt/hdinsightcontainers/aio/_configuration.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     8208 2024-04-07 03:33:17.000000 azure-mgmt-hdinsightcontainers-1.0.0b2/azure/mgmt/hdinsightcontainers/aio/_hd_insight_containers_mgmt_client.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-04-07 03:33:17.000000 azure-mgmt-hdinsightcontainers-1.0.0b2/azure/mgmt/hdinsightcontainers/aio/_patch.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-07 03:34:25.161396 azure-mgmt-hdinsightcontainers-1.0.0b2/azure/mgmt/hdinsightcontainers/aio/operations/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1645 2024-04-07 03:33:17.000000 azure-mgmt-hdinsightcontainers-1.0.0b2/azure/mgmt/hdinsightcontainers/aio/operations/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5988 2024-04-07 03:33:17.000000 azure-mgmt-hdinsightcontainers-1.0.0b2/azure/mgmt/hdinsightcontainers/aio/operations/_available_cluster_pool_versions_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5949 2024-04-07 03:33:17.000000 azure-mgmt-hdinsightcontainers-1.0.0b2/azure/mgmt/hdinsightcontainers/aio/operations/_available_cluster_versions_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6415 2024-04-07 03:33:17.000000 azure-mgmt-hdinsightcontainers-1.0.0b2/azure/mgmt/hdinsightcontainers/aio/operations/_cluster_available_upgrades_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    15933 2024-04-07 03:33:17.000000 azure-mgmt-hdinsightcontainers-1.0.0b2/azure/mgmt/hdinsightcontainers/aio/operations/_cluster_jobs_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6282 2024-04-07 03:33:17.000000 azure-mgmt-hdinsightcontainers-1.0.0b2/azure/mgmt/hdinsightcontainers/aio/operations/_cluster_pool_available_upgrades_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    43074 2024-04-07 03:33:17.000000 azure-mgmt-hdinsightcontainers-1.0.0b2/azure/mgmt/hdinsightcontainers/aio/operations/_cluster_pools_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    61614 2024-04-07 03:33:17.000000 azure-mgmt-hdinsightcontainers-1.0.0b2/azure/mgmt/hdinsightcontainers/aio/operations/_clusters_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     7403 2024-04-07 03:33:17.000000 azure-mgmt-hdinsightcontainers-1.0.0b2/azure/mgmt/hdinsightcontainers/aio/operations/_locations_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5588 2024-04-07 03:33:17.000000 azure-mgmt-hdinsightcontainers-1.0.0b2/azure/mgmt/hdinsightcontainers/aio/operations/_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-04-07 03:33:17.000000 azure-mgmt-hdinsightcontainers-1.0.0b2/azure/mgmt/hdinsightcontainers/aio/operations/_patch.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-07 03:34:25.161396 azure-mgmt-hdinsightcontainers-1.0.0b2/azure/mgmt/hdinsightcontainers/models/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    13533 2024-04-07 03:33:17.000000 azure-mgmt-hdinsightcontainers-1.0.0b2/azure/mgmt/hdinsightcontainers/models/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     7937 2024-04-07 03:33:17.000000 azure-mgmt-hdinsightcontainers-1.0.0b2/azure/mgmt/hdinsightcontainers/models/_hd_insight_containers_mgmt_client_enums.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)   234617 2024-04-07 03:33:17.000000 azure-mgmt-hdinsightcontainers-1.0.0b2/azure/mgmt/hdinsightcontainers/models/_models_py3.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-04-07 03:33:17.000000 azure-mgmt-hdinsightcontainers-1.0.0b2/azure/mgmt/hdinsightcontainers/models/_patch.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-07 03:34:25.165396 azure-mgmt-hdinsightcontainers-1.0.0b2/azure/mgmt/hdinsightcontainers/operations/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1645 2024-04-07 03:33:17.000000 azure-mgmt-hdinsightcontainers-1.0.0b2/azure/mgmt/hdinsightcontainers/operations/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     7091 2024-04-07 03:33:17.000000 azure-mgmt-hdinsightcontainers-1.0.0b2/azure/mgmt/hdinsightcontainers/operations/_available_cluster_pool_versions_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     7053 2024-04-07 03:33:17.000000 azure-mgmt-hdinsightcontainers-1.0.0b2/azure/mgmt/hdinsightcontainers/operations/_available_cluster_versions_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     7885 2024-04-07 03:33:17.000000 azure-mgmt-hdinsightcontainers-1.0.0b2/azure/mgmt/hdinsightcontainers/operations/_cluster_available_upgrades_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    19029 2024-04-07 03:33:17.000000 azure-mgmt-hdinsightcontainers-1.0.0b2/azure/mgmt/hdinsightcontainers/operations/_cluster_jobs_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     7628 2024-04-07 03:33:17.000000 azure-mgmt-hdinsightcontainers-1.0.0b2/azure/mgmt/hdinsightcontainers/operations/_cluster_pool_available_upgrades_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    52116 2024-04-07 03:33:17.000000 azure-mgmt-hdinsightcontainers-1.0.0b2/azure/mgmt/hdinsightcontainers/operations/_cluster_pools_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    76413 2024-04-07 03:33:17.000000 azure-mgmt-hdinsightcontainers-1.0.0b2/azure/mgmt/hdinsightcontainers/operations/_clusters_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     8781 2024-04-07 03:33:17.000000 azure-mgmt-hdinsightcontainers-1.0.0b2/azure/mgmt/hdinsightcontainers/operations/_locations_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6288 2024-04-07 03:33:17.000000 azure-mgmt-hdinsightcontainers-1.0.0b2/azure/mgmt/hdinsightcontainers/operations/_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-04-07 03:33:17.000000 azure-mgmt-hdinsightcontainers-1.0.0b2/azure/mgmt/hdinsightcontainers/operations/_patch.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       26 2024-04-07 03:33:17.000000 azure-mgmt-hdinsightcontainers-1.0.0b2/azure/mgmt/hdinsightcontainers/py.typed
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-07 03:34:25.165396 azure-mgmt-hdinsightcontainers-1.0.0b2/azure_mgmt_hdinsightcontainers.egg-info/
+-rw-r--r--   0 cloudtest  (1000) cloudtest  (1000)     8586 2024-04-07 03:34:25.000000 azure-mgmt-hdinsightcontainers-1.0.0b2/azure_mgmt_hdinsightcontainers.egg-info/PKG-INFO
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2862 2024-04-07 03:34:25.000000 azure-mgmt-hdinsightcontainers-1.0.0b2/azure_mgmt_hdinsightcontainers.egg-info/SOURCES.txt
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        1 2024-04-07 03:34:25.000000 azure-mgmt-hdinsightcontainers-1.0.0b2/azure_mgmt_hdinsightcontainers.egg-info/dependency_links.txt
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        1 2024-04-07 03:34:24.000000 azure-mgmt-hdinsightcontainers-1.0.0b2/azure_mgmt_hdinsightcontainers.egg-info/not-zip-safe
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       56 2024-04-07 03:34:25.000000 azure-mgmt-hdinsightcontainers-1.0.0b2/azure_mgmt_hdinsightcontainers.egg-info/requires.txt
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        6 2024-04-07 03:34:25.000000 azure-mgmt-hdinsightcontainers-1.0.0b2/azure_mgmt_hdinsightcontainers.egg-info/top_level.txt
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       38 2024-04-07 03:34:25.165396 azure-mgmt-hdinsightcontainers-1.0.0b2/setup.cfg
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2791 2024-04-07 03:33:17.000000 azure-mgmt-hdinsightcontainers-1.0.0b2/setup.py
```

### Comparing `azure-mgmt-hdinsightcontainers-1.0.0b1/LICENSE` & `azure-mgmt-hdinsightcontainers-1.0.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `azure-mgmt-hdinsightcontainers-1.0.0b1/PKG-INFO` & `azure-mgmt-hdinsightcontainers-1.0.0b2/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,45 +1,22 @@
-Metadata-Version: 2.1
-Name: azure-mgmt-hdinsightcontainers
-Version: 1.0.0b1
-Summary: Microsoft Azure Hdinsightcontainers Management Client Library for Python
-Home-page: https://github.com/Azure/azure-sdk-for-python
-Author: Microsoft Corporation
-Author-email: azpysdkhelp@microsoft.com
-License: MIT License
-Keywords: azure,azure sdk
-Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Microsoft Azure SDK for Python
 
 This is the Microsoft Azure Hdinsightcontainers Management Client Library.
-This package has been tested with Python 3.7+.
+This package has been tested with Python 3.8+.
 For a more complete view of Azure libraries, see the [azure sdk python release](https://aka.ms/azsdk/python/all).
 
 ## _Disclaimer_
 
 _Azure SDK Python packages support for Python 2.7 has ended 01 January 2022. For more information and questions, please refer to https://github.com/Azure/azure-sdk-for-python/issues/20691_
 
 ## Getting started
 
 ### Prerequisites
 
-- Python 3.7+ is required to use this package.
+- Python 3.8+ is required to use this package.
 - [Azure subscription](https://azure.microsoft.com/free/)
 
 ### Install the package
 
 ```bash
 pip install azure-mgmt-hdinsightcontainers
 pip install azure-identity
@@ -78,17 +55,7 @@
 ## Next steps
 
 ## Provide Feedback
 
 If you encounter any bugs or have suggestions, please file an issue in the
 [Issues](https://github.com/Azure/azure-sdk-for-python/issues)
 section of the project. 
-
-
-![Impressions](https://azure-sdk-impressions.azurewebsites.net/api/impressions/azure-sdk-for-python%2Fazure-mgmt-hdinsightcontainers%2FREADME.png)
-
-
-# Release History
-
-## 1.0.0b1 (2023-08-18)
-
-* Initial Release
```

### Comparing `azure-mgmt-hdinsightcontainers-1.0.0b1/_meta.json` & `azure-mgmt-hdinsightcontainers-1.0.0b2/_meta.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.75%*

 * *Differences: {"'autorest_command'": "'autorest "*

 * *                       'specification/hdinsight/resource-manager/Microsoft.HDInsight/HDInsightOnAks/readme.md '*

 * *                       '--generate-sample=True --include-x-ms-examples-original-file=True --python '*

 * *                       '--python-sdks-folder=/home/vsts/work/1/azure-sdk-for-python/sdk '*

 * *                       '--tag=package-preview-2023-11 --use=@autorest/python@6.13.7 '*

 * *                       '--use=@autorest/modelerfour@4.27.0 --version=3.9.7 '*

 * *           […]*

```diff
@@ -1,11 +1,11 @@
 {
     "autorest": "3.9.7",
-    "autorest_command": "autorest specification/hdinsight/resource-manager/Microsoft.HDInsight/HDInsightOnAks/readme.md --generate-sample=True --include-x-ms-examples-original-file=True --python --python-sdks-folder=/home/vsts/work/1/azure-sdk-for-python/sdk --use=@autorest/python@6.7.1 --use=@autorest/modelerfour@4.26.2 --version=3.9.7 --version-tolerant=False",
-    "commit": "ec882de9043fe225777bbf5fd28ed5259b0949db",
+    "autorest_command": "autorest specification/hdinsight/resource-manager/Microsoft.HDInsight/HDInsightOnAks/readme.md --generate-sample=True --include-x-ms-examples-original-file=True --python --python-sdks-folder=/home/vsts/work/1/azure-sdk-for-python/sdk --tag=package-preview-2023-11 --use=@autorest/python@6.13.7 --use=@autorest/modelerfour@4.27.0 --version=3.9.7 --version-tolerant=False",
+    "commit": "92de53a5f1e0e03c94b40475d2135d97148ed014",
     "readme": "specification/hdinsight/resource-manager/Microsoft.HDInsight/HDInsightOnAks/readme.md",
     "repository_url": "https://github.com/Azure/azure-rest-api-specs",
     "use": [
-        "@autorest/python@6.7.1",
-        "@autorest/modelerfour@4.26.2"
+        "@autorest/python@6.13.7",
+        "@autorest/modelerfour@4.27.0"
     ]
 }
```

### Comparing `azure-mgmt-hdinsightcontainers-1.0.0b1/azure/mgmt/hdinsightcontainers/__init__.py` & `azure-mgmt-hdinsightcontainers-1.0.0b2/azure/mgmt/hdinsightcontainers/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-hdinsightcontainers-1.0.0b1/azure/mgmt/hdinsightcontainers/_configuration.py` & `azure-mgmt-hdinsightcontainers-1.0.0b2/azure/mgmt/hdinsightcontainers/_configuration.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,63 +4,62 @@
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from typing import Any, TYPE_CHECKING
 
-from azure.core.configuration import Configuration
 from azure.core.pipeline import policies
 from azure.mgmt.core.policies import ARMChallengeAuthenticationPolicy, ARMHttpLoggingPolicy
 
 from ._version import VERSION
 
 if TYPE_CHECKING:
     # pylint: disable=unused-import,ungrouped-imports
     from azure.core.credentials import TokenCredential
 
 
-class HDInsightContainersMgmtClientConfiguration(Configuration):  # pylint: disable=too-many-instance-attributes
+class HDInsightContainersMgmtClientConfiguration:  # pylint: disable=too-many-instance-attributes,name-too-long
     """Configuration for HDInsightContainersMgmtClient.
 
     Note that all parameters used to create this instance are saved as instance
     attributes.
 
     :param credential: Credential needed for the client to connect to Azure. Required.
     :type credential: ~azure.core.credentials.TokenCredential
     :param subscription_id: The ID of the target subscription. The value must be an UUID. Required.
     :type subscription_id: str
-    :keyword api_version: Api Version. Default value is "2023-06-01-preview". Note that overriding
+    :keyword api_version: Api Version. Default value is "2023-11-01-preview". Note that overriding
      this default value may result in unsupported behavior.
     :paramtype api_version: str
     """
 
     def __init__(self, credential: "TokenCredential", subscription_id: str, **kwargs: Any) -> None:
-        super(HDInsightContainersMgmtClientConfiguration, self).__init__(**kwargs)
-        api_version: str = kwargs.pop("api_version", "2023-06-01-preview")
+        api_version: str = kwargs.pop("api_version", "2023-11-01-preview")
 
         if credential is None:
             raise ValueError("Parameter 'credential' must not be None.")
         if subscription_id is None:
             raise ValueError("Parameter 'subscription_id' must not be None.")
 
         self.credential = credential
         self.subscription_id = subscription_id
         self.api_version = api_version
         self.credential_scopes = kwargs.pop("credential_scopes", ["https://management.azure.com/.default"])
         kwargs.setdefault("sdk_moniker", "mgmt-hdinsightcontainers/{}".format(VERSION))
+        self.polling_interval = kwargs.get("polling_interval", 30)
         self._configure(**kwargs)
 
     def _configure(self, **kwargs: Any) -> None:
         self.user_agent_policy = kwargs.get("user_agent_policy") or policies.UserAgentPolicy(**kwargs)
         self.headers_policy = kwargs.get("headers_policy") or policies.HeadersPolicy(**kwargs)
         self.proxy_policy = kwargs.get("proxy_policy") or policies.ProxyPolicy(**kwargs)
         self.logging_policy = kwargs.get("logging_policy") or policies.NetworkTraceLoggingPolicy(**kwargs)
         self.http_logging_policy = kwargs.get("http_logging_policy") or ARMHttpLoggingPolicy(**kwargs)
-        self.retry_policy = kwargs.get("retry_policy") or policies.RetryPolicy(**kwargs)
         self.custom_hook_policy = kwargs.get("custom_hook_policy") or policies.CustomHookPolicy(**kwargs)
         self.redirect_policy = kwargs.get("redirect_policy") or policies.RedirectPolicy(**kwargs)
+        self.retry_policy = kwargs.get("retry_policy") or policies.RetryPolicy(**kwargs)
         self.authentication_policy = kwargs.get("authentication_policy")
         if self.credential and not self.authentication_policy:
             self.authentication_policy = ARMChallengeAuthenticationPolicy(
                 self.credential, *self.credential_scopes, **kwargs
             )
```

### Comparing `azure-mgmt-hdinsightcontainers-1.0.0b1/azure/mgmt/hdinsightcontainers/_hd_insight_containers_mgmt_client.py` & `azure-mgmt-hdinsightcontainers-1.0.0b2/azure/mgmt/hdinsightcontainers/_hd_insight_containers_mgmt_client.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,42 +5,52 @@
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from copy import deepcopy
 from typing import Any, TYPE_CHECKING
 
+from azure.core.pipeline import policies
 from azure.core.rest import HttpRequest, HttpResponse
 from azure.mgmt.core import ARMPipelineClient
+from azure.mgmt.core.policies import ARMAutoResourceProviderRegistrationPolicy
 
 from . import models as _models
 from ._configuration import HDInsightContainersMgmtClientConfiguration
 from ._serialization import Deserializer, Serializer
 from .operations import (
     AvailableClusterPoolVersionsOperations,
     AvailableClusterVersionsOperations,
+    ClusterAvailableUpgradesOperations,
     ClusterJobsOperations,
+    ClusterPoolAvailableUpgradesOperations,
     ClusterPoolsOperations,
     ClustersOperations,
     LocationsOperations,
     Operations,
 )
 
 if TYPE_CHECKING:
     # pylint: disable=unused-import,ungrouped-imports
     from azure.core.credentials import TokenCredential
 
 
 class HDInsightContainersMgmtClient:  # pylint: disable=client-accepts-api-version-keyword,too-many-instance-attributes
-    """HDInsight On Aks Management Client.
+    """HDInsight Containers Management Client.
 
     :ivar cluster_pools: ClusterPoolsOperations operations
     :vartype cluster_pools: azure.mgmt.hdinsightcontainers.operations.ClusterPoolsOperations
+    :ivar cluster_pool_available_upgrades: ClusterPoolAvailableUpgradesOperations operations
+    :vartype cluster_pool_available_upgrades:
+     azure.mgmt.hdinsightcontainers.operations.ClusterPoolAvailableUpgradesOperations
     :ivar clusters: ClustersOperations operations
     :vartype clusters: azure.mgmt.hdinsightcontainers.operations.ClustersOperations
+    :ivar cluster_available_upgrades: ClusterAvailableUpgradesOperations operations
+    :vartype cluster_available_upgrades:
+     azure.mgmt.hdinsightcontainers.operations.ClusterAvailableUpgradesOperations
     :ivar cluster_jobs: ClusterJobsOperations operations
     :vartype cluster_jobs: azure.mgmt.hdinsightcontainers.operations.ClusterJobsOperations
     :ivar locations: LocationsOperations operations
     :vartype locations: azure.mgmt.hdinsightcontainers.operations.LocationsOperations
     :ivar operations: Operations operations
     :vartype operations: azure.mgmt.hdinsightcontainers.operations.Operations
     :ivar available_cluster_pool_versions: AvailableClusterPoolVersionsOperations operations
@@ -51,15 +61,15 @@
      azure.mgmt.hdinsightcontainers.operations.AvailableClusterVersionsOperations
     :param credential: Credential needed for the client to connect to Azure. Required.
     :type credential: ~azure.core.credentials.TokenCredential
     :param subscription_id: The ID of the target subscription. The value must be an UUID. Required.
     :type subscription_id: str
     :param base_url: Service URL. Default value is "https://management.azure.com".
     :type base_url: str
-    :keyword api_version: Api Version. Default value is "2023-06-01-preview". Note that overriding
+    :keyword api_version: Api Version. Default value is "2023-11-01-preview". Note that overriding
      this default value may result in unsupported behavior.
     :paramtype api_version: str
     :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
      Retry-After header is present.
     """
 
     def __init__(
@@ -68,33 +78,57 @@
         subscription_id: str,
         base_url: str = "https://management.azure.com",
         **kwargs: Any
     ) -> None:
         self._config = HDInsightContainersMgmtClientConfiguration(
             credential=credential, subscription_id=subscription_id, **kwargs
         )
-        self._client: ARMPipelineClient = ARMPipelineClient(base_url=base_url, config=self._config, **kwargs)
+        _policies = kwargs.pop("policies", None)
+        if _policies is None:
+            _policies = [
+                policies.RequestIdPolicy(**kwargs),
+                self._config.headers_policy,
+                self._config.user_agent_policy,
+                self._config.proxy_policy,
+                policies.ContentDecodePolicy(**kwargs),
+                ARMAutoResourceProviderRegistrationPolicy(),
+                self._config.redirect_policy,
+                self._config.retry_policy,
+                self._config.authentication_policy,
+                self._config.custom_hook_policy,
+                self._config.logging_policy,
+                policies.DistributedTracingPolicy(**kwargs),
+                policies.SensitiveHeaderCleanupPolicy(**kwargs) if self._config.redirect_policy else None,
+                self._config.http_logging_policy,
+            ]
+        self._client: ARMPipelineClient = ARMPipelineClient(base_url=base_url, policies=_policies, **kwargs)
 
         client_models = {k: v for k, v in _models.__dict__.items() if isinstance(v, type)}
         self._serialize = Serializer(client_models)
         self._deserialize = Deserializer(client_models)
         self._serialize.client_side_validation = False
         self.cluster_pools = ClusterPoolsOperations(self._client, self._config, self._serialize, self._deserialize)
+        self.cluster_pool_available_upgrades = ClusterPoolAvailableUpgradesOperations(
+            self._client, self._config, self._serialize, self._deserialize
+        )
         self.clusters = ClustersOperations(self._client, self._config, self._serialize, self._deserialize)
+        self.cluster_available_upgrades = ClusterAvailableUpgradesOperations(
+            self._client, self._config, self._serialize, self._deserialize
+        )
         self.cluster_jobs = ClusterJobsOperations(self._client, self._config, self._serialize, self._deserialize)
         self.locations = LocationsOperations(self._client, self._config, self._serialize, self._deserialize)
         self.operations = Operations(self._client, self._config, self._serialize, self._deserialize)
         self.available_cluster_pool_versions = AvailableClusterPoolVersionsOperations(
             self._client, self._config, self._serialize, self._deserialize
         )
         self.available_cluster_versions = AvailableClusterVersionsOperations(
             self._client, self._config, self._serialize, self._deserialize
         )
 
-    def _send_request(self, request: HttpRequest, **kwargs: Any) -> HttpResponse:
+    def _send_request(self, request: HttpRequest, *, stream: bool = False, **kwargs: Any) -> HttpResponse:
         """Runs the network request through the client's chained policies.
 
         >>> from azure.core.rest import HttpRequest
         >>> request = HttpRequest("GET", "https://www.example.org/")
         <HttpRequest [GET], url: 'https://www.example.org/'>
         >>> response = client._send_request(request)
         <HttpResponse: 200 OK>
@@ -106,15 +140,15 @@
         :keyword bool stream: Whether the response payload will be streamed. Defaults to False.
         :return: The response of your network call. Does not do error handling on your response.
         :rtype: ~azure.core.rest.HttpResponse
         """
 
         request_copy = deepcopy(request)
         request_copy.url = self._client.format_url(request_copy.url)
-        return self._client.send_request(request_copy, **kwargs)
+        return self._client.send_request(request_copy, stream=stream, **kwargs)  # type: ignore
 
     def close(self) -> None:
         self._client.close()
 
     def __enter__(self) -> "HDInsightContainersMgmtClient":
         self._client.__enter__()
         return self
```

### Comparing `azure-mgmt-hdinsightcontainers-1.0.0b1/azure/mgmt/hdinsightcontainers/_patch.py` & `azure-mgmt-hdinsightcontainers-1.0.0b2/azure/mgmt/hdinsightcontainers/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-hdinsightcontainers-1.0.0b1/azure/mgmt/hdinsightcontainers/_serialization.py` & `azure-mgmt-hdinsightcontainers-1.0.0b2/azure/mgmt/hdinsightcontainers/_serialization.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,16 +59,16 @@
     from urllib import quote  # type: ignore
 except ImportError:
     from urllib.parse import quote
 import xml.etree.ElementTree as ET
 
 import isodate  # type: ignore
 
-from azure.core.exceptions import DeserializationError, SerializationError, raise_with_traceback
-from azure.core.serialization import NULL as AzureCoreNull
+from azure.core.exceptions import DeserializationError, SerializationError
+from azure.core.serialization import NULL as CoreNull
 
 _BOM = codecs.BOM_UTF8.decode(encoding="utf-8")
 
 ModelType = TypeVar("ModelType", bound="Model")
 JSON = MutableMapping[str, Any]
 
 
@@ -120,15 +120,15 @@
                     if isinstance(data, unicode):  # type: ignore
                         # If I'm Python 2.7 and unicode XML will scream if I try a "fromstring" on unicode string
                         data_as_str = data_as_str.encode(encoding="utf-8")  # type: ignore
                 except NameError:
                     pass
 
                 return ET.fromstring(data_as_str)  # nosec
-            except ET.ParseError:
+            except ET.ParseError as err:
                 # It might be because the server has an issue, and returned JSON with
                 # content-type XML....
                 # So let's try a JSON load, and if it's still broken
                 # let's flow the initial exception
                 def _json_attemp(data):
                     try:
                         return True, json.loads(data)
@@ -139,15 +139,15 @@
                 if success:
                     return json_result
                 # If i'm here, it's not JSON, it's not XML, let's scream
                 # and raise the last context in this block (the XML exception)
                 # The function hack is because Py2.7 messes up with exception
                 # context otherwise.
                 _LOGGER.critical("Wasn't XML not JSON, failing")
-                raise_with_traceback(DeserializationError, "XML is invalid")
+                raise DeserializationError("XML is invalid") from err
         raise DeserializationError("Cannot deserialize content-type: {}".format(content_type))
 
     @classmethod
     def deserialize_from_http_generics(cls, body_bytes: Optional[Union[AnyStr, IO]], headers: Mapping) -> Any:
         """Deserialize from HTTP response.
 
         Use bytes and headers to NOT use any requests/aiohttp or whatever
@@ -166,21 +166,14 @@
             content_type = "application/json"
 
         if body_bytes:
             return cls.deserialize_from_text(body_bytes, content_type)
         return None
 
 
-try:
-    basestring  # type: ignore
-    unicode_str = unicode  # type: ignore
-except NameError:
-    basestring = str
-    unicode_str = str
-
 _LOGGER = logging.getLogger(__name__)
 
 try:
     _long_type = long  # type: ignore
 except NameError:
     _long_type = int
 
@@ -291,15 +284,15 @@
     """
 
     _subtype_map: Dict[str, Dict[str, Any]] = {}
     _attribute_map: Dict[str, Dict[str, Any]] = {}
     _validation: Dict[str, Dict[str, Any]] = {}
 
     def __init__(self, **kwargs: Any) -> None:
-        self.additional_properties: Dict[str, Any] = {}
+        self.additional_properties: Optional[Dict[str, Any]] = {}
         for k in kwargs:
             if k not in self._attribute_map:
                 _LOGGER.warning("%s is not a known attribute of class %s and will be ignored", k, self.__class__)
             elif k in self._validation and self._validation[k].get("readonly", False):
                 _LOGGER.warning("Readonly attribute %s will be ignored in class %s", k, self.__class__)
             else:
                 setattr(self, k, kwargs[k])
@@ -336,26 +329,26 @@
             xml_map = cls._xml_map  # type: ignore
         except AttributeError:
             xml_map = {}
 
         return _create_xml_node(xml_map.get("name", cls.__name__), xml_map.get("prefix", None), xml_map.get("ns", None))
 
     def serialize(self, keep_readonly: bool = False, **kwargs: Any) -> JSON:
-        """Return the JSON that would be sent to azure from this model.
+        """Return the JSON that would be sent to server from this model.
 
         This is an alias to `as_dict(full_restapi_key_transformer, keep_readonly=False)`.
 
         If you want XML serialization, you can pass the kwargs is_xml=True.
 
         :param bool keep_readonly: If you want to serialize the readonly attributes
         :returns: A dict JSON compatible object
         :rtype: dict
         """
         serializer = Serializer(self._infer_class_models())
-        return serializer._serialize(self, keep_readonly=keep_readonly, **kwargs)
+        return serializer._serialize(self, keep_readonly=keep_readonly, **kwargs)  # type: ignore
 
     def as_dict(
         self,
         keep_readonly: bool = True,
         key_transformer: Callable[[str, Dict[str, Any], Any], Any] = attribute_transformer,
         **kwargs: Any
     ) -> JSON:
@@ -386,15 +379,15 @@
         If you want XML serialization, you can pass the kwargs is_xml=True.
 
         :param function key_transformer: A key transformer function.
         :returns: A dict JSON compatible object
         :rtype: dict
         """
         serializer = Serializer(self._infer_class_models())
-        return serializer._serialize(self, key_transformer=key_transformer, keep_readonly=keep_readonly, **kwargs)
+        return serializer._serialize(self, key_transformer=key_transformer, keep_readonly=keep_readonly, **kwargs)  # type: ignore
 
     @classmethod
     def _infer_class_models(cls):
         try:
             str_models = cls.__module__.rsplit(".", 1)[0]
             models = sys.modules[str_models]
             client_models = {k: v for k, v in models.__dict__.items() if isinstance(v, type)}
@@ -411,15 +404,15 @@
 
         :param str data: A str using RestAPI structure. JSON by default.
         :param str content_type: JSON by default, set application/xml if XML.
         :returns: An instance of this model
         :raises: DeserializationError if something went wrong
         """
         deserializer = Deserializer(cls._infer_class_models())
-        return deserializer(cls.__name__, data, content_type=content_type)
+        return deserializer(cls.__name__, data, content_type=content_type)  # type: ignore
 
     @classmethod
     def from_dict(
         cls: Type[ModelType],
         data: Any,
         key_extractors: Optional[Callable[[str, Dict[str, Any], Any], Any]] = None,
         content_type: Optional[str] = None,
@@ -441,15 +434,15 @@
                 attribute_key_case_insensitive_extractor,
                 rest_key_case_insensitive_extractor,
                 last_rest_key_case_insensitive_extractor,
             ]
             if key_extractors is None
             else key_extractors
         )
-        return deserializer(cls.__name__, data, content_type=content_type)
+        return deserializer(cls.__name__, data, content_type=content_type)  # type: ignore
 
     @classmethod
     def _flatten_subtype(cls, key, objects):
         if "_subtype_map" not in cls.__dict__:
             return {}
         result = dict(cls._subtype_map[key])
         for valuetype in cls._subtype_map[key].values():
@@ -541,15 +534,15 @@
         "min_items": lambda x, y: len(x) < y,
         "max_items": lambda x, y: len(x) > y,
         "pattern": lambda x, y: not re.match(y, x, re.UNICODE),
         "unique": lambda x, y: len(x) != len(set(x)),
         "multiple": lambda x, y: x % y != 0,
     }
 
-    def __init__(self, classes: Optional[Mapping[str, Type[ModelType]]] = None):
+    def __init__(self, classes: Optional[Mapping[str, type]] = None):
         self.serialize_type = {
             "iso-8601": Serializer.serialize_iso,
             "rfc-1123": Serializer.serialize_rfc,
             "unix-time": Serializer.serialize_unix,
             "duration": Serializer.serialize_duration,
             "date": Serializer.serialize_date,
             "time": Serializer.serialize_time,
@@ -557,15 +550,15 @@
             "long": Serializer.serialize_long,
             "bytearray": Serializer.serialize_bytearray,
             "base64": Serializer.serialize_base64,
             "object": self.serialize_object,
             "[]": self.serialize_iter,
             "{}": self.serialize_dict,
         }
-        self.dependencies: Dict[str, Type[ModelType]] = dict(classes) if classes else {}
+        self.dependencies: Dict[str, type] = dict(classes) if classes else {}
         self.key_transformer = full_restapi_key_transformer
         self.client_side_validation = True
 
     def _serialize(self, target_obj, data_type=None, **kwargs):
         """Serialize data into a string according to type.
 
         :param target_obj: The data to be serialized.
@@ -645,15 +638,15 @@
                                     new_attr.tag = "}".join([splitted_tag[0], xml_name])
                                 else:
                                     new_attr.tag = xml_name
                             serialized.append(new_attr)  # type: ignore
                         else:  # That's a basic type
                             # Integrate namespace if necessary
                             local_node = _create_xml_node(xml_name, xml_prefix, xml_ns)
-                            local_node.text = unicode_str(new_attr)
+                            local_node.text = str(new_attr)
                             serialized.append(local_node)  # type: ignore
                     else:  # JSON
                         for k in reversed(keys):  # type: ignore
                             new_attr = {k: new_attr}
 
                         _new_attr = new_attr
                         _serialized = serialized
@@ -664,15 +657,15 @@
                             _serialized = _serialized[k]
                 except ValueError as err:
                     if isinstance(err, SerializationError):
                         raise
 
         except (AttributeError, KeyError, TypeError) as err:
             msg = "Attribute {} in object {} cannot be serialized.\n{}".format(attr_name, class_name, str(target_obj))
-            raise_with_traceback(SerializationError, msg, err)
+            raise SerializationError(msg) from err
         else:
             return serialized
 
     def body(self, data, data_type, **kwargs):
         """Serialize data intended for a request body.
 
         :param data: The data to be serialized.
@@ -706,15 +699,15 @@
                     deserializer.key_extractors = [
                         rest_key_case_insensitive_extractor,
                         attribute_key_case_insensitive_extractor,
                         last_rest_key_case_insensitive_extractor,
                     ]
                 data = deserializer._deserialize(data_type, data)
             except DeserializationError as err:
-                raise_with_traceback(SerializationError, "Unable to build a model: " + str(err), err)
+                raise SerializationError("Unable to build a model: " + str(err)) from err
 
         return self._serialize(data, data_type, **kwargs)
 
     def url(self, name, data, data_type, **kwargs):
         """Serialize data intended for a URL path.
 
         :param data: The data to be serialized.
@@ -726,38 +719,39 @@
         try:
             output = self.serialize_data(data, data_type, **kwargs)
             if data_type == "bool":
                 output = json.dumps(output)
 
             if kwargs.get("skip_quote") is True:
                 output = str(output)
+                output = output.replace("{", quote("{")).replace("}", quote("}"))
             else:
                 output = quote(str(output), safe="")
         except SerializationError:
             raise TypeError("{} must be type {}.".format(name, data_type))
         else:
             return output
 
     def query(self, name, data, data_type, **kwargs):
         """Serialize data intended for a URL query.
 
         :param data: The data to be serialized.
         :param str data_type: The type to be serialized from.
         :keyword bool skip_quote: Whether to skip quote the serialized result.
         Defaults to False.
-        :rtype: str
+        :rtype: str, list
         :raises: TypeError if serialization fails.
         :raises: ValueError if data is None
         """
         try:
             # Treat the list aside, since we don't want to encode the div separator
             if data_type.startswith("["):
                 internal_data_type = data_type[1:-1]
                 do_quote = not kwargs.get("skip_quote", False)
-                return str(self.serialize_iter(data, internal_data_type, do_quote=do_quote, **kwargs))
+                return self.serialize_iter(data, internal_data_type, do_quote=do_quote, **kwargs)
 
             # Not a list, regular serialization
             output = self.serialize_data(data, data_type, **kwargs)
             if data_type == "bool":
                 output = json.dumps(output)
             if kwargs.get("skip_quote") is True:
                 output = str(output)
@@ -800,15 +794,15 @@
         :raises: ValueError if data is None
         :raises: SerializationError if serialization fails.
         """
         if data is None:
             raise ValueError("No value for given attribute")
 
         try:
-            if data is AzureCoreNull:
+            if data is CoreNull:
                 return None
             if data_type in self.basic_types.values():
                 return self.serialize_basic(data, data_type, **kwargs)
 
             elif data_type in self.serialize_type:
                 return self.serialize_type[data_type](data, **kwargs)
 
@@ -820,15 +814,15 @@
 
             iter_type = data_type[0] + data_type[-1]
             if iter_type in self.serialize_type:
                 return self.serialize_type[iter_type](data, data_type[1:-1], **kwargs)
 
         except (ValueError, TypeError) as err:
             msg = "Unable to serialize value: {!r} as type: {!r}."
-            raise_with_traceback(SerializationError, msg.format(data, data_type), err)
+            raise SerializationError(msg.format(data, data_type)) from err
         else:
             return self._serialize(data, **kwargs)
 
     @classmethod
     def _get_custom_serializers(cls, data_type, **kwargs):
         custom_serializer = kwargs.get("basic_types_serializers", {}).get(data_type)
         if custom_serializer:
@@ -989,15 +983,15 @@
         if isinstance(attr, ET.Element):
             return attr
         obj_type = type(attr)
         if obj_type in self.basic_types:
             return self.serialize_basic(attr, self.basic_types[obj_type], **kwargs)
         if obj_type is _long_type:
             return self.serialize_long(attr)
-        if obj_type is unicode_str:
+        if obj_type is str:
             return self.serialize_unicode(attr)
         if obj_type is datetime.datetime:
             return self.serialize_iso(attr)
         if obj_type is datetime.date:
             return self.serialize_date(attr)
         if obj_type is datetime.time:
             return self.serialize_time(attr)
@@ -1166,18 +1160,18 @@
                 microseconds = "." + microseconds
             date = "{:04}-{:02}-{:02}T{:02}:{:02}:{:02}".format(
                 utc.tm_year, utc.tm_mon, utc.tm_mday, utc.tm_hour, utc.tm_min, utc.tm_sec
             )
             return date + microseconds + "Z"
         except (ValueError, OverflowError) as err:
             msg = "Unable to serialize datetime object."
-            raise_with_traceback(SerializationError, msg, err)
+            raise SerializationError(msg) from err
         except AttributeError as err:
             msg = "ISO-8601 object must be valid Datetime object."
-            raise_with_traceback(TypeError, msg, err)
+            raise TypeError(msg) from err
 
     @staticmethod
     def serialize_unix(attr, **kwargs):
         """Serialize Datetime object into IntTime format.
         This is represented as seconds.
 
         :param Datetime attr: Object to be serialized.
@@ -1205,15 +1199,14 @@
             key = _decode_attribute_map_key(dict_keys[0])
             break
         working_key = _decode_attribute_map_key(dict_keys[0])
         working_data = working_data.get(working_key, data)
         if working_data is None:
             # If at any point while following flatten JSON path see None, it means
             # that all properties under are None as well
-            # https://github.com/Azure/msrest-for-python/issues/197
             return None
         key = ".".join(dict_keys[1:])
 
     return working_data.get(key)
 
 
 def rest_key_case_insensitive_extractor(attr, attr_desc, data):
@@ -1226,15 +1219,14 @@
             key = _decode_attribute_map_key(dict_keys[0])
             break
         working_key = _decode_attribute_map_key(dict_keys[0])
         working_data = attribute_key_case_insensitive_extractor(working_key, None, working_data)
         if working_data is None:
             # If at any point while following flatten JSON path see None, it means
             # that all properties under are None as well
-            # https://github.com/Azure/msrest-for-python/issues/197
             return None
         key = ".".join(dict_keys[1:])
 
     if working_data:
         return attribute_key_case_insensitive_extractor(key, None, working_data)
 
 
@@ -1367,15 +1359,15 @@
     :ivar list key_extractors: Ordered list of extractors to be used by this deserializer.
     """
 
     basic_types = {str: "str", int: "int", bool: "bool", float: "float"}
 
     valid_date = re.compile(r"\d{4}[-]\d{2}[-]\d{2}T\d{2}:\d{2}:\d{2}" r"\.?\d*Z?[-+]?[\d{2}]?:?[\d{2}]?")
 
-    def __init__(self, classes: Optional[Mapping[str, Type[ModelType]]] = None):
+    def __init__(self, classes: Optional[Mapping[str, type]] = None):
         self.deserialize_type = {
             "iso-8601": Deserializer.deserialize_iso,
             "rfc-1123": Deserializer.deserialize_rfc,
             "unix-time": Deserializer.deserialize_unix,
             "duration": Deserializer.deserialize_duration,
             "date": Deserializer.deserialize_date,
             "time": Deserializer.deserialize_time,
@@ -1387,15 +1379,15 @@
             "[]": self.deserialize_iter,
             "{}": self.deserialize_dict,
         }
         self.deserialize_expected_types = {
             "duration": (isodate.Duration, datetime.timedelta),
             "iso-8601": (datetime.datetime),
         }
-        self.dependencies: Dict[str, Type[ModelType]] = dict(classes) if classes else {}
+        self.dependencies: Dict[str, type] = dict(classes) if classes else {}
         self.key_extractors = [rest_key_extractor, xml_key_extractor]
         # Additional properties only works if the "rest_key_extractor" is used to
         # extract the keys. Making it to work whatever the key extractor is too much
         # complicated, with no real scenario for now.
         # So adding a flag to disable additional properties detection. This flag should be
         # used if your expect the deserialization to NOT come from a JSON REST syntax.
         # Otherwise, result are unexpected
@@ -1440,15 +1432,15 @@
                     setattr(data, attr, self._deserialize(local_type, value))
                 return data
             except AttributeError:
                 return
 
         response, class_name = self._classify_target(target_obj, data)
 
-        if isinstance(response, basestring):
+        if isinstance(response, str):
             return self.deserialize_data(data, response)
         elif isinstance(response, type) and issubclass(response, Enum):
             return self.deserialize_enum(data, response)
 
         if data is None:
             return data
         try:
@@ -1477,15 +1469,15 @@
                             continue
                         raw_value = found_value
 
                 value = self.deserialize_data(raw_value, attr_desc["type"])
                 d_attrs[attr] = value
         except (AttributeError, TypeError, KeyError) as err:
             msg = "Unable to deserialize to object: " + class_name  # type: ignore
-            raise_with_traceback(DeserializationError, msg, err)
+            raise DeserializationError(msg) from err
         else:
             additional_properties = self._build_additional_properties(attributes, data)
             return self._instantiate_model(response, d_attrs, additional_properties)
 
     def _build_additional_properties(self, attribute_map, data):
         if not self.additional_properties_detection:
             return None
@@ -1511,22 +1503,22 @@
 
         :param str target: The target object type to deserialize to.
         :param str/dict data: The response data to deserialize.
         """
         if target is None:
             return None, None
 
-        if isinstance(target, basestring):
+        if isinstance(target, str):
             try:
                 target = self.dependencies[target]
             except KeyError:
                 return target, target
 
         try:
-            target = target._classify(data, self.dependencies)
+            target = target._classify(data, self.dependencies)  # type: ignore
         except AttributeError:
             pass  # Target is not a Model, no classify
         return target, target.__class__.__name__  # type: ignore
 
     def failsafe_deserialize(self, target_obj, data, content_type=None):
         """Ignores any errors encountered in deserialization,
         and falls back to not deserializing the object. Recommended
@@ -1574,15 +1566,15 @@
         if hasattr(raw_data, "body"):
             return RawDeserializer.deserialize_from_http_generics(raw_data.text(), raw_data.headers)
 
         # Assume this enough to recognize requests.Response without importing it.
         if hasattr(raw_data, "_content_consumed"):
             return RawDeserializer.deserialize_from_http_generics(raw_data.text, raw_data.headers)
 
-        if isinstance(raw_data, (basestring, bytes)) or hasattr(raw_data, "read"):
+        if isinstance(raw_data, (str, bytes)) or hasattr(raw_data, "read"):
             return RawDeserializer.deserialize_from_text(raw_data, content_type)  # type: ignore
         return raw_data
 
     def _instantiate_model(self, response, attrs, additional_properties=None):
         """Instantiate a response model passing in deserialized args.
 
         :param response: The response model class.
@@ -1648,15 +1640,15 @@
                 if isinstance(data, ET.Element):
                     data = data.text
                 return self.deserialize_enum(data, obj_type)
 
         except (ValueError, TypeError, AttributeError) as err:
             msg = "Unable to deserialize response data."
             msg += " Data: {}, {}".format(data, data_type)
-            raise_with_traceback(DeserializationError, msg, err)
+            raise DeserializationError(msg) from err
         else:
             return self._deserialize(obj_type, data)
 
     def deserialize_iter(self, attr, iter_type):
         """Deserialize an iterable.
 
         :param list attr: Iterable to be deserialized.
@@ -1696,15 +1688,15 @@
         :raises: TypeError if non-builtin datatype encountered.
         """
         if attr is None:
             return None
         if isinstance(attr, ET.Element):
             # Do no recurse on XML, just return the tree as-is
             return attr
-        if isinstance(attr, basestring):
+        if isinstance(attr, str):
             return self.deserialize_basic(attr, "str")
         obj_type = type(attr)
         if obj_type in self.basic_types:
             return self.deserialize_basic(attr, self.basic_types[obj_type])
         if obj_type is _long_type:
             return self.deserialize_long(attr)
 
@@ -1753,15 +1745,15 @@
                     # None or '', node <a/> with a strong type is None.
                     # Don't try to model "empty bool" or "empty int"
                     return None
 
         if data_type == "bool":
             if attr in [True, False, 1, 0]:
                 return bool(attr)
-            elif isinstance(attr, basestring):
+            elif isinstance(attr, str):
                 if attr.lower() in ["true", "1"]:
                     return True
                 elif attr.lower() in ["false", "0"]:
                     return False
             raise TypeError("Invalid boolean value: {}".format(attr))
 
         if data_type == "str":
@@ -1804,15 +1796,14 @@
         """
         if isinstance(data, enum_obj) or data is None:
             return data
         if isinstance(data, Enum):
             data = data.value
         if isinstance(data, int):
             # Workaround. We might consider remove it in the future.
-            # https://github.com/Azure/azure-rest-api-specs/issues/141
             try:
                 return list(enum_obj.__members__.values())[data]
             except IndexError:
                 error = "{!r} is not a valid index for enum {!r}"
                 raise DeserializationError(error.format(data, enum_obj))
         try:
             return enum_obj(str(data))
@@ -1858,18 +1849,18 @@
         :param str attr: response string to be deserialized.
         :rtype: Decimal
         :raises: DeserializationError if string format invalid.
         """
         if isinstance(attr, ET.Element):
             attr = attr.text
         try:
-            return decimal.Decimal(attr)  # type: ignore
+            return decimal.Decimal(str(attr))  # type: ignore
         except decimal.DecimalException as err:
             msg = "Invalid decimal {}".format(attr)
-            raise_with_traceback(DeserializationError, msg, err)
+            raise DeserializationError(msg) from err
 
     @staticmethod
     def deserialize_long(attr):
         """Deserialize string into long (Py2) or int (Py3).
 
         :param str attr: response string to be deserialized.
         :rtype: long or int
@@ -1889,15 +1880,15 @@
         """
         if isinstance(attr, ET.Element):
             attr = attr.text
         try:
             duration = isodate.parse_duration(attr)
         except (ValueError, OverflowError, AttributeError) as err:
             msg = "Cannot deserialize duration object."
-            raise_with_traceback(DeserializationError, msg, err)
+            raise DeserializationError(msg) from err
         else:
             return duration
 
     @staticmethod
     def deserialize_date(attr):
         """Deserialize ISO-8601 formatted string into Date object.
 
@@ -1906,15 +1897,15 @@
         :raises: DeserializationError if string format invalid.
         """
         if isinstance(attr, ET.Element):
             attr = attr.text
         if re.search(r"[^\W\d_]", attr, re.I + re.U):  # type: ignore
             raise DeserializationError("Date must have only digits and -. Received: %s" % attr)
         # This must NOT use defaultmonth/defaultday. Using None ensure this raises an exception.
-        return isodate.parse_date(attr, defaultmonth=None, defaultday=None)
+        return isodate.parse_date(attr, defaultmonth=0, defaultday=0)
 
     @staticmethod
     def deserialize_time(attr):
         """Deserialize ISO-8601 formatted string into time object.
 
         :param str attr: response string to be deserialized.
         :rtype: datetime.time
@@ -1941,15 +1932,15 @@
             date_obj = datetime.datetime(
                 *parsed_date[:6], tzinfo=_FixedOffset(datetime.timedelta(minutes=(parsed_date[9] or 0) / 60))
             )
             if not date_obj.tzinfo:
                 date_obj = date_obj.astimezone(tz=TZ_UTC)
         except ValueError as err:
             msg = "Cannot deserialize to rfc datetime object."
-            raise_with_traceback(DeserializationError, msg, err)
+            raise DeserializationError(msg) from err
         else:
             return date_obj
 
     @staticmethod
     def deserialize_iso(attr):
         """Deserialize ISO-8601 formatted string into Datetime object.
 
@@ -1978,15 +1969,15 @@
 
             date_obj = isodate.parse_datetime(attr)
             test_utc = date_obj.utctimetuple()
             if test_utc.tm_year > 9999 or test_utc.tm_year < 1:
                 raise OverflowError("Hit max or min date")
         except (ValueError, OverflowError, AttributeError) as err:
             msg = "Cannot deserialize datetime object."
-            raise_with_traceback(DeserializationError, msg, err)
+            raise DeserializationError(msg) from err
         else:
             return date_obj
 
     @staticmethod
     def deserialize_unix(attr):
         """Serialize Datetime object into IntTime format.
         This is represented as seconds.
@@ -1994,13 +1985,14 @@
         :param int attr: Object to be serialized.
         :rtype: Datetime
         :raises: DeserializationError if format invalid
         """
         if isinstance(attr, ET.Element):
             attr = int(attr.text)  # type: ignore
         try:
+            attr = int(attr)
             date_obj = datetime.datetime.fromtimestamp(attr, TZ_UTC)
         except ValueError as err:
             msg = "Cannot deserialize to unix datetime object."
-            raise_with_traceback(DeserializationError, msg, err)
+            raise DeserializationError(msg) from err
         else:
             return date_obj
```

### Comparing `azure-mgmt-hdinsightcontainers-1.0.0b1/azure/mgmt/hdinsightcontainers/_vendor.py` & `azure-mgmt-hdinsightcontainers-1.0.0b2/azure/mgmt/hdinsightcontainers/_vendor.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-hdinsightcontainers-1.0.0b1/azure/mgmt/hdinsightcontainers/aio/__init__.py` & `azure-mgmt-hdinsightcontainers-1.0.0b2/azure/mgmt/hdinsightcontainers/aio/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-hdinsightcontainers-1.0.0b1/azure/mgmt/hdinsightcontainers/aio/_configuration.py` & `azure-mgmt-hdinsightcontainers-1.0.0b2/azure/mgmt/hdinsightcontainers/aio/_configuration.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,63 +4,62 @@
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from typing import Any, TYPE_CHECKING
 
-from azure.core.configuration import Configuration
 from azure.core.pipeline import policies
 from azure.mgmt.core.policies import ARMHttpLoggingPolicy, AsyncARMChallengeAuthenticationPolicy
 
 from .._version import VERSION
 
 if TYPE_CHECKING:
     # pylint: disable=unused-import,ungrouped-imports
     from azure.core.credentials_async import AsyncTokenCredential
 
 
-class HDInsightContainersMgmtClientConfiguration(Configuration):  # pylint: disable=too-many-instance-attributes
+class HDInsightContainersMgmtClientConfiguration:  # pylint: disable=too-many-instance-attributes,name-too-long
     """Configuration for HDInsightContainersMgmtClient.
 
     Note that all parameters used to create this instance are saved as instance
     attributes.
 
     :param credential: Credential needed for the client to connect to Azure. Required.
     :type credential: ~azure.core.credentials_async.AsyncTokenCredential
     :param subscription_id: The ID of the target subscription. The value must be an UUID. Required.
     :type subscription_id: str
-    :keyword api_version: Api Version. Default value is "2023-06-01-preview". Note that overriding
+    :keyword api_version: Api Version. Default value is "2023-11-01-preview". Note that overriding
      this default value may result in unsupported behavior.
     :paramtype api_version: str
     """
 
     def __init__(self, credential: "AsyncTokenCredential", subscription_id: str, **kwargs: Any) -> None:
-        super(HDInsightContainersMgmtClientConfiguration, self).__init__(**kwargs)
-        api_version: str = kwargs.pop("api_version", "2023-06-01-preview")
+        api_version: str = kwargs.pop("api_version", "2023-11-01-preview")
 
         if credential is None:
             raise ValueError("Parameter 'credential' must not be None.")
         if subscription_id is None:
             raise ValueError("Parameter 'subscription_id' must not be None.")
 
         self.credential = credential
         self.subscription_id = subscription_id
         self.api_version = api_version
         self.credential_scopes = kwargs.pop("credential_scopes", ["https://management.azure.com/.default"])
         kwargs.setdefault("sdk_moniker", "mgmt-hdinsightcontainers/{}".format(VERSION))
+        self.polling_interval = kwargs.get("polling_interval", 30)
         self._configure(**kwargs)
 
     def _configure(self, **kwargs: Any) -> None:
         self.user_agent_policy = kwargs.get("user_agent_policy") or policies.UserAgentPolicy(**kwargs)
         self.headers_policy = kwargs.get("headers_policy") or policies.HeadersPolicy(**kwargs)
         self.proxy_policy = kwargs.get("proxy_policy") or policies.ProxyPolicy(**kwargs)
         self.logging_policy = kwargs.get("logging_policy") or policies.NetworkTraceLoggingPolicy(**kwargs)
         self.http_logging_policy = kwargs.get("http_logging_policy") or ARMHttpLoggingPolicy(**kwargs)
-        self.retry_policy = kwargs.get("retry_policy") or policies.AsyncRetryPolicy(**kwargs)
         self.custom_hook_policy = kwargs.get("custom_hook_policy") or policies.CustomHookPolicy(**kwargs)
         self.redirect_policy = kwargs.get("redirect_policy") or policies.AsyncRedirectPolicy(**kwargs)
+        self.retry_policy = kwargs.get("retry_policy") or policies.AsyncRetryPolicy(**kwargs)
         self.authentication_policy = kwargs.get("authentication_policy")
         if self.credential and not self.authentication_policy:
             self.authentication_policy = AsyncARMChallengeAuthenticationPolicy(
                 self.credential, *self.credential_scopes, **kwargs
             )
```

### Comparing `azure-mgmt-hdinsightcontainers-1.0.0b1/azure/mgmt/hdinsightcontainers/aio/_hd_insight_containers_mgmt_client.py` & `azure-mgmt-hdinsightcontainers-1.0.0b2/azure/mgmt/hdinsightcontainers/aio/_hd_insight_containers_mgmt_client.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,42 +5,52 @@
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from copy import deepcopy
 from typing import Any, Awaitable, TYPE_CHECKING
 
+from azure.core.pipeline import policies
 from azure.core.rest import AsyncHttpResponse, HttpRequest
 from azure.mgmt.core import AsyncARMPipelineClient
+from azure.mgmt.core.policies import AsyncARMAutoResourceProviderRegistrationPolicy
 
 from .. import models as _models
 from .._serialization import Deserializer, Serializer
 from ._configuration import HDInsightContainersMgmtClientConfiguration
 from .operations import (
     AvailableClusterPoolVersionsOperations,
     AvailableClusterVersionsOperations,
+    ClusterAvailableUpgradesOperations,
     ClusterJobsOperations,
+    ClusterPoolAvailableUpgradesOperations,
     ClusterPoolsOperations,
     ClustersOperations,
     LocationsOperations,
     Operations,
 )
 
 if TYPE_CHECKING:
     # pylint: disable=unused-import,ungrouped-imports
     from azure.core.credentials_async import AsyncTokenCredential
 
 
 class HDInsightContainersMgmtClient:  # pylint: disable=client-accepts-api-version-keyword,too-many-instance-attributes
-    """HDInsight On Aks Management Client.
+    """HDInsight Containers Management Client.
 
     :ivar cluster_pools: ClusterPoolsOperations operations
     :vartype cluster_pools: azure.mgmt.hdinsightcontainers.aio.operations.ClusterPoolsOperations
+    :ivar cluster_pool_available_upgrades: ClusterPoolAvailableUpgradesOperations operations
+    :vartype cluster_pool_available_upgrades:
+     azure.mgmt.hdinsightcontainers.aio.operations.ClusterPoolAvailableUpgradesOperations
     :ivar clusters: ClustersOperations operations
     :vartype clusters: azure.mgmt.hdinsightcontainers.aio.operations.ClustersOperations
+    :ivar cluster_available_upgrades: ClusterAvailableUpgradesOperations operations
+    :vartype cluster_available_upgrades:
+     azure.mgmt.hdinsightcontainers.aio.operations.ClusterAvailableUpgradesOperations
     :ivar cluster_jobs: ClusterJobsOperations operations
     :vartype cluster_jobs: azure.mgmt.hdinsightcontainers.aio.operations.ClusterJobsOperations
     :ivar locations: LocationsOperations operations
     :vartype locations: azure.mgmt.hdinsightcontainers.aio.operations.LocationsOperations
     :ivar operations: Operations operations
     :vartype operations: azure.mgmt.hdinsightcontainers.aio.operations.Operations
     :ivar available_cluster_pool_versions: AvailableClusterPoolVersionsOperations operations
@@ -51,15 +61,15 @@
      azure.mgmt.hdinsightcontainers.aio.operations.AvailableClusterVersionsOperations
     :param credential: Credential needed for the client to connect to Azure. Required.
     :type credential: ~azure.core.credentials_async.AsyncTokenCredential
     :param subscription_id: The ID of the target subscription. The value must be an UUID. Required.
     :type subscription_id: str
     :param base_url: Service URL. Default value is "https://management.azure.com".
     :type base_url: str
-    :keyword api_version: Api Version. Default value is "2023-06-01-preview". Note that overriding
+    :keyword api_version: Api Version. Default value is "2023-11-01-preview". Note that overriding
      this default value may result in unsupported behavior.
     :paramtype api_version: str
     :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
      Retry-After header is present.
     """
 
     def __init__(
@@ -68,33 +78,59 @@
         subscription_id: str,
         base_url: str = "https://management.azure.com",
         **kwargs: Any
     ) -> None:
         self._config = HDInsightContainersMgmtClientConfiguration(
             credential=credential, subscription_id=subscription_id, **kwargs
         )
-        self._client: AsyncARMPipelineClient = AsyncARMPipelineClient(base_url=base_url, config=self._config, **kwargs)
+        _policies = kwargs.pop("policies", None)
+        if _policies is None:
+            _policies = [
+                policies.RequestIdPolicy(**kwargs),
+                self._config.headers_policy,
+                self._config.user_agent_policy,
+                self._config.proxy_policy,
+                policies.ContentDecodePolicy(**kwargs),
+                AsyncARMAutoResourceProviderRegistrationPolicy(),
+                self._config.redirect_policy,
+                self._config.retry_policy,
+                self._config.authentication_policy,
+                self._config.custom_hook_policy,
+                self._config.logging_policy,
+                policies.DistributedTracingPolicy(**kwargs),
+                policies.SensitiveHeaderCleanupPolicy(**kwargs) if self._config.redirect_policy else None,
+                self._config.http_logging_policy,
+            ]
+        self._client: AsyncARMPipelineClient = AsyncARMPipelineClient(base_url=base_url, policies=_policies, **kwargs)
 
         client_models = {k: v for k, v in _models.__dict__.items() if isinstance(v, type)}
         self._serialize = Serializer(client_models)
         self._deserialize = Deserializer(client_models)
         self._serialize.client_side_validation = False
         self.cluster_pools = ClusterPoolsOperations(self._client, self._config, self._serialize, self._deserialize)
+        self.cluster_pool_available_upgrades = ClusterPoolAvailableUpgradesOperations(
+            self._client, self._config, self._serialize, self._deserialize
+        )
         self.clusters = ClustersOperations(self._client, self._config, self._serialize, self._deserialize)
+        self.cluster_available_upgrades = ClusterAvailableUpgradesOperations(
+            self._client, self._config, self._serialize, self._deserialize
+        )
         self.cluster_jobs = ClusterJobsOperations(self._client, self._config, self._serialize, self._deserialize)
         self.locations = LocationsOperations(self._client, self._config, self._serialize, self._deserialize)
         self.operations = Operations(self._client, self._config, self._serialize, self._deserialize)
         self.available_cluster_pool_versions = AvailableClusterPoolVersionsOperations(
             self._client, self._config, self._serialize, self._deserialize
         )
         self.available_cluster_versions = AvailableClusterVersionsOperations(
             self._client, self._config, self._serialize, self._deserialize
         )
 
-    def _send_request(self, request: HttpRequest, **kwargs: Any) -> Awaitable[AsyncHttpResponse]:
+    def _send_request(
+        self, request: HttpRequest, *, stream: bool = False, **kwargs: Any
+    ) -> Awaitable[AsyncHttpResponse]:
         """Runs the network request through the client's chained policies.
 
         >>> from azure.core.rest import HttpRequest
         >>> request = HttpRequest("GET", "https://www.example.org/")
         <HttpRequest [GET], url: 'https://www.example.org/'>
         >>> response = await client._send_request(request)
         <AsyncHttpResponse: 200 OK>
@@ -106,15 +142,15 @@
         :keyword bool stream: Whether the response payload will be streamed. Defaults to False.
         :return: The response of your network call. Does not do error handling on your response.
         :rtype: ~azure.core.rest.AsyncHttpResponse
         """
 
         request_copy = deepcopy(request)
         request_copy.url = self._client.format_url(request_copy.url)
-        return self._client.send_request(request_copy, **kwargs)
+        return self._client.send_request(request_copy, stream=stream, **kwargs)  # type: ignore
 
     async def close(self) -> None:
         await self._client.close()
 
     async def __aenter__(self) -> "HDInsightContainersMgmtClient":
         await self._client.__aenter__()
         return self
```

### Comparing `azure-mgmt-hdinsightcontainers-1.0.0b1/azure/mgmt/hdinsightcontainers/aio/_patch.py` & `azure-mgmt-hdinsightcontainers-1.0.0b2/azure/mgmt/hdinsightcontainers/aio/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-hdinsightcontainers-1.0.0b1/azure/mgmt/hdinsightcontainers/aio/operations/__init__.py` & `azure-mgmt-hdinsightcontainers-1.0.0b2/azure/mgmt/hdinsightcontainers/aio/operations/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,28 +3,32 @@
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from ._cluster_pools_operations import ClusterPoolsOperations
+from ._cluster_pool_available_upgrades_operations import ClusterPoolAvailableUpgradesOperations
 from ._clusters_operations import ClustersOperations
+from ._cluster_available_upgrades_operations import ClusterAvailableUpgradesOperations
 from ._cluster_jobs_operations import ClusterJobsOperations
 from ._locations_operations import LocationsOperations
 from ._operations import Operations
 from ._available_cluster_pool_versions_operations import AvailableClusterPoolVersionsOperations
 from ._available_cluster_versions_operations import AvailableClusterVersionsOperations
 
 from ._patch import __all__ as _patch_all
 from ._patch import *  # pylint: disable=unused-wildcard-import
 from ._patch import patch_sdk as _patch_sdk
 
 __all__ = [
     "ClusterPoolsOperations",
+    "ClusterPoolAvailableUpgradesOperations",
     "ClustersOperations",
+    "ClusterAvailableUpgradesOperations",
     "ClusterJobsOperations",
     "LocationsOperations",
     "Operations",
     "AvailableClusterPoolVersionsOperations",
     "AvailableClusterVersionsOperations",
 ]
 __all__.extend([p for p in _patch_all if p not in __all__])
```

### Comparing `azure-mgmt-hdinsightcontainers-1.0.0b1/azure/mgmt/hdinsightcontainers/aio/operations/_available_cluster_pool_versions_operations.py` & `azure-mgmt-hdinsightcontainers-1.0.0b2/azure/mgmt/hdinsightcontainers/operations/_available_cluster_pool_versions_operations.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,71 +1,100 @@
-# pylint: disable=too-many-lines
+# pylint: disable=too-many-lines,too-many-statements
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-from typing import Any, AsyncIterable, Callable, Dict, Optional, TypeVar
+from typing import Any, Callable, Dict, Iterable, Optional, TypeVar
 import urllib.parse
 
-from azure.core.async_paging import AsyncItemPaged, AsyncList
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
     ResourceNotFoundError,
     ResourceNotModifiedError,
     map_error,
 )
+from azure.core.paging import ItemPaged
 from azure.core.pipeline import PipelineResponse
-from azure.core.pipeline.transport import AsyncHttpResponse
+from azure.core.pipeline.transport import HttpResponse
 from azure.core.rest import HttpRequest
 from azure.core.tracing.decorator import distributed_trace
 from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
 
-from ... import models as _models
-from ..._vendor import _convert_request
-from ...operations._available_cluster_pool_versions_operations import build_list_by_location_request
+from .. import models as _models
+from .._serialization import Serializer
+from .._vendor import _convert_request
 
 T = TypeVar("T")
-ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
+ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
+
+_SERIALIZER = Serializer()
+_SERIALIZER.client_side_validation = False
+
+
+def build_list_by_location_request(location: str, subscription_id: str, **kwargs: Any) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+    _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-11-01-preview"))
+    accept = _headers.pop("Accept", "application/json")
+
+    # Construct URL
+    _url = kwargs.pop(
+        "template_url",
+        "/subscriptions/{subscriptionId}/providers/Microsoft.HDInsight/locations/{location}/availableClusterPoolVersions",
+    )  # pylint: disable=line-too-long
+    path_format_arguments = {
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
+        "location": _SERIALIZER.url("location", location, "str", min_length=1),
+    }
+
+    _url: str = _url.format(**path_format_arguments)  # type: ignore
+
+    # Construct parameters
+    _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
+
+    # Construct headers
+    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
+
+    return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
 
 
 class AvailableClusterPoolVersionsOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
-        :class:`~azure.mgmt.hdinsightcontainers.aio.HDInsightContainersMgmtClient`'s
+        :class:`~azure.mgmt.hdinsightcontainers.HDInsightContainersMgmtClient`'s
         :attr:`available_cluster_pool_versions` attribute.
     """
 
     models = _models
 
-    def __init__(self, *args, **kwargs) -> None:
+    def __init__(self, *args, **kwargs):
         input_args = list(args)
         self._client = input_args.pop(0) if input_args else kwargs.pop("client")
         self._config = input_args.pop(0) if input_args else kwargs.pop("config")
         self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
         self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
 
     @distributed_trace
-    def list_by_location(self, location: str, **kwargs: Any) -> AsyncIterable["_models.ClusterPoolVersion"]:
+    def list_by_location(self, location: str, **kwargs: Any) -> Iterable["_models.ClusterPoolVersion"]:
         """Returns a list of available cluster pool versions.
 
         :param location: The name of the Azure region. Required.
         :type location: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either ClusterPoolVersion or the result of cls(response)
-        :rtype:
-         ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.hdinsightcontainers.models.ClusterPoolVersion]
+        :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.hdinsightcontainers.models.ClusterPoolVersion]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.ClusterPoolVersionsListResult] = kwargs.pop("cls", None)
@@ -77,64 +106,59 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         def prepare_request(next_link=None):
             if not next_link:
 
-                request = build_list_by_location_request(
+                _request = build_list_by_location_request(
                     location=location,
                     subscription_id=self._config.subscription_id,
                     api_version=api_version,
-                    template_url=self.list_by_location.metadata["url"],
                     headers=_headers,
                     params=_params,
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
 
             else:
                 # make call to next link with the client's api-version
                 _parsed_next_link = urllib.parse.urlparse(next_link)
                 _next_request_params = case_insensitive_dict(
                     {
                         key: [urllib.parse.quote(v) for v in value]
                         for key, value in urllib.parse.parse_qs(_parsed_next_link.query).items()
                     }
                 )
                 _next_request_params["api-version"] = self._config.api_version
-                request = HttpRequest(
+                _request = HttpRequest(
                     "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
-                request.method = "GET"
-            return request
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
+                _request.method = "GET"
+            return _request
 
-        async def extract_data(pipeline_response):
+        def extract_data(pipeline_response):
             deserialized = self._deserialize("ClusterPoolVersionsListResult", pipeline_response)
             list_of_elem = deserialized.value
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
-            return deserialized.next_link or None, AsyncList(list_of_elem)
+            return deserialized.next_link or None, iter(list_of_elem)
 
-        async def get_next(next_link=None):
-            request = prepare_request(next_link)
+        def get_next(next_link=None):
+            _request = prepare_request(next_link)
 
             _stream = False
-            pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=_stream, **kwargs
+            pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+                _request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
             return pipeline_response
 
-        return AsyncItemPaged(get_next, extract_data)
-
-    list_by_location.metadata = {
-        "url": "/subscriptions/{subscriptionId}/providers/Microsoft.HDInsight/locations/{location}/availableClusterPoolVersions"
-    }
+        return ItemPaged(get_next, extract_data)
```

### Comparing `azure-mgmt-hdinsightcontainers-1.0.0b1/azure/mgmt/hdinsightcontainers/aio/operations/_available_cluster_versions_operations.py` & `azure-mgmt-hdinsightcontainers-1.0.0b2/azure/mgmt/hdinsightcontainers/aio/operations/_available_cluster_versions_operations.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=too-many-lines
+# pylint: disable=too-many-lines,too-many-statements
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
@@ -54,15 +54,14 @@
 
     @distributed_trace
     def list_by_location(self, location: str, **kwargs: Any) -> AsyncIterable["_models.ClusterVersion"]:
         """Returns a list of available cluster versions.
 
         :param location: The name of the Azure region. Required.
         :type location: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either ClusterVersion or the result of cls(response)
         :rtype:
          ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.hdinsightcontainers.models.ClusterVersion]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
@@ -77,64 +76,59 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         def prepare_request(next_link=None):
             if not next_link:
 
-                request = build_list_by_location_request(
+                _request = build_list_by_location_request(
                     location=location,
                     subscription_id=self._config.subscription_id,
                     api_version=api_version,
-                    template_url=self.list_by_location.metadata["url"],
                     headers=_headers,
                     params=_params,
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
 
             else:
                 # make call to next link with the client's api-version
                 _parsed_next_link = urllib.parse.urlparse(next_link)
                 _next_request_params = case_insensitive_dict(
                     {
                         key: [urllib.parse.quote(v) for v in value]
                         for key, value in urllib.parse.parse_qs(_parsed_next_link.query).items()
                     }
                 )
                 _next_request_params["api-version"] = self._config.api_version
-                request = HttpRequest(
+                _request = HttpRequest(
                     "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
-                request.method = "GET"
-            return request
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
+                _request.method = "GET"
+            return _request
 
         async def extract_data(pipeline_response):
             deserialized = self._deserialize("ClusterVersionsListResult", pipeline_response)
             list_of_elem = deserialized.value
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, AsyncList(list_of_elem)
 
         async def get_next(next_link=None):
-            request = prepare_request(next_link)
+            _request = prepare_request(next_link)
 
             _stream = False
             pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=_stream, **kwargs
+                _request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
             return pipeline_response
 
         return AsyncItemPaged(get_next, extract_data)
-
-    list_by_location.metadata = {
-        "url": "/subscriptions/{subscriptionId}/providers/Microsoft.HDInsight/locations/{location}/availableClusterVersions"
-    }
```

### Comparing `azure-mgmt-hdinsightcontainers-1.0.0b1/azure/mgmt/hdinsightcontainers/aio/operations/_cluster_jobs_operations.py` & `azure-mgmt-hdinsightcontainers-1.0.0b2/azure/mgmt/hdinsightcontainers/operations/_cluster_jobs_operations.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,71 +1,152 @@
-# pylint: disable=too-many-lines
+# pylint: disable=too-many-lines,too-many-statements
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 from io import IOBase
-from typing import Any, AsyncIterable, Callable, Dict, IO, Optional, TypeVar, Union, cast, overload
+from typing import Any, Callable, Dict, IO, Iterable, Optional, TypeVar, Union, cast, overload
 import urllib.parse
 
-from azure.core.async_paging import AsyncItemPaged, AsyncList
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
     ResourceNotFoundError,
     ResourceNotModifiedError,
     map_error,
 )
+from azure.core.paging import ItemPaged
 from azure.core.pipeline import PipelineResponse
-from azure.core.pipeline.transport import AsyncHttpResponse
-from azure.core.polling import AsyncLROPoller, AsyncNoPolling, AsyncPollingMethod
+from azure.core.pipeline.transport import HttpResponse
+from azure.core.polling import LROPoller, NoPolling, PollingMethod
 from azure.core.rest import HttpRequest
 from azure.core.tracing.decorator import distributed_trace
-from azure.core.tracing.decorator_async import distributed_trace_async
 from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
-from azure.mgmt.core.polling.async_arm_polling import AsyncARMPolling
+from azure.mgmt.core.polling.arm_polling import ARMPolling
 
-from ... import models as _models
-from ..._vendor import _convert_request
-from ...operations._cluster_jobs_operations import build_list_request, build_run_job_request
+from .. import models as _models
+from .._serialization import Serializer
+from .._vendor import _convert_request
 
 T = TypeVar("T")
-ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
+ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
+
+_SERIALIZER = Serializer()
+_SERIALIZER.client_side_validation = False
+
+
+def build_run_job_request(
+    resource_group_name: str, cluster_pool_name: str, cluster_name: str, subscription_id: str, **kwargs: Any
+) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+    _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-11-01-preview"))
+    content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+    accept = _headers.pop("Accept", "application/json")
+
+    # Construct URL
+    _url = kwargs.pop(
+        "template_url",
+        "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HDInsight/clusterpools/{clusterPoolName}/clusters/{clusterName}/runJob",
+    )  # pylint: disable=line-too-long
+    path_format_arguments = {
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
+        ),
+        "clusterPoolName": _SERIALIZER.url("cluster_pool_name", cluster_pool_name, "str"),
+        "clusterName": _SERIALIZER.url("cluster_name", cluster_name, "str"),
+    }
+
+    _url: str = _url.format(**path_format_arguments)  # type: ignore
+
+    # Construct parameters
+    _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
+
+    # Construct headers
+    if content_type is not None:
+        _headers["Content-Type"] = _SERIALIZER.header("content_type", content_type, "str")
+    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
+
+    return HttpRequest(method="POST", url=_url, params=_params, headers=_headers, **kwargs)
+
+
+def build_list_request(
+    resource_group_name: str,
+    cluster_pool_name: str,
+    cluster_name: str,
+    subscription_id: str,
+    *,
+    filter: Optional[str] = None,
+    **kwargs: Any
+) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+    _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-11-01-preview"))
+    accept = _headers.pop("Accept", "application/json")
+
+    # Construct URL
+    _url = kwargs.pop(
+        "template_url",
+        "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HDInsight/clusterpools/{clusterPoolName}/clusters/{clusterName}/jobs",
+    )  # pylint: disable=line-too-long
+    path_format_arguments = {
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
+        ),
+        "clusterPoolName": _SERIALIZER.url("cluster_pool_name", cluster_pool_name, "str"),
+        "clusterName": _SERIALIZER.url("cluster_name", cluster_name, "str"),
+    }
+
+    _url: str = _url.format(**path_format_arguments)  # type: ignore
+
+    # Construct parameters
+    _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
+    if filter is not None:
+        _params["$filter"] = _SERIALIZER.query("filter", filter, "str")
+
+    # Construct headers
+    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
+
+    return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
 
 
 class ClusterJobsOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
-        :class:`~azure.mgmt.hdinsightcontainers.aio.HDInsightContainersMgmtClient`'s
+        :class:`~azure.mgmt.hdinsightcontainers.HDInsightContainersMgmtClient`'s
         :attr:`cluster_jobs` attribute.
     """
 
     models = _models
 
-    def __init__(self, *args, **kwargs) -> None:
+    def __init__(self, *args, **kwargs):
         input_args = list(args)
         self._client = input_args.pop(0) if input_args else kwargs.pop("client")
         self._config = input_args.pop(0) if input_args else kwargs.pop("config")
         self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
         self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
 
-    async def _run_job_initial(
+    def _run_job_initial(
         self,
         resource_group_name: str,
         cluster_pool_name: str,
         cluster_name: str,
-        cluster_job: Union[_models.ClusterJob, IO],
+        cluster_job: Union[_models.ClusterJob, IO[bytes]],
         **kwargs: Any
     ) -> Optional[_models.ClusterJob]:
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -83,33 +164,32 @@
         _json = None
         _content = None
         if isinstance(cluster_job, (IOBase, bytes)):
             _content = cluster_job
         else:
             _json = self._serialize.body(cluster_job, "ClusterJob")
 
-        request = build_run_job_request(
+        _request = build_run_job_request(
             resource_group_name=resource_group_name,
             cluster_pool_name=cluster_pool_name,
             cluster_name=cluster_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             content_type=content_type,
             json=_json,
             content=_content,
-            template_url=self._run_job_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
-        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -120,147 +200,113 @@
         if response.status_code == 200:
             deserialized = self._deserialize("ClusterJob", pipeline_response)
 
         if response.status_code == 202:
             response_headers["location"] = self._deserialize("str", response.headers.get("location"))
 
         if cls:
-            return cls(pipeline_response, deserialized, response_headers)
-
-        return deserialized
+            return cls(pipeline_response, deserialized, response_headers)  # type: ignore
 
-    _run_job_initial.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HDInsight/clusterpools/{clusterPoolName}/clusters/{clusterName}/runJob"
-    }
+        return deserialized  # type: ignore
 
     @overload
-    async def begin_run_job(
+    def begin_run_job(
         self,
         resource_group_name: str,
         cluster_pool_name: str,
         cluster_name: str,
         cluster_job: _models.ClusterJob,
         *,
         content_type: str = "application/json",
         **kwargs: Any
-    ) -> AsyncLROPoller[_models.ClusterJob]:
+    ) -> LROPoller[_models.ClusterJob]:
         """Operations on jobs of HDInsight on AKS cluster.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param cluster_pool_name: The name of the cluster pool. Required.
         :type cluster_pool_name: str
         :param cluster_name: The name of the HDInsight cluster. Required.
         :type cluster_name: str
         :param cluster_job: The Cluster job. Required.
         :type cluster_job: ~azure.mgmt.hdinsightcontainers.models.ClusterJob
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
-         this operation to not poll, or pass in your own initialized polling object for a personal
-         polling strategy.
-        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
-        :return: An instance of AsyncLROPoller that returns either ClusterJob or the result of
-         cls(response)
-        :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.hdinsightcontainers.models.ClusterJob]
+        :return: An instance of LROPoller that returns either ClusterJob or the result of cls(response)
+        :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.hdinsightcontainers.models.ClusterJob]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
-    async def begin_run_job(
+    def begin_run_job(
         self,
         resource_group_name: str,
         cluster_pool_name: str,
         cluster_name: str,
-        cluster_job: IO,
+        cluster_job: IO[bytes],
         *,
         content_type: str = "application/json",
         **kwargs: Any
-    ) -> AsyncLROPoller[_models.ClusterJob]:
+    ) -> LROPoller[_models.ClusterJob]:
         """Operations on jobs of HDInsight on AKS cluster.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param cluster_pool_name: The name of the cluster pool. Required.
         :type cluster_pool_name: str
         :param cluster_name: The name of the HDInsight cluster. Required.
         :type cluster_name: str
         :param cluster_job: The Cluster job. Required.
-        :type cluster_job: IO
+        :type cluster_job: IO[bytes]
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
-         this operation to not poll, or pass in your own initialized polling object for a personal
-         polling strategy.
-        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
-        :return: An instance of AsyncLROPoller that returns either ClusterJob or the result of
-         cls(response)
-        :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.hdinsightcontainers.models.ClusterJob]
+        :return: An instance of LROPoller that returns either ClusterJob or the result of cls(response)
+        :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.hdinsightcontainers.models.ClusterJob]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
-    @distributed_trace_async
-    async def begin_run_job(
+    @distributed_trace
+    def begin_run_job(
         self,
         resource_group_name: str,
         cluster_pool_name: str,
         cluster_name: str,
-        cluster_job: Union[_models.ClusterJob, IO],
+        cluster_job: Union[_models.ClusterJob, IO[bytes]],
         **kwargs: Any
-    ) -> AsyncLROPoller[_models.ClusterJob]:
+    ) -> LROPoller[_models.ClusterJob]:
         """Operations on jobs of HDInsight on AKS cluster.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param cluster_pool_name: The name of the cluster pool. Required.
         :type cluster_pool_name: str
         :param cluster_name: The name of the HDInsight cluster. Required.
         :type cluster_name: str
-        :param cluster_job: The Cluster job. Is either a ClusterJob type or a IO type. Required.
-        :type cluster_job: ~azure.mgmt.hdinsightcontainers.models.ClusterJob or IO
-        :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
-         Default value is None.
-        :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
-         this operation to not poll, or pass in your own initialized polling object for a personal
-         polling strategy.
-        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
-        :return: An instance of AsyncLROPoller that returns either ClusterJob or the result of
-         cls(response)
-        :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.hdinsightcontainers.models.ClusterJob]
+        :param cluster_job: The Cluster job. Is either a ClusterJob type or a IO[bytes] type. Required.
+        :type cluster_job: ~azure.mgmt.hdinsightcontainers.models.ClusterJob or IO[bytes]
+        :return: An instance of LROPoller that returns either ClusterJob or the result of cls(response)
+        :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.hdinsightcontainers.models.ClusterJob]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.ClusterJob] = kwargs.pop("cls", None)
-        polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
+        polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
-            raw_result = await self._run_job_initial(
+            raw_result = self._run_job_initial(
                 resource_group_name=resource_group_name,
                 cluster_pool_name=cluster_pool_name,
                 cluster_name=cluster_name,
                 cluster_job=cluster_job,
                 api_version=api_version,
                 content_type=content_type,
                 cls=lambda x, y, z: x,
@@ -269,55 +315,59 @@
                 **kwargs
             )
         kwargs.pop("error_map", None)
 
         def get_long_running_output(pipeline_response):
             deserialized = self._deserialize("ClusterJob", pipeline_response)
             if cls:
-                return cls(pipeline_response, deserialized, {})
+                return cls(pipeline_response, deserialized, {})  # type: ignore
             return deserialized
 
         if polling is True:
-            polling_method: AsyncPollingMethod = cast(
-                AsyncPollingMethod, AsyncARMPolling(lro_delay, lro_options={"final-state-via": "location"}, **kwargs)
+            polling_method: PollingMethod = cast(
+                PollingMethod, ARMPolling(lro_delay, lro_options={"final-state-via": "location"}, **kwargs)
             )
         elif polling is False:
-            polling_method = cast(AsyncPollingMethod, AsyncNoPolling())
+            polling_method = cast(PollingMethod, NoPolling())
         else:
             polling_method = polling
         if cont_token:
-            return AsyncLROPoller.from_continuation_token(
+            return LROPoller[_models.ClusterJob].from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
                 deserialization_callback=get_long_running_output,
             )
-        return AsyncLROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
-
-    begin_run_job.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HDInsight/clusterpools/{clusterPoolName}/clusters/{clusterName}/runJob"
-    }
+        return LROPoller[_models.ClusterJob](
+            self._client, raw_result, get_long_running_output, polling_method  # type: ignore
+        )
 
     @distributed_trace
     def list(
-        self, resource_group_name: str, cluster_pool_name: str, cluster_name: str, **kwargs: Any
-    ) -> AsyncIterable["_models.ClusterJob"]:
+        self,
+        resource_group_name: str,
+        cluster_pool_name: str,
+        cluster_name: str,
+        filter: Optional[str] = None,
+        **kwargs: Any
+    ) -> Iterable["_models.ClusterJob"]:
         """Get jobs of HDInsight on AKS cluster.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param cluster_pool_name: The name of the cluster pool. Required.
         :type cluster_pool_name: str
         :param cluster_name: The name of the HDInsight cluster. Required.
         :type cluster_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
+        :param filter: The system query option to filter job returned in the response. Allowed value is
+         'jobName eq {jobName}' or 'jarName eq {jarName}'. Default value is None.
+        :type filter: str
         :return: An iterator like instance of either ClusterJob or the result of cls(response)
-        :rtype:
-         ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.hdinsightcontainers.models.ClusterJob]
+        :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.hdinsightcontainers.models.ClusterJob]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.ClusterJobList] = kwargs.pop("cls", None)
@@ -329,66 +379,62 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         def prepare_request(next_link=None):
             if not next_link:
 
-                request = build_list_request(
+                _request = build_list_request(
                     resource_group_name=resource_group_name,
                     cluster_pool_name=cluster_pool_name,
                     cluster_name=cluster_name,
                     subscription_id=self._config.subscription_id,
+                    filter=filter,
                     api_version=api_version,
-                    template_url=self.list.metadata["url"],
                     headers=_headers,
                     params=_params,
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
 
             else:
                 # make call to next link with the client's api-version
                 _parsed_next_link = urllib.parse.urlparse(next_link)
                 _next_request_params = case_insensitive_dict(
                     {
                         key: [urllib.parse.quote(v) for v in value]
                         for key, value in urllib.parse.parse_qs(_parsed_next_link.query).items()
                     }
                 )
                 _next_request_params["api-version"] = self._config.api_version
-                request = HttpRequest(
+                _request = HttpRequest(
                     "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
-                request.method = "GET"
-            return request
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
+                _request.method = "GET"
+            return _request
 
-        async def extract_data(pipeline_response):
+        def extract_data(pipeline_response):
             deserialized = self._deserialize("ClusterJobList", pipeline_response)
             list_of_elem = deserialized.value
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
-            return deserialized.next_link or None, AsyncList(list_of_elem)
+            return deserialized.next_link or None, iter(list_of_elem)
 
-        async def get_next(next_link=None):
-            request = prepare_request(next_link)
+        def get_next(next_link=None):
+            _request = prepare_request(next_link)
 
             _stream = False
-            pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=_stream, **kwargs
+            pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+                _request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
             return pipeline_response
 
-        return AsyncItemPaged(get_next, extract_data)
-
-    list.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HDInsight/clusterpools/{clusterPoolName}/clusters/{clusterName}/jobs"
-    }
+        return ItemPaged(get_next, extract_data)
```

### Comparing `azure-mgmt-hdinsightcontainers-1.0.0b1/azure/mgmt/hdinsightcontainers/aio/operations/_cluster_pools_operations.py` & `azure-mgmt-hdinsightcontainers-1.0.0b2/azure/mgmt/hdinsightcontainers/aio/operations/_cluster_pools_operations.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=too-many-lines
+# pylint: disable=too-many-lines,too-many-statements
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
@@ -34,14 +34,15 @@
 from ...operations._cluster_pools_operations import (
     build_create_or_update_request,
     build_delete_request,
     build_get_request,
     build_list_by_resource_group_request,
     build_list_by_subscription_request,
     build_update_tags_request,
+    build_upgrade_request,
 )
 
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 
 class ClusterPoolsOperations:
@@ -68,15 +69,14 @@
         """Gets a cluster pool.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param cluster_pool_name: The name of the cluster pool. Required.
         :type cluster_pool_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: ClusterPool or the result of cls(response)
         :rtype: ~azure.mgmt.hdinsightcontainers.models.ClusterPool
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -87,54 +87,49 @@
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.ClusterPool] = kwargs.pop("cls", None)
 
-        request = build_get_request(
+        _request = build_get_request(
             resource_group_name=resource_group_name,
             cluster_pool_name=cluster_pool_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
-            template_url=self.get.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         deserialized = self._deserialize("ClusterPool", pipeline_response)
 
         if cls:
-            return cls(pipeline_response, deserialized, {})
-
-        return deserialized
+            return cls(pipeline_response, deserialized, {})  # type: ignore
 
-    get.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HDInsight/clusterpools/{clusterPoolName}"
-    }
+        return deserialized  # type: ignore
 
     async def _create_or_update_initial(
         self,
         resource_group_name: str,
         cluster_pool_name: str,
-        cluster_pool: Union[_models.ClusterPool, IO],
+        cluster_pool: Union[_models.ClusterPool, IO[bytes]],
         **kwargs: Any
     ) -> _models.ClusterPool:
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -152,32 +147,31 @@
         _json = None
         _content = None
         if isinstance(cluster_pool, (IOBase, bytes)):
             _content = cluster_pool
         else:
             _json = self._serialize.body(cluster_pool, "ClusterPool")
 
-        request = build_create_or_update_request(
+        _request = build_create_or_update_request(
             resource_group_name=resource_group_name,
             cluster_pool_name=cluster_pool_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             content_type=content_type,
             json=_json,
             content=_content,
-            template_url=self._create_or_update_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 201]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -190,18 +184,14 @@
             deserialized = self._deserialize("ClusterPool", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})  # type: ignore
 
         return deserialized  # type: ignore
 
-    _create_or_update_initial.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HDInsight/clusterpools/{clusterPoolName}"
-    }
-
     @overload
     async def begin_create_or_update(
         self,
         resource_group_name: str,
         cluster_pool_name: str,
         cluster_pool: _models.ClusterPool,
         *,
@@ -216,93 +206,66 @@
         :param cluster_pool_name: The name of the cluster pool. Required.
         :type cluster_pool_name: str
         :param cluster_pool: The Cluster Pool to create. Required.
         :type cluster_pool: ~azure.mgmt.hdinsightcontainers.models.ClusterPool
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
-         this operation to not poll, or pass in your own initialized polling object for a personal
-         polling strategy.
-        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
         :return: An instance of AsyncLROPoller that returns either ClusterPool or the result of
          cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.hdinsightcontainers.models.ClusterPool]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
     async def begin_create_or_update(
         self,
         resource_group_name: str,
         cluster_pool_name: str,
-        cluster_pool: IO,
+        cluster_pool: IO[bytes],
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> AsyncLROPoller[_models.ClusterPool]:
         """Creates or updates a cluster pool.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param cluster_pool_name: The name of the cluster pool. Required.
         :type cluster_pool_name: str
         :param cluster_pool: The Cluster Pool to create. Required.
-        :type cluster_pool: IO
+        :type cluster_pool: IO[bytes]
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
-         this operation to not poll, or pass in your own initialized polling object for a personal
-         polling strategy.
-        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
         :return: An instance of AsyncLROPoller that returns either ClusterPool or the result of
          cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.hdinsightcontainers.models.ClusterPool]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace_async
     async def begin_create_or_update(
         self,
         resource_group_name: str,
         cluster_pool_name: str,
-        cluster_pool: Union[_models.ClusterPool, IO],
+        cluster_pool: Union[_models.ClusterPool, IO[bytes]],
         **kwargs: Any
     ) -> AsyncLROPoller[_models.ClusterPool]:
         """Creates or updates a cluster pool.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param cluster_pool_name: The name of the cluster pool. Required.
         :type cluster_pool_name: str
-        :param cluster_pool: The Cluster Pool to create. Is either a ClusterPool type or a IO type.
-         Required.
-        :type cluster_pool: ~azure.mgmt.hdinsightcontainers.models.ClusterPool or IO
-        :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
-         Default value is None.
-        :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
-         this operation to not poll, or pass in your own initialized polling object for a personal
-         polling strategy.
-        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
+        :param cluster_pool: The Cluster Pool to create. Is either a ClusterPool type or a IO[bytes]
+         type. Required.
+        :type cluster_pool: ~azure.mgmt.hdinsightcontainers.models.ClusterPool or IO[bytes]
         :return: An instance of AsyncLROPoller that returns either ClusterPool or the result of
          cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.hdinsightcontainers.models.ClusterPool]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
@@ -326,44 +289,42 @@
                 **kwargs
             )
         kwargs.pop("error_map", None)
 
         def get_long_running_output(pipeline_response):
             deserialized = self._deserialize("ClusterPool", pipeline_response)
             if cls:
-                return cls(pipeline_response, deserialized, {})
+                return cls(pipeline_response, deserialized, {})  # type: ignore
             return deserialized
 
         if polling is True:
             polling_method: AsyncPollingMethod = cast(
                 AsyncPollingMethod,
                 AsyncARMPolling(lro_delay, lro_options={"final-state-via": "azure-async-operation"}, **kwargs),
             )
         elif polling is False:
             polling_method = cast(AsyncPollingMethod, AsyncNoPolling())
         else:
             polling_method = polling
         if cont_token:
-            return AsyncLROPoller.from_continuation_token(
+            return AsyncLROPoller[_models.ClusterPool].from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
                 deserialization_callback=get_long_running_output,
             )
-        return AsyncLROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
-
-    begin_create_or_update.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HDInsight/clusterpools/{clusterPoolName}"
-    }
+        return AsyncLROPoller[_models.ClusterPool](
+            self._client, raw_result, get_long_running_output, polling_method  # type: ignore
+        )
 
     async def _update_tags_initial(
         self,
         resource_group_name: str,
         cluster_pool_name: str,
-        cluster_pool_tags: Union[_models.TagsObject, IO],
+        cluster_pool_tags: Union[_models.TagsObject, IO[bytes]],
         **kwargs: Any
     ) -> _models.ClusterPool:
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -381,32 +342,31 @@
         _json = None
         _content = None
         if isinstance(cluster_pool_tags, (IOBase, bytes)):
             _content = cluster_pool_tags
         else:
             _json = self._serialize.body(cluster_pool_tags, "TagsObject")
 
-        request = build_update_tags_request(
+        _request = build_update_tags_request(
             resource_group_name=resource_group_name,
             cluster_pool_name=cluster_pool_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             content_type=content_type,
             json=_json,
             content=_content,
-            template_url=self._update_tags_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -422,18 +382,14 @@
             deserialized = self._deserialize("ClusterPool", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, response_headers)  # type: ignore
 
         return deserialized  # type: ignore
 
-    _update_tags_initial.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HDInsight/clusterpools/{clusterPoolName}"
-    }
-
     @overload
     async def begin_update_tags(
         self,
         resource_group_name: str,
         cluster_pool_name: str,
         cluster_pool_tags: _models.TagsObject,
         *,
@@ -448,93 +404,66 @@
         :param cluster_pool_name: The name of the cluster pool. Required.
         :type cluster_pool_name: str
         :param cluster_pool_tags: Parameters supplied to update tags. Required.
         :type cluster_pool_tags: ~azure.mgmt.hdinsightcontainers.models.TagsObject
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
-         this operation to not poll, or pass in your own initialized polling object for a personal
-         polling strategy.
-        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
         :return: An instance of AsyncLROPoller that returns either ClusterPool or the result of
          cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.hdinsightcontainers.models.ClusterPool]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
     async def begin_update_tags(
         self,
         resource_group_name: str,
         cluster_pool_name: str,
-        cluster_pool_tags: IO,
+        cluster_pool_tags: IO[bytes],
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> AsyncLROPoller[_models.ClusterPool]:
         """Updates an existing Cluster Pool Tags.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param cluster_pool_name: The name of the cluster pool. Required.
         :type cluster_pool_name: str
         :param cluster_pool_tags: Parameters supplied to update tags. Required.
-        :type cluster_pool_tags: IO
+        :type cluster_pool_tags: IO[bytes]
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
-         this operation to not poll, or pass in your own initialized polling object for a personal
-         polling strategy.
-        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
         :return: An instance of AsyncLROPoller that returns either ClusterPool or the result of
          cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.hdinsightcontainers.models.ClusterPool]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace_async
     async def begin_update_tags(
         self,
         resource_group_name: str,
         cluster_pool_name: str,
-        cluster_pool_tags: Union[_models.TagsObject, IO],
+        cluster_pool_tags: Union[_models.TagsObject, IO[bytes]],
         **kwargs: Any
     ) -> AsyncLROPoller[_models.ClusterPool]:
         """Updates an existing Cluster Pool Tags.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param cluster_pool_name: The name of the cluster pool. Required.
         :type cluster_pool_name: str
         :param cluster_pool_tags: Parameters supplied to update tags. Is either a TagsObject type or a
-         IO type. Required.
-        :type cluster_pool_tags: ~azure.mgmt.hdinsightcontainers.models.TagsObject or IO
-        :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
-         Default value is None.
-        :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
-         this operation to not poll, or pass in your own initialized polling object for a personal
-         polling strategy.
-        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
+         IO[bytes] type. Required.
+        :type cluster_pool_tags: ~azure.mgmt.hdinsightcontainers.models.TagsObject or IO[bytes]
         :return: An instance of AsyncLROPoller that returns either ClusterPool or the result of
          cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.hdinsightcontainers.models.ClusterPool]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
@@ -558,38 +487,36 @@
                 **kwargs
             )
         kwargs.pop("error_map", None)
 
         def get_long_running_output(pipeline_response):
             deserialized = self._deserialize("ClusterPool", pipeline_response)
             if cls:
-                return cls(pipeline_response, deserialized, {})
+                return cls(pipeline_response, deserialized, {})  # type: ignore
             return deserialized
 
         if polling is True:
             polling_method: AsyncPollingMethod = cast(
                 AsyncPollingMethod,
                 AsyncARMPolling(lro_delay, lro_options={"final-state-via": "azure-async-operation"}, **kwargs),
             )
         elif polling is False:
             polling_method = cast(AsyncPollingMethod, AsyncNoPolling())
         else:
             polling_method = polling
         if cont_token:
-            return AsyncLROPoller.from_continuation_token(
+            return AsyncLROPoller[_models.ClusterPool].from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
                 deserialization_callback=get_long_running_output,
             )
-        return AsyncLROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
-
-    begin_update_tags.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HDInsight/clusterpools/{clusterPoolName}"
-    }
+        return AsyncLROPoller[_models.ClusterPool](
+            self._client, raw_result, get_long_running_output, polling_method  # type: ignore
+        )
 
     async def _delete_initial(  # pylint: disable=inconsistent-return-statements
         self, resource_group_name: str, cluster_pool_name: str, **kwargs: Any
     ) -> None:
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -600,68 +527,55 @@
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
-        request = build_delete_request(
+        _request = build_delete_request(
             resource_group_name=resource_group_name,
             cluster_pool_name=cluster_pool_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
-            template_url=self._delete_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         response_headers = {}
         if response.status_code == 202:
             response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
 
         if cls:
-            return cls(pipeline_response, None, response_headers)
-
-    _delete_initial.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HDInsight/clusterpools/{clusterPoolName}"
-    }
+            return cls(pipeline_response, None, response_headers)  # type: ignore
 
     @distributed_trace_async
     async def begin_delete(
         self, resource_group_name: str, cluster_pool_name: str, **kwargs: Any
     ) -> AsyncLROPoller[None]:
         """Deletes a Cluster Pool.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param cluster_pool_name: The name of the cluster pool. Required.
         :type cluster_pool_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
-         this operation to not poll, or pass in your own initialized polling object for a personal
-         polling strategy.
-        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
         :return: An instance of AsyncLROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
@@ -680,40 +594,35 @@
                 params=_params,
                 **kwargs
             )
         kwargs.pop("error_map", None)
 
         def get_long_running_output(pipeline_response):  # pylint: disable=inconsistent-return-statements
             if cls:
-                return cls(pipeline_response, None, {})
+                return cls(pipeline_response, None, {})  # type: ignore
 
         if polling is True:
             polling_method: AsyncPollingMethod = cast(AsyncPollingMethod, AsyncARMPolling(lro_delay, **kwargs))
         elif polling is False:
             polling_method = cast(AsyncPollingMethod, AsyncNoPolling())
         else:
             polling_method = polling
         if cont_token:
-            return AsyncLROPoller.from_continuation_token(
+            return AsyncLROPoller[None].from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
                 deserialization_callback=get_long_running_output,
             )
-        return AsyncLROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
-
-    begin_delete.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HDInsight/clusterpools/{clusterPoolName}"
-    }
+        return AsyncLROPoller[None](self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
 
     @distributed_trace
     def list_by_subscription(self, **kwargs: Any) -> AsyncIterable["_models.ClusterPool"]:
         """Gets the list of Cluster Pools within a Subscription.
 
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either ClusterPool or the result of cls(response)
         :rtype:
          ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.hdinsightcontainers.models.ClusterPool]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
@@ -728,79 +637,73 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         def prepare_request(next_link=None):
             if not next_link:
 
-                request = build_list_by_subscription_request(
+                _request = build_list_by_subscription_request(
                     subscription_id=self._config.subscription_id,
                     api_version=api_version,
-                    template_url=self.list_by_subscription.metadata["url"],
                     headers=_headers,
                     params=_params,
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
 
             else:
                 # make call to next link with the client's api-version
                 _parsed_next_link = urllib.parse.urlparse(next_link)
                 _next_request_params = case_insensitive_dict(
                     {
                         key: [urllib.parse.quote(v) for v in value]
                         for key, value in urllib.parse.parse_qs(_parsed_next_link.query).items()
                     }
                 )
                 _next_request_params["api-version"] = self._config.api_version
-                request = HttpRequest(
+                _request = HttpRequest(
                     "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
-                request.method = "GET"
-            return request
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
+                _request.method = "GET"
+            return _request
 
         async def extract_data(pipeline_response):
             deserialized = self._deserialize("ClusterPoolListResult", pipeline_response)
             list_of_elem = deserialized.value
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, AsyncList(list_of_elem)
 
         async def get_next(next_link=None):
-            request = prepare_request(next_link)
+            _request = prepare_request(next_link)
 
             _stream = False
             pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=_stream, **kwargs
+                _request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
             return pipeline_response
 
         return AsyncItemPaged(get_next, extract_data)
 
-    list_by_subscription.metadata = {
-        "url": "/subscriptions/{subscriptionId}/providers/Microsoft.HDInsight/clusterpools"
-    }
-
     @distributed_trace
     def list_by_resource_group(self, resource_group_name: str, **kwargs: Any) -> AsyncIterable["_models.ClusterPool"]:
         """Lists the HDInsight cluster pools under a resource group.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either ClusterPool or the result of cls(response)
         :rtype:
          ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.hdinsightcontainers.models.ClusterPool]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
@@ -815,64 +718,256 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         def prepare_request(next_link=None):
             if not next_link:
 
-                request = build_list_by_resource_group_request(
+                _request = build_list_by_resource_group_request(
                     resource_group_name=resource_group_name,
                     subscription_id=self._config.subscription_id,
                     api_version=api_version,
-                    template_url=self.list_by_resource_group.metadata["url"],
                     headers=_headers,
                     params=_params,
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
 
             else:
                 # make call to next link with the client's api-version
                 _parsed_next_link = urllib.parse.urlparse(next_link)
                 _next_request_params = case_insensitive_dict(
                     {
                         key: [urllib.parse.quote(v) for v in value]
                         for key, value in urllib.parse.parse_qs(_parsed_next_link.query).items()
                     }
                 )
                 _next_request_params["api-version"] = self._config.api_version
-                request = HttpRequest(
+                _request = HttpRequest(
                     "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
-                request.method = "GET"
-            return request
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
+                _request.method = "GET"
+            return _request
 
         async def extract_data(pipeline_response):
             deserialized = self._deserialize("ClusterPoolListResult", pipeline_response)
             list_of_elem = deserialized.value
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, AsyncList(list_of_elem)
 
         async def get_next(next_link=None):
-            request = prepare_request(next_link)
+            _request = prepare_request(next_link)
 
             _stream = False
             pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=_stream, **kwargs
+                _request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
             return pipeline_response
 
         return AsyncItemPaged(get_next, extract_data)
 
-    list_by_resource_group.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HDInsight/clusterpools"
-    }
+    async def _upgrade_initial(
+        self,
+        resource_group_name: str,
+        cluster_pool_name: str,
+        cluster_pool_upgrade_request: Union[_models.ClusterPoolUpgrade, IO[bytes]],
+        **kwargs: Any
+    ) -> Optional[_models.ClusterPool]:
+        error_map = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[Optional[_models.ClusterPool]] = kwargs.pop("cls", None)
+
+        content_type = content_type or "application/json"
+        _json = None
+        _content = None
+        if isinstance(cluster_pool_upgrade_request, (IOBase, bytes)):
+            _content = cluster_pool_upgrade_request
+        else:
+            _json = self._serialize.body(cluster_pool_upgrade_request, "ClusterPoolUpgrade")
+
+        _request = build_upgrade_request(
+            resource_group_name=resource_group_name,
+            cluster_pool_name=cluster_pool_name,
+            subscription_id=self._config.subscription_id,
+            api_version=api_version,
+            content_type=content_type,
+            json=_json,
+            content=_content,
+            headers=_headers,
+            params=_params,
+        )
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+            _request, stream=_stream, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200, 202]:
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
+            raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
+
+        deserialized = None
+        response_headers = {}
+        if response.status_code == 200:
+            deserialized = self._deserialize("ClusterPool", pipeline_response)
+
+        if response.status_code == 202:
+            response_headers["location"] = self._deserialize("str", response.headers.get("location"))
+
+        if cls:
+            return cls(pipeline_response, deserialized, response_headers)  # type: ignore
+
+        return deserialized  # type: ignore
+
+    @overload
+    async def begin_upgrade(
+        self,
+        resource_group_name: str,
+        cluster_pool_name: str,
+        cluster_pool_upgrade_request: _models.ClusterPoolUpgrade,
+        *,
+        content_type: str = "application/json",
+        **kwargs: Any
+    ) -> AsyncLROPoller[_models.ClusterPool]:
+        """Upgrade a cluster pool.
+
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
+        :type resource_group_name: str
+        :param cluster_pool_name: The name of the cluster pool. Required.
+        :type cluster_pool_name: str
+        :param cluster_pool_upgrade_request: Upgrade a cluster pool. Required.
+        :type cluster_pool_upgrade_request: ~azure.mgmt.hdinsightcontainers.models.ClusterPoolUpgrade
+        :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: An instance of AsyncLROPoller that returns either ClusterPool or the result of
+         cls(response)
+        :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.hdinsightcontainers.models.ClusterPool]
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @overload
+    async def begin_upgrade(
+        self,
+        resource_group_name: str,
+        cluster_pool_name: str,
+        cluster_pool_upgrade_request: IO[bytes],
+        *,
+        content_type: str = "application/json",
+        **kwargs: Any
+    ) -> AsyncLROPoller[_models.ClusterPool]:
+        """Upgrade a cluster pool.
+
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
+        :type resource_group_name: str
+        :param cluster_pool_name: The name of the cluster pool. Required.
+        :type cluster_pool_name: str
+        :param cluster_pool_upgrade_request: Upgrade a cluster pool. Required.
+        :type cluster_pool_upgrade_request: IO[bytes]
+        :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: An instance of AsyncLROPoller that returns either ClusterPool or the result of
+         cls(response)
+        :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.hdinsightcontainers.models.ClusterPool]
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @distributed_trace_async
+    async def begin_upgrade(
+        self,
+        resource_group_name: str,
+        cluster_pool_name: str,
+        cluster_pool_upgrade_request: Union[_models.ClusterPoolUpgrade, IO[bytes]],
+        **kwargs: Any
+    ) -> AsyncLROPoller[_models.ClusterPool]:
+        """Upgrade a cluster pool.
+
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
+        :type resource_group_name: str
+        :param cluster_pool_name: The name of the cluster pool. Required.
+        :type cluster_pool_name: str
+        :param cluster_pool_upgrade_request: Upgrade a cluster pool. Is either a ClusterPoolUpgrade
+         type or a IO[bytes] type. Required.
+        :type cluster_pool_upgrade_request: ~azure.mgmt.hdinsightcontainers.models.ClusterPoolUpgrade
+         or IO[bytes]
+        :return: An instance of AsyncLROPoller that returns either ClusterPool or the result of
+         cls(response)
+        :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.hdinsightcontainers.models.ClusterPool]
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[_models.ClusterPool] = kwargs.pop("cls", None)
+        polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
+        lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
+        cont_token: Optional[str] = kwargs.pop("continuation_token", None)
+        if cont_token is None:
+            raw_result = await self._upgrade_initial(
+                resource_group_name=resource_group_name,
+                cluster_pool_name=cluster_pool_name,
+                cluster_pool_upgrade_request=cluster_pool_upgrade_request,
+                api_version=api_version,
+                content_type=content_type,
+                cls=lambda x, y, z: x,
+                headers=_headers,
+                params=_params,
+                **kwargs
+            )
+        kwargs.pop("error_map", None)
+
+        def get_long_running_output(pipeline_response):
+            deserialized = self._deserialize("ClusterPool", pipeline_response)
+            if cls:
+                return cls(pipeline_response, deserialized, {})  # type: ignore
+            return deserialized
+
+        if polling is True:
+            polling_method: AsyncPollingMethod = cast(
+                AsyncPollingMethod, AsyncARMPolling(lro_delay, lro_options={"final-state-via": "location"}, **kwargs)
+            )
+        elif polling is False:
+            polling_method = cast(AsyncPollingMethod, AsyncNoPolling())
+        else:
+            polling_method = polling
+        if cont_token:
+            return AsyncLROPoller[_models.ClusterPool].from_continuation_token(
+                polling_method=polling_method,
+                continuation_token=cont_token,
+                client=self._client,
+                deserialization_callback=get_long_running_output,
+            )
+        return AsyncLROPoller[_models.ClusterPool](
+            self._client, raw_result, get_long_running_output, polling_method  # type: ignore
+        )
```

### Comparing `azure-mgmt-hdinsightcontainers-1.0.0b1/azure/mgmt/hdinsightcontainers/aio/operations/_clusters_operations.py` & `azure-mgmt-hdinsightcontainers-1.0.0b2/azure/mgmt/hdinsightcontainers/aio/operations/_clusters_operations.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=too-many-lines
+# pylint: disable=too-many-lines,too-many-statements
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
@@ -37,14 +37,15 @@
     build_get_instance_view_request,
     build_get_request,
     build_list_by_cluster_pool_name_request,
     build_list_instance_views_request,
     build_list_service_configs_request,
     build_resize_request,
     build_update_request,
+    build_upgrade_request,
 )
 
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 
 class ClustersOperations:
@@ -73,15 +74,14 @@
         """Lists the HDInsight cluster pools under a resource group.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param cluster_pool_name: The name of the cluster pool. Required.
         :type cluster_pool_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either Cluster or the result of cls(response)
         :rtype: ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.hdinsightcontainers.models.Cluster]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
@@ -95,79 +95,283 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         def prepare_request(next_link=None):
             if not next_link:
 
-                request = build_list_by_cluster_pool_name_request(
+                _request = build_list_by_cluster_pool_name_request(
                     resource_group_name=resource_group_name,
                     cluster_pool_name=cluster_pool_name,
                     subscription_id=self._config.subscription_id,
                     api_version=api_version,
-                    template_url=self.list_by_cluster_pool_name.metadata["url"],
                     headers=_headers,
                     params=_params,
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
 
             else:
                 # make call to next link with the client's api-version
                 _parsed_next_link = urllib.parse.urlparse(next_link)
                 _next_request_params = case_insensitive_dict(
                     {
                         key: [urllib.parse.quote(v) for v in value]
                         for key, value in urllib.parse.parse_qs(_parsed_next_link.query).items()
                     }
                 )
                 _next_request_params["api-version"] = self._config.api_version
-                request = HttpRequest(
+                _request = HttpRequest(
                     "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
-                request.method = "GET"
-            return request
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
+                _request.method = "GET"
+            return _request
 
         async def extract_data(pipeline_response):
             deserialized = self._deserialize("ClusterListResult", pipeline_response)
             list_of_elem = deserialized.value
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, AsyncList(list_of_elem)
 
         async def get_next(next_link=None):
-            request = prepare_request(next_link)
+            _request = prepare_request(next_link)
 
             _stream = False
             pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=_stream, **kwargs
+                _request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
             return pipeline_response
 
         return AsyncItemPaged(get_next, extract_data)
 
-    list_by_cluster_pool_name.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HDInsight/clusterpools/{clusterPoolName}/clusters"
-    }
+    async def _upgrade_initial(
+        self,
+        resource_group_name: str,
+        cluster_pool_name: str,
+        cluster_name: str,
+        cluster_upgrade_request: Union[_models.ClusterUpgrade, IO[bytes]],
+        **kwargs: Any
+    ) -> Optional[_models.Cluster]:
+        error_map = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[Optional[_models.Cluster]] = kwargs.pop("cls", None)
+
+        content_type = content_type or "application/json"
+        _json = None
+        _content = None
+        if isinstance(cluster_upgrade_request, (IOBase, bytes)):
+            _content = cluster_upgrade_request
+        else:
+            _json = self._serialize.body(cluster_upgrade_request, "ClusterUpgrade")
+
+        _request = build_upgrade_request(
+            resource_group_name=resource_group_name,
+            cluster_pool_name=cluster_pool_name,
+            cluster_name=cluster_name,
+            subscription_id=self._config.subscription_id,
+            api_version=api_version,
+            content_type=content_type,
+            json=_json,
+            content=_content,
+            headers=_headers,
+            params=_params,
+        )
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+            _request, stream=_stream, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200, 202]:
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
+            raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
+
+        deserialized = None
+        response_headers = {}
+        if response.status_code == 200:
+            deserialized = self._deserialize("Cluster", pipeline_response)
+
+        if response.status_code == 202:
+            response_headers["location"] = self._deserialize("str", response.headers.get("location"))
+
+        if cls:
+            return cls(pipeline_response, deserialized, response_headers)  # type: ignore
+
+        return deserialized  # type: ignore
+
+    @overload
+    async def begin_upgrade(
+        self,
+        resource_group_name: str,
+        cluster_pool_name: str,
+        cluster_name: str,
+        cluster_upgrade_request: _models.ClusterUpgrade,
+        *,
+        content_type: str = "application/json",
+        **kwargs: Any
+    ) -> AsyncLROPoller[_models.Cluster]:
+        """Upgrade a cluster.
+
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
+        :type resource_group_name: str
+        :param cluster_pool_name: The name of the cluster pool. Required.
+        :type cluster_pool_name: str
+        :param cluster_name: The name of the HDInsight cluster. Required.
+        :type cluster_name: str
+        :param cluster_upgrade_request: Upgrade a cluster. Required.
+        :type cluster_upgrade_request: ~azure.mgmt.hdinsightcontainers.models.ClusterUpgrade
+        :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: An instance of AsyncLROPoller that returns either Cluster or the result of
+         cls(response)
+        :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.hdinsightcontainers.models.Cluster]
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @overload
+    async def begin_upgrade(
+        self,
+        resource_group_name: str,
+        cluster_pool_name: str,
+        cluster_name: str,
+        cluster_upgrade_request: IO[bytes],
+        *,
+        content_type: str = "application/json",
+        **kwargs: Any
+    ) -> AsyncLROPoller[_models.Cluster]:
+        """Upgrade a cluster.
+
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
+        :type resource_group_name: str
+        :param cluster_pool_name: The name of the cluster pool. Required.
+        :type cluster_pool_name: str
+        :param cluster_name: The name of the HDInsight cluster. Required.
+        :type cluster_name: str
+        :param cluster_upgrade_request: Upgrade a cluster. Required.
+        :type cluster_upgrade_request: IO[bytes]
+        :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: An instance of AsyncLROPoller that returns either Cluster or the result of
+         cls(response)
+        :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.hdinsightcontainers.models.Cluster]
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @distributed_trace_async
+    async def begin_upgrade(
+        self,
+        resource_group_name: str,
+        cluster_pool_name: str,
+        cluster_name: str,
+        cluster_upgrade_request: Union[_models.ClusterUpgrade, IO[bytes]],
+        **kwargs: Any
+    ) -> AsyncLROPoller[_models.Cluster]:
+        """Upgrade a cluster.
+
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
+        :type resource_group_name: str
+        :param cluster_pool_name: The name of the cluster pool. Required.
+        :type cluster_pool_name: str
+        :param cluster_name: The name of the HDInsight cluster. Required.
+        :type cluster_name: str
+        :param cluster_upgrade_request: Upgrade a cluster. Is either a ClusterUpgrade type or a
+         IO[bytes] type. Required.
+        :type cluster_upgrade_request: ~azure.mgmt.hdinsightcontainers.models.ClusterUpgrade or
+         IO[bytes]
+        :return: An instance of AsyncLROPoller that returns either Cluster or the result of
+         cls(response)
+        :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.hdinsightcontainers.models.Cluster]
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[_models.Cluster] = kwargs.pop("cls", None)
+        polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
+        lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
+        cont_token: Optional[str] = kwargs.pop("continuation_token", None)
+        if cont_token is None:
+            raw_result = await self._upgrade_initial(
+                resource_group_name=resource_group_name,
+                cluster_pool_name=cluster_pool_name,
+                cluster_name=cluster_name,
+                cluster_upgrade_request=cluster_upgrade_request,
+                api_version=api_version,
+                content_type=content_type,
+                cls=lambda x, y, z: x,
+                headers=_headers,
+                params=_params,
+                **kwargs
+            )
+        kwargs.pop("error_map", None)
+
+        def get_long_running_output(pipeline_response):
+            deserialized = self._deserialize("Cluster", pipeline_response)
+            if cls:
+                return cls(pipeline_response, deserialized, {})  # type: ignore
+            return deserialized
+
+        if polling is True:
+            polling_method: AsyncPollingMethod = cast(
+                AsyncPollingMethod, AsyncARMPolling(lro_delay, lro_options={"final-state-via": "location"}, **kwargs)
+            )
+        elif polling is False:
+            polling_method = cast(AsyncPollingMethod, AsyncNoPolling())
+        else:
+            polling_method = polling
+        if cont_token:
+            return AsyncLROPoller[_models.Cluster].from_continuation_token(
+                polling_method=polling_method,
+                continuation_token=cont_token,
+                client=self._client,
+                deserialization_callback=get_long_running_output,
+            )
+        return AsyncLROPoller[_models.Cluster](
+            self._client, raw_result, get_long_running_output, polling_method  # type: ignore
+        )
 
     async def _resize_initial(
         self,
         resource_group_name: str,
         cluster_pool_name: str,
         cluster_name: str,
-        cluster_resize_request: Union[_models.ClusterResizeData, IO],
+        cluster_resize_request: Union[_models.ClusterResizeData, IO[bytes]],
         **kwargs: Any
     ) -> Optional[_models.Cluster]:
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -185,33 +389,32 @@
         _json = None
         _content = None
         if isinstance(cluster_resize_request, (IOBase, bytes)):
             _content = cluster_resize_request
         else:
             _json = self._serialize.body(cluster_resize_request, "ClusterResizeData")
 
-        request = build_resize_request(
+        _request = build_resize_request(
             resource_group_name=resource_group_name,
             cluster_pool_name=cluster_pool_name,
             cluster_name=cluster_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             content_type=content_type,
             json=_json,
             content=_content,
-            template_url=self._resize_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -222,21 +425,17 @@
         if response.status_code == 200:
             deserialized = self._deserialize("Cluster", pipeline_response)
 
         if response.status_code == 202:
             response_headers["location"] = self._deserialize("str", response.headers.get("location"))
 
         if cls:
-            return cls(pipeline_response, deserialized, response_headers)
-
-        return deserialized
+            return cls(pipeline_response, deserialized, response_headers)  # type: ignore
 
-    _resize_initial.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HDInsight/clusterpools/{clusterPoolName}/clusters/{clusterName}/resize"
-    }
+        return deserialized  # type: ignore
 
     @overload
     async def begin_resize(
         self,
         resource_group_name: str,
         cluster_pool_name: str,
         cluster_name: str,
@@ -255,99 +454,73 @@
         :param cluster_name: The name of the HDInsight cluster. Required.
         :type cluster_name: str
         :param cluster_resize_request: Resize a cluster. Required.
         :type cluster_resize_request: ~azure.mgmt.hdinsightcontainers.models.ClusterResizeData
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
-         this operation to not poll, or pass in your own initialized polling object for a personal
-         polling strategy.
-        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
         :return: An instance of AsyncLROPoller that returns either Cluster or the result of
          cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.hdinsightcontainers.models.Cluster]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
     async def begin_resize(
         self,
         resource_group_name: str,
         cluster_pool_name: str,
         cluster_name: str,
-        cluster_resize_request: IO,
+        cluster_resize_request: IO[bytes],
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> AsyncLROPoller[_models.Cluster]:
         """Resize an existing Cluster.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param cluster_pool_name: The name of the cluster pool. Required.
         :type cluster_pool_name: str
         :param cluster_name: The name of the HDInsight cluster. Required.
         :type cluster_name: str
         :param cluster_resize_request: Resize a cluster. Required.
-        :type cluster_resize_request: IO
+        :type cluster_resize_request: IO[bytes]
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
-         this operation to not poll, or pass in your own initialized polling object for a personal
-         polling strategy.
-        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
         :return: An instance of AsyncLROPoller that returns either Cluster or the result of
          cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.hdinsightcontainers.models.Cluster]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace_async
     async def begin_resize(
         self,
         resource_group_name: str,
         cluster_pool_name: str,
         cluster_name: str,
-        cluster_resize_request: Union[_models.ClusterResizeData, IO],
+        cluster_resize_request: Union[_models.ClusterResizeData, IO[bytes]],
         **kwargs: Any
     ) -> AsyncLROPoller[_models.Cluster]:
         """Resize an existing Cluster.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param cluster_pool_name: The name of the cluster pool. Required.
         :type cluster_pool_name: str
         :param cluster_name: The name of the HDInsight cluster. Required.
         :type cluster_name: str
-        :param cluster_resize_request: Resize a cluster. Is either a ClusterResizeData type or a IO
-         type. Required.
-        :type cluster_resize_request: ~azure.mgmt.hdinsightcontainers.models.ClusterResizeData or IO
-        :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
-         Default value is None.
-        :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
-         this operation to not poll, or pass in your own initialized polling object for a personal
-         polling strategy.
-        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
+        :param cluster_resize_request: Resize a cluster. Is either a ClusterResizeData type or a
+         IO[bytes] type. Required.
+        :type cluster_resize_request: ~azure.mgmt.hdinsightcontainers.models.ClusterResizeData or
+         IO[bytes]
         :return: An instance of AsyncLROPoller that returns either Cluster or the result of
          cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.hdinsightcontainers.models.Cluster]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
@@ -372,52 +545,49 @@
                 **kwargs
             )
         kwargs.pop("error_map", None)
 
         def get_long_running_output(pipeline_response):
             deserialized = self._deserialize("Cluster", pipeline_response)
             if cls:
-                return cls(pipeline_response, deserialized, {})
+                return cls(pipeline_response, deserialized, {})  # type: ignore
             return deserialized
 
         if polling is True:
             polling_method: AsyncPollingMethod = cast(
                 AsyncPollingMethod, AsyncARMPolling(lro_delay, lro_options={"final-state-via": "location"}, **kwargs)
             )
         elif polling is False:
             polling_method = cast(AsyncPollingMethod, AsyncNoPolling())
         else:
             polling_method = polling
         if cont_token:
-            return AsyncLROPoller.from_continuation_token(
+            return AsyncLROPoller[_models.Cluster].from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
                 deserialization_callback=get_long_running_output,
             )
-        return AsyncLROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
-
-    begin_resize.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HDInsight/clusterpools/{clusterPoolName}/clusters/{clusterName}/resize"
-    }
+        return AsyncLROPoller[_models.Cluster](
+            self._client, raw_result, get_long_running_output, polling_method  # type: ignore
+        )
 
     @distributed_trace_async
     async def get(
         self, resource_group_name: str, cluster_pool_name: str, cluster_name: str, **kwargs: Any
     ) -> _models.Cluster:
         """Gets a HDInsight cluster.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param cluster_pool_name: The name of the cluster pool. Required.
         :type cluster_pool_name: str
         :param cluster_name: The name of the HDInsight cluster. Required.
         :type cluster_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: Cluster or the result of cls(response)
         :rtype: ~azure.mgmt.hdinsightcontainers.models.Cluster
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -428,56 +598,51 @@
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.Cluster] = kwargs.pop("cls", None)
 
-        request = build_get_request(
+        _request = build_get_request(
             resource_group_name=resource_group_name,
             cluster_pool_name=cluster_pool_name,
             cluster_name=cluster_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
-            template_url=self.get.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         deserialized = self._deserialize("Cluster", pipeline_response)
 
         if cls:
-            return cls(pipeline_response, deserialized, {})
-
-        return deserialized
+            return cls(pipeline_response, deserialized, {})  # type: ignore
 
-    get.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HDInsight/clusterpools/{clusterPoolName}/clusters/{clusterName}"
-    }
+        return deserialized  # type: ignore
 
     async def _create_initial(
         self,
         resource_group_name: str,
         cluster_pool_name: str,
         cluster_name: str,
-        hd_insight_cluster: Union[_models.Cluster, IO],
+        hd_insight_cluster: Union[_models.Cluster, IO[bytes]],
         **kwargs: Any
     ) -> _models.Cluster:
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -495,33 +660,32 @@
         _json = None
         _content = None
         if isinstance(hd_insight_cluster, (IOBase, bytes)):
             _content = hd_insight_cluster
         else:
             _json = self._serialize.body(hd_insight_cluster, "Cluster")
 
-        request = build_create_request(
+        _request = build_create_request(
             resource_group_name=resource_group_name,
             cluster_pool_name=cluster_pool_name,
             cluster_name=cluster_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             content_type=content_type,
             json=_json,
             content=_content,
-            template_url=self._create_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 201]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -534,18 +698,14 @@
             deserialized = self._deserialize("Cluster", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})  # type: ignore
 
         return deserialized  # type: ignore
 
-    _create_initial.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HDInsight/clusterpools/{clusterPoolName}/clusters/{clusterName}"
-    }
-
     @overload
     async def begin_create(
         self,
         resource_group_name: str,
         cluster_pool_name: str,
         cluster_name: str,
         hd_insight_cluster: _models.Cluster,
@@ -563,99 +723,72 @@
         :param cluster_name: The name of the HDInsight cluster. Required.
         :type cluster_name: str
         :param hd_insight_cluster: The cluster to create. Required.
         :type hd_insight_cluster: ~azure.mgmt.hdinsightcontainers.models.Cluster
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
-         this operation to not poll, or pass in your own initialized polling object for a personal
-         polling strategy.
-        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
         :return: An instance of AsyncLROPoller that returns either Cluster or the result of
          cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.hdinsightcontainers.models.Cluster]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
     async def begin_create(
         self,
         resource_group_name: str,
         cluster_pool_name: str,
         cluster_name: str,
-        hd_insight_cluster: IO,
+        hd_insight_cluster: IO[bytes],
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> AsyncLROPoller[_models.Cluster]:
         """Creates a cluster.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param cluster_pool_name: The name of the cluster pool. Required.
         :type cluster_pool_name: str
         :param cluster_name: The name of the HDInsight cluster. Required.
         :type cluster_name: str
         :param hd_insight_cluster: The cluster to create. Required.
-        :type hd_insight_cluster: IO
+        :type hd_insight_cluster: IO[bytes]
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
-         this operation to not poll, or pass in your own initialized polling object for a personal
-         polling strategy.
-        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
         :return: An instance of AsyncLROPoller that returns either Cluster or the result of
          cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.hdinsightcontainers.models.Cluster]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace_async
     async def begin_create(
         self,
         resource_group_name: str,
         cluster_pool_name: str,
         cluster_name: str,
-        hd_insight_cluster: Union[_models.Cluster, IO],
+        hd_insight_cluster: Union[_models.Cluster, IO[bytes]],
         **kwargs: Any
     ) -> AsyncLROPoller[_models.Cluster]:
         """Creates a cluster.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param cluster_pool_name: The name of the cluster pool. Required.
         :type cluster_pool_name: str
         :param cluster_name: The name of the HDInsight cluster. Required.
         :type cluster_name: str
-        :param hd_insight_cluster: The cluster to create. Is either a Cluster type or a IO type.
+        :param hd_insight_cluster: The cluster to create. Is either a Cluster type or a IO[bytes] type.
          Required.
-        :type hd_insight_cluster: ~azure.mgmt.hdinsightcontainers.models.Cluster or IO
-        :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
-         Default value is None.
-        :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
-         this operation to not poll, or pass in your own initialized polling object for a personal
-         polling strategy.
-        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
+        :type hd_insight_cluster: ~azure.mgmt.hdinsightcontainers.models.Cluster or IO[bytes]
         :return: An instance of AsyncLROPoller that returns either Cluster or the result of
          cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.hdinsightcontainers.models.Cluster]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
@@ -680,45 +813,43 @@
                 **kwargs
             )
         kwargs.pop("error_map", None)
 
         def get_long_running_output(pipeline_response):
             deserialized = self._deserialize("Cluster", pipeline_response)
             if cls:
-                return cls(pipeline_response, deserialized, {})
+                return cls(pipeline_response, deserialized, {})  # type: ignore
             return deserialized
 
         if polling is True:
             polling_method: AsyncPollingMethod = cast(
                 AsyncPollingMethod,
                 AsyncARMPolling(lro_delay, lro_options={"final-state-via": "azure-async-operation"}, **kwargs),
             )
         elif polling is False:
             polling_method = cast(AsyncPollingMethod, AsyncNoPolling())
         else:
             polling_method = polling
         if cont_token:
-            return AsyncLROPoller.from_continuation_token(
+            return AsyncLROPoller[_models.Cluster].from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
                 deserialization_callback=get_long_running_output,
             )
-        return AsyncLROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
-
-    begin_create.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HDInsight/clusterpools/{clusterPoolName}/clusters/{clusterName}"
-    }
+        return AsyncLROPoller[_models.Cluster](
+            self._client, raw_result, get_long_running_output, polling_method  # type: ignore
+        )
 
     async def _update_initial(
         self,
         resource_group_name: str,
         cluster_pool_name: str,
         cluster_name: str,
-        cluster_patch_request: Union[_models.ClusterPatch, IO],
+        cluster_patch_request: Union[_models.ClusterPatch, IO[bytes]],
         **kwargs: Any
     ) -> _models.Cluster:
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -736,33 +867,32 @@
         _json = None
         _content = None
         if isinstance(cluster_patch_request, (IOBase, bytes)):
             _content = cluster_patch_request
         else:
             _json = self._serialize.body(cluster_patch_request, "ClusterPatch")
 
-        request = build_update_request(
+        _request = build_update_request(
             resource_group_name=resource_group_name,
             cluster_pool_name=cluster_pool_name,
             cluster_name=cluster_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             content_type=content_type,
             json=_json,
             content=_content,
-            template_url=self._update_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -778,18 +908,14 @@
             deserialized = self._deserialize("Cluster", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, response_headers)  # type: ignore
 
         return deserialized  # type: ignore
 
-    _update_initial.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HDInsight/clusterpools/{clusterPoolName}/clusters/{clusterName}"
-    }
-
     @overload
     async def begin_update(
         self,
         resource_group_name: str,
         cluster_pool_name: str,
         cluster_name: str,
         cluster_patch_request: _models.ClusterPatch,
@@ -807,99 +933,72 @@
         :param cluster_name: The name of the HDInsight cluster. Required.
         :type cluster_name: str
         :param cluster_patch_request: Patch a cluster. Required.
         :type cluster_patch_request: ~azure.mgmt.hdinsightcontainers.models.ClusterPatch
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
-         this operation to not poll, or pass in your own initialized polling object for a personal
-         polling strategy.
-        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
         :return: An instance of AsyncLROPoller that returns either Cluster or the result of
          cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.hdinsightcontainers.models.Cluster]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
     async def begin_update(
         self,
         resource_group_name: str,
         cluster_pool_name: str,
         cluster_name: str,
-        cluster_patch_request: IO,
+        cluster_patch_request: IO[bytes],
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> AsyncLROPoller[_models.Cluster]:
         """Updates an existing Cluster.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param cluster_pool_name: The name of the cluster pool. Required.
         :type cluster_pool_name: str
         :param cluster_name: The name of the HDInsight cluster. Required.
         :type cluster_name: str
         :param cluster_patch_request: Patch a cluster. Required.
-        :type cluster_patch_request: IO
+        :type cluster_patch_request: IO[bytes]
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
-         this operation to not poll, or pass in your own initialized polling object for a personal
-         polling strategy.
-        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
         :return: An instance of AsyncLROPoller that returns either Cluster or the result of
          cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.hdinsightcontainers.models.Cluster]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace_async
     async def begin_update(
         self,
         resource_group_name: str,
         cluster_pool_name: str,
         cluster_name: str,
-        cluster_patch_request: Union[_models.ClusterPatch, IO],
+        cluster_patch_request: Union[_models.ClusterPatch, IO[bytes]],
         **kwargs: Any
     ) -> AsyncLROPoller[_models.Cluster]:
         """Updates an existing Cluster.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param cluster_pool_name: The name of the cluster pool. Required.
         :type cluster_pool_name: str
         :param cluster_name: The name of the HDInsight cluster. Required.
         :type cluster_name: str
-        :param cluster_patch_request: Patch a cluster. Is either a ClusterPatch type or a IO type.
-         Required.
-        :type cluster_patch_request: ~azure.mgmt.hdinsightcontainers.models.ClusterPatch or IO
-        :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
-         Default value is None.
-        :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
-         this operation to not poll, or pass in your own initialized polling object for a personal
-         polling strategy.
-        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
+        :param cluster_patch_request: Patch a cluster. Is either a ClusterPatch type or a IO[bytes]
+         type. Required.
+        :type cluster_patch_request: ~azure.mgmt.hdinsightcontainers.models.ClusterPatch or IO[bytes]
         :return: An instance of AsyncLROPoller that returns either Cluster or the result of
          cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.hdinsightcontainers.models.Cluster]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
@@ -924,38 +1023,36 @@
                 **kwargs
             )
         kwargs.pop("error_map", None)
 
         def get_long_running_output(pipeline_response):
             deserialized = self._deserialize("Cluster", pipeline_response)
             if cls:
-                return cls(pipeline_response, deserialized, {})
+                return cls(pipeline_response, deserialized, {})  # type: ignore
             return deserialized
 
         if polling is True:
             polling_method: AsyncPollingMethod = cast(
                 AsyncPollingMethod,
                 AsyncARMPolling(lro_delay, lro_options={"final-state-via": "azure-async-operation"}, **kwargs),
             )
         elif polling is False:
             polling_method = cast(AsyncPollingMethod, AsyncNoPolling())
         else:
             polling_method = polling
         if cont_token:
-            return AsyncLROPoller.from_continuation_token(
+            return AsyncLROPoller[_models.Cluster].from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
                 deserialization_callback=get_long_running_output,
             )
-        return AsyncLROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
-
-    begin_update.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HDInsight/clusterpools/{clusterPoolName}/clusters/{clusterName}"
-    }
+        return AsyncLROPoller[_models.Cluster](
+            self._client, raw_result, get_long_running_output, polling_method  # type: ignore
+        )
 
     async def _delete_initial(  # pylint: disable=inconsistent-return-statements
         self, resource_group_name: str, cluster_pool_name: str, cluster_name: str, **kwargs: Any
     ) -> None:
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -966,71 +1063,58 @@
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
-        request = build_delete_request(
+        _request = build_delete_request(
             resource_group_name=resource_group_name,
             cluster_pool_name=cluster_pool_name,
             cluster_name=cluster_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
-            template_url=self._delete_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         response_headers = {}
         if response.status_code == 202:
             response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
 
         if cls:
-            return cls(pipeline_response, None, response_headers)
-
-    _delete_initial.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HDInsight/clusterpools/{clusterPoolName}/clusters/{clusterName}"
-    }
+            return cls(pipeline_response, None, response_headers)  # type: ignore
 
     @distributed_trace_async
     async def begin_delete(
         self, resource_group_name: str, cluster_pool_name: str, cluster_name: str, **kwargs: Any
     ) -> AsyncLROPoller[None]:
         """Deletes a cluster.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param cluster_pool_name: The name of the cluster pool. Required.
         :type cluster_pool_name: str
         :param cluster_name: The name of the HDInsight cluster. Required.
         :type cluster_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
-         this operation to not poll, or pass in your own initialized polling object for a personal
-         polling strategy.
-        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
         :return: An instance of AsyncLROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
@@ -1050,52 +1134,47 @@
                 params=_params,
                 **kwargs
             )
         kwargs.pop("error_map", None)
 
         def get_long_running_output(pipeline_response):  # pylint: disable=inconsistent-return-statements
             if cls:
-                return cls(pipeline_response, None, {})
+                return cls(pipeline_response, None, {})  # type: ignore
 
         if polling is True:
             polling_method: AsyncPollingMethod = cast(
                 AsyncPollingMethod,
                 AsyncARMPolling(lro_delay, lro_options={"final-state-via": "azure-async-operation"}, **kwargs),
             )
         elif polling is False:
             polling_method = cast(AsyncPollingMethod, AsyncNoPolling())
         else:
             polling_method = polling
         if cont_token:
-            return AsyncLROPoller.from_continuation_token(
+            return AsyncLROPoller[None].from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
                 deserialization_callback=get_long_running_output,
             )
-        return AsyncLROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
-
-    begin_delete.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HDInsight/clusterpools/{clusterPoolName}/clusters/{clusterName}"
-    }
+        return AsyncLROPoller[None](self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
 
     @distributed_trace
     def list_service_configs(
         self, resource_group_name: str, cluster_pool_name: str, cluster_name: str, **kwargs: Any
     ) -> AsyncIterable["_models.ServiceConfigResult"]:
         """Lists the config dump of all services running in cluster.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param cluster_pool_name: The name of the cluster pool. Required.
         :type cluster_pool_name: str
         :param cluster_name: The name of the HDInsight cluster. Required.
         :type cluster_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either ServiceConfigResult or the result of cls(response)
         :rtype:
          ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.hdinsightcontainers.models.ServiceConfigResult]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
@@ -1110,88 +1189,82 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         def prepare_request(next_link=None):
             if not next_link:
 
-                request = build_list_service_configs_request(
+                _request = build_list_service_configs_request(
                     resource_group_name=resource_group_name,
                     cluster_pool_name=cluster_pool_name,
                     cluster_name=cluster_name,
                     subscription_id=self._config.subscription_id,
                     api_version=api_version,
-                    template_url=self.list_service_configs.metadata["url"],
                     headers=_headers,
                     params=_params,
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
 
             else:
                 # make call to next link with the client's api-version
                 _parsed_next_link = urllib.parse.urlparse(next_link)
                 _next_request_params = case_insensitive_dict(
                     {
                         key: [urllib.parse.quote(v) for v in value]
                         for key, value in urllib.parse.parse_qs(_parsed_next_link.query).items()
                     }
                 )
                 _next_request_params["api-version"] = self._config.api_version
-                request = HttpRequest(
+                _request = HttpRequest(
                     "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
-                request.method = "GET"
-            return request
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
+                _request.method = "GET"
+            return _request
 
         async def extract_data(pipeline_response):
             deserialized = self._deserialize("ServiceConfigListResult", pipeline_response)
             list_of_elem = deserialized.value
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, AsyncList(list_of_elem)
 
         async def get_next(next_link=None):
-            request = prepare_request(next_link)
+            _request = prepare_request(next_link)
 
             _stream = False
             pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=_stream, **kwargs
+                _request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
             return pipeline_response
 
         return AsyncItemPaged(get_next, extract_data)
 
-    list_service_configs.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HDInsight/clusterpools/{clusterPoolName}/clusters/{clusterName}/serviceConfigs"
-    }
-
     @distributed_trace
     def list_instance_views(
         self, resource_group_name: str, cluster_pool_name: str, cluster_name: str, **kwargs: Any
     ) -> AsyncIterable["_models.ClusterInstanceViewResult"]:
         """Lists the lists of instance views.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param cluster_pool_name: The name of the cluster pool. Required.
         :type cluster_pool_name: str
         :param cluster_name: The name of the HDInsight cluster. Required.
         :type cluster_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either ClusterInstanceViewResult or the result of
          cls(response)
         :rtype:
          ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.hdinsightcontainers.models.ClusterInstanceViewResult]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
@@ -1207,88 +1280,82 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         def prepare_request(next_link=None):
             if not next_link:
 
-                request = build_list_instance_views_request(
+                _request = build_list_instance_views_request(
                     resource_group_name=resource_group_name,
                     cluster_pool_name=cluster_pool_name,
                     cluster_name=cluster_name,
                     subscription_id=self._config.subscription_id,
                     api_version=api_version,
-                    template_url=self.list_instance_views.metadata["url"],
                     headers=_headers,
                     params=_params,
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
 
             else:
                 # make call to next link with the client's api-version
                 _parsed_next_link = urllib.parse.urlparse(next_link)
                 _next_request_params = case_insensitive_dict(
                     {
                         key: [urllib.parse.quote(v) for v in value]
                         for key, value in urllib.parse.parse_qs(_parsed_next_link.query).items()
                     }
                 )
                 _next_request_params["api-version"] = self._config.api_version
-                request = HttpRequest(
+                _request = HttpRequest(
                     "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
-                request.method = "GET"
-            return request
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
+                _request.method = "GET"
+            return _request
 
         async def extract_data(pipeline_response):
             deserialized = self._deserialize("ClusterInstanceViewsResult", pipeline_response)
             list_of_elem = deserialized.value
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, AsyncList(list_of_elem)
 
         async def get_next(next_link=None):
-            request = prepare_request(next_link)
+            _request = prepare_request(next_link)
 
             _stream = False
             pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=_stream, **kwargs
+                _request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
             return pipeline_response
 
         return AsyncItemPaged(get_next, extract_data)
 
-    list_instance_views.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HDInsight/clusterpools/{clusterPoolName}/clusters/{clusterName}/instanceViews"
-    }
-
     @distributed_trace_async
     async def get_instance_view(
         self, resource_group_name: str, cluster_pool_name: str, cluster_name: str, **kwargs: Any
     ) -> _models.ClusterInstanceViewResult:
         """Gets the status of a cluster instance.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param cluster_pool_name: The name of the cluster pool. Required.
         :type cluster_pool_name: str
         :param cluster_name: The name of the HDInsight cluster. Required.
         :type cluster_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: ClusterInstanceViewResult or the result of cls(response)
         :rtype: ~azure.mgmt.hdinsightcontainers.models.ClusterInstanceViewResult
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -1299,42 +1366,37 @@
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.ClusterInstanceViewResult] = kwargs.pop("cls", None)
 
-        request = build_get_instance_view_request(
+        _request = build_get_instance_view_request(
             resource_group_name=resource_group_name,
             cluster_pool_name=cluster_pool_name,
             cluster_name=cluster_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
-            template_url=self.get_instance_view.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         deserialized = self._deserialize("ClusterInstanceViewResult", pipeline_response)
 
         if cls:
-            return cls(pipeline_response, deserialized, {})
-
-        return deserialized
+            return cls(pipeline_response, deserialized, {})  # type: ignore
 
-    get_instance_view.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HDInsight/clusterpools/{clusterPoolName}/clusters/{clusterName}/instanceViews/default"
-    }
+        return deserialized  # type: ignore
```

### Comparing `azure-mgmt-hdinsightcontainers-1.0.0b1/azure/mgmt/hdinsightcontainers/aio/operations/_locations_operations.py` & `azure-mgmt-hdinsightcontainers-1.0.0b2/azure/mgmt/hdinsightcontainers/aio/operations/_locations_operations.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=too-many-lines
+# pylint: disable=too-many-lines,too-many-statements
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
@@ -66,55 +66,57 @@
         :type location: str
         :param name_availability_parameters: The name and type of the resource. Required.
         :type name_availability_parameters:
          ~azure.mgmt.hdinsightcontainers.models.NameAvailabilityParameters
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: NameAvailabilityResult or the result of cls(response)
         :rtype: ~azure.mgmt.hdinsightcontainers.models.NameAvailabilityResult
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
     async def check_name_availability(
-        self, location: str, name_availability_parameters: IO, *, content_type: str = "application/json", **kwargs: Any
+        self,
+        location: str,
+        name_availability_parameters: IO[bytes],
+        *,
+        content_type: str = "application/json",
+        **kwargs: Any
     ) -> _models.NameAvailabilityResult:
         """Check the availability of the resource name.
 
         :param location: The name of the Azure region. Required.
         :type location: str
         :param name_availability_parameters: The name and type of the resource. Required.
-        :type name_availability_parameters: IO
+        :type name_availability_parameters: IO[bytes]
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: NameAvailabilityResult or the result of cls(response)
         :rtype: ~azure.mgmt.hdinsightcontainers.models.NameAvailabilityResult
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace_async
     async def check_name_availability(
-        self, location: str, name_availability_parameters: Union[_models.NameAvailabilityParameters, IO], **kwargs: Any
+        self,
+        location: str,
+        name_availability_parameters: Union[_models.NameAvailabilityParameters, IO[bytes]],
+        **kwargs: Any
     ) -> _models.NameAvailabilityResult:
         """Check the availability of the resource name.
 
         :param location: The name of the Azure region. Required.
         :type location: str
         :param name_availability_parameters: The name and type of the resource. Is either a
-         NameAvailabilityParameters type or a IO type. Required.
+         NameAvailabilityParameters type or a IO[bytes] type. Required.
         :type name_availability_parameters:
-         ~azure.mgmt.hdinsightcontainers.models.NameAvailabilityParameters or IO
-        :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
-         Default value is None.
-        :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
+         ~azure.mgmt.hdinsightcontainers.models.NameAvailabilityParameters or IO[bytes]
         :return: NameAvailabilityResult or the result of cls(response)
         :rtype: ~azure.mgmt.hdinsightcontainers.models.NameAvailabilityResult
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -134,43 +136,38 @@
         _json = None
         _content = None
         if isinstance(name_availability_parameters, (IOBase, bytes)):
             _content = name_availability_parameters
         else:
             _json = self._serialize.body(name_availability_parameters, "NameAvailabilityParameters")
 
-        request = build_check_name_availability_request(
+        _request = build_check_name_availability_request(
             location=location,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             content_type=content_type,
             json=_json,
             content=_content,
-            template_url=self.check_name_availability.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         deserialized = self._deserialize("NameAvailabilityResult", pipeline_response)
 
         if cls:
-            return cls(pipeline_response, deserialized, {})
-
-        return deserialized
+            return cls(pipeline_response, deserialized, {})  # type: ignore
 
-    check_name_availability.metadata = {
-        "url": "/subscriptions/{subscriptionId}/providers/Microsoft.HDInsight/locations/{location}/checkNameAvailability"
-    }
+        return deserialized  # type: ignore
```

### Comparing `azure-mgmt-hdinsightcontainers-1.0.0b1/azure/mgmt/hdinsightcontainers/aio/operations/_operations.py` & `azure-mgmt-hdinsightcontainers-1.0.0b2/azure/mgmt/hdinsightcontainers/aio/operations/_operations.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=too-many-lines
+# pylint: disable=too-many-lines,too-many-statements
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
@@ -52,15 +52,14 @@
         self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
         self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
 
     @distributed_trace
     def list(self, **kwargs: Any) -> AsyncIterable["_models.Operation"]:
         """Returns list of operations.
 
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either Operation or the result of cls(response)
         :rtype:
          ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.hdinsightcontainers.models.Operation]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
@@ -75,60 +74,57 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         def prepare_request(next_link=None):
             if not next_link:
 
-                request = build_list_request(
+                _request = build_list_request(
                     api_version=api_version,
-                    template_url=self.list.metadata["url"],
                     headers=_headers,
                     params=_params,
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
 
             else:
                 # make call to next link with the client's api-version
                 _parsed_next_link = urllib.parse.urlparse(next_link)
                 _next_request_params = case_insensitive_dict(
                     {
                         key: [urllib.parse.quote(v) for v in value]
                         for key, value in urllib.parse.parse_qs(_parsed_next_link.query).items()
                     }
                 )
                 _next_request_params["api-version"] = self._config.api_version
-                request = HttpRequest(
+                _request = HttpRequest(
                     "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
-                request.method = "GET"
-            return request
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
+                _request.method = "GET"
+            return _request
 
         async def extract_data(pipeline_response):
             deserialized = self._deserialize("OperationListResult", pipeline_response)
             list_of_elem = deserialized.value
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, AsyncList(list_of_elem)
 
         async def get_next(next_link=None):
-            request = prepare_request(next_link)
+            _request = prepare_request(next_link)
 
             _stream = False
             pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=_stream, **kwargs
+                _request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
             return pipeline_response
 
         return AsyncItemPaged(get_next, extract_data)
-
-    list.metadata = {"url": "/providers/Microsoft.HDInsight/operations"}
```

### Comparing `azure-mgmt-hdinsightcontainers-1.0.0b1/azure/mgmt/hdinsightcontainers/aio/operations/_patch.py` & `azure-mgmt-hdinsightcontainers-1.0.0b2/azure/mgmt/hdinsightcontainers/aio/operations/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-hdinsightcontainers-1.0.0b1/azure/mgmt/hdinsightcontainers/models/__init__.py` & `azure-mgmt-hdinsightcontainers-1.0.0b2/azure/mgmt/hdinsightcontainers/models/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,72 +8,107 @@
 
 from ._models_py3 import AksClusterProfile
 from ._models_py3 import AksClusterProfileAksClusterAgentPoolIdentityProfile
 from ._models_py3 import AuthorizationProfile
 from ._models_py3 import AutoscaleProfile
 from ._models_py3 import CatalogOptions
 from ._models_py3 import Cluster
+from ._models_py3 import ClusterAKSPatchVersionUpgradeProperties
+from ._models_py3 import ClusterAccessProfile
+from ._models_py3 import ClusterAvailableUpgrade
+from ._models_py3 import ClusterAvailableUpgradeAksPatchUpgradeProperties
+from ._models_py3 import ClusterAvailableUpgradeHotfixUpgradeProperties
+from ._models_py3 import ClusterAvailableUpgradeList
+from ._models_py3 import ClusterAvailableUpgradeProperties
 from ._models_py3 import ClusterComponentsItem
 from ._models_py3 import ClusterConfigFile
+from ._models_py3 import ClusterHotfixUpgradeProperties
 from ._models_py3 import ClusterInstanceViewProperties
 from ._models_py3 import ClusterInstanceViewPropertiesStatus
 from ._models_py3 import ClusterInstanceViewResult
 from ._models_py3 import ClusterInstanceViewResultProperties
 from ._models_py3 import ClusterInstanceViewStatus
 from ._models_py3 import ClusterInstanceViewsResult
 from ._models_py3 import ClusterJob
 from ._models_py3 import ClusterJobList
 from ._models_py3 import ClusterJobProperties
 from ._models_py3 import ClusterListResult
 from ._models_py3 import ClusterLogAnalyticsApplicationLogs
 from ._models_py3 import ClusterLogAnalyticsProfile
 from ._models_py3 import ClusterPatch
+from ._models_py3 import ClusterPatchProperties
 from ._models_py3 import ClusterPool
+from ._models_py3 import ClusterPoolAKSPatchVersionUpgradeProperties
+from ._models_py3 import ClusterPoolAvailableUpgrade
+from ._models_py3 import ClusterPoolAvailableUpgradeAksPatchUpgradeProperties
+from ._models_py3 import ClusterPoolAvailableUpgradeList
+from ._models_py3 import ClusterPoolAvailableUpgradeNodeOsUpgradeProperties
+from ._models_py3 import ClusterPoolAvailableUpgradeProperties
 from ._models_py3 import ClusterPoolComputeProfile
 from ._models_py3 import ClusterPoolListResult
 from ._models_py3 import ClusterPoolLogAnalyticsProfile
 from ._models_py3 import ClusterPoolNetworkProfile
+from ._models_py3 import ClusterPoolNodeOsImageUpdateProperties
 from ._models_py3 import ClusterPoolProfile
+from ._models_py3 import ClusterPoolResourceProperties
 from ._models_py3 import ClusterPoolResourcePropertiesAksClusterProfile
 from ._models_py3 import ClusterPoolResourcePropertiesClusterPoolProfile
 from ._models_py3 import ClusterPoolResourcePropertiesComputeProfile
 from ._models_py3 import ClusterPoolResourcePropertiesLogAnalyticsProfile
 from ._models_py3 import ClusterPoolResourcePropertiesNetworkProfile
+from ._models_py3 import ClusterPoolUpgrade
+from ._models_py3 import ClusterPoolUpgradeProperties
 from ._models_py3 import ClusterPoolVersion
+from ._models_py3 import ClusterPoolVersionProperties
 from ._models_py3 import ClusterPoolVersionsListResult
 from ._models_py3 import ClusterProfile
 from ._models_py3 import ClusterPrometheusProfile
+from ._models_py3 import ClusterRangerPluginProfile
 from ._models_py3 import ClusterResizeData
+from ._models_py3 import ClusterResizeProperties
+from ._models_py3 import ClusterResourceProperties
 from ._models_py3 import ClusterServiceConfig
 from ._models_py3 import ClusterServiceConfigsProfile
+from ._models_py3 import ClusterUpgrade
+from ._models_py3 import ClusterUpgradeProperties
 from ._models_py3 import ClusterVersion
+from ._models_py3 import ClusterVersionProperties
 from ._models_py3 import ClusterVersionsListResult
 from ._models_py3 import ComparisonRule
 from ._models_py3 import ComputeProfile
 from ._models_py3 import ComputeResourceDefinition
 from ._models_py3 import ConnectivityProfile
 from ._models_py3 import ConnectivityProfileWeb
+from ._models_py3 import DiskStorageProfile
 from ._models_py3 import ErrorAdditionalInfo
 from ._models_py3 import ErrorDetail
 from ._models_py3 import ErrorResponse
 from ._models_py3 import FlinkCatalogOptions
 from ._models_py3 import FlinkHiveCatalogOption
+from ._models_py3 import FlinkJobProfile
 from ._models_py3 import FlinkJobProperties
 from ._models_py3 import FlinkProfile
 from ._models_py3 import FlinkStorageProfile
 from ._models_py3 import HiveCatalogOption
 from ._models_py3 import IdentityProfile
+from ._models_py3 import KafkaConnectivityEndpoints
+from ._models_py3 import KafkaProfile
 from ._models_py3 import LoadBasedConfig
 from ._models_py3 import NameAvailabilityParameters
 from ._models_py3 import NameAvailabilityResult
 from ._models_py3 import NodeProfile
 from ._models_py3 import Operation
 from ._models_py3 import OperationDisplay
 from ._models_py3 import OperationListResult
 from ._models_py3 import ProxyResource
+from ._models_py3 import RangerAdminSpec
+from ._models_py3 import RangerAdminSpecDatabase
+from ._models_py3 import RangerAuditSpec
+from ._models_py3 import RangerProfile
+from ._models_py3 import RangerUsersyncSpec
 from ._models_py3 import Resource
 from ._models_py3 import ScalingRule
 from ._models_py3 import Schedule
 from ._models_py3 import ScheduleBasedConfig
 from ._models_py3 import ScriptActionProfile
 from ._models_py3 import SecretReference
 from ._models_py3 import SecretsProfile
@@ -89,104 +124,154 @@
 from ._models_py3 import SparkUserPlugins
 from ._models_py3 import SshConnectivityEndpoint
 from ._models_py3 import SshProfile
 from ._models_py3 import SystemData
 from ._models_py3 import TagsObject
 from ._models_py3 import TrackedResource
 from ._models_py3 import TrinoCoordinator
+from ._models_py3 import TrinoDebugConfig
 from ._models_py3 import TrinoProfile
 from ._models_py3 import TrinoTelemetryConfig
 from ._models_py3 import TrinoUserPlugin
 from ._models_py3 import TrinoUserPlugins
 from ._models_py3 import TrinoUserTelemetry
 from ._models_py3 import TrinoWorker
 from ._models_py3 import UpdatableClusterProfile
 from ._models_py3 import WebConnectivityEndpoint
 
 from ._hd_insight_containers_mgmt_client_enums import Action
 from ._hd_insight_containers_mgmt_client_enums import ActionType
 from ._hd_insight_containers_mgmt_client_enums import AutoscaleType
+from ._hd_insight_containers_mgmt_client_enums import ClusterAvailableUpgradeType
+from ._hd_insight_containers_mgmt_client_enums import ClusterPoolAvailableUpgradeType
+from ._hd_insight_containers_mgmt_client_enums import ClusterPoolUpgradeType
+from ._hd_insight_containers_mgmt_client_enums import ClusterUpgradeType
 from ._hd_insight_containers_mgmt_client_enums import ComparisonOperator
 from ._hd_insight_containers_mgmt_client_enums import ContentEncoding
 from ._hd_insight_containers_mgmt_client_enums import CreatedByType
+from ._hd_insight_containers_mgmt_client_enums import CurrentClusterAksVersionStatus
+from ._hd_insight_containers_mgmt_client_enums import CurrentClusterPoolAksVersionStatus
+from ._hd_insight_containers_mgmt_client_enums import DataDiskType
+from ._hd_insight_containers_mgmt_client_enums import DbConnectionAuthenticationMode
+from ._hd_insight_containers_mgmt_client_enums import DeploymentMode
 from ._hd_insight_containers_mgmt_client_enums import JobType
 from ._hd_insight_containers_mgmt_client_enums import KeyVaultObjectType
+from ._hd_insight_containers_mgmt_client_enums import MetastoreDbConnectionAuthenticationMode
 from ._hd_insight_containers_mgmt_client_enums import Origin
+from ._hd_insight_containers_mgmt_client_enums import OutboundType
 from ._hd_insight_containers_mgmt_client_enums import ProvisioningStatus
+from ._hd_insight_containers_mgmt_client_enums import RangerUsersyncMode
 from ._hd_insight_containers_mgmt_client_enums import ScaleActionType
 from ._hd_insight_containers_mgmt_client_enums import ScheduleDay
+from ._hd_insight_containers_mgmt_client_enums import Severity
+from ._hd_insight_containers_mgmt_client_enums import UpgradeMode
 from ._patch import __all__ as _patch_all
 from ._patch import *  # pylint: disable=unused-wildcard-import
 from ._patch import patch_sdk as _patch_sdk
 
 __all__ = [
     "AksClusterProfile",
     "AksClusterProfileAksClusterAgentPoolIdentityProfile",
     "AuthorizationProfile",
     "AutoscaleProfile",
     "CatalogOptions",
     "Cluster",
+    "ClusterAKSPatchVersionUpgradeProperties",
+    "ClusterAccessProfile",
+    "ClusterAvailableUpgrade",
+    "ClusterAvailableUpgradeAksPatchUpgradeProperties",
+    "ClusterAvailableUpgradeHotfixUpgradeProperties",
+    "ClusterAvailableUpgradeList",
+    "ClusterAvailableUpgradeProperties",
     "ClusterComponentsItem",
     "ClusterConfigFile",
+    "ClusterHotfixUpgradeProperties",
     "ClusterInstanceViewProperties",
     "ClusterInstanceViewPropertiesStatus",
     "ClusterInstanceViewResult",
     "ClusterInstanceViewResultProperties",
     "ClusterInstanceViewStatus",
     "ClusterInstanceViewsResult",
     "ClusterJob",
     "ClusterJobList",
     "ClusterJobProperties",
     "ClusterListResult",
     "ClusterLogAnalyticsApplicationLogs",
     "ClusterLogAnalyticsProfile",
     "ClusterPatch",
+    "ClusterPatchProperties",
     "ClusterPool",
+    "ClusterPoolAKSPatchVersionUpgradeProperties",
+    "ClusterPoolAvailableUpgrade",
+    "ClusterPoolAvailableUpgradeAksPatchUpgradeProperties",
+    "ClusterPoolAvailableUpgradeList",
+    "ClusterPoolAvailableUpgradeNodeOsUpgradeProperties",
+    "ClusterPoolAvailableUpgradeProperties",
     "ClusterPoolComputeProfile",
     "ClusterPoolListResult",
     "ClusterPoolLogAnalyticsProfile",
     "ClusterPoolNetworkProfile",
+    "ClusterPoolNodeOsImageUpdateProperties",
     "ClusterPoolProfile",
+    "ClusterPoolResourceProperties",
     "ClusterPoolResourcePropertiesAksClusterProfile",
     "ClusterPoolResourcePropertiesClusterPoolProfile",
     "ClusterPoolResourcePropertiesComputeProfile",
     "ClusterPoolResourcePropertiesLogAnalyticsProfile",
     "ClusterPoolResourcePropertiesNetworkProfile",
+    "ClusterPoolUpgrade",
+    "ClusterPoolUpgradeProperties",
     "ClusterPoolVersion",
+    "ClusterPoolVersionProperties",
     "ClusterPoolVersionsListResult",
     "ClusterProfile",
     "ClusterPrometheusProfile",
+    "ClusterRangerPluginProfile",
     "ClusterResizeData",
+    "ClusterResizeProperties",
+    "ClusterResourceProperties",
     "ClusterServiceConfig",
     "ClusterServiceConfigsProfile",
+    "ClusterUpgrade",
+    "ClusterUpgradeProperties",
     "ClusterVersion",
+    "ClusterVersionProperties",
     "ClusterVersionsListResult",
     "ComparisonRule",
     "ComputeProfile",
     "ComputeResourceDefinition",
     "ConnectivityProfile",
     "ConnectivityProfileWeb",
+    "DiskStorageProfile",
     "ErrorAdditionalInfo",
     "ErrorDetail",
     "ErrorResponse",
     "FlinkCatalogOptions",
     "FlinkHiveCatalogOption",
+    "FlinkJobProfile",
     "FlinkJobProperties",
     "FlinkProfile",
     "FlinkStorageProfile",
     "HiveCatalogOption",
     "IdentityProfile",
+    "KafkaConnectivityEndpoints",
+    "KafkaProfile",
     "LoadBasedConfig",
     "NameAvailabilityParameters",
     "NameAvailabilityResult",
     "NodeProfile",
     "Operation",
     "OperationDisplay",
     "OperationListResult",
     "ProxyResource",
+    "RangerAdminSpec",
+    "RangerAdminSpecDatabase",
+    "RangerAuditSpec",
+    "RangerProfile",
+    "RangerUsersyncSpec",
     "Resource",
     "ScalingRule",
     "Schedule",
     "ScheduleBasedConfig",
     "ScriptActionProfile",
     "SecretReference",
     "SecretsProfile",
@@ -202,30 +287,45 @@
     "SparkUserPlugins",
     "SshConnectivityEndpoint",
     "SshProfile",
     "SystemData",
     "TagsObject",
     "TrackedResource",
     "TrinoCoordinator",
+    "TrinoDebugConfig",
     "TrinoProfile",
     "TrinoTelemetryConfig",
     "TrinoUserPlugin",
     "TrinoUserPlugins",
     "TrinoUserTelemetry",
     "TrinoWorker",
     "UpdatableClusterProfile",
     "WebConnectivityEndpoint",
     "Action",
     "ActionType",
     "AutoscaleType",
+    "ClusterAvailableUpgradeType",
+    "ClusterPoolAvailableUpgradeType",
+    "ClusterPoolUpgradeType",
+    "ClusterUpgradeType",
     "ComparisonOperator",
     "ContentEncoding",
     "CreatedByType",
+    "CurrentClusterAksVersionStatus",
+    "CurrentClusterPoolAksVersionStatus",
+    "DataDiskType",
+    "DbConnectionAuthenticationMode",
+    "DeploymentMode",
     "JobType",
     "KeyVaultObjectType",
+    "MetastoreDbConnectionAuthenticationMode",
     "Origin",
+    "OutboundType",
     "ProvisioningStatus",
+    "RangerUsersyncMode",
     "ScaleActionType",
     "ScheduleDay",
+    "Severity",
+    "UpgradeMode",
 ]
 __all__.extend([p for p in _patch_all if p not in __all__])
 _patch_sdk()
```

### Comparing `azure-mgmt-hdinsightcontainers-1.0.0b1/azure/mgmt/hdinsightcontainers/models/_models_py3.py` & `azure-mgmt-hdinsightcontainers-1.0.0b2/azure/mgmt/hdinsightcontainers/models/_models_py3.py`

 * *Files 13% similar despite different names*

```diff
@@ -67,15 +67,15 @@
         self.aks_cluster_agent_pool_identity_profile = aks_cluster_agent_pool_identity_profile
         self.aks_version = None
 
 
 class IdentityProfile(_serialization.Model):
     """Identity Profile with details of an MSI.
 
-    All required parameters must be populated in order to send to Azure.
+    All required parameters must be populated in order to send to server.
 
     :ivar msi_resource_id: ResourceId of the MSI. Required.
     :vartype msi_resource_id: str
     :ivar msi_client_id: ClientId of the MSI. Required.
     :vartype msi_client_id: str
     :ivar msi_object_id: ObjectId of the MSI. Required.
     :vartype msi_object_id: str
@@ -110,58 +110,27 @@
         """
         super().__init__(**kwargs)
         self.msi_resource_id = msi_resource_id
         self.msi_client_id = msi_client_id
         self.msi_object_id = msi_object_id
 
 
-class AksClusterProfileAksClusterAgentPoolIdentityProfile(IdentityProfile):
+class AksClusterProfileAksClusterAgentPoolIdentityProfile(IdentityProfile):  # pylint: disable=name-too-long
     """Identity properties of the AKS cluster agentpool MSI.
 
-    All required parameters must be populated in order to send to Azure.
+    All required parameters must be populated in order to send to server.
 
     :ivar msi_resource_id: ResourceId of the MSI. Required.
     :vartype msi_resource_id: str
     :ivar msi_client_id: ClientId of the MSI. Required.
     :vartype msi_client_id: str
     :ivar msi_object_id: ObjectId of the MSI. Required.
     :vartype msi_object_id: str
     """
 
-    _validation = {
-        "msi_resource_id": {"required": True},
-        "msi_client_id": {
-            "required": True,
-            "pattern": r"^[{(]?[0-9A-Fa-f]{8}[-]?(?:[0-9A-Fa-f]{4}[-]?){3}[0-9A-Fa-f]{12}[)}]?$",
-        },
-        "msi_object_id": {
-            "required": True,
-            "pattern": r"^[{(]?[0-9A-Fa-f]{8}[-]?(?:[0-9A-Fa-f]{4}[-]?){3}[0-9A-Fa-f]{12}[)}]?$",
-        },
-    }
-
-    _attribute_map = {
-        "msi_resource_id": {"key": "msiResourceId", "type": "str"},
-        "msi_client_id": {"key": "msiClientId", "type": "str"},
-        "msi_object_id": {"key": "msiObjectId", "type": "str"},
-    }
-
-    def __init__(self, *, msi_resource_id: str, msi_client_id: str, msi_object_id: str, **kwargs: Any) -> None:
-        """
-        :keyword msi_resource_id: ResourceId of the MSI. Required.
-        :paramtype msi_resource_id: str
-        :keyword msi_client_id: ClientId of the MSI. Required.
-        :paramtype msi_client_id: str
-        :keyword msi_object_id: ObjectId of the MSI. Required.
-        :paramtype msi_object_id: str
-        """
-        super().__init__(
-            msi_resource_id=msi_resource_id, msi_client_id=msi_client_id, msi_object_id=msi_object_id, **kwargs
-        )
-
 
 class AuthorizationProfile(_serialization.Model):
     """Authorization profile with details of AAD user Ids and group Ids authorized for data plane
     access.
 
     :ivar user_ids: AAD user Ids authorized for data plane access.
     :vartype user_ids: list[str]
@@ -188,15 +157,15 @@
         self.group_ids = group_ids
 
 
 class AutoscaleProfile(_serialization.Model):
     """This is the Autoscale profile for the cluster. This will allow customer to create cluster
     enabled with Autoscale.
 
-    All required parameters must be populated in order to send to Azure.
+    All required parameters must be populated in order to send to server.
 
     :ivar enabled: This indicates whether auto scale is enabled on HDInsight on AKS cluster.
      Required.
     :vartype enabled: bool
     :ivar graceful_decommission_timeout: This property is for graceful decommission timeout; It has
      a default setting of 3600 seconds before forced shutdown takes place. This is the maximal time
      to wait for running containers and applications to complete before transition a DECOMMISSIONING
@@ -282,15 +251,15 @@
 
 class Resource(_serialization.Model):
     """Common fields that are returned in the response for all Azure Resource Manager resources.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
     :ivar id: Fully qualified resource ID for the resource. E.g.
-     "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{resourceType}/{resourceName}".
+     "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{resourceType}/{resourceName}".  # pylint: disable=line-too-long
     :vartype id: str
     :ivar name: The name of the resource.
     :vartype name: str
     :ivar type: The type of the resource. E.g. "Microsoft.Compute/virtualMachines" or
      "Microsoft.Storage/storageAccounts".
     :vartype type: str
     :ivar system_data: Azure Resource Manager metadata containing createdBy and modifiedBy
@@ -323,18 +292,18 @@
 
 class TrackedResource(Resource):
     """The resource model definition for an Azure Resource Manager tracked top level resource which
     has 'tags' and a 'location'.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
-    All required parameters must be populated in order to send to Azure.
+    All required parameters must be populated in order to send to server.
 
     :ivar id: Fully qualified resource ID for the resource. E.g.
-     "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{resourceType}/{resourceName}".
+     "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{resourceType}/{resourceName}".  # pylint: disable=line-too-long
     :vartype id: str
     :ivar name: The name of the resource.
     :vartype name: str
     :ivar type: The type of the resource. E.g. "Microsoft.Compute/virtualMachines" or
      "Microsoft.Storage/storageAccounts".
     :vartype type: str
     :ivar system_data: Azure Resource Manager metadata containing createdBy and modifiedBy
@@ -371,107 +340,476 @@
         :paramtype location: str
         """
         super().__init__(**kwargs)
         self.tags = tags
         self.location = location
 
 
-class Cluster(TrackedResource):  # pylint: disable=too-many-instance-attributes
+class Cluster(TrackedResource):
     """The cluster.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
-    All required parameters must be populated in order to send to Azure.
+    All required parameters must be populated in order to send to server.
 
     :ivar id: Fully qualified resource ID for the resource. E.g.
-     "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{resourceType}/{resourceName}".
+     "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{resourceType}/{resourceName}".  # pylint: disable=line-too-long
     :vartype id: str
     :ivar name: The name of the resource.
     :vartype name: str
     :ivar type: The type of the resource. E.g. "Microsoft.Compute/virtualMachines" or
      "Microsoft.Storage/storageAccounts".
     :vartype type: str
     :ivar system_data: Azure Resource Manager metadata containing createdBy and modifiedBy
      information.
     :vartype system_data: ~azure.mgmt.hdinsightcontainers.models.SystemData
     :ivar tags: Resource tags.
     :vartype tags: dict[str, str]
     :ivar location: The geo-location where the resource lives. Required.
     :vartype location: str
-    :ivar provisioning_state: Provisioning state of the resource. Known values are: "Accepted",
-     "Succeeded", "Canceled", and "Failed".
-    :vartype provisioning_state: str or ~azure.mgmt.hdinsightcontainers.models.ProvisioningStatus
-    :ivar cluster_type: The type of cluster.
-    :vartype cluster_type: str
-    :ivar deployment_id: A unique id generated by the RP to identify the resource.
-    :vartype deployment_id: str
-    :ivar compute_profile: The compute profile.
-    :vartype compute_profile: ~azure.mgmt.hdinsightcontainers.models.ComputeProfile
-    :ivar cluster_profile: Cluster profile.
-    :vartype cluster_profile: ~azure.mgmt.hdinsightcontainers.models.ClusterProfile
-    :ivar status: Business status of the resource.
-    :vartype status: str
+    :ivar properties: Gets or sets the properties. Define cluster specific properties.
+    :vartype properties: ~azure.mgmt.hdinsightcontainers.models.ClusterResourceProperties
     """
 
     _validation = {
         "id": {"readonly": True},
         "name": {"readonly": True},
         "type": {"readonly": True},
         "system_data": {"readonly": True},
         "location": {"required": True},
-        "provisioning_state": {"readonly": True},
-        "cluster_type": {"pattern": r"^[a-zA-Z][a-zA-Z0-9]{0,31}$"},
-        "deployment_id": {"readonly": True},
-        "status": {"readonly": True},
     }
 
     _attribute_map = {
         "id": {"key": "id", "type": "str"},
         "name": {"key": "name", "type": "str"},
         "type": {"key": "type", "type": "str"},
         "system_data": {"key": "systemData", "type": "SystemData"},
         "tags": {"key": "tags", "type": "{str}"},
         "location": {"key": "location", "type": "str"},
-        "provisioning_state": {"key": "properties.provisioningState", "type": "str"},
-        "cluster_type": {"key": "properties.clusterType", "type": "str"},
-        "deployment_id": {"key": "properties.deploymentId", "type": "str"},
-        "compute_profile": {"key": "properties.computeProfile", "type": "ComputeProfile"},
-        "cluster_profile": {"key": "properties.clusterProfile", "type": "ClusterProfile"},
-        "status": {"key": "properties.status", "type": "str"},
+        "properties": {"key": "properties", "type": "ClusterResourceProperties"},
     }
 
     def __init__(
         self,
         *,
         location: str,
         tags: Optional[Dict[str, str]] = None,
-        cluster_type: Optional[str] = None,
-        compute_profile: Optional["_models.ComputeProfile"] = None,
-        cluster_profile: Optional["_models.ClusterProfile"] = None,
+        properties: Optional["_models.ClusterResourceProperties"] = None,
         **kwargs: Any
     ) -> None:
         """
         :keyword tags: Resource tags.
         :paramtype tags: dict[str, str]
         :keyword location: The geo-location where the resource lives. Required.
         :paramtype location: str
-        :keyword cluster_type: The type of cluster.
-        :paramtype cluster_type: str
-        :keyword compute_profile: The compute profile.
-        :paramtype compute_profile: ~azure.mgmt.hdinsightcontainers.models.ComputeProfile
-        :keyword cluster_profile: Cluster profile.
-        :paramtype cluster_profile: ~azure.mgmt.hdinsightcontainers.models.ClusterProfile
+        :keyword properties: Gets or sets the properties. Define cluster specific properties.
+        :paramtype properties: ~azure.mgmt.hdinsightcontainers.models.ClusterResourceProperties
         """
         super().__init__(tags=tags, location=location, **kwargs)
-        self.provisioning_state = None
-        self.cluster_type = cluster_type
-        self.deployment_id = None
-        self.compute_profile = compute_profile
-        self.cluster_profile = cluster_profile
-        self.status = None
+        self.properties = properties
+
+
+class ClusterAccessProfile(_serialization.Model):
+    """Cluster access profile.
+
+    Variables are only populated by the server, and will be ignored when sending a request.
+
+    All required parameters must be populated in order to send to server.
+
+    :ivar enable_internal_ingress: Whether to create cluster using private IP instead of public IP.
+     This property must be set at create time. Required.
+    :vartype enable_internal_ingress: bool
+    :ivar private_link_service_id: Private link service resource ID. Only when
+     enableInternalIngress is true, this property will be returned.
+    :vartype private_link_service_id: str
+    """
+
+    _validation = {
+        "enable_internal_ingress": {"required": True},
+        "private_link_service_id": {"readonly": True},
+    }
+
+    _attribute_map = {
+        "enable_internal_ingress": {"key": "enableInternalIngress", "type": "bool"},
+        "private_link_service_id": {"key": "privateLinkServiceId", "type": "str"},
+    }
+
+    def __init__(self, *, enable_internal_ingress: bool, **kwargs: Any) -> None:
+        """
+        :keyword enable_internal_ingress: Whether to create cluster using private IP instead of public
+         IP. This property must be set at create time. Required.
+        :paramtype enable_internal_ingress: bool
+        """
+        super().__init__(**kwargs)
+        self.enable_internal_ingress = enable_internal_ingress
+        self.private_link_service_id = None
+
+
+class ClusterUpgradeProperties(_serialization.Model):
+    """Properties of upgrading cluster.
+
+    You probably want to use the sub-classes and not this class directly. Known sub-classes are:
+    ClusterAKSPatchVersionUpgradeProperties, ClusterHotfixUpgradeProperties
+
+    All required parameters must be populated in order to send to server.
+
+    :ivar upgrade_type: Type of upgrade. Required. Known values are: "AKSPatchUpgrade" and
+     "HotfixUpgrade".
+    :vartype upgrade_type: str or ~azure.mgmt.hdinsightcontainers.models.ClusterUpgradeType
+    """
+
+    _validation = {
+        "upgrade_type": {"required": True},
+    }
+
+    _attribute_map = {
+        "upgrade_type": {"key": "upgradeType", "type": "str"},
+    }
+
+    _subtype_map = {
+        "upgrade_type": {
+            "AKSPatchUpgrade": "ClusterAKSPatchVersionUpgradeProperties",
+            "HotfixUpgrade": "ClusterHotfixUpgradeProperties",
+        }
+    }
+
+    def __init__(self, **kwargs: Any) -> None:
+        """ """
+        super().__init__(**kwargs)
+        self.upgrade_type: Optional[str] = None
+
+
+class ClusterAKSPatchVersionUpgradeProperties(ClusterUpgradeProperties):
+    """Properties of upgrading cluster's AKS patch version.
+
+    All required parameters must be populated in order to send to server.
+
+    :ivar upgrade_type: Type of upgrade. Required. Known values are: "AKSPatchUpgrade" and
+     "HotfixUpgrade".
+    :vartype upgrade_type: str or ~azure.mgmt.hdinsightcontainers.models.ClusterUpgradeType
+    """
+
+    _validation = {
+        "upgrade_type": {"required": True},
+    }
+
+    _attribute_map = {
+        "upgrade_type": {"key": "upgradeType", "type": "str"},
+    }
+
+    def __init__(self, **kwargs: Any) -> None:
+        """ """
+        super().__init__(**kwargs)
+        self.upgrade_type: str = "AKSPatchUpgrade"
+
+
+class ProxyResource(Resource):
+    """The resource model definition for a Azure Resource Manager proxy resource. It will not have
+    tags and a location.
+
+    Variables are only populated by the server, and will be ignored when sending a request.
+
+    :ivar id: Fully qualified resource ID for the resource. E.g.
+     "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{resourceType}/{resourceName}".  # pylint: disable=line-too-long
+    :vartype id: str
+    :ivar name: The name of the resource.
+    :vartype name: str
+    :ivar type: The type of the resource. E.g. "Microsoft.Compute/virtualMachines" or
+     "Microsoft.Storage/storageAccounts".
+    :vartype type: str
+    :ivar system_data: Azure Resource Manager metadata containing createdBy and modifiedBy
+     information.
+    :vartype system_data: ~azure.mgmt.hdinsightcontainers.models.SystemData
+    """
+
+
+class ClusterAvailableUpgrade(ProxyResource):
+    """Cluster available upgrade.
+
+    Variables are only populated by the server, and will be ignored when sending a request.
+
+    :ivar id: Fully qualified resource ID for the resource. E.g.
+     "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{resourceType}/{resourceName}".  # pylint: disable=line-too-long
+    :vartype id: str
+    :ivar name: The name of the resource.
+    :vartype name: str
+    :ivar type: The type of the resource. E.g. "Microsoft.Compute/virtualMachines" or
+     "Microsoft.Storage/storageAccounts".
+    :vartype type: str
+    :ivar system_data: Azure Resource Manager metadata containing createdBy and modifiedBy
+     information.
+    :vartype system_data: ~azure.mgmt.hdinsightcontainers.models.SystemData
+    :ivar properties: Gets or sets the properties. Define cluster upgrade specific properties.
+    :vartype properties: ~azure.mgmt.hdinsightcontainers.models.ClusterAvailableUpgradeProperties
+    """
+
+    _validation = {
+        "id": {"readonly": True},
+        "name": {"readonly": True},
+        "type": {"readonly": True},
+        "system_data": {"readonly": True},
+    }
+
+    _attribute_map = {
+        "id": {"key": "id", "type": "str"},
+        "name": {"key": "name", "type": "str"},
+        "type": {"key": "type", "type": "str"},
+        "system_data": {"key": "systemData", "type": "SystemData"},
+        "properties": {"key": "properties", "type": "ClusterAvailableUpgradeProperties"},
+    }
+
+    def __init__(
+        self, *, properties: Optional["_models.ClusterAvailableUpgradeProperties"] = None, **kwargs: Any
+    ) -> None:
+        """
+        :keyword properties: Gets or sets the properties. Define cluster upgrade specific properties.
+        :paramtype properties: ~azure.mgmt.hdinsightcontainers.models.ClusterAvailableUpgradeProperties
+        """
+        super().__init__(**kwargs)
+        self.properties = properties
+
+
+class ClusterAvailableUpgradeProperties(_serialization.Model):
+    """Cluster available upgrade properties.
+
+    You probably want to use the sub-classes and not this class directly. Known sub-classes are:
+    ClusterAvailableUpgradeAksPatchUpgradeProperties,
+    ClusterAvailableUpgradeHotfixUpgradeProperties
+
+    All required parameters must be populated in order to send to server.
+
+    :ivar upgrade_type: Type of upgrade. Required. Known values are: "AKSPatchUpgrade" and
+     "HotfixUpgrade".
+    :vartype upgrade_type: str or
+     ~azure.mgmt.hdinsightcontainers.models.ClusterAvailableUpgradeType
+    """
+
+    _validation = {
+        "upgrade_type": {"required": True},
+    }
+
+    _attribute_map = {
+        "upgrade_type": {"key": "upgradeType", "type": "str"},
+    }
+
+    _subtype_map = {
+        "upgrade_type": {
+            "AKSPatchUpgrade": "ClusterAvailableUpgradeAksPatchUpgradeProperties",
+            "HotfixUpgrade": "ClusterAvailableUpgradeHotfixUpgradeProperties",
+        }
+    }
+
+    def __init__(self, **kwargs: Any) -> None:
+        """ """
+        super().__init__(**kwargs)
+        self.upgrade_type: Optional[str] = None
+
+
+class ClusterAvailableUpgradeAksPatchUpgradeProperties(
+    ClusterAvailableUpgradeProperties
+):  # pylint: disable=name-too-long
+    """Cluster available AKS patch version upgrade.
+
+    All required parameters must be populated in order to send to server.
+
+    :ivar upgrade_type: Type of upgrade. Required. Known values are: "AKSPatchUpgrade" and
+     "HotfixUpgrade".
+    :vartype upgrade_type: str or
+     ~azure.mgmt.hdinsightcontainers.models.ClusterAvailableUpgradeType
+    :ivar current_version: Current node pool version.
+    :vartype current_version: str
+    :ivar current_version_status: Current AKS version's status: whether it is deprecated or
+     supported. Known values are: "Deprecated" and "Supported".
+    :vartype current_version_status: str or
+     ~azure.mgmt.hdinsightcontainers.models.CurrentClusterAksVersionStatus
+    :ivar latest_version: Latest available version, which should be equal to AKS control plane
+     version if it's not deprecated.
+    :vartype latest_version: str
+    """
+
+    _validation = {
+        "upgrade_type": {"required": True},
+    }
+
+    _attribute_map = {
+        "upgrade_type": {"key": "upgradeType", "type": "str"},
+        "current_version": {"key": "currentVersion", "type": "str"},
+        "current_version_status": {"key": "currentVersionStatus", "type": "str"},
+        "latest_version": {"key": "latestVersion", "type": "str"},
+    }
+
+    def __init__(
+        self,
+        *,
+        current_version: Optional[str] = None,
+        current_version_status: Optional[Union[str, "_models.CurrentClusterAksVersionStatus"]] = None,
+        latest_version: Optional[str] = None,
+        **kwargs: Any
+    ) -> None:
+        """
+        :keyword current_version: Current node pool version.
+        :paramtype current_version: str
+        :keyword current_version_status: Current AKS version's status: whether it is deprecated or
+         supported. Known values are: "Deprecated" and "Supported".
+        :paramtype current_version_status: str or
+         ~azure.mgmt.hdinsightcontainers.models.CurrentClusterAksVersionStatus
+        :keyword latest_version: Latest available version, which should be equal to AKS control plane
+         version if it's not deprecated.
+        :paramtype latest_version: str
+        """
+        super().__init__(**kwargs)
+        self.upgrade_type: str = "AKSPatchUpgrade"
+        self.current_version = current_version
+        self.current_version_status = current_version_status
+        self.latest_version = latest_version
+
+
+class ClusterAvailableUpgradeHotfixUpgradeProperties(
+    ClusterAvailableUpgradeProperties
+):  # pylint: disable=too-many-instance-attributes,name-too-long
+    """Cluster available hotfix version upgrade.
+
+    All required parameters must be populated in order to send to server.
+
+    :ivar upgrade_type: Type of upgrade. Required. Known values are: "AKSPatchUpgrade" and
+     "HotfixUpgrade".
+    :vartype upgrade_type: str or
+     ~azure.mgmt.hdinsightcontainers.models.ClusterAvailableUpgradeType
+    :ivar description: Hotfix version upgrade description.
+    :vartype description: str
+    :ivar source_oss_version: Source OSS version of current cluster component.
+    :vartype source_oss_version: str
+    :ivar source_cluster_version: Source cluster version of current cluster component.
+    :vartype source_cluster_version: str
+    :ivar source_build_number: Source build number of current cluster component.
+    :vartype source_build_number: str
+    :ivar target_oss_version: Target OSS version of component to be upgraded.
+    :vartype target_oss_version: str
+    :ivar target_cluster_version: Target cluster version of component to be upgraded.
+    :vartype target_cluster_version: str
+    :ivar target_build_number: Target build number of component to be upgraded.
+    :vartype target_build_number: str
+    :ivar component_name: Name of component to be upgraded.
+    :vartype component_name: str
+    :ivar severity: Severity of this upgrade. Known values are: "low", "medium", "high", and
+     "critical".
+    :vartype severity: str or ~azure.mgmt.hdinsightcontainers.models.Severity
+    :ivar extended_properties: Extended properties of current available upgrade version.
+    :vartype extended_properties: str
+    :ivar created_time: Created time of current available upgrade version.
+    :vartype created_time: ~datetime.datetime
+    """
+
+    _validation = {
+        "upgrade_type": {"required": True},
+    }
+
+    _attribute_map = {
+        "upgrade_type": {"key": "upgradeType", "type": "str"},
+        "description": {"key": "description", "type": "str"},
+        "source_oss_version": {"key": "sourceOssVersion", "type": "str"},
+        "source_cluster_version": {"key": "sourceClusterVersion", "type": "str"},
+        "source_build_number": {"key": "sourceBuildNumber", "type": "str"},
+        "target_oss_version": {"key": "targetOssVersion", "type": "str"},
+        "target_cluster_version": {"key": "targetClusterVersion", "type": "str"},
+        "target_build_number": {"key": "targetBuildNumber", "type": "str"},
+        "component_name": {"key": "componentName", "type": "str"},
+        "severity": {"key": "severity", "type": "str"},
+        "extended_properties": {"key": "extendedProperties", "type": "str"},
+        "created_time": {"key": "createdTime", "type": "iso-8601"},
+    }
+
+    def __init__(
+        self,
+        *,
+        description: Optional[str] = None,
+        source_oss_version: Optional[str] = None,
+        source_cluster_version: Optional[str] = None,
+        source_build_number: Optional[str] = None,
+        target_oss_version: Optional[str] = None,
+        target_cluster_version: Optional[str] = None,
+        target_build_number: Optional[str] = None,
+        component_name: Optional[str] = None,
+        severity: Optional[Union[str, "_models.Severity"]] = None,
+        extended_properties: Optional[str] = None,
+        created_time: Optional[datetime.datetime] = None,
+        **kwargs: Any
+    ) -> None:
+        """
+        :keyword description: Hotfix version upgrade description.
+        :paramtype description: str
+        :keyword source_oss_version: Source OSS version of current cluster component.
+        :paramtype source_oss_version: str
+        :keyword source_cluster_version: Source cluster version of current cluster component.
+        :paramtype source_cluster_version: str
+        :keyword source_build_number: Source build number of current cluster component.
+        :paramtype source_build_number: str
+        :keyword target_oss_version: Target OSS version of component to be upgraded.
+        :paramtype target_oss_version: str
+        :keyword target_cluster_version: Target cluster version of component to be upgraded.
+        :paramtype target_cluster_version: str
+        :keyword target_build_number: Target build number of component to be upgraded.
+        :paramtype target_build_number: str
+        :keyword component_name: Name of component to be upgraded.
+        :paramtype component_name: str
+        :keyword severity: Severity of this upgrade. Known values are: "low", "medium", "high", and
+         "critical".
+        :paramtype severity: str or ~azure.mgmt.hdinsightcontainers.models.Severity
+        :keyword extended_properties: Extended properties of current available upgrade version.
+        :paramtype extended_properties: str
+        :keyword created_time: Created time of current available upgrade version.
+        :paramtype created_time: ~datetime.datetime
+        """
+        super().__init__(**kwargs)
+        self.upgrade_type: str = "HotfixUpgrade"
+        self.description = description
+        self.source_oss_version = source_oss_version
+        self.source_cluster_version = source_cluster_version
+        self.source_build_number = source_build_number
+        self.target_oss_version = target_oss_version
+        self.target_cluster_version = target_cluster_version
+        self.target_build_number = target_build_number
+        self.component_name = component_name
+        self.severity = severity
+        self.extended_properties = extended_properties
+        self.created_time = created_time
+
+
+class ClusterAvailableUpgradeList(_serialization.Model):
+    """Collection of cluster available upgrade.
+
+    All required parameters must be populated in order to send to server.
+
+    :ivar value: Collection of Cluster available upgrade. Required.
+    :vartype value: list[~azure.mgmt.hdinsightcontainers.models.ClusterAvailableUpgrade]
+    :ivar next_link: The URL of next result page.
+    :vartype next_link: str
+    """
+
+    _validation = {
+        "value": {"required": True},
+    }
+
+    _attribute_map = {
+        "value": {"key": "value", "type": "[ClusterAvailableUpgrade]"},
+        "next_link": {"key": "nextLink", "type": "str"},
+    }
+
+    def __init__(
+        self, *, value: List["_models.ClusterAvailableUpgrade"], next_link: Optional[str] = None, **kwargs: Any
+    ) -> None:
+        """
+        :keyword value: Collection of Cluster available upgrade. Required.
+        :paramtype value: list[~azure.mgmt.hdinsightcontainers.models.ClusterAvailableUpgrade]
+        :keyword next_link: The URL of next result page.
+        :paramtype next_link: str
+        """
+        super().__init__(**kwargs)
+        self.value = value
+        self.next_link = next_link
 
 
 class ClusterComponentsItem(_serialization.Model):
     """ClusterComponentsItem.
 
     :ivar name:
     :vartype name: str
@@ -495,15 +833,15 @@
         self.name = name
         self.version = version
 
 
 class ClusterConfigFile(_serialization.Model):
     """Cluster configuration files.
 
-    All required parameters must be populated in order to send to Azure.
+    All required parameters must be populated in order to send to server.
 
     :ivar file_name: Configuration file name. Required.
     :vartype file_name: str
     :ivar content: Free form content of the entire configuration file.
     :vartype content: str
     :ivar encoding: This property indicates if the content is encoded and is case-insensitive.
      Please set the value to base64 if the content is base64 encoded. Set it to none or skip it if
@@ -559,22 +897,79 @@
         self.file_name = file_name
         self.content = content
         self.encoding = encoding
         self.path = path
         self.values = values
 
 
+class ClusterHotfixUpgradeProperties(ClusterUpgradeProperties):
+    """Properties of upgrading cluster's hotfix.
+
+    All required parameters must be populated in order to send to server.
+
+    :ivar upgrade_type: Type of upgrade. Required. Known values are: "AKSPatchUpgrade" and
+     "HotfixUpgrade".
+    :vartype upgrade_type: str or ~azure.mgmt.hdinsightcontainers.models.ClusterUpgradeType
+    :ivar target_oss_version: Target OSS version of component to be upgraded.
+    :vartype target_oss_version: str
+    :ivar target_cluster_version: Target cluster version of component to be upgraded.
+    :vartype target_cluster_version: str
+    :ivar target_build_number: Target build number of component to be upgraded.
+    :vartype target_build_number: str
+    :ivar component_name: Name of component to be upgraded.
+    :vartype component_name: str
+    """
+
+    _validation = {
+        "upgrade_type": {"required": True},
+    }
+
+    _attribute_map = {
+        "upgrade_type": {"key": "upgradeType", "type": "str"},
+        "target_oss_version": {"key": "targetOssVersion", "type": "str"},
+        "target_cluster_version": {"key": "targetClusterVersion", "type": "str"},
+        "target_build_number": {"key": "targetBuildNumber", "type": "str"},
+        "component_name": {"key": "componentName", "type": "str"},
+    }
+
+    def __init__(
+        self,
+        *,
+        target_oss_version: Optional[str] = None,
+        target_cluster_version: Optional[str] = None,
+        target_build_number: Optional[str] = None,
+        component_name: Optional[str] = None,
+        **kwargs: Any
+    ) -> None:
+        """
+        :keyword target_oss_version: Target OSS version of component to be upgraded.
+        :paramtype target_oss_version: str
+        :keyword target_cluster_version: Target cluster version of component to be upgraded.
+        :paramtype target_cluster_version: str
+        :keyword target_build_number: Target build number of component to be upgraded.
+        :paramtype target_build_number: str
+        :keyword component_name: Name of component to be upgraded.
+        :paramtype component_name: str
+        """
+        super().__init__(**kwargs)
+        self.upgrade_type: str = "HotfixUpgrade"
+        self.target_oss_version = target_oss_version
+        self.target_cluster_version = target_cluster_version
+        self.target_build_number = target_build_number
+        self.component_name = component_name
+
+
 class ClusterInstanceViewProperties(_serialization.Model):
     """Cluster Instance View Properties.
 
-    All required parameters must be populated in order to send to Azure.
+    All required parameters must be populated in order to send to server.
 
     :ivar status: Status of the instance view. Required.
     :vartype status: ~azure.mgmt.hdinsightcontainers.models.ClusterInstanceViewPropertiesStatus
-    :ivar service_statuses: List of statuses of relevant services that make up the HDInsight on aks
+    :ivar service_statuses: List of statuses of relevant services that make up the HDInsight on AKS
      cluster to surface to the customer. Required.
     :vartype service_statuses: list[~azure.mgmt.hdinsightcontainers.models.ServiceStatus]
     """
 
     _validation = {
         "status": {"required": True},
         "service_statuses": {"required": True},
@@ -592,26 +987,26 @@
         service_statuses: List["_models.ServiceStatus"],
         **kwargs: Any
     ) -> None:
         """
         :keyword status: Status of the instance view. Required.
         :paramtype status: ~azure.mgmt.hdinsightcontainers.models.ClusterInstanceViewPropertiesStatus
         :keyword service_statuses: List of statuses of relevant services that make up the HDInsight on
-         aks cluster to surface to the customer. Required.
+         AKS cluster to surface to the customer. Required.
         :paramtype service_statuses: list[~azure.mgmt.hdinsightcontainers.models.ServiceStatus]
         """
         super().__init__(**kwargs)
         self.status = status
         self.service_statuses = service_statuses
 
 
 class ClusterInstanceViewStatus(_serialization.Model):
     """Status of the instance view.
 
-    All required parameters must be populated in order to send to Azure.
+    All required parameters must be populated in order to send to server.
 
     :ivar ready: The cluster ready status. Required.
     :vartype ready: str
     :ivar reason: The status reason.
     :vartype reason: str
     :ivar message: The additional message.
     :vartype message: str
@@ -643,135 +1038,71 @@
         self.reason = reason
         self.message = message
 
 
 class ClusterInstanceViewPropertiesStatus(ClusterInstanceViewStatus):
     """Status of the instance view.
 
-    All required parameters must be populated in order to send to Azure.
+    All required parameters must be populated in order to send to server.
 
     :ivar ready: The cluster ready status. Required.
     :vartype ready: str
     :ivar reason: The status reason.
     :vartype reason: str
     :ivar message: The additional message.
     :vartype message: str
     """
 
-    _validation = {
-        "ready": {"required": True},
-    }
-
-    _attribute_map = {
-        "ready": {"key": "ready", "type": "str"},
-        "reason": {"key": "reason", "type": "str"},
-        "message": {"key": "message", "type": "str"},
-    }
-
-    def __init__(
-        self, *, ready: str, reason: Optional[str] = None, message: Optional[str] = None, **kwargs: Any
-    ) -> None:
-        """
-        :keyword ready: The cluster ready status. Required.
-        :paramtype ready: str
-        :keyword reason: The status reason.
-        :paramtype reason: str
-        :keyword message: The additional message.
-        :paramtype message: str
-        """
-        super().__init__(ready=ready, reason=reason, message=message, **kwargs)
-
 
 class ClusterInstanceViewResult(_serialization.Model):
     """Cluster Instance View.
 
-    All required parameters must be populated in order to send to Azure.
+    All required parameters must be populated in order to send to server.
 
     :ivar name: Name of the instance view. Required.
     :vartype name: str
-    :ivar status: Status of the instance view. Required.
-    :vartype status: ~azure.mgmt.hdinsightcontainers.models.ClusterInstanceViewPropertiesStatus
-    :ivar service_statuses: List of statuses of relevant services that make up the HDInsight on aks
-     cluster to surface to the customer. Required.
-    :vartype service_statuses: list[~azure.mgmt.hdinsightcontainers.models.ServiceStatus]
+    :ivar properties: Properties of the instance view. Required.
+    :vartype properties: ~azure.mgmt.hdinsightcontainers.models.ClusterInstanceViewResultProperties
     """
 
     _validation = {
         "name": {"required": True},
-        "status": {"required": True},
-        "service_statuses": {"required": True},
+        "properties": {"required": True},
     }
 
     _attribute_map = {
         "name": {"key": "name", "type": "str"},
-        "status": {"key": "properties.status", "type": "ClusterInstanceViewPropertiesStatus"},
-        "service_statuses": {"key": "properties.serviceStatuses", "type": "[ServiceStatus]"},
+        "properties": {"key": "properties", "type": "ClusterInstanceViewResultProperties"},
     }
 
-    def __init__(
-        self,
-        *,
-        name: str,
-        status: "_models.ClusterInstanceViewPropertiesStatus",
-        service_statuses: List["_models.ServiceStatus"],
-        **kwargs: Any
-    ) -> None:
+    def __init__(self, *, name: str, properties: "_models.ClusterInstanceViewResultProperties", **kwargs: Any) -> None:
         """
         :keyword name: Name of the instance view. Required.
         :paramtype name: str
-        :keyword status: Status of the instance view. Required.
-        :paramtype status: ~azure.mgmt.hdinsightcontainers.models.ClusterInstanceViewPropertiesStatus
-        :keyword service_statuses: List of statuses of relevant services that make up the HDInsight on
-         aks cluster to surface to the customer. Required.
-        :paramtype service_statuses: list[~azure.mgmt.hdinsightcontainers.models.ServiceStatus]
+        :keyword properties: Properties of the instance view. Required.
+        :paramtype properties:
+         ~azure.mgmt.hdinsightcontainers.models.ClusterInstanceViewResultProperties
         """
         super().__init__(**kwargs)
         self.name = name
-        self.status = status
-        self.service_statuses = service_statuses
+        self.properties = properties
 
 
 class ClusterInstanceViewResultProperties(ClusterInstanceViewProperties):
     """Properties of the instance view.
 
-    All required parameters must be populated in order to send to Azure.
+    All required parameters must be populated in order to send to server.
 
     :ivar status: Status of the instance view. Required.
     :vartype status: ~azure.mgmt.hdinsightcontainers.models.ClusterInstanceViewPropertiesStatus
-    :ivar service_statuses: List of statuses of relevant services that make up the HDInsight on aks
+    :ivar service_statuses: List of statuses of relevant services that make up the HDInsight on AKS
      cluster to surface to the customer. Required.
     :vartype service_statuses: list[~azure.mgmt.hdinsightcontainers.models.ServiceStatus]
     """
 
-    _validation = {
-        "status": {"required": True},
-        "service_statuses": {"required": True},
-    }
-
-    _attribute_map = {
-        "status": {"key": "status", "type": "ClusterInstanceViewPropertiesStatus"},
-        "service_statuses": {"key": "serviceStatuses", "type": "[ServiceStatus]"},
-    }
-
-    def __init__(
-        self,
-        *,
-        status: "_models.ClusterInstanceViewPropertiesStatus",
-        service_statuses: List["_models.ServiceStatus"],
-        **kwargs: Any
-    ) -> None:
-        """
-        :keyword status: Status of the instance view. Required.
-        :paramtype status: ~azure.mgmt.hdinsightcontainers.models.ClusterInstanceViewPropertiesStatus
-        :keyword service_statuses: List of statuses of relevant services that make up the HDInsight on
-         aks cluster to surface to the customer. Required.
-        :paramtype service_statuses: list[~azure.mgmt.hdinsightcontainers.models.ServiceStatus]
-        """
-        super().__init__(status=status, service_statuses=service_statuses, **kwargs)
-
 
 class ClusterInstanceViewsResult(_serialization.Model):
     """The instance view of a HDInsight Cluster.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
     :ivar value: Cluster instance view array.
@@ -795,61 +1126,23 @@
         :paramtype value: list[~azure.mgmt.hdinsightcontainers.models.ClusterInstanceViewResult]
         """
         super().__init__(**kwargs)
         self.value = value
         self.next_link = None
 
 
-class ProxyResource(Resource):
-    """The resource model definition for a Azure Resource Manager proxy resource. It will not have
-    tags and a location.
-
-    Variables are only populated by the server, and will be ignored when sending a request.
-
-    :ivar id: Fully qualified resource ID for the resource. E.g.
-     "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{resourceType}/{resourceName}".
-    :vartype id: str
-    :ivar name: The name of the resource.
-    :vartype name: str
-    :ivar type: The type of the resource. E.g. "Microsoft.Compute/virtualMachines" or
-     "Microsoft.Storage/storageAccounts".
-    :vartype type: str
-    :ivar system_data: Azure Resource Manager metadata containing createdBy and modifiedBy
-     information.
-    :vartype system_data: ~azure.mgmt.hdinsightcontainers.models.SystemData
-    """
-
-    _validation = {
-        "id": {"readonly": True},
-        "name": {"readonly": True},
-        "type": {"readonly": True},
-        "system_data": {"readonly": True},
-    }
-
-    _attribute_map = {
-        "id": {"key": "id", "type": "str"},
-        "name": {"key": "name", "type": "str"},
-        "type": {"key": "type", "type": "str"},
-        "system_data": {"key": "systemData", "type": "SystemData"},
-    }
-
-    def __init__(self, **kwargs: Any) -> None:
-        """ """
-        super().__init__(**kwargs)
-
-
 class ClusterJob(ProxyResource):
     """Cluster job.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
-    All required parameters must be populated in order to send to Azure.
+    All required parameters must be populated in order to send to server.
 
     :ivar id: Fully qualified resource ID for the resource. E.g.
-     "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{resourceType}/{resourceName}".
+     "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{resourceType}/{resourceName}".  # pylint: disable=line-too-long
     :vartype id: str
     :ivar name: The name of the resource.
     :vartype name: str
     :ivar type: The type of the resource. E.g. "Microsoft.Compute/virtualMachines" or
      "Microsoft.Storage/storageAccounts".
     :vartype type: str
     :ivar system_data: Azure Resource Manager metadata containing createdBy and modifiedBy
@@ -883,15 +1176,15 @@
         super().__init__(**kwargs)
         self.properties = properties
 
 
 class ClusterJobList(_serialization.Model):
     """Collection of cluster job.
 
-    All required parameters must be populated in order to send to Azure.
+    All required parameters must be populated in order to send to server.
 
     :ivar value: Collection of cluster job. Required.
     :vartype value: list[~azure.mgmt.hdinsightcontainers.models.ClusterJob]
     :ivar next_link: The Url of next result page.
     :vartype next_link: str
     """
 
@@ -918,15 +1211,15 @@
 
 class ClusterJobProperties(_serialization.Model):
     """Properties of cluster job.
 
     You probably want to use the sub-classes and not this class directly. Known sub-classes are:
     FlinkJobProperties
 
-    All required parameters must be populated in order to send to Azure.
+    All required parameters must be populated in order to send to server.
 
     :ivar job_type: Type of cluster job. Required. "FlinkJob"
     :vartype job_type: str or ~azure.mgmt.hdinsightcontainers.models.JobType
     """
 
     _validation = {
         "job_type": {"required": True},
@@ -1001,15 +1294,15 @@
         self.std_out_enabled = std_out_enabled
         self.std_error_enabled = std_error_enabled
 
 
 class ClusterLogAnalyticsProfile(_serialization.Model):
     """Cluster log analytics profile to enable or disable OMS agent for cluster.
 
-    All required parameters must be populated in order to send to Azure.
+    All required parameters must be populated in order to send to server.
 
     :ivar enabled: True if log analytics is enabled for the cluster, otherwise false. Required.
     :vartype enabled: bool
     :ivar application_logs: Collection of logs to be enabled or disabled for log analytics.
     :vartype application_logs:
      ~azure.mgmt.hdinsightcontainers.models.ClusterLogAnalyticsApplicationLogs
     :ivar metrics_enabled: True if metrics are enabled, otherwise false.
@@ -1045,38 +1338,90 @@
         """
         super().__init__(**kwargs)
         self.enabled = enabled
         self.application_logs = application_logs
         self.metrics_enabled = metrics_enabled
 
 
-class ClusterPatch(TrackedResource):
+class ClusterPatch(_serialization.Model):
     """The patch for a cluster.
 
+    :ivar properties: Define cluster patch specific properties.
+    :vartype properties: ~azure.mgmt.hdinsightcontainers.models.ClusterPatchProperties
+    :ivar tags: Resource tags.
+    :vartype tags: dict[str, str]
+    """
+
+    _attribute_map = {
+        "properties": {"key": "properties", "type": "ClusterPatchProperties"},
+        "tags": {"key": "tags", "type": "{str}"},
+    }
+
+    def __init__(
+        self,
+        *,
+        properties: Optional["_models.ClusterPatchProperties"] = None,
+        tags: Optional[Dict[str, str]] = None,
+        **kwargs: Any
+    ) -> None:
+        """
+        :keyword properties: Define cluster patch specific properties.
+        :paramtype properties: ~azure.mgmt.hdinsightcontainers.models.ClusterPatchProperties
+        :keyword tags: Resource tags.
+        :paramtype tags: dict[str, str]
+        """
+        super().__init__(**kwargs)
+        self.properties = properties
+        self.tags = tags
+
+
+class ClusterPatchProperties(_serialization.Model):
+    """Cluster resource patch data.
+
+    :ivar cluster_profile: Cluster resource patch properties.
+    :vartype cluster_profile: ~azure.mgmt.hdinsightcontainers.models.UpdatableClusterProfile
+    """
+
+    _attribute_map = {
+        "cluster_profile": {"key": "clusterProfile", "type": "UpdatableClusterProfile"},
+    }
+
+    def __init__(self, *, cluster_profile: Optional["_models.UpdatableClusterProfile"] = None, **kwargs: Any) -> None:
+        """
+        :keyword cluster_profile: Cluster resource patch properties.
+        :paramtype cluster_profile: ~azure.mgmt.hdinsightcontainers.models.UpdatableClusterProfile
+        """
+        super().__init__(**kwargs)
+        self.cluster_profile = cluster_profile
+
+
+class ClusterPool(TrackedResource):
+    """Cluster pool.
+
     Variables are only populated by the server, and will be ignored when sending a request.
 
-    All required parameters must be populated in order to send to Azure.
+    All required parameters must be populated in order to send to server.
 
     :ivar id: Fully qualified resource ID for the resource. E.g.
-     "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{resourceType}/{resourceName}".
+     "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{resourceType}/{resourceName}".  # pylint: disable=line-too-long
     :vartype id: str
     :ivar name: The name of the resource.
     :vartype name: str
     :ivar type: The type of the resource. E.g. "Microsoft.Compute/virtualMachines" or
      "Microsoft.Storage/storageAccounts".
     :vartype type: str
     :ivar system_data: Azure Resource Manager metadata containing createdBy and modifiedBy
      information.
     :vartype system_data: ~azure.mgmt.hdinsightcontainers.models.SystemData
     :ivar tags: Resource tags.
     :vartype tags: dict[str, str]
     :ivar location: The geo-location where the resource lives. Required.
     :vartype location: str
-    :ivar cluster_profile: Cluster resource patch properties.
-    :vartype cluster_profile: ~azure.mgmt.hdinsightcontainers.models.UpdatableClusterProfile
+    :ivar properties: Gets or sets the properties. Define cluster pool specific properties.
+    :vartype properties: ~azure.mgmt.hdinsightcontainers.models.ClusterPoolResourceProperties
     """
 
     _validation = {
         "id": {"readonly": True},
         "name": {"readonly": True},
         "type": {"readonly": True},
         "system_data": {"readonly": True},
@@ -1086,191 +1431,347 @@
     _attribute_map = {
         "id": {"key": "id", "type": "str"},
         "name": {"key": "name", "type": "str"},
         "type": {"key": "type", "type": "str"},
         "system_data": {"key": "systemData", "type": "SystemData"},
         "tags": {"key": "tags", "type": "{str}"},
         "location": {"key": "location", "type": "str"},
-        "cluster_profile": {"key": "properties.clusterProfile", "type": "UpdatableClusterProfile"},
+        "properties": {"key": "properties", "type": "ClusterPoolResourceProperties"},
     }
 
     def __init__(
         self,
         *,
         location: str,
         tags: Optional[Dict[str, str]] = None,
-        cluster_profile: Optional["_models.UpdatableClusterProfile"] = None,
+        properties: Optional["_models.ClusterPoolResourceProperties"] = None,
         **kwargs: Any
     ) -> None:
         """
         :keyword tags: Resource tags.
         :paramtype tags: dict[str, str]
         :keyword location: The geo-location where the resource lives. Required.
         :paramtype location: str
-        :keyword cluster_profile: Cluster resource patch properties.
-        :paramtype cluster_profile: ~azure.mgmt.hdinsightcontainers.models.UpdatableClusterProfile
+        :keyword properties: Gets or sets the properties. Define cluster pool specific properties.
+        :paramtype properties: ~azure.mgmt.hdinsightcontainers.models.ClusterPoolResourceProperties
         """
         super().__init__(tags=tags, location=location, **kwargs)
-        self.cluster_profile = cluster_profile
+        self.properties = properties
 
 
-class ClusterPool(TrackedResource):  # pylint: disable=too-many-instance-attributes
-    """Cluster pool.
+class ClusterPoolUpgradeProperties(_serialization.Model):
+    """Properties of upgrading cluster pool.
+
+    You probably want to use the sub-classes and not this class directly. Known sub-classes are:
+    ClusterPoolAKSPatchVersionUpgradeProperties, ClusterPoolNodeOsImageUpdateProperties
+
+    All required parameters must be populated in order to send to server.
+
+    :ivar upgrade_type: Type of upgrade. Required. Known values are: "AKSPatchUpgrade" and
+     "NodeOsUpgrade".
+    :vartype upgrade_type: str or ~azure.mgmt.hdinsightcontainers.models.ClusterPoolUpgradeType
+    """
+
+    _validation = {
+        "upgrade_type": {"required": True},
+    }
+
+    _attribute_map = {
+        "upgrade_type": {"key": "upgradeType", "type": "str"},
+    }
+
+    _subtype_map = {
+        "upgrade_type": {
+            "AKSPatchUpgrade": "ClusterPoolAKSPatchVersionUpgradeProperties",
+            "NodeOsUpgrade": "ClusterPoolNodeOsImageUpdateProperties",
+        }
+    }
+
+    def __init__(self, **kwargs: Any) -> None:
+        """ """
+        super().__init__(**kwargs)
+        self.upgrade_type: Optional[str] = None
 
-    Variables are only populated by the server, and will be ignored when sending a request.
 
-    All required parameters must be populated in order to send to Azure.
+class ClusterPoolAKSPatchVersionUpgradeProperties(ClusterPoolUpgradeProperties):  # pylint: disable=name-too-long
+    """Properties of upgrading cluster pool's AKS patch version.
+
+    All required parameters must be populated in order to send to server.
+
+    :ivar upgrade_type: Type of upgrade. Required. Known values are: "AKSPatchUpgrade" and
+     "NodeOsUpgrade".
+    :vartype upgrade_type: str or ~azure.mgmt.hdinsightcontainers.models.ClusterPoolUpgradeType
+    :ivar upgrade_cluster_pool: whether upgrade cluster pool or not. If it's true,
+     upgradeAllClusterNodes should be false.
+    :vartype upgrade_cluster_pool: bool
+    :ivar upgrade_all_cluster_nodes: whether upgrade all clusters' nodes. If it's true,
+     upgradeClusterPool should be false.
+    :vartype upgrade_all_cluster_nodes: bool
+    :ivar target_aks_version: Target AKS version. When it's not set, latest version will be used.
+     When upgradeClusterPool is true and upgradeAllClusterNodes is false, target version should be
+     greater or equal to current version. When upgradeClusterPool is false and
+     upgradeAllClusterNodes is true, target version should be equal to AKS version of cluster pool.
+    :vartype target_aks_version: str
+    """
+
+    _validation = {
+        "upgrade_type": {"required": True},
+    }
+
+    _attribute_map = {
+        "upgrade_type": {"key": "upgradeType", "type": "str"},
+        "upgrade_cluster_pool": {"key": "upgradeClusterPool", "type": "bool"},
+        "upgrade_all_cluster_nodes": {"key": "upgradeAllClusterNodes", "type": "bool"},
+        "target_aks_version": {"key": "targetAksVersion", "type": "str"},
+    }
+
+    def __init__(
+        self,
+        *,
+        upgrade_cluster_pool: bool = False,
+        upgrade_all_cluster_nodes: bool = False,
+        target_aks_version: Optional[str] = None,
+        **kwargs: Any
+    ) -> None:
+        """
+        :keyword upgrade_cluster_pool: whether upgrade cluster pool or not. If it's true,
+         upgradeAllClusterNodes should be false.
+        :paramtype upgrade_cluster_pool: bool
+        :keyword upgrade_all_cluster_nodes: whether upgrade all clusters' nodes. If it's true,
+         upgradeClusterPool should be false.
+        :paramtype upgrade_all_cluster_nodes: bool
+        :keyword target_aks_version: Target AKS version. When it's not set, latest version will be
+         used. When upgradeClusterPool is true and upgradeAllClusterNodes is false, target version
+         should be greater or equal to current version. When upgradeClusterPool is false and
+         upgradeAllClusterNodes is true, target version should be equal to AKS version of cluster pool.
+        :paramtype target_aks_version: str
+        """
+        super().__init__(**kwargs)
+        self.upgrade_type: str = "AKSPatchUpgrade"
+        self.upgrade_cluster_pool = upgrade_cluster_pool
+        self.upgrade_all_cluster_nodes = upgrade_all_cluster_nodes
+        self.target_aks_version = target_aks_version
+
+
+class ClusterPoolAvailableUpgrade(ProxyResource):
+    """Cluster pool available upgrade.
+
+    Variables are only populated by the server, and will be ignored when sending a request.
 
     :ivar id: Fully qualified resource ID for the resource. E.g.
-     "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{resourceType}/{resourceName}".
+     "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{resourceType}/{resourceName}".  # pylint: disable=line-too-long
     :vartype id: str
     :ivar name: The name of the resource.
     :vartype name: str
     :ivar type: The type of the resource. E.g. "Microsoft.Compute/virtualMachines" or
      "Microsoft.Storage/storageAccounts".
     :vartype type: str
     :ivar system_data: Azure Resource Manager metadata containing createdBy and modifiedBy
      information.
     :vartype system_data: ~azure.mgmt.hdinsightcontainers.models.SystemData
-    :ivar tags: Resource tags.
-    :vartype tags: dict[str, str]
-    :ivar location: The geo-location where the resource lives. Required.
-    :vartype location: str
-    :ivar provisioning_state: Provisioning state of the resource. Known values are: "Accepted",
-     "Succeeded", "Canceled", and "Failed".
-    :vartype provisioning_state: str or ~azure.mgmt.hdinsightcontainers.models.ProvisioningStatus
-    :ivar deployment_id: A unique id generated by the RP to identify the resource.
-    :vartype deployment_id: str
-    :ivar managed_resource_group_name: A resource group created by RP, to hold the resources
-     created by RP on-behalf of customers. It will also be used to generate
-     aksManagedResourceGroupName by pattern: MC\ *{managedResourceGroupName}*\
-     {clusterPoolName}_{region}. Please make sure it meets resource group name restriction.
-    :vartype managed_resource_group_name: str
-    :ivar aks_managed_resource_group_name: A resource group created by AKS, to hold the
-     infrastructure resources created by AKS on-behalf of customers. It is generated by cluster pool
-     name and managed resource group name by pattern: MC\ *{managedResourceGroupName}*\
-     {clusterPoolName}_{region}.
-    :vartype aks_managed_resource_group_name: str
-    :ivar cluster_pool_profile: CLuster pool profile.
-    :vartype cluster_pool_profile:
-     ~azure.mgmt.hdinsightcontainers.models.ClusterPoolResourcePropertiesClusterPoolProfile
-    :ivar compute_profile: CLuster pool compute profile.
-    :vartype compute_profile:
-     ~azure.mgmt.hdinsightcontainers.models.ClusterPoolResourcePropertiesComputeProfile
-    :ivar aks_cluster_profile: Properties of underlying AKS cluster.
-    :vartype aks_cluster_profile:
-     ~azure.mgmt.hdinsightcontainers.models.ClusterPoolResourcePropertiesAksClusterProfile
-    :ivar network_profile: Cluster pool network profile.
-    :vartype network_profile:
-     ~azure.mgmt.hdinsightcontainers.models.ClusterPoolResourcePropertiesNetworkProfile
-    :ivar log_analytics_profile: Cluster pool log analytics profile to enable OMS agent for AKS
-     cluster.
-    :vartype log_analytics_profile:
-     ~azure.mgmt.hdinsightcontainers.models.ClusterPoolResourcePropertiesLogAnalyticsProfile
-    :ivar status: Business status of the resource.
-    :vartype status: str
+    :ivar properties: Gets or sets the properties. Define cluster pool upgrade specific properties.
+    :vartype properties:
+     ~azure.mgmt.hdinsightcontainers.models.ClusterPoolAvailableUpgradeProperties
     """
 
     _validation = {
         "id": {"readonly": True},
         "name": {"readonly": True},
         "type": {"readonly": True},
         "system_data": {"readonly": True},
-        "location": {"required": True},
-        "provisioning_state": {"readonly": True},
-        "deployment_id": {"readonly": True},
-        "managed_resource_group_name": {"max_length": 40, "min_length": 1},
-        "aks_managed_resource_group_name": {"readonly": True},
-        "aks_cluster_profile": {"readonly": True},
-        "status": {"readonly": True},
     }
 
     _attribute_map = {
         "id": {"key": "id", "type": "str"},
         "name": {"key": "name", "type": "str"},
         "type": {"key": "type", "type": "str"},
         "system_data": {"key": "systemData", "type": "SystemData"},
-        "tags": {"key": "tags", "type": "{str}"},
-        "location": {"key": "location", "type": "str"},
-        "provisioning_state": {"key": "properties.provisioningState", "type": "str"},
-        "deployment_id": {"key": "properties.deploymentId", "type": "str"},
-        "managed_resource_group_name": {"key": "properties.managedResourceGroupName", "type": "str"},
-        "aks_managed_resource_group_name": {"key": "properties.aksManagedResourceGroupName", "type": "str"},
-        "cluster_pool_profile": {
-            "key": "properties.clusterPoolProfile",
-            "type": "ClusterPoolResourcePropertiesClusterPoolProfile",
-        },
-        "compute_profile": {"key": "properties.computeProfile", "type": "ClusterPoolResourcePropertiesComputeProfile"},
-        "aks_cluster_profile": {
-            "key": "properties.aksClusterProfile",
-            "type": "ClusterPoolResourcePropertiesAksClusterProfile",
-        },
-        "network_profile": {"key": "properties.networkProfile", "type": "ClusterPoolResourcePropertiesNetworkProfile"},
-        "log_analytics_profile": {
-            "key": "properties.logAnalyticsProfile",
-            "type": "ClusterPoolResourcePropertiesLogAnalyticsProfile",
-        },
-        "status": {"key": "properties.status", "type": "str"},
+        "properties": {"key": "properties", "type": "ClusterPoolAvailableUpgradeProperties"},
+    }
+
+    def __init__(
+        self, *, properties: Optional["_models.ClusterPoolAvailableUpgradeProperties"] = None, **kwargs: Any
+    ) -> None:
+        """
+        :keyword properties: Gets or sets the properties. Define cluster pool upgrade specific
+         properties.
+        :paramtype properties:
+         ~azure.mgmt.hdinsightcontainers.models.ClusterPoolAvailableUpgradeProperties
+        """
+        super().__init__(**kwargs)
+        self.properties = properties
+
+
+class ClusterPoolAvailableUpgradeProperties(_serialization.Model):
+    """Cluster pool available upgrade properties.
+
+    You probably want to use the sub-classes and not this class directly. Known sub-classes are:
+    ClusterPoolAvailableUpgradeAksPatchUpgradeProperties,
+    ClusterPoolAvailableUpgradeNodeOsUpgradeProperties
+
+    All required parameters must be populated in order to send to server.
+
+    :ivar upgrade_type: Type of upgrade. Required. Known values are: "AKSPatchUpgrade" and
+     "NodeOsUpgrade".
+    :vartype upgrade_type: str or
+     ~azure.mgmt.hdinsightcontainers.models.ClusterPoolAvailableUpgradeType
+    """
+
+    _validation = {
+        "upgrade_type": {"required": True},
+    }
+
+    _attribute_map = {
+        "upgrade_type": {"key": "upgradeType", "type": "str"},
+    }
+
+    _subtype_map = {
+        "upgrade_type": {
+            "AKSPatchUpgrade": "ClusterPoolAvailableUpgradeAksPatchUpgradeProperties",
+            "NodeOsUpgrade": "ClusterPoolAvailableUpgradeNodeOsUpgradeProperties",
+        }
+    }
+
+    def __init__(self, **kwargs: Any) -> None:
+        """ """
+        super().__init__(**kwargs)
+        self.upgrade_type: Optional[str] = None
+
+
+class ClusterPoolAvailableUpgradeAksPatchUpgradeProperties(
+    ClusterPoolAvailableUpgradeProperties
+):  # pylint: disable=name-too-long
+    """Cluster pool available AKS patch version upgrade.
+
+    All required parameters must be populated in order to send to server.
+
+    :ivar upgrade_type: Type of upgrade. Required. Known values are: "AKSPatchUpgrade" and
+     "NodeOsUpgrade".
+    :vartype upgrade_type: str or
+     ~azure.mgmt.hdinsightcontainers.models.ClusterPoolAvailableUpgradeType
+    :ivar current_version: Current AKS version.
+    :vartype current_version: str
+    :ivar current_version_status: Current AKS version's status: whether it is deprecated or
+     supported. Known values are: "Deprecated" and "Supported".
+    :vartype current_version_status: str or
+     ~azure.mgmt.hdinsightcontainers.models.CurrentClusterPoolAksVersionStatus
+    :ivar latest_version: Latest AKS patch version.
+    :vartype latest_version: str
+    """
+
+    _validation = {
+        "upgrade_type": {"required": True},
+    }
+
+    _attribute_map = {
+        "upgrade_type": {"key": "upgradeType", "type": "str"},
+        "current_version": {"key": "currentVersion", "type": "str"},
+        "current_version_status": {"key": "currentVersionStatus", "type": "str"},
+        "latest_version": {"key": "latestVersion", "type": "str"},
     }
 
     def __init__(
         self,
         *,
-        location: str,
-        tags: Optional[Dict[str, str]] = None,
-        managed_resource_group_name: Optional[str] = None,
-        cluster_pool_profile: Optional["_models.ClusterPoolResourcePropertiesClusterPoolProfile"] = None,
-        compute_profile: Optional["_models.ClusterPoolResourcePropertiesComputeProfile"] = None,
-        network_profile: Optional["_models.ClusterPoolResourcePropertiesNetworkProfile"] = None,
-        log_analytics_profile: Optional["_models.ClusterPoolResourcePropertiesLogAnalyticsProfile"] = None,
+        current_version: Optional[str] = None,
+        current_version_status: Optional[Union[str, "_models.CurrentClusterPoolAksVersionStatus"]] = None,
+        latest_version: Optional[str] = None,
         **kwargs: Any
     ) -> None:
         """
-        :keyword tags: Resource tags.
-        :paramtype tags: dict[str, str]
-        :keyword location: The geo-location where the resource lives. Required.
-        :paramtype location: str
-        :keyword managed_resource_group_name: A resource group created by RP, to hold the resources
-         created by RP on-behalf of customers. It will also be used to generate
-         aksManagedResourceGroupName by pattern: MC\ *{managedResourceGroupName}*\
-         {clusterPoolName}_{region}. Please make sure it meets resource group name restriction.
-        :paramtype managed_resource_group_name: str
-        :keyword cluster_pool_profile: CLuster pool profile.
-        :paramtype cluster_pool_profile:
-         ~azure.mgmt.hdinsightcontainers.models.ClusterPoolResourcePropertiesClusterPoolProfile
-        :keyword compute_profile: CLuster pool compute profile.
-        :paramtype compute_profile:
-         ~azure.mgmt.hdinsightcontainers.models.ClusterPoolResourcePropertiesComputeProfile
-        :keyword network_profile: Cluster pool network profile.
-        :paramtype network_profile:
-         ~azure.mgmt.hdinsightcontainers.models.ClusterPoolResourcePropertiesNetworkProfile
-        :keyword log_analytics_profile: Cluster pool log analytics profile to enable OMS agent for AKS
-         cluster.
-        :paramtype log_analytics_profile:
-         ~azure.mgmt.hdinsightcontainers.models.ClusterPoolResourcePropertiesLogAnalyticsProfile
+        :keyword current_version: Current AKS version.
+        :paramtype current_version: str
+        :keyword current_version_status: Current AKS version's status: whether it is deprecated or
+         supported. Known values are: "Deprecated" and "Supported".
+        :paramtype current_version_status: str or
+         ~azure.mgmt.hdinsightcontainers.models.CurrentClusterPoolAksVersionStatus
+        :keyword latest_version: Latest AKS patch version.
+        :paramtype latest_version: str
         """
-        super().__init__(tags=tags, location=location, **kwargs)
-        self.provisioning_state = None
-        self.deployment_id = None
-        self.managed_resource_group_name = managed_resource_group_name
-        self.aks_managed_resource_group_name = None
-        self.cluster_pool_profile = cluster_pool_profile
-        self.compute_profile = compute_profile
-        self.aks_cluster_profile = None
-        self.network_profile = network_profile
-        self.log_analytics_profile = log_analytics_profile
-        self.status = None
+        super().__init__(**kwargs)
+        self.upgrade_type: str = "AKSPatchUpgrade"
+        self.current_version = current_version
+        self.current_version_status = current_version_status
+        self.latest_version = latest_version
+
+
+class ClusterPoolAvailableUpgradeList(_serialization.Model):
+    """collection of cluster pool available upgrade.
+
+    All required parameters must be populated in order to send to server.
+
+    :ivar value: Collection of cluster pool available upgrade. Required.
+    :vartype value: list[~azure.mgmt.hdinsightcontainers.models.ClusterPoolAvailableUpgrade]
+    :ivar next_link: The Url of next result page.
+    :vartype next_link: str
+    """
+
+    _validation = {
+        "value": {"required": True},
+    }
+
+    _attribute_map = {
+        "value": {"key": "value", "type": "[ClusterPoolAvailableUpgrade]"},
+        "next_link": {"key": "nextLink", "type": "str"},
+    }
+
+    def __init__(
+        self, *, value: List["_models.ClusterPoolAvailableUpgrade"], next_link: Optional[str] = None, **kwargs: Any
+    ) -> None:
+        """
+        :keyword value: Collection of cluster pool available upgrade. Required.
+        :paramtype value: list[~azure.mgmt.hdinsightcontainers.models.ClusterPoolAvailableUpgrade]
+        :keyword next_link: The Url of next result page.
+        :paramtype next_link: str
+        """
+        super().__init__(**kwargs)
+        self.value = value
+        self.next_link = next_link
+
+
+class ClusterPoolAvailableUpgradeNodeOsUpgradeProperties(
+    ClusterPoolAvailableUpgradeProperties
+):  # pylint: disable=name-too-long
+    """Cluster pool available node OS update.
+
+    All required parameters must be populated in order to send to server.
+
+    :ivar upgrade_type: Type of upgrade. Required. Known values are: "AKSPatchUpgrade" and
+     "NodeOsUpgrade".
+    :vartype upgrade_type: str or
+     ~azure.mgmt.hdinsightcontainers.models.ClusterPoolAvailableUpgradeType
+    :ivar latest_version: The latest node OS version.
+    :vartype latest_version: str
+    """
+
+    _validation = {
+        "upgrade_type": {"required": True},
+    }
+
+    _attribute_map = {
+        "upgrade_type": {"key": "upgradeType", "type": "str"},
+        "latest_version": {"key": "latestVersion", "type": "str"},
+    }
+
+    def __init__(self, *, latest_version: Optional[str] = None, **kwargs: Any) -> None:
+        """
+        :keyword latest_version: The latest node OS version.
+        :paramtype latest_version: str
+        """
+        super().__init__(**kwargs)
+        self.upgrade_type: str = "NodeOsUpgrade"
+        self.latest_version = latest_version
 
 
 class ClusterPoolComputeProfile(_serialization.Model):
     """Cluster pool compute profile.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
-    All required parameters must be populated in order to send to Azure.
+    All required parameters must be populated in order to send to server.
 
     :ivar vm_size: The virtual machine SKU. Required.
     :vartype vm_size: str
     :ivar count: The number of virtual machines.
     :vartype count: int
     """
 
@@ -1323,15 +1824,15 @@
         self.value = value
         self.next_link = None
 
 
 class ClusterPoolLogAnalyticsProfile(_serialization.Model):
     """Cluster pool log analytics profile used to enable or disable OMS agent for AKS cluster.
 
-    All required parameters must be populated in order to send to Azure.
+    All required parameters must be populated in order to send to server.
 
     :ivar enabled: True if log analytics is enabled for cluster pool, otherwise false. Required.
     :vartype enabled: bool
     :ivar workspace_id: Log analytics workspace to associate with the OMS agent.
     :vartype workspace_id: str
     """
 
@@ -1355,41 +1856,103 @@
         self.enabled = enabled
         self.workspace_id = workspace_id
 
 
 class ClusterPoolNetworkProfile(_serialization.Model):
     """Cluster pool networking configuration.
 
-    All required parameters must be populated in order to send to Azure.
+    All required parameters must be populated in order to send to server.
 
     :ivar subnet_id: Cluster pool subnet resource id. Required.
     :vartype subnet_id: str
+    :ivar outbound_type: This can only be set at cluster pool creation time and cannot be changed
+     later. Known values are: "loadBalancer" and "userDefinedRouting".
+    :vartype outbound_type: str or ~azure.mgmt.hdinsightcontainers.models.OutboundType
+    :ivar enable_private_api_server: ClusterPool is based on AKS cluster. AKS cluster exposes the
+     API server to public internet by default. If you set this property to true, a private AKS
+     cluster will be created, and it will use private apiserver, which is not exposed to public
+     internet.
+    :vartype enable_private_api_server: bool
+    :ivar api_server_authorized_ip_ranges: IP ranges are specified in CIDR format, e.g.
+     137.117.106.88/29. This feature is not compatible with private AKS clusters. So you cannot set
+     enablePrivateApiServer to true and apiServerAuthorizedIpRanges at the same time.
+    :vartype api_server_authorized_ip_ranges: list[str]
     """
 
     _validation = {
         "subnet_id": {"required": True},
     }
 
     _attribute_map = {
         "subnet_id": {"key": "subnetId", "type": "str"},
+        "outbound_type": {"key": "outboundType", "type": "str"},
+        "enable_private_api_server": {"key": "enablePrivateApiServer", "type": "bool"},
+        "api_server_authorized_ip_ranges": {"key": "apiServerAuthorizedIpRanges", "type": "[str]"},
     }
 
-    def __init__(self, *, subnet_id: str, **kwargs: Any) -> None:
+    def __init__(
+        self,
+        *,
+        subnet_id: str,
+        outbound_type: Union[str, "_models.OutboundType"] = "loadBalancer",
+        enable_private_api_server: Optional[bool] = None,
+        api_server_authorized_ip_ranges: Optional[List[str]] = None,
+        **kwargs: Any
+    ) -> None:
         """
         :keyword subnet_id: Cluster pool subnet resource id. Required.
         :paramtype subnet_id: str
+        :keyword outbound_type: This can only be set at cluster pool creation time and cannot be
+         changed later. Known values are: "loadBalancer" and "userDefinedRouting".
+        :paramtype outbound_type: str or ~azure.mgmt.hdinsightcontainers.models.OutboundType
+        :keyword enable_private_api_server: ClusterPool is based on AKS cluster. AKS cluster exposes
+         the API server to public internet by default. If you set this property to true, a private AKS
+         cluster will be created, and it will use private apiserver, which is not exposed to public
+         internet.
+        :paramtype enable_private_api_server: bool
+        :keyword api_server_authorized_ip_ranges: IP ranges are specified in CIDR format, e.g.
+         137.117.106.88/29. This feature is not compatible with private AKS clusters. So you cannot set
+         enablePrivateApiServer to true and apiServerAuthorizedIpRanges at the same time.
+        :paramtype api_server_authorized_ip_ranges: list[str]
         """
         super().__init__(**kwargs)
         self.subnet_id = subnet_id
+        self.outbound_type = outbound_type
+        self.enable_private_api_server = enable_private_api_server
+        self.api_server_authorized_ip_ranges = api_server_authorized_ip_ranges
+
+
+class ClusterPoolNodeOsImageUpdateProperties(ClusterPoolUpgradeProperties):
+    """Properties of upgrading cluster pool's AKS patch version.
+
+    All required parameters must be populated in order to send to server.
+
+    :ivar upgrade_type: Type of upgrade. Required. Known values are: "AKSPatchUpgrade" and
+     "NodeOsUpgrade".
+    :vartype upgrade_type: str or ~azure.mgmt.hdinsightcontainers.models.ClusterPoolUpgradeType
+    """
+
+    _validation = {
+        "upgrade_type": {"required": True},
+    }
+
+    _attribute_map = {
+        "upgrade_type": {"key": "upgradeType", "type": "str"},
+    }
+
+    def __init__(self, **kwargs: Any) -> None:
+        """ """
+        super().__init__(**kwargs)
+        self.upgrade_type: str = "NodeOsUpgrade"
 
 
 class ClusterPoolProfile(_serialization.Model):
     """Cluster pool profile.
 
-    All required parameters must be populated in order to send to Azure.
+    All required parameters must be populated in order to send to server.
 
     :ivar cluster_pool_version: Cluster pool version is a 2-part version. Required.
     :vartype cluster_pool_version: str
     """
 
     _validation = {
         "cluster_pool_version": {"required": True, "pattern": r"^(0|[1-9][0-9]{0,18})\.(0|[1-9][0-9]{0,18})$"},
@@ -1404,217 +1967,291 @@
         :keyword cluster_pool_version: Cluster pool version is a 2-part version. Required.
         :paramtype cluster_pool_version: str
         """
         super().__init__(**kwargs)
         self.cluster_pool_version = cluster_pool_version
 
 
-class ClusterPoolResourcePropertiesAksClusterProfile(AksClusterProfile):
-    """Properties of underlying AKS cluster.
+class ClusterPoolResourceProperties(_serialization.Model):
+    """Cluster pool resource properties.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
-    :ivar aks_cluster_resource_id: ARM Resource ID of the AKS cluster.
-    :vartype aks_cluster_resource_id: str
-    :ivar aks_cluster_agent_pool_identity_profile: Identity properties of the AKS cluster agentpool
-     MSI.
-    :vartype aks_cluster_agent_pool_identity_profile:
-     ~azure.mgmt.hdinsightcontainers.models.AksClusterProfileAksClusterAgentPoolIdentityProfile
-    :ivar aks_version: AKS control plane and default node pool version of this ClusterPool.
-    :vartype aks_version: str
+    All required parameters must be populated in order to send to server.
+
+    :ivar provisioning_state: Provisioning state of the resource. Known values are: "Accepted",
+     "Succeeded", "Canceled", and "Failed".
+    :vartype provisioning_state: str or ~azure.mgmt.hdinsightcontainers.models.ProvisioningStatus
+    :ivar deployment_id: A unique id generated by the RP to identify the resource.
+    :vartype deployment_id: str
+    :ivar managed_resource_group_name: A resource group created by RP, to hold the resources
+     created by RP on-behalf of customers. It will also be used to generate
+     aksManagedResourceGroupName by pattern: MC\ *{managedResourceGroupName}*\
+     {clusterPoolName}_{region}. Please make sure it meets resource group name restriction.
+    :vartype managed_resource_group_name: str
+    :ivar aks_managed_resource_group_name: A resource group created by AKS, to hold the
+     infrastructure resources created by AKS on-behalf of customers. It is generated by cluster pool
+     name and managed resource group name by pattern: MC\ *{managedResourceGroupName}*\
+     {clusterPoolName}_{region}.
+    :vartype aks_managed_resource_group_name: str
+    :ivar cluster_pool_profile: CLuster pool profile.
+    :vartype cluster_pool_profile:
+     ~azure.mgmt.hdinsightcontainers.models.ClusterPoolResourcePropertiesClusterPoolProfile
+    :ivar compute_profile: CLuster pool compute profile. Required.
+    :vartype compute_profile:
+     ~azure.mgmt.hdinsightcontainers.models.ClusterPoolResourcePropertiesComputeProfile
+    :ivar aks_cluster_profile: Properties of underlying AKS cluster.
+    :vartype aks_cluster_profile:
+     ~azure.mgmt.hdinsightcontainers.models.ClusterPoolResourcePropertiesAksClusterProfile
+    :ivar network_profile: Cluster pool network profile.
+    :vartype network_profile:
+     ~azure.mgmt.hdinsightcontainers.models.ClusterPoolResourcePropertiesNetworkProfile
+    :ivar log_analytics_profile: Cluster pool log analytics profile to enable OMS agent for AKS
+     cluster.
+    :vartype log_analytics_profile:
+     ~azure.mgmt.hdinsightcontainers.models.ClusterPoolResourcePropertiesLogAnalyticsProfile
+    :ivar status: Business status of the resource.
+    :vartype status: str
     """
 
     _validation = {
-        "aks_version": {"readonly": True},
+        "provisioning_state": {"readonly": True},
+        "deployment_id": {"readonly": True},
+        "managed_resource_group_name": {"max_length": 40, "min_length": 1},
+        "aks_managed_resource_group_name": {"readonly": True},
+        "compute_profile": {"required": True},
+        "aks_cluster_profile": {"readonly": True},
+        "status": {"readonly": True},
     }
 
     _attribute_map = {
-        "aks_cluster_resource_id": {"key": "aksClusterResourceId", "type": "str"},
-        "aks_cluster_agent_pool_identity_profile": {
-            "key": "aksClusterAgentPoolIdentityProfile",
-            "type": "AksClusterProfileAksClusterAgentPoolIdentityProfile",
+        "provisioning_state": {"key": "provisioningState", "type": "str"},
+        "deployment_id": {"key": "deploymentId", "type": "str"},
+        "managed_resource_group_name": {"key": "managedResourceGroupName", "type": "str"},
+        "aks_managed_resource_group_name": {"key": "aksManagedResourceGroupName", "type": "str"},
+        "cluster_pool_profile": {
+            "key": "clusterPoolProfile",
+            "type": "ClusterPoolResourcePropertiesClusterPoolProfile",
         },
-        "aks_version": {"key": "aksVersion", "type": "str"},
+        "compute_profile": {"key": "computeProfile", "type": "ClusterPoolResourcePropertiesComputeProfile"},
+        "aks_cluster_profile": {"key": "aksClusterProfile", "type": "ClusterPoolResourcePropertiesAksClusterProfile"},
+        "network_profile": {"key": "networkProfile", "type": "ClusterPoolResourcePropertiesNetworkProfile"},
+        "log_analytics_profile": {
+            "key": "logAnalyticsProfile",
+            "type": "ClusterPoolResourcePropertiesLogAnalyticsProfile",
+        },
+        "status": {"key": "status", "type": "str"},
     }
 
     def __init__(
         self,
         *,
-        aks_cluster_resource_id: Optional[str] = None,
-        aks_cluster_agent_pool_identity_profile: Optional[
-            "_models.AksClusterProfileAksClusterAgentPoolIdentityProfile"
-        ] = None,
+        compute_profile: "_models.ClusterPoolResourcePropertiesComputeProfile",
+        managed_resource_group_name: Optional[str] = None,
+        cluster_pool_profile: Optional["_models.ClusterPoolResourcePropertiesClusterPoolProfile"] = None,
+        network_profile: Optional["_models.ClusterPoolResourcePropertiesNetworkProfile"] = None,
+        log_analytics_profile: Optional["_models.ClusterPoolResourcePropertiesLogAnalyticsProfile"] = None,
         **kwargs: Any
     ) -> None:
         """
-        :keyword aks_cluster_resource_id: ARM Resource ID of the AKS cluster.
-        :paramtype aks_cluster_resource_id: str
-        :keyword aks_cluster_agent_pool_identity_profile: Identity properties of the AKS cluster
-         agentpool MSI.
-        :paramtype aks_cluster_agent_pool_identity_profile:
-         ~azure.mgmt.hdinsightcontainers.models.AksClusterProfileAksClusterAgentPoolIdentityProfile
-        """
-        super().__init__(
-            aks_cluster_resource_id=aks_cluster_resource_id,
-            aks_cluster_agent_pool_identity_profile=aks_cluster_agent_pool_identity_profile,
-            **kwargs
-        )
+        :keyword managed_resource_group_name: A resource group created by RP, to hold the resources
+         created by RP on-behalf of customers. It will also be used to generate
+         aksManagedResourceGroupName by pattern: MC\ *{managedResourceGroupName}*\
+         {clusterPoolName}_{region}. Please make sure it meets resource group name restriction.
+        :paramtype managed_resource_group_name: str
+        :keyword cluster_pool_profile: CLuster pool profile.
+        :paramtype cluster_pool_profile:
+         ~azure.mgmt.hdinsightcontainers.models.ClusterPoolResourcePropertiesClusterPoolProfile
+        :keyword compute_profile: CLuster pool compute profile. Required.
+        :paramtype compute_profile:
+         ~azure.mgmt.hdinsightcontainers.models.ClusterPoolResourcePropertiesComputeProfile
+        :keyword network_profile: Cluster pool network profile.
+        :paramtype network_profile:
+         ~azure.mgmt.hdinsightcontainers.models.ClusterPoolResourcePropertiesNetworkProfile
+        :keyword log_analytics_profile: Cluster pool log analytics profile to enable OMS agent for AKS
+         cluster.
+        :paramtype log_analytics_profile:
+         ~azure.mgmt.hdinsightcontainers.models.ClusterPoolResourcePropertiesLogAnalyticsProfile
+        """
+        super().__init__(**kwargs)
+        self.provisioning_state = None
+        self.deployment_id = None
+        self.managed_resource_group_name = managed_resource_group_name
+        self.aks_managed_resource_group_name = None
+        self.cluster_pool_profile = cluster_pool_profile
+        self.compute_profile = compute_profile
+        self.aks_cluster_profile = None
+        self.network_profile = network_profile
+        self.log_analytics_profile = log_analytics_profile
+        self.status = None
 
 
-class ClusterPoolResourcePropertiesClusterPoolProfile(ClusterPoolProfile):
-    """CLuster pool profile.
+class ClusterPoolResourcePropertiesAksClusterProfile(AksClusterProfile):  # pylint: disable=name-too-long
+    """Properties of underlying AKS cluster.
 
-    All required parameters must be populated in order to send to Azure.
+    Variables are only populated by the server, and will be ignored when sending a request.
 
-    :ivar cluster_pool_version: Cluster pool version is a 2-part version. Required.
-    :vartype cluster_pool_version: str
+    :ivar aks_cluster_resource_id: ARM Resource ID of the AKS cluster.
+    :vartype aks_cluster_resource_id: str
+    :ivar aks_cluster_agent_pool_identity_profile: Identity properties of the AKS cluster agentpool
+     MSI.
+    :vartype aks_cluster_agent_pool_identity_profile:
+     ~azure.mgmt.hdinsightcontainers.models.AksClusterProfileAksClusterAgentPoolIdentityProfile
+    :ivar aks_version: AKS control plane and default node pool version of this ClusterPool.
+    :vartype aks_version: str
     """
 
-    _validation = {
-        "cluster_pool_version": {"required": True, "pattern": r"^(0|[1-9][0-9]{0,18})\.(0|[1-9][0-9]{0,18})$"},
-    }
 
-    _attribute_map = {
-        "cluster_pool_version": {"key": "clusterPoolVersion", "type": "str"},
-    }
+class ClusterPoolResourcePropertiesClusterPoolProfile(ClusterPoolProfile):  # pylint: disable=name-too-long
+    """CLuster pool profile.
 
-    def __init__(self, *, cluster_pool_version: str, **kwargs: Any) -> None:
-        """
-        :keyword cluster_pool_version: Cluster pool version is a 2-part version. Required.
-        :paramtype cluster_pool_version: str
-        """
-        super().__init__(cluster_pool_version=cluster_pool_version, **kwargs)
+    All required parameters must be populated in order to send to server.
 
+    :ivar cluster_pool_version: Cluster pool version is a 2-part version. Required.
+    :vartype cluster_pool_version: str
+    """
 
-class ClusterPoolResourcePropertiesComputeProfile(ClusterPoolComputeProfile):
+
+class ClusterPoolResourcePropertiesComputeProfile(ClusterPoolComputeProfile):  # pylint: disable=name-too-long
     """CLuster pool compute profile.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
-    All required parameters must be populated in order to send to Azure.
+    All required parameters must be populated in order to send to server.
 
     :ivar vm_size: The virtual machine SKU. Required.
     :vartype vm_size: str
     :ivar count: The number of virtual machines.
     :vartype count: int
     """
 
-    _validation = {
-        "vm_size": {"required": True, "pattern": r"^[a-zA-Z0-9_\-]{0,256}$"},
-        "count": {"readonly": True},
-    }
-
-    _attribute_map = {
-        "vm_size": {"key": "vmSize", "type": "str"},
-        "count": {"key": "count", "type": "int"},
-    }
 
-    def __init__(self, *, vm_size: str, **kwargs: Any) -> None:
-        """
-        :keyword vm_size: The virtual machine SKU. Required.
-        :paramtype vm_size: str
-        """
-        super().__init__(vm_size=vm_size, **kwargs)
-
-
-class ClusterPoolResourcePropertiesLogAnalyticsProfile(ClusterPoolLogAnalyticsProfile):
+class ClusterPoolResourcePropertiesLogAnalyticsProfile(ClusterPoolLogAnalyticsProfile):  # pylint: disable=name-too-long
     """Cluster pool log analytics profile to enable OMS agent for AKS cluster.
 
-    All required parameters must be populated in order to send to Azure.
+    All required parameters must be populated in order to send to server.
 
     :ivar enabled: True if log analytics is enabled for cluster pool, otherwise false. Required.
     :vartype enabled: bool
     :ivar workspace_id: Log analytics workspace to associate with the OMS agent.
     :vartype workspace_id: str
     """
 
-    _validation = {
-        "enabled": {"required": True},
-    }
 
-    _attribute_map = {
-        "enabled": {"key": "enabled", "type": "bool"},
-        "workspace_id": {"key": "workspaceId", "type": "str"},
-    }
-
-    def __init__(self, *, enabled: bool, workspace_id: Optional[str] = None, **kwargs: Any) -> None:
-        """
-        :keyword enabled: True if log analytics is enabled for cluster pool, otherwise false. Required.
-        :paramtype enabled: bool
-        :keyword workspace_id: Log analytics workspace to associate with the OMS agent.
-        :paramtype workspace_id: str
-        """
-        super().__init__(enabled=enabled, workspace_id=workspace_id, **kwargs)
-
-
-class ClusterPoolResourcePropertiesNetworkProfile(ClusterPoolNetworkProfile):
+class ClusterPoolResourcePropertiesNetworkProfile(ClusterPoolNetworkProfile):  # pylint: disable=name-too-long
     """Cluster pool network profile.
 
-    All required parameters must be populated in order to send to Azure.
+    All required parameters must be populated in order to send to server.
 
     :ivar subnet_id: Cluster pool subnet resource id. Required.
     :vartype subnet_id: str
+    :ivar outbound_type: This can only be set at cluster pool creation time and cannot be changed
+     later. Known values are: "loadBalancer" and "userDefinedRouting".
+    :vartype outbound_type: str or ~azure.mgmt.hdinsightcontainers.models.OutboundType
+    :ivar enable_private_api_server: ClusterPool is based on AKS cluster. AKS cluster exposes the
+     API server to public internet by default. If you set this property to true, a private AKS
+     cluster will be created, and it will use private apiserver, which is not exposed to public
+     internet.
+    :vartype enable_private_api_server: bool
+    :ivar api_server_authorized_ip_ranges: IP ranges are specified in CIDR format, e.g.
+     137.117.106.88/29. This feature is not compatible with private AKS clusters. So you cannot set
+     enablePrivateApiServer to true and apiServerAuthorizedIpRanges at the same time.
+    :vartype api_server_authorized_ip_ranges: list[str]
+    """
+
+
+class ClusterPoolUpgrade(_serialization.Model):
+    """Cluster Pool Upgrade.
+
+    All required parameters must be populated in order to send to server.
+
+    :ivar properties: Properties of upgrading cluster pool. Required.
+    :vartype properties: ~azure.mgmt.hdinsightcontainers.models.ClusterPoolUpgradeProperties
     """
 
     _validation = {
-        "subnet_id": {"required": True},
+        "properties": {"required": True},
     }
 
     _attribute_map = {
-        "subnet_id": {"key": "subnetId", "type": "str"},
+        "properties": {"key": "properties", "type": "ClusterPoolUpgradeProperties"},
     }
 
-    def __init__(self, *, subnet_id: str, **kwargs: Any) -> None:
+    def __init__(self, *, properties: "_models.ClusterPoolUpgradeProperties", **kwargs: Any) -> None:
         """
-        :keyword subnet_id: Cluster pool subnet resource id. Required.
-        :paramtype subnet_id: str
+        :keyword properties: Properties of upgrading cluster pool. Required.
+        :paramtype properties: ~azure.mgmt.hdinsightcontainers.models.ClusterPoolUpgradeProperties
         """
-        super().__init__(subnet_id=subnet_id, **kwargs)
+        super().__init__(**kwargs)
+        self.properties = properties
 
 
 class ClusterPoolVersion(ProxyResource):
     """Available cluster pool version.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
     :ivar id: Fully qualified resource ID for the resource. E.g.
-     "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{resourceType}/{resourceName}".
+     "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{resourceType}/{resourceName}".  # pylint: disable=line-too-long
     :vartype id: str
     :ivar name: The name of the resource.
     :vartype name: str
     :ivar type: The type of the resource. E.g. "Microsoft.Compute/virtualMachines" or
      "Microsoft.Storage/storageAccounts".
     :vartype type: str
     :ivar system_data: Azure Resource Manager metadata containing createdBy and modifiedBy
      information.
     :vartype system_data: ~azure.mgmt.hdinsightcontainers.models.SystemData
-    :ivar cluster_pool_version: Cluster pool version is a 2-part version.
-    :vartype cluster_pool_version: str
-    :ivar aks_version: AKS version.
-    :vartype aks_version: str
-    :ivar is_preview: Indicate if this version is in preview or not.
-    :vartype is_preview: bool
+    :ivar properties: Cluster pool version properties.
+    :vartype properties: ~azure.mgmt.hdinsightcontainers.models.ClusterPoolVersionProperties
     """
 
     _validation = {
         "id": {"readonly": True},
         "name": {"readonly": True},
         "type": {"readonly": True},
         "system_data": {"readonly": True},
-        "cluster_pool_version": {"pattern": r"^(0|[1-9][0-9]{0,18})\.(0|[1-9][0-9]{0,18})$"},
     }
 
     _attribute_map = {
         "id": {"key": "id", "type": "str"},
         "name": {"key": "name", "type": "str"},
         "type": {"key": "type", "type": "str"},
         "system_data": {"key": "systemData", "type": "SystemData"},
-        "cluster_pool_version": {"key": "properties.clusterPoolVersion", "type": "str"},
-        "aks_version": {"key": "properties.aksVersion", "type": "str"},
-        "is_preview": {"key": "properties.isPreview", "type": "bool"},
+        "properties": {"key": "properties", "type": "ClusterPoolVersionProperties"},
+    }
+
+    def __init__(self, *, properties: Optional["_models.ClusterPoolVersionProperties"] = None, **kwargs: Any) -> None:
+        """
+        :keyword properties: Cluster pool version properties.
+        :paramtype properties: ~azure.mgmt.hdinsightcontainers.models.ClusterPoolVersionProperties
+        """
+        super().__init__(**kwargs)
+        self.properties = properties
+
+
+class ClusterPoolVersionProperties(_serialization.Model):
+    """Cluster pool version properties.
+
+    :ivar cluster_pool_version: Cluster pool version is a 2-part version.
+    :vartype cluster_pool_version: str
+    :ivar aks_version: AKS version.
+    :vartype aks_version: str
+    :ivar is_preview: Indicate if this version is in preview or not.
+    :vartype is_preview: bool
+    """
+
+    _validation = {
+        "cluster_pool_version": {"pattern": r"^(0|[1-9][0-9]{0,18})\.(0|[1-9][0-9]{0,18})$"},
+    }
+
+    _attribute_map = {
+        "cluster_pool_version": {"key": "clusterPoolVersion", "type": "str"},
+        "aks_version": {"key": "aksVersion", "type": "str"},
+        "is_preview": {"key": "isPreview", "type": "bool"},
     }
 
     def __init__(
         self,
         *,
         cluster_pool_version: Optional[str] = None,
         aks_version: Optional[str] = None,
@@ -1666,55 +2303,63 @@
 
 
 class ClusterProfile(_serialization.Model):  # pylint: disable=too-many-instance-attributes
     """Cluster profile.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
-    All required parameters must be populated in order to send to Azure.
+    All required parameters must be populated in order to send to server.
 
     :ivar cluster_version: Version with 3/4 part. Required.
     :vartype cluster_version: str
     :ivar oss_version: Version with three part. Required.
     :vartype oss_version: str
     :ivar components: Component list of this cluster type and version.
     :vartype components: list[~azure.mgmt.hdinsightcontainers.models.ClusterComponentsItem]
-    :ivar identity_profile: Identity Profile with details of an MSI. Required.
+    :ivar identity_profile: This property is required by Trino, Spark and Flink cluster but is
+     optional for Kafka cluster.
     :vartype identity_profile: ~azure.mgmt.hdinsightcontainers.models.IdentityProfile
     :ivar authorization_profile: Authorization profile with details of AAD user Ids and group Ids
      authorized for data plane access. Required.
     :vartype authorization_profile: ~azure.mgmt.hdinsightcontainers.models.AuthorizationProfile
     :ivar secrets_profile: The cluster secret profile.
     :vartype secrets_profile: ~azure.mgmt.hdinsightcontainers.models.SecretsProfile
     :ivar service_configs_profiles: The service configs profiles.
     :vartype service_configs_profiles:
      list[~azure.mgmt.hdinsightcontainers.models.ClusterServiceConfigsProfile]
     :ivar connectivity_profile: Cluster connectivity profile.
     :vartype connectivity_profile: ~azure.mgmt.hdinsightcontainers.models.ConnectivityProfile
+    :ivar cluster_access_profile: Cluster access profile.
+    :vartype cluster_access_profile: ~azure.mgmt.hdinsightcontainers.models.ClusterAccessProfile
     :ivar log_analytics_profile: Cluster log analytics profile to enable or disable OMS agent for
      cluster.
     :vartype log_analytics_profile:
      ~azure.mgmt.hdinsightcontainers.models.ClusterLogAnalyticsProfile
     :ivar prometheus_profile: Cluster Prometheus profile.
     :vartype prometheus_profile: ~azure.mgmt.hdinsightcontainers.models.ClusterPrometheusProfile
     :ivar ssh_profile: Ssh profile for the cluster.
     :vartype ssh_profile: ~azure.mgmt.hdinsightcontainers.models.SshProfile
     :ivar autoscale_profile: This is the Autoscale profile for the cluster. This will allow
      customer to create cluster enabled with Autoscale.
     :vartype autoscale_profile: ~azure.mgmt.hdinsightcontainers.models.AutoscaleProfile
-    :ivar kafka_profile: Kafka cluster profile.
-    :vartype kafka_profile: dict[str, any]
+    :ivar ranger_plugin_profile: Cluster Ranger plugin profile.
+    :vartype ranger_plugin_profile:
+     ~azure.mgmt.hdinsightcontainers.models.ClusterRangerPluginProfile
+    :ivar kafka_profile: The Kafka cluster profile.
+    :vartype kafka_profile: ~azure.mgmt.hdinsightcontainers.models.KafkaProfile
     :ivar trino_profile: Trino Cluster profile.
     :vartype trino_profile: ~azure.mgmt.hdinsightcontainers.models.TrinoProfile
     :ivar llap_profile: LLAP cluster profile.
     :vartype llap_profile: dict[str, any]
     :ivar flink_profile: The Flink cluster profile.
     :vartype flink_profile: ~azure.mgmt.hdinsightcontainers.models.FlinkProfile
     :ivar spark_profile: The spark cluster profile.
     :vartype spark_profile: ~azure.mgmt.hdinsightcontainers.models.SparkProfile
+    :ivar ranger_profile: The ranger cluster profile.
+    :vartype ranger_profile: ~azure.mgmt.hdinsightcontainers.models.RangerProfile
     :ivar stub_profile: Stub cluster profile.
     :vartype stub_profile: dict[str, any]
     :ivar script_action_profiles: The script action profile list.
     :vartype script_action_profiles:
      list[~azure.mgmt.hdinsightcontainers.models.ScriptActionProfile]
     """
 
@@ -1724,99 +2369,112 @@
             "pattern": r"^(0|[1-9][0-9]{0,18})\.(0|[1-9][0-9]{0,18})\.(0|[1-9][0-9]{0,18})(?:\.(0|[1-9][0-9]{0,18}))?$",
         },
         "oss_version": {
             "required": True,
             "pattern": r"^(0|[1-9][0-9]{0,18})\.(0|[1-9][0-9]{0,18})\.(0|[1-9][0-9]{0,18})$",
         },
         "components": {"readonly": True},
-        "identity_profile": {"required": True},
         "authorization_profile": {"required": True},
         "connectivity_profile": {"readonly": True},
     }
 
     _attribute_map = {
         "cluster_version": {"key": "clusterVersion", "type": "str"},
         "oss_version": {"key": "ossVersion", "type": "str"},
         "components": {"key": "components", "type": "[ClusterComponentsItem]"},
         "identity_profile": {"key": "identityProfile", "type": "IdentityProfile"},
         "authorization_profile": {"key": "authorizationProfile", "type": "AuthorizationProfile"},
         "secrets_profile": {"key": "secretsProfile", "type": "SecretsProfile"},
         "service_configs_profiles": {"key": "serviceConfigsProfiles", "type": "[ClusterServiceConfigsProfile]"},
         "connectivity_profile": {"key": "connectivityProfile", "type": "ConnectivityProfile"},
+        "cluster_access_profile": {"key": "clusterAccessProfile", "type": "ClusterAccessProfile"},
         "log_analytics_profile": {"key": "logAnalyticsProfile", "type": "ClusterLogAnalyticsProfile"},
         "prometheus_profile": {"key": "prometheusProfile", "type": "ClusterPrometheusProfile"},
         "ssh_profile": {"key": "sshProfile", "type": "SshProfile"},
         "autoscale_profile": {"key": "autoscaleProfile", "type": "AutoscaleProfile"},
-        "kafka_profile": {"key": "kafkaProfile", "type": "{object}"},
+        "ranger_plugin_profile": {"key": "rangerPluginProfile", "type": "ClusterRangerPluginProfile"},
+        "kafka_profile": {"key": "kafkaProfile", "type": "KafkaProfile"},
         "trino_profile": {"key": "trinoProfile", "type": "TrinoProfile"},
         "llap_profile": {"key": "llapProfile", "type": "{object}"},
         "flink_profile": {"key": "flinkProfile", "type": "FlinkProfile"},
         "spark_profile": {"key": "sparkProfile", "type": "SparkProfile"},
+        "ranger_profile": {"key": "rangerProfile", "type": "RangerProfile"},
         "stub_profile": {"key": "stubProfile", "type": "{object}"},
         "script_action_profiles": {"key": "scriptActionProfiles", "type": "[ScriptActionProfile]"},
     }
 
     def __init__(
         self,
         *,
         cluster_version: str,
         oss_version: str,
-        identity_profile: "_models.IdentityProfile",
         authorization_profile: "_models.AuthorizationProfile",
+        identity_profile: Optional["_models.IdentityProfile"] = None,
         secrets_profile: Optional["_models.SecretsProfile"] = None,
         service_configs_profiles: Optional[List["_models.ClusterServiceConfigsProfile"]] = None,
+        cluster_access_profile: Optional["_models.ClusterAccessProfile"] = None,
         log_analytics_profile: Optional["_models.ClusterLogAnalyticsProfile"] = None,
         prometheus_profile: Optional["_models.ClusterPrometheusProfile"] = None,
         ssh_profile: Optional["_models.SshProfile"] = None,
         autoscale_profile: Optional["_models.AutoscaleProfile"] = None,
-        kafka_profile: Optional[Dict[str, Any]] = None,
+        ranger_plugin_profile: Optional["_models.ClusterRangerPluginProfile"] = None,
+        kafka_profile: Optional["_models.KafkaProfile"] = None,
         trino_profile: Optional["_models.TrinoProfile"] = None,
         llap_profile: Optional[Dict[str, Any]] = None,
         flink_profile: Optional["_models.FlinkProfile"] = None,
         spark_profile: Optional["_models.SparkProfile"] = None,
+        ranger_profile: Optional["_models.RangerProfile"] = None,
         stub_profile: Optional[Dict[str, Any]] = None,
         script_action_profiles: Optional[List["_models.ScriptActionProfile"]] = None,
         **kwargs: Any
     ) -> None:
         """
         :keyword cluster_version: Version with 3/4 part. Required.
         :paramtype cluster_version: str
         :keyword oss_version: Version with three part. Required.
         :paramtype oss_version: str
-        :keyword identity_profile: Identity Profile with details of an MSI. Required.
+        :keyword identity_profile: This property is required by Trino, Spark and Flink cluster but is
+         optional for Kafka cluster.
         :paramtype identity_profile: ~azure.mgmt.hdinsightcontainers.models.IdentityProfile
         :keyword authorization_profile: Authorization profile with details of AAD user Ids and group
          Ids authorized for data plane access. Required.
         :paramtype authorization_profile: ~azure.mgmt.hdinsightcontainers.models.AuthorizationProfile
         :keyword secrets_profile: The cluster secret profile.
         :paramtype secrets_profile: ~azure.mgmt.hdinsightcontainers.models.SecretsProfile
         :keyword service_configs_profiles: The service configs profiles.
         :paramtype service_configs_profiles:
          list[~azure.mgmt.hdinsightcontainers.models.ClusterServiceConfigsProfile]
+        :keyword cluster_access_profile: Cluster access profile.
+        :paramtype cluster_access_profile: ~azure.mgmt.hdinsightcontainers.models.ClusterAccessProfile
         :keyword log_analytics_profile: Cluster log analytics profile to enable or disable OMS agent
          for cluster.
         :paramtype log_analytics_profile:
          ~azure.mgmt.hdinsightcontainers.models.ClusterLogAnalyticsProfile
         :keyword prometheus_profile: Cluster Prometheus profile.
         :paramtype prometheus_profile: ~azure.mgmt.hdinsightcontainers.models.ClusterPrometheusProfile
         :keyword ssh_profile: Ssh profile for the cluster.
         :paramtype ssh_profile: ~azure.mgmt.hdinsightcontainers.models.SshProfile
         :keyword autoscale_profile: This is the Autoscale profile for the cluster. This will allow
          customer to create cluster enabled with Autoscale.
         :paramtype autoscale_profile: ~azure.mgmt.hdinsightcontainers.models.AutoscaleProfile
-        :keyword kafka_profile: Kafka cluster profile.
-        :paramtype kafka_profile: dict[str, any]
+        :keyword ranger_plugin_profile: Cluster Ranger plugin profile.
+        :paramtype ranger_plugin_profile:
+         ~azure.mgmt.hdinsightcontainers.models.ClusterRangerPluginProfile
+        :keyword kafka_profile: The Kafka cluster profile.
+        :paramtype kafka_profile: ~azure.mgmt.hdinsightcontainers.models.KafkaProfile
         :keyword trino_profile: Trino Cluster profile.
         :paramtype trino_profile: ~azure.mgmt.hdinsightcontainers.models.TrinoProfile
         :keyword llap_profile: LLAP cluster profile.
         :paramtype llap_profile: dict[str, any]
         :keyword flink_profile: The Flink cluster profile.
         :paramtype flink_profile: ~azure.mgmt.hdinsightcontainers.models.FlinkProfile
         :keyword spark_profile: The spark cluster profile.
         :paramtype spark_profile: ~azure.mgmt.hdinsightcontainers.models.SparkProfile
+        :keyword ranger_profile: The ranger cluster profile.
+        :paramtype ranger_profile: ~azure.mgmt.hdinsightcontainers.models.RangerProfile
         :keyword stub_profile: Stub cluster profile.
         :paramtype stub_profile: dict[str, any]
         :keyword script_action_profiles: The script action profile list.
         :paramtype script_action_profiles:
          list[~azure.mgmt.hdinsightcontainers.models.ScriptActionProfile]
         """
         super().__init__(**kwargs)
@@ -1824,31 +2482,34 @@
         self.oss_version = oss_version
         self.components = None
         self.identity_profile = identity_profile
         self.authorization_profile = authorization_profile
         self.secrets_profile = secrets_profile
         self.service_configs_profiles = service_configs_profiles
         self.connectivity_profile = None
+        self.cluster_access_profile = cluster_access_profile
         self.log_analytics_profile = log_analytics_profile
         self.prometheus_profile = prometheus_profile
         self.ssh_profile = ssh_profile
         self.autoscale_profile = autoscale_profile
+        self.ranger_plugin_profile = ranger_plugin_profile
         self.kafka_profile = kafka_profile
         self.trino_profile = trino_profile
         self.llap_profile = llap_profile
         self.flink_profile = flink_profile
         self.spark_profile = spark_profile
+        self.ranger_profile = ranger_profile
         self.stub_profile = stub_profile
         self.script_action_profiles = script_action_profiles
 
 
 class ClusterPrometheusProfile(_serialization.Model):
     """Cluster Prometheus profile.
 
-    All required parameters must be populated in order to send to Azure.
+    All required parameters must be populated in order to send to server.
 
     :ivar enabled: Enable Prometheus for cluster or not. Required.
     :vartype enabled: bool
     """
 
     _validation = {
         "enabled": {"required": True},
@@ -1863,38 +2524,64 @@
         :keyword enabled: Enable Prometheus for cluster or not. Required.
         :paramtype enabled: bool
         """
         super().__init__(**kwargs)
         self.enabled = enabled
 
 
+class ClusterRangerPluginProfile(_serialization.Model):
+    """Cluster Ranger plugin profile.
+
+    All required parameters must be populated in order to send to server.
+
+    :ivar enabled: Enable Ranger for cluster or not. Required.
+    :vartype enabled: bool
+    """
+
+    _validation = {
+        "enabled": {"required": True},
+    }
+
+    _attribute_map = {
+        "enabled": {"key": "enabled", "type": "bool"},
+    }
+
+    def __init__(self, *, enabled: bool = False, **kwargs: Any) -> None:
+        """
+        :keyword enabled: Enable Ranger for cluster or not. Required.
+        :paramtype enabled: bool
+        """
+        super().__init__(**kwargs)
+        self.enabled = enabled
+
+
 class ClusterResizeData(TrackedResource):
     """The parameters for resizing a cluster.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
-    All required parameters must be populated in order to send to Azure.
+    All required parameters must be populated in order to send to server.
 
     :ivar id: Fully qualified resource ID for the resource. E.g.
-     "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{resourceType}/{resourceName}".
+     "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{resourceType}/{resourceName}".  # pylint: disable=line-too-long
     :vartype id: str
     :ivar name: The name of the resource.
     :vartype name: str
     :ivar type: The type of the resource. E.g. "Microsoft.Compute/virtualMachines" or
      "Microsoft.Storage/storageAccounts".
     :vartype type: str
     :ivar system_data: Azure Resource Manager metadata containing createdBy and modifiedBy
      information.
     :vartype system_data: ~azure.mgmt.hdinsightcontainers.models.SystemData
     :ivar tags: Resource tags.
     :vartype tags: dict[str, str]
     :ivar location: The geo-location where the resource lives. Required.
     :vartype location: str
-    :ivar target_worker_node_count: Target node count of worker node.
-    :vartype target_worker_node_count: int
+    :ivar properties: Sets the properties. Define cluster resize specific properties.
+    :vartype properties: ~azure.mgmt.hdinsightcontainers.models.ClusterResizeProperties
     """
 
     _validation = {
         "id": {"readonly": True},
         "name": {"readonly": True},
         "type": {"readonly": True},
         "system_data": {"readonly": True},
@@ -1904,41 +2591,132 @@
     _attribute_map = {
         "id": {"key": "id", "type": "str"},
         "name": {"key": "name", "type": "str"},
         "type": {"key": "type", "type": "str"},
         "system_data": {"key": "systemData", "type": "SystemData"},
         "tags": {"key": "tags", "type": "{str}"},
         "location": {"key": "location", "type": "str"},
-        "target_worker_node_count": {"key": "properties.targetWorkerNodeCount", "type": "int"},
+        "properties": {"key": "properties", "type": "ClusterResizeProperties"},
     }
 
     def __init__(
         self,
         *,
         location: str,
         tags: Optional[Dict[str, str]] = None,
-        target_worker_node_count: Optional[int] = None,
+        properties: Optional["_models.ClusterResizeProperties"] = None,
         **kwargs: Any
     ) -> None:
         """
         :keyword tags: Resource tags.
         :paramtype tags: dict[str, str]
         :keyword location: The geo-location where the resource lives. Required.
         :paramtype location: str
-        :keyword target_worker_node_count: Target node count of worker node.
-        :paramtype target_worker_node_count: int
+        :keyword properties: Sets the properties. Define cluster resize specific properties.
+        :paramtype properties: ~azure.mgmt.hdinsightcontainers.models.ClusterResizeProperties
         """
         super().__init__(tags=tags, location=location, **kwargs)
+        self.properties = properties
+
+
+class ClusterResizeProperties(_serialization.Model):
+    """The properties for resizing a cluster.
+
+    All required parameters must be populated in order to send to server.
+
+    :ivar target_worker_node_count: Target node count of worker node. Required.
+    :vartype target_worker_node_count: int
+    """
+
+    _validation = {
+        "target_worker_node_count": {"required": True},
+    }
+
+    _attribute_map = {
+        "target_worker_node_count": {"key": "targetWorkerNodeCount", "type": "int"},
+    }
+
+    def __init__(self, *, target_worker_node_count: int, **kwargs: Any) -> None:
+        """
+        :keyword target_worker_node_count: Target node count of worker node. Required.
+        :paramtype target_worker_node_count: int
+        """
+        super().__init__(**kwargs)
         self.target_worker_node_count = target_worker_node_count
 
 
+class ClusterResourceProperties(_serialization.Model):
+    """Cluster resource properties.
+
+    Variables are only populated by the server, and will be ignored when sending a request.
+
+    All required parameters must be populated in order to send to server.
+
+    :ivar provisioning_state: Provisioning state of the resource. Known values are: "Accepted",
+     "Succeeded", "Canceled", and "Failed".
+    :vartype provisioning_state: str or ~azure.mgmt.hdinsightcontainers.models.ProvisioningStatus
+    :ivar cluster_type: The type of cluster. Required.
+    :vartype cluster_type: str
+    :ivar deployment_id: A unique id generated by the RP to identify the resource.
+    :vartype deployment_id: str
+    :ivar compute_profile: The compute profile. Required.
+    :vartype compute_profile: ~azure.mgmt.hdinsightcontainers.models.ComputeProfile
+    :ivar cluster_profile: Cluster profile. Required.
+    :vartype cluster_profile: ~azure.mgmt.hdinsightcontainers.models.ClusterProfile
+    :ivar status: Business status of the resource.
+    :vartype status: str
+    """
+
+    _validation = {
+        "provisioning_state": {"readonly": True},
+        "cluster_type": {"required": True, "pattern": r"^[a-zA-Z][a-zA-Z0-9]{0,31}$"},
+        "deployment_id": {"readonly": True},
+        "compute_profile": {"required": True},
+        "cluster_profile": {"required": True},
+        "status": {"readonly": True},
+    }
+
+    _attribute_map = {
+        "provisioning_state": {"key": "provisioningState", "type": "str"},
+        "cluster_type": {"key": "clusterType", "type": "str"},
+        "deployment_id": {"key": "deploymentId", "type": "str"},
+        "compute_profile": {"key": "computeProfile", "type": "ComputeProfile"},
+        "cluster_profile": {"key": "clusterProfile", "type": "ClusterProfile"},
+        "status": {"key": "status", "type": "str"},
+    }
+
+    def __init__(
+        self,
+        *,
+        cluster_type: str,
+        compute_profile: "_models.ComputeProfile",
+        cluster_profile: "_models.ClusterProfile",
+        **kwargs: Any
+    ) -> None:
+        """
+        :keyword cluster_type: The type of cluster. Required.
+        :paramtype cluster_type: str
+        :keyword compute_profile: The compute profile. Required.
+        :paramtype compute_profile: ~azure.mgmt.hdinsightcontainers.models.ComputeProfile
+        :keyword cluster_profile: Cluster profile. Required.
+        :paramtype cluster_profile: ~azure.mgmt.hdinsightcontainers.models.ClusterProfile
+        """
+        super().__init__(**kwargs)
+        self.provisioning_state = None
+        self.cluster_type = cluster_type
+        self.deployment_id = None
+        self.compute_profile = compute_profile
+        self.cluster_profile = cluster_profile
+        self.status = None
+
+
 class ClusterServiceConfig(_serialization.Model):
     """Cluster configs per component.
 
-    All required parameters must be populated in order to send to Azure.
+    All required parameters must be populated in order to send to server.
 
     :ivar component: Name of the component the config files should apply to. Required.
     :vartype component: str
     :ivar files: List of Config Files. Required.
     :vartype files: list[~azure.mgmt.hdinsightcontainers.models.ClusterConfigFile]
     """
 
@@ -1963,15 +2741,15 @@
         self.component = component
         self.files = files
 
 
 class ClusterServiceConfigsProfile(_serialization.Model):
     """Cluster service configs.
 
-    All required parameters must be populated in order to send to Azure.
+    All required parameters must be populated in order to send to server.
 
     :ivar service_name: Name of the service the configurations should apply to. Required.
     :vartype service_name: str
     :ivar configs: List of service configs. Required.
     :vartype configs: list[~azure.mgmt.hdinsightcontainers.models.ClusterServiceConfig]
     """
 
@@ -1993,30 +2771,89 @@
         :paramtype configs: list[~azure.mgmt.hdinsightcontainers.models.ClusterServiceConfig]
         """
         super().__init__(**kwargs)
         self.service_name = service_name
         self.configs = configs
 
 
+class ClusterUpgrade(_serialization.Model):
+    """Cluster Upgrade.
+
+    All required parameters must be populated in order to send to server.
+
+    :ivar properties: Properties of upgrading cluster. Required.
+    :vartype properties: ~azure.mgmt.hdinsightcontainers.models.ClusterUpgradeProperties
+    """
+
+    _validation = {
+        "properties": {"required": True},
+    }
+
+    _attribute_map = {
+        "properties": {"key": "properties", "type": "ClusterUpgradeProperties"},
+    }
+
+    def __init__(self, *, properties: "_models.ClusterUpgradeProperties", **kwargs: Any) -> None:
+        """
+        :keyword properties: Properties of upgrading cluster. Required.
+        :paramtype properties: ~azure.mgmt.hdinsightcontainers.models.ClusterUpgradeProperties
+        """
+        super().__init__(**kwargs)
+        self.properties = properties
+
+
 class ClusterVersion(ProxyResource):
     """Available cluster version.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
     :ivar id: Fully qualified resource ID for the resource. E.g.
-     "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{resourceType}/{resourceName}".
+     "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{resourceType}/{resourceName}".  # pylint: disable=line-too-long
     :vartype id: str
     :ivar name: The name of the resource.
     :vartype name: str
     :ivar type: The type of the resource. E.g. "Microsoft.Compute/virtualMachines" or
      "Microsoft.Storage/storageAccounts".
     :vartype type: str
     :ivar system_data: Azure Resource Manager metadata containing createdBy and modifiedBy
      information.
     :vartype system_data: ~azure.mgmt.hdinsightcontainers.models.SystemData
+    :ivar properties: Cluster version properties.
+    :vartype properties: ~azure.mgmt.hdinsightcontainers.models.ClusterVersionProperties
+    """
+
+    _validation = {
+        "id": {"readonly": True},
+        "name": {"readonly": True},
+        "type": {"readonly": True},
+        "system_data": {"readonly": True},
+    }
+
+    _attribute_map = {
+        "id": {"key": "id", "type": "str"},
+        "name": {"key": "name", "type": "str"},
+        "type": {"key": "type", "type": "str"},
+        "system_data": {"key": "systemData", "type": "SystemData"},
+        "properties": {"key": "properties", "type": "ClusterVersionProperties"},
+    }
+
+    def __init__(self, *, properties: Optional["_models.ClusterVersionProperties"] = None, **kwargs: Any) -> None:
+        """
+        :keyword properties: Cluster version properties.
+        :paramtype properties: ~azure.mgmt.hdinsightcontainers.models.ClusterVersionProperties
+        """
+        super().__init__(**kwargs)
+        self.properties = properties
+
+
+class ClusterVersionProperties(_serialization.Model):
+    """Cluster version properties.
+
+    Variables are only populated by the server, and will be ignored when sending a request.
+
     :ivar cluster_type: The type of cluster.
     :vartype cluster_type: str
     :ivar cluster_version: Version with three part.
     :vartype cluster_version: str
     :ivar oss_version: Version with three part.
     :vartype oss_version: str
     :ivar cluster_pool_version: The two part cluster pool version. If the cluster version is before
@@ -2025,35 +2862,27 @@
     :ivar is_preview: Indicate if this version is in preview or not.
     :vartype is_preview: bool
     :ivar components: Component list of this cluster type and version.
     :vartype components: list[~azure.mgmt.hdinsightcontainers.models.ClusterComponentsItem]
     """
 
     _validation = {
-        "id": {"readonly": True},
-        "name": {"readonly": True},
-        "type": {"readonly": True},
-        "system_data": {"readonly": True},
         "cluster_type": {"pattern": r"^[a-zA-Z][a-zA-Z0-9]{0,31}$"},
         "cluster_version": {"pattern": r"^(0|[1-9][0-9]{0,18})\.(0|[1-9][0-9]{0,18})\.(0|[1-9][0-9]{0,18})$"},
         "oss_version": {"pattern": r"^(0|[1-9][0-9]{0,18})\.(0|[1-9][0-9]{0,18})\.(0|[1-9][0-9]{0,18})$"},
         "components": {"readonly": True},
     }
 
     _attribute_map = {
-        "id": {"key": "id", "type": "str"},
-        "name": {"key": "name", "type": "str"},
-        "type": {"key": "type", "type": "str"},
-        "system_data": {"key": "systemData", "type": "SystemData"},
-        "cluster_type": {"key": "properties.clusterType", "type": "str"},
-        "cluster_version": {"key": "properties.clusterVersion", "type": "str"},
-        "oss_version": {"key": "properties.ossVersion", "type": "str"},
-        "cluster_pool_version": {"key": "properties.clusterPoolVersion", "type": "str"},
-        "is_preview": {"key": "properties.isPreview", "type": "bool"},
-        "components": {"key": "properties.components", "type": "[ClusterComponentsItem]"},
+        "cluster_type": {"key": "clusterType", "type": "str"},
+        "cluster_version": {"key": "clusterVersion", "type": "str"},
+        "oss_version": {"key": "ossVersion", "type": "str"},
+        "cluster_pool_version": {"key": "clusterPoolVersion", "type": "str"},
+        "is_preview": {"key": "isPreview", "type": "bool"},
+        "components": {"key": "components", "type": "[ClusterComponentsItem]"},
     }
 
     def __init__(
         self,
         *,
         cluster_type: Optional[str] = None,
         cluster_version: Optional[str] = None,
@@ -2113,15 +2942,15 @@
         self.value = value
         self.next_link = None
 
 
 class ComparisonRule(_serialization.Model):
     """The comparison rule.
 
-    All required parameters must be populated in order to send to Azure.
+    All required parameters must be populated in order to send to server.
 
     :ivar operator: The comparison operator. Required. Known values are: "greaterThan",
      "greaterThanOrEqual", "lessThan", and "lessThanOrEqual".
     :vartype operator: str or ~azure.mgmt.hdinsightcontainers.models.ComparisonOperator
     :ivar threshold: Threshold setting. Required.
     :vartype threshold: float
     """
@@ -2148,15 +2977,15 @@
         self.operator = operator
         self.threshold = threshold
 
 
 class ComputeProfile(_serialization.Model):
     """The compute profile.
 
-    All required parameters must be populated in order to send to Azure.
+    All required parameters must be populated in order to send to server.
 
     :ivar nodes: The nodes definitions. Required.
     :vartype nodes: list[~azure.mgmt.hdinsightcontainers.models.NodeProfile]
     """
 
     _validation = {
         "nodes": {"required": True},
@@ -2174,15 +3003,15 @@
         super().__init__(**kwargs)
         self.nodes = nodes
 
 
 class ComputeResourceDefinition(_serialization.Model):
     """The cpu and memory requirement definition.
 
-    All required parameters must be populated in order to send to Azure.
+    All required parameters must be populated in order to send to server.
 
     :ivar cpu: The required CPU. Required.
     :vartype cpu: float
     :ivar memory: The required memory in MB, Container memory will be 110 percentile. Required.
     :vartype memory: int
     """
 
@@ -2207,15 +3036,15 @@
         self.cpu = cpu
         self.memory = memory
 
 
 class ConnectivityProfile(_serialization.Model):
     """Cluster connectivity profile.
 
-    All required parameters must be populated in order to send to Azure.
+    All required parameters must be populated in order to send to server.
 
     :ivar web: Web connectivity endpoint details. Required.
     :vartype web: ~azure.mgmt.hdinsightcontainers.models.ConnectivityProfileWeb
     :ivar ssh: List of SSH connectivity endpoints.
     :vartype ssh: list[~azure.mgmt.hdinsightcontainers.models.SshConnectivityEndpoint]
     """
 
@@ -2245,60 +3074,97 @@
         self.web = web
         self.ssh = ssh
 
 
 class WebConnectivityEndpoint(_serialization.Model):
     """Web connectivity endpoint details.
 
-    All required parameters must be populated in order to send to Azure.
+    All required parameters must be populated in order to send to server.
 
     :ivar fqdn: Web connectivity endpoint. Required.
     :vartype fqdn: str
+    :ivar private_fqdn: Private web connectivity endpoint. This property will only be returned when
+     enableInternalIngress is true.
+    :vartype private_fqdn: str
     """
 
     _validation = {
         "fqdn": {"required": True},
     }
 
     _attribute_map = {
         "fqdn": {"key": "fqdn", "type": "str"},
+        "private_fqdn": {"key": "privateFqdn", "type": "str"},
     }
 
-    def __init__(self, *, fqdn: str, **kwargs: Any) -> None:
+    def __init__(self, *, fqdn: str, private_fqdn: Optional[str] = None, **kwargs: Any) -> None:
         """
         :keyword fqdn: Web connectivity endpoint. Required.
         :paramtype fqdn: str
+        :keyword private_fqdn: Private web connectivity endpoint. This property will only be returned
+         when enableInternalIngress is true.
+        :paramtype private_fqdn: str
         """
         super().__init__(**kwargs)
         self.fqdn = fqdn
+        self.private_fqdn = private_fqdn
 
 
 class ConnectivityProfileWeb(WebConnectivityEndpoint):
     """Web connectivity endpoint details.
 
-    All required parameters must be populated in order to send to Azure.
+    All required parameters must be populated in order to send to server.
 
     :ivar fqdn: Web connectivity endpoint. Required.
     :vartype fqdn: str
+    :ivar private_fqdn: Private web connectivity endpoint. This property will only be returned when
+     enableInternalIngress is true.
+    :vartype private_fqdn: str
+    """
+
+
+class DiskStorageProfile(_serialization.Model):
+    """Kafka disk storage profile.
+
+    All required parameters must be populated in order to send to server.
+
+    :ivar data_disk_size: Managed Disk size in GB. The maximum supported disk size for Standard and
+     Premium HDD/SSD is 32TB, except for Premium SSD v2, which supports up to 64TB. Required.
+    :vartype data_disk_size: int
+    :ivar data_disk_type: Managed Disk Type. Required. Known values are: "Standard_HDD_LRS",
+     "Standard_SSD_LRS", "Standard_SSD_ZRS", "Premium_SSD_LRS", "Premium_SSD_ZRS", and
+     "Premium_SSD_v2_LRS".
+    :vartype data_disk_type: str or ~azure.mgmt.hdinsightcontainers.models.DataDiskType
     """
 
     _validation = {
-        "fqdn": {"required": True},
+        "data_disk_size": {"required": True},
+        "data_disk_type": {"required": True},
     }
 
     _attribute_map = {
-        "fqdn": {"key": "fqdn", "type": "str"},
+        "data_disk_size": {"key": "dataDiskSize", "type": "int"},
+        "data_disk_type": {"key": "dataDiskType", "type": "str"},
     }
 
-    def __init__(self, *, fqdn: str, **kwargs: Any) -> None:
+    def __init__(
+        self, *, data_disk_size: int, data_disk_type: Union[str, "_models.DataDiskType"], **kwargs: Any
+    ) -> None:
         """
-        :keyword fqdn: Web connectivity endpoint. Required.
-        :paramtype fqdn: str
+        :keyword data_disk_size: Managed Disk size in GB. The maximum supported disk size for Standard
+         and Premium HDD/SSD is 32TB, except for Premium SSD v2, which supports up to 64TB. Required.
+        :paramtype data_disk_size: int
+        :keyword data_disk_type: Managed Disk Type. Required. Known values are: "Standard_HDD_LRS",
+         "Standard_SSD_LRS", "Standard_SSD_ZRS", "Premium_SSD_LRS", "Premium_SSD_ZRS", and
+         "Premium_SSD_v2_LRS".
+        :paramtype data_disk_type: str or ~azure.mgmt.hdinsightcontainers.models.DataDiskType
         """
-        super().__init__(fqdn=fqdn, **kwargs)
+        super().__init__(**kwargs)
+        self.data_disk_size = data_disk_size
+        self.data_disk_type = data_disk_type
 
 
 class ErrorAdditionalInfo(_serialization.Model):
     """The resource management error additional info.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
@@ -2408,70 +3274,174 @@
         super().__init__(**kwargs)
         self.hive = hive
 
 
 class FlinkHiveCatalogOption(_serialization.Model):
     """Hive Catalog Option for Flink cluster.
 
-    All required parameters must be populated in order to send to Azure.
+    All required parameters must be populated in order to send to server.
 
+    :ivar metastore_db_connection_authentication_mode: The authentication mode to connect to your
+     Hive metastore database. More details:
+     https://learn.microsoft.com/en-us/azure/azure-sql/database/logins-create-manage?view=azuresql#authentication-and-authorization.  # pylint: disable=line-too-long
+     Known values are: "SqlAuth" and "IdentityAuth".
+    :vartype metastore_db_connection_authentication_mode: str or
+     ~azure.mgmt.hdinsightcontainers.models.MetastoreDbConnectionAuthenticationMode
     :ivar metastore_db_connection_password_secret: Secret reference name from
-     secretsProfile.secrets containing password for database connection. Required.
+     secretsProfile.secrets containing password for database connection.
     :vartype metastore_db_connection_password_secret: str
     :ivar metastore_db_connection_url: Connection string for hive metastore database. Required.
     :vartype metastore_db_connection_url: str
-    :ivar metastore_db_connection_user_name: User name for database connection. Required.
+    :ivar metastore_db_connection_user_name: User name for database connection.
     :vartype metastore_db_connection_user_name: str
     """
 
     _validation = {
-        "metastore_db_connection_password_secret": {"required": True},
         "metastore_db_connection_url": {"required": True},
-        "metastore_db_connection_user_name": {"required": True},
     }
 
     _attribute_map = {
+        "metastore_db_connection_authentication_mode": {
+            "key": "metastoreDbConnectionAuthenticationMode",
+            "type": "str",
+        },
         "metastore_db_connection_password_secret": {"key": "metastoreDbConnectionPasswordSecret", "type": "str"},
         "metastore_db_connection_url": {"key": "metastoreDbConnectionURL", "type": "str"},
         "metastore_db_connection_user_name": {"key": "metastoreDbConnectionUserName", "type": "str"},
     }
 
     def __init__(
         self,
         *,
-        metastore_db_connection_password_secret: str,
         metastore_db_connection_url: str,
-        metastore_db_connection_user_name: str,
+        metastore_db_connection_authentication_mode: Optional[
+            Union[str, "_models.MetastoreDbConnectionAuthenticationMode"]
+        ] = None,
+        metastore_db_connection_password_secret: Optional[str] = None,
+        metastore_db_connection_user_name: Optional[str] = None,
         **kwargs: Any
     ) -> None:
         """
+        :keyword metastore_db_connection_authentication_mode: The authentication mode to connect to
+         your Hive metastore database. More details:
+         https://learn.microsoft.com/en-us/azure/azure-sql/database/logins-create-manage?view=azuresql#authentication-and-authorization.  # pylint: disable=line-too-long
+         Known values are: "SqlAuth" and "IdentityAuth".
+        :paramtype metastore_db_connection_authentication_mode: str or
+         ~azure.mgmt.hdinsightcontainers.models.MetastoreDbConnectionAuthenticationMode
         :keyword metastore_db_connection_password_secret: Secret reference name from
-         secretsProfile.secrets containing password for database connection. Required.
+         secretsProfile.secrets containing password for database connection.
         :paramtype metastore_db_connection_password_secret: str
         :keyword metastore_db_connection_url: Connection string for hive metastore database. Required.
         :paramtype metastore_db_connection_url: str
-        :keyword metastore_db_connection_user_name: User name for database connection. Required.
+        :keyword metastore_db_connection_user_name: User name for database connection.
         :paramtype metastore_db_connection_user_name: str
         """
         super().__init__(**kwargs)
+        self.metastore_db_connection_authentication_mode = metastore_db_connection_authentication_mode
         self.metastore_db_connection_password_secret = metastore_db_connection_password_secret
         self.metastore_db_connection_url = metastore_db_connection_url
         self.metastore_db_connection_user_name = metastore_db_connection_user_name
 
 
+class FlinkJobProfile(_serialization.Model):
+    """Job specifications for flink clusters in application deployment mode. The specification is
+    immutable even if job properties are changed by calling the RunJob API, please use the ListJob
+    API to get the latest job information.
+
+    All required parameters must be populated in order to send to server.
+
+    :ivar job_jar_directory: A string property that specifies the directory where the job JAR is
+     located. Required.
+    :vartype job_jar_directory: str
+    :ivar jar_name: A string property that represents the name of the job JAR. Required.
+    :vartype jar_name: str
+    :ivar entry_class: A string property that specifies the entry class for the Flink job. If not
+     specified, the entry point is auto-detected from the flink job jar package.
+    :vartype entry_class: str
+    :ivar args: A string property representing additional JVM arguments for the Flink job. It
+     should be space separated value.
+    :vartype args: str
+    :ivar save_point_name: A string property that represents the name of the savepoint for the
+     Flink job.
+    :vartype save_point_name: str
+    :ivar upgrade_mode: A string property that indicates the upgrade mode to be performed on the
+     Flink job. It can have one of the following enum values => STATELESS_UPDATE, UPDATE,
+     LAST_STATE_UPDATE. Required. Known values are: "STATELESS_UPDATE", "UPDATE", and
+     "LAST_STATE_UPDATE".
+    :vartype upgrade_mode: str or ~azure.mgmt.hdinsightcontainers.models.UpgradeMode
+    """
+
+    _validation = {
+        "job_jar_directory": {"required": True},
+        "jar_name": {"required": True},
+        "upgrade_mode": {"required": True},
+    }
+
+    _attribute_map = {
+        "job_jar_directory": {"key": "jobJarDirectory", "type": "str"},
+        "jar_name": {"key": "jarName", "type": "str"},
+        "entry_class": {"key": "entryClass", "type": "str"},
+        "args": {"key": "args", "type": "str"},
+        "save_point_name": {"key": "savePointName", "type": "str"},
+        "upgrade_mode": {"key": "upgradeMode", "type": "str"},
+    }
+
+    def __init__(
+        self,
+        *,
+        job_jar_directory: str,
+        jar_name: str,
+        upgrade_mode: Union[str, "_models.UpgradeMode"],
+        entry_class: Optional[str] = None,
+        args: Optional[str] = None,
+        save_point_name: Optional[str] = None,
+        **kwargs: Any
+    ) -> None:
+        """
+        :keyword job_jar_directory: A string property that specifies the directory where the job JAR is
+         located. Required.
+        :paramtype job_jar_directory: str
+        :keyword jar_name: A string property that represents the name of the job JAR. Required.
+        :paramtype jar_name: str
+        :keyword entry_class: A string property that specifies the entry class for the Flink job. If
+         not specified, the entry point is auto-detected from the flink job jar package.
+        :paramtype entry_class: str
+        :keyword args: A string property representing additional JVM arguments for the Flink job. It
+         should be space separated value.
+        :paramtype args: str
+        :keyword save_point_name: A string property that represents the name of the savepoint for the
+         Flink job.
+        :paramtype save_point_name: str
+        :keyword upgrade_mode: A string property that indicates the upgrade mode to be performed on the
+         Flink job. It can have one of the following enum values => STATELESS_UPDATE, UPDATE,
+         LAST_STATE_UPDATE. Required. Known values are: "STATELESS_UPDATE", "UPDATE", and
+         "LAST_STATE_UPDATE".
+        :paramtype upgrade_mode: str or ~azure.mgmt.hdinsightcontainers.models.UpgradeMode
+        """
+        super().__init__(**kwargs)
+        self.job_jar_directory = job_jar_directory
+        self.jar_name = jar_name
+        self.entry_class = entry_class
+        self.args = args
+        self.save_point_name = save_point_name
+        self.upgrade_mode = upgrade_mode
+
+
 class FlinkJobProperties(ClusterJobProperties):  # pylint: disable=too-many-instance-attributes
     """Properties of flink job.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
-    All required parameters must be populated in order to send to Azure.
+    All required parameters must be populated in order to send to server.
 
     :ivar job_type: Type of cluster job. Required. "FlinkJob"
     :vartype job_type: str or ~azure.mgmt.hdinsightcontainers.models.JobType
-    :ivar job_name: Name of job. Required.
+    :ivar run_id: Run id of job.
+    :vartype run_id: str
+    :ivar job_name: Name of job.
     :vartype job_name: str
     :ivar job_jar_directory: A string property that specifies the directory where the job JAR is
      located.
     :vartype job_jar_directory: str
     :ivar jar_name: A string property that represents the name of the job JAR.
     :vartype jar_name: str
     :ivar entry_class: A string property that specifies the entry class for the Flink job.
@@ -2481,15 +3451,16 @@
     :vartype args: str
     :ivar save_point_name: A string property that represents the name of the savepoint for the
      Flink job.
     :vartype save_point_name: str
     :ivar action: A string property that indicates the action to be performed on the Flink job. It
      can have one of the following enum values => NEW, UPDATE, STATELESS_UPDATE, STOP, START,
      CANCEL, SAVEPOINT, LIST_SAVEPOINT, or DELETE. Known values are: "NEW", "UPDATE",
-     "STATELESS_UPDATE", "STOP", "START", "CANCEL", "SAVEPOINT", "LIST_SAVEPOINT", and "DELETE".
+     "STATELESS_UPDATE", "STOP", "START", "CANCEL", "SAVEPOINT", "LIST_SAVEPOINT", "DELETE",
+     "LAST_STATE_UPDATE", and "RE_LAUNCH".
     :vartype action: str or ~azure.mgmt.hdinsightcontainers.models.Action
     :ivar flink_configuration: Additional properties used to configure Flink jobs. It allows users
      to set properties such as parallelism and jobSavePointDirectory. It accepts additional
      key-value pairs as properties, where the keys are strings and the values are strings as well.
     :vartype flink_configuration: dict[str, str]
     :ivar job_id: Unique id for identifying a job.
     :vartype job_id: str
@@ -2501,24 +3472,24 @@
     :vartype action_result: str
     :ivar last_save_point: The last savepoint.
     :vartype last_save_point: str
     """
 
     _validation = {
         "job_type": {"required": True},
-        "job_name": {"required": True},
         "job_id": {"readonly": True},
         "status": {"readonly": True},
         "job_output": {"readonly": True},
         "action_result": {"readonly": True},
         "last_save_point": {"readonly": True},
     }
 
     _attribute_map = {
         "job_type": {"key": "jobType", "type": "str"},
+        "run_id": {"key": "runId", "type": "str"},
         "job_name": {"key": "jobName", "type": "str"},
         "job_jar_directory": {"key": "jobJarDirectory", "type": "str"},
         "jar_name": {"key": "jarName", "type": "str"},
         "entry_class": {"key": "entryClass", "type": "str"},
         "args": {"key": "args", "type": "str"},
         "save_point_name": {"key": "savePointName", "type": "str"},
         "action": {"key": "action", "type": "str"},
@@ -2529,26 +3500,29 @@
         "action_result": {"key": "actionResult", "type": "str"},
         "last_save_point": {"key": "lastSavePoint", "type": "str"},
     }
 
     def __init__(
         self,
         *,
-        job_name: str,
+        run_id: Optional[str] = None,
+        job_name: Optional[str] = None,
         job_jar_directory: Optional[str] = None,
         jar_name: Optional[str] = None,
         entry_class: Optional[str] = None,
         args: Optional[str] = None,
         save_point_name: Optional[str] = None,
         action: Optional[Union[str, "_models.Action"]] = None,
         flink_configuration: Optional[Dict[str, str]] = None,
         **kwargs: Any
     ) -> None:
         """
-        :keyword job_name: Name of job. Required.
+        :keyword run_id: Run id of job.
+        :paramtype run_id: str
+        :keyword job_name: Name of job.
         :paramtype job_name: str
         :keyword job_jar_directory: A string property that specifies the directory where the job JAR is
          located.
         :paramtype job_jar_directory: str
         :keyword jar_name: A string property that represents the name of the job JAR.
         :paramtype jar_name: str
         :keyword entry_class: A string property that specifies the entry class for the Flink job.
@@ -2558,23 +3532,25 @@
         :paramtype args: str
         :keyword save_point_name: A string property that represents the name of the savepoint for the
          Flink job.
         :paramtype save_point_name: str
         :keyword action: A string property that indicates the action to be performed on the Flink job.
          It can have one of the following enum values => NEW, UPDATE, STATELESS_UPDATE, STOP, START,
          CANCEL, SAVEPOINT, LIST_SAVEPOINT, or DELETE. Known values are: "NEW", "UPDATE",
-         "STATELESS_UPDATE", "STOP", "START", "CANCEL", "SAVEPOINT", "LIST_SAVEPOINT", and "DELETE".
+         "STATELESS_UPDATE", "STOP", "START", "CANCEL", "SAVEPOINT", "LIST_SAVEPOINT", "DELETE",
+         "LAST_STATE_UPDATE", and "RE_LAUNCH".
         :paramtype action: str or ~azure.mgmt.hdinsightcontainers.models.Action
         :keyword flink_configuration: Additional properties used to configure Flink jobs. It allows
          users to set properties such as parallelism and jobSavePointDirectory. It accepts additional
          key-value pairs as properties, where the keys are strings and the values are strings as well.
         :paramtype flink_configuration: dict[str, str]
         """
         super().__init__(**kwargs)
         self.job_type: str = "FlinkJob"
+        self.run_id = run_id
         self.job_name = job_name
         self.job_jar_directory = job_jar_directory
         self.jar_name = jar_name
         self.entry_class = entry_class
         self.args = args
         self.save_point_name = save_point_name
         self.action = action
@@ -2585,28 +3561,36 @@
         self.action_result = None
         self.last_save_point = None
 
 
 class FlinkProfile(_serialization.Model):
     """The Flink cluster profile.
 
-    All required parameters must be populated in order to send to Azure.
+    All required parameters must be populated in order to send to server.
 
     :ivar storage: The storage profile. Required.
     :vartype storage: ~azure.mgmt.hdinsightcontainers.models.FlinkStorageProfile
     :ivar num_replicas: The number of task managers.
     :vartype num_replicas: int
     :ivar job_manager: Job Manager container/ process CPU and memory requirements. Required.
     :vartype job_manager: ~azure.mgmt.hdinsightcontainers.models.ComputeResourceDefinition
     :ivar history_server: History Server container/ process CPU and memory requirements.
     :vartype history_server: ~azure.mgmt.hdinsightcontainers.models.ComputeResourceDefinition
     :ivar task_manager: Task Manager container/ process CPU and memory requirements. Required.
     :vartype task_manager: ~azure.mgmt.hdinsightcontainers.models.ComputeResourceDefinition
     :ivar catalog_options: Flink cluster catalog options.
     :vartype catalog_options: ~azure.mgmt.hdinsightcontainers.models.FlinkCatalogOptions
+    :ivar deployment_mode: A string property that indicates the deployment mode of Flink cluster.
+     It can have one of the following enum values => Application, Session. Default value is Session.
+     Known values are: "Application" and "Session".
+    :vartype deployment_mode: str or ~azure.mgmt.hdinsightcontainers.models.DeploymentMode
+    :ivar job_spec: Job specifications for flink clusters in application deployment mode. The
+     specification is immutable even if job properties are changed by calling the RunJob API, please
+     use the ListJob API to get the latest job information.
+    :vartype job_spec: ~azure.mgmt.hdinsightcontainers.models.FlinkJobProfile
     """
 
     _validation = {
         "storage": {"required": True},
         "job_manager": {"required": True},
         "task_manager": {"required": True},
     }
@@ -2614,25 +3598,29 @@
     _attribute_map = {
         "storage": {"key": "storage", "type": "FlinkStorageProfile"},
         "num_replicas": {"key": "numReplicas", "type": "int"},
         "job_manager": {"key": "jobManager", "type": "ComputeResourceDefinition"},
         "history_server": {"key": "historyServer", "type": "ComputeResourceDefinition"},
         "task_manager": {"key": "taskManager", "type": "ComputeResourceDefinition"},
         "catalog_options": {"key": "catalogOptions", "type": "FlinkCatalogOptions"},
+        "deployment_mode": {"key": "deploymentMode", "type": "str"},
+        "job_spec": {"key": "jobSpec", "type": "FlinkJobProfile"},
     }
 
     def __init__(
         self,
         *,
         storage: "_models.FlinkStorageProfile",
         job_manager: "_models.ComputeResourceDefinition",
         task_manager: "_models.ComputeResourceDefinition",
         num_replicas: Optional[int] = None,
         history_server: Optional["_models.ComputeResourceDefinition"] = None,
         catalog_options: Optional["_models.FlinkCatalogOptions"] = None,
+        deployment_mode: Optional[Union[str, "_models.DeploymentMode"]] = None,
+        job_spec: Optional["_models.FlinkJobProfile"] = None,
         **kwargs: Any
     ) -> None:
         """
         :keyword storage: The storage profile. Required.
         :paramtype storage: ~azure.mgmt.hdinsightcontainers.models.FlinkStorageProfile
         :keyword num_replicas: The number of task managers.
         :paramtype num_replicas: int
@@ -2640,38 +3628,48 @@
         :paramtype job_manager: ~azure.mgmt.hdinsightcontainers.models.ComputeResourceDefinition
         :keyword history_server: History Server container/ process CPU and memory requirements.
         :paramtype history_server: ~azure.mgmt.hdinsightcontainers.models.ComputeResourceDefinition
         :keyword task_manager: Task Manager container/ process CPU and memory requirements. Required.
         :paramtype task_manager: ~azure.mgmt.hdinsightcontainers.models.ComputeResourceDefinition
         :keyword catalog_options: Flink cluster catalog options.
         :paramtype catalog_options: ~azure.mgmt.hdinsightcontainers.models.FlinkCatalogOptions
+        :keyword deployment_mode: A string property that indicates the deployment mode of Flink
+         cluster. It can have one of the following enum values => Application, Session. Default value is
+         Session. Known values are: "Application" and "Session".
+        :paramtype deployment_mode: str or ~azure.mgmt.hdinsightcontainers.models.DeploymentMode
+        :keyword job_spec: Job specifications for flink clusters in application deployment mode. The
+         specification is immutable even if job properties are changed by calling the RunJob API, please
+         use the ListJob API to get the latest job information.
+        :paramtype job_spec: ~azure.mgmt.hdinsightcontainers.models.FlinkJobProfile
         """
         super().__init__(**kwargs)
         self.storage = storage
         self.num_replicas = num_replicas
         self.job_manager = job_manager
         self.history_server = history_server
         self.task_manager = task_manager
         self.catalog_options = catalog_options
+        self.deployment_mode = deployment_mode
+        self.job_spec = job_spec
 
 
 class FlinkStorageProfile(_serialization.Model):
     """The storage profile.
 
-    All required parameters must be populated in order to send to Azure.
+    All required parameters must be populated in order to send to server.
 
     :ivar storage_uri: Storage account uri which is used for savepoint and checkpoint state.
      Required.
     :vartype storage_uri: str
     :ivar storagekey: Storage key is only required for wasb(s) storage.
     :vartype storagekey: str
     """
 
     _validation = {
-        "storage_uri": {"required": True, "pattern": r"^(\w{4,5})://(.*)@(.*).\b(blob|dfs)\b\.core\.windows\.net$"},
+        "storage_uri": {"required": True, "pattern": r"^(\w{4,5})://(.*)@(.*).\b(blob|dfs)\b.*$"},
     }
 
     _attribute_map = {
         "storage_uri": {"key": "storageUri", "type": "str"},
         "storagekey": {"key": "storagekey", "type": "str"},
     }
 
@@ -2687,87 +3685,206 @@
         self.storage_uri = storage_uri
         self.storagekey = storagekey
 
 
 class HiveCatalogOption(_serialization.Model):
     """Hive Catalog Option.
 
-    All required parameters must be populated in order to send to Azure.
+    All required parameters must be populated in order to send to server.
 
     :ivar catalog_name: Name of trino catalog which should use specified hive metastore. Required.
     :vartype catalog_name: str
+    :ivar metastore_db_connection_authentication_mode: The authentication mode to connect to your
+     Hive metastore database. More details:
+     https://learn.microsoft.com/en-us/azure/azure-sql/database/logins-create-manage?view=azuresql#authentication-and-authorization.  # pylint: disable=line-too-long
+     Known values are: "SqlAuth" and "IdentityAuth".
+    :vartype metastore_db_connection_authentication_mode: str or
+     ~azure.mgmt.hdinsightcontainers.models.MetastoreDbConnectionAuthenticationMode
     :ivar metastore_db_connection_password_secret: Secret reference name from
-     secretsProfile.secrets containing password for database connection. Required.
+     secretsProfile.secrets containing password for database connection.
     :vartype metastore_db_connection_password_secret: str
     :ivar metastore_db_connection_url: Connection string for hive metastore database. Required.
     :vartype metastore_db_connection_url: str
-    :ivar metastore_db_connection_user_name: User name for database connection. Required.
+    :ivar metastore_db_connection_user_name: User name for database connection.
     :vartype metastore_db_connection_user_name: str
     :ivar metastore_warehouse_dir: Metastore root directory URI, format:
      abfs[s]://<container>@:code:`<account_name>`.dfs.core.windows.net/:code:`<path>`. More details:
      https://docs.microsoft.com/en-us/azure/storage/blobs/data-lake-storage-introduction-abfs-uri.
      Required.
     :vartype metastore_warehouse_dir: str
     """
 
     _validation = {
         "catalog_name": {"required": True, "min_length": 1},
-        "metastore_db_connection_password_secret": {"required": True},
         "metastore_db_connection_url": {"required": True},
-        "metastore_db_connection_user_name": {"required": True},
         "metastore_warehouse_dir": {"required": True},
     }
 
     _attribute_map = {
         "catalog_name": {"key": "catalogName", "type": "str"},
+        "metastore_db_connection_authentication_mode": {
+            "key": "metastoreDbConnectionAuthenticationMode",
+            "type": "str",
+        },
         "metastore_db_connection_password_secret": {"key": "metastoreDbConnectionPasswordSecret", "type": "str"},
         "metastore_db_connection_url": {"key": "metastoreDbConnectionURL", "type": "str"},
         "metastore_db_connection_user_name": {"key": "metastoreDbConnectionUserName", "type": "str"},
         "metastore_warehouse_dir": {"key": "metastoreWarehouseDir", "type": "str"},
     }
 
     def __init__(
         self,
         *,
         catalog_name: str,
-        metastore_db_connection_password_secret: str,
         metastore_db_connection_url: str,
-        metastore_db_connection_user_name: str,
         metastore_warehouse_dir: str,
+        metastore_db_connection_authentication_mode: Optional[
+            Union[str, "_models.MetastoreDbConnectionAuthenticationMode"]
+        ] = None,
+        metastore_db_connection_password_secret: Optional[str] = None,
+        metastore_db_connection_user_name: Optional[str] = None,
         **kwargs: Any
     ) -> None:
         """
         :keyword catalog_name: Name of trino catalog which should use specified hive metastore.
          Required.
         :paramtype catalog_name: str
+        :keyword metastore_db_connection_authentication_mode: The authentication mode to connect to
+         your Hive metastore database. More details:
+         https://learn.microsoft.com/en-us/azure/azure-sql/database/logins-create-manage?view=azuresql#authentication-and-authorization.  # pylint: disable=line-too-long
+         Known values are: "SqlAuth" and "IdentityAuth".
+        :paramtype metastore_db_connection_authentication_mode: str or
+         ~azure.mgmt.hdinsightcontainers.models.MetastoreDbConnectionAuthenticationMode
         :keyword metastore_db_connection_password_secret: Secret reference name from
-         secretsProfile.secrets containing password for database connection. Required.
+         secretsProfile.secrets containing password for database connection.
         :paramtype metastore_db_connection_password_secret: str
         :keyword metastore_db_connection_url: Connection string for hive metastore database. Required.
         :paramtype metastore_db_connection_url: str
-        :keyword metastore_db_connection_user_name: User name for database connection. Required.
+        :keyword metastore_db_connection_user_name: User name for database connection.
         :paramtype metastore_db_connection_user_name: str
         :keyword metastore_warehouse_dir: Metastore root directory URI, format:
          abfs[s]://<container>@:code:`<account_name>`.dfs.core.windows.net/:code:`<path>`. More details:
          https://docs.microsoft.com/en-us/azure/storage/blobs/data-lake-storage-introduction-abfs-uri.
          Required.
         :paramtype metastore_warehouse_dir: str
         """
         super().__init__(**kwargs)
         self.catalog_name = catalog_name
+        self.metastore_db_connection_authentication_mode = metastore_db_connection_authentication_mode
         self.metastore_db_connection_password_secret = metastore_db_connection_password_secret
         self.metastore_db_connection_url = metastore_db_connection_url
         self.metastore_db_connection_user_name = metastore_db_connection_user_name
         self.metastore_warehouse_dir = metastore_warehouse_dir
 
 
+class KafkaConnectivityEndpoints(_serialization.Model):
+    """Kafka bootstrap server and broker related connectivity endpoints.
+
+    :ivar bootstrap_server_endpoint: bootstrap server connectivity endpoint.
+    :vartype bootstrap_server_endpoint: str
+    :ivar broker_endpoints: Kafka broker endpoint list.
+    :vartype broker_endpoints: list[str]
+    """
+
+    _attribute_map = {
+        "bootstrap_server_endpoint": {"key": "bootstrapServerEndpoint", "type": "str"},
+        "broker_endpoints": {"key": "brokerEndpoints", "type": "[str]"},
+    }
+
+    def __init__(
+        self,
+        *,
+        bootstrap_server_endpoint: Optional[str] = None,
+        broker_endpoints: Optional[List[str]] = None,
+        **kwargs: Any
+    ) -> None:
+        """
+        :keyword bootstrap_server_endpoint: bootstrap server connectivity endpoint.
+        :paramtype bootstrap_server_endpoint: str
+        :keyword broker_endpoints: Kafka broker endpoint list.
+        :paramtype broker_endpoints: list[str]
+        """
+        super().__init__(**kwargs)
+        self.bootstrap_server_endpoint = bootstrap_server_endpoint
+        self.broker_endpoints = broker_endpoints
+
+
+class KafkaProfile(_serialization.Model):
+    """The Kafka cluster profile.
+
+    Variables are only populated by the server, and will be ignored when sending a request.
+
+    All required parameters must be populated in order to send to server.
+
+    :ivar enable_k_raft: Expose Kafka cluster in KRaft mode.
+    :vartype enable_k_raft: bool
+    :ivar enable_public_endpoints: Expose worker nodes as public endpoints.
+    :vartype enable_public_endpoints: bool
+    :ivar remote_storage_uri: Fully qualified path of Azure Storage container used for Tiered
+     Storage.
+    :vartype remote_storage_uri: str
+    :ivar disk_storage: Kafka disk storage profile. Required.
+    :vartype disk_storage: ~azure.mgmt.hdinsightcontainers.models.DiskStorageProfile
+    :ivar cluster_identity: Identity of the internal service components inside the Kafka cluster.
+    :vartype cluster_identity: ~azure.mgmt.hdinsightcontainers.models.IdentityProfile
+    :ivar connectivity_endpoints: Kafka bootstrap server and brokers related connectivity
+     endpoints.
+    :vartype connectivity_endpoints:
+     ~azure.mgmt.hdinsightcontainers.models.KafkaConnectivityEndpoints
+    """
+
+    _validation = {
+        "remote_storage_uri": {"pattern": r"^(https?|abfss?):\/\/[^/]+(?:\/|$)"},
+        "disk_storage": {"required": True},
+        "cluster_identity": {"readonly": True},
+        "connectivity_endpoints": {"readonly": True},
+    }
+
+    _attribute_map = {
+        "enable_k_raft": {"key": "enableKRaft", "type": "bool"},
+        "enable_public_endpoints": {"key": "enablePublicEndpoints", "type": "bool"},
+        "remote_storage_uri": {"key": "remoteStorageUri", "type": "str"},
+        "disk_storage": {"key": "diskStorage", "type": "DiskStorageProfile"},
+        "cluster_identity": {"key": "clusterIdentity", "type": "IdentityProfile"},
+        "connectivity_endpoints": {"key": "connectivityEndpoints", "type": "KafkaConnectivityEndpoints"},
+    }
+
+    def __init__(
+        self,
+        *,
+        disk_storage: "_models.DiskStorageProfile",
+        enable_k_raft: bool = True,
+        enable_public_endpoints: bool = False,
+        remote_storage_uri: Optional[str] = None,
+        **kwargs: Any
+    ) -> None:
+        """
+        :keyword enable_k_raft: Expose Kafka cluster in KRaft mode.
+        :paramtype enable_k_raft: bool
+        :keyword enable_public_endpoints: Expose worker nodes as public endpoints.
+        :paramtype enable_public_endpoints: bool
+        :keyword remote_storage_uri: Fully qualified path of Azure Storage container used for Tiered
+         Storage.
+        :paramtype remote_storage_uri: str
+        :keyword disk_storage: Kafka disk storage profile. Required.
+        :paramtype disk_storage: ~azure.mgmt.hdinsightcontainers.models.DiskStorageProfile
+        """
+        super().__init__(**kwargs)
+        self.enable_k_raft = enable_k_raft
+        self.enable_public_endpoints = enable_public_endpoints
+        self.remote_storage_uri = remote_storage_uri
+        self.disk_storage = disk_storage
+        self.cluster_identity = None
+        self.connectivity_endpoints = None
+
+
 class LoadBasedConfig(_serialization.Model):
     """Profile of load based Autoscale.
 
-    All required parameters must be populated in order to send to Azure.
+    All required parameters must be populated in order to send to server.
 
     :ivar min_nodes: User needs to set the minimum number of nodes for load based scaling, the load
      based scaling will use this to scale up and scale down between minimum and maximum number of
      nodes. Required.
     :vartype min_nodes: int
     :ivar max_nodes: User needs to set the maximum number of nodes for load based scaling, the load
      based scaling will use this to scale up and scale down between minimum and maximum number of
@@ -2901,15 +4018,15 @@
         self.reason = reason
         self.message = message
 
 
 class NodeProfile(_serialization.Model):
     """The node profile.
 
-    All required parameters must be populated in order to send to Azure.
+    All required parameters must be populated in order to send to server.
 
     :ivar type: The node type. Required.
     :vartype type: str
     :ivar vm_size: The virtual machine SKU. Required.
     :vartype vm_size: str
     :ivar count: The number of virtual machines. Required.
     :vartype count: int
@@ -3059,18 +4176,243 @@
     def __init__(self, **kwargs: Any) -> None:
         """ """
         super().__init__(**kwargs)
         self.value = None
         self.next_link = None
 
 
+class RangerAdminSpec(_serialization.Model):
+    """Specification for the Ranger Admin service.
+
+    All required parameters must be populated in order to send to server.
+
+    :ivar admins: List of usernames that should be marked as ranger admins. These usernames should
+     match the user principal name (UPN) of the respective AAD users. Required.
+    :vartype admins: list[str]
+    :ivar database: Required.
+    :vartype database: ~azure.mgmt.hdinsightcontainers.models.RangerAdminSpecDatabase
+    """
+
+    _validation = {
+        "admins": {"required": True},
+        "database": {"required": True},
+    }
+
+    _attribute_map = {
+        "admins": {"key": "admins", "type": "[str]"},
+        "database": {"key": "database", "type": "RangerAdminSpecDatabase"},
+    }
+
+    def __init__(self, *, admins: List[str], database: "_models.RangerAdminSpecDatabase", **kwargs: Any) -> None:
+        """
+        :keyword admins: List of usernames that should be marked as ranger admins. These usernames
+         should match the user principal name (UPN) of the respective AAD users. Required.
+        :paramtype admins: list[str]
+        :keyword database: Required.
+        :paramtype database: ~azure.mgmt.hdinsightcontainers.models.RangerAdminSpecDatabase
+        """
+        super().__init__(**kwargs)
+        self.admins = admins
+        self.database = database
+
+
+class RangerAdminSpecDatabase(_serialization.Model):
+    """RangerAdminSpecDatabase.
+
+    All required parameters must be populated in order to send to server.
+
+    :ivar host: The database URL. Required.
+    :vartype host: str
+    :ivar name: The database name. Required.
+    :vartype name: str
+    :ivar password_secret_ref: Reference for the database password.
+    :vartype password_secret_ref: str
+    :ivar username: The name of the database user.
+    :vartype username: str
+    """
+
+    _validation = {
+        "host": {"required": True},
+        "name": {"required": True},
+    }
+
+    _attribute_map = {
+        "host": {"key": "host", "type": "str"},
+        "name": {"key": "name", "type": "str"},
+        "password_secret_ref": {"key": "passwordSecretRef", "type": "str"},
+        "username": {"key": "username", "type": "str"},
+    }
+
+    def __init__(
+        self,
+        *,
+        host: str,
+        name: str,
+        password_secret_ref: Optional[str] = None,
+        username: Optional[str] = None,
+        **kwargs: Any
+    ) -> None:
+        """
+        :keyword host: The database URL. Required.
+        :paramtype host: str
+        :keyword name: The database name. Required.
+        :paramtype name: str
+        :keyword password_secret_ref: Reference for the database password.
+        :paramtype password_secret_ref: str
+        :keyword username: The name of the database user.
+        :paramtype username: str
+        """
+        super().__init__(**kwargs)
+        self.host = host
+        self.name = name
+        self.password_secret_ref = password_secret_ref
+        self.username = username
+
+
+class RangerAuditSpec(_serialization.Model):
+    """Properties required to describe audit log storage.
+
+    :ivar storage_account: Azure storage location of the blobs. MSI should have read/write access
+     to this Storage account.
+    :vartype storage_account: str
+    """
+
+    _validation = {
+        "storage_account": {"min_length": 1, "pattern": r"^(https)|(abfss)://.*$"},
+    }
+
+    _attribute_map = {
+        "storage_account": {"key": "storageAccount", "type": "str"},
+    }
+
+    def __init__(self, *, storage_account: Optional[str] = None, **kwargs: Any) -> None:
+        """
+        :keyword storage_account: Azure storage location of the blobs. MSI should have read/write
+         access to this Storage account.
+        :paramtype storage_account: str
+        """
+        super().__init__(**kwargs)
+        self.storage_account = storage_account
+
+
+class RangerProfile(_serialization.Model):
+    """The ranger cluster profile.
+
+    All required parameters must be populated in order to send to server.
+
+    :ivar ranger_admin: Specification for the Ranger Admin service. Required.
+    :vartype ranger_admin: ~azure.mgmt.hdinsightcontainers.models.RangerAdminSpec
+    :ivar ranger_audit: Properties required to describe audit log storage.
+    :vartype ranger_audit: ~azure.mgmt.hdinsightcontainers.models.RangerAuditSpec
+    :ivar ranger_usersync: Specification for the Ranger Usersync service. Required.
+    :vartype ranger_usersync: ~azure.mgmt.hdinsightcontainers.models.RangerUsersyncSpec
+    """
+
+    _validation = {
+        "ranger_admin": {"required": True},
+        "ranger_usersync": {"required": True},
+    }
+
+    _attribute_map = {
+        "ranger_admin": {"key": "rangerAdmin", "type": "RangerAdminSpec"},
+        "ranger_audit": {"key": "rangerAudit", "type": "RangerAuditSpec"},
+        "ranger_usersync": {"key": "rangerUsersync", "type": "RangerUsersyncSpec"},
+    }
+
+    def __init__(
+        self,
+        *,
+        ranger_admin: "_models.RangerAdminSpec",
+        ranger_usersync: "_models.RangerUsersyncSpec",
+        ranger_audit: Optional["_models.RangerAuditSpec"] = None,
+        **kwargs: Any
+    ) -> None:
+        """
+        :keyword ranger_admin: Specification for the Ranger Admin service. Required.
+        :paramtype ranger_admin: ~azure.mgmt.hdinsightcontainers.models.RangerAdminSpec
+        :keyword ranger_audit: Properties required to describe audit log storage.
+        :paramtype ranger_audit: ~azure.mgmt.hdinsightcontainers.models.RangerAuditSpec
+        :keyword ranger_usersync: Specification for the Ranger Usersync service. Required.
+        :paramtype ranger_usersync: ~azure.mgmt.hdinsightcontainers.models.RangerUsersyncSpec
+        """
+        super().__init__(**kwargs)
+        self.ranger_admin = ranger_admin
+        self.ranger_audit = ranger_audit
+        self.ranger_usersync = ranger_usersync
+
+
+class RangerUsersyncSpec(_serialization.Model):
+    """Specification for the Ranger Usersync service.
+
+    :ivar enabled: Denotes whether usersync service should be enabled.
+    :vartype enabled: bool
+    :ivar groups: List of groups that should be synced. These group names should match the object
+     id of the respective AAD groups.
+    :vartype groups: list[str]
+    :ivar mode: User & groups can be synced automatically or via a static list that's refreshed.
+     Known values are: "static" and "automatic".
+    :vartype mode: str or ~azure.mgmt.hdinsightcontainers.models.RangerUsersyncMode
+    :ivar user_mapping_location: Azure storage location of a mapping file that lists user & group
+     associations.
+    :vartype user_mapping_location: str
+    :ivar users: List of user names that should be synced. These usernames should match the User
+     principal name of the respective AAD users.
+    :vartype users: list[str]
+    """
+
+    _validation = {
+        "user_mapping_location": {"min_length": 1, "pattern": r"^(https)|(abfss)://.*$"},
+    }
+
+    _attribute_map = {
+        "enabled": {"key": "enabled", "type": "bool"},
+        "groups": {"key": "groups", "type": "[str]"},
+        "mode": {"key": "mode", "type": "str"},
+        "user_mapping_location": {"key": "userMappingLocation", "type": "str"},
+        "users": {"key": "users", "type": "[str]"},
+    }
+
+    def __init__(
+        self,
+        *,
+        enabled: bool = True,
+        groups: Optional[List[str]] = None,
+        mode: Union[str, "_models.RangerUsersyncMode"] = "automatic",
+        user_mapping_location: Optional[str] = None,
+        users: Optional[List[str]] = None,
+        **kwargs: Any
+    ) -> None:
+        """
+        :keyword enabled: Denotes whether usersync service should be enabled.
+        :paramtype enabled: bool
+        :keyword groups: List of groups that should be synced. These group names should match the
+         object id of the respective AAD groups.
+        :paramtype groups: list[str]
+        :keyword mode: User & groups can be synced automatically or via a static list that's refreshed.
+         Known values are: "static" and "automatic".
+        :paramtype mode: str or ~azure.mgmt.hdinsightcontainers.models.RangerUsersyncMode
+        :keyword user_mapping_location: Azure storage location of a mapping file that lists user &
+         group associations.
+        :paramtype user_mapping_location: str
+        :keyword users: List of user names that should be synced. These usernames should match the User
+         principal name of the respective AAD users.
+        :paramtype users: list[str]
+        """
+        super().__init__(**kwargs)
+        self.enabled = enabled
+        self.groups = groups
+        self.mode = mode
+        self.user_mapping_location = user_mapping_location
+        self.users = users
+
+
 class ScalingRule(_serialization.Model):
     """The scaling rule.
 
-    All required parameters must be populated in order to send to Azure.
+    All required parameters must be populated in order to send to server.
 
     :ivar action_type: The action type. Required. Known values are: "scaleup" and "scaledown".
     :vartype action_type: str or ~azure.mgmt.hdinsightcontainers.models.ScaleActionType
     :ivar evaluation_count: This is an evaluation count for a scaling condition, the number of
      times a trigger condition should be successful, before scaling activity is triggered. Required.
     :vartype evaluation_count: int
     :ivar scaling_metric: Metrics name for individual workloads. For example: cpu. Required.
@@ -3119,15 +4461,15 @@
         self.scaling_metric = scaling_metric
         self.comparison_rule = comparison_rule
 
 
 class Schedule(_serialization.Model):
     """Schedule definition.
 
-    All required parameters must be populated in order to send to Azure.
+    All required parameters must be populated in order to send to server.
 
     :ivar start_time: User has to set the start time of current schedule configuration, format like
      10:30 (HH:MM). Required.
     :vartype start_time: str
     :ivar end_time: User has to set the end time of current schedule configuration, format like
      10:30 (HH:MM). Required.
     :vartype end_time: str
@@ -3182,15 +4524,15 @@
         self.count = count
         self.days = days
 
 
 class ScheduleBasedConfig(_serialization.Model):
     """Profile of schedule based Autoscale.
 
-    All required parameters must be populated in order to send to Azure.
+    All required parameters must be populated in order to send to server.
 
     :ivar time_zone: User has to specify the timezone on which the schedule has to be set for
      schedule based autoscale configuration. Required.
     :vartype time_zone: str
     :ivar default_count: Setting default node count of current schedule configuration. Default node
      count specifies the number of nodes which are default when an specified scaling operation is
      executed (scale up/scale down). Required.
@@ -3234,15 +4576,15 @@
         self.default_count = default_count
         self.schedules = schedules
 
 
 class ScriptActionProfile(_serialization.Model):
     """The script action profile.
 
-    All required parameters must be populated in order to send to Azure.
+    All required parameters must be populated in order to send to server.
 
     :ivar type: Type of the script action. Supported type is bash scripts. Required.
     :vartype type: str
     :ivar name: Script name. Required.
     :vartype name: str
     :ivar url: Url of the script file. Required.
     :vartype url: str
@@ -3256,15 +4598,15 @@
     :ivar should_persist: Specify if the script should persist on the cluster.
     :vartype should_persist: bool
     """
 
     _validation = {
         "type": {"required": True},
         "name": {"required": True},
-        "url": {"required": True, "pattern": r"^(https)|(http)|(abfss)|(abfs)|(wasbs)|(wasb)://.*$"},
+        "url": {"required": True, "pattern": r"^(https)|(http)://.*$"},
         "services": {"required": True},
     }
 
     _attribute_map = {
         "type": {"key": "type", "type": "str"},
         "name": {"key": "name", "type": "str"},
         "url": {"key": "url", "type": "str"},
@@ -3312,15 +4654,15 @@
         self.timeout_in_minutes = timeout_in_minutes
         self.should_persist = should_persist
 
 
 class SecretReference(_serialization.Model):
     """Secret reference and corresponding properties of a key vault secret.
 
-    All required parameters must be populated in order to send to Azure.
+    All required parameters must be populated in order to send to server.
 
     :ivar reference_name: Reference name of the secret to be used in service configs. Required.
     :vartype reference_name: str
     :ivar type: Type of key vault object: secret, key or certificate. Required. Known values are:
      "Key", "Secret", and "Certificate".
     :vartype type: str or ~azure.mgmt.hdinsightcontainers.models.KeyVaultObjectType
     :ivar version: Version of the secret in key vault.
@@ -3368,15 +4710,15 @@
         self.version = version
         self.key_vault_object_name = key_vault_object_name
 
 
 class SecretsProfile(_serialization.Model):
     """The cluster secret profile.
 
-    All required parameters must be populated in order to send to Azure.
+    All required parameters must be populated in order to send to server.
 
     :ivar key_vault_resource_id: Name of the user Key Vault where all the cluster specific user
      secrets are stored. Required.
     :vartype key_vault_resource_id: str
     :ivar secrets: Properties of Key Vault secret.
     :vartype secrets: list[~azure.mgmt.hdinsightcontainers.models.SecretReference]
     """
@@ -3434,15 +4776,15 @@
         self.value = value
         self.next_link = None
 
 
 class ServiceConfigListResultProperties(_serialization.Model):
     """Service config response.
 
-    All required parameters must be populated in order to send to Azure.
+    All required parameters must be populated in order to send to server.
 
     :ivar service_name: Service Config Name. Required.
     :vartype service_name: str
     :ivar file_name: File Name. Required.
     :vartype file_name: str
     :ivar content: Content in the service config file.
     :vartype content: str
@@ -3518,15 +4860,15 @@
         self.custom_keys = custom_keys
         self.default_keys = default_keys
 
 
 class ServiceConfigListResultValueEntity(_serialization.Model):
     """Default config details.
 
-    All required parameters must be populated in order to send to Azure.
+    All required parameters must be populated in order to send to server.
 
     :ivar value: Config value. Required.
     :vartype value: str
     :ivar description: Config description.
     :vartype description: str
     """
 
@@ -3550,91 +4892,35 @@
         self.value = value
         self.description = description
 
 
 class ServiceConfigResult(_serialization.Model):
     """Cluster instance service config.
 
-    :ivar service_name: Service Config Name.
-    :vartype service_name: str
-    :ivar file_name: File Name.
-    :vartype file_name: str
-    :ivar content: Content in the service config file.
-    :vartype content: str
-    :ivar component_name: Component Name.
-    :vartype component_name: str
-    :ivar type: Config type.
-    :vartype type: str
-    :ivar path: Config file path.
-    :vartype path: str
-    :ivar custom_keys: The custom keys.
-    :vartype custom_keys: dict[str, str]
-    :ivar default_keys: The default keys.
-    :vartype default_keys: dict[str,
-     ~azure.mgmt.hdinsightcontainers.models.ServiceConfigListResultValueEntity]
+    :ivar properties: Cluster instance service config properties.
+    :vartype properties: ~azure.mgmt.hdinsightcontainers.models.ServiceConfigResultProperties
     """
 
     _attribute_map = {
-        "service_name": {"key": "properties.serviceName", "type": "str"},
-        "file_name": {"key": "properties.fileName", "type": "str"},
-        "content": {"key": "properties.content", "type": "str"},
-        "component_name": {"key": "properties.componentName", "type": "str"},
-        "type": {"key": "properties.type", "type": "str"},
-        "path": {"key": "properties.path", "type": "str"},
-        "custom_keys": {"key": "properties.customKeys", "type": "{str}"},
-        "default_keys": {"key": "properties.defaultKeys", "type": "{ServiceConfigListResultValueEntity}"},
+        "properties": {"key": "properties", "type": "ServiceConfigResultProperties"},
     }
 
-    def __init__(
-        self,
-        *,
-        service_name: Optional[str] = None,
-        file_name: Optional[str] = None,
-        content: Optional[str] = None,
-        component_name: Optional[str] = None,
-        type: Optional[str] = None,
-        path: Optional[str] = None,
-        custom_keys: Optional[Dict[str, str]] = None,
-        default_keys: Optional[Dict[str, "_models.ServiceConfigListResultValueEntity"]] = None,
-        **kwargs: Any
-    ) -> None:
+    def __init__(self, *, properties: Optional["_models.ServiceConfigResultProperties"] = None, **kwargs: Any) -> None:
         """
-        :keyword service_name: Service Config Name.
-        :paramtype service_name: str
-        :keyword file_name: File Name.
-        :paramtype file_name: str
-        :keyword content: Content in the service config file.
-        :paramtype content: str
-        :keyword component_name: Component Name.
-        :paramtype component_name: str
-        :keyword type: Config type.
-        :paramtype type: str
-        :keyword path: Config file path.
-        :paramtype path: str
-        :keyword custom_keys: The custom keys.
-        :paramtype custom_keys: dict[str, str]
-        :keyword default_keys: The default keys.
-        :paramtype default_keys: dict[str,
-         ~azure.mgmt.hdinsightcontainers.models.ServiceConfigListResultValueEntity]
+        :keyword properties: Cluster instance service config properties.
+        :paramtype properties: ~azure.mgmt.hdinsightcontainers.models.ServiceConfigResultProperties
         """
         super().__init__(**kwargs)
-        self.service_name = service_name
-        self.file_name = file_name
-        self.content = content
-        self.component_name = component_name
-        self.type = type
-        self.path = path
-        self.custom_keys = custom_keys
-        self.default_keys = default_keys
+        self.properties = properties
 
 
 class ServiceConfigResultProperties(ServiceConfigListResultProperties):
     """Cluster instance service config properties.
 
-    All required parameters must be populated in order to send to Azure.
+    All required parameters must be populated in order to send to server.
 
     :ivar service_name: Service Config Name. Required.
     :vartype service_name: str
     :ivar file_name: File Name. Required.
     :vartype file_name: str
     :ivar content: Content in the service config file.
     :vartype content: str
@@ -3647,80 +4933,19 @@
     :ivar custom_keys: The custom keys.
     :vartype custom_keys: dict[str, str]
     :ivar default_keys: The default keys.
     :vartype default_keys: dict[str,
      ~azure.mgmt.hdinsightcontainers.models.ServiceConfigListResultValueEntity]
     """
 
-    _validation = {
-        "service_name": {"required": True},
-        "file_name": {"required": True},
-        "component_name": {"required": True},
-    }
-
-    _attribute_map = {
-        "service_name": {"key": "serviceName", "type": "str"},
-        "file_name": {"key": "fileName", "type": "str"},
-        "content": {"key": "content", "type": "str"},
-        "component_name": {"key": "componentName", "type": "str"},
-        "type": {"key": "type", "type": "str"},
-        "path": {"key": "path", "type": "str"},
-        "custom_keys": {"key": "customKeys", "type": "{str}"},
-        "default_keys": {"key": "defaultKeys", "type": "{ServiceConfigListResultValueEntity}"},
-    }
-
-    def __init__(
-        self,
-        *,
-        service_name: str,
-        file_name: str,
-        component_name: str,
-        content: Optional[str] = None,
-        type: Optional[str] = None,
-        path: Optional[str] = None,
-        custom_keys: Optional[Dict[str, str]] = None,
-        default_keys: Optional[Dict[str, "_models.ServiceConfigListResultValueEntity"]] = None,
-        **kwargs: Any
-    ) -> None:
-        """
-        :keyword service_name: Service Config Name. Required.
-        :paramtype service_name: str
-        :keyword file_name: File Name. Required.
-        :paramtype file_name: str
-        :keyword content: Content in the service config file.
-        :paramtype content: str
-        :keyword component_name: Component Name. Required.
-        :paramtype component_name: str
-        :keyword type: Config type.
-        :paramtype type: str
-        :keyword path: Config file path.
-        :paramtype path: str
-        :keyword custom_keys: The custom keys.
-        :paramtype custom_keys: dict[str, str]
-        :keyword default_keys: The default keys.
-        :paramtype default_keys: dict[str,
-         ~azure.mgmt.hdinsightcontainers.models.ServiceConfigListResultValueEntity]
-        """
-        super().__init__(
-            service_name=service_name,
-            file_name=file_name,
-            content=content,
-            component_name=component_name,
-            type=type,
-            path=path,
-            custom_keys=custom_keys,
-            default_keys=default_keys,
-            **kwargs
-        )
-
 
 class ServiceStatus(_serialization.Model):
-    """Describes the status of a service of a HDInsight on aks cluster.
+    """Describes the status of a service of a HDInsight on AKS cluster.
 
-    All required parameters must be populated in order to send to Azure.
+    All required parameters must be populated in order to send to server.
 
     :ivar kind: Kind of the service. E.g. "Zookeeper". Required.
     :vartype kind: str
     :ivar ready: Indicates if the service is ready / healthy. Values can be "true", "false",
      "unknown" or anything else. Required.
     :vartype ready: str
     :ivar message: A message describing the error if any.
@@ -3753,77 +4978,87 @@
         self.ready = ready
         self.message = message
 
 
 class SparkMetastoreSpec(_serialization.Model):
     """The metastore specification for Spark cluster.
 
-    All required parameters must be populated in order to send to Azure.
+    All required parameters must be populated in order to send to server.
 
     :ivar db_server_host: The database server host. Required.
     :vartype db_server_host: str
     :ivar db_name: The database name. Required.
     :vartype db_name: str
-    :ivar db_user_name: The database user name. Required.
+    :ivar db_connection_authentication_mode: The authentication mode to connect to your Hive
+     metastore database. More details:
+     https://learn.microsoft.com/en-us/azure/azure-sql/database/logins-create-manage?view=azuresql#authentication-and-authorization.  # pylint: disable=line-too-long
+     Known values are: "SqlAuth" and "IdentityAuth".
+    :vartype db_connection_authentication_mode: str or
+     ~azure.mgmt.hdinsightcontainers.models.DbConnectionAuthenticationMode
+    :ivar db_user_name: The database user name.
     :vartype db_user_name: str
     :ivar db_password_secret_name: The secret name which contains the database user password.
-     Required.
     :vartype db_password_secret_name: str
-    :ivar key_vault_id: The key vault resource id. Required.
+    :ivar key_vault_id: The key vault resource id.
     :vartype key_vault_id: str
     :ivar thrift_url: The thrift url.
     :vartype thrift_url: str
     """
 
     _validation = {
         "db_server_host": {"required": True},
         "db_name": {"required": True},
-        "db_user_name": {"required": True},
-        "db_password_secret_name": {"required": True},
-        "key_vault_id": {"required": True},
     }
 
     _attribute_map = {
         "db_server_host": {"key": "dbServerHost", "type": "str"},
         "db_name": {"key": "dbName", "type": "str"},
+        "db_connection_authentication_mode": {"key": "dbConnectionAuthenticationMode", "type": "str"},
         "db_user_name": {"key": "dbUserName", "type": "str"},
         "db_password_secret_name": {"key": "dbPasswordSecretName", "type": "str"},
         "key_vault_id": {"key": "keyVaultId", "type": "str"},
         "thrift_url": {"key": "thriftUrl", "type": "str"},
     }
 
     def __init__(
         self,
         *,
         db_server_host: str,
         db_name: str,
-        db_user_name: str,
-        db_password_secret_name: str,
-        key_vault_id: str,
+        db_connection_authentication_mode: Union[str, "_models.DbConnectionAuthenticationMode"] = "IdentityAuth",
+        db_user_name: Optional[str] = None,
+        db_password_secret_name: Optional[str] = None,
+        key_vault_id: Optional[str] = None,
         thrift_url: Optional[str] = None,
         **kwargs: Any
     ) -> None:
         """
         :keyword db_server_host: The database server host. Required.
         :paramtype db_server_host: str
         :keyword db_name: The database name. Required.
         :paramtype db_name: str
-        :keyword db_user_name: The database user name. Required.
+        :keyword db_connection_authentication_mode: The authentication mode to connect to your Hive
+         metastore database. More details:
+         https://learn.microsoft.com/en-us/azure/azure-sql/database/logins-create-manage?view=azuresql#authentication-and-authorization.  # pylint: disable=line-too-long
+         Known values are: "SqlAuth" and "IdentityAuth".
+        :paramtype db_connection_authentication_mode: str or
+         ~azure.mgmt.hdinsightcontainers.models.DbConnectionAuthenticationMode
+        :keyword db_user_name: The database user name.
         :paramtype db_user_name: str
         :keyword db_password_secret_name: The secret name which contains the database user password.
-         Required.
         :paramtype db_password_secret_name: str
-        :keyword key_vault_id: The key vault resource id. Required.
+        :keyword key_vault_id: The key vault resource id.
         :paramtype key_vault_id: str
         :keyword thrift_url: The thrift url.
         :paramtype thrift_url: str
         """
         super().__init__(**kwargs)
         self.db_server_host = db_server_host
         self.db_name = db_name
+        self.db_connection_authentication_mode = db_connection_authentication_mode
         self.db_user_name = db_user_name
         self.db_password_secret_name = db_password_secret_name
         self.key_vault_id = key_vault_id
         self.thrift_url = thrift_url
 
 
 class SparkProfile(_serialization.Model):
@@ -3864,15 +5099,15 @@
         self.metastore_spec = metastore_spec
         self.user_plugins_spec = user_plugins_spec
 
 
 class SparkUserPlugin(_serialization.Model):
     """Spark user plugin.
 
-    All required parameters must be populated in order to send to Azure.
+    All required parameters must be populated in order to send to server.
 
     :ivar path: Fully qualified path to the folder containing the plugins. Required.
     :vartype path: str
     """
 
     _validation = {
         "path": {"required": True, "min_length": 1, "pattern": r"^(https)|(abfss)://.*$"},
@@ -3910,43 +5145,51 @@
         super().__init__(**kwargs)
         self.plugins = plugins
 
 
 class SshConnectivityEndpoint(_serialization.Model):
     """SSH connectivity endpoint details.
 
-    All required parameters must be populated in order to send to Azure.
+    All required parameters must be populated in order to send to server.
 
     :ivar endpoint: SSH connectivity endpoint. Required.
     :vartype endpoint: str
+    :ivar private_ssh_endpoint: Private SSH connectivity endpoint. This property will only be
+     returned when enableInternalIngress is true.
+    :vartype private_ssh_endpoint: str
     """
 
     _validation = {
         "endpoint": {"required": True},
     }
 
     _attribute_map = {
         "endpoint": {"key": "endpoint", "type": "str"},
+        "private_ssh_endpoint": {"key": "privateSshEndpoint", "type": "str"},
     }
 
-    def __init__(self, *, endpoint: str, **kwargs: Any) -> None:
+    def __init__(self, *, endpoint: str, private_ssh_endpoint: Optional[str] = None, **kwargs: Any) -> None:
         """
         :keyword endpoint: SSH connectivity endpoint. Required.
         :paramtype endpoint: str
+        :keyword private_ssh_endpoint: Private SSH connectivity endpoint. This property will only be
+         returned when enableInternalIngress is true.
+        :paramtype private_ssh_endpoint: str
         """
         super().__init__(**kwargs)
         self.endpoint = endpoint
+        self.private_ssh_endpoint = private_ssh_endpoint
 
 
 class SshProfile(_serialization.Model):
     """Ssh profile for the cluster.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
-    All required parameters must be populated in order to send to Azure.
+    All required parameters must be populated in order to send to server.
 
     :ivar count: Number of ssh pods per cluster. Required.
     :vartype count: int
     :ivar pod_prefix: Prefix of the pod names. Pod number will be appended to the prefix. The
      ingress URLs for the pods will be available at
      :code:`<clusterFqdn>`/:code:`<sshBasePath>`/:code:`<prefix>`-:code:`<number>`.
     :vartype pod_prefix: str
@@ -4055,54 +5298,72 @@
         super().__init__(**kwargs)
         self.tags = tags
 
 
 class TrinoCoordinator(_serialization.Model):
     """Trino Coordinator.
 
+    :ivar debug: Trino debug configuration.
+    :vartype debug: ~azure.mgmt.hdinsightcontainers.models.TrinoDebugConfig
     :ivar high_availability_enabled: The flag that if enable coordinator HA, uses multiple
      coordinator replicas with auto failover, one per each head node. Default: true.
     :vartype high_availability_enabled: bool
-    :ivar enable: The flag that if enable debug or not.
-    :vartype enable: bool
-    :ivar port: The debug port.
-    :vartype port: int
-    :ivar suspend: The flag that if suspend debug or not.
-    :vartype suspend: bool
     """
 
     _attribute_map = {
+        "debug": {"key": "debug", "type": "TrinoDebugConfig"},
         "high_availability_enabled": {"key": "highAvailabilityEnabled", "type": "bool"},
-        "enable": {"key": "debug.enable", "type": "bool"},
-        "port": {"key": "debug.port", "type": "int"},
-        "suspend": {"key": "debug.suspend", "type": "bool"},
     }
 
     def __init__(
         self,
         *,
+        debug: Optional["_models.TrinoDebugConfig"] = None,
         high_availability_enabled: bool = True,
-        enable: bool = False,
-        port: int = 8008,
-        suspend: bool = False,
         **kwargs: Any
     ) -> None:
         """
+        :keyword debug: Trino debug configuration.
+        :paramtype debug: ~azure.mgmt.hdinsightcontainers.models.TrinoDebugConfig
         :keyword high_availability_enabled: The flag that if enable coordinator HA, uses multiple
          coordinator replicas with auto failover, one per each head node. Default: true.
         :paramtype high_availability_enabled: bool
+        """
+        super().__init__(**kwargs)
+        self.debug = debug
+        self.high_availability_enabled = high_availability_enabled
+
+
+class TrinoDebugConfig(_serialization.Model):
+    """Trino debug configuration.
+
+    :ivar enable: The flag that if enable debug or not.
+    :vartype enable: bool
+    :ivar port: The debug port.
+    :vartype port: int
+    :ivar suspend: The flag that if suspend debug or not.
+    :vartype suspend: bool
+    """
+
+    _attribute_map = {
+        "enable": {"key": "enable", "type": "bool"},
+        "port": {"key": "port", "type": "int"},
+        "suspend": {"key": "suspend", "type": "bool"},
+    }
+
+    def __init__(self, *, enable: bool = False, port: int = 8008, suspend: bool = False, **kwargs: Any) -> None:
+        """
         :keyword enable: The flag that if enable debug or not.
         :paramtype enable: bool
         :keyword port: The debug port.
         :paramtype port: int
         :keyword suspend: The flag that if suspend debug or not.
         :paramtype suspend: bool
         """
         super().__init__(**kwargs)
-        self.high_availability_enabled = high_availability_enabled
         self.enable = enable
         self.port = port
         self.suspend = suspend
 
 
 class TrinoProfile(_serialization.Model):
     """Trino Cluster profile.
@@ -4294,41 +5555,29 @@
         super().__init__(**kwargs)
         self.storage = storage
 
 
 class TrinoWorker(_serialization.Model):
     """Trino worker.
 
-    :ivar enable: The flag that if enable debug or not.
-    :vartype enable: bool
-    :ivar port: The debug port.
-    :vartype port: int
-    :ivar suspend: The flag that if suspend debug or not.
-    :vartype suspend: bool
+    :ivar debug: Trino debug configuration.
+    :vartype debug: ~azure.mgmt.hdinsightcontainers.models.TrinoDebugConfig
     """
 
     _attribute_map = {
-        "enable": {"key": "debug.enable", "type": "bool"},
-        "port": {"key": "debug.port", "type": "int"},
-        "suspend": {"key": "debug.suspend", "type": "bool"},
+        "debug": {"key": "debug", "type": "TrinoDebugConfig"},
     }
 
-    def __init__(self, *, enable: bool = False, port: int = 8008, suspend: bool = False, **kwargs: Any) -> None:
+    def __init__(self, *, debug: Optional["_models.TrinoDebugConfig"] = None, **kwargs: Any) -> None:
         """
-        :keyword enable: The flag that if enable debug or not.
-        :paramtype enable: bool
-        :keyword port: The debug port.
-        :paramtype port: int
-        :keyword suspend: The flag that if suspend debug or not.
-        :paramtype suspend: bool
+        :keyword debug: Trino debug configuration.
+        :paramtype debug: ~azure.mgmt.hdinsightcontainers.models.TrinoDebugConfig
         """
         super().__init__(**kwargs)
-        self.enable = enable
-        self.port = port
-        self.suspend = suspend
+        self.debug = debug
 
 
 class UpdatableClusterProfile(_serialization.Model):
     """Cluster resource patch properties.
 
     :ivar service_configs_profiles: The service configs profiles.
     :vartype service_configs_profiles:
@@ -4343,38 +5592,47 @@
     :vartype authorization_profile: ~azure.mgmt.hdinsightcontainers.models.AuthorizationProfile
     :ivar log_analytics_profile: Cluster log analytics profile to enable or disable OMS agent for
      cluster.
     :vartype log_analytics_profile:
      ~azure.mgmt.hdinsightcontainers.models.ClusterLogAnalyticsProfile
     :ivar prometheus_profile: Cluster Prometheus profile.
     :vartype prometheus_profile: ~azure.mgmt.hdinsightcontainers.models.ClusterPrometheusProfile
+    :ivar ranger_plugin_profile: Cluster Ranger plugin profile.
+    :vartype ranger_plugin_profile:
+     ~azure.mgmt.hdinsightcontainers.models.ClusterRangerPluginProfile
+    :ivar ranger_profile: The ranger cluster profile.
+    :vartype ranger_profile: ~azure.mgmt.hdinsightcontainers.models.RangerProfile
     :ivar script_action_profiles: The script action profile list.
     :vartype script_action_profiles:
      list[~azure.mgmt.hdinsightcontainers.models.ScriptActionProfile]
     """
 
     _attribute_map = {
         "service_configs_profiles": {"key": "serviceConfigsProfiles", "type": "[ClusterServiceConfigsProfile]"},
         "ssh_profile": {"key": "sshProfile", "type": "SshProfile"},
         "autoscale_profile": {"key": "autoscaleProfile", "type": "AutoscaleProfile"},
         "authorization_profile": {"key": "authorizationProfile", "type": "AuthorizationProfile"},
         "log_analytics_profile": {"key": "logAnalyticsProfile", "type": "ClusterLogAnalyticsProfile"},
         "prometheus_profile": {"key": "prometheusProfile", "type": "ClusterPrometheusProfile"},
+        "ranger_plugin_profile": {"key": "rangerPluginProfile", "type": "ClusterRangerPluginProfile"},
+        "ranger_profile": {"key": "rangerProfile", "type": "RangerProfile"},
         "script_action_profiles": {"key": "scriptActionProfiles", "type": "[ScriptActionProfile]"},
     }
 
     def __init__(
         self,
         *,
         service_configs_profiles: Optional[List["_models.ClusterServiceConfigsProfile"]] = None,
         ssh_profile: Optional["_models.SshProfile"] = None,
         autoscale_profile: Optional["_models.AutoscaleProfile"] = None,
         authorization_profile: Optional["_models.AuthorizationProfile"] = None,
         log_analytics_profile: Optional["_models.ClusterLogAnalyticsProfile"] = None,
         prometheus_profile: Optional["_models.ClusterPrometheusProfile"] = None,
+        ranger_plugin_profile: Optional["_models.ClusterRangerPluginProfile"] = None,
+        ranger_profile: Optional["_models.RangerProfile"] = None,
         script_action_profiles: Optional[List["_models.ScriptActionProfile"]] = None,
         **kwargs: Any
     ) -> None:
         """
         :keyword service_configs_profiles: The service configs profiles.
         :paramtype service_configs_profiles:
          list[~azure.mgmt.hdinsightcontainers.models.ClusterServiceConfigsProfile]
@@ -4388,19 +5646,26 @@
         :paramtype authorization_profile: ~azure.mgmt.hdinsightcontainers.models.AuthorizationProfile
         :keyword log_analytics_profile: Cluster log analytics profile to enable or disable OMS agent
          for cluster.
         :paramtype log_analytics_profile:
          ~azure.mgmt.hdinsightcontainers.models.ClusterLogAnalyticsProfile
         :keyword prometheus_profile: Cluster Prometheus profile.
         :paramtype prometheus_profile: ~azure.mgmt.hdinsightcontainers.models.ClusterPrometheusProfile
+        :keyword ranger_plugin_profile: Cluster Ranger plugin profile.
+        :paramtype ranger_plugin_profile:
+         ~azure.mgmt.hdinsightcontainers.models.ClusterRangerPluginProfile
+        :keyword ranger_profile: The ranger cluster profile.
+        :paramtype ranger_profile: ~azure.mgmt.hdinsightcontainers.models.RangerProfile
         :keyword script_action_profiles: The script action profile list.
         :paramtype script_action_profiles:
          list[~azure.mgmt.hdinsightcontainers.models.ScriptActionProfile]
         """
         super().__init__(**kwargs)
         self.service_configs_profiles = service_configs_profiles
         self.ssh_profile = ssh_profile
         self.autoscale_profile = autoscale_profile
         self.authorization_profile = authorization_profile
         self.log_analytics_profile = log_analytics_profile
         self.prometheus_profile = prometheus_profile
+        self.ranger_plugin_profile = ranger_plugin_profile
+        self.ranger_profile = ranger_profile
         self.script_action_profiles = script_action_profiles
```

### Comparing `azure-mgmt-hdinsightcontainers-1.0.0b1/azure/mgmt/hdinsightcontainers/models/_patch.py` & `azure-mgmt-hdinsightcontainers-1.0.0b2/azure/mgmt/hdinsightcontainers/models/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-hdinsightcontainers-1.0.0b1/azure/mgmt/hdinsightcontainers/operations/__init__.py` & `azure-mgmt-hdinsightcontainers-1.0.0b2/azure/mgmt/hdinsightcontainers/operations/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,28 +3,32 @@
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from ._cluster_pools_operations import ClusterPoolsOperations
+from ._cluster_pool_available_upgrades_operations import ClusterPoolAvailableUpgradesOperations
 from ._clusters_operations import ClustersOperations
+from ._cluster_available_upgrades_operations import ClusterAvailableUpgradesOperations
 from ._cluster_jobs_operations import ClusterJobsOperations
 from ._locations_operations import LocationsOperations
 from ._operations import Operations
 from ._available_cluster_pool_versions_operations import AvailableClusterPoolVersionsOperations
 from ._available_cluster_versions_operations import AvailableClusterVersionsOperations
 
 from ._patch import __all__ as _patch_all
 from ._patch import *  # pylint: disable=unused-wildcard-import
 from ._patch import patch_sdk as _patch_sdk
 
 __all__ = [
     "ClusterPoolsOperations",
+    "ClusterPoolAvailableUpgradesOperations",
     "ClustersOperations",
+    "ClusterAvailableUpgradesOperations",
     "ClusterJobsOperations",
     "LocationsOperations",
     "Operations",
     "AvailableClusterPoolVersionsOperations",
     "AvailableClusterVersionsOperations",
 ]
 __all__.extend([p for p in _patch_all if p not in __all__])
```

### Comparing `azure-mgmt-hdinsightcontainers-1.0.0b1/azure/mgmt/hdinsightcontainers/operations/_available_cluster_pool_versions_operations.py` & `azure-mgmt-hdinsightcontainers-1.0.0b2/azure/mgmt/hdinsightcontainers/operations/_available_cluster_versions_operations.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=too-many-lines
+# pylint: disable=too-many-lines,too-many-statements
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
@@ -36,21 +36,21 @@
 _SERIALIZER.client_side_validation = False
 
 
 def build_list_by_location_request(location: str, subscription_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-01-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-11-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
-        "/subscriptions/{subscriptionId}/providers/Microsoft.HDInsight/locations/{location}/availableClusterPoolVersions",
+        "/subscriptions/{subscriptionId}/providers/Microsoft.HDInsight/locations/{location}/availableClusterVersions",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
         "location": _SERIALIZER.url("location", location, "str", min_length=1),
     }
 
     _url: str = _url.format(**path_format_arguments)  # type: ignore
@@ -60,111 +60,105 @@
 
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
 
 
-class AvailableClusterPoolVersionsOperations:
+class AvailableClusterVersionsOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
         :class:`~azure.mgmt.hdinsightcontainers.HDInsightContainersMgmtClient`'s
-        :attr:`available_cluster_pool_versions` attribute.
+        :attr:`available_cluster_versions` attribute.
     """
 
     models = _models
 
     def __init__(self, *args, **kwargs):
         input_args = list(args)
         self._client = input_args.pop(0) if input_args else kwargs.pop("client")
         self._config = input_args.pop(0) if input_args else kwargs.pop("config")
         self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
         self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
 
     @distributed_trace
-    def list_by_location(self, location: str, **kwargs: Any) -> Iterable["_models.ClusterPoolVersion"]:
-        """Returns a list of available cluster pool versions.
+    def list_by_location(self, location: str, **kwargs: Any) -> Iterable["_models.ClusterVersion"]:
+        """Returns a list of available cluster versions.
 
         :param location: The name of the Azure region. Required.
         :type location: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: An iterator like instance of either ClusterPoolVersion or the result of cls(response)
-        :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.hdinsightcontainers.models.ClusterPoolVersion]
+        :return: An iterator like instance of either ClusterVersion or the result of cls(response)
+        :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.hdinsightcontainers.models.ClusterVersion]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
-        cls: ClsType[_models.ClusterPoolVersionsListResult] = kwargs.pop("cls", None)
+        cls: ClsType[_models.ClusterVersionsListResult] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         def prepare_request(next_link=None):
             if not next_link:
 
-                request = build_list_by_location_request(
+                _request = build_list_by_location_request(
                     location=location,
                     subscription_id=self._config.subscription_id,
                     api_version=api_version,
-                    template_url=self.list_by_location.metadata["url"],
                     headers=_headers,
                     params=_params,
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
 
             else:
                 # make call to next link with the client's api-version
                 _parsed_next_link = urllib.parse.urlparse(next_link)
                 _next_request_params = case_insensitive_dict(
                     {
                         key: [urllib.parse.quote(v) for v in value]
                         for key, value in urllib.parse.parse_qs(_parsed_next_link.query).items()
                     }
                 )
                 _next_request_params["api-version"] = self._config.api_version
-                request = HttpRequest(
+                _request = HttpRequest(
                     "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
-                request.method = "GET"
-            return request
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
+                _request.method = "GET"
+            return _request
 
         def extract_data(pipeline_response):
-            deserialized = self._deserialize("ClusterPoolVersionsListResult", pipeline_response)
+            deserialized = self._deserialize("ClusterVersionsListResult", pipeline_response)
             list_of_elem = deserialized.value
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, iter(list_of_elem)
 
         def get_next(next_link=None):
-            request = prepare_request(next_link)
+            _request = prepare_request(next_link)
 
             _stream = False
             pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=_stream, **kwargs
+                _request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
             return pipeline_response
 
         return ItemPaged(get_next, extract_data)
-
-    list_by_location.metadata = {
-        "url": "/subscriptions/{subscriptionId}/providers/Microsoft.HDInsight/locations/{location}/availableClusterPoolVersions"
-    }
```

### Comparing `azure-mgmt-hdinsightcontainers-1.0.0b1/azure/mgmt/hdinsightcontainers/operations/_available_cluster_versions_operations.py` & `azure-mgmt-hdinsightcontainers-1.0.0b2/azure/mgmt/hdinsightcontainers/operations/_cluster_pool_available_upgrades_operations.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=too-many-lines
+# pylint: disable=too-many-lines,too-many-statements
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
@@ -32,139 +32,146 @@
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
 
 _SERIALIZER = Serializer()
 _SERIALIZER.client_side_validation = False
 
 
-def build_list_by_location_request(location: str, subscription_id: str, **kwargs: Any) -> HttpRequest:
+def build_list_request(
+    resource_group_name: str, cluster_pool_name: str, subscription_id: str, **kwargs: Any
+) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-01-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-11-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
-        "/subscriptions/{subscriptionId}/providers/Microsoft.HDInsight/locations/{location}/availableClusterVersions",
+        "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HDInsight/clusterpools/{clusterPoolName}/availableUpgrades",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
-        "location": _SERIALIZER.url("location", location, "str", min_length=1),
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
+        ),
+        "clusterPoolName": _SERIALIZER.url("cluster_pool_name", cluster_pool_name, "str"),
     }
 
     _url: str = _url.format(**path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
 
 
-class AvailableClusterVersionsOperations:
+class ClusterPoolAvailableUpgradesOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
         :class:`~azure.mgmt.hdinsightcontainers.HDInsightContainersMgmtClient`'s
-        :attr:`available_cluster_versions` attribute.
+        :attr:`cluster_pool_available_upgrades` attribute.
     """
 
     models = _models
 
     def __init__(self, *args, **kwargs):
         input_args = list(args)
         self._client = input_args.pop(0) if input_args else kwargs.pop("client")
         self._config = input_args.pop(0) if input_args else kwargs.pop("config")
         self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
         self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
 
     @distributed_trace
-    def list_by_location(self, location: str, **kwargs: Any) -> Iterable["_models.ClusterVersion"]:
-        """Returns a list of available cluster versions.
-
-        :param location: The name of the Azure region. Required.
-        :type location: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: An iterator like instance of either ClusterVersion or the result of cls(response)
-        :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.hdinsightcontainers.models.ClusterVersion]
+    def list(
+        self, resource_group_name: str, cluster_pool_name: str, **kwargs: Any
+    ) -> Iterable["_models.ClusterPoolAvailableUpgrade"]:
+        """List a cluster pool available upgrade.
+
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
+        :type resource_group_name: str
+        :param cluster_pool_name: The name of the cluster pool. Required.
+        :type cluster_pool_name: str
+        :return: An iterator like instance of either ClusterPoolAvailableUpgrade or the result of
+         cls(response)
+        :rtype:
+         ~azure.core.paging.ItemPaged[~azure.mgmt.hdinsightcontainers.models.ClusterPoolAvailableUpgrade]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
-        cls: ClsType[_models.ClusterVersionsListResult] = kwargs.pop("cls", None)
+        cls: ClsType[_models.ClusterPoolAvailableUpgradeList] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         def prepare_request(next_link=None):
             if not next_link:
 
-                request = build_list_by_location_request(
-                    location=location,
+                _request = build_list_request(
+                    resource_group_name=resource_group_name,
+                    cluster_pool_name=cluster_pool_name,
                     subscription_id=self._config.subscription_id,
                     api_version=api_version,
-                    template_url=self.list_by_location.metadata["url"],
                     headers=_headers,
                     params=_params,
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
 
             else:
                 # make call to next link with the client's api-version
                 _parsed_next_link = urllib.parse.urlparse(next_link)
                 _next_request_params = case_insensitive_dict(
                     {
                         key: [urllib.parse.quote(v) for v in value]
                         for key, value in urllib.parse.parse_qs(_parsed_next_link.query).items()
                     }
                 )
                 _next_request_params["api-version"] = self._config.api_version
-                request = HttpRequest(
+                _request = HttpRequest(
                     "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
-                request.method = "GET"
-            return request
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
+                _request.method = "GET"
+            return _request
 
         def extract_data(pipeline_response):
-            deserialized = self._deserialize("ClusterVersionsListResult", pipeline_response)
+            deserialized = self._deserialize("ClusterPoolAvailableUpgradeList", pipeline_response)
             list_of_elem = deserialized.value
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, iter(list_of_elem)
 
         def get_next(next_link=None):
-            request = prepare_request(next_link)
+            _request = prepare_request(next_link)
 
             _stream = False
             pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=_stream, **kwargs
+                _request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
             return pipeline_response
 
         return ItemPaged(get_next, extract_data)
-
-    list_by_location.metadata = {
-        "url": "/subscriptions/{subscriptionId}/providers/Microsoft.HDInsight/locations/{location}/availableClusterVersions"
-    }
```

### Comparing `azure-mgmt-hdinsightcontainers-1.0.0b1/azure/mgmt/hdinsightcontainers/operations/_cluster_jobs_operations.py` & `azure-mgmt-hdinsightcontainers-1.0.0b2/azure/mgmt/hdinsightcontainers/aio/operations/_cluster_jobs_operations.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,144 +1,71 @@
-# pylint: disable=too-many-lines
+# pylint: disable=too-many-lines,too-many-statements
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 from io import IOBase
-from typing import Any, Callable, Dict, IO, Iterable, Optional, TypeVar, Union, cast, overload
+from typing import Any, AsyncIterable, Callable, Dict, IO, Optional, TypeVar, Union, cast, overload
 import urllib.parse
 
+from azure.core.async_paging import AsyncItemPaged, AsyncList
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
     ResourceNotFoundError,
     ResourceNotModifiedError,
     map_error,
 )
-from azure.core.paging import ItemPaged
 from azure.core.pipeline import PipelineResponse
-from azure.core.pipeline.transport import HttpResponse
-from azure.core.polling import LROPoller, NoPolling, PollingMethod
+from azure.core.pipeline.transport import AsyncHttpResponse
+from azure.core.polling import AsyncLROPoller, AsyncNoPolling, AsyncPollingMethod
 from azure.core.rest import HttpRequest
 from azure.core.tracing.decorator import distributed_trace
+from azure.core.tracing.decorator_async import distributed_trace_async
 from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
-from azure.mgmt.core.polling.arm_polling import ARMPolling
+from azure.mgmt.core.polling.async_arm_polling import AsyncARMPolling
 
-from .. import models as _models
-from .._serialization import Serializer
-from .._vendor import _convert_request
+from ... import models as _models
+from ..._vendor import _convert_request
+from ...operations._cluster_jobs_operations import build_list_request, build_run_job_request
 
 T = TypeVar("T")
-ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
-
-_SERIALIZER = Serializer()
-_SERIALIZER.client_side_validation = False
-
-
-def build_run_job_request(
-    resource_group_name: str, cluster_pool_name: str, cluster_name: str, subscription_id: str, **kwargs: Any
-) -> HttpRequest:
-    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
-    _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
-
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-01-preview"))
-    content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
-    accept = _headers.pop("Accept", "application/json")
-
-    # Construct URL
-    _url = kwargs.pop(
-        "template_url",
-        "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HDInsight/clusterpools/{clusterPoolName}/clusters/{clusterName}/runJob",
-    )  # pylint: disable=line-too-long
-    path_format_arguments = {
-        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
-        "resourceGroupName": _SERIALIZER.url(
-            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
-        ),
-        "clusterPoolName": _SERIALIZER.url("cluster_pool_name", cluster_pool_name, "str"),
-        "clusterName": _SERIALIZER.url("cluster_name", cluster_name, "str"),
-    }
-
-    _url: str = _url.format(**path_format_arguments)  # type: ignore
-
-    # Construct parameters
-    _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
-
-    # Construct headers
-    if content_type is not None:
-        _headers["Content-Type"] = _SERIALIZER.header("content_type", content_type, "str")
-    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
-
-    return HttpRequest(method="POST", url=_url, params=_params, headers=_headers, **kwargs)
-
-
-def build_list_request(
-    resource_group_name: str, cluster_pool_name: str, cluster_name: str, subscription_id: str, **kwargs: Any
-) -> HttpRequest:
-    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
-    _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
-
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-01-preview"))
-    accept = _headers.pop("Accept", "application/json")
-
-    # Construct URL
-    _url = kwargs.pop(
-        "template_url",
-        "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HDInsight/clusterpools/{clusterPoolName}/clusters/{clusterName}/jobs",
-    )  # pylint: disable=line-too-long
-    path_format_arguments = {
-        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
-        "resourceGroupName": _SERIALIZER.url(
-            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
-        ),
-        "clusterPoolName": _SERIALIZER.url("cluster_pool_name", cluster_pool_name, "str"),
-        "clusterName": _SERIALIZER.url("cluster_name", cluster_name, "str"),
-    }
-
-    _url: str = _url.format(**path_format_arguments)  # type: ignore
-
-    # Construct parameters
-    _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
-
-    # Construct headers
-    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
-
-    return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
+ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 
 class ClusterJobsOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
-        :class:`~azure.mgmt.hdinsightcontainers.HDInsightContainersMgmtClient`'s
+        :class:`~azure.mgmt.hdinsightcontainers.aio.HDInsightContainersMgmtClient`'s
         :attr:`cluster_jobs` attribute.
     """
 
     models = _models
 
-    def __init__(self, *args, **kwargs):
+    def __init__(self, *args, **kwargs) -> None:
         input_args = list(args)
         self._client = input_args.pop(0) if input_args else kwargs.pop("client")
         self._config = input_args.pop(0) if input_args else kwargs.pop("config")
         self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
         self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
 
-    def _run_job_initial(
+    async def _run_job_initial(
         self,
         resource_group_name: str,
         cluster_pool_name: str,
         cluster_name: str,
-        cluster_job: Union[_models.ClusterJob, IO],
+        cluster_job: Union[_models.ClusterJob, IO[bytes]],
         **kwargs: Any
     ) -> Optional[_models.ClusterJob]:
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -156,33 +83,32 @@
         _json = None
         _content = None
         if isinstance(cluster_job, (IOBase, bytes)):
             _content = cluster_job
         else:
             _json = self._serialize.body(cluster_job, "ClusterJob")
 
-        request = build_run_job_request(
+        _request = build_run_job_request(
             resource_group_name=resource_group_name,
             cluster_pool_name=cluster_pool_name,
             cluster_name=cluster_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             content_type=content_type,
             json=_json,
             content=_content,
-            template_url=self._run_job_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
-        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -193,144 +119,116 @@
         if response.status_code == 200:
             deserialized = self._deserialize("ClusterJob", pipeline_response)
 
         if response.status_code == 202:
             response_headers["location"] = self._deserialize("str", response.headers.get("location"))
 
         if cls:
-            return cls(pipeline_response, deserialized, response_headers)
-
-        return deserialized
+            return cls(pipeline_response, deserialized, response_headers)  # type: ignore
 
-    _run_job_initial.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HDInsight/clusterpools/{clusterPoolName}/clusters/{clusterName}/runJob"
-    }
+        return deserialized  # type: ignore
 
     @overload
-    def begin_run_job(
+    async def begin_run_job(
         self,
         resource_group_name: str,
         cluster_pool_name: str,
         cluster_name: str,
         cluster_job: _models.ClusterJob,
         *,
         content_type: str = "application/json",
         **kwargs: Any
-    ) -> LROPoller[_models.ClusterJob]:
+    ) -> AsyncLROPoller[_models.ClusterJob]:
         """Operations on jobs of HDInsight on AKS cluster.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param cluster_pool_name: The name of the cluster pool. Required.
         :type cluster_pool_name: str
         :param cluster_name: The name of the HDInsight cluster. Required.
         :type cluster_name: str
         :param cluster_job: The Cluster job. Required.
         :type cluster_job: ~azure.mgmt.hdinsightcontainers.models.ClusterJob
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
-         operation to not poll, or pass in your own initialized polling object for a personal polling
-         strategy.
-        :paramtype polling: bool or ~azure.core.polling.PollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
-        :return: An instance of LROPoller that returns either ClusterJob or the result of cls(response)
-        :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.hdinsightcontainers.models.ClusterJob]
+        :return: An instance of AsyncLROPoller that returns either ClusterJob or the result of
+         cls(response)
+        :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.hdinsightcontainers.models.ClusterJob]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
-    def begin_run_job(
+    async def begin_run_job(
         self,
         resource_group_name: str,
         cluster_pool_name: str,
         cluster_name: str,
-        cluster_job: IO,
+        cluster_job: IO[bytes],
         *,
         content_type: str = "application/json",
         **kwargs: Any
-    ) -> LROPoller[_models.ClusterJob]:
+    ) -> AsyncLROPoller[_models.ClusterJob]:
         """Operations on jobs of HDInsight on AKS cluster.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param cluster_pool_name: The name of the cluster pool. Required.
         :type cluster_pool_name: str
         :param cluster_name: The name of the HDInsight cluster. Required.
         :type cluster_name: str
         :param cluster_job: The Cluster job. Required.
-        :type cluster_job: IO
+        :type cluster_job: IO[bytes]
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
-         operation to not poll, or pass in your own initialized polling object for a personal polling
-         strategy.
-        :paramtype polling: bool or ~azure.core.polling.PollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
-        :return: An instance of LROPoller that returns either ClusterJob or the result of cls(response)
-        :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.hdinsightcontainers.models.ClusterJob]
+        :return: An instance of AsyncLROPoller that returns either ClusterJob or the result of
+         cls(response)
+        :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.hdinsightcontainers.models.ClusterJob]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
-    @distributed_trace
-    def begin_run_job(
+    @distributed_trace_async
+    async def begin_run_job(
         self,
         resource_group_name: str,
         cluster_pool_name: str,
         cluster_name: str,
-        cluster_job: Union[_models.ClusterJob, IO],
+        cluster_job: Union[_models.ClusterJob, IO[bytes]],
         **kwargs: Any
-    ) -> LROPoller[_models.ClusterJob]:
+    ) -> AsyncLROPoller[_models.ClusterJob]:
         """Operations on jobs of HDInsight on AKS cluster.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param cluster_pool_name: The name of the cluster pool. Required.
         :type cluster_pool_name: str
         :param cluster_name: The name of the HDInsight cluster. Required.
         :type cluster_name: str
-        :param cluster_job: The Cluster job. Is either a ClusterJob type or a IO type. Required.
-        :type cluster_job: ~azure.mgmt.hdinsightcontainers.models.ClusterJob or IO
-        :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
-         Default value is None.
-        :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
-         operation to not poll, or pass in your own initialized polling object for a personal polling
-         strategy.
-        :paramtype polling: bool or ~azure.core.polling.PollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
-        :return: An instance of LROPoller that returns either ClusterJob or the result of cls(response)
-        :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.hdinsightcontainers.models.ClusterJob]
+        :param cluster_job: The Cluster job. Is either a ClusterJob type or a IO[bytes] type. Required.
+        :type cluster_job: ~azure.mgmt.hdinsightcontainers.models.ClusterJob or IO[bytes]
+        :return: An instance of AsyncLROPoller that returns either ClusterJob or the result of
+         cls(response)
+        :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.hdinsightcontainers.models.ClusterJob]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.ClusterJob] = kwargs.pop("cls", None)
-        polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
+        polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
-            raw_result = self._run_job_initial(
+            raw_result = await self._run_job_initial(
                 resource_group_name=resource_group_name,
                 cluster_pool_name=cluster_pool_name,
                 cluster_name=cluster_name,
                 cluster_job=cluster_job,
                 api_version=api_version,
                 content_type=content_type,
                 cls=lambda x, y, z: x,
@@ -339,54 +237,60 @@
                 **kwargs
             )
         kwargs.pop("error_map", None)
 
         def get_long_running_output(pipeline_response):
             deserialized = self._deserialize("ClusterJob", pipeline_response)
             if cls:
-                return cls(pipeline_response, deserialized, {})
+                return cls(pipeline_response, deserialized, {})  # type: ignore
             return deserialized
 
         if polling is True:
-            polling_method: PollingMethod = cast(
-                PollingMethod, ARMPolling(lro_delay, lro_options={"final-state-via": "location"}, **kwargs)
+            polling_method: AsyncPollingMethod = cast(
+                AsyncPollingMethod, AsyncARMPolling(lro_delay, lro_options={"final-state-via": "location"}, **kwargs)
             )
         elif polling is False:
-            polling_method = cast(PollingMethod, NoPolling())
+            polling_method = cast(AsyncPollingMethod, AsyncNoPolling())
         else:
             polling_method = polling
         if cont_token:
-            return LROPoller.from_continuation_token(
+            return AsyncLROPoller[_models.ClusterJob].from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
                 deserialization_callback=get_long_running_output,
             )
-        return LROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
-
-    begin_run_job.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HDInsight/clusterpools/{clusterPoolName}/clusters/{clusterName}/runJob"
-    }
+        return AsyncLROPoller[_models.ClusterJob](
+            self._client, raw_result, get_long_running_output, polling_method  # type: ignore
+        )
 
     @distributed_trace
     def list(
-        self, resource_group_name: str, cluster_pool_name: str, cluster_name: str, **kwargs: Any
-    ) -> Iterable["_models.ClusterJob"]:
+        self,
+        resource_group_name: str,
+        cluster_pool_name: str,
+        cluster_name: str,
+        filter: Optional[str] = None,
+        **kwargs: Any
+    ) -> AsyncIterable["_models.ClusterJob"]:
         """Get jobs of HDInsight on AKS cluster.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param cluster_pool_name: The name of the cluster pool. Required.
         :type cluster_pool_name: str
         :param cluster_name: The name of the HDInsight cluster. Required.
         :type cluster_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
+        :param filter: The system query option to filter job returned in the response. Allowed value is
+         'jobName eq {jobName}' or 'jarName eq {jarName}'. Default value is None.
+        :type filter: str
         :return: An iterator like instance of either ClusterJob or the result of cls(response)
-        :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.hdinsightcontainers.models.ClusterJob]
+        :rtype:
+         ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.hdinsightcontainers.models.ClusterJob]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.ClusterJobList] = kwargs.pop("cls", None)
@@ -398,66 +302,62 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         def prepare_request(next_link=None):
             if not next_link:
 
-                request = build_list_request(
+                _request = build_list_request(
                     resource_group_name=resource_group_name,
                     cluster_pool_name=cluster_pool_name,
                     cluster_name=cluster_name,
                     subscription_id=self._config.subscription_id,
+                    filter=filter,
                     api_version=api_version,
-                    template_url=self.list.metadata["url"],
                     headers=_headers,
                     params=_params,
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
 
             else:
                 # make call to next link with the client's api-version
                 _parsed_next_link = urllib.parse.urlparse(next_link)
                 _next_request_params = case_insensitive_dict(
                     {
                         key: [urllib.parse.quote(v) for v in value]
                         for key, value in urllib.parse.parse_qs(_parsed_next_link.query).items()
                     }
                 )
                 _next_request_params["api-version"] = self._config.api_version
-                request = HttpRequest(
+                _request = HttpRequest(
                     "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
-                request.method = "GET"
-            return request
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
+                _request.method = "GET"
+            return _request
 
-        def extract_data(pipeline_response):
+        async def extract_data(pipeline_response):
             deserialized = self._deserialize("ClusterJobList", pipeline_response)
             list_of_elem = deserialized.value
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
-            return deserialized.next_link or None, iter(list_of_elem)
+            return deserialized.next_link or None, AsyncList(list_of_elem)
 
-        def get_next(next_link=None):
-            request = prepare_request(next_link)
+        async def get_next(next_link=None):
+            _request = prepare_request(next_link)
 
             _stream = False
-            pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=_stream, **kwargs
+            pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+                _request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
             return pipeline_response
 
-        return ItemPaged(get_next, extract_data)
-
-    list.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HDInsight/clusterpools/{clusterPoolName}/clusters/{clusterName}/jobs"
-    }
+        return AsyncItemPaged(get_next, extract_data)
```

### Comparing `azure-mgmt-hdinsightcontainers-1.0.0b1/azure/mgmt/hdinsightcontainers/operations/_cluster_pools_operations.py` & `azure-mgmt-hdinsightcontainers-1.0.0b2/azure/mgmt/hdinsightcontainers/operations/_cluster_pools_operations.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=too-many-lines
+# pylint: disable=too-many-lines,too-many-statements
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
@@ -41,15 +41,15 @@
 
 def build_get_request(
     resource_group_name: str, cluster_pool_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-01-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-11-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HDInsight/clusterpools/{clusterPoolName}",
     )  # pylint: disable=line-too-long
@@ -74,15 +74,15 @@
 
 def build_create_or_update_request(
     resource_group_name: str, cluster_pool_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-01-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-11-01-preview"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HDInsight/clusterpools/{clusterPoolName}",
@@ -110,15 +110,15 @@
 
 def build_update_tags_request(
     resource_group_name: str, cluster_pool_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-01-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-11-01-preview"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HDInsight/clusterpools/{clusterPoolName}",
@@ -146,15 +146,15 @@
 
 def build_delete_request(
     resource_group_name: str, cluster_pool_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-01-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-11-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HDInsight/clusterpools/{clusterPoolName}",
     )  # pylint: disable=line-too-long
@@ -177,15 +177,15 @@
     return HttpRequest(method="DELETE", url=_url, params=_params, headers=_headers, **kwargs)
 
 
 def build_list_by_subscription_request(subscription_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-01-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-11-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop("template_url", "/subscriptions/{subscriptionId}/providers/Microsoft.HDInsight/clusterpools")
     path_format_arguments = {
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
     }
@@ -201,15 +201,15 @@
     return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
 
 
 def build_list_by_resource_group_request(resource_group_name: str, subscription_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-01-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-11-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HDInsight/clusterpools",
     )  # pylint: disable=line-too-long
@@ -227,14 +227,50 @@
 
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
 
 
+def build_upgrade_request(
+    resource_group_name: str, cluster_pool_name: str, subscription_id: str, **kwargs: Any
+) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+    _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-11-01-preview"))
+    content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+    accept = _headers.pop("Accept", "application/json")
+
+    # Construct URL
+    _url = kwargs.pop(
+        "template_url",
+        "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HDInsight/clusterpools/{clusterPoolName}/upgrade",
+    )  # pylint: disable=line-too-long
+    path_format_arguments = {
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
+        ),
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
+        "clusterPoolName": _SERIALIZER.url("cluster_pool_name", cluster_pool_name, "str"),
+    }
+
+    _url: str = _url.format(**path_format_arguments)  # type: ignore
+
+    # Construct parameters
+    _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
+
+    # Construct headers
+    if content_type is not None:
+        _headers["Content-Type"] = _SERIALIZER.header("content_type", content_type, "str")
+    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
+
+    return HttpRequest(method="POST", url=_url, params=_params, headers=_headers, **kwargs)
+
+
 class ClusterPoolsOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
         :class:`~azure.mgmt.hdinsightcontainers.HDInsightContainersMgmtClient`'s
@@ -255,15 +291,14 @@
         """Gets a cluster pool.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param cluster_pool_name: The name of the cluster pool. Required.
         :type cluster_pool_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: ClusterPool or the result of cls(response)
         :rtype: ~azure.mgmt.hdinsightcontainers.models.ClusterPool
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -274,54 +309,49 @@
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.ClusterPool] = kwargs.pop("cls", None)
 
-        request = build_get_request(
+        _request = build_get_request(
             resource_group_name=resource_group_name,
             cluster_pool_name=cluster_pool_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
-            template_url=self.get.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         deserialized = self._deserialize("ClusterPool", pipeline_response)
 
         if cls:
-            return cls(pipeline_response, deserialized, {})
-
-        return deserialized
+            return cls(pipeline_response, deserialized, {})  # type: ignore
 
-    get.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HDInsight/clusterpools/{clusterPoolName}"
-    }
+        return deserialized  # type: ignore
 
     def _create_or_update_initial(
         self,
         resource_group_name: str,
         cluster_pool_name: str,
-        cluster_pool: Union[_models.ClusterPool, IO],
+        cluster_pool: Union[_models.ClusterPool, IO[bytes]],
         **kwargs: Any
     ) -> _models.ClusterPool:
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -339,32 +369,31 @@
         _json = None
         _content = None
         if isinstance(cluster_pool, (IOBase, bytes)):
             _content = cluster_pool
         else:
             _json = self._serialize.body(cluster_pool, "ClusterPool")
 
-        request = build_create_or_update_request(
+        _request = build_create_or_update_request(
             resource_group_name=resource_group_name,
             cluster_pool_name=cluster_pool_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             content_type=content_type,
             json=_json,
             content=_content,
-            template_url=self._create_or_update_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 201]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -377,18 +406,14 @@
             deserialized = self._deserialize("ClusterPool", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})  # type: ignore
 
         return deserialized  # type: ignore
 
-    _create_or_update_initial.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HDInsight/clusterpools/{clusterPoolName}"
-    }
-
     @overload
     def begin_create_or_update(
         self,
         resource_group_name: str,
         cluster_pool_name: str,
         cluster_pool: _models.ClusterPool,
         *,
@@ -403,93 +428,66 @@
         :param cluster_pool_name: The name of the cluster pool. Required.
         :type cluster_pool_name: str
         :param cluster_pool: The Cluster Pool to create. Required.
         :type cluster_pool: ~azure.mgmt.hdinsightcontainers.models.ClusterPool
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
-         operation to not poll, or pass in your own initialized polling object for a personal polling
-         strategy.
-        :paramtype polling: bool or ~azure.core.polling.PollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
         :return: An instance of LROPoller that returns either ClusterPool or the result of
          cls(response)
         :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.hdinsightcontainers.models.ClusterPool]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
     def begin_create_or_update(
         self,
         resource_group_name: str,
         cluster_pool_name: str,
-        cluster_pool: IO,
+        cluster_pool: IO[bytes],
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> LROPoller[_models.ClusterPool]:
         """Creates or updates a cluster pool.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param cluster_pool_name: The name of the cluster pool. Required.
         :type cluster_pool_name: str
         :param cluster_pool: The Cluster Pool to create. Required.
-        :type cluster_pool: IO
+        :type cluster_pool: IO[bytes]
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
-         operation to not poll, or pass in your own initialized polling object for a personal polling
-         strategy.
-        :paramtype polling: bool or ~azure.core.polling.PollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
         :return: An instance of LROPoller that returns either ClusterPool or the result of
          cls(response)
         :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.hdinsightcontainers.models.ClusterPool]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace
     def begin_create_or_update(
         self,
         resource_group_name: str,
         cluster_pool_name: str,
-        cluster_pool: Union[_models.ClusterPool, IO],
+        cluster_pool: Union[_models.ClusterPool, IO[bytes]],
         **kwargs: Any
     ) -> LROPoller[_models.ClusterPool]:
         """Creates or updates a cluster pool.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param cluster_pool_name: The name of the cluster pool. Required.
         :type cluster_pool_name: str
-        :param cluster_pool: The Cluster Pool to create. Is either a ClusterPool type or a IO type.
-         Required.
-        :type cluster_pool: ~azure.mgmt.hdinsightcontainers.models.ClusterPool or IO
-        :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
-         Default value is None.
-        :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
-         operation to not poll, or pass in your own initialized polling object for a personal polling
-         strategy.
-        :paramtype polling: bool or ~azure.core.polling.PollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
+        :param cluster_pool: The Cluster Pool to create. Is either a ClusterPool type or a IO[bytes]
+         type. Required.
+        :type cluster_pool: ~azure.mgmt.hdinsightcontainers.models.ClusterPool or IO[bytes]
         :return: An instance of LROPoller that returns either ClusterPool or the result of
          cls(response)
         :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.hdinsightcontainers.models.ClusterPool]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
@@ -513,43 +511,41 @@
                 **kwargs
             )
         kwargs.pop("error_map", None)
 
         def get_long_running_output(pipeline_response):
             deserialized = self._deserialize("ClusterPool", pipeline_response)
             if cls:
-                return cls(pipeline_response, deserialized, {})
+                return cls(pipeline_response, deserialized, {})  # type: ignore
             return deserialized
 
         if polling is True:
             polling_method: PollingMethod = cast(
                 PollingMethod, ARMPolling(lro_delay, lro_options={"final-state-via": "azure-async-operation"}, **kwargs)
             )
         elif polling is False:
             polling_method = cast(PollingMethod, NoPolling())
         else:
             polling_method = polling
         if cont_token:
-            return LROPoller.from_continuation_token(
+            return LROPoller[_models.ClusterPool].from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
                 deserialization_callback=get_long_running_output,
             )
-        return LROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
-
-    begin_create_or_update.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HDInsight/clusterpools/{clusterPoolName}"
-    }
+        return LROPoller[_models.ClusterPool](
+            self._client, raw_result, get_long_running_output, polling_method  # type: ignore
+        )
 
     def _update_tags_initial(
         self,
         resource_group_name: str,
         cluster_pool_name: str,
-        cluster_pool_tags: Union[_models.TagsObject, IO],
+        cluster_pool_tags: Union[_models.TagsObject, IO[bytes]],
         **kwargs: Any
     ) -> _models.ClusterPool:
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -567,32 +563,31 @@
         _json = None
         _content = None
         if isinstance(cluster_pool_tags, (IOBase, bytes)):
             _content = cluster_pool_tags
         else:
             _json = self._serialize.body(cluster_pool_tags, "TagsObject")
 
-        request = build_update_tags_request(
+        _request = build_update_tags_request(
             resource_group_name=resource_group_name,
             cluster_pool_name=cluster_pool_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             content_type=content_type,
             json=_json,
             content=_content,
-            template_url=self._update_tags_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -608,18 +603,14 @@
             deserialized = self._deserialize("ClusterPool", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, response_headers)  # type: ignore
 
         return deserialized  # type: ignore
 
-    _update_tags_initial.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HDInsight/clusterpools/{clusterPoolName}"
-    }
-
     @overload
     def begin_update_tags(
         self,
         resource_group_name: str,
         cluster_pool_name: str,
         cluster_pool_tags: _models.TagsObject,
         *,
@@ -634,93 +625,66 @@
         :param cluster_pool_name: The name of the cluster pool. Required.
         :type cluster_pool_name: str
         :param cluster_pool_tags: Parameters supplied to update tags. Required.
         :type cluster_pool_tags: ~azure.mgmt.hdinsightcontainers.models.TagsObject
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
-         operation to not poll, or pass in your own initialized polling object for a personal polling
-         strategy.
-        :paramtype polling: bool or ~azure.core.polling.PollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
         :return: An instance of LROPoller that returns either ClusterPool or the result of
          cls(response)
         :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.hdinsightcontainers.models.ClusterPool]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
     def begin_update_tags(
         self,
         resource_group_name: str,
         cluster_pool_name: str,
-        cluster_pool_tags: IO,
+        cluster_pool_tags: IO[bytes],
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> LROPoller[_models.ClusterPool]:
         """Updates an existing Cluster Pool Tags.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param cluster_pool_name: The name of the cluster pool. Required.
         :type cluster_pool_name: str
         :param cluster_pool_tags: Parameters supplied to update tags. Required.
-        :type cluster_pool_tags: IO
+        :type cluster_pool_tags: IO[bytes]
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
-         operation to not poll, or pass in your own initialized polling object for a personal polling
-         strategy.
-        :paramtype polling: bool or ~azure.core.polling.PollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
         :return: An instance of LROPoller that returns either ClusterPool or the result of
          cls(response)
         :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.hdinsightcontainers.models.ClusterPool]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace
     def begin_update_tags(
         self,
         resource_group_name: str,
         cluster_pool_name: str,
-        cluster_pool_tags: Union[_models.TagsObject, IO],
+        cluster_pool_tags: Union[_models.TagsObject, IO[bytes]],
         **kwargs: Any
     ) -> LROPoller[_models.ClusterPool]:
         """Updates an existing Cluster Pool Tags.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param cluster_pool_name: The name of the cluster pool. Required.
         :type cluster_pool_name: str
         :param cluster_pool_tags: Parameters supplied to update tags. Is either a TagsObject type or a
-         IO type. Required.
-        :type cluster_pool_tags: ~azure.mgmt.hdinsightcontainers.models.TagsObject or IO
-        :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
-         Default value is None.
-        :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
-         operation to not poll, or pass in your own initialized polling object for a personal polling
-         strategy.
-        :paramtype polling: bool or ~azure.core.polling.PollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
+         IO[bytes] type. Required.
+        :type cluster_pool_tags: ~azure.mgmt.hdinsightcontainers.models.TagsObject or IO[bytes]
         :return: An instance of LROPoller that returns either ClusterPool or the result of
          cls(response)
         :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.hdinsightcontainers.models.ClusterPool]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
@@ -744,37 +708,35 @@
                 **kwargs
             )
         kwargs.pop("error_map", None)
 
         def get_long_running_output(pipeline_response):
             deserialized = self._deserialize("ClusterPool", pipeline_response)
             if cls:
-                return cls(pipeline_response, deserialized, {})
+                return cls(pipeline_response, deserialized, {})  # type: ignore
             return deserialized
 
         if polling is True:
             polling_method: PollingMethod = cast(
                 PollingMethod, ARMPolling(lro_delay, lro_options={"final-state-via": "azure-async-operation"}, **kwargs)
             )
         elif polling is False:
             polling_method = cast(PollingMethod, NoPolling())
         else:
             polling_method = polling
         if cont_token:
-            return LROPoller.from_continuation_token(
+            return LROPoller[_models.ClusterPool].from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
                 deserialization_callback=get_long_running_output,
             )
-        return LROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
-
-    begin_update_tags.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HDInsight/clusterpools/{clusterPoolName}"
-    }
+        return LROPoller[_models.ClusterPool](
+            self._client, raw_result, get_long_running_output, polling_method  # type: ignore
+        )
 
     def _delete_initial(  # pylint: disable=inconsistent-return-statements
         self, resource_group_name: str, cluster_pool_name: str, **kwargs: Any
     ) -> None:
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -785,66 +747,53 @@
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
-        request = build_delete_request(
+        _request = build_delete_request(
             resource_group_name=resource_group_name,
             cluster_pool_name=cluster_pool_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
-            template_url=self._delete_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         response_headers = {}
         if response.status_code == 202:
             response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
 
         if cls:
-            return cls(pipeline_response, None, response_headers)
-
-    _delete_initial.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HDInsight/clusterpools/{clusterPoolName}"
-    }
+            return cls(pipeline_response, None, response_headers)  # type: ignore
 
     @distributed_trace
     def begin_delete(self, resource_group_name: str, cluster_pool_name: str, **kwargs: Any) -> LROPoller[None]:
         """Deletes a Cluster Pool.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param cluster_pool_name: The name of the cluster pool. Required.
         :type cluster_pool_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
-         operation to not poll, or pass in your own initialized polling object for a personal polling
-         strategy.
-        :paramtype polling: bool or ~azure.core.polling.PollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
         :return: An instance of LROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.LROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
@@ -863,40 +812,35 @@
                 params=_params,
                 **kwargs
             )
         kwargs.pop("error_map", None)
 
         def get_long_running_output(pipeline_response):  # pylint: disable=inconsistent-return-statements
             if cls:
-                return cls(pipeline_response, None, {})
+                return cls(pipeline_response, None, {})  # type: ignore
 
         if polling is True:
             polling_method: PollingMethod = cast(PollingMethod, ARMPolling(lro_delay, **kwargs))
         elif polling is False:
             polling_method = cast(PollingMethod, NoPolling())
         else:
             polling_method = polling
         if cont_token:
-            return LROPoller.from_continuation_token(
+            return LROPoller[None].from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
                 deserialization_callback=get_long_running_output,
             )
-        return LROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
-
-    begin_delete.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HDInsight/clusterpools/{clusterPoolName}"
-    }
+        return LROPoller[None](self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
 
     @distributed_trace
     def list_by_subscription(self, **kwargs: Any) -> Iterable["_models.ClusterPool"]:
         """Gets the list of Cluster Pools within a Subscription.
 
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either ClusterPool or the result of cls(response)
         :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.hdinsightcontainers.models.ClusterPool]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
@@ -910,79 +854,73 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         def prepare_request(next_link=None):
             if not next_link:
 
-                request = build_list_by_subscription_request(
+                _request = build_list_by_subscription_request(
                     subscription_id=self._config.subscription_id,
                     api_version=api_version,
-                    template_url=self.list_by_subscription.metadata["url"],
                     headers=_headers,
                     params=_params,
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
 
             else:
                 # make call to next link with the client's api-version
                 _parsed_next_link = urllib.parse.urlparse(next_link)
                 _next_request_params = case_insensitive_dict(
                     {
                         key: [urllib.parse.quote(v) for v in value]
                         for key, value in urllib.parse.parse_qs(_parsed_next_link.query).items()
                     }
                 )
                 _next_request_params["api-version"] = self._config.api_version
-                request = HttpRequest(
+                _request = HttpRequest(
                     "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
-                request.method = "GET"
-            return request
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
+                _request.method = "GET"
+            return _request
 
         def extract_data(pipeline_response):
             deserialized = self._deserialize("ClusterPoolListResult", pipeline_response)
             list_of_elem = deserialized.value
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, iter(list_of_elem)
 
         def get_next(next_link=None):
-            request = prepare_request(next_link)
+            _request = prepare_request(next_link)
 
             _stream = False
             pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=_stream, **kwargs
+                _request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
             return pipeline_response
 
         return ItemPaged(get_next, extract_data)
 
-    list_by_subscription.metadata = {
-        "url": "/subscriptions/{subscriptionId}/providers/Microsoft.HDInsight/clusterpools"
-    }
-
     @distributed_trace
     def list_by_resource_group(self, resource_group_name: str, **kwargs: Any) -> Iterable["_models.ClusterPool"]:
         """Lists the HDInsight cluster pools under a resource group.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either ClusterPool or the result of cls(response)
         :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.hdinsightcontainers.models.ClusterPool]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
@@ -996,64 +934,256 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         def prepare_request(next_link=None):
             if not next_link:
 
-                request = build_list_by_resource_group_request(
+                _request = build_list_by_resource_group_request(
                     resource_group_name=resource_group_name,
                     subscription_id=self._config.subscription_id,
                     api_version=api_version,
-                    template_url=self.list_by_resource_group.metadata["url"],
                     headers=_headers,
                     params=_params,
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
 
             else:
                 # make call to next link with the client's api-version
                 _parsed_next_link = urllib.parse.urlparse(next_link)
                 _next_request_params = case_insensitive_dict(
                     {
                         key: [urllib.parse.quote(v) for v in value]
                         for key, value in urllib.parse.parse_qs(_parsed_next_link.query).items()
                     }
                 )
                 _next_request_params["api-version"] = self._config.api_version
-                request = HttpRequest(
+                _request = HttpRequest(
                     "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
-                request.method = "GET"
-            return request
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
+                _request.method = "GET"
+            return _request
 
         def extract_data(pipeline_response):
             deserialized = self._deserialize("ClusterPoolListResult", pipeline_response)
             list_of_elem = deserialized.value
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, iter(list_of_elem)
 
         def get_next(next_link=None):
-            request = prepare_request(next_link)
+            _request = prepare_request(next_link)
 
             _stream = False
             pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=_stream, **kwargs
+                _request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
             return pipeline_response
 
         return ItemPaged(get_next, extract_data)
 
-    list_by_resource_group.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HDInsight/clusterpools"
-    }
+    def _upgrade_initial(
+        self,
+        resource_group_name: str,
+        cluster_pool_name: str,
+        cluster_pool_upgrade_request: Union[_models.ClusterPoolUpgrade, IO[bytes]],
+        **kwargs: Any
+    ) -> Optional[_models.ClusterPool]:
+        error_map = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[Optional[_models.ClusterPool]] = kwargs.pop("cls", None)
+
+        content_type = content_type or "application/json"
+        _json = None
+        _content = None
+        if isinstance(cluster_pool_upgrade_request, (IOBase, bytes)):
+            _content = cluster_pool_upgrade_request
+        else:
+            _json = self._serialize.body(cluster_pool_upgrade_request, "ClusterPoolUpgrade")
+
+        _request = build_upgrade_request(
+            resource_group_name=resource_group_name,
+            cluster_pool_name=cluster_pool_name,
+            subscription_id=self._config.subscription_id,
+            api_version=api_version,
+            content_type=content_type,
+            json=_json,
+            content=_content,
+            headers=_headers,
+            params=_params,
+        )
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+            _request, stream=_stream, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200, 202]:
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
+            raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
+
+        deserialized = None
+        response_headers = {}
+        if response.status_code == 200:
+            deserialized = self._deserialize("ClusterPool", pipeline_response)
+
+        if response.status_code == 202:
+            response_headers["location"] = self._deserialize("str", response.headers.get("location"))
+
+        if cls:
+            return cls(pipeline_response, deserialized, response_headers)  # type: ignore
+
+        return deserialized  # type: ignore
+
+    @overload
+    def begin_upgrade(
+        self,
+        resource_group_name: str,
+        cluster_pool_name: str,
+        cluster_pool_upgrade_request: _models.ClusterPoolUpgrade,
+        *,
+        content_type: str = "application/json",
+        **kwargs: Any
+    ) -> LROPoller[_models.ClusterPool]:
+        """Upgrade a cluster pool.
+
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
+        :type resource_group_name: str
+        :param cluster_pool_name: The name of the cluster pool. Required.
+        :type cluster_pool_name: str
+        :param cluster_pool_upgrade_request: Upgrade a cluster pool. Required.
+        :type cluster_pool_upgrade_request: ~azure.mgmt.hdinsightcontainers.models.ClusterPoolUpgrade
+        :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: An instance of LROPoller that returns either ClusterPool or the result of
+         cls(response)
+        :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.hdinsightcontainers.models.ClusterPool]
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @overload
+    def begin_upgrade(
+        self,
+        resource_group_name: str,
+        cluster_pool_name: str,
+        cluster_pool_upgrade_request: IO[bytes],
+        *,
+        content_type: str = "application/json",
+        **kwargs: Any
+    ) -> LROPoller[_models.ClusterPool]:
+        """Upgrade a cluster pool.
+
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
+        :type resource_group_name: str
+        :param cluster_pool_name: The name of the cluster pool. Required.
+        :type cluster_pool_name: str
+        :param cluster_pool_upgrade_request: Upgrade a cluster pool. Required.
+        :type cluster_pool_upgrade_request: IO[bytes]
+        :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: An instance of LROPoller that returns either ClusterPool or the result of
+         cls(response)
+        :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.hdinsightcontainers.models.ClusterPool]
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @distributed_trace
+    def begin_upgrade(
+        self,
+        resource_group_name: str,
+        cluster_pool_name: str,
+        cluster_pool_upgrade_request: Union[_models.ClusterPoolUpgrade, IO[bytes]],
+        **kwargs: Any
+    ) -> LROPoller[_models.ClusterPool]:
+        """Upgrade a cluster pool.
+
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
+        :type resource_group_name: str
+        :param cluster_pool_name: The name of the cluster pool. Required.
+        :type cluster_pool_name: str
+        :param cluster_pool_upgrade_request: Upgrade a cluster pool. Is either a ClusterPoolUpgrade
+         type or a IO[bytes] type. Required.
+        :type cluster_pool_upgrade_request: ~azure.mgmt.hdinsightcontainers.models.ClusterPoolUpgrade
+         or IO[bytes]
+        :return: An instance of LROPoller that returns either ClusterPool or the result of
+         cls(response)
+        :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.hdinsightcontainers.models.ClusterPool]
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[_models.ClusterPool] = kwargs.pop("cls", None)
+        polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
+        lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
+        cont_token: Optional[str] = kwargs.pop("continuation_token", None)
+        if cont_token is None:
+            raw_result = self._upgrade_initial(
+                resource_group_name=resource_group_name,
+                cluster_pool_name=cluster_pool_name,
+                cluster_pool_upgrade_request=cluster_pool_upgrade_request,
+                api_version=api_version,
+                content_type=content_type,
+                cls=lambda x, y, z: x,
+                headers=_headers,
+                params=_params,
+                **kwargs
+            )
+        kwargs.pop("error_map", None)
+
+        def get_long_running_output(pipeline_response):
+            deserialized = self._deserialize("ClusterPool", pipeline_response)
+            if cls:
+                return cls(pipeline_response, deserialized, {})  # type: ignore
+            return deserialized
+
+        if polling is True:
+            polling_method: PollingMethod = cast(
+                PollingMethod, ARMPolling(lro_delay, lro_options={"final-state-via": "location"}, **kwargs)
+            )
+        elif polling is False:
+            polling_method = cast(PollingMethod, NoPolling())
+        else:
+            polling_method = polling
+        if cont_token:
+            return LROPoller[_models.ClusterPool].from_continuation_token(
+                polling_method=polling_method,
+                continuation_token=cont_token,
+                client=self._client,
+                deserialization_callback=get_long_running_output,
+            )
+        return LROPoller[_models.ClusterPool](
+            self._client, raw_result, get_long_running_output, polling_method  # type: ignore
+        )
```

### Comparing `azure-mgmt-hdinsightcontainers-1.0.0b1/azure/mgmt/hdinsightcontainers/operations/_clusters_operations.py` & `azure-mgmt-hdinsightcontainers-1.0.0b2/azure/mgmt/hdinsightcontainers/operations/_clusters_operations.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=too-many-lines
+# pylint: disable=too-many-lines,too-many-statements
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
@@ -41,15 +41,15 @@
 
 def build_list_by_cluster_pool_name_request(
     resource_group_name: str, cluster_pool_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-01-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-11-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HDInsight/clusterpools/{clusterPoolName}/clusters",
     )  # pylint: disable=line-too-long
@@ -68,21 +68,58 @@
 
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
 
 
+def build_upgrade_request(
+    resource_group_name: str, cluster_pool_name: str, cluster_name: str, subscription_id: str, **kwargs: Any
+) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+    _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-11-01-preview"))
+    content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+    accept = _headers.pop("Accept", "application/json")
+
+    # Construct URL
+    _url = kwargs.pop(
+        "template_url",
+        "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HDInsight/clusterpools/{clusterPoolName}/clusters/{clusterName}/upgrade",
+    )  # pylint: disable=line-too-long
+    path_format_arguments = {
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
+        ),
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
+        "clusterPoolName": _SERIALIZER.url("cluster_pool_name", cluster_pool_name, "str"),
+        "clusterName": _SERIALIZER.url("cluster_name", cluster_name, "str"),
+    }
+
+    _url: str = _url.format(**path_format_arguments)  # type: ignore
+
+    # Construct parameters
+    _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
+
+    # Construct headers
+    if content_type is not None:
+        _headers["Content-Type"] = _SERIALIZER.header("content_type", content_type, "str")
+    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
+
+    return HttpRequest(method="POST", url=_url, params=_params, headers=_headers, **kwargs)
+
+
 def build_resize_request(
     resource_group_name: str, cluster_pool_name: str, cluster_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-01-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-11-01-preview"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HDInsight/clusterpools/{clusterPoolName}/clusters/{clusterName}/resize",
@@ -111,15 +148,15 @@
 
 def build_get_request(
     resource_group_name: str, cluster_pool_name: str, cluster_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-01-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-11-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HDInsight/clusterpools/{clusterPoolName}/clusters/{clusterName}",
     )  # pylint: disable=line-too-long
@@ -145,15 +182,15 @@
 
 def build_create_request(
     resource_group_name: str, cluster_pool_name: str, cluster_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-01-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-11-01-preview"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HDInsight/clusterpools/{clusterPoolName}/clusters/{clusterName}",
@@ -182,15 +219,15 @@
 
 def build_update_request(
     resource_group_name: str, cluster_pool_name: str, cluster_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-01-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-11-01-preview"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HDInsight/clusterpools/{clusterPoolName}/clusters/{clusterName}",
@@ -219,15 +256,15 @@
 
 def build_delete_request(
     resource_group_name: str, cluster_pool_name: str, cluster_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-01-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-11-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HDInsight/clusterpools/{clusterPoolName}/clusters/{clusterName}",
     )  # pylint: disable=line-too-long
@@ -253,15 +290,15 @@
 
 def build_list_service_configs_request(
     resource_group_name: str, cluster_pool_name: str, cluster_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-01-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-11-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HDInsight/clusterpools/{clusterPoolName}/clusters/{clusterName}/serviceConfigs",
     )  # pylint: disable=line-too-long
@@ -287,15 +324,15 @@
 
 def build_list_instance_views_request(
     resource_group_name: str, cluster_pool_name: str, cluster_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-01-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-11-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HDInsight/clusterpools/{clusterPoolName}/clusters/{clusterName}/instanceViews",
     )  # pylint: disable=line-too-long
@@ -321,15 +358,15 @@
 
 def build_get_instance_view_request(
     resource_group_name: str, cluster_pool_name: str, cluster_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-01-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-11-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HDInsight/clusterpools/{clusterPoolName}/clusters/{clusterName}/instanceViews/default",
     )  # pylint: disable=line-too-long
@@ -379,15 +416,14 @@
         """Lists the HDInsight cluster pools under a resource group.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param cluster_pool_name: The name of the cluster pool. Required.
         :type cluster_pool_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either Cluster or the result of cls(response)
         :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.hdinsightcontainers.models.Cluster]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
@@ -401,79 +437,280 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         def prepare_request(next_link=None):
             if not next_link:
 
-                request = build_list_by_cluster_pool_name_request(
+                _request = build_list_by_cluster_pool_name_request(
                     resource_group_name=resource_group_name,
                     cluster_pool_name=cluster_pool_name,
                     subscription_id=self._config.subscription_id,
                     api_version=api_version,
-                    template_url=self.list_by_cluster_pool_name.metadata["url"],
                     headers=_headers,
                     params=_params,
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
 
             else:
                 # make call to next link with the client's api-version
                 _parsed_next_link = urllib.parse.urlparse(next_link)
                 _next_request_params = case_insensitive_dict(
                     {
                         key: [urllib.parse.quote(v) for v in value]
                         for key, value in urllib.parse.parse_qs(_parsed_next_link.query).items()
                     }
                 )
                 _next_request_params["api-version"] = self._config.api_version
-                request = HttpRequest(
+                _request = HttpRequest(
                     "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
-                request.method = "GET"
-            return request
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
+                _request.method = "GET"
+            return _request
 
         def extract_data(pipeline_response):
             deserialized = self._deserialize("ClusterListResult", pipeline_response)
             list_of_elem = deserialized.value
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, iter(list_of_elem)
 
         def get_next(next_link=None):
-            request = prepare_request(next_link)
+            _request = prepare_request(next_link)
 
             _stream = False
             pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=_stream, **kwargs
+                _request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
             return pipeline_response
 
         return ItemPaged(get_next, extract_data)
 
-    list_by_cluster_pool_name.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HDInsight/clusterpools/{clusterPoolName}/clusters"
-    }
+    def _upgrade_initial(
+        self,
+        resource_group_name: str,
+        cluster_pool_name: str,
+        cluster_name: str,
+        cluster_upgrade_request: Union[_models.ClusterUpgrade, IO[bytes]],
+        **kwargs: Any
+    ) -> Optional[_models.Cluster]:
+        error_map = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[Optional[_models.Cluster]] = kwargs.pop("cls", None)
+
+        content_type = content_type or "application/json"
+        _json = None
+        _content = None
+        if isinstance(cluster_upgrade_request, (IOBase, bytes)):
+            _content = cluster_upgrade_request
+        else:
+            _json = self._serialize.body(cluster_upgrade_request, "ClusterUpgrade")
+
+        _request = build_upgrade_request(
+            resource_group_name=resource_group_name,
+            cluster_pool_name=cluster_pool_name,
+            cluster_name=cluster_name,
+            subscription_id=self._config.subscription_id,
+            api_version=api_version,
+            content_type=content_type,
+            json=_json,
+            content=_content,
+            headers=_headers,
+            params=_params,
+        )
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+            _request, stream=_stream, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200, 202]:
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
+            raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
+
+        deserialized = None
+        response_headers = {}
+        if response.status_code == 200:
+            deserialized = self._deserialize("Cluster", pipeline_response)
+
+        if response.status_code == 202:
+            response_headers["location"] = self._deserialize("str", response.headers.get("location"))
+
+        if cls:
+            return cls(pipeline_response, deserialized, response_headers)  # type: ignore
+
+        return deserialized  # type: ignore
+
+    @overload
+    def begin_upgrade(
+        self,
+        resource_group_name: str,
+        cluster_pool_name: str,
+        cluster_name: str,
+        cluster_upgrade_request: _models.ClusterUpgrade,
+        *,
+        content_type: str = "application/json",
+        **kwargs: Any
+    ) -> LROPoller[_models.Cluster]:
+        """Upgrade a cluster.
+
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
+        :type resource_group_name: str
+        :param cluster_pool_name: The name of the cluster pool. Required.
+        :type cluster_pool_name: str
+        :param cluster_name: The name of the HDInsight cluster. Required.
+        :type cluster_name: str
+        :param cluster_upgrade_request: Upgrade a cluster. Required.
+        :type cluster_upgrade_request: ~azure.mgmt.hdinsightcontainers.models.ClusterUpgrade
+        :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: An instance of LROPoller that returns either Cluster or the result of cls(response)
+        :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.hdinsightcontainers.models.Cluster]
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @overload
+    def begin_upgrade(
+        self,
+        resource_group_name: str,
+        cluster_pool_name: str,
+        cluster_name: str,
+        cluster_upgrade_request: IO[bytes],
+        *,
+        content_type: str = "application/json",
+        **kwargs: Any
+    ) -> LROPoller[_models.Cluster]:
+        """Upgrade a cluster.
+
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
+        :type resource_group_name: str
+        :param cluster_pool_name: The name of the cluster pool. Required.
+        :type cluster_pool_name: str
+        :param cluster_name: The name of the HDInsight cluster. Required.
+        :type cluster_name: str
+        :param cluster_upgrade_request: Upgrade a cluster. Required.
+        :type cluster_upgrade_request: IO[bytes]
+        :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: An instance of LROPoller that returns either Cluster or the result of cls(response)
+        :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.hdinsightcontainers.models.Cluster]
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @distributed_trace
+    def begin_upgrade(
+        self,
+        resource_group_name: str,
+        cluster_pool_name: str,
+        cluster_name: str,
+        cluster_upgrade_request: Union[_models.ClusterUpgrade, IO[bytes]],
+        **kwargs: Any
+    ) -> LROPoller[_models.Cluster]:
+        """Upgrade a cluster.
+
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
+        :type resource_group_name: str
+        :param cluster_pool_name: The name of the cluster pool. Required.
+        :type cluster_pool_name: str
+        :param cluster_name: The name of the HDInsight cluster. Required.
+        :type cluster_name: str
+        :param cluster_upgrade_request: Upgrade a cluster. Is either a ClusterUpgrade type or a
+         IO[bytes] type. Required.
+        :type cluster_upgrade_request: ~azure.mgmt.hdinsightcontainers.models.ClusterUpgrade or
+         IO[bytes]
+        :return: An instance of LROPoller that returns either Cluster or the result of cls(response)
+        :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.hdinsightcontainers.models.Cluster]
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[_models.Cluster] = kwargs.pop("cls", None)
+        polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
+        lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
+        cont_token: Optional[str] = kwargs.pop("continuation_token", None)
+        if cont_token is None:
+            raw_result = self._upgrade_initial(
+                resource_group_name=resource_group_name,
+                cluster_pool_name=cluster_pool_name,
+                cluster_name=cluster_name,
+                cluster_upgrade_request=cluster_upgrade_request,
+                api_version=api_version,
+                content_type=content_type,
+                cls=lambda x, y, z: x,
+                headers=_headers,
+                params=_params,
+                **kwargs
+            )
+        kwargs.pop("error_map", None)
+
+        def get_long_running_output(pipeline_response):
+            deserialized = self._deserialize("Cluster", pipeline_response)
+            if cls:
+                return cls(pipeline_response, deserialized, {})  # type: ignore
+            return deserialized
+
+        if polling is True:
+            polling_method: PollingMethod = cast(
+                PollingMethod, ARMPolling(lro_delay, lro_options={"final-state-via": "location"}, **kwargs)
+            )
+        elif polling is False:
+            polling_method = cast(PollingMethod, NoPolling())
+        else:
+            polling_method = polling
+        if cont_token:
+            return LROPoller[_models.Cluster].from_continuation_token(
+                polling_method=polling_method,
+                continuation_token=cont_token,
+                client=self._client,
+                deserialization_callback=get_long_running_output,
+            )
+        return LROPoller[_models.Cluster](
+            self._client, raw_result, get_long_running_output, polling_method  # type: ignore
+        )
 
     def _resize_initial(
         self,
         resource_group_name: str,
         cluster_pool_name: str,
         cluster_name: str,
-        cluster_resize_request: Union[_models.ClusterResizeData, IO],
+        cluster_resize_request: Union[_models.ClusterResizeData, IO[bytes]],
         **kwargs: Any
     ) -> Optional[_models.Cluster]:
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -491,33 +728,32 @@
         _json = None
         _content = None
         if isinstance(cluster_resize_request, (IOBase, bytes)):
             _content = cluster_resize_request
         else:
             _json = self._serialize.body(cluster_resize_request, "ClusterResizeData")
 
-        request = build_resize_request(
+        _request = build_resize_request(
             resource_group_name=resource_group_name,
             cluster_pool_name=cluster_pool_name,
             cluster_name=cluster_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             content_type=content_type,
             json=_json,
             content=_content,
-            template_url=self._resize_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -528,21 +764,17 @@
         if response.status_code == 200:
             deserialized = self._deserialize("Cluster", pipeline_response)
 
         if response.status_code == 202:
             response_headers["location"] = self._deserialize("str", response.headers.get("location"))
 
         if cls:
-            return cls(pipeline_response, deserialized, response_headers)
-
-        return deserialized
+            return cls(pipeline_response, deserialized, response_headers)  # type: ignore
 
-    _resize_initial.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HDInsight/clusterpools/{clusterPoolName}/clusters/{clusterName}/resize"
-    }
+        return deserialized  # type: ignore
 
     @overload
     def begin_resize(
         self,
         resource_group_name: str,
         cluster_pool_name: str,
         cluster_name: str,
@@ -561,97 +793,71 @@
         :param cluster_name: The name of the HDInsight cluster. Required.
         :type cluster_name: str
         :param cluster_resize_request: Resize a cluster. Required.
         :type cluster_resize_request: ~azure.mgmt.hdinsightcontainers.models.ClusterResizeData
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
-         operation to not poll, or pass in your own initialized polling object for a personal polling
-         strategy.
-        :paramtype polling: bool or ~azure.core.polling.PollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
         :return: An instance of LROPoller that returns either Cluster or the result of cls(response)
         :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.hdinsightcontainers.models.Cluster]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
     def begin_resize(
         self,
         resource_group_name: str,
         cluster_pool_name: str,
         cluster_name: str,
-        cluster_resize_request: IO,
+        cluster_resize_request: IO[bytes],
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> LROPoller[_models.Cluster]:
         """Resize an existing Cluster.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param cluster_pool_name: The name of the cluster pool. Required.
         :type cluster_pool_name: str
         :param cluster_name: The name of the HDInsight cluster. Required.
         :type cluster_name: str
         :param cluster_resize_request: Resize a cluster. Required.
-        :type cluster_resize_request: IO
+        :type cluster_resize_request: IO[bytes]
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
-         operation to not poll, or pass in your own initialized polling object for a personal polling
-         strategy.
-        :paramtype polling: bool or ~azure.core.polling.PollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
         :return: An instance of LROPoller that returns either Cluster or the result of cls(response)
         :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.hdinsightcontainers.models.Cluster]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace
     def begin_resize(
         self,
         resource_group_name: str,
         cluster_pool_name: str,
         cluster_name: str,
-        cluster_resize_request: Union[_models.ClusterResizeData, IO],
+        cluster_resize_request: Union[_models.ClusterResizeData, IO[bytes]],
         **kwargs: Any
     ) -> LROPoller[_models.Cluster]:
         """Resize an existing Cluster.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param cluster_pool_name: The name of the cluster pool. Required.
         :type cluster_pool_name: str
         :param cluster_name: The name of the HDInsight cluster. Required.
         :type cluster_name: str
-        :param cluster_resize_request: Resize a cluster. Is either a ClusterResizeData type or a IO
-         type. Required.
-        :type cluster_resize_request: ~azure.mgmt.hdinsightcontainers.models.ClusterResizeData or IO
-        :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
-         Default value is None.
-        :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
-         operation to not poll, or pass in your own initialized polling object for a personal polling
-         strategy.
-        :paramtype polling: bool or ~azure.core.polling.PollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
+        :param cluster_resize_request: Resize a cluster. Is either a ClusterResizeData type or a
+         IO[bytes] type. Required.
+        :type cluster_resize_request: ~azure.mgmt.hdinsightcontainers.models.ClusterResizeData or
+         IO[bytes]
         :return: An instance of LROPoller that returns either Cluster or the result of cls(response)
         :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.hdinsightcontainers.models.Cluster]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
@@ -675,52 +881,49 @@
                 **kwargs
             )
         kwargs.pop("error_map", None)
 
         def get_long_running_output(pipeline_response):
             deserialized = self._deserialize("Cluster", pipeline_response)
             if cls:
-                return cls(pipeline_response, deserialized, {})
+                return cls(pipeline_response, deserialized, {})  # type: ignore
             return deserialized
 
         if polling is True:
             polling_method: PollingMethod = cast(
                 PollingMethod, ARMPolling(lro_delay, lro_options={"final-state-via": "location"}, **kwargs)
             )
         elif polling is False:
             polling_method = cast(PollingMethod, NoPolling())
         else:
             polling_method = polling
         if cont_token:
-            return LROPoller.from_continuation_token(
+            return LROPoller[_models.Cluster].from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
                 deserialization_callback=get_long_running_output,
             )
-        return LROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
-
-    begin_resize.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HDInsight/clusterpools/{clusterPoolName}/clusters/{clusterName}/resize"
-    }
+        return LROPoller[_models.Cluster](
+            self._client, raw_result, get_long_running_output, polling_method  # type: ignore
+        )
 
     @distributed_trace
     def get(
         self, resource_group_name: str, cluster_pool_name: str, cluster_name: str, **kwargs: Any
     ) -> _models.Cluster:
         """Gets a HDInsight cluster.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param cluster_pool_name: The name of the cluster pool. Required.
         :type cluster_pool_name: str
         :param cluster_name: The name of the HDInsight cluster. Required.
         :type cluster_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: Cluster or the result of cls(response)
         :rtype: ~azure.mgmt.hdinsightcontainers.models.Cluster
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -731,56 +934,51 @@
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.Cluster] = kwargs.pop("cls", None)
 
-        request = build_get_request(
+        _request = build_get_request(
             resource_group_name=resource_group_name,
             cluster_pool_name=cluster_pool_name,
             cluster_name=cluster_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
-            template_url=self.get.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         deserialized = self._deserialize("Cluster", pipeline_response)
 
         if cls:
-            return cls(pipeline_response, deserialized, {})
-
-        return deserialized
+            return cls(pipeline_response, deserialized, {})  # type: ignore
 
-    get.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HDInsight/clusterpools/{clusterPoolName}/clusters/{clusterName}"
-    }
+        return deserialized  # type: ignore
 
     def _create_initial(
         self,
         resource_group_name: str,
         cluster_pool_name: str,
         cluster_name: str,
-        hd_insight_cluster: Union[_models.Cluster, IO],
+        hd_insight_cluster: Union[_models.Cluster, IO[bytes]],
         **kwargs: Any
     ) -> _models.Cluster:
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -798,33 +996,32 @@
         _json = None
         _content = None
         if isinstance(hd_insight_cluster, (IOBase, bytes)):
             _content = hd_insight_cluster
         else:
             _json = self._serialize.body(hd_insight_cluster, "Cluster")
 
-        request = build_create_request(
+        _request = build_create_request(
             resource_group_name=resource_group_name,
             cluster_pool_name=cluster_pool_name,
             cluster_name=cluster_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             content_type=content_type,
             json=_json,
             content=_content,
-            template_url=self._create_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 201]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -837,18 +1034,14 @@
             deserialized = self._deserialize("Cluster", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})  # type: ignore
 
         return deserialized  # type: ignore
 
-    _create_initial.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HDInsight/clusterpools/{clusterPoolName}/clusters/{clusterName}"
-    }
-
     @overload
     def begin_create(
         self,
         resource_group_name: str,
         cluster_pool_name: str,
         cluster_name: str,
         hd_insight_cluster: _models.Cluster,
@@ -866,97 +1059,70 @@
         :param cluster_name: The name of the HDInsight cluster. Required.
         :type cluster_name: str
         :param hd_insight_cluster: The cluster to create. Required.
         :type hd_insight_cluster: ~azure.mgmt.hdinsightcontainers.models.Cluster
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
-         operation to not poll, or pass in your own initialized polling object for a personal polling
-         strategy.
-        :paramtype polling: bool or ~azure.core.polling.PollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
         :return: An instance of LROPoller that returns either Cluster or the result of cls(response)
         :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.hdinsightcontainers.models.Cluster]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
     def begin_create(
         self,
         resource_group_name: str,
         cluster_pool_name: str,
         cluster_name: str,
-        hd_insight_cluster: IO,
+        hd_insight_cluster: IO[bytes],
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> LROPoller[_models.Cluster]:
         """Creates a cluster.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param cluster_pool_name: The name of the cluster pool. Required.
         :type cluster_pool_name: str
         :param cluster_name: The name of the HDInsight cluster. Required.
         :type cluster_name: str
         :param hd_insight_cluster: The cluster to create. Required.
-        :type hd_insight_cluster: IO
+        :type hd_insight_cluster: IO[bytes]
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
-         operation to not poll, or pass in your own initialized polling object for a personal polling
-         strategy.
-        :paramtype polling: bool or ~azure.core.polling.PollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
         :return: An instance of LROPoller that returns either Cluster or the result of cls(response)
         :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.hdinsightcontainers.models.Cluster]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace
     def begin_create(
         self,
         resource_group_name: str,
         cluster_pool_name: str,
         cluster_name: str,
-        hd_insight_cluster: Union[_models.Cluster, IO],
+        hd_insight_cluster: Union[_models.Cluster, IO[bytes]],
         **kwargs: Any
     ) -> LROPoller[_models.Cluster]:
         """Creates a cluster.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param cluster_pool_name: The name of the cluster pool. Required.
         :type cluster_pool_name: str
         :param cluster_name: The name of the HDInsight cluster. Required.
         :type cluster_name: str
-        :param hd_insight_cluster: The cluster to create. Is either a Cluster type or a IO type.
+        :param hd_insight_cluster: The cluster to create. Is either a Cluster type or a IO[bytes] type.
          Required.
-        :type hd_insight_cluster: ~azure.mgmt.hdinsightcontainers.models.Cluster or IO
-        :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
-         Default value is None.
-        :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
-         operation to not poll, or pass in your own initialized polling object for a personal polling
-         strategy.
-        :paramtype polling: bool or ~azure.core.polling.PollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
+        :type hd_insight_cluster: ~azure.mgmt.hdinsightcontainers.models.Cluster or IO[bytes]
         :return: An instance of LROPoller that returns either Cluster or the result of cls(response)
         :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.hdinsightcontainers.models.Cluster]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
@@ -980,44 +1146,42 @@
                 **kwargs
             )
         kwargs.pop("error_map", None)
 
         def get_long_running_output(pipeline_response):
             deserialized = self._deserialize("Cluster", pipeline_response)
             if cls:
-                return cls(pipeline_response, deserialized, {})
+                return cls(pipeline_response, deserialized, {})  # type: ignore
             return deserialized
 
         if polling is True:
             polling_method: PollingMethod = cast(
                 PollingMethod, ARMPolling(lro_delay, lro_options={"final-state-via": "azure-async-operation"}, **kwargs)
             )
         elif polling is False:
             polling_method = cast(PollingMethod, NoPolling())
         else:
             polling_method = polling
         if cont_token:
-            return LROPoller.from_continuation_token(
+            return LROPoller[_models.Cluster].from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
                 deserialization_callback=get_long_running_output,
             )
-        return LROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
-
-    begin_create.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HDInsight/clusterpools/{clusterPoolName}/clusters/{clusterName}"
-    }
+        return LROPoller[_models.Cluster](
+            self._client, raw_result, get_long_running_output, polling_method  # type: ignore
+        )
 
     def _update_initial(
         self,
         resource_group_name: str,
         cluster_pool_name: str,
         cluster_name: str,
-        cluster_patch_request: Union[_models.ClusterPatch, IO],
+        cluster_patch_request: Union[_models.ClusterPatch, IO[bytes]],
         **kwargs: Any
     ) -> _models.Cluster:
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -1035,33 +1199,32 @@
         _json = None
         _content = None
         if isinstance(cluster_patch_request, (IOBase, bytes)):
             _content = cluster_patch_request
         else:
             _json = self._serialize.body(cluster_patch_request, "ClusterPatch")
 
-        request = build_update_request(
+        _request = build_update_request(
             resource_group_name=resource_group_name,
             cluster_pool_name=cluster_pool_name,
             cluster_name=cluster_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             content_type=content_type,
             json=_json,
             content=_content,
-            template_url=self._update_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -1077,18 +1240,14 @@
             deserialized = self._deserialize("Cluster", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, response_headers)  # type: ignore
 
         return deserialized  # type: ignore
 
-    _update_initial.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HDInsight/clusterpools/{clusterPoolName}/clusters/{clusterName}"
-    }
-
     @overload
     def begin_update(
         self,
         resource_group_name: str,
         cluster_pool_name: str,
         cluster_name: str,
         cluster_patch_request: _models.ClusterPatch,
@@ -1106,97 +1265,70 @@
         :param cluster_name: The name of the HDInsight cluster. Required.
         :type cluster_name: str
         :param cluster_patch_request: Patch a cluster. Required.
         :type cluster_patch_request: ~azure.mgmt.hdinsightcontainers.models.ClusterPatch
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
-         operation to not poll, or pass in your own initialized polling object for a personal polling
-         strategy.
-        :paramtype polling: bool or ~azure.core.polling.PollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
         :return: An instance of LROPoller that returns either Cluster or the result of cls(response)
         :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.hdinsightcontainers.models.Cluster]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
     def begin_update(
         self,
         resource_group_name: str,
         cluster_pool_name: str,
         cluster_name: str,
-        cluster_patch_request: IO,
+        cluster_patch_request: IO[bytes],
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> LROPoller[_models.Cluster]:
         """Updates an existing Cluster.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param cluster_pool_name: The name of the cluster pool. Required.
         :type cluster_pool_name: str
         :param cluster_name: The name of the HDInsight cluster. Required.
         :type cluster_name: str
         :param cluster_patch_request: Patch a cluster. Required.
-        :type cluster_patch_request: IO
+        :type cluster_patch_request: IO[bytes]
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
-         operation to not poll, or pass in your own initialized polling object for a personal polling
-         strategy.
-        :paramtype polling: bool or ~azure.core.polling.PollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
         :return: An instance of LROPoller that returns either Cluster or the result of cls(response)
         :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.hdinsightcontainers.models.Cluster]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace
     def begin_update(
         self,
         resource_group_name: str,
         cluster_pool_name: str,
         cluster_name: str,
-        cluster_patch_request: Union[_models.ClusterPatch, IO],
+        cluster_patch_request: Union[_models.ClusterPatch, IO[bytes]],
         **kwargs: Any
     ) -> LROPoller[_models.Cluster]:
         """Updates an existing Cluster.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param cluster_pool_name: The name of the cluster pool. Required.
         :type cluster_pool_name: str
         :param cluster_name: The name of the HDInsight cluster. Required.
         :type cluster_name: str
-        :param cluster_patch_request: Patch a cluster. Is either a ClusterPatch type or a IO type.
-         Required.
-        :type cluster_patch_request: ~azure.mgmt.hdinsightcontainers.models.ClusterPatch or IO
-        :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
-         Default value is None.
-        :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
-         operation to not poll, or pass in your own initialized polling object for a personal polling
-         strategy.
-        :paramtype polling: bool or ~azure.core.polling.PollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
+        :param cluster_patch_request: Patch a cluster. Is either a ClusterPatch type or a IO[bytes]
+         type. Required.
+        :type cluster_patch_request: ~azure.mgmt.hdinsightcontainers.models.ClusterPatch or IO[bytes]
         :return: An instance of LROPoller that returns either Cluster or the result of cls(response)
         :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.hdinsightcontainers.models.Cluster]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
@@ -1220,37 +1352,35 @@
                 **kwargs
             )
         kwargs.pop("error_map", None)
 
         def get_long_running_output(pipeline_response):
             deserialized = self._deserialize("Cluster", pipeline_response)
             if cls:
-                return cls(pipeline_response, deserialized, {})
+                return cls(pipeline_response, deserialized, {})  # type: ignore
             return deserialized
 
         if polling is True:
             polling_method: PollingMethod = cast(
                 PollingMethod, ARMPolling(lro_delay, lro_options={"final-state-via": "azure-async-operation"}, **kwargs)
             )
         elif polling is False:
             polling_method = cast(PollingMethod, NoPolling())
         else:
             polling_method = polling
         if cont_token:
-            return LROPoller.from_continuation_token(
+            return LROPoller[_models.Cluster].from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
                 deserialization_callback=get_long_running_output,
             )
-        return LROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
-
-    begin_update.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HDInsight/clusterpools/{clusterPoolName}/clusters/{clusterName}"
-    }
+        return LROPoller[_models.Cluster](
+            self._client, raw_result, get_long_running_output, polling_method  # type: ignore
+        )
 
     def _delete_initial(  # pylint: disable=inconsistent-return-statements
         self, resource_group_name: str, cluster_pool_name: str, cluster_name: str, **kwargs: Any
     ) -> None:
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -1261,71 +1391,58 @@
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
-        request = build_delete_request(
+        _request = build_delete_request(
             resource_group_name=resource_group_name,
             cluster_pool_name=cluster_pool_name,
             cluster_name=cluster_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
-            template_url=self._delete_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         response_headers = {}
         if response.status_code == 202:
             response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
 
         if cls:
-            return cls(pipeline_response, None, response_headers)
-
-    _delete_initial.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HDInsight/clusterpools/{clusterPoolName}/clusters/{clusterName}"
-    }
+            return cls(pipeline_response, None, response_headers)  # type: ignore
 
     @distributed_trace
     def begin_delete(
         self, resource_group_name: str, cluster_pool_name: str, cluster_name: str, **kwargs: Any
     ) -> LROPoller[None]:
         """Deletes a cluster.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param cluster_pool_name: The name of the cluster pool. Required.
         :type cluster_pool_name: str
         :param cluster_name: The name of the HDInsight cluster. Required.
         :type cluster_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
-         operation to not poll, or pass in your own initialized polling object for a personal polling
-         strategy.
-        :paramtype polling: bool or ~azure.core.polling.PollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
         :return: An instance of LROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.LROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
@@ -1345,51 +1462,46 @@
                 params=_params,
                 **kwargs
             )
         kwargs.pop("error_map", None)
 
         def get_long_running_output(pipeline_response):  # pylint: disable=inconsistent-return-statements
             if cls:
-                return cls(pipeline_response, None, {})
+                return cls(pipeline_response, None, {})  # type: ignore
 
         if polling is True:
             polling_method: PollingMethod = cast(
                 PollingMethod, ARMPolling(lro_delay, lro_options={"final-state-via": "azure-async-operation"}, **kwargs)
             )
         elif polling is False:
             polling_method = cast(PollingMethod, NoPolling())
         else:
             polling_method = polling
         if cont_token:
-            return LROPoller.from_continuation_token(
+            return LROPoller[None].from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
                 deserialization_callback=get_long_running_output,
             )
-        return LROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
-
-    begin_delete.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HDInsight/clusterpools/{clusterPoolName}/clusters/{clusterName}"
-    }
+        return LROPoller[None](self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
 
     @distributed_trace
     def list_service_configs(
         self, resource_group_name: str, cluster_pool_name: str, cluster_name: str, **kwargs: Any
     ) -> Iterable["_models.ServiceConfigResult"]:
         """Lists the config dump of all services running in cluster.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param cluster_pool_name: The name of the cluster pool. Required.
         :type cluster_pool_name: str
         :param cluster_name: The name of the HDInsight cluster. Required.
         :type cluster_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either ServiceConfigResult or the result of cls(response)
         :rtype:
          ~azure.core.paging.ItemPaged[~azure.mgmt.hdinsightcontainers.models.ServiceConfigResult]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
@@ -1404,88 +1516,82 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         def prepare_request(next_link=None):
             if not next_link:
 
-                request = build_list_service_configs_request(
+                _request = build_list_service_configs_request(
                     resource_group_name=resource_group_name,
                     cluster_pool_name=cluster_pool_name,
                     cluster_name=cluster_name,
                     subscription_id=self._config.subscription_id,
                     api_version=api_version,
-                    template_url=self.list_service_configs.metadata["url"],
                     headers=_headers,
                     params=_params,
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
 
             else:
                 # make call to next link with the client's api-version
                 _parsed_next_link = urllib.parse.urlparse(next_link)
                 _next_request_params = case_insensitive_dict(
                     {
                         key: [urllib.parse.quote(v) for v in value]
                         for key, value in urllib.parse.parse_qs(_parsed_next_link.query).items()
                     }
                 )
                 _next_request_params["api-version"] = self._config.api_version
-                request = HttpRequest(
+                _request = HttpRequest(
                     "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
-                request.method = "GET"
-            return request
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
+                _request.method = "GET"
+            return _request
 
         def extract_data(pipeline_response):
             deserialized = self._deserialize("ServiceConfigListResult", pipeline_response)
             list_of_elem = deserialized.value
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, iter(list_of_elem)
 
         def get_next(next_link=None):
-            request = prepare_request(next_link)
+            _request = prepare_request(next_link)
 
             _stream = False
             pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=_stream, **kwargs
+                _request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
             return pipeline_response
 
         return ItemPaged(get_next, extract_data)
 
-    list_service_configs.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HDInsight/clusterpools/{clusterPoolName}/clusters/{clusterName}/serviceConfigs"
-    }
-
     @distributed_trace
     def list_instance_views(
         self, resource_group_name: str, cluster_pool_name: str, cluster_name: str, **kwargs: Any
     ) -> Iterable["_models.ClusterInstanceViewResult"]:
         """Lists the lists of instance views.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param cluster_pool_name: The name of the cluster pool. Required.
         :type cluster_pool_name: str
         :param cluster_name: The name of the HDInsight cluster. Required.
         :type cluster_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either ClusterInstanceViewResult or the result of
          cls(response)
         :rtype:
          ~azure.core.paging.ItemPaged[~azure.mgmt.hdinsightcontainers.models.ClusterInstanceViewResult]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
@@ -1501,88 +1607,82 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         def prepare_request(next_link=None):
             if not next_link:
 
-                request = build_list_instance_views_request(
+                _request = build_list_instance_views_request(
                     resource_group_name=resource_group_name,
                     cluster_pool_name=cluster_pool_name,
                     cluster_name=cluster_name,
                     subscription_id=self._config.subscription_id,
                     api_version=api_version,
-                    template_url=self.list_instance_views.metadata["url"],
                     headers=_headers,
                     params=_params,
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
 
             else:
                 # make call to next link with the client's api-version
                 _parsed_next_link = urllib.parse.urlparse(next_link)
                 _next_request_params = case_insensitive_dict(
                     {
                         key: [urllib.parse.quote(v) for v in value]
                         for key, value in urllib.parse.parse_qs(_parsed_next_link.query).items()
                     }
                 )
                 _next_request_params["api-version"] = self._config.api_version
-                request = HttpRequest(
+                _request = HttpRequest(
                     "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
-                request.method = "GET"
-            return request
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
+                _request.method = "GET"
+            return _request
 
         def extract_data(pipeline_response):
             deserialized = self._deserialize("ClusterInstanceViewsResult", pipeline_response)
             list_of_elem = deserialized.value
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, iter(list_of_elem)
 
         def get_next(next_link=None):
-            request = prepare_request(next_link)
+            _request = prepare_request(next_link)
 
             _stream = False
             pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=_stream, **kwargs
+                _request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
             return pipeline_response
 
         return ItemPaged(get_next, extract_data)
 
-    list_instance_views.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HDInsight/clusterpools/{clusterPoolName}/clusters/{clusterName}/instanceViews"
-    }
-
     @distributed_trace
     def get_instance_view(
         self, resource_group_name: str, cluster_pool_name: str, cluster_name: str, **kwargs: Any
     ) -> _models.ClusterInstanceViewResult:
         """Gets the status of a cluster instance.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param cluster_pool_name: The name of the cluster pool. Required.
         :type cluster_pool_name: str
         :param cluster_name: The name of the HDInsight cluster. Required.
         :type cluster_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: ClusterInstanceViewResult or the result of cls(response)
         :rtype: ~azure.mgmt.hdinsightcontainers.models.ClusterInstanceViewResult
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -1593,42 +1693,37 @@
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.ClusterInstanceViewResult] = kwargs.pop("cls", None)
 
-        request = build_get_instance_view_request(
+        _request = build_get_instance_view_request(
             resource_group_name=resource_group_name,
             cluster_pool_name=cluster_pool_name,
             cluster_name=cluster_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
-            template_url=self.get_instance_view.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         deserialized = self._deserialize("ClusterInstanceViewResult", pipeline_response)
 
         if cls:
-            return cls(pipeline_response, deserialized, {})
-
-        return deserialized
+            return cls(pipeline_response, deserialized, {})  # type: ignore
 
-    get_instance_view.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HDInsight/clusterpools/{clusterPoolName}/clusters/{clusterName}/instanceViews/default"
-    }
+        return deserialized  # type: ignore
```

### Comparing `azure-mgmt-hdinsightcontainers-1.0.0b1/azure/mgmt/hdinsightcontainers/operations/_locations_operations.py` & `azure-mgmt-hdinsightcontainers-1.0.0b2/azure/mgmt/hdinsightcontainers/operations/_locations_operations.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=too-many-lines
+# pylint: disable=too-many-lines,too-many-statements
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
@@ -35,15 +35,15 @@
 _SERIALIZER.client_side_validation = False
 
 
 def build_check_name_availability_request(location: str, subscription_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-01-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-11-01-preview"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/providers/Microsoft.HDInsight/locations/{location}/checkNameAvailability",
@@ -100,55 +100,57 @@
         :type location: str
         :param name_availability_parameters: The name and type of the resource. Required.
         :type name_availability_parameters:
          ~azure.mgmt.hdinsightcontainers.models.NameAvailabilityParameters
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: NameAvailabilityResult or the result of cls(response)
         :rtype: ~azure.mgmt.hdinsightcontainers.models.NameAvailabilityResult
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
     def check_name_availability(
-        self, location: str, name_availability_parameters: IO, *, content_type: str = "application/json", **kwargs: Any
+        self,
+        location: str,
+        name_availability_parameters: IO[bytes],
+        *,
+        content_type: str = "application/json",
+        **kwargs: Any
     ) -> _models.NameAvailabilityResult:
         """Check the availability of the resource name.
 
         :param location: The name of the Azure region. Required.
         :type location: str
         :param name_availability_parameters: The name and type of the resource. Required.
-        :type name_availability_parameters: IO
+        :type name_availability_parameters: IO[bytes]
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: NameAvailabilityResult or the result of cls(response)
         :rtype: ~azure.mgmt.hdinsightcontainers.models.NameAvailabilityResult
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace
     def check_name_availability(
-        self, location: str, name_availability_parameters: Union[_models.NameAvailabilityParameters, IO], **kwargs: Any
+        self,
+        location: str,
+        name_availability_parameters: Union[_models.NameAvailabilityParameters, IO[bytes]],
+        **kwargs: Any
     ) -> _models.NameAvailabilityResult:
         """Check the availability of the resource name.
 
         :param location: The name of the Azure region. Required.
         :type location: str
         :param name_availability_parameters: The name and type of the resource. Is either a
-         NameAvailabilityParameters type or a IO type. Required.
+         NameAvailabilityParameters type or a IO[bytes] type. Required.
         :type name_availability_parameters:
-         ~azure.mgmt.hdinsightcontainers.models.NameAvailabilityParameters or IO
-        :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
-         Default value is None.
-        :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
+         ~azure.mgmt.hdinsightcontainers.models.NameAvailabilityParameters or IO[bytes]
         :return: NameAvailabilityResult or the result of cls(response)
         :rtype: ~azure.mgmt.hdinsightcontainers.models.NameAvailabilityResult
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -168,43 +170,38 @@
         _json = None
         _content = None
         if isinstance(name_availability_parameters, (IOBase, bytes)):
             _content = name_availability_parameters
         else:
             _json = self._serialize.body(name_availability_parameters, "NameAvailabilityParameters")
 
-        request = build_check_name_availability_request(
+        _request = build_check_name_availability_request(
             location=location,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             content_type=content_type,
             json=_json,
             content=_content,
-            template_url=self.check_name_availability.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         deserialized = self._deserialize("NameAvailabilityResult", pipeline_response)
 
         if cls:
-            return cls(pipeline_response, deserialized, {})
+            return cls(pipeline_response, deserialized, {})  # type: ignore
 
-        return deserialized
-
-    check_name_availability.metadata = {
-        "url": "/subscriptions/{subscriptionId}/providers/Microsoft.HDInsight/locations/{location}/checkNameAvailability"
-    }
+        return deserialized  # type: ignore
```

### Comparing `azure-mgmt-hdinsightcontainers-1.0.0b1/azure/mgmt/hdinsightcontainers/operations/_operations.py` & `azure-mgmt-hdinsightcontainers-1.0.0b2/azure/mgmt/hdinsightcontainers/operations/_operations.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=too-many-lines
+# pylint: disable=too-many-lines,too-many-statements
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
@@ -36,15 +36,15 @@
 _SERIALIZER.client_side_validation = False
 
 
 def build_list_request(**kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-01-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-11-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop("template_url", "/providers/Microsoft.HDInsight/operations")
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
@@ -74,15 +74,14 @@
         self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
         self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
 
     @distributed_trace
     def list(self, **kwargs: Any) -> Iterable["_models.Operation"]:
         """Returns list of operations.
 
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either Operation or the result of cls(response)
         :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.hdinsightcontainers.models.Operation]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
@@ -96,60 +95,57 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         def prepare_request(next_link=None):
             if not next_link:
 
-                request = build_list_request(
+                _request = build_list_request(
                     api_version=api_version,
-                    template_url=self.list.metadata["url"],
                     headers=_headers,
                     params=_params,
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
 
             else:
                 # make call to next link with the client's api-version
                 _parsed_next_link = urllib.parse.urlparse(next_link)
                 _next_request_params = case_insensitive_dict(
                     {
                         key: [urllib.parse.quote(v) for v in value]
                         for key, value in urllib.parse.parse_qs(_parsed_next_link.query).items()
                     }
                 )
                 _next_request_params["api-version"] = self._config.api_version
-                request = HttpRequest(
+                _request = HttpRequest(
                     "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
-                request.method = "GET"
-            return request
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
+                _request.method = "GET"
+            return _request
 
         def extract_data(pipeline_response):
             deserialized = self._deserialize("OperationListResult", pipeline_response)
             list_of_elem = deserialized.value
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, iter(list_of_elem)
 
         def get_next(next_link=None):
-            request = prepare_request(next_link)
+            _request = prepare_request(next_link)
 
             _stream = False
             pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=_stream, **kwargs
+                _request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
             return pipeline_response
 
         return ItemPaged(get_next, extract_data)
-
-    list.metadata = {"url": "/providers/Microsoft.HDInsight/operations"}
```

### Comparing `azure-mgmt-hdinsightcontainers-1.0.0b1/azure/mgmt/hdinsightcontainers/operations/_patch.py` & `azure-mgmt-hdinsightcontainers-1.0.0b2/azure/mgmt/hdinsightcontainers/operations/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-hdinsightcontainers-1.0.0b1/azure_mgmt_hdinsightcontainers.egg-info/SOURCES.txt` & `azure-mgmt-hdinsightcontainers-1.0.0b2/azure_mgmt_hdinsightcontainers.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -17,28 +17,32 @@
 azure/mgmt/hdinsightcontainers/aio/__init__.py
 azure/mgmt/hdinsightcontainers/aio/_configuration.py
 azure/mgmt/hdinsightcontainers/aio/_hd_insight_containers_mgmt_client.py
 azure/mgmt/hdinsightcontainers/aio/_patch.py
 azure/mgmt/hdinsightcontainers/aio/operations/__init__.py
 azure/mgmt/hdinsightcontainers/aio/operations/_available_cluster_pool_versions_operations.py
 azure/mgmt/hdinsightcontainers/aio/operations/_available_cluster_versions_operations.py
+azure/mgmt/hdinsightcontainers/aio/operations/_cluster_available_upgrades_operations.py
 azure/mgmt/hdinsightcontainers/aio/operations/_cluster_jobs_operations.py
+azure/mgmt/hdinsightcontainers/aio/operations/_cluster_pool_available_upgrades_operations.py
 azure/mgmt/hdinsightcontainers/aio/operations/_cluster_pools_operations.py
 azure/mgmt/hdinsightcontainers/aio/operations/_clusters_operations.py
 azure/mgmt/hdinsightcontainers/aio/operations/_locations_operations.py
 azure/mgmt/hdinsightcontainers/aio/operations/_operations.py
 azure/mgmt/hdinsightcontainers/aio/operations/_patch.py
 azure/mgmt/hdinsightcontainers/models/__init__.py
 azure/mgmt/hdinsightcontainers/models/_hd_insight_containers_mgmt_client_enums.py
 azure/mgmt/hdinsightcontainers/models/_models_py3.py
 azure/mgmt/hdinsightcontainers/models/_patch.py
 azure/mgmt/hdinsightcontainers/operations/__init__.py
 azure/mgmt/hdinsightcontainers/operations/_available_cluster_pool_versions_operations.py
 azure/mgmt/hdinsightcontainers/operations/_available_cluster_versions_operations.py
+azure/mgmt/hdinsightcontainers/operations/_cluster_available_upgrades_operations.py
 azure/mgmt/hdinsightcontainers/operations/_cluster_jobs_operations.py
+azure/mgmt/hdinsightcontainers/operations/_cluster_pool_available_upgrades_operations.py
 azure/mgmt/hdinsightcontainers/operations/_cluster_pools_operations.py
 azure/mgmt/hdinsightcontainers/operations/_clusters_operations.py
 azure/mgmt/hdinsightcontainers/operations/_locations_operations.py
 azure/mgmt/hdinsightcontainers/operations/_operations.py
 azure/mgmt/hdinsightcontainers/operations/_patch.py
 azure_mgmt_hdinsightcontainers.egg-info/PKG-INFO
 azure_mgmt_hdinsightcontainers.egg-info/SOURCES.txt
```

### Comparing `azure-mgmt-hdinsightcontainers-1.0.0b1/setup.py` & `azure-mgmt-hdinsightcontainers-1.0.0b2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,19 +49,19 @@
     url="https://github.com/Azure/azure-sdk-for-python",
     keywords="azure, azure sdk",  # update with search keywords relevant to the azure service / product
     classifiers=[
         "Development Status :: 4 - Beta",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
         "License :: OSI Approved :: MIT License",
     ],
     zip_safe=False,
     packages=find_packages(
         exclude=[
             "tests",
             # Exclude packages that will be covered by PEP420 or nspkg
@@ -70,14 +70,13 @@
         ]
     ),
     include_package_data=True,
     package_data={
         "pytyped": ["py.typed"],
     },
     install_requires=[
-        "isodate<1.0.0,>=0.6.1",
-        "azure-common~=1.1",
-        "azure-mgmt-core>=1.3.2,<2.0.0",
-        "typing-extensions>=4.3.0; python_version<'3.8.0'",
+        "isodate>=0.6.1",
+        "azure-common>=1.1",
+        "azure-mgmt-core>=1.3.2",
     ],
-    python_requires=">=3.7",
+    python_requires=">=3.8",
 )
```

