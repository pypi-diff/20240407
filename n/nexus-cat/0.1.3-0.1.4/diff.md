# Comparing `tmp/nexus-cat-0.1.3.tar.gz` & `tmp/nexus-cat-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nexus-cat-0.1.3.tar", last modified: Sat Apr  6 22:27:32 2024, max compression
+gzip compressed data, was "nexus-cat-0.1.4.tar", last modified: Sun Apr  7 15:57:18 2024, max compression
```

## Comparing `nexus-cat-0.1.3.tar` & `nexus-cat-0.1.4.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxr-x   0 perraju   (1000) perraju   (1000)        0 2024-04-06 22:27:32.568428 nexus-cat-0.1.3/
--rw-rw-r--   0 perraju   (1000) perraju   (1000)     1076 2024-04-06 13:06:16.000000 nexus-cat-0.1.3/LICENSE
--rw-r--r--   0 perraju   (1000) perraju   (1000)      646 2024-04-06 22:27:32.568428 nexus-cat-0.1.3/PKG-INFO
--rw-rw-r--   0 perraju   (1000) perraju   (1000)     1613 2024-04-06 22:00:41.000000 nexus-cat-0.1.3/README.md
-drwxrwxr-x   0 perraju   (1000) perraju   (1000)        0 2024-04-06 22:27:32.564428 nexus-cat-0.1.3/nexus/
--rw-rw-r--   0 perraju   (1000) perraju   (1000)      175 2024-04-06 22:27:10.000000 nexus-cat-0.1.3/nexus/__init__.py
-drwxrwxr-x   0 perraju   (1000) perraju   (1000)        0 2024-04-06 22:27:32.564428 nexus-cat-0.1.3/nexus/core/
--rw-rw-r--   0 perraju   (1000) perraju   (1000)      145 2024-04-06 20:39:23.000000 nexus-cat-0.1.3/nexus/core/__init__.py
--rw-rw-r--   0 perraju   (1000) perraju   (1000)     8816 2024-04-06 21:10:52.000000 nexus-cat-0.1.3/nexus/core/atom.py
--rw-rw-r--   0 perraju   (1000) perraju   (1000)     2616 2024-03-31 10:20:59.000000 nexus-cat-0.1.3/nexus/core/box.py
--rw-rw-r--   0 perraju   (1000) perraju   (1000)    14213 2024-04-06 20:40:34.000000 nexus-cat-0.1.3/nexus/core/cluster.py
--rw-rw-r--   0 perraju   (1000) perraju   (1000)     2141 2024-03-31 11:54:45.000000 nexus-cat-0.1.3/nexus/core/cutoff.py
--rw-rw-r--   0 perraju   (1000) perraju   (1000)    30889 2024-04-06 21:49:13.000000 nexus-cat-0.1.3/nexus/core/system.py
-drwxrwxr-x   0 perraju   (1000) perraju   (1000)        0 2024-04-06 22:27:32.564428 nexus-cat-0.1.3/nexus/data/
--rw-rw-r--   0 perraju   (1000) perraju   (1000)     7530 2024-03-31 11:07:05.000000 nexus-cat-0.1.3/nexus/data/__init__.py
-drwxrwxr-x   0 perraju   (1000) perraju   (1000)        0 2024-04-06 22:27:32.564428 nexus-cat-0.1.3/nexus/extensions/
--rw-rw-r--   0 perraju   (1000) perraju   (1000)     2021 2024-04-06 20:41:19.000000 nexus-cat-0.1.3/nexus/extensions/Na.py
--rw-rw-r--   0 perraju   (1000) perraju   (1000)    14516 2024-04-06 21:08:33.000000 nexus-cat-0.1.3/nexus/extensions/SiOz.py
--rw-rw-r--   0 perraju   (1000) perraju   (1000)       35 2024-04-06 21:21:46.000000 nexus-cat-0.1.3/nexus/extensions/__init__.py
-drwxrwxr-x   0 perraju   (1000) perraju   (1000)        0 2024-04-06 22:27:32.568428 nexus-cat-0.1.3/nexus/io/
--rw-rw-r--   0 perraju   (1000) perraju   (1000)      612 2024-04-06 20:42:58.000000 nexus-cat-0.1.3/nexus/io/__init__.py
--rw-rw-r--   0 perraju   (1000) perraju   (1000)      707 2024-04-05 12:20:44.000000 nexus-cat-0.1.3/nexus/io/make_lines_unique.py
--rw-rw-r--   0 perraju   (1000) perraju   (1000)     4761 2024-04-06 22:23:48.000000 nexus-cat-0.1.3/nexus/io/read_and_create_system.py
--rw-rw-r--   0 perraju   (1000) perraju   (1000)     1032 2024-03-31 11:09:48.000000 nexus-cat-0.1.3/nexus/io/read_lattices_properties.py
--rw-rw-r--   0 perraju   (1000) perraju   (1000)      662 2024-03-31 11:10:34.000000 nexus-cat-0.1.3/nexus/io/read_number_of_configurations.py
--rw-rw-r--   0 perraju   (1000) perraju   (1000)    29013 2024-04-06 20:42:35.000000 nexus-cat-0.1.3/nexus/io/result.py
--rw-rw-r--   0 perraju   (1000) perraju   (1000)      722 2024-04-05 17:39:46.000000 nexus-cat-0.1.3/nexus/io/write_list_of_files.py
--rw-rw-r--   0 perraju   (1000) perraju   (1000)    13679 2024-04-06 21:50:04.000000 nexus-cat-0.1.3/nexus/main.py
-drwxrwxr-x   0 perraju   (1000) perraju   (1000)        0 2024-04-06 22:27:32.568428 nexus-cat-0.1.3/nexus/settings/
--rw-rw-r--   0 perraju   (1000) perraju   (1000)       30 2024-04-06 20:43:10.000000 nexus-cat-0.1.3/nexus/settings/__init__.py
--rw-rw-r--   0 perraju   (1000) perraju   (1000)     5787 2024-04-05 17:06:57.000000 nexus-cat-0.1.3/nexus/settings/parameter.py
--rw-rw-r--   0 perraju   (1000) perraju   (1000)     9113 2024-04-06 21:49:55.000000 nexus-cat-0.1.3/nexus/settings/settings.py
-drwxrwxr-x   0 perraju   (1000) perraju   (1000)        0 2024-04-06 22:27:32.568428 nexus-cat-0.1.3/nexus/utils/
--rw-rw-r--   0 perraju   (1000) perraju   (1000)       97 2024-04-06 20:43:29.000000 nexus-cat-0.1.3/nexus/utils/__init__.py
--rw-rw-r--   0 perraju   (1000) perraju   (1000)     1150 2024-03-31 12:26:32.000000 nexus-cat-0.1.3/nexus/utils/generate_color_gradient.py
--rw-rw-r--   0 perraju   (1000) perraju   (1000)      927 2024-04-06 22:08:51.000000 nexus-cat-0.1.3/nexus/utils/print_title.py
-drwxrwxr-x   0 perraju   (1000) perraju   (1000)        0 2024-04-06 22:27:32.568428 nexus-cat-0.1.3/nexus_cat.egg-info/
--rw-r--r--   0 perraju   (1000) perraju   (1000)      646 2024-04-06 22:27:32.000000 nexus-cat-0.1.3/nexus_cat.egg-info/PKG-INFO
--rw-rw-r--   0 perraju   (1000) perraju   (1000)      834 2024-04-06 22:27:32.000000 nexus-cat-0.1.3/nexus_cat.egg-info/SOURCES.txt
--rw-rw-r--   0 perraju   (1000) perraju   (1000)        1 2024-04-06 22:27:32.000000 nexus-cat-0.1.3/nexus_cat.egg-info/dependency_links.txt
--rw-rw-r--   0 perraju   (1000) perraju   (1000)       25 2024-04-06 22:27:32.000000 nexus-cat-0.1.3/nexus_cat.egg-info/requires.txt
--rw-rw-r--   0 perraju   (1000) perraju   (1000)        6 2024-04-06 22:27:32.000000 nexus-cat-0.1.3/nexus_cat.egg-info/top_level.txt
--rw-rw-r--   0 perraju   (1000) perraju   (1000)       38 2024-04-06 22:27:32.568428 nexus-cat-0.1.3/setup.cfg
--rw-rw-r--   0 perraju   (1000) perraju   (1000)      751 2024-04-06 22:27:04.000000 nexus-cat-0.1.3/setup.py
+drwxrwxr-x   0 perraju   (1000) perraju   (1000)        0 2024-04-07 15:57:18.593455 nexus-cat-0.1.4/
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)     1076 2024-04-06 13:06:16.000000 nexus-cat-0.1.4/LICENSE
+-rw-r--r--   0 perraju   (1000) perraju   (1000)      646 2024-04-07 15:57:18.593455 nexus-cat-0.1.4/PKG-INFO
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)     1620 2024-04-06 22:29:20.000000 nexus-cat-0.1.4/README.md
+drwxrwxr-x   0 perraju   (1000) perraju   (1000)        0 2024-04-07 15:57:18.589455 nexus-cat-0.1.4/nexus/
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)      175 2024-04-06 22:27:10.000000 nexus-cat-0.1.4/nexus/__init__.py
+drwxrwxr-x   0 perraju   (1000) perraju   (1000)        0 2024-04-07 15:57:18.589455 nexus-cat-0.1.4/nexus/core/
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)      145 2024-04-06 20:39:23.000000 nexus-cat-0.1.4/nexus/core/__init__.py
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)     8816 2024-04-06 21:10:52.000000 nexus-cat-0.1.4/nexus/core/atom.py
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)     2616 2024-03-31 10:20:59.000000 nexus-cat-0.1.4/nexus/core/box.py
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)    14174 2024-04-07 12:47:37.000000 nexus-cat-0.1.4/nexus/core/cluster.py
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)     2141 2024-03-31 11:54:45.000000 nexus-cat-0.1.4/nexus/core/cutoff.py
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)    30774 2024-04-07 14:28:12.000000 nexus-cat-0.1.4/nexus/core/system.py
+drwxrwxr-x   0 perraju   (1000) perraju   (1000)        0 2024-04-07 15:57:18.589455 nexus-cat-0.1.4/nexus/data/
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)     7530 2024-03-31 11:07:05.000000 nexus-cat-0.1.4/nexus/data/__init__.py
+drwxrwxr-x   0 perraju   (1000) perraju   (1000)        0 2024-04-07 15:57:18.589455 nexus-cat-0.1.4/nexus/extensions/
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)     2021 2024-04-06 20:41:19.000000 nexus-cat-0.1.4/nexus/extensions/Na.py
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)    14478 2024-04-07 15:13:15.000000 nexus-cat-0.1.4/nexus/extensions/SiOz.py
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)       35 2024-04-06 21:21:46.000000 nexus-cat-0.1.4/nexus/extensions/__init__.py
+drwxrwxr-x   0 perraju   (1000) perraju   (1000)        0 2024-04-07 15:57:18.589455 nexus-cat-0.1.4/nexus/io/
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)      612 2024-04-06 20:42:58.000000 nexus-cat-0.1.4/nexus/io/__init__.py
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)      707 2024-04-05 12:20:44.000000 nexus-cat-0.1.4/nexus/io/make_lines_unique.py
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)     4761 2024-04-06 22:23:48.000000 nexus-cat-0.1.4/nexus/io/read_and_create_system.py
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)     1032 2024-03-31 11:09:48.000000 nexus-cat-0.1.4/nexus/io/read_lattices_properties.py
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)      662 2024-03-31 11:10:34.000000 nexus-cat-0.1.4/nexus/io/read_number_of_configurations.py
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)    28785 2024-04-07 13:55:57.000000 nexus-cat-0.1.4/nexus/io/result.py
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)      722 2024-04-05 17:39:46.000000 nexus-cat-0.1.4/nexus/io/write_list_of_files.py
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)    13679 2024-04-06 21:50:04.000000 nexus-cat-0.1.4/nexus/main.py
+drwxrwxr-x   0 perraju   (1000) perraju   (1000)        0 2024-04-07 15:57:18.589455 nexus-cat-0.1.4/nexus/settings/
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)       30 2024-04-06 20:43:10.000000 nexus-cat-0.1.4/nexus/settings/__init__.py
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)     5787 2024-04-05 17:06:57.000000 nexus-cat-0.1.4/nexus/settings/parameter.py
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)     9113 2024-04-06 21:49:55.000000 nexus-cat-0.1.4/nexus/settings/settings.py
+drwxrwxr-x   0 perraju   (1000) perraju   (1000)        0 2024-04-07 15:57:18.593455 nexus-cat-0.1.4/nexus/utils/
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)       97 2024-04-06 20:43:29.000000 nexus-cat-0.1.4/nexus/utils/__init__.py
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)     1150 2024-03-31 12:26:32.000000 nexus-cat-0.1.4/nexus/utils/generate_color_gradient.py
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)      927 2024-04-06 22:08:51.000000 nexus-cat-0.1.4/nexus/utils/print_title.py
+drwxrwxr-x   0 perraju   (1000) perraju   (1000)        0 2024-04-07 15:57:18.593455 nexus-cat-0.1.4/nexus_cat.egg-info/
+-rw-r--r--   0 perraju   (1000) perraju   (1000)      646 2024-04-07 15:57:18.000000 nexus-cat-0.1.4/nexus_cat.egg-info/PKG-INFO
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)      834 2024-04-07 15:57:18.000000 nexus-cat-0.1.4/nexus_cat.egg-info/SOURCES.txt
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)        1 2024-04-07 15:57:18.000000 nexus-cat-0.1.4/nexus_cat.egg-info/dependency_links.txt
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)       25 2024-04-07 15:57:18.000000 nexus-cat-0.1.4/nexus_cat.egg-info/requires.txt
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)        6 2024-04-07 15:57:18.000000 nexus-cat-0.1.4/nexus_cat.egg-info/top_level.txt
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)       38 2024-04-07 15:57:18.593455 nexus-cat-0.1.4/setup.cfg
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)      801 2024-04-07 15:57:13.000000 nexus-cat-0.1.4/setup.py
```

### Comparing `nexus-cat-0.1.3/LICENSE` & `nexus-cat-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nexus-cat-0.1.3/PKG-INFO` & `nexus-cat-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nexus-cat
-Version: 0.1.3
+Version: 0.1.4
 Summary: Nexus is a Cluster Analysing Toolkit package for atomic systems.
 Home-page: https://github.com/JulienPerradin/nexus
 Author: Julien Perradin
 Author-email: julien.perradin@umontpellier.fr
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `nexus-cat-0.1.3/README.md` & `nexus-cat-0.1.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 ```bash
 git clone git@github.com:JulienPerradin/nexus.git
 ```
 Then you can use pip, it will install dependencies and the main package in your Python environment:
 
 ```bash
