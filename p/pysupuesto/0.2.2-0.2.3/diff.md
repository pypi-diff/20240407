# Comparing `tmp/pysupuesto-0.2.2.tar.gz` & `tmp/pysupuesto-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysupuesto-0.2.2.tar", last modified: Thu Apr 28 21:12:51 2022, max compression
+gzip compressed data, was "pysupuesto-0.2.3.tar", last modified: Sun Apr  7 17:21:58 2024, max compression
```

## Comparing `pysupuesto-0.2.2.tar` & `pysupuesto-0.2.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 mato      (1000) mato      (1000)        0 2022-04-28 21:12:51.088217 pysupuesto-0.2.2/
--rw-rw-r--   0 mato      (1000) mato      (1000)       72 2022-04-28 21:11:52.000000 pysupuesto-0.2.2/CHANGELOG.txt
--rw-rw-r--   0 mato      (1000) mato      (1000)       32 2021-10-01 18:48:52.000000 pysupuesto-0.2.2/MANIFEST.in
--rw-rw-r--   0 mato      (1000) mato      (1000)     4481 2022-04-28 21:12:51.088217 pysupuesto-0.2.2/PKG-INFO
--rw-rw-r--   0 mato      (1000) mato      (1000)     3787 2021-10-01 22:00:58.000000 pysupuesto-0.2.2/README.md
-drwxrwxr-x   0 mato      (1000) mato      (1000)        0 2022-04-28 21:12:51.088217 pysupuesto-0.2.2/pysupuesto/
--rw-rw-r--   0 mato      (1000) mato      (1000)     5879 2022-04-28 19:21:09.000000 pysupuesto-0.2.2/pysupuesto/__init__.py
-drwxrwxr-x   0 mato      (1000) mato      (1000)        0 2022-04-28 21:12:51.088217 pysupuesto-0.2.2/pysupuesto.egg-info/
--rw-rw-r--   0 mato      (1000) mato      (1000)     4481 2022-04-28 21:12:51.000000 pysupuesto-0.2.2/pysupuesto.egg-info/PKG-INFO
--rw-rw-r--   0 mato      (1000) mato      (1000)      220 2022-04-28 21:12:51.000000 pysupuesto-0.2.2/pysupuesto.egg-info/SOURCES.txt
--rw-rw-r--   0 mato      (1000) mato      (1000)        1 2022-04-28 21:12:51.000000 pysupuesto-0.2.2/pysupuesto.egg-info/dependency_links.txt
--rw-rw-r--   0 mato      (1000) mato      (1000)       11 2022-04-28 21:12:51.000000 pysupuesto-0.2.2/pysupuesto.egg-info/top_level.txt
--rw-rw-r--   0 mato      (1000) mato      (1000)      148 2021-09-19 15:23:21.000000 pysupuesto-0.2.2/requirements.txt
--rw-rw-r--   0 mato      (1000) mato      (1000)       38 2022-04-28 21:12:51.088217 pysupuesto-0.2.2/setup.cfg
--rw-rw-r--   0 mato      (1000) mato      (1000)      818 2022-04-28 21:11:46.000000 pysupuesto-0.2.2/setup.py
+drwxrwxr-x   0 mato      (1000) mato      (1000)        0 2024-04-07 17:21:58.939612 pysupuesto-0.2.3/
+-rw-rw-r--   0 mato      (1000) mato      (1000)      208 2024-04-07 17:18:33.000000 pysupuesto-0.2.3/CHANGELOG.txt
+-rw-rw-r--   0 mato      (1000) mato      (1000)       32 2021-10-01 18:48:52.000000 pysupuesto-0.2.3/MANIFEST.in
+-rw-rw-r--   0 mato      (1000) mato      (1000)     4590 2024-04-07 17:21:58.935612 pysupuesto-0.2.3/PKG-INFO
+-rw-rw-r--   0 mato      (1000) mato      (1000)     3787 2021-10-01 22:00:58.000000 pysupuesto-0.2.3/README.md
+drwxrwxr-x   0 mato      (1000) mato      (1000)        0 2024-04-07 17:21:58.935612 pysupuesto-0.2.3/pysupuesto/
+-rw-rw-r--   0 mato      (1000) mato      (1000)     6079 2024-04-07 17:09:38.000000 pysupuesto-0.2.3/pysupuesto/__init__.py
+drwxrwxr-x   0 mato      (1000) mato      (1000)        0 2024-04-07 17:21:58.935612 pysupuesto-0.2.3/pysupuesto.egg-info/
+-rw-rw-r--   0 mato      (1000) mato      (1000)     4590 2024-04-07 17:21:58.000000 pysupuesto-0.2.3/pysupuesto.egg-info/PKG-INFO
+-rw-rw-r--   0 mato      (1000) mato      (1000)      220 2024-04-07 17:21:58.000000 pysupuesto-0.2.3/pysupuesto.egg-info/SOURCES.txt
+-rw-rw-r--   0 mato      (1000) mato      (1000)        1 2024-04-07 17:21:58.000000 pysupuesto-0.2.3/pysupuesto.egg-info/dependency_links.txt
+-rw-rw-r--   0 mato      (1000) mato      (1000)       11 2024-04-07 17:21:58.000000 pysupuesto-0.2.3/pysupuesto.egg-info/top_level.txt
+-rw-rw-r--   0 mato      (1000) mato      (1000)      148 2021-09-19 15:23:21.000000 pysupuesto-0.2.3/requirements.txt
+-rw-rw-r--   0 mato      (1000) mato      (1000)       38 2024-04-07 17:21:58.939612 pysupuesto-0.2.3/setup.cfg
+-rw-rw-r--   0 mato      (1000) mato      (1000)      818 2024-04-07 17:10:19.000000 pysupuesto-0.2.3/setup.py
```

### Comparing `pysupuesto-0.2.2/PKG-INFO` & `pysupuesto-0.2.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: pysupuesto
-Version: 0.2.2
+Version: 0.2.3
 Summary: Módulo para descargar bases de diferentes ejercicios (o series temporales) del presupuesto público nacional argentino desde el Ministerio de Economía
