# Comparing `tmp/ansar-connect-0.1.134.tar.gz` & `tmp/ansar-connect-0.1.135.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansar-connect-0.1.134.tar", last modified: Sat Apr  6 04:55:52 2024, max compression
+gzip compressed data, was "ansar-connect-0.1.135.tar", last modified: Sun Apr  7 00:48:47 2024, max compression
```

## Comparing `ansar-connect-0.1.134.tar` & `ansar-connect-0.1.135.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-06 04:55:52.575913 ansar-connect-0.1.134/
--rw-rw-r--   0 scott     (1000) scott     (1000)     1124 2023-06-30 14:19:32.000000 ansar-connect-0.1.134/LICENSE
--rw-r--r--   0 scott     (1000) scott     (1000)     2674 2024-04-06 04:55:52.575913 ansar-connect-0.1.134/PKG-INFO
--rwxr-xr-x   0 scott     (1000) scott     (1000)     1966 2023-06-28 15:55:38.000000 ansar-connect-0.1.134/README.md
--rwxr-xr-x   0 scott     (1000) scott     (1000)      723 2024-03-28 18:04:29.000000 ansar-connect-0.1.134/pyproject.toml
--rw-rw-r--   0 scott     (1000) scott     (1000)       38 2024-04-06 04:55:52.575913 ansar-connect-0.1.134/setup.cfg
--rwxr-xr-x   0 scott     (1000) scott     (1000)     2210 2024-03-28 18:04:17.000000 ansar-connect-0.1.134/setup.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-06 04:55:52.571913 ansar-connect-0.1.134/src/
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-06 04:55:52.571913 ansar-connect-0.1.134/src/ansar/
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-06 04:55:52.571913 ansar-connect-0.1.134/src/ansar/command/
--rw-rw-r--   0 scott     (1000) scott     (1000)    14427 2024-03-29 02:37:30.000000 ansar-connect-0.1.134/src/ansar/command/ansar_command.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     3072 2024-03-04 07:28:05.000000 ansar-connect-0.1.134/src/ansar/command/ansar_directory.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     9940 2024-03-26 18:46:17.000000 ansar-connect-0.1.134/src/ansar/command/ansar_group.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     8658 2024-03-29 22:32:03.000000 ansar-connect-0.1.134/src/ansar/command/shared_directory.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-06 04:55:52.575913 ansar-connect-0.1.134/src/ansar/connect/
--rwxrwxr-x   0 scott     (1000) scott     (1000)     3012 2024-04-06 04:55:49.000000 ansar-connect-0.1.134/src/ansar/connect/__init__.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    13387 2024-03-23 02:08:11.000000 ansar-connect-0.1.134/src/ansar/connect/connect_directory.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    76423 2024-04-06 04:31:47.000000 ansar-connect-0.1.134/src/ansar/connect/directory.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     7752 2024-04-01 20:33:07.000000 ansar-connect-0.1.134/src/ansar/connect/directory_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     9979 2024-04-02 12:37:04.000000 ansar-connect-0.1.134/src/ansar/connect/foh_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2119 2024-03-23 19:35:11.000000 ansar-connect-0.1.134/src/ansar/connect/group_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    14174 2024-03-01 03:02:47.000000 ansar-connect-0.1.134/src/ansar/connect/grouping.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2221 2024-04-02 20:33:16.000000 ansar-connect-0.1.134/src/ansar/connect/moving.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    21087 2024-04-06 01:12:06.000000 ansar-connect-0.1.134/src/ansar/connect/networking.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     1558 2024-03-01 02:40:39.000000 ansar-connect-0.1.134/src/ansar/connect/networking_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    34999 2024-03-23 01:59:51.000000 ansar-connect-0.1.134/src/ansar/connect/node.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2091 2024-03-05 13:29:47.000000 ansar-connect-0.1.134/src/ansar/connect/plumbing.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    37271 2024-04-04 20:50:42.000000 ansar-connect-0.1.134/src/ansar/connect/procedure.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2323 2024-03-29 22:32:03.000000 ansar-connect-0.1.134/src/ansar/connect/product.py
--rwxrwxr-x   0 scott     (1000) scott     (1000)    36421 2024-03-26 19:24:58.000000 ansar-connect-0.1.134/src/ansar/connect/socketry.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2159 2024-03-25 00:38:01.000000 ansar-connect-0.1.134/src/ansar/connect/standard.py
--rwxr-xr-x   0 scott     (1000) scott     (1000)     2065 2023-09-27 02:08:10.000000 ansar-connect-0.1.134/src/ansar/connect/transporting.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     6187 2024-03-28 02:15:57.000000 ansar-connect-0.1.134/src/ansar/connect/wan.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-06 04:55:52.575913 ansar-connect-0.1.134/src/ansar_connect.egg-info/
--rw-r--r--   0 scott     (1000) scott     (1000)     2674 2024-04-06 04:55:52.000000 ansar-connect-0.1.134/src/ansar_connect.egg-info/PKG-INFO
--rw-rw-r--   0 scott     (1000) scott     (1000)      984 2024-04-06 04:55:52.000000 ansar-connect-0.1.134/src/ansar_connect.egg-info/SOURCES.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)        1 2024-04-06 04:55:52.000000 ansar-connect-0.1.134/src/ansar_connect.egg-info/dependency_links.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)      212 2024-04-06 04:55:52.000000 ansar-connect-0.1.134/src/ansar_connect.egg-info/entry_points.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)       21 2024-04-06 04:55:52.000000 ansar-connect-0.1.134/src/ansar_connect.egg-info/requires.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)        6 2024-04-06 04:55:52.000000 ansar-connect-0.1.134/src/ansar_connect.egg-info/top_level.txt
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-07 00:48:47.011826 ansar-connect-0.1.135/
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1124 2023-06-30 14:19:32.000000 ansar-connect-0.1.135/LICENSE
+-rw-r--r--   0 scott     (1000) scott     (1000)     2674 2024-04-07 00:48:47.011826 ansar-connect-0.1.135/PKG-INFO
+-rwxr-xr-x   0 scott     (1000) scott     (1000)     1966 2023-06-28 15:55:38.000000 ansar-connect-0.1.135/README.md
+-rwxr-xr-x   0 scott     (1000) scott     (1000)      723 2024-03-28 18:04:29.000000 ansar-connect-0.1.135/pyproject.toml
+-rw-rw-r--   0 scott     (1000) scott     (1000)       38 2024-04-07 00:48:47.011826 ansar-connect-0.1.135/setup.cfg
+-rwxr-xr-x   0 scott     (1000) scott     (1000)     2210 2024-03-28 18:04:17.000000 ansar-connect-0.1.135/setup.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-07 00:48:47.007826 ansar-connect-0.1.135/src/
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-07 00:48:47.007826 ansar-connect-0.1.135/src/ansar/
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-07 00:48:47.011826 ansar-connect-0.1.135/src/ansar/command/
+-rw-rw-r--   0 scott     (1000) scott     (1000)    14427 2024-03-29 02:37:30.000000 ansar-connect-0.1.135/src/ansar/command/ansar_command.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     3072 2024-03-04 07:28:05.000000 ansar-connect-0.1.135/src/ansar/command/ansar_directory.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     9940 2024-03-26 18:46:17.000000 ansar-connect-0.1.135/src/ansar/command/ansar_group.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     8658 2024-03-29 22:32:03.000000 ansar-connect-0.1.135/src/ansar/command/shared_directory.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-07 00:48:47.011826 ansar-connect-0.1.135/src/ansar/connect/
+-rwxrwxr-x   0 scott     (1000) scott     (1000)     3012 2024-04-07 00:48:43.000000 ansar-connect-0.1.135/src/ansar/connect/__init__.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    13387 2024-03-23 02:08:11.000000 ansar-connect-0.1.135/src/ansar/connect/connect_directory.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    77328 2024-04-07 00:39:18.000000 ansar-connect-0.1.135/src/ansar/connect/directory.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     7752 2024-04-01 20:33:07.000000 ansar-connect-0.1.135/src/ansar/connect/directory_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     9979 2024-04-02 12:37:04.000000 ansar-connect-0.1.135/src/ansar/connect/foh_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2119 2024-03-23 19:35:11.000000 ansar-connect-0.1.135/src/ansar/connect/group_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    14174 2024-03-01 03:02:47.000000 ansar-connect-0.1.135/src/ansar/connect/grouping.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2221 2024-04-02 20:33:16.000000 ansar-connect-0.1.135/src/ansar/connect/moving.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    21087 2024-04-06 01:12:06.000000 ansar-connect-0.1.135/src/ansar/connect/networking.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1558 2024-03-01 02:40:39.000000 ansar-connect-0.1.135/src/ansar/connect/networking_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    34999 2024-03-23 01:59:51.000000 ansar-connect-0.1.135/src/ansar/connect/node.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2091 2024-03-05 13:29:47.000000 ansar-connect-0.1.135/src/ansar/connect/plumbing.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    37271 2024-04-04 20:50:42.000000 ansar-connect-0.1.135/src/ansar/connect/procedure.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2323 2024-03-29 22:32:03.000000 ansar-connect-0.1.135/src/ansar/connect/product.py
+-rwxrwxr-x   0 scott     (1000) scott     (1000)    36421 2024-03-26 19:24:58.000000 ansar-connect-0.1.135/src/ansar/connect/socketry.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2159 2024-03-25 00:38:01.000000 ansar-connect-0.1.135/src/ansar/connect/standard.py
+-rwxr-xr-x   0 scott     (1000) scott     (1000)     2065 2023-09-27 02:08:10.000000 ansar-connect-0.1.135/src/ansar/connect/transporting.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     6187 2024-03-28 02:15:57.000000 ansar-connect-0.1.135/src/ansar/connect/wan.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-07 00:48:47.011826 ansar-connect-0.1.135/src/ansar_connect.egg-info/
+-rw-r--r--   0 scott     (1000) scott     (1000)     2674 2024-04-07 00:48:47.000000 ansar-connect-0.1.135/src/ansar_connect.egg-info/PKG-INFO
+-rw-rw-r--   0 scott     (1000) scott     (1000)      984 2024-04-07 00:48:47.000000 ansar-connect-0.1.135/src/ansar_connect.egg-info/SOURCES.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)        1 2024-04-07 00:48:47.000000 ansar-connect-0.1.135/src/ansar_connect.egg-info/dependency_links.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)      212 2024-04-07 00:48:47.000000 ansar-connect-0.1.135/src/ansar_connect.egg-info/entry_points.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)       21 2024-04-07 00:48:47.000000 ansar-connect-0.1.135/src/ansar_connect.egg-info/requires.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)        6 2024-04-07 00:48:47.000000 ansar-connect-0.1.135/src/ansar_connect.egg-info/top_level.txt
```

### Comparing `ansar-connect-0.1.134/LICENSE` & `ansar-connect-0.1.135/LICENSE`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.134/PKG-INFO` & `ansar-connect-0.1.135/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansar-connect
-Version: 0.1.134
+Version: 0.1.135
 Summary: Tools and runtime for asynchronous programming
 Author: Scott Woods
 Author-email: Scott Woods <scott.18.ansar@gmail.com.com>
 Project-URL: Documentation, https://ansar-connect-manual.s3.ap-southeast-2.amazonaws.com/0.1.1/index.html
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ansar-connect-0.1.134/README.md` & `ansar-connect-0.1.135/README.md`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.134/pyproject.toml` & `ansar-connect-0.1.135/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.134/setup.py` & `ansar-connect-0.1.135/setup.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.134/src/ansar/command/ansar_command.py` & `ansar-connect-0.1.135/src/ansar/command/ansar_command.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.134/src/ansar/command/ansar_directory.py` & `ansar-connect-0.1.135/src/ansar/command/ansar_directory.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.134/src/ansar/command/ansar_group.py` & `ansar-connect-0.1.135/src/ansar/command/ansar_group.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.134/src/ansar/command/shared_directory.py` & `ansar-connect-0.1.135/src/ansar/command/shared_directory.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.134/src/ansar/connect/__init__.py` & `ansar-connect-0.1.135/src/ansar/connect/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -21,16 +21,16 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 """Tools and runtime for asynchronous programming.
 
 Repo: git@github.com:mr-ansar/ansar-connect.git
 Branch: main
-Commit: 90770010a44a59f2a8a4a6e5fc1227b47045b73d
-Version: 0.1.133 (2024-04-06@17:55:49+NZDT)
+Commit: 99cba99c752cd34c824bf5e5839f4fbb432fc948
+Version: 0.1.134 (2024-04-07@12:48:43+NZST)
 """
 
 from ansar.create import *
 
 #bind = bind_any
 #create = create_object
