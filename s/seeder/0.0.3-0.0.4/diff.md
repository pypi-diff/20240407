# Comparing `tmp/seeder-0.0.3.tar.gz` & `tmp/seeder-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seeder-0.0.3.tar", last modified: Sat Apr  6 13:48:16 2024, max compression
+gzip compressed data, was "seeder-0.0.4.tar", last modified: Sun Apr  7 13:19:34 2024, max compression
```

## Comparing `seeder-0.0.3.tar` & `seeder-0.0.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2024-04-06 13:48:16.009433 seeder-0.0.3/
--rw-r--r--   0 solst      (501) staff       (20)    11337 2024-04-06 12:52:34.000000 seeder-0.0.3/LICENSE
--rw-r--r--   0 solst      (501) staff       (20)      111 2024-04-06 12:52:34.000000 seeder-0.0.3/MANIFEST.in
--rw-r--r--   0 solst      (501) staff       (20)     3533 2024-04-06 13:48:16.009058 seeder-0.0.3/PKG-INFO
--rw-r--r--   0 solst      (501) staff       (20)     2704 2024-04-06 13:33:05.000000 seeder-0.0.3/README.md
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2024-04-06 13:48:16.007027 seeder-0.0.3/seeder/
--rw-r--r--   0 solst      (501) staff       (20)      319 2024-04-06 13:47:27.000000 seeder-0.0.3/seeder/__init__.py
--rw-r--r--   0 solst      (501) staff       (20)     1761 2024-04-06 13:47:27.000000 seeder-0.0.3/seeder/_modidx.py
--rw-r--r--   0 solst      (501) staff       (20)     7219 2024-04-06 13:47:27.000000 seeder-0.0.3/seeder/core.py
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2024-04-06 13:48:16.008039 seeder-0.0.3/seeder.egg-info/
--rw-r--r--   0 solst      (501) staff       (20)     3533 2024-04-06 13:48:15.000000 seeder-0.0.3/seeder.egg-info/PKG-INFO
--rw-r--r--   0 solst      (501) staff       (20)      314 2024-04-06 13:48:15.000000 seeder-0.0.3/seeder.egg-info/SOURCES.txt
--rw-r--r--   0 solst      (501) staff       (20)        1 2024-04-06 13:48:15.000000 seeder-0.0.3/seeder.egg-info/dependency_links.txt
--rw-r--r--   0 solst      (501) staff       (20)       34 2024-04-06 13:48:15.000000 seeder-0.0.3/seeder.egg-info/entry_points.txt
--rw-r--r--   0 solst      (501) staff       (20)        1 2024-04-06 13:36:40.000000 seeder-0.0.3/seeder.egg-info/not-zip-safe
--rw-r--r--   0 solst      (501) staff       (20)       67 2024-04-06 13:48:15.000000 seeder-0.0.3/seeder.egg-info/requires.txt
--rw-r--r--   0 solst      (501) staff       (20)        7 2024-04-06 13:48:15.000000 seeder-0.0.3/seeder.egg-info/top_level.txt
--rw-r--r--   0 solst      (501) staff       (20)      847 2024-04-06 13:44:22.000000 seeder-0.0.3/settings.ini
--rw-r--r--   0 solst      (501) staff       (20)       38 2024-04-06 13:48:16.009503 seeder-0.0.3/setup.cfg
--rw-r--r--   0 solst      (501) staff       (20)     2585 2024-04-06 12:52:34.000000 seeder-0.0.3/setup.py
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2024-04-07 13:19:34.023337 seeder-0.0.4/
+-rw-r--r--   0 solst      (501) staff       (20)    11337 2024-04-06 12:52:34.000000 seeder-0.0.4/LICENSE
+-rw-r--r--   0 solst      (501) staff       (20)      111 2024-04-06 12:52:34.000000 seeder-0.0.4/MANIFEST.in
+-rw-r--r--   0 solst      (501) staff       (20)     3335 2024-04-07 13:19:34.023198 seeder-0.0.4/PKG-INFO
+-rw-r--r--   0 solst      (501) staff       (20)     2752 2024-04-06 13:54:46.000000 seeder-0.0.4/README.md
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2024-04-07 13:19:34.022064 seeder-0.0.4/seeder/
+-rw-r--r--   0 solst      (501) staff       (20)      319 2024-04-07 13:19:31.000000 seeder-0.0.4/seeder/__init__.py
+-rw-r--r--   0 solst      (501) staff       (20)     1672 2024-04-07 13:19:31.000000 seeder-0.0.4/seeder/_modidx.py
+-rw-r--r--   0 solst      (501) staff       (20)     7094 2024-04-07 13:19:31.000000 seeder-0.0.4/seeder/core.py
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2024-04-07 13:19:34.022998 seeder-0.0.4/seeder.egg-info/
+-rw-r--r--   0 solst      (501) staff       (20)     3335 2024-04-07 13:19:33.000000 seeder-0.0.4/seeder.egg-info/PKG-INFO
+-rw-r--r--   0 solst      (501) staff       (20)      314 2024-04-07 13:19:33.000000 seeder-0.0.4/seeder.egg-info/SOURCES.txt
+-rw-r--r--   0 solst      (501) staff       (20)        1 2024-04-07 13:19:33.000000 seeder-0.0.4/seeder.egg-info/dependency_links.txt
+-rw-r--r--   0 solst      (501) staff       (20)       34 2024-04-07 13:19:33.000000 seeder-0.0.4/seeder.egg-info/entry_points.txt
+-rw-r--r--   0 solst      (501) staff       (20)        1 2024-04-06 13:36:40.000000 seeder-0.0.4/seeder.egg-info/not-zip-safe
+-rw-r--r--   0 solst      (501) staff       (20)       72 2024-04-07 13:19:33.000000 seeder-0.0.4/seeder.egg-info/requires.txt
+-rw-r--r--   0 solst      (501) staff       (20)        7 2024-04-07 13:19:33.000000 seeder-0.0.4/seeder.egg-info/top_level.txt
+-rw-r--r--   0 solst      (501) staff       (20)      851 2024-04-07 13:11:28.000000 seeder-0.0.4/settings.ini
+-rw-r--r--   0 solst      (501) staff       (20)       38 2024-04-07 13:19:34.023388 seeder-0.0.4/setup.cfg
+-rw-r--r--   0 solst      (501) staff       (20)     2585 2024-04-06 12:52:34.000000 seeder-0.0.4/setup.py
```

### Comparing `seeder-0.0.3/LICENSE` & `seeder-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `seeder-0.0.3/PKG-INFO` & `seeder-0.0.4/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,70 +1,64 @@
 Metadata-Version: 2.1
 Name: seeder
-Version: 0.0.3
+Version: 0.0.4
 Summary: util torch
 Home-page: https://github.com/dsm-72/seeder
 Author: dsm-72
 Author-email: sumner.magruder@yale.edu
 License: Apache Software License 2.0
 Keywords: utility for seeding
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
-License-File: LICENSE
 Provides-Extra: dev
-Requires-Dist: numpy; extra == "dev"
-Requires-Dist: pandas; extra == "dev"
-Requires-Dist: matplotlib; extra == "dev"
-Requires-Dist: torch; extra == "dev"
-Requires-Dist: pytorch_lightning; extra == "dev"
-Requires-Dist: torchvision; extra == "dev"
+License-File: LICENSE
 
-# sow
+# seeder
 
 <!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
 
 ## Developer Guide
 
 ### Setup
 
 ``` sh
 # create conda environment
 $ mamba env create -f env.yml
 
 # update conda environment
