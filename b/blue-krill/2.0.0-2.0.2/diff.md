# Comparing `tmp/blue_krill-2.0.0.tar.gz` & `tmp/blue_krill-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blue_krill-2.0.0.tar", max compression
+gzip compressed data, was "blue_krill-2.0.2.tar", max compression
```

## Comparing `blue_krill-2.0.0.tar` & `blue_krill-2.0.2.tar`

### file list

```diff
@@ -1,63 +1,63 @@
--rw-r--r--   0        0        0    23858 2023-08-03 07:52:58.364678 blue_krill-2.0.0/README.md
--rw-r--r--   0        0        0      782 2023-08-04 09:02:43.854603 blue_krill-2.0.0/blue_krill/__init__.py
--rw-r--r--   0        0        0      760 2023-08-03 07:45:22.724240 blue_krill-2.0.0/blue_krill/async_utils/__init__.py
--rw-r--r--   0        0        0     1755 2023-08-03 07:52:58.364848 blue_krill-2.0.0/blue_krill/async_utils/django_utils.py
--rw-r--r--   0        0        0    11538 2023-08-03 07:45:22.724307 blue_krill-2.0.0/blue_krill/async_utils/poll_task.py
--rw-r--r--   0        0        0      760 2023-08-03 07:45:22.724432 blue_krill-2.0.0/blue_krill/auth/__init__.py
--rw-r--r--   0        0        0     6068 2023-08-03 07:52:58.364926 blue_krill-2.0.0/blue_krill/auth/client.py
--rw-r--r--   0        0        0     2683 2023-08-03 07:52:58.365035 blue_krill-2.0.0/blue_krill/auth/jwt.py
--rw-r--r--   0        0        0     1629 2023-08-03 07:52:58.365093 blue_krill-2.0.0/blue_krill/auth/utils.py
--rw-r--r--   0        0        0      760 2023-08-03 07:45:22.724648 blue_krill-2.0.0/blue_krill/connections/__init__.py
--rw-r--r--   0        0        0      824 2023-08-03 07:45:22.724801 blue_krill-2.0.0/blue_krill/connections/exceptions.py
--rw-r--r--   0        0        0     1718 2023-08-03 07:52:58.365204 blue_krill-2.0.0/blue_krill/connections/ha_algorithm.py
--rw-r--r--   0        0        0     7147 2023-08-03 07:52:58.365348 blue_krill-2.0.0/blue_krill/connections/ha_endpoint_pool.py
--rw-r--r--   0        0        0     1457 2023-08-03 07:45:22.725046 blue_krill-2.0.0/blue_krill/contextlib.py
--rw-r--r--   0        0        0     6964 2023-08-03 07:45:22.725125 blue_krill-2.0.0/blue_krill/cubing_case.py
--rw-r--r--   0        0        0      760 2023-08-03 07:45:22.725231 blue_krill-2.0.0/blue_krill/data_types/__init__.py
--rw-r--r--   0        0        0     8652 2023-08-03 07:45:22.725343 blue_krill-2.0.0/blue_krill/data_types/enum.py
--rw-r--r--   0        0        0     3603 2023-08-03 07:52:58.365460 blue_krill-2.0.0/blue_krill/data_types/url.py
--rw-r--r--   0        0        0      760 2023-08-03 07:45:22.725461 blue_krill-2.0.0/blue_krill/editions/__init__.py
--rw-r--r--   0        0        0    21444 2023-08-04 09:02:43.855095 blue_krill-2.0.0/blue_krill/editions/editionctl.py
--rw-r--r--   0        0        0     2777 2023-08-03 07:45:22.725728 blue_krill-2.0.0/blue_krill/encoding.py
--rw-r--r--   0        0        0      760 2023-08-03 07:45:22.725821 blue_krill-2.0.0/blue_krill/encrypt/__init__.py
--rw-r--r--   0        0        0     4258 2023-08-03 07:52:58.365646 blue_krill-2.0.0/blue_krill/encrypt/handler.py
--rw-r--r--   0        0        0     2399 2023-08-03 07:45:22.725959 blue_krill-2.0.0/blue_krill/encrypt/legacy.py
--rw-r--r--   0        0        0     1980 2023-08-03 07:52:58.365786 blue_krill-2.0.0/blue_krill/encrypt/utils.py
--rw-r--r--   0        0        0      760 2023-08-03 07:45:22.726143 blue_krill-2.0.0/blue_krill/models/__init__.py
--rw-r--r--   0        0        0      867 2023-08-03 07:45:22.726293 blue_krill-2.0.0/blue_krill/models/better_loaddata/__init__.py
--rw-r--r--   0        0        0      882 2023-08-03 07:45:22.726367 blue_krill-2.0.0/blue_krill/models/better_loaddata/apps.py
--rw-r--r--   0        0        0      760 2023-08-03 07:45:22.726474 blue_krill-2.0.0/blue_krill/models/better_loaddata/management/__init__.py
--rw-r--r--   0        0        0      760 2023-08-03 07:45:22.726595 blue_krill-2.0.0/blue_krill/models/better_loaddata/management/commands/__init__.py
--rw-r--r--   0        0        0     4997 2023-08-04 09:02:43.855521 blue_krill-2.0.0/blue_krill/models/better_loaddata/management/commands/better_loaddata.py
--rw-r--r--   0        0        0     1727 2023-08-03 07:52:58.365924 blue_krill-2.0.0/blue_krill/models/fields.py
--rw-r--r--   0        0        0      760 2023-08-03 07:45:22.726881 blue_krill-2.0.0/blue_krill/monitoring/__init__.py
--rw-r--r--   0        0        0      760 2023-08-03 07:45:22.726999 blue_krill-2.0.0/blue_krill/monitoring/probe/__init__.py
--rw-r--r--   0        0        0     3827 2023-08-03 07:45:22.727086 blue_krill-2.0.0/blue_krill/monitoring/probe/base.py
--rw-r--r--   0        0        0      906 2023-08-03 07:45:22.727150 blue_krill-2.0.0/blue_krill/monitoring/probe/exceptions.py
--rw-r--r--   0        0        0     3723 2023-08-03 07:45:22.727225 blue_krill-2.0.0/blue_krill/monitoring/probe/http.py
--rw-r--r--   0        0        0     2689 2023-08-04 09:02:43.855873 blue_krill-2.0.0/blue_krill/monitoring/probe/mysql.py
--rw-r--r--   0        0        0     2906 2023-08-03 07:52:58.366060 blue_krill-2.0.0/blue_krill/monitoring/probe/redis.py
--rw-r--r--   0        0        0     1908 2023-08-03 07:45:22.727438 blue_krill-2.0.0/blue_krill/monitoring/probe/tcp.py
--rw-r--r--   0        0        0      760 2023-08-03 07:45:22.727558 blue_krill-2.0.0/blue_krill/monitoring/prometheus/__init__.py
--rw-r--r--   0        0        0     5004 2023-08-03 07:45:22.727652 blue_krill-2.0.0/blue_krill/monitoring/prometheus/django_utils.py
--rw-r--r--   0        0        0     1344 2023-08-03 07:45:22.727737 blue_krill-2.0.0/blue_krill/monitoring/prometheus/setups.py
--rw-r--r--   0        0        0        0 2023-08-03 07:45:22.727765 blue_krill-2.0.0/blue_krill/py.typed
--rw-r--r--   0        0        0      760 2023-08-03 07:45:22.727888 blue_krill-2.0.0/blue_krill/redis_tools/__init__.py
--rw-r--r--   0        0        0     6517 2023-08-03 07:45:22.727975 blue_krill-2.0.0/blue_krill/redis_tools/messaging.py
--rw-r--r--   0        0        0     3756 2023-08-04 07:08:34.176357 blue_krill-2.0.0/blue_krill/redis_tools/sentinel.py
--rw-r--r--   0        0        0      760 2023-08-03 07:45:22.728076 blue_krill-2.0.0/blue_krill/secure/__init__.py
--rw-r--r--   0        0        0     3886 2023-08-03 07:45:22.728154 blue_krill-2.0.0/blue_krill/secure/bk_secure.py
--rw-r--r--   0        0        0     2233 2023-08-03 07:45:22.728229 blue_krill-2.0.0/blue_krill/secure/dj_environ.py
--rw-r--r--   0        0        0      760 2023-08-03 07:45:22.728346 blue_krill-2.0.0/blue_krill/storages/__init__.py
--rw-r--r--   0        0        0      760 2023-08-03 07:45:22.728439 blue_krill-2.0.0/blue_krill/storages/blobstore/__init__.py
--rw-r--r--   0        0        0     4045 2023-08-03 07:45:22.728521 blue_krill-2.0.0/blue_krill/storages/blobstore/base.py
--rw-r--r--   0        0        0    13906 2023-08-03 07:52:58.366273 blue_krill-2.0.0/blue_krill/storages/blobstore/bkrepo.py
--rw-r--r--   0        0        0     1910 2023-08-03 07:52:58.366375 blue_krill-2.0.0/blue_krill/storages/blobstore/exceptions.py
--rw-r--r--   0        0        0     6262 2023-08-03 07:45:22.728776 blue_krill-2.0.0/blue_krill/storages/blobstore/s3.py
--rw-r--r--   0        0        0    10889 2023-08-03 07:45:22.728867 blue_krill-2.0.0/blue_krill/termcolors.py
--rw-r--r--   0        0        0     1666 2023-08-03 07:52:58.366457 blue_krill-2.0.0/blue_krill/text.py
--rw-r--r--   0        0        0      760 2023-08-03 07:45:22.728963 blue_krill-2.0.0/blue_krill/web/__init__.py
--rw-r--r--   0        0        0     9697 2023-08-03 07:45:22.729063 blue_krill-2.0.0/blue_krill/web/drf_utils.py
--rw-r--r--   0        0        0     5644 2023-08-03 07:52:58.366559 blue_krill-2.0.0/blue_krill/web/std_error.py
--rw-r--r--   0        0        0     1997 2023-08-04 09:02:43.857348 blue_krill-2.0.0/pyproject.toml
--rw-r--r--   0        0        0    24846 1970-01-01 00:00:00.000000 blue_krill-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0    23858 2023-08-17 02:08:16.437125 blue_krill-2.0.2/README.md
+-rw-r--r--   0        0        0      782 2023-08-17 02:08:16.437514 blue_krill-2.0.2/blue_krill/__init__.py
+-rw-r--r--   0        0        0      760 2023-08-17 02:08:16.437781 blue_krill-2.0.2/blue_krill/async_utils/__init__.py
+-rw-r--r--   0        0        0     1755 2023-08-17 02:08:16.437983 blue_krill-2.0.2/blue_krill/async_utils/django_utils.py
+-rw-r--r--   0        0        0    11538 2023-08-17 02:08:16.438186 blue_krill-2.0.2/blue_krill/async_utils/poll_task.py
+-rw-r--r--   0        0        0      760 2023-08-17 02:08:16.438428 blue_krill-2.0.2/blue_krill/auth/__init__.py
+-rw-r--r--   0        0        0     6068 2023-08-17 02:08:16.438696 blue_krill-2.0.2/blue_krill/auth/client.py
+-rw-r--r--   0        0        0     2683 2023-08-17 02:08:16.439000 blue_krill-2.0.2/blue_krill/auth/jwt.py
+-rw-r--r--   0        0        0     1629 2023-08-17 02:08:16.439275 blue_krill-2.0.2/blue_krill/auth/utils.py
+-rw-r--r--   0        0        0      760 2023-08-17 02:08:16.439698 blue_krill-2.0.2/blue_krill/connections/__init__.py
+-rw-r--r--   0        0        0      824 2023-08-17 02:08:16.440059 blue_krill-2.0.2/blue_krill/connections/exceptions.py
+-rw-r--r--   0        0        0     1718 2023-08-17 02:08:16.440309 blue_krill-2.0.2/blue_krill/connections/ha_algorithm.py
+-rw-r--r--   0        0        0     7147 2023-08-17 02:08:16.440544 blue_krill-2.0.2/blue_krill/connections/ha_endpoint_pool.py
+-rw-r--r--   0        0        0     1457 2023-08-17 02:08:16.440806 blue_krill-2.0.2/blue_krill/contextlib.py
+-rw-r--r--   0        0        0     6964 2023-08-17 02:08:16.441145 blue_krill-2.0.2/blue_krill/cubing_case.py
+-rw-r--r--   0        0        0      760 2023-08-17 02:08:16.441527 blue_krill-2.0.2/blue_krill/data_types/__init__.py
+-rw-r--r--   0        0        0     8652 2023-08-17 02:08:16.441841 blue_krill-2.0.2/blue_krill/data_types/enum.py
+-rw-r--r--   0        0        0     3603 2023-08-17 02:08:16.442068 blue_krill-2.0.2/blue_krill/data_types/url.py
+-rw-r--r--   0        0        0      760 2023-08-17 02:08:16.442366 blue_krill-2.0.2/blue_krill/editions/__init__.py
+-rw-r--r--   0        0        0    21444 2023-08-17 02:08:16.442761 blue_krill-2.0.2/blue_krill/editions/editionctl.py
+-rw-r--r--   0        0        0     2777 2023-08-17 02:08:16.443042 blue_krill-2.0.2/blue_krill/encoding.py
+-rw-r--r--   0        0        0      760 2023-08-17 02:08:16.443448 blue_krill-2.0.2/blue_krill/encrypt/__init__.py
+-rw-r--r--   0        0        0     4419 2023-08-17 02:08:16.443688 blue_krill-2.0.2/blue_krill/encrypt/handler.py
+-rw-r--r--   0        0        0     2399 2023-08-17 02:08:16.444410 blue_krill-2.0.2/blue_krill/encrypt/legacy.py
+-rw-r--r--   0        0        0     1980 2023-08-17 02:08:16.444609 blue_krill-2.0.2/blue_krill/encrypt/utils.py
+-rw-r--r--   0        0        0      760 2023-08-17 02:08:16.445696 blue_krill-2.0.2/blue_krill/models/__init__.py
+-rw-r--r--   0        0        0      867 2023-08-17 02:08:16.446064 blue_krill-2.0.2/blue_krill/models/better_loaddata/__init__.py
+-rw-r--r--   0        0        0      882 2023-08-17 02:08:16.446297 blue_krill-2.0.2/blue_krill/models/better_loaddata/apps.py
+-rw-r--r--   0        0        0      760 2023-08-17 02:08:16.446668 blue_krill-2.0.2/blue_krill/models/better_loaddata/management/__init__.py
+-rw-r--r--   0        0        0      760 2023-08-17 02:08:16.449554 blue_krill-2.0.2/blue_krill/models/better_loaddata/management/commands/__init__.py
+-rw-r--r--   0        0        0     4997 2023-08-17 02:08:16.449811 blue_krill-2.0.2/blue_krill/models/better_loaddata/management/commands/better_loaddata.py
+-rw-r--r--   0        0        0     1727 2023-08-17 02:08:16.450015 blue_krill-2.0.2/blue_krill/models/fields.py
+-rw-r--r--   0        0        0      760 2023-08-17 02:08:16.451192 blue_krill-2.0.2/blue_krill/monitoring/__init__.py
+-rw-r--r--   0        0        0      760 2023-08-17 02:08:16.451882 blue_krill-2.0.2/blue_krill/monitoring/probe/__init__.py
+-rw-r--r--   0        0        0     3827 2023-08-17 02:08:16.454115 blue_krill-2.0.2/blue_krill/monitoring/probe/base.py
+-rw-r--r--   0        0        0      906 2023-08-17 02:08:16.454324 blue_krill-2.0.2/blue_krill/monitoring/probe/exceptions.py
+-rw-r--r--   0        0        0     3723 2023-08-17 02:08:16.454485 blue_krill-2.0.2/blue_krill/monitoring/probe/http.py
+-rw-r--r--   0        0        0     2689 2023-08-17 02:08:16.454877 blue_krill-2.0.2/blue_krill/monitoring/probe/mysql.py
+-rw-r--r--   0        0        0     2906 2023-08-17 02:08:16.455201 blue_krill-2.0.2/blue_krill/monitoring/probe/redis.py
+-rw-r--r--   0        0        0     1908 2023-08-17 02:08:16.455549 blue_krill-2.0.2/blue_krill/monitoring/probe/tcp.py
+-rw-r--r--   0        0        0      760 2023-08-17 02:08:16.455816 blue_krill-2.0.2/blue_krill/monitoring/prometheus/__init__.py
+-rw-r--r--   0        0        0     5004 2023-08-17 02:08:16.456747 blue_krill-2.0.2/blue_krill/monitoring/prometheus/django_utils.py
+-rw-r--r--   0        0        0     1344 2023-08-17 02:08:16.457095 blue_krill-2.0.2/blue_krill/monitoring/prometheus/setups.py
+-rw-r--r--   0        0        0        0 2023-08-17 02:08:16.457262 blue_krill-2.0.2/blue_krill/py.typed
+-rw-r--r--   0        0        0      760 2023-08-17 02:08:16.457530 blue_krill-2.0.2/blue_krill/redis_tools/__init__.py
+-rw-r--r--   0        0        0     6517 2023-08-17 02:08:16.457770 blue_krill-2.0.2/blue_krill/redis_tools/messaging.py
+-rw-r--r--   0        0        0     3756 2023-08-17 02:08:16.458040 blue_krill-2.0.2/blue_krill/redis_tools/sentinel.py
+-rw-r--r--   0        0        0      760 2023-08-17 02:08:16.458342 blue_krill-2.0.2/blue_krill/secure/__init__.py
+-rw-r--r--   0        0        0     3886 2023-08-17 02:08:16.458605 blue_krill-2.0.2/blue_krill/secure/bk_secure.py
+-rw-r--r--   0        0        0     2233 2023-08-17 02:08:16.458875 blue_krill-2.0.2/blue_krill/secure/dj_environ.py
+-rw-r--r--   0        0        0      760 2023-08-17 02:08:16.459214 blue_krill-2.0.2/blue_krill/storages/__init__.py
+-rw-r--r--   0        0        0      760 2023-08-17 02:08:16.459490 blue_krill-2.0.2/blue_krill/storages/blobstore/__init__.py
+-rw-r--r--   0        0        0     4045 2023-08-17 02:08:16.459758 blue_krill-2.0.2/blue_krill/storages/blobstore/base.py
+-rw-r--r--   0        0        0    13906 2023-08-17 02:08:16.460083 blue_krill-2.0.2/blue_krill/storages/blobstore/bkrepo.py
+-rw-r--r--   0        0        0     1910 2023-08-17 02:08:16.460312 blue_krill-2.0.2/blue_krill/storages/blobstore/exceptions.py
+-rw-r--r--   0        0        0     6262 2023-08-17 02:08:16.460541 blue_krill-2.0.2/blue_krill/storages/blobstore/s3.py
+-rw-r--r--   0        0        0    10889 2023-08-17 02:08:16.460814 blue_krill-2.0.2/blue_krill/termcolors.py
+-rw-r--r--   0        0        0     1666 2023-08-17 02:08:16.461054 blue_krill-2.0.2/blue_krill/text.py
+-rw-r--r--   0        0        0      760 2023-08-17 02:08:16.461395 blue_krill-2.0.2/blue_krill/web/__init__.py
+-rw-r--r--   0        0        0     9697 2023-08-17 02:08:16.461670 blue_krill-2.0.2/blue_krill/web/drf_utils.py
+-rw-r--r--   0        0        0     5644 2023-08-17 02:08:16.461914 blue_krill-2.0.2/blue_krill/web/std_error.py
+-rw-r--r--   0        0        0     1997 2023-08-17 02:08:16.463107 blue_krill-2.0.2/pyproject.toml
+-rw-r--r--   0        0        0    24846 1970-01-01 00:00:00.000000 blue_krill-2.0.2/PKG-INFO
```

### Comparing `blue_krill-2.0.0/README.md` & `blue_krill-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `blue_krill-2.0.0/blue_krill/__init__.py` & `blue_krill-2.0.2/blue_krill/__init__.py`

 * *Files identical despite different names*

