# Comparing `tmp/ansar-connect-0.1.135.tar.gz` & `tmp/ansar-connect-0.1.136.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansar-connect-0.1.135.tar", last modified: Sun Apr  7 00:48:47 2024, max compression
+gzip compressed data, was "ansar-connect-0.1.136.tar", last modified: Sun Apr  7 04:19:05 2024, max compression
```

## Comparing `ansar-connect-0.1.135.tar` & `ansar-connect-0.1.136.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-07 00:48:47.011826 ansar-connect-0.1.135/
--rw-rw-r--   0 scott     (1000) scott     (1000)     1124 2023-06-30 14:19:32.000000 ansar-connect-0.1.135/LICENSE
--rw-r--r--   0 scott     (1000) scott     (1000)     2674 2024-04-07 00:48:47.011826 ansar-connect-0.1.135/PKG-INFO
--rwxr-xr-x   0 scott     (1000) scott     (1000)     1966 2023-06-28 15:55:38.000000 ansar-connect-0.1.135/README.md
--rwxr-xr-x   0 scott     (1000) scott     (1000)      723 2024-03-28 18:04:29.000000 ansar-connect-0.1.135/pyproject.toml
--rw-rw-r--   0 scott     (1000) scott     (1000)       38 2024-04-07 00:48:47.011826 ansar-connect-0.1.135/setup.cfg
--rwxr-xr-x   0 scott     (1000) scott     (1000)     2210 2024-03-28 18:04:17.000000 ansar-connect-0.1.135/setup.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-07 00:48:47.007826 ansar-connect-0.1.135/src/
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-07 00:48:47.007826 ansar-connect-0.1.135/src/ansar/
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-07 00:48:47.011826 ansar-connect-0.1.135/src/ansar/command/
--rw-rw-r--   0 scott     (1000) scott     (1000)    14427 2024-03-29 02:37:30.000000 ansar-connect-0.1.135/src/ansar/command/ansar_command.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     3072 2024-03-04 07:28:05.000000 ansar-connect-0.1.135/src/ansar/command/ansar_directory.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     9940 2024-03-26 18:46:17.000000 ansar-connect-0.1.135/src/ansar/command/ansar_group.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     8658 2024-03-29 22:32:03.000000 ansar-connect-0.1.135/src/ansar/command/shared_directory.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-07 00:48:47.011826 ansar-connect-0.1.135/src/ansar/connect/
--rwxrwxr-x   0 scott     (1000) scott     (1000)     3012 2024-04-07 00:48:43.000000 ansar-connect-0.1.135/src/ansar/connect/__init__.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    13387 2024-03-23 02:08:11.000000 ansar-connect-0.1.135/src/ansar/connect/connect_directory.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    77328 2024-04-07 00:39:18.000000 ansar-connect-0.1.135/src/ansar/connect/directory.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     7752 2024-04-01 20:33:07.000000 ansar-connect-0.1.135/src/ansar/connect/directory_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     9979 2024-04-02 12:37:04.000000 ansar-connect-0.1.135/src/ansar/connect/foh_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2119 2024-03-23 19:35:11.000000 ansar-connect-0.1.135/src/ansar/connect/group_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    14174 2024-03-01 03:02:47.000000 ansar-connect-0.1.135/src/ansar/connect/grouping.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2221 2024-04-02 20:33:16.000000 ansar-connect-0.1.135/src/ansar/connect/moving.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    21087 2024-04-06 01:12:06.000000 ansar-connect-0.1.135/src/ansar/connect/networking.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     1558 2024-03-01 02:40:39.000000 ansar-connect-0.1.135/src/ansar/connect/networking_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    34999 2024-03-23 01:59:51.000000 ansar-connect-0.1.135/src/ansar/connect/node.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2091 2024-03-05 13:29:47.000000 ansar-connect-0.1.135/src/ansar/connect/plumbing.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    37271 2024-04-04 20:50:42.000000 ansar-connect-0.1.135/src/ansar/connect/procedure.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2323 2024-03-29 22:32:03.000000 ansar-connect-0.1.135/src/ansar/connect/product.py
--rwxrwxr-x   0 scott     (1000) scott     (1000)    36421 2024-03-26 19:24:58.000000 ansar-connect-0.1.135/src/ansar/connect/socketry.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2159 2024-03-25 00:38:01.000000 ansar-connect-0.1.135/src/ansar/connect/standard.py
--rwxr-xr-x   0 scott     (1000) scott     (1000)     2065 2023-09-27 02:08:10.000000 ansar-connect-0.1.135/src/ansar/connect/transporting.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     6187 2024-03-28 02:15:57.000000 ansar-connect-0.1.135/src/ansar/connect/wan.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-07 00:48:47.011826 ansar-connect-0.1.135/src/ansar_connect.egg-info/
--rw-r--r--   0 scott     (1000) scott     (1000)     2674 2024-04-07 00:48:47.000000 ansar-connect-0.1.135/src/ansar_connect.egg-info/PKG-INFO
--rw-rw-r--   0 scott     (1000) scott     (1000)      984 2024-04-07 00:48:47.000000 ansar-connect-0.1.135/src/ansar_connect.egg-info/SOURCES.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)        1 2024-04-07 00:48:47.000000 ansar-connect-0.1.135/src/ansar_connect.egg-info/dependency_links.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)      212 2024-04-07 00:48:47.000000 ansar-connect-0.1.135/src/ansar_connect.egg-info/entry_points.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)       21 2024-04-07 00:48:47.000000 ansar-connect-0.1.135/src/ansar_connect.egg-info/requires.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)        6 2024-04-07 00:48:47.000000 ansar-connect-0.1.135/src/ansar_connect.egg-info/top_level.txt
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-07 04:19:05.187583 ansar-connect-0.1.136/
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1124 2023-06-30 14:19:32.000000 ansar-connect-0.1.136/LICENSE
+-rw-r--r--   0 scott     (1000) scott     (1000)     2674 2024-04-07 04:19:05.187583 ansar-connect-0.1.136/PKG-INFO
+-rwxr-xr-x   0 scott     (1000) scott     (1000)     1966 2023-06-28 15:55:38.000000 ansar-connect-0.1.136/README.md
+-rwxr-xr-x   0 scott     (1000) scott     (1000)      723 2024-03-28 18:04:29.000000 ansar-connect-0.1.136/pyproject.toml
+-rw-rw-r--   0 scott     (1000) scott     (1000)       38 2024-04-07 04:19:05.187583 ansar-connect-0.1.136/setup.cfg
+-rwxr-xr-x   0 scott     (1000) scott     (1000)     2210 2024-03-28 18:04:17.000000 ansar-connect-0.1.136/setup.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-07 04:19:05.187583 ansar-connect-0.1.136/src/
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-07 04:19:05.187583 ansar-connect-0.1.136/src/ansar/
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-07 04:19:05.187583 ansar-connect-0.1.136/src/ansar/command/
+-rw-rw-r--   0 scott     (1000) scott     (1000)    14427 2024-03-29 02:37:30.000000 ansar-connect-0.1.136/src/ansar/command/ansar_command.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     3072 2024-03-04 07:28:05.000000 ansar-connect-0.1.136/src/ansar/command/ansar_directory.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     9940 2024-03-26 18:46:17.000000 ansar-connect-0.1.136/src/ansar/command/ansar_group.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     8658 2024-03-29 22:32:03.000000 ansar-connect-0.1.136/src/ansar/command/shared_directory.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-07 04:19:05.187583 ansar-connect-0.1.136/src/ansar/connect/
+-rwxrwxr-x   0 scott     (1000) scott     (1000)     3012 2024-04-07 04:19:02.000000 ansar-connect-0.1.136/src/ansar/connect/__init__.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    13865 2024-04-07 03:44:19.000000 ansar-connect-0.1.136/src/ansar/connect/connect_directory.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    77328 2024-04-07 00:39:18.000000 ansar-connect-0.1.136/src/ansar/connect/directory.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     7752 2024-04-01 20:33:07.000000 ansar-connect-0.1.136/src/ansar/connect/directory_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     9979 2024-04-02 12:37:04.000000 ansar-connect-0.1.136/src/ansar/connect/foh_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2119 2024-03-23 19:35:11.000000 ansar-connect-0.1.136/src/ansar/connect/group_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    14174 2024-03-01 03:02:47.000000 ansar-connect-0.1.136/src/ansar/connect/grouping.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2221 2024-04-02 20:33:16.000000 ansar-connect-0.1.136/src/ansar/connect/moving.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    21087 2024-04-06 01:12:06.000000 ansar-connect-0.1.136/src/ansar/connect/networking.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1558 2024-03-01 02:40:39.000000 ansar-connect-0.1.136/src/ansar/connect/networking_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    34999 2024-03-23 01:59:51.000000 ansar-connect-0.1.136/src/ansar/connect/node.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2091 2024-03-05 13:29:47.000000 ansar-connect-0.1.136/src/ansar/connect/plumbing.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    37271 2024-04-04 20:50:42.000000 ansar-connect-0.1.136/src/ansar/connect/procedure.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2323 2024-03-29 22:32:03.000000 ansar-connect-0.1.136/src/ansar/connect/product.py
+-rwxrwxr-x   0 scott     (1000) scott     (1000)    36421 2024-03-26 19:24:58.000000 ansar-connect-0.1.136/src/ansar/connect/socketry.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2159 2024-03-25 00:38:01.000000 ansar-connect-0.1.136/src/ansar/connect/standard.py
+-rwxr-xr-x   0 scott     (1000) scott     (1000)     2065 2023-09-27 02:08:10.000000 ansar-connect-0.1.136/src/ansar/connect/transporting.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     6367 2024-04-07 03:37:54.000000 ansar-connect-0.1.136/src/ansar/connect/wan.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-07 04:19:05.187583 ansar-connect-0.1.136/src/ansar_connect.egg-info/
+-rw-r--r--   0 scott     (1000) scott     (1000)     2674 2024-04-07 04:19:05.000000 ansar-connect-0.1.136/src/ansar_connect.egg-info/PKG-INFO
+-rw-rw-r--   0 scott     (1000) scott     (1000)      984 2024-04-07 04:19:05.000000 ansar-connect-0.1.136/src/ansar_connect.egg-info/SOURCES.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)        1 2024-04-07 04:19:05.000000 ansar-connect-0.1.136/src/ansar_connect.egg-info/dependency_links.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)      212 2024-04-07 04:19:05.000000 ansar-connect-0.1.136/src/ansar_connect.egg-info/entry_points.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)       21 2024-04-07 04:19:05.000000 ansar-connect-0.1.136/src/ansar_connect.egg-info/requires.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)        6 2024-04-07 04:19:05.000000 ansar-connect-0.1.136/src/ansar_connect.egg-info/top_level.txt
```

### Comparing `ansar-connect-0.1.135/LICENSE` & `ansar-connect-0.1.136/LICENSE`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.135/PKG-INFO` & `ansar-connect-0.1.136/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansar-connect
-Version: 0.1.135
+Version: 0.1.136
 Summary: Tools and runtime for asynchronous programming
 Author: Scott Woods
 Author-email: Scott Woods <scott.18.ansar@gmail.com.com>
 Project-URL: Documentation, https://ansar-connect-manual.s3.ap-southeast-2.amazonaws.com/0.1.1/index.html
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ansar-connect-0.1.135/README.md` & `ansar-connect-0.1.136/README.md`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.135/pyproject.toml` & `ansar-connect-0.1.136/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.135/setup.py` & `ansar-connect-0.1.136/setup.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.135/src/ansar/command/ansar_command.py` & `ansar-connect-0.1.136/src/ansar/command/ansar_command.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.135/src/ansar/command/ansar_directory.py` & `ansar-connect-0.1.136/src/ansar/command/ansar_directory.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.135/src/ansar/command/ansar_group.py` & `ansar-connect-0.1.136/src/ansar/command/ansar_group.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.135/src/ansar/command/shared_directory.py` & `ansar-connect-0.1.136/src/ansar/command/shared_directory.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.135/src/ansar/connect/__init__.py` & `ansar-connect-0.1.136/src/ansar/connect/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,16 +21,16 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 """Tools and runtime for asynchronous programming.
 
 Repo: git@github.com:mr-ansar/ansar-connect.git
 Branch: main
-Commit: 99cba99c752cd34c824bf5e5839f4fbb432fc948
-Version: 0.1.134 (2024-04-07@12:48:43+NZST)
+Commit: 3dda573a75708fd4a61d6a9d00c224478c2d1e93
+Version: 0.1.135 (2024-04-07@16:19:02+NZST)
 """
 
 from ansar.create import *
 
 #bind = bind_any
 #create = create_object
