# Comparing `tmp/aws-delete-all-0.5.4.tar.gz` & `tmp/aws-delete-all-0.5.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws-delete-all-0.5.4.tar", last modified: Tue Mar 19 22:47:28 2024, max compression
+gzip compressed data, was "aws-delete-all-0.5.4.1.tar", last modified: Tue Mar 19 22:52:42 2024, max compression
```

## Comparing `aws-delete-all-0.5.4.tar` & `aws-delete-all-0.5.4.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 synan      (501) staff       (20)        0 2024-03-19 22:47:28.443620 aws-delete-all-0.5.4/
--rw-r--r--   0 synan      (501) staff       (20)     1101 2024-03-19 21:27:33.000000 aws-delete-all-0.5.4/LICENSE
--rw-r--r--   0 synan      (501) staff       (20)     3695 2024-03-19 22:47:28.443395 aws-delete-all-0.5.4/PKG-INFO
--rw-r--r--   0 synan      (501) staff       (20)     3112 2024-03-19 22:19:20.000000 aws-delete-all-0.5.4/README.md
-drwxr-xr-x   0 synan      (501) staff       (20)        0 2024-03-19 22:47:28.443019 aws-delete-all-0.5.4/aws_delete_all.egg-info/
--rw-r--r--   0 synan      (501) staff       (20)     3695 2024-03-19 22:47:28.000000 aws-delete-all-0.5.4/aws_delete_all.egg-info/PKG-INFO
--rw-r--r--   0 synan      (501) staff       (20)      264 2024-03-19 22:47:28.000000 aws-delete-all-0.5.4/aws_delete_all.egg-info/SOURCES.txt
--rw-r--r--   0 synan      (501) staff       (20)        1 2024-03-19 22:47:28.000000 aws-delete-all-0.5.4/aws_delete_all.egg-info/dependency_links.txt
--rw-r--r--   0 synan      (501) staff       (20)       45 2024-03-19 22:47:28.000000 aws-delete-all-0.5.4/aws_delete_all.egg-info/entry_points.txt
--rw-r--r--   0 synan      (501) staff       (20)       13 2024-03-19 22:47:28.000000 aws-delete-all-0.5.4/aws_delete_all.egg-info/requires.txt
--rw-r--r--   0 synan      (501) staff       (20)        5 2024-03-19 22:47:28.000000 aws-delete-all-0.5.4/aws_delete_all.egg-info/top_level.txt
--rw-r--r--   0 synan      (501) staff       (20)    87145 2024-03-19 22:13:34.000000 aws-delete-all-0.5.4/main.py
--rw-r--r--   0 synan      (501) staff       (20)       38 2024-03-19 22:47:28.443672 aws-delete-all-0.5.4/setup.cfg
--rw-r--r--   0 synan      (501) staff       (20)     1006 2024-03-19 22:44:57.000000 aws-delete-all-0.5.4/setup.py
+drwxr-xr-x   0 synan      (501) staff       (20)        0 2024-03-19 22:52:42.162579 aws-delete-all-0.5.4.1/
+-rw-r--r--   0 synan      (501) staff       (20)     1101 2024-03-19 21:27:33.000000 aws-delete-all-0.5.4.1/LICENSE
+-rw-r--r--   0 synan      (501) staff       (20)     3697 2024-03-19 22:52:42.162334 aws-delete-all-0.5.4.1/PKG-INFO
+-rw-r--r--   0 synan      (501) staff       (20)     3112 2024-03-19 22:19:20.000000 aws-delete-all-0.5.4.1/README.md
+drwxr-xr-x   0 synan      (501) staff       (20)        0 2024-03-19 22:52:42.161928 aws-delete-all-0.5.4.1/aws_delete_all.egg-info/
+-rw-r--r--   0 synan      (501) staff       (20)     3697 2024-03-19 22:52:42.000000 aws-delete-all-0.5.4.1/aws_delete_all.egg-info/PKG-INFO
+-rw-r--r--   0 synan      (501) staff       (20)      264 2024-03-19 22:52:42.000000 aws-delete-all-0.5.4.1/aws_delete_all.egg-info/SOURCES.txt
+-rw-r--r--   0 synan      (501) staff       (20)        1 2024-03-19 22:52:42.000000 aws-delete-all-0.5.4.1/aws_delete_all.egg-info/dependency_links.txt
+-rw-r--r--   0 synan      (501) staff       (20)       45 2024-03-19 22:52:42.000000 aws-delete-all-0.5.4.1/aws_delete_all.egg-info/entry_points.txt
+-rw-r--r--   0 synan      (501) staff       (20)       13 2024-03-19 22:52:42.000000 aws-delete-all-0.5.4.1/aws_delete_all.egg-info/requires.txt
+-rw-r--r--   0 synan      (501) staff       (20)        5 2024-03-19 22:52:42.000000 aws-delete-all-0.5.4.1/aws_delete_all.egg-info/top_level.txt
+-rw-r--r--   0 synan      (501) staff       (20)    87182 2024-03-19 22:51:47.000000 aws-delete-all-0.5.4.1/main.py
+-rw-r--r--   0 synan      (501) staff       (20)       38 2024-03-19 22:52:42.162765 aws-delete-all-0.5.4.1/setup.cfg
+-rw-r--r--   0 synan      (501) staff       (20)     1008 2024-03-19 22:52:36.000000 aws-delete-all-0.5.4.1/setup.py
```

### Comparing `aws-delete-all-0.5.4/LICENSE` & `aws-delete-all-0.5.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aws-delete-all-0.5.4/PKG-INFO` & `aws-delete-all-0.5.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-delete-all
-Version: 0.5.4
+Version: 0.5.4.1
 Summary: A script that concurrently deletes common AWS resources like S3 buckets, RDS instances, and EC2 instances across all AWS regions.
 Home-page: https://github.com/sinanartun/aws_delete_all
 Author: Sinan Artun
 Author-email: sinanartun@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `aws-delete-all-0.5.4/README.md` & `aws-delete-all-0.5.4.1/README.md`

 * *Files identical despite different names*

### Comparing `aws-delete-all-0.5.4/aws_delete_all.egg-info/PKG-INFO` & `aws-delete-all-0.5.4.1/aws_delete_all.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-delete-all
-Version: 0.5.4
+Version: 0.5.4.1
 Summary: A script that concurrently deletes common AWS resources like S3 buckets, RDS instances, and EC2 instances across all AWS regions.
 Home-page: https://github.com/sinanartun/aws_delete_all
 Author: Sinan Artun
 Author-email: sinanartun@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `aws-delete-all-0.5.4/main.py` & `aws-delete-all-0.5.4.1/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -1964,10 +1964,12 @@
                     sqs_client.delete_queue(QueueUrl=queue_url)
                     logger.info(f"Deleted queue: {queue_url}")
                 except Exception as e:
                     logger.error(f"Error deleting queue {queue_url}: {e}")
                     continue
             logger.success(f"Deleting queue end for region: {region_name}")
 
+def main():
+    AwsDeleteAll().run()
 
 if __name__ == "__main__":
     AwsDeleteAll().run()
```

### Comparing `aws-delete-all-0.5.4/setup.py` & `aws-delete-all-0.5.4.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='aws-delete-all',
-    version='0.5.4',
+    version='0.5.4.1',
     author='Sinan Artun',
     author_email='sinanartun@gmail.com',
     description='A script that concurrently deletes common AWS resources like S3 buckets, RDS instances, and EC2 instances across all AWS regions.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/sinanartun/aws_delete_all',
     packages=find_packages(),
```

