# Comparing `tmp/fasttrackpy-0.4.1.tar.gz` & `tmp/fasttrackpy-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fasttrackpy-0.4.1.tar", max compression
+gzip compressed data, was "fasttrackpy-0.4.2.tar", max compression
```

## Comparing `fasttrackpy-0.4.1.tar` & `fasttrackpy-0.4.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1072 2023-11-15 22:25:59.747254 fasttrackpy-0.4.1/LICENSE
--rw-r--r--   0        0        0      889 2024-03-14 21:53:55.296369 fasttrackpy-0.4.1/README.md
--rw-r--r--   0        0        0     1708 2024-03-22 21:33:24.711117 fasttrackpy-0.4.1/pyproject.toml
--rw-r--r--   0        0        0      629 2023-11-28 04:58:49.197727 fasttrackpy-0.4.1/src/fasttrackpy/__init__.py
--rw-r--r--   0        0        0    17445 2024-03-13 17:49:48.608913 fasttrackpy-0.4.1/src/fasttrackpy/cli.py
--rw-r--r--   0        0        0        0 2023-11-15 22:25:59.749448 fasttrackpy-0.4.1/src/fasttrackpy/patterns/__init__.py
--rw-r--r--   0        0        0     6223 2024-03-22 21:32:36.644068 fasttrackpy-0.4.1/src/fasttrackpy/patterns/audio_textgrid.py
--rw-r--r--   0        0        0     7550 2024-03-22 21:32:36.644304 fasttrackpy-0.4.1/src/fasttrackpy/patterns/corpus.py
--rw-r--r--   0        0        0     7249 2024-03-22 21:32:36.644532 fasttrackpy-0.4.1/src/fasttrackpy/patterns/just_audio.py
--rw-r--r--   0        0        0        0 2023-11-15 22:11:10.457070 fasttrackpy-0.4.1/src/fasttrackpy/processors/__init__.py
--rw-r--r--   0        0        0      844 2023-11-15 22:25:59.749799 fasttrackpy-0.4.1/src/fasttrackpy/processors/aggs.py
--rw-r--r--   0        0        0     1753 2023-11-15 22:25:59.749908 fasttrackpy-0.4.1/src/fasttrackpy/processors/losses.py
--rw-r--r--   0        0        0    12686 2024-03-22 21:32:36.644723 fasttrackpy-0.4.1/src/fasttrackpy/processors/outputs.py
--rw-r--r--   0        0        0     3277 2023-11-27 01:47:20.549714 fasttrackpy-0.4.1/src/fasttrackpy/processors/smoothers.py
--rw-r--r--   0        0        0        0 2023-11-27 01:47:20.549781 fasttrackpy-0.4.1/src/fasttrackpy/resources/config.yml
--rw-r--r--   0        0        0    19345 2024-03-22 21:32:36.644915 fasttrackpy-0.4.1/src/fasttrackpy/tracks.py
--rw-r--r--   0        0        0     2467 1970-01-01 00:00:00.000000 fasttrackpy-0.4.1/setup.py
--rw-r--r--   0        0        0     2250 1970-01-01 00:00:00.000000 fasttrackpy-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-11-15 22:25:59.747254 fasttrackpy-0.4.2/LICENSE
+-rw-r--r--   0        0        0      889 2024-03-14 21:53:55.296369 fasttrackpy-0.4.2/README.md
+-rw-r--r--   0        0        0     1708 2024-04-07 18:52:45.451536 fasttrackpy-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0      629 2023-11-28 04:58:49.197727 fasttrackpy-0.4.2/src/fasttrackpy/__init__.py
+-rw-r--r--   0        0        0    17445 2024-04-07 18:41:19.124172 fasttrackpy-0.4.2/src/fasttrackpy/cli.py
+-rw-r--r--   0        0        0        0 2023-11-15 22:25:59.749448 fasttrackpy-0.4.2/src/fasttrackpy/patterns/__init__.py
+-rw-r--r--   0        0        0     6223 2024-03-22 21:32:36.644068 fasttrackpy-0.4.2/src/fasttrackpy/patterns/audio_textgrid.py
+-rw-r--r--   0        0        0     7550 2024-03-22 21:32:36.644304 fasttrackpy-0.4.2/src/fasttrackpy/patterns/corpus.py
+-rw-r--r--   0        0        0     7249 2024-03-22 21:32:36.644532 fasttrackpy-0.4.2/src/fasttrackpy/patterns/just_audio.py
+-rw-r--r--   0        0        0        0 2023-11-15 22:11:10.457070 fasttrackpy-0.4.2/src/fasttrackpy/processors/__init__.py
+-rw-r--r--   0        0        0      844 2023-11-15 22:25:59.749799 fasttrackpy-0.4.2/src/fasttrackpy/processors/aggs.py
+-rw-r--r--   0        0        0     1753 2023-11-15 22:25:59.749908 fasttrackpy-0.4.2/src/fasttrackpy/processors/losses.py
+-rw-r--r--   0        0        0    12670 2024-04-07 18:52:45.451767 fasttrackpy-0.4.2/src/fasttrackpy/processors/outputs.py
+-rw-r--r--   0        0        0     3277 2023-11-27 01:47:20.549714 fasttrackpy-0.4.2/src/fasttrackpy/processors/smoothers.py
+-rw-r--r--   0        0        0        0 2023-11-27 01:47:20.549781 fasttrackpy-0.4.2/src/fasttrackpy/resources/config.yml
+-rw-r--r--   0        0        0    19345 2024-03-22 21:32:36.644915 fasttrackpy-0.4.2/src/fasttrackpy/tracks.py
+-rw-r--r--   0        0        0     2467 1970-01-01 00:00:00.000000 fasttrackpy-0.4.2/setup.py
+-rw-r--r--   0        0        0     2250 1970-01-01 00:00:00.000000 fasttrackpy-0.4.2/PKG-INFO
```

### Comparing `fasttrackpy-0.4.1/LICENSE` & `fasttrackpy-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fasttrackpy-0.4.1/README.md` & `fasttrackpy-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `fasttrackpy-0.4.1/pyproject.toml` & `fasttrackpy-0.4.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fasttrackpy"
-version = "0.4.1"
+version = "0.4.2"
 description = "A python implementation of FastTrack"
 authors = [
     "JoFrhwld <JoFrhwld@gmail.com>",
     "santiagobarreda <sbarreda@ucdavis.edu>"
 ]
 license = "MIT"
 readme = "README.md"
@@ -18,15 +18,15 @@
 repository = "https://github.com/FastTrackiverse/fasttrackpy"
 
 [tool.poetry.dependencies]
 python = ">=3.10,<3.12"
 praat-parselmouth = "^0.4.3"
 scipy = {version = "^1.11.3", python = ">=3.10,<3.12"}
 numpy = {version = "^1.26.1", python = ">=3.10,<3.12"}
-polars = "^0.19.16"
+polars = "^0.20.18"
 pytest-cov = "^4.1.0"
 pytest = "^7.4.3"
 python-magic = {version = "^0.4.27", markers = "sys_platform != 'win32'"}
 python-magic-bin = {version = "^0.4.14", markers = "sys_platform == 'win32'"}
 click = "^8.1.7"
 cloup = "^3.0.3"
 matplotlib = "^3.8.2"
```

