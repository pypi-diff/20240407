# Comparing `tmp/gammarer.aws-secure-flow-log-bucket-1.3.3.tar.gz` & `tmp/gammarer.aws-secure-flow-log-bucket-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gammarer.aws-secure-flow-log-bucket-1.3.3.tar", last modified: Sun Mar 31 19:20:00 2024, max compression
+gzip compressed data, was "gammarer.aws-secure-flow-log-bucket-1.3.4.tar", last modified: Sun Apr  7 19:19:25 2024, max compression
```

## Comparing `gammarer.aws-secure-flow-log-bucket-1.3.3.tar` & `gammarer.aws-secure-flow-log-bucket-1.3.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 19:20:00.355817 gammarer.aws-secure-flow-log-bucket-1.3.3/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-03-31 19:19:48.000000 gammarer.aws-secure-flow-log-bucket-1.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-03-31 19:19:48.000000 gammarer.aws-secure-flow-log-bucket-1.3.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3442 2024-03-31 19:20:00.355817 gammarer.aws-secure-flow-log-bucket-1.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2506 2024-03-31 19:19:48.000000 gammarer.aws-secure-flow-log-bucket-1.3.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-03-31 19:19:48.000000 gammarer.aws-secure-flow-log-bucket-1.3.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-31 19:20:00.355817 gammarer.aws-secure-flow-log-bucket-1.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-03-31 19:19:48.000000 gammarer.aws-secure-flow-log-bucket-1.3.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 19:20:00.351817 gammarer.aws-secure-flow-log-bucket-1.3.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 19:20:00.351817 gammarer.aws-secure-flow-log-bucket-1.3.3/src/gammarer/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 19:20:00.351817 gammarer.aws-secure-flow-log-bucket-1.3.3/src/gammarer/aws_secure_flow_log_bucket/
--rw-r--r--   0 runner    (1001) docker     (127)     9821 2024-03-31 19:19:48.000000 gammarer.aws-secure-flow-log-bucket-1.3.3/src/gammarer/aws_secure_flow_log_bucket/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 19:20:00.355817 gammarer.aws-secure-flow-log-bucket-1.3.3/src/gammarer/aws_secure_flow_log_bucket/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-03-31 19:19:48.000000 gammarer.aws-secure-flow-log-bucket-1.3.3/src/gammarer/aws_secure_flow_log_bucket/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24324 2024-03-31 19:19:48.000000 gammarer.aws-secure-flow-log-bucket-1.3.3/src/gammarer/aws_secure_flow_log_bucket/_jsii/aws-secure-flow-log-bucket@1.3.3.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-31 19:19:48.000000 gammarer.aws-secure-flow-log-bucket-1.3.3/src/gammarer/aws_secure_flow_log_bucket/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 19:20:00.351817 gammarer.aws-secure-flow-log-bucket-1.3.3/src/gammarer.aws_secure_flow_log_bucket.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3442 2024-03-31 19:20:00.000000 gammarer.aws-secure-flow-log-bucket-1.3.3/src/gammarer.aws_secure_flow_log_bucket.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-03-31 19:20:00.000000 gammarer.aws-secure-flow-log-bucket-1.3.3/src/gammarer.aws_secure_flow_log_bucket.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-31 19:20:00.000000 gammarer.aws-secure-flow-log-bucket-1.3.3/src/gammarer.aws_secure_flow_log_bucket.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-03-31 19:20:00.000000 gammarer.aws-secure-flow-log-bucket-1.3.3/src/gammarer.aws_secure_flow_log_bucket.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-31 19:20:00.000000 gammarer.aws-secure-flow-log-bucket-1.3.3/src/gammarer.aws_secure_flow_log_bucket.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 19:19:25.157124 gammarer.aws-secure-flow-log-bucket-1.3.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-07 19:19:14.000000 gammarer.aws-secure-flow-log-bucket-1.3.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-07 19:19:14.000000 gammarer.aws-secure-flow-log-bucket-1.3.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3442 2024-04-07 19:19:25.157124 gammarer.aws-secure-flow-log-bucket-1.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2506 2024-04-07 19:19:14.000000 gammarer.aws-secure-flow-log-bucket-1.3.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-07 19:19:14.000000 gammarer.aws-secure-flow-log-bucket-1.3.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 19:19:25.157124 gammarer.aws-secure-flow-log-bucket-1.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-04-07 19:19:14.000000 gammarer.aws-secure-flow-log-bucket-1.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 19:19:25.153124 gammarer.aws-secure-flow-log-bucket-1.3.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 19:19:25.153124 gammarer.aws-secure-flow-log-bucket-1.3.4/src/gammarer/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 19:19:25.153124 gammarer.aws-secure-flow-log-bucket-1.3.4/src/gammarer/aws_secure_flow_log_bucket/
+-rw-r--r--   0 runner    (1001) docker     (127)     9821 2024-04-07 19:19:14.000000 gammarer.aws-secure-flow-log-bucket-1.3.4/src/gammarer/aws_secure_flow_log_bucket/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 19:19:25.157124 gammarer.aws-secure-flow-log-bucket-1.3.4/src/gammarer/aws_secure_flow_log_bucket/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-07 19:19:14.000000 gammarer.aws-secure-flow-log-bucket-1.3.4/src/gammarer/aws_secure_flow_log_bucket/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24324 2024-04-07 19:19:14.000000 gammarer.aws-secure-flow-log-bucket-1.3.4/src/gammarer/aws_secure_flow_log_bucket/_jsii/aws-secure-flow-log-bucket@1.3.4.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 19:19:14.000000 gammarer.aws-secure-flow-log-bucket-1.3.4/src/gammarer/aws_secure_flow_log_bucket/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 19:19:25.153124 gammarer.aws-secure-flow-log-bucket-1.3.4/src/gammarer.aws_secure_flow_log_bucket.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3442 2024-04-07 19:19:25.000000 gammarer.aws-secure-flow-log-bucket-1.3.4/src/gammarer.aws_secure_flow_log_bucket.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-07 19:19:25.000000 gammarer.aws-secure-flow-log-bucket-1.3.4/src/gammarer.aws_secure_flow_log_bucket.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 19:19:25.000000 gammarer.aws-secure-flow-log-bucket-1.3.4/src/gammarer.aws_secure_flow_log_bucket.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-07 19:19:25.000000 gammarer.aws-secure-flow-log-bucket-1.3.4/src/gammarer.aws_secure_flow_log_bucket.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-07 19:19:25.000000 gammarer.aws-secure-flow-log-bucket-1.3.4/src/gammarer.aws_secure_flow_log_bucket.egg-info/top_level.txt
```

### Comparing `gammarer.aws-secure-flow-log-bucket-1.3.3/LICENSE` & `gammarer.aws-secure-flow-log-bucket-1.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `gammarer.aws-secure-flow-log-bucket-1.3.3/PKG-INFO` & `gammarer.aws-secure-flow-log-bucket-1.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gammarer.aws-secure-flow-log-bucket
-Version: 1.3.3
+Version: 1.3.4
 Summary: Specific AWS VPC FlowLog Bucket
 Home-page: https://github.com/gammarer/aws-secure-flow-log-bucket.git
 Author: yicr<yicr@users.noreply.github.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/gammarer/aws-secure-flow-log-bucket.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `gammarer.aws-secure-flow-log-bucket-1.3.3/README.md` & `gammarer.aws-secure-flow-log-bucket-1.3.4/README.md`

 * *Files identical despite different names*

### Comparing `gammarer.aws-secure-flow-log-bucket-1.3.3/setup.py` & `gammarer.aws-secure-flow-log-bucket-1.3.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "gammarer.aws-secure-flow-log-bucket",
-    "version": "1.3.3",
+    "version": "1.3.4",
     "description": "Specific AWS VPC FlowLog Bucket",
     "license": "Apache-2.0",
     "url": "https://github.com/gammarer/aws-secure-flow-log-bucket.git",
     "long_description_content_type": "text/markdown",
     "author": "yicr<yicr@users.noreply.github.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "gammarer.aws_secure_flow_log_bucket",
         "gammarer.aws_secure_flow_log_bucket._jsii"
     ],
     "package_data": {
         "gammarer.aws_secure_flow_log_bucket._jsii": [
-            "aws-secure-flow-log-bucket@1.3.3.jsii.tgz"
+            "aws-secure-flow-log-bucket@1.3.4.jsii.tgz"
         ],
         "gammarer.aws_secure_flow_log_bucket": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
```

### Comparing `gammarer.aws-secure-flow-log-bucket-1.3.3/src/gammarer/aws_secure_flow_log_bucket/__init__.py` & `gammarer.aws-secure-flow-log-bucket-1.3.4/src/gammarer/aws_secure_flow_log_bucket/__init__.py`

 * *Files identical despite different names*

### Comparing `gammarer.aws-secure-flow-log-bucket-1.3.3/src/gammarer/aws_secure_flow_log_bucket/_jsii/__init__.py` & `gammarer.aws-secure-flow-log-bucket-1.3.4/src/gammarer/aws_secure_flow_log_bucket/_jsii/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,17 +16,17 @@
 import aws_cdk._jsii
 import constructs._jsii
 import gammarer.aws_secure_bucket._jsii
 import gammarer.aws_secure_log_bucket._jsii
 
 __jsii_assembly__ = jsii.JSIIAssembly.load(
     "@gammarer/aws-secure-flow-log-bucket",
-    "1.3.3",
+    "1.3.4",
     __name__[0:-6],
-    "aws-secure-flow-log-bucket@1.3.3.jsii.tgz",
+    "aws-secure-flow-log-bucket@1.3.4.jsii.tgz",
 )
 
 __all__ = [
     "__jsii_assembly__",
 ]
 
 publication.publish()
```

### Comparing `gammarer.aws-secure-flow-log-bucket-1.3.3/src/gammarer/aws_secure_flow_log_bucket/_jsii/aws-secure-flow-log-bucket@1.3.3.jsii.tgz` & `gammarer.aws-secure-flow-log-bucket-1.3.4/src/gammarer/aws_secure_flow_log_bucket/_jsii/aws-secure-flow-log-bucket@1.3.4.jsii.tgz`

 * *Files 20% similar despite different names*

#### Comparing `aws-secure-flow-log-bucket@1.3.3.jsii.tgz-content` & `aws-secure-flow-log-bucket@1.3.4.jsii.tgz-content`

##### package/.jsii

###### Pretty-printed

 * *Similarity: 0.9444444444444444%*

 * *Differences: {"'fingerprint'": "'0CDsFnUqjWC9Q6Ehn/RcphD/+QApSjdstfk/PRcpZBg='", "'version'": "'1.3.4'"}*

```diff
@@ -3494,15 +3494,15 @@
             }
         }
     },
     "description": "Specific AWS VPC FlowLog Bucket",
     "docs": {
         "stability": "stable"
     },
