# Comparing `tmp/dmjone-0.1.3.tar.gz` & `tmp/dmjone-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dmjone-0.1.3.tar", last modified: Sun Apr  7 07:05:34 2024, max compression
+gzip compressed data, was "dmjone-0.1.4.tar", last modified: Sun Apr  7 07:34:23 2024, max compression
```

## Comparing `dmjone-0.1.3.tar` & `dmjone-0.1.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 07:05:34.070443 dmjone-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-07 07:05:22.000000 dmjone-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-07 07:05:22.000000 dmjone-0.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    41708 2024-04-07 07:05:34.070443 dmjone-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-07 07:05:22.000000 dmjone-0.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-04-07 07:05:22.000000 dmjone-0.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 07:05:34.070443 dmjone-0.1.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 07:05:34.066443 dmjone-0.1.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 07:05:34.070443 dmjone-0.1.3/src/dmjone/
--rw-r--r--   0 runner    (1001) docker     (127)    12482 2024-04-07 07:05:22.000000 dmjone-0.1.3/src/dmjone/StudentManagementSystem.py
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-07 07:05:22.000000 dmjone-0.1.3/src/dmjone/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-07 07:05:22.000000 dmjone-0.1.3/src/dmjone/lab4.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 07:05:34.070443 dmjone-0.1.3/src/dmjone.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    41708 2024-04-07 07:05:34.000000 dmjone-0.1.3/src/dmjone.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-07 07:05:34.000000 dmjone-0.1.3/src/dmjone.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 07:05:34.000000 dmjone-0.1.3/src/dmjone.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-07 07:05:34.000000 dmjone-0.1.3/src/dmjone.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-07 07:05:34.000000 dmjone-0.1.3/src/dmjone.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 07:34:23.549579 dmjone-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-07 07:34:11.000000 dmjone-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-07 07:34:11.000000 dmjone-0.1.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    44497 2024-04-07 07:34:23.549579 dmjone-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2931 2024-04-07 07:34:11.000000 dmjone-0.1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-04-07 07:34:11.000000 dmjone-0.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 07:34:23.549579 dmjone-0.1.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 07:34:23.549579 dmjone-0.1.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 07:34:23.549579 dmjone-0.1.4/src/dmjone/
+-rw-r--r--   0 runner    (1001) docker     (127)    12482 2024-04-07 07:34:11.000000 dmjone-0.1.4/src/dmjone/StudentManagementSystem.py
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-07 07:34:11.000000 dmjone-0.1.4/src/dmjone/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-07 07:34:11.000000 dmjone-0.1.4/src/dmjone/lab4.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 07:34:23.549579 dmjone-0.1.4/src/dmjone.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    44497 2024-04-07 07:34:23.000000 dmjone-0.1.4/src/dmjone.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-07 07:34:23.000000 dmjone-0.1.4/src/dmjone.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 07:34:23.000000 dmjone-0.1.4/src/dmjone.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-07 07:34:23.000000 dmjone-0.1.4/src/dmjone.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-07 07:34:23.000000 dmjone-0.1.4/src/dmjone.egg-info/top_level.txt
```

### Comparing `dmjone-0.1.3/LICENSE` & `dmjone-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dmjone-0.1.3/PKG-INFO` & `dmjone-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: dmjone
-Version: 0.1.3
+Version: 0.1.4
 Summary: Public Welfare initiatives by dmj.one - Educational Initiative
-Author: Divya Mohan, Aarushi Sharma, Anshuman Mohanty, Ashutosh Rana, Jatin Sharma, Lakshika Tanwar, Vedansh Sharma
+Author: Divya Mohan, Aarushi Sharma, Anshuman Mohanty, Ashutosh Rana, Jatin Sharma, Kaustuv Sharma, Lakshika Tanwar, Vedansh Sharma
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
         
@@ -693,10 +693,84 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: mysql-connector-python>=8.0.23
 Requires-Dist: Faker>=8.1.1
 
