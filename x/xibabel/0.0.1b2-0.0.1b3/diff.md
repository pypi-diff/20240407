# Comparing `tmp/xibabel-0.0.1b2.tar.gz` & `tmp/xibabel-0.0.1b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xibabel-0.0.1b2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "xibabel-0.0.1b3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `xibabel-0.0.1b2.tar` & `xibabel-0.0.1b3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     3241 2024-04-06 17:55:02.342516 xibabel-0.0.1b2/README.md
--rw-r--r--   0        0        0     1172 2024-04-06 22:04:37.266298 xibabel-0.0.1b2/pyproject.toml
--rw-r--r--   0        0        0      200 2024-04-06 22:48:04.482036 xibabel-0.0.1b2/src/xibabel/__init__.py
--rw-r--r--   0        0        0      571 2024-04-06 17:55:02.346667 xibabel-0.0.1b2/src/xibabel/bench/bench_nib_xib_load.py
--rw-r--r--   0        0        0    26374 2024-04-06 17:55:02.346881 xibabel-0.0.1b2/src/xibabel/loaders.py
--rw-r--r--   0        0        0       20 2024-04-06 17:55:02.347197 xibabel-0.0.1b2/src/xibabel/testing/.gitignore
--rw-r--r--   0        0        0     2584 2024-04-06 17:55:02.347343 xibabel-0.0.1b2/src/xibabel/testing/__init__.py
--rw-r--r--   0        0        0      627 2024-04-06 17:55:02.347577 xibabel-0.0.1b2/src/xibabel/testing/__main__.py
--rw-r--r--   0        0        0     5225 2024-04-06 17:55:02.347801 xibabel-0.0.1b2/src/xibabel/testing/fetcher.py
--rw-r--r--   0        0        0      463 2024-04-06 17:55:02.348095 xibabel-0.0.1b2/src/xibabel/testing/test_files.yml
--rw-r--r--   0        0        0      396 2024-04-06 17:55:02.348320 xibabel-0.0.1b2/src/xibabel/testing/test_sets.yml
--rw-r--r--   0        0        0        0 2024-04-06 17:55:02.348361 xibabel-0.0.1b2/src/xibabel/tests/__init__.py
--rw-r--r--   0        0        0     2512 2024-04-06 17:55:02.348672 xibabel-0.0.1b2/src/xibabel/tests/conftest.py
--rw-r--r--   0        0        0      332 2024-04-06 17:55:02.348819 xibabel-0.0.1b2/src/xibabel/tests/markers.py
--rw-r--r--   0        0        0     1306 2024-04-06 17:55:02.349085 xibabel-0.0.1b2/src/xibabel/tests/run_server.py
--rw-r--r--   0        0        0    20938 2024-04-06 17:55:02.349301 xibabel-0.0.1b2/src/xibabel/tests/test_loaders.py
--rw-r--r--   0        0        0     1205 2024-04-06 17:55:02.349677 xibabel-0.0.1b2/src/xibabel/tests/test_merge.py
--rw-r--r--   0        0        0     2855 2024-04-06 17:55:02.349851 xibabel-0.0.1b2/src/xibabel/tests/test_scripting.py
--rw-r--r--   0        0        0     2264 2024-04-06 17:55:02.350007 xibabel-0.0.1b2/src/xibabel/tests/test_testing.py
--rw-r--r--   0        0        0      794 2024-04-06 17:55:02.350222 xibabel-0.0.1b2/src/xibabel/xutils.py
--rw-r--r--   0        0        0     4814 1970-01-01 00:00:00.000000 xibabel-0.0.1b2/PKG-INFO
+-rw-r--r--   0        0        0     3297 2024-04-07 16:19:14.887274 xibabel-0.0.1b3/README.md
+-rw-r--r--   0        0        0     1219 2024-04-07 16:19:14.889269 xibabel-0.0.1b3/pyproject.toml
+-rw-r--r--   0        0        0      200 2024-04-07 16:20:37.174809 xibabel-0.0.1b3/src/xibabel/__init__.py
+-rw-r--r--   0        0        0      571 2024-04-07 15:22:16.624201 xibabel-0.0.1b3/src/xibabel/bench/bench_nib_xib_load.py
+-rw-r--r--   0        0        0    26467 2024-04-07 15:22:16.624535 xibabel-0.0.1b3/src/xibabel/loaders.py
+-rw-r--r--   0        0        0       20 2024-04-07 15:22:16.624850 xibabel-0.0.1b3/src/xibabel/testing/.gitignore
+-rw-r--r--   0        0        0     2584 2024-04-07 15:22:16.625223 xibabel-0.0.1b3/src/xibabel/testing/__init__.py
+-rw-r--r--   0        0        0      627 2024-04-07 15:22:16.625441 xibabel-0.0.1b3/src/xibabel/testing/__main__.py
+-rw-r--r--   0        0        0     5225 2024-04-07 15:22:16.625822 xibabel-0.0.1b3/src/xibabel/testing/fetcher.py
+-rw-r--r--   0        0        0      463 2024-04-07 15:22:16.626137 xibabel-0.0.1b3/src/xibabel/testing/test_files.yml
+-rw-r--r--   0        0        0      396 2024-04-07 15:22:16.626362 xibabel-0.0.1b3/src/xibabel/testing/test_sets.yml
+-rw-r--r--   0        0        0        0 2024-04-07 15:22:16.626413 xibabel-0.0.1b3/src/xibabel/tests/__init__.py
+-rw-r--r--   0        0        0     2512 2024-04-07 15:22:16.626863 xibabel-0.0.1b3/src/xibabel/tests/conftest.py
+-rw-r--r--   0        0        0      332 2024-04-07 15:22:16.627123 xibabel-0.0.1b3/src/xibabel/tests/markers.py
+-rw-r--r--   0        0        0     1306 2024-04-07 15:22:16.627411 xibabel-0.0.1b3/src/xibabel/tests/run_server.py
+-rw-r--r--   0        0        0    20900 2024-04-07 15:22:16.627824 xibabel-0.0.1b3/src/xibabel/tests/test_loaders.py
+-rw-r--r--   0        0        0     1205 2024-04-07 15:22:16.628147 xibabel-0.0.1b3/src/xibabel/tests/test_merge.py
+-rw-r--r--   0        0        0     2855 2024-04-07 15:22:16.628417 xibabel-0.0.1b3/src/xibabel/tests/test_scripting.py
+-rw-r--r--   0        0        0     2264 2024-04-07 15:22:16.628815 xibabel-0.0.1b3/src/xibabel/tests/test_testing.py
+-rw-r--r--   0        0        0      794 2024-04-07 15:22:16.629096 xibabel-0.0.1b3/src/xibabel/xutils.py
+-rw-r--r--   0        0        0     4969 1970-01-01 00:00:00.000000 xibabel-0.0.1b3/PKG-INFO
```

### Comparing `xibabel-0.0.1b2/README.md` & `xibabel-0.0.1b3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -31,24 +31,25 @@
 mean_img = ximg.mean('time')
 
 # Notice that we haven't yet fetched the data.   We do so only when we need
 # it - for example, when plotting the image data:
 plt.imshow(mean_img.sel(k=32))
 ```
 
-See the example notebooks in the `experiments` directory for more.
+See [Xibabel documentation](https://matthew-brett.github.io/xibabel) for more.
 
 ## Features
 
 - Xibabel images are [Xarrays](https://docs.xarray.dev). They have labeled
   axes, with default labels for spatial axes of `i`, `j` and `k`; time is
   `time`. The labels allow slicing operations such as selecting slices over
   time.
-- The labels allow concise and readable operations on named axes. See the
-  `glm_in_xibabel` notebook in the `experiments` directory.
+- The labels allow concise and readable operations on named axes.
+  See the [glm_in_xibabel
+  notebook](https://matthew-brett.github.io/xibabel/glm_with_xibabel) for an example.
 - Xarrays have attributes that can be attached to the image or the axes of the
   image. We can load these attributes from
   [BIDS](https://bids.neuroimaging.io/) format JSON files. This allows better
   transmission of metadata.
 - The Xarrays have a Dask backend, so computations can be deferred and run at
   the point at which you need the data in memory.
 - Xarrays and Dask allow new storage formats, including storage as
```

