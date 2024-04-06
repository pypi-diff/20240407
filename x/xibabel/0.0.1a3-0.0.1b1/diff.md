# Comparing `tmp/xibabel-0.0.1a3.tar.gz` & `tmp/xibabel-0.0.1b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xibabel-0.0.1a3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "xibabel-0.0.1b1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `xibabel-0.0.1a3.tar` & `xibabel-0.0.1b1.tar`

### file list

```diff
@@ -1,19 +1,21 @@
--rw-r--r--   0        0        0     3029 2024-04-01 23:12:14.443020 xibabel-0.0.1a3/README.md
--rw-r--r--   0        0        0     1176 2024-04-01 23:00:24.571221 xibabel-0.0.1a3/pyproject.toml
--rw-r--r--   0        0        0      104 2024-04-01 23:12:43.530790 xibabel-0.0.1a3/src/xibabel/__init__.py
--rw-r--r--   0        0        0      571 2024-04-01 20:13:24.938488 xibabel-0.0.1a3/src/xibabel/bench/bench_nib_xib_load.py
--rw-r--r--   0        0        0    18610 2024-04-01 22:51:03.504803 xibabel-0.0.1a3/src/xibabel/loaders.py
--rw-r--r--   0        0        0       20 2024-04-01 20:13:24.938858 xibabel-0.0.1a3/src/xibabel/testing/.gitignore
--rw-r--r--   0        0        0      921 2024-04-01 20:13:24.939016 xibabel-0.0.1a3/src/xibabel/testing/__init__.py
--rw-r--r--   0        0        0      627 2024-04-01 20:13:24.939155 xibabel-0.0.1a3/src/xibabel/testing/__main__.py
--rw-r--r--   0        0        0     5075 2024-04-01 20:13:24.939378 xibabel-0.0.1a3/src/xibabel/testing/fetcher.py
--rw-r--r--   0        0        0      463 2024-04-01 20:13:24.939585 xibabel-0.0.1a3/src/xibabel/testing/test_files.yml
--rw-r--r--   0        0        0      396 2024-04-01 20:13:24.939726 xibabel-0.0.1a3/src/xibabel/testing/test_sets.yml
--rw-r--r--   0        0        0        0 2024-04-01 20:13:24.939864 xibabel-0.0.1a3/src/xibabel/tests/__init__.py
--rw-r--r--   0        0        0     2512 2024-04-01 20:13:24.940151 xibabel-0.0.1a3/src/xibabel/tests/conftest.py
--rw-r--r--   0        0        0     1306 2024-04-01 20:13:24.940358 xibabel-0.0.1a3/src/xibabel/tests/run_server.py
--rw-r--r--   0        0        0    14228 2024-04-01 22:51:03.505743 xibabel-0.0.1a3/src/xibabel/tests/test_loaders.py
--rw-r--r--   0        0        0     1205 2024-04-01 20:13:24.940719 xibabel-0.0.1a3/src/xibabel/tests/test_merge.py
--rw-r--r--   0        0        0     2792 2024-04-01 20:13:24.940931 xibabel-0.0.1a3/src/xibabel/tests/test_scripting.py
--rw-r--r--   0        0        0      794 2024-04-01 20:13:24.941154 xibabel-0.0.1a3/src/xibabel/xutils.py
--rw-r--r--   0        0        0     4578 1970-01-01 00:00:00.000000 xibabel-0.0.1a3/PKG-INFO
+-rw-r--r--   0        0        0     3241 2024-04-06 17:55:02.342516 xibabel-0.0.1b1/README.md
+-rw-r--r--   0        0        0     1172 2024-04-06 22:04:37.266298 xibabel-0.0.1b1/pyproject.toml
+-rw-r--r--   0        0        0      114 2024-04-06 22:03:34.775306 xibabel-0.0.1b1/src/xibabel/__init__.py
+-rw-r--r--   0        0        0      571 2024-04-06 17:55:02.346667 xibabel-0.0.1b1/src/xibabel/bench/bench_nib_xib_load.py
+-rw-r--r--   0        0        0    26374 2024-04-06 17:55:02.346881 xibabel-0.0.1b1/src/xibabel/loaders.py
+-rw-r--r--   0        0        0       20 2024-04-06 17:55:02.347197 xibabel-0.0.1b1/src/xibabel/testing/.gitignore
+-rw-r--r--   0        0        0     2584 2024-04-06 17:55:02.347343 xibabel-0.0.1b1/src/xibabel/testing/__init__.py
+-rw-r--r--   0        0        0      627 2024-04-06 17:55:02.347577 xibabel-0.0.1b1/src/xibabel/testing/__main__.py
+-rw-r--r--   0        0        0     5225 2024-04-06 17:55:02.347801 xibabel-0.0.1b1/src/xibabel/testing/fetcher.py
+-rw-r--r--   0        0        0      463 2024-04-06 17:55:02.348095 xibabel-0.0.1b1/src/xibabel/testing/test_files.yml
+-rw-r--r--   0        0        0      396 2024-04-06 17:55:02.348320 xibabel-0.0.1b1/src/xibabel/testing/test_sets.yml
+-rw-r--r--   0        0        0        0 2024-04-06 17:55:02.348361 xibabel-0.0.1b1/src/xibabel/tests/__init__.py
+-rw-r--r--   0        0        0     2512 2024-04-06 17:55:02.348672 xibabel-0.0.1b1/src/xibabel/tests/conftest.py
+-rw-r--r--   0        0        0      332 2024-04-06 17:55:02.348819 xibabel-0.0.1b1/src/xibabel/tests/markers.py
+-rw-r--r--   0        0        0     1306 2024-04-06 17:55:02.349085 xibabel-0.0.1b1/src/xibabel/tests/run_server.py
+-rw-r--r--   0        0        0    20938 2024-04-06 17:55:02.349301 xibabel-0.0.1b1/src/xibabel/tests/test_loaders.py
+-rw-r--r--   0        0        0     1205 2024-04-06 17:55:02.349677 xibabel-0.0.1b1/src/xibabel/tests/test_merge.py
+-rw-r--r--   0        0        0     2855 2024-04-06 17:55:02.349851 xibabel-0.0.1b1/src/xibabel/tests/test_scripting.py
+-rw-r--r--   0        0        0     2264 2024-04-06 17:55:02.350007 xibabel-0.0.1b1/src/xibabel/tests/test_testing.py
+-rw-r--r--   0        0        0      794 2024-04-06 17:55:02.350222 xibabel-0.0.1b1/src/xibabel/xutils.py
+-rw-r--r--   0        0        0     4808 1970-01-01 00:00:00.000000 xibabel-0.0.1b1/PKG-INFO
```

