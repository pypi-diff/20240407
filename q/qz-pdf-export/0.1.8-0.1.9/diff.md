# Comparing `tmp/qz_pdf_export-0.1.8.tar.gz` & `tmp/qz_pdf_export-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qz_pdf_export-0.1.8.tar", last modified: Tue Mar 19 02:30:13 2024, max compression
+gzip compressed data, was "qz_pdf_export-0.1.9.tar", last modified: Tue Mar 19 02:40:49 2024, max compression
```

## Comparing `qz_pdf_export-0.1.8.tar` & `qz_pdf_export-0.1.9.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxrwx   0        0        0        0 2024-03-19 02:30:13.960011 qz_pdf_export-0.1.8/
--rw-rw-rw-   0        0        0       88 2024-03-07 03:52:57.000000 qz_pdf_export-0.1.8/MANIFEST.in
--rw-rw-rw-   0        0        0   374518 2024-03-19 02:30:13.959011 qz_pdf_export-0.1.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-03-19 02:30:13.929807 qz_pdf_export-0.1.8/example_pdf/
--rw-rw-rw-   0        0        0        0 2024-03-07 02:32:47.000000 qz_pdf_export-0.1.8/example_pdf/__init__.py
--rw-rw-rw-   0        0        0     2551 2024-03-19 01:56:41.000000 qz_pdf_export-0.1.8/example_pdf/admin.py
--rw-rw-rw-   0        0        0      159 2024-03-07 02:32:47.000000 qz_pdf_export-0.1.8/example_pdf/apps.py
-drwxrwxrwx   0        0        0        0 2024-03-19 02:30:13.937985 qz_pdf_export-0.1.8/example_pdf/migrations/
--rw-rw-rw-   0        0        0     3342 2024-03-07 02:34:43.000000 qz_pdf_export-0.1.8/example_pdf/migrations/0001_initial.py
--rw-rw-rw-   0        0        0     1254 2024-03-18 03:05:42.000000 qz_pdf_export-0.1.8/example_pdf/migrations/0002_modela_modelb_delete_todoitem_delete_todotype.py
--rw-rw-rw-   0        0        0      797 2024-03-18 03:21:08.000000 qz_pdf_export-0.1.8/example_pdf/migrations/0003_modelc.py
--rw-rw-rw-   0        0        0     1744 2024-03-18 03:44:16.000000 qz_pdf_export-0.1.8/example_pdf/migrations/0004_modeltype_modelx.py
--rw-rw-rw-   0        0        0      567 2024-03-18 08:17:46.000000 qz_pdf_export-0.1.8/example_pdf/migrations/0005_modela_modelx.py
--rw-rw-rw-   0        0        0      593 2024-03-18 08:19:03.000000 qz_pdf_export-0.1.8/example_pdf/migrations/0006_remove_modelx_model_filed7_modelx_model_filed7.py
--rw-rw-rw-   0        0        0     1004 2024-03-18 08:20:11.000000 qz_pdf_export-0.1.8/example_pdf/migrations/0007_remove_modela_modelx_remove_modelx_model_filed7_and_more.py
--rw-rw-rw-   0        0        0        0 2024-03-07 02:32:47.000000 qz_pdf_export-0.1.8/example_pdf/migrations/__init__.py
--rw-rw-rw-   0        0        0     1811 2024-03-18 08:20:07.000000 qz_pdf_export-0.1.8/example_pdf/models.py
--rw-rw-rw-   0        0        0       63 2024-03-07 02:32:47.000000 qz_pdf_export-0.1.8/example_pdf/tests.py
--rw-rw-rw-   0        0        0       66 2024-03-07 02:32:47.000000 qz_pdf_export-0.1.8/example_pdf/views.py
-drwxrwxrwx   0        0        0        0 2024-03-19 02:30:13.941991 qz_pdf_export-0.1.8/pass_PdfExport/
--rw-rw-rw-   0        0        0        0 2024-02-28 07:59:19.000000 qz_pdf_export-0.1.8/pass_PdfExport/__init__.py
--rw-rw-rw-   0        0        0      418 2024-03-07 02:04:49.000000 qz_pdf_export-0.1.8/pass_PdfExport/asgi.py
--rw-rw-rw-   0        0        0     3434 2024-03-07 02:34:13.000000 qz_pdf_export-0.1.8/pass_PdfExport/settings.py
--rw-rw-rw-   0        0        0      800 2024-03-18 07:08:21.000000 qz_pdf_export-0.1.8/pass_PdfExport/urls.py
--rw-rw-rw-   0        0        0      418 2024-03-07 02:04:57.000000 qz_pdf_export-0.1.8/pass_PdfExport/wsgi.py
-drwxrwxrwx   0        0        0        0 2024-03-19 02:30:13.947876 qz_pdf_export-0.1.8/pdfExport/
--rw-rw-rw-   0        0        0        0 2024-02-28 08:01:15.000000 qz_pdf_export-0.1.8/pdfExport/__init__.py
--rw-rw-rw-   0        0        0     7243 2024-03-19 01:59:21.000000 qz_pdf_export-0.1.8/pdfExport/admin.py
--rw-rw-rw-   0        0        0      156 2024-02-28 08:01:15.000000 qz_pdf_export-0.1.8/pdfExport/apps.py
--rw-rw-rw-   0        0        0       66 2024-03-07 02:33:28.000000 qz_pdf_export-0.1.8/pdfExport/models.py
-drwxrwxrwx   0        0        0        0 2024-03-19 02:30:13.922297 qz_pdf_export-0.1.8/pdfExport/templates/
-drwxrwxrwx   0        0        0        0 2024-03-19 02:30:13.950006 qz_pdf_export-0.1.8/pdfExport/templates/pdfExport/
--rw-rw-rw-   0        0        0     5937 2024-03-19 02:29:56.000000 qz_pdf_export-0.1.8/pdfExport/templates/pdfExport/base_pdf_template.html
--rw-rw-rw-   0        0        0      207 2024-03-07 02:30:08.000000 qz_pdf_export-0.1.8/pdfExport/templates/pdfExport/pdf_export_change_form.html
--rw-rw-rw-   0        0        0       63 2024-02-28 08:01:15.000000 qz_pdf_export-0.1.8/pdfExport/tests.py
--rw-rw-rw-   0        0        0        0 2024-03-18 07:08:27.000000 qz_pdf_export-0.1.8/pdfExport/views.py
-drwxrwxrwx   0        0        0        0 2024-03-19 02:30:13.957012 qz_pdf_export-0.1.8/qz_pdf_export.egg-info/
--rw-rw-rw-   0        0        0   374518 2024-03-19 02:30:13.000000 qz_pdf_export-0.1.8/qz_pdf_export.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1096 2024-03-19 02:30:13.000000 qz_pdf_export-0.1.8/qz_pdf_export.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-19 02:30:13.000000 qz_pdf_export-0.1.8/qz_pdf_export.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2024-03-19 02:30:13.000000 qz_pdf_export-0.1.8/qz_pdf_export.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-19 02:30:13.960011 qz_pdf_export-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0      662 2024-03-19 02:30:09.000000 qz_pdf_export-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-03-19 02:40:49.458202 qz_pdf_export-0.1.9/
+-rw-rw-rw-   0        0        0       88 2024-03-07 03:52:57.000000 qz_pdf_export-0.1.9/MANIFEST.in
+-rw-rw-rw-   0        0        0   374493 2024-03-19 02:40:49.457203 qz_pdf_export-0.1.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-03-19 02:40:49.428525 qz_pdf_export-0.1.9/example_pdf/
+-rw-rw-rw-   0        0        0        0 2024-03-07 02:32:47.000000 qz_pdf_export-0.1.9/example_pdf/__init__.py
+-rw-rw-rw-   0        0        0     2551 2024-03-19 01:56:41.000000 qz_pdf_export-0.1.9/example_pdf/admin.py
+-rw-rw-rw-   0        0        0      159 2024-03-07 02:32:47.000000 qz_pdf_export-0.1.9/example_pdf/apps.py
+drwxrwxrwx   0        0        0        0 2024-03-19 02:40:49.434862 qz_pdf_export-0.1.9/example_pdf/migrations/
+-rw-rw-rw-   0        0        0     3342 2024-03-07 02:34:43.000000 qz_pdf_export-0.1.9/example_pdf/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0     1254 2024-03-18 03:05:42.000000 qz_pdf_export-0.1.9/example_pdf/migrations/0002_modela_modelb_delete_todoitem_delete_todotype.py
+-rw-rw-rw-   0        0        0      797 2024-03-18 03:21:08.000000 qz_pdf_export-0.1.9/example_pdf/migrations/0003_modelc.py
+-rw-rw-rw-   0        0        0     1744 2024-03-18 03:44:16.000000 qz_pdf_export-0.1.9/example_pdf/migrations/0004_modeltype_modelx.py
+-rw-rw-rw-   0        0        0      567 2024-03-18 08:17:46.000000 qz_pdf_export-0.1.9/example_pdf/migrations/0005_modela_modelx.py
+-rw-rw-rw-   0        0        0      593 2024-03-18 08:19:03.000000 qz_pdf_export-0.1.9/example_pdf/migrations/0006_remove_modelx_model_filed7_modelx_model_filed7.py
+-rw-rw-rw-   0        0        0     1004 2024-03-18 08:20:11.000000 qz_pdf_export-0.1.9/example_pdf/migrations/0007_remove_modela_modelx_remove_modelx_model_filed7_and_more.py
+-rw-rw-rw-   0        0        0        0 2024-03-07 02:32:47.000000 qz_pdf_export-0.1.9/example_pdf/migrations/__init__.py
+-rw-rw-rw-   0        0        0     1811 2024-03-18 08:20:07.000000 qz_pdf_export-0.1.9/example_pdf/models.py
+-rw-rw-rw-   0        0        0       63 2024-03-07 02:32:47.000000 qz_pdf_export-0.1.9/example_pdf/tests.py
+-rw-rw-rw-   0        0        0       66 2024-03-07 02:32:47.000000 qz_pdf_export-0.1.9/example_pdf/views.py
+drwxrwxrwx   0        0        0        0 2024-03-19 02:40:49.438909 qz_pdf_export-0.1.9/pass_PdfExport/
+-rw-rw-rw-   0        0        0        0 2024-02-28 07:59:19.000000 qz_pdf_export-0.1.9/pass_PdfExport/__init__.py
+-rw-rw-rw-   0        0        0      418 2024-03-07 02:04:49.000000 qz_pdf_export-0.1.9/pass_PdfExport/asgi.py
+-rw-rw-rw-   0        0        0     3434 2024-03-07 02:34:13.000000 qz_pdf_export-0.1.9/pass_PdfExport/settings.py
+-rw-rw-rw-   0        0        0      800 2024-03-18 07:08:21.000000 qz_pdf_export-0.1.9/pass_PdfExport/urls.py
+-rw-rw-rw-   0        0        0      418 2024-03-07 02:04:57.000000 qz_pdf_export-0.1.9/pass_PdfExport/wsgi.py
+drwxrwxrwx   0        0        0        0 2024-03-19 02:40:49.444908 qz_pdf_export-0.1.9/pdfExport/
+-rw-rw-rw-   0        0        0        0 2024-02-28 08:01:15.000000 qz_pdf_export-0.1.9/pdfExport/__init__.py
+-rw-rw-rw-   0        0        0     7243 2024-03-19 01:59:21.000000 qz_pdf_export-0.1.9/pdfExport/admin.py
+-rw-rw-rw-   0        0        0      156 2024-02-28 08:01:15.000000 qz_pdf_export-0.1.9/pdfExport/apps.py
+-rw-rw-rw-   0        0        0       66 2024-03-07 02:33:28.000000 qz_pdf_export-0.1.9/pdfExport/models.py
+drwxrwxrwx   0        0        0        0 2024-03-19 02:40:49.421502 qz_pdf_export-0.1.9/pdfExport/templates/
+drwxrwxrwx   0        0        0        0 2024-03-19 02:40:49.448780 qz_pdf_export-0.1.9/pdfExport/templates/pdfExport/
+-rw-rw-rw-   0        0        0     5937 2024-03-19 02:29:56.000000 qz_pdf_export-0.1.9/pdfExport/templates/pdfExport/base_pdf_template.html
+-rw-rw-rw-   0        0        0      207 2024-03-07 02:30:08.000000 qz_pdf_export-0.1.9/pdfExport/templates/pdfExport/pdf_export_change_form.html
+-rw-rw-rw-   0        0        0       63 2024-02-28 08:01:15.000000 qz_pdf_export-0.1.9/pdfExport/tests.py
+-rw-rw-rw-   0        0        0        0 2024-03-18 07:08:27.000000 qz_pdf_export-0.1.9/pdfExport/views.py
+drwxrwxrwx   0        0        0        0 2024-03-19 02:40:49.454203 qz_pdf_export-0.1.9/qz_pdf_export.egg-info/
+-rw-rw-rw-   0        0        0   374493 2024-03-19 02:40:49.000000 qz_pdf_export-0.1.9/qz_pdf_export.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1096 2024-03-19 02:40:49.000000 qz_pdf_export-0.1.9/qz_pdf_export.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-03-19 02:40:49.000000 qz_pdf_export-0.1.9/qz_pdf_export.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2024-03-19 02:40:49.000000 qz_pdf_export-0.1.9/qz_pdf_export.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-03-19 02:40:49.458202 qz_pdf_export-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0      631 2024-03-19 02:40:38.000000 qz_pdf_export-0.1.9/setup.py
```

### Comparing `qz_pdf_export-0.1.8/PKG-INFO` & `qz_pdf_export-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: qz_pdf_export
-Version: 0.1.8
+Version: 0.1.9
 Summary: 方便快捷的pdf导出工具
 Home-page: 
 Author: qz
 Author-email: 2902934039@qq.com
 Classifier: Framework :: Django
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 
 新加PdfAdmin,如有需要导出pdf的admin直接继承PdfAdmin
 如需在列表添加查看pdf功能，在list_display中添加'pdf_show'字段
 
 setting.py中