```

### Comparing `ansar-connect-0.1.134/src/ansar/connect/connect_directory.py` & `ansar-connect-0.1.135/src/ansar/connect/connect_directory.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.134/src/ansar/connect/directory.py` & `ansar-connect-0.1.135/src/ansar/connect/directory.py`

 * *Files 2% similar despite different names*

```diff
@@ -468,14 +468,29 @@
 	try:
 		a = key.index('@')
 		c = key.index(':')
 	except ValueError:
 		return None
 	return key[a + 1:c]
 
+def id_connection(kid):
+	try:
+		a = kid.index('(')
+		c = kid.index(')')
+	except ValueError:
+		return None
+	return kid[a + 1:c]
+
+def id_process(kid):
+	try:
+		a = kid.index(')')
+	except ValueError:
+		return None
+	return kid[a + 1:]
+
 def overlapping_route(a, b):
 	ra = reversed(a)
 	rb = reversed(b)
 	for x, y in zip(ra, rb):
 		if x != y:
 			return False
 	return True
@@ -511,18 +526,17 @@
 		listing_address = listing.agent_address
 		listing_id = listing.listing_id
 		listing_matched = d[1]
 
 		# As well as being unique within this directory the
 		# connection engine in the subscriber agent relies on
 		# content and layout of this key. Refer to