-Home-page: UNKNOWN
+Home-page: 
 Author: @Mato
 Author-email: no@email.org
 License: MIT
 Keywords: presupuesto,budget
-Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Other Audience
 Classifier: Operating System :: POSIX :: Linux
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 
@@ -104,13 +103,14 @@
 - Mejorar el sistema de logs.
 - Intentar analizar toda la información disponible (para eso cree ``get_docs``) para expandir el modulo y poner a disposición mayor cantidad descargas.
 
 
 	
 
 
+CHANGELOG
 
-
-Version 0.2.2:
+VERSION 0.2.2:
+- Update url for downloading data from years 2019-2023
+- Change 'append' (now deprecated) package for 'concat'.
+VERSION 0.2.2:
 - Change url for downloading data from years 1995-2018
-
-
```

### Comparing `pysupuesto-0.2.2/README.md` & `pysupuesto-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `pysupuesto-0.2.2/pysupuesto/__init__.py` & `pysupuesto-0.2.3/pysupuesto/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,15 +28,18 @@
              2014:{'diario':'', 'mensual':'-mensual-2014', 'anual':'-anual-2014'},
              2015:{'diario':'', 'mensual':'-mensual-2015', 'anual':'-anual-2015'},
              2016:{'diario':'', 'mensual':'-mensual-2016', 'anual':'-anual-2016'},
              2017:{'diario':'-diario-2017', 'mensual':'-mensual-2017', 'anual':'-anual-2017'},
              2018:{'diario':'-diario-2018', 'mensual':'-mensual-2018', 'anual':'-anual-2018'},
              2019:{'diario':'-diario-2019', 'mensual':'-mensual-2019', 'anual':'-anual-2019'},
              2020:{'diario':'-diario-2020', 'mensual':'-mensual-2020', 'anual':'-anual-2020'},
-             2021:{'diario':'-diario-2021', 'mensual':'-mensual-2021', 'anual':'-anual-2021'}}
+             2021:{'diario':'-diario-2021', 'mensual':'-mensual-2021', 'anual':'-anual-2021'},
+             2022:{'diario':'-diario-2022', 'mensual':'-mensual-2022', 'anual':'-anual-2022'},
+             2023:{'diario':'-diario-2023', 'mensual':'-mensual-2023', 'anual':'-anual-2023'}
+             }
 
 
 def get_data(topic, frq='', year1='', year2=''):
     df_return = pd.DataFrame()
     url = ''
     df = pd.DataFrame()
 
@@ -54,15 +57,15 @@
 
     # Verificamos que la periodicidad ingresada exista
     if frq not in list_frq:
         logging.debug('Error! La periodicidad {0} no existe en el servidor!'.format(frq))
         return ()
 
     # Verificamos que la periodicidad ingresada exista
-    if year1 < 1995 or year1 > 2021:
+    if year1 < 1995 or year1 > 2023:
         logging.debug('Error! El año {0} no existe en el servidor!'.format(year1))
         return ()
 
     # Corregimos la fecha superior
     if year2 == '' or year2 < year1:
         year2 = year1
 
@@ -82,24 +85,23 @@
         logging.debug('Ejercicio: {}'.format(year))
 
         # Descartamos los periodos para los cuales no existe la frecuencia en credito y armamos la url
         if files_dict[year][frq_dict[frq]] != '':
             if frq in list_frq:
                 url = read_url + topic + files_dict[year][frq_dict[frq]] + '.zip'
 
-                # Descargamos el archivo
+        # Descargamos el archivo
         try:
             logging.debug('  Intentando descargar desde {}'.format(url))
             df = pd.read_csv(url, compression='zip')
             logging.debug('  Se descargó con éxito el archivo solicitado desde {}'.format(url))
         except:
             logging.debug('  Error al intentar descargar desde {0}'.format(url))
-
         # 'Pegamos' el dataframe al acumulado (si el rango de periodos es >1)
-        df_return = df_return.append(df)
+        df_return = pd.concat([df_return,df])
 
     return (df_return)
 
 
 # Función que devuelve el contenido del directorio en el servidor.
 
 def get_docs(year='2021'):
```

