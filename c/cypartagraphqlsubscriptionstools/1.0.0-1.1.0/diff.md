# Comparing `tmp/cypartagraphqlsubscriptionstools-1.0.0.tar.gz` & `tmp/cypartagraphqlsubscriptionstools-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cypartagraphqlsubscriptionstools-1.0.0.tar", last modified: Wed Feb 14 23:42:27 2024, max compression
+gzip compressed data, was "cypartagraphqlsubscriptionstools-1.1.0.tar", last modified: Sat Apr  6 22:34:04 2024, max compression
```

## Comparing `cypartagraphqlsubscriptionstools-1.0.0.tar` & `cypartagraphqlsubscriptionstools-1.1.0.tar`

### file list

```diff
@@ -1,29 +1,43 @@
-drwxr-xr-x   0 eslam     (1000) eslam     (1003)        0 2024-02-14 23:42:27.920207 cypartagraphqlsubscriptionstools-1.0.0/
-drwxr-xr-x   0 eslam     (1000) eslam     (1003)        0 2024-02-14 23:42:27.916874 cypartagraphqlsubscriptionstools-1.0.0/CypartaGraphqlSubscriptionsTools/
--rw-r--r--   0 eslam     (1000) eslam     (1003)       89 2024-01-03 00:49:23.000000 cypartagraphqlsubscriptionstools-1.0.0/CypartaGraphqlSubscriptionsTools/__init__.py
--rw-r--r--   0 eslam     (1000) eslam     (1003)       86 2024-01-02 21:02:10.000000 cypartagraphqlsubscriptionstools-1.0.0/CypartaGraphqlSubscriptionsTools/admin.py
--rw-r--r--   0 eslam     (1000) eslam     (1003)      128 2024-01-03 00:49:23.000000 cypartagraphqlsubscriptionstools-1.0.0/CypartaGraphqlSubscriptionsTools/apps.py
--rw-r--r--   0 eslam     (1000) eslam     (1003)     7310 2024-02-11 17:16:48.000000 cypartagraphqlsubscriptionstools-1.0.0/CypartaGraphqlSubscriptionsTools/consumers.py
--rw-r--r--   0 eslam     (1000) eslam     (1003)      788 2024-02-11 17:02:04.000000 cypartagraphqlsubscriptionstools-1.0.0/CypartaGraphqlSubscriptionsTools/events.py
-drwxr-xr-x   0 eslam     (1000) eslam     (1003)        0 2024-02-14 23:42:27.920207 cypartagraphqlsubscriptionstools-1.0.0/CypartaGraphqlSubscriptionsTools/migrations/
--rw-r--r--   0 eslam     (1000) eslam     (1003)      711 2024-01-27 22:54:49.000000 cypartagraphqlsubscriptionstools-1.0.0/CypartaGraphqlSubscriptionsTools/migrations/0001_initial.py
--rw-r--r--   0 eslam     (1000) eslam     (1003)        0 2023-12-19 19:58:28.000000 cypartagraphqlsubscriptionstools-1.0.0/CypartaGraphqlSubscriptionsTools/migrations/__init__.py
--rw-r--r--   0 eslam     (1000) eslam     (1003)     1254 2024-01-27 22:54:49.000000 cypartagraphqlsubscriptionstools-1.0.0/CypartaGraphqlSubscriptionsTools/mixins.py
--rw-r--r--   0 eslam     (1000) eslam     (1003)      342 2024-01-27 22:54:49.000000 cypartagraphqlsubscriptionstools-1.0.0/CypartaGraphqlSubscriptionsTools/models.py
--rw-r--r--   0 eslam     (1000) eslam     (1003)      359 2024-01-27 20:50:25.000000 cypartagraphqlsubscriptionstools-1.0.0/CypartaGraphqlSubscriptionsTools/routing.py
--rw-r--r--   0 eslam     (1000) eslam     (1003)     3601 2024-01-29 21:53:40.000000 cypartagraphqlsubscriptionstools-1.0.0/CypartaGraphqlSubscriptionsTools/schema.py
--rw-r--r--   0 eslam     (1000) eslam     (1003)      925 2024-02-11 17:10:05.000000 cypartagraphqlsubscriptionstools-1.0.0/CypartaGraphqlSubscriptionsTools/serialize.py
--rw-r--r--   0 eslam     (1000) eslam     (1003)      320 2023-12-19 19:56:53.000000 cypartagraphqlsubscriptionstools-1.0.0/CypartaGraphqlSubscriptionsTools/urls.py
--rw-r--r--   0 eslam     (1000) eslam     (1003)      384 2024-02-11 17:11:58.000000 cypartagraphqlsubscriptionstools-1.0.0/CypartaGraphqlSubscriptionsTools/utils.py
--rw-r--r--   0 eslam     (1000) eslam     (1003)      709 2024-01-03 00:49:23.000000 cypartagraphqlsubscriptionstools-1.0.0/CypartaGraphqlSubscriptionsTools/views.py
--rw-r--r--   0 eslam     (1000) eslam     (1003)     1079 2024-02-12 22:02:14.000000 cypartagraphqlsubscriptionstools-1.0.0/LICENSE
--rw-r--r--   0 eslam     (1000) eslam     (1003)    14115 2024-02-14 23:42:27.920207 cypartagraphqlsubscriptionstools-1.0.0/PKG-INFO
--rw-r--r--   0 eslam     (1000) eslam     (1003)    13243 2024-01-28 23:37:02.000000 cypartagraphqlsubscriptionstools-1.0.0/README.md
-drwxr-xr-x   0 eslam     (1000) eslam     (1003)        0 2024-02-14 23:42:27.920207 cypartagraphqlsubscriptionstools-1.0.0/cypartagraphqlsubscriptionstools.egg-info/
--rw-r--r--   0 eslam     (1000) eslam     (1003)    14115 2024-02-14 23:42:27.000000 cypartagraphqlsubscriptionstools-1.0.0/cypartagraphqlsubscriptionstools.egg-info/PKG-INFO
--rw-r--r--   0 eslam     (1000) eslam     (1003)      982 2024-02-14 23:42:27.000000 cypartagraphqlsubscriptionstools-1.0.0/cypartagraphqlsubscriptionstools.egg-info/SOURCES.txt
--rw-r--r--   0 eslam     (1000) eslam     (1003)        1 2024-02-14 23:42:27.000000 cypartagraphqlsubscriptionstools-1.0.0/cypartagraphqlsubscriptionstools.egg-info/dependency_links.txt
--rw-r--r--   0 eslam     (1000) eslam     (1003)       55 2024-02-14 23:42:27.000000 cypartagraphqlsubscriptionstools-1.0.0/cypartagraphqlsubscriptionstools.egg-info/requires.txt
--rw-r--r--   0 eslam     (1000) eslam     (1003)       33 2024-02-14 23:42:27.000000 cypartagraphqlsubscriptionstools-1.0.0/cypartagraphqlsubscriptionstools.egg-info/top_level.txt
--rw-r--r--   0 eslam     (1000) eslam     (1003)       38 2024-02-14 23:42:27.920207 cypartagraphqlsubscriptionstools-1.0.0/setup.cfg
--rw-r--r--   0 eslam     (1000) eslam     (1003)     1198 2024-02-14 23:38:04.000000 cypartagraphqlsubscriptionstools-1.0.0/setup.py
+drwxr-xr-x   0 eslam     (1000) eslam     (1003)        0 2024-04-06 22:34:04.396942 cypartagraphqlsubscriptionstools-1.1.0/
+drwxr-xr-x   0 eslam     (1000) eslam     (1003)        0 2024-04-06 22:34:04.390275 cypartagraphqlsubscriptionstools-1.1.0/.vscode/
+-rw-r--r--   0 eslam     (1000) eslam     (1003)      791 2024-03-12 16:56:38.000000 cypartagraphqlsubscriptionstools-1.1.0/.vscode/launch.json
+-rw-r--r--   0 eslam     (1000) eslam     (1003)       69 2024-03-12 16:56:38.000000 cypartagraphqlsubscriptionstools-1.1.0/.vscode/settings.json
+drwxr-xr-x   0 eslam     (1000) eslam     (1003)        0 2024-04-06 22:34:04.393608 cypartagraphqlsubscriptionstools-1.1.0/CypartaGraphqlSubscriptionsTools/
+drwxr-xr-x   0 eslam     (1000) eslam     (1003)        0 2024-04-06 22:34:04.386942 cypartagraphqlsubscriptionstools-1.1.0/CypartaGraphqlSubscriptionsTools/.github/
+drwxr-xr-x   0 eslam     (1000) eslam     (1003)        0 2024-04-06 22:34:04.393608 cypartagraphqlsubscriptionstools-1.1.0/CypartaGraphqlSubscriptionsTools/.github/workflows/
+-rw-r--r--   0 eslam     (1000) eslam     (1003)      409 2024-03-12 16:56:38.000000 cypartagraphqlsubscriptionstools-1.1.0/CypartaGraphqlSubscriptionsTools/.github/workflows/test.yml
+-rw-r--r--   0 eslam     (1000) eslam     (1003)     1121 2024-03-12 16:56:38.000000 cypartagraphqlsubscriptionstools-1.1.0/CypartaGraphqlSubscriptionsTools/.gitignore
+-rw-r--r--   0 eslam     (1000) eslam     (1003)       89 2024-03-12 16:56:38.000000 cypartagraphqlsubscriptionstools-1.1.0/CypartaGraphqlSubscriptionsTools/__init__.py
+-rw-r--r--   0 eslam     (1000) eslam     (1003)       86 2024-03-12 16:56:38.000000 cypartagraphqlsubscriptionstools-1.1.0/CypartaGraphqlSubscriptionsTools/admin.py
+-rw-r--r--   0 eslam     (1000) eslam     (1003)      128 2024-03-12 16:56:38.000000 cypartagraphqlsubscriptionstools-1.1.0/CypartaGraphqlSubscriptionsTools/apps.py
+-rw-r--r--   0 eslam     (1000) eslam     (1003)     7310 2024-03-12 16:56:38.000000 cypartagraphqlsubscriptionstools-1.1.0/CypartaGraphqlSubscriptionsTools/consumers.py
+-rw-r--r--   0 eslam     (1000) eslam     (1003)      800 2024-03-14 22:41:03.000000 cypartagraphqlsubscriptionstools-1.1.0/CypartaGraphqlSubscriptionsTools/events.py
+-rw-r--r--   0 eslam     (1000) eslam     (1003)     1046 2024-04-06 21:47:52.000000 cypartagraphqlsubscriptionstools-1.1.0/CypartaGraphqlSubscriptionsTools/middleware.py
+drwxr-xr-x   0 eslam     (1000) eslam     (1003)        0 2024-04-06 22:34:04.393608 cypartagraphqlsubscriptionstools-1.1.0/CypartaGraphqlSubscriptionsTools/migrations/
+-rw-r--r--   0 eslam     (1000) eslam     (1003)      711 2024-03-12 16:56:38.000000 cypartagraphqlsubscriptionstools-1.1.0/CypartaGraphqlSubscriptionsTools/migrations/0001_initial.py
+-rw-r--r--   0 eslam     (1000) eslam     (1003)        0 2024-03-12 16:56:38.000000 cypartagraphqlsubscriptionstools-1.1.0/CypartaGraphqlSubscriptionsTools/migrations/__init__.py
+-rw-r--r--   0 eslam     (1000) eslam     (1003)     1254 2024-03-12 16:56:38.000000 cypartagraphqlsubscriptionstools-1.1.0/CypartaGraphqlSubscriptionsTools/mixins.py
+-rw-r--r--   0 eslam     (1000) eslam     (1003)      342 2024-03-12 16:56:38.000000 cypartagraphqlsubscriptionstools-1.1.0/CypartaGraphqlSubscriptionsTools/models.py
+-rw-r--r--   0 eslam     (1000) eslam     (1003)      359 2024-03-12 16:56:38.000000 cypartagraphqlsubscriptionstools-1.1.0/CypartaGraphqlSubscriptionsTools/routing.py
+-rw-r--r--   0 eslam     (1000) eslam     (1003)     3601 2024-03-12 16:56:38.000000 cypartagraphqlsubscriptionstools-1.1.0/CypartaGraphqlSubscriptionsTools/schema.py
+-rw-r--r--   0 eslam     (1000) eslam     (1003)      925 2024-03-12 16:56:38.000000 cypartagraphqlsubscriptionstools-1.1.0/CypartaGraphqlSubscriptionsTools/serialize.py
+-rw-r--r--   0 eslam     (1000) eslam     (1003)      320 2024-03-12 16:56:38.000000 cypartagraphqlsubscriptionstools-1.1.0/CypartaGraphqlSubscriptionsTools/urls.py
+-rw-r--r--   0 eslam     (1000) eslam     (1003)      648 2024-03-14 22:24:44.000000 cypartagraphqlsubscriptionstools-1.1.0/CypartaGraphqlSubscriptionsTools/utils.py
+-rw-r--r--   0 eslam     (1000) eslam     (1003)      709 2024-03-12 16:56:38.000000 cypartagraphqlsubscriptionstools-1.1.0/CypartaGraphqlSubscriptionsTools/views.py
+-rw-r--r--   0 eslam     (1000) eslam     (1003)     1079 2024-03-12 16:56:38.000000 cypartagraphqlsubscriptionstools-1.1.0/LICENSE
+-rw-r--r--   0 eslam     (1000) eslam     (1003)    14736 2024-04-06 22:34:04.393608 cypartagraphqlsubscriptionstools-1.1.0/PKG-INFO
+-rw-r--r--   0 eslam     (1000) eslam     (1003)    13819 2024-04-06 21:57:21.000000 cypartagraphqlsubscriptionstools-1.1.0/README.md
+-rw-r--r--   0 eslam     (1000) eslam     (1003)    30445 2024-03-12 16:56:38.000000 cypartagraphqlsubscriptionstools-1.1.0/cover.jpg
+drwxr-xr-x   0 eslam     (1000) eslam     (1003)        0 2024-04-06 22:34:04.393608 cypartagraphqlsubscriptionstools-1.1.0/cypartagraphqlsubscriptionstools.egg-info/
+-rw-r--r--   0 eslam     (1000) eslam     (1003)    14736 2024-04-06 22:34:04.000000 cypartagraphqlsubscriptionstools-1.1.0/cypartagraphqlsubscriptionstools.egg-info/PKG-INFO
+-rw-r--r--   0 eslam     (1000) eslam     (1003)     1273 2024-04-06 22:34:04.000000 cypartagraphqlsubscriptionstools-1.1.0/cypartagraphqlsubscriptionstools.egg-info/SOURCES.txt
+-rw-r--r--   0 eslam     (1000) eslam     (1003)        1 2024-04-06 22:34:04.000000 cypartagraphqlsubscriptionstools-1.1.0/cypartagraphqlsubscriptionstools.egg-info/dependency_links.txt
+-rw-r--r--   0 eslam     (1000) eslam     (1003)       55 2024-04-06 22:34:04.000000 cypartagraphqlsubscriptionstools-1.1.0/cypartagraphqlsubscriptionstools.egg-info/requires.txt
+-rw-r--r--   0 eslam     (1000) eslam     (1003)       33 2024-04-06 22:34:04.000000 cypartagraphqlsubscriptionstools-1.1.0/cypartagraphqlsubscriptionstools.egg-info/top_level.txt
+drwxr-xr-x   0 eslam     (1000) eslam     (1003)        0 2024-04-06 22:34:04.393608 cypartagraphqlsubscriptionstools-1.1.0/dist/
+-rw-r--r--   0 eslam     (1000) eslam     (1003)   522166 2024-04-06 22:21:03.000000 cypartagraphqlsubscriptionstools-1.1.0/dist/cypartagraphqlsubscriptionstools-1.0.0.tar.gz
+-rw-r--r--   0 eslam     (1000) eslam     (1003)   499268 2024-03-12 16:56:38.000000 cypartagraphqlsubscriptionstools-1.1.0/graph.jpg
+-rwxr-xr-x   0 eslam     (1000) eslam     (1003)      663 2024-03-12 16:56:38.000000 cypartagraphqlsubscriptionstools-1.1.0/manage.py
+-rw-r--r--   0 eslam     (1000) eslam     (1003)       77 2024-03-12 16:56:38.000000 cypartagraphqlsubscriptionstools-1.1.0/requirements.txt
+-rw-r--r--   0 eslam     (1000) eslam     (1003)       38 2024-04-06 22:34:04.396942 cypartagraphqlsubscriptionstools-1.1.0/setup.cfg
+-rw-r--r--   0 eslam     (1000) eslam     (1003)     1243 2024-04-06 22:33:46.000000 cypartagraphqlsubscriptionstools-1.1.0/setup.py
```

### Comparing `cypartagraphqlsubscriptionstools-1.0.0/CypartaGraphqlSubscriptionsTools/consumers.py` & `cypartagraphqlsubscriptionstools-1.1.0/CypartaGraphqlSubscriptionsTools/consumers.py`

 * *Files identical despite different names*

### Comparing `cypartagraphqlsubscriptionstools-1.0.0/CypartaGraphqlSubscriptionsTools/events.py` & `cypartagraphqlsubscriptionstools-1.1.0/CypartaGraphqlSubscriptionsTools/events.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from channels.layers import get_channel_layer
 from django.core import serializers
 from .serialize import serialize_value
 async def trigger_subscription(group, value):
     # Print some information for debugging purposes
