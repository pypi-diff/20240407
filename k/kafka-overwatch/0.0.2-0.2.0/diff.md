# Comparing `tmp/kafka_overwatch-0.0.2.tar.gz` & `tmp/kafka_overwatch-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kafka_overwatch-0.0.2.tar", max compression
+gzip compressed data, was "kafka_overwatch-0.2.0.tar", max compression
```

## Comparing `kafka_overwatch-0.0.2.tar` & `kafka_overwatch-0.2.0.tar`

### file list

```diff
@@ -1,30 +1,47 @@
--rw-r--r--   0        0        0    16725 2023-12-13 12:48:29.115693 kafka_overwatch-0.0.2/LICENSE
--rw-r--r--   0        0        0     2418 2024-01-03 00:45:07.778910 kafka_overwatch-0.0.2/README.rst
--rw-r--r--   0        0        0      176 2024-01-03 01:09:30.798965 kafka_overwatch-0.0.2/kafka_overwatch/__init__.py
--rw-r--r--   0        0        0     1614 2024-01-03 00:44:12.649974 kafka_overwatch-0.0.2/kafka_overwatch/aws_helpers/__init__.py
--rw-r--r--   0        0        0     1993 2024-01-03 00:44:12.649974 kafka_overwatch-0.0.2/kafka_overwatch/aws_helpers/kafka_client_secrets.py
--rw-r--r--   0        0        0     2624 2024-01-03 00:44:12.649974 kafka_overwatch-0.0.2/kafka_overwatch/aws_helpers/s3.py
--rw-r--r--   0        0        0     1631 2024-01-02 16:20:41.591572 kafka_overwatch-0.0.2/kafka_overwatch/cli.py
--rw-r--r--   0        0        0      970 2024-01-02 07:32:22.109588 kafka_overwatch-0.0.2/kafka_overwatch/config/__init__.py
--rw-r--r--   0        0        0     1601 2024-01-02 07:38:42.091830 kafka_overwatch-0.0.2/kafka_overwatch/config/config.py
--rw-r--r--   0        0        0     3229 2024-01-01 08:48:18.162847 kafka_overwatch-0.0.2/kafka_overwatch/config/logging.py
--rw-r--r--   0        0        0      250 2024-01-02 07:32:22.088588 kafka_overwatch-0.0.2/kafka_overwatch/config/threads_settings.py
--rw-r--r--   0        0        0     1430 2024-01-02 07:32:22.083588 kafka_overwatch-0.0.2/kafka_overwatch/kafka_resources/__init__.py
--rw-r--r--   0        0        0     6457 2024-01-02 16:32:32.717833 kafka_overwatch-0.0.2/kafka_overwatch/kafka_resources/groups.py
--rw-r--r--   0        0        0     6806 2024-01-03 00:44:20.213828 kafka_overwatch-0.0.2/kafka_overwatch/kafka_resources/topics.py
--rw-r--r--   0        0        0       88 2024-01-02 07:32:22.087588 kafka_overwatch-0.0.2/kafka_overwatch/monitoring/__init__.py
--rw-r--r--   0        0        0     1921 2024-01-02 07:32:22.098588 kafka_overwatch-0.0.2/kafka_overwatch/monitoring/prometheus.py
--rw-r--r--   0        0        0     3295 2024-01-02 16:29:57.815101 kafka_overwatch-0.0.2/kafka_overwatch/overwatch.py
--rw-r--r--   0        0        0       86 2024-01-02 07:32:22.104588 kafka_overwatch-0.0.2/kafka_overwatch/overwatch_resources/__init__.py
--rw-r--r--   0        0        0    10415 2024-01-03 00:44:12.649974 kafka_overwatch-0.0.2/kafka_overwatch/overwatch_resources/clusters.py
--rw-r--r--   0        0        0     1975 2024-01-02 07:32:22.085588 kafka_overwatch-0.0.2/kafka_overwatch/overwatch_resources/groups.py
--rw-r--r--   0        0        0     5376 2024-01-02 15:55:34.365483 kafka_overwatch-0.0.2/kafka_overwatch/overwatch_resources/topics.py
--rw-r--r--   0        0        0       88 2024-01-02 07:33:58.717637 kafka_overwatch-0.0.2/kafka_overwatch/processing/__init__.py
--rw-r--r--   0        0        0     3590 2024-01-02 07:38:42.100830 kafka_overwatch-0.0.2/kafka_overwatch/processing/clusters.py
--rw-r--r--   0        0        0       86 2024-01-02 07:32:22.103588 kafka_overwatch-0.0.2/kafka_overwatch/specs/__init__.py
--rw-r--r--   0        0        0    10983 2024-01-03 01:09:38.801812 kafka_overwatch-0.0.2/kafka_overwatch/specs/config.json
--rw-r--r--   0        0        0     6315 2024-01-03 00:44:12.649974 kafka_overwatch-0.0.2/kafka_overwatch/specs/config.py
--rw-r--r--   0        0        0     4467 2024-01-03 01:09:38.801812 kafka_overwatch-0.0.2/kafka_overwatch/specs/report.json
--rw-r--r--   0        0        0     2364 2024-01-03 00:41:50.143723 kafka_overwatch-0.0.2/kafka_overwatch/specs/report.py
--rw-r--r--   0        0        0     2479 2024-01-03 01:09:30.797965 kafka_overwatch-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     3935 1970-01-01 00:00:00.000000 kafka_overwatch-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0    16725 2023-12-13 12:48:29.115693 kafka_overwatch-0.2.0/LICENSE
+-rw-r--r--   0        0        0     3130 2024-02-14 21:24:07.217496 kafka_overwatch-0.2.0/README.rst
+-rw-r--r--   0        0        0      176 2024-04-07 20:44:09.224497 kafka_overwatch-0.2.0/kafka_overwatch/__init__.py
+-rw-r--r--   0        0        0     1300 2024-02-15 16:51:43.978241 kafka_overwatch-0.2.0/kafka_overwatch/aws_helpers/__init__.py
+-rw-r--r--   0        0        0     2372 2024-03-12 06:50:39.512258 kafka_overwatch-0.2.0/kafka_overwatch/aws_helpers/kafka_client_secrets.py
+-rw-r--r--   0        0        0     2862 2024-04-07 20:43:52.705782 kafka_overwatch-0.2.0/kafka_overwatch/aws_helpers/s3.py
+-rw-r--r--   0        0        0     2626 2024-02-07 21:36:59.982077 kafka_overwatch-0.2.0/kafka_overwatch/cli.py
+-rw-r--r--   0        0        0     1175 2024-04-07 20:43:52.705782 kafka_overwatch-0.2.0/kafka_overwatch/common/__init__.py
+-rw-r--r--   0        0        0      970 2024-01-04 01:27:32.802689 kafka_overwatch-0.2.0/kafka_overwatch/config/__init__.py
+-rw-r--r--   0        0        0     3228 2024-04-07 20:43:52.705782 kafka_overwatch-0.2.0/kafka_overwatch/config/config.py
+-rw-r--r--   0        0        0     3229 2024-01-01 08:48:18.162847 kafka_overwatch-0.2.0/kafka_overwatch/config/logging.py
+-rw-r--r--   0        0        0      250 2024-04-06 19:12:23.350109 kafka_overwatch-0.2.0/kafka_overwatch/config/threads_settings.py
+-rw-r--r--   0        0        0     1542 2024-04-07 20:43:52.706782 kafka_overwatch-0.2.0/kafka_overwatch/kafka_resources/__init__.py
+-rw-r--r--   0        0        0     7948 2024-04-07 20:43:52.706782 kafka_overwatch-0.2.0/kafka_overwatch/kafka_resources/groups.py
+-rw-r--r--   0        0        0     8939 2024-04-07 20:43:52.706782 kafka_overwatch-0.2.0/kafka_overwatch/kafka_resources/topics.py
+-rw-r--r--   0        0        0       88 2024-01-02 07:32:22.087588 kafka_overwatch-0.2.0/kafka_overwatch/monitoring/__init__.py
+-rw-r--r--   0        0        0     2513 2024-04-07 20:43:52.706782 kafka_overwatch-0.2.0/kafka_overwatch/monitoring/prometheus.py
+-rw-r--r--   0        0        0      176 2024-03-11 21:31:12.971386 kafka_overwatch-0.2.0/kafka_overwatch/notifications/__init__.py
+-rw-r--r--   0        0        0     5230 2024-04-07 20:43:52.706782 kafka_overwatch-0.2.0/kafka_overwatch/notifications/aws_sns/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-11 21:31:12.972386 kafka_overwatch-0.2.0/kafka_overwatch/notifications/aws_sns/usage_report/__init__.py
+-rw-r--r--   0        0        0       83 2024-03-11 21:31:12.972386 kafka_overwatch-0.2.0/kafka_overwatch/notifications/aws_sns/usage_report/default.j2
+-rw-r--r--   0        0        0      484 2024-03-11 21:31:12.972386 kafka_overwatch-0.2.0/kafka_overwatch/notifications/aws_sns/usage_report/email.j2
+-rw-r--r--   0        0        0     3496 2024-04-07 20:43:52.706782 kafka_overwatch-0.2.0/kafka_overwatch/overwatch.py
+-rw-r--r--   0        0        0       86 2024-01-02 07:32:22.104588 kafka_overwatch-0.2.0/kafka_overwatch/overwatch_resources/__init__.py
+-rw-r--r--   0        0        0    14000 2024-04-07 20:43:52.706782 kafka_overwatch-0.2.0/kafka_overwatch/overwatch_resources/clusters.py
+-rw-r--r--   0        0        0     5026 2024-03-11 06:55:53.345126 kafka_overwatch-0.2.0/kafka_overwatch/overwatch_resources/groups.py
+-rw-r--r--   0        0        0     4487 2024-04-07 20:43:52.707782 kafka_overwatch-0.2.0/kafka_overwatch/overwatch_resources/schema_registry/__init__.py
+-rw-r--r--   0        0        0     2412 2024-04-07 20:43:52.707782 kafka_overwatch-0.2.0/kafka_overwatch/overwatch_resources/schema_registry/schema.py
+-rw-r--r--   0        0        0      801 2024-04-07 20:43:52.707782 kafka_overwatch-0.2.0/kafka_overwatch/overwatch_resources/schema_registry/subject.py
+-rw-r--r--   0        0        0     7286 2024-04-07 20:43:52.707782 kafka_overwatch-0.2.0/kafka_overwatch/overwatch_resources/topics.py
+-rw-r--r--   0        0        0     1089 2024-04-07 20:43:52.707782 kafka_overwatch-0.2.0/kafka_overwatch/processing/__init__.py
+-rw-r--r--   0        0        0     5893 2024-04-07 20:43:52.707782 kafka_overwatch-0.2.0/kafka_overwatch/processing/clusters.py
+-rw-r--r--   0        0        0     9011 2024-04-07 20:43:52.707782 kafka_overwatch-0.2.0/kafka_overwatch/processing/schema_registries.py
+-rw-r--r--   0        0        0     4793 2024-04-07 20:43:52.707782 kafka_overwatch-0.2.0/kafka_overwatch/reporting/__init__.py
+-rw-r--r--   0        0        0       88 2024-02-14 21:24:07.217496 kafka_overwatch-0.2.0/kafka_overwatch/reporting/governance/__init__.py
+-rw-r--r--   0        0        0     1364 2024-03-11 06:55:53.346126 kafka_overwatch-0.2.0/kafka_overwatch/reporting/governance/consumer_groups_naming_convention.py
+-rw-r--r--   0        0        0     1355 2024-02-14 21:24:07.217496 kafka_overwatch-0.2.0/kafka_overwatch/reporting/governance/topic_naming_convention.py
+-rw-r--r--   0        0        0     1128 2024-04-07 20:43:52.707782 kafka_overwatch-0.2.0/kafka_overwatch/reporting/schema_registry.py
+-rw-r--r--   0        0        0     1963 2024-03-11 06:55:53.346126 kafka_overwatch-0.2.0/kafka_overwatch/reporting/tools.py
+-rw-r--r--   0        0        0     3967 2024-04-07 20:43:52.707782 kafka_overwatch-0.2.0/kafka_overwatch/reporting/topics.py
+-rw-r--r--   0        0        0       86 2024-01-02 07:32:22.103588 kafka_overwatch-0.2.0/kafka_overwatch/specs/__init__.py
+-rw-r--r--   0        0        0    21799 2024-04-07 20:44:09.498493 kafka_overwatch-0.2.0/kafka_overwatch/specs/config.json
+-rw-r--r--   0        0        0    11668 2024-04-07 20:43:52.708782 kafka_overwatch-0.2.0/kafka_overwatch/specs/config.py
+-rw-r--r--   0        0        0     6716 2024-04-07 20:44:09.498493 kafka_overwatch-0.2.0/kafka_overwatch/specs/report.json
+-rw-r--r--   0        0        0     3249 2024-04-07 20:43:52.708782 kafka_overwatch-0.2.0/kafka_overwatch/specs/report.py
+-rw-r--r--   0        0        0     2812 2024-04-07 20:44:09.224497 kafka_overwatch-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     4938 1970-01-01 00:00:00.000000 kafka_overwatch-0.2.0/PKG-INFO
```

### Comparing `kafka_overwatch-0.0.2/LICENSE` & `kafka_overwatch-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kafka_overwatch-0.0.2/README.rst` & `kafka_overwatch-0.2.0/README.rst`

 * *Files 10% similar despite different names*

```diff
@@ -67,7 +67,24 @@
 
 .. _EMF: https://docs.aws.amazon.com/AmazonCloudWatch/latest/monitoring/CloudWatch_Embedded_Metric_Format_Specification.html
 .. _kafka-idle-topics: https://github.com/abraham-leal/kafka-idle-topics
 .. _cfn-kafka-admin: https://github.com/compose-x/cfn-kafka-admin
 .. _cruise-control: https://github.com/linkedin/cruise-control
 .. _jsonschema: https://pypi.org/project/jsonschema/
 .. _NASA: https://www.nasa.gov/
