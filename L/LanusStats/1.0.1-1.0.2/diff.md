# Comparing `tmp/LanusStats-1.0.1.tar.gz` & `tmp/LanusStats-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LanusStats-1.0.1.tar", last modified: Sun Apr  7 16:06:57 2024, max compression
+gzip compressed data, was "LanusStats-1.0.2.tar", last modified: Sun Apr  7 21:19:37 2024, max compression
```

## Comparing `LanusStats-1.0.1.tar` & `LanusStats-1.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-04-07 16:06:57.401585 LanusStats-1.0.1/
-drwxrwxrwx   0        0        0        0 2024-04-07 16:06:57.376691 LanusStats-1.0.1/LanusStats/
--rw-rw-rw-   0        0        0      222 2024-04-07 03:06:19.000000 LanusStats-1.0.1/LanusStats/__init__.py
--rw-rw-rw-   0        0        0     1759 2024-04-04 03:40:59.000000 LanusStats-1.0.1/LanusStats/exceptions.py
--rw-rw-rw-   0        0        0    14779 2024-04-07 03:01:27.000000 LanusStats-1.0.1/LanusStats/fbref.py
--rw-rw-rw-   0        0        0    11325 2024-04-07 03:01:27.000000 LanusStats-1.0.1/LanusStats/fotmob.py
--rw-rw-rw-   0        0        0    16568 2024-04-07 03:01:27.000000 LanusStats-1.0.1/LanusStats/functions.py
--rw-rw-rw-   0        0        0    19043 2024-04-04 03:40:59.000000 LanusStats-1.0.1/LanusStats/sofascore.py
--rw-rw-rw-   0        0        0     6439 2024-04-07 03:01:27.000000 LanusStats-1.0.1/LanusStats/threesixfivescores.py
--rw-rw-rw-   0        0        0     8640 2024-04-07 03:10:29.000000 LanusStats-1.0.1/LanusStats/visualizations.py
-drwxrwxrwx   0        0        0        0 2024-04-07 16:06:57.397589 LanusStats-1.0.1/LanusStats.egg-info/
--rw-rw-rw-   0        0        0     4858 2024-04-07 16:06:56.000000 LanusStats-1.0.1/LanusStats.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      386 2024-04-07 16:06:57.000000 LanusStats-1.0.1/LanusStats.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-07 16:06:56.000000 LanusStats-1.0.1/LanusStats.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2024-04-07 16:06:56.000000 LanusStats-1.0.1/LanusStats.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-07 16:06:56.000000 LanusStats-1.0.1/LanusStats.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4858 2024-04-07 16:06:57.400627 LanusStats-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     4476 2024-04-07 16:05:01.000000 LanusStats-1.0.1/README.md
--rw-rw-rw-   0        0        0       42 2024-04-07 16:06:57.401585 LanusStats-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1012 2024-04-07 16:06:24.000000 LanusStats-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-07 21:19:37.696142 LanusStats-1.0.2/
+drwxrwxrwx   0        0        0        0 2024-04-07 21:19:37.673043 LanusStats-1.0.2/LanusStats/
+-rw-rw-rw-   0        0        0      222 2024-04-07 03:06:19.000000 LanusStats-1.0.2/LanusStats/__init__.py
+-rw-rw-rw-   0        0        0     1759 2024-04-04 03:40:59.000000 LanusStats-1.0.2/LanusStats/exceptions.py
+-rw-rw-rw-   0        0        0    14779 2024-04-07 03:01:27.000000 LanusStats-1.0.2/LanusStats/fbref.py
+-rw-rw-rw-   0        0        0    11325 2024-04-07 03:01:27.000000 LanusStats-1.0.2/LanusStats/fotmob.py
+-rw-rw-rw-   0        0        0    16568 2024-04-07 03:01:27.000000 LanusStats-1.0.2/LanusStats/functions.py
+-rw-rw-rw-   0        0        0    19078 2024-04-07 21:18:09.000000 LanusStats-1.0.2/LanusStats/sofascore.py
+-rw-rw-rw-   0        0        0     6439 2024-04-07 03:01:27.000000 LanusStats-1.0.2/LanusStats/threesixfivescores.py
+-rw-rw-rw-   0        0        0     8640 2024-04-07 03:10:29.000000 LanusStats-1.0.2/LanusStats/visualizations.py
+drwxrwxrwx   0        0        0        0 2024-04-07 21:19:37.691513 LanusStats-1.0.2/LanusStats.egg-info/
+-rw-rw-rw-   0        0        0     4858 2024-04-07 21:19:37.000000 LanusStats-1.0.2/LanusStats.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      386 2024-04-07 21:19:37.000000 LanusStats-1.0.2/LanusStats.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-07 21:19:37.000000 LanusStats-1.0.2/LanusStats.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2024-04-07 21:19:37.000000 LanusStats-1.0.2/LanusStats.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-07 21:19:37.000000 LanusStats-1.0.2/LanusStats.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4858 2024-04-07 21:19:37.695137 LanusStats-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4476 2024-04-07 16:05:01.000000 LanusStats-1.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-07 21:19:37.697139 LanusStats-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1012 2024-04-07 21:18:52.000000 LanusStats-1.0.2/setup.py
```

### Comparing `LanusStats-1.0.1/LanusStats/exceptions.py` & `LanusStats-1.0.2/LanusStats/exceptions.py`

 * *Files identical despite different names*

### Comparing `LanusStats-1.0.1/LanusStats/fbref.py` & `LanusStats-1.0.2/LanusStats/fbref.py`

 * *Files identical despite different names*

### Comparing `LanusStats-1.0.1/LanusStats/fotmob.py` & `LanusStats-1.0.2/LanusStats/fotmob.py`

 * *Files identical despite different names*

### Comparing `LanusStats-1.0.1/LanusStats/functions.py` & `LanusStats-1.0.2/LanusStats/functions.py`

 * *Files identical despite different names*

### Comparing `LanusStats-1.0.1/LanusStats/sofascore.py` & `LanusStats-1.0.2/LanusStats/sofascore.py`

 * *Files 1% similar despite different names*

```diff
@@ -256,28 +256,28 @@
             if page == pages:
                 print('End of the pages')
                 break
             offset += 100
 
         return df
 
