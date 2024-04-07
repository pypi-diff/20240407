# Comparing `tmp/afreeca-0.3.1.tar.gz` & `tmp/afreeca-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "afreeca-0.3.1.tar", last modified: Wed Mar  6 18:54:03 2024, max compression
+gzip compressed data, was "afreeca-0.4.0.tar", last modified: Sun Apr  7 17:10:13 2024, max compression
```

## Comparing `afreeca-0.3.1.tar` & `afreeca-0.4.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-03-06 18:54:03.460485 afreeca-0.3.1/
--rw-rw-rw-   0        0        0     1086 2024-01-29 15:14:51.000000 afreeca-0.3.1/LICENSE
--rw-rw-rw-   0        0        0     1009 2024-03-06 18:54:03.459485 afreeca-0.3.1/PKG-INFO
--rw-rw-rw-   0        0        0      570 2024-01-27 07:19:42.000000 afreeca-0.3.1/README.md
-drwxrwxrwx   0        0        0        0 2024-03-06 18:54:03.435913 afreeca-0.3.1/afreeca/
--rw-rw-rw-   0        0        0      397 2024-03-06 18:53:44.000000 afreeca-0.3.1/afreeca/__init__.py
--rw-rw-rw-   0        0        0     7610 2024-02-11 07:58:25.000000 afreeca-0.3.1/afreeca/constants.py
--rw-rw-rw-   0        0        0     7598 2024-03-06 18:48:01.000000 afreeca-0.3.1/afreeca/core.py
--rw-rw-rw-   0        0        0     1710 2024-03-05 16:22:32.000000 afreeca-0.3.1/afreeca/credential.py
--rw-rw-rw-   0        0        0      454 2024-03-05 16:21:21.000000 afreeca-0.3.1/afreeca/exceptions.py
--rw-rw-rw-   0        0        0     2310 2024-03-06 18:46:56.000000 afreeca-0.3.1/afreeca/interfaces.py
--rw-rw-rw-   0        0        0      581 2024-02-01 15:35:35.000000 afreeca-0.3.1/afreeca/packet.py
-drwxrwxrwx   0        0        0        0 2024-03-06 18:54:03.456452 afreeca-0.3.1/afreeca/types/
--rw-rw-rw-   0        0        0      284 2024-02-11 17:45:35.000000 afreeca-0.3.1/afreeca/types/bj_info.py
--rw-rw-rw-   0        0        0      522 2024-02-01 15:35:35.000000 afreeca-0.3.1/afreeca/types/packet.py
--rw-rw-rw-   0        0        0     1528 2024-02-11 17:15:11.000000 afreeca-0.3.1/afreeca/utils.py
-drwxrwxrwx   0        0        0        0 2024-03-06 18:54:03.458479 afreeca-0.3.1/afreeca.egg-info/
--rw-rw-rw-   0        0        0     1009 2024-03-06 18:54:03.000000 afreeca-0.3.1/afreeca.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      393 2024-03-06 18:54:03.000000 afreeca-0.3.1/afreeca.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-06 18:54:03.000000 afreeca-0.3.1/afreeca.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2024-03-06 18:54:03.000000 afreeca-0.3.1/afreeca.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-03-06 18:54:03.000000 afreeca-0.3.1/afreeca.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      664 2024-02-01 15:35:35.000000 afreeca-0.3.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-06 18:54:03.460485 afreeca-0.3.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-07 17:10:13.100756 afreeca-0.4.0/
+-rw-rw-rw-   0        0        0     1086 2024-01-29 15:14:51.000000 afreeca-0.4.0/LICENSE
+-rw-rw-rw-   0        0        0     1009 2024-04-07 17:10:13.098757 afreeca-0.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0      570 2024-01-27 07:19:42.000000 afreeca-0.4.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-07 17:10:13.061673 afreeca-0.4.0/afreeca/
+-rw-rw-rw-   0        0        0      397 2024-04-07 17:09:01.000000 afreeca-0.4.0/afreeca/__init__.py
+-rw-rw-rw-   0        0        0     7610 2024-02-11 07:58:25.000000 afreeca-0.4.0/afreeca/constants.py
+-rw-rw-rw-   0        0        0     7640 2024-04-07 17:09:21.000000 afreeca-0.4.0/afreeca/core.py
+-rw-rw-rw-   0        0        0     1710 2024-03-05 16:22:32.000000 afreeca-0.4.0/afreeca/credential.py
+-rw-rw-rw-   0        0        0      454 2024-03-05 16:21:21.000000 afreeca-0.4.0/afreeca/exceptions.py
+-rw-rw-rw-   0        0        0     2310 2024-03-06 18:46:56.000000 afreeca-0.4.0/afreeca/interfaces.py
+-rw-rw-rw-   0        0        0      581 2024-02-01 15:35:35.000000 afreeca-0.4.0/afreeca/packet.py
+drwxrwxrwx   0        0        0        0 2024-04-07 17:10:13.095758 afreeca-0.4.0/afreeca/types/
+-rw-rw-rw-   0        0        0      284 2024-02-11 17:45:35.000000 afreeca-0.4.0/afreeca/types/bj_info.py
+-rw-rw-rw-   0        0        0      522 2024-02-01 15:35:35.000000 afreeca-0.4.0/afreeca/types/packet.py
+-rw-rw-rw-   0        0        0     1528 2024-02-11 17:15:11.000000 afreeca-0.4.0/afreeca/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-07 17:10:13.097757 afreeca-0.4.0/afreeca.egg-info/
+-rw-rw-rw-   0        0        0     1009 2024-04-07 17:10:13.000000 afreeca-0.4.0/afreeca.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      393 2024-04-07 17:10:13.000000 afreeca-0.4.0/afreeca.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-07 17:10:13.000000 afreeca-0.4.0/afreeca.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2024-04-07 17:10:13.000000 afreeca-0.4.0/afreeca.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-07 17:10:13.000000 afreeca-0.4.0/afreeca.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      664 2024-02-01 15:35:35.000000 afreeca-0.4.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-07 17:10:13.100756 afreeca-0.4.0/setup.cfg
```

### Comparing `afreeca-0.3.1/LICENSE` & `afreeca-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `afreeca-0.3.1/PKG-INFO` & `afreeca-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: afreeca
-Version: 0.3.1
+Version: 0.4.0
 Summary: AfreecaTV API Wrapper
 Author-email: minibox <minibox724@gmail.com>
 License: MIT
 Project-URL: homepage, https://github.com/wakscord/afreeca
 Project-URL: repository, https://github.com/wakscord/afreeca
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `afreeca-0.3.1/README.md` & `afreeca-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `afreeca-0.3.1/afreeca/constants.py` & `afreeca-0.4.0/afreeca/constants.py`

 * *Files identical despite different names*

