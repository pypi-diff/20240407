# Comparing `tmp/spark_gaps_date_rorc_tools-0.2.0.tar.gz` & `tmp/spark_gaps_date_rorc_tools-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\spark_gaps_date_rorc_tools-0.2.0.tar", last modified: Thu Jan  6 05:13:12 2022, max compression
+gzip compressed data, was "spark_gaps_date_rorc_tools-0.2.1.tar", last modified: Sun Apr  7 06:03:50 2024, max compression
```

## Comparing `spark_gaps_date_rorc_tools-0.2.0.tar` & `spark_gaps_date_rorc_tools-0.2.1.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxrwxrwx   0        0        0        0 2022-01-06 05:13:12.000000 spark_gaps_date_rorc_tools-0.2.0/
--rw-rw-rw-   0        0        0     1092 2021-05-12 14:35:37.000000 spark_gaps_date_rorc_tools-0.2.0/LICENSE
--rw-rw-rw-   0        0        0       54 2021-12-01 07:34:35.000000 spark_gaps_date_rorc_tools-0.2.0/MANIFEST.in
--rw-rw-rw-   0        0        0     3648 2022-01-06 05:13:12.000000 spark_gaps_date_rorc_tools-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     2170 2022-01-06 05:13:08.000000 spark_gaps_date_rorc_tools-0.2.0/README.md
--rw-rw-rw-   0        0        0       86 2022-01-06 05:13:12.000000 spark_gaps_date_rorc_tools-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1249 2022-01-06 05:13:08.000000 spark_gaps_date_rorc_tools-0.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2022-01-06 05:13:12.000000 spark_gaps_date_rorc_tools-0.2.0/spark_gaps_date_rorc_tools/
--rw-rw-rw-   0        0        0      537 2021-12-01 07:23:11.000000 spark_gaps_date_rorc_tools-0.2.0/spark_gaps_date_rorc_tools/__init__.py
-drwxrwxrwx   0        0        0        0 2022-01-06 05:13:12.000000 spark_gaps_date_rorc_tools-0.2.0/spark_gaps_date_rorc_tools/functions/
--rw-rw-rw-   0        0        0        0 2021-06-29 00:15:39.000000 spark_gaps_date_rorc_tools-0.2.0/spark_gaps_date_rorc_tools/functions/__init__.py
--rw-rw-rw-   0        0        0     5547 2022-01-06 05:10:40.000000 spark_gaps_date_rorc_tools-0.2.0/spark_gaps_date_rorc_tools/functions/gaps_date.py
-drwxrwxrwx   0        0        0        0 2022-01-06 05:13:12.000000 spark_gaps_date_rorc_tools-0.2.0/spark_gaps_date_rorc_tools/utils/
--rw-rw-rw-   0        0        0       75 2021-11-24 15:23:35.000000 spark_gaps_date_rorc_tools-0.2.0/spark_gaps_date_rorc_tools/utils/__init__.py
--rw-rw-rw-   0        0        0      331 2021-11-18 05:47:55.000000 spark_gaps_date_rorc_tools-0.2.0/spark_gaps_date_rorc_tools/utils/config.py
--rw-rw-rw-   0        0        0     2522 2021-12-01 22:45:56.000000 spark_gaps_date_rorc_tools-0.2.0/spark_gaps_date_rorc_tools/utils/dataframe.py
--rw-rw-rw-   0        0        0      463 2021-06-29 05:08:46.000000 spark_gaps_date_rorc_tools-0.2.0/spark_gaps_date_rorc_tools/utils/logger.py
--rw-rw-rw-   0        0        0     1056 2021-06-29 05:08:46.000000 spark_gaps_date_rorc_tools-0.2.0/spark_gaps_date_rorc_tools/utils/memory.py
-drwxrwxrwx   0        0        0        0 2022-01-06 05:13:12.000000 spark_gaps_date_rorc_tools-0.2.0/spark_gaps_date_rorc_tools/utils/templates/
--rw-rw-rw-   0        0        0        0 2021-06-29 00:15:39.000000 spark_gaps_date_rorc_tools-0.2.0/spark_gaps_date_rorc_tools/utils/templates/__init__.py
--rw-rw-rw-   0        0        0     1861 2021-12-01 05:37:58.000000 spark_gaps_date_rorc_tools-0.2.0/spark_gaps_date_rorc_tools/utils/templates/table.html
--rw-rw-rw-   0        0        0     1430 2021-06-29 04:59:54.000000 spark_gaps_date_rorc_tools-0.2.0/spark_gaps_date_rorc_tools/utils/time_execution.py
-drwxrwxrwx   0        0        0        0 2022-01-06 05:13:12.000000 spark_gaps_date_rorc_tools-0.2.0/spark_gaps_date_rorc_tools.egg-info/
--rw-rw-rw-   0        0        0     3648 2022-01-06 05:13:10.000000 spark_gaps_date_rorc_tools-0.2.0/spark_gaps_date_rorc_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      815 2022-01-06 05:13:10.000000 spark_gaps_date_rorc_tools-0.2.0/spark_gaps_date_rorc_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-01-06 05:13:10.000000 spark_gaps_date_rorc_tools-0.2.0/spark_gaps_date_rorc_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      214 2022-01-06 05:13:10.000000 spark_gaps_date_rorc_tools-0.2.0/spark_gaps_date_rorc_tools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       27 2022-01-06 05:13:10.000000 spark_gaps_date_rorc_tools-0.2.0/spark_gaps_date_rorc_tools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-07 06:03:50.063581 spark_gaps_date_rorc_tools-0.2.1/
+-rw-rw-rw-   0        0        0     1092 2024-04-07 04:34:08.000000 spark_gaps_date_rorc_tools-0.2.1/LICENSE
+-rw-rw-rw-   0        0        0       54 2024-04-07 04:34:08.000000 spark_gaps_date_rorc_tools-0.2.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     2963 2024-04-07 06:03:50.063581 spark_gaps_date_rorc_tools-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2170 2024-04-07 04:34:08.000000 spark_gaps_date_rorc_tools-0.2.1/README.md
+-rw-rw-rw-   0        0        0      534 2024-04-07 06:02:12.000000 spark_gaps_date_rorc_tools-0.2.1/pyproject.toml
+-rw-rw-rw-   0        0        0       86 2024-04-07 06:03:50.064581 spark_gaps_date_rorc_tools-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     1199 2024-04-07 06:00:01.000000 spark_gaps_date_rorc_tools-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-07 06:03:50.051578 spark_gaps_date_rorc_tools-0.2.1/spark_gaps_date_rorc_tools/
+-rw-rw-rw-   0        0        0      537 2024-04-07 04:34:08.000000 spark_gaps_date_rorc_tools-0.2.1/spark_gaps_date_rorc_tools/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-07 06:03:50.058580 spark_gaps_date_rorc_tools-0.2.1/spark_gaps_date_rorc_tools/functions/
+-rw-rw-rw-   0        0        0        0 2024-04-07 04:34:08.000000 spark_gaps_date_rorc_tools-0.2.1/spark_gaps_date_rorc_tools/functions/__init__.py
+-rw-rw-rw-   0        0        0     5449 2024-04-07 06:00:01.000000 spark_gaps_date_rorc_tools-0.2.1/spark_gaps_date_rorc_tools/functions/gaps_date.py
+drwxrwxrwx   0        0        0        0 2024-04-07 06:03:50.061580 spark_gaps_date_rorc_tools-0.2.1/spark_gaps_date_rorc_tools/utils/
+-rw-rw-rw-   0        0        0       75 2024-04-07 04:34:08.000000 spark_gaps_date_rorc_tools-0.2.1/spark_gaps_date_rorc_tools/utils/__init__.py
+-rw-rw-rw-   0        0        0      331 2024-04-07 04:34:08.000000 spark_gaps_date_rorc_tools-0.2.1/spark_gaps_date_rorc_tools/utils/config.py
+-rw-rw-rw-   0        0        0     2522 2024-04-07 04:34:08.000000 spark_gaps_date_rorc_tools-0.2.1/spark_gaps_date_rorc_tools/utils/dataframe.py
+-rw-rw-rw-   0        0        0      463 2024-04-07 04:34:08.000000 spark_gaps_date_rorc_tools-0.2.1/spark_gaps_date_rorc_tools/utils/logger.py
+-rw-rw-rw-   0        0        0     1056 2024-04-07 04:34:08.000000 spark_gaps_date_rorc_tools-0.2.1/spark_gaps_date_rorc_tools/utils/memory.py
+drwxrwxrwx   0        0        0        0 2024-04-07 06:03:50.062581 spark_gaps_date_rorc_tools-0.2.1/spark_gaps_date_rorc_tools/utils/templates/
+-rw-rw-rw-   0        0        0        0 2024-04-07 04:34:08.000000 spark_gaps_date_rorc_tools-0.2.1/spark_gaps_date_rorc_tools/utils/templates/__init__.py
+-rw-rw-rw-   0        0        0     1861 2024-04-07 04:34:08.000000 spark_gaps_date_rorc_tools-0.2.1/spark_gaps_date_rorc_tools/utils/templates/table.html
+-rw-rw-rw-   0        0        0     1430 2024-04-07 04:34:08.000000 spark_gaps_date_rorc_tools-0.2.1/spark_gaps_date_rorc_tools/utils/time_execution.py
+drwxrwxrwx   0        0        0        0 2024-04-07 06:03:50.056578 spark_gaps_date_rorc_tools-0.2.1/spark_gaps_date_rorc_tools.egg-info/
+-rw-rw-rw-   0        0        0     2963 2024-04-07 06:03:49.000000 spark_gaps_date_rorc_tools-0.2.1/spark_gaps_date_rorc_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      830 2024-04-07 06:03:49.000000 spark_gaps_date_rorc_tools-0.2.1/spark_gaps_date_rorc_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-07 06:03:49.000000 spark_gaps_date_rorc_tools-0.2.1/spark_gaps_date_rorc_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       69 2024-04-07 06:03:49.000000 spark_gaps_date_rorc_tools-0.2.1/spark_gaps_date_rorc_tools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       27 2024-04-07 06:03:49.000000 spark_gaps_date_rorc_tools-0.2.1/spark_gaps_date_rorc_tools.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `spark_gaps_date_rorc_tools-0.2.0/LICENSE` & `spark_gaps_date_rorc_tools-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `spark_gaps_date_rorc_tools-0.2.0/PKG-INFO` & `spark_gaps_date_rorc_tools-0.2.1/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,101 +1,81 @@
-Metadata-Version: 2.1
-Name: spark_gaps_date_rorc_tools
-Version: 0.2.0
-Summary: spark_gaps_date_rorc_tools
-Home-page: https://github.com/jonaqp/spark_gaps_date_rorc_tools/
-Author: Jonathan Quiza
-Author-email: jony327@gmail.com
-License: UNKNOWN
-Download-URL: https://github.com/jonaqp/spark_gaps_date_rorct_tools/archive/main.zip
-Description: # spark_gaps_date_rorc_tools
-        
-        
-        [![Github License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
-        [![Updates](https://pyup.io/repos/github/woctezuma/google-colab-transfer/shield.svg)](pyup)
-        [![Python 3](https://pyup.io/repos/github/woctezuma/google-colab-transfer/python-3-shield.svg)](pyup)
-        [![Code coverage](https://codecov.io/gh/woctezuma/google-colab-transfer/branch/master/graph/badge.svg)](codecov)
-        
-        
-        
-        
-        spark_gaps_date_rorc_tools is a Python library that implements get gaps dates
-        ## Installation
-        
-        The code is packaged for PyPI, so that the installation consists in running:
-        ```sh
-        pip install spark-gaps-date-rorc-tools 
-        ```
-        
-        
-        ## Usage
-        
-        wrapper take gaps dates
-        
-        ```sh
-        config.yaml
-        ===========
-          conf:
-            t_psan_test:
-              table_path: "/data/master/psan/data/t_psan_test/"
-              supplies : [
-                  "/data/master/psan/data/t_ksag_test/",
-                  "/data/master/psan/data/t_psan_test/"
-              ]
-            t_kctk_cust_rating_atrb:
-              table_path: ""
-              supplies : []
-        
-        
-        
-        example1: file.py
-        =================
-        from spark_gaps_date_rorc_tools import show_gaps_date
-        df_pivot = show_gaps_date(spark=spark,
-                                  config_path_name="config.yaml",
-                                  table_rorc=["t_psan_xxx"]
-                                  hdfs_uri="hdfs://pedaaslive.scmx2p100.isi",
-                                  filter_date_initial="202101",
-                                  filter_date_final="202112")
-        
-        Spark Style Dataframe: file.py
-        ==============================                     
-        df_pivot.show2(limit=10)
-        
-        
-        
-        Pandas Style Dataframe: file.py
-        ==============================                 
-        df_pivot2 = df_pivot.toPandas()                      
-        df_pivot2.show2()
-        
-        ```
-        
-        ## License
-        
-        [Apache License 2.0](https://www.dropbox.com/s/8t6xtgk06o3ij61/LICENSE?dl=0).
-        
-        
-        ## New features v1.0
-        
-         
-        ## BugFix
-        - choco install visualcpp-build-tools
-        
-        
-        
-        ## Reference
-        
-         - Jonathan Quiza [github](https://github.com/jonaqp).
-         - Jonathan Quiza [RumiMLSpark](http://rumi-ml.herokuapp.com/).
-         - Jonathan Quiza [linkedin](https://www.linkedin.com/in/jonaqp/).
-        
-Keywords: spark,gaps,date
-Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Science/Research
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.7
-Description-Content-Type: text/markdown
+# spark_gaps_date_rorc_tools
+
+
+[![Github License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
+[![Updates](https://pyup.io/repos/github/woctezuma/google-colab-transfer/shield.svg)](pyup)
+[![Python 3](https://pyup.io/repos/github/woctezuma/google-colab-transfer/python-3-shield.svg)](pyup)
+[![Code coverage](https://codecov.io/gh/woctezuma/google-colab-transfer/branch/master/graph/badge.svg)](codecov)
+
+
+
+
+spark_gaps_date_rorc_tools is a Python library that implements get gaps dates
+## Installation
+
+The code is packaged for PyPI, so that the installation consists in running:
+```sh
+pip install spark-gaps-date-rorc-tools 
+```
+
+
+## Usage
+
+wrapper take gaps dates
+
+```sh
+config.yaml
+===========
+  conf:
+    t_psan_test:
+      table_path: "/data/master/psan/data/t_psan_test/"
+      supplies : [
+          "/data/master/psan/data/t_ksag_test/",
+          "/data/master/psan/data/t_psan_test/"
+      ]
+    t_kctk_cust_rating_atrb:
+      table_path: ""
+      supplies : []
+
+
+
+example1: file.py
+=================
+from spark_gaps_date_rorc_tools import show_gaps_date
+df_pivot = show_gaps_date(spark=spark,
+                          config_path_name="config.yaml",
+                          table_rorc=["t_psan_xxx"]
+                          hdfs_uri="hdfs://pedaaslive.scmx2p100.isi",
+                          filter_date_initial="202101",
+                          filter_date_final="202112")
+
+Spark Style Dataframe: file.py
+==============================                     
+df_pivot.show2(limit=10)
+
+
+
+Pandas Style Dataframe: file.py
+==============================                 
+df_pivot2 = df_pivot.toPandas()                      
+df_pivot2.show2()
+
+```
+
+## License
+
+[Apache License 2.0](https://www.dropbox.com/s/8t6xtgk06o3ij61/LICENSE?dl=0).
+
+
+## New features v1.0
+
+ 
+## BugFix
+- choco install visualcpp-build-tools
+
+
+
+## Reference
+
+ - Jonathan Quiza [github](https://github.com/jonaqp).
+ - Jonathan Quiza [RumiMLSpark](http://rumi-ml.herokuapp.com/).
+ - Jonathan Quiza [linkedin](https://www.linkedin.com/in/jonaqp/).
```

### Comparing `spark_gaps_date_rorc_tools-0.2.0/README.md` & `spark_gaps_date_rorc_tools-0.2.1/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,27 @@
+Metadata-Version: 2.1
+Name: spark_gaps_date_rorc_tools
+Version: 0.2.1
+Summary: spark_gaps_date_rorc_tools
+Home-page: https://github.com/jonaqp/spark_gaps_date_rorc_tools/
+Author: Jonathan Quiza
+Author-email: jony327@gmail.com
+License: UNKNOWN
+Download-URL: https://github.com/jonaqp/spark_gaps_date_rorct_tools/archive/main.zip
+Keywords: spark,gaps,date
+Platform: UNKNOWN
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # spark_gaps_date_rorc_tools
 
 
 [![Github License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![Updates](https://pyup.io/repos/github/woctezuma/google-colab-transfer/shield.svg)](pyup)
 [![Python 3](https://pyup.io/repos/github/woctezuma/google-colab-transfer/python-3-shield.svg)](pyup)
 [![Code coverage](https://codecov.io/gh/woctezuma/google-colab-transfer/branch/master/graph/badge.svg)](codecov)
@@ -75,7 +95,9 @@
 
 
 ## Reference
 
  - Jonathan Quiza [github](https://github.com/jonaqp).
  - Jonathan Quiza [RumiMLSpark](http://rumi-ml.herokuapp.com/).
  - Jonathan Quiza [linkedin](https://www.linkedin.com/in/jonaqp/).
+
+
```

### Comparing `spark_gaps_date_rorc_tools-0.2.0/setup.py` & `spark_gaps_date_rorc_tools-0.2.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import find_packages
 
 setuppath = os.path.dirname(os.path.abspath(__file__))
 
 setup(
     name='spark_gaps_date_rorc_tools',
     packages=find_packages(),
-    version='0.2.0',
+    version='0.2.1',
     description='spark_gaps_date_rorc_tools',
     long_description=open(os.path.join(setuppath, 'README.md')).read(),
     long_description_content_type="text/markdown",
     author='Jonathan Quiza',
     author_email='jony327@gmail.com',
     url='https://github.com/jonaqp/spark_gaps_date_rorc_tools/',
     download_url='https://github.com/jonaqp/spark_gaps_date_rorct_tools/archive/main.zip',
@@ -21,11 +21,10 @@
     include_package_data=True,
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'Intended Audience :: Science/Research',
         'Topic :: Scientific/Engineering :: Artificial Intelligence',
         'License :: OSI Approved :: Apache Software License',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.9',
     ],
 )
```

### Comparing `spark_gaps_date_rorc_tools-0.2.0/spark_gaps_date_rorc_tools/__init__.py` & `spark_gaps_date_rorc_tools-0.2.1/spark_gaps_date_rorc_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `spark_gaps_date_rorc_tools-0.2.0/spark_gaps_date_rorc_tools/functions/gaps_date.py` & `spark_gaps_date_rorc_tools-0.2.1/spark_gaps_date_rorc_tools/functions/gaps_date.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import gc
-
 import numpy as np
 import pandas as pd
 import pyspark
+
 from spark_gaps_date_rorc_tools.utils.config import load_config
-from spark_gaps_date_rorc_tools.utils.dataframe import show_spark_df
 from spark_gaps_date_rorc_tools.utils.dataframe import show_pd_df
+from spark_gaps_date_rorc_tools.utils.dataframe import show_spark_df
 
 
 def show_gaps_date(spark=None,
                    config_path_name=None,
                    hdfs_uri=None,
                    table_rorc=None,
                    filter_date_initial="202101",
@@ -35,17 +35,14 @@
     FileSystem = sc._gateway.jvm.org.apache.hadoop.fs.FileSystem
     Configuration = sc._gateway.jvm.org.apache.hadoop.conf.Configuration
     fs = FileSystem.get(URI(f"{hdfs_uri}"), Configuration())
 
     data = load_config(path_name=f"{config_path_name}")
     conf_table_job_dict = data["conf"]
 
-    pyspark.sql.dataframe.DataFrame.show2 = show_spark_df
-    pd.DataFrame.show2 = show_pd_df
-
     if table_rorc in ("", None):
         table_list = [key for key, value in conf_table_job_dict.items()]
     else:
         table_list = [key for key, value in conf_table_job_dict.items() if key in table_rorc]
 
     global df_detail
     global df_detail2
```

### Comparing `spark_gaps_date_rorc_tools-0.2.0/spark_gaps_date_rorc_tools/utils/dataframe.py` & `spark_gaps_date_rorc_tools-0.2.1/spark_gaps_date_rorc_tools/utils/dataframe.py`

 * *Files identical despite different names*

### Comparing `spark_gaps_date_rorc_tools-0.2.0/spark_gaps_date_rorc_tools/utils/memory.py` & `spark_gaps_date_rorc_tools-0.2.1/spark_gaps_date_rorc_tools/utils/memory.py`

 * *Files identical despite different names*

### Comparing `spark_gaps_date_rorc_tools-0.2.0/spark_gaps_date_rorc_tools/utils/templates/table.html` & `spark_gaps_date_rorc_tools-0.2.1/spark_gaps_date_rorc_tools/utils/templates/table.html`

 * *Files identical despite different names*

### Comparing `spark_gaps_date_rorc_tools-0.2.0/spark_gaps_date_rorc_tools/utils/time_execution.py` & `spark_gaps_date_rorc_tools-0.2.1/spark_gaps_date_rorc_tools/utils/time_execution.py`

 * *Files identical despite different names*

### Comparing `spark_gaps_date_rorc_tools-0.2.0/spark_gaps_date_rorc_tools.egg-info/SOURCES.txt` & `spark_gaps_date_rorc_tools-0.2.1/spark_gaps_date_rorc_tools.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 LICENSE
 MANIFEST.in
 README.md
+pyproject.toml
 setup.cfg
 setup.py
 spark_gaps_date_rorc_tools/__init__.py
 spark_gaps_date_rorc_tools.egg-info/PKG-INFO
 spark_gaps_date_rorc_tools.egg-info/SOURCES.txt
 spark_gaps_date_rorc_tools.egg-info/dependency_links.txt
 spark_gaps_date_rorc_tools.egg-info/requires.txt
```

