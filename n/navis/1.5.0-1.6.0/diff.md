# Comparing `tmp/navis-1.5.0.tar.gz` & `tmp/navis-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "navis-1.5.0.tar", last modified: Fri Jul 28 08:22:55 2023, max compression
+gzip compressed data, was "navis-1.6.0.tar", last modified: Sun Apr  7 15:47:23 2024, max compression
```

## Comparing `navis-1.5.0.tar` & `navis-1.6.0.tar`

### file list

```diff
@@ -1,202 +1,206 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:22:55.789556 navis-1.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35141 2023-07-28 08:22:49.000000 navis-1.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-28 08:22:49.000000 navis-1.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8628 2023-07-28 08:22:55.785556 navis-1.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6962 2023-07-28 08:22:49.000000 navis-1.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:22:55.725555 navis-1.5.0/navis/
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-07-28 08:22:51.000000 navis-1.5.0/navis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-07-28 08:22:51.000000 navis-1.5.0/navis/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4340 2023-07-28 08:22:51.000000 navis-1.5.0/navis/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-07-28 08:22:51.000000 navis-1.5.0/navis/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:22:55.729555 navis-1.5.0/navis/connectivity/
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-07-28 08:22:51.000000 navis-1.5.0/navis/connectivity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4374 2023-07-28 08:22:51.000000 navis-1.5.0/navis/connectivity/cnmetrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     4858 2023-07-28 08:22:51.000000 navis-1.5.0/navis/connectivity/matrix_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6691 2023-07-28 08:22:51.000000 navis-1.5.0/navis/connectivity/predict.py
--rw-r--r--   0 runner    (1001) docker     (123)    19869 2023-07-28 08:22:51.000000 navis-1.5.0/navis/connectivity/similarity.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:22:55.729555 navis-1.5.0/navis/conversion/
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-07-28 08:22:51.000000 navis-1.5.0/navis/conversion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20355 2023-07-28 08:22:51.000000 navis-1.5.0/navis/conversion/converters.py
--rw-r--r--   0 runner    (1001) docker     (123)    18037 2023-07-28 08:22:51.000000 navis-1.5.0/navis/conversion/meshing.py
--rw-r--r--   0 runner    (1001) docker     (123)     7696 2023-07-28 08:22:51.000000 navis-1.5.0/navis/conversion/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:22:55.733555 navis-1.5.0/navis/core/
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-07-28 08:22:51.000000 navis-1.5.0/navis/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26391 2023-07-28 08:22:51.000000 navis-1.5.0/navis/core/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    18002 2023-07-28 08:22:51.000000 navis-1.5.0/navis/core/core_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    22028 2023-07-28 08:22:51.000000 navis-1.5.0/navis/core/dotprop.py
--rw-r--r--   0 runner    (1001) docker     (123)    15350 2023-07-28 08:22:51.000000 navis-1.5.0/navis/core/mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)    38381 2023-07-28 08:22:51.000000 navis-1.5.0/navis/core/neuronlist.py
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-07-28 08:22:51.000000 navis-1.5.0/navis/core/neurons.py
--rw-r--r--   0 runner    (1001) docker     (123)    46188 2023-07-28 08:22:51.000000 navis-1.5.0/navis/core/skeleton.py
--rw-r--r--   0 runner    (1001) docker     (123)    22037 2023-07-28 08:22:51.000000 navis-1.5.0/navis/core/volumes.py
--rw-r--r--   0 runner    (1001) docker     (123)    13041 2023-07-28 08:22:51.000000 navis-1.5.0/navis/core/voxel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:22:55.733555 navis-1.5.0/navis/data/
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-07-28 08:22:51.000000 navis-1.5.0/navis/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:22:55.737555 navis-1.5.0/navis/data/gml/
--rw-r--r--   0 runner    (1001) docker     (123)   500970 2023-07-28 08:22:51.000000 navis-1.5.0/navis/data/gml/1734350788.gml
--rw-r--r--   0 runner    (1001) docker     (123)   545251 2023-07-28 08:22:51.000000 navis-1.5.0/navis/data/gml/1734350908.gml
--rw-r--r--   0 runner    (1001) docker     (123)   485390 2023-07-28 08:22:51.000000 navis-1.5.0/navis/data/gml/722817260.gml
--rw-r--r--   0 runner    (1001) docker     (123)   528774 2023-07-28 08:22:51.000000 navis-1.5.0/navis/data/gml/754534424.gml
--rw-r--r--   0 runner    (1001) docker     (123)   549154 2023-07-28 08:22:51.000000 navis-1.5.0/navis/data/gml/754538881.gml
--rw-r--r--   0 runner    (1001) docker     (123)     6924 2023-07-28 08:22:51.000000 navis-1.5.0/navis/data/load_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-07-28 08:22:51.000000 navis-1.5.0/navis/data/meta.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:22:55.741555 navis-1.5.0/navis/data/obj/
--rw-r--r--   0 runner    (1001) docker     (123)   509952 2023-07-28 08:22:51.000000 navis-1.5.0/navis/data/obj/1734350788.obj
--rw-r--r--   0 runner    (1001) docker     (123)   573635 2023-07-28 08:22:51.000000 navis-1.5.0/navis/data/obj/1734350908.obj
--rw-r--r--   0 runner    (1001) docker     (123)   534422 2023-07-28 08:22:51.000000 navis-1.5.0/navis/data/obj/722817260.obj
--rw-r--r--   0 runner    (1001) docker     (123)   533660 2023-07-28 08:22:51.000000 navis-1.5.0/navis/data/obj/754534424.obj
--rw-r--r--   0 runner    (1001) docker     (123)   531212 2023-07-28 08:22:51.000000 navis-1.5.0/navis/data/obj/754538881.obj
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-28 08:22:51.000000 navis-1.5.0/navis/data/readme.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:22:55.745555 navis-1.5.0/navis/data/swc/
--rw-r--r--   0 runner    (1001) docker     (123)   186313 2023-07-28 08:22:51.000000 navis-1.5.0/navis/data/swc/1734350788.swc
--rw-r--r--   0 runner    (1001) docker     (123)   202615 2023-07-28 08:22:51.000000 navis-1.5.0/navis/data/swc/1734350908.swc
--rw-r--r--   0 runner    (1001) docker     (123)   180566 2023-07-28 08:22:51.000000 navis-1.5.0/navis/data/swc/722817260.swc
--rw-r--r--   0 runner    (1001) docker     (123)   196153 2023-07-28 08:22:51.000000 navis-1.5.0/navis/data/swc/754534424.swc
--rw-r--r--   0 runner    (1001) docker     (123)   203788 2023-07-28 08:22:51.000000 navis-1.5.0/navis/data/swc/754538881.swc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:22:55.745555 navis-1.5.0/navis/data/synapses/
--rw-r--r--   0 runner    (1001) docker     (123)   124574 2023-07-28 08:22:51.000000 navis-1.5.0/navis/data/synapses/1734350788.csv
--rw-r--r--   0 runner    (1001) docker     (123)   140166 2023-07-28 08:22:51.000000 navis-1.5.0/navis/data/synapses/1734350908.csv
--rw-r--r--   0 runner    (1001) docker     (123)   144503 2023-07-28 08:22:51.000000 navis-1.5.0/navis/data/synapses/722817260.csv
--rw-r--r--   0 runner    (1001) docker     (123)   139110 2023-07-28 08:22:51.000000 navis-1.5.0/navis/data/synapses/754534424.csv
--rw-r--r--   0 runner    (1001) docker     (123)   135951 2023-07-28 08:22:51.000000 navis-1.5.0/navis/data/synapses/754538881.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:22:55.749555 navis-1.5.0/navis/data/volumes/
--rw-r--r--   0 runner    (1001) docker     (123)    27418 2023-07-28 08:22:51.000000 navis-1.5.0/navis/data/volumes/lh.obj
--rw-r--r--   0 runner    (1001) docker     (123)   719824 2023-07-28 08:22:51.000000 navis-1.5.0/navis/data/volumes/neuropil.obj
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:22:55.749555 navis-1.5.0/navis/graph/
--rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-07-28 08:22:51.000000 navis-1.5.0/navis/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7108 2023-07-28 08:22:51.000000 navis-1.5.0/navis/graph/clinic.py
--rw-r--r--   0 runner    (1001) docker     (123)    24337 2023-07-28 08:22:51.000000 navis-1.5.0/navis/graph/converters.py
--rw-r--r--   0 runner    (1001) docker     (123)    72995 2023-07-28 08:22:51.000000 navis-1.5.0/navis/graph/graph_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:22:55.753555 navis-1.5.0/navis/interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 08:22:51.000000 navis-1.5.0/navis/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-07-28 08:22:51.000000 navis-1.5.0/navis/interfaces/allen_celltypes.py
--rw-r--r--   0 runner    (1001) docker     (123)    40988 2023-07-28 08:22:51.000000 navis-1.5.0/navis/interfaces/blender.py
--rw-r--r--   0 runner    (1001) docker     (123)     4939 2023-07-28 08:22:51.000000 navis-1.5.0/navis/interfaces/cytoscape.py
--rw-r--r--   0 runner    (1001) docker     (123)    20984 2023-07-28 08:22:51.000000 navis-1.5.0/navis/interfaces/insectbrain_db.py
--rw-r--r--   0 runner    (1001) docker     (123)    13317 2023-07-28 08:22:51.000000 navis-1.5.0/navis/interfaces/microns.py
--rw-r--r--   0 runner    (1001) docker     (123)    20282 2023-07-28 08:22:51.000000 navis-1.5.0/navis/interfaces/neuprint.py
--rw-r--r--   0 runner    (1001) docker     (123)     9254 2023-07-28 08:22:51.000000 navis-1.5.0/navis/interfaces/neuromorpho.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:22:55.753555 navis-1.5.0/navis/interfaces/neuron/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-28 08:22:51.000000 navis-1.5.0/navis/interfaces/neuron/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31672 2023-07-28 08:22:51.000000 navis-1.5.0/navis/interfaces/neuron/comp.py
--rw-r--r--   0 runner    (1001) docker     (123)    30302 2023-07-28 08:22:51.000000 navis-1.5.0/navis/interfaces/neuron/network.py
--rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-07-28 08:22:51.000000 navis-1.5.0/navis/interfaces/neuron/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    61225 2023-07-28 08:22:51.000000 navis-1.5.0/navis/interfaces/r.py
--rw-r--r--   0 runner    (1001) docker     (123)    11695 2023-07-28 08:22:51.000000 navis-1.5.0/navis/interfaces/vfb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:22:55.757556 navis-1.5.0/navis/intersection/
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-07-28 08:22:51.000000 navis-1.5.0/navis/intersection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-07-28 08:22:51.000000 navis-1.5.0/navis/intersection/convex.py
--rw-r--r--   0 runner    (1001) docker     (123)    17628 2023-07-28 08:22:51.000000 navis-1.5.0/navis/intersection/intersect.py
--rw-r--r--   0 runner    (1001) docker     (123)     4137 2023-07-28 08:22:51.000000 navis-1.5.0/navis/intersection/ray.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:22:55.761556 navis-1.5.0/navis/io/
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-07-28 08:22:51.000000 navis-1.5.0/navis/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30440 2023-07-28 08:22:51.000000 navis-1.5.0/navis/io/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    41325 2023-07-28 08:22:51.000000 navis-1.5.0/navis/io/hdf_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     4364 2023-07-28 08:22:51.000000 navis-1.5.0/navis/io/json_io.py
--rw-r--r--   0 runner    (1001) docker     (123)    11421 2023-07-28 08:22:51.000000 navis-1.5.0/navis/io/mesh_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     7135 2023-07-28 08:22:51.000000 navis-1.5.0/navis/io/nmx_io.py
--rw-r--r--   0 runner    (1001) docker     (123)    14530 2023-07-28 08:22:51.000000 navis-1.5.0/navis/io/nrrd_io.py
--rw-r--r--   0 runner    (1001) docker     (123)    22308 2023-07-28 08:22:51.000000 navis-1.5.0/navis/io/precomputed_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     7970 2023-07-28 08:22:51.000000 navis-1.5.0/navis/io/rda_io.py
--rw-r--r--   0 runner    (1001) docker     (123)    25489 2023-07-28 08:22:51.000000 navis-1.5.0/navis/io/swc_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     9974 2023-07-28 08:22:51.000000 navis-1.5.0/navis/io/tiff_io.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:22:55.761556 navis-1.5.0/navis/matching/
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-07-28 08:22:51.000000 navis-1.5.0/navis/matching/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10115 2023-07-28 08:22:51.000000 navis-1.5.0/navis/matching/bipartite.py
--rw-r--r--   0 runner    (1001) docker     (123)     7624 2023-07-28 08:22:51.000000 navis-1.5.0/navis/matching/pipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:22:55.765556 navis-1.5.0/navis/meshes/
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-07-28 08:22:51.000000 navis-1.5.0/navis/meshes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5436 2023-07-28 08:22:51.000000 navis-1.5.0/navis/meshes/b3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-07-28 08:22:51.000000 navis-1.5.0/navis/meshes/fqmr.py
--rw-r--r--   0 runner    (1001) docker     (123)    17290 2023-07-28 08:22:51.000000 navis-1.5.0/navis/meshes/mesh_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4072 2023-07-28 08:22:51.000000 navis-1.5.0/navis/meshes/o3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     9294 2023-07-28 08:22:51.000000 navis-1.5.0/navis/meshes/operations.py
--rw-r--r--   0 runner    (1001) docker     (123)     3697 2023-07-28 08:22:51.000000 navis-1.5.0/navis/meshes/pyml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:22:55.765556 navis-1.5.0/navis/meshes/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-07-28 08:22:51.000000 navis-1.5.0/navis/meshes/templates/blender_decimate.py.template
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-28 08:22:51.000000 navis-1.5.0/navis/meshes/templates/blender_smooth.py.template
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:22:55.765556 navis-1.5.0/navis/models/
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-07-28 08:22:51.000000 navis-1.5.0/navis/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23204 2023-07-28 08:22:51.000000 navis-1.5.0/navis/models/network_models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:22:55.765556 navis-1.5.0/navis/morpho/
--rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-07-28 08:22:51.000000 navis-1.5.0/navis/morpho/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-07-28 08:22:51.000000 navis-1.5.0/navis/morpho/analyze.py
--rw-r--r--   0 runner    (1001) docker     (123)     5945 2023-07-28 08:22:51.000000 navis-1.5.0/navis/morpho/fq.py
--rw-r--r--   0 runner    (1001) docker     (123)    81191 2023-07-28 08:22:51.000000 navis-1.5.0/navis/morpho/manipulation.py
--rw-r--r--   0 runner    (1001) docker     (123)    61726 2023-07-28 08:22:51.000000 navis-1.5.0/navis/morpho/mmetrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    14387 2023-07-28 08:22:51.000000 navis-1.5.0/navis/morpho/persistence.py
--rw-r--r--   0 runner    (1001) docker     (123)    11705 2023-07-28 08:22:51.000000 navis-1.5.0/navis/morpho/subset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:22:55.769556 navis-1.5.0/navis/nbl/
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-07-28 08:22:51.000000 navis-1.5.0/navis/nbl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25736 2023-07-28 08:22:51.000000 navis-1.5.0/navis/nbl/ablast_funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6598 2023-07-28 08:22:51.000000 navis-1.5.0/navis/nbl/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    66298 2023-07-28 08:22:51.000000 navis-1.5.0/navis/nbl/nblast_funcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:22:55.769556 navis-1.5.0/navis/nbl/score_mats/
--rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-07-28 08:22:51.000000 navis-1.5.0/navis/nbl/score_mats/smat_alpha_fcwb.csv
--rw-r--r--   0 runner    (1001) docker     (123)     3979 2023-07-28 08:22:51.000000 navis-1.5.0/navis/nbl/score_mats/smat_fcwb.csv
--rw-r--r--   0 runner    (1001) docker     (123)    40790 2023-07-28 08:22:51.000000 navis-1.5.0/navis/nbl/smat.py
--rw-r--r--   0 runner    (1001) docker     (123)    21255 2023-07-28 08:22:51.000000 navis-1.5.0/navis/nbl/synblast_funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)    14594 2023-07-28 08:22:51.000000 navis-1.5.0/navis/nbl/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:22:55.773556 navis-1.5.0/navis/plotting/
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-07-28 08:22:51.000000 navis-1.5.0/navis/plotting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24991 2023-07-28 08:22:51.000000 navis-1.5.0/navis/plotting/colors.py
--rw-r--r--   0 runner    (1001) docker     (123)     7373 2023-07-28 08:22:51.000000 navis-1.5.0/navis/plotting/d.py
--rw-r--r--   0 runner    (1001) docker     (123)    48337 2023-07-28 08:22:51.000000 navis-1.5.0/navis/plotting/dd.py
--rw-r--r--   0 runner    (1001) docker     (123)    20753 2023-07-28 08:22:51.000000 navis-1.5.0/navis/plotting/ddd.py
--rw-r--r--   0 runner    (1001) docker     (123)    16502 2023-07-28 08:22:51.000000 navis-1.5.0/navis/plotting/flat.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:22:55.773556 navis-1.5.0/navis/plotting/k3d/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 08:22:51.000000 navis-1.5.0/navis/plotting/k3d/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-28 08:22:51.000000 navis-1.5.0/navis/plotting/k3d/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    15616 2023-07-28 08:22:51.000000 navis-1.5.0/navis/plotting/k3d/k3d_objects.py
--rw-r--r--   0 runner    (1001) docker     (123)    11012 2023-07-28 08:22:51.000000 navis-1.5.0/navis/plotting/plot_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:22:55.773556 navis-1.5.0/navis/plotting/plotly/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 08:22:51.000000 navis-1.5.0/navis/plotting/plotly/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24548 2023-07-28 08:22:51.000000 navis-1.5.0/navis/plotting/plotly/graph_objs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:22:55.777556 navis-1.5.0/navis/plotting/vispy/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-28 08:22:51.000000 navis-1.5.0/navis/plotting/vispy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    48166 2023-07-28 08:22:51.000000 navis-1.5.0/navis/plotting/vispy/viewer.py
--rw-r--r--   0 runner    (1001) docker     (123)    27104 2023-07-28 08:22:51.000000 navis-1.5.0/navis/plotting/vispy/visuals.py
--rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-07-28 08:22:51.000000 navis-1.5.0/navis/plotting/vispy/vputils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:22:55.777556 navis-1.5.0/navis/sampling/
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-07-28 08:22:51.000000 navis-1.5.0/navis/sampling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8875 2023-07-28 08:22:51.000000 navis-1.5.0/navis/sampling/downsampling.py
--rw-r--r--   0 runner    (1001) docker     (123)    18706 2023-07-28 08:22:51.000000 navis-1.5.0/navis/sampling/resampling.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:22:55.781556 navis-1.5.0/navis/transforms/
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-07-28 08:22:51.000000 navis-1.5.0/navis/transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3268 2023-07-28 08:22:51.000000 navis-1.5.0/navis/transforms/affine.py
--rw-r--r--   0 runner    (1001) docker     (123)    15215 2023-07-28 08:22:51.000000 navis-1.5.0/navis/transforms/align.py
--rw-r--r--   0 runner    (1001) docker     (123)    11571 2023-07-28 08:22:51.000000 navis-1.5.0/navis/transforms/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    15283 2023-07-28 08:22:51.000000 navis-1.5.0/navis/transforms/cmtk.py
--rw-r--r--   0 runner    (1001) docker     (123)    10109 2023-07-28 08:22:51.000000 navis-1.5.0/navis/transforms/elastix.py
--rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-07-28 08:22:51.000000 navis-1.5.0/navis/transforms/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    19064 2023-07-28 08:22:51.000000 navis-1.5.0/navis/transforms/h5reg.py
--rw-r--r--   0 runner    (1001) docker     (123)     7544 2023-07-28 08:22:51.000000 navis-1.5.0/navis/transforms/h5reg_java.py
--rw-r--r--   0 runner    (1001) docker     (123)     3922 2023-07-28 08:22:51.000000 navis-1.5.0/navis/transforms/moving_least_squares.py
--rw-r--r--   0 runner    (1001) docker     (123)    51158 2023-07-28 08:22:51.000000 navis-1.5.0/navis/transforms/templates.py
--rw-r--r--   0 runner    (1001) docker     (123)     4803 2023-07-28 08:22:51.000000 navis-1.5.0/navis/transforms/thinplate.py
--rw-r--r--   0 runner    (1001) docker     (123)    20684 2023-07-28 08:22:51.000000 navis-1.5.0/navis/transforms/xfm_funcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:22:55.785556 navis-1.5.0/navis/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-07-28 08:22:51.000000 navis-1.5.0/navis/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4249 2023-07-28 08:22:51.000000 navis-1.5.0/navis/utils/cv.py
--rw-r--r--   0 runner    (1001) docker     (123)    21944 2023-07-28 08:22:51.000000 navis-1.5.0/navis/utils/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)    10952 2023-07-28 08:22:51.000000 navis-1.5.0/navis/utils/eval.py
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-28 08:22:51.000000 navis-1.5.0/navis/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-07-28 08:22:51.000000 navis-1.5.0/navis/utils/iterables.py
--rw-r--r--   0 runner    (1001) docker     (123)    12683 2023-07-28 08:22:51.000000 navis-1.5.0/navis/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5134 2023-07-28 08:22:51.000000 navis-1.5.0/navis/utils/validate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:22:55.729555 navis-1.5.0/navis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8628 2023-07-28 08:22:55.000000 navis-1.5.0/navis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4448 2023-07-28 08:22:55.000000 navis-1.5.0/navis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 08:22:55.000000 navis-1.5.0/navis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 08:22:55.000000 navis-1.5.0/navis.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-07-28 08:22:55.000000 navis-1.5.0/navis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-28 08:22:55.000000 navis-1.5.0/navis.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-28 08:22:51.000000 navis-1.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 08:22:55.789556 navis-1.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2548 2023-07-28 08:22:51.000000 navis-1.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:22:55.785556 navis-1.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-07-28 08:22:51.000000 navis-1.5.0/tests/test_io.py
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-28 08:22:51.000000 navis-1.5.0/tests/test_neurons.py
--rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-07-28 08:22:51.000000 navis-1.5.0/tests/test_notebooks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-07-28 08:22:51.000000 navis-1.5.0/tests/test_parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-07-28 08:22:51.000000 navis-1.5.0/tests/test_transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:47:23.357362 navis-1.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35141 2024-04-07 15:47:19.000000 navis-1.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-07 15:47:19.000000 navis-1.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    12595 2024-04-07 15:47:23.357362 navis-1.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7464 2024-04-07 15:47:19.000000 navis-1.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:47:23.313361 navis-1.6.0/navis/
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-07 15:47:20.000000 navis-1.6.0/navis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-07 15:47:20.000000 navis-1.6.0/navis/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4340 2024-04-07 15:47:20.000000 navis-1.6.0/navis/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-04-07 15:47:20.000000 navis-1.6.0/navis/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:47:23.313361 navis-1.6.0/navis/connectivity/
+-rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-04-07 15:47:20.000000 navis-1.6.0/navis/connectivity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8233 2024-04-07 15:47:20.000000 navis-1.6.0/navis/connectivity/adjacency.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4374 2024-04-07 15:47:20.000000 navis-1.6.0/navis/connectivity/cnmetrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4858 2024-04-07 15:47:20.000000 navis-1.6.0/navis/connectivity/matrix_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6691 2024-04-07 15:47:20.000000 navis-1.6.0/navis/connectivity/predict.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19869 2024-04-07 15:47:20.000000 navis-1.6.0/navis/connectivity/similarity.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:47:23.317361 navis-1.6.0/navis/conversion/
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-04-07 15:47:20.000000 navis-1.6.0/navis/conversion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20373 2024-04-07 15:47:20.000000 navis-1.6.0/navis/conversion/converters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18037 2024-04-07 15:47:20.000000 navis-1.6.0/navis/conversion/meshing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7696 2024-04-07 15:47:20.000000 navis-1.6.0/navis/conversion/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:47:23.317361 navis-1.6.0/navis/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-04-07 15:47:20.000000 navis-1.6.0/navis/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26616 2024-04-07 15:47:20.000000 navis-1.6.0/navis/core/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18002 2024-04-07 15:47:20.000000 navis-1.6.0/navis/core/core_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22039 2024-04-07 15:47:20.000000 navis-1.6.0/navis/core/dotprop.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15225 2024-04-07 15:47:20.000000 navis-1.6.0/navis/core/mesh.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38381 2024-04-07 15:47:20.000000 navis-1.6.0/navis/core/neuronlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      895 2024-04-07 15:47:20.000000 navis-1.6.0/navis/core/neurons.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47630 2024-04-07 15:47:20.000000 navis-1.6.0/navis/core/skeleton.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22129 2024-04-07 15:47:20.000000 navis-1.6.0/navis/core/volumes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13041 2024-04-07 15:47:20.000000 navis-1.6.0/navis/core/voxel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:47:23.317361 navis-1.6.0/navis/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-07 15:47:20.000000 navis-1.6.0/navis/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:47:23.321361 navis-1.6.0/navis/data/gml/
+-rw-r--r--   0 runner    (1001) docker     (127)   500970 2024-04-07 15:47:20.000000 navis-1.6.0/navis/data/gml/1734350788.gml
+-rw-r--r--   0 runner    (1001) docker     (127)   545251 2024-04-07 15:47:20.000000 navis-1.6.0/navis/data/gml/1734350908.gml
+-rw-r--r--   0 runner    (1001) docker     (127)   485390 2024-04-07 15:47:20.000000 navis-1.6.0/navis/data/gml/722817260.gml
+-rw-r--r--   0 runner    (1001) docker     (127)   528774 2024-04-07 15:47:20.000000 navis-1.6.0/navis/data/gml/754534424.gml
+-rw-r--r--   0 runner    (1001) docker     (127)   549154 2024-04-07 15:47:20.000000 navis-1.6.0/navis/data/gml/754538881.gml
+-rw-r--r--   0 runner    (1001) docker     (127)     6924 2024-04-07 15:47:20.000000 navis-1.6.0/navis/data/load_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-07 15:47:20.000000 navis-1.6.0/navis/data/meta.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:47:23.325361 navis-1.6.0/navis/data/obj/
+-rw-r--r--   0 runner    (1001) docker     (127)   509952 2024-04-07 15:47:20.000000 navis-1.6.0/navis/data/obj/1734350788.obj
+-rw-r--r--   0 runner    (1001) docker     (127)   573635 2024-04-07 15:47:20.000000 navis-1.6.0/navis/data/obj/1734350908.obj
+-rw-r--r--   0 runner    (1001) docker     (127)   534422 2024-04-07 15:47:20.000000 navis-1.6.0/navis/data/obj/722817260.obj
+-rw-r--r--   0 runner    (1001) docker     (127)   533660 2024-04-07 15:47:20.000000 navis-1.6.0/navis/data/obj/754534424.obj
+-rw-r--r--   0 runner    (1001) docker     (127)   531212 2024-04-07 15:47:20.000000 navis-1.6.0/navis/data/obj/754538881.obj
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-04-07 15:47:20.000000 navis-1.6.0/navis/data/readme.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:47:23.329362 navis-1.6.0/navis/data/swc/
+-rw-r--r--   0 runner    (1001) docker     (127)   186313 2024-04-07 15:47:20.000000 navis-1.6.0/navis/data/swc/1734350788.swc
+-rw-r--r--   0 runner    (1001) docker     (127)   202615 2024-04-07 15:47:20.000000 navis-1.6.0/navis/data/swc/1734350908.swc
+-rw-r--r--   0 runner    (1001) docker     (127)   180566 2024-04-07 15:47:20.000000 navis-1.6.0/navis/data/swc/722817260.swc
+-rw-r--r--   0 runner    (1001) docker     (127)   196153 2024-04-07 15:47:20.000000 navis-1.6.0/navis/data/swc/754534424.swc
+-rw-r--r--   0 runner    (1001) docker     (127)   203788 2024-04-07 15:47:20.000000 navis-1.6.0/navis/data/swc/754538881.swc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:47:23.329362 navis-1.6.0/navis/data/synapses/
+-rw-r--r--   0 runner    (1001) docker     (127)   124574 2024-04-07 15:47:20.000000 navis-1.6.0/navis/data/synapses/1734350788.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   140166 2024-04-07 15:47:20.000000 navis-1.6.0/navis/data/synapses/1734350908.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   144503 2024-04-07 15:47:20.000000 navis-1.6.0/navis/data/synapses/722817260.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   139110 2024-04-07 15:47:20.000000 navis-1.6.0/navis/data/synapses/754534424.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   135951 2024-04-07 15:47:20.000000 navis-1.6.0/navis/data/synapses/754538881.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:47:23.329362 navis-1.6.0/navis/data/volumes/
+-rw-r--r--   0 runner    (1001) docker     (127)    27418 2024-04-07 15:47:20.000000 navis-1.6.0/navis/data/volumes/lh.obj
+-rw-r--r--   0 runner    (1001) docker     (127)   719824 2024-04-07 15:47:20.000000 navis-1.6.0/navis/data/volumes/neuropil.obj
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:47:23.333361 navis-1.6.0/navis/graph/
+-rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-04-07 15:47:20.000000 navis-1.6.0/navis/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7108 2024-04-07 15:47:20.000000 navis-1.6.0/navis/graph/clinic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24337 2024-04-07 15:47:20.000000 navis-1.6.0/navis/graph/converters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    75766 2024-04-07 15:47:20.000000 navis-1.6.0/navis/graph/graph_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:47:23.333361 navis-1.6.0/navis/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 15:47:20.000000 navis-1.6.0/navis/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2939 2024-04-07 15:47:20.000000 navis-1.6.0/navis/interfaces/allen_celltypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40988 2024-04-07 15:47:20.000000 navis-1.6.0/navis/interfaces/blender.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4939 2024-04-07 15:47:20.000000 navis-1.6.0/navis/interfaces/cytoscape.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22028 2024-04-07 15:47:20.000000 navis-1.6.0/navis/interfaces/insectbrain_db.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13317 2024-04-07 15:47:20.000000 navis-1.6.0/navis/interfaces/microns.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20845 2024-04-07 15:47:20.000000 navis-1.6.0/navis/interfaces/neuprint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9254 2024-04-07 15:47:20.000000 navis-1.6.0/navis/interfaces/neuromorpho.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:47:23.337362 navis-1.6.0/navis/interfaces/neuron/
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-07 15:47:20.000000 navis-1.6.0/navis/interfaces/neuron/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31908 2024-04-07 15:47:20.000000 navis-1.6.0/navis/interfaces/neuron/comp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30388 2024-04-07 15:47:20.000000 navis-1.6.0/navis/interfaces/neuron/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-04-07 15:47:20.000000 navis-1.6.0/navis/interfaces/neuron/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61225 2024-04-07 15:47:20.000000 navis-1.6.0/navis/interfaces/r.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11695 2024-04-07 15:47:20.000000 navis-1.6.0/navis/interfaces/vfb.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:47:23.337362 navis-1.6.0/navis/intersection/
+-rw-r--r--   0 runner    (1001) docker     (127)      821 2024-04-07 15:47:20.000000 navis-1.6.0/navis/intersection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-04-07 15:47:20.000000 navis-1.6.0/navis/intersection/convex.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17628 2024-04-07 15:47:20.000000 navis-1.6.0/navis/intersection/intersect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4137 2024-04-07 15:47:20.000000 navis-1.6.0/navis/intersection/ray.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:47:23.337362 navis-1.6.0/navis/io/
+-rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-04-07 15:47:20.000000 navis-1.6.0/navis/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35448 2024-04-07 15:47:20.000000 navis-1.6.0/navis/io/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41325 2024-04-07 15:47:20.000000 navis-1.6.0/navis/io/hdf_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4364 2024-04-07 15:47:20.000000 navis-1.6.0/navis/io/json_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11421 2024-04-07 15:47:20.000000 navis-1.6.0/navis/io/mesh_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10736 2024-04-07 15:47:20.000000 navis-1.6.0/navis/io/nmx_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14530 2024-04-07 15:47:20.000000 navis-1.6.0/navis/io/nrrd_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16591 2024-04-07 15:47:20.000000 navis-1.6.0/navis/io/pq_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23780 2024-04-07 15:47:20.000000 navis-1.6.0/navis/io/precomputed_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7970 2024-04-07 15:47:20.000000 navis-1.6.0/navis/io/rda_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25826 2024-04-07 15:47:20.000000 navis-1.6.0/navis/io/swc_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9974 2024-04-07 15:47:20.000000 navis-1.6.0/navis/io/tiff_io.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:47:23.341362 navis-1.6.0/navis/matching/
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-07 15:47:20.000000 navis-1.6.0/navis/matching/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10115 2024-04-07 15:47:20.000000 navis-1.6.0/navis/matching/bipartite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7624 2024-04-07 15:47:20.000000 navis-1.6.0/navis/matching/pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:47:23.341362 navis-1.6.0/navis/meshes/
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-04-07 15:47:20.000000 navis-1.6.0/navis/meshes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5436 2024-04-07 15:47:20.000000 navis-1.6.0/navis/meshes/b3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-04-07 15:47:20.000000 navis-1.6.0/navis/meshes/fqmr.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20554 2024-04-07 15:47:20.000000 navis-1.6.0/navis/meshes/mesh_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4072 2024-04-07 15:47:20.000000 navis-1.6.0/navis/meshes/o3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9294 2024-04-07 15:47:20.000000 navis-1.6.0/navis/meshes/operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3697 2024-04-07 15:47:20.000000 navis-1.6.0/navis/meshes/pyml.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:47:23.341362 navis-1.6.0/navis/meshes/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-04-07 15:47:20.000000 navis-1.6.0/navis/meshes/templates/blender_decimate.py.template
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-04-07 15:47:20.000000 navis-1.6.0/navis/meshes/templates/blender_smooth.py.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:47:23.341362 navis-1.6.0/navis/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-04-07 15:47:20.000000 navis-1.6.0/navis/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24453 2024-04-07 15:47:20.000000 navis-1.6.0/navis/models/network_models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:47:23.341362 navis-1.6.0/navis/morpho/
+-rw-r--r--   0 runner    (1001) docker     (127)     2241 2024-04-07 15:47:20.000000 navis-1.6.0/navis/morpho/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3247 2024-04-07 15:47:20.000000 navis-1.6.0/navis/morpho/analyze.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6069 2024-04-07 15:47:20.000000 navis-1.6.0/navis/morpho/fq.py
+-rw-r--r--   0 runner    (1001) docker     (127)    82129 2024-04-07 15:47:20.000000 navis-1.6.0/navis/morpho/manipulation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61726 2024-04-07 15:47:20.000000 navis-1.6.0/navis/morpho/mmetrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14387 2024-04-07 15:47:20.000000 navis-1.6.0/navis/morpho/persistence.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11730 2024-04-07 15:47:20.000000 navis-1.6.0/navis/morpho/subset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:47:23.345362 navis-1.6.0/navis/nbl/
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-04-07 15:47:20.000000 navis-1.6.0/navis/nbl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25736 2024-04-07 15:47:20.000000 navis-1.6.0/navis/nbl/ablast_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6598 2024-04-07 15:47:20.000000 navis-1.6.0/navis/nbl/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    67721 2024-04-07 15:47:20.000000 navis-1.6.0/navis/nbl/nblast_funcs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:47:23.345362 navis-1.6.0/navis/nbl/score_mats/
+-rw-r--r--   0 runner    (1001) docker     (127)     3083 2024-04-07 15:47:20.000000 navis-1.6.0/navis/nbl/score_mats/smat_alpha_fcwb.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     3979 2024-04-07 15:47:20.000000 navis-1.6.0/navis/nbl/score_mats/smat_fcwb.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    40853 2024-04-07 15:47:20.000000 navis-1.6.0/navis/nbl/smat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21255 2024-04-07 15:47:20.000000 navis-1.6.0/navis/nbl/synblast_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15005 2024-04-07 15:47:20.000000 navis-1.6.0/navis/nbl/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:47:23.345362 navis-1.6.0/navis/plotting/
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-04-07 15:47:20.000000 navis-1.6.0/navis/plotting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24991 2024-04-07 15:47:20.000000 navis-1.6.0/navis/plotting/colors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7373 2024-04-07 15:47:20.000000 navis-1.6.0/navis/plotting/d.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48337 2024-04-07 15:47:20.000000 navis-1.6.0/navis/plotting/dd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20753 2024-04-07 15:47:20.000000 navis-1.6.0/navis/plotting/ddd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16502 2024-04-07 15:47:20.000000 navis-1.6.0/navis/plotting/flat.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:47:23.345362 navis-1.6.0/navis/plotting/k3d/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 15:47:20.000000 navis-1.6.0/navis/plotting/k3d/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-07 15:47:20.000000 navis-1.6.0/navis/plotting/k3d/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15616 2024-04-07 15:47:20.000000 navis-1.6.0/navis/plotting/k3d/k3d_objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11214 2024-04-07 15:47:20.000000 navis-1.6.0/navis/plotting/plot_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:47:23.345362 navis-1.6.0/navis/plotting/plotly/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 15:47:20.000000 navis-1.6.0/navis/plotting/plotly/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24580 2024-04-07 15:47:20.000000 navis-1.6.0/navis/plotting/plotly/graph_objs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:47:23.349362 navis-1.6.0/navis/plotting/vispy/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-07 15:47:20.000000 navis-1.6.0/navis/plotting/vispy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48166 2024-04-07 15:47:20.000000 navis-1.6.0/navis/plotting/vispy/viewer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27104 2024-04-07 15:47:20.000000 navis-1.6.0/navis/plotting/vispy/visuals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2495 2024-04-07 15:47:20.000000 navis-1.6.0/navis/plotting/vispy/vputils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:47:23.349362 navis-1.6.0/navis/sampling/
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-04-07 15:47:20.000000 navis-1.6.0/navis/sampling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8875 2024-04-07 15:47:20.000000 navis-1.6.0/navis/sampling/downsampling.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18780 2024-04-07 15:47:20.000000 navis-1.6.0/navis/sampling/resampling.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:47:23.349362 navis-1.6.0/navis/transforms/
+-rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-04-07 15:47:20.000000 navis-1.6.0/navis/transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3268 2024-04-07 15:47:20.000000 navis-1.6.0/navis/transforms/affine.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15215 2024-04-07 15:47:20.000000 navis-1.6.0/navis/transforms/align.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11571 2024-04-07 15:47:20.000000 navis-1.6.0/navis/transforms/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21914 2024-04-07 15:47:20.000000 navis-1.6.0/navis/transforms/cmtk.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10109 2024-04-07 15:47:20.000000 navis-1.6.0/navis/transforms/elastix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2989 2024-04-07 15:47:20.000000 navis-1.6.0/navis/transforms/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19173 2024-04-07 15:47:20.000000 navis-1.6.0/navis/transforms/h5reg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7544 2024-04-07 15:47:20.000000 navis-1.6.0/navis/transforms/h5reg_java.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7065 2024-04-07 15:47:20.000000 navis-1.6.0/navis/transforms/images.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3922 2024-04-07 15:47:20.000000 navis-1.6.0/navis/transforms/moving_least_squares.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57826 2024-04-07 15:47:20.000000 navis-1.6.0/navis/transforms/templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4803 2024-04-07 15:47:20.000000 navis-1.6.0/navis/transforms/thinplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21013 2024-04-07 15:47:20.000000 navis-1.6.0/navis/transforms/xfm_funcs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:47:23.353362 navis-1.6.0/navis/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-04-07 15:47:20.000000 navis-1.6.0/navis/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4428 2024-04-07 15:47:20.000000 navis-1.6.0/navis/utils/cv.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21944 2024-04-07 15:47:20.000000 navis-1.6.0/navis/utils/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10952 2024-04-07 15:47:20.000000 navis-1.6.0/navis/utils/eval.py
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-07 15:47:20.000000 navis-1.6.0/navis/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3335 2024-04-07 15:47:20.000000 navis-1.6.0/navis/utils/iterables.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12683 2024-04-07 15:47:20.000000 navis-1.6.0/navis/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5134 2024-04-07 15:47:20.000000 navis-1.6.0/navis/utils/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:47:23.353362 navis-1.6.0/navis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12595 2024-04-07 15:47:23.000000 navis-1.6.0/navis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4552 2024-04-07 15:47:23.000000 navis-1.6.0/navis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 15:47:23.000000 navis-1.6.0/navis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 15:47:23.000000 navis-1.6.0/navis.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-04-07 15:47:23.000000 navis-1.6.0/navis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-07 15:47:23.000000 navis-1.6.0/navis.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-07 15:47:20.000000 navis-1.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 15:47:23.357362 navis-1.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2606 2024-04-07 15:47:20.000000 navis-1.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:47:23.353362 navis-1.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3494 2024-04-07 15:47:20.000000 navis-1.6.0/tests/test_connectivity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2968 2024-04-07 15:47:20.000000 navis-1.6.0/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-04-07 15:47:20.000000 navis-1.6.0/tests/test_neurons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-04-07 15:47:20.000000 navis-1.6.0/tests/test_notebooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-04-07 15:47:20.000000 navis-1.6.0/tests/test_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2910 2024-04-07 15:47:20.000000 navis-1.6.0/tests/test_transforms.py
```

### Comparing `navis-1.5.0/LICENSE` & `navis-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `navis-1.5.0/PKG-INFO` & `navis-1.6.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,78 +1,30 @@
-Metadata-Version: 2.1
-Name: navis
-Version: 1.5.0
-Summary: Neuron Analysis and Visualization library
-Home-page: http://navis.readthedocs.io
-Author: Philipp Schlegel
-Author-email: pms70@cam.ac.uk
-License: GNU GPL V3
-Project-URL: Documentation, http://navis.readthedocs.io
-Project-URL: Source, https://github.com/navis-org/navis
-Project-URL: Changelog, https://navis.readthedocs.io/en/latest/source/whats_new.html
-Keywords: Neuron Analysis Visualization Morphometrics Morphology Anatomy Connectivity Transform Neuroscience NBLAST Skeletons SWC neuPrint
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Science/Research
-Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
-Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: pathos
-Provides-Extra: shapely
-Provides-Extra: r
-Provides-Extra: kdtree
-Provides-Extra: hash
-Provides-Extra: flybrains
-Provides-Extra: cloudvolume
-Provides-Extra: vispy-default
-Provides-Extra: meshes
-Provides-Extra: test-notebook
-Provides-Extra: dev
-Provides-Extra: all
-Provides-Extra: all-dev
-Provides-Extra: vispy-pyglet
-Provides-Extra: vispy-pyqt5
-Provides-Extra: vispy-pyqt6
-Provides-Extra: vispy-pyside
-Provides-Extra: vispy-pyside2
-Provides-Extra: vispy-pyside6
-Provides-Extra: vispy-glfw
-Provides-Extra: vispy-sdl2
-Provides-Extra: vispy-wx
-Provides-Extra: vispy-tk
-License-File: LICENSE
+[![Documentation Status](https://readthedocs.org/projects/navis/badge/?version=latest)](http://navis.readthedocs.io/en/latest/?badge=latest) [![Tests](https://github.com/navis-org/navis/actions/workflows/test-package.yml/badge.svg)](https://github.com/navis-org/navis/actions/workflows/test-package.yml) [![Run notebooks](https://github.com/navis-org/navis/actions/workflows/notebooktest-package.yml/badge.svg)](https://github.com/navis-org/navis/actions/workflows/notebooktest-package.yml) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/navis-org/navis/blob/master/examples/colab.ipynb) [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.8191725.svg)](https://zenodo.org/doi/10.5281/zenodo.4699382) [![Downloads](https://pepy.tech/badge/navis)](https://pepy.tech/project/navis)
 
-[![Documentation Status](https://readthedocs.org/projects/navis/badge/?version=latest)](http://navis.readthedocs.io/en/latest/?badge=latest) [![Tests](https://github.com/navis-org/navis/actions/workflows/test-package.yml/badge.svg)](https://github.com/navis-org/navis/actions/workflows/test-package.yml) [![Run notebooks](https://github.com/navis-org/navis/actions/workflows/notebooktest-package.yml/badge.svg)](https://github.com/navis-org/navis/actions/workflows/notebooktest-package.yml) [![Coverage Status](https://coveralls.io/repos/github/navis-org/navis/badge.svg?branch=master)](https://coveralls.io/github/navis-org/navis?branch=master) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/navis-org/navis/blob/master/examples/colab.ipynb) [![DOI](https://zenodo.org/badge/168142416.svg)](https://zenodo.org/badge/latestdoi/168142416) [![Downloads](https://pepy.tech/badge/navis)](https://pepy.tech/project/navis)
+<img src="https://github.com/navis-org/navis/raw/master/docs/_static/logo_new.png" height="150">
 
-<img src="https://github.com/navis-org/navis/raw/master/docs/_static/favicon.png" height="60">
-
-NAVis is a Python 3 (3.8 or later) library for **N**euron **A**nalysis and **Vis**ualization.
+NAVis is a Python 3 library for **N**euron **A**nalysis and **Vis**ualization.
 
 ## Documentation
 NAVis is on [ReadTheDocs](http://navis.readthedocs.io/ "NAVis ReadTheDocs").
 
 ## Features
-* works as Jupyter notebook, script or from terminal
-* support for various neuron types: **skeletons**, **meshes**, **dotprops**, **voxels**
-* 2D (matplotlib) and 3D (vispy, plotly or k3d) **plotting**
-* neuron **surgery**: cutting, stitching, pruning, rerooting, intersections, ...
-* **morphometrics**: Strahler analysis, cable length, volume, tortuosity, ...
-* compare & cluster by morphology (e.g. **NBLAST**, persistence, form factor) and connectivity
-* **transform** data between template brains (support for e.g. HDF5, CMTK, Elastix and thin plate spline transforms)
-* load neurons directly from [neuPrint](https://neuprint.janelia.org), [neuromorpho.org](http://neuromorpho.org) and others
-* simulate neurons and networks using the **NEURON** simulator
-* interface with **Blender 3D** for high quality [renderings](https://youtu.be/wl3sFG7WQJc)
-* interface with **R** neuron libraries (e.g. [nat](https://github.com/jefferis/nat), [rcatmaid](https://github.com/jefferis/rcatmaid), [elmr](https://github.com/jefferis/elmr))
-* import-export from/to **SWC**, neuroglancer's ["**precomputed**"](https://github.com/google/neuroglancer/tree/master/src/neuroglancer/datasource/precomputed) format and more
-* scalable thanks to out-of-the-box support for multiprocessing
-* designed to be **extensible** - see for example [pymaid](https://pymaid.readthedocs.io/en/latest/)
+* **polyglot**: work and convert between neuron skeletons, meshes, dotprops and images
+* **visualize**: 2D (matplotlib) and 3D (vispy, plotly or k3d)
+* **process**: skeletonization, meshing, smoothing, repair, downsampling, etc.
+* **morphometrics**: Strahler analysis, cable length, volume, tortuosity and more
+* **similarity**: compare & cluster by morphology (e.g. NBLAST, persistence or form factor) or connectivity metrics
+* **transform**: move data between template brains (built-in support for HDF5, CMTK, Elastix and landmark-based transforms)
+* **interface**: load neurons directly from [neuPrint](https://neuprint.janelia.org), [neuromorpho.org](http://neuromorpho.org) and other data sources
+* **model** neurons and networks using the *NEURON* simulator
+* **render**: use Blender 3D for high quality [visualizations](https://youtu.be/wl3sFG7WQJc)
+* **R** neuron libraries: interfaces with [nat](https://github.com/jefferis/nat), [rcatmaid](https://github.com/jefferis/rcatmaid), [elmr](https://github.com/jefferis/elmr) and more
+* **import-export**: read/write SWCs, neuroglancer's ["*precomputed*"](https://github.com/google/neuroglancer/tree/master/src/neuroglancer/datasource/precomputed) format, NMX/NML, NRRD, mesh-files and more
+* **scalable**: out-of-the-box support for multiprocessing
+* **extensible**: build your own package on top of navis - see [pymaid](https://pymaid.readthedocs.io/en/latest/) for example
 
 ## Getting started
 See the [documentation](http://navis.readthedocs.io/ "NAVis ReadTheDocs") for detailed installation instructions, tutorials and examples. For the impatient:
 
 ```sh
 pip3 install 'navis[all]'
 ```
@@ -91,60 +43,73 @@
 
 3D plotting from a python REPL is provided by `vispy`, which has a choice of backends.
 Different backends work best on different combinations of hardware, OS, python distribution, and REPL, so there may be some trial and error involved.
 `vispy`'s backends are [listed here](https://vispy.org/installation.html#backend-requirements), and each can be installed as a navis extra, e.g. `pip3 install 'navis[vispy-pyqt6]'`.
 
 ![movie](https://user-images.githubusercontent.com/7161148/114312307-28a72700-9aea-11eb-89a6-ee1d72bfa730.mov)
 
+## Questions?
+Questions on how to use `navis` are best placed in [discussions](https://github.com/navis-org/navis/discussions). Same goes for cool projects or analyses you made using `navis` -
+we'd love to hear from you!
+
 ## Changelog
 
 A summary of changes can be found
 [here](https://navis.readthedocs.io/en/latest/source/whats_new.html).
 
 ## NAVis & friends
 <p align="center">
 <img src="https://github.com/navis-org/navis/blob/master/docs/_static/navis_ecosystem.png?raw=true" width="700">
 </p>
 
 NAVis comes with batteries included but is also highly extensible. Some
 libraries built on top of NAVis:
 * [flybrains](https://github.com/navis-org/navis-flybrains) provides templates and transforms for *Drosophila* brains to use with navis
 * [pymaid](https://pymaid.readthedocs.io/en/latest/) pulls and pushes data from/to CATMAID servers
-* [fafbseg](https://fafbseg-py.readthedocs.io/en/latest/index.html) contains tools to work with auto-segmented data for the FAFB EM dataset
+* [fafbseg](https://fafbseg-py.readthedocs.io/en/latest/index.html) contains tools to work with auto-segmented data for the FAFB EM dataset including FlyWire
+
+## Who uses NAVis?
+NAVis has been used in a range of neurobiological publications. See [here](publications.md) for a list.
+
+We have implemented various published algorithms and methods:
+
+1. NBLAST: Comparison of neurons based on morphology [(Costa et al., 2016)](https://www.cell.com/neuron/fulltext/S0896-6273(16)30265-3?_returnURL=https%3A%2F%2Flinkinghub.elsevier.com%2Fretrieve%2Fpii%2FS0896627316302653%3Fshowall%3Dtrue)
+2. Vertex Similarity: Comparison of neurons based on connectivity [(Jarrell et al., 2012)](http://science.sciencemag.org/content/337/6093/437.long)
+3. Comparison of neurons based on synapse distribution
+[(Schlegel et al., 2016)](https://elifesciences.org/content/5/e16799)
+4. Synapse flow centrality for axon-dendrite splits [(Schneider-Mizell et al., 2016)](https://elifesciences.org/articles/12059)
+
+Working on your own cool new method? Consider adding it to NAVis!
+
+## Citing NAVis
+We'd love to know if you found NAVis useful for your research! You can help us
+spread the word by citing the DOI provided by Zenodo [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.8191725.svg)](https://zenodo.org/doi/10.5281/zenodo.4699382)
 
 ## License
-This code is under GNU GPL V3
+This code is under [GNU GPL V3](LICENSE).
 
 ## Acknowledgments
 NAVis is inspired by and inherits much of its design from the excellent
 [natverse](http://natverse.org) R packages by
 [Greg Jefferis](https://github.com/jefferis), [Alex Bates](https://github.com/alexanderbates),
 [James Manton](https://github.com/ajdm) and others.
 
-## References
-NAVis implements or provides interfaces with algorithms described in:
+## Contributing
+Want to contribute? Great, here is how!
 
-1. **Comparison of neurons based on morphology**: Neuron. 2016 doi: 10.1016/j.neuron.2016.06.012
-*NBLAST: Rapid, Sensitive Comparison of Neuronal Structure and Construction of Neuron Family Databases.*
-Costa M, Manton JD, Ostrovsky AD, Prohaska S, Jefferis GSXE.
-[link](https://www.cell.com/neuron/fulltext/S0896-6273(16)30265-3?_returnURL=https%3A%2F%2Flinkinghub.elsevier.com%2Fretrieve%2Fpii%2FS0896627316302653%3Fshowall%3Dtrue)
-2. **Comparison of neurons based on connectivity**: Science. 2012 Jul 27;337(6093):437-44. doi: 10.1126/science.1221762.
-*The connectome of a decision-making neural network.*
-Jarrell TA, Wang Y, Bloniarz AE, Brittin CA, Xu M, Thomson JN, Albertson DG, Hall DH, Emmons SW.
-[link](http://science.sciencemag.org/content/337/6093/437.long)
-3. **Comparison of neurons based on synapse distribution**: eLife. doi: 10.7554/eLife.16799
-*Synaptic transmission parallels neuromodulation in a central food-intake circuit.*
-Schlegel P, Texada MJ, Miroschnikow A, Schoofs A, Hückesfeld S, Peters M, … Pankratz MJ.
-[link](https://elifesciences.org/content/5/e16799)
-4. **Synapse flow centrality and segregation index**: eLife. doi: 10.7554/eLife.12059
-*Quantitative neuroanatomy for connectomics in Drosophila.*
-Schneider-Mizell CM, Gerhard S, Longair M, Kazimiers T, Li, Feng L, Zwart M … Cardona A.
-[link](https://elifesciences.org/articles/12059)
+#### Report bugs or request features
+Open an [issue](https://github.com/navis-org/navis/issues). For bug reports
+please make sure to include some code/data with a minimum example for us to
+reproduce the bug.
+
+#### Contribute code
+We're always happy for people to contribute code - be it a small bug fix, a
+new feature or improved documentation.
 
-## Contributing
+Here's how you'd do it in a nutshell:
 
 1. Fork this repository
 2. `git clone` it to your local machine
 3. Install the full development dependencies with `pip install -r requirements.txt`
 4. Install the package in editable mode with `pip install -e ".[all]"`
 5. Create, `git add`, `git commit`, `git push`, and pull request your changes.
 
@@ -153,7 +118,11 @@
 Docstrings should use the [numpydoc](https://numpydoc.readthedocs.io/en/latest/format.html) format,
 and make sure you include any relevant links and citations.
 Unit tests should be [doctests](https://docs.python.org/3/library/doctest.html)
 and/or use [pytest](https://docs.pytest.org/en/stable/) in the `./tests` directory.
 
 Doctests have access to the `tmp_dir: pathlib.Path` variable,
 which should be used if any files need to be written.
+
+Feel free to get in touch either through an [issue](https://github.com/navis-org/navis/issues)
+or [discussion](https://github.com/navis-org/navis/discussions) if you need
+pointers or input on how to implement an idea.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `navis-1.5.0/navis/__init__.py` & `navis-1.6.0/navis/__init__.py`

 * *Files identical despite different names*

### Comparing `navis-1.5.0/navis/__version__.py` & `navis-1.6.0/navis/__version__.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,9 +7,9 @@
 #    (at your option) any later version.
 #
 #    This program is distributed in the hope that it will be useful,
 #    but WITHOUT ANY WARRANTY; without even the implied warranty of
 #    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #    GNU General Public License for more details.
 