-		# key_service().
-		key_service
+		# key_service(), key_id(), etc.
 		who = address_to_text(find_address)
-		key = f'{who}@{listing_id}:{listing.requested_name}'
+		key = f'{who}@{listing_address}{listing_id}:{listing.requested_name}'
 
 		if key in self.matched:
 			self.warning(f'Duplicate find/service match [{ScopeOfService.to_name(self.scope)}] "{key}"')
 			return
 		self.trace(f'Adds route [{ScopeOfService.to_name(self.scope)}] "{key}"')
 
 		# Everything lines up - we have a relation. Connection details
@@ -1714,16 +1728,17 @@
 # Stop -> application
 def SubscriberLoop_LOOPED_Completed(self, message):
 	d = self.debrief()
 	# 0) Latch, 1) Session, *) Unknown
 	if d == 1:
 		self.forward(Cleared(message.value), self.subscriber_address, self.origin_address)
 	else:
-		self.warning(f'Unexpected loop completion {d}')
-		self.forward(Dropped(f'Loop management'), self.subscriber_address, self.origin_address)
+		f = ar.Faulted('Loop management', f'unexpected completion {d}')
+		self.warning(str(f))
+		self.forward(Cleared(f), self.subscriber_address, self.origin_address)
 
 	self.close_loop()
 
 	if self.working():
 		self.abort()
 		self.clearing_value = True
 		return CLEARING
