# Comparing `tmp/diaspora-event-sdk-0.1.6.tar.gz` & `tmp/diaspora-event-sdk-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "diaspora-event-sdk-0.1.6.tar", last modified: Wed Mar 20 20:25:42 2024, max compression
+gzip compressed data, was "diaspora-event-sdk-0.1.7.tar", last modified: Sun Apr  7 17:23:12 2024, max compression
```

## Comparing `diaspora-event-sdk-0.1.6.tar` & `diaspora-event-sdk-0.1.7.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 haochen    (501) staff       (20)        0 2024-03-20 20:25:42.736430 diaspora-event-sdk-0.1.6/
--rw-r--r--   0 haochen    (501) staff       (20)    11357 2023-11-25 23:14:02.000000 diaspora-event-sdk-0.1.6/LICENSE
--rw-r--r--   0 haochen    (501) staff       (20)       58 2023-12-01 02:49:57.000000 diaspora-event-sdk-0.1.6/MANIFEST.in
--rw-r--r--   0 haochen    (501) staff       (20)     2477 2024-03-20 20:25:42.735500 diaspora-event-sdk-0.1.6/PKG-INFO
--rw-r--r--   0 haochen    (501) staff       (20)     1722 2024-03-01 21:27:50.000000 diaspora-event-sdk-0.1.6/README.md
-drwxr-xr-x   0 haochen    (501) staff       (20)        0 2024-03-20 20:25:42.720274 diaspora-event-sdk-0.1.6/diaspora_event_sdk/
--rw-r--r--   0 haochen    (501) staff       (20)      457 2023-12-06 16:48:23.000000 diaspora-event-sdk-0.1.6/diaspora_event_sdk/__init__.py
-drwxr-xr-x   0 haochen    (501) staff       (20)        0 2024-03-20 20:25:42.724491 diaspora-event-sdk-0.1.6/diaspora_event_sdk/sdk/
--rw-r--r--   0 haochen    (501) staff       (20)        0 2023-11-25 23:14:02.000000 diaspora-event-sdk-0.1.6/diaspora_event_sdk/sdk/__init__.py
--rw-r--r--   0 haochen    (501) staff       (20)      203 2024-01-26 20:44:42.000000 diaspora-event-sdk-0.1.6/diaspora_event_sdk/sdk/_environments.py
--rw-r--r--   0 haochen    (501) staff       (20)     7321 2024-03-20 19:50:43.000000 diaspora-event-sdk-0.1.6/diaspora_event_sdk/sdk/client.py
--rw-r--r--   0 haochen    (501) staff       (20)      884 2023-11-28 14:17:53.000000 diaspora-event-sdk-0.1.6/diaspora_event_sdk/sdk/decorators.py
--rw-r--r--   0 haochen    (501) staff       (20)     4361 2024-01-27 14:28:34.000000 diaspora-event-sdk-0.1.6/diaspora_event_sdk/sdk/kafka_client.py
-drwxr-xr-x   0 haochen    (501) staff       (20)        0 2024-03-20 20:25:42.729337 diaspora-event-sdk-0.1.6/diaspora_event_sdk/sdk/login_manager/
--rw-r--r--   0 haochen    (501) staff       (20)      239 2023-11-25 23:14:02.000000 diaspora-event-sdk-0.1.6/diaspora_event_sdk/sdk/login_manager/__init__.py
--rw-r--r--   0 haochen    (501) staff       (20)     1798 2023-11-25 23:14:02.000000 diaspora-event-sdk-0.1.6/diaspora_event_sdk/sdk/login_manager/client_login.py
--rw-r--r--   0 haochen    (501) staff       (20)     1047 2023-11-25 23:14:02.000000 diaspora-event-sdk-0.1.6/diaspora_event_sdk/sdk/login_manager/decorators.py
--rw-r--r--   0 haochen    (501) staff       (20)      389 2023-11-25 23:14:02.000000 diaspora-event-sdk-0.1.6/diaspora_event_sdk/sdk/login_manager/globus_auth.py
--rw-r--r--   0 haochen    (501) staff       (20)      954 2023-11-25 23:14:02.000000 diaspora-event-sdk-0.1.6/diaspora_event_sdk/sdk/login_manager/login_flow.py
--rw-r--r--   0 haochen    (501) staff       (20)     7040 2024-01-27 13:52:46.000000 diaspora-event-sdk-0.1.6/diaspora_event_sdk/sdk/login_manager/manager.py
--rw-r--r--   0 haochen    (501) staff       (20)      710 2023-11-25 23:14:02.000000 diaspora-event-sdk-0.1.6/diaspora_event_sdk/sdk/login_manager/protocol.py
--rw-r--r--   0 haochen    (501) staff       (20)     2094 2023-12-07 20:06:52.000000 diaspora-event-sdk-0.1.6/diaspora_event_sdk/sdk/login_manager/tokenstore.py
-drwxr-xr-x   0 haochen    (501) staff       (20)        0 2024-03-20 20:25:42.730449 diaspora-event-sdk-0.1.6/diaspora_event_sdk/sdk/utils/
--rw-r--r--   0 haochen    (501) staff       (20)        0 2023-11-25 23:14:02.000000 diaspora-event-sdk-0.1.6/diaspora_event_sdk/sdk/utils/__init__.py
--rw-r--r--   0 haochen    (501) staff       (20)      470 2023-11-28 14:18:09.000000 diaspora-event-sdk-0.1.6/diaspora_event_sdk/sdk/utils/uuid_like.py
--rw-r--r--   0 haochen    (501) staff       (20)     4332 2024-03-20 20:19:05.000000 diaspora-event-sdk-0.1.6/diaspora_event_sdk/sdk/web_client.py
--rw-r--r--   0 haochen    (501) staff       (20)       22 2024-03-20 19:50:52.000000 diaspora-event-sdk-0.1.6/diaspora_event_sdk/version.py
-drwxr-xr-x   0 haochen    (501) staff       (20)        0 2024-03-20 20:25:42.732606 diaspora-event-sdk-0.1.6/diaspora_event_sdk.egg-info/
--rw-r--r--   0 haochen    (501) staff       (20)     2477 2024-03-20 20:25:42.000000 diaspora-event-sdk-0.1.6/diaspora_event_sdk.egg-info/PKG-INFO
--rw-r--r--   0 haochen    (501) staff       (20)     1068 2024-03-20 20:25:42.000000 diaspora-event-sdk-0.1.6/diaspora_event_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 haochen    (501) staff       (20)        1 2024-03-20 20:25:42.000000 diaspora-event-sdk-0.1.6/diaspora_event_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 haochen    (501) staff       (20)      141 2024-03-20 20:25:42.000000 diaspora-event-sdk-0.1.6/diaspora_event_sdk.egg-info/requires.txt
--rw-r--r--   0 haochen    (501) staff       (20)       25 2024-03-20 20:25:42.000000 diaspora-event-sdk-0.1.6/diaspora_event_sdk.egg-info/top_level.txt
--rw-r--r--   0 haochen    (501) staff       (20)       38 2024-03-20 20:25:42.736616 diaspora-event-sdk-0.1.6/setup.cfg
--rw-r--r--   0 haochen    (501) staff       (20)     1389 2024-01-26 15:40:24.000000 diaspora-event-sdk-0.1.6/setup.py
-drwxr-xr-x   0 haochen    (501) staff       (20)        0 2024-03-20 20:25:42.731319 diaspora-event-sdk-0.1.6/tests/
--rw-r--r--   0 haochen    (501) staff       (20)        0 2023-11-29 19:23:13.000000 diaspora-event-sdk-0.1.6/tests/__init__.py
-drwxr-xr-x   0 haochen    (501) staff       (20)        0 2024-03-20 20:25:42.731814 diaspora-event-sdk-0.1.6/tests/unit/
--rw-r--r--   0 haochen    (501) staff       (20)     2995 2024-01-27 14:42:11.000000 diaspora-event-sdk-0.1.6/tests/unit/test_client.py
--rw-r--r--   0 haochen    (501) staff       (20)      236 2024-01-27 14:28:21.000000 diaspora-event-sdk-0.1.6/tox.ini
+drwxr-xr-x   0 haochen    (501) staff       (20)        0 2024-04-07 17:23:12.505994 diaspora-event-sdk-0.1.7/
+-rw-r--r--   0 haochen    (501) staff       (20)    11357 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.1.7/LICENSE
+-rw-r--r--   0 haochen    (501) staff       (20)       58 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.1.7/MANIFEST.in
+-rw-r--r--   0 haochen    (501) staff       (20)     2092 2024-04-07 17:23:12.505867 diaspora-event-sdk-0.1.7/PKG-INFO
+-rw-r--r--   0 haochen    (501) staff       (20)     1722 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.1.7/README.md
+drwxr-xr-x   0 haochen    (501) staff       (20)        0 2024-04-07 17:23:12.502589 diaspora-event-sdk-0.1.7/diaspora_event_sdk/
+-rw-r--r--   0 haochen    (501) staff       (20)      457 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.1.7/diaspora_event_sdk/__init__.py
+drwxr-xr-x   0 haochen    (501) staff       (20)        0 2024-04-07 17:23:12.504078 diaspora-event-sdk-0.1.7/diaspora_event_sdk/sdk/
+-rw-r--r--   0 haochen    (501) staff       (20)        0 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.1.7/diaspora_event_sdk/sdk/__init__.py
+-rw-r--r--   0 haochen    (501) staff       (20)      204 2024-04-07 13:11:12.000000 diaspora-event-sdk-0.1.7/diaspora_event_sdk/sdk/_environments.py
+-rw-r--r--   0 haochen    (501) staff       (20)     6834 2024-04-07 13:36:26.000000 diaspora-event-sdk-0.1.7/diaspora_event_sdk/sdk/client.py
+-rw-r--r--   0 haochen    (501) staff       (20)      884 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.1.7/diaspora_event_sdk/sdk/decorators.py
+-rw-r--r--   0 haochen    (501) staff       (20)     4361 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.1.7/diaspora_event_sdk/sdk/kafka_client.py
+drwxr-xr-x   0 haochen    (501) staff       (20)        0 2024-04-07 17:23:12.505129 diaspora-event-sdk-0.1.7/diaspora_event_sdk/sdk/login_manager/
+-rw-r--r--   0 haochen    (501) staff       (20)      239 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.1.7/diaspora_event_sdk/sdk/login_manager/__init__.py
+-rw-r--r--   0 haochen    (501) staff       (20)     1798 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.1.7/diaspora_event_sdk/sdk/login_manager/client_login.py
+-rw-r--r--   0 haochen    (501) staff       (20)     1047 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.1.7/diaspora_event_sdk/sdk/login_manager/decorators.py
+-rw-r--r--   0 haochen    (501) staff       (20)      389 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.1.7/diaspora_event_sdk/sdk/login_manager/globus_auth.py
+-rw-r--r--   0 haochen    (501) staff       (20)      954 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.1.7/diaspora_event_sdk/sdk/login_manager/login_flow.py
+-rw-r--r--   0 haochen    (501) staff       (20)     7040 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.1.7/diaspora_event_sdk/sdk/login_manager/manager.py
+-rw-r--r--   0 haochen    (501) staff       (20)      710 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.1.7/diaspora_event_sdk/sdk/login_manager/protocol.py
+-rw-r--r--   0 haochen    (501) staff       (20)     2094 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.1.7/diaspora_event_sdk/sdk/login_manager/tokenstore.py
+drwxr-xr-x   0 haochen    (501) staff       (20)        0 2024-04-07 17:23:12.505317 diaspora-event-sdk-0.1.7/diaspora_event_sdk/sdk/utils/
+-rw-r--r--   0 haochen    (501) staff       (20)        0 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.1.7/diaspora_event_sdk/sdk/utils/__init__.py
+-rw-r--r--   0 haochen    (501) staff       (20)      470 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.1.7/diaspora_event_sdk/sdk/utils/uuid_like.py
+-rw-r--r--   0 haochen    (501) staff       (20)     3630 2024-04-07 13:33:42.000000 diaspora-event-sdk-0.1.7/diaspora_event_sdk/sdk/web_client.py
+-rw-r--r--   0 haochen    (501) staff       (20)       22 2024-04-07 13:08:18.000000 diaspora-event-sdk-0.1.7/diaspora_event_sdk/version.py
+drwxr-xr-x   0 haochen    (501) staff       (20)        0 2024-04-07 17:23:12.503134 diaspora-event-sdk-0.1.7/diaspora_event_sdk.egg-info/
+-rw-r--r--   0 haochen    (501) staff       (20)     2092 2024-04-07 17:23:12.000000 diaspora-event-sdk-0.1.7/diaspora_event_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 haochen    (501) staff       (20)     1068 2024-04-07 17:23:12.000000 diaspora-event-sdk-0.1.7/diaspora_event_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 haochen    (501) staff       (20)        1 2024-04-07 17:23:12.000000 diaspora-event-sdk-0.1.7/diaspora_event_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 haochen    (501) staff       (20)      141 2024-04-07 17:23:12.000000 diaspora-event-sdk-0.1.7/diaspora_event_sdk.egg-info/requires.txt
+-rw-r--r--   0 haochen    (501) staff       (20)       25 2024-04-07 17:23:12.000000 diaspora-event-sdk-0.1.7/diaspora_event_sdk.egg-info/top_level.txt
+-rw-r--r--   0 haochen    (501) staff       (20)       38 2024-04-07 17:23:12.506039 diaspora-event-sdk-0.1.7/setup.cfg
+-rw-r--r--   0 haochen    (501) staff       (20)     1389 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.1.7/setup.py
+drwxr-xr-x   0 haochen    (501) staff       (20)        0 2024-04-07 17:23:12.505427 diaspora-event-sdk-0.1.7/tests/
+-rw-r--r--   0 haochen    (501) staff       (20)        0 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.1.7/tests/__init__.py
+drwxr-xr-x   0 haochen    (501) staff       (20)        0 2024-04-07 17:23:12.505526 diaspora-event-sdk-0.1.7/tests/unit/
+-rw-r--r--   0 haochen    (501) staff       (20)     2995 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.1.7/tests/unit/test_client.py
+-rw-r--r--   0 haochen    (501) staff       (20)      236 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.1.7/tox.ini
```

### Comparing `diaspora-event-sdk-0.1.6/LICENSE` & `diaspora-event-sdk-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `diaspora-event-sdk-0.1.6/PKG-INFO` & `diaspora-event-sdk-0.1.7/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,18 @@
 Metadata-Version: 2.1
 Name: diaspora-event-sdk
-Version: 0.1.6
+Version: 0.1.7
 Summary: SDK of Diaspora Event Fabric: Resilience-enabling services for science from HPC to edge
 Home-page: https://github.com/globus-labs/diaspora-event-sdk
 License: LICENSE
+Platform: UNKNOWN
 Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: globus-sdk<4,>=3.20.1
 Provides-Extra: kafka-python
-Requires-Dist: kafka-python; extra == "kafka-python"
-Requires-Dist: aws-msk-iam-sasl-signer-python; extra == "kafka-python"
 Provides-Extra: test
-Requires-Dist: pytest; extra == "test"
-Requires-Dist: pytest-cov; extra == "test"
-Requires-Dist: coverage; extra == "test"
-Requires-Dist: mypy; extra == "test"
-Requires-Dist: tox; extra == "test"
-Requires-Dist: check-manifest; extra == "test"
+License-File: LICENSE
 
 # Diaspora: Resilience-enabling services for science from HPC to edge
 
 ## Event Fabric SDK Installation Guide
 ### Recommended Method: Use with `kafka-python`
 For easy integration with Diaspora Event Fabric, use the `KafkaProducer` and `KafkaConsumer` classes from our SDK. This requires the `kafka-python` library.
 
@@ -43,7 +35,8 @@
 **Getting Started**: Visit our [QuickStart Guide](docs/quickstart.md) for details on using the SDK with the kafka-python library and instructions for other Kafka clients.
 
 **Troubleshooting and Credential Management**: Consult our [TrobleShooting Guide](docs/troubleshooting.md) for solving common issues and tips on managing keys effectively.
 
 **Advanced Consumers with Faust**: Explore the [Faust Streaming Guide](docs/faust_weather_app.md) for advanced event streaming with Faust.
 
 **Advanced Consumer Functions**: See our [Colab example](https://colab.research.google.com/drive/1tPKfxU2qPsLvNTreF6nKINU62k7pQWxa?usp=sharing) for demonstration.
+
```

