# Comparing `tmp/iam_actions-1.2.20240406.tar.gz` & `tmp/iam_actions-1.2.20240407.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iam_actions-1.2.20240406.tar", max compression
+gzip compressed data, was "iam_actions-1.2.20240407.tar", max compression
```

## Comparing `iam_actions-1.2.20240406.tar` & `iam_actions-1.2.20240407.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1071 2024-04-06 02:13:43.538872 iam_actions-1.2.20240406/LICENSE
--rw-r--r--   0        0        0     2302 2024-04-06 02:13:43.538872 iam_actions-1.2.20240406/README.md
--rw-r--r--   0        0        0      228 2024-04-06 02:13:43.538872 iam_actions-1.2.20240406/iam_actions/__init__.py
--rw-r--r--   0        0        0  4783715 2024-04-06 02:15:56.186891 iam_actions-1.2.20240406/iam_actions/actions.json
--rw-r--r--   0        0        0      496 2024-04-06 02:13:43.538872 iam_actions-1.2.20240406/iam_actions/data.py
--rw-r--r--   0        0        0       80 2024-04-06 02:13:43.538872 iam_actions-1.2.20240406/iam_actions/generate/__init__.py
--rw-r--r--   0        0        0     3097 2024-04-06 02:13:43.538872 iam_actions-1.2.20240406/iam_actions/generate/action_map.py
--rw-r--r--   0        0        0    23329 2024-04-06 02:13:43.538872 iam_actions-1.2.20240406/iam_actions/generate/aws_docs.py
--rw-r--r--   0        0        0     3739 2024-04-06 02:13:43.538872 iam_actions-1.2.20240406/iam_actions/generate/generate.py
--rw-r--r--   0        0        0     3272 2024-04-06 02:13:43.538872 iam_actions-1.2.20240406/iam_actions/generate/notifier.py
--rw-r--r--   0        0        0     1902 2024-04-06 02:13:43.538872 iam_actions-1.2.20240406/iam_actions/generate/resource_type.py
--rw-r--r--   0        0        0     2277 2024-04-06 02:13:43.538872 iam_actions-1.2.20240406/iam_actions/generate/services.py
--rw-r--r--   0        0        0   621709 2024-04-06 02:15:56.186891 iam_actions-1.2.20240406/iam_actions/policies.json
--rw-r--r--   0        0        0   207224 2024-04-06 02:15:56.186891 iam_actions-1.2.20240406/iam_actions/resourcetypes.json
--rw-r--r--   0        0        0   603130 2024-04-06 02:15:56.186891 iam_actions-1.2.20240406/iam_actions/services.json
--rw-r--r--   0        0        0     1154 2024-04-06 02:15:56.834891 iam_actions-1.2.20240406/pyproject.toml
--rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20240406/setup.py
--rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20240406/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-04-07 02:18:42.183692 iam_actions-1.2.20240407/LICENSE
+-rw-r--r--   0        0        0     2302 2024-04-07 02:18:42.183692 iam_actions-1.2.20240407/README.md
+-rw-r--r--   0        0        0      228 2024-04-07 02:18:42.183692 iam_actions-1.2.20240407/iam_actions/__init__.py
+-rw-r--r--   0        0        0  4783715 2024-04-07 02:20:01.055419 iam_actions-1.2.20240407/iam_actions/actions.json
+-rw-r--r--   0        0        0      496 2024-04-07 02:18:42.183692 iam_actions-1.2.20240407/iam_actions/data.py
+-rw-r--r--   0        0        0       80 2024-04-07 02:18:42.183692 iam_actions-1.2.20240407/iam_actions/generate/__init__.py
+-rw-r--r--   0        0        0     3097 2024-04-07 02:18:42.183692 iam_actions-1.2.20240407/iam_actions/generate/action_map.py
+-rw-r--r--   0        0        0    23329 2024-04-07 02:18:42.183692 iam_actions-1.2.20240407/iam_actions/generate/aws_docs.py
+-rw-r--r--   0        0        0     3739 2024-04-07 02:18:42.183692 iam_actions-1.2.20240407/iam_actions/generate/generate.py
+-rw-r--r--   0        0        0     3272 2024-04-07 02:18:42.183692 iam_actions-1.2.20240407/iam_actions/generate/notifier.py
+-rw-r--r--   0        0        0     1902 2024-04-07 02:18:42.183692 iam_actions-1.2.20240407/iam_actions/generate/resource_type.py
+-rw-r--r--   0        0        0     2277 2024-04-07 02:18:42.183692 iam_actions-1.2.20240407/iam_actions/generate/services.py
+-rw-r--r--   0        0        0   621709 2024-04-07 02:20:01.055419 iam_actions-1.2.20240407/iam_actions/policies.json
+-rw-r--r--   0        0        0   207224 2024-04-07 02:20:01.055419 iam_actions-1.2.20240407/iam_actions/resourcetypes.json
+-rw-r--r--   0        0        0   603130 2024-04-07 02:20:01.055419 iam_actions-1.2.20240407/iam_actions/services.json
+-rw-r--r--   0        0        0     1154 2024-04-07 02:20:01.707416 iam_actions-1.2.20240407/pyproject.toml
+-rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20240407/setup.py
+-rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20240407/PKG-INFO
```

### Comparing `iam_actions-1.2.20240406/LICENSE` & `iam_actions-1.2.20240407/LICENSE`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240406/README.md` & `iam_actions-1.2.20240407/README.md`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240406/iam_actions/actions.json` & `iam_actions-1.2.20240407/iam_actions/actions.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Ordering differences only*

