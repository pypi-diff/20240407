# Comparing `tmp/tjfu-3.0.0.tar.gz` & `tmp/tjfu-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tjfu-3.0.0.tar", last modified: Wed Mar 27 17:01:48 2024, max compression
+gzip compressed data, was "tjfu-3.1.0.tar", last modified: Sun Apr  7 15:39:42 2024, max compression
```

## Comparing `tjfu-3.0.0.tar` & `tjfu-3.1.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 duynguyen  (1000) duynguyen  (1000)        0 2024-03-27 17:01:48.175410 tjfu-3.0.0/
--rw-rw-r--   0 duynguyen  (1000) duynguyen  (1000)     6866 2024-03-27 17:01:48.175410 tjfu-3.0.0/PKG-INFO
--rw-rw-r--   0 duynguyen  (1000) duynguyen  (1000)     6175 2024-03-27 16:18:55.000000 tjfu-3.0.0/README.md
--rw-rw-r--   0 duynguyen  (1000) duynguyen  (1000)       38 2024-03-27 17:01:48.175410 tjfu-3.0.0/setup.cfg
--rw-rw-r--   0 duynguyen  (1000) duynguyen  (1000)     1236 2024-03-27 17:01:36.000000 tjfu-3.0.0/setup.py
-drwxrwxr-x   0 duynguyen  (1000) duynguyen  (1000)        0 2024-03-27 17:01:48.175410 tjfu-3.0.0/tjfu/
--rw-rw-r--   0 duynguyen  (1000) duynguyen  (1000)       66 2024-03-27 14:23:57.000000 tjfu-3.0.0/tjfu/__init__.py
--rw-rw-r--   0 duynguyen  (1000) duynguyen  (1000)     1205 2024-03-27 16:00:16.000000 tjfu-3.0.0/tjfu/route.py
--rw-rw-r--   0 duynguyen  (1000) duynguyen  (1000)      490 2024-03-27 14:31:38.000000 tjfu-3.0.0/tjfu/tj_socket.py
--rw-rw-r--   0 duynguyen  (1000) duynguyen  (1000)     7490 2024-03-27 16:33:06.000000 tjfu-3.0.0/tjfu/tjfu.py
-drwxrwxr-x   0 duynguyen  (1000) duynguyen  (1000)        0 2024-03-27 17:01:48.175410 tjfu-3.0.0/tjfu.egg-info/
--rw-rw-r--   0 duynguyen  (1000) duynguyen  (1000)     6866 2024-03-27 17:01:48.000000 tjfu-3.0.0/tjfu.egg-info/PKG-INFO
--rw-rw-r--   0 duynguyen  (1000) duynguyen  (1000)      219 2024-03-27 17:01:48.000000 tjfu-3.0.0/tjfu.egg-info/SOURCES.txt
--rw-rw-r--   0 duynguyen  (1000) duynguyen  (1000)        1 2024-03-27 17:01:48.000000 tjfu-3.0.0/tjfu.egg-info/dependency_links.txt
--rw-rw-r--   0 duynguyen  (1000) duynguyen  (1000)       65 2024-03-27 17:01:48.000000 tjfu-3.0.0/tjfu.egg-info/requires.txt
--rw-rw-r--   0 duynguyen  (1000) duynguyen  (1000)        5 2024-03-27 17:01:48.000000 tjfu-3.0.0/tjfu.egg-info/top_level.txt
+drwxrwxrwx   0 duynguyen  (1000) duynguyen  (1000)        0 2024-04-07 15:39:42.193922 tjfu-3.1.0/
+-rwxrwxrwx   0 duynguyen  (1000) duynguyen  (1000)     7564 2024-04-07 15:39:42.193295 tjfu-3.1.0/PKG-INFO
+-rwxrwxrwx   0 duynguyen  (1000) duynguyen  (1000)     6873 2024-04-07 15:11:08.000000 tjfu-3.1.0/README.md
+-rwxrwxrwx   0 duynguyen  (1000) duynguyen  (1000)       38 2024-04-07 15:39:42.194201 tjfu-3.1.0/setup.cfg
+-rwxrwxrwx   0 duynguyen  (1000) duynguyen  (1000)     1236 2024-04-07 12:47:25.000000 tjfu-3.1.0/setup.py
+drwxrwxrwx   0 duynguyen  (1000) duynguyen  (1000)        0 2024-04-07 15:39:42.188043 tjfu-3.1.0/tjfu/
+-rwxrwxrwx   0 duynguyen  (1000) duynguyen  (1000)       66 2024-04-07 12:46:51.000000 tjfu-3.1.0/tjfu/__init__.py
+-rwxrwxrwx   0 duynguyen  (1000) duynguyen  (1000)     1205 2024-04-07 13:02:35.000000 tjfu-3.1.0/tjfu/route.py
+-rwxrwxrwx   0 duynguyen  (1000) duynguyen  (1000)      490 2024-04-07 12:46:51.000000 tjfu-3.1.0/tjfu/tj_socket.py
+-rwxrwxrwx   0 duynguyen  (1000) duynguyen  (1000)     8156 2024-04-07 13:21:26.000000 tjfu-3.1.0/tjfu/tjfu.py
+drwxrwxrwx   0 duynguyen  (1000) duynguyen  (1000)        0 2024-04-07 15:39:42.192367 tjfu-3.1.0/tjfu.egg-info/
+-rwxrwxrwx   0 duynguyen  (1000) duynguyen  (1000)     7564 2024-04-07 15:39:42.000000 tjfu-3.1.0/tjfu.egg-info/PKG-INFO
+-rwxrwxrwx   0 duynguyen  (1000) duynguyen  (1000)      219 2024-04-07 15:39:42.000000 tjfu-3.1.0/tjfu.egg-info/SOURCES.txt
+-rwxrwxrwx   0 duynguyen  (1000) duynguyen  (1000)        1 2024-04-07 15:39:42.000000 tjfu-3.1.0/tjfu.egg-info/dependency_links.txt
+-rwxrwxrwx   0 duynguyen  (1000) duynguyen  (1000)       65 2024-04-07 15:39:42.000000 tjfu-3.1.0/tjfu.egg-info/requires.txt
+-rwxrwxrwx   0 duynguyen  (1000) duynguyen  (1000)        5 2024-04-07 15:39:42.000000 tjfu-3.1.0/tjfu.egg-info/top_level.txt
```

### Comparing `tjfu-3.0.0/PKG-INFO` & `tjfu-3.1.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tjfu
-Version: 3.0.0
+Version: 3.1.0
 Summary: Python library helps optimize Flask development to be flexible and object-oriented.
 Home-page: UNKNOWN
 Author: DuyNguyen02
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -15,15 +15,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 
 # TJFU
 Python library helps optimize Flask development to be flexible and object-oriented.
