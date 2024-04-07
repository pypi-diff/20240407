# Comparing `tmp/weasyform-0.0.7.tar.gz` & `tmp/weasyform-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "weasyform-0.0.7.tar", last modified: Tue Apr 12 20:50:41 2022, max compression
+gzip compressed data, was "weasyform-0.0.8.tar", last modified: Sun Apr  7 06:57:02 2024, max compression
```

## Comparing `weasyform-0.0.7.tar` & `weasyform-0.0.8.tar`

### file list

```diff
@@ -1,20 +1,15 @@
-drwxr-xr-x   0 sadam     (1000) users      (100)        0 2022-04-12 20:50:41.792861 weasyform-0.0.7/
--rw-r--r--   0 sadam     (1000) users      (100)     1121 2022-04-12 20:50:41.792861 weasyform-0.0.7/PKG-INFO
--rw-r--r--   0 sadam     (1000) users      (100)      126 2022-03-13 18:55:31.000000 weasyform-0.0.7/README.md
--rw-r--r--   0 sadam     (1000) users      (100)       38 2022-04-12 20:50:41.792861 weasyform-0.0.7/setup.cfg
--rw-r--r--   0 sadam     (1000) users      (100)     1380 2022-04-12 20:50:12.000000 weasyform-0.0.7/setup.py
--rw-r--r--   0 sadam     (1000) users      (100)     1110 2022-03-21 17:34:56.000000 weasyform-0.0.7/test.py
-drwxr-xr-x   0 sadam     (1000) users      (100)        0 2022-04-12 20:50:41.792861 weasyform-0.0.7/weasyform/
--rw-r--r--   0 sadam     (1000) users      (100)     1559 2022-04-12 20:49:12.000000 weasyform-0.0.7/weasyform/FormFinisher.py
--rw-r--r--   0 sadam     (1000) users      (100)     3056 2022-03-27 14:04:10.000000 weasyform-0.0.7/weasyform/WeasyForm.py
--rw-r--r--   0 sadam     (1000) users      (100)     6492 2022-03-22 14:22:29.000000 weasyform-0.0.7/weasyform/__init__.py
--rw-r--r--   0 sadam     (1000) users      (100)       89 2022-03-13 11:27:01.000000 weasyform-0.0.7/weasyform/exceptions.py
-drwxr-xr-x   0 sadam     (1000) users      (100)        0 2022-04-12 20:50:41.792861 weasyform-0.0.7/weasyform/fields/
--rw-r--r--   0 sadam     (1000) users      (100)        0 2022-03-08 23:14:08.000000 weasyform-0.0.7/weasyform/fields/__init__.py
--rw-r--r--   0 sadam     (1000) users      (100)     5837 2022-03-26 14:12:59.000000 weasyform-0.0.7/weasyform/fields/signature.py
-drwxr-xr-x   0 sadam     (1000) users      (100)        0 2022-04-12 20:50:41.792861 weasyform-0.0.7/weasyform.egg-info/
--rw-r--r--   0 sadam     (1000) users      (100)     1121 2022-04-12 20:50:41.000000 weasyform-0.0.7/weasyform.egg-info/PKG-INFO
--rw-r--r--   0 sadam     (1000) users      (100)      344 2022-04-12 20:50:41.000000 weasyform-0.0.7/weasyform.egg-info/SOURCES.txt
--rw-r--r--   0 sadam     (1000) users      (100)        1 2022-04-12 20:50:41.000000 weasyform-0.0.7/weasyform.egg-info/dependency_links.txt
--rw-r--r--   0 sadam     (1000) users      (100)       11 2022-04-12 20:50:41.000000 weasyform-0.0.7/weasyform.egg-info/requires.txt
--rw-r--r--   0 sadam     (1000) users      (100)       10 2022-04-12 20:50:41.000000 weasyform-0.0.7/weasyform.egg-info/top_level.txt
+drwxr-xr-x   0 sadam     (1000) users      (100)        0 2024-04-07 06:57:02.335121 weasyform-0.0.8/
+-rw-r--r--   0 sadam     (1000) users      (100)     1134 2024-04-07 06:57:02.335121 weasyform-0.0.8/PKG-INFO
+-rw-r--r--   0 sadam     (1000) users      (100)      126 2022-03-13 18:55:31.000000 weasyform-0.0.8/README.md
+-rw-r--r--   0 sadam     (1000) users      (100)       38 2024-04-07 06:57:02.335121 weasyform-0.0.8/setup.cfg
+-rw-r--r--   0 sadam     (1000) users      (100)     1386 2024-04-07 06:53:45.000000 weasyform-0.0.8/setup.py
+-rw-r--r--   0 sadam     (1000) users      (100)     1203 2024-04-06 22:23:31.000000 weasyform-0.0.8/test.py
+drwxr-xr-x   0 sadam     (1000) users      (100)        0 2024-04-07 06:57:02.335121 weasyform-0.0.8/weasyform/
+-rw-r--r--   0 sadam     (1000) users      (100)     6203 2024-04-06 22:22:56.000000 weasyform-0.0.8/weasyform/FormFinisher.py
+-rw-r--r--   0 sadam     (1000) users      (100)        0 2024-04-06 22:04:54.000000 weasyform-0.0.8/weasyform/__init__.py
+drwxr-xr-x   0 sadam     (1000) users      (100)        0 2024-04-07 06:57:02.335121 weasyform-0.0.8/weasyform.egg-info/
+-rw-r--r--   0 sadam     (1000) users      (100)     1134 2024-04-07 06:57:02.000000 weasyform-0.0.8/weasyform.egg-info/PKG-INFO
+-rw-r--r--   0 sadam     (1000) users      (100)      238 2024-04-07 06:57:02.000000 weasyform-0.0.8/weasyform.egg-info/SOURCES.txt
+-rw-r--r--   0 sadam     (1000) users      (100)        1 2024-04-07 06:57:02.000000 weasyform-0.0.8/weasyform.egg-info/dependency_links.txt
+-rw-r--r--   0 sadam     (1000) users      (100)       17 2024-04-07 06:57:02.000000 weasyform-0.0.8/weasyform.egg-info/requires.txt
+-rw-r--r--   0 sadam     (1000) users      (100)       10 2024-04-07 06:57:02.000000 weasyform-0.0.8/weasyform.egg-info/top_level.txt
```

### Comparing `weasyform-0.0.7/PKG-INFO` & `weasyform-0.0.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: weasyform
-Version: 0.0.7
+Version: 0.0.8
 Summary: Simple form support for WeasyPrint
 Home-page: https://github.com/Salamek/weasyform
 Author: Adam Schubert
 Author-email: adam.schubert@sg1-game.net
 License: BSD
 Project-URL: Release notes, https://github.com/Salamek/weasyform/releases
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -19,12 +18,12 @@
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Software Development
 Requires-Python: >=3.4
 Description-Content-Type: text/markdown
