# Comparing `tmp/reddit2text-0.0.7.tar.gz` & `tmp/reddit2text-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reddit2text-0.0.7.tar", last modified: Sat Apr  6 21:02:35 2024, max compression
+gzip compressed data, was "reddit2text-0.0.8.tar", last modified: Sat Apr  6 23:37:41 2024, max compression
```

## Comparing `reddit2text-0.0.7.tar` & `reddit2text-0.0.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 21:02:35.351683 reddit2text-0.0.7/
--rw-r--r--   0 root         (0) root         (0)    11357 2024-03-05 18:59:10.000000 reddit2text-0.0.7/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3494 2024-04-06 21:02:35.351683 reddit2text-0.0.7/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2806 2024-04-06 20:46:04.000000 reddit2text-0.0.7/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 21:02:35.347684 reddit2text-0.0.7/reddit2text/
--rw-r--r--   0 root         (0) root         (0)       30 2024-04-06 20:45:56.000000 reddit2text-0.0.7/reddit2text/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2962 2024-04-06 20:45:56.000000 reddit2text-0.0.7/reddit2text/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 21:02:35.351683 reddit2text-0.0.7/reddit2text.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3494 2024-04-06 21:02:35.000000 reddit2text-0.0.7/reddit2text.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      244 2024-04-06 21:02:35.000000 reddit2text-0.0.7/reddit2text.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-06 21:02:35.000000 reddit2text-0.0.7/reddit2text.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        5 2024-04-06 21:02:35.000000 reddit2text-0.0.7/reddit2text.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2024-04-06 21:02:35.000000 reddit2text-0.0.7/reddit2text.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-06 21:02:35.351683 reddit2text-0.0.7/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     4081 2024-04-06 21:01:07.000000 reddit2text-0.0.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 23:37:41.811179 reddit2text-0.0.8/
+-rw-r--r--   0 root         (0) root         (0)    11357 2024-03-05 18:59:10.000000 reddit2text-0.0.8/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3684 2024-04-06 23:37:41.811179 reddit2text-0.0.8/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2997 2024-04-06 23:36:04.000000 reddit2text-0.0.8/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 23:37:41.803178 reddit2text-0.0.8/reddit2text/
+-rw-r--r--   0 root         (0) root         (0)       30 2024-04-06 20:45:56.000000 reddit2text-0.0.8/reddit2text/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2962 2024-04-06 20:45:56.000000 reddit2text-0.0.8/reddit2text/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 23:37:41.811179 reddit2text-0.0.8/reddit2text.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3684 2024-04-06 23:37:41.000000 reddit2text-0.0.8/reddit2text.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      244 2024-04-06 23:37:41.000000 reddit2text-0.0.8/reddit2text.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-06 23:37:41.000000 reddit2text-0.0.8/reddit2text.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2024-04-06 23:37:41.000000 reddit2text-0.0.8/reddit2text.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2024-04-06 23:37:41.000000 reddit2text-0.0.8/reddit2text.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-06 23:37:41.811179 reddit2text-0.0.8/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     4366 2024-04-06 23:37:25.000000 reddit2text-0.0.8/setup.py
```

### Comparing `reddit2text-0.0.7/LICENSE` & `reddit2text-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `reddit2text-0.0.7/PKG-INFO` & `reddit2text-0.0.8/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reddit2text
-Version: 0.0.7
+Version: 0.0.8
 Summary: Convert Reddit posts to text
 Author: Nicholas Hansen-Feruch
 Author-email: nicholas.feruch@gmail.com
 Keywords: python,reddit,text conversion,reddit api,praw,reddit to text,reddit comments,social media analysis
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -15,91 +15,97 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: praw
 
 
 # Reddit2Text
 
-`reddit2text` is a Python library designed to effortlessly **transform any Reddit post and its comments into a clean, readable text format**.
+`reddit2text` is *the* Python library designed to effortlessly **transform any Reddit thread into clean, readable text data**.
 
-Perfect for *feeding to an LLM, data analysis, or simply reading offline*, `reddit2text` offers a straightforward interface to access and convert content from Reddit.
+Perfect for *feeding to an LLM, performing textual/data analysis, or simply archiving for offline use*, `reddit2text` offers a straightforward interface to access and convert content from Reddit.
 
-## Table of contents
+## Table of Contents
 - [Features](#features)
 - [Installation](#installation)
 - [Quickstart](#quickstart)
   - [Example Code](#example)
+  - [Example Output](#output)
 - [Configs](#configs)
 - [Contributions](#contributions)
 - [License](#license)
 
 <a id="features"></a>
 
 ## Features
-- Convert any Reddit post into structured text format.
-- Include all comments, with support for specifying maximum comment depth.
-- Configurable comment delimiter for visual separation of nested comments.
-
-> **Want Something Added?**
-> Simply ***open an issue*** here on github and tell us what should be added to the next release!
+- Convert any Reddit thread (the post + all its comments) into structured text.
+- Include all comments, with the ability to specify the maximum comment depth.
+- Configure a custom comment delimiter, for visual separation of nested comments.
+
+> **Have a Feature Idea?**
+>
+> Simply ***open an issue on github*** and tell us what should be added to the next release!
 
 <a id="installation"></a>
 
 ## Installation
-Install reddit2text using pip
+Easy install using pip
 ```sh
 pip3 install reddit2text
 ```
 
 <a id="quickstart"></a>
 
 ## Quickstart
-**First**, you need to register a Reddit application to obtain a **client_id** and **client_secret**. Follow the instructions on [Reddit's API documentation](https://www.reddit.com/wiki/api) to set up your application.
+**First**, you need to create a Reddit app to get your **client_id** and **client_secret**. Follow the instructions on [Reddit's API documentation](https://www.reddit.com/wiki/api) to set up your application.
 
-Then, replace the `client_id`, `client_secret`, and `user_agent` with your credentials.
+**Then**, replace the `client_id`, `client_secret`, and `user_agent` with your credentials.
 
-The user agent can be anything you like, but we recommend following this convention that follows Reddit's guidelines: `'<app type>:<app name>:<version> (by <your username>)'`
+The user agent can be anything you like, but we recommend following this convention according to Reddit's guidelines: `'<app type>:<app name>:<version> (by <your username>)'`
 
 <a id="example"></a>
 
 *Here's an example:*
 ```python
 from reddit2text import Reddit2Text
 
 r2t = Reddit2Text(
     # example credentials
     client_id='123abc',
     client_secret='123abc',
     user_agent='script:my_app:v1.0 (by u/reddit2text)'
 )
 