-#### Version: 1.0.0
+#### Version: 3.1.0
 ### Extensions have been integrated
 1. [JWT](https://flask-jwt-extended.readthedocs.io/en/stable/)
 2. [SocketIO](https://flask-socketio.readthedocs.io/en/latest/)
 3. [Limiter](https://flask-limiter.readthedocs.io/en/stable/)
 ### Installation
 ```
 pip install tjfu
@@ -156,14 +156,49 @@
 my_custom_route.register_route(another_my_custom_route)
 
 # You must register routes and sockets before calling the init_app function
 app = TJFU.init_app(index_route)
 
 # OTHER CODE...
 ```
+Register Routes using Dictionary (>=3.1.0):
+```Python
+# OTHER CODE...
+
+app = TJFU.init_app(
+    Route("index", "/"), 
+    {
+        Route("api", "/api"):{
+            
+            Route("v1", "/v1"):{
+                
+                Route("user", "/user"):{
+            
+                }    
+                
+            }
+            
+        },
+        Route("tool", "/tool"):{
+            SimpleRenderTemplateRoute(
+                "my_tool",
+                "/my_tool",
+                "my_tool.html"
+            )
+        },
+        SimpleRenderTemplateRoute(
+            "hello_world",
+            "/hello_world",
+            "hello_world.html"
+        ): None
+    }
+)
+
+# OTHER CODE...
+```
 
 Define a Socket Handle:
 ```Python
 # OTHER CODE...
 
 from tjfu import SocketEvent, SocketHandle
 from flask import request
```

### Comparing `tjfu-3.0.0/README.md` & `tjfu-3.1.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # TJFU
 Python library helps optimize Flask development to be flexible and object-oriented.
-#### Version: 1.0.0
+#### Version: 3.1.0
 ### Extensions have been integrated
 1. [JWT](https://flask-jwt-extended.readthedocs.io/en/stable/)
 2. [SocketIO](https://flask-socketio.readthedocs.io/en/latest/)
 3. [Limiter](https://flask-limiter.readthedocs.io/en/stable/)
 ### Installation
 ```
 pip install tjfu
@@ -137,14 +137,49 @@
 my_custom_route.register_route(another_my_custom_route)
 
 # You must register routes and sockets before calling the init_app function
 app = TJFU.init_app(index_route)
 
 # OTHER CODE...
 ```
+Register Routes using Dictionary (>=3.1.0):
+```Python
+# OTHER CODE...
+
+app = TJFU.init_app(
+    Route("index", "/"), 
+    {
+        Route("api", "/api"):{
+            
+            Route("v1", "/v1"):{
+                
+                Route("user", "/user"):{
+            
+                }    
+                
+            }
+            
+        },
+        Route("tool", "/tool"):{
+            SimpleRenderTemplateRoute(
+                "my_tool",
+                "/my_tool",
+                "my_tool.html"
+            )
+        },
+        SimpleRenderTemplateRoute(
+            "hello_world",
+            "/hello_world",
+            "hello_world.html"
+        ): None
+    }
+)
+
+# OTHER CODE...
+```
 
 Define a Socket Handle:
 ```Python
 # OTHER CODE...
 
 from tjfu import SocketEvent, SocketHandle
 from flask import request
```

### Comparing `tjfu-3.0.0/setup.py` & `tjfu-3.1.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 HERE = path.abspath(path.dirname(__file__))
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='tjfu',
     packages=find_packages(include=['tjfu']),
-    version='3.0.0',
+    version='3.1.0',
     description='Python library helps optimize Flask development to be flexible and object-oriented.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='DuyNguyen02',
     install_requires=[
         "flask",
         "flask_cors",
```

### Comparing `tjfu-3.0.0/tjfu/route.py` & `tjfu-3.1.0/tjfu/route.py`

 * *Files identical despite different names*

### Comparing `tjfu-3.0.0/tjfu/tjfu.py` & `tjfu-3.1.0/tjfu/tjfu.py`

 * *Files 19% similar despite different names*

```diff
@@ -183,18 +183,32 @@
         )
         
         TJFU._SOCKET_IO = SocketIO(
             TJFU._FLASK_APP,
             cors_allowed_origins="*",
             async_mode=TJFU._SOCKET_ASYNC_MODE
         )
-        
+    
+    def _routes_map_register(index_route: Route, routes_map: dict):
+        if isinstance(routes_map, dict):
+            for route, sub_routes_map in routes_map.items():
+                if isinstance(route, Route):
+                    index_route.register_route(route)
+                    TJFU._routes_map_register(route, sub_routes_map)
+        elif isinstance(routes_map, (set, list, tuple)):
+            for route in routes_map:
+                if isinstance(route, Route):
+                    index_route.register_route(route)
         
     @staticmethod
-    def init_app(index_route: Route):
+    def init_app(index_route: Route, routes_map: dict=None):
+        
+        if routes_map is not None:
+            TJFU._routes_map_register(index_route, routes_map)
+        
         TJFU._FLASK_APP.register_blueprint(
             index_route.blueprint,
             url_prefix=index_route.url_prefix
         )
         return TJFU._FLASK_APP
     
     @staticmethod
```

### Comparing `tjfu-3.0.0/tjfu.egg-info/PKG-INFO` & `tjfu-3.1.0/tjfu.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tjfu
-Version: 3.0.0
+Version: 3.1.0
 Summary: Python library helps optimize Flask development to be flexible and object-oriented.
 Home-page: UNKNOWN
 Author: DuyNguyen02
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -15,15 +15,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 
 # TJFU
 Python library helps optimize Flask development to be flexible and object-oriented.
-#### Version: 1.0.0
+#### Version: 3.1.0
 ### Extensions have been integrated
 1. [JWT](https://flask-jwt-extended.readthedocs.io/en/stable/)
 2. [SocketIO](https://flask-socketio.readthedocs.io/en/latest/)
 3. [Limiter](https://flask-limiter.readthedocs.io/en/stable/)
 ### Installation
 ```
 pip install tjfu
@@ -156,14 +156,49 @@
 my_custom_route.register_route(another_my_custom_route)
 
 # You must register routes and sockets before calling the init_app function
 app = TJFU.init_app(index_route)
 
 # OTHER CODE...
 ```
+Register Routes using Dictionary (>=3.1.0):
+```Python
+# OTHER CODE...
+
+app = TJFU.init_app(
+    Route("index", "/"), 
+    {
+        Route("api", "/api"):{
+            
+            Route("v1", "/v1"):{
+                
+                Route("user", "/user"):{
+            
+                }    
+                
+            }
+            
+        },
+        Route("tool", "/tool"):{
+            SimpleRenderTemplateRoute(
+                "my_tool",
+                "/my_tool",
+                "my_tool.html"
+            )
+        },
+        SimpleRenderTemplateRoute(
+            "hello_world",
+            "/hello_world",
+            "hello_world.html"
+        ): None
+    }
+)
+
+# OTHER CODE...
+```
 
 Define a Socket Handle:
 ```Python
 # OTHER CODE...
 
 from tjfu import SocketEvent, SocketHandle
 from flask import request
```