### Comparing `blue_krill-2.0.0/blue_krill/async_utils/__init__.py` & `blue_krill-2.0.2/blue_krill/async_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `blue_krill-2.0.0/blue_krill/async_utils/django_utils.py` & `blue_krill-2.0.2/blue_krill/async_utils/django_utils.py`

 * *Files identical despite different names*

### Comparing `blue_krill-2.0.0/blue_krill/async_utils/poll_task.py` & `blue_krill-2.0.2/blue_krill/async_utils/poll_task.py`

 * *Files identical despite different names*

### Comparing `blue_krill-2.0.0/blue_krill/auth/__init__.py` & `blue_krill-2.0.2/blue_krill/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `blue_krill-2.0.0/blue_krill/auth/client.py` & `blue_krill-2.0.2/blue_krill/auth/client.py`

 * *Files identical despite different names*

### Comparing `blue_krill-2.0.0/blue_krill/auth/jwt.py` & `blue_krill-2.0.2/blue_krill/auth/jwt.py`

 * *Files identical despite different names*

### Comparing `blue_krill-2.0.0/blue_krill/auth/utils.py` & `blue_krill-2.0.2/blue_krill/auth/utils.py`

 * *Files identical despite different names*

### Comparing `blue_krill-2.0.0/blue_krill/connections/__init__.py` & `blue_krill-2.0.2/blue_krill/connections/__init__.py`

 * *Files identical despite different names*

