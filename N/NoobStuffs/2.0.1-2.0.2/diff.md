# Comparing `tmp/noobstuffs-2.0.1.tar.gz` & `tmp/noobstuffs-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "noobstuffs-2.0.1.tar", max compression
+gzip compressed data, was "noobstuffs-2.0.2.tar", max compression
```

## Comparing `noobstuffs-2.0.1.tar` & `noobstuffs-2.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      797 2024-04-07 11:40:15.413972 noobstuffs-2.0.1/NoobStuffs/__init__.py
--rw-r--r--   0        0        0     2085 2022-11-19 04:49:54.617779 noobstuffs-2.0.1/NoobStuffs/libandroid/__init__.py
--rw-r--r--   0        0        0     1770 2022-11-19 04:49:54.628785 noobstuffs-2.0.1/NoobStuffs/libdatetime/__init__.py
--rw-r--r--   0        0        0     4477 2022-11-19 04:49:54.638787 noobstuffs-2.0.1/NoobStuffs/libformatter/__init__.py
--rw-r--r--   0        0        0     1473 2022-11-19 04:49:54.646774 noobstuffs-2.0.1/NoobStuffs/libformatter/escape.py
--rw-r--r--   0        0        0     3414 2022-11-19 04:49:54.655784 noobstuffs-2.0.1/NoobStuffs/libgithub/__init__.py
--rw-r--r--   0        0        0     2540 2022-11-19 04:49:54.664783 noobstuffs-2.0.1/NoobStuffs/liblogging/__init__.py
--rw-r--r--   0        0        0     1443 2022-11-19 04:49:54.673781 noobstuffs-2.0.1/NoobStuffs/libpasty/__init__.py
--rwxr-xr-x   0        0        0     1981 2024-04-07 11:39:45.271696 noobstuffs-2.0.1/NoobStuffs/libtelegrambot/__init__.py
--rw-r--r--   0        0        0     2724 2024-04-07 07:05:32.639477 noobstuffs-2.0.1/NoobStuffs/libtelegraph/__init__.py
--rw-r--r--   0        0        0      604 2022-11-19 04:49:54.687784 noobstuffs-2.0.1/README.md
--rw-r--r--   0        0        0      805 2024-04-07 11:40:23.305548 noobstuffs-2.0.1/pyproject.toml
--rw-r--r--   0        0        0     1515 1970-01-01 00:00:00.000000 noobstuffs-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0      797 2024-04-07 12:58:05.080759 noobstuffs-2.0.2/NoobStuffs/__init__.py
+-rw-r--r--   0        0        0     2085 2022-11-19 04:49:54.617779 noobstuffs-2.0.2/NoobStuffs/libandroid/__init__.py
+-rw-r--r--   0        0        0     1770 2022-11-19 04:49:54.628785 noobstuffs-2.0.2/NoobStuffs/libdatetime/__init__.py
+-rw-r--r--   0        0        0     4477 2022-11-19 04:49:54.638787 noobstuffs-2.0.2/NoobStuffs/libformatter/__init__.py
+-rw-r--r--   0        0        0     1473 2022-11-19 04:49:54.646774 noobstuffs-2.0.2/NoobStuffs/libformatter/escape.py
+-rw-r--r--   0        0        0     3414 2022-11-19 04:49:54.655784 noobstuffs-2.0.2/NoobStuffs/libgithub/__init__.py
+-rw-r--r--   0        0        0     2540 2022-11-19 04:49:54.664783 noobstuffs-2.0.2/NoobStuffs/liblogging/__init__.py
+-rw-r--r--   0        0        0     1443 2022-11-19 04:49:54.673781 noobstuffs-2.0.2/NoobStuffs/libpasty/__init__.py
+-rwxr-xr-x   0        0        0     1914 2024-04-07 12:57:14.898248 noobstuffs-2.0.2/NoobStuffs/libtelegrambot/__init__.py
+-rw-r--r--   0        0        0     2724 2024-04-07 07:05:32.639477 noobstuffs-2.0.2/NoobStuffs/libtelegraph/__init__.py
+-rw-r--r--   0        0        0      604 2022-11-19 04:49:54.687784 noobstuffs-2.0.2/README.md
+-rw-r--r--   0        0        0      805 2024-04-07 12:58:10.975919 noobstuffs-2.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1515 1970-01-01 00:00:00.000000 noobstuffs-2.0.2/PKG-INFO
```

### Comparing `noobstuffs-2.0.1/NoobStuffs/__init__.py` & `noobstuffs-2.0.2/NoobStuffs/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,8 +14,8 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 #
 
