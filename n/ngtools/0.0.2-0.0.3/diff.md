# Comparing `tmp/ngtools-0.0.2.tar.gz` & `tmp/ngtools-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ngtools-0.0.2.tar", last modified: Fri Apr  5 19:51:47 2024, max compression
+gzip compressed data, was "ngtools-0.0.3.tar", last modified: Sat Apr  6 10:20:46 2024, max compression
```

## Comparing `ngtools-0.0.2.tar` & `ngtools-0.0.3.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:51:47.537914 ngtools-0.0.2/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1072 2024-04-05 19:51:38.000000 ngtools-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6665 2024-04-05 19:51:47.537914 ngtools-0.0.2/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (127)     4820 2024-04-05 19:51:38.000000 ngtools-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:51:47.537914 ngtools-0.0.2/ngtools/
--rwxr-xr-x   0 runner    (1001) docker     (127)       73 2024-04-05 19:51:38.000000 ngtools-0.0.2/ngtools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-05 19:51:47.541914 ngtools-0.0.2/ngtools/_version.py
--rwxr-xr-x   0 runner    (1001) docker     (127)   140462 2024-04-05 19:51:38.000000 ngtools-0.0.2/ngtools/cmdata.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    14653 2024-04-05 19:51:38.000000 ngtools-0.0.2/ngtools/dandifs.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      705 2024-04-05 19:51:38.000000 ngtools-0.0.2/ngtools/drawroi.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6429 2024-04-05 19:51:38.000000 ngtools-0.0.2/ngtools/fileserver.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1832 2024-04-05 19:51:38.000000 ngtools-0.0.2/ngtools/nglocal.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3572 2024-04-05 19:51:38.000000 ngtools-0.0.2/ngtools/opener.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    13130 2024-04-05 19:51:38.000000 ngtools-0.0.2/ngtools/parserapp.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8131 2024-04-05 19:51:38.000000 ngtools-0.0.2/ngtools/shaders.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    16603 2024-04-05 19:51:38.000000 ngtools-0.0.2/ngtools/spaces.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    12225 2024-04-05 19:51:38.000000 ngtools-0.0.2/ngtools/tracts.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2434 2024-04-05 19:51:38.000000 ngtools-0.0.2/ngtools/transforms.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1678 2024-04-05 19:51:38.000000 ngtools-0.0.2/ngtools/utils.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    64294 2024-04-05 19:51:38.000000 ngtools-0.0.2/ngtools/viewer.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    17750 2024-04-05 19:51:38.000000 ngtools-0.0.2/ngtools/volume.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:51:47.537914 ngtools-0.0.2/ngtools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6665 2024-04-05 19:51:47.000000 ngtools-0.0.2/ngtools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-05 19:51:47.000000 ngtools-0.0.2/ngtools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 19:51:47.000000 ngtools-0.0.2/ngtools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-05 19:51:47.000000 ngtools-0.0.2/ngtools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-05 19:51:47.000000 ngtools-0.0.2/ngtools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-05 19:51:47.000000 ngtools-0.0.2/ngtools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-05 19:51:38.000000 ngtools-0.0.2/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (127)     1207 2024-04-05 19:51:47.541914 ngtools-0.0.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)      720 2024-04-05 19:51:38.000000 ngtools-0.0.2/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)    86677 2024-04-05 19:51:38.000000 ngtools-0.0.2/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 10:20:46.465992 ngtools-0.0.3/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1072 2024-04-06 10:20:36.000000 ngtools-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6665 2024-04-06 10:20:46.465992 ngtools-0.0.3/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4820 2024-04-06 10:20:36.000000 ngtools-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 10:20:46.461992 ngtools-0.0.3/ngtools/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       73 2024-04-06 10:20:36.000000 ngtools-0.0.3/ngtools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-06 10:20:46.465992 ngtools-0.0.3/ngtools/_version.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)   140462 2024-04-06 10:20:36.000000 ngtools-0.0.3/ngtools/cmdata.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    14653 2024-04-06 10:20:36.000000 ngtools-0.0.3/ngtools/dandifs.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      705 2024-04-06 10:20:36.000000 ngtools-0.0.3/ngtools/drawroi.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6429 2024-04-06 10:20:36.000000 ngtools-0.0.3/ngtools/fileserver.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1832 2024-04-06 10:20:36.000000 ngtools-0.0.3/ngtools/nglocal.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3572 2024-04-06 10:20:36.000000 ngtools-0.0.3/ngtools/opener.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    13130 2024-04-06 10:20:36.000000 ngtools-0.0.3/ngtools/parserapp.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8131 2024-04-06 10:20:36.000000 ngtools-0.0.3/ngtools/shaders.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    18375 2024-04-06 10:20:36.000000 ngtools-0.0.3/ngtools/spaces.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12225 2024-04-06 10:20:36.000000 ngtools-0.0.3/ngtools/tracts.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2434 2024-04-06 10:20:36.000000 ngtools-0.0.3/ngtools/transforms.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1678 2024-04-06 10:20:36.000000 ngtools-0.0.3/ngtools/utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    67310 2024-04-06 10:20:36.000000 ngtools-0.0.3/ngtools/viewer.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    17750 2024-04-06 10:20:36.000000 ngtools-0.0.3/ngtools/volume.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 10:20:46.465992 ngtools-0.0.3/ngtools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6665 2024-04-06 10:20:46.000000 ngtools-0.0.3/ngtools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-06 10:20:46.000000 ngtools-0.0.3/ngtools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 10:20:46.000000 ngtools-0.0.3/ngtools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-06 10:20:46.000000 ngtools-0.0.3/ngtools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-06 10:20:46.000000 ngtools-0.0.3/ngtools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-06 10:20:46.000000 ngtools-0.0.3/ngtools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-06 10:20:36.000000 ngtools-0.0.3/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1207 2024-04-06 10:20:46.465992 ngtools-0.0.3/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)      720 2024-04-06 10:20:36.000000 ngtools-0.0.3/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    86677 2024-04-06 10:20:36.000000 ngtools-0.0.3/versioneer.py
```

### Comparing `ngtools-0.0.2/LICENSE` & `ngtools-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ngtools-0.0.2/PKG-INFO` & `ngtools-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ngtools
-Version: 0.0.2
+Version: 0.0.3
 Summary: Tracts visualization and annotation in neuroglancer
 Home-page: UNKNOWN
 Author: Yael Balbastre
 Author-email: ybalbastre@mgh.harvard.edu
 License: MIT
 Project-URL: Source Code, https://github.com/balbasty/ngtools
 Project-URL: Homepage, https://github.com/balbasty/ngtools