### Comparing `blue_krill-2.0.0/blue_krill/connections/exceptions.py` & `blue_krill-2.0.2/blue_krill/connections/exceptions.py`

 * *Files identical despite different names*

### Comparing `blue_krill-2.0.0/blue_krill/connections/ha_algorithm.py` & `blue_krill-2.0.2/blue_krill/connections/ha_algorithm.py`

 * *Files identical despite different names*

### Comparing `blue_krill-2.0.0/blue_krill/connections/ha_endpoint_pool.py` & `blue_krill-2.0.2/blue_krill/connections/ha_endpoint_pool.py`

 * *Files identical despite different names*

### Comparing `blue_krill-2.0.0/blue_krill/contextlib.py` & `blue_krill-2.0.2/blue_krill/contextlib.py`

 * *Files identical despite different names*

### Comparing `blue_krill-2.0.0/blue_krill/cubing_case.py` & `blue_krill-2.0.2/blue_krill/cubing_case.py`

 * *Files identical despite different names*

### Comparing `blue_krill-2.0.0/blue_krill/data_types/__init__.py` & `blue_krill-2.0.2/blue_krill/data_types/__init__.py`

 * *Files identical despite different names*

### Comparing `blue_krill-2.0.0/blue_krill/data_types/enum.py` & `blue_krill-2.0.2/blue_krill/data_types/enum.py`

 * *Files identical despite different names*

