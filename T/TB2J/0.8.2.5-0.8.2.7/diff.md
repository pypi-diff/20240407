# Comparing `tmp/TB2J-0.8.2.5.tar.gz` & `tmp/TB2J-0.8.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TB2J-0.8.2.5.tar", last modified: Fri Apr  5 14:41:07 2024, max compression
+gzip compressed data, was "TB2J-0.8.2.7.tar", last modified: Sun Apr  7 14:52:48 2024, max compression
```

## Comparing `TB2J-0.8.2.5.tar` & `TB2J-0.8.2.7.tar`

### file list

```diff
@@ -1,90 +1,90 @@
-drwxr-xr-x   0 hexu      (1032) phythema   (500)        0 2024-04-05 14:41:07.331923 TB2J-0.8.2.5/
--rw-r--r--   0 hexu      (1032) phythema   (500)     1332 2024-02-28 11:18:04.000000 TB2J-0.8.2.5/LICENSE
--rw-r--r--   0 hexu      (1032) phythema   (500)     1256 2024-04-05 14:41:07.331923 TB2J-0.8.2.5/PKG-INFO
--rw-r--r--   0 hexu      (1032) phythema   (500)     2089 2024-03-08 15:04:05.000000 TB2J-0.8.2.5/README.md
-drwxr-xr-x   0 hexu      (1032) phythema   (500)        0 2024-04-05 14:41:07.331923 TB2J-0.8.2.5/TB2J/
--rw-r--r--   0 hexu      (1032) phythema   (500)     6980 2024-02-28 11:18:04.000000 TB2J-0.8.2.5/TB2J/Jdownfolder.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     3179 2024-02-28 11:18:04.000000 TB2J-0.8.2.5/TB2J/Jtensor.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     3595 2024-02-28 11:18:04.000000 TB2J-0.8.2.5/TB2J/Oiju.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     7332 2024-02-28 11:18:04.000000 TB2J-0.8.2.5/TB2J/Oiju_epc.py
--rw-r--r--   0 hexu      (1032) phythema   (500)       24 2024-04-05 14:40:14.000000 TB2J-0.8.2.5/TB2J/__init__.py
-drwxr-xr-x   0 hexu      (1032) phythema   (500)        0 2024-04-05 14:41:07.331923 TB2J-0.8.2.5/TB2J/abacus/
--rw-r--r--   0 hexu      (1032) phythema   (500)       56 2024-03-04 09:41:08.000000 TB2J-0.8.2.5/TB2J/abacus/__init__.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     7267 2024-03-04 09:41:08.000000 TB2J-0.8.2.5/TB2J/abacus/abacus_api.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     8492 2024-03-08 15:04:05.000000 TB2J-0.8.2.5/TB2J/abacus/abacus_wrapper.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     2973 2024-03-04 09:41:08.000000 TB2J-0.8.2.5/TB2J/abacus/gen_exchange_abacus.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     1562 2024-03-04 09:41:08.000000 TB2J-0.8.2.5/TB2J/abacus/orbital_api.py
--rw-r--r--   0 hexu      (1032) phythema   (500)    67888 2024-03-08 12:59:31.000000 TB2J-0.8.2.5/TB2J/abacus/stru_api.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     1254 2024-03-04 09:41:08.000000 TB2J-0.8.2.5/TB2J/abacus/test_read_HRSR.py
--rw-r--r--   0 hexu      (1032) phythema   (500)      785 2024-03-04 09:41:08.000000 TB2J-0.8.2.5/TB2J/abacus/test_read_stru.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     1558 2024-03-04 09:41:08.000000 TB2J-0.8.2.5/TB2J/basis.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     2891 2024-02-28 11:18:04.000000 TB2J-0.8.2.5/TB2J/citation.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     2633 2024-02-28 11:18:04.000000 TB2J-0.8.2.5/TB2J/contour.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     1514 2024-02-28 11:18:04.000000 TB2J-0.8.2.5/TB2J/density_matrix.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     3474 2024-02-28 11:18:04.000000 TB2J-0.8.2.5/TB2J/epc.py
--rw-r--r--   0 hexu      (1032) phythema   (500)    30380 2024-04-05 14:38:23.000000 TB2J-0.8.2.5/TB2J/exchange.py
--rw-r--r--   0 hexu      (1032) phythema   (500)    11350 2024-04-05 14:37:55.000000 TB2J-0.8.2.5/TB2J/exchangeCL2.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     8521 2024-02-28 11:18:04.000000 TB2J-0.8.2.5/TB2J/exchange_pert.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     8436 2024-02-28 11:18:04.000000 TB2J-0.8.2.5/TB2J/exchange_qspace.py
-drwxr-xr-x   0 hexu      (1032) phythema   (500)        0 2024-04-05 14:41:07.331923 TB2J-0.8.2.5/TB2J/external/
--rw-r--r--   0 hexu      (1032) phythema   (500)      137 2024-02-28 11:18:04.000000 TB2J-0.8.2.5/TB2J/external/__init__.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     5831 2024-02-28 11:18:04.000000 TB2J-0.8.2.5/TB2J/external/p_tqdm.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     6890 2024-02-28 11:18:04.000000 TB2J-0.8.2.5/TB2J/gpaw_wrapper.py
--rw-r--r--   0 hexu      (1032) phythema   (500)    13169 2024-02-28 11:18:04.000000 TB2J-0.8.2.5/TB2J/green.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     1603 2024-02-28 11:18:04.000000 TB2J-0.8.2.5/TB2J/greentest.py
-drwxr-xr-x   0 hexu      (1032) phythema   (500)        0 2024-04-05 14:41:07.331923 TB2J-0.8.2.5/TB2J/io_exchange/
--rw-r--r--   0 hexu      (1032) phythema   (500)       32 2024-02-28 11:09:31.000000 TB2J-0.8.2.5/TB2J/io_exchange/__init__.py
--rw-r--r--   0 hexu      (1032) phythema   (500)    19354 2024-03-27 09:14:31.000000 TB2J-0.8.2.5/TB2J/io_exchange/io_exchange.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     6739 2024-02-28 11:18:04.000000 TB2J-0.8.2.5/TB2J/io_exchange/io_multibinit.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     4173 2024-02-28 11:18:04.000000 TB2J-0.8.2.5/TB2J/io_exchange/io_tomsasd.py
--rw-r--r--   0 hexu      (1032) phythema   (500)    10547 2024-02-28 11:18:04.000000 TB2J-0.8.2.5/TB2J/io_exchange/io_txt.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     3301 2024-02-28 11:18:04.000000 TB2J-0.8.2.5/TB2J/io_exchange/io_uppasd.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     5583 2024-02-28 11:18:04.000000 TB2J-0.8.2.5/TB2J/io_exchange/io_vampire.py
--rw-r--r--   0 hexu      (1032) phythema   (500)    15265 2024-03-08 15:04:05.000000 TB2J-0.8.2.5/TB2J/io_merge.py
--rw-r--r--   0 hexu      (1032) phythema   (500)      532 2024-02-28 11:18:04.000000 TB2J-0.8.2.5/TB2J/kpoints.py
--rw-r--r--   0 hexu      (1032) phythema   (500)    15817 2024-03-18 09:10:54.000000 TB2J-0.8.2.5/TB2J/manager.py
--rw-r--r--   0 hexu      (1032) phythema   (500)      300 2024-02-28 11:18:04.000000 TB2J-0.8.2.5/TB2J/mathutils.py
--rw-r--r--   0 hexu      (1032) phythema   (500)    17721 2024-03-04 10:09:47.000000 TB2J-0.8.2.5/TB2J/myTB.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     6669 2024-02-28 11:18:04.000000 TB2J-0.8.2.5/TB2J/orbmap.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     4120 2024-02-28 11:18:04.000000 TB2J-0.8.2.5/TB2J/pauli.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     1192 2024-02-28 11:18:04.000000 TB2J-0.8.2.5/TB2J/pert.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     4104 2024-02-28 11:18:04.000000 TB2J-0.8.2.5/TB2J/plot.py
--rwxr-xr-x   0 hexu      (1032) phythema   (500)     3031 2024-02-28 11:18:04.000000 TB2J-0.8.2.5/TB2J/rotate_atoms.py
--rw-r--r--   0 hexu      (1032) phythema   (500)    14823 2024-03-18 09:10:54.000000 TB2J-0.8.2.5/TB2J/sisl_wrapper.py
-drwxr-xr-x   0 hexu      (1032) phythema   (500)        0 2024-04-05 14:41:07.331923 TB2J-0.8.2.5/TB2J/spinham/
--rw-rw-r--   0 hexu      (1032) phythema   (500)        0 2020-07-08 14:12:19.000000 TB2J-0.8.2.5/TB2J/spinham/__init__.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     2196 2024-02-28 11:18:04.000000 TB2J-0.8.2.5/TB2J/spinham/base_parser.py
--rw-r--r--   0 hexu      (1032) phythema   (500)      762 2024-02-28 11:18:04.000000 TB2J-0.8.2.5/TB2J/spinham/constants.py
--rw-r--r--   0 hexu      (1032) phythema   (500)    16607 2024-02-28 11:18:04.000000 TB2J-0.8.2.5/TB2J/spinham/hamiltonian.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     9714 2024-02-28 11:18:04.000000 TB2J-0.8.2.5/TB2J/spinham/hamiltonian_terms.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     6599 2024-02-28 11:18:04.000000 TB2J-0.8.2.5/TB2J/spinham/plot.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     4986 2024-02-28 11:18:04.000000 TB2J-0.8.2.5/TB2J/spinham/qsolver.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     2219 2024-02-28 11:18:04.000000 TB2J-0.8.2.5/TB2J/spinham/spin_api.py
--rw-r--r--   0 hexu      (1032) phythema   (500)    11033 2024-02-28 11:18:04.000000 TB2J-0.8.2.5/TB2J/spinham/spin_xml.py
--rw-r--r--   0 hexu      (1032) phythema   (500)    12217 2024-02-28 11:18:04.000000 TB2J-0.8.2.5/TB2J/spinham/supercell.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     8083 2024-02-28 11:18:04.000000 TB2J-0.8.2.5/TB2J/tensor_rotate.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     3897 2024-02-28 11:18:04.000000 TB2J-0.8.2.5/TB2J/utest.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     9880 2024-03-18 09:04:29.000000 TB2J-0.8.2.5/TB2J/utils.py
--rw-r--r--   0 hexu      (1032) phythema   (500)      337 2024-02-28 11:18:04.000000 TB2J-0.8.2.5/TB2J/versioninfo.py
-drwxr-xr-x   0 hexu      (1032) phythema   (500)        0 2024-04-05 14:41:07.331923 TB2J-0.8.2.5/TB2J/wannier/
--rw-r--r--   0 hexu      (1032) phythema   (500)       80 2024-03-04 10:09:47.000000 TB2J-0.8.2.5/TB2J/wannier/__init__.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     4620 2024-03-14 08:56:01.000000 TB2J-0.8.2.5/TB2J/wannier/w90_parser.py
--rw-r--r--   0 hexu      (1032) phythema   (500)     4610 2024-03-04 10:09:47.000000 TB2J-0.8.2.5/TB2J/wannier/w90_tb_parser.py
-drwxr-xr-x   0 hexu      (1032) phythema   (500)        0 2024-04-05 14:41:07.331923 TB2J-0.8.2.5/TB2J.egg-info/
--rw-r--r--   0 hexu      (1032) phythema   (500)     1256 2024-04-05 14:41:07.000000 TB2J-0.8.2.5/TB2J.egg-info/PKG-INFO
--rw-r--r--   0 hexu      (1032) phythema   (500)     1747 2024-04-05 14:41:07.000000 TB2J-0.8.2.5/TB2J.egg-info/SOURCES.txt
--rw-r--r--   0 hexu      (1032) phythema   (500)        1 2024-04-05 14:41:07.000000 TB2J-0.8.2.5/TB2J.egg-info/dependency_links.txt
--rw-r--r--   0 hexu      (1032) phythema   (500)       79 2024-04-05 14:41:07.000000 TB2J-0.8.2.5/TB2J.egg-info/requires.txt
--rw-r--r--   0 hexu      (1032) phythema   (500)        5 2024-04-05 14:41:07.000000 TB2J-0.8.2.5/TB2J.egg-info/top_level.txt
-drwxr-xr-x   0 hexu      (1032) phythema   (500)        0 2024-04-05 14:41:07.331923 TB2J-0.8.2.5/scripts/
--rwxr-xr-x   0 hexu      (1032) phythema   (500)     1868 2024-02-28 11:18:04.000000 TB2J-0.8.2.5/scripts/TB2J_downfold.py
--rwxr-xr-x   0 hexu      (1032) phythema   (500)     1142 2024-02-28 11:18:04.000000 TB2J-0.8.2.5/scripts/TB2J_eigen.py
--rwxr-xr-x   0 hexu      (1032) phythema   (500)     3115 2024-02-28 11:18:04.000000 TB2J-0.8.2.5/scripts/TB2J_magnon.py
--rwxr-xr-x   0 hexu      (1032) phythema   (500)      124 2024-02-28 11:18:04.000000 TB2J-0.8.2.5/scripts/TB2J_magnon_dos.py
--rwxr-xr-x   0 hexu      (1032) phythema   (500)     1636 2024-02-28 11:18:04.000000 TB2J-0.8.2.5/scripts/TB2J_merge.py
--rwxr-xr-x   0 hexu      (1032) phythema   (500)      648 2024-02-28 11:18:04.000000 TB2J-0.8.2.5/scripts/TB2J_rotate.py
--rwxr-xr-x   0 hexu      (1032) phythema   (500)     4422 2024-03-04 09:41:08.000000 TB2J-0.8.2.5/scripts/abacus2J.py
--rwxr-xr-x   0 hexu      (1032) phythema   (500)     4720 2024-02-28 11:18:04.000000 TB2J-0.8.2.5/scripts/siesta2J.py
--rwxr-xr-x   0 hexu      (1032) phythema   (500)     6534 2024-02-28 11:18:04.000000 TB2J-0.8.2.5/scripts/wann2J.py
--rw-r--r--   0 hexu      (1032) phythema   (500)       38 2024-04-05 14:41:07.331923 TB2J-0.8.2.5/setup.cfg
--rw-r--r--   0 hexu      (1032) phythema   (500)     1952 2024-04-05 14:40:20.000000 TB2J-0.8.2.5/setup.py
+drwxr-xr-x   0 hexu      (1032) phythema   (500)        0 2024-04-07 14:52:48.742868 TB2J-0.8.2.7/
+-rw-r--r--   0 hexu      (1032) phythema   (500)     1332 2024-02-28 11:18:04.000000 TB2J-0.8.2.7/LICENSE
+-rw-r--r--   0 hexu      (1032) phythema   (500)     1256 2024-04-07 14:52:48.742868 TB2J-0.8.2.7/PKG-INFO
+-rw-r--r--   0 hexu      (1032) phythema   (500)     2089 2024-03-08 15:04:05.000000 TB2J-0.8.2.7/README.md
+drwxr-xr-x   0 hexu      (1032) phythema   (500)        0 2024-04-07 14:52:48.734868 TB2J-0.8.2.7/TB2J/
+-rw-r--r--   0 hexu      (1032) phythema   (500)     6980 2024-02-28 11:18:04.000000 TB2J-0.8.2.7/TB2J/Jdownfolder.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     3179 2024-02-28 11:18:04.000000 TB2J-0.8.2.7/TB2J/Jtensor.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     3383 2024-04-07 10:46:54.000000 TB2J-0.8.2.7/TB2J/Oiju.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     6809 2024-04-07 10:46:54.000000 TB2J-0.8.2.7/TB2J/Oiju_epc.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)       24 2024-04-07 14:52:09.000000 TB2J-0.8.2.7/TB2J/__init__.py
+drwxr-xr-x   0 hexu      (1032) phythema   (500)        0 2024-04-07 14:52:48.738868 TB2J-0.8.2.7/TB2J/abacus/
+-rw-r--r--   0 hexu      (1032) phythema   (500)       56 2024-03-04 09:41:08.000000 TB2J-0.8.2.7/TB2J/abacus/__init__.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     7267 2024-03-04 09:41:08.000000 TB2J-0.8.2.7/TB2J/abacus/abacus_api.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     8492 2024-03-08 15:04:05.000000 TB2J-0.8.2.7/TB2J/abacus/abacus_wrapper.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     2973 2024-03-04 09:41:08.000000 TB2J-0.8.2.7/TB2J/abacus/gen_exchange_abacus.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     1562 2024-03-04 09:41:08.000000 TB2J-0.8.2.7/TB2J/abacus/orbital_api.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)    67888 2024-03-08 12:59:31.000000 TB2J-0.8.2.7/TB2J/abacus/stru_api.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     1254 2024-03-04 09:41:08.000000 TB2J-0.8.2.7/TB2J/abacus/test_read_HRSR.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)      785 2024-03-04 09:41:08.000000 TB2J-0.8.2.7/TB2J/abacus/test_read_stru.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     1558 2024-03-04 09:41:08.000000 TB2J-0.8.2.7/TB2J/basis.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     2891 2024-02-28 11:18:04.000000 TB2J-0.8.2.7/TB2J/citation.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     2633 2024-02-28 11:18:04.000000 TB2J-0.8.2.7/TB2J/contour.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     1514 2024-02-28 11:18:04.000000 TB2J-0.8.2.7/TB2J/density_matrix.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     3474 2024-02-28 11:18:04.000000 TB2J-0.8.2.7/TB2J/epc.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)    29570 2024-04-07 10:46:54.000000 TB2J-0.8.2.7/TB2J/exchange.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)    10985 2024-04-07 14:47:26.000000 TB2J-0.8.2.7/TB2J/exchangeCL2.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     8523 2024-04-07 10:46:54.000000 TB2J-0.8.2.7/TB2J/exchange_pert.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     8436 2024-02-28 11:18:04.000000 TB2J-0.8.2.7/TB2J/exchange_qspace.py
+drwxr-xr-x   0 hexu      (1032) phythema   (500)        0 2024-04-07 14:52:48.738868 TB2J-0.8.2.7/TB2J/external/
+-rw-r--r--   0 hexu      (1032) phythema   (500)      137 2024-02-28 11:18:04.000000 TB2J-0.8.2.7/TB2J/external/__init__.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     5831 2024-02-28 11:18:04.000000 TB2J-0.8.2.7/TB2J/external/p_tqdm.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     6890 2024-02-28 11:18:04.000000 TB2J-0.8.2.7/TB2J/gpaw_wrapper.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)    13011 2024-04-07 10:46:54.000000 TB2J-0.8.2.7/TB2J/green.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     1603 2024-02-28 11:18:04.000000 TB2J-0.8.2.7/TB2J/greentest.py
+drwxr-xr-x   0 hexu      (1032) phythema   (500)        0 2024-04-07 14:52:48.738868 TB2J-0.8.2.7/TB2J/io_exchange/
+-rw-r--r--   0 hexu      (1032) phythema   (500)       32 2024-02-28 11:09:31.000000 TB2J-0.8.2.7/TB2J/io_exchange/__init__.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)    19354 2024-03-27 09:14:31.000000 TB2J-0.8.2.7/TB2J/io_exchange/io_exchange.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     6739 2024-02-28 11:18:04.000000 TB2J-0.8.2.7/TB2J/io_exchange/io_multibinit.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     4173 2024-02-28 11:18:04.000000 TB2J-0.8.2.7/TB2J/io_exchange/io_tomsasd.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)    10547 2024-02-28 11:18:04.000000 TB2J-0.8.2.7/TB2J/io_exchange/io_txt.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     3301 2024-02-28 11:18:04.000000 TB2J-0.8.2.7/TB2J/io_exchange/io_uppasd.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     5583 2024-02-28 11:18:04.000000 TB2J-0.8.2.7/TB2J/io_exchange/io_vampire.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)    15265 2024-03-08 15:04:05.000000 TB2J-0.8.2.7/TB2J/io_merge.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)      532 2024-02-28 11:18:04.000000 TB2J-0.8.2.7/TB2J/kpoints.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)    15372 2024-04-07 10:46:54.000000 TB2J-0.8.2.7/TB2J/manager.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)      300 2024-02-28 11:18:04.000000 TB2J-0.8.2.7/TB2J/mathutils.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)    17721 2024-03-04 10:09:47.000000 TB2J-0.8.2.7/TB2J/myTB.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     6669 2024-02-28 11:18:04.000000 TB2J-0.8.2.7/TB2J/orbmap.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     4120 2024-02-28 11:18:04.000000 TB2J-0.8.2.7/TB2J/pauli.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     1192 2024-02-28 11:18:04.000000 TB2J-0.8.2.7/TB2J/pert.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     4104 2024-02-28 11:18:04.000000 TB2J-0.8.2.7/TB2J/plot.py
+-rwxr-xr-x   0 hexu      (1032) phythema   (500)     3031 2024-02-28 11:18:04.000000 TB2J-0.8.2.7/TB2J/rotate_atoms.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)    14823 2024-03-18 09:10:54.000000 TB2J-0.8.2.7/TB2J/sisl_wrapper.py
+drwxr-xr-x   0 hexu      (1032) phythema   (500)        0 2024-04-07 14:52:48.738868 TB2J-0.8.2.7/TB2J/spinham/
+-rw-rw-r--   0 hexu      (1032) phythema   (500)        0 2020-07-08 14:12:19.000000 TB2J-0.8.2.7/TB2J/spinham/__init__.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     2196 2024-02-28 11:18:04.000000 TB2J-0.8.2.7/TB2J/spinham/base_parser.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)      762 2024-02-28 11:18:04.000000 TB2J-0.8.2.7/TB2J/spinham/constants.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)    16607 2024-02-28 11:18:04.000000 TB2J-0.8.2.7/TB2J/spinham/hamiltonian.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     9714 2024-02-28 11:18:04.000000 TB2J-0.8.2.7/TB2J/spinham/hamiltonian_terms.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     6599 2024-02-28 11:18:04.000000 TB2J-0.8.2.7/TB2J/spinham/plot.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     4986 2024-02-28 11:18:04.000000 TB2J-0.8.2.7/TB2J/spinham/qsolver.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     2219 2024-02-28 11:18:04.000000 TB2J-0.8.2.7/TB2J/spinham/spin_api.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)    11033 2024-02-28 11:18:04.000000 TB2J-0.8.2.7/TB2J/spinham/spin_xml.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)    12217 2024-02-28 11:18:04.000000 TB2J-0.8.2.7/TB2J/spinham/supercell.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     8083 2024-02-28 11:18:04.000000 TB2J-0.8.2.7/TB2J/tensor_rotate.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     3897 2024-02-28 11:18:04.000000 TB2J-0.8.2.7/TB2J/utest.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     9880 2024-03-18 09:04:29.000000 TB2J-0.8.2.7/TB2J/utils.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)      337 2024-02-28 11:18:04.000000 TB2J-0.8.2.7/TB2J/versioninfo.py
+drwxr-xr-x   0 hexu      (1032) phythema   (500)        0 2024-04-07 14:52:48.738868 TB2J-0.8.2.7/TB2J/wannier/
+-rw-r--r--   0 hexu      (1032) phythema   (500)       80 2024-03-04 10:09:47.000000 TB2J-0.8.2.7/TB2J/wannier/__init__.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     4620 2024-03-14 08:56:01.000000 TB2J-0.8.2.7/TB2J/wannier/w90_parser.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)     4610 2024-03-04 10:09:47.000000 TB2J-0.8.2.7/TB2J/wannier/w90_tb_parser.py
+drwxr-xr-x   0 hexu      (1032) phythema   (500)        0 2024-04-07 14:52:48.734868 TB2J-0.8.2.7/TB2J.egg-info/
+-rw-r--r--   0 hexu      (1032) phythema   (500)     1256 2024-04-07 14:52:48.000000 TB2J-0.8.2.7/TB2J.egg-info/PKG-INFO
+-rw-r--r--   0 hexu      (1032) phythema   (500)     1747 2024-04-07 14:52:48.000000 TB2J-0.8.2.7/TB2J.egg-info/SOURCES.txt
+-rw-r--r--   0 hexu      (1032) phythema   (500)        1 2024-04-07 14:52:48.000000 TB2J-0.8.2.7/TB2J.egg-info/dependency_links.txt
+-rw-r--r--   0 hexu      (1032) phythema   (500)       79 2024-04-07 14:52:48.000000 TB2J-0.8.2.7/TB2J.egg-info/requires.txt
+-rw-r--r--   0 hexu      (1032) phythema   (500)        5 2024-04-07 14:52:48.000000 TB2J-0.8.2.7/TB2J.egg-info/top_level.txt
+drwxr-xr-x   0 hexu      (1032) phythema   (500)        0 2024-04-07 14:52:48.742868 TB2J-0.8.2.7/scripts/
+-rwxr-xr-x   0 hexu      (1032) phythema   (500)     1868 2024-02-28 11:18:04.000000 TB2J-0.8.2.7/scripts/TB2J_downfold.py
+-rwxr-xr-x   0 hexu      (1032) phythema   (500)     1142 2024-02-28 11:18:04.000000 TB2J-0.8.2.7/scripts/TB2J_eigen.py
+-rwxr-xr-x   0 hexu      (1032) phythema   (500)     3115 2024-02-28 11:18:04.000000 TB2J-0.8.2.7/scripts/TB2J_magnon.py
+-rwxr-xr-x   0 hexu      (1032) phythema   (500)      124 2024-02-28 11:18:04.000000 TB2J-0.8.2.7/scripts/TB2J_magnon_dos.py
+-rwxr-xr-x   0 hexu      (1032) phythema   (500)     1636 2024-02-28 11:18:04.000000 TB2J-0.8.2.7/scripts/TB2J_merge.py
+-rwxr-xr-x   0 hexu      (1032) phythema   (500)      648 2024-02-28 11:18:04.000000 TB2J-0.8.2.7/scripts/TB2J_rotate.py
+-rwxr-xr-x   0 hexu      (1032) phythema   (500)     4422 2024-03-04 09:41:08.000000 TB2J-0.8.2.7/scripts/abacus2J.py
+-rwxr-xr-x   0 hexu      (1032) phythema   (500)     4317 2024-04-07 10:46:54.000000 TB2J-0.8.2.7/scripts/siesta2J.py
+-rwxr-xr-x   0 hexu      (1032) phythema   (500)     5728 2024-04-07 10:46:54.000000 TB2J-0.8.2.7/scripts/wann2J.py
+-rw-r--r--   0 hexu      (1032) phythema   (500)       38 2024-04-07 14:52:48.742868 TB2J-0.8.2.7/setup.cfg
+-rw-r--r--   0 hexu      (1032) phythema   (500)     1952 2024-04-07 14:52:02.000000 TB2J-0.8.2.7/setup.py
```

### Comparing `TB2J-0.8.2.5/LICENSE` & `TB2J-0.8.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.5/PKG-INFO` & `TB2J-0.8.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TB2J
-Version: 0.8.2.5
+Version: 0.8.2.7
 Summary: TB2J: First principle to Heisenberg exchange J using tight-binding Green function method
 Home-page: UNKNOWN
 Author: Xu He
 Author-email: mailhexu@gmail.com
 License: BSD-2-clause
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `TB2J-0.8.2.5/README.md` & `TB2J-0.8.2.7/README.md`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.5/TB2J/Jdownfolder.py` & `TB2J-0.8.2.7/TB2J/Jdownfolder.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.5/TB2J/Jtensor.py` & `TB2J-0.8.2.7/TB2J/Jtensor.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.5/TB2J/Oiju.py` & `TB2J-0.8.2.7/TB2J/Oiju.py`

 * *Files 7% similar despite different names*

```diff
@@ -41,18 +41,14 @@
     min_hopping_norm=1e-6,
     max_distance=None,
     efermi=3.0,
     magnetic_elements=[],
     kmesh=[5, 5, 5],
     emin=-12.0,
     emax=0.0,