-    "fingerprint": "vSKMM/xhTNwhXqam9ywSRgG40QJ4UNC3n76nWyn2WD4=",
+    "fingerprint": "0CDsFnUqjWC9Q6Ehn/RcphD/+QApSjdstfk/PRcpZBg=",
     "homepage": "https://github.com/gammarer/aws-secure-flow-log-bucket.git",
     "jsiiVersion": "5.2.44 (build ff4e411)",
     "keywords": [
         "aws",
         "aws-cdk",
         "bucket",
         "cdk",
@@ -3632,9 +3632,9 @@
                         }
                     }
                 }
             ],
             "symbolId": "src/index:SecureFlowLogBucketProps"
         }
     },
-    "version": "1.3.3"
+    "version": "1.3.4"
 }
```

##### package/lib/index.js

###### js-beautify {}

```diff
@@ -48,10 +48,10 @@
         }));
     }
 }
 exports.SecureFlowLogBucket = SecureFlowLogBucket;
 _a = JSII_RTTI_SYMBOL_1;
 SecureFlowLogBucket[_a] = {
     fqn: "@gammarer/aws-secure-flow-log-bucket.SecureFlowLogBucket",
-    version: "1.3.3"
+    version: "1.3.4"
 };
 //# sourceMappingURL=data:application/json;base64,eyJ2ZXJzaW9uIjozLCJmaWxlIjoiaW5kZXguanMiLCJzb3VyY2VSb290IjoiIiwic291cmNlcyI6WyIuLi9zcmMvaW5kZXgudHMiXSwibmFtZXMiOltdLCJtYXBwaW5ncyI6Ijs7Ozs7QUFBQSwyRUFBd0Y7QUFDeEYsbUNBQW1DO0FBQ25DLDJDQUEyQztBQU8zQyxNQUFhLG1CQUFvQixTQUFRLHVDQUFlO0lBQ3RELFlBQVksS0FBZ0IsRUFBRSxFQUFVLEVBQUUsS0FBZ0M7UUFDeEUsS0FBSyxDQUFDLEtBQUssRUFBRSxFQUFFLEVBQUUsS0FBSyxDQUFDLENBQUM7UUFFeEIsd0JBQXdCO1FBQ3hCLE1BQU0sT0FBTyxHQUFHLEdBQUcsQ0FBQyxLQUFLLENBQUMsRUFBRSxDQUFDLElBQUksQ0FBQyxDQUFDLE9BQU8sQ0FBQztRQUUzQyxpQkFBaUI7UUFDakIsSUFBSSxDQUFDLG1CQUFtQixDQUFDLElBQUksR0FBRyxDQUFDLGVBQWUsQ0FBQztZQUMvQyxNQUFNLEVBQUUsR0FBRyxDQUFDLE1BQU0sQ0FBQyxLQUFLO1lBQ3hCLE9BQU8sRUFBRSxDQUFDLGlCQUFpQixDQUFDO1lBQzVCLFVBQVUsRUFBRTtnQkFDVixJQUFJLEdBQUcsQ0FBQyxnQkFBZ0IsQ0FBQyw2QkFBNkIsQ0FBQzthQUN4RDtZQUNELFNBQVMsRUFBRSxDQUFDLElBQUksQ0FBQyxTQUFTLENBQUM7U0FDNUIsQ0FBQyxDQUFDLENBQUM7UUFFSixrQkFBa0I7UUFDbEIsSUFBSSxDQUFDLG1CQUFtQixDQUFDLElBQUksR0FBRyxDQUFDLGVBQWUsQ0FBQztZQUMvQyxNQUFNLEVBQUUsR0FBRyxDQUFDLE1BQU0sQ0FBQyxLQUFLO1lBQ3hCLE9BQU8sRUFBRSxDQUFDLGNBQWMsQ0FBQztZQUN6QixVQUFVLEVBQUU7Z0JBQ1YsSUFBSSxHQUFHLENBQUMsZ0JBQWdCLENBQUMsNkJBQTZCLENBQUM7YUFDeEQ7WUFDRCx3REFBd0Q7WUFDeEQsU0FBUyxFQUFFLENBQUMsR0FBRyxFQUFFO2dCQUNmLElBQUksS0FBSyxFQUFFLFdBQVcsSUFBSSxLQUFLLENBQUMsV0FBVyxDQUFDLE1BQU0sR0FBRyxDQUFDLEVBQUU7b0JBQ3RELE1BQU0sU0FBUyxHQUFrQixFQUFFLENBQUM7b0JBQ3BDLEtBQUssTUFBTSxTQUFTLElBQUksS0FBSyxDQUFDLFdBQVcsRUFBRTt3QkFDekMsU0FBUyxDQUFDLElBQUksQ0FBQyxHQUFHLElBQUksQ0FBQyxTQUFTLElBQUksU0FBUyxZQUFZLE9BQU8sSUFBSSxDQUFDLENBQUM7cUJBQ3ZFO29CQUNELE9BQU8sU0FBUyxDQUFDO2lCQUNsQjtnQkFDRCxPQUFPLENBQUMsR0FBRyxJQUFJLENBQUMsU0FBUyxZQUFZLE9BQU8sSUFBSSxDQUFDLENBQUM7WUFDcEQsQ0FBQyxDQUFDLEVBQUU7WUFDSixVQUFVLEVBQUU7Z0JBQ1YsWUFBWSxFQUFFO29CQUNaLGNBQWMsRUFBRSwyQkFBMkI7aUJBQzVDO2FBQ0Y7U0FDRixDQUFDLENBQUMsQ0FBQztJQUVOLENBQUM7O0FBMUNILGtEQTJDQyIsInNvdXJjZXNDb250ZW50IjpbImltcG9ydCB7IFNlY3VyZUxvZ0J1Y2tldCwgU2VjdXJlTG9nQnVja2V0UHJvcHMgfSBmcm9tICdAZ2FtbWFyZXIvYXdzLXNlY3VyZS1sb2ctYnVja2V0JztcbmltcG9ydCAqIGFzIGNkayBmcm9tICdhd3MtY2RrLWxpYic7XG5pbXBvcnQgKiBhcyBpYW0gZnJvbSAnYXdzLWNkay1saWIvYXdzLWlhbSc7XG5pbXBvcnQgeyBDb25zdHJ1Y3QgfSBmcm9tICdjb25zdHJ1Y3RzJztcblxuZXhwb3J0IGludGVyZmFjZSBTZWN1cmVGbG93TG9nQnVja2V0UHJvcHMgZXh0ZW5kcyBTZWN1cmVMb2dCdWNrZXRQcm9wcyB7XG4gIHJlYWRvbmx5IGtleVByZWZpeGVzPzogc3RyaW5nW107XG59XG5cbmV4cG9ydCBjbGFzcyBTZWN1cmVGbG93TG9nQnVja2V0IGV4dGVuZHMgU2VjdXJlTG9nQnVja2V0IHtcbiAgY29uc3RydWN0b3Ioc2NvcGU6IENvbnN0cnVjdCwgaWQ6IHN0cmluZywgcHJvcHM/OiBTZWN1cmVGbG93TG9nQnVja2V0UHJvcHMpIHtcbiAgICBzdXBlcihzY29wZSwgaWQsIHByb3BzKTtcblxuICAgIC8vIPCfkYdHZXQgY3VycmVudCBhY2NvdW50XG4gICAgY29uc3QgYWNjb3VudCA9IGNkay5TdGFjay5vZih0aGlzKS5hY2NvdW50O1xuXG4gICAgLy8g8J+Rh+ODkOOCseODg+ODiEFDTOOCouOCr+OCu+OCueaoqVxuICAgIHRoaXMuYWRkVG9SZXNvdXJjZVBvbGljeShuZXcgaWFtLlBvbGljeVN0YXRlbWVudCh7XG4gICAgICBlZmZlY3Q6IGlhbS5FZmZlY3QuQUxMT1csXG4gICAgICBhY3Rpb25zOiBbJ3MzOkdldEJ1Y2tldEFjbCddLFxuICAgICAgcHJpbmNpcGFsczogW1xuICAgICAgICBuZXcgaWFtLlNlcnZpY2VQcmluY2lwYWwoJ2RlbGl2ZXJ5LmxvZ3MuYW1hem9uYXdzLmNvbScpLFxuICAgICAgXSxcbiAgICAgIHJlc291cmNlczogW3RoaXMuYnVja2V0QXJuXSxcbiAgICB9KSk7XG5cbiAgICAvLyDwn5GH44OQ44Kx44OD44OI5pu444GN6L6844G/44Ki44Kv44K744K55qipXG4gICAgdGhpcy5hZGRUb1Jlc291cmNlUG9saWN5KG5ldyBpYW0uUG9saWN5U3RhdGVtZW50KHtcbiAgICAgIGVmZmVjdDogaWFtLkVmZmVjdC5BTExPVyxcbiAgICAgIGFjdGlvbnM6IFsnczM6UHV0T2JqZWN0J10sXG4gICAgICBwcmluY2lwYWxzOiBbXG4gICAgICAgIG5ldyBpYW0uU2VydmljZVByaW5jaXBhbCgnZGVsaXZlcnkubG9ncy5hbWF6b25hd3MuY29tJyksXG4gICAgICBdLFxuICAgICAgLy9yZXNvdXJjZXM6IFtgJHt0aGlzLmJ1Y2tldEFybn0vQVdTTG9ncy8ke2FjY291bnR9LypgXSxcbiAgICAgIHJlc291cmNlczogKCgpID0+IHtcbiAgICAgICAgaWYgKHByb3BzPy5rZXlQcmVmaXhlcyAmJiBwcm9wcy5rZXlQcmVmaXhlcy5sZW5ndGggPiAwKSB7XG4gICAgICAgICAgY29uc3QgcmVzb3VyY2VzOiBBcnJheTxzdHJpbmc+ID0gW107XG4gICAgICAgICAgZm9yIChjb25zdCBrZXlQcmVmaXggb2YgcHJvcHMua2V5UHJlZml4ZXMpIHtcbiAgICAgICAgICAgIHJlc291cmNlcy5wdXNoKGAke3RoaXMuYnVja2V0QXJufS8ke2tleVByZWZpeH0vQVdTTG9ncy8ke2FjY291bnR9LypgKTtcbiAgICAgICAgICB9XG4gICAgICAgICAgcmV0dXJuIHJlc291cmNlcztcbiAgICAgICAgfVxuICAgICAgICByZXR1cm4gW2Ake3RoaXMuYnVja2V0QXJufS9BV1NMb2dzLyR7YWNjb3VudH0vKmBdO1xuICAgICAgfSkoKSxcbiAgICAgIGNvbmRpdGlvbnM6IHtcbiAgICAgICAgU3RyaW5nRXF1YWxzOiB7XG4gICAgICAgICAgJ3MzOngtYW16LWFjbCc6ICdidWNrZXQtb3duZXItZnVsbC1jb250cm9sJyxcbiAgICAgICAgfSxcbiAgICAgIH0sXG4gICAgfSkpO1xuXG4gIH1cbn0iXX0=
