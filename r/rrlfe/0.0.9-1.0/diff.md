# Comparing `tmp/rrlfe-0.0.9.tar.gz` & `tmp/rrlfe-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/rrlfe-0.0.9.tar", last modified: Wed Apr  6 22:14:35 2022, max compression
+gzip compressed data, was "rrlfe-1.0.tar", max compression
```

## Comparing `rrlfe-0.0.9.tar` & `rrlfe-1.0.tar`

### file list

```diff
@@ -1,42 +1,77 @@
-drwxr-xr-x   0 bandari    (501) staff       (20)        0 2022-04-06 22:14:35.000000 rrlfe-0.0.9/
--rw-r--r--   0 bandari    (501) staff       (20)      523 2022-04-06 22:14:35.000000 rrlfe-0.0.9/PKG-INFO
--rw-r--r--   0 bandari    (501) staff       (20)     5029 2022-03-06 22:35:23.000000 rrlfe-0.0.9/high_level_application_script.py
--rw-r--r--   0 bandari    (501) staff       (20)      806 2022-03-06 22:35:26.000000 rrlfe-0.0.9/app2.py
--rw-r--r--   0 bandari    (501) staff       (20)     2363 2022-03-09 23:28:15.000000 rrlfe-0.0.9/high_level_reduction_script.py
--rw-r--r--   0 bandari    (501) staff       (20)       54 2022-03-06 22:36:02.000000 rrlfe-0.0.9/__init__.py
--rw-r--r--   0 bandari    (501) staff       (20)      734 2022-03-23 21:55:16.000000 rrlfe-0.0.9/README.md
--rw-r--r--   0 bandari    (501) staff       (20)     1018 2022-04-06 22:14:33.000000 rrlfe-0.0.9/setup.py
-drwxr-xr-x   0 bandari    (501) staff       (20)        0 2022-04-06 22:14:35.000000 rrlfe-0.0.9/rrlfe.egg-info/
--rw-r--r--   0 bandari    (501) staff       (20)      523 2022-04-06 22:14:35.000000 rrlfe-0.0.9/rrlfe.egg-info/PKG-INFO
--rw-r--r--   0 bandari    (501) staff       (20)     1001 2022-04-06 22:14:35.000000 rrlfe-0.0.9/rrlfe.egg-info/SOURCES.txt
--rw-r--r--   0 bandari    (501) staff       (20)        9 2022-04-06 22:14:35.000000 rrlfe-0.0.9/rrlfe.egg-info/top_level.txt
--rw-r--r--   0 bandari    (501) staff       (20)        1 2022-04-06 22:14:35.000000 rrlfe-0.0.9/rrlfe.egg-info/dependency_links.txt
--rw-r--r--   0 bandari    (501) staff       (20)      710 2022-03-06 22:36:54.000000 rrlfe-0.0.9/app.py
--rw-r--r--   0 bandari    (501) staff       (20)       38 2022-04-06 22:14:35.000000 rrlfe-0.0.9/setup.cfg
-drwxr-xr-x   0 bandari    (501) staff       (20)        0 2022-04-06 22:14:35.000000 rrlfe-0.0.9/modules/
--rw-r--r--   0 bandari    (501) staff       (20)        0 2022-03-06 22:37:06.000000 rrlfe-0.0.9/modules/conftest.py
--rw-r--r--   0 bandari    (501) staff       (20)     5909 2022-03-24 12:47:33.000000 rrlfe-0.0.9/modules/run_robo.py
--rw-r--r--   0 bandari    (501) staff       (20)    16694 2022-03-06 22:37:06.000000 rrlfe-0.0.9/modules/sdss_spectra_cosmic_ray_removal.py
--rw-r--r--   0 bandari    (501) staff       (20)    14838 2022-03-06 22:37:06.000000 rrlfe-0.0.9/modules/error_propagation_and_mapping.py
--rw-r--r--   0 bandari    (501) staff       (20)     2272 2022-03-06 22:37:06.000000 rrlfe-0.0.9/modules/norm_spec.py
--rw-r--r--   0 bandari    (501) staff       (20)    29312 2022-03-07 00:01:37.000000 rrlfe-0.0.9/modules/scrape_ew_and_errew.py
--rw-r--r--   0 bandari    (501) staff       (20)       29 2022-03-06 22:37:06.000000 rrlfe-0.0.9/modules/__init__backup.py
--rw-r--r--   0 bandari    (501) staff       (20)     3843 2022-03-06 22:37:06.000000 rrlfe-0.0.9/modules/__init__.py
--rw-r--r--   0 bandari    (501) staff       (20)     6358 2022-03-06 22:37:06.000000 rrlfe-0.0.9/modules/teff_retrieval.py
--rw-r--r--   0 bandari    (501) staff       (20)      119 2022-03-06 22:37:06.000000 rrlfe-0.0.9/modules/junk_test.py
--rw-r--r--   0 bandari    (501) staff       (20)     3170 2022-03-06 22:37:07.000000 rrlfe-0.0.9/modules/covars.py
--rw-r--r--   0 bandari    (501) staff       (20)     5231 2022-03-06 22:37:07.000000 rrlfe-0.0.9/modules/manually_remove_points_spectra.py
--rw-r--r--   0 bandari    (501) staff       (20)     9015 2022-03-06 22:37:07.000000 rrlfe-0.0.9/modules/interpolate_spectra_masked_regions.py
--rw-r--r--   0 bandari    (501) staff       (20)     1564 2022-03-06 22:37:07.000000 rrlfe-0.0.9/modules/sift_manual_spectra.py
--rw-r--r--   0 bandari    (501) staff       (20)    10383 2022-03-06 22:37:07.000000 rrlfe-0.0.9/modules/consolidate_pre_mcmc.py
--rw-r--r--   0 bandari    (501) staff       (20)     4208 2022-03-06 22:37:07.000000 rrlfe-0.0.9/modules/make_high_res_feh_basis.py
--rw-r--r--   0 bandari    (501) staff       (20)    17726 2022-03-06 22:37:07.000000 rrlfe-0.0.9/modules/plot_utils.py
--rw-r--r--   0 bandari    (501) staff       (20)      167 2022-03-06 22:37:07.000000 rrlfe-0.0.9/modules/yada_compile_normalization.py
--rw-r--r--   0 bandari    (501) staff       (20)     1626 2022-03-24 21:39:29.000000 rrlfe-0.0.9/modules/compile_normalization.py
--rw-r--r--   0 bandari    (501) staff       (20)      442 2022-03-06 22:37:07.000000 rrlfe-0.0.9/modules/ca_correction.py
--rw-r--r--   0 bandari    (501) staff       (20)     2738 2022-03-06 22:37:07.000000 rrlfe-0.0.9/modules/write_masks_for_no_ray_spectra.py
--rw-r--r--   0 bandari    (501) staff       (20)     1626 2022-03-24 21:47:26.000000 rrlfe-0.0.9/modules/junk_compile_normalization.py
--rw-r--r--   0 bandari    (501) staff       (20)    13840 2022-03-06 22:37:07.000000 rrlfe-0.0.9/modules/find_feh.py
--rw-r--r--   0 bandari    (501) staff       (20)    22615 2022-03-06 22:37:07.000000 rrlfe-0.0.9/modules/run_emcee.py
--rw-r--r--   0 bandari    (501) staff       (20)    20063 2022-03-09 23:37:08.000000 rrlfe-0.0.9/modules/create_spec_realizations.py
--rw-r--r--   0 bandari    (501) staff       (20)     8628 2022-03-06 22:37:07.000000 rrlfe-0.0.9/modules/normalize_simple.py
+-rw-r--r--   0        0        0     1068 2023-04-25 05:27:14.483283 rrlfe-1.0/LICENSE
+-rw-r--r--   0        0        0     1073 2023-04-25 05:27:14.484284 rrlfe-1.0/LICENSE.txt
+-rw-r--r--   0        0        0     1325 2024-03-29 01:29:32.958696 rrlfe-1.0/README.md
+-rw-r--r--   0        0        0      686 2024-04-07 04:45:38.710104 rrlfe-1.0/pyproject.toml
+-rw-r--r--   0        0        0     8178 2024-03-30 04:59:10.430180 rrlfe-1.0/rrlfe/__init__.py
+-rw-r--r--   0        0        0       29 2024-03-30 04:59:10.431180 rrlfe-1.0/rrlfe/__init__backup.py
+-rw-r--r--   0        0        0     1896 2024-03-30 04:59:10.432180 rrlfe-1.0/rrlfe/compile_normalization.py
+-rw-r--r--   0        0        0     4064 2024-03-30 04:59:10.433180 rrlfe-1.0/rrlfe/conf/config_apply.ini
+-rw-r--r--   0        0        0     3206 2024-03-31 02:59:36.146454 rrlfe-1.0/rrlfe/conf/config_gen.ini
+-rw-r--r--   0        0        0        0 2024-03-30 04:59:10.434180 rrlfe-1.0/rrlfe/conftest.py
+-rw-r--r--   0        0        0     8818 2024-03-30 04:59:10.435180 rrlfe-1.0/rrlfe/consolidate_pre_mcmc.py
+-rw-r--r--   0        0        0     3170 2024-03-30 04:59:10.436179 rrlfe-1.0/rrlfe/covars.py
+-rw-r--r--   0        0        0    20081 2024-03-31 02:27:06.774278 rrlfe-1.0/rrlfe/create_spec_realizations.py
+-rw-r--r--   0        0        0    14654 2024-03-30 04:59:10.438180 rrlfe-1.0/rrlfe/error_propagation_and_mapping.py
+-rw-r--r--   0        0        0     8130 2024-03-30 04:59:10.439180 rrlfe-1.0/rrlfe/final_corrxn.py
+-rw-r--r--   0        0        0     9609 2024-03-30 04:59:10.440180 rrlfe-1.0/rrlfe/find_feh.py
+-rw-r--r--   0        0        0     1696 2024-03-30 04:59:10.441180 rrlfe-1.0/rrlfe/high_level_application_accordion.py
+-rw-r--r--   0        0        0     1730 2024-03-30 04:59:10.442180 rrlfe-1.0/rrlfe/high_level_generation_accordion.py
+-rw-r--r--   0        0        0     9015 2024-03-30 04:59:10.443180 rrlfe-1.0/rrlfe/interpolate_spectra_masked_regions.py
+-rw-r--r--   0        0        0    23139 2024-03-30 04:59:10.444180 rrlfe-1.0/rrlfe/make_high_res_feh_basis.py
+-rw-r--r--   0        0        0     5231 2024-03-30 04:59:10.444180 rrlfe-1.0/rrlfe/manually_remove_points_spectra.py
+-rw-r--r--   0        0        0     2219 2024-03-30 04:59:10.446180 rrlfe-1.0/rrlfe/norm_spec.py
+-rw-r--r--   0        0        0     7629 2024-03-30 04:59:10.446180 rrlfe-1.0/rrlfe/normalize_simple.py
+-rw-r--r--   0        0        0    17491 2024-03-30 04:59:10.447180 rrlfe-1.0/rrlfe/plot_utils.py
+-rw-r--r--   0        0        0    23166 2024-04-07 02:43:21.147563 rrlfe-1.0/rrlfe/run_emcee.py
+-rw-r--r--   0        0        0     6711 2024-03-30 04:59:10.449180 rrlfe-1.0/rrlfe/run_robo.py
+-rw-r--r--   0        0        0    36182 2024-03-30 04:59:10.450180 rrlfe-1.0/rrlfe/scrape_ew_and_errew.py
+-rw-r--r--   0        0        0    16694 2024-03-30 04:59:10.451180 rrlfe-1.0/rrlfe/sdss_spectra_cosmic_ray_removal.py
+-rw-r--r--   0        0        0     3688 2024-03-30 04:59:10.452180 rrlfe-1.0/rrlfe/set_params.py
+-rw-r--r--   0        0        0     1529 2024-03-30 04:59:10.453180 rrlfe-1.0/rrlfe/sift_manual_spectra.py
+-rw-r--r--   0        0        0     8030 2024-03-30 04:59:10.453180 rrlfe-1.0/rrlfe/teff_retrieval.py
+-rw-r--r--   0        0        0    11592 2023-04-25 05:27:14.608284 rrlfe-1.0/rrlfe/test.pdf
+-rw-r--r--   0        0        0    11572 2023-04-25 05:27:14.679285 rrlfe-1.0/rrlfe/test_resids.pdf
+-rw-r--r--   0        0        0      175 2024-03-31 02:55:04.380015 rrlfe-1.0/rrlfe/test_src/bckgrnd_input.txt
+-rw-r--r--   0        0        0    12071 2023-04-25 05:27:14.740285 rrlfe-1.0/rrlfe/test_synced.pdf
+-rw-r--r--   0        0        0    11808 2023-04-25 05:27:14.741285 rrlfe-1.0/rrlfe/test_unsynced.pdf
+-rw-r--r--   0        0        0    53248 2024-03-30 04:59:10.457180 rrlfe-1.0/rrlfe/tests/.coverage
+-rw-r--r--   0        0        0        0 2024-03-30 04:59:10.457180 rrlfe-1.0/rrlfe/tests/20230226_170843.log
+-rw-r--r--   0        0        0        0 2024-03-30 04:59:10.458180 rrlfe-1.0/rrlfe/tests/__init__.py
+-rw-r--r--   0        0        0      141 2024-03-30 04:59:10.459180 rrlfe-1.0/rrlfe/tests/__pycache__/__init__.cpython-36.pyc
+-rw-r--r--   0        0        0      145 2024-03-30 04:59:10.460180 rrlfe-1.0/rrlfe/tests/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0        0        0      149 2024-03-31 02:59:36.148454 rrlfe-1.0/rrlfe/tests/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     1508 2024-03-30 04:59:10.462180 rrlfe-1.0/rrlfe/tests/__pycache__/junk_test.cpython-38-pytest-7.1.2.pyc
+-rw-r--r--   0        0        0     1344 2024-03-30 04:59:10.463180 rrlfe-1.0/rrlfe/tests/__pycache__/test_compile_normalization.cpython-36-PYTEST.pyc
+-rw-r--r--   0        0        0     1344 2024-03-30 04:59:10.463180 rrlfe-1.0/rrlfe/tests/__pycache__/test_compile_normalization.cpython-36-pytest-6.2.4.pyc
+-rw-r--r--   0        0        0     1337 2024-03-30 04:59:10.464180 rrlfe-1.0/rrlfe/tests/__pycache__/test_compile_normalization.cpython-37-pytest-7.1.2.pyc
+-rw-r--r--   0        0        0     1341 2024-03-30 04:59:10.465180 rrlfe-1.0/rrlfe/tests/__pycache__/test_compile_normalization.cpython-38-pytest-5.4.3.pyc
+-rw-r--r--   0        0        0     1442 2024-03-31 02:59:36.149454 rrlfe-1.0/rrlfe/tests/__pycache__/test_compile_normalization.cpython-38-pytest-7.1.2.pyc
+-rw-r--r--   0        0        0    12235 2024-03-30 04:59:10.467180 rrlfe-1.0/rrlfe/tests/__pycache__/test_create_spec_realizations.cpython-36-PYTEST.pyc
+-rw-r--r--   0        0        0     9533 2024-03-30 04:59:10.468180 rrlfe-1.0/rrlfe/tests/__pycache__/test_create_spec_realizations.cpython-36-pytest-6.2.4.pyc
+-rw-r--r--   0        0        0    11568 2024-03-31 02:59:36.171454 rrlfe-1.0/rrlfe/tests/__pycache__/test_create_spec_realizations.cpython-38-pytest-7.1.2.pyc
+-rw-r--r--   0        0        0     1996 2024-03-30 04:59:10.470180 rrlfe-1.0/rrlfe/tests/__pycache__/test_init_fcns.cpython-36-PYTEST.pyc
+-rw-r--r--   0        0        0     1995 2024-03-30 04:59:10.471180 rrlfe-1.0/rrlfe/tests/__pycache__/test_init_fcns.cpython-36-pytest-6.2.4.pyc
+-rw-r--r--   0        0        0     2347 2024-03-31 02:59:36.173454 rrlfe-1.0/rrlfe/tests/__pycache__/test_init_fcns.cpython-38-pytest-7.1.2.pyc
+-rw-r--r--   0        0        0     1181 2024-03-30 04:59:10.473180 rrlfe-1.0/rrlfe/tests/__pycache__/test_junk.cpython-38-pytest-7.1.2.pyc
+-rw-r--r--   0        0        0    13715 2024-03-30 04:59:10.474180 rrlfe-1.0/rrlfe/tests/__pycache__/test_run_emcee.cpython-36-PYTEST.pyc
+-rw-r--r--   0        0        0    13196 2024-03-30 04:59:10.475180 rrlfe-1.0/rrlfe/tests/__pycache__/test_run_emcee.cpython-36-pytest-6.2.4.pyc
+-rw-r--r--   0        0        0    12182 2024-03-31 02:59:36.174454 rrlfe-1.0/rrlfe/tests/__pycache__/test_run_emcee.cpython-38-pytest-7.1.2.pyc
+-rw-r--r--   0        0        0      580 2024-03-30 04:59:10.477180 rrlfe-1.0/rrlfe/tests/__pycache__/test_run_robo.cpython-36-PYTEST.pyc
+-rw-r--r--   0        0        0      580 2024-03-30 04:59:10.477180 rrlfe-1.0/rrlfe/tests/__pycache__/test_run_robo.cpython-36-pytest-6.2.4.pyc
+-rw-r--r--   0        0        0      594 2024-03-31 02:59:36.175454 rrlfe-1.0/rrlfe/tests/__pycache__/test_run_robo.cpython-38-pytest-7.1.2.pyc
+-rw-r--r--   0        0        0    18058 2024-03-30 04:59:10.479180 rrlfe-1.0/rrlfe/tests/__pycache__/test_scrape_ew_and_errew.cpython-36-PYTEST.pyc
+-rw-r--r--   0        0        0    14330 2024-03-30 04:59:10.480180 rrlfe-1.0/rrlfe/tests/__pycache__/test_scrape_ew_and_errew.cpython-36-pytest-6.2.4.pyc
+-rw-r--r--   0        0        0    16508 2024-03-31 02:59:36.177454 rrlfe-1.0/rrlfe/tests/__pycache__/test_scrape_ew_and_errew.cpython-38-pytest-7.1.2.pyc
+-rw-r--r--   0        0        0     3525 2024-03-30 04:59:10.482180 rrlfe-1.0/rrlfe/tests/__pycache__/test_teff_retrieval.cpython-36-PYTEST.pyc
+-rw-r--r--   0        0        0     3523 2024-03-30 04:59:10.483180 rrlfe-1.0/rrlfe/tests/__pycache__/test_teff_retrieval.cpython-36-pytest-6.2.4.pyc
+-rw-r--r--   0        0        0     3473 2024-03-30 04:59:10.484180 rrlfe-1.0/rrlfe/tests/__pycache__/test_teff_retrieval.cpython-37-pytest-7.1.2.pyc
+-rw-r--r--   0        0        0     3554 2024-03-31 02:59:36.178454 rrlfe-1.0/rrlfe/tests/__pycache__/test_teff_retrieval.cpython-38-pytest-7.1.2.pyc
+-rw-r--r--   0        0        0      807 2024-03-30 04:59:10.486180 rrlfe-1.0/rrlfe/tests/test_compile_normalization.py
+-rw-r--r--   0        0        0    11096 2024-03-30 04:59:10.487180 rrlfe-1.0/rrlfe/tests/test_create_spec_realizations.py
+-rw-r--r--   0        0        0     1785 2024-03-30 04:59:10.487180 rrlfe-1.0/rrlfe/tests/test_init_fcns.py
+-rw-r--r--   0        0        0    11043 2024-03-30 04:59:10.488180 rrlfe-1.0/rrlfe/tests/test_run_emcee.py
+-rw-r--r--   0        0        0     1487 2024-03-30 04:59:10.489180 rrlfe-1.0/rrlfe/tests/test_run_robo.py
+-rw-r--r--   0        0        0    12438 2024-03-30 04:59:10.490180 rrlfe-1.0/rrlfe/tests/test_scrape_ew_and_errew.py
+-rw-r--r--   0        0        0     2948 2024-03-30 04:59:10.491180 rrlfe-1.0/rrlfe/tests/test_teff_retrieval.py
+-rw-r--r--   0        0        0     2738 2024-03-30 04:59:10.492180 rrlfe-1.0/rrlfe/write_masks_for_no_ray_spectra.py
+-rw-r--r--   0        0        0     1994 1970-01-01 00:00:00.000000 rrlfe-1.0/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `rrlfe-0.0.9/modules/run_robo.py` & `rrlfe-1.0/rrlfe/run_robo.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,49 +1,44 @@
-'''
-Calls Robospect to find EWs of the normalized, noise-churned spectra
-'''
-
 import os
 import glob
 import multiprocessing
+from multiprocessing import get_context
 import logging
 from . import *
 
 
 class RunRobo:
+    """
+    Enables multiprocessing
 
-    def __init__(self, write_dir, robo_dir):
+    Parameters:
+        write_dir (str): directory to write to
+        robo_dir (str): directory in which robospect.py lives
+    """
 
-        '''
-        This just configures IO
-        '''
+    def __init__(self, write_dir, robo_dir):
 
         self.norm_spec_deposit_dir = write_dir
         self.robo_dir = robo_dir
 
     def __call__(self, file_name):
 
-        '''
-        INPUTS:
-        file_name: the absolute file name of one file to run Robospect on
-        normzed_spec_source_dir: directory containing the normalized spectra
-        robo_dir: directory of the robospect.py repo
-
-        OUTPUTS:
-        (writes files to disk)
-        '''
-        print("deposit: " + self.norm_spec_deposit_dir)
-        print("robo_dir: " + self.norm_spec_deposit_dir)
+        """
+        Parameters:
+            file_name: the absolute file name of one file to run Robospect on
+
+        Returns:
+            (writes files to disk)
+        """
 
         # for applying to synthetic spectra
         logging.info("Running Robospect on "+ file_name + " \n")
 
         # define string for output base names
-        #file_specific_string = p.split(".")[-2].split("/")[-1]
-        ## ## the below is specific to *smo* files
+        # the below is specific to *smo* files
         file_specific_string = file_name.split("/")[-1]
 
         # example rSpect command:
         ## python rSpect.py -i 4       ['Run four iterations of the full fitting loop,
         ##                               with noise/continuum/detection/initial line
         ##                               fits/non-linear least squares line fits all
         ##                               happening on each iteration.' --C. Waters]
@@ -59,87 +54,108 @@
         ##                               when estimating FWHM value.' --C. Waters]
         ## -F chi_window 20.0          ['Fit chi^2 calculation using windows of
         ##                               +/- 20AA from the line center.' --C. Waters]
         ## -vvvv                       ['Enable all debug messages for all components.'
         ##                               --C. Waters]
 
         logging.info("Robospect cmd:")
-        logging.info("python "+self.robo_dir + "bin/rSpect.py -i 4 " +str(file_name) + \
-                    " -P " + self.norm_spec_deposit_dir + file_specific_string + \
-                    " --line_list " + self.robo_dir + "tmp/ll" +" -C name null" + \
-                    " -D name null" +" -N name boxcar" + " -I range 10.0" + \
-                    " -F chi_window 20.0 " + "-vvvv")
-        os.system("python " +
-              self.robo_dir + "bin/rSpect.py -i 4 " +
-              str(file_name) +
-              " -P " + self.norm_spec_deposit_dir + file_specific_string +
-              " --line_list " + self.robo_dir + "tmp/ll" +
-              " -C name null" +
-              " -D name null" +
-              " -N name boxcar" +
-              " -I range 10.0" +
-              " -F chi_window 20.0 " +
-              "-vvvv")
-
-        logging.info("Robospect output files written to " + \
-            self.norm_spec_deposit_dir + file_specific_string + "*")
-
-
-def main(
-        normzed_spec_source_dir = config_red["data_dirs"]["DIR_REZNS_SPEC_NORM_FINAL"],
-        write_dir=config_red["data_dirs"]["DIR_ROBO_OUTPUT"],
-        robo_dir=config_red["sys_dirs"]["DIR_ROBO"]
-        ):
-    '''
-    Accumulate list of filenames of normalized synthetic spectra, then
-    measure EWs
-
-    INPUTS:
-    normzed_spec_source_dir: source directory of normalized spectra which
-        Robospect will be run on
-    write_dir: directory to which Robospect output will be written to
-    robo_dir: directory of the robospect.py repo
-
-    OUTPUTS:
-    (EW data written to file)
-    '''
-
-    ## ## note that I have put in a specific string to look for
-    ## ## in the file name here; this might be a weakness later on
-
-    pool = multiprocessing.Pool(ncpu)
-
-    ## ## note the below file name list collects ALL files in that directory,
-    ## ## not just the ones listed in the initial .list file
-    file_name_list = glob.glob(normzed_spec_source_dir+"*")
-    logging.info('Reading in spectra from directory')
-    logging.info(normzed_spec_source_dir)
-
-    # Check to see if it is empty (if not, there is data from a previous
-    # run that will inadvertently be used later)
-    preexisting_file_list = glob.glob(write_dir + "/*", recursive=False)
-    print(preexisting_file_list)
-
-    print(len(preexisting_file_list))
-    if (len(preexisting_file_list) > 0):
-        logging.info("------------------------------")
-        logging.info("Directory to receive Robospect output not empty!!")
-        logging.info(write_dir)
-        logging.info("------------------------------")
-        input("Do what you want with those files, then hit [Enter]")
-
-    # run Robospect on normalized spectra in parallel
-    # (N.b. Setting the config files allows Robospect to dump files in the right places)
-    run_robospect_instance = RunRobo(write_dir = write_dir, robo_dir = robo_dir)
-    #if (configuration == "config"):
-    #    run_robospect_instance = RunRobo(config_data=configuration)
-    #elif (configuration == "config_apply"):
-    #    run_robospect_instance = RunRobo(config_data=config_apply)
+        cmd_string = "python "+ self.robo_dir + "bin/rSpect.py -i 4 " + str(file_name) + \
+            " -P " + self.norm_spec_deposit_dir + file_specific_string + \
+            " --line_list " + self.robo_dir + "tmp/ll" +" -C name null" + \
+            " -D name null" + " -N name boxcar" + " -I range 10.0" + \
+            " -F chi_window 20.0 " + "-vvvv"
+        logging.info(cmd_string)
+        try:
+            os.system(cmd_string)
+            logging.info("Robospect output files written to " + \
+                self.norm_spec_deposit_dir + file_specific_string + "*")
+        except:
+            logging.error("Failed to carry out cmd " + cmd_string)
+
+
+class Robo():
+    """
+    Runs the Robospect EW measurement
+
+    Parameters:
+        module_name (str): name of module
+        robo_dir_read (str): directory Robospect reads spectra from
+        normzed_spec_dir_read (str): directory of normalized spectra
+        robo_output_write (str): directory Robospect writes EW info to
+
+    Returns:
+        [EW data written to text file]
+    """
+
+    def __init__(self,
+        module_name,
+        robo_dir_read,
+        normzed_spec_dir_read,
+        robo_output_write):
+
+        self.name = module_name
+        self.robo_dir_read = robo_dir_read
+        self.normzed_spec_source_dir = normzed_spec_dir_read
+        self.robo_output_write = robo_output_write
+
+    def run_step(self, attribs = None):
+
+        # check if write directories exist and are empty
+        #make_dir(self.robo_output_write)
+
+        # explicit syntax necessary for Macbook M1
+        pool = get_context("fork").Pool(ncpu)
+
+        # note the below file name list collects ALL files in that directory,
+        # not just the ones listed in the initial .list file
+        file_name_list = glob.glob(self.normzed_spec_source_dir+"*")
+        
+        # check Robospect input directory exists
+        if os.path.isdir(self.normzed_spec_source_dir):
+            # check if directory exists
+            logging.info('Reading in spectra from '+str(self.normzed_spec_source_dir))
+        else:
+            logging.warning('Making new directory '+str(self.normzed_spec_source_dir)+ ' which will contain normalized input spectra for Robospec')
+            make_dir(self.normzed_spec_source_dir)
+        # check Robospect output directory exists
+        if os.path.isdir(self.robo_output_write):
+            # check if directory exists
+            logging.info('Reading in spectra from '+str(self.robo_output_write))
+        else:
+            logging.warning('Making new directory '+str(self.robo_output_write)+ ' which will contain Robospec output')
+            make_dir(self.robo_output_write)
+
+        # Check to see if it is empty (if not, there is data from a previous
+        # run that will inadvertently be used later)
+        preexisting_file_list = glob.glob(self.robo_output_write + "/*", recursive=False)
+
+        if (len(preexisting_file_list) > 0):
+            logging.info("------------------------------")
+            logging.info("Directory to receive Robospect output not empty!! Pre-existing files will also be used later")
+            logging.info(self.robo_output_write)
+            logging.info("------------------------------")
+
+        # run Robospect on normalized spectra in parallel
+        # (N.b. Setting the config files allows Robospect to dump files in the right places)
+
+        # check if Robospect binary dir exists
+        if os.path.isdir(self.robo_dir_read):
+            # check if directory exists
+            logging.info('Reading in background binary from '+str(self.robo_dir_read))
+        else:
+            logging.error('Robospect input directory '+str(self.robo_dir_read)+ ' does not exist! ')
+            exit()
+       
+        run_robospect_instance = RunRobo(write_dir = self.robo_output_write, robo_dir = self.robo_dir_read)
+        #if (configuration == "config"):
+        #    run_robospect_instance = RunRobo(config_data=configuration)
+        #elif (configuration == "config_apply"):
+        #    run_robospect_instance = RunRobo(config_data=config_apply)
 
-    # in parallel
-    pool.map(run_robospect_instance, file_name_list)
+        # in parallel
+        pool.map(run_robospect_instance, file_name_list)
 
-    # serial (testing only)
-    #run_robospect_instance(file_name_list[0])
+        # serial (testing only)
+        #run_robospect_instance(file_name_list[0])
 
-    logging.info("Done with Robospect")
-    logging.info("-------------------")
+        logging.info("Done with Robospect")
+        logging.info("-------------------")
```