### Comparing `diaspora-event-sdk-0.1.6/README.md` & `diaspora-event-sdk-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `diaspora-event-sdk-0.1.6/diaspora_event_sdk/sdk/client.py` & `diaspora-event-sdk-0.1.7/diaspora_event_sdk/sdk/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -85,24 +85,14 @@
         else:
             return {
                 "access_key": tokens["access_key"],
                 "secret_key": tokens["secret_key"],
                 "endpoint": tokens["endpoint"],
             }
 
-    # @requires_login  # TODO
-    # def get_secret_key(self):
-    #     tokens = self.login_manager._token_storage.get_token_data(
-    #         DIASPORA_RESOURCE_SERVER
-    #     )
-    #     if tokens is None or "secret_key" not in tokens:
-    #         return None
-    #     else:
-    #         return tokens["secret_key"]
-
     @requires_login
     def put_secret_key(self, access_key, secret_key, endpoint):
         tokens = self.login_manager._token_storage.get_token_data(
             DIASPORA_RESOURCE_SERVER
         )
         tokens["access_key"] = access_key
         tokens["secret_key"] = secret_key
@@ -129,85 +119,78 @@
         return self.web_client.list_topics(self.subject_openid)
 
     @requires_login
     def register_topic(self, topic):
         """
         Registers a new topic under the user's OpenID.
         """