-    def match_momentum(self, match_url):
+    def match_momentum(self, match_url, colors = ['red', 'green']):
         """Get the match momentum plot
         Args:
             match_url (str): Full link to a SofaScore match
         Returns:
             fig, ax: Plot of match momentum and fig/axes for further customization
         """
         headers = self.requests_headers
         match_id = self.get_match_id(match_url)
         graph_url = f'https://api.sofascore.com/api/v1/event/{match_id}/graph'
         response = requests.get(graph_url, headers=headers)
         match_momentum_df = pd.DataFrame(response.json()['graphPoints'])
 
-        fig, ax = self.match_momentum_plot(match_momentum_df, match_id)
+        fig, ax = self.match_momentum_plot(match_momentum_df, match_id, colors)
 
         return fig, ax
 
     def get_general_match_stats(self, match_url):
         """Get general match statistics (possession, passes, duels) by teams.
         Args:
             match_url (str): Full link to a SofaScore match
```

### Comparing `LanusStats-1.0.1/LanusStats/threesixfivescores.py` & `LanusStats-1.0.2/LanusStats/threesixfivescores.py`

 * *Files identical despite different names*

### Comparing `LanusStats-1.0.1/LanusStats/visualizations.py` & `LanusStats-1.0.2/LanusStats/visualizations.py`

 * *Files identical despite different names*

### Comparing `LanusStats-1.0.1/LanusStats.egg-info/PKG-INFO` & `LanusStats-1.0.2/LanusStats.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LanusStats
-Version: 1.0.1
+Version: 1.0.2
 Summary: Python library for scraping football data and visualize it / Libreria de Python para scrapear data de fútbol y visualizarla
 Home-page: https://github.com/federicorabanos
 Author: Federico Rábanos
 Author-email: lanusstats@gmail.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `LanusStats-1.0.1/PKG-INFO` & `LanusStats-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LanusStats
-Version: 1.0.1
+Version: 1.0.2
 Summary: Python library for scraping football data and visualize it / Libreria de Python para scrapear data de fútbol y visualizarla
 Home-page: https://github.com/federicorabanos
 Author: Federico Rábanos
 Author-email: lanusstats@gmail.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `LanusStats-1.0.1/README.md` & `LanusStats-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `LanusStats-1.0.1/setup.py` & `LanusStats-1.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pathlib
 from setuptools import find_packages, setup
 
 HERE = pathlib.Path(__file__).parent
 
-VERSION = '1.0.1'
+VERSION = '1.0.2'
 PACKAGE_NAME = 'LanusStats'
 AUTHOR = 'Federico Rábanos'
 AUTHOR_EMAIL = 'lanusstats@gmail.com'
 URL = 'https://github.com/federicorabanos'
 
 LICENSE = 'MIT'
 DESCRIPTION = 'Python library for scraping football data and visualize it / Libreria de Python para scrapear data de fútbol y visualizarla'
```