### Comparing `fasttrackpy-0.4.1/src/fasttrackpy/__init__.py` & `fasttrackpy-0.4.2/src/fasttrackpy/__init__.py`

 * *Files identical despite different names*

### Comparing `fasttrackpy-0.4.1/src/fasttrackpy/cli.py` & `fasttrackpy-0.4.2/src/fasttrackpy/cli.py`

 * *Files identical despite different names*

### Comparing `fasttrackpy-0.4.1/src/fasttrackpy/patterns/audio_textgrid.py` & `fasttrackpy-0.4.2/src/fasttrackpy/patterns/audio_textgrid.py`

 * *Files identical despite different names*

### Comparing `fasttrackpy-0.4.1/src/fasttrackpy/patterns/corpus.py` & `fasttrackpy-0.4.2/src/fasttrackpy/patterns/corpus.py`

 * *Files identical despite different names*

### Comparing `fasttrackpy-0.4.1/src/fasttrackpy/patterns/just_audio.py` & `fasttrackpy-0.4.2/src/fasttrackpy/patterns/just_audio.py`

 * *Files identical despite different names*

### Comparing `fasttrackpy-0.4.1/src/fasttrackpy/processors/aggs.py` & `fasttrackpy-0.4.2/src/fasttrackpy/processors/aggs.py`

 * *Files identical despite different names*