### Comparing `rrlfe-0.0.9/modules/sdss_spectra_cosmic_ray_removal.py` & `rrlfe-1.0/rrlfe/sdss_spectra_cosmic_ray_removal.py`

 * *Files identical despite different names*

### Comparing `rrlfe-0.0.9/modules/error_propagation_and_mapping.py` & `rrlfe-1.0/rrlfe/error_propagation_and_mapping.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import scipy
 import matplotlib.pyplot as plt
 import numpy as np
 from scipy import optimize
 from astropy.stats import bootstrap
 from astropy.utils import NumpyRNGContext
 from multiprocessing import Pool
-#from rrlfe.modules2 import *
+from multiprocessing import get_context
 
 class feh_plotter():
     '''
     Class containing a bunch of the functions we will use to map metallicities
     '''
 
     def __init__(self):
@@ -31,16 +31,14 @@
         '''
         Return CDF of an unsorted input array of values
         '''
 
         number_cum_norm = np.divide(np.arange(len(array_input)),
                                     len(array_input))
         array_input_sort = np.sort(array_input)
-        #array_cdf = np.divide(np.cumsum(array_input_sort),
-        #                      np.cumsum(array_input_sort)[-1])
 
         return array_input_sort, number_cum_norm
 
 
     def cdf_gauss(self, x_range, mu, sig):
         '''
         Returns the CDF of a general Gaussian function for any mu and sig
@@ -70,16 +68,16 @@
         '''
 
         x_vals, y_vals = self.cdf_fcn(np.ravel(feh_mapped_array))
 
         # fit a Gaussian
         popt, pcov = optimize.curve_fit(self.cdf_gauss, x_vals, y_vals)
 
-        print("Line parameters")
-        print(popt)
+        logging.info("Line parameters")
+        logging.info(popt)
 
         xvals_interp = np.arange(x_vals[0], x_vals[-1], 0.001)
         yvals_interp = np.interp(xvals_interp, x_vals, y_vals)
 
         # find element of value closest to 0.5
         percent_bar = 0.5
         idx = np.abs(yvals_interp - percent_bar).argmin()
@@ -120,23 +118,23 @@
                 shortest_xrange_upper = xvals_interp[idx_1sig_above]
                 shortest_xrange_halfway = (0.5*np.subtract(shortest_xrange_upper,
                                                            shortest_xrange_lower) +
                                            shortest_xrange_lower)
 
         # ---------------------------------------------------------------------------
 
-        print("Fe/H at 50 percentile")
+        logging.info("Fe/H at 50 percentile")
         feh_50_perc = xvals_interp[idx]
-        print(feh_50_perc)
+        logging.info(feh_50_perc)
 
-        print("1-sigma interval")
+        logging.info("1-sigma interval")
         feh_1sig_low = xvals_interp[idx_1sig_low]
         feh_1sig_high = xvals_interp[idx_1sig_high]