-        return self.web_client.register_topic(self.subject_openid, topic)
+        return self.web_client.register_topic(self.subject_openid, topic, "register")
 
     @requires_login
     def unregister_topic(self, topic):
         """
         Unregisters a topic from the user's OpenID.
         """
-        return self.web_client.unregister_topic(self.subject_openid, topic)
-
-    @requires_login
-    def register_topic_for_user(self, topic, user):
-        """
-        Registers a new topic under the user's OpenID.
-        """
-        return self.web_client.register_topic_for_user(self.subject_openid, topic, user)
+        return self.web_client.register_topic(self.subject_openid, topic, "unregister")
 
     @requires_login
-    def unregister_topic_for_user(self, topic, user):
+    def get_topic_configs(self, topic):
         """
-        Unregisters a topic from the user's OpenID.
+        Get topic configurations.
         """
-        return self.web_client.unregister_topic_for_user(self.subject_openid, topic, user)
+        return self.web_client.get_topic_configs(self.subject_openid, topic)
 
     @requires_login
-    def list_functions(self):
+    def update_topic_configs(self, topic, configs):
         """
-        Retrieves the list of functions associated with the user's OpenID.
+        Set topic configurations.
         """
-        return self.web_client.list_functions(self.subject_openid)
+        return self.web_client.update_topic_configs(self.subject_openid, topic, configs)
 
     @requires_login
