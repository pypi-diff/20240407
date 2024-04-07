# Comparing `tmp/dmjone-0.1.9.4.tar.gz` & `tmp/dmjone-0.1.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dmjone-0.1.9.4.tar", last modified: Sun Apr  7 15:35:22 2024, max compression
+gzip compressed data, was "dmjone-0.1.9.7.tar", last modified: Sun Apr  7 19:49:57 2024, max compression
```

## Comparing `dmjone-0.1.9.4.tar` & `dmjone-0.1.9.7.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:35:22.370972 dmjone-0.1.9.4/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-07 15:35:13.000000 dmjone-0.1.9.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-07 15:35:13.000000 dmjone-0.1.9.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    45223 2024-04-07 15:35:22.370972 dmjone-0.1.9.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3666 2024-04-07 15:35:13.000000 dmjone-0.1.9.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-04-07 15:35:13.000000 dmjone-0.1.9.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 15:35:22.370972 dmjone-0.1.9.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:35:22.362972 dmjone-0.1.9.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:35:22.366972 dmjone-0.1.9.4/src/dmjone/
--rw-r--r--   0 runner    (1001) docker     (127)    12688 2024-04-07 15:35:13.000000 dmjone-0.1.9.4/src/dmjone/StudentManagementSystem.py
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-07 15:35:13.000000 dmjone-0.1.9.4/src/dmjone/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:35:22.366972 dmjone-0.1.9.4/src/dmjone/aarushi/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-07 15:35:13.000000 dmjone-0.1.9.4/src/dmjone/aarushi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-04-07 15:35:13.000000 dmjone-0.1.9.4/src/dmjone/aarushi/aarushi_todolist.py
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-07 15:35:13.000000 dmjone-0.1.9.4/src/dmjone/hello.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:35:22.366972 dmjone-0.1.9.4/src/dmjone/kaustuv/
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-07 15:35:13.000000 dmjone-0.1.9.4/src/dmjone/kaustuv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-07 15:35:13.000000 dmjone-0.1.9.4/src/dmjone/kaustuv/kaustuv_common.py
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-07 15:35:13.000000 dmjone-0.1.9.4/src/dmjone/kaustuv/kaustuv_project.py
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-07 15:35:13.000000 dmjone-0.1.9.4/src/dmjone/lab4.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:35:22.370972 dmjone-0.1.9.4/src/dmjone/lakshika/
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-07 15:35:13.000000 dmjone-0.1.9.4/src/dmjone/lakshika/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-07 15:35:13.000000 dmjone-0.1.9.4/src/dmjone/lakshika/calculator.py
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-07 15:35:13.000000 dmjone-0.1.9.4/src/dmjone/lakshika/lakshika_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-07 15:35:13.000000 dmjone-0.1.9.4/src/dmjone/lakshika/typecasting.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:35:22.370972 dmjone-0.1.9.4/src/dmjone.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    45223 2024-04-07 15:35:22.000000 dmjone-0.1.9.4/src/dmjone.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-07 15:35:22.000000 dmjone-0.1.9.4/src/dmjone.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 15:35:22.000000 dmjone-0.1.9.4/src/dmjone.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-07 15:35:22.000000 dmjone-0.1.9.4/src/dmjone.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-07 15:35:22.000000 dmjone-0.1.9.4/src/dmjone.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 19:49:57.325723 dmjone-0.1.9.7/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-07 19:49:52.000000 dmjone-0.1.9.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-07 19:49:52.000000 dmjone-0.1.9.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    49537 2024-04-07 19:49:57.321723 dmjone-0.1.9.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7541 2024-04-07 19:49:52.000000 dmjone-0.1.9.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-04-07 19:49:52.000000 dmjone-0.1.9.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 19:49:57.325723 dmjone-0.1.9.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 19:49:57.317723 dmjone-0.1.9.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 19:49:57.321723 dmjone-0.1.9.7/src/dmjone/
+-rw-r--r--   0 runner    (1001) docker     (127)    12688 2024-04-07 19:49:52.000000 dmjone-0.1.9.7/src/dmjone/StudentManagementSystem.py
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-07 19:49:52.000000 dmjone-0.1.9.7/src/dmjone/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 19:49:57.321723 dmjone-0.1.9.7/src/dmjone/aarushi/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-07 19:49:52.000000 dmjone-0.1.9.7/src/dmjone/aarushi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-04-07 19:49:52.000000 dmjone-0.1.9.7/src/dmjone/aarushi/aarushi_todolist.py
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-07 19:49:52.000000 dmjone-0.1.9.7/src/dmjone/hello.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 19:49:57.321723 dmjone-0.1.9.7/src/dmjone/kaustuv/
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-07 19:49:52.000000 dmjone-0.1.9.7/src/dmjone/kaustuv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-07 19:49:52.000000 dmjone-0.1.9.7/src/dmjone/kaustuv/kaustuv_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-07 19:49:52.000000 dmjone-0.1.9.7/src/dmjone/kaustuv/kaustuv_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-07 19:49:52.000000 dmjone-0.1.9.7/src/dmjone/lab4.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 19:49:57.321723 dmjone-0.1.9.7/src/dmjone/lakshika/
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-07 19:49:52.000000 dmjone-0.1.9.7/src/dmjone/lakshika/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-07 19:49:52.000000 dmjone-0.1.9.7/src/dmjone/lakshika/calculator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-07 19:49:52.000000 dmjone-0.1.9.7/src/dmjone/lakshika/lakshika_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-07 19:49:52.000000 dmjone-0.1.9.7/src/dmjone/lakshika/typecasting.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 19:49:57.321723 dmjone-0.1.9.7/src/dmjone.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    49537 2024-04-07 19:49:57.000000 dmjone-0.1.9.7/src/dmjone.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-07 19:49:57.000000 dmjone-0.1.9.7/src/dmjone.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 19:49:57.000000 dmjone-0.1.9.7/src/dmjone.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-07 19:49:57.000000 dmjone-0.1.9.7/src/dmjone.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-07 19:49:57.000000 dmjone-0.1.9.7/src/dmjone.egg-info/top_level.txt
```

### Comparing `dmjone-0.1.9.4/LICENSE` & `dmjone-0.1.9.7/LICENSE`

 * *Files identical despite different names*

### Comparing `dmjone-0.1.9.4/PKG-INFO` & `dmjone-0.1.9.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: dmjone
-Version: 0.1.9.4
-Summary: Public Welfare initiatives by dmj.one - Educational Initiative
-Author: Divya Mohan, Aarushi Sharma, Anshuman Mohanty, Ashutosh Rana, Jatin Sharma, Kaustuv Sharma, Lakshika Tanwar, Vedansh Sharma
+Version: 0.1.9.7
+Summary: A suite of public welfare and educational tools developed by dmj.one, focusing on accessibility and innovation in learning resources.
+Author-email: Divya Mohan <contact@dmj.one>, Aarushi Sharma <aarushi@dmj.one>, Kaustuv Sharma <kaustuv@dmj.one>, Lakshika Tanwar <lakshika@dmj.one>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
         