-pip install nexus-cat
+pip install nexus-cat==0.1.3
 ```
 
 
 ## Usage
 
 As a first example you can run the script `launch-nexus-quick-test.py`:
```

### Comparing `nexus-cat-0.1.3/nexus/core/atom.py` & `nexus-cat-0.1.4/nexus/core/atom.py`

 * *Files identical despite different names*

### Comparing `nexus-cat-0.1.3/nexus/core/box.py` & `nexus-cat-0.1.4/nexus/core/box.py`

 * *Files identical despite different names*

### Comparing `nexus-cat-0.1.3/nexus/core/cluster.py` & `nexus-cat-0.1.4/nexus/core/cluster.py`

 * *Files 0% similar despite different names*

```diff
@@ -161,16 +161,14 @@
         for i in range(self.unwrapped_positions.shape[0]):
             squared_rij = np.linalg.norm(self.unwrapped_positions[i, :] - self.unwrapped_positions[:, :], axis=1)** 2
             self.gyration_radius += np.sum(squared_rij)
         
         # Normalize the sum by 0.5 s²
         self.gyration_radius = np.sqrt((0.5 / (self.size**2)) * self.gyration_radius) 
         
-        DEBUG = False
-                
     def calculate_percolation_probability(self) -> None:
         r"""
         Calculate the percolation probability of the cluster.
         
         Returns:
         --------
             - None.
```