-    print('Value:', value)
-    print('ID:', value.id)
-    print('Group:', group)
+    # print('Value:', value)
+    # print('ID:', value.id)
+    # print('Group:', group)
     
     # Get the channel layer
     channel_layer = get_channel_layer()
 
     # Send a message to the specified channel group
     await channel_layer.group_send(
         group,
         {
             "type": "subscription.triggered",  # Type of the message
-            "value": await serialize_value(value),  # The value to be sent
+            "value": await serialize_value(value,group),  # The value to be sent
             "group": group  # The channel group to send the message to
         }
     )
 
     # Print a message indicating that the message has been sent
```

### Comparing `cypartagraphqlsubscriptionstools-1.0.0/CypartaGraphqlSubscriptionsTools/migrations/0001_initial.py` & `cypartagraphqlsubscriptionstools-1.1.0/CypartaGraphqlSubscriptionsTools/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `cypartagraphqlsubscriptionstools-1.0.0/CypartaGraphqlSubscriptionsTools/mixins.py` & `cypartagraphqlsubscriptionstools-1.1.0/CypartaGraphqlSubscriptionsTools/mixins.py`

 * *Files identical despite different names*

### Comparing `cypartagraphqlsubscriptionstools-1.0.0/CypartaGraphqlSubscriptionsTools/schema.py` & `cypartagraphqlsubscriptionstools-1.1.0/CypartaGraphqlSubscriptionsTools/schema.py`

 * *Files identical despite different names*