@@ -675,113 +675,178 @@
         into proprietary programs.  If your program is a subroutine library, you
         may consider it more useful to permit linking proprietary applications with
         the library.  If this is what you want to do, use the GNU Lesser General
         Public License instead of this License.  But first, please read
         <https://www.gnu.org/licenses/why-not-lgpl.html>.
         
 Project-URL: homepage, https://dmj.one
-Project-URL: repository, https://github.com/dmjone/
-Project-URL: documentation, https://dmj.one/
-Keywords: education,dmjone,dmj.one,shooliniuniversity,shoolini
+Project-URL: repository, https://github.com/dmjone/dmjone_pypi
+Project-URL: bug_tracker, https://github.com/dmjone/dmjone_pypi/issues
+Keywords: education,public welfare initiative,learning resources,shoolini university,dmjone
+Classifier: Development Status :: 4 - Beta
+Classifier: Environment :: Web Environment
+Classifier: Intended Audience :: Education
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
-Classifier: Operating System :: OS Independent
-Classifier: Intended Audience :: Education
 Classifier: Topic :: Education
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: mysql-connector-python>=8.0.23
 Requires-Dist: Faker>=8.1.1
+Requires-Dist: Flask>=1.1.2
+Requires-Dist: requests>=2.25.1
+Provides-Extra: testing
+Requires-Dist: pytest>=6.2.4; extra == "testing"
+Requires-Dist: coverage>=5.5; extra == "testing"
 
 # dmjone
 
 Official Python package for [dmj.one](https://dmj.one) - a platform dedicated to public welfare initiatives with a strong focus on educational projects. Our mission is to provide accessible, innovative, and valuable tools and resources for students, educators, and the general public to promote learning and educational excellence.
 
+### Setting Up Your Environment
+Before you start, set up a development environment. Ensure you have Python 3.0 or later installed.
+
 ## Installation
 Install `dmjone` via pip. Ensure you have Python 3.7 or later installed.
 
 ```bash
 pip install dmjone
 ```
 
 ## Quick Start
 Here's a quick example to get you started with `dmjone`:
 
 ```python
+# Method 1 - Import entire library 
 import dmjone
+# You can now use all functionalities available in the package library.
 
-# Access the Student Management System
-dmjone.projectsms() # Ensure you have MySQL installed on your system if you are running it locally. 
+# Method 2 - Import your *own* specific code or functionalities
+from dmjone import kaustuv as ks
+# Now you can access specific functions of ks by calling ks.specific_function_name()
 
-# hello there!
+# Hello World ?
 dmjone.hello()
 
-# Get collaborating! - dmjone._your-name_.projectfunction()
-dmjone.aarushi.TodoList()
+# Get collaborating! Reserve your name at - dmjone._your-name_.function()
+dmjone.aarushi.todolist()
 dmjone.lakshika.calculator()
+dmjone.jatin.demoName()
 dmjone.kaustuv.calculate_absolute()
+dmjone.subhojeet.packagebySubhojeet()
 ```
 
-## Authors
-- **Divya Mohan** - *__init__* - [GitHub](https://github.com/divyamohan1993)
-- **Aarushi Sharma** - [GitHub](https://github.com/letscodeitup)
-- **Anshuman Mohanty** - [GitHub](https://github.com/anshumanmohanty00)
-- **Ashutosh Rana**
-- **Jatin Sharma**
-- **Kaustuv Sharma** - *Contributor* - [GitHub](https://github.com/kaustuvsharma)
-- **Lakshika Tanwar** - *Contributor* - [GitHub](https://github.com/LakshikaTanwar)
-- **Rijul Chaudhary** - [GitHub](https://github.com/Rijul777)
-- **Vedansh Sharma** - [GitHub](https://github.com/Elysian-Reverie)
+## Example Usage
+Example 1
+```python
+import dmjone
+dmjone.aarushi.todolist()
+```
+Example 2
+```python
+# Access the Student Management System, A Project by Students
+import dmjone
+dmjone.projectsms() # Ensure you have MySQL installed on your system if you are running it locally.
+```
+Example 3
+```python
+from dmjone import kaustuv as ks
+ks.check_all_true()
+```
 
-See also the list of [contributors](https://github.com/dmjone/dmjone_pypi/contributors) who participated in this project.
+## Notable User Contributions and Collaborations
+#### Aarushi Sharma
+- **TodoList**: A simple To-Do List creator.
+#### Kaustuv Sharma
+- **Calculate Absolute Value**: Calculate absolute value of a given number
+#### Lakshika Tanwar
+- **Typecasting**: Demonstrate Typecasting in python
+- **Calculator**: Calculator to do arithmetic operations on numbers
 
-## Features
+## Highlighted Features and Collaborations
 - **Student Management System**: A simple yet powerful system for managing student records, designed for educational institutions.
 - **Lab Projects**: Access to various educational projects and lab work to facilitate learning and teaching.
 - **Educational Tools**: A collection of tools aimed at enhancing the learning experience.
 
-## User Collaborations
-### Aarushi Sharma
-- **TodoList**: A simple To-Do List creator.
-### Kaustuv Sharma
-- **Calculate Absolute Value**: Calculate absolute value of a given number
-### Lakshika Tanwar
-- **Typecasting**: Demonstrate Typecasting in python
-- **Calculator**: Calculator to do arithmetic operations on numbers
+## Authors
+- **Divya Mohan** - *__init__* - [GitHub](https://github.com/divyamohan1993) | **Lakshika Tanwar** - *Top Contributor* - [GitHub](https://github.com/LakshikaTanwar) | **Aarushi Sharma** - *Contributor* - [GitHub](https://github.com/letscodeitup) | **Kaustuv Sharma** - *Contributor* - [GitHub](https://github.com/kaustuvsharma) | **Anshuman Mohanty** - [GitHub](https://github.com/anshumanmohanty00) | **Ashutosh Rana** | **Jatin Sharma** | **Rijul Chaudhary** - [GitHub](https://github.com/Rijul777) | **Vedansh Sharma** - [GitHub](https://github.com/Elysian-Reverie) | Subhojeet Ghosh [GitHub](https://github.com/subhojeetghosh123)
 
-## Documentation
-<!-- For comprehensive documentation, visit [dmj.one/docs](https://dmj.one/docs). Here, you'll find detailed information on how to make the most of the tools and resources offered by `dmjone`. -->
-For comprehensive documentation, visit [dmj.one](https://dmj.one). Here, you'll find detailed information on how to make the most of the tools and resources offered by `dmjone`.
+See also the list of [contributors](https://github.com/dmjone/dmjone_pypi/contributors) who participated in this project.
 
-## Contributing
+## How To Contribute
 
-Contributions are what make the open-source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.
+We thank you for your interest in contributing to `dmjone`! 🎉 Your efforts make a big difference. Whether you're fixing a bug, adding a feature, or improving documentation, we appreciate your help. Here’s how to contribute in a friendly and easy way:
 
-1. Fork the Project
-2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
-3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
-4. Push to the Branch (`git push origin feature/AmazingFeature`)
-5. Open a Pull Request
+#### Found a solution to a problem? Let's get you started!
 
-## License
+1. **Find something to work on**: Look through the [GitHub issues](https://github.com/dmjone/dmjone_pypi/issues) for something that interests you or open a new issue to suggest improvements or report bugs.
 
-Distributed under the GPL-3.0 License. See `LICENSE` for more information.
+#### Making Changes
 
-## Acknowledgements
+##### Using GitHub Web Interface
+For small changes, like fixing typos or small code snippets, using the GitHub web interface is the easiest way:
+
+1. Navigate to the file you want to edit on the [dmjone GitHub Repo](https://github.com/dmjone/dmjone_pypi).
+2. Click the pencil icon (Edit this file) to start making changes.
+3. After making changes, describe what you did and why in the **Commit changes** box.
+4. Choose the option to **Create a new branch for this commit and start a pull request**. Name it appropriately, like `fix/typo-in-readme`.
+5. Click **Propose changes** and then **Create pull request** on the next page.
+
+##### Using Command Line
+For larger changes or new features, you might prefer working locally:
+
+1. **Fork the Repository**: Click the "Fork" button on the top right of the [dmjone GitHub Repo](https://github.com/dmjone/dmjone_pypi) page to create your copy.
+2. **Clone Your Fork**: `git clone https://github.com/your-username/dmjone_pypi.git` to clone the project to your computer.
+3. **Create a Branch**: Switch to your clone and use `git checkout -b feature/YourFeatureName` or `fix/YourBugFix` to create a new branch.
+4. **Make Your Changes**: Add your changes using your favorite editor or IDE.
+5. **Commit Your Changes**: Use `git commit -m 'A brief description of your changes'` to save your work.
+6. **Push to GitHub**: Use `git push origin feature/YourFeatureName` to upload your changes to your GitHub fork.
+7. **Open a Pull Request**: Go to your fork on GitHub and press the "New pull request" button. Describe your changes and submit!
+
+### Before You Submit
+
+- **Review Your Changes**: Double-check your changes and make sure everything works as expected. Try to keep your changes simple and focused on solving a single problem.
+- **Follow the Style Guide**: Make sure your contributions follow the existing code style to keep the project organized.
+- **Update Tests**: If you're adding a new feature, consider adding tests to support it.
+
+### Submitting Your Contribution
+
+Once you’re ready to submit, open a pull request with your changes. Provide a clear description of the problem and solution, including any relevant issue numbers.
+
+### After You Submit
 
+- **Patience is Key**: Maintainers will review your contribution and may suggest changes. This is a normal part of the process; feedback helps improve the project.
+- **Stay Engaged**: Check back in case the maintainers have questions or feedback. Your pull request may spark a conversation.
+
+### And That's It!
+
+You've contributed to `dmjone`! We're grateful for your help in making this project better. Remember, contributing is not just about code; every bit of documentation, bug reports, or even suggestions are valuable to us.
+
+Thank you for being part of our open-source community! Let the world be educated!🌟
+
+## Acknowledgements
 - Shoolini University
 - All educators and students at Shoolini University
 
 ## Contact
-
 For any queries, please reach out to us via [the message button on dmj.one](https://dmj.one/).
 
+## Documentation
+<!-- For comprehensive documentation, visit [dmj.one/docs](https://dmj.one/docs). Here, you'll find detailed information on how to make the most of the tools and resources offered by `dmjone`. -->
+For comprehensive documentation, visit [dmj.one](https://dmj.one). Here, you'll find detailed information on how to make the most of the tools and resources offered by `dmjone`.
+
+## License
+Distributed under the GPL-3.0 License. See `LICENSE` for more information.
+
 ## Project Links
 
 - **Project Homepage**: [dmj.one](https://dmj.one)
 - **PyPI Repository**: [dmjone on PyPI](https://pypi.org/project/dmjone/)
 - **Source Code**: [GitHub Repository](https://github.com/dmjone/dmjone_pypi)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `dmjone-0.1.9.4/pyproject.toml` & `dmjone-0.1.9.7/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,43 +1,52 @@
 [build-system]
 requires = ["setuptools>=42", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dmjone"
-version = "0.1.9.4"
-description = "Public Welfare initiatives by dmj.one - Educational Initiative"
+version = "0.1.9.7"
+description = "A suite of public welfare and educational tools developed by dmj.one, focusing on accessibility and innovation in learning resources."
 readme = "README.md"
 license = {file = "LICENSE"}
-# license-files = ["LICENSE"]  # Explicitly list license files if you have multiple or non-standard ones.
 authors = [
-    {name = "Divya Mohan"},
-    {name = "Aarushi Sharma"},
-    {name = "Anshuman Mohanty"},
-    {name = "Ashutosh Rana"},
-    {name = "Jatin Sharma"},
-    {name = "Kaustuv Sharma"},
-    {name = "Lakshika Tanwar"},
-    {name = "Vedansh Sharma"},
+    {name = "Divya Mohan", email = "contact@dmj.one"},
+    {name = "Aarushi Sharma", email = "aarushi@dmj.one"},
+    {name = "Kaustuv Sharma", email = "kaustuv@dmj.one"},
+    {name = "Lakshika Tanwar", email = "lakshika@dmj.one"},    
 ]
-keywords = ["education", "dmjone", "dmj.one", "shooliniuniversity", "shoolini"]
+keywords = ["education", "public welfare initiative", "learning resources", "shoolini university", "dmjone"]
 classifiers = [
+    "Development Status :: 4 - Beta",
+    "Environment :: Web Environment",
+    #"Framework :: Flask",
+    "Intended Audience :: Education",
+    "Intended Audience :: Developers",
+    "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
+    "Natural Language :: English",
+    "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
-    "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
-    "Operating System :: OS Independent",
-    "Intended Audience :: Education",
     "Topic :: Education",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
-requires-python = ">=3.7"  # Specify the Python version requirement.
+requires-python = ">=3.7"
 dependencies = [
     "mysql-connector-python>=8.0.23",
-    "Faker>=8.1.1"
+    "Faker>=8.1.1",
+    "Flask>=1.1.2",  # Flask is used for web components.
+    "requests>=2.25.1"  # For any HTTP requests to external services or APIs.
+]
+
+[project.optional-dependencies]
+testing = [
+    "pytest>=6.2.4",
+    "coverage>=5.5"
 ]
 
 [project.urls]
 homepage = "https://dmj.one"
-repository = "https://github.com/dmjone/"
-documentation = "https://dmj.one/"  # Add a URL for your project's documentation if available.
+repository = "https://github.com/dmjone/dmjone_pypi"
+# documentation = "https://dmj.one/docs"  # Assuming documentation is hosted under a `/docs` path.
+bug_tracker = "https://github.com/dmjone/dmjone_pypi/issues"  # Direct link to your project's issue tracker.
```

### Comparing `dmjone-0.1.9.4/src/dmjone/StudentManagementSystem.py` & `dmjone-0.1.9.7/src/dmjone/StudentManagementSystem.py`

 * *Files identical despite different names*

### Comparing `dmjone-0.1.9.4/src/dmjone/__init__.py` & `dmjone-0.1.9.7/src/dmjone/__init__.py`

 * *Files identical despite different names*

### Comparing `dmjone-0.1.9.4/src/dmjone/aarushi/aarushi_todolist.py` & `dmjone-0.1.9.7/src/dmjone/aarushi/aarushi_todolist.py`

 * *Files identical despite different names*

### Comparing `dmjone-0.1.9.4/src/dmjone/lakshika/lakshika_functions.py` & `dmjone-0.1.9.7/src/dmjone/lakshika/lakshika_functions.py`

 * *Files identical despite different names*

### Comparing `dmjone-0.1.9.4/src/dmjone.egg-info/PKG-INFO` & `dmjone-0.1.9.7/src/dmjone.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: dmjone
-Version: 0.1.9.4
-Summary: Public Welfare initiatives by dmj.one - Educational Initiative
-Author: Divya Mohan, Aarushi Sharma, Anshuman Mohanty, Ashutosh Rana, Jatin Sharma, Kaustuv Sharma, Lakshika Tanwar, Vedansh Sharma
+Version: 0.1.9.7
+Summary: A suite of public welfare and educational tools developed by dmj.one, focusing on accessibility and innovation in learning resources.
+Author-email: Divya Mohan <contact@dmj.one>, Aarushi Sharma <aarushi@dmj.one>, Kaustuv Sharma <kaustuv@dmj.one>, Lakshika Tanwar <lakshika@dmj.one>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
         
@@ -675,113 +675,178 @@
         into proprietary programs.  If your program is a subroutine library, you
         may consider it more useful to permit linking proprietary applications with
         the library.  If this is what you want to do, use the GNU Lesser General
         Public License instead of this License.  But first, please read
         <https://www.gnu.org/licenses/why-not-lgpl.html>.
         
 Project-URL: homepage, https://dmj.one
-Project-URL: repository, https://github.com/dmjone/
-Project-URL: documentation, https://dmj.one/
-Keywords: education,dmjone,dmj.one,shooliniuniversity,shoolini
+Project-URL: repository, https://github.com/dmjone/dmjone_pypi
+Project-URL: bug_tracker, https://github.com/dmjone/dmjone_pypi/issues
+Keywords: education,public welfare initiative,learning resources,shoolini university,dmjone
+Classifier: Development Status :: 4 - Beta
+Classifier: Environment :: Web Environment
+Classifier: Intended Audience :: Education
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
-Classifier: Operating System :: OS Independent
-Classifier: Intended Audience :: Education
 Classifier: Topic :: Education
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: mysql-connector-python>=8.0.23
 Requires-Dist: Faker>=8.1.1
+Requires-Dist: Flask>=1.1.2
+Requires-Dist: requests>=2.25.1
+Provides-Extra: testing
+Requires-Dist: pytest>=6.2.4; extra == "testing"
+Requires-Dist: coverage>=5.5; extra == "testing"
 
 # dmjone
 
 Official Python package for [dmj.one](https://dmj.one) - a platform dedicated to public welfare initiatives with a strong focus on educational projects. Our mission is to provide accessible, innovative, and valuable tools and resources for students, educators, and the general public to promote learning and educational excellence.
 
+### Setting Up Your Environment
+Before you start, set up a development environment. Ensure you have Python 3.0 or later installed.
+
 ## Installation
 Install `dmjone` via pip. Ensure you have Python 3.7 or later installed.
 
 ```bash
 pip install dmjone
 ```
 
 ## Quick Start
 Here's a quick example to get you started with `dmjone`:
 
 ```python
+# Method 1 - Import entire library 
 import dmjone
+# You can now use all functionalities available in the package library.
 
-# Access the Student Management System
-dmjone.projectsms() # Ensure you have MySQL installed on your system if you are running it locally. 
+# Method 2 - Import your *own* specific code or functionalities
+from dmjone import kaustuv as ks
+# Now you can access specific functions of ks by calling ks.specific_function_name()
 
-# hello there!
+# Hello World ?
 dmjone.hello()
 
-# Get collaborating! - dmjone._your-name_.projectfunction()
-dmjone.aarushi.TodoList()
+# Get collaborating! Reserve your name at - dmjone._your-name_.function()
+dmjone.aarushi.todolist()
 dmjone.lakshika.calculator()
+dmjone.jatin.demoName()
 dmjone.kaustuv.calculate_absolute()
+dmjone.subhojeet.packagebySubhojeet()
 ```
 
-## Authors
-- **Divya Mohan** - *__init__* - [GitHub](https://github.com/divyamohan1993)
-- **Aarushi Sharma** - [GitHub](https://github.com/letscodeitup)
-- **Anshuman Mohanty** - [GitHub](https://github.com/anshumanmohanty00)
-- **Ashutosh Rana**
-- **Jatin Sharma**
-- **Kaustuv Sharma** - *Contributor* - [GitHub](https://github.com/kaustuvsharma)
-- **Lakshika Tanwar** - *Contributor* - [GitHub](https://github.com/LakshikaTanwar)
-- **Rijul Chaudhary** - [GitHub](https://github.com/Rijul777)
-- **Vedansh Sharma** - [GitHub](https://github.com/Elysian-Reverie)
+## Example Usage
+Example 1
+```python
+import dmjone
+dmjone.aarushi.todolist()
+```
+Example 2
+```python
+# Access the Student Management System, A Project by Students
+import dmjone
+dmjone.projectsms() # Ensure you have MySQL installed on your system if you are running it locally.
+```
+Example 3
+```python
+from dmjone import kaustuv as ks
+ks.check_all_true()
+```
 
-See also the list of [contributors](https://github.com/dmjone/dmjone_pypi/contributors) who participated in this project.
+## Notable User Contributions and Collaborations
+#### Aarushi Sharma
+- **TodoList**: A simple To-Do List creator.
+#### Kaustuv Sharma
+- **Calculate Absolute Value**: Calculate absolute value of a given number
+#### Lakshika Tanwar
+- **Typecasting**: Demonstrate Typecasting in python
+- **Calculator**: Calculator to do arithmetic operations on numbers
 
-## Features
+## Highlighted Features and Collaborations
 - **Student Management System**: A simple yet powerful system for managing student records, designed for educational institutions.
 - **Lab Projects**: Access to various educational projects and lab work to facilitate learning and teaching.
 - **Educational Tools**: A collection of tools aimed at enhancing the learning experience.
 
-## User Collaborations
-### Aarushi Sharma
-- **TodoList**: A simple To-Do List creator.
-### Kaustuv Sharma
-- **Calculate Absolute Value**: Calculate absolute value of a given number
-### Lakshika Tanwar
-- **Typecasting**: Demonstrate Typecasting in python
-- **Calculator**: Calculator to do arithmetic operations on numbers
+## Authors
+- **Divya Mohan** - *__init__* - [GitHub](https://github.com/divyamohan1993) | **Lakshika Tanwar** - *Top Contributor* - [GitHub](https://github.com/LakshikaTanwar) | **Aarushi Sharma** - *Contributor* - [GitHub](https://github.com/letscodeitup) | **Kaustuv Sharma** - *Contributor* - [GitHub](https://github.com/kaustuvsharma) | **Anshuman Mohanty** - [GitHub](https://github.com/anshumanmohanty00) | **Ashutosh Rana** | **Jatin Sharma** | **Rijul Chaudhary** - [GitHub](https://github.com/Rijul777) | **Vedansh Sharma** - [GitHub](https://github.com/Elysian-Reverie) | Subhojeet Ghosh [GitHub](https://github.com/subhojeetghosh123)
 
-## Documentation
-<!-- For comprehensive documentation, visit [dmj.one/docs](https://dmj.one/docs). Here, you'll find detailed information on how to make the most of the tools and resources offered by `dmjone`. -->
-For comprehensive documentation, visit [dmj.one](https://dmj.one). Here, you'll find detailed information on how to make the most of the tools and resources offered by `dmjone`.
+See also the list of [contributors](https://github.com/dmjone/dmjone_pypi/contributors) who participated in this project.
 
-## Contributing
+## How To Contribute
 
-Contributions are what make the open-source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.
+We thank you for your interest in contributing to `dmjone`! 🎉 Your efforts make a big difference. Whether you're fixing a bug, adding a feature, or improving documentation, we appreciate your help. Here’s how to contribute in a friendly and easy way:
 
-1. Fork the Project
-2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
-3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
-4. Push to the Branch (`git push origin feature/AmazingFeature`)
-5. Open a Pull Request
+#### Found a solution to a problem? Let's get you started!
 
-## License
+1. **Find something to work on**: Look through the [GitHub issues](https://github.com/dmjone/dmjone_pypi/issues) for something that interests you or open a new issue to suggest improvements or report bugs.
 
-Distributed under the GPL-3.0 License. See `LICENSE` for more information.
+#### Making Changes
 
-## Acknowledgements
+##### Using GitHub Web Interface
+For small changes, like fixing typos or small code snippets, using the GitHub web interface is the easiest way:
+
+1. Navigate to the file you want to edit on the [dmjone GitHub Repo](https://github.com/dmjone/dmjone_pypi).
+2. Click the pencil icon (Edit this file) to start making changes.
+3. After making changes, describe what you did and why in the **Commit changes** box.
+4. Choose the option to **Create a new branch for this commit and start a pull request**. Name it appropriately, like `fix/typo-in-readme`.
+5. Click **Propose changes** and then **Create pull request** on the next page.
+
+##### Using Command Line
+For larger changes or new features, you might prefer working locally:
+
+1. **Fork the Repository**: Click the "Fork" button on the top right of the [dmjone GitHub Repo](https://github.com/dmjone/dmjone_pypi) page to create your copy.
+2. **Clone Your Fork**: `git clone https://github.com/your-username/dmjone_pypi.git` to clone the project to your computer.
+3. **Create a Branch**: Switch to your clone and use `git checkout -b feature/YourFeatureName` or `fix/YourBugFix` to create a new branch.
+4. **Make Your Changes**: Add your changes using your favorite editor or IDE.
+5. **Commit Your Changes**: Use `git commit -m 'A brief description of your changes'` to save your work.
+6. **Push to GitHub**: Use `git push origin feature/YourFeatureName` to upload your changes to your GitHub fork.
+7. **Open a Pull Request**: Go to your fork on GitHub and press the "New pull request" button. Describe your changes and submit!
+
+### Before You Submit
+
+- **Review Your Changes**: Double-check your changes and make sure everything works as expected. Try to keep your changes simple and focused on solving a single problem.
+- **Follow the Style Guide**: Make sure your contributions follow the existing code style to keep the project organized.
+- **Update Tests**: If you're adding a new feature, consider adding tests to support it.
+
+### Submitting Your Contribution
+
+Once you’re ready to submit, open a pull request with your changes. Provide a clear description of the problem and solution, including any relevant issue numbers.
+
+### After You Submit
 
+- **Patience is Key**: Maintainers will review your contribution and may suggest changes. This is a normal part of the process; feedback helps improve the project.
+- **Stay Engaged**: Check back in case the maintainers have questions or feedback. Your pull request may spark a conversation.
+
+### And That's It!
+
+You've contributed to `dmjone`! We're grateful for your help in making this project better. Remember, contributing is not just about code; every bit of documentation, bug reports, or even suggestions are valuable to us.
+
+Thank you for being part of our open-source community! Let the world be educated!🌟
+
+## Acknowledgements
 - Shoolini University
 - All educators and students at Shoolini University
 
 ## Contact
-
 For any queries, please reach out to us via [the message button on dmj.one](https://dmj.one/).
 
+## Documentation
+<!-- For comprehensive documentation, visit [dmj.one/docs](https://dmj.one/docs). Here, you'll find detailed information on how to make the most of the tools and resources offered by `dmjone`. -->
+For comprehensive documentation, visit [dmj.one](https://dmj.one). Here, you'll find detailed information on how to make the most of the tools and resources offered by `dmjone`.
+
+## License
+Distributed under the GPL-3.0 License. See `LICENSE` for more information.
+
 ## Project Links
 
 - **Project Homepage**: [dmj.one](https://dmj.one)
 - **PyPI Repository**: [dmjone on PyPI](https://pypi.org/project/dmjone/)
 - **Source Code**: [GitHub Repository](https://github.com/dmjone/dmjone_pypi)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `dmjone-0.1.9.4/src/dmjone.egg-info/SOURCES.txt` & `dmjone-0.1.9.7/src/dmjone.egg-info/SOURCES.txt`

 * *Files identical despite different names*