### Comparing `blue_krill-2.0.0/blue_krill/data_types/url.py` & `blue_krill-2.0.2/blue_krill/data_types/url.py`

 * *Files identical despite different names*

### Comparing `blue_krill-2.0.0/blue_krill/editions/__init__.py` & `blue_krill-2.0.2/blue_krill/editions/__init__.py`

 * *Files identical despite different names*

### Comparing `blue_krill-2.0.0/blue_krill/editions/editionctl.py` & `blue_krill-2.0.2/blue_krill/editions/editionctl.py`

 * *Files identical despite different names*

### Comparing `blue_krill-2.0.0/blue_krill/encoding.py` & `blue_krill-2.0.2/blue_krill/encoding.py`

 * *Files identical despite different names*

### Comparing `blue_krill-2.0.0/blue_krill/encrypt/__init__.py` & `blue_krill-2.0.2/blue_krill/encrypt/__init__.py`

 * *Files identical despite different names*

### Comparing `blue_krill-2.0.0/blue_krill/encrypt/handler.py` & `blue_krill-2.0.2/blue_krill/encrypt/handler.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,27 +26,31 @@
     def add_header(self, text: str):
         return self.header + text
 
     def strip_header(self, text: str):
         # 兼容无 header 加密串
         if not self.contain_header(text):
             return text