-    height=0.2,
-    nz1=50,
-    nz2=200,
-    nz3=50,
     exclude_orbs=[],
     Rmesh=[1, 1, 1],
     description="",
 ):
     atoms = read(os.path.join(path, poscar))
     basis_fname = os.path.join(path, "basisb.txt")
     if colinear:
@@ -89,18 +85,14 @@
             atoms=atoms,
             basis=basis,
             efermi=efermi,
             magnetic_elements=magnetic_elements,
             kmesh=kmesh,
             emin=emin,
             emax=emax,
-            height=height,
-            nz1=nz1,
-            nz2=nz2,
-            nz3=nz3,
             exclude_orbs=exclude_orbs,
             Rmesh=Rmesh,
             description=description,
         )
         exchange.set_dHdx(dHdx)
         exchange.run("DJ_amp%.3f" % amp)
 
@@ -119,15 +111,11 @@
         min_hopping_norm=1e-4,
         max_distance=None,
         efermi=3.95,
         magnetic_elements=["Mn"],
         kmesh=[4, 4, 4],
         emin=-12.0,
         emax=0.0,
-        height=0.1,
-        nz1=50,
-        nz2=200,
-        nz3=50,
         exclude_orbs=[],
         Rmesh=[1, 1, 1],
         description="",
     )