```

### Comparing `qz_pdf_export-0.1.8/example_pdf/admin.py` & `qz_pdf_export-0.1.9/example_pdf/admin.py`

 * *Files identical despite different names*

### Comparing `qz_pdf_export-0.1.8/example_pdf/migrations/0001_initial.py` & `qz_pdf_export-0.1.9/example_pdf/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `qz_pdf_export-0.1.8/example_pdf/migrations/0002_modela_modelb_delete_todoitem_delete_todotype.py` & `qz_pdf_export-0.1.9/example_pdf/migrations/0002_modela_modelb_delete_todoitem_delete_todotype.py`

 * *Files identical despite different names*

### Comparing `qz_pdf_export-0.1.8/example_pdf/migrations/0003_modelc.py` & `qz_pdf_export-0.1.9/example_pdf/migrations/0003_modelc.py`

 * *Files identical despite different names*

### Comparing `qz_pdf_export-0.1.8/example_pdf/migrations/0004_modeltype_modelx.py` & `qz_pdf_export-0.1.9/example_pdf/migrations/0004_modeltype_modelx.py`

 * *Files identical despite different names*

### Comparing `qz_pdf_export-0.1.8/example_pdf/migrations/0005_modela_modelx.py` & `qz_pdf_export-0.1.9/example_pdf/migrations/0005_modela_modelx.py`

 * *Files identical despite different names*