-        print(feh_1sig_low)
-        print(feh_1sig_high)
+        logging.info(feh_1sig_low)
+        logging.info(feh_1sig_high)
 
         # pickle the data for this one star, to avoid choking the machine
         # with too much plot-making all at once
 
         # replace space with underscore
         name_star_underscore = str(name_star).replace(" ", "_")
         pickle_write_name = (write_pickle_subdir + "plot_info_" +
@@ -177,15 +175,15 @@
         INPUTS:
         name_star: string ID of the star
         read_pickle_subdir: directory to read the pickled Fe/H info from
         write_plot_subdir: directory to write the FYI plots to
         write_plot: write plot or not
         '''
 
-        print("Making CDF and histogram plots of FeH for " + name_star + "...")
+        logging.info("Making CDF and histogram plots of FeH for " + name_star + "...")
 
         # replace space with underscore
         name_star_underscore = str(name_star).replace(" ", "_")
         pickle_read_name = (read_pickle_subdir + "plot_info_" +
                             name_star_underscore + ".pkl")
 
         # open the pickle file
@@ -247,26 +245,25 @@
 
         INPUTS:
         read_pickle_subdir: directory containing the pickle file of Fe/H data
 
         OUTPUTS:
         m_array: array of slopes for each bootstrap step
         b_array: array of y-intercepts for each bootstrap step
-        params_list_star_feh: star names and basis set Fe/H ## ## for what?
+        params_list_star_feh: star names and basis set Fe/H 
         data_1: original data which is fed into the bootstrap
         '''
 
         # read in actual data
-        ## ## N.b. this is just the RRabs with RRab offsets for now
         real_data_1 = pickle.load( open( read_pickle_subdir
                                          + config["file_names"]["RRAB_RRAB_OFFSETS"], "rb" ) )
 
         # arrange the data in a way we can use
         # N.b. This is NOT fake data; I'm just appropriating the old variable name
-        ## ## Note the ersatz Layden errors for now; need to revisit this with values from his paper
+        # Note the placeholder Layden errors for now
         data_1 = { "star_name": real_data_1[0]["name_star"],
                 "feh_lit": real_data_1[0]["feh_highres"],
                 "feh_layden": real_data_1[0]["feh_basis"],
                 "err_feh_lit": np.zeros(len(real_data_1[0]["feh_basis"])),
                 "err_feh_layden": 0.07*np.ones(len(real_data_1[0]["feh_basis"]))}
         #dataset_1 = pd.DataFrame(data=data_1)
 
@@ -318,71 +315,70 @@
 
         time_start = time.time()
         feh_mapped_array = np.nan*np.ones(len(m_array)) # initialize array
 
         # get name and Layden Fe/H of star
         name_star = params_element[:][0]
         feh_test = params_element[:][1]
-        print("Star:")
-        print(name_star)
-        print("Layden Fe/H:")
-        print(feh_test)
+        logging.info("Star:")
+        logging.info(name_star)
+        logging.info("Layden Fe/H:")
+        logging.info(feh_test)
 
         for sample_num in range(0, len(m_array)):
 
             feh_mapped_1sample = m_array[sample_num]*feh_test + b_array[sample_num]
             feh_mapped_array[sample_num] = feh_mapped_1sample
 
         ## take one basis set Fe/H (integral over a Gaussian)
         ## and find what the mapped value should be
 
         # number of samples to take within the Gaussian error around Layden's Fe/H value
         N = 100
-        gaussian_spread = 0.07 ## ## change this in future
+        gaussian_spread = 0.07 # might change this in future
         layden_feh = feh_test # this is the discrete value
 
         # N_m_samples x N_Layden_samples
         feh_mapped_array = np.nan*np.ones((len(m_array), N))
 
         # loop over each sample within the Gaussian around Layden's Fe/H
         for integal_piece in range(0, N):
 
             # set the offset (note mu=0; this is a relative offset)
             offset = np.random.normal(loc=0.0, scale=gaussian_spread)
 
             # loop over all (m,b) combinations found further above
             for sample_num in range(0, len(m_array)):
 
-                ## ## is it layden_feh*(1. + offset) or (layden_feh + offset) ?
                 feh_mapped_1sample = (m_array[sample_num]*layden_feh*(1. + offset) +
                                       b_array[sample_num])
                 feh_mapped_array[sample_num][integal_piece] = feh_mapped_1sample
 
         # pickle plot info
         self.pickle_plot_info(name_star,
                               feh_mapped_array,
                               write_pickle_subdir=self.write_pickle_subdir)
 
-        print("Elapsed time:")
-        print(str(time.time() - time_start))
-        print("--------------------------")
+        logging.info("Elapsed time:")
+        logging.info(str(time.time() - time_start))
+        logging.info("--------------------------")
 
 
     def do(self):
 
         # do the bootstrap
         global m_array # have to make this global for multiprocessing to work
         global b_array
         m_array, b_array, params_list_star_feh, data_1 = self.do_bootstrap()
 
         # parallel process the Fe/H info
-        #ncpu = multiprocessing.cpu_count()
-        pool = Pool(ncpu)
+        # explicit syntax necessary for Macbook M1
+        pool = get_context("fork").Pool(ncpu)
         outdat = pool.map(self.map_feh_one_star, params_list_star_feh) # FeH info is pickled here
         pool.close()
 
         # now make and save the plots of Fe/H values
         # (this is done in series to avoid memory chokes)
         for t in range(0, len(data_1["star_name"])):
             this_star = data_1["star_name"][t]
-            print("Writing Fe/H CDF for star " + this_star)
+            logging.info("Writing Fe/H CDF for star " + this_star)
             self.write_cdf_hist_plot(this_star)
```

### Comparing `rrlfe-0.0.9/modules/norm_spec.py` & `rrlfe-1.0/rrlfe/norm_spec.py`

 * *Files 10% similar despite different names*

```diff
@@ -35,16 +35,14 @@
         # run the normalization routine on the data
         normzn_run1 = shlex.split("./bkgrnd --smooth "+str(self.smoothing)+" "+self.input_file) # self.input_file can be 'in.data'
         normzn_run2 = subprocess.Popen(normzn_run1, stdout=subprocess.PIPE, stderr=subprocess.PIPE) # run and capture output
                                   
         # make list of all output files put out by Robospect
         dir_name = "test_robo_output/"
         list_output_files = [name for name in os.listdir(dir_name) if os.path.isfile(os.path.join(dir_name, name))]
-        print(list_output_files)
-        print('--')
                                   
         # divide the second column of the output files (empirical) with the third (normalization) 
         header = ['WAVELENGTH', 'FLUX'] # headers of output file that Robospect will use (see Robospect user manual)
         for filenum in range(0,len(list_output_files)):
             df = pd.read_csv(dir_name + str(list_output_files[filenum]), delim_whitespace=True, header=None)
             df['WAVELENGTH'] = df[0]
             df['FLUX'] = np.divide(df[1],df[2]) # normalize
```

### Comparing `rrlfe-0.0.9/modules/scrape_ew_and_errew.py` & `rrlfe-1.0/rrlfe/scrape_ew_and_errew.py`

 * *Files 24% similar despite different names*

```diff
@@ -12,20 +12,27 @@
 from astropy.io.fits import getdata
 #import matplotlib # kernel needs to be restarted to avoid TkAgg error
 #matplotlib.use('TkAgg')
 import matplotlib.pyplot as plt
 import matplotlib.pylab as pl
 from . import *
 
+
 def line_order_check(line_centers):
-    '''
-    Sanity check: are the lines listed in order?
+    """
+    Sanity check that the absorption lines are listed in order
     N.b. This checks the wavelengths using the given line list
     values (and not the fitted centers)
-    '''
+
+    Parameters:
+        line_centers (array of floats): array of measured line centers
+
+    Returns:
+        int of number of apparent bad line centers
+    """
 
     logging.info('Verifying line centers...')
     logging.info(line_centers[0])
     glitch_count = int(0) # boolean for bookeeping
     if ((line_centers[0] < 3933.660-10) or
         (line_centers[0] > 3933.660+10)): # CaIIK
         logging.warning('CaIIK line center does not match!')
@@ -43,70 +50,93 @@
         logging.warning('H-gamma line center does not match!')
         glitch_count = int(1) # boolean for bookeeping
     if ((line_centers[4] < 4861.290-10) or
           (line_centers[4] > 4861.290+10)): # H-beta
         logging.warning('H-beta line center does not match!')
         glitch_count = 1 # boolean for bookeeping
     if (glitch_count == int(0)):
-        logging.info('CaIIK, H-eps, H-del, H-gam, h_beta line centers are consistent')
+        logging.info('CaIIK, H-eps, H-del, H-gam, H-beta line centers are consistent')
     return glitch_count
 
 
+
+
 class Scraper():
-    '''
-    Scrape all the equivalent width info from the Robospect *robolines files
-    '''
+    """
+    Scrape all the equivalent width info from the Robospect robolines files
+
+    Parameters:
+        module_name (str): arbitrary module name
+        orig_spec_list (list): original file names of spectra to read in
+        robo_output_read (str): directory containing Robospect output
+        file_scraped_write (str): file name of csv containing the scraped data
+
+    Returns:
+        [csv written to disk; dataframe is returned for testing only]
+    """
 
     def __init__(self,
-                 subdir=config_red["data_dirs"]["DIR_ROBO_OUTPUT"],
-                 file_scraped_info=config_red["data_dirs"]["DIR_EW_PRODS"]+config_red["file_names"]["SCRAPED_EW_ALL_DATA"],
-                 orig_spec_list = config_red["data_dirs"]["DIR_SRC"] + config_red["file_names"]["LIST_SPEC_PHASE"],
-                 verbose=False):
+        module_name,
+        input_spec_list_read,
+        robo_output_read,
+        file_scraped_write):
+
+        self.name = module_name
+        self.orig_spec_list = input_spec_list_read
+        self.robo_output_read = robo_output_read
+        self.file_scraped_info = file_scraped_write
 
-        '''
-        INPUTS:
-        subdir:
-        file_scraped_info:
-        orig_spec_list: the file containing the original file names of the spectra
-        '''
+    def run_step(self, attribs = None):
+
+        verbose=False
 
         # directory containing the *.fits.robolines
         # files with the EW info
-        self.stem = '.' ## ##
+        stem = '.' ## ##
         # subdirectory containing the *.c.dat files
-        self.subdir = subdir ## ##
+        subdir = self.robo_output_read
 
         # get list of filenames without the path
-        ## ## note the string being sought here is specific to RW's synthetic spectra; this is a weakness here and needs to be fixed later!
-        file_list_long = glob.glob(self.subdir+'/'+'*robolines')
+        # note the string being sought here is specific to RW's synthetic spectra; might change later
+        if os.path.isdir(subdir):
+            logging.info('Reading in Robolines output from '+str(subdir))
+        else:
+            logging.warning('Making new directory '+str(subdir)+ ' which will contain Robospect output')
+            make_dir(subdir)
+
+        file_list_long = glob.glob(subdir+'/'+'*robolines')
         file_list_unsorted = [os.path.basename(x) for x in file_list_long]
-        self.file_list = sorted(file_list_unsorted)
+        file_list = sorted(file_list_unsorted)
 
-        # read in original file names
-        input_list = pd.read_csv(orig_spec_list)
-        self.orig_spec_list = input_list["orig_spec_file_name"]
+        # read in original file names (note variable is being renamed here)
+        input_list = pd.read_csv(self.orig_spec_list)
+        orig_spec_list = input_list["orig_spec_file_name"]
 
         # EW info will get scraped into this
-        self.write_out_filename = file_scraped_info
+        write_out_filename = self.file_scraped_info
+        # check receiving directory exists in first place
+        if os.path.dirname(write_out_filename):
+            # check if directory exists
+            logging.info('File to contain scraped EW data is '+str(write_out_filename))
+        else:
+            logging.warning('Making new directory '+str(os.path.dirname(write_out_filename))+ ' which will contain EW output data')
+            make_dir(os.path.dirname(write_out_filename))
 
         # return tables of EW data?
-        self.verbose = verbose
-
-    def __call__(self):
+        verbose = verbose
 
         df_master = pd.DataFrame() # initialize
 
         # loop over all filenames of realizations of empirical spectra, extract line data
-        #import ipdb; ipdb.set_trace()
-        for t in range(0, len(self.file_list)):
+        for t in range(0, len(file_list)):
 
             # read in Robospect output
             logging.info("--------------------")
             logging.info("Reading in Robospect output from directory")
-            logging.info(self.subdir)
+            logging.info(subdir)
 
             '''
             The following parses lines from Robospect *robolines output files,
             which look like the following, as of the v0.76 tag of Robospect:
 
             ## Units
             ##AA      [ AA           AA             None]        [ AA             AA                None]             [ AA           AA          None]       mAA        mAA             None      None     None       None
@@ -115,456 +145,604 @@
             3933.6600 [ 3933.618556  1.636451       -0.338310]   [ 0.043767       0.045441          0.008054]         [ 3934.427147  1.754001    0.384793]   1.387738   0.127230        0.004045  0x10020  0          CaII-K
             3970.0750 [ 3969.912002  6.497202       -0.626854]   [ 0.245555       0.237816          0.023196]         [ 3971.262223  4.535872    0.781687]   10.208984  1.331932        0.117392  0x10020  0          H-eps
             4101.7100 [ 4101.728498  6.829899       -0.596311]   [ 0.335244       0.327236          0.025288]         [ 4102.885050  4.878668    0.734648]   10.208852  1.637334        0.220112  0x10020  0          H-del
             4340.4720 [ 4340.374387  7.365172       -0.557777]   [ 0.395447       0.378434          0.025443]         [ 4340.943149  4.961159    0.689719]   10.297539  1.773505        0.300238  0x10020  0          H-gam
             4861.2900 [ 4861.316520  7.570797       -0.505060]   [ 0.441626       0.426212          0.025690]         [ 4861.746895  4.898021    0.635582]   9.584604   1.822847        0.377350  0x10020  0          H-beta
             '''
 
-            df = pd.read_csv(self.subdir+'/'+self.file_list[t],
+            df = pd.read_csv(subdir+'/'+file_list[t],
                              skiprows=19,
                              delim_whitespace=True,
                              index_col=False,
                              usecols=[0,1,2,3,4,5,6,7,8,9,10,11,12,13,14,15,16,17,18],
                              names=  ["wavel_stated_center","[1","wavel_found_center","gaussianSigma","gaussianAmp",
                                         "[2","uncertaintyMu","uncertaintySigma","uncertaintyAmp",
                                         "[3","priorMu","priorSigma","priorAmp","EQW","uncertaintyEQW",
                                         "chiSqr","flags","blendGroup","line_name"])
+
             # remove dummy columns
             df = df.drop(columns=["[1","[2","[3"])
             # remove Robospect delimiter strings from columns and cast contents as floats
-            logging.info("Parsing " + self.file_list[t])
+            logging.info("Parsing " + file_list[t])
             try:
                 # this will fail if there are infs in the EWs
-                df["gaussianAmp"] = df["gaussianAmp"].str.replace("]","")
-                df["gaussianAmp"] = df["gaussianAmp"].astype(np.float)
-                df["uncertaintyAmp"] = df["uncertaintyAmp"].str.replace("]","")
-                df["uncertaintyAmp"] = df["uncertaintyAmp"].astype(np.float)
-                df["priorAmp"] = df["priorAmp"].str.replace("]","")
-                df["priorAmp"] = df["priorAmp"].astype(np.float)
+                df["gaussianAmp"] = df["gaussianAmp"].str.replace("]","", regex=True)
+                df["gaussianAmp"] = df["gaussianAmp"].astype(float)
+                df["uncertaintyAmp"] = df["uncertaintyAmp"].str.replace("]","", regex=True)
+                df["uncertaintyAmp"] = df["uncertaintyAmp"].astype(float)
+                df["priorAmp"] = df["priorAmp"].str.replace("]","", regex=True)
+                df["priorAmp"] = df["priorAmp"].astype(float)
             except:
                 # skip this file
-                logging.error("Parsing error! " + self.file_list[t])
+                logging.error("Parsing error! " + file_list[t])
                 continue
 
             # check lines are in the right order
             # if they are not, a warning is printed in the log
             glitches_num = line_order_check(df['wavel_found_center'])
 
             # add two cols on the left: the filename, and the name of the line
             #s_length = len(df['mean']) # number of lines (should be 5)
 
             # file names
-            df['robolines_file_name'] = pd.Series(self.file_list[t],
+            df['robolines_file_name'] = pd.Series(file_list[t],
                                         index=df.index)
 
             # names of empirical spectra realizations (multiple ones
             # correspond to one empirical spectrum)
             # remove .robolines extension
-            df['realization_spec_file_name'] = pd.Series(self.file_list[t].split(".robolines")[0],
+            df['realization_spec_file_name'] = pd.Series(file_list[t].split(".robolines")[0],
                                               index=df.index)
 
             # names of the absorption lines
             df['line_name'] = ['CaIIK', 'Heps', 'Hdel', 'Hgam', 'Hbet']
 
             # print progress
-            logging.info('Out of '+str(len(self.file_list))+' files, '+str(t+1)+' scraped...')
+            logging.info('Out of '+str(len(file_list))+' files, '+str(t+1)+' scraped...')
 
             # if this is the first list, start a master copy from it to concatenate stuff to it
             if (t == 0):
                 df_master = df.copy()
             else:
                 df_master = pd.concat([df_master, df])
                 del df # clear variable
 
         # write to csv, while resetting the indices
         # note THIS TABLE INCLUDES ALL DATA, GOOD AND BAD
         #df_master_reset = df_master.reset_index(drop=True).copy()
         # this is effectively the same, but gets written out
-        df_master.reset_index(drop=True).to_csv(self.write_out_filename,index=False)
-        logging.info("Table of ALL EW info written to " + str(self.write_out_filename))
+        make_dir(write_out_filename) # check if write directory exists and is empty
+        df_master.reset_index(drop=True).to_csv(write_out_filename,index=False)
+        logging.info("Table of ALL EW info written to " + str(write_out_filename))
         #if self.verbose:
         #    return df_master_reset, df_master_reset_drop_bad_spectra
         # return for checking
         return df_master
 
 
-def add_synthetic_meta_data(input_list = config_red["data_dirs"]["DIR_SRC"] + config_red["file_names"]["LIST_SPEC_PHASE"],
-                            read_in_filename = config_red["data_dirs"]["DIR_EW_PRODS"]+config_red["file_names"]["RESTACKED_EW_DATA_W_NET_BALMER_ERRORS"],
-                            write_out_filename = config_red["data_dirs"]["DIR_EW_PRODS"]+config_red["file_names"]["RESTACKED_EW_DATA_W_METADATA"]):
-
-    '''
+class AddSyntheticMetaData():
+    """
     For the generation of a calibration, this reads in a file with spectrum file
     names and other info like Fe/H, and adds everything to the table with EWs
 
-    INPUTS:
-    input_list: file name of list containing original spectrum names and meta-data
-    read_in_filename: file name of table containing EW data including Balmer lines and their errors
-    write_out_filename: file name with everything together to write out
-    '''
-
-    # read in metadata
-    input_data_arr = pd.read_csv(input_list)
-
-    # read in EW data
-    all_data = pd.read_csv(read_in_filename)
-
-    # add rows of meta-data table to EW data table, based on matchings of original spectrum file names
-    combined_data = all_data.merge(input_data_arr,how="left",on="orig_spec_file_name")
-
-    # write out
-    combined_data.to_csv(write_out_filename,index=False)
-    logging.info("Table of EW info with meta-data written to " + str(write_out_filename))
-
-    # return for testing
-    return combined_data
-
-
-def quality_check(
-    read_in_filename = config_red["data_dirs"]["DIR_EW_PRODS"]+config_red["file_names"]["SCRAPED_EW_ALL_DATA"],
-    write_out_filename = config_red["data_dirs"]["DIR_EW_PRODS"]+config_red["file_names"]["SCRAPED_EW_DATA_GOOD_ONLY"]):
-    '''
-    This reads in all the scraped EW data in raw form, removes spectra that have fits
+    Parameters:
+        module_name (str): arbitrary module name
+        input_spec_list_read (str): file name of list containing original spectrum names and meta-data
+        ew_data_w_net_balmer_read (str): file name of table containing EW data including Balmer lines and their errors
+        file_w_meta_data_write (str): file name with everything together to write out
+
+    Returns:
+        [csv written to disk; dataframe is returned for testing only]
+    """
+
+    def __init__(self,
+                module_name,
+                input_spec_list_read,
+                ew_data_w_net_balmer_read,
+                file_w_meta_data_write):
+
+        self.name = module_name
+        self.input_spec_list_read = input_spec_list_read
+        self.ew_data_w_net_balmer_read = ew_data_w_net_balmer_read
+        self.file_w_meta_data_write = file_w_meta_data_write
+
+    def run_step(self, attribs = None):
+
+        input_list = self.input_spec_list_read
+        read_in_filename = self.ew_data_w_net_balmer_read
+        write_out_filename = self.file_w_meta_data_write
+
+        # read in metadata
+        logging.info("Reading in meta-data from file " + str(input_list))
+        input_data_arr = pd.read_csv(input_list)
+
+        # read in EW data
+        all_data = pd.read_csv(read_in_filename)
+
+        # add rows of meta-data table to EW data table, based on matchings of original spectrum file names
+        combined_data = all_data.merge(input_data_arr,how="left",on="orig_spec_file_name")
+
+        # write out
+        combined_data.to_csv(write_out_filename,index=False)
+        logging.info("Table of EW info with meta-data written to " + str(write_out_filename))
+
+        # return for testing
+        return combined_data
+
+
+class QualityCheck():
+    """
+    Reads in all the scraped EW data in raw form, removes spectra that have fits
     which are bad based on multiple criteria, and writes out another data_table
 
-    INPUTS:
-    read_in_filename: file name of the table with ALL scraped data from Robospect
-    write_out_filename: file name of the table with spectra with any bad line fits removed
-    '''
-
-    # read in data
-    all_data = pd.read_csv(read_in_filename)
-
-    # make new column for 'good' (G) or 'bad' (B) based on the below criteria
-    # (initialize all as 'G')
-    all_data["quality"] = "G"
-
-    # impose criteria for pruning of data
-
-    # Criterion 1. Remove all rows with a Robospect flag ending with something other than zero
-    # (i.e., Robospect found the fit to be bad)
-    # make an array consisting of the last character in each spectrum's flag
-    red_flag_array = ([u[-1] for u in all_data["flags"]])
-    # consider bad flags to be of any flag with a nonzero last character
-    where_red_flag = np.where(np.array(red_flag_array) != '0')
-    # identify the synthetic spectrum names which have at least one line with a bad fit
-    bad_robo_spectra = all_data["realization_spec_file_name"][np.squeeze(where_red_flag)]
-
-    # remove duplicate names
-    bad_robo_spectra_uniq = bad_robo_spectra.drop_duplicates()
-    # flag as bad the spectra with those names
-    all_data.loc[all_data["realization_spec_file_name"].isin(bad_robo_spectra_uniq),"quality"] = "B"
-
-    # Criterion 2. Remove rows where the line centers are not right, using steps similar to above
-    # (specifically, if measured line center is more than 10 A away from perfect center)
-    where_bad_line_center = np.where(np.abs(np.subtract(all_data["wavel_found_center"],all_data["wavel_stated_center"]) > 10))
-    bad_line_center_spectra = all_data["realization_spec_file_name"][np.squeeze(where_bad_line_center,axis=0)] # squeeze necessary to preserve finite size
-    bad_line_center_spectra_uniq = bad_line_center_spectra.drop_duplicates()
-    all_data.loc[all_data["realization_spec_file_name"].isin(bad_line_center_spectra_uniq),"quality"] = "B"
-
-    # Criterion 3. Remove rows with EWs which are clearly unrealistically large which slipped through other checks
-    # (this is particularly an issue with the CaIIK line, which is close to CaIIH)
-    # set cutoff at 18 A, based on inspection of >200 Robospect plots of fits to
-    # synthetic spectra; all those with CaIIK EW > 18 are clearly not fit right,
-    # and all those with EW < 18 look acceptable -E.S.
-    where_bad_CaIIK = np.where(np.logical_and(all_data["line_name"] == "CaIIK", all_data["EQW"] > 18))
-    bad_CaIIK_spectra = all_data["realization_spec_file_name"][np.squeeze(where_bad_CaIIK)]
-    bad_CaIIK_spectra_uniq = bad_CaIIK_spectra.drop_duplicates()
-    all_data.loc[all_data["realization_spec_file_name"].isin(bad_CaIIK_spectra_uniq),"quality"] = "B"
-
-    # Criterion 4. Remove bad phases (for empirical data)
-    '''
-    min_good, max_good = phase_regions()
-    #[...]
-    #good_indices = np.intersect1d(good_phase, good_metal)
-    #[...]
-    '''
-
-    # Last step: Write only the rows with a good ("G") flag to file
-    # (note that if AT LEAST one absorption line was found to be bad, ALL the
-    # data corresponding to that spectrum is removed)
-    pruned_data = all_data[all_data.quality == "G"]#.reset_index()
-    pruned_data.to_csv(write_out_filename,index=False)
-
-    logging.info("--------------------------")
-    logging.info('Scraped Robospect output written to')
-    logging.info(write_out_filename)
-    #import ipdb; ipdb.set_trace()
-
-    return pruned_data
-
-
-def generate_net_balmer(read_in_filename = config_red["data_dirs"]["DIR_EW_PRODS"]+config_red["file_names"]["RESTACKED_EW_DATA_GOOD_ONLY"],
-                        write_out_filename = config_red["data_dirs"]["DIR_EW_PRODS"]+config_red["file_names"]["RESTACKED_EW_DATA_W_NET_BALMER"]):
-    '''
+    Parameters:
+        module_name (str): arbitrary module name
+        file_scraped_all_read: file name of the table with ALL scraped data from Robospect
+        file_scraped_good_write: file name of the table with spectra with any bad line fits removed
+
+    Returns:
+        [csv written to disk; dataframe is returned for testing only]
+    """
+
+    def __init__(self,
+                module_name,
+                file_scraped_all_read,
+                file_scraped_good_write):
+
+        self.name = module_name
+        self.file_scraped_all_read = file_scraped_all_read
+        self.file_scraped_good_write = file_scraped_good_write
+
+    def run_step(self, attribs = None):
+
+        read_in_filename = self.file_scraped_all_read
+        write_out_filename = self.file_scraped_good_write
+
+        # read in data
+        if os.path.exists(read_in_filename):
+            # check if directory exists
+            logging.info("Reading in for quality check: " + str(read_in_filename))
+        else:
+            logging.error('File '+str(read_in_filename)+ ' which is supposed to contain scraped EW data does not exist! ')
+            exit()
+        
+        all_data = pd.read_csv(read_in_filename)
+
+        # make new column for 'good' (G) or 'bad' (B) based on the below criteria
+        # (initialize all as 'G')
+        all_data["quality"] = "G"
+
+        # impose criteria for pruning of data
+
+        # Criterion 1. Remove all rows with a Robospect flag ending with something other than zero
+        # (i.e., Robospect found the fit to be bad)
+        # make an array consisting of the last character in each spectrum's flag
+        red_flag_array = ([u[-1] for u in all_data["flags"]])
+        # consider bad flags to be of any flag with a nonzero last character
+        # and remove rows if the bad flag corresponds to CaIIK, Hgam, or Hdel
+        where_red_flag = np.where(np.logical_and(
+                                                np.array(red_flag_array) != '0',
+                                                np.logical_or(all_data["line_name"] == "CaIIK",
+                                                    np.logical_or(all_data["line_name"] == "Hgam",all_data["line_name"] == "Hdel")
+                                                    )
+                                                )
+                                )
+        # identify the synthetic spectrum names which have at least one line with a bad fit
+        bad_robo_spectra = all_data["realization_spec_file_name"][np.squeeze(where_red_flag)]
+
+        # remove duplicate names
+        try:
+            # case of >1 bad spectrum
+            bad_robo_spectra_uniq = bad_robo_spectra.drop_duplicates()
+        except:
+            bad_robo_spectra_uniq = bad_robo_spectra_uniq
+        # flag as bad the spectra with those names
+        all_data.loc[all_data["realization_spec_file_name"].isin(bad_robo_spectra_uniq),"quality"] = "B"
+
+        # Criterion 2. Remove rows where the line centers are not right, using steps similar to above
+        # (specifically, if measured line center is more than 10 A away from perfect center)
+        where_bad_line_center = np.where(np.abs(np.subtract(all_data["wavel_found_center"],all_data["wavel_stated_center"]) > 10))
+        bad_line_center_spectra = all_data["realization_spec_file_name"][np.squeeze(where_bad_line_center,axis=0)] # squeeze necessary to preserve finite size
+        bad_line_center_spectra_uniq = bad_line_center_spectra.drop_duplicates()
+        all_data.loc[all_data["realization_spec_file_name"].isin(bad_line_center_spectra_uniq),"quality"] = "B"
+
+        # Criterion 3. Remove rows with EWs which are clearly unrealistically large which slipped through other checks
+        # (this is particularly an issue with the CaIIK line, which is close to CaIIH)
+        # set cutoff at 18 A, based on inspection of >200 Robospect plots of fits to
+        # synthetic spectra; all those with CaIIK EW > 18 are clearly not fit right,
+        # and all those with EW < 18 look acceptable -E.S.
+        '''
+        where_bad_CaIIK = np.where(np.logical_and(all_data["line_name"] == "CaIIK", all_data["EQW"] > 18))
+        bad_CaIIK_spectra = all_data["realization_spec_file_name"][np.squeeze(where_bad_CaIIK)]
+        bad_CaIIK_spectra_uniq = bad_CaIIK_spectra.drop_duplicates()
+        all_data.loc[all_data["realization_spec_file_name"].isin(bad_CaIIK_spectra_uniq),"quality"] = "B"
+        '''
+
+        # Criterion 4. Remove bad phases (for empirical data)
+        '''
+        min_good, max_good = phase_regions()
+        #[...]
+        #good_indices = np.intersect1d(good_phase, good_metal)
+        #[...]
+        '''
+
+        # Last step: Write only the rows with a good ("G") flag to file
+        # (note that if AT LEAST one absorption line was found to be bad, ALL the
+        # data corresponding to that spectrum is removed)
+        pruned_data = all_data[all_data.quality == "G"]#.reset_index()
+        pruned_data.to_csv(write_out_filename,index=False)
+
+        logging.info("--------------------------")
+        logging.info('Scraped Robospect output written to')
+        logging.info(write_out_filename)
+
+        return pruned_data
+
+
+class GenerateNetBalmer():
+    """
     Takes stacked spectra data and adds a column representing a net Balmer line,
     and populates another column for the error (based on propagation of the Robo
     errors of constituent lines, and then some error propagation)
 
-    INPUTS:
-    read_in_filename: name of the file with stacked EW data from Robospect, and
-        only including 'good' data
-    write_out_filename: name of the file to be written out; identical to the file read in,
-        except that additional columns contain info on a net Balmer line
-
-    OUTPUTS:
-    (writes out csv with net Balmer line EWs)
-    [m, err_m, b, err_b], [m_1to1, err_m_1to1, b_1to1, err_b_1to1], df_poststack:
-        info used in test functions
-    '''
-
-    # read in
-    df_poststack = pd.read_csv(read_in_filename)
-
-    ####### BETWEEN HERE...
-
-    # to generate a net Balmer line, make a rescaling of Hgamma
-    # based on Hdelta
-    logging.info("Making a net Balmer line")
-
-    # get rid of *really* bad points, and make sure they're simultaneously finite
-    # (otherwise a skipped 'nan' may cause a phase shift between the two series)
-
-    idx_cond = np.logical_and(
-                            np.logical_and(df_poststack["EW_Hdelta"] > 0.5, df_poststack["EW_Hdelta"] < 20.),
-                            np.logical_and(df_poststack["EW_Hgamma"] > 0.5, df_poststack["EW_Hgamma"] < 20.)
-                            )
-
-    EW_Hgamma_good = df_poststack["EW_Hgamma"].where(idx_cond).dropna()
-    EW_Hdelta_good = df_poststack["EW_Hdelta"].where(idx_cond).dropna()
-
-    # vestigial from when we were trying to scale the lines instead of simply averaging them
-    [m, err_m, b, err_b] = [0,0,0,0]
-
-    # Propagate the error by simply doing
-    #
-    # err_W_B = sqrt ( err_W_delta^2 + err_W_gamma^2 )
-
-    # add column of net Balmer line
-    cols = ["EW_Hgamma","EW_Hdelta"]
-    df_poststack["EW_Balmer"] = df_poststack[cols].mean() # simple average; note these are all of the spectra
-    df_poststack["err_EW_Balmer_from_Robo"] = np.sqrt(
-                                                        np.add( np.power(df_poststack["err_EW_Hdelta_from_robo"],2.),
-                                                                np.power(df_poststack["err_EW_Hgamma_from_robo"],2.)
-                                                                )
-                                                        ) # sigma_B
-
-    # write out
-    df_poststack.to_csv(write_out_filename,index=False)
-    logging.info("Table with net Balmer line EWs written to " + str(write_out_filename))
-
-    # returns parameters of line fit, and DataFrame with net Balmer info
-    return [m, err_m, b, err_b], df_poststack
-
-
-def generate_addl_ew_errors(read_in_filename = config_red["data_dirs"]["DIR_EW_PRODS"]+config_red["file_names"]["RESTACKED_EW_DATA_W_NET_BALMER"],
-                            write_out_filename = config_red["data_dirs"]["DIR_EW_PRODS"]+config_red["file_names"]["RESTACKED_EW_DATA_W_NET_BALMER_ERRORS"],
-                            groupby_parent = True):
-    '''
+    Parameters:
+        module_name (str): arbitrary module name
+        file_restacked_read: name of the file with stacked EW data from Robospect, and
+            only including 'good' data
+        file_ew_net_balmer_write: name of the file to be written out; identical to the file read in,
+            except that additional columns contain info on a net Balmer line
+
+    Returns:
+        writes out csv with net Balmer line EWs, and the following for testing: [m, err_m, b, err_b], [m_1to1, err_m_1to1, b_1to1, err_b_1to1], df_poststack
+    """
+
+    def __init__(self,
+                module_name,
+                file_restacked_read,
+                file_ew_net_balmer_write):
+
+        self.name = module_name
+        self.file_restacked_read = file_restacked_read
+        self.file_ew_net_balmer_write = file_ew_net_balmer_write
+
+    def run_step(self, attribs = None):
+
+        read_in_filename = self.file_restacked_read
+        write_out_filename = self.file_ew_net_balmer_write
+
+        # read in
+        if os.path.exists(read_in_filename):
+            # check if directory exists
+            logging.info('Reading in restacked EW data from '+str(read_in_filename))
+        else:
+            logging.error('File '+str(read_in_filename)+ ' which is supposed to contain restacked EW data does not exist! ')
+            exit()
+        df_poststack = pd.read_csv(read_in_filename)
+
+        # to generate a net Balmer line, make a rescaling of Hgamma
+        # based on Hdelta
+        logging.info("Making a net Balmer line")
+
+        # get rid of *really* bad points, and make sure they're simultaneously finite
+        # (otherwise a skipped 'nan' may cause a phase shift between the two series)
+
+        idx_cond = np.logical_and(
+                                np.logical_and(df_poststack["EW_Hdelta"] > 0.5, df_poststack["EW_Hdelta"] < 20.),
+                                np.logical_and(df_poststack["EW_Hgamma"] > 0.5, df_poststack["EW_Hgamma"] < 20.)
+                                )
+
+        EW_Hgamma_good = df_poststack["EW_Hgamma"].where(idx_cond).dropna()
+        EW_Hdelta_good = df_poststack["EW_Hdelta"].where(idx_cond).dropna()
+
+        # vestigial from when we were trying to scale the lines instead of simply averaging them
+        [m, err_m, b, err_b] = [0,0,0,0]
+
+        # Propagate the error by simply doing
+        #
+        # err_W_B = sqrt ( err_W_delta^2 + err_W_gamma^2 )
+
+        # add column of net Balmer line
+        cols = ["EW_Hgamma","EW_Hdelta"]
+        df_poststack["EW_Balmer"] = df_poststack[cols].mean(axis=1) # simple average; note these are all of the spectra
+
+
+        df_poststack["err_EW_Balmer_from_robo"] = 0.5*np.sqrt(
+                                                            np.add( np.power(df_poststack["err_EW_Hdelta_from_robo"],2.),
+                                                                    np.power(df_poststack["err_EW_Hgamma_from_robo"],2.)
+                                                                    )
+                                                            ) # sigma_B
+
+        # write out
+        if os.path.exists(os.path.dirname(write_out_filename)):
+            # check if directory exists
+            logging.info("Table with net Balmer line EWs being written to " + str(write_out_filename))
+        else:
+            logging.warning('Making new directory '+str(os.path.dirname(write_out_filename))+ ' which will contain Balmer line EW file')
+            make_dir(os.path.dirname(write_out_filename))
+        df_poststack.to_csv(write_out_filename,index=False)
+        
+
+        # returns parameters of line fit, and DataFrame with net Balmer info
+        return [m, err_m, b, err_b], df_poststack
+
+
+class GenerateAddlEwErrors():
+    """
     Calculates errors in EW using the method of finding the stdev of EWs across
     a set of spectra that are realizations of the same single, original spectrum.
-    This supplements the errors produced directly by Robospect.
+    This is an alternative to the errors produced directly by Robospect.
+
+    Parameters:
+        module_name (str): arbitrary module name
+        ew_data_restacked_read (str): file name of restacked EW data to read
+        ew_data_w_net_balmer_read (str): file name of restacked EW data to read
+        groupby_parent (bool): if True, collapse noise-churned spectra into 1 after calculating the EW errors;
+            else write out a giant table containing data for all noise-churned spectra,
+            which is useful if calibration is being applied, and Fe/H will be retrieved
+            across all churnings and that will give Fe/H error
+    """
+
+    def __init__(self,
+                module_name,
+                ew_data_restacked_read,
+                ew_data_w_net_balmer_read,
+                groupby_parent=True):
+
+        self.name = module_name
+        self.ew_data_restacked_read = ew_data_restacked_read
+        self.ew_data_w_net_balmer_read = ew_data_w_net_balmer_read
+        self.groupby_parent = groupby_parent
+
+    def run_step(self, attribs = None):
+
+        read_in_filename = self.ew_data_restacked_read
+        write_out_filename = self.ew_data_w_net_balmer_read
+        groupby_parent = self.groupby_parent
+
+        df_postbalmer = pd.read_csv(read_in_filename)
+
+        # calculate errors from noise churning (may get added later)
+        '''
+        orig_specs_nonrepeating = df_postbalmer["orig_spec_file_name"].drop_duplicates().values
+        df_postbalmer["err_EW_Balmer_based_noise_churning"] = np.nan # initialize
+        df_postbalmer["err_EW_Hbeta_based_noise_churning"] = np.nan # initialize
+        df_postbalmer["err_EW_Hdelta_based_noise_churning"] = np.nan # initialize
+        df_postbalmer["err_EW_Hgamma_based_noise_churning"] = np.nan # initialize
+        df_postbalmer["err_EW_Heps_based_noise_churning"] = np.nan # initialize
+        df_postbalmer["err_EW_CaIIK_based_noise_churning"] = np.nan # initialize
+
+        for orig_spec in orig_specs_nonrepeating:
+            # loop over the parent spectra, and get stdev of EWs from each set
+            # of spectra with the same parent
+
+            # net Balmer
+            stdev_this_set_balmer = np.nanstd(df_postbalmer.where(df_postbalmer["orig_spec_file_name"] == orig_spec)["EW_Balmer"])
+            df_postbalmer.loc[(df_postbalmer["orig_spec_file_name"] == orig_spec),"err_EW_Balmer_based_noise_churning"] = stdev_this_set_balmer
+
+            # Hbeta
+            stdev_this_set_Hbeta = np.nanstd(df_postbalmer.where(df_postbalmer["orig_spec_file_name"] == orig_spec)["EW_Hbeta"])
+            df_postbalmer.loc[(df_postbalmer["orig_spec_file_name"] == orig_spec),"err_EW_Hbeta_based_noise_churning"] = stdev_this_set_Hbeta
+
+            # Hdelta
+            stdev_this_set_Hdelta = np.nanstd(df_postbalmer.where(df_postbalmer["orig_spec_file_name"] == orig_spec)["EW_Hdelta"])
+            df_postbalmer.loc[(df_postbalmer["orig_spec_file_name"] == orig_spec),"err_EW_Hdelta_based_noise_churning"] = stdev_this_set_Hdelta
+
+            # Hgamma
+            stdev_this_set_Hgamma = np.nanstd(df_postbalmer.where(df_postbalmer["orig_spec_file_name"] == orig_spec)["EW_Hgamma"])
+            df_postbalmer.loc[(df_postbalmer["orig_spec_file_name"] == orig_spec),"err_EW_Hgamma_based_noise_churning"] = stdev_this_set_Hgamma
+
+            # Hepsilon
+            stdev_this_set_Heps = np.nanstd(df_postbalmer.where(df_postbalmer["orig_spec_file_name"] == orig_spec)["EW_Heps"])
+            df_postbalmer.loc[(df_postbalmer["orig_spec_file_name"] == orig_spec),"err_EW_Heps_based_noise_churning"] = stdev_this_set_Heps
+
+            # CaIIK
+            stdev_this_set_CaIIK = np.nanstd(df_postbalmer.where(df_postbalmer["orig_spec_file_name"] == orig_spec)["EW_CaIIK"])
+            df_postbalmer.loc[(df_postbalmer["orig_spec_file_name"] == orig_spec),"err_EW_CaIIK_based_noise_churning"] = stdev_this_set_CaIIK
+
+
+        logging.info("Added column of EW errors based on stdev across noise-churned spectra")
+
+        if groupby_parent:
+            # collapse the noise-churned data such that there is only one row for each parent spectrum
+            df_postbalmer_grouped = df_postbalmer.groupby("orig_spec_file_name", as_index=False).median()
+            df_postbalmer_errors = df_postbalmer_grouped.to_csv(write_out_filename, index=False)
+            logging.info("Grouped spectra by parent, and collapsed by taking median down the columns.")
+
+        else:
+            df_postbalmer_errors = df_postbalmer.to_csv(write_out_filename, index=False)
+            logging.info("Did not group spectra by parent; table with all noise churnings will be written out.")
+        '''
+
+
+        # calculate EW errors based on linear fit to 
+        # std of EW returned by Robo (y) vs err of EW returned by Robo (x)
+        def scale_robo_err_to_err(robo_err):
+        
+            poly_fit_stdvsRobo = np.array([0.04154731,0.44331584]) # fit coeffs
+
+            err = np.multiply(poly_fit_stdvsRobo[0],robo_err) + poly_fit_stdvsRobo[1]
 
-    groupby_parent: collapse noise-churned spectra into 1 after calculating the EW errors;
-        else write out a giant table containing data for all noise-churned spectra,
-        which is useful if calibration is being applied, and Fe/H will be retrieved
-        across all churnings and that will give Fe/H error
-    '''
-
-    #df_poststack = error_scatter_ew(df_poststack)
-    df_postbalmer = pd.read_csv(read_in_filename)
-
-    orig_specs_nonrepeating = df_postbalmer["orig_spec_file_name"].drop_duplicates().values
-    df_postbalmer["err_EW_Balmer_based_noise_churning"] = np.nan # initialize
-    df_postbalmer["err_EW_Hbeta_based_noise_churning"] = np.nan # initialize
-    df_postbalmer["err_EW_Hdelta_based_noise_churning"] = np.nan # initialize
-    df_postbalmer["err_EW_Hgamma_based_noise_churning"] = np.nan # initialize
-    df_postbalmer["err_EW_Heps_based_noise_churning"] = np.nan # initialize
-    df_postbalmer["err_EW_CaIIK_based_noise_churning"] = np.nan # initialize
-    for orig_spec in orig_specs_nonrepeating:
-        # loop over the parent spectra, and get stdev of EWs from each set
-        # of spectra with the same parent
-
-        # net Balmer
-        stdev_this_set_balmer = np.nanstd(df_postbalmer.where(df_postbalmer["orig_spec_file_name"] == orig_spec)["EW_Balmer"])
-        df_postbalmer.loc[(df_postbalmer["orig_spec_file_name"] == orig_spec),"err_EW_Balmer_based_noise_churning"] = stdev_this_set_balmer
-
-        # Hbeta
-        stdev_this_set_Hbeta = np.nanstd(df_postbalmer.where(df_postbalmer["orig_spec_file_name"] == orig_spec)["EW_Hbeta"])
-        df_postbalmer.loc[(df_postbalmer["orig_spec_file_name"] == orig_spec),"err_EW_Hbeta_based_noise_churning"] = stdev_this_set_Hbeta
-
-        # Hdelta
-        stdev_this_set_Hdelta = np.nanstd(df_postbalmer.where(df_postbalmer["orig_spec_file_name"] == orig_spec)["EW_Hdelta"])
-        df_postbalmer.loc[(df_postbalmer["orig_spec_file_name"] == orig_spec),"err_EW_Hdelta_based_noise_churning"] = stdev_this_set_Hdelta
-
-        # Hgamma
-        stdev_this_set_Hgamma = np.nanstd(df_postbalmer.where(df_postbalmer["orig_spec_file_name"] == orig_spec)["EW_Hgamma"])
-        df_postbalmer.loc[(df_postbalmer["orig_spec_file_name"] == orig_spec),"err_EW_Hgamma_based_noise_churning"] = stdev_this_set_Hgamma
-
-        # Hepsilon
-        stdev_this_set_Heps = np.nanstd(df_postbalmer.where(df_postbalmer["orig_spec_file_name"] == orig_spec)["EW_Heps"])
-        df_postbalmer.loc[(df_postbalmer["orig_spec_file_name"] == orig_spec),"err_EW_Heps_based_noise_churning"] = stdev_this_set_Heps
-
-        # CaIIK
-        stdev_this_set_CaIIK = np.nanstd(df_postbalmer.where(df_postbalmer["orig_spec_file_name"] == orig_spec)["EW_CaIIK"])
-        df_postbalmer.loc[(df_postbalmer["orig_spec_file_name"] == orig_spec),"err_EW_CaIIK_based_noise_churning"] = stdev_this_set_CaIIK
-
-
-    logging.info("Added column of EW errors based on stdev across noise-churned spectra")
-
-    if groupby_parent:
-        # collapse the noise-churned data such that there is only one row for each parent spectrum
-        df_postbalmer_grouped = df_postbalmer.groupby("orig_spec_file_name", as_index=False).median()
-        df_postbalmer_errors = df_postbalmer_grouped.to_csv(write_out_filename, index=False)
-        logging.info("Grouped spectra by parent, and collapsed by taking median down the columns.")
-
-    else:
-        df_postbalmer_errors = df_postbalmer.to_csv(write_out_filename, index=False)
-        logging.info("Did not group spectra by parent; table with all noise churnings will be written out.")
-
-    logging.info("Wrote table out to " + str(write_out_filename))
-
-
-    '''
-    logging.info("------------------------------")
-    #logging.info("Data will be written out to file " + write_out_filename)
-    #input("Hit [Enter] to continue")
-    logging.info("Writing out re-casting of Robospect EWs and rescaled Balmer line to " + write_out_filename)
-    df_poststack.to_csv(write_out_filename)
-    '''
-
-    # FYI plot: how do Balmer lines scale with each other?
-    '''
-    plt.clf()
-    plt.title("Scaling of lines with Hdelta")
-    plt.scatter(df_poststack["EW_Hdelta"],df_poststack["EW_Hbeta"], s=3, label="Hbeta")
-    plt.scatter(df_poststack["EW_Hdelta"],np.add(df_poststack["EW_Hgamma"],4), s=3, label="Hgamma+4")
-    plt.scatter(df_poststack["EW_Hdelta"],np.add(df_poststack["EW_Heps"],8), s=3, label="Heps+8")
-    #plt.ylim([0,15])
-    plt.xlabel("EW, Hdelta (Angstr)")
-    plt.ylabel("EW, non-Hdelta (Angstr)")
-    plt.legend()
-    plt.savefig("junk_balmer_rescalings.pdf")
-
-    # FYI plot: KH plot
-    plt.clf()
-    plt.title("KH plot")
-    plt.errorbar(df_poststack["EW_resc_Hgamma"],df_poststack["EW_CaIIK"],
-                 yerr=df_poststack["err_EW_CaIIK_from_robo"],
-                 marker="o", markersize=2, mfc="k", mec="k", ecolor="gray", linestyle="")
-    plt.ylim([0,30])
-    plt.xlabel("EW, net Balmer (Angstr)")
-    plt.ylabel("EW, CaIIK (Angstr)")
-    plt.savefig("junk_KH_plot.pdf")
-    '''
-
-    # return dataframe for test function
-    return df_postbalmer
-
-
-def stack_spectra(
-    read_in_filename = config_red["data_dirs"]["DIR_EW_PRODS"]+config_red["file_names"]["SCRAPED_EW_DATA_GOOD_ONLY"],
-    write_out_filename = config_red["data_dirs"]["DIR_EW_PRODS"]+config_red["file_names"]["RESTACKED_EW_DATA_GOOD_ONLY"],
-    input_list = config_red["data_dirs"]["DIR_SRC"] + config_red["file_names"]["LIST_SPEC_PHASE"]):
-    '''
+            return err
+
+        df_postbalmer['err_EW_Balmer_scaled'] = scale_robo_err_to_err(df_postbalmer['err_EW_Balmer_from_robo'])
+        df_postbalmer['err_EW_CaIIK_scaled'] = scale_robo_err_to_err(df_postbalmer['err_EW_CaIIK_from_robo'])
+
+        df_postbalmer.to_csv(write_out_filename, index=False)
+        logging.info("Wrote table out to " + str(write_out_filename))
+
+        '''
+        logging.info("------------------------------")
+        #logging.info("Data will be written out to file " + write_out_filename)
+        #input("Hit [Enter] to continue")
+        logging.info("Writing out re-casting of Robospect EWs and rescaled Balmer line to " + write_out_filename)
+        df_poststack.to_csv(write_out_filename)
+        '''
+
+        # FYI plot: how do Balmer lines scale with each other?
+        '''
+        plt.clf()
+        plt.title("Scaling of lines with Hdelta")
+        plt.scatter(df_poststack["EW_Hdelta"],df_poststack["EW_Hbeta"], s=3, label="Hbeta")
+        plt.scatter(df_poststack["EW_Hdelta"],np.add(df_poststack["EW_Hgamma"],4), s=3, label="Hgamma+4")
+        plt.scatter(df_poststack["EW_Hdelta"],np.add(df_poststack["EW_Heps"],8), s=3, label="Heps+8")
+        #plt.ylim([0,15])
+        plt.xlabel("EW, Hdelta (Angstr)")
+        plt.ylabel("EW, non-Hdelta (Angstr)")
+        plt.legend()
+        plt.savefig("junk_balmer_rescalings.pdf")
+
+        # FYI plot: KH plot
+        plt.clf()
+        plt.title("KH plot")
+        plt.errorbar(df_poststack["EW_resc_Hgamma"],df_poststack["EW_CaIIK"],
+                     yerr=df_poststack["err_EW_CaIIK_from_Robo"],
+                     marker="o", markersize=2, mfc="k", mec="k", ecolor="gray", linestyle="")
+        plt.ylim([0,30])
+        plt.xlabel("EW, net Balmer (Angstr)")
+        plt.ylabel("EW, CaIIK (Angstr)")
+        plt.savefig("junk_KH_plot.pdf")
+        '''
+
+        # return dataframe for test function
+        return df_postbalmer
+
+
+class StackSpectra():
+    """
     Takes output of quality_check() and transposes and stacks data so that the data has *rows* of spectra and *cols* of absorption lines
 
-    INPUTS:
-    read_in_filename: file name of scraped Robospect data, after removing bad spectra
-    write_out_filename: name of file to contain re-stacked data
-    input_list: list of original file names
-    '''
-
-    # read in EW data
-    df_prestack = pd.read_csv(read_in_filename)
-
-    # read in the list of original file names
-    original_names = pd.read_csv(input_list)
-
-    logging.info("--------------")
-    logging.info("Reading in spectra as listed in " + input_list)
-
-    # make list of individual spectra for which we have EW data, and
-    # initialize DataFrame to hold the re-cast data
-
-    list_indiv_spectra = list(df_prestack["realization_spec_file_name"].drop_duplicates())
-
-    num_indiv_spectra = len(list_indiv_spectra)
-
-    df_poststack = pd.DataFrame(columns=["realization_spec_file_name",
-                                         "orig_spec_file_name",
-                                         "EW_Hbeta", "err_EW_Hbeta_from_robo",
-                                         "EW_Hdelta", "err_EW_Hdelta_from_robo",
-                                         "EW_Hgamma", "err_EW_Hgamma_from_robo",
-                                         "EW_Heps", "err_EW_Heps_from_robo",
-                                         "EW_CaIIK", "err_EW_CaIIK_from_robo"], index=range(num_indiv_spectra))
-
-    for t in range(0,num_indiv_spectra):
-        # loop over all spectra realizations we have measured EWs from to populate the dataframe
-
-        this_realization_spectrum = list_indiv_spectra[t]
-        logging.info("Extracting EW data corresponding to " + this_realization_spectrum)
-
-        # extract original file name (the one from which realizations are made)
-        # loop over all the original spectrum names; which contains a string that
-        # appears in the name of the noise-churned spectrum name?
-        ## ## inelegant; determine original spectrum name later in better way
-        #for orig_num in range(0,len(original_names)):
-        condition_array = []
-
-        for this_parent_spectrum in original_names["orig_spec_file_name"]:
-            # based on naming convention where noise-churned spec is given a 'ver' name
-            # ex. (original, realization) = (700030p00.smo, 700030p00_noise_ver_009.smo)
-            trunc_name_parent_spectrum = this_parent_spectrum.split(".")[0]
-            condition_array.append(trunc_name_parent_spectrum in this_realization_spectrum)
+    Parameters:
+        module_name (str): arbitrary module name
+        input_spec_list_read (str): list of spectrum file names to read
+        file_ew_data_read (str): file name of file with EW data
+        file_restacked_write (str): file name of restacked data
+
+    Returns:
+        [writes out csv with stacked data, and returns it for testing only]
+    """
 
-        try:
-            orig_name = original_names[condition_array]["orig_spec_file_name"].values[0]
-        except: # pragma: no cover
-            # sanity check: if strings are not shared, abort
-            input("Spectrum file strings don't match!!")
-        #import ipdb; ipdb.set_trace()
-
-        # select data from table relevant to this spectrum realization
-        data_this_spectrum = df_prestack.where(df_prestack["realization_spec_file_name"] == this_realization_spectrum).dropna().reset_index()
-        #orig_name = original_names[condition_array]["orig_spec_file_name"].values[0]
+    def __init__(self,
+                module_name,
+                input_spec_list_read,
+                file_ew_data_read,
+                file_restacked_write):
+
+        self.name = module_name
+        self.input_list_read = input_spec_list_read
+        self.file_ew_data_read = file_ew_data_read
+        self.file_restacked_write = file_restacked_write
+
+    def run_step(self, attribs = None):
+
+        read_in_filename = self.file_ew_data_read
+        write_out_filename = self.file_restacked_write
+        input_list = self.input_list_read
+
+        # read in EW data
+        if os.path.exists(read_in_filename):
+            logging.info('Reading in file with good EW data from '+str(read_in_filename))
+        else:
+            logging.error('File '+str(read_in_filename)+ ' which is supposed to contain background good EW data does not exist! ')
+            exit()
+        df_prestack = pd.read_csv(read_in_filename)
+
+        print('--------')
+        #print(read_in_filename)
+        print(df_prestack)
+        print('--------')
+        #print('Reading in original input spectrum file list from '+str(input_list))
+
+        # read in the list of original file names
+        if os.path.exists(input_list):
+            logging.info('Reading in original input spectrum file list from '+str(input_list))
+        else:
+            logging.error('File '+str(input_list)+ ' which is supposed to contain original spectrum file names does not exist! ')
+            exit()
+        original_names = pd.read_csv(input_list)
+
+        logging.info("--------------")
+        logging.info("Reading in spectra as listed in " + input_list)
+
+        # make list of individual spectra for which we have EW data, and
+        # initialize DataFrame to hold the re-cast data
+
+        list_indiv_spectra = list(df_prestack["realization_spec_file_name"].drop_duplicates())
+
+        print(df_prestack["realization_spec_file_name"])
+        print(list_indiv_spectra)
+
+        num_indiv_spectra = len(list_indiv_spectra)
+
+        df_poststack = pd.DataFrame(columns=["realization_spec_file_name",
+                                             "orig_spec_file_name",
+                                             "EW_Hbeta", "err_EW_Hbeta_from_robo",
+                                             "EW_Hdelta", "err_EW_Hdelta_from_robo",
+                                             "EW_Hgamma", "err_EW_Hgamma_from_robo",
+                                             "EW_Heps", "err_EW_Heps_from_robo",
+                                             "EW_CaIIK", "err_EW_CaIIK_from_robo"], index=range(num_indiv_spectra))
+
+        for t in range(0,num_indiv_spectra):
+            # loop over all spectra realizations we have measured EWs from to populate the dataframe
+
+            this_realization_spectrum = list_indiv_spectra[t]
+            logging.info("Extracting EW data corresponding to " + this_realization_spectrum)
+
+            # extract original file name (the one from which realizations are made)
+            # loop over all the original spectrum names; which contains a string that
+            # appears in the name of the noise-churned spectrum name?
+            condition_array = []
+
+            for this_parent_spectrum in original_names["orig_spec_file_name"]:
+                # based on naming convention where noise-churned spec is given a 'ver' name
+                # ex. (original, realization) = (700030p00.smo, 700030p00_noise_ver_009.smo)
+                trunc_name_parent_spectrum = this_parent_spectrum.split(".")[0]
+                condition_array.append(trunc_name_parent_spectrum in this_realization_spectrum)
 
-        try:
-            # extract Balmer lines from the table of data for this specific spectrum realization
-            Hbeta = data_this_spectrum["EQW"].where(data_this_spectrum["line_name"] == "Hbet").dropna().values[0]
-            err_Hbeta = data_this_spectrum["uncertaintyEQW"].where(data_this_spectrum["line_name"] == "Hbet").dropna().values[0]
-
-            Hgamma = data_this_spectrum["EQW"].where(data_this_spectrum["line_name"] == "Hgam").dropna().values[0]
-            err_Hgamma = data_this_spectrum["uncertaintyEQW"].where(data_this_spectrum["line_name"] == "Hgam").dropna().values[0]
-
-            Hdelta = data_this_spectrum["EQW"].where(data_this_spectrum["line_name"] == "Hdel").dropna().values[0]
-            err_Hdelta = data_this_spectrum["uncertaintyEQW"].where(data_this_spectrum["line_name"] == "Hdel").dropna().values[0]
-
-            Heps = data_this_spectrum["EQW"].where(data_this_spectrum["line_name"] == "Heps").dropna().values[0]
-            err_Heps = data_this_spectrum["uncertaintyEQW"].where(data_this_spectrum["line_name"] == "Heps").dropna().values[0]
-
-            CaIIK = data_this_spectrum["EQW"].where(data_this_spectrum["line_name"] == "CaIIK").dropna().values[0]
-            err_CaIIK = data_this_spectrum["uncertaintyEQW"].where(data_this_spectrum["line_name"] == "CaIIK").dropna().values[0]
-
-            # fill in that row in the dataframe
-            df_poststack.iloc[t]["realization_spec_file_name"] = this_realization_spectrum
-            df_poststack.iloc[t]["orig_spec_file_name"] = orig_name
-            df_poststack.iloc[t]["EW_Hbeta"] = Hbeta
-            df_poststack.iloc[t]["err_EW_Hbeta_from_robo"] = err_Hbeta
-            df_poststack.iloc[t]["EW_Hdelta"] = Hdelta
-            df_poststack.iloc[t]["err_EW_Hdelta_from_robo"] = err_Hdelta
-            df_poststack.iloc[t]["EW_Hgamma"] = Hgamma
-            df_poststack.iloc[t]["err_EW_Hgamma_from_robo"] = err_Hgamma
-            df_poststack.iloc[t]["EW_Heps"] = Heps
-            df_poststack.iloc[t]["err_EW_Heps_from_robo"] = err_Heps
-            df_poststack.iloc[t]["EW_CaIIK"] = CaIIK
-            df_poststack.iloc[t]["err_EW_CaIIK_from_robo"] = err_CaIIK
-
-        except: # pragma: no cover
-            logging.error("Data stacking error in data for " + this_realization_spectrum)
-            logging.error("Data anomaly; skipping " + this_realization_spectrum)
-            #import ipdb; ipdb.set_trace()
-    #import ipdb; ipdb.set_trace()
-    # save intermediary table of data, before adding rescaled Balmer line
-    logging.info("Writing out intermediary file of stacked Robospect EWs and rescaled Balmer lines to " + write_out_filename)
-    df_poststack.to_csv(write_out_filename,index=False)
+            try:
+                orig_name = original_names[condition_array]["orig_spec_file_name"].values[0]
+            except: # pragma: no cover
+                # sanity check: if strings are not shared, skip and move to next spectrum
+                logging.warning("Spectrum file strings don't match!! Skipping " + this_realization_spectrum)
+
+            # select data from table relevant to this spectrum realization
+            data_this_spectrum = df_prestack.where(df_prestack["realization_spec_file_name"] == this_realization_spectrum).dropna().reset_index()
+
+            try:
+                # extract Balmer lines from the table of data for this specific spectrum realization
+                Hbeta = data_this_spectrum["EQW"].where(data_this_spectrum["line_name"] == "Hbet").dropna().values[0]
+                err_Hbeta = data_this_spectrum["uncertaintyEQW"].where(data_this_spectrum["line_name"] == "Hbet").dropna().values[0]
+
+                Hgamma = data_this_spectrum["EQW"].where(data_this_spectrum["line_name"] == "Hgam").dropna().values[0]
+                err_Hgamma = data_this_spectrum["uncertaintyEQW"].where(data_this_spectrum["line_name"] == "Hgam").dropna().values[0]
+
+                Hdelta = data_this_spectrum["EQW"].where(data_this_spectrum["line_name"] == "Hdel").dropna().values[0]
+                err_Hdelta = data_this_spectrum["uncertaintyEQW"].where(data_this_spectrum["line_name"] == "Hdel").dropna().values[0]
+
+                Heps = data_this_spectrum["EQW"].where(data_this_spectrum["line_name"] == "Heps").dropna().values[0]
+                err_Heps = data_this_spectrum["uncertaintyEQW"].where(data_this_spectrum["line_name"] == "Heps").dropna().values[0]
+
+                CaIIK = data_this_spectrum["EQW"].where(data_this_spectrum["line_name"] == "CaIIK").dropna().values[0]
+                err_CaIIK = data_this_spectrum["uncertaintyEQW"].where(data_this_spectrum["line_name"] == "CaIIK").dropna().values[0]
+
+                # fill in that row in the dataframe
+                df_poststack.iloc[t]["realization_spec_file_name"] = this_realization_spectrum
+                df_poststack.iloc[t]["orig_spec_file_name"] = orig_name
+                df_poststack.iloc[t]["EW_Hbeta"] = Hbeta
+                df_poststack.iloc[t]["err_EW_Hbeta_from_robo"] = err_Hbeta
+                df_poststack.iloc[t]["EW_Hdelta"] = Hdelta
+                df_poststack.iloc[t]["err_EW_Hdelta_from_robo"] = err_Hdelta
+                df_poststack.iloc[t]["EW_Hgamma"] = Hgamma
+                df_poststack.iloc[t]["err_EW_Hgamma_from_robo"] = err_Hgamma
+                df_poststack.iloc[t]["EW_Heps"] = Heps
+                df_poststack.iloc[t]["err_EW_Heps_from_robo"] = err_Heps
+                df_poststack.iloc[t]["EW_CaIIK"] = CaIIK
+                df_poststack.iloc[t]["err_EW_CaIIK_from_robo"] = err_CaIIK
+
+            except: # pragma: no cover
+                logging.error("Data stacking error in data for " + this_realization_spectrum)
+                logging.error("Data anomaly; skipping " + this_realization_spectrum)
+
+        # save intermediary table of data, before adding rescaled Balmer line
+        logging.info("Writing out intermediary file of stacked Robospect EWs and rescaled Balmer lines to " + write_out_filename)
+        df_poststack.to_csv(write_out_filename,index=False)
 
-    return df_poststack
+        return df_poststack
```

### Comparing `rrlfe-0.0.9/modules/covars.py` & `rrlfe-1.0/rrlfe/covars.py`

 * *Files identical despite different names*

### Comparing `rrlfe-0.0.9/modules/manually_remove_points_spectra.py` & `rrlfe-1.0/rrlfe/manually_remove_points_spectra.py`

 * *Files identical despite different names*

### Comparing `rrlfe-0.0.9/modules/interpolate_spectra_masked_regions.py` & `rrlfe-1.0/rrlfe/interpolate_spectra_masked_regions.py`

 * *Files identical despite different names*

### Comparing `rrlfe-0.0.9/modules/sift_manual_spectra.py` & `rrlfe-1.0/rrlfe/sift_manual_spectra.py`

 * *Files 10% similar despite different names*

```diff
@@ -32,15 +32,14 @@
     fig = plt.figure(figsize=(20,10))
     plt.imshow(img)
     plt.show()
 
     choice = input("[d]isc/[g]ood/[c]osmic: ")
 
     plt.clf()
-    #import ipdb; ipdb.set_trace()
 
     dat_file_name = os.path.basename(file_list[file_num]).split(".")[-2]+".dat"
     if choice == "d":
         disc.write(dat_file_name+"\n")
         disc.close()
     elif choice == "g":
         norays.write(dat_file_name+"\n")
```

### Comparing `rrlfe-0.0.9/modules/consolidate_pre_mcmc.py` & `rrlfe-1.0/rrlfe/consolidate_pre_mcmc.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,55 +4,50 @@
 
 import glob
 import sys
 import pickle
 import numpy as np
 import pandas as pd
 from pylab import *
-from IPython.display import clear_output
 from . import *
 
 
-def graft_feh(pickle_source_dir=config_red["data_dirs"]["DIR_PICKLE"],
-              stars_and_offsets_info_file=config_red["file_names"]["RRAB_RRAB_OFFSETS"],
-              hk_source_dir=config_red["data_dirs"]["DIR_SRC"],
+def graft_feh(pickle_source_dir,
+              stars_and_offsets_info_file,
+              hk_source_dir,
               synthetic=False):
-    '''
+    """
     Read in the EW and phase data, and attach Fe/H values
 
-    INPUTS:
-    pickle_source_dir: source directory of pickled mapped Fe/H data
-    stars_and_offsets_info_file: file name of star subtypes and their offsets
-    hk_source_dir: source directory for HK info
-    synthetic:
-        =False: the Fe/H will be derived from the basis
-        =True: the Fe/H will be extracted from the file name
-
-    OUTPUTS:
-    (written pickle file of EW and Fe/H values for each star)
-    '''
-
-    ## ## TACK PHASES ONTO LIST OF EWS FROM SPECTRA
-    ## ## NEED TO GET RID OF THE 'FAKE' AT SOME POINT
+    Parameters:
+        pickle_source_dir (str): source directory of pickled mapped Fe/H data
+        stars_and_offsets_info_file (str): file name of star subtypes and their offsets
+        hk_source_dir (str): source directory for HK info
+        synthetic (bool):
+            =False: the Fe/H will be derived from the basis
+            =True: the Fe/H will be extracted from the file name
+
+    Returns:
+        [text file of EW and Fe/H values for each star written to disk]
+    """
 
     if not synthetic:
         # read in star names first
-        ## ## N.b. this is just the RRabs with RRab offsets for now
+        # N.b. this is just the RRabs with RRab offsets for now
         real_data_1 = pickle.load( open(pickle_source_dir  +
                                     stars_and_offsets_info_file, "rb" ) )
 
         # arrange the data in a way we can use
         # N.b. This is NOT fake data; I'm just appropriating the old variable name
-        ## ## Note the ersatz Layden errors for now; need to revisit this with values from his paper
+        # Note the placeholder Layden errors for now
         data_1 = { "star_name": real_data_1[0]["name_star"],
                 "feh_lit": real_data_1[0]["feh_highres"],
                 "feh_layden": real_data_1[0]["feh_basis"],
                 "err_feh_lit": np.zeros(len(real_data_1[0]["feh_basis"])),
                 "err_feh_layden": 0.07*np.ones(len(real_data_1[0]["feh_basis"]))}
-        #dataset_1 = pd.DataFrame(data=data_1)
 
         # loop over each star to read in the calculated metallicities
         final_star_feh = pd.DataFrame(columns=["star_name",
                                            "final_feh_center",
                                            "final_feh_lower",
                                            "final_feh_upper"])
         for t in range(0, len(data_1["star_name"])):
@@ -75,67 +70,61 @@
             final_star_feh = final_star_feh.append({"star_name_underscore": name_star_underscore,
                                                "final_feh_center": this_feh_center,
                                                "final_feh_lower": this_feh_lower,
                                                "final_feh_upper": this_feh_upper},
                                                ignore_index=True)
 
     # read in the EW and phase info
-    hk_ews = pd.read_csv(hk_source_dir + config_red["file_names"]["MORE_REALISTIC"])
-    #import ipdb; ipdb.set_trace()
+    hk_ews = pd.read_csv(hk_source_dir + config_choice["file_names"]["MORE_REALISTIC"])
+
     # paste the feh values onto the HK table
     # loop over each row of the HK table and assign an FeH based
     # on string in empirical spectrum name
     hk_ews["final_feh_center"] = np.nan
     hk_ews["final_feh_lower"] = np.nan
     hk_ews["final_feh_upper"] = np.nan
     hk_ews["Teff"] = np.nan
     hk_ews["logg"] = np.nan
 
     # loop over each star name (of which our program stars are a subset)
     # and paste the FeH values to the HK table rows corresponding to the
     # empirical spectra for that star
     if not synthetic:
-        print("Filling in Fe/H values for empirical spectra")
+        logging.info("Filling in Fe/H values for empirical spectra")
         for star_num in range(0, len(final_star_feh["star_name_underscore"])):
             this_star = final_star_feh["star_name_underscore"][star_num]
-            print("Retrieving calculated Fe/H value for " + this_star)
+            logging.info("Retrieving calculated Fe/H value for " + this_star)
             feh_center_this_star = final_star_feh["final_feh_center"][star_num]
             feh_lower_this_star = final_star_feh["final_feh_lower"][star_num]
             feh_upper_this_star = final_star_feh["final_feh_upper"][star_num]
 
             # loop over each of our program stars; i.e., empirical spectra
             for em_spec_num in range(0, len(hk_ews["original_spec_file_name"])):
 
                 # if the star assigned to an FeH value appears in the empirical spectrum name
                 if (this_star in hk_ews["original_spec_file_name"][em_spec_num]):
-                    print("this_star is in hk_ews")
                     hk_ews["final_feh_center"].iloc[em_spec_num] = feh_center_this_star
                     hk_ews["final_feh_lower"].iloc[em_spec_num] = feh_lower_this_star
                     hk_ews["final_feh_upper"].iloc[em_spec_num] = feh_upper_this_star
 
-                #else:
-                #    print("Spectrum is not synthetic and does not appear among the program stars.")
-
     # if these are synthetic spectra
     elif synthetic:
-        print("Filling in Fe/H values for synthetic spectra")
+        logging.info("Filling in Fe/H values for synthetic spectra")
 
         # read in FeH values
-        feh_info = pd.read_csv(hk_source_dir + config_red["file_names"]["LIST_SPEC_PHASE"],
+        feh_info = pd.read_csv(hk_source_dir + config_choice["file_names"]["LIST_SPEC_PHASE"],
                     delim_whitespace=True)
-        #print(feh_info)
-        #import ipdb; ipdb.set_trace()
+
         for synth_spec_num in range(0, len(hk_ews["original_spec_file_name"])):
-            print("Num " + str(synth_spec_num) + " out of " + str(len(hk_ews["original_spec_file_name"])))
+            logging.info("Num " + str(synth_spec_num) + " out of " + str(len(hk_ews["original_spec_file_name"])))
             this_synth_spectrum_name = hk_ews["original_spec_file_name"][synth_spec_num]
 
             # find where spectrum name in feh_info matches, and grab the FeH from there
             row_of_interest = feh_info.where(feh_info["Original_spectrum_file_name"] == this_synth_spectrum_name).dropna()
             # take FeH of zeroth location (there could be repeats)
-            #import ipdb; ipdb.set_trace()
             feh_center_this_star = row_of_interest["final_FeH"].values[0]
             err_feh_center_this_star = row_of_interest["final_err_FeH"].values[0]
             feh_lower_this_star = np.subtract(feh_center_this_star,err_feh_center_this_star)
             feh_upper_this_star = np.add(feh_center_this_star,err_feh_center_this_star)
 
             # also obtain logg and Teff
             Teff_this_star = row_of_interest["Teff"].values[0]
@@ -143,86 +132,63 @@
 
             hk_ews["final_feh_center"].iloc[synth_spec_num] = feh_center_this_star
             hk_ews["final_feh_lower"].iloc[synth_spec_num] = feh_lower_this_star
             hk_ews["final_feh_upper"].iloc[synth_spec_num] = feh_upper_this_star
             hk_ews["Teff"].iloc[synth_spec_num] = Teff_this_star
             hk_ews["logg"].iloc[synth_spec_num] = logg_this_star
 
-        #import ipdb; ipdb.set_trace()
-        ### START HERE
         # now remove the synthetic spectra with Teff<6000, Teff>7500, logg=2
         # ... this functionality should be moved
         hk_ews = hk_ews[hk_ews.Teff >= 6000]
         hk_ews = hk_ews[hk_ews.Teff <= 7500]
         hk_ews = hk_ews[hk_ews.logg > 2]
         hk_ews = hk_ews.reset_index()
-        #import ipdb; ipdb.set_trace()
-        # ... then find Fe/H abcd; this is 'infinte S/N'
-        # ... then check the spectra with xmgrace to see why there are some error large KH bars
-        # ... then put in more realistic noise and repeat
 
     # fyi
     hk_ews.to_csv('junk.csv')
 
-    #print("HK_EWS")
-    #print(hk_ews)
-
     # pickle the table of H,K,phases,Fe/H
-    ## ## NEED TO ADD STAR TYPE, TOO
-    pickle_write_name = pickle_source_dir + config_red["file_names"]["KH_FINAL_PKL"]
+    pickle_write_name = pickle_source_dir + config_choice["file_names"]["KH_FINAL_PKL"]
     with open(pickle_write_name, "wb") as f:
         pickle.dump(hk_ews, f)
-    print("-----------------------------")
-    print("Wrote HK data with Fe/H values to ")
-    print(pickle_write_name)
+    logging.info("-----------------------------")
+    logging.info("Wrote HK data with Fe/H values to ")
+    logging.info(pickle_write_name)
 
     return
 
 
-def winnow(pickle_source_dir=config_red["data_dirs"]["DIR_PICKLE"],
-                         hk_winnowed_write_dir=config_red["data_dirs"]["DIR_BIN"]):
-    '''
-    This removes the program star spectra based on criteria such as
-    1. phase (0 to 1)
+def winnow(pickle_source_dir=config_choice["data_dirs"]["DIR_PICKLE"],
+                         hk_winnowed_write_dir=config_choice["data_dirs"]["DIR_BIN"]):
+    """
+    Removes the program star spectra based on criteria such as \n
+    1. phase (0 to 1) \n
     2. star subtype (ab, c)
 
-    INPUTS:
-    pickle_source_dir: directory containing
-    hk_winnowed_write_dir: directory to which csv info on H, K is written
-    remove_rrl_subtype: RR Lyrae subtype to remove from analysis ("ab", "c", or none)
-    '''
+    Parameters:
+        pickle_source_dir (str): directory containing
+        hk_winnowed_write_dir (str): directory to which csv info on H, K is written
+        remove_rrl_subtype (str): RR Lyrae subtype to remove from analysis ("ab", "c", or none)
+
+    Returns:
+        [csv written to disk]
+    """
 
     # read in phase boundaries
     min_good, max_good = phase_regions()
 
     # restore pickle file with all the H,K data
     hk_data = pickle.load( open( pickle_source_dir +
-                                 config_red["file_names"]["KH_FINAL_PKL"], "rb" ) )
-    #hk_data_df = pd.DataFrame(hk_data)
-    #print(hk_data)
-    #print("hk_data keys:")
-    #print(hk_data.keys())
-    #print(hk_data["phase"])
-
-    # drop bad phases
-    ## ## NOTE THAT THE DROPNA HERE SEEMS TO BE DROPPING ALL ROWS WITH ANY NANS IN IT (SOME OF THE RRC FEHS ARE NANS)
-    ## ## ALSO CHECK THAT WERE NOT LOSING V535 OR V445 THROUGH SILLY NAME DIFFERENCES
+                                 config_choice["file_names"]["KH_FINAL_PKL"], "rb" ) )
+
     hk_data_winnowed = hk_data.where(np.logical_and(hk_data["phase"] > min_good,
                                                     hk_data["phase"] < max_good)).dropna().reset_index()
 
-    ## ## drop by type, too?
-    #hk_data_winnowed_phase_and_type = hk_data_winnowed_phase.where(np.logical_and(hk_data["phase"] > min_good,
-    #                                            hk_data["phase"] < max_good)).dropna().reset_index()
-    #hk_data_winnowed_phase_and_type = hk_data_winnowed_phase
-
-
-    #hk_data_winnowed_file_name = "hk_data_winnowed.csv"
-    winnowed_file_name = hk_winnowed_write_dir + config_red["file_names"]["KH_WINNOWED"]
+    winnowed_file_name = hk_winnowed_write_dir + config_choice["file_names"]["KH_WINNOWED"]
     hk_data_winnowed.to_csv(winnowed_file_name)
-    print("--------------------------")
-    print("Wrote winnowed EW data for MCMC to ")
-    print(winnowed_file_name)
-
+    logging.info("--------------------------")
+    logging.info("Wrote winnowed EW data for MCMC to ")
+    logging.info(winnowed_file_name)
 
-    ## ## NEED TO WINNOW BY STAR TYPE, TOO
+    # future possibility to winnow by star type, too
 
     return
```

### Comparing `rrlfe-0.0.9/modules/plot_utils.py` & `rrlfe-1.0/rrlfe/plot_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 '''
 Take data the pipeline has written out, and generate FYI plots
 '''
 
 def plot_isometal():
 
-    ## ## THE BELOW IS CRIBBED FROM ELSEWHERE
     # plot data points
     cmap = plt.get_cmap(name='jet')
     fig = plt.figure(figsize=(20, 10))
     ax = fig.add_subplot(111)
 
     # make set of colors/markers I can loop over
     colors = ['red', 'blue', 'orange', 'teal', 'black', 'green', 'purple']*10
@@ -27,16 +26,14 @@
             data_to_plot['star_name'] == unique_star_names[y])
         err_y_data = data_to_plot['err_K'].where(
             data_to_plot['star_name'] == unique_star_names[y])
 
         empirical_spectrum_names = data_to_plot['original_spec_file_name'].where(
             data_to_plot['star_name'] == unique_star_names[y])
 
-        #import ipdb; ipdb.set_trace()
-
         # plot, and keep the same color for each star
         #color_this_star = cmap(float(y)/len(unique_star_names))
         ax.errorbar(x_data,
                     y_data,
                     yerr=err_y_data,
                     xerr=err_x_data,
                     linestyle='',
@@ -62,25 +59,23 @@
         ax.annotate(unique_star_names[y],
                     xy=(np.array(x_data.dropna())[0],
                         np.array(y_data.dropna())[0]),
                     xytext=(np.array(x_data.dropna())[0],
                             np.array(y_data.dropna())[0]))
 
         # overplot the name of the empirical spectrum at each data point
-        #import ipdb; ipdb.set_trace()
         empirical_spectra_names_this_star = np.array(empirical_spectrum_names.dropna())
         for spec_annotate_num in range(0,len(empirical_spectra_names_this_star)):
             ax.annotate(empirical_spectra_names_this_star[spec_annotate_num],
                     xy=(np.array(x_data.dropna())[spec_annotate_num],
                         np.array(y_data.dropna())[spec_annotate_num]),
                     xytext=(np.array(x_data.dropna())[spec_annotate_num],
                             np.array(y_data.dropna())[spec_annotate_num]),
                     fontsize=6)
     '''
-    #import ipdb; ipdb.set_trace()
     # connect lines between each 'star'; that is, with the same gravity and metallicity
     df_20m10 = data_to_plot[data_to_plot['original_spec_file_name'].str.contains('20m10')].sort_values(by=["original_spec_file_name"]).reset_index()
     df_20m15 = data_to_plot[data_to_plot['original_spec_file_name'].str.contains('20m15')].sort_values(by=["original_spec_file_name"]).reset_index()
     df_20m20 = data_to_plot[data_to_plot['original_spec_file_name'].str.contains('20m20')].sort_values(by=["original_spec_file_name"]).reset_index()
     df_20m25 = data_to_plot[data_to_plot['original_spec_file_name'].str.contains('20m25')].sort_values(by=["original_spec_file_name"]).reset_index()
     df_20m30 = data_to_plot[data_to_plot['original_spec_file_name'].str.contains('20m30')].sort_values(by=["original_spec_file_name"]).reset_index()
     df_20p02 = data_to_plot[data_to_plot['original_spec_file_name'].str.contains('20p02')].sort_values(by=["original_spec_file_name"]).reset_index()
@@ -102,15 +97,14 @@
     df_25p02 = data_to_plot[data_to_plot['original_spec_file_name'].str.contains('25p02')].sort_values(by=["original_spec_file_name"]).reset_index()
     df_20m05 = data_to_plot[data_to_plot['original_spec_file_name'].str.contains('20m05')].sort_values(by=["original_spec_file_name"]).reset_index()
     df_20p00 = data_to_plot[data_to_plot['original_spec_file_name'].str.contains('20p00')].sort_values(by=["original_spec_file_name"]).reset_index()
 
     # establish color map
     n = 16
     colors = pl.cm.jet(np.linspace(0,1,n))
-    #import ipdb; ipdb.set_trace()
     # definition for making the annotation a bit simpler
     def annotate_fcn(ax_pass, stuff_2_plot):
         for spec_annotate_num in range(0,len(stuff_2_plot)):
             ax_pass.annotate(stuff_2_plot["original_spec_file_name"][spec_annotate_num],
                     xy=(stuff_2_plot["balmer"][spec_annotate_num],stuff_2_plot["K"][spec_annotate_num]),fontsize=6)
     # definition for making the dashed-line plots a bit simpler
     def dashed_line_plot(ax_pass,df_pass):
@@ -269,20 +263,14 @@
     ax.errorbar(df_30p00["balmer"], df_30p00["K"], yerr=df_30p00["err_K"], xerr=df_30p00["err_balmer"], linestyle="-", color=colors[14],
                  fmt='o', elinewidth=0.5, ecolor='k', capsize=5, capthick=0.5)
     annotate_fcn(ax,df_30p00)
     ax.errorbar(df_30p02["balmer"], df_30p02["K"], yerr=df_30p02["err_K"], xerr=df_30p02["err_balmer"], linestyle="-", color=colors[15],
                  fmt='o', elinewidth=0.5, ecolor='k', capsize=5, capthick=0.5)
     annotate_fcn(ax,df_30p02)
 
-    #import ipdb; ipdb.set_trace()
-
-
-
-
-
     plt.title('KH plot\n(unfilled markers = bad phase region)')
     plt.ylabel('CaIIK EW ($m\AA$?)')
     plt.xlabel('Balmer EW ($m\AA$?)')
     plt.tight_layout()
     plt.savefig(self.plot_write_subdir + config["file_names"]["KH_PLOT_NAME"])
 
     plt.ylim([0,20])
```

### Comparing `rrlfe-0.0.9/modules/write_masks_for_no_ray_spectra.py` & `rrlfe-1.0/rrlfe/write_masks_for_no_ray_spectra.py`

 * *Files identical despite different names*

### Comparing `rrlfe-0.0.9/modules/run_emcee.py` & `rrlfe-1.0/rrlfe/run_emcee.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,146 +7,132 @@
 import git
 import time
 import numpy as np
 import pandas as pd
 import emcee
 import corner
 import logging
+import matplotlib.pyplot as plt
 from scipy.optimize import least_squares
 from astropy.io import fits
 from . import *
 
 
-def corner_plot(model,
-                mcmc_text_output_file_name = config_red["data_dirs"]["DIR_BIN"] + config_red["file_names"]["MCMC_OUTPUT"],
-                corner_plot_putput_file_name = config_red["data_dirs"]["DIR_BIN"] + config_red["file_names"]["MCMC_CORNER"]):
-    '''
-    Reads in MCMC output and writes out a corner plot
-    '''
-
-    if (model == "abcd"):
-
-        # corner plot (requires 'storechain=True' in enumerate above)
-        test_samples = pd.read_csv(mcmc_text_output_file_name, delim_whitespace=True, nrows=5) # read in first rows to check column number
-        samples = pd.read_csv(mcmc_text_output_file_name, delim_whitespace=True, usecols=(1,2,3,4), names=["a", "b", "c", "d"])
-        fig = corner.corner(samples, labels=["$a$", "$b$", "$c$", "$d$"],
-                            quantiles=[0.16, 0.5, 0.84],
-                            title_fmt='.2f',
-                            show_titles=True,
-                            verbose=True,
-                            title_kwargs={"fontsize": 12})
-        fig.savefig(corner_plot_putput_file_name)
-        logging.info("--------------------------")
-        logging.info("Corner plot of MCMC posteriors written out to")
-        print(corner_plot_putput_file_name)
-
-        # if its necessary to read in MCMC output again
-        #data = np.loadtxt(self.mcmc_text_output, usecols=range(1,5))
-
-        # This code snippet from Foreman-Mackey's emcee documentation, v2.2.1 of
-        # https://emcee.readthedocs.io/en/stable/user/line.html#results
-        a_mcmc, b_mcmc, c_mcmc, d_mcmc = map(lambda v: (v[1], v[2]-v[1], v[1]-v[0]),
-                                             zip(*np.percentile(samples, [16, 50, 84], axis=0)))
-
-        print("--------------------------")
-        print("Coefficients a, b, c, d, and errors (see corner plot):")
-        print("coeff a: " + " ".join(map(str,a_mcmc)))
-        print("coeff b: " + " ".join(map(str,b_mcmc)))
-        print("coeff c: " + " ".join(map(str,c_mcmc)))
-        print("coeff d: " + " ".join(map(str,d_mcmc)))
-        logging.info("--------------------------")
-        logging.info("Coefficients a, b, c, d, and errors (see corner plot):")
-        logging.info("coeff a: " + " ".join(map(str,a_mcmc)))
-        logging.info("coeff b: " + " ".join(map(str,b_mcmc)))
-        logging.info("coeff c: " + " ".join(map(str,c_mcmc)))
-        logging.info("coeff d: " + " ".join(map(str,d_mcmc)))
-
-        #logging.info("--------------------------")
-        #logging.info("MCMC data written to ")
-        #logging.info(self.mcmc_text_output)
-
-
-    elif (model == "abcdfghk"):
-        # corner plot (requires 'storechain=True' in enumerate above)
-        # just first few lines to test
-        test_samples = pd.read_csv(mcmc_text_output_file_name, delim_whitespace=True, nrows=5) # read in first rows to check column number
-        samples = pd.read_csv(mcmc_text_output_file_name, delim_whitespace=True, usecols=(1,2,3,4,5,6,7,8), names=["a", "b", "c", "d", "f", "g", "h", "k"])
-        fig = corner.corner(samples, labels=["$a$", "$b$", "$c$", "$d$", "$f$", "$g$", "$h$", "$k$"],
-                            quantiles=[0.16, 0.5, 0.84],
-                            title_fmt='.2f',
-                            show_titles=True,
-                            verbose=True,
-                            title_kwargs={"fontsize": 12})
-        fig.savefig(corner_plot_putput_file_name)
-        logging.info("--------------------------")
-        logging.info("Corner plot of MCMC posteriors written out to")
-        print(str(corner_plot_putput_file_name))
+class CornerPlot():
+    """
+    Wrapper to read in MCMC output and writes out a corner plot
+
+    Parameters:
+        module_name (str): module name
+        file_name_mcmc_posterior_read (str): file name of MCMC posterior
+        plot_corner_write (str): file name of PNG to write
+
+    Returns:
+        [a few posterior test_samples for testing only, and writes PNG to disk]
+    """
 
-        # if its necessary to read in MCMC output again
-        #data = np.loadtxt(self.mcmc_text_output, usecols=range(1,5))
-
-        # This code snippet from Foreman-Mackey's emcee documentation, v2.2.1 of
-        # https://emcee.readthedocs.io/en/stable/user/line.html#results
-        a_mcmc, b_mcmc, c_mcmc, d_mcmc, f_mcmc, g_mcmc, h_mcmc, k_mcmc = map(lambda v: (v[1], v[2]-v[1], v[1]-v[0]),
-                                             zip(*np.percentile(samples, [16, 50, 84], axis=0)))
-
-        print("--------------------------")
-        print("Coefficients a, b, c, d, f, g, h, k, and errors (see corner plot):")
-        print("coeff a: " + " ".join(map(str,a_mcmc)))
-        print("coeff b: " + " ".join(map(str,b_mcmc)))
-        print("coeff c: " + " ".join(map(str,c_mcmc)))
-        print("coeff d: " + " ".join(map(str,d_mcmc)))
-        print("coeff f: " + " ".join(map(str,f_mcmc)))
-        print("coeff g: " + " ".join(map(str,g_mcmc)))
-        print("coeff h: " + " ".join(map(str,h_mcmc)))
-        print("coeff k: " + " ".join(map(str,k_mcmc)))
-        logging.info("--------------------------")
-        logging.info("Coefficients a, b, c, d, f, g, h, k, and errors (see corner plot):")
-        logging.info("coeff a: " + " ".join(map(str,a_mcmc)))
-        logging.info("coeff b: " + " ".join(map(str,b_mcmc)))
-        logging.info("coeff c: " + " ".join(map(str,c_mcmc)))
-        logging.info("coeff d: " + " ".join(map(str,d_mcmc)))
-        logging.info("coeff f: " + " ".join(map(str,f_mcmc)))
-        logging.info("coeff g: " + " ".join(map(str,g_mcmc)))
-        logging.info("coeff h: " + " ".join(map(str,h_mcmc)))
-        logging.info("coeff k: " + " ".join(map(str,k_mcmc)))
+    def __init__(self,
+                module_name,
+                file_name_mcmc_posterior_read,
+                plot_corner_write):
+
+        self.name = module_name
+        self.file_name_mcmc_posterior_read = file_name_mcmc_posterior_read
+        self.plot_corner_write = plot_corner_write
+
+    def run_step(self, attribs = None):
+
+        mcmc_text_output_file_name = self.file_name_mcmc_posterior_read
+        corner_plot_putput_file_name = self.plot_corner_write
+
+        test_samples = pd.read_csv(mcmc_text_output_file_name, delimiter = ',', nrows=5) # read in first rows to check column number
+
+        if np.shape(test_samples)[1] == 8:
+            # 9 rows: 1 index and 8 chains
+            model = "abcdfghk"
+
+        if (model == "abcdfghk"):
+
+            if os.path.dirname(corner_plot_putput_file_name):
+                # check if directory exists
+                logging.info('Corner plot file will be '+str(corner_plot_putput_file_name))
+            else:
+                logging.warning('Making new directory '+str(os.path.dirname(corner_plot_putput_file_name))+ ' which will contain corner plot')
+                make_dir(os.path.dirname(corner_plot_putput_file_name))
+        
+            # corner plot (requires 'storechain=True' in enumerate above)
+            # just first few lines to test
+            test_samples = pd.read_csv(mcmc_text_output_file_name, delimiter = ',', nrows=5) # read in first rows to check column number
+            samples = pd.read_csv(mcmc_text_output_file_name, usecols=(0,1,2,3,4,5,6,7), delimiter = ',', names=["a", "b", "c", "d", "f", "g", "h", "k"])
+            #N_remove = 1e3 # plot only 1 out of every N links of the chains
+            #samples = samples_all[samples_all.index % N_remove != 0]
+            fig = corner.corner(samples, labels=["$a$", "$b$", "$c$", "$d$", "$f$", "$g$", "$h$", "$k$"],
+                                quantiles=[0.16, 0.5, 0.84],
+                                title_fmt='.2f',
+                                show_titles=True,
+                                verbose=True,
+                                title_kwargs={"fontsize": 12})
+            fig.savefig(corner_plot_putput_file_name)
+            logging.info("--------------------------")
+            logging.info("Corner plot of MCMC posteriors written out to")
+            logging.info(str(corner_plot_putput_file_name))
+
+            # if its necessary to read in MCMC output again
+            #data = np.loadtxt(self.mcmc_text_output, usecols=range(1,5))
+
+            # This code snippet from Foreman-Mackey's emcee documentation, v2.2.1 of
+            # https://emcee.readthedocs.io/en/stable/user/line.html#results
+            a_mcmc, b_mcmc, c_mcmc, d_mcmc, f_mcmc, g_mcmc, h_mcmc, k_mcmc = map(lambda v: (v[1], v[2]-v[1], v[1]-v[0]),
+                                                 zip(*np.percentile(samples, [16, 50, 84], axis=0)))
+
+
+            logging.info("--------------------------")
+            logging.info("Coefficients a, b, c, d, f, g, h, k, and errors (see corner plot):")
+            logging.info("coeff a: " + " ".join(map(str,a_mcmc)))
+            logging.info("coeff b: " + " ".join(map(str,b_mcmc)))
+            logging.info("coeff c: " + " ".join(map(str,c_mcmc)))
+            logging.info("coeff d: " + " ".join(map(str,d_mcmc)))
+            logging.info("coeff f: " + " ".join(map(str,f_mcmc)))
+            logging.info("coeff g: " + " ".join(map(str,g_mcmc)))
+            logging.info("coeff h: " + " ".join(map(str,h_mcmc)))
+            logging.info("coeff k: " + " ".join(map(str,k_mcmc)))
 
 
-    else: # pragma: no cover
+        else: # pragma: no cover
 
-        logging.error("Error! No calibration model chosen for the MCMC posteriors!")
+            logging.error("Error! No calibration model chosen for the MCMC posteriors!")
 
-    return test_samples
+        return test_samples
 
 
 def lnprob(walker_pos_array,
            Teff_pass,
            measured_H_pass,
            measured_F_pass,
            measured_K_pass,
            err_measured_H_pass,
            err_measured_F_pass,
            err_measured_K_pass):
-    '''
+    """
     Nat log of probability density
 
-    INPUTS:
-    walker_pos_array: array of coefficients (regardless of model)
-    Teff_pass: Teff (a vestigial MCMC constant; this is NOT astrophysical Teff)
-    measured_H_pass: Balmer EW
-    measured_F_pass: [Fe/H]
-    measured_K_pass: CaIIK EW
-    err_measured_H_pass: error in Balmer EW
-    err_measured_F_pass: error in [Fe/H]
-    err_measured_K_pass: error in CaIIK EW
+    Parameters:
+        walker_pos_array (array): array of coefficients (regardless of model)
+        Teff_pass (float): Teff (a vestigial MCMC constant; this is NOT astrophysical Teff)
+        measured_H_pass (float): Balmer EW
+        measured_F_pass (float): [Fe/H]
+        measured_K_pass (float): CaIIK EW
+        err_measured_H_pass (float): error in Balmer EW
+        err_measured_F_pass (float): error in [Fe/H]
+        err_measured_K_pass (float): error in CaIIK EW
 
 
-    OUTPUTS:
-    ln(prior*like)
-    '''
+    Returns:
+        ln(prior*like)
+    """
 
     # walker_pos is the proposed walker position in N-D (likely 4-D) space
     # (i.e., these are the inputs to the model)
     lp = lnprior(walker_pos_array) # prior
     if not np.isfinite(lp): # afoul of prior
       return -np.inf
     result = -np.divide(1, 2*Teff_pass)*chi_sqd_fcn(measured_H_pass,
@@ -158,25 +144,26 @@
                                                     walker_pos_array)
 
     return lp + result # ln(prior*like)
 
 
 
 def lnprior(theta):
-    '''
-    Prior
+    """
+    Prior (top-hat priors only)
 
-    INPUTS:
-    theta: array of parameter values
+    Parameters:
+        theta (array): array of parameter values
 
-    OUTPUTS: 0 or -inf (top-hat priors only)
-    '''
+    Returns:
+        0 or -inf
+    """
 
     if (len(theta) == 4):
-        # Layden '94 relation
+        # Layden '94 relation (obsolete)
         a_test, b_test, c_test, d_test = theta
     elif (len(theta) == 8):
         # updated relation
         a_test, b_test, c_test, d_test, f_test, g_test, h_test, k_test = theta
 
     # top-hat priors
     if ((np.abs(a_test) < 40) and
@@ -185,25 +172,25 @@
         (np.abs(d_test) < 10)):
         return 0.0
 
     return -np.inf
 
 
 def function_K(coeffs_pass,Bal_pass,F_pass):
-    '''
+    """
     Function which gives CaIIK EW as function of Balmer, [Fe/H]
 
-    INPUTS:
-    coeffs_pass: array of coefficients
-    Bal_pass: Balmer EWs
-    F_pass: [Fe/H]
-
-    OUTPUTS:
-    K_pass: CaIIK EW
-    '''
+    Parameters:
+        coeffs_pass (array of floats): array of coefficients
+        Bal_pass (array of floats): Balmer EWs
+        F_pass (array of floats): [Fe/H]
+
+    Returns:
+        CaIIK EW
+    """
 
     if (len(coeffs_pass) == 4):
         # Layden '94 relation
 
         K_pass = coeffs_pass[0] \
                     + coeffs_pass[1]*Bal_pass \
                     + coeffs_pass[2]*F_pass \
@@ -221,21 +208,41 @@
                     + coeffs_pass[6]*np.power(Bal_pass,2.)*F_pass \
                     + coeffs_pass[7]*Bal_pass*np.power(F_pass,2.)
 
     return K_pass
 
 
 def K_residual(coeffs_pass,Bal_pass,F_pass,y):
-    # residual function, which we want to minimize for the Levenberg-Marquardt fit
-    # ('y' here is the measured CaIIK EW)
+    """
+    Residual function to minimize for the Levenberg-Marquardt fit
+
+    Parameters:
+        coeffs_pass (array): array of coefficients
+        Bal_pass (array): Balmer EWs
+        F_pass (array): [Fe/H]
+        y (float): measured CaIIK EW
+
+    Returns:
+        residual
+    """
 
     return y - function_K(coeffs_pass,Bal_pass,F_pass)
 
 
 def sigma_Km_sqd(coeffs_pass,Bal_pass,err_Bal_pass,Feh_pass,err_Feh_pass):
+    """
+    Definition of model CaIIK error squared (this is general, regardless of number of coeffs)
+
+    Parameters:
+        coeffs_pass (array): array of coefficients
+        Bal_pass (array): Balmer EWs
+        err_Bal_pass (array): error in Balmer EWs
+        Feh_pass (array): [Fe/H]
+        err_Feh_pass (array): error in [Fe/H]
+    """
     # def of model CaIIK error squared (this is general, regardless of number of coeffs):
     # sigma_Km^2 = (del_K/del_H)^2 * sig_H^2 + (del_K/del_F)^2 * sig_F^2
 
     # case of 4 coefficients
     if (len(coeffs_pass) == 4):
 
         dKdH = coeffs_pass[1] + coeffs_pass[3]*Feh_pass
@@ -261,29 +268,29 @@
 def chi_sqd_fcn(Bal_pass,
                 Feh_pass,
                 Caiik_pass,
                 sig_Bal_pass,
                 sig_Feh_pass,
                 sig_Caiik_pass,
                 coeffs_pass):
-    '''
+    """
     Chi-squared
 
-    INPUTS:
-    Bal_pass: Balmer EW (angstroms)
-    Feh_pass: [Fe/H]
-    Caiik_pass: CaIIK EW (angstroms)
-    err_Bal_pass: error in Balmer EW (angstroms)
-    err_Feh_pass: error in [Fe/H]
-    err_Caiik_pass: error in CaIIK EW (angstroms)
-    coeffs_pass: array of coefficients
-
-    OUTPUTS:
-    val: chi^2
-    '''
+    Parameters:
+        Bal_pass (float): Balmer EW (angstroms)
+        Feh_pass (float): [Fe/H]
+        Caiik_pass (float): CaIIK EW (angstroms)
+        err_Bal_pass (float): error in Balmer EW (angstroms)
+        err_Feh_pass (float): error in [Fe/H]
+        err_Caiik_pass (float): error in CaIIK EW (angstroms)
+        coeffs_pass (array): array of coefficients
+
+    Returns:
+        chi^2
+    """
 
     # def. of chi-squared for collection of datapoints which each have
     # subscript i:
     # X2 = Sigma_i [(K0,i - Km,i)^2/(sigma_K0,i^2 + sigma_Km,i^2)]
     # K0: measured CaIIK EW (error sigma_K0)
     # Km: model CaIIK EW (error sigma_Km)
 
@@ -305,176 +312,196 @@
     i_element = np.divide(numerator_array,denominator_array)
 
     val = np.sum(i_element)
 
     return val
 
 
-def write_soln_to_fits(model,
-                        mcmc_text_output_file_name = config_red["data_dirs"]["DIR_BIN"] + config_red["file_names"]["MCMC_OUTPUT"],
-                        teff_data_retrieve_file_name = config_red["data_dirs"]["DIR_BIN"] + config_red["file_names"]["TREND_TEFF_VS_BALMER"],
-                        soln_write_name = config_red["data_dirs"]["DIR_BIN"] + config_red["file_names"]["CALIB_SOLN"],
-                        test_flag=False):
-    '''
+class WriteSolnToFits():
+    """
     Takes the full reduction solution and writes it to a FITS file with
-    1) The MCMC posteriors in tabular form
-    2) Meta-data in FITS header
-
-    test_flag: if True, then terminal prompts are suppressed to enable continuous integration
-    '''
-
-    # initialize FITS header and append keys
-    hdr = fits.Header()
 
-    # retrieve git hash
-    repo = git.Repo(search_parent_directories=True)
-    sha = repo.head.object.hexsha
-    hdr["HASH"] = (sha, "Hash of rrlfe pipeline")
-
-    # get Teff vs Balmer line info
-    # set compound datatype
-    dtype=np.rec.fromrecords([['string_key', 189.6752158]]).dtype
-    # load data, skipping header and hash corresponding to that file
-    teff_data = np.loadtxt(teff_data_retrieve_file_name, skiprows=2, usecols=(0,1), delimiter=':', dtype=dtype)
-
-    dict_teff_data = {}
-    for key, val in teff_data:
-        dict_teff_data.update({key: val})
-
-    hdr["MODEL"] = (model, "Calibration type")
-    hdr["TEFF_MIN"] = (dict_teff_data["Teff_min"], "Minimum Teff for linear Teff vs. Balmer EW fit")
-    hdr["TEFF_MAX"] = (dict_teff_data["Teff_max"], "Maximum Teff for linear Teff vs. Balmer EW fit")
-    hdr["SLOPE_M"] = (dict_teff_data["m"], "Slope of Teff vs. Balmer EW")
-    hdr["ESLOPE_M"] = (dict_teff_data["err_m"], "Error in slope of Teff vs. Balmer EW")
-    hdr["YINT_B"] = (dict_teff_data["b"], "Y-intercept of Teff vs. Balmer EW")
-    hdr["EYINT_B"] = (dict_teff_data["err_b"], "Error in y-intercept of Teff vs. Balmer EW")
-    # comment explaining the solution
-    hdr["COMMENT"] = "Coefficients are defined as "
-    hdr["COMMENT"] = "K = a + bH + cF + dHF + f(H^2) + g(F^2) + h(H^2)F + kH(F^2)"
-
-    # read in posterior in csv form
-    if (model == "abcd"):
-
-        # corner plot (requires 'storechain=True' in enumerate above)
-        samples = pd.read_csv(mcmc_text_output_file_name, delim_whitespace=True, usecols=(1,2,3,4), names=["a", "b", "c", "d"])
-        c1 = fits.Column(name="a", array=np.array(samples.iloc[:,0].values), format="D")
-        c2 = fits.Column(name="b", array=np.array(samples.iloc[:,1].values), format="D")
-        c3 = fits.Column(name="c", array=np.array(samples.iloc[:,2].values), format="D")
-        c4 = fits.Column(name="d", array=np.array(samples.iloc[:,3].values), format="D")
-        table_hdu = fits.BinTableHDU.from_columns([c1, c2, c3, c4], header=hdr)
-
-
-    elif (model == "abcdfghk"):
-        # corner plot (requires 'storechain=True' in enumerate above)
-        # just first few lines to test
-        samples = pd.read_csv(mcmc_text_output_file_name, delim_whitespace=True, usecols=(1,2,3,4,5,6,7,8), names=["a", "b", "c", "d", "f", "g", "h", "k"])
-        c1 = fits.Column(name="a", array=np.array(samples.iloc[:,0].values), format="D")
-        c2 = fits.Column(name="b", array=np.array(samples.iloc[:,1].values), format="D")
-        c3 = fits.Column(name="c", array=np.array(samples.iloc[:,2].values), format="D")
-        c4 = fits.Column(name="d", array=np.array(samples.iloc[:,3].values), format="D")
-        c5 = fits.Column(name="f", array=np.array(samples.iloc[:,4].values), format="D")
-        c6 = fits.Column(name="g", array=np.array(samples.iloc[:,5].values), format="D")
-        c7 = fits.Column(name="h", array=np.array(samples.iloc[:,6].values), format="D")
-        c8 = fits.Column(name="k", array=np.array(samples.iloc[:,7].values), format="D")
-        table_hdu = fits.BinTableHDU.from_columns([c1, c2, c3, c4, c5, c6, c7, c8], header=hdr)
-
-
-    # write out
-    if not test_flag: # pragma: no cover
-        if os.path.exists(soln_write_name):
+    Parameters:
+        module_name (str): module name
+        file_name_mcmc_posterior_read (str): file name of MCMC posterior to write back out as FITS file
+        file_name_teff_data_read (str): file name of Teff data
+        soln_write_name (str): file name of FITS file to write
+        model_type_override (str): calibration model (obsolete) ("None")
+        test_flag (bool): if True, then terminal prompts are suppressed to enable continuous integration
+
+    Returns:
+        [FITS file written to disk with The MCMC posteriors in tabular form, and meta-data in header]
+    """
 
-            input("A calibration solution file already exists! \nDo " +\
-                    "what you want with that file and hit [ENTER] (will overwrite)")
+    def __init__(self,
+                module_name,
+                file_name_mcmc_posterior_read,
+                file_name_teff_data_read,
+                soln_write_name,
+                model_type_override=None,
+                test_flag=False):
+
+        self.name = module_name
+        self.file_name_mcmc_posterior_read = file_name_mcmc_posterior_read
+        self.file_name_teff_data_read = file_name_teff_data_read
+        self.soln_write_name = soln_write_name
+        self.model_type_override = model_type_override 
+        self.test_flag = test_flag
+
+    def run_step(self, attribs = None):
+
+        model = str(attribs["calib_type"]["COEFFS"]) # coefficients of model
+        mcmc_text_output_file_name = self.file_name_mcmc_posterior_read
+        teff_data_retrieve_file_name = self.file_name_teff_data_read
+        soln_write_name = self.soln_write_name
+        model_type_override = self.model_type_override
+        test_flag=self.test_flag
+
+        # initialize FITS header and append keys
+        hdr = fits.Header()
+
+        # retrieve git hash (throws error on cluster)
+        #repo = git.Repo(search_parent_directories=True)
+        #sha = repo.head.object.hexsha
+        #hdr["HASH"] = (sha, "Hash of rrlfe pipeline")
+
+        # get Teff vs Balmer line info
+        # set compound datatype
+        dtype=np.rec.fromrecords([['string_key', 189.6752158]]).dtype # all floats
+        # load data, skipping header and hash corresponding to that file
+        teff_data = np.loadtxt(teff_data_retrieve_file_name, skiprows=1, usecols=(0,1), delimiter=':', dtype=dtype)
+        dict_teff_data = {}
+        for key, val in teff_data:
+            dict_teff_data.update({key: val})
+
+        hdr["MODEL"] = (model, "Calibration type")
+        hdr["TEFF_MIN"] = (dict_teff_data["Teff_min"], "Minimum Teff for linear Teff vs. Balmer EW fit")
+        hdr["TEFF_MAX"] = (dict_teff_data["Teff_max"], "Maximum Teff for linear Teff vs. Balmer EW fit")
+        hdr["SLOPE_M"] = (dict_teff_data["m"], "Slope of Teff vs. Balmer EW")
+        hdr["ESLOPE_M"] = (dict_teff_data["err_m"], "Error in slope of Teff vs. Balmer EW")
+        hdr["YINT_B"] = (dict_teff_data["b"], "Y-intercept of Teff vs. Balmer EW")
+        hdr["EYINT_B"] = (dict_teff_data["err_b"], "Error in y-intercept of Teff vs. Balmer EW")
+        # comment explaining the solution
+        hdr["COMMENT"] = "Coefficients are defined as "
+        hdr["COMMENT"] = "K = a + bH + cF + dHF + f(H^2) + g(F^2) + h(H^2)F + kH(F^2)"
+        # history
+        hdr["COMMENT"] = "------------------------------------------------------------"
+        # hdr["HISTORY"] = "Solution generated with rrlfe, git hash " + sha # sha causes problems in the cloud
+        hdr["HISTORY"] = "Start time " + timestring_human
+        hdr["HISTORY"] = "Log file " + log_filename
+
+        # was there an override command when the class was called? if so, override the model type here
+        if model_type_override:
+            model = model_type_override
+
+        # read in posterior in csv form
+        if (model == "abcdfghk"):
+            # corner plot (requires 'storechain=True' in enumerate above)
+            # just first few lines to test
+            samples = pd.read_csv(mcmc_text_output_file_name, usecols=(0,1,2,3,4,5,6,7), delimiter=",", names=["a", "b", "c", "d", "f", "g", "h", "k"])
+
+            c1 = fits.Column(name="a", array=np.array(samples.iloc[:,0].values), format="D")
+            c2 = fits.Column(name="b", array=np.array(samples.iloc[:,1].values), format="D")
+            c3 = fits.Column(name="c", array=np.array(samples.iloc[:,2].values), format="D")
+            c4 = fits.Column(name="d", array=np.array(samples.iloc[:,3].values), format="D")
+            c5 = fits.Column(name="f", array=np.array(samples.iloc[:,4].values), format="D")
+            c6 = fits.Column(name="g", array=np.array(samples.iloc[:,5].values), format="D")
+            c7 = fits.Column(name="h", array=np.array(samples.iloc[:,6].values), format="D")
+            c8 = fits.Column(name="k", array=np.array(samples.iloc[:,7].values), format="D")
+            table_hdu = fits.BinTableHDU.from_columns([c1, c2, c3, c4, c5, c6, c7, c8], header=hdr)
+        
+        else:
+            logging.error('Error! No clear selection of model')
+
+
+        # write out as FITS table
+        # check receiving directory exists in first place
+        if os.path.dirname(soln_write_name):
+            # check if directory exists
+            logging.info('File to contain FITS calibration is '+str(soln_write_name))
+        else:
+            logging.warning('Making new directory '+str(os.path.dirname(soln_write_name))+ ' which will contain FITS calibration')
+            make_dir(os.path.dirname(soln_write_name))
+        if not test_flag: # pragma: no cover
+            if os.path.exists(soln_write_name):
+                logging.warning("A calibration solution file already exists! Will overwrite")
 
-        table_hdu.writeto(soln_write_name, overwrite=True)
-        logging.info("Full calibration MCMC posterior written to " + soln_write_name)
+            table_hdu.writeto(soln_write_name, overwrite=True)
+            logging.info("Full calibration MCMC posterior written to " + soln_write_name)
 
-    # return FITS table for testing
-    return table_hdu
+        # return FITS table for testing
+        return table_hdu
 
 
 
 class RunEmcee():
-    '''
+    """
     Run the emcee MCMC to obtain coefficients a, b, c, d (+ f, g, h, k)
-    '''
+
+    Parameters:
+        module_name (str): module name
+        file_name_scraped_ews_good_only_read (str): file name of scraped EW data, containing only the 'good' data
+        file_name_write_mcmc_text_write (str): file name of MCMC posteriors to write as csv
+
+    Returns:
+        [posteriors written to disk]
+    """
 
     def __init__(self,
-                 scraped_ews_good_only_file_name = config_red["data_dirs"]["DIR_EW_PRODS"] + config_red["file_names"]["RESTACKED_EW_DATA_GOOD_ONLY_TEFFFIT"],
-                 mcmc_text_output_file_name = config_red["data_dirs"]["DIR_BIN"] + config_red["file_names"]["MCMC_OUTPUT"]
-                 ):
+                module_name,
+                file_name_scraped_ews_good_only_read,
+                file_name_write_mcmc_text_write):
 
-        # name of file with final K, H, FeH, and error values (and not the others from the noise-churned spectra)
-        self.scraped_ew_filename = scraped_ews_good_only_file_name
+        self.name = module_name
+        self.file_name_scraped_ews_good_only_read = file_name_scraped_ews_good_only_read
+        self.file_name_write_mcmc_text_write = file_name_write_mcmc_text_write
 
-        # name of file of the MCMC output
-        self.mcmc_text_output = mcmc_text_output_file_name
+    def run_step(self, attribs = None):
 
+        scraped_ews_good_only_file_name = self.file_name_scraped_ews_good_only_read
+        mcmc_text_output_file_name = self.file_name_write_mcmc_text_write
 
-    def __call__(self, model, post_burn_in_links = 3e5):
-        '''
-        INPUTS
-
-        model: list of coefficients to use as the model
-            'abcd':     corresponds to Layden '94
-            'abcdfghk': corresponds to K = a + b*H + c*F + d*H*F + f*(H^2) + g*(F^2) + h*(H^2)*F + k*H*(F^2)
-        post_burn_in_links: chain links following burn-in
-        '''
+        model = str(attribs["calib_type"]["COEFFS"]) # coefficients of model
+        post_burn_in_links = int(attribs["reduc_params"]["MCMC_POSTBURN"])
 
         # read in EWs, Fe/Hs, phases, errors, etc.
         logging.info("--------------------------")
-        logging.info("Reading in data from " + self.scraped_ew_filename)
+        logging.info("Reading in data from " + scraped_ews_good_only_file_name)
 
-        ## ## make df_choice.Spectrum -> df_choice["Spectrum etc.
-        df_choice = pd.read_csv(self.scraped_ew_filename,delim_whitespace=False)
+        df_choice = pd.read_csv(scraped_ews_good_only_file_name,delim_whitespace=False)
 
         # EWs in table are in angstroms and are mislabeled as mA (2020 Jan 12)
         name = df_choice['orig_spec_file_name']
         #caii = np.divide(df_choice['K'], 1000.)
         caii = df_choice['EW_CaIIK']
         #ecaii = np.divide(df_choice['err_K'], 1000.)
-        ecaii = df_choice['err_EW_CaIIK_from_robo'] # might try other error sources later
+        ecaii = df_choice['err_EW_CaIIK_scaled'] # might try other error sources later
         #ecaii = df_choice['err_EW_CaIIK']
         #ave = np.divide(df_choice['balmer'], 1000.)
         ave = df_choice['EW_Balmer']
-        eave = df_choice['err_EW_Balmer_from_Robo']
+        eave = df_choice['err_EW_Balmer_scaled']
         #eave = np.divide(df_choice['err_balmer'], 1000.)
-        ## ## THE BELOW FEH VALUES NEED TO BE CHECKED/FIXED
         feh = df_choice['feh']
         efeh = df_choice['err_feh']
 
         # non-zero starting points for coefficients fghk (i.e., those beyond the Layden
         # model)
         f_init = 0.1
         g_init = 0.1
         h_init = 0.1
         k_init = 0.1
         m_init = 0. # 4th-order term; vestigial
         n_init = 0. # 4th-order term; vestigial
-        #sigma_a_layden = 0.416
-        #sigma_b_layden = 0.076
-        #sigma_c_layden = 0.285
-        #sigma_d_layden = 0.052
 
         # starting position, before adding a perturbation
 
-        if model == 'abcd':
-            # coeffs_pass = [a,b,c,d]
-
-            nwalkers = 8 # number of MCMC chains (at least 2x number of parameters)
-
-            param_array_0 = [float(a_layden),
-                            float(b_layden),
-                            float(c_layden),
-                            float(d_layden)]
-
-        elif model == 'abcdfghk':
+        if model == 'abcdfghk':
             # coeffs_pass = [a,b,c,d,f,g,h,k]
 
-            nwalkers = 16 # number of MCMC chains (at least 2x number of parameters)
+            nwalkers = int(16) # number of MCMC chains (at least 2x number of parameters)
 
             param_array_0 = [float(a_layden),
                             float(b_layden),
                             float(c_layden),
                             float(d_layden),
                             float(f_init),
                             float(g_init),
@@ -485,61 +512,73 @@
         # this is for abcd or abcdfghk calibrations, whichever is being done by the MCMC
         lstsq_soln = least_squares(K_residual, param_array_0, args=(ave, feh, caii), method="lm")
         logging.info("--------------------------")
         logging.info("Levenberg-Marquardt soln made. Vector array: ")
         logging.info(lstsq_soln.x)
 
         ################# MCMC setup #################
-
         logging.info("--------------------------")
         logging.info("Setting up MCMC ...")
 
-        ndim = len(param_array_0) # dimensions of space to explore
+        ndim = int(len(param_array_0)) # dimensions of space to explore
+
+        # Set up the backend
+        # Don't forget to clear it in case the file already exists
+        '''
+        filename = "tutorial.h5"
+        backend = emcee.backends.HDFBackend(filename)
+        backend.reset(nwalkers, ndim)
+        '''
 
         # convert the one starting point into a nwalkers*ndim array with gaussian-offset starting points
         p0 = [np.add(param_array_0,
                      np.multiply(param_array_0, 1e-4*np.random.randn(ndim))) for i in range(nwalkers)]
 
         # set up sampler
         sampler = emcee.EnsembleSampler(nwalkers,
                                         ndim,
                                         lnprob,
                                         args=[Teff, ave, feh, caii, eave, efeh, ecaii])
 
         # burn-in
-        burn_in = 3e4
-        posAfterBurn, prob, state = sampler.run_mcmc(p0, burn_in)
+        burn_in = int(3e4)
+        state = sampler.run_mcmc(p0, burn_in)
+        sampler.reset()
 
-        # post-burn-in
-        start_time = time.time()
-
-        ################# SAVE PROGRESSIVELY TO TEXT FILE #################
+        ################# SAVE TO FILE #################
         ## ## refer to these code snippets from Foreman-Mackey's website
         # IMPORTANT: sampler will only have memory of the last iteration if
         # storechain flag is set to False
 
         logging.info("--------------------------")
-        logging.info("Saving MCMC chains to text file ...")
+        logging.info("Saving MCMC chains to file ...")
+        logging.info("nwalkers:", nwalkers)
+        logging.info("ndim:", ndim)
+        logging.info("burn in:", burn_in)
 
         # post-burn-in calculate and save iteratively
-        f = open(self.mcmc_text_output, "w")
-        f.close()
-        progBarWidth = 30
-        start_time = time.time()
-        for i, result in enumerate(sampler.sample(posAfterBurn,
-                                                  iterations=post_burn_in_links,
-                                                  storechain=True)):
-            position = result[0]
-            f = open(self.mcmc_text_output, "a") # append
-            for k in range(position.shape[0]): # loop over number of chains
-                position_string = str(position[k]).strip("[]") # convert to string
-                f.write("{0:4d} {1:s}\n".format(k, " ".join(str(p) for p in position[k])))
-            n = int((progBarWidth+1) * float(i) / post_burn_in_links) # update progress bar
-            sys.stdout.write("\r[{0}{1}]".format("#" * n, " " * (progBarWidth - n)))
-            f.close()
-        elapsed_time = time.time() - start_time
-        sys.stdout.write(" Done!\n")
-        sys.stdout.write("{0:s} {1:10d} {2:s}\n".format("Elapsed time: ",
-                                                        int(elapsed_time), "sec"))
+        # mcmc_text_output_file_name,
+        post_burn_in_links = int(post_burn_in_links)
+        sampler.run_mcmc(state, post_burn_in_links)
+
+        samples = sampler.get_chain(flat=True)
+
+        # test plot
+        '''
+        plt.hist(samples[:, 0], 100, color="k", histtype="step")
+        plt.xlabel(r"$\theta_1$")
+        plt.ylabel(r"$p(\theta_1)$")
+        plt.gca().set_yticks([])
+        plt.savefig("junk.png")
+        plt.clf()
+        '''
+
+        # test csv file
         logging.info("--------------------------")
-        sys.stdout.write("MCMC chain data written out to\n")
-        logging.info(self.mcmc_text_output)
+        if os.path.dirname(mcmc_text_output_file_name):
+            # check if directory exists
+            logging.info('File to contain MCMC data will be '+str(mcmc_text_output_file_name))
+        else:
+            logging.warning('Making new directory '+str(os.path.dirname(mcmc_text_output_file_name))+ ' which will contain MCMC output data')
+            make_dir(os.path.dirname(mcmc_text_output_file_name))
+        np.savetxt(mcmc_text_output_file_name,samples,delimiter=",")
+        logging.info("MCMC chains written out as " + str(mcmc_text_output_file_name))
```

### Comparing `rrlfe-0.0.9/modules/create_spec_realizations.py` & `rrlfe-1.0/rrlfe/create_spec_realizations.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,86 +1,64 @@
 #!/usr/bin/python
-'''
-This module takes a list of spectra and generates normalized realizations using Gaussian Error.
-
-This module takes a list of spectra. First it generates 100 realizations of the spectra using the error bar to move the points around
-simulating Gaussian noise. Then it runs Ken Carrell's bkgrnd routine to determine the normalization and finally creates the normalized spectra.
-
-@package create_spec_realizations
-@author deleenm
-@version \e \$Revision$
-@date \e \$Date$
-
-Usage: create_spec_realizations.py
-'''
 
 # -----------------------------
 # Standard library dependencies
 # -----------------------------
 import argparse
 import os
 import glob
 from subprocess import Popen, PIPE
-## ## import test.so # experimenting with C extensions
 # -------------------
 # Third-party imports
 # -------------------
-#from astropy.io import fits ## Pylint says this is not used
 from astropy.io import fits
 from astropy.table import Table
-#import pyfits
 import sys
 import numpy as np
 import pandas as pd
 from pathlib import *
 
 current_dir = os.path.dirname(__file__)
-print("Current dir:")
-print(current_dir)
 
 from . import *
 
-
-
 # --------------------
 # Function Definitions
 # --------------------
 def create_norm_spec(name_list,
                      normdir,
                      finaldir):
-    '''
+    """
     Create final normalized spectra, using the output from the bkgrnd routine (which
     puts out wavelength, flux, and continuum flux, but not the actual normalized flux)
 
-    Arguments:
-        name_list: List of Realization file names (no path info); should have 3 cols
-        normdir: Directory where files in name_list are located
-        finaldir: The final directory for files which have completed the full
+    Parameters:
+        name_list (list): list of realization file names (no path info); should have 3 cols
+        normdir (str): directory where files in name_list are located
+        finaldir (str): final directory for files which have completed the full
             normalization process; these will have 3 cols too
     Returns:
-       A list of final file names
-    '''
+       list of final file names
+    """
 
     logging.info("Creating normalized spectra")
 
     new_name_list = list()
 
     for spec in name_list: # loop through spectrum realizations
-        #import ipdb; ipdb.set_trace()
 
         # spectrum realization file name (as output by bkgrnd), with relative path info
         spec_name = os.path.join(normdir, spec)
 
         # astropy table containing a spectrum's 1.) wavelength, 2.) flux, 3.) background flux
         spec_tab = read_bkgrnd_spec(spec_name)
         # output file name of final, normalized spectrum, with relative path info
         new_name = os.path.join(finaldir, spec) # vestigial, from adding .smo to help Robospect pick it out
         # add to list
         new_name_list.append(new_name)
-        #import ipdb; ipdb.set_trace()
 
         try:
             # open file to write normalized spectrum to
             outfile = open(new_name, 'w')
         except IOError:  # pragma: no cover
             logging.info("File {} could not be opened!".format(new_name))
         for j in range(len(spec_tab['wavelength'])):
@@ -89,14 +67,31 @@
                                                spec_tab['flux'][j]/spec_tab['bckgrnd_flux'][j]))
 
         outfile.close()
 
     return(new_name_list)
 
 def calc_noise(noise_level, spectrum_df):
+    """
+    Generate noise spectrum
+
+    Parameters:
+        noise_level (str/float): define noise level \n
+            "file": from file \n
+            "None": no noise \n
+            (float): level of relative noise to use
+        spectrum_df (pandas dataframe): spectrum file; if noise is being read in from file, or is 
+            being calculated from the flux, those must be in this file, in cols as follows: \n
+            [0]: wavelength [angstr] \n
+            [1]: flux \n
+            [2]: background flux \n
+
+    Returns:
+        Numpy array of noise spectrum
+    """
 
     if (noise_level == "file"):
         # add Gaussian error to the empirical flux, taking sigma to be the
         # 'error' column in an input file; note this is an ABSOLUTE error
         noise_to_add = np.random.standard_normal(len(spectrum_df))*spectrum_df["error"]
         logging.info("Injecting Gaussian noise based on error column in file.")
     elif (noise_level == "None"):
@@ -104,174 +99,158 @@
         noise_to_add = 0
         logging.info("Injecting no noise at all")
     else:
         # noise is a set value, representing a Gaussian sigma; this is normalized,
         # so a '0.01' means 'Gaussian-distributed random number with sigma=0.01*flux_input';
         # note this 0.01 is a RELATIVE error
         noise_to_add = np.random.standard_normal(len(spectrum_df))*noise_level*spectrum_df["flux"]
-        logging.info("Injecting Gaussian noise based on fixed value.")
+        logging.info("Injecting "+str(noise_level)+" of Gaussian noise.")
 
     return noise_to_add
 
 
-def generate_realizations(spec_name, outdir, spec_file_format, num, noise_level):
-    '''
-    Calculates a Number of Realizations of a given spectrum using Gaussian Errorbars
-
-    Arguments:
-        spec_name: The spectrum filename
-        outdir: The working directory
-        spec_file_format: The format of the input spectra ["fits", "ascii.no_header"]
-        num: Number of realizations to generate
-        noise: 'None': add no noise; 'file': take Gaussian samples of error with spread based on the error column in file
+def generate_realizations(spec_name, 
+                          outdir, 
+                          spec_file_format, 
+                          num, 
+                          noise_level):
+    '''
+    Calculates a number of realizations of a given spectrum using Gaussian error bars
+
+    Parameters:
+        spec_name (str): the spectrum filename
+        outdir (str): the working directory
+        spec_file_format (str): the format of the input spectra ["fits", "ascii.no_header"]
+        num (int): number of realizations to generate
+        noise (str/float): 'None': add no noise; 'file': take Gaussian samples of error with spread based on the error column in file
     Returns:
-       A list of filenames for the realization spectra.
+       list of filenames for the realization spectra.
     '''
 
     logging.info("Generating spectrum realizations of " + spec_name)
 
     # astropy table containing an empirical spectrum's 1.) wavelength, 2.) flux, 3.) error
     # and the header of the source FITS file
     spec_tab, hdr = read_spec(spec_name, format=spec_file_format)
 
-    #import ipdb; ipdb.set_trace()
     basename = os.path.basename(spec_name) # shave off path stem
 
+    # check if directory to write to exists
+    if os.path.isdir(outdir):
+        logging.info('Writing realizations of input spectra to '+str(outdir))
+    else:
+        logging.warning('Making new directory '+str(outdir)+ ' which is supposed to contain written out spectrum realizations')
+        make_dir(outdir)
+
     # generate realizations
     new_basename_list = list()
 
     for i in range(num):
 
         # make file names
 
         # basename of spectrum realization, ascii
-        new_prefix_ascii = "{}_noise_ver_{:03d}".format(basename.split(".")[-2], i)
+        new_prefix_ascii = "{}_{:03d}".format(basename.split(".")[-2], i)
         suffix_ascii = basename.split(".")[-1] # could be .dat, .csv, .txt, etc.
         new_basename_ascii = new_prefix_ascii + "." + suffix_ascii
         # if we want to change to FITS intermediary files:
-        new_basename_fits = "{}_noise_ver_{:03d}".format(basename.split(".fits")[0], i) + ".fits"
+        new_basename_fits = "{}_{:03d}".format(basename.split(".fits")[0], i) + ".fits"
         # don't need path info in spec_name list; add ascii name here
         new_basename_list.append(new_basename_ascii)
 
         # name of spectrum realization, with path
         new_name_ascii = os.path.join(outdir, new_basename_ascii)
         new_name_fits = os.path.join(outdir, new_basename_fits)
 
         noise_to_add = calc_noise(noise_level=noise_level, spectrum_df=spec_tab)
 
         # add the noise
         new_flux = noise_to_add + spec_tab['flux']
-        #print(new_flux)
-        print(new_name_ascii)
-
 
         try:
             outfile = open(new_name_ascii, 'w')
         except IOError: # pragma: no cover
             logging.info("File {} could not be opened!".format(new_name_ascii))
 
-        #import ipdb; ipdb.set_trace()
-
-        ### write out new realization of file, in two formats:
-        '''
-        ## ## obsolete?
-        df_realization = Table([spec_tab["wavelength"], new_flux],
-                                names=("wavelength","new_flux"))
-        # set column names and write
-        c1=fits.Column(name="wavelength", format='D', array=spec_tab["wavelength"])
-        c2=fits.Column(name="new_flux", format='D', array=new_flux)
-        t = fits.BinTableHDU.from_columns([c1, c2], header=hdr)
-        '''
-        ## second format: ascii, so bkgrnd can read it in
+        # write out new realization of file in ascii, so bkgrnd can read it in
         logging.info("Writing out ascii realization file " + new_name_ascii + \
             " with noise level stdev " + str(np.std(noise_to_add)))
         for j in range(len(new_flux)):
             outfile.write("{} {:.2f}\n".format(spec_tab['wavelength'][j], new_flux[j]))
         outfile.close()
 
     return(new_basename_list)
 
 def read_bkgrnd_spec(spec_name):
-    '''
+    """
     Reads in ascii spectra created by bckgrnd and returns numpy arrays of wavelength, flux, bckgrnd_flux
 
     Arguments:
-        spec_name: The spectrum filename. If Ascii file should have 3 columns: wavelength, flux, bckgrnd_flux
+        spec_name (str): The spectrum filename. If ascii file, should have 3 columns: \n
+            [0]: wavelength [angstr] \n
+            [1]: flux \n
+            [2]: background flux \n
     Returns:
-       spec_tab: A numpy Table with three columns: wavelength, flux, background flux
-    '''
+       numpy table with three columns: wavelength, flux, background flux
+    """
 
     logging.info("Reading ascii spectrum realization and background in " + spec_name)
-
+    
     spec_tab = Table.read(spec_name, format='ascii.no_header',
                           names=['wavelength', 'flux', 'bckgrnd_flux'])
 
     return(spec_tab)
 
 
-#####
-
-'''
-    ## note Feb. 9 2021: change to read in FITS files, but output same
-    if (format == "fits"):
-        # read in table info
-        spec_tab = Table.read(spec_name, format='fits')
-        # read in header info
-        hdul = fits.open(spec_name)
-        hdr = hdul[0].header
-    elif (format == "ascii.no_header"):
-        # this option is antiquated; we want to preserve FITS header info
-        spec_tab = Table.read(spec_name, format='ascii.no_header',
-                          names=['wavelength', 'flux', 'error'])
-        hdr = np.nan
-
-    return(spec_tab, hdr)
-'''
-#####
-
 def read_list(input_list):
-    '''
-    Reads in list of spectrum names and returns a table of filenamse
+    """
+    Read in list of spectrum names and returns a table of filenamse
 
     Arguments:
-        input_list: a csv file with columns
-            [0]: filename
-            [1]: subtype (RRab, RRc)
-            [2]: phase (0. to 1., -9999 for NaN)
-            [3]: metallicity (if producing the calibration)
+        input_list (str): file name of a csv file with columns \n
+            [0]: filename \n
+            [1]: subtype (RRab, RRc) \n
+            [2]: phase (0. to 1., -9999 for NaN) \n
+            [3]: metallicity (if producing the calibration) \n
             [4]: error in metallicity (if producing the calibration)
     Returns:
-       Numpy array of filenames
-    '''
+       numpy array of filenames
+    """
 
-    logging.info("Reading in list of spectrum names to return table of filenames")
+    if os.path.exists(input_list):
+        logging.info("Reading in list of spectrum names " + input_list)
+    else:
+        logging.info("List of spectrum names does not exist! " + input_list)
 
     # expects header reading
     # spectrum,subtype,phase,feh,err_feh
     input_data_arr = pd.read_csv(input_list)
 
     # col 0 contains the file names
     filenames_arr = input_data_arr["orig_spec_file_name"].values
 
     return(filenames_arr)
 
 
 def read_spec(spec_name, format):
-    '''
-    Reads in ascii empirical spectra and returns numpy arrays of
+    """
+    Read in ascii empirical spectrum and return
     wavelength, flux, and error.
 
-    Arguments:
-        spec_name: The spectrum filename. If Ascii file should have
-           3 columns (wavelength, flux, error no headers)
-        format: "fits" or "ascii.no_header"
+    Parameters:
+        spec_name (str): The spectrum filename. If ascii file (no headers), should have
+           3 columns \n
+           [0]: wavelength \n
+           [1] flux \n
+           [2] error \n
+        format (str): format of the spectrum file ("ascii.no_header" is the only option for now)
     Returns:
        spec_tab: A numpy Table with three columns: wavelength, flux, error
        hdr: FITS header of the input spectrum
-    '''
+    """
 
     logging.info("Reading spectrum " + spec_name)
 
     if (format == "ascii.no_header"):
 
         try:
             spec_tab = Table.read(spec_name, format='ascii.no_header',
@@ -286,33 +265,41 @@
     else: # pragma: no cover
         logging.info("File format unknown!!!")
 
     return(spec_tab, hdr)
 
 
 def write_bckgrnd_input(name_list, indir, normdir):
-    '''
+    """
     Create input file for the bckgrnd program
 
-    Arguments:
-        name_list: List of Realization file names (no path info)
-        indir: The working directory with files to be fed into bkgrnd routine
-        normdir: The output directory for normalized files
+    Parameters:
+        name_list (list): List of Realization file names (no path info)
+        indir (str): The working directory with files to be fed into bkgrnd routine
+        normdir (str): The output directory for normalized files
     Returns:
-       A string with the background input filename; the filename itself which
-       has been written out lists the input and output directories, and a
+      background input filename string; the filename itself (which
+       has been written to disk) lists the input and output directories, and a
        list of the FITS files which are the spectrum realizations in the input
        directory
-    '''
+    """
 
     logging.info("Creating input file list of spectrum realization filenames")
 
+    # check if directory exists
+    if os.path.isdir(indir):
+        logging.info('Spectrum realizations being read in from '+str(indir))
+    else:
+        logging.warning('Making new directory '+str(indir)+ ' which will contain spectrum realizations')
+        make_dir(indir)
+
     #Check to see if inputfile is already there
     bckgrnd_input = os.path.join(indir, "bckgrnd_input.txt")
     if os.path.isfile(bckgrnd_input) is True:
+        logging.warning('Removing pre-existing file bckgrnd_input.txt')
         os.remove(bckgrnd_input)
     try:
         outfile = open(bckgrnd_input, 'w')
     except IOError:   # pragma: no cover
             logging.info("File {} could not be opened!".format(bckgrnd_input))
 
 
@@ -323,167 +310,158 @@
     outfile.close()
 
     return(bckgrnd_input)
 
 # -------------
 # Main Function
 # -------------
-def create_spec_realizations_main(noise_level,
-                                spec_file_type,
-                                num = 100,
-                                  input_spec_list_dir = config_red["data_dirs"]["DIR_SRC"],
-                                  input_list = config_red["data_dirs"]["DIR_SRC"] + config_red["file_names"]["LIST_SPEC_PHASE"],
-                                  unnorm_empirical_spectra_dir = config_red["data_dirs"]["DIR_RAW_SPEC_DATA"],
-                                  unnorm_noise_churned_spectra_dir = config_red["data_dirs"]["DIR_REZNS_SPEC"],
-                                  bkgrnd_output_dir = config_red["data_dirs"]["DIR_REZNS_SPEC_NORM"],
-                                  final_dir = config_red["data_dirs"]["DIR_REZNS_SPEC_NORM_FINAL"],
-                                  verb=False):
-    '''
-    INPUTS:
-    num: number of spectrum realizations to make, per empirical spectrum
-    spec_file_type: file format of input spectra ["fits"/"ascii.no_header"]
-    input_spec_list_dir: directory containing list of empirical spectra (## OBSOLETE? ##)
-    input_list: file listing spectra we want to normalize
-    unnorm_empirical_spectra_dir: directory of empirical spectra (or, if they are actually
-        synthetic spectra, these are the original synthetic spectra which we will generate
-        multiple realizations of)
-    unnorm_noise_churned_spectra_dir: directory to contain noise-churned spectrum realizations
-    bkgrnd_output_dir: directory to contain output of bkgrnd (spectra and fit continuua)
-    final_dir: directory to contain normalized spectrum realizations
+class CreateSpecRealizationsMain():
+    """
 
-    OUTPUTS:
-    (text files written)
-    '''
+    Generate multiple realizations of the same empirical spectrum based on a noise level.
 
-    logging.info("--------------------------")
-    logging.info("Making "+str(num)+" realizations of each input spectrum")
+    Parameters:
+        module_name (str): name of module (arbitrary)
+        cc_bkgrnd_dir (str): absolute path of the directory containing the compiled binary for spectrum backround normalization
+        input_spec_list_read (str): absolute path of the file containing the list of spectrum file names (basenames only)
+        unnorm_spectra_dir_read (str): absolute path of the directory containing the spectra
+        unnorm_noise_churned_spectra_dir_read (str): absolute path of the directory to contain the output spectra with noise added at the level given by user (which may be zero noise)
+        bkgrnd_output_dir_write (str): absolute path of the directory to contain spectra after normalization (reads in from dir set by unnorm_noise_churned_spectra_dir_read/)
+        final_spec_dir_write (str): absolute path of the directory to contain spectra after normalization, with two-column formatting (reads in from dir set by bkgrnd_output_dir_write/)
+        noise_level (str or float): (file name) of file containing noise levels, "None", or float value to set level of noise being injected into spectra (if the calibration is being applied to the spectra, you almost certainly want this to be zero)
+        spec_file_type (str): defines the input file type (only option is "ascii.no_header" for now)
+        number_specs (int): number of spectrum realizations to make, per empirical spectrum (if the calibration is being applied, this almost certainly should be 1)
+        verb (bool): verbose option
 
-    if (num > 1) and (noise_level == "None"):
-        logging.warning("Realizing multiple spectra but noise level is zero")
-        input("Hit [Enter] to continue")
-
-    # Read list of input spectra
-    # input_list ALREADY SET IN DEFAULTS ## input_list = input_spec_list_dir + config_red["file_names"]["LIST_SPEC_PHASE"]
-    list_arr = read_list(input_list)
-
-    #logging.info('list_arr')
-    #logging.info(list_arr)
-
-    # Check to make sure the files in the list are actually in the input directory;
-    # if not, just remove those from the list and set a warning
-    list_actually_there = glob.glob(unnorm_empirical_spectra_dir + "*.*")
-    list_actually_basenames = np.array([os.path.basename(t) for t in list_actually_there])
-
-    num_sought = len(list_arr) # number of wanted files
-    num_existing = np.sum(np.in1d(list_arr, list_actually_basenames)) # number of wanted files found
-    bool_present = np.in1d(list_arr, list_actually_basenames, invert=False)
-    bool_missing = np.in1d(list_arr, list_actually_basenames, invert=True)
-    files_missing = list_arr[bool_missing] # files in input list, but not found
-    files_present = list_arr[bool_present] # files in input list, and found
-    num_extra = np.sum(np.in1d(list_actually_basenames, list_arr, invert=True)) # number of extra files found in the input directory
-
-    # did we find all the spectra we wanted?
-    if (num_existing < num_sought):
-        logging.warning(print("Found only "+str(num_existing)+" of "+str(num_sought)+" spectra in input list"))
-        logging.warning("Files missing from input directory:")
-        logging.warning(files_missing)
-    else:
-        logging.info("All spectra in input list found in input directory")
-
-    # did any other spectra appear in the directory, which may or may not be a good thing?
-    if (num_extra > 1):
-        logging.warning(print("Found "+str(num_extra)+" files in directory which do not appear in input list"))
-    else:
-        logging.info("No spectra found in input directory which do not appear in input list.")
-
-    # if there are files missing from the directory, just remove those from the input list
-    list_arr = files_present
+    Returns:
+        [text files of spectra written to disk]
+    """
 
-    # Check to make sure outdir (to receive realizations of spectra) exists
-    outdir = unnorm_noise_churned_spectra_dir
-    if not os.path.isdir(outdir):
-        os.mkdir(outdir)
-    else:
-        # Check to see if there are any files in the output directories (if not,
-        # there is data from a previous run that will inadvertently be used later)
-        # read the entries
-
-        #import ipdb; ipdb.set_trace()
-
-        with os.scandir(outdir) as list_of_entries1:
-            counter1 = 0
-            for entry1 in list_of_entries1:
-                if entry1.is_file():
-                    counter1 += 1
-        if (counter1 != 0):
-            logging.info("------------------------------")
-            logging.info("Directory to write realizations not empty!!")
-            logging.info(outdir)
-            logging.info("------------------------------")
-            input("Do what you want with those files, then hit [Enter]")
-
-        with os.scandir(bkgrnd_output_dir) as list_of_entries2:
-            counter2 = 0
-            for entry2 in list_of_entries2:
-                if entry2.is_file():
-                    counter2 += 1
-        if (counter2 != 0):
-            logging.info("------------------------------")
-            logging.info("Directory to write raw normalization output not empty!!")
-            logging.info(bkgrnd_output_dir)
-            logging.info("------------------------------")
-            input("Do what you want with those files, then hit [Enter]")
-
-        with os.scandir(final_dir) as list_of_entries3:
-            counter3 = 0
-            for entry3 in list_of_entries3:
-                if entry3.is_file():
-                    counter3 += 1
-        if (counter3 != 0):
-            logging.info("------------------------------")
-            logging.info("Directory to write final normalization output not empty!!")
-            logging.info(final_dir)
-            logging.info("------------------------------")
-            input("Do what you want with those files, then hit [Enter]")
-
-    # create noise-churned realizations for each spectrum
-    name_list = list() # initialize
-    #import ipdb; ipdb.set_trace()
-    for i in range(len(list_arr)): # make spectrum realizations and list of their filenames
-        #import ipdb; ipdb.set_trace()
-        print(i)
-        name_list.extend(generate_realizations(spec_name=unnorm_empirical_spectra_dir+"/"+list_arr[i],
-                                               outdir=outdir,
-                                               spec_file_format=spec_file_type,
-                                               num=num,
-                                               noise_level=noise_level))
-
-    # next we need to normalize the spectra; begin by creating input list of
-    # spectrum realizations written in the previous step
-    bkg_input_file = write_bckgrnd_input(name_list, outdir, bkgrnd_output_dir)
-    logging.info("-------------------------------------------")
-    logging.info('The file containing the list of spectra which will be fed ' + \
-                'into the normalization routine is ' + bkg_input_file)
-
-    # normalize each spectrum realization (smoothing parameter is set in __init__)
-    bkgrnd = Popen([str(config_red["data_dirs"]["DIR_BIN"]) + "bkgrnd", "--smooth "+str(config_red["reduc_params"]["SMOOTH"]),
-                    "--sismoo 1", "--no-plot", "{}".format(bkg_input_file)], stdout=PIPE, stderr=PIPE)
-    (out, err) = bkgrnd.communicate() # returns tuple (stdout, stderr)
-
-    if verb == True: ## ## decode messages (are they used later? why take this step?)
-        logging.info(out.decode("utf-8"))
-        logging.info(err.decode("utf-8"))
-
-    # read in input files, normalize them, write out, and return list of those filenames
-    final_list = create_norm_spec(name_list, bkgrnd_output_dir, final_dir)
-
-    logging.info("-------------------------------------------")
-    logging.info("Wrote realizations of original spectra to directory")
-    logging.info(outdir)
-    logging.info("-------------------------------------------")
-    logging.info("Wrote raw normalization output to directory")
-    logging.info(bkgrnd_output_dir)
-    logging.info("-------------------------------------------")
-    logging.info("Wrote final normalized spectra to directory")
-    logging.info(final_dir)
+    def __init__(self,
+                module_name,
+                cc_bkgrnd_dir,
+                input_spec_list_read,
+                unnorm_spectra_dir_read,
+                unnorm_noise_churned_spectra_dir_read,
+                bkgrnd_output_dir_write,
+                final_spec_dir_write,
+                noise_level,
+                spec_file_type,
+                number_specs,
+                verb=False):
+
+        self.name = module_name
+        self.cc_bkgrnd_dir = cc_bkgrnd_dir
+        self.input_spec_list_read = input_spec_list_read
+        self.unnorm_spectra_dir_read = unnorm_spectra_dir_read
+        self.unnorm_noise_churned_spectra_dir_read = unnorm_noise_churned_spectra_dir_read
+        self.bkgrnd_output_dir_write = bkgrnd_output_dir_write
+        self.final_spec_dir_write = final_spec_dir_write
+        self.noise_level = noise_level
+        self.spec_file_type = spec_file_type
+        self.number_specs = number_specs
+        self.verb = verb
+
+    def run_step(self, attribs = None):
+
+        #input_list = self.input_spec_list_read
+
+        # check if write directories exist and are empty
+        make_dir(self.bkgrnd_output_dir_write)
+        make_dir(self.final_spec_dir_write)
+
+        logging.info("--------------------------")
+        logging.info("Making "+str(self.number_specs)+" realizations of each input spectrum")
+
+        if (self.number_specs > 1) and (self.noise_level == "None"):
+            logging.warning("Realizing multiple spectra but noise level is zero")
+            input("Hit [Enter] to continue")
+
+        # Read list of input spectra
+        # input_list ALREADY SET IN DEFAULTS ## input_list = input_spec_list_read_dir + config_red["file_names"]["LIST_SPEC_PHASE"]
+        list_arr = read_list(self.input_spec_list_read)
+
+        if os.path.isdir(self.cc_bkgrnd_dir):
+            # check if directory exists
+            logging.info("Reading in unnormalized spectra from dir " + self.unnorm_spectra_dir_read)
+        else:
+            logging.warning('Making new directory '+str(self.unnorm_spectra_dir_read)+ ' which will contain contain unnormalized spectra')
+            make_dir(self.cc_bkgrnd_dir)
+
+
+        # Check to make sure the files in the list are actually in the input directory;
+        # if not, just remove those from the list and set a warning
+        list_actually_there = glob.glob(self.unnorm_spectra_dir_read + "*.*")
+        list_actually_basenames = np.array([os.path.basename(t) for t in list_actually_there])
+
+        num_sought = len(list_arr) # number of wanted files
+        num_existing = np.sum(np.in1d(list_arr, list_actually_basenames)) # number of wanted files found
+        bool_present = np.in1d(list_arr, list_actually_basenames, invert=False)
+        bool_missing = np.in1d(list_arr, list_actually_basenames, invert=True)
+        files_missing = list_arr[bool_missing] # files in input list, but not found
+        files_present = list_arr[bool_present] # files in input list, and found
+        num_extra = np.sum(np.in1d(list_actually_basenames, list_arr, invert=True)) # number of extra files found in the input directory
+
+        # did we find all the spectra we wanted?
+        if (num_existing < num_sought):
+            logging.warning("Found only "+str(num_existing)+" of "+str(num_sought)+" spectra in input list")
+            logging.warning("Files missing from input directory:")
+            logging.warning(files_missing)
+        else:
+            logging.info("All spectra in input list found in input directory")
+
+        # did any other spectra appear in the directory, which may or may not be a good thing?
+        if (num_extra > 1):
+            logging.warning("Found "+str(num_extra)+" files in directory which do not appear in input list")
+        else:
+            logging.info("No spectra found in input directory which do not appear in input list.")
+
+        # if there are files missing from the directory, just remove those from the input list
+        list_arr = files_present
+
+        # create noise-churned realizations for each spectrum
+        name_list = list() # initialize
+
+        for i in range(len(list_arr)): # make spectrum realizations and list of their filenames
+            name_list.extend(generate_realizations(spec_name=self.unnorm_spectra_dir_read+"/"+list_arr[i],
+                                                   outdir=self.unnorm_noise_churned_spectra_dir_read,
+                                                   spec_file_format=self.spec_file_type,
+                                                   num=self.number_specs,
+                                                   noise_level=self.noise_level))
+
+        # next we need to normalize the spectra; begin by creating input list of
+        # spectrum realizations written in the previous step
+        bkg_input_file = write_bckgrnd_input(name_list, self.unnorm_noise_churned_spectra_dir_read, self.bkgrnd_output_dir_write)
+        logging.info("-------------------------------------------")
+        logging.info('The file containing the list of spectra which will be fed ' + \
+                    'into the normalization routine is ' + bkg_input_file)
+
+        # normalize each spectrum realization (smoothing parameter is set in __init__)
+        if os.path.isdir(self.cc_bkgrnd_dir):
+            # check if directory exists
+            logging.info('Reading in background binary from '+str(self.cc_bkgrnd_dir))
+        else:
+            logging.warning('Making new directory '+str(self.normzed_spec_source_dir)+ ' which will contain background binary')
+            make_dir(self.cc_bkgrnd_dir)
+
+        bkgrnd = Popen([str(self.cc_bkgrnd_dir) + "bkgrnd", "--smooth "+str(attribs["reduc_params"]["SMOOTH"]),
+                        "--sismoo 1", "--no-plot", "{}".format(bkg_input_file)], stdout=PIPE, stderr=PIPE)
+        (out, err) = bkgrnd.communicate() # returns tuple (stdout, stderr)
+
+        if self.verb == True: # decode messages
+            logging.info(out.decode("utf-8"))
+            logging.info(err.decode("utf-8"))
+
+        # read in input files, normalize them, write out, and return list of those filenames
+        final_list = create_norm_spec(name_list, self.bkgrnd_output_dir_write, self.final_spec_dir_write)
+
+        logging.info("-------------------------------------------")
+        logging.info("Wrote realizations of original spectra to directory")
+        logging.info(self.unnorm_noise_churned_spectra_dir_read)
+        logging.info("-------------------------------------------")
+        logging.info("Wrote raw normalization output to directory")
+        logging.info(self.bkgrnd_output_dir_write)
+        logging.info("-------------------------------------------")
+        logging.info("Wrote final normalized spectra to directory")
+        logging.info(self.final_spec_dir_write)
 
-    return final_list
+        return final_list
```

### Comparing `rrlfe-0.0.9/modules/normalize_simple.py` & `rrlfe-1.0/rrlfe/normalize_simple.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,27 +13,22 @@
 # Standard library dependencies
 # -----------------------------
 import argparse
 import os
 from subprocess import Popen,PIPE
 import sys
 import glob
-## ## import test.so # experimenting with C extensions
 # -------------------
 # Third-party imports
 # -------------------
 from astropy.io import fits
 from astropy.table import Table
 import numpy as np
 from rrlyrae_metallicity.modules2 import *
 
-"""
-FYI text
-"""
-
 # --------------------
 # Function Definitions
 # --------------------
 def junk_np_calc_chisq(data, b, w, coef):
     """
     Calculate chi squared
 
@@ -181,35 +176,14 @@
     OUTPUTS:
     (text files written)
     '''
 
     print("--------------------------")
     print("Normalizing spectra")
 
-    # read file containing list of stemless filenames of science spectra to normalize and
-    # apply calibration to. Note the input science spectra need to have two columns:
-    # [0]: wavelength (angstroms); [1]: unnormalized flux
-    #input_list = input_spec_list_dir + config_apply["file_names"]["LIST_SPEC_APPLY"]
-    #list_arr = read_list(input_list)
-
-    #print(list_arr)
-
-    # make list of stemless filenames for the normalized spectra
-    #name_list = list_arr
-    ##name_list = [s + "_norm" for s in list_arr]
-    ## ## ersatz
-    #name_list = ['spec-2609-54476-0201g001.dat', 'spec-2609-54476-0201g002.dat']
-
-    # create file with list of bkgrnd output filenames
-    #bkg_input_file = write_bckgrnd_input(name_list = name_list,
-    #                                     indir = unnorm_science_spectra_dir,
-    #                                     normdir = bkgrnd_output_dir)
-
-    import ipdb; ipdb.set_trace()
-
     # make list of spectra files in the directory
     unnorm_sci_spectra_list = glob.glob(unnorm_science_spectra_dir + "/*.{*}")
 
     # Normalize each spectrum (smoothing parameter is set in __init__)
     bkgrnd = Popen([str(config_apply["data_dirs"]["DIR_BIN"]) + "bkgrnd", "--smooth "+str(config_apply["reduc_params"]["SMOOTH"]),
                     "--sismoo 1", "--no-plot", "{}".format(bkg_input_file)], stdout=PIPE, stderr=PIPE)
     (out,err) = bkgrnd.communicate() # returns tuple (stdout,stderr)
```

