# Comparing `tmp/rubymarshal-1.2.6.tar.gz` & `tmp/rubymarshal-1.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/rubymarshal-1.2.6.tar", last modified: Mon Jun 10 06:56:47 2019, max compression
+gzip compressed data, was "dist/rubymarshal-1.2.7.tar", last modified: Mon Aug 10 21:40:58 2020, max compression
```

## Comparing `rubymarshal-1.2.6.tar` & `rubymarshal-1.2.7.tar`

### file list

```diff
@@ -1,27 +1,20 @@
-drwxr-xr-x   0 flanker    (501) staff       (20)        0 2019-06-10 06:56:47.000000 rubymarshal-1.2.6/
--rw-r--r--   0 flanker    (501) staff       (20)      478 2019-06-05 06:17:11.000000 rubymarshal-1.2.6/LICENSE
--rw-r--r--   0 flanker    (501) staff       (20)      103 2019-06-05 06:17:11.000000 rubymarshal-1.2.6/MANIFEST.in
--rw-r--r--   0 flanker    (501) staff       (20)     4234 2019-06-10 06:56:47.000000 rubymarshal-1.2.6/PKG-INFO
--rw-r--r--   0 flanker    (501) staff       (20)     2656 2019-06-09 15:00:24.000000 rubymarshal-1.2.6/README.md
-drwxr-xr-x   0 flanker    (501) staff       (20)        0 2019-06-10 06:56:47.000000 rubymarshal-1.2.6/rubymarshal/
--rw-r--r--   0 flanker    (501) staff       (20)       53 2019-06-10 06:55:46.000000 rubymarshal-1.2.6/rubymarshal/__init__.py
--rw-r--r--   0 flanker    (501) staff       (20)     4956 2019-06-10 06:55:46.000000 rubymarshal-1.2.6/rubymarshal/classes.py
--rw-r--r--   0 flanker    (501) staff       (20)     1311 2019-06-05 17:41:03.000000 rubymarshal-1.2.6/rubymarshal/constants.py
--rw-r--r--   0 flanker    (501) staff       (20)     9000 2019-06-09 21:46:21.000000 rubymarshal-1.2.6/rubymarshal/reader.py
--rw-r--r--   0 flanker    (501) staff       (20)      478 2019-06-07 06:07:24.000000 rubymarshal-1.2.6/rubymarshal/utils.py
--rw-r--r--   0 flanker    (501) staff       (20)     9224 2019-06-09 14:49:53.000000 rubymarshal-1.2.6/rubymarshal/writer.py
-drwxr-xr-x   0 flanker    (501) staff       (20)        0 2019-06-10 06:56:47.000000 rubymarshal-1.2.6/rubymarshal.egg-info/
--rw-r--r--   0 flanker    (501) staff       (20)     4234 2019-06-10 06:56:47.000000 rubymarshal-1.2.6/rubymarshal.egg-info/PKG-INFO
--rw-r--r--   0 flanker    (501) staff       (20)      471 2019-06-10 06:56:47.000000 rubymarshal-1.2.6/rubymarshal.egg-info/SOURCES.txt
--rw-r--r--   0 flanker    (501) staff       (20)        1 2019-06-10 06:56:47.000000 rubymarshal-1.2.6/rubymarshal.egg-info/dependency_links.txt
--rw-r--r--   0 flanker    (501) staff       (20)       12 2019-06-10 06:56:47.000000 rubymarshal-1.2.6/rubymarshal.egg-info/top_level.txt
--rw-r--r--   0 flanker    (501) staff       (20)        1 2019-06-08 14:45:08.000000 rubymarshal-1.2.6/rubymarshal.egg-info/zip-safe
--rw-r--r--   0 flanker    (501) staff       (20)       38 2019-06-10 06:56:47.000000 rubymarshal-1.2.6/setup.cfg
--rw-r--r--   0 flanker    (501) staff       (20)     1348 2019-06-09 14:24:49.000000 rubymarshal-1.2.6/setup.py
-drwxr-xr-x   0 flanker    (501) staff       (20)        0 2019-06-10 06:56:47.000000 rubymarshal-1.2.6/tests/
--rw-r--r--   0 flanker    (501) staff       (20)      259 2019-06-09 14:58:59.000000 rubymarshal-1.2.6/tests/__init__.py
--rw-r--r--   0 flanker    (501) staff       (20)     1079 2019-06-05 06:22:03.000000 rubymarshal-1.2.6/tests/test_hypothesis.py
--rw-r--r--   0 flanker    (501) staff       (20)    16076 2019-06-09 14:55:13.000000 rubymarshal-1.2.6/tests/test_reader.py
--rw-r--r--   0 flanker    (501) staff       (20)      347 2019-06-05 06:22:03.000000 rubymarshal-1.2.6/tests/test_symbol.py
--rw-r--r--   0 flanker    (501) staff       (20)     1584 2019-06-05 06:22:03.000000 rubymarshal-1.2.6/tests/test_utils.py
--rw-r--r--   0 flanker    (501) staff       (20)     6138 2019-06-09 14:53:53.000000 rubymarshal-1.2.6/tests/test_writer.py
+drwxr-xr-x   0 flanker    (501) staff       (20)        0 2020-08-10 21:40:58.147720 rubymarshal-1.2.7/
+-rw-r--r--   0 flanker    (501) staff       (20)      478 2020-07-19 13:18:55.000000 rubymarshal-1.2.7/LICENSE
+-rw-r--r--   0 flanker    (501) staff       (20)      103 2020-07-19 13:18:55.000000 rubymarshal-1.2.7/MANIFEST.in
+-rw-r--r--   0 flanker    (501) staff       (20)     4184 2020-08-10 21:40:58.147362 rubymarshal-1.2.7/PKG-INFO
+-rw-r--r--   0 flanker    (501) staff       (20)     2656 2020-07-19 13:18:55.000000 rubymarshal-1.2.7/README.md
+drwxr-xr-x   0 flanker    (501) staff       (20)        0 2020-08-10 21:40:58.124059 rubymarshal-1.2.7/rubymarshal/
+-rw-r--r--   0 flanker    (501) staff       (20)       53 2020-08-10 21:36:50.000000 rubymarshal-1.2.7/rubymarshal/__init__.py
+-rw-r--r--   0 flanker    (501) staff       (20)     4975 2020-08-10 21:06:31.000000 rubymarshal-1.2.7/rubymarshal/classes.py
+-rw-r--r--   0 flanker    (501) staff       (20)     1311 2020-07-19 13:18:55.000000 rubymarshal-1.2.7/rubymarshal/constants.py
+-rw-r--r--   0 flanker    (501) staff       (20)     9825 2020-08-10 21:12:59.000000 rubymarshal-1.2.7/rubymarshal/reader.py
+-rw-r--r--   0 flanker    (501) staff       (20)      478 2020-07-19 13:18:55.000000 rubymarshal-1.2.7/rubymarshal/utils.py
+-rw-r--r--   0 flanker    (501) staff       (20)     9377 2020-07-19 13:18:55.000000 rubymarshal-1.2.7/rubymarshal/writer.py
+drwxr-xr-x   0 flanker    (501) staff       (20)        0 2020-08-10 21:40:58.146616 rubymarshal-1.2.7/rubymarshal.egg-info/
+-rw-r--r--   0 flanker    (501) staff       (20)     4184 2020-08-10 21:40:58.000000 rubymarshal-1.2.7/rubymarshal.egg-info/PKG-INFO
+-rw-r--r--   0 flanker    (501) staff       (20)      345 2020-08-10 21:40:58.000000 rubymarshal-1.2.7/rubymarshal.egg-info/SOURCES.txt
+-rw-r--r--   0 flanker    (501) staff       (20)        1 2020-08-10 21:40:58.000000 rubymarshal-1.2.7/rubymarshal.egg-info/dependency_links.txt
+-rw-r--r--   0 flanker    (501) staff       (20)       12 2020-08-10 21:40:58.000000 rubymarshal-1.2.7/rubymarshal.egg-info/top_level.txt
+-rw-r--r--   0 flanker    (501) staff       (20)        1 2020-08-10 20:48:37.000000 rubymarshal-1.2.7/rubymarshal.egg-info/zip-safe
+-rw-r--r--   0 flanker    (501) staff       (20)       38 2020-08-10 21:40:58.147828 rubymarshal-1.2.7/setup.cfg
+-rw-r--r--   0 flanker    (501) staff       (20)     1299 2020-07-19 13:18:55.000000 rubymarshal-1.2.7/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `rubymarshal-1.2.6/PKG-INFO` & `rubymarshal-1.2.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rubymarshal
-Version: 1.2.6
+Version: 1.2.7
 Summary: Read and write Ruby-marshalled data
 Home-page: https://github.com/d9pouces/RubyMarshal
 Author: Matthieu Gallet
 Author-email: github@19pouces.net
 License: WTFPL
 Description: RubyMarshal
         ===========
@@ -115,13 +115,12 @@
           * Documentation is on readthedocs: http://rubymarshal.readthedocs.org/en/latest/ 
           * Tests are on travis-ci: https://travis-ci.org/d9pouces/RubyMarshal
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
```