-__version__ = "1.5.0"
-__version_vector__ = (1, 5, 0)
+__version__ = "1.6.0"
+__version_vector__ = (1, 6, 0)
```

### Comparing `navis-1.5.0/navis/config.py` & `navis-1.6.0/navis/config.py`

 * *Files identical despite different names*

### Comparing `navis-1.5.0/navis/conftest.py` & `navis-1.6.0/navis/conftest.py`

 * *Files identical despite different names*

### Comparing `navis-1.5.0/navis/connectivity/__init__.py` & `navis-1.6.0/navis/connectivity/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,12 +9,14 @@
 #    This program is distributed in the hope that it will be useful,
 #    but WITHOUT ANY WARRANTY; without even the implied warranty of
 #    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #    GNU General Public License for more details.
 
 from .predict import cable_overlap
 from .matrix_utils import group_matrix
+from .adjacency import NeuronConnector
 from .cnmetrics import connectivity_sparseness
 from .similarity import connectivity_similarity, synapse_similarity
 
 __all__ = ['connectivity_sparseness', 'cable_overlap',
-           'connectivity_similarity', 'synapse_similarity']
+           'connectivity_similarity', 'synapse_similarity',
+           'NeuronConnector']
```

### Comparing `navis-1.5.0/navis/connectivity/cnmetrics.py` & `navis-1.6.0/navis/connectivity/cnmetrics.py`

 * *Files identical despite different names*

### Comparing `navis-1.5.0/navis/connectivity/matrix_utils.py` & `navis-1.6.0/navis/connectivity/matrix_utils.py`

 * *Files identical despite different names*

### Comparing `navis-1.5.0/navis/connectivity/predict.py` & `navis-1.6.0/navis/connectivity/predict.py`

 * *Files identical despite different names*

### Comparing `navis-1.5.0/navis/connectivity/similarity.py` & `navis-1.6.0/navis/connectivity/similarity.py`

 * *Files identical despite different names*

### Comparing `navis-1.5.0/navis/conversion/__init__.py` & `navis-1.6.0/navis/conversion/__init__.py`

 * *Files identical despite different names*

### Comparing `navis-1.5.0/navis/conversion/converters.py` & `navis-1.6.0/navis/conversion/converters.py`

 * *Files 0% similar despite different names*

```diff
@@ -146,15 +146,15 @@
     fix_mesh :  bool
                 Whether to try to fix some common issues in the mesh before
                 skeletonization. Note that this might compromise the
                 vertex-to-node-ID mapping.
     shave :     bool
                 Whether to "shave" the resulting skeleton to reduce bristles
                 on the backbone.
