# Comparing `tmp/noobstuffs-1.0.9.tar.gz` & `tmp/noobstuffs-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "noobstuffs-1.0.9.tar", max compression
+gzip compressed data, was "noobstuffs-2.0.0.tar", max compression
```

## Comparing `noobstuffs-1.0.9.tar` & `noobstuffs-2.0.0.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0      797 2023-04-08 03:24:38.232423 noobstuffs-1.0.9/NoobStuffs/__init__.py
--rw-r--r--   0        0        0     2085 2022-11-18 06:09:27.000000 noobstuffs-1.0.9/NoobStuffs/libandroid/__init__.py
--rw-r--r--   0        0        0     1770 2022-11-18 06:09:27.000000 noobstuffs-1.0.9/NoobStuffs/libdatetime/__init__.py
--rw-r--r--   0        0        0     4477 2022-11-18 06:09:27.000000 noobstuffs-1.0.9/NoobStuffs/libformatter/__init__.py
--rw-r--r--   0        0        0     1473 2022-11-18 06:09:27.000000 noobstuffs-1.0.9/NoobStuffs/libformatter/escape.py
--rw-r--r--   0        0        0     3414 2022-11-18 06:09:27.000000 noobstuffs-1.0.9/NoobStuffs/libgithub/__init__.py
--rw-r--r--   0        0        0     2540 2022-11-18 06:09:27.000000 noobstuffs-1.0.9/NoobStuffs/liblogging/__init__.py
--rw-r--r--   0        0        0     1443 2022-11-18 06:09:27.000000 noobstuffs-1.0.9/NoobStuffs/libpasty/__init__.py
--rw-r--r--   0        0        0     2639 2022-11-18 06:09:27.000000 noobstuffs-1.0.9/NoobStuffs/libtelegraph/__init__.py
--rw-r--r--   0        0        0      604 2022-11-18 06:09:27.000000 noobstuffs-1.0.9/README.md
--rw-r--r--   0        0        0      767 2023-04-08 03:25:29.532421 noobstuffs-1.0.9/pyproject.toml
--rw-r--r--   0        0        0     1509 1970-01-01 00:00:00.000000 noobstuffs-1.0.9/PKG-INFO
+-rw-r--r--   0        0        0      797 2024-04-07 08:05:04.177705 noobstuffs-2.0.0/NoobStuffs/__init__.py
+-rw-r--r--   0        0        0     2085 2022-11-19 04:49:54.617779 noobstuffs-2.0.0/NoobStuffs/libandroid/__init__.py
+-rw-r--r--   0        0        0     1770 2022-11-19 04:49:54.628785 noobstuffs-2.0.0/NoobStuffs/libdatetime/__init__.py
+-rw-r--r--   0        0        0     4477 2022-11-19 04:49:54.638787 noobstuffs-2.0.0/NoobStuffs/libformatter/__init__.py
+-rw-r--r--   0        0        0     1473 2022-11-19 04:49:54.646774 noobstuffs-2.0.0/NoobStuffs/libformatter/escape.py
+-rw-r--r--   0        0        0     3414 2022-11-19 04:49:54.655784 noobstuffs-2.0.0/NoobStuffs/libgithub/__init__.py
+-rw-r--r--   0        0        0     2540 2022-11-19 04:49:54.664783 noobstuffs-2.0.0/NoobStuffs/liblogging/__init__.py
+-rw-r--r--   0        0        0     1443 2022-11-19 04:49:54.673781 noobstuffs-2.0.0/NoobStuffs/libpasty/__init__.py
+-rwxr-xr-x   0        0        0     1883 2024-04-07 08:02:01.488957 noobstuffs-2.0.0/NoobStuffs/libtelegrambot/__init__.py
+-rw-r--r--   0        0        0     2724 2024-04-07 07:05:32.639477 noobstuffs-2.0.0/NoobStuffs/libtelegraph/__init__.py
+-rw-r--r--   0        0        0      604 2022-11-19 04:49:54.687784 noobstuffs-2.0.0/README.md
+-rw-r--r--   0        0        0      805 2024-04-07 08:05:24.094385 noobstuffs-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1515 1970-01-01 00:00:00.000000 noobstuffs-2.0.0/PKG-INFO
```

### Comparing `noobstuffs-1.0.9/NoobStuffs/__init__.py` & `noobstuffs-2.0.0/NoobStuffs/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,8 +14,8 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 #
 