### Comparing `nexus-cat-0.1.3/nexus/core/cutoff.py` & `nexus-cat-0.1.4/nexus/core/cutoff.py`

 * *Files identical despite different names*

### Comparing `nexus-cat-0.1.3/nexus/core/system.py` & `nexus-cat-0.1.4/nexus/core/system.py`

 * *Files 1% similar despite different names*

```diff
@@ -324,16 +324,14 @@
         module = importlib.import_module(f"nexus.extensions.{extension}")
         
         self.structural_units = module.calculate_structural_units(self.get_atoms())
     
     
     #____________CLUSTERS METHODS____________
     
-    # TODO reorganize the getters, optimize the code #PRIO1
-    
     def get_all_clusters(self, connectivity:str) -> list:
         r"""
         Return the list of all Cluster objects associated with the given connectivity.
         
         Parameters:
         -----------
             - connectivity (str) : Connectivity of the cluster.
@@ -470,15 +468,15 @@
         cluster = [cluster for cluster in self.clusters if (cluster.connectivity == connectivity) and (len(cluster.percolation_probability) > 0)]
         
         if len(cluster) == 0:
             # No percolating cluster
             return [0.0] * 3
         if len(cluster) > 1:
             # More than one percolating cluster
-            print(f"\tWARNING: More than one percolating cluster found for the connectivity {connectivity}. Taking the biggest one.")
+            # print(f"\tWARNING: More than one percolating cluster found for the connectivity {connectivity}. Taking the biggest one.")
             
             # get the biggest cluster
             cluster = max(cluster, key=lambda x: x.size)
             
             order_parameter = cluster.order_parameter
             
         else:
@@ -501,15 +499,15 @@
         cluster = [cluster for cluster in self.clusters if (cluster.connectivity == connectivity) and (len(cluster.percolation_probability) > 0)]
         
         if len(cluster) == 0:
             # No percolating cluster
             return [0.0] * 3
         if len(cluster) > 1:
             # More than one percolating cluster
-            print(f"\tWARNING: More than one percolating cluster found for the connectivity {connectivity}. Taking the biggest one.")
+            # print(f"\tWARNING: More than one percolating cluster found for the connectivity {connectivity}. Taking the biggest one.")
             
             # get the biggest cluster
             cluster = max(cluster, key=lambda x: x.size)
             
             percolation_probability = cluster.percolation_probability
             if len(percolation_probability) == 1:
                 percolation_probability = [1.0, 0.0, 0.0]
@@ -651,15 +649,14 @@
         
         # Load cluster properties to analyse
         cluster_settings = self.settings.cluster_settings.get_value()
         criteria = cluster_settings['criteria']
         
         list_of_elements, z1, z2 = self.decrypt_connectivity(connectivity)
         
-        # Error management #TODO enhanced this #PRIO3
         if criteria != "distance" and criteria != "bond":
             raise ValueError(f"\tERROR: Criteria '{criteria}' is not supported. Please select 'bond' or 'distance'.")
         for e in list_of_elements:
             if e not in cluster_settings['connectivity']:
                 raise ValueError(f"\tERROR: Something wrong in the connectivity in cluster settings.")
```