+
+
+Status
+=======
+
+Images build status
+
+|BUILD|
+
+Docs build status
+
+|DOCS_BUILD|
+
+
+.. |BUILD| image:: https://codebuild.eu-west-1.amazonaws.com/badges?uuid=eyJlbmNyeXB0ZWREYXRhIjoiU3RHQnZ2eFpnQTlOSmU2MUM3NDB5NW9uMDY2TS9DZXBWZ2hmejdoK2xJRStHK2Fhd3FkS1FoQjJOSTcvYjVBNkFTTW5kVDNZK0NqZEthU3gveFpOVEljPSIsIml2UGFyYW1ldGVyU3BlYyI6IjlUbE0vNmpPQU92U1o0SmkiLCJtYXRlcmlhbFNldFNlcmlhbCI6MX0%3D&branch=main
+
+.. |DOCS_BUILD| image:: https://codebuild.eu-west-1.amazonaws.com/badges?uuid=eyJlbmNyeXB0ZWREYXRhIjoiSVNBZkVSUkx1NHhtamlqSEJqempIdHd2aVNqV2RkTTFVYlphUzJ2ekprOVU4ODZ4cUNWcTNVSkRVM2ovcGFyak5NTTNJZ1Vra2ErSzVOdi84TkVLOUp3PSIsIml2UGFyYW1ldGVyU3BlYyI6IjAvK25MSmNPcjNScVpwdTQiLCJtYXRlcmlhbFNldFNlcmlhbCI6MX0%3D&branch=main
```

### Comparing `kafka_overwatch-0.0.2/kafka_overwatch/aws_helpers/kafka_client_secrets.py` & `kafka_overwatch-0.2.0/kafka_overwatch/aws_helpers/kafka_client_secrets.py`

 * *Files 13% similar despite different names*

```diff
@@ -18,23 +18,18 @@
     parse_secret_resolve_string,
     retrieve_secret,
 )
 from boto3.session import Session
 
 from kafka_overwatch.aws_helpers import get_session_from_iam_override
 from kafka_overwatch.config.logging import KAFKA_LOG
+from kafka_overwatch.specs.config import ClusterConfig, MskClusterConfig
 
 
-def eval_kafka_client_config(kafka_cluster: KafkaCluster) -> dict:
-    """
-    If a configuration value is a string starting with {{resolve:}} the value is interpolated
-    using AWS SecretsManager or AWS SSM.
-    We create a new dict in order to preserve the original
-    """
-
+def handle_librdkafka_config(kafka_cluster: KafkaCluster) -> dict:
     if (
         kafka_cluster.config.cluster_config.cluster_config_auth
         and kafka_cluster.config.cluster_config.cluster_config_auth.iam_override
     ):
         session = get_session_from_iam_override(
             kafka_cluster.config.cluster_config.cluster_config_auth.iam_override
         )