-__version__ = "1.0.9"
+__version__ = "2.0.0"
```

### Comparing `noobstuffs-1.0.9/NoobStuffs/libandroid/__init__.py` & `noobstuffs-2.0.0/NoobStuffs/libandroid/__init__.py`

 * *Files identical despite different names*

### Comparing `noobstuffs-1.0.9/NoobStuffs/libdatetime/__init__.py` & `noobstuffs-2.0.0/NoobStuffs/libdatetime/__init__.py`

 * *Files identical despite different names*

### Comparing `noobstuffs-1.0.9/NoobStuffs/libformatter/__init__.py` & `noobstuffs-2.0.0/NoobStuffs/libformatter/__init__.py`

 * *Files identical despite different names*

### Comparing `noobstuffs-1.0.9/NoobStuffs/libformatter/escape.py` & `noobstuffs-2.0.0/NoobStuffs/libformatter/escape.py`

 * *Files identical despite different names*

### Comparing `noobstuffs-1.0.9/NoobStuffs/libgithub/__init__.py` & `noobstuffs-2.0.0/NoobStuffs/libgithub/__init__.py`

 * *Files identical despite different names*

### Comparing `noobstuffs-1.0.9/NoobStuffs/liblogging/__init__.py` & `noobstuffs-2.0.0/NoobStuffs/liblogging/__init__.py`

 * *Files identical despite different names*

### Comparing `noobstuffs-1.0.9/NoobStuffs/libpasty/__init__.py` & `noobstuffs-2.0.0/NoobStuffs/libpasty/__init__.py`

 * *Files identical despite different names*

### Comparing `noobstuffs-1.0.9/NoobStuffs/libtelegraph/__init__.py` & `noobstuffs-2.0.0/NoobStuffs/libtelegraph/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,16 +26,21 @@
 from telegraph import Telegraph
 from telegraph.exceptions import RetryAfterError
 
 LOGGER = getLogger("TelegraphHelper")
 
 
 class TelegraphHelper:
-    def __init__(self, author_name: str, author_url: str):
-        self.telegraph = Telegraph()
+    def __init__(
+        self,
+        author_name: str,
+        author_url: str,
+        domain: str = "telegra.ph",
+    ):
+        self.telegraph = Telegraph(domain=domain)
         self.short_name = "".join(choices(population=ascii_letters, k=5))
         self.author_name = author_name
         self.author_url = author_url
         self.create_account()
 
     def create_account(self):
         LOGGER.info(f"Creating account: {self.author_name}")
```

### Comparing `noobstuffs-1.0.9/README.md` & `noobstuffs-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `noobstuffs-1.0.9/pyproject.toml` & `noobstuffs-2.0.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "NoobStuffs"
-version = "1.0.9"
+version = "2.0.0"
 description = "Python Library for PrajjuS Projects"
 license = "GPL-3.0"
 authors = ["PrajjuS <theprajjus@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/PrajjuS/NoobStuffs"
 keywords = ["noobstuffs", "libs", "noob", "lazy"]
 classifiers = [
@@ -15,16 +15,17 @@
 packages = [
     { include = "NoobStuffs" }
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 requests = "^2.28.0"
-pytz = ">=2022.1,<2024.0"
-PyGithub = "^1.55"
+pytz = ">=2022.1,<2025.0"
+PyGithub = ">=1.55,<3.0"
 telegraph = "^2.2.0"
+python-telegram-bot = "^21.0.1"
 
 [tool.poetry.dev-dependencies]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `noobstuffs-1.0.9/PKG-INFO` & `noobstuffs-2.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
-Name: noobstuffs
-Version: 1.0.9
+Name: NoobStuffs
+Version: 2.0.0
 Summary: Python Library for PrajjuS Projects
 Home-page: https://github.com/PrajjuS/NoobStuffs
 License: GPL-3.0
 Keywords: noobstuffs,libs,noob,lazy
 Author: PrajjuS
 Author-email: theprajjus@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
-Requires-Dist: PyGithub (>=1.55,<2.0)
-Requires-Dist: pytz (>=2022.1,<2024.0)
+Requires-Dist: PyGithub (>=1.55,<3.0)
+Requires-Dist: python-telegram-bot (>=21.0.1,<22.0.0)
+Requires-Dist: pytz (>=2022.1,<2025.0)
 Requires-Dist: requests (>=2.28.0,<3.0.0)
 Requires-Dist: telegraph (>=2.2.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 # NoobStuffs
 
 [![PyPi version](https://img.shields.io/pypi/v/noobstuffs)](https://pypi.org/project/noobstuffs/)
```

