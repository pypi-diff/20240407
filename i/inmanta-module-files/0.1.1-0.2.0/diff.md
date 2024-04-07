# Comparing `tmp/inmanta_module_files-0.1.1-py3-none-any.whl.zip` & `tmp/inmanta_module_files-0.2.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,21 @@
-Zip file size: 18566 bytes, number of entries: 17
--rw-r--r--  2.0 unx      602 b- defN 24-Mar-10 17:03 inmanta_plugins/files/__init__.py
--rw-r--r--  2.0 unx     2583 b- defN 24-Mar-10 17:03 inmanta_plugins/files/base.py
--rw-r--r--  2.0 unx     6585 b- defN 24-Mar-10 17:03 inmanta_plugins/files/host.py
--rw-r--r--  2.0 unx     5848 b- defN 24-Mar-10 17:03 inmanta_plugins/files/json.py
--rw-r--r--  2.0 unx     2170 b- defN 24-Mar-10 17:04 inmanta_plugins/files/setup.cfg
--rw-r--r--  2.0 unx     2258 b- defN 24-Mar-10 17:03 inmanta_plugins/files/systemd_unit.py
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-10 17:03 inmanta_plugins/files/files/.gitkeep
--rw-r--r--  2.0 unx     3202 b- defN 24-Mar-10 17:03 inmanta_plugins/files/model/_init.cf
--rw-r--r--  2.0 unx     1661 b- defN 24-Mar-10 17:03 inmanta_plugins/files/model/host.cf
--rw-r--r--  2.0 unx     1586 b- defN 24-Mar-10 17:03 inmanta_plugins/files/model/json.cf
--rw-r--r--  2.0 unx    10884 b- defN 24-Mar-10 17:03 inmanta_plugins/files/model/systemd_unit.cf
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-10 17:03 inmanta_plugins/files/templates/.gitkeep
--rw-r--r--  2.0 unx     2950 b- defN 24-Mar-10 17:03 inmanta_plugins/files/templates/systemd_unit.j2
--rw-r--r--  2.0 unx      431 b- defN 24-Mar-10 17:04 inmanta_module_files-0.1.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Mar-10 17:04 inmanta_module_files-0.1.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       16 b- defN 24-Mar-10 17:04 inmanta_module_files-0.1.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1544 b- defN 24-Mar-10 17:04 inmanta_module_files-0.1.1.dist-info/RECORD
-17 files, 42412 bytes uncompressed, 15972 bytes compressed:  62.3%
+Zip file size: 20900 bytes, number of entries: 19
+-rw-r--r--  2.0 unx      602 b- defN 24-Apr-07 17:20 inmanta_plugins/files/__init__.py
+-rw-r--r--  2.0 unx     2624 b- defN 24-Apr-07 17:20 inmanta_plugins/files/base.py
+-rw-r--r--  2.0 unx     2330 b- defN 24-Apr-07 17:20 inmanta_plugins/files/directory.py
+-rw-r--r--  2.0 unx     6585 b- defN 24-Apr-07 17:20 inmanta_plugins/files/host.py
+-rw-r--r--  2.0 unx     5848 b- defN 24-Apr-07 17:20 inmanta_plugins/files/json.py
+-rw-r--r--  2.0 unx     2170 b- defN 24-Apr-07 17:21 inmanta_plugins/files/setup.cfg
+-rw-r--r--  2.0 unx     2258 b- defN 24-Apr-07 17:20 inmanta_plugins/files/systemd_unit.py
+-rw-r--r--  2.0 unx     2200 b- defN 24-Apr-07 17:20 inmanta_plugins/files/text.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-07 17:20 inmanta_plugins/files/files/.gitkeep
+-rw-r--r--  2.0 unx     3679 b- defN 24-Apr-07 17:20 inmanta_plugins/files/model/_init.cf
+-rw-r--r--  2.0 unx     1661 b- defN 24-Apr-07 17:20 inmanta_plugins/files/model/host.cf
+-rw-r--r--  2.0 unx     1586 b- defN 24-Apr-07 17:20 inmanta_plugins/files/model/json.cf
+-rw-r--r--  2.0 unx    10884 b- defN 24-Apr-07 17:20 inmanta_plugins/files/model/systemd_unit.cf
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-07 17:20 inmanta_plugins/files/templates/.gitkeep
+-rw-r--r--  2.0 unx     2950 b- defN 24-Apr-07 17:20 inmanta_plugins/files/templates/systemd_unit.j2
+-rw-r--r--  2.0 unx      742 b- defN 24-Apr-07 17:21 inmanta_module_files-0.2.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-07 17:21 inmanta_module_files-0.2.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       16 b- defN 24-Apr-07 17:21 inmanta_module_files-0.2.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1721 b- defN 24-Apr-07 17:21 inmanta_module_files-0.2.0.dist-info/RECORD
+19 files, 47948 bytes uncompressed, 18028 bytes compressed:  62.4%
```

## zipnote {}

```diff
@@ -1,25 +1,31 @@
 Filename: inmanta_plugins/files/__init__.py
 Comment: 
 
 Filename: inmanta_plugins/files/base.py
 Comment: 
 