-# The URL must have the post ID after the /comments/ to work
+# The URL must have the post ID after the /comments/ to work, e.g. `1buyr0g`
 URL = 'https://www.reddit.com/r/MadeMeSmile/comments/1buyr0g/ryan_reynolds_being_wholesome/'
 
 output = r2t.textualize_post(URL)
 print(output)
 ```
 
+<a id="output"></a>
+
+Here is an example (truncated) output from the above code!
+https://pastebin.com/mmHFJtcc
+
 <a id="configs"></a>
 
 ## Extra Configuration
 - **max_comment_depth**: Maximum depth of comments to output. Includes the top-most comment. Defaults to `None` or `-1` to include all.
 - **comment_delim**: String/character used to indent comments according to their nesting level. Defaults to `|` to mimic reddit.
 
 ```python
 r2t = Reddit2Text(
     # credentials ...
-    max_comment_depth=3,  # all comment trees will be limited to a max of 3 replies
+    max_comment_depth=3,  # all comment chains will be limited to a max of 3 replies
     comment_delim='#'  # each comment level will be preceded by multiples of this string
 )
 ```
 
 <a id="contributions"></a>
 
 ## Contributions
 Contributions to reddit2text are welcome. Please submit pull requests or issues to our GitHub repository.
 
 <a id="license"></a>
 
 ## License
 reddit2text is released under the MIT License. See the LICENSE file for more details.
-
```

### Comparing `reddit2text-0.0.7/README.md` & `reddit2text-0.0.8/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,79 +1,86 @@
 # Reddit2Text
 
-`reddit2text` is a Python library designed to effortlessly **transform any Reddit post and its comments into a clean, readable text format**.
+`reddit2text` is *the* Python library designed to effortlessly **transform any Reddit thread into clean, readable text data**.
 
-Perfect for *feeding to an LLM, data analysis, or simply reading offline*, `reddit2text` offers a straightforward interface to access and convert content from Reddit.
+Perfect for *feeding to an LLM, performing textual/data analysis, or simply archiving for offline use*, `reddit2text` offers a straightforward interface to access and convert content from Reddit.
 