-        return text[len(self.header) :]
+        return text[len(self.header):]
 
     def contain_header(self, text: str) -> bool:
         return text.startswith(self.header)
 
 
 class EncryptHandler:
     cipher_classes: ClassVar[Dict] = {}
 
     def __init__(self, encrypt_cipher_type: Optional[str] = None, secret_key: Optional[bytes] = None):
-        self.encrypt_cipher_type = encrypt_cipher_type or get_default_encrypt_cipher_type()
+        self._encrypt_cipher_type = encrypt_cipher_type
         self.secret_key = secret_key or get_default_secret_key()
 
+    @property
+    def encrypt_cipher_type(self):
+        return self._encrypt_cipher_type or get_default_encrypt_cipher_type()
+
     def encrypt(self, text: str) -> str:
         """根据指定加密算法，加密字段"""
         # 已加密则不处理
         for _, cls in self.cipher_classes.items():
             if cls.header.contain_header(text):
                 return text
 
@@ -95,15 +99,16 @@
 @register_cipher
 class SM4CTR:
     header = _Header("sm4ctr$")
 
     def __init__(self, secret_key: Optional[bytes] = None):
         self.secret_key = secret_key or get_default_secret_key()
         self.cipher = get_symmetric_cipher(
-            common={"key": secret_key},
+            common={"key": self.secret_key},
+            cipher_type=constants.SymmetricCipherType.SM4.value,
             cipher_options={
                 constants.SymmetricCipherType.SM4.value: SM4SymmetricOptions(mode=constants.SymmetricMode.CTR)
             },
         )
 
     def encrypt(self, text: str) -> str:
         return self.header.add_header((self.cipher.encrypt(text)))