@@ -1747,15 +1762,15 @@
 	if self.working():
 		self.abort()
 		self.clearing_value = False
 		return CLEARING
 	self.complete(False)
 
 def SubscriberLoop_LOOPED_Stop(self, message):
-	self.forward(Dropped('Aborted'), self.subscriber_address, self.origin_address)
+	self.forward(Cleared(ar.Aborted()), self.subscriber_address, self.origin_address)
 
 	self.close_loop()
 
 	if self.working():
 		self.abort()
 		self.clearing_value = False
 		return CLEARING
@@ -1840,16 +1855,17 @@
 
 def SubscriberLoop_CONNECTION_LOOPED_Completed(self, message):
 	d = self.debrief()
 	# 0) Latch, 1) Session, *) Unknown
 	if d == 1:
 		self.forward(Cleared(message.value), self.subscriber_address, self.origin_address)
 	else:
-		self.warning(f'Unexpected loop completion {d}')
-		self.forward(Dropped(f'Loop management'), self.subscriber_address, self.origin_address)
+		f = ar.Faulted('Loop management', f'unexpected completion {d}')
+		self.warning(str(f))
+		self.forward(Cleared(f), self.subscriber_address, self.origin_address)
 
 	self.close_loop()
 	self.close_peer()
 	if self.working():
 		self.abort()
 		self.clearing_value = True
 		return CLEARING
