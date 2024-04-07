# Comparing `tmp/biofkit-0.1.8.tar.gz` & `tmp/biofkit-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biofkit-0.1.8.tar", last modified: Wed Mar  6 01:41:53 2024, max compression
+gzip compressed data, was "biofkit-0.1.9.tar", last modified: Wed Mar  6 02:06:07 2024, max compression
```

## Comparing `biofkit-0.1.8.tar` & `biofkit-0.1.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 chouuken  (1000) chouuken  (1000)        0 2024-03-06 01:41:53.279473 biofkit-0.1.8/
--rw-rw-r--   0 chouuken  (1000) chouuken  (1000)    11357 2024-01-29 08:08:06.000000 biofkit-0.1.8/LICENSE
--rw-r--r--   0 chouuken  (1000) chouuken  (1000)     1040 2024-03-06 01:41:53.279473 biofkit-0.1.8/PKG-INFO
--rw-rw-r--   0 chouuken  (1000) chouuken  (1000)      381 2024-03-06 01:08:13.000000 biofkit-0.1.8/README.md
--rw-rw-r--   0 chouuken  (1000) chouuken  (1000)      655 2024-03-06 01:41:11.000000 biofkit-0.1.8/pyproject.toml
--rw-rw-r--   0 chouuken  (1000) chouuken  (1000)       38 2024-03-06 01:41:53.279473 biofkit-0.1.8/setup.cfg
-drwxrwxr-x   0 chouuken  (1000) chouuken  (1000)        0 2024-03-06 01:41:53.275473 biofkit-0.1.8/src/
-drwxrwxr-x   0 chouuken  (1000) chouuken  (1000)        0 2024-03-06 01:41:53.275473 biofkit-0.1.8/src/biofkit/
--rw-rw-r--   0 chouuken  (1000) chouuken  (1000)      100 2024-01-29 08:08:06.000000 biofkit-0.1.8/src/biofkit/__init__.py
-drwxrwxr-x   0 chouuken  (1000) chouuken  (1000)        0 2024-03-06 01:41:53.275473 biofkit-0.1.8/src/biofkit/proteinKit/
--rw-rw-r--   0 chouuken  (1000) chouuken  (1000)        0 2024-03-06 01:05:25.000000 biofkit-0.1.8/src/biofkit/proteinKit/__init__.py
--rw-rw-r--   0 chouuken  (1000) chouuken  (1000)     5426 2024-03-06 01:38:28.000000 biofkit-0.1.8/src/biofkit/proteinKit/oldProtein.py
--rw-rw-r--   0 chouuken  (1000) chouuken  (1000)    14204 2024-02-26 03:51:02.000000 biofkit-0.1.8/src/biofkit/proteinKit/pdbKit.py
--rw-rw-r--   0 chouuken  (1000) chouuken  (1000)     3735 2024-02-26 03:52:24.000000 biofkit-0.1.8/src/biofkit/proteinKit/proteinClass.py
-drwxrwxr-x   0 chouuken  (1000) chouuken  (1000)        0 2024-03-06 01:41:53.275473 biofkit-0.1.8/src/biofkit/seqKit/
--rw-rw-r--   0 chouuken  (1000) chouuken  (1000)        0 2024-01-29 08:08:06.000000 biofkit-0.1.8/src/biofkit/seqKit/__init__.py
--rw-rw-r--   0 chouuken  (1000) chouuken  (1000)    33925 2024-02-20 08:02:23.000000 biofkit-0.1.8/src/biofkit/seqKit/convKit.py
-drwxrwxr-x   0 chouuken  (1000) chouuken  (1000)        0 2024-03-06 01:41:53.279473 biofkit-0.1.8/src/biofkit.egg-info/
--rw-r--r--   0 chouuken  (1000) chouuken  (1000)     1040 2024-03-06 01:41:53.000000 biofkit-0.1.8/src/biofkit.egg-info/PKG-INFO
--rw-rw-r--   0 chouuken  (1000) chouuken  (1000)      401 2024-03-06 01:41:53.000000 biofkit-0.1.8/src/biofkit.egg-info/SOURCES.txt
--rw-rw-r--   0 chouuken  (1000) chouuken  (1000)        1 2024-03-06 01:41:53.000000 biofkit-0.1.8/src/biofkit.egg-info/dependency_links.txt
--rw-rw-r--   0 chouuken  (1000) chouuken  (1000)        8 2024-03-06 01:41:53.000000 biofkit-0.1.8/src/biofkit.egg-info/top_level.txt
+drwxrwxr-x   0 chouuken  (1000) chouuken  (1000)        0 2024-03-06 02:06:07.046106 biofkit-0.1.9/
+-rw-rw-r--   0 chouuken  (1000) chouuken  (1000)    11357 2024-01-29 08:08:06.000000 biofkit-0.1.9/LICENSE
+-rw-r--r--   0 chouuken  (1000) chouuken  (1000)     1040 2024-03-06 02:06:07.046106 biofkit-0.1.9/PKG-INFO
+-rw-rw-r--   0 chouuken  (1000) chouuken  (1000)      381 2024-03-06 01:08:13.000000 biofkit-0.1.9/README.md
+-rw-rw-r--   0 chouuken  (1000) chouuken  (1000)      655 2024-03-06 02:05:27.000000 biofkit-0.1.9/pyproject.toml
+-rw-rw-r--   0 chouuken  (1000) chouuken  (1000)       38 2024-03-06 02:06:07.046106 biofkit-0.1.9/setup.cfg
+drwxrwxr-x   0 chouuken  (1000) chouuken  (1000)        0 2024-03-06 02:06:07.042111 biofkit-0.1.9/src/
+drwxrwxr-x   0 chouuken  (1000) chouuken  (1000)        0 2024-03-06 02:06:07.046106 biofkit-0.1.9/src/biofkit/
+-rw-rw-r--   0 chouuken  (1000) chouuken  (1000)      100 2024-01-29 08:08:06.000000 biofkit-0.1.9/src/biofkit/__init__.py
+drwxrwxr-x   0 chouuken  (1000) chouuken  (1000)        0 2024-03-06 02:06:07.046106 biofkit-0.1.9/src/biofkit/proteinKit/
+-rw-rw-r--   0 chouuken  (1000) chouuken  (1000)        0 2024-03-06 01:05:25.000000 biofkit-0.1.9/src/biofkit/proteinKit/__init__.py
+-rw-rw-r--   0 chouuken  (1000) chouuken  (1000)     5450 2024-03-06 02:02:19.000000 biofkit-0.1.9/src/biofkit/proteinKit/oldProtein.py
+-rw-rw-r--   0 chouuken  (1000) chouuken  (1000)    14223 2024-03-06 02:04:13.000000 biofkit-0.1.9/src/biofkit/proteinKit/pdbKit.py
+-rw-rw-r--   0 chouuken  (1000) chouuken  (1000)     3735 2024-03-06 02:02:38.000000 biofkit-0.1.9/src/biofkit/proteinKit/proteinClass.py
+drwxrwxr-x   0 chouuken  (1000) chouuken  (1000)        0 2024-03-06 02:06:07.046106 biofkit-0.1.9/src/biofkit/seqKit/
+-rw-rw-r--   0 chouuken  (1000) chouuken  (1000)        0 2024-01-29 08:08:06.000000 biofkit-0.1.9/src/biofkit/seqKit/__init__.py
+-rw-rw-r--   0 chouuken  (1000) chouuken  (1000)    33930 2024-03-06 02:05:02.000000 biofkit-0.1.9/src/biofkit/seqKit/convKit.py
+drwxrwxr-x   0 chouuken  (1000) chouuken  (1000)        0 2024-03-06 02:06:07.046106 biofkit-0.1.9/src/biofkit.egg-info/
+-rw-r--r--   0 chouuken  (1000) chouuken  (1000)     1040 2024-03-06 02:06:07.000000 biofkit-0.1.9/src/biofkit.egg-info/PKG-INFO
+-rw-rw-r--   0 chouuken  (1000) chouuken  (1000)      401 2024-03-06 02:06:07.000000 biofkit-0.1.9/src/biofkit.egg-info/SOURCES.txt
+-rw-rw-r--   0 chouuken  (1000) chouuken  (1000)        1 2024-03-06 02:06:07.000000 biofkit-0.1.9/src/biofkit.egg-info/dependency_links.txt
+-rw-rw-r--   0 chouuken  (1000) chouuken  (1000)        8 2024-03-06 02:06:07.000000 biofkit-0.1.9/src/biofkit.egg-info/top_level.txt
```

### Comparing `biofkit-0.1.8/LICENSE` & `biofkit-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `biofkit-0.1.8/PKG-INFO` & `biofkit-0.1.9/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biofkit
-Version: 0.1.8
+Version: 0.1.9
 Summary: With biofkit you can deal with pdb file (extract sequence, atom information and so on) very easily. 
 Author-email: Zhang Yujian <Chouuken@outlook.com>, Wu Yuexin <wuyvexiaoxin@163.com>
 Project-URL: Homepage, https://github.com/Chou-Uken/biofkit
 Project-URL: Issues, https://github.com/Chou-Uken/biofkit/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `biofkit-0.1.8/pyproject.toml` & `biofkit-0.1.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "biofkit"