```

### Comparing `blue_krill-2.0.0/blue_krill/encrypt/legacy.py` & `blue_krill-2.0.2/blue_krill/encrypt/legacy.py`

 * *Files identical despite different names*

### Comparing `blue_krill-2.0.0/blue_krill/encrypt/utils.py` & `blue_krill-2.0.2/blue_krill/encrypt/utils.py`

 * *Files identical despite different names*

### Comparing `blue_krill-2.0.0/blue_krill/models/__init__.py` & `blue_krill-2.0.2/blue_krill/models/__init__.py`

 * *Files identical despite different names*

### Comparing `blue_krill-2.0.0/blue_krill/models/better_loaddata/__init__.py` & `blue_krill-2.0.2/blue_krill/models/better_loaddata/__init__.py`

 * *Files identical despite different names*

### Comparing `blue_krill-2.0.0/blue_krill/models/better_loaddata/apps.py` & `blue_krill-2.0.2/blue_krill/models/better_loaddata/apps.py`

 * *Files identical despite different names*

### Comparing `blue_krill-2.0.0/blue_krill/models/better_loaddata/management/__init__.py` & `blue_krill-2.0.2/blue_krill/models/better_loaddata/management/__init__.py`

 * *Files identical despite different names*

### Comparing `blue_krill-2.0.0/blue_krill/models/better_loaddata/management/commands/__init__.py` & `blue_krill-2.0.2/blue_krill/models/better_loaddata/management/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `blue_krill-2.0.0/blue_krill/models/better_loaddata/management/commands/better_loaddata.py` & `blue_krill-2.0.2/blue_krill/models/better_loaddata/management/commands/better_loaddata.py`

 * *Files identical despite different names*

