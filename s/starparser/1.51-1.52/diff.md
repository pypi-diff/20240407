# Comparing `tmp/starparser-1.51.tar.gz` & `tmp/starparser-1.52.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starparser-1.51.tar", last modified: Sat Jan 27 12:34:50 2024, max compression
+gzip compressed data, was "starparser-1.52.tar", last modified: Sun Apr  7 13:19:20 2024, max compression
```

## Comparing `starparser-1.51.tar` & `starparser-1.52.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 chaaban    (501) staff       (20)        0 2024-01-27 12:34:50.348348 starparser-1.51/
--rw-r--r--   0 chaaban    (501) staff       (20)     1069 2023-06-05 21:07:33.000000 starparser-1.51/LICENSE.txt
--rw-r--r--   0 chaaban    (501) staff       (20)    36626 2024-01-27 12:34:50.348221 starparser-1.51/PKG-INFO
--rw-r--r--   0 chaaban    (501) staff       (20)    36323 2024-01-27 11:34:22.000000 starparser-1.51/README.md
--rw-r--r--   0 chaaban    (501) staff       (20)       38 2024-01-27 12:34:50.348390 starparser-1.51/setup.cfg
--rw-r--r--   0 chaaban    (501) staff       (20)      880 2023-08-26 16:02:58.000000 starparser-1.51/setup.py
-drwxr-xr-x   0 chaaban    (501) staff       (20)        0 2024-01-27 12:34:50.347252 starparser-1.51/starparser/
--rw-r--r--   0 chaaban    (501) staff       (20)       82 2024-01-27 12:33:46.000000 starparser-1.51/starparser/__init__.py
--rw-r--r--   0 chaaban    (501) staff       (20)      119 2023-08-11 15:52:04.000000 starparser-1.51/starparser/__main__.py
--rw-r--r--   0 chaaban    (501) staff       (20)    20302 2023-09-18 14:49:41.000000 starparser-1.51/starparser/argparser.py
--rw-r--r--   0 chaaban    (501) staff       (20)     9351 2024-01-27 11:30:44.000000 starparser-1.51/starparser/columnplay.py
--rw-r--r--   0 chaaban    (501) staff       (20)    51371 2024-01-27 12:32:26.000000 starparser-1.51/starparser/decisiontree.py
--rw-r--r--   0 chaaban    (501) staff       (20)    10273 2023-08-27 08:10:34.000000 starparser-1.51/starparser/fileparser.py
--rw-r--r--   0 chaaban    (501) staff       (20)    21697 2024-01-27 12:30:22.000000 starparser-1.51/starparser/particleplay.py
--rw-r--r--   0 chaaban    (501) staff       (20)    26805 2023-09-02 00:09:18.000000 starparser-1.51/starparser/plots.py
--rw-r--r--   0 chaaban    (501) staff       (20)    13056 2023-08-26 18:27:37.000000 starparser-1.51/starparser/specialparticles.py
--rw-r--r--   0 chaaban    (501) staff       (20)     1890 2023-08-11 15:52:04.000000 starparser-1.51/starparser/splits.py
-drwxr-xr-x   0 chaaban    (501) staff       (20)        0 2024-01-27 12:34:50.348059 starparser-1.51/starparser.egg-info/
--rw-r--r--   0 chaaban    (501) staff       (20)    36626 2024-01-27 12:34:50.000000 starparser-1.51/starparser.egg-info/PKG-INFO
--rw-r--r--   0 chaaban    (501) staff       (20)      482 2024-01-27 12:34:50.000000 starparser-1.51/starparser.egg-info/SOURCES.txt
--rw-r--r--   0 chaaban    (501) staff       (20)        1 2024-01-27 12:34:50.000000 starparser-1.51/starparser.egg-info/dependency_links.txt
--rw-r--r--   0 chaaban    (501) staff       (20)       56 2024-01-27 12:34:50.000000 starparser-1.51/starparser.egg-info/entry_points.txt
--rw-r--r--   0 chaaban    (501) staff       (20)       30 2024-01-27 12:34:50.000000 starparser-1.51/starparser.egg-info/requires.txt
--rw-r--r--   0 chaaban    (501) staff       (20)       11 2024-01-27 12:34:50.000000 starparser-1.51/starparser.egg-info/top_level.txt
+drwxr-xr-x   0 chaaban    (501) staff       (20)        0 2024-04-07 13:19:20.201904 starparser-1.52/
+-rw-r--r--   0 chaaban    (501) staff       (20)     1069 2023-06-05 21:07:33.000000 starparser-1.52/LICENSE.txt
+-rw-r--r--   0 chaaban    (501) staff       (20)    36955 2024-04-07 13:19:20.201774 starparser-1.52/PKG-INFO
+-rw-r--r--   0 chaaban    (501) staff       (20)    36652 2024-04-07 12:48:53.000000 starparser-1.52/README.md
+-rw-r--r--   0 chaaban    (501) staff       (20)       38 2024-04-07 13:19:20.201961 starparser-1.52/setup.cfg
+-rw-r--r--   0 chaaban    (501) staff       (20)      880 2023-08-26 16:02:58.000000 starparser-1.52/setup.py
+drwxr-xr-x   0 chaaban    (501) staff       (20)        0 2024-04-07 13:19:20.200818 starparser-1.52/starparser/
+-rw-r--r--   0 chaaban    (501) staff       (20)       82 2024-04-07 12:47:08.000000 starparser-1.52/starparser/__init__.py
+-rw-r--r--   0 chaaban    (501) staff       (20)      119 2023-08-11 15:52:04.000000 starparser-1.52/starparser/__main__.py
+-rw-r--r--   0 chaaban    (501) staff       (20)    20433 2024-04-07 12:48:12.000000 starparser-1.52/starparser/argparser.py
+-rw-r--r--   0 chaaban    (501) staff       (20)     9351 2024-01-27 11:30:44.000000 starparser-1.52/starparser/columnplay.py
+-rw-r--r--   0 chaaban    (501) staff       (20)    52470 2024-04-07 12:48:26.000000 starparser-1.52/starparser/decisiontree.py
+-rw-r--r--   0 chaaban    (501) staff       (20)    10557 2024-04-07 12:37:09.000000 starparser-1.52/starparser/fileparser.py
+-rw-r--r--   0 chaaban    (501) staff       (20)    21935 2024-04-07 12:48:19.000000 starparser-1.52/starparser/particleplay.py
+-rw-r--r--   0 chaaban    (501) staff       (20)    26805 2023-09-02 00:09:18.000000 starparser-1.52/starparser/plots.py
+-rw-r--r--   0 chaaban    (501) staff       (20)    13056 2023-08-26 18:27:37.000000 starparser-1.52/starparser/specialparticles.py
+-rw-r--r--   0 chaaban    (501) staff       (20)     1890 2023-08-11 15:52:04.000000 starparser-1.52/starparser/splits.py
+drwxr-xr-x   0 chaaban    (501) staff       (20)        0 2024-04-07 13:19:20.201585 starparser-1.52/starparser.egg-info/
+-rw-r--r--   0 chaaban    (501) staff       (20)    36955 2024-04-07 13:19:20.000000 starparser-1.52/starparser.egg-info/PKG-INFO
+-rw-r--r--   0 chaaban    (501) staff       (20)      482 2024-04-07 13:19:20.000000 starparser-1.52/starparser.egg-info/SOURCES.txt
+-rw-r--r--   0 chaaban    (501) staff       (20)        1 2024-04-07 13:19:20.000000 starparser-1.52/starparser.egg-info/dependency_links.txt
+-rw-r--r--   0 chaaban    (501) staff       (20)       56 2024-04-07 13:19:20.000000 starparser-1.52/starparser.egg-info/entry_points.txt
+-rw-r--r--   0 chaaban    (501) staff       (20)       30 2024-04-07 13:19:20.000000 starparser-1.52/starparser.egg-info/requires.txt
+-rw-r--r--   0 chaaban    (501) staff       (20)       11 2024-04-07 13:19:20.000000 starparser-1.52/starparser.egg-info/top_level.txt
```

### Comparing `starparser-1.51/LICENSE.txt` & `starparser-1.52/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `starparser-1.51/PKG-INFO` & `starparser-1.52/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: starparser
-Version: 1.51
-Summary: Manipulate and mine Relion star files.
-Home-page: http://pypi.python.org/pypi/starparser/
-Author: Sami Chaaban
-Author-email: chaaban@mrc-lmb.cam.ac.uk
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
 # starparser
 
 Use this package to manipulate Relion star files, including counting, modifying, plotting, and sifting the data. At the very least, this is a useful alternative to *awk* commands, which can get *awk*ward. Below is a description of the command-line options with some examples. Alternatively, use starparser within Relion or load the modules in your own Python scripts.
 
 Some of the options below are already available in Relion with "relion_star_handler".
 
 1. [Installation](#installation)
@@ -49,15 +38,15 @@
 ```
 starparser --i particles.star --list_column OriginX
 ```
 
 For some options, a second star file can also be passed as input ```--f secondfile.star```.
 
 ```