### Comparing `nexus-cat-0.1.3/nexus/data/__init__.py` & `nexus-cat-0.1.4/nexus/data/__init__.py`

 * *Files identical despite different names*

### Comparing `nexus-cat-0.1.3/nexus/extensions/Na.py` & `nexus-cat-0.1.4/nexus/extensions/Na.py`

 * *Files identical despite different names*

### Comparing `nexus-cat-0.1.3/nexus/extensions/SiOz.py` & `nexus-cat-0.1.4/nexus/extensions/SiOz.py`

 * *Files 1% similar despite different names*

```diff
@@ -159,15 +159,15 @@
     Calculate the following properties.
     
     Returns:
     --------
         - SiO4      : list of SiO4 tetrahedra
         - SiO5      : list of SiO5 pentahedra
         - SiO6      : list of SiO6 octahedra
-        - SiO7      : list of SiO7 eptahedra #PRIO3 check if "eptahedra" exists
+        - SiO7      : list of SiO7 eptahedra 
         - OSi1      : list of OSi1
         - OSi2      : list of OSi2
         - OSi3      : list of OSi3
         - OSi4      : list of OSi4
         - ES_SiO6   : proportion of edge-sharing in SiO6 units
     """
     
@@ -195,15 +195,15 @@
         if counter == 5:
             SiO5.append(atom)
         if counter == 6:
             SiO6.append(atom)
         if counter == 7:
             SiO7.append(atom)
     
-    _debug_histogram_proportion_SiOz = np.histogram(coordination_SiOz, bins=[4,5,6,7,8], density=True) #DEBUG
+    _debug_histogram_proportion_SiOz = np.histogram(coordination_SiOz, bins=[4,5,6,7,8], density=True) 
     
     # Calculate the proportion of each OSiz units
     coordination_OSiz = []
     for atom in oxygens:
         counter = len([neighbour for neighbour in atom.get_neighbours() if neighbour.get_element() == "Si"])
         coordination_OSiz.append(counter)
         if counter == 1:
@@ -211,15 +211,15 @@
         if counter == 2:
             OSi2.append(atom)
         if counter == 3:
             OSi3.append(atom)
         if counter == 4:
             OSi4.append(atom)
             
-    _debug_histogram_proportion_OSik = np.histogram(coordination_OSiz, bins=[1,2,3,4,5], density=True) #DEBUG
+    _debug_histogram_proportion_OSik = np.histogram(coordination_OSiz, bins=[1,2,3,4,5], density=True) 
     
     # Calculate the number of edge-sharing (2 oxygens shared by 2 silicons)
     for silicon in silicons:
         unique_bond = []
         for oxygen in [atom for atom in silicon.get_neighbours() if atom.get_element() == 'O']:
             for second_silicon in [atom for atom in oxygen.get_neighbours() if atom.get_element() == 'Si']:
                 if second_silicon.id != silicon.id:
@@ -346,15 +346,15 @@
                     and atom.number_of_edges == 2 and neighbour.number_of_edges == 2):
                     union(neighbour, atom)
         
         if criteria == 'bond':
             for neighbour in atom.neighbours:
                 if neighbour.element == bridge:
                     for second_neighbour in neighbour.neighbours:
-                        if (atom.element == node_1 and second_neighbour == node_2
+                        if (atom.element == node_1 and second_neighbour.element == node_2
                             and atom.coordination == 6 and second_neighbour.coordination == 6
                             and atom.number_of_edges == 2 and second_neighbour.number_of_edges == 2): 
                             union(neighbour, atom)
         
     clusters_found = {}
     local_clusters = []
```