```

### Comparing `ngtools-0.0.2/README.md` & `ngtools-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `ngtools-0.0.2/ngtools/cmdata.py` & `ngtools-0.0.3/ngtools/cmdata.py`

 * *Files identical despite different names*

### Comparing `ngtools-0.0.2/ngtools/dandifs.py` & `ngtools-0.0.3/ngtools/dandifs.py`

 * *Files identical despite different names*

### Comparing `ngtools-0.0.2/ngtools/drawroi.py` & `ngtools-0.0.3/ngtools/drawroi.py`

 * *Files identical despite different names*

### Comparing `ngtools-0.0.2/ngtools/fileserver.py` & `ngtools-0.0.3/ngtools/fileserver.py`

 * *Files identical despite different names*

### Comparing `ngtools-0.0.2/ngtools/nglocal.py` & `ngtools-0.0.3/ngtools/nglocal.py`

 * *Files identical despite different names*

### Comparing `ngtools-0.0.2/ngtools/opener.py` & `ngtools-0.0.3/ngtools/opener.py`

 * *Files identical despite different names*

### Comparing `ngtools-0.0.2/ngtools/parserapp.py` & `ngtools-0.0.3/ngtools/parserapp.py`

 * *Files identical despite different names*

### Comparing `ngtools-0.0.2/ngtools/shaders.py` & `ngtools-0.0.3/ngtools/shaders.py`

 * *Files identical despite different names*