+Requires-Dist: WeasyPrint>=61.0
 
 # [WIP] WeasyPrint form support
 
 Only input type="signature" is supported to create PDF signature placeholder in generated PDF
-
```

### Comparing `weasyform-0.0.7/setup.py` & `weasyform-0.0.8/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 def read_readme() -> str:
     with open('README.md', 'r', encoding='utf-8') as f:
         return f.read()
 
 
 setup(
     name='weasyform',
-    version='0.0.7',
+    version='0.0.8',
     packages=find_packages(exclude=['tests', 'tests.*']),
     install_requires=[
-        'WeasyPrint'
+        'WeasyPrint>=61.0'
     ],
 
     url='https://github.com/Salamek/weasyform',
     license='BSD',
     author='Adam Schubert',
     author_email='adam.schubert@sg1-game.net',
     description='Simple form support for WeasyPrint',
```

### Comparing `weasyform-0.0.7/test.py` & `weasyform-0.0.8/test.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from weasyform.FormFinisher import FormFinisher
-from weasyform import HTML
-
+from weasyprint import HTML
 html = """
 <style>
 table {
     width: 100%;
     
 }
 
@@ -13,45 +12,48 @@
 }
 
 input {
     width: 100%;
     height: 20px;
 }
 
+input, textarea, select {
+  display: block;
+  appearance: auto;
+}
+
 </style>
 <h1>TEST</h1>
 <table>
 <tr>
     <th>URL</th><td><a href="https://salamek.cz">This is a URL</a></td>
 </tr>
 <tr>
     <th>URL</th><td><textarea name="asdasd">dfsfsf</textarea></td>
 </tr>
 <tr>
     <th>Signature</th><td><input type="signature" name="testSignature" style="width: 100% height: 20px"></td>
 </tr>
 <tr>
-    <th>Input text</th><td><input name="testText" type="text"></td>
+    <th>Input text</th><td><input name="testText" type="text" value="value"/></td>
 </tr>
 <tr>
     <th>Input number</th><td><input name="testNumber" type="number"></td>
 </tr>
 <tr>
     <th>Input email</th><td><input name="testEmail" type="email"></td>
 </tr>
 <tr>
     <th>Select</th><td><select name="testSelect"><option>A</option><option>B</option></select></td>
 </tr>
 </table>
 """
 
+
 pdf_html = HTML(string=html).render()
 
 
 target = 'forms.pdf'
-form_finisher = FormFinisher(inject_empty_cryptographic_signature=True)
-pdf_html.write_pdf(finisher=form_finisher)
-
-form_finisher.write_pdf(target)
-
+form_finisher = FormFinisher(inject_empty_cryptographic_signature=False, is_signature_visible=False)
+pdf_html.write_pdf(finisher=form_finisher, target=target)
```

#### html2text {}

```diff
@@ -1,13 +1,14 @@
-from weasyform.FormFinisher import FormFinisher from weasyform import HTML html
-= """
+from weasyform.FormFinisher import FormFinisher from weasyprint import HTML
+html = """
 ************ TTEESSTT ************
 UURRLL          _T_h_i_s_ _i_s_ _a_ _U_R_L
 UURRLL          dfsfsf
 SSiiggnnaattuurree    [Unknown INPUT type]
-IInnppuutt tteexxtt   [testText            ]
+IInnppuutt tteexxtt   [value               ]
 IInnppuutt nnuummbbeerr [Unknown INPUT type]
 IInnppuutt eemmaaiill  [Unknown INPUT type]
 SSeelleecctt       [One of: A/B]
 """ pdf_html = HTML(string=html).render() target = 'forms.pdf' form_finisher =
-FormFinisher(inject_empty_cryptographic_signature=True) pdf_html.write_pdf
-(finisher=form_finisher) form_finisher.write_pdf(target)
+FormFinisher(inject_empty_cryptographic_signature=False,
+is_signature_visible=False) pdf_html.write_pdf(finisher=form_finisher,
+target=target)
```

### Comparing `weasyform-0.0.7/weasyform.egg-info/PKG-INFO` & `weasyform-0.0.8/weasyform.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: weasyform
-Version: 0.0.7
+Version: 0.0.8
 Summary: Simple form support for WeasyPrint
 Home-page: https://github.com/Salamek/weasyform
 Author: Adam Schubert
 Author-email: adam.schubert@sg1-game.net
 License: BSD
 Project-URL: Release notes, https://github.com/Salamek/weasyform/releases
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -19,12 +18,12 @@
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Software Development
 Requires-Python: >=3.4
 Description-Content-Type: text/markdown
+Requires-Dist: WeasyPrint>=61.0
 
 # [WIP] WeasyPrint form support
 
 Only input type="signature" is supported to create PDF signature placeholder in generated PDF
-
```