### Comparing `blue_krill-2.0.0/blue_krill/models/fields.py` & `blue_krill-2.0.2/blue_krill/models/fields.py`

 * *Files identical despite different names*

### Comparing `blue_krill-2.0.0/blue_krill/monitoring/__init__.py` & `blue_krill-2.0.2/blue_krill/monitoring/__init__.py`

 * *Files identical despite different names*

### Comparing `blue_krill-2.0.0/blue_krill/monitoring/probe/__init__.py` & `blue_krill-2.0.2/blue_krill/monitoring/probe/__init__.py`

 * *Files identical despite different names*

### Comparing `blue_krill-2.0.0/blue_krill/monitoring/probe/base.py` & `blue_krill-2.0.2/blue_krill/monitoring/probe/base.py`

 * *Files identical despite different names*

### Comparing `blue_krill-2.0.0/blue_krill/monitoring/probe/exceptions.py` & `blue_krill-2.0.2/blue_krill/monitoring/probe/exceptions.py`

 * *Files identical despite different names*

### Comparing `blue_krill-2.0.0/blue_krill/monitoring/probe/http.py` & `blue_krill-2.0.2/blue_krill/monitoring/probe/http.py`

 * *Files identical despite different names*

### Comparing `blue_krill-2.0.0/blue_krill/monitoring/probe/mysql.py` & `blue_krill-2.0.2/blue_krill/monitoring/probe/mysql.py`

 * *Files identical despite different names*

### Comparing `blue_krill-2.0.0/blue_krill/monitoring/probe/redis.py` & `blue_krill-2.0.2/blue_krill/monitoring/probe/redis.py`

 * *Files identical despite different names*

### Comparing `blue_krill-2.0.0/blue_krill/monitoring/probe/tcp.py` & `blue_krill-2.0.2/blue_krill/monitoring/probe/tcp.py`

 * *Files identical despite different names*

### Comparing `blue_krill-2.0.0/blue_krill/monitoring/prometheus/__init__.py` & `blue_krill-2.0.2/blue_krill/monitoring/prometheus/__init__.py`

 * *Files identical despite different names*

### Comparing `blue_krill-2.0.0/blue_krill/monitoring/prometheus/django_utils.py` & `blue_krill-2.0.2/blue_krill/monitoring/prometheus/django_utils.py`

 * *Files identical despite different names*