-$ mamba env update -n sow --file env.yml
+$ mamba env update -n seeder --file env.yml
 ```
 
 ### Install
 
 ``` sh
 pip install -e .
 
 # install from pypi
-pip install sow
+pip install seeder
 ```
 
 ### nbdev
 
 ``` sh
 # activate conda environment
-$ conda activate sow
+$ conda activate seeder
 
-# make sure the sow package is installed in development mode
+# make sure the seeder package is installed in development mode
 $ pip install -e .
 
 # make changes under nbs/ directory
 # ...
 
-# compile to have changes apply to the sow package
+# compile to have changes apply to the seeder package
 $ nbdev_prepare
 ```
 
 ### Publishing
 
 ``` sh
 # publish to pypi
@@ -76,40 +70,40 @@
 ```
 
 # Usage
 
 ## Installation
 
 Install latest from the GitHub
-[repository](https://github.com/dsm-72/sow):
+[repository](https://github.com/dsm-72/seeder):
 
 ``` sh
-$ pip install git+https://github.com/dsm-72/sow.git
+$ pip install git+https://github.com/dsm-72/seeder.git
 ```
 
-or from [conda](https://anaconda.org/dsm-72/sow)
+or from [conda](https://anaconda.org/dsm-72/seeder)
 
 ``` sh