### Comparing `xibabel-0.0.1b2/pyproject.toml` & `xibabel-0.0.1b3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -31,16 +31,18 @@
     'nbclassic',
     'jupytext',
     'dicom_parser',
     'ipywidgets',
     'zarr'
 ]
 docs = [
-    'sphinx>=7.0',
     'numpydoc>=1.6.0',
+    'mkdocs-jupyter',
+    'mkdocs-gitbook',
+    'mkdocs-exclude',
     'matplotlib',
     'ipython',
     'jupytext',
     'aiohttp'
 ]
 test = [
     'pyyaml',
```

### Comparing `xibabel-0.0.1b2/src/xibabel/bench/bench_nib_xib_load.py` & `xibabel-0.0.1b3/src/xibabel/bench/bench_nib_xib_load.py`

 * *Files identical despite different names*

### Comparing `xibabel-0.0.1b2/src/xibabel/loaders.py` & `xibabel-0.0.1b3/src/xibabel/loaders.py`

 * *Files 2% similar despite different names*

```diff
@@ -263,14 +263,16 @@
     """
 
 
 _JSON_MARKER = '__json__'
 
 
 def _json_attrs2attrs(attrs):
+    """ Read JSON formed for encoding nested structures to netCDF
+    """
     out = {}
     for key, value in attrs.items():
         if (isinstance(value, list) and
             len(value) == 2 and
             value[0] == _JSON_MARKER):
             value = json.loads(value[1])
         out[key] = value
@@ -293,14 +295,16 @@
         return super().default(self, obj)
 
 
 _jdumps = partial(json.dumps, cls=NPEncoder)
 
 
 def _attrs2json_attrs(attrs):
+    """ Write JSON formed for encoding nested structures to netCDF
+    """
     out = {}
     for key, value in attrs.items():
         if (isinstance(value, dict) or
             (isinstance(value, (list, tuple)) and not _1d_arrayable(value))):
             value = [_JSON_MARKER, _jdumps(value)]
         out[key] = value
     return out
@@ -494,15 +498,15 @@
         elif require_json:
             raise XibFileError(
                 f'BIDS loading {url_or_path} but no corresponding '
                 f'{url_json} file, and `require_json` is True')
     img, meta = _nibabel2img_meta(img_file)
     if sidecar_file:
         with sidecar_file as fobj:
-            meta.update(_json_attrs2attrs(json.load(fobj)))
+            meta.update(json.load(fobj))
     return _img_meta2ximg(img, meta, url_or_path)
 
 
 def load_nibabel(url_or_path, **kwargs):
     r""" Load image from Nibabel-format data at `url_or_path`
 
     `url_or_path` may point directly to ``.json`` file, or to Nibabel format
@@ -663,15 +667,14 @@
         Any remaining named arguments passed to `fsspec.open`.
 
     Returns
     -------
     None
     """
     nib_img, attrs = to_nifti(obj)
-    attrs = _attrs2json_attrs(attrs)
     if str(url_or_path).endswith('.json'):
         json_uop = url_or_path
         img_uop = replace_suffix(url_or_path, '.json', '.nii.gz')
     else:
         img_uop = url_or_path
         json_uop = replace_suffix(
             drop_suffix(url_or_path, _comp_exts()),
```

### Comparing `xibabel-0.0.1b2/src/xibabel/testing/__init__.py` & `xibabel-0.0.1b3/src/xibabel/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `xibabel-0.0.1b2/src/xibabel/testing/__main__.py` & `xibabel-0.0.1b3/src/xibabel/testing/__main__.py`

 * *Files identical despite different names*

### Comparing `xibabel-0.0.1b2/src/xibabel/testing/fetcher.py` & `xibabel-0.0.1b3/src/xibabel/testing/fetcher.py`

 * *Files identical despite different names*

### Comparing `xibabel-0.0.1b2/src/xibabel/tests/conftest.py` & `xibabel-0.0.1b3/src/xibabel/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `xibabel-0.0.1b2/src/xibabel/tests/run_server.py` & `xibabel-0.0.1b3/src/xibabel/tests/run_server.py`

 * *Files identical despite different names*

### Comparing `xibabel-0.0.1b2/src/xibabel/tests/test_loaders.py` & `xibabel-0.0.1b3/src/xibabel/tests/test_loaders.py`

 * *Files 0% similar despite different names*

```diff
@@ -553,18 +553,18 @@
     fdata = nib_img.get_fdata()
     ximg = load(img_path)
     out_fname = tmp_path / 'out.json'
     save(ximg, out_fname)
     back_nib = nib.load(tmp_path / 'out.nii.gz')
     assert np.allclose(back_nib.get_fdata(), fdata)
     with open(out_fname, 'rt') as fobj:
-        back_attrs = _json_attrs2attrs(json.load(fobj))
+        back_attrs = json.load(fobj)
     assert arr_dict_allclose(back_attrs, meta)
     assert arr_dict_allclose(load(out_fname).attrs, ximg.attrs)
     out_fname = tmp_path / 'out2.nii'
     save(ximg, out_fname)
     back_nib = nib.load(out_fname)
     assert np.allclose(back_nib.get_fdata(), fdata)
     with open(tmp_path / 'out2.json', 'rt') as fobj:
-        back_attrs = _json_attrs2attrs(json.load(fobj))
+        back_attrs = json.load(fobj)
     assert arr_dict_allclose(back_attrs, meta)
     assert arr_dict_allclose(load(out_fname).attrs, ximg.attrs)
```

### Comparing `xibabel-0.0.1b2/src/xibabel/tests/test_merge.py` & `xibabel-0.0.1b3/src/xibabel/tests/test_merge.py`

 * *Files identical despite different names*

### Comparing `xibabel-0.0.1b2/src/xibabel/tests/test_scripting.py` & `xibabel-0.0.1b3/src/xibabel/tests/test_scripting.py`

 * *Files identical despite different names*

### Comparing `xibabel-0.0.1b2/src/xibabel/tests/test_testing.py` & `xibabel-0.0.1b3/src/xibabel/tests/test_testing.py`

 * *Files identical despite different names*

### Comparing `xibabel-0.0.1b2/src/xibabel/xutils.py` & `xibabel-0.0.1b3/src/xibabel/xutils.py`

 * *Files identical despite different names*

### Comparing `xibabel-0.0.1b2/PKG-INFO` & `xibabel-0.0.1b3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xibabel
-Version: 0.0.1b2
+Version: 0.0.1b3
 Summary: Xibabel neuroimaging interface
 Author-email: Matthew Brett <matthew.brett@gmail.com>, Paul Ivanov <pi@berkeley.edu>, "Christopher J. Markiewicz" <markiewicz@stanford.edu>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Development Status :: 3 - Alpha
 Requires-Dist: xarray
@@ -13,16 +13,18 @@
 Requires-Dist: psutil
 Requires-Dist: pre-commit ; extra == "developer"
 Requires-Dist: nbclassic ; extra == "developer"
 Requires-Dist: jupytext ; extra == "developer"
 Requires-Dist: dicom_parser ; extra == "developer"
 Requires-Dist: ipywidgets ; extra == "developer"
 Requires-Dist: zarr ; extra == "developer"
-Requires-Dist: sphinx>=7.0 ; extra == "docs"
 Requires-Dist: numpydoc>=1.6.0 ; extra == "docs"
+Requires-Dist: mkdocs-jupyter ; extra == "docs"
+Requires-Dist: mkdocs-gitbook ; extra == "docs"
+Requires-Dist: mkdocs-exclude ; extra == "docs"
 Requires-Dist: matplotlib ; extra == "docs"
 Requires-Dist: ipython ; extra == "docs"
 Requires-Dist: jupytext ; extra == "docs"
 Requires-Dist: aiohttp ; extra == "docs"
 Requires-Dist: nipy ; extra == "optional"
 Requires-Dist: h5netcdf ; extra == "optional"
 Requires-Dist: matplotlib ; extra == "optional"
@@ -71,24 +73,25 @@
 mean_img = ximg.mean('time')
 
 # Notice that we haven't yet fetched the data.   We do so only when we need
 # it - for example, when plotting the image data:
 plt.imshow(mean_img.sel(k=32))
 ```
 
-See the example notebooks in the `experiments` directory for more.
+See [Xibabel documentation](https://matthew-brett.github.io/xibabel) for more.
 
 ## Features
 
 - Xibabel images are [Xarrays](https://docs.xarray.dev). They have labeled
   axes, with default labels for spatial axes of `i`, `j` and `k`; time is
   `time`. The labels allow slicing operations such as selecting slices over
   time.
-- The labels allow concise and readable operations on named axes. See the
-  `glm_in_xibabel` notebook in the `experiments` directory.
+- The labels allow concise and readable operations on named axes.
+  See the [glm_in_xibabel
+  notebook](https://matthew-brett.github.io/xibabel/glm_with_xibabel) for an example.
 - Xarrays have attributes that can be attached to the image or the axes of the
   image. We can load these attributes from
   [BIDS](https://bids.neuroimaging.io/) format JSON files. This allows better
   transmission of metadata.
 - The Xarrays have a Dask backend, so computations can be deferred and run at
   the point at which you need the data in memory.
 - Xarrays and Dask allow new storage formats, including storage as
```