-starparser --i particles1.star --f particles2.star --find_shared MicrographName
+starparser --i particles1.star --find_shared MicrographName --f particles2.star
 ```
 
 The list of options are organized by [Data Mining](#mining), [Modifications](#modify), and [Plots](#plot). Arguments that are not required are surrounded by parentheses in the descriptions below. Do not include the parentheses in your arguments.
 
 ### Input
 
 **```--i```** *```filename.star```*
@@ -160,18 +149,22 @@
 
 Remove particles that match a query (specified with ```--q```) within a column header (specified with ```--c```; see the [*Querying*](#query) options), and write to a new star file (default output.star, or specified with ```--o```).
 
 **```--remove_duplicates```** *```column-name```*
 
 Remove duplicate particles based on the column provided here (e.g. *ImageName*) (one instance of the duplicate is retained).
 
-**```--remove_mics_fromlist```** *`--f micrographs.txt`*
+**```--remove_mics_list```** *`--f micrographs.txt`*
 
 Remove particles that belong to micrographs that have a match in a second file provided by ```--f```, and write to a new star file (default output.star, or specified with ```--o```). You only need to have the micrograph names and not necessarily the full paths in the second file.
 
+**```--keep_mics_list```** *`--f micrographs.txt`*
+
+Keep particles that belong to micrographs that have a match in a second file provided by ```--f```, and write to a new star file (default output.star, or specified with ```--o```). You only need to have the micrograph names and not necessarily the full paths in the second file.
+
 **```--insert_column```** *```column-name```* *`--f values.txt`*
 
 Insert a new column that doesn't already exist with the values found in the file provided by ```--f```. The file should be a single column and should have an equivalent number to the star file. The result is written to a new star file (default output.star, or specified with ```--o```).
 
 **```--replace_column```** *```column-name```* *`--f values.txt`*
 
 Replace all entries of a column with a list of values found in the file provided by ```--f```. The file should be a single column and should have an equivalent number to the star file. This is useful when used in conjunction with ```--list_column```, which outputs column values for easy editing before reinsertion with ```--replace_column```. The result is written to a new star file (default output.star, or specified with ```--o```).
@@ -280,15 +273,15 @@
 
 ## Tips<a name="tips"></a>
 
 * Your input file needs to be a standard **Relion** *.star* file. Typical files include *particles.star*, *run_data.star*, *run_itxxx_data.star*, *movies.star*, *micrographs_ctf.star*, etc. You cannot parse *\*\_model.star* files for example.
 
 * The term *particles* here refers to rows in a star file, but the star files don't need to contain particles (e.g. parsing movies in a *movies.star* file).
 
-* Columns can be specified by their full or short names (e.g. \_rlnColumnName, rlnColumnName, or ColumnName). If scripting with the starparser package, columns are specified as their full name (i.e.\_rlnColumnName).
+* Columns can be specified by their full or short names (e.g. \_rlnColumnName, rlnColumnName, or ColumnName). If scripting with the starparser package, columns are specified as their full name (i.e. \_rlnColumnName).
 
 * If the star file lacks an optics table, such as those from Relion 3.0, add the ```--opticsless``` option to parse it.
 
 ---
 
 ## Limitations<a name="limits"></a>
```