### Comparing `afreeca-0.3.1/afreeca/core.py` & `afreeca-0.4.0/afreeca/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -137,27 +137,27 @@
             except asyncio.TimeoutError:
                 continue
 
     async def start(self) -> None:
         await self.connect()
         await self.loop()
 
-    async def connect(self) -> None:
+    async def connect(self, sub: bool = False) -> None:
         if not self.info:
             self.info = await AfreecaTV.fetch_bj_info(self.credential, self.bj_id)
 
         self.session = ClientSession()
         self.connection = await self.session.ws_connect(self.info.chat_url)
 
         await self.send(
             ServiceCode.SVC_LOGIN,
             [
                 self.info.tk if self.info.tk else "",
                 "",
-                Flag().add(FLAG["GUEST"]).flag1,
+                Flag().add(FLAG["FOLLOWER" if sub else "GUEST"]).flag1,
             ],
         )
 
         if not self.keepalive_task:
             self.keepalive_task = asyncio.create_task(self._keepalive())
 
     async def send(self, svc: int, data: list[str]) -> None:
```

### Comparing `afreeca-0.3.1/afreeca/credential.py` & `afreeca-0.4.0/afreeca/credential.py`

 * *Files identical despite different names*

### Comparing `afreeca-0.3.1/afreeca/interfaces.py` & `afreeca-0.4.0/afreeca/interfaces.py`

 * *Files identical despite different names*

### Comparing `afreeca-0.3.1/afreeca/packet.py` & `afreeca-0.4.0/afreeca/packet.py`

 * *Files identical despite different names*

### Comparing `afreeca-0.3.1/afreeca/types/packet.py` & `afreeca-0.4.0/afreeca/types/packet.py`

 * *Files identical despite different names*

### Comparing `afreeca-0.3.1/afreeca/utils.py` & `afreeca-0.4.0/afreeca/utils.py`

 * *Files identical despite different names*

### Comparing `afreeca-0.3.1/afreeca.egg-info/PKG-INFO` & `afreeca-0.4.0/afreeca.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: afreeca
-Version: 0.3.1
+Version: 0.4.0
 Summary: AfreecaTV API Wrapper
 Author-email: minibox <minibox724@gmail.com>
 License: MIT
 Project-URL: homepage, https://github.com/wakscord/afreeca
 Project-URL: repository, https://github.com/wakscord/afreeca
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `afreeca-0.3.1/pyproject.toml` & `afreeca-0.4.0/pyproject.toml`

 * *Files identical despite different names*