@@ -1884,15 +1900,15 @@
 	if self.working():
 		self.abort()
 		self.clearing_value = False
 		return CLEARING
 	self.complete(False)
 
 def SubscriberLoop_CONNECTION_LOOPED_Stop(self, message):
-	self.forward(Dropped('Aborted'), self.subscriber_address, self.origin_address)
+	self.forward(Cleared(ar.Aborted()), self.subscriber_address, self.origin_address)
 
 	self.close_loop()
 	self.close_peer()
 
 	if self.working():
 		self.abort()
 		self.clearing_value = False
@@ -1981,16 +1997,17 @@
 
 def SubscriberLoop_RELAY_LOOPED_Completed(self, message):
 	d = self.debrief()
 	# 0) Latch, 1) Session, *) Unknown
 	if d == 1:
 		self.forward(Cleared(message.value), self.subscriber_address, self.origin_address)
 	else:
-		self.warning(f'Unexpected loop completion {d}')
-		self.forward(Dropped(f'Loop management'), self.subscriber_address, self.origin_address)
+		f = ar.Faulted('Loop management', f'unexpected completion {d}')
+		self.warning(str(f))
+		self.forward(Cleared(f), self.subscriber_address, self.origin_address)
 
 	self.close_loop()
 	self.close_relay()
 	self.close_peer()
 
 	if self.working():
 		self.abort()
@@ -2032,15 +2049,15 @@
 	if self.working():
 		self.abort()
 		self.clearing_value = False
 		return CLEARING
 	self.complete(False)
 
 def SubscriberLoop_RELAY_LOOPED_Stop(self, message):
-	self.forward(Dropped('Aborted'), self.subscriber_address, self.origin_address)
+	self.forward(Cleared(ar.Aborted()), self.subscriber_address, self.origin_address)
 
 	self.close_loop()
 	self.close_relay()
 	self.close_peer()
 
 	if self.working():
 		self.abort()
@@ -2128,33 +2145,56 @@
 			self.service_looping[name] = looping
 			return
 
 		table, opened, loop, completed = looping
 		table[scope] = route
 
 		if route.scope == opened.scope:
-			self.trace(f'Replacement [{sos}] route')
-			if loop is None and not completed and key_id(route.key) != key_id(opened.key):
-				self.trace(f'Start replacement loop "{name}" [{sos}] {tag}')
-				a = self.create(SubscriberLoop, route, self.subscriber_address, self.create_session)
-				self.assign(a, name)
-				looping[1] = route
-				looping[2] = a
+			if loop:
+				self.trace(f'Replacement [{sos}] route (loop running)')
+				return
+			if completed:
+				self.trace(f'Replacement [{sos}] route (previous positive completion)')
+				return
+
+			route_id = key_id(route.key)
+			opened_id = key_id(opened.key)
+			if route_id == opened_id:
+				self.trace(f'Replacement [{sos}] route (no change)')
+				return
+
+			if id_process(route_id) != id_process(opened_id):
+				s = 'process'
+			elif id_connection(route_id) != id_connection(opened_id):
+				s = 'connection'
+			else:
+				self.warning(f'Replacement [{sos}] route (change of id but not process or connection)')
+				return
+
+			self.trace(f'Start replacement [{sos}] route for "{name}", change of {s}')
+			a = self.create(SubscriberLoop, route, self.subscriber_address, self.create_session)
+			self.assign(a, name)
+			looping[1] = route
+			looping[2] = a
 			return
 
 		if route.scope < opened.scope:
 			if loop:
-				self.trace(f'Better [{sos}] route, pushing current loop')
+				self.trace(f'Upgrade [{sos}] route, pushing current loop')
 				self.send(ar.Stop(), loop)
-			elif not completed:
-				self.trace(f'Start continuation loop "{name}" [{sos}] {tag}')
-				a = self.create(SubscriberLoop, route, self.subscriber_address, self.create_session)
-				self.assign(a, name)
-				looping[1] = route
-				looping[2] = a
+				return
+			if completed:
+				self.trace(f'Upgrade [{sos}] route, (previous positive completion)')
+				return
+
+			self.trace(f'Start upgrade [{sos}] route for "{name}"')
+			a = self.create(SubscriberLoop, route, self.subscriber_address, self.create_session)
+			self.assign(a, name)
+			looping[1] = route
+			looping[2] = a
 			return
 
 		self.trace(f'Fallback [{sos}] route')
 
 
 # Register interest in services matching pattern.
 def SubscriptionAgent_INITIAL_Start(self, message):
```

### Comparing `ansar-connect-0.1.134/src/ansar/connect/directory_if.py` & `ansar-connect-0.1.135/src/ansar/connect/directory_if.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.134/src/ansar/connect/foh_if.py` & `ansar-connect-0.1.135/src/ansar/connect/foh_if.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.134/src/ansar/connect/group_if.py` & `ansar-connect-0.1.135/src/ansar/connect/group_if.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.134/src/ansar/connect/grouping.py` & `ansar-connect-0.1.135/src/ansar/connect/grouping.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.134/src/ansar/connect/moving.py` & `ansar-connect-0.1.135/src/ansar/connect/moving.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.134/src/ansar/connect/networking.py` & `ansar-connect-0.1.135/src/ansar/connect/networking.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.134/src/ansar/connect/networking_if.py` & `ansar-connect-0.1.135/src/ansar/connect/networking_if.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.134/src/ansar/connect/node.py` & `ansar-connect-0.1.135/src/ansar/connect/node.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.134/src/ansar/connect/plumbing.py` & `ansar-connect-0.1.135/src/ansar/connect/plumbing.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.134/src/ansar/connect/procedure.py` & `ansar-connect-0.1.135/src/ansar/connect/procedure.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.134/src/ansar/connect/product.py` & `ansar-connect-0.1.135/src/ansar/connect/product.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.134/src/ansar/connect/socketry.py` & `ansar-connect-0.1.135/src/ansar/connect/socketry.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.134/src/ansar/connect/standard.py` & `ansar-connect-0.1.135/src/ansar/connect/standard.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.134/src/ansar/connect/transporting.py` & `ansar-connect-0.1.135/src/ansar/connect/transporting.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.134/src/ansar/connect/wan.py` & `ansar-connect-0.1.135/src/ansar/connect/wan.py`

 * *Files identical despite different names*

### Comparing `ansar-connect-0.1.134/src/ansar_connect.egg-info/PKG-INFO` & `ansar-connect-0.1.135/src/ansar_connect.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansar-connect
-Version: 0.1.134
+Version: 0.1.135
 Summary: Tools and runtime for asynchronous programming
 Author: Scott Woods
 Author-email: Scott Woods <scott.18.ansar@gmail.com.com>
 Project-URL: Documentation, https://ansar-connect-manual.s3.ap-southeast-2.amazonaws.com/0.1.1/index.html
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ansar-connect-0.1.134/src/ansar_connect.egg-info/SOURCES.txt` & `ansar-connect-0.1.135/src/ansar_connect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