### Comparing `starparser-1.51/README.md` & `starparser-1.52/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+Metadata-Version: 2.1
+Name: starparser
+Version: 1.52
+Summary: Manipulate and mine Relion star files.
+Home-page: http://pypi.python.org/pypi/starparser/
+Author: Sami Chaaban
+Author-email: chaaban@mrc-lmb.cam.ac.uk
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
 # starparser
 
 Use this package to manipulate Relion star files, including counting, modifying, plotting, and sifting the data. At the very least, this is a useful alternative to *awk* commands, which can get *awk*ward. Below is a description of the command-line options with some examples. Alternatively, use starparser within Relion or load the modules in your own Python scripts.
 
 Some of the options below are already available in Relion with "relion_star_handler".
 
 1. [Installation](#installation)
@@ -38,15 +49,15 @@
 ```
 starparser --i particles.star --list_column OriginX
 ```
 
 For some options, a second star file can also be passed as input ```--f secondfile.star```.
 
 ```
-starparser --i particles1.star --f particles2.star --find_shared MicrographName
+starparser --i particles1.star --find_shared MicrographName --f particles2.star
 ```
 
 The list of options are organized by [Data Mining](#mining), [Modifications](#modify), and [Plots](#plot). Arguments that are not required are surrounded by parentheses in the descriptions below. Do not include the parentheses in your arguments.
 
 ### Input
 
 **```--i```** *```filename.star```*
@@ -149,18 +160,22 @@
 
 Remove particles that match a query (specified with ```--q```) within a column header (specified with ```--c```; see the [*Querying*](#query) options), and write to a new star file (default output.star, or specified with ```--o```).
 
 **```--remove_duplicates```** *```column-name```*
 
 Remove duplicate particles based on the column provided here (e.g. *ImageName*) (one instance of the duplicate is retained).
 
-**```--remove_mics_fromlist```** *`--f micrographs.txt`*
+**```--remove_mics_list```** *`--f micrographs.txt`*
 
 Remove particles that belong to micrographs that have a match in a second file provided by ```--f```, and write to a new star file (default output.star, or specified with ```--o```). You only need to have the micrograph names and not necessarily the full paths in the second file.
 
+**```--keep_mics_list```** *`--f micrographs.txt`*
+
+Keep particles that belong to micrographs that have a match in a second file provided by ```--f```, and write to a new star file (default output.star, or specified with ```--o```). You only need to have the micrograph names and not necessarily the full paths in the second file.
+
 **```--insert_column```** *```column-name```* *`--f values.txt`*
 
 Insert a new column that doesn't already exist with the values found in the file provided by ```--f```. The file should be a single column and should have an equivalent number to the star file. The result is written to a new star file (default output.star, or specified with ```--o```).
 
 **```--replace_column```** *```column-name```* *`--f values.txt`*
 
 Replace all entries of a column with a list of values found in the file provided by ```--f```. The file should be a single column and should have an equivalent number to the star file. This is useful when used in conjunction with ```--list_column```, which outputs column values for easy editing before reinsertion with ```--replace_column```. The result is written to a new star file (default output.star, or specified with ```--o```).
@@ -269,15 +284,15 @@
 
 ## Tips<a name="tips"></a>
 
 * Your input file needs to be a standard **Relion** *.star* file. Typical files include *particles.star*, *run_data.star*, *run_itxxx_data.star*, *movies.star*, *micrographs_ctf.star*, etc. You cannot parse *\*\_model.star* files for example.
 
 * The term *particles* here refers to rows in a star file, but the star files don't need to contain particles (e.g. parsing movies in a *movies.star* file).
 
-* Columns can be specified by their full or short names (e.g. \_rlnColumnName, rlnColumnName, or ColumnName). If scripting with the starparser package, columns are specified as their full name (i.e.\_rlnColumnName).
+* Columns can be specified by their full or short names (e.g. \_rlnColumnName, rlnColumnName, or ColumnName). If scripting with the starparser package, columns are specified as their full name (i.e. \_rlnColumnName).
 
 * If the star file lacks an optics table, such as those from Relion 3.0, add the ```--opticsless``` option to parse it.
 
 ---
 
 ## Limitations<a name="limits"></a>
```

### Comparing `starparser-1.51/setup.py` & `starparser-1.52/setup.py`

 * *Files identical despite different names*

### Comparing `starparser-1.51/starparser/argparser.py` & `starparser-1.52/starparser/argparser.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,27 +25,27 @@
 
     info_opts.add_option("--extract",
         action="store_true", dest="parser_extractparticles", default=False,
         help="Find particles that match a column header (--c) and query (--q) and write them to a new star file.")
 
     info_opts.add_option("--limit",
         action="store", dest="parser_limitparticles", type="string", default = "", metavar='column/comparator/value',
-        help="Extract particles that match a specific comparison (\"lt\" for less than, \"gt\" for greater than, \"le\" for less than or equal to, \"ge\" for greater than or equal to). The argument to pass is column/comparator/value (e.g. \"_rlnDefocusU/lt/40000\" for defocus values less than 40000).")
+        help="Extract particles that match a specific comparison (\"lt\" for less than, \"gt\" for greater than, \"le\" for less than or equal to, \"ge\" for greater than or equal to). The argument to pass is column/comparator/value (e.g. \"DefocusU/lt/40000\" for defocus values less than 40000).")
     
     info_opts.add_option("--count",
         action="store_true", dest="parser_countme", default=False,
         help="Count particles and display the result. Optionally, use --c and --q to count a subset of particles, otherwise counts all.")
     
     info_opts.add_option("--count_mics",
         action="store_true", dest="parser_uniquemics", default=False,
         help="Count the number of unique micrographs. Optionally, use --c and --q to count from a subset of particles, otherwise counts all.")
     
     info_opts.add_option("--list_column",
         action="store", dest="parser_writecol", type="string", default="", metavar='column-name(s)',
-        help="Write all values of a column to a file. For example, passing \"_rlnMicrographName\" will write all values to MicrographName.txt. To write multiple columns, separate the column names with a slash (for example, \"_rlnMicrographName/_rlnCoordinateX\" outputs MicrographName.txt and CoordinateX.txt). This can be used with --c and --q to only consider values that match the query, otherwise it lists all values.")
+        help="Write all values of a column to a file. For example, passing \"MicrographName\" will write all values to MicrographName.txt. To write multiple columns, separate the column names with a slash (for example, \"MicrographName/CoordinateX\" outputs MicrographName.txt and CoordinateX.txt). This can be used with --c and --q to only consider values that match the query, otherwise it lists all values.")
 
     info_opts.add_option("--find_shared",
         action="store", dest="parser_findshared", type="string", default="", metavar='column-name',
         help="Find particles that are shared between the input star file and the one provided by --f based on the column provided here. Two new star files will be written, one with the shared particles and one with the unique particles.")
 
     info_opts.add_option("--match_mics",
         action="store_true", dest="parser_matchmics", default=False,
@@ -89,80 +89,84 @@
 
     info_opts.add_option("--split_optics",
         action="store_true", dest="parser_splitoptics", default=False,
         help="Split the input star file into independent star files for each optics group. The files will have the names of the optics group.")
 
     info_opts.add_option("--sort_by",
         action="store", dest="parser_sort", type="string", default="", metavar='column-name',
-        help="Sort the column in ascending order and write a new file. Add a slash followed by \"n\" if the column contains numeric values (e.g. \"_rlnClassNumber/n\"); otherwise, it will sort the values as text.")   
+        help="Sort the column in ascending order and write a new file. Add a slash followed by \"n\" if the column contains numeric values (e.g. \"ClassNumber/n\"); otherwise, it will sort the values as text.")   
 
     parser.add_option_group(info_opts)
 
     modify_opts = optparse.OptionGroup(
         parser, 'Modification Options')
 
     modify_opts.add_option("--operate",
         action="store", dest="parser_operate", type="string", default="", metavar='column[operator]value',
-        help="Perform operation on all values of a column. The argument to pass is column[operator]value (without the brackets and without any spaces); operators include \"*\", \"/\", \"+\", and \"-\" (e.g. _rlnHelicalTrackLength*0.25). If the terminal throws an error, try surrounding the argument with quotes.")
+        help="Perform operation on all values of a column. The argument to pass is column[operator]value (without the brackets and without any spaces); operators include \"*\", \"/\", \"+\", and \"-\" (e.g. HelicalTrackLength*0.25). If the terminal throws an error, try surrounding the argument with quotes.")
 
     modify_opts.add_option("--operate_columns",
         action="store", dest="parser_operatecolumns", type="string", default="", metavar='column[operator]value',
-        help="Perform operation between two columns and write to a new column. The argument to pass is column1[operator]column2=newcolumn (without the brackets and without any spaces); operators include \"*\", \"/\", \"+\", and \"-\" (e.g. _rlnCoordinateX*_rlnOriginX=_rlnShifted). If the terminal throws an error, try surrounding the argument with quotes.")
+        help="Perform operation between two columns and write to a new column. The argument to pass is column1[operator]column2=newcolumn (without the brackets and without any spaces); operators include \"*\", \"/\", \"+\", and \"-\" (e.g. CoordinateX*OriginX=Shifted). If the terminal throws an error, try surrounding the argument with quotes.")
 
     modify_opts.add_option("--remove_column",
         action="store", dest="parser_delcolumn", type="string", default="", metavar='column-name(s)',
-        help="Remove column, renumber headers, and write to a new star file. E.g. _rlnMicrographName. To enter multiple columns, separate them with a slash: _rlnMicrographName/_rlnCoordinateX.")
+        help="Remove column, renumber headers, and write to a new star file. E.g. MicrographName. To enter multiple columns, separate them with a slash: MicrographName/CoordinateX.")
     
     modify_opts.add_option("--remove_particles",
         action="store_true", dest="parser_delparticles", default=False,
         help="Remove particles that match a query (specified with --q) within a column header (specified with --c), and write to a new star file.")
 
     modify_opts.add_option("--remove_duplicates",
         action="store", dest="parser_delduplicates", default="", metavar='column-name',
-        help="Remove duplicate particles based on the column provided here (e.g. _rlnImageName).")
+        help="Remove duplicate particles based on the column provided here (e.g. ImageName).")
 