```

### Comparing `ansar-connect-0.1.135/src/ansar/connect/connect_directory.py` & `ansar-connect-0.1.136/src/ansar/connect/connect_directory.py`

 * *Files 1% similar despite different names*

```diff
@@ -227,15 +227,17 @@
 # Waiting for results of connect.
 # Transport established.
 def ConnectToDirectory_CLOUDY_Connected(self, message):
 	self.cancel(ar.T1)
 	self.connected = message
 
 	c = self.connect_above
-	lookup = WideAreaLookup(account_id=c.account_id, directory_id=c.directory_id)
+	lookup = WideAreaLookup(account_id=c.account_id, directory_id=c.directory_id,
+		access_token=c.access_token,
+		product_name=c.product_name, product_instance=c.product_instance)
 	self.reply(lookup)
 	self.start(ar.T2, seconds=4.0)
 	return LOOKING
 
 def ConnectToDirectory_CLOUDY_NotConnected(self, message):
 	self.send(message, self.parent_address)
 	self.cancel(ar.T1)
@@ -267,14 +269,23 @@
 	self.redirect = message
 	ipp = message.redirect_ipp
 	self.trace(f'Redirecting from FOH to WAN ({ipp})')
 	connect(self, ipp)
 	self.reply(Close())
 	return REDIRECTING
 