```diff
@@ -4442,217 +4442,217 @@
             "resources": [
                 "application",
                 "configurationprofile"
             ]
         }
     },
     "appfabric": {
-        "UpdateIngestionDestination": {
+        "CreateAppAuthorization": {
             "access_level": "Undocumented",
-            "action": "UpdateIngestionDestination",
+            "action": "CreateAppAuthorization",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAppAuthorization": {
+        "ConnectAppAuthorization": {
             "access_level": "Undocumented",
-            "action": "GetAppAuthorization",
+            "action": "ConnectAppAuthorization",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAppBundle": {
+        "StartIngestion": {
             "access_level": "Undocumented",
-            "action": "GetAppBundle",
+            "action": "StartIngestion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "UpdateAppAuthorization": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "UpdateAppAuthorization",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartIngestion": {
+        "ListIngestions": {
             "access_level": "Undocumented",
-            "action": "StartIngestion",
+            "action": "ListIngestions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "BatchGetUserAccessTasks": {
+        "ListAppAuthorizations": {
             "access_level": "Undocumented",
-            "action": "BatchGetUserAccessTasks",
+            "action": "ListAppAuthorizations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetIngestionDestination": {
+        "CreateAppBundle": {
             "access_level": "Undocumented",
-            "action": "GetIngestionDestination",
+            "action": "CreateAppBundle",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ConnectAppAuthorization": {
+        "StopIngestion": {
             "access_level": "Undocumented",
-            "action": "ConnectAppAuthorization",
+            "action": "StopIngestion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateIngestionDestination": {
+        "GetAppAuthorization": {
             "access_level": "Undocumented",
-            "action": "CreateIngestionDestination",
+            "action": "GetAppAuthorization",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteAppBundle": {
+        "DeleteAppAuthorization": {
             "access_level": "Undocumented",
-            "action": "DeleteAppBundle",
+            "action": "DeleteAppAuthorization",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetIngestion": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "GetIngestion",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "GetIngestionDestination": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "GetIngestionDestination",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAppAuthorizations": {
+        "CreateIngestionDestination": {
             "access_level": "Undocumented",
-            "action": "ListAppAuthorizations",
+            "action": "CreateIngestionDestination",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListIngestionDestinations": {
+        "DeleteIngestion": {
             "access_level": "Undocumented",
-            "action": "ListIngestionDestinations",
+            "action": "DeleteIngestion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartUserAccessTasks": {
+        "ListAppBundles": {
             "access_level": "Undocumented",
-            "action": "StartUserAccessTasks",
+            "action": "ListAppBundles",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListIngestions": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "ListIngestions",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StopIngestion": {
+        "CreateIngestion": {
             "access_level": "Undocumented",
-            "action": "StopIngestion",
+            "action": "CreateIngestion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateIngestion": {
+        "BatchGetUserAccessTasks": {
             "access_level": "Undocumented",
-            "action": "CreateIngestion",
+            "action": "BatchGetUserAccessTasks",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAppBundles": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "ListAppBundles",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteAppAuthorization": {
+        "StartUserAccessTasks": {
             "access_level": "Undocumented",
-            "action": "DeleteAppAuthorization",
+            "action": "StartUserAccessTasks",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateAppBundle": {
+        "DeleteIngestionDestination": {
             "access_level": "Undocumented",
-            "action": "CreateAppBundle",
+            "action": "DeleteIngestionDestination",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "DeleteAppBundle": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "DeleteAppBundle",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateAppAuthorization": {
+        "UpdateIngestionDestination": {
             "access_level": "Undocumented",
-            "action": "CreateAppAuthorization",
+            "action": "UpdateIngestionDestination",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateAppAuthorization": {
+        "GetAppBundle": {
             "access_level": "Undocumented",
-            "action": "UpdateAppAuthorization",
+            "action": "GetAppBundle",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteIngestion": {
+        "ListIngestionDestinations": {
             "access_level": "Undocumented",
-            "action": "DeleteIngestion",
+            "action": "ListIngestionDestinations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteIngestionDestination": {
+        "GetIngestion": {
             "access_level": "Undocumented",
-            "action": "DeleteIngestionDestination",
+            "action": "GetIngestion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "appflow": {
@@ -5170,121 +5170,121 @@
             "condition_keys": [],
             "description": "Grants permission to update an existing Application Cost Profiler Report configuration",
             "orphan": false,
             "resources": []
         }
     },
     "application-transformation": {
-        "PutLogData": {
+        "GetPortingCompatibilityAssessment": {
             "access_level": "Undocumented",
-            "action": "PutLogData",
+            "action": "GetPortingCompatibilityAssessment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartGroupingAssessment": {
+        "GetDeployment": {
             "access_level": "Undocumented",
-            "action": "StartGroupingAssessment",
+            "action": "GetDeployment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartContainerization": {
+        "GetGroupingAssessment": {
             "access_level": "Undocumented",
-            "action": "StartContainerization",
+            "action": "GetGroupingAssessment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutMetricData": {
+        "StartContainerization": {
             "access_level": "Undocumented",
-            "action": "PutMetricData",
+            "action": "StartContainerization",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartPortingCompatibilityAssessment": {
+        "StartRuntimeAssessment": {
             "access_level": "Undocumented",
-            "action": "StartPortingCompatibilityAssessment",
+            "action": "StartRuntimeAssessment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartRuntimeAssessment": {
+        "StartDeployment": {
             "access_level": "Undocumented",
-            "action": "StartRuntimeAssessment",
+            "action": "StartDeployment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetGroupingAssessment": {
+        "GetContainerization": {
             "access_level": "Undocumented",
-            "action": "GetGroupingAssessment",
+            "action": "GetContainerization",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetRuntimeAssessment": {
+        "PutMetricData": {
             "access_level": "Undocumented",
-            "action": "GetRuntimeAssessment",
+            "action": "PutMetricData",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartDeployment": {
+        "StartPortingRecommendationAssessment": {
             "access_level": "Undocumented",
-            "action": "StartDeployment",
+            "action": "StartPortingRecommendationAssessment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartPortingRecommendationAssessment": {
+        "StartPortingCompatibilityAssessment": {
             "access_level": "Undocumented",
-            "action": "StartPortingRecommendationAssessment",
+            "action": "StartPortingCompatibilityAssessment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPortingRecommendationAssessment": {
+        "StartGroupingAssessment": {
             "access_level": "Undocumented",
-            "action": "GetPortingRecommendationAssessment",
+            "action": "StartGroupingAssessment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPortingCompatibilityAssessment": {
+        "PutLogData": {
             "access_level": "Undocumented",
-            "action": "GetPortingCompatibilityAssessment",
+            "action": "PutLogData",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetDeployment": {
+        "GetRuntimeAssessment": {
             "access_level": "Undocumented",
-            "action": "GetDeployment",
+            "action": "GetRuntimeAssessment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetContainerization": {
+        "GetPortingRecommendationAssessment": {
             "access_level": "Undocumented",
-            "action": "GetContainerization",
+            "action": "GetPortingRecommendationAssessment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "applicationinsights": {
@@ -11937,225 +11937,225 @@
             "condition_keys": [],
             "description": "Validates Server Migration Connector Id that was registered with AWS Connector Service.",
             "orphan": false,
             "resources": []
         }
     },
     "b2bi": {
-        "DeleteTransformer": {
+        "DeleteCapability": {
             "access_level": "Undocumented",
-            "action": "DeleteTransformer",
+            "action": "DeleteCapability",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateCapability": {
+        "GetTransformerJob": {
             "access_level": "Undocumented",
-            "action": "CreateCapability",
+            "action": "GetTransformerJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdatePartnership": {
+        "DeletePartnership": {
             "access_level": "Undocumented",
-            "action": "UpdatePartnership",
+            "action": "DeletePartnership",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPartnerships": {
+        "ListCapabilities": {
             "access_level": "Undocumented",
-            "action": "ListPartnerships",
+            "action": "ListCapabilities",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "ListTransformers": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "ListTransformers",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateTransformer": {
+        "CreateProfile": {
             "access_level": "Undocumented",
-            "action": "UpdateTransformer",
+            "action": "CreateProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeletePartnership": {
+        "UpdateTransformer": {
             "access_level": "Undocumented",
-            "action": "DeletePartnership",
+            "action": "UpdateTransformer",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetProfile": {
+        "DeleteProfile": {
             "access_level": "Undocumented",
-            "action": "GetProfile",
+            "action": "DeleteProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateProfile": {
+        "TestMapping": {
             "access_level": "Undocumented",
-            "action": "UpdateProfile",
+            "action": "TestMapping",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "GetPartnership": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "GetPartnership",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TestParsing": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "TestParsing",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPartnership": {
+        "GetCapability": {
             "access_level": "Undocumented",
-            "action": "GetPartnership",
+            "action": "GetCapability",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTransformers": {
+        "ListPartnerships": {
             "access_level": "Undocumented",
-            "action": "ListTransformers",
+            "action": "ListPartnerships",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetCapability": {
+        "GetProfile": {
             "access_level": "Undocumented",
-            "action": "GetCapability",
+            "action": "GetProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TestMapping": {
+        "CreateCapability": {
             "access_level": "Undocumented",
-            "action": "TestMapping",
+            "action": "CreateCapability",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateCapability": {
+        "UpdatePartnership": {
             "access_level": "Undocumented",
-            "action": "UpdateCapability",
+            "action": "UpdatePartnership",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "CreateTransformer": {
             "access_level": "Undocumented",
             "action": "CreateTransformer",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "CreatePartnership": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "CreatePartnership",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateProfile": {
+        "StartTransformerJob": {
             "access_level": "Undocumented",
-            "action": "CreateProfile",
+            "action": "StartTransformerJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreatePartnership": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "CreatePartnership",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListCapabilities": {
+        "UpdateProfile": {
             "access_level": "Undocumented",
-            "action": "ListCapabilities",
+            "action": "UpdateProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteCapability": {
+        "GetTransformer": {
             "access_level": "Undocumented",
-            "action": "DeleteCapability",
+            "action": "GetTransformer",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetTransformer": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "GetTransformer",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartTransformerJob": {
+        "DeleteTransformer": {
             "access_level": "Undocumented",
-            "action": "StartTransformerJob",
+            "action": "DeleteTransformer",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "ListProfiles": {
             "access_level": "Undocumented",
             "action": "ListProfiles",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteProfile": {
+        "TestParsing": {
             "access_level": "Undocumented",
-            "action": "DeleteProfile",
+            "action": "TestParsing",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetTransformerJob": {
+        "UpdateCapability": {
             "access_level": "Undocumented",
-            "action": "GetTransformerJob",
+            "action": "UpdateCapability",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "backup": {
@@ -13789,885 +13789,885 @@
             "orphan": false,
             "resources": [
                 "scheduling-policy"
             ]
         }
     },
     "bcm-data-exports": {
-        "UpdateExport": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "UpdateExport",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetExport": {
+        "CreateExport": {
             "access_level": "Undocumented",
-            "action": "GetExport",
+            "action": "CreateExport",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "ListTables": {
             "access_level": "Undocumented",
             "action": "ListTables",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "GetTable": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "GetTable",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "UpdateExport": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "UpdateExport",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteExport": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "DeleteExport",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetTable": {
+        "ListExecutions": {
             "access_level": "Undocumented",
-            "action": "GetTable",
+            "action": "ListExecutions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetExecution": {
+        "ListExports": {
             "access_level": "Undocumented",
-            "action": "GetExecution",
+            "action": "ListExports",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "DeleteExport": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "DeleteExport",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateExport": {
+        "GetExecution": {
             "access_level": "Undocumented",
-            "action": "CreateExport",
+            "action": "GetExecution",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListExecutions": {
+        "GetExport": {
             "access_level": "Undocumented",
-            "action": "ListExecutions",
+            "action": "GetExport",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListExports": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "ListExports",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "bedrock": {
-        "ListIngestionJobs": {
+        "CreateKnowledgeBase": {
             "access_level": "Undocumented",
-            "action": "ListIngestionJobs",
+            "action": "CreateKnowledgeBase",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateKnowledgeBase": {
+        "GetCustomModel": {
             "access_level": "Undocumented",
-            "action": "CreateKnowledgeBase",
+            "action": "GetCustomModel",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetDataSource": {
+        "InvokeModel": {
             "access_level": "Undocumented",
-            "action": "GetDataSource",
+            "action": "InvokeModel",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListFoundationModelAgreementOffers": {
+        "DetectGeneratedContent": {
             "access_level": "Undocumented",
-            "action": "ListFoundationModelAgreementOffers",
+            "action": "DetectGeneratedContent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RetrieveAndGenerate": {
+        "GetAgentAlias": {
             "access_level": "Undocumented",
-            "action": "RetrieveAndGenerate",
+            "action": "GetAgentAlias",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateDataSource": {
+        "ListFoundationModelAgreementOffers": {
             "access_level": "Undocumented",
-            "action": "CreateDataSource",
+            "action": "ListFoundationModelAgreementOffers",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateAgentActionGroup": {
+        "StopModelCustomizationJob": {
             "access_level": "Undocumented",
-            "action": "UpdateAgentActionGroup",
+            "action": "StopModelCustomizationJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAgentVersions": {
+        "CreateAgentAlias": {
             "access_level": "Undocumented",
-            "action": "ListAgentVersions",
+            "action": "CreateAgentAlias",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetModelEvaluationJob": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "GetModelEvaluationJob",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAgentAliases": {
+        "GetAgentVersion": {
             "access_level": "Undocumented",
-            "action": "ListAgentAliases",
+            "action": "GetAgentVersion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "GetAgent": {
             "access_level": "Undocumented",
             "action": "GetAgent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListCustomModels": {
+        "ListGuardrails": {
             "access_level": "Undocumented",
-            "action": "ListCustomModels",
+            "action": "ListGuardrails",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetFoundationModel": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "GetFoundationModel",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteFoundationModelAgreement": {
+        "AssociateThirdPartyKnowledgeBase": {
             "access_level": "Undocumented",
-            "action": "DeleteFoundationModelAgreement",
+            "action": "AssociateThirdPartyKnowledgeBase",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateAgentAlias": {
+        "DeleteKnowledgeBase": {
             "access_level": "Undocumented",
-            "action": "UpdateAgentAlias",
+            "action": "DeleteKnowledgeBase",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListModelInvocationJobs": {
+        "CreateModelEvaluationJob": {
             "access_level": "Undocumented",
-            "action": "ListModelInvocationJobs",
+            "action": "CreateModelEvaluationJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartIngestionJob": {
+        "DeleteProvisionedModelThroughput": {
             "access_level": "Undocumented",
-            "action": "StartIngestionJob",
+            "action": "DeleteProvisionedModelThroughput",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateGuardrailVersion": {
+        "ListProvisionedModelThroughputs": {
             "access_level": "Undocumented",
-            "action": "CreateGuardrailVersion",
+            "action": "ListProvisionedModelThroughputs",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateProvisionedModelThroughput": {
+        "DeleteFoundationModelAgreement": {
             "access_level": "Undocumented",
-            "action": "UpdateProvisionedModelThroughput",
+            "action": "DeleteFoundationModelAgreement",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateProvisionedModelThroughput": {
+        "ListAgentAliases": {
             "access_level": "Undocumented",
-            "action": "CreateProvisionedModelThroughput",
+            "action": "ListAgentAliases",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateModelInvocationJob": {
+        "CreateProvisionedModelThroughput": {
             "access_level": "Undocumented",
-            "action": "CreateModelInvocationJob",
+            "action": "CreateProvisionedModelThroughput",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetGuardrail": {
+        "UpdateAgent": {
             "access_level": "Undocumented",
-            "action": "GetGuardrail",
+            "action": "UpdateAgent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "InvokeModel": {
+        "GetGuardrail": {
             "access_level": "Undocumented",
-            "action": "InvokeModel",
+            "action": "GetGuardrail",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteProvisionedModelThroughput": {
+        "PutFoundationModelEntitlement": {
             "access_level": "Undocumented",
-            "action": "DeleteProvisionedModelThroughput",
+            "action": "PutFoundationModelEntitlement",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateFoundationModelAgreement": {
+        "DeleteAgentAlias": {
             "access_level": "Undocumented",
-            "action": "CreateFoundationModelAgreement",
+            "action": "DeleteAgentAlias",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAgentVersion": {
+        "GetIngestionJob": {
             "access_level": "Undocumented",
-            "action": "GetAgentVersion",
+            "action": "GetIngestionJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListProvisionedModelThroughputs": {
+        "GetModelEvaluationJob": {
             "access_level": "Undocumented",
-            "action": "ListProvisionedModelThroughputs",
+            "action": "GetModelEvaluationJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteAgent": {
+        "DeleteModelInvocationLoggingConfiguration": {
             "access_level": "Undocumented",
-            "action": "DeleteAgent",
+            "action": "DeleteModelInvocationLoggingConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetKnowledgeBase": {
+        "PrepareAgent": {
             "access_level": "Undocumented",
-            "action": "GetKnowledgeBase",
+            "action": "PrepareAgent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "GetAgentKnowledgeBase": {
             "access_level": "Undocumented",
             "action": "GetAgentKnowledgeBase",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteAgentAlias": {
+        "StartIngestionJob": {
             "access_level": "Undocumented",
-            "action": "DeleteAgentAlias",
+            "action": "StartIngestionJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutModelInvocationLoggingConfiguration": {
+        "ListAgentActionGroups": {
             "access_level": "Undocumented",
-            "action": "PutModelInvocationLoggingConfiguration",
+            "action": "ListAgentActionGroups",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateAgentAlias": {
+        "CreateFoundationModelAgreement": {
             "access_level": "Undocumented",
-            "action": "CreateAgentAlias",
+            "action": "CreateFoundationModelAgreement",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetIngestionJob": {
+        "StopModelInvocationJob": {
             "access_level": "Undocumented",
-            "action": "GetIngestionJob",
+            "action": "StopModelInvocationJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateModelCustomizationJob": {
+        "InvokeAgent": {
             "access_level": "Undocumented",
-            "action": "CreateModelCustomizationJob",
+            "action": "InvokeAgent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteDataSource": {
+        "CreateAgent": {
             "access_level": "Undocumented",
-            "action": "DeleteDataSource",
+            "action": "CreateAgent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StopModelCustomizationJob": {
+        "DeleteGuardrail": {
             "access_level": "Undocumented",
-            "action": "StopModelCustomizationJob",
+            "action": "DeleteGuardrail",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DetectGeneratedContent": {
+        "UpdateProvisionedModelThroughput": {
             "access_level": "Undocumented",
-            "action": "DetectGeneratedContent",
+            "action": "UpdateProvisionedModelThroughput",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateModelEvaluationJob": {
+        "GetProvisionedModelThroughput": {
             "access_level": "Undocumented",
-            "action": "CreateModelEvaluationJob",
+            "action": "GetProvisionedModelThroughput",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteGuardrail": {
+        "CreateModelInvocationJob": {
             "access_level": "Undocumented",
-            "action": "DeleteGuardrail",
+            "action": "CreateModelInvocationJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateAgentActionGroup": {
+        "ListCustomModels": {
             "access_level": "Undocumented",
-            "action": "CreateAgentActionGroup",
+            "action": "ListCustomModels",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAgentActionGroups": {
+        "UpdateDataSource": {
             "access_level": "Undocumented",
-            "action": "ListAgentActionGroups",
+            "action": "UpdateDataSource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListKnowledgeBases": {
+        "ListIngestionJobs": {
             "access_level": "Undocumented",
-            "action": "ListKnowledgeBases",
+            "action": "ListIngestionJobs",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAgentAlias": {
+        "DeleteAgentActionGroup": {
             "access_level": "Undocumented",
-            "action": "GetAgentAlias",
+            "action": "DeleteAgentActionGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateAgent": {
+        "PutUseCaseForModelAccess": {
             "access_level": "Undocumented",
-            "action": "CreateAgent",
+            "action": "PutUseCaseForModelAccess",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetModelInvocationJob": {
+        "DisassociateAgentKnowledgeBase": {
             "access_level": "Undocumented",
-            "action": "GetModelInvocationJob",
+            "action": "DisassociateAgentKnowledgeBase",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateGuardrail": {
+        "UpdateAgentAlias": {
             "access_level": "Undocumented",
-            "action": "CreateGuardrail",
+            "action": "UpdateAgentAlias",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetModelInvocationLoggingConfiguration": {
+        "UpdateGuardrail": {
             "access_level": "Undocumented",
-            "action": "GetModelInvocationLoggingConfiguration",
+            "action": "UpdateGuardrail",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetModelCustomizationJob": {
+        "ListAgentVersions": {
             "access_level": "Undocumented",
-            "action": "GetModelCustomizationJob",
+            "action": "ListAgentVersions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "InvokeAgent": {
+        "CreateDataSource": {
             "access_level": "Undocumented",
-            "action": "InvokeAgent",
+            "action": "CreateDataSource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAgentKnowledgeBases": {
+        "UpdateAgentKnowledgeBase": {
             "access_level": "Undocumented",
-            "action": "ListAgentKnowledgeBases",
+            "action": "UpdateAgentKnowledgeBase",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListGuardrails": {
+        "ListAgentKnowledgeBases": {
             "access_level": "Undocumented",
-            "action": "ListGuardrails",
+            "action": "ListAgentKnowledgeBases",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PrepareAgent": {
+        "CreateGuardrailVersion": {
             "access_level": "Undocumented",
-            "action": "PrepareAgent",
+            "action": "CreateGuardrailVersion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateAgent": {
+        "UpdateKnowledgeBase": {
             "access_level": "Undocumented",
-            "action": "UpdateAgent",
+            "action": "UpdateKnowledgeBase",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "InvokeModelWithResponseStream": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "InvokeModelWithResponseStream",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "ListModelEvaluationJobs": {
             "access_level": "Undocumented",
             "action": "ListModelEvaluationJobs",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DisassociateAgentKnowledgeBase": {
+        "UpdateAgentActionGroup": {
             "access_level": "Undocumented",
-            "action": "DisassociateAgentKnowledgeBase",
+            "action": "UpdateAgentActionGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateAgentKnowledgeBase": {
+        "CreateModelCustomizationJob": {
             "access_level": "Undocumented",
-            "action": "UpdateAgentKnowledgeBase",
+            "action": "CreateModelCustomizationJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListFoundationModels": {
+        "DeleteAgentVersion": {
             "access_level": "Undocumented",
-            "action": "ListFoundationModels",
+            "action": "DeleteAgentVersion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateDataSource": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "UpdateDataSource",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssociateAgentKnowledgeBase": {
+        "ListDataSources": {
             "access_level": "Undocumented",
-            "action": "AssociateAgentKnowledgeBase",
+            "action": "ListDataSources",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutFoundationModelEntitlement": {
+        "GetAgentActionGroup": {
             "access_level": "Undocumented",
-            "action": "PutFoundationModelEntitlement",
+            "action": "GetAgentActionGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "Retrieve": {
+        "CreateAgentActionGroup": {
             "access_level": "Undocumented",
-            "action": "Retrieve",
+            "action": "CreateAgentActionGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StopModelInvocationJob": {
+        "GetFoundationModel": {
             "access_level": "Undocumented",
-            "action": "StopModelInvocationJob",
+            "action": "GetFoundationModel",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteKnowledgeBase": {
+        "GetUseCaseForModelAccess": {
             "access_level": "Undocumented",
-            "action": "DeleteKnowledgeBase",
+            "action": "GetUseCaseForModelAccess",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "ListModelInvocationJobs": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "ListModelInvocationJobs",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListModelCustomizationJobs": {
+        "GetDataSource": {
             "access_level": "Undocumented",
-            "action": "ListModelCustomizationJobs",
+            "action": "GetDataSource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAgentActionGroup": {
+        "RetrieveAndGenerate": {
             "access_level": "Undocumented",
-            "action": "GetAgentActionGroup",
+            "action": "RetrieveAndGenerate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListDataSources": {
+        "DeleteAgent": {
             "access_level": "Undocumented",
-            "action": "ListDataSources",
+            "action": "DeleteAgent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateGuardrail": {
+        "DeleteDataSource": {
             "access_level": "Undocumented",
-            "action": "UpdateGuardrail",
+            "action": "DeleteDataSource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "InvokeModelWithResponseStream": {
+        "GetModelInvocationJob": {
             "access_level": "Undocumented",
-            "action": "InvokeModelWithResponseStream",
+            "action": "GetModelInvocationJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteCustomModel": {
+        "AssociateAgentKnowledgeBase": {
             "access_level": "Undocumented",
-            "action": "DeleteCustomModel",
+            "action": "AssociateAgentKnowledgeBase",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetUseCaseForModelAccess": {
+        "DeleteCustomModel": {
             "access_level": "Undocumented",
-            "action": "GetUseCaseForModelAccess",
+            "action": "DeleteCustomModel",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetProvisionedModelThroughput": {
+        "GetFoundationModelAvailability": {
             "access_level": "Undocumented",
-            "action": "GetProvisionedModelThroughput",
+            "action": "GetFoundationModelAvailability",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAgents": {
+        "GetModelInvocationLoggingConfiguration": {
             "access_level": "Undocumented",
-            "action": "ListAgents",
+            "action": "GetModelInvocationLoggingConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "ListAgents": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "ListAgents",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssociateThirdPartyKnowledgeBase": {
+        "ListFoundationModels": {
             "access_level": "Undocumented",
-            "action": "AssociateThirdPartyKnowledgeBase",
+            "action": "ListFoundationModels",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetCustomModel": {
+        "Retrieve": {
             "access_level": "Undocumented",
-            "action": "GetCustomModel",
+            "action": "Retrieve",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteModelInvocationLoggingConfiguration": {
+        "PutModelInvocationLoggingConfiguration": {
             "access_level": "Undocumented",
-            "action": "DeleteModelInvocationLoggingConfiguration",
+            "action": "PutModelInvocationLoggingConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateKnowledgeBase": {
+        "CreateGuardrail": {
             "access_level": "Undocumented",
-            "action": "UpdateKnowledgeBase",
+            "action": "CreateGuardrail",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteAgentVersion": {
+        "GetKnowledgeBase": {
             "access_level": "Undocumented",
-            "action": "DeleteAgentVersion",
+            "action": "GetKnowledgeBase",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteAgentActionGroup": {
+        "GetModelCustomizationJob": {
             "access_level": "Undocumented",
-            "action": "DeleteAgentActionGroup",
+            "action": "GetModelCustomizationJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutUseCaseForModelAccess": {
+        "ListModelCustomizationJobs": {
             "access_level": "Undocumented",
-            "action": "PutUseCaseForModelAccess",
+            "action": "ListModelCustomizationJobs",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetFoundationModelAvailability": {
+        "ListKnowledgeBases": {
             "access_level": "Undocumented",
-            "action": "GetFoundationModelAvailability",
+            "action": "ListKnowledgeBases",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "billing": {
-        "GetBillingPreferences": {
+        "GetBillingDetails": {
             "access_level": "Undocumented",
-            "action": "GetBillingPreferences",
+            "action": "GetBillingDetails",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetCredits": {
+        "GetBillingPreferences": {
             "access_level": "Undocumented",
-            "action": "GetCredits",
+            "action": "GetBillingPreferences",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSellerOfRecord": {
+        "GetBillingData": {
             "access_level": "Undocumented",
-            "action": "GetSellerOfRecord",
+            "action": "GetBillingData",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListBillingViews": {
+        "PutContractInformation": {
             "access_level": "Undocumented",
-            "action": "ListBillingViews",
+            "action": "PutContractInformation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "UpdateBillingPreferences": {
             "access_level": "Undocumented",
             "action": "UpdateBillingPreferences",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetBillingData": {
+        "GetCredits": {
             "access_level": "Undocumented",
-            "action": "GetBillingData",
+            "action": "GetCredits",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetIAMAccessPreference": {
+        "UpdateIAMAccessPreference": {
             "access_level": "Undocumented",
-            "action": "GetIAMAccessPreference",
+            "action": "UpdateIAMAccessPreference",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RedeemCredits": {
+        "GetBillingNotifications": {
             "access_level": "Undocumented",
-            "action": "RedeemCredits",
+            "action": "GetBillingNotifications",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetContractInformation": {
+        "GetIAMAccessPreference": {
             "access_level": "Undocumented",
-            "action": "GetContractInformation",
+            "action": "GetIAMAccessPreference",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetBillingDetails": {
+        "GetContractInformation": {
             "access_level": "Undocumented",
-            "action": "GetBillingDetails",
+            "action": "GetContractInformation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetBillingNotifications": {
+        "GetSellerOfRecord": {
             "access_level": "Undocumented",
-            "action": "GetBillingNotifications",
+            "action": "GetSellerOfRecord",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateIAMAccessPreference": {
+        "ListBillingViews": {
             "access_level": "Undocumented",
-            "action": "UpdateIAMAccessPreference",
+            "action": "ListBillingViews",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutContractInformation": {
+        "RedeemCredits": {
             "access_level": "Undocumented",
-            "action": "PutContractInformation",
+            "action": "RedeemCredits",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "billingconductor": {
@@ -19752,715 +19752,715 @@
             "condition_keys": [],
             "description": "Grants permission to validate an address to be used for 911 calls made with Amazon Chime Voice Connectors",
             "orphan": false,
             "resources": []
         }
     },
     "cleanrooms": {
-        "CreateConfiguredTable": {
+        "CreateConfiguredTableAssociation": {
             "access_level": "Undocumented",
-            "action": "CreateConfiguredTable",
+            "action": "CreateConfiguredTableAssociation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteAnalysisTemplate": {
+        "DeleteConfiguredTable": {
             "access_level": "Undocumented",
-            "action": "DeleteAnalysisTemplate",
+            "action": "DeleteConfiguredTable",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetCollaborationAnalysisTemplate": {
+        "GetCollaborationPrivacyBudgetTemplate": {
             "access_level": "Undocumented",
-            "action": "GetCollaborationAnalysisTemplate",
+            "action": "GetCollaborationPrivacyBudgetTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetConfiguredTableAssociation": {
+        "CreateConfiguredAudienceModelAssociation": {
             "access_level": "Undocumented",
-            "action": "GetConfiguredTableAssociation",
+            "action": "CreateConfiguredAudienceModelAssociation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteMember": {
+        "DeleteMembership": {
             "access_level": "Undocumented",
-            "action": "DeleteMember",
+            "action": "DeleteMembership",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdatePrivacyBudgetTemplate": {
+        "CreateMembership": {
             "access_level": "Undocumented",
-            "action": "UpdatePrivacyBudgetTemplate",
+            "action": "CreateMembership",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAnalysisTemplates": {
+        "UpdatePrivacyBudgetTemplate": {
             "access_level": "Undocumented",
-            "action": "ListAnalysisTemplates",
+            "action": "UpdatePrivacyBudgetTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateAnalysisTemplate": {
+        "ListCollaborationAnalysisTemplates": {
             "access_level": "Undocumented",
-            "action": "UpdateAnalysisTemplate",
+            "action": "ListCollaborationAnalysisTemplates",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPrivacyBudgetTemplate": {
+        "CreateAnalysisTemplate": {
             "access_level": "Undocumented",
-            "action": "GetPrivacyBudgetTemplate",
+            "action": "CreateAnalysisTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetProtectedQuery": {
+        "GetCollaborationConfiguredAudienceModelAssociation": {
             "access_level": "Undocumented",
-            "action": "GetProtectedQuery",
+            "action": "GetCollaborationConfiguredAudienceModelAssociation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "UpdateCollaboration": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "UpdateCollaboration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListProtectedQueries": {
+        "UpdateConfiguredTableAssociation": {
             "access_level": "Undocumented",
-            "action": "ListProtectedQueries",
+            "action": "UpdateConfiguredTableAssociation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateConfiguredAudienceModelAssociation": {
+        "BatchGetSchema": {
             "access_level": "Undocumented",
-            "action": "UpdateConfiguredAudienceModelAssociation",
+            "action": "BatchGetSchema",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetConfiguredAudienceModelAssociation": {
+        "UpdateAnalysisTemplate": {
             "access_level": "Undocumented",
-            "action": "GetConfiguredAudienceModelAssociation",
+            "action": "UpdateAnalysisTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateMembership": {
+        "ListConfiguredAudienceModelAssociations": {
             "access_level": "Undocumented",
-            "action": "UpdateMembership",
+            "action": "ListConfiguredAudienceModelAssociations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListConfiguredTableAssociations": {
+        "ListMemberships": {
             "access_level": "Undocumented",
-            "action": "ListConfiguredTableAssociations",
+            "action": "ListMemberships",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPrivacyBudgetTemplates": {
+        "GetMembership": {
             "access_level": "Undocumented",
-            "action": "ListPrivacyBudgetTemplates",
+            "action": "GetMembership",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateMembership": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "CreateMembership",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAnalysisTemplate": {
+        "StartProtectedQuery": {
             "access_level": "Undocumented",
-            "action": "GetAnalysisTemplate",
+            "action": "StartProtectedQuery",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteConfiguredTable": {
+        "ListPrivacyBudgets": {
             "access_level": "Undocumented",
-            "action": "DeleteConfiguredTable",
+            "action": "ListPrivacyBudgets",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateConfiguredTable": {
+        "ListConfiguredTables": {
             "access_level": "Undocumented",
-            "action": "UpdateConfiguredTable",
+            "action": "ListConfiguredTables",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteConfiguredTableAssociation": {
+        "CreatePrivacyBudgetTemplate": {
             "access_level": "Undocumented",
-            "action": "DeleteConfiguredTableAssociation",
+            "action": "CreatePrivacyBudgetTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListMemberships": {
+        "ListAnalysisTemplates": {
             "access_level": "Undocumented",
-            "action": "ListMemberships",
+            "action": "ListAnalysisTemplates",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetConfiguredTableAnalysisRule": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "GetConfiguredTableAnalysisRule",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateConfiguredTableAnalysisRule": {
+        "BatchGetSchemaAnalysisRule": {
             "access_level": "Undocumented",
-            "action": "CreateConfiguredTableAnalysisRule",
+            "action": "BatchGetSchemaAnalysisRule",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteConfiguredTableAnalysisRule": {
+        "GetPrivacyBudgetTemplate": {
             "access_level": "Undocumented",
-            "action": "DeleteConfiguredTableAnalysisRule",
+            "action": "GetPrivacyBudgetTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetCollaborationPrivacyBudgetTemplate": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "GetCollaborationPrivacyBudgetTemplate",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListCollaborations": {
+        "ListSchemas": {
             "access_level": "Undocumented",
-            "action": "ListCollaborations",
+            "action": "ListSchemas",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartProtectedQuery": {
+        "GetAnalysisTemplate": {
             "access_level": "Undocumented",
-            "action": "StartProtectedQuery",
+            "action": "GetAnalysisTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSchema": {
+        "ListCollaborationConfiguredAudienceModelAssociations": {
             "access_level": "Undocumented",
-            "action": "GetSchema",
+            "action": "ListCollaborationConfiguredAudienceModelAssociations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListCollaborationPrivacyBudgetTemplates": {
+        "UpdateConfiguredTable": {
             "access_level": "Undocumented",
-            "action": "ListCollaborationPrivacyBudgetTemplates",
+            "action": "UpdateConfiguredTable",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "BatchGetSchemaAnalysisRule": {
+        "UpdateMembership": {
             "access_level": "Undocumented",
-            "action": "BatchGetSchemaAnalysisRule",
+            "action": "UpdateMembership",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSchemaAnalysisRule": {
+        "GetCollaboration": {
             "access_level": "Undocumented",
-            "action": "GetSchemaAnalysisRule",
+            "action": "GetCollaboration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetCollaboration": {
+        "DeleteCollaboration": {
             "access_level": "Undocumented",
-            "action": "GetCollaboration",
+            "action": "DeleteCollaboration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPrivacyBudgets": {
+        "GetCollaborationAnalysisTemplate": {
             "access_level": "Undocumented",
-            "action": "ListPrivacyBudgets",
+            "action": "GetCollaborationAnalysisTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PreviewPrivacyImpact": {
+        "DeleteConfiguredTableAnalysisRule": {
             "access_level": "Undocumented",
-            "action": "PreviewPrivacyImpact",
+            "action": "DeleteConfiguredTableAnalysisRule",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreatePrivacyBudgetTemplate": {
+        "GetConfiguredTableAssociation": {
             "access_level": "Undocumented",
-            "action": "CreatePrivacyBudgetTemplate",
+            "action": "GetConfiguredTableAssociation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteCollaboration": {
+        "ListProtectedQueries": {
             "access_level": "Undocumented",
-            "action": "DeleteCollaboration",
+            "action": "ListProtectedQueries",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "BatchGetSchema": {
+        "GetProtectedQuery": {
             "access_level": "Undocumented",
-            "action": "BatchGetSchema",
+            "action": "GetProtectedQuery",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteConfiguredAudienceModelAssociation": {
+        "CreateCollaboration": {
             "access_level": "Undocumented",
-            "action": "DeleteConfiguredAudienceModelAssociation",
+            "action": "CreateCollaboration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListCollaborationConfiguredAudienceModelAssociations": {
+        "GetConfiguredTableAnalysisRule": {
             "access_level": "Undocumented",
-            "action": "ListCollaborationConfiguredAudienceModelAssociations",
+            "action": "GetConfiguredTableAnalysisRule",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListConfiguredAudienceModelAssociations": {
+        "DeleteConfiguredTableAssociation": {
             "access_level": "Undocumented",
-            "action": "ListConfiguredAudienceModelAssociations",
+            "action": "DeleteConfiguredTableAssociation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "PreviewPrivacyImpact": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "PreviewPrivacyImpact",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateAnalysisTemplate": {
+        "ListConfiguredTableAssociations": {
             "access_level": "Undocumented",
-            "action": "CreateAnalysisTemplate",
+            "action": "ListConfiguredTableAssociations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListMembers": {
+        "UpdateConfiguredAudienceModelAssociation": {
             "access_level": "Undocumented",
-            "action": "ListMembers",
+            "action": "UpdateConfiguredAudienceModelAssociation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateConfiguredTableAssociation": {
+        "BatchGetCollaborationAnalysisTemplate": {
             "access_level": "Undocumented",
-            "action": "UpdateConfiguredTableAssociation",
+            "action": "BatchGetCollaborationAnalysisTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteMembership": {
+        "GetConfiguredAudienceModelAssociation": {
             "access_level": "Undocumented",
-            "action": "DeleteMembership",
+            "action": "GetConfiguredAudienceModelAssociation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateConfiguredAudienceModelAssociation": {
+        "GetConfiguredTable": {
             "access_level": "Undocumented",
-            "action": "CreateConfiguredAudienceModelAssociation",
+            "action": "GetConfiguredTable",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeletePrivacyBudgetTemplate": {
+        "GetSchema": {
             "access_level": "Undocumented",
-            "action": "DeletePrivacyBudgetTemplate",
+            "action": "GetSchema",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetMembership": {
+        "DeleteAnalysisTemplate": {
             "access_level": "Undocumented",
-            "action": "GetMembership",
+            "action": "DeleteAnalysisTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateConfiguredTableAnalysisRule": {
+        "ListCollaborationPrivacyBudgets": {
             "access_level": "Undocumented",
-            "action": "UpdateConfiguredTableAnalysisRule",
+            "action": "ListCollaborationPrivacyBudgets",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateProtectedQuery": {
+        "DeleteMember": {
             "access_level": "Undocumented",
-            "action": "UpdateProtectedQuery",
+            "action": "DeleteMember",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "BatchGetCollaborationAnalysisTemplate": {
+        "CreateConfiguredTable": {
             "access_level": "Undocumented",
-            "action": "BatchGetCollaborationAnalysisTemplate",
+            "action": "CreateConfiguredTable",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListCollaborationPrivacyBudgets": {
+        "ListPrivacyBudgetTemplates": {
             "access_level": "Undocumented",
-            "action": "ListCollaborationPrivacyBudgets",
+            "action": "ListPrivacyBudgetTemplates",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSchemas": {
+        "UpdateConfiguredTableAnalysisRule": {
             "access_level": "Undocumented",
-            "action": "ListSchemas",
+            "action": "UpdateConfiguredTableAnalysisRule",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateCollaboration": {
+        "GetSchemaAnalysisRule": {
             "access_level": "Undocumented",
-            "action": "CreateCollaboration",
+            "action": "GetSchemaAnalysisRule",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetCollaborationConfiguredAudienceModelAssociation": {
+        "ListMembers": {
             "access_level": "Undocumented",
-            "action": "GetCollaborationConfiguredAudienceModelAssociation",
+            "action": "ListMembers",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetConfiguredTable": {
+        "UpdateProtectedQuery": {
             "access_level": "Undocumented",
-            "action": "GetConfiguredTable",
+            "action": "UpdateProtectedQuery",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListCollaborationAnalysisTemplates": {
+        "ListCollaborationPrivacyBudgetTemplates": {
             "access_level": "Undocumented",
-            "action": "ListCollaborationAnalysisTemplates",
+            "action": "ListCollaborationPrivacyBudgetTemplates",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListConfiguredTables": {
+        "DeleteConfiguredAudienceModelAssociation": {
             "access_level": "Undocumented",
-            "action": "ListConfiguredTables",
+            "action": "DeleteConfiguredAudienceModelAssociation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "CreateConfiguredTableAnalysisRule": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "CreateConfiguredTableAnalysisRule",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateCollaboration": {
+        "ListCollaborations": {
             "access_level": "Undocumented",
-            "action": "UpdateCollaboration",
+            "action": "ListCollaborations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateConfiguredTableAssociation": {
+        "DeletePrivacyBudgetTemplate": {
             "access_level": "Undocumented",
-            "action": "CreateConfiguredTableAssociation",
+            "action": "DeletePrivacyBudgetTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "cleanrooms-ml": {
-        "GetTrainingDataset": {
+        "DeleteConfiguredAudienceModel": {
             "access_level": "Undocumented",
-            "action": "GetTrainingDataset",
+            "action": "DeleteConfiguredAudienceModel",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListConfiguredAudienceModels": {
+        "ListAudienceGenerationJobs": {
             "access_level": "Undocumented",
-            "action": "ListConfiguredAudienceModels",
+            "action": "ListAudienceGenerationJobs",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetConfiguredAudienceModel": {
+        "StartAudienceGenerationJob": {
             "access_level": "Undocumented",
-            "action": "GetConfiguredAudienceModel",
+            "action": "StartAudienceGenerationJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTrainingDatasets": {
+        "CreateAudienceModel": {
             "access_level": "Undocumented",
-            "action": "ListTrainingDatasets",
+            "action": "CreateAudienceModel",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateAudienceModel": {
+        "GetConfiguredAudienceModel": {
             "access_level": "Undocumented",
-            "action": "CreateAudienceModel",
+            "action": "GetConfiguredAudienceModel",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "ListConfiguredAudienceModels": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "ListConfiguredAudienceModels",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartAudienceGenerationJob": {
+        "UnTagResource": {
             "access_level": "Undocumented",
-            "action": "StartAudienceGenerationJob",
+            "action": "UnTagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetConfiguredAudienceModelPolicy": {
+        "GetTrainingDataset": {
             "access_level": "Undocumented",
-            "action": "GetConfiguredAudienceModelPolicy",
+            "action": "GetTrainingDataset",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAudienceGenerationJobs": {
+        "UpdateConfiguredAudienceModel": {
             "access_level": "Undocumented",
-            "action": "ListAudienceGenerationJobs",
+            "action": "UpdateConfiguredAudienceModel",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateConfiguredAudienceModel": {
+        "GetAudienceModel": {
             "access_level": "Undocumented",
-            "action": "CreateConfiguredAudienceModel",
+            "action": "GetAudienceModel",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAudienceGenerationJob": {
+        "ListAudienceModels": {
             "access_level": "Undocumented",
-            "action": "GetAudienceGenerationJob",
+            "action": "ListAudienceModels",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateConfiguredAudienceModel": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "UpdateConfiguredAudienceModel",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateTrainingDataset": {
+        "DeleteAudienceModel": {
             "access_level": "Undocumented",
-            "action": "CreateTrainingDataset",
+            "action": "DeleteAudienceModel",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteAudienceModel": {
+        "ListAudienceExportJobs": {
             "access_level": "Undocumented",
-            "action": "DeleteAudienceModel",
+            "action": "ListAudienceExportJobs",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAudienceModels": {
+        "DeleteTrainingDataset": {
             "access_level": "Undocumented",
-            "action": "ListAudienceModels",
+            "action": "DeleteTrainingDataset",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteAudienceGenerationJob": {
+        "PutConfiguredAudienceModelPolicy": {
             "access_level": "Undocumented",
-            "action": "DeleteAudienceGenerationJob",
+            "action": "PutConfiguredAudienceModelPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteTrainingDataset": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "DeleteTrainingDataset",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UnTagResource": {
+        "ListTrainingDatasets": {
             "access_level": "Undocumented",
-            "action": "UnTagResource",
+            "action": "ListTrainingDatasets",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutConfiguredAudienceModelPolicy": {
+        "CreateConfiguredAudienceModel": {
             "access_level": "Undocumented",
-            "action": "PutConfiguredAudienceModelPolicy",
+            "action": "CreateConfiguredAudienceModel",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartAudienceExportJob": {
+        "GetAudienceGenerationJob": {
             "access_level": "Undocumented",
-            "action": "StartAudienceExportJob",
+            "action": "GetAudienceGenerationJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "StartAudienceExportJob": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "StartAudienceExportJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAudienceExportJobs": {
+        "GetConfiguredAudienceModelPolicy": {
             "access_level": "Undocumented",
-            "action": "ListAudienceExportJobs",
+            "action": "GetConfiguredAudienceModelPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteConfiguredAudienceModelPolicy": {
+        "DeleteAudienceGenerationJob": {
             "access_level": "Undocumented",
-            "action": "DeleteConfiguredAudienceModelPolicy",
+            "action": "DeleteAudienceGenerationJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteConfiguredAudienceModel": {
+        "DeleteConfiguredAudienceModelPolicy": {
             "access_level": "Undocumented",
-            "action": "DeleteConfiguredAudienceModel",
+            "action": "DeleteConfiguredAudienceModelPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAudienceModel": {
+        "CreateTrainingDataset": {
             "access_level": "Undocumented",
-            "action": "GetAudienceModel",
+            "action": "CreateTrainingDataset",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "cloud9": {
@@ -23447,57 +23447,57 @@
             "orphan": false,
             "resources": [
                 "streaming-distribution"
             ]
         }
     },
     "cloudfront-keyvaluestore": {
-        "GetKey": {
+        "PutKey": {
             "access_level": "Undocumented",
-            "action": "GetKey",
+            "action": "PutKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeKeyValueStore": {
+        "UpdateKeys": {
             "access_level": "Undocumented",
-            "action": "DescribeKeyValueStore",
+            "action": "UpdateKeys",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteKey": {
+        "GetKey": {
             "access_level": "Undocumented",
-            "action": "DeleteKey",
+            "action": "GetKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutKey": {
+        "DeleteKey": {
             "access_level": "Undocumented",
-            "action": "PutKey",
+            "action": "DeleteKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateKeys": {
+        "ListKeys": {
             "access_level": "Undocumented",
-            "action": "UpdateKeys",
+            "action": "ListKeys",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListKeys": {
+        "DescribeKeyValueStore": {
             "access_level": "Undocumented",
-            "action": "ListKeys",
+            "action": "DescribeKeyValueStore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "cloudhsm": {
@@ -27649,305 +27649,305 @@
             "orphan": false,
             "resources": [
                 "repository"
             ]
         }
     },
     "codeconnections": {
-        "GetSyncBlockerSummary": {
+        "DeleteHost": {
             "access_level": "Undocumented",
-            "action": "GetSyncBlockerSummary",
+            "action": "DeleteHost",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UseConnection": {
+        "StartOAuthHandshake": {
             "access_level": "Undocumented",
-            "action": "UseConnection",
+            "action": "StartOAuthHandshake",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartOAuthHandshake": {
+        "CreateConnection": {
             "access_level": "Undocumented",
-            "action": "StartOAuthHandshake",
+            "action": "CreateConnection",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetConnection": {
+        "DeleteSyncConfiguration": {
             "access_level": "Undocumented",
-            "action": "GetConnection",
+            "action": "DeleteSyncConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateRepositoryLink": {
+        "ListRepositoryLinks": {
             "access_level": "Undocumented",
-            "action": "CreateRepositoryLink",
+            "action": "ListRepositoryLinks",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "GetRepositoryLink": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "GetRepositoryLink",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetRepositoryLink": {
+        "RegisterAppCode": {
             "access_level": "Undocumented",
-            "action": "GetRepositoryLink",
+            "action": "RegisterAppCode",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateHost": {
+        "ListHosts": {
             "access_level": "Undocumented",
-            "action": "UpdateHost",
+            "action": "ListHosts",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListRepositorySyncDefinitions": {
+        "ListSyncConfigurations": {
             "access_level": "Undocumented",
-            "action": "ListRepositorySyncDefinitions",
+            "action": "ListSyncConfigurations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PassRepository": {
+        "GetRepositorySyncStatus": {
             "access_level": "Undocumented",
-            "action": "PassRepository",
+            "action": "GetRepositorySyncStatus",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateHost": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "CreateHost",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetResourceSyncStatus": {
+        "GetInstallationUrl": {
             "access_level": "Undocumented",
-            "action": "GetResourceSyncStatus",
+            "action": "GetInstallationUrl",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateRepositoryLink": {
+        "UpdateSyncConfiguration": {
             "access_level": "Undocumented",
-            "action": "UpdateRepositoryLink",
+            "action": "UpdateSyncConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateConnection": {
+        "DeleteConnection": {
             "access_level": "Undocumented",
-            "action": "CreateConnection",
+            "action": "DeleteConnection",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSyncConfiguration": {
+        "GetResourceSyncStatus": {
             "access_level": "Undocumented",
-            "action": "GetSyncConfiguration",
+            "action": "GetResourceSyncStatus",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteSyncConfiguration": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "DeleteSyncConfiguration",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetRepositorySyncStatus": {
+        "PassConnection": {
             "access_level": "Undocumented",
-            "action": "GetRepositorySyncStatus",
+            "action": "PassConnection",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListRepositoryLinks": {
+        "ListConnections": {
             "access_level": "Undocumented",
-            "action": "ListRepositoryLinks",
+            "action": "ListConnections",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteRepositoryLink": {
+        "UpdateSyncBlocker": {
             "access_level": "Undocumented",
-            "action": "DeleteRepositoryLink",
+            "action": "UpdateSyncBlocker",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateSyncConfiguration": {
+        "ListInstallationTargets": {
             "access_level": "Undocumented",
-            "action": "UpdateSyncConfiguration",
+            "action": "ListInstallationTargets",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartAppRegistrationHandshake": {
+        "CreateSyncConfiguration": {
             "access_level": "Undocumented",
-            "action": "StartAppRegistrationHandshake",
+            "action": "CreateSyncConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateSyncBlocker": {
+        "StartAppRegistrationHandshake": {
             "access_level": "Undocumented",
-            "action": "UpdateSyncBlocker",
+            "action": "StartAppRegistrationHandshake",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateConnectionInstallation": {
+        "GetSyncConfiguration": {
             "access_level": "Undocumented",
-            "action": "UpdateConnectionInstallation",
+            "action": "GetSyncConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListHosts": {
+        "UpdateHost": {
             "access_level": "Undocumented",
-            "action": "ListHosts",
+            "action": "UpdateHost",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetIndividualAccessToken": {
+        "UpdateRepositoryLink": {
             "access_level": "Undocumented",
-            "action": "GetIndividualAccessToken",
+            "action": "UpdateRepositoryLink",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListConnections": {
+        "GetHost": {
             "access_level": "Undocumented",
-            "action": "ListConnections",
+            "action": "GetHost",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteConnection": {
+        "GetIndividualAccessToken": {
             "access_level": "Undocumented",
-            "action": "DeleteConnection",
+            "action": "GetIndividualAccessToken",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "GetSyncBlockerSummary": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "GetSyncBlockerSummary",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RegisterAppCode": {
+        "DeleteRepositoryLink": {
             "access_level": "Undocumented",
-            "action": "RegisterAppCode",
+            "action": "DeleteRepositoryLink",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetInstallationUrl": {
+        "UpdateConnectionInstallation": {
             "access_level": "Undocumented",
-            "action": "GetInstallationUrl",
+            "action": "UpdateConnectionInstallation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateSyncConfiguration": {
+        "PassRepository": {
             "access_level": "Undocumented",
-            "action": "CreateSyncConfiguration",
+            "action": "PassRepository",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListInstallationTargets": {
+        "CreateHost": {
             "access_level": "Undocumented",
-            "action": "ListInstallationTargets",
+            "action": "CreateHost",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetHost": {
+        "UseConnection": {
             "access_level": "Undocumented",
-            "action": "GetHost",
+            "action": "UseConnection",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSyncConfigurations": {
+        "GetConnection": {
             "access_level": "Undocumented",
-            "action": "ListSyncConfigurations",
+            "action": "GetConnection",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PassConnection": {
+        "CreateRepositoryLink": {
             "access_level": "Undocumented",
-            "action": "PassConnection",
+            "action": "CreateRepositoryLink",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteHost": {
+        "ListRepositorySyncDefinitions": {
             "access_level": "Undocumented",
-            "action": "DeleteHost",
+            "action": "ListRepositorySyncDefinitions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "codedeploy": {
@@ -28879,129 +28879,129 @@
             "orphan": false,
             "resources": [
                 "association"
             ]
         }
     },
     "codeguru-security": {
-        "ListFindingsMetrics": {
+        "GetScan": {
             "access_level": "Undocumented",
-            "action": "ListFindingsMetrics",
+            "action": "GetScan",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetScan": {
+        "CreateUploadUrl": {
             "access_level": "Undocumented",
-            "action": "GetScan",
+            "action": "CreateUploadUrl",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetMetricsSummary": {
+        "ListFindings": {
             "access_level": "Undocumented",
-            "action": "GetMetricsSummary",
+            "action": "ListFindings",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "GetMetricsSummary": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "GetMetricsSummary",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateAccountConfiguration": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "UpdateAccountConfiguration",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListFindings": {
+        "ListFindingsMetrics": {
             "access_level": "Undocumented",
-            "action": "ListFindings",
+            "action": "ListFindingsMetrics",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateScan": {
+        "UpdateAccountConfiguration": {
             "access_level": "Undocumented",
-            "action": "CreateScan",
+            "action": "UpdateAccountConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "BatchGetFindings": {
+        "DeleteScansByCategory": {
             "access_level": "Undocumented",
-            "action": "BatchGetFindings",
+            "action": "DeleteScansByCategory",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAccountConfiguration": {
+        "CreateScan": {
             "access_level": "Undocumented",
-            "action": "GetAccountConfiguration",
+            "action": "CreateScan",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "GetFindings": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "GetFindings",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListScans": {
+        "GetAccountConfiguration": {
             "access_level": "Undocumented",
-            "action": "ListScans",
+            "action": "GetAccountConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetFindings": {
+        "ListScans": {
             "access_level": "Undocumented",
-            "action": "GetFindings",
+            "action": "ListScans",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteScansByCategory": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "DeleteScansByCategory",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateUploadUrl": {
+        "BatchGetFindings": {
             "access_level": "Undocumented",
-            "action": "CreateUploadUrl",
+            "action": "BatchGetFindings",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "codepipeline": {
@@ -37515,25 +37515,25 @@
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "consolidatedbilling": {
-        "ListLinkedAccounts": {
+        "GetAccountBillingRole": {
             "access_level": "Undocumented",
-            "action": "ListLinkedAccounts",
+            "action": "GetAccountBillingRole",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAccountBillingRole": {
+        "ListLinkedAccounts": {
             "access_level": "Undocumented",
-            "action": "GetAccountBillingRole",
+            "action": "ListLinkedAccounts",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "controltower": {
@@ -38083,65 +38083,65 @@
             "orphan": false,
             "resources": [
                 "LandingZone"
             ]
         }
     },
     "cost-optimization-hub": {
-        "UpdateEnrollmentStatus": {
+        "ListRecommendations": {
             "access_level": "Undocumented",
-            "action": "UpdateEnrollmentStatus",
+            "action": "ListRecommendations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListEnrollmentStatuses": {
+        "UpdatePreferences": {
             "access_level": "Undocumented",
-            "action": "ListEnrollmentStatuses",
+            "action": "UpdatePreferences",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPreferences": {
+        "ListEnrollmentStatuses": {
             "access_level": "Undocumented",
-            "action": "GetPreferences",
+            "action": "ListEnrollmentStatuses",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListRecommendationSummaries": {
+        "GetPreferences": {
             "access_level": "Undocumented",
-            "action": "ListRecommendationSummaries",
+            "action": "GetPreferences",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListRecommendations": {
+        "GetRecommendation": {
             "access_level": "Undocumented",
-            "action": "ListRecommendations",
+            "action": "GetRecommendation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdatePreferences": {
+        "ListRecommendationSummaries": {
             "access_level": "Undocumented",
-            "action": "UpdatePreferences",
+            "action": "ListRecommendationSummaries",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetRecommendation": {
+        "UpdateEnrollmentStatus": {
             "access_level": "Undocumented",
-            "action": "GetRecommendation",
+            "action": "UpdateEnrollmentStatus",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "cur": {
@@ -38260,41 +38260,41 @@
             "condition_keys": [],
             "description": "Grants permission to validates if the s3 bucket exists with appropriate permissions for CUR delivery",
             "orphan": false,
             "resources": []
         }
     },
     "customer-verification": {
-        "UpdateCustomerVerificationDetails": {
+        "GetCustomerVerificationEligibility": {
             "access_level": "Undocumented",
-            "action": "UpdateCustomerVerificationDetails",
+            "action": "GetCustomerVerificationEligibility",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateCustomerVerificationDetails": {
+        "GetCustomerVerificationDetails": {
             "access_level": "Undocumented",
-            "action": "CreateCustomerVerificationDetails",
+            "action": "GetCustomerVerificationDetails",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetCustomerVerificationEligibility": {
+        "CreateCustomerVerificationDetails": {
             "access_level": "Undocumented",
-            "action": "GetCustomerVerificationEligibility",
+            "action": "CreateCustomerVerificationDetails",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetCustomerVerificationDetails": {
+        "UpdateCustomerVerificationDetails": {
             "access_level": "Undocumented",
-            "action": "GetCustomerVerificationDetails",
+            "action": "UpdateCustomerVerificationDetails",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "databrew": {
@@ -39978,1033 +39978,1033 @@
             "orphan": false,
             "resources": [
                 "taskexecution"
             ]
         }
     },
     "datazone": {
-        "Search": {
+        "RejectSubscriptionRequest": {
             "access_level": "Undocumented",
-            "action": "Search",
+            "action": "RejectSubscriptionRequest",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteSubscriptionGrant": {
+        "UpdateEnvironmentProfile": {
             "access_level": "Undocumented",
-            "action": "DeleteSubscriptionGrant",
+            "action": "UpdateEnvironmentProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateSubscriptionTarget": {
+        "DeleteGlossaryTerm": {
             "access_level": "Undocumented",
-            "action": "UpdateSubscriptionTarget",
+            "action": "DeleteGlossaryTerm",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SsoLogout": {
+        "UpdateUserProfile": {
             "access_level": "Undocumented",
-            "action": "SsoLogout",
+            "action": "UpdateUserProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetDataSource": {
+        "CreateAsset": {
             "access_level": "Undocumented",
-            "action": "GetDataSource",
+            "action": "CreateAsset",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RefreshToken": {
+        "CancelMetadataGenerationRun": {
             "access_level": "Undocumented",
-            "action": "RefreshToken",
+            "action": "CancelMetadataGenerationRun",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSubscriptions": {
+        "GetDomain": {
             "access_level": "Undocumented",
-            "action": "ListSubscriptions",
+            "action": "GetDomain",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetUserProfile": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "GetUserProfile",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteAssetType": {
+        "GetGlossary": {
             "access_level": "Undocumented",
-            "action": "DeleteAssetType",
+            "action": "GetGlossary",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteTimeSeriesDataPoints": {
+        "ListAccountEnvironments": {
             "access_level": "Undocumented",
-            "action": "DeleteTimeSeriesDataPoints",
+            "action": "ListAccountEnvironments",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteAsset": {
+        "CreateProject": {
             "access_level": "Undocumented",
-            "action": "DeleteAsset",
+            "action": "CreateProject",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListGroupsForUser": {
+        "PutDomainSharingPolicy": {
             "access_level": "Undocumented",
-            "action": "ListGroupsForUser",
+            "action": "PutDomainSharingPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ValidatePassRole": {
+        "UpdateDomain": {
             "access_level": "Undocumented",
-            "action": "ValidatePassRole",
+            "action": "UpdateDomain",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateGlossaryTerm": {
+        "CancelSubscription": {
             "access_level": "Undocumented",
-            "action": "UpdateGlossaryTerm",
+            "action": "CancelSubscription",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListDataSourceRuns": {
+        "CreateDomain": {
             "access_level": "Undocumented",
-            "action": "ListDataSourceRuns",
+            "action": "CreateDomain",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateAssetRevision": {
+        "ListWarehouseMetadata": {
             "access_level": "Undocumented",
-            "action": "CreateAssetRevision",
+            "action": "ListWarehouseMetadata",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartDataSourceRun": {
+        "DeleteSubscriptionGrant": {
             "access_level": "Undocumented",
-            "action": "StartDataSourceRun",
+            "action": "DeleteSubscriptionGrant",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StopMetadataGenerationRun": {
+        "GetSubscriptionGrant": {
             "access_level": "Undocumented",
-            "action": "StopMetadataGenerationRun",
+            "action": "GetSubscriptionGrant",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListProjectMemberships": {
+        "UpdateEnvironmentDeploymentStatus": {
             "access_level": "Undocumented",
-            "action": "ListProjectMemberships",
+            "action": "UpdateEnvironmentDeploymentStatus",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateSubscriptionRequest": {
+        "UpdateGlossary": {
             "access_level": "Undocumented",
-            "action": "UpdateSubscriptionRequest",
+            "action": "UpdateGlossary",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RevokeSubscription": {
+        "ListSubscriptionGrants": {
             "access_level": "Undocumented",
-            "action": "RevokeSubscription",
+            "action": "ListSubscriptionGrants",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteDomainSharingPolicy": {
+        "DeleteTimeSeriesDataPoints": {
             "access_level": "Undocumented",
-            "action": "DeleteDomainSharingPolicy",
+            "action": "DeleteTimeSeriesDataPoints",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateProject": {
+        "ListEnvironmentBlueprints": {
             "access_level": "Undocumented",
-            "action": "CreateProject",
+            "action": "ListEnvironmentBlueprints",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateSubscriptionGrant": {
+        "ListSubscriptions": {
             "access_level": "Undocumented",
-            "action": "CreateSubscriptionGrant",
+            "action": "ListSubscriptions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SearchTypes": {
+        "StartDataSourceRun": {
             "access_level": "Undocumented",
-            "action": "SearchTypes",
+            "action": "StartDataSourceRun",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetListing": {
+        "ListProjects": {
             "access_level": "Undocumented",
-            "action": "GetListing",
+            "action": "ListProjects",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSubscriptionRequestDetails": {
+        "CreateFormType": {
             "access_level": "Undocumented",
-            "action": "GetSubscriptionRequestDetails",
+            "action": "CreateFormType",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateListingChangeSet": {
+        "DeleteDomain": {
             "access_level": "Undocumented",
-            "action": "CreateListingChangeSet",
+            "action": "DeleteDomain",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateAssetType": {
+        "UpdateDataSource": {
             "access_level": "Undocumented",
-            "action": "CreateAssetType",
+            "action": "UpdateDataSource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateSubscriptionTarget": {
+        "GetEnvironmentActionLink": {
             "access_level": "Undocumented",
-            "action": "CreateSubscriptionTarget",
+            "action": "GetEnvironmentActionLink",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateGlossary": {
+        "DeleteEnvironment": {
             "access_level": "Undocumented",
-            "action": "UpdateGlossary",
+            "action": "DeleteEnvironment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListDataSourceRunActivities": {
+        "RejectPredictions": {
             "access_level": "Undocumented",
-            "action": "ListDataSourceRunActivities",
+            "action": "RejectPredictions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTimeSeriesDataPoints": {
+        "GetSubscription": {
             "access_level": "Undocumented",
-            "action": "ListTimeSeriesDataPoints",
+            "action": "GetSubscription",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteEnvironmentProfile": {
+        "ListAssetRevisions": {
             "access_level": "Undocumented",
-            "action": "DeleteEnvironmentProfile",
+            "action": "ListAssetRevisions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateDomain": {
+        "UpdateEnvironmentConfiguration": {
             "access_level": "Undocumented",
-            "action": "UpdateDomain",
+            "action": "UpdateEnvironmentConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutEnvironmentBlueprintConfiguration": {
+        "CreateDataSource": {
             "access_level": "Undocumented",
-            "action": "PutEnvironmentBlueprintConfiguration",
+            "action": "CreateDataSource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteListing": {
+        "SsoLogin": {
             "access_level": "Undocumented",
-            "action": "DeleteListing",
+            "action": "SsoLogin",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteEnvironmentBlueprint": {
+        "GetEnvironmentBlueprintConfiguration": {
             "access_level": "Undocumented",
-            "action": "DeleteEnvironmentBlueprint",
+            "action": "GetEnvironmentBlueprintConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteEnvironment": {
+        "DeleteDomainSharingPolicy": {
             "access_level": "Undocumented",
-            "action": "DeleteEnvironment",
+            "action": "DeleteDomainSharingPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateDataSource": {
+        "PostTimeSeriesDataPoints": {
             "access_level": "Undocumented",
-            "action": "UpdateDataSource",
+            "action": "PostTimeSeriesDataPoints",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetGlossaryTerm": {
+        "UpdateSubscriptionGrantStatus": {
             "access_level": "Undocumented",
-            "action": "GetGlossaryTerm",
+            "action": "UpdateSubscriptionGrantStatus",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateProject": {
+        "SearchTypes": {
             "access_level": "Undocumented",
-            "action": "UpdateProject",
+            "action": "SearchTypes",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetIamPortalLoginUrl": {
+        "CreateSubscriptionGrant": {
             "access_level": "Undocumented",
-            "action": "GetIamPortalLoginUrl",
+            "action": "CreateSubscriptionGrant",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListEnvironmentBlueprintConfigurations": {
+        "DeleteEnvironmentBlueprintConfiguration": {
             "access_level": "Undocumented",
-            "action": "ListEnvironmentBlueprintConfigurations",
+            "action": "DeleteEnvironmentBlueprintConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteSubscriptionRequest": {
+        "GetDataSource": {
             "access_level": "Undocumented",
-            "action": "DeleteSubscriptionRequest",
+            "action": "GetDataSource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListProjects": {
+        "UpdateGroupProfile": {
             "access_level": "Undocumented",
-            "action": "ListProjects",
+            "action": "UpdateGroupProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "DeleteDataSource": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "DeleteDataSource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CancelSubscription": {
+        "DeleteProjectMembership": {
             "access_level": "Undocumented",
-            "action": "CancelSubscription",
+            "action": "DeleteProjectMembership",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListDataSources": {
+        "DeleteSubscriptionTarget": {
             "access_level": "Undocumented",
-            "action": "ListDataSources",
+            "action": "DeleteSubscriptionTarget",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetGlossary": {
+        "RevokeSubscription": {
             "access_level": "Undocumented",
-            "action": "GetGlossary",
+            "action": "RevokeSubscription",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSubscriptionGrant": {
+        "StartMetadataGenerationRun": {
             "access_level": "Undocumented",
-            "action": "GetSubscriptionGrant",
+            "action": "StartMetadataGenerationRun",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SearchGroupProfiles": {
+        "CreateAssetType": {
             "access_level": "Undocumented",
-            "action": "SearchGroupProfiles",
+            "action": "CreateAssetType",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartMetadataGenerationRun": {
+        "GetAsset": {
             "access_level": "Undocumented",
-            "action": "StartMetadataGenerationRun",
+            "action": "GetAsset",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "GetEnvironment": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "GetEnvironment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetFormType": {
+        "SearchListings": {
             "access_level": "Undocumented",
-            "action": "GetFormType",
+            "action": "SearchListings",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SearchListings": {
+        "GetMetadataGenerationRun": {
             "access_level": "Undocumented",
-            "action": "SearchListings",
+            "action": "GetMetadataGenerationRun",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateGroupProfile": {
+        "GetDomainSharingPolicy": {
             "access_level": "Undocumented",
-            "action": "UpdateGroupProfile",
+            "action": "GetDomainSharingPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSubscriptionRequests": {
+        "GetSubscriptionTarget": {
             "access_level": "Undocumented",
-            "action": "ListSubscriptionRequests",
+            "action": "GetSubscriptionTarget",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetDomain": {
+        "CreateProjectMembership": {
             "access_level": "Undocumented",
-            "action": "GetDomain",
+            "action": "CreateProjectMembership",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ProvisionDomain": {
+        "GetListing": {
             "access_level": "Undocumented",
-            "action": "ProvisionDomain",
+            "action": "GetListing",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateEnvironment": {
+        "UpdateSubscriptionTarget": {
             "access_level": "Undocumented",
-            "action": "UpdateEnvironment",
+            "action": "UpdateSubscriptionTarget",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAssetType": {
+        "CreateListingChangeSet": {
             "access_level": "Undocumented",
-            "action": "GetAssetType",
+            "action": "CreateListingChangeSet",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteGlossaryTerm": {
+        "GetEnvironmentCredentials": {
             "access_level": "Undocumented",
-            "action": "DeleteGlossaryTerm",
+            "action": "GetEnvironmentCredentials",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateDataSource": {
+        "UpdateProject": {
             "access_level": "Undocumented",
-            "action": "CreateDataSource",
+            "action": "UpdateProject",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateSubscriptionRequest": {
+        "UpdateEnvironment": {
             "access_level": "Undocumented",
-            "action": "CreateSubscriptionRequest",
+            "action": "UpdateEnvironment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListEnvironments": {
+        "ListSubscriptionRequests": {
             "access_level": "Undocumented",
-            "action": "ListEnvironments",
+            "action": "ListSubscriptionRequests",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListMetadataGenerationRuns": {
+        "UpdateGlossaryTerm": {
             "access_level": "Undocumented",
-            "action": "ListMetadataGenerationRuns",
+            "action": "UpdateGlossaryTerm",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAsset": {
+        "CreateGroupProfile": {
             "access_level": "Undocumented",
-            "action": "GetAsset",
+            "action": "CreateGroupProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetDomainSharingPolicy": {
+        "GetDataSourceRun": {
             "access_level": "Undocumented",
-            "action": "GetDomainSharingPolicy",
+            "action": "GetDataSourceRun",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSubscriptionTarget": {
+        "ListTimeSeriesDataPoints": {
             "access_level": "Undocumented",
-            "action": "GetSubscriptionTarget",
+            "action": "ListTimeSeriesDataPoints",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AcceptPredictions": {
+        "SearchUserProfiles": {
             "access_level": "Undocumented",
-            "action": "AcceptPredictions",
+            "action": "SearchUserProfiles",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAccountEnvironments": {
+        "SearchGroupProfiles": {
             "access_level": "Undocumented",
-            "action": "ListAccountEnvironments",
+            "action": "SearchGroupProfiles",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SsoLogin": {
+        "DeleteSubscriptionRequest": {
             "access_level": "Undocumented",
-            "action": "SsoLogin",
+            "action": "DeleteSubscriptionRequest",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateEnvironment": {
+        "AcceptPredictions": {
             "access_level": "Undocumented",
-            "action": "CreateEnvironment",
+            "action": "AcceptPredictions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListNotifications": {
+        "ListSubscriptionTargets": {
             "access_level": "Undocumented",
-            "action": "ListNotifications",
+            "action": "ListSubscriptionTargets",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateSubscriptionGrantStatus": {
+        "DeleteListing": {
             "access_level": "Undocumented",
-            "action": "UpdateSubscriptionGrantStatus",
+            "action": "DeleteListing",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetGroupProfile": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "GetGroupProfile",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateGlossary": {
+        "DeleteGlossary": {
             "access_level": "Undocumented",
-            "action": "CreateGlossary",
+            "action": "DeleteGlossary",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateEnvironmentConfiguration": {
+        "ListDataSourceRuns": {
             "access_level": "Undocumented",
-            "action": "UpdateEnvironmentConfiguration",
+            "action": "ListDataSourceRuns",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateProjectMembership": {
+        "ListNotifications": {
             "access_level": "Undocumented",
-            "action": "CreateProjectMembership",
+            "action": "ListNotifications",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateFormType": {
+        "UpdateEnvironmentBlueprint": {
             "access_level": "Undocumented",
-            "action": "CreateFormType",
+            "action": "UpdateEnvironmentBlueprint",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateUserProfile": {
+        "ListEnvironmentBlueprintConfigurationSummaries": {
             "access_level": "Undocumented",
-            "action": "CreateUserProfile",
+            "action": "ListEnvironmentBlueprintConfigurationSummaries",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListWarehouseMetadata": {
+        "CreateEnvironmentProfile": {
             "access_level": "Undocumented",
-            "action": "ListWarehouseMetadata",
+            "action": "CreateEnvironmentProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetEnvironment": {
+        "GetIamPortalLoginUrl": {
             "access_level": "Undocumented",
-            "action": "GetEnvironment",
+            "action": "GetIamPortalLoginUrl",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteGlossary": {
+        "CreateSubscriptionTarget": {
             "access_level": "Undocumented",
-            "action": "DeleteGlossary",
+            "action": "CreateSubscriptionTarget",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetEnvironmentProfile": {
+        "ListMetadataGenerationRuns": {
             "access_level": "Undocumented",
-            "action": "GetEnvironmentProfile",
+            "action": "ListMetadataGenerationRuns",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetEnvironmentBlueprintConfiguration": {
+        "DeleteProject": {
             "access_level": "Undocumented",
-            "action": "GetEnvironmentBlueprintConfiguration",
+            "action": "DeleteProject",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSubscription": {
+        "GetSubscriptionEligibility": {
             "access_level": "Undocumented",
-            "action": "GetSubscription",
+            "action": "GetSubscriptionEligibility",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "GetEnvironmentBlueprint": {
             "access_level": "Undocumented",
             "action": "GetEnvironmentBlueprint",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteDataSource": {
+        "ListEnvironments": {
             "access_level": "Undocumented",
-            "action": "DeleteDataSource",
+            "action": "ListEnvironments",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateEnvironmentProfile": {
+        "GetTimeSeriesDataPoint": {
             "access_level": "Undocumented",
-            "action": "UpdateEnvironmentProfile",
+            "action": "GetTimeSeriesDataPoint",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteEnvironmentBlueprintConfiguration": {
+        "CreateAssetRevision": {
             "access_level": "Undocumented",
-            "action": "DeleteEnvironmentBlueprintConfiguration",
+            "action": "CreateAssetRevision",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PostTimeSeriesDataPoints": {
+        "CreateEnvironmentBlueprint": {
             "access_level": "Undocumented",
-            "action": "PostTimeSeriesDataPoints",
+            "action": "CreateEnvironmentBlueprint",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SearchUserProfiles": {
+        "CreateSubscriptionRequest": {
             "access_level": "Undocumented",
-            "action": "SearchUserProfiles",
+            "action": "CreateSubscriptionRequest",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListDomains": {
+        "ListEnvironmentBlueprintConfigurations": {
             "access_level": "Undocumented",
-            "action": "ListDomains",
+            "action": "ListEnvironmentBlueprintConfigurations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteDomain": {
+        "ListProjectMemberships": {
             "access_level": "Undocumented",
-            "action": "DeleteDomain",
+            "action": "ListProjectMemberships",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateAsset": {
+        "CreateGlossary": {
             "access_level": "Undocumented",
-            "action": "CreateAsset",
+            "action": "CreateGlossary",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetDataSourceRun": {
+        "ListEnvironmentProfiles": {
             "access_level": "Undocumented",
-            "action": "GetDataSourceRun",
+            "action": "ListEnvironmentProfiles",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AcceptSubscriptionRequest": {
+        "DeleteAsset": {
             "access_level": "Undocumented",
-            "action": "AcceptSubscriptionRequest",
+            "action": "DeleteAsset",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateUserProfile": {
+        "AcceptSubscriptionRequest": {
             "access_level": "Undocumented",
-            "action": "UpdateUserProfile",
+            "action": "AcceptSubscriptionRequest",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetMetadataGenerationRun": {
+        "GetGroupProfile": {
             "access_level": "Undocumented",
-            "action": "GetMetadataGenerationRun",
+            "action": "GetGroupProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "CreateUserProfile": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "CreateUserProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSubscriptionEligibility": {
+        "ValidatePassRole": {
             "access_level": "Undocumented",
-            "action": "GetSubscriptionEligibility",
+            "action": "ValidatePassRole",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateEnvironmentBlueprint": {
+        "GetEnvironmentProfile": {
             "access_level": "Undocumented",
-            "action": "CreateEnvironmentBlueprint",
+            "action": "GetEnvironmentProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetProject": {
+        "RefreshToken": {
             "access_level": "Undocumented",
-            "action": "GetProject",
+            "action": "RefreshToken",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSubscriptionGrants": {
+        "DeleteEnvironmentBlueprint": {
             "access_level": "Undocumented",
-            "action": "ListSubscriptionGrants",
+            "action": "DeleteEnvironmentBlueprint",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteFormType": {
+        "ProvisionDomain": {
             "access_level": "Undocumented",
-            "action": "DeleteFormType",
+            "action": "ProvisionDomain",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RejectSubscriptionRequest": {
+        "CreateEnvironment": {
             "access_level": "Undocumented",
-            "action": "RejectSubscriptionRequest",
+            "action": "CreateEnvironment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetTimeSeriesDataPoint": {
+        "CreateGlossaryTerm": {
             "access_level": "Undocumented",
-            "action": "GetTimeSeriesDataPoint",
+            "action": "CreateGlossaryTerm",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetEnvironmentActionLink": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "GetEnvironmentActionLink",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAssetRevisions": {
+        "ListDataSources": {
             "access_level": "Undocumented",
-            "action": "ListAssetRevisions",
+            "action": "ListDataSources",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateGroupProfile": {
+        "UpdateSubscriptionRequest": {
             "access_level": "Undocumented",
-            "action": "CreateGroupProfile",
+            "action": "UpdateSubscriptionRequest",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RejectPredictions": {
+        "GetProject": {
             "access_level": "Undocumented",
-            "action": "RejectPredictions",
+            "action": "GetProject",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateEnvironmentBlueprint": {
+        "ListGroupsForUser": {
             "access_level": "Undocumented",
-            "action": "UpdateEnvironmentBlueprint",
+            "action": "ListGroupsForUser",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateEnvironmentDeploymentStatus": {
+        "GetAssetType": {
             "access_level": "Undocumented",
-            "action": "UpdateEnvironmentDeploymentStatus",
+            "action": "GetAssetType",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteProjectMembership": {
+        "ListDataSourceRunActivities": {
             "access_level": "Undocumented",
-            "action": "DeleteProjectMembership",
+            "action": "ListDataSourceRunActivities",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListEnvironmentBlueprintConfigurationSummaries": {
+        "Search": {
             "access_level": "Undocumented",
-            "action": "ListEnvironmentBlueprintConfigurationSummaries",
+            "action": "Search",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteProject": {
+        "GetSubscriptionRequestDetails": {
             "access_level": "Undocumented",
-            "action": "DeleteProject",
+            "action": "GetSubscriptionRequestDetails",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateGlossaryTerm": {
+        "DeleteEnvironmentProfile": {
             "access_level": "Undocumented",
-            "action": "CreateGlossaryTerm",
+            "action": "DeleteEnvironmentProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CancelMetadataGenerationRun": {
+        "DeleteFormType": {
             "access_level": "Undocumented",
-            "action": "CancelMetadataGenerationRun",
+            "action": "DeleteFormType",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateEnvironmentProfile": {
+        "GetGlossaryTerm": {
             "access_level": "Undocumented",
-            "action": "CreateEnvironmentProfile",
+            "action": "GetGlossaryTerm",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetEnvironmentCredentials": {
+        "GetFormType": {
             "access_level": "Undocumented",
-            "action": "GetEnvironmentCredentials",
+            "action": "GetFormType",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateDomain": {
+        "GetUserProfile": {
             "access_level": "Undocumented",
-            "action": "CreateDomain",
+            "action": "GetUserProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListEnvironmentProfiles": {
+        "ListDomains": {
             "access_level": "Undocumented",
-            "action": "ListEnvironmentProfiles",
+            "action": "ListDomains",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListEnvironmentBlueprints": {
+        "StopMetadataGenerationRun": {
             "access_level": "Undocumented",
-            "action": "ListEnvironmentBlueprints",
+            "action": "StopMetadataGenerationRun",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutDomainSharingPolicy": {
+        "SsoLogout": {
             "access_level": "Undocumented",
-            "action": "PutDomainSharingPolicy",
+            "action": "SsoLogout",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSubscriptionTargets": {
+        "DeleteAssetType": {
             "access_level": "Undocumented",
-            "action": "ListSubscriptionTargets",
+            "action": "DeleteAssetType",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteSubscriptionTarget": {
+        "PutEnvironmentBlueprintConfiguration": {
             "access_level": "Undocumented",
-            "action": "DeleteSubscriptionTarget",
+            "action": "PutEnvironmentBlueprintConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "dax": {
@@ -41398,833 +41398,833 @@
             "condition_keys": [],
             "description": "Grants permission to update query tab",
             "orphan": false,
             "resources": []
         }
     },
     "deadline": {
-        "ListWorkers": {
+        "AssociateMemberToJob": {
             "access_level": "Undocumented",
-            "action": "ListWorkers",
+            "action": "AssociateMemberToJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListQueueMembers": {
+        "PutMeteredProduct": {
             "access_level": "Undocumented",
-            "action": "ListQueueMembers",
+            "action": "PutMeteredProduct",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSessionsStatisticsAggregation": {
+        "ListStorageProfilesForQueue": {
             "access_level": "Undocumented",
-            "action": "GetSessionsStatisticsAggregation",
+            "action": "ListStorageProfilesForQueue",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SearchJobs": {
+        "SearchSteps": {
             "access_level": "Undocumented",
-            "action": "SearchJobs",
+            "action": "SearchSteps",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateJob": {
+        "ListQueueMembers": {
             "access_level": "Undocumented",
-            "action": "UpdateJob",
+            "action": "ListQueueMembers",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutMeteredProduct": {
+        "GetStorageProfileForQueue": {
             "access_level": "Undocumented",
-            "action": "PutMeteredProduct",
+            "action": "GetStorageProfileForQueue",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetLicenseEndpoint": {
+        "UpdateWorker": {
             "access_level": "Undocumented",
-            "action": "GetLicenseEndpoint",
+            "action": "UpdateWorker",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSessions": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "ListSessions",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteStorageProfile": {
+        "DeleteLicenseEndpoint": {
             "access_level": "Undocumented",
-            "action": "DeleteStorageProfile",
+            "action": "DeleteLicenseEndpoint",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DisassociateMemberFromFleet": {
+        "CreateQueue": {
             "access_level": "Undocumented",
-            "action": "DisassociateMemberFromFleet",
+            "action": "CreateQueue",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SearchWorkers": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "SearchWorkers",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateQueue": {
+        "DeleteWorker": {
             "access_level": "Undocumented",
-            "action": "CreateQueue",
+            "action": "DeleteWorker",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateStorageProfile": {
+        "UpdateWorkerSchedule": {
             "access_level": "Undocumented",
-            "action": "UpdateStorageProfile",
+            "action": "UpdateWorkerSchedule",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssociateMemberToQueue": {
+        "CreateMonitor": {
             "access_level": "Undocumented",
-            "action": "AssociateMemberToQueue",
+            "action": "CreateMonitor",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListQueueEnvironments": {
+        "ListSessions": {
             "access_level": "Undocumented",
-            "action": "ListQueueEnvironments",
+            "action": "ListSessions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetQueueEnvironment": {
+        "BatchGetJobEntity": {
             "access_level": "Undocumented",
-            "action": "GetQueueEnvironment",
+            "action": "BatchGetJobEntity",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListQueueFleetAssociations": {
+        "DisassociateMemberFromFarm": {
             "access_level": "Undocumented",
-            "action": "ListQueueFleetAssociations",
+            "action": "DisassociateMemberFromFarm",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DisassociateMemberFromJob": {
+        "CreateBudget": {
             "access_level": "Undocumented",
-            "action": "DisassociateMemberFromJob",
+            "action": "CreateBudget",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DisassociateMemberFromFarm": {
+        "AssumeFleetRoleForWorker": {
             "access_level": "Undocumented",
-            "action": "DisassociateMemberFromFarm",
+            "action": "AssumeFleetRoleForWorker",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSessionsForWorker": {
+        "GetLicenseEndpoint": {
             "access_level": "Undocumented",
-            "action": "ListSessionsForWorker",
+            "action": "GetLicenseEndpoint",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListQueues": {
+        "GetQueue": {
             "access_level": "Undocumented",
-            "action": "ListQueues",
+            "action": "GetQueue",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssumeFleetRoleForRead": {
+        "GetSessionAction": {
             "access_level": "Undocumented",
-            "action": "AssumeFleetRoleForRead",
+            "action": "GetSessionAction",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetTask": {
+        "AssociateMemberToQueue": {
             "access_level": "Undocumented",
-            "action": "GetTask",
+            "action": "AssociateMemberToQueue",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateFarm": {
+        "GetWorker": {
             "access_level": "Undocumented",
-            "action": "UpdateFarm",
+            "action": "GetWorker",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetFarm": {
+        "ListQueueEnvironments": {
             "access_level": "Undocumented",
-            "action": "GetFarm",
+            "action": "ListQueueEnvironments",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateMonitor": {
+        "StartSessionsStatisticsAggregation": {
             "access_level": "Undocumented",
-            "action": "UpdateMonitor",
+            "action": "StartSessionsStatisticsAggregation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateWorker": {
+        "AssumeQueueRoleForWorker": {
             "access_level": "Undocumented",
-            "action": "CreateWorker",
+            "action": "AssumeQueueRoleForWorker",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateWorkerSchedule": {
+        "DeleteQueueFleetAssociation": {
             "access_level": "Undocumented",
-            "action": "UpdateWorkerSchedule",
+            "action": "DeleteQueueFleetAssociation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteQueue": {
+        "GetJob": {
             "access_level": "Undocumented",
-            "action": "DeleteQueue",
+            "action": "GetJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateFleet": {
+        "DeleteBudget": {
             "access_level": "Undocumented",
-            "action": "CreateFleet",
+            "action": "DeleteBudget",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAvailableMeteredProducts": {
+        "GetStep": {
             "access_level": "Undocumented",
-            "action": "ListAvailableMeteredProducts",
+            "action": "GetStep",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListBudgets": {
+        "SearchJobs": {
             "access_level": "Undocumented",
-            "action": "ListBudgets",
+            "action": "SearchJobs",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTasks": {
+        "CreateLicenseEndpoint": {
             "access_level": "Undocumented",
-            "action": "ListTasks",
+            "action": "CreateLicenseEndpoint",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CopyJobTemplate": {
+        "ListQueues": {
             "access_level": "Undocumented",
-            "action": "CopyJobTemplate",
+            "action": "ListQueues",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteFarm": {
+        "UpdateFleet": {
             "access_level": "Undocumented",
-            "action": "DeleteFarm",
+            "action": "UpdateFleet",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSessionAction": {
+        "ListWorkers": {
             "access_level": "Undocumented",
-            "action": "GetSessionAction",
+            "action": "ListWorkers",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateQueueEnvironment": {
+        "SearchWorkers": {
             "access_level": "Undocumented",
-            "action": "UpdateQueueEnvironment",
+            "action": "SearchWorkers",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSession": {
+        "ListFarms": {
             "access_level": "Undocumented",
-            "action": "GetSession",
+            "action": "ListFarms",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListFarms": {
+        "DisassociateMemberFromQueue": {
             "access_level": "Undocumented",
-            "action": "ListFarms",
+            "action": "DisassociateMemberFromQueue",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListStorageProfiles": {
+        "AssumeQueueRoleForUser": {
             "access_level": "Undocumented",
-            "action": "ListStorageProfiles",
+            "action": "AssumeQueueRoleForUser",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateFleet": {
+        "UpdateStorageProfile": {
             "access_level": "Undocumented",
-            "action": "UpdateFleet",
+            "action": "UpdateStorageProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListMeteredProducts": {
+        "UpdateSession": {
             "access_level": "Undocumented",
-            "action": "ListMeteredProducts",
+            "action": "UpdateSession",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartSessionsStatisticsAggregation": {
+        "CreateFarm": {
             "access_level": "Undocumented",
-            "action": "StartSessionsStatisticsAggregation",
+            "action": "CreateFarm",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListStorageProfilesForQueue": {
+        "GetTask": {
             "access_level": "Undocumented",
-            "action": "ListStorageProfilesForQueue",
+            "action": "GetTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssumeFleetRoleForWorker": {
+        "UpdateQueueEnvironment": {
             "access_level": "Undocumented",
-            "action": "AssumeFleetRoleForWorker",
+            "action": "UpdateQueueEnvironment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssumeQueueRoleForWorker": {
+        "ListMeteredProducts": {
             "access_level": "Undocumented",
-            "action": "AssumeQueueRoleForWorker",
+            "action": "ListMeteredProducts",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateQueueFleetAssociation": {
+        "SearchTasks": {
             "access_level": "Undocumented",
-            "action": "UpdateQueueFleetAssociation",
+            "action": "SearchTasks",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteMonitor": {
+        "CopyJobTemplate": {
             "access_level": "Undocumented",
-            "action": "DeleteMonitor",
+            "action": "CopyJobTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteBudget": {
+        "ListSessionActions": {
             "access_level": "Undocumented",
-            "action": "DeleteBudget",
+            "action": "ListSessionActions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SearchSteps": {
+        "ListStorageProfiles": {
             "access_level": "Undocumented",
-            "action": "SearchSteps",
+            "action": "ListStorageProfiles",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteQueueFleetAssociation": {
+        "ListSteps": {
             "access_level": "Undocumented",
-            "action": "DeleteQueueFleetAssociation",
+            "action": "ListSteps",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "GetQueueEnvironment": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "GetQueueEnvironment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "BatchGetJobEntity": {
+        "ListStepDependencies": {
             "access_level": "Undocumented",
-            "action": "BatchGetJobEntity",
+            "action": "ListStepDependencies",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateStorageProfile": {
+        "DeleteStorageProfile": {
             "access_level": "Undocumented",
-            "action": "CreateStorageProfile",
+            "action": "DeleteStorageProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSessionActions": {
+        "DisassociateMemberFromJob": {
             "access_level": "Undocumented",
-            "action": "ListSessionActions",
+            "action": "DisassociateMemberFromJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetQueueFleetAssociation": {
+        "CreateJob": {
             "access_level": "Undocumented",
-            "action": "GetQueueFleetAssociation",
+            "action": "CreateJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetFleet": {
+        "ListSessionsForWorker": {
             "access_level": "Undocumented",
-            "action": "GetFleet",
+            "action": "ListSessionsForWorker",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SearchTasks": {
+        "ListAvailableMeteredProducts": {
             "access_level": "Undocumented",
-            "action": "SearchTasks",
+            "action": "ListAvailableMeteredProducts",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetApplicationVersion": {
+        "ListStepConsumers": {
             "access_level": "Undocumented",
-            "action": "GetApplicationVersion",
+            "action": "ListStepConsumers",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListStepDependencies": {
+        "GetMonitor": {
             "access_level": "Undocumented",
-            "action": "ListStepDependencies",
+            "action": "GetMonitor",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetStorageProfileForQueue": {
+        "UpdateQueue": {
             "access_level": "Undocumented",
-            "action": "GetStorageProfileForQueue",
+            "action": "UpdateQueue",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssumeQueueRoleForUser": {
+        "UpdateStep": {
             "access_level": "Undocumented",
-            "action": "AssumeQueueRoleForUser",
+            "action": "UpdateStep",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateSession": {
+        "CreateWorker": {
             "access_level": "Undocumented",
-            "action": "UpdateSession",
+            "action": "CreateWorker",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssociateMemberToFarm": {
+        "ListTasks": {
             "access_level": "Undocumented",
-            "action": "AssociateMemberToFarm",
+            "action": "ListTasks",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateQueueFleetAssociation": {
+        "AssociateMemberToFleet": {
             "access_level": "Undocumented",
-            "action": "CreateQueueFleetAssociation",
+            "action": "AssociateMemberToFleet",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteQueueEnvironment": {
+        "ListJobMembers": {
             "access_level": "Undocumented",
-            "action": "DeleteQueueEnvironment",
+            "action": "ListJobMembers",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteWorker": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "DeleteWorker",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListJobs": {
+        "DeleteMonitor": {
             "access_level": "Undocumented",
-            "action": "ListJobs",
+            "action": "DeleteMonitor",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetMonitor": {
+        "ListFleetMembers": {
             "access_level": "Undocumented",
-            "action": "GetMonitor",
+            "action": "ListFleetMembers",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateWorker": {
+        "DeleteFleet": {
             "access_level": "Undocumented",
-            "action": "UpdateWorker",
+            "action": "DeleteFleet",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListFleets": {
+        "DeleteMeteredProduct": {
             "access_level": "Undocumented",
-            "action": "ListFleets",
+            "action": "DeleteMeteredProduct",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListJobMembers": {
+        "DisassociateMemberFromFleet": {
             "access_level": "Undocumented",
-            "action": "ListJobMembers",
+            "action": "DisassociateMemberFromFleet",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListFleetMembers": {
+        "GetFarm": {
             "access_level": "Undocumented",
-            "action": "ListFleetMembers",
+            "action": "GetFarm",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetWorker": {
+        "CreateFleet": {
             "access_level": "Undocumented",
-            "action": "GetWorker",
+            "action": "CreateFleet",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateStep": {
+        "CreateStorageProfile": {
             "access_level": "Undocumented",
-            "action": "UpdateStep",
+            "action": "CreateStorageProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateJob": {
+        "AssumeQueueRoleForRead": {
             "access_level": "Undocumented",
-            "action": "CreateJob",
+            "action": "AssumeQueueRoleForRead",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateBudget": {
+        "CreateQueueFleetAssociation": {
             "access_level": "Undocumented",
-            "action": "UpdateBudget",
+            "action": "CreateQueueFleetAssociation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteMeteredProduct": {
+        "AssociateMemberToFarm": {
             "access_level": "Undocumented",
-            "action": "DeleteMeteredProduct",
+            "action": "AssociateMemberToFarm",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetJob": {
+        "ListQueueFleetAssociations": {
             "access_level": "Undocumented",
-            "action": "GetJob",
+            "action": "ListQueueFleetAssociations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "GetStorageProfile": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "GetStorageProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListLicenseEndpoints": {
+        "UpdateJob": {
             "access_level": "Undocumented",
-            "action": "ListLicenseEndpoints",
+            "action": "UpdateJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateTask": {
+        "DeleteQueueEnvironment": {
             "access_level": "Undocumented",
-            "action": "UpdateTask",
+            "action": "DeleteQueueEnvironment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSteps": {
+        "DeleteFarm": {
             "access_level": "Undocumented",
-            "action": "ListSteps",
+            "action": "DeleteFarm",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteLicenseEndpoint": {
+        "ListJobs": {
             "access_level": "Undocumented",
-            "action": "DeleteLicenseEndpoint",
+            "action": "ListJobs",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateQueueEnvironment": {
+        "ListLicenseEndpoints": {
             "access_level": "Undocumented",
-            "action": "CreateQueueEnvironment",
+            "action": "ListLicenseEndpoints",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteFleet": {
+        "UpdateFarm": {
             "access_level": "Undocumented",
-            "action": "DeleteFleet",
+            "action": "UpdateFarm",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssumeQueueRoleForRead": {
+        "UpdateBudget": {
             "access_level": "Undocumented",
-            "action": "AssumeQueueRoleForRead",
+            "action": "UpdateBudget",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssociateMemberToFleet": {
+        "ListBudgets": {
             "access_level": "Undocumented",
-            "action": "AssociateMemberToFleet",
+            "action": "ListBudgets",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateBudget": {
+        "ListMonitors": {
             "access_level": "Undocumented",
-            "action": "CreateBudget",
+            "action": "ListMonitors",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetBudget": {
+        "GetApplicationVersion": {
             "access_level": "Undocumented",
-            "action": "GetBudget",
+            "action": "GetApplicationVersion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetStorageProfile": {
+        "UpdateMonitor": {
             "access_level": "Undocumented",
-            "action": "GetStorageProfile",
+            "action": "UpdateMonitor",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "GetBudget": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "GetBudget",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetQueue": {
+        "CreateQueueEnvironment": {
             "access_level": "Undocumented",
-            "action": "GetQueue",
+            "action": "CreateQueueEnvironment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetStep": {
+        "UpdateTask": {
             "access_level": "Undocumented",
-            "action": "GetStep",
+            "action": "UpdateTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateLicenseEndpoint": {
+        "AssumeFleetRoleForRead": {
             "access_level": "Undocumented",
-            "action": "CreateLicenseEndpoint",
+            "action": "AssumeFleetRoleForRead",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListMonitors": {
+        "GetQueueFleetAssociation": {
             "access_level": "Undocumented",
-            "action": "ListMonitors",
+            "action": "GetQueueFleetAssociation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListFarmMembers": {
+        "GetSessionsStatisticsAggregation": {
             "access_level": "Undocumented",
-            "action": "ListFarmMembers",
+            "action": "GetSessionsStatisticsAggregation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateMonitor": {
+        "UpdateQueueFleetAssociation": {
             "access_level": "Undocumented",
-            "action": "CreateMonitor",
+            "action": "UpdateQueueFleetAssociation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DisassociateMemberFromQueue": {
+        "DeleteQueue": {
             "access_level": "Undocumented",
-            "action": "DisassociateMemberFromQueue",
+            "action": "DeleteQueue",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateFarm": {
+        "GetSession": {
             "access_level": "Undocumented",
-            "action": "CreateFarm",
+            "action": "GetSession",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListStepConsumers": {
+        "ListFleets": {
             "access_level": "Undocumented",
-            "action": "ListStepConsumers",
+            "action": "ListFleets",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateQueue": {
+        "ListFarmMembers": {
             "access_level": "Undocumented",
-            "action": "UpdateQueue",
+            "action": "ListFarmMembers",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssociateMemberToJob": {
+        "GetFleet": {
             "access_level": "Undocumented",
-            "action": "AssociateMemberToJob",
+            "action": "GetFleet",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "deepcomposer": {
@@ -64715,305 +64715,305 @@
             ],
             "description": "Grants permission to replace the current set of policies for the specified load balancer port with the specified set of policies",
             "orphan": false,
             "resources": [
                 "loadbalancer"
             ]
         },
-        "AddTrustStoreRevocations": {
+        "SetWebAcl": {
             "access_level": "Undocumented",
-            "action": "AddTrustStoreRevocations",
+            "action": "SetWebAcl",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RemoveListenerCertificates": {
+        "SetIpAddressType": {
             "access_level": "Undocumented",
-            "action": "RemoveListenerCertificates",
+            "action": "SetIpAddressType",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetTrustStoreRevocationContent": {
+        "DescribeTargetGroups": {
             "access_level": "Undocumented",
-            "action": "GetTrustStoreRevocationContent",
+            "action": "DescribeTargetGroups",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeTargetGroups": {
+        "ModifyRule": {
             "access_level": "Undocumented",
-            "action": "DescribeTargetGroups",
+            "action": "ModifyRule",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeTrustStoreAssociations": {
+        "CreateTrustStore": {
             "access_level": "Undocumented",
-            "action": "DescribeTrustStoreAssociations",
+            "action": "CreateTrustStore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeTrustStores": {
+        "AddListenerCertificates": {
             "access_level": "Undocumented",
-            "action": "DescribeTrustStores",
+            "action": "AddListenerCertificates",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ModifyListener": {
+        "GetTrustStoreRevocationContent": {
             "access_level": "Undocumented",
-            "action": "ModifyListener",
+            "action": "GetTrustStoreRevocationContent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeListenerCertificates": {
+        "RemoveListenerCertificates": {
             "access_level": "Undocumented",
-            "action": "DescribeListenerCertificates",
+            "action": "RemoveListenerCertificates",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RegisterTargets": {
+        "DeregisterTargets": {
             "access_level": "Undocumented",
-            "action": "RegisterTargets",
+            "action": "DeregisterTargets",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateRule": {
+        "DescribeTrustStoreRevocations": {
             "access_level": "Undocumented",
-            "action": "CreateRule",
+            "action": "DescribeTrustStoreRevocations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateTrustStore": {
+        "CreateListener": {
             "access_level": "Undocumented",
-            "action": "CreateTrustStore",
+            "action": "CreateListener",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AddListenerCertificates": {
+        "CreateRule": {
             "access_level": "Undocumented",
-            "action": "AddListenerCertificates",
+            "action": "CreateRule",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateTargetGroup": {
+        "DeleteRule": {
             "access_level": "Undocumented",
-            "action": "CreateTargetGroup",
+            "action": "DeleteRule",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteTrustStore": {
+        "SetRulePriorities": {
             "access_level": "Undocumented",
-            "action": "DeleteTrustStore",
+            "action": "SetRulePriorities",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteTargetGroup": {
+        "DescribeSSLPolicies": {
             "access_level": "Undocumented",
-            "action": "DeleteTargetGroup",
+            "action": "DescribeSSLPolicies",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeregisterTargets": {
+        "DeleteListener": {
             "access_level": "Undocumented",
-            "action": "DeregisterTargets",
+            "action": "DeleteListener",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeTargetHealth": {
+        "DeleteTargetGroup": {
             "access_level": "Undocumented",
-            "action": "DescribeTargetHealth",
+            "action": "DeleteTargetGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ModifyTargetGroup": {
+        "DescribeTrustStoreAssociations": {
             "access_level": "Undocumented",
-            "action": "ModifyTargetGroup",
+            "action": "DescribeTrustStoreAssociations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SetWebAcl": {
+        "AddTrustStoreRevocations": {
             "access_level": "Undocumented",
-            "action": "SetWebAcl",
+            "action": "AddTrustStoreRevocations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SetSecurityGroups": {
+        "DescribeTargetHealth": {
             "access_level": "Undocumented",
-            "action": "SetSecurityGroups",
+            "action": "DescribeTargetHealth",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateListener": {
+        "ModifyTargetGroupAttributes": {
             "access_level": "Undocumented",
-            "action": "CreateListener",
+            "action": "ModifyTargetGroupAttributes",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteListener": {
+        "DescribeAccountLimits": {
             "access_level": "Undocumented",
-            "action": "DeleteListener",
+            "action": "DescribeAccountLimits",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ModifyRule": {
+        "DescribeTrustStores": {
             "access_level": "Undocumented",
-            "action": "ModifyRule",
+            "action": "DescribeTrustStores",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SetRulePriorities": {
+        "ModifyListener": {
             "access_level": "Undocumented",
-            "action": "SetRulePriorities",
+            "action": "ModifyListener",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeListeners": {
+        "ModifyTargetGroup": {
             "access_level": "Undocumented",
-            "action": "DescribeListeners",
+            "action": "ModifyTargetGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DescribeTargetGroupAttributes": {
             "access_level": "Undocumented",
             "action": "DescribeTargetGroupAttributes",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RemoveTrustStoreRevocations": {
+        "DeleteTrustStore": {
             "access_level": "Undocumented",
-            "action": "RemoveTrustStoreRevocations",
+            "action": "DeleteTrustStore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeAccountLimits": {
+        "CreateTargetGroup": {
             "access_level": "Undocumented",
-            "action": "DescribeAccountLimits",
+            "action": "CreateTargetGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteRule": {
+        "SetSecurityGroups": {
             "access_level": "Undocumented",
-            "action": "DeleteRule",
+            "action": "SetSecurityGroups",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeSSLPolicies": {
+        "RemoveTrustStoreRevocations": {
             "access_level": "Undocumented",
-            "action": "DescribeSSLPolicies",
+            "action": "RemoveTrustStoreRevocations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeTrustStoreRevocations": {
+        "DescribeListenerCertificates": {
             "access_level": "Undocumented",
-            "action": "DescribeTrustStoreRevocations",
+            "action": "DescribeListenerCertificates",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ModifyTargetGroupAttributes": {
+        "SetSubnets": {
             "access_level": "Undocumented",
-            "action": "ModifyTargetGroupAttributes",
+            "action": "SetSubnets",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetTrustStoreCaCertificatesBundle": {
+        "DescribeRules": {
             "access_level": "Undocumented",
-            "action": "GetTrustStoreCaCertificatesBundle",
+            "action": "DescribeRules",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeRules": {
+        "GetTrustStoreCaCertificatesBundle": {
             "access_level": "Undocumented",
-            "action": "DescribeRules",
+            "action": "GetTrustStoreCaCertificatesBundle",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SetIpAddressType": {
+        "RegisterTargets": {
             "access_level": "Undocumented",
-            "action": "SetIpAddressType",
+            "action": "RegisterTargets",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SetSubnets": {
+        "ModifyTrustStore": {
             "access_level": "Undocumented",
-            "action": "SetSubnets",
+            "action": "ModifyTrustStore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ModifyTrustStore": {
+        "DescribeListeners": {
             "access_level": "Undocumented",
-            "action": "ModifyTrustStore",
+            "action": "DescribeListeners",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "elasticmapreduce": {
@@ -66685,305 +66685,305 @@
             "orphan": false,
             "resources": [
                 "application"
             ]
         }
     },
     "entityresolution": {
-        "GetMatchId": {
+        "GetPolicy": {
             "access_level": "Undocumented",
-            "action": "GetMatchId",
+            "action": "GetPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListProviderServices": {
+        "UseIdNamespace": {
             "access_level": "Undocumented",
-            "action": "ListProviderServices",
+            "action": "UseIdNamespace",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSchemaMapping": {
+        "GetIdMappingJob": {
             "access_level": "Undocumented",
-            "action": "GetSchemaMapping",
+            "action": "GetIdMappingJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListIdMappingWorkflows": {
+        "ListIdNamespaces": {
             "access_level": "Undocumented",
-            "action": "ListIdMappingWorkflows",
+            "action": "ListIdNamespaces",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteSchemaMapping": {
+        "GetMatchingWorkflow": {
             "access_level": "Undocumented",
-            "action": "DeleteSchemaMapping",
+            "action": "GetMatchingWorkflow",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateSchemaMapping": {
+        "UpdateMatchingWorkflow": {
             "access_level": "Undocumented",
-            "action": "UpdateSchemaMapping",
+            "action": "UpdateMatchingWorkflow",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutPolicy": {
+        "AddPolicyStatement": {
             "access_level": "Undocumented",
-            "action": "PutPolicy",
+            "action": "AddPolicyStatement",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartMatchingJob": {
+        "UpdateSchemaMapping": {
             "access_level": "Undocumented",
-            "action": "StartMatchingJob",
+            "action": "UpdateSchemaMapping",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateMatchingWorkflow": {
+        "DeleteSchemaMapping": {
             "access_level": "Undocumented",
-            "action": "CreateMatchingWorkflow",
+            "action": "DeleteSchemaMapping",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetIdMappingWorkflow": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "GetIdMappingWorkflow",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "CreateSchemaMapping": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "CreateSchemaMapping",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListIdMappingJobs": {
+        "GetMatchingJob": {
             "access_level": "Undocumented",
-            "action": "ListIdMappingJobs",
+            "action": "GetMatchingJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteIdMappingWorkflow": {
+        "PutPolicy": {
             "access_level": "Undocumented",
-            "action": "DeleteIdMappingWorkflow",
+            "action": "PutPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateIdNamespace": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "CreateIdNamespace",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPolicy": {
+        "ListProviderServices": {
             "access_level": "Undocumented",
-            "action": "GetPolicy",
+            "action": "ListProviderServices",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateIdMappingWorkflow": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "UpdateIdMappingWorkflow",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartIdMappingJob": {
+        "CreateIdNamespace": {
             "access_level": "Undocumented",
-            "action": "StartIdMappingJob",
+            "action": "CreateIdNamespace",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetProviderService": {
+        "ListIdMappingWorkflows": {
             "access_level": "Undocumented",
-            "action": "GetProviderService",
+            "action": "ListIdMappingWorkflows",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateIdNamespace": {
+        "CreateIdMappingWorkflow": {
             "access_level": "Undocumented",
-            "action": "UpdateIdNamespace",
+            "action": "CreateIdMappingWorkflow",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetIdNamespace": {
+        "GetMatchId": {
             "access_level": "Undocumented",
-            "action": "GetIdNamespace",
+            "action": "GetMatchId",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeletePolicyStatement": {
+        "StartIdMappingJob": {
             "access_level": "Undocumented",
-            "action": "DeletePolicyStatement",
+            "action": "StartIdMappingJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListMatchingWorkflows": {
+        "DeleteIdMappingWorkflow": {
             "access_level": "Undocumented",
-            "action": "ListMatchingWorkflows",
+            "action": "DeleteIdMappingWorkflow",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "GetIdMappingWorkflow": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "GetIdMappingWorkflow",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UseIdNamespace": {
+        "ListIdMappingJobs": {
             "access_level": "Undocumented",
-            "action": "UseIdNamespace",
+            "action": "ListIdMappingJobs",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetIdMappingJob": {
+        "CreateMatchingWorkflow": {
             "access_level": "Undocumented",
-            "action": "GetIdMappingJob",
+            "action": "CreateMatchingWorkflow",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteMatchingWorkflow": {
+        "ListMatchingJobs": {
             "access_level": "Undocumented",
-            "action": "DeleteMatchingWorkflow",
+            "action": "ListMatchingJobs",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListMatchingJobs": {
+        "UpdateIdNamespace": {
             "access_level": "Undocumented",
-            "action": "ListMatchingJobs",
+            "action": "UpdateIdNamespace",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AddPolicyStatement": {
+        "GetProviderService": {
             "access_level": "Undocumented",
-            "action": "AddPolicyStatement",
+            "action": "GetProviderService",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DeleteIdNamespace": {
             "access_level": "Undocumented",
             "action": "DeleteIdNamespace",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateMatchingWorkflow": {
+        "DeleteMatchingWorkflow": {
             "access_level": "Undocumented",
-            "action": "UpdateMatchingWorkflow",
+            "action": "DeleteMatchingWorkflow",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListIdNamespaces": {
+        "DeletePolicyStatement": {
             "access_level": "Undocumented",
-            "action": "ListIdNamespaces",
+            "action": "DeletePolicyStatement",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "ListSchemaMappings": {
             "access_level": "Undocumented",
             "action": "ListSchemaMappings",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "StartMatchingJob": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "StartMatchingJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetMatchingWorkflow": {
+        "GetIdNamespace": {
             "access_level": "Undocumented",
-            "action": "GetMatchingWorkflow",
+            "action": "GetIdNamespace",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateIdMappingWorkflow": {
+        "ListMatchingWorkflows": {
             "access_level": "Undocumented",
-            "action": "CreateIdMappingWorkflow",
+            "action": "ListMatchingWorkflows",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetMatchingJob": {
+        "GetSchemaMapping": {
             "access_level": "Undocumented",
-            "action": "GetMatchingJob",
+            "action": "GetSchemaMapping",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateSchemaMapping": {
+        "UpdateIdMappingWorkflow": {
             "access_level": "Undocumented",
-            "action": "CreateSchemaMapping",
+            "action": "UpdateIdMappingWorkflow",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "es": {
@@ -69701,225 +69701,225 @@
             "orphan": false,
             "resources": [
                 "deliverystream"
             ]
         }
     },
     "fis": {
-        "StartExperiment": {
+        "GetTargetAccountConfiguration": {
             "access_level": "Undocumented",
-            "action": "StartExperiment",
+            "action": "GetTargetAccountConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateTargetAccountConfiguration": {
+        "ListTargetResourceTypes": {
             "access_level": "Undocumented",
-            "action": "UpdateTargetAccountConfiguration",
+            "action": "ListTargetResourceTypes",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAction": {
+        "ListExperiments": {
             "access_level": "Undocumented",
-            "action": "GetAction",
+            "action": "ListExperiments",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "InjectApiThrottleError": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "InjectApiThrottleError",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetExperimentTemplate": {
+        "ListActions": {
             "access_level": "Undocumented",
-            "action": "GetExperimentTemplate",
+            "action": "ListActions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTargetResourceTypes": {
+        "DeleteTargetAccountConfiguration": {
             "access_level": "Undocumented",
-            "action": "ListTargetResourceTypes",
+            "action": "DeleteTargetAccountConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "InjectApiInternalError": {
+        "CreateTargetAccountConfiguration": {
             "access_level": "Undocumented",
-            "action": "InjectApiInternalError",
+            "action": "CreateTargetAccountConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListExperimentTargetAccountConfigurations": {
+        "InjectApiInternalError": {
             "access_level": "Undocumented",
-            "action": "ListExperimentTargetAccountConfigurations",
+            "action": "InjectApiInternalError",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "InjectApiUnavailableError": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "InjectApiUnavailableError",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTargetAccountConfigurations": {
+        "UpdateTargetAccountConfiguration": {
             "access_level": "Undocumented",
-            "action": "ListTargetAccountConfigurations",
+            "action": "UpdateTargetAccountConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "ListExperimentResolvedTargets": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "ListExperimentResolvedTargets",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetExperimentTargetAccountConfiguration": {
+        "GetExperimentTemplate": {
             "access_level": "Undocumented",
-            "action": "GetExperimentTargetAccountConfiguration",
+            "action": "GetExperimentTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListActions": {
+        "GetAction": {
             "access_level": "Undocumented",
-            "action": "ListActions",
+            "action": "GetAction",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListExperimentResolvedTargets": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "ListExperimentResolvedTargets",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListExperimentTemplates": {
+        "InjectApiUnavailableError": {
             "access_level": "Undocumented",
-            "action": "ListExperimentTemplates",
+            "action": "InjectApiUnavailableError",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DeleteExperimentTemplate": {
             "access_level": "Undocumented",
             "action": "DeleteExperimentTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetExperiment": {
+        "ListTargetAccountConfigurations": {
             "access_level": "Undocumented",
-            "action": "GetExperiment",
+            "action": "ListTargetAccountConfigurations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetTargetResourceType": {
+        "StopExperiment": {
             "access_level": "Undocumented",
-            "action": "GetTargetResourceType",
+            "action": "StopExperiment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateTargetAccountConfiguration": {
+        "ListExperimentTargetAccountConfigurations": {
             "access_level": "Undocumented",
-            "action": "CreateTargetAccountConfiguration",
+            "action": "ListExperimentTargetAccountConfigurations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateExperimentTemplate": {
+        "GetExperiment": {
             "access_level": "Undocumented",
-            "action": "CreateExperimentTemplate",
+            "action": "GetExperiment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateExperimentTemplate": {
+        "CreateExperimentTemplate": {
             "access_level": "Undocumented",
-            "action": "UpdateExperimentTemplate",
+            "action": "CreateExperimentTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteTargetAccountConfiguration": {
+        "GetExperimentTargetAccountConfiguration": {
             "access_level": "Undocumented",
-            "action": "DeleteTargetAccountConfiguration",
+            "action": "GetExperimentTargetAccountConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetTargetAccountConfiguration": {
+        "GetTargetResourceType": {
             "access_level": "Undocumented",
-            "action": "GetTargetAccountConfiguration",
+            "action": "GetTargetResourceType",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "InjectApiThrottleError": {
+        "StartExperiment": {
             "access_level": "Undocumented",
-            "action": "InjectApiThrottleError",
+            "action": "StartExperiment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListExperiments": {
+        "ListExperimentTemplates": {
             "access_level": "Undocumented",
-            "action": "ListExperiments",
+            "action": "ListExperimentTemplates",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StopExperiment": {
+        "UpdateExperimentTemplate": {
             "access_level": "Undocumented",
-            "action": "StopExperiment",
+            "action": "UpdateExperimentTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "fms": {
@@ -72158,33 +72158,33 @@
             "condition_keys": [],
             "description": "Grants permission to verify the email for FreeRTOS extended maintenance plan (EMP)",
             "orphan": false,
             "resources": []
         }
     },
     "freetier": {
-        "PutFreeTierAlertPreference": {
+        "GetFreeTierAlertPreference": {
             "access_level": "Undocumented",
-            "action": "PutFreeTierAlertPreference",
+            "action": "GetFreeTierAlertPreference",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetFreeTierUsage": {
+        "PutFreeTierAlertPreference": {
             "access_level": "Undocumented",
-            "action": "GetFreeTierUsage",
+            "action": "PutFreeTierAlertPreference",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetFreeTierAlertPreference": {
+        "GetFreeTierUsage": {
             "access_level": "Undocumented",
-            "action": "GetFreeTierAlertPreference",
+            "action": "GetFreeTierUsage",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "fsx": {
@@ -80206,169 +80206,169 @@
             "condition_keys": [],
             "description": "Grants permission to enable the Organizational View feature",
             "orphan": false,
             "resources": []
         }
     },
     "healthlake": {
-        "ListFHIRExportJobs": {
+        "CreateFHIRDatastore": {
             "access_level": "Undocumented",
-            "action": "ListFHIRExportJobs",
+            "action": "CreateFHIRDatastore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SearchWithGet": {
+        "ListFHIRDatastores": {
             "access_level": "Undocumented",
-            "action": "SearchWithGet",
+            "action": "ListFHIRDatastores",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListFHIRDatastores": {
+        "StartFHIRExportJob": {
             "access_level": "Undocumented",
-            "action": "ListFHIRDatastores",
+            "action": "StartFHIRExportJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "UpdateResource": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "UpdateResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartFHIRImportJob": {
+        "GetCapabilities": {
             "access_level": "Undocumented",
-            "action": "StartFHIRImportJob",
+            "action": "GetCapabilities",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateResource": {
+        "DeleteFHIRDatastore": {
             "access_level": "Undocumented",
-            "action": "CreateResource",
+            "action": "DeleteFHIRDatastore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "ReadResource": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "ReadResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SearchWithPost": {
+        "DescribeFHIRExportJob": {
             "access_level": "Undocumented",
-            "action": "SearchWithPost",
+            "action": "DescribeFHIRExportJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeFHIRExportJob": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "DescribeFHIRExportJob",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DescribeFHIRImportJob": {
             "access_level": "Undocumented",
             "action": "DescribeFHIRImportJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "ListFHIRExportJobs": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "ListFHIRExportJobs",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteResource": {
+        "ListFHIRImportJobs": {
             "access_level": "Undocumented",
-            "action": "DeleteResource",
+            "action": "ListFHIRImportJobs",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartFHIRExportJob": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "StartFHIRExportJob",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateFHIRDatastore": {
+        "CreateResource": {
             "access_level": "Undocumented",
-            "action": "CreateFHIRDatastore",
+            "action": "CreateResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListFHIRImportJobs": {
+        "SearchWithGet": {
             "access_level": "Undocumented",
-            "action": "ListFHIRImportJobs",
+            "action": "SearchWithGet",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ReadResource": {
+        "SearchWithPost": {
             "access_level": "Undocumented",
-            "action": "ReadResource",
+            "action": "SearchWithPost",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateResource": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "UpdateResource",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteFHIRDatastore": {
+        "DeleteResource": {
             "access_level": "Undocumented",
-            "action": "DeleteFHIRDatastore",
+            "action": "DeleteResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DescribeFHIRDatastore": {
             "access_level": "Undocumented",
             "action": "DescribeFHIRDatastore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetCapabilities": {
+        "StartFHIRImportJob": {
             "access_level": "Undocumented",
-            "action": "GetCapabilities",
+            "action": "StartFHIRImportJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "honeycode": {
@@ -80634,1377 +80634,1377 @@
             "condition_keys": [],
             "description": "Grants permission to update an Amazon Honeycode team for your AWS Account",
             "orphan": false,
             "resources": []
         }
     },
     "iam": {
-        "CreateLoginProfile": {
+        "GetServiceLastAccessedDetailsWithEntities": {
             "access_level": "Undocumented",
-            "action": "CreateLoginProfile",
+            "action": "GetServiceLastAccessedDetailsWithEntities",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPoliciesGrantingServiceAccess": {
+        "UpdateAccountPasswordPolicy": {
             "access_level": "Undocumented",
-            "action": "ListPoliciesGrantingServiceAccess",
+            "action": "UpdateAccountPasswordPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateVirtualMFADevice": {
+        "UploadCloudFrontPublicKey": {
             "access_level": "Undocumented",
-            "action": "CreateVirtualMFADevice",
+            "action": "UploadCloudFrontPublicKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListEntitiesForPolicy": {
+        "UpdateAccountEmailAddress": {
             "access_level": "Undocumented",
-            "action": "ListEntitiesForPolicy",
+            "action": "UpdateAccountEmailAddress",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagUser": {
+        "TagPolicy": {
             "access_level": "Undocumented",
-            "action": "TagUser",
+            "action": "TagPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListGroups": {
+        "DeleteRolePolicy": {
             "access_level": "Undocumented",
-            "action": "ListGroups",
+            "action": "DeleteRolePolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SimulateCustomPolicy": {
+        "UpdateRoleDescription": {
             "access_level": "Undocumented",
-            "action": "SimulateCustomPolicy",
+            "action": "UpdateRoleDescription",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetContextKeysForPrincipalPolicy": {
+        "GetAccountSummary": {
             "access_level": "Undocumented",
-            "action": "GetContextKeysForPrincipalPolicy",
+            "action": "GetAccountSummary",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeactivateMFADevice": {
+        "DeleteGroupPolicy": {
             "access_level": "Undocumented",
-            "action": "DeactivateMFADevice",
+            "action": "DeleteGroupPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UploadSSHPublicKey": {
+        "GenerateServiceLastAccessedDetails": {
             "access_level": "Undocumented",
-            "action": "UploadSSHPublicKey",
+            "action": "GenerateServiceLastAccessedDetails",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSAMLProvider": {
+        "UntagInstanceProfile": {
             "access_level": "Undocumented",
-            "action": "GetSAMLProvider",
+            "action": "UntagInstanceProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetCredentialReport": {
+        "DeleteUser": {
             "access_level": "Undocumented",
-            "action": "GetCredentialReport",
+            "action": "DeleteUser",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteRolePermissionsBoundary": {
+        "GetAccountAuthorizationDetails": {
             "access_level": "Undocumented",
-            "action": "DeleteRolePermissionsBoundary",
+            "action": "GetAccountAuthorizationDetails",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteSAMLProvider": {
+        "AddUserToGroup": {
             "access_level": "Undocumented",
-            "action": "DeleteSAMLProvider",
+            "action": "AddUserToGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateSAMLProvider": {
+        "DeleteOpenIDConnectProvider": {
             "access_level": "Undocumented",
-            "action": "UpdateSAMLProvider",
+            "action": "DeleteOpenIDConnectProvider",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SimulatePrincipalPolicy": {
+        "GetMFADevice": {
             "access_level": "Undocumented",
-            "action": "SimulatePrincipalPolicy",
+            "action": "GetMFADevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListGroupsForUser": {
+        "ListInstanceProfilesForRole": {
             "access_level": "Undocumented",
-            "action": "ListGroupsForUser",
+            "action": "ListInstanceProfilesForRole",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetCloudFrontPublicKey": {
+        "CreateGroup": {
             "access_level": "Undocumented",
-            "action": "GetCloudFrontPublicKey",
+            "action": "CreateGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteUser": {
+        "ListPolicyTags": {
             "access_level": "Undocumented",
-            "action": "DeleteUser",
+            "action": "ListPolicyTags",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutUserPolicy": {
+        "CreateAccessKey": {
             "access_level": "Undocumented",
-            "action": "PutUserPolicy",
+            "action": "CreateAccessKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteLoginProfile": {
+        "DeleteInstanceProfile": {
             "access_level": "Undocumented",
-            "action": "DeleteLoginProfile",
+            "action": "DeleteInstanceProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListRoleTags": {
+        "GetSAMLProvider": {
             "access_level": "Undocumented",
-            "action": "ListRoleTags",
+            "action": "GetSAMLProvider",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateServiceLinkedRole": {
+        "DeletePolicy": {
             "access_level": "Undocumented",
-            "action": "CreateServiceLinkedRole",
+            "action": "DeletePolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetOrganizationsAccessReport": {
+        "DetachUserPolicy": {
             "access_level": "Undocumented",
-            "action": "GetOrganizationsAccessReport",
+            "action": "DetachUserPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateSSHPublicKey": {
+        "DeleteAccessKey": {
             "access_level": "Undocumented",
-            "action": "UpdateSSHPublicKey",
+            "action": "DeleteAccessKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DetachRolePolicy": {
+        "GetAccountEmailAddress": {
             "access_level": "Undocumented",
-            "action": "DetachRolePolicy",
+            "action": "GetAccountEmailAddress",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAccountAliases": {
+        "ListAccessKeys": {
             "access_level": "Undocumented",
-            "action": "ListAccountAliases",
+            "action": "ListAccessKeys",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateGroup": {
+        "ListServerCertificates": {
             "access_level": "Undocumented",
-            "action": "CreateGroup",
+            "action": "ListServerCertificates",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAccountName": {
+        "CreatePolicy": {
             "access_level": "Undocumented",
-            "action": "GetAccountName",
+            "action": "CreatePolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSSHPublicKey": {
+        "UpdateAccountName": {
             "access_level": "Undocumented",
-            "action": "GetSSHPublicKey",
+            "action": "UpdateAccountName",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagSAMLProvider": {
+        "ListInstanceProfiles": {
             "access_level": "Undocumented",
-            "action": "UntagSAMLProvider",
+            "action": "ListInstanceProfiles",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UploadCloudFrontPublicKey": {
+        "GetSSHPublicKey": {
             "access_level": "Undocumented",
-            "action": "UploadCloudFrontPublicKey",
+            "action": "GetSSHPublicKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AddUserToGroup": {
+        "ListRolePolicies": {
             "access_level": "Undocumented",
-            "action": "AddUserToGroup",
+            "action": "ListRolePolicies",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListServiceSpecificCredentials": {
+        "ListEntitiesForPolicy": {
             "access_level": "Undocumented",
-            "action": "ListServiceSpecificCredentials",
+            "action": "ListEntitiesForPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListUsers": {
+        "AddClientIDToOpenIDConnectProvider": {
             "access_level": "Undocumented",
-            "action": "ListUsers",
+            "action": "AddClientIDToOpenIDConnectProvider",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteAccountPasswordPolicy": {
+        "GetAccessKeyLastUsed": {
             "access_level": "Undocumented",
-            "action": "DeleteAccountPasswordPolicy",
+            "action": "GetAccessKeyLastUsed",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteInstanceProfile": {
+        "TagUser": {
             "access_level": "Undocumented",
-            "action": "DeleteInstanceProfile",
+            "action": "TagUser",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAccountPasswordPolicy": {
+        "GetContextKeysForPrincipalPolicy": {
             "access_level": "Undocumented",
-            "action": "GetAccountPasswordPolicy",
+            "action": "GetContextKeysForPrincipalPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAccessKeys": {
+        "GetOpenIDConnectProvider": {
             "access_level": "Undocumented",
-            "action": "ListAccessKeys",
+            "action": "GetOpenIDConnectProvider",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RemoveRoleFromInstanceProfile": {
+        "DetachRolePolicy": {
             "access_level": "Undocumented",
-            "action": "RemoveRoleFromInstanceProfile",
+            "action": "DetachRolePolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListServerCertificates": {
+        "EnableMFADevice": {
             "access_level": "Undocumented",
-            "action": "ListServerCertificates",
+            "action": "EnableMFADevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeletePolicyVersion": {
+        "DeleteUserPolicy": {
             "access_level": "Undocumented",
-            "action": "DeletePolicyVersion",
+            "action": "DeleteUserPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetServiceLastAccessedDetails": {
+        "UntagMFADevice": {
             "access_level": "Undocumented",
-            "action": "GetServiceLastAccessedDetails",
+            "action": "UntagMFADevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagRole": {
+        "GetServerCertificate": {
             "access_level": "Undocumented",
-            "action": "UntagRole",
+            "action": "GetServerCertificate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateAccountPasswordPolicy": {
+        "ListMFADevices": {
             "access_level": "Undocumented",
-            "action": "UpdateAccountPasswordPolicy",
+            "action": "ListMFADevices",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateServiceSpecificCredential": {
+        "DeleteAccountPasswordPolicy": {
             "access_level": "Undocumented",
-            "action": "UpdateServiceSpecificCredential",
+            "action": "DeleteAccountPasswordPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AddClientIDToOpenIDConnectProvider": {
+        "ListSSHPublicKeys": {
             "access_level": "Undocumented",
-            "action": "AddClientIDToOpenIDConnectProvider",
+            "action": "ListSSHPublicKeys",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateRoleDescription": {
+        "ListRoleTags": {
             "access_level": "Undocumented",
-            "action": "UpdateRoleDescription",
+            "action": "ListRoleTags",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagServerCertificate": {
+        "ListSAMLProviderTags": {
             "access_level": "Undocumented",
-            "action": "TagServerCertificate",
+            "action": "ListSAMLProviderTags",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListInstanceProfileTags": {
+        "UpdateOpenIDConnectProviderThumbprint": {
             "access_level": "Undocumented",
-            "action": "ListInstanceProfileTags",
+            "action": "UpdateOpenIDConnectProviderThumbprint",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateInstanceProfile": {
+        "PassRole": {
             "access_level": "Undocumented",
-            "action": "CreateInstanceProfile",
+            "action": "PassRole",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagUser": {
+        "GetContextKeysForCustomPolicy": {
             "access_level": "Undocumented",
-            "action": "UntagUser",
+            "action": "GetContextKeysForCustomPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListVirtualMFADevices": {
+        "ListSAMLProviders": {
             "access_level": "Undocumented",
-            "action": "ListVirtualMFADevices",
+            "action": "ListSAMLProviders",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AttachGroupPolicy": {
+        "ListAccountAliases": {
             "access_level": "Undocumented",
-            "action": "AttachGroupPolicy",
+            "action": "ListAccountAliases",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagRole": {
+        "ListOpenIDConnectProviders": {
             "access_level": "Undocumented",
-            "action": "TagRole",
+            "action": "ListOpenIDConnectProviders",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteSSHPublicKey": {
+        "ListUserTags": {
             "access_level": "Undocumented",
-            "action": "DeleteSSHPublicKey",
+            "action": "ListUserTags",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetServerCertificate": {
+        "AttachUserPolicy": {
             "access_level": "Undocumented",
-            "action": "GetServerCertificate",
+            "action": "AttachUserPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RemoveClientIDFromOpenIDConnectProvider": {
+        "CreateSAMLProvider": {
             "access_level": "Undocumented",
-            "action": "RemoveClientIDFromOpenIDConnectProvider",
+            "action": "CreateSAMLProvider",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GenerateCredentialReport": {
+        "AttachRolePolicy": {
             "access_level": "Undocumented",
-            "action": "GenerateCredentialReport",
+            "action": "AttachRolePolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetLoginProfile": {
+        "SetSecurityTokenServicePreferences": {
             "access_level": "Undocumented",
-            "action": "GetLoginProfile",
+            "action": "SetSecurityTokenServicePreferences",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateAccessKey": {
+        "GetCredentialReport": {
             "access_level": "Undocumented",
-            "action": "CreateAccessKey",
+            "action": "GetCredentialReport",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteUserPolicy": {
+        "ListPolicyVersions": {
             "access_level": "Undocumented",
-            "action": "DeleteUserPolicy",
+            "action": "ListPolicyVersions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteServiceLinkedRole": {
+        "PutUserPermissionsBoundary": {
             "access_level": "Undocumented",
-            "action": "DeleteServiceLinkedRole",
+            "action": "PutUserPermissionsBoundary",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteAccountAlias": {
+        "ListRoles": {
             "access_level": "Undocumented",
-            "action": "DeleteAccountAlias",
+            "action": "ListRoles",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAccessKeyLastUsed": {
+        "GetRole": {
             "access_level": "Undocumented",
-            "action": "GetAccessKeyLastUsed",
+            "action": "GetRole",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UploadServerCertificate": {
+        "TagMFADevice": {
             "access_level": "Undocumented",
-            "action": "UploadServerCertificate",
+            "action": "TagMFADevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetUserPolicy": {
+        "ListPoliciesGrantingServiceAccess": {
             "access_level": "Undocumented",
-            "action": "GetUserPolicy",
+            "action": "ListPoliciesGrantingServiceAccess",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPolicy": {
+        "UpdateAccessKey": {
             "access_level": "Undocumented",
-            "action": "GetPolicy",
+            "action": "UpdateAccessKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RemoveUserFromGroup": {
+        "SetSTSRegionalEndpointStatus": {
             "access_level": "Undocumented",
-            "action": "RemoveUserFromGroup",
+            "action": "SetSTSRegionalEndpointStatus",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSAMLProviders": {
+        "CreatePolicyVersion": {
             "access_level": "Undocumented",
-            "action": "ListSAMLProviders",
+            "action": "CreatePolicyVersion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ResyncMFADevice": {
+        "GetRolePolicy": {
             "access_level": "Undocumented",
-            "action": "ResyncMFADevice",
+            "action": "GetRolePolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagOpenIDConnectProvider": {
+        "DeleteLoginProfile": {
             "access_level": "Undocumented",
-            "action": "UntagOpenIDConnectProvider",
+            "action": "DeleteLoginProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSTSRegionalEndpointsStatus": {
+        "UploadSigningCertificate": {
             "access_level": "Undocumented",
-            "action": "ListSTSRegionalEndpointsStatus",
+            "action": "UploadSigningCertificate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListCloudFrontPublicKeys": {
+        "DeleteServerCertificate": {
             "access_level": "Undocumented",
-            "action": "ListCloudFrontPublicKeys",
+            "action": "DeleteServerCertificate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetRole": {
+        "CreateRole": {
             "access_level": "Undocumented",
-            "action": "GetRole",
+            "action": "CreateRole",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAccountSummary": {
+        "DeleteRole": {
             "access_level": "Undocumented",
-            "action": "GetAccountSummary",
+            "action": "DeleteRole",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AttachUserPolicy": {
+        "GetGroupPolicy": {
             "access_level": "Undocumented",
-            "action": "AttachUserPolicy",
+            "action": "GetGroupPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAttachedRolePolicies": {
+        "DeleteServiceSpecificCredential": {
             "access_level": "Undocumented",
-            "action": "ListAttachedRolePolicies",
+            "action": "DeleteServiceSpecificCredential",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetGroup": {
+        "DeleteSigningCertificate": {
             "access_level": "Undocumented",
-            "action": "GetGroup",
+            "action": "DeleteSigningCertificate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagServerCertificate": {
+        "UntagOpenIDConnectProvider": {
             "access_level": "Undocumented",
-            "action": "UntagServerCertificate",
+            "action": "UntagOpenIDConnectProvider",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPolicyVersion": {
+        "PutRolePolicy": {
             "access_level": "Undocumented",
-            "action": "GetPolicyVersion",
+            "action": "PutRolePolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateCloudFrontPublicKey": {
+        "PutGroupPolicy": {
             "access_level": "Undocumented",
-            "action": "UpdateCloudFrontPublicKey",
+            "action": "PutGroupPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DetachUserPolicy": {
+        "UpdateServerCertificate": {
             "access_level": "Undocumented",
-            "action": "DetachUserPolicy",
+            "action": "UpdateServerCertificate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetGroupPolicy": {
+        "CreateUser": {
             "access_level": "Undocumented",
-            "action": "GetGroupPolicy",
+            "action": "CreateUser",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListUserPolicies": {
+        "GetUserPolicy": {
             "access_level": "Undocumented",
-            "action": "ListUserPolicies",
+            "action": "GetUserPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetOpenIDConnectProvider": {
+        "GenerateCredentialReport": {
             "access_level": "Undocumented",
-            "action": "GetOpenIDConnectProvider",
+            "action": "GenerateCredentialReport",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateUser": {
+        "RemoveUserFromGroup": {
             "access_level": "Undocumented",
-            "action": "CreateUser",
+            "action": "RemoveUserFromGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteServiceSpecificCredential": {
+        "AttachGroupPolicy": {
             "access_level": "Undocumented",
-            "action": "DeleteServiceSpecificCredential",
+            "action": "AttachGroupPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SetSTSRegionalEndpointStatus": {
+        "DetachGroupPolicy": {
             "access_level": "Undocumented",
-            "action": "SetSTSRegionalEndpointStatus",
+            "action": "DetachGroupPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SetSecurityTokenServicePreferences": {
+        "UpdateSSHPublicKey": {
             "access_level": "Undocumented",
-            "action": "SetSecurityTokenServicePreferences",
+            "action": "UpdateSSHPublicKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UploadSigningCertificate": {
+        "UntagSAMLProvider": {
             "access_level": "Undocumented",
-            "action": "UploadSigningCertificate",
+            "action": "UntagSAMLProvider",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutUserPermissionsBoundary": {
+        "ListAttachedRolePolicies": {
             "access_level": "Undocumented",
-            "action": "PutUserPermissionsBoundary",
+            "action": "ListAttachedRolePolicies",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteAccessKey": {
+        "GetServiceLinkedRoleDeletionStatus": {
             "access_level": "Undocumented",
-            "action": "DeleteAccessKey",
+            "action": "GetServiceLinkedRoleDeletionStatus",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteUserPermissionsBoundary": {
+        "GetLoginProfile": {
             "access_level": "Undocumented",
-            "action": "DeleteUserPermissionsBoundary",
+            "action": "GetLoginProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListInstanceProfilesForRole": {
+        "UpdateServiceSpecificCredential": {
             "access_level": "Undocumented",
-            "action": "ListInstanceProfilesForRole",
+            "action": "UpdateServiceSpecificCredential",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateOpenIDConnectProvider": {
+        "ListInstanceProfileTags": {
             "access_level": "Undocumented",
-            "action": "CreateOpenIDConnectProvider",
+            "action": "ListInstanceProfileTags",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetServiceLinkedRoleDeletionStatus": {
+        "PutUserPolicy": {
             "access_level": "Undocumented",
-            "action": "GetServiceLinkedRoleDeletionStatus",
+            "action": "PutUserPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteRolePolicy": {
+        "SetDefaultPolicyVersion": {
             "access_level": "Undocumented",
-            "action": "DeleteRolePolicy",
+            "action": "SetDefaultPolicyVersion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreatePolicyVersion": {
+        "CreateLoginProfile": {
             "access_level": "Undocumented",
-            "action": "CreatePolicyVersion",
+            "action": "CreateLoginProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListRolePolicies": {
+        "DeleteSSHPublicKey": {
             "access_level": "Undocumented",
-            "action": "ListRolePolicies",
+            "action": "DeleteSSHPublicKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateAccountEmailAddress": {
+        "DeleteServiceLinkedRole": {
             "access_level": "Undocumented",
-            "action": "UpdateAccountEmailAddress",
+            "action": "DeleteServiceLinkedRole",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateAssumeRolePolicy": {
+        "CreateInstanceProfile": {
             "access_level": "Undocumented",
-            "action": "UpdateAssumeRolePolicy",
+            "action": "CreateInstanceProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutRolePolicy": {
+        "DeactivateMFADevice": {
             "access_level": "Undocumented",
-            "action": "PutRolePolicy",
+            "action": "DeactivateMFADevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagPolicy": {
+        "ListAttachedUserPolicies": {
             "access_level": "Undocumented",
-            "action": "UntagPolicy",
+            "action": "ListAttachedUserPolicies",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GenerateServiceLastAccessedDetails": {
+        "AddRoleToInstanceProfile": {
             "access_level": "Undocumented",
-            "action": "GenerateServiceLastAccessedDetails",
+            "action": "AddRoleToInstanceProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagInstanceProfile": {
+        "CreateAccountAlias": {
             "access_level": "Undocumented",
-            "action": "UntagInstanceProfile",
+            "action": "CreateAccountAlias",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ResetServiceSpecificCredential": {
+        "UpdateGroup": {
             "access_level": "Undocumented",
-            "action": "ResetServiceSpecificCredential",
+            "action": "UpdateGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SetDefaultPolicyVersion": {
+        "UpdateRole": {
             "access_level": "Undocumented",
-            "action": "SetDefaultPolicyVersion",
+            "action": "UpdateRole",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetUser": {
+        "GetAccountName": {
             "access_level": "Undocumented",
-            "action": "GetUser",
+            "action": "GetAccountName",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPolicyVersions": {
+        "UpdateUser": {
             "access_level": "Undocumented",
-            "action": "ListPolicyVersions",
+            "action": "UpdateUser",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagMFADevice": {
+        "UploadServerCertificate": {
             "access_level": "Undocumented",
-            "action": "TagMFADevice",
+            "action": "UploadServerCertificate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteCloudFrontPublicKey": {
+        "SimulatePrincipalPolicy": {
             "access_level": "Undocumented",
-            "action": "DeleteCloudFrontPublicKey",
+            "action": "SimulatePrincipalPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateOpenIDConnectProviderThumbprint": {
+        "GetInstanceProfile": {
             "access_level": "Undocumented",
-            "action": "UpdateOpenIDConnectProviderThumbprint",
+            "action": "GetInstanceProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateGroup": {
+        "GetAccountPasswordPolicy": {
             "access_level": "Undocumented",
-            "action": "UpdateGroup",
+            "action": "GetAccountPasswordPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PassRole": {
+        "DeletePolicyVersion": {
             "access_level": "Undocumented",
-            "action": "PassRole",
+            "action": "DeletePolicyVersion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetServiceLastAccessedDetailsWithEntities": {
+        "UpdateLoginProfile": {
             "access_level": "Undocumented",
-            "action": "GetServiceLastAccessedDetailsWithEntities",
+            "action": "UpdateLoginProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateRole": {
+        "CreateServiceLinkedRole": {
             "access_level": "Undocumented",
-            "action": "CreateRole",
+            "action": "CreateServiceLinkedRole",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateUser": {
+        "ListServerCertificateTags": {
             "access_level": "Undocumented",
-            "action": "UpdateUser",
+            "action": "ListServerCertificateTags",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListInstanceProfiles": {
+        "DeleteCloudFrontPublicKey": {
             "access_level": "Undocumented",
-            "action": "ListInstanceProfiles",
+            "action": "DeleteCloudFrontPublicKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetInstanceProfile": {
+        "GenerateOrganizationsAccessReport": {
             "access_level": "Undocumented",
-            "action": "GetInstanceProfile",
+            "action": "GenerateOrganizationsAccessReport",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateAccountName": {
+        "CreateServiceSpecificCredential": {
             "access_level": "Undocumented",
-            "action": "UpdateAccountName",
+            "action": "CreateServiceSpecificCredential",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreatePolicy": {
+        "UntagPolicy": {
             "access_level": "Undocumented",
-            "action": "CreatePolicy",
+            "action": "UntagPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetRolePolicy": {
+        "TagOpenIDConnectProvider": {
             "access_level": "Undocumented",
-            "action": "GetRolePolicy",
+            "action": "TagOpenIDConnectProvider",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListOpenIDConnectProviders": {
+        "UploadSSHPublicKey": {
             "access_level": "Undocumented",
-            "action": "ListOpenIDConnectProviders",
+            "action": "UploadSSHPublicKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteVirtualMFADevice": {
+        "DeleteRolePermissionsBoundary": {
             "access_level": "Undocumented",
-            "action": "DeleteVirtualMFADevice",
+            "action": "DeleteRolePermissionsBoundary",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAccountAuthorizationDetails": {
+        "ListPolicies": {
             "access_level": "Undocumented",
-            "action": "GetAccountAuthorizationDetails",
+            "action": "ListPolicies",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DetachGroupPolicy": {
+        "DeleteGroup": {
             "access_level": "Undocumented",
-            "action": "DetachGroupPolicy",
+            "action": "DeleteGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSigningCertificates": {
+        "UntagUser": {
             "access_level": "Undocumented",
-            "action": "ListSigningCertificates",
+            "action": "UntagUser",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateRole": {
+        "ListGroupPolicies": {
             "access_level": "Undocumented",
-            "action": "UpdateRole",
+            "action": "ListGroupPolicies",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteGroup": {
+        "ListUserPolicies": {
             "access_level": "Undocumented",
-            "action": "DeleteGroup",
+            "action": "ListUserPolicies",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteOpenIDConnectProvider": {
+        "SimulateCustomPolicy": {
             "access_level": "Undocumented",
-            "action": "DeleteOpenIDConnectProvider",
+            "action": "SimulateCustomPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAccountEmailAddress": {
+        "DeleteAccountAlias": {
             "access_level": "Undocumented",
-            "action": "GetAccountEmailAddress",
+            "action": "DeleteAccountAlias",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetMFADevice": {
+        "GetCloudFrontPublicKey": {
             "access_level": "Undocumented",
-            "action": "GetMFADevice",
+            "action": "GetCloudFrontPublicKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAttachedGroupPolicies": {
+        "UpdateSAMLProvider": {
             "access_level": "Undocumented",
-            "action": "ListAttachedGroupPolicies",
+            "action": "UpdateSAMLProvider",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutGroupPolicy": {
+        "ListOpenIDConnectProviderTags": {
             "access_level": "Undocumented",
-            "action": "PutGroupPolicy",
+            "action": "ListOpenIDConnectProviderTags",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "PutRolePermissionsBoundary": {
             "access_level": "Undocumented",
             "action": "PutRolePermissionsBoundary",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteGroupPolicy": {
+        "GetPolicy": {
             "access_level": "Undocumented",
-            "action": "DeleteGroupPolicy",
+            "action": "GetPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteSigningCertificate": {
+        "DeleteSAMLProvider": {
             "access_level": "Undocumented",
-            "action": "DeleteSigningCertificate",
+            "action": "DeleteSAMLProvider",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListUserTags": {
+        "ListGroups": {
             "access_level": "Undocumented",
-            "action": "ListUserTags",
+            "action": "ListGroups",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPolicyTags": {
+        "UpdateCloudFrontPublicKey": {
             "access_level": "Undocumented",
-            "action": "ListPolicyTags",
+            "action": "UpdateCloudFrontPublicKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateSAMLProvider": {
+        "DeleteUserPermissionsBoundary": {
             "access_level": "Undocumented",
-            "action": "CreateSAMLProvider",
+            "action": "DeleteUserPermissionsBoundary",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateServiceSpecificCredential": {
+        "ListMFADeviceTags": {
             "access_level": "Undocumented",
-            "action": "CreateServiceSpecificCredential",
+            "action": "ListMFADeviceTags",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSSHPublicKeys": {
+        "GetPolicyVersion": {
             "access_level": "Undocumented",
-            "action": "ListSSHPublicKeys",
+            "action": "GetPolicyVersion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteServerCertificate": {
+        "UpdateAssumeRolePolicy": {
             "access_level": "Undocumented",
-            "action": "DeleteServerCertificate",
+            "action": "UpdateAssumeRolePolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagInstanceProfile": {
+        "RemoveRoleFromInstanceProfile": {
             "access_level": "Undocumented",
-            "action": "TagInstanceProfile",
+            "action": "RemoveRoleFromInstanceProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListRoles": {
+        "TagSAMLProvider": {
             "access_level": "Undocumented",
-            "action": "ListRoles",
+            "action": "TagSAMLProvider",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListGroupPolicies": {
+        "CreateOpenIDConnectProvider": {
             "access_level": "Undocumented",
-            "action": "ListGroupPolicies",
+            "action": "CreateOpenIDConnectProvider",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListMFADevices": {
+        "ListVirtualMFADevices": {
             "access_level": "Undocumented",
-            "action": "ListMFADevices",
+            "action": "ListVirtualMFADevices",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GenerateOrganizationsAccessReport": {
+        "ResyncMFADevice": {
             "access_level": "Undocumented",
-            "action": "GenerateOrganizationsAccessReport",
+            "action": "ResyncMFADevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetContextKeysForCustomPolicy": {
+        "ListServiceSpecificCredentials": {
             "access_level": "Undocumented",
-            "action": "GetContextKeysForCustomPolicy",
+            "action": "ListServiceSpecificCredentials",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagOpenIDConnectProvider": {
+        "ListCloudFrontPublicKeys": {
             "access_level": "Undocumented",
-            "action": "TagOpenIDConnectProvider",
+            "action": "ListCloudFrontPublicKeys",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateLoginProfile": {
+        "ListSigningCertificates": {
             "access_level": "Undocumented",
-            "action": "UpdateLoginProfile",
+            "action": "ListSigningCertificates",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListServerCertificateTags": {
+        "DeleteVirtualMFADevice": {
             "access_level": "Undocumented",
-            "action": "ListServerCertificateTags",
+            "action": "DeleteVirtualMFADevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListOpenIDConnectProviderTags": {
+        "TagServerCertificate": {
             "access_level": "Undocumented",
-            "action": "ListOpenIDConnectProviderTags",
+            "action": "TagServerCertificate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AttachRolePolicy": {
+        "GetUser": {
             "access_level": "Undocumented",
-            "action": "AttachRolePolicy",
+            "action": "GetUser",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListMFADeviceTags": {
+        "ChangePassword": {
             "access_level": "Undocumented",
-            "action": "ListMFADeviceTags",
+            "action": "ChangePassword",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagMFADevice": {
+        "ListGroupsForUser": {
             "access_level": "Undocumented",
-            "action": "UntagMFADevice",
+            "action": "ListGroupsForUser",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeletePolicy": {
+        "GetGroup": {
             "access_level": "Undocumented",
-            "action": "DeletePolicy",
+            "action": "GetGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteRole": {
+        "RemoveClientIDFromOpenIDConnectProvider": {
             "access_level": "Undocumented",
-            "action": "DeleteRole",
+            "action": "RemoveClientIDFromOpenIDConnectProvider",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateServerCertificate": {
+        "UntagRole": {
             "access_level": "Undocumented",
-            "action": "UpdateServerCertificate",
+            "action": "UntagRole",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AddRoleToInstanceProfile": {
+        "CreateVirtualMFADevice": {
             "access_level": "Undocumented",
-            "action": "AddRoleToInstanceProfile",
+            "action": "CreateVirtualMFADevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateSigningCertificate": {
+        "TagInstanceProfile": {
             "access_level": "Undocumented",
-            "action": "UpdateSigningCertificate",
+            "action": "TagInstanceProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPolicies": {
+        "ListSTSRegionalEndpointsStatus": {
             "access_level": "Undocumented",
-            "action": "ListPolicies",
+            "action": "ListSTSRegionalEndpointsStatus",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "EnableMFADevice": {
+        "GetOrganizationsAccessReport": {
             "access_level": "Undocumented",
-            "action": "EnableMFADevice",
+            "action": "GetOrganizationsAccessReport",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAttachedUserPolicies": {
+        "ListUsers": {
             "access_level": "Undocumented",
-            "action": "ListAttachedUserPolicies",
+            "action": "ListUsers",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateAccessKey": {
+        "UntagServerCertificate": {
             "access_level": "Undocumented",
-            "action": "UpdateAccessKey",
+            "action": "UntagServerCertificate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagSAMLProvider": {
+        "ListAttachedGroupPolicies": {
             "access_level": "Undocumented",
-            "action": "TagSAMLProvider",
+            "action": "ListAttachedGroupPolicies",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagPolicy": {
+        "TagRole": {
             "access_level": "Undocumented",
-            "action": "TagPolicy",
+            "action": "TagRole",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSAMLProviderTags": {
+        "ResetServiceSpecificCredential": {
             "access_level": "Undocumented",
-            "action": "ListSAMLProviderTags",
+            "action": "ResetServiceSpecificCredential",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateAccountAlias": {
+        "GetServiceLastAccessedDetails": {
             "access_level": "Undocumented",
-            "action": "CreateAccountAlias",
+            "action": "GetServiceLastAccessedDetails",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ChangePassword": {
+        "UpdateSigningCertificate": {
             "access_level": "Undocumented",
-            "action": "ChangePassword",
+            "action": "UpdateSigningCertificate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "identity-sync": {
@@ -84227,41 +84227,41 @@
             "orphan": false,
             "resources": [
                 "Monitor"
             ]
         }
     },
     "invoicing": {
-        "ListInvoiceSummaries": {
+        "PutInvoiceEmailDeliveryPreferences": {
             "access_level": "Undocumented",
-            "action": "ListInvoiceSummaries",
+            "action": "PutInvoiceEmailDeliveryPreferences",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutInvoiceEmailDeliveryPreferences": {
+        "GetInvoicePDF": {
             "access_level": "Undocumented",
-            "action": "PutInvoiceEmailDeliveryPreferences",
+            "action": "GetInvoicePDF",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetInvoiceEmailDeliveryPreferences": {
+        "ListInvoiceSummaries": {
             "access_level": "Undocumented",
-            "action": "GetInvoiceEmailDeliveryPreferences",
+            "action": "ListInvoiceSummaries",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetInvoicePDF": {
+        "GetInvoiceEmailDeliveryPreferences": {
             "access_level": "Undocumented",
-            "action": "GetInvoicePDF",
+            "action": "GetInvoiceEmailDeliveryPreferences",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "iot": {
@@ -90426,913 +90426,913 @@
             "orphan": false,
             "resources": [
                 "workspace"
             ]
         }
     },
     "iotwireless": {
-        "UpdateResourceEventConfiguration": {
+        "CancelMulticastGroupSession": {
             "access_level": "Undocumented",
-            "action": "UpdateResourceEventConfiguration",
+            "action": "CancelMulticastGroupSession",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssociateWirelessGatewayWithThing": {
+        "UpdateMetricConfiguration": {
             "access_level": "Undocumented",
-            "action": "AssociateWirelessGatewayWithThing",
+            "action": "UpdateMetricConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListDestinations": {
+        "GetDestination": {
             "access_level": "Undocumented",
-            "action": "ListDestinations",
+            "action": "GetDestination",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateMetricConfiguration": {
+        "ListMulticastGroupsByFuotaTask": {
             "access_level": "Undocumented",
-            "action": "UpdateMetricConfiguration",
+            "action": "ListMulticastGroupsByFuotaTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteNetworkAnalyzerConfiguration": {
+        "CreateFuotaTask": {
             "access_level": "Undocumented",
-            "action": "DeleteNetworkAnalyzerConfiguration",
+            "action": "CreateFuotaTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListMulticastGroupsByFuotaTask": {
+        "UpdatePartnerAccount": {
             "access_level": "Undocumented",
-            "action": "ListMulticastGroupsByFuotaTask",
+            "action": "UpdatePartnerAccount",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartMulticastGroupSession": {
+        "UpdateResourceEventConfiguration": {
             "access_level": "Undocumented",
-            "action": "StartMulticastGroupSession",
+            "action": "UpdateResourceEventConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPositionEstimate": {
+        "DisassociateWirelessDeviceFromFuotaTask": {
             "access_level": "Undocumented",
-            "action": "GetPositionEstimate",
+            "action": "DisassociateWirelessDeviceFromFuotaTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetEventConfigurationByResourceTypes": {
+        "DeleteMulticastGroup": {
             "access_level": "Undocumented",
-            "action": "GetEventConfigurationByResourceTypes",
+            "action": "DeleteMulticastGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DisassociateWirelessGatewayFromCertificate": {
+        "StartBulkDisassociateWirelessDeviceFromMulticastGroup": {
             "access_level": "Undocumented",
-            "action": "DisassociateWirelessGatewayFromCertificate",
+            "action": "StartBulkDisassociateWirelessDeviceFromMulticastGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartBulkAssociateWirelessDeviceWithMulticastGroup": {
+        "GetMulticastGroup": {
             "access_level": "Undocumented",
-            "action": "StartBulkAssociateWirelessDeviceWithMulticastGroup",
+            "action": "GetMulticastGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteWirelessDevice": {
+        "ListDeviceProfiles": {
             "access_level": "Undocumented",
-            "action": "DeleteWirelessDevice",
+            "action": "ListDeviceProfiles",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetWirelessDeviceImportTask": {
+        "TestWirelessDevice": {
             "access_level": "Undocumented",
-            "action": "GetWirelessDeviceImportTask",
+            "action": "TestWirelessDevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteFuotaTask": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "DeleteFuotaTask",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListQueuedMessages": {
+        "GetEventConfigurationByResourceTypes": {
             "access_level": "Undocumented",
-            "action": "ListQueuedMessages",
+            "action": "GetEventConfigurationByResourceTypes",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateDestination": {
+        "ListWirelessDevices": {
             "access_level": "Undocumented",
-            "action": "CreateDestination",
+            "action": "ListWirelessDevices",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListMulticastGroups": {
+        "StartWirelessDeviceImportTask": {
             "access_level": "Undocumented",
-            "action": "ListMulticastGroups",
+            "action": "StartWirelessDeviceImportTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListWirelessGatewayTaskDefinitions": {
+        "AssociateAwsAccountWithPartnerAccount": {
             "access_level": "Undocumented",
-            "action": "ListWirelessGatewayTaskDefinitions",
+            "action": "AssociateAwsAccountWithPartnerAccount",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetWirelessGatewayCertificate": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "GetWirelessGatewayCertificate",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DeleteServiceProfile": {
             "access_level": "Undocumented",
             "action": "DeleteServiceProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartNetworkAnalyzerStream": {
+        "ListDevicesForWirelessDeviceImportTask": {
             "access_level": "Undocumented",
-            "action": "StartNetworkAnalyzerStream",
+            "action": "ListDevicesForWirelessDeviceImportTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateDeviceProfile": {
+        "AssociateWirelessDeviceWithFuotaTask": {
             "access_level": "Undocumented",
-            "action": "CreateDeviceProfile",
+            "action": "AssociateWirelessDeviceWithFuotaTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetWirelessDevice": {
+        "DeleteQueuedMessages": {
             "access_level": "Undocumented",
-            "action": "GetWirelessDevice",
+            "action": "DeleteQueuedMessages",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetDeviceProfile": {
+        "ListPartnerAccounts": {
             "access_level": "Undocumented",
-            "action": "GetDeviceProfile",
+            "action": "ListPartnerAccounts",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DisassociateAwsAccountFromPartnerAccount": {
+        "UpdateEventConfigurationByResourceTypes": {
             "access_level": "Undocumented",
-            "action": "DisassociateAwsAccountFromPartnerAccount",
+            "action": "UpdateEventConfigurationByResourceTypes",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateWirelessDevice": {
+        "AssociateWirelessDeviceWithMulticastGroup": {
             "access_level": "Undocumented",
-            "action": "UpdateWirelessDevice",
+            "action": "AssociateWirelessDeviceWithMulticastGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetMulticastGroupSession": {
+        "DisassociateMulticastGroupFromFuotaTask": {
             "access_level": "Undocumented",
-            "action": "GetMulticastGroupSession",
+            "action": "DisassociateMulticastGroupFromFuotaTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetNetworkAnalyzerConfiguration": {
+        "GetPartnerAccount": {
             "access_level": "Undocumented",
-            "action": "GetNetworkAnalyzerConfiguration",
+            "action": "GetPartnerAccount",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SendDataToMulticastGroup": {
+        "ListMulticastGroups": {
             "access_level": "Undocumented",
-            "action": "SendDataToMulticastGroup",
+            "action": "ListMulticastGroups",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ResetResourceLogLevel": {
+        "DisassociateWirelessDeviceFromThing": {
             "access_level": "Undocumented",
-            "action": "ResetResourceLogLevel",
+            "action": "DisassociateWirelessDeviceFromThing",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateServiceProfile": {
+        "GetPositionEstimate": {
             "access_level": "Undocumented",
-            "action": "CreateServiceProfile",
+            "action": "GetPositionEstimate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteMulticastGroup": {
+        "ResetResourceLogLevel": {
             "access_level": "Undocumented",
-            "action": "DeleteMulticastGroup",
+            "action": "ResetResourceLogLevel",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetMetrics": {
+        "DisassociateWirelessDeviceFromMulticastGroup": {
             "access_level": "Undocumented",
-            "action": "GetMetrics",
+            "action": "DisassociateWirelessDeviceFromMulticastGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteWirelessGatewayTask": {
+        "UpdatePosition": {
             "access_level": "Undocumented",
-            "action": "DeleteWirelessGatewayTask",
+            "action": "UpdatePosition",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetDestination": {
+        "DeleteWirelessGatewayTaskDefinition": {
             "access_level": "Undocumented",
-            "action": "GetDestination",
+            "action": "DeleteWirelessGatewayTaskDefinition",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteDeviceProfile": {
+        "GetPosition": {
             "access_level": "Undocumented",
-            "action": "DeleteDeviceProfile",
+            "action": "GetPosition",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TestWirelessDevice": {
+        "DeregisterWirelessDevice": {
             "access_level": "Undocumented",
-            "action": "TestWirelessDevice",
+            "action": "DeregisterWirelessDevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateWirelessGatewayTask": {
+        "CreateWirelessDevice": {
             "access_level": "Undocumented",
-            "action": "CreateWirelessGatewayTask",
+            "action": "CreateWirelessDevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssociateMulticastGroupWithFuotaTask": {
+        "UpdateWirelessGateway": {
             "access_level": "Undocumented",
-            "action": "AssociateMulticastGroupWithFuotaTask",
+            "action": "UpdateWirelessGateway",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateWirelessGatewayTaskDefinition": {
+        "AssociateWirelessGatewayWithThing": {
             "access_level": "Undocumented",
-            "action": "CreateWirelessGatewayTaskDefinition",
+            "action": "AssociateWirelessGatewayWithThing",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "ListNetworkAnalyzerConfigurations": {
             "access_level": "Undocumented",
             "action": "ListNetworkAnalyzerConfigurations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssociateWirelessDeviceWithMulticastGroup": {
+        "DeleteWirelessDeviceImportTask": {
             "access_level": "Undocumented",
-            "action": "AssociateWirelessDeviceWithMulticastGroup",
+            "action": "DeleteWirelessDeviceImportTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateResourcePosition": {
+        "GetServiceProfile": {
             "access_level": "Undocumented",
-            "action": "UpdateResourcePosition",
+            "action": "GetServiceProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPartnerAccount": {
+        "CreateWirelessGateway": {
             "access_level": "Undocumented",
-            "action": "GetPartnerAccount",
+            "action": "CreateWirelessGateway",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateDestination": {
+        "ListWirelessDeviceImportTasks": {
             "access_level": "Undocumented",
-            "action": "UpdateDestination",
+            "action": "ListWirelessDeviceImportTasks",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssociateWirelessDeviceWithThing": {
+        "CreateWirelessGatewayTaskDefinition": {
             "access_level": "Undocumented",
-            "action": "AssociateWirelessDeviceWithThing",
+            "action": "CreateWirelessGatewayTaskDefinition",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateEventConfigurationByResourceTypes": {
+        "GetResourceEventConfiguration": {
             "access_level": "Undocumented",
-            "action": "UpdateEventConfigurationByResourceTypes",
+            "action": "GetResourceEventConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateFuotaTask": {
+        "PutPositionConfiguration": {
             "access_level": "Undocumented",
-            "action": "CreateFuotaTask",
+            "action": "PutPositionConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetWirelessDeviceStatistics": {
+        "GetWirelessGatewayTaskDefinition": {
             "access_level": "Undocumented",
-            "action": "GetWirelessDeviceStatistics",
+            "action": "GetWirelessGatewayTaskDefinition",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ResetAllResourceLogLevels": {
+        "GetWirelessDevice": {
             "access_level": "Undocumented",
-            "action": "ResetAllResourceLogLevels",
+            "action": "GetWirelessDevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetWirelessGatewayTask": {
+        "GetPositionConfiguration": {
             "access_level": "Undocumented",
-            "action": "GetWirelessGatewayTask",
+            "action": "GetPositionConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CancelMulticastGroupSession": {
+        "ListEventConfigurations": {
             "access_level": "Undocumented",
-            "action": "CancelMulticastGroupSession",
+            "action": "ListEventConfigurations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdatePartnerAccount": {
+        "StartNetworkAnalyzerStream": {
             "access_level": "Undocumented",
-            "action": "UpdatePartnerAccount",
+            "action": "StartNetworkAnalyzerStream",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssociateAwsAccountWithPartnerAccount": {
+        "DisassociateWirelessGatewayFromCertificate": {
             "access_level": "Undocumented",
-            "action": "AssociateAwsAccountWithPartnerAccount",
+            "action": "DisassociateWirelessGatewayFromCertificate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteWirelessDeviceImportTask": {
+        "GetWirelessGatewayStatistics": {
             "access_level": "Undocumented",
-            "action": "DeleteWirelessDeviceImportTask",
+            "action": "GetWirelessGatewayStatistics",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetServiceEndpoint": {
+        "DeleteDeviceProfile": {
             "access_level": "Undocumented",
-            "action": "GetServiceEndpoint",
+            "action": "DeleteDeviceProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DisassociateWirelessDeviceFromFuotaTask": {
+        "AssociateMulticastGroupWithFuotaTask": {
             "access_level": "Undocumented",
-            "action": "DisassociateWirelessDeviceFromFuotaTask",
+            "action": "AssociateMulticastGroupWithFuotaTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "GetLogLevelsByResourceTypes": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "GetLogLevelsByResourceTypes",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SendDataToWirelessDevice": {
+        "CreateServiceProfile": {
             "access_level": "Undocumented",
-            "action": "SendDataToWirelessDevice",
+            "action": "CreateServiceProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetFuotaTask": {
+        "DeleteWirelessGateway": {
             "access_level": "Undocumented",
-            "action": "GetFuotaTask",
+            "action": "DeleteWirelessGateway",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetLogLevelsByResourceTypes": {
+        "ListFuotaTasks": {
             "access_level": "Undocumented",
-            "action": "GetLogLevelsByResourceTypes",
+            "action": "ListFuotaTasks",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetWirelessGatewayTaskDefinition": {
+        "ListDestinations": {
             "access_level": "Undocumented",
-            "action": "GetWirelessGatewayTaskDefinition",
+            "action": "ListDestinations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetResourceEventConfiguration": {
+        "StartSingleWirelessDeviceImportTask": {
             "access_level": "Undocumented",
-            "action": "GetResourceEventConfiguration",
+            "action": "StartSingleWirelessDeviceImportTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListDevicesForWirelessDeviceImportTask": {
+        "AssociateWirelessGatewayWithCertificate": {
             "access_level": "Undocumented",
-            "action": "ListDevicesForWirelessDeviceImportTask",
+            "action": "AssociateWirelessGatewayWithCertificate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssociateWirelessGatewayWithCertificate": {
+        "ListPositionConfigurations": {
             "access_level": "Undocumented",
-            "action": "AssociateWirelessGatewayWithCertificate",
+            "action": "ListPositionConfigurations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetWirelessGateway": {
+        "GetResourcePosition": {
             "access_level": "Undocumented",
-            "action": "GetWirelessGateway",
+            "action": "GetResourcePosition",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetWirelessGatewayStatistics": {
+        "DeleteFuotaTask": {
             "access_level": "Undocumented",
-            "action": "GetWirelessGatewayStatistics",
+            "action": "DeleteFuotaTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetResourceLogLevel": {
+        "StartBulkAssociateWirelessDeviceWithMulticastGroup": {
             "access_level": "Undocumented",
-            "action": "GetResourceLogLevel",
+            "action": "StartBulkAssociateWirelessDeviceWithMulticastGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListEventConfigurations": {
+        "GetWirelessGatewayFirmwareInformation": {
             "access_level": "Undocumented",
-            "action": "ListEventConfigurations",
+            "action": "GetWirelessGatewayFirmwareInformation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeregisterWirelessDevice": {
+        "UpdateMulticastGroup": {
             "access_level": "Undocumented",
-            "action": "DeregisterWirelessDevice",
+            "action": "UpdateMulticastGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteWirelessGateway": {
+        "DeleteNetworkAnalyzerConfiguration": {
             "access_level": "Undocumented",
-            "action": "DeleteWirelessGateway",
+            "action": "DeleteNetworkAnalyzerConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteWirelessGatewayTaskDefinition": {
+        "GetResourceLogLevel": {
             "access_level": "Undocumented",
-            "action": "DeleteWirelessGatewayTaskDefinition",
+            "action": "GetResourceLogLevel",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetServiceProfile": {
+        "StartFuotaTask": {
             "access_level": "Undocumented",
-            "action": "GetServiceProfile",
+            "action": "StartFuotaTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetMetricConfiguration": {
+        "UpdateLogLevelsByResourceTypes": {
             "access_level": "Undocumented",
-            "action": "GetMetricConfiguration",
+            "action": "UpdateLogLevelsByResourceTypes",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetResourcePosition": {
+        "GetFuotaTask": {
             "access_level": "Undocumented",
-            "action": "GetResourcePosition",
+            "action": "GetFuotaTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutResourceLogLevel": {
+        "CreateDeviceProfile": {
             "access_level": "Undocumented",
-            "action": "PutResourceLogLevel",
+            "action": "CreateDeviceProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DisassociateMulticastGroupFromFuotaTask": {
+        "DisassociateAwsAccountFromPartnerAccount": {
             "access_level": "Undocumented",
-            "action": "DisassociateMulticastGroupFromFuotaTask",
+            "action": "DisassociateAwsAccountFromPartnerAccount",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdatePosition": {
+        "DeleteWirelessGatewayTask": {
             "access_level": "Undocumented",
-            "action": "UpdatePosition",
+            "action": "DeleteWirelessGatewayTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetMulticastGroup": {
+        "ListWirelessGatewayTaskDefinitions": {
             "access_level": "Undocumented",
-            "action": "GetMulticastGroup",
+            "action": "ListWirelessGatewayTaskDefinitions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutPositionConfiguration": {
+        "UpdateFuotaTask": {
             "access_level": "Undocumented",
-            "action": "PutPositionConfiguration",
+            "action": "UpdateFuotaTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPositionConfiguration": {
+        "GetWirelessGateway": {
             "access_level": "Undocumented",
-            "action": "GetPositionConfiguration",
+            "action": "GetWirelessGateway",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateWirelessDeviceImportTask": {
+        "PutResourceLogLevel": {
             "access_level": "Undocumented",
-            "action": "UpdateWirelessDeviceImportTask",
+            "action": "PutResourceLogLevel",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListWirelessDeviceImportTasks": {
+        "GetWirelessDeviceImportTask": {
             "access_level": "Undocumented",
-            "action": "ListWirelessDeviceImportTasks",
+            "action": "GetWirelessDeviceImportTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateMulticastGroup": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "CreateMulticastGroup",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListWirelessGateways": {
+        "ListQueuedMessages": {
             "access_level": "Undocumented",
-            "action": "ListWirelessGateways",
+            "action": "ListQueuedMessages",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListDeviceProfiles": {
+        "GetWirelessGatewayCertificate": {
             "access_level": "Undocumented",
-            "action": "ListDeviceProfiles",
+            "action": "GetWirelessGatewayCertificate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "SendDataToMulticastGroup": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "SendDataToMulticastGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartBulkDisassociateWirelessDeviceFromMulticastGroup": {
+        "GetMetricConfiguration": {
             "access_level": "Undocumented",
-            "action": "StartBulkDisassociateWirelessDeviceFromMulticastGroup",
+            "action": "GetMetricConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListServiceProfiles": {
+        "UpdateNetworkAnalyzerConfiguration": {
             "access_level": "Undocumented",
-            "action": "ListServiceProfiles",
+            "action": "UpdateNetworkAnalyzerConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateWirelessGateway": {
+        "ListServiceProfiles": {
             "access_level": "Undocumented",
-            "action": "UpdateWirelessGateway",
+            "action": "ListServiceProfiles",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateNetworkAnalyzerConfiguration": {
+        "SendDataToWirelessDevice": {
             "access_level": "Undocumented",
-            "action": "CreateNetworkAnalyzerConfiguration",
+            "action": "SendDataToWirelessDevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartSingleWirelessDeviceImportTask": {
+        "UpdateWirelessDevice": {
             "access_level": "Undocumented",
-            "action": "StartSingleWirelessDeviceImportTask",
+            "action": "UpdateWirelessDevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPosition": {
+        "UpdateWirelessDeviceImportTask": {
             "access_level": "Undocumented",
-            "action": "GetPosition",
+            "action": "UpdateWirelessDeviceImportTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DisassociateWirelessDeviceFromMulticastGroup": {
+        "ListWirelessGateways": {
             "access_level": "Undocumented",
-            "action": "DisassociateWirelessDeviceFromMulticastGroup",
+            "action": "ListWirelessGateways",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateFuotaTask": {
+        "CreateMulticastGroup": {
             "access_level": "Undocumented",
-            "action": "UpdateFuotaTask",
+            "action": "CreateMulticastGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateLogLevelsByResourceTypes": {
+        "AssociateWirelessDeviceWithThing": {
             "access_level": "Undocumented",
-            "action": "UpdateLogLevelsByResourceTypes",
+            "action": "AssociateWirelessDeviceWithThing",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateWirelessGateway": {
+        "DeleteDestination": {
             "access_level": "Undocumented",
-            "action": "CreateWirelessGateway",
+            "action": "DeleteDestination",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateMulticastGroup": {
+        "CreateWirelessGatewayTask": {
             "access_level": "Undocumented",
-            "action": "UpdateMulticastGroup",
+            "action": "CreateWirelessGatewayTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPositionConfigurations": {
+        "GetNetworkAnalyzerConfiguration": {
             "access_level": "Undocumented",
-            "action": "ListPositionConfigurations",
+            "action": "GetNetworkAnalyzerConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteQueuedMessages": {
+        "GetServiceEndpoint": {
             "access_level": "Undocumented",
-            "action": "DeleteQueuedMessages",
+            "action": "GetServiceEndpoint",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartFuotaTask": {
+        "CreateDestination": {
             "access_level": "Undocumented",
-            "action": "StartFuotaTask",
+            "action": "CreateDestination",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DisassociateWirelessGatewayFromThing": {
+        "StartMulticastGroupSession": {
             "access_level": "Undocumented",
-            "action": "DisassociateWirelessGatewayFromThing",
+            "action": "StartMulticastGroupSession",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DisassociateWirelessDeviceFromThing": {
+        "CreateNetworkAnalyzerConfiguration": {
             "access_level": "Undocumented",
-            "action": "DisassociateWirelessDeviceFromThing",
+            "action": "CreateNetworkAnalyzerConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssociateWirelessDeviceWithFuotaTask": {
+        "GetDeviceProfile": {
             "access_level": "Undocumented",
-            "action": "AssociateWirelessDeviceWithFuotaTask",
+            "action": "GetDeviceProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListFuotaTasks": {
+        "GetWirelessGatewayTask": {
             "access_level": "Undocumented",
-            "action": "ListFuotaTasks",
+            "action": "GetWirelessGatewayTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "DisassociateWirelessGatewayFromThing": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "DisassociateWirelessGatewayFromThing",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteDestination": {
+        "GetMetrics": {
             "access_level": "Undocumented",
-            "action": "DeleteDestination",
+            "action": "GetMetrics",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPartnerAccounts": {
+        "UpdateResourcePosition": {
             "access_level": "Undocumented",
-            "action": "ListPartnerAccounts",
+            "action": "UpdateResourcePosition",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateWirelessDevice": {
+        "GetMulticastGroupSession": {
             "access_level": "Undocumented",
-            "action": "CreateWirelessDevice",
+            "action": "GetMulticastGroupSession",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetWirelessGatewayFirmwareInformation": {
+        "ResetAllResourceLogLevels": {
             "access_level": "Undocumented",
-            "action": "GetWirelessGatewayFirmwareInformation",
+            "action": "ResetAllResourceLogLevels",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListWirelessDevices": {
+        "UpdateDestination": {
             "access_level": "Undocumented",
-            "action": "ListWirelessDevices",
+            "action": "UpdateDestination",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartWirelessDeviceImportTask": {
+        "DeleteWirelessDevice": {
             "access_level": "Undocumented",
-            "action": "StartWirelessDeviceImportTask",
+            "action": "DeleteWirelessDevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateNetworkAnalyzerConfiguration": {
+        "GetWirelessDeviceStatistics": {
             "access_level": "Undocumented",
-            "action": "UpdateNetworkAnalyzerConfiguration",
+            "action": "GetWirelessDeviceStatistics",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "iq": {
@@ -94499,339 +94499,339 @@
             "resources": [
                 "index",
                 "thesaurus"
             ]
         }
     },
     "kendra-ranking": {
-        "DescribeRescoreExecutionPlan": {
+        "CreateRescoreExecutionPlan": {
             "access_level": "Undocumented",
-            "action": "DescribeRescoreExecutionPlan",
+            "action": "CreateRescoreExecutionPlan",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateRescoreExecutionPlan": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "CreateRescoreExecutionPlan",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "ListTagsForResource": {
             "access_level": "Undocumented",
             "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "DescribeRescoreExecutionPlan": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "DescribeRescoreExecutionPlan",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateRescoreExecutionPlan": {
+        "DeleteRescoreExecutionPlan": {
             "access_level": "Undocumented",
-            "action": "UpdateRescoreExecutionPlan",
+            "action": "DeleteRescoreExecutionPlan",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "Rescore": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "Rescore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteRescoreExecutionPlan": {
+        "UpdateRescoreExecutionPlan": {
             "access_level": "Undocumented",
-            "action": "DeleteRescoreExecutionPlan",
+            "action": "UpdateRescoreExecutionPlan",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "ListRescoreExecutionPlans": {
             "access_level": "Undocumented",
             "action": "ListRescoreExecutionPlans",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "Rescore": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "Rescore",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "kinesis": {
-        "GetShardIterator": {
+        "CreateStream": {
             "access_level": "Undocumented",
-            "action": "GetShardIterator",
+            "action": "CreateStream",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForStream": {
+        "RegisterStreamConsumer": {
             "access_level": "Undocumented",
-            "action": "ListTagsForStream",
+            "action": "RegisterStreamConsumer",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteStream": {
+        "DecreaseStreamRetentionPeriod": {
             "access_level": "Undocumented",
-            "action": "DeleteStream",
+            "action": "DecreaseStreamRetentionPeriod",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "IncreaseStreamRetentionPeriod": {
+        "DeregisterStreamConsumer": {
             "access_level": "Undocumented",
-            "action": "IncreaseStreamRetentionPeriod",
+            "action": "DeregisterStreamConsumer",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeregisterStreamConsumer": {
+        "DescribeStreamConsumer": {
             "access_level": "Undocumented",
-            "action": "DeregisterStreamConsumer",
+            "action": "DescribeStreamConsumer",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AddTagsToStream": {
+        "ListStreams": {
             "access_level": "Undocumented",
-            "action": "AddTagsToStream",
+            "action": "ListStreams",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeStreamSummary": {
+        "GetShardIterator": {
             "access_level": "Undocumented",
-            "action": "DescribeStreamSummary",
+            "action": "GetShardIterator",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListStreams": {
+        "MergeShards": {
             "access_level": "Undocumented",
-            "action": "ListStreams",
+            "action": "MergeShards",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateShardCount": {
+        "PutRecords": {
             "access_level": "Undocumented",
-            "action": "UpdateShardCount",
+            "action": "PutRecords",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetResourcePolicy": {
+        "DeleteResourcePolicy": {
             "access_level": "Undocumented",
-            "action": "GetResourcePolicy",
+            "action": "DeleteResourcePolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SubscribeToShard": {
+        "DisableEnhancedMonitoring": {
             "access_level": "Undocumented",
-            "action": "SubscribeToShard",
+            "action": "DisableEnhancedMonitoring",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateStream": {
+        "SubscribeToShard": {
             "access_level": "Undocumented",
-            "action": "CreateStream",
+            "action": "SubscribeToShard",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SplitShard": {
+        "ListStreamConsumers": {
             "access_level": "Undocumented",
-            "action": "SplitShard",
+            "action": "ListStreamConsumers",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DecreaseStreamRetentionPeriod": {
+        "IncreaseStreamRetentionPeriod": {
             "access_level": "Undocumented",
-            "action": "DecreaseStreamRetentionPeriod",
+            "action": "IncreaseStreamRetentionPeriod",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "EnableEnhancedMonitoring": {
+        "ListTagsForStream": {
             "access_level": "Undocumented",
-            "action": "EnableEnhancedMonitoring",
+            "action": "ListTagsForStream",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetRecords": {
+        "RemoveTagsFromStream": {
             "access_level": "Undocumented",
-            "action": "GetRecords",
+            "action": "RemoveTagsFromStream",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "MergeShards": {
+        "AddTagsToStream": {
             "access_level": "Undocumented",
-            "action": "MergeShards",
+            "action": "AddTagsToStream",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RemoveTagsFromStream": {
+        "PutRecord": {
             "access_level": "Undocumented",
-            "action": "RemoveTagsFromStream",
+            "action": "PutRecord",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateStreamMode": {
+        "PutResourcePolicy": {
             "access_level": "Undocumented",
-            "action": "UpdateStreamMode",
+            "action": "PutResourcePolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeStreamConsumer": {
+        "DescribeLimits": {
             "access_level": "Undocumented",
-            "action": "DescribeStreamConsumer",
+            "action": "DescribeLimits",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeLimits": {
+        "DeleteStream": {
             "access_level": "Undocumented",
-            "action": "DescribeLimits",
+            "action": "DeleteStream",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListStreamConsumers": {
+        "SplitShard": {
             "access_level": "Undocumented",
-            "action": "ListStreamConsumers",
+            "action": "SplitShard",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutRecord": {
+        "DescribeStream": {
             "access_level": "Undocumented",
-            "action": "PutRecord",
+            "action": "DescribeStream",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteResourcePolicy": {
+        "EnableEnhancedMonitoring": {
             "access_level": "Undocumented",
-            "action": "DeleteResourcePolicy",
+            "action": "EnableEnhancedMonitoring",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutResourcePolicy": {
+        "StartStreamEncryption": {
             "access_level": "Undocumented",
-            "action": "PutResourcePolicy",
+            "action": "StartStreamEncryption",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeStream": {
+        "UpdateStreamMode": {
             "access_level": "Undocumented",
-            "action": "DescribeStream",
+            "action": "UpdateStreamMode",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListShards": {
+        "GetRecords": {
             "access_level": "Undocumented",
-            "action": "ListShards",
+            "action": "GetRecords",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutRecords": {
+        "GetResourcePolicy": {
             "access_level": "Undocumented",
-            "action": "PutRecords",
+            "action": "GetResourcePolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RegisterStreamConsumer": {
+        "DescribeStreamSummary": {
             "access_level": "Undocumented",
-            "action": "RegisterStreamConsumer",
+            "action": "DescribeStreamSummary",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "StopStreamEncryption": {
             "access_level": "Undocumented",
             "action": "StopStreamEncryption",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartStreamEncryption": {
+        "ListShards": {
             "access_level": "Undocumented",
-            "action": "StartStreamEncryption",
+            "action": "ListShards",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DisableEnhancedMonitoring": {
+        "UpdateShardCount": {
             "access_level": "Undocumented",
-            "action": "DisableEnhancedMonitoring",
+            "action": "UpdateShardCount",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "kinesisanalytics": {
@@ -97474,273 +97474,273 @@
             "orphan": false,
             "resources": [
                 "function"
             ]
         }
     },
     "launchwizard": {
-        "GetIpAddress": {
+        "ListWorkloadDeploymentPatterns": {
             "access_level": "Undocumented",
-            "action": "GetIpAddress",
+            "action": "ListWorkloadDeploymentPatterns",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateAdditionalNode": {
+        "ListDeployments": {
             "access_level": "Undocumented",
-            "action": "CreateAdditionalNode",
+            "action": "ListDeployments",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteAdditionalNode": {
+        "ListDeploymentEvents": {
             "access_level": "Undocumented",
-            "action": "DeleteAdditionalNode",
+            "action": "ListDeploymentEvents",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListWorkloadDeploymentPatterns": {
+        "GetResourceRecommendation": {
             "access_level": "Undocumented",
-            "action": "ListWorkloadDeploymentPatterns",
+            "action": "GetResourceRecommendation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSettingsSets": {
+        "GetDeployment": {
             "access_level": "Undocumented",
-            "action": "ListSettingsSets",
+            "action": "GetDeployment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeSettingsSet": {
+        "UpdateSettingsSet": {
             "access_level": "Undocumented",
-            "action": "DescribeSettingsSet",
+            "action": "UpdateSettingsSet",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetWorkloadAssets": {
+        "GetWorkloadAsset": {
             "access_level": "Undocumented",
-            "action": "GetWorkloadAssets",
+            "action": "GetWorkloadAsset",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateSettingsSet": {
+        "GetWorkloadAssets": {
             "access_level": "Undocumented",
-            "action": "UpdateSettingsSet",
+            "action": "GetWorkloadAssets",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListDeployments": {
+        "PutSettingsSet": {
             "access_level": "Undocumented",
-            "action": "ListDeployments",
+            "action": "PutSettingsSet",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAdditionalNodes": {
+        "CreateSettingsSet": {
             "access_level": "Undocumented",
-            "action": "ListAdditionalNodes",
+            "action": "CreateSettingsSet",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListResourceCostEstimates": {
+        "StartProvisioning": {
             "access_level": "Undocumented",
-            "action": "ListResourceCostEstimates",
+            "action": "StartProvisioning",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutSettingsSet": {
+        "CreateDeployment": {
             "access_level": "Undocumented",
-            "action": "PutSettingsSet",
+            "action": "CreateDeployment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DeleteApp": {
             "access_level": "Undocumented",
             "action": "DeleteApp",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListWorkloadDeploymentOptions": {
+        "DeleteAdditionalNode": {
             "access_level": "Undocumented",
-            "action": "ListWorkloadDeploymentOptions",
+            "action": "DeleteAdditionalNode",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartProvisioning": {
+        "ListProvisionedApps": {
             "access_level": "Undocumented",
-            "action": "StartProvisioning",
+            "action": "ListProvisionedApps",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteSettingsSet": {
+        "ListWorkloadDeploymentOptions": {
             "access_level": "Undocumented",
-            "action": "DeleteSettingsSet",
+            "action": "ListWorkloadDeploymentOptions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListDeploymentEvents": {
+        "DescribeProvisionedApp": {
             "access_level": "Undocumented",
-            "action": "ListDeploymentEvents",
+            "action": "DescribeProvisionedApp",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteDeployment": {
+        "ListAllowedResources": {
             "access_level": "Undocumented",
-            "action": "DeleteDeployment",
+            "action": "ListAllowedResources",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSettingsSet": {
+        "DescribeProvisioningEvents": {
             "access_level": "Undocumented",
-            "action": "GetSettingsSet",
+            "action": "DescribeProvisioningEvents",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeAdditionalNode": {
+        "GetWorkload": {
             "access_level": "Undocumented",
-            "action": "DescribeAdditionalNode",
+            "action": "GetWorkload",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeProvisioningEvents": {
+        "ListSettingsSets": {
             "access_level": "Undocumented",
-            "action": "DescribeProvisioningEvents",
+            "action": "ListSettingsSets",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateSettingsSet": {
+        "GetInfrastructureSuggestion": {
             "access_level": "Undocumented",
-            "action": "CreateSettingsSet",
+            "action": "GetInfrastructureSuggestion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetResourceRecommendation": {
+        "DescribeAdditionalNode": {
             "access_level": "Undocumented",
-            "action": "GetResourceRecommendation",
+            "action": "DescribeAdditionalNode",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListProvisionedApps": {
+        "DescribeSettingsSet": {
             "access_level": "Undocumented",
-            "action": "ListProvisionedApps",
+            "action": "DescribeSettingsSet",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateDeployment": {
+        "DeleteSettingsSet": {
             "access_level": "Undocumented",
-            "action": "CreateDeployment",
+            "action": "DeleteSettingsSet",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetResourceCostEstimate": {
+        "GetSettingsSet": {
             "access_level": "Undocumented",
-            "action": "GetResourceCostEstimate",
+            "action": "GetSettingsSet",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetWorkload": {
+        "GetIpAddress": {
             "access_level": "Undocumented",
-            "action": "GetWorkload",
+            "action": "GetIpAddress",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeProvisionedApp": {
+        "ListAdditionalNodes": {
             "access_level": "Undocumented",
-            "action": "DescribeProvisionedApp",
+            "action": "ListAdditionalNodes",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetInfrastructureSuggestion": {
+        "CreateAdditionalNode": {
             "access_level": "Undocumented",
-            "action": "GetInfrastructureSuggestion",
+            "action": "CreateAdditionalNode",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAllowedResources": {
+        "ListWorkloads": {
             "access_level": "Undocumented",
-            "action": "ListAllowedResources",
+            "action": "ListWorkloads",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListWorkloads": {
+        "ListResourceCostEstimates": {
             "access_level": "Undocumented",
-            "action": "ListWorkloads",
+            "action": "ListResourceCostEstimates",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetDeployment": {
+        "DeleteDeployment": {
             "access_level": "Undocumented",
-            "action": "GetDeployment",
+            "action": "DeleteDeployment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetWorkloadAsset": {
+        "GetResourceCostEstimate": {
             "access_level": "Undocumented",
-            "action": "GetWorkloadAsset",
+            "action": "GetResourceCostEstimate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "lex": {
@@ -104963,73 +104963,73 @@
             "access_level": "Undocumented",
             "action": "BatchGetTokenBalance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTransactionEvents": {
+        "GetTokenBalance": {
             "access_level": "Undocumented",
-            "action": "ListTransactionEvents",
+            "action": "GetTokenBalance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTokenBalances": {
+        "ListAssetContracts": {
             "access_level": "Undocumented",
-            "action": "ListTokenBalances",
+            "action": "ListAssetContracts",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAssetContracts": {
+        "ListFilteredTransactionEvents": {
             "access_level": "Undocumented",
-            "action": "ListAssetContracts",
+            "action": "ListFilteredTransactionEvents",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetTokenBalance": {
+        "ListTransactionEvents": {
             "access_level": "Undocumented",
-            "action": "GetTokenBalance",
+            "action": "ListTransactionEvents",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "ListTransactions": {
             "access_level": "Undocumented",
             "action": "ListTransactions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetTransaction": {
+        "GetAssetContract": {
             "access_level": "Undocumented",
-            "action": "GetTransaction",
+            "action": "GetAssetContract",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAssetContract": {
+        "ListTokenBalances": {
             "access_level": "Undocumented",
-            "action": "GetAssetContract",
+            "action": "ListTokenBalances",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListFilteredTransactionEvents": {
+        "GetTransaction": {
             "access_level": "Undocumented",
-            "action": "ListFilteredTransactionEvents",
+            "action": "GetTransaction",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "mapcredits": {
@@ -107205,229 +107205,229 @@
             "orphan": false,
             "resources": [
                 "packaging-groups"
             ]
         }
     },
     "mediapackagev2": {
-        "CreateChannel": {
-            "access_level": "Undocumented",
-            "action": "CreateChannel",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
-            "orphan": false,
-            "resources": []
-        },
-        "GetChannel": {
+        "ListChannels": {
             "access_level": "Undocumented",
-            "action": "GetChannel",
+            "action": "ListChannels",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateChannelGroup": {
+        "CreateOriginEndpoint": {
             "access_level": "Undocumented",
-            "action": "CreateChannelGroup",
+            "action": "CreateOriginEndpoint",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateOriginEndpoint": {
+        "GetChannel": {
             "access_level": "Undocumented",
-            "action": "CreateOriginEndpoint",
+            "action": "GetChannel",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetObject": {
+        "PutOriginEndpointPolicy": {
             "access_level": "Undocumented",
-            "action": "GetObject",
+            "action": "PutOriginEndpointPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetHeadObject": {
+        "DeleteChannelPolicy": {
             "access_level": "Undocumented",
-            "action": "GetHeadObject",
+            "action": "DeleteChannelPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "GetChannelGroup": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "GetChannelGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetOriginEndpointPolicy": {
+        "GetObject": {
             "access_level": "Undocumented",
-            "action": "GetOriginEndpointPolicy",
+            "action": "GetObject",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "UpdateChannel": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "UpdateChannel",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "UpdateChannelGroup": {
             "access_level": "Undocumented",
             "action": "UpdateChannelGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteChannelPolicy": {
+        "DeleteOriginEndpointPolicy": {
             "access_level": "Undocumented",
-            "action": "DeleteChannelPolicy",
+            "action": "DeleteOriginEndpointPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutOriginEndpointPolicy": {
+        "GetOriginEndpoint": {
             "access_level": "Undocumented",
-            "action": "PutOriginEndpointPolicy",
+            "action": "GetOriginEndpoint",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateChannel": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "UpdateChannel",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutChannelPolicy": {
+        "CreateChannelGroup": {
             "access_level": "Undocumented",
-            "action": "PutChannelPolicy",
+            "action": "CreateChannelGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutObject": {
+        "DeleteChannelGroup": {
             "access_level": "Undocumented",
-            "action": "PutObject",
+            "action": "DeleteChannelGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListChannelGroups": {
+        "DeleteChannel": {
             "access_level": "Undocumented",
-            "action": "ListChannelGroups",
+            "action": "DeleteChannel",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteChannel": {
+        "DeleteOriginEndpoint": {
             "access_level": "Undocumented",
-            "action": "DeleteChannel",
+            "action": "DeleteOriginEndpoint",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteOriginEndpoint": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "DeleteOriginEndpoint",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "PutObject": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "PutObject",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteChannelGroup": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "DeleteChannelGroup",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetChannelPolicy": {
+        "GetOriginEndpointPolicy": {
             "access_level": "Undocumented",
-            "action": "GetChannelPolicy",
+            "action": "GetOriginEndpointPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "UpdateOriginEndpoint": {
             "access_level": "Undocumented",
             "action": "UpdateOriginEndpoint",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetChannelGroup": {
+        "PutChannelPolicy": {
             "access_level": "Undocumented",
-            "action": "GetChannelGroup",
+            "action": "PutChannelPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListChannels": {
+        "GetHeadObject": {
             "access_level": "Undocumented",
-            "action": "ListChannels",
+            "action": "GetHeadObject",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetOriginEndpoint": {
+        "ListChannelGroups": {
             "access_level": "Undocumented",
-            "action": "GetOriginEndpoint",
+            "action": "ListChannelGroups",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteOriginEndpointPolicy": {
+        "CreateChannel": {
             "access_level": "Undocumented",
-            "action": "DeleteOriginEndpointPolicy",
+            "action": "CreateChannel",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "ListOriginEndpoints": {
             "access_level": "Undocumented",
             "action": "ListOriginEndpoints",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
+        },
+        "GetChannelPolicy": {
+            "access_level": "Undocumented",
+            "action": "GetChannelPolicy",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
         }
     },
     "mediastore": {
         "CreateContainer": {
             "access_level": "Write",
             "action": "CreateContainer",
             "condition_keys": [
@@ -108141,153 +108141,153 @@
             "orphan": false,
             "resources": [
                 "vodSource"
             ]
         }
     },
     "medical-imaging": {
-        "GetDatastore": {
+        "DeleteDatastore": {
             "access_level": "Undocumented",
-            "action": "GetDatastore",
+            "action": "DeleteDatastore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetImageSetMetadata": {
+        "StartDICOMImportJob": {
             "access_level": "Undocumented",
-            "action": "GetImageSetMetadata",
+            "action": "StartDICOMImportJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CopyImageSet": {
+        "GetImageFrame": {
             "access_level": "Undocumented",
-            "action": "CopyImageSet",
+            "action": "GetImageFrame",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "GetDICOMImportJob": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "GetDICOMImportJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "SearchImageSets": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "SearchImageSets",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateImageSetMetadata": {
+        "DeleteImageSet": {
             "access_level": "Undocumented",
-            "action": "UpdateImageSetMetadata",
+            "action": "DeleteImageSet",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SearchImageSets": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "SearchImageSets",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteDatastore": {
+        "ListDatastores": {
             "access_level": "Undocumented",
-            "action": "DeleteDatastore",
+            "action": "ListDatastores",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListDICOMImportJobs": {
+        "GetImageSetMetadata": {
             "access_level": "Undocumented",
-            "action": "ListDICOMImportJobs",
+            "action": "GetImageSetMetadata",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateDatastore": {
+        "GetDatastore": {
             "access_level": "Undocumented",
-            "action": "CreateDatastore",
+            "action": "GetDatastore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetImageFrame": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "GetImageFrame",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListImageSetVersions": {
+        "GetImageSet": {
             "access_level": "Undocumented",
-            "action": "ListImageSetVersions",
+            "action": "GetImageSet",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartDICOMImportJob": {
+        "CopyImageSet": {
             "access_level": "Undocumented",
-            "action": "StartDICOMImportJob",
+            "action": "CopyImageSet",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "ListDICOMImportJobs": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "ListDICOMImportJobs",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteImageSet": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "DeleteImageSet",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListDatastores": {
+        "ListImageSetVersions": {
             "access_level": "Undocumented",
-            "action": "ListDatastores",
+            "action": "ListImageSetVersions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetImageSet": {
+        "CreateDatastore": {
             "access_level": "Undocumented",
-            "action": "GetImageSet",
+            "action": "CreateDatastore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetDICOMImportJob": {
+        "UpdateImageSetMetadata": {
             "access_level": "Undocumented",
-            "action": "GetDICOMImportJob",
+            "action": "UpdateImageSetMetadata",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "memorydb": {
@@ -112703,265 +112703,265 @@
             "orphan": false,
             "resources": [
                 "database"
             ]
         }
     },
     "neptune-graph": {
-        "ListQueries": {
+        "DeletePrivateGraphEndpoint": {
             "access_level": "Undocumented",
-            "action": "ListQueries",
+            "action": "DeletePrivateGraphEndpoint",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteDataViaQuery": {
+        "GetImportTask": {
             "access_level": "Undocumented",
-            "action": "DeleteDataViaQuery",
+            "action": "GetImportTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteGraphSnapshot": {
+        "GetPrivateGraphEndpoint": {
             "access_level": "Undocumented",
-            "action": "DeleteGraphSnapshot",
+            "action": "GetPrivateGraphEndpoint",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateGraph": {
+        "DeleteDataViaQuery": {
             "access_level": "Undocumented",
-            "action": "UpdateGraph",
+            "action": "DeleteDataViaQuery",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeletePrivateGraphEndpoint": {
+        "GetQueryStatus": {
             "access_level": "Undocumented",
-            "action": "DeletePrivateGraphEndpoint",
+            "action": "GetQueryStatus",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetGraphSummary": {
+        "CreatePrivateGraphEndpoint": {
             "access_level": "Undocumented",
-            "action": "GetGraphSummary",
+            "action": "CreatePrivateGraphEndpoint",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ReadDataViaQuery": {
+        "ListImportTasks": {
             "access_level": "Undocumented",
-            "action": "ReadDataViaQuery",
+            "action": "ListImportTasks",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartImportTask": {
+        "CreateGraphUsingImportTask": {
             "access_level": "Undocumented",
-            "action": "StartImportTask",
+            "action": "CreateGraphUsingImportTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RestoreGraphFromSnapshot": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "RestoreGraphFromSnapshot",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetStatisticsStatus": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "GetStatisticsStatus",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListGraphs": {
+        "CancelImportTask": {
             "access_level": "Undocumented",
-            "action": "ListGraphs",
+            "action": "CancelImportTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetGraph": {
+        "GetGraphSnapshot": {
             "access_level": "Undocumented",
-            "action": "GetGraph",
+            "action": "GetGraphSnapshot",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CancelQuery": {
+        "GetGraphSummary": {
             "access_level": "Undocumented",
-            "action": "CancelQuery",
+            "action": "GetGraphSummary",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "WriteDataViaQuery": {
+        "DeleteGraph": {
             "access_level": "Undocumented",
-            "action": "WriteDataViaQuery",
+            "action": "DeleteGraph",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateGraphSnapshot": {
+        "ResetGraph": {
             "access_level": "Undocumented",
-            "action": "CreateGraphSnapshot",
+            "action": "ResetGraph",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateGraphUsingImportTask": {
+        "CreateGraph": {
             "access_level": "Undocumented",
-            "action": "CreateGraphUsingImportTask",
+            "action": "CreateGraph",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreatePrivateGraphEndpoint": {
+        "UpdateGraph": {
             "access_level": "Undocumented",
-            "action": "CreatePrivateGraphEndpoint",
+            "action": "UpdateGraph",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetQueryStatus": {
+        "DeleteGraphSnapshot": {
             "access_level": "Undocumented",
-            "action": "GetQueryStatus",
+            "action": "DeleteGraphSnapshot",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "GetGraph": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "GetGraph",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetEngineStatus": {
+        "ReadDataViaQuery": {
             "access_level": "Undocumented",
-            "action": "GetEngineStatus",
+            "action": "ReadDataViaQuery",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetImportTask": {
+        "CancelQuery": {
             "access_level": "Undocumented",
-            "action": "GetImportTask",
+            "action": "CancelQuery",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ResetGraph": {
+        "CreateGraphSnapshot": {
             "access_level": "Undocumented",
-            "action": "ResetGraph",
+            "action": "CreateGraphSnapshot",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetGraphSnapshot": {
+        "ListGraphSnapshots": {
             "access_level": "Undocumented",
-            "action": "GetGraphSnapshot",
+            "action": "ListGraphSnapshots",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListImportTasks": {
+        "GetEngineStatus": {
             "access_level": "Undocumented",
-            "action": "ListImportTasks",
+            "action": "GetEngineStatus",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListGraphSnapshots": {
+        "ListGraphs": {
             "access_level": "Undocumented",
-            "action": "ListGraphSnapshots",
+            "action": "ListGraphs",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "ListPrivateGraphEndpoints": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "ListPrivateGraphEndpoints",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteGraph": {
+        "StartImportTask": {
             "access_level": "Undocumented",
-            "action": "DeleteGraph",
+            "action": "StartImportTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPrivateGraphEndpoint": {
+        "GetStatisticsStatus": {
             "access_level": "Undocumented",
-            "action": "GetPrivateGraphEndpoint",
+            "action": "GetStatisticsStatus",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateGraph": {
+        "RestoreGraphFromSnapshot": {
             "access_level": "Undocumented",
-            "action": "CreateGraph",
+            "action": "RestoreGraphFromSnapshot",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CancelImportTask": {
+        "ListQueries": {
             "access_level": "Undocumented",
-            "action": "CancelImportTask",
+            "action": "ListQueries",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPrivateGraphEndpoints": {
+        "WriteDataViaQuery": {
             "access_level": "Undocumented",
-            "action": "ListPrivateGraphEndpoints",
+            "action": "WriteDataViaQuery",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "network-firewall": {
@@ -114328,65 +114328,65 @@
             "orphan": false,
             "resources": [
                 "attachment"
             ]
         }
     },
     "networkmanager-chat": {
-        "ListConversationMessages": {
+        "ListConversations": {
             "access_level": "Undocumented",
-            "action": "ListConversationMessages",
+            "action": "ListConversations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CancelMessageResponse": {
+        "ListConversationMessages": {
             "access_level": "Undocumented",
-            "action": "CancelMessageResponse",
+            "action": "ListConversationMessages",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListConversations": {
+        "CreateConversation": {
             "access_level": "Undocumented",
-            "action": "ListConversations",
+            "action": "CreateConversation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SendConversationMessage": {
+        "CancelMessageResponse": {
             "access_level": "Undocumented",
-            "action": "SendConversationMessage",
+            "action": "CancelMessageResponse",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DeleteConversation": {
             "access_level": "Undocumented",
             "action": "DeleteConversation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateConversation": {
+        "NotifyConversationIsActive": {
             "access_level": "Undocumented",
-            "action": "CreateConversation",
+            "action": "NotifyConversationIsActive",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "NotifyConversationIsActive": {
+        "SendConversationMessage": {
             "access_level": "Undocumented",
-            "action": "NotifyConversationIsActive",
+            "action": "SendConversationMessage",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "networkmonitor": {
@@ -114394,97 +114394,97 @@
             "access_level": "Undocumented",
             "action": "GetProbe",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteProbe": {
+        "ListMonitors": {
             "access_level": "Undocumented",
-            "action": "DeleteProbe",
+            "action": "ListMonitors",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteMonitor": {
+        "GetMonitor": {
             "access_level": "Undocumented",
-            "action": "DeleteMonitor",
+            "action": "GetMonitor",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateMonitor": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "UpdateMonitor",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "CreateProbe": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "CreateProbe",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "UpdateMonitor": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "UpdateMonitor",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetMonitor": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "GetMonitor",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateProbe": {
+        "CreateMonitor": {
             "access_level": "Undocumented",
-            "action": "CreateProbe",
+            "action": "CreateMonitor",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListMonitors": {
+        "DeleteMonitor": {
             "access_level": "Undocumented",
-            "action": "ListMonitors",
+            "action": "DeleteMonitor",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "UpdateProbe": {
             "access_level": "Undocumented",
             "action": "UpdateProbe",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateMonitor": {
+        "DeleteProbe": {
             "access_level": "Undocumented",
-            "action": "CreateMonitor",
+            "action": "DeleteProbe",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "nimble": {
@@ -115052,251 +115052,251 @@
             "orphan": false,
             "resources": [
                 "studio-component"
             ]
         }
     },
     "notifications": {
-        "GetNotificationConfiguration": {
+        "ListChannels": {
             "access_level": "Undocumented",
-            "action": "GetNotificationConfiguration",
+            "action": "ListChannels",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateEventRule": {
+        "ListNotificationEvents": {
             "access_level": "Undocumented",
-            "action": "CreateEventRule",
+            "action": "ListNotificationEvents",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateNotificationConfiguration": {
+        "DisassociateChannel": {
             "access_level": "Undocumented",
-            "action": "UpdateNotificationConfiguration",
+            "action": "DisassociateChannel",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListNotificationHubs": {
+        "RegisterNotificationHub": {
             "access_level": "Undocumented",
-            "action": "ListNotificationHubs",
+            "action": "RegisterNotificationHub",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RegisterNotificationHub": {
+        "GetNotificationConfiguration": {
             "access_level": "Undocumented",
-            "action": "RegisterNotificationHub",
+            "action": "GetNotificationConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "UntagResource": {
             "access_level": "Undocumented",
             "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteEventRule": {
+        "UpdateEventRule": {
             "access_level": "Undocumented",
-            "action": "DeleteEventRule",
+            "action": "UpdateEventRule",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListEventRules": {
+        "GetEventRule": {
             "access_level": "Undocumented",
-            "action": "ListEventRules",
+            "action": "GetEventRule",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteNotificationConfiguration": {
+        "AssociateChannel": {
             "access_level": "Undocumented",
-            "action": "DeleteNotificationConfiguration",
+            "action": "AssociateChannel",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DisassociateChannel": {
+        "CreateEventRule": {
             "access_level": "Undocumented",
-            "action": "DisassociateChannel",
+            "action": "CreateEventRule",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateEventRule": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "UpdateEventRule",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListNotificationEvents": {
+        "DeregisterNotificationHub": {
             "access_level": "Undocumented",
-            "action": "ListNotificationEvents",
+            "action": "DeregisterNotificationHub",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetNotificationEvent": {
+        "CreateNotificationConfiguration": {
             "access_level": "Undocumented",
-            "action": "GetNotificationEvent",
+            "action": "CreateNotificationConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListNotificationConfigurations": {
+        "DeleteNotificationConfiguration": {
             "access_level": "Undocumented",
-            "action": "ListNotificationConfigurations",
+            "action": "DeleteNotificationConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssociateChannel": {
+        "ListNotificationConfigurations": {
             "access_level": "Undocumented",
-            "action": "AssociateChannel",
+            "action": "ListNotificationConfigurations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "ListEventRules": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "ListEventRules",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetEventRule": {
+        "UpdateNotificationConfiguration": {
             "access_level": "Undocumented",
-            "action": "GetEventRule",
+            "action": "UpdateNotificationConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateNotificationConfiguration": {
+        "DeleteEventRule": {
             "access_level": "Undocumented",
-            "action": "CreateNotificationConfiguration",
+            "action": "DeleteEventRule",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeregisterNotificationHub": {
+        "ListNotificationHubs": {
             "access_level": "Undocumented",
-            "action": "DeregisterNotificationHub",
+            "action": "ListNotificationHubs",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListChannels": {
+        "GetNotificationEvent": {
             "access_level": "Undocumented",
-            "action": "ListChannels",
+            "action": "GetNotificationEvent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "notifications-contacts": {
-        "ListTagsForResource": {
+        "DeleteEmailContact": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "DeleteEmailContact",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "CreateEmailContact": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "CreateEmailContact",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetEmailContact": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "GetEmailContact",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "ListEmailContacts": {
             "access_level": "Undocumented",
             "action": "ListEmailContacts",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SendActivationCode": {
+        "ActivateEmailContact": {
             "access_level": "Undocumented",
-            "action": "SendActivationCode",
+            "action": "ActivateEmailContact",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteEmailContact": {
+        "GetEmailContact": {
             "access_level": "Undocumented",
-            "action": "DeleteEmailContact",
+            "action": "GetEmailContact",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ActivateEmailContact": {
+        "SendActivationCode": {
             "access_level": "Undocumented",
-            "action": "ActivateEmailContact",
+            "action": "SendActivationCode",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateEmailContact": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "CreateEmailContact",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "oam": {
@@ -115474,887 +115474,887 @@
             "orphan": false,
             "resources": [
                 "Link"
             ]
         }
     },
     "omics": {
-        "StartReadSetExportJob": {
+        "ListReferences": {
             "access_level": "Undocumented",
-            "action": "StartReadSetExportJob",
+            "action": "ListReferences",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetReadSet": {
+        "GetReferenceStore": {
             "access_level": "Undocumented",
-            "action": "GetReadSet",
+            "action": "GetReferenceStore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListReadSetExportJobs": {
+        "CreateMultipartReadSetUpload": {
             "access_level": "Undocumented",
-            "action": "ListReadSetExportJobs",
+            "action": "CreateMultipartReadSetUpload",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetRunGroup": {
+        "ListVariantImportJobs": {
             "access_level": "Undocumented",
-            "action": "GetRunGroup",
+            "action": "ListVariantImportJobs",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListReferenceStores": {
+        "UpdateAnnotationStoreVersion": {
             "access_level": "Undocumented",
-            "action": "ListReferenceStores",
+            "action": "UpdateAnnotationStoreVersion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateVariantStore": {
+        "StartReadSetImportJob": {
             "access_level": "Undocumented",
-            "action": "CreateVariantStore",
+            "action": "StartReadSetImportJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetVariantStore": {
+        "ListSequenceStores": {
             "access_level": "Undocumented",
-            "action": "GetVariantStore",
+            "action": "ListSequenceStores",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateShare": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "CreateShare",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateAnnotationStore": {
+        "ListAnnotationImportJobs": {
             "access_level": "Undocumented",
-            "action": "UpdateAnnotationStore",
+            "action": "ListAnnotationImportJobs",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListRunTasks": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "ListRunTasks",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartRun": {
+        "CreateRunGroup": {
             "access_level": "Undocumented",
-            "action": "StartRun",
+            "action": "CreateRunGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateWorkflow": {
+        "GetReadSet": {
             "access_level": "Undocumented",
-            "action": "CreateWorkflow",
+            "action": "GetReadSet",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteAnnotationStoreVersions": {
+        "UpdateAnnotationStore": {
             "access_level": "Undocumented",
-            "action": "DeleteAnnotationStoreVersions",
+            "action": "UpdateAnnotationStore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSequenceStores": {
+        "ListReadSetImportJobs": {
             "access_level": "Undocumented",
-            "action": "ListSequenceStores",
+            "action": "ListReadSetImportJobs",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AbortMultipartReadSetUpload": {
+        "StartVariantImportJob": {
             "access_level": "Undocumented",
-            "action": "AbortMultipartReadSetUpload",
+            "action": "StartVariantImportJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetReadSetMetadata": {
+        "StartAnnotationImportJob": {
             "access_level": "Undocumented",
-            "action": "GetReadSetMetadata",
+            "action": "StartAnnotationImportJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAnnotationStoreVersion": {
+        "GetAnnotationImportJob": {
             "access_level": "Undocumented",
-            "action": "GetAnnotationStoreVersion",
+            "action": "GetAnnotationImportJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartReferenceImportJob": {
+        "BatchDeleteReadSet": {
             "access_level": "Undocumented",
-            "action": "StartReferenceImportJob",
+            "action": "BatchDeleteReadSet",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateSequenceStore": {
+        "GetAnnotationStoreVersion": {
             "access_level": "Undocumented",
-            "action": "CreateSequenceStore",
+            "action": "GetAnnotationStoreVersion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetReadSetActivationJob": {
+        "CancelRun": {
             "access_level": "Undocumented",
-            "action": "GetReadSetActivationJob",
+            "action": "CancelRun",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteReference": {
+        "GetRunTask": {
             "access_level": "Undocumented",
-            "action": "DeleteReference",
+            "action": "GetRunTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CancelRun": {
+        "StartReferenceImportJob": {
             "access_level": "Undocumented",
-            "action": "CancelRun",
+            "action": "StartReferenceImportJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetReferenceImportJob": {
+        "GetWorkflow": {
             "access_level": "Undocumented",
-            "action": "GetReferenceImportJob",
+            "action": "GetWorkflow",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListVariantStores": {
+        "ListAnnotationStoreVersions": {
             "access_level": "Undocumented",
-            "action": "ListVariantStores",
+            "action": "ListAnnotationStoreVersions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteReferenceStore": {
+        "CancelAnnotationImportJob": {
             "access_level": "Undocumented",
-            "action": "DeleteReferenceStore",
+            "action": "CancelAnnotationImportJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListReferenceImportJobs": {
+        "CreateWorkflow": {
             "access_level": "Undocumented",
-            "action": "ListReferenceImportJobs",
+            "action": "CreateWorkflow",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CancelAnnotationImportJob": {
+        "DeleteShare": {
             "access_level": "Undocumented",
-            "action": "CancelAnnotationImportJob",
+            "action": "DeleteShare",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartReadSetActivationJob": {
+        "ListMultipartReadSetUploads": {
             "access_level": "Undocumented",
-            "action": "StartReadSetActivationJob",
+            "action": "ListMultipartReadSetUploads",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetReference": {
+        "ListRunTasks": {
             "access_level": "Undocumented",
-            "action": "GetReference",
+            "action": "ListRunTasks",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateAnnotationStore": {
+        "CreateVariantStore": {
             "access_level": "Undocumented",
-            "action": "CreateAnnotationStore",
+            "action": "CreateVariantStore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CancelVariantImportJob": {
+        "ListWorkflows": {
             "access_level": "Undocumented",
-            "action": "CancelVariantImportJob",
+            "action": "ListWorkflows",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AcceptShare": {
+        "AbortMultipartReadSetUpload": {
             "access_level": "Undocumented",
-            "action": "AcceptShare",
+            "action": "AbortMultipartReadSetUpload",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteRunGroup": {
+        "GetReadSetExportJob": {
             "access_level": "Undocumented",
-            "action": "DeleteRunGroup",
+            "action": "GetReadSetExportJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartReadSetImportJob": {
+        "ListReadSetUploadParts": {
             "access_level": "Undocumented",
-            "action": "StartReadSetImportJob",
+            "action": "ListReadSetUploadParts",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListReferences": {
+        "UpdateWorkflow": {
             "access_level": "Undocumented",
-            "action": "ListReferences",
+            "action": "UpdateWorkflow",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateRunGroup": {
+        "GetReadSetImportJob": {
             "access_level": "Undocumented",
-            "action": "UpdateRunGroup",
+            "action": "GetReadSetImportJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAnnotationStores": {
+        "DeleteReference": {
             "access_level": "Undocumented",
-            "action": "ListAnnotationStores",
+            "action": "DeleteReference",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UploadReadSetPart": {
+        "ListReferenceStores": {
             "access_level": "Undocumented",
-            "action": "UploadReadSetPart",
+            "action": "ListReferenceStores",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateAnnotationStoreVersion": {
+        "DeleteSequenceStore": {
             "access_level": "Undocumented",
-            "action": "UpdateAnnotationStoreVersion",
+            "action": "DeleteSequenceStore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CompleteMultipartReadSetUpload": {
+        "UpdateVariantStore": {
             "access_level": "Undocumented",
-            "action": "CompleteMultipartReadSetUpload",
+            "action": "UpdateVariantStore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetRun": {
+        "CancelVariantImportJob": {
             "access_level": "Undocumented",
-            "action": "GetRun",
+            "action": "CancelVariantImportJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAnnotationStore": {
+        "GetReadSetMetadata": {
             "access_level": "Undocumented",
-            "action": "GetAnnotationStore",
+            "action": "GetReadSetMetadata",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetVariantImportJob": {
+        "DeleteAnnotationStoreVersions": {
             "access_level": "Undocumented",
-            "action": "GetVariantImportJob",
+            "action": "DeleteAnnotationStoreVersions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetReferenceStore": {
+        "ListRunGroups": {
             "access_level": "Undocumented",
-            "action": "GetReferenceStore",
+            "action": "ListRunGroups",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "ListReadSetExportJobs": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "ListReadSetExportJobs",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteSequenceStore": {
+        "DeleteReferenceStore": {
             "access_level": "Undocumented",
-            "action": "DeleteSequenceStore",
+            "action": "DeleteReferenceStore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetRunTask": {
+        "GetRun": {
             "access_level": "Undocumented",
-            "action": "GetRunTask",
+            "action": "GetRun",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListMultipartReadSetUploads": {
+        "CompleteMultipartReadSetUpload": {
             "access_level": "Undocumented",
-            "action": "ListMultipartReadSetUploads",
+            "action": "CompleteMultipartReadSetUpload",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetWorkflow": {
+        "GetAnnotationStore": {
             "access_level": "Undocumented",
-            "action": "GetWorkflow",
+            "action": "GetAnnotationStore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListWorkflows": {
+        "CreateAnnotationStoreVersion": {
             "access_level": "Undocumented",
-            "action": "ListWorkflows",
+            "action": "CreateAnnotationStoreVersion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetShare": {
+        "GetReference": {
             "access_level": "Undocumented",
-            "action": "GetShare",
+            "action": "GetReference",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAnnotationImportJobs": {
+        "StartRun": {
             "access_level": "Undocumented",
-            "action": "ListAnnotationImportJobs",
+            "action": "StartRun",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListShares": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "ListShares",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAnnotationImportJob": {
+        "UploadReadSetPart": {
             "access_level": "Undocumented",
-            "action": "GetAnnotationImportJob",
+            "action": "UploadReadSetPart",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListRunGroups": {
+        "DeleteRun": {
             "access_level": "Undocumented",
-            "action": "ListRunGroups",
+            "action": "DeleteRun",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartAnnotationImportJob": {
+        "GetReadSetActivationJob": {
             "access_level": "Undocumented",
-            "action": "StartAnnotationImportJob",
+            "action": "GetReadSetActivationJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateAnnotationStoreVersion": {
+        "StartReadSetExportJob": {
             "access_level": "Undocumented",
-            "action": "CreateAnnotationStoreVersion",
+            "action": "StartReadSetExportJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteAnnotationStore": {
+        "GetShare": {
             "access_level": "Undocumented",
-            "action": "DeleteAnnotationStore",
+            "action": "GetShare",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetReferenceMetadata": {
+        "DeleteRunGroup": {
             "access_level": "Undocumented",
-            "action": "GetReferenceMetadata",
+            "action": "DeleteRunGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetReadSetImportJob": {
+        "GetVariantImportJob": {
             "access_level": "Undocumented",
-            "action": "GetReadSetImportJob",
+            "action": "GetVariantImportJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateReferenceStore": {
+        "ListReferenceImportJobs": {
             "access_level": "Undocumented",
-            "action": "CreateReferenceStore",
+            "action": "ListReferenceImportJobs",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "BatchDeleteReadSet": {
+        "ListShares": {
             "access_level": "Undocumented",
-            "action": "BatchDeleteReadSet",
+            "action": "ListShares",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartVariantImportJob": {
+        "ListRuns": {
             "access_level": "Undocumented",
-            "action": "StartVariantImportJob",
+            "action": "ListRuns",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateVariantStore": {
+        "GetReferenceImportJob": {
             "access_level": "Undocumented",
-            "action": "UpdateVariantStore",
+            "action": "GetReferenceImportJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListReadSetImportJobs": {
+        "GetRunGroup": {
             "access_level": "Undocumented",
-            "action": "ListReadSetImportJobs",
+            "action": "GetRunGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListVariantImportJobs": {
+        "CreateShare": {
             "access_level": "Undocumented",
-            "action": "ListVariantImportJobs",
+            "action": "CreateShare",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "CreateReferenceStore": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "CreateReferenceStore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateRunGroup": {
+        "ListReadSets": {
             "access_level": "Undocumented",
-            "action": "CreateRunGroup",
+            "action": "ListReadSets",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSequenceStore": {
+        "AcceptShare": {
             "access_level": "Undocumented",
-            "action": "GetSequenceStore",
+            "action": "AcceptShare",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListRuns": {
+        "GetVariantStore": {
             "access_level": "Undocumented",
-            "action": "ListRuns",
+            "action": "GetVariantStore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateMultipartReadSetUpload": {
+        "GetReferenceMetadata": {
             "access_level": "Undocumented",
-            "action": "CreateMultipartReadSetUpload",
+            "action": "GetReferenceMetadata",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListReadSetActivationJobs": {
+        "CreateSequenceStore": {
             "access_level": "Undocumented",
-            "action": "ListReadSetActivationJobs",
+            "action": "CreateSequenceStore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetReadSetExportJob": {
+        "CreateAnnotationStore": {
             "access_level": "Undocumented",
-            "action": "GetReadSetExportJob",
+            "action": "CreateAnnotationStore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteVariantStore": {
+        "UpdateRunGroup": {
             "access_level": "Undocumented",
-            "action": "DeleteVariantStore",
+            "action": "UpdateRunGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAnnotationStoreVersions": {
+        "GetSequenceStore": {
             "access_level": "Undocumented",
-            "action": "ListAnnotationStoreVersions",
+            "action": "GetSequenceStore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "ListVariantStores": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "ListVariantStores",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteRun": {
+        "ListAnnotationStores": {
             "access_level": "Undocumented",
-            "action": "DeleteRun",
+            "action": "ListAnnotationStores",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateWorkflow": {
+        "DeleteAnnotationStore": {
             "access_level": "Undocumented",
-            "action": "UpdateWorkflow",
+            "action": "DeleteAnnotationStore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteShare": {
+        "DeleteWorkflow": {
             "access_level": "Undocumented",
-            "action": "DeleteShare",
+            "action": "DeleteWorkflow",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteWorkflow": {
+        "ListReadSetActivationJobs": {
             "access_level": "Undocumented",
-            "action": "DeleteWorkflow",
+            "action": "ListReadSetActivationJobs",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListReadSets": {
+        "DeleteVariantStore": {
             "access_level": "Undocumented",
-            "action": "ListReadSets",
+            "action": "DeleteVariantStore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListReadSetUploadParts": {
+        "StartReadSetActivationJob": {
             "access_level": "Undocumented",
-            "action": "ListReadSetUploadParts",
+            "action": "StartReadSetActivationJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "one": {
-        "UpdateDeviceConfigurationTemplate": {
-            "access_level": "Undocumented",
-            "action": "UpdateDeviceConfigurationTemplate",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
-            "orphan": false,
-            "resources": []
-        },
-        "ListSites": {
+        "GetSiteAddress": {
             "access_level": "Undocumented",
-            "action": "ListSites",
+            "action": "GetSiteAddress",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListUsers": {
+        "DeleteSite": {
             "access_level": "Undocumented",
-            "action": "ListUsers",
+            "action": "DeleteSite",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "GetDeviceInstanceConfiguration": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "GetDeviceInstanceConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSite": {
+        "CreateDeviceInstanceConfiguration": {
             "access_level": "Undocumented",
-            "action": "GetSite",
+            "action": "CreateDeviceInstanceConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListDeviceConfigurationTemplates": {
+        "CreateDeviceInstance": {
             "access_level": "Undocumented",
-            "action": "ListDeviceConfigurationTemplates",
+            "action": "CreateDeviceInstance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "GetDeviceInstance": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "GetDeviceInstance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteDeviceConfigurationTemplate": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "DeleteDeviceConfigurationTemplate",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateDeviceInstance": {
+        "ListUsers": {
             "access_level": "Undocumented",
-            "action": "UpdateDeviceInstance",
+            "action": "ListUsers",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RebootDevice": {
+        "UpdateDeviceConfigurationTemplate": {
             "access_level": "Undocumented",
-            "action": "RebootDevice",
+            "action": "UpdateDeviceConfigurationTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DeleteAssociatedDevice": {
             "access_level": "Undocumented",
             "action": "DeleteAssociatedDevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetDeviceConfigurationTemplate": {
+        "UpdateSite": {
             "access_level": "Undocumented",
-            "action": "GetDeviceConfigurationTemplate",
+            "action": "UpdateSite",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateSite": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "CreateSite",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateDeviceInstance": {
+        "UpdateDeviceInstance": {
             "access_level": "Undocumented",
-            "action": "CreateDeviceInstance",
+            "action": "UpdateDeviceInstance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetDeviceInstance": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "GetDeviceInstance",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateDeviceConfigurationTemplate": {
+        "ListDeviceConfigurationTemplates": {
             "access_level": "Undocumented",
-            "action": "CreateDeviceConfigurationTemplate",
+            "action": "ListDeviceConfigurationTemplates",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetDeviceInstanceConfiguration": {
+        "ListSites": {
             "access_level": "Undocumented",
-            "action": "GetDeviceInstanceConfiguration",
+            "action": "ListSites",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteUser": {
+        "CreateDeviceActivationQrCode": {
             "access_level": "Undocumented",
-            "action": "DeleteUser",
+            "action": "CreateDeviceActivationQrCode",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListDeviceInstances": {
+        "CreateSite": {
             "access_level": "Undocumented",
-            "action": "ListDeviceInstances",
+            "action": "CreateSite",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "DeleteUser": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "DeleteUser",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSiteAddress": {
+        "GetSite": {
             "access_level": "Undocumented",
-            "action": "GetSiteAddress",
+            "action": "GetSite",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateSite": {
+        "ListDeviceInstances": {
             "access_level": "Undocumented",
-            "action": "UpdateSite",
+            "action": "ListDeviceInstances",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateDeviceInstanceConfiguration": {
+        "DeleteDeviceConfigurationTemplate": {
             "access_level": "Undocumented",
-            "action": "CreateDeviceInstanceConfiguration",
+            "action": "DeleteDeviceConfigurationTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "UpdateSiteAddress": {
             "access_level": "Undocumented",
             "action": "UpdateSiteAddress",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateDeviceActivationQrCode": {
+        "RebootDevice": {
             "access_level": "Undocumented",
-            "action": "CreateDeviceActivationQrCode",
+            "action": "RebootDevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteSite": {
+        "GetDeviceConfigurationTemplate": {
             "access_level": "Undocumented",
-            "action": "DeleteSite",
+            "action": "GetDeviceConfigurationTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DeleteDeviceInstance": {
             "access_level": "Undocumented",
             "action": "DeleteDeviceInstance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
+        },
+        "CreateDeviceConfigurationTemplate": {
+            "access_level": "Undocumented",
+            "action": "CreateDeviceConfigurationTemplate",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
         }
     },
     "opsworks": {
         "AssignInstance": {
             "access_level": "Write",
             "action": "AssignInstance",
             "condition_keys": [],
@@ -117823,129 +117823,129 @@
             "orphan": false,
             "resources": [
                 "policy"
             ]
         }
     },
     "osis": {
-        "DeletePipeline": {
+        "UpdatePipeline": {
             "access_level": "Undocumented",
-            "action": "DeletePipeline",
+            "action": "UpdatePipeline",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "GetPipelineBlueprint": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "GetPipelineBlueprint",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "CreatePipeline": {
             "access_level": "Undocumented",
             "action": "CreatePipeline",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPipelineBlueprints": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "ListPipelineBlueprints",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "GetPipeline": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "GetPipeline",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "Ingest": {
+        "DeletePipeline": {
             "access_level": "Undocumented",
-            "action": "Ingest",
+            "action": "DeletePipeline",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StopPipeline": {
+        "GetPipelineChangeProgress": {
             "access_level": "Undocumented",
-            "action": "StopPipeline",
+            "action": "GetPipelineChangeProgress",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ValidatePipeline": {
+        "ListPipelineBlueprints": {
             "access_level": "Undocumented",
-            "action": "ValidatePipeline",
+            "action": "ListPipelineBlueprints",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPipelines": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "ListPipelines",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "StartPipeline": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "StartPipeline",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPipeline": {
+        "Ingest": {
             "access_level": "Undocumented",
-            "action": "GetPipeline",
+            "action": "Ingest",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPipelineChangeProgress": {
+        "StopPipeline": {
             "access_level": "Undocumented",
-            "action": "GetPipelineChangeProgress",
+            "action": "StopPipeline",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPipelineBlueprint": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "GetPipelineBlueprint",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdatePipeline": {
+        "ListPipelines": {
             "access_level": "Undocumented",
-            "action": "UpdatePipeline",
+            "action": "ListPipelines",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartPipeline": {
+        "ValidatePipeline": {
             "access_level": "Undocumented",
-            "action": "StartPipeline",
+            "action": "ValidatePipeline",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "outposts": {
@@ -118568,535 +118568,535 @@
             "access_level": "Undocumented",
             "action": "DisassociatePartnerUser",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssociatePartnerAccount": {
+        "AssociatePartnerUser": {
             "access_level": "Undocumented",
-            "action": "AssociatePartnerAccount",
+            "action": "AssociatePartnerUser",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssociatePartnerUser": {
+        "AssociatePartnerAccount": {
             "access_level": "Undocumented",
-            "action": "AssociatePartnerUser",
+            "action": "AssociatePartnerAccount",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "payment-cryptography": {
-        "StopKeyUsage": {
+        "UpdateAlias": {
             "access_level": "Undocumented",
-            "action": "StopKeyUsage",
+            "action": "UpdateAlias",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "GetKey": {
             "access_level": "Undocumented",
             "action": "GetKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartKeyUsage": {
+        "GenerateMac": {
             "access_level": "Undocumented",
-            "action": "StartKeyUsage",
+            "action": "GenerateMac",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "VerifyMac": {
+        "CreateKey": {
             "access_level": "Undocumented",
-            "action": "VerifyMac",
+            "action": "CreateKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "EncryptData": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "EncryptData",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListKeys": {
+        "GeneratePinData": {
             "access_level": "Undocumented",
-            "action": "ListKeys",
+            "action": "GeneratePinData",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPublicKeyCertificate": {
+        "VerifyCardValidationData": {
             "access_level": "Undocumented",
-            "action": "GetPublicKeyCertificate",
+            "action": "VerifyCardValidationData",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteKey": {
+        "StartKeyUsage": {
             "access_level": "Undocumented",
-            "action": "DeleteKey",
+            "action": "StartKeyUsage",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateAlias": {
+        "ImportKey": {
             "access_level": "Undocumented",
-            "action": "CreateAlias",
+            "action": "ImportKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "ListAliases": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "ListAliases",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GeneratePinData": {
+        "DeleteAlias": {
             "access_level": "Undocumented",
-            "action": "GeneratePinData",
+            "action": "DeleteAlias",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DecryptData": {
+        "RestoreKey": {
             "access_level": "Undocumented",
-            "action": "DecryptData",
+            "action": "RestoreKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ReEncryptData": {
+        "GetAlias": {
             "access_level": "Undocumented",
-            "action": "ReEncryptData",
+            "action": "GetAlias",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RestoreKey": {
+        "DeleteKey": {
             "access_level": "Undocumented",
-            "action": "RestoreKey",
+            "action": "DeleteKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetParametersForExport": {
+        "ListKeys": {
             "access_level": "Undocumented",
-            "action": "GetParametersForExport",
+            "action": "ListKeys",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ImportKey": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "ImportKey",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetParametersForImport": {
+        "VerifyMac": {
             "access_level": "Undocumented",
-            "action": "GetParametersForImport",
+            "action": "VerifyMac",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAliases": {
+        "ReEncryptData": {
             "access_level": "Undocumented",
-            "action": "ListAliases",
+            "action": "ReEncryptData",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAlias": {
+        "GetParametersForExport": {
             "access_level": "Undocumented",
-            "action": "GetAlias",
+            "action": "GetParametersForExport",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GenerateMac": {
+        "VerifyPinData": {
             "access_level": "Undocumented",
-            "action": "GenerateMac",
+            "action": "VerifyPinData",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "VerifyAuthRequestCryptogram": {
+        "CreateAlias": {
             "access_level": "Undocumented",
-            "action": "VerifyAuthRequestCryptogram",
+            "action": "CreateAlias",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "ExportKey": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "ExportKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateKey": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "CreateKey",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "EncryptData": {
+        "TranslatePinData": {
             "access_level": "Undocumented",
-            "action": "EncryptData",
+            "action": "TranslatePinData",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ExportKey": {
+        "GetParametersForImport": {
             "access_level": "Undocumented",
-            "action": "ExportKey",
+            "action": "GetParametersForImport",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "VerifyPinData": {
+        "GetPublicKeyCertificate": {
             "access_level": "Undocumented",
-            "action": "VerifyPinData",
+            "action": "GetPublicKeyCertificate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateAlias": {
+        "DecryptData": {
             "access_level": "Undocumented",
-            "action": "UpdateAlias",
+            "action": "DecryptData",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteAlias": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "DeleteAlias",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "GenerateCardValidationData": {
             "access_level": "Undocumented",
             "action": "GenerateCardValidationData",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TranslatePinData": {
+        "VerifyAuthRequestCryptogram": {
             "access_level": "Undocumented",
-            "action": "TranslatePinData",
+            "action": "VerifyAuthRequestCryptogram",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "VerifyCardValidationData": {
+        "StopKeyUsage": {
             "access_level": "Undocumented",
-            "action": "VerifyCardValidationData",
+            "action": "StopKeyUsage",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "payments": {
-        "MakePayment": {
+        "CreatePaymentInstrument": {
             "access_level": "Undocumented",
-            "action": "MakePayment",
+            "action": "CreatePaymentInstrument",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeletePaymentInstrument": {
+        "GetPaymentInstrument": {
             "access_level": "Undocumented",
-            "action": "DeletePaymentInstrument",
+            "action": "GetPaymentInstrument",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreatePaymentInstrument": {
+        "DeletePaymentInstrument": {
             "access_level": "Undocumented",
-            "action": "CreatePaymentInstrument",
+            "action": "DeletePaymentInstrument",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPaymentPreferences": {
+        "MakePayment": {
             "access_level": "Undocumented",
-            "action": "ListPaymentPreferences",
+            "action": "MakePayment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "GetPaymentStatus": {
             "access_level": "Undocumented",
             "action": "GetPaymentStatus",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdatePaymentPreferences": {
+        "ListPaymentPreferences": {
             "access_level": "Undocumented",
-            "action": "UpdatePaymentPreferences",
+            "action": "ListPaymentPreferences",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPaymentInstrument": {
+        "UpdatePaymentPreferences": {
             "access_level": "Undocumented",
-            "action": "GetPaymentInstrument",
+            "action": "UpdatePaymentPreferences",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "pca-connector-ad": {
-        "ListTemplates": {
+        "GetDirectoryRegistration": {
             "access_level": "Undocumented",
-            "action": "ListTemplates",
+            "action": "GetDirectoryRegistration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateTemplateGroupAccessControlEntry": {
+        "GetTemplate": {
             "access_level": "Undocumented",
-            "action": "CreateTemplateGroupAccessControlEntry",
+            "action": "GetTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetConnector": {
+        "CreateDirectoryRegistration": {
             "access_level": "Undocumented",
-            "action": "GetConnector",
+            "action": "CreateDirectoryRegistration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetTemplateGroupAccessControlEntry": {
+        "DeleteTemplateGroupAccessControlEntry": {
             "access_level": "Undocumented",
-            "action": "GetTemplateGroupAccessControlEntry",
+            "action": "DeleteTemplateGroupAccessControlEntry",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetDirectoryRegistration": {
+        "CreateTemplateGroupAccessControlEntry": {
             "access_level": "Undocumented",
-            "action": "GetDirectoryRegistration",
+            "action": "CreateTemplateGroupAccessControlEntry",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "DeleteServicePrincipalName": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "DeleteServicePrincipalName",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateTemplateGroupAccessControlEntry": {
+        "ListConnectors": {
             "access_level": "Undocumented",
-            "action": "UpdateTemplateGroupAccessControlEntry",
+            "action": "ListConnectors",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteTemplateGroupAccessControlEntry": {
+        "ListTemplates": {
             "access_level": "Undocumented",
-            "action": "DeleteTemplateGroupAccessControlEntry",
+            "action": "ListTemplates",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateDirectoryRegistration": {
+        "ListTemplateGroupAccessControlEntries": {
             "access_level": "Undocumented",
-            "action": "CreateDirectoryRegistration",
+            "action": "ListTemplateGroupAccessControlEntries",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "UpdateTemplate": {
             "access_level": "Undocumented",
             "action": "UpdateTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteServicePrincipalName": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "DeleteServicePrincipalName",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "DeleteTemplate": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "DeleteTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetTemplate": {
+        "DeleteDirectoryRegistration": {
             "access_level": "Undocumented",
-            "action": "GetTemplate",
+            "action": "DeleteDirectoryRegistration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListServicePrincipalNames": {
+        "CreateTemplate": {
             "access_level": "Undocumented",
-            "action": "ListServicePrincipalNames",
+            "action": "CreateTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetServicePrincipalName": {
+        "DeleteConnector": {
             "access_level": "Undocumented",
-            "action": "GetServicePrincipalName",
+            "action": "DeleteConnector",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteTemplate": {
+        "CreateServicePrincipalName": {
             "access_level": "Undocumented",
-            "action": "DeleteTemplate",
+            "action": "CreateServicePrincipalName",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteDirectoryRegistration": {
+        "GetTemplateGroupAccessControlEntry": {
             "access_level": "Undocumented",
-            "action": "DeleteDirectoryRegistration",
+            "action": "GetTemplateGroupAccessControlEntry",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateConnector": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "CreateConnector",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListDirectoryRegistrations": {
+        "GetServicePrincipalName": {
             "access_level": "Undocumented",
-            "action": "ListDirectoryRegistrations",
+            "action": "GetServicePrincipalName",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateServicePrincipalName": {
+        "ListServicePrincipalNames": {
             "access_level": "Undocumented",
-            "action": "CreateServicePrincipalName",
+            "action": "ListServicePrincipalNames",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTemplateGroupAccessControlEntries": {
+        "UpdateTemplateGroupAccessControlEntry": {
             "access_level": "Undocumented",
-            "action": "ListTemplateGroupAccessControlEntries",
+            "action": "UpdateTemplateGroupAccessControlEntry",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListConnectors": {
+        "ListDirectoryRegistrations": {
             "access_level": "Undocumented",
-            "action": "ListConnectors",
+            "action": "ListDirectoryRegistrations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateTemplate": {
+        "CreateConnector": {
             "access_level": "Undocumented",
-            "action": "CreateTemplate",
+            "action": "CreateConnector",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteConnector": {
+        "GetConnector": {
             "access_level": "Undocumented",
-            "action": "DeleteConnector",
+            "action": "GetConnector",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "personalize": {
@@ -122425,555 +122425,555 @@
             "orphan": false,
             "resources": [
                 "purchase-order"
             ]
         }
     },
     "q": {
-        "GetTroubleshootingResults": {
+        "ListConversations": {
             "access_level": "Undocumented",
-            "action": "GetTroubleshootingResults",
+            "action": "ListConversations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SendMessage": {
+        "GetConversation": {
             "access_level": "Undocumented",
-            "action": "SendMessage",
+            "action": "GetConversation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListConversations": {
+        "StartTroubleshootingAnalysis": {
             "access_level": "Undocumented",
-            "action": "ListConversations",
+            "action": "StartTroubleshootingAnalysis",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartTroubleshootingAnalysis": {
+        "SendMessage": {
             "access_level": "Undocumented",
-            "action": "StartTroubleshootingAnalysis",
+            "action": "SendMessage",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "StartConversation": {
             "access_level": "Undocumented",
             "action": "StartConversation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartTroubleshootingResolutionExplanation": {
+        "GetTroubleshootingResults": {
             "access_level": "Undocumented",
-            "action": "StartTroubleshootingResolutionExplanation",
+            "action": "GetTroubleshootingResults",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetConversation": {
+        "StartTroubleshootingResolutionExplanation": {
             "access_level": "Undocumented",
-            "action": "GetConversation",
+            "action": "StartTroubleshootingResolutionExplanation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "qbusiness": {
-        "BatchPutDocument": {
+        "ListDocuments": {
             "access_level": "Undocumented",
-            "action": "BatchPutDocument",
+            "action": "ListDocuments",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteGroup": {
+        "ListGroups": {
             "access_level": "Undocumented",
-            "action": "DeleteGroup",
+            "action": "ListGroups",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateWebExperience": {
+        "DeleteRetriever": {
             "access_level": "Undocumented",
-            "action": "UpdateWebExperience",
+            "action": "DeleteRetriever",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListGroups": {
+        "UpdateApplication": {
             "access_level": "Undocumented",
-            "action": "ListGroups",
+            "action": "UpdateApplication",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPlugins": {
+        "RemoveUserLicenses": {
             "access_level": "Undocumented",
-            "action": "ListPlugins",
+            "action": "RemoveUserLicenses",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateIndex": {
+        "CreateDataSource": {
             "access_level": "Undocumented",
-            "action": "CreateIndex",
+            "action": "CreateDataSource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetDataSource": {
+        "ListRetrievers": {
             "access_level": "Undocumented",
-            "action": "GetDataSource",
+            "action": "ListRetrievers",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteRetriever": {
+        "UpdatePlugin": {
             "access_level": "Undocumented",
-            "action": "DeleteRetriever",
+            "action": "UpdatePlugin",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateDataSource": {
+        "UpdateWebExperience": {
             "access_level": "Undocumented",
-            "action": "CreateDataSource",
+            "action": "UpdateWebExperience",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPlugin": {
+        "DeleteApplication": {
             "access_level": "Undocumented",
-            "action": "GetPlugin",
+            "action": "DeleteApplication",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateChatControlsConfiguration": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "UpdateChatControlsConfiguration",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListIndices": {
+        "ListConversations": {
             "access_level": "Undocumented",
-            "action": "ListIndices",
+            "action": "ListConversations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListWebExperiences": {
+        "UpdateDataSource": {
             "access_level": "Undocumented",
-            "action": "ListWebExperiences",
+            "action": "UpdateDataSource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "CreateApplication": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "CreateApplication",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateIndex": {
+        "DeletePlugin": {
             "access_level": "Undocumented",
-            "action": "UpdateIndex",
+            "action": "DeletePlugin",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RemoveUserLicenses": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "RemoveUserLicenses",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ChatSync": {
+        "CreateIndex": {
             "access_level": "Undocumented",
-            "action": "ChatSync",
+            "action": "CreateIndex",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateApplication": {
+        "GetRetriever": {
             "access_level": "Undocumented",
-            "action": "CreateApplication",
+            "action": "GetRetriever",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetRetriever": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "GetRetriever",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListUserLicenses": {
+        "ListDataSources": {
             "access_level": "Undocumented",
-            "action": "ListUserLicenses",
+            "action": "ListDataSources",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartDataSourceSyncJob": {
+        "ListWebExperiences": {
             "access_level": "Undocumented",
-            "action": "StartDataSourceSyncJob",
+            "action": "ListWebExperiences",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreatePlugin": {
+        "CreateLicense": {
             "access_level": "Undocumented",
-            "action": "CreatePlugin",
+            "action": "CreateLicense",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteUser": {
+        "GetUser": {
             "access_level": "Undocumented",
-            "action": "DeleteUser",
+            "action": "GetUser",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateDataSource": {
+        "DeleteUser": {
             "access_level": "Undocumented",
-            "action": "UpdateDataSource",
+            "action": "DeleteUser",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListConversations": {
+        "ListPlugins": {
             "access_level": "Undocumented",
-            "action": "ListConversations",
+            "action": "ListPlugins",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutGroup": {
+        "UpdateUser": {
             "access_level": "Undocumented",
-            "action": "PutGroup",
+            "action": "UpdateUser",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateApplication": {
+        "ChatSync": {
             "access_level": "Undocumented",
-            "action": "UpdateApplication",
+            "action": "ChatSync",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdatePlugin": {
+        "BatchDeleteDocument": {
             "access_level": "Undocumented",
-            "action": "UpdatePlugin",
+            "action": "BatchDeleteDocument",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateWebExperience": {
+        "Chat": {
             "access_level": "Undocumented",
-            "action": "CreateWebExperience",
+            "action": "Chat",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetUser": {
+        "GetGroup": {
             "access_level": "Undocumented",
-            "action": "GetUser",
+            "action": "GetGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "ListIndices": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "ListIndices",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListMessages": {
+        "GetLicense": {
             "access_level": "Undocumented",
-            "action": "ListMessages",
+            "action": "GetLicense",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetWebExperience": {
+        "ListApplications": {
             "access_level": "Undocumented",
-            "action": "GetWebExperience",
+            "action": "ListApplications",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListDataSourceSyncJobs": {
+        "ListUserLicenses": {
             "access_level": "Undocumented",
-            "action": "ListDataSourceSyncJobs",
+            "action": "ListUserLicenses",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListRetrievers": {
+        "PutGroup": {
             "access_level": "Undocumented",
-            "action": "ListRetrievers",
+            "action": "PutGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetApplication": {
+        "GetDataSource": {
             "access_level": "Undocumented",
-            "action": "GetApplication",
+            "action": "GetDataSource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateLicense": {
+        "CreateRetriever": {
             "access_level": "Undocumented",
-            "action": "CreateLicense",
+            "action": "CreateRetriever",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetGroup": {
+        "GetChatControlsConfiguration": {
             "access_level": "Undocumented",
-            "action": "GetGroup",
+            "action": "GetChatControlsConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListDataSources": {
+        "DeleteDataSource": {
             "access_level": "Undocumented",
-            "action": "ListDataSources",
+            "action": "DeleteDataSource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteWebExperience": {
+        "UpdateRetriever": {
             "access_level": "Undocumented",
-            "action": "DeleteWebExperience",
+            "action": "UpdateRetriever",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetLicense": {
+        "UpdateChatControlsConfiguration": {
             "access_level": "Undocumented",
-            "action": "GetLicense",
+            "action": "UpdateChatControlsConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AddUserLicenses": {
+        "CreateWebExperience": {
             "access_level": "Undocumented",
-            "action": "AddUserLicenses",
+            "action": "CreateWebExperience",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeletePlugin": {
+        "AddUserLicenses": {
             "access_level": "Undocumented",
-            "action": "DeletePlugin",
+            "action": "AddUserLicenses",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetChatControlsConfiguration": {
+        "BatchPutDocument": {
             "access_level": "Undocumented",
-            "action": "GetChatControlsConfiguration",
+            "action": "BatchPutDocument",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteConversation": {
+        "ListMessages": {
             "access_level": "Undocumented",
-            "action": "DeleteConversation",
+            "action": "ListMessages",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutFeedback": {
+        "GetIndex": {
             "access_level": "Undocumented",
-            "action": "PutFeedback",
+            "action": "GetIndex",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateRetriever": {
+        "CreatePlugin": {
             "access_level": "Undocumented",
-            "action": "UpdateRetriever",
+            "action": "CreatePlugin",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateUser": {
+        "DeleteGroup": {
             "access_level": "Undocumented",
-            "action": "UpdateUser",
+            "action": "DeleteGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListDocuments": {
+        "PutFeedback": {
             "access_level": "Undocumented",
-            "action": "ListDocuments",
+            "action": "PutFeedback",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StopDataSourceSyncJob": {
+        "GetPlugin": {
             "access_level": "Undocumented",
-            "action": "StopDataSourceSyncJob",
+            "action": "GetPlugin",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteDataSource": {
+        "StopDataSourceSyncJob": {
             "access_level": "Undocumented",
-            "action": "DeleteDataSource",
+            "action": "StopDataSourceSyncJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateRetriever": {
+        "DeleteChatControlsConfiguration": {
             "access_level": "Undocumented",
-            "action": "CreateRetriever",
+            "action": "DeleteChatControlsConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "DeleteIndex": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "DeleteIndex",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteChatControlsConfiguration": {
+        "ListDataSourceSyncJobs": {
             "access_level": "Undocumented",
-            "action": "DeleteChatControlsConfiguration",
+            "action": "ListDataSourceSyncJobs",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "BatchDeleteDocument": {
+        "StartDataSourceSyncJob": {
             "access_level": "Undocumented",
-            "action": "BatchDeleteDocument",
+            "action": "StartDataSourceSyncJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteApplication": {
+        "GetWebExperience": {
             "access_level": "Undocumented",
-            "action": "DeleteApplication",
+            "action": "GetWebExperience",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "Chat": {
+        "UpdateIndex": {
             "access_level": "Undocumented",
-            "action": "Chat",
+            "action": "UpdateIndex",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateUser": {
+        "GetApplication": {
             "access_level": "Undocumented",
-            "action": "CreateUser",
+            "action": "GetApplication",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetIndex": {
+        "DeleteWebExperience": {
             "access_level": "Undocumented",
-            "action": "GetIndex",
+            "action": "DeleteWebExperience",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteIndex": {
+        "DeleteConversation": {
             "access_level": "Undocumented",
-            "action": "DeleteIndex",
+            "action": "DeleteConversation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListApplications": {
+        "CreateUser": {
             "access_level": "Undocumented",
-            "action": "ListApplications",
+            "action": "CreateUser",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "qldb": {
@@ -125422,281 +125422,281 @@
             "orphan": false,
             "resources": [
                 "vpcconnection"
             ]
         }
     },
     "ram": {
-        "ListPendingInvitationResources": {
+        "ListPermissionVersions": {
             "access_level": "Undocumented",
-            "action": "ListPendingInvitationResources",
+            "action": "ListPermissionVersions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeletePermission": {
+        "AcceptResourceShareInvitation": {
             "access_level": "Undocumented",
-            "action": "DeletePermission",
+            "action": "AcceptResourceShareInvitation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetResourcePolicies": {
+        "DisassociateResourceShare": {
             "access_level": "Undocumented",
-            "action": "GetResourcePolicies",
+            "action": "DisassociateResourceShare",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "GetResourceShares": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "GetResourceShares",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteResourceShare": {
+        "GetResourceShareAssociations": {
             "access_level": "Undocumented",
-            "action": "DeleteResourceShare",
+            "action": "GetResourceShareAssociations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPermissions": {
+        "CreateResourceShare": {
             "access_level": "Undocumented",
-            "action": "ListPermissions",
+            "action": "CreateResourceShare",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListResourceTypes": {
+        "EnableSharingWithAwsOrganization": {
             "access_level": "Undocumented",
-            "action": "ListResourceTypes",
+            "action": "EnableSharingWithAwsOrganization",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListReplacePermissionAssociationsWork": {
+        "DisassociateResourceSharePermission": {
             "access_level": "Undocumented",
-            "action": "ListReplacePermissionAssociationsWork",
+            "action": "DisassociateResourceSharePermission",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateResourceShare": {
+        "ListPendingInvitationResources": {
             "access_level": "Undocumented",
-            "action": "UpdateResourceShare",
+            "action": "ListPendingInvitationResources",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListResourceSharePermissions": {
+        "ListResourceTypes": {
             "access_level": "Undocumented",
-            "action": "ListResourceSharePermissions",
+            "action": "ListResourceTypes",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPermissionVersions": {
+        "SetDefaultPermissionVersion": {
             "access_level": "Undocumented",
-            "action": "ListPermissionVersions",
+            "action": "SetDefaultPermissionVersion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ReplacePermissionAssociations": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "ReplacePermissionAssociations",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DisassociateResourceSharePermission": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "DisassociateResourceSharePermission",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateResourceShare": {
+        "DeletePermission": {
             "access_level": "Undocumented",
-            "action": "CreateResourceShare",
+            "action": "DeletePermission",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPrincipals": {
+        "ListPermissionAssociations": {
             "access_level": "Undocumented",
-            "action": "ListPrincipals",
+            "action": "ListPermissionAssociations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetResourceShareAssociations": {
+        "PromoteResourceShareCreatedFromPolicy": {
             "access_level": "Undocumented",
-            "action": "GetResourceShareAssociations",
+            "action": "PromoteResourceShareCreatedFromPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListResources": {
+        "AssociateResourceShare": {
             "access_level": "Undocumented",
-            "action": "ListResources",
+            "action": "AssociateResourceShare",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SetDefaultPermissionVersion": {
+        "CreatePermissionVersion": {
             "access_level": "Undocumented",
-            "action": "SetDefaultPermissionVersion",
+            "action": "CreatePermissionVersion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "EnableSharingWithAwsOrganization": {
+        "RejectResourceShareInvitation": {
             "access_level": "Undocumented",
-            "action": "EnableSharingWithAwsOrganization",
+            "action": "RejectResourceShareInvitation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetResourceShareInvitations": {
+        "CreatePermission": {
             "access_level": "Undocumented",
-            "action": "GetResourceShareInvitations",
+            "action": "CreatePermission",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreatePermissionVersion": {
+        "ListResources": {
             "access_level": "Undocumented",
-            "action": "CreatePermissionVersion",
+            "action": "ListResources",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPermissionAssociations": {
+        "ListReplacePermissionAssociationsWork": {
             "access_level": "Undocumented",
-            "action": "ListPermissionAssociations",
+            "action": "ListReplacePermissionAssociationsWork",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PromoteResourceShareCreatedFromPolicy": {
+        "GetResourceShareInvitations": {
             "access_level": "Undocumented",
-            "action": "PromoteResourceShareCreatedFromPolicy",
+            "action": "GetResourceShareInvitations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreatePermission": {
+        "DeleteResourceShare": {
             "access_level": "Undocumented",
-            "action": "CreatePermission",
+            "action": "DeleteResourceShare",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PromotePermissionCreatedFromPolicy": {
+        "GetResourcePolicies": {
             "access_level": "Undocumented",
-            "action": "PromotePermissionCreatedFromPolicy",
+            "action": "GetResourcePolicies",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RejectResourceShareInvitation": {
+        "PromotePermissionCreatedFromPolicy": {
             "access_level": "Undocumented",
-            "action": "RejectResourceShareInvitation",
+            "action": "PromotePermissionCreatedFromPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeletePermissionVersion": {
+        "ListResourceSharePermissions": {
             "access_level": "Undocumented",
-            "action": "DeletePermissionVersion",
+            "action": "ListResourceSharePermissions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetResourceShares": {
+        "DeletePermissionVersion": {
             "access_level": "Undocumented",
-            "action": "GetResourceShares",
+            "action": "DeletePermissionVersion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssociateResourceShare": {
+        "ReplacePermissionAssociations": {
             "access_level": "Undocumented",
-            "action": "AssociateResourceShare",
+            "action": "ReplacePermissionAssociations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "AssociateResourceSharePermission": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "AssociateResourceSharePermission",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DisassociateResourceShare": {
+        "ListPrincipals": {
             "access_level": "Undocumented",
-            "action": "DisassociateResourceShare",
+            "action": "ListPrincipals",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPermission": {
+        "UpdateResourceShare": {
             "access_level": "Undocumented",
-            "action": "GetPermission",
+            "action": "UpdateResourceShare",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssociateResourceSharePermission": {
+        "GetPermission": {
             "access_level": "Undocumented",
-            "action": "AssociateResourceSharePermission",
+            "action": "GetPermission",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AcceptResourceShareInvitation": {
+        "ListPermissions": {
             "access_level": "Undocumented",
-            "action": "AcceptResourceShareInvitation",
+            "action": "ListPermissions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "rbin": {
@@ -131078,557 +131078,557 @@
             "orphan": false,
             "resources": [
                 "streamprocessor"
             ]
         }
     },
     "repostspace": {
-        "DeregisterAdmin": {
-            "access_level": "Undocumented",
-            "action": "DeregisterAdmin",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
-            "orphan": false,
-            "resources": []
-        },
-        "ListTagsForResource": {
+        "UpdateSpace": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "UpdateSpace",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "ListSpaces": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "ListSpaces",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteSpace": {
+        "DeregisterAdmin": {
             "access_level": "Undocumented",
-            "action": "DeleteSpace",
+            "action": "DeregisterAdmin",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "UntagResource": {
             "access_level": "Undocumented",
             "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSpace": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "GetSpace",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "SendInvites": {
             "access_level": "Undocumented",
             "action": "SendInvites",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateSpace": {
+        "CreateSpace": {
             "access_level": "Undocumented",
-            "action": "UpdateSpace",
+            "action": "CreateSpace",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateSpace": {
+        "DeleteSpace": {
             "access_level": "Undocumented",
-            "action": "CreateSpace",
+            "action": "DeleteSpace",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "RegisterAdmin": {
             "access_level": "Undocumented",
             "action": "RegisterAdmin",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSpaces": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "ListSpaces",
+            "action": "TagResource",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "GetSpace": {
+            "access_level": "Undocumented",
+            "action": "GetSpace",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "resiliencehub": {
-        "UpdateAppVersion": {
+        "ListAppVersionResources": {
             "access_level": "Undocumented",
-            "action": "UpdateAppVersion",
+            "action": "ListAppVersionResources",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAppVersionResourceMappings": {
+        "DeleteAppAssessment": {
             "access_level": "Undocumented",
-            "action": "ListAppVersionResourceMappings",
+            "action": "DeleteAppAssessment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListApps": {
+        "ListTestRecommendations": {
             "access_level": "Undocumented",
-            "action": "ListApps",
+            "action": "ListTestRecommendations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateAppVersionResource": {
+        "AddDraftAppVersionResourceMappings": {
             "access_level": "Undocumented",
-            "action": "CreateAppVersionResource",
+            "action": "AddDraftAppVersionResourceMappings",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateAppVersionAppComponent": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "CreateAppVersionAppComponent",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RemoveDraftAppVersionResourceMappings": {
+        "ListResiliencyPolicies": {
             "access_level": "Undocumented",
-            "action": "RemoveDraftAppVersionResourceMappings",
+            "action": "ListResiliencyPolicies",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeAppAssessment": {
+        "RemoveDraftAppVersionResourceMappings": {
             "access_level": "Undocumented",
-            "action": "DescribeAppAssessment",
+            "action": "RemoveDraftAppVersionResourceMappings",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteAppVersionResource": {
+        "DescribeAppVersionResourcesResolutionStatus": {
             "access_level": "Undocumented",
-            "action": "DeleteAppVersionResource",
+            "action": "DescribeAppVersionResourcesResolutionStatus",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeResiliencyPolicy": {
+        "CreateAppVersionAppComponent": {
             "access_level": "Undocumented",
-            "action": "DescribeResiliencyPolicy",
+            "action": "CreateAppVersionAppComponent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateApp": {
+        "DescribeDraftAppVersionResourcesImportStatus": {
             "access_level": "Undocumented",
-            "action": "CreateApp",
+            "action": "DescribeDraftAppVersionResourcesImportStatus",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeAppVersionAppComponent": {
+        "ResolveAppVersionResources": {
             "access_level": "Undocumented",
-            "action": "DescribeAppVersionAppComponent",
+            "action": "ResolveAppVersionResources",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteAppAssessment": {
+        "ListAppInputSources": {
             "access_level": "Undocumented",
-            "action": "DeleteAppAssessment",
+            "action": "ListAppInputSources",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "UntagResource": {
             "access_level": "Undocumented",
             "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAppInputSources": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "ListAppInputSources",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAppComponentRecommendations": {
+        "DeleteApp": {
             "access_level": "Undocumented",
-            "action": "ListAppComponentRecommendations",
+            "action": "DeleteApp",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListResiliencyPolicies": {
+        "DescribeAppAssessment": {
             "access_level": "Undocumented",
-            "action": "ListResiliencyPolicies",
+            "action": "DescribeAppAssessment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PublishAppVersion": {
+        "UpdateAppVersion": {
             "access_level": "Undocumented",
-            "action": "PublishAppVersion",
+            "action": "UpdateAppVersion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeApp": {
+        "ListAppVersionResourceMappings": {
             "access_level": "Undocumented",
-            "action": "DescribeApp",
+            "action": "ListAppVersionResourceMappings",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateAppVersionResource": {
+        "ListApps": {
             "access_level": "Undocumented",
-            "action": "UpdateAppVersionResource",
+            "action": "ListApps",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAppComponentCompliances": {
+        "PublishAppVersion": {
             "access_level": "Undocumented",
-            "action": "ListAppComponentCompliances",
+            "action": "PublishAppVersion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAppAssessments": {
+        "ListAppComponentCompliances": {
             "access_level": "Undocumented",
-            "action": "ListAppAssessments",
+            "action": "ListAppComponentCompliances",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSuggestedResiliencyPolicies": {
+        "DescribeResiliencyPolicy": {
             "access_level": "Undocumented",
-            "action": "ListSuggestedResiliencyPolicies",
+            "action": "DescribeResiliencyPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartAppAssessment": {
+        "ListAppVersions": {
             "access_level": "Undocumented",
-            "action": "StartAppAssessment",
+            "action": "ListAppVersions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteAppVersionAppComponent": {
+        "ListAppAssessments": {
             "access_level": "Undocumented",
-            "action": "DeleteAppVersionAppComponent",
+            "action": "ListAppAssessments",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeDraftAppVersionResourcesImportStatus": {
+        "UpdateApp": {
             "access_level": "Undocumented",
-            "action": "DescribeDraftAppVersionResourcesImportStatus",
+            "action": "UpdateApp",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAppVersionAppComponents": {
+        "ListUnsupportedAppVersionResources": {
             "access_level": "Undocumented",
-            "action": "ListAppVersionAppComponents",
+            "action": "ListUnsupportedAppVersionResources",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteApp": {
+        "DeleteAppVersionResource": {
             "access_level": "Undocumented",
-            "action": "DeleteApp",
+            "action": "DeleteAppVersionResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ImportResourcesToDraftAppVersion": {
+        "UpdateAppVersionAppComponent": {
             "access_level": "Undocumented",
-            "action": "ImportResourcesToDraftAppVersion",
+            "action": "UpdateAppVersionAppComponent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListRecommendationTemplates": {
+        "DescribeAppVersionResource": {
             "access_level": "Undocumented",
-            "action": "ListRecommendationTemplates",
+            "action": "DescribeAppVersionResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutDraftAppVersionTemplate": {
+        "CreateAppVersionResource": {
             "access_level": "Undocumented",
-            "action": "PutDraftAppVersionTemplate",
+            "action": "CreateAppVersionResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteAppInputSource": {
+        "DeleteAppVersionAppComponent": {
             "access_level": "Undocumented",
-            "action": "DeleteAppInputSource",
+            "action": "DeleteAppVersionAppComponent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateResiliencyPolicy": {
+        "ListAlarmRecommendations": {
             "access_level": "Undocumented",
-            "action": "CreateResiliencyPolicy",
+            "action": "ListAlarmRecommendations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "BatchUpdateRecommendationStatus": {
+        "CreateApp": {
             "access_level": "Undocumented",
-            "action": "BatchUpdateRecommendationStatus",
+            "action": "CreateApp",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "ListSuggestedResiliencyPolicies": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "ListSuggestedResiliencyPolicies",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteRecommendationTemplate": {
+        "UpdateResiliencyPolicy": {
             "access_level": "Undocumented",
-            "action": "DeleteRecommendationTemplate",
+            "action": "UpdateResiliencyPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "ListSopRecommendations": {
             "access_level": "Undocumented",
             "action": "ListSopRecommendations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeAppVersionTemplate": {
+        "DescribeAppVersion": {
             "access_level": "Undocumented",
-            "action": "DescribeAppVersionTemplate",
+            "action": "DescribeAppVersion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateApp": {
+        "ImportResourcesToDraftAppVersion": {
             "access_level": "Undocumented",
-            "action": "UpdateApp",
+            "action": "ImportResourcesToDraftAppVersion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteResiliencyPolicy": {
+        "UpdateAppVersionResource": {
             "access_level": "Undocumented",
-            "action": "DeleteResiliencyPolicy",
+            "action": "UpdateAppVersionResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListUnsupportedAppVersionResources": {
+        "ListRecommendationTemplates": {
             "access_level": "Undocumented",
-            "action": "ListUnsupportedAppVersionResources",
+            "action": "ListRecommendationTemplates",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateAppVersionAppComponent": {
+        "CreateRecommendationTemplate": {
             "access_level": "Undocumented",
-            "action": "UpdateAppVersionAppComponent",
+            "action": "CreateRecommendationTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAppVersions": {
+        "DeleteRecommendationTemplate": {
             "access_level": "Undocumented",
-            "action": "ListAppVersions",
+            "action": "DeleteRecommendationTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAppAssessmentComplianceDrifts": {
+        "ListAppComponentRecommendations": {
             "access_level": "Undocumented",
-            "action": "ListAppAssessmentComplianceDrifts",
+            "action": "ListAppComponentRecommendations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeAppVersion": {
+        "DescribeAppVersionAppComponent": {
             "access_level": "Undocumented",
-            "action": "DescribeAppVersion",
+            "action": "DescribeAppVersionAppComponent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "DescribeApp": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "DescribeApp",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateResiliencyPolicy": {
+        "ListAppAssessmentComplianceDrifts": {
             "access_level": "Undocumented",
-            "action": "UpdateResiliencyPolicy",
+            "action": "ListAppAssessmentComplianceDrifts",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeAppVersionResource": {
+        "CreateResiliencyPolicy": {
             "access_level": "Undocumented",
-            "action": "DescribeAppVersionResource",
+            "action": "CreateResiliencyPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeAppVersionResourcesResolutionStatus": {
+        "StartAppAssessment": {
             "access_level": "Undocumented",
-            "action": "DescribeAppVersionResourcesResolutionStatus",
+            "action": "StartAppAssessment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAppVersionResources": {
+        "DeleteAppInputSource": {
             "access_level": "Undocumented",
-            "action": "ListAppVersionResources",
+            "action": "DeleteAppInputSource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ResolveAppVersionResources": {
+        "DescribeAppVersionTemplate": {
             "access_level": "Undocumented",
-            "action": "ResolveAppVersionResources",
+            "action": "DescribeAppVersionTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AddDraftAppVersionResourceMappings": {
+        "BatchUpdateRecommendationStatus": {
             "access_level": "Undocumented",
-            "action": "AddDraftAppVersionResourceMappings",
+            "action": "BatchUpdateRecommendationStatus",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAlarmRecommendations": {
+        "DeleteResiliencyPolicy": {
             "access_level": "Undocumented",
-            "action": "ListAlarmRecommendations",
+            "action": "DeleteResiliencyPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTestRecommendations": {
+        "ListAppVersionAppComponents": {
             "access_level": "Undocumented",
-            "action": "ListTestRecommendations",
+            "action": "ListAppVersionAppComponents",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateRecommendationTemplate": {
+        "PutDraftAppVersionTemplate": {
             "access_level": "Undocumented",
-            "action": "CreateRecommendationTemplate",
+            "action": "PutDraftAppVersionTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "resource-explorer": {
-        "ListResources": {
+        "ListResourceTypes": {
             "access_level": "Undocumented",
-            "action": "ListResources",
+            "action": "ListResourceTypes",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTags": {
+        "ListResources": {
             "access_level": "Undocumented",
-            "action": "ListTags",
+            "action": "ListResources",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListResourceTypes": {
+        "ListTags": {
             "access_level": "Undocumented",
-            "action": "ListResourceTypes",
+            "action": "ListTags",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "resource-explorer-2": {
@@ -139583,49 +139583,49 @@
             "orphan": false,
             "resources": [
                 "object"
             ]
         }
     },
     "s3express": {
-        "ListAllMyDirectoryBuckets": {
+        "DeleteBucket": {
             "access_level": "Undocumented",
-            "action": "ListAllMyDirectoryBuckets",
+            "action": "DeleteBucket",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteBucket": {
+        "ListAllMyDirectoryBuckets": {
             "access_level": "Undocumented",
-            "action": "DeleteBucket",
+            "action": "ListAllMyDirectoryBuckets",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateSession": {
+        "GetBucketPolicy": {
             "access_level": "Undocumented",
-            "action": "CreateSession",
+            "action": "GetBucketPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateBucket": {
+        "CreateSession": {
             "access_level": "Undocumented",
-            "action": "CreateBucket",
+            "action": "CreateSession",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetBucketPolicy": {
+        "CreateBucket": {
             "access_level": "Undocumented",
-            "action": "GetBucketPolicy",
+            "action": "CreateBucket",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DeleteBucketPolicy": {
             "access_level": "Undocumented",
@@ -144422,129 +144422,129 @@
             "orphan": false,
             "resources": [
                 "schema"
             ]
         }
     },
     "scn": {
-        "RemoveAdminPermissionsForUser": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "RemoveAdminPermissionsForUser",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetBillOfMaterialsImportJob": {
+        "AssignAdminPermissionsToUser": {
             "access_level": "Undocumented",
-            "action": "GetBillOfMaterialsImportJob",
+            "action": "AssignAdminPermissionsToUser",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateInstance": {
+        "CreateBillOfMaterialsImportJob": {
             "access_level": "Undocumented",
-            "action": "UpdateInstance",
+            "action": "CreateBillOfMaterialsImportJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "ListInstances": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "ListInstances",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateInstance": {
+        "UpdateInstance": {
             "access_level": "Undocumented",
-            "action": "CreateInstance",
+            "action": "UpdateInstance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssignAdminPermissionsToUser": {
+        "DeleteSSOApplication": {
             "access_level": "Undocumented",
-            "action": "AssignAdminPermissionsToUser",
+            "action": "DeleteSSOApplication",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAdminUsers": {
+        "CreateSSOApplication": {
             "access_level": "Undocumented",
-            "action": "ListAdminUsers",
+            "action": "CreateSSOApplication",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "DescribeInstance": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "DescribeInstance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeInstance": {
+        "DeleteInstance": {
             "access_level": "Undocumented",
-            "action": "DescribeInstance",
+            "action": "DeleteInstance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteInstance": {
+        "GetBillOfMaterialsImportJob": {
             "access_level": "Undocumented",
-            "action": "DeleteInstance",
+            "action": "GetBillOfMaterialsImportJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteSSOApplication": {
+        "CreateInstance": {
             "access_level": "Undocumented",
-            "action": "DeleteSSOApplication",
+            "action": "CreateInstance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateBillOfMaterialsImportJob": {
+        "RemoveAdminPermissionsForUser": {
             "access_level": "Undocumented",
-            "action": "CreateBillOfMaterialsImportJob",
+            "action": "RemoveAdminPermissionsForUser",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListInstances": {
+        "ListAdminUsers": {
             "access_level": "Undocumented",
-            "action": "ListInstances",
+            "action": "ListAdminUsers",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateSSOApplication": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "CreateSSOApplication",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "sdb": {
@@ -155551,41 +155551,41 @@
             "condition_keys": [],
             "description": "Grants permission to update the HANA backup settings of a specified database",
             "orphan": false,
             "resources": []
         }
     },
     "ssmmessages": {
-        "CreateControlChannel": {
+        "OpenControlChannel": {
             "access_level": "Undocumented",
-            "action": "CreateControlChannel",
+            "action": "OpenControlChannel",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "OpenControlChannel": {
+        "CreateDataChannel": {
             "access_level": "Undocumented",
-            "action": "OpenControlChannel",
+            "action": "CreateDataChannel",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "OpenDataChannel": {
+        "CreateControlChannel": {
             "access_level": "Undocumented",
-            "action": "OpenDataChannel",
+            "action": "CreateControlChannel",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateDataChannel": {
+        "OpenDataChannel": {
             "access_level": "Undocumented",
-            "action": "CreateDataChannel",
+            "action": "OpenDataChannel",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "sso": {
@@ -160401,145 +160401,145 @@
             "orphan": false,
             "resources": [
                 "adapter"
             ]
         }
     },
     "thinclient": {
-        "UpdateEnvironment": {
+        "DeregisterDevice": {
             "access_level": "Undocumented",
-            "action": "UpdateEnvironment",
+            "action": "DeregisterDevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSoftwareSets": {
+        "GetDevice": {
             "access_level": "Undocumented",
-            "action": "ListSoftwareSets",
+            "action": "GetDevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "DeleteEnvironment": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "DeleteEnvironment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSoftwareSet": {
+        "ListEnvironments": {
             "access_level": "Undocumented",
-            "action": "GetSoftwareSet",
+            "action": "ListEnvironments",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteDevice": {
+        "CreateEnvironment": {
             "access_level": "Undocumented",
-            "action": "DeleteDevice",
+            "action": "CreateEnvironment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "GetEnvironment": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "GetEnvironment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListDeviceSessions": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "ListDeviceSessions",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListEnvironments": {
+        "DeleteDevice": {
             "access_level": "Undocumented",
-            "action": "ListEnvironments",
+            "action": "DeleteDevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateSoftwareSet": {
+        "GetSoftwareSet": {
             "access_level": "Undocumented",
-            "action": "UpdateSoftwareSet",
+            "action": "GetSoftwareSet",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetEnvironment": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "GetEnvironment",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetDevice": {
+        "UpdateSoftwareSet": {
             "access_level": "Undocumented",
-            "action": "GetDevice",
+            "action": "UpdateSoftwareSet",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteEnvironment": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "DeleteEnvironment",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "ListDeviceSessions": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "ListDeviceSessions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateEnvironment": {
+        "ListDevices": {
             "access_level": "Undocumented",
-            "action": "CreateEnvironment",
+            "action": "ListDevices",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeregisterDevice": {
+        "UpdateDevice": {
             "access_level": "Undocumented",
-            "action": "DeregisterDevice",
+            "action": "UpdateDevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateDevice": {
+        "ListSoftwareSets": {
             "access_level": "Undocumented",
-            "action": "UpdateDevice",
+            "action": "ListSoftwareSets",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListDevices": {
+        "UpdateEnvironment": {
             "access_level": "Undocumented",
-            "action": "ListDevices",
+            "action": "UpdateEnvironment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "timestream": {
@@ -160897,89 +160897,89 @@
             "access_level": "Undocumented",
             "action": "CreateDbInstance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetDbInstance": {
+        "UpdateDbInstance": {
             "access_level": "Undocumented",
-            "action": "GetDbInstance",
+            "action": "UpdateDbInstance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateDbInstance": {
+        "CreateDbParameterGroup": {
             "access_level": "Undocumented",
-            "action": "UpdateDbInstance",
+            "action": "CreateDbParameterGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "ListDbParameterGroups": {
             "access_level": "Undocumented",
             "action": "ListDbParameterGroups",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "DeleteDbInstance": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "DeleteDbInstance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteDbInstance": {
+        "ListDbInstances": {
             "access_level": "Undocumented",
-            "action": "DeleteDbInstance",
+            "action": "ListDbInstances",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListDbInstances": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "ListDbInstances",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "GetDbParameterGroup": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "GetDbParameterGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateDbParameterGroup": {
+        "GetDbInstance": {
             "access_level": "Undocumented",
-            "action": "CreateDbParameterGroup",
+            "action": "GetDbInstance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetDbParameterGroup": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "GetDbParameterGroup",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "tiros": {
@@ -161021,121 +161021,113 @@
             "condition_keys": [],
             "description": "Grants permission to list accounts that might be useful in a new query",
             "orphan": false,
             "resources": []
         }
     },
     "tnb": {
-        "CreateSolNetworkInstance": {
-            "access_level": "Undocumented",
-            "action": "CreateSolNetworkInstance",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
-            "orphan": false,
-            "resources": []
-        },
-        "UpdateSolNetworkInstance": {
+        "UpdateSolNetworkPackage": {
             "access_level": "Undocumented",
-            "action": "UpdateSolNetworkInstance",
+            "action": "UpdateSolNetworkPackage",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSolNetworkPackageContent": {
+        "PutSolFunctionPackageContent": {
             "access_level": "Undocumented",
-            "action": "GetSolNetworkPackageContent",
+            "action": "PutSolFunctionPackageContent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSolFunctionPackageContent": {
+        "ValidateSolFunctionPackageContent": {
             "access_level": "Undocumented",
-            "action": "GetSolFunctionPackageContent",
+            "action": "ValidateSolFunctionPackageContent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "CreateSolFunctionPackage": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "CreateSolFunctionPackage",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteSolNetworkPackage": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "DeleteSolNetworkPackage",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ValidateSolNetworkPackageContent": {
+        "ListSolFunctionPackages": {
             "access_level": "Undocumented",
-            "action": "ValidateSolNetworkPackageContent",
+            "action": "ListSolFunctionPackages",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutSolNetworkPackageContent": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "PutSolNetworkPackageContent",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CancelSolNetworkOperation": {
+        "UpdateSolNetworkInstance": {
             "access_level": "Undocumented",
-            "action": "CancelSolNetworkOperation",
+            "action": "UpdateSolNetworkInstance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TerminateSolNetworkInstance": {
+        "GetSolNetworkPackageDescriptor": {
             "access_level": "Undocumented",
-            "action": "TerminateSolNetworkInstance",
+            "action": "GetSolNetworkPackageDescriptor",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateSolNetworkPackage": {
+        "GetSolFunctionPackageDescriptor": {
             "access_level": "Undocumented",
-            "action": "UpdateSolNetworkPackage",
+            "action": "GetSolFunctionPackageDescriptor",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateSolFunctionPackage": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "UpdateSolFunctionPackage",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "GetSolNetworkOperation": {
             "access_level": "Undocumented",
             "action": "GetSolNetworkOperation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteSolNetworkInstance": {
+        "DeleteSolNetworkPackage": {
             "access_level": "Undocumented",
-            "action": "DeleteSolNetworkInstance",
+            "action": "DeleteSolNetworkPackage",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "ListSolNetworkOperations": {
             "access_level": "Undocumented",
@@ -161149,145 +161141,153 @@
             "access_level": "Undocumented",
             "action": "GetSolFunctionInstance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateSolFunctionPackage": {
+        "ListSolNetworkPackages": {
             "access_level": "Undocumented",
-            "action": "CreateSolFunctionPackage",
+            "action": "ListSolNetworkPackages",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSolFunctionPackageDescriptor": {
+        "UpdateSolFunctionPackage": {
             "access_level": "Undocumented",
-            "action": "GetSolFunctionPackageDescriptor",
+            "action": "UpdateSolFunctionPackage",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "TerminateSolNetworkInstance": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "TerminateSolNetworkInstance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSolNetworkInstances": {
+        "CancelSolNetworkOperation": {
             "access_level": "Undocumented",
-            "action": "ListSolNetworkInstances",
+            "action": "CancelSolNetworkOperation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSolFunctionInstances": {
+        "CreateSolNetworkPackage": {
             "access_level": "Undocumented",
-            "action": "ListSolFunctionInstances",
+            "action": "CreateSolNetworkPackage",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSolNetworkPackage": {
+        "InstantiateSolNetworkInstance": {
             "access_level": "Undocumented",
-            "action": "GetSolNetworkPackage",
+            "action": "InstantiateSolNetworkInstance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSolNetworkInstance": {
+        "DeleteSolFunctionPackage": {
             "access_level": "Undocumented",
-            "action": "GetSolNetworkInstance",
+            "action": "DeleteSolFunctionPackage",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSolFunctionPackage": {
+        "ListSolNetworkInstances": {
             "access_level": "Undocumented",
-            "action": "GetSolFunctionPackage",
+            "action": "ListSolNetworkInstances",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "GetSolFunctionPackageContent": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "GetSolFunctionPackageContent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSolFunctionPackages": {
+        "DeleteSolNetworkInstance": {
             "access_level": "Undocumented",
-            "action": "ListSolFunctionPackages",
+            "action": "DeleteSolNetworkInstance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "InstantiateSolNetworkInstance": {
+        "ValidateSolNetworkPackageContent": {
             "access_level": "Undocumented",
-            "action": "InstantiateSolNetworkInstance",
+            "action": "ValidateSolNetworkPackageContent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateSolNetworkPackage": {
+        "CreateSolNetworkInstance": {
             "access_level": "Undocumented",
-            "action": "CreateSolNetworkPackage",
+            "action": "CreateSolNetworkInstance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteSolFunctionPackage": {
+        "PutSolNetworkPackageContent": {
             "access_level": "Undocumented",
-            "action": "DeleteSolFunctionPackage",
+            "action": "PutSolNetworkPackageContent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ValidateSolFunctionPackageContent": {
+        "GetSolNetworkInstance": {
             "access_level": "Undocumented",
-            "action": "ValidateSolFunctionPackageContent",
+            "action": "GetSolNetworkInstance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutSolFunctionPackageContent": {
+        "GetSolNetworkPackageContent": {
             "access_level": "Undocumented",
-            "action": "PutSolFunctionPackageContent",
+            "action": "GetSolNetworkPackageContent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSolNetworkPackageDescriptor": {
+        "GetSolNetworkPackage": {
             "access_level": "Undocumented",
-            "action": "GetSolNetworkPackageDescriptor",
+            "action": "GetSolNetworkPackage",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSolNetworkPackages": {
+        "ListSolFunctionInstances": {
             "access_level": "Undocumented",
-            "action": "ListSolNetworkPackages",
+            "action": "ListSolFunctionInstances",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "GetSolFunctionPackage": {
+            "access_level": "Undocumented",
+            "action": "GetSolFunctionPackage",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "transcribe": {
@@ -162987,81 +162987,81 @@
             "condition_keys": [],
             "description": "Grants permission to update the risk status in AWS Trusted Advisor Priority",
             "orphan": false,
             "resources": []
         }
     },
     "ts": {
-        "ListTagsForResource": {
+        "ListTools": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "ListTools",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartExecution": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "StartExecution",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetTool": {
+        "StartExecution": {
             "access_level": "Undocumented",
-            "action": "GetTool",
+            "action": "StartExecution",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetExecutionOutput": {
+        "GetTool": {
             "access_level": "Undocumented",
-            "action": "GetExecutionOutput",
+            "action": "GetTool",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetExecution": {
+        "ListExecutions": {
             "access_level": "Undocumented",
-            "action": "GetExecution",
+            "action": "ListExecutions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "GetExecutionOutput": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "GetExecutionOutput",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListExecutions": {
+        "GetExecution": {
             "access_level": "Undocumented",
-            "action": "ListExecutions",
+            "action": "GetExecution",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTools": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "ListTools",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "vendor-insights": {
@@ -163347,201 +163347,201 @@
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "verifiedpermissions": {
-        "UpdatePolicyTemplate": {
+        "ListPolicyTemplates": {
             "access_level": "Undocumented",
-            "action": "UpdatePolicyTemplate",
+            "action": "ListPolicyTemplates",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreatePolicyTemplate": {
+        "UpdatePolicyTemplate": {
             "access_level": "Undocumented",
-            "action": "CreatePolicyTemplate",
+            "action": "UpdatePolicyTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteIdentitySource": {
+        "GetPolicy": {
             "access_level": "Undocumented",
-            "action": "DeleteIdentitySource",
+            "action": "GetPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPolicyStore": {
+        "PutSchema": {
             "access_level": "Undocumented",
-            "action": "GetPolicyStore",
+            "action": "PutSchema",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeletePolicy": {
+        "ListPolicyStores": {
             "access_level": "Undocumented",
-            "action": "DeletePolicy",
+            "action": "ListPolicyStores",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreatePolicyStore": {
+        "GetPolicyTemplate": {
             "access_level": "Undocumented",
-            "action": "CreatePolicyStore",
+            "action": "GetPolicyTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeletePolicyStore": {
+        "ListIdentitySources": {
             "access_level": "Undocumented",
-            "action": "DeletePolicyStore",
+            "action": "ListIdentitySources",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPolicyTemplates": {
+        "DeletePolicy": {
             "access_level": "Undocumented",
-            "action": "ListPolicyTemplates",
+            "action": "DeletePolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdatePolicyStore": {
+        "IsAuthorized": {
             "access_level": "Undocumented",
-            "action": "UpdatePolicyStore",
+            "action": "IsAuthorized",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPolicyTemplate": {
+        "UpdateIdentitySource": {
             "access_level": "Undocumented",
-            "action": "GetPolicyTemplate",
+            "action": "UpdateIdentitySource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "IsAuthorized": {
+        "CreatePolicy": {
             "access_level": "Undocumented",
-            "action": "IsAuthorized",
+            "action": "CreatePolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateIdentitySource": {
+        "ListPolicies": {
             "access_level": "Undocumented",
-            "action": "UpdateIdentitySource",
+            "action": "ListPolicies",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPolicies": {
+        "CreatePolicyStore": {
             "access_level": "Undocumented",
-            "action": "ListPolicies",
+            "action": "CreatePolicyStore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListIdentitySources": {
+        "GetSchema": {
             "access_level": "Undocumented",
-            "action": "ListIdentitySources",
+            "action": "GetSchema",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateIdentitySource": {
+        "CreatePolicyTemplate": {
             "access_level": "Undocumented",
-            "action": "CreateIdentitySource",
+            "action": "CreatePolicyTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdatePolicy": {
+        "DeleteIdentitySource": {
             "access_level": "Undocumented",
-            "action": "UpdatePolicy",
+            "action": "DeleteIdentitySource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutSchema": {
+        "DeletePolicyTemplate": {
             "access_level": "Undocumented",
-            "action": "PutSchema",
+            "action": "DeletePolicyTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetIdentitySource": {
+        "IsAuthorizedWithToken": {
             "access_level": "Undocumented",
-            "action": "GetIdentitySource",
+            "action": "IsAuthorizedWithToken",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPolicy": {
+        "CreateIdentitySource": {
             "access_level": "Undocumented",
-            "action": "GetPolicy",
+            "action": "CreateIdentitySource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPolicyStores": {
+        "DeletePolicyStore": {
             "access_level": "Undocumented",
-            "action": "ListPolicyStores",
+            "action": "DeletePolicyStore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreatePolicy": {
+        "GetIdentitySource": {
             "access_level": "Undocumented",
-            "action": "CreatePolicy",
+            "action": "GetIdentitySource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeletePolicyTemplate": {
+        "UpdatePolicy": {
             "access_level": "Undocumented",
-            "action": "DeletePolicyTemplate",
+            "action": "UpdatePolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSchema": {
+        "UpdatePolicyStore": {
             "access_level": "Undocumented",
-            "action": "GetSchema",
+            "action": "UpdatePolicyStore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "IsAuthorizedWithToken": {
+        "GetPolicyStore": {
             "access_level": "Undocumented",
-            "action": "IsAuthorizedWithToken",
+            "action": "GetPolicyStore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "voiceid": {
@@ -167472,345 +167472,345 @@
             "orphan": false,
             "resources": [
                 "network"
             ]
         }
     },
     "wisdom": {
-        "ListKnowledgeBases": {
+        "CreateAssistantAssociation": {
             "access_level": "Undocumented",
-            "action": "ListKnowledgeBases",
+            "action": "CreateAssistantAssociation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "CreateKnowledgeBase": {
             "access_level": "Undocumented",
             "action": "CreateKnowledgeBase",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "ListAssistants": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "ListAssistants",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListImportJobs": {
+        "SearchQuickResponses": {
             "access_level": "Undocumented",
-            "action": "ListImportJobs",
+            "action": "SearchQuickResponses",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetContent": {
+        "GetAssistantAssociation": {
             "access_level": "Undocumented",
-            "action": "GetContent",
+            "action": "GetAssistantAssociation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAssistants": {
+        "GetContent": {
             "access_level": "Undocumented",
-            "action": "ListAssistants",
+            "action": "GetContent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateContent": {
+        "NotifyRecommendationsReceived": {
             "access_level": "Undocumented",
-            "action": "CreateContent",
+            "action": "NotifyRecommendationsReceived",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateSession": {
+        "RemoveKnowledgeBaseTemplateUri": {
             "access_level": "Undocumented",
-            "action": "CreateSession",
+            "action": "RemoveKnowledgeBaseTemplateUri",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "QueryAssistant": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "QueryAssistant",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetRecommendations": {
+        "UpdateContent": {
             "access_level": "Undocumented",
-            "action": "GetRecommendations",
+            "action": "UpdateContent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListQuickResponses": {
+        "DeleteKnowledgeBase": {
             "access_level": "Undocumented",
-            "action": "ListQuickResponses",
+            "action": "DeleteKnowledgeBase",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SearchSessions": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "SearchSessions",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RemoveKnowledgeBaseTemplateUri": {
+        "ListAssistantAssociations": {
             "access_level": "Undocumented",
-            "action": "RemoveKnowledgeBaseTemplateUri",
+            "action": "ListAssistantAssociations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartImportJob": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "StartImportJob",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAssistantAssociation": {
+        "GetContentSummary": {
             "access_level": "Undocumented",
-            "action": "GetAssistantAssociation",
+            "action": "GetContentSummary",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteKnowledgeBase": {
+        "UpdateQuickResponse": {
             "access_level": "Undocumented",
-            "action": "DeleteKnowledgeBase",
+            "action": "UpdateQuickResponse",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetImportJob": {
+        "CreateAssistant": {
             "access_level": "Undocumented",
-            "action": "GetImportJob",
+            "action": "CreateAssistant",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAssistantAssociations": {
+        "ListQuickResponses": {
             "access_level": "Undocumented",
-            "action": "ListAssistantAssociations",
+            "action": "ListQuickResponses",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteAssistantAssociation": {
+        "DeleteQuickResponse": {
             "access_level": "Undocumented",
-            "action": "DeleteAssistantAssociation",
+            "action": "DeleteQuickResponse",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteImportJob": {
+        "GetAssistant": {
             "access_level": "Undocumented",
-            "action": "DeleteImportJob",
+            "action": "GetAssistant",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetContentSummary": {
+        "ListImportJobs": {
             "access_level": "Undocumented",
-            "action": "GetContentSummary",
+            "action": "ListImportJobs",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "SearchContent": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "SearchContent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateAssistant": {
+        "DeleteImportJob": {
             "access_level": "Undocumented",
-            "action": "CreateAssistant",
+            "action": "DeleteImportJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "NotifyRecommendationsReceived": {
+        "ListContents": {
             "access_level": "Undocumented",
-            "action": "NotifyRecommendationsReceived",
+            "action": "ListContents",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SearchQuickResponses": {
+        "CreateContent": {
             "access_level": "Undocumented",
-            "action": "SearchQuickResponses",
+            "action": "CreateContent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteQuickResponse": {
+        "QueryAssistant": {
             "access_level": "Undocumented",
-            "action": "DeleteQuickResponse",
+            "action": "QueryAssistant",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetKnowledgeBase": {
+        "CreateQuickResponse": {
             "access_level": "Undocumented",
-            "action": "GetKnowledgeBase",
+            "action": "CreateQuickResponse",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartContentUpload": {
+        "UpdateKnowledgeBaseTemplateUri": {
             "access_level": "Undocumented",
-            "action": "StartContentUpload",
+            "action": "UpdateKnowledgeBaseTemplateUri",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutFeedback": {
+        "DeleteContent": {
             "access_level": "Undocumented",
-            "action": "PutFeedback",
+            "action": "DeleteContent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListContents": {
+        "GetRecommendations": {
             "access_level": "Undocumented",
-            "action": "ListContents",
+            "action": "GetRecommendations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteAssistant": {
+        "PutFeedback": {
             "access_level": "Undocumented",
-            "action": "DeleteAssistant",
+            "action": "PutFeedback",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSession": {
+        "GetQuickResponse": {
             "access_level": "Undocumented",
-            "action": "GetSession",
+            "action": "GetQuickResponse",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "CreateSession": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "CreateSession",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SearchContent": {
+        "SearchSessions": {
             "access_level": "Undocumented",
-            "action": "SearchContent",
+            "action": "SearchSessions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateContent": {
+        "GetImportJob": {
             "access_level": "Undocumented",
-            "action": "UpdateContent",
+            "action": "GetImportJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetQuickResponse": {
+        "DeleteAssistant": {
             "access_level": "Undocumented",
-            "action": "GetQuickResponse",
+            "action": "DeleteAssistant",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateQuickResponse": {
+        "GetKnowledgeBase": {
             "access_level": "Undocumented",
-            "action": "UpdateQuickResponse",
+            "action": "GetKnowledgeBase",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateKnowledgeBaseTemplateUri": {
+        "GetSession": {
             "access_level": "Undocumented",
-            "action": "UpdateKnowledgeBaseTemplateUri",
+            "action": "GetSession",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateQuickResponse": {
+        "StartImportJob": {
             "access_level": "Undocumented",
-            "action": "CreateQuickResponse",
+            "action": "StartImportJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteContent": {
+        "DeleteAssistantAssociation": {
             "access_level": "Undocumented",
-            "action": "DeleteContent",
+            "action": "DeleteAssistantAssociation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAssistant": {
+        "ListKnowledgeBases": {
             "access_level": "Undocumented",
-            "action": "GetAssistant",
+            "action": "ListKnowledgeBases",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateAssistantAssociation": {
+        "StartContentUpload": {
             "access_level": "Undocumented",
-            "action": "CreateAssistantAssociation",
+            "action": "StartContentUpload",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "workdocs": {
```