-    modify_opts.add_option("--remove_mics_fromlist",
+    modify_opts.add_option("--remove_mics_list",
         action="store_true", dest="parser_delmics", default=False,
-        help="Remove particles that belong to micrographs that have a match in a second file provided by --f.")
+        help="Remove particles that belong to micrographs that have a match in a second file provided by --f (single column list of micrographs).")
+
+    modify_opts.add_option("--keep_mics_list",
+        action="store_true", dest="parser_keepmics", default=False,
+        help="Keep particles that belong to micrographs that have a match in a second file provided by --f (single column list of micrographs).")
 
     modify_opts.add_option("--insert_column",
         action="store", dest="parser_insertcol", type="string", default="", metavar='column-name',
         help="Insert a new column that has the values found in the file provided by --f. The file should be a single column and should have an equivalent number to the star file.")     
 
     modify_opts.add_option("--replace_column",
         action="store", dest="parser_replacecol", type="string", default="", metavar='column-name',
         help="Replace all entries of a column with a list of values found in the file provided by --f. The file should be a single column and should have an equivalent number to the star file.")     
 
     modify_opts.add_option("--copy_column",
         action="store", dest="parser_copycol", type="string", default="", metavar='source-column/target-column',
-        help="Replace all entries of a target column with those of a source column in the same star file. If the target column exists, its values will be replaced. If the target does not exist, a new column will be made. The argument to pass is source-column/target-column (e.g. _rlnAngleTiltPrior/_rlnAngleTilt)")     
+        help="Replace all entries of a target column with those of a source column in the same star file. If the target column exists, its values will be replaced. If the target does not exist, a new column will be made. The argument to pass is source-column/target-column (e.g. AngleTiltPrior/AngleTilt)")     
 
     modify_opts.add_option("--reset_column",
         action="store", dest="parser_resetcol", type="string", default="", metavar='column-name/new-value',
-        help="Change all values of a column to the one provided here. The argument to pass is column-name/new-value (e.g. _rlnOriginX/0).")
+        help="Change all values of a column to the one provided here. The argument to pass is column-name/new-value (e.g. OriginX/0).")
 
     modify_opts.add_option("--swap_columns",
         action="store", dest="parser_swapcolumns", type="string", default="", metavar='column-name(s)',
-        help="Swap columns from another star file (specified with --f). E.g. _rlnMicrographName. To enter multiple columns, separate them with a slash: _rlnMicrographName/_rlnCoordinateX.")
+        help="Swap columns from another star file (specified with --f). E.g. MicrographName. To enter multiple columns, separate them with a slash: MicrographName/CoordinateX.")
 
     modify_opts.add_option("--insert_optics_column",
         action="store", dest="parser_insertopticscol", type="string", default="", metavar='column-name/value',
-        help="Insert a new column in the optics table with the name and value provided (e.g. _rlnAmplitudeContrast/0.1). The value will populate all rows of the optics table.")
+        help="Insert a new column in the optics table with the name and value provided (e.g. AmplitudeContrast/0.1). The value will populate all rows of the optics table.")
 
     modify_opts.add_option("--fetch_from_nearby",
         action="store", dest="parser_fetchnearby", type="string", default="", metavar='distance/column-name(s)',
-        help="Find the nearest particle in a second star file (specified by --f) and if it is within a threshold distance, retrieve its column value to replace the original particle column value. The argument to pass is distance/column-name (e.g. 300/_rlnClassNumber). Particles that couldn't be matched to a neighbor will be skipped (i.e. if the second star file lacks particles in that micrograph). The micrograph paths from _rlnMicrographName do not necessarily need to match, just the filenames need to.")
+        help="Find the nearest particle in a second star file (specified by --f) and if it is within a threshold distance, retrieve its column value to replace the original particle column value. The argument to pass is distance/column-name (e.g. 300/ClassNumber). Particles that couldn't be matched to a neighbor will be skipped (i.e. if the second star file lacks particles in that micrograph). The micrograph paths from MicrographName do not necessarily need to match, just the filenames need to.")
 
     modify_opts.add_option("--import_mic_values",
         action="store", dest="parser_importmicvalues", type="string", default="", metavar='column-name(s)',
-        help="For every particle, find the micrograph that it belongs to in a second star file (provided by --f) and replace the original column value with that of the second star file (e.g. _rlnOpticsGroup). This requires that the second star file only has one instance of each micrograph name (e.g. a micrographfs_ctf.star file). To import multiple columns, separate them with a slash.")
+        help="For every particle, find the micrograph that it belongs to in a second star file (provided by --f) and replace the original column value with that of the second star file (e.g. OpticsGroup). The paths do not have to be identical, just the micrograph filename itself. To import multiple columns, separate them with a slash.")
 
     modify_opts.add_option("--import_particle_values",
         action="store", dest="parser_importpartvalues", type="string", default="", metavar='column-name(s)',
-        help="For every particle in the input star file, find the equivalent particle in a second star file (provided by --f) (i.e. those with equivalent _rlnImageName values) and replace the original column value with the one from the second star file. To import multiple columns, separate them with a slash.")
+        help="For every particle in the input star file, find the equivalent particle in a second star file (provided by --f) (i.e. those with equivalent ImageName values) and replace the original column value with the one from the second star file. To import multiple columns, separate them with a slash.")
 
     modify_opts.add_option("--regroup",
         action="store", dest="parser_regroup", type="int", default=0, metavar='particles-per-group',
         help="Regroup particles such that those with similar defocus values are in the same group. Any value can be entered. This is useful if there aren't enough particles in each micrograph to make meaningful groups. Note that Subset selection in Relion can also regroup.")
 
     modify_opts.add_option("--swap_optics",
         action="store_true", dest="parser_swapoptics", default=False,
@@ -187,15 +191,15 @@
 
     plot_opts.add_option("--histogram",
         action="store", dest="parser_plot", default="", metavar="column-name",
         help="Plot values of a column as a histogram. Optionally, use --c and --q to only plot a subset of particles, otherwise it will plot all. The filename will be that of the column name. Use --t to change the filetype.")
 
     plot_opts.add_option("--plot_orientations",
         action="store_true", dest="parser_plotangledist", default=False,
-        help="Plot the particle orientations based on the _rlnAngleRot and _rlnAngleTilt columns on a Mollweide projection (longitude and latitude, respectively). Optionally, use --c and --q to only plot a subset of particles, otherwise it will plot all. Use --t to change the filetype.")
+        help="Plot the particle orientations based on the AngleRot and AngleTilt columns on a Mollweide projection (longitude and latitude, respectively). Optionally, use --c and --q to only plot a subset of particles, otherwise it will plot all. Use --t to change the filetype.")
     
     plot_opts.add_option("--plot_class_iterations",
         action="store", dest="parser_classiterations", type="string", default="", metavar="classes",
         help="Plot the number of particles per class for all iterations up to the one provided in the input (skips iterations 0 and 1). Pass \"all\" to plot all classes or separate the classes you want with a dash (e.g. 1/2/5). Use --t to change filetype.")
     
     plot_opts.add_option("--plot_class_proportions",
         action="store_true", dest="parser_classproportion", default=False,
@@ -208,15 +212,15 @@
     parser.add_option_group(plot_opts)
 
     query_opts = optparse.OptionGroup(
         parser, 'Query Options')
     
     query_opts.add_option("--c",
         action="store", dest="parser_column", type="string", default="", metavar='column-name(s)',
-        help="Column query. E.g. _rlnMicrographName. To enter multiple columns, separate them with a slash: _rlnMicrographName/_rlnCoordinateX.")
+        help="Column query. E.g. MicrographName. To enter multiple columns, separate them with a slash: MicrographName/CoordinateX.")
     
     query_opts.add_option("--q",
         action="store", dest="parser_query", type="string", default="", metavar='query(ies)',
         help="Particle query term(s) to look for in the values within the specified column. To enter multiple queries, separate them with a slash: 20200101/20200203. To escape a slash, use a \",\". Use --e if the query should exactly match the value.")
 
     query_opts.add_option("--e",
         action="store_true", dest="parser_exact", default=False, metavar="match-exactly",
```

### Comparing `starparser-1.51/starparser/columnplay.py` & `starparser-1.52/starparser/columnplay.py`

 * *Files identical despite different names*

### Comparing `starparser-1.51/starparser/decisiontree.py` & `starparser-1.52/starparser/decisiontree.py`

 * *Files 1% similar despite different names*

```diff
@@ -248,15 +248,15 @@
         newtotal = len(newparticles.index)
         print("\n>> Removed " + str(purgednumber) + " particles (out of " + str(totalparticles) + ", " + str(round(purgednumber*100/totalparticles,1)) + "%) that were duplicates based on the " + column + " column.")
         print(">> The new total is " + str(newtotal) + " particles.")
         fileparser.writestar(newparticles, metadata, params["parser_outname"], relegateflag)
         sys.exit()
 
     """
-    --remove_mics_fromlist
+    --remove_mics_list
     """
 
     if params["parser_delmics"]:
         if params["parser_query"] != "" or params["parser_column"] != "":
             print("\n>> Error: you cannot provide a query to the --remove_mics_fromlist option.\n")
             sys.exit()
         if params["parser_file2"] == "":
@@ -269,14 +269,37 @@
         with open(file2) as f:
             micstodelete = [line.split()[0] for line in f]
         newparticles = particleplay.delmics(allparticles,micstodelete)
         purgednumber = totalparticles - len(newparticles.index)
         print("\n>> Removed " + str(purgednumber) + " particles (out of " + str(totalparticles) + ", " + str(round(purgednumber*100/totalparticles,1)) + "%) that matched the micrographs in " + file2 + ".")
         fileparser.writestar(newparticles, metadata, params["parser_outname"], relegateflag)
         sys.exit()
+
+    """
+    --keep_mics_list
+    """
+
+    if params["parser_keepmics"]:
+        if params["parser_query"] != "" or params["parser_column"] != "":
+            print("\n>> Error: you cannot provide a query to the --keep_mics_fromlist option.\n")
+            sys.exit()
+        if params["parser_file2"] == "":
+            print("\n>> Error: provide a second file with --f to match micrographs.\n")
+            sys.exit()
+        file2 = params["parser_file2"]
+        if not os.path.isfile(file2):
+            print("\n>> Error: \"" + file2 + "\" does not exist.\n")
+            sys.exit()
+        with open(file2) as f:
+            micstokeep = [line.split()[0] for line in f]
+        newparticles = particleplay.keepmics(allparticles,micstokeep)
+        keptnumber = len(newparticles.index)
+        print("\n>> Kept " + str(keptnumber) + " particles (out of " + str(totalparticles) + ", " + str(round(keptnumber*100/totalparticles,1)) + "%) that matched the micrographs in " + file2 + ".")
+        fileparser.writestar(newparticles, metadata, params["parser_outname"], relegateflag)
+        sys.exit()
         
     """
     --swap_columns
     """
 
     if params["parser_swapcolumns"] != "":
         columnstoswap = params["parser_swapcolumns"].split("/")
```

### Comparing `starparser-1.51/starparser/fileparser.py` & `starparser-1.52/starparser/fileparser.py`

 * *Files 2% similar despite different names*

```diff
@@ -130,14 +130,20 @@
     #Table Name
     """
 
     """
     For the second data table, we want to know what kind of table it is
     e.g. data_particles
     """
+    try:
+        starfilesplit_test[opticsheaderend:].index("#")
+        starfilesplit_test[opticsheaderend:].index("loop_")
+    except ValueError:
+        print("\n>> Error: could not parse the star file. If it does not have an optics table, add --opticsless.\n")
+        sys.exit()
 
     if versionexist:
         opticsdataend = starfilesplit_test[opticsheaderend:].index("#") + opticsheaderend
         tablename = starfilesplit_test[opticsdataend+3]
     else:
         opticsdataend = starfilesplit_test[opticsheaderend:].index("loop_") + opticsheaderend - 1
         tablename = starfilesplit_test[opticsdataend]
```

### Comparing `starparser-1.51/starparser/particleplay.py` & `starparser-1.52/starparser/particleplay.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,23 +85,32 @@
 --remove_duplicates
 """
 def delduplicates(particles, column):
 
     return(particles.drop_duplicates(subset=[column]))
 
 """
---remove_mics_fromlist
+--remove_mics_list
 """
 def delmics(particles, micstodelete):
     purgedparticles = particles.copy()
     m = "|".join(micstodelete)
     purgedparticles.drop(purgedparticles[purgedparticles["_rlnMicrographName"].str.contains(m)].index , axis=0,inplace=True)    
     return(purgedparticles)
 
 """
+--keep_mics_list
+"""
+def keepmics(particles, micstokeep):
+    keptparticles = particles.copy()
+    m = "|".join(micstokeep)
+    keptparticles = keptparticles[keptparticles["_rlnMicrographName"].str.contains(m)]
+    return(keptparticles)
+
+"""
 --extract
 """
 def extractparticles(particles, columns, query, queryexact):
     
     if len(columns)>1:
         print("\n>> Error: you have specified two columns. Only specify one if you're extracting from a subset of the data using a query.\n")
         sys.exit()
```

### Comparing `starparser-1.51/starparser/plots.py` & `starparser-1.52/starparser/plots.py`

 * *Files identical despite different names*

### Comparing `starparser-1.51/starparser/specialparticles.py` & `starparser-1.52/starparser/specialparticles.py`

 * *Files identical despite different names*

### Comparing `starparser-1.51/starparser/splits.py` & `starparser-1.52/starparser/splits.py`

 * *Files identical despite different names*

### Comparing `starparser-1.51/starparser.egg-info/PKG-INFO` & `starparser-1.52/starparser.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starparser
-Version: 1.51
+Version: 1.52
 Summary: Manipulate and mine Relion star files.
 Home-page: http://pypi.python.org/pypi/starparser/
 Author: Sami Chaaban
 Author-email: chaaban@mrc-lmb.cam.ac.uk
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
@@ -49,15 +49,15 @@
 ```
 starparser --i particles.star --list_column OriginX
 ```
 
 For some options, a second star file can also be passed as input ```--f secondfile.star```.
 
 ```
-starparser --i particles1.star --f particles2.star --find_shared MicrographName
+starparser --i particles1.star --find_shared MicrographName --f particles2.star
 ```
 
 The list of options are organized by [Data Mining](#mining), [Modifications](#modify), and [Plots](#plot). Arguments that are not required are surrounded by parentheses in the descriptions below. Do not include the parentheses in your arguments.
 
 ### Input
 
 **```--i```** *```filename.star```*
@@ -160,18 +160,22 @@
 
 Remove particles that match a query (specified with ```--q```) within a column header (specified with ```--c```; see the [*Querying*](#query) options), and write to a new star file (default output.star, or specified with ```--o```).
 
 **```--remove_duplicates```** *```column-name```*
 
 Remove duplicate particles based on the column provided here (e.g. *ImageName*) (one instance of the duplicate is retained).
 
-**```--remove_mics_fromlist```** *`--f micrographs.txt`*
+**```--remove_mics_list```** *`--f micrographs.txt`*
 
 Remove particles that belong to micrographs that have a match in a second file provided by ```--f```, and write to a new star file (default output.star, or specified with ```--o```). You only need to have the micrograph names and not necessarily the full paths in the second file.
 
+**```--keep_mics_list```** *`--f micrographs.txt`*
+
+Keep particles that belong to micrographs that have a match in a second file provided by ```--f```, and write to a new star file (default output.star, or specified with ```--o```). You only need to have the micrograph names and not necessarily the full paths in the second file.
+
 **```--insert_column```** *```column-name```* *`--f values.txt`*
 
 Insert a new column that doesn't already exist with the values found in the file provided by ```--f```. The file should be a single column and should have an equivalent number to the star file. The result is written to a new star file (default output.star, or specified with ```--o```).
 
 **```--replace_column```** *```column-name```* *`--f values.txt`*
 
 Replace all entries of a column with a list of values found in the file provided by ```--f```. The file should be a single column and should have an equivalent number to the star file. This is useful when used in conjunction with ```--list_column```, which outputs column values for easy editing before reinsertion with ```--replace_column```. The result is written to a new star file (default output.star, or specified with ```--o```).
@@ -280,15 +284,15 @@
 
 ## Tips<a name="tips"></a>
 
 * Your input file needs to be a standard **Relion** *.star* file. Typical files include *particles.star*, *run_data.star*, *run_itxxx_data.star*, *movies.star*, *micrographs_ctf.star*, etc. You cannot parse *\*\_model.star* files for example.
 
 * The term *particles* here refers to rows in a star file, but the star files don't need to contain particles (e.g. parsing movies in a *movies.star* file).
 
-* Columns can be specified by their full or short names (e.g. \_rlnColumnName, rlnColumnName, or ColumnName). If scripting with the starparser package, columns are specified as their full name (i.e.\_rlnColumnName).
+* Columns can be specified by their full or short names (e.g. \_rlnColumnName, rlnColumnName, or ColumnName). If scripting with the starparser package, columns are specified as their full name (i.e. \_rlnColumnName).
 
 * If the star file lacks an optics table, such as those from Relion 3.0, add the ```--opticsless``` option to parse it.
 
 ---
 
 ## Limitations<a name="limits"></a>
```