```

### Comparing `TB2J-0.8.2.5/TB2J/Oiju_epc.py` & `TB2J-0.8.2.7/TB2J/Oiju_epc.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,18 +15,14 @@
         atoms,
         efermi,
         basis=None,
         magnetic_elements=[],
         kmesh=[4, 4, 4],
         emin=-15,  # integration lower bound, relative to fermi energy
         emax=0.05,  # integration upper bound. Should be 0 (fermi energy). But DFT codes define Fermi energy in various ways.
-        height=0.5,  # the delta in the (i delta) in green's function to prevent divergence
-        nz1=150,  # grid from emin to emin+(i delta)
-        nz2=300,  # grid from emin +(i delta) to emax+(i delta)
-        nz3=150,  # grid from emax + (i delta) to emax
         exclude_orbs=[],  #
         Rmesh=[0, 0, 0],  # Rmesh.
         description="",
         qmesh=[2, 2, 2],
         EPCmats=None,
         WannUmats=None,
     ):
@@ -36,18 +32,14 @@
             efermi,
             basis=None,
             magnetic_elements=[],
             kmesh=[4, 4, 4],
             emin=-15,  # integration lower bound, relative to fermi energy
             emax=0.05,  # integration upper bound. Should be 0 (fermi energy).
             # But DFT codes define Fermi energy in various ways.
