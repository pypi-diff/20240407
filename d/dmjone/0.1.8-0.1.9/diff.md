# Comparing `tmp/dmjone-0.1.8.tar.gz` & `tmp/dmjone-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dmjone-0.1.8.tar", last modified: Sun Apr  7 08:54:05 2024, max compression
+gzip compressed data, was "dmjone-0.1.9.tar", last modified: Sun Apr  7 14:58:32 2024, max compression
```

## Comparing `dmjone-0.1.8.tar` & `dmjone-0.1.9.tar`

### file list

```diff
@@ -1,19 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 08:54:05.143474 dmjone-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-07 08:54:00.000000 dmjone-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-07 08:54:00.000000 dmjone-0.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    44497 2024-04-07 08:54:05.143474 dmjone-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2931 2024-04-07 08:54:00.000000 dmjone-0.1.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-04-07 08:54:00.000000 dmjone-0.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 08:54:05.143474 dmjone-0.1.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 08:54:05.139474 dmjone-0.1.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 08:54:05.143474 dmjone-0.1.8/src/dmjone/
--rw-r--r--   0 runner    (1001) docker     (127)    12688 2024-04-07 08:54:00.000000 dmjone-0.1.8/src/dmjone/StudentManagementSystem.py
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-07 08:54:00.000000 dmjone-0.1.8/src/dmjone/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-07 08:54:00.000000 dmjone-0.1.8/src/dmjone/hello.py
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-07 08:54:00.000000 dmjone-0.1.8/src/dmjone/lab4.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 08:54:05.143474 dmjone-0.1.8/src/dmjone.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    44497 2024-04-07 08:54:05.000000 dmjone-0.1.8/src/dmjone.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-07 08:54:05.000000 dmjone-0.1.8/src/dmjone.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 08:54:05.000000 dmjone-0.1.8/src/dmjone.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-07 08:54:05.000000 dmjone-0.1.8/src/dmjone.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-07 08:54:05.000000 dmjone-0.1.8/src/dmjone.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:58:32.002574 dmjone-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-07 14:58:17.000000 dmjone-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-07 14:58:17.000000 dmjone-0.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    45221 2024-04-07 14:58:32.002574 dmjone-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3666 2024-04-07 14:58:17.000000 dmjone-0.1.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-04-07 14:58:17.000000 dmjone-0.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 14:58:32.002574 dmjone-0.1.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:58:31.994574 dmjone-0.1.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:58:31.998574 dmjone-0.1.9/src/dmjone/
+-rw-r--r--   0 runner    (1001) docker     (127)    12688 2024-04-07 14:58:17.000000 dmjone-0.1.9/src/dmjone/StudentManagementSystem.py
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-07 14:58:17.000000 dmjone-0.1.9/src/dmjone/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-04-07 14:58:17.000000 dmjone-0.1.9/src/dmjone/aarushi_TodoList.py
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-07 14:58:17.000000 dmjone-0.1.9/src/dmjone/hello.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:58:31.998574 dmjone-0.1.9/src/dmjone/kaustuv/
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-07 14:58:17.000000 dmjone-0.1.9/src/dmjone/kaustuv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-07 14:58:17.000000 dmjone-0.1.9/src/dmjone/kaustuv/kaustuv_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-07 14:58:17.000000 dmjone-0.1.9/src/dmjone/kaustuv/kaustuv_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-07 14:58:17.000000 dmjone-0.1.9/src/dmjone/kaustuv_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-07 14:58:17.000000 dmjone-0.1.9/src/dmjone/lab4.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:58:31.998574 dmjone-0.1.9/src/dmjone/lakshika/
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-07 14:58:17.000000 dmjone-0.1.9/src/dmjone/lakshika/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-07 14:58:17.000000 dmjone-0.1.9/src/dmjone/lakshika/calculator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-07 14:58:17.000000 dmjone-0.1.9/src/dmjone/lakshika/lakshika_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-07 14:58:17.000000 dmjone-0.1.9/src/dmjone/lakshika/typecasting.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:58:32.002574 dmjone-0.1.9/src/dmjone.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    45221 2024-04-07 14:58:31.000000 dmjone-0.1.9/src/dmjone.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-07 14:58:31.000000 dmjone-0.1.9/src/dmjone.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 14:58:31.000000 dmjone-0.1.9/src/dmjone.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-07 14:58:31.000000 dmjone-0.1.9/src/dmjone.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-07 14:58:31.000000 dmjone-0.1.9/src/dmjone.egg-info/top_level.txt
```

### Comparing `dmjone-0.1.8/LICENSE` & `dmjone-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `dmjone-0.1.8/PKG-INFO` & `dmjone-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dmjone
-Version: 0.1.8
+Version: 0.1.9
 Summary: Public Welfare initiatives by dmj.one - Educational Initiative
 Author: Divya Mohan, Aarushi Sharma, Anshuman Mohanty, Ashutosh Rana, Jatin Sharma, Kaustuv Sharma, Lakshika Tanwar, Vedansh Sharma
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -695,47 +695,71 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: mysql-connector-python>=8.0.23
 Requires-Dist: Faker>=8.1.1
 
 # dmjone
 
-Welcome to the official Python package for [dmj.one](https://dmj.one) - a platform dedicated to public welfare initiatives with a strong focus on educational projects. Our mission is to provide accessible, innovative, and valuable tools and resources for students, educators, and the general public to promote learning and educational excellence.
+Official Python package for [dmj.one](https://dmj.one) - a platform dedicated to public welfare initiatives with a strong focus on educational projects. Our mission is to provide accessible, innovative, and valuable tools and resources for students, educators, and the general public to promote learning and educational excellence.
 
 ## Installation
-
 Install `dmjone` via pip. Ensure you have Python 3.7 or later installed.
 
 ```bash
 pip install dmjone
 ```
 
-## Features
-
-- **Student Management System**: A simple yet powerful system for managing student records, designed for educational institutions.
-- **Lab Projects**: Access to various educational projects and lab work to facilitate learning and teaching.
-- **Educational Tools**: A collection of tools aimed at enhancing the learning experience.
-
 ## Quick Start
-
 Here's a quick example to get you started with `dmjone`:
 
 ```python
 import dmjone
 
 # Access the Student Management System
 dmjone.projectsms() # Ensure you have MySQL installed on your system if you are running it locally. 
 