-version = "0.1.8"
+version = "0.1.9"
 authors = [
   { name="Zhang Yujian", email="Chouuken@outlook.com" },
   { name="Wu Yuexin", email="wuyvexiaoxin@163.com" }
 ]
 description = "With biofkit you can deal with pdb file (extract sequence, atom information and so on) very easily. "
 readme = "README.md"
 requires-python = ">=3.10"
```

### Comparing `biofkit-0.1.8/src/biofkit/proteinKit/oldProtein.py` & `biofkit-0.1.9/src/biofkit/proteinKit/oldProtein.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 '''
 This script was created on Jan 3rd, 2024 by Zhang Yujian as a doctoral candidate in Institute of Zoology, CAS.
 Thanks for using. Please report bugs (if any) at zhangyujian23@mails.ucas.ac.cn.
 Sorry for my poor English.
 '''
 
 import os
-import pdbKit
+from biofkit.proteinKit import pdbKit
 
 # This funtion 'proDict2ProList' is used to tranfer pdbDict into pdbList.
 def proDict2ProList(rawDict: dict) -> list:
     output: list = [[] for count in range(len(rawDict['Serial']))]
     for atomIdx in range(len(rawDict['Serial'])):
         output[atomIdx].append(rawDict['Serial'][atomIdx])
         output[atomIdx].append(rawDict['Atom'][atomIdx])