-    heal :      bool
+    heal :      bool | "LEAFS" | "ALL"
                 Whether to heal the resulting skeleton if it is fragmented.
                 For more control over the stitching set `heal=False` and use
                 :func:`navis.heal_skeleton` directly. Note that this
                 can be fairly costly if the mesh as many tiny fragments.
     connectors : bool
                 Whether to carry over existing connector tables. This will
                 attach connectors by first snapping them to the closest mesh
```

### Comparing `navis-1.5.0/navis/conversion/meshing.py` & `navis-1.6.0/navis/conversion/meshing.py`

 * *Files identical despite different names*

### Comparing `navis-1.5.0/navis/conversion/wrappers.py` & `navis-1.6.0/navis/conversion/wrappers.py`

 * *Files identical despite different names*

### Comparing `navis-1.5.0/navis/core/__init__.py` & `navis-1.6.0/navis/core/__init__.py`

 * *Files identical despite different names*

### Comparing `navis-1.5.0/navis/core/base.py` & `navis-1.6.0/navis/core/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -334,15 +334,19 @@
             raise ValueError('Neuron must implement `.bbox` (bounding box) '
                              'property to calculate extents.')
         bbox = self.bbox
         return bbox[:, 1] - bbox[:, 0]
 
     @property
     def id(self) -> Any:
-        """Hashable ID."""
+        """ID of the neuron.
+
+        Must be hashable. If not set, will assign a random unique identifier.
+        Can be indexed by using the ``NeuronList.idx[]`` locator.
+        """
         return getattr(self, '_id', None)
 
     @id.setter
     def id(self, value):
         try:
             hash(value)
         except BaseException:
@@ -408,15 +412,15 @@
             self._connectors = utils.validate_table(v,
                                                     required=['x', 'y', 'z'],
                                                     rename=True,
                                                     restrict=False)
 
     @property
     def presynapses(self):
-        """Table with presynapses.
+        """Table with presynapses (filtered from connectors table).
 
         Requires a "type" column in connector table. Will look for type labels
         that include "pre" or that equal 0 or "0".
         """
         if not isinstance(getattr(self, 'connectors', None), pd.DataFrame):
             raise ValueError('No connector table found.')
         # Make an educated guess what presynapses are
@@ -429,15 +433,15 @@
         elif len(pre) > 1:
             raise ValueError(f'Found ambigous presynapse labels: {pre}')
 
         return self.connectors[self.connectors['type'] == pre[0]]
 
     @property
     def postsynapses(self):
-        """Table with postsynapses.
+        """Table with postsynapses (filtered from connectors table).
 
         Requires a "type" column in connector table. Will look for type labels
         that include "post" or that equal 1 or "1".
         """
         if not isinstance(getattr(self, 'connectors', None), pd.DataFrame):
             raise ValueError('No connector table found.')
         # Make an educated guess what presynapses are
```

### Comparing `navis-1.5.0/navis/core/core_utils.py` & `navis-1.6.0/navis/core/core_utils.py`

 * *Files identical despite different names*

### Comparing `navis-1.5.0/navis/core/dotprop.py` & `navis-1.6.0/navis/core/dotprop.py`

 * *Files 0% similar despite different names*

```diff
@@ -194,15 +194,15 @@
             if 'pykdtree' in str(type(state['_tree'])):
                 _ = state.pop('_tree')
 
         return state
 
     @property
     def alpha(self):
-        """Alpha value for tangent vectors."""
+        """Alpha value for tangent vectors (optional)."""
         if isinstance(self._alpha, type(None)):
             if isinstance(self.k, type(None)) or (self.k <= 0):
                 raise ValueError('Unable to calculate `alpha` for Dotprops not '
                                  'generated using k-nearest-neighbors.')
 
             self.recalculate_tangents(self.k, inplace=True)
         return self._alpha
```

### Comparing `navis-1.5.0/navis/core/mesh.py` & `navis-1.6.0/navis/core/mesh.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 
 import copy
 import numbers
 import os
 import pint
 import warnings
 import scipy
-import warnings
 
 import networkx as nx
 import numpy as np
 import pandas as pd
 import skeletor as sk
 import trimesh as tm
 
@@ -52,15 +51,15 @@
 
 
 class MeshNeuron(BaseNeuron):
     """Neuron represented as mesh with vertices and faces.
 
     Parameters
     ----------
-    x
+    x :             mesh-like | tuple | dictionary | filepath | None
                     Data to construct neuron from:
                      - any object that has ``.vertices`` and ``.faces``
                        properties (e.g. a trimesh.Trimesh)
                      - a tuple ``(vertices, faces)``
                      - a dictionary ``{"vertices": (N, 3), "faces": (M, 3)}``
                      - filepath to a file that can be read by ``trimesh.load``
                      - ``None`` will initialize an empty MeshNeuron
@@ -98,19 +97,15 @@
     #: Temporary attributes that need clearing when neuron data changes
     TEMP_ATTR = ['_memory_usage', '_trimesh', '_skeleton', '_igraph', '_graph_nx']
 
     #: Core data table(s) used to calculate hash
     CORE_DATA = ['vertices', 'faces']
 
     def __init__(self,
-                 x: Union[pd.DataFrame,
-                          BufferedIOBase,
-                          str,
-                          'TreeNeuron',
-                          nx.DiGraph],
+                 x,
                  units: Union[pint.Unit, str] = None,
                  process: bool = True,
                  validate: bool = False,
                  **metadata
                  ):
         """Initialize Mesh Neuron."""
         super().__init__()
```

### Comparing `navis-1.5.0/navis/core/neuronlist.py` & `navis-1.6.0/navis/core/neuronlist.py`

 * *Files identical despite different names*

### Comparing `navis-1.5.0/navis/core/neurons.py` & `navis-1.6.0/navis/core/neurons.py`

 * *Files identical despite different names*

### Comparing `navis-1.5.0/navis/core/skeleton.py` & `navis-1.6.0/navis/core/skeleton.py`

 * *Files 2% similar despite different names*

```diff
@@ -390,14 +390,21 @@
                                                      ('parent_id', 'link', 'parent', 'Parent'),
                                                      ('x', 'X'),
                                                      ('y', 'Y'),
                                                      ('z', 'Z')],
                                            rename=True,
                                            optional={('radius', 'W'): 0},
                                            restrict=False)
+
+        # Make sure we don't end up with object dtype anywhere as this can
+        # cause problems
+        for c in ('node_id', 'parent_id'):
+            if self._nodes[c].dtype == 'O':
+                self._nodes[c] = self._nodes[c].astype(int)
+
         graph.classify_nodes(self)
 
     @property
     def n_trees(self) -> int:
         """Count number of connected trees in this neuron."""
         return len(self.subtrees)
 
@@ -454,15 +461,15 @@
                                                               ('type', 'relation', 'label', 'prepost')],
                                                     rename=True,
                                                     restrict=False)
 
     @property
     @requires_nodes
     def cycles(self) -> Optional[List[int]]:
-        """Cycles in neuron if any.
+        """Cycles in neuron (if any).
 
         See also
         --------
         networkx.find_cycles()
                     Function used to find cycles.
 
         """
@@ -473,19 +480,15 @@
         except nx.exception.NetworkXNoCycle:
             return None
         except BaseException:
             raise
 
     @property
     def simple(self) -> 'TreeNeuron':
-        """Return simple neuron representation.
-
-        Consists only of root, branch points and leafs.
-
-        """
+        """Simplified representation consisting only of root, branch points and leafs."""
         if not hasattr(self, '_simple'):
             self._simple = self.downsample(float('inf'),
                                            inplace=False)
         return self._simple
 
     @property
     def soma(self) -> Optional[Union[str, int]]:
@@ -590,27 +593,59 @@
 
     @property
     @requires_nodes
     def n_branches(self) -> Optional[int]:
         """Number of branch points."""
         return self.nodes[self.nodes.type == 'branch'].shape[0]
 
+    @property
+    @requires_nodes
+    def n_leafs(self) -> Optional[int]:
+        """Number of leaf nodes."""
+        return self.nodes[self.nodes.type == 'end'].shape[0]
+
     @temp_property
     def cable_length(self) -> Union[int, float]:
         """Cable length."""
         if not hasattr(self, '_cable_length'):
             # Simply sum up edge weight of all graph edges
             if config.use_igraph and self.igraph:
                 w = self.igraph.es.get_attribute_values('weight')  # type: ignore # doesn't know iGraph
             else:
                 w = nx.get_edge_attributes(self.graph, 'weight').values()
             self._cable_length = np.nansum(list(w))
         return self._cable_length
 
     @property
+    def surface_area(self) -> float:
+        """Radius-based lateral surface area."""
+        if 'radius' not in self.nodes.columns:
+            raise ValueError(f'Neuron {self.id} does not have radius information')
+
+        if any(self.nodes.radius < 0):
+            logger.warning(f'Neuron {self.id} has negative radii - area will not be correct.')
+
+        if any(self.nodes.radius.isnull()):
+            logger.warning(f'Neuron {self.id} has NaN radii - area will not be correct.')
+
+        # Generate radius dict
+        radii = self.nodes.set_index('node_id').radius.to_dict()
+        # Drop root node(s)
+        not_root = self.nodes.parent_id >= 0
+        # For each cylinder get the height
+        h = morpho.mmetrics.parent_dist(self, root_dist=0)[not_root]
+
+        # Radii for top and bottom of tapered cylinder
+        nodes = self.nodes[not_root]
+        r1 = nodes.node_id.map(radii).values
+        r2 = nodes.parent_id.map(radii).values
+
+        return (np.pi * (r1 + r2) * np.sqrt( (r1-r2)**2 + h**2)).sum()
+
+    @property
     def volume(self) -> float:
         """Radius-based volume."""
         if 'radius' not in self.nodes.columns:
             raise ValueError(f'Neuron {self.id} does not have radius information')
 
         if any(self.nodes.radius < 0):
             logger.warning(f'Neuron {self.id} has negative radii - volume will not be correct.')
@@ -645,15 +680,15 @@
             mn = np.min(np.vstack((mn, cn_mn)), axis=0)
             mx = np.max(np.vstack((mx, cn_mx)), axis=0)
 
         return np.vstack((mn, mx)).T
 
     @property
     def sampling_resolution(self) -> float:
-        """Average cable length between 2 nodes."""
+        """Average cable length between child -> parent nodes."""
         return self.cable_length / self.n_nodes
 
     @temp_property
     def segments(self) -> List[list]:
         """Neuron broken down into linear segments (see also `.small_segments`)."""
         # Calculate if required
         if not hasattr(self, '_segments'):
@@ -680,15 +715,15 @@
         elif how == 'break':
             return graph._break_segments(self)
         else:
             raise ValueError(f'Unknown method: "{how}"')
 
     @property
     def n_skeletons(self) -> int:
-        """Return number of seperate skeletons in this neuron."""
+        """Number of seperate skeletons in this neuron."""
         return len(self.root)
 
     def _clear_temp_attr(self, exclude: list = []) -> None:
         """Clear temporary attributes."""
         super()._clear_temp_attr(exclude=exclude)
 
         # Remove temporary node values
```

### Comparing `navis-1.5.0/navis/core/volumes.py` & `navis-1.6.0/navis/core/volumes.py`

 * *Files 2% similar despite different names*

```diff
@@ -588,18 +588,18 @@
         accepted_views = ['x', 'z', 'y', '-x', '-z', '-y']
 
         for ax in view:
             if ax not in accepted_views:
                 raise ValueError(f'Unable to parse "{ax}" view')
 
         try:
-            from shapely.ops import cascaded_union, polygonize  # type: ignore
+            from shapely.ops import unary_union, polygonize  # type: ignore
             import shapely.geometry as geometry  # type: ignore
         except ImportError:
-            raise ImportError('This function needs the shapely package.')
+            raise ImportError('This function needs the shapely>=1.8.0')
 
         coords: np.ndarray
 
         map = {'x': 0, 'y': 1, 'z': 2}
 
         x_ix = map[view[0].replace('-', '').replace('+', '')]
         y_ix = map[view[1].replace('-', '').replace('+', '')]
@@ -608,17 +608,17 @@
         ymod = -1 if '-' in view[1] else 1
         coords = self.vertices[:, [x_ix, y_ix]] * np.array([xmod, ymod])
 
         tri = scipy.spatial.Delaunay(coords)
         edges: set = set()
         edge_points: list = []
         # loop over triangles:
-        # ia, ib, ic = indices of corner points of the
-        # triangle
-        for ia, ib, ic in tri.vertices:
+        # ia, ib, ic = indices of corner points of the triangle
+        # Note that "vertices" property was renamed to "simplices"
+        for ia, ib, ic in getattr(tri, 'simplices', getattr(tri, 'vertices', [])):
             pa: np.ndarray = coords[ia]  # type: ignore
             pb: np.ndarray = coords[ib]  # type: ignore
             pc: np.ndarray = coords[ic]  # type: ignore
             # Lengths of sides of triangle
             a = math.sqrt((pa[0] - pb[0])**2 + (pa[1] - pb[1])**2)  # type: ignore
             b = math.sqrt((pb[0] - pc[0])**2 + (pb[1] - pc[1])**2)  # type: ignore
             c = math.sqrt((pc[0] - pa[0])**2 + (pc[1] - pa[1])**2)  # type: ignore
@@ -631,15 +631,15 @@
             if circum_r < 1.0 / alpha:
                 add_edge(edges, edge_points, coords, ia, ib)
                 add_edge(edges, edge_points, coords, ib, ic)
                 add_edge(edges, edge_points, coords, ic, ia)
 
         m = geometry.MultiLineString(edge_points)
         triangles = list(polygonize(m))
-        concave_hull = cascaded_union(triangles)
+        concave_hull = unary_union(triangles)
 
         # Try with current settings, if this is not successful, try again
         # with lower alpha
         try:
             return list(concave_hull.exterior.coords)
         except AttributeError:
             return self.to_2d(alpha=alpha / 10, view=view, invert_y=invert_y)
```

### Comparing `navis-1.5.0/navis/core/voxel.py` & `navis-1.6.0/navis/core/voxel.py`

 * *Files identical despite different names*

### Comparing `navis-1.5.0/navis/data/__init__.py` & `navis-1.6.0/navis/data/__init__.py`

 * *Files identical despite different names*

### Comparing `navis-1.5.0/navis/data/gml/1734350788.gml` & `navis-1.6.0/navis/data/gml/1734350788.gml`

 * *Files identical despite different names*

### Comparing `navis-1.5.0/navis/data/gml/1734350908.gml` & `navis-1.6.0/navis/data/gml/1734350908.gml`

 * *Files identical despite different names*

### Comparing `navis-1.5.0/navis/data/gml/722817260.gml` & `navis-1.6.0/navis/data/gml/722817260.gml`

 * *Files identical despite different names*

### Comparing `navis-1.5.0/navis/data/gml/754534424.gml` & `navis-1.6.0/navis/data/gml/754534424.gml`

 * *Files identical despite different names*

### Comparing `navis-1.5.0/navis/data/gml/754538881.gml` & `navis-1.6.0/navis/data/gml/754538881.gml`

 * *Files identical despite different names*

### Comparing `navis-1.5.0/navis/data/load_data.py` & `navis-1.6.0/navis/data/load_data.py`

 * *Files identical despite different names*

### Comparing `navis-1.5.0/navis/data/obj/1734350788.obj` & `navis-1.6.0/navis/data/obj/1734350788.obj`

 * *Files identical despite different names*

### Comparing `navis-1.5.0/navis/data/obj/1734350908.obj` & `navis-1.6.0/navis/data/obj/1734350908.obj`

 * *Files identical despite different names*

### Comparing `navis-1.5.0/navis/data/obj/722817260.obj` & `navis-1.6.0/navis/data/obj/722817260.obj`

 * *Files identical despite different names*

### Comparing `navis-1.5.0/navis/data/obj/754534424.obj` & `navis-1.6.0/navis/data/obj/754534424.obj`

 * *Files identical despite different names*

### Comparing `navis-1.5.0/navis/data/obj/754538881.obj` & `navis-1.6.0/navis/data/obj/754538881.obj`

 * *Files identical despite different names*

### Comparing `navis-1.5.0/navis/data/readme.md` & `navis-1.6.0/navis/data/readme.md`

 * *Files identical despite different names*

### Comparing `navis-1.5.0/navis/data/swc/1734350788.swc` & `navis-1.6.0/navis/data/swc/1734350788.swc`

 * *Files identical despite different names*

### Comparing `navis-1.5.0/navis/data/swc/1734350908.swc` & `navis-1.6.0/navis/data/swc/1734350908.swc`

 * *Files identical despite different names*

### Comparing `navis-1.5.0/navis/data/swc/722817260.swc` & `navis-1.6.0/navis/data/swc/722817260.swc`

 * *Files identical despite different names*

### Comparing `navis-1.5.0/navis/data/swc/754534424.swc` & `navis-1.6.0/navis/data/swc/754534424.swc`

 * *Files identical despite different names*

### Comparing `navis-1.5.0/navis/data/swc/754538881.swc` & `navis-1.6.0/navis/data/swc/754538881.swc`

 * *Files identical despite different names*

### Comparing `navis-1.5.0/navis/data/synapses/1734350788.csv` & `navis-1.6.0/navis/data/synapses/1734350788.csv`

 * *Files identical despite different names*

### Comparing `navis-1.5.0/navis/data/synapses/1734350908.csv` & `navis-1.6.0/navis/data/synapses/1734350908.csv`

 * *Files identical despite different names*

### Comparing `navis-1.5.0/navis/data/synapses/722817260.csv` & `navis-1.6.0/navis/data/synapses/722817260.csv`

 * *Files identical despite different names*

### Comparing `navis-1.5.0/navis/data/synapses/754534424.csv` & `navis-1.6.0/navis/data/synapses/754534424.csv`

 * *Files identical despite different names*

### Comparing `navis-1.5.0/navis/data/synapses/754538881.csv` & `navis-1.6.0/navis/data/synapses/754538881.csv`

 * *Files identical despite different names*

### Comparing `navis-1.5.0/navis/data/volumes/lh.obj` & `navis-1.6.0/navis/data/volumes/lh.obj`

 * *Files identical despite different names*

### Comparing `navis-1.5.0/navis/data/volumes/neuropil.obj` & `navis-1.6.0/navis/data/volumes/neuropil.obj`

 * *Files identical despite different names*

### Comparing `navis-1.5.0/navis/graph/__init__.py` & `navis-1.6.0/navis/graph/__init__.py`

 * *Files identical despite different names*

### Comparing `navis-1.5.0/navis/graph/clinic.py` & `navis-1.6.0/navis/graph/clinic.py`

 * *Files identical despite different names*

### Comparing `navis-1.5.0/navis/graph/converters.py` & `navis-1.6.0/navis/graph/converters.py`

 * *Files identical despite different names*

### Comparing `navis-1.5.0/navis/graph/graph_utils.py` & `navis-1.6.0/navis/graph/graph_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,15 +81,15 @@
 
     assert weight in ('weight', None), f'Unable to use weight "{weight}"'
     d = dist_to_root(x, igraph_indices=False, weight=weight)
     endNodeIDs = x.nodes[x.nodes.type == 'end'].node_id.values
     endNodeIDs = sorted(endNodeIDs, key=lambda x: d.get(x, 0), reverse=True)
 
     if config.use_igraph and x.igraph:
-        g: igraph.Graph = x.igraph
+        g: igraph.Graph = x.igraph  # noqa
         # Convert endNodeIDs to indices
         id2ix = dict(zip(x.igraph.vs['node_id'], range(len(x.igraph.vs))))
         endNodeIDs = [id2ix[n] for n in endNodeIDs]
     else:
         g: nx.DiGraph = x.graph
 
     seen: set = set()
@@ -147,15 +147,15 @@
     >>> m = navis.example_neurons(1, kind='mesh')
     >>> cc = navis.graph_utils._connected_components(m)
 
     """
     assert isinstance(x, (core.TreeNeuron, core.MeshNeuron))
 
     if config.use_igraph and x.igraph:
-        G: igraph.Graph = x.igraph
+        G: igraph.Graph = x.igraph  # noqa
         # Get the vertex clustering
         vc = G.components(mode='WEAK')
         # Membership maps indices to connected components
         ms = np.array(vc.membership)
         if isinstance(x, core.TreeNeuron):
             # For skeletons we need node IDs
             ids = np.array(G.vs['node_id'])
@@ -203,15 +203,15 @@
         logger.error('Unexpected datatype: %s' % str(type(x)))
         raise ValueError
 
     # At this point x is TreeNeuron
     x: core.TreeNeuron
 
     if x.igraph and config.use_igraph:
-        g: Union['igraph.Graph', 'nx.DiGraph'] = x.igraph
+        g: Union['igraph.Graph', 'nx.DiGraph'] = x.igraph # noqa
         end = g.vs.select(_indegree=0).indices
         branch = g.vs.select(_indegree_gt=1, _outdegree=1).indices
         root = g.vs.select(_outdegree=0).indices
 
         # Get seeds
         seeds = branch + end
         # Remove seeds that are also roots (=disconnected single nodes)
@@ -304,15 +304,15 @@
 def _edge_count_to_root_old(x: 'core.TreeNeuron') -> dict:
     """Return a map of nodeID vs number of edges.
 
     Starts from the first node that lacks successors (aka the root).
 
     """
     current_level: List[int]
-    g: Union['igraph.Graph', 'nx.DiGraph']
+    g: Union['igraph.Graph', 'nx.DiGraph']  # noqa
     if x.igraph and config.use_igraph:
         g = x.igraph
         current_level = g.vs(_outdegree=0).indices
     else:
         g = x.graph
         current_level = list(x.root)
 
@@ -336,17 +336,17 @@
         dist = {g.vs[k]['node_id']: v for k, v in dist.items()}
 
     return dist
 
 
 @utils.map_neuronlist(desc='Classifying', allow_parallel=True)
 @utils.lock_neuron
-def classify_nodes(x: 'core.NeuronObject',
-                   inplace: bool = True
-                   ) -> Optional['core.NeuronObject']:
+def _classify_nodes_old(x: 'core.NeuronObject',
+                        inplace: bool = True
+                        ) -> Optional['core.NeuronObject']:
     """Classify neuron's nodes into end nodes, branches, slabs or root.
 
     Adds ``'type'`` column to ``x.nodes``.
 
     Parameters
     ----------
     x :         TreeNeuron | NeuronList
@@ -410,14 +410,82 @@
     cat_types = CategoricalDtype(categories=["end", "branch", "root", "slab"],
                                  ordered=False)
     x.nodes['type'] = x.nodes['type'].astype(cat_types)
 
     return x
 
 
+
+@utils.map_neuronlist(desc='Classifying', allow_parallel=True)
+@utils.lock_neuron
+def classify_nodes(x: "core.NeuronObject", categorical=True, inplace: bool = True):
+    """Classify neuron's nodes into end nodes, branches, slabs or root.
+
+    Adds a ``'type'`` column to ``x.nodes`` table.
+
+    Parameters
+    ----------
+    x :         TreeNeuron | NeuronList
+                Neuron(s) whose nodes to classify.
+    categorical : bool
+                If True (default), will use categorical data type which takes
+                up much less memory at a small run-time overhead.
+    inplace :   bool, optional
+                If ``False``, nodes will be classified on a copy which is then
+                returned leaving the original neuron unchanged.
+
+    Returns
+    -------
+    TreeNeuron/List
+
+    Examples
+    --------
+    >>> import navis
+    >>> nl = navis.example_neurons(2)
+    >>> _ = navis.graph.classify_nodes(nl, inplace=True)
+
+    """
+    if not inplace:
+        x = x.copy()
+
+    if not isinstance(x, core.TreeNeuron):
+        raise TypeError(f'Expected TreeNeuron(s), got "{type(x)}"')
+
+    if x.nodes.empty:
+        x.nodes["type"] = None
+        return x
+
+    # Make sure there are nodes to classify
+    # Note: I have tried to optimized the s**t out of this, i.e. every
+    # single line of code here has been tested for speed. Do not
+    # change anything unless you know what you're doing!
+
+    # Turns out that numpy.isin() recently started to complain if the
+    # node_ids are uint64 and the parent_ids are int64 (but strangely
+    # not with 32bit integers). If that's the case we have to convert
+    # the node_ids to int64.
+    node_ids = x.nodes.node_id.values
+    parent_ids = x.nodes.parent_id.values
+
+    if node_ids.dtype == np.uint64:
+        node_ids = node_ids.astype(np.int64)
+
+    cl = np.full(len(x.nodes), "slab", dtype="<U6")
+    cl[~np.isin(node_ids, parent_ids)] = "end"
+    bp = x.nodes.parent_id.value_counts()
+    bp = bp.index.values[bp.values > 1]
+    cl[np.isin(node_ids, bp)] = "branch"
+    cl[parent_ids < 0] = "root"
+    if categorical:
+        cl = pd.Categorical(cl, categories=["end", "branch", "root", "slab"], ordered=False)
+    x.nodes["type"] = cl
+
+    return x
+
+
 #  only this combination will return a single bool
 @overload
 def distal_to(x: 'core.TreeNeuron',
               a: Union[str, str],
               b: Union[str, int],
               ) -> bool:
     pass
@@ -678,14 +746,18 @@
 
         indices = np.where(np.isin(nodeList, from_))[0]
         ix = nodeList[indices]
     else:
         indices = None
         ix = nodeList
 
+    # For some reason csgrpah.dijkstra expects indices/indptr as int32
+    # igraph seems to do that by default but networkx uses int64 for indices
+    m.indptr = m.indptr.astype('int32', copy=False)
+    m.indices = m.indices.astype('int32', copy=False)
     dmat = csgraph.dijkstra(m,
                             directed=directed,
                             indices=indices,
                             limit=limit)
 
     return pd.DataFrame(dmat, columns=nodeList, index=ix)  # type: ignore  # no stubs
 
@@ -773,15 +845,15 @@
     if isinstance(x, core.NeuronList):
         if len(x) == 1:
             x = x[0]
         else:
             raise ValueError(f'Need a single TreeNeuron, got {len(x)}')
 
     if isinstance(x, (core.TreeNeuron, core.MeshNeuron)):