-__version__ = "2.0.1"
+__version__ = "2.0.2"
```

### Comparing `noobstuffs-2.0.1/NoobStuffs/libandroid/__init__.py` & `noobstuffs-2.0.2/NoobStuffs/libandroid/__init__.py`

 * *Files identical despite different names*

### Comparing `noobstuffs-2.0.1/NoobStuffs/libdatetime/__init__.py` & `noobstuffs-2.0.2/NoobStuffs/libdatetime/__init__.py`

 * *Files identical despite different names*

### Comparing `noobstuffs-2.0.1/NoobStuffs/libformatter/__init__.py` & `noobstuffs-2.0.2/NoobStuffs/libformatter/__init__.py`

 * *Files identical despite different names*

### Comparing `noobstuffs-2.0.1/NoobStuffs/libformatter/escape.py` & `noobstuffs-2.0.2/NoobStuffs/libformatter/escape.py`

 * *Files identical despite different names*

### Comparing `noobstuffs-2.0.1/NoobStuffs/libgithub/__init__.py` & `noobstuffs-2.0.2/NoobStuffs/libgithub/__init__.py`

 * *Files identical despite different names*

### Comparing `noobstuffs-2.0.1/NoobStuffs/liblogging/__init__.py` & `noobstuffs-2.0.2/NoobStuffs/liblogging/__init__.py`

 * *Files identical despite different names*

### Comparing `noobstuffs-2.0.1/NoobStuffs/libpasty/__init__.py` & `noobstuffs-2.0.2/NoobStuffs/libpasty/__init__.py`

 * *Files identical despite different names*

### Comparing `noobstuffs-2.0.1/NoobStuffs/libtelegrambot/__init__.py` & `noobstuffs-2.0.2/NoobStuffs/libtelegrambot/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,16 +11,14 @@
         self.__app = ApplicationBuilder().token(token).build()
         self.__chat_id = chat_id
         self.__parse_mode = parse_mode
         self.__buttons = []
         self.__button_index = -1
 
     def build_button(self, text: str, link: str, newline: bool = False):
-        print(self.__button_index)
-        print(self.__buttons)
         button = InlineKeyboardButton(text=text, url=link)
         if newline or len(self.__buttons) == 0:
             self.__button_index += 1
             self.__buttons.append([button])
         else:
             self.__buttons[self.__button_index].append(button)
```

### Comparing `noobstuffs-2.0.1/NoobStuffs/libtelegraph/__init__.py` & `noobstuffs-2.0.2/NoobStuffs/libtelegraph/__init__.py`

 * *Files identical despite different names*

### Comparing `noobstuffs-2.0.1/README.md` & `noobstuffs-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `noobstuffs-2.0.1/pyproject.toml` & `noobstuffs-2.0.2/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "NoobStuffs"
-version = "2.0.1"
+version = "2.0.2"
 description = "Python Library for PrajjuS Projects"
 license = "GPL-3.0"
 authors = ["PrajjuS <theprajjus@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/PrajjuS/NoobStuffs"
 keywords = ["noobstuffs", "libs", "noob", "lazy"]
 classifiers = [
```

### Comparing `noobstuffs-2.0.1/PKG-INFO` & `noobstuffs-2.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NoobStuffs
-Version: 2.0.1
+Version: 2.0.2
 Summary: Python Library for PrajjuS Projects
 Home-page: https://github.com/PrajjuS/NoobStuffs
 License: GPL-3.0
 Keywords: noobstuffs,libs,noob,lazy
 Author: PrajjuS
 Author-email: theprajjus@gmail.com
 Requires-Python: >=3.8,<4.0
```