### Comparing `ngtools-0.0.2/ngtools/spaces.py` & `ngtools-0.0.3/ngtools/spaces.py`

 * *Files 6% similar despite different names*

```diff
@@ -167,25 +167,58 @@
     """
     if isinstance(name, Sequence):
         return name
     name = list(name.lower())
     return [letter2full.get(n, n) for n in name]
 
 
-def _get_neuronames():
-    letters = (('r', 'l'), ('a', 'p'), ('i', 's'))
-    all_neurospaces = []
-    for perm in itertools.permutations(range(3)):
-        for flip in itertools.product([0, 1], repeat=3):
-            space = ''.join([letters[p][f] for p, f in zip(perm, flip)])
-            all_neurospaces.append(space)
-    return all_neurospaces
+def get_neuronames(ndim=None):
+    """
+    Return all short neuronames ("ras", "lpi", etc)
+
+    By default, return names for all possible number of dimensions (1, 2, 3).
+    Specify `ndim` to pnly return names for a specific number of dimensions.
+    """
+    if ndim is None:
+        range_letters = list(range(1, 4))
+    else:
+        range_letters = [ndim]
+    all_neuronames = []
+    all_letters = (('r', 'l'), ('a', 'p'), ('i', 's'))
+    for ndim in range_letters:
+        for letters in itertools.combinations(all_letters, ndim):
+            for perm in itertools.permutations(range(ndim)):
+                for flip in itertools.product([0, 1], repeat=ndim):
+                    space = [letters[p][f] for p, f in zip(perm, flip)]
+                    space = ''.join(space)
+                    all_neuronames.append(space)
+    return all_neuronames
+
+
+def get_defaultnames(ndim=None):
+    """
+    Return all short default names ("xyz", "zyx", etc)
+
+    By default, return names for all possible number of dimensions (1, 2, 3).
+    Specify `ndim` to pnly return names for a specific number of dimensions.
+    """
+    if ndim is None:
+        range_letters = list(range(1, 4))
+    else:
+        range_letters = [ndim]
+    defaultnames = []
+    for ndim in range_letters:
+        for letters in itertools.combinations(['x', 'y', 'z'], ndim):
+            for name in itertools.permutations(letters):
+                defaultnames.append(''.join(name))
+    return defaultnames
 
 
-neuronames = _get_neuronames()
+neuronames = get_neuronames()
+defaultnames = get_defaultnames()
 
 
 def _get_src2ras(src):
     """Return a matrix mapping from `src` to RAS space."""
     xyz2ras = {'x': 'r', 'y': 'a', 'z': 's'}
     src = [xyz2ras.get(x, x) for x in src.lower()]
     pos = list('ras')
@@ -202,73 +235,96 @@
     return mat
 
 
 def _get_src2dst(src, dst):
     """Return a matrix mapping from `src` to `dst` space."""
     src_to_ras = _get_src2ras(src)
     dst_to_ras = _get_src2ras(dst)
-    return np.linalg.inv(dst_to_ras) @ src_to_ras
+    return np.linalg.pinv(dst_to_ras) @ src_to_ras
 
 
 # Build coordinate spaces
 neurospaces = {
     name: ng.CoordinateSpace(
         names=[letter2full[letter.lower()] for letter in name],
-        scales=[1]*3,
-        units=['mm']*3,
+        scales=[1]*len(name),
+        units=['mm']*len(name),
     )
     for name in neuronames
 }
 
-
 defaultspaces = {
-    ''.join(name): ng.CoordinateSpace(
-        names=name,
-        scales=[1]*3,
-        units=['mm']*3,
+    name: ng.CoordinateSpace(
+        names=list(name),
+        scales=[1]*len(name),
+        units=['mm']*len(name),
     )
-    for name in itertools.permutations(['x', 'y', 'z'])
+    for name in defaultnames
 }
 default = defaultspaces['xyz']
 neurospaces.update(defaultspaces)
 
 
+def space_is_compatible(src, dst):
+    to_xyz = {
+        'r': 'x',
+        'l': 'x',
+        'a': 'y',
+        'p': 'y',
+        's': 'z',
+        'i': 'z',
+    }
+    src = list(map(lambda x: to_xyz.get(x, x), src))
+    dst = list(map(lambda x: to_xyz.get(x, x), dst))
+    for x in src:
+        if x not in dst:
+            return False
+    for x in dst:
+        if x not in src:
+            return False
+    return True
+
+
 # Build coordinate transforms
 # 1) key = string
 neurotransforms = {
     (src, dst): ng.CoordinateSpaceTransform(
         matrix=_get_src2dst(src, dst)[:3, :4],
         input_dimensions=neurospaces[src],
         output_dimensions=neurospaces[dst],
     )
     for src in neuronames
     for dst in neuronames
+    if len(src) == len(dst) and space_is_compatible(src, dst)
 }
 # 2) key = CoordinateSpace instances
 neurotransforms.update({
     (neurospaces[src], neurospaces[dst]): neurotransforms[src, dst]
     for src in neuronames
     for dst in neuronames
+    if len(src) == len(dst) and space_is_compatible(src, dst)
 })
 # 3) neurospace to/from xyz
-for name in itertools.permutations(['x', 'y', 'z']):
-    name = ''.join(name)
-    for neuroname in _get_neuronames():
+for name in defaultnames:
+    ndim = len(name)
+    for neuroname in get_neuronames(ndim):
+        if not space_is_compatible(name, neuroname):
+            continue
         matrix = _get_src2dst(neuroname, name)
         neurotransforms[(neuroname, name)] \
             = neurotransforms[(neurospaces[neuroname], defaultspaces[name])] \
             = ng.CoordinateSpaceTransform(
-                matrix=matrix[:3, :4],
+                matrix=matrix[:ndim, :ndim+1],
                 input_dimensions=neurospaces[neuroname],
                 output_dimensions=defaultspaces[name],
             )
         neurotransforms[(name, neuroname)] \
             = neurotransforms[(defaultspaces[name], neurospaces[neuroname])] \
             = ng.CoordinateSpaceTransform(
-                matrix=np.linalg.inv(matrix)[:3, :4],
+                matrix=np.linalg.inv(matrix)[:ndim, :ndim+1],
                 input_dimensions=defaultspaces[name],
                 output_dimensions=neurospaces[neuroname],
             )
 
 
 def compose(left, right):
     """
```