### Comparing `xibabel-0.0.1a3/README.md` & `xibabel-0.0.1b1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -45,17 +45,17 @@
   time.
 - The labels allow concise and readable operations on named axes. See the
   `glm_in_xibabel` notebook in the `experiments` directory.
 - Xarrays have attributes that can be attached to the image or the axes of the
   image. We can load these attributes from
   [BIDS](https://bids.neuroimaging.io/) format JSON files. This allows better
   transmission of metadata.
-- The Xarrays have a Dask backend, to computations can be deferred and run at
+- The Xarrays have a Dask backend, so computations can be deferred and run at
   the point at which you need the data in memory.
-- Xarrays and Dask allow new storage formats, including storage in
+- Xarrays and Dask allow new storage formats, including storage as
   [Zarr](https://zarr.readthedocs.io) and
   HDF5 / [netCDF](https://en.wikipedia.org/wiki/NetCDF).
 - You can optimize the on-disk format for memory and CPU by adjusting
   _chunking_. We are working on performance metrics for different processing
   steps.
 - Xibabel uses [fsspec](https://filesystem-spec.readthedocs.io) for reading
   NIfTI and other files, allowing you to use many filesystems as the source for
@@ -80,7 +80,13 @@
 ```bash
 pip install git+https://github.com/matthew-brett/xibabel@main
 ```
 
 ## License
 
 We release Xibabel under a BSD simplified 2-clause license (see `LICENSE`).
+
+## Acknowledgments
+
+This work was entirely supported by Chan Zuckerberg Initiative Essential Open
+Source Software for Science grant "Strengthening community and code foundations
+for brain imaging", with thanks.
```

### Comparing `xibabel-0.0.1a3/pyproject.toml` & `xibabel-0.0.1b1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -10,20 +10,19 @@
     {name = "Christopher J. Markiewicz", email = "markiewicz@stanford.edu"}
 ]
 readme = "README.md"
 requires-python = ">=3.8"
 dynamic = ["version", "description"]
 home-page = "https://github.com/matthew-brett/xibabel"
 classifiers = ['License :: OSI Approved :: BSD License',
-               'Development Status :: 2 - Pre-Alpha']
+               'Development Status :: 3 - Alpha']
 dependencies = [
     'xarray',
     'dask',
     'nibabel',
-    'nipy',
     'psutil'
 ]
 
 [project.scripts]
 xib-get-test-set = "xibabel.testing.__main__:main"
 
 [project.optional-dependencies]
@@ -47,12 +46,13 @@
     'pyyaml',
     'pytest-doctestplus',
     'pytest-xprocess',
     'requests',
     'aiohttp',
 ]
 optional = [
+    'nipy',
     'h5netcdf',
     'matplotlib',
     'requests',
     'aiohttp'
 ]
```

### Comparing `xibabel-0.0.1a3/src/xibabel/bench/bench_nib_xib_load.py` & `xibabel-0.0.1b1/src/xibabel/bench/bench_nib_xib_load.py`

 * *Files identical despite different names*

### Comparing `xibabel-0.0.1a3/src/xibabel/loaders.py` & `xibabel-0.0.1b1/src/xibabel/loaders.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 """ Load various data formats into xibabel images
 """
 
+from functools import partial
 from pathlib import Path
 import json
 import logging
 import importlib
 import os.path as op
 
 import numpy as np
 import psutil
 
 import nibabel as nib
 from nibabel.spatialimages import HeaderDataError
 from nibabel.filename_parser import parse_filename
 from nibabel.fileholders import FileHolder
+from nibabel.affines import from_matvec, apply_affine
 
 import fsspec
 import xarray as xr
 import dask.array as da
 
 
 logger = logging.getLogger(__name__)
@@ -80,37 +82,39 @@
             if n_chunks:
                 sizes[axis_no] = int(n_chunks)
                 return sizes
             sizes[axis_no] = 1
         return sizes
 
 
-dim_recoder = {
+dimno2name= {
     None: None,
     0: 'i',
     1: 'j',
     2: 'k'}
 
+dimname2no = {v: k for k, v in dimno2name.items()}
+
 
 time_unit_scaler = {
     'sec': 1,
     'msec': 1 / 1000,
     'usec': 1 / 1_000_000}
 
 
-class NiftiWrapper:
+class NiHeader2Meta:
 
     def __init__(self, header):
         self.header = nib.Nifti1Header.from_header(header)
 
     def get_dim_labels(self):
         freq_dim, phase_dim, slice_dim = self.header.get_dim_info()
-        return {'xib-FrequencyEncodingDirection': dim_recoder[freq_dim],
-                'PhaseEncodingDirection': dim_recoder[phase_dim],
-                'SliceEncodingDirection': dim_recoder[slice_dim]}
+        return {'xib-FrequencyEncodingDirection': dimno2name[freq_dim],
+                'PhaseEncodingDirection': dimno2name[phase_dim],
+                'SliceEncodingDirection': dimno2name[slice_dim]}
 
     def get_slice_timing(self):
         hdr = self.header
         freq_dim, phase_dim, slice_dim = hdr.get_dim_info()
         if not slice_dim:
             return None
         duration = hdr.get_slice_duration()
@@ -152,17 +156,76 @@
         meta = self.get_dim_labels()
         meta['SliceTiming'] = self.get_slice_timing()
         meta['RepetitionTime'] = self.get_repetition_time()
         meta['xib-affines'] = self.get_affines()
         return {k: v for k, v in meta.items() if v is not None}
 
 
-def wrap_header(header):
+class Meta2NiHeader:
+    """ Class writes BIDS attribute dictionary into NIfTI header.
+    """
+
+    def __init__(self, header=None, meta=None):
+        self.header = nib.Nifti1Header.from_header(header)
+        self.meta = {} if meta is None else meta.copy()
+
+    def set_dim_labels(self):
+        # Assume canonical axis order.
+        d = self.meta
+        self.header.set_dim_info(
+            freq=dimname2no.get(d.get('xib-FrequencyEncodingDirection')),
+            phase=dimname2no.get(d.get('PhaseEncodingDirection')),
+            slice=dimname2no.get(d.get('SliceEncodingDirection')))
+
+    def set_slice_timing(self):
+        slice_times = self.meta.get('SliceTiming')
+        if slice_times is None:
+            return
+        try:
+            return self.header.set_slice_times(slice_times)
+        except HeaderDataError:
+            pass
+
+    def set_repetition_time(self):
+        hdr = self.header
+        zooms = np.array(hdr.get_zooms())
+        # Assume header record of image already has correct shape.
+        if len(zooms) < 4:
+            return
+        TR = self.meta.get('RepetitionTime')
+        TR, units = (0, None) if TR is None else (TR, 'sec')
+        zooms[3] = TR
+        hdr.set_xyzt_units(t=units)
+        hdr.set_zooms(zooms)
+
+    def set_affines(self):
+        """ Set valid affines to header.
+        """
+        hdr = self.header
+        affines = self.meta.get('xib-affines', {})
+        for code in ('aligned', 'scanner'):
+            if code in affines:
+                hdr.set_qform(affines[code], code)
+                break
+        for code in ('mni', 'talairach', 'template'):
+            if code in affines:
+                hdr.set_sform(affines[code], code)
+                break
+
+    def updated_header(self):
+        self.set_dim_labels()
+        self.set_slice_timing()
+        self.set_affines()
+        self.set_repetition_time()
+        return self.header
+
+
+def hdr2meta(header):
     # We could try extracting more information from other file types, but
-    return NiftiWrapper(header)
+    return NiHeader2Meta(header).to_meta()
 
 
 def load_zarr(url_or_path, **kwargs):
     r""" Load image from Zarr/Xibabel-format data at `url_or_path`
 
     Parameters
     ----------
@@ -218,20 +281,31 @@
     try:
         arr = np.array(v)
     except ValueError:
         return False
     return arr.ndim < 2
 
 
+class NPEncoder(json.JSONEncoder):
+
+    def default(self, obj):
+        if hasattr(obj, 'tolist'):
+            return obj.tolist()
+        return super().default(self, obj)
+
+
+_jdumps = partial(json.dumps, cls=NPEncoder)
+
+
 def _attrs2json_attrs(attrs):
     out = {}
     for key, value in attrs.items():
         if (isinstance(value, dict) or
             (isinstance(value, (list, tuple)) and not _1d_arrayable(value))):
-            value = [_JSON_MARKER, json.dumps(value)]
+            value = [_JSON_MARKER, _jdumps(value)]
         out[key] = value
     return out
 
 
 def _check_netcdf():
     if importlib.util.find_spec('h5netcdf') is None:
         raise XibFileError('Please install h5netcdf module to load netCDF')
@@ -420,15 +494,15 @@
         elif require_json:
             raise XibFileError(
                 f'BIDS loading {url_or_path} but no corresponding '
                 f'{url_json} file, and `require_json` is True')
     img, meta = _nibabel2img_meta(img_file)
     if sidecar_file:
         with sidecar_file as fobj:
-            meta.update(json.load(fobj))
+            meta.update(_json_attrs2attrs(json.load(fobj)))
     return _img_meta2ximg(img, meta, url_or_path)
 
 
 def load_nibabel(url_or_path, **kwargs):
     r""" Load image from Nibabel-format data at `url_or_path`
 
     `url_or_path` may point directly to ``.json`` file, or to Nibabel format
@@ -470,41 +544,53 @@
 
 class FSFileHolder(FileHolder):
 
     def __del__(self):
         self.fileobj.close()
 
 
+_NI_SPACE_DIMS = ('i', 'j', 'k')
+_NI_TIME_DIM = 'time'
+
+
 def _nibabel2img_meta(img_file):
     # Identify relevant files from img_file
     # Make file_map with opened files.
     if 'local' in img_file.fs.protocol:
         img = nib.load(img_file.path)
     else:  # Not local - use stream interface.
         img_klass = _path2class(img_file.full_name)
         # We are passing out opened fsspec files.
         fh = FileHolder(img_file.full_name, img_file.open())
         img = img_klass.from_file_map({'image': fh})
-    return img, wrap_header(img.header).to_meta()
+    return img, hdr2meta(img.header)
 
 
 def _img_meta2ximg(img, meta, url_or_path):
+    dataobj = FDataObj(img.dataobj)
     coords = {}
-    if (TR := meta.get("RepetitionTime")):
+    dims = _NI_SPACE_DIMS
+    for ax_no, ax_name in enumerate(dims):
+        coords[ax_name] = xr.DataArray(
+            np.arange(img.shape[ax_no]),
+            dims=[ax_name])
+    if dataobj.ndim > 3 and (TR := meta.get("RepetitionTime")):
+        dims += (_NI_TIME_DIM,)
         time_coords = np.arange(0, (img.shape[-1]) * TR, TR)
-        coords = {
-            "time":
-            xr.DataArray(time_coords, dims=["time"], attrs={"units": "s"})}
-    dataobj = FDataObj(img.dataobj)
-    return xr.DataArray(da.from_array(dataobj, chunks=dataobj.chunk_sizes()),
-                        dims=["i", "j", "k", "time"][:dataobj.ndim],
-                        coords=coords,
-                        name=_url2name(url_or_path),
-                        # NB: zarr can't serialize numpy arrays as attrs
-                        attrs=meta)
+        coords[_NI_TIME_DIM] = xr.DataArray(
+            time_coords,
+            dims=[_NI_TIME_DIM],
+            attrs={"units": "s"})
+    return xr.DataArray(
+        da.from_array(dataobj, chunks=dataobj.chunk_sizes()),
+        dims=dims,
+        coords=coords,
+        name=_url2name(url_or_path),
+        # NB: zarr can't serialize numpy arrays as attrs
+        attrs=meta)
 
 
 def _url2name(url_or_path):
     name = drop_suffix(url_or_path, _comp_exts())
     return Path(name).stem
 
 
@@ -525,36 +611,34 @@
     -------
     ret : object
         Return depends on `format`.  See `save_zarr` and `save_netcdf` for
         examples.
     """
     if format is None:
         format = PROCESSORS.guess_format(url_or_path)
-    if format is None:
-        raise XibFormatError(f"Could not guess format from {url_or_path}")
     return PROCESSORS.get_saver(format)(obj, url_or_path, **kwargs)
 
 
-def save_zarr(obj, file_path, **kwargs):
+def save_zarr(obj, url_or_path, **kwargs):
     r""" Save Xibabel image at `url_or_path` in Zarr / Xibabel format.
 
     Parameters
     ----------
     url_or_path : str or Path
     \*\*kwargs : dict
         Arguments to pass to `to_zarr` method of `obj`.
 
     Returns
     -------
     zbe : ZarrBackendStore
     """
-    return obj.to_zarr(file_path, mode='w', **kwargs)
+    return obj.to_zarr(url_or_path, mode='w', **kwargs)
 
 
-def save_netcdf(obj, file_path, **kwargs):
+def save_netcdf(obj, url_or_path, **kwargs):
     r""" Save Xibabel image at `url_or_path` in netCDF / Xibabel format.
 
     Parameters
     ----------
     url_or_path : str or Path
     \*\*kwargs : dict
         Arguments to pass to `to_netcdf` method of `obj`.
@@ -562,32 +646,72 @@
     Returns
     -------
     None
     """
     _check_netcdf()
     out = obj.copy()  # Shallow copy by default.
     out.attrs = _attrs2json_attrs(out.attrs)
-    return out.to_netcdf(file_path, engine='h5netcdf', **kwargs)
+    return out.to_netcdf(url_or_path, engine='h5netcdf', **kwargs)
+
+
+def save_bids(obj, url_or_path, **kwargs):
+    r""" Save Xibabel image at `url_or_path` as NIfTI / BIDS JSON
+
+    Parameters
+    ----------
+    url_or_path : str or Path
+    \*\*kwargs : dict
+        Any remaining named arguments passed to `fsspec.open`.
+
+    Returns
+    -------
+    None
+    """
+    nib_img, attrs = to_nifti(obj)
+    attrs = _attrs2json_attrs(attrs)
+    if str(url_or_path).endswith('.json'):
+        json_uop = url_or_path
+        img_uop = replace_suffix(url_or_path, '.json', '.nii.gz')
+    else:
+        img_uop = url_or_path
+        json_uop = replace_suffix(
+            drop_suffix(url_or_path, _comp_exts()),
+            (),
+            '.json')
+    sidecar_file, img_file = fsspec.open_files((json_uop, img_uop),
+                                               mode='wt',
+                                               compression='infer',
+                                               **kwargs)
+    with sidecar_file as f:
+        f.write(_jdumps(attrs))
+    if 'local' in img_file.fs.protocol:
+        nib.save(nib_img, img_file.path)
+        return
+    # Not local - use stream interface.
+    img_klass = _path2class(img_uop.full_name)
+    # We are passing out opened fsspec files.
+    with img_uop as fh:
+        img_klass.to_file_map({'image': fh})
 
 
 class Processors:
 
     format_processors = {
         'zarr': dict(exts=('ximg',),
                      loader=load_zarr,
                      saver=save_zarr),
         'netcdf': dict(exts=('nc',),
                      loader=load_netcdf,
                      saver=save_netcdf),
         'bids': dict(exts=('json',),
                      loader=load_bids,
-                     saver=None),
+                     saver=save_bids),
         'nibabel': dict(exts=(),  # Defer to Nibabel for extensions
                      loader=load_nibabel,
-                     saver=None),
+                     saver=save_bids),
     }
 
     def __init__(self):
         self.loaders = set()
         self.savers = set()
         self.ext2fmt = {}
         for fmt, info in self.format_processors.items():
@@ -616,7 +740,122 @@
 
     def guess_format(self, file_path):
         suff = str(file_path).split('.')[-1]
         return self.ext2fmt.get(suff)
 
 
 PROCESSORS = Processors()
+
+
+def _ni_sort_expand_dims(img_dims):
+    # Allow for 3D images
+    target_dims = _NI_SPACE_DIMS
+    if not set(img_dims).issubset(_NI_SPACE_DIMS):
+        target_dims += (_NI_TIME_DIM,)
+    x_dims = []
+    x_axes = []
+    out_order = []
+    for expected_pos, expected_dim in enumerate(target_dims):
+        try:
+            curr_pos = img_dims.index(expected_dim)
+        except ValueError:
+            x_dims.append(expected_dim)
+            x_axes.append(expected_pos)
+            continue
+        out_order.append(img_dims[curr_pos])
+    return (out_order + [d for d in img_dims if d not in out_order],
+            x_dims,
+            x_axes)
+
+
+def to_nifti(ximg):
+    # Reorient, expand missing dimensions
+    order, dims, axes = _ni_sort_expand_dims(ximg.dims)
+    ximg = ximg.transpose(*order).expand_dims(dims, axes)
+    # Adjust affines to current state of ximg.
+    back = ximg.xi.with_updated_affines()
+    # Build preliminary header.
+    hdr = nib.Nifti1Header()
+    hdr.set_data_shape(back.shape)
+    # Build header from attributes.
+    hdr = Meta2NiHeader(hdr, back.attrs).updated_header()
+    return nib.Nifti1Image(back, None, hdr), back.attrs
+
+
+@xr.register_dataarray_accessor("xi")
+class XiAccessor:
+
+    def __init__(self, xarray_obj):
+        self._obj = xarray_obj
+
+    def get_affines(self):
+        """ Get spatial affines from attributes of image
+
+        Returns
+        -------
+        affines : dict
+            Dictionary with key, value pairs where key is string giving space
+            to which affine maps, and values are 4x4 spatial affine arrays.
+
+        Notes
+        -----
+        Returned `affines` are copies; if you modify the arrays in `affines`,
+        this will not affect the original image.
+        """
+        aff_d = self._obj.attrs.get('xib-affines', {})
+        return {space: np.array(aff) for space, aff in aff_d.items()}
+
+    def with_updated_affines(self):
+        """ Return image with affines, coordinates updated to match state.
+
+        Return image `adj_img` where the affines and coordinates correctly
+        reflect any detected slicing of the original image.
+
+        Returns
+        -------
+        adj_img : Xibabel image
+            Image with adjusted affines, and for which spatial coordinate
+            indices have been reset to sequential 0-based default.
+
+        Notes
+        -----
+        The affines and i, j, k coordinates reflect the state of the image as
+        of the last call to this function, or as of image load.
+
+        The affines are always 4x4, and always refer to i, j, k space,
+        regardless of dimension ordering, and of the presence of i, j, k
+        dimensions.
+        """
+        adj_img = self._obj.copy()
+        assert adj_img.attrs is not self._obj.attrs
+        out_affines = {}
+        for space, affine in self.get_affines().items():
+            out_affines[space] = self._adjusted_affine(affine, adj_img.coords)
+        adj_img.attrs['xib-affines'] = out_affines
+        return adj_img.xi._with_reset_coordinates()
+
+    def _adjusted_affine(self, affine, coords):
+        vox_origin = np.zeros(3)
+        vox_scalings = np.ones(3)
+        for i, name in enumerate(_NI_SPACE_DIMS):
+            vox_indices = np.ravel(coords.get(name, 0))
+            vox_origin[i] = vox_indices[0]
+            if len(vox_indices) > 1:
+                vd = np.diff(vox_indices)
+                if any(vd[1:] != vd[0]):
+                    raise XibFormatError(
+                        'Cannot handle irregular voxel spacing for {name}')
+                vox_scalings[i] = vd[0]
+        return from_matvec(affine[:3, :3] * vox_scalings,
+                           apply_affine(affine, vox_origin))
+
+    def _with_reset_coordinates(self):
+        ximg = self._obj
+        coords = {}
+        for name in _NI_SPACE_DIMS:
+            if name not in ximg.dims:
+                coords[name] = xr.DataArray(0)
+                continue
+            coords[name] = xr.DataArray(
+                np.arange(ximg[name].shape[0]),
+                dims=[name])
+        return ximg.assign_coords(coords)
```

### Comparing `xibabel-0.0.1a3/src/xibabel/testing/__main__.py` & `xibabel-0.0.1b1/src/xibabel/testing/__main__.py`

 * *Files identical despite different names*

### Comparing `xibabel-0.0.1a3/src/xibabel/testing/fetcher.py` & `xibabel-0.0.1b1/src/xibabel/testing/fetcher.py`

 * *Files 3% similar despite different names*

```diff
@@ -70,14 +70,16 @@
         """ True if `path` is local file
 
         We need this function to deal with Datalad, which used ``git annex`` to
         store links to larger files.  This function needs to check whether the file
         we have is the actual file, or a link (sort-of-thing) to the file, that
         still needs a ``datalad get`` to fetch the actual contents.
         """
+        # Also consider output of `git annex whereis` on `path`.  This shows
+        # one entry for [here] if the file is present.  Test on Windows.
         if not path.is_file():  # Can be True for git annex links on Windows.
             return False
         if path.is_symlink():  # Appears to be True on Unices.
             return True
         # By exploration on Windows - detecting git annex placeholder for file.
         with open(path, 'rb') as fobj:
             start = fobj.read(15)
```

### Comparing `xibabel-0.0.1a3/src/xibabel/tests/conftest.py` & `xibabel-0.0.1b1/src/xibabel/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `xibabel-0.0.1a3/src/xibabel/tests/run_server.py` & `xibabel-0.0.1b1/src/xibabel/tests/run_server.py`

 * *Files identical despite different names*

### Comparing `xibabel-0.0.1a3/src/xibabel/tests/test_loaders.py` & `xibabel-0.0.1b1/src/xibabel/tests/test_loaders.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 """ Test loaders
 """
 
 from pathlib import Path
+from copy import deepcopy
 import os
-from importlib.util import find_spec
 import gzip
-from itertools import product
+from itertools import product, permutations
 import json
 import shutil
 
 import numpy as np
 
 import nibabel as nib
 
 from xibabel import loaders
 from xibabel.loaders import (FDataObj, load_bids, load_nibabel, load, save,
                              PROCESSORS, _json_attrs2attrs, drop_suffix,
-                             replace_suffix, _attrs2json_attrs, wrap_header,
-                             _path2class, XibFileError)
+                             replace_suffix, _attrs2json_attrs, hdr2meta,
+                             _path2class, XibFileError, to_nifti,
+                             _ni_sort_expand_dims, _NI_SPACE_DIMS,
+                             _NI_TIME_DIM)
 from xibabel.xutils import merge
 from xibabel.testing import (JC_EG_FUNC, JC_EG_FUNC_JSON, JC_EG_ANAT,
                              JC_EG_ANAT_JSON, JH_EG_FUNC, skip_without_file,
-                             fetcher)
+                             fetcher, arr_dict_allclose)
+from xibabel.tests.markers import h5netcdf_test
 
 import pytest
 
 rng = np.random.default_rng()
 
 
 class FakeProxy:
@@ -88,15 +91,15 @@
 
 
 def out_back(img, out_path):
     if out_path.is_file():
         os.unlink(out_path)
     nib.save(img, out_path)
     img = nib.load(out_path)
-    return img, wrap_header(img.header).to_meta()
+    return img, hdr2meta(img.header)
 
 
 def test_nibabel_tr(tmp_path):
     # Default image.
     arr = np.zeros((2, 3, 4))
     img = nib.Nifti1Image(arr, np.eye(4), None)
     out_path = tmp_path / 'test.nii'
@@ -221,70 +224,93 @@
     ddj = {'foo': 1,
            'bar': ['__json__', '{"baz": [2, 3]}'],
            'baf': ['__json__', arr_j]}
     assert _attrs2json_attrs(dd) == ddj
     assert _json_attrs2attrs(ddj) == dd
 
 
+def _check_dims_coords(ximg):
+    ndims = len(ximg.dims)
+    space_dims = ximg.dims[:3]
+    assert space_dims == _NI_SPACE_DIMS
+    assert space_dims == tuple(ximg.coords)[:3]
+    for dim_no, dim in enumerate(space_dims):
+        coord = ximg.coords[dim]
+        assert np.all(np.array(coord) == np.arange(ximg.shape[dim_no]))
+    if ndims > 3:
+        assert ximg.dims[3] == _NI_TIME_DIM
+
+
 @skip_without_file(JC_EG_FUNC)
 def test_nib_loader_jc():
     img = nib.load(JC_EG_FUNC)
     ximg = load_nibabel(JC_EG_FUNC)
     assert ximg.attrs == JC_EG_FUNC_META
+    _check_dims_coords(ximg)
     assert np.all(np.array(ximg) == img.get_fdata())
 
 
 @skip_without_file(JH_EG_FUNC)
 def test_nib_loader_jh():
     img = nib.load(JH_EG_FUNC)
     ximg = load_nibabel(JH_EG_FUNC)
     assert ximg.attrs == {'RepetitionTime': 2.5,
                           'xib-affines':
                           {'scanner': img.affine.tolist()}
                          }
+    _check_dims_coords(ximg)
 
 
 if fetcher.have_file(JC_EG_FUNC):
     img = nib.load(JC_EG_FUNC)
     JC_EG_FUNC_META = json.loads(JC_EG_FUNC_JSON.read_text())
     JC_EG_FUNC_META_RAW = {
         'xib-FrequencyEncodingDirection': 'i',
          'PhaseEncodingDirection': 'j',
          'SliceEncodingDirection': 'k',
          'RepetitionTime': 2.0,
          'xib-affines':
          {'scanner': img.affine.tolist()}
     }
     JC_EG_FUNC_META.update(JC_EG_FUNC_META_RAW)
+else:  # For parametrized tests.
+    JC_EG_FUNC_META = {}
+    JC_EG_FUNC_META_RAW = {}
 
 
 if fetcher.have_file(JC_EG_ANAT):
     img = nib.load(JC_EG_ANAT)
     JC_EG_ANAT_META = json.loads(JC_EG_ANAT_JSON.read_text())
     JC_EG_ANAT_META_RAW = {
         'xib-FrequencyEncodingDirection': 'j',
          'PhaseEncodingDirection': 'i',
          'SliceEncodingDirection': 'k',
          'xib-affines':
          {'scanner': img.affine.tolist()}
     }
     JC_EG_ANAT_META.update(JC_EG_ANAT_META_RAW)
+else:  # For parametrized tests.
+    JC_EG_ANAT_META = {}
+    JC_EG_ANAT_META_RAW = {}
+
 
 
 @skip_without_file(JC_EG_ANAT)
 def test_anat_loader():
     img = nib.load(JC_EG_ANAT)
     for loader, in_path in product(
         (load, load_bids, load_nibabel),
         (JC_EG_ANAT, str(JC_EG_ANAT),
          JC_EG_ANAT_JSON, str(JC_EG_ANAT_JSON))):
         ximg = loader(in_path)
         assert ximg.shape == (176, 256, 256)
+        assert ximg.dims == _NI_SPACE_DIMS
         assert ximg.name == JC_EG_ANAT.name.split('.')[0]
         assert ximg.attrs == JC_EG_ANAT_META
+        _check_dims_coords(ximg)
         assert np.all(np.array(ximg) == img.get_fdata())
 
 
 @skip_without_file(JC_EG_ANAT)
 def test_anat_loader_http(fserver):
     nb_img = nib.load(JC_EG_ANAT)
     # Read nibabel from HTTP
@@ -300,14 +326,15 @@
         ximg = load(out_url)
         # Check we can read the data
         ximg.compute()
         # Check parameters
         assert ximg.shape == (176, 256, 256)
         assert ximg.name == JC_EG_ANAT.name.split('.')[0]
         assert ximg.attrs == JC_EG_ANAT_META
+        _check_dims_coords(ximg)
         assert np.all(np.array(ximg) == nb_img.get_fdata())
 
 
 @skip_without_file(JC_EG_ANAT)
 def test_anat_loader_http_params(fserver, tmp_path):
     # Test params get passed through in kwargs.
     nb_img = nib.load(JC_EG_ANAT)
@@ -321,64 +348,122 @@
     assert len(list(out_cache.glob('*'))) == 2  # JSON and Nifti
 
 
 @skip_without_file(JC_EG_ANAT)
 def test_round_trip(tmp_path):
     ximg = load(JC_EG_ANAT)
     assert ximg.shape == (176, 256, 256)
+    _check_dims_coords(ximg)
     out_path = tmp_path / 'out.ximg'
     save(ximg, out_path)
     back = load(out_path)
     assert back.shape == (176, 256, 256)
     assert back.attrs == JC_EG_ANAT_META
+    _check_dims_coords(back)
     # And again
     save(ximg, out_path)
     back = load(out_path)
     assert back.attrs == JC_EG_ANAT_META
+    _check_dims_coords(back)
     # With url
     back = load(f'file:///{out_path}')
     assert back.attrs == JC_EG_ANAT_META
+    _check_dims_coords(back)
 
 
-@pytest.mark.skipif(not find_spec('h5netcdf'),
-                    reason='Need h5netcdf module for test')
+@h5netcdf_test
 @skip_without_file(JC_EG_ANAT)
 def test_round_trip_netcdf(tmp_path):
     ximg = load(JC_EG_ANAT)
     out_path = tmp_path / 'out.nc'
     save(ximg, out_path)
     back = load(out_path)
     assert back.shape == (176, 256, 256)
     assert back.attrs == JC_EG_ANAT_META
     back = load(f'file:///{out_path}')
     assert back.attrs == JC_EG_ANAT_META
+    _check_dims_coords(back)
+
+
+@skip_without_file(JC_EG_ANAT)
+@skip_without_file(JC_EG_FUNC)
+@pytest.mark.parametrize("img_path", [JC_EG_ANAT, JC_EG_FUNC])
+def test_affines(img_path):
+    ximg = load(img_path)
+    nib_img = nib.load(img_path)
+    affines = ximg.xi.get_affines()
+    assert list(affines) == ['scanner']
+    assert np.all(affines['scanner'] == nib_img.affine)
+    back = ximg.xi.with_updated_affines()
+    assert np.all(back.xi.get_affines()['scanner'] == nib_img.affine)
+    xT = ximg.T
+    sp_dims = _NI_SPACE_DIMS
+    assert xT.dims == ximg.dims[::-1]
+    transposed = xT.xi.with_updated_affines()
+    assert np.all(transposed.xi.get_affines()['scanner'] == nib_img.affine)
+    for i, (name, slice_no) in enumerate(zip(sp_dims, (42, 32, 10))):
+        ximg_plane = ximg.sel(**{name: slice_no})
+        assert ximg_plane.dims == tuple(d for d in ximg.dims if d != name)
+        assert tuple(ximg_plane.coords) == ximg.dims
+        adj_img = ximg_plane.xi.with_updated_affines()
+        new_origin = np.array([0, 0, 0, 1])
+        new_origin[i] = slice_no
+        new_affine = nib_img.affine.copy()
+        new_affine[:, 3] = nib_img.affine @ new_origin
+        assert np.all(adj_img.xi.get_affines()['scanner'] == new_affine)
+        # Check Nibabel slicer gives the same result.
+        slicers = [slice(None) for d in range(len(ximg.dims))]
+        slicers[i] = slice(slice_no, slice_no + 1)
+        assert np.all(nib_img.slicer[tuple(slicers)].affine == new_affine)
+    for i, (name, spacing) in enumerate(zip(sp_dims, (2, 3, 4))):
+        slicers = [slice(None) for d in range(len(ximg.dims))]
+        slicers[i] = slice(None, None, spacing)
+        ximg_sliced = ximg[tuple(slicers)]
+        assert ximg_sliced.dims == ximg.dims
+        assert tuple(ximg_sliced.coords) == ximg.dims
+        adj_img = ximg_sliced.xi.with_updated_affines()
+        new_affine = nib_img.affine.copy()
+        scalers = np.ones(3)
+        scalers[i] = spacing
+        new_affine[:3, :3] = nib_img.affine[:3, :3] @ np.diag(scalers)
+        assert np.all(adj_img.xi.get_affines()['scanner'] == new_affine)
+        # Check Nibabel slicer gives the same result.
+        assert np.all(nib_img.slicer[tuple(slicers)].affine == new_affine)
+    # Some more complex slicings, benchmark against nibabel
+    for slicers in permutations([slice(10, 20, 2),
+                                 slice(30, 15, -1),
+                                 slice(5, 16, 3)]):
+        sliced_ximg = ximg[tuple(slicers)].xi.with_updated_affines()
+        sliced_nib_img = nib_img.slicer[tuple(slicers)]
+        assert np.all(sliced_ximg.xi.get_affines()['scanner'] ==
+                    sliced_nib_img.affine)
 
 
 def test_tornado(fserver):
     # Test static file server for URL reads
     fserver.write_text_to('text_file', 'some text')
     fserver.write_bytes_to('binary_file', b'binary')
     response = fserver.get('text_file')
     assert response.status_code == 200
     assert response.text == 'some text'
     assert fserver.read_text('text_file') == 'some text'
     assert fserver.read_bytes('text_file') == b'some text'
     assert fserver.read_bytes('binary_file') == b'binary'
 
 
-@pytest.mark.skipif(not find_spec('h5netcdf'),
-                    reason='Need h5netcdf module for test')
+@h5netcdf_test
 @skip_without_file(JC_EG_ANAT)
 def test_round_trip_netcdf_url(fserver):
     ximg = load(JC_EG_ANAT)
     save(ximg, fserver.server_path / 'out.nc')
     out_url = fserver.make_url('out.nc')
     back = load(out_url)
     assert back.shape == (176, 256, 256)
     assert back.attrs == JC_EG_ANAT_META
+    _check_dims_coords(back)
 
 
 @skip_without_file(JC_EG_ANAT)
 def test_matching_img_error(tmp_path):
     out_json = tmp_path / JC_EG_ANAT_JSON.name
     with pytest.raises(XibFileError, match='does not appear to exist'):
         load(out_json)
@@ -386,18 +471,100 @@
     with pytest.raises(XibFileError, match='No valid file matching'):
         load(out_json)
     out_img = tmp_path / JC_EG_ANAT.name
     shutil.copy2(JC_EG_ANAT, tmp_path)
     back = load(out_img)
     assert back.shape == (176, 256, 256)
     assert back.attrs == JC_EG_ANAT_META
+    _check_dims_coords(back)
     os.unlink(out_img)
     with pytest.raises(XibFileError, match='does not appear to exist'):
         load(out_img)
     shutil.copy2(JC_EG_ANAT, tmp_path)
     os.unlink(out_json)
     back = load(out_img)
+    _check_dims_coords(back)
     assert back.attrs == JC_EG_ANAT_META_RAW
     back = load_bids(out_img, require_json=False)
     assert back.attrs == JC_EG_ANAT_META_RAW
+    _check_dims_coords(back)
     with pytest.raises(XibFileError, match='`require_json` is True'):
         load_bids(out_img, require_json=True)
+
+
+def test_ni_sort_expand_dims():
+    assert _ni_sort_expand_dims([]) == ([],
+                                        ['i', 'j', 'k'],
+                                        [0, 1, 2])
+    assert _ni_sort_expand_dims(['time']) == (['time'],
+                                              ['i', 'j', 'k'],
+                                              [0, 1, 2])
+    assert (_ni_sort_expand_dims(['j']) ==
+            (['j'],
+             ['i', 'k'],
+             [0, 2]))
+    assert (_ni_sort_expand_dims(['time', 'j']) ==
+            (['j', 'time'],
+             ['i', 'k'],
+             [0, 2]))
+    assert (_ni_sort_expand_dims(['j', 'i']) ==
+            (['i', 'j'],
+             ['k'],
+             [2]))
+    assert (_ni_sort_expand_dims(['time', 'j', 'k']) ==
+            (['j', 'k', 'time'],
+             ['i'],
+             [0]))
+
+
+@skip_without_file(JC_EG_ANAT)
+@skip_without_file(JC_EG_FUNC)
+@pytest.mark.parametrize("img_path, meta_raw",
+                         ((JC_EG_ANAT, JC_EG_ANAT_META_RAW),
+                          (JC_EG_FUNC, JC_EG_FUNC_META_RAW)))
+def test_to_nifti(img_path, meta_raw):
+    orig_img = nib.load(img_path)
+    orig_data = orig_img.get_fdata()
+    ximg = load(img_path)
+    # Check data is the same for basic load.
+    assert np.all(ximg == orig_data)
+    # Basic conversion.
+    img, attrs = to_nifti(ximg)
+    assert np.all(img.get_fdata() == orig_data)
+    assert arr_dict_allclose(hdr2meta(img.header), meta_raw)
+    img, attrs = to_nifti(ximg.T)
+    assert np.all(img.get_fdata() == orig_data)
+    assert arr_dict_allclose(hdr2meta(img.header), meta_raw)
+    img, attrs = to_nifti(ximg.T.sel(k=32))  # Drop k axis
+    assert np.all(img.get_fdata() == orig_data[:, :, 32:33])
+    # This changes the origin of the affine.
+    new_affine = orig_img.slicer[:, :, 32:33].affine
+    exp_meta_32 = deepcopy(meta_raw)
+    exp_meta_32['xib-affines']['scanner'] = new_affine
+    assert arr_dict_allclose(hdr2meta(img.header), exp_meta_32)
+
+
+@skip_without_file(JC_EG_ANAT)
+@skip_without_file(JC_EG_FUNC)
+@pytest.mark.parametrize("img_path, meta",
+                         ((JC_EG_ANAT, JC_EG_ANAT_META),
+                          (JC_EG_FUNC, JC_EG_FUNC_META)))
+def test_to_bids(img_path, meta, tmp_path):
+    nib_img = nib.load(img_path)
+    fdata = nib_img.get_fdata()
+    ximg = load(img_path)
+    out_fname = tmp_path / 'out.json'
+    save(ximg, out_fname)
+    back_nib = nib.load(tmp_path / 'out.nii.gz')
+    assert np.allclose(back_nib.get_fdata(), fdata)
+    with open(out_fname, 'rt') as fobj:
+        back_attrs = _json_attrs2attrs(json.load(fobj))
+    assert arr_dict_allclose(back_attrs, meta)
+    assert arr_dict_allclose(load(out_fname).attrs, ximg.attrs)
+    out_fname = tmp_path / 'out2.nii'
+    save(ximg, out_fname)
+    back_nib = nib.load(out_fname)
+    assert np.allclose(back_nib.get_fdata(), fdata)
+    with open(tmp_path / 'out2.json', 'rt') as fobj:
+        back_attrs = _json_attrs2attrs(json.load(fobj))
+    assert arr_dict_allclose(back_attrs, meta)
+    assert arr_dict_allclose(load(out_fname).attrs, ximg.attrs)
```

### Comparing `xibabel-0.0.1a3/src/xibabel/tests/test_merge.py` & `xibabel-0.0.1b1/src/xibabel/tests/test_merge.py`

 * *Files identical despite different names*

### Comparing `xibabel-0.0.1a3/src/xibabel/tests/test_scripting.py` & `xibabel-0.0.1b1/src/xibabel/tests/test_scripting.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,34 +7,36 @@
 
 import xarray as xr
 
 import nibabel as nib
 import xibabel as xib
 
 from xibabel import testing
-
-# For constructing the design.
-from nipy.modalities.fmri.design import block_design, natural_spline
+from xibabel.tests.markers import nipy_test
 
 import pytest
 
 img_path_root = (testing.DATA_PATH /
                 'ds000105' /
                 'sub-1' /
                 'func' /
                 'sub-1_task-objectviewing_run-01_')
 
 bold_path = img_path_root.with_name(img_path_root.name + 'bold.nii.gz')
 tsv_path = img_path_root.with_name(img_path_root.name + 'events.tsv')
 
 
+@nipy_test
 @pytest.mark.skipif(not bold_path.is_file(), reason=f'Missing "{bold_path}"')
 @pytest.mark.skipif(not tsv_path.is_file(), reason=f'Missing "{tsv_path}"')
 def test_glm():
 
+    # For constructing the design.
+    from nipy.modalities.fmri.design import block_design, natural_spline
+
     # Load the events ready to make a design.
     event_df = pd.read_csv(tsv_path, sep='\t')
     df = event_df.rename(columns={'onset': 'start', 'duration': 'end'})
     df['end'] = df['start'] + df['end']
     block_spec = df.to_records(index=None)
 
     nib_img = nib.load(bold_path)
```

### Comparing `xibabel-0.0.1a3/src/xibabel/xutils.py` & `xibabel-0.0.1b1/src/xibabel/xutils.py`

 * *Files identical despite different names*

### Comparing `xibabel-0.0.1a3/PKG-INFO` & `xibabel-0.0.1b1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 Metadata-Version: 2.1
 Name: xibabel
-Version: 0.0.1a3
+Version: 0.0.1b1
 Summary: Init for Xibabel package
 Author-email: Matthew Brett <matthew.brett@gmail.com>, Paul Ivanov <pi@berkeley.edu>, "Christopher J. Markiewicz" <markiewicz@stanford.edu>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: BSD License
-Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Development Status :: 3 - Alpha
 Requires-Dist: xarray
 Requires-Dist: dask
 Requires-Dist: nibabel
-Requires-Dist: nipy
 Requires-Dist: psutil
 Requires-Dist: pre-commit ; extra == "developer"
 Requires-Dist: nbclassic ; extra == "developer"
 Requires-Dist: jupytext ; extra == "developer"
 Requires-Dist: dicom_parser ; extra == "developer"
 Requires-Dist: ipywidgets ; extra == "developer"
 Requires-Dist: zarr ; extra == "developer"
 Requires-Dist: sphinx>=7.0 ; extra == "docs"
 Requires-Dist: numpydoc>=1.6.0 ; extra == "docs"
 Requires-Dist: matplotlib ; extra == "docs"
 Requires-Dist: ipython ; extra == "docs"
 Requires-Dist: jupytext ; extra == "docs"
 Requires-Dist: aiohttp ; extra == "docs"
+Requires-Dist: nipy ; extra == "optional"
 Requires-Dist: h5netcdf ; extra == "optional"
 Requires-Dist: matplotlib ; extra == "optional"
 Requires-Dist: requests ; extra == "optional"
 Requires-Dist: aiohttp ; extra == "optional"
 Requires-Dist: pyyaml ; extra == "test"
 Requires-Dist: pytest-doctestplus ; extra == "test"
 Requires-Dist: pytest-xprocess ; extra == "test"
@@ -85,17 +85,17 @@
   time.
 - The labels allow concise and readable operations on named axes. See the
   `glm_in_xibabel` notebook in the `experiments` directory.
 - Xarrays have attributes that can be attached to the image or the axes of the
   image. We can load these attributes from
   [BIDS](https://bids.neuroimaging.io/) format JSON files. This allows better
   transmission of metadata.
-- The Xarrays have a Dask backend, to computations can be deferred and run at
+- The Xarrays have a Dask backend, so computations can be deferred and run at
   the point at which you need the data in memory.
-- Xarrays and Dask allow new storage formats, including storage in
+- Xarrays and Dask allow new storage formats, including storage as
   [Zarr](https://zarr.readthedocs.io) and
   HDF5 / [netCDF](https://en.wikipedia.org/wiki/NetCDF).
 - You can optimize the on-disk format for memory and CPU by adjusting
   _chunking_. We are working on performance metrics for different processing
   steps.
 - Xibabel uses [fsspec](https://filesystem-spec.readthedocs.io) for reading
   NIfTI and other files, allowing you to use many filesystems as the source for
@@ -121,7 +121,13 @@
 pip install git+https://github.com/matthew-brett/xibabel@main
 ```
 
 ## License
 
 We release Xibabel under a BSD simplified 2-clause license (see `LICENSE`).
 
+## Acknowledgments
+
+This work was entirely supported by Chan Zuckerberg Initiative Essential Open
+Source Software for Science grant "Strengthening community and code foundations
+for brain imaging", with thanks.
+
```