@@ -51,7 +46,20 @@
                 client_config[config_key] = secret
             except Exception as error:
                 KAFKA_LOG.exception(error)
                 KAFKA_LOG.error(
                     f"Error while resolving {config_value}: {error}. Using value as-is."
                 )
     return client_config
+
+
+def eval_kafka_client_config(kafka_cluster: KafkaCluster) -> dict:
+    """
+    If a configuration value is a string starting with {{resolve:}} the value is interpolated
+    using AWS SecretsManager or AWS SSM.
+    We create a new dict in order to preserve the original
+    """
+    if isinstance(kafka_cluster.config.cluster_config, MskClusterConfig):
+        raise NotImplementedError("MskClusterConfig is not yet implemented.")
+
+    client_config = handle_librdkafka_config(kafka_cluster)
+    return client_config
```

### Comparing `kafka_overwatch-0.0.2/kafka_overwatch/aws_helpers/s3.py` & `kafka_overwatch-0.2.0/kafka_overwatch/aws_helpers/s3.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from kafka_overwatch.specs.config import S3Output
 
 
 class S3Handler:
     def __init__(self, s3_output_config: S3Output):
         self._config = s3_output_config
 
-        if not self._config.IamOverride:
+        if not self._config.iam_override:
             self._session: Session = Session()
         else:
             self._session = None
 
         if self._session:
             self._client = self._session.client("s3")
         else:
@@ -30,48 +30,55 @@
 
     @property
     def config(self) -> S3Output:
         return self._config
 
     @property
     def session(self) -> Session:
-        if not self._config.IamOverride:
+        if not self._config.iam_override:
             return self._session
         else:
-            return get_session_from_iam_override(self._config.IamOverride)
+            return get_session_from_iam_override(self._config.iam_override)
 
     @property
     def client(self):
         """Ensures to get client with a fresh session if needed"""
         if not self._client and self._session:
             self._client = self.session.client("s3")
             return self._client
         elif self._client:
             return self._client
         return self.session.client("s3")
 
     @retry((S3UploadFailedError,), tries=3, delay=1, logger=KAFKA_LOG)
-    def upload(self, report: str, report_name: str, mime_type: str = None):
+    def upload(
+        self, body: str | bytes, file_name: str, mime_type: str = None
+    ) -> str | None:
+        prefix_key: str = (
+            f"{self._config.prefix_key}/{file_name}"
+            if self._config.prefix_key != ""
+            else file_name
+        )
+        upload_path: str = (
+            f"{self.config.bucket_name}/{self.config.prefix_key}/{file_name}"
+        )
         try:
             self.client.put_object(
-                Bucket=self._config.BucketName,
-                Key=f"{self._config.PrefixKey}/{report_name}",
-                Body=report.encode("utf-8"),
+                Bucket=self._config.bucket_name,
+                Key=prefix_key,
+                Body=body.encode("utf-8") if not isinstance(body, bytes) else body,
                 ContentType="application/json" if not mime_type else mime_type,
             )
-            KAFKA_LOG.info(
-                "File uploaded to "
-                f"{self.config.BucketName}/{self.config.PrefixKey}/{report_name}"
-            )
-            return
+            KAFKA_LOG.info(f"File uploaded to {upload_path}")
+            return upload_path
         except ClientError as error:
             KAFKA_LOG.exception(error)
             KAFKA_LOG.error(
                 "Failed to upload report to "
-                f"{self.config.BucketName}/{self.config.PrefixKey}/{report_name}"
+                f"{self.config.bucket_name}/{self.config.prefix_key}/{file_name}"
             )
         except Exception as error:
             KAFKA_LOG.exception(error)
             KAFKA_LOG.error(
                 "Failed to upload report to "
-                f"{self.config.BucketName}/{self.config.PrefixKey}/{report_name}"
+                f"{self.config.bucket_name}/{self.config.prefix_key}/{file_name}"
             )
```

### Comparing `kafka_overwatch-0.0.2/kafka_overwatch/config/__init__.py` & `kafka_overwatch-0.2.0/kafka_overwatch/config/__init__.py`

 * *Files identical despite different names*

### Comparing `kafka_overwatch-0.0.2/kafka_overwatch/config/config.py` & `kafka_overwatch-0.2.0/kafka_overwatch/config/config.py`

 * *Files 24% similar despite different names*

```diff
@@ -6,20 +6,24 @@
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
     from kafka_overwatch.specs.config import KafkaOverwatchInputConfiguration
 
 from tempfile import TemporaryDirectory
 
+from cryptography.fernet import Fernet
 from dacite import from_dict
 from prometheus_client import CollectorRegistry, multiprocess
 
 from kafka_overwatch.monitoring.prometheus import (
-    set_cluster_prometheus_registry_collectors,
+    set_kafka_cluster_prometheus_registry_collectors,
+    set_schema_registry_prometheus_registry_collectors,
 )