### Comparing `cypartagraphqlsubscriptionstools-1.0.0/CypartaGraphqlSubscriptionsTools/serialize.py` & `cypartagraphqlsubscriptionstools-1.1.0/CypartaGraphqlSubscriptionsTools/serialize.py`

 * *Files identical despite different names*

### Comparing `cypartagraphqlsubscriptionstools-1.0.0/CypartaGraphqlSubscriptionsTools/views.py` & `cypartagraphqlsubscriptionstools-1.1.0/CypartaGraphqlSubscriptionsTools/views.py`

 * *Files identical despite different names*

### Comparing `cypartagraphqlsubscriptionstools-1.0.0/LICENSE` & `cypartagraphqlsubscriptionstools-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cypartagraphqlsubscriptionstools-1.0.0/PKG-INFO` & `cypartagraphqlsubscriptionstools-1.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: cypartagraphqlsubscriptionstools
-Version: 1.0.0
+Version: 1.1.0
 Summary: A CypartaGraphqlSubscriptionsTools implementation for Graphene + Django built using Django Channels +reactive programming in python (RxPY) . Provides support for model creation, mutation and deletion,and get data with websocket or path list of events name for subscriptions .
 Home-page: https://cyparta.com/
 Author: Cyparta Software House
 Author-email: Support@cyparta.com
 License: LICENSE