-# Run a lab project
-dmjone.lab4()
+# hello there!
+dmjone.hello()
+
+# Get collaborating! - dmjone._your-name_.projectfunction()
+dmjone.aarushi.TodoList()
+dmjone.lakshika.calculator()
+dmjone.kaustuv.calculate_absolute()
 ```
 
-## Documentation
+## Authors
+- **Divya Mohan** - *__init__* - [GitHub](https://github.com/divyamohan1993)
+- **Aarushi Sharma** - [GitHub](https://github.com/letscodeitup)
+- **Anshuman Mohanty** - [GitHub](https://github.com/anshumanmohanty00)
+- **Ashutosh Rana**
+- **Jatin Sharma**
+- **Kaustuv Sharma** - *Contributor* - [GitHub](https://github.com/kaustuvsharma)
+- **Lakshika Tanwar** - *Contributor* - [GitHub](https://github.com/LakshikaTanwar)
+- **Rijul Chaudhary** - [GitHub](https://github.com/Rijul777)
+- **Vedansh Sharma** - [GitHub](https://github.com/Elysian-Reverie)
 
-For comprehensive documentation, visit [dmj.one/docs](https://go.dmj.one/docs). Here, you'll find detailed information on how to make the most of the tools and resources offered by `dmjone`.
+See also the list of [contributors](https://github.com/dmjone/dmjone_pypi/contributors) who participated in this project.
+
+## Features
+- **Student Management System**: A simple yet powerful system for managing student records, designed for educational institutions.
+- **Lab Projects**: Access to various educational projects and lab work to facilitate learning and teaching.
+- **Educational Tools**: A collection of tools aimed at enhancing the learning experience.
+
+## User Collaborations
+### Aarushi Sharma
+- **TodoList**: A simple To-Do List creator.
+### Kaustuv Sharma
+- **Calculate Absolute Value**: Calculate absolute value of a given number
+### Lakshika Tanwar
+- **Typecasting**: Demonstrate Typecasting in python
+- **Calculator**: Calculator to do arithmetic operations on numbers
+
+## Documentation
+<!-- For comprehensive documentation, visit [dmj.one/docs](https://dmj.one/docs). Here, you'll find detailed information on how to make the most of the tools and resources offered by `dmjone`. -->
+For comprehensive documentation, visit [dmj.one](https://dmj.one). Here, you'll find detailed information on how to make the most of the tools and resources offered by `dmjone`.
 
 ## Contributing
 
 Contributions are what make the open-source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.
 
 1. Fork the Project
 2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
@@ -743,34 +767,21 @@
 4. Push to the Branch (`git push origin feature/AmazingFeature`)
 5. Open a Pull Request
 
 ## License
 
 Distributed under the GPL-3.0 License. See `LICENSE` for more information.
 
-## Authors
-
-- **Divya Mohan** - *Initial Work* - [GitHub](https://github.com/divyamohan1993)
-- **Aarushi Sharma** - [GitHub](https://github.com/letscodeitup)
-- **Anshuman Mohanty** - [GitHub](https://github.com/anshumanmohanty00)
-- **Ashutosh Rana**
-- **Jatin Sharma**
-- **Kaustuv Sharma** - [GitHub](https://github.com/kaustuvsharma)
-- **Lakshika Tanwar** - [GitHub](https://github.com/LakshikaTanwar)
-- **Vedansh Sharma** - [GitHub](https://github.com/Elysian-Reverie)
-
-See also the list of [contributors](https://github.com/dmjone/dmjone_pypi/contributors) who participated in this project.
-
 ## Acknowledgements
 
 - Shoolini University
 - All educators and students at Shoolini University
 
 ## Contact
 
-For any queries, please reach out to us via [contact page on dmj.one](https://dmj.one/contact).
+For any queries, please reach out to us via [the message button on dmj.one](https://dmj.one/).
 
 ## Project Links
 
 - **Project Homepage**: [dmj.one](https://dmj.one)
 - **PyPI Repository**: [dmjone on PyPI](https://pypi.org/project/dmjone/)
 - **Source Code**: [GitHub Repository](https://github.com/dmjone/dmjone_pypi)
```