+from kafka_overwatch.notifications.aws_sns import SnsChannel
+from kafka_overwatch.overwatch_resources.schema_registry import SchemaRegistry
 from kafka_overwatch.specs.config import Global
 
 
 class OverwatchConfig:
     """
     Class to store in-memory the clusters and their configurations, derived from the input configuration
     classes.
@@ -27,28 +31,58 @@
 
     def __init__(
         self,
         config: KafkaOverwatchInputConfiguration,
         prometheus_dir: TemporaryDirectory,
     ):
         if not config.global_:
-            config.global_ = from_dict(Global, {"ClusterScanIntervalInSeconds": 30})
+            config.global_ = from_dict(Global, {"cluster_scan_interval_in_seconds": 30})
         self._config = config
         self._prometheus_registry_dir = prometheus_dir
 
         self.prometheus_registry: CollectorRegistry = CollectorRegistry(
             auto_describe=True,
         )
-        self.prometheus_collectors = set_cluster_prometheus_registry_collectors(
+        self.prometheus_collectors = set_kafka_cluster_prometheus_registry_collectors(
             self.prometheus_registry
         )
+        self.prometheus_collectors.update(
+            set_schema_registry_prometheus_registry_collectors(self.prometheus_registry)
+        )
         multiprocess.MultiProcessCollector(
             self.prometheus_registry, path=self._prometheus_registry_dir.name
         )
+        self.runtime_key = Fernet.generate_key()
+        self.sns_channels: dict[str, SnsChannel] = {}
+        self.schema_registries: dict[str, SchemaRegistry] = {}
+        self.init_schema_registries()
+        self.init_notification_channels()
+
+    def __reduce__(self):
+        # Return a tuple with the callable and its arguments
+        return (self.__class__, (self._config, self._prometheus_registry_dir))
 
     @property
     def input_config(self):
         return self._config
 
     @property
     def prometheus_registry_dir(self) -> TemporaryDirectory:
         return self._prometheus_registry_dir
+
+    def init_schema_registries(self):
+        """Initializes the Schema Registries client if setup in the configuration"""
+        for registry_name, registry in self.input_config.schema_registries.items():
+            _registry = SchemaRegistry(registry_name, registry, self.runtime_key)
+            self.schema_registries[registry_name] = _registry
+
+    def init_notification_channels(self):
+        if not self._config.notification_channels:
+            return
+        if not self._config.notification_channels.sns:
+            return
+        for (
+            sns_channel_name,
+            sns_channel_definition,
+        ) in self._config.notification_channels.sns.items():
+            sns_channel = SnsChannel(sns_channel_name, sns_channel_definition)
+            self.sns_channels[sns_channel_name] = sns_channel
```

### Comparing `kafka_overwatch-0.0.2/kafka_overwatch/config/logging.py` & `kafka_overwatch-0.2.0/kafka_overwatch/config/logging.py`

 * *Files identical despite different names*

### Comparing `kafka_overwatch-0.0.2/kafka_overwatch/kafka_resources/__init__.py` & `kafka_overwatch-0.2.0/kafka_overwatch/kafka_resources/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,38 +2,40 @@
 # Copyright 2024 John Mille <john@ews-network.net>
 
 from __future__ import annotations
 
 from copy import deepcopy
 from os import environ
 
-from confluent_kafka import Consumer
+from confluent_kafka import Consumer, KafkaException
 from confluent_kafka.admin import AdminClient
+from retry import retry
 
 
+@retry((KafkaException,), delay=5, max_delay=30, backoff=2)
 def wait_for_result(result_container: dict) -> dict:
     for _future in result_container.values():
         while not _future.done():
-            pass
+            _future.result()
     return result_container
 
 
-def get_consumer_client(settings: dict) -> Consumer:
+def set_consumer_client(settings: dict) -> Consumer:
     """Creates a new librdkafka Consumer client"""
     client_id: str = f"consumer_partitions_hunter"
     cluster_config = deepcopy(settings)
     cluster_config.update({"client.id": client_id})
     if "group.id" not in cluster_config:
         cluster_config["group.id"] = environ.get(
             "CONSUMER_GROUP_ID", "kafka-partitions-hunter"
         )
     return Consumer(cluster_config)
 
 
-def get_admin_client(settings: dict) -> AdminClient:
+def set_admin_client(settings: dict) -> AdminClient:
     """Creates a new librdkafka Admin client"""
     client_id: str = f"admin_partitions_hunter"
     timeout_ms_env = int(environ.get("ADMIN_REQUEST_TIMEOUT_MS", 60000))
     cluster_config = deepcopy(settings)
     cluster_config.update({"client.id": client_id})
     if "group.id" in cluster_config:
         del cluster_config["group.id"]
```

### Comparing `kafka_overwatch-0.0.2/kafka_overwatch/kafka_resources/groups.py` & `kafka_overwatch-0.2.0/kafka_overwatch/kafka_resources/groups.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,110 +5,196 @@
 
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
     from kafka_overwatch.overwatch_resources.clusters import KafkaCluster
     from confluent_kafka.admin import ConsumerGroupDescription
 
-from queue import Queue
-from threading import Thread
+import concurrent.futures
 
 from confluent_kafka import ConsumerGroupTopicPartitions
-from confluent_kafka.error import KafkaError
-from retry import retry
+from confluent_kafka.error import KafkaError, KafkaException
 
+from kafka_overwatch.common import waiting_on_futures
 from kafka_overwatch.config.logging import KAFKA_LOG
-from kafka_overwatch.config.threads_settings import NUM_THREADS
 from kafka_overwatch.kafka_resources import wait_for_result
 from kafka_overwatch.overwatch_resources.groups import ConsumerGroup
 
 
-@retry((KafkaError,), tries=10, delay=5, backoff=2, jitter=(2, 5))
-def get_consumer_groups_desc(kafka_cluster: KafkaCluster, groups_list: list) -> dict:
-    try:
-        groups_desc = wait_for_result(
-            kafka_cluster.admin_client.describe_consumer_groups(
-                [_group for _group in groups_list]
+def get_consumer_groups_desc(
+    kafka_cluster: KafkaCluster,
+    groups_list: list,
+    groups_desc: dict[str, ConsumerGroupDescription] | None = None,
+) -> dict[str, ConsumerGroupDescription]:
+    if groups_desc is None:
+        groups_desc: dict[str, ConsumerGroupDescription] = {}
+
+    groups_to_describe: list[str] = [_group for _group in groups_list]
+    groups_desc_r: dict[str, concurrent.futures.Future] = (
+        kafka_cluster.get_admin_client().describe_consumer_groups(groups_to_describe)
+    )
+
+    to_retry: list[str] = []
+
+    for _group_name, _future in groups_desc_r.items():
+        try:
+            groups_desc[_group_name] = _future.result()
+        except (KafkaError, KafkaException) as error:
+            KAFKA_LOG.error(
+                "%s - %s - Error getting consumer group description"
+                % (kafka_cluster.name, _group_name)
             )
-        )
-        return groups_desc
-    except KafkaError as error:
-        print(error)
-        raise
+            print(error)
+            to_retry.append(_group_name)
+    if to_retry:
+        print(f"GOT TO RETRY {len(to_retry)} CGs")
+        get_consumer_groups_desc(kafka_cluster, to_retry, groups_desc)
+
+    return groups_desc
 
 
 def tidy_consumer_groups(
     kafka_cluster: KafkaCluster, query_groups_list: list[str]
 ) -> None:
-    existing_groups_list: list = list(kafka_cluster.groups.keys())
+    existing_groups_list: list[str] = list(kafka_cluster.groups.keys())
     if existing_groups_list and query_groups_list:
         for group in existing_groups_list:
             if group not in query_groups_list:
                 try:
+                    for topic in kafka_cluster.topics.values():
+                        if topic.consumer_groups and group in topic.consumer_groups:
+                            del topic.consumer_groups[group]
                     print(
                         f"Consumer group {group} no longer on cluster {kafka_cluster.name} metadata"
                     )
                     del kafka_cluster.groups[group]
                 except KeyError:
                     pass
 
 
-def set_update_cluster_consumer_groups(
-    kafka_cluster: KafkaCluster,
-) -> None:
+def set_update_filter_cluster_consumer_groups(kafka_cluster: KafkaCluster) -> None:
     """