+Project-URL: homepage, https://cyparta.com/
 Project-URL: Documentation, https://github.com/Cyparta/CypartaGraphqlSubscriptionsTools
 Project-URL: Source, https://github.com/Cyparta/CypartaGraphqlSubscriptionsTools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
@@ -128,14 +129,15 @@
    ```
 
 5. Define your subscriptions and connect them to your project schema
 
    ```python
    #your_project/schema.py
    import graphene
+   from asgiref.sync import async_to_sync
 
    from your_app.graphql.subscriptions import YourSubscription
 
 
    class Query(graphene.ObjectType):
        base = graphene.String()
 
@@ -344,7 +346,24 @@
 
 
 # elsewhere in your app:
 from CypartaGraphqlSubscriptionsTools.events import trigger_subscription
 
 async_to_sync(trigger_subscription)(f"{model_name}Created", self)
 ```
+
+Custom middleware, such as `TokenAuthMiddleware`, can be added to provide additional functionality, such as authentication or permission checks, to WebSocket connections.
+
+
+```python
+from CypartaGraphqlSubscriptionsTools.middleware import TokenAuthMiddleware
+application = ProtocolTypeRouter({
+  "http": django_asgi_app,
+  "websocket": 
+        AuthMiddlewareStack(
+            TokenAuthMiddleware(
+            URLRouter(
+                CypartaGraphqlSubscriptionsTools.routing.websocket_urlpatterns
+            )
+        ))
+    
+})
```

### Comparing `cypartagraphqlsubscriptionstools-1.0.0/README.md` & `cypartagraphqlsubscriptionstools-1.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -111,14 +111,15 @@
    ```
 
 5. Define your subscriptions and connect them to your project schema
 
    ```python
    #your_project/schema.py
    import graphene