### Comparing `blue_krill-2.0.0/blue_krill/monitoring/prometheus/setups.py` & `blue_krill-2.0.2/blue_krill/monitoring/prometheus/setups.py`

 * *Files identical despite different names*

### Comparing `blue_krill-2.0.0/blue_krill/redis_tools/__init__.py` & `blue_krill-2.0.2/blue_krill/redis_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `blue_krill-2.0.0/blue_krill/redis_tools/messaging.py` & `blue_krill-2.0.2/blue_krill/redis_tools/messaging.py`

 * *Files identical despite different names*

### Comparing `blue_krill-2.0.0/blue_krill/redis_tools/sentinel.py` & `blue_krill-2.0.2/blue_krill/redis_tools/sentinel.py`

 * *Files identical despite different names*

### Comparing `blue_krill-2.0.0/blue_krill/secure/__init__.py` & `blue_krill-2.0.2/blue_krill/secure/__init__.py`

 * *Files identical despite different names*

### Comparing `blue_krill-2.0.0/blue_krill/secure/bk_secure.py` & `blue_krill-2.0.2/blue_krill/secure/bk_secure.py`

 * *Files identical despite different names*

### Comparing `blue_krill-2.0.0/blue_krill/secure/dj_environ.py` & `blue_krill-2.0.2/blue_krill/secure/dj_environ.py`

 * *Files identical despite different names*

### Comparing `blue_krill-2.0.0/blue_krill/storages/__init__.py` & `blue_krill-2.0.2/blue_krill/storages/__init__.py`

 * *Files identical despite different names*

### Comparing `blue_krill-2.0.0/blue_krill/storages/blobstore/__init__.py` & `blue_krill-2.0.2/blue_krill/storages/blobstore/__init__.py`

 * *Files identical despite different names*

### Comparing `blue_krill-2.0.0/blue_krill/storages/blobstore/base.py` & `blue_krill-2.0.2/blue_krill/storages/blobstore/base.py`

 * *Files identical despite different names*

### Comparing `blue_krill-2.0.0/blue_krill/storages/blobstore/bkrepo.py` & `blue_krill-2.0.2/blue_krill/storages/blobstore/bkrepo.py`

 * *Files identical despite different names*

### Comparing `blue_krill-2.0.0/blue_krill/storages/blobstore/exceptions.py` & `blue_krill-2.0.2/blue_krill/storages/blobstore/exceptions.py`

 * *Files identical despite different names*

### Comparing `blue_krill-2.0.0/blue_krill/storages/blobstore/s3.py` & `blue_krill-2.0.2/blue_krill/storages/blobstore/s3.py`

 * *Files identical despite different names*

### Comparing `blue_krill-2.0.0/blue_krill/termcolors.py` & `blue_krill-2.0.2/blue_krill/termcolors.py`

 * *Files identical despite different names*

### Comparing `blue_krill-2.0.0/blue_krill/text.py` & `blue_krill-2.0.2/blue_krill/text.py`

 * *Files identical despite different names*

### Comparing `blue_krill-2.0.0/blue_krill/web/__init__.py` & `blue_krill-2.0.2/blue_krill/web/__init__.py`

 * *Files identical despite different names*

### Comparing `blue_krill-2.0.0/blue_krill/web/drf_utils.py` & `blue_krill-2.0.2/blue_krill/web/drf_utils.py`

 * *Files identical despite different names*

### Comparing `blue_krill-2.0.0/blue_krill/web/std_error.py` & `blue_krill-2.0.2/blue_krill/web/std_error.py`

 * *Files identical despite different names*

### Comparing `blue_krill-2.0.0/pyproject.toml` & `blue_krill-2.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "blue-krill"
-version = "2.0.0"
+version = "2.0.2"
 description = "Tools and common packages for blueking paas"
 license = "Apache License 2.0"
 readme = "README.md"
 authors = ["blueking"]
 include = ["blue_krill/py.typed"]
 
 [tool.poetry.dependencies]
```

### Comparing `blue_krill-2.0.0/PKG-INFO` & `blue_krill-2.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blue-krill
-Version: 2.0.0
+Version: 2.0.2
 Summary: Tools and common packages for blueking paas
 License: Apache-2.0
 Author: blueking
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