-    def register_function(self, topic, function, function_configs):
+    def update_topic_partitions(self, topic, new_partitions):
         """
-        Registers a new functions under the user's OpenID.
+        Adjust topic number of partitions
         """
-        return self.web_client.register_function(self.subject_openid, topic, function, function_configs)
+        return self.web_client.update_topic_partitions(self.subject_openid, topic, new_partitions)
 
     @requires_login
-    def unregister_function(self, topic, function):
+    def grant_user_access(self, topic, user):
         """
-        Unregisters a functions from the user's OpenID.
+        Registers a new topic under the user's OpenID.
         """
-        return self.web_client.unregister_function(self.subject_openid, topic, function)
+        return self.web_client.grant_user_access(self.subject_openid, topic, user, "grant")
 
     @requires_login
-    def update_trigger_config(self, trigger_uuid, trigger_configs):
+    def revoke_user_access(self, topic, user):
         """
-        Update a functions's trigger'.
+        Unregisters a topic from the user's OpenID.
         """
-        return self.web_client.update_function_trigger(self.subject_openid, trigger_uuid, trigger_configs)
+        return self.web_client.grant_user_access(self.subject_openid, topic, user, "revoke")
 
     @requires_login
-    def get_identities(self):
+    def list_triggers(self):
         """
-        Get the user identities.
+        Retrieves the list of functions associated with the user's OpenID.
         """