### Comparing `rubymarshal-1.2.6/README.md` & `rubymarshal-1.2.7/README.md`

 * *Files identical despite different names*

### Comparing `rubymarshal-1.2.6/rubymarshal/classes.py` & `rubymarshal-1.2.7/rubymarshal/classes.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,15 +63,15 @@
     def __lt__(self, other):
         return self.text < other
 
     def __gt__(self, other):
         return self.text > other
 
     def __le__(self, other):
-        return self.text > other
+        return self.text <= other
 
     def __ge__(self, other):
         return self.text >= other
 
     def __iter__(self):
         yield from self.text
 
@@ -162,15 +162,15 @@
         self._registry[cls.ruby_class_name] = cls
 
     def unregister(self, cls: Type[RubyObject]):
         assert issubclass(cls, RubyObject)
         if cls.ruby_class_name in self._registry:
             del self._registry[cls.ruby_class_name]
 
-    def get(self, ruby_class_name: str, default_cls):
+    def get(self, ruby_class_name: str, default_cls: Type[RubyObject]):
         return self._registry.get(ruby_class_name, default_cls)
 
     def __contains__(self, item):
         return item in self._registry
 
     def __getitem__(self, item):
         return self._registry[item]
```

### Comparing `rubymarshal-1.2.6/rubymarshal/constants.py` & `rubymarshal-1.2.7/rubymarshal/constants.py`

 * *Files identical despite different names*

### Comparing `rubymarshal-1.2.6/rubymarshal/reader.py` & `rubymarshal-1.2.7/rubymarshal/reader.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,14 +46,18 @@
         self.objects = []
         self.fd = fd
         self.registry = registry or global_registry
 
     def read(self, token=None):
         if token is None:
             token = self.fd.read(1)