-            height=0.5,  # the delta in the (i delta) in green's function.
-            nz1=150,  # grid from emin to emin+(i delta)
-            nz2=300,  # grid from emin +(i delta) to emax+(i delta)
-            nz3=150,  # grid from emax + (i delta) to emax
             exclude_orbs=[],  #
             Rmesh=[0, 0, 0],  # Rmesh.
             description="",
         )
 
         # prepare EPC in electron wannier space
         self.EPCmat_up, self.EPCmat_dn = EPCmats
```

### Comparing `TB2J-0.8.2.5/TB2J/abacus/abacus_api.py` & `TB2J-0.8.2.7/TB2J/abacus/abacus_api.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.5/TB2J/abacus/abacus_wrapper.py` & `TB2J-0.8.2.7/TB2J/abacus/abacus_wrapper.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.5/TB2J/abacus/gen_exchange_abacus.py` & `TB2J-0.8.2.7/TB2J/abacus/gen_exchange_abacus.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.5/TB2J/abacus/orbital_api.py` & `TB2J-0.8.2.7/TB2J/abacus/orbital_api.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.5/TB2J/abacus/stru_api.py` & `TB2J-0.8.2.7/TB2J/abacus/stru_api.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.5/TB2J/abacus/test_read_HRSR.py` & `TB2J-0.8.2.7/TB2J/abacus/test_read_HRSR.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.5/TB2J/abacus/test_read_stru.py` & `TB2J-0.8.2.7/TB2J/abacus/test_read_stru.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.5/TB2J/basis.py` & `TB2J-0.8.2.7/TB2J/basis.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.5/TB2J/citation.py` & `TB2J-0.8.2.7/TB2J/citation.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.5/TB2J/contour.py` & `TB2J-0.8.2.7/TB2J/contour.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.5/TB2J/density_matrix.py` & `TB2J-0.8.2.7/TB2J/density_matrix.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.5/TB2J/epc.py` & `TB2J-0.8.2.7/TB2J/epc.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.5/TB2J/exchange.py` & `TB2J-0.8.2.7/TB2J/exchange.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,38 +22,28 @@
         include_orbs={},
         kmesh=[4, 4, 4],
         emin=-15,  # integration lower bound, relative to fermi energy
         # integration upper bound. Should be 0 (fermi energy). But DFT codes define Fermi energy in various ways.
         emax=0.05,
         nz=100,
         # the delta in the (i delta) in green's function to prevent divergence
-        height=0.5,
-        nz1=150,  # grid from emin to emin+(i delta)
-        nz2=300,  # grid from emin +(i delta) to emax+(i delta)
-        nz3=150,  # grid from emax + (i delta) to emax
         exclude_orbs=[],  #
         ne=None,  # number of electrons in Wannier function.
         Rcut=None,  # Rcut.
         use_cache=False,
         np=1,
         description="",
         write_density_matrix=False,
         orb_decomposition=False,
         output_path="TB2J_results",
     ):
         self.efermi = efermi
         self.emin = emin
         self.emax = emax
         self.nz = nz