-        G: Union['igraph.Graph',
+        G: Union['igraph.Graph',  # noqa
                  'nx.DiGraph'] = x.igraph if (x.igraph and config.use_igraph) else x.graph
     elif isinstance(x, nx.DiGraph):
         G = x
     elif 'igraph' in str(type(x.igraph)):
         # We can't use isinstance here because igraph library might not be installed
         G = x
     else:
@@ -1705,16 +1777,19 @@
     if weight_attr is None:
         weights = [1] * len(edges)
     else:
         weights = graph.es[weight_attr]
     if not graph.is_directed():
         edges.extend([(v, u) for u, v in edges])
         weights.extend(weights)
-    return csr_matrix((weights, zip(*edges)),
-                      shape=(len(graph.vs), len(graph.vs)))
+    # Note: previously, we used a generator (weights, zip(*egdes)) as input to
+    # csr_matrix but with Scipy 1.13.0 this has stopped working
+    edges = np.array(edges)
+    return csr_matrix((weights, (edges[:,0], edges[:,1])),
+                       shape=(len(graph.vs), len(graph.vs)))
 
 
 def connected_subgraph(x: Union['core.TreeNeuron', nx.DiGraph],
                        ss: Sequence[Union[str, int]]) -> Tuple[np.ndarray, Union[int, str]]:
     """Return set of nodes necessary to connect all nodes in subset ``ss``.
 
     Parameters
@@ -2068,14 +2143,16 @@
 
     if not inplace:
         x = x.copy()
 
     if g.is_directed():
         g = g.to_undirected()
 
+    g = nx.minimum_spanning_tree(g, weight='weight')
+
     if not root:
         root = x.root[0] if x.root[0] in g.nodes else next(iter(g.nodes))
 
     # Generate tree for the main component
     tree = nx.dfs_tree(g, source=root)
 
     # Generate list of parents
```

### Comparing `navis-1.5.0/navis/interfaces/allen_celltypes.py` & `navis-1.6.0/navis/interfaces/allen_celltypes.py`

 * *Files identical despite different names*

### Comparing `navis-1.5.0/navis/interfaces/blender.py` & `navis-1.6.0/navis/interfaces/blender.py`

 * *Files identical despite different names*

### Comparing `navis-1.5.0/navis/interfaces/cytoscape.py` & `navis-1.6.0/navis/interfaces/cytoscape.py`

 * *Files identical despite different names*

### Comparing `navis-1.5.0/navis/interfaces/insectbrain_db.py` & `navis-1.6.0/navis/interfaces/insectbrain_db.py`

 * *Files 2% similar despite different names*

```diff
@@ -179,41 +179,42 @@
     if token:
         session.token = token
     else:
         session.fetch_token()
 
 
 def get_brain_meshes(species: Union[str, int],
-                     combine: bool = False
+                     combine: bool = False,
+                     max_threads: int = 4
                      ) -> Optional[List[Volume]]:
     """Fetch brain meshes for given species.
 
     Parameters
     ----------
     species:        str | int
                     Species for which to fetch brain volumes. Strings are
                     interpreted as names (scientific or common), integers as IDs.
     combine :       bool, optional
                     If True, will combine subvolumes (i.e. neuropils) into
                     a single navis.Volume - else will return list with volumes.
+    max_threads :   int
+                    Number of parallel threads to use for fetching meshes.
 
     Returns
     -------
     list of navis.Volume
 
     Examples
     --------
     >>> import navis
     >>> import navis.interfaces.insectbrain_db as ibdb
     >>> v = ibdb.get_brain_meshes('Desert Locust', combine_vols=True)
     >>> navis.plot3d(v)
 
     """
-    obj_url = 'https://s3.eu-central-1.amazonaws.com/ibdb-file-storage/'
-
     # Get info with all available neuropils
     sp_info = get_species_info(species)
 
     # Go over all brains
     n_brains = len(sp_info.reconstructions)  # type: ignore
     n_reconstr = len([r for r in sp_info.reconstructions if r.get('viewer_files')])  # type: ignore
     logger.info(f'{n_reconstr} reconstruction(s) from {n_brains} brain(s) found')
@@ -223,56 +224,79 @@
                              disable=config.pbar_hide,
                              leave=config.pbar_leave,
                              desc='Brains'):  # type: ignore
         this_v = []
         # If no reconstructions, continue
         if not brain.get('viewer_files'):  # type: ignore
             continue
-        for file in config.tqdm(brain['viewer_files'],
-                                desc='Neuropils',
-                                disable=config.pbar_hide,
-                                leave=config.pbar_leave):
-            filename = file['p_file']['file_name']
-            path = file['p_file']['path']
-            url = make_url(obj_url, path)
-
-            resp = requests.get(url)
-            resp.raise_for_status()
-
-            f = io.BytesIO(resp.content)
-            mesh = tm.load_mesh(f, file_type='obj')
-
-            structures = file.get('structures')
-            if structures:
-                structure = structures[0].get('structure')
-                hemisphere = structures[0].get('hemisphere')
-                if structure:
-                    color = structure.get('color')
-                    if color:
-                        color = mcl.to_rgba(color, alpha=.5)
-                    else:
-                        color = (.85, .85, .85, .5)
-                name = structure.get('name', filename)
 
-                if hemisphere:
-                    name = f'{name} ({hemisphere})'
-
-            v = Volume(mesh, name=name, color=color)
-            this_v.append(v)
+        with ThreadPoolExecutor(max_workers=max_threads) as executor:
+            futures = {}
+            for file in brain['viewer_files']:
+                # If no file UUID, continue
+                if not file['p_file']['uuid']:
+                    continue
+                filename = file['p_file']['file_name']
+                f = executor.submit(_get_neuropil_mesh, file,)
+                futures[f] = filename
+
+            with config.tqdm(desc='Fetching',
+                            total=len(futures),
+                            leave=config.pbar_leave,
+                            disable=len(futures) == 1 or config.pbar_hide) as pbar:
+                for f in as_completed(futures):
+                    name = futures[f]
+                    pbar.update(1)
+                    try:
+                        this_v.append(f.result())
+                    except Exception as exc:
+                        print(f'{name} generated an exception:', exc)
 
         # Combine all volumes in this brain
         if combine:
             this_v = [Volume.combine(this_v)]
             this_v[0].color = (.85, .85, .85, .5)
+            this_v[0].name = sp_info.scientific_name
 
         volumes += this_v
 
     return volumes
 
 
+def _get_neuropil_mesh(file):
+    filename = file['p_file']['file_name']
+    # Get the AWS URL (with all the required headers) for this object
+    url = _get_download_url(file['p_file']['uuid'])
+
+    resp = requests.get(url)
+    resp.raise_for_status()
+
+    f = io.BytesIO(resp.content)
+    mesh = tm.load_mesh(f, file_type='obj')
+
+    structures = file.get('structures')
+    if structures:
+        structure = structures[0].get('structure')
+        hemisphere = structures[0].get('hemisphere')
+        if structure:
+            color = structure.get('color')
+            if color:
+                color = mcl.to_rgba(color, alpha=.5)
+            else:
+                color = (.85, .85, .85, .5)
+        name = structure.get('name', filename)
+
+        if hemisphere:
+            name = f'{name} ({hemisphere})'
+    else:
+        name = file['p_file']['file_name']
+
+    return Volume(mesh, name=name, color=color)
+
+
 @lru_cache()
 def get_species_info(species: Union[str, int]) -> pd.Series:
     """Get all info for given species.
 
     Parameters
     ----------
     species :       str | int
@@ -698,8 +722,16 @@
     prio['description'] = 100
 
     cols = sorted(df.columns, key=lambda x: prio.get(x, 10))
 
     return df[cols]
 
 
+def _get_download_url(uuid):
+    """Get AWS download URL for given object."""
+    url = f"https://www.insectbraindb.org/filestore/download_url/?uuid={uuid}"
+    r = requests.get(url)
+    r.raise_for_status()
+    return r.json()['url']
+
+
 session = Session()
```

### Comparing `navis-1.5.0/navis/interfaces/microns.py` & `navis-1.6.0/navis/interfaces/microns.py`

 * *Files identical despite different names*

### Comparing `navis-1.5.0/navis/interfaces/neuprint.py` & `navis-1.6.0/navis/interfaces/neuprint.py`

 * *Files 4% similar despite different names*

```diff
@@ -288,29 +288,36 @@
 
 
 def __fetch_mesh(bodyId, *, vol, lod, missing_mesh='raise'):
     """Fetch a single mesh (+ synapses) and construct navis MeshNeuron."""
     # Fetch mesh
     import cloudvolume
     try:
-        mesh = vol.mesh.get(bodyId, lod=lod)[bodyId]
+        if lod is None:
+            mesh = vol.mesh.get(bodyId)
+        else:
+            mesh = vol.mesh.get(bodyId, lod=lod)
     except cloudvolume.exceptions.MeshDecodeError as err:
         if 'not found' in str(err):
             if missing_mesh in ['warn', 'skip']:
                 if missing_mesh == 'warn':
                     logger.warning(f'No mesh found for {r.bodyId}')
                 return
             else:
                 raise
         else:
             raise
 
+    # Make sure we don't pass through a {bodyId: MeshObject} dictionary
+    if isinstance(mesh, dict):
+        mesh = mesh[bodyId]
+
     n = MeshNeuron(mesh)
     n.lod = lod
-    n.id =bodyId
+    n.id = bodyId
 
     return n
 
 
 @inject_client
 def fetch_skeletons(x, *, with_synapses=False, heal=False, missing_swc='raise',
                     parallel=True, max_threads=5, client=None):
@@ -423,15 +430,15 @@
     try:
         data = client.fetch_skeleton(r.bodyId, format='pandas', heal=heal)
     except HTTPError as err:
         if err.response.status_code == 400:
             if missing_swc in ['warn', 'skip']:
                 if missing_swc == 'warn':
                     logger.warning(f'No SWC found for {r.bodyId}')
-                    return
+                return
             else:
                 raise
         else:
             raise
 
     # Generate neuron
     # Note that we are currently assuming that the x/y/z data is isotropic
@@ -570,19 +577,29 @@
         return None
 
     # Check if any segmentation source matches our dataset exactly
     named_segs = [s for s in segs if s.get('name') == client.dataset]
     if len(named_segs):
         segs = named_segs
 
-    # Get the first entry
+    # If there are multiple segmentation layers, select the first entry
     seg_source = segs[0]['source']
 
-    # Make sure it's actually a string and not a {'source': url, 'subsources'...} dict
+    # If there are multiple segmentation sources for
+    # the layer we picked, select the first source.
+    if isinstance(seg_source, list):
+        seg_source = seg_source[0]
+
+    # If it's a dict like {'source': url, 'subsources'...},
+    # select the url.
     if isinstance(seg_source, dict):
         seg_source = seg_source['url']
 
+    if not isinstance(seg_source, str):
+        e = f"Could not understand segmentation source: {seg_source}"
+        raise RuntimeError(e)
+
     if len(segs) > 1:
         logger.warning(f'{len(segs)} segmentation sources found. Using the '
                        f'first entry: "{seg_source}"')
 
     return seg_source
```

### Comparing `navis-1.5.0/navis/interfaces/neuromorpho.py` & `navis-1.6.0/navis/interfaces/neuromorpho.py`

 * *Files identical despite different names*

### Comparing `navis-1.5.0/navis/interfaces/neuron/comp.py` & `navis-1.6.0/navis/interfaces/neuron/comp.py`

 * *Files 2% similar despite different names*

```diff
@@ -570,21 +570,26 @@
         if not what.startswith('_ref_'):
             what = f'_ref_{what}'
 
         rec_type = what.split('_')[-1]
         if rec_type not in self.records:
             self.records[rec_type] = {}
 
-        for w in where:
+        # # Get node segments only for nodes
+        is_node = ~np.array([is_NEURON_object(w) for w in where])
+        node_segs = np.zeros(len(where), dtype=object)
+        node_segs[is_node] = self.get_node_segment(where[is_node])
+
+        for i, w in enumerate(where):
             # If this is a neuron object (e.g. segment, section or point
             # process) we assume this does not need mapping
             if is_NEURON_object(w):
                 seg = w
             else:
-                seg = self.get_node_segment(w)
+                seg = node_segs[i]
 
             rec = neuron.h.Vector().record(getattr(seg, what))
 
             if label:
                 self.records[rec_type][label] = rec
             else:
                 self.records[rec_type][w] = rec
```

### Comparing `navis-1.5.0/navis/interfaces/neuron/network.py` & `navis-1.6.0/navis/interfaces/neuron/network.py`

 * *Files 0% similar despite different names*

```diff
@@ -334,14 +334,18 @@
 
             nc = neuron.h.NetCon(ns, proc)
             nc.weight[0] = weight
             nc.delay = 0
 
             self._stimuli.append(Stimulus(start, stop, f, randomness, i, ns, nc, label))
 
+    def clear_stimuli(self):
+        """Clear stimuli."""
+        self._stimuli = {}
+
     def connect(self, source, target, weight, delay=5):
         """Connect two neurons.
 
         Parameters
         ----------
         source :    int | str
                     ID of the source.
```

### Comparing `navis-1.5.0/navis/interfaces/neuron/utils.py` & `navis-1.6.0/navis/interfaces/neuron/utils.py`

 * *Files identical despite different names*

### Comparing `navis-1.5.0/navis/interfaces/r.py` & `navis-1.6.0/navis/interfaces/r.py`

 * *Files identical despite different names*

### Comparing `navis-1.5.0/navis/interfaces/vfb.py` & `navis-1.6.0/navis/interfaces/vfb.py`

 * *Files identical despite different names*

### Comparing `navis-1.5.0/navis/intersection/__init__.py` & `navis-1.6.0/navis/intersection/__init__.py`

 * *Files identical despite different names*

### Comparing `navis-1.5.0/navis/intersection/convex.py` & `navis-1.6.0/navis/intersection/convex.py`

 * *Files identical despite different names*

### Comparing `navis-1.5.0/navis/intersection/intersect.py` & `navis-1.6.0/navis/intersection/intersect.py`

 * *Files identical despite different names*

### Comparing `navis-1.5.0/navis/intersection/ray.py` & `navis-1.6.0/navis/intersection/ray.py`

 * *Files identical despite different names*

### Comparing `navis-1.5.0/navis/io/__init__.py` & `navis-1.6.0/navis/io/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,24 +7,28 @@
 #    (at your option) any later version.
 #
 #    This program is distributed in the hope that it will be useful,
 #    but WITHOUT ANY WARRANTY; without even the implied warranty of
 #    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #    GNU General Public License for more details.
 
-from .json_io import write_json, read_json
+from .json_io import read_json, write_json
 from .swc_io import read_swc, write_swc
 from .nrrd_io import read_nrrd, write_nrrd
-from .precomputed_io import write_precomputed, read_precomputed
+from .precomputed_io import read_precomputed, write_precomputed
 from .hdf_io import read_h5, write_h5, inspect_h5
 from .rda_io import read_rda
-from .nmx_io import read_nmx
+from .nmx_io import read_nmx, read_nml
 from .mesh_io import read_mesh, write_mesh
 from .tiff_io import read_tiff
+from .pq_io import read_parquet, write_parquet, scan_parquet
 
-__all__ = ['write_json', 'read_json',
+__all__ = ['read_json', 'write_json',
            'read_swc', 'write_swc',
            'read_nrrd', 'write_nrrd',
            'read_h5', 'write_h5', 'inspect_h5',
-           'write_precomputed', 'read_precomputed',
+           'read_precomputed', 'write_precomputed',
            'read_tiff',
-           'read_rda', 'read_nmx', 'read_mesh', 'write_mesh']
+           'read_rda',
+           'read_nmx', 'read_nml',
+           'read_mesh', 'write_mesh',
+           'read_parquet', 'write_parquet', 'scan_parquet']
```

### Comparing `navis-1.5.0/navis/io/base.py` & `navis-1.6.0/navis/io/base.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 
 import datetime
 import io
 import os
 import re
 import requests
 import tempfile
+import tarfile
 
 import multiprocessing as mp
 import numpy as np
 import pandas as pd
 
 from abc import ABC
 from functools import partial
@@ -246,14 +247,16 @@
 
         yield from (f for f in dpath.glob(pattern) if self.is_valid_file(f))
 
     def is_valid_file(self, file):
         """Return true if file should be considered for reading."""
         if isinstance(file, ZipInfo):
             file = file.filename
+        elif isinstance(file, tarfile.TarInfo):
+            file = file.name
         elif isinstance(file, Path):
             file = file.name
 
         if str(file).endswith(self.file_ext):
             return True
         return False
 
@@ -400,21 +403,106 @@
         core.NeuronList
 
         """
         fpath = Path(fpath).expanduser()
         read_fn = partial(self.read_from_zip,
                           zippath=fpath, attrs=attrs,
                           on_error=on_error)
-        neurons = parallel_read_zip(read_fn=read_fn,
+        neurons = parallel_read_archive(read_fn=read_fn,
                                     fpath=fpath,
                                     file_ext=self.is_valid_file,
                                     limit=limit,
                                     parallel=parallel)
         return core.NeuronList(neurons)
 
+    def read_from_tar(
+        self, files: Union[str, List[str]],
+        tarpath: os.PathLike,
+        attrs: Optional[Dict[str, Any]] = None,
+        on_error: Union[Literal['ignore', Literal['raise']]] = 'ignore'
+    ) -> 'core.NeuronList':
+        """Read given files from a tar into a NeuronList.
+
+        Typically not used directly but via `read_tar()` dispatcher.
+
+        Parameters
+        ----------
+        files :     tarfile.TarInfo | list thereof
+                    Files inside the tar file to read.
+        tarpath :   str | os.PathLike
+                    Path to tar file.
+        attrs :     dict or None
+                    Arbitrary attributes to include in the TreeNeuron.
+        on_error :  'ignore' | 'raise'
+                    What do do when error is encountered.
+
+        Returns
+        -------
+        core.NeuronList
+
+        """
+        p = Path(tarpath)
+        files = utils.make_iterable(files)
+
+        neurons = []
+        with tarfile.open(p, 'r') as tf:
+            for file in files:
+                # Note the `file` is of type tarfile.TarInfo here
+                props = self.parse_filename(file.name.split('/')[-1])
+                props['origin'] = str(p)
+                try:
+                    n = self.read_bytes(tf.extractfile(file).read(),
+                                        merge_dicts(props, attrs))
+                    neurons.append(n)
+                except BaseException:
+                    if on_error == 'ignore':
+                        logger.warning(f'Failed to read "{file.filename}" from tar.')
+                    else:
+                        raise
+
+        return core.NeuronList(neurons)
+
+    def read_tar(
+        self, fpath: os.PathLike,
+        parallel="auto",
+        limit: Optional[int] = None,
+        attrs: Optional[Dict[str, Any]] = None,
+        on_error: Union[Literal['ignore', Literal['raise']]] = 'ignore'
+    ) -> 'core.NeuronList':
+        """Read files from a tar archive into a NeuronList.
+
+        This is a dispatcher for `.read_from_tar`.
+
+        Parameters
+        ----------
+        fpath :     str | os.PathLike
+                    Path to tar file.
+        limit :     int, optional
+                    Limit the number of files read from this directory.
+        attrs :     dict or None
+                    Arbitrary attributes to include in the TreeNeuron.
+        on_error :  'ignore' | 'raise'
+                    What do do when error is encountered.
+
+        Returns
+        -------
+        core.NeuronList
+
+        """
+        fpath = Path(fpath).expanduser()
+        read_fn = partial(self.read_from_tar,
+                          tarpath=fpath, attrs=attrs,
+                          on_error=on_error)
+        neurons = parallel_read_archive(read_fn=read_fn,
+                                        fpath=fpath,
+                                        file_ext=self.is_valid_file,
+                                        limit=limit,
+                                        parallel=parallel)
+        return core.NeuronList(neurons)
+
     def read_directory(
         self, path: os.PathLike,
         include_subdirs=DEFAULT_INCLUDE_SUBDIRS,
         parallel="auto",
         limit: Optional[int] = None,
         attrs: Optional[Dict[str, Any]] = None
     ) -> 'core.NeuronList':
@@ -458,20 +546,29 @@
         attrs :     dict or None
                     Arbitrary attributes to include in the neuron.
 
         Returns
         -------
         core.BaseNeuron
         """
-        with requests.get(url, stream=True) as r:
+        # Note: originally, we used stream=True and passed `r.raw` to the
+        # read_buffer function but that caused issue when there was more
+        # than one chunk which would require us to concatenate the chunks
+        # `via r.raw.iter_content()`.
+        # Instead, we will simply read the whole content, wrap it in a BytesIO
+        # and pass that to the read_buffer function. This is not ideal as it
+        # will load the whole file into memory while the streaming solution
+        # may have raised an exception earlier if the file was corrupted or
+        # the wrong format.
+        with requests.get(url, stream=False) as r:
             r.raise_for_status()
             props = self.parse_filename(url.split('/')[-1])
             props['origin'] = url
             return self.read_buffer(
-                r.raw,
+                io.BytesIO(r.content),
                 merge_dicts(props, attrs)
             )
 
     def read_string(
         self, s: str, attrs: Optional[Dict[str, Any]] = None
     ) -> 'core.BaseNeuron':
         """Read single string into a Neuron.
@@ -553,14 +650,16 @@
         if hasattr(obj, "read"):
             return self.read_buffer(obj, attrs)
         if isinstance(obj, pd.DataFrame):
             return self.read_dataframe(obj, attrs)
         if isinstance(obj, os.PathLike):
             if str(obj).endswith('.zip'):
                 return self.read_zip(obj, attrs=attrs)
+            elif ".tar" in str(obj):
+                return self.read_tar(obj, attrs=attrs)
             return self.read_file_path(obj, attrs)
         if isinstance(obj, str):
             # See if this might be a file (make sure to expand user)
             if os.path.isfile(os.path.expanduser(obj)):
                 p = Path(obj).expanduser()
                 if p.suffix == '.zip':
                     return self.read_zip(p, attrs=attrs)
@@ -661,17 +760,18 @@
                         obj, include_subdirs, parallel, limit, attrs
                     )
             except TypeError:
                 pass
             try:
                 if os.path.isfile(os.path.expanduser(obj)) and str(obj).endswith('.zip'):
                     return self.read_zip(obj, parallel, limit, attrs)
+                if os.path.isfile(os.path.expanduser(obj)) and ".tar" in str(obj):
+                    return self.read_tar(obj, parallel, limit, attrs)
             except TypeError:
                 pass
-
             return self.read_any_single(obj, attrs)
 
     def parse_filename(
         self, filename: str
     ) -> dict:
         """Extract properties from filename according to specified formatter.
 
@@ -803,19 +903,19 @@
             neurons = list(prog(results))
     else:
         neurons = [read_fn(obj) for obj in prog(objs)]
 
     return neurons
 
 
-def parallel_read_zip(read_fn, fpath, file_ext,
+def parallel_read_archive(read_fn, fpath, file_ext,
                       limit=None,
                       parallel="auto",
                       ignore_hidden=True) -> List['core.NeuronList']:
-    """Read neurons from a ZIP file, potentially in parallel.
+    """Read neurons from a archive (zip or tar), potentially in parallel.
 
     Reader function must be picklable.
 
     Parameters
     ----------
     read_fn :       Callable
     fpath :         str | Path
@@ -842,31 +942,54 @@
     -------
     core.NeuronList
 
     """
     # Check zip content
     p = Path(fpath)
     to_read = []
-    with ZipFile(p, 'r') as zip:
-        for file in zip.filelist:
-            fname = file.filename.split('/')[-1]
-            if ignore_hidden and fname.startswith('._'):
-                continue
-            if callable(file_ext):
-                if file_ext(file):
+
+    if p.name.endswith('.zip'):
+        with ZipFile(p, 'r') as zip:
+            for i, file in enumerate(zip.filelist):
+                fname = file.filename.split('/')[-1]
+                if ignore_hidden and fname.startswith('._'):
+                    continue
+                if callable(file_ext):
+                    if file_ext(file):
+                        to_read.append(file)
+                elif file_ext == '*':
+                    to_read.append(file)
+                elif file_ext and fname.endswith(file_ext):
+                    to_read.append(file)
+                elif '.' not in file.filename:
                     to_read.append(file)
-            elif file_ext == '*':
-                to_read.append(file)
-            elif file_ext and fname.endswith(file_ext):
-                to_read.append(file)
-            elif '.' not in file.filename:
-                to_read.append(file)
 
-    if limit:
-        to_read = to_read[:limit]
+                if isinstance(limit, int) and i >= limit:
+                    break
+    elif '.tar' in p.name:  # can be ".tar", "tar.gz" or "tar.bz"
+        with tarfile.open(p, 'r') as tf:
+            for i, file in enumerate(tf):
+                fname = file.name.split('/')[-1]
+                if ignore_hidden and fname.startswith('._'):
+                    continue
+                if callable(file_ext):
+                    if file_ext(file):
+                        to_read.append(file)
+                elif file_ext == '*':
+                    to_read.append(file)
+                elif file_ext and fname.endswith(file_ext):
+                    to_read.append(file)
+                elif '.' not in file.filename:
+                    to_read.append(file)
+
+                if isinstance(limit, int) and i >= limit:
+                    break
+
+    if isinstance(limit, list):
+        to_read = [f for f in to_read if f in limit]
 
     prog = partial(
         config.tqdm,
         desc='Importing',
         total=len(to_read),
         disable=config.pbar_hide,
         leave=config.pbar_leave
```

### Comparing `navis-1.5.0/navis/io/hdf_io.py` & `navis-1.6.0/navis/io/hdf_io.py`

 * *Files identical despite different names*

### Comparing `navis-1.5.0/navis/io/json_io.py` & `navis-1.6.0/navis/io/json_io.py`

 * *Files identical despite different names*

### Comparing `navis-1.5.0/navis/io/mesh_io.py` & `navis-1.6.0/navis/io/mesh_io.py`

 * *Files identical despite different names*

### Comparing `navis-1.5.0/navis/io/nrrd_io.py` & `navis-1.6.0/navis/io/nrrd_io.py`

 * *Files identical despite different names*

### Comparing `navis-1.5.0/navis/io/precomputed_io.py` & `navis-1.6.0/navis/io/precomputed_io.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,20 +12,22 @@
 #    GNU General Public License for more details.
 
 import io
 import json
 import os
 import struct
 import tempfile
+import requests
 
 import numpy as np
 import pandas as pd
 
 from pathlib import Path
-from typing import Union, Dict, Optional, Any, IO
+from functools import lru_cache
+from typing import Union, Dict, Optional, Any, IO, List
 from typing_extensions import Literal
 from zipfile import ZipFile, ZipInfo
 
 from .. import config, utils, core
 from . import base
 
 try:
@@ -106,15 +108,15 @@
 
 
 class PrecomputedSkeletonReader(PrecomputedReader):
     def __init__(
         self,
         fmt: str = DEFAULT_FMT,
         attrs: Optional[Dict[str, Any]] = None,
-        info: Dict[str, Any] ={}
+        info: Dict[str, Any] = {}
     ):
         super().__init__(fmt=fmt,
                          attrs=attrs,
                          file_ext='',
                          name_fallback='skeleton',
                          read_binary=True)
         self.info = info
@@ -131,27 +133,32 @@
                     Readable buffer - must be bytes.
         attrs :     dict | None
                     Arbitrary attributes to include in the TreeNeuron.
 
         Returns
         -------
         core.TreeNeuron
+
         """
         if not isinstance(f.read(0), bytes):
             raise ValueError(f'Expected bytes, got {type(f.read(0))}')
 
         num_nodes = np.frombuffer(f.read(4), np.uint32)[0]
         num_edges = np.frombuffer(f.read(4), np.uint32)[0]
         nodes = np.frombuffer(f.read(int(3 * 4 * num_nodes)),
                               np.float32).reshape(-1, 3)
         edges = np.frombuffer(f.read(int(2 * 4 * num_edges)),
                               np.uint32).reshape(-1, 2)
 
         swc = self.make_swc(nodes, edges)
 
+        # Check for malformed vertex attributes (should be list of dicts)
+        if isinstance(self.info.get('vertex_attributes', None), dict):
+            self.info['vertex_attributes'] = [self.info['vertex_attributes']]
+
         # Parse additional vertex attributes if specified as per the info file
         for attr in self.info.get('vertex_attributes', []):
             dtype = np.dtype(attr['data_type'])
             n_comp = attr['num_components']
             values = np.frombuffer(f.read(int(n_comp * dtype.itemsize * num_nodes)),
                                    dtype).reshape(-1, n_comp)
             if n_comp == 1:
@@ -179,39 +186,40 @@
         pandas.DataFrame
         """
         swc = pd.DataFrame()
         swc['node_id'] = np.arange(len(nodes))
         swc['x'], swc['y'], swc['z'] = nodes[:, 0], nodes[:, 1], nodes[:, 2]
 
         edge_dict = dict(zip(edges[:, 1], edges[:, 0]))
-        swc['parent_id'] = swc.node_id.map(lambda x: edge_dict.get(x, -1))
+        swc['parent_id'] = swc.node_id.map(lambda x: edge_dict.get(x, -1)).astype(np.int32)
 
         return swc
 
 
 def read_precomputed(f: Union[str, io.BytesIO],
                      datatype: Union[Literal['auto'],
                                      Literal['mesh'],
                                      Literal['skeleton']] = 'auto',
                      include_subdirs: bool = False,
                      fmt: str = '{id}',
                      info: Union[bool, str, dict] = True,
+                     limit: Optional[int] = None,
                      parallel: Union[bool, int] = 'auto',
                      **kwargs) -> 'core.NeuronObject':
     """Read skeletons and meshes from neuroglancer's precomputed format.
 
     Follows the formats specified
     `here <https://github.com/google/neuroglancer/tree/master/src/neuroglancer/datasource/precomputed>`_.
 
     Parameters
     ----------
     f :                 filepath | folder | zip file | bytes
                         Filename, folder or bytes. If folder, will import all
-                        files. If a ``.zip`` archive will read all files in the
-                        file.
+                        files. If a ``.zip``, ``.tar`` or ``.tar.gz`` file will
+                        read all files in the archive. See also ``limit`` parameter.
     datatype :          "auto" | "skeleton" | "mesh"
                         Which data type we expect to read from the files. If
                         "auto", we require a "info" file in the same directory
                         as ``f``.
     include_subdirs :   bool, optional
                         If True and ``f`` is a folder, will also search
                         subdirectories for binary files.
@@ -240,14 +248,19 @@
                         filename. Ignored for DataFrames.
     info :              bool | str | dict
                         An info file describing the data:
                           - ``True`` = will look for `info` file in base folder
                           - ``False`` = do not use/look for `info` file
                           - ``str`` = filepath to `info` file
                           - ``dict`` = already parsed info file
+    limit :             int, optional
+                        If reading from a folder you can use this parameter to
+                        read only the first ``limit`` files. Useful if
+                        wanting to get a sample from a large library of
+                        skeletons/meshes.
     parallel :          "auto" | bool | int
                         Defaults to ``auto`` which means only use parallel
                         processing if more than 200 files are imported. Spawning
                         and joining processes causes overhead and is
                         considerably slower for imports of small numbers of
                         neurons. Integer will be interpreted as the
                         number of cores (otherwise defaults to
@@ -268,60 +281,71 @@
                         Export neurons/volumes to precomputed format.
 
     """
     utils.eval_param(datatype, name='datatype', allowed_values=('skeleton',
                                                                 'mesh',
                                                                 'auto'))
 
-    # Parse data type from info file (if required)
-    if isinstance(f, bytes):
-        if datatype == 'auto':
-            raise ValueError('Unable to infer data type from bytes. Please '
-                             'specify using the `datatype` parameter.')
-        f = io.BytesIO(f)
-    elif datatype == 'auto':
-        f = Path(f).expanduser()
+    # See if we can get the info file from somewhere
+    if info is True and not isinstance(f, bytes):
+        # Find info in zip archive
         if str(f).endswith('.zip'):
-            with ZipFile(f, 'r') as zip:
-                if 'info' not in [f.filename for f in zip.filelist]:
+            with ZipFile(Path(f).expanduser(), 'r') as zip:
+                if 'info' in [f.filename for f in zip.filelist]:
+                    info = json.loads(zip.read('info').decode())
+                elif datatype == 'auto':
                     raise ValueError('No `info` file found in zip file. Please '
                                      'specify data type using the `datatype` '
                                      'parameter.')
-                info = json.loads(zip.read('info').decode())
+        # Try loading info from URL
+        elif utils.is_url(str(f)):
+            base_url = '/'.join(str(f).split('/')[:-1])
+            info = _fetch_info_file(base_url, raise_missing=False)
+        # Try loading info from parent path
         else:
             fp = Path(str(f))
             # Find first existing root
             while not fp.is_dir():
                 fp = fp.parent
             fp = fp / 'info'
-            if not fp.is_file():
-                raise ValueError(f'No `info` file found in {fp.parent}. Please '
-                                 'specify data type using the `datatype` '
-                                 'parameter.')
-            with open(fp, 'r') as info_file:
-                info = json.load(info_file)
-        if not isinstance(info, dict) or '@type' not in info:
-            raise ValueError('`info` file does not contain a `@type` property. '
-                             'Please specify data type using the `datatype` '
-                             'parameter.')
+            if fp.is_file():
+                with open(fp, 'r') as info_file:
+                    info = json.load(info_file)
+
+    # At this point we should have a dictionary - even if it's empty
+    if not isinstance(info, dict):
+        info = {}
+
+    # Parse data type from info file (if required)
+    if datatype == 'auto':
+        if '@type' not in info:
+            raise ValueError('Either no `info` file found or it does not specify '
+                             'a data type. Please provide data type using the '
+                             '`datatype` parameter.')
 
-        if info['@type'] == 'neuroglancer_legacy_mesh':
+        if info.get('@type', None) == 'neuroglancer_legacy_mesh':
             datatype = 'mesh'
-        elif info['@type'] == 'neuroglancer_skeletons':
+        elif info.get('@type', None) == 'neuroglancer_skeletons':
             datatype = 'skeleton'
         else:
             raise ValueError('Data type specified in `info` file unknown: '
-                             f'{info["@type"]}.')
+                             f'{info.get("@type", None)}. Please provide data '
+                             'type using the `datatype` parameter.')
+
+    if isinstance(f, bytes):
+        f = io.BytesIO(f)
 
     if datatype == 'skeleton':
-        reader = PrecomputedSkeletonReader(fmt=fmt, attrs=kwargs)
+        if not isinstance(info, dict):
+            info = {}
+        reader = PrecomputedSkeletonReader(fmt=fmt, attrs=kwargs, info=info)
     else:
         reader = PrecomputedMeshReader(fmt=fmt, attrs=kwargs)
 
-    return reader.read_any(f, include_subdirs, parallel)
+    return reader.read_any(f, include_subdirs, parallel, limit=limit)
 
 
 class PrecomputedWriter(base.Writer):
     """Writer class that also takes care of `info` files."""
 
     def write_any(self, x, filepath, write_info=True, **kwargs):
         """Write any to file. Default entry point."""
@@ -329,17 +353,17 @@
         kwargs['write_info'] = False
         super().write_any(x, filepath=filepath, **kwargs)
 
         # Write info file to the correct directory/zipfile
         if write_info:
             add_props = {}
             if kwargs.get('radius', False):
-                add_props['vertex_attributes'] = {'id': 'radius',
+                add_props['vertex_attributes'] = [{'id': 'radius',
                                                   'data_type': 'float32',
-                                                  'num_components': 1}
+                                                  'num_components': 1}]
 
             if str(self.path).endswith('.zip'):
                 with ZipFile(self.path, mode='a') as zf:
                     # Context-manager will remove temporary directory and its contents
                     with tempfile.TemporaryDirectory() as tempdir:
                         # Write info to zip
                         if write_info:
@@ -557,7 +581,27 @@
         result.write(x.nodes.radius.values.astype('float32').tobytes())
 
     if filename:
         with open(filename, 'wb') as f:
             f.write(result.getvalue())
     else:
         return result.getvalue()
+
+
+@lru_cache
+def _fetch_info_file(base_url, raise_missing=True):
+    """Try and fetch `info` file for given base url."""
+    if not base_url.endswith('/'):
+        base_url += '/'
+    r = requests.get(f'{base_url}info')
+
+    try:
+        r.raise_for_status()
+    except requests.HTTPError:
+        if raise_missing:
+            raise
+        else:
+            return {}
+    except BaseException:
+        raise
+
+    return r.json()
```

### Comparing `navis-1.5.0/navis/io/rda_io.py` & `navis-1.6.0/navis/io/rda_io.py`

 * *Files identical despite different names*

### Comparing `navis-1.5.0/navis/io/swc_io.py` & `navis-1.6.0/navis/io/swc_io.py`

 * *Files 5% similar despite different names*

```diff
@@ -267,15 +267,16 @@
     `here <http://www.neuronland.org/NLMorphologyConverter/MorphologyFormats/SWC/Spec.html>`_
 
     Parameters
     ----------
     f :                 str | pandas.DataFrame | iterable
                         Filename, folder, SWC string, URL or DataFrame.
                         If folder, will import all ``.swc`` files. If a
-                        ``.zip`` file will read all SWC files in the file.
+                        ``.zip``, ``.tar`` or ``.tar.gz`` file will read all
+                        SWC files in the file. See also ``limit`` parameter.
     connector_labels :  dict, optional
                         If provided will extract connectors from SWC.
                         Dictionary must map type to label:
                         ``{'presynapse': 7, 'postsynapse': 8}``
     include_subdirs :   bool, optional
                         If True and ``f`` is a folder, will also search
                         subdirectories for ``.swc`` files.
@@ -415,15 +416,15 @@
     """Write TreeNeuron(s) to SWC.
 
     Follows the format specified
     `here <http://www.neuronland.org/NLMorphologyConverter/MorphologyFormats/SWC/Spec.html>`_.
 
     Parameters
     ----------
-    x :                 TreeNeuron | Dotprops | NeuronList
+    x :                 TreeNeuron | NeuronList
                         If multiple neurons, will generate a single SWC file
                         for each neuron (see also ``filepath``).
     filepath :          str | pathlib.Path | list thereof
                         Destination for the SWC files. See examples for options.
                         If ``x`` is multiple neurons, ``filepath`` must either
                         be a folder, a "formattable" filename, a filename ending
                         in `.zip` or a list of filenames (one for each neuron
@@ -504,23 +505,29 @@
     Save multiple neurons to a zip file but modify the filenames:
 
     >>> import navis
     >>> nl = navis.example_neurons(5, kind='skeleton')
     >>> navis.write_swc(nl, tmp_dir / 'skel-{neuron.name}.swc@neuronlist.zip')
 
     """
-    # Make sure inputs are only TreeNeurons or Dotprops
+    # Make sure inputs are only TreeNeurons
     if isinstance(x, core.NeuronList):
         for n in x:
-            if not isinstance(n, (core.TreeNeuron, core.Dotprops)):
-                raise TypeError('Can only write TreeNeurons or Dotprops to SWC '
-                                f', not "{type(n)}"')
-    elif not isinstance(x, (core.TreeNeuron, core.Dotprops)):
-        raise TypeError('Can only write TreeNeurons or Dotprops to SWC, not '
-                        f'"{type(x)}"')
+            if not isinstance(n, core.TreeNeuron):
+                msg = f'Can only write TreeNeurons to SWC, not "{type(n)}"'
+                if isinstance(n, core.Dotprops):
+                    msg += (". For Dotprops, you can use either `navis.write_nrrd`"
+                            " or `navis.write_parquet`.")
+                raise TypeError(msg)
+    elif not isinstance(x, core.TreeNeuron):
+        msg = f'Can only write TreeNeurons to SWC, not "{type(n)}"'
+        if isinstance(n, core.Dotprops):
+            msg += (". For Dotprops, you can use either `navis.write_nrrd`"
+                    " or `navis.write_parquet`.")
+        raise TypeError(msg)
 
     writer = base.Writer(write_func=_write_swc, ext='.swc')
 
     return writer.write_any(x,
                             filepath=filepath,
                             header=header,
                             write_meta=write_meta,
```

### Comparing `navis-1.5.0/navis/io/tiff_io.py` & `navis-1.6.0/navis/io/tiff_io.py`

 * *Files identical despite different names*

### Comparing `navis-1.5.0/navis/matching/__init__.py` & `navis-1.6.0/navis/matching/__init__.py`

 * *Files identical despite different names*

### Comparing `navis-1.5.0/navis/matching/bipartite.py` & `navis-1.6.0/navis/matching/bipartite.py`

 * *Files identical despite different names*

### Comparing `navis-1.5.0/navis/matching/pipeline.py` & `navis-1.6.0/navis/matching/pipeline.py`

 * *Files identical despite different names*

### Comparing `navis-1.5.0/navis/meshes/__init__.py` & `navis-1.6.0/navis/meshes/__init__.py`

 * *Files identical despite different names*

### Comparing `navis-1.5.0/navis/meshes/b3d.py` & `navis-1.6.0/navis/meshes/b3d.py`

 * *Files identical despite different names*

### Comparing `navis-1.5.0/navis/meshes/fqmr.py` & `navis-1.6.0/navis/meshes/fqmr.py`

 * *Files identical despite different names*

### Comparing `navis-1.5.0/navis/meshes/mesh_utils.py` & `navis-1.6.0/navis/meshes/mesh_utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -247,49 +247,59 @@
 
     # Need to fix normals
     mesh.fix_normals()
 
     return mesh
 
 
-def pointlabels_to_meshes(points, labels, res, threshold=0.05, drop_fluff=True,
-                          volume=None, n_cores=os.cpu_count() // 2, progress=True):
+def pointlabels_to_meshes(points, labels, res, method='kde',
+                          threshold=0.05, drop_fluff=True, volume=None,
+                          n_cores=os.cpu_count() // 2, progress=True):
     """Generate non-overlapping meshes from a labelled point cloud.
 
-    Briefly, the workflow is this:
+    Briefly, the default workflow is this:
 
       1. Create a Gaussian KDE for each unique label.
       2. Tile the point's bounding box into voxels of size ``res``.
       3. Calculate the KDE's point density function (PDF) to assign a label to
          each voxel.
       4. (Optional) Denoise the matrix by a round of binary erosion + dilation
          and fill holes.
       5. Use marching cubes to produce a mesh.
 
+    See `method` parameter for an alternative method.
+
     Parameters
     ----------
     points :    (N, 3) array
                 Point cloud.
     labels :    (N, ) array
                 A label for each point.
     res :       int
                 Size of the voxels. Note that this also determines the
                 gap between meshes: higher resolution = smaller, more precise gaps.
+    method :    "kde" | "majority"
+                Which method to use. "kde" (default) uses above described
+                workflow. "majority" vote will simply ask, for each voxel, which
+                labels are contained within it and which is the most numerous.
+                The latter is much faster but may produce coarser meshes - in
+                particular if the number of points is low.
     threshold : float [0-1], optional
                 Threshold for dropping voxels that don't appear to belong to
                 any of the original labels. This is the quantile! I.e. the
                 default value of 0.05 means that we'll be dropping the bottom 5%.
     drop_fluff : bool
                 Whether to drop small bits and pieces from meshes and only keep
                 the largest contiguous pieces.
     volume :    Volume | Trimesh, optional
                 Provide a mesh to contrain the sampled voxels to inside this
                 volume.
     n_cores :   int
-                Number of cores to use for parallel processing.
+                Number of cores to use for parallel processing. Each unique
+                label will be processed on a separate core.
 
 
     Returns
     -------
     meshes  :   list
                 List of ``navis.Volume``. Their names correspond to unique
                 ``labels``.
@@ -299,83 +309,143 @@
         raise ImportError('Meshing requires `skimage`:\n '
                           'pip3 install scikit-image')
 
     if len(points) != len(labels):
         raise ValueError(f'Number of labels ({len(labels)}) must match number '
                          f'of points ({len(points)})')
 
+    assert method in ('kde', 'majority')
+
     points = np.asarray(points)
     labels = np.asarray(labels)
-
-    # For each label create a KDE
-    kde = {}
     labels_unique = np.unique(labels)
-    for l in tqdm(labels_unique,
-                  desc='Generating KDEs',
-                  disable=not progress,
-                  leave=False):
-        this_p = points[labels == l]
 
-        kde[l] = stats.gaussian_kde(this_p.T)
+    if method == 'kde':
+        # Now create voxel coordinates for the volume we want to fill:
+        # First the bounding box
+        bbox = np.vstack((points.min(axis=0), points.max(axis=0)))
+
+        # We'll pad the volume by 2x the resolution
+        padding = res * 2
+
+        xco = np.arange(bbox[0][0] - padding, bbox[1][0] + padding, res)
+        yco = np.arange(bbox[0][1] - padding, bbox[1][1] + padding, res)
+        zco = np.arange(bbox[0][2] - padding, bbox[1][2] + padding, res)
+
+        i = np.arange(0, xco.shape[0], 1)
+        j = np.arange(0, yco.shape[0], 1)
+        k = np.arange(0, zco.shape[0], 1)
+
+        ii, jj, kk = np.meshgrid(i, j, k)
+        xx, yy, zz = np.meshgrid(xco, yco, zco)
+
+        voxels = np.vstack((xx.flatten(), yy.flatten(), zz.flatten())).T
+        voxels = pd.DataFrame(voxels, columns=['x', 'y', 'z'])
+
+        voxels['i'] = ii.flatten()
+        voxels['j'] = jj.flatten()
+        voxels['k'] = kk.flatten()
+
+        if not isinstance(volume, type(None)):
+            in_vol = intersection.in_volume(voxels[['x', 'y', 'z']].values,
+                                            volume)
+            print(f'Dropping {(~in_vol).sum()}/{len(voxels)} voxels outside of provided volume.')
+            voxels = voxels.loc[in_vol].copy()
+
+        # For each label create a KDE
+        kde = {}
+        for l in tqdm(labels_unique,
+                    desc='Generating KDEs',
+                    disable=not progress,
+                    leave=False):
+            this_p = points[labels == l]
+
+            kde[l] = stats.gaussian_kde(this_p.T)
+
+        # For each point get the point density function for each KDE
+        combinations = [(kde[l], [voxels[['x', 'y', 'z']].values.T], {}) for l in kde]
+        with mp.Pool(n_cores) as pool:
+            results = list(tqdm(pool.imap(_worker_wrapper,
+                                        combinations,
+                                        chunksize=1),
+                                leave=False,
+                                disable=not progress,
+                                total=len(combinations),
+                                desc=f'Assigning {len(voxels):,} voxels'))
+
+        # Fill results
+        for l, r in zip(kde, results):
+            voxels[l] = r
+
+        # Drop voxels that have a PDF of less than the given threshold
+        if threshold:
+            pdf = voxels[labels_unique].max(axis=1)
+            keep = pdf >= np.quantile(pdf, threshold)
+            print(f'Dropping {(~keep).sum()}/{len(voxels)} voxels with too low density.')
+            voxels = voxels.loc[keep].copy()
+
+        # Assign label to each voxel based on the max probability
+        voxels['label'] = labels_unique[np.argmax(voxels[labels_unique].values, axis=1)]
+    else:
+        # Turn points into voxels of given size
+        points_vxl = points // res
+
+        # Turn labels into an array of integers
+        labels_dict = dict(zip(labels_unique, np.arange(len(labels_unique))))
+        labels_int = np.array([labels_dict[la] for la in labels])
+
+        # Combine (N, 3) voxels and (N, ) labels into (N, 4) array
+        point_labels = np.hstack((points_vxl, labels_int.reshape(-1, 1)))
+
+        # Count unique voxel + label combinations
+        point_labels_unique, cnt = np.unique(point_labels, axis=0, return_counts=True)
+
+        # For each x/y/z coordinate (but not the label column) get a unique index
+        unique_voxel, voxel_ix = np.unique(
+            point_labels_unique[:, :3], axis=0, return_inverse=True
+        )
+
+        # Turn into DataFrame for tallying up
+        point_labels_df = pd.DataFrame()
+        point_labels_df["voxel_ix"] = voxel_ix
+        point_labels_df["label_ix"] = point_labels_unique[:, -1]
+        point_labels_df["cnt"] = cnt
+
+        # Turn into a N_point x N_labels matrix
+        adj = point_labels_df.groupby(["voxel_ix", "label_ix"]).cnt.sum().unstack()
+
+        # Now generate the DataFrame we will use to create meshes
+        voxels = pd.DataFrame()
+        voxels['i'] = unique_voxel[:, 0]
+        voxels['j'] = unique_voxel[:, 1]
+        voxels['k'] = unique_voxel[:, 2]
+
+        # Also re-generate x/y/z coordinates
+        voxels['x'] = voxels['i'] * res
+        voxels['y'] = voxels['j'] * res
+        voxels['z'] = voxels['k'] * res
+
+        # Make sure i/j/k start at zero (otherwise matrix further down might
+        # end up really huge)
+        voxels['i'] -= unique_voxel[:, 0].min()
+        voxels['j'] -= unique_voxel[:, 1].min()
+        voxels['k'] -= unique_voxel[:, 2].min()
+
+        # For each voxel get the top label...
+        voxels['label'] = labels_unique[np.nanargmax(adj, axis=1)]
+
+        # Drop voxels that have less than given points inside
+        if threshold:
+            top_count = np.nanmax(adj, axis=1)
+            keep = top_count >= np.quantile(top_count, threshold)
+            print(f'Dropping {(~keep).sum()}/{len(voxels)} voxels with too low density.')
+            voxels = voxels.loc[keep].copy()
 
-    # Now create voxel coordinates for the volume we want to fill:
-    # First the bounding box
-    bbox = np.vstack((points.min(axis=0), points.max(axis=0)))
-
-    # We'll pad the volume by 2x the resolution
-    padding = res * 2
-
-    xco = np.arange(bbox[0][0] - padding, bbox[1][0] + padding, res)
-    yco = np.arange(bbox[0][1] - padding, bbox[1][1] + padding, res)
-    zco = np.arange(bbox[0][2] - padding, bbox[1][2] + padding, res)
-
-    i = np.arange(0, xco.shape[0], 1)
-    j = np.arange(0, yco.shape[0], 1)
-    k = np.arange(0, zco.shape[0], 1)
-
-    ii, jj, kk = np.meshgrid(i, j, k)
-    xx, yy, zz = np.meshgrid(xco, yco, zco)
-
-    voxels = np.vstack((xx.flatten(), yy.flatten(), zz.flatten())).T
-    voxels = pd.DataFrame(voxels, columns=['x', 'y', 'z'])
-
-    voxels['i'] = ii.flatten()
-    voxels['j'] = jj.flatten()
-    voxels['k'] = kk.flatten()
-
-    if not isinstance(volume, type(None)):
-        in_vol = intersection.in_volume(voxels[['x', 'y', 'z']].values,
-                                        volume)
-        print(f'Dropping {(~in_vol).sum()}/{len(voxels)} voxels outside of provided volume.')
-        voxels = voxels.loc[in_vol].copy()
-
-    # For each point get the point density function for each KDE
-    combinations = [(kde[l], [voxels[['x', 'y', 'z']].values.T], {}) for l in kde]
-    with mp.Pool(n_cores) as pool:
-        results = list(tqdm(pool.imap(_worker_wrapper,
-                                      combinations,
-                                      chunksize=1),
-                            leave=False,
-                            disable=not progress,
-                            total=len(combinations),
-                            desc='Assigning voxels'))
-
-    # Fill results
-    for l, r in zip(kde, results):
-        voxels[l] = r
-
-    # Drop voxels that have a PDF of less than the given threshold
-    if threshold:
-        pdf = voxels[labels_unique].max(axis=1)
-        keep = pdf >= np.quantile(pdf, threshold)
-        print(f'Dropping {(~keep).sum()}/{len(voxels)} voxels with too low density.')
-        voxels = voxels.loc[keep].copy()
-
-    # Assign label to each voxel based on the max probability
-    voxels['label'] = labels_unique[np.argmax(voxels[labels_unique].values, axis=1)]
+        # Some settings for the meshing
+        padding = 0
 
     meshes = []
     for l in tqdm(labels_unique,
                   desc='Creating meshes',
                   disable=not progress,
                   leave=False):
         # Generate empty matrix
@@ -406,27 +476,30 @@
         # Use marching cubes to create surface model
         # (newer versions of skimage have a "marching cubes" function and
         # the marching_cubes_lewiner is deprecreated)
         marching_cubes = getattr(measure, 'marching_cubes',
                                  getattr(measure, 'marching_cubes_lewiner', None))
         verts, faces, normals, values = marching_cubes(mat.astype(float),
                                                        level=0,
-                                                       allow_degenerate=False, step_size=1)
+                                                       allow_degenerate=False,
+                                                       step_size=1)
 
         # Scale back to original units
         verts *= res
 
         # Add offset
-        offset = voxels[['x', 'y', 'z']].min(axis=0)
+        offset = voxels[['x', 'y', 'z']].min(axis=0).values  # keep .values !
         verts += offset
 
         # Somehow we seem to have introduced an offset
         verts -= padding
         verts += 0.5 * res
-        verts[:, 1] -= 0.5 * res
+
+        if method == 'kde':
+            verts[:, 1] -= 0.5 * res
 
         # Make a trimesh
         new_mesh = tm.Trimesh(vertices=verts, faces=faces, normals=normals)
 
         if drop_fluff:
             # Drop small stuff (anything that makes up less than 10% of the faces)
             cc = tm.graph.connected_components(edges=new_mesh.face_adjacency,
```

### Comparing `navis-1.5.0/navis/meshes/o3d.py` & `navis-1.6.0/navis/meshes/o3d.py`

 * *Files identical despite different names*

### Comparing `navis-1.5.0/navis/meshes/operations.py` & `navis-1.6.0/navis/meshes/operations.py`

 * *Files identical despite different names*

### Comparing `navis-1.5.0/navis/meshes/pyml.py` & `navis-1.6.0/navis/meshes/pyml.py`

 * *Files identical despite different names*

### Comparing `navis-1.5.0/navis/meshes/templates/blender_decimate.py.template` & `navis-1.6.0/navis/meshes/templates/blender_decimate.py.template`

 * *Files identical despite different names*

### Comparing `navis-1.5.0/navis/meshes/templates/blender_smooth.py.template` & `navis-1.6.0/navis/meshes/templates/blender_smooth.py.template`

 * *Files identical despite different names*

### Comparing `navis-1.5.0/navis/models/__init__.py` & `navis-1.6.0/navis/models/__init__.py`

 * *Files identical despite different names*

### Comparing `navis-1.5.0/navis/models/network_models.py` & `navis-1.6.0/navis/models/network_models.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,29 +20,35 @@
 from typing import Iterable, Union, Optional, Callable
 
 from .. import config
 
 # Set up logging
 logger = config.get_logger(__name__)
 
-__all__ = ['BayesianTraversalModel', 'TraversalModel', 'linear_activation_p', 'random_linear_activation_function']
+__all__ = ['BayesianTraversalModel', 'TraversalModel', 'linear_activation_p',
+           'random_linear_activation_function']
 
 
 class BaseNetworkModel:
     """Base model for network simulations."""
 
     def __init__(self, edges: pd.DataFrame, source: str, target: str):
         """Initialize model."""
         assert isinstance(edges, pd.DataFrame), f'edges must be pandas DataFrame, got "{type(edges)}"'
         assert source in edges.columns, f'edges DataFrame must contain "{source}" column'
         assert target in edges.columns, f'edges DataFrame must contain "{target}" column'
         self.edges = edges
         self.source = source
         self.target = target
 
+        if (self.edges.dtypes[source] == object) or (self.edges.dtypes[target] == object):
+            logger.warning('Looks like sources and/or targets in your edge list '
+                           'might be strings? This can massively slow down '
+                           'computations. If at all possible try to use numeric IDs.')
+
     @property
     def n_nodes(self) -> int:
         """Return unique nodes in network."""
         return np.unique(self.edges[[self.source, self.target]].values.flatten()).shape[0]
 
     @property
     def has_results(self) -> bool:
@@ -243,75 +249,95 @@
 
         Use ``.run_parallel`` to use parallel processes.
 
         """
         # For some reason this is required for progress bars in Jupyter to show
         print(' ', end='', flush=True)
         # For faster access, use the raw array
-        edges = self.edges[[self.source, self.target, self.weights]].values
+        # Note: we're splitting the columns in case we have different datatypes
+        # (e.g. int64 for IDs and float for weights)
+        sources = self.edges[self.source].values
+        targets = self.edges[self.target].values
+        weights = self.edges[self.weights].values
 
         # For some reason the progress bar does not show unless we have a print here
-        all_trav = None
+        all_enc_nodes = None
         for it in config.trange(1, iterations + 1,
                                 disable=config.pbar_hide,
                                 leave=config.pbar_leave,
                                 position=kwargs.get('position', 0)):
             # Set seeds as encountered in step 1
-            if not return_iterations:
-                enc = np.array([[1, s] for s in self.seeds])
-            else:
-                enc = np.array([[1, s, it] for s in self.seeds])
+            enc_nodes = self.seeds
+            enc_steps = np.repeat(1, len(self.seeds))
+            if return_iterations:
+                enc_it = np.repeat(it, len(self.seeds))
 
             # Start with all edges
-            this_edges = edges
+            this_weights = weights
+            this_sources = sources
+            this_targets = targets
             for i in range(2, self.max_steps + 1):
                 # Which edges have their presynaptic node already traversed?
-                pre_trav = np.isin(this_edges[:, 0], enc[:, 1])  # 21
+                pre_trav = np.isin(this_sources, enc_nodes)
                 # Among those, which edges have the postsynaptic node traversed?
-                post_trav = np.isin(this_edges[pre_trav, 1], enc[:, 1])  # 63
+                post_trav = np.isin(this_targets[pre_trav], enc_nodes)
 
                 # Combine conditions to find edges where the presynaptic node
                 # has been traversed but not the postsynaptic node
                 pre_not_post = np.where(pre_trav)[0][~post_trav]
-                out_edges = this_edges[pre_not_post]
+                out_targets = this_targets[pre_not_post]
+                out_weights = this_weights[pre_not_post]
 
                 # Drop edges that have already been traversed - speeds up things
                 pre_and_post = np.where(pre_trav)[0][post_trav]
-                this_edges = np.delete(this_edges, pre_and_post, axis=0)
+                this_targets = np.delete(this_targets, pre_and_post, axis=0)
+                this_sources = np.delete(this_sources, pre_and_post, axis=0)
+                this_weights = np.delete(this_weights, pre_and_post, axis=0)
 
                 # Stop if we traversed the entire (reachable) graph
-                if out_edges.size == 0:
+                if out_targets.size == 0:
                     break
 
-                # Collect weights
-                w = out_edges[:, 2]
-
                 # Edges traversed in this round
-                trav_edges = out_edges[self.traversal_func(w)]
+                trav = self.traversal_func(out_weights)
+                if not trav.sum():
+                    continue
+
+                trav_targets = out_targets[trav]
 
                 # Keep track
-                if not trav_edges.size == 0:
-                    new_trav = np.unique(trav_edges[:, 1]).astype(int)
-                    if not return_iterations:
-                        enc = np.concatenate((enc, [[i, b] for b in new_trav]), axis=0)
-                    else:
-                        enc = np.concatenate((enc, [[i, b, it] for b in new_trav]), axis=0)
+                new_trav = np.unique(trav_targets)
+
+                # Store results
+                enc_nodes = np.concatenate((enc_nodes, new_trav))
+                enc_steps = np.concatenate((enc_steps, np.repeat(i, len(new_trav))))
+                if return_iterations:
+                    enc_it = np.concatenate((enc_it, np.repeat(it, len(new_trav))))
 
             # Save this round of traversal
-            if not isinstance(all_trav, np.ndarray):
-                all_trav = enc
+            if all_enc_nodes is None:
+                all_enc_nodes = enc_nodes
+                all_enc_steps = enc_steps
+                if return_iterations:
+                    all_enc_it = enc_it
             else:
-                all_trav = np.concatenate((all_trav, enc), axis=0)
+                all_enc_nodes = np.concatenate((all_enc_nodes, enc_nodes))
+                all_enc_steps = np.concatenate((all_enc_steps, enc_steps))
+                if return_iterations:
+                    all_enc_it = np.concatenate((all_enc_it, enc_it))
 
         self.iterations = iterations
 
-        cols = ['steps', 'node']
+        # Combine results into DataFrame
+        self.results = pd.DataFrame()
+        self.results['steps'] = all_enc_steps
+        self.results['node'] = all_enc_nodes
         if return_iterations:
-            cols += ['iteration']
-        self.results = pd.DataFrame(all_trav, columns=cols).astype(int)
+            self.results['iteration'] = all_enc_it
+
         return self.results
 
 
 class BayesianTraversalModel(TraversalModel):
     """Model for traversing a network starting with given seed nodes.
 
     This model is a Bayes net version of
```

### Comparing `navis-1.5.0/navis/morpho/__init__.py` & `navis-1.6.0/navis/morpho/__init__.py`

 * *Files identical despite different names*

### Comparing `navis-1.5.0/navis/morpho/analyze.py` & `navis-1.6.0/navis/morpho/analyze.py`

 * *Files identical despite different names*

### Comparing `navis-1.5.0/navis/morpho/fq.py` & `navis-1.6.0/navis/morpho/fq.py`

 * *Files 11% similar despite different names*

```diff
@@ -63,15 +63,16 @@
                 be ``np.logspace(start, stop, num)``.
     parallel :  bool
                 Whether to use multiple cores when ``x`` is a NeuronList.
     n_cores :   bool
                 Number of cores to use when ``x`` is a NeuronList and
                 ``parallel=True``. Even on a single core this function makes
                 heavy use of numpy which itself uses multiple threads - it is
-                therefore not
+                therefore not advisable to use all your cores as this would
+                create a bottleneck.
     progress :  bool
                 Whether to show a progress bar.
 
     Returns
     -------
     Fq :        np.ndarray
                 For single neurons: ``(num,)`` array
@@ -83,14 +84,15 @@
     Kiri Choi, Won Kyu Kim, Changbong Hyeon
     bioRxiv 2022.04.07.487455; doi: https://doi.org/10.1101/2022.04.07.487455
 
     Examples
     --------
     >>> import navis
     >>> nl = navis.example_neurons(3)
+    >>> nl = nl.convert_units('microns')
     >>> # Resample to 1 node / micron
     >>> rs = navis.resample_skeleton(nl, '1 micron')
     >>> # Calculate form factor
     >>> Fq = navis.form_factor(rs, start=-3, stop=3, num=301,
     ...                        parallel=True, n_cores=3)
     >>> # Plot
     >>> import matplotlib.pyplot as plt
```

### Comparing `navis-1.5.0/navis/morpho/manipulation.py` & `navis-1.6.0/navis/morpho/manipulation.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,19 +19,23 @@
 import pandas as pd
 import numpy as np
 import networkx as nx
 import trimesh as tm
 
 from collections import namedtuple
 from itertools import combinations
-from scipy.spatial import cKDTree
 from scipy.ndimage import gaussian_filter
 from typing import Union, Optional, Sequence, List, Set
 from typing_extensions import Literal
 
+try:
+    from pykdtree.kdtree import KDTree
+except ImportError:
+    from scipy.spatial import cKDTree as KDTree
+
 from .. import graph, utils, config, core
 from . import mmetrics, subset
 
 # Set up logging
 logger = config.get_logger(__name__)
 
 __all__ = sorted(['prune_by_strahler', 'stitch_skeletons', 'split_axon_dendrite',
@@ -947,15 +951,15 @@
 
         if any(nl.has_connectors):
             x._connectors = pd.concat([n.connectors for n in nl],  # type: ignore  # no stubs for concat
                                       ignore_index=True)
     elif isinstance(nl[0], core.VoxelNeuron):
         raise TypeError('Combining VoxelNeuron not (yet) supported')
     else:
-        raise TypeError(f'Unable to combine {ty}')
+        raise TypeError(f'Unable to combine {type(nl[0])}')
 
     return x
 
 
 def stitch_skeletons(*x: Union[Sequence[NeuronObject], 'core.NeuronList'],
                      method: Union[Literal['LEAFS'],
                                    Literal['ALL'],
@@ -1391,15 +1395,15 @@
     if reverse:
         segs_to_walk += x.segments[::-1]
 
     # For each spike length do -> do this in reverse to correct the long
     # spikes first
     for l in list(range(1, max_spike_length + 1))[::-1]:
         # Go over all segments
-        for seg in x.segments:
+        for seg in segs_to_walk:
             # Get nodes A, B and C of this segment
             this_A = this_nodes.loc[seg[:-l - 1]]
             this_B = this_nodes.loc[seg[l:-1]]
             this_C = this_nodes.loc[seg[l + 1:]]
 
             # Get coordinates
             A = this_A[['x', 'y', 'z']].values
@@ -1592,15 +1596,15 @@
     if not isinstance(x, core.TreeNeuron):
         raise TypeError(f'Can only process TreeNeurons, not {type(x)}')
 
     if not inplace:
         x = x.copy()
 
     # Prepare nodes (add parent_dist for later, set index)
-    mmetrics.parent_dist(x, root_dist=0)
+    # mmetrics.parent_dist(x, root_dist=0)
     nodes = x.nodes.set_index('node_id', inplace=False).copy()
 
     to_smooth = utils.make_iterable(to_smooth)
 
     miss = to_smooth[~np.isin(to_smooth, nodes.columns)]
     if len(miss):
         raise ValueError(f'Column(s) not found in node table: {miss}')
@@ -1906,75 +1910,99 @@
             if len(mask) != len(x.nodes):
                 raise ValueError("Length of boolean mask must match number of "
                                  "nodes in the neuron")
             mask = x.nodes.node_id.values[mask]
 
     g = x.graph.to_undirected()
 
-    # Extract each fragment's rows and construct a KD-Tree
-    Fragment = namedtuple('Fragment', ['frag_id', 'df', 'kd'])
-    fragments = []
-    for frag_id, cc in enumerate(nx.connected_components(g)):
-        if len(cc) == len(g.nodes):
-            # There's only one component -- no healing necessary
-            return x
-
-        # Skip if fragment is smaller than threshold
-        if not isinstance(min_size, type(None)):
-            if len(cc) < min_size:
-                continue
+    # Get connected components
+    cc = list(nx.connected_components(g))
+    if len(cc) == 1:
+        # There's only one component -- no healing necessary
+        return x
+
+    # Turn into a dictionary node -> component
+    cc = {n: i for i, c in enumerate(cc) for n in c}
 
-        df = x.nodes.query('node_id in @cc')
+    # Turn into a Series
+    cc = x.nodes.node_id.map(cc)
 
-        # If mask, drop everything that is masked out
-        if not isinstance(mask, type(None)):
-            df = df[df.node_id.isin(mask)]
-
-        # Filter to leaf nodes if applicable
-        if nodes == 'LEAFS':
-            df = df[df['type'].isin(['end', 'root'])]
-
-        if not df.empty:
-            kd = cKDTree(df[[*'xyz']].values)
-            fragments.append(Fragment(frag_id, df, kd))
+    to_use = x.nodes
+    # Drop fragments smaller than threshold
+    if not isinstance(min_size, type(None)):
+        sizes = cc.value_counts()
+        above = sizes[sizes >= min_size].index
+        to_use = to_use[cc.isin(above)]
+        cc = cc[cc.isin(above)]
+
+    # Filter to leaf nodes if applicable
+    if nodes == 'LEAFS':
+        keep = to_use['type'].isin(['end', 'root'])
+        to_use = to_use[keep]
+        cc = cc[keep]
+
+    # If mask, drop everything that is masked out
+    if not isinstance(mask, type(None)):
+        keep = to_use.node_id.isin(mask)
+        to_use = to_use[keep]
+        cc = cc[keep]
+
+    # Collect fragments
+    Fragment = namedtuple('Fragment', ['frag_id', 'node_ids', 'kd'])
+    fragments = []
+    for frag_id, df in to_use.groupby(cc):
+        kd = KDTree(df[[*'xyz']].values)
+        fragments.append(Fragment(frag_id, df.node_id.values, kd))
 
     # Sort from big-to-small, so the calculations below use a
     # KD tree for the larger point set in every fragment pair.
-    fragments = sorted(fragments, key=lambda frag: -len(frag.df))
+    fragments = sorted(fragments, key=lambda frag: -len(frag.node_ids))
 
     # We could use the full graph and connect all
     # fragment pairs at their nearest neighbors,
     # but it's faster to treat each fragment as a
     # single node and run MST on that quotient graph,
     # which is tiny.
+    # Note to self:
+    # This approach works well if we have a small number of fragments to connect
+    # But with a large number of fragments, the number of comparisons grows
+    # exponentially (len(fragments) ** 2 - len(fragments)) / 2) and we would be
+    # better off running a brute force pairwise distance function on all
+    # relevant nodes and constructing the graph from that.
     frag_graph = nx.Graph()
     for frag_a, frag_b in combinations(fragments, 2):
         coords_b = frag_b.kd.data
-        distances, indexes = frag_a.kd.query(coords_b)
+        if coords_b.ndim == 1:
+            coords_b = coords_b.reshape(-1, 3)
+        distances, indexes = frag_a.kd.query(coords_b, distance_upper_bound=max_dist)
+
+        # Ignore fragments that are too far apart
+        if np.all(np.isinf(distances)):
+            continue
 
         index_b = np.argmin(distances)
         index_a = indexes[index_b]
 
-        node_a = frag_a.df['node_id'].iloc[index_a]
-        node_b = frag_b.df['node_id'].iloc[index_b]
+        node_a = frag_a.node_ids[index_a]
+        node_b = frag_b.node_ids[index_b]
         dist_ab = distances[index_b]
 
         # Add edge from one fragment to another,
         # but keep track of which fine-grained skeleton
         # nodes were used to calculate distance.
         frag_graph.add_edge(frag_a.frag_id, frag_b.frag_id,
                             node_a=node_a, node_b=node_b,
                             distance=dist_ab)
 
     # Compute inter-fragment MST edges
     frag_edges = nx.minimum_spanning_edges(frag_graph, weight='distance', data=True)
 
     # For each inter-fragment edge, add the corresponding
     # fine-grained edge between skeleton nodes in the original graph.
-    to_add = [[e[2]['node_a'], e[2]['node_b']] for e in frag_edges if e[2]['distance'] <= max_dist]
+    to_add = [[e[2]['node_a'], e[2]['node_b']] for e in frag_edges]
     g.add_edges_from(to_add)
 
     # Rewire based on graph
     return graph.rewire_skeleton(x, g, inplace=inplace)
 
 
 @utils.map_neuronlist(desc='Pruning', must_zip=['source'], allow_parallel=True)
```

### Comparing `navis-1.5.0/navis/morpho/mmetrics.py` & `navis-1.6.0/navis/morpho/mmetrics.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -628,25 +628,25 @@
     This is a variation of the algorithm for calculating synapse flow from
     Schneider-Mizell et al. (eLife, 2016).
 
     The way this implementation works is by iterating over each branch point
     and counting the number of pre->post synapse paths that "flow" from one
     child branch to the other(s).
 
-    Parameters
-    ----------
-    x :         TreeNeuron | MeshNeuron | NeuronList
-                Neuron(s) to calculate bending flow for. Must have connectors!
-
     Notes
     -----
     This is algorithm appears to be more reliable than synapse flow
     centrality for identifying the main branch point for neurons that have
     incompletely annotated synapses.
 
+    Parameters
+    ----------
+    x :         TreeNeuron | MeshNeuron | NeuronList
+                Neuron(s) to calculate bending flow for. Must have connectors!
+
     Returns
     -------
     neuron
                 Adds "bending_flow" as column in the node table (for
                 TreeNeurons) or as `.bending_flow` property
                 (for MeshNeurons).
```

### Comparing `navis-1.5.0/navis/morpho/persistence.py` & `navis-1.6.0/navis/morpho/persistence.py`

 * *Files identical despite different names*

### Comparing `navis-1.5.0/navis/morpho/subset.py` & `navis-1.6.0/navis/morpho/subset.py`

 * *Files 1% similar despite different names*

```diff
@@ -277,20 +277,20 @@
     # We won't produce new slabs but roots and leaves might change
     x.nodes.loc[x.nodes.parent_id < 0, 'type'] = 'root'
     x.nodes.loc[(~x.nodes.node_id.isin(x.nodes.parent_id.values)
                  & (x.nodes.parent_id >= 0)), 'type'] = 'end'
 
     # Filter connectors
     if not keep_disc_cn and x.has_connectors:
-        x._connectors = x.connectors[x.connectors.node_id.isin(subset)]
+        x._connectors = x.connectors[x.connectors.node_id.isin(x.nodes.node_id)]
         x._connectors.reset_index(inplace=True, drop=True)
 
     if getattr(x, 'tags', None) is not None:
         # Filter tags
-        x.tags = {t: [tn for tn in x.tags[t] if tn in subset] for t in x.tags}  # type: ignore  # TreeNeuron has no tags
+        x.tags = {t: [tn for tn in x.tags[t] if tn in x.nodes.node_id.values] for t in x.tags}  # type: ignore  # TreeNeuron has no tags
 
         # Remove empty tags
         x.tags = {t: x.tags[t] for t in x.tags if x.tags[t]}  # type: ignore  # TreeNeuron has no tags
 
     # Fix graph representations
     if '_graph_nx' in x.__dict__:
         x._graph_nx = x.graph.subgraph(x.nodes.node_id.values)
```

### Comparing `navis-1.5.0/navis/nbl/__init__.py` & `navis-1.6.0/navis/nbl/__init__.py`

 * *Files identical despite different names*

### Comparing `navis-1.5.0/navis/nbl/ablast_funcs.py` & `navis-1.6.0/navis/nbl/ablast_funcs.py`

 * *Files identical despite different names*

### Comparing `navis-1.5.0/navis/nbl/base.py` & `navis-1.6.0/navis/nbl/base.py`

 * *Files identical despite different names*

### Comparing `navis-1.5.0/navis/nbl/nblast_funcs.py` & `navis-1.6.0/navis/nbl/nblast_funcs.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from functools import partial
 
 import numpy as np
 import pandas as pd
 import multiprocessing as mp
 
 from concurrent.futures import ProcessPoolExecutor, as_completed
-from typing import Callable, Dict, Union, Optional, List
+from typing import Callable, Dict, Union, Optional
 from typing_extensions import Literal
 
 from navis.nbl.smat import Lookup2d, smat_fcwb, _nblast_v1_scoring
 
 from .. import utils, config
 from ..core import NeuronList, Dotprops, make_dotprops
 from .base import Blaster, NestedIndices
@@ -42,19 +42,22 @@
 logger = config.get_logger(__name__)
 
 # This multiplier controls job size for NBLASTs (only relevant for
 # multiprocessing and if progress=True).
 # Larger multiplier = larger job sizes = fewer jobs = slower updates & less overhead
 # Smaller multiplier = smaller job sizes = more jobs = faster updates & more overhead
 JOB_SIZE_MULTIPLIER = 1
+JOB_MAX_TIME_SECONDS = 60 * 30
 
 # This controls how many threads we allow pykdtree to use during multi-core
 # NBLAST
 OMP_NUM_THREADS_LIMIT = 1
 
+ALLOWED_SCORES = ('forward', 'mean', 'min', 'max', 'both')
+
 
 class NBlaster(Blaster):
     """Implements version 2 of the NBLAST algorithm.
 
     Please note that some properties are computed on initialization and
     changing parameters (e.g. ``use_alpha``) at a later stage will mess things
     up!
@@ -363,14 +366,15 @@
                 A more efficient way than ``nblast(query=x, target=x)``.
     :func:`navis.synblast`
                 A synapse-based variant of NBLAST.
 
     """
     utils.eval_param(criterion, name='criterion',
                      allowed_values=("percentile", "score", "N"))
+    utils.eval_param(scores, name='scores', allowed_values=ALLOWED_SCORES)
 
     # We will make a couple tweaks for speed things up if this is
     # an all-by-all NBLAST
     aba = False
     pre_scores = scores
     if isinstance(target, type(None)):
         target = query
@@ -574,15 +578,14 @@
                                         normalized=normalized,
                                         smat=smat,
                                         limit_dist=limit_dist,
                                         dtype=precision,
                                         approx_nn=approx_nn,
                                         progress=progress,
                                         smat_kwargs=smat_kwargs)
-
                         # Add queries and targets
                         for i, ix in enumerate(qix):
                             this.append(query_dps[ix], query_self_hits[ix])
                         for i, ix in enumerate(tix):
                             this.append(target_dps[ix], target_self_hits[ix])
 
                         # Find the pairs to NBLAST in this part of the matrix
@@ -767,14 +770,16 @@
                 A more efficient way than ``nblast(query=x, target=x)``.
     :func:`navis.nblast_smart`
                 A smart(er) NBLAST suited for very large NBLAST.
     :func:`navis.synblast`
                 A synapse-based variant of NBLAST.
 
     """
+    utils.eval_param(scores, name='scores', allowed_values=ALLOWED_SCORES)
+
     if isinstance(target, type(None)):
         target = query
 
     # Make sure we're working on NeuronLists
     query_dps = NeuronList(query)
     target_dps = NeuronList(target)
 
@@ -795,16 +800,19 @@
             # are. Here, we run a quick test and try to extrapolate from there
             n_rows, n_cols = find_batch_partition(query_dps, target_dps,
                                                   T=10 * JOB_SIZE_MULTIPLIER)
         else:
             # If no progress bar needed, we could just split neurons evenly across
             # all available cores but that can lead to one core lagging behind
             # and finishing much later than all the others. To avoid this, we
-            # should probably
-            n_rows, n_cols = find_optimal_partition(n_cores, query_dps, target_dps)
+            # should aim for each batch to finish in a certain amount of time
+            n_rows, n_cols = find_batch_partition(query_dps, target_dps,
+                                                  T=JOB_MAX_TIME_SECONDS)
+            if (n_rows * n_cols) < n_cores:
+                n_rows, n_cols = find_optimal_partition(n_cores, query_dps, target_dps)
     else:
         n_rows = n_cols = 1
 
     # Calculate self-hits once for all neurons
     nb = NBlaster(use_alpha=use_alpha,
                   normalized=normalized,
                   smat=smat,
@@ -1128,44 +1136,83 @@
                     scores.iloc[this.queries_ix, this.targets_ix] = res.values
             else:
                 scores = this.all_by_all()
 
     return scores
 
 
-def find_batch_partition(q, t, T=10):
-    """Find partitions such that each batch takes about `T` seconds."""
+def test_single_query_time(q, t, it=100):
+    """Test average time of a single NBLAST query."""
     # Get a median-sized query and target
     q_ix = np.argsort(q.n_points)[len(q)//2]
     t_ix = np.argsort(t.n_points)[len(t)//2]
 
     # Run a quick single query benchmark
     timings = []
-    for i in range(10):  # Run 10 tests
+    for i in range(it):  # Run N tests
         s = time.time()
         _ = t[t_ix].dist_dots(q[q_ix])  # Dist dot (ignore scoring / normalizing)
         timings.append(time.time() - s)
-    time_per_query = min(timings)  # seconds per medium sized query
+    return np.mean(timings)  # seconds per medium sized query
+
+
+def find_batch_partition(q, t, T=10, n_cores=None):
+    """Find partitions such that each batch takes about `T` seconds.
+
+    Parameters
+    ----------
+    q,t :       NeuronList of Dotprops
+                Query and targets, respectively.
+    T :         int
+                Time (in seconds) to aim for.
+    n_cores :   int, optional
+                Number of cores that will be used. If provided, will try to
+                make sure that (n_rows * n_cols) is a multiple of n_cores by
+                increasing the number of rows (thereby decreasing the time
+                per batch).
+
+    Returns
+    -------
+    n_rows, n_cols
+
+    """
+    # Test a single query
+    time_per_query = test_single_query_time(q, t)
 
     # Number of queries per job such that each job runs in `T` second
     queries_per_batch = T / time_per_query
 
     # Number of neurons per batch
     neurons_per_batch  = max(1, int(np.sqrt(queries_per_batch)))
 
-    n_rows = len(q) // neurons_per_batch
-    n_cols = len(t) // neurons_per_batch
+    n_rows = max(1, len(q) // neurons_per_batch)
+    n_cols = max(1, len(t) // neurons_per_batch)
+
+    if n_cores and ((n_rows * n_cols) > n_cores):
+        while (n_rows * n_cols) % n_cores:
+            n_rows += 1
 
-    return max(1, n_rows), max(1, n_cols)
+    return n_rows, n_cols
 
 
 def find_optimal_partition(N_cores, q, t):
-    """Find an optimal partition for given NBLAST query."""
-    # Find an optimal partition that minimizes the number of neurons
-    # we have to send to each process
+    """Find an optimal partition for given NBLAST query.
+
+    Parameters
+    ----------
+    N_cores :   int
+                Number of available cores.
+    q,t :       NeuronList of Dotprops
+                Query and targets, respectively.
+
+    Returns
+    -------
+    n_rows, n_cols
+
+    """
     neurons_per_query = []
     for n_rows in range(1, N_cores + 1):
         # Skip splits we can't make
         if N_cores % n_rows:
             continue
         if n_rows > len(q):
             continue
```

### Comparing `navis-1.5.0/navis/nbl/score_mats/smat_alpha_fcwb.csv` & `navis-1.6.0/navis/nbl/score_mats/smat_alpha_fcwb.csv`

 * *Files identical despite different names*

### Comparing `navis-1.5.0/navis/nbl/score_mats/smat_fcwb.csv` & `navis-1.6.0/navis/nbl/score_mats/smat_fcwb.csv`

 * *Files identical despite different names*

### Comparing `navis-1.5.0/navis/nbl/smat.py` & `navis-1.6.0/navis/nbl/smat.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,16 @@
 import math
 from collections import defaultdict
 
 import numpy as np
 import pandas as pd
 
 from .. import config
-from ..core import Dotprops
+#from ..core import Dotprops
+from .. import core
 
 logger = logging.getLogger(__name__)
 
 DEFAULT_SEED = 1991
 
 epsilon = sys.float_info.epsilon
 cpu_count = max(1, os.cpu_count() - 1)
@@ -551,27 +552,27 @@
         -------
         LookupNd
         """
         dig, cells = self._build(threads)
         return LookupNd(dig, cells)
 
 
-def dist_dot(q: Dotprops, t: Dotprops):
+def dist_dot(q: 'core.Dotprops', t: 'core.Dotprops'):
     return list(q.dist_dots(t))
 
 
-def dist_dot_alpha(q: Dotprops, t: Dotprops):
+def dist_dot_alpha(q: 'core.Dotprops', t: 'core.Dotprops'):
     dist, dot, alpha = q.dist_dots(t, alpha=True)
     return [dist, dot * np.sqrt(alpha)]
 
 
 class LookupDistDotBuilder(LookupNdBuilder):
     def __init__(
         self,
-        dotprops: Union[List[Dotprops], Mapping[NeuronKey, Dotprops]],
+        dotprops: Union[List['core.Dotprops'], Mapping[NeuronKey, 'core.Dotprops']],
         matching_lists: List[List[NeuronKey]],
         nonmatching_list: Optional[List[NeuronKey]] = None,
         use_alpha: bool = False,
         draw_strat: str = 'batched',
         seed: int = DEFAULT_SEED,
     ):
         f"""Class for building a 2-dimensional score lookup for NBLAST.
```

### Comparing `navis-1.5.0/navis/nbl/synblast_funcs.py` & `navis-1.6.0/navis/nbl/synblast_funcs.py`

 * *Files identical despite different names*

### Comparing `navis-1.5.0/navis/nbl/utils.py` & `navis-1.6.0/navis/nbl/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 from .. import config
 
 logger = config.logger
 
 
 def extract_matches(scores, N=None, threshold=None, percentage=None,
-                    axis=0, distances=False):
+                    axis=0, distances='auto'):
     """Extract top matches from score matrix.
 
     See `N`, `threshold` or `percentage` for the criterion.
 
     Parameters
     ----------
     scores :        pd.DataFrame
@@ -43,17 +43,19 @@
                     E.g. `percentage=0.05` will return all matches within
                     5% of the top match.
     single_cols :   bool
                     If True will return single columns with comma-separated
                     strings for match ID and match score, respectively.
     axis :          0 | 1
                     For which axis to produce matches.
-    distances :     bool
-                    Set to True if input is distances instead of similarities (i.e.
+    distances :     "auto" | bool
+                    Whether `scores` is distances or similarities (i.e. whether
                     we need to look for the lowest instead of the highest values).
+                    "auto" (default) will infer based on the diagonal of the
+                    `scores` matrix. Use boolean to override.
 
     Returns
     -------
     pd.DataFrame
                     Note that the format is slightly different depending on
                     the criterion.
 
@@ -64,15 +66,18 @@
         raise ValueError('Must provide either `N` or `threshold` or '
                          '`percentage` as criterion for match extraction.')
     elif len({N, threshold, percentage}) > 2:
         # We expect {criterion, None}
         raise ValueError('Please provide either `N`, `threshold` or '
                          '`percentage` as criterion for match extraction.')
 
-    # Transposing is easier than dealing with the different axis further down
+    if distances == 'auto':
+        distances = True if most(np.diag(scores.values).round(2) == 0) else False
+
+    # Transposing is easier than dealing with the different axes further down
     if axis == 1:
         scores = scores.T
 
     if N is not None:
         return _extract_matches_n(scores,
                                   N=N,
                                   distances=distances)
@@ -411,7 +416,14 @@
 
     pca = PCA(n_components=n_dim)
     X_new = pca.fit_transform(scores.values)
 
     dist = pdist(X_new, metric=metric)
 
     return pd.DataFrame(1 - squareform(dist), index=scores.index, columns=scores.columns)
+
+
+def most(x, f=.9):
+    """Check if most (as opposed to all) entries are True."""
+    if x.sum() >= (x.shape[0] * f):
+        return True
+    return False
```

### Comparing `navis-1.5.0/navis/plotting/__init__.py` & `navis-1.6.0/navis/plotting/__init__.py`

 * *Files identical despite different names*

### Comparing `navis-1.5.0/navis/plotting/colors.py` & `navis-1.6.0/navis/plotting/colors.py`

 * *Files identical despite different names*

### Comparing `navis-1.5.0/navis/plotting/d.py` & `navis-1.6.0/navis/plotting/d.py`

 * *Files identical despite different names*

### Comparing `navis-1.5.0/navis/plotting/dd.py` & `navis-1.6.0/navis/plotting/dd.py`

 * *Files identical despite different names*

### Comparing `navis-1.5.0/navis/plotting/ddd.py` & `navis-1.6.0/navis/plotting/ddd.py`

 * *Files identical despite different names*

### Comparing `navis-1.5.0/navis/plotting/flat.py` & `navis-1.6.0/navis/plotting/flat.py`

 * *Files identical despite different names*

### Comparing `navis-1.5.0/navis/plotting/k3d/k3d_objects.py` & `navis-1.6.0/navis/plotting/k3d/k3d_objects.py`

 * *Files identical despite different names*

### Comparing `navis-1.5.0/navis/plotting/plot_utils.py` & `navis-1.6.0/navis/plotting/plot_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -261,14 +261,19 @@
     # Compute tangent vectors for each segment
     tangents = np.roll(points, -1, axis=0) - np.roll(points, 1, axis=0)
 
     tangents[0] = points[1] - points[0]
     tangents[-1] = points[-1] - points[-2]
 
     mags = np.sqrt(np.sum(tangents * tangents, axis=1))
+
+    # Make sure we don't have any zeros in `mags` that would mess with the
+    # subdivision ->  we will set those to the smallest possible value
+    mags[mags == 0] = np.finfo(mags.dtype).resolution
+
     tangents /= mags[:, np.newaxis]
 
     # Get initial normal and binormal
     t = np.abs(tangents[0])
 
     smallest = np.argmin(t)
     normal = np.zeros(3)
```

### Comparing `navis-1.5.0/navis/plotting/plotly/graph_objs.py` & `navis-1.6.0/navis/plotting/plotly/graph_objs.py`

 * *Files 0% similar despite different names*

```diff
@@ -346,15 +346,15 @@
                                        hoverinfo=hoverinfo)]
 
     return trace_data
 
 
 def skeleton2plotly(neuron, legendgroup, showlegend, label, color, **kwargs):
     """Convert skeleton (i.e. TreeNeuron) to plotly line plot."""
-    if neuron.nodes.empty:
+    if not hasattr(neuron, 'nodes') or neuron.nodes.empty:
         logger.warning(f'Skipping TreeNeuron w/o nodes: {neuron.label}')
         return []
     elif neuron.nodes.shape[0] == 1:
         logger.warning(f'Skipping single-node TreeNeuron: {neuron.label}')
         return []
 
     coords = segments_to_coords(neuron, neuron.segments)
```

### Comparing `navis-1.5.0/navis/plotting/vispy/viewer.py` & `navis-1.6.0/navis/plotting/vispy/viewer.py`

 * *Files identical despite different names*

### Comparing `navis-1.5.0/navis/plotting/vispy/visuals.py` & `navis-1.6.0/navis/plotting/vispy/visuals.py`

 * *Files identical despite different names*

### Comparing `navis-1.5.0/navis/plotting/vispy/vputils.py` & `navis-1.6.0/navis/plotting/vispy/vputils.py`

 * *Files identical despite different names*

### Comparing `navis-1.5.0/navis/sampling/__init__.py` & `navis-1.6.0/navis/sampling/__init__.py`

 * *Files identical despite different names*

### Comparing `navis-1.5.0/navis/sampling/downsampling.py` & `navis-1.6.0/navis/sampling/downsampling.py`

 * *Files identical despite different names*

### Comparing `navis-1.5.0/navis/sampling/resampling.py` & `navis-1.6.0/navis/sampling/resampling.py`

 * *Files 3% similar despite different names*

```diff
@@ -129,27 +129,26 @@
     # Map units (non-str are just passed through)
     resample_to = x.map_units(resample_to, on_error='raise')
 
     if not inplace:
         x = x.copy()
 
     # Collect some information for later
-    nodes = x.nodes.set_index('node_id', inplace=False)
-    locs = nodes[['x', 'y', 'z']]
-    radii = nodes['radius'].to_dict()
+    locs = dict(zip(x.nodes.node_id.values, x.nodes[['x', 'y', 'z']].values))
+    radii = dict(zip(x.nodes.node_id.values, x.nodes.radius.values))
 
     new_nodes: List = []
     max_tn_id = x.nodes.node_id.max() + 1
 
     errors = 0
 
     # Iterate over segments
     for i, seg in enumerate(x.small_segments):
         # Get coordinates
-        coords = locs.loc[seg].values.astype(float)
+        coords = np.vstack([locs[n] for n in seg])
         # Get radii
         rad = [radii[tn] for tn in seg]
 
         # Vecs between subsequently measured points
         vecs = np.diff(coords.T)
 
         # path: cum distance along points (norm from first to Nth point)
@@ -239,14 +238,15 @@
     # Note that if `._soma` is a soma detection function we can't tell
     # how to deal with it. Ideally the new soma node will
     # be automatically detected but it is possible, for example, that
     # the radii of nodes have changed due to interpolation such that more
     # than one soma is detected now. Also a "label" column in the node
     # table would be lost at this point.
     # We will go for the easy option which is to pin the soma at this point.
+    nodes = x.nodes.set_index('node_id', inplace=False)
     if np.any(getattr(x, 'soma')):
         soma_nodes = utils.make_iterable(x.soma)
         old_pos = nodes.loc[soma_nodes, ['x', 'y', 'z']].values
 
         # Get nearest neighbours
         dist, ix = tree.query(old_pos)
         node_map = dict(zip(soma_nodes, new_nodes.node_id.values[ix]))
```

### Comparing `navis-1.5.0/navis/transforms/__init__.py` & `navis-1.6.0/navis/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `navis-1.5.0/navis/transforms/affine.py` & `navis-1.6.0/navis/transforms/affine.py`

 * *Files identical despite different names*

### Comparing `navis-1.5.0/navis/transforms/align.py` & `navis-1.6.0/navis/transforms/align.py`

 * *Files identical despite different names*

### Comparing `navis-1.5.0/navis/transforms/base.py` & `navis-1.6.0/navis/transforms/base.py`

 * *Files identical despite different names*

### Comparing `navis-1.5.0/navis/transforms/elastix.py` & `navis-1.6.0/navis/transforms/elastix.py`

 * *Files identical despite different names*

### Comparing `navis-1.5.0/navis/transforms/factory.py` & `navis-1.6.0/navis/transforms/factory.py`

 * *Files identical despite different names*

### Comparing `navis-1.5.0/navis/transforms/h5reg.py` & `navis-1.6.0/navis/transforms/h5reg.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,15 +97,15 @@
                 self._level = str(level)
 
                 # Shape of deformation field
                 self.shape = h5[self.level][self.field].shape
 
                 # Data type of deformation field
                 self.dtype = h5[self.level][self.field].dtype
-            elif 'dfield' in h5.keys():
+            elif self.field in h5.keys():
                 # Set level
                 self._level = None
 
                 # Shape of deformation field
                 self.shape = h5[self.field].shape
 
                 # Data type of deformation field
@@ -192,14 +192,18 @@
                            direction=self.direction,
                            level=int(self.level) if self.level else None,
                            cache=self.use_cache,
                            full_ingest=False)
 
     def full_ingest(self):
         """Fully ingest the deformation field."""
+        # Skip if already ingested
+        if getattr(self, '_fully_ingested', False):
+            return
+
         with h5py.File(self.file, 'r') as h5:
             # Read in the entire field
             if self.level:
                 self.cache = h5[self.level][self.field][:, :, :]
             else:
                 self.cache = h5[self.field][:, :, :]
             # Keep a flag of this
```

### Comparing `navis-1.5.0/navis/transforms/h5reg_java.py` & `navis-1.6.0/navis/transforms/h5reg_java.py`

 * *Files identical despite different names*

### Comparing `navis-1.5.0/navis/transforms/moving_least_squares.py` & `navis-1.6.0/navis/transforms/moving_least_squares.py`

 * *Files identical despite different names*

### Comparing `navis-1.5.0/navis/transforms/templates.py` & `navis-1.6.0/navis/transforms/templates.py`

 * *Files 7% similar despite different names*

```diff
@@ -209,15 +209,15 @@
                             Target for forward transform. Ignored for mirror
                             transforms.
         transform_type :    "bridging" | "mirror"
                             Type of transform.
         skip_existing :     bool
                             If True will skip if transform is already in registry.
         weight :            int
-                            Giving a transform a higher weight will make it
+                            Giving a transform a lower weight will make it
                             preferable when plotting bridging sequences.
 
         See Also
         --------
         register_transformfile
                             If you want to register a file instead of an
                             already constructed transform.
@@ -374,25 +374,28 @@
         G.add_edges_from(edges)
 
         return G
 
     def find_bridging_path(self, source: str,
                            target: str,
                            via: Optional[str] = None,
+                           avoid: Optional[str] = None,
                            reciprocal=True) -> tuple:
         """Find bridging path from source to target.
 
         Parameters
         ----------
         source :        str
                         Source from which to transform to ``target``.
         target :        str
                         Target to which to transform to.
-        via :           str, optional
-                        Force a specific intermediate template.
+        via :           str | list thereof, optional
+                        Force specific intermediate template(s).
+        avoid :         str | list thereof, optional
+                        Avoid going through specific intermediate template(s).
         reciprocal :    bool | float
                         If True or float, will add forward and inverse edges for
                         transforms that are invertible. If float, the inverse
                         edges' weights will be scaled by that factor.
 
         Returns
         -------
@@ -420,35 +423,69 @@
         if target not in G.nodes:
             best_match = fw.process.extractOne(target, nodes,
                                                scorer=fw.fuzz.token_sort_ratio)
             raise ValueError(f'Target "{target}" has no known bridging '
                              f'registrations. Did you mean "{best_match[0]}" '
                              'instead?')
 
-        if via and via not in G.nodes:
-            best_match = fw.process.extractOne(via, nodes,
-                                               scorer=fw.fuzz.token_sort_ratio)
-            raise ValueError(f'Via "{via}" has no known bridging '
-                             f'registrations. Did you mean "{best_match[0]}" '
-                             'instead?')
+        if via:
+            via = list(utils.make_iterable(via))  # do not remove the list() here
+            for v in via:
+                if v not in G.nodes:
+                    best_match = fw.process.extractOne(v, nodes,
+                                                       scorer=fw.fuzz.token_sort_ratio)
+                    raise ValueError(f'Via "{v}" has no known bridging '
+                                    f'registrations. Did you mean "{best_match[0]}" '
+                                    'instead?')
+
+        if avoid:
+            avoid = list(utils.make_iterable(avoid))
 
         # This will raise a error message if no path is found
-        if not via:
+        if not via and not avoid:
             try:
                 path = nx.shortest_path(G, source, target, weight='weight')
             except nx.NetworkXNoPath:
                 raise nx.NetworkXNoPath(f'No bridging path connecting {source} '
                                         f'and {target} found.')
         else:
+            # Go through all possible paths and find one that...
+            found_any = False  # track if we found any path
+            found_good = False  # track if we found a path matching the criteria
             for path in nx.all_simple_paths(G, source, target):
-                if via in path:
+                found_any = True
+                # ... has all `via`s...
+                if via and all([v in path for v in via]):
+                    # ... and none of the `avoid``
+                    if avoid:
+                        if not any([v in path for v in avoid]):
+                            found_good = True
+                            break
+                    else:
+                        found_good = True
+                        break
+                # If we only have `avoid`` but no `via`
+                elif avoid and not any([v in path for v in avoid]):
+                    found_good = True
                     break
-            if via not in path:
-                raise nx.NetworkXNoPath(f'No bridging path connecting {source}'
-                                        f'and {target} via {via} found.')
+
+            if not found_any:
+                raise nx.NetworkXNoPath(f'No bridging path connecting {source} '
+                                        f'and {target} found.')
+            elif not found_good:
+                if via and avoid:
+                    raise nx.NetworkXNoPath(f'No bridging path connecting {source}'
+                                            f'and {target} via "{via}" and '
+                                            f'avoiding "{avoid}" found')
+                elif via:
+                    raise nx.NetworkXNoPath(f'No bridging path connecting {source}'
+                                            f'and {target} via "{via}" found.')
+                else:
+                    raise nx.NetworkXNoPath(f'No bridging path connecting {source}'
+                                            f'and {target} avoiding "{avoid}" found.')
 
         # `path` holds the sequence of nodes we are traversing but not which
         # transforms (i.e. edges) to use
         transforms = []
         for n1, n2 in zip(path[:-1], path[1:]):
             this_edges = []
             i = 0
@@ -465,14 +502,115 @@
             # Now find the edge with the highest weight
             # (inverse transforms might have a lower weight)
             this_edges = sorted(this_edges, key=lambda x: x[-1])
             transforms.append(this_edges[-1][0])
 
         return path, transforms
 
+    def find_all_bridging_paths(self, source: str,
+                                target: str,
+                                via: Optional[str] = None,
+                                avoid: Optional[str] = None,
+                                reciprocal: bool = True,
+                                cutoff: int = None) -> tuple:
+        """Find all bridging paths from source to target.
+
+        Parameters
+        ----------
+        source :        str
+                        Source from which to transform to ``target``.
+        target :        str
+                        Target to which to transform to.
+        via :           str | list thereof, optional
+                        Force specific intermediate template(s).
+        avoid :         str | list thereof, optional
+                        Avoid specific intermediate template(s).
+        reciprocal :    bool | float
+                        If True or float, will add forward and inverse edges for
+                        transforms that are invertible. If float, the inverse
+                        edges' weights will be scaled by that factor.
+        cutoff :        int, optional
+                        Depth to stop the search. Only paths of length
+                        <= cutoff are returned.
+
+        Returns
+        -------
+
+        path :          list
+                        Path from source to target: [source, ..., target]
+        transforms :    list
+                        Transforms as [[path_to_transform, inverse], ...]
+
+        """
+        # Generate (or get cached) bridging graph
+        G = self.bridging_graph(reciprocal=reciprocal)
+
+        if len(G) == 0:
+            raise ValueError('No bridging registrations available')
+
+        # Do not remove the conversion to list - fuzzy matching does act up
+        # otherwise
+        nodes = list(G.nodes)
+        if source not in nodes:
+            best_match = fw.process.extractOne(source, nodes,
+                                               scorer=fw.fuzz.token_sort_ratio)
+            raise ValueError(f'Source "{source}" has no known bridging '
+                             f'registrations. Did you mean "{best_match[0]}" '
+                             'instead?')
+        if target not in G.nodes:
+            best_match = fw.process.extractOne(target, nodes,
+                                               scorer=fw.fuzz.token_sort_ratio)
+            raise ValueError(f'Target "{target}" has no known bridging '
+                             f'registrations. Did you mean "{best_match[0]}" '
+                             'instead?')
+
+        if via and via not in G.nodes:
+            best_match = fw.process.extractOne(via, nodes,
+                                               scorer=fw.fuzz.token_sort_ratio)
+            raise ValueError(f'Via "{via}" has no known bridging '
+                             f'registrations. Did you mean "{best_match[0]}" '
+                             'instead?')
+
+        # This will raise a error message if no path is found
+        for path in nx.all_simple_paths(G, source, target, cutoff=cutoff):
+            # Skip paths that don't contain `via`
+            if isinstance(via, str) and (via not in path):
+                continue
+            elif isinstance(via, (list, tuple, np.ndarray)) and not all([v in path for v in via]):
+                continue
+
+            # Skip paths that contain `avoid`
+            if isinstance(avoid, str) and (avoid in path):
+                continue
+            elif isinstance(avoid, (list, tuple, np.ndarray)) and any([v in path for v in avoid]):
+                continue
+
+            # `path` holds the sequence of nodes we are traversing but not which
+            # transforms (i.e. edges) to use
+            transforms = []
+            for n1, n2 in zip(path[:-1], path[1:]):
+                this_edges = []
+                i = 0
+                # First collect all edges between those two nodes
+                # - this is annoyingly complicated with MultiDiGraphs
+                while True:
+                    try:
+                        e = G.edges[(n1, n2, i)]
+                    except KeyError:
+                        break
+                    this_edges.append([e['transform'], e['weight']])
+                    i += 1
+
+                # Now find the edge with the highest weight
+                # (inverse transforms might have a lower weight)
+                this_edges = sorted(this_edges, key=lambda x: x[-1])
+                transforms.append(this_edges[-1][0])
+
+            yield path, transforms
+
     @functools.lru_cache()
     def shortest_bridging_seq(self, source: str, target: str,
                               via: Optional[str] = None,
                               inverse_weight: float = .5) -> tuple:
         """Find shortest bridging sequence to get from source to target.
 
         Parameters
@@ -574,15 +712,15 @@
         # Templates with mirror registrations
         temps_w_mirrors = [t.source for t in self.mirrors]
 
         # Add symmetrical template brains
         temps_w_mirrors += [t.label for t in self.templates if getattr(t, 'symmetrical', False) == True]
 
         if not temps_w_mirrors:
-            raise ValueError(f'No mirror transformations registered')
+            raise ValueError('No mirror transformations registered')
 
         # If this template has a mirror registration:
         if template in temps_w_mirrors:
             return template
 
         # Get bridging graph
         G = self.bridging_graph()
@@ -680,14 +818,15 @@
         plt.legend(lines, labels)
 
 
 def xform_brain(x: Union['core.NeuronObject', 'pd.DataFrame', 'np.ndarray'],
                 source: str,
                 target: str,
                 via: Optional[str] = None,
+                avoid: Optional[str] = None,
                 affine_fallback: bool = True,
                 caching: bool = True,
                 verbose: bool = True) -> Union['core.NeuronObject',
                                                'pd.DataFrame',
                                                'np.ndarray']:
     """Transform 3D data between template brains.
 
@@ -712,17 +851,19 @@
                         Data to transform. Dataframe must contain ``['x', 'y', 'z']``
                         columns. Numpy array must be shape ``(N, 3)``.
     source :            str
                         Source template brain that the data currently is in.
     target :            str
                         Target template brain that the data should be
                         transformed into.
-    via :               str, optional
-                        Optionally set an intermediate template. This can be
+    via :               str | list thereof, optional
+                        Optionally set intermediate template(s). This can be
                         helpful to force a specific transformation sequence.
+    avoid :             str | list thereof, optional
+                        Prohibit going through specific intermediate template(s).
     affine_fallback :   bool
                         In some cases the non-rigid transformation of points
                         can fail - for example if points are outside the
                         deformation field. If that happens, they will be
                         returned as ``NaN``. If ``affine_fallback=True``
                         we will apply only the rigid affine part of the
                         transformation to those points to get as close as
@@ -779,15 +920,15 @@
     if not isinstance(source, str):
         TypeError(f'Expected source of type str, got "{type(source)}"')
 
     if not isinstance(target, str):
         TypeError(f'Expected target of type str, got "{type(target)}"')
 
     # Get the transformation sequence
-    path, transforms = registry.find_bridging_path(source, target, via=via)
+    path, transforms = registry.find_bridging_path(source, target, via=via, avoid=avoid)
 
     if verbose:
         path_str = path[0]
         for p, tr in zip(path[1:], transforms):
             if isinstance(tr, AliasTransform):
                 link = '='
             else:
```

### Comparing `navis-1.5.0/navis/transforms/thinplate.py` & `navis-1.6.0/navis/transforms/thinplate.py`

 * *Files identical despite different names*

### Comparing `navis-1.5.0/navis/transforms/xfm_funcs.py` & `navis-1.6.0/navis/transforms/xfm_funcs.py`

 * *Files 2% similar despite different names*

```diff
@@ -177,15 +177,15 @@
                            'must have at least two nodes/points.')
 
         # Round change -> this rounds to the first non-zero digit
         # change = np.around(change, decimals=-magnitude)
 
         # Map xformed coordinates back
         if isinstance(xf, core.TreeNeuron):
-            xf.nodes.loc[:, ['x', 'y', 'z']] = xyz_xf[:xf.n_nodes]
+            xf.nodes[['x', 'y', 'z']] = xyz_xf[:xf.n_nodes]
             # Fix radius based on our best estimate
             if 'radius' in xf.nodes.columns:
                 xf.nodes['radius'] *= 10**magnitude
         elif isinstance(xf, core.Dotprops):
             xf.points = xyz_xf[:xf.points.shape[0]]
 
             # If this dotprops has a `k`, set tangent vectors and alpha to
@@ -198,15 +198,15 @@
                 vect = xf.points - hp
                 vect = vect / np.linalg.norm(vect, axis=1).reshape(-1, 1)
                 xf._vect = vect
         elif isinstance(xf, core.MeshNeuron):
             xf.vertices = xyz_xf[:xf.vertices.shape[0]]
 
         if xf.has_connectors:
-            xf.connectors.loc[:, ['x', 'y', 'z']] = xyz_xf[-xf.connectors.shape[0]:]
+            xf.connectors[['x', 'y', 'z']] = xyz_xf[-xf.connectors.shape[0]:]
 
         # Make an educated guess as to whether the units have changed
         if hasattr(xf, 'units') and magnitude != 0:
             if isinstance(xf.units, (config.ureg.Unit, config.ureg.Quantity)):
                 xf.units = (xf.units / 10**magnitude).to_compact()
 
         # Fix soma radius if applicable
@@ -214,17 +214,17 @@
             xf.soma_radius *= 10**magnitude
 
         return xf
     elif isinstance(x, pd.DataFrame):
         if any([c not in x.columns for c in ['x', 'y', 'z']]):
             raise ValueError('DataFrame must have x, y and z columns.')
         x = x.copy()
-        x.loc[:, ['x', 'y', 'z']] = xform(x[['x', 'y', 'z']].values,
-                                          transform=transform,
-                                          affine_fallback=affine_fallback)
+        x[['x', 'y', 'z']] = xform(x[['x', 'y', 'z']].values,
+                                   transform=transform,
+                                   affine_fallback=affine_fallback)
         return x
     elif isinstance(x, tm.Trimesh):
         x = x.copy()
         x.vertices = xform(x.vertices,
                            transform=transform,
                            affine_fallback=affine_fallback)
         return x
@@ -313,40 +313,47 @@
     spacing :       (3, ) tuple
                     The voxel dimensions.
     """
     # Parameters must be hashable for cache - hence no arrays
     # Here, we convert bbox back to arrays
     bbox = np.array(bbox).reshape(3, 2)
 
+    # We could just use the two points of the source's bounding box to calculate
+    # the target's bounding box. However, this can yield incorrect results.
+    # It's better to sample a couple more points on the surface of the source's
+    # bounding box
+    b = tm.primitives.Box(extents=bbox[:, 1] - bbox[:, 0]).to_mesh()
+    b.vertices += bbox.mean(axis=1)
+    b = b.subdivide().vertices  # Subdivide to get more points on the surface
+
     # Temporarily ignore warnings
     current_level = int(logger.level)
     try:
         logger.setLevel('ERROR')
-        # First transform the bounding box. We are doing this in two steps (one for
-        # each point) to avoid caching large volumes
-        mn = xform(bbox[:, :1].T, transform=transform, affine_fallback=True)
-        mx = xform(bbox[:, 1:].T, transform=transform, affine_fallback=True)
-        bbox_xf = np.vstack((mn, mx)).T
+        # Transform points individually to avoid caching the entire volume
+        b_xf = np.vstack([transform.xform(p.reshape(-1, 3), affine_fallback=True) for p in b])
+        bbox_xf = np.vstack([np.min(b_xf, axis=0), np.max(b_xf, axis=0)]).T
     except BaseException:
         raise
     finally:
         logger.setLevel(current_level)
 
     # Next: generate a voxel grid in the target space of the same shape as
     # our input grid
-    target_voxel_size = (bbox_xf[:, 1] - bbox_xf[:, 0]) / shape
+    target_voxel_size = np.abs((bbox_xf[:, 1] - bbox_xf[:, 0]) / shape)
 
     # Generate a grid of xyz coordinates
     XX, YY, ZZ = np.meshgrid(range(shape[0]),
                              range(shape[1]),
                              range(shape[2]),
                              indexing='ij')
     # Coordinate grid has, for each voxel, in the (M, N, K) voxel grid an xyz
     # index coordinate -> hence shape is (3, M, N, K)
     ix_grid = np.array([XX, YY, ZZ])
+
     # Potential idea:
     # - generate a downsampled grid and upsample by interpolation later
     #   -> tried that but the interpolation during upsampling is just as
     #      expensive as transforming all points from the get-go
     # - or process in bocks which allows to skip blocks that are entirely empty
 
     # Convert grid into (N * N * K, 3) voxel array
```

### Comparing `navis-1.5.0/navis/utils/__init__.py` & `navis-1.6.0/navis/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `navis-1.5.0/navis/utils/cv.py` & `navis-1.6.0/navis/utils/cv.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 #    (at your option) any later version.
 #
 #    This program is distributed in the hope that it will be useful,
 #    but WITHOUT ANY WARRANTY; without even the implied warranty of
 #    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #    GNU General Public License for more details.
 
+import uuid
 import functools
 
 from .. import config, core, io
 
 # Set up logging
 logger = config.get_logger(__name__)
 
@@ -28,23 +29,27 @@
 
     Examples
     --------
     >>> import navis
     >>> import cloudvolume as cv
     >>> # Monkey patch cloudvolume
     >>> navis.patch_cloudvolume()
-    >>> # Connect to the public microns dataset
-    >>> vol = cv.CloudVolume('precomputed://gs://iarpa_microns/minnie/minnie65/seg',
-    ...                      use_https=True)
+    >>> # Connect to the Google segmentation of FAFB
+    >>> vol = cv.CloudVolume('precomputed://gs://fafb-ffn1-20200412/segmentation',
+    ...                       use_https=True,
+    ...                       progress=False)
+    >>> ids = [2137190164, 2268989790]
     >>> # Fetch as navis neuron using newly added method or ...
-    >>> nl = vol.mesh.get_navis(864691135293126156, lod=3)
+    >>> nl = vol.mesh.get_navis(ids, lod=3)
     >>> # ... alternatively use `as_navis` keyword argument in original method
-    >>> nl = vol.mesh.get(864691135293126156, lod=3, as_navis=True)
+    >>> nl = vol.mesh.get(ids, lod=3, as_navis=True)
     >>> type(nl)
     <class 'navis.core.neuronlist.NeuronList'>
+    >>> # The same works for skeletons
+    >>> skels = vol.skeleton.get_navis(ids)
 
     """
     global cv
     try:
         import cloudvolume as cv
     except ImportError:
         cv = None
@@ -83,18 +88,18 @@
     @functools.wraps(func)
     def wrapper(*args, **kwargs):
         ret_navis = kwargs.pop('as_navis', False)
         res = func(*args, **kwargs)
 
         if not only_on_kwarg or ret_navis:
             neurons = []
-            if isinstance(res, list):
-                res = {getattr(n, 'id', 'NA'): n for n in res}
+            if isinstance(res, (list, tuple)):
+                res = {getattr(n, "id", uuid.uuid4()): n for n in res}
             if isinstance(res, (cv.Mesh, cv.Skeleton)):
-                res = {getattr(res, 'id', 'NA'): res}
+                res = {getattr(res, "id", uuid.uuid4()): res}
 
             for k, v in res.items():
                 if isinstance(v, cv.Mesh):
                     n = core.MeshNeuron(v, id=k, units='nm')
                     neurons.append(n)
                 elif isinstance(v, cv.Skeleton):
                     swc_str = v.to_swc()
```

### Comparing `navis-1.5.0/navis/utils/decorators.py` & `navis-1.6.0/navis/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `navis-1.5.0/navis/utils/eval.py` & `navis-1.6.0/navis/utils/eval.py`

 * *Files identical despite different names*

### Comparing `navis-1.5.0/navis/utils/exceptions.py` & `navis-1.6.0/navis/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `navis-1.5.0/navis/utils/iterables.py` & `navis-1.6.0/navis/utils/iterables.py`

 * *Files identical despite different names*

### Comparing `navis-1.5.0/navis/utils/misc.py` & `navis-1.6.0/navis/utils/misc.py`

 * *Files identical despite different names*

### Comparing `navis-1.5.0/navis/utils/validate.py` & `navis-1.6.0/navis/utils/validate.py`

 * *Files identical despite different names*

### Comparing `navis-1.5.0/navis.egg-info/SOURCES.txt` & `navis-1.6.0/navis.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 navis.egg-info/PKG-INFO
 navis.egg-info/SOURCES.txt
 navis.egg-info/dependency_links.txt
 navis.egg-info/not-zip-safe
 navis.egg-info/requires.txt
 navis.egg-info/top_level.txt
 navis/connectivity/__init__.py
+navis/connectivity/adjacency.py
 navis/connectivity/cnmetrics.py
 navis/connectivity/matrix_utils.py
 navis/connectivity/predict.py
 navis/connectivity/similarity.py
 navis/conversion/__init__.py
 navis/conversion/converters.py
 navis/conversion/meshing.py
@@ -83,14 +84,15 @@
 navis/io/__init__.py
 navis/io/base.py
 navis/io/hdf_io.py
 navis/io/json_io.py
 navis/io/mesh_io.py
 navis/io/nmx_io.py
 navis/io/nrrd_io.py
+navis/io/pq_io.py
 navis/io/precomputed_io.py
 navis/io/rda_io.py
 navis/io/swc_io.py
 navis/io/tiff_io.py
 navis/matching/__init__.py
 navis/matching/bipartite.py
 navis/matching/pipeline.py
@@ -145,24 +147,26 @@
 navis/transforms/align.py
 navis/transforms/base.py
 navis/transforms/cmtk.py
 navis/transforms/elastix.py
 navis/transforms/factory.py
 navis/transforms/h5reg.py
 navis/transforms/h5reg_java.py
+navis/transforms/images.py
 navis/transforms/moving_least_squares.py
 navis/transforms/templates.py
 navis/transforms/thinplate.py
 navis/transforms/xfm_funcs.py
 navis/utils/__init__.py
 navis/utils/cv.py
 navis/utils/decorators.py
 navis/utils/eval.py
 navis/utils/exceptions.py
 navis/utils/iterables.py
 navis/utils/misc.py
 navis/utils/validate.py
+tests/test_connectivity.py
 tests/test_io.py
 tests/test_neurons.py
 tests/test_notebooks.py
 tests/test_parallel.py
 tests/test_transforms.py
```

### Comparing `navis-1.5.0/navis.egg-info/requires.txt` & `navis-1.6.0/navis.egg-info/requires.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 h5py>=3.1
-matplotlib>=3.3
+matplotlib>=3.6
 morphops>=0.1.11
 ncollpyde>=0.18
 networkx>=2.4
 numpy>=1.16
 pandas>=1.0
 pint>=0.10
 plotly>=4.9
 pynrrd>=0.4.2
 pypng>=0.0.18
 requests>=2.20
 seaborn>=0.10
-setuptools>=50.6
+setuptools>=65.5.1
 scipy>=1.5
 six>=1.11
 tqdm>=4.45
 typing-extensions>=3.7.4
 trimesh>=3.8
 fuzzywuzzy>=0.18
 molesq>=0.2.0
```

### Comparing `navis-1.5.0/setup.py` & `navis-1.6.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -62,21 +62,22 @@
 
         'Intended Audience :: Science/Research',
         'Topic :: Scientific/Engineering :: Bio-Informatics',
 
         'License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)',
 
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
+        # 'Programming Language :: Python :: 3.12',
     ],
     install_requires=install_requires,
     extras_require=dict(extras_require),
     tests_require=extras_require["dev"],
     # CI runs against >=3.8
-    python_requires='>=3.8',
+    python_requires='>=3.9,<4.0',
     zip_safe=False,
 
     include_package_data=True
 
 )
```

### Comparing `navis-1.5.0/tests/test_io.py` & `navis-1.6.0/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `navis-1.5.0/tests/test_neurons.py` & `navis-1.6.0/tests/test_neurons.py`

 * *Files identical despite different names*

### Comparing `navis-1.5.0/tests/test_notebooks.py` & `navis-1.6.0/tests/test_notebooks.py`

 * *Files identical despite different names*

### Comparing `navis-1.5.0/tests/test_parallel.py` & `navis-1.6.0/tests/test_parallel.py`

 * *Files identical despite different names*

### Comparing `navis-1.5.0/tests/test_transforms.py` & `navis-1.6.0/tests/test_transforms.py`

 * *Files identical despite different names*