### Comparing `iam_actions-1.2.20240406/iam_actions/generate/action_map.py` & `iam_actions-1.2.20240407/iam_actions/generate/action_map.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240406/iam_actions/generate/aws_docs.py` & `iam_actions-1.2.20240407/iam_actions/generate/aws_docs.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240406/iam_actions/generate/generate.py` & `iam_actions-1.2.20240407/iam_actions/generate/generate.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240406/iam_actions/generate/notifier.py` & `iam_actions-1.2.20240407/iam_actions/generate/notifier.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240406/iam_actions/generate/resource_type.py` & `iam_actions-1.2.20240407/iam_actions/generate/resource_type.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240406/iam_actions/generate/services.py` & `iam_actions-1.2.20240407/iam_actions/generate/services.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240406/iam_actions/policies.json` & `iam_actions-1.2.20240407/iam_actions/policies.json`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240406/iam_actions/resourcetypes.json` & `iam_actions-1.2.20240407/iam_actions/resourcetypes.json`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240406/iam_actions/services.json` & `iam_actions-1.2.20240407/iam_actions/services.json`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240406/pyproject.toml` & `iam_actions-1.2.20240407/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iam-actions"
-version = "1.2.20240406"
+version = "1.2.20240407"
 description = "JSON of AWS policy components"
 authors = ["Constable <info@constableapp.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/constableapp/iam_actions"
 packages = [{include = "iam_actions"}]
```

### Comparing `iam_actions-1.2.20240406/setup.py` & `iam_actions-1.2.20240407/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['iam_actions', 'iam_actions.generate']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'iam-actions',
-    'version': '1.2.20240406',
+    'version': '1.2.20240407',
     'description': 'JSON of AWS policy components',
     'long_description': '# iam_actions\n\n`iam_actions` is a python module which contains a dictionary of AWS IAM information. Ideally, it is a complete catalog of all AWS services, actions, and resource types. The information is scraped from the AWS documentation pages.\n\nNightly, the scraping service runs, and publishes a new version with the date appended. \n\nThe package is meant to be used as a consumable package, but it also contains the code to generate the definitions for packaging.\n\nThere are three "roots" that you can consume: actions, resource_types, and services. They all currently return as dict\'s. *However, in a future release, it will be returned as python data structures*\n\n## Actions\n\nActions is a listing of all the actions for a given service. The structure is as follows:\n```\n{\n    "service_name": {\n        "action_name: {\n            "access_level": access_level,\n            "action": action_name,\n            "condition_keys": [condition_key1, ...],\n            "description": description\n        }\n    }\n}\n```\n\nTherefore, you can find information about an action as follows\n\n```\n>>> iam_actions.actions[\'s3\'][\'GetObject\']\n{\'access_level\': \'Read\', \'action\': \'GetObject\', \'condition_keys\': [\'s3:AccessPointNetworkOrigin\', \'s3:DataAccessPointAccount\', \'s3:DataAccessPointArn\', \'s3:ExistingObjectTag/<key>\', \'s3:ResourceAccount\', \'s3:TlsVersion\', \'s3:authType\', \'s3:signatureAge\', \'s3:signatureversion\', \'s3:x-amz-content-sha256\'], \'description\': \'Grants permission to retrieve objects from Amazon S3\', \'orphan\': False, \'resources\': [\'object\']}\n```\n\n## Services\n\nServices list information about the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "Actions": [action1, ...]\n        "ServiceNames": [service_name1, ...]\n        "ARNFormats": [arn_format1, ...]\n        "ConditionKeys": [condition_key1, ...]\n        "HasResource": bool\n    }\n}\n```\n\n## Resource Types\n\nResource Types list information about the resource types for the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "resource_name": {\n            "arn_pattern": arn_pattern,\n            "condition_keys": [condition_key1, ...]\n        }\n    }\n}\n```\n\n## Usage\n\n```python\nimport iam_actions\n\nprint(item_actions.services)\nprint(item_actions.actions)\nprint(item_actions.resource_types)\n```\n',
     'author': 'Constable',
     'author_email': 'info@constableapp.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/constableapp/iam_actions',
```

### Comparing `iam_actions-1.2.20240406/PKG-INFO` & `iam_actions-1.2.20240407/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iam-actions
-Version: 1.2.20240406
+Version: 1.2.20240407
 Summary: JSON of AWS policy components
 Home-page: https://github.com/constableapp/iam_actions
 License: MIT
 Author: Constable
 Author-email: info@constableapp.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