-# dmjone_pypi
-## Install using pip install dmjone
-Call using dmjone.projectsms()
+# dmjone
+
+Welcome to the official Python package for [dmj.one](https://dmj.one) - a platform dedicated to public welfare initiatives with a strong focus on educational projects. Our mission is to provide accessible, innovative, and valuable tools and resources for students, educators, and the general public to promote learning and educational excellence.
+
+## Installation
+
+Install `dmjone` via pip. Ensure you have Python 3.7 or later installed.
+
+```bash
+pip install dmjone
+```
+
+## Features
+
+- **Student Management System**: A simple yet powerful system for managing student records, designed for educational institutions.
+- **Lab Projects**: Access to various educational projects and lab work to facilitate learning and teaching.
+- **Educational Tools**: A collection of tools aimed at enhancing the learning experience.
+
+## Quick Start
+
+Here's a quick example to get you started with `dmjone`:
+
+```python
+import dmjone
+
+# Access the Student Management System
+dmjone.projectsms() # Ensure you have MySQL installed on your system if you are running it locally. 
+
+# Run a lab project
+dmjone.lab4()
+```
+
+## Documentation
+
+For comprehensive documentation, visit [dmj.one/docs](https://go.dmj.one/docs). Here, you'll find detailed information on how to make the most of the tools and resources offered by `dmjone`.
+
+## Contributing
+
+Contributions are what make the open-source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.
+
+1. Fork the Project
+2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
+3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
+4. Push to the Branch (`git push origin feature/AmazingFeature`)
+5. Open a Pull Request
+
+## License
+
+Distributed under the GPL-3.0 License. See `LICENSE` for more information.
+
+## Authors
+
+- **Divya Mohan** - *Initial Work* - [GitHub](https://github.com/divyamohan1993)
+- **Aarushi Sharma** - [GitHub](https://github.com/letscodeitup)
+- **Anshuman Mohanty** - [GitHub](https://github.com/anshumanmohanty00)
+- **Ashutosh Rana**
+- **Jatin Sharma**
+- **Kaustuv Sharma** - [GitHub](https://github.com/kaustuvsharma)
+- **Lakshika Tanwar** - [GitHub](https://github.com/LakshikaTanwar)
+- **Vedansh Sharma** - [GitHub](https://github.com/Elysian-Reverie)
+
+See also the list of [contributors](https://github.com/dmjone/dmjone_pypi/contributors) who participated in this project.
+
+## Acknowledgements
+
+- Shoolini University
+- All educators and students at Shoolini University
+
+## Contact
+
+For any queries, please reach out to us via [contact page on dmj.one](https://dmj.one/contact).
+
+## Project Links
+
+- **Project Homepage**: [dmj.one](https://dmj.one)
+- **PyPI Repository**: [dmjone on PyPI](https://pypi.org/project/dmjone/)
+- **Source Code**: [GitHub Repository](https://github.com/dmjone/dmjone_pypi)
```

### Comparing `dmjone-0.1.3/pyproject.toml` & `dmjone-0.1.4/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 [build-system]
 requires = ["setuptools>=42", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dmjone"
-version = "0.1.3"
+version = "0.1.4"
 description = "Public Welfare initiatives by dmj.one - Educational Initiative"
 readme = "README.md"
 license = {file = "LICENSE"}
 # license-files = ["LICENSE"]  # Explicitly list license files if you have multiple or non-standard ones.
 authors = [
     {name = "Divya Mohan"},
     {name = "Aarushi Sharma"},
     {name = "Anshuman Mohanty"},
     {name = "Ashutosh Rana"},
     {name = "Jatin Sharma"},
+    {name = "Kaustuv Sharma"},
     {name = "Lakshika Tanwar"},
     {name = "Vedansh Sharma"},
 ]
 keywords = ["education", "dmjone", "dmj.one", "shooliniuniversity", "shoolini"]
 classifiers = [
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.7",
```

### Comparing `dmjone-0.1.3/src/dmjone/StudentManagementSystem.py` & `dmjone-0.1.4/src/dmjone/StudentManagementSystem.py`

 * *Files identical despite different names*

### Comparing `dmjone-0.1.3/src/dmjone.egg-info/PKG-INFO` & `dmjone-0.1.4/src/dmjone.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: dmjone
-Version: 0.1.3
+Version: 0.1.4
 Summary: Public Welfare initiatives by dmj.one - Educational Initiative
-Author: Divya Mohan, Aarushi Sharma, Anshuman Mohanty, Ashutosh Rana, Jatin Sharma, Lakshika Tanwar, Vedansh Sharma
+Author: Divya Mohan, Aarushi Sharma, Anshuman Mohanty, Ashutosh Rana, Jatin Sharma, Kaustuv Sharma, Lakshika Tanwar, Vedansh Sharma
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
         
@@ -693,10 +693,84 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: mysql-connector-python>=8.0.23
 Requires-Dist: Faker>=8.1.1
 
-# dmjone_pypi
-## Install using pip install dmjone
-Call using dmjone.projectsms()
+# dmjone
+
+Welcome to the official Python package for [dmj.one](https://dmj.one) - a platform dedicated to public welfare initiatives with a strong focus on educational projects. Our mission is to provide accessible, innovative, and valuable tools and resources for students, educators, and the general public to promote learning and educational excellence.
+
+## Installation
+
+Install `dmjone` via pip. Ensure you have Python 3.7 or later installed.
+
+```bash
+pip install dmjone
+```
+
+## Features
+
+- **Student Management System**: A simple yet powerful system for managing student records, designed for educational institutions.
+- **Lab Projects**: Access to various educational projects and lab work to facilitate learning and teaching.
+- **Educational Tools**: A collection of tools aimed at enhancing the learning experience.
+
+## Quick Start
+
+Here's a quick example to get you started with `dmjone`:
+
+```python
+import dmjone
+
+# Access the Student Management System
+dmjone.projectsms() # Ensure you have MySQL installed on your system if you are running it locally. 
+
+# Run a lab project
+dmjone.lab4()
+```
+
+## Documentation
+
+For comprehensive documentation, visit [dmj.one/docs](https://go.dmj.one/docs). Here, you'll find detailed information on how to make the most of the tools and resources offered by `dmjone`.
+
+## Contributing
+
+Contributions are what make the open-source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.
+
+1. Fork the Project
+2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
+3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
+4. Push to the Branch (`git push origin feature/AmazingFeature`)
+5. Open a Pull Request
+
+## License
+
+Distributed under the GPL-3.0 License. See `LICENSE` for more information.
+
+## Authors
+
+- **Divya Mohan** - *Initial Work* - [GitHub](https://github.com/divyamohan1993)
+- **Aarushi Sharma** - [GitHub](https://github.com/letscodeitup)
+- **Anshuman Mohanty** - [GitHub](https://github.com/anshumanmohanty00)
+- **Ashutosh Rana**
+- **Jatin Sharma**
+- **Kaustuv Sharma** - [GitHub](https://github.com/kaustuvsharma)
+- **Lakshika Tanwar** - [GitHub](https://github.com/LakshikaTanwar)
+- **Vedansh Sharma** - [GitHub](https://github.com/Elysian-Reverie)
+
+See also the list of [contributors](https://github.com/dmjone/dmjone_pypi/contributors) who participated in this project.
+
+## Acknowledgements
+
+- Shoolini University
+- All educators and students at Shoolini University
+
+## Contact
+
+For any queries, please reach out to us via [contact page on dmj.one](https://dmj.one/contact).
+
+## Project Links
+
+- **Project Homepage**: [dmj.one](https://dmj.one)
+- **PyPI Repository**: [dmjone on PyPI](https://pypi.org/project/dmjone/)
+- **Source Code**: [GitHub Repository](https://github.com/dmjone/dmjone_pypi)
```