### Comparing `ngtools-0.0.2/ngtools/tracts.py` & `ngtools-0.0.3/ngtools/tracts.py`

 * *Files identical despite different names*

### Comparing `ngtools-0.0.2/ngtools/transforms.py` & `ngtools-0.0.3/ngtools/transforms.py`

 * *Files identical despite different names*

### Comparing `ngtools-0.0.2/ngtools/utils.py` & `ngtools-0.0.3/ngtools/utils.py`

 * *Files identical despite different names*

### Comparing `ngtools-0.0.2/ngtools/viewer.py` & `ngtools-0.0.3/ngtools/viewer.py`

 * *Files 2% similar despite different names*

```diff
@@ -634,16 +634,16 @@
 
         if not dimensions:
             return
 
         dimensions = ensure_list(dimensions)
         if len(dimensions) == 1:
             dimensions = list(dimensions[0])
-        if len(dimensions) != 3:
-            raise ValueError('display takes three axis names')
+        if len(dimensions) > 3:
+            raise ValueError('display takes at most three axis names')
         dimensions = [letter2full.get(letter.lower(), letter)
                       for letter in dimensions]
         display_dimensions = dimensions
 
         def compactNames(names):
             names = list(map(lambda x: x[0].lower(), names))
             names = ''.join([d for d in names if d not in 'ct'])
@@ -896,81 +896,165 @@
             newspace = {}
             for key, val in space.items():
                 if key == src:
                     key = dst
                 newspace[key] = val
             return ng.CoordinateSpace(newspace)
 
+        def update_transform(transform, olddim, newdim):
+            if newdim.endswith(("'", "^")):
+                sdim = newdim[:-1]
+            else:
+                sdim = newdim
+            cdim = sdim + '^'
+            transform.outputDimensions = rename_key(
+                transform.outputDimensions, olddim, newdim)
+            odims = list(transform.outputDimensions.to_json().keys())
+            if newdim == cdim:
+                # to channel dimension -> half unit shift
+                shift = 0.5
+            elif olddim == cdim:
+                # from channel dimension -> remove half unit shift
+                shift = -0.5
+            else:
+                shift = 0
+            if shift:
+                print(transform.matrix)
+                if transform.matrix is not None:
+                    transform.matrix[odims.index(newdim), -1] += shift
+                else:
+                    matrix = np.eye(len(odims)+1)[:-1]
+                    matrix[odims.index(newdim), -1] = shift
+                    transform.matrix = matrix
+                print(transform.matrix)
+            return transform
+
+        def create_transform(scale, olddim, newdim):
+            if newdim.endswith(("'", "^")):
+                sdim = newdim[:-1]
+            else:
+                sdim = newdim
+            cdim = sdim + '^'
+            if newdim == cdim:
+                # to channel dimension -> half unit shift
+                shift = 0.5
+            elif olddim == cdim:
+                # from channel dimension -> remove half unit shift
+                shift = -0.5
+            else:
+                shift = 0
+            transform = ng.CoordinateSpaceTransform(
+                matrix=np.asarray([[1, shift]]),
+                inputDimensions=ng.CoordinateSpace(
+                    names=[olddim],
+                    scales=[scale[0]],
+                    units=[scale[1]],
+                ),
+                outputDimensions=ng.CoordinateSpace(
+                    names=[newdim],
+                    scales=[scale[0]],
+                    units=[scale[1]],
+                )
+            )
+            return transform
+
         for layer in state.layers:
             if layers and layer.name not in layers:
                 continue
             layer = layer.layer
             for dimension in dimensions:
                 ldim = dimension + "'"
                 cdim = dimension + "^"
                 sdim = dimension
                 localDimensions = layer.localDimensions.to_json()
+                if layer.localPosition:
+                    localPosition = layer.localPosition.tolist()
+                else:
+                    localPosition = []
                 channelDimensions = layer.channelDimensions.to_json()
                 transform = None
                 for source in layer.source:
                     if getattr(source, 'transform', {}):
                         transform = source.transform
                         break
-                if mode == 'l':
+                else:
+                    source = layer.source[0]
+
+                if mode == 'l':     # LOCAL
                     if ldim in localDimensions:
                         continue
+                    was_channel = False
+                    if cdim in channelDimensions:
+                        was_channel = True
+                        scale = channelDimensions.pop(cdim)
                     else:
-                        if cdim in channelDimensions:
-                            scale = channelDimensions[cdim]
-                            del channelDimensions[cdim]
-                        else:
-                            scale = [1, ""]
-                        localDimensions[ldim] = scale
+                        scale = [1, ""]
+                    localDimensions[ldim] = scale
+                    localPosition = [*(localPosition or []), 0]
                     if transform:
-                        odims = list(transform.outputDimensions.to_json())
-                        if cdim in odims:
-                            transform.matrix[odims.index(cdim), -1] -= 0.5
-                        transform.outputDimensions = rename_key(
-                            transform.outputDimensions, cdim, ldim)
-                        transform.outputDimensions = rename_key(
-                            transform.outputDimensions, sdim, ldim)
-                elif mode == 'c':
+                        update_transform(
+                            transform, cdim if was_channel else sdim, ldim)
+                    else:
+                        source.transform = create_transform(
+                            scale, cdim if was_channel else sdim, ldim)
+
+                elif mode == 'c':   # CHANNEL
                     if cdim in channelDimensions:
                         continue
+                    was_local = False
+                    if ldim in localDimensions:
+                        was_local = True
+                        for i, key in enumerate(localDimensions.keys()):
+                            if key == ldim:
+                                break
+                        scale = localDimensions.pop(ldim)
+                        if i < len(localPosition):
+                            localPosition.pop(i)
                     else:
-                        if ldim in localDimensions:
-                            scale = localDimensions[ldim]
-                            del localDimensions[ldim]
-                        else:
-                            scale = [1, ""]
-                        channelDimensions[cdim] = scale
+                        scale = [1, ""]
+                    channelDimensions[cdim] = scale
                     if transform:
-                        transform.outputDimensions = rename_key(
-                            transform.outputDimensions, ldim, cdim)
-                        transform.outputDimensions = rename_key(
-                            transform.outputDimensions, sdim, cdim)
-                        odims = list(transform.outputDimensions.to_json())
-                        if dimension + "^" in odims:
-                            transform.matrix[odims.index(cdim), -1] += 0.5
-                elif mode == 's':
+                        update_transform(
+                            transform, ldim if was_local else sdim, cdim)
+                    else:
+                        source.transform = create_transform(
+                            scale, ldim if was_local else sdim, cdim)
+
+                elif mode == 's':   # SPATIAL
+                    if cdim not in channelDimensions and \
+                            ldim not in localDimensions:
+                        continue
+                    scale = [1, ""]
+                    was_channel = False
                     if cdim in channelDimensions:
-                        del channelDimensions[cdim]
+                        scale = channelDimensions.pop(cdim)
+                        was_channel = True
                     if ldim in localDimensions:
-                        del localDimensions[ldim]
+                        for i, key in enumerate(localDimensions.keys()):
+                            if key == ldim:
+                                break
+                        scale = localDimensions.pop(ldim)
+                        if i < len(localPosition):
+                            localPosition.pop(i)
                     if transform:
-                        transform.outputDimensions = rename_key(
-                            transform.outputDimensions, cdim, sdim)
-                        transform.outputDimensions = rename_key(
-                            transform.outputDimensions, ldim, sdim)
-                        odims = list(transform.outputDimensions.to_json())
-                        if cdim in odims:
-                            transform.matrix[odims.index(cdim), -1] += 0.5
+                        update_transform(
+                            transform, cdim if was_channel else ldim, sdim)
+                    else:
+                        source.transform = create_transform(
+                            scale, cdim if was_channel else ldim, sdim)
+                    if sdim not in state.dimensions.to_json():
+                        dimensions = state.dimensions.to_json()
+                        dimensions[sdim] = scale
+                        state.dimensions = CoordinateSpace(dimensions)
                 layer.localDimensions = CoordinateSpace(localDimensions)
+                layer.localPosition = np.asarray(localPosition)
                 layer.channelDimensions = CoordinateSpace(channelDimensions)
 
+        print(state)
+
     @action(needstate=True)
     def position(self, coord, dimensions=None, unit=None,
                  world=False, layer=False, *, state=None, **kwargs):
         """
         Change cursor position
 
         Parameters
```

### Comparing `ngtools-0.0.2/ngtools/volume.py` & `ngtools-0.0.3/ngtools/volume.py`

 * *Files identical despite different names*

### Comparing `ngtools-0.0.2/ngtools.egg-info/PKG-INFO` & `ngtools-0.0.3/ngtools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ngtools
-Version: 0.0.2
+Version: 0.0.3
 Summary: Tracts visualization and annotation in neuroglancer
 Home-page: UNKNOWN
 Author: Yael Balbastre
 Author-email: ybalbastre@mgh.harvard.edu
 License: MIT
 Project-URL: Source Code, https://github.com/balbasty/ngtools
 Project-URL: Homepage, https://github.com/balbasty/ngtools
```

### Comparing `ngtools-0.0.2/ngtools.egg-info/SOURCES.txt` & `ngtools-0.0.3/ngtools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ngtools-0.0.2/setup.cfg` & `ngtools-0.0.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `ngtools-0.0.2/setup.py` & `ngtools-0.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `ngtools-0.0.2/versioneer.py` & `ngtools-0.0.3/versioneer.py`

 * *Files identical despite different names*