### Comparing `fasttrackpy-0.4.1/src/fasttrackpy/processors/losses.py` & `fasttrackpy-0.4.2/src/fasttrackpy/processors/losses.py`

 * *Files identical despite different names*

### Comparing `fasttrackpy-0.4.1/src/fasttrackpy/processors/outputs.py` & `fasttrackpy-0.4.2/src/fasttrackpy/processors/outputs.py`

 * *Files 1% similar despite different names*

```diff
@@ -243,15 +243,15 @@
     all_cols = [x for x in formant_cols+smooth_cols if x in data.columns]
 
     data = data\
         .select(["time"]+all_cols)\
         .melt(id_vars = "time")\
         .with_columns(
             pl.col("variable")\
-            .replace(mapping=ptolmap)\
+            .replace(ptolmap)\
             .alias("color")
             )
 
     if tracks:
         mp.scatter(x = "time",
                    y="value",
                    c="color",
@@ -344,15 +344,15 @@
             all_cols = [x for x in formant_cols+smooth_cols if x in data.columns]
 
             data = data\
                 .select(["time"]+all_cols)\
                 .melt(id_vars = "time")\
                 .with_columns(
                     pl.col("variable")\
-                    .replace(mapping=ptolmap)\
+                    .replace(ptolmap)\
                     .alias("color")
                 )
 
             axs[i,j].scatter(
                 x = "time",
                 y = "value",
                 c = "color",
```

### Comparing `fasttrackpy-0.4.1/src/fasttrackpy/processors/smoothers.py` & `fasttrackpy-0.4.2/src/fasttrackpy/processors/smoothers.py`

 * *Files identical despite different names*

### Comparing `fasttrackpy-0.4.1/src/fasttrackpy/tracks.py` & `fasttrackpy-0.4.2/src/fasttrackpy/tracks.py`

 * *Files identical despite different names*

### Comparing `fasttrackpy-0.4.1/setup.py` & `fasttrackpy-0.4.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 install_requires = \
 ['aligned-textgrid>=0.6.2,<0.7.0',
  'click>=8.1.7,<9.0.0',
  'cloup>=3.0.3,<4.0.0',
  'joblib>=1.3.2,<2.0.0',
  'matplotlib>=3.8.2,<4.0.0',
- 'polars>=0.19.16,<0.20.0',
+ 'polars>=0.20.18,<0.21.0',
  'praat-parselmouth>=0.4.3,<0.5.0',
  'pytest-cov>=4.1.0,<5.0.0',
  'pytest>=7.4.3,<8.0.0',
  'pyyaml>=6.0.1,<7.0.0',
  'tqdm>=4.66.1,<5.0.0']
 
 extras_require = \