+   from asgiref.sync import async_to_sync
 
    from your_app.graphql.subscriptions import YourSubscription
 
 
    class Query(graphene.ObjectType):
        base = graphene.String()
 
@@ -327,7 +328,24 @@
 
 
 # elsewhere in your app:
 from CypartaGraphqlSubscriptionsTools.events import trigger_subscription
 
 async_to_sync(trigger_subscription)(f"{model_name}Created", self)
 ```
+
+Custom middleware, such as `TokenAuthMiddleware`, can be added to provide additional functionality, such as authentication or permission checks, to WebSocket connections.
+
+
+```python
+from CypartaGraphqlSubscriptionsTools.middleware import TokenAuthMiddleware
+application = ProtocolTypeRouter({
+  "http": django_asgi_app,
+  "websocket": 
+        AuthMiddlewareStack(
+            TokenAuthMiddleware(
+            URLRouter(
+                CypartaGraphqlSubscriptionsTools.routing.websocket_urlpatterns
+            )
+        ))
+    
+})
```

### Comparing `cypartagraphqlsubscriptionstools-1.0.0/cypartagraphqlsubscriptionstools.egg-info/PKG-INFO` & `cypartagraphqlsubscriptionstools-1.1.0/cypartagraphqlsubscriptionstools.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: cypartagraphqlsubscriptionstools
-Version: 1.0.0
+Version: 1.1.0
 Summary: A CypartaGraphqlSubscriptionsTools implementation for Graphene + Django built using Django Channels +reactive programming in python (RxPY) . Provides support for model creation, mutation and deletion,and get data with websocket or path list of events name for subscriptions .
 Home-page: https://cyparta.com/
 Author: Cyparta Software House
 Author-email: Support@cyparta.com
 License: LICENSE