-## Table of contents
+## Table of Contents
 - [Features](#features)
 - [Installation](#installation)
 - [Quickstart](#quickstart)
   - [Example Code](#example)
+  - [Example Output](#output)
 - [Configs](#configs)
 - [Contributions](#contributions)
 - [License](#license)
 
 <a id="features"></a>
 
 ## Features
-- Convert any Reddit post into structured text format.
-- Include all comments, with support for specifying maximum comment depth.
-- Configurable comment delimiter for visual separation of nested comments.
-
-> **Want Something Added?**
-> Simply ***open an issue*** here on github and tell us what should be added to the next release!
+- Convert any Reddit thread (the post + all its comments) into structured text.
+- Include all comments, with the ability to specify the maximum comment depth.
+- Configure a custom comment delimiter, for visual separation of nested comments.
+
+> **Have a Feature Idea?**
+>
+> Simply ***open an issue on github*** and tell us what should be added to the next release!
 
 <a id="installation"></a>
 
 ## Installation
-Install reddit2text using pip
+Easy install using pip
 ```sh
 pip3 install reddit2text
 ```
 
 <a id="quickstart"></a>
 
 ## Quickstart
-**First**, you need to register a Reddit application to obtain a **client_id** and **client_secret**. Follow the instructions on [Reddit's API documentation](https://www.reddit.com/wiki/api) to set up your application.
+**First**, you need to create a Reddit app to get your **client_id** and **client_secret**. Follow the instructions on [Reddit's API documentation](https://www.reddit.com/wiki/api) to set up your application.
 
-Then, replace the `client_id`, `client_secret`, and `user_agent` with your credentials.
+**Then**, replace the `client_id`, `client_secret`, and `user_agent` with your credentials.
 
-The user agent can be anything you like, but we recommend following this convention that follows Reddit's guidelines: `'<app type>:<app name>:<version> (by <your username>)'`
+The user agent can be anything you like, but we recommend following this convention according to Reddit's guidelines: `'<app type>:<app name>:<version> (by <your username>)'`
 
 <a id="example"></a>
 
 *Here's an example:*
 ```python
 from reddit2text import Reddit2Text
 
 r2t = Reddit2Text(
     # example credentials
     client_id='123abc',
     client_secret='123abc',
     user_agent='script:my_app:v1.0 (by u/reddit2text)'
 )
 
-# The URL must have the post ID after the /comments/ to work
+# The URL must have the post ID after the /comments/ to work, e.g. `1buyr0g`
 URL = 'https://www.reddit.com/r/MadeMeSmile/comments/1buyr0g/ryan_reynolds_being_wholesome/'
 
 output = r2t.textualize_post(URL)
 print(output)
 ```
 
+<a id="output"></a>
+
+Here is an example (truncated) output from the above code!
+https://pastebin.com/mmHFJtcc
+
 <a id="configs"></a>
 
 ## Extra Configuration
 - **max_comment_depth**: Maximum depth of comments to output. Includes the top-most comment. Defaults to `None` or `-1` to include all.
 - **comment_delim**: String/character used to indent comments according to their nesting level. Defaults to `|` to mimic reddit.
 
 ```python
 r2t = Reddit2Text(
     # credentials ...
-    max_comment_depth=3,  # all comment trees will be limited to a max of 3 replies
+    max_comment_depth=3,  # all comment chains will be limited to a max of 3 replies
     comment_delim='#'  # each comment level will be preceded by multiples of this string
 )
 ```
 
 <a id="contributions"></a>
 
 ## Contributions
```

### Comparing `reddit2text-0.0.7/reddit2text/main.py` & `reddit2text-0.0.8/reddit2text/main.py`

 * *Files identical despite different names*

### Comparing `reddit2text-0.0.7/reddit2text.egg-info/PKG-INFO` & `reddit2text-0.0.8/reddit2text.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reddit2text
-Version: 0.0.7
+Version: 0.0.8
 Summary: Convert Reddit posts to text
 Author: Nicholas Hansen-Feruch
 Author-email: nicholas.feruch@gmail.com
 Keywords: python,reddit,text conversion,reddit api,praw,reddit to text,reddit comments,social media analysis
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -15,91 +15,97 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: praw
 
 
 # Reddit2Text
 
-`reddit2text` is a Python library designed to effortlessly **transform any Reddit post and its comments into a clean, readable text format**.
+`reddit2text` is *the* Python library designed to effortlessly **transform any Reddit thread into clean, readable text data**.
 
-Perfect for *feeding to an LLM, data analysis, or simply reading offline*, `reddit2text` offers a straightforward interface to access and convert content from Reddit.
+Perfect for *feeding to an LLM, performing textual/data analysis, or simply archiving for offline use*, `reddit2text` offers a straightforward interface to access and convert content from Reddit.
 
-## Table of contents
+## Table of Contents
 - [Features](#features)
 - [Installation](#installation)
 - [Quickstart](#quickstart)
   - [Example Code](#example)
+  - [Example Output](#output)
 - [Configs](#configs)
 - [Contributions](#contributions)
 - [License](#license)
 
 <a id="features"></a>
 
 ## Features
-- Convert any Reddit post into structured text format.
-- Include all comments, with support for specifying maximum comment depth.
-- Configurable comment delimiter for visual separation of nested comments.
-
-> **Want Something Added?**
-> Simply ***open an issue*** here on github and tell us what should be added to the next release!
+- Convert any Reddit thread (the post + all its comments) into structured text.
+- Include all comments, with the ability to specify the maximum comment depth.
+- Configure a custom comment delimiter, for visual separation of nested comments.
+
+> **Have a Feature Idea?**
+>
+> Simply ***open an issue on github*** and tell us what should be added to the next release!
 
 <a id="installation"></a>
 
 ## Installation
-Install reddit2text using pip
+Easy install using pip
 ```sh
 pip3 install reddit2text
 ```
 
 <a id="quickstart"></a>
 
 ## Quickstart
-**First**, you need to register a Reddit application to obtain a **client_id** and **client_secret**. Follow the instructions on [Reddit's API documentation](https://www.reddit.com/wiki/api) to set up your application.
+**First**, you need to create a Reddit app to get your **client_id** and **client_secret**. Follow the instructions on [Reddit's API documentation](https://www.reddit.com/wiki/api) to set up your application.
 
-Then, replace the `client_id`, `client_secret`, and `user_agent` with your credentials.
+**Then**, replace the `client_id`, `client_secret`, and `user_agent` with your credentials.
 
-The user agent can be anything you like, but we recommend following this convention that follows Reddit's guidelines: `'<app type>:<app name>:<version> (by <your username>)'`
+The user agent can be anything you like, but we recommend following this convention according to Reddit's guidelines: `'<app type>:<app name>:<version> (by <your username>)'`
 
 <a id="example"></a>
 
 *Here's an example:*
 ```python
 from reddit2text import Reddit2Text
 
 r2t = Reddit2Text(
     # example credentials
     client_id='123abc',
     client_secret='123abc',
     user_agent='script:my_app:v1.0 (by u/reddit2text)'
 )
 
-# The URL must have the post ID after the /comments/ to work
+# The URL must have the post ID after the /comments/ to work, e.g. `1buyr0g`
 URL = 'https://www.reddit.com/r/MadeMeSmile/comments/1buyr0g/ryan_reynolds_being_wholesome/'
 
 output = r2t.textualize_post(URL)
 print(output)
 ```
 
+<a id="output"></a>
+
+Here is an example (truncated) output from the above code!
+https://pastebin.com/mmHFJtcc
+
 <a id="configs"></a>
 
 ## Extra Configuration
 - **max_comment_depth**: Maximum depth of comments to output. Includes the top-most comment. Defaults to `None` or `-1` to include all.
 - **comment_delim**: String/character used to indent comments according to their nesting level. Defaults to `|` to mimic reddit.
 
 ```python
 r2t = Reddit2Text(
     # credentials ...
-    max_comment_depth=3,  # all comment trees will be limited to a max of 3 replies
+    max_comment_depth=3,  # all comment chains will be limited to a max of 3 replies
     comment_delim='#'  # each comment level will be preceded by multiples of this string
 )
 ```
 
 <a id="contributions"></a>
 
 ## Contributions
 Contributions to reddit2text are welcome. Please submit pull requests or issues to our GitHub repository.
 
 <a id="license"></a>
 
 ## License
 reddit2text is released under the MIT License. See the LICENSE file for more details.
-
```

### Comparing `reddit2text-0.0.7/setup.py` & `reddit2text-0.0.8/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,98 +1,105 @@
+# clear && python3 setup.py sdist bdist_wheel && twine upload --skip-existing dist/* --verbose
 from setuptools import setup, find_packages
 
-VERSION = '0.0.7'  # Consider starting with a semantic versioning scheme
+VERSION = '0.0.8'  # Consider starting with a semantic versioning scheme
 DESCRIPTION = 'Convert Reddit posts to text'
 LONG_DESCRIPTION = """
 # Reddit2Text
 
-`reddit2text` is a Python library designed to effortlessly **transform any Reddit post and its comments into a clean, readable text format**.
+`reddit2text` is *the* Python library designed to effortlessly **transform any Reddit thread into clean, readable text data**.
 
-Perfect for *feeding to an LLM, data analysis, or simply reading offline*, `reddit2text` offers a straightforward interface to access and convert content from Reddit.
+Perfect for *feeding to an LLM, performing textual/data analysis, or simply archiving for offline use*, `reddit2text` offers a straightforward interface to access and convert content from Reddit.
 
-## Table of contents
+## Table of Contents
 - [Features](#features)
 - [Installation](#installation)
 - [Quickstart](#quickstart)
   - [Example Code](#example)
+  - [Example Output](#output)
 - [Configs](#configs)
 - [Contributions](#contributions)
 - [License](#license)
 
 <a id="features"></a>
 
 ## Features
-- Convert any Reddit post into structured text format.
-- Include all comments, with support for specifying maximum comment depth.
-- Configurable comment delimiter for visual separation of nested comments.
-
-> **Want Something Added?**
-> Simply ***open an issue*** here on github and tell us what should be added to the next release!
+- Convert any Reddit thread (the post + all its comments) into structured text.
+- Include all comments, with the ability to specify the maximum comment depth.
+- Configure a custom comment delimiter, for visual separation of nested comments.
+
+> **Have a Feature Idea?**
+>
+> Simply ***open an issue on github*** and tell us what should be added to the next release!
 
 <a id="installation"></a>
 
 ## Installation
-Install reddit2text using pip
+Easy install using pip
 ```sh
 pip3 install reddit2text
 ```
 
 <a id="quickstart"></a>
 
 ## Quickstart
-**First**, you need to register a Reddit application to obtain a **client_id** and **client_secret**. Follow the instructions on [Reddit's API documentation](https://www.reddit.com/wiki/api) to set up your application.
+**First**, you need to create a Reddit app to get your **client_id** and **client_secret**. Follow the instructions on [Reddit's API documentation](https://www.reddit.com/wiki/api) to set up your application.
 
-Then, replace the `client_id`, `client_secret`, and `user_agent` with your credentials.
+**Then**, replace the `client_id`, `client_secret`, and `user_agent` with your credentials.
 
-The user agent can be anything you like, but we recommend following this convention that follows Reddit's guidelines: `'<app type>:<app name>:<version> (by <your username>)'`
+The user agent can be anything you like, but we recommend following this convention according to Reddit's guidelines: `'<app type>:<app name>:<version> (by <your username>)'`
 
 <a id="example"></a>
 
 *Here's an example:*
 ```python
 from reddit2text import Reddit2Text
 
 r2t = Reddit2Text(
     # example credentials
     client_id='123abc',
     client_secret='123abc',
     user_agent='script:my_app:v1.0 (by u/reddit2text)'
 )
 
-# The URL must have the post ID after the /comments/ to work
+# The URL must have the post ID after the /comments/ to work, e.g. `1buyr0g`
 URL = 'https://www.reddit.com/r/MadeMeSmile/comments/1buyr0g/ryan_reynolds_being_wholesome/'
 
 output = r2t.textualize_post(URL)
 print(output)
 ```
 
+<a id="output"></a>
+
+Here is an example (truncated) output from the above code!
+https://pastebin.com/mmHFJtcc
+
 <a id="configs"></a>
 
 ## Extra Configuration
 - **max_comment_depth**: Maximum depth of comments to output. Includes the top-most comment. Defaults to `None` or `-1` to include all.
 - **comment_delim**: String/character used to indent comments according to their nesting level. Defaults to `|` to mimic reddit.
 
 ```python
 r2t = Reddit2Text(
     # credentials ...
-    max_comment_depth=3,  # all comment trees will be limited to a max of 3 replies
+    max_comment_depth=3,  # all comment chains will be limited to a max of 3 replies
     comment_delim='#'  # each comment level will be preceded by multiples of this string
 )
 ```
 
 <a id="contributions"></a>
 
 ## Contributions
 Contributions to reddit2text are welcome. Please submit pull requests or issues to our GitHub repository.
 
 <a id="license"></a>
 
 ## License
 reddit2text is released under the MIT License. See the LICENSE file for more details.
-
 """
 
 # Setting up
 setup(
     name="reddit2text",
     version=VERSION,
     author="Nicholas Hansen-Feruch",
```