### Comparing `pysupuesto-0.2.2/pysupuesto.egg-info/PKG-INFO` & `pysupuesto-0.2.3/pysupuesto.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: pysupuesto
-Version: 0.2.2
+Version: 0.2.3
 Summary: Módulo para descargar bases de diferentes ejercicios (o series temporales) del presupuesto público nacional argentino desde el Ministerio de Economía
-Home-page: UNKNOWN
+Home-page: 
 Author: @Mato
 Author-email: no@email.org
 License: MIT
 Keywords: presupuesto,budget
-Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Other Audience
 Classifier: Operating System :: POSIX :: Linux
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 
@@ -104,13 +103,14 @@
 - Mejorar el sistema de logs.
 - Intentar analizar toda la información disponible (para eso cree ``get_docs``) para expandir el modulo y poner a disposición mayor cantidad descargas.
 
 
 	
 
 
+CHANGELOG
 
-
-Version 0.2.2:
+VERSION 0.2.2:
+- Update url for downloading data from years 2019-2023
+- Change 'append' (now deprecated) package for 'concat'.
+VERSION 0.2.2:
 - Change url for downloading data from years 1995-2018
-
-
```

### Comparing `pysupuesto-0.2.2/setup.py` & `pysupuesto-0.2.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
   'Operating System :: POSIX :: Linux',
   'License :: OSI Approved :: MIT License',
   'Programming Language :: Python :: 3'
 ]
  
 setup(
   name='pysupuesto',
-  version='0.2.2',
+  version='0.2.3',
   description='Módulo para descargar bases de diferentes ejercicios (o series temporales) del presupuesto público nacional argentino desde el Ministerio de Economía',
   long_description_content_type="text/markdown",
   long_description=open('README.md').read() + '\n\n' + open('CHANGELOG.txt').read(),
   url='',  
   author='@Mato',
   author_email='no@email.org',
   license='MIT',
```