-    Lists all Consumer Groups
-    Checks if all the listed CGs were present in the existing cluster CGs. If not, remove.
-    Describe all Consumer Groups
-    List all Consumer Group Offsets (serial, no support for list of CGs)
-    If CG not in the cluster groups, add to it
+    Lists all the consumer groups from the Kafka cluster
+    Filters out of the Kafka cluster groups attribute all the consumer groups that are not in the list
+    Retrieves the consumer group description/details from the cluster
     """
-    groups_list_future = kafka_cluster.admin_client.list_consumer_groups()
+
+    groups_list_future = kafka_cluster.get_admin_client().list_consumer_groups()
     while not groups_list_future.done():
-        pass
+        if groups_list_future.exception():
+            print(f"{kafka_cluster.name} - Failed to get consumer groups list")
+            return
+
     query_groups_list = [
         _group.group_id for _group in groups_list_future.result().valid
     ]
-    tidy_consumer_groups(kafka_cluster, query_groups_list)
     if not query_groups_list:
         KAFKA_LOG.warning(f"{kafka_cluster.name}: No consumer groups to describe.")
         return
+    tidy_consumer_groups(kafka_cluster, query_groups_list)
 
     groups_desc = get_consumer_groups_desc(kafka_cluster, query_groups_list)
-    groups_processing_threads: list[Thread] = []
-    KAFKA_LOG.debug(f"{kafka_cluster.name} has {len(query_groups_list)} CGs")
-    for desc_future in groups_desc.values():
-        kafka_cluster.groups_describe_queue.put(
-            [desc_future, kafka_cluster],
-            False,
+
+    for group_desc in groups_desc.values():
+        if group_desc.group_id not in kafka_cluster.groups:
+            consumer_group = ConsumerGroup(
+                group_desc.group_id,
+                group_desc.members,
+                group_desc.state,
+            )
+            kafka_cluster.groups[group_desc.group_id] = consumer_group
+        else:
+            consumer_group: ConsumerGroup = kafka_cluster.groups[group_desc.group_id]
+            consumer_group.members = group_desc.members
+            consumer_group.state = group_desc.state
+
+
+def set_update_cluster_consumer_groups(
+    kafka_cluster: KafkaCluster,
+) -> None:
+    """
+    Lists all Consumer Groups
+    Checks if all the listed CGs were present in the existing cluster CGs. If not, remove.
+    Describe all Consumer Groups
+    List all Consumer Group Offsets (serial, no support for list of CGs)
+    If CG not in the cluster groups, add to it
+    """
+    set_update_filter_cluster_consumer_groups(kafka_cluster)
+    _tasks = len(kafka_cluster.groups)
+    groups_jobs: dict = {
+        _consumer_group_name: [_consumer_group, kafka_cluster]
+        for _consumer_group_name, _consumer_group in kafka_cluster.groups.items()
+    }
+
+    with concurrent.futures.ThreadPoolExecutor(
+        max_workers=kafka_cluster.cluster_brokers_count
+    ) as executor:
+        futures_to_data: dict[concurrent.futures.Future, list] = {
+            executor.submit(
+                describe_update_consumer_group_offsets, *job_params
+            ): job_params
+            for job_params in groups_jobs.values()
+        }
+        _pending = len(futures_to_data)
+        KAFKA_LOG.info(f"Kafka cluster: {kafka_cluster.name} | CGs to scan: {_pending}")
+        waiting_on_futures(
+            executor,
+            futures_to_data,
+            "Kafka Cluster",
+            kafka_cluster.name,
+            "Consumer groups",
         )
-    if kafka_cluster.groups_describe_queue.qsize() == 0:
-        KAFKA_LOG.info(f"{kafka_cluster.name}: no consumer group to describe in queue.")
-        return
 
-    for _ in range(NUM_THREADS):
-        _thread = Thread(
-            target=describe_update_consumer_groups,
-            daemon=True,
-            args=(kafka_cluster.groups_describe_queue,),
+
+def describe_update_consumer_group_offsets(
+    consumer_group: ConsumerGroup, kafka_cluster: KafkaCluster
+) -> None:
+    """
+    Retrieve a given Consumer group details, given that the list_consumer_group_offsets cannot take
+    multiple groups as argument.
+    Updates the kafka_cluster.groups.
+    """
+    if not consumer_group or not kafka_cluster:
+        return
+    try:
+        consumer_group.partitions_offsets = wait_for_result(
+            kafka_cluster.get_admin_client().list_consumer_group_offsets(
+                [ConsumerGroupTopicPartitions(consumer_group.group_id)],
+                require_stable=True,
+            )
         )
-        _thread.start()
-        groups_processing_threads.append(_thread)
-    kafka_cluster.groups_describe_queue.join()
+    except Exception as error:
+        if error.args[0] == KafkaError.REQUEST_TIMED_OUT:
+            print("CG DESCRIBE TIMEOUT", error)
+        else:
+            print("CG DESCRIBE ERROR", error)
+
+
+def retry_kafka_describe_update_consumer_group_offsets(
+    future, futures_to_data, executor
+):
+    # get the associated data for the task
+    data = futures_to_data[future]
+    # submit the task again
+    _retry = executor.submit(describe_update_consumer_group_offsets, data)
+    # store so we can track the retries
+    futures_to_data[_retry] = data
+    return data
 
 
 def update_set_consumer_group_topics_partitions_offsets(
-    kafka_cluster: KafkaCluster, consumer_group: ConsumerGroup, groups_offsets: dict
+    kafka_cluster: KafkaCluster,
+    consumer_group: ConsumerGroup,
 ) -> None:
     """
     Groups topic partitions offsets per topic
     Assigns partitions offsets to the consumer group
     Maps consumer group to topic
     """
-    for _group, _future in groups_offsets.items():
+    for _group, _future in consumer_group.partitions_offsets.items():
         offsets_result = _future.result()
 
         __topic_partitions_new_offsets: dict = {}
         for _topic_partition in offsets_result.topic_partitions:
             if _topic_partition.topic in kafka_cluster.topics:
                 _topic = kafka_cluster.topics[_topic_partition.topic]
             else:
@@ -119,47 +205,7 @@
                 __topic_partitions_new_offsets[_topic] = [_topic_partition]
             else:
                 __topic_partitions_new_offsets[_topic].append(_topic_partition)
         for _topic, _topic_partitions in __topic_partitions_new_offsets.items():
             consumer_group.topic_offsets[_topic] = _topic_partitions
             if consumer_group not in _topic.consumer_groups:
                 _topic.consumer_groups[consumer_group.group_id] = consumer_group
-
-
-def describe_update_consumer_groups(queue: Queue) -> None:
-    """
-    Thread worker to retrieve a given Consumer group details, given that the list_consumer_group_offsets cannot take
-    multiple groups as argument.
-    Updates the kafka_cluster.groups.
-    """
-    while 42:
-        if not queue.empty():
-            desc_future, kafka_cluster = queue.get()
-            group_description: ConsumerGroupDescription = desc_future.result()
-            group = group_description.group_id
-            KAFKA_LOG.debug(f"Describing consumer group {group} - {kafka_cluster.name}")
-            try:
-                if group not in kafka_cluster.groups:
-                    kafka_cluster.groups[group] = ConsumerGroup(
-                        group_description.group_id,
-                        group_description.members,
-                        group_description.state,
-                    )
-                consumer_group = kafka_cluster.groups[group]
-                group_offsets = wait_for_result(
-                    kafka_cluster.admin_client.list_consumer_group_offsets(
-                        [ConsumerGroupTopicPartitions(group_description.group_id)]
-                    )
-                )
-                update_set_consumer_group_topics_partitions_offsets(
-                    kafka_cluster, consumer_group, group_offsets
-                )
-            except Exception as error:
-                KAFKA_LOG.exception(error)
-                KAFKA_LOG.error(
-                    f"{kafka_cluster.name}:{desc_future.result().group_id} - "
-                    "Failure during retrieving consumer group details"
-                )
-            queue.task_done()
-        else:
-            KAFKA_LOG.debug("Thread closing for describe_update_consumer_groups")
-            return
```

### Comparing `kafka_overwatch-0.0.2/kafka_overwatch/monitoring/prometheus.py` & `kafka_overwatch-0.2.0/kafka_overwatch/monitoring/prometheus.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #  SPDX-License-Identifier: MPL-2.0
 #  Copyright 2024 John Mille <john@ews-network.net>
 
 from prometheus_client import CollectorRegistry, Gauge, Summary
 
 
-def set_cluster_prometheus_registry_collectors(
+def set_kafka_cluster_prometheus_registry_collectors(
     prometheus_registry: CollectorRegistry,
 ) -> dict[str, Gauge | Summary]:
     collectors: dict = {
         "topic_partition_new_messages": Summary(
             "topic_partition_new_messages",
             "New messages added since last interval",
             labelnames=["cluster", "topic_name", "partition_id"],
@@ -49,7 +49,27 @@
             "consumer_group_lag",
             "Consumer group lag",
             ["cluster", "consumer_group", "topic_name"],
             registry=prometheus_registry,
         ),
     }
     return collectors
+
+
+def set_schema_registry_prometheus_registry_collectors(
+    prometheus_registry: CollectorRegistry,
+) -> dict[str, Gauge | Summary]:
+    collectors: dict = {
+        "subjects_count": Gauge(
+            "subjects_count",
+            "Total number of subjects",
+            labelnames=["schema_registry"],
+            registry=prometheus_registry,
+        ),
+        "schemas_count": Gauge(
+            "schemas_count",
+            "Total number of subjects",
+            labelnames=["schema_registry"],
+            registry=prometheus_registry,
+        ),
+    }
+    return collectors
```

### Comparing `kafka_overwatch-0.0.2/kafka_overwatch/specs/config.py` & `kafka_overwatch-0.2.0/kafka_overwatch/specs/config.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # generated by datamodel-codegen:
 #   filename:  config.json
 
 from __future__ import annotations
 
 from dataclasses import dataclass, field
 from enum import Enum
-from typing import Any, Dict, List, Optional
+from typing import Any, Dict, List, Optional, Union
 
 
 @dataclass
 class AwsEmf:
     namespace: str
     high_resolution_metrics: bool | None = False
     """
@@ -28,18 +28,14 @@
     Allows to set specific templates for email and sms
     """
 
     email: str | None = None
     """
     Optional - Path to a template for SNS Email messages
     """
-    sms: str | None = None
-    """
-    Optional - Path to a template for SNS SMS messages
-    """
 
 
 @dataclass
 class SnsTopicChannel:
     topic_arn: str
     """
     ARN of the SNS topic.
@@ -68,58 +64,108 @@
     prometheus: Prometheus | None = None
     aws_emf: AwsEmf | None = None
 
 
 Regexes = list[str]
 
 
+@dataclass
+class OutputFormats:
+    """
+    The different types of outputs to produce.
+    """
+
+    pandas_dataframe: list[str] | None = None
+
+
 class BackupStyle(Enum):
     cfn_kafka_admin = "cfn-kafka-admin"
     kafka_topics_sh = "kafka-topics.sh"
 
 
+ClusterScanIntervalInSeconds = int
+
+
 @dataclass
-class AssumeRole:
-    RoleArn: str
+class ConfluentCloudAuth:
+    api_key: str | None = None
     """
-    Optional - IAM Role ARN to assume
+    The API key to use to perform API calls to Confluent Cloud
     """
-    RoleSessionName: str | None = "kafka-overwatch@aws"
+    api_secret: str | None = None
     """
-    Optional - Name of the session to use
+    The API Secret to perform API calls to Confluent Cloud
     """