### Comparing `dmjone-0.1.8/README.md` & `dmjone-0.1.9/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,42 +1,66 @@
 # dmjone
 
-Welcome to the official Python package for [dmj.one](https://dmj.one) - a platform dedicated to public welfare initiatives with a strong focus on educational projects. Our mission is to provide accessible, innovative, and valuable tools and resources for students, educators, and the general public to promote learning and educational excellence.
+Official Python package for [dmj.one](https://dmj.one) - a platform dedicated to public welfare initiatives with a strong focus on educational projects. Our mission is to provide accessible, innovative, and valuable tools and resources for students, educators, and the general public to promote learning and educational excellence.
 
 ## Installation
-
 Install `dmjone` via pip. Ensure you have Python 3.7 or later installed.
 
 ```bash
 pip install dmjone
 ```
 
-## Features
-
-- **Student Management System**: A simple yet powerful system for managing student records, designed for educational institutions.
-- **Lab Projects**: Access to various educational projects and lab work to facilitate learning and teaching.
-- **Educational Tools**: A collection of tools aimed at enhancing the learning experience.
-
 ## Quick Start
-
 Here's a quick example to get you started with `dmjone`:
 
 ```python
 import dmjone
 
 # Access the Student Management System
 dmjone.projectsms() # Ensure you have MySQL installed on your system if you are running it locally. 
 
-# Run a lab project
-dmjone.lab4()
+# hello there!
+dmjone.hello()
+
+# Get collaborating! - dmjone._your-name_.projectfunction()
+dmjone.aarushi.TodoList()
+dmjone.lakshika.calculator()
+dmjone.kaustuv.calculate_absolute()
 ```
 
-## Documentation
+## Authors
+- **Divya Mohan** - *__init__* - [GitHub](https://github.com/divyamohan1993)
+- **Aarushi Sharma** - [GitHub](https://github.com/letscodeitup)
+- **Anshuman Mohanty** - [GitHub](https://github.com/anshumanmohanty00)
+- **Ashutosh Rana**
+- **Jatin Sharma**
+- **Kaustuv Sharma** - *Contributor* - [GitHub](https://github.com/kaustuvsharma)
+- **Lakshika Tanwar** - *Contributor* - [GitHub](https://github.com/LakshikaTanwar)
+- **Rijul Chaudhary** - [GitHub](https://github.com/Rijul777)
+- **Vedansh Sharma** - [GitHub](https://github.com/Elysian-Reverie)
 
-For comprehensive documentation, visit [dmj.one/docs](https://go.dmj.one/docs). Here, you'll find detailed information on how to make the most of the tools and resources offered by `dmjone`.
+See also the list of [contributors](https://github.com/dmjone/dmjone_pypi/contributors) who participated in this project.
+
+## Features
+- **Student Management System**: A simple yet powerful system for managing student records, designed for educational institutions.
+- **Lab Projects**: Access to various educational projects and lab work to facilitate learning and teaching.
+- **Educational Tools**: A collection of tools aimed at enhancing the learning experience.
+
+## User Collaborations
+### Aarushi Sharma
+- **TodoList**: A simple To-Do List creator.
+### Kaustuv Sharma
+- **Calculate Absolute Value**: Calculate absolute value of a given number
+### Lakshika Tanwar
+- **Typecasting**: Demonstrate Typecasting in python
+- **Calculator**: Calculator to do arithmetic operations on numbers
+
+## Documentation
+<!-- For comprehensive documentation, visit [dmj.one/docs](https://dmj.one/docs). Here, you'll find detailed information on how to make the most of the tools and resources offered by `dmjone`. -->
+For comprehensive documentation, visit [dmj.one](https://dmj.one). Here, you'll find detailed information on how to make the most of the tools and resources offered by `dmjone`.
 
 ## Contributing
 
 Contributions are what make the open-source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.
 
 1. Fork the Project
 2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
@@ -44,34 +68,21 @@
 4. Push to the Branch (`git push origin feature/AmazingFeature`)
 5. Open a Pull Request
 
 ## License
 
 Distributed under the GPL-3.0 License. See `LICENSE` for more information.
 
-## Authors
-
-- **Divya Mohan** - *Initial Work* - [GitHub](https://github.com/divyamohan1993)
-- **Aarushi Sharma** - [GitHub](https://github.com/letscodeitup)
-- **Anshuman Mohanty** - [GitHub](https://github.com/anshumanmohanty00)
-- **Ashutosh Rana**
-- **Jatin Sharma**
-- **Kaustuv Sharma** - [GitHub](https://github.com/kaustuvsharma)
-- **Lakshika Tanwar** - [GitHub](https://github.com/LakshikaTanwar)
-- **Vedansh Sharma** - [GitHub](https://github.com/Elysian-Reverie)
-
-See also the list of [contributors](https://github.com/dmjone/dmjone_pypi/contributors) who participated in this project.
-
 ## Acknowledgements
 
 - Shoolini University
 - All educators and students at Shoolini University
 
 ## Contact
 
-For any queries, please reach out to us via [contact page on dmj.one](https://dmj.one/contact).
+For any queries, please reach out to us via [the message button on dmj.one](https://dmj.one/).
 
 ## Project Links
 
 - **Project Homepage**: [dmj.one](https://dmj.one)
 - **PyPI Repository**: [dmjone on PyPI](https://pypi.org/project/dmjone/)
 - **Source Code**: [GitHub Repository](https://github.com/dmjone/dmjone_pypi)
```

### Comparing `dmjone-0.1.8/pyproject.toml` & `dmjone-0.1.9/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=42", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dmjone"
-version = "0.1.8"
+version = "0.1.9"
 description = "Public Welfare initiatives by dmj.one - Educational Initiative"
 readme = "README.md"
 license = {file = "LICENSE"}
 # license-files = ["LICENSE"]  # Explicitly list license files if you have multiple or non-standard ones.
 authors = [
     {name = "Divya Mohan"},
     {name = "Aarushi Sharma"},
```

### Comparing `dmjone-0.1.8/src/dmjone/StudentManagementSystem.py` & `dmjone-0.1.9/src/dmjone/StudentManagementSystem.py`

 * *Files identical despite different names*

### Comparing `dmjone-0.1.8/src/dmjone.egg-info/PKG-INFO` & `dmjone-0.1.9/src/dmjone.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dmjone
-Version: 0.1.8
+Version: 0.1.9
 Summary: Public Welfare initiatives by dmj.one - Educational Initiative
 Author: Divya Mohan, Aarushi Sharma, Anshuman Mohanty, Ashutosh Rana, Jatin Sharma, Kaustuv Sharma, Lakshika Tanwar, Vedansh Sharma
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -695,47 +695,71 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: mysql-connector-python>=8.0.23
 Requires-Dist: Faker>=8.1.1
 
 # dmjone
 
-Welcome to the official Python package for [dmj.one](https://dmj.one) - a platform dedicated to public welfare initiatives with a strong focus on educational projects. Our mission is to provide accessible, innovative, and valuable tools and resources for students, educators, and the general public to promote learning and educational excellence.
+Official Python package for [dmj.one](https://dmj.one) - a platform dedicated to public welfare initiatives with a strong focus on educational projects. Our mission is to provide accessible, innovative, and valuable tools and resources for students, educators, and the general public to promote learning and educational excellence.
 
 ## Installation
-
 Install `dmjone` via pip. Ensure you have Python 3.7 or later installed.
 
 ```bash
 pip install dmjone
 ```
 
-## Features
-
-- **Student Management System**: A simple yet powerful system for managing student records, designed for educational institutions.
-- **Lab Projects**: Access to various educational projects and lab work to facilitate learning and teaching.
-- **Educational Tools**: A collection of tools aimed at enhancing the learning experience.
-
 ## Quick Start
-
 Here's a quick example to get you started with `dmjone`:
 
 ```python
 import dmjone
 
 # Access the Student Management System
 dmjone.projectsms() # Ensure you have MySQL installed on your system if you are running it locally. 
 
-# Run a lab project
-dmjone.lab4()
+# hello there!
+dmjone.hello()
+
+# Get collaborating! - dmjone._your-name_.projectfunction()
+dmjone.aarushi.TodoList()
+dmjone.lakshika.calculator()
+dmjone.kaustuv.calculate_absolute()
 ```
 
-## Documentation
+## Authors
+- **Divya Mohan** - *__init__* - [GitHub](https://github.com/divyamohan1993)
+- **Aarushi Sharma** - [GitHub](https://github.com/letscodeitup)
+- **Anshuman Mohanty** - [GitHub](https://github.com/anshumanmohanty00)
+- **Ashutosh Rana**
+- **Jatin Sharma**
+- **Kaustuv Sharma** - *Contributor* - [GitHub](https://github.com/kaustuvsharma)
+- **Lakshika Tanwar** - *Contributor* - [GitHub](https://github.com/LakshikaTanwar)
+- **Rijul Chaudhary** - [GitHub](https://github.com/Rijul777)
+- **Vedansh Sharma** - [GitHub](https://github.com/Elysian-Reverie)
 
-For comprehensive documentation, visit [dmj.one/docs](https://go.dmj.one/docs). Here, you'll find detailed information on how to make the most of the tools and resources offered by `dmjone`.
+See also the list of [contributors](https://github.com/dmjone/dmjone_pypi/contributors) who participated in this project.
+
+## Features
+- **Student Management System**: A simple yet powerful system for managing student records, designed for educational institutions.
+- **Lab Projects**: Access to various educational projects and lab work to facilitate learning and teaching.
+- **Educational Tools**: A collection of tools aimed at enhancing the learning experience.
+
+## User Collaborations
+### Aarushi Sharma
+- **TodoList**: A simple To-Do List creator.
+### Kaustuv Sharma
+- **Calculate Absolute Value**: Calculate absolute value of a given number
+### Lakshika Tanwar
+- **Typecasting**: Demonstrate Typecasting in python
+- **Calculator**: Calculator to do arithmetic operations on numbers
+
+## Documentation
+<!-- For comprehensive documentation, visit [dmj.one/docs](https://dmj.one/docs). Here, you'll find detailed information on how to make the most of the tools and resources offered by `dmjone`. -->
+For comprehensive documentation, visit [dmj.one](https://dmj.one). Here, you'll find detailed information on how to make the most of the tools and resources offered by `dmjone`.
 
 ## Contributing
 
 Contributions are what make the open-source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.
 
 1. Fork the Project
 2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
@@ -743,34 +767,21 @@
 4. Push to the Branch (`git push origin feature/AmazingFeature`)
 5. Open a Pull Request
 
 ## License
 
 Distributed under the GPL-3.0 License. See `LICENSE` for more information.
 
-## Authors
-
-- **Divya Mohan** - *Initial Work* - [GitHub](https://github.com/divyamohan1993)
-- **Aarushi Sharma** - [GitHub](https://github.com/letscodeitup)
-- **Anshuman Mohanty** - [GitHub](https://github.com/anshumanmohanty00)
-- **Ashutosh Rana**
-- **Jatin Sharma**
-- **Kaustuv Sharma** - [GitHub](https://github.com/kaustuvsharma)
-- **Lakshika Tanwar** - [GitHub](https://github.com/LakshikaTanwar)
-- **Vedansh Sharma** - [GitHub](https://github.com/Elysian-Reverie)
-
-See also the list of [contributors](https://github.com/dmjone/dmjone_pypi/contributors) who participated in this project.
-
 ## Acknowledgements
 
 - Shoolini University
 - All educators and students at Shoolini University
 
 ## Contact
 
-For any queries, please reach out to us via [contact page on dmj.one](https://dmj.one/contact).
+For any queries, please reach out to us via [the message button on dmj.one](https://dmj.one/).
 
 ## Project Links
 
 - **Project Homepage**: [dmj.one](https://dmj.one)
 - **PyPI Repository**: [dmjone on PyPI](https://pypi.org/project/dmjone/)
 - **Source Code**: [GitHub Repository](https://github.com/dmjone/dmjone_pypi)
```