-$ conda install -c dsm-72 sow
+$ conda install -c dsm-72 seeder
 ```
 
-or from [pypi](https://pypi.org/project/sow/)
+or from [pypi](https://pypi.org/project/seeder/)
 
 ``` sh
-$ pip install sow
+$ pip install seeder
 ```
 
 ## Documentation
 
 Documentation can be found hosted on GitHub
-[repository](https://github.com/dsm-72/sow)
-[pages](https://dsm-72.github.io/sow/). Additionally you can find
+[repository](https://github.com/dsm-72/seeder)
+[pages](https://dsm-72.github.io/seeder/). Additionally you can find
 package manager specific guidelines on
-[conda](https://anaconda.org/dsm-72/sow) and
-[pypi](https://pypi.org/project/sow/) respectively.
+[conda](https://anaconda.org/dsm-72/seeder) and
+[pypi](https://pypi.org/project/seeder/) respectively.
 
 ## NumPy Documentation:
 
 - [`np.DataSource`](https://numpy.org/doc/stable/reference/generated/numpy.DataSource.html)
 
 ## PyTorch Documentation:
```

### Comparing `seeder-0.0.3/README.md` & `seeder-0.0.4/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,45 +1,45 @@
-# sow
+# seeder
 
 <!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
 
 ## Developer Guide
 
 ### Setup
 
 ``` sh
 # create conda environment
 $ mamba env create -f env.yml
 
 # update conda environment
-$ mamba env update -n sow --file env.yml
+$ mamba env update -n seeder --file env.yml
 ```
 
 ### Install
 
 ``` sh
 pip install -e .
 
 # install from pypi
-pip install sow
+pip install seeder
 ```
 
 ### nbdev
 
 ``` sh
 # activate conda environment
-$ conda activate sow
+$ conda activate seeder
 
-# make sure the sow package is installed in development mode
+# make sure the seeder package is installed in development mode
 $ pip install -e .
 
 # make changes under nbs/ directory
 # ...
 
-# compile to have changes apply to the sow package
+# compile to have changes apply to the seeder package
 $ nbdev_prepare
 ```
 
 ### Publishing
 
 ``` sh
 # publish to pypi
@@ -51,40 +51,40 @@
 ```
 
 # Usage
 
 ## Installation
 
 Install latest from the GitHub