-    ExternalId: str | None = None
+
+
+@dataclass
+class NamingConvention:
     """
-    Optional - External ID to use when assuming a role
+    Evaluates topic name against one or more regex and reports non-compliant topics
     """
 
+    regexes: list[str]
+    ignore_regexes: list[str] | None = None
+    """
+    List/Array of regular expression of topic names to ignore for review. Use to ignore internal or stream topics
+    """
+
+
+@dataclass
+class BasicAuth:
+    username: str | None = None
+    password: str | None = None
+
 
 @dataclass
-class IamOverride:
+class ConfluentSchemaRegistry:
     """
-    Optional - IAM profile/settings override to use. Defaults to SDK settings.
+    Schema registry client configuration. Uses APIs of Confluent Schema Registry
     """
 
-    ProfileName: str | None = None
+    schema_registry_url: str
+    basic_auth: BasicAuth | str | None = None
+
+
+@dataclass
+class ClusterReportSnsChannel:
     """
-    Optional - Use IAM profile to publish messages using another IAM profile
+    Sns topic to send the messages to
     """
-    AssumeRole: AssumeRole | None = None
 
+    name: str
+    sign_s3_url: bool | float | None = None
 
-ClusterScanIntervalInSeconds = int
+
+@dataclass
+class AssumeRole:
+    RoleArn: str
+    """
+    Optional - IAM Role ARN to assume
+    """
+    RoleSessionName: str | None = "kafka-overwatch@aws"
+    """
+    Optional - Name of the session to use
+    """
+    ExternalId: str | None = None
+    """
+    Optional - External ID to use when assuming a role
+    """
 
 
 @dataclass
 class Global:
     """
-    Global settings. Apply to all clusters
+    Global settings. Defines global default values that can be overriden for each cluster.
     """
 
-    ClusterScanIntervalInSeconds: ClusterScanIntervalInSeconds
+    cluster_scan_interval_in_seconds: ClusterScanIntervalInSeconds
+    """
+    Default topics & consumer groups scan interval
+    """
 
 
 @dataclass
 class AwsEmfModel:
     log_group_name: str | None = "kafka/cluster/overwatch/metrics"
     """
     override log group name to publish metrics to. Importance: High
@@ -137,62 +183,145 @@
     Channels to send notifications to when reports have been generated.
     """
 
     sns: dict[str, SnsTopicChannel] | None = None
 
 
 @dataclass
+class Iam:
+    ProfileName: str | None = None
+    AssumeRole: AssumeRole | None = None
+
+
+IamOverride = Union[str, AssumeRole]
+
+
+@dataclass
+class MskProvider:
+    iam_override: IamOverride | None = None
+    """
+    Override default session to perform the clusters discovery
+    """
+    exclude_regions: list[str] | None = None
+    """
+    List of regions not to look for MSK clusters
+    """
+
+
+@dataclass
+class SaaSProviderAwsSecretsManager:
+    secret_id: str | None = None
+    """
+    Name or ARN of secret to use to store the key. If ARN is detected, existing secret content will be updated. If name is provided but not found, creates new secret.
+    """
+    iam_override: IamOverride | None = None
+
+
+@dataclass
+class GovernanceReportingConfig:
+    """
+    Configuration for governance cluster analysis
+    """
+
+    topic_naming_convention: NamingConvention | None = None
+    consumer_groups_naming_convention: NamingConvention | None = None
+
+
+@dataclass
+class AwsGlueSchemaRegistry:
+    """
+    AWS Glue Schema Registry configuration.
+    """
+
+    registry_arn: str
+    iam_override: IamOverride | None = None
+
+
+@dataclass
+class ClusterReportingNotificationChannels:
+    """
+    Channels to send notifications to when reports have been generated.
+    """
+
+    sns: list[ClusterReportSnsChannel] | None = None
+    """
+    List of SNS channels defined in notifications_channels
+    """
+
+
+@dataclass
 class S3Output:
-    BucketName: str | None = None
+    bucket_name: str | None = None
     """
     Name of the S3 bucket
     """
-    PrefixKey: str | None = ""
+    prefix_key: str | None = ""
     """
     Path in the bucket.
     """
-    IamOverride: IamOverride | None = None
+    iam_override: IamOverride | None = None
 
 
 @dataclass
-class ReportingConfig:
+class Exports:
     """
-    Configure reporting output. Applies to all clusters.
+    Reporting export locations
     """
 
-    evaluation_period_in_seconds: int | None = 60
-    """
-    Time to wait before generating reports
-    """
     S3: S3Output | None = None
     local: str | None = "/tmp/kafka-overwatch-reports/"
     """
     Local directory to store the reports to.
     """
     kafka: dict[str, Any] | None = None
     """
     Configuration to persist reports into Kafka. Not yet implemented.
     """
 
 
 @dataclass
+class ReportingConfig:
+    """
+    Configure reporting output. Applies to all clusters.
+    """
+
+    evaluation_period_in_seconds: int | None = 60
+    """
+    Interval between reports.
+    """
+    notification_channels: ClusterReportingNotificationChannels | None = None
+    output_formats: OutputFormats | None = None
+    """
+    The different types of outputs to produce.
+    """
+    exports: Exports | None = None
+    """
+    Reporting export locations
+    """
+
+
+@dataclass
 class ClusterConfigAuth:
     """
     Allows to set override configuration for secret values interpolation
     """
 
     iam_override: IamOverride | None = None
 
 
 @dataclass
 class ClusterConfig:
-    kafka: dict[str, Any]
+    kafka: dict[str, Any] | None = None
     """
     Configuration as documented in https://github.com/confluentinc/librdkafka/blob/master/CONFIGURATION.md
     """
+    schema_registry: str | None = None
+    """
+    Name of the schema registry defined at the top level.
+    """
     cluster_config_auth: ClusterConfigAuth | None = None
     """
     Allows to set override configuration for secret values interpolation
     """
 
 
 @dataclass
@@ -222,26 +351,120 @@
     )
     """
     List the types of backups you want to generate.
     """
 
 
 @dataclass
+class SaveCredentials:
+    """
+    Optional - If set, will save the generated credentials for the cluster
+    """
+
+    aws_secrets_manager: SaaSProviderAwsSecretsManager | None = None
+
+
+@dataclass
+class KafkaServiceAccount:
+    name: str | None = "kafka-overwatch"
+    """
+    Name of the Confluent service account to create
+    """
+    description: str | None = "kafka-overwatch"
+    """
+    Service account description
+    """
+    allow_create: bool | None = True
+    """
+    If the service account with the ServiceAccountName is not found, creates one. If false and cannot find service account, provider will be failed.
+    """
+    save_credentials: SaveCredentials | None = None
+    """
+    Optional - If set, will save the generated credentials for the cluster
+    """
+
+
+@dataclass
+class ConfluentProvider:
+    """
+    Confluent Cloud settings to use to perform the discovery
+    """
+
+    confluent_cloud_auth: ConfluentCloudAuth | None = None
+    kafka_service_account: KafkaServiceAccount | None = None
+
+
+@dataclass
+class BackupConfig:
+    """
+    Configuration for schema registry schemas & subjects backup
+    """
+
+    enabled: bool | None = None
+    """
+    Turn backup on
+    """
+    backup_interval_seconds: int | None = None
+    S3: S3Output | None = None
+
+
+@dataclass
+class SchemaRegistry:
+    config: ConfluentSchemaRegistry | AwsGlueSchemaRegistry
+    backup_config: BackupConfig | None = None
+    """
+    Configuration for schema registry schemas & subjects backup
+    """
+    schema_registry_scan_interval: int | None = 300
+    """
+    Interval, in seconds, between two scans of the schema registry.
+    """
+
+
+@dataclass
+class Providers:
+    """
+    Allows to define a Kafka SaaS provider and perform discovery of existing clusters to scan. (Not yet implemented)
+    """
+
+    aiven: Any | None = None
+    aws_msk: MskProvider | None = None
+    """
+    AWS MSK Clusters discovery
+    """
+    confluent_cloud: ConfluentProvider | None = None
+    """
+    Confluent Cloud environments & clusters discovery.
+    """
+    conduktor_gateway: dict[str, GatewayConfiguration] | None = None
+    """
+    Gateways to monitor and import the vClusters from the partitions usage
+    """
+
+
+@dataclass
+class MskClusterConfig:
+    cluster_arn: str | None = None
+    """
+    The ARN of the MSK Cluster. This will be used to get the cluster details, including bootstrap details.
+    """
+    schema_registry: SchemaRegistry | None = None
+    iam: Iam | None = None
+
+
+@dataclass
 class ClusterConfiguration:
-    cluster_config: ClusterConfig
+    cluster_config: ClusterConfig | MskClusterConfig
     reporting_config: ReportingConfig
     cluster_scan_interval_in_seconds: ClusterScanIntervalInSeconds | None = 60
     """
     Overrides the global setting
     """
+    governance: GovernanceReportingConfig | None = None
     topics_backup_config: ClusterTopicBackupConfig | None = None
-    awareness_topic: str | None = "_overwatchAwareness"
-    """
-    Name of a topic that the Overwatch will subscribe to. This allows multiple instances of the overwatch to be aware and disable features that shouldn't be distributed
-    """
     topic_include_regexes: Regexes | None = None
     topic_exclude_regexes: Regexes | None = None
     metrics: ClusterMetrics | None = None
     """
     Configure metrics export for the cluster
     """
 
@@ -250,20 +473,24 @@
 class KafkaOverwatchInputConfiguration:
     """
     Specification for Kafka topics/partitions hunter service
     """
 
     global_: Global | None = None
     """
-    Global settings. Apply to all clusters
+    Global settings. Defines global default values that can be overriden for each cluster.
     """
     clusters: dict[str, ClusterConfiguration] | None = None
     """
     Kafka clusters to monitor and report on the partitions usage
     """
-    gateways: dict[str, GatewayConfiguration] | None = None
+    providers: Providers | None = None
     """
-    Gateways to monitor and import the vClusters from the partitions usage
+    Allows to define a Kafka SaaS provider and perform discovery of existing clusters to scan. (Not yet implemented)
     """
     prometheus: Any | None = None
     notification_channels: NotificationChannels | None = None
+    """
+    Allows to define notification channels for reporting (not yet implemented).
+    """
+    schema_registries: dict[str, SchemaRegistry] | dict[str, Any] | None = None
     aws_emf: AwsEmfModel | None = None
```

### Comparing `kafka_overwatch-0.0.2/kafka_overwatch/specs/report.json` & `kafka_overwatch-0.2.0/kafka_overwatch/specs/report.json`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9531094990079365%*

 * *Differences: {"'definitions'": "{'ClusterReport': {'required': {delete: [1]}, 'properties': {'statistics': "*

 * *                  "{'properties': {'most_active_topics': OrderedDict([('description', 'Topics in "*

 * *                  'the 0.75 percentile of number of messages and new_messages which active '*

 * *                  "consumer groups'), ('oneOf', [OrderedDict([('type', 'array'), ('items', "*

 * *                  "OrderedDict([('type', 'string')]))]), OrderedDict([('type', 'object')])])])}}, "*

 * *                  "'estimated_w […]*

```diff
@@ -10,32 +10,55 @@
                 },
                 "estimated_waste": {
                     "properties": {
                         "partitions": {
                             "description": "Sum of partitions for the topics",
                             "type": "integer"
                         },
+                        "topic_categories": {
+                            "patternProperties": {
+                                "^[a-zA-Z0-9]+": {
+                                    "$ref": "#/definitions/topic_waste_category"
+                                }
+                            },
+                            "type": "object"
+                        },
                         "topics": {
                             "type": "integer"
                         }
                     },
                     "type": "object"
                 },
+                "governance": {
+                    "description": "Governance report structure",
+                    "properties": {
+                        "consumer_group_naming_convention": {
+                            "$ref": "#/definitions/governance_naming_convention_report"
+                        },
+                        "topic_naming_convention": {
+                            "$ref": "#/definitions/governance_naming_convention_report"
+                        }
+                    },
+                    "type": "object"
+                },
                 "metadata": {
                     "properties": {
                         "timestamp": {
                             "description": "Time the report was generated at",
                             "type": "string"
                         }
                     },
                     "required": [
                         "timestamp"
                     ],
                     "type": "object"
                 },
+                "schema_registry": {
+                    "$ref": "#/definitions/schema_registry_report"
+                },
                 "statistics": {
                     "additionalProperties": false,
                     "properties": {
                         "consumer_groups": {
                             "additionalProperties": false,
                             "properties": {
                                 "active": {
@@ -52,100 +75,158 @@
                                 }
                             },
                             "required": [
                                 "total"
                             ],
                             "type": "object"
                         },
+                        "most_active_topics": {
+                            "description": "Topics in the 0.75 percentile of number of messages and new_messages which active consumer groups",
+                            "oneOf": [
+                                {
+                                    "items": {
+                                        "type": "string"
+                                    },
+                                    "type": "array"
+                                },
+                                {
+                                    "type": "object"
+                                }
+                            ]
+                        },
                         "partitions": {
                             "description": "Sum of partitions for the topics",
                             "type": "integer"
                         },
                         "topics": {
                             "description": "Total count of topics counted at the time of generating the report",
                             "type": "integer"
                         }
                     },
                     "required": [
                         "topics"
                     ],
                     "type": "object"
-                },
-                "topics": {
-                    "patternProperties": {
-                        "^[a-zA-Z0-9\\.\\_\\-]+": {
-                            "$ref": "#/definitions/topic"
-                        }
-                    },
-                    "type": "object"
                 }
             },
             "required": [
                 "cluster_name",
-                "topics",
                 "metadata"
             ],
             "type": "object"
         },