### Comparing `nexus-cat-0.1.3/nexus/io/__init__.py` & `nexus-cat-0.1.4/nexus/io/__init__.py`

 * *Files identical despite different names*

### Comparing `nexus-cat-0.1.3/nexus/io/make_lines_unique.py` & `nexus-cat-0.1.4/nexus/io/make_lines_unique.py`

 * *Files identical despite different names*

### Comparing `nexus-cat-0.1.3/nexus/io/read_and_create_system.py` & `nexus-cat-0.1.4/nexus/io/read_and_create_system.py`

 * *Files identical despite different names*

### Comparing `nexus-cat-0.1.3/nexus/io/read_lattices_properties.py` & `nexus-cat-0.1.4/nexus/io/read_lattices_properties.py`

 * *Files identical despite different names*

### Comparing `nexus-cat-0.1.3/nexus/io/read_number_of_configurations.py` & `nexus-cat-0.1.4/nexus/io/read_number_of_configurations.py`

 * *Files identical despite different names*

### Comparing `nexus-cat-0.1.3/nexus/io/result.py` & `nexus-cat-0.1.4/nexus/io/result.py`

 * *Files 1% similar despite different names*

```diff
@@ -519,17 +519,14 @@
         
         Mathematically, the correlation length is defined as:
         $\(\xi = \sqrt{\frac{2 \sum_{i=1}^{N} r_{i}^{2} s_{i}^{2}}{\sum_{i=1}^{N} s_{i}^{2}}}$\) where:
             - \(r_{i}\) is the radius of the cluster \(i\),
             - \(s_{i}\) is the size of the cluster \(i\),
             - \(N\) is the number of clusters.
         
-        
-        TODO : find out why there's a difference between the results obtained with the current implementation and the one in the original code.
-               The results are different at the low decimal places. #PRIO1
         """
 
         lists_r_s = {}
         lists_s_ns = {}
         correlation_lengths = {}
         numerators = {}
```

