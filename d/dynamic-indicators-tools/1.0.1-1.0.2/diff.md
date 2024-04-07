# Comparing `tmp/dynamic_indicators_tools-1.0.1.tar.gz` & `tmp/dynamic_indicators_tools-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dynamic_indicators_tools-1.0.1.tar", last modified: Mon Apr  1 21:00:55 2024, max compression
+gzip compressed data, was "dynamic_indicators_tools-1.0.2.tar", last modified: Sun Apr  7 17:11:54 2024, max compression
```

## Comparing `dynamic_indicators_tools-1.0.1.tar` & `dynamic_indicators_tools-1.0.2.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxrwxr-x   0 santhiperbolico  (1000) santhiperbolico  (1000)        0 2024-04-01 21:00:55.969436 dynamic_indicators_tools-1.0.1/
--rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)     1072 2023-09-08 10:49:06.000000 dynamic_indicators_tools-1.0.1/LICENSE
--rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)     7232 2024-04-01 21:00:55.969436 dynamic_indicators_tools-1.0.1/PKG-INFO
--rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)     6746 2023-09-11 23:29:58.000000 dynamic_indicators_tools-1.0.1/README.md
--rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)       38 2024-04-01 21:00:55.969436 dynamic_indicators_tools-1.0.1/setup.cfg
--rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)      862 2024-04-01 20:59:24.000000 dynamic_indicators_tools-1.0.1/setup.py
-drwxrwxr-x   0 santhiperbolico  (1000) santhiperbolico  (1000)        0 2024-04-01 21:00:55.965436 dynamic_indicators_tools-1.0.1/src/
-drwxrwxr-x   0 santhiperbolico  (1000) santhiperbolico  (1000)        0 2024-04-01 21:00:55.965436 dynamic_indicators_tools-1.0.1/src/dynamic_indicators_tools/
--rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)        0 2023-09-08 10:50:04.000000 dynamic_indicators_tools-1.0.1/src/dynamic_indicators_tools/__init__.py
-drwxrwxr-x   0 santhiperbolico  (1000) santhiperbolico  (1000)        0 2024-04-01 21:00:55.965436 dynamic_indicators_tools-1.0.1/src/dynamic_indicators_tools/differentials_systems/
--rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)        0 2023-09-08 10:50:04.000000 dynamic_indicators_tools-1.0.1/src/dynamic_indicators_tools/differentials_systems/__init__.py
--rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)     1829 2023-09-08 10:50:04.000000 dynamic_indicators_tools-1.0.1/src/dynamic_indicators_tools/differentials_systems/data_transformations.py
--rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)    13333 2024-04-01 20:57:01.000000 dynamic_indicators_tools-1.0.1/src/dynamic_indicators_tools/differentials_systems/diff_system.py
--rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)     5769 2023-09-08 10:50:04.000000 dynamic_indicators_tools-1.0.1/src/dynamic_indicators_tools/differentials_systems/solver_integrators.py
-drwxrwxr-x   0 santhiperbolico  (1000) santhiperbolico  (1000)        0 2024-04-01 21:00:55.965436 dynamic_indicators_tools-1.0.1/src/dynamic_indicators_tools/dynamic_indicators/
--rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)        0 2023-09-08 10:50:04.000000 dynamic_indicators_tools-1.0.1/src/dynamic_indicators_tools/dynamic_indicators/__init__.py
--rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)     1863 2024-04-01 20:57:01.000000 dynamic_indicators_tools-1.0.1/src/dynamic_indicators_tools/dynamic_indicators/dynamic_indicators_process.py
--rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)     3431 2024-04-01 20:57:01.000000 dynamic_indicators_tools-1.0.1/src/dynamic_indicators_tools/dynamic_indicators/dynamic_indicators_utils.py
-drwxrwxr-x   0 santhiperbolico  (1000) santhiperbolico  (1000)        0 2024-04-01 21:00:55.965436 dynamic_indicators_tools-1.0.1/src/dynamic_indicators_tools/dynamic_indicators/finite_time_lyapunov_exponents/
--rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)        0 2024-04-01 20:57:01.000000 dynamic_indicators_tools-1.0.1/src/dynamic_indicators_tools/dynamic_indicators/finite_time_lyapunov_exponents/__init__.py
--rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)    17262 2024-04-01 20:57:01.000000 dynamic_indicators_tools-1.0.1/src/dynamic_indicators_tools/dynamic_indicators/finite_time_lyapunov_exponents/ftle_indicator.py
--rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)     3097 2024-04-01 20:57:01.000000 dynamic_indicators_tools-1.0.1/src/dynamic_indicators_tools/dynamic_indicators/finite_time_lyapunov_exponents/ftle_params.py
--rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)    17540 2024-04-01 20:57:01.000000 dynamic_indicators_tools-1.0.1/src/dynamic_indicators_tools/dynamic_indicators/finite_time_lyapunov_exponents/ftle_utils.py
-drwxrwxr-x   0 santhiperbolico  (1000) santhiperbolico  (1000)        0 2024-04-01 21:00:55.965436 dynamic_indicators_tools-1.0.1/src/dynamic_indicators_tools/dynamic_indicators/lagrangian_descriptors/
--rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)        0 2024-04-01 20:57:01.000000 dynamic_indicators_tools-1.0.1/src/dynamic_indicators_tools/dynamic_indicators/lagrangian_descriptors/__init__.py
--rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)     6506 2024-04-01 20:57:01.000000 dynamic_indicators_tools-1.0.1/src/dynamic_indicators_tools/dynamic_indicators/lagrangian_descriptors/ld_indicator.py
--rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)      927 2024-04-01 20:57:01.000000 dynamic_indicators_tools-1.0.1/src/dynamic_indicators_tools/dynamic_indicators/lagrangian_descriptors/ld_params.py
--rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)    13642 2024-04-01 20:57:01.000000 dynamic_indicators_tools-1.0.1/src/dynamic_indicators_tools/dynamic_indicators/lagrangian_descriptors/ld_utils.py
--rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)    10224 2024-04-01 20:57:01.000000 dynamic_indicators_tools-1.0.1/src/dynamic_indicators_tools/dynamic_indicators/params_methods.py
--rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)     4748 2024-04-01 20:57:01.000000 dynamic_indicators_tools-1.0.1/src/dynamic_indicators_tools/dynamic_indicators/plot_descriptors.py
-drwxrwxr-x   0 santhiperbolico  (1000) santhiperbolico  (1000)        0 2024-04-01 21:00:55.965436 dynamic_indicators_tools-1.0.1/src/dynamic_indicators_tools/dynamic_indicators/poincare_maps/
--rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)        0 2024-04-01 20:57:01.000000 dynamic_indicators_tools-1.0.1/src/dynamic_indicators_tools/dynamic_indicators/poincare_maps/__init__.py
--rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)     6358 2024-04-01 20:57:01.000000 dynamic_indicators_tools-1.0.1/src/dynamic_indicators_tools/dynamic_indicators/poincare_maps/poincare_indicator.py
--rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)     1842 2024-04-01 20:57:01.000000 dynamic_indicators_tools-1.0.1/src/dynamic_indicators_tools/dynamic_indicators/poincare_maps/poincare_params.py
--rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)    19000 2024-04-01 20:57:01.000000 dynamic_indicators_tools-1.0.1/src/dynamic_indicators_tools/dynamic_indicators/poincare_maps/poincare_utils.py
--rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)      796 2024-04-01 20:57:01.000000 dynamic_indicators_tools-1.0.1/src/dynamic_indicators_tools/main_dynamic_indicators_process.py
-drwxrwxr-x   0 santhiperbolico  (1000) santhiperbolico  (1000)        0 2024-04-01 21:00:55.965436 dynamic_indicators_tools-1.0.1/src/dynamic_indicators_tools/numercial_methods/
--rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)        0 2023-09-08 10:50:04.000000 dynamic_indicators_tools-1.0.1/src/dynamic_indicators_tools/numercial_methods/__init__.py
--rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)     6398 2023-09-08 10:50:04.000000 dynamic_indicators_tools-1.0.1/src/dynamic_indicators_tools/numercial_methods/differentiation.py
--rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)     3329 2023-09-08 10:50:04.000000 dynamic_indicators_tools-1.0.1/src/dynamic_indicators_tools/numercial_methods/integrators.py
-drwxrwxr-x   0 santhiperbolico  (1000) santhiperbolico  (1000)        0 2024-04-01 21:00:55.965436 dynamic_indicators_tools-1.0.1/src/dynamic_indicators_tools.egg-info/
--rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)     7232 2024-04-01 21:00:55.000000 dynamic_indicators_tools-1.0.1/src/dynamic_indicators_tools.egg-info/PKG-INFO
--rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)     2606 2024-04-01 21:00:55.000000 dynamic_indicators_tools-1.0.1/src/dynamic_indicators_tools.egg-info/SOURCES.txt
--rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)        1 2024-04-01 21:00:55.000000 dynamic_indicators_tools-1.0.1/src/dynamic_indicators_tools.egg-info/dependency_links.txt
--rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)       40 2024-04-01 21:00:55.000000 dynamic_indicators_tools-1.0.1/src/dynamic_indicators_tools.egg-info/requires.txt
--rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)       31 2024-04-01 21:00:55.000000 dynamic_indicators_tools-1.0.1/src/dynamic_indicators_tools.egg-info/top_level.txt
-drwxrwxr-x   0 santhiperbolico  (1000) santhiperbolico  (1000)        0 2024-04-01 21:00:55.969436 dynamic_indicators_tools-1.0.1/src/tests/
--rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)        0 2023-09-08 10:50:04.000000 dynamic_indicators_tools-1.0.1/src/tests/__init__.py
--rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)     2378 2023-09-08 10:50:04.000000 dynamic_indicators_tools-1.0.1/src/tests/test_data_transformations.py
--rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)     7833 2023-09-08 10:50:04.000000 dynamic_indicators_tools-1.0.1/src/tests/test_diff_systems.py
--rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)     5757 2023-09-08 10:50:04.000000 dynamic_indicators_tools-1.0.1/src/tests/test_differentiation.py
--rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)     1938 2024-04-01 20:57:01.000000 dynamic_indicators_tools-1.0.1/src/tests/test_dynamic_indicators_process.py
--rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)     8630 2024-04-01 20:57:01.000000 dynamic_indicators_tools-1.0.1/src/tests/test_finite_time_lyapunov_exponents.py
--rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)     3045 2024-04-01 20:57:01.000000 dynamic_indicators_tools-1.0.1/src/tests/test_lagrangian_descriptors.py
--rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)     4785 2024-04-01 20:57:01.000000 dynamic_indicators_tools-1.0.1/src/tests/test_params_method.py
--rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)     4244 2024-04-01 20:57:01.000000 dynamic_indicators_tools-1.0.1/src/tests/test_poincare_map.py
--rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)     4426 2023-09-08 11:19:22.000000 dynamic_indicators_tools-1.0.1/src/tests/test_system_black_hole_schwarzchids.py
+drwxrwxr-x   0 santhiperbolico  (1000) santhiperbolico  (1000)        0 2024-04-07 17:11:54.860159 dynamic_indicators_tools-1.0.2/
+-rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)     1072 2023-09-08 10:49:06.000000 dynamic_indicators_tools-1.0.2/LICENSE
+-rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)     7232 2024-04-07 17:11:54.860159 dynamic_indicators_tools-1.0.2/PKG-INFO
+-rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)     6746 2023-09-11 23:29:58.000000 dynamic_indicators_tools-1.0.2/README.md
+-rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)       38 2024-04-07 17:11:54.860159 dynamic_indicators_tools-1.0.2/setup.cfg
+-rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)      862 2024-04-07 17:11:33.000000 dynamic_indicators_tools-1.0.2/setup.py
+drwxrwxr-x   0 santhiperbolico  (1000) santhiperbolico  (1000)        0 2024-04-07 17:11:54.848158 dynamic_indicators_tools-1.0.2/src/
+drwxrwxr-x   0 santhiperbolico  (1000) santhiperbolico  (1000)        0 2024-04-07 17:11:54.848158 dynamic_indicators_tools-1.0.2/src/dynamic_indicators_tools/
+-rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)        0 2023-09-08 10:50:04.000000 dynamic_indicators_tools-1.0.2/src/dynamic_indicators_tools/__init__.py
+drwxrwxr-x   0 santhiperbolico  (1000) santhiperbolico  (1000)        0 2024-04-07 17:11:54.848158 dynamic_indicators_tools-1.0.2/src/dynamic_indicators_tools/differentials_systems/
+-rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)        0 2023-09-08 10:50:04.000000 dynamic_indicators_tools-1.0.2/src/dynamic_indicators_tools/differentials_systems/__init__.py
+-rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)     1829 2023-09-08 10:50:04.000000 dynamic_indicators_tools-1.0.2/src/dynamic_indicators_tools/differentials_systems/data_transformations.py
+-rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)    13333 2024-04-01 20:57:01.000000 dynamic_indicators_tools-1.0.2/src/dynamic_indicators_tools/differentials_systems/diff_system.py
+-rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)     5769 2023-09-08 10:50:04.000000 dynamic_indicators_tools-1.0.2/src/dynamic_indicators_tools/differentials_systems/solver_integrators.py
+drwxrwxr-x   0 santhiperbolico  (1000) santhiperbolico  (1000)        0 2024-04-07 17:11:54.852158 dynamic_indicators_tools-1.0.2/src/dynamic_indicators_tools/dynamic_indicators/
+-rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)        0 2023-09-08 10:50:04.000000 dynamic_indicators_tools-1.0.2/src/dynamic_indicators_tools/dynamic_indicators/__init__.py
+-rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)     1863 2024-04-01 20:57:01.000000 dynamic_indicators_tools-1.0.2/src/dynamic_indicators_tools/dynamic_indicators/dynamic_indicators_process.py
+-rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)     3431 2024-04-01 20:57:01.000000 dynamic_indicators_tools-1.0.2/src/dynamic_indicators_tools/dynamic_indicators/dynamic_indicators_utils.py
+drwxrwxr-x   0 santhiperbolico  (1000) santhiperbolico  (1000)        0 2024-04-07 17:11:54.852158 dynamic_indicators_tools-1.0.2/src/dynamic_indicators_tools/dynamic_indicators/finite_time_lyapunov_exponents/
+-rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)        0 2024-04-01 20:57:01.000000 dynamic_indicators_tools-1.0.2/src/dynamic_indicators_tools/dynamic_indicators/finite_time_lyapunov_exponents/__init__.py
+-rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)    17262 2024-04-01 20:57:01.000000 dynamic_indicators_tools-1.0.2/src/dynamic_indicators_tools/dynamic_indicators/finite_time_lyapunov_exponents/ftle_indicator.py
+-rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)     3097 2024-04-01 20:57:01.000000 dynamic_indicators_tools-1.0.2/src/dynamic_indicators_tools/dynamic_indicators/finite_time_lyapunov_exponents/ftle_params.py
+-rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)    17540 2024-04-01 20:57:01.000000 dynamic_indicators_tools-1.0.2/src/dynamic_indicators_tools/dynamic_indicators/finite_time_lyapunov_exponents/ftle_utils.py
+drwxrwxr-x   0 santhiperbolico  (1000) santhiperbolico  (1000)        0 2024-04-07 17:11:54.852158 dynamic_indicators_tools-1.0.2/src/dynamic_indicators_tools/dynamic_indicators/lagrangian_descriptors/
+-rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)        0 2024-04-01 20:57:01.000000 dynamic_indicators_tools-1.0.2/src/dynamic_indicators_tools/dynamic_indicators/lagrangian_descriptors/__init__.py
+-rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)     6506 2024-04-01 20:57:01.000000 dynamic_indicators_tools-1.0.2/src/dynamic_indicators_tools/dynamic_indicators/lagrangian_descriptors/ld_indicator.py
+-rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)      927 2024-04-01 20:57:01.000000 dynamic_indicators_tools-1.0.2/src/dynamic_indicators_tools/dynamic_indicators/lagrangian_descriptors/ld_params.py
+-rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)    13642 2024-04-01 20:57:01.000000 dynamic_indicators_tools-1.0.2/src/dynamic_indicators_tools/dynamic_indicators/lagrangian_descriptors/ld_utils.py
+-rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)    10224 2024-04-01 20:57:01.000000 dynamic_indicators_tools-1.0.2/src/dynamic_indicators_tools/dynamic_indicators/params_methods.py
+-rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)     4748 2024-04-01 20:57:01.000000 dynamic_indicators_tools-1.0.2/src/dynamic_indicators_tools/dynamic_indicators/plot_descriptors.py
+drwxrwxr-x   0 santhiperbolico  (1000) santhiperbolico  (1000)        0 2024-04-07 17:11:54.856158 dynamic_indicators_tools-1.0.2/src/dynamic_indicators_tools/dynamic_indicators/poincare_maps/
+-rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)        0 2024-04-01 20:57:01.000000 dynamic_indicators_tools-1.0.2/src/dynamic_indicators_tools/dynamic_indicators/poincare_maps/__init__.py
+-rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)     6358 2024-04-01 20:57:01.000000 dynamic_indicators_tools-1.0.2/src/dynamic_indicators_tools/dynamic_indicators/poincare_maps/poincare_indicator.py
+-rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)     1842 2024-04-01 20:57:01.000000 dynamic_indicators_tools-1.0.2/src/dynamic_indicators_tools/dynamic_indicators/poincare_maps/poincare_params.py
+-rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)    19000 2024-04-01 20:57:01.000000 dynamic_indicators_tools-1.0.2/src/dynamic_indicators_tools/dynamic_indicators/poincare_maps/poincare_utils.py
+-rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)     1020 2024-04-07 17:11:33.000000 dynamic_indicators_tools-1.0.2/src/dynamic_indicators_tools/main_dynamic_indicators_process.py
+drwxrwxr-x   0 santhiperbolico  (1000) santhiperbolico  (1000)        0 2024-04-07 17:11:54.856158 dynamic_indicators_tools-1.0.2/src/dynamic_indicators_tools/numercial_methods/
+-rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)        0 2023-09-08 10:50:04.000000 dynamic_indicators_tools-1.0.2/src/dynamic_indicators_tools/numercial_methods/__init__.py
+-rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)     6398 2023-09-08 10:50:04.000000 dynamic_indicators_tools-1.0.2/src/dynamic_indicators_tools/numercial_methods/differentiation.py
+-rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)     3329 2023-09-08 10:50:04.000000 dynamic_indicators_tools-1.0.2/src/dynamic_indicators_tools/numercial_methods/integrators.py
+drwxrwxr-x   0 santhiperbolico  (1000) santhiperbolico  (1000)        0 2024-04-07 17:11:54.848158 dynamic_indicators_tools-1.0.2/src/dynamic_indicators_tools.egg-info/
+-rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)     7232 2024-04-07 17:11:54.000000 dynamic_indicators_tools-1.0.2/src/dynamic_indicators_tools.egg-info/PKG-INFO
+-rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)     2606 2024-04-07 17:11:54.000000 dynamic_indicators_tools-1.0.2/src/dynamic_indicators_tools.egg-info/SOURCES.txt
+-rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)        1 2024-04-07 17:11:54.000000 dynamic_indicators_tools-1.0.2/src/dynamic_indicators_tools.egg-info/dependency_links.txt
+-rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)       40 2024-04-07 17:11:54.000000 dynamic_indicators_tools-1.0.2/src/dynamic_indicators_tools.egg-info/requires.txt
+-rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)       31 2024-04-07 17:11:54.000000 dynamic_indicators_tools-1.0.2/src/dynamic_indicators_tools.egg-info/top_level.txt
+drwxrwxr-x   0 santhiperbolico  (1000) santhiperbolico  (1000)        0 2024-04-07 17:11:54.860159 dynamic_indicators_tools-1.0.2/src/tests/
+-rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)        0 2023-09-08 10:50:04.000000 dynamic_indicators_tools-1.0.2/src/tests/__init__.py
+-rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)     2378 2023-09-08 10:50:04.000000 dynamic_indicators_tools-1.0.2/src/tests/test_data_transformations.py
+-rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)     7833 2023-09-08 10:50:04.000000 dynamic_indicators_tools-1.0.2/src/tests/test_diff_systems.py
+-rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)     5757 2023-09-08 10:50:04.000000 dynamic_indicators_tools-1.0.2/src/tests/test_differentiation.py
+-rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)     1938 2024-04-01 20:57:01.000000 dynamic_indicators_tools-1.0.2/src/tests/test_dynamic_indicators_process.py
+-rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)     8630 2024-04-01 20:57:01.000000 dynamic_indicators_tools-1.0.2/src/tests/test_finite_time_lyapunov_exponents.py
+-rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)     3045 2024-04-01 20:57:01.000000 dynamic_indicators_tools-1.0.2/src/tests/test_lagrangian_descriptors.py
+-rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)     4785 2024-04-01 20:57:01.000000 dynamic_indicators_tools-1.0.2/src/tests/test_params_method.py
+-rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)     4244 2024-04-01 20:57:01.000000 dynamic_indicators_tools-1.0.2/src/tests/test_poincare_map.py
+-rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)     4426 2023-09-08 11:19:22.000000 dynamic_indicators_tools-1.0.2/src/tests/test_system_black_hole_schwarzchids.py
```

### Comparing `dynamic_indicators_tools-1.0.1/LICENSE` & `dynamic_indicators_tools-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dynamic_indicators_tools-1.0.1/PKG-INFO` & `dynamic_indicators_tools-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dynamic_indicators_tools
-Version: 1.0.1
+Version: 1.0.2
 Summary: Repositorio que recoge herramientas para el análisis de sistemas dinámicos
 Home-page: https://github.com/santhiperbolico/dynamic_indicators_tools
 Author: Santiago Arranz Sanz
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `dynamic_indicators_tools-1.0.1/README.md` & `dynamic_indicators_tools-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `dynamic_indicators_tools-1.0.1/setup.py` & `dynamic_indicators_tools-1.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="dynamic_indicators_tools",
-    version="1.0.1",
+    version="1.0.2",
     author="Santiago Arranz Sanz",
     description="Repositorio que recoge herramientas para el análisis de sistemas dinámicos",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(where="src"),
     url="https://github.com/santhiperbolico/dynamic_indicators_tools",
     classifiers=[
```

### Comparing `dynamic_indicators_tools-1.0.1/src/dynamic_indicators_tools/differentials_systems/data_transformations.py` & `dynamic_indicators_tools-1.0.2/src/dynamic_indicators_tools/differentials_systems/data_transformations.py`

 * *Files identical despite different names*

### Comparing `dynamic_indicators_tools-1.0.1/src/dynamic_indicators_tools/differentials_systems/diff_system.py` & `dynamic_indicators_tools-1.0.2/src/dynamic_indicators_tools/differentials_systems/diff_system.py`

 * *Files identical despite different names*

### Comparing `dynamic_indicators_tools-1.0.1/src/dynamic_indicators_tools/differentials_systems/solver_integrators.py` & `dynamic_indicators_tools-1.0.2/src/dynamic_indicators_tools/differentials_systems/solver_integrators.py`

 * *Files identical despite different names*

### Comparing `dynamic_indicators_tools-1.0.1/src/dynamic_indicators_tools/dynamic_indicators/dynamic_indicators_process.py` & `dynamic_indicators_tools-1.0.2/src/dynamic_indicators_tools/dynamic_indicators/dynamic_indicators_process.py`

 * *Files identical despite different names*

### Comparing `dynamic_indicators_tools-1.0.1/src/dynamic_indicators_tools/dynamic_indicators/dynamic_indicators_utils.py` & `dynamic_indicators_tools-1.0.2/src/dynamic_indicators_tools/dynamic_indicators/dynamic_indicators_utils.py`

 * *Files identical despite different names*

### Comparing `dynamic_indicators_tools-1.0.1/src/dynamic_indicators_tools/dynamic_indicators/finite_time_lyapunov_exponents/ftle_indicator.py` & `dynamic_indicators_tools-1.0.2/src/dynamic_indicators_tools/dynamic_indicators/finite_time_lyapunov_exponents/ftle_indicator.py`

 * *Files identical despite different names*

### Comparing `dynamic_indicators_tools-1.0.1/src/dynamic_indicators_tools/dynamic_indicators/finite_time_lyapunov_exponents/ftle_params.py` & `dynamic_indicators_tools-1.0.2/src/dynamic_indicators_tools/dynamic_indicators/finite_time_lyapunov_exponents/ftle_params.py`

 * *Files identical despite different names*

### Comparing `dynamic_indicators_tools-1.0.1/src/dynamic_indicators_tools/dynamic_indicators/finite_time_lyapunov_exponents/ftle_utils.py` & `dynamic_indicators_tools-1.0.2/src/dynamic_indicators_tools/dynamic_indicators/finite_time_lyapunov_exponents/ftle_utils.py`

 * *Files identical despite different names*

### Comparing `dynamic_indicators_tools-1.0.1/src/dynamic_indicators_tools/dynamic_indicators/lagrangian_descriptors/ld_indicator.py` & `dynamic_indicators_tools-1.0.2/src/dynamic_indicators_tools/dynamic_indicators/lagrangian_descriptors/ld_indicator.py`

 * *Files identical despite different names*

### Comparing `dynamic_indicators_tools-1.0.1/src/dynamic_indicators_tools/dynamic_indicators/lagrangian_descriptors/ld_params.py` & `dynamic_indicators_tools-1.0.2/src/dynamic_indicators_tools/dynamic_indicators/lagrangian_descriptors/ld_params.py`

 * *Files identical despite different names*

### Comparing `dynamic_indicators_tools-1.0.1/src/dynamic_indicators_tools/dynamic_indicators/lagrangian_descriptors/ld_utils.py` & `dynamic_indicators_tools-1.0.2/src/dynamic_indicators_tools/dynamic_indicators/lagrangian_descriptors/ld_utils.py`

 * *Files identical despite different names*

### Comparing `dynamic_indicators_tools-1.0.1/src/dynamic_indicators_tools/dynamic_indicators/params_methods.py` & `dynamic_indicators_tools-1.0.2/src/dynamic_indicators_tools/dynamic_indicators/params_methods.py`

 * *Files identical despite different names*

### Comparing `dynamic_indicators_tools-1.0.1/src/dynamic_indicators_tools/dynamic_indicators/plot_descriptors.py` & `dynamic_indicators_tools-1.0.2/src/dynamic_indicators_tools/dynamic_indicators/plot_descriptors.py`

 * *Files identical despite different names*

### Comparing `dynamic_indicators_tools-1.0.1/src/dynamic_indicators_tools/dynamic_indicators/poincare_maps/poincare_indicator.py` & `dynamic_indicators_tools-1.0.2/src/dynamic_indicators_tools/dynamic_indicators/poincare_maps/poincare_indicator.py`

 * *Files identical despite different names*

### Comparing `dynamic_indicators_tools-1.0.1/src/dynamic_indicators_tools/dynamic_indicators/poincare_maps/poincare_params.py` & `dynamic_indicators_tools-1.0.2/src/dynamic_indicators_tools/dynamic_indicators/poincare_maps/poincare_params.py`

 * *Files identical despite different names*

### Comparing `dynamic_indicators_tools-1.0.1/src/dynamic_indicators_tools/dynamic_indicators/poincare_maps/poincare_utils.py` & `dynamic_indicators_tools-1.0.2/src/dynamic_indicators_tools/dynamic_indicators/poincare_maps/poincare_utils.py`

 * *Files identical despite different names*

### Comparing `dynamic_indicators_tools-1.0.1/src/dynamic_indicators_tools/numercial_methods/differentiation.py` & `dynamic_indicators_tools-1.0.2/src/dynamic_indicators_tools/numercial_methods/differentiation.py`

 * *Files identical despite different names*

### Comparing `dynamic_indicators_tools-1.0.1/src/dynamic_indicators_tools/numercial_methods/integrators.py` & `dynamic_indicators_tools-1.0.2/src/dynamic_indicators_tools/numercial_methods/integrators.py`

 * *Files identical despite different names*

### Comparing `dynamic_indicators_tools-1.0.1/src/dynamic_indicators_tools.egg-info/PKG-INFO` & `dynamic_indicators_tools-1.0.2/src/dynamic_indicators_tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dynamic-indicators-tools
-Version: 1.0.1
+Version: 1.0.2
 Summary: Repositorio que recoge herramientas para el análisis de sistemas dinámicos
 Home-page: https://github.com/santhiperbolico/dynamic_indicators_tools
 Author: Santiago Arranz Sanz
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `dynamic_indicators_tools-1.0.1/src/dynamic_indicators_tools.egg-info/SOURCES.txt` & `dynamic_indicators_tools-1.0.2/src/dynamic_indicators_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dynamic_indicators_tools-1.0.1/src/tests/test_data_transformations.py` & `dynamic_indicators_tools-1.0.2/src/tests/test_data_transformations.py`

 * *Files identical despite different names*

### Comparing `dynamic_indicators_tools-1.0.1/src/tests/test_diff_systems.py` & `dynamic_indicators_tools-1.0.2/src/tests/test_diff_systems.py`

 * *Files identical despite different names*

### Comparing `dynamic_indicators_tools-1.0.1/src/tests/test_differentiation.py` & `dynamic_indicators_tools-1.0.2/src/tests/test_differentiation.py`

 * *Files identical despite different names*

### Comparing `dynamic_indicators_tools-1.0.1/src/tests/test_dynamic_indicators_process.py` & `dynamic_indicators_tools-1.0.2/src/tests/test_dynamic_indicators_process.py`

 * *Files identical despite different names*

### Comparing `dynamic_indicators_tools-1.0.1/src/tests/test_finite_time_lyapunov_exponents.py` & `dynamic_indicators_tools-1.0.2/src/tests/test_finite_time_lyapunov_exponents.py`

 * *Files identical despite different names*

### Comparing `dynamic_indicators_tools-1.0.1/src/tests/test_lagrangian_descriptors.py` & `dynamic_indicators_tools-1.0.2/src/tests/test_lagrangian_descriptors.py`

 * *Files identical despite different names*

### Comparing `dynamic_indicators_tools-1.0.1/src/tests/test_params_method.py` & `dynamic_indicators_tools-1.0.2/src/tests/test_params_method.py`

 * *Files identical despite different names*

### Comparing `dynamic_indicators_tools-1.0.1/src/tests/test_poincare_map.py` & `dynamic_indicators_tools-1.0.2/src/tests/test_poincare_map.py`

 * *Files identical despite different names*

### Comparing `dynamic_indicators_tools-1.0.1/src/tests/test_system_black_hole_schwarzchids.py` & `dynamic_indicators_tools-1.0.2/src/tests/test_system_black_hole_schwarzchids.py`

 * *Files identical despite different names*