-[repository](https://github.com/dsm-72/sow):
+[repository](https://github.com/dsm-72/seeder):
 
 ``` sh
-$ pip install git+https://github.com/dsm-72/sow.git
+$ pip install git+https://github.com/dsm-72/seeder.git
 ```
 
-or from [conda](https://anaconda.org/dsm-72/sow)
+or from [conda](https://anaconda.org/dsm-72/seeder)
 
 ``` sh
-$ conda install -c dsm-72 sow
+$ conda install -c dsm-72 seeder
 ```
 
-or from [pypi](https://pypi.org/project/sow/)
+or from [pypi](https://pypi.org/project/seeder/)
 
 ``` sh
-$ pip install sow
+$ pip install seeder
 ```
 
 ## Documentation
 
 Documentation can be found hosted on GitHub
-[repository](https://github.com/dsm-72/sow)
-[pages](https://dsm-72.github.io/sow/). Additionally you can find
+[repository](https://github.com/dsm-72/seeder)
+[pages](https://dsm-72.github.io/seeder/). Additionally you can find
 package manager specific guidelines on
-[conda](https://anaconda.org/dsm-72/sow) and
-[pypi](https://pypi.org/project/sow/) respectively.
+[conda](https://anaconda.org/dsm-72/seeder) and
+[pypi](https://pypi.org/project/seeder/) respectively.
 
 ## NumPy Documentation:
 
 - [`np.DataSource`](https://numpy.org/doc/stable/reference/generated/numpy.DataSource.html)
 
 ## PyTorch Documentation:
```

### Comparing `seeder-0.0.3/seeder/_modidx.py` & `seeder-0.0.4/seeder/_modidx.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 d = { 'settings': { 'branch': 'main',
                 'doc_baseurl': '/seeder',
                 'doc_host': 'https://dsm-72.github.io',
                 'git_url': 'https://github.com/dsm-72/seeder',
                 'lib_path': 'seeder'},
   'syms': { 'seeder.core': { 'seeder.core.make_seedfn': ('core.html#make_seedfn', 'seeder/core.py'),
                              'seeder.core.module_name': ('core.html#module_name', 'seeder/core.py'),
-                             'seeder.core.quiet': ('core.html#quiet', 'seeder/core.py'),
                              'seeder.core.seedall': ('core.html#seedall', 'seeder/core.py'),
                              'seeder.core.seeder': ('core.html#seeder', 'seeder/core.py'),
                              'seeder.core.seeder.all': ('core.html#seeder.all', 'seeder/core.py'),
                              'seeder.core.seeder.get': ('core.html#seeder.get', 'seeder/core.py'),
                              'seeder.core.seeder.issown': ('core.html#seeder.issown', 'seeder/core.py'),
                              'seeder.core.seeder.new': ('core.html#seeder.new', 'seeder/core.py'),
                              'seeder.core.seeder.plant': ('core.html#seeder.plant', 'seeder/core.py'),
```

### Comparing `seeder-0.0.3/seeder/core.py` & `seeder-0.0.4/seeder/core.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/00_core.ipynb.
 
 # %% auto 0
-__all__ = ['WRAPS_ASSIGN_ANNDOCS', 'osseed', 'npseed', 'ptseed', 'plseed', 'module_name', 'make_seedfn', 'quiet', 'singleton',
-           'seeder', 'seedall']
+__all__ = ['WRAPS_ASSIGN_ANNDOCS', 'osseed', 'npseed', 'ptseed', 'plseed', 'module_name', 'make_seedfn', 'singleton', 'seeder',
+           'seedall']
 
 # %% ../nbs/00_core.ipynb 6
 import io, logging, warnings
 from contextlib import redirect_stdout, redirect_stderr
 from functools import wraps
-from itertools import takewhile, accumulate
 from importlib import import_module
 
 # %% ../nbs/00_core.ipynb 8
 from types import FunctionType, ModuleType
 from numbers import Number
 from typing import Callable
 
@@ -28,81 +27,70 @@
 
 
 # %% ../nbs/00_core.ipynb 17
 #| export
 
 
 # %% ../nbs/00_core.ipynb 19
-#| export
+from lull import lull
 
 # %% ../nbs/00_core.ipynb 21
 _SEEDED = '_seeded'
 WRAPS_ASSIGN_ANNDOCS = ('__doc__', '__module__', '__annotations__')
 
 # %% ../nbs/00_core.ipynb 22
 def module_name(mo: str | ModuleType):
     if isinstance(mo, ModuleType): mo = mo.__name__
     name, *_ = mo.partition('.')
     return name
 
-def make_seedfn(mo: str | ModuleType, fn: str, alias: str | None = None) -> Callable[[int], int]:
+def make_seedfn(mo: str | ModuleType, fn: str, alias: str | None = None) -> Callable[[int, bool], int]:
     moname = alias or module_name(mo)
     fnname = f'{moname}seed'
     
-    def seedfn(seed: int) -> int:
+    def seedfn(seed: int, __hush: bool = True) -> int:
         f'''Set {moname}'s seed for reproducibility.'''
-        try: 
-            sn: Callable[[int], None] = getattr(import_module(mo), fn)
-            sn(seed)
-            
-        except ImportError: 
-            ...
+        with lull(hush=__hush):
+            try:
+                sn: Callable[[int], None] = getattr(import_module(mo), fn)
+                sn(seed)
+                
+            except ImportError: 
+                ...
+                
             
         return seed
     
     seedfn.__name__ = fnname
     seedfn.__qualname__ = fnname
     return seedfn
 
-
-def quiet(fn: FunctionType):
-    @wraps(fn)
-    def shush(*args, **kwargs):
-        if not kwargs.pop('__hush', False): 
-            return fn(*args, **kwargs)
-        with redirect_stdout(io.StringIO()), redirect_stderr(io.StringIO()):
-            logging.disable(100000)
-            warnings.simplefilter('ignore')
-            try:
-                return fn(*args, **kwargs)
-            except: ...
-    return shush
-
 # %% ../nbs/00_core.ipynb 23
 class singleton(type):
     _fns: dict = dict()
     def __repr__(self) -> str:
         return f'{self.__name__}{{fns = {len(self._fns)}}}'
     ...
 
 class seeder(metaclass=singleton):
     
-    _fns = dict()
+    _fns: dict[str, Callable[[int, bool], int]] = dict()
     
     @classmethod
     def seeded(cls, fn: FunctionType):
         '''Set the seed function attribute `fn._seeded` to `True`.'''
         setattr(fn, _SEEDED, True)
     
     @classmethod
-    def sow(cls, fn: FunctionType, seed: int = 3, reseed: bool = True) -> int:
+    def sow(cls, fn: FunctionType, seed: int = 3, reseed: bool = True, __hush: bool = True) -> int:
         '''Invoke the seed function `fn` with `seed` if it has not yet been called.'''
-        if not cls.issown(fn) or reseed:
-            fn(seed)
-            cls.seeded(fn)
+        with lull(hush=__hush):
+            if not cls.issown(fn) or reseed:
+                fn(seed)
+                cls.seeded(fn)
         return seed
     
     @classmethod
     def issown(cls, fn: FunctionType) -> bool:
         '''Check if seed function `fn` has been called already.'''
         return getattr(fn, _SEEDED, False) 
         
@@ -120,16 +108,15 @@
     @classmethod
     @wraps(plant)
     def new(cls, mo: str | ModuleType, fn: str, alias: str | None = None) -> Callable[[int], int]:
         '''Alias for `seeder.plant`.'''
         return cls.plant(mo, fn, alias)
     
     @classmethod
-    @quiet
-    def all(cls, seed: int = 3, reseed: bool = True) -> int:
+    def all(cls, seed: int = 3, reseed: bool = True, __hush: bool = True) -> int:
         '''Set seeds for reproducibility.
         
         Parameters
         ----------
         seed : int
 
         Returns
@@ -152,17 +139,18 @@
         random.seed, np.random.seed, torch.manual_seed, pl.seed_everything
 
         .. _randomness: https://pytorch.org/docs/stable/notes/randomness.html
         .. _random.seed: https://docs.python.org/3/library/random.html#random.seed
         .. _np.random.seed: https://numpy.org/doc/stable/reference/random/generated/numpy.random.seed.html
         .. _torch.manual_seed: https://pytorch.org/docs/stable/generated/torch.manual_seed.html
         .. _pl.seed_everything: https://pytorch-lightning.readthedocs.io/en/latest/common/seed_everything.html
-        '''    
-        for _, fn in cls._fns.items():
-            cls.sow(fn, seed, reseed)
+        '''
+        with lull(hush=__hush):
+            for _, fn in cls._fns.items():
+                cls.sow(fn, seed, reseed, __hush)
         return seed
     
     @classmethod
     def get(cls, name: str) -> Callable[[int], int] | None:
         return cls._fns.get(name, None)
     
     @classmethod
@@ -172,16 +160,15 @@
 # %% ../nbs/00_core.ipynb 24
 osseed = seeder.new('random', 'seed', 'os')
 npseed = seeder.new('numpy.random', 'seed', 'np')
 ptseed = seeder.new('torch', 'manual_seed', 'pt')
 plseed = seeder.new('lightning', 'seed_everything', 'pl')
 
 # %% ../nbs/00_core.ipynb 25
-@wraps(seeder.all)
-def seedall(seed: int = 3, reseed: bool = True) -> int:
+def seedall(seed: int = 3, reseed: bool = True, __hush: bool = True) -> int:
     '''Set seeds for reproducibility.
         
     Parameters
     ----------
     seed : int
 
     Returns
@@ -197,19 +184,21 @@
     [random.seed](https://docs.python.org/3/library/random.html#random.seed), 
     [np.random.seed](https://numpy.org/doc/stable/reference/random/generated/numpy.random.seed.html),
     [torch.manual_seed](https://pytorch.org/docs/stable/generated/torch.manual_seed.html), and
     [pl.seed_everything]( https://pytorch-lightning.readthedocs.io/en/latest/common/seed_everything.html).
 
     See Also
     --------
+    seeder.all : Alias for `seedall`
     random.seed, np.random.seed, torch.manual_seed, pl.seed_everything
 
     .. _randomness: https://pytorch.org/docs/stable/notes/randomness.html
     .. _random.seed: https://docs.python.org/3/library/random.html#random.seed
     .. _np.random.seed: https://numpy.org/doc/stable/reference/random/generated/numpy.random.seed.html
     .. _torch.manual_seed: https://pytorch.org/docs/stable/generated/torch.manual_seed.html
     .. _pl.seed_everything: https://pytorch-lightning.readthedocs.io/en/latest/common/seed_everything.html
     ''' 
-    return seeder.all(seed, reseed)
+    with lull(hush=__hush):
+        return seeder.all(seed, reseed, __hush)
 
 # %% ../nbs/00_core.ipynb 27
 #| export
```

### Comparing `seeder-0.0.3/seeder.egg-info/PKG-INFO` & `seeder-0.0.4/seeder.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,70 +1,64 @@
 Metadata-Version: 2.1
 Name: seeder
-Version: 0.0.3
+Version: 0.0.4
 Summary: util torch
 Home-page: https://github.com/dsm-72/seeder
 Author: dsm-72
 Author-email: sumner.magruder@yale.edu
 License: Apache Software License 2.0
 Keywords: utility for seeding
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
-License-File: LICENSE
 Provides-Extra: dev
-Requires-Dist: numpy; extra == "dev"
-Requires-Dist: pandas; extra == "dev"
-Requires-Dist: matplotlib; extra == "dev"
-Requires-Dist: torch; extra == "dev"
-Requires-Dist: pytorch_lightning; extra == "dev"
-Requires-Dist: torchvision; extra == "dev"
+License-File: LICENSE
 
-# sow
+# seeder
 
 <!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
 
 ## Developer Guide
 
 ### Setup
 
 ``` sh
 # create conda environment
 $ mamba env create -f env.yml
 
 # update conda environment
-$ mamba env update -n sow --file env.yml
+$ mamba env update -n seeder --file env.yml
 ```
 
 ### Install
 
 ``` sh
 pip install -e .
 
 # install from pypi
-pip install sow
+pip install seeder
 ```
 
 ### nbdev
 
 ``` sh
 # activate conda environment
-$ conda activate sow
+$ conda activate seeder
 
-# make sure the sow package is installed in development mode
+# make sure the seeder package is installed in development mode
 $ pip install -e .
 
 # make changes under nbs/ directory
 # ...
 
-# compile to have changes apply to the sow package
+# compile to have changes apply to the seeder package
 $ nbdev_prepare
 ```
 
 ### Publishing
 
 ``` sh
 # publish to pypi
@@ -76,40 +70,40 @@
 ```
 
 # Usage
 
 ## Installation
 
 Install latest from the GitHub
-[repository](https://github.com/dsm-72/sow):
+[repository](https://github.com/dsm-72/seeder):
 
 ``` sh
-$ pip install git+https://github.com/dsm-72/sow.git
+$ pip install git+https://github.com/dsm-72/seeder.git
 ```
 
-or from [conda](https://anaconda.org/dsm-72/sow)
+or from [conda](https://anaconda.org/dsm-72/seeder)
 
 ``` sh
-$ conda install -c dsm-72 sow
+$ conda install -c dsm-72 seeder
 ```
 
-or from [pypi](https://pypi.org/project/sow/)
+or from [pypi](https://pypi.org/project/seeder/)
 
 ``` sh
-$ pip install sow
+$ pip install seeder
 ```
 
 ## Documentation
 
 Documentation can be found hosted on GitHub
-[repository](https://github.com/dsm-72/sow)
-[pages](https://dsm-72.github.io/sow/). Additionally you can find
+[repository](https://github.com/dsm-72/seeder)
+[pages](https://dsm-72.github.io/seeder/). Additionally you can find
 package manager specific guidelines on
-[conda](https://anaconda.org/dsm-72/sow) and
-[pypi](https://pypi.org/project/sow/) respectively.
+[conda](https://anaconda.org/dsm-72/seeder) and
+[pypi](https://pypi.org/project/seeder/) respectively.
 
 ## NumPy Documentation:
 
 - [`np.DataSource`](https://numpy.org/doc/stable/reference/generated/numpy.DataSource.html)
 
 ## PyTorch Documentation:
```

### Comparing `seeder-0.0.3/settings.ini` & `seeder-0.0.4/settings.ini`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = seeder
 lib_name = seeder
-version = 0.0.3
+version = 0.0.4
 min_python = 3.11
 license = apache2
 black_formatting = False
 doc_path = _docs
 lib_path = seeder
 nbs_path = nbs
 recursive = True
@@ -29,10 +29,10 @@
 conda_user = dsm-72
 jupyter_hooks = True
 clean_ids = True
 clear_all = False
 readme_nb = index.ipynb
 allowed_metadata_keys = 
 allowed_cell_metadata_keys = 
-requirements = 
+requirements = lull
 dev_requirements = numpy pandas matplotlib torch pytorch_lightning torchvision
```

### Comparing `seeder-0.0.3/setup.py` & `seeder-0.0.4/setup.py`

 * *Files identical despite different names*