```

### Comparing `biofkit-0.1.8/src/biofkit/proteinKit/pdbKit.py` & `biofkit-0.1.9/src/biofkit/proteinKit/pdbKit.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 '''
 This script was created on Dec 17th, 2023 by Zhang Yujian as a doctoral candidate in Institute of Zoology, CAS.
 Thanks for using. Please report bugs (if any) at zhangyujian23@mails.ucas.ac.cn.
 Sorry for my poor English.
 '''
 
 import os
+from biofkit.proteinKit.proteinClass import Atom, Residue, Peptide, Protein
 
 class ProteinKit:
 
     # Dictionary used to transfer abbreviation with the first letter capitalized to shorter abbreviation.
     aaDictTHREE2One: dict[str, str] = {
         'ALA': 'A', 'ARG': 'R', 'ASN': 'N', 'ASP': 'D', 'CYS': 'C',    \
         'GLN': 'Q', 'GLU': 'E', 'GLY': 'G', 'HIS': 'H', 'ILE': 'I',    \
@@ -199,15 +200,14 @@
                 output[keyNameList[6]].append(float(line[38:46].strip()))
                 output[keyNameList[7]].append(float(line[46:54].strip()))
     return (output)
 
 
 
 # load PDB file
-from proteinClass import Atom, Residue, Peptide, Protein
 def readPDB(pdbFile: str) -> Protein:
     proteinKit: ProteinKit = ProteinKit()
     with open(file=pdbFile, mode='r') as pdb:
         atomBuffer: list[Atom] = []
         residueBuffer: list[Residue] = []
         peptideBuffer: list[Peptide] = []
         resSeq: int = 0
```

### Comparing `biofkit-0.1.8/src/biofkit/proteinKit/proteinClass.py` & `biofkit-0.1.9/src/biofkit/proteinKit/proteinClass.py`

 * *Files identical despite different names*

### Comparing `biofkit-0.1.8/src/biofkit/seqKit/convKit.py` & `biofkit-0.1.9/src/biofkit/seqKit/convKit.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     # Unitary matrix
     dnaUnitaryMatrix: dict[bool, int] = {True: 1, False: 0}
     
     # Transition-transversion matrix
     dnaTTMatrix: dict[str, int] = {True: 1, 'transition': -1, 'transversion': -5}
 
     # BLAST matrix
-    dnaBlastMatrix: dict[bool] = {True: 5, False: -4}
+    dnaBlastMatrix: dict[bool, int] = {True: 5, False: -4}
 
     # Protein Substitution Matrix
     # Unitary matrix
     protUnitaryMatrix: dict[bool, int] = {True: 1, False: 0}
 
     # PAM-250 matrix
     pam250Matrix: dict[str, int] = {
```

### Comparing `biofkit-0.1.8/src/biofkit.egg-info/PKG-INFO` & `biofkit-0.1.9/src/biofkit.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biofkit
-Version: 0.1.8
+Version: 0.1.9
 Summary: With biofkit you can deal with pdb file (extract sequence, atom information and so on) very easily. 
 Author-email: Zhang Yujian <Chouuken@outlook.com>, Wu Yuexin <wuyvexiaoxin@163.com>
 Project-URL: Homepage, https://github.com/Chou-Uken/biofkit
 Project-URL: Issues, https://github.com/Chou-Uken/biofkit/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