-        return self.web_client.get_identities(self.subject_openid)
+        return self.web_client.list_triggers(self.subject_openid)
 
     @requires_login
-    def get_topic_configs(self, topic, configs):
+    def create_trigger(self, topic, function, function_configs):
         """
-        Get topic configurations.
+        Registers a new functions under the user's OpenID.
         """
-        return self.web_client.get_topic_configs(self.subject_openid, topic, configs)
+        return self.web_client.create_trigger(self.subject_openid, topic, function, "create", function_configs)
 
     @requires_login
-    def set_topic_configs(self, topic, configs):
+    def delete_trigger(self, topic, function):
         """
-        Set topic configurations.
+        Unregisters a functions from the user's OpenID.
         """
-        return self.web_client.set_topic_configs(self.subject_openid, topic, configs)
+        return self.web_client.create_trigger(self.subject_openid, topic, function, "delete", {})
 
     @requires_login
-    def create_partitions(self, topic, new_partitions):
+    def update_trigger(self, trigger_uuid, trigger_configs):
         """
-        Set topic configurations.
+        Update a functions's trigger'.
         """
-        return self.web_client.create_partitions(self.subject_openid, topic, new_partitions)
+        return self.web_client.update_trigger(self.subject_openid, trigger_uuid, trigger_configs)
```

### Comparing `diaspora-event-sdk-0.1.6/diaspora_event_sdk/sdk/decorators.py` & `diaspora-event-sdk-0.1.7/diaspora_event_sdk/sdk/decorators.py`

 * *Files identical despite different names*

### Comparing `diaspora-event-sdk-0.1.6/diaspora_event_sdk/sdk/kafka_client.py` & `diaspora-event-sdk-0.1.7/diaspora_event_sdk/sdk/kafka_client.py`

 * *Files identical despite different names*

### Comparing `diaspora-event-sdk-0.1.6/diaspora_event_sdk/sdk/login_manager/client_login.py` & `diaspora-event-sdk-0.1.7/diaspora_event_sdk/sdk/login_manager/client_login.py`

 * *Files identical despite different names*

### Comparing `diaspora-event-sdk-0.1.6/diaspora_event_sdk/sdk/login_manager/decorators.py` & `diaspora-event-sdk-0.1.7/diaspora_event_sdk/sdk/login_manager/decorators.py`

 * *Files identical despite different names*

### Comparing `diaspora-event-sdk-0.1.6/diaspora_event_sdk/sdk/login_manager/login_flow.py` & `diaspora-event-sdk-0.1.7/diaspora_event_sdk/sdk/login_manager/login_flow.py`

 * *Files identical despite different names*

### Comparing `diaspora-event-sdk-0.1.6/diaspora_event_sdk/sdk/login_manager/manager.py` & `diaspora-event-sdk-0.1.7/diaspora_event_sdk/sdk/login_manager/manager.py`

 * *Files identical despite different names*

### Comparing `diaspora-event-sdk-0.1.6/diaspora_event_sdk/sdk/login_manager/protocol.py` & `diaspora-event-sdk-0.1.7/diaspora_event_sdk/sdk/login_manager/protocol.py`

 * *Files identical despite different names*

### Comparing `diaspora-event-sdk-0.1.6/diaspora_event_sdk/sdk/login_manager/tokenstore.py` & `diaspora-event-sdk-0.1.7/diaspora_event_sdk/sdk/login_manager/tokenstore.py`

 * *Files identical despite different names*

### Comparing `diaspora-event-sdk-0.1.6/diaspora_event_sdk/sdk/web_client.py` & `diaspora-event-sdk-0.1.7/diaspora_event_sdk/sdk/web_client.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from typing import Optional
-
+import json
 import globus_sdk
 from diaspora_event_sdk.sdk.utils.uuid_like import UUID_LIKE_T
 
 from ._environments import TOKEN_EXCHANGE
 
 
 class WebClient(globus_sdk.BaseClient):