@@ -30,15 +30,15 @@
  ':sys_platform == "win32"': ['python-magic-bin>=0.4.14,<0.5.0']}
 
 entry_points = \
 {'console_scripts': ['fasttrack = fasttrackpy.cli:fasttrack']}
 
 setup_kwargs = {
     'name': 'fasttrackpy',
-    'version': '0.4.1',
+    'version': '0.4.2',
     'description': 'A python implementation of FastTrack',
     'long_description': '# FastTrackPy\n[![PyPI](https://img.shields.io/pypi/v/fasttrackpy)](https://pypi.org/project/fasttrackpy/)\n[![Python CI](https://github.com/JoFrhwld/fasttrackpy/actions/workflows/test-and-run.yml/badge.svg)](https://github.com/JoFrhwld/fasttrackpy/actions/workflows/test-and-run.yml) [![codecov](https://codecov.io/gh/FastTrackiverse/fasttrackpy/graph/badge.svg?token=GOAWY4B5C8)](https://codecov.io/gh/FastTrackiverse/fasttrackpy) <a href="https://codeclimate.com/github/JoFrhwld/fasttrackpy/maintainability"><img src="https://api.codeclimate.com/v1/badges/6725fded174b21a3c59f/maintainability" /></a> [![DOI](https://zenodo.org/badge/580169086.svg)](https://zenodo.org/badge/latestdoi/580169086)\n\n\nGoal: A FastTrack python implementation with importable modules\n\n## Installation\n\n```bash\npip install fasttrackpy\n```\n\n## Usage\n\n```bash\nfasttrack --file audio.wav --output formants.csv\n```\n',
     'author': 'JoFrhwld',
     'author_email': 'JoFrhwld@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://fasttrackiverse.github.io/fasttrackpy/',
```

#### html2text {}

```diff
@@ -1,21 +1,21 @@
 # -*- coding: utf-8 -*- from setuptools import setup package_dir = \ {'':
 'src'} packages = \ ['fasttrackpy', 'fasttrackpy.patterns',
 'fasttrackpy.processors'] package_data = \ {'': ['*'], 'fasttrackpy':
 ['resources/*']} install_requires = \ ['aligned-textgrid>=0.6.2,<0.7.0',
 'click>=8.1.7,<9.0.0', 'cloup>=3.0.3,<4.0.0', 'joblib>=1.3.2,<2.0.0',
-'matplotlib>=3.8.2,<4.0.0', 'polars>=0.19.16,<0.20.0', 'praat-
+'matplotlib>=3.8.2,<4.0.0', 'polars>=0.20.18,<0.21.0', 'praat-
 parselmouth>=0.4.3,<0.5.0', 'pytest-cov>=4.1.0,<5.0.0', 'pytest>=7.4.3,<8.0.0',
 'pyyaml>=6.0.1,<7.0.0', 'tqdm>=4.66.1,<5.0.0'] extras_require = \ {':
 python_version >= "3.10" and python_version < "3.12"': ['scipy>=1.11.3,<2.0.0',
 'numpy>=1.26.1,<2.0.0'], ':sys_platform != "win32"': ['python-
 magic>=0.4.27,<0.5.0'], ':sys_platform == "win32"': ['python-magic-
 bin>=0.4.14,<0.5.0']} entry_points = \ {'console_scripts': ['fasttrack =
 fasttrackpy.cli:fasttrack']} setup_kwargs = { 'name': 'fasttrackpy', 'version':
-'0.4.1', 'description': 'A python implementation of FastTrack',
+'0.4.2', 'description': 'A python implementation of FastTrack',
 'long_description': '# FastTrackPy\n[![PyPI](https://img.shields.io/pypi/v/
 fasttrackpy)](https://pypi.org/project/fasttrackpy/)\n[![Python CI](https://
 github.com/JoFrhwld/fasttrackpy/actions/workflows/test-and-run.yml/badge.svg)]
 (https://github.com/JoFrhwld/fasttrackpy/actions/workflows/test-and-run.yml) [!
 [codecov](https://codecov.io/gh/FastTrackiverse/fasttrackpy/graph/
 badge.svg?token=GOAWY4B5C8)](https://codecov.io/gh/FastTrackiverse/fasttrackpy)
 _[_h_t_t_p_s_:_/_/_a_p_i_._c_o_d_e_c_l_i_m_a_t_e_._c_o_m_/_v_1_/_b_a_d_g_e_s_/_6_7_2_5_f_d_e_d_1_7_4_b_2_1_a_3_c_5_9_f_/_m_a_i_n_t_a_i_n_a_b_i_l_i_t_y_][!
```

### Comparing `fasttrackpy-0.4.1/PKG-INFO` & `fasttrackpy-0.4.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fasttrackpy
-Version: 0.4.1
+Version: 0.4.2
 Summary: A python implementation of FastTrack
 Home-page: https://fasttrackiverse.github.io/fasttrackpy/
 License: MIT
 Author: JoFrhwld
 Author-email: JoFrhwld@gmail.com
 Requires-Python: >=3.10,<3.12
 Classifier: License :: OSI Approved :: MIT License
@@ -13,15 +13,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aligned-textgrid (>=0.6.2,<0.7.0)
 Requires-Dist: click (>=8.1.7,<9.0.0)
 Requires-Dist: cloup (>=3.0.3,<4.0.0)
 Requires-Dist: joblib (>=1.3.2,<2.0.0)
 Requires-Dist: matplotlib (>=3.8.2,<4.0.0)
 Requires-Dist: numpy (>=1.26.1,<2.0.0) ; python_version >= "3.10" and python_version < "3.12"
-Requires-Dist: polars (>=0.19.16,<0.20.0)
+Requires-Dist: polars (>=0.20.18,<0.21.0)
 Requires-Dist: praat-parselmouth (>=0.4.3,<0.5.0)
 Requires-Dist: pytest (>=7.4.3,<8.0.0)
 Requires-Dist: pytest-cov (>=4.1.0,<5.0.0)
 Requires-Dist: python-magic (>=0.4.27,<0.5.0) ; sys_platform != "win32"
 Requires-Dist: python-magic-bin (>=0.4.14,<0.5.0) ; sys_platform == "win32"
 Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
 Requires-Dist: scipy (>=1.11.3,<2.0.0) ; python_version >= "3.10" and python_version < "3.12"
```

#### html2text {}

```diff
@@ -1,18 +1,18 @@
-Metadata-Version: 2.1 Name: fasttrackpy Version: 0.4.1 Summary: A python
+Metadata-Version: 2.1 Name: fasttrackpy Version: 0.4.2 Summary: A python
 implementation of FastTrack Home-page: https://fasttrackiverse.github.io/
 fasttrackpy/ License: MIT Author: JoFrhwld Author-email: JoFrhwld@gmail.com
 Requires-Python: >=3.10,<3.12 Classifier: License :: OSI Approved :: MIT
 License Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aligned-textgrid (>=0.6.2,<0.7.0) Requires-Dist: click
 (>=8.1.7,<9.0.0) Requires-Dist: cloup (>=3.0.3,<4.0.0) Requires-Dist: joblib
 (>=1.3.2,<2.0.0) Requires-Dist: matplotlib (>=3.8.2,<4.0.0) Requires-Dist:
 numpy (>=1.26.1,<2.0.0) ; python_version >= "3.10" and python_version < "3.12"
-Requires-Dist: polars (>=0.19.16,<0.20.0) Requires-Dist: praat-parselmouth
+Requires-Dist: polars (>=0.20.18,<0.21.0) Requires-Dist: praat-parselmouth
 (>=0.4.3,<0.5.0) Requires-Dist: pytest (>=7.4.3,<8.0.0) Requires-Dist: pytest-
 cov (>=4.1.0,<5.0.0) Requires-Dist: python-magic (>=0.4.27,<0.5.0) ;
 sys_platform != "win32" Requires-Dist: python-magic-bin (>=0.4.14,<0.5.0) ;
 sys_platform == "win32" Requires-Dist: pyyaml (>=6.0.1,<7.0.0) Requires-Dist:
 scipy (>=1.11.3,<2.0.0) ; python_version >= "3.10" and python_version < "3.12"
 Requires-Dist: tqdm (>=4.66.1,<5.0.0) Project-URL: Repository, https://
 github.com/FastTrackiverse/fasttrackpy Description-Content-Type: text/markdown
```