+def ConnectToDirectory_LOOKING_Faulted(self, message):
+	self.trace(f'Access denied - {message}')
+	self.send(Close(message), self.connected.remote_address)
+	if self.reschedule():
+		return GLARING
+
+	x = ar.Exhausted(message, attempts=self.attempts, started=self.started)
+	self.complete(x)
+
 def ConnectToDirectory_LOOKING_T2(self, message):
 	value = ar.TimedOut(message)
 	self.send(Close(value), self.connected.remote_address)
 	if self.reschedule():
 		return GLARING
 
 	x = ar.Exhausted(message, attempts=self.attempts, started=self.started)
@@ -353,14 +364,17 @@
 	self.attempts = 1
 	return self.connect()
 
 def ConnectToDirectory_GLARING_GlareTimer(self, message):
 	self.attempts += 1
 	return self.connect()
 
+def ConnectToDirectory_GLARING_Closed(self, message):
+	return GLARING
+
 def ConnectToDirectory_GLARING_Stop(self, message):
 	# Drop GlareTimer
 	self.complete(ar.Aborted())
 
 # CONNECTED
 # Caretaker role. Pass app messages on to owner
 # and wait for further control messages.
@@ -452,24 +466,24 @@
 	GLANCING: (
 		(YourProduct, ar.Stop), (ar.Anything,)
 	),
 	CLOUDY: (
 		(Connected, NotConnected, ar.T1, ar.Stop), (ar.Anything,)
 	),
 	LOOKING: (
-		(WideAreaRedirect, ar.T2, ar.Stop), (ar.Anything,)
+		(WideAreaRedirect, ar.Faulted, ar.T2, ar.Stop), (ar.Anything,)
 	),
 	REDIRECTING: (
 		(Connected, NotConnected, ar.T2, ar.Stop), (ar.Anything,)
 	),
 	ASSIGNING: (
 		(YourWideArea, Closed, ar.Unknown, ar.T2, ar.Stop), (ar.Anything,)
 	),
 	GLARING: (
-		(ar.Unknown, ar.Anything, GlareTimer, ar.Stop), ()
+		(ar.Unknown, ar.Anything, Closed, GlareTimer, ar.Stop), ()
 	),
 	CONNECTED: (
 		(ar.Unknown, ar.Anything, Abandoned, Closed, ar.Stop), ()
 	),
 	RECONNECTING: (
 		(Closed, Abandoned, ar.Stop), ()
 	),