-        self.height = height
-        self.nz1 = nz1
-        self.nz2 = nz2
-        self.nz3 = nz3
-        if nz is None:
-            self.nz = nz1 + nz2 + nz3
         self.Rcut = Rcut
         self.basis = basis
         self.magnetic_elements = magnetic_elements
         self.include_orbs = include_orbs
 
         self.exclude_orbs = exclude_orbs
         self.ne = ne
@@ -77,18 +67,14 @@
         include_orbs={},
         kmesh=[4, 4, 4],
         emin=-15,  # integration lower bound, relative to fermi energy
         # integration upper bound. Should be 0 (fermi energy). But DFT codes define Fermi energy in various ways.
         emax=0.05,
         nz=100,
         # the delta in the (i delta) in green's function to prevent divergence
-        height=0.5,
-        nz1=150,  # grid from emin to emin+(i delta)
-        nz2=300,  # grid from emin +(i delta) to emax+(i delta)
-        nz3=150,  # grid from emax + (i delta) to emax
         exclude_orbs=[],  #
         ne=None,  # number of electrons in Wannier function.
         Rcut=None,  # Rcut.
         use_cache=False,
         np=1,
         description="",
         write_density_matrix=False,
@@ -101,18 +87,14 @@
             basis=basis,
             magnetic_elements=magnetic_elements,
             include_orbs=include_orbs,
             kmesh=kmesh,
             emin=emin,
             emax=emax,
             nz=nz,
-            height=height,
-            nz1=nz1,
-            nz2=nz2,
-            nz3=nz3,
             exclude_orbs=exclude_orbs,
             ne=ne,
             Rcut=Rcut,
             use_cache=use_cache,
             np=np,
             description=description,
             write_density_matrix=write_density_matrix,
@@ -160,19 +142,19 @@
     def _prepare_elist(self, method="legendre"):
         """
         prepare list of energy for integration.
         The path has three segments:
          emin --1-> emin + 1j*height --2-> emax+1j*height --3-> emax
         """
         self.contour = Contour(self.emin, self.emax)
-        if method.lower() == "rectangle":
-            self.contour.build_path_rectangle(
-                height=self.height, nz1=self.nz1, nz2=self.nz2, nz3=self.nz3
-            )
-        elif method.lower() == "semicircle":
+        # if method.lower() == "rectangle":
+        #    self.contour.build_path_rectangle(
+        #        height=self.height, nz1=self.nz1, nz2=self.nz2, nz3=self.nz3
+        #    )
+        if method.lower() == "semicircle":
             self.contour.build_path_semicircle(npoints=self.nz, endpoint=True)
         elif method.lower() == "legendre":
             self.contour.build_path_legendre(npoints=self.nz, endpoint=True)
         else:
             raise ValueError(f"The path cannot be of type {method}.")
 
     def _prepare_Rlist(self):
@@ -358,15 +340,16 @@
             self.kmesh,
             self.efermi,
             use_cache=self._use_cache,
             nproc=self.np,
         )
         self.norb = self.G.norb
         self.nbasis = self.G.nbasis
-        self.rho = np.zeros((self.nbasis, self.nbasis), dtype=complex)
+        # self.rho = np.zeros((self.nbasis, self.nbasis), dtype=complex)
+        self.rho = self.G.get_density_matrix().real
         self.A_ijR_list = defaultdict(lambda: [])
         self.A_ijR = defaultdict(lambda: np.zeros((4, 4), dtype=complex))
         self.A_ijR_orb = dict()
         self.HR0 = self.G.H0
         self._is_collinear = False
         self.Pdict = {}
         if self.write_density_matrix:
@@ -591,45 +574,45 @@
                 Jprime = np.imag(val[0, 0] - val[3, 3]) - 2 * np.sign(
                     np.dot(Si, Sj)
                 ) * np.imag(val[3, 3])
                 # Jprime = np.imag(val[0, 0] - 3*val[3, 3])
                 B = np.imag(val[3, 3])
                 self.B[keyspin] = Jprime, B
 
-    def get_N_e(self, GR, de):
-        """
-        calcualte density matrix for all R,i, j
-        """
-        self.N = defaultdict(lambda: 0.0)
-        for R, G in GR.items():
-            self.N[R] += -1.0 / np.pi * np.imag(G * de)
+    # def get_N_e(self, GR, de):
+    #    """
+    #    calcualte density matrix for all R,i, j
+    #    """
+    #    self.N = defaultdict(lambda: 0.0)
+    #    for R, G in GR.items():
+    #        self.N[R] += -1.0 / np.pi * np.imag(G * de)
+
+    # def get_rho_e(self, rhoR):
+    #    """add component to density matrix from a green's function
+    #    :param GR: Green's funciton in real space.
+    #    """
+    #    return -1.0 / np.pi * rhoR[0, 0, 0]
 
-    def get_rho_e(self, rhoR):
-        """add component to density matrix from a green's function
-        :param GR: Green's funciton in real space.
-        """
-        return -1.0 / np.pi * rhoR[0, 0, 0]
-
-    def get_total_charges(self):
-        return np.sum(np.imag(np.diag(self.rho)))
+    # def get_total_charges(self):
+    #    return np.sum(np.imag(np.diag(self.rho)))
 
     def get_rho_atom(self):
         """
         calculate charge and spin for each atom.
         """
         rho = {}
         self.charges = np.zeros(len(self.atoms), dtype=float)
         self.spinat = np.zeros((len(self.atoms), 3), dtype=float)
         for iatom in self.orb_dict:
             iorb = self.iorb(iatom)
             tmp = self.rho[np.ix_(iorb, iorb)]
             # *2 because there is a 1/2 in the paui_block_all function