+
+        # From https://docs.ruby-lang.org/en/2.1.0/marshal_rdoc.html:
+        # The stream contains only one copy of each object for all objects except
+        # true, false, nil, Fixnums and Symbols.
         object_index = None
         if token in (
             TYPE_IVAR,
             # TYPE_EXTENDED, TYPE_UCLASS, ????
             TYPE_CLASS,
             TYPE_MODULE,
             TYPE_FLOAT,
@@ -64,16 +68,18 @@
             TYPE_STRUCT,
             TYPE_OBJECT,
             TYPE_DATA,
             TYPE_USRMARSHAL,
         ):
             self.objects.append(None)
             object_index = len(self.objects)
+
+        result = None
         if token == TYPE_NIL:
-            result = None
+            pass
         elif token == TYPE_TRUE:
             result = True
         elif token == TYPE_FALSE:
             result = False
         elif token == TYPE_IVAR:
             sub_token = self.fd.read(1)
             result = self.read(sub_token)
@@ -84,15 +90,18 @@
                 if options & 1:
                     flags |= re.IGNORECASE
                 if options & 4:
                     flags |= re.MULTILINE
             attributes = self.read_attributes()
             if sub_token in (TYPE_STRING, TYPE_REGEXP):
                 encoding = self._get_encoding(attributes)
-                result = result.decode(encoding)
+                try:
+                    result = result.decode(encoding)
+                except UnicodeDecodeError as u:
+                    result = result.decode("unicode-escape")
             # string instance attributes are discarded
             if attributes and sub_token == TYPE_STRING:
                 result = RubyString(result, attributes)
             if sub_token == TYPE_REGEXP:
                 result = re.compile(str(result), flags)
             elif attributes:
                 result.set_attributes(attributes)