### Comparing `nexus-cat-0.1.3/nexus/io/write_list_of_files.py` & `nexus-cat-0.1.4/nexus/io/write_list_of_files.py`

 * *Files identical despite different names*

### Comparing `nexus-cat-0.1.3/nexus/main.py` & `nexus-cat-0.1.4/nexus/main.py`

 * *Files identical despite different names*

### Comparing `nexus-cat-0.1.3/nexus/settings/parameter.py` & `nexus-cat-0.1.4/nexus/settings/parameter.py`

 * *Files identical despite different names*

### Comparing `nexus-cat-0.1.3/nexus/settings/settings.py` & `nexus-cat-0.1.4/nexus/settings/settings.py`

 * *Files identical despite different names*

### Comparing `nexus-cat-0.1.3/nexus/utils/generate_color_gradient.py` & `nexus-cat-0.1.4/nexus/utils/generate_color_gradient.py`

 * *Files identical despite different names*

### Comparing `nexus-cat-0.1.3/nexus/utils/print_title.py` & `nexus-cat-0.1.4/nexus/utils/print_title.py`

 * *Files identical despite different names*

### Comparing `nexus-cat-0.1.3/nexus_cat.egg-info/PKG-INFO` & `nexus-cat-0.1.4/nexus_cat.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nexus-cat
-Version: 0.1.3
+Version: 0.1.4
 Summary: Nexus is a Cluster Analysing Toolkit package for atomic systems.
 Home-page: https://github.com/JulienPerradin/nexus
 Author: Julien Perradin
 Author-email: julien.perradin@umontpellier.fr
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `nexus-cat-0.1.3/nexus_cat.egg-info/SOURCES.txt` & `nexus-cat-0.1.4/nexus_cat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nexus-cat-0.1.3/setup.py` & `nexus-cat-0.1.4/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='nexus-cat',
-    version='0.1.3',
+    version='0.1.4',
     description='Nexus is a Cluster Analysing Toolkit package for atomic systems.',
     author='Julien Perradin',
     author_email='julien.perradin@umontpellier.fr',
     url='https://github.com/JulienPerradin/nexus',
     packages=find_packages(),
     install_requires=[
         'numpy',
@@ -18,8 +18,9 @@
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
     ],
+    project_description=open('README.md').read(),
 )
```