-            rho[iatom] = np.array([np.trace(x) * 2 for x in pauli_block_all(tmp)])
-            self.charges[iatom] = np.imag(rho[iatom][0])
-            self.spinat[iatom, :] = np.imag(rho[iatom][1:])
+            rho[iatom] = np.array([np.trace(x) * 2 for x in pauli_block_all(tmp)]).real
+            self.charges[iatom] = rho[iatom][0]
+            self.spinat[iatom, :] = rho[iatom][1:]
         self.rho_dict = rho
         return self.rho_dict
 
     def calculate_DMI_NJT(self):
         """
         calculate exchange and DMI with the
         D(i,j) =
@@ -672,38 +655,38 @@
                     jspin = self.ispin(jatom)
                     Ddict_NJT[(R, ispin, jspin)] = D
                     Jdict_NJT[(R, ispin, jspin)] = J
         self.Jdict_NJT = Jdict_NJT
         self.Ddict_NJT = Ddict_NJT
         return Ddict_NJT
 
-    def integrate(self, rhoRs, AijRs, AijRs_orb=None, method="simpson"):
+    def integrate(self, AijRs, AijRs_orb=None, method="simpson"):
         """
         AijRs: a list of AijR,
         wherer AijR: array of ((nR, n, n, 4,4), dtype=complex)
         """
         if method == "trapezoidal":
             integrate = trapezoidal_nonuniform
         elif method == "simpson":
             integrate = simpson_nonuniform
 
-        self.rho = integrate(self.contour.path, rhoRs)
+        # self.rho = integrate(self.contour.path, rhoRs)
         for iR, R in enumerate(self.R_ijatom_dict):
             for iatom, jatom in self.R_ijatom_dict[R]:
                 f = AijRs[(R, iatom, jatom)]
                 self.A_ijR[(R, iatom, jatom)] = integrate(self.contour.path, f)
                 if self.orb_decomposition:
                     self.A_ijR_orb[(R, iatom, jatom)] = integrate(
                         self.contour.path, AijRs_orb[(R, iatom, jatom)]
                     )
 
-    def get_AijR_rhoR(self, e):
-        GR, rhoR = self.G.get_GR(self.short_Rlist, energy=e, get_rho=True)
+    def get_AijR(self, e):
+        GR = self.G.get_GR(self.short_Rlist, energy=e, get_rho=False)
         AijR, AijR_orb = self.get_all_A(GR)
-        return AijR, AijR_orb, self.get_rho_e(rhoR)
+        return AijR, AijR_orb
 
     def save_AijR(self, AijRs, fname):
         result = dict(path=self.contour.path, AijRs=AijRs)
         with open(fname, "wb") as myfile:
             pickle.dump(result, myfile)
 
     def validate(self):
@@ -713,28 +696,25 @@
 
     def calculate_all(self):
         """
         The top level.
         """
         print("Green's function Calculation started.")
 
-        rhoRs = []
         AijRs = {}
 
         AijRs_orb = {}
 
         self.validate()
 
         npole = len(self.contour.path)
         if self.np > 1:
-            # executor = ProcessPool(nodes=self.np)
-            # results = executor.map(self.get_AijR_rhoR, self.contour.path)
-            results = p_map(self.get_AijR_rhoR, self.contour.path, num_cpus=self.np)
+            results = p_map(self.get_AijR, self.contour.path, num_cpus=self.np)
         else:
-            results = map(self.get_AijR_rhoR, tqdm(self.contour.path, total=npole))
+            results = map(self.get_AijR, tqdm(self.contour.path, total=npole))
 
         for i, result in enumerate(results):
             for iR, R in enumerate(self.R_ijatom_dict):
                 for iatom, jatom in self.R_ijatom_dict[R]:
                     if (R, iatom, jatom) in AijRs:
                         AijRs[(R, iatom, jatom)].append(result[0][R, iatom, jatom])
                         if self.orb_decomposition:
@@ -746,24 +726,22 @@
                         AijRs[(R, iatom, jatom)] = []
                         AijRs[(R, iatom, jatom)].append(result[0][R, iatom, jatom])
                         if self.orb_decomposition:
                             AijRs_orb[(R, iatom, jatom)] = []
                             AijRs_orb[(R, iatom, jatom)].append(
                                 result[1][R, iatom, jatom]
                             )
-            rhoRs.append(result[2])
         if self.np > 1:
             # executor.close()
             # executor.join()
             # executor.clear()
             pass
 
         # self.save_AijRs(AijRs)
-        self.integrate(rhoRs, AijRs, AijRs_orb)
-
+        self.integrate(AijRs, AijRs_orb)
         self.get_rho_atom()
         self.A_to_Jtensor()
         self.A_to_Jtensor_orb()
 
     def _prepare_index_spin(self):
         # index_spin: index in spin hamiltonian of atom. starts from 1. -1 means not considered.
         ind_matoms = []
```

### Comparing `TB2J-0.8.2.5/TB2J/exchangeCL2.py` & `TB2J-0.8.2.7/TB2J/exchangeCL2.py`

 * *Files 7% similar despite different names*

```diff
@@ -38,18 +38,18 @@
                 Rlist=self.Rlist, fname=os.path.join(self.output_path, "rho_up.pickle")
             )
             self.Gdn.write_rho_R(
                 Rlist=self.Rlist, fname=os.path.join(self.output_path, "rho_dn.pickle")
             )
         self.norb = self.Gup.norb
         self.nbasis = self.Gup.nbasis + self.Gdn.nbasis
-        self.rho_up_list = []
-        self.rho_dn_list = []
-        self.rho_up = np.zeros((self.norb, self.norb), dtype=float)
-        self.rho_dn = np.zeros((self.norb, self.norb), dtype=float)
+        # self.rho_up_list = []
+        # self.rho_dn_list = []
+        self.rho_up = self.Gup.get_density_matrix()
+        self.rho_dn = self.Gdn.get_density_matrix()
         self.Jorb_list = defaultdict(lambda: [])
         self.JJ_list = defaultdict(lambda: [])
         self.JJ = defaultdict(lambda: 0.0j)
         self.Jorb = defaultdict(lambda: 0.0j)
         self.HR0_up = self.Gup.H0
         self.HR0_dn = self.Gdn.H0
         self.Delta = self.HR0_up - self.HR0_dn
@@ -221,49 +221,44 @@
         #    shutil.rmtree(path)
 
     def integrate(self, method="simpson"):
         if method == "trapezoidal":
             integrate = trapezoidal_nonuniform
         elif method == "simpson":
             integrate = simpson_nonuniform
-        self.rho_up = np.imag(integrate(self.contour.path, self.rho_up_list))
-        self.rho_dn = np.imag(integrate(self.contour.path, self.rho_dn_list))
         for R, ijpairs in self.R_ijatom_dict.items():
             for iatom, jatom in ijpairs:
                 self.Jorb[(R, iatom, jatom)] = integrate(
                     self.contour.path, self.Jorb_list[(R, iatom, jatom)]
                 )
                 self.JJ[(R, iatom, jatom)] = integrate(
                     self.contour.path, self.JJ_list[(R, iatom, jatom)]
                 )
 
-    def get_AijR_rhoR(self, e):
-        GR_up, rho_up = self.Gup.get_GR(self.short_Rlist, energy=e, get_rho=True)
-        GR_dn, rho_dn = self.Gdn.get_GR(self.short_Rlist, energy=e, get_rho=True)
-        rup, rdn = self.get_rho_e(rho_up, rho_dn)
+    def get_AijR(self, e):
+        GR_up = self.Gup.get_GR(self.short_Rlist, energy=e, get_rho=False)
+        GR_dn = self.Gdn.get_GR(self.short_Rlist, energy=e, get_rho=False)
         Jorb_list, JJ_list = self.get_all_A(GR_up, GR_dn)
-        return rup, rdn, Jorb_list, JJ_list
+        return Jorb_list, JJ_list
 
     def calculate_all(self):
         """
         The top level.
         """
         print("Green's function Calculation started.")
 
         npole = len(self.contour.path)
         if self.np == 1:
-            results = map(self.get_AijR_rhoR, tqdm(self.contour.path, total=npole))
+            results = map(self.get_AijR, tqdm(self.contour.path, total=npole))
         else:
             # pool = ProcessPool(nodes=self.np)
             # results = pool.map(self.get_AijR_rhoR ,self.contour.path)
-            results = p_map(self.get_AijR_rhoR, self.contour.path, num_cpus=self.np)
+            results = p_map(self.get_AijR, self.contour.path, num_cpus=self.np)
         for i, result in enumerate(results):
-            rup, rdn, Jorb_list, JJ_list = result
-            self.rho_up_list.append(rup)
-            self.rho_dn_list.append(rdn)
+            Jorb_list, JJ_list = result
             for iR, R in enumerate(self.R_ijatom_dict):
                 for iatom, jatom in self.R_ijatom_dict[R]:
                     key = (R, iatom, jatom)
                     self.Jorb_list[key].append(Jorb_list[key])
                     self.JJ_list[key].append(JJ_list[key])
         if self.np > 1:
             pass
```

### Comparing `TB2J-0.8.2.5/TB2J/exchange_pert.py` & `TB2J-0.8.2.7/TB2J/exchange_pert.py`

 * *Files 0% similar despite different names*

```diff
@@ -190,15 +190,15 @@
         # bar = progressbar.ProgressBar(maxval=self.contour.npoints, widgets=widgets)
         # bar.start()
         for ie in range(self.contour.npoints):
             # bar.update(ie)
             e = self.contour.elist[ie]
             de = self.contour.de[ie]
             GR, dGdx = self.G.get_GR_and_dGRdx(self.Rlist, energy=e, dHdx=self.dHdx)
-            self.get_rho_e(GR, de)
+            # self.get_rho_e(GR, de)
             self.get_all_A(GR, dGdx, de)
             if self.calc_NJt:
                 self.get_N_e(GR, de)
 
         self.get_rho_atom()
         self.A_to_Jtensor()
         if self.calc_NJt:
```

### Comparing `TB2J-0.8.2.5/TB2J/exchange_qspace.py` & `TB2J-0.8.2.7/TB2J/exchange_qspace.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.5/TB2J/external/p_tqdm.py` & `TB2J-0.8.2.7/TB2J/external/p_tqdm.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.5/TB2J/gpaw_wrapper.py` & `TB2J-0.8.2.7/TB2J/gpaw_wrapper.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.5/TB2J/green.py` & `TB2J-0.8.2.7/TB2J/green.py`

 * *Files 1% similar despite different names*

```diff
@@ -234,17 +234,14 @@
         return rho
 
     def get_rho_R(self, Rlist):
         nR = len(Rlist)
         rho_R = np.zeros((nR, self.nbasis, self.nbasis), dtype=complex)
         for ik, kpt in enumerate(self.kpts):
             evec = self.get_evecs(ik)
-            # rhok=(evec * fermi(self.evals[ik], self.efermi)
-            #        ) @ evec.T.conj()
-            # print(fermi(self.evals[ik] , self.efermi))
             rhok = np.einsum(
                 "ib,b, bj-> ij", evec, fermi(self.evals[ik], self.efermi), evec.conj().T
             )
             for iR, R in enumerate(Rlist):
                 rho_R[iR] += rhok * np.exp(self.k2Rfactor * kpt @ R) * self.kweights[ik]
         return rho_R
```

### Comparing `TB2J-0.8.2.5/TB2J/greentest.py` & `TB2J-0.8.2.7/TB2J/greentest.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.5/TB2J/io_exchange/io_exchange.py` & `TB2J-0.8.2.7/TB2J/io_exchange/io_exchange.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.5/TB2J/io_exchange/io_multibinit.py` & `TB2J-0.8.2.7/TB2J/io_exchange/io_multibinit.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.5/TB2J/io_exchange/io_tomsasd.py` & `TB2J-0.8.2.7/TB2J/io_exchange/io_tomsasd.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.5/TB2J/io_exchange/io_txt.py` & `TB2J-0.8.2.7/TB2J/io_exchange/io_txt.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.5/TB2J/io_exchange/io_uppasd.py` & `TB2J-0.8.2.7/TB2J/io_exchange/io_uppasd.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.5/TB2J/io_exchange/io_vampire.py` & `TB2J-0.8.2.7/TB2J/io_exchange/io_vampire.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.5/TB2J/io_merge.py` & `TB2J-0.8.2.7/TB2J/io_merge.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.5/TB2J/kpoints.py` & `TB2J-0.8.2.7/TB2J/kpoints.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.5/TB2J/manager.py` & `TB2J-0.8.2.7/TB2J/manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,18 +23,14 @@
     max_distance=None,
     efermi=0,
     magnetic_elements=[],
     kmesh=[4, 4, 4],
     emin=-12.0,
     emax=0.0,
     nz=100,
-    height=0.2,
-    nz1=50,
-    nz2=200,
-    nz3=50,
     exclude_orbs=[],
     Rcut=None,
     ne=None,
     use_cache=False,
     np=1,
     output_path="TB2J_results",
     wannier_type="wannier90",
@@ -109,18 +105,14 @@
                 basis=basis,
                 efermi=efermi,
                 magnetic_elements=magnetic_elements,
                 kmesh=kmesh,
                 emin=emin,
                 emax=emax,
                 nz=nz,
-                height=height,
-                nz1=nz1,
-                nz2=nz2,
-                nz3=nz3,
                 exclude_orbs=exclude_orbs,
                 Rcut=Rcut,
                 ne=ne,
                 np=np,
                 use_cache=use_cache,
                 output_path=output_path,
                 write_density_matrix=write_density_matrix,
@@ -133,18 +125,14 @@
                 basis=basis,
                 efermi=efermi,
                 magnetic_elements=magnetic_elements,
                 kmesh=kmesh,
                 emin=emin,
                 emax=emax,
                 nz=nz,
-                height=height,
-                nz1=nz1,
-                nz2=nz2,
-                nz3=nz3,
                 exclude_orbs=exclude_orbs,
                 Rcut=Rcut,
                 ne=ne,
                 np=np,
                 use_cache=use_cache,
                 output_path=output_path,
                 write_density_matrix=write_density_matrix,
@@ -181,18 +169,14 @@
             basis=basis,
             efermi=efermi,
             magnetic_elements=magnetic_elements,
             kmesh=kmesh,
             emin=emin,
             emax=emax,
             nz=nz,
-            height=height,
-            nz1=nz1,
-            nz2=nz2,
-            nz3=nz3,
             exclude_orbs=exclude_orbs,
             Rcut=Rcut,
             ne=ne,
             np=np,
             use_cache=use_cache,
             output_path=output_path,
             write_density_matrix=write_density_matrix,
@@ -233,18 +217,14 @@
             basis=basis,
             efermi=efermi,
             magnetic_elements=magnetic_elements,
             kmesh=kmesh,
             emin=emin,
             emax=emax,
             nz=nz,
-            height=height,
-            nz1=nz1,
-            nz2=nz2,
-            nz3=nz3,
             exclude_orbs=exclude_orbs,
             Rcut=Rcut,
             ne=ne,
             np=np,
             use_cache=use_cache,
             description=description,
             output_path=output_path,
```

### Comparing `TB2J-0.8.2.5/TB2J/myTB.py` & `TB2J-0.8.2.7/TB2J/myTB.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.5/TB2J/orbmap.py` & `TB2J-0.8.2.7/TB2J/orbmap.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.5/TB2J/pauli.py` & `TB2J-0.8.2.7/TB2J/pauli.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.5/TB2J/pert.py` & `TB2J-0.8.2.7/TB2J/pert.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.5/TB2J/plot.py` & `TB2J-0.8.2.7/TB2J/plot.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.5/TB2J/rotate_atoms.py` & `TB2J-0.8.2.7/TB2J/rotate_atoms.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.5/TB2J/sisl_wrapper.py` & `TB2J-0.8.2.7/TB2J/sisl_wrapper.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.5/TB2J/spinham/base_parser.py` & `TB2J-0.8.2.7/TB2J/spinham/base_parser.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.5/TB2J/spinham/constants.py` & `TB2J-0.8.2.7/TB2J/spinham/constants.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.5/TB2J/spinham/hamiltonian.py` & `TB2J-0.8.2.7/TB2J/spinham/hamiltonian.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.5/TB2J/spinham/hamiltonian_terms.py` & `TB2J-0.8.2.7/TB2J/spinham/hamiltonian_terms.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.5/TB2J/spinham/plot.py` & `TB2J-0.8.2.7/TB2J/spinham/plot.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.5/TB2J/spinham/qsolver.py` & `TB2J-0.8.2.7/TB2J/spinham/qsolver.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.5/TB2J/spinham/spin_api.py` & `TB2J-0.8.2.7/TB2J/spinham/spin_api.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.5/TB2J/spinham/spin_xml.py` & `TB2J-0.8.2.7/TB2J/spinham/spin_xml.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.5/TB2J/spinham/supercell.py` & `TB2J-0.8.2.7/TB2J/spinham/supercell.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.5/TB2J/tensor_rotate.py` & `TB2J-0.8.2.7/TB2J/tensor_rotate.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.5/TB2J/utest.py` & `TB2J-0.8.2.7/TB2J/utest.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.5/TB2J/utils.py` & `TB2J-0.8.2.7/TB2J/utils.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.5/TB2J/wannier/w90_parser.py` & `TB2J-0.8.2.7/TB2J/wannier/w90_parser.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.5/TB2J/wannier/w90_tb_parser.py` & `TB2J-0.8.2.7/TB2J/wannier/w90_tb_parser.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.5/TB2J.egg-info/PKG-INFO` & `TB2J-0.8.2.7/TB2J.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TB2J
-Version: 0.8.2.5
+Version: 0.8.2.7
 Summary: TB2J: First principle to Heisenberg exchange J using tight-binding Green function method
 Home-page: UNKNOWN
 Author: Xu He
 Author-email: mailhexu@gmail.com
 License: BSD-2-clause
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `TB2J-0.8.2.5/TB2J.egg-info/SOURCES.txt` & `TB2J-0.8.2.7/TB2J.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.5/scripts/TB2J_downfold.py` & `TB2J-0.8.2.7/scripts/TB2J_downfold.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.5/scripts/TB2J_eigen.py` & `TB2J-0.8.2.7/scripts/TB2J_eigen.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.5/scripts/TB2J_magnon.py` & `TB2J-0.8.2.7/scripts/TB2J_magnon.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.5/scripts/TB2J_merge.py` & `TB2J-0.8.2.7/scripts/TB2J_merge.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.5/scripts/TB2J_rotate.py` & `TB2J-0.8.2.7/scripts/TB2J_rotate.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.5/scripts/abacus2J.py` & `TB2J-0.8.2.7/scripts/abacus2J.py`

 * *Files identical despite different names*

### Comparing `TB2J-0.8.2.5/scripts/siesta2J.py` & `TB2J-0.8.2.7/scripts/wann2J.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,154 +1,194 @@
 #!/usr/bin/env python3
-from TB2J.manager import gen_exchange_siesta
-from TB2J.versioninfo import print_license
-import sys
 import argparse
+import sys
+from TB2J.manager import gen_exchange
+from TB2J.versioninfo import print_license
 
 
-def run_siesta2J():
+def run_wann2J():
     print_license()
     parser = argparse.ArgumentParser(
-        description="siesta2J: Using magnetic force theorem to calculate exchange parameter J from siesta Hamiltonian"
+        description="wann2J: Using magnetic force theorem to calculate exchange parameter J from wannier functions"
+    )
+    parser.add_argument(
+        "--path", help="path to the wannier files", default="./", type=str
+    )
+    parser.add_argument(
+        "--posfile", help="name of the position file", default="POSCAR", type=str
+    )
+    parser.add_argument(
+        "--prefix_spinor",
+        help="prefix to the spinor wannier files",
+        default="wannier90",
+        type=str,
+    )
+    parser.add_argument(
+        "--prefix_up",
+        help="prefix to the spin up wannier files",
+        default="wannier90.up",
+        type=str,
     )
     parser.add_argument(
-        "--fdf_fname", help="path of the input fdf file", default="./", type=str
+        "--prefix_down",
+        help="prefix to the spin down wannier files",
+        default="wannier90.dn",
+        type=str,
     )
     parser.add_argument(
         "--elements",
-        help="list of elements to be considered in Heisenberg model. For each element, a postfixes can be used to specify the orbitals(Only with Siesta backend), eg. Fe_3d, or Fe_3d_4s ",
+        help="elements to be considered in Heisenberg model",
         default=None,
         type=str,
         nargs="*",
     )
     parser.add_argument(
+        "--groupby",
+        help="In the spinor case, the order of the orbitals have two conventions: 1: group by spin (orb1_up, orb2_up,... orb1_down, ...), 2,group by orbital (orb1_up, orb1_down, orb2_up, ...,). Use 'spin' in the former case and 'orbital' in the latter case. The default is spin.",
+        default="spin",
+        type=str,
+    )
+    parser.add_argument(
+        "--write_dm",
+        help="whether to write density matrix",
+        action="store_true",
+        default=False,
+    )
+
+    parser.add_argument(
         "--rcut",
-        help="range of R. The default is all the commesurate R to the kmesh",
+        help="cutoff of spin pair distance. The default is to calculate all commensurate R point to the k mesh.",
         default=None,
         type=float,
     )
-    parser.add_argument(
-        "--efermi", help="Fermi energy in eV. For test only. ", default=None, type=float
-    )
+    parser.add_argument("--efermi", help="Fermi energy in eV", default=None, type=float)
     parser.add_argument(
         "--kmesh",
-        help="kmesh in the format of kx ky kz. Monkhorst pack. If all the numbers are odd, it is Gamma cenetered. (strongly recommended), Default: 5 5 5",
+        help="kmesh in the format of kx ky kz",
         type=int,
         nargs="*",
         default=[5, 5, 5],
     )
     parser.add_argument(
         "--emin",
         help="energy minimum below efermi, default -14 eV",
         type=float,
         default=-14.0,
     )
     parser.add_argument(
         "--emax",
-        help="energy maximum above efermi. Default 0.0 eV",
+        help="energy maximum above efermi, default 0.0 eV",
         type=float,
-        default=0.05,
+        default=0.0,
     )
     parser.add_argument(
-        "--use_cache",
-        help="whether to use disk file for temporary storing wavefunctions and hamiltonian to reduce memory usage. Default: False",
-        action="store_true",
-        default=False,
+        "--nz",
+        help="number of steps for semicircle contour, default: 100",
+        default=100,
+        type=int,
     )
-    # parser.add_argument(
-    #    '--height',
-    #    help=
-    #    'energy contour, a small number (often between 0.1 to 0.5, default 0.2)',
-    #    type=float,
-    #    default=0.1)
-    parser.add_argument(
-        "--nz", help="number of integration steps. Default: 50", default=50, type=int
-    )
-    # parser.add_argument(
-    #    '--nz2', help='number of steps 2, default: 200', default=200, type=int)
-    # parser.add_argument(
-    #    '--nz3', help='number of steps 3, default: 50', default=50, type=int)
     parser.add_argument(
         "--cutoff",
-        help="The minimum of J amplitude to write, (in eV). Default: 1e-5 eV",
+        help="The minimum of J amplitude to write, (in eV), default is 1e-5 eV",
         default=1e-5,
         type=float,
     )
-
     parser.add_argument(
         "--exclude_orbs",
-        help="the indices of wannier functions to be excluded from magnetic site. counting start from 0. Default is none.",
+        help="the indices of wannier functions to be excluded from magnetic site. counting start from 0",
         default=[],
         type=int,
         nargs="+",
     )
 
     parser.add_argument(
         "--np",
         help="number of cpu cores to use in parallel, default: 1",
         default=1,
         type=int,
     )
 
     parser.add_argument(
+        "--use_cache",
+        help="whether to use disk file for temporary storing wavefunctions and hamiltonian to reduce memory usage. Default: False",
+        action="store_true",
+        default=False,
+    )
+
+    parser.add_argument(
         "--description",
         help="add description of the calculatiion to the xml file. Essential information, like the xc functional, U values, magnetic state should be given.",
         type=str,
         default="Calculated with TB2J.",
     )
 
     parser.add_argument(
-        "--orb_decomposition",
-        default=False,
+        "--spinor",
         action="store_true",
-        help="whether to do orbital decomposition in the non-collinear mode. Default: False.",
+        help="Whether to use spinor wannier function.",
+        default=False,
     )
 
     parser.add_argument(
-        "--fname",
-        default="exchange.xml",
-        type=str,
-        help="exchange xml file name. default: exchange.xml",
+        "--orb_decomposition",
+        default=False,
+        action="store_true",
+        help="whether to do orbital decomposition in the non-collinear mode.",
     )
 
     parser.add_argument(
         "--output_path",
         help="The path of the output directory, default is TB2J_results",
         type=str,
         default="TB2J_results",
     )
 
+    parser.add_argument(
+        "--wannier_type",
+        help="The type of Wannier function, either Wannier90 or banddownfolder",
+        type=str,
+        default="Wannier90",
+    )
+
+    # parser.add_argument("--qspace",
+    #                    action="store_true",
+    #                    help="Whether to calculate J in qspace first and transform to real space.",
+    #                    default=False)
+
     args = parser.parse_args()
 
+    if args.efermi is None:
+        print("Please input fermi energy using --efermi ")
+        sys.exit()
     if args.elements is None:
         print("Please input the magnetic elements, e.g. --elements Fe Ni")
         sys.exit()
 
-    include_orbs = {}
-    for element in args.elements:
-        if "_" in element:
-            elem = element.split("_")[0]
-            orb = element.split("_")[1:]
-            include_orbs[elem] = orb
-        else:
-            include_orbs[element] = None
-
-    gen_exchange_siesta(
-        fdf_fname=args.fdf_fname,
+    gen_exchange(
+        path=args.path,
+        colinear=(not args.spinor),
+        groupby=args.groupby,
+        posfile=args.posfile,
+        efermi=args.efermi,
         kmesh=args.kmesh,
-        magnetic_elements=list(include_orbs.keys()),
-        include_orbs=include_orbs,
+        magnetic_elements=args.elements,
         Rcut=args.rcut,
+        prefix_SOC=args.prefix_spinor,
+        prefix_up=args.prefix_up,
+        prefix_dn=args.prefix_down,
         emin=args.emin,
         emax=args.emax,
         nz=args.nz,
-        description=args.description,
-        output_path=args.output_path,
         use_cache=args.use_cache,
         np=args.np,
+        description=args.description,
+        output_path=args.output_path,
         exclude_orbs=args.exclude_orbs,
+        wannier_type=args.wannier_type,
+        # qspace=args.qspace,
+        write_density_matrix=args.write_dm,
         orb_decomposition=args.orb_decomposition,
     )
 
 
 if __name__ == "__main__":
-    run_siesta2J()
+    run_wann2J()
```

### Comparing `TB2J-0.8.2.5/setup.py` & `TB2J-0.8.2.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 from setuptools import setup, find_packages
 
-__version__ = "0.8.2.5"
+__version__ = "0.8.2.7"
 
 long_description = """TB2J is a Python package aimed to compute automatically the magnetic interactions (superexchange  and Dzyaloshinskii-Moriya) between atoms of magnetic crystals from DFT Hamiltonian based on Wannier functions or Linear combination of atomic orbitals. It uses the Green's function method and take the local rigid spin rotation as a perturbation. The package can take the output from Wannier90, which is interfaced with many density functional theory codes or from codes based on localised orbitals. A minimal user input is needed, which allows for an easily integration into a high-throughput workflows. """
 
 setup(
     name="TB2J",
     version=__version__,
     description="TB2J: First principle to Heisenberg exchange J using tight-binding Green function method",
```