```

### Comparing `ansar-connect-0.1.135/src/ansar/connect/directory.py` & `ansar-connect-0.1.136/src/ansar/connect/directory.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.135/src/ansar/connect/directory_if.py` & `ansar-connect-0.1.136/src/ansar/connect/directory_if.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.135/src/ansar/connect/foh_if.py` & `ansar-connect-0.1.136/src/ansar/connect/foh_if.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.135/src/ansar/connect/group_if.py` & `ansar-connect-0.1.136/src/ansar/connect/group_if.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.135/src/ansar/connect/grouping.py` & `ansar-connect-0.1.136/src/ansar/connect/grouping.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.135/src/ansar/connect/moving.py` & `ansar-connect-0.1.136/src/ansar/connect/moving.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.135/src/ansar/connect/networking.py` & `ansar-connect-0.1.136/src/ansar/connect/networking.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.135/src/ansar/connect/networking_if.py` & `ansar-connect-0.1.136/src/ansar/connect/networking_if.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.135/src/ansar/connect/node.py` & `ansar-connect-0.1.136/src/ansar/connect/node.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.135/src/ansar/connect/plumbing.py` & `ansar-connect-0.1.136/src/ansar/connect/plumbing.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.135/src/ansar/connect/procedure.py` & `ansar-connect-0.1.136/src/ansar/connect/procedure.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.135/src/ansar/connect/product.py` & `ansar-connect-0.1.136/src/ansar/connect/product.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.135/src/ansar/connect/socketry.py` & `ansar-connect-0.1.136/src/ansar/connect/socketry.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.135/src/ansar/connect/standard.py` & `ansar-connect-0.1.136/src/ansar/connect/standard.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.135/src/ansar/connect/transporting.py` & `ansar-connect-0.1.136/src/ansar/connect/transporting.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.135/src/ansar/connect/wan.py` & `ansar-connect-0.1.136/src/ansar/connect/wan.py`

 * *Files 4% similar despite different names*

```diff
@@ -100,17 +100,22 @@
 		self.product_instance = product_instance
 
 	def __str__(self):
 		t = InstanceOfProduct.to_name(self.product_instance)
 		return f'{self.product_name}/{t}'
 
 class WideAreaLookup(object):