@@ -113,42 +122,52 @@
             for x in range(num_elements):
                 key = self.read()
                 value = self.read()
                 result[key] = value
             result = result
         elif token == TYPE_FLOAT:
             size = self.read_long()
-            result = float(self.fd.read(size).decode("utf-8"))
+            floatn = self.fd.read(size)
+            floatn = floatn.split(b"\0")
+            result = float(floatn[0].decode("utf-8"))
         elif token == TYPE_BIGNUM:
             sign = 1 if self.fd.read(1) == b"+" else -1
             num_elements = self.read_long()
             result = 0
             factor = 1
             for x in range(num_elements):
                 result += self.read_short() * factor
                 factor *= 2 ** 16
             result *= sign
         elif token == TYPE_REGEXP:
             size = self.read_long()
             result = self.fd.read(size)
         elif token == TYPE_USRMARSHAL:
-            class_name = self.read()
+            class_symbol = self.read()
+            if not isinstance(class_symbol, Symbol):
+                raise ValueError("invalid class name: %r" % class_symbol)
+            class_name = class_symbol.name
             attr_list = self.read()
             python_class = self.registry.get(class_name, UsrMarshal)
             if not issubclass(python_class, UsrMarshal):
                 raise ValueError(
                     "invalid class mapping for %r: %r should be a subclass of %r."
                     % (class_name, python_class, UsrMarshal)
                 )
             result = python_class(class_name)
             result.marshal_load(attr_list)
         elif token == TYPE_SYMLINK:
             result = self.read_symlink()
         elif token == TYPE_LINK:
             link_id = self.read_long()
+            if object_index and link_id >= object_index:
+                raise ValueError(
+                    "invalid link destination: %d should be lower than %d."
+                    % (link_id, object_index)
+                )
             result = self.objects[link_id]
         elif token == TYPE_USERDEF:
             class_symbol = self.read()
             private_data = self.read(TYPE_STRING)
             if not isinstance(class_symbol, Symbol):
                 raise ValueError("invalid class name: %r" % class_symbol)
             class_name = class_symbol.name
```

### Comparing `rubymarshal-1.2.6/rubymarshal/writer.py` & `rubymarshal-1.2.7/rubymarshal/writer.py`

 * *Files 2% similar despite different names*

```diff
@@ -120,18 +120,22 @@
             self.write_long(len(bdata))
             self.fd.write(bdata)
             if obj.attributes:
                 self.write_attributes(obj.attributes)
 
     def write_usr_marshal(self, obj):
         if self.must_write(obj):
+            if obj.attributes:
+                self.fd.write(TYPE_IVAR)
             self.fd.write(TYPE_USRMARSHAL)
             self.write(Symbol(obj.ruby_class_name))
-            obj_attributes = obj.marshal_dump()
-            self.write(obj_attributes)
+            private_data = obj.marshal_dump()
+            self.write(private_data)
+            if obj.attributes:
+                self.write_attributes(obj.attributes)
 
     def write_module(self, obj):
         self.fd.write(TYPE_MODULE)
         self.write_long(len(obj.ruby_class_name.encode()))
         self.fd.write(obj.ruby_class_name.encode())
 
     def write_regexp(self, obj):
```

### Comparing `rubymarshal-1.2.6/rubymarshal.egg-info/PKG-INFO` & `rubymarshal-1.2.7/rubymarshal.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rubymarshal
-Version: 1.2.6
+Version: 1.2.7
 Summary: Read and write Ruby-marshalled data
 Home-page: https://github.com/d9pouces/RubyMarshal
 Author: Matthieu Gallet
 Author-email: github@19pouces.net
 License: WTFPL
 Description: RubyMarshal
         ===========
@@ -115,13 +115,12 @@
           * Documentation is on readthedocs: http://rubymarshal.readthedocs.org/en/latest/ 
           * Tests are on travis-ci: https://travis-ci.org/d9pouces/RubyMarshal
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
```

### Comparing `rubymarshal-1.2.6/setup.py` & `rubymarshal-1.2.7/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -30,14 +30,13 @@
     install_requires=[],
     setup_requires=[],
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: System Administrators",
         "License :: OSI Approved",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.5",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Topic :: Utilities",
     ],
 )
```

