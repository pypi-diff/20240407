# Comparing `tmp/gdpx-0.0.5.tar.gz` & `tmp/gdpx-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gdpx-0.0.5.tar", last modified: Sun Mar 17 21:31:33 2024, max compression
+gzip compressed data, was "gdpx-0.0.6.tar", last modified: Sun Apr  7 20:51:53 2024, max compression
```

## Comparing `gdpx-0.0.5.tar` & `gdpx-0.0.6.tar`

### file list

```diff
@@ -1,283 +1,299 @@
-drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-03-17 21:31:33.531270 gdpx-0.0.5/
--rw-r--r--   0 jx1279   (353055) chem     (30004)    35149 2023-04-10 18:29:40.000000 gdpx-0.0.5/LICENSE
--rw-r--r--   0 jx1279   (353055) chem     (30004)    47663 2024-03-17 21:31:33.531270 gdpx-0.0.5/PKG-INFO
--rw-r--r--   0 jx1279   (353055) chem     (30004)     6294 2023-12-12 17:08:13.000000 gdpx-0.0.5/README.md
--rw-r--r--   0 jx1279   (353055) chem     (30004)      899 2024-03-17 21:31:28.000000 gdpx-0.0.5/pyproject.toml
--rw-r--r--   0 jx1279   (353055) chem     (30004)       38 2024-03-17 21:31:33.531270 gdpx-0.0.5/setup.cfg
-drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-03-17 21:31:33.422271 gdpx-0.0.5/src/
-drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-03-17 21:31:33.431271 gdpx-0.0.5/src/gdpx/
-drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-03-17 21:31:33.437271 gdpx-0.0.5/src/gdpx/bias/
--rw-r--r--   0 jx1279   (353055) chem     (30004)      543 2024-03-02 03:59:21.000000 gdpx-0.0.5/src/gdpx/bias/__init__.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     3140 2024-02-14 21:26:12.000000 gdpx-0.0.5/src/gdpx/bias/afir.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     1679 2024-03-02 03:59:21.000000 gdpx-0.0.5/src/gdpx/bias/bias.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     3071 2024-03-17 21:29:07.000000 gdpx-0.0.5/src/gdpx/bias/gaussian.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     2866 2024-03-02 03:59:21.000000 gdpx-0.0.5/src/gdpx/bias/harmonic.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     1209 2023-12-01 19:22:44.000000 gdpx-0.0.5/src/gdpx/bias/nuclei.py
-drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-03-17 21:31:33.449271 gdpx-0.0.5/src/gdpx/builder/
--rw-r--r--   0 jx1279   (353055) chem     (30004)     2881 2024-03-17 21:29:29.000000 gdpx-0.0.5/src/gdpx/builder/__init__.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     3100 2024-03-17 21:29:29.000000 gdpx-0.0.5/src/gdpx/builder/builder.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)      800 2023-12-03 04:28:22.000000 gdpx-0.0.5/src/gdpx/builder/cleave_group.py
--rwxr-xr-x   0 jx1279   (353055) chem     (30004)     2659 2023-12-03 04:22:10.000000 gdpx-0.0.5/src/gdpx/builder/cleave_surface.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     5743 2023-12-01 19:22:44.000000 gdpx-0.0.5/src/gdpx/builder/constraints.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)      384 2023-12-01 19:22:44.000000 gdpx-0.0.5/src/gdpx/builder/crossover.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     1469 2023-12-01 19:22:44.000000 gdpx-0.0.5/src/gdpx/builder/dimer.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     7451 2023-12-01 19:22:44.000000 gdpx-0.0.5/src/gdpx/builder/direct.py
-drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-03-17 21:31:33.451271 gdpx-0.0.5/src/gdpx/builder/graph/
--rw-r--r--   0 jx1279   (353055) chem     (30004)      287 2023-12-01 19:22:44.000000 gdpx-0.0.5/src/gdpx/builder/graph/__init__.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     5942 2024-03-17 21:29:29.000000 gdpx-0.0.5/src/gdpx/builder/graph/exchange.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     5089 2024-03-17 21:29:29.000000 gdpx-0.0.5/src/gdpx/builder/graph/insert.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     5355 2024-03-17 21:29:29.000000 gdpx-0.0.5/src/gdpx/builder/graph/modifier.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     5664 2024-03-17 21:29:29.000000 gdpx-0.0.5/src/gdpx/builder/graph/remove.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     5373 2024-03-17 21:29:29.000000 gdpx-0.0.5/src/gdpx/builder/group.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     6914 2024-03-02 03:59:21.000000 gdpx-0.0.5/src/gdpx/builder/hypercube.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     2745 2024-03-17 21:29:29.000000 gdpx-0.0.5/src/gdpx/builder/insert.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     8537 2024-03-17 21:29:29.000000 gdpx-0.0.5/src/gdpx/builder/interface.py
-drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-03-17 21:31:33.451271 gdpx-0.0.5/src/gdpx/builder/mutation/
--rw-r--r--   0 jx1279   (353055) chem     (30004)      892 2023-12-01 19:22:44.000000 gdpx-0.0.5/src/gdpx/builder/mutation/__init__.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     5565 2023-12-01 19:22:44.000000 gdpx-0.0.5/src/gdpx/builder/packer.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     2972 2024-03-17 21:29:29.000000 gdpx-0.0.5/src/gdpx/builder/perturbator.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)    15179 2024-03-17 21:29:29.000000 gdpx-0.0.5/src/gdpx/builder/randomBuilder.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)    19280 2024-03-17 21:29:29.000000 gdpx-0.0.5/src/gdpx/builder/region.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)      745 2023-12-01 19:22:44.000000 gdpx-0.0.5/src/gdpx/builder/repeat.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     3614 2023-12-01 19:22:44.000000 gdpx-0.0.5/src/gdpx/builder/species.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     6065 2024-03-17 21:29:29.000000 gdpx-0.0.5/src/gdpx/builder/utils.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     1391 2023-12-01 19:22:44.000000 gdpx-0.0.5/src/gdpx/builder/zoom.py
-drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-03-17 21:31:33.456271 gdpx-0.0.5/src/gdpx/colvar/
--rw-r--r--   0 jx1279   (353055) chem     (30004)      463 2024-03-17 21:29:07.000000 gdpx-0.0.5/src/gdpx/colvar/__init__.py
--rwxr-xr-x   0 jx1279   (353055) chem     (30004)     2622 2023-09-06 03:11:48.000000 gdpx-0.0.5/src/gdpx/colvar/compute_reweight.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     1554 2024-03-02 03:59:21.000000 gdpx-0.0.5/src/gdpx/colvar/coordination.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)      636 2024-03-17 21:29:07.000000 gdpx-0.0.5/src/gdpx/colvar/distance.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     3567 2024-02-19 02:43:10.000000 gdpx-0.0.5/src/gdpx/colvar/fingerprint.py
--rwxr-xr-x   0 jx1279   (353055) chem     (30004)     5096 2023-08-21 19:26:15.000000 gdpx-0.0.5/src/gdpx/colvar/plot_meta.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     5603 2023-11-09 19:54:15.000000 gdpx-0.0.5/src/gdpx/colvar/plot_string.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     4637 2023-08-31 04:35:40.000000 gdpx-0.0.5/src/gdpx/colvar/plotstring.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)      178 2023-12-01 19:22:44.000000 gdpx-0.0.5/src/gdpx/colvar/position.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     2749 2023-09-05 04:11:13.000000 gdpx-0.0.5/src/gdpx/colvar/reweight.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     1461 2024-02-21 03:43:26.000000 gdpx-0.0.5/src/gdpx/colvar/rmsd.py
-drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-03-17 21:31:33.459271 gdpx-0.0.5/src/gdpx/comparator/
--rw-r--r--   0 jx1279   (353055) chem     (30004)      954 2024-03-02 03:59:21.000000 gdpx-0.0.5/src/gdpx/comparator/__init__.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     2739 2023-12-06 01:21:35.000000 gdpx-0.0.5/src/gdpx/comparator/cartesian.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)      827 2024-01-23 21:20:47.000000 gdpx-0.0.5/src/gdpx/comparator/comparator.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     5645 2024-03-02 03:59:21.000000 gdpx-0.0.5/src/gdpx/comparator/coordination.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     4595 2023-12-06 01:21:35.000000 gdpx-0.0.5/src/gdpx/comparator/graph.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     1193 2023-12-01 19:22:44.000000 gdpx-0.0.5/src/gdpx/comparator/interface.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     3067 2023-12-01 19:22:44.000000 gdpx-0.0.5/src/gdpx/comparator/reaction.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     5123 2023-12-01 19:22:44.000000 gdpx-0.0.5/src/gdpx/comparator/singlepoint.py
-drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-03-17 21:31:33.465271 gdpx-0.0.5/src/gdpx/computation/
--rw-r--r--   0 jx1279   (353055) chem     (30004)      657 2023-12-01 19:22:44.000000 gdpx-0.0.5/src/gdpx/computation/__init__.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)    23849 2024-03-17 21:29:29.000000 gdpx-0.0.5/src/gdpx/computation/asedriver.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)    21642 2023-12-01 19:22:44.000000 gdpx-0.0.5/src/gdpx/computation/cp2k.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     7170 2023-12-01 19:22:44.000000 gdpx-0.0.5/src/gdpx/computation/dpx.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)    15669 2024-03-17 21:29:29.000000 gdpx-0.0.5/src/gdpx/computation/driver.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     8651 2023-12-01 19:22:44.000000 gdpx-0.0.5/src/gdpx/computation/espresso.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)    18883 2024-03-17 21:29:29.000000 gdpx-0.0.5/src/gdpx/computation/interface.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)    31350 2024-03-02 03:59:21.000000 gdpx-0.0.5/src/gdpx/computation/lammps.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)    21780 2024-03-17 21:29:29.000000 gdpx-0.0.5/src/gdpx/computation/lasp.py
-drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-03-17 21:31:33.466271 gdpx-0.0.5/src/gdpx/computation/md/
--rw-r--r--   0 jx1279   (353055) chem     (30004)     1082 2024-03-17 21:29:29.000000 gdpx-0.0.5/src/gdpx/computation/md/md_utils.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     5296 2024-03-17 21:29:29.000000 gdpx-0.0.5/src/gdpx/computation/md/nosehoover.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)    10883 2023-12-01 19:22:44.000000 gdpx-0.0.5/src/gdpx/computation/plumed.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)        0 2024-03-17 21:29:29.000000 gdpx-0.0.5/src/gdpx/computation/reann.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     3016 2023-12-01 19:22:44.000000 gdpx-0.0.5/src/gdpx/computation/utils.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)    15738 2024-03-02 03:59:21.000000 gdpx-0.0.5/src/gdpx/computation/vasp.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     1463 2024-03-17 21:29:29.000000 gdpx-0.0.5/src/gdpx/config.py
-drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-03-17 21:31:33.468271 gdpx-0.0.5/src/gdpx/core/
--rw-r--r--   0 jx1279   (353055) chem     (30004)      108 2024-03-02 03:59:21.000000 gdpx-0.0.5/src/gdpx/core/__init__.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     2415 2024-03-17 21:29:29.000000 gdpx-0.0.5/src/gdpx/core/node.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     2216 2024-03-17 21:29:29.000000 gdpx-0.0.5/src/gdpx/core/operation.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)      861 2024-03-02 03:59:21.000000 gdpx-0.0.5/src/gdpx/core/placeholder.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     7037 2024-03-17 21:29:29.000000 gdpx-0.0.5/src/gdpx/core/register.py
-drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-03-17 21:31:33.470271 gdpx-0.0.5/src/gdpx/core/session/
--rw-r--r--   0 jx1279   (353055) chem     (30004)      148 2024-03-02 03:59:21.000000 gdpx-0.0.5/src/gdpx/core/session/__init__.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)    12769 2024-03-17 21:29:29.000000 gdpx-0.0.5/src/gdpx/core/session/active.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     2552 2024-03-02 03:59:21.000000 gdpx-0.0.5/src/gdpx/core/session/basic.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     6672 2024-03-17 21:29:29.000000 gdpx-0.0.5/src/gdpx/core/session/interface.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     1998 2024-03-17 21:29:29.000000 gdpx-0.0.5/src/gdpx/core/session/utils.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     1461 2024-03-17 21:29:29.000000 gdpx-0.0.5/src/gdpx/core/variable.py
-drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-03-17 21:31:33.475271 gdpx-0.0.5/src/gdpx/data/
--rwxr-xr-x   0 jx1279   (353055) chem     (30004)     6210 2023-12-01 19:22:44.000000 gdpx-0.0.5/src/gdpx/data/ClusterAndCUR.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)      249 2023-12-01 19:22:44.000000 gdpx-0.0.5/src/gdpx/data/__init__.py
--rwxr-xr-x   0 jx1279   (353055) chem     (30004)    57236 2024-03-17 21:29:29.000000 gdpx-0.0.5/src/gdpx/data/analyser.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)    14420 2024-03-17 21:29:29.000000 gdpx-0.0.5/src/gdpx/data/array.py
--rwxr-xr-x   0 jx1279   (353055) chem     (30004)     7981 2023-12-01 19:22:44.000000 gdpx-0.0.5/src/gdpx/data/cleave_deviation.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     1901 2023-12-01 19:22:44.000000 gdpx-0.0.5/src/gdpx/data/convert.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     3103 2023-12-01 19:22:44.000000 gdpx-0.0.5/src/gdpx/data/correction.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     9171 2023-12-01 19:22:44.000000 gdpx-0.0.5/src/gdpx/data/database.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     8873 2024-03-17 21:29:29.000000 gdpx-0.0.5/src/gdpx/data/dataset.py
--rwxr-xr-x   0 jx1279   (353055) chem     (30004)     3389 2023-12-01 19:22:44.000000 gdpx-0.0.5/src/gdpx/data/extract_evolution.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)    13864 2024-03-17 21:29:29.000000 gdpx-0.0.5/src/gdpx/data/interface.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)    12314 2023-12-01 19:22:44.000000 gdpx-0.0.5/src/gdpx/data/operators.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     1950 2023-12-01 19:22:44.000000 gdpx-0.0.5/src/gdpx/data/system.py
-drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-03-17 21:31:33.477271 gdpx-0.0.5/src/gdpx/describer/
--rw-r--r--   0 jx1279   (353055) chem     (30004)      170 2023-12-01 19:22:44.000000 gdpx-0.0.5/src/gdpx/describer/__init__.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     2325 2024-02-09 18:38:45.000000 gdpx-0.0.5/src/gdpx/describer/describer.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)      520 2023-12-01 19:22:44.000000 gdpx-0.0.5/src/gdpx/describer/interface.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     2365 2023-12-01 19:22:44.000000 gdpx-0.0.5/src/gdpx/describer/soap.py
-drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-03-17 21:31:33.478271 gdpx-0.0.5/src/gdpx/expedition/
--rw-r--r--   0 jx1279   (353055) chem     (30004)     1383 2023-12-01 19:22:44.000000 gdpx-0.0.5/src/gdpx/expedition/__init__.py
-drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-03-17 21:31:33.478271 gdpx-0.0.5/src/gdpx/expedition/af/
--rw-r--r--   0 jx1279   (353055) chem     (30004)    11079 2024-03-17 21:29:29.000000 gdpx-0.0.5/src/gdpx/expedition/af/afir.py
-drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-03-17 21:31:33.479271 gdpx-0.0.5/src/gdpx/expedition/bh/
--rw-r--r--   0 jx1279   (353055) chem     (30004)     1121 2024-03-02 03:59:21.000000 gdpx-0.0.5/src/gdpx/expedition/bh/bh.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     1203 2024-03-17 21:29:29.000000 gdpx-0.0.5/src/gdpx/expedition/expedition.py
-drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-03-17 21:31:33.480271 gdpx-0.0.5/src/gdpx/expedition/ga/
--rwxr-xr-x   0 jx1279   (353055) chem     (30004)    27253 2024-03-02 03:59:21.000000 gdpx-0.0.5/src/gdpx/expedition/ga/engine.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)    17387 2024-02-27 18:01:28.000000 gdpx-0.0.5/src/gdpx/expedition/ga/population.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     3923 2024-03-17 21:29:29.000000 gdpx-0.0.5/src/gdpx/expedition/interface.py
-drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-03-17 21:31:33.480271 gdpx-0.0.5/src/gdpx/expedition/mc/
--rw-r--r--   0 jx1279   (353055) chem     (30004)    16303 2024-03-17 21:29:29.000000 gdpx-0.0.5/src/gdpx/expedition/mc/mc.py
-drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-03-17 21:31:33.482271 gdpx-0.0.5/src/gdpx/expedition/mc/operators/
--rw-r--r--   0 jx1279   (353055) chem     (30004)     2251 2024-01-22 03:21:03.000000 gdpx-0.0.5/src/gdpx/expedition/mc/operators/__init__.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)    10696 2024-03-17 21:29:29.000000 gdpx-0.0.5/src/gdpx/expedition/mc/operators/exchange.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     6764 2024-03-02 06:03:09.000000 gdpx-0.0.5/src/gdpx/expedition/mc/operators/move.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     4734 2024-03-02 03:59:21.000000 gdpx-0.0.5/src/gdpx/expedition/mc/operators/operator.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     4644 2023-12-01 19:22:44.000000 gdpx-0.0.5/src/gdpx/expedition/mc/operators/swap.py
-drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-03-17 21:31:33.485271 gdpx-0.0.5/src/gdpx/graph/
--rw-r--r--   0 jx1279   (353055) chem     (30004)      147 2024-03-17 21:29:29.000000 gdpx-0.0.5/src/gdpx/graph/__init__.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)    13870 2023-12-01 19:22:44.000000 gdpx-0.0.5/src/gdpx/graph/comparison.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)    12839 2024-03-17 21:29:29.000000 gdpx-0.0.5/src/gdpx/graph/creator.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)    12200 2023-12-01 19:22:44.000000 gdpx-0.0.5/src/gdpx/graph/graph_main.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     5142 2024-03-17 21:29:29.000000 gdpx-0.0.5/src/gdpx/graph/molecule.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)    31066 2024-03-17 21:29:29.000000 gdpx-0.0.5/src/gdpx/graph/sites.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     2905 2024-03-17 21:29:29.000000 gdpx-0.0.5/src/gdpx/graph/surface.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     1849 2023-12-01 19:22:44.000000 gdpx-0.0.5/src/gdpx/graph/utils.py
--rwxr-xr-x   0 jx1279   (353055) chem     (30004)     8780 2024-03-17 21:29:29.000000 gdpx-0.0.5/src/gdpx/main.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     2242 2023-07-23 06:17:20.000000 gdpx-0.0.5/src/gdpx/nanoparticle.py
-drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-03-17 21:31:33.487270 gdpx-0.0.5/src/gdpx/potential/
--rw-r--r--   0 jx1279   (353055) chem     (30004)      273 2024-03-17 21:29:29.000000 gdpx-0.0.5/src/gdpx/potential/__init__.py
-drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-03-17 21:31:33.487270 gdpx-0.0.5/src/gdpx/potential/calculators/
--rw-r--r--   0 jx1279   (353055) chem     (30004)     4675 2024-03-17 21:29:29.000000 gdpx-0.0.5/src/gdpx/potential/calculators/mixer.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     1256 2024-03-17 21:29:29.000000 gdpx-0.0.5/src/gdpx/potential/interface.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     6138 2024-03-17 21:29:29.000000 gdpx-0.0.5/src/gdpx/potential/manager.py
-drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-03-17 21:31:33.494270 gdpx-0.0.5/src/gdpx/potential/managers/
--rw-r--r--   0 jx1279   (353055) chem     (30004)     2940 2024-03-17 21:29:29.000000 gdpx-0.0.5/src/gdpx/potential/managers/__init__.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     1559 2024-03-02 03:59:21.000000 gdpx-0.0.5/src/gdpx/potential/managers/bias.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     2947 2024-03-02 03:59:21.000000 gdpx-0.0.5/src/gdpx/potential/managers/cp2k.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)    25018 2024-03-17 21:29:29.000000 gdpx-0.0.5/src/gdpx/potential/managers/deepmd.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     1149 2023-12-01 19:22:44.000000 gdpx-0.0.5/src/gdpx/potential/managers/dftd3.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     2231 2024-03-02 03:59:21.000000 gdpx-0.0.5/src/gdpx/potential/managers/eam.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     1117 2024-03-02 03:59:21.000000 gdpx-0.0.5/src/gdpx/potential/managers/emt.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     2363 2024-03-02 03:59:21.000000 gdpx-0.0.5/src/gdpx/potential/managers/espresso.py
-drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-03-17 21:31:33.496271 gdpx-0.0.5/src/gdpx/potential/managers/gp/
--rw-r--r--   0 jx1279   (353055) chem     (30004)       83 2024-03-02 03:59:21.000000 gdpx-0.0.5/src/gdpx/potential/managers/gp/__init__.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     2348 2024-03-02 03:59:21.000000 gdpx-0.0.5/src/gdpx/potential/managers/gp/bench.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     1376 2024-03-02 03:59:21.000000 gdpx-0.0.5/src/gdpx/potential/managers/gp/fgp.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     3746 2024-03-02 03:59:21.000000 gdpx-0.0.5/src/gdpx/potential/managers/gp/gptools.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     3474 2024-03-02 03:59:21.000000 gdpx-0.0.5/src/gdpx/potential/managers/gp/representation.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)    46869 2024-03-02 03:59:21.000000 gdpx-0.0.5/src/gdpx/potential/managers/gp/sgp.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     2715 2023-12-01 19:22:44.000000 gdpx-0.0.5/src/gdpx/potential/managers/grid.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     1986 2024-03-02 03:59:21.000000 gdpx-0.0.5/src/gdpx/potential/managers/lasp.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)    12691 2024-03-17 21:29:29.000000 gdpx-0.0.5/src/gdpx/potential/managers/mace.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     1840 2024-03-17 21:29:29.000000 gdpx-0.0.5/src/gdpx/potential/managers/mixer.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     7976 2024-03-17 21:29:29.000000 gdpx-0.0.5/src/gdpx/potential/managers/nequip.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     1990 2024-03-02 03:59:21.000000 gdpx-0.0.5/src/gdpx/potential/managers/plumed.py
-drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-03-17 21:31:33.497270 gdpx-0.0.5/src/gdpx/potential/managers/reann/
--rw-r--r--   0 jx1279   (353055) chem     (30004)     7421 2024-03-17 21:29:29.000000 gdpx-0.0.5/src/gdpx/potential/managers/reann/beann.py
-drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-03-17 21:31:33.497270 gdpx-0.0.5/src/gdpx/potential/managers/reann/calculators/
--rw-r--r--   0 jx1279   (353055) chem     (30004)     3361 2024-03-17 21:29:29.000000 gdpx-0.0.5/src/gdpx/potential/managers/reann/calculators/reann.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)    17641 2024-03-17 21:29:29.000000 gdpx-0.0.5/src/gdpx/potential/managers/reann/reann.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     1396 2024-03-02 03:59:21.000000 gdpx-0.0.5/src/gdpx/potential/managers/reax.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     8903 2024-03-02 03:59:21.000000 gdpx-0.0.5/src/gdpx/potential/managers/schnet.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     3654 2024-03-02 03:59:21.000000 gdpx-0.0.5/src/gdpx/potential/managers/vasp.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     1207 2024-03-02 03:59:21.000000 gdpx-0.0.5/src/gdpx/potential/managers/xtb.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     5520 2024-03-17 21:29:29.000000 gdpx-0.0.5/src/gdpx/potential/trainer.py
-drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-03-17 21:31:33.499270 gdpx-0.0.5/src/gdpx/reactor/
--rw-r--r--   0 jx1279   (353055) chem     (30004)      750 2024-03-17 21:29:29.000000 gdpx-0.0.5/src/gdpx/reactor/__init__.py
-drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-03-17 21:31:33.503270 gdpx-0.0.5/src/gdpx/reactor/future/
--rw-r--r--   0 jx1279   (353055) chem     (30004)    23672 2023-12-01 19:22:44.000000 gdpx-0.0.5/src/gdpx/reactor/future/AccCons.py
--rwxr-xr-x   0 jx1279   (353055) chem     (30004)    16224 2023-12-01 19:22:44.000000 gdpx-0.0.5/src/gdpx/reactor/future/AccHop.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     2601 2023-12-01 19:22:44.000000 gdpx-0.0.5/src/gdpx/reactor/future/AccNEB.py
--rwxr-xr-x   0 jx1279   (353055) chem     (30004)     2921 2023-12-01 19:22:44.000000 gdpx-0.0.5/src/gdpx/reactor/future/cmp_mep.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     3833 2023-12-01 19:22:44.000000 gdpx-0.0.5/src/gdpx/reactor/future/constrain.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     7051 2023-12-01 19:22:44.000000 gdpx-0.0.5/src/gdpx/reactor/future/crs.py
--rwxr-xr-x   0 jx1279   (353055) chem     (30004)     2226 2023-12-01 19:22:44.000000 gdpx-0.0.5/src/gdpx/reactor/future/diffusion3.py
--rwxr-xr-x   0 jx1279   (353055) chem     (30004)    11410 2023-12-01 19:22:44.000000 gdpx-0.0.5/src/gdpx/reactor/future/find_adsorption.py
--rwxr-xr-x   0 jx1279   (353055) chem     (30004)     3188 2023-12-01 19:22:44.000000 gdpx-0.0.5/src/gdpx/reactor/future/find_inter.py
--rwxr-xr-x   0 jx1279   (353055) chem     (30004)     3002 2023-12-01 19:22:44.000000 gdpx-0.0.5/src/gdpx/reactor/future/muller-brown.py
--rwxr-xr-x   0 jx1279   (353055) chem     (30004)     1154 2023-12-01 19:22:44.000000 gdpx-0.0.5/src/gdpx/reactor/future/test_mh.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     7056 2023-12-01 19:22:44.000000 gdpx-0.0.5/src/gdpx/reactor/interface.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     1482 2023-12-01 19:22:44.000000 gdpx-0.0.5/src/gdpx/reactor/reactor.py
-drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-03-17 21:31:33.505270 gdpx-0.0.5/src/gdpx/reactor/string/
--rw-r--r--   0 jx1279   (353055) chem     (30004)      232 2023-12-01 19:22:44.000000 gdpx-0.0.5/src/gdpx/reactor/string/__init__.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)    17830 2024-03-17 21:29:29.000000 gdpx-0.0.5/src/gdpx/reactor/string/cp2k.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     5117 2024-03-17 21:29:29.000000 gdpx-0.0.5/src/gdpx/reactor/string/grid.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     7928 2024-03-17 21:29:29.000000 gdpx-0.0.5/src/gdpx/reactor/string/pathway.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     9640 2024-03-17 21:29:29.000000 gdpx-0.0.5/src/gdpx/reactor/string/string.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     7869 2024-03-17 21:29:29.000000 gdpx-0.0.5/src/gdpx/reactor/string/vasp.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     2428 2024-03-02 03:59:21.000000 gdpx-0.0.5/src/gdpx/reactor/utils.py
-drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-03-17 21:31:33.508270 gdpx-0.0.5/src/gdpx/scheduler/
--rw-r--r--   0 jx1279   (353055) chem     (30004)      699 2024-03-17 21:29:30.000000 gdpx-0.0.5/src/gdpx/scheduler/__init__.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)      624 2023-12-01 19:22:44.000000 gdpx-0.0.5/src/gdpx/scheduler/interface.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)      631 2024-03-17 21:29:30.000000 gdpx-0.0.5/src/gdpx/scheduler/local.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     3553 2024-03-17 21:29:30.000000 gdpx-0.0.5/src/gdpx/scheduler/lsf.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     1147 2024-03-17 21:29:30.000000 gdpx-0.0.5/src/gdpx/scheduler/pbs.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     4439 2024-03-17 21:29:30.000000 gdpx-0.0.5/src/gdpx/scheduler/scheduler.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     3226 2024-03-17 21:29:30.000000 gdpx-0.0.5/src/gdpx/scheduler/slurm.py
-drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-03-17 21:31:33.513270 gdpx-0.0.5/src/gdpx/selector/
--rw-r--r--   0 jx1279   (353055) chem     (30004)     1006 2024-03-17 21:29:30.000000 gdpx-0.0.5/src/gdpx/selector/__init__.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     3664 2024-03-17 21:29:30.000000 gdpx-0.0.5/src/gdpx/selector/basin.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     6276 2024-03-17 21:29:30.000000 gdpx-0.0.5/src/gdpx/selector/compare.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     1376 2024-03-17 21:29:30.000000 gdpx-0.0.5/src/gdpx/selector/composition.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     8362 2024-03-17 21:29:30.000000 gdpx-0.0.5/src/gdpx/selector/cur.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     6960 2024-03-17 21:29:30.000000 gdpx-0.0.5/src/gdpx/selector/descriptor.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     5631 2024-03-17 21:29:30.000000 gdpx-0.0.5/src/gdpx/selector/graph.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     5185 2024-03-17 21:29:30.000000 gdpx-0.0.5/src/gdpx/selector/interface.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     2905 2024-03-17 21:29:30.000000 gdpx-0.0.5/src/gdpx/selector/interval.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)      622 2024-03-17 21:29:30.000000 gdpx-0.0.5/src/gdpx/selector/invariant.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     3284 2024-03-17 21:29:30.000000 gdpx-0.0.5/src/gdpx/selector/locate.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)    11955 2024-03-17 21:29:30.000000 gdpx-0.0.5/src/gdpx/selector/property.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     1987 2024-03-17 21:29:30.000000 gdpx-0.0.5/src/gdpx/selector/random.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     9259 2024-03-17 21:29:30.000000 gdpx-0.0.5/src/gdpx/selector/selector.py
-drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-03-17 21:31:33.514270 gdpx-0.0.5/src/gdpx/trainer/
--rw-r--r--   0 jx1279   (353055) chem     (30004)     1050 2024-03-17 21:29:30.000000 gdpx-0.0.5/src/gdpx/trainer/__init__.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     6277 2024-03-17 21:29:30.000000 gdpx-0.0.5/src/gdpx/trainer/interface.py
-drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-03-17 21:31:33.518270 gdpx-0.0.5/src/gdpx/utils/
--rw-r--r--   0 jx1279   (353055) chem     (30004)       83 2023-12-01 19:22:44.000000 gdpx-0.0.5/src/gdpx/utils/__init__.py
--rwxr-xr-x   0 jx1279   (353055) chem     (30004)     7894 2023-12-01 19:22:44.000000 gdpx-0.0.5/src/gdpx/utils/atomUtils.py
--rwxr-xr-x   0 jx1279   (353055) chem     (30004)     2908 2023-12-01 19:22:44.000000 gdpx-0.0.5/src/gdpx/utils/cleave_cluster.py
--rwxr-xr-x   0 jx1279   (353055) chem     (30004)     6500 2023-12-01 19:22:44.000000 gdpx-0.0.5/src/gdpx/utils/cmp_refdat.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     6382 2024-03-17 21:29:30.000000 gdpx-0.0.5/src/gdpx/utils/command.py
--rwxr-xr-x   0 jx1279   (353055) chem     (30004)    12328 2023-12-01 19:22:44.000000 gdpx-0.0.5/src/gdpx/utils/comparision.py
-drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-03-17 21:31:33.519270 gdpx-0.0.5/src/gdpx/utils/dputils/
--rw-r--r--   0 jx1279   (353055) chem     (30004)     9418 2023-12-01 19:22:44.000000 gdpx-0.0.5/src/gdpx/utils/dputils/DeepPot.py
--rwxr-xr-x   0 jx1279   (353055) chem     (30004)    14661 2023-12-01 19:22:44.000000 gdpx-0.0.5/src/gdpx/utils/dputils/acquire_dmat.py
--rwxr-xr-x   0 jx1279   (353055) chem     (30004)     3727 2023-12-01 19:22:44.000000 gdpx-0.0.5/src/gdpx/utils/dputils/dpset2xyz-all.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     1095 2023-12-01 19:22:44.000000 gdpx-0.0.5/src/gdpx/utils/geometry.py
--rwxr-xr-x   0 jx1279   (353055) chem     (30004)     2147 2023-12-01 19:22:44.000000 gdpx-0.0.5/src/gdpx/utils/plot_dimer.py
--rwxr-xr-x   0 jx1279   (353055) chem     (30004)     7761 2023-12-01 19:22:44.000000 gdpx-0.0.5/src/gdpx/utils/reduce_dataset.py
--rwxr-xr-x   0 jx1279   (353055) chem     (30004)     6200 2023-12-01 19:22:44.000000 gdpx-0.0.5/src/gdpx/utils/second_reduce.py
--rwxr-xr-x   0 jx1279   (353055) chem     (30004)     5412 2024-03-17 21:29:30.000000 gdpx-0.0.5/src/gdpx/utils/split-dataset.py
-drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-03-17 21:31:33.525270 gdpx-0.0.5/src/gdpx/validator/
--rw-r--r--   0 jx1279   (353055) chem     (30004)     1945 2023-12-01 19:22:44.000000 gdpx-0.0.5/src/gdpx/validator/__init__.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     5610 2024-03-17 21:29:30.000000 gdpx-0.0.5/src/gdpx/validator/diffusion_coefficient.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     4063 2024-03-17 21:29:30.000000 gdpx-0.0.5/src/gdpx/validator/dimer.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     2640 2024-03-17 21:29:30.000000 gdpx-0.0.5/src/gdpx/validator/eos.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     4779 2024-03-02 03:59:21.000000 gdpx-0.0.5/src/gdpx/validator/interface.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     5879 2024-03-17 21:29:30.000000 gdpx-0.0.5/src/gdpx/validator/mdf.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     7477 2024-03-17 21:29:30.000000 gdpx-0.0.5/src/gdpx/validator/melting_point.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     5744 2023-12-01 19:22:44.000000 gdpx-0.0.5/src/gdpx/validator/minima.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)      583 2023-12-01 19:22:44.000000 gdpx-0.0.5/src/gdpx/validator/rank.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     9391 2024-03-17 21:29:30.000000 gdpx-0.0.5/src/gdpx/validator/rdf.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     2486 2024-03-17 21:29:30.000000 gdpx-0.0.5/src/gdpx/validator/rxn.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     8725 2024-03-02 03:59:21.000000 gdpx-0.0.5/src/gdpx/validator/spc.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     3690 2023-12-01 19:22:44.000000 gdpx-0.0.5/src/gdpx/validator/surface_energy.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     2029 2023-12-01 19:22:44.000000 gdpx-0.0.5/src/gdpx/validator/utils.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)      980 2023-12-01 19:22:44.000000 gdpx-0.0.5/src/gdpx/validator/validator.py
-drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-03-17 21:31:33.529270 gdpx-0.0.5/src/gdpx/worker/
--rw-r--r--   0 jx1279   (353055) chem     (30004)       84 2023-12-01 19:22:44.000000 gdpx-0.0.5/src/gdpx/worker/__init__.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)    30113 2024-03-17 21:29:30.000000 gdpx-0.0.5/src/gdpx/worker/drive.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     6935 2024-03-17 21:29:30.000000 gdpx-0.0.5/src/gdpx/worker/explore.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     7188 2023-12-01 19:22:44.000000 gdpx-0.0.5/src/gdpx/worker/grid.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)    11343 2024-03-17 21:29:30.000000 gdpx-0.0.5/src/gdpx/worker/interface.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)    18256 2023-12-01 19:22:44.000000 gdpx-0.0.5/src/gdpx/worker/react.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)    12484 2024-03-17 21:29:30.000000 gdpx-0.0.5/src/gdpx/worker/single.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)    11940 2024-03-17 21:29:30.000000 gdpx-0.0.5/src/gdpx/worker/train.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     1958 2023-12-01 19:22:44.000000 gdpx-0.0.5/src/gdpx/worker/utils.py
--rw-r--r--   0 jx1279   (353055) chem     (30004)     6077 2024-03-17 21:29:30.000000 gdpx-0.0.5/src/gdpx/worker/worker.py
-drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-03-17 21:31:33.530270 gdpx-0.0.5/src/gdpx.egg-info/
--rw-r--r--   0 jx1279   (353055) chem     (30004)    47663 2024-03-17 21:31:33.000000 gdpx-0.0.5/src/gdpx.egg-info/PKG-INFO
--rw-r--r--   0 jx1279   (353055) chem     (30004)     7528 2024-03-17 21:31:33.000000 gdpx-0.0.5/src/gdpx.egg-info/SOURCES.txt
--rw-r--r--   0 jx1279   (353055) chem     (30004)        1 2024-03-17 21:31:33.000000 gdpx-0.0.5/src/gdpx.egg-info/dependency_links.txt
--rw-r--r--   0 jx1279   (353055) chem     (30004)       39 2024-03-17 21:31:33.000000 gdpx-0.0.5/src/gdpx.egg-info/entry_points.txt
--rw-r--r--   0 jx1279   (353055) chem     (30004)      111 2024-03-17 21:31:33.000000 gdpx-0.0.5/src/gdpx.egg-info/requires.txt
--rw-r--r--   0 jx1279   (353055) chem     (30004)        5 2024-03-17 21:31:33.000000 gdpx-0.0.5/src/gdpx.egg-info/top_level.txt
+drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-07 20:51:53.978648 gdpx-0.0.6/
+-rw-r--r--   0 jx1279   (353055) chem     (30004)    35149 2023-04-10 18:29:40.000000 gdpx-0.0.6/LICENSE
+-rw-r--r--   0 jx1279   (353055) chem     (30004)    47663 2024-04-07 20:51:53.977647 gdpx-0.0.6/PKG-INFO
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     6294 2023-12-12 17:08:13.000000 gdpx-0.0.6/README.md
+-rw-r--r--   0 jx1279   (353055) chem     (30004)      899 2024-04-07 20:50:42.000000 gdpx-0.0.6/pyproject.toml
+-rw-r--r--   0 jx1279   (353055) chem     (30004)       38 2024-04-07 20:51:53.978648 gdpx-0.0.6/setup.cfg
+drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-07 20:51:53.498654 gdpx-0.0.6/src/
+drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-07 20:51:53.507654 gdpx-0.0.6/src/gdpx/
+drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-07 20:51:53.527653 gdpx-0.0.6/src/gdpx/bias/
+-rw-r--r--   0 jx1279   (353055) chem     (30004)      543 2024-03-02 03:59:21.000000 gdpx-0.0.6/src/gdpx/bias/__init__.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     3140 2024-02-14 21:26:12.000000 gdpx-0.0.6/src/gdpx/bias/afir.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     1679 2024-03-02 03:59:21.000000 gdpx-0.0.6/src/gdpx/bias/bias.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     3071 2024-04-07 20:47:54.000000 gdpx-0.0.6/src/gdpx/bias/gaussian.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     2866 2024-03-02 03:59:21.000000 gdpx-0.0.6/src/gdpx/bias/harmonic.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     1209 2023-12-01 19:22:44.000000 gdpx-0.0.6/src/gdpx/bias/nuclei.py
+drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-07 20:51:53.537653 gdpx-0.0.6/src/gdpx/builder/
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     2881 2024-03-17 21:29:29.000000 gdpx-0.0.6/src/gdpx/builder/__init__.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     3100 2024-03-17 21:29:29.000000 gdpx-0.0.6/src/gdpx/builder/builder.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)      800 2023-12-03 04:28:22.000000 gdpx-0.0.6/src/gdpx/builder/cleave_group.py
+-rwxr-xr-x   0 jx1279   (353055) chem     (30004)     2659 2023-12-03 04:22:10.000000 gdpx-0.0.6/src/gdpx/builder/cleave_surface.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     5743 2023-12-01 19:22:44.000000 gdpx-0.0.6/src/gdpx/builder/constraints.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)      384 2023-12-01 19:22:44.000000 gdpx-0.0.6/src/gdpx/builder/crossover.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     1469 2023-12-01 19:22:44.000000 gdpx-0.0.6/src/gdpx/builder/dimer.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     7451 2023-12-01 19:22:44.000000 gdpx-0.0.6/src/gdpx/builder/direct.py
+drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-07 20:51:53.540653 gdpx-0.0.6/src/gdpx/builder/graph/
+-rw-r--r--   0 jx1279   (353055) chem     (30004)      287 2023-12-01 19:22:44.000000 gdpx-0.0.6/src/gdpx/builder/graph/__init__.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     5942 2024-03-17 21:29:29.000000 gdpx-0.0.6/src/gdpx/builder/graph/exchange.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     5089 2024-03-17 21:29:29.000000 gdpx-0.0.6/src/gdpx/builder/graph/insert.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     5355 2024-03-17 21:29:29.000000 gdpx-0.0.6/src/gdpx/builder/graph/modifier.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     5664 2024-03-17 21:29:29.000000 gdpx-0.0.6/src/gdpx/builder/graph/remove.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     5373 2024-03-17 21:29:29.000000 gdpx-0.0.6/src/gdpx/builder/group.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     6914 2024-03-02 03:59:21.000000 gdpx-0.0.6/src/gdpx/builder/hypercube.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     2745 2024-03-17 21:29:29.000000 gdpx-0.0.6/src/gdpx/builder/insert.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     8537 2024-03-17 21:29:29.000000 gdpx-0.0.6/src/gdpx/builder/interface.py
+drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-07 20:51:53.540653 gdpx-0.0.6/src/gdpx/builder/mutation/
+-rw-r--r--   0 jx1279   (353055) chem     (30004)      892 2023-12-01 19:22:44.000000 gdpx-0.0.6/src/gdpx/builder/mutation/__init__.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     5565 2023-12-01 19:22:44.000000 gdpx-0.0.6/src/gdpx/builder/packer.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     2972 2024-03-17 21:29:29.000000 gdpx-0.0.6/src/gdpx/builder/perturbator.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)    15179 2024-03-17 21:29:29.000000 gdpx-0.0.6/src/gdpx/builder/randomBuilder.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)    19280 2024-03-17 21:29:29.000000 gdpx-0.0.6/src/gdpx/builder/region.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)      745 2023-12-01 19:22:44.000000 gdpx-0.0.6/src/gdpx/builder/repeat.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     3614 2023-12-01 19:22:44.000000 gdpx-0.0.6/src/gdpx/builder/species.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     6065 2024-03-17 21:29:29.000000 gdpx-0.0.6/src/gdpx/builder/utils.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     1391 2023-12-01 19:22:44.000000 gdpx-0.0.6/src/gdpx/builder/zoom.py
+drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-07 20:51:53.550653 gdpx-0.0.6/src/gdpx/colvar/
+-rw-r--r--   0 jx1279   (353055) chem     (30004)      463 2024-04-07 20:47:54.000000 gdpx-0.0.6/src/gdpx/colvar/__init__.py
+-rwxr-xr-x   0 jx1279   (353055) chem     (30004)     2622 2023-09-06 03:11:48.000000 gdpx-0.0.6/src/gdpx/colvar/compute_reweight.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     1554 2024-03-02 03:59:21.000000 gdpx-0.0.6/src/gdpx/colvar/coordination.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)      636 2024-04-07 20:47:54.000000 gdpx-0.0.6/src/gdpx/colvar/distance.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     3567 2024-02-19 02:43:10.000000 gdpx-0.0.6/src/gdpx/colvar/fingerprint.py
+-rwxr-xr-x   0 jx1279   (353055) chem     (30004)     5096 2023-08-21 19:26:15.000000 gdpx-0.0.6/src/gdpx/colvar/plot_meta.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     5603 2023-11-09 19:54:15.000000 gdpx-0.0.6/src/gdpx/colvar/plot_string.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     4637 2023-08-31 04:35:40.000000 gdpx-0.0.6/src/gdpx/colvar/plotstring.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)      178 2023-12-01 19:22:44.000000 gdpx-0.0.6/src/gdpx/colvar/position.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     2749 2023-09-05 04:11:13.000000 gdpx-0.0.6/src/gdpx/colvar/reweight.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     1461 2024-02-21 03:43:26.000000 gdpx-0.0.6/src/gdpx/colvar/rmsd.py
+drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-07 20:51:53.614652 gdpx-0.0.6/src/gdpx/comparator/
+-rw-r--r--   0 jx1279   (353055) chem     (30004)      954 2024-03-02 03:59:21.000000 gdpx-0.0.6/src/gdpx/comparator/__init__.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     2739 2023-12-06 01:21:35.000000 gdpx-0.0.6/src/gdpx/comparator/cartesian.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)      827 2024-01-23 21:20:47.000000 gdpx-0.0.6/src/gdpx/comparator/comparator.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     5645 2024-03-02 03:59:21.000000 gdpx-0.0.6/src/gdpx/comparator/coordination.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     4595 2023-12-06 01:21:35.000000 gdpx-0.0.6/src/gdpx/comparator/graph.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     1193 2023-12-01 19:22:44.000000 gdpx-0.0.6/src/gdpx/comparator/interface.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     3067 2023-12-01 19:22:44.000000 gdpx-0.0.6/src/gdpx/comparator/reaction.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     5123 2023-12-01 19:22:44.000000 gdpx-0.0.6/src/gdpx/comparator/singlepoint.py
+drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-07 20:51:53.636652 gdpx-0.0.6/src/gdpx/computation/
+-rw-r--r--   0 jx1279   (353055) chem     (30004)      657 2023-12-01 19:22:44.000000 gdpx-0.0.6/src/gdpx/computation/__init__.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)    27174 2024-04-07 20:49:18.000000 gdpx-0.0.6/src/gdpx/computation/asedriver.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)    21647 2024-04-07 20:49:18.000000 gdpx-0.0.6/src/gdpx/computation/cp2k.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)    18003 2024-04-07 20:49:18.000000 gdpx-0.0.6/src/gdpx/computation/driver.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     8651 2023-12-01 19:22:44.000000 gdpx-0.0.6/src/gdpx/computation/espresso.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)    19842 2024-04-07 20:49:18.000000 gdpx-0.0.6/src/gdpx/computation/interface.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)    31347 2024-04-07 20:49:18.000000 gdpx-0.0.6/src/gdpx/computation/lammps.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)    22229 2024-04-07 20:49:18.000000 gdpx-0.0.6/src/gdpx/computation/lasp.py
+drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-07 20:51:53.637652 gdpx-0.0.6/src/gdpx/computation/md/
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     1082 2024-03-17 21:29:29.000000 gdpx-0.0.6/src/gdpx/computation/md/md_utils.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     5296 2024-03-17 21:29:29.000000 gdpx-0.0.6/src/gdpx/computation/md/nosehoover.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)        0 2024-03-17 21:29:29.000000 gdpx-0.0.6/src/gdpx/computation/reann.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     2372 2024-04-07 20:49:18.000000 gdpx-0.0.6/src/gdpx/computation/utils.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)    20268 2024-04-07 20:49:18.000000 gdpx-0.0.6/src/gdpx/computation/vasp.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     1463 2024-03-17 21:29:29.000000 gdpx-0.0.6/src/gdpx/config.py
+drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-07 20:51:53.640652 gdpx-0.0.6/src/gdpx/core/
+-rw-r--r--   0 jx1279   (353055) chem     (30004)      108 2024-03-02 03:59:21.000000 gdpx-0.0.6/src/gdpx/core/__init__.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     2415 2024-03-17 21:29:29.000000 gdpx-0.0.6/src/gdpx/core/node.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     2492 2024-04-07 20:49:18.000000 gdpx-0.0.6/src/gdpx/core/operation.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)      861 2024-03-02 03:59:21.000000 gdpx-0.0.6/src/gdpx/core/placeholder.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     7032 2024-04-07 20:49:18.000000 gdpx-0.0.6/src/gdpx/core/register.py
+drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-07 20:51:53.644652 gdpx-0.0.6/src/gdpx/core/session/
+-rw-r--r--   0 jx1279   (353055) chem     (30004)      148 2024-03-02 03:59:21.000000 gdpx-0.0.6/src/gdpx/core/session/__init__.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)    12927 2024-04-07 20:49:18.000000 gdpx-0.0.6/src/gdpx/core/session/active.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     2007 2024-04-07 20:49:18.000000 gdpx-0.0.6/src/gdpx/core/session/basic.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     7692 2024-04-07 20:49:18.000000 gdpx-0.0.6/src/gdpx/core/session/interface.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     2583 2024-04-07 20:49:18.000000 gdpx-0.0.6/src/gdpx/core/session/session.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     1998 2024-03-17 21:29:29.000000 gdpx-0.0.6/src/gdpx/core/session/utils.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     1461 2024-03-17 21:29:29.000000 gdpx-0.0.6/src/gdpx/core/variable.py
+drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-07 20:51:53.673651 gdpx-0.0.6/src/gdpx/data/
+-rwxr-xr-x   0 jx1279   (353055) chem     (30004)     6210 2023-12-01 19:22:44.000000 gdpx-0.0.6/src/gdpx/data/ClusterAndCUR.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)      249 2023-12-01 19:22:44.000000 gdpx-0.0.6/src/gdpx/data/__init__.py
+-rwxr-xr-x   0 jx1279   (353055) chem     (30004)    57236 2024-03-17 21:29:29.000000 gdpx-0.0.6/src/gdpx/data/analyser.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)    14976 2024-04-07 20:49:18.000000 gdpx-0.0.6/src/gdpx/data/array.py
+-rwxr-xr-x   0 jx1279   (353055) chem     (30004)     7981 2023-12-01 19:22:44.000000 gdpx-0.0.6/src/gdpx/data/cleave_deviation.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     1901 2023-12-01 19:22:44.000000 gdpx-0.0.6/src/gdpx/data/convert.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     3103 2023-12-01 19:22:44.000000 gdpx-0.0.6/src/gdpx/data/correction.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     9171 2023-12-01 19:22:44.000000 gdpx-0.0.6/src/gdpx/data/database.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)    11961 2024-04-07 20:49:18.000000 gdpx-0.0.6/src/gdpx/data/dataset.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     1552 2024-04-07 20:49:18.000000 gdpx-0.0.6/src/gdpx/data/extatoms.py
+-rwxr-xr-x   0 jx1279   (353055) chem     (30004)     3389 2023-12-01 19:22:44.000000 gdpx-0.0.6/src/gdpx/data/extract_evolution.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)    14345 2024-04-07 20:49:18.000000 gdpx-0.0.6/src/gdpx/data/interface.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)    10543 2024-04-07 20:49:18.000000 gdpx-0.0.6/src/gdpx/data/operators.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     1950 2023-12-01 19:22:44.000000 gdpx-0.0.6/src/gdpx/data/system.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     1210 2024-04-07 20:49:18.000000 gdpx-0.0.6/src/gdpx/data/utils.py
+drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-07 20:51:53.676651 gdpx-0.0.6/src/gdpx/describer/
+-rw-r--r--   0 jx1279   (353055) chem     (30004)      441 2024-04-07 20:49:18.000000 gdpx-0.0.6/src/gdpx/describer/__init__.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     2325 2024-02-09 18:38:45.000000 gdpx-0.0.6/src/gdpx/describer/describer.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     2066 2024-04-07 20:49:18.000000 gdpx-0.0.6/src/gdpx/describer/interface.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     2365 2023-12-01 19:22:44.000000 gdpx-0.0.6/src/gdpx/describer/soap.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     2438 2024-04-07 20:49:18.000000 gdpx-0.0.6/src/gdpx/describer/spc.py
+drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-07 20:51:53.678651 gdpx-0.0.6/src/gdpx/expedition/
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     1360 2024-04-07 20:49:18.000000 gdpx-0.0.6/src/gdpx/expedition/__init__.py
+drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-07 20:51:53.679651 gdpx-0.0.6/src/gdpx/expedition/af/
+-rw-r--r--   0 jx1279   (353055) chem     (30004)    10315 2024-04-07 20:49:18.000000 gdpx-0.0.6/src/gdpx/expedition/af/afir.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     1793 2024-04-07 20:49:18.000000 gdpx-0.0.6/src/gdpx/expedition/expedition.py
+drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-07 20:51:53.680651 gdpx-0.0.6/src/gdpx/expedition/ga/
+-rwxr-xr-x   0 jx1279   (353055) chem     (30004)    25925 2024-04-07 20:49:18.000000 gdpx-0.0.6/src/gdpx/expedition/ga/engine.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)    17387 2024-02-27 18:01:28.000000 gdpx-0.0.6/src/gdpx/expedition/ga/population.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     5346 2024-04-07 20:49:18.000000 gdpx-0.0.6/src/gdpx/expedition/interface.py
+drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-07 20:51:53.682651 gdpx-0.0.6/src/gdpx/expedition/monte_carlo/
+-rw-r--r--   0 jx1279   (353055) chem     (30004)      149 2024-04-07 20:49:18.000000 gdpx-0.0.6/src/gdpx/expedition/monte_carlo/__init__.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)      802 2024-04-07 20:49:18.000000 gdpx-0.0.6/src/gdpx/expedition/monte_carlo/basin_hopping.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)    18345 2024-04-07 20:49:18.000000 gdpx-0.0.6/src/gdpx/expedition/monte_carlo/monte_carlo.py
+drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-07 20:51:53.686651 gdpx-0.0.6/src/gdpx/expedition/monte_carlo/operators/
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     2356 2024-04-07 20:49:18.000000 gdpx-0.0.6/src/gdpx/expedition/monte_carlo/operators/__init__.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     9188 2024-04-07 20:49:18.000000 gdpx-0.0.6/src/gdpx/expedition/monte_carlo/operators/exchange.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     5008 2024-04-07 20:49:18.000000 gdpx-0.0.6/src/gdpx/expedition/monte_carlo/operators/move.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     8411 2024-04-07 20:49:18.000000 gdpx-0.0.6/src/gdpx/expedition/monte_carlo/operators/operator.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)    11096 2024-04-07 20:49:18.000000 gdpx-0.0.6/src/gdpx/expedition/monte_carlo/operators/react.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     4394 2024-04-07 20:49:18.000000 gdpx-0.0.6/src/gdpx/expedition/monte_carlo/operators/swap.py
+drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-07 20:51:53.686651 gdpx-0.0.6/src/gdpx/expedition/simulated_annealing/
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     5956 2024-04-07 20:49:18.000000 gdpx-0.0.6/src/gdpx/expedition/simulated_annealing/simulated_annealing.py
+drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-07 20:51:53.738651 gdpx-0.0.6/src/gdpx/graph/
+-rw-r--r--   0 jx1279   (353055) chem     (30004)      147 2024-03-17 21:29:29.000000 gdpx-0.0.6/src/gdpx/graph/__init__.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)    13870 2023-12-01 19:22:44.000000 gdpx-0.0.6/src/gdpx/graph/comparison.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)    12839 2024-03-17 21:29:29.000000 gdpx-0.0.6/src/gdpx/graph/creator.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)    12200 2023-12-01 19:22:44.000000 gdpx-0.0.6/src/gdpx/graph/graph_main.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     5142 2024-03-17 21:29:29.000000 gdpx-0.0.6/src/gdpx/graph/molecule.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)    31066 2024-03-17 21:29:29.000000 gdpx-0.0.6/src/gdpx/graph/sites.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     2905 2024-03-17 21:29:29.000000 gdpx-0.0.6/src/gdpx/graph/surface.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     1849 2023-12-01 19:22:44.000000 gdpx-0.0.6/src/gdpx/graph/utils.py
+-rwxr-xr-x   0 jx1279   (353055) chem     (30004)     8927 2024-04-07 20:49:18.000000 gdpx-0.0.6/src/gdpx/main.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     2242 2023-07-23 06:17:20.000000 gdpx-0.0.6/src/gdpx/nanoparticle.py
+drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-07 20:51:53.757650 gdpx-0.0.6/src/gdpx/potential/
+-rw-r--r--   0 jx1279   (353055) chem     (30004)      273 2024-03-17 21:29:29.000000 gdpx-0.0.6/src/gdpx/potential/__init__.py
+drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-07 20:51:53.758650 gdpx-0.0.6/src/gdpx/potential/calculators/
+-rw-r--r--   0 jx1279   (353055) chem     (30004)      654 2024-04-07 20:49:18.000000 gdpx-0.0.6/src/gdpx/potential/calculators/dummy.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     4675 2024-03-17 21:29:29.000000 gdpx-0.0.6/src/gdpx/potential/calculators/mixer.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     1256 2024-03-17 21:29:29.000000 gdpx-0.0.6/src/gdpx/potential/interface.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     5629 2024-04-07 20:49:18.000000 gdpx-0.0.6/src/gdpx/potential/manager.py
+drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-07 20:51:53.779650 gdpx-0.0.6/src/gdpx/potential/managers/
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     2977 2024-04-07 20:49:18.000000 gdpx-0.0.6/src/gdpx/potential/managers/__init__.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     1534 2024-04-07 20:49:18.000000 gdpx-0.0.6/src/gdpx/potential/managers/bias.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     2947 2024-03-02 03:59:21.000000 gdpx-0.0.6/src/gdpx/potential/managers/cp2k.py
+drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-07 20:51:53.782650 gdpx-0.0.6/src/gdpx/potential/managers/deepmd/
+-rw-r--r--   0 jx1279   (353055) chem     (30004)      225 2024-04-07 20:49:18.000000 gdpx-0.0.6/src/gdpx/potential/managers/deepmd/__init__.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     7170 2024-04-07 20:49:18.000000 gdpx-0.0.6/src/gdpx/potential/managers/deepmd/calculator.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     4058 2024-04-07 20:49:18.000000 gdpx-0.0.6/src/gdpx/potential/managers/deepmd/convert.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)    23429 2024-04-07 20:49:18.000000 gdpx-0.0.6/src/gdpx/potential/managers/deepmd/deepmd.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     1141 2024-04-07 20:49:18.000000 gdpx-0.0.6/src/gdpx/potential/managers/dftd3.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     2231 2024-03-02 03:59:21.000000 gdpx-0.0.6/src/gdpx/potential/managers/eam.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     1117 2024-03-02 03:59:21.000000 gdpx-0.0.6/src/gdpx/potential/managers/emt.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     2363 2024-03-02 03:59:21.000000 gdpx-0.0.6/src/gdpx/potential/managers/espresso.py
+drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-07 20:51:53.786650 gdpx-0.0.6/src/gdpx/potential/managers/gp/
+-rw-r--r--   0 jx1279   (353055) chem     (30004)       83 2024-03-02 03:59:21.000000 gdpx-0.0.6/src/gdpx/potential/managers/gp/__init__.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     2348 2024-03-02 03:59:21.000000 gdpx-0.0.6/src/gdpx/potential/managers/gp/bench.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     1376 2024-03-02 03:59:21.000000 gdpx-0.0.6/src/gdpx/potential/managers/gp/fgp.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     3746 2024-03-02 03:59:21.000000 gdpx-0.0.6/src/gdpx/potential/managers/gp/gptools.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     3474 2024-03-02 03:59:21.000000 gdpx-0.0.6/src/gdpx/potential/managers/gp/representation.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)    46869 2024-03-02 03:59:21.000000 gdpx-0.0.6/src/gdpx/potential/managers/gp/sgp.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     2715 2023-12-01 19:22:44.000000 gdpx-0.0.6/src/gdpx/potential/managers/grid.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     1986 2024-03-02 03:59:21.000000 gdpx-0.0.6/src/gdpx/potential/managers/lasp.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)    13122 2024-04-07 20:49:18.000000 gdpx-0.0.6/src/gdpx/potential/managers/mace.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     1840 2024-03-17 21:29:29.000000 gdpx-0.0.6/src/gdpx/potential/managers/mixer.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     7976 2024-03-17 21:29:29.000000 gdpx-0.0.6/src/gdpx/potential/managers/nequip.py
+drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-07 20:51:53.786650 gdpx-0.0.6/src/gdpx/potential/managers/plumed/
+drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-07 20:51:53.788650 gdpx-0.0.6/src/gdpx/potential/managers/plumed/calculators/
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     2728 2024-04-07 20:49:18.000000 gdpx-0.0.6/src/gdpx/potential/managers/plumed/calculators/plumed.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     9361 2024-04-07 20:49:18.000000 gdpx-0.0.6/src/gdpx/potential/managers/plumed/calculators/plumed2.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     2394 2024-04-07 20:49:18.000000 gdpx-0.0.6/src/gdpx/potential/managers/plumed/plumed.py
+drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-07 20:51:53.789650 gdpx-0.0.6/src/gdpx/potential/managers/reann/
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     7421 2024-03-17 21:29:29.000000 gdpx-0.0.6/src/gdpx/potential/managers/reann/beann.py
+drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-07 20:51:53.790650 gdpx-0.0.6/src/gdpx/potential/managers/reann/calculators/
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     3361 2024-03-17 21:29:29.000000 gdpx-0.0.6/src/gdpx/potential/managers/reann/calculators/reann.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)    17687 2024-04-07 20:49:18.000000 gdpx-0.0.6/src/gdpx/potential/managers/reann/reann.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     1396 2024-03-02 03:59:21.000000 gdpx-0.0.6/src/gdpx/potential/managers/reax.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     8903 2024-03-02 03:59:21.000000 gdpx-0.0.6/src/gdpx/potential/managers/schnet.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     3654 2024-03-02 03:59:21.000000 gdpx-0.0.6/src/gdpx/potential/managers/vasp.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     1207 2024-03-02 03:59:21.000000 gdpx-0.0.6/src/gdpx/potential/managers/xtb.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     5499 2024-04-07 20:49:18.000000 gdpx-0.0.6/src/gdpx/potential/trainer.py
+drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-07 20:51:53.804650 gdpx-0.0.6/src/gdpx/reactor/
+-rw-r--r--   0 jx1279   (353055) chem     (30004)      860 2024-04-07 20:49:18.000000 gdpx-0.0.6/src/gdpx/reactor/__init__.py
+drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-07 20:51:53.811650 gdpx-0.0.6/src/gdpx/reactor/future/
+-rw-r--r--   0 jx1279   (353055) chem     (30004)    23672 2023-12-01 19:22:44.000000 gdpx-0.0.6/src/gdpx/reactor/future/AccCons.py
+-rwxr-xr-x   0 jx1279   (353055) chem     (30004)    16224 2023-12-01 19:22:44.000000 gdpx-0.0.6/src/gdpx/reactor/future/AccHop.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     2601 2023-12-01 19:22:44.000000 gdpx-0.0.6/src/gdpx/reactor/future/AccNEB.py
+-rwxr-xr-x   0 jx1279   (353055) chem     (30004)     2921 2023-12-01 19:22:44.000000 gdpx-0.0.6/src/gdpx/reactor/future/cmp_mep.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     3833 2023-12-01 19:22:44.000000 gdpx-0.0.6/src/gdpx/reactor/future/constrain.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     7051 2023-12-01 19:22:44.000000 gdpx-0.0.6/src/gdpx/reactor/future/crs.py
+-rwxr-xr-x   0 jx1279   (353055) chem     (30004)     2226 2023-12-01 19:22:44.000000 gdpx-0.0.6/src/gdpx/reactor/future/diffusion3.py
+-rwxr-xr-x   0 jx1279   (353055) chem     (30004)    11410 2023-12-01 19:22:44.000000 gdpx-0.0.6/src/gdpx/reactor/future/find_adsorption.py
+-rwxr-xr-x   0 jx1279   (353055) chem     (30004)     3188 2023-12-01 19:22:44.000000 gdpx-0.0.6/src/gdpx/reactor/future/find_inter.py
+-rwxr-xr-x   0 jx1279   (353055) chem     (30004)     3002 2023-12-01 19:22:44.000000 gdpx-0.0.6/src/gdpx/reactor/future/muller-brown.py
+-rwxr-xr-x   0 jx1279   (353055) chem     (30004)     1154 2023-12-01 19:22:44.000000 gdpx-0.0.6/src/gdpx/reactor/future/test_mh.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     7056 2023-12-01 19:22:44.000000 gdpx-0.0.6/src/gdpx/reactor/interface.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     1482 2023-12-01 19:22:44.000000 gdpx-0.0.6/src/gdpx/reactor/reactor.py
+drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-07 20:51:53.818650 gdpx-0.0.6/src/gdpx/reactor/string/
+-rw-r--r--   0 jx1279   (353055) chem     (30004)      232 2023-12-01 19:22:44.000000 gdpx-0.0.6/src/gdpx/reactor/string/__init__.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)    17830 2024-03-17 21:29:29.000000 gdpx-0.0.6/src/gdpx/reactor/string/cp2k.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     5117 2024-03-17 21:29:29.000000 gdpx-0.0.6/src/gdpx/reactor/string/grid.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     9587 2024-04-07 20:49:18.000000 gdpx-0.0.6/src/gdpx/reactor/string/pathway.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)    11394 2024-04-07 20:49:18.000000 gdpx-0.0.6/src/gdpx/reactor/string/string.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     8168 2024-04-07 20:49:18.000000 gdpx-0.0.6/src/gdpx/reactor/string/vasp.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     2320 2024-04-07 20:49:18.000000 gdpx-0.0.6/src/gdpx/reactor/utils.py
+drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-07 20:51:53.822650 gdpx-0.0.6/src/gdpx/scheduler/
+-rw-r--r--   0 jx1279   (353055) chem     (30004)      699 2024-03-17 21:29:30.000000 gdpx-0.0.6/src/gdpx/scheduler/__init__.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)      624 2023-12-01 19:22:44.000000 gdpx-0.0.6/src/gdpx/scheduler/interface.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)      631 2024-03-17 21:29:30.000000 gdpx-0.0.6/src/gdpx/scheduler/local.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     3553 2024-03-17 21:29:30.000000 gdpx-0.0.6/src/gdpx/scheduler/lsf.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     1147 2024-03-17 21:29:30.000000 gdpx-0.0.6/src/gdpx/scheduler/pbs.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     4439 2024-03-17 21:29:30.000000 gdpx-0.0.6/src/gdpx/scheduler/scheduler.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     3226 2024-03-17 21:29:30.000000 gdpx-0.0.6/src/gdpx/scheduler/slurm.py
+drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-07 20:51:53.862649 gdpx-0.0.6/src/gdpx/selector/
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     1078 2024-04-07 20:49:18.000000 gdpx-0.0.6/src/gdpx/selector/__init__.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     3664 2024-03-17 21:29:30.000000 gdpx-0.0.6/src/gdpx/selector/basin.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     6276 2024-03-17 21:29:30.000000 gdpx-0.0.6/src/gdpx/selector/compare.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     1376 2024-03-17 21:29:30.000000 gdpx-0.0.6/src/gdpx/selector/composition.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     8362 2024-03-17 21:29:30.000000 gdpx-0.0.6/src/gdpx/selector/cur.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     7161 2024-04-07 20:49:18.000000 gdpx-0.0.6/src/gdpx/selector/descriptor.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     5631 2024-03-17 21:29:30.000000 gdpx-0.0.6/src/gdpx/selector/graph.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     6398 2024-04-07 20:49:18.000000 gdpx-0.0.6/src/gdpx/selector/interface.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     2905 2024-03-17 21:29:30.000000 gdpx-0.0.6/src/gdpx/selector/interval.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)      622 2024-03-17 21:29:30.000000 gdpx-0.0.6/src/gdpx/selector/invariant.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     3284 2024-03-17 21:29:30.000000 gdpx-0.0.6/src/gdpx/selector/locate.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)    11955 2024-03-17 21:29:30.000000 gdpx-0.0.6/src/gdpx/selector/property.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     1987 2024-03-17 21:29:30.000000 gdpx-0.0.6/src/gdpx/selector/random.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)      955 2024-04-07 20:49:18.000000 gdpx-0.0.6/src/gdpx/selector/scf.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)    10041 2024-04-07 20:49:18.000000 gdpx-0.0.6/src/gdpx/selector/selector.py
+drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-07 20:51:53.874649 gdpx-0.0.6/src/gdpx/trainer/
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     1050 2024-03-17 21:29:30.000000 gdpx-0.0.6/src/gdpx/trainer/__init__.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     6277 2024-03-17 21:29:30.000000 gdpx-0.0.6/src/gdpx/trainer/interface.py
+drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-07 20:51:53.901648 gdpx-0.0.6/src/gdpx/utils/
+-rw-r--r--   0 jx1279   (353055) chem     (30004)       83 2023-12-01 19:22:44.000000 gdpx-0.0.6/src/gdpx/utils/__init__.py
+-rwxr-xr-x   0 jx1279   (353055) chem     (30004)     7894 2023-12-01 19:22:44.000000 gdpx-0.0.6/src/gdpx/utils/atomUtils.py
+-rwxr-xr-x   0 jx1279   (353055) chem     (30004)     2908 2023-12-01 19:22:44.000000 gdpx-0.0.6/src/gdpx/utils/cleave_cluster.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     1247 2024-04-07 20:49:18.000000 gdpx-0.0.6/src/gdpx/utils/cmdrun.py
+-rwxr-xr-x   0 jx1279   (353055) chem     (30004)     6500 2023-12-01 19:22:44.000000 gdpx-0.0.6/src/gdpx/utils/cmp_refdat.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     6476 2024-04-07 20:49:18.000000 gdpx-0.0.6/src/gdpx/utils/command.py
+-rwxr-xr-x   0 jx1279   (353055) chem     (30004)    12328 2023-12-01 19:22:44.000000 gdpx-0.0.6/src/gdpx/utils/comparision.py
+drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-07 20:51:53.902649 gdpx-0.0.6/src/gdpx/utils/dputils/
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     9418 2023-12-01 19:22:44.000000 gdpx-0.0.6/src/gdpx/utils/dputils/DeepPot.py
+-rwxr-xr-x   0 jx1279   (353055) chem     (30004)    14661 2023-12-01 19:22:44.000000 gdpx-0.0.6/src/gdpx/utils/dputils/acquire_dmat.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     1095 2023-12-01 19:22:44.000000 gdpx-0.0.6/src/gdpx/utils/geometry.py
+-rwxr-xr-x   0 jx1279   (353055) chem     (30004)     2147 2023-12-01 19:22:44.000000 gdpx-0.0.6/src/gdpx/utils/plot_dimer.py
+-rwxr-xr-x   0 jx1279   (353055) chem     (30004)     7761 2023-12-01 19:22:44.000000 gdpx-0.0.6/src/gdpx/utils/reduce_dataset.py
+-rwxr-xr-x   0 jx1279   (353055) chem     (30004)     6200 2023-12-01 19:22:44.000000 gdpx-0.0.6/src/gdpx/utils/second_reduce.py
+-rwxr-xr-x   0 jx1279   (353055) chem     (30004)     5412 2024-03-17 21:29:30.000000 gdpx-0.0.6/src/gdpx/utils/split-dataset.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     2444 2024-04-07 20:49:18.000000 gdpx-0.0.6/src/gdpx/utils/strucopy.py
+drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-07 20:51:53.957648 gdpx-0.0.6/src/gdpx/validator/
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     1945 2023-12-01 19:22:44.000000 gdpx-0.0.6/src/gdpx/validator/__init__.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     5610 2024-03-17 21:29:30.000000 gdpx-0.0.6/src/gdpx/validator/diffusion_coefficient.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     4095 2024-04-07 20:49:18.000000 gdpx-0.0.6/src/gdpx/validator/dimer.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     2640 2024-03-17 21:29:30.000000 gdpx-0.0.6/src/gdpx/validator/eos.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     4779 2024-03-02 03:59:21.000000 gdpx-0.0.6/src/gdpx/validator/interface.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     5879 2024-03-17 21:29:30.000000 gdpx-0.0.6/src/gdpx/validator/mdf.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     7477 2024-03-17 21:29:30.000000 gdpx-0.0.6/src/gdpx/validator/melting_point.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     5744 2023-12-01 19:22:44.000000 gdpx-0.0.6/src/gdpx/validator/minima.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)      583 2023-12-01 19:22:44.000000 gdpx-0.0.6/src/gdpx/validator/rank.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     9391 2024-03-17 21:29:30.000000 gdpx-0.0.6/src/gdpx/validator/rdf.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     3436 2024-04-07 20:49:18.000000 gdpx-0.0.6/src/gdpx/validator/rxn.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     8794 2024-04-07 20:49:18.000000 gdpx-0.0.6/src/gdpx/validator/spc.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     3690 2023-12-01 19:22:44.000000 gdpx-0.0.6/src/gdpx/validator/surface_energy.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     2029 2023-12-01 19:22:44.000000 gdpx-0.0.6/src/gdpx/validator/utils.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)      980 2023-12-01 19:22:44.000000 gdpx-0.0.6/src/gdpx/validator/validator.py
+drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-07 20:51:53.976647 gdpx-0.0.6/src/gdpx/worker/
+-rw-r--r--   0 jx1279   (353055) chem     (30004)       84 2023-12-01 19:22:44.000000 gdpx-0.0.6/src/gdpx/worker/__init__.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)    31878 2024-04-07 20:49:18.000000 gdpx-0.0.6/src/gdpx/worker/drive.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     6935 2024-03-17 21:29:30.000000 gdpx-0.0.6/src/gdpx/worker/explore.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     7188 2023-12-01 19:22:44.000000 gdpx-0.0.6/src/gdpx/worker/grid.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)    11343 2024-03-17 21:29:30.000000 gdpx-0.0.6/src/gdpx/worker/interface.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)    18256 2023-12-01 19:22:44.000000 gdpx-0.0.6/src/gdpx/worker/react.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)    12738 2024-04-07 20:49:18.000000 gdpx-0.0.6/src/gdpx/worker/single.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)    11940 2024-03-17 21:29:30.000000 gdpx-0.0.6/src/gdpx/worker/train.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     1958 2023-12-01 19:22:44.000000 gdpx-0.0.6/src/gdpx/worker/utils.py
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     6077 2024-03-17 21:29:30.000000 gdpx-0.0.6/src/gdpx/worker/worker.py
+drwxr-xr-x   0 jx1279   (353055) chem     (30004)        0 2024-04-07 20:51:53.977647 gdpx-0.0.6/src/gdpx.egg-info/
+-rw-r--r--   0 jx1279   (353055) chem     (30004)    47663 2024-04-07 20:51:53.000000 gdpx-0.0.6/src/gdpx.egg-info/PKG-INFO
+-rw-r--r--   0 jx1279   (353055) chem     (30004)     8166 2024-04-07 20:51:53.000000 gdpx-0.0.6/src/gdpx.egg-info/SOURCES.txt
+-rw-r--r--   0 jx1279   (353055) chem     (30004)        1 2024-04-07 20:51:53.000000 gdpx-0.0.6/src/gdpx.egg-info/dependency_links.txt
+-rw-r--r--   0 jx1279   (353055) chem     (30004)       39 2024-04-07 20:51:53.000000 gdpx-0.0.6/src/gdpx.egg-info/entry_points.txt
+-rw-r--r--   0 jx1279   (353055) chem     (30004)      111 2024-04-07 20:51:53.000000 gdpx-0.0.6/src/gdpx.egg-info/requires.txt
+-rw-r--r--   0 jx1279   (353055) chem     (30004)        5 2024-04-07 20:51:53.000000 gdpx-0.0.6/src/gdpx.egg-info/top_level.txt
```

### Comparing `gdpx-0.0.5/LICENSE` & `gdpx-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.5/PKG-INFO` & `gdpx-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gdpx
-Version: 0.0.5
+Version: 0.0.6
 Summary: Automate computational chemistry/materials sciance and machine learning interatomic potential training workflow.
 Author-email: Jiayan Xu <ahcigar@foxmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `gdpx-0.0.5/README.md` & `gdpx-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.5/pyproject.toml` & `gdpx-0.0.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gdpx"
-version = "0.0.5"
+version = "0.0.6"
 dependencies = [
   "ase>=3.22",
   "h5py>=3.7.0",
   "joblib>=1.1.0",
   "networkx>=2.6.3",
   "omegaconf>=2.3.0",
   "pydantic>=2.1.1",
```

### Comparing `gdpx-0.0.5/src/gdpx/bias/__init__.py` & `gdpx-0.0.6/src/gdpx/bias/__init__.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.5/src/gdpx/bias/afir.py` & `gdpx-0.0.6/src/gdpx/bias/afir.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.5/src/gdpx/bias/bias.py` & `gdpx-0.0.6/src/gdpx/bias/bias.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.5/src/gdpx/bias/gaussian.py` & `gdpx-0.0.6/src/gdpx/bias/gaussian.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.5/src/gdpx/bias/harmonic.py` & `gdpx-0.0.6/src/gdpx/bias/harmonic.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.5/src/gdpx/bias/nuclei.py` & `gdpx-0.0.6/src/gdpx/bias/nuclei.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.5/src/gdpx/builder/__init__.py` & `gdpx-0.0.6/src/gdpx/builder/__init__.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.5/src/gdpx/builder/builder.py` & `gdpx-0.0.6/src/gdpx/builder/builder.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.5/src/gdpx/builder/cleave_group.py` & `gdpx-0.0.6/src/gdpx/builder/cleave_group.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.5/src/gdpx/builder/cleave_surface.py` & `gdpx-0.0.6/src/gdpx/builder/cleave_surface.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.5/src/gdpx/builder/constraints.py` & `gdpx-0.0.6/src/gdpx/builder/constraints.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.5/src/gdpx/builder/dimer.py` & `gdpx-0.0.6/src/gdpx/builder/dimer.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.5/src/gdpx/builder/direct.py` & `gdpx-0.0.6/src/gdpx/builder/direct.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.5/src/gdpx/builder/graph/exchange.py` & `gdpx-0.0.6/src/gdpx/builder/graph/exchange.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.5/src/gdpx/builder/graph/insert.py` & `gdpx-0.0.6/src/gdpx/builder/graph/insert.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.5/src/gdpx/builder/graph/modifier.py` & `gdpx-0.0.6/src/gdpx/builder/graph/modifier.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.5/src/gdpx/builder/graph/remove.py` & `gdpx-0.0.6/src/gdpx/builder/graph/remove.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.5/src/gdpx/builder/group.py` & `gdpx-0.0.6/src/gdpx/builder/group.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.5/src/gdpx/builder/hypercube.py` & `gdpx-0.0.6/src/gdpx/builder/hypercube.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.5/src/gdpx/builder/insert.py` & `gdpx-0.0.6/src/gdpx/builder/insert.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.5/src/gdpx/builder/interface.py` & `gdpx-0.0.6/src/gdpx/builder/interface.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.5/src/gdpx/builder/mutation/__init__.py` & `gdpx-0.0.6/src/gdpx/builder/mutation/__init__.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.5/src/gdpx/builder/packer.py` & `gdpx-0.0.6/src/gdpx/builder/packer.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.5/src/gdpx/builder/perturbator.py` & `gdpx-0.0.6/src/gdpx/builder/perturbator.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.5/src/gdpx/builder/randomBuilder.py` & `gdpx-0.0.6/src/gdpx/builder/randomBuilder.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.5/src/gdpx/builder/region.py` & `gdpx-0.0.6/src/gdpx/builder/region.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.5/src/gdpx/builder/repeat.py` & `gdpx-0.0.6/src/gdpx/builder/repeat.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.5/src/gdpx/builder/species.py` & `gdpx-0.0.6/src/gdpx/builder/species.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.5/src/gdpx/builder/utils.py` & `gdpx-0.0.6/src/gdpx/builder/utils.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.5/src/gdpx/builder/zoom.py` & `gdpx-0.0.6/src/gdpx/builder/zoom.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.5/src/gdpx/colvar/compute_reweight.py` & `gdpx-0.0.6/src/gdpx/colvar/compute_reweight.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.5/src/gdpx/colvar/coordination.py` & `gdpx-0.0.6/src/gdpx/colvar/coordination.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.5/src/gdpx/colvar/distance.py` & `gdpx-0.0.6/src/gdpx/colvar/distance.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.5/src/gdpx/colvar/fingerprint.py` & `gdpx-0.0.6/src/gdpx/colvar/fingerprint.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.5/src/gdpx/colvar/plot_meta.py` & `gdpx-0.0.6/src/gdpx/colvar/plot_meta.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.5/src/gdpx/colvar/plot_string.py` & `gdpx-0.0.6/src/gdpx/colvar/plot_string.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.5/src/gdpx/colvar/plotstring.py` & `gdpx-0.0.6/src/gdpx/colvar/plotstring.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.5/src/gdpx/colvar/reweight.py` & `gdpx-0.0.6/src/gdpx/colvar/reweight.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.5/src/gdpx/colvar/rmsd.py` & `gdpx-0.0.6/src/gdpx/colvar/rmsd.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.5/src/gdpx/comparator/__init__.py` & `gdpx-0.0.6/src/gdpx/comparator/__init__.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.5/src/gdpx/comparator/cartesian.py` & `gdpx-0.0.6/src/gdpx/comparator/cartesian.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.5/src/gdpx/comparator/comparator.py` & `gdpx-0.0.6/src/gdpx/comparator/comparator.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.5/src/gdpx/comparator/coordination.py` & `gdpx-0.0.6/src/gdpx/comparator/coordination.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.5/src/gdpx/comparator/graph.py` & `gdpx-0.0.6/src/gdpx/comparator/graph.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.5/src/gdpx/comparator/interface.py` & `gdpx-0.0.6/src/gdpx/comparator/interface.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.5/src/gdpx/comparator/reaction.py` & `gdpx-0.0.6/src/gdpx/comparator/reaction.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.5/src/gdpx/comparator/singlepoint.py` & `gdpx-0.0.6/src/gdpx/comparator/singlepoint.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.5/src/gdpx/computation/__init__.py` & `gdpx-0.0.6/src/gdpx/computation/__init__.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.5/src/gdpx/computation/asedriver.py` & `gdpx-0.0.6/src/gdpx/computation/asedriver.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,45 +1,65 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
-import os
+
 import copy
 import dataclasses
 import io
-import shutil
 import pathlib
 import tarfile
 import traceback
-from typing import NoReturn, List, Tuple
+from typing import Optional, List, Tuple
 import warnings
 
 import numpy as np
 
+import yaml
+
 from ase import Atoms
 from ase import units
 
 from ase.io import read, write
 import ase.constraints
-from ase.constraints import Filter, FixAtoms
+from ase.constraints import Filter
 from ase.optimize.optimize import Dynamics
 from ase.md.velocitydistribution import (
     MaxwellBoltzmannDistribution,
     Stationary,
     ZeroRotation,
 )
 
+from ase.calculators.calculator import Calculator
 from ase.calculators.singlepoint import SinglePointCalculator
 
 from .. import config as GDPCONFIG
-from ..builder.constraints import parse_constraint_info
-from .driver import AbstractDriver, DriverSetting
-from .md.md_utils import force_temperature
 from ..potential.calculators.mixer import EnhancedCalculator
+from .driver import AbstractDriver, DriverSetting, Controller
+from .md.md_utils import force_temperature
+
+
+def set_calc_state(calc: Calculator, timestep: float, stride: int):
+    """Some calculators need driver information e.g. PLUMED."""
+    if calc.name == "plumed":
+        calc.timestep = timestep
+        calc.stride = stride
+    if hasattr(calc, "calcs"):
+        for subcalc in calc.calcs:
+            set_calc_state(subcalc, timestep, stride)
+    else:
+        ...
+
+    return
+
 
-from .plumed import set_plumed_state
+def update_atoms_info(atoms: Atoms, dyn: Dynamics, start_step: int = 0) -> None:
+    """Update step in atoms.info."""
+    atoms.info["step"] = dyn.nsteps + start_step
+
+    return
 
 
 def retrieve_and_save_deviation(atoms, devi_fpath) -> None:
     """Read model deviation and add results to atoms.info if the file exists."""
     results = copy.deepcopy(atoms.calc.results)
     # devi_results = [(k,v) for k,v in results.items() if "devi" in k]
     devi_results = [
@@ -85,14 +105,17 @@
         atoms_to_save.set_momenta(atoms.get_momenta())
     results = dict(
         energy=atoms.get_potential_energy(), forces=copy.deepcopy(atoms.get_forces())
     )
     spc = SinglePointCalculator(atoms, **results)
     atoms_to_save.calc = spc
 
+    # - save atoms info...
+    atoms_to_save.info["step"] = atoms.info["step"]
+
     # - save special keys and arrays from calc
     natoms = len(atoms)
 
     # -- add deviation
     for k, v in atoms.calc.results.items():
         if k in GDPCONFIG.VALID_DEVI_FRAME_KEYS:
             atoms_to_save.info[k] = v
@@ -112,77 +135,202 @@
 
     # - append to traj
     write(log_fpath, atoms_to_save, append=True)
 
     return
 
 
+def save_checkpoint(
+    dyn: Dynamics, atoms: Atoms, wdir: pathlib.Path, start_step: int = 0
+):
+    """"""
+    ckpt_wdir = wdir / f"checkpoint.{dyn.nsteps+start_step}"
+    ckpt_wdir.mkdir(parents=True, exist_ok=True)
+
+    # write(ckpt_wdir/"structure.xyz", atoms)
+    save_trajectory(atoms=atoms, log_fpath=ckpt_wdir / "structures.xyz")
+
+    # For some optimisers and dynamics, they use random generator.
+    if hasattr(dyn, "rng"):
+        with open(ckpt_wdir / "rng_state.yaml", "w") as fopen:
+            yaml.safe_dump(dyn.rng.bit_generator.state, fopen)
+
+    # For some mixed calculator, save information, for example, PLUMED...
+    if hasattr(atoms.calc, "calcs"):
+        for calc in atoms.calc.calcs:
+            if hasattr(calc, "_save_checkpoint"):
+                calc._save_checkpoint(ckpt_wdir)
+
+    return
+
+
+@dataclasses.dataclass
+class BerendsenThermostat(Controller):
+
+    name: str = "berendsen"
+
+    def __post_init__(
+        self,
+    ):
+        """"""
+        taut = self.params.get("Tdamp", 100.0)
+        assert taut is not None
+
+        self.conv_params = dict(taut=taut * units.fs)
+
+        return
+
+
+@dataclasses.dataclass
+class LangevinThermostat(Controller):
+
+    name: str = "langevin"
+
+    def __post_init__(
+        self,
+    ):
+        """"""
+        friction = self.params.get("friction", None)  # fs^-1
+        assert friction is not None
+
+        self.conv_params = dict(
+            friction=friction / units.fs,
+            # NOTE: The rng that generates friction normal distribution
+            #       is set in `create_dynamics` by the driver's random_seed
+            rng=None,
+        )
+
+        return
+
+
+@dataclasses.dataclass
+class NoseHooverThermostat(Controller):
+
+    name: str = "nosehoover"
+
+    def __post_init__(
+        self,
+    ):
+        """"""
+        nvt_q = self.params.get("nvt_q", None)
+        assert nvt_q is not None
+
+        self.conv_params = dict(nvt_q=nvt_q)  # thermostat mass
+
+        return
+
+
+@dataclasses.dataclass
+class BerendsenBarostat(Controller):
+
+    name: str = "berendsen"
+
+    def __post_init__(
+        self,
+    ):
+        """"""
+        taut = self.params.get("Tdamp", 100.0)  # fs
+        assert taut is not None
+
+        taup = self.params.get("Pdamp", 100.0)  # fs
+        assert taup is not None
+
+        compressibility = self.params.get("compressibility", 4.57e-5)  # bar^-1
+
+        self.conv_params = dict(
+            taut=taut * units.fs,
+            taup=taup * units.fs,
+            compressibility_au=compressibility / units.bar,
+        )
+
+        return
+
+
+controllers = dict(
+    # - nvt
+    berendsen_nvt=BerendsenThermostat,
+    langevin_nvt=LangevinThermostat,
+    nosehoover_nvt=NoseHooverThermostat,
+    # - npt
+    berendsen_npt=BerendsenBarostat,
+)
+
+
 @dataclasses.dataclass
 class AseDriverSetting(DriverSetting):
 
-    driver_cls: Dynamics = None
-    filter_cls: Filter = None
+    driver_cls: Optional[Dynamics] = None
+    filter_cls: Optional[Filter] = None
 
-    thermostat: str = None
-    friction: float = 0.01
-    friction_seed: int = None
+    ensemble: str = "nve"
+
+    controller: dict = dataclasses.field(default_factory=dict)
 
     fix_cm: bool = False
 
     fmax: float = 0.05  # eV/Ang
 
     def __post_init__(self):
         """"""
         # - task-specific params
         if self.task == "md":
             self._internals.update(
                 # - helper params
                 velocity_seed=self.velocity_seed,
                 ignore_atoms_velocities=self.ignore_atoms_velocities,
-                md_style=self.md_style,  # ensemble...
-                thermostat=self.thermostat,
-                # -
-                fixcm=self.fix_cm,
-                timestep=self.timestep,
-                temperature_K=self.temp,
-                taut=self.Tdamp,
-                pressure=self.press,
-                taup=self.Pdamp,
             )
-            # TODO: provide a unified class for thermostat
-            if self.md_style == "nve":
+            if self.ensemble == "nve":
                 from ase.md.verlet import VelocityVerlet as driver_cls
-            elif self.md_style == "nvt":
-                thermostat = (
-                    self.thermostat if self.thermostat is not None else "berendsen"
+
+                _init_md_params = dict(
+                    timestep=self.timestep * units.fs,
                 )
-                if thermostat == "berendsen":
+            elif self.ensemble == "nvt":
+                if self.controller:
+                    thermo_cls_name = self.controller["name"] + "_" + self.ensemble
+                    thermo_cls = controllers[thermo_cls_name]
+                else:
+                    thermo_cls = BerendsenThermostat
+                thermostat = thermo_cls(**self.controller)
+                if thermostat.name == "berendsen":
                     from ase.md.nvtberendsen import NVTBerendsen as driver_cls
-
-                    thermostat_params = dict(taut=self._internals["taut"])
-                elif thermostat == "langevin":
+                elif thermostat.name == "langevin":
                     from ase.md.langevin import Langevin as driver_cls
-
-                    if self.friction_seed is not None:
-                        friction_seed = self.friction_seed
-                    else:
-                        friction_seed = np.random.randint(0, 100000000)
-                    thermostat_params = dict(
-                        friction=self.friction / units.fs,
-                        # TODO: use driver's seed instead!
-                        rng=np.random.default_rng(seed=friction_seed),
-                    )
-                elif thermostat == "nose_hoover":
+                elif thermostat.name == "nose_hoover":
                     from .md.nosehoover import NoseHoover as driver_cls
                 else:
                     raise RuntimeError(f"Unknown thermostat {thermostat}.")
-                self._internals["thermostat"] = thermostat
-                self._internals["thermostat_params"] = thermostat_params
-            elif self.md_style == "npt":
-                from ase.md.nptberendsen import NPTBerendsen as driver_cls
+                thermo_params = thermostat.conv_params
+                _init_md_params = dict(
+                    fixcm=self.fix_cm,
+                    timestep=self.timestep * units.fs,
+                    temperature_K=self.temp,
+                )
+                _init_md_params.update(**thermo_params)
+            elif self.ensemble == "npt":
+                if self.controller:
+                    baro_cls_name = self.controller["name"] + "_" + self.ensemble
+                    baro_cls = controllers[baro_cls_name]
+                else:
+                    baro_cls = BerendsenBarostat
+                barostat = baro_cls(**self.controller)
+                if barostat.name == "berendsen":
+                    from ase.md.nptberendsen import NPTBerendsen as driver_cls
+                else:
+                    raise RuntimeError(f"Unknown barostat {barostat}.")
+                baro_params = barostat.conv_params
+                _init_md_params = dict(
+                    fixcm=self.fix_cm,
+                    timestep=self.timestep * units.fs,
+                    temperature_K=self.temp,
+                    pressure_au=self.press * (1e5 * units.Pascal),
+                )
+                _init_md_params.update(**baro_params)
+
+            self._internals.update(**_init_md_params)
 
         if self.task == "min":
             # - to opt atomic positions
             from ase.optimize import BFGS
 
             if self.min_style == "bfgs":
                 driver_cls = BFGS
@@ -275,118 +423,86 @@
         super(AseDriver, AseDriver).directory.__set__(self, directory_)
 
         # - other files
         self._log_fpath = self.directory / self.log_fname
 
         return
 
-    def _create_dynamics(self, atoms, *args, **kwargs) -> Tuple[Dynamics, dict]:
+    def _create_dynamics(self, atoms: Atoms, *args, **kwargs) -> Tuple[Dynamics, dict]:
         """Create the correct class of this simulation with running parameters.
 
         Respect `steps` and `fmax` as restart.
 
         """
         # - overwrite
         run_params = self.setting.get_run_params(*args, **kwargs)
 
-        # NOTE: if have cons in kwargs overwrite current cons stored in atoms
-        cons_text = run_params.pop("constraint", None)
-        if cons_text is not None:
-            atoms._del_constraints()
-            mobile_indices, frozen_indices = parse_constraint_info(
-                atoms, cons_text, ignore_ase_constraints=True, ret_text=False
-            )
-            if frozen_indices:
-                atoms.set_constraint(FixAtoms(indices=frozen_indices))
+        # -
+        self._preprocess_constraints(atoms, run_params)
 
         # - init driver
         if self.setting.task == "min":
             if self.setting.filter_cls:
                 atoms = self.setting.filter_cls(atoms)
             driver = self.setting.driver_cls(
                 atoms, logfile=self.log_fpath, trajectory=None
             )
         elif self.setting.task == "ts":
             driver = self.setting.driver_cls(
                 atoms, order=1, internal=False, logfile=self.log_fpath, trajectory=None
             )
         elif self.setting.task == "md":
             # - adjust params
-            init_params_ = copy.deepcopy(self.setting.get_init_params())
-            # NOTE: every dynamics will have a new rng...
-            self._print(f"MD Driver's random_seed: {self.random_seed}")
-            rng = np.random.default_rng(self.random_seed)
+            init_params_ = self.setting.get_init_params()
 
             # - velocity
-            if (
-                not init_params_["ignore_atoms_velocities"]
-                and atoms.get_kinetic_energy() > 0.0
-            ):
+            # NOTE: every dynamics will have a new rng...
+            velocity_seed = init_params_.pop("velocity_seed")
+            if velocity_seed is None:
+                self._print(f"MD Driver's velocity_seed: {self.random_seed}")
+                vrng = np.random.Generator(np.random.PCG64(self.random_seed))
+            else:
+                self._print(f"MD Driver's velocity_seed: {velocity_seed}")
+                # vrng = np.random.default_rng(velocity_seed)
+                vrng = np.random.Generator(np.random.PCG64(velocity_seed))
+
+            ignore_atoms_velocities = init_params_.pop("ignore_atoms_velocities")
+            if not ignore_atoms_velocities and atoms.get_kinetic_energy() > 0.0:
                 # atoms have momenta
                 ...
             else:
                 MaxwellBoltzmannDistribution(
-                    atoms, temperature_K=init_params_["temperature_K"], rng=rng
+                    atoms, temperature_K=init_params_["temperature_K"], rng=vrng
                 )
                 if self.setting.remove_rotation:
                     ZeroRotation(atoms, preserve_temperature=False)
                 if self.setting.remove_translation:
                     Stationary(atoms, preserve_temperature=False)
                 # NOTE: respect constraints
                 #       ase code does not consider constraints
                 force_temperature(atoms, init_params_["temperature_K"], unit="K")
 
-            # - prepare args
-            # TODO: move this part to setting post_init?
-            md_style = init_params_.pop("md_style")
-            if md_style == "nve":
-                init_params_ = {
-                    k: v
-                    for k, v in init_params_.items()
-                    if k in ["loginterval", "timestep"]
-                }
-            elif md_style == "nvt":
-                init_params_ = {
-                    k: v
-                    for k, v in init_params_.items()
-                    if k in ["loginterval", "fixcm", "timestep", "temperature_K"]
-                }
-                init_params_.update(**self.setting._internals["thermostat_params"])
-            elif md_style == "npt":
-                init_params_ = {
-                    k: v
-                    for k, v in init_params_.items()
-                    if k
-                    in [
-                        "loginterval",
-                        "fixcm",
-                        "timestep",
-                        "temperature_K",
-                        "taut",
-                        "pressure",
-                        "taup",
-                    ]
-                }
-                init_params_["pressure"] *= 1.0 / (160.21766208 / 0.000101325)
-
-            init_params_["timestep"] *= units.fs
+            # - some dynamics need rng
+            if "rng" in init_params_:
+                self._print(f"MD Driver's rng: {self.rng.bit_generator.state}")
+                init_params_["rng"] = self.rng
 
-            # NOTE: plumed
-            set_plumed_state(
+            # - other callbacks
+            set_calc_state(
                 self.calc,
                 timestep=init_params_["timestep"],
                 stride=init_params_["loginterval"],
             )
 
             # - construct the driver
             driver = self.setting.driver_cls(
                 atoms=atoms, **init_params_, logfile=self.log_fpath, trajectory=None
             )
         else:
-            raise NotImplementedError(f"Unknown task {self.task}.")
+            raise NotImplementedError(f"Unknown task {self.setting.task}.")
 
         return driver, run_params
 
     def _verify_checkpoint(self, *args, **kwargs) -> bool:
         """"""
         verified = super()._verify_checkpoint()
         if verified:
@@ -400,89 +516,143 @@
             else:
                 verified = False
         else:
             ...
 
         return verified
 
-    def _irun(self, atoms: Atoms, ckpt_wdir=None, *args, **kwargs):
+    def _find_latest_checkpoint(self, wdir: pathlib.Path):
+        """"""
+        ckpt_dirs = sorted(
+            wdir.glob("checkpoint.*"), key=lambda x: int(x.name.split(".")[-1])
+        )
+        latest_ckpt_dir = ckpt_dirs[-1]
+
+        return latest_ckpt_dir
+
+    def _load_checkpoint(self, ckpt_dir: pathlib.Path):
+        """"""
+        atoms = read(ckpt_dir / "structures.xyz", ":")[-1]
+
+        rng_state_fpath = ckpt_dir / "rng_state.yaml"
+        if rng_state_fpath.exists():
+            with open(ckpt_dir / "rng_state.yaml", "r") as fopen:
+                rng_state = yaml.safe_load(fopen)
+        else:
+            rng_state = None
+
+        return atoms, rng_state
+
+    def _irun(
+        self,
+        atoms: Atoms,
+        ckpt_wdir=None,
+        cache_traj: List[Atoms] = None,
+        *args,
+        **kwargs,
+    ):
         """Run the simulation."""
+        prev_wdir = ckpt_wdir
         try:
             # To restart, velocities are always retained
             prev_ignore_atoms_velocities = self.setting.ignore_atoms_velocities
-            if ckpt_wdir is None:  # start from the scratch
+            if prev_wdir is None:  # start from the scratch
+                start_step = 0
+                rng_state = None
+
                 curr_params = {}
                 curr_params["random_seed"] = self.random_seed
                 curr_params["init"] = self.setting.get_init_params()
-                if self.setting.task == "md":  # check rng for MD simulations...
-                    if "rng" in curr_params["init"]["thermostat_params"]:  # langevin...
-                        rng = curr_params["init"]["thermostat_params"]["rng"]
-                        curr_params["init"]["thermostat_params"][
-                            "rng"
-                        ] = rng._bit_generator.state
-                else:
-                    ...
                 curr_params["run"] = self.setting.get_run_params()
-                import yaml
 
                 with open(self.directory / "params.yaml", "w") as fopen:
                     yaml.safe_dump(curr_params, fopen, indent=2)
             else:  # restart ...
-                traj = self.read_trajectory()
-                nframes = len(traj)
-                assert nframes > 0, "AseDriver restarts with a zero-frame trajectory."
-                atoms = traj[-1]
+                ckpt_wdir = self._find_latest_checkpoint(prev_wdir)
+                atoms, rng_state = self._load_checkpoint(ckpt_wdir)
+                start_step = atoms.info["step"]
+                if hasattr(self.calc, "calcs"):
+                    for calc in self.calc.calcs:
+                        if hasattr(calc, "_load_checkpoint"):
+                            calc._load_checkpoint(ckpt_wdir, start_step=start_step)
                 # --- update run_params in settings
-                dump_period = self.setting.get_init_params()["loginterval"]
                 target_steps = self.setting.get_run_params(*args, **kwargs)["steps"]
                 if target_steps > 0:
-                    steps = target_steps + dump_period - nframes * dump_period
+                    steps = target_steps - start_step
                 assert steps > 0, "Steps should be greater than 0."
                 kwargs.update(steps=steps)
 
                 # To restart, velocities are always retained
                 self.setting.ignore_atoms_velocities = False
 
             # - set calculator
             atoms.calc = self.calc
 
             # - set dynamics
             dynamics, run_params = self._create_dynamics(atoms, *args, **kwargs)
-
+            # dynamics.nsteps = start_step
+            if hasattr(dynamics, "rng") and rng_state is not None:
+                dynamics.rng.bit_generator.state = rng_state
+
+            # --- callback functions
+            dynamics.insert_observer(
+                update_atoms_info,
+                dyn=dynamics,
+                atoms=atoms,
+                start_step=start_step,
+            )
             # NOTE: traj file not stores properties (energy, forces) properly
             init_params = self.setting.get_init_params()
             dynamics.attach(
+                save_checkpoint,
+                interval=self.setting.ckpt_period,
+                dyn=dynamics,
+                atoms=atoms,
+                wdir=self.directory,
+                start_step=start_step,
+            )
+            dynamics.attach(
                 save_trajectory,
                 interval=init_params["loginterval"],
                 atoms=atoms,
                 log_fpath=self.directory / self.xyz_fname,
             )
             # NOTE: retrieve deviation info
             dynamics.attach(
                 retrieve_and_save_deviation,
                 interval=init_params["loginterval"],
                 atoms=atoms,
                 devi_fpath=self.directory / self.devi_fname,
             )
             dynamics.run(**run_params)
+
             # NOTE: check if the last frame is properly stored
-            loginterval = init_params["loginterval"]
-            if loginterval > 1:
+            dump_period = self.setting.dump_period
+            assert init_params["loginterval"] == dump_period
+
+            if dump_period > 1:
+                should_dump_last = False
                 if self.setting.task == "min":
-                    data = np.loadtxt(self.directory/"dyn.log", dtype=str, skiprows=1)
+                    # optimiser dumps every step to log...
+                    data = np.loadtxt(self.directory / "dyn.log", dtype=str, skiprows=1)
                     if len(data.shape) == 1:
-                        data = data[np.newaxis,:]
+                        data = data[np.newaxis, :]
                     nsteps = data.shape[0]
-                    if nsteps > 0 and (nsteps - 1) % loginterval != 0:
-                        save_trajectory(atoms, self.directory / self.xyz_fname)
-                        retrieve_and_save_deviation(
-                            atoms, self.directory / self.devi_fname
-                        )
-                else:  # TODO: If MD breaks due to some errors?
-                    ...
+                    if nsteps > 0 and (nsteps - 1) % dump_period != 0:
+                        should_dump_last = True
+                elif self.setting.task == "md":
+                    if dump_period > self.setting.steps:
+                        should_dump_last = True
+                if should_dump_last:
+                    update_atoms_info(atoms, dynamics, start_step=start_step)
+                    save_checkpoint(
+                        dynamics, atoms, self.directory, start_step=start_step
+                    )
+                    save_trajectory(atoms, self.directory / self.xyz_fname)
+                    retrieve_and_save_deviation(atoms, self.directory / self.devi_fname)
             else:
                 ...
 
             # - Some interactive calculator needs kill processes after finishing,
             #   e.g. VaspInteractive...
             if hasattr(self.calc, "finalize"):
                 self.calc.finalize()
@@ -522,61 +692,40 @@
     def _read_a_single_trajectory(
         self, wdir: pathlib.Path, archive_path: pathlib.Path = None, *args, **kwargs
     ):
         """"""
         self._debug(f"archive_path: {archive_path}")
         self._debug(f"wdir: {wdir}")
         if archive_path is None:
-            frames = read(wdir / self.xyz_fname, ":")  # TODO: check traj existence?
+            if (wdir / self.xyz_fname).exists():
+                frames = read(wdir / self.xyz_fname, ":")
+            else:
+                frames = []
         else:
             target_name = str(
                 (wdir / self.xyz_fname).relative_to(self.directory.parent)
             )
             with tarfile.open(archive_path, "r:gz") as tar:
                 for tarinfo in tar:
                     if tarinfo.name == target_name:
                         fobj = io.StringIO(
                             tar.extractfile(tarinfo.name).read().decode()
                         )
                         frames = read(fobj, ":", format="extxyz")
                         fobj.close()
                         break
-                else:  # TODO: if not find target traj?
-                    ...
+                else:
+                    frames = []
 
         return frames
 
     def read_trajectory(self, archive_path=None, *args, **kwargs) -> List[Atoms]:
         """Read trajectory in the current working directory."""
-        # -
-        prev_wdirs = sorted(self.directory.glob(r"[0-9][0-9][0-9][0-9][.]run"))
-        self._debug(f"prev_wdirs: {prev_wdirs}")
-
-        traj_list = []
-        for w in prev_wdirs:
-            curr_frames = self._read_a_single_trajectory(w, archive_path=archive_path)
-            traj_list.append(curr_frames)
-
-        # Even though xyz file may be empty, the read can give a empty list...
-        curr_frames = self._read_a_single_trajectory(
-            self.directory, archive_path=archive_path
-        )
-        traj_list.append(curr_frames)
-
-        # -- concatenate
-        traj_frames, ntrajs = [], len(traj_list)
-        if ntrajs > 0:
-            traj_frames.extend(traj_list[0])
-            for i in range(1, ntrajs):
-                assert np.allclose(
-                    traj_list[i - 1][-1].positions, traj_list[i][0].positions
-                ), f"Traj {i-1} and traj {i} are not consecutive."
-                traj_frames.extend(traj_list[i][1:])
-        else:
-            ...
+        # - read trajectory
+        traj_frames = self._aggregate_trajectories(archive_path=archive_path)
 
         # - add some info
         init_params = self.setting.get_init_params()
         if self.setting.task == "md":
             # Time[ps]      Etot[eV]     Epot[eV]     Ekin[eV]    T[K]
             # 0.0000           3.4237       2.8604       0.5633   272.4
             # data = np.loadtxt(self.directory/"dyn.log", dtype=float, skiprows=1)
@@ -598,16 +747,14 @@
             # steps = [int(s) for s in data[:, 1]]
             # fmaxs = [float(fmax) for fmax in data[:, 4]]
             for atoms in traj_frames:
                 atoms.info["fmax"] = np.max(
                     np.fabs(atoms.get_forces(apply_constraint=True))
                 )
         # assert len(steps) == len(traj_frames), f"Number of steps {len(steps)} and number of frames {len(traj_frames)} are inconsistent..."
-        for step, atoms in enumerate(traj_frames):
-            atoms.info["step"] = int(step) * init_params["loginterval"]
 
         # - deviation stored in traj, no need to read from file
 
         nframes = len(traj_frames)
 
         # calculation happens but some errors in calculation
         if self.directory.exists():
```

### Comparing `gdpx-0.0.5/src/gdpx/computation/cp2k.py` & `gdpx-0.0.6/src/gdpx/computation/cp2k.py`

 * *Files 0% similar despite different names*

```diff
@@ -101,15 +101,15 @@
         steps, frame_symbols, boxes, frame_positions, frame_energies, frame_forces
     ):
         atoms = Atoms(
             symbols, positions=positions,
             cell=box.reshape(3,3), 
             pbc=[1,1,1] # TODO: should determine in the cp2k input file
         )
-        atoms.info["step"] = step
+        atoms.info["step"] = int(step)
         spc = SinglePointCalculator(
             atoms=atoms, energy=energy, 
             free_energy=energy, # TODO: depand on electronic method used
             forces=forces
         )
         atoms.calc = spc
         frames.append(atoms)
```

### Comparing `gdpx-0.0.5/src/gdpx/computation/dpx.py` & `gdpx-0.0.6/src/gdpx/potential/managers/deepmd/calculator.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.5/src/gdpx/computation/driver.py` & `gdpx-0.0.6/src/gdpx/computation/driver.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 import abc
 import copy
 import dataclasses
 import pathlib
 import re
 import shutil
+import tarfile
 import warnings
 
 from typing import Optional, NoReturn, List, Callable, Union
 from collections.abc import Iterable
 
 import numpy as np
 
@@ -32,16 +33,23 @@
 
 #: Parameter keys used to init a molecular-dynamics task.
 MD_INIT_KEYS: List[str] = [
     "md_style", "velocity_seed", "timestep", "temp", "Tdamp", 
     "press", "Pdamp", "dump_period"
 ]
 
-#: Parameter keys used to run a molecular-dynamics task.
-MD_RUN_KEYS: List[str] = ["steps"]
+
+@dataclasses.dataclass
+class Controller:
+
+    #: Thermostat name.
+    name: str = "controller" # thermostat or barostat
+
+    #: Parameters.
+    params: dict = dataclasses.field(default_factory=dict)
 
 
 @dataclasses.dataclass
 class DriverSetting:
 
     """These are geometric parameters. Electronic?
     """
@@ -93,18 +101,22 @@
     steps: int = 0
 
     constraint: str = None
 
     #: Parameters that are used to update 
     _internals: dict = dataclasses.field(default_factory=dict)
 
-    #def __post_init__(self):
-    #    """A dummy function that will be overridden by subclasses."""
+    def update(self, **kwargs):
+        """"""
+        for k, v in kwargs.items():
+            if hasattr(self, k):
+                setattr(self, k, v)
+        self.__post_init__()
 
-    #    return
+        return
     
     def get_init_params(self):
         """"""
 
         return copy.deepcopy(self._internals)
     
     def get_run_params(self, *args, **kwargs):
@@ -339,14 +351,36 @@
         # retain calculator-related files
         for fname in self.removed_fnames:
             curr_fpath = self.directory/fname
             if curr_fpath.exists():
                 curr_fpath.unlink()
 
         return
+
+    def _preprocess_constraints(self, atoms: Atoms, run_params: dict) -> None:
+        """Remove existing constraints on atoms and add FixAtoms.
+
+        If have cons in kwargs overwrite current cons stored in atoms.
+
+        """
+        # - check constraint
+        cons_text = run_params.pop("constraint", None)
+        if cons_text is not None: # FIXME: check cons_text in parse_?
+            atoms._del_constraints()
+            mobile_indices, frozen_indices = parse_constraint_info(
+                atoms, cons_text, ignore_ase_constraints=True, ret_text=False
+            )
+            if frozen_indices:
+                atoms.set_constraint(FixAtoms(indices=frozen_indices))
+            else:
+                ...
+        else:
+            ...
+
+        return
     
     def read_convergence(self, cache_traj: List[Atoms]=None, *args, **kwargs) -> bool:
         """Read output to check whether the simulation is converged.
 
         TODO:
             If not converged, specific params in input files should be updated.
 
@@ -407,43 +441,76 @@
                     maxfrc = np.max(np.fabs(end_atoms.get_forces(apply_constraint=True)))
                     if maxfrc <= self.setting.fmax or step+1 >= self.setting.steps:
                         converged = True
                     self._debug(
                         f"MIN convergence: {converged} STEP: {step+1} >=? {self.setting.steps} MAXFRC: {maxfrc} <=? {self.setting.fmax}"
                     )
                 elif self.setting.task == "md":
-                    #print("steps: ", step, self.setting.steps)
                     if step+1 >= self.setting.steps: # step startswith 0
                         converged = True
-                    self._debug(f"MD convergence: {converged}")
+                    self._debug(f"MD convergence: {converged} STEP: {step+1} >=? {self.setting.steps}")
                 else:
                     raise NotImplementedError("Unknown task in read_convergence.")
             else:
                 # just spc, only need to check force convergence
                 if nframes == 1:
                     converged = True
             self._print(f"energy: {traj_frames[-1].get_potential_energy():12.4f}")
         else:
             ...
 
-        # TODO: if driver converged but force (scf) is not, return True
-        #       and discard this structures which is due to DFT or ...
-        force_converged = True
-        if hasattr(self, "read_force_convergence"):
-            force_converged = self.read_force_convergence()
-
-        return (converged and force_converged)
+        return converged
 
     @abc.abstractmethod
     def read_trajectory(self, *args, **kwargs) -> List[Atoms]:
         """Read trajectory in the current working directory.
         """
 
         return
     
+    def _aggregate_trajectories(self, archive_path=None) -> List[Atoms]:
+        """"""
+        prev_wdirs = []
+        if archive_path is None:
+            prev_wdirs = sorted(self.directory.glob(r"[0-9][0-9][0-9][0-9][.]run"))
+        else:
+            pattern = self.directory.name + "/" + r"[0-9][0-9][0-9][0-9][.]run"
+            with tarfile.open(archive_path, "r:gz") as tar:
+                for tarinfo in tar:
+                    if tarinfo.isdir() and re.match(pattern, tarinfo.name):
+                        prev_wdirs.append(tarinfo.name)
+            prev_wdirs = [self.directory/pathlib.Path(p).name for p in sorted(prev_wdirs)]
+        self._debug(f"prev_wdirs: {prev_wdirs}")
+
+        all_wdirs = prev_wdirs + [self.directory]
+
+        traj_list = []
+        for w in all_wdirs:
+            curr_frames = self._read_a_single_trajectory(w, archive_path=archive_path)
+            if curr_frames:
+                traj_list.append(curr_frames)
+
+        # -- concatenate
+        # NOTE: For DFT calculations,
+        #       some spin systems may give different scf convergence on the same
+        #       structure. Sometimes, the preivous failed but the next run converged,
+        #       The concat below uses the previous one...
+        traj_frames, ntrajs = [], len(traj_list)
+        if ntrajs > 0:
+            traj_frames.extend(traj_list[0])
+            for i in range(1, ntrajs):
+                assert np.allclose(
+                    traj_list[i - 1][-1].positions, traj_list[i][0].positions
+                ), f"Traj {i-1} and traj {i} are not consecutive."
+                traj_frames.extend(traj_list[i][1:])
+        else:
+            ...
+
+        return traj_frames
+    
     def as_dict(self) -> dict:
         """Return parameters of this driver."""
         params = dict(
             backend = self.name,
             ignore_convergence = self.ignore_convergence,
             random_seed=self.random_seed
         )
```

### Comparing `gdpx-0.0.5/src/gdpx/computation/espresso.py` & `gdpx-0.0.6/src/gdpx/computation/espresso.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.5/src/gdpx/computation/interface.py` & `gdpx-0.0.6/src/gdpx/computation/interface.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from ase.io import read, write
 
 from .. import config
 from ..core.operation import Operation
 from ..core.register import registers
 from ..core.variable import Variable
 from ..data.array import AtomsNDArray
+from ..selector.scf import ScfSelector
 from ..utils.command import CustomTimer
 from ..worker.drive import (
     CommandDriverBasedWorker,
     DriverBasedWorker,
     QueueDriverBasedWorker,
 )
 from ..worker.interface import ComputerVariable
@@ -152,15 +153,15 @@
     # - load previous structures' shape
     if shape_dir.exists():
         inp_shape = np.loadtxt(shape_dir / "shape.dat", dtype=int)
         inp_markers = np.loadtxt(shape_dir / "markers.dat", dtype=int)
     else:
         inp_shape = None
         inp_markers = None
-    
+
     return inp_shape, inp_markers
 
 
 def convert_results_to_structures(
     structures: List[Atoms],
     inp_shape,
     inp_markers,
@@ -177,35 +178,35 @@
 
     # TODO: Convert to correct input data shape for spc workers...
     #       Optimise the codes here?
     _print(f"target structure shape: {inp_shape}")
     _print(f"input  structure shape: {structures.shape}")
     if inp_shape is not None and inp_markers is not None:
         converted_structures = []
-        for curr_structures in structures:  # shape (nworkers, ncandidates, 1) 
+        for curr_structures in structures:  # shape (nworkers, ncandidates, 1)
             curr_structures = list(itertools.chain(*curr_structures))
             inp_shape_ = np.max(inp_markers, axis=0) + 1
-            #assert np.allclose(
+            # assert np.allclose(
             #    inp_shape_, inp_shape
-            #), "Inconsistent shape {inp_shape_} vs. {inp_shape}"
+            # ), "Inconsistent shape {inp_shape_} vs. {inp_shape}"
             _print(f"previous  structure shape: {inp_shape}")
             _print(f"target    structure shape: {inp_shape_}")
             # - get a full list of indices and fill None to a flatten Atoms List
-            #_print(inp_markers)
+            # _print(inp_markers)
             curr_converted_structures = []
             full_list = list(itertools.product(*[range(x) for x in inp_shape_]))
             for i, iloc in enumerate(full_list):
                 if iloc in inp_markers:
                     curr_converted_structures.append(
                         curr_structures[inp_markers.index(iloc)]
                     )
                 else:
                     curr_converted_structures.append(None)
-            #_print(len(curr_converted_structures))
-            #_print(curr_converted_structures[0])
+            # _print(len(curr_converted_structures))
+            # _print(curr_converted_structures[0])
             # - reshape
             for s in inp_shape_[:0:-1]:
                 npoints = len(curr_converted_structures)
                 repeats = int(npoints / s)
                 reshaped_converted_structures = [
                     [curr_converted_structures[i] for i in range(r * s, (r + 1) * s)]
                     for r in range(repeats)
@@ -216,15 +217,15 @@
     else:  # No data available to convert structures
         converted_structures = structures
 
     # --- further convert
     if reduce_single_worker:  #  nworkers == 1
         converted_structures = converted_structures[0]
 
-    if merge_workers: # squeeze the dimension one...
+    if merge_workers:  # squeeze the dimension one...
         converted_structures = list(itertools.chain(*converted_structures))
     converted_structures = AtomsNDArray(converted_structures)
     _print(f"extracted_results: {converted_structures}")
 
     return converted_structures
 
 
@@ -239,14 +240,15 @@
         batchsize: Optional[int] = None,
         share_wdir: bool = False,
         retain_info: bool = False,
         extract_data: bool = True,
         use_archive: bool = True,
         merge_workers: bool = False,
         reduce_single_worker: bool = True,
+        check_scf_convergence: bool = False,
         directory: Union[str, pathlib.Path] = "./",
     ):
         """Initialise a compute operation.
 
         Args:
             builder: A builder node.
             worker: A worker node.
@@ -265,14 +267,17 @@
 
         # - worker-retrieve-related settings
         self.extract_data = extract_data
         self.use_archive = use_archive
         self.merge_workers = merge_workers
         self.reduce_single_worker = reduce_single_worker
 
+        # -
+        self.check_scf_convergence = check_scf_convergence
+
         return
 
     def _preprocess_input_nodes(self, input_nodes):
         """"""
         builder, worker = input_nodes
         if isinstance(worker, dict) or isinstance(
             worker, omegaconf.dictconfig.DictConfig
@@ -301,17 +306,18 @@
 
         nworkers = len(workers)
 
         # TODO: It is better to move this part to driver...
         #       We only convert spc worker structures shape here...
         driver0_dict = workers[0].driver.as_dict()
         if (
-            nworkers == 1 and driver0_dict.get("task", "min") == "min" and
-            (driver0_dict.get("steps", 0) <= 0)
-        ): # TODO: spc?
+            nworkers == 1
+            and driver0_dict.get("task", "min") == "min"
+            and (driver0_dict.get("steps", 0) <= 0)
+        ):  # TODO: spc?
             # - check input data type
             inp_shape, inp_markers = None, None
             if isinstance(structures, AtomsNDArray):
                 frames = structures.get_marked_structures()
                 nframes = len(frames)
                 inp_shape = structures.shape
                 inp_markers = [tuple(iloc.tolist()) for iloc in structures.markers]
@@ -322,25 +328,30 @@
                 inp_markers = [(0, i) for i in range(nframes)]
             # self._print(inp_markers)
             # -- Dump shape data
             # NOTE: Since all workers use the same input structures,
             #       we only need to dump once here
             shape_dir = self.directory / "_shape"
             shape_dir.mkdir(parents=True, exist_ok=True)
-            np.savetxt(shape_dir / "shape.dat", np.array(inp_shape, dtype=np.int32), fmt="%8d")
-            np.savetxt(shape_dir / "markers.dat", np.array(inp_markers, dtype=np.int32), fmt="%8d")
+            np.savetxt(
+                shape_dir / "shape.dat", np.array(inp_shape, dtype=np.int32), fmt="%8d"
+            )
+            np.savetxt(
+                shape_dir / "markers.dat",
+                np.array(inp_markers, dtype=np.int32),
+                fmt="%8d",
+            )
         else:
             if isinstance(structures, AtomsNDArray):
                 frames = structures.get_marked_structures()
-            else: # assume it is just a plain List of Atoms
+            else:  # assume it is just a plain List of Atoms
                 frames = structures
             nframes = len(frames)
             inp_shape, inp_markers = None, None
 
-
         # - create workers
         for i, worker in enumerate(workers):
             worker.directory = self.directory / f"w{i}"
             if self.batchsize is not None:
                 worker.batchsize = self.batchsize
             else:
                 worker.batchsize = nframes
@@ -399,16 +410,22 @@
                     computed_structures = convert_results_to_structures(
                         computed_structures,
                         inp_shape,
                         inp_markers,
                         reduce_single_worker=reduce_single_worker,
                         merge_workers=self.merge_workers,
                         print_func=self._print,
-                        debug_func=self._debug
+                        debug_func=self._debug,
                     )
+                    if self.check_scf_convergence:
+                        selector = ScfSelector(scf_converged=True)
+                        selector.directory = self.directory / "selected"
+                        selector.select(
+                            computed_structures,
+                        )
                     output = computed_structures
                 else:
                     ...
             else:
                 self.status = "finished"
         else:
             ...
@@ -482,14 +499,15 @@
 
     def __init__(
         self,
         compute,
         merge_workers: bool = False,
         reduce_single_worker: bool = True,
         use_archive: bool = True,
+        check_scf_convergence: bool = False,
         directory="./",
         *args,
         **kwargs,
     ) -> None:
         """Init an extract operation.
 
         Args:
@@ -500,14 +518,15 @@
         """
         super().__init__(input_nodes=[compute], directory=directory)
 
         self.merge_workers = merge_workers
         self.reduce_single_worker = reduce_single_worker
 
         self.use_archive = use_archive
+        self.check_scf_convergence = check_scf_convergence
 
         return
 
     def forward(self, workers: List[DriverBasedWorker]) -> AtomsNDArray:
         """
         Args:
             workers: ...
@@ -517,15 +536,17 @@
 
         """
         super().forward()
 
         self.workers = workers  # for operations to access
 
         # - shape
-        inp_shape, inp_markers = get_shape_data(self.input_nodes[0].directory/"_shape")
+        inp_shape, inp_markers = get_shape_data(
+            self.input_nodes[0].directory / "_shape"
+        )
 
         # - extract results
         status, computed_structures = extract_results_from_workers(
             self.directory,
             workers,
             use_archive=self.use_archive,
             print_func=self._print,
@@ -540,16 +561,22 @@
             computed_structures = convert_results_to_structures(
                 computed_structures,
                 inp_shape,
                 inp_markers,
                 reduce_single_worker=reduce_single_worker,
                 merge_workers=self.merge_workers,
                 print_func=self._print,
-                debug_func=self._debug
+                debug_func=self._debug,
             )
+            if self.check_scf_convergence:
+                selector = ScfSelector(scf_converged=True)
+                selector.directory = self.directory / "selected"
+                selector.select(
+                    computed_structures,
+                )
 
         self.status = status
 
         return computed_structures
 
 
 if __name__ == "__main__":
```

### Comparing `gdpx-0.0.5/src/gdpx/computation/lammps.py` & `gdpx-0.0.6/src/gdpx/computation/lammps.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,18 +28,19 @@
 from ase.calculators.calculator import (
     CalculationFailed,
     Calculator, all_changes, PropertyNotImplementedError, FileIOCalculator
 )
 from ase.calculators.singlepoint import SinglePointCalculator
 from ase.calculators.mixing import LinearCombinationCalculator
 
-from gdpx import config
-from gdpx.computation.driver import AbstractDriver, DriverSetting, BACKUP_PREFIX_FORMAT 
-from gdpx.builder.constraints import parse_constraint_info
-from .plumed import Plumed, update_stride_and_file
+from .. import config
+from ..builder.constraints import parse_constraint_info
+from .driver import AbstractDriver, DriverSetting
+
+from ..potential.managers.plumed.calculators.plumed2 import Plumed, update_stride_and_file
 
 
 dataclasses.dataclass(frozen=True)
 class AseLammpsSettings:
 
     """File names."""
```

### Comparing `gdpx-0.0.5/src/gdpx/computation/lasp.py` & `gdpx-0.0.6/src/gdpx/computation/lasp.py`

 * *Files 2% similar despite different names*

```diff
@@ -153,14 +153,18 @@
 def read_lasp_structures(
         mdir: pathlib.Path, wdir: pathlib.Path, archive_path: pathlib.Path=None, 
         *args, **kwargs
     ) -> List[Atoms]:
     """Read simulation trajectory."""
     wdir = pathlib.Path(wdir)
 
+    # - check if output file exists...
+    if (not (wdir/"allstr.arc").exists()) and archive_path is None:
+        return []
+
     # - get IO
     if archive_path is None:
         with open(wdir/"allstr.arc", "r") as fopen:
             stru_io = io.StringIO(fopen.read())
         afrc_io = open(wdir/"allfor.arc", "r") # atomic forces in arc format
         lout_io = open(wdir/"lasp.out", "r")
     else:
@@ -266,17 +270,14 @@
     lout_io.close()
 
     return traj_frames
 
 @dataclasses.dataclass
 class LaspDriverSetting(DriverSetting):
 
-    #: Whether accepct the bad structure due to crashed FF or SCF-unconverged DFT.
-    accept_bad_structure: bool = True
-
     def __post_init__(self):
         """"""
         if self.task == "min":
             self._internals.update(
                 **{
                     "explore_type": "ssw",
                     "SSW.SSWsteps": 1, # BFGS
@@ -343,14 +344,17 @@
 
 class LaspDriver(AbstractDriver):
 
     """Driver for LASP."""
 
     name = "lasp"
 
+    #: Whether accepct the bad structure due to crashed FF or SCF-unconverged DFT.
+    accept_bad_structure: bool = True
+
     # - defaults
     default_task = "min"
     supported_tasks = ["min", "md"]
 
     def __init__(self, calc, params: dict, directory="./", *args, **kwargs):
         """"""
         super().__init__(calc, params, directory=directory, *args, **kwargs)
@@ -369,29 +373,33 @@
             else:
                 verified = False
         else:
             ...
 
         return verified
 
-    def _irun(self, atoms: Atoms, ckpt_wdir=None, *args, **kwargs) -> None:
+    def _irun(self, atoms: Atoms, ckpt_wdir=None, cache_traj: List[Atoms]=None, *args, **kwargs) -> None:
         """"""
         try:
             if ckpt_wdir is None: # start from the scratch
                 # - init params
                 run_params = self.setting.get_init_params()
                 run_params.update(**self.setting.get_run_params(**kwargs))
 
                 self.calc.set(**run_params)
                 atoms.calc = self.calc
 
                 _ = atoms.get_forces()
             else:
                 # TODO: velocities?
-                traj = self.read_trajectory()
+                if cache_traj is None:
+                    traj = self.read_trajectory()
+                else:
+                    self._debug("use cache trajectory to restart...")
+                    traj = cache_traj
                 nframes = len(traj)
                 assert nframes > 0, "LaspDriver restarts with a zero-frame trajectory."
                 atoms = traj[-1]
                 target_steps = self.setting.steps
                 dump_period = self.setting.dump_period
                 if target_steps > 0:
                     steps = target_steps + dump_period - nframes*dump_period
@@ -410,42 +418,45 @@
 
         return
     
     def read_force_convergence(self, *args, **kwargs) -> bool:
         """"""
         return self.calc._is_converged()
     
-    def _read_a_single_trajectory(self, wdir: pathlib.Path, archive_path: pathlib.Path, *args, **kwargs):
+    def _read_a_single_trajectory(self, wdir: pathlib.Path, archive_path: pathlib.Path, *args, **kwargs) -> List[Atoms]:
         """"""
         curr_frames = read_lasp_structures(self.directory, wdir, archive_path=archive_path)
 
         return curr_frames
     
     def read_trajectory(self, archive_path: pathlib.Path=None, *args, **kwargs) -> List[Atoms]:
         """Read trajectory in the current working directory."""
         prev_wdirs = sorted(self.directory.glob(r"[0-9][0-9][0-9][0-9][.]run"))
         self._debug(f"prev_wdirs: {prev_wdirs}")
 
         traj_list = []
         for w in prev_wdirs:
-            curr_frames = self._read_a_single_trajectory(self.directory, w, archive_path)
+            curr_frames = self._read_a_single_trajectory(w, archive_path)
             traj_list.append(curr_frames)
         
         # Even though arc file may be empty, the read can give a empty list...
         laspstr = self.directory / "allstr.arc"
-        traj_list.append(read_lasp_structures(self.directory, self.directory, archive_path))
+        traj_list.append(self._read_a_single_trajectory(self.directory, archive_path))
 
         # -- concatenate
         traj_frames, ntrajs = [], len(traj_list)
         if ntrajs > 0:
             traj_frames.extend(traj_list[0])
             for i in range(1, ntrajs):
-                #assert np.allclose(traj_list[i-1][-1].positions, traj_list[i][0].positions), f"Traj {i-1} and traj {i} are not consecutive."
-                assert compare_trajectory_continuity(traj_list[i-1], traj_list[i]), f"Traj {i-1} and traj {i} are not consecutive."
-                traj_frames.extend(traj_list[i][1:])
+                if traj_list[i]: # check if the traj is a empty list
+                    #assert np.allclose(traj_list[i-1][-1].positions, traj_list[i][0].positions), f"Traj {i-1} and traj {i} are not consecutive."
+                    assert compare_trajectory_continuity(traj_list[i-1], traj_list[i]), f"Traj {i-1} and traj {i} are not consecutive."
+                    traj_frames.extend(traj_list[i][1:])
+                else:
+                    ...
         else:
             ...
         
         nframes = len(traj_frames)
         self._debug(f"LASP read_trajectory nframes: {nframes}")
 
         # NOTE: LASP only save step info in MD simulations...
```

### Comparing `gdpx-0.0.5/src/gdpx/computation/md/md_utils.py` & `gdpx-0.0.6/src/gdpx/computation/md/md_utils.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.5/src/gdpx/computation/md/nosehoover.py` & `gdpx-0.0.6/src/gdpx/computation/md/nosehoover.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.5/src/gdpx/computation/plumed.py` & `gdpx-0.0.6/src/gdpx/potential/managers/plumed/calculators/plumed2.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 #!/usr3/bin/env python3
 # -*- coding: utf-8 -*
 
 import copy
 import os
+import pathlib
+import shutil
+
 from typing import List
 
 import numpy as np
 
 from ase import units
-from ase.calculators.calculator import Calculator, all_changes
-from ase.io.trajectory import Trajectory
-import numpy as np
-from os.path import exists
 from ase.units import fs, mol, kJ, nm
+from ase.calculators.calculator import Calculator, all_changes
 
 try:
     import plumed
 except Exception as e:
     print(e)
 
 
@@ -39,155 +39,59 @@
 Notes:
 
     conda install -c conda-forge plumed
     conda install -c conda-forge py-plumed
 
 """
 
-def set_plumed_state(calc, timestep: float, stride: int):
-    """"""
-    if isinstance(calc, Plumed):
-        calc.timestep = timestep
-        calc.stride = stride
-    if hasattr(calc, "calcs"):
-        for subcalc in calc.calcs:
-            set_plumed_state(subcalc, timestep, stride)
-    else:
-        ...
-
-    return
-
-
-class AsePlumed(object):
-
-    def __init__(
-            self, atoms, timestep,
-            in_file = 'plumed.dat', 
-            out_file = 'plumed.out'
-        ):
-
-        self.atoms = atoms
-        self.timestep = timestep
-        self.natoms = len(atoms)
-        self.masses = self.atoms.get_masses().copy() # masses cannot change
-
-        self.in_file = in_file
-        self.out_file = out_file
-
-        self.worker = self.initialize()
-
-        return
-
-    def initialize(self):
-        # init
-        p_md = plumed.Plumed()
-
-        # units
-        energyUnits = units.mol / units.kJ  # eV to kJ/mol
-        lengthUnits = 1./units.nm # angstrom to nm
-        timeUnits = 1./(1000.*units.fs) # fs to ps
-
-        p_md.cmd("setMDEnergyUnits", energyUnits)
-        p_md.cmd("setMDLengthUnits", lengthUnits)
-        p_md.cmd("setMDTimeUnits", timeUnits)
-
-        # inp, out
-        p_md.cmd("setPlumedDat", self.in_file)
-        p_md.cmd("setLogFile", self.out_file)
-
-        # simulation details
-        p_md.cmd("setTimestep", self.timestep)
-        p_md.cmd("setNatoms", self.natoms)
-        p_md.cmd("setMDEngine", 'ase')
-
-        # finally!
-        p_md.cmd("init")
-
-        return p_md
-
-    def external_forces(
-            self, 
-            istep, 
-            new_energy = None,
-            new_forces = None, # sometimes use forces not attached to self.atoms
-            new_virial = None,
-            delta_forces = False
-        ):
-        """return external forces from plumed"""
-        # structure info
-        positions = self.atoms.get_positions().copy()
-        cell = self.atoms.cell[:].copy()
-
-        if new_forces is None:
-            forces = self.atoms.get_forces().copy()
-        else:
-            forces = new_forces.copy()
-        original_forces = forces.copy()
-
-        if new_energy is None:
-            energy = self.atoms.get_potential_energy()
-        else:
-            energy = new_energy
-
-        # TODO: get virial
-        virial = np.zeros((3,3))
-
-        self.worker.cmd("setStep", istep)
-        self.worker.cmd("setMasses", self.masses)
-        self.worker.cmd("setForces", forces)
-        self.worker.cmd("setPositions", positions)
-        self.worker.cmd("setEnergy", energy)
-        self.worker.cmd("setBox", cell)
-        self.worker.cmd("setVirial", virial)
-        self.worker.cmd("calc", None)
-
-        # implent plumed external forces into momenta
-        if delta_forces:
-            plumed_forces = forces - original_forces
-        else:
-            plumed_forces = forces
-
-        return plumed_forces
-
-    def finalize(self):
-        self.worker.finalize()
-
 
 def update_input_value(line: str, key: str, value, func: callable):
     """Update the given key with the new value."""
-    shift = len(key) + 1 # key name and =
+    shift = len(key) + 1  # key name and =
     if line.find(key) != -1:
         ini = line.find(key)
-        end = line.find(' ', ini)
+        end = line.find(" ", ini)
         if end == -1:
-            prev = line[ini + shift:]
-            line = line[:ini+shift] + func(prev, value)
+            prev = line[ini + shift :]
+            line = line[: ini + shift] + func(prev, value)
         else:
-            prev = line[ini + shift:end]
-            line = line[:ini+shift] + func(prev, value) + line[end:]
+            prev = line[ini + shift : end]
+            line = line[: ini + shift] + func(prev, value) + line[end:]
 
     return line
 
+
 def update_stride_and_file(input_lines: List[str], wdir: str, stride: int) -> List[str]:
     """"""
     input_lines, parsed_lines = copy.deepcopy(input_lines), []
     for line in input_lines:
-        parsed_line = update_input_value(line, "FILE", wdir, func=lambda x,y: os.path.join(y,x))
-        parsed_line = update_input_value(parsed_line, "STRIDE", stride, func=lambda x,y: str(y))
+        parsed_line = update_input_value(
+            line, "FILE", wdir, func=lambda x, y: os.path.join(y, x)
+        )
+        parsed_line = update_input_value(
+            parsed_line, "STRIDE", stride, func=lambda x, y: str(y)
+        )
         parsed_lines.append(parsed_line)
-    
+
     return parsed_lines
 
 
 class Plumed(Calculator):
 
     implemented_properties = ["energy", "forces"]
 
-    def __init__(self, input: List[str], atoms=None, kT=1.,
-                 restart=False, use_charge=False, update_charge=False):
+    def __init__(
+        self,
+        input: List[str],
+        atoms=None,
+        kT=1.0,
+        restart=False,
+        use_charge=False,
+        update_charge=False,
+    ):
         """
         Plumed calculator is used for simulations of enhanced sampling methods
         with the open-source code PLUMED (plumed.org).
 
         [1] The PLUMED consortium, Nat. Methods 16, 670 (2019)
         [2] Tribello, Bonomi, Branduardi, Camilloni, and Bussi,
         Comput. Phys. Commun. 185, 604 (2014)
@@ -228,15 +132,15 @@
             momenta, positions and Plumed.istep, where the positions and
             momenta corresponds to the last configuration in the previous
             simulation, while Plumed.istep is the number of timesteps
             performed previously. This can be done using
             ase.calculators.plumed.restart_from_trajectory.
         """
 
-        #if atoms is None:
+        # if atoms is None:
         #    raise TypeError('plumed calculator has to be defined with the \
         #                     object atoms inside.')
 
         self.istep = 0
         Calculator.__init__(self, atoms=atoms)
 
         self.input = input
@@ -244,86 +148,135 @@
         self.update_charge = update_charge
 
         self.kT = kT
         self.restart = restart
 
         self._timestep = None
         self._stride = 1
-        
+
         return
-    
+
     @property
     def timestep(self):
         """"""
 
         return self._timestep
-    
+
     @timestep.setter
     def timestep(self, timestep):
         """"""
         self._timestep = timestep
 
         return
-    
+
     @property
     def stride(self):
 
         return self._stride
-    
+
     @stride.setter
     def stride(self, stride):
         """"""
         self._stride = stride
 
         return self._stride
-    
-    def _prepare(self, natoms, input_lines, timestep, restart, kT):
+
+    def _prepare(
+        self,
+        natoms: int,
+        input_lines: List[str],
+        timestep: float,
+        restart: bool,
+        kT: float,
+    ):
         """"""
         self.plumed = plumed.Plumed()
 
         # - basic configuration
         ps = 1000 * fs
         self.plumed.cmd("setMDEnergyUnits", mol / kJ)
         self.plumed.cmd("setMDLengthUnits", 1 / nm)
         self.plumed.cmd("setMDTimeUnits", 1 / ps)
-        self.plumed.cmd("setMDChargeUnits", 1.)
-        self.plumed.cmd("setMDMassUnits", 1.)
+        self.plumed.cmd("setMDChargeUnits", 1.0)
+        self.plumed.cmd("setMDMassUnits", 1.0)
         self.plumed.cmd("setMDEngine", "ASE")
 
         self.plumed.cmd("setNatoms", natoms)
         self.plumed.cmd("setLogFile", os.path.join(self.directory, "plumed.out"))
         self.plumed.cmd("setTimestep", float(timestep))
         self.plumed.cmd("setRestart", restart)
         self.plumed.cmd("setKbT", float(kT))
         self.plumed.cmd("init")
 
         # - parse lines, update FILE and STRIDE
         input_lines, parsed_lines = copy.deepcopy(input_lines), []
         for line in input_lines:
-            parsed_line = update_input_value(line, "FILE", self.directory, func=lambda x,y: os.path.join(y,x))
-            parsed_line = update_input_value(parsed_line, "STRIDE", self.stride, func=lambda x,y: str(y))
+            parsed_line = update_input_value(
+                line, "FILE", self.directory, func=lambda x, y: os.path.join(y, x)
+            )
+            parsed_line = update_input_value(
+                parsed_line, "STRIDE", self.stride, func=lambda x, y: str(y)
+            )
+            parsed_line = update_input_value(
+                parsed_line, "PACE", self.stride, func=lambda x, y: str(y)
+            )
             parsed_lines.append(parsed_line)
 
         for line in parsed_lines:
             self.plumed.cmd("readInputLine", line)
 
+        # - save input lines
+        inp_fpath = pathlib.Path(self.directory, "plumed.inp")
+        with open(inp_fpath, "w") as fopen:
+            fopen.write("\n".join(input_lines))
+
         return
 
-    def calculate(self, atoms=None, properties=['energy', 'forces'],
-                  system_changes=all_changes):
+    def _save_checkpoint(self, ckpt_wdir: pathlib.Path):
+        """"""
+        calc_wdir = pathlib.Path(self.directory)
+        if (ckpt_wdir / calc_wdir.name).exists():
+            shutil.rmtree(ckpt_wdir / calc_wdir.name)
+        _ = shutil.copytree(calc_wdir, ckpt_wdir / calc_wdir.name)
+
+        return
+
+    def _load_checkpoint(
+        self, ckpt_wdir: pathlib.Path, dst_wdir=None, start_step: int = 0
+    ):
+        """"""
+        calc_wdir = list(ckpt_wdir.glob(f"*Plumed"))[0]
+        if dst_wdir is None:
+            dst_wdir = ckpt_wdir.parent
+        else:
+            dst_wdir = pathlib.Path(dst_wdir)
+        _ = shutil.copytree(calc_wdir, dst_wdir / calc_wdir.name)
+
+        if hasattr(self, "plumed"):
+            self.plumed.finalize()
+            delattr(self, "plumed")
+        self.istep = int(start_step)
+        self.input = ["RESTART"] + self.input
+        self.restart = True
+
+        return
+
+    def calculate(
+        self, atoms=None, properties=["energy", "forces"], system_changes=all_changes
+    ):
         """"""
         Calculator.calculate(self, atoms, properties, system_changes)
 
         if self.timestep is None:
-            raise RuntimeError("Plumed needs a valid timestep set by an external class.")
+            raise RuntimeError(
+                "Plumed needs a valid timestep set by an external class."
+            )
 
         if not hasattr(self, "plumed"):
-            self._prepare(
-                len(atoms), self.input, self.timestep, self.restart, self.kT
-            )
+            self._prepare(len(atoms), self.input, self.timestep, self.restart, self.kT)
 
         energy_bias, forces_bias = self.compute_bias(
             self.atoms.get_positions(), self.istep
         )
 
         self.results["energy"], self.results["forces"] = energy_bias, forces_bias
         self.istep += 1
@@ -336,15 +289,15 @@
 
         # Box for functions with PBC in plumed
         if np.any(self.atoms.pbc):
             cell = self.atoms.get_cell(complete=True).array
             self.plumed.cmd("setBox", cell)
 
         self.plumed.cmd("setPositions", pos)
-        self.plumed.cmd("setEnergy", 0.)
+        self.plumed.cmd("setEnergy", 0.0)
         self.plumed.cmd("setMasses", self.atoms.get_masses())
         forces_bias = np.zeros((self.atoms.get_positions()).shape)
         self.plumed.cmd("setForces", forces_bias)
         virial = np.zeros((3, 3))
         self.plumed.cmd("setVirial", virial)
         self.plumed.cmd("prepareCalc")
         self.plumed.cmd("performCalc")
@@ -357,8 +310,8 @@
         return self
 
     def __exit__(self, *args):
         self.plumed.finalize()
 
 
 if __name__ == "__main__":
-    ...
+    ...
```

### Comparing `gdpx-0.0.5/src/gdpx/computation/utils.py` & `gdpx-0.0.6/src/gdpx/computation/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 import copy
-from typing import List
-
-import numpy as np
+from typing import List, Callable
 
 from ase import Atoms
-from ase.io import read, write
 from ase.calculators.singlepoint import SinglePointCalculator
 
 
 def copy_minimal_frames(prev_frames: List[Atoms]):
     """Copy atoms without extra information.
 
     Do not copy atoms.info since it is a dict and does not maitain order.
@@ -20,82 +17,67 @@
     curr_frames, curr_info = [], []
     for prev_atoms in prev_frames:
         # - copy geometry
         curr_atoms = Atoms(
             symbols=copy.deepcopy(prev_atoms.get_chemical_symbols()),
             positions=copy.deepcopy(prev_atoms.get_positions()),
             cell=copy.deepcopy(prev_atoms.get_cell(complete=True)),
-            pbc=copy.deepcopy(prev_atoms.get_pbc())
+            pbc=copy.deepcopy(prev_atoms.get_pbc()),
         )
         curr_frames.append(curr_atoms)
         # - save info
         confid = prev_atoms.info.get("confid", -1)
         dynstep = prev_atoms.info.get("step", -1)
         prev_wdir = prev_atoms.info.get("wdir", "null")
-        curr_info.append((confid,dynstep,prev_wdir))
+        curr_info.append((confid, dynstep, prev_wdir))
 
     return curr_frames, curr_info
 
-def make_clean_atoms(atoms_: Atoms, results: dict=None):
+
+def make_clean_atoms(atoms_: Atoms, results: dict = None):
     """Create a clean atoms from the input."""
     atoms = Atoms(
         symbols=atoms_.get_chemical_symbols(),
         positions=atoms_.get_positions().copy(),
         cell=atoms_.get_cell().copy(),
-        pbc=copy.deepcopy(atoms_.get_pbc())
+        pbc=copy.deepcopy(atoms_.get_pbc()),
     )
     if results is not None:
         spc = SinglePointCalculator(atoms, **results)
         atoms.calc = spc
 
     return atoms
 
-def create_single_point_calculator(atoms_sorted, resort, calc_name):
-    """ create a spc to store calc results
-        since some atoms may share a calculator
-    """
-    atoms = atoms_sorted.copy()[resort]
-
-    try:
-        calc = SinglePointCalculator(
-            atoms,
-            energy=atoms_sorted.get_potential_energy(),
-            forces=atoms_sorted.get_forces(apply_constraint=False)[resort]
-            # TODO: magmoms?
-        )
-        calc.name = calc_name
-        atoms.calc = calc
-    except Exception as e:
-        print(f"create_single_point_calculator: {e}")
-        atoms = None
-
-    return atoms
 
 def parse_type_list(atoms):
     """parse type list for read and write structure of lammps"""
     # elements
     type_list = list(set(atoms.get_chemical_symbols()))
-    type_list.sort() # by alphabet
+    type_list.sort()  # by alphabet
 
     return type_list
 
+
 def get_composition_from_atoms(atoms):
     """"""
     from collections import Counter
+
     chemical_symbols = atoms.get_chemical_symbols()
     composition = Counter(chemical_symbols)
-    sorted_composition = sorted(composition.items(), key=lambda x:x[0])
+    sorted_composition = sorted(composition.items(), key=lambda x: x[0])
 
     return sorted_composition
 
+
 def get_formula_from_atoms(atoms):
     """"""
     from collections import Counter
+
     chemical_symbols = atoms.get_chemical_symbols()
     composition = Counter(chemical_symbols)
-    sorted_composition = sorted(composition.items(), key=lambda x:x[0])
+    sorted_composition = sorted(composition.items(), key=lambda x: x[0])
 
-    return "".join([str(k)+str(v) for k,v in sorted_composition])
+    return "".join([str(k) + str(v) for k, v in sorted_composition])
 
 
 if __name__ == "__main__":
-    ...
+    ...
```

### Comparing `gdpx-0.0.5/src/gdpx/config.py` & `gdpx-0.0.6/src/gdpx/config.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.5/src/gdpx/core/node.py` & `gdpx-0.0.6/src/gdpx/core/node.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.5/src/gdpx/core/operation.py` & `gdpx-0.0.6/src/gdpx/core/operation.py`

 * *Files 5% similar despite different names*

```diff
@@ -60,14 +60,22 @@
     def reset(self):
         """Reset node's output and status."""
         if hasattr(self, "output"):
             delattr(self, "output")
             self.status = "unfinished"
 
         return
+    
+    def is_about_to_exit(self) -> bool:
+        """Check whether this operation has an input is about to exit."""
+        status = [node.status == "exit" for node in self.input_nodes]
+        if any(status):
+            return True
+        else:
+            return False
 
     def is_ready_to_forward(self) -> bool:
         """Check whether this operation is ready to forward."""
         # - check input nodes' status
         status = [node.status == "finished" for node in self.input_nodes]
         if all(status):
             return True
```

### Comparing `gdpx-0.0.5/src/gdpx/core/placeholder.py` & `gdpx-0.0.6/src/gdpx/core/placeholder.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.5/src/gdpx/core/register.py` & `gdpx-0.0.6/src/gdpx/core/register.py`

 * *Files 1% similar despite different names*

```diff
@@ -166,15 +166,15 @@
     # -- genetic-algorithm-related
     ("gdpx.builder", ["crossover", "mutation"]),
     # -- colvar
     ("gdpx", ["colvar"]),
     # -- selectors
     ("gdpx", ["selector"]),
     # -- describer
-    ("gdpx.describer", ["soap"]),
+    ("gdpx", ["describer"]),
     # -- comparators
     ("gdpx", ["comparator"]),
     # -- expeditions
     ("gdpx", ["expedition"]),
     # -- reactors
     # -- validators
     ("gdpx", ["validator"]),
```

### Comparing `gdpx-0.0.5/src/gdpx/core/session/active.py` & `gdpx-0.0.6/src/gdpx/core/session/active.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,115 +3,127 @@
 
 import copy
 import pathlib
 import time
 
 from typing import NoReturn, Union, Tuple, List, Callable
 
-from .. import config
+
 from ..placeholder import Placeholder
 from ..variable import Variable
-from .basic import Session
+from .session import AbstractSession
 from .utils import traverse_postorder
 
 
-class ActiveSession():
-
-    #: Standard print function.
-    _print: Callable = config._print
-
-    #: Standard debug function.
-    _debug: Callable = config._debug
+class ActiveSession(AbstractSession):
 
     def __init__(
-        self, steps: int=2, reset_random_state: bool=False, 
-        reset_random_config: Tuple[str, int]=("init", 0), 
-        directory="./"
+        self,
+        steps: int = 2,
+        reset_random_state: bool = False,
+        reset_random_config: Tuple[str, int] = ("init", 0),
+        directory="./",
     ) -> None:
         """Initialise an ActiveSession.
 
         Args:
             steps: Number of active learning steps.
             reset_random_seed: A tuple of a str and a int.
 
         """
         self.steps = steps
 
         # - random-related ...
         self.reset_random_state = reset_random_state
-        assert reset_random_config[0] in ["init", "zero"], "Reset random seed mode must either be init or zero."
+        assert reset_random_config[0] in [
+            "init",
+            "zero",
+        ], "Reset random seed mode must either be init or zero."
         self.reset_random_seed_mode = reset_random_config[0]
         self.reset_random_seed_step = reset_random_config[1]
 
         self.directory = pathlib.Path(directory)
 
         return
-    
-    def run(self, operation, feed_dict: dict={}, *args, **kwargs) -> None:
+
+    def run(self, operation, feed_dict: dict = {}, *args, **kwargs) -> None:
         """"""
+        self.state = "StepToStart"
         # - update nodes' attrs based on the previous iteration
-        #nodes_postorder = traverse_postorder(operation)
-        #for node in nodes_postorder:
+        # nodes_postorder = traverse_postorder(operation)
+        # for node in nodes_postorder:
         #    if hasattr(node, "enable_active"):
         #        node.enable_active()
         if self.reset_random_state:
             self._print(
                 f"RESET RANDOM SEED - MODE: {self.reset_random_seed_mode} STEP: {self.reset_random_seed_step}"
             )
 
         # -
         for curr_step in range(self.steps):
-            curr_wdir = self.directory/f"iter.{str(curr_step).zfill(4)}"
+            curr_wdir = self.directory / f"iter.{str(curr_step).zfill(4)}"
             # -- run operation
             nodes_postorder = traverse_postorder(operation)
             # NOTE:
             if self.reset_random_state and curr_step >= self.reset_random_seed_step:
                 for node in nodes_postorder:
                     if hasattr(node, "reset_random_seed"):
                         self._print(f"reset {node.directory.name}'s random seeds.")
                         node.reset_random_seed(mode=self.reset_random_seed_mode)
             # -- run operations
-            finished = self._irun(
-                wdir=curr_wdir, nodes_postorder=nodes_postorder, feed_dict=feed_dict, 
+            self._irun(
+                wdir=curr_wdir,
+                nodes_postorder=nodes_postorder,
+                feed_dict=feed_dict,
             )
-            if not finished:
+            if not (self.state == "StepFinished"):
                 self._print("wait current iteration to finish...")
-                break
             else:
                 # NOTE: If previous step finished, the nodes may not have outputs
                 #       as we skip them...
-                if not (curr_wdir/"FINISHED").exists():
-                    with open(curr_wdir/"FINISHED", "w") as fopen:
-                        fopen.write(
-                            f"FINISHED AT {time.asctime( time.localtime(time.time()) )}."
-                        )
+                if not (curr_wdir / "FINISHED").exists():
                     # --- report
                     self._print("[{:^24s}]".format("CONVERGENCE"))
                     converged_list = []
                     for node in nodes_postorder:
                         if hasattr(node, "report_convergence"):
                             converged = node.report_convergence()
                             converged_list.append(converged)
                     if converged_list and all(converged_list):
                         self._print(f"Active Session converged at step {curr_step}.")
-                        break
+                        self.state = "LoopConverged"
                     else:
                         self._print(f"Active Session UNconverged at step {curr_step}.")
+                        if curr_step + 1 == self.steps:
+                            self.state = "LoopUnConverged"
+                        else:
+                            ...  # Just StepFinished
+                    # --- save state to FILE
+                    with open(curr_wdir / "FINISHED", "w") as fopen:
+                        fopen.write(
+                            f"STATE {self.state} FINISHED AT {time.asctime( time.localtime(time.time()) )}."
+                        )
                 else:
-                    self._print("[{:^24s}] FINISHED".format(f"STEP.{str(curr_step).zfill(4)}"))
+                    self._print(
+                        "[{:^24s}] FINISHED".format(f"STEP.{str(curr_step).zfill(4)}")
+                    )
+            # -- add an atrribute that indicates all steps are finished
+            if self.state != "StepFinished":
+                break
         else:
-            ... # ALL iterations finished...
+            self.state = "LoopFinished"
 
         return
-    
-    def _irun(self, wdir, nodes_postorder, feed_dict: dict={}) -> bool:
+
+    def _irun(self, wdir, nodes_postorder, feed_dict: dict = {}) -> None:
         """"""
-        if (wdir/"FINISHED").exists():
-            return True
-        
+        if (wdir / "FINISHED").exists():
+            self.state = "StepFinished"
+            return
+
         # - clear previous nodes' outputs
         #   somtimes two steps run consecutively and some nodes in the second step
         #   breaks and make its following nodes use outputs from the last step,
         #   which is a hidden error
         for node in nodes_postorder:
             node.reset()
 
@@ -119,26 +131,26 @@
         self._print(
             "[{:^24s}] NUM_NODES: {} AT MAIN: {}".format(
                 "START", len(nodes_postorder), str(wdir)
             )
         )
 
         # - run nodes
-        finished = True
+        self.state = "StepFinished"
         for i, node in enumerate(nodes_postorder):
             # -- change version ...
             if hasattr(node, "version"):
                 node.version = wdir.name
 
             # NOTE: reset directory since it maybe changed
-            prev_name = node.directory.name.split(".")[-1] # remove previous orders
+            prev_name = node.directory.name.split(".")[-1]  # remove previous orders
             if not prev_name:
                 prev_name = node.__class__.__name__
-            #prev_name = node.__class__.__name__
-            node.directory = wdir/f"{str(i).zfill(4)}.{prev_name}"
+            # prev_name = node.__class__.__name__
+            node.directory = wdir / f"{str(i).zfill(4)}.{prev_name}"
             if node.__class__.__name__.endswith("Variable"):
                 node_type = "VX"
             else:
                 node_type = "OP"
             self._print(
                 "[{:^24s}] NAME: {} AT {}".format(
                     node_type, node.__class__.__name__.upper(), node.directory.name
@@ -146,160 +158,151 @@
             )
 
             # -- forward
             if isinstance(node, Placeholder):
                 node.output = feed_dict[node]
             elif isinstance(node, Variable):
                 node.output = node.value
-            else: # Operation
+            else:  # Operation
+                # FIXME: If the session has many branches,
+                #        how do we define the state?
                 self._debug(f"node: {node}")
-                if node.is_ready_to_forward():
-                    node.inputs = [input_node.output for input_node in node.input_nodes]
-                    node.output = node.forward(*node.inputs)
-                else:
-                    finished = False
-                    self._print("wait previous nodes to finish...")
-                    continue
-
-        return finished
+                self._process_operation(node)
 
-class OTFSession():
+        return
 
-    #: Standard print function.
-    _print: Callable = config._print
 
-    #: Standard debug function.
-    _debug: Callable = config._debug
+class OTFSession(AbstractSession):
 
     def __init__(self, directory="./") -> None:
         """"""
         self.directory = pathlib.Path(directory)
 
         return
-    
-    def run(self, operation, feed_dict: dict={}) -> None:
+
+    def run(self, operation, feed_dict: dict = {}) -> None:
         """"""
         for curr_step in range(3):
             # -- update operation
             if curr_step > 0:
                 curr_step = curr_step
                 self._update_potter(operation)
             # -- run operation
             finished = self._irun(
-                operation=operation, feed_dict=feed_dict, 
-                wdir=self.directory/f"iter.{str(curr_step).zfill(4)}"
+                operation=operation,
+                feed_dict=feed_dict,
+                wdir=self.directory / f"iter.{str(curr_step).zfill(4)}",
             )
             if not finished:
                 self._print("wait current iteration to finish...")
                 break
         else:
-            ... # ALL iterations finished...
+            ...  # ALL iterations finished...
 
         return
-    
+
     def _update_potter(self, operation):
         """"""
 
         return
-    
-    def _irun(self, operation, feed_dict: dict={}, wdir=None):
+
+    def _irun(self, operation, feed_dict: dict = {}, wdir=None):
         """"""
         # - find forward order
         nodes_postorder = traverse_postorder(operation)
         self._print(
             "[{:^24s}] NUM_NODES: {} AT MAIN: {}".format(
                 "START", len(nodes_postorder), str(wdir)
             )
         )
 
         # - run nodes
         finished = True
         for i, node in enumerate(nodes_postorder):
             # NOTE: reset directory since it maybe changed
-            #prev_name = node.directory.name
-            #if not prev_name:
+            # prev_name = node.directory.name
+            # if not prev_name:
             #    prev_name = node.__class__.__name__
             prev_name = node.__class__.__name__
-            node.directory = wdir/f"{str(i).zfill(4)}.{prev_name}"
+            node.directory = wdir / f"{str(i).zfill(4)}.{prev_name}"
             if node.__class__.__name__.endswith("Variable"):
                 node_type = "VX"
             else:
                 node_type = "OP"
             self._print(
                 "[{:^24s}] NAME: {} AT {}".format(
                     node_type, node.__class__.__name__.upper(), node.directory.name
                 )
             )
 
             if isinstance(node, Placeholder):
                 node.output = feed_dict[node]
             elif isinstance(node, Variable):
                 node.output = node.value
-            else: # Operation
+            else:  # Operation
                 self._debug(f"node: {node}")
                 if node.is_ready_to_forward():
                     node.inputs = [input_node.output for input_node in node.input_nodes]
                     node.output = node.forward(*node.inputs)
                 else:
                     finished = False
                     self._print("wait previous nodes to finish...")
                     continue
 
         return finished
 
 
-class CyclicSession:
-
+class CyclicSession(AbstractSession):
     """Create a cyclic session.
 
     This supports a session that contains preprocess, iteration, and postprocess.
 
     """
 
-    #: Standard print function.
-    _print: Callable = config._print
-
-    #: Standard debug function.
-    _debug: Callable = config._debug
-
     def __init__(self, directory="./") -> None:
         """"""
         self.directory = pathlib.Path(directory)
 
         return
-    
+
     def iteration(self, operations):
         """Iterative part that converges at certain criteria.
 
         This noramlly includes steps: sample, select, label, and train. Some inputs of
-        operations should be update during the iterations, for instance, the models 
+        operations should be update during the iterations, for instance, the models
         in the potential.
 
         """
 
         return
-    
-    def run(self, init_node, iter_node=None, post_node=None, repeat=1, *args, **kwargs) -> None:
+
+    def run(
+        self, init_node, iter_node=None, post_node=None, repeat=1, *args, **kwargs
+    ) -> None:
         """"""
         # - init
-        self._print(("="*28+"{:^24s}"+"="*28+"\n").format("INIT"))
-        session = Session(self.directory/"init")
+        self._print(("=" * 28 + "{:^24s}" + "=" * 28 + "\n").format("INIT"))
+        session = Session(self.directory / "init")
         _ = session.run(init_node, feed_dict={})
         self._print("status: ", init_node.status)
 
         init_state = init_node.status
         if init_state != "finished":
             self._print("wait init session to finish...")
             return
 
         # - iter
-        curr_potter_node = init_node # a node that forwards a potter manager
+        curr_potter_node = init_node  # a node that forwards a potter manager
         for i in range(repeat):
-            self._print(("="*28+"{:^24s}"+"="*28+"\n").format(f"ITER.{str(i).zfill(4)}"))
-            session = Session(self.directory/f"iter.{str(i).zfill(4)}")
+            self._print(
+                ("=" * 28 + "{:^24s}" + "=" * 28 + "\n").format(
+                    f"ITER.{str(i).zfill(4)}"
+                )
+            )
+            session = Session(self.directory / f"iter.{str(i).zfill(4)}")
             # -- update some parameters
             curr_node = copy.deepcopy(iter_node)
             nodes_postorder = traverse_postorder(curr_node)
             # --- trainer
             # --- potter
             for x in nodes_postorder:
                 if x.__class__.__name__ == "drive":
@@ -315,15 +318,15 @@
         else:
             self._print(f"iter finished...")
 
         # - post
 
         return
 
-    def _irun(self, operation, feed_dict: dict={}) -> NoReturn:
+    def _irun(self, operation, feed_dict: dict = {}) -> NoReturn:
         """"""
         # - find forward order
         nodes_postorder = traverse_postorder(operation)
         self._print(
             "[{:^24s}] NUM_NODES: {} AT MAIN: {}".format(
                 "START", len(nodes_postorder), str(self.directory)
             )
@@ -331,34 +334,35 @@
 
         # - run nodes
         for i, node in enumerate(nodes_postorder):
             # NOTE: reset directory since it maybe changed
             prev_name = node.directory.name
             if not prev_name:
                 prev_name = node.__class__.__name__
-            node.directory = self.directory/f"{str(i).zfill(4)}.{prev_name}"
+            node.directory = self.directory / f"{str(i).zfill(4)}.{prev_name}"
             if node.__class__.__name__.endswith("Variable"):
                 node_type = "VX"
             else:
                 node_type = "OP"
             self._print(
                 "[{:^24s}] {:<36s} AT {}".format(
                     node_type, node.__class__.__name__.upper(), node.directory.name
                 )
             )
 
             if isinstance(node, Placeholder):
                 node.output = feed_dict[node]
             elif isinstance(node, Variable):
                 node.output = node.value
-            else: # Operation
+            else:  # Operation
                 if node.is_ready_to_forward():
                     node.inputs = [input_node.output for input_node in node.input_nodes]
                     node.output = node.forward(*node.inputs)
                 else:
                     print("wait previous nodes to finish...")
                     continue
 
         return
 
+
 if __name__ == "__main__":
     ...
```

### Comparing `gdpx-0.0.5/src/gdpx/core/session/basic.py` & `gdpx-0.0.6/src/gdpx/core/session/basic.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,44 +1,28 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
-import abc
-import copy
-import json
-from typing import NoReturn, Union, List, Callable
-import pathlib
-import yaml
-
-import numpy as np
 
-from ase import Atoms
-from ase.io import read, write
+import pathlib
 
-from .. import config
 from ..placeholder import Placeholder
 from ..variable import Variable
+from .session import AbstractSession
 from .utils import traverse_postorder
 
 
-class Session:
-
-    #: Standard print function.
-    _print: Callable = config._print
-
-    #: Standard debug function.
-    _debug: Callable = config._debug
-
+class Session(AbstractSession):
 
     def __init__(self, directory="./") -> None:
         """"""
         self.directory = pathlib.Path(directory)
 
         return
 
-    def run(self, operation, feed_dict: dict={}) -> None:
+    def run(self, operation, feed_dict: dict = {}) -> None:
         """"""
         # - find forward order
         nodes_postorder = traverse_postorder(operation)
         for node in nodes_postorder:
             if hasattr(node, "_active") and node._active:
                 node._active = False
                 self._print(
@@ -53,36 +37,31 @@
 
         # - run nodes
         for i, node in enumerate(nodes_postorder):
             # NOTE: reset directory since it maybe changed
             prev_name = node.directory.name
             if not prev_name:
                 prev_name = node.__class__.__name__
-            node.directory = self.directory/f"{str(i).zfill(4)}.{prev_name}"
+            node.directory = self.directory / f"{str(i).zfill(4)}.{prev_name}"
             if node.__class__.__name__.endswith("Variable"):
                 node_type = "VX"
             else:
                 node_type = "OP"
             self._print(
                 "[{:^24s}] NAME: {} AT {}".format(
                     node_type, node.__class__.__name__.upper(), node.directory.name
                 )
             )
 
             if isinstance(node, Placeholder):
                 node.output = feed_dict[node]
             elif isinstance(node, Variable):
                 node.output = node.value
-            else: # Operation
+            else:  # Operation
                 self._debug(f"node: {node}")
-                if node.is_ready_to_forward():
-                    node.inputs = [input_node.output for input_node in node.input_nodes]
-                    node.output = node.forward(*node.inputs)
-                else:
-                    self._print("wait previous nodes to finish...")
-                    continue
+                self._process_operation(node)
 
         return
 
 
 if __name__ == "__main__":
     ...
```

### Comparing `gdpx-0.0.5/src/gdpx/core/session/interface.py` & `gdpx-0.0.6/src/gdpx/core/session/interface.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,224 +1,264 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 import copy
 import json
 import logging
 import pathlib
+import time
 import traceback
 
 import yaml
 
 import omegaconf
 from omegaconf import OmegaConf
 
 from .. import config
-from .utils import create_variable, create_operation, traverse_postorder
+from .utils import create_variable, create_operation
 
-cache_nodes = {}
 
-def instantiate_variable(vx_name, vx_params):
-    """"""
-    print(f"----- {vx_name} -----")
-    params = {}
-    for k, v in vx_params.items():
-        print(k, v)
-        ...
+#: GLOBAL ATTR.
+cache_nodes = {}
 
-    return
+# def instantiate_variable(vx_name, vx_params):
+#     """"""
+#     print(f"----- {vx_name} -----")
+#     params = {}
+#     for k, v in vx_params.items():
+#         print(k, v)
+#         ...
+#
+#     return
+#
+# def resolve_variables(variables: dict):
+#     """"""
+#     for vx_name, vx_params in variables.items():
+#         vx = instantiate_variable(vx_name, vx_params)
+#         ...
+#
+#     return
 
-def resolve_variables(variables: dict):
-    """"""
-    for vx_name, vx_params in variables.items():
-        vx = instantiate_variable(vx_name, vx_params)
-        ...
-
-    return
 
 def instantiate_operation(op_name, op_params):
     """"""
-    #print(f"----- {op_name} -----")
     params = {}
     for k, v in op_params.items():
-        params[k] = v # resolve one by one...
+        params[k] = v  # resolve one by one...
     op = create_operation(op_name, op_params)
-    #print(op)
-    #print(op.input_nodes)
 
     return op
 
+
 def resolve_operations(config: dict):
     """"""
     operations = {}
     for op_name, op_params in config.items():
         op = instantiate_operation(op_name, op_params)
         operations[op_name] = op
         cache_nodes[op_name] = op
 
     return operations
 
-def run_session(config_filepath, feed_command=None, directory="./"):
-    """Configure session with omegaconfig."""
-    directory = pathlib.Path(directory)
+
+def register_custom_resolvers():
+    """"""
 
     # - add resolvers
     def create_vx_instance(vx_name, _root_):
         """"""
         if vx_name not in cache_nodes:
             vx_params = OmegaConf.to_object(_root_.variables.get(vx_name))
             vx = create_variable(vx_name, vx_params)
             cache_nodes[vx_name] = vx
             return vx
         else:
             return cache_nodes[vx_name]
 
-    OmegaConf.register_new_resolver(
-        "vx", create_vx_instance, use_cache=False
-    )
+    OmegaConf.register_new_resolver("vx", create_vx_instance, use_cache=False)
 
     def create_op_instance(op_name, _root_):
         """"""
         if op_name not in cache_nodes:
             op_params = OmegaConf.to_object(_root_.operations.get(op_name))
             op = create_operation(op_name, op_params)
             cache_nodes[op_name] = op
             return op
         else:
             return cache_nodes[op_name]
 
-    OmegaConf.register_new_resolver(
-        "op", create_op_instance, use_cache=False
-    )
+    OmegaConf.register_new_resolver("op", create_op_instance, use_cache=False)
 
     # --
     def read_json(input_file):
         with open(input_file, "r") as fopen:
             input_dict = json.load(fopen)
 
         return input_dict
 
-    OmegaConf.register_new_resolver(
-        "json", read_json
-    )
+    OmegaConf.register_new_resolver("json", read_json)
 
     def read_yaml(input_file):
         with open(input_file, "r") as fopen:
             input_dict = yaml.safe_load(fopen)
 
         return input_dict
 
-    OmegaConf.register_new_resolver(
-        "yaml", read_yaml
-    )
+    OmegaConf.register_new_resolver("yaml", read_yaml)
+
+    return
+
+
+def run_session_once(config_dict: dict, feed_command=None, directory="./"):
+    """Configure session with omegaconfig."""
+    # - set directory
+    directory = pathlib.Path(directory)
 
     # - load configuration and resolve it
-    conf = OmegaConf.load(config_filepath)
+    conf = OmegaConf.create(config_dict)
 
     # - add placeholders and their directories
     if "placeholders" not in conf:
         conf.placeholders = {}
     if feed_command is not None:
         pairs = [x.split("=") for x in feed_command]
         for k, v in pairs:
             if v.isdigit():
                 v = int(v)
             conf.placeholders[k] = v
     config._debug(f"YAML: {OmegaConf.to_yaml(conf)}")
 
     # - check operations and their directories
     for op_name, op_params in conf.operations.items():
-        op_params["directory"] = str(directory/op_name)
-    
+        op_params["directory"] = str(directory / op_name)
+
     # - set variable directory
     if "variables" not in conf:
         conf.variables = {}
     for k, v_dict in conf.variables.items():
-        v_dict["directory"] = str(directory/"variables"/k)
-    #print("YAML: ", OmegaConf.to_yaml(conf))
+        v_dict["directory"] = str(directory / "variables" / k)
+    # print("YAML: ", OmegaConf.to_yaml(conf))
 
     # - resolve sessions
-    #container = OmegaConf.to_object(conf.sessions)
-    #for k, v in container.items():
+    # container = OmegaConf.to_object(conf.sessions)
+    # for k, v in container.items():
     #    print(k, v)
 
     try:
         operations = resolve_operations(conf["operations"])
     except omegaconf.errors.InterpolationResolutionError as err:
-        config._debug (traceback.format_exc())
+        config._debug(traceback.format_exc())
         err_key = (str(err).strip().split("\n")[1]).strip().split(":")[1]
         config._print(f"FAILED TO PARSE `{err_key}` KEY.")
+        err_info_tail = traceback.format_exc().split("\n")[-10:]
+        for e in err_info_tail:
+            config._print(f"{e}")
         exit()
 
     container = {}
     for k, v in conf["sessions"].items():
         container[k] = operations[v]
 
     # - run session
     names = conf.placeholders.get("names", None)
     if names is not None:
         session_names = [x.strip() for x in names.strip().split(",")]
     else:
-        session_names =[None]*len(container)
-    
-    # - some imported packages change `logging.basicConfig` 
+        session_names = [None] * len(container)
+
+    # - some imported packages change `logging.basicConfig`
     #   and accidently add a StreamHandler to logging.root
     #   so remove it...
     for h in logging.root.handlers:
-        if isinstance(h, logging.StreamHandler) and not isinstance(h, logging.FileHandler):
+        if isinstance(h, logging.StreamHandler) and not isinstance(
+            h, logging.FileHandler
+        ):
             logging.root.removeHandler(h)
-    
+
     # - get session general configs
     sconfigs = conf.get("configs", {})
 
     exec_mode = sconfigs.get("mode", "basic")
-    if exec_mode == "basic": # sequential
+    if exec_mode == "basic":  # sequential
         from .basic import Session
-        # -- sequential
+
+        session_states = [True]
         for i, (k, v) in enumerate(container.items()):
             n = session_names[i]
             if n is None:
                 n = k
             entry_operation = v
-            session = Session(directory=directory/n)
+            session = Session(directory=directory / n)
             session.run(entry_operation, feed_dict={})
     elif exec_mode == "active":
         from .active import ActiveSession
+
         assert len(container) == 1, "ActiveSession only accepts one operation."
+
+        session_states = []
         for i, (k, v) in enumerate(container.items()):
             n = session_names[i]
             if n is None:
                 n = k
             entry_operation = v
             session = ActiveSession(
-                steps=sconfigs.get("steps", 2), 
+                steps=sconfigs.get("steps", 2),
                 reset_random_state=sconfigs.get("reset_random_state", False),
                 reset_random_config=sconfigs.get("reset_random_config", ("init", 0)),
-                directory=directory/n
+                directory=directory / n,
             )
             session.run(entry_operation, feed_dict={})
-    elif exec_mode == "cyc":
-        from .active import CyclicSession
-        # -- iterative
-        session = CyclicSession(directory="./")
-        session.run(
-            container["init"], container["iter"], container.get("post"),
-            repeat=conf.get("repeat", 1)
-        )
-    elif exec_mode == "otf":
-        config._print("Use OTF Session...")
-        from .active import OTFSession
-        for i, (k, v) in enumerate(container.items()):
-            n = session_names[i]
-            if n is None:
-                n = k
-            entry_operation = v
-            session = OTFSession(directory=directory/n)
-            session.run(entry_operation, feed_dict={})
+            # config._print(f"{session.state =}")
+            session_states.append(session.is_finished())
+            # config._print(f"{session.state =}")
     else:
+        session_states = [False]
         raise RuntimeError(f"Unknown session type {exec_mode}.")
 
+    return all(session_states)
+
+
+def run_session(
+    config_filepath: str,
+    feed_command=None,
+    timewait: float = -1.0,
+    directory: str = "./",
+):
+    """Configure session with omegaconfig."""
+    directory = pathlib.Path(directory)
+
+    config_filepath = pathlib.Path(config_filepath)
+
+    if config_filepath.suffix == ".json":
+        with open(config_filepath, "r") as fopen:
+            config_dict = json.load(fopen)
+    elif config_filepath.suffix == ".yaml":
+        with open(config_filepath, "r") as fopen:
+            config_dict = yaml.safe_load(fopen)
+    else:
+        raise RuntimeError(f"Fail to load config `{str(config_filepath)}`")
+
+    raw_config_dict = config_dict
+
+    register_custom_resolvers()
+
+    # -
+    if timewait > 0:
+        for i in range(1000):
+            config._print(f"Monitor is running step {i}!!!")
+            config_dict = copy.deepcopy(raw_config_dict)
+            is_finished = run_session_once(config_dict, feed_command, directory)
+            if is_finished:
+                break
+            else:
+                config._print(f"Monitor is sleeping for {timewait} seconds.")
+                time.sleep(timewait)
+        else:
+            config._print("Reach maximum monitor for-loop.")
+    else:
+        run_session_once(config_dict, feed_command, directory)
+
     return
 
 
 if __name__ == "__main__":
     ...
```

### Comparing `gdpx-0.0.5/src/gdpx/core/session/utils.py` & `gdpx-0.0.6/src/gdpx/core/session/utils.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.5/src/gdpx/core/variable.py` & `gdpx-0.0.6/src/gdpx/core/variable.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.5/src/gdpx/data/ClusterAndCUR.py` & `gdpx-0.0.6/src/gdpx/data/ClusterAndCUR.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.5/src/gdpx/data/analyser.py` & `gdpx-0.0.6/src/gdpx/data/analyser.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.5/src/gdpx/data/array.py` & `gdpx-0.0.6/src/gdpx/data/array.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,16 +29,18 @@
 RETAIEND_INFO_DTYPES: List[str] = [
     "i8", "i8",
     "f", "f", "f",
     "f", "f", "f",
     "f", "f", "f"
 ]
 
-#:
-RETAINED_CALC_PROPS: List[str] = ["energy", "forces"]
+#: Saved calculated property names.
+RETAINED_CALC_PROPS: List[str] = ["energy", "free_energy", "forces"]
+
+#: Saved calculated atomic property names.
 RETAINED_ATOMIC_CALC_PROPS: List[str] = ["forces"]
 
 
 def _flat_data(items):
     """"""
     # if not isinstance(ret, Atoms):
     if isinstance(items, list) and not isinstance(items[0], Atoms):
@@ -369,22 +371,32 @@
         for name, dtype in zip(RETAINED_INFO_NAMES, RETAIEND_INFO_DTYPES):
             data = [a.info.get(name, np.nan) for a in images]
             if not np.all(np.isnan(data)):
                 _ = grp.create_dataset(name, data=data, dtype=dtype)
 
         # -- calc props
         # TODO: without calc properties?
+        # NOTE: energy and forces have apply_constraint True...
         energies = np.array([a.get_potential_energy()
                             for a in images], dtype=np.float64)
+        free_energies = []
+        for i, a in enumerate(images):
+            try:
+                free_energy = a.get_potential_energy(force_consistent=True)
+            except: # Assume no free_energy property is available.
+                free_energy = energies[i]
+            free_energies.append(free_energy)
+
         # forces = np.array([a.get_forces() for a in images], dtype=np.float64)
         forces = np.zeros((nimages, max(natoms_list), 3), dtype=np.float64)
         for i, a in enumerate(images):
             forces[i, :natoms_list[i], :] = a.get_forces()
 
         ene_dset = grp.create_dataset("energy", data=energies, dtype="f8")
+        fen_dset = grp.create_dataset("free_energy", data=free_energies, dtype="f8")
         frc_dset = grp.create_dataset("forces", data=forces, dtype="f8")
 
         return
 
     # @classmethod
     # def squeeze(cls, axis=0):
     #    """Squeeze TODO: treat markers and map properly."""
```

### Comparing `gdpx-0.0.5/src/gdpx/data/cleave_deviation.py` & `gdpx-0.0.6/src/gdpx/data/cleave_deviation.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.5/src/gdpx/data/convert.py` & `gdpx-0.0.6/src/gdpx/data/convert.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.5/src/gdpx/data/correction.py` & `gdpx-0.0.6/src/gdpx/data/correction.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.5/src/gdpx/data/database.py` & `gdpx-0.0.6/src/gdpx/data/database.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.5/src/gdpx/data/extract_evolution.py` & `gdpx-0.0.6/src/gdpx/data/extract_evolution.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.5/src/gdpx/data/interface.py` & `gdpx-0.0.6/src/gdpx/data/interface.py`

 * *Files 4% similar despite different names*

```diff
@@ -247,25 +247,28 @@
 class transfer(Operation):
 
     """Transfer worker results to target destination.
     """
 
     def __init__(
         self, structures, dataset, version, 
-        prefix: str="", system: str="mixed", directory="./"
+        prefix: str="", system: str="mixed", clean_info: bool=False,
+        directory="./"
     ) -> None:
         """"""
         input_nodes = [structures, dataset]
         super().__init__(input_nodes=input_nodes, directory=directory)
 
         self.version = version
 
         self.prefix = prefix
         self.system = system # molecule/cluster, surface, bulk
 
+        self.clean_info = clean_info # whether clean atoms info
+
         return
     
     def forward(self, frames: List[Atoms], dataset):
         """"""
         super().forward()
 
         if isinstance(frames, AtomsNDArray):
@@ -300,14 +303,17 @@
             target_subdir = target_dir/dirname
             target_subdir.mkdir(parents=True, exist_ok=True)
 
             # -- save frames
             curr_frames = [frames[i] for i in curr_indices]
             curr_nframes = len(curr_frames)
 
+            if self.clean_info:
+                self._clean_frames(curr_frames)
+
             strname = self.version + ".xyz"
             target_destination = target_dir/dirname/strname
             if not target_destination.exists():
                 write(target_destination, curr_frames)
                 self._print(f"nframes {curr_nframes} -> {str(target_destination.relative_to(target_dir))}")
             else:
                 #warnings.warn(f"{target_destination} exists.", UserWarning)
@@ -316,14 +322,24 @@
             acc_nframes += curr_nframes
 
         assert nframes == acc_nframes
         
         self.status = "finished"
 
         return dataset
+    
+    def _clean_frames(self, frames: List[Atoms]):
+        """"""
+        for atoms in frames:
+            info_keys = copy.deepcopy(list(atoms.info.keys()))
+            for k in info_keys:
+                if k not in ["energy", "free_energy"]:
+                    del atoms.info[k]
+
+        return
 
 
 @registers.operation.register
 class scope(Operation):
 
     def __init__(
             self, dataset, describer,
```

### Comparing `gdpx-0.0.5/src/gdpx/data/operators.py` & `gdpx-0.0.6/src/gdpx/data/operators.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,17 +9,19 @@
 
 from ase import Atoms
 from ase.calculators.singlepoint import SinglePointCalculator
 from gdpx.utils.comparasion import parity_plot, parity_plot_dict, PropInfo
 
 
 import matplotlib as mpl
-mpl.use("Agg")  # silent mode
 from matplotlib import pyplot as plt
-plt.style.use("presentation")
+try:
+    plt.style.use("presentation")
+except:
+    ...
 
 
 def use_dpeval():
     import matplotlib as mpl
     mpl.use('Agg') #silent mode
     from matplotlib import pyplot as plt
     plt.style.use('presentation')
@@ -267,69 +269,14 @@
                     tot_props[prop] = [atoms.calc.results[prop]]
 
     if tot_props:
         return tot_energies, tot_forces, tot_props
     else:
         return tot_energies, tot_forces
 
-def set2frames(set_dir, chemical_symbols):
-    """ convert set into frames
-    """
-    frames = []
-    #boxes.extend( np.load(set_dir / 'box.npy') )
-    #coords.extend( np.load(set_dir / 'coord.npy') )
-    #energies.extend( np.load(set_dir / 'energy.npy') )
-    #forces.extend( np.load(set_dir / 'force.npy') )
-    boxes = np.load(set_dir / 'box.npy')
-    coords = np.load(set_dir / 'coord.npy')
-    energies = np.load(set_dir / 'energy.npy')
-    forces = np.load(set_dir / 'force.npy')
-    nframes = boxes.shape[0]
-    print('nframes in train', nframes)
-    for i in range(nframes):
-        cell = boxes[i,:].reshape(3,3)
-        positions = coords[i,:].reshape(-1,3)
-        atoms = Atoms(
-            symbols=chemical_symbols, positions=positions, cell=cell,
-            pbc=[1,1,1] # make atoms periodic
-        )
-        results = {'energy': energies[i], 'forces': forces[i,:].reshape(-1,3)}
-        spc = SinglePointCalculator(atoms, **results)
-        atoms.calc = spc
-        frames.append(atoms)
-
-    return frames
-
-def find_systems_set(cur_system: Union[str, pathlib.Path]):
-    # find all set dirs
-    set_dirs = []
-    for p in cur_system.glob('set*'):
-        set_dirs.append(p)
-    set_dirs.sort()
-
-    #inverse_type_map = dict(zip())
-    type_list = np.loadtxt(cur_system / 'type_map.raw', dtype=str)
-    atype = np.loadtxt(cur_system / 'type.raw', dtype=int)
-    chemical_symbols = [type_list[a] for a in atype]
-    #print(atype)
-
-    # train data
-    train_frames = []
-    for set_dir in set_dirs[:-1]:
-        train_frames.extend(set2frames(set_dir, chemical_symbols))
-
-    # test data
-    test_frames = []
-    for set_dir in set_dirs[-1:]:
-        test_frames.extend(set2frames(set_dir, chemical_symbols))
-
-
-    return train_frames, test_frames
-
-
 def calc_and_compare_results(frames, calc):
     """"""
     ref_energies, ref_forces = xyz2results(frames, calc=None)
     natoms_array = np.array([len(x) for x in frames])
 
     calc_name = calc.name.lower()
     #print("Calculating with MLP...")
```

### Comparing `gdpx-0.0.5/src/gdpx/data/system.py` & `gdpx-0.0.6/src/gdpx/data/system.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.5/src/gdpx/describer/describer.py` & `gdpx-0.0.6/src/gdpx/describer/describer.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.5/src/gdpx/describer/soap.py` & `gdpx-0.0.6/src/gdpx/describer/soap.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.5/src/gdpx/expedition/af/afir.py` & `gdpx-0.0.6/src/gdpx/expedition/af/afir.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 
 import numpy as np
 
 from ase import Atoms
 from ase.io import read, write
 from ase.formula import Formula
 
-from .. import Variable
 from .. import registers
 from .. import StructureBuilder
 from .. import ComputerVariable, DriverBasedWorker
 from ..expedition import AbstractExpedition
 
 from gdpx.worker.grid import GridDriverBasedWorker
 from gdpx.potential.interface import create_mixer
@@ -38,36 +37,14 @@
             Formula.from_list(symbols).format("hill")
         )
     #formulae = sorted(formulae)
 
     return formulae
 
 
-class ArtificialReactionVariable(Variable):
-
-    def __init__(self, builder, directory="./", *args, **kwargs) -> None:
-        """"""
-        if isinstance(builder, dict):
-            builder_params = copy.deepcopy(builder)
-            builder_method = builder_params.pop("method")
-            builder = registers.create(
-                "builder", builder_method, convert_name=False, **builder_params
-            )
-        elif isinstance(builder, StructureBuilder):
-            builder = builder
-        else:
-            raise RuntimeError(f"Unknown type {type(StructureBuilder)} for Builder.")
-
-        engine = AFIRSearch(builder, *args, **kwargs)
-
-        super().__init__(initial_value=engine, directory=directory)
-
-        return
-
-
 def find_target_fragments(atoms, target_commands: List[str]) -> Mapping[str,List[List[int]]]:
     """Find target fragments in the structure to react.
 
     This is a wrapper for group commands as there are several ways to defind
     a (atomic) group but we need a group of molecules here. Optional ways are 
     using `molecule` all, using `tag`...
```

### Comparing `gdpx-0.0.5/src/gdpx/expedition/bh/bh.py` & `gdpx-0.0.6/src/gdpx/expedition/monte_carlo/basin_hopping.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,28 +1,15 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 
 import copy 
 from typing import List
 
-from .. import registers, Variable, SingleWorker
-
-from ..expedition import AbstractExpedition
-from ..mc.mc import MonteCarlo, MonteCarloVariable
-
-
-class BasinHoppingVariable(MonteCarloVariable):
-
-    def _create_engine(self, builder, *args, **kwargs) -> None:
-        """"""
-        engine = BasinHopping(builder, *args, **kwargs)
-
-        return engine
-
+from .monte_carlo import MonteCarlo
 
 
 class BasinHopping(MonteCarlo):
 
     def __init__(
         self, builder: dict, operators: List[dict], 
         convergence: dict, random_seed=None, dump_period: int=1, ckpt_period: int=100,
```

### Comparing `gdpx-0.0.5/src/gdpx/expedition/ga/engine.py` & `gdpx-0.0.6/src/gdpx/expedition/ga/engine.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,38 +1,31 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 import copy
 import inspect
 import time
-from random import random
 import pathlib
-from pathlib import Path
 from typing import Callable, List
 import warnings
 
 import numpy as np
 
-import ase.data
 import ase.formula
 
 from ase import Atoms
 from ase.io import read, write
 from ase.ga.data import PrepareDB, DataConnection
 from ase.ga.population import Population
 from ase.ga.offspring_creator import OperationSelector
 
 from .population import AbstractPopulationManager
 
-from gdpx.core.variable import Variable
-from gdpx.core.register import registers
-from gdpx.utils.command import convert_indices
-from gdpx.worker.interface import ComputerVariable
-from gdpx.worker.drive import DriverBasedWorker, CommandDriverBasedWorker
-from gdpx.potential.managers.deepmd import DeepmdManager
+from .. import registers
+from .. import convert_indices
 from ..expedition import AbstractExpedition
 
 """
 TODO: search variational composition
 
 Workflow
     check current calculation
@@ -58,86 +51,54 @@
     comparator
     crossover (pairing)
     mutation
 
 """
 
 
-class GeneticAlgorithmVariable(Variable):
-
-    def __init__(self, builder, params: dict, directory="./", *args, **kwargs) -> None:
-        """"""
-        random_seed = kwargs.get("random_seed", None)
-        if random_seed is None:
-            random_seed = np.random.randint(0, 1e8)
-
-        # - builder
-        if isinstance(builder, dict):
-            builder_params = copy.deepcopy(builder)
-            builder_params.update(random_seed=random_seed)
-            builder_method = builder_params.pop("method")
-            builder = registers.create(
-                "builder", builder_method, convert_name=False, **builder_params
-            )
-        else: # variable
-            builder = builder.value
-            np.random.seed(random_seed)
-
-        # - worker
-        #if isinstance(worker, dict):
-        #    worker_params = copy.deepcopy(worker)
-        #    worker = registers.create("variable", "computer", convert_name=True, **worker_params).value[0]
-        #elif isinstance(worker, DriverBasedWorker):
-        #    worker = worker
-        #else: # computer variable
-        #    worker = worker.value[0]
-        engine = self._create_engine(builder, params, directory, *args, **kwargs)
-        super().__init__(initial_value=engine, directory=directory)
-
-        return
-    
-    def _create_engine(self, builder, params, directory, *args, **kwargs):
-        """"""
-        engine = GeneticAlgorithemEngine(builder, params, directory, *args, **kwargs)
-
-        return engine
-
-
 class GeneticAlgorithemEngine(AbstractExpedition):
+    """Genetic Algorithem Engine."""
 
-    """Genetic Algorithem Engine.
-    """
-
-    _directory = Path.cwd()
+    _directory = pathlib.Path.cwd()
 
     # local optimisation directory
     CALC_DIRNAME = "tmp_folder"
 
     #: Prefix of each generation's directory.
     GEN_PREFIX: str = "gen"
 
     # TODO: Neighbor list and parametrization parameters to screen
     # candidates before relaxation can be added. Default is not to use.
     find_neighbors = None
     perform_parametrization = None
 
-    def __init__(self, builder: dict, ga_dict: dict, directroy="./", random_seed=None, *args, **kwargs):
+    def __init__(
+        self,
+        builder: dict,
+        params: dict,
+        directroy="./",
+        random_seed=None,
+        *args,
+        **kwargs,
+    ):
         """Initialise engine.
 
         Args:
             builder: Define the system to explore.
 
         """
+        ga_dict = params # For compat
+
         # --- database ---
         self.db_name = ga_dict.get("database", "mydb.db")
 
-        # - 
+        # -
         self.directory = directroy
 
-        # - 
+        # -
         self.ga_dict = copy.deepcopy(ga_dict)
 
         # - random consistency, generator and population
         if random_seed is None:
             random_seed = np.random.randint(0, 1e8)
         self.random_seed = random_seed
         self._print(f"GA RANDOM SEED {random_seed}")
@@ -175,100 +136,80 @@
         # --- convergence ---
         self.conv_dict = ga_dict["convergence"]
 
         # - misc
         self.use_archive = ga_dict.get("use_archive", True)
 
         return
-    
+
     @property
     def directory(self):
         return self._directory
-    
+
     @directory.setter
     def directory(self, directory_):
         self._directory = pathlib.Path(directory_)
-        self.db_path = self._directory/self.db_name
+        self.db_path = self._directory / self.db_name
         return
 
     def report(self):
         self._print("restart the database...")
         self.da = DataConnection(self.db_path)
-        results = self.directory/"results"
+        results = self.directory / "results"
         if not results.exists():
             results.mkdir()
 
         # - write structures
         all_relaxed_candidates = self.da.get_all_relaxed_candidates()
-        write(results/"all_candidates.xyz", all_relaxed_candidates)
+        write(results / "all_candidates.xyz", all_relaxed_candidates)
 
         # - plot population evolution
         data = []
-        cur_gen_num = self.da.get_generation_number() # equals finished generation plus one
+        cur_gen_num = (
+            self.da.get_generation_number()
+        )  # equals finished generation plus one
         self._print(f"Current generation number: {cur_gen_num}")
         for i in range(cur_gen_num):
-            #print('generation ', i)
+            # print('generation ', i)
             energies = [
-                atoms.get_potential_energy() for atoms in all_relaxed_candidates 
-                    if atoms.info["key_value_pairs"]["generation"]==i
+                atoms.get_potential_energy()
+                for atoms in all_relaxed_candidates
+                if atoms.info["key_value_pairs"]["generation"] == i
             ]
             self._print(energies)
             data.append([i, energies])
 
         import matplotlib as mpl
-        mpl.use("Agg") #silent mode
+
+        mpl.use("Agg")  # silent mode
         from matplotlib import pyplot as plt
 
-        fig, ax = plt.subplots(nrows=1, ncols=1, figsize=(12,8))
-        ax.set_title(
-            "Population Evolution", 
-            fontsize=20, 
-            fontweight="bold"
-        )
+        fig, ax = plt.subplots(nrows=1, ncols=1, figsize=(12, 8))
+        ax.set_title("Population Evolution", fontsize=20, fontweight="bold")
 
         for i, energies in data:
-            ax.scatter([i]*len(energies), energies)
+            ax.scatter([i] * len(energies), energies)
 
-        plt.savefig(results/"pop.png")
+        plt.savefig(results / "pop.png")
 
         return
-    
-    def register_worker(self, worker: dict, *args, **kwargs):
-        """"""
-        if isinstance(worker, dict):
-            worker_params = copy.deepcopy(worker)
-            worker = registers.create(
-                "variable", "computer", convert_name=True, **worker_params
-            ).value[0]
-        elif isinstance(worker, list): # assume it is from a computervariable
-            worker = worker[0]
-        elif isinstance(worker, ComputerVariable):
-            worker = worker.value[0]
-        elif isinstance(worker, DriverBasedWorker):
-            worker = worker
-        else:
-            raise RuntimeError(f"Unknown worker type {worker}")
-        
-        self.worker = worker
 
-        return
-    
     def update_active_params(self, prev_wdir, *args, **kwargs):
         """"""
-        candidates = read(prev_wdir/"results"/"all_candidates.xyz", ":")
+        candidates = read(prev_wdir / "results" / "all_candidates.xyz", ":")
 
         init_size = self.pop_manager.init_size
         self.pop_manager.init_seed_file = candidates[:init_size]
 
         return
-    
+
     def run(self, *args, **kwargs):
         """Run the GA procedure several steps.
 
-        Default setting would run the algorithm many times until its convergence. 
+        Default setting would run the algorithm many times until its convergence.
         This is useful for running optimisations with serial worker.
 
         """
         # - outputs
         assert self.worker is not None, "GA has not set its worker properly."
         self.worker.directory = self.directory / self.CALC_DIRNAME
         self.pop_manager._print = self._print
@@ -308,364 +249,435 @@
                 break
             curr_convergence = self._irun()
             if not curr_convergence:
                 self._print("current generation does not converge...")
                 break
 
         return
-    
+
     def _check_generation(self):
         """"""
         # --- check current generation number
         self.cur_gen = self.da.get_generation_number()
         # output a few info
-        unrelaxed_strus_gen_ = list(self.da.c.select("relaxed=0,generation=%d" %self.cur_gen))
+        unrelaxed_strus_gen_ = list(
+            self.da.c.select("relaxed=0,generation=%d" % self.cur_gen)
+        )
         unrelaxed_strus_gen = []
         for row in unrelaxed_strus_gen_:
             # NOTE: mark_as_queue unrelaxed_candidate will have relaxed field too...
             if "queued" not in row:
                 unrelaxed_strus_gen.append(row)
         self.unrelaxed_confids = [row["gaid"] for row in unrelaxed_strus_gen]
         self.num_unrelaxed_gen = len(self.unrelaxed_confids)
 
-        relaxed_strus_gen = list(self.da.c.select("relaxed=1,generation=%d" %self.cur_gen))
+        relaxed_strus_gen = list(
+            self.da.c.select("relaxed=1,generation=%d" % self.cur_gen)
+        )
         for row in relaxed_strus_gen:
             self._debug(row)
         self.relaxed_confids = [row["gaid"] for row in relaxed_strus_gen]
         self.num_relaxed_gen = len(self.relaxed_confids)
 
         # check if this is the begin or the end of the current generation
-        self.beg_of_gen = (self.num_relaxed_gen == self.num_unrelaxed_gen) and (self.num_relaxed_gen == 0)
-        self.end_of_gen = (self.num_relaxed_gen == self.num_unrelaxed_gen) and (self.num_relaxed_gen != 0)
+        self.beg_of_gen = (self.num_relaxed_gen == self.num_unrelaxed_gen) and (
+            self.num_relaxed_gen == 0
+        )
+        self.end_of_gen = (self.num_relaxed_gen == self.num_unrelaxed_gen) and (
+            self.num_relaxed_gen != 0
+        )
 
         return
 
     def _irun(self):
-        """ main procedure
-        """
+        """main procedure"""
         if not hasattr(self, "cur_gen"):
-            raise RuntimeError("The current genertion is unknown. Check generation before.")
+            raise RuntimeError(
+                "The current genertion is unknown. Check generation before."
+            )
         # - generation
         self._print("\n\n===== Generation Info =====")
         self._print(f"current generation number: {self.cur_gen}")
         self._print(f"number of relaxed in current generation: {self.num_relaxed_gen}")
         self._print(convert_indices(sorted(self.relaxed_confids)))
-        self._print(f"number of unrelaxed in current generation: {self.num_unrelaxed_gen}")
+        self._print(
+            f"number of unrelaxed in current generation: {self.num_unrelaxed_gen}"
+        )
         self._print(convert_indices(sorted(self.unrelaxed_confids)))
         self._print(f"end of current generation: {self.end_of_gen}")
 
         # - population
         self._print("\n\n===== Population Info =====")
         content = "For generation > 0,\n"
         content += "{:>8s}  {:>8s}  {:>8s}  {:>8s}\n".format(
             "Reprod", "Random", "Mutate", "Total"
         )
         content += "{:>8d}  {:>8d}  {:>8d}  {:>8d}\n".format(
-            self.pop_manager.gen_rep_size, self.pop_manager.gen_ran_size,
-            self.pop_manager.gen_mut_size, self.pop_manager.gen_size
+            self.pop_manager.gen_rep_size,
+            self.pop_manager.gen_ran_size,
+            self.pop_manager.gen_mut_size,
+            self.pop_manager.gen_size,
         )
         content += "Note: Reproduced structure has a chance (pmut) to mutate.\n"
         self._print(content)
 
         # - minimise
         if self.cur_gen == 0:
             self._print("\n\n===== Initial Population Calculation =====")
             frames_to_work = []
-            while (self.da.get_number_of_unrelaxed_candidates()): # NOTE: this uses GADB get_atoms which adds extra_info
+            while (
+                self.da.get_number_of_unrelaxed_candidates()
+            ):  # NOTE: this uses GADB get_atoms which adds extra_info
                 # calculate structures from init population
                 atoms = self.da.get_an_unrelaxed_candidate()
                 frames_to_work.append(atoms)
-                self.da.mark_as_queued(atoms) # this marks relaxation is in the queue
+                self.da.mark_as_queued(atoms)  # this marks relaxation is in the queue
             confids = [a.info["confid"] for a in frames_to_work]
             self._print(f"start to run structure {convert_indices(confids)}")
             # NOTE: provide unified interface to mlp and dft
             if frames_to_work:
-                self.worker.directory = self.directory/self.CALC_DIRNAME/f"gen{self.cur_gen}"
-                _ = self.worker.run(frames_to_work) # retrieve later
+                self.worker.directory = (
+                    self.directory / self.CALC_DIRNAME / f"gen{self.cur_gen}"
+                )
+                _ = self.worker.run(frames_to_work)  # retrieve later
         else:
             # --- update population
             self._print("\n\n===== Update Population =====")
             # - create the population used for crossover and mutation
-            candidate_groups, num_paired, num_mutated, num_random = self.pop_manager._get_current_candidates(
-                database=self.da, curr_gen=self.cur_gen
+            candidate_groups, num_paired, num_mutated, num_random = (
+                self.pop_manager._get_current_candidates(
+                    database=self.da, curr_gen=self.cur_gen
+                )
             )
-            #candidate_groups, num_paired, num_mutated, num_random = self.pop_manager._get_current_candidates(
+            # candidate_groups, num_paired, num_mutated, num_random = self.pop_manager._get_current_candidates(
             #    database=self.da, curr_gen=self.cur_gen-1
-            #)
-            #for a in candidate_groups["paired"]:
+            # )
+            # for a in candidate_groups["paired"]:
             #    print(a.info)
 
             # TODO: random seed...
             current_population = Population(
-                data_connection = self.da,
-                population_size = self.pop_manager.gen_size,
-                comparator = self.comparing, 
-                rng = np.random # This is set when the generator is created
+                data_connection=self.da,
+                population_size=self.pop_manager.gen_size,
+                comparator=self.comparing,
+                rng=np.random,  # This is set when the generator is created
             )
             self.pop_manager._update_generation_settings(
                 current_population, self.mutations, self.pairing
             )
 
             # ----
             current_candidates = []
-            if self.beg_of_gen: # (num_relaxed == num_unrelaxed == 0)
-                # - 
+            if self.beg_of_gen:  # (num_relaxed == num_unrelaxed == 0)
+                # -
                 current_candidates = self.pop_manager._prepare_current_population(
-                    database=self.da, curr_gen=self.cur_gen, population=current_population, 
-                    generator=self.generator, pairing=self.pairing, mutations=self.mutations
+                    database=self.da,
+                    curr_gen=self.cur_gen,
+                    population=current_population,
+                    generator=self.generator,
+                    pairing=self.pairing,
+                    mutations=self.mutations,
                 )
             else:
                 self._print("Current generation has not finished...")
                 # NOTE: The current candidates have not been created completely.
                 #       For example, num_relaxed != num_unrelaxed,
                 #       need create more candidates...
-                if self.num_relaxed_gen == 0 and (self.num_unrelaxed_gen < self.pop_manager.gen_size):
+                if self.num_relaxed_gen == 0 and (
+                    self.num_unrelaxed_gen < self.pop_manager.gen_size
+                ):
                     current_candidates = self.pop_manager._prepare_current_population(
-                        database=self.da, curr_gen=self.cur_gen, population=current_population, 
-                        generator=self.generator, pairing=self.pairing, mutations=self.mutations,
-                        candidate_groups=candidate_groups, num_paired=num_paired, num_mutated=num_mutated, num_random=num_random
+                        database=self.da,
+                        curr_gen=self.cur_gen,
+                        population=current_population,
+                        generator=self.generator,
+                        pairing=self.pairing,
+                        mutations=self.mutations,
+                        candidate_groups=candidate_groups,
+                        num_paired=num_paired,
+                        num_mutated=num_mutated,
+                        num_random=num_random,
                     )
-                elif self.num_relaxed_gen == 0 and (self.num_unrelaxed_gen == self.pop_manager.gen_size):
+                elif self.num_relaxed_gen == 0 and (
+                    self.num_unrelaxed_gen == self.pop_manager.gen_size
+                ):
                     # no relaxed, and finished creation, num_relaxed == gen_size?
                     current_candidates = self.pop_manager._prepare_current_population(
-                        database=self.da, curr_gen=self.cur_gen, population=current_population, 
-                        generator=self.generator, pairing=self.pairing, mutations=self.mutations,
-                        candidate_groups=candidate_groups, num_paired=num_paired, num_mutated=num_mutated, num_random=num_random
+                        database=self.da,
+                        curr_gen=self.cur_gen,
+                        population=current_population,
+                        generator=self.generator,
+                        pairing=self.pairing,
+                        mutations=self.mutations,
+                        candidate_groups=candidate_groups,
+                        num_paired=num_paired,
+                        num_mutated=num_mutated,
+                        num_random=num_random,
                     )
                 else:
                     ...
-                
+
             # -- validate current candidates
-            #candidate_groups, num_paired, num_mutated, num_random = self.pop_manager._get_current_candidates(
+            # candidate_groups, num_paired, num_mutated, num_random = self.pop_manager._get_current_candidates(
             #    database=self.da, curr_gen=self.cur_gen
-            #)
-            #for ia, a in enumerate(candidate_groups["paired"]):
+            # )
+            # for ia, a in enumerate(candidate_groups["paired"]):
             #    self._print(f"{ia} {a.info}")
 
             # TODO: send candidates directly to worker that respects the batchsize
             self._print("\n")
             self._print("\n")
             self._print("===== Optimisation =====")
             for ia, a in enumerate(current_candidates):
                 self._print(f"{ia} {a.info}")
-            if not (self.directory/self.CALC_DIRNAME/f"gen{self.cur_gen}").exists():
+            if not (self.directory / self.CALC_DIRNAME / f"gen{self.cur_gen}").exists():
                 frames_to_work = []
                 for atoms in current_candidates:
-                    print(atoms.info)
                     frames_to_work.append(atoms)
-                    self.da.mark_as_queued(atoms) # this marks relaxation is in the queue
+                    self.da.mark_as_queued(
+                        atoms
+                    )  # this marks relaxation is in the queue
                 if frames_to_work:
                     confids = [a.info["confid"] for a in frames_to_work]
                     self._print(f"start to run structure {convert_indices(confids)}")
-                    self.worker.directory = self.directory/self.CALC_DIRNAME/f"gen{self.cur_gen}"
-                    _ = self.worker.run(frames_to_work) # retrieve later
+                    self.worker.directory = (
+                        self.directory / self.CALC_DIRNAME / f"gen{self.cur_gen}"
+                    )
+                    _ = self.worker.run(frames_to_work)  # retrieve later
             else:
-                self._print(f"calculation directory for generation {self.cur_gen} exists.")
+                self._print(
+                    f"calculation directory for generation {self.cur_gen} exists."
+                )
 
         # --- check if there were finished jobs
         curr_convergence = False
-        self.worker.directory = self.directory/self.CALC_DIRNAME/f"gen{self.cur_gen}"
+        self.worker.directory = (
+            self.directory / self.CALC_DIRNAME / f"gen{self.cur_gen}"
+        )
         self.worker.inspect(resubmit=True)
         if self.worker.get_number_of_running_jobs() == 0:
             self._print("\n\n===== Retrieve Relaxed Population =====")
-            converged_candidates = [t[-1] for t in self.worker.retrieve(use_archive=self.use_archive)]
+            converged_candidates = [
+                t[-1] for t in self.worker.retrieve(use_archive=self.use_archive)
+            ]
             for cand in converged_candidates:
                 self._print(cand)
                 self._print(cand.info)
                 # update extra info
-                extra_info = dict(
-                    data = {},
-                    key_value_pairs = {"extinct": 0}
-                )
+                extra_info = dict(data={}, key_value_pairs={"extinct": 0})
                 cand.info.update(extra_info)
                 # get tags
                 confid = cand.info["confid"]
                 if self.generator.use_tags:
                     rows = list(self.da.c.select(f"relaxed=0,gaid={confid}"))
                     for row in rows:
                         if row.formula:
-                            previous_atoms = row.toatoms(add_additional_information=True)
+                            previous_atoms = row.toatoms(
+                                add_additional_information=True
+                            )
                             previous_tags = previous_atoms.get_tags()
                             self._print(f"tags: {previous_tags}")
                             break
                     else:
                         raise RuntimeError(f"Cant find tags for cand {confid}")
                     cand.set_tags(previous_tags)
                 # evaluate raw score
                 self.evaluate_candidate(cand)
                 self._print(f"  add relaxed cand {confid}")
-                self._print("  with raw_score {:.4f}".format(cand.info["key_value_pairs"]["raw_score"]))
+                self._print(
+                    "  with raw_score {:.4f}".format(
+                        cand.info["key_value_pairs"]["raw_score"]
+                    )
+                )
                 self.da.add_relaxed_step(
                     cand,
                     find_neighbors=self.find_neighbors,
-                    perform_parametrization=self.perform_parametrization
+                    perform_parametrization=self.perform_parametrization,
                 )
             curr_convergence = True
         else:
             self._print("Worker is unfinished.")
 
         return curr_convergence
-    
+
     def get_workers(self):
         """Get all workers used by this expedition."""
         if not hasattr(self, "da"):
             self.da = DataConnection(self.db_path)
             self._check_generation()
-        
+
         num_gen = self.cur_gen
         if self.end_of_gen:
             num_gen += 1
 
         if hasattr(self.worker.potter, "remove_loaded_models"):
             self.worker.potter.remove_loaded_models()
-        
+
         workers = []
         for i in range(num_gen):
             curr_worker = copy.deepcopy(self.worker)
-            curr_worker.directory = self.directory/self.CALC_DIRNAME/(f"{self.GEN_PREFIX}{i}")
+            curr_worker.directory = (
+                self.directory / self.CALC_DIRNAME / (f"{self.GEN_PREFIX}{i}")
+            )
             workers.append(curr_worker)
 
         return workers
-    
+
     def read_convergence(self):
-        """ check whether the search is converged
-        """
+        """check whether the search is converged"""
         if not hasattr(self, "cur_gen"):
             self.da = DataConnection(self.db_path)
             self._check_generation()
         max_gen = self.conv_dict["generation"]
         if self.cur_gen > max_gen and (self.num_relaxed_gen == self.num_unrelaxed_gen):
             return True
         else:
             return False
-    
-    def _create_operator(self, op_params: dict, specific_params: dict, mod_name: str, convert_name=False):
-        """ Create operators such as comparator, crossover, and mutation.
+
+    def _create_operator(
+        self, op_params: dict, specific_params: dict, mod_name: str, convert_name=False
+    ):
+        """Create operators such as comparator, crossover, and mutation.
 
         Args:
             op_params: Operator parameters loaded from input file.
             specific_params: Operator parameters obtained based on system.
 
         """
         op_params = copy.deepcopy(op_params)
         method = op_params.pop("method", None)
         if method is None:
             raise RuntimeError(f"There is no operator {method}.")
         op_cls = registers.get(mod_name, method, convert_name=convert_name)
-        init_args = inspect.getargspec(op_cls.__init__).args[1:] # skip self
+        init_args = inspect.getargspec(op_cls.__init__).args[1:]  # skip self
         for k, v in specific_params.items():
             if k in init_args:
                 op_params.update(**{k: v})
         op = op_cls(**op_params)
 
         return op
-    
+
     def _register_operators(self):
-        """ register various operators
-            comparator, pairing, mutations
+        """register various operators
+        comparator, pairing, mutations
         """
         op_dict = copy.deepcopy(self.ga_dict.get("operators", None))
         if op_dict is None:
             op_dict = {
                 "comparator": {"name": "InteratomicDistanceComparator"},
-                "crossover": {"name": "CutAndSplicePairing"}
+                "crossover": {"name": "CutAndSplicePairing"},
             }
 
         specific_params = dict(
-            slab = self.da.get_slab(),
-            n_top = len(self.da.get_atom_numbers_to_optimize()),
-            blmin = self.generator.blmin,
-            number_of_variable_cell_vectors = self.generator.number_of_variable_cell_vectors,
-            cell_bounds = self.generator.cell_bounds,
-            test_dist_to_slab = self.generator.test_dist_to_slab,
-            use_tags = self.generator.use_tags,
-            used_modes_file = self.directory/self.CALC_DIRNAME/"used_modes.json",
-            #rng = self.rng # TODO: ase operators need np.random
+            slab=self.da.get_slab(),
+            n_top=len(self.da.get_atom_numbers_to_optimize()),
+            blmin=self.generator.blmin,
+            number_of_variable_cell_vectors=self.generator.number_of_variable_cell_vectors,
+            cell_bounds=self.generator.cell_bounds,
+            test_dist_to_slab=self.generator.test_dist_to_slab,
+            use_tags=self.generator.use_tags,
+            used_modes_file=self.directory / self.CALC_DIRNAME / "used_modes.json",
+            # rng = self.rng # TODO: ase operators need np.random
         )
 
         # --- comparator
         comp_params = op_dict.get("comparator", None)
-        self.comparing = self._create_operator(comp_params, specific_params, "comparator", convert_name=True)
+        self.comparing = self._create_operator(
+            comp_params, specific_params, "comparator", convert_name=True
+        )
 
         self._print("--- comparator ---")
         self._print(f"Use comparator {self.comparing.__class__.__name__}.")
 
         # --- crossover
         crossover_params = op_dict.get("crossover", None)
-        self.pairing = self._create_operator(crossover_params, specific_params, "builder", convert_name=False)
+        self.pairing = self._create_operator(
+            crossover_params, specific_params, "builder", convert_name=False
+        )
 
         self._print("--- crossover ---")
         self._print(f"Use crossover {self.pairing.__class__.__name__}.")
-        #self._print("pairing: ", self.pairing)
+        # self._print("pairing: ", self.pairing)
 
         # --- mutations
         mutations, probs = [], []
         mutation_list = op_dict.get("mutation", [])
         if not isinstance(mutation_list, list):
             mutation_list = [mutation_list]
         for mut_params in mutation_list:
             prob = mut_params.pop("prob", 1.0)
             probs.append(prob)
-            mut = self._create_operator(mut_params, specific_params, "builder", convert_name=False)
+            mut = self._create_operator(
+                mut_params, specific_params, "builder", convert_name=False
+            )
             mutations.append(mut)
 
         self._print("--- mutations ---")
-        #self._print(f"mutation probability: {self.pmut}")
+        # self._print(f"mutation probability: {self.pmut}")
         for mut, prob in zip(mutations, probs):
             self._print(f"Use mutation {mut.descriptor} with prob {prob}.")
         self.mutations = OperationSelector(probs, mutations, rng=np.random)
 
         return
-    
+
     def _create_initial_population(
-            self, 
-        ):
+        self,
+    ):
         # create the database to store information in
         # TODO: move this part to where before generator is created
         da = PrepareDB(
-            db_file_name = self.db_path,
-            simulation_cell = self.generator._substrate,
-            stoichiometry = self.generator.composition_atom_numbers
+            db_file_name=self.db_path,
+            simulation_cell=self.generator._substrate,
+            stoichiometry=self.generator.composition_atom_numbers,
         )
 
-        starting_population = self.pop_manager._prepare_initial_population(generator=self.generator)
+        starting_population = self.pop_manager._prepare_initial_population(
+            generator=self.generator
+        )
 
         self._print(f"save population {len(starting_population)} to database")
         for a in starting_population:
             da.add_unrelaxed_candidate(a)
-        
+
         # TODO: change this to the DB interface
-        self._print("save population size {0} into database...".format(self.pop_manager.gen_size))
+        self._print(
+            "save population size {0} into database...".format(
+                self.pop_manager.gen_size
+            )
+        )
         row = da.c.get(1)
         new_data = row["data"].copy()
         new_data["population_size"] = self.pop_manager.gen_size
         da.c.update(1, data=new_data)
 
         self.da = DataConnection(self.db_path)
 
         return
-    
+
     def evaluate_candidate(self, atoms):
-        """ TODO: evaluate candidate based on raw score
-            in most cases, it's potential energy
-            but this is should be more flexible
-            e.g. enthalpy (pot+pressure), reaction energy
+        """TODO: evaluate candidate based on raw score
+        in most cases, it's potential energy
+        but this is should be more flexible
+        e.g. enthalpy (pot+pressure), reaction energy
         """
-        assert atoms.info["key_value_pairs"].get("raw_score", None) is None, "candidate already has raw_score before evaluation"
-        
+        assert (
+            atoms.info["key_value_pairs"].get("raw_score", None) is None
+        ), "candidate already has raw_score before evaluation"
+
         # NOTE: larger raw_score, better candidate
 
         # evaluate based on target property
         target = self.prop_dict["target"]
         if target == "energy":
             energy = atoms.get_potential_energy()
             forces = atoms.get_forces()
             atoms.info["key_value_pairs"]["raw_score"] = -energy
             from ase.build import niggli_reduce
             from ase.calculators.singlepoint import SinglePointCalculator
+
             if self.generator.cell_bounds:
                 stress = atoms.get_stress()
                 niggli_reduce(atoms)
                 calc = SinglePointCalculator(
                     atoms, energy=energy, forces=forces, stress=stress
                 )
                 atoms.calc = calc
@@ -675,23 +687,24 @@
                     atoms.info["key_value_pairs"]["raw_score"] = -1e8
         elif target == "barrier":
             pass
         else:
             raise RuntimeError(f"Unknown target {target}...")
 
         return
-    
+
     def as_dict(self) -> dict:
         """"""
         engine_params = {}
         engine_params["random_seed"] = self.random_seed
         engine_params["method"] = "genetic_algorithm"
         engine_params["builder"] = self.generator.as_dict()
         engine_params["worker"] = self.worker.as_dict()
         engine_params["params"] = self.ga_dict
 
         engine_params = copy.deepcopy(engine_params)
 
         return engine_params
 
+
 if __name__ == "__main__":
     ...
```

### Comparing `gdpx-0.0.5/src/gdpx/expedition/ga/population.py` & `gdpx-0.0.6/src/gdpx/expedition/ga/population.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.5/src/gdpx/expedition/interface.py` & `gdpx-0.0.6/src/gdpx/expedition/interface.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,25 +1,67 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*
 
+
+import copy
 import logging
 import pathlib
 import time
 
+import numpy as np
+
 from .. import config
 from ..utils.command import parse_input_file
+from ..core.variable import Variable
 from ..core.operation import Operation
 from ..core.register import registers
 from ..worker.explore import ExpeditionBasedWorker
 from ..scheduler.interface import SchedulerVariable
 
 
 """
 """
 
+class ExpeditionVariable(Variable):
+
+    def __init__(self, directory="./", **kwargs):
+        """"""
+        random_seed = kwargs.get("random_seed", None)
+        if random_seed is None:
+            random_seed = np.random.randint(0, 1e8)
+
+        method = kwargs.pop("method", None)
+        if "builder" in kwargs:
+            builder = self._create_a_builder(kwargs["builder"], random_seed)
+            kwargs["builder"] = builder
+
+        expedition = registers.create(
+            "expedition", method, convert_name=False, **kwargs
+        )
+
+        super().__init__(initial_value=expedition, directory=directory)
+
+        return
+    
+    def _create_a_builder(self, builder: dict, random_seed: int):
+        """"""
+        # - builder
+        if isinstance(builder, dict):
+            builder_params = copy.deepcopy(builder)
+            builder_method = builder_params.pop("method")
+            builder = registers.create(
+                "builder", builder_method, convert_name=False, **builder_params
+            )
+        else:  # variable
+            builder = builder.value
+            np.random.seed(random_seed)
+        
+        return builder
+
+
 class explore(Operation):
 
     #: Whether to actively update some attrs.
     _active: bool = False
 
     def __init__(
         self, expedition, worker, scheduler=None, wait_time=60, 
@@ -86,22 +128,26 @@
         return basic_workers
 
 
 def run_expedition(exp_params: dict, wait: float=None, directory="./", potter=None):
     """"""
     directory = pathlib.Path(directory)
 
-    method = exp_params.pop("method")
     if potter is not None:
         exp_params["worker"] = potter
+    else:
+        if "worker" not in exp_params:
+            raise RuntimeError("Expedition must have a worker.")
 
     scheduler_params = exp_params.pop("scheduler", {})
     scheduler = SchedulerVariable(**scheduler_params).value
 
-    expedition = registers.create("variable", method, convert_name=True, **exp_params).value
+    #method = exp_params.pop("method")
+    #expedition = registers.create("variable", method, convert_name=True, **exp_params).value
+    expedition = ExpeditionVariable(directory=directory, **exp_params).value
     expedition.directory = directory
     if hasattr(expedition, "register_worker"):
         expedition.register_worker(exp_params["worker"])
 
     if scheduler.name == "local":
         if wait is not None:
             for i in range(1000):
```

### Comparing `gdpx-0.0.5/src/gdpx/expedition/mc/mc.py` & `gdpx-0.0.6/src/gdpx/expedition/monte_carlo/monte_carlo.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,52 +11,55 @@
 import pickle
 import tarfile
 from typing import NoReturn, List
 
 import numpy as np
 
 from ase import Atoms
+from ase import data, units
 from ase.io import read, write
+from ase.formula import Formula
+from ase.ga.utilities import closest_distances_generator
 
 from .. import registers
-from .. import Variable
-from .. import SingleWorker
+from .. import SingleWorker, DriverBasedWorker
+from .. import dict2str
 from ..expedition import AbstractExpedition
 from .operators import select_operator, parse_operators, save_operator, load_operator
 
 """This module tries to offer a base class for all MonteCarlo-like methods.
 """
 
 
-class MonteCarloVariable(Variable):
-
-    def __init__(self, builder, directory="./", *args, **kwargs) -> None:
-        """"""
-        # - builder
-        if isinstance(builder, dict):
-            builder_params = copy.deepcopy(builder)
-            builder_method = builder_params.pop("method")
-            builder = registers.create(
-                "builder", builder_method, convert_name=False, **builder_params
-            )
-        else:  # variable
-            builder = builder.value
-
-        # - engine
-        engine = self._create_engine(builder, *args, **kwargs)
-        engine.directory = directory
-        super().__init__(initial_value=engine, directory=directory)
-
-        return
-
-    def _create_engine(self, builder, *args, **kwargs) -> None:
-        """"""
-        engine = MonteCarlo(builder, *args, **kwargs)
+def convert_blmin_to_str(blmin: dict) -> str:
+    """"""
+    elements = []
+    for k in blmin.keys():
+        elements.extend(k)
+    elements = set(elements)
+    nelements = len(elements)
+
+    index_map = {}
+    for i, e in enumerate(elements):
+        index_map[e] = i
+    distance_map = np.zeros((nelements, nelements))
+    for (i, j), dis in blmin.items():
+        distance_map[index_map[i], index_map[j]] = dis
+
+    symbols = [data.chemical_symbols[e] for e in elements]
+
+    content = "Bond Distance Minimum\n"
+    # content += "  covalent ratio: {}\n".format(covalent_min)
+    content += "  " + " " * 4 + ("{:>6}  " * nelements).format(*symbols) + "\n"
+    for i, s in enumerate(symbols):
+        content += "  " + ("{:<4}" + "{:>8.4f}" * nelements + "\n").format(
+            s, *list(distance_map[i])
+        )
 
-        return engine
+    return content
 
 
 class MonteCarlo(AbstractExpedition):
 
     restart = False
 
     #: Prefix of the working directory.
@@ -127,15 +130,15 @@
 
         return
 
     def _init_structure(self):
         """Initialise the input structure.
 
         Set proper tags and minimise the structure. Prepare `self.atoms`,
-        `self.energy_stored`, and `self.curr_step`.
+        `self.energy_stored`, and `self.start_step`.
 
         """
         step_wdir = self.directory / f"{self.WDIR_PREFIX}0"
         if not step_wdir.exists():
             # - prepare atoms
             self._print("===== MonteCarlo Structure =====\n")
             tags = self.atoms.arrays.get("tags", None)
@@ -171,69 +174,107 @@
             self.energy_stored = curr_atoms.get_potential_energy()
             self._print(f"ene: {self.energy_stored}")
             self.atoms = curr_atoms
             self.atoms.set_tags(curr_tags)
             write(self.directory / self.TRAJ_NAME, self.atoms)
 
             # -
-            self.curr_step = 0
+            self.start_step = 0
 
             # - log operator status
             with open(self.directory / self.INFO_NAME, "w") as fopen:
                 fopen.write(
                     "{:<24s}  {:<24s}  {:<12s}  {:<12s}  {:<24s}  {:<24s}  \n".format(
                         "#Operator", "Info", "natoms", "Success", "prev_ene", "curr_ene"
                     )
                 )
             step_converged = True
         else:
             step_converged = False
 
         return step_converged
 
+    def _attach_bond_length_minimum_list(
+        self,
+    ):
+        """"""
+        type_list = []
+        for op in self.operators:
+            # TODO: wee need further unify the names here
+            if hasattr(op, "particles"):
+                for p in op.particles:
+                    type_list.extend(list(Formula(p).count().keys()))
+            elif hasattr(op, "reservoir"):
+                type_list.extend(list(Formula(op.reservoir["species"]).count().keys()))
+            else:
+                ...
+        type_list = list(set(type_list))
+        self._print(f"{type_list =}")
+        unique_atomic_numbers = [data.atomic_numbers[a] for a in type_list]
+
+        for op in self.operators:
+            op.blmin = closest_distances_generator(
+                atom_numbers=unique_atomic_numbers,
+                ratio_of_covalent_radii=op.covalent_min,
+            )
+
+        return
+
     def run(self, *args, **kwargs):
         """Run MonteCarlo simulation."""
         # - some imported packages change `logging.basicConfig`
         #   and accidently add a StreamHandler to logging.root
         #   so remove it...
         for h in logging.root.handlers:
             if isinstance(h, logging.StreamHandler) and not isinstance(
                 h, logging.FileHandler
             ):
                 logging.root.removeHandler(h)
 
         # - check if it has a valid worker..
         assert self.worker is not None, "MC has not set its worker properly."
+        if isinstance(self.worker, DriverBasedWorker):
+            self._print("Convert a DriverBasedWorker to a SingleWorker.")
+            self.worker = SingleWorker.from_a_worker(self.worker)
         assert isinstance(
             self.worker, SingleWorker
         ), f"{self.__class__.__name__} only supports SingleWorker (set use_single=True)."
         self.worker.directory = self.directory
 
         # - prepare logger and output some basic info...
         if not self.directory.exists():
             self.directory.mkdir(parents=True)
 
+        # - show operator information
         self._print("===== MonteCarlo Operators (Modifiers) =====\n")
+
+        # -- register bond list
+        self._attach_bond_length_minimum_list()
+
         for op in self.operators:
             for x in str(op).split("\n"):
                 self._print(x)
+            for l in convert_blmin_to_str(op.blmin).split("\n"):
+                self._print(l)
         self._print(f"normalised probabilities {self.op_probs}\n")
 
         # -- add print function to operators
         for op in self.operators:
             op._print = self._print
+            op._debug = self._debug
 
         # NOTE: check if operators' regions are consistent
         #       though it works, unexpected results may occur
         # TODO: need rewrite eq function as compare array is difficult
         # noperators = len(self.operators)
         # for i in range(1,noperators):
         #    if self.operators[i].region != self.operators[i-1].region:
         #        raise RuntimeError(f"Inconsistent region found in op {i-1} and op {i}")
 
+        # - start!!!
         converged = self.read_convergence()
         if not converged:
             # - init structure
             # --
             step_converged = False
             if not self._veri_checkpoint():
                 step_converged = self._init_structure()
@@ -241,51 +282,62 @@
                 step_converged = True
                 self._load_checkpoint()
 
             if not step_converged:
                 self._print("Wait structure to initialise.")
                 return
             else:
-                self.curr_step += 1
+                self.start_step += 1
 
             # - run mc steps
-            step_converged = False
-            for i in range(self.curr_step, self.convergence["steps"] + 1):
-                self._print(f"RANDOM_SEED:  {self.random_seed}")
-                self._print(f"RANDOM_STATE: {self.rng.bit_generator.state}")
-                step_converged = self._irun(i)
-                if not step_converged:
+            curr_step = self.start_step  # start_step
+            while True:
+                if curr_step > self.convergence["steps"]:
+                    break
+                step_state = self._irun(curr_step)
+                if step_state == "UNFINISHED":
                     self._print("Wait MC step to finish.")
                     break
-                else:
+                elif step_state == "FINISHED":
                     # -- save checkpoint
-                    self._save_checkpoint(step=i)
+                    self._save_checkpoint(step=curr_step)
                     # -- clean up
-                    if ((self.directory / f"{self.WDIR_PREFIX}{i}").exists()) and (
-                        i % self.dump_period != 0
-                    ):
-                        shutil.rmtree(self.directory / f"{self.WDIR_PREFIX}{i}")
-            else:
-                self._print("MC is converged...")
+                    if (
+                        (self.directory / f"{self.WDIR_PREFIX}{curr_step}").exists()
+                    ) and (curr_step % self.dump_period != 0):
+                        shutil.rmtree(self.directory / f"{self.WDIR_PREFIX}{curr_step}")
+                    curr_step += 1
+                elif step_state == "FAILED":
+                    self._print(f"RETRY STEP {curr_step}.")
+                else:
+                    ...  # This should not happen.
         else:
             self._print("Monte Carlo is converged.")
 
         return
 
-    def _irun(self, i):
-        """Run a single MC step."""
+    def _irun(self, i: int) -> str:
+        """Run a single MC step.
+
+        Each step has three status as FINISHED, UNFINISHED, and FAILED.
+
+        """
         self._print(f"===== MC Step {i} =====")
+        self._print(f"RANDOM_SEED:  {self.random_seed}")
+        for l in dict2str(self.rng.bit_generator.state).split("\n"):
+            self._print(l)
+
         step_wdir = self.directory / f"{self.WDIR_PREFIX}{i}"
         self.worker.wdir_name = step_wdir.name
 
         # - operate atoms
         curr_op = select_operator(self.operators, self.op_probs, self.rng)
         self._print(f"operator {curr_op.__class__.__name__}")
         curr_atoms = curr_op.run(self.atoms, self.rng)
-        if curr_atoms:
+        if curr_atoms:  # is not None
             # --- add info
             curr_atoms.info["confid"] = int(f"{i}")
             curr_atoms.info["step"] = -1  # NOTE: remove step info from driver
         else:
             self._print("FAILED to run operation...")
 
         # - run postprocess
@@ -315,23 +367,22 @@
                     self.energy_stored = self.energy_operated
                     self.atoms = curr_atoms
                     self._print("success...")
                 else:
                     self._print("failure...")
                 write(self.directory / self.TRAJ_NAME, self.atoms, append=True)
 
-                step_converged = True
+                step_state = "FINISHED"
             else:
-                step_converged = False
+                step_state = "UNFINISHED"
         else:
             # save the previous structure as the current operation gives no structure.
-            step_converged = True
-            write(self.directory / self.TRAJ_NAME, self.atoms, append=True)
+            step_state = "FAILED"
 
-        return step_converged
+        return step_state
 
     def _veri_checkpoint(self) -> bool:
         """Verify checkpoints."""
         ckpt_wdirs = list(self.directory.glob("checkpoint.*"))
         nwdirs = len(ckpt_wdirs)
 
         verified = True
@@ -380,34 +431,41 @@
 
         saved_operators = []
         for i, op_file in enumerate(op_files):
             saved_operator = load_operator(op_file)
             saved_operators.append(saved_operator)
         self.operators = saved_operators
 
+        self._attach_bond_length_minimum_list()
+
         # -- add print function to operators
         for op in self.operators:
             op._print = self._print
+            op._debug = self._debug
 
         self._print("===== Saved MonteCarlo Operators (Modifiers) =====\n")
         for op in self.operators:
             for x in str(op).split("\n"):
                 self._print(x)
         self._print(f"normalised probabilities {self.op_probs}\n")
 
         # -- load random state
         with open(ckpt_wdir / "rng.ckpt", "rb") as fopen:
             rng_state = pickle.load(fopen)
         self.rng.bit_generator.state = rng_state
 
         # -- load structure
-        self.curr_step = step
+        self.start_step = step
         self.atoms = read(ckpt_wdir / "structure.xyz")
         self.energy_stored = self.atoms.get_potential_energy()
 
+        # -- reset mctraj
+        mctraj = read(self.directory / self.TRAJ_NAME, f":{step+1}")
+        write(self.directory / self.TRAJ_NAME, mctraj)
+
         return
 
     def _save_step_info(self, curr_op, success: bool):
         """"""
         extra_info = getattr(curr_op, "_extra_info", "-")
         with open(self.directory / self.INFO_NAME, "a") as fopen:
             fopen.write(
@@ -430,29 +488,29 @@
         steps.
 
         """
         converged = False
         if (self.directory / self.TRAJ_NAME).exists():
             mctraj = read(self.directory / self.TRAJ_NAME, ":")
             nframes = len(mctraj)
-            # self.curr_step = nframes
+            # self.start_step = nframes
             if nframes > self.convergence["steps"]:
                 converged = True
         else:
             ...
 
         return converged
 
     def get_workers(self):
         """Get all workers used by this expedition."""
         if hasattr(self.worker.potter, "remove_loaded_models"):
             self.worker.potter.remove_loaded_models()
 
-        #workers = []
-        #for curr_wdir in wdirs:
+        # workers = []
+        # for curr_wdir in wdirs:
         #    curr_worker = copy.deepcopy(self.worker)
         #    curr_worker.directory = curr_wdir.parent
         #    curr_worker.wdir_name = curr_wdir.name
         #    workers.append(curr_worker)
         curr_worker = copy.deepcopy(self.worker)
         curr_worker.directory = self.directory
         curr_worker._retrieve_mode = "all"
```

### Comparing `gdpx-0.0.5/src/gdpx/expedition/mc/operators/__init__.py` & `gdpx-0.0.6/src/gdpx/expedition/monte_carlo/operators/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,18 +4,19 @@
 import pickle
 
 import numpy as np
 
 from ase import Atoms
 from ase import data, units
 
-from gdpx.builder.species import build_species
+from .. import convert_string_to_atoms
 from .move import MoveOperator
 from .swap import SwapOperator
 from .exchange import ExchangeOperator
+from .react import ReactOperator
 
 def save_operator(op, p):
     """"""
     with open(p, "wb") as fopen:
         pickle.dump(op, fopen)
 
     return
@@ -47,14 +48,16 @@
         prob = param.get("prob", 1.0)
         if name == "move":
             op = MoveOperator(**param)
         elif name == "swap":
             op = SwapOperator(**param)
         elif name == "exchange":
             op = ExchangeOperator(**param)
+        elif name == "react":
+            op = ReactOperator(**param)
         else:
             raise NotImplementedError(f"{name} is not supported.")
         operators.append(op)
         probs.append(prob)
     
     # - reweight probabilities
     probs = (np.array(probs) / np.sum(probs)).tolist()
@@ -65,15 +68,15 @@
     # - beta
     kBT_eV = units.kB * temperature
     beta = 1./kBT_eV # 1/(kb*T), eV
 
     # - cubic thermo de broglie 
     hplanck = units._hplanck # J/Hz = kg*m2*s-1
     #_mass = np.sum([data.atomic_masses[data.atomic_numbers[e]] for e in expart]) # g/mol
-    _species = build_species(expart)
+    _species = convert_string_to_atoms(expart)
     _species_mass = np.sum(_species.get_masses())
     #print("species mass: ", _mass)
     _mass = _species_mass * units._amu
     kbT_J = kBT_eV * units._e # J = kg*m2*s-2
     cubic_wavelength = (hplanck/np.sqrt(2*np.pi*_mass*kbT_J)*1e10)**3 # thermal de broglie wavelength
 
     return _species_mass, beta, cubic_wavelength
```

### Comparing `gdpx-0.0.5/src/gdpx/expedition/mc/operators/exchange.py` & `gdpx-0.0.6/src/gdpx/expedition/monte_carlo/operators/exchange.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,141 +8,151 @@
 
 import numpy as np
 
 from ase import Atoms
 from ase import data, units
 from ase.md.velocitydistribution import MaxwellBoltzmannDistribution
 from ase.neighborlist import NeighborList, natural_cutoffs
-from ase.ga.utilities import closest_distances_generator
-
-from gdpx.builder.group import create_a_group
-from gdpx.builder.species import build_species
 
+from .. import convert_string_to_atoms
 from .operator import AbstractOperator
 
 
-class ExchangeOperator(AbstractOperator):
-
-    name: str = "exchange"
-
-    MIN_RANDOM_TAG = 10000
-    MAX_RANDOM_TAG = 100000
-
-    #: The current suboperation (insert or remove).
-    _curr_operation: str = None # insert or remove
+class BasicExchangeOperator(AbstractOperator):
 
-    #: The current tags dict.
-    _curr_tags_dict: dict = None
+    MIN_RANDOM_TAG: int = 10000
 
-    #: The current accpetable volume.
-    _curr_volume: float = None
+    MAX_RANDOM_TAG: int = 100000
 
-    def __init__(
-        self, region: dict, reservoir: dict, temperature: float=300., pressure: float=1.,
-        covalent_ratio=[0.8,2.0], use_rotation: bool=True, use_bias: bool=True, 
-        *args, **kwargs
-    ):
-        """"""
-        super().__init__(
-            region=region, temperature=temperature, pressure=pressure, 
-            covalent_ratio=covalent_ratio, use_rotation=use_rotation,
-            *args, **kwargs
-        )
-
-        self.species = reservoir["species"]
-        self.mu = reservoir["mu"]
-
-        self.use_bias = use_bias
-
-        return
-    
-    def _insert(self, atoms_, species: str, rng):
+    def _insert(self, atoms_, species: str, rng=np.random.Generator(np.random.PCG64())):
         """"""
         atoms = atoms_.copy()
 
-        # - prepare
-        adpart = build_species(species) # particle to add
-        
+        # - prepare particle to add
+        adpart = convert_string_to_atoms(species)
+
         # - add velocity in case the mixed MC/MD is performed
         MaxwellBoltzmannDistribution(adpart, temperature_K=self.temperature, rng=rng)
 
         # - add tag
         used_tags = set(atoms.get_tags().tolist())
         adpart_tag = 0
         while adpart_tag in used_tags:
             # NOTE: np.random only has randint
             adpart_tag = rng.integers(self.MIN_RANDOM_TAG, self.MAX_RANDOM_TAG)
         adpart_tag = int(adpart_tag)
-        self._print(f"adpart tag: {adpart_tag} {type(adpart_tag)}")
+        self._print(
+            f"adpart {adpart.get_chemical_formula()} tag: {adpart_tag} {type(adpart_tag)}"
+        )
         # NOTE: ase accepts int or list as tags
         adpart.set_tags(adpart_tag)
 
         # - add particle
         atoms.extend(adpart)
 
         # - find species indices
         #   NOTE: adpart is always added to the end
         species_indices = [i for i, t in enumerate(atoms.get_tags()) if t == adpart_tag]
 
-        # - init blmin
+        # - blmin is initialised by MC
         cell = atoms.get_cell(complete=True)
-        chemical_symbols = atoms.get_chemical_symbols()
-
-        type_list = list(set(chemical_symbols))
-        unique_atomic_numbers = [data.atomic_numbers[a] for a in type_list]
-        self.blmin = closest_distances_generator(
-            atom_numbers=unique_atomic_numbers,
-            ratio_of_covalent_radii = self.covalent_min # be careful with test too far
-        )
 
         # - neighbour list
         nl = NeighborList(
-            self.covalent_max*np.array(natural_cutoffs(atoms)), 
-            skin=0.0, self_interaction=False, bothways=True
+            self.covalent_max * np.array(natural_cutoffs(atoms)),
+            skin=0.0,
+            self_interaction=False,
+            bothways=True,
         )
 
         # - get a random position
         species = atoms[species_indices]
         org_com = np.mean(species.positions, axis=0)
         org_positions = species.positions.copy()
 
         for i in range(self.MAX_RANDOM_ATTEMPTS):
             # - make a copy
             species_ = self._rotate_species(species, rng=rng)
             curr_cop = np.average(species_.positions, axis=0)
-            ran_pos = self.region.get_random_positions(size=1,rng=rng)[0]
+            ran_pos = self.region.get_random_positions(size=1, rng=rng)[0]
             new_vec = ran_pos - curr_cop
             species_.translate(new_vec)
             atoms.positions[species_indices] = copy.deepcopy(species_.positions)
             if not self.check_overlap_neighbour(nl, atoms, cell, species_indices):
                 self._print(f"succeed to insert after {i+1} attempts...")
                 self._print(f"original position: {org_com}")
                 self._print(f"random position: {ran_pos}")
-                self._print(f"actual position: {np.average(atoms.positions[species_indices], axis=0)}")
+                self._print(
+                    f"actual position: {np.average(atoms.positions[species_indices], axis=0)}"
+                )
                 break
             atoms.positions[species_indices] = org_positions
         else:
             # -- remove adpart since the insertion fails
             del atoms[species_indices]
             atoms = None
 
         return atoms
-    
-    def _remove(self, atoms_, species: str, rng):
+
+    def _remove(self, atoms_, species: str, rng=np.random.Generator(np.random.PCG64())):
         """"""
         atoms = atoms_.copy()
 
         # - pick a random atom/molecule
         species_indices = self._select_species(atoms, [species], rng)
-        
+
         # - remove then
         del atoms[species_indices]
 
         return atoms
-    
+
+
+class ExchangeOperator(BasicExchangeOperator):
+
+    name: str = "exchange"
+
+    #: The current suboperation (insert or remove).
+    _curr_operation: str = None  # insert or remove
+
+    #: The current tags dict.
+    _curr_tags_dict: dict = None
+
+    #: The current accpetable volume.
+    _curr_volume: float = None
+
+    def __init__(
+        self,
+        region: dict,
+        reservoir: dict,
+        temperature: float = 300.0,
+        pressure: float = 1.0,
+        covalent_ratio=[0.8, 2.0],
+        use_rotation: bool = True,
+        use_bias: bool = True,
+        *args,
+        **kwargs,
+    ):
+        """"""
+        super().__init__(
+            region=region,
+            temperature=temperature,
+            pressure=pressure,
+            covalent_ratio=covalent_ratio,
+            use_rotation=use_rotation,
+            *args,
+            **kwargs,
+        )
+
+        self.species = reservoir["species"]
+        self.mu = reservoir["mu"]
+
+        self.use_bias = use_bias
+
+        return
+
     def run(self, atoms: Atoms, rng=np.random) -> Atoms:
         """"""
         super().run(atoms)
         self._extra_info = "-"
 
         # -- compute acceptable volume
         if self.use_bias:
@@ -150,146 +160,117 @@
             acc_volume = self.region.get_empty_volume(atoms)
         else:
             # --- get normal region
             acc_volume = self.region.get_volume()
         self._curr_volume = acc_volume
 
         # - choose a species to exchange
-        #valid_species = [k for k, v in tag_dict.items() if len(v) > 0]
+        # valid_species = [k for k, v in tag_dict.items() if len(v) > 0]
         nparticles = len(self._curr_tags_dict.get(self.species, []))
 
         # - choose insert or remove
         if nparticles > 0:
             rn_ex = rng.uniform()
             if rn_ex < 0.5:
                 self._print("...insert...")
                 self._curr_operation = "insert"
                 curr_atoms = self._insert(atoms, self.species, rng)
-                self._extra_info = f"Insert {self.species}"
+                self._extra_info = f"Insert_{self.species}"
             else:
                 self._print("...remove...")
                 self._curr_operation = "remove"
                 curr_atoms = self._remove(atoms, self.species, rng)
-                self._extra_info = f"Remove {self.species}"
+                self._extra_info = f"Remove_{self.species}"
         else:
             self._print("...insert...")
             self._curr_operation = "insert"
             curr_atoms = self._insert(atoms, self.species, rng)
-            self._extra_info = f"Insert {self.species}"
+            self._extra_info = f"Insert_{self.species}"
 
         return curr_atoms
 
-    def check_overlap_neighbour(
-        self, nl, new_atoms, cell, species_indices: List[int]
-    ):
-        """ use neighbour list to check newly added atom is neither too close or too
-            far from other atoms
-        """
-        # - get symbols here since some operators may change the symbol
-        chemical_symbols = new_atoms.get_chemical_symbols()
-
-        overlapped = False
-        nl.update(new_atoms)
-        for idx_pick in species_indices:
-            self._print(f"- check index {idx_pick} {new_atoms.positions[idx_pick]}")
-            indices, offsets = nl.get_neighbors(idx_pick)
-            if len(indices) > 0:
-                self._print(f"nneighs: {len(indices)}")
-                # should close to other atoms
-                for ni, offset in zip(indices, offsets):
-                    dis = np.linalg.norm(new_atoms.positions[idx_pick] - (new_atoms.positions[ni] + np.dot(offset, cell)))
-                    pairs = [chemical_symbols[ni], chemical_symbols[idx_pick]]
-                    pairs = tuple([data.atomic_numbers[p] for p in pairs])
-                    #print("distance: ", ni, dis, self.blmin[pairs])
-                    if dis < self.blmin[pairs]:
-                        overlapped = True
-                        break
-            else:
-                # TODO: is no neighbours valid?
-                self._print("no neighbours, being isolated...")
-                overlapped = True
-                break
-
-        return overlapped
-    
     def metropolis(self, prev_ene: float, curr_ene: float, rng=np.random) -> bool:
         """"""
         # - acceptance ratio
         kBT_eV = units.kB * self.temperature
-        beta = 1./kBT_eV # 1/(kb*T), eV
+        beta = 1.0 / kBT_eV  # 1/(kb*T), eV
 
-        # - cubic thermo de broglie 
-        hplanck = units._hplanck # J/Hz = kg*m2*s-1
-        #_mass = np.sum([data.atomic_masses[data.atomic_numbers[e]] for e in expart]) # g/mol
-        _species = build_species(self.species)
+        # - cubic thermo de broglie
+        hplanck = units._hplanck  # J/Hz = kg*m2*s-1
+        # _mass = np.sum([data.atomic_masses[data.atomic_numbers[e]] for e in expart]) # g/mol
+        _species = convert_string_to_atoms(self.species)
         _species_mass = np.sum(_species.get_masses())
-        #print("species mass: ", _mass)
+        # print("species mass: ", _mass)
         _mass = _species_mass * units._amu
-        kbT_J = kBT_eV * units._e # J = kg*m2*s-2
-        cubic_wavelength = (hplanck/np.sqrt(2*np.pi*_mass*kbT_J)*1e10)**3 # thermal de broglie wavelength
+        kbT_J = kBT_eV * units._e  # J = kg*m2*s-2
+        cubic_wavelength = (
+            hplanck / np.sqrt(2 * np.pi * _mass * kbT_J) * 1e10
+        ) ** 3  # thermal de broglie wavelength
 
         # - compute coefficient
         # -- determine number of exchangeable particles
-        #print("miaow: ", self._curr_tags_dict)
+        # print("miaow: ", self._curr_tags_dict)
         if self.species not in self._curr_tags_dict:
             self._curr_tags_dict[self.species] = []
         nexatoms = len(self._curr_tags_dict[self.species])
 
         # -- compute composed coefficient
         if self._curr_operation == "insert":
-            coef = self._curr_volume/(nexatoms+1)/cubic_wavelength
+            coef = self._curr_volume / (nexatoms + 1) / cubic_wavelength
             ene_diff = curr_ene - self.mu - prev_ene
         elif self._curr_operation == "remove":
-            coef = nexatoms*cubic_wavelength/self._curr_volume
+            coef = nexatoms * cubic_wavelength / self._curr_volume
             ene_diff = curr_ene + self.mu - prev_ene
         else:
             raise RuntimeError(f"Unknown exchange operation {self._curr_operation}.")
 
-        acc_ratio = np.min([1.0, coef * np.exp(-beta*(ene_diff))])
+        acc_ratio = np.min([1.0, coef * np.exp(-beta * (ene_diff))])
 
-        content = "\nVolume %.4f Nexatoms %.4f CubicWave %.4f Coefficient %.4f\n" %(
-            self._curr_volume, nexatoms, cubic_wavelength, coef
+        content = "\nVolume %.4f Nexatoms %.4f CubicWave %.4f Coefficient %.4f\n" % (
+            self._curr_volume,
+            nexatoms,
+            cubic_wavelength,
+            coef,
         )
-        #content = "\nVolume %.4f Beta %.4f Coefficient %.4f\n" %(
+        # content = "\nVolume %.4f Beta %.4f Coefficient %.4f\n" %(
         #    0., beta, coef
-        #)
-        content += "Energy Difference %.4f [eV]\n" %ene_diff
-        content += "Accept Ratio %.4f\n" %acc_ratio
+        # )
+        content += "Energy Difference %.4f [eV]\n" % ene_diff
+        content += "Accept Ratio %.4f\n" % acc_ratio
         for x in content.split("\n"):
             self._print(x)
 
         rn_move = rng.uniform()
-        self._print(f"{self.__class__.__name__} Probability %.4f" %rn_move)
+        self._print(f"{self.__class__.__name__} Probability %.4f" % rn_move)
 
         # - reset stored temp data
         self._curr_operation = None
         self._curr_tags_dict = None
         self._curr_volume = None
 
         return rn_move < acc_ratio
-    
+
     def __repr__(self) -> str:
         """"""
         content = f"@Modifier {self.__class__.__name__}\n"
-        content += f"temperature {self.temperature} [K] pressure {self.pressure} [bar]\n"
+        content += (
+            f"temperature {self.temperature} [K] pressure {self.pressure} [bar]\n"
+        )
         content += "covalent ratio: \n"
         content += f"  min: {self.covalent_min} max: {self.covalent_max}\n"
         content += f"reservoir: "
         content += f"  species {self.species} with chemical potential {self.mu} [eV]\n"
         content += f"  within the region {self.region}\n"
 
         return content
 
     def as_dict(self) -> dict:
         """"""
         params = super().as_dict()
-        params["reservoir"] = dict(
-            species = self.species,
-            mu = self.mu
-        )
+        params["reservoir"] = dict(species=self.species, mu=self.mu)
         params["use_bias"] = self.use_bias
 
         return params
-    
+
 
 if __name__ == "__main__":
     ...
```

### Comparing `gdpx-0.0.5/src/gdpx/expedition/mc/operators/move.py` & `gdpx-0.0.6/src/gdpx/reactor/future/crs.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,186 +1,226 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
-from typing import List
-
 import numpy as np
+from pathlib import Path
 
 from ase import Atoms
-from ase import data, units
-from ase.neighborlist import NeighborList, natural_cutoffs
-from ase.ga.utilities import closest_distances_generator
+from ase.io import read, write
 
-from gdpx.builder.group import create_a_group
-from gdpx.builder.species import build_species
+import ase
+from ase.ga.utilities import (closest_distances_generator, atoms_too_close,
+                              atoms_too_close_two_sets)
 
-from .operator import AbstractOperator
+from ase.constraints import FixAtoms
 
+# molecular dynamics
+from ase.md.velocitydistribution import MaxwellBoltzmannDistribution
+from ase.md.langevin import Langevin
 
-class MoveOperator(AbstractOperator):
+from gdpx.computation.aseplumed import AsePlumed
 
-    name: str = "move"
 
-    def __init__(
-        self, particles: List[str]=None, region: dict={}, temperature: float=300., pressure: float=1.,
-        covalent_ratio=[0.8,2.0], max_disp: float=2.0, use_rotation: bool=True,
-        *args, **kwargs
-    ):
-        """"""
-        super().__init__(
-            region=region, temperature=temperature, pressure=pressure, 
-            covalent_ratio=covalent_ratio, use_rotation=use_rotation,
-            *args, **kwargs
-        )
+class GridReactionSampling():
 
-        self.particles = particles
+    """ steps
+        1. slice surface grid
+        2. random placement
+        3. constrained MD (harmonic potential with large spring constant)
+        4. free MD towards IS and FS
+        5. collect data and train
+    """
 
-        self.max_disp = max_disp
+    grid_length = 5.0
 
-        return
-    
-    def run(self, atoms: Atoms, rng=np.random) -> Atoms:
-        """"""
-        super().run(atoms)
-        self._extra_info = "-"
+    constrained_distance = 2.2
 
-        # BUG: If there is no species in the system...
-        species_indices = self._select_species(atoms, self.particles, rng=rng)
+    # MD parameters
+    temperature = 600 # Kelvin
+    timestep = 2.0 # fs
 
-        # - basic
-        cur_atoms = atoms.copy() # TODO: use clean atoms?
-        chemical_symbols = cur_atoms.get_chemical_symbols()
-        cell = cur_atoms.get_cell(complete=True)
-
-        # -- TODO: init blmin?
-        type_list = list(set(chemical_symbols))
-        unique_atomic_numbers = [data.atomic_numbers[a] for a in type_list]
-        self.blmin = closest_distances_generator(
-            atom_numbers=unique_atomic_numbers,
-            ratio_of_covalent_radii = self.covalent_min # be careful with test too far
-        )
+    def __init__(self, reactant, surface):
+        """"""
+        self.reactant = reactant
+        self.surface = surface
 
-        # - neighbour list
-        nl = NeighborList(
-            self.covalent_max*np.array(natural_cutoffs(cur_atoms)), 
-            skin=0.0, self_interaction=False, bothways=True
+        # generate blmin
+        # tag every molecules and state atomice types
+        #unique_atom_types = []
+        #for i, atoms in enumerate(reactants):
+        #    atoms.set_tags(i)
+        #    unique_atom_types.extend(atoms.get_atomic_numbers())
+        #unique_atom_types = list(set(unique_atom_types))
+        unique_atom_types = ["C", "O", "Cr", "Zn"]
+        unique_atom_types = [6, 8, 24, 30]
+
+        blmin = closest_distances_generator(
+            atom_numbers=unique_atom_types,
+            ratio_of_covalent_radii=0.8 # be careful with test too far
         )
+        self.blmin = blmin
 
-        # - find tag atoms
-        # record original position of species_indices
-        species = cur_atoms[species_indices]
-        self._extra_info = f"{species.get_chemical_formula()}_{species_indices}"
-
-        #org_pos = new_atoms[species_indices].position.copy() # original position
-        # TODO: deal with pbc, especially for move step
-        org_com = np.mean(species.positions, axis=0)
-        org_positions = species.positions.copy()
-
-        # - move the atom
-        for i in range(self.MAX_RANDOM_ATTEMPTS):
-            rsq = 1.1
-            while (rsq > 1.0):
-                rvec = 2*rng.uniform(size=3) - 1.0
-                rsq = np.linalg.norm(rvec)
-            ran_pos = org_com + rvec*self.max_disp
-            # -- make a copy and rotate
-            species_ = self._rotate_species(species, rng=rng)
-            curr_cop = np.average(species_.positions, axis=0)
-            # -- translate
-            new_vec = ran_pos - curr_cop
-            species_.translate(new_vec)
-            cur_atoms.positions[species_indices] = species_.positions.copy()
-            # use neighbour list
-            if not self.check_overlap_neighbour(nl, cur_atoms, cell, species_indices):
-                self._print(f"succeed to random after {i+1} attempts...")
-                self._print(f"original position: {org_com}")
-                self._print(f"random position: {ran_pos}")
-                self._print(f"actual position: {np.average(cur_atoms.positions[species_indices], axis=0)}")
-                break
-            cur_atoms.positions[species_indices] = org_positions
-        else:
-            cur_atoms = None
+        return
+    
+    def __partition_surface_grid(self):
+        # surface
+        surface = self.surface
+        positions = surface.positions
+
+        # generate grid
+        cell = self.surface.cell.complete()
+        print("cell: ", cell)
+
+        a, b, c, alpha, beta, gamma = self.surface.get_cell_lengths_and_angles()
+
+        grid_length = self.grid_length
+        na, nb = int(np.round(a/grid_length)), int(np.round(b/grid_length))
+        la, lb = a/na, b/nb
+        print("number of grids: ", na, nb)
+        print("grid size", la, lb)
+
+        # run over regions and place reactant
+        candidates = []
+        for i in range(na):
+            for j in range(nb):
+                print("region: ", i, j)
+                x1, x2 = i*la, (i+1)*la
+                y1, y2 = j*lb, (j+1)*lb
+                # find zmax in the region
+                indices = []
+                for idx, pos in enumerate(positions):
+                    if (x1 <= pos[0] < x2) and (y1 <= pos[1] < y2):
+                        indices.append(idx)
+                print("number in this region: ", len(indices))
+                zmax = np.max(positions[indices][:, 2])
+                origin = np.array([x1,y1,zmax])
+                lengths = np.array([la, lb, 2.6]) # 2.6 is distance between reactant and surface
+                print("origin: ", origin)
+
+                # add reactant
+                candidate = self.__place_random_configuration(self.constrained_distance, origin, lengths)
+                candidates.append(candidate)
+        write("cand.xyz", candidates)
 
-        return cur_atoms
+        return candidates
 
-    def check_overlap_neighbour(
-        self, nl, new_atoms, cell, species_indices: List[int]
-    ):
-        """ use neighbour list to check newly added atom is neither too close or too
-            far from other atoms
+    def __place_random_configuration(self, bond_distance, origin, lengths):
+        """ randomly place reactants in a given region
         """
-        # - get symbols here since some operators may change the symbol
-        chemical_symbols = new_atoms.get_chemical_symbols()
-
-        overlapped = False
-        nl.update(new_atoms)
-        for idx_pick in species_indices:
-            #self._print(f"- check index {idx_pick}")
-            indices, offsets = nl.get_neighbors(idx_pick)
-            if len(indices) > 0:
-                #self._print(f"nneighs: {len(indices)}")
-                # should close to other atoms
-                for ni, offset in zip(indices, offsets):
-                    dis = np.linalg.norm(new_atoms.positions[idx_pick] - (new_atoms.positions[ni] + np.dot(offset, cell)))
-                    pairs = [chemical_symbols[ni], chemical_symbols[idx_pick]]
-                    pairs = tuple([data.atomic_numbers[p] for p in pairs])
-                    #print("distance: ", ni, dis, self.blmin[pairs])
-                    if dis < self.blmin[pairs]:
-                        overlapped = True
-                        break
-            else:
-                # TODO: is no neighbours valid?
-                self._print("no neighbours, being isolated...")
-                overlapped = True
+        # place positions
+        atoms = self.reactant.copy()
+        # adjust bond distance
+        vec = atoms[0].position - atoms[1].position
+        new_pos = atoms[0].position + vec / np.linalg.norm(vec) * bond_distance
+        atoms[1].position = new_pos
+
+        # Apply a random translation
+        for i in range(100):
+            candidate = self.surface.copy()
+            ran_pos = np.random.random(3) 
+            ran_pos[2] = 1.0
+            pos = ran_pos * lengths + origin
+            com = atoms.get_center_of_mass()
+            atoms.translate(pos - com) # set to the origin
+            # Apply a random rotation to multi-atom blocks
+            phi, theta, psi = 360 * np.random.random(3)
+            atoms.euler_rotate(
+                phi=phi, theta=0.5 * theta, psi=psi,
+                center=pos
+            )
+            # add reactant
+            candidate.extend(atoms)
+            # TODO: check anchor point (C is under O)
+            # check distance
+            if not atoms_too_close(candidate, self.blmin):
+                # print(f"generate after {i+1} attempts...")
                 break
-
-        return overlapped
+        else:
+            candidate = None
+        
+        return candidate
     
-    def metropolis(self, prev_ene: float, curr_ene: float, rng=np.random) -> bool:
-        """"""
-        # - acceptance ratio
-        kBT_eV = units.kB * self.temperature
-        beta = 1./kBT_eV # 1/(kb*T), eV
-
-        coef = 1.0
-        ene_diff = curr_ene - prev_ene
-        acc_ratio = np.min([1.0, coef * np.exp(-beta*(ene_diff))])
-
-        #content = "\nVolume %.4f Nexatoms %.4f CubicWave %.4f Coefficient %.4f\n" %(
-        #    self.acc_volume, len(self.tag_list[expart]), cubic_wavelength, coef
-        #)
-        content = "\nVolume %.4f Beta %.4f Coefficient %.4f\n" %(
-            self.region.get_volume(), beta, coef
+    def __molecular_dynamics(self, atoms):
+        """ CMD
+        """
+        cons = FixAtoms(indices=[a.index for a in atoms if a.position[2] < 4.5])
+        atoms.set_constraint(cons)
+
+        MaxwellBoltzmannDistribution(atoms, temperature_K=self.temperature)
+        print("initial temperature: ", atoms.get_temperature())
+        write("xxx.xyz", atoms)
+        dyn = Langevin(
+            atoms, 
+            timestep = self.timestep*ase.units.fs, 
+            temperature_K = self.temperature, 
+            friction = 0.002, # TODO: what is the unit?
+            fixcm = True
+        )
+        plumed_worker = AsePlumed(
+            atoms, timestep=0,
+            in_file = "plumed.dat",
+            out_file = "plumed.out"
         )
-        content += "Energy Difference %.4f [eV]\n" %ene_diff
-        content += "Accept Ratio %.4f\n" %acc_ratio
-        for x in content.split("\n"):
-            self._print(x)
 
-        rn_move = rng.uniform()
-        self._print(f"{self.__class__.__name__} Probability %.4f" %rn_move)
+        md_forces = atoms.get_forces()
 
-        return rn_move < acc_ratio
+        with open("md.xyz", "w") as fopen:
+            fopen.write("")
+
+        mdsteps = 500
+        for i in range(mdsteps):
+            dyn.step(md_forces)
+
+            # bias forces
+            energy = atoms.get_potential_energy()
+            md_forces = atoms.get_forces()
+            bias_forces = plumed_worker.external_forces(
+                i, new_energy=energy, new_forces=md_forces
+            )
+            md_forces = bias_forces
+
+            write("md.xyz", atoms, append=True)
+        
+        return
     
-    def as_dict(self) -> dict:
-        """"""
-        params = super().as_dict()
-        params["particles"] = self.particles
-        params["max_disp"] = self.max_disp
+    def __call__(self, calc):
 
-        return params
+        # place MD
+        if Path("./cand.xyz").exists():
+            candidates = read("./cand.xyz", ":")
+        else:
+            candidates = self.__partition_surface_grid()
+        print("number of candidates: ", candidates)
 
-    def __repr__(self) -> str:
-        """"""
-        content = f"@Modifier {self.__class__.__name__}\n"
-        content += f"temperature {self.temperature} [K] pressure {self.pressure} [bar]\n"
-        content += "covalent ratio: \n"
-        content += f"  min: {self.covalent_min} max: {self.covalent_max}\n"
-        content += f"max disp: {self.max_disp}\n"
-        content += f"particles: \n"
-        content += f"  {self.particles}\n"
+        # run constrained MD
+        for cand in candidates[3:]:
+            calc.reset()
+            cand.calc = calc
+            self.__molecular_dynamics(cand)
 
-        return content
+            # exit()
+
+        return
 
 
 if __name__ == "__main__":
-    ...
+    reactant = read("/mnt/scratch2/users/40247882/catsign/lasp-main/reactions/CO/allstr.arc", "-1", format="dmol-arc")
+    surface = read("/mnt/scratch2/users/40247882/catsign/lasp-main/sample/ZnO-2Ov4Cr/IS/allstr.arc", "-1", format="dmol-arc")
+
+    grs = GridReactionSampling(reactant, surface)
+
+    from gdpx.computation.lasp import LaspNN
+    pot_path = "/mnt/scratch2/users/40247882/catsign/lasp-main/ZnCrOCH.pot"
+    pot = dict(
+        H  = pot_path,
+        C  = pot_path,
+        O  = pot_path,
+        Cr = pot_path,
+        Zn = pot_path
+    )
+    calc = LaspNN(
+        directory = "./LaspNN-Worker",
+        command = "mpirun -n 4 lasp",
+        pot=pot
+    )
+
+    grs(calc)
```

### Comparing `gdpx-0.0.5/src/gdpx/expedition/mc/operators/swap.py` & `gdpx-0.0.6/src/gdpx/expedition/monte_carlo/operators/swap.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,126 +5,137 @@
 from typing import List
 
 import numpy as np
 
 from ase import Atoms
 from ase import data, units
 from ase.neighborlist import NeighborList, natural_cutoffs
-from ase.ga.utilities import closest_distances_generator
 
-from gdpx.builder.species import build_species
-from gdpx.builder.group import create_a_group
 from .move import MoveOperator
 
 
 class SwapOperator(MoveOperator):
 
     name: str = "swap"
 
     def __init__(
-        self, particles: List[str], region: dict={}, temperature: float = 300, pressure: float = 1, 
-        covalent_ratio=[0.8,2.0], use_rotation: bool = True,
-        *args, **kwargs
+        self,
+        particles: List[str],
+        region: dict = {},
+        temperature: float = 300,
+        pressure: float = 1,
+        covalent_ratio=[0.8, 2.0],
+        use_rotation: bool = True,
+        *args,
+        **kwargs,
     ):
         """"""
         super().__init__(
-            particles=particles, region=region, temperature=temperature, pressure=pressure, 
-            covalent_ratio=covalent_ratio, use_rotation=use_rotation, *args, **kwargs
+            particles=particles,
+            region=region,
+            temperature=temperature,
+            pressure=pressure,
+            covalent_ratio=covalent_ratio,
+            use_rotation=use_rotation,
+            *args,
+            **kwargs,
         )
 
         # NOTE: Prohibit swapping the same type of particles.
-        assert len(set(self.particles)) == 2, f"f{self.__class__.__name__} needs two types of particles."
+        assert (
+            len(set(self.particles)) == 2
+        ), f"f{self.__class__.__name__} needs two types of particles."
 
         return
-    
+
     def run(self, atoms: Atoms, rng=np.random) -> Atoms:
         """"""
         super().run(atoms)
 
         # - basic
-        cur_atoms = atoms
-        chemical_symbols = cur_atoms.get_chemical_symbols()
-        cell = cur_atoms.get_cell(complete=True)
+        curr_atoms = atoms
+        cell = curr_atoms.get_cell(complete=True)
 
         # -- neighbour list
         nl = NeighborList(
-            self.covalent_max*np.array(natural_cutoffs(cur_atoms)), 
-            skin=0.0, self_interaction=False, bothways=True
-        )
-
-        # -- TODO: init blmin?
-        type_list = list(set(chemical_symbols))
-        unique_atomic_numbers = [data.atomic_numbers[a] for a in type_list]
-        self.blmin = closest_distances_generator(
-            atom_numbers=unique_atomic_numbers,
-            ratio_of_covalent_radii = self.covalent_min # be careful with test too far
+            self.covalent_max * np.array(natural_cutoffs(curr_atoms)),
+            skin=0.0,
+            self_interaction=False,
+            bothways=True,
         )
 
         # - swap the species
         for i in range(self.MAX_RANDOM_ATTEMPTS):
             # -- swap
-            cur_atoms = atoms.copy()
+            curr_atoms = atoms.copy()
 
             # -- pick an atom
             #   either index of an atom or tag of an moiety
-            first_pick = self._select_species(cur_atoms, [self.particles[0]], rng=rng)
-            second_pick = self._select_species(cur_atoms, [self.particles[1]], rng=rng)
+            first_pick = self._select_species(curr_atoms, [self.particles[0]], rng=rng)
+            second_pick = self._select_species(curr_atoms, [self.particles[1]], rng=rng)
             self._print(f"first: {first_pick} second: {second_pick}")
 
             # -- find tag atoms
-            first_species = cur_atoms[first_pick] # default copy
-            second_species = cur_atoms[second_pick]
+            first_species = curr_atoms[first_pick]  # default copy
+            second_species = curr_atoms[second_pick]
             # TODO: deal with pbc
             first_cop = np.average(copy.deepcopy(first_species.get_positions()), axis=0)
-            second_cop = np.average(copy.deepcopy(second_species.get_positions()), axis=0)
+            second_cop = np.average(
+                copy.deepcopy(second_species.get_positions()), axis=0
+            )
 
             self._print(f"origin: {first_species.symbols} {first_cop}")
             self._print(f"origin: {second_species.symbols} {second_cop}")
 
             # -- rotate and swap
             first_species = self._rotate_species(first_species, rng=rng)
             second_species = self._rotate_species(second_species, rng=rng)
 
-            cur_atoms.positions[first_pick] += (second_cop - first_cop)
-            cur_atoms.positions[second_pick] += (first_cop - second_cop)
+            curr_atoms.positions[first_pick] += second_cop - first_cop
+            curr_atoms.positions[second_pick] += first_cop - second_cop
 
-            first_species = cur_atoms[first_pick]
-            second_species = cur_atoms[second_pick]
+            first_species = curr_atoms[first_pick]
+            second_species = curr_atoms[second_pick]
             # TODO: deal with pbc
             first_cop = np.average(copy.deepcopy(first_species.get_positions()), axis=0)
-            second_cop = np.average(copy.deepcopy(second_species.get_positions()), axis=0)
+            second_cop = np.average(
+                copy.deepcopy(second_species.get_positions()), axis=0
+            )
 
             self._print(f"swapped: {first_species.symbols} {first_cop}")
             self._print(f"swapped: {second_species.symbols} {second_cop}")
 
             # -- use neighbour list
             idx_pick = []
             idx_pick.extend(first_pick)
             idx_pick.extend(second_pick)
-            if not self.check_overlap_neighbour(nl, cur_atoms, cell, idx_pick):
+            if not self.check_overlap_neighbour(nl, curr_atoms, cell, idx_pick):
                 self._print(f"succeed to random after {i+1} attempts...")
                 break
         else:
-            cur_atoms = None
+            curr_atoms = None
 
-        return cur_atoms
+        return curr_atoms
 
     def as_dict(self) -> dict:
         """"""
         params = super().as_dict()
+        params["particles"] = self.particles
 
         return params
 
     def __repr__(self) -> str:
         """"""
         content = f"@Modifier {self.__class__.__name__}\n"
-        content += f"temperature {self.temperature} [K] pressure {self.pressure} [bar]\n"
+        content += (
+            f"temperature {self.temperature} [K] pressure {self.pressure} [bar]\n"
+        )
         content += "covalent ratio: \n"
         content += f"  min: {self.covalent_min} max: {self.covalent_max}\n"
         content += f"swapped groups: \n"
         content += f"  {self.particles[0]} <-> {self.particles[1]}\n"
 
         return content
 
 
 if __name__ == "__main__":
-    ...
+    ...
```

### Comparing `gdpx-0.0.5/src/gdpx/graph/comparison.py` & `gdpx-0.0.6/src/gdpx/graph/comparison.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.5/src/gdpx/graph/creator.py` & `gdpx-0.0.6/src/gdpx/graph/creator.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.5/src/gdpx/graph/graph_main.py` & `gdpx-0.0.6/src/gdpx/graph/graph_main.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.5/src/gdpx/graph/molecule.py` & `gdpx-0.0.6/src/gdpx/graph/molecule.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.5/src/gdpx/graph/sites.py` & `gdpx-0.0.6/src/gdpx/graph/sites.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.5/src/gdpx/graph/surface.py` & `gdpx-0.0.6/src/gdpx/graph/surface.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.5/src/gdpx/graph/utils.py` & `gdpx-0.0.6/src/gdpx/graph/utils.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.5/src/gdpx/main.py` & `gdpx-0.0.6/src/gdpx/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,17 +71,21 @@
         description=str(registers.variable)+"\n"+str(registers.operation), 
         formatter_class=argparse.RawDescriptionHelpFormatter
     )
     parser_session.add_argument(
         "SESSION", help="session configuration file (json/yaml)"
     )
     parser_session.add_argument(
-        "-f", "--feed", default=None, nargs="+", 
+        "--feed", default=None, nargs="+", 
         help="session placeholders"
     )
+    parser_session.add_argument(
+        "--timewait", default=-1, type=float,
+        help="waiting time between repeated running"
+    )
     
     # - build structures
     parser_build = subparsers.add_parser(
         "build", help="build structures",
         description=str(registers.builder), 
         formatter_class=argparse.RawDescriptionHelpFormatter
     )
@@ -232,15 +236,15 @@
     if args.potential:
         from gdpx.worker.interface import convert_config_to_potter
         potter = convert_config_to_potter(args.potential)
 
     # - use subcommands
     if args.subcommand == "session":
         from gdpx.core.session import run_session
-        run_session(args.SESSION, args.feed, args.directory)
+        run_session(args.SESSION, args.feed, args.timewait, args.directory)
     elif args.subcommand == "convert":
         from gdpx.data import convert_dataset
         convert_dataset(args.INPUT)
     elif args.subcommand == "train":
         from gdpx.trainer import run_newtrainer
         run_newtrainer(args.CONFIG, args.directory)
     elif args.subcommand == "build":
```

### Comparing `gdpx-0.0.5/src/gdpx/nanoparticle.py` & `gdpx-0.0.6/src/gdpx/nanoparticle.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.5/src/gdpx/potential/calculators/mixer.py` & `gdpx-0.0.6/src/gdpx/potential/calculators/mixer.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.5/src/gdpx/potential/interface.py` & `gdpx-0.0.6/src/gdpx/potential/interface.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.5/src/gdpx/potential/manager.py` & `gdpx-0.0.6/src/gdpx/potential/manager.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,164 +3,154 @@
 
 import abc
 import copy
 from typing import Optional, Union, List, NoReturn
 
 import numpy as np
 
-from ase.calculators.calculator import Calculator, all_properties, all_changes
-
 from .. import config
 from ..core.register import registers
 from ..computation import register_drivers
 
 """The abstract base class of any potential manager.
 
 """
 
-class DummyCalculator(Calculator):
-
-    name = "dummy"
-
-    def __init__(self, restart=None, label="dummy", atoms=None, directory=".", **kwargs):
-        super().__init__(restart, label=label, atoms=atoms, directory=directory, **kwargs)
-
-        return
-
-    def calculate(self, atoms=None, properties=all_properties, system_changes=all_changes):
-        """"""
-        raise NotImplementedError("DummyCalculator is unable to calculate.")
-
 
 class AbstractPotentialManager(abc.ABC):
     """
     Create various potential instances
     """
 
     name = "potential"
-    version = "m00" # calculator name
+    version = "m00"  # calculator name
 
     implemented_backends = []
     valid_combinations = []
 
     _calc = None
 
     calc_backend: Optional[str] = None
 
     def __init__(self):
-        """
-        """
+        """ """
 
         return
-    
+
     @property
     def calc(self):
         return self._calc
-    
+
     @calc.setter
     def calc(self, calc_):
         self._calc = calc_
-        return 
-    
+        return
+
     @abc.abstractmethod
     def register_calculator(self, calc_params: dict, *agrs, **kwargs):
-        """Register the host calculator.
-        """
+        """Register the host calculator."""
         if self.calc_backend is None:
             self.calc_backend = calc_params.pop("backend", self.name)
         if self.calc_backend not in self.implemented_backends:
-            raise RuntimeError(f"Unknown backend {self.calc_backend} for potential {self.name}")
+            raise RuntimeError(
+                f"Unknown backend {self.calc_backend} for potential {self.name}"
+            )
 
         self.calc_params = copy.deepcopy(calc_params)
 
         return
 
-    def create_driver(
-        self, 
-        dyn_params: dict = {},
-        *args, **kwargs
-    ):
+    def create_driver(self, dyn_params: dict = {}, *args, **kwargs):
         """Create a driver for dynamics.
 
-        Default the dynamics backend will be the same as calc. However, 
+        Default the dynamics backend will be the same as calc. However,
         ase-based dynamics can be used for all calculators.
 
         """
         # - check whether there is a calc
         if not hasattr(self, "calc"):
-            raise AttributeError("Cannot create driver since a calculator has been properly registered.")
-            
+            raise AttributeError(
+                "Cannot create driver since a calculator has been properly registered."
+            )
+
         # parse backends
         self.dyn_params = dyn_params
         dynamics = dyn_params.get("backend", self.calc_backend)
         if dynamics == "external":
             dynamics = self.calc_backend
 
         if (self.calc_backend, dynamics) not in self.valid_combinations:
-            raise RuntimeError(f"Invalid dynamics backend {dynamics} based on {self.calc_backend} calculator")
-        
+            raise RuntimeError(
+                f"Invalid dynamics backend {dynamics} based on {self.calc_backend} calculator"
+            )
+
         # - merge params for compat
         merged_params = {}
         if "task" in dyn_params:
             merged_params.update(task=dyn_params.get("task", "min"))
 
         if "init" in dyn_params or "run" in dyn_params:
             merged_params.update(**dyn_params.get("init", {}))
             merged_params.update(**dyn_params.get("run", {}))
         else:
             merged_params.update(**dyn_params)
 
         # -- add params from key besides task, init, and run
         merged_params.update(
             ignore_convergence=dyn_params.get("ignore_convergence", False),
-            random_seed=dyn_params.get("random_seed", None)
+            random_seed=dyn_params.get("random_seed", None),
         )
 
         # -- other params
         ignore_convergence = merged_params.pop("ignore_convergence", False)
 
         # TODO: make PotentialManager a Node as well???
         random_seed = merged_params.pop(
             "random_seed", int(config.GRNG.integers(0, 1e8))
         )
 
         # - create dynamics
         driver_cls = register_drivers[dynamics]
-        #assert driver_cls is not None, f"Cannot find a driver named {dynamics}."
+        # assert driver_cls is not None, f"Cannot find a driver named {dynamics}."
 
         driver = driver_cls(
-            self.calc, merged_params, directory=self.calc.directory, 
-            ignore_convergence=ignore_convergence, random_seed=random_seed
+            self.calc,
+            merged_params,
+            directory=self.calc.directory,
+            ignore_convergence=ignore_convergence,
+            random_seed=random_seed,
         )
         driver.pot_params = self.as_dict()
-        
+
         return driver
 
     def create_reactor(self, rxn_params: dict = {}, *args, **kwargs):
         """Create a reactor for reaction.
 
-        Default the reaction backend will be the same as calc. However, 
+        Default the reaction backend will be the same as calc. However,
         ase-based dynamics can be used for all calculators.
 
         """
         # - check whether there is a calc
         if not hasattr(self, "calc"):
-            raise AttributeError("Cant create reactor before a calculator has been properly registered.")
-            
+            raise AttributeError(
+                "Cant create reactor before a calculator has been properly registered."
+            )
+
         # parse backends
         self.rxn_params = rxn_params
         reaction = rxn_params.get("backend", self.calc_backend)
         if reaction == "external":
             reaction = self.calc_backend
 
         if (self.calc_backend, reaction) not in self.valid_combinations:
             raise RuntimeError(
                 f"Invalid reaction backend {reaction} based on {self.calc_backend} calculator. Valid combinations are {self.valid_combinations}"
             )
-        
+
         # - merge params for compat
         merged_params = {}
         if "task" in rxn_params:
             merged_params.update(task=rxn_params.get("task", "min"))
         if "init" in rxn_params or "run" in rxn_params:
             merged_params.update(**rxn_params.get("init", {}))
             merged_params.update(**rxn_params.get("run", {}))
@@ -168,22 +158,20 @@
             merged_params.update(**rxn_params)
 
         # - other params
         ignore_convergence = merged_params.pop("ignore_convergence", False)
 
         # - construct driver params
         inp_params = dict(
-            calc = self.calc,
-            params = merged_params,
-            ignore_convergence = ignore_convergence
+            calc=self.calc, params=merged_params, ignore_convergence=ignore_convergence
         )
 
         driver = registers.create("reactor", reaction, convert_name=False, **inp_params)
         driver.pot_params = self.as_dict()
-        
+
         return driver
 
     def as_dict(self):
         """"""
         params = {}
         params["name"] = self.name
```

### Comparing `gdpx-0.0.5/src/gdpx/potential/managers/__init__.py` & `gdpx-0.0.6/src/gdpx/potential/managers/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*
 
 
 import warnings
 
 from .. import registers
-from ..manager import AbstractPotentialManager, DummyCalculator
+from ..manager import AbstractPotentialManager
 from ..trainer import AbstractTrainer
 
+from ..calculators.dummy import DummyCalculator
 from ..calculators.mixer import CommitteeCalculator
 
 
 # - basic potentials
 # -- MLIP
 from .deepmd import DeepmdManager, DeepmdTrainer, DeepmdDataloader
 registers.manager.register(DeepmdManager)
@@ -88,18 +89,17 @@
 
 try:
     from .bias import BiasManager
     registers.manager.register(BiasManager)
 except ImportError as e:
     warnings.warn("Module {} import failed: {}".format("bias", e), UserWarning)
 
-from .plumed import PlumedManager
+from .plumed.plumed import PlumedManager
 registers.manager.register(PlumedManager)
 
-
 # - trainers
 from .gp.fgp import FGPTrainer
 registers.trainer.register("FgpTrainer")(FGPTrainer)
 
 from .gp.sgp import SGPTrainer
 registers.trainer.register("SgpTrainer")(SGPTrainer)
```

### Comparing `gdpx-0.0.5/src/gdpx/potential/managers/bias.py` & `gdpx-0.0.6/src/gdpx/potential/managers/bias.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 
 import copy
 
-from gdpx.core.register import registers
-from ..manager import AbstractPotentialManager, DummyCalculator
+from . import registers
+from . import AbstractPotentialManager, DummyCalculator
 from gdpx.bias import bias_register
 
 """This manager registers ALL jax-based bias calculators."""
 
 
 class BiasManager(AbstractPotentialManager):
```

### Comparing `gdpx-0.0.5/src/gdpx/potential/managers/cp2k.py` & `gdpx-0.0.6/src/gdpx/potential/managers/cp2k.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.5/src/gdpx/potential/managers/deepmd.py` & `gdpx-0.0.6/src/gdpx/potential/managers/deepmd/deepmd.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,47 +1,218 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*
 
 import os
 import copy
-from pathlib import Path
+import dataclasses
 import pathlib
 import subprocess
-from typing import Union, List, Callable
+from typing import Optional, Union, List, Tuple, Callable
 
 import json
 
 import numpy as np
 
 from ase import Atoms
 from ase.io import read, write
 from ase.calculators.calculator import Calculator
+from ase.calculators.singlepoint import SinglePointCalculator
 
-from . import AbstractPotentialManager, AbstractTrainer
-from . import DummyCalculator, CommitteeCalculator
+from .. import AbstractPotentialManager, AbstractTrainer
+from .. import DummyCalculator, CommitteeCalculator
 
+from .convert import convert_groups
 
-class DeepmdDataloader():
+
+@dataclasses.dataclass
+class DeepmdSystem:
+
+    #: System name.
+    name: str
+
+    #: Frames.
+    frames: List[Atoms]
+
+    #: Number of train_and_split.
+    train_and_split: Tuple[int, int]
+
+    #: Batchsize
+    batchsize: int = 1
+
+    def __post_init__(
+        self,
+    ):
+        """"""
+        self.nframes = len(self.frames)
+        assert self.nframes == sum(
+            self.train_and_split
+        ), f"{self.name}: {self.nframes} != sum({self.train_and_split})"
+
+        composition_list = [a.get_chemical_formula() for a in self.frames]
+        assert len(set(composition_list)) == 1, f"{self.name}: {composition_list[0]}?"
+        self.composition = composition_list[0]
+
+        return
+
+    def write(self, directory: pathlib.Path) -> None:
+        """"""
+        directory.mkdir(parents=True, exist_ok=True)
+        write(directory / f"{self.composition}.xyz", self.frames)
+
+        return
+
+
+class DeepmdDataloader:
 
     #: Datasset name.
     name: str = "deepmd"
 
+    #:
+    _systems: List[DeepmdSystem] = []
+
     def __init__(
-        self, batchsizes, cum_batchsizes, train_sys_dirs, valid_sys_dirs, 
-        *args, **kwargs
+        self,
+        batchsizes,
+        cum_batchsizes,
+        train_sys_dirs,
+        valid_sys_dirs,
+        *args,
+        **kwargs,
     ) -> None:
         """"""
         self.batchsizes = batchsizes
         self.cum_batchsizes = cum_batchsizes
         self.train_sys_dirs = [str(x) for x in train_sys_dirs]
         self.valid_sys_dirs = [str(x) for x in valid_sys_dirs]
 
         return
-    
-    def as_dict(self, ) -> dict:
+
+    @staticmethod
+    def from_directory(
+        train_directory: Union[str, pathlib.Path],
+        valid_directory: Optional[Union[str, pathlib.Path]]=None,
+    ) -> "DeepmdDataloader":
+        """"""
+        # - read trainset...
+        train_wdir = pathlib.Path(train_directory)
+        trainset_dirs = sorted(train_wdir.iterdir())
+
+        if valid_directory is not None:
+            valid_wdir = pathlib.Path(valid_directory)
+            validset_dirs = sorted(valid_wdir.iterdir())
+        else:
+            validset_dirs = []
+
+        batchsizes = [1]*len(trainset_dirs)
+        cum_batchsizes = sum(batchsizes)
+
+        return DeepmdDataloader(batchsizes, cum_batchsizes, trainset_dirs, validset_dirs)
+
+    @property
+    def systems(
+        self,
+    ):
+        """"""
+
+        return self._systems
+
+    def load(
+        self,
+    ) -> None:
+        """"""
+        systems = []
+        for p in self.train_sys_dirs:
+            p = pathlib.Path(p)
+            print(p)
+            curr_train_frames = DeepmdDataloader.convert_system_to_frames(p)
+            num_curr_train_frames = len(curr_train_frames)
+            curr_frames = curr_train_frames
+            for p2 in self.valid_sys_dirs:
+                p2 = pathlib.Path(p2)
+                if p2.name == p.name:
+                    curr_valid_frames = DeepmdDataloader.convert_system_to_frames(p2)
+                    num_curr_valid_frames = len(curr_valid_frames)
+                    curr_frames.extend(curr_valid_frames)
+                    break
+            else:
+                num_curr_valid_frames = 0
+            curr_system = DeepmdSystem(
+                p.name, curr_frames, (num_curr_train_frames, num_curr_valid_frames)
+            )
+            systems.append(curr_system)
+        self._systems = systems
+
+        return
+
+    def dump(self, directory: Union[str, pathlib.Path]) -> None:
+        """"""
+        directory = pathlib.Path(directory)
+        for curr_system in self.systems:
+            curr_system.write(
+                directory / (curr_system.name + "-" + curr_system.composition),
+            )
+            print(
+                f"{curr_system.name =} {curr_system.composition} {curr_system.train_and_split} {curr_system.nframes}"
+            )
+
+        return
+
+    @staticmethod
+    def set2frames(
+        set_dir: pathlib.Path, chemical_symbols: List[str], pbc: List[int]
+    ) -> List[Atoms]:
+        """Convert set into frames."""
+        boxes = np.load(set_dir / "box.npy")
+        nframes = boxes.shape[0]
+        coords = np.load(set_dir / "coord.npy")
+        energies = np.load(set_dir / "energy.npy")
+        forces = np.load(set_dir / "force.npy")
+
+        if nframes == 1:
+            energies = energies.reshape(-1)
+
+        frames = []
+        for i in range(nframes):
+            cell = boxes[i, :].reshape(3, 3)
+            positions = coords[i, :].reshape(-1, 3)
+            atoms = Atoms(
+                symbols=chemical_symbols, positions=positions, cell=cell, pbc=pbc
+            )
+            results = {"energy": energies[i], "forces": forces[i, :].reshape(-1, 3)}
+            spc = SinglePointCalculator(atoms, **results)
+            atoms.calc = spc
+            frames.append(atoms)
+
+        return frames
+
+    @staticmethod
+    def convert_system_to_frames(curr_system: pathlib.Path):
+        """"""
+        # find all set dirs
+        set_dirs = sorted(curr_system.glob("set*"))
+
+        type_list = np.loadtxt(curr_system / "type_map.raw", dtype=str)
+        if len(type_list.shape) == 0:
+            type_list = type_list.reshape(-1)
+        atype = np.loadtxt(curr_system / "type.raw", dtype=int)
+        if len(atype.shape) == 0:
+            atype = atype.reshape(-1)
+        chemical_symbols = [type_list[a] for a in atype]
+        pbc = [1, 1, 1] if not (curr_system / "nopbc").exists() else [0, 0, 0]
+
+        # train data
+        frames = []
+        for set_dir in set_dirs[:]:
+            frames.extend(DeepmdDataloader.set2frames(set_dir, chemical_symbols, pbc))
+
+        return frames
+
+    def as_dict(
+        self,
+    ) -> dict:
         """"""
         params = {}
         params["name"] = self.name
         params["batchsizes"] = self.batchsizes
         params["cum_batchsizes"] = self.cum_batchsizes
         params["train_sys_dirs"] = self.train_sys_dirs
         params["valid_sys_dirs"] = self.valid_sys_dirs
@@ -56,25 +227,38 @@
     freeze_command = "dp"
     prefix = "config"
 
     #: Flag indicates that the training is finished properly.
     CONVERGENCE_FLAG: str = "finished training"
 
     def __init__(
-        self, config: dict, type_list: List[str]=None, train_epochs: int=200,
+        self,
+        config: dict,
+        type_list: List[str] = None,
+        train_epochs: int = 200,
         print_epochs: int = 5,
-        directory=".", command="dp", freeze_command="dp", random_seed=1112, 
-        *args, **kwargs
+        directory=".",
+        command="dp",
+        freeze_command="dp",
+        random_seed=1112,
+        *args,
+        **kwargs,
     ) -> None:
         """"""
         super().__init__(
-            config=config, type_list=type_list, train_epochs=train_epochs,
+            config=config,
+            type_list=type_list,
+            train_epochs=train_epochs,
             print_epochs=print_epochs,
-            directory=directory, command=command, freeze_command=freeze_command, 
-            random_seed=random_seed, *args, **kwargs
+            directory=directory,
+            command=command,
+            freeze_command=freeze_command,
+            random_seed=random_seed,
+            *args,
+            **kwargs,
         )
 
         # - TODO: sync type_list
         if type_list is None:
             self._type_list = config["model"]["type_map"]
         else:
             self._type_list = type_list
@@ -121,208 +305,131 @@
 
         return command
 
     @property
     def frozen_name(self):
         """"""
         return f"{self.name}.pb"
-    
+
     def _train_from_the_restart(self, dataset, init_model):
         """Train from the restart"""
         if not self.directory.exists():
             command = self._train_from_the_scratch(dataset, init_model)
         else:
-            ckpt_info = self.directory/"checkpoint"
+            ckpt_info = self.directory / "checkpoint"
             if ckpt_info.exists() and ckpt_info.stat().st_size != 0:
                 # TODO: check if the ckpt model exists?
                 command = f"{self.command} train {self.name}.json "
                 command += f"--restart model.ckpt"
                 self._print(f"TRAINING COMMAND: {command}")
-            else: # assume not at any ckpt so start from the scratch
+            else:  # assume not at any ckpt so start from the scratch
                 command = self._train_from_the_scratch(dataset, init_model)
 
         return command
 
-    def _prepare_dataset(self, dataset, reduce_system: bool=False, *args, **kwargs):
+    def _prepare_dataset(self, dataset, *args, **kwargs):
         """"""
         if not self.directory.exists():
             self.directory.mkdir(parents=True, exist_ok=True)
         if not isinstance(dataset, DeepmdDataloader):
-            set_names, train_frames, test_frames, adjusted_batchsizes = self._get_dataset(
-                dataset, reduce_system
+            set_names, train_frames, test_frames, adjusted_batchsizes = (
+                dataset.split_train_and_test()
             )
-
             train_dir = self.directory
 
             # - update config
             self._print("--- write dp train data---")
             batchsizes = adjusted_batchsizes
             cum_batchsizes, train_sys_dirs = convert_groups(
-                set_names, train_frames, batchsizes, 
+                set_names,
+                train_frames,
+                batchsizes,
                 self.config["model"]["type_map"],
-                "train", train_dir, self._print
+                "train",
+                train_dir,
+                self._print,
             )
             _, valid_sys_dirs = convert_groups(
-                set_names, test_frames, batchsizes,
-                self.config["model"]["type_map"], 
-                "valid", train_dir, self._print
+                set_names,
+                test_frames,
+                batchsizes,
+                self.config["model"]["type_map"],
+                "valid",
+                train_dir,
+                self._print,
             )
             self._print(f"accumulated number of batches: {cum_batchsizes}")
 
             dataset = DeepmdDataloader(
                 batchsizes, cum_batchsizes, train_sys_dirs, valid_sys_dirs
             )
         else:
             ...
 
         return dataset
 
-    def write_input(self, dataset, reduce_system: bool=False):
-        """Write inputs for training.
-
-        Args:
-            reduce_system: Whether merge structures.
-
-        """
+    def write_input(self, dataset):
+        """Write inputs for training."""
         # - prepare dataset (convert dataset to DeepmdDataloader)
-        dataset = self._prepare_dataset(dataset, reduce_system)
+        dataset = self._prepare_dataset(dataset)
 
         # - check train config
         # NOTE: parameters
         #       numb_steps, seed
         #       descriptor-seed, fitting_net-seed
         #       training - training_data, validation_data
         train_config = copy.deepcopy(self.config)
 
-        train_config["model"]["descriptor"]["seed"] =  self.rng.integers(0,10000, dtype=int)
-        train_config["model"]["fitting_net"]["seed"] = self.rng.integers(0,10000, dtype=int)
+        train_config["model"]["descriptor"]["seed"] = self.rng.integers(
+            0, 10000, dtype=int
+        )
+        train_config["model"]["fitting_net"]["seed"] = self.rng.integers(
+            0, 10000, dtype=int
+        )
 
-        train_config["training"]["training_data"]["systems"] = [x for x in dataset.train_sys_dirs]
+        train_config["training"]["training_data"]["systems"] = [
+            x for x in dataset.train_sys_dirs
+        ]
         train_config["training"]["training_data"]["batch_size"] = dataset.batchsizes
 
-        train_config["training"]["validation_data"]["systems"] = [x for x in dataset.valid_sys_dirs]
+        train_config["training"]["validation_data"]["systems"] = [
+            x for x in dataset.valid_sys_dirs
+        ]
         train_config["training"]["validation_data"]["batch_size"] = dataset.batchsizes
 
-        train_config["training"]["seed"] = self.rng.integers(0,10000, dtype=int)
+        train_config["training"]["seed"] = self.rng.integers(0, 10000, dtype=int)
 
         # --- calc numb_steps
-        min_freq_unit = 100.
-        save_freq = int(np.ceil(dataset.cum_batchsizes*self.print_epochs/min_freq_unit)*min_freq_unit)
+        min_freq_unit = 100.0
+        save_freq = int(
+            np.ceil(dataset.cum_batchsizes * self.print_epochs / min_freq_unit)
+            * min_freq_unit
+        )
         train_config["training"]["save_freq"] = save_freq
 
-        numb_steps = dataset.cum_batchsizes*self.train_epochs
-        n_checkpoints = int(np.ceil(dataset.cum_batchsizes*self.train_epochs/save_freq))
-        numb_steps = n_checkpoints*save_freq
+        numb_steps = dataset.cum_batchsizes * self.train_epochs
+        n_checkpoints = int(
+            np.ceil(dataset.cum_batchsizes * self.train_epochs / save_freq)
+        )
+        numb_steps = n_checkpoints * save_freq
         train_config["training"]["numb_steps"] = numb_steps
 
         # - write
-        with open(self.directory/f"{self.name}.json", "w") as fopen:
+        with open(self.directory / f"{self.name}.json", "w") as fopen:
             json.dump(train_config, fopen, indent=2)
 
         return
 
-    def _get_dataset(self, dataset, reduce_system):
-        """"""
-        data_dirs = dataset.load()
-        self._print("--- auto data reader ---")
-        self._debug(data_dirs)
-
-        batchsizes = dataset.batchsize
-        nsystems = len(data_dirs)
-        if isinstance(batchsizes, int):
-            batchsizes = [batchsizes]*nsystems
-        assert len(batchsizes) == nsystems, "Number of systems and batchsizes are inconsistent."
-
-        # read configurations
-        set_names = []
-        train_size, test_size = [], []
-        train_frames, test_frames = [], []
-        adjusted_batchsizes = [] # auto-adjust batchsize based on nframes
-        for i, (curr_system, curr_batchsize) in enumerate(zip(data_dirs, batchsizes)):
-            curr_system = pathlib.Path(curr_system)
-            set_name = "+".join(str(curr_system.relative_to(dataset.directory)).split("/"))
-            set_names.append(set_name)
-            self._print(f"System {set_name} Batchsize {curr_batchsize}")
-            frames = [] # all frames in this subsystem
-            subsystems = list(curr_system.glob("*.xyz"))
-            subsystems.sort() # sort by alphabet
-            for p in subsystems:
-                # read and split dataset
-                p_frames = read(p, ":")
-                p_nframes = len(p_frames)
-                frames.extend(p_frames)
-                self._print(f"  subsystem: {p.name} number {p_nframes}")
-
-            # split dataset and get adjusted batchsize
-            # TODO: adjust batchsize of train and test separately
-            nframes = len(frames)
-            if nframes <= curr_batchsize:
-                if nframes == 1 or curr_batchsize == 1:
-                    new_batchsize = 1
-                else:
-                    new_batchsize = int(2**np.floor(np.log2(nframes)))
-                adjusted_batchsizes.append(new_batchsize)
-                # NOTE: use same train and test set
-                #       since they are very important structures...
-                train_index = list(range(nframes))
-                test_index = list(range(nframes))
-            else:
-                if nframes == 1 or curr_batchsize == 1:
-                    new_batchsize = 1
-                    train_index = list(range(nframes))
-                    test_index = list(range(nframes))
-                else:
-                    new_batchsize = curr_batchsize
-                    # - assure there is at least one batch for test
-                    #          and number of train frames is integer times of batchsize
-                    ntrain = int(np.floor(nframes * dataset.train_ratio / new_batchsize) * new_batchsize)
-                    train_index = self.rng.choice(nframes, ntrain, replace=False)
-                    test_index = [x for x in range(nframes) if x not in train_index]
-                adjusted_batchsizes.append(new_batchsize)
-
-            ntrain, ntest = len(train_index), len(test_index)
-            train_size.append(ntrain)
-            test_size.append(ntest)
-
-            self._print(f"    ntrain: {ntrain} ntest: {ntest} ntotal: {nframes} batchsize: {new_batchsize}")
-
-            curr_train_frames = [frames[train_i] for train_i in train_index]
-            curr_test_frames = [frames[test_i] for test_i in test_index]
-            if reduce_system:
-                # train
-                train_frames.extend(curr_train_frames)
-                n_train_frames = len(train_frames)
-
-                # test
-                test_frames.extend(curr_test_frames)
-                n_test_frames = len(test_frames)
-            else:
-                # train
-                train_frames.append(curr_train_frames)
-                n_train_frames = sum([len(x) for x in train_frames])
-
-                # test
-                test_frames.append(curr_test_frames)
-                n_test_frames = sum([len(x) for x in test_frames])
-            self._print(f"  Current Dataset -> ntrain: {n_train_frames} ntest: {n_test_frames}")
-
-        assert len(train_size) == len(test_size), "inconsistent train_size and test_size"
-        train_size = sum(train_size)
-        test_size = sum(test_size)
-        self._print(f"Total Dataset -> ntrain: {train_size} ntest: {test_size}")
-
-        return set_names, train_frames, test_frames, adjusted_batchsizes
-
     def freeze(self):
         """"""
         # - freeze model
         frozen_model = super().freeze()
 
         # - compress model
-        compressed_model = (self.directory/f"{self.name}-c.pb").absolute()
+        compressed_model = (self.directory / f"{self.name}-c.pb").absolute()
         if frozen_model.exists() and not compressed_model.exists():
             command = self._resolve_compress_command()
             try:
                 proc = subprocess.Popen(command, shell=True, cwd=self.directory)
             except OSError as err:
                 msg = "Failed to execute `{}`".format(command)
                 # raise RuntimeError(msg) from err
@@ -330,33 +437,36 @@
                 self._print("Failed to compress model.")
             except RuntimeError as err:
                 self._print("Failed to compress model.")
 
             errorcode = proc.wait()
             if errorcode:
                 path = os.path.abspath(self.directory)
-                msg = ('Trainer "{}" failed with command "{}" failed in '
-                       '{} with error code {}'.format(self.name, command,
-                                                      path, errorcode))
+                msg = (
+                    'Trainer "{}" failed with command "{}" failed in '
+                    "{} with error code {}".format(self.name, command, path, errorcode)
+                )
                 # NOTE: sometimes dp cannot compress the model
                 #       this happens when the descriptor trainable is set False?
                 # raise RuntimeError(msg)
                 # self._print(msg)
-                compressed_model.symlink_to(frozen_model.relative_to(compressed_model.parent))
+                compressed_model.symlink_to(
+                    frozen_model.relative_to(compressed_model.parent)
+                )
         else:
             ...
 
         return compressed_model
 
     def read_convergence(self) -> bool:
         """Read training convergence.
 
         Check deepmd training progress by comparing the `numb_steps` in the input
         configuration and the current step in `lcurve.out`.
-        
+
         """
         self._print(f"check {self.name} training convergence...")
         converged = False
 
         dpconfig_path = self.directory / f"{self.name}.json"
         if dpconfig_path.exists():
             # - get numb_steps
@@ -380,157 +490,81 @@
                 ...
         else:
             ...
 
         return converged
 
 
-def convert_groups(
-    names: List[str], groups: List[List[Atoms]], batchsizes: Union[List[int],int],
-    type_map: List[str], suffix, dest_dir="./", pfunc=print
-):
-    """"""
-    nsystems = len(groups)
-    if isinstance(batchsizes, int):
-        batchsizes = [batchsizes]*nsystems
-
-    from gdpx.computation.utils import get_formula_from_atoms
-
-    # --- dpdata conversion
-    import dpdata
-    dest_dir = pathlib.Path(dest_dir)
-    train_set_dir = dest_dir/f"{suffix}"
-    if not train_set_dir.exists():
-        train_set_dir.mkdir()
-
-    sys_dirs = []
-        
-    cum_batchsizes = 0 # number of batchsizes for training
-    for name, frames, batchsize in zip(names, groups, batchsizes):
-        nframes = len(frames)
-        nbatch = int(np.ceil(nframes / batchsize))
-        pfunc(f"{suffix} system {name} nframes {nframes} nbatch {nbatch} batchsize {batchsize}")
-        # --- check composition consistent
-        compositions = [get_formula_from_atoms(a) for a in frames]
-        assert len(set(compositions)) == 1, f"Inconsistent composition {len(set(compositions))} =? 1..."
-        curr_composition = compositions[0]
-
-        cum_batchsizes += nbatch
-        # --- NOTE: need convert forces to force
-        frames_ = copy.deepcopy(frames) 
-        # check pbc
-        pbc = np.all([np.all(a.get_pbc()) for a in frames_])
-        for atoms in frames_:
-            try:
-                forces = atoms.get_forces().copy()
-                del atoms.arrays["forces"]
-                atoms.arrays["force"] = forces
-                keys = copy.deepcopy(list(atoms.arrays.keys()))
-                for k in keys:
-                    if k not in ["numbers", "positions", "force"]:
-                        del atoms.arrays[k]
-                #if "tags" in atoms.arrays:
-                #    del atoms.arrays["tags"]
-                #if "momenta" in atoms.arrays:
-                #    del atoms.arrays["momenta"]
-                #if "initial_charges" in atoms.arrays:
-                #    del atoms.arrays["initial_charges"]
-            except:
-                pass
-            finally:
-                atoms.calc = None
-
-        # --- convert data
-        write(train_set_dir/f"{name}-{suffix}.xyz", frames_)
-        dsys = dpdata.MultiSystems.from_file(
-            train_set_dir/f"{name}-{suffix}.xyz", fmt="quip/gap/xyz", 
-            type_map = type_map
-        )
-        # NOTE: this function create dir with composition and overwrite files
-        #       so we need separate dirs...
-        sys_dir = train_set_dir/name
-        if sys_dir.exists():
-            raise FileExistsError(f"{sys_dir} exists. Please check the dataset.")
-        else:
-            dsys.to_deepmd_npy(train_set_dir/"_temp") # prec, set_size
-            (train_set_dir/"_temp"/curr_composition).rename(sys_dir)
-            if not pbc:
-                with open(sys_dir/"nopbc", "w") as fopen:
-                    fopen.write("nopbc\n")
-        sys_dirs.append(sys_dir)
-    (train_set_dir/"_temp").rmdir()
-
-    return cum_batchsizes, sys_dirs
-
-
 class DeepmdManager(AbstractPotentialManager):
 
     name = "deepmd"
 
     implemented_backends = ["ase", "lammps"]
 
     valid_combinations = (
         # calculator, dynamics
         ("ase", "ase"),
         ("lammps", "ase"),
-        ("lammps", "lammps")
+        ("lammps", "lammps"),
     )
 
     #: Used for estimating uncertainty.
     _estimator = None
 
     def __init__(self, *args, **kwargs):
         """"""
 
         return
-    
+
     def _create_calculator(self, calc_params: dict) -> Calculator:
         """Create an ase calculator.
 
         Todo:
             In fact, uncertainty estimation has various backends as well.
-        
+
         """
         calc_params = copy.deepcopy(calc_params)
 
         # - some shared params
         command = calc_params.pop("command", None)
-        directory = calc_params.pop("directory", Path.cwd())
+        directory = calc_params.pop("directory", pathlib.Path.cwd())
 
         type_list = calc_params.pop("type_list", [])
         type_map = {}
         for i, a in enumerate(type_list):
             type_map[a] = i
-        
+
         # --- model files
         model_ = calc_params.get("model", [])
         if not isinstance(model_, list):
             model_ = [model_]
 
         models = []
         for m in model_:
-            m = Path(m).resolve()
+            m = pathlib.Path(m).resolve()
             if not m.exists():
                 raise FileNotFoundError(f"Cant find model file {str(m)}")
             models.append(str(m))
+        self.calc_params.update(model=models)
 
         # TODO: make this a dataclass??
         #       currently, default disable uncertainty estimation
         estimate_uncertainty = calc_params.get("estimate_uncertainty", False)
 
         # - create specific calculator
         calc = DummyCalculator()
         if self.calc_backend == "ase":
             # return ase calculator
             try:
-                #from deepmd.calculator import DP
-                from gdpx.computation.dpx import DP
+                from .calculator import DP
             except:
-                raise ModuleNotFoundError("Please install deepmd-kit to use the ase interface.")
-            #if models and type_map:
+                raise ModuleNotFoundError(
+                    "Please install deepmd-kit to use the ase interface."
+                )
+            # if models and type_map:
             #    calc = DP(model=models[0], type_dict=type_map)
             calcs = []
             for m in models:
                 curr_calc = DP(model=m, type_dict=type_map)
                 calcs.append(curr_calc)
             if len(calcs) == 1:
                 calc = calcs[0]
@@ -539,101 +573,116 @@
                     calc = CommitteeCalculator(calcs=calcs)
                 else:
                     calc = calcs[0]
             else:
                 ...
         elif self.calc_backend == "lammps":
             from gdpx.computation.lammps import Lammps
+
             if models:
                 if len(models) == 1:
                     pair_style = "deepmd {}".format(" ".join(models))
                 else:
                     if estimate_uncertainty:
                         pair_style = "deepmd {}".format(" ".join(models))
                     else:
                         pair_style = "deepmd {}".format(models[0])
                 pair_coeff = calc_params.pop("pair_coeff", "* *")
 
                 pair_style_name = pair_style.split()[0]
-                assert pair_style_name == "deepmd", "Incorrect pair_style for lammps deepmd..."
+                assert (
+                    pair_style_name == "deepmd"
+                ), "Incorrect pair_style for lammps deepmd..."
 
                 calc = Lammps(
-                    command=command, directory=directory, 
-                    pair_style=pair_style, pair_coeff=pair_coeff,
-                    **calc_params
+                    command=command,
+                    directory=directory,
+                    pair_style=pair_style,
+                    pair_coeff=pair_coeff,
+                    **calc_params,
                 )
                 # - update several params
                 calc.units = "metal"
                 calc.atom_style = "atomic"
 
         return calc
 
     def register_calculator(self, calc_params, *args, **kwargs) -> None:
-        """ generate calculator with various backends
-        """
+        """generate calculator with various backends"""
         super().register_calculator(calc_params)
-        
+
         self.calc = self._create_calculator(self.calc_params)
 
         return
-    
-    def switch_backend(self, backend: str=None) -> None:
+
+    def switch_backend(self, backend: str = None) -> None:
         """Switch the potential's calculation backend."""
         if backend is None:
             return
 
         if not hasattr(self, "calc"):
-            raise RuntimeError(f"{self.name} cannot switch backend as it does not have a calculator attached.")
+            raise RuntimeError(
+                f"{self.name} cannot switch backend as it does not have a calculator attached."
+            )
         if backend not in self.implemented_backends:
-            raise RuntimeError(f"{self.name} cannot switch backend from {self.calc_backend} to {backend}.")
-        
+            raise RuntimeError(
+                f"{self.name} cannot switch backend from {self.calc_backend} to {backend}."
+            )
+
         prev_backend = self.calc_backend
         if prev_backend == "ase" and backend == "lammps":
             calc_params = copy.deepcopy(self.calc_params)
             calc_params["backend"] = "lammps"
             command = calc_params.get("command", None)
             if command is None:
-                raise RuntimeError(f"{self.name} cannot switch backend from ase to lammps as no command is provided.")
+                raise RuntimeError(
+                    f"{self.name} cannot switch backend from ase to lammps as no command is provided."
+                )
+            else:
+                self.calc_backend = None
             self.register_calculator(calc_params)
         elif prev_backend == "lammps" and backend == "ase":
             calc_params = copy.deepcopy(self.calc_params)
             calc_params["backend"] = "ase"
+            self.calc_backend = None
             self.register_calculator(calc_params)
-        else: # Nothing to do for other combinations
+        else:  # Nothing to do for other combinations
             ...
 
         return
-    
-    def switch_uncertainty_estimation(self, status: bool=True):
+
+    def switch_uncertainty_estimation(self, status: bool = True):
         """Switch on/off the uncertainty estimation."""
         # NOTE: Sometimes the manager loads several models and supports uncertainty
-        #       by committee but the user disables it. We need change the calc to 
+        #       by committee but the user disables it. We need change the calc to
         #       the correct one as the loaded one is just a single calculator.
         if not hasattr(self, "calc"):
-            raise RuntimeError("Fail to switch uncertainty status as it does not have a calc.")
-        #print(f"{self.calc}")
+            raise RuntimeError(
+                "Fail to switch uncertainty status as it does not have a calc."
+            )
+        # print(f"{self.calc}")
 
         # NOTE: make sure manager.as_dict() can have correct param
         self.calc_params["estimate_uncertainty"] = status
 
         # - convert calculator
         if self.calc_backend == "ase":
             if status:
                 if isinstance(self.calc, CommitteeCalculator):
-                    ... # nothing to do
-                else: # reload models
+                    ...  # nothing to do
+                else:  # reload models
                     self.calc = self._create_calculator(self.calc_params)
             else:
                 if isinstance(self.calc, CommitteeCalculator):
                     # TODO: save previous calc?
                     self.calc = self.calc.calcs[0]
                 else:
                     ...
         elif self.calc_backend == "lammps":
-            models = self.calc.pair_style.split()[1:] # model paths
+            models = self.calc.pair_style.split()[1:]  # model paths
             nmodels = len(models)
             if status:
                 if nmodels > 1:
                     ...
                 else:
                     self.calc = self._create_calculator(self.calc_params)
             else:
@@ -644,18 +693,18 @@
                 else:
                     ...
         else:
             # TODO:
             # Other backends cannot have uncertainty estimation,
             # give a warning?
             ...
-        #print(f"{self.calc}")
+        # print(f"{self.calc}")
 
         return
-    
+
     def remove_loaded_models(self, *args, **kwargs):
         """Loaded TF models should be removed before any copy.deepcopy operations."""
         self.calc.reset()
         if self.calc_backend == "ase":
             if isinstance(self.calc, CommitteeCalculator):
                 for c in self.calc.calcs:
                     c.dp = None
```

### Comparing `gdpx-0.0.5/src/gdpx/potential/managers/dftd3.py` & `gdpx-0.0.6/src/gdpx/potential/managers/dftd3.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*
 
 
-from ..manager import AbstractPotentialManager, DummyCalculator
+from . import AbstractPotentialManager, DummyCalculator
 
 
 """Check https://dftd3.readthedocs.io/en/latest/api/ase.html
 
 To install, use conda install dftd3-python -c conda-forge.
 
 Calculator parameters should have `method` (xc e.g. PBE) and `damping` (e.g. d3bj).
```

### Comparing `gdpx-0.0.5/src/gdpx/potential/managers/eam.py` & `gdpx-0.0.6/src/gdpx/potential/managers/eam.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.5/src/gdpx/potential/managers/emt.py` & `gdpx-0.0.6/src/gdpx/potential/managers/emt.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.5/src/gdpx/potential/managers/espresso.py` & `gdpx-0.0.6/src/gdpx/potential/managers/espresso.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.5/src/gdpx/potential/managers/gp/bench.py` & `gdpx-0.0.6/src/gdpx/potential/managers/gp/bench.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.5/src/gdpx/potential/managers/gp/fgp.py` & `gdpx-0.0.6/src/gdpx/potential/managers/gp/fgp.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.5/src/gdpx/potential/managers/gp/gptools.py` & `gdpx-0.0.6/src/gdpx/potential/managers/gp/gptools.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.5/src/gdpx/potential/managers/gp/representation.py` & `gdpx-0.0.6/src/gdpx/potential/managers/gp/representation.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.5/src/gdpx/potential/managers/gp/sgp.py` & `gdpx-0.0.6/src/gdpx/potential/managers/gp/sgp.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.5/src/gdpx/potential/managers/grid.py` & `gdpx-0.0.6/src/gdpx/potential/managers/grid.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.5/src/gdpx/potential/managers/lasp.py` & `gdpx-0.0.6/src/gdpx/potential/managers/lasp.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.5/src/gdpx/potential/managers/mace.py` & `gdpx-0.0.6/src/gdpx/potential/managers/mace.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     name: str = "mace"
 
     def __init__(
         self,
         train_file: Union[str, pathlib.Path],
         test_file: Union[str, pathlib.Path],
         batchsize: int,
-        directory: Union[str, pathlib.Path]="./",
+        directory: Union[str, pathlib.Path] = "./",
         *args,
         **kwargs,
     ) -> None:
         """"""
         self.train_file = pathlib.Path(train_file).resolve()
         self.test_file = pathlib.Path(test_file).resolve()
 
@@ -89,15 +89,15 @@
             *args,
             **kwargs,
         )
 
         self._type_list = type_list
 
         return
-    
+
     def _resolve_train_command(self, init_model=None, *args, **kwargs) -> str:
         """"""
 
         return self.command
 
     def freeze(self):
         """"""
@@ -141,15 +141,17 @@
         train_config["eval_interval"] = self.print_epochs
         train_config["batch_size"] = dataset.batchsize
 
         swa = train_config.get("swa", False)
         if swa:
             start_swa = train_config.get("start_swa", -1)
             if not (0 < start_swa < self.train_epochs):
-                raise RuntimeError(f"{start_swa = } must be smaller than {self.train_epochs = }")
+                raise RuntimeError(
+                    f"{start_swa = } must be smaller than {self.train_epochs = }"
+                )
         else:
             ...
 
         # - misc
         import torch
 
         train_config["device"] = "cuda" if torch.cuda.is_available() else "cpu"
@@ -164,39 +166,44 @@
         train_config.pop("checkpoints_dir", None)
         train_config.pop("results_dir", None)
 
         return train_config
 
     def _train_from_the_restart(self, dataset, init_model) -> str:
         """Train from the restart"""
+        if init_model is not None:
+            raise NotImplementedError(
+                f"{self.name} does not support initialising from a previous model."
+            )
+
         def _add_command_options(command, config) -> str:
             """"""
             # - convert to command line options...
             command = command + " "
             for k, v in config.items():
                 if isinstance(v, bool):
                     if v:
                         command += f"--{k}  "
                 elif isinstance(v, int) or isinstance(v, float):
                     command += f"--{k}={str(v)}  "
                 else:
                     command += f"--{k}='{str(v)}'  "
 
             return command
-        
+
         train_config = self._update_config(dataset)
 
         if not self.directory.exists():
             command = self._train_from_the_scratch(dataset, init_model)
             if init_model is not None:
                 ...
             command = _add_command_options(command, train_config)
         else:
             command = self._train_from_the_scratch(dataset, init_model)
-            ckpt_dir = self.directory/"checkpoints"
+            ckpt_dir = self.directory / "checkpoints"
             if ckpt_dir.exists():
                 model_name = train_config["name"]
                 ckpts = [p for p in ckpt_dir.glob(f"{model_name}*")]
                 self._print(ckpts)
                 ckpt_models = [c for c in ckpts if c.name.endswith(".model")]
                 if len(ckpt_models) > 0:
                     ckpt_model = ckpt_models[0]
@@ -307,17 +314,20 @@
 
         models = []
         for m in model_:
             m = pathlib.Path(m).resolve()
             if not m.exists():
                 raise FileNotFoundError(f"Cant find model file {str(m)}")
             models.append(str(m))
+        self.calc_params.update(model=models)
 
         precision = calc_params.pop("precision", "float32")
 
+        estimate_uncertainty = calc_params.get("estimate_uncertainty", False)
+
         # - create specific calculator
         calc = DummyCalculator()
         if self.calc_backend == "ase":
             # return ase calculator
             try:
                 import torch
                 from mace.calculators import MACECalculator
@@ -333,15 +343,18 @@
                     device="cuda" if torch.cuda.is_available() else "cpu",
                     default_dtype=precision,
                 )
                 calcs.append(curr_calc)
             if len(calcs) == 1:
                 calc = calcs[0]
             elif len(calcs) > 1:
-                calc = CommitteeCalculator(calcs)
+                if estimate_uncertainty:
+                    calc = CommitteeCalculator(calcs)
+                else:
+                    calc = calcs[0]
             else:
                 ...
         elif self.calc_backend == "lammps":
             raise RuntimeError("The LAMMPS backend for MACE is under development.")
         else:
             ...
```

### Comparing `gdpx-0.0.5/src/gdpx/potential/managers/mixer.py` & `gdpx-0.0.6/src/gdpx/potential/managers/mixer.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.5/src/gdpx/potential/managers/nequip.py` & `gdpx-0.0.6/src/gdpx/potential/managers/nequip.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.5/src/gdpx/potential/managers/plumed.py` & `gdpx-0.0.6/src/gdpx/potential/managers/plumed/plumed.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr3/bin/env python3
 # -*- coding: utf-8 -*
 
 
 import pathlib
 
-from . import AbstractPotentialManager, DummyCalculator
+from .. import AbstractPotentialManager, DummyCalculator
 
 
 class PlumedManager(AbstractPotentialManager):
 
     name = "plumed"
 
     implemented_backends = ["ase"]
@@ -18,52 +18,63 @@
         ("ase", "ase"),
     )
 
     def __init__(self) -> None:
         """"""
 
         return
-    
+
     def register_calculator(self, calc_params: dict, *agrs, **kwargs) -> None:
         """"""
         super().register_calculator(calc_params, *agrs, **kwargs)
 
         calc = DummyCalculator()
         if self.calc_backend == "ase":
             try:
-                from gdpx.computation.plumed import Plumed
+                from .calculators.plumed2 import Plumed
             except:
-                raise ModuleNotFoundError("Please install py-plumed to use the ase interface.")
-
-            inp = pathlib.Path(calc_params.get("inp", "./plumed.inp"))
-            if inp.exists():
-                self.calc_params.update(inp=str(inp.absolute()))
+                raise ModuleNotFoundError(
+                    "Please install py-plumed to use the ase interface."
+                )
+
+            inp = calc_params.get("inp", "./plumed.inp")
+            if isinstance(inp, str) or isinstance(inp, pathlib.Path):
+                inp = pathlib.Path(inp)
+                if inp.exists():
+                    input_lines = []
+                    with open(inp, "r") as fopen:
+                        lines = fopen.readlines()
+                        for line in lines:
+                            line = line.strip()
+                            if line and not line.startswith("#"):
+                                if "#" in line:
+                                    line = line[: line.index("#")]
+                                else:
+                                    line = line
+                                input_lines.append(line + "\n")
+                    self.calc_params.update(inp=input_lines)
+                else:
+                    raise FileNotFoundError(f"{inp} does not exist.")
+            elif isinstance(inp, list):
+                input_lines = inp
             else:
-                raise FileNotFoundError(f"{inp} does not exist.")
+                raise ValueError(f"Plumed input {inp} {type(inp)} is invalid.")
 
-            input_lines = []
-            with open(inp, "r") as fopen:
-                lines = fopen.readlines()
-                for line in lines:
-                    line = line.strip()
-                    if line and not line.startswith("#"):
-                        if "#" in line:
-                            line = line[:line.index("#")]
-                        else:
-                            line = line
-                        input_lines.append(line+"\n")
-            #print(f"input_lines: {input_lines}")
-                
-            kT = calc_params.get("kT", 1.)
+            kT = calc_params.get("kT", 1.0)
             use_charge = calc_params.get("use_charge", False)
             update_charge = calc_params.get("update_charge", False)
-            calc = Plumed(input=input_lines, kT=kT, use_charge=use_charge, update_charge=update_charge)
+            calc = Plumed(
+                input=input_lines,
+                kT=kT,
+                use_charge=use_charge,
+                update_charge=update_charge,
+            )
         else:
             ...
-        
+
         self.calc = calc
 
         return
 
 
 if __name__ == "__main__":
     ...
```

### Comparing `gdpx-0.0.5/src/gdpx/potential/managers/reann/beann.py` & `gdpx-0.0.6/src/gdpx/potential/managers/reann/beann.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.5/src/gdpx/potential/managers/reann/calculators/reann.py` & `gdpx-0.0.6/src/gdpx/potential/managers/reann/calculators/reann.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.5/src/gdpx/potential/managers/reann/reann.py` & `gdpx-0.0.6/src/gdpx/potential/managers/reann/reann.py`

 * *Files 2% similar despite different names*

```diff
@@ -451,14 +451,15 @@
 
         models = []
         for m in model_:
             m = pathlib.Path(m).resolve()
             if not m.exists():
                 raise FileNotFoundError(f"Cant find model file {str(m)}")
             models.append(str(m))
+        self.calc_params.update(model=models)
 
         precision = calc_params.pop("precision", "float32")
         assert precision in ["float32", "float64"]
 
         # TODO: make this a dataclass??
         #       currently, default disable uncertainty estimation
         estimate_uncertainty = calc_params.get("estimate_uncertainty", False)
```

### Comparing `gdpx-0.0.5/src/gdpx/potential/managers/reax.py` & `gdpx-0.0.6/src/gdpx/potential/managers/reax.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.5/src/gdpx/potential/managers/schnet.py` & `gdpx-0.0.6/src/gdpx/potential/managers/schnet.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.5/src/gdpx/potential/managers/vasp.py` & `gdpx-0.0.6/src/gdpx/potential/managers/vasp.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.5/src/gdpx/potential/managers/xtb.py` & `gdpx-0.0.6/src/gdpx/potential/managers/xtb.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.5/src/gdpx/potential/trainer.py` & `gdpx-0.0.6/src/gdpx/potential/trainer.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,15 +116,15 @@
         if command is None:
             raise TrainingFailed(
                 f"Please supply the command keyword for {self.name.upper()}."
             )
 
         if not self.directory.exists():
             self.directory.mkdir(parents=True, exist_ok=True)
-        self.write_input(dataset, reduce_system=False)
+        self.write_input(dataset)
 
         return command
 
     def train(self, dataset, init_model=None, *args, **kwargs):
         """"""
         if not hasattr(self, "_train_from_the_restart"):
             command = self._train_from_the_scratch(dataset, init_model)
```

### Comparing `gdpx-0.0.5/src/gdpx/reactor/__init__.py` & `gdpx-0.0.6/src/gdpx/reactor/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,14 +5,17 @@
 
 from .. import config
 from ..core.register import registers
 
 from ..builder.constraints import parse_constraint_info
 from ..potential.calculators.mixer import EnhancedCalculator
 
+from ..utils.strucopy import read_sort, resort_atoms_with_spc
+from ..utils.cmdrun import run_ase_calculator
+
 
 """ This submodule is for exploring, sampling, 
     and performing (chemical) reactions with
     various advanced algorithms.
 """
 
 # - string methods...
@@ -23,8 +26,8 @@
 registers.reactor.register("ase")(AseStringReactor)
 registers.reactor.register("cp2k")(Cp2kStringReactor)
 registers.reactor.register("vasp")(VaspStringReactor)
 registers.reactor.register("grid")(ZeroStringReactor)
 
 
 if __name__ == "__main__":
-    ...
+    ...
```

### Comparing `gdpx-0.0.5/src/gdpx/reactor/future/AccCons.py` & `gdpx-0.0.6/src/gdpx/reactor/future/AccCons.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.5/src/gdpx/reactor/future/AccHop.py` & `gdpx-0.0.6/src/gdpx/reactor/future/AccHop.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.5/src/gdpx/reactor/future/AccNEB.py` & `gdpx-0.0.6/src/gdpx/reactor/future/AccNEB.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.5/src/gdpx/reactor/future/cmp_mep.py` & `gdpx-0.0.6/src/gdpx/reactor/future/cmp_mep.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.5/src/gdpx/reactor/future/constrain.py` & `gdpx-0.0.6/src/gdpx/reactor/future/constrain.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.5/src/gdpx/reactor/future/crs.py` & `gdpx-0.0.6/src/gdpx/validator/melting_point.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,226 +1,249 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
+import pathlib
+from typing import NoReturn, List, Union
+
 import numpy as np
-from pathlib import Path
+import scipy as sp
+from scipy.optimize import curve_fit
+from scipy.spatial import distance_matrix
+
+from joblib import Parallel, delayed
 
 from ase import Atoms
 from ase.io import read, write
 
-import ase
-from ase.ga.utilities import (closest_distances_generator, atoms_too_close,
-                              atoms_too_close_two_sets)
+import matplotlib as mpl
+mpl.use("Agg") #silent mode
+from matplotlib import pyplot as plt
+try:
+    plt.style.use("presentation")
+except Exception as e:
+    #print("Used default matplotlib style.")
+    ...
+
+from ..utils.command import CustomTimer
+from .validator import AbstractValidator
+from .utils import wrap_traj
+from ..data.array import AtomsNDArray
+from ..builder.group import create_a_group
+
+"""Measure melting point.
+
+"""
+
+def jpcc2020_func(T, Tm, x1, x2, x3, x4):
+    """JPCC2020"""
+
+    return x1/(1+np.exp(-x2*(T-Tm)))+x3*T+x4
+
+def sigmoid_func(T, Tm, x1, x2, x4):
+    """"""
+
+    return x1/(1+np.exp(-x2*(T-Tm)))+x4
+
+def get_distance_matrix(atoms: Atoms, indices=None):
+    """"""
+    if indices is None:
+        return atoms.get_all_distances(mic=False,vector=False)
+    else:
+        selected_positions = atoms.positions[indices, :]
+        return distance_matrix(selected_positions, selected_positions)
+
+def _icalc_local_lindemann_index(frames, group, n_jobs=1):
+    """Calculate Lindemann Index of each atom.
 
-from ase.constraints import FixAtoms
+    Returns:
+        An array with shape (natoms,)
 
-# molecular dynamics
-from ase.md.velocitydistribution import MaxwellBoltzmannDistribution
-from ase.md.langevin import Langevin
+    """
+    # NOTE: Use unwrapped positions when under PBC?
+    frames = wrap_traj(frames) # align structures
+
+    group_indices = create_a_group(frames[0], group)
+    natoms = len(group_indices)
 
-from gdpx.computation.aseplumed import AsePlumed
+    with CustomTimer("Lindemann Index"):
+        distances = Parallel(n_jobs=n_jobs)(
+            delayed(get_distance_matrix)(atoms, group_indices) 
+            for atoms in frames
+        )
+    distances = np.array(distances)
 
+    dis2 = np.square(distances)
+    dis2_avg = np.average(dis2, axis=0)
 
-class GridReactionSampling():
+    dis_avg = np.average(distances, axis=0)
+    masked_dis_avg = dis_avg + np.eye(natoms) # avoid 0. in denominator
+    #print(masked_dis_avg)
+
+    q = np.sum( np.sqrt(dis2_avg - dis_avg**2) / masked_dis_avg, axis=1) / (natoms-1)
+
+    return q
+
+
+class MeltingPointValidator(AbstractValidator):
+
+    """Estimate the melting point from a series of MD simulations.
+    
+    For nanoparticles, the lindeman index is used. MD simulations with various 
+    initial temperatures are performed. For bulk, phase co-existence approach is used.
+    Different initial temperatures are set for solid and liquid, where the steady state is
+    found.
 
-    """ steps
-        1. slice surface grid
-        2. random placement
-        3. constrained MD (harmonic potential with large spring constant)
-        4. free MD towards IS and FS
-        5. collect data and train
     """
 
-    grid_length = 5.0
+    def __init__(self, group, run_fit: bool=True, start=0, temperatures: List[float]=None, fitting="sigmoid", directory: Union[str, pathlib.Path] = "./", *args, **kwargs):
+        """"""
+        super().__init__(directory, *args, **kwargs)
+
+        self.group = group
 
-    constrained_distance = 2.2
+        self.run_fit = run_fit
 
-    # MD parameters
-    temperature = 600 # Kelvin
-    timestep = 2.0 # fs
+        self.start = start
+
+        if temperatures is None:
+            temperatures = []
+        self.temperatures = temperatures
+        
+        assert fitting in ["sigmoid", "jpcc2020"], "Unsupported fitting function."
+        self.fitting = fitting
 
-    def __init__(self, reactant, surface):
+        return
+    
+    def _process_data(self, data) -> List[List[Atoms]]:
         """"""
-        self.reactant = reactant
-        self.surface = surface
+        data = AtomsNDArray(data)
 
-        # generate blmin
-        # tag every molecules and state atomice types
-        #unique_atom_types = []
-        #for i, atoms in enumerate(reactants):
-        #    atoms.set_tags(i)
-        #    unique_atom_types.extend(atoms.get_atomic_numbers())
-        #unique_atom_types = list(set(unique_atom_types))
-        unique_atom_types = ["C", "O", "Cr", "Zn"]
-        unique_atom_types = [6, 8, 24, 30]
-
-        blmin = closest_distances_generator(
-            atom_numbers=unique_atom_types,
-            ratio_of_covalent_radii=0.8 # be careful with test too far
-        )
-        self.blmin = blmin
+        if data.ndim == 1:
+            data = [data.tolist()]
+        elif data.ndim == 2: # assume it is from extract_cache...
+            data = data.tolist()
+        elif data.ndim == 3: # assume it is from a compute node...
+            data_ = []
+            for d in data[:]: # TODO: add squeeze method?
+                data_.extend(d)
+            data = data_
+        else:
+            raise RuntimeError(f"Invalid shape {data.shape}.")
+
+        return data
+
+    def run(self, dataset: dict, worker=None, *args, **kwargs):
+        """"""
+        super().run()
+
+        self._print("process reference ->")
+        reference = dataset.get("reference")
+        if reference is not None:
+            reference = self._process_data(reference)
+            data = self._compute_melting_point(reference, prefix="ref-")
+            self._plot_figure(data[:, 1], data[:, 0], prefix="ref-", run_fit=self.run_fit)
+
+        self._print("process prediction ->")
+        prediction = dataset.get("prediction")
+        if prediction is not None:
+            prediction = self._process_data(prediction)
+            data = self._compute_melting_point(prediction, prefix="pre-")
+            self._plot_figure(data[:, 1], data[:, 0], prefix="pre-", run_fit=self.run_fit)
 
         return
     
-    def __partition_surface_grid(self):
-        # surface
-        surface = self.surface
-        positions = surface.positions
-
-        # generate grid
-        cell = self.surface.cell.complete()
-        print("cell: ", cell)
-
-        a, b, c, alpha, beta, gamma = self.surface.get_cell_lengths_and_angles()
-
-        grid_length = self.grid_length
-        na, nb = int(np.round(a/grid_length)), int(np.round(b/grid_length))
-        la, lb = a/na, b/nb
-        print("number of grids: ", na, nb)
-        print("grid size", la, lb)
-
-        # run over regions and place reactant
-        candidates = []
-        for i in range(na):
-            for j in range(nb):
-                print("region: ", i, j)
-                x1, x2 = i*la, (i+1)*la
-                y1, y2 = j*lb, (j+1)*lb
-                # find zmax in the region
-                indices = []
-                for idx, pos in enumerate(positions):
-                    if (x1 <= pos[0] < x2) and (y1 <= pos[1] < y2):
-                        indices.append(idx)
-                print("number in this region: ", len(indices))
-                zmax = np.max(positions[indices][:, 2])
-                origin = np.array([x1,y1,zmax])
-                lengths = np.array([la, lb, 2.6]) # 2.6 is distance between reactant and surface
-                print("origin: ", origin)
-
-                # add reactant
-                candidate = self.__place_random_configuration(self.constrained_distance, origin, lengths)
-                candidates.append(candidate)
-        write("cand.xyz", candidates)
-
-        return candidates
-
-    def __place_random_configuration(self, bond_distance, origin, lengths):
-        """ randomly place reactants in a given region
-        """
-        # place positions
-        atoms = self.reactant.copy()
-        # adjust bond distance
-        vec = atoms[0].position - atoms[1].position
-        new_pos = atoms[0].position + vec / np.linalg.norm(vec) * bond_distance
-        atoms[1].position = new_pos
-
-        # Apply a random translation
-        for i in range(100):
-            candidate = self.surface.copy()
-            ran_pos = np.random.random(3) 
-            ran_pos[2] = 1.0
-            pos = ran_pos * lengths + origin
-            com = atoms.get_center_of_mass()
-            atoms.translate(pos - com) # set to the origin
-            # Apply a random rotation to multi-atom blocks
-            phi, theta, psi = 360 * np.random.random(3)
-            atoms.euler_rotate(
-                phi=phi, theta=0.5 * theta, psi=psi,
-                center=pos
+    def _compute_melting_point(self, trajectories, prefix=""):
+        """"""
+        start, intv, end = self.start, None, None
+        temperatures = self.temperatures
+        assert len(trajectories) == len(temperatures), "Inconsitent number of trajectories and temperatures."
+
+        qnames = [str(t) for t in temperatures]
+
+        cached_data_path = self.directory / f"{prefix}qmat.txt"
+        if not cached_data_path.exists():
+            self._debug(f"nprocessors: {self.njobs}")
+            with CustomTimer("joblib", func=self._print):
+                qmat = Parallel(n_jobs=1)(
+                    delayed(_icalc_local_lindemann_index)(
+                        [a for a in curr_frames[start::] if a is not None], 
+                        self.group, n_jobs=self.njobs
+                    ) for curr_frames in trajectories
+                )
+            qmat = np.array(qmat)
+
+            np.savetxt(
+                cached_data_path, qmat.T,
+                header=(
+                    "{:>11s}"+"{:>12s}"*(len(qnames)-1)
+                ).format(*qnames),
+                fmt="%12.4f"
             )
-            # add reactant
-            candidate.extend(atoms)
-            # TODO: check anchor point (C is under O)
-            # check distance
-            if not atoms_too_close(candidate, self.blmin):
-                # print(f"generate after {i+1} attempts...")
-                break
         else:
-            candidate = None
+            qmat = np.loadtxt(cached_data_path).T
         
-        return candidate
-    
-    def __molecular_dynamics(self, atoms):
-        """ CMD
-        """
-        cons = FixAtoms(indices=[a.index for a in atoms if a.position[2] < 4.5])
-        atoms.set_constraint(cons)
-
-        MaxwellBoltzmannDistribution(atoms, temperature_K=self.temperature)
-        print("initial temperature: ", atoms.get_temperature())
-        write("xxx.xyz", atoms)
-        dyn = Langevin(
-            atoms, 
-            timestep = self.timestep*ase.units.fs, 
-            temperature_K = self.temperature, 
-            friction = 0.002, # TODO: what is the unit?
-            fixcm = True
-        )
-        plumed_worker = AsePlumed(
-            atoms, timestep=0,
-            in_file = "plumed.dat",
-            out_file = "plumed.out"
+        # - postprocess data
+        t = temperatures
+        q = np.average(qmat, axis=1)
+
+        sorted_indices = [
+            x[0] for x in sorted(enumerate(temperatures), key=lambda x: x[1])
+        ]
+        self._debug(sorted_indices)
+
+        data = np.vstack(
+            (
+                [t[i] for i in sorted_indices],
+                [q[i] for i in sorted_indices]
+            )
+        ).T
+
+        np.savetxt(
+            self.directory/f"{prefix}data.txt", data,
+            header="{:>11s}  {:>12s}".format("temperature", "<q>"),
+            fmt="%12.4f"
         )
 
-        md_forces = atoms.get_forces()
+        return data
 
-        with open("md.xyz", "w") as fopen:
-            fopen.write("")
+    def _plot_figure(self, q, t: List[float], prefix="", run_fit=True):
+        """"""
+        fig, ax = plt.subplots(nrows=1, ncols=1, figsize=(12,8))
 
-        mdsteps = 500
-        for i in range(mdsteps):
-            dyn.step(md_forces)
-
-            # bias forces
-            energy = atoms.get_potential_energy()
-            md_forces = atoms.get_forces()
-            bias_forces = plumed_worker.external_forces(
-                i, new_energy=energy, new_forces=md_forces
-            )
-            md_forces = bias_forces
+        # - text
+        fig.suptitle("Lindemann Index")
 
-            write("md.xyz", atoms, append=True)
-        
-        return
-    
-    def __call__(self, calc):
+        ax.set_xlabel("Temperature [K]")
+        ax.set_ylabel("$<q(T)>$")
 
-        # place MD
-        if Path("./cand.xyz").exists():
-            candidates = read("./cand.xyz", ":")
-        else:
-            candidates = self.__partition_surface_grid()
-        print("number of candidates: ", candidates)
+        # - 
+        ax.scatter(t, q)
+
+        # - fitted curve
+        if run_fit:
+            if self.fitting == "sigmoid":
+                func = sigmoid_func
+                initial_guess = [np.median(t), np.max(q), 1., np.min(q)]
+            elif self.fitting == "jpcc2020":
+                func = jpcc2020_func
+                initial_guess = [np.median(t), np.max(q), 1., 0., np.min(q)]
+            coefs, cov = curve_fit(func, t, q, initial_guess, method="dogbox")
+            self._debug(coefs)
+
+            t_ = np.arange(np.min(t), np.max(t), 2.)
+            q_ = func(t_, *coefs)
+            ax.plot(t_, q_, label=f"$T_m={coefs[0]:>8.2f}$")
 
-        # run constrained MD
-        for cand in candidates[3:]:
-            calc.reset()
-            cand.calc = calc
-            self.__molecular_dynamics(cand)
+            ax.legend(loc="upper left")
 
-            # exit()
+        plt.savefig(self.directory/f"{prefix}mp.png")
 
         return
+    
+    def _compare_results(self):
+        """Compare reference and prediction."""
 
+        return
 
-if __name__ == "__main__":
-    reactant = read("/mnt/scratch2/users/40247882/catsign/lasp-main/reactions/CO/allstr.arc", "-1", format="dmol-arc")
-    surface = read("/mnt/scratch2/users/40247882/catsign/lasp-main/sample/ZnO-2Ov4Cr/IS/allstr.arc", "-1", format="dmol-arc")
-
-    grs = GridReactionSampling(reactant, surface)
-
-    from gdpx.computation.lasp import LaspNN
-    pot_path = "/mnt/scratch2/users/40247882/catsign/lasp-main/ZnCrOCH.pot"
-    pot = dict(
-        H  = pot_path,
-        C  = pot_path,
-        O  = pot_path,
-        Cr = pot_path,
-        Zn = pot_path
-    )
-    calc = LaspNN(
-        directory = "./LaspNN-Worker",
-        command = "mpirun -n 4 lasp",
-        pot=pot
-    )
 
-    grs(calc)
+if __name__ == "__main__":
+    ...
```

### Comparing `gdpx-0.0.5/src/gdpx/reactor/future/diffusion3.py` & `gdpx-0.0.6/src/gdpx/reactor/future/diffusion3.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.5/src/gdpx/reactor/future/find_adsorption.py` & `gdpx-0.0.6/src/gdpx/reactor/future/find_adsorption.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.5/src/gdpx/reactor/future/find_inter.py` & `gdpx-0.0.6/src/gdpx/reactor/future/find_inter.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.5/src/gdpx/reactor/future/muller-brown.py` & `gdpx-0.0.6/src/gdpx/reactor/future/muller-brown.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.5/src/gdpx/reactor/future/test_mh.py` & `gdpx-0.0.6/src/gdpx/reactor/future/test_mh.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.5/src/gdpx/reactor/interface.py` & `gdpx-0.0.6/src/gdpx/reactor/interface.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.5/src/gdpx/reactor/reactor.py` & `gdpx-0.0.6/src/gdpx/reactor/reactor.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.5/src/gdpx/reactor/string/cp2k.py` & `gdpx-0.0.6/src/gdpx/reactor/string/cp2k.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.5/src/gdpx/reactor/string/grid.py` & `gdpx-0.0.6/src/gdpx/reactor/string/grid.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.5/src/gdpx/reactor/string/pathway.py` & `gdpx-0.0.6/src/gdpx/reactor/string/vasp.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,254 +1,287 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
-import copy
+
 import dataclasses
+import os
+import re
 import pathlib
-from typing import Callable, List
+import traceback
+
+from typing import Union, List
 
 import numpy as np
 
 from ase import Atoms
 from ase.io import read, write
-from ase.geometry import find_mic
-from ase.constraints import Filter, FixAtoms
-from ase.neb import NEB, NEBTools
 from ase.calculators.singlepoint import SinglePointCalculator
+from ase.calculators.vasp import Vasp
 
-
-from .. import config as GDPCONFIG
-from .. import EnhancedCalculator
-from .. import parse_constraint_info
+from .. import read_sort, resort_atoms_with_spc, run_ase_calculator
 from .string import AbstractStringReactor, StringReactorSetting
 
-def set_constraint(atoms, cons_text):
-    """"""
-    atoms._del_constraints()
-    mobile_indices, frozen_indices = parse_constraint_info(
-        atoms, cons_text, ignore_ase_constraints=True, ret_text=False
-    )
-    if frozen_indices:
-        atoms.set_constraint(FixAtoms(indices=frozen_indices))
-
-    return atoms
-
-def print_step(neb, pfunc):
-    """"""
-    content = "{} {}"
 
-    return
+#: Ase-vasp sort fname.
+ASE_VASP_SORT_FNAME: str = "ase-sort.dat"
 
-def save_nebtraj(neb, log_fpath) -> None:
-    """Create a clean atoms from the input and save simulation trajectory.
 
-    We need an explicit copy of atoms as some calculators may not return all 
-    necessary information. For example, schnet only returns required properties.
-    If only energy is required, there are no forces.
-
-    """
-    def _convert_atoms(atoms):
-        # - save atoms
-        atoms_to_save = Atoms(
-            symbols=atoms.get_chemical_symbols(),
-            positions=atoms.get_positions().copy(),
-            cell=atoms.get_cell().copy(),
-            pbc=copy.deepcopy(atoms.get_pbc())
-        )
-        if "tags" in atoms.arrays:
-            atoms_to_save.set_tags(atoms.get_tags())
-        if atoms.get_kinetic_energy() > 0.:
-            atoms_to_save.set_momenta(atoms.get_momenta())
-        results = dict(
-            energy = atoms.get_potential_energy(),
-            forces = copy.deepcopy(atoms.get_forces())
-        )
-        spc = SinglePointCalculator(atoms, **results)
-        atoms_to_save.calc = spc
+def read_vaspout(
+    lines: List[str],
+) -> int:
+    """"""
+    pattern = re.compile("[0-9]+ F=")
 
-        # - save special keys and arrays from calc
-        natoms = len(atoms)
-        # -- add deviation
-        for k, v in atoms.calc.results.items():
-            if k in GDPCONFIG.VALID_DEVI_FRAME_KEYS:
-                atoms_to_save.info[k] = v
-        for k, v in atoms.calc.results.items():
-            if k in GDPCONFIG.VALID_DEVI_ATOMIC_KEYS:
-                atoms_to_save.arrays[k] = np.reshape(v, (natoms, -1))
-
-        # -- check special metadata
-        calc = atoms.calc
-        if isinstance(calc, EnhancedCalculator):
-            atoms_to_save.info["host_energy"] = copy.deepcopy(calc.results["host_energy"])
-            atoms_to_save.arrays["host_forces"] = copy.deepcopy(calc.results["host_forces"])
-
-        return atoms_to_save
-    
-    # - append to traj
-    for atoms in neb.iterimages():
-        atoms_to_save = _convert_atoms(atoms)
-        write(log_fpath, atoms_to_save, append=True)
+    steps = [0]
+    for line in lines:
+        m = pattern.match(line.strip())
+        if m:
+            step = int(m.group().split()[0])
+            steps.append(step)
+        else:
+            ...
+    # print(f"{steps =}")
 
-    return
+    return max(steps)
 
 
 @dataclasses.dataclass
-class AseStringReactorSetting(StringReactorSetting):
+class VaspStringReactorSetting(StringReactorSetting):
+
+    backend: str = "vasp"
 
-    backend: str = "ase"
+    #: Number of tasks/processors/cpus for each image.
+    ntasks_per_image: int = 1
 
     def __post_init__(self):
         """"""
-        # - ...
-        opt_cls = None
-        if self.optimiser == "bfgs": # Takes a lot of time to solve hessian.
-            from ase.optimize import BFGS as opt_cls
-        elif self.optimiser == "fire": # BUG: STRANGE BEHAVIOUR.
-            from ase.optimize import FIRE as opt_cls
-        elif self.optimiser == "mdmin":
-            from ase.optimize import MDMin as opt_cls
-        else:
-            ...
-        
-        self.opt_cls = opt_cls
+        self._internals.update(
+            # ---
+            ibrion=3,
+            potim=0,
+            isif=2,
+            # ---
+            lclimb=self.climb,
+            ichain=0,
+            images=self.nimages - 2,
+            iopt=1,
+            spring=-5,
+        )
 
         return
 
     def get_run_params(self, *args, **kwargs):
         """"""
+        # - convergence criteria
+        fmax_ = kwargs.get("fmax", self.fmax)
         steps_ = kwargs.get("steps", self.steps)
-        if steps_ <= 0:
-            steps_ = -1
+
         run_params = dict(
-            steps = steps_,
-            fmax = self.fmax
+            constraint=kwargs.get("constraint", self.constraint),
+            ediffg=fmax_ * -1.0,
+            nsw=steps_,
         )
 
         return run_params
 
 
-class AseStringReactor(AbstractStringReactor):
-
-    """Find the minimum energy path based on input structures.
+class VaspStringReactor(AbstractStringReactor):
 
-    Methods based on the number of input structures such as single, double, multi...
+    name: str = "vasp"
 
-    """
+    traj_name: str = "01/OUTCAR"
 
-    name = "ase"
-
-    traj_name: str = "nebtraj.xyz"
-
-    def __init__(self, calc=None, params={}, ignore_convergence=False, directory="./", *args, **kwargs) -> None:
+    def __init__(
+        self,
+        calc: Vasp = None,
+        params: dict = {},
+        ignore_convergence: bool = False,
+        directory: Union[str, pathlib.Path] = "./",
+        *args,
+        **kwargs,
+    ) -> None:
         """"""
         self.calc = calc
         if self.calc is not None:
             self.calc.reset()
 
         self.ignore_convergence = ignore_convergence
 
         self.directory = directory
-        self.cache_nebtraj = self.directory/self.traj_name
 
         # - parse params
-        self.setting = AseStringReactorSetting(**params)
+        self.setting = VaspStringReactorSetting(**params)
         self._debug(self.setting)
 
         return
-    
-    @AbstractStringReactor.directory.setter
-    def directory(self, directory_):
-        self._directory = pathlib.Path(directory_)
-        self.calc.directory = str(self.directory) # NOTE: avoid inconsistent in ASE
 
-        self.cache_nebtraj = self.directory/self.traj_name
+    def _verify_checkpoint(self):
+        """Check if the current directory has any valid outputs or it just created
+        the input files.
 
-        return
-    
-    def _verify_checkpoint(self, *args, **kwargs) -> bool:
-        """"""
-        verified = super()._verify_checkpoint(*args, **kwargs)
+        """
+        verified = super()._verify_checkpoint()
         if verified:
-            if self.cache_nebtraj.exists() and self.cache_nebtraj.stat().st_size != 0:
-                verified = True
+            vasprun = self.directory / "01" / "OUTCAR"
+            if vasprun.exists() and vasprun.stat().st_size != 0:
+                temp_frames = read(vasprun, ":")
+                try:
+                    _ = temp_frames[0].get_forces()
+                except:
+                    verified = False
             else:
                 verified = False
         else:
-            ...
+            verified = False
 
         return verified
-    
+
     def _irun(self, structures: List[Atoms], ckpt_wdir=None, *args, **kwargs):
         """"""
         try:
-            run_params = self.setting.get_run_params()
-
-            if ckpt_wdir is None: # start from the scratch
-                images = self._align_structures(structures)
-                write(self.directory/"images.xyz", images)
+            # --
+            run_params = self.setting.get_run_params(**kwargs)
+            run_params.update(**self.setting.get_init_params())
+
+            if ckpt_wdir is None:  # start from the scratch
+                images = self._align_structures(structures, run_params)
+                write(self.directory / "images.xyz", images)
             else:
-                nebtraj = self.read_trajectory()
-                images = nebtraj[-1]
-                run_params["steps"] = run_params["steps"] - (len(nebtraj)-1)
-
-            for a in images:
-                set_constraint(a, self.setting.constraint)
-                a.calc = self.calc
-
-            neb = NEB(
-                images=images, k=self.setting.k, climb=self.setting.climb,
-                remove_rotation_and_translation=False, method="aseneb",
-                allow_shared_calculator=True, precon=None,
-            )
-            #neb.interpolate(apply_constraint=True)
+                # - update structures
+                rep_dirs = sorted(
+                    [x.name for x in sorted(self.directory.glob(r"[0-9][0-9]"))]
+                )
 
-            driver = self.setting.opt_cls(neb, logfile="-", trajectory=None)
-            driver.attach(
-                save_nebtraj, interval=1,
-                neb=neb, log_fpath=self.cache_nebtraj
-            )
+                frames_ = []
+                for x in rep_dirs[1:-1]:
+                    frames_.append(read(self.directory / x / "OUTCAR", ":"))
+                nframes = min([len(x) for x in frames_])
+                assert nframes > 0, "At least one step finished before resume..."
+                intermediates_ = [x[nframes - 1] for x in frames_]
+                images = [structures[0]] + intermediates_ + [structures[-1]]
+
+                run_params.update(steps=self.setting.steps - nframes)
+
+            # - update input
+            self.calc.set(**run_params)
+
+            atoms = images[0]
+            atoms.calc = self.calc
+
+            # -- write input files
+            self.calc.write_input(atoms)
+            if (self.directory / "POSCAR").exists():
+                os.remove(self.directory / "POSCAR")
+
+            # -- add replica information
+            for i, a in enumerate(images):
+                rep_dir = self.directory / str(i).zfill(2)
+                # It has already been created when images are written.
+                # If the previous run has no outputs, we just overwrite everything.
+                rep_dir.mkdir(exist_ok=True)
+                write(
+                    rep_dir / "POSCAR",
+                    a[self.calc.sort],
+                    symbol_count=self.calc.symbol_count,
+                )
+
+            # - run calculation
+            run_ase_calculator("vasp", atoms.calc.command, self.directory)
 
-            driver.run(steps=run_params["steps"], fmax=run_params["fmax"])
         except Exception as e:
             self._debug(e)
+            self._debug(traceback.print_exc())
 
         return
-    
+
+    def read_convergence(self, *args, **kwargs):
+        """Check whether vasp-neb is converged.
+
+        The convergence meets when either the required force is reached or
+        the maximum steps exceed.
+
+        """
+        converged = super().read_convergence(*args, **kwargs)
+
+        self._print(f"{self.directory =}")
+        vaspout_fpath = self.directory / "vasp.out"
+        if vaspout_fpath.exists():
+            with open(self.directory / "vasp.out", "r") as fopen:
+                lines = fopen.readlines()
+
+            steps = read_vaspout(lines)
+            if steps >= self.setting.steps:
+                converged = True
+
+            for line in lines:
+                if "reached required accuracy" in line:
+                    converged = True
+                    break
+        else:
+            ...
+
+        return converged
+
     def _read_a_single_trajectory(self, wdir, *args, **kwargs):
-        """"""
-        cache_nebtraj = wdir/self.traj_name
-        nimages_per_band = self.setting.nimages
-        if cache_nebtraj.exists():
-            images = read(cache_nebtraj, ":")
+        """
+
+        NOTE: Fixed atoms have zero forces.
+
+        """
+        self._debug(f"***** read_trajectory *****")
+        self._debug(f"{str(wdir)}")
+
+        images = read(wdir / "images.xyz", ":")
+        ini_atoms, fin_atoms = images[0], images[-1]
+
+        # TODO: energy and forces of IS and FS?
+        calc = SinglePointCalculator(
+            ini_atoms,
+            energy=ini_atoms.info["energy"],
+            forces=np.zeros((len(ini_atoms), 3)),
+        )
+        ini_atoms.calc = calc
+        calc = SinglePointCalculator(
+            fin_atoms,
+            energy=fin_atoms.info["energy"],
+            forces=np.zeros((len(fin_atoms), 3)),
+        )
+        fin_atoms.calc = calc
+
+        # - read OUTCARs
+        if (self.directory / ASE_VASP_SORT_FNAME).exists():
+            sort, resort = read_sort(self.directory, ASE_VASP_SORT_FNAME)
         else:
-            raise FileNotFoundError(f"No cache trajectory {str(cache_nebtraj)}.")
-        
-        nimages = len(images)
-        assert nimages%nimages_per_band == 0, "Inconsistent number of bands."
-        nbands = int(nimages/nimages_per_band)
-
-        reshaped_images = []
-        for i in range(nbands):
-            reshaped_images.append(images[i*nimages_per_band:(i+1)*nimages_per_band])
-
-        return reshaped_images
-    
-    def read_convergence(self, *args, **kwargs) -> bool:
-        """"""
-        converged = False
-        if self.cache_nebtraj.exists():
-            nimages_per_band = self.setting.nimages
-            images = self.read_trajectory()
-            nsteps = len(images)
-            nt = NEBTools(images[-1])
-            fmax = nt.get_fmax()
-            if (fmax <= self.setting.fmax) or (nsteps >= self.setting.steps+1):
-                converged = True
-                self._print(
-                    f"STEP: {nsteps} >= {self.setting.steps} MAXFRC: {fmax} <=? {self.setting.fmax}"
+            natoms = len(ini_atoms)
+            sort, resort = list(range(natoms)), list(range(natoms))
+
+        frames_ = []
+        for i in range(1, self.setting.nimages - 1):
+            curr_frames = read(wdir / f"{str(i).zfill(2)}" / "OUTCAR", ":")
+            sorted_frames = []
+            for a in curr_frames:
+                sorted_atoms = resort_atoms_with_spc(
+                    a, resort, "vasp", print_func=self._print, debug_func=self._debug
                 )
+                sorted_frames.append(sorted_atoms)
+            frames_.append(sorted_frames)
 
-        return converged
+        # nframes may not consistent across replicas
+        # due to unfinished calculations
+        nframes_list = [len(x) for x in frames_]
+        nsteps = min(nframes_list)
+
+        frames = []
+        for i in range(nsteps):
+            curr_frames = (
+                [ini_atoms]
+                + [frames_[j][i] for j in range(self.setting.nimages - 2)]
+                + [fin_atoms]
+            )
+            frames.append(curr_frames)
+
+        return frames
 
 
 if __name__ == "__main__":
     ...
+
```

### Comparing `gdpx-0.0.5/src/gdpx/reactor/string/string.py` & `gdpx-0.0.6/src/gdpx/reactor/string/string.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,56 +5,47 @@
 import abc
 import copy
 import dataclasses
 import itertools
 import pathlib
 import re
 import shutil
-from typing import List
+from typing import Optional, Union, List
 
 import numpy as np
 
 from ase import Atoms
 from ase.io import read, write
 from ase.geometry import find_mic
 from ase.constraints import FixAtoms
 from ase.neb import interpolate, idpp_interpolate
 
 from .. import parse_constraint_info
 from ..reactor import AbstractReactor
-from ..utils import plot_bands, plot_mep
-
-
-def set_constraint(atoms, cons_text):
-    """"""
-    atoms._del_constraints()
-    mobile_indices, frozen_indices = parse_constraint_info(
-        atoms, cons_text, ignore_ase_constraints=True, ret_text=False
-    )
-    if frozen_indices:
-        atoms.set_constraint(FixAtoms(indices=frozen_indices))
-
-    return atoms
+from ..utils import plot_bands, plot_mep, compute_rxn_coords
 
 
 @dataclasses.dataclass
 class StringReactorSetting:
 
     #: Reactor setting.
     backend: str = "external"
 
+    #: Period to save the trajectory.
+    dump_period: int = 1
+
     #: Period to save the restart file.
     ckpt_period: int = 100
 
     #: Number of images along the pathway.
     nimages: int = 7
 
     #: Align IS and FS based on the mic.
     mic: bool = True
-    
+
     #: Optimiser.
     optimiser: str = "bfgs"
 
     #: Spring constant, eV/Ang2.
     k: float = 5.0
 
     #: Whether use CI-NEB.
@@ -72,39 +63,44 @@
     #: Convergence force tolerance.
     fmax: float = 0.05
 
     #: Maximum number of steps.
     steps: int = 100
 
     #: FixAtoms.
-    constraint: str = None
+    constraint: Optional[str] = None
 
     #: Parameters that are used to update.
     _internals: dict = dataclasses.field(default_factory=dict)
 
     def get_init_params(self):
         """"""
 
         return copy.deepcopy(self._internals)
 
     def get_run_params(self):
         """"""
 
-        raise NotImplementedError(f"{self.__class__.__name__} has no function for run params.")
+        raise NotImplementedError(
+            f"{self.__class__.__name__} has no function for run params."
+        )
+
 
 class AbstractStringReactor(AbstractReactor):
 
     name: str = "string"
 
     traj_name: str = "nebtraj.xyz"
 
     @AbstractReactor.directory.setter
-    def directory(self, directory_):
+    def directory(self, directory_: Union[str, pathlib.Path]):
         self._directory = pathlib.Path(directory_)
-        self.calc.directory = str(self.directory) # NOTE: avoid inconsistent in ASE
+        # avoid inconsistent in ASE
+        # the actual calc directory will be set in _irun
+        self.calc.directory = str(self.directory)
 
         return
 
     def run(self, structures: List[Atoms], read_ckpt=True, *args, **kwargs):
         """"""
         super().run(structures=structures, *args, **kwargs)
 
@@ -137,117 +133,152 @@
             if not converged:
                 self._debug(f"... unconverged @ {self.directory.name} ...")
                 ckpt_wdir = self._save_checkpoint() if read_ckpt else None
                 self._debug(f"... checkpoint @ {str(ckpt_wdir)} ...")
                 self._irun(structures, ckpt_wdir=ckpt_wdir, *args, **kwargs)
             else:
                 self._debug(f"... converged @ {self.directory.name} ...")
-        
+
         self.calc.parameters = prev_params
         self.calc.reset()
 
         # - check again
         curr_band, converged = None, self.read_convergence()
         if converged:
             self._debug(f"... 2. converged @ {self.directory.name} ...")
-            band_frames = self.read_trajectory() # (nbands, nimages)
+            band_frames = self.read_trajectory()  # (nbands, nimages)
             if band_frames:
+                # FIXME: make below a function
                 plot_mep(self.directory, band_frames[-1])
-                #plot_bands(self.directory, images, nimages=nimages_per_band)
-                write(self.directory/"temptraj.xyz", itertools.chain(*band_frames))
-                # --
+                write(self.directory / "temptraj.xyz", itertools.chain(*band_frames))
+
                 curr_band = band_frames[-1]
+
+                rxn_coords = compute_rxn_coords(curr_band)
+
                 energies = [a.get_potential_energy() for a in curr_band]
                 imax = 1 + np.argsort(energies[1:-1])[-1]
                 # NOTE: maxforce in cp2k is norm(atomic_forces)
                 maxfrc = np.max(curr_band[imax].get_forces(apply_constraint=True))
 
-                self._print(f"imax: {imax}")
                 self._print(
-                    f"maxfrc: {maxfrc} Ea_f: {energies[imax]-energies[0]:<8.4f} dE: {energies[-1]-energies[0]:<8.4f}"
+                    f"rxncoords: {rxn_coords[0]:.2f} -> {rxn_coords[imax]:.2f} "
+                    + f"-> {rxn_coords[-1]:.2f}"
+                )
+                self._print(
+                    f"maxfrc: {maxfrc} Ea_f: {energies[imax]-energies[0]:<8.4f} "
+                    + f"dE: {energies[-1]-energies[0]:<8.4f}"
                 )
             else:
                 self._debug(f"... CANNOT read bands @ {self.directory.name} ...")
                 ...
         else:
             self._debug(f"... 2. unconverged @ {self.directory.name} ...")
 
         return curr_band
-    
+
     @abc.abstractmethod
     def _irun(self, structures: List[Atoms], *args, **kwargs):
         """"""
 
         return
 
     def _verify_checkpoint(self, *args, **kwargs) -> bool:
-        """Check if the current directory has any valid outputs or it just created 
-            the input files.
+        """Check if the current directory has any valid outputs or it just created
+        the input files.
 
         """
 
         return self.directory.exists()
-    
+
     def _save_checkpoint(self, *args, **kwargs):
         """"""
         # - find previous runs...
         prev_wdirs = sorted(self.directory.glob(r"[0-9][0-9][0-9][0-9][.]run"))
         self._debug(f"prev_wdirs: {prev_wdirs}")
         curr_index = len(prev_wdirs)
 
-        curr_wdir = self.directory/f"{str(curr_index).zfill(4)}.run"
+        curr_wdir = self.directory / f"{str(curr_index).zfill(4)}.run"
         self._debug(f"curr_wdir: {curr_wdir}")
 
         # - backup files
         curr_wdir.mkdir()
         for x in self.directory.iterdir():
             if not re.match(r"[0-9]{4}\.run", x.name):
                 # NOTE: default is to move everything to the new folder
-                #if x.name in self.saved_fnames:
+                # if x.name in self.saved_fnames:
                 #    shutil.move(x, curr_wdir)
-                #else:
+                # else:
                 #    x.unlink()
                 shutil.move(x, curr_wdir)
             else:
                 ...
 
         return curr_wdir
 
-    def _align_structures(self, structures, *args, **kwargs) -> List[Atoms]:
+    def _preprocess_constraints(self, atoms, cons_text: str) -> None:
         """"""
+        atoms._del_constraints()
+        mobile_indices, frozen_indices = parse_constraint_info(
+            atoms, cons_text, ignore_ase_constraints=True, ret_text=False
+        )
+        if frozen_indices:
+            atoms.set_constraint(FixAtoms(indices=frozen_indices))
+
+        return
+
+    def _align_structures(
+        self, structures: List[Atoms], run_params: dict, *args, **kwargs
+    ) -> List[Atoms]:
+        """Create a reaction pathway based on two structures.
+
+        Args:
+            structures: Two structures - Initial state and Final State.
+            run_params: We need thet latest `constraint` information.
+
+        Returns:
+            A List of Atoms structures.
+
+        """
         nstructures = len(structures)
         if nstructures == 2:
             # - check lattice consistency
             ini_atoms, fin_atoms = structures
-            c1, c2 = ini_atoms.get_cell(complete=True), fin_atoms.get_cell(complete=True)
+            c1, c2 = ini_atoms.get_cell(complete=True), fin_atoms.get_cell(
+                complete=True
+            )
             assert np.allclose(c1, c2), "Inconsistent unit cell..."
 
             # - align structures
             shifts = fin_atoms.get_positions() - ini_atoms.get_positions()
             if self.setting.mic:
                 self._print("Align IS and FS based on MIC.")
                 curr_vectors, curr_distances = find_mic(shifts, c1, pbc=True)
                 self._debug(f"curr_vectors: {curr_vectors}")
                 self._print(f"disp: {np.linalg.norm(curr_vectors)}")
                 fin_atoms.positions = ini_atoms.get_positions() + curr_vectors
             else:
                 self._print(f"disp: {np.linalg.norm(shifts)}")
 
-            ini_atoms = set_constraint(ini_atoms, self.setting.constraint)
-            fin_atoms = set_constraint(fin_atoms, self.setting.constraint)
+            cons_text = run_params.pop("constraint", None)
+            self._preprocess_constraints(ini_atoms, cons_text)
+            self._preprocess_constraints(fin_atoms, cons_text)
 
             # - find mep
             nimages = self.setting.nimages
             images = [ini_atoms]
-            images += [ini_atoms.copy() for i in range(nimages-2)]
+            images += [ini_atoms.copy() for i in range(nimages - 2)]
             images.append(fin_atoms)
 
             interpolate(
-                images=images, mic=False, interpolate_cell=False, 
-                use_scaled_coord=False, apply_constraint=False
+                images=images,
+                mic=False,
+                interpolate_cell=False,
+                use_scaled_coord=False,
+                apply_constraint=False,
             )
         else:
             self._print("Use a pre-defined pathway.")
             images = [a.copy() for a in structures]
 
         return images
 
@@ -257,38 +288,63 @@
         prev_wdirs = sorted(self.directory.glob(r"[0-9][0-9][0-9][0-9][.]run"))
         self._debug(f"prev_wdirs: {prev_wdirs}")
 
         traj_list = []
         for w in prev_wdirs:
             curr_frames = self._read_a_single_trajectory(wdir=w)
             traj_list.append(curr_frames)
-        
+
         cache_nebtraj = self.directory / self.traj_name
         if cache_nebtraj.exists() and cache_nebtraj.stat().st_size != 0:
             traj_list.append(self._read_a_single_trajectory(wdir=self.directory))
-        
+
         # - concatenate
         traj_frames, ntrajs = [], len(traj_list)
         if ntrajs > 0:
             traj_frames.extend(traj_list[0])
             for i in range(1, ntrajs):
-                prev_end_band, curr_beg_band = traj_list[i-1][-1], traj_list[i][0]
+                prev_end_band, curr_beg_band = traj_list[i - 1][-1], traj_list[i][0]
                 for j, (a, b) in enumerate(zip(prev_end_band, curr_beg_band)):
-                    assert np.allclose(a.positions, b.positions), f"Traj {i-1} and traj {i} are not consecutive in positions."
+                    assert np.allclose(
+                        a.positions, b.positions
+                    ), f"Traj {i-1} and traj {i} are not consecutive in positions."
                 traj_frames.extend(traj_list[i][1:])
         else:
             ...
 
+        if traj_frames:
+            # FIXME: make below a function
+            plot_mep(self.directory, traj_frames[-1])
+
+            curr_band = traj_frames[-1]
+
+            rxn_coords = compute_rxn_coords(curr_band)
+
+            energies = [a.get_potential_energy() for a in curr_band]
+            imax = 1 + np.argsort(energies[1:-1])[-1]
+            # NOTE: maxforce in cp2k is norm(atomic_forces)
+            maxfrc = np.max(curr_band[imax].get_forces(apply_constraint=True))
+
+            self._print(f"imax: {imax}")
+            self._print(
+                f"rxncoords: {rxn_coords[0]:.2f} -> {rxn_coords[imax]:.2f} "
+                + f"-> {rxn_coords[-1]:.2f}"
+            )
+            self._print(
+                f"maxfrc: {maxfrc} Ea_f: {energies[imax]-energies[0]:<8.4f} "
+                + f"dE: {energies[-1]-energies[0]:<8.4f}"
+            )
+
         return traj_frames
 
     def as_dict(self) -> dict:
         """"""
         params = {}
 
-        #self._print(f"{self.setting.backend = }")
+        # self._print(f"{self.setting.backend = }")
 
         for k, v in dataclasses.asdict(self.setting).items():
             if not k.startswith("_"):
                 params[k] = v
 
         return params
```

### Comparing `gdpx-0.0.5/src/gdpx/reactor/string/vasp.py` & `gdpx-0.0.6/src/gdpx/utils/atomUtils.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,256 +1,268 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
-
 import copy
-import itertools
-import dataclasses
-import os
-import pathlib
-import re
 import shutil
-import traceback
-
-from typing import Union, List
+import argparse
+from pathlib import Path
 
 import numpy as np
+import networkx as nx
+
+from tqdm import tqdm
 
 from ase import Atoms
-from ase import units
 from ase.io import read, write
-from ase.calculators.cp2k import parse_input, InputSection
-from ase.calculators.singlepoint import SinglePointCalculator
-from ase.constraints import FixAtoms
-from ase.neb import NEB
 
-from .string import AbstractStringReactor, StringReactorSetting
-from .. import parse_constraint_info
-
-
-def run_vasp(name, command, directory):
-    """Run vasp from the command. 
-    
-    ASE Vasp does not treat restart of a MD simulation well. Therefore, we run 
-    directly from the command if INCAR aready exists.
-    
-    """
-    import subprocess
-    from ase.calculators.calculator import EnvironmentError, CalculationFailed
 
-    try:
-        proc = subprocess.Popen(command, shell=True, cwd=directory)
-    except OSError as err:
-        # Actually this may never happen with shell=True, since
-        # probably the shell launches successfully.  But we soon want
-        # to allow calling the subprocess directly, and then this
-        # distinction (failed to launch vs failed to run) is useful.
-        msg = 'Failed to execute "{}"'.format(command)
-        raise EnvironmentError(msg) from err
-
-    errorcode = proc.wait()
-
-    if errorcode:
-        path = os.path.abspath(directory)
-        msg = ('Calculator "{}" failed with command "{}" failed in '
-               '{} with error code {}'.format(name, command,
-                                              path, errorcode))
-        raise CalculationFailed(msg)
-
-    return
-
-
-@dataclasses.dataclass
-class VaspStringReactorSetting(StringReactorSetting):
-
-    backend: str = "vasp"
-
-    #: Number of tasks/processors/cpus for each image.
-    ntasks_per_image: int = 1
-
-    def __post_init__(self):
-        """"""
-        self._internals.update(
-            # ---
-            ibrion = 3,
-            potim = 0,
-            isif = 2,
-            # ---
-            lclimb = self.climb,
-            ichain = 0,
-            images = self.nimages-2,
-            iopt = 1,
-            spring = -5,
-        )
+"""This temporarily stores some utilities for atoms object.
+"""
 
-        return
-    
-    def get_run_params(self, *args, **kwargs):
-        """"""
-        # - convergence criteria
-        fmax_ = kwargs.get("fmax", self.fmax)
-        steps_ = kwargs.get("steps", self.steps)
+def check_convergence(atoms, fmax=0.05):
+    """Check the convergence of the trajectory"""
 
-        run_params = dict(
-            constraint = kwargs.get("constraint", self.constraint),
-            ediffg = fmax_*-1., nsw=steps_
-        )
+    forces = atoms.get_forces()
 
-        return run_params
+    max_force = np.max(np.fabs(forces))
+
+    converged = False
+    if max_force < fmax:
+        converged = True 
+
+    return converged
+
+def merge_xyz():
+    parser = argparse.ArgumentParser()
+    parser.add_argument(
+        "-p", "--pattern",
+        help="pattern to find xyz files"
+    )
+    args = parser.parse_args()
+
+    #pattern = "s2hcp"
+    pattern = args.pattern
+    cwd = Path.cwd()
+
+    sorted_paths = []
+    for p in cwd.glob(pattern+"*.xyz"):
+        sorted_paths.append(p)
+    sorted_paths.sort()
+
+    frames = []
+    for p in sorted_paths:
+        cur_frames = read(p, ":")
+        print(p.stem)
+        for atoms in cur_frames:
+            atoms.info["source"] = str(p.stem)
+        print(p, " #frames: ", len(cur_frames))
+        frames.extend(cur_frames)
+    print("TOTAL #frames: ", len(frames))
+    write(pattern+"-0906.xyz", frames)
+
+    for p in sorted_paths:
+        shutil.move(p, cwd / ("bak."+p.name))
+
+
+def sort_atoms(atoms):
+    # sort atoms by symbols and z-positions especially for supercells 
+    numbers = atoms.numbers 
+    zposes = atoms.positions[:,2].tolist()
+    sorted_indices = np.lexsort((zposes,numbers))
+    atoms = atoms[sorted_indices]
 
+    return atoms
 
-class VaspStringReactor(AbstractStringReactor):
 
-    name: str = "vasp"
+def try_sort():
+    frames = read('./test_data.xyz', ':')
+    
+    new_frames = [sort_atoms(atoms) for atoms in frames]
+    write('new_test.xyz', new_frames)
 
-    traj_name: str = "01/OUTCAR"
 
-    def __init__(self, calc=None, params={}, ignore_convergence=False, directory="./", *args, **kwargs) -> None:
-        """"""
-        self.calc = calc
-        if self.calc is not None:
-            self.calc.reset()
+def get_structure_type(atoms_: Atoms) -> str:
+    """Determine the structure type based on atom connectivity.
 
-        self.ignore_convergence = ignore_convergence
+    For bulk, there are bond connections in xyz 3 dimensions. For surface, there 
+    are bond connections in one dimensions (default should be z-axis). For cluster
+    or molecue, there are no bond connections among neighbour cells.
 
-        self.directory = directory
+    Returns:
+        bulk, surface, and cluster
 
-        # - parse params
-        self.setting = VaspStringReactorSetting(**params)
-        self._debug(self.setting)
+    """
+    #natoms = len(atoms)
 
-        return
-    
-    def _verify_checkpoint(self):
-        """Check if the current directory has any valid outputs or it just created 
-            the input files.
-
-        """
-        verified = super()._verify_checkpoint()
-        if verified:
-            checkpoints = list(self.directory.glob("*vasprun.xml"))
-            self._debug(f"checkpoints: {checkpoints}")
-            if not checkpoints:
-                verified = False
+    #from ase.neighborlist import natural_cutoffs, NeighborList
+    #cutoffs = natural_cutoffs(atoms, mult=1.0)
+    #neigh = NeighborList(
+    #    cutoffs, skin=0.0, sorted=False, self_interaction=True, bothways=False,
+    #)
+    #neigh.update(atoms)
+
+    #stype = "cluster"
+    #has_x, has_y, has_z = False, False, False
+    #for i in range(natoms):
+    #    indices, offsets = neigh.get_neighbors(i)
+    #    for j, offset in zip(indices, offsets):
+    #        if offset[0] != 0:
+    #            has_x = True
+    #        if offset[1] != 0:
+    #            has_y = True
+    #        if offset[2] != 0:
+    #            has_z = True
+    #        print(f"{i}-{j}: ", offset, [has_x, has_y, has_z])
+    #    if has_x and has_y and has_z:
+    #        stype = "bulk"
+    #        break
+    #if sum([has_x, has_y, has_z]) == 2:
+    #    stype = "surface"
+    #    # TODO: find in which direction is the vaccum
+    #    ...
+    #print([has_x, has_y, has_z])
+    atoms = copy.deepcopy(atoms_)
+    #stype = atoms.info.get("stype")
+
+    # -
+    graph = create_multipgraph(atoms)
+    # NOTE: A cluster has atoms concentrated around the centre.
+    is_cluster = True
+    # TODO: water box?
+    #print(graph)
+    for u, v, d in graph.edges.data():
+        #print(u, v, d)
+        # NOTE: at least a surface if there are bonds between neighbour boxs
+        # TODO: a single molecule crosses the boundary?
+        if sum(d["offset"]) != 0:
+            is_cluster = False
+            break
+
+    if not is_cluster:
+        # --- check if surface or bulk
+        graph = create_multipgraph(atoms, pbc=False)
+        subgraphs = [graph.subgraph(nodes) for nodes in nx.connected_components(graph)]
+        #print(subgraphs)
+        # TODO: water box?
+        cell_ = atoms.get_cell(complete=True)
+        if len(subgraphs) == 1:
+            #stype = "bulk"
+            positions_ = atoms.get_positions()
         else:
-            ...
-
-        return verified
-    
-    def _irun(self, structures: List[Atoms], ckpt_wdir=None, *args, **kwargs):
-        """"""
-        try:
-            # --
-            run_params = self.setting.get_run_params(**kwargs)
-            run_params.update(**self.setting.get_init_params())
-
-            if ckpt_wdir is None: # start from the scratch
-                images = self._align_structures(structures)
-                write(self.directory/"images.xyz", images)
-            else:
-                # - update structures
-                rep_dirs = sorted([x.name for x in sorted(self.directory.glob(r"[0-9][0-9]"))])
-
-                frames_ = []
-                for x in rep_dirs[1:-1]:
-                    frames_.append(read(self.directory/x/"OUTCAR", ":"))
-                nframes = min([len(x) for x in frames_])
-                assert nframes > 0, "At least one step finished before resume..."
-                intermediates_ = [x[nframes-1] for x in frames_]
-                images = [structures[0]] + intermediates_ + [structures[-1]]
-
-                run_params.update(
-                    steps = self.setting.steps - nframes
-                )
-
-            # -- check constraint
-            atoms = images[0] # use the initial state
-            cons_text = run_params.pop("constraint", None)
-            mobile_indices, frozen_indices = parse_constraint_info(
-                atoms, cons_text=cons_text, ignore_ase_constraints=True, ret_text=False
-            )
-            if frozen_indices:
-                #atoms._del_constraints()
-                #atoms.set_constraint(FixAtoms(indices=frozen_indices))
-                frozen_indices = sorted(frozen_indices)
-                for a in images:
-                    a.set_constraint(FixAtoms(indices=frozen_indices))
-
-            # -- add replica information
-            for i, a in enumerate(images):
-                rep_dir = (self.directory/str(i).zfill(2))
-                rep_dir.mkdir() # TODO: exists?
-                write(rep_dir/"POSCAR", a)
-
-            # - update input
-            self.calc.set(**run_params)
-            atoms.calc = self.calc
-
-            # - run calculation
-            self.calc.write_input(atoms)
-            if (self.directory/"POSCAR").exists():
-                os.remove(self.directory/"POSCAR")
-            run_vasp("vasp", atoms.calc.command, self.directory)
-
-        except Exception as e:
-            self._debug(e)
-            self._debug(traceback.print_exc())
-
-        return
-    
-    def read_convergence(self, *args, **kwargs):
-        """"""
-        converged = super().read_convergence(*args, **kwargs)
-
-        with open(self.directory/"vasp.out", "r") as fopen:
-            lines = fopen.readlines()
-        
-        for line in lines:
-            if "reached required accuracy" in line:
-                converged = True
-                break
-
-        return converged
+            cops = [
+                np.average(atoms.positions[g.nodes], axis=0).tolist()
+                for g in subgraphs
+            ]
+            orders = [x[0] for x in sorted(enumerate(cops), key=lambda x: x[1][2])]
+            #print(cops)
+            #print(orders)
+            positions_ = copy.deepcopy(atoms.get_positions())
+            for i in orders[1:]:
+                for a_idx in subgraphs[i].nodes:
+                    positions_[a_idx] += np.dot(cell_, [0,0,-1])
+            # NOTE: avoid some bulk systems that they are moved far below
+            if np.average(positions_, axis=0)[2] < 0.:
+                positions_ = copy.deepcopy(atoms.get_positions())
+
+        zvec = np.cross(cell_[0], cell_[1])
+        zlength = np.dot(zvec/np.linalg.norm(zvec), cell_[2])
+        max_zpos = np.max(positions_[:,2])
+        #print("max_zpos: ", max_zpos)
+        if max_zpos + 6.0 <= zlength: # NOTE: larger than a cutoff
+            stype = "surface"
+        else:
+            stype = "bulk"
+        #print(stype)
+    else:
+        stype = "cluster"
+
+    return stype
+
+def create_multipgraph(atoms_, pbc=True):
+    """"""
+    atoms = copy.deepcopy(atoms_)
+
+    graph = nx.MultiGraph(atoms=atoms)
+    #print(graph.graph)
+
+    # - find neighbours
+    natoms = len(atoms)
+    atoms.pbc = pbc
+    #atoms.pbc = False
+    #atoms.pbc = [True, True, False]
+
+    from ase.neighborlist import natural_cutoffs, NeighborList
+    cutoffs = natural_cutoffs(atoms, mult=1.2)
+    #cutoffs = [6.0]*natoms
+    neigh = NeighborList(
+        cutoffs, skin=0.0, sorted=False, self_interaction=False, bothways=False,
+    )
+    neigh.update(atoms)
+
+    # -- add nodes
+    nodes = [[i, {"symbol": a.symbol}] for i, a in enumerate(atoms)]
+    graph.add_nodes_from(nodes)
+    #print(graph)
+    #for u, d in graph.nodes.data():
+    #    print(u, d)
+
+    # -- add edges
+    edges = []
+    for i in range(natoms):
+        indices, offsets = neigh.get_neighbors(i)
+        for j, offset in zip(indices, offsets):
+            edges.append([i, j, {"route": 2, "offset": offset.tolist()}])
+    graph.add_edges_from(edges)
+
+    #print("--- edges ---") # find egdes without offset [0,0,0]
+    #for u, v, d in graph.edges.data():
+    #    print(u, v, d)
+    #for u, v, keys in graph.edges(keys=True):
+    #    print(u, v, keys)
+    #for n, nbrsdict in graph.adjacency():
+    #    print(n, nbrsdict)
+    #    for nbr, keydict in nbrsdict.items():
+    #        print(nbr, keydict)
+    #        for key, eattr in keydict.items():
+    #            ...
+    #print(graph.edges())
+    #print(set(graph.edges()))
+    #for u, v, d in graph.edges.data(nbunch=[10]):
+    #    print(u, v, d)
     
-    def _read_a_single_trajectory(self, wdir, *args, **kwargs):
-        """
+    # -- find subgraphs
+    #subgraphs = nx.connected_components(graph)
+    #print(subgraphs)
 
-        NOTE: Fixed atoms have zero forces.
-
-        """
-        self._debug(f"***** read_trajectory *****")
-        self._debug(f"{str(wdir)}")
-
-        images = read(wdir/"images.xyz", ":")
-        ini_atoms, fin_atoms = images[0], images[-1]
-
-        # TODO: energy and forces of IS and FS?
-        calc = SinglePointCalculator(
-            ini_atoms, energy=ini_atoms.info["energy"], forces=np.zeros((len(ini_atoms), 3))
-        )
-        ini_atoms.calc = calc
-        calc = SinglePointCalculator(
-            fin_atoms, energy=fin_atoms.info["energy"], forces=np.zeros((len(fin_atoms), 3))
-        )
-        fin_atoms.calc = calc
-
-        # - read OUTCARs
-        frames_ = []
-        for i in range(1, self.setting.nimages-1):
-            curr_frames = read(wdir/f"{str(i).zfill(2)}"/"OUTCAR", ":")
-            frames_.append(curr_frames)
-
-        # nframes may not consistent across replicas 
-        # due to unfinished calculations
-        nframes_list = [len(x) for x in frames_]
-        nsteps = min(nframes_list) 
-
-        frames = []
-        for i in range(nsteps):
-            curr_frames = [ini_atoms] + [frames_[j][i] for j in range(self.setting.nimages-2)] + [fin_atoms]
-            frames.append(curr_frames)
-
-        return frames
+    return graph
 
 
 if __name__ == "__main__":
+    """"""
+    stru_dict = {}
+
+    frames = read("/home/jx1279/projects/sintering/dataset/Cu12.xyz", ":")
+    #frames = read("/home/jx1279/projects/sintering/dataset/Cu16.xyz", ":")
+    #frames = read("/home/jx1279/projects/sintering/dataset/Cu87.xyz", ":")
+    nframes = len(frames)
+    print("nframes: ", nframes)
+
+    for i, atoms in tqdm(enumerate(frames)):
+        atoms.info["confid"] = i
+        # NOTE: cluster/molecule (0d), nanowire (1d), surface (2d), bulk (3d)
+        # TODO: determine by volume?
+        stype = get_structure_type(atoms)
+
+        # -- 
+        name = f"{atoms.get_chemical_formula()}_{stype}"
+        if name in stru_dict:
+            stru_dict[name].append(atoms)
+        else:
+            stru_dict[name] = [atoms]
+    
+    new_nframes = 0
+    for (name, cur_frames) in stru_dict.items():
+        new_nframes += len(cur_frames)
+        print(len(cur_frames))
+        write(f"./{name}.xyz", cur_frames)
+    print(new_nframes)
     ...
```

### Comparing `gdpx-0.0.5/src/gdpx/reactor/utils.py` & `gdpx-0.0.6/src/gdpx/reactor/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 
 import copy
 
-from typing import List
+from typing import List, Callable
 
 import numpy as np
 
 from matplotlib import pyplot as plt
 try:
     plt.style.use("presentation")
 except Exception as e:
@@ -53,18 +53,14 @@
     rxn_coords = np.cumsum(rxn_coords)
     rxn_coords = np.hstack(([0.], rxn_coords))
 
     return rxn_coords
 
 def plot_mep(wdir, images):
     """"""
-    print("nimages: ", len(images))
-    rxn_coords = compute_rxn_coords(images)
-    print("rxn_coords: ", rxn_coords)
-
     fig, ax = plt.subplots(nrows=1, ncols=1, figsize=(12, 8))
     plt.suptitle("Nudged Elastic Band Calculation")
 
     nbt = NEBTools(images=images)
     nbt.plot_band(ax=ax)
 
     plt.savefig(wdir/"neb.png")
@@ -91,8 +87,8 @@
 
     plt.savefig(wdir/"bands.png")
 
     return
 
 
 if __name__ == "__main__":
-    ...
+    ...
```

### Comparing `gdpx-0.0.5/src/gdpx/scheduler/__init__.py` & `gdpx-0.0.6/src/gdpx/scheduler/__init__.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.5/src/gdpx/scheduler/interface.py` & `gdpx-0.0.6/src/gdpx/scheduler/interface.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.5/src/gdpx/scheduler/local.py` & `gdpx-0.0.6/src/gdpx/scheduler/local.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.5/src/gdpx/scheduler/lsf.py` & `gdpx-0.0.6/src/gdpx/scheduler/lsf.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.5/src/gdpx/scheduler/pbs.py` & `gdpx-0.0.6/src/gdpx/scheduler/pbs.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.5/src/gdpx/scheduler/scheduler.py` & `gdpx-0.0.6/src/gdpx/scheduler/scheduler.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.5/src/gdpx/scheduler/slurm.py` & `gdpx-0.0.6/src/gdpx/scheduler/slurm.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.5/src/gdpx/selector/__init__.py` & `gdpx-0.0.6/src/gdpx/selector/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,14 +30,18 @@
 
 registers.selector.register(PropertySelector)
 
 from .random import RandomSelector
 
 registers.selector.register(RandomSelector)
 
+from .scf import ScfSelector
+
+registers.selector.register(ScfSelector)
+
 try:
     # TODO: This selector depends on an external package dscribe.
     from .descriptor import DescriptorSelector
 
     registers.selector.register(DescriptorSelector)
 except ImportError as e:
     warnings.warn(f"Module DescriptorSelector import failed: {e}", UserWarning)
```

### Comparing `gdpx-0.0.5/src/gdpx/selector/basin.py` & `gdpx-0.0.6/src/gdpx/selector/basin.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.5/src/gdpx/selector/compare.py` & `gdpx-0.0.6/src/gdpx/selector/compare.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.5/src/gdpx/selector/composition.py` & `gdpx-0.0.6/src/gdpx/selector/composition.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.5/src/gdpx/selector/cur.py` & `gdpx-0.0.6/src/gdpx/selector/cur.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.5/src/gdpx/selector/descriptor.py` & `gdpx-0.0.6/src/gdpx/selector/descriptor.py`

 * *Files 2% similar despite different names*

```diff
@@ -186,37 +186,40 @@
         import matplotlib.pyplot as plt
 
         try:
             plt.style.use("presentation")
         except Exception as e:
             ...
 
-        reducer = PCA(n_components=2)
-        reducer.fit(features)
-        proj = reducer.transform(features)
-
-        for grp_name, inds in groups.items():
-            sc = plt.scatter(
-                proj[others[grp_name], 0],
-                proj[others[grp_name], 1],
-                marker="o",
-                alpha=0.25,
-                label=f"grp-{grp_name} {len(others[grp_name])} -> {len(inds)}",
-            )
-            # --
-            selected_proj = reducer.transform(np.array([features[i] for i in inds]))
-            plt.scatter(
-                selected_proj[:, 0],
-                selected_proj[:, 1],
-                marker="*",
-                alpha=0.5,
-                color="r",
-            )
-        plt.legend(fontsize=12)
-        plt.axis("off")
-        plt.savefig(self.info_fpath.parent / (self.info_fpath.stem + ".png"))
+        if features.shape[0] > 1:
+            reducer = PCA(n_components=2)
+            reducer.fit(features)
+            proj = reducer.transform(features)
+
+            for grp_name, inds in groups.items():
+                sc = plt.scatter(
+                    proj[others[grp_name], 0],
+                    proj[others[grp_name], 1],
+                    marker="o",
+                    alpha=0.25,
+                    label=f"grp-{grp_name} {len(others[grp_name])} -> {len(inds)}",
+                )
+                # --
+                selected_proj = reducer.transform(np.array([features[i] for i in inds]))
+                plt.scatter(
+                    selected_proj[:, 0],
+                    selected_proj[:, 1],
+                    marker="*",
+                    alpha=0.5,
+                    color="r",
+                )
+            plt.legend(fontsize=12)
+            plt.axis("off")
+            plt.savefig(self.info_fpath.parent / (self.info_fpath.stem + ".png"))
+        else:
+            ... # Cannot plot PCA with only one structure...
 
         return
 
 
 if __name__ == "__main__":
     ...
```

### Comparing `gdpx-0.0.5/src/gdpx/selector/graph.py` & `gdpx-0.0.6/src/gdpx/selector/graph.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.5/src/gdpx/selector/interface.py` & `gdpx-0.0.6/src/gdpx/validator/interface.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,172 +1,155 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 import copy
-import itertools
-import pathlib
-from typing import Union, List, NoReturn
+from typing import NoReturn
 
 import omegaconf
 
-from ase import Atoms
-from ase.io import read, write
-
-from ..core.variable import Variable
+from ..core.variable import Variable, DummyVariable
 from ..core.operation import Operation
 from ..core.register import registers
 
-from ..worker.worker import AbstractWorker
 from ..data.array import AtomsNDArray
-
-from ..builder.interface import build, BuilderVariable
-
-from .selector import AbstractSelector, load_cache
-from .composition import ComposedSelector
-
+from ..data.dataset import AbstractDataloader
+from ..worker.drive import DriverBasedWorker
+from .validator import AbstractValidator
 
 @registers.variable.register
-class SelectorVariable(Variable):
+class ValidatorVariable(Variable):
 
-    def __init__(self, selection: Union[dict, List[dict]], directory="./", *args, **kwargs) -> None:
-        """Define a Variable that has a Selector."""
-        # We can define a selector in two different ways:
-        # The Dict must have a selection key
-        # - a Dict that defines a single selector
-        # - a List of Dict that defines several selectors, 
-        #   which will be converted into a composed one
-        selection = copy.deepcopy(selection)
-        if isinstance(selection, dict) or isinstance(selection, omegaconf.dictconfig.DictConfig):
-            selection = [selection]
-        elif isinstance(selection, list) or isinstance(selection, omegaconf.listconfig.ListConfig):
-            ...
-        else:
-            raise TypeError(f"Unknown type of {selection =}.")
-
-        selectors = []
-        for params in selection:
-            method = params.pop("method", None)
-            selector = registers.create("selector", method, convert_name=True, **params)
-            selectors.append(selector)
-        nselectors = len(selectors)
-        if nselectors > 1:
-            selector = ComposedSelector(selectors)
-        else:
-            selector = selectors[0]
+    def __init__(self, directory="./", **kwargs):
+        """"""
+        # - create a validator
+        method = kwargs.get("method", "minima")
+        validator = registers.create("validator", method, convert_name=False, **kwargs)
 
-        super().__init__(initial_value=selector, directory=directory)
+        # - save
+        super().__init__(initial_value=validator, directory=directory)
 
         return
-
-
+    
 @registers.operation.register
-class select(Operation):
+class validate(Operation):
 
-    cache_fname = "selected_frames.xyz"
+    """The operation to validate properties by potentials.
 
-    def __init__(self, structures, selector, directory="./", *args, **kwargs):
-        """"""
-        super().__init__(input_nodes=[structures, selector], directory=directory)
+    The reference properties should be stored and accessed through `structures`.
 
-        return
+    """
 
-    @Operation.directory.setter
-    def directory(self, directory_) -> NoReturn:
-        """"""
-        super(select, select).directory.__set__(self, directory_)
+    def __init__(
+        self, structures, validator, worker=DummyVariable(), 
+        run_params: dict={}, directory="./", *args, **kwargs
+    ) -> None:
+        """Init a validate operation.
+
+        Args:
+            structures: A node that forwards structures.
+            validator: A validator.
+            worker: A worker to run calculations. TODO: Make this optional.
+        
+        """
+        super().__init__(
+            input_nodes=[structures, validator, worker], directory=directory
+        )
 
-        return
+        self.run_params = run_params
 
+        return
+    
     def _preprocess_input_nodes(self, input_nodes):
-        """"""
-        structures, selector = input_nodes
-        if isinstance(structures, str) or isinstance(structures, pathlib.Path):
-            # TODO: check if it is a molecule name
-            structures = build(
-                BuilderVariable(
-                    directory=self.directory / "structures",
-                    method="reader",
-                    fname=structures,
-                )
-            )
-        # We can define a selector in two different ways:
-        # The Dict must have a selection key
-        # - a Dict that defines a single selector
-        # - a List of Dict that defines several selectors, 
-        #   which will be converted into a composed one
-        if isinstance(selector, dict) or isinstance(
-            selector, omegaconf.dictconfig.DictConfig
-        ):
-            selector = SelectorVariable(
-                directory=self.directory / "selector", **selector
-            )
-        #self._print(f"{selector = }")
-
-        return structures, selector
-
-    def forward(
-        self, structures: AtomsNDArray, selector: AbstractSelector
-    ) -> AtomsNDArray:
-        """"""
-        super().forward()
-        selector.directory = self.directory
+        """Preprocess valid input nodes.
 
-        cache_fpath = self.directory / self.cache_fname
-        if not cache_fpath.exists():
-            new_frames = selector.select(structures)
-            write(cache_fpath, new_frames)
-        else:
-            markers = load_cache(selector.info_fpath)
-            structures.markers = markers
-            new_frames = read(cache_fpath, ":")
-        self._print(f"nframes: {len(new_frames)}")
+        Some arguments accept basic python objects such list or dict, which are 
+        not necessary to be a Variable or an Operation.
 
-        self.status = "finished"
-
-        return structures
+        """
+        structures, validator, worker = input_nodes
 
+        if isinstance(validator, dict) or isinstance(validator, omegaconf.dictconfig.DictConfig):
+            validator = ValidatorVariable(self.directory/"validator", **validator)
+            self._print(validator)
 
-def run_selection(
-    param_file: Union[str, pathlib.Path],
-    structure: Union[str, dict],
-    directory: Union[str, pathlib.Path] = "./",
-) -> None:
-    """Run selection with input selector and input structures.
-
-    This no more accepts a worker as all data used in the selection should be 
-    computed in advance.
+        return structures, validator, worker
     
-    """
-    directory = pathlib.Path(directory)
-    if not directory.exists():
-        directory.mkdir(parents=True, exist_ok=False)
+    def _convert_dataset(self, structures):
+        """Validator can accept various formats of input structures. 
 
-    from gdpx.utils.command import parse_input_file
+        We convert all formats into one.
+        
+        """
+        # NOTE: In an active session, the dataset is dynamic, thus, 
+        #       we need load the dataset before run...
+        #       Validator accepts dict(reference=[], prediction=[])
+        dataset_ = {}
+        if hasattr(structures, "items"): # check if the input is a dict-like object
+            stru_dict = structures
+        else: # assume it is just an AtomsNDArray
+            stru_dict = {}
+            stru_dict["reference"] = structures
+
+        for k, v in stru_dict.items():
+            if isinstance(v, dict):
+                ...
+            elif isinstance(v, list):
+                ...
+            elif isinstance(v, AtomsNDArray):
+                ...
+            elif isinstance(v, AbstractDataloader):
+                v = v.load_frames()
+            else:
+                raise RuntimeError(f"{k} Dataset {type(v)} is not a dict or loader.")
+            dataset_[k] = v
 
-    params = parse_input_file(param_file)
+        dataset = dataset_
 
-    selector = SelectorVariable(
-        directory=directory, **params
-    ).value
-    selector.directory = directory
+        return dataset
+    
+    def forward(self, structures, validator: AbstractValidator, workers):
+        """Run a validator on input dataset.
+
+        Args:
+            structures: Any format that has Atoms objects.
 
-    # - read structures
-    from gdpx.builder import create_builder
+        """
+        super().forward()
 
-    builder = create_builder(structure)
-    frames = builder.run()  # -> List[Atoms]
+        # - create a worker
+        if workers is not None:
+            nworkers = len(workers)
+            assert nworkers == 1, f"Validator only accepts one worker but {nworkers} were given."
+            worker = workers[0]
+            worker.directory = self.directory
+        else:
+            worker = None
 
-    # TODO: convert to a bundle of atoms?
-    data = AtomsNDArray(frames)
+        # - convert dataset
+        dataset = self._convert_dataset(structures)
 
-    # -
-    selected_frames = selector.select(data)
+        # - run validation
+        validator.directory = self.directory
+        validator.run(dataset, worker, **self.run_params)
 
-    from ase.io import read, write
+        self.status = "finished"
 
-    write(directory / "selected_frames.xyz", selected_frames)
+        return # TODO: forward a reference-prediction pair?
+    
+    def report_convergence(self, *args, **kwargs) -> bool:
+        """"""
+        input_nodes = self.input_nodes
+        assert hasattr(input_nodes[1], "output"), f"Operation {self.directory.name} cannot report convergence without forwarding."
+        validator = input_nodes[1].output
+
+        self._print(f"{validator.__class__.__name__} Convergence")
+        if hasattr(validator, "report_convergence"):
+            converged = validator.report_convergence()
+        else:
+            self._print("    >>> True  (No report available)")
+            converged = True
 
-    return
+        return converged
 
 
 if __name__ == "__main__":
     ...
```

### Comparing `gdpx-0.0.5/src/gdpx/selector/interval.py` & `gdpx-0.0.6/src/gdpx/selector/interval.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.5/src/gdpx/selector/invariant.py` & `gdpx-0.0.6/src/gdpx/selector/invariant.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.5/src/gdpx/selector/locate.py` & `gdpx-0.0.6/src/gdpx/selector/locate.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.5/src/gdpx/selector/property.py` & `gdpx-0.0.6/src/gdpx/selector/property.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.5/src/gdpx/selector/random.py` & `gdpx-0.0.6/src/gdpx/selector/random.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.5/src/gdpx/selector/selector.py` & `gdpx-0.0.6/src/gdpx/selector/selector.py`

 * *Files 6% similar despite different names*

```diff
@@ -45,19 +45,29 @@
     header = lines[0]
 
     # - data
     data = lines[1:-1] # TODO: test empty data
 
     raw_markers = []
     if data:
-        # new_markers looks like [(0,1),(0,2),(1,0)]
+        # NOTE: new_markers looks like [(0,1),(0,2),(1,0)]
+        #       If no structures are selected, the info file should only contain
+        #       the header and the footer
         new_markers =[
             [int(x) for x in (d.strip().split()[0]).split(",")] for d in data
         ]
-        #raw_markers = group_markers(new_markers)
+        #new_markers = []
+        #for d in data:
+        #    curr_marker = []
+        #    for x in d.strip().split()[0].split(","):
+        #        if x.isdigit(): # MUST BE AN INTEGER
+        #            curr_marker.append(int(x))
+        #        else:
+        #            curr_marker.append(np.nan)
+        #    new_markers.append(curr_marker)
         raw_markers = new_markers
 
     # - footer
     footer = lines[-1]
     cache_random_seed = int(footer.strip().split()[-1]) # TODO: random state
     #assert cache_random_seed == random_seed
 
@@ -284,24 +294,30 @@
                 maxforce = np.max(np.fabs(atoms.get_forces(apply_constraint=True)))
             except:
                 maxforce = np.NaN
             score = atoms.info.get("score", np.nan)
             # - add info
             ind_str = ",".join([str(x) for x in ind])
             data.append([f"{ind_str}", confid, step, natoms, ene, ae, maxforce, score])
-
+        
         if data:
             save_cache(self.info_fpath, data, self.random_seed)
         else:
-            np.savetxt(
-                self.info_fpath, [[np.NaN]*8],
-                header="{:>11s}  {:>8s}  {:>8s}  {:>8s}  {:>12s}  {:>12s}  {:>12s}  {:>12s}".format(
-                    *"index confid step natoms ene aene maxfrc score".split()
-                ),
-                footer=f"random_seed {self.random_seed}"
+            #np.savetxt(
+            #    self.info_fpath, [[np.NaN]*8],
+            #    header="{:>11s}  {:>8s}  {:>8s}  {:>8s}  {:>12s}  {:>12s}  {:>12s}  {:>12s}".format(
+            #        *"index confid step natoms ene aene maxfrc score".split()
+            #    ),
+            #    footer=f"random_seed {self.random_seed}"
+            #)
+            content ="{:>11s}  {:>8s}  {:>8s}  {:>8s}  {:>12s}  {:>12s}  {:>12s}  {:>12s}".format(
+                *"index confid step natoms ene aene maxfrc score".split()
             )
+            content += f"random_seed {self.random_seed}"
+            with open(self.info_fpath, "w") as fopen:
+                fopen.write(content)
 
         return
 
 
 if __name__ == "__main__":
     ...
```

### Comparing `gdpx-0.0.5/src/gdpx/trainer/__init__.py` & `gdpx-0.0.6/src/gdpx/trainer/__init__.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.5/src/gdpx/trainer/interface.py` & `gdpx-0.0.6/src/gdpx/trainer/interface.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.5/src/gdpx/utils/cleave_cluster.py` & `gdpx-0.0.6/src/gdpx/utils/cleave_cluster.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.5/src/gdpx/utils/cmp_refdat.py` & `gdpx-0.0.6/src/gdpx/utils/cmp_refdat.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.5/src/gdpx/utils/command.py` & `gdpx-0.0.6/src/gdpx/utils/command.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,178 +8,190 @@
 from operator import itemgetter
 
 from typing import Any, Union, List
 
 import json
 import yaml
 
-import numpy as np
 
-
-def dict2str(d: dict, indent: int=2):
+def dict2str(d: dict, indent: int = 2):
     """Convert a nested dict to str."""
 
     def _dict2str(d_: dict, indent_: int):
         """Recursive function."""
         content = ""
         for k, v in d_.items():
             if isinstance(v, dict):
-                content += f"{k}:\n" + _dict2str(v, indent_+indent)
+                content += f"{k}:\n" + _dict2str(v, indent_ + indent)
             else:
-                content += " "*indent_ + f"{k}: {v}\n"
+                content += " " * indent_ + f"{k}: {v}\n"
 
         return content
 
     content = _dict2str(d, 0)
 
     return content
 
 
-class CustomTimer():
+class CustomTimer:
 
     def __init__(self, name="code", func=print):
         """"""
         self.name = name
         self._print = func
 
         return
-    
+
     def __call__(self, func) -> Any:
         """"""
 
         def func_timer(*args, **kwargs):
             st = time.time()
             ret = func(*args, **kwargs)
             et = time.time()
-            content = "*** "+self.name+" time: "+"{:>8.4f}".format(et-st)+" ***"
+            content = (
+                "*** " + self.name + " time: " + "{:>8.4f}".format(et - st) + " ***"
+            )
             self._print(content)
 
             return ret
 
         return func_timer
 
-
     def __enter__(self):
         """"""
-        self.st = time.time() # start time
+        self.st = time.time()  # start time
 
         return self
-    
+
     def __exit__(self, *args):
         """"""
-        self.et = time.time() # end time
+        self.et = time.time()  # end time
 
-        content = "*** "+self.name+" time: "+"{:>8.4f}".format(self.et-self.st)+" ***"
+        content = (
+            "*** "
+            + self.name
+            + " time: "
+            + "{:>8.4f}".format(self.et - self.st)
+            + " ***"
+        )
         self._print(content)
 
         return
 
+
 def check_path(target_dir: Union[str, Path]) -> bool:
-    """ check path existence, if so skip the following
-        TODO: add output option
-        make this into a context?
+    """check path existence, if so skip the following
+    TODO: add output option
+    make this into a context?
     """
     target_dir = Path(target_dir)
     if not target_dir.exists():
         target_dir.mkdir(parents=True)
     else:
         print(f"  {target_dir.name} exists, so next...")
 
     return
 
+
 def find_backups(dpath, fname, prefix="bak"):
-    """ find a series of files in a dir
-        such as fname, bak.0.fname, bak.1.fname
+    """find a series of files in a dir
+    such as fname, bak.0.fname, bak.1.fname
     """
     dpath = Path(dpath)
     fpath = dpath / fname
     if not fpath.exists():
         raise FileNotFoundError(f"fpath does not exist.")
 
-    backups = list(dpath.glob(prefix+".[0-9]*."+fname))
+    backups = list(dpath.glob(prefix + ".[0-9]*." + fname))
     backups = sorted(backups, key=lambda x: int(x.name.split(".")[1]))
     backups.append(fpath)
 
     return backups
 
+
 def run_command(directory, command, comment="", timeout=None):
     proc = subprocess.Popen(
-        command, shell=True, cwd=directory, 
-        stdout=subprocess.PIPE, stderr=subprocess.PIPE,
-        encoding = "utf-8"
+        command,
+        shell=True,
+        cwd=directory,
+        stdout=subprocess.PIPE,
+        stderr=subprocess.PIPE,
+        encoding="utf-8",
     )
     if timeout is None:
         errorcode = proc.wait()
     else:
         errorcode = proc.wait(timeout=timeout)
 
     msg = "Message: " + "".join(proc.stdout.readlines())
     print(msg)
     if errorcode:
-        raise RuntimeError("Error in %s at %s." %(comment, directory))
-    
+        raise RuntimeError("Error in %s at %s." % (comment, directory))
+
     return msg
 
-def convert_indices(indices: Union[str,List[int]], index_convention="lmp"):
-    """ parse indices for reading xyz by ase, get start for counting
-        constrained indices followed by lammps convention
-        "2:4 3:8"
-        convert [1,2,3,6,7,8] to "1:3 6:8"
-        lammps convention starts from 1 and includes end
-        ---
-        input can be either py or lmp
-        output for indices is in py since it can be used to access atoms
-        output for text is in lmp since it can be used in lammps or sth
+
+def convert_indices(indices: Union[str, List[int]], index_convention="lmp"):
+    """parse indices for reading xyz by ase, get start for counting
+    constrained indices followed by lammps convention
+    "2:4 3:8"
+    convert [1,2,3,6,7,8] to "1:3 6:8"
+    lammps convention starts from 1 and includes end
+    ---
+    input can be either py or lmp
+    output for indices is in py since it can be used to access atoms
+    output for text is in lmp since it can be used in lammps or sth
     """
     ret = []
     if isinstance(indices, str):
         # string to List[int]
         for x in indices.strip().split():
             cur_range = list(map(int, x.split(":")))
             if len(cur_range) == 1:
                 start, end = cur_range[0], cur_range[0]
             else:
                 start, end = cur_range
             if index_convention == "lmp":
-                ret.extend([i-1 for i in list(range(start,end+1))])
+                ret.extend([i - 1 for i in list(range(start, end + 1))])
             elif index_convention == "py":
-                ret.extend(list(range(start,end)))
+                ret.extend(list(range(start, end)))
             else:
                 pass
     elif isinstance(indices, list):
         # List[int] to string
         indices = sorted(indices)
         if index_convention == "lmp":
             pass
         elif index_convention == "py":
-            indices = [i+1 for i in indices]
+            indices = [i + 1 for i in indices]
         ret = []
-        #ranges = []
-        for k, g in groupby(enumerate(indices),lambda x:x[0]-x[1]):
-            group = (map(itemgetter(1),g))
-            group = list(map(int,group))
-            #ranges.append((group[0],group[-1]))
+        # ranges = []
+        for k, g in groupby(enumerate(indices), lambda x: x[0] - x[1]):
+            group = map(itemgetter(1), g)
+            group = list(map(int, group))
+            # ranges.append((group[0],group[-1]))
             if group[0] == group[-1]:
                 ret.append(str(group[0]))
             else:
-                ret.append("{}:{}".format(group[0],group[-1]))
+                ret.append("{}:{}".format(group[0], group[-1]))
         ret = " ".join(ret)
     else:
         pass
 
     return ret
 
 
 def parse_input_file(
     input_fpath: Union[str, Path],
-    write_json: bool = False # write readin dict to check if alright
+    write_json: bool = False,  # write readin dict to check if alright
 ):
     """"""
     input_dict = None
-    
+
     # - parse input type
     if isinstance(input_fpath, dict):
         input_dict = input_fpath
         json_path = Path.cwd()
     else:
         if isinstance(input_fpath, str):
             input_file = Path(input_fpath)
@@ -199,24 +211,25 @@
                 with open(input_file, "r") as fopen:
                     input_dict = yaml.safe_load(fopen)
             else:
                 ...
         except FileNotFoundError as e:
             # NOTE: There is json or yaml in the string but it is not a file though.
             input_dict = None
-    
+
     # NOTE: recursive read internal json or yaml files
     if input_dict is not None:
         for key, value in input_dict.items():
             key_dict = parse_input_file(value, write_json=False)
             if key_dict is not None:
                 input_dict[key] = key_dict
 
     if input_dict and write_json:
-        with open(json_path/"params.json", "w") as fopen:
+        with open(json_path / "params.json", "w") as fopen:
             json.dump(input_dict, fopen, indent=4)
         print("See params.json for values of all parameters...")
 
     return input_dict
 
+
 if __name__ == "__main__":
     ...
```

### Comparing `gdpx-0.0.5/src/gdpx/utils/comparision.py` & `gdpx-0.0.6/src/gdpx/utils/comparision.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.5/src/gdpx/utils/dputils/DeepPot.py` & `gdpx-0.0.6/src/gdpx/utils/dputils/DeepPot.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.5/src/gdpx/utils/dputils/acquire_dmat.py` & `gdpx-0.0.6/src/gdpx/utils/dputils/acquire_dmat.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.5/src/gdpx/utils/geometry.py` & `gdpx-0.0.6/src/gdpx/utils/geometry.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.5/src/gdpx/utils/plot_dimer.py` & `gdpx-0.0.6/src/gdpx/utils/plot_dimer.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.5/src/gdpx/utils/reduce_dataset.py` & `gdpx-0.0.6/src/gdpx/utils/reduce_dataset.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.5/src/gdpx/utils/second_reduce.py` & `gdpx-0.0.6/src/gdpx/utils/second_reduce.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.5/src/gdpx/utils/split-dataset.py` & `gdpx-0.0.6/src/gdpx/utils/split-dataset.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.5/src/gdpx/validator/__init__.py` & `gdpx-0.0.6/src/gdpx/validator/__init__.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.5/src/gdpx/validator/diffusion_coefficient.py` & `gdpx-0.0.6/src/gdpx/validator/diffusion_coefficient.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.5/src/gdpx/validator/dimer.py` & `gdpx-0.0.6/src/gdpx/validator/dimer.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,15 +26,16 @@
 
 
 class DimerValidator(AbstractValidator):
 
     def run(self, dataset, worker: DriverBasedWorker, *args, **kwargs):
         """"""
         super().run()
-        for prefix, frames in dataset["reference"]:
+        self._print(dataset["reference"])
+        for prefix, frames in dataset["reference"].items():
             self._irun(prefix, frames, None, worker)
 
         return
 
     def _irun(self, prefix: str, ref_frames: List[Atoms], pred_frames: List[Atoms], worker):
         """"""
         # - check if input frames are dimers...
@@ -48,51 +49,51 @@
         # - read reference
         ref_symbols, ref_energies, ref_forces = get_properties(ref_frames)
         nframes = len(ref_frames)
         ref_natoms = [len(a) for a in ref_frames]
 
         if pred_frames is None:
             # NOTE: use worker to calculate
-            # TODO: use cached data?
             self._print(f"Calculate reference frames {prefix} with potential...")
             cached_pred_fpath = self.directory / prefix / "pred.xyz"
             if not cached_pred_fpath.exists():
                 worker.directory = self.directory / prefix
                 worker.batchsize = nframes
 
                 worker._share_wdir = True
 
                 worker.run(ref_frames)
                 worker.inspect(resubmit=True)
                 if worker.get_number_of_running_jobs() == 0:
                     ret = worker.retrieve(
                         include_retrieved=True,
                     )
-                    pred_frames = itertools.chain(*ret)
+                    pred_frames = list(itertools.chain(*ret))
                 else:
-                    # TODO: ...
                     ...
                 write(cached_pred_fpath, pred_frames)
             else:
                 pred_frames = read(cached_pred_fpath, ":")
+        else:
+            ...
         pred_symbols, pred_energies, pred_forces = get_properties(pred_frames)
     
         # - get reaction coordinate (dimer distance here)
         ref_distances = []
         for atoms in ref_frames:
             dis = atoms.get_distance(0, 1, mic=True)
             ref_distances.append(dis)
         
         # - save data
         abs_errors = [x-y for x,y in zip(pred_energies, ref_energies)]
         rel_errors = [(x/y)*100. for x,y in zip(abs_errors,ref_energies)]
         data = np.array([ref_distances,ref_energies,pred_energies,abs_errors,rel_errors]).T
 
         np.savetxt(
-            self.directory/f"{prefix}.dat", data, 
+            self.directory/prefix/f"{prefix}.dat", data, 
             fmt="%8.4f  %12.4f  %12.4f  %12.4f  %8.4f", 
             header="{:<8s}  {:<12s}  {:<12s}  {:<12s}  {:<8s}".format(
                 "dis", "ref", "mlp", "abs", "rel [%]"
             )
         )
 
         # - plot data
@@ -109,14 +110,14 @@
         ax.set_xlabel("Dimer Distance [Å]")
 
         ax.legend()
 
         if (self.directory/f"{prefix}.png").exists():
             warnings.warn(f"Figure file {prefix} exists.", UserWarning)
         else:
-            plt.savefig(self.directory/f"{prefix}.png")
+            plt.savefig(self.directory/prefix/f"{prefix}.png")
 
         return
     
 
 if __name__ == "__main__":
-    pass
+    pass
```

### Comparing `gdpx-0.0.5/src/gdpx/validator/eos.py` & `gdpx-0.0.6/src/gdpx/validator/eos.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.5/src/gdpx/validator/mdf.py` & `gdpx-0.0.6/src/gdpx/validator/mdf.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.5/src/gdpx/validator/melting_point.py` & `gdpx-0.0.6/src/gdpx/validator/rdf.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,122 +1,205 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
+import copy
+import itertools
 import pathlib
-from typing import NoReturn, List, Union
+from typing import List
 
 import numpy as np
-import scipy as sp
-from scipy.optimize import curve_fit
-from scipy.spatial import distance_matrix
+from scipy.interpolate import make_interp_spline, BSpline
 
-from joblib import Parallel, delayed
-
-from ase import Atoms
-from ase.io import read, write
-
-import matplotlib as mpl
-mpl.use("Agg") #silent mode
-from matplotlib import pyplot as plt
+import matplotlib.pyplot as plt
 try:
     plt.style.use("presentation")
 except Exception as e:
     #print("Used default matplotlib style.")
     ...
 
-from ..utils.command import CustomTimer
+from ase import Atoms
+from ase.io import read, write
+from ase.neighborlist import NeighborList
+
 from .validator import AbstractValidator
 from .utils import wrap_traj
 from ..data.array import AtomsNDArray
-from ..builder.group import create_a_group
 
-"""Measure melting point.
+def smooth_curve(bins, points):
+    """"""
+    spl = make_interp_spline(bins, points, k=3)
+    bins = np.linspace(bins.min(), bins.max(), 300)
+    points= spl(bins)
+
+    for i, d in enumerate(points):
+        if d < 1e-6:
+            points[i] = 0.0
+
+    return bins, points
+
+def calc_rdf(
+        wdir: pathlib.Path, frames, pairs, volume: float=None, 
+        nbins: int=60, cutoff: float=6.0
+    ) -> dict:
+    """Calculate radial distribution.
+
+    Args:
+        wdir: Working directory that stores RDF results.
+        frames: A List of Atoms objects.
+        pairs: Target species pairs, for example, ["Cu-Cu", "Cu-O"].
+        volume: System volume.
+        nbins: Number of bins for histogram.
+        cutoff: Cut-off radius in Angstrom.
 
-"""
+    """
+    if not wdir.exists():
+        wdir.mkdir(parents=True)
 
-def jpcc2020_func(T, Tm, x1, x2, x3, x4):
-    """JPCC2020"""
+    # --- parse system
+    # NOTE: We assume the system volume does not change along the trajectory!
+    if volume is None:
+        volume = frames[0].get_volume()
+
+    # NOTE: the atom order should be consistent in the entire trajectory
+    #       i.e. this does not work for variable-composition system
+    chemical_symbols = frames[0].get_chemical_symbols()
+    sym_dict = {k: [] for k in set(chemical_symbols)}
+    for k, v in itertools.groupby(enumerate(chemical_symbols), key=lambda x:x[1]):
+        sym_dict[k].extend([x[0] for x in v])
+
+    pair_dict = {}
+    for pair in pairs:
+        p0, p1 = pair.split("-")
+        first_indices  = copy.deepcopy(sym_dict.get(p0, []))
+        second_indices = copy.deepcopy(sym_dict.get(p1, []))
+        assert len(first_indices) > 0, f"Cant found {p0}."
+        assert len(second_indices) > 0, f"Cant found {p1}."
+        #self._debug(f"first : {first_indices}")
+        #self._debug(f"second: {second_indices}")
 
-    return x1/(1+np.exp(-x2*(T-Tm)))+x3*T+x4
+        if p0 == p1:
+            avg_density = len(first_indices)/volume
+        else:
+            avg_density = (len(first_indices)+len(second_indices))/volume
 
-def sigmoid_func(T, Tm, x1, x2, x4):
-    """"""
+        pair_dict[pair] = [first_indices, second_indices, avg_density]
 
-    return x1/(1+np.exp(-x2*(T-Tm)))+x4
+    # -- What atoms we need access neighbour list
+    combined_first_indices = set(itertools.chain(*[v[0] for k, v in pair_dict.items()]))
 
-def get_distance_matrix(atoms: Atoms, indices=None):
-    """"""
-    if indices is None:
-        return atoms.get_all_distances(mic=False,vector=False)
-    else:
-        selected_positions = atoms.positions[indices, :]
-        return distance_matrix(selected_positions, selected_positions)
+    # ---
+    binwidth = cutoff/nbins
+    bincentres = np.linspace(binwidth/2., cutoff+binwidth/2., nbins+1)
+    left_edges = np.copy(bincentres) - binwidth/2.
+    right_edges = np.copy(bincentres) + binwidth/2.
+    bins = np.linspace(0., cutoff+binwidth, nbins+2)
+
+    # ---
+    dis_hist = {k: [] for k in pairs}
+    for atoms in frames:
+        cell = atoms.get_cell()
+        symbols = atoms.get_chemical_symbols()
+        positions = atoms.get_positions()
+        natoms = len(atoms)
+        nl = NeighborList(
+            [(cutoff+binwidth)/2.]*natoms, skin=0., sorted=False,
+            self_interaction=False, bothways=True,
+        )
+        nl.update(atoms)
+        for x in combined_first_indices:
+            nei_indices, nei_offsets = nl.get_neighbors(x)
+            #distances, sel_indices = [], []
+            distance_dict = {k: [] for k in pairs}
+            for nei_ind, nei_off in zip(nei_indices, nei_offsets):
+                #if nei_ind in second_indices:
+                curr_pair = "-".join([symbols[s] for s in [x, nei_ind]])
+                if curr_pair in pairs:
+                    dis = np.linalg.norm(
+                        positions[x] -
+                        (positions[nei_ind] + np.dot(cell, nei_off))
+                    )
+                    distance_dict[curr_pair].append(dis)
+            for k, v in distance_dict.items():
+                hist_, edges_ = np.histogram(v, bins)
+                dis_hist[k].append(hist_)
+
+    # - reformat data
+    results = {}
+    for k, v in dis_hist.items():
+        curr_dis_hist = np.array(v)
+        avg_density = pair_dict[k][2]
+
+        vshells = 4.*np.pi*left_edges**2*binwidth # NOTE: VMD likely uses this formula
+        #vshells = 4./3.*np.pi*binwidth*(3*left_edges**2+3*left_edges*binwidth+binwidth**2)
+        vshells[0] = 1. # avoid zero in division
+
+        rdf = curr_dis_hist/vshells/avg_density
+
+        rdf_avg = np.average(rdf, axis=0)
+        rdf_min = np.min(rdf, axis=0)
+        rdf_max = np.max(rdf, axis=0)
+        rdf_svar = np.sqrt(np.var(rdf, axis=0))
 
-def _icalc_local_lindemann_index(frames, group, n_jobs=1):
-    """Calculate Lindemann Index of each atom.
+        data = np.vstack((bincentres, rdf_avg, rdf_svar, rdf_min, rdf_max)).T
+        np.savetxt(
+            wdir/f"{k}.dat", data, 
+            fmt="%8.4f  %8.4f  %8.4f  %8.4f  %8.4f", 
+            header=("{:<8s}  "*5).format("r", "rdf", "svar", "min", "max")
+        )
+        results[k] = data
 
-    Returns:
-        An array with shape (natoms,)
+    return results
 
-    """
-    # NOTE: Use unwrapped positions when under PBC?
-    frames = wrap_traj(frames) # align structures
 
-    group_indices = create_a_group(frames[0], group)
-    natoms = len(group_indices)
+def plot_rdf(fig_path, data=None, ref_data=None, title="RDF"):
+    """"""
+    fig, ax = plt.subplots(nrows=1, ncols=1, figsize=(12,8))
 
-    with CustomTimer("Lindemann Index"):
-        distances = Parallel(n_jobs=n_jobs)(
-            delayed(get_distance_matrix)(atoms, group_indices) 
-            for atoms in frames
-        )
-    distances = np.array(distances)
+    plt.suptitle("Radial Distribution Function")
+    ax.set_xlabel("r [Å]")
+    ax.set_ylabel("g(r)")
 
-    dis2 = np.square(distances)
-    dis2_avg = np.average(dis2, axis=0)
+    ax.set_title(title)
 
-    dis_avg = np.average(distances, axis=0)
-    masked_dis_avg = dis_avg + np.eye(natoms) # avoid 0. in denominator
-    #print(masked_dis_avg)
+    if data is not None:
+        bincentres, rdf = data[:,0], data[:,1]
+        bincentres_, rdf_ = smooth_curve(bincentres, rdf)
+        ax.plot(bincentres_, rdf_, label="prediction")
 
-    q = np.sum( np.sqrt(dis2_avg - dis_avg**2) / masked_dis_avg, axis=1) / (natoms-1)
+    if ref_data is not None:
+        bincentres, rdf = ref_data[:,0], ref_data[:,1]
+        bincentres_, rdf_ = smooth_curve(bincentres, rdf)
+        ax.plot(bincentres_, rdf_, ls="-.", label="reference")
 
-    return q
+    plt.legend()
 
+    plt.savefig(fig_path)
 
-class MeltingPointValidator(AbstractValidator):
+    return
 
-    """Estimate the melting point from a series of MD simulations.
-    
-    For nanoparticles, the lindeman index is used. MD simulations with various 
-    initial temperatures are performed. For bulk, phase co-existence approach is used.
-    Different initial temperatures are set for solid and liquid, where the steady state is
-    found.
 
-    """
+class RdfValidator(AbstractValidator):
 
-    def __init__(self, group, run_fit: bool=True, start=0, temperatures: List[float]=None, fitting="sigmoid", directory: Union[str, pathlib.Path] = "./", *args, **kwargs):
-        """"""
-        super().__init__(directory, *args, **kwargs)
+    def __init__(self, pairs: List[str], cutoff: float=6., nbins: int=60, directory = "./", *args, **kwargs) -> None:
+        """Radial Distribution.
 
-        self.group = group
+        Args:
+            paris: A List of species pairs [Cu-Cu, ..., ...].
 
-        self.run_fit = run_fit
+        """
+        super().__init__(directory=directory, *args, **kwargs)
 
-        self.start = start
+        self.pairs = pairs
+        #assert len(self.pair), f"{self.__class__.__name__} requires two elements."
 
-        if temperatures is None:
-            temperatures = []
-        self.temperatures = temperatures
-        
-        assert fitting in ["sigmoid", "jpcc2020"], "Unsupported fitting function."
-        self.fitting = fitting
+        self.cutoff = cutoff
+        self.nbins = nbins
 
         return
-    
+
     def _process_data(self, data) -> List[List[Atoms]]:
         """"""
         data = AtomsNDArray(data)
 
         if data.ndim == 1:
             data = [data.tolist()]
         elif data.ndim == 2: # assume it is from extract_cache...
@@ -125,125 +208,88 @@
             data_ = []
             for d in data[:]: # TODO: add squeeze method?
                 data_.extend(d)
             data = data_
         else:
             raise RuntimeError(f"Invalid shape {data.shape}.")
 
-        return data
+        return data[0] # TODO: support several trajectories
 
-    def run(self, dataset: dict, worker=None, *args, **kwargs):
-        """"""
-        super().run()
+    def run(self, dataset, worker=None, *args, **kwargs):
+        """Process reference and prediction data separately.
+
+        TODO:
 
+            Support average over several trajectories.
+
+        """
+        # - get custom volume
+        volume = kwargs.get("volume", None)
+
+        # - process dataset
         self._print("process reference ->")
-        reference = dataset.get("reference")
+        reference = dataset.get("reference", None)
         if reference is not None:
-            reference = self._process_data(reference)
-            data = self._compute_melting_point(reference, prefix="ref-")
-            self._plot_figure(data[:, 1], data[:, 0], prefix="ref-", run_fit=self.run_fit)
+            ref_frames = self._process_data(reference)
+            self._debug(f"reference  nframes: {len(ref_frames)}")
+            ref_data = self._compute_rdf(
+                self.directory/"reference", 
+                ref_frames, self.pairs, self.cutoff, self.nbins,
+                volume=volume
+            )
+        else:
+            ref_data = None
 
         self._print("process prediction ->")
-        prediction = dataset.get("prediction")
+        prediction = dataset.get("prediction", None)
         if prediction is not None:
-            prediction = self._process_data(prediction)
-            data = self._compute_melting_point(prediction, prefix="pre-")
-            self._plot_figure(data[:, 1], data[:, 0], prefix="pre-", run_fit=self.run_fit)
+            pre_frames = self._process_data(prediction)
+            self._debug(f"prediction nframes: {len(pre_frames)}")
+            pre_data = self._compute_rdf(
+                self.directory/"prediction", 
+                pre_frames, self.pairs, self.cutoff, self.nbins,
+                volume=volume
+            )
+        else:
+            pre_data = None
+        
+        assert (ref_data is not None or pre_data is not None), "Neither reference nor prediction is given."
+
+        # - compare results
+        self._compare_results(ref_data, pre_data)
 
         return
     
-    def _compute_melting_point(self, trajectories, prefix=""):
+    def _compute_rdf(self, wdir, frames: List[Atoms], pairs, cutoff, nbins, volume: float=None):
         """"""
-        start, intv, end = self.start, None, None
-        temperatures = self.temperatures
-        assert len(trajectories) == len(temperatures), "Inconsitent number of trajectories and temperatures."
-
-        qnames = [str(t) for t in temperatures]
-
-        cached_data_path = self.directory / f"{prefix}qmat.txt"
-        if not cached_data_path.exists():
-            self._debug(f"nprocessors: {self.njobs}")
-            with CustomTimer("joblib", func=self._print):
-                qmat = Parallel(n_jobs=1)(
-                    delayed(_icalc_local_lindemann_index)(
-                        [a for a in curr_frames[start::] if a is not None], 
-                        self.group, n_jobs=self.njobs
-                    ) for curr_frames in trajectories
-                )
-            qmat = np.array(qmat)
-
-            np.savetxt(
-                cached_data_path, qmat.T,
-                header=(
-                    "{:>11s}"+"{:>12s}"*(len(qnames)-1)
-                ).format(*qnames),
-                fmt="%12.4f"
+        # - treat pbc
+        if any(frames[0].pbc):
+            frames = wrap_traj(frames)
+
+        if not wdir.exists():
+            data = calc_rdf(
+                wdir, frames, pairs, volume, nbins, cutoff
             )
         else:
-            qmat = np.loadtxt(cached_data_path).T
-        
-        # - postprocess data
-        t = temperatures
-        q = np.average(qmat, axis=1)
-
-        sorted_indices = [
-            x[0] for x in sorted(enumerate(temperatures), key=lambda x: x[1])
-        ]
-        self._debug(sorted_indices)
-
-        data = np.vstack(
-            (
-                [t[i] for i in sorted_indices],
-                [q[i] for i in sorted_indices]
-            )
-        ).T
-
-        np.savetxt(
-            self.directory/f"{prefix}data.txt", data,
-            header="{:>11s}  {:>12s}".format("temperature", "<q>"),
-            fmt="%12.4f"
-        )
+            data = {}
+            saved_files = list(wdir.glob("*.dat"))
+            for p in saved_files:
+                data[p.name[:-4]] = np.loadtxt(p)
 
         return data
-
-    def _plot_figure(self, q, t: List[float], prefix="", run_fit=True):
-        """"""
-        fig, ax = plt.subplots(nrows=1, ncols=1, figsize=(12,8))
-
-        # - text
-        fig.suptitle("Lindemann Index")
-
-        ax.set_xlabel("Temperature [K]")
-        ax.set_ylabel("$<q(T)>$")
-
-        # - 
-        ax.scatter(t, q)
-
-        # - fitted curve
-        if run_fit:
-            if self.fitting == "sigmoid":
-                func = sigmoid_func
-                initial_guess = [np.median(t), np.max(q), 1., np.min(q)]
-            elif self.fitting == "jpcc2020":
-                func = jpcc2020_func
-                initial_guess = [np.median(t), np.max(q), 1., 0., np.min(q)]
-            coefs, cov = curve_fit(func, t, q, initial_guess, method="dogbox")
-            self._debug(coefs)
-
-            t_ = np.arange(np.min(t), np.max(t), 2.)
-            q_ = func(t_, *coefs)
-            ax.plot(t_, q_, label=f"$T_m={coefs[0]:>8.2f}$")
-
-            ax.legend(loc="upper left")
-
-        plt.savefig(self.directory/f"{prefix}mp.png")
-
-        return
     
-    def _compare_results(self):
-        """Compare reference and prediction."""
+    def _compare_results(self, reference, prediction):
+        """"""
+        for pair in self.pairs:
+            p = prediction.get(pair, None)
+            r = reference.get(pair, None)
+            if not (p is None and r is None):
+                plot_rdf(
+                    self.directory/f"{pair}_rdf.png", 
+                    p, r, title=pair
+                )
 
         return
 
 
 if __name__ == "__main__":
     ...
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `gdpx-0.0.5/src/gdpx/validator/minima.py` & `gdpx-0.0.6/src/gdpx/validator/minima.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.5/src/gdpx/validator/rank.py` & `gdpx-0.0.6/src/gdpx/validator/rank.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.5/src/gdpx/validator/rxn.py` & `gdpx-0.0.6/src/gdpx/validator/rxn.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 import copy
+import itertools
+
+from typing import List
 
 import numpy as np
 
-import matplotlib as mpl
-mpl.use("Agg") #silent mode
-from matplotlib import pyplot as plt
+import matplotlib.colors as mcolors
+import matplotlib.pyplot as plt
 try:
     plt.style.use("presentation")
 except Exception as e:
     #print("Used default matplotlib style.")
     ...
 
 from ase import Atoms
 from ase.io import read, write
 from ase.calculators.singlepoint import SinglePointCalculator
 from ase.utils.forcecurve import fit_raw
 
-from gdpx.validator.validator import AbstractValidator
+from .validator import AbstractValidator
 
 """Validate reaction pathway using NEB.
 """
 
 def make_clean_atoms(atoms_):
     """Create a clean atoms from the input."""
     atoms = Atoms(
@@ -46,55 +48,77 @@
     #rxn_coords = compute_rxn_coords(images)
     #ax.scatter(rxn_coords, energies, label="dp")
     ff = fit_raw(energies, forces, positions, cell, pbc) # ForceFit
     #print(ff)
 
     return ff
 
-def plot_results(images, prefix, wdir):
+def plot_results(images_dict: dict, prefix, wdir):
     """"""
     fig, ax = plt.subplots(nrows=1, ncols=1, figsize=(12, 8))
     plt.suptitle("Nudged Elastic Band Calculation")
 
     ax.set_xlabel("Reaction Coordinate [Å]")
     ax.set_ylabel("Potential Energy [eV]")
 
-    ff = get_forcefit(images)
+    #print(mcolors.TABLEAU_COLORS)
+    for (name, images), c in zip(images_dict.items(), itertools.cycle(mcolors.TABLEAU_COLORS.keys())):
+        ff = get_forcefit(images)
 
-    ax.scatter(ff.path, ff.energies)
-    ax.plot(ff.fit_path, ff.fit_energies, "k--")
+        ax.scatter(ff.path, ff.energies, color=c, facecolor="w", zorder=100)
+        ax.plot(ff.fit_path, ff.fit_energies, "-", color=c, label=name)
 
     np.savetxt(wdir/f"{prefix}neb.dat", np.vstack((ff.fit_path, ff.fit_energies)).T, fmt="%8.4f")
 
-    #ax.legend()
+    ax.legend()
 
     plt.savefig(wdir/f"{prefix}neb.png")
 
     return
 
 class PathwayValidator(AbstractValidator):
 
 
     def run(self, dataset, worker = None, *args, **kwargs):
         """"""
         super().run()
 
         # - prediction
-        nebtraj = dataset.get("prediction", None)[0]
-        self._irun(images=nebtraj, prefix="pre-")
+        #nebtraj = dataset.get("prediction", None)[0]
+        nebtraj = dataset.get("prediction", None)
+        self._irun(images=nebtraj, prefix="pre-", worker=worker)
 
         return
     
-    def _irun(self, images, prefix):
+    def _irun(self, images: List[Atoms], prefix: str, worker):
         """"""
-        plot_results(images=images, prefix=prefix, wdir=self.directory)
+        self._print(f"{worker = }")
+        # TODO: Different NEB pathway
+        #       default number of images
+        #       use its own number
+        #       same number as reference
+        worker.directory = self.directory/"_xxx"
+        worker.run([images[0], images[-1]])
+        worker.inspect(resubmit=True)
+        if worker.get_number_of_running_jobs() == 0:
+            ret = worker.retrieve(
+                include_retrieved=True,
+            ) # (npairs, nbands, nimages)
+            #self._print(f"{ret = }")
+
+        images_dict = dict(
+            reference = images,
+            prediction = ret[0][-1]
+        )
+
+        plot_results(images_dict, prefix=prefix, wdir=self.directory)
 
         return
 
     def _compare_results(self, images_dict: dict):
         """"""        
 
         raise NotImplementedError()
 
 
 if __name__ == "__main__":
-    ...
+    ...
```

### Comparing `gdpx-0.0.5/src/gdpx/validator/spc.py` & `gdpx-0.0.6/src/gdpx/validator/spc.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,34 +11,32 @@
 import numpy as np
 import numpy.ma as ma
 
 from ase import Atoms
 from ase.io import read, write
 
 import matplotlib.pyplot as plt
+
 try:
     plt.style.use("presentation")
 except Exception as e:
-    #print("Used default matplotlib style.")
     ...
 
-from gdpx.validator.validator import AbstractValidator
-from gdpx.worker.drive import DriverBasedWorker
 
+from ..worker.drive import DriverBasedWorker
 from ..utils.comparision import get_properties, plot_parity, plot_distribution
+from ..utils.command import convert_indices
 
-from gdpx.utils.command import convert_indices
+from .validator import AbstractValidator
 
 
 class SinglepointValidator(AbstractValidator):
+    """Calculate energies on each structures and save them to file."""
 
-    """Calculate energies on each structures and save them to file.
-    """
-
-    def __init__(self, groups: dict=None, convergence: dict=None, *args, **kwargs):
+    def __init__(self, groups: dict = None, convergence: dict = None, *args, **kwargs):
         """Init a spc validator.
 
         Args:
             groups: Errors are estimated for given groups.
 
         """
         super().__init__(*args, **kwargs)
@@ -58,70 +56,79 @@
             nframes, rmse_ret = self._plot_comparison(prefix, frames, pred_frames)
             frame_pairs.append([frames, pred_frames])
             data.append([prefix, nframes, rmse_ret])
         self.write_data(data)
 
         # - plot specific groups
         group_params = copy.deepcopy(self.groups)
+
         def run_selection():
             selected_prefixes, selected_groups = [], []
             for k, v in group_params.items():
                 selected_prefixes.append(k)
-                selected_groups.append(
-                    convert_indices(v, index_convention="lmp")
-                )
+                selected_groups.append(convert_indices(v, index_convention="lmp"))
             self._debug(selected_groups)
             self._debug(selected_prefixes)
 
             for curr_prefix, curr_indices in zip(selected_prefixes, selected_groups):
-                curr_ref = list(itertools.chain(*[frame_pairs[i][0] for i in curr_indices]))
-                curr_pre = list(itertools.chain(*[frame_pairs[i][1] for i in curr_indices]))
-                nframes, rmse_ret = self._plot_comparison(curr_prefix, curr_ref, curr_pre)
-                self.write_data([[curr_prefix, nframes, rmse_ret]], f"{curr_prefix}-rmse.dat")
-        
+                curr_ref = list(
+                    itertools.chain(*[frame_pairs[i][0] for i in curr_indices])
+                )
+                curr_pre = list(
+                    itertools.chain(*[frame_pairs[i][1] for i in curr_indices])
+                )
+                nframes, rmse_ret = self._plot_comparison(
+                    curr_prefix, curr_ref, curr_pre
+                )
+                self.write_data(
+                    [[curr_prefix, nframes, rmse_ret]], f"{curr_prefix}-rmse.dat"
+                )
+
         if group_params is not None:
             run_selection()
 
         return
 
-    def write_data(self, data, fname: str="rmse.dat"):
+    def write_data(self, data, fname: str = "rmse.dat"):
         """"""
         # - check data file
         keys = ["ene", "frc"]
         for rmse_ret in [x[2] for x in data]:
             for k in rmse_ret.keys():
                 if k not in keys:
                     keys.append(k)
-        content_fmt = "{:<24s}  {:>8d}  " + "{:>8.4f}  {:>8.4f}  "*len(keys) + "\n"
+        content_fmt = "{:<48s}  {:>8d}  " + "{:>8.4f}  {:>8.4f}  " * len(keys) + "\n"
 
-        header_fmt = "{:<24s}  {:>8s}  " + "{:>8s}  {:>8s}  "*len(keys) + "\n"
+        header_fmt = "{:<48s}  {:>8s}  " + "{:>8s}  {:>8s}  " * len(keys) + "\n"
         header_data = ["#prefix", "nframes"]
         for k in keys:
             header_data.extend([f"{k}_rmse", f"{k}_std"])
         header = header_fmt.format(*header_data)
-        
+
         content = header
         for prefix, nframes, rmse_ret in data:
             cur_data = [prefix, nframes]
             for k in keys:
                 v = rmse_ret.get(k, None)
                 if v is None:
                     cur_data.extend([np.nan, np.nan])
                 else:
                     cur_data.extend([v["rmse"], v["std"]])
             content += content_fmt.format(*cur_data)
-        
-        with open(self.directory/fname, "w") as fopen:
+
+        with open(self.directory / fname, "w") as fopen:
             fopen.write(content)
         for l in content.split("\n"):
             self._print(l)
 
         return
 
-    def _irun(self, prefix: str, ref_frames: List[Atoms], pred_frames: List[Atoms], worker):
+    def _irun(
+        self, prefix: str, ref_frames: List[Atoms], pred_frames: List[Atoms], worker
+    ):
         """"""
         # - read structures
         nframes = len(ref_frames)
         if pred_frames is None:
             # NOTE: use worker to calculate
             # TODO: use cached data?
             self._print(f"Calculate reference frames {prefix} with potential...")
@@ -143,115 +150,119 @@
                     # TODO: ...
                     ...
                 write(cached_pred_fpath, pred_frames)
             else:
                 pred_frames = read(cached_pred_fpath, ":")
         else:
             ...
-        
+
         return pred_frames
-    
-    def _plot_comparison(self, prefix, ref_frames: List[Atoms], pred_frames: List[Atoms]):
+
+    def _plot_comparison(
+        self, prefix, ref_frames: List[Atoms], pred_frames: List[Atoms]
+    ):
         """"""
-        if not (self.directory/prefix).exists():
-            (self.directory/prefix).mkdir(parents=True)
+        if not (self.directory / prefix).exists():
+            (self.directory / prefix).mkdir(parents=True)
 
         nframes = len(ref_frames)
         ref_symbols, ref_energies, ref_forces = get_properties(ref_frames)
         ref_natoms = [len(a) for a in ref_frames]
         pred_symbols, pred_energies, pred_forces = get_properties(pred_frames)
-        
+
         # - figure
         fig, axarr = plt.subplots(
-            nrows=1, ncols=2,
-            gridspec_kw={"hspace": 0.3}, figsize=(16, 9)
+            nrows=1, ncols=2, gridspec_kw={"hspace": 0.3}, figsize=(16, 9)
         )
         axarr = axarr.flatten()
         plt.suptitle(f"{prefix} with nframes {nframes}")
 
         # -- energies
         ene_rmse = plot_parity(
             axarr[0], ref_energies, pred_energies, x_name="ene", weights=ref_natoms
         )
 
         # -- forces
         frc_rmse = plot_parity(
             axarr[1], ref_forces, pred_forces, x_name="frc", x_types=ref_symbols
         )
 
-        #if (self.directory/f"{prefix}.png").exists():
+        # if (self.directory/f"{prefix}.png").exists():
         #    warnings.warn(f"Figure file {prefix} exists.", UserWarning)
-        plt.savefig(self.directory/prefix/"rmse.png")
+        plt.savefig(self.directory / prefix / "rmse.png")
         plt.close()
 
         # plot distributions
         fig, axarr = plt.subplots(
-            nrows=1, ncols=2,
-            gridspec_kw={"hspace": 0.3}, figsize=(16, 9)
+            nrows=1, ncols=2, gridspec_kw={"hspace": 0.3}, figsize=(16, 9)
         )
         axarr = axarr.flatten()
         plt.suptitle(f"{prefix} with nframes {nframes}")
 
         plot_distribution(
             axarr[0], ref_energies, pred_energies, x_name="ene", weights=ref_natoms
         )
         plot_distribution(
             axarr[1], ref_forces, pred_forces, x_name="frc", x_types=ref_symbols
         )
 
-        plt.savefig(self.directory/prefix/"dist.png")
+        plt.savefig(self.directory / prefix / "dist.png")
         plt.close()
 
         # - save results to data file
         rmse_ret = {}
         x_rmse, x_rmse_names = ene_rmse
         for _rms, rms_name in zip(x_rmse, x_rmse_names):
             rmse_ret[rms_name] = _rms
         x_rmse, x_rmse_names = frc_rmse
         for _rms, rms_name in zip(x_rmse, x_rmse_names):
             rmse_ret[rms_name] = _rms
 
         return nframes, rmse_ret
-    
+
     def report_convergence(self, *args, **kwargs):
         """"""
         converged = True
 
-        rmse_fpath = self.directory/"rmse.dat"
+        rmse_fpath = self.directory / "rmse.dat"
         if rmse_fpath.exists():
             with open(rmse_fpath, "r") as fopen:
                 lines = fopen.readlines()
             col_names = lines[0].strip()[1:].split()[1:]
             row_names = [x.strip().split()[0] for x in lines[1:]]
-            data = np.array([x.strip().split()[1:] for x in lines[1:]], dtype=np.float32)
+            data = np.array(
+                [x.strip().split()[1:] for x in lines[1:]], dtype=np.float32
+            )
 
             # --
             convergence = copy.deepcopy(self.convergence)
             pattern = convergence.pop("pattern", None)
             if pattern is not None:
                 matched_names = [x for x in row_names if re.match(pattern, x)]
             else:
                 matched_names = row_names
-            
-            assert all([x in col_names for x in convergence.keys()]), "Unavailable keys for convergence."
+
+            assert all(
+                [x in col_names for x in convergence.keys()]
+            ), "Unavailable keys for convergence."
 
             converged = True
             for name in matched_names:
                 self._print(name)
                 iname = row_names.index(name)
                 for k, v in convergence.items():
                     ik = col_names.index(k)
                     self._print(f"{data[iname, ik]} <=? {v}")
                     if data[iname, ik] <= v:
                         converged = True
                     else:
                         converged = False
         else:
             self._print("No rmse data is available and set convergence to True.")
-        
+
         self._print(f"    >>> {converged}")
 
         return converged
 
 
 if __name__ == "__main__":
-    ...
+    ...
```

### Comparing `gdpx-0.0.5/src/gdpx/validator/surface_energy.py` & `gdpx-0.0.6/src/gdpx/validator/surface_energy.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.5/src/gdpx/validator/utils.py` & `gdpx-0.0.6/src/gdpx/validator/utils.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.5/src/gdpx/validator/validator.py` & `gdpx-0.0.6/src/gdpx/validator/validator.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.5/src/gdpx/worker/drive.py` & `gdpx-0.0.6/src/gdpx/worker/drive.py`

 * *Files 6% similar despite different names*

```diff
@@ -43,295 +43,328 @@
     Structures will be different if the atom order changes.
 
     """
     c1 = a1.get_cell(complete=True)
     c2 = a2.get_cell(complete=True)
     if np.sum(c1 - c2) >= 1e-8:
         return False
-    
+
     s1 = a1.get_chemical_symbols()
     s2 = a2.get_chemical_symbols()
     if s1 != s2:
         return False
-    
+
     p1 = a1.get_positions()
     p2 = a2.get_positions()
     if np.sum(p1 - p2) >= 1e-8:
         return False
 
     return True
 
 
 class DriverBasedWorker(AbstractWorker):
-
     """Monitor driver-based jobs.
 
     Lifetime: queued (running) -> finished -> retrieved
 
     Note:
         The database stores each unique job ID and its working directory.
 
     """
 
-    batchsize = 1 # how many structures performed in one job
+    #: How many structures performed in one job.
+    batchsize: int = 1
 
     #: Reserved keys in atoms.info by gdp.
     reserved_keys: List["str"] = ["energy", "step", "wdir"]
 
+    #: Attached driver object.
     _driver = None
 
+    #: Whether generate an independant random_seed for each candidate's driver.
+    _share_random_seed: bool = False
+
     #: Whether share calc dir for each candidate. Only for command run and spc.
     _share_wdir: bool = False
 
     #: Whether retain the info stored in atoms and add to trajectory.
     _retain_info: bool = False
 
-    def __init__(self, potter_, driver_=None, scheduler_=None, directory_=None, *args, **kwargs):
+    def __init__(
+        self, potter_, driver_=None, scheduler_=None, directory_=None, *args, **kwargs
+    ):
         """"""
         self.batchsize = kwargs.pop("batchsize", 1)
 
         assert isinstance(potter_, AbstractPotentialManager), ""
 
         self.potter = potter_
         self.driver = driver_
         self.scheduler = scheduler_
         if directory_:
             self.directory = directory_
-        
+
         self.n_jobs = config.NJOBS
 
         return
-    
+
     @property
-    def driver(self):
+    def driver(self) -> AbstractDriver:
         return self._driver
-    
+
     @driver.setter
     def driver(self, driver_):
         """"""
         assert isinstance(driver_, AbstractDriver), ""
         # TODO: check driver is consistent with potter
         self._driver = driver_
         return
 
-    def _split_groups(self, nframes: int, batchsize: int=1) -> Tuple[List[int],List[int]]:
+    def _split_groups(
+        self, nframes: int, batchsize: int = 1
+    ) -> Tuple[List[int], List[int]]:
         """Split nframes into groups."""
         # - split frames
         self._debug(f"split_groups for {nframes} nframes and {batchsize} batchsize.")
-        ngroups = int(np.floor(1.*nframes/batchsize))
+        ngroups = int(np.floor(1.0 * nframes / batchsize))
         group_indices = [0]
         for i in range(ngroups):
-            group_indices.append((i+1)*batchsize)
+            group_indices.append((i + 1) * batchsize)
         if group_indices[-1] != nframes:
             group_indices.append(nframes)
         starts, ends = group_indices[:-1], group_indices[1:]
         assert len(starts) == len(ends), "Inconsistent start and end indices..."
-        #group_indices = [f"{s}:{e}" for s, e in zip(starts,ends)]
+        # group_indices = [f"{s}:{e}" for s, e in zip(starts,ends)]
 
         return (starts, ends)
-    
+
     def _read_cached_info(self):
         # - read extra info data
         _info_data = []
-        for p in (self.directory/"_data").glob("*_info.txt"):
-            identifier = p.name[:self.UUIDLEN] # MD5
+        for p in (self.directory / "_data").glob("*_info.txt"):
+            identifier = p.name[: self.UUIDLEN]  # MD5
             with open(p, "r") as fopen:
                 for line in fopen.readlines():
                     if not line.startswith("#"):
                         _info_data.append(line.strip().split())
         _info_data = sorted(_info_data, key=lambda x: int(x[0]))
 
         return _info_data
 
     def _read_cached_xinfo(self):
         # - read extra info data
         info_keys, _info_data = [], []
-        for p in (self.directory/"_data").glob("*_xinfo.txt"):
-            identifier = p.name[:self.UUIDLEN] # MD5
+        for p in (self.directory / "_data").glob("*_xinfo.txt"):
+            identifier = p.name[: self.UUIDLEN]  # MD5
             with open(p, "r") as fopen:
                 lines = fopen.readlines()
                 info_keys = lines[0].split()[1:]
                 for line in lines:
                     if not line.startswith("#"):
                         _info_data.append(line.strip().split()[1:])
-        #_info_data = sorted(_info_data, key=lambda x: int(x[0]))
+        # _info_data = sorted(_info_data, key=lambda x: int(x[0]))
         assert info_keys, f"info_keys must not be empty."
 
         return info_keys, _info_data
-    
+
     def _preprocess(self, builder, *args, **kwargs):
         """"""
         # - get frames
         frames = []
         if isinstance(builder, StructureBuilder):
             frames = builder.run()
         else:
-            assert all(isinstance(x,Atoms) for x in frames), "Input should be a list of atoms."
+            assert all(
+                isinstance(x, Atoms) for x in frames
+            ), "Input should be a list of atoms."
             frames = builder
         prev_frames = frames
 
         # - check differences of input structures
-        processed_dpath = self.directory/"_data"
+        processed_dpath = self.directory / "_data"
         processed_dpath.mkdir(exist_ok=True)
 
         # - NOTE: atoms.info is a dict that does not maintain order
         #         thus, the saved file maybe different
         curr_frames, curr_info = copy_minimal_frames(prev_frames)
 
         # -- get MD5 of current input structures
         # NOTE: if two jobs start too close,
         #       there may be conflicts in checking structures
         with tempfile.NamedTemporaryFile(mode="w", suffix=".xyz") as tmp:
             write(tmp.name, curr_frames, columns=["symbols", "positions", "move_mask"])
 
             with open(tmp.name, "rb") as fopen:
                 curr_md5 = get_file_md5(fopen)
-        
+
         # - generate random_seeds
-        #   NOTE: no matter the job status is, they are generated to sync GRNG
-        #   TODO: worker should also have a proper RNG instead of GRNG?
-        random_seeds = config.GRNG.integers(0, 1e8, size=len(curr_frames))
-        random_seeds = [int(x) for x in random_seeds] # We need List[int]!!
-        #self._print(f"Worker random_seeds: {random_seeds}")
+        #   NOTE: no matter the job status is, they are generated to sync rng state
+        self._print(f"Driver's random_seed: {self.driver.random_seed}")
+        if not self._share_random_seed:
+            rng = np.random.Generator(np.random.PCG64(self.driver.random_seed))
+            random_seeds = rng.integers(0, 1e8, size=len(curr_frames))
+            random_seeds = [int(x) for x in random_seeds]  # We need List[int]!!
+        else:
+            random_seeds = [self.driver.random_seed] * len(curr_frames)
 
         # - check info data
         _info_data = self._read_cached_info()
 
         stored_fname = f"{curr_md5}.xyz"
-        if (processed_dpath/stored_fname).exists():
+        if (processed_dpath / stored_fname).exists():
             self._print(f"Found file with md5 {curr_md5}")
             self._info_data = _info_data
             start_confid = 0
             for x in self._info_data:
                 if x[1] == curr_md5:
                     break
                 start_confid += 1
             # NOTE: compatability
             if len(_info_data[0]) > 5:
                 random_seeds = [int(x[-1]) for x in _info_data]
             else:
-                ... # Use generated random seeds
+                ...  # Use generated random seeds
         else:
             if self._retain_info:
                 info_keys = []
                 for a in prev_frames:
                     info_keys.extend(list(a.info.keys()))
                 info_keys = sorted(set(info_keys))
-                content = f'{"#id":<12s}  ' + ("{:<24s}  "*len(info_keys)).format(*info_keys) + "\n"
+                content = (
+                    f'{"#id":<12s}  '
+                    + ("{:<24s}  " * len(info_keys)).format(*info_keys)
+                    + "\n"
+                )
                 for i, a in enumerate(prev_frames):
-                    line = f"{i:<24d}  " + "  ".join([f"{str(a.info.get(k)):<24s}" for k in info_keys]) + "\n"
+                    line = (
+                        f"{i:<24d}  "
+                        + "  ".join([f"{str(a.info.get(k)):<24s}" for k in info_keys])
+                        + "\n"
+                    )
                     content += line
-                with open(processed_dpath/f"{curr_md5}_xinfo.txt", "w") as fopen:
+                with open(processed_dpath / f"{curr_md5}_xinfo.txt", "w") as fopen:
                     fopen.write(content)
             # - save structures
             write(
-                processed_dpath/stored_fname, curr_frames, 
+                processed_dpath / stored_fname,
+                curr_frames,
                 # columns=["symbols", "positions", "momenta", "tags", "move_mask"]
             )
             # - save current atoms.info and append curr_info to _info_data
             start_confid = len(_info_data)
             content = "{:<12s}  {:<32s}  {:<12s}  {:<12s}  {:<s}  {:>24s}\n".format(
                 "#id", "MD5", "confid", "step", "wdir", "rs"
             )
-            for i, ((confid, step, wdir), rs) in enumerate(zip(curr_info, random_seeds)):
+            for i, ((confid, step, wdir), rs) in enumerate(
+                zip(curr_info, random_seeds)
+            ):
                 line = "{:<12d}  {:<32s}  {:<12d}  {:<12d}  {:<s}  {:>24d}\n".format(
-                    i+start_confid, curr_md5, confid, step, wdir, rs
+                    i + start_confid, curr_md5, confid, step, wdir, rs
                 )
                 content += line
                 _info_data.append(line.strip().split())
             self._info_data = _info_data
-            with open(processed_dpath/f"{curr_md5}_info.txt", "w") as fopen:
+            with open(processed_dpath / f"{curr_md5}_info.txt", "w") as fopen:
                 fopen.write(content)
 
         return curr_md5, curr_frames, start_confid, random_seeds
-    
-    def _prepare_batches(self, frames: List[Atoms], start_confid: int, random_seeds: List[int]):
+
+    def _prepare_batches(
+        self, frames: List[Atoms], start_confid: int, rng_states: Union[List[int], List[dict]]
+    ):
         # - check wdir
         nframes = len(frames)
         # NOTE: get a list even if it only has one structure
         # TODO: a better strategy to deal with wdirs...
         #       conflicts:
         #           merged trajectories from different drivers that all have cand0
-        wdirs = [] # [(confid,dynstep), ..., ()]
+        wdirs = []  # [(confid,dynstep), ..., ()]
         for i, atoms in enumerate(frames):
             # -- set wdir
-            wdir = "cand{}".format(int(self._info_data[i+start_confid][0]))
+            wdir = "cand{}".format(int(self._info_data[i + start_confid][0]))
             wdirs.append(wdir)
             atoms.info["wdir"] = wdir
         # - check whether each structure has a unique wdir
-        assert len(set(wdirs)) == nframes, f"Found duplicated wdirs {len(set(wdirs))} vs. {nframes}..."
+        assert (
+            len(set(wdirs)) == nframes
+        ), f"Found duplicated wdirs {len(set(wdirs))} vs. {nframes}..."
 
         # - split structures into different batches
-        #if self.scheduler.name == "local":
+        # if self.scheduler.name == "local":
         #    self._print(f"Worker overwrites batchsize to nframes {nframes} as it uses a LOCAL SCHEDULER.")
         #    batchsize_ = nframes
-        #else:
+        # else:
         #    batchsize_ = self.batchsize
         batchsize_ = self.batchsize
         starts, ends = self._split_groups(nframes, batchsize_)
 
         batches = []
         for i, (s, e) in enumerate(zip(starts, ends)):
             # - prepare structures and dirnames
-            global_indices = range(s,e)
+            global_indices = range(s, e)
             # NOTE: get a list even if it only has one structure
             cur_frames = [frames[x] for x in global_indices]
             cur_wdirs = [wdirs[x] for x in global_indices]
-            curr_rs = [random_seeds[x] for x in global_indices]
+            curr_rs = [rng_states[x] for x in global_indices]
             for x in cur_frames:
                 x.info["group"] = i
             # - check whether each structure has a unique wdir
-            assert len(set(cur_wdirs)) == len(cur_frames), f"Found duplicated wdirs {len(set(wdirs))} vs. {len(cur_frames)} for group {i}..."
+            assert len(set(cur_wdirs)) == len(
+                cur_frames
+            ), f"Found duplicated wdirs {len(set(wdirs))} vs. {len(cur_frames)} for group {i}..."
 
             # - set specific params
             batches.append([global_indices, cur_wdirs, curr_rs])
 
         return batches
-    
-    def run(self, builder=None, *args, **kwargs) -> None:
-        """Split frames into groups and submit jobs.
-        """
+
+    def run(self, builder=None, rng_states=list(), *args, **kwargs) -> None:
+        """Split frames into groups and submit jobs."""
         super().run(*args, **kwargs)
 
         # - check if the same input structures are provided
-        identifier, frames, start_confid, random_seeds = self._preprocess(builder)
-        batches = self._prepare_batches(frames, start_confid, random_seeds)
+        identifier, frames, start_confid, new_rng_states = self._preprocess(builder)
+        if rng_states: # Sometimes we need explicit rng_states as in active learning
+            new_rng_states = rng_states
+        batches = self._prepare_batches(frames, start_confid, new_rng_states)
 
         # - read metadata from file or database
         with TinyDB(
-            self.directory/f"_{self.scheduler.name}_jobs.json", indent=2
+            self.directory / f"_{self.scheduler.name}_jobs.json", indent=2
         ) as database:
             queued_jobs = database.search(Query().queued.exists())
-        queued_names = [q["gdir"][self.UUIDLEN+1:] for q in queued_jobs]
+        queued_names = [q["gdir"][self.UUIDLEN + 1 :] for q in queued_jobs]
         queued_frames = [q["md5"] for q in queued_jobs]
 
         for ig, (global_indices, wdirs, rs) in enumerate(batches):
             # - set job name
             batch_name = f"group-{ig}"
             uid = str(uuid.uuid1())
             job_name = uid + "-" + batch_name
 
             # -- whether store job info
             if self.scheduler.name != "local":
                 if batch_name in queued_names and identifier in queued_frames:
                     self._print(f"{batch_name} at {self.directory.name} was submitted.")
                     continue
-            else: # Local Scheduler
+            else:  # Local Scheduler
                 is_resubmit = kwargs.get("resubmit", False)
                 if not is_resubmit:
                     # NOTE:  Only re-run computation when resubmit is set
                     if batch_name in queued_names and identifier in queued_frames:
-                        self._print(f"{batch_name} at {self.directory.name} was submitted.")
+                        self._print(
+                            f"{batch_name} at {self.directory.name} was submitted."
+                        )
                         continue
                 else:
                     ...
 
             # - specify which group this worker is responsible for
             #   if not, then skip
-            #   Skip batch here assures the skipped batches will not recorded and 
+            #   Skip batch here assures the skipped batches will not recorded and
             #   thus will not affect their execution if several batches run at the same time.
             target_number = kwargs.get("batch", None)
             if isinstance(target_number, int):
                 if ig != target_number:
                     with CustomTimer(name="run-driver", func=self._print):
                         self._print(
                             f"{time.asctime( time.localtime(time.time()) )} {self.driver.directory.name} batch {ig} is skipped..."
@@ -340,159 +373,181 @@
                 else:
                     ...
             else:
                 ...
 
             # - run batch
             # NOTE: For command execution, if computation exits incorrectly,
-            #       it will not be recorded. The computation will resume next 
+            #       it will not be recorded. The computation will resume next
             #       time.
             self._irun(
-                batch_name, uid, identifier, 
-                frames, global_indices, wdirs, 
-                random_seeds=rs, *args, **kwargs
+                batch_name,
+                uid,
+                identifier,
+                frames,
+                global_indices,
+                wdirs,
+                rng_states=rs,
+                *args,
+                **kwargs,
             )
 
             # - save this batch job to the database
             if identifier not in queued_frames:
                 with TinyDB(
-                    self.directory/f"_{self.scheduler.name}_jobs.json", indent=2
+                    self.directory / f"_{self.scheduler.name}_jobs.json", indent=2
                 ) as database:
                     _ = database.insert(
                         dict(
-                            uid = uid,
-                            md5 = identifier,
-                            gdir=job_name, 
-                            group_number=ig, 
-                            wdir_names=wdirs, 
-                            queued=True
+                            uid=uid,
+                            md5=identifier,
+                            gdir=job_name,
+                            group_number=ig,
+                            wdir_names=wdirs,
+                            queued=True,
                         )
                     )
 
         return
-    
+
     def _irun(self, *args, **kwargs):
         """"""
 
         raise NotImplementedError("Function to run a batch of structures is undefined.")
-    
+
     def inspect(self, resubmit=False, *args, **kwargs):
         """Check if any job were finished correctly not due to time limit.
 
         Args:
             resubmit: Check whether submit unfinished jobs.
 
         """
         self._initialise(*args, **kwargs)
         self._print(f"~~~{self.__class__.__name__}+inspect")
 
         running_jobs = self._get_running_jobs()
 
         with TinyDB(
-            self.directory/f"_{self.scheduler.name}_jobs.json", indent=2
+            self.directory / f"_{self.scheduler.name}_jobs.json", indent=2
         ) as database:
             for job_name in running_jobs:
                 self._debug(f"inspect {job_name}")
                 doc_data = database.get(Query().gdir == job_name)
                 uid = doc_data["uid"]
                 identifier = doc_data["md5"]
                 batch = doc_data["group_number"]
 
-                #self.scheduler.set(**{"job-name": job_name})
+                # self.scheduler.set(**{"job-name": job_name})
                 self.scheduler.job_name = job_name
-                self.scheduler.script = self.directory/f"run-{uid}.script" 
+                self.scheduler.script = self.directory / f"run-{uid}.script"
 
                 # -- check whether the jobs if running
-                if self.scheduler.is_finished(): # if it is still in the queue
+                if self.scheduler.is_finished():  # if it is still in the queue
                     # -- valid if the task finished correctly not due to time-limit
                     is_finished = False
                     wdir_names = doc_data["wdir_names"]
                     if not self._share_wdir:
                         # - first a quick check if all wdirs exist
-                        wdir_existence = [(self.directory/x).exists() for x in wdir_names]
+                        wdir_existence = [
+                            (self.directory / x).exists() for x in wdir_names
+                        ]
                         nwdir_exists = sum(1 for x in wdir_existence if x)
                         if all(wdir_existence):
                             for x in wdir_names:
-                                curr_wdir = self.directory/x
+                                curr_wdir = self.directory / x
                                 self.driver.directory = curr_wdir
                                 if not self.driver.read_convergence():
-                                    self._print(f"Found unfinished computation at {curr_wdir.name}")
+                                    self._print(
+                                        f"Found unfinished computation at {curr_wdir.name}"
+                                    )
                                     break
                             else:
                                 is_finished = True
                         else:
                             self._print("NOT ALL wdirs exist.")
                         self._print(f"progress: {nwdir_exists}/{len(wdir_existence)}")
                     else:
-                        cache_frames = read(self.directory/"_data"/f"{identifier}_cache.xyz", ":")
+                        cache_frames = read(
+                            self.directory / "_data" / f"{identifier}_cache.xyz", ":"
+                        )
                         cache_wdirs = [a.info["wdir"] for a in cache_frames]
                         if set(wdir_names) == set(cache_wdirs):
                             is_finished = True
-                            self._print(f"Found unfinished computation at cand{len(cache_wdirs)}")
+                            self._print(
+                                f"Found unfinished computation at cand{len(cache_wdirs)}"
+                            )
                     if is_finished:
                         # -- finished correctly
                         self._print(f"{job_name} is finished...")
                         doc_data = database.get(Query().gdir == job_name)
                         database.update({"finished": True}, doc_ids=[doc_data.doc_id])
                     else:
                         # NOTE: no need to remove unfinished structures
                         #       since the driver would check it
                         # BUG: If batchsize == 1, the resbumit run many times
                         #      This is not as expected.
                         if resubmit:
                             if self.scheduler.name != "local":
                                 jobid = self.scheduler.submit()
-                                self._print(f"{job_name} is re-submitted with JOBID {jobid}.")
+                                self._print(
+                                    f"{job_name} is re-submitted with JOBID {jobid}."
+                                )
                             else:
-                                frames = read(self.directory/"_data"/f"{identifier}.xyz", ":")
+                                frames = read(
+                                    self.directory / "_data" / f"{identifier}.xyz", ":"
+                                )
                                 self.run(frames, batch=batch, resubmit=True)
                 else:
                     self._print(f"{job_name} is running...")
 
         return
-    
+
     def retrieve(
-        self, include_retrieved: bool=False, given_wdirs: List[str]=None, 
-        use_archive: bool=False, *args, **kwargs
+        self,
+        include_retrieved: bool = False,
+        given_wdirs: List[str] = None,
+        use_archive: bool = False,
+        *args,
+        **kwargs,
     ):
         """Read results from wdirs.
 
         Args:
             include_retrieved: Whether include wdirs that are already retrieved.
                               Otherwise, all finished jobs are included.
-        
+
         Returns:
             A nested List of Atoms.
 
         """
         self.inspect(*args, **kwargs)
         self._print(f"~~~{self.__class__.__name__}+retrieve")
 
         # NOTE: sometimes retrieve is used without run
-        self._info_data = self._read_cached_info() # update _info_data
+        self._info_data = self._read_cached_info()  # update _info_data
 
         # - check status and get latest results
         unretrieved_wdirs_ = []
         if not include_retrieved:
             unretrieved_jobs = self._get_unretrieved_jobs()
         else:
             unretrieved_jobs = self._get_finished_jobs()
-            
+
         unretrieved_identifiers = []
 
         with TinyDB(
-            self.directory/f"_{self.scheduler.name}_jobs.json", indent=2
+            self.directory / f"_{self.scheduler.name}_jobs.json", indent=2
         ) as database:
             for job_name in unretrieved_jobs:
                 doc_data = database.get(Query().gdir == job_name)
                 unretrieved_identifiers.append(doc_data["md5"])
                 unretrieved_wdirs_.extend(
-                    self.directory/w for w in doc_data["wdir_names"]
+                    self.directory / w for w in doc_data["wdir_names"]
                 )
-        
+
         # - get given wdirs
         unretrieved_wdirs = []
         if given_wdirs is not None:
             for wdir in unretrieved_wdirs_:
                 wdir_name = wdir.name
                 if wdir_name in given_wdirs:
                     unretrieved_wdirs.append(wdir)
@@ -500,22 +555,21 @@
             unretrieved_wdirs = unretrieved_wdirs_
 
         # - read results
         if unretrieved_wdirs:
             # - read results
             unretrieved_wdirs = [pathlib.Path(x) for x in unretrieved_wdirs]
             if not self._share_wdir:
-                archive_path = (self.directory/"cand.tgz").absolute()
-                if not archive_path.exists(): # read unarchived data
+                archive_path = (self.directory / "cand.tgz").absolute()
+                if not archive_path.exists():  # read unarchived data
                     results = self._read_results(unretrieved_wdirs, *args, **kwargs)
                 else:
                     self._print("read archived data...")
                     results = self._read_results(
-                        unretrieved_wdirs, archive_path=archive_path, 
-                        *args, **kwargs
+                        unretrieved_wdirs, archive_path=archive_path, *args, **kwargs
                     )
                 # - archive results if it has not been done
                 if use_archive and not archive_path.exists():
                     self._print("archive computation folders...")
                     with tarfile.open(archive_path, "w:gz", compresslevel=6) as tar:
                         for w in unretrieved_wdirs:
                             tar.add(w, arcname=w.name)
@@ -524,111 +578,118 @@
                 else:
                     ...
             else:
                 # TODO: deal with traj...
                 cache_frames = []
                 for identifier in unretrieved_identifiers:
                     cache_frames.extend(
-                        read(self.directory/"_data"/f"{identifier}_cache.xyz", ":")
+                        read(self.directory / "_data" / f"{identifier}_cache.xyz", ":")
                     )
                 wdir_names = [x.name for x in unretrieved_wdirs]
                 results_ = [a for a in cache_frames if a.info["wdir"] in wdir_names]
                 # - convert to a List[List[Atoms]] as non-shared run
                 results_ = [[a] for a in results_]
                 # -- re-add info
                 if self._retain_info:
                     info_keys, info_data = self._read_cached_xinfo()
-                    retained_keys = [k for k in info_keys if k not in self.reserved_keys]
+                    retained_keys = [
+                        k for k in info_keys if k not in self.reserved_keys
+                    ]
                     for i, traj_frames in enumerate(results_):
                         retained_dict = {
-                            k: v for k, v in zip(info_keys, info_data[i]) 
+                            k: v
+                            for k, v in zip(info_keys, info_data[i])
                             if k in retained_keys and v is not None
                         }
                         traj_frames[0].info.update(retained_dict)
                 results = results_
         else:
             results = []
 
         with TinyDB(
-            self.directory/f"_{self.scheduler.name}_jobs.json", indent=2
+            self.directory / f"_{self.scheduler.name}_jobs.json", indent=2
         ) as database:
             for job_name in unretrieved_jobs:
                 doc_data = database.get(Query().gdir == job_name)
                 database.update({"retrieved": True}, doc_ids=[doc_data.doc_id])
 
         return results
-    
+
     def _read_results(
-        self, unretrieved_wdirs: List[pathlib.Path], archive_path: pathlib.Path=None,
-        *args, **kwargs
-    ) -> Union[List[Atoms],List[List[Atoms]]]:
+        self,
+        unretrieved_wdirs: List[pathlib.Path],
+        archive_path: pathlib.Path = None,
+        *args,
+        **kwargs,
+    ) -> Union[List[Atoms], List[List[Atoms]]]:
         """Read results from calculation directories.
 
         Args:
             unretrieved_wdirs: Calculation directories.
 
         """
         with CustomTimer(name="read-results", func=self._print):
             # NOTE: works for vasp, ...
             results_ = Parallel(n_jobs=self.n_jobs)(
                 delayed(self._iread_results)(
-                    self.driver, wdir, info_data = self._info_data,
-                    archive_path=archive_path
-                ) 
+                    self.driver,
+                    wdir,
+                    info_data=self._info_data,
+                    archive_path=archive_path,
+                )
                 for wdir in unretrieved_wdirs
             )
 
             # -- re-add info
             if self._retain_info:
                 info_keys, info_data = self._read_cached_xinfo()
                 retained_keys = [k for k in info_keys if k not in self.reserved_keys]
                 for i, traj_frames in enumerate(results_):
                     retained_dict = {
-                        k: v for k, v in zip(info_keys, info_data[i]) 
+                        k: v
+                        for k, v in zip(info_keys, info_data[i])
                         if k in retained_keys and v is not None
                     }
                     traj_frames[0].info.update(retained_dict)
 
             # NOTE: Failed Calcution, One fail, traj fails
             results = []
             for i, traj_frames in enumerate(results_):
                 # - sift error structures
                 if traj_frames:
-                    error_info = traj_frames[0].info.get("error", None)
-                    if error_info:
-                        self._print(f"Found failed calculation at {error_info}...")
-                    else:
-                        results.append(traj_frames)
+                    results.append(traj_frames)
                 else:
-                    self._print(f"Found empty calculation at {str(self.directory)} with cand{i}...")
+                    self._print(
+                        f"Found empty calculation at {str(self.directory)} with cand{i}..."
+                    )
 
             if results:
                 self._print(
                     f"new_trajectories: {len(results)} nframes of the first: {len(results[0])}"
                 )
-            
+
         return results
-    
+
     @staticmethod
     def _iread_results(
-        driver, wdir, info_data: dict = None, archive_path: pathlib.Path=None
+        driver, wdir, info_data: dict = None, archive_path: pathlib.Path = None
     ) -> List[Atoms]:
         """Extract results from a single directory.
 
-        This must be a staticmethod as it may be pickled by joblib for parallel 
+        This must be a staticmethod as it may be pickled by joblib for parallel
         running.
 
         Args:
             wdir: Working directory.
 
         """
         driver.directory = wdir
         # NOTE: name convention, cand1112_field1112_field1112
-        confid_ = int(wdir.name.strip("cand").split("_")[0]) # internal name
-        if info_data is not None: 
+        confid_ = int(wdir.name.strip("cand").split("_")[0])  # internal name
+        if info_data is not None:
             cache_confid = int(info_data[confid_][2])
             if cache_confid >= 0:
                 confid = cache_confid
             else:
                 confid = confid_
         else:
             confid = confid_
@@ -636,120 +697,145 @@
         # NOTE: always return the entire trajectories
         traj_frames = driver.read_trajectory(
             add_step_info=True, archive_path=archive_path
         )
         for a in traj_frames:
             a.info["confid"] = confid
             a.info["wdir"] = str(wdir.name)
-        
+
         return traj_frames
-    
+
     def as_dict(self) -> dict:
         """"""
         worker_params = super().as_dict()
         worker_params["batchsize"] = self.batchsize
 
         return worker_params
 
+
 class QueueDriverBasedWorker(DriverBasedWorker):
 
     def _irun(
-        self, batch_name: str, uid: str, identifier: str, frames: List[Atoms], 
-        curr_indices: List[int], curr_wdirs: List[Union[str,pathlib.Path]], 
-        random_seeds: List[int], *args, **kwargs
+        self,
+        batch_name: str,
+        uid: str,
+        identifier: str,
+        frames: List[Atoms],
+        curr_indices: List[int],
+        curr_wdirs: List[Union[str, pathlib.Path]],
+        rng_states: Union[List[int], List[dict]],
+        *args,
+        **kwargs,
     ) -> None:
         """"""
         batch_number = int(batch_name.split("-")[-1])
 
         # - save worker file
         worker_params = {}
         worker_params["driver"] = self.driver.as_dict()
         worker_params["potential"] = self.potter.as_dict()
         worker_params["batchsize"] = self.batchsize
         worker_params["share_wdir"] = self._share_wdir
         worker_params["retain_info"] = self._retain_info
 
-        with open(self.directory/f"worker-{uid}.yaml", "w") as fopen:
+        with open(self.directory / f"worker-{uid}.yaml", "w") as fopen:
             yaml.dump(worker_params, fopen)
 
         # - save structures
-        dataset_path = str((self.directory/"_data"/f"{identifier}.xyz").resolve())
+        dataset_path = str((self.directory / "_data" / f"{identifier}.xyz").resolve())
 
         # - save scheduler file
         jobscript_fname = f"run-{uid}.script"
         self.scheduler.job_name = uid + "-" + batch_name
-        self.scheduler.script = self.directory/jobscript_fname
+        self.scheduler.script = self.directory / jobscript_fname
 
         self.scheduler.user_commands = "gdp -p {} compute {} --batch {} --spawn\n".format(
-            (self.directory/f"worker-{uid}.yaml").name, 
-            #(self.directory/structure_fname).name
-            dataset_path, batch_number
+            (self.directory / f"worker-{uid}.yaml").name,
+            # (self.directory/structure_fname).name
+            dataset_path,
+            batch_number,
         )
 
         # - TODO: check whether params for scheduler is changed
         self.scheduler.write()
         if self._submit:
             self._print(f"{self.directory.name} JOBID: {self.scheduler.submit()}")
         else:
             self._print(f"{self.directory.name} waits to submit.")
 
         return
 
-class CommandDriverBasedWorker(DriverBasedWorker):
 
+class CommandDriverBasedWorker(DriverBasedWorker):
 
     def _irun(
-        self, batch_name: str, uid: str, identifier: str, frames: List[Atoms], 
-        curr_indices: List[int], curr_wdirs: List[Union[str,pathlib.Path]], 
-        random_seeds: List[int], *args, **kwargs
+        self,
+        batch_name: str,
+        uid: str,
+        identifier: str,
+        frames: List[Atoms],
+        curr_indices: List[int],
+        curr_wdirs: List[Union[str, pathlib.Path]],
+        rng_states: Union[List[int], List[dict]],
+        *args,
+        **kwargs,
     ) -> None:
         """Run calculations directly in the command line.
 
-        Local execution supports a compact mode as structures will reuse the 
+        Local execution supports a compact mode as structures will reuse the
         calculation working directory.
 
         """
         batch_number = int(batch_name.split("-")[-1])
 
         # - get structures
         curr_frames = [frames[i] for i in curr_indices]
 
         # - run calculations
         with CustomTimer(name="run-driver", func=self._print):
             if not self._share_wdir:
-                for wdir, atoms, rs in zip(curr_wdirs, curr_frames, random_seeds):
-                    self.driver.directory = self.directory/wdir
+                for wdir, atoms, rs in zip(curr_wdirs, curr_frames, rng_states):
+                    self.driver.directory = self.directory / wdir
+                    prev_random_seed = self.driver.random_seed
                     self.driver.set_rng(seed=rs)
                     self._print(
                         f"{time.asctime( time.localtime(time.time()) )} {str(wdir)} {self.driver.directory.name} is running..."
                     )
                     self.driver.reset()
                     self.driver.run(atoms, read_exists=True, extra_info=None)
+                    self.driver.set_rng(seed=prev_random_seed)
             else:
-                cache_fpath = self.directory/"_data"/f"{identifier}_cache.xyz"
+                cache_fpath = self.directory / "_data" / f"{identifier}_cache.xyz"
                 if cache_fpath.exists():
                     cache_frames = read(cache_fpath, ":")
                     cache_wdirs = [a.info["wdir"] for a in cache_frames]
                 else:
                     cache_wdirs = []
-                temp_wdir = self.directory/"_shared"
-                for wdir, atoms, rs in zip(curr_wdirs, curr_frames, random_seeds):
+                temp_wdir = self.directory / "_shared"
+                for wdir, atoms, rs in zip(curr_wdirs, curr_frames, rng_states):
                     if wdir in cache_wdirs:
                         continue
                     if temp_wdir.exists():
                         shutil.rmtree(temp_wdir)
                     self.driver.directory = temp_wdir
                     self.driver.set_rng(seed=rs)
                     self._print(
                         f"{time.asctime( time.localtime(time.time()) )} {str(wdir)} {self.driver.directory.name} is running..."
                     )
                     self.driver.reset()
-                    new_atoms = self.driver.run(atoms, read_exists=False, extra_info=dict(wdir=wdir))
+                    new_atoms = self.driver.run(
+                        atoms, read_exists=False, extra_info=dict(wdir=wdir)
+                    )
                     # - save data
                     # TODO: There may have conflicts in write as many groups may run at the same time.
                     #       Add protection to the file.
-                    write(self.directory/"_data"/f"{identifier}_cache.xyz", new_atoms, append=True)
+                    write(
+                        self.directory / "_data" / f"{identifier}_cache.xyz",
+                        new_atoms,
+                        append=True,
+                    )
 
         return
 
+
 if __name__ == "__main__":
     ...
```

### Comparing `gdpx-0.0.5/src/gdpx/worker/explore.py` & `gdpx-0.0.6/src/gdpx/worker/explore.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.5/src/gdpx/worker/grid.py` & `gdpx-0.0.6/src/gdpx/worker/grid.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.5/src/gdpx/worker/interface.py` & `gdpx-0.0.6/src/gdpx/worker/interface.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.5/src/gdpx/worker/react.py` & `gdpx-0.0.6/src/gdpx/worker/react.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.5/src/gdpx/worker/single.py` & `gdpx-0.0.6/src/gdpx/worker/single.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,14 +40,24 @@
 
         self.potter = potter
         self.driver = driver
         self.scheduler = scheduler
 
         return
     
+    @staticmethod
+    def from_a_worker(worker) -> "SingleWorker":
+        """"""
+        single_worker = SingleWorker(
+            worker.potter, worker.driver, worker.scheduler,
+            worker.directory
+        )
+
+        return single_worker
+    
     @property
     def wdir_name(self):
         """"""
 
         return self._wdir_name
     
     @wdir_name.setter
```

### Comparing `gdpx-0.0.5/src/gdpx/worker/train.py` & `gdpx-0.0.6/src/gdpx/worker/train.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.5/src/gdpx/worker/utils.py` & `gdpx-0.0.6/src/gdpx/worker/utils.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.5/src/gdpx/worker/worker.py` & `gdpx-0.0.6/src/gdpx/worker/worker.py`

 * *Files identical despite different names*

### Comparing `gdpx-0.0.5/src/gdpx.egg-info/PKG-INFO` & `gdpx-0.0.6/src/gdpx.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gdpx
-Version: 0.0.5
+Version: 0.0.6
 Summary: Automate computational chemistry/materials sciance and machine learning interatomic potential training workflow.
 Author-email: Jiayan Xu <ahcigar@foxmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `gdpx-0.0.5/src/gdpx.egg-info/SOURCES.txt` & `gdpx-0.0.6/src/gdpx.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -60,21 +60,19 @@
 src/gdpx/comparator/graph.py
 src/gdpx/comparator/interface.py
 src/gdpx/comparator/reaction.py
 src/gdpx/comparator/singlepoint.py
 src/gdpx/computation/__init__.py
 src/gdpx/computation/asedriver.py
 src/gdpx/computation/cp2k.py
-src/gdpx/computation/dpx.py
 src/gdpx/computation/driver.py
 src/gdpx/computation/espresso.py
 src/gdpx/computation/interface.py
 src/gdpx/computation/lammps.py
 src/gdpx/computation/lasp.py
-src/gdpx/computation/plumed.py
 src/gdpx/computation/reann.py
 src/gdpx/computation/utils.py
 src/gdpx/computation/vasp.py
 src/gdpx/computation/md/md_utils.py
 src/gdpx/computation/md/nosehoover.py
 src/gdpx/core/__init__.py
 src/gdpx/core/node.py
@@ -82,82 +80,95 @@
 src/gdpx/core/placeholder.py
 src/gdpx/core/register.py
 src/gdpx/core/variable.py
 src/gdpx/core/session/__init__.py
 src/gdpx/core/session/active.py
 src/gdpx/core/session/basic.py
 src/gdpx/core/session/interface.py
+src/gdpx/core/session/session.py
 src/gdpx/core/session/utils.py
 src/gdpx/data/ClusterAndCUR.py
 src/gdpx/data/__init__.py
 src/gdpx/data/analyser.py
 src/gdpx/data/array.py
 src/gdpx/data/cleave_deviation.py
 src/gdpx/data/convert.py
 src/gdpx/data/correction.py
 src/gdpx/data/database.py
 src/gdpx/data/dataset.py
+src/gdpx/data/extatoms.py
 src/gdpx/data/extract_evolution.py
 src/gdpx/data/interface.py
 src/gdpx/data/operators.py
 src/gdpx/data/system.py
+src/gdpx/data/utils.py
 src/gdpx/describer/__init__.py
 src/gdpx/describer/describer.py
 src/gdpx/describer/interface.py
 src/gdpx/describer/soap.py
+src/gdpx/describer/spc.py
 src/gdpx/expedition/__init__.py
 src/gdpx/expedition/expedition.py
 src/gdpx/expedition/interface.py
 src/gdpx/expedition/af/afir.py
-src/gdpx/expedition/bh/bh.py
 src/gdpx/expedition/ga/engine.py
 src/gdpx/expedition/ga/population.py
-src/gdpx/expedition/mc/mc.py
-src/gdpx/expedition/mc/operators/__init__.py
-src/gdpx/expedition/mc/operators/exchange.py
-src/gdpx/expedition/mc/operators/move.py
-src/gdpx/expedition/mc/operators/operator.py
-src/gdpx/expedition/mc/operators/swap.py
+src/gdpx/expedition/monte_carlo/__init__.py
+src/gdpx/expedition/monte_carlo/basin_hopping.py
+src/gdpx/expedition/monte_carlo/monte_carlo.py
+src/gdpx/expedition/monte_carlo/operators/__init__.py
+src/gdpx/expedition/monte_carlo/operators/exchange.py
+src/gdpx/expedition/monte_carlo/operators/move.py
+src/gdpx/expedition/monte_carlo/operators/operator.py
+src/gdpx/expedition/monte_carlo/operators/react.py
+src/gdpx/expedition/monte_carlo/operators/swap.py
+src/gdpx/expedition/simulated_annealing/simulated_annealing.py
 src/gdpx/graph/__init__.py
 src/gdpx/graph/comparison.py
 src/gdpx/graph/creator.py
 src/gdpx/graph/graph_main.py
 src/gdpx/graph/molecule.py
 src/gdpx/graph/sites.py
 src/gdpx/graph/surface.py
 src/gdpx/graph/utils.py
 src/gdpx/potential/__init__.py
 src/gdpx/potential/interface.py
 src/gdpx/potential/manager.py
 src/gdpx/potential/trainer.py
+src/gdpx/potential/calculators/dummy.py
 src/gdpx/potential/calculators/mixer.py
 src/gdpx/potential/managers/__init__.py
 src/gdpx/potential/managers/bias.py
 src/gdpx/potential/managers/cp2k.py
-src/gdpx/potential/managers/deepmd.py
 src/gdpx/potential/managers/dftd3.py
 src/gdpx/potential/managers/eam.py
 src/gdpx/potential/managers/emt.py
 src/gdpx/potential/managers/espresso.py
 src/gdpx/potential/managers/grid.py
 src/gdpx/potential/managers/lasp.py
 src/gdpx/potential/managers/mace.py
 src/gdpx/potential/managers/mixer.py
 src/gdpx/potential/managers/nequip.py
-src/gdpx/potential/managers/plumed.py
 src/gdpx/potential/managers/reax.py
 src/gdpx/potential/managers/schnet.py
 src/gdpx/potential/managers/vasp.py
 src/gdpx/potential/managers/xtb.py
+src/gdpx/potential/managers/deepmd/__init__.py
+src/gdpx/potential/managers/deepmd/calculator.py
+src/gdpx/potential/managers/deepmd/convert.py
+src/gdpx/potential/managers/deepmd/deepmd.py
 src/gdpx/potential/managers/gp/__init__.py
 src/gdpx/potential/managers/gp/bench.py
 src/gdpx/potential/managers/gp/fgp.py
 src/gdpx/potential/managers/gp/gptools.py
 src/gdpx/potential/managers/gp/representation.py
 src/gdpx/potential/managers/gp/sgp.py
+src/gdpx/potential/managers/plumed/plumed.py
+src/gdpx/potential/managers/plumed/calculators/plumed.py
+src/gdpx/potential/managers/plumed/calculators/plumed2.py
 src/gdpx/potential/managers/reann/beann.py
 src/gdpx/potential/managers/reann/reann.py
 src/gdpx/potential/managers/reann/calculators/reann.py
 src/gdpx/reactor/__init__.py
 src/gdpx/reactor/interface.py
 src/gdpx/reactor/reactor.py
 src/gdpx/reactor/utils.py
@@ -194,31 +205,33 @@
 src/gdpx/selector/graph.py
 src/gdpx/selector/interface.py
 src/gdpx/selector/interval.py
 src/gdpx/selector/invariant.py
 src/gdpx/selector/locate.py
 src/gdpx/selector/property.py
 src/gdpx/selector/random.py
+src/gdpx/selector/scf.py
 src/gdpx/selector/selector.py
 src/gdpx/trainer/__init__.py
 src/gdpx/trainer/interface.py
 src/gdpx/utils/__init__.py
 src/gdpx/utils/atomUtils.py
 src/gdpx/utils/cleave_cluster.py
+src/gdpx/utils/cmdrun.py
 src/gdpx/utils/cmp_refdat.py
 src/gdpx/utils/command.py
 src/gdpx/utils/comparision.py
 src/gdpx/utils/geometry.py
 src/gdpx/utils/plot_dimer.py
 src/gdpx/utils/reduce_dataset.py
 src/gdpx/utils/second_reduce.py
 src/gdpx/utils/split-dataset.py
+src/gdpx/utils/strucopy.py
 src/gdpx/utils/dputils/DeepPot.py
 src/gdpx/utils/dputils/acquire_dmat.py
-src/gdpx/utils/dputils/dpset2xyz-all.py
 src/gdpx/validator/__init__.py
 src/gdpx/validator/diffusion_coefficient.py
 src/gdpx/validator/dimer.py
 src/gdpx/validator/eos.py
 src/gdpx/validator/interface.py
 src/gdpx/validator/mdf.py
 src/gdpx/validator/melting_point.py
```