+Filename: inmanta_plugins/files/directory.py
+Comment: 
+
 Filename: inmanta_plugins/files/host.py
 Comment: 
 
 Filename: inmanta_plugins/files/json.py
 Comment: 
 
 Filename: inmanta_plugins/files/setup.cfg
 Comment: 
 
 Filename: inmanta_plugins/files/systemd_unit.py
 Comment: 
 
+Filename: inmanta_plugins/files/text.py
+Comment: 
+
 Filename: inmanta_plugins/files/files/.gitkeep
 Comment: 
 
 Filename: inmanta_plugins/files/model/_init.cf
 Comment: 
 
 Filename: inmanta_plugins/files/model/host.cf
@@ -33,20 +39,20 @@
 
 Filename: inmanta_plugins/files/templates/.gitkeep
 Comment: 
 
 Filename: inmanta_plugins/files/templates/systemd_unit.j2
 Comment: 
 
-Filename: inmanta_module_files-0.1.1.dist-info/METADATA
+Filename: inmanta_module_files-0.2.0.dist-info/METADATA
 Comment: 
 
-Filename: inmanta_module_files-0.1.1.dist-info/WHEEL
+Filename: inmanta_module_files-0.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: inmanta_module_files-0.1.1.dist-info/top_level.txt
+Filename: inmanta_module_files-0.2.0.dist-info/top_level.txt
 Comment: 
 
-Filename: inmanta_module_files-0.1.1.dist-info/RECORD
+Filename: inmanta_module_files-0.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## inmanta_plugins/files/base.py

```diff
@@ -23,15 +23,17 @@
 import inmanta.agent.io.local
 import inmanta.const
 import inmanta.execute.proxy
 import inmanta.export
 import inmanta.resources
 
 
-class BaseFileResource(inmanta.resources.PurgeableResource):
+class BaseFileResource(
+    inmanta.resources.PurgeableResource, inmanta.resources.ManagedResource
+):
     fields = ("path", "permissions", "owner", "group")
     path: str
     permissions: typing.Optional[int]
     owner: typing.Optional[str]
     group: typing.Optional[str]
```

## inmanta_plugins/files/setup.cfg

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = inmanta-module-files
-version = 0.1.1
+version = 0.2.0
 description = Simple module containing various types of resource to manage files.
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Guillaume Everarts de Velp
 author_email = edvgui@gmail.com
 license = ASL 2.0
 copyright = 2023 Guillaume Everarts de Velp
```

## inmanta_plugins/files/model/_init.cf

```diff
@@ -48,14 +48,28 @@
 end
 BaseFile.host [1] -- std::Host
 """
 The host that this file is managed on.
 """
 
 
+entity TextFile extends BaseFile:
+    """
+    A simple text file.
+
+    :attr content: The content of the text file
+    """
+    string content
+end
+
+index TextFile(host, path)
+
+implement TextFile using std::none
+
+
 entity HostFile extends BaseFile:
     """
     A host file containing a mapping from ips to domain names.  The host file
     is comanaged, we will only merge/replace/remove entries which are specified in
     the entries relation.
     """
 end
@@ -110,7 +124,21 @@
 """
 Compose the [install] section of the file
 """
 
 index SystemdUnitFile(host, path)
 
 implement SystemdUnitFile using std::none
+
+
+entity Directory extends BaseFile:
+    """
+    Create a directory on the host.
+
+    :attr create_parents: Create all the parents directory, recursively.
+    """
+    bool create_parents = false
+end
+
+index Directory(host, path)
+
+implement Directory using std::none
```