### Comparing `qz_pdf_export-0.1.8/example_pdf/migrations/0006_remove_modelx_model_filed7_modelx_model_filed7.py` & `qz_pdf_export-0.1.9/example_pdf/migrations/0006_remove_modelx_model_filed7_modelx_model_filed7.py`

 * *Files identical despite different names*

### Comparing `qz_pdf_export-0.1.8/example_pdf/migrations/0007_remove_modela_modelx_remove_modelx_model_filed7_and_more.py` & `qz_pdf_export-0.1.9/example_pdf/migrations/0007_remove_modela_modelx_remove_modelx_model_filed7_and_more.py`

 * *Files identical despite different names*

### Comparing `qz_pdf_export-0.1.8/example_pdf/models.py` & `qz_pdf_export-0.1.9/example_pdf/models.py`

 * *Files identical despite different names*

### Comparing `qz_pdf_export-0.1.8/pass_PdfExport/settings.py` & `qz_pdf_export-0.1.9/pass_PdfExport/settings.py`

 * *Files identical despite different names*

### Comparing `qz_pdf_export-0.1.8/pass_PdfExport/urls.py` & `qz_pdf_export-0.1.9/pass_PdfExport/urls.py`

 * *Files identical despite different names*

### Comparing `qz_pdf_export-0.1.8/pdfExport/admin.py` & `qz_pdf_export-0.1.9/pdfExport/admin.py`

 * *Files identical despite different names*

### Comparing `qz_pdf_export-0.1.8/pdfExport/templates/pdfExport/base_pdf_template.html` & `qz_pdf_export-0.1.9/pdfExport/templates/pdfExport/base_pdf_template.html`

 * *Files identical despite different names*

### Comparing `qz_pdf_export-0.1.8/qz_pdf_export.egg-info/PKG-INFO` & `qz_pdf_export-0.1.9/qz_pdf_export.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: qz_pdf_export
-Version: 0.1.8
+Version: 0.1.9
 Summary: 方便快捷的pdf导出工具
 Home-page: 
 Author: qz
 Author-email: 2902934039@qq.com
 Classifier: Framework :: Django
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 
 新加PdfAdmin,如有需要导出pdf的admin直接继承PdfAdmin
 如需在列表添加查看pdf功能，在list_display中添加'pdf_show'字段
 
 setting.py中
```

### Comparing `qz_pdf_export-0.1.8/qz_pdf_export.egg-info/SOURCES.txt` & `qz_pdf_export-0.1.9/qz_pdf_export.egg-info/SOURCES.txt`

 * *Files identical despite different names*