```

##### package/package.json

###### Pretty-printed

 * *Similarity: 0.9730861244019139%*

 * *Differences: {"'devDependencies'": "{'projen': '^0.80.19'}", "'version'": "'1.3.4'"}*

```diff
@@ -23,15 +23,15 @@
         "jest": "^29.7.0",
         "jest-junit": "^15",
         "jsii": "5.2.x",
         "jsii-diff": "^1.96.0",
         "jsii-docgen": "^10.3.26",
         "jsii-pacmak": "^1.96.0",
         "jsii-rosetta": "5.2.x",
-        "projen": "^0.80.15",
+        "projen": "^0.80.19",
         "standard-version": "^9",
         "ts-jest": "^29.1.2",
         "ts-node": "^10.9.2",
         "typescript": "5.2.x"
     },
     "engines": {
         "node": ">= 16.0.0"
@@ -152,9 +152,9 @@
         "test:watch": "npx projen test:watch",
         "unbump": "npx projen unbump",
         "upgrade": "npx projen upgrade",
         "watch": "npx projen watch"
     },
     "stability": "stable",
     "types": "lib/index.d.ts",
-    "version": "1.3.3"
+    "version": "1.3.4"
 }
```

### Comparing `gammarer.aws-secure-flow-log-bucket-1.3.3/src/gammarer.aws_secure_flow_log_bucket.egg-info/PKG-INFO` & `gammarer.aws-secure-flow-log-bucket-1.3.4/src/gammarer.aws_secure_flow_log_bucket.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gammarer.aws-secure-flow-log-bucket
-Version: 1.3.3
+Version: 1.3.4
 Summary: Specific AWS VPC FlowLog Bucket
 Home-page: https://github.com/gammarer/aws-secure-flow-log-bucket.git
 Author: yicr<yicr@users.noreply.github.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/gammarer/aws-secure-flow-log-bucket.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `gammarer.aws-secure-flow-log-bucket-1.3.3/src/gammarer.aws_secure_flow_log_bucket.egg-info/SOURCES.txt` & `gammarer.aws-secure-flow-log-bucket-1.3.4/src/gammarer.aws_secure_flow_log_bucket.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/gammarer.aws_secure_flow_log_bucket.egg-info/SOURCES.txt
 src/gammarer.aws_secure_flow_log_bucket.egg-info/dependency_links.txt
 src/gammarer.aws_secure_flow_log_bucket.egg-info/requires.txt
 src/gammarer.aws_secure_flow_log_bucket.egg-info/top_level.txt
 src/gammarer/aws_secure_flow_log_bucket/__init__.py
 src/gammarer/aws_secure_flow_log_bucket/py.typed
 src/gammarer/aws_secure_flow_log_bucket/_jsii/__init__.py
-src/gammarer/aws_secure_flow_log_bucket/_jsii/aws-secure-flow-log-bucket@1.3.3.jsii.tgz
+src/gammarer/aws_secure_flow_log_bucket/_jsii/aws-secure-flow-log-bucket@1.3.4.jsii.tgz
```