-        "topic": {
+        "governance_naming_convention_report": {
             "properties": {
-                "consumption": {
-                    "properties": {
-                        "active_consumer_groups_count": {
-                            "description": "Number of active consumer groups (lag = 0)",
-                            "type": "integer"
-                        },
-                        "inactive_consumer_groups_count": {
-                            "description": "Number of inactive consumer groups (lag > 0) or groups without members",
-                            "type": "integer"
-                        }
-                    },
-                    "type": "object"
+                "compliant_percentage": {
+                    "description": "Percentage of compliant consumer_groups, out of total_topic_measured",
+                    "maximum": 100,
+                    "minimum": 0,
+                    "type": "number"
+                },
+                "non_compliant_resources": {
+                    "description": "List of non-compliant topic names",
+                    "items": {
+                        "description": "Topic name that is not compliant",
+                        "type": "string"
+                    },
+                    "type": "array"
+                },
+                "total": {
+                    "description": "Total number of consumer_groups in the cluster",
+                    "minimum": 1,
+                    "type": "number"
+                },
+                "total_ignored": {
+                    "description": "Total number of consumer_groups ignored via regex",
+                    "minimum": 0,
+                    "type": "number"
+                },
+                "total_measured": {
+                    "description": "Total number of consumer_groups measured",
+                    "minimum": 0,
+                    "type": "number"
+                }
+            },
+            "type": "object"
+        },
+        "schema_registry_report": {
+            "additionalProperties": false,
+            "patternProperties": {
+                "x-": {}
+            },
+            "properties": {
+                "schemas_count": {
+                    "minimum": 0,
+                    "type": "integer"
                 },
-                "new_messages_observed": {
-                    "properties": {
-                        "count": {
-                            "description": "Number of new messages observed, as per offset ends changed",
-                            "type": "integer"
-                        },
-                        "elapsed_time": {
-                            "description": "Amount of time in seconds passed for the evaluation",
-                            "type": "integer"
-                        }
+                "schemas_estimates": {
+                    "$ref": "#/definitions/schemas_waste_estimates"
+                },
+                "subjects_count": {
+                    "minimum": 0,
+                    "type": "integer"
+                }
+            },
+            "type": "object"
+        },
+        "schemas_waste_estimates": {
+            "additionalProperties": false,
+            "patternProperties": {
+                "x-": {}
+            },
+            "properties": {
+                "detected_unused": {
+                    "items": {
+                        "type": "string"
                     },
-                    "required": [
-                        "count",
-                        "elapsed_time"
-                    ],
-                    "type": "object"
+                    "type": "array"
+                },
+                "detected_unused_count": {
+                    "minimum": 0,
+                    "type": "integer"
+                }
+            },
+            "type": "object"
+        },
+        "topic_waste_category": {
+            "properties": {
+                "cluster_percentage": {
+                    "description": "The percentage of topics fit into that category within the cluster",
+                    "maximum": 100,
+                    "minimum": 0,
+                    "type": "number"
+                },
+                "description": {
+                    "description": "The description of the category",
+                    "type": "string"
                 },
-                "partitions_count": {
-                    "description": "Number of partitions for the topic",
+                "topic_partitions_sum": {
+                    "minimum": 1,
                     "type": "integer"
                 },
-                "recommendation": {
-                    "properties": {
-                        "description": {
-                            "description": "Recommendation for the topic",
-                            "type": "string"
-                        },
-                        "suggested_actions": {
-                            "description": "List of suggested actions",
-                            "items": {
-                                "type": "string"
-                            },
-                            "type": "array"
+                "topics": {
+                    "additionalProperties": false,
+                    "patternProperties": {
+                        "[a-zA-Z0-9_.\\-]{3,256}": {
+                            "description": "Topic Name: Partitions count",
+                            "minimum": 1,
+                            "type": "integer"
                         }
                     },
                     "type": "object"
+                },
+                "topics_count": {
+                    "minimum": 1,
+                    "type": "integer"
                 }
             },
             "required": [
-                "partitions_count",
-                "new_messages_observed"
+                "topics",
+                "topic_partitions_sum",
+                "description"
             ],
             "type": "object"
         }
     },
     "description": "Defines the format of the cluster topics report",
     "id": "report_structure.spec.json",
     "properties": {
```

### Comparing `kafka_overwatch-0.0.2/pyproject.toml` & `kafka_overwatch-0.2.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kafka-overwatch"
-version = "0.0.2"
+version = "0.2.0"
 description = "Continuously monitors Kafka cluster topics & consumer groups"
 authors = ["John \"Preston\" Mille <john@ews-network.net>"]
 maintainers = ["John \"Preston\" Mille <john@ews-network.net>"]
 readme = "README.rst"
 license = "MPL-2.0"
 keywords = ["kafka", "monitoring", "reporting", "usage-analysis", "cost-savings"]
 
@@ -25,36 +25,48 @@
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/JohnPreston/kafka-overwatch/issues"
 
 
 [tool.poetry.dependencies]
 python = "^3.10"
 confluent-kafka = "^2.3.0"
-compose-x-common = "^1.4.3"
-boto3 = ">=1.34,<2.0"
+compose-x-common = "^1.4.4"
+boto3 = ">=1.26,<2.0"
 dacite = "^1.8.1"
 pyyaml = "^6.0.1"
-aws-cfn-custom-resource-resolve-parser = "^0.3.1"
+aws-cfn-custom-resource-resolve-parser = "^0.3"
 retry2 = "^0.9.5"
 jsonschema = "^4.20.0"
 aws-embedded-metrics = "^3.2.0"
 importlib-resources = "^6.1.1"
 prometheus-client = "^0.19.0"
-
+jinja2 = "^3.1.2"
+aws-msk-iam-sasl-signer-python = "^1.0.0"
+pandas = "^2.1.4"
+codeguru-profiler-agent = "^1.2.4"
+kafka-schema-registry-admin = ">=0.5"
+cryptography = "^42.0.5"
 
 [tool.poetry.group.dev.dependencies]
-black = "^23.12"
+black = ">=23.12,<25.0"
 isort = "^5.13"
 pyupgrade = "^3.15"
 pre-commit = "^3.6"
 datamodel-code-generator = "^0.25.1"
 pytest = "^7.4"
 testcontainers = "^3.7.1"
 tbump = "^6.11.0"
 
+
+[tool.poetry.group.docs.dependencies]
+sphinx = "^7.2.6"
+sphinx-jsonschema = "^1.19.1"
+sphinx-material = "^0.0.36"
+sphinx-autodoc-typehints = "^1.25.2"
+
 [tool.poetry.scripts]
 kafka-overwatch = "kafka_overwatch.cli:main"
 
 [tool.black]
 line-length = 88
 
 [tool.isort]
@@ -75,15 +87,15 @@
   "*/cli.py"
 ]
 
 [tool.tbump]
 github_url = "https://github.com/johnpreston/kafka-overwatch"
 
 [tool.tbump.version]
-current = "0.0.2"
+current = "0.2.0"
 regex = '''
   (?P<major>\d+)
   \.
   (?P<minor>\d+)
   \.
   (?P<patch>\d+)
   (?:(?P<rc>[\S]+))?
```

### Comparing `kafka_overwatch-0.0.2/PKG-INFO` & `kafka_overwatch-0.2.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kafka-overwatch
-Version: 0.0.2
+Version: 0.2.0
 Summary: Continuously monitors Kafka cluster topics & consumer groups
 License: MPL-2.0
 Keywords: kafka,monitoring,reporting,usage-analysis,cost-savings
 Author: John "Preston" Mille
 Author-email: john@ews-network.net
 Maintainer: John "Preston" Mille
 Maintainer-email: john@ews-network.net
@@ -15,22 +15,28 @@
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: aws-cfn-custom-resource-resolve-parser (>=0.3.1,<0.4.0)
+Requires-Dist: aws-cfn-custom-resource-resolve-parser (>=0.3,<0.4)
 Requires-Dist: aws-embedded-metrics (>=3.2.0,<4.0.0)
-Requires-Dist: boto3 (>=1.34,<2.0)
-Requires-Dist: compose-x-common (>=1.4.3,<2.0.0)
+Requires-Dist: aws-msk-iam-sasl-signer-python (>=1.0.0,<2.0.0)
+Requires-Dist: boto3 (>=1.26,<2.0)
+Requires-Dist: codeguru-profiler-agent (>=1.2.4,<2.0.0)
+Requires-Dist: compose-x-common (>=1.4.4,<2.0.0)
 Requires-Dist: confluent-kafka (>=2.3.0,<3.0.0)
+Requires-Dist: cryptography (>=42.0.5,<43.0.0)
 Requires-Dist: dacite (>=1.8.1,<2.0.0)
 Requires-Dist: importlib-resources (>=6.1.1,<7.0.0)
+Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: jsonschema (>=4.20.0,<5.0.0)
+Requires-Dist: kafka-schema-registry-admin (>=0.5)
+Requires-Dist: pandas (>=2.1.4,<3.0.0)
 Requires-Dist: prometheus-client (>=0.19.0,<0.20.0)
 Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
 Requires-Dist: retry2 (>=0.9.5,<0.10.0)
 Project-URL: Bug Tracker, https://github.com/JohnPreston/kafka-overwatch/issues
 Description-Content-Type: text/x-rst
 
 ========================================
@@ -103,7 +109,24 @@
 .. _EMF: https://docs.aws.amazon.com/AmazonCloudWatch/latest/monitoring/CloudWatch_Embedded_Metric_Format_Specification.html
 .. _kafka-idle-topics: https://github.com/abraham-leal/kafka-idle-topics
 .. _cfn-kafka-admin: https://github.com/compose-x/cfn-kafka-admin
 .. _cruise-control: https://github.com/linkedin/cruise-control
 .. _jsonschema: https://pypi.org/project/jsonschema/
 .. _NASA: https://www.nasa.gov/
 
+
+Status
+=======
+
+Images build status
+
+|BUILD|
+
+Docs build status
+
+|DOCS_BUILD|
+
+
+.. |BUILD| image:: https://codebuild.eu-west-1.amazonaws.com/badges?uuid=eyJlbmNyeXB0ZWREYXRhIjoiU3RHQnZ2eFpnQTlOSmU2MUM3NDB5NW9uMDY2TS9DZXBWZ2hmejdoK2xJRStHK2Fhd3FkS1FoQjJOSTcvYjVBNkFTTW5kVDNZK0NqZEthU3gveFpOVEljPSIsIml2UGFyYW1ldGVyU3BlYyI6IjlUbE0vNmpPQU92U1o0SmkiLCJtYXRlcmlhbFNldFNlcmlhbCI6MX0%3D&branch=main
+
+.. |DOCS_BUILD| image:: https://codebuild.eu-west-1.amazonaws.com/badges?uuid=eyJlbmNyeXB0ZWREYXRhIjoiSVNBZkVSUkx1NHhtamlqSEJqempIdHd2aVNqV2RkTTFVYlphUzJ2ekprOVU4ODZ4cUNWcTNVSkRVM2ovcGFyak5NTTNJZ1Vra2ErSzVOdi84TkVLOUp3PSIsIml2UGFyYW1ldGVyU3BlYyI6IjAvK25MSmNPcjNScVpwdTQiLCJtYXRlcmlhbFNldFNlcmlhbCI6MX0%3D&branch=main
+
```