-	def __init__(self, account_id=None, directory_id=None):
+	def __init__(self, account_id=None, directory_id=None,
+			access_token=None,
+			product_name=None, product_instance=None):
 		self.account_id = account_id
 		self.directory_id = directory_id
+		self.access_token = access_token
+		self.product_name = product_name
+		self.product_instance = product_instance
 
 class WideAreaRedirect(object):
 	def __init__(self, redirect_ipp=None, directory_id=None, assignment_token=None):
 		self.redirect_ipp = redirect_ipp or HostPort()
 		self.directory_id = directory_id
 		self.assignment_token = assignment_token
```

### Comparing `ansar-connect-0.1.135/src/ansar_connect.egg-info/PKG-INFO` & `ansar-connect-0.1.136/src/ansar_connect.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansar-connect
-Version: 0.1.135
+Version: 0.1.136
 Summary: Tools and runtime for asynchronous programming
 Author: Scott Woods
 Author-email: Scott Woods <scott.18.ansar@gmail.com.com>
 Project-URL: Documentation, https://ansar-connect-manual.s3.ap-southeast-2.amazonaws.com/0.1.1/index.html
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ansar-connect-0.1.135/src/ansar_connect.egg-info/SOURCES.txt` & `ansar-connect-0.1.136/src/ansar_connect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