@@ -20,108 +20,80 @@
 
         super().__init__(environment=environment, base_url=base_url, **kwargs)
 
         self._user_app_name = None
         self.user_app_name = app_name
 
     def create_key(self, subject: UUID_LIKE_T) -> globus_sdk.GlobusHTTPResponse:
-        return self.post("/v1/create_key", headers={"Subject": str(subject)})
+        return self.get("/api/v2/create_key", headers={"Subject": str(subject)})
 
     def list_topics(self, subject: UUID_LIKE_T) -> globus_sdk.GlobusHTTPResponse:
-        return self.get("/v1/list_topics", headers={"Subject": str(subject)})
+        return self.get("/api/v2/topics", headers={"Subject": str(subject)})
 
     def register_topic(
-        self, subject: UUID_LIKE_T, topic: str
+        self, subject: UUID_LIKE_T, topic: str, action: str
     ) -> globus_sdk.GlobusHTTPResponse:
-        return self.post(
-            "/v1/register_topic", headers={"Subject": str(subject), "Topic": topic}
+        return self.put(
+            f"/api/v2/topic/{topic}", headers={"Subject": str(subject), "Action": action}
         )
 
-    def unregister_topic(
+    def get_topic_configs(
         self, subject: UUID_LIKE_T, topic: str
     ) -> globus_sdk.GlobusHTTPResponse:
-        return self.post(
-            "/v1/unregister_topic", headers={"Subject": str(subject), "Topic": topic}
-        )
-
-    def register_topic_for_user(
-        self, subject: UUID_LIKE_T, topic: str, user: UUID_LIKE_T
-    ) -> globus_sdk.GlobusHTTPResponse:
-        return self.post(
-            "/v1/register_topic_for_user",
-            headers={"Subject": str(
-                subject), "Topic": topic, "User": str(user)}
-        )
-
-    def unregister_topic_for_user(
-        self, subject: UUID_LIKE_T, topic: str, user: UUID_LIKE_T
-    ) -> globus_sdk.GlobusHTTPResponse:
-        return self.post(
-            "/v1/unregister_topic_for_user",
-            headers={"Subject": str(
-                subject), "Topic": topic, "User": str(user)}
+        return self.get(
+            f"/api/v2/topic/{topic}",
+            headers={"Subject": str(subject), "Topic": topic},
+            # data=json.dumps(configs).encode("utf-8")
         )
 
-    def list_functions(self, subject: UUID_LIKE_T) -> globus_sdk.GlobusHTTPResponse:
-        return self.get("/v1/list_functions", headers={"Subject": str(subject)})
-
-    def register_function(
-        self, subject: UUID_LIKE_T, topic: str, function: str,
-        function_configs: dict
+    def update_topic_configs(
+        self, subject: UUID_LIKE_T, topic: str, configs: dict
     ) -> globus_sdk.GlobusHTTPResponse:
         return self.post(
-            "/v1/register_function",
+            f"/api/v2/topic/{topic}",
             headers={"Subject": str(subject), "Topic": topic,
-                     "Function": function},
-            data=function_configs
-        )
-
-    def unregister_function(
-        self, subject: UUID_LIKE_T, topic: str, function: str
-    ) -> globus_sdk.GlobusHTTPResponse:
-        return self.post(
-            "/v1/unregister_function", headers={"Subject": str(subject), "Topic": topic, "Function": function}
+                     "Content-Type": "text/plain"},
+            data=json.dumps(configs).encode("utf-8")
         )
 
-    def update_function_trigger(
-        self, subject: UUID_LIKE_T, trigger_uuid: UUID_LIKE_T, trigger_configs: dict
+    def update_topic_partitions(
+        self, subject: UUID_LIKE_T, topic: str, new_partitions: int
     ) -> globus_sdk.GlobusHTTPResponse:
         return self.post(
-            "/v1/update_function_trigger",
-            headers={"Subject": str(subject), "Trigger": str(trigger_uuid)},
-            data=trigger_configs
+            f"/api/v2/topic/{topic}/partitions",
+            headers={"Subject": str(subject), "Topic": topic,
+                     "NewPartitions": str(new_partitions)},
         )
 
-    def get_identities(
-        self, subject: UUID_LIKE_T
+    def grant_user_access(
+        self, subject: UUID_LIKE_T, topic: str, user: UUID_LIKE_T, action: str
     ) -> globus_sdk.GlobusHTTPResponse:
         return self.post(
-            "/v1/get_identities",
-            headers={"Subject": str(subject)}
+            f"/api/v2/topic/{topic}/user",
+            headers={"Subject": str(subject), "Action": action,
+                     "Topic": topic, "User": str(user)}
         )
 
-    def get_topic_configs(
-        self, subject: UUID_LIKE_T, topic: str, configs: dict
-    ) -> globus_sdk.GlobusHTTPResponse:
-        return self.post(
-            "/v1/get_topic_configs",
-            headers={"Subject": str(subject), "Topic": topic},
-            data=configs
-        )
+    def list_triggers(self, subject: UUID_LIKE_T) -> globus_sdk.GlobusHTTPResponse:
+        return self.get("/api/v2/triggers", headers={"Subject": str(subject)})
 
-    def set_topic_configs(
-        self, subject: UUID_LIKE_T, topic: str, configs: dict
+    def create_trigger(
+        self, subject: UUID_LIKE_T, topic: str, function: str, action: str,
+        function_configs: dict
     ) -> globus_sdk.GlobusHTTPResponse:
-        return self.post(
-            "/v1/set_topic_configs",
-            headers={"Subject": str(subject), "Topic": topic},
-            data=configs
+        return self.put(
+            "/api/v2/trigger",
+            headers={"Subject": str(subject), "Topic": topic,
+                     "Trigger": function, "Action": action,
+                     "Content-Type": "text/plain"},
+            data=json.dumps(function_configs).encode("utf-8")
         )
 
-    def create_partitions(
-        self, subject: UUID_LIKE_T, topic: str, new_partitions: int
+    def update_trigger(
+        self, subject: UUID_LIKE_T, trigger_uuid: UUID_LIKE_T, trigger_configs: dict
     ) -> globus_sdk.GlobusHTTPResponse:
         return self.post(
-            "/v1/create_partitions",
-            headers={"Subject": str(subject), "Topic": topic,
-                     "NewPartitions": str(new_partitions)},
+            f"/api/v2/triggers/{trigger_uuid}",
+            headers={"Subject": str(subject), "Trigger_id": str(trigger_uuid),
+                     "Content-Type": "text/plain"},
+            data=json.dumps(trigger_configs).encode("utf-8")
         )
```

### Comparing `diaspora-event-sdk-0.1.6/diaspora_event_sdk.egg-info/PKG-INFO` & `diaspora-event-sdk-0.1.7/diaspora_event_sdk.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,18 @@
 Metadata-Version: 2.1
 Name: diaspora-event-sdk
-Version: 0.1.6
+Version: 0.1.7
 Summary: SDK of Diaspora Event Fabric: Resilience-enabling services for science from HPC to edge
 Home-page: https://github.com/globus-labs/diaspora-event-sdk
 License: LICENSE
+Platform: UNKNOWN
 Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: globus-sdk<4,>=3.20.1
 Provides-Extra: kafka-python
-Requires-Dist: kafka-python; extra == "kafka-python"
-Requires-Dist: aws-msk-iam-sasl-signer-python; extra == "kafka-python"
 Provides-Extra: test
-Requires-Dist: pytest; extra == "test"
-Requires-Dist: pytest-cov; extra == "test"
-Requires-Dist: coverage; extra == "test"
-Requires-Dist: mypy; extra == "test"
-Requires-Dist: tox; extra == "test"
-Requires-Dist: check-manifest; extra == "test"
+License-File: LICENSE
 
 # Diaspora: Resilience-enabling services for science from HPC to edge
 
 ## Event Fabric SDK Installation Guide
 ### Recommended Method: Use with `kafka-python`
 For easy integration with Diaspora Event Fabric, use the `KafkaProducer` and `KafkaConsumer` classes from our SDK. This requires the `kafka-python` library.
 
@@ -43,7 +35,8 @@
 **Getting Started**: Visit our [QuickStart Guide](docs/quickstart.md) for details on using the SDK with the kafka-python library and instructions for other Kafka clients.
 
 **Troubleshooting and Credential Management**: Consult our [TrobleShooting Guide](docs/troubleshooting.md) for solving common issues and tips on managing keys effectively.
 
 **Advanced Consumers with Faust**: Explore the [Faust Streaming Guide](docs/faust_weather_app.md) for advanced event streaming with Faust.
 
 **Advanced Consumer Functions**: See our [Colab example](https://colab.research.google.com/drive/1tPKfxU2qPsLvNTreF6nKINU62k7pQWxa?usp=sharing) for demonstration.
+
```

### Comparing `diaspora-event-sdk-0.1.6/diaspora_event_sdk.egg-info/SOURCES.txt` & `diaspora-event-sdk-0.1.7/diaspora_event_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `diaspora-event-sdk-0.1.6/setup.py` & `diaspora-event-sdk-0.1.7/setup.py`

 * *Files identical despite different names*

### Comparing `diaspora-event-sdk-0.1.6/tests/unit/test_client.py` & `diaspora-event-sdk-0.1.7/tests/unit/test_client.py`

 * *Files identical despite different names*