+Project-URL: homepage, https://cyparta.com/
 Project-URL: Documentation, https://github.com/Cyparta/CypartaGraphqlSubscriptionsTools
 Project-URL: Source, https://github.com/Cyparta/CypartaGraphqlSubscriptionsTools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
@@ -128,14 +129,15 @@
    ```
 
 5. Define your subscriptions and connect them to your project schema
 
    ```python
    #your_project/schema.py
    import graphene
+   from asgiref.sync import async_to_sync
 
    from your_app.graphql.subscriptions import YourSubscription
 
 
    class Query(graphene.ObjectType):
        base = graphene.String()
 
@@ -344,7 +346,24 @@
 
 
 # elsewhere in your app:
 from CypartaGraphqlSubscriptionsTools.events import trigger_subscription
 
 async_to_sync(trigger_subscription)(f"{model_name}Created", self)
 ```
+
+Custom middleware, such as `TokenAuthMiddleware`, can be added to provide additional functionality, such as authentication or permission checks, to WebSocket connections.
+
+
+```python
+from CypartaGraphqlSubscriptionsTools.middleware import TokenAuthMiddleware
+application = ProtocolTypeRouter({
+  "http": django_asgi_app,
+  "websocket": 
+        AuthMiddlewareStack(
+            TokenAuthMiddleware(
+            URLRouter(
+                CypartaGraphqlSubscriptionsTools.routing.websocket_urlpatterns
+            )
+        ))
+    
+})
```

### Comparing `cypartagraphqlsubscriptionstools-1.0.0/cypartagraphqlsubscriptionstools.egg-info/SOURCES.txt` & `cypartagraphqlsubscriptionstools-1.1.0/cypartagraphqlsubscriptionstools.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,33 @@
 LICENSE
 README.md
+cover.jpg
+graph.jpg
+manage.py
+requirements.txt
 setup.py
+.vscode/launch.json
+.vscode/settings.json
+CypartaGraphqlSubscriptionsTools/.gitignore
 CypartaGraphqlSubscriptionsTools/__init__.py
 CypartaGraphqlSubscriptionsTools/admin.py
 CypartaGraphqlSubscriptionsTools/apps.py
 CypartaGraphqlSubscriptionsTools/consumers.py
 CypartaGraphqlSubscriptionsTools/events.py
+CypartaGraphqlSubscriptionsTools/middleware.py
 CypartaGraphqlSubscriptionsTools/mixins.py
 CypartaGraphqlSubscriptionsTools/models.py
 CypartaGraphqlSubscriptionsTools/routing.py
 CypartaGraphqlSubscriptionsTools/schema.py
 CypartaGraphqlSubscriptionsTools/serialize.py
 CypartaGraphqlSubscriptionsTools/urls.py
 CypartaGraphqlSubscriptionsTools/utils.py
 CypartaGraphqlSubscriptionsTools/views.py
+CypartaGraphqlSubscriptionsTools/.github/workflows/test.yml
 CypartaGraphqlSubscriptionsTools/migrations/0001_initial.py
 CypartaGraphqlSubscriptionsTools/migrations/__init__.py
 cypartagraphqlsubscriptionstools.egg-info/PKG-INFO
 cypartagraphqlsubscriptionstools.egg-info/SOURCES.txt
 cypartagraphqlsubscriptionstools.egg-info/dependency_links.txt
 cypartagraphqlsubscriptionstools.egg-info/requires.txt
-cypartagraphqlsubscriptionstools.egg-info/top_level.txt
+cypartagraphqlsubscriptionstools.egg-info/top_level.txt
+dist/cypartagraphqlsubscriptionstools-1.0.0.tar.gz
```

### Comparing `cypartagraphqlsubscriptionstools-1.0.0/setup.py` & `cypartagraphqlsubscriptionstools-1.1.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 import pathlib
 
 import setuptools
 
 setuptools.setup(
     name="cypartagraphqlsubscriptionstools",
-    version="1.0.0",
+    version="1.1.0",
     description = "A CypartaGraphqlSubscriptionsTools implementation for Graphene + Django built using Django Channels +reactive programming in python (RxPY) . Provides support for model creation, mutation and deletion,and get data with websocket or path list of events name for subscriptions .",
     long_description=pathlib.Path("README.md").read_text(),
     long_description_content_type="text/markdown",
     url="https://cyparta.com/",
     author="Cyparta Software House",
     author_email="Support@cyparta.com",
     license="LICENSE",
     project_urls={
+        "homepage" : "https://cyparta.com/",
         "Documentation":"https://github.com/Cyparta/CypartaGraphqlSubscriptionsTools",
         "Source":"https://github.com/Cyparta/CypartaGraphqlSubscriptionsTools",
     },
     classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
```

