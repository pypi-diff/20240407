# Comparing `tmp/feloopy-0.2.8.tar.gz` & `tmp/feloopy-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feloopy-0.2.8.tar", last modified: Mon Dec 25 13:28:43 2023, max compression
+gzip compressed data, was "feloopy-0.2.9.tar", last modified: Sun Apr  7 21:21:03 2024, max compression
```

## Comparing `feloopy-0.2.8.tar` & `feloopy-0.2.9.tar`

### file list

```diff
@@ -1,164 +1,187 @@
-drwxr-xr-x   0 keivant   (1000) keivant   (1000)        0 2023-12-25 13:28:43.604375 feloopy-0.2.8/
--rwxr-xr-x   0 keivant   (1000) keivant   (1000)     1100 2023-12-25 13:21:32.000000 feloopy-0.2.8/LICENSE
--rw-r--r--   0 keivant   (1000) keivant   (1000)    77973 2023-12-25 13:28:43.604375 feloopy-0.2.8/PKG-INFO
-drwxr-xr-x   0 keivant   (1000) keivant   (1000)        0 2023-12-25 13:28:43.571041 feloopy-0.2.8/feloopy/
--rwxr-xr-x   0 keivant   (1000) keivant   (1000)    15501 2023-12-25 13:21:32.000000 feloopy-0.2.8/feloopy/__init__.py
-drwxr-xr-x   0 keivant   (1000) keivant   (1000)        0 2023-12-25 13:28:43.574375 feloopy-0.2.8/feloopy/algorithms/
--rwxr-xr-x   0 keivant   (1000) keivant   (1000)      117 2023-12-25 13:21:32.000000 feloopy-0.2.8/feloopy/algorithms/__init__.py
-drwxr-xr-x   0 keivant   (1000) keivant   (1000)        0 2023-12-25 13:28:43.574375 feloopy-0.2.8/feloopy/algorithms/constraint/
--rwxr-xr-x   0 keivant   (1000) keivant   (1000)      117 2023-12-25 13:21:32.000000 feloopy-0.2.8/feloopy/algorithms/constraint/__init__.py
-drwxr-xr-x   0 keivant   (1000) keivant   (1000)        0 2023-12-25 13:28:43.574375 feloopy-0.2.8/feloopy/algorithms/exact/
--rwxr-xr-x   0 keivant   (1000) keivant   (1000)      117 2023-12-25 13:21:32.000000 feloopy-0.2.8/feloopy/algorithms/exact/__init__.py
--rwxr-xr-x   0 keivant   (1000) keivant   (1000)      117 2023-12-25 13:21:32.000000 feloopy-0.2.8/feloopy/algorithms/exact/benders.py
-drwxr-xr-x   0 keivant   (1000) keivant   (1000)        0 2023-12-25 13:28:43.574375 feloopy-0.2.8/feloopy/algorithms/heuristic/
--rwxr-xr-x   0 keivant   (1000) keivant   (1000)     2941 2023-12-25 13:21:32.000000 feloopy-0.2.8/feloopy/algorithms/heuristic/DE.py
--rwxr-xr-x   0 keivant   (1000) keivant   (1000)     3867 2023-12-25 13:21:32.000000 feloopy-0.2.8/feloopy/algorithms/heuristic/GA.py
--rwxr-xr-x   0 keivant   (1000) keivant   (1000)     2549 2023-12-25 13:21:32.000000 feloopy-0.2.8/feloopy/algorithms/heuristic/GWO.py
--rwxr-xr-x   0 keivant   (1000) keivant   (1000)     3891 2023-12-25 13:21:32.000000 feloopy-0.2.8/feloopy/algorithms/heuristic/SA.py
--rwxr-xr-x   0 keivant   (1000) keivant   (1000)     1995 2023-12-25 13:21:32.000000 feloopy-0.2.8/feloopy/algorithms/heuristic/TS.py
--rwxr-xr-x   0 keivant   (1000) keivant   (1000)      117 2023-12-25 13:21:32.000000 feloopy-0.2.8/feloopy/algorithms/heuristic/__init__.py
-drwxr-xr-x   0 keivant   (1000) keivant   (1000)        0 2023-12-25 13:28:43.574375 feloopy-0.2.8/feloopy/classes/
--rw-r--r--   0 keivant   (1000) keivant   (1000)      117 2023-12-25 13:21:32.000000 feloopy-0.2.8/feloopy/classes/__init__.py
--rw-r--r--   0 keivant   (1000) keivant   (1000)    24230 2023-12-25 13:21:32.000000 feloopy-0.2.8/feloopy/classes/constraint_programming.py
--rw-r--r--   0 keivant   (1000) keivant   (1000)     3801 2023-12-25 13:21:32.000000 feloopy-0.2.8/feloopy/classes/event_variable.py
--rw-r--r--   0 keivant   (1000) keivant   (1000)     2106 2023-12-25 13:21:32.000000 feloopy-0.2.8/feloopy/classes/event_variable_collection.py
--rw-r--r--   0 keivant   (1000) keivant   (1000)    14094 2023-12-25 13:21:32.000000 feloopy-0.2.8/feloopy/classes/linearization.py
--rw-r--r--   0 keivant   (1000) keivant   (1000)    12025 2023-12-25 13:21:32.000000 feloopy-0.2.8/feloopy/classes/multidim_variable.py
--rw-r--r--   0 keivant   (1000) keivant   (1000)     8645 2023-12-25 13:21:32.000000 feloopy-0.2.8/feloopy/classes/multidim_variable_collection.py
--rw-r--r--   0 keivant   (1000) keivant   (1000)    15879 2023-12-25 13:21:32.000000 feloopy-0.2.8/feloopy/classes/special_constraint.py
--rw-r--r--   0 keivant   (1000) keivant   (1000)     7989 2023-12-25 13:21:32.000000 feloopy-0.2.8/feloopy/classes/tensor_variable.py
--rw-r--r--   0 keivant   (1000) keivant   (1000)     7849 2023-12-25 13:21:32.000000 feloopy-0.2.8/feloopy/classes/tensor_variable_collection.py
--rw-r--r--   0 keivant   (1000) keivant   (1000)     3103 2023-12-25 13:21:32.000000 feloopy-0.2.8/feloopy/cli.py
-drwxr-xr-x   0 keivant   (1000) keivant   (1000)        0 2023-12-25 13:28:43.577708 feloopy-0.2.8/feloopy/clitools/
--rw-r--r--   0 keivant   (1000) keivant   (1000)      175 2023-12-25 13:21:32.000000 feloopy-0.2.8/feloopy/clitools/__init__.py
--rw-r--r--   0 keivant   (1000) keivant   (1000)     1338 2023-12-25 13:21:32.000000 feloopy-0.2.8/feloopy/clitools/pkg_manager_detector.py
--rw-r--r--   0 keivant   (1000) keivant   (1000)    14168 2023-12-25 13:21:32.000000 feloopy-0.2.8/feloopy/clitools/utils.py
--rwxr-xr-x   0 keivant   (1000) keivant   (1000)   168915 2023-12-25 13:21:32.000000 feloopy-0.2.8/feloopy/feloopy.py
-drwxr-xr-x   0 keivant   (1000) keivant   (1000)        0 2023-12-25 13:28:43.577708 feloopy-0.2.8/feloopy/generators/
--rwxr-xr-x   0 keivant   (1000) keivant   (1000)      246 2023-12-25 13:21:32.000000 feloopy-0.2.8/feloopy/generators/__init__.py
-drwxr-xr-x   0 keivant   (1000) keivant   (1000)        0 2023-12-25 13:28:43.584375 feloopy-0.2.8/feloopy/generators/model/
--rwxr-xr-x   0 keivant   (1000) keivant   (1000)      117 2023-12-25 13:21:32.000000 feloopy-0.2.8/feloopy/generators/model/__init__.py
--rwxr-xr-x   0 keivant   (1000) keivant   (1000)      310 2023-12-25 13:21:32.000000 feloopy-0.2.8/feloopy/generators/model/copt_model_generator.py
--rwxr-xr-x   0 keivant   (1000) keivant   (1000)      253 2023-12-25 13:21:32.000000 feloopy-0.2.8/feloopy/generators/model/cplex_cp_model_generator.py
--rwxr-xr-x   0 keivant   (1000) keivant   (1000)      620 2023-12-25 13:21:32.000000 feloopy-0.2.8/feloopy/generators/model/cplex_model_generator.py
--rwxr-xr-x   0 keivant   (1000) keivant   (1000)      582 2023-12-25 13:21:32.000000 feloopy-0.2.8/feloopy/generators/model/cvxpy_model_generator.py
--rwxr-xr-x   0 keivant   (1000) keivant   (1000)      635 2023-12-25 13:21:32.000000 feloopy-0.2.8/feloopy/generators/model/cylp_model_generator.py
--rwxr-xr-x   0 keivant   (1000) keivant   (1000)     4863 2023-12-25 13:21:32.000000 feloopy-0.2.8/feloopy/generators/model/feloopy_model_generator.py
--rwxr-xr-x   0 keivant   (1000) keivant   (1000)      629 2023-12-25 13:21:32.000000 feloopy-0.2.8/feloopy/generators/model/gekko_model_generator.py
--rwxr-xr-x   0 keivant   (1000) keivant   (1000)      615 2023-12-25 13:21:32.000000 feloopy-0.2.8/feloopy/generators/model/gurobi_model_generator.py
--rwxr-xr-x   0 keivant   (1000) keivant   (1000)      586 2023-12-25 13:21:32.000000 feloopy-0.2.8/feloopy/generators/model/linopy_model_generator.py
--rw-r--r--   0 keivant   (1000) keivant   (1000)      682 2023-12-25 13:21:32.000000 feloopy-0.2.8/feloopy/generators/model/localsolver_model_generator.py
--rwxr-xr-x   0 keivant   (1000) keivant   (1000)    14666 2023-12-25 13:21:32.000000 feloopy-0.2.8/feloopy/generators/model/mealpy_model_generator.py
--rwxr-xr-x   0 keivant   (1000) keivant   (1000)      622 2023-12-25 13:21:32.000000 feloopy-0.2.8/feloopy/generators/model/mip_model_generator.py
--rwxr-xr-x   0 keivant   (1000) keivant   (1000)     8394 2023-12-25 13:21:32.000000 feloopy-0.2.8/feloopy/generators/model/niapy_model_generator.py
--rwxr-xr-x   0 keivant   (1000) keivant   (1000)      620 2023-12-25 13:21:32.000000 feloopy-0.2.8/feloopy/generators/model/ortools_cp_model_generator.py
--rwxr-xr-x   0 keivant   (1000) keivant   (1000)      642 2023-12-25 13:21:32.000000 feloopy-0.2.8/feloopy/generators/model/ortools_model_generator.py
--rwxr-xr-x   0 keivant   (1000) keivant   (1000)      617 2023-12-25 13:21:32.000000 feloopy-0.2.8/feloopy/generators/model/picos_model_generator.py
--rwxr-xr-x   0 keivant   (1000) keivant   (1000)      638 2023-12-25 13:21:32.000000 feloopy-0.2.8/feloopy/generators/model/pulp_model_generator.py
--rwxr-xr-x   0 keivant   (1000) keivant   (1000)      609 2023-12-25 13:21:32.000000 feloopy-0.2.8/feloopy/generators/model/pymprog_model_generator.py
--rwxr-xr-x   0 keivant   (1000) keivant   (1000)      631 2023-12-25 13:21:32.000000 feloopy-0.2.8/feloopy/generators/model/pyomo_model_generator.py
--rwxr-xr-x   0 keivant   (1000) keivant   (1000)      639 2023-12-25 13:21:32.000000 feloopy-0.2.8/feloopy/generators/model/rsome_dro_model_generator.py
--rwxr-xr-x   0 keivant   (1000) keivant   (1000)      611 2023-12-25 13:21:32.000000 feloopy-0.2.8/feloopy/generators/model/rsome_ro_model_generator.py
--rwxr-xr-x   0 keivant   (1000) keivant   (1000)      613 2023-12-25 13:21:32.000000 feloopy-0.2.8/feloopy/generators/model/xpress_model_generator.py
--rwxr-xr-x   0 keivant   (1000) keivant   (1000)     2986 2023-12-25 13:21:32.000000 feloopy-0.2.8/feloopy/generators/model_generator.py
-drwxr-xr-x   0 keivant   (1000) keivant   (1000)        0 2023-12-25 13:28:43.587708 feloopy-0.2.8/feloopy/generators/result/
--rwxr-xr-x   0 keivant   (1000) keivant   (1000)      117 2023-12-25 13:21:32.000000 feloopy-0.2.8/feloopy/generators/result/__init__.py
--rwxr-xr-x   0 keivant   (1000) keivant   (1000)     1691 2023-12-25 13:21:32.000000 feloopy-0.2.8/feloopy/generators/result/copt_result_generator.py
--rwxr-xr-x   0 keivant   (1000) keivant   (1000)      504 2023-12-25 13:21:32.000000 feloopy-0.2.8/feloopy/generators/result/cplex_cp_result_generator.py
--rwxr-xr-x   0 keivant   (1000) keivant   (1000)     1137 2023-12-25 13:21:32.000000 feloopy-0.2.8/feloopy/generators/result/cplex_result_generator.py
--rwxr-xr-x   0 keivant   (1000) keivant   (1000)     1167 2023-12-25 13:21:32.000000 feloopy-0.2.8/feloopy/generators/result/cvxpy_result_generator.py
--rwxr-xr-x   0 keivant   (1000) keivant   (1000)      576 2023-12-25 13:21:32.000000 feloopy-0.2.8/feloopy/generators/result/cylp_result_generator.py
--rwxr-xr-x   0 keivant   (1000) keivant   (1000)      752 2023-12-25 13:21:32.000000 feloopy-0.2.8/feloopy/generators/result/gekko_result_generator.py
--rwxr-xr-x   0 keivant   (1000) keivant   (1000)     2263 2023-12-25 13:21:32.000000 feloopy-0.2.8/feloopy/generators/result/gurobi_result_generator.py
--rwxr-xr-x   0 keivant   (1000) keivant   (1000)      561 2023-12-25 13:21:32.000000 feloopy-0.2.8/feloopy/generators/result/linopy_result_generator.py
--rw-r--r--   0 keivant   (1000) keivant   (1000)     1138 2023-12-25 13:21:32.000000 feloopy-0.2.8/feloopy/generators/result/localsolver_result_generator.py
--rwxr-xr-x   0 keivant   (1000) keivant   (1000)      498 2023-12-25 13:21:32.000000 feloopy-0.2.8/feloopy/generators/result/mip_result_generator.py
--rwxr-xr-x   0 keivant   (1000) keivant   (1000)      784 2023-12-25 13:21:32.000000 feloopy-0.2.8/feloopy/generators/result/ortools_cp_result_generator.py
--rwxr-xr-x   0 keivant   (1000) keivant   (1000)      933 2023-12-25 13:21:32.000000 feloopy-0.2.8/feloopy/generators/result/ortools_result_generator.py
--rwxr-xr-x   0 keivant   (1000) keivant   (1000)      948 2023-12-25 13:21:32.000000 feloopy-0.2.8/feloopy/generators/result/picos_result_generator.py
--rwxr-xr-x   0 keivant   (1000) keivant   (1000)     1787 2023-12-25 13:21:32.000000 feloopy-0.2.8/feloopy/generators/result/pulp_result_generator.py
--rwxr-xr-x   0 keivant   (1000) keivant   (1000)      602 2023-12-25 13:21:32.000000 feloopy-0.2.8/feloopy/generators/result/pymprog_result_generator.py
--rwxr-xr-x   0 keivant   (1000) keivant   (1000)      900 2023-12-25 13:21:32.000000 feloopy-0.2.8/feloopy/generators/result/pyomo_result_generator.py
--rwxr-xr-x   0 keivant   (1000) keivant   (1000)      678 2023-12-25 13:21:32.000000 feloopy-0.2.8/feloopy/generators/result/rsome_dro_result_generator.py
--rwxr-xr-x   0 keivant   (1000) keivant   (1000)      666 2023-12-25 13:21:32.000000 feloopy-0.2.8/feloopy/generators/result/rsome_ro_result_generator.py
--rwxr-xr-x   0 keivant   (1000) keivant   (1000)      556 2023-12-25 13:21:32.000000 feloopy-0.2.8/feloopy/generators/result/xpress_result_generator.py
--rwxr-xr-x   0 keivant   (1000) keivant   (1000)     7673 2023-12-25 13:21:32.000000 feloopy-0.2.8/feloopy/generators/result_generator.py
-drwxr-xr-x   0 keivant   (1000) keivant   (1000)        0 2023-12-25 13:28:43.591042 feloopy-0.2.8/feloopy/generators/solution/
--rwxr-xr-x   0 keivant   (1000) keivant   (1000)      117 2023-12-25 13:21:32.000000 feloopy-0.2.8/feloopy/generators/solution/__init__.py
--rwxr-xr-x   0 keivant   (1000) keivant   (1000)     2903 2023-12-25 13:21:32.000000 feloopy-0.2.8/feloopy/generators/solution/copt_solution_generator.py
--rwxr-xr-x   0 keivant   (1000) keivant   (1000)     2103 2023-12-25 13:21:32.000000 feloopy-0.2.8/feloopy/generators/solution/cplex_cp_solution_generator.py
--rwxr-xr-x   0 keivant   (1000) keivant   (1000)     4156 2023-12-25 13:21:32.000000 feloopy-0.2.8/feloopy/generators/solution/cplex_solution_generator.py
--rwxr-xr-x   0 keivant   (1000) keivant   (1000)     3427 2023-12-25 13:21:32.000000 feloopy-0.2.8/feloopy/generators/solution/cvxpy_solution_generator.py
--rwxr-xr-x   0 keivant   (1000) keivant   (1000)     2106 2023-12-25 13:21:32.000000 feloopy-0.2.8/feloopy/generators/solution/cylp_solution_generator.py
--rwxr-xr-x   0 keivant   (1000) keivant   (1000)     3017 2023-12-25 13:21:32.000000 feloopy-0.2.8/feloopy/generators/solution/feloopy_solution_generator.py
--rwxr-xr-x   0 keivant   (1000) keivant   (1000)     2759 2023-12-25 13:21:32.000000 feloopy-0.2.8/feloopy/generators/solution/gekko_solution_generator.py
--rwxr-xr-x   0 keivant   (1000) keivant   (1000)     3011 2023-12-25 13:21:32.000000 feloopy-0.2.8/feloopy/generators/solution/gurobi_solution_generator.py
--rwxr-xr-x   0 keivant   (1000) keivant   (1000)     2378 2023-12-25 13:21:32.000000 feloopy-0.2.8/feloopy/generators/solution/linopy_solution_generator.py
--rw-r--r--   0 keivant   (1000) keivant   (1000)     1504 2023-12-25 13:21:32.000000 feloopy-0.2.8/feloopy/generators/solution/localsolver_solution_generator.py
--rwxr-xr-x   0 keivant   (1000) keivant   (1000)     5330 2023-12-25 13:21:32.000000 feloopy-0.2.8/feloopy/generators/solution/mealpy_solution_generator.py
--rwxr-xr-x   0 keivant   (1000) keivant   (1000)     2136 2023-12-25 13:21:32.000000 feloopy-0.2.8/feloopy/generators/solution/mip_solution_generator.py
--rwxr-xr-x   0 keivant   (1000) keivant   (1000)     3615 2023-12-25 13:21:32.000000 feloopy-0.2.8/feloopy/generators/solution/niapy_solution_generator.py
--rwxr-xr-x   0 keivant   (1000) keivant   (1000)     2801 2023-12-25 13:21:32.000000 feloopy-0.2.8/feloopy/generators/solution/ortools_cp_solution_generator.py
--rwxr-xr-x   0 keivant   (1000) keivant   (1000)     3403 2023-12-25 13:21:32.000000 feloopy-0.2.8/feloopy/generators/solution/ortools_solution_generator.py
--rwxr-xr-x   0 keivant   (1000) keivant   (1000)     2709 2023-12-25 13:21:32.000000 feloopy-0.2.8/feloopy/generators/solution/picos_solution_generator.py
--rwxr-xr-x   0 keivant   (1000) keivant   (1000)     3522 2023-12-25 13:21:32.000000 feloopy-0.2.8/feloopy/generators/solution/pulp_solution_generator.py
--rwxr-xr-x   0 keivant   (1000) keivant   (1000)     3590 2023-12-25 13:21:32.000000 feloopy-0.2.8/feloopy/generators/solution/pygad_solution_generator.py
--rwxr-xr-x   0 keivant   (1000) keivant   (1000)     4608 2023-12-25 13:21:32.000000 feloopy-0.2.8/feloopy/generators/solution/pymoo_solution_generator.py
--rwxr-xr-x   0 keivant   (1000) keivant   (1000)     2204 2023-12-25 13:21:32.000000 feloopy-0.2.8/feloopy/generators/solution/pymprog_solution_generator.py
--rwxr-xr-x   0 keivant   (1000) keivant   (1000)     5151 2023-12-25 13:21:32.000000 feloopy-0.2.8/feloopy/generators/solution/pymultiobjective_solution_generator.py
--rwxr-xr-x   0 keivant   (1000) keivant   (1000)     6085 2023-12-25 13:21:32.000000 feloopy-0.2.8/feloopy/generators/solution/pyomo_solution_generator.py
--rwxr-xr-x   0 keivant   (1000) keivant   (1000)     3244 2023-12-25 13:21:32.000000 feloopy-0.2.8/feloopy/generators/solution/rsome_dro_solution_generator.py
--rwxr-xr-x   0 keivant   (1000) keivant   (1000)     3272 2023-12-25 13:21:32.000000 feloopy-0.2.8/feloopy/generators/solution/rsome_ro_solution_generator.py
--rwxr-xr-x   0 keivant   (1000) keivant   (1000)     2142 2023-12-25 13:21:32.000000 feloopy-0.2.8/feloopy/generators/solution/xpress_solution_generator.py
--rwxr-xr-x   0 keivant   (1000) keivant   (1000)     3453 2023-12-25 13:21:32.000000 feloopy-0.2.8/feloopy/generators/solution_generator.py
-drwxr-xr-x   0 keivant   (1000) keivant   (1000)        0 2023-12-25 13:28:43.597708 feloopy-0.2.8/feloopy/generators/variable/
--rwxr-xr-x   0 keivant   (1000) keivant   (1000)      117 2023-12-25 13:21:32.000000 feloopy-0.2.8/feloopy/generators/variable/__init__.py
--rwxr-xr-x   0 keivant   (1000) keivant   (1000)     7400 2023-12-25 13:21:32.000000 feloopy-0.2.8/feloopy/generators/variable/copt_variable_generator.py
--rwxr-xr-x   0 keivant   (1000) keivant   (1000)     2948 2023-12-25 13:21:32.000000 feloopy-0.2.8/feloopy/generators/variable/cplex_cp_variable_generator.py
--rwxr-xr-x   0 keivant   (1000) keivant   (1000)     3259 2023-12-25 13:21:32.000000 feloopy-0.2.8/feloopy/generators/variable/cplex_variable_generator.py
--rwxr-xr-x   0 keivant   (1000) keivant   (1000)     4070 2023-12-25 13:21:32.000000 feloopy-0.2.8/feloopy/generators/variable/cvxpy_variable_generator.py
--rwxr-xr-x   0 keivant   (1000) keivant   (1000)     3519 2023-12-25 13:21:32.000000 feloopy-0.2.8/feloopy/generators/variable/cylp_variable_generator.py
--rwxr-xr-x   0 keivant   (1000) keivant   (1000)     4013 2023-12-25 13:21:32.000000 feloopy-0.2.8/feloopy/generators/variable/gekko_variable_generator.py
--rwxr-xr-x   0 keivant   (1000) keivant   (1000)     7425 2023-12-25 13:21:32.000000 feloopy-0.2.8/feloopy/generators/variable/gurobi_variable_generator.py
--rwxr-xr-x   0 keivant   (1000) keivant   (1000)     3571 2023-12-25 13:21:32.000000 feloopy-0.2.8/feloopy/generators/variable/linopy_variable_generator.py
--rw-r--r--   0 keivant   (1000) keivant   (1000)     2844 2023-12-25 13:21:32.000000 feloopy-0.2.8/feloopy/generators/variable/localsolver_variable_generator.py
--rwxr-xr-x   0 keivant   (1000) keivant   (1000)     2780 2023-12-25 13:21:32.000000 feloopy-0.2.8/feloopy/generators/variable/mip_variable_generator.py
--rwxr-xr-x   0 keivant   (1000) keivant   (1000)     3567 2023-12-25 13:21:32.000000 feloopy-0.2.8/feloopy/generators/variable/ortools_cp_variable_generator.py
--rwxr-xr-x   0 keivant   (1000) keivant   (1000)     3783 2023-12-25 13:21:32.000000 feloopy-0.2.8/feloopy/generators/variable/ortools_variable_generator.py
--rwxr-xr-x   0 keivant   (1000) keivant   (1000)     3001 2023-12-25 13:21:32.000000 feloopy-0.2.8/feloopy/generators/variable/picos_variable_generator.py
--rwxr-xr-x   0 keivant   (1000) keivant   (1000)     3487 2023-12-25 13:21:32.000000 feloopy-0.2.8/feloopy/generators/variable/pulp_variable_generator.py
--rwxr-xr-x   0 keivant   (1000) keivant   (1000)     3333 2023-12-25 13:21:32.000000 feloopy-0.2.8/feloopy/generators/variable/pymprog_variable_generator.py
--rwxr-xr-x   0 keivant   (1000) keivant   (1000)     2529 2023-12-25 13:21:32.000000 feloopy-0.2.8/feloopy/generators/variable/pyomo_variable_generator.py
--rwxr-xr-x   0 keivant   (1000) keivant   (1000)     5000 2023-12-25 13:21:32.000000 feloopy-0.2.8/feloopy/generators/variable/rsome_dro_variable_generator.py
--rwxr-xr-x   0 keivant   (1000) keivant   (1000)     5023 2023-12-25 13:21:32.000000 feloopy-0.2.8/feloopy/generators/variable/rsome_ro_variable_generator.py
--rwxr-xr-x   0 keivant   (1000) keivant   (1000)     4057 2023-12-25 13:21:32.000000 feloopy-0.2.8/feloopy/generators/variable/xpress_variable_generator.py
--rwxr-xr-x   0 keivant   (1000) keivant   (1000)     3353 2023-12-25 13:21:32.000000 feloopy-0.2.8/feloopy/generators/variable_generator.py
-drwxr-xr-x   0 keivant   (1000) keivant   (1000)        0 2023-12-25 13:28:43.597708 feloopy-0.2.8/feloopy/helpers/
--rwxr-xr-x   0 keivant   (1000) keivant   (1000)      117 2023-12-25 13:21:32.000000 feloopy-0.2.8/feloopy/helpers/__init__.py
--rwxr-xr-x   0 keivant   (1000) keivant   (1000)     1317 2023-12-25 13:21:32.000000 feloopy-0.2.8/feloopy/helpers/empty.py
--rwxr-xr-x   0 keivant   (1000) keivant   (1000)      215 2023-12-25 13:21:32.000000 feloopy-0.2.8/feloopy/helpers/error.py
--rwxr-xr-x   0 keivant   (1000) keivant   (1000)     9132 2023-12-25 13:21:32.000000 feloopy-0.2.8/feloopy/helpers/formatter.py
-drwxr-xr-x   0 keivant   (1000) keivant   (1000)        0 2023-12-25 13:28:43.604375 feloopy-0.2.8/feloopy/operators/
--rwxr-xr-x   0 keivant   (1000) keivant   (1000)      209 2023-12-25 13:21:32.000000 feloopy-0.2.8/feloopy/operators/__init__.py
--rwxr-xr-x   0 keivant   (1000) keivant   (1000)    19504 2023-12-25 13:21:32.000000 feloopy-0.2.8/feloopy/operators/common.py
--rwxr-xr-x   0 keivant   (1000) keivant   (1000)    15381 2023-12-25 13:21:32.000000 feloopy-0.2.8/feloopy/operators/data_handler.py
--rwxr-xr-x   0 keivant   (1000) keivant   (1000)      117 2023-12-25 13:21:32.000000 feloopy-0.2.8/feloopy/operators/epsilon.py
--rwxr-xr-x   0 keivant   (1000) keivant   (1000)      206 2023-12-25 13:21:32.000000 feloopy-0.2.8/feloopy/operators/exact.py
--rwxr-xr-x   0 keivant   (1000) keivant   (1000)      388 2023-12-25 13:21:32.000000 feloopy-0.2.8/feloopy/operators/fix_operators.py
--rwxr-xr-x   0 keivant   (1000) keivant   (1000)      297 2023-12-25 13:21:32.000000 feloopy-0.2.8/feloopy/operators/heuristic.py
--rwxr-xr-x   0 keivant   (1000) keivant   (1000)     5207 2023-12-25 13:21:32.000000 feloopy-0.2.8/feloopy/operators/heuristic_operators.py
--rwxr-xr-x   0 keivant   (1000) keivant   (1000)     2153 2023-12-25 13:21:32.000000 feloopy-0.2.8/feloopy/operators/math_operators.py
--rw-r--r--   0 keivant   (1000) keivant   (1000)      117 2023-12-25 13:21:32.000000 feloopy-0.2.8/feloopy/operators/pareto.py
--rwxr-xr-x   0 keivant   (1000) keivant   (1000)      296 2023-12-25 13:21:32.000000 feloopy-0.2.8/feloopy/operators/random_operators.py
--rwxr-xr-x   0 keivant   (1000) keivant   (1000)      400 2023-12-25 13:21:32.000000 feloopy-0.2.8/feloopy/operators/set_operators.py
--rwxr-xr-x   0 keivant   (1000) keivant   (1000)     2091 2023-12-25 13:21:32.000000 feloopy-0.2.8/feloopy/operators/update_operators.py
-drwxr-xr-x   0 keivant   (1000) keivant   (1000)        0 2023-12-25 13:28:43.571041 feloopy-0.2.8/feloopy.egg-info/
--rw-r--r--   0 keivant   (1000) keivant   (1000)    77973 2023-12-25 13:28:43.000000 feloopy-0.2.8/feloopy.egg-info/PKG-INFO
--rw-r--r--   0 keivant   (1000) keivant   (1000)     6661 2023-12-25 13:28:43.000000 feloopy-0.2.8/feloopy.egg-info/SOURCES.txt
--rw-r--r--   0 keivant   (1000) keivant   (1000)        1 2023-12-25 13:28:43.000000 feloopy-0.2.8/feloopy.egg-info/dependency_links.txt
--rw-r--r--   0 keivant   (1000) keivant   (1000)       91 2023-12-25 13:28:43.000000 feloopy-0.2.8/feloopy.egg-info/entry_points.txt
--rw-r--r--   0 keivant   (1000) keivant   (1000)     1600 2023-12-25 13:28:43.000000 feloopy-0.2.8/feloopy.egg-info/requires.txt
--rw-r--r--   0 keivant   (1000) keivant   (1000)        8 2023-12-25 13:28:43.000000 feloopy-0.2.8/feloopy.egg-info/top_level.txt
--rw-r--r--   0 keivant   (1000) keivant   (1000)     2840 2023-12-25 13:21:32.000000 feloopy-0.2.8/pyproject.toml
--rw-r--r--   0 keivant   (1000) keivant   (1000)       38 2023-12-25 13:28:43.604375 feloopy-0.2.8/setup.cfg
--rwxr-xr-x   0 keivant   (1000) keivant   (1000)     3537 2023-12-25 13:21:32.000000 feloopy-0.2.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-07 21:21:03.409414 feloopy-0.2.9/
+-rw-rw-rw-   0        0        0     1100 2024-04-07 21:17:47.000000 feloopy-0.2.9/LICENSE
+-rw-rw-rw-   0        0        0    10479 2024-04-07 21:21:03.409414 feloopy-0.2.9/PKG-INFO
+-rw-rw-rw-   0        0        0     4357 2024-04-07 21:17:47.000000 feloopy-0.2.9/README.md
+drwxrwxrwx   0        0        0        0 2024-04-07 21:21:01.122842 feloopy-0.2.9/feloopy/
+-rw-rw-rw-   0        0        0      177 2024-04-07 21:17:47.000000 feloopy-0.2.9/feloopy/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-07 21:21:01.173317 feloopy-0.2.9/feloopy/algorithms/
+-rw-rw-rw-   0        0        0      117 2024-04-07 21:17:47.000000 feloopy-0.2.9/feloopy/algorithms/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-07 21:21:01.177317 feloopy-0.2.9/feloopy/algorithms/constraint/
+-rw-rw-rw-   0        0        0      117 2024-04-07 21:17:47.000000 feloopy-0.2.9/feloopy/algorithms/constraint/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-07 21:21:01.194350 feloopy-0.2.9/feloopy/algorithms/exact/
+-rw-rw-rw-   0        0        0      117 2024-04-07 21:17:47.000000 feloopy-0.2.9/feloopy/algorithms/exact/__init__.py
+-rw-rw-rw-   0        0        0      117 2024-04-07 21:17:47.000000 feloopy-0.2.9/feloopy/algorithms/exact/benders.py
+-rw-rw-rw-   0        0        0    12140 2024-04-07 21:17:47.000000 feloopy-0.2.9/feloopy/algorithms/exact/multiobjective.py
+drwxrwxrwx   0        0        0        0 2024-04-07 21:21:01.260939 feloopy-0.2.9/feloopy/algorithms/heuristic/
+-rw-rw-rw-   0        0        0     2941 2024-04-07 21:17:47.000000 feloopy-0.2.9/feloopy/algorithms/heuristic/DE.py
+-rw-rw-rw-   0        0        0     3867 2024-04-07 21:17:47.000000 feloopy-0.2.9/feloopy/algorithms/heuristic/GA.py
+-rw-rw-rw-   0        0        0     2549 2024-04-07 21:17:47.000000 feloopy-0.2.9/feloopy/algorithms/heuristic/GWO.py
+-rw-rw-rw-   0        0        0     3891 2024-04-07 21:17:47.000000 feloopy-0.2.9/feloopy/algorithms/heuristic/SA.py
+-rw-rw-rw-   0        0        0     1995 2024-04-07 21:17:47.000000 feloopy-0.2.9/feloopy/algorithms/heuristic/TS.py
+-rw-rw-rw-   0        0        0      117 2024-04-07 21:17:47.000000 feloopy-0.2.9/feloopy/algorithms/heuristic/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-07 21:21:01.409848 feloopy-0.2.9/feloopy/classes/
+-rw-rw-rw-   0        0        0      472 2024-04-07 21:17:47.000000 feloopy-0.2.9/feloopy/classes/__init__.py
+-rw-rw-rw-   0        0        0    24858 2024-04-07 21:17:47.000000 feloopy-0.2.9/feloopy/classes/constraint_programming.py
+-rw-rw-rw-   0        0        0     4041 2024-04-07 21:17:47.000000 feloopy-0.2.9/feloopy/classes/event_variable.py
+-rw-rw-rw-   0        0        0     1339 2024-04-07 21:17:47.000000 feloopy-0.2.9/feloopy/classes/event_variable_collection.py
+-rw-rw-rw-   0        0        0    14094 2024-04-07 21:17:47.000000 feloopy-0.2.9/feloopy/classes/linearization.py
+-rw-rw-rw-   0        0        0    12477 2024-04-07 21:17:47.000000 feloopy-0.2.9/feloopy/classes/multidim_variable.py
+-rw-rw-rw-   0        0        0     3642 2024-04-07 21:17:47.000000 feloopy-0.2.9/feloopy/classes/multidim_variable_collection.py
+-rw-rw-rw-   0        0        0     7957 2024-04-07 21:17:47.000000 feloopy-0.2.9/feloopy/classes/normal_constraint.py
+-rw-rw-rw-   0        0        0    15872 2024-04-07 21:17:47.000000 feloopy-0.2.9/feloopy/classes/special_constraint.py
+-rw-rw-rw-   0        0        0     8175 2024-04-07 21:17:47.000000 feloopy-0.2.9/feloopy/classes/tensor_variable.py
+-rw-rw-rw-   0        0        0     3812 2024-04-07 21:17:47.000000 feloopy-0.2.9/feloopy/classes/tensor_variable_collection.py
+-rw-rw-rw-   0        0        0     3103 2024-04-07 21:17:47.000000 feloopy-0.2.9/feloopy/cli.py
+drwxrwxrwx   0        0        0        0 2024-04-07 21:21:01.433866 feloopy-0.2.9/feloopy/clitools/
+-rw-rw-rw-   0        0        0      175 2024-04-07 21:17:47.000000 feloopy-0.2.9/feloopy/clitools/__init__.py
+-rw-rw-rw-   0        0        0     1338 2024-04-07 21:17:47.000000 feloopy-0.2.9/feloopy/clitools/pkg_manager_detector.py
+-rw-rw-rw-   0        0        0    14168 2024-04-07 21:17:47.000000 feloopy-0.2.9/feloopy/clitools/utils.py
+-rw-rw-rw-   0        0        0   225113 2024-04-07 21:17:47.000000 feloopy-0.2.9/feloopy/feloopy.py
+drwxrwxrwx   0        0        0        0 2024-04-07 21:21:01.495483 feloopy-0.2.9/feloopy/generators/
+-rw-rw-rw-   0        0        0      274 2024-04-07 21:17:47.000000 feloopy-0.2.9/feloopy/generators/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-07 21:21:01.558385 feloopy-0.2.9/feloopy/generators/init/
+-rw-rw-rw-   0        0        0      117 2024-04-07 21:17:47.000000 feloopy-0.2.9/feloopy/generators/init/__init__.py
+-rw-rw-rw-   0        0        0      266 2024-04-07 21:17:47.000000 feloopy-0.2.9/feloopy/generators/init/copt_init_generator.py
+-rw-rw-rw-   0        0        0      283 2024-04-07 21:17:47.000000 feloopy-0.2.9/feloopy/generators/init/cplex_init_generator.py
+-rw-rw-rw-   0        0        0      328 2024-04-07 21:17:47.000000 feloopy-0.2.9/feloopy/generators/init/gekko_init_generator.py
+-rw-rw-rw-   0        0        0      310 2024-04-07 21:17:47.000000 feloopy-0.2.9/feloopy/generators/init/gurobi_init_generator.py
+-rw-rw-rw-   0        0        0      317 2024-04-07 21:17:47.000000 feloopy-0.2.9/feloopy/generators/init/pulp_init_generator.py
+-rw-rw-rw-   0        0        0      254 2024-04-07 21:17:47.000000 feloopy-0.2.9/feloopy/generators/init/pyomo_init_generator.py
+-rw-rw-rw-   0        0        0     1262 2024-04-07 21:17:47.000000 feloopy-0.2.9/feloopy/generators/init_generator.py
+drwxrwxrwx   0        0        0        0 2024-04-07 21:21:01.778005 feloopy-0.2.9/feloopy/generators/model/
+-rw-rw-rw-   0        0        0      117 2024-04-07 21:17:47.000000 feloopy-0.2.9/feloopy/generators/model/__init__.py
+-rw-rw-rw-   0        0        0      310 2024-04-07 21:17:47.000000 feloopy-0.2.9/feloopy/generators/model/copt_model_generator.py
+-rw-rw-rw-   0        0        0      253 2024-04-07 21:17:47.000000 feloopy-0.2.9/feloopy/generators/model/cplex_cp_model_generator.py
+-rw-rw-rw-   0        0        0      249 2024-04-07 21:17:47.000000 feloopy-0.2.9/feloopy/generators/model/cplex_model_generator.py
+-rw-rw-rw-   0        0        0      211 2024-04-07 21:17:47.000000 feloopy-0.2.9/feloopy/generators/model/cvxpy_model_generator.py
+-rw-rw-rw-   0        0        0      263 2024-04-07 21:17:47.000000 feloopy-0.2.9/feloopy/generators/model/cylp_model_generator.py
+-rw-rw-rw-   0        0        0     4492 2024-04-07 21:17:47.000000 feloopy-0.2.9/feloopy/generators/model/feloopy_model_generator.py
+-rw-rw-rw-   0        0        0      218 2024-04-07 21:17:47.000000 feloopy-0.2.9/feloopy/generators/model/gamspy_model_generator.py
+-rw-rw-rw-   0        0        0      258 2024-04-07 21:17:47.000000 feloopy-0.2.9/feloopy/generators/model/gekko_model_generator.py
+-rw-rw-rw-   0        0        0      244 2024-04-07 21:17:47.000000 feloopy-0.2.9/feloopy/generators/model/gurobi_model_generator.py
+-rw-rw-rw-   0        0        0      218 2024-04-07 21:17:47.000000 feloopy-0.2.9/feloopy/generators/model/highs_model_generator.py
+-rw-rw-rw-   0        0        0      215 2024-04-07 21:17:47.000000 feloopy-0.2.9/feloopy/generators/model/linopy_model_generator.py
+-rw-rw-rw-   0        0        0    14295 2024-04-07 21:17:47.000000 feloopy-0.2.9/feloopy/generators/model/mealpy_model_generator.py
+-rw-rw-rw-   0        0        0      251 2024-04-07 21:17:47.000000 feloopy-0.2.9/feloopy/generators/model/mip_model_generator.py
+-rw-rw-rw-   0        0        0     8023 2024-04-07 21:17:47.000000 feloopy-0.2.9/feloopy/generators/model/niapy_model_generator.py
+-rw-rw-rw-   0        0        0      249 2024-04-07 21:17:47.000000 feloopy-0.2.9/feloopy/generators/model/ortools_cp_model_generator.py
+-rw-rw-rw-   0        0        0      271 2024-04-07 21:17:47.000000 feloopy-0.2.9/feloopy/generators/model/ortools_model_generator.py
+-rw-rw-rw-   0        0        0      246 2024-04-07 21:17:47.000000 feloopy-0.2.9/feloopy/generators/model/picos_model_generator.py
+-rw-rw-rw-   0        0        0      267 2024-04-07 21:17:47.000000 feloopy-0.2.9/feloopy/generators/model/pulp_model_generator.py
+-rw-rw-rw-   0        0        0      238 2024-04-07 21:17:47.000000 feloopy-0.2.9/feloopy/generators/model/pymprog_model_generator.py
+-rw-rw-rw-   0        0        0      260 2024-04-07 21:17:47.000000 feloopy-0.2.9/feloopy/generators/model/pyomo_model_generator.py
+-rw-rw-rw-   0        0        0      268 2024-04-07 21:17:47.000000 feloopy-0.2.9/feloopy/generators/model/rsome_dro_model_generator.py
+-rw-rw-rw-   0        0        0      240 2024-04-07 21:17:47.000000 feloopy-0.2.9/feloopy/generators/model/rsome_ro_model_generator.py
+-rw-rw-rw-   0        0        0      306 2024-04-07 21:17:47.000000 feloopy-0.2.9/feloopy/generators/model/seeker_model_generator.py
+-rw-rw-rw-   0        0        0      242 2024-04-07 21:17:47.000000 feloopy-0.2.9/feloopy/generators/model/xpress_model_generator.py
+-rw-rw-rw-   0        0        0     3612 2024-04-07 21:17:47.000000 feloopy-0.2.9/feloopy/generators/model_generator.py
+drwxrwxrwx   0        0        0        0 2024-04-07 21:21:02.044393 feloopy-0.2.9/feloopy/generators/result/
+-rw-rw-rw-   0        0        0      117 2024-04-07 21:17:47.000000 feloopy-0.2.9/feloopy/generators/result/__init__.py
+-rw-rw-rw-   0        0        0     1691 2024-04-07 21:17:47.000000 feloopy-0.2.9/feloopy/generators/result/copt_result_generator.py
+-rw-rw-rw-   0        0        0      504 2024-04-07 21:17:47.000000 feloopy-0.2.9/feloopy/generators/result/cplex_cp_result_generator.py
+-rw-rw-rw-   0        0        0     1137 2024-04-07 21:17:47.000000 feloopy-0.2.9/feloopy/generators/result/cplex_result_generator.py
+-rw-rw-rw-   0        0        0     1167 2024-04-07 21:17:47.000000 feloopy-0.2.9/feloopy/generators/result/cvxpy_result_generator.py
+-rw-rw-rw-   0        0        0      576 2024-04-07 21:17:47.000000 feloopy-0.2.9/feloopy/generators/result/cylp_result_generator.py
+-rw-rw-rw-   0        0        0     1053 2024-04-07 21:17:47.000000 feloopy-0.2.9/feloopy/generators/result/gamspy_result_generator.py
+-rw-rw-rw-   0        0        0      752 2024-04-07 21:17:47.000000 feloopy-0.2.9/feloopy/generators/result/gekko_result_generator.py
+-rw-rw-rw-   0        0        0     2271 2024-04-07 21:17:47.000000 feloopy-0.2.9/feloopy/generators/result/gurobi_result_generator.py
+-rw-rw-rw-   0        0        0      799 2024-04-07 21:17:47.000000 feloopy-0.2.9/feloopy/generators/result/highs_result_generator.py
+-rw-rw-rw-   0        0        0      561 2024-04-07 21:17:47.000000 feloopy-0.2.9/feloopy/generators/result/linopy_result_generator.py
+-rw-rw-rw-   0        0        0      498 2024-04-07 21:17:47.000000 feloopy-0.2.9/feloopy/generators/result/mip_result_generator.py
+-rw-rw-rw-   0        0        0      784 2024-04-07 21:17:47.000000 feloopy-0.2.9/feloopy/generators/result/ortools_cp_result_generator.py
+-rw-rw-rw-   0        0        0      933 2024-04-07 21:17:47.000000 feloopy-0.2.9/feloopy/generators/result/ortools_result_generator.py
+-rw-rw-rw-   0        0        0      948 2024-04-07 21:17:47.000000 feloopy-0.2.9/feloopy/generators/result/picos_result_generator.py
+-rw-rw-rw-   0        0        0     1787 2024-04-07 21:17:47.000000 feloopy-0.2.9/feloopy/generators/result/pulp_result_generator.py
+-rw-rw-rw-   0        0        0      602 2024-04-07 21:17:47.000000 feloopy-0.2.9/feloopy/generators/result/pymprog_result_generator.py
+-rw-rw-rw-   0        0        0      900 2024-04-07 21:17:47.000000 feloopy-0.2.9/feloopy/generators/result/pyomo_result_generator.py
+-rw-rw-rw-   0        0        0      678 2024-04-07 21:17:47.000000 feloopy-0.2.9/feloopy/generators/result/rsome_dro_result_generator.py
+-rw-rw-rw-   0        0        0      666 2024-04-07 21:17:47.000000 feloopy-0.2.9/feloopy/generators/result/rsome_ro_result_generator.py
+-rw-rw-rw-   0        0        0      532 2024-04-07 21:17:47.000000 feloopy-0.2.9/feloopy/generators/result/seeker_result_generator.py
+-rw-rw-rw-   0        0        0      556 2024-04-07 21:17:47.000000 feloopy-0.2.9/feloopy/generators/result/xpress_result_generator.py
+-rw-rw-rw-   0        0        0     9259 2024-04-07 21:17:47.000000 feloopy-0.2.9/feloopy/generators/result_generator.py
+drwxrwxrwx   0        0        0        0 2024-04-07 21:21:02.860372 feloopy-0.2.9/feloopy/generators/solution/
+-rw-rw-rw-   0        0        0      117 2024-04-07 21:17:47.000000 feloopy-0.2.9/feloopy/generators/solution/__init__.py
+-rw-rw-rw-   0        0        0     2903 2024-04-07 21:17:47.000000 feloopy-0.2.9/feloopy/generators/solution/copt_solution_generator.py
+-rw-rw-rw-   0        0        0     2103 2024-04-07 21:17:47.000000 feloopy-0.2.9/feloopy/generators/solution/cplex_cp_solution_generator.py
+-rw-rw-rw-   0        0        0     4298 2024-04-07 21:17:47.000000 feloopy-0.2.9/feloopy/generators/solution/cplex_solution_generator.py
+-rw-rw-rw-   0        0        0     3427 2024-04-07 21:17:47.000000 feloopy-0.2.9/feloopy/generators/solution/cvxpy_solution_generator.py
+-rw-rw-rw-   0        0        0     2106 2024-04-07 21:17:47.000000 feloopy-0.2.9/feloopy/generators/solution/cylp_solution_generator.py
+-rw-rw-rw-   0        0        0     3154 2024-04-07 21:17:47.000000 feloopy-0.2.9/feloopy/generators/solution/feloopy_solution_generator.py
+-rw-rw-rw-   0        0        0     3874 2024-04-07 21:17:47.000000 feloopy-0.2.9/feloopy/generators/solution/gamspy_solution_generator.py
+-rw-rw-rw-   0        0        0     2759 2024-04-07 21:17:47.000000 feloopy-0.2.9/feloopy/generators/solution/gekko_solution_generator.py
+-rw-rw-rw-   0        0        0     3024 2024-04-07 21:17:47.000000 feloopy-0.2.9/feloopy/generators/solution/gurobi_solution_generator.py
+-rw-rw-rw-   0        0        0     2257 2024-04-07 21:17:47.000000 feloopy-0.2.9/feloopy/generators/solution/highs_solution_generator.py
+-rw-rw-rw-   0        0        0     2243 2024-04-07 21:17:47.000000 feloopy-0.2.9/feloopy/generators/solution/linopy_solution_generator.py
+-rw-rw-rw-   0        0        0     5454 2024-04-07 21:17:47.000000 feloopy-0.2.9/feloopy/generators/solution/mealpy_solution_generator.py
+-rw-rw-rw-   0        0        0     2136 2024-04-07 21:17:47.000000 feloopy-0.2.9/feloopy/generators/solution/mip_solution_generator.py
+-rw-rw-rw-   0        0        0     3615 2024-04-07 21:17:47.000000 feloopy-0.2.9/feloopy/generators/solution/niapy_solution_generator.py
+-rw-rw-rw-   0        0        0     3100 2024-04-07 21:17:47.000000 feloopy-0.2.9/feloopy/generators/solution/ortools_cp_solution_generator.py
+-rw-rw-rw-   0        0        0     3403 2024-04-07 21:17:47.000000 feloopy-0.2.9/feloopy/generators/solution/ortools_solution_generator.py
+-rw-rw-rw-   0        0        0     2709 2024-04-07 21:17:47.000000 feloopy-0.2.9/feloopy/generators/solution/picos_solution_generator.py
+-rw-rw-rw-   0        0        0     4425 2024-04-07 21:17:47.000000 feloopy-0.2.9/feloopy/generators/solution/pulp_solution_generator.py
+-rw-rw-rw-   0        0        0     3590 2024-04-07 21:17:47.000000 feloopy-0.2.9/feloopy/generators/solution/pygad_solution_generator.py
+-rw-rw-rw-   0        0        0     4608 2024-04-07 21:17:47.000000 feloopy-0.2.9/feloopy/generators/solution/pymoo_solution_generator.py
+-rw-rw-rw-   0        0        0     2213 2024-04-07 21:17:47.000000 feloopy-0.2.9/feloopy/generators/solution/pymprog_solution_generator.py
+-rw-rw-rw-   0        0        0     5151 2024-04-07 21:17:47.000000 feloopy-0.2.9/feloopy/generators/solution/pymultiobjective_solution_generator.py
+-rw-rw-rw-   0        0        0     6085 2024-04-07 21:17:47.000000 feloopy-0.2.9/feloopy/generators/solution/pyomo_solution_generator.py
+-rw-rw-rw-   0        0        0     3244 2024-04-07 21:17:47.000000 feloopy-0.2.9/feloopy/generators/solution/rsome_dro_solution_generator.py
+-rw-rw-rw-   0        0        0     3272 2024-04-07 21:17:47.000000 feloopy-0.2.9/feloopy/generators/solution/rsome_ro_solution_generator.py
+-rw-rw-rw-   0        0        0     3422 2024-04-07 21:17:47.000000 feloopy-0.2.9/feloopy/generators/solution/seeker_solution_generator.py
+-rw-rw-rw-   0        0        0     2142 2024-04-07 21:17:47.000000 feloopy-0.2.9/feloopy/generators/solution/xpress_solution_generator.py
+-rw-rw-rw-   0        0        0     4178 2024-04-07 21:17:47.000000 feloopy-0.2.9/feloopy/generators/solution_generator.py
+drwxrwxrwx   0        0        0        0 2024-04-07 21:21:03.142909 feloopy-0.2.9/feloopy/generators/variable/
+-rw-rw-rw-   0        0        0      117 2024-04-07 21:17:47.000000 feloopy-0.2.9/feloopy/generators/variable/__init__.py
+-rw-rw-rw-   0        0        0     7400 2024-04-07 21:17:47.000000 feloopy-0.2.9/feloopy/generators/variable/copt_variable_generator.py
+-rw-rw-rw-   0        0        0     2948 2024-04-07 21:17:47.000000 feloopy-0.2.9/feloopy/generators/variable/cplex_cp_variable_generator.py
+-rw-rw-rw-   0        0        0     3258 2024-04-07 21:17:47.000000 feloopy-0.2.9/feloopy/generators/variable/cplex_variable_generator.py
+-rw-rw-rw-   0        0        0     3940 2024-04-07 21:17:47.000000 feloopy-0.2.9/feloopy/generators/variable/cvxpy_variable_generator.py
+-rw-rw-rw-   0        0        0     3519 2024-04-07 21:17:47.000000 feloopy-0.2.9/feloopy/generators/variable/cylp_variable_generator.py
+-rw-rw-rw-   0        0        0     2743 2024-04-07 21:17:47.000000 feloopy-0.2.9/feloopy/generators/variable/gamspy_variable_generator.py
+-rw-rw-rw-   0        0        0     4013 2024-04-07 21:17:47.000000 feloopy-0.2.9/feloopy/generators/variable/gekko_variable_generator.py
+-rw-rw-rw-   0        0        0     7425 2024-04-07 21:17:47.000000 feloopy-0.2.9/feloopy/generators/variable/gurobi_variable_generator.py
+-rw-rw-rw-   0        0        0     3526 2024-04-07 21:17:47.000000 feloopy-0.2.9/feloopy/generators/variable/highs_variable_generator.py
+-rw-rw-rw-   0        0        0     4000 2024-04-07 21:17:47.000000 feloopy-0.2.9/feloopy/generators/variable/linopy_variable_generator.py
+-rw-rw-rw-   0        0        0     2780 2024-04-07 21:17:47.000000 feloopy-0.2.9/feloopy/generators/variable/mip_variable_generator.py
+-rw-rw-rw-   0        0        0     3567 2024-04-07 21:17:47.000000 feloopy-0.2.9/feloopy/generators/variable/ortools_cp_variable_generator.py
+-rw-rw-rw-   0        0        0     3783 2024-04-07 21:17:47.000000 feloopy-0.2.9/feloopy/generators/variable/ortools_variable_generator.py
+-rw-rw-rw-   0        0        0     3001 2024-04-07 21:17:47.000000 feloopy-0.2.9/feloopy/generators/variable/picos_variable_generator.py
+-rw-rw-rw-   0        0        0     3487 2024-04-07 21:17:47.000000 feloopy-0.2.9/feloopy/generators/variable/pulp_variable_generator.py
+-rw-rw-rw-   0        0        0     3333 2024-04-07 21:17:47.000000 feloopy-0.2.9/feloopy/generators/variable/pymprog_variable_generator.py
+-rw-rw-rw-   0        0        0     2529 2024-04-07 21:17:47.000000 feloopy-0.2.9/feloopy/generators/variable/pyomo_variable_generator.py
+-rw-rw-rw-   0        0        0     5000 2024-04-07 21:17:47.000000 feloopy-0.2.9/feloopy/generators/variable/rsome_dro_variable_generator.py
+-rw-rw-rw-   0        0        0     5023 2024-04-07 21:17:47.000000 feloopy-0.2.9/feloopy/generators/variable/rsome_ro_variable_generator.py
+-rw-rw-rw-   0        0        0     2685 2024-04-07 21:17:47.000000 feloopy-0.2.9/feloopy/generators/variable/seeker_variable_generator.py
+-rw-rw-rw-   0        0        0     4057 2024-04-07 21:17:47.000000 feloopy-0.2.9/feloopy/generators/variable/xpress_variable_generator.py
+-rw-rw-rw-   0        0        0     3991 2024-04-07 21:17:47.000000 feloopy-0.2.9/feloopy/generators/variable_generator.py
+drwxrwxrwx   0        0        0        0 2024-04-07 21:21:03.205427 feloopy-0.2.9/feloopy/helpers/
+-rw-rw-rw-   0        0        0      216 2024-04-07 21:17:47.000000 feloopy-0.2.9/feloopy/helpers/__init__.py
+-rw-rw-rw-   0        0        0      364 2024-04-07 21:17:47.000000 feloopy-0.2.9/feloopy/helpers/context_manager.py
+-rw-rw-rw-   0        0        0     1316 2024-04-07 21:17:47.000000 feloopy-0.2.9/feloopy/helpers/empty.py
+-rw-rw-rw-   0        0        0      212 2024-04-07 21:17:47.000000 feloopy-0.2.9/feloopy/helpers/error.py
+-rw-rw-rw-   0        0        0    21824 2024-04-07 21:17:47.000000 feloopy-0.2.9/feloopy/helpers/formatter.py
+drwxrwxrwx   0        0        0        0 2024-04-07 21:21:03.378167 feloopy-0.2.9/feloopy/operators/
+-rw-rw-rw-   0        0        0      471 2024-04-07 21:17:47.000000 feloopy-0.2.9/feloopy/operators/__init__.py
+-rw-rw-rw-   0        0        0     8163 2024-04-07 21:17:47.000000 feloopy-0.2.9/feloopy/operators/common.py
+-rw-rw-rw-   0        0        0    18277 2024-04-07 21:17:47.000000 feloopy-0.2.9/feloopy/operators/data_handler.py
+-rw-rw-rw-   0        0        0      117 2024-04-07 21:17:47.000000 feloopy-0.2.9/feloopy/operators/epsilon.py
+-rw-rw-rw-   0        0        0      206 2024-04-07 21:17:47.000000 feloopy-0.2.9/feloopy/operators/exact.py
+-rw-rw-rw-   0        0        0      388 2024-04-07 21:17:47.000000 feloopy-0.2.9/feloopy/operators/fix_operators.py
+-rw-rw-rw-   0        0        0      297 2024-04-07 21:17:47.000000 feloopy-0.2.9/feloopy/operators/heuristic.py
+-rw-rw-rw-   0        0        0     6035 2024-04-07 21:17:47.000000 feloopy-0.2.9/feloopy/operators/heuristic_operators.py
+-rw-rw-rw-   0        0        0     2153 2024-04-07 21:17:47.000000 feloopy-0.2.9/feloopy/operators/math_operators.py
+-rw-rw-rw-   0        0        0     1596 2024-04-07 21:17:47.000000 feloopy-0.2.9/feloopy/operators/metrics.py
+-rw-rw-rw-   0        0        0      117 2024-04-07 21:17:47.000000 feloopy-0.2.9/feloopy/operators/pareto.py
+-rw-rw-rw-   0        0        0      294 2024-04-07 21:17:47.000000 feloopy-0.2.9/feloopy/operators/random_operators.py
+-rw-rw-rw-   0        0        0      400 2024-04-07 21:17:47.000000 feloopy-0.2.9/feloopy/operators/set_operators.py
+-rw-rw-rw-   0        0        0     2091 2024-04-07 21:17:47.000000 feloopy-0.2.9/feloopy/operators/update_operators.py
+-rw-rw-rw-   0        0        0     1184 2024-04-07 21:17:47.000000 feloopy-0.2.9/feloopy/operators/validator.py
+drwxrwxrwx   0        0        0        0 2024-04-07 21:21:03.378167 feloopy-0.2.9/feloopy.egg-info/
+-rw-rw-rw-   0        0        0    10479 2024-04-07 21:21:00.000000 feloopy-0.2.9/feloopy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     7618 2024-04-07 21:21:00.000000 feloopy-0.2.9/feloopy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-07 21:21:00.000000 feloopy-0.2.9/feloopy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       91 2024-04-07 21:21:00.000000 feloopy-0.2.9/feloopy.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0     1589 2024-04-07 21:21:00.000000 feloopy-0.2.9/feloopy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-07 21:21:00.000000 feloopy-0.2.9/feloopy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3014 2024-04-07 21:17:47.000000 feloopy-0.2.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-07 21:21:03.409414 feloopy-0.2.9/setup.cfg
+-rw-rw-rw-   0        0        0     3661 2024-04-07 21:17:47.000000 feloopy-0.2.9/setup.py
```

### Comparing `feloopy-0.2.8/LICENSE` & `feloopy-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.8/feloopy/algorithms/heuristic/DE.py` & `feloopy-0.2.9/feloopy/algorithms/heuristic/DE.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.8/feloopy/algorithms/heuristic/GA.py` & `feloopy-0.2.9/feloopy/algorithms/heuristic/GA.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.8/feloopy/algorithms/heuristic/GWO.py` & `feloopy-0.2.9/feloopy/algorithms/heuristic/GWO.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.8/feloopy/algorithms/heuristic/SA.py` & `feloopy-0.2.9/feloopy/algorithms/heuristic/SA.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.8/feloopy/algorithms/heuristic/TS.py` & `feloopy-0.2.9/feloopy/algorithms/heuristic/TS.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.8/feloopy/classes/constraint_programming.py` & `feloopy-0.2.9/feloopy/classes/constraint_programming.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 
 This module defines a class, `ConstraintProgrammingClass`, that is used in constraint programming.
 
 Copyright (c) 2022-2024, Keivan Tafakkori. All rights reserved.
 See the file LICENSE file for licensing details.
 """
 
-
 from .event_variable import EventVariable
 from .special_constraint import Expression
 from typing import Optional, Union
 import numpy as np
 import math as mt
 
 class ConstraintFeature:
@@ -582,8 +581,25 @@
         :param expr1: First expression.
         :param expr2: Second expression.
         """
         if self.features['interface_name'] == 'cplex_cp':
             return self.model.greater_than(expr1, expr2)
             
         if self.features['interface_name'] == 'ortools_cp':
-            return self.model.Add(expr1 > expr2)
+            return self.model.Add(expr1 > expr2)
+        
+    def cp_add_exactly_one(self, variable_list):
+
+        if self.features['interface_name'] == 'ortools_cp':
+            return self.model.AddExactlyOne(variable_list)
+
+    def cp_add_at_least_one(self, variable_list):
+
+        if self.features['interface_name'] == 'ortools_cp':
+            return self.model.AddAtLeastOne(variable_list)
+
+    def cp_add_all_different(self, expressions):
+
+        if self.features['interface_name'] == 'cplex_cp':
+            return self.model.all_diff(expressions)
+        if self.features['interface_name'] == 'ortools_cp':
+            return self.model.AddAllDifferent(expressions)
```

### Comparing `feloopy-0.2.8/feloopy/classes/event_variable.py` & `feloopy-0.2.9/feloopy/classes/event_variable.py`

 * *Files 12% similar despite different names*

```diff
@@ -51,40 +51,40 @@
 
         if len(event) == 1:
             event = [event[0], None, None]
 
         if dim == 0:
 
             if self.features['interface_name'] == 'cplex_cp':
-                self.mainvars[("evar", name)] = self.model.interval_var(start=event[1], size=event[0], end=event[2], name=name, optional=optional)
-                self.maindims[name] = dim
-                return self.mainvars[("evar", name)]
+                self.features['variables'][("evar", name)] = self.model.interval_var(start=event[1], size=event[0], end=event[2], name=name, optional=optional)
+                self.features['dimensions'][name] = dim
+                return self.features['variables'][("evar", name)]
                 
             elif self.features['interface_name'] == 'ortools_cp':
-                self.mainvars[("evar", name)] = self.model.NewOptionalIntervalVar(start=event[1], size=event[0], end=event[2], name=name, is_present=optional)
-                self.maindims[name] = dim
-                return self.mainvars[("evar", name)]
+                self.features['variables'][("evar", name)] = self.model.NewOptionalIntervalVar(start=event[1], size=event[0], end=event[2], name=name, is_present=optional)
+                self.features['dimensions'][name] = dim
+                return self.features['variables'][("evar", name)]
         else:
 
             if self.features['interface_name'] == 'cplex_cp':
 
                 if len(dim) == 1:
-                    self.mainvars[("evar", name)] = {key: self.model.interval_var(start=event[1], size=event[0], end=event[2], name=f"{name}{key}", optional=optional) for key in dim[0]}
-                    self.maindims[name] = dim
-                    return self.mainvars[("evar", name)] 
+                    self.features['variables'][("evar", name)] = {key: self.model.interval_var(start=event[1], size=event[0], end=event[2], name=f"{name}{key}", optional=optional) for key in dim[0]}
+                    self.features['dimensions'][name] = dim
+                    return self.features['variables'][("evar", name)] 
                     
                 else:
-                    self.mainvars[("evar", name)]  = {key: self.model.interval_var(start=event[1], size=event[0], end=event[2], name=f"{name}{key}", optional=optional) for key in sets(*dim)}
-                    self.maindims[name] = dim
-                    return  self.mainvars[("evar", name)] 
+                    self.features['variables'][("evar", name)]  = {key: self.model.interval_var(start=event[1], size=event[0], end=event[2], name=f"{name}{key}", optional=optional) for key in sets(*dim)}
+                    self.features['dimensions'][name] = dim
+                    return  self.features['variables'][("evar", name)] 
 
             elif self.features['interface_name'] == 'ortools_cp':
 
                 if len(dim) == 1:
-                    self.mainvars[("evar", name)] = {key: self.model.NewOptionalIntervalVar(start=event[1], size=event[0], end=event[2], name=f"{name}{key}", is_present=optional) for key in dim[0]}
-                    self.maindims[name] = dim
-                    return self.mainvars[("evar", name)]
+                    self.features['variables'][("evar", name)] = {key: self.model.NewOptionalIntervalVar(start=event[1], size=event[0], end=event[2], name=f"{name}{key}", is_present=optional) for key in dim[0]}
+                    self.features['dimensions'][name] = dim
+                    return self.features['variables'][("evar", name)]
                     
                 else:
-                    self.mainvars[("evar", name)]  = {key: self.model.NewOptionalIntervalVar(start=event[1], size=event[0], end=event[2], name=f"{name}{key}", is_present=optional) for key in sets(*dim)}
-                    self.maindims[name] = dim
-                    return self.mainvars[("evar", name)]
+                    self.features['variables'][("evar", name)]  = {key: self.model.NewOptionalIntervalVar(start=event[1], size=event[0], end=event[2], name=f"{name}{key}", is_present=optional) for key in sets(*dim)}
+                    self.features['dimensions'][name] = dim
+                    return self.features['variables'][("evar", name)]
```

### Comparing `feloopy-0.2.8/feloopy/classes/linearization.py` & `feloopy-0.2.9/feloopy/classes/linearization.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.8/feloopy/classes/multidim_variable.py` & `feloopy-0.2.9/feloopy/classes/multidim_variable.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 """
-
-**Multi-dimensional variables module**
+Multi-dimensional variables module
 
 This module facilitates the creation of various types of multi-dimensional variables.
 
+Copyright (c) 2022-2024, Keivan Tafakkori. All rights reserved.
+See the file LICENSE file for licensing details.
 """
 
-# Copyright (c) 2022-2024, Keivan Tafakkori. All rights reserved.
-# See the file LICENSE file for licensing details.
-
 from typing import List, Optional, Union
 import itertools as it
 import numpy as np
 from ..operators.fix_operators import fix_dims
 from ..operators.update_operators import update_variable_features
 
 
+    
 class MultidimVariable:
     """Specifies the variable type."""
 
 class MultidimVariableClass:
     """Class that provides methods to create multi-dimensional variables."""
     
     def fvar(
         self,
         name: str,
         dim: List[int] = 0,
         bound: List[Optional[float]] = [None, None]
     ) -> MultidimVariable:
+        
         """
         Creates and returns a free variable.
 
         Parameters
         ----------
         name : str
             Name.
@@ -42,24 +42,24 @@
 
         Returns
         -------
         MultidimVariable
             A free variable.
         """
 
-        dim = fix_dims(dim)
+        dim = self.fix_ifneeded(dim)
         self.features = update_variable_features(name, dim, bound, 'free_variable_counter', self.features)
 
         if self.features['solution_method'] == 'exact':
             from ..generators import variable_generator
-            self.mainvars[("fvar", name)] = variable_generator.generate_variable(
+            self.features['variables'][("fvar", name)] = variable_generator.generate_variable(
                 self.features['interface_name'], self.model, 'fvar', name, bound, dim
             )
-            self.maindims[name] = dim
-            return self.mainvars[("fvar", name)]
+            self.features['dimensions'][name] = dim
+            return self.features['variables'][("fvar", name)]
 
         elif self.features['solution_method'] == 'heuristic':
             from ..operators.heuristic_operators import generate_heuristic_variable
             return generate_heuristic_variable(
                 self.features, 'fvar', name, dim, bound, self.agent, self.no_agents
             )
         
@@ -83,41 +83,41 @@
 
         Returns
         -------
         MultidimVariable
             A positive variable.
         """
 
-        dim = fix_dims(dim)
+        dim = self.fix_ifneeded(dim)
         self.features = update_variable_features(name, dim, bound, 'positive_variable_counter', self.features)
 
         if self.features['solution_method'] == 'exact':
             from ..generators import variable_generator
-            self.mainvars[("pvar", name)] = variable_generator.generate_variable(
+            self.features['variables'][("pvar", name)] = variable_generator.generate_variable(
                 self.features['interface_name'], self.model, 'pvar', name, bound, dim
             )
-            self.maindims[name] = dim
+            self.features['dimensions'][name] = dim
 
             if self.features['interface_name'] in ['rsome_ro', 'rsome_dro', 'cvxpy']:
                 if dim == 0:
-                    self.con(self.mainvars[("pvar", name)] >= 0)
+                    self.con(self.features['variables'][("pvar", name)] >= 0)
                     if bound[1] is not None:
-                        self.con(self.mainvars[("pvar", name)] <= bound[1])
+                        self.con(self.features['variables'][("pvar", name)] <= bound[1])
                 elif len(dim) == 1:
                     for i in dim[0]:
-                        self.con(self.mainvars[("pvar", name)][i] >= 0)
+                        self.con(self.features['variables'][("pvar", name)][i] >= 0)
                         if bound[1] is not None:
-                            self.con(self.mainvars[("pvar", name)][i] <= bound[1])
+                            self.con(self.features['variables'][("pvar", name)][i] <= bound[1])
                 else:
                     for i in it.product(*tuple(dim)):
-                        self.con(self.mainvars[("pvar", name)][i] >= 0)
+                        self.con(self.features['variables'][("pvar", name)][i] >= 0)
                         if bound[1] is not None:
-                            self.con(self.mainvars[("pvar", name)][i] <= bound[1])
+                            self.con(self.features['variables'][("pvar", name)][i] <= bound[1])
 
-            return self.mainvars[("pvar", name)]
+            return self.features['variables'][("pvar", name)]
 
         elif self.features['solution_method'] == 'heuristic':
             from ..operators.heuristic_operators import generate_heuristic_variable
             return generate_heuristic_variable(
                 self.features, 'pvar', name, dim, bound, self.agent, self.no_agents
             )
     
@@ -141,41 +141,41 @@
 
         Returns
         -------
         MultidimVariable
             An integer variable.
         """
 
-        dim = fix_dims(dim)
+        dim = self.fix_ifneeded(dim)
         self.features = update_variable_features(name, dim, bound, 'integer_variable_counter', self.features)
 
         if self.features['solution_method'] == 'exact':
             from ..generators import variable_generator
-            self.mainvars[("ivar", name)] = variable_generator.generate_variable(
+            self.features['variables'][("ivar", name)] = variable_generator.generate_variable(
                 self.features['interface_name'], self.model, 'ivar', name, bound, dim
             )
-            self.maindims[name] = dim
+            self.features['dimensions'][name] = dim
 
             if self.features['interface_name'] in ['rsome_ro', 'rsome_dro', 'cvxpy']:
                 if dim == 0:
-                    self.con(self.mainvars[("ivar", name)] >= 0)
+                    self.con(self.features['variables'][("ivar", name)] >= 0)
                     if bound[1] is not None:
-                        self.con(self.mainvars[("ivar", name)] <= bound[1])
+                        self.con(self.features['variables'][("ivar", name)] <= bound[1])
                 elif len(dim) == 1:
                     for i in dim[0]:
-                        self.con(self.mainvars[("ivar", name)][i] >= 0)
+                        self.con(self.features['variables'][("ivar", name)][i] >= 0)
                         if bound[1] is not None:
-                            self.con(self.mainvars[("ivar", name)][i] <= bound[1])
+                            self.con(self.features['variables'][("ivar", name)][i] <= bound[1])
                 else:
                     for i in it.product(*tuple(dim)):
-                        self.con(self.mainvars[("ivar", name)][i] >= 0)
+                        self.con(self.features['variables'][("ivar", name)][i] >= 0)
                         if bound[1] is not None:
-                            self.con(self.mainvars[("ivar", name)][i] <= bound[1])
+                            self.con(self.features['variables'][("ivar", name)][i] <= bound[1])
 
-            return self.mainvars[("ivar", name)]
+            return self.features['variables'][("ivar", name)]
 
         elif self.features['solution_method'] == 'heuristic':
             from ..operators.heuristic_operators import generate_heuristic_variable
             return generate_heuristic_variable(
                 self.features, 'ivar', name, dim, bound, self.agent, self.no_agents
             )
 
@@ -199,37 +199,37 @@
 
         Returns
         -------
         MultidimVariable
             A binary variable.
         """
 
-        dim = fix_dims(dim)
+        dim = self.fix_ifneeded(dim)
         self.features = update_variable_features(name, dim, bound, 'binary_variable_counter', self.features)
 
         if self.features['solution_method'] == 'exact':
             from ..generators import variable_generator
-            self.mainvars[("bvar", name)] = variable_generator.generate_variable(
+            self.features['variables'][("bvar", name)] = variable_generator.generate_variable(
                 self.features['interface_name'], self.model, 'bvar', name, bound, dim
             )
-            self.maindims[name] = dim
+            self.features['dimensions'][name] = dim
 
             if self.features['interface_name'] in ['cvxpy']:
                 if dim == 0:
-                    self.con(self.mainvars[("bvar", name)] >= 0)
-                    self.con(self.mainvars[("bvar", name)] <= 1)
+                    self.con(self.features['variables'][("bvar", name)] >= 0)
+                    self.con(self.features['variables'][("bvar", name)] <= 1)
                 elif len(dim) == 1:
                     for i in dim[0]:
-                        self.con(self.mainvars[("bvar", name)][i] >= 0)
-                        self.con(self.mainvars[("bvar", name)][i] <= 1)
+                        self.con(self.features['variables'][("bvar", name)][i] >= 0)
+                        self.con(self.features['variables'][("bvar", name)][i] <= 1)
                 else:
                     for i in it.product(*tuple(dim)):
-                        self.con(self.mainvars[("bvar", name)][i] >= 0)
-                        self.con(self.mainvars[("bvar", name)][i] <= 1)
-            return self.mainvars[("bvar", name)]
+                        self.con(self.features['variables'][("bvar", name)][i] >= 0)
+                        self.con(self.features['variables'][("bvar", name)][i] <= 1)
+            return self.features['variables'][("bvar", name)]
 
         elif self.features['solution_method'] == 'heuristic':
             from ..operators.heuristic_operators import generate_heuristic_variable
             return generate_heuristic_variable(
                 self.features, 'bvar', name, dim, bound, self.agent, self.no_agents
             )
             
@@ -279,15 +279,15 @@
             Dimensions of this variable. Default: 0.
 
         Returns
         -------
         MultidimVariable
             A random variable.
         """
-        dim = fix_dims(dim)
+        dim = self.fix_ifneeded(dim)
         from ..generators import variable_generator
         return variable_generator.generate_variable(
             self.features['interface_name'], self.model, 'rvar', name, [None, None], dim
         )
         
     def dvar(
         self,
@@ -306,15 +306,15 @@
 
         Returns
         -------
         np.ndarray
             A dependent variable.
 
         """
-        dim = fix_dims(dim)
+        dim = self.fix_ifneeded(dim)
 
         if self.no_agents is not None:
             default_pop = self.no_agents
         else:
             default_pop = 100
 
         if self.features['solution_method'] == 'exact':
```

### Comparing `feloopy-0.2.8/feloopy/classes/special_constraint.py` & `feloopy-0.2.9/feloopy/classes/special_constraint.py`

 * *Files 1% similar despite different names*

```diff
@@ -308,28 +308,28 @@
             self.features['indicators'].append(self.features['indicators'][-1] + 1)
         except:
             self.features['indicators'] = [0]
         z = self.pvar(f"indicator{self.features['indicators'][-1]}")
         self.con(expr - z == rhs)
         return z
 
-    def con_expr_in_bound(self, expr: Expression, lb: Optional[float] = None, ub: Optional[float] = None, label: Optional[str] = None):
+    def con_expr_in_bound(self, expr: Expression, lb: Optional[float] = None, ub: Optional[float] = None, name: Optional[str] = None):
         """
         Creates upper and/or lower bounds on the given variable in the optimization model.
 
         Parameters:
             expr (Expression): The variable expression.
             lb (float, optional): Lower bound. Default is None.
             ub (float, optional): Upper bound. Default is None.
-            label (str, optional): Label for the constraint. Default is None.
+            name (str, optional): name for the constraint. Default is None.
         """
         if lb is not None:
-            self.con(expr >= lb, label=label)
+            self.con(expr >= lb, name=name)
         if ub is not None:
-            self.con(expr <= ub, label=label)
+            self.con(expr <= ub, name=name)
 
     def con_abs_leq(self, expr: Expression, rhs: float):
         """
         Linearizes a constraint like │a│ <= b.
 
         Parameters:
             expr (Expression): The expression inside the absolute value.
```

### Comparing `feloopy-0.2.8/feloopy/classes/tensor_variable.py` & `feloopy-0.2.9/feloopy/classes/tensor_variable.py`

 * *Files 11% similar despite different names*

```diff
@@ -52,19 +52,19 @@
             A tensor variable that accepts matrix/tensor-wise operations.
         """
         dim = fix_dims(shape)
         self.features = update_variable_features(name, dim, bound or [None, None], 'free_variable_counter', self.features)
         
         if self.features['solution_method'] == 'exact':
             from ..generators import variable_generator
-            self.mainvars[("ftvar", name)] = variable_generator.generate_variable(
+            self.features['variables'][("ftvar", name)] = variable_generator.generate_variable(
                 self.features['interface_name'], self.model, 'ftvar', name, bound, dim
             )
-            self.maindims[name] = dim
-            return self.mainvars[("ftvar", name)]
+            self.features['dimensions'][name] = dim
+            return self.features['variables'][("ftvar", name)]
 
         raise ValueError(f"Error: TensorVariable '{name}' cannot be created.")
     
     def ptvar(
         self,
         name: str,
         shape: Optional[Union[int, List[Union[int, range]]]] = 0,
@@ -89,26 +89,26 @@
         """
         dim = fix_dims(shape)
         self.features = update_variable_features(name, dim, bound or [0, None], 'positive_variable_counter', self.features)
 
         if self.features['solution_method'] == 'exact':
             from ..generators import variable_generator
 
-            self.mainvars[("ptvar", name)] = variable_generator.generate_variable(
+            self.features['variables'][("ptvar", name)] = variable_generator.generate_variable(
                 self.features['interface_name'], self.model, 'ptvar', name, bound, dim
             )
-            self.maindims[name] = dim
+            self.features['dimensions'][name] = dim
 
             if self.features['interface_name'] in ['rsome_ro', 'rsome_dro', 'cvxpy']:
-                self.con(self.mainvars[("ptvar", name)] >= 0)
+                self.con(self.features['variables'][("ptvar", name)] >= 0)
 
                 if bound and bound[1] is not None:
-                    self.con(self.mainvars[("ptvar", name)] <= bound[1])
+                    self.con(self.features['variables'][("ptvar", name)] <= bound[1])
 
-            return self.mainvars[("ptvar", name)]
+            return self.features['variables'][("ptvar", name)]
     
         raise ValueError(f"Error: TensorVariable '{name}' cannot be created.")
     
     def itvar(
         self,
         name: str,
         shape: Optional[Union[int, List[Union[int, range]]]] = 0,
@@ -134,19 +134,19 @@
 
         dim = fix_dims(shape)
         self.features = update_variable_features(name, dim, bound or [0, None], 'integer_variable_counter', self.features)
 
         if self.features['solution_method'] == 'exact':
             from ..generators import variable_generator
 
-            self.mainvars[("itvar", name)] = variable_generator.generate_variable(
+            self.features['variables'][("itvar", name)] = variable_generator.generate_variable(
                 self.features['interface_name'], self.model, 'itvar', name, bound, dim
             )
-            self.maindims[name] = dim
-            return self.mainvars[("itvar", name)]
+            self.features['dimensions'][name] = dim
+            return self.features['variables'][("itvar", name)]
 
         raise ValueError(f"Error: TensorVariable '{name}' cannot be created.")
     
     def btvar(
         self,
         name: str,
         shape: Optional[Union[int, List[Union[int, range]]]] = 0,
@@ -172,19 +172,19 @@
 
         dim = fix_dims(shape)
         self.features = update_variable_features(name, dim, bound or [0, 1], 'binary_variable_counter', self.features)
 
         if self.features['solution_method'] == 'exact':
             from ..generators import variable_generator
 
-            self.mainvars[("btvar", name)] = variable_generator.generate_variable(
+            self.features['variables'][("btvar", name)] = variable_generator.generate_variable(
                 self.features['interface_name'], self.model, 'btvar', name, bound, dim
             )
-            self.maindims[name] = dim
-            return self.mainvars[("btvar", name)]
+            self.features['dimensions'][name] = dim
+            return self.features['variables'][("btvar", name)]
 
         raise ValueError(f"Error: TensorVariable '{name}' cannot be created.")
 
     def rtvar(
         self,
         name: str,
         shape: Optional[Union[int, List[Union[int, range]]]] = 0
```

### Comparing `feloopy-0.2.8/feloopy/cli.py` & `feloopy-0.2.9/feloopy/cli.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.8/feloopy/clitools/pkg_manager_detector.py` & `feloopy-0.2.9/feloopy/clitools/pkg_manager_detector.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.8/feloopy/clitools/utils.py` & `feloopy-0.2.9/feloopy/clitools/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 import zipfile
 import subprocess
 import sys
 import urllib.request
 from tqdm import tqdm
 from datetime import datetime
 
-__version__ = "v0.2.8"
+__version__ = "v0.2.9"
 
 def download_and_extract(url, output_folder, filename):
    print(f"Downloading and unpacking {filename}")
    with urllib.request.urlopen(url) as url:
        f = open(filename, 'wb')
        total_size = int(url.info().get("Content-Length", 0))
        chunk_size = 1024 # 1 KB
@@ -54,21 +54,21 @@
 
  os.chdir(install_dir)
 
  os.makedirs("solvers", exist_ok=True)
 
  versions = {
      "cbc": ("2.10.11", "https://github.com/coin-or/Cbc/releases/download/releases%2F{version}/Cbc-releases.{version}-x86_64-w64-mingw64.zip"),
-     "highs": ("1.5.3", "https://github.com/JuliaBinaryWrappers/HiGHSstatic_jll.jl/releases/download/HiGHSstatic-v{version}%2B0/HiGHSstatic.v{version}.x86_64-w64-mingw32.tar.gz"),
-     "ipopt": ("3.14.13", "https://github.com/coin-or/Ipopt/releases/download/releases%2F{version}/Ipopt-{version}-win64-msvs2019-md.zip"),
+     "highs": ("1.7.0", "https://github.com/JuliaBinaryWrappers/HiGHSstatic_jll.jl/releases/download/HiGHSstatic-v{version}%2B0/HiGHSstatic.v{version}.x86_64-w64-mingw32.tar.gz"),
+     "ipopt": ("3.14.14", "https://github.com/coin-or/Ipopt/releases/download/releases%2F{version}/Ipopt-{version}-win64-msvs2019-md.zip"),
      "glpk": ("4.65", "https://sourceforge.net/projects/winglpk/files/winglpk/GLPK-{version}/winglpk-{version}.zip/download"),
      "bonmin": ("1.4.0", "https://www.coin-or.org/download/binary/Bonmin/Bonmin-{version}-win32-msvc9.zip"),
      "couenne": ("0.3.2", "https://www.coin-or.org/download/binary/Couenne/Couenne-{version}-win32-msvc9.zip"),
-     "scip": ("8.0.4", "https://github.com/scipopt/scip/releases/download/v{version_no_dots}/SCIPOptSuite-{version}-win64-VS15.exe"),
-     "git": ("2.43.0", "https://github.com/git-for-windows/git/releases/download/v{version}.windows.1/Git-{version}-64-bit.exe"),
+     "scip": ("9.0.0", "https://github.com/scipopt/scip/releases/download/v{version_no_dots}/SCIPOptSuite-{version}-win64-VS15.exe"),
+     "git": ("2.44.0", "https://github.com/git-for-windows/git/releases/download/v{version}.windows.1/Git-{version}-64-bit.exe"),
  }
 
  for solver, (version, url) in versions.items():
      url = url.format(version=version, version_no_dots=version.replace(".", ""))
      output_folder = os.path.join("solvers", solver + "-windows")
      if "zip" in url.lower():
         filename = os.path.join("solvers", solver + "-windows.zip")
```

### Comparing `feloopy-0.2.8/feloopy/feloopy.py` & `feloopy-0.2.9/feloopy/feloopy.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,173 +1,733 @@
 # Copyright (c) 2022-2024, Keivan Tafakkori. All rights reserved.
 # See the file LICENSE file for licensing details.
 
-__author__ = ['Keivan Tafakkori']
-
-
-from .helpers.empty import *
-from .helpers.error import *
-from .helpers.formatter import *
-from .operators.data_handler import *
-from .operators.fix_operators import *
-from .operators.heuristic_operators import *
-from .operators.math_operators import *
-from .operators.random_operators import *
-from .operators.set_operators import *
-from .operators.update_operators import *
-
-from collections import defaultdict
-from tabulate import tabulate as tb
-from typing import Literal, List, Dict, Tuple, Union, Optional, Any, Callable
+import contextlib
 import importlib
 import itertools as it
 import math as mt
-import numpy as np
+import os
 import platform
 import sys
 import time
 import warnings
+from collections import defaultdict
+from typing import Literal, Optional, Union
+from contextlib import suppress
+from .operators.metrics import compute_similarity
+import timeit 
+import copy
+
+import numpy as np
+
+
+__author__ = ['Keivan Tafakkori']
+
+HEURISTIC_ALGORITHMS = [
+    
+    ['feloopy', 'de'],
+    ['feloopy', 'ga'],
+    ['feloopy', 'gwo'],
+    ['feloopy', 'sa'],
+    ['feloopy', 'ts'],
+    
+    ['mealpy', 'a-bfo'], 
+    ['mealpy', 'adap-ba'], 
+    ['mealpy', 'adap-eo'], 
+    ['mealpy', 'augm-aeo'], 
+    ['mealpy', 'base-alo'], 
+    ['mealpy', 'base-bbo'], 
+    ['mealpy', 'base-bro'], 
+    ['mealpy', 'base-chio'],
+    ['mealpy', 'base-de'],
+    ['mealpy', 'base-efo'],
+    ['mealpy', 'base-fbio'],
+    ['mealpy', 'base-foa'],
+
+    ['mealpy', 'base-gco'], 
+    ['mealpy', 'base-gska'], 
+    ['mealpy', 'base-hs'],
+    ['mealpy', 'base-ja'], 
+    ['mealpy', 'base-lco'], 
+    ['mealpy', 'base-mfo'], 
+    ['mealpy', 'base-mvo'], 
+    ['mealpy', 'base-qsa'], 
+    ['mealpy', 'base-saro'], 
+    ['mealpy', 'base-sbo'], 
+    ['mealpy', 'base-sca'], 
+    ['mealpy', 'base-sma'], 
+    ['mealpy', 'base-ssa'], 
+    ['mealpy', 'base-tlo'], 
+    ['mealpy', 'base-vcs'],
+
+    ['mealpy', 'c-pso'], 
+    ['mealpy', 'cl-pso'], 
+    ['mealpy', 'h-pso-tvac'],  
+    ['mealpy', 'cl-pso'], 
+    ['mealpy', 'h-pso-tvac'],
+    ['mealpy', 'p-pso'],
+    ['mealpy', 'orig-pso'],
+
+    ['mealpy', 'base-ga'],
+    ['mealpy', 'single-ga'],
+    ['mealpy', 'multi-ga'], 
+    ['mealpy', 'elite-multi-ga'], 
+    ['mealpy', 'elite-single-ga'],
+
+    ['mealpy', 'orig-abc'],
+    
+    ['mealpy', 'cma-es'], 
+    ['mealpy', 'dev-dmoa'], 
+    ['mealpy', 'dev-soa'], 
+    ['mealpy', 'dev-spbo'],
+
+    ['mealpy', 'enha-aeo'], 
+    ['mealpy', 'enha-two'], 
+    ['mealpy', 'gwo-woa'], 
+    ['mealpy', 'hi-woa'], 
+    ['mealpy', 'impr-aeo'], 
+    ['mealpy', 'impr-bso'], 
+    ['mealpy', 'impr-lco'], 
+    ['mealpy', 'impr-nmra'], 
+    ['mealpy', 'impr-qsa'], 
+    ['mealpy', 'impr-sfo'], 
+    ['mealpy', 'impr-slo'], 
+    ['mealpy', 'itlo'], 
+    ['mealpy', 'ja-de'], 
+    ['mealpy', 'l-sha-de'], 
+    ['mealpy', 'levy-aro'], 
+    ['mealpy', 'levy-ep'], 
+    ['mealpy', 'levy-es'], 
+    ['mealpy', 'levy-ja'], 
+    ['mealpy', 'levy-qsa'], 
+    ['mealpy', 'levy-two'], 
+    ['mealpy', 'modi-aeo'], 
+    ['mealpy', 'modi-ba'], 
+    ['mealpy', 'modi-eo'],
+    ['mealpy', 'modi-slo'],
+    ['mealpy', 'modi101-gto'],
+    ['mealpy', 'modi102-gto'],
+    
+    ['mealpy', 'o-cro'], 
+    ['mealpy', 'oppo-qsa'], 
+    ['mealpy', 'oppo-two'], 
+     
+    ['mealpy', 'orig-acor'], 
+    ['mealpy', 'orig-aeo'], 
+    ['mealpy', 'orig-agto'], 
+    ['mealpy', 'orig-alo'], 
+    ['mealpy', 'orig-ao'], 
+    ['mealpy', 'orig-archoa'], 
+    ['mealpy', 'orig-aro'], 
+    ['mealpy', 'orig-aso'], 
+    ['mealpy', 'orig-avoa'], 
+    ['mealpy', 'orig-ba'], 
+    ['mealpy', 'orig-bbo'], 
+    ['mealpy', 'orig-beesa'], 
+    ['mealpy', 'orig-beesa'], 
+    ['mealpy', 'orig-bes'], 
+    ['mealpy', 'orig-bfo'], 
+    ['mealpy', 'orig-bmo'], 
+    ['mealpy', 'orig-bro'], 
+    ['mealpy', 'orig-bsa'], 
+    ['mealpy', 'orig-bso'], 
+    ['mealpy', 'orig-ca'], 
+    ['mealpy', 'orig-cdo'], 
+    ['mealpy', 'orig-cem'], 
+    ['mealpy', 'orig-cgo'], 
+    ['mealpy', 'orig-chio'], 
+    ['mealpy', 'orig-circle-sa'], 
+    ['mealpy', 'orig-coa'], 
+    ['mealpy', 'orig-cro'], 
+    ['mealpy', 'orig-csa'], 
+    ['mealpy', 'orig-cso'], 
+    ['mealpy', 'orig-dmoa'], 
+    ['mealpy', 'orig-do'], 
+    ['mealpy', 'orig-efo'], 
+    ['mealpy', 'orig-eho'], 
+    ['mealpy', 'orig-eo'], 
+    ['mealpy', 'orig-eoa'], 
+    ['mealpy', 'orig-ep'], 
+    ['mealpy', 'orig-es'], 
+    ['mealpy', 'orig-esoa'], 
+    ['mealpy', 'orig-evo'], 
+    ['mealpy', 'orig-fa'], 
+    ['mealpy', 'orig-fbio'], 
+    ['mealpy', 'orig-ffa'], 
+    ['mealpy', 'orig-fla'], 
+    ['mealpy', 'orig-foa'], 
+    ['mealpy', 'orig-fox'], 
+    ['mealpy', 'orig-fpa'], 
+    ['mealpy', 'orig-gbo'], 
+    ['mealpy', 'orig-gco'], 
+    ['mealpy', 'orig-gjo'], 
+    ['mealpy', 'orig-goa'], 
+    ['mealpy', 'orig-gska'], 
+    ['mealpy', 'orig-gto'],
+    ['mealpy', 'orig-gwo'], 
+    ['mealpy', 'orig-hba'], 
+    ['mealpy', 'orig-hbo'], 
+    ['mealpy', 'orig-hc'], 
+    ['mealpy', 'orig-hgs'], 
+    ['mealpy', 'orig-hgso'], 
+    ['mealpy', 'orig-hho'], 
+    ['mealpy', 'orig-hs'], 
+    ['mealpy', 'orig-huco'], 
+    ['mealpy', 'orig-ica'], 
+    ['mealpy', 'orig-info'], 
+    ['mealpy', 'orig-iwo'], 
+    ['mealpy', 'orig-ja'], 
+    ['mealpy', 'orig-lco'], 
+    ['mealpy', 'orig-ma'], 
+    ['mealpy', 'orig-mfo'], 
+    ['mealpy', 'orig-mgo'], 
+    ['mealpy', 'orig-mpa'], 
+    ['mealpy', 'orig-mrfo'], 
+    ['mealpy', 'orig-msa'], 
+    ['mealpy', 'orig-mvo'], 
+    ['mealpy', 'orig-nmra'], 
+    ['mealpy', 'orig-nro'], 
+    ['mealpy', 'orig-pfa'], 
+     
+    ['mealpy', 'orig-pss'], 
+    ['mealpy', 'orig-qsa'], 
+    ['mealpy', 'orig-rime'], 
+    ['mealpy', 'orig-run'], 
+    ['mealpy', 'orig-sa'], 
+    ['mealpy', 'orig-saro'],
+    ['mealpy', 'orig-sbo'], 
+    ['mealpy', 'orig-sca'], 
+    ['mealpy', 'orig-scso'], 
+    ['mealpy', 'orig-sfo'], 
+    ['mealpy', 'orig-shio'], 
+    ['mealpy', 'orig-sho'], 
+    ['mealpy', 'orig-slo'], 
+    ['mealpy', 'orig-sma'], 
+    ['mealpy', 'orig-soa'], 
+    ['mealpy', 'orig-sos'], 
+    ['mealpy', 'orig-spbo'], 
+    ['mealpy', 'orig-srsr'], 
+    ['mealpy', 'orig-ssa'], 
+    ['mealpy', 'orig-ssdo'], 
+    ['mealpy', 'orig-sso'], 
+    ['mealpy', 'orig-sspidera'], 
+    ['mealpy', 'orig-sspidero'], 
+    ['mealpy', 'orig-tlo'], 
+    ['mealpy', 'orig-tsa'], 
+    ['mealpy', 'orig-tso'], 
+    ['mealpy', 'orig-two'], 
+    ['mealpy', 'orig-vcs'], 
+    ['mealpy', 'orig-warso'], 
+    ['mealpy', 'orig-wca'], 
+    ['mealpy', 'orig-wdo'], 
+    ['mealpy', 'orig-who'], 
+    ['mealpy', 'orig-woa'],  
+    ['mealpy', 'prob-beesa'], 
+    ['mealpy', 'ql-sca'], 
+    ['mealpy', 'rw-gwo'], 
+    ['mealpy', 'sa-de'], 
+    ['mealpy', 'sap-de'], 
+    ['mealpy', 'sea-ho'], 
+    ['mealpy', 'selec-aro'], 
+    ['mealpy', 'sha-de'], 
+    ['mealpy', 'simp-cma-es'],  
+    ['mealpy', 'swarm-hc'], 
+    ['mealpy', 'whale-foa'], 
+    ['mealpy', 'wmqi-mrfo'], 
+
+    ['niapy', 'base-abc'],
+    ['niapy', 'base-ba'],
+    ['niapy', 'base-bea'],
+    ['niapy', 'base-bfo'],
+    ['niapy', 'base-ca'],
+    ['niapy', 'base-clonalg'],
+    ['niapy', 'base-cro'],
+    ['niapy', 'base-cs'],
+    ['niapy', 'base-cso'],
+    ['niapy', 'base-de'],
+    ['niapy', 'base-dynnp-de'],
+    ['niapy', 'base-anp-de'],
+    ['niapy', 'base-ms-de'],
+    ['niapy', 'base-dynnp-ms-de'],
+    ['niapy', 'base-1+1-es'],
+    ['niapy', 'base-m+1-es'],
+    ['niapy', 'base-m+l-es'],
+    ['niapy', 'base-m,l-es'],
+    ['niapy', 'base-fa'],
+    ['niapy', 'base-foa'],
+    ['niapy', 'base-fpa'],
+    ['niapy', 'base-fss'],
+    ['niapy', 'base-bb-fwa'],
+    ['niapy', 'base-fwa'],
+    ['niapy', 'base-e-fwa'],
+    ['niapy', 'base-dyn-fwa-g'],
+    ['niapy', 'base-dyn-fwa'],
+    ['niapy', 'base-ga'],
+    ['niapy', 'base-gsa'],
+    ['niapy', 'base-gso'],
+    ['niapy', 'base-gso-v1'],
+    ['niapy', 'base-gso-v2'],
+    ['niapy', 'base-gso-v3'],
+    ['niapy', 'base-gwo'],
+    ['niapy', 'base-hho'],
+    ['niapy', 'base-hs'],
+    ['niapy', 'base-hs-v1'],
+    ['niapy', 'base-kh'],
+    ['niapy', 'base-loa'],
+    ['niapy', 'base-mbo'],
+    ['niapy', 'base-mfo'],
+    ['niapy', 'base-mke-v1'],
+    ['niapy', 'base-mke-v2'],
+    ['niapy', 'base-mke-v3'],
+    ['niapy', 'base-wvc-pso'],
+    ['niapy', 'base-pso'],
+    ['niapy', 'base-ovc-pso'],
+    ['niapy', 'base-c-pso'],
+    ['niapy', 'base-m-pso'],
+    ['niapy', 'base-mc-pso'],
+    ['niapy', 'base-mcu-pso'],
+    ['niapy', 'base-cl-pso'],
+    ['niapy', 'base-sca'],
+    
+    ['niapy', 'modi-h-ba'],
+    ['niapy', 'modi-de-mts'],
+    ['niapy', 'modi-de-mts-v1'],
+    ['niapy', 'modi-dynnp-de-mts'],
+    ['niapy', 'modi-dynnp-de-mts-v1'],
+    ['niapy', 'modi-ms-de-mts'],
+    ['niapy', 'modi-ms-de-mts-v1'],
+    ['niapy', 'modi-dynnp-ms-de-mts'],
+    ['niapy', 'modi-dynnp-ms-de-mts-v1'],
+    ['niapy', 'modi-sa-de'],
+    ['niapy', 'modi-ms-sa-de'],
+    ['niapy', 'modi-a-ba'],
+    ['niapy', 'modi-sa-ba'],
+    ['niapy', 'modi-hsa-ba'],
+    ['niapy', 'modi-pf-ba'],
+    ['niapy', 'modi-sh-a-de'],
+    ['niapy', 'modi-lpsr-sh-a-de'],
+  
+    ['niapy', 'other-nmm'],
+    ['niapy', 'other-hc'],
+    ['niapy', 'other-sa'],
+    ['niapy', 'other-mts'],
+    ['niapy', 'other-mts1'],
+    ['niapy', 'other-mts-ls1'],
+    ['niapy', 'other-mts-ls2'],
+    ['niapy', 'other-mts-ls3'],
+    ['niapy', 'other-mts-ls1v1'],
+    ['niapy', 'other-mts-ls3v1'],
+    ['niapy', 'other-aso'],
+    ['niapy', 'other-rs'],
+  
+    ]
+
+EXACT_ALGORITHMS = [
+
+    ['copt', 'copt'],
+    ['cplex', 'cplex'],
+    ['cvxpy', 'cbc'],
+    ['cvxpy', 'clarabel'],
+    ['cvxpy', 'copt'],
+    ['cvxpy', 'cplex'],
+    ['cvxpy', 'cvxopt'],
+    ['cvxpy', 'ecos'],
+    ['cvxpy', 'glop'],
+    ['cvxpy', 'glpk-mi'],
+    ['cvxpy', 'glpk'],
+    ['cvxpy', 'gurobi'],
+    ['cvxpy', 'mosek'],
+    ['cvxpy', 'nag'],
+    ['cvxpy', 'osqp'],
+    ['cvxpy', 'pdlp'],
+    ['cvxpy', 'proxqp'],
+    ['cvxpy', 'scip'],
+    ['cvxpy', 'scipy'],
+    ['cvxpy', 'scs'],
+    ['cvxpy', 'xpress'],
+    ['cylp', 'cbc'],
+    ['gams', 'alphaecp'],
+    ['gams', 'antigone'],
+    ['gams', 'baron'],
+    ['gams', 'cbc'],
+    ['gams', 'conopt'],
+    ['gams', 'convert'],
+    ['gams', 'copt'],
+    ['gams', 'cplex'],
+    ['gams', 'de'],
+    ['gams', 'decis'],
+    ['gams', 'dicopt'],
+    ['gams', 'examiner'],
+    ['gams', 'gamschk'],
+    ['gams', 'gurobi'],
+    ['gams', 'guss'],
+    ['gams', 'highs'],
+    ['gams', 'ipopt'],
+    ['gams', 'jams'],
+    ['gams', 'kestrel'],
+    ['gams', 'knitro'],
+    ['gams', 'lindo'],
+    ['gams', 'lindoglobal'],
+    ['gams', 'miles'],
+    ['gams', 'minos'],
+    ['gams', 'mosek'],
+    ['gams', 'mps2gms'],
+    ['gams', 'mpsge'],
+    ['gams', 'msnlp'],
+    ['gams', 'nlpec'],
+    ['gams', 'octeract'],
+    ['gams', 'odh'],
+    ['gams', 'path'],
+    ['gams', 'pathnlp'],
+    ['gams', 'quad'],
+    ['gams', 'sbb'],
+    ['gams', 'scip'],
+    ['gams', 'shot'],
+    ['gams', 'snopt'],
+    ['gams', 'soplex'],
+    ['gams', 'xpress'],
+    ['gekko', 'apopt'],
+    ['gekko', 'bpopt'],
+    ['gekko', 'ipopt'],
+    ['gurobi', 'gurobi'],
+    ['highs', 'highs'],
+    ['insideopt-demo', 'seeker'],
+    ['insideopt', 'seeker'],
+    ['linopy', 'cbc'],
+    ['linopy', 'cplex'],
+    ['linopy', 'glpk'],
+    ['linopy', 'gurobi'],
+    ['linopy', 'highs'],
+    ['linopy', 'xpress'],
+    ['mip', 'cbc'],
+    ['mip', 'cplex'],
+    ['mip', 'glpk'],
+    ['mip', 'gurobi'],
+    ['ortools', 'bop'],
+    ['ortools', 'cbc'],
+    ['ortools', 'clp'],
+    ['ortools', 'cplex-'],
+    ['ortools', 'cplex'],
+    ['ortools', 'glop'],
+    ['ortools', 'glpk-'],
+    ['ortools', 'glpk'],
+    ['ortools', 'gurobi-'],
+    ['ortools', 'gurobi'],
+    ['ortools', 'sat'],
+    ['ortools', 'scip'],
+    ['ortools', 'xpress-'],
+    ['ortools', 'xpress'],
+    ['picos', 'cplex'],
+    ['picos', 'cvxopt'],
+    ['picos', 'ecos'],
+    ['picos', 'glpk'],
+    ['picos', 'gurobi'],
+    ['picos', 'mosek'],
+    ['picos', 'mskfn'],
+    ['picos', 'osqp'],
+    ['picos', 'scip'],
+    ['picos', 'smcp'],
+    ['pulp', 'cbc'],
+    ['pulp', 'choco'],
+    ['pulp', 'coin'],
+    ['pulp', 'coinmp-dll'],
+    ['pulp', 'cplex-py'],
+    ['pulp', 'cplex'],
+    ['pulp', 'glpk'],
+    ['pulp', 'gurobi-cmd'],
+    ['pulp', 'gurobi'],
+    ['pulp', 'highs'],
+    ['pulp', 'mipcl'],
+    ['pulp', 'mosek'],
+    ['pulp', 'pyglpk'],
+    ['pulp', 'scip'],
+    ['pulp', 'xpress-py'],
+    ['pulp', 'xpress'],
+    ['pymprog', 'glpk'],
+    ['pyomo', 'asl'],
+    ['pyomo', 'baron'],
+    ['pyomo', 'cbc'],
+    ['pyomo', 'conopt'],
+    ['pyomo', 'cplex-direct'],
+    ['pyomo', 'cplex-persistent'],
+    ['pyomo', 'cplex'],
+    ['pyomo', 'cyipopt'],
+    ['pyomo', 'gams'],
+    ['pyomo', 'gdpopt.gloa'],
+    ['pyomo', 'gdpopt.lbb'],
+    ['pyomo', 'gdpopt.loa'],
+    ['pyomo', 'gdpopt.ric'],
+    ['pyomo', 'gdpopt'],
+    ['pyomo', 'glpk'],
+    ['pyomo', 'gurobi-direct'],
+    ['pyomo', 'gurobi-persistent'],
+    ['pyomo', 'gurobi'],
+    ['pyomo', 'highs'],
+    ['pyomo', 'ipopt'],
+    ['pyomo', 'mindtpy'],
+    ['pyomo', 'mosek-direct'],
+    ['pyomo', 'mosek-persistent'],
+    ['pyomo', 'mosek'],
+    ['pyomo', 'mpec-minlp'],
+    ['pyomo', 'mpec-nlp'],
+    ['pyomo', 'multistart'],
+    ['pyomo', 'path'],
+    ['pyomo', 'scip'],
+    ['pyomo', 'trustregion'],
+    ['pyomo', 'xpress-direct'],
+    ['pyomo', 'xpress-persistent'],
+    ['pyomo', 'xpress'],
+    ['xpress', 'xpress'],
+]
+
+UNCERTAINTY_ALGORITHMS = [
+    ['rsome-dro', 'copt'],
+    ['rsome-dro', 'cplex'],
+    ['rsome-dro', 'cvxpy'],
+    ['rsome-dro', 'cylp'],
+    ['rsome-dro', 'ecos'],
+    ['rsome-dro', 'gurobi'],
+    ['rsome-dro', 'mosek'],
+    ['rsome-dro', 'ortools'],
+    ['rsome-dro', 'scipy'],
+    ['rsome-ro', 'copt'],
+    ['rsome-ro', 'cplex'],
+    ['rsome-ro', 'cvxpy'],
+    ['rsome-ro', 'cylp'],
+    ['rsome-ro', 'ecos'],
+    ['rsome-ro', 'gurobi'],
+    ['rsome-ro', 'mosek'],
+    ['rsome-ro', 'ortools'],
+    ['rsome-ro', 'scipy'],
+]
+
+CONSTRAINT_ALGORITHMS = [
+    ['cplex-cp', 'cplex'],
+    ['ortools-cp', 'ortools']
+]
+
+MOO_ALGORITHMS = [
+    ['pymoo', 'age-mo-ea-ii'],
+    ['pymoo', 'age-mo-ea'],
+    ['pymoo', 'cta-ea'],
+    ['pymoo', 'd-ns-ga-ii'],
+    ['pymoo', 'mo-ea-d'],
+    ['pymoo', 'ns-ga-ii'],
+    ['pymoo', 'ns-ga-iii'],
+    ['pymoo', 'r-ns-ga-ii'],
+    ['pymoo', 'r-ns-ga-iii'],
+    ['pymoo', 'rv-ea'],
+    ['pymoo', 'sms-ea'],
+    ['pymoo', 'sp-ea-ii'],
+    ['pymoo', 'u-ns-ga-iii'],
+    ['pymultiobjective', 'cta-ea'],
+    ['pymultiobjective', 'ea-d'],
+    ['pymultiobjective', 'ea-fc'],
+    ['pymultiobjective', 'ea-hv'],
+    ['pymultiobjective', 'est-hv'],
+    ['pymultiobjective', 'gr-ea'],
+    ['pymultiobjective', 'modi-pso'],
+    ['pymultiobjective', 'na-ea'],
+    ['pymultiobjective', 'ns-ga-ii'],
+    ['pymultiobjective', 'ns-ga-ii'],
+    ['pymultiobjective', 'ns-ga-iii'],
+    ['pymultiobjective', 'pa-es'],
+    ['pymultiobjective', 'rv-ea'],
+    ['pymultiobjective', 'sm-pso'],
+    ['pymultiobjective', 'sms-ea'],
+    ['pymultiobjective', 'sp-ea-ii'],
+    ['pymultiobjective', 'u-ns-ga-iii'],
+]
+
+WEIGHTING_ALGORITHMS = [
+    ['ahp_method','pydecision'],
+    ['bw_method','pydecision'],
+    ['cilos_method', 'pydecision'],
+    ['critic_method', 'pydecision'],
+    ['entropy_method', 'pydecision'],
+    ['fuzzy_ahp_method','pydecision'],
+    ['fuzzy_bw_method','pydecision'],
+    ['idocriw_method', 'pydecision'],
+    ['lp_method', 'feloopy'],
+    ['merec_method', 'pydecision'],
+    ]
 
-from .classes.tensor_variable import *
-from .classes.tensor_variable_collection import *
-from .classes.multidim_variable import *
-from .classes.multidim_variable_collection import *
-from .classes.event_variable import *
-from .classes.event_variable_collection import *
-from .classes.special_constraint import *
-from .classes.linearization import *
-from .classes.constraint_programming import *
-
-warnings.filterwarnings("ignore")
-
-class ModelObject:
-    pass
-
-class AgentObject:
-    pass
-
-class ConditionalObject:
-    pass
-
-class TensorVariableCollection:
-    pass
-
-class MultidimVariableCollection:
-    pass
-
-class EventVariable:
-    pass
-
-class Model(TensorVariableClass,
-            TensorVariableCollectionClass,
-            MultidimVariableClass,
-            MultidimVariableCollectionClass,
-            EventVariableClass,
-            EventVariableCollectionClass,
-            SpecialConstraintClass,
-            LinearizationClass,
-            ConstraintProgrammingClass):
-    
-    def __init__(self,
-                 solution_method: Literal[
-                     'constraint', 
-                     'convex', 
-                     'exact', 
-                     'heuristic', 
-                     'uncertain',
-                 ],
-                 model_name: str,
-                 interface_name: Literal[
-                     'copt',
-                     'cplex',
-                     'cplex_cp',
-                     'cvxpy',
-                     'cylp',
-                     'feloopy',
-                     'gekko',
-                     'gurobi',
-                     'linopy',
-                     'mealpy',
-                     'mip',
-                     'niapy',
-                     'ortools',
-                     'ortools_cp'
-                     'picos',
-                     'pulp',
-                     'pygad',
-                     'pymoo',
-                     'pymprog',
-                     'pymultiobjective',
-                     'pyomo',
-                     'rsome_dro',
-                     'rsome_ro',
-                     'xpress',
-                 ],
-                 agent: Optional[Union[AgentObject, None]] = None,
-                 scens: Optional[int] = 1,
-                 no_agents: Optional[int] = None,
-                 ) -> None:
+RANKING_ALGORITHMS = [
+    ['aras_method', 'pydecision'],
+    ['borda_method', 'pydecision'],
+    ['cocoso_method', 'pydecision'],
+    ['codas_method', 'pydecision'],
+    ['copeland_method', 'pydecision'],
+    ['copras_method', 'pydecision'],
+    ['cradis_method', 'pydecision'],
+    ['edas_method', 'pydecision'],
+    ['fuzzy_aras_method', 'pydecision'],
+    ['fuzzy_copras_method', 'pydecision'],
+    ['fuzzy_edas_method', 'pydecision'],
+    ['fuzzy_moora_method', 'pydecision'],
+    ['fuzzy_ocra_method', 'pydecision'],
+    ['fuzzy_topsis_method', 'pydecision'],
+    ['fuzzy_vikor_method', 'pydecision'],
+    ['fuzzy_waspas_method', 'pydecision'],
+    ['gra_method', 'pydecision'],
+    ['la_method', 'feloopy'],
+    ['mabac_method', 'pydecision'],
+    ['macbeth_method', 'pydecision'],
+    ['mairca_method', 'pydecision'],
+    ['marcos_method', 'pydecision'],
+    ['maut_method', 'pydecision'],
+    ['moora_method', 'pydecision'],
+    ['moosra_method', 'pydecision'],
+    ['multimoora_method', 'pydecision'],
+    ['ocra_method', 'pydecision'],
+    ['oreste_method', 'pydecision'],
+    ['piv_method', 'pydecision'],
+    ['promethee_ii', 'pydecision'],
+    ['promethee_iv', 'pydecision'],
+    ['promethee_vi', 'pydecision'],
+    ['psi_method', 'pydecision'],
+    ['regime_method', 'pydecision'],
+    ['rov_method', 'pydecision'],
+    ['saw_method', 'pydecision'],
+    ['smart_method', 'pydecision'],
+    ['spotis_method', 'pydecision'],
+    ['todim_method', 'pydecision'],
+    ['topsis_method', 'pydecision'],
+    ['vikor_method', 'pydecision'],
+    ['waspas_method', 'pydecision'],
+    ]
+
+SPECIAL_ALGORITHMS = [
+    ['cwdea_method', 'feloopy'],
+    ['dematel_method', 'pydecision'],
+    ['electre_i_s', 'pydecision'],
+    ['electre_i_v', 'pydecision'],
+    ['electre_i', 'pydecision'],
+    ['electre_ii', 'pydecision'],
+    ['electre_iii', 'pydecision'],
+    ['electre_iv', 'pydecision'],
+    ['electre_tri_b', 'pydecision'],
+    ['fuzzy_dematel_method', 'pydecision'],
+    ['promethee_gaia', 'pydecision'],
+    ['promethee_i', 'pydecision'],
+    ['promethee_iii', 'pydecision'],
+    ['promethee_v', 'pydecision'],
+    ['wings_method', 'pydecision'],
+]
+
+from .algorithms import *
+from .classes import *
+from .helpers import *
+from .operators import *
+
+class model(
+    TensorVariableClass,
+    TensorVariableCollectionClass,
+    MultidimVariableClass,
+    MultidimVariableCollectionClass,
+    EventVariableClass,
+    EventVariableCollectionClass,
+    SpecialConstraintClass,
+    NormalConstraintClass,
+    LinearizationClass,
+    ConstraintProgrammingClass,
+    ):
+    
+    def __init__(
+        self,
+        name: str = 'model_name',
+        method: Literal['constraint', 'convex', 'exact', 'heuristic', 'uncertain'] = 'exact',
+        interface: Literal['copt','cplex','cplex_cp','cvxpy','cylp','feloopy','gekko','gurobi','linopy','mealpy','mip','niapy','ortools','ortools_cp','picos','pulp','pygad','pymoo','pymprog','pymultiobjective','pyomo','rsome_dro','rsome_ro','xpress','insideopt','insideopt-demo', 'gams','highs'] = 'pulp',
+        agent: Optional[Any] = None,
+        no_scenarios: Optional[int] = None,
+        no_agents: Optional[int] = None,
+        scenario_ids: Optional[list] = None,
+        constraint_ids: Optional[list] = None,
+        validate: bool = True,
+        ):
+        
         """
         Creates and initializes the mathematical modeling environment.
 
         Parameters
         ----------
-        solution_method : Literal['exact', 'heuristic', 'constraint', 'convex', 'uncertain']
-            The desired solution method for optimization.
-        model_name : str
-            The name of the optimization model.
-        interface_name : Literal[
-            'copt', 'cplex', 'cplex_cp', 'cvxpy', 'cylp', 'feloopy', 'gekko', 'gurobi', 'linopy',
-            'mealpy', 'mip', 'niapy', 'ortools', 'ortools_cp', 'picos', 'pulp', 'pygad', 'pymoo',
-            'pymprog', 'pymultiobjective', 'pyomo', 'rsome_dro', 'rsome_ro', 'xpress',
-        ]
-            The selected solver interface for optimization.
-        agent : Optional[Union[AgentObject, None]] (default=None)
-            An optional search agent object. If not provided, the optimization will be agentless.
-        scens : Optional[int] (default=1)
-            The number of scenarios for the optimization problem. Defaults to 1 if not specified.
-        no_agents : Optional[int] (default=None)
-            The number of search agents to use in the optimization. If not specified, the default behavior will be applied.
-        """
-        
-        if solution_method not in {'exact', 'heuristic', 'constraint', 'convex', 'uncertain'}:
-            raise ValueError("Invalid solution method. Please choose from 'exact', 'heuristic', 'constraint', 'convex', or 'uncertain'.")
-        
-        if interface_name not in {'copt', 'cplex', 'cplex_cp', 'cvxpy', 'cylp', 'feloopy', 'gekko', 'gurobi', 'linopy',
-                                  'mealpy', 'mip', 'niapy', 'ortools', 'ortools_cp', 'picos', 'pulp', 'pygad', 'pymoo',
-                                  'pymprog', 'pymultiobjective', 'pyomo', 'rsome_dro', 'rsome_ro', 'xpress'}:
-            raise ValueError("Invalid solver interface. Please choose from the provided options.")
-        
-        if not isinstance(scens, int) or scens < 1:
-            raise ValueError("The number of scenarios (scens) must be a positive integer (>=1).")
-        
-        if no_agents is not None and (not isinstance(no_agents, int) or no_agents < 1):
-            raise ValueError("The number of search agents (no_agents) must be a positive integer (>=1) or None.")
-
+        name
+            Name of the mathematical model.
+        method
+            Desired solution method.
+        interface
+            Desired solver interface.
+        agent
+            Search agent in heuristic optimization.
+        no_scenarios
+            Number of scenarios in uncertainty handling.
+        no_agents
+            Number of search agents in heuristic optimization.
+        scenario_ids
+            Indices of scenarios in uncertainty handling.
+        constraint_ids
+            Indices of constraints to be considered.
+        """
+        
+        if validate: 
+
+            validate_string(
+                label="method", 
+                list_of_allowed_values=['constraint', 'convex', 'exact', 'heuristic', 'uncertain'], 
+                input_string=method,
+                required=True)
+
+            validate_string(
+                label="interface", 
+                list_of_allowed_values=['copt','cplex','cplex_cp','cvxpy','cylp','feloopy','gekko','gurobi','linopy','mealpy','mip','niapy','ortools','ortools_cp','picos','pulp','pygad','pymoo','pymprog','pymultiobjective','pyomo','rsome_dro','rsome_ro','xpress','insideopt','insideopt-demo', 'gams','highs'], 
+                input_string=interface,
+                required=True)
+            
+            validate_integer(
+                label="no_scenarios", 
+                min_value=1, 
+                max_value=None, 
+                input_integer=no_scenarios, 
+                required=False)
+
+            validate_integer(
+                label="no_agents", 
+                min_value=1, 
+                max_value=None, 
+                input_integer=no_agents, 
+                required=False)
+            
+            validate_existence(
+                label="agent", 
+                input_value=agent, 
+                condition=True if method=="heuristic" else False)
+                           
+        self.name = name
+        self.method = method
+        self.interface = interface
+        self.agent = agent
+        self.no_scenarios = no_scenarios
         self.no_agents = no_agents
+        self.scenario_ids = scenario_ids
+        self.constraint_ids = constraint_ids
 
-        if solution_method == 'constraint':
-            self.solution_method_was = 'constraint'
-            solution_method = 'exact'
-
-        elif solution_method == 'convex':
-            self.solution_method_was = 'convex'
-            solution_method = 'exact'
-
-        elif solution_method == 'uncertain':
-            self.solution_method_was = 'uncertain'
-            solution_method = 'exact'
-
+        if self.method in ["constraint", "convex", "uncertain"]:
+            self.method_was = self.method
+            self.method = "exact"
         else:
-            self.solution_method_was=None
+            self.method_was = None
 
         self.features = {
-            'solution_method': solution_method,
-            'model_name': model_name,
-            'interface_name': interface_name,
+            'solution_method': self.method,
+            'model_name': self.name,
+            'interface_name': self.interface,
+            'no_scenarios': self.no_scenarios,
+            'no_agents': self.no_agents,
+            'scenario_ids': self.scenario_ids,
+            'constraint_ids': self.constraint_ids,
             'solver_name': None,
             'constraints': [],
             'constraint_labels': [],
             'objectives': [],
             'objective_labels': [],
             'directions': [],
             'positive_variable_counter': [0, 0],
@@ -177,143 +737,83 @@
             'event_variable_counter': [0, 0],
             'sequential_variable_counter': [0,0],
             'dependent_variable_counter': [0,0],
             'total_variable_counter': [0, 0],
             'objective_counter': [0, 0],
             'constraint_counter': [0, 0],
             'objective_being_optimized': 0,
-            'scens': scens,
+            'solver_options': {},
         }
 
-        if solution_method == 'heuristic':
+        if self.method == 'exact':
+
+            from .generators import model_generator
+            self.model = model_generator.generate_model(self.features)
+                   
+                   
+            self.features.update(
+                {
+                'model_object': self.model,
+                'variables': defaultdict(),
+                'dimensions': defaultdict(),
+                }
+            )
             
-            self.agent = agent
+            self.link_to_interface = self.lti = self._ = self.model
+                    
+        if self.method == 'heuristic':
             
             self.features.update(
                 {
                 'agent_status': self.agent[0],
                 'variable_spread': self.agent[2] if self.agent[0] != 'idle' else dict(),
                 'variable_type': dict() if self.agent[0] == 'idle' else None,
                 'variable_bound': dict() if self.agent[0] == 'idle' else None,
                 'variable_dim': dict() if self.agent[0] == 'idle' else None,
                 'pop_size': 1 if self.agent[0] == 'idle' else len(self.agent[1]),
                 'penalty_coefficient': 0 if self.agent[0] == 'idle' else self.agent[3],
-                'vectorized': None,
+                'vectorized': self.interface in ['feloopy', 'pymoo'],
                 }
             )
-
-            self.features['vectorized'] = interface_name in ['feloopy', 'pymoo']
-
             if self.agent[0] != 'idle':
-
                 self.agent = self.agent[1].copy()
-
-            if self.features['agent_status']!='idle':
-                self.access = True
-                
-            else:
-                self.access = False
-
-        if solution_method == 'exact':
-
-            self.mainvars = defaultdict()
-            self.maindims = defaultdict()
-
-            from .generators import model_generator
-            self.model = model_generator.generate_model(self.features)
-            self.sm = self.link_to_interface = self.lti = self.model
-            
-        # Alias methods
-        
-        # Binary variable aliases
+ 
         self.binary_variable = self.binary = self.bool = self.add_bool = self.add_binary = self.add_binary_variable = self.boolean_variable = self.add_boolean_variable = self.bvar
-        
-        # Positive variable aliases
         self.positive_variable = self.positive = self.add_positive = self.add_positive_variable = self.pvar
-        
-        # Integer variable aliases
         self.integer_variable = self.integer = self.add_integer = self.add_integer_variable = self.ivar
-        
-        # Free variable aliases
         self.free_variable = self.free = self.float = self.add_free = self.add_float = self.real = self.add_real = self.add_free_variable = self.fvar
-        
-        # Sequential variable aliases
         self.sequential_variable = self.sequence = self.sequential = self.add_sequence = self.add_sequential = self.add_sequential_variable = self.permutation_variable = self.add_permutation_variable = self.svar
-        
-        # Positive tensor variable aliases
         self.positive_tensor_variable = self.positive_tensor = self.add_positive_tensor = self.add_positive_tensor_variable = self.ptvar
-        
-        # Binary tensor variable aliases
         self.binary_tensor_variable = self.binary_tensor = self.add_binary_tensor = self.add_binary_tensor_variable = self.add_boolean_tensor_variable = self.boolean_tensor_variable = self.btvar
-        
-        # Integer tensor variable aliases
         self.integer_tensor_variable = self.integer_tensor = self.add_integer_tensor = self.add_integer_tensor_variable = self.itvar
-        
-        # Free tensor variable aliases
         self.free_tensor_variable = self.free_tensor = self.float_tensor = self.add_free_tensor = self.add_float_tensor = self.add_free_tensor_variable = self.ftvar
-        
-        # Random variable aliases
         self.random_variable = self.add_random_variable = self.rvar
-        
-        # Random tensor variable aliases
         self.random_tensor_variable = self.add_random_tensor_variable = self.rtvar
-        
-        # Dependent variable aliases
         self.dependent_variable = self.array = self.add_array = self.add_dependent_variable = self.dvar
-        
-        # Objective aliases
         self.objective = self.reward = self.hypothesis = self.fitness = self.goal = self.add_objective = self.loss = self.gain = self.obj
-        
-        # Constraint aliases
         self.constraint = self.equation = self.add_constraint = self.add_equation = self.st = self.subject_to = self.cb = self.computed_by = self.penalize = self.pen = self.eq = self.con
-        
-        # Solve aliases
         self.solve = self.implement = self.run = self.optimize = self.sol
-        
-        # Query aliases
         self.get_obj = self.get_objective
         self.get_stat = self.get_status
         self.get_tensor = self.get_numpy_var
         self.get_var = self.value = self.get = self.get_variable
 
-    def __getitem__(self, agent: AgentObject) -> ConditionalObject:
-        """
-        Retrieve the required features of the model object.
-
-        Parameters
-        ----------
-        agent : AgentObject
-            The search agent object used to determine the feature retrieval method.
-
-        Returns
-        -------
-        ConditionalObject
-            The requested features or the model object itself based on the agent's status.
-
-        Notes
-        -----
-        - If the agent's status is 'idle', the method returns the model object.
-        - If the agent's status is 'feasibility_check', the method invokes `_feasibility_check()` and returns its result.
-        - For other statuses, the method calls `_get_result(vectorized, interface_name)` and returns the result.
-        """
-
+    def __getitem__(self, agent):
         agent_status = self.features['agent_status']
         vectorized = self.features['vectorized']
         interface_name = self.features['interface_name']
-
         if agent_status == 'idle':
             return self
-        
         elif agent_status == 'feasibility_check':
             return self._feasibility_check()
-        
         else:
             return self._get_result(vectorized, interface_name)
 
     def _feasibility_check(self) -> str:
+        
         """
         Perform a feasibility check based on the model's features.
 
         Returns
         -------
         str
             The feasibility status:
@@ -323,15 +823,18 @@
         """
         
         if self.features['penalty_coefficient'] == 0:
             return 'feasible (unconstrained)'
         else:
             return 'infeasible (constrained)' if self.penalty > 0 else 'feasible (constrained)'
 
-    def _get_result(self, vectorized: bool, interface_name: str) -> ConditionalObject:
+    def fix_ifneeded(self, dims):
+        return fix_dims(dims)
+    
+    def _get_result(self, vectorized: bool, interface_name: str):
         """
         Retrieve the optimization result based on the specified parameters.
 
         Parameters
         ----------
         vectorized : bool
             A boolean indicating whether the result should be vectorized.
@@ -347,30 +850,91 @@
             - If vectorized is False, returns the response.
         """
         
         if vectorized:
             return self.agent if interface_name == 'feloopy' else self.sing_result
         else:
             return self.response
+
+    def vstart(self, variable, input_value):
+        
+        from .generators import init_generator
+        init_generator.generate_init(self.features,variable,input_value,fix=False)
+         
+    def tstart(self, name, input_tensor):
+        
+        input_tensor = np.array(input_tensor)
+        
+        from .generators import init_generator
+        for i,j in self.features['variables'].keys():
+            if j==name:
+                if self.features['dimensions'][j]==0:
+                    init_generator.generate_init(self.features,self.features['variables'][(i,j)],input_tensor,fix=False)
+                    
+                elif len(self.features['dimensions'][j])==1:
+                
+                    for k in fix_dims(self.features['dimensions'][j])[0]:
+                        init_generator.generate_init(self.features,self.features['variables'][(i,j)][k],input_tensor[k],fix=False)
+                else:
+                    for k in it.product(*tuple(fix_dims(self.features['dimensions'][j]))):
+                        init_generator.generate_init(self.features,self.features['variables'][(i,j)][k],input_tensor[k],fix=False)
+                            
+    def vfix(self, variables, values):
+        
+        from .generators import init_generator
+        init_generator.generate_init(self.features,variables,values,fix=True)
+
+    def tfix(self, name, input_tensor):
+        
+        input_tensor = np.array(input_tensor)
         
+        from .generators import init_generator
+        for i,j in self.features['variables'].keys():
+            if j==name:
+                if self.features['dimensions'][j]==0:
+                    init_generator.generate_init(self.features,self.features['variables'][(i,j)],input_tensor,fix=True)
+                    
+                elif len(self.features['dimensions'][j])==1:
+                
+                    for k in fix_dims(self.features['dimensions'][j])[0]:
+                        init_generator.generate_init(self.features,self.features['variables'][(i,j)][k],input_tensor[k],fix=True)
+                else:
+                    for k in it.product(*tuple(fix_dims(self.features['dimensions'][j]))):
+                        init_generator.generate_init(self.features,self.features['variables'][(i,j)][k],input_tensor[k],fix=True)
+                          
     def obj(self, expression=0, direction=None, label=None):
+            
             """
             Defines the objective function for the optimization problem.
 
             Parameters
             ----------
             expression : formula
                 The terms of the objective function.
             direction : str, optional
                 The direction for optimizing this objective ("min" or "max").
             label : str, optional
                 The label for this objective function.
 
             """
             
+            if self.features['interface_name'] == 'gams':
+                
+                try:
+                    self.features['of'].append(self.features['of'][-1] + 1)
+                except:
+                    self.features['of'] = [0]
+
+                z = self.fvar(f"of{self.features['of'][-1]}")
+                self.features['objective_variable'] = z
+                
+                expression = expression == self.features['objective_variable']
+                    
+                
+                
             if self.features['solution_method'] == 'exact' or (self.features['solution_method'] == 'heuristic' and self.features['agent_status'] == 'idle'):
 
                 self.features['directions'].append(direction)
                 self.features['objectives'].append(expression)
                 self.features['objective_labels'].append(label)
 
                 self.features['objective_counter'][0] += 1
@@ -378,61 +942,15 @@
 
             elif self.features['solution_method'] == 'heuristic' and self.features['agent_status'] != 'idle':
 
                 self.features['directions'].append(direction)
                 self.features['objectives'].append(expression)
                 self.features['objective_counter'][0] += 1
 
-    def con(self, expression, label=None):
-        """
-        Constraint Definition
-        ~~~~~~~~~~~~~~~~~~~~~
-        To define a constraint.
-
-        Args:
-            expression (formula): what are the terms of this constraint?
-            label (str, optional): what is the label of this constraint?. Defaults to None.
-        """
-
-        match self.features['solution_method']:
-
-            case 'exact':
-
-                self.features['constraint_labels'].append(label)
-                self.features['constraint_counter'][0] = len(
-                    set(self.features['constraint_labels']))
-                self.features['constraints'].append(expression)
-                self.features['constraint_counter'][1] = len(
-                    self.features['constraints'])
-
-            case 'heuristic':
-
-                if self.features['agent_status'] == 'idle':
-
-                    self.features['constraint_labels'].append(label)
-
-                    self.features['constraint_counter'][0] = len(
-                        set(self.features['constraint_labels']))
-
-                    self.features['constraints'].append(expression)
-
-                    self.features['constraint_counter'][1] = len(
-                        self.features['constraints'])
-
-                else:
-
-                    if self.features['vectorized']:
-
-                        self.features['constraints'].append(
-                            np.reshape(expression, [np.shape(self.agent)[0], 1]))
-
-                    else:
-                        self.features['constraints'].append(expression)
-
-    def sol(self, directions=None, solver_name=None, solver_options=dict(), obj_id=0, email=None, debug=False, time_limit=None, cpu_threads=None, absolute_gap=None, relative_gap=None, show_log=False, save_log=False, save_model=False, max_iterations=None, obj_operators=[]):
+    def sol(self, directions=None, solver=None, solver_options=dict(), obj_id=0, email=None, debug=False, time_limit=None, cpu_threads=None, absolute_gap=None, relative_gap=None, show_log=False, save_log=False, save_model=False, max_iterations=None, obj_operators=[]):
         """
         Solve Command Definition
         ~~~~~~~~~~~~~~~~~~~~~~~~
         To define solver and its settings to solve the problem.
 
         Args:
             directions (list, optional): please set the optimization directions of the objectives, if not provided before. Defaults to None.
@@ -451,27 +969,27 @@
             if self.features['interface_name'] in ['mealpy' , 'feloopy', 'niapy', 'pygad']:
                 solver_options['pop_size'] = self.no_agents
 
         if len(self.features['objectives']) !=0 and len(directions)!=len(self.features['objectives']):
             raise MultiObjectivityError("The number of directions and the provided objectives do not match.")
 
         self.features['objective_being_optimized'] = obj_id
-        self.features['solver_options'] = solver_options
+        self.features['solver_options'].update(solver_options)
         self.features['debug_mode'] = debug
         self.features['time_limit'] = time_limit
         self.features['thread_count'] = cpu_threads
         self.features['absolute_gap'] = absolute_gap
         self.features['relative_gap'] = relative_gap
         self.features['log'] = show_log
         self.features['write_model_file'] = save_model
         self.features['save_solver_log'] = save_log
         self.features['email_address'] = email
         self.features['max_iterations'] = max_iterations
         self.features['obj_operators'] = obj_operators
-        self.features['solver_name'] = solver_name
+        self.features['solver_name'] = solver
 
         try:
             if type(obj_id) != str and directions != None:
 
                 if self.features['directions'][obj_id] == None:
 
                     self.features['directions'][obj_id] = directions[obj_id]
@@ -533,17 +1051,17 @@
             case 'heuristic':
 
                 if self.features['agent_status'] == 'idle':
 
                     "Do nothing"
 
                 else:
-
+                    
                     if self.features['vectorized']:
-
+                        
                         if self.features['interface_name']=='feloopy':
 
                             self.penalty = np.zeros(np.shape(self.agent)[0])
 
                             if self.features['penalty_coefficient'] != 0 and len(self.features['constraints']) == 1:
 
                                 self.features['constraints'][0] = np.reshape(
@@ -631,19 +1149,18 @@
                                         self.sing_result.append(self.features['objectives'][i] - self.features['penalty_coefficient'] * (self.penalty)**2)
 
                                     if directions[i] == 'min':
                                         self.sing_result.append(self.features['objectives'][i] + self.features['penalty_coefficient'] * (self.penalty)**2)
                     else:
 
                         self.penalty = 0
-
+                        
                         if len(self.features['constraints']) >= 1:
-
-                            self.penalty = np.amax(
-                                np.array([0]+self.features['constraints'], dtype=object))
+                            
+                            self.penalty = np.amax(np.array([0]+self.features['constraints'], dtype=object))
 
                         if type(obj_id) != str:
 
                             if directions[obj_id] == 'max':
                                 self.response = self.features['objectives'][obj_id] - \
                                     self.features['penalty_coefficient'] * \
                                     (self.penalty-0)**2
@@ -668,14 +1185,16 @@
                                         (self.penalty)**2
 
                                 if directions[i] == 'min':
 
                                     self.response[i] = self.features['objectives'][i] + \
                                         self.features['penalty_coefficient'] * \
                                         (self.penalty)**2
+                        
+                        
 
     def healthy(self):
         try:
             status = self.get_status().lower()
             return ('optimal' in status or 'feasible' in status) and 'infeasible' not in status
         except:
             try:
@@ -788,37 +1307,94 @@
         
             from rsome import sumsqr
             return sumsqr(expr_or_1D_array_of_variables)
     
     def state_function(self):
         
         """
-
         Creates and returns a state function.
-
         """
 
         return self.model.state_function()
 
-    def report(self, all_metrics: bool = False, feloopy_info: bool = True, math_info: bool = False, sys_info: bool = False, model_info: bool = True, sol_info: bool = True, obj_values: bool = True, dec_info: bool = True, metric_info: bool = True, ideal_pareto: Optional[np.ndarray] = [], ideal_point: Optional[np.array] = [], show_tensors = False, show_detailed_tensors=False, save=None):
+    def append_full_report(self, filename="result.txt", dir='./results/texts/', **kwargs):
+        path = dir + filename
+        if not os.path.exists(dir):
+            os.makedirs(dir)
+        if not os.path.isfile(path):
+            open(path, 'w').close()
+        with open(path, 'a', encoding='utf-8') as f:
+            with contextlib.redirect_stdout(f):
+                self.full_report(**kwargs)
+                
+    def append_report(self, filename="result.txt", dir='./results/texts/', **kwargs):
+        path = dir + filename
+        if not os.path.exists(dir):
+            os.makedirs(dir)
+        if not os.path.isfile(path):
+            open(path, 'w').close()
+        with open(path, 'a', encoding='utf-8') as f:
+            with contextlib.redirect_stdout(f):
+                self.report(**kwargs)
+                               
+    def write_full_report(self, filename="result.txt", dir='./results/texts/', **kwargs):
+        path = dir + filename
+        if not os.path.exists(dir):
+            os.makedirs(dir)
+        if not os.path.isfile(path):
+            open(path, 'w').close()
+        with open(path, 'w', encoding='utf-8') as f:
+            with contextlib.redirect_stdout(f):
+                self.full_report(**kwargs)
+
+    def write_report(self, filename="result.txt", dir='./results/texts/', **kwargs):
+        path = dir + filename
+        if not os.path.exists(dir):
+            os.makedirs(dir)
+        if not os.path.isfile(path):
+            open(path, 'w').close()
+        with open(path, 'w', encoding='utf-8') as f:
+            with contextlib.redirect_stdout(f):
+                self.report(**kwargs)
+            
+    def full_report(self,show_tensors=False, detailed=False):
+        
+        self.report(all_metrics = True, 
+                    feloopy_info = True, 
+                    extra_info = True, 
+                    math_info = True, 
+                    sys_info = True, 
+                    model_info = True, 
+                    sol_info = True, 
+                    obj_values = True, 
+                    dec_info = True, 
+                    metric_info = True, 
+                    show_tensors=show_tensors, 
+                    show_detailed_tensors=detailed)
+            
+    def clean_report(self):
 
+        command = "cls" if os.name == "nt" else "clear"
+        os.system(command)
+        self.report()
+         
+    def report(self, all_metrics: bool = False, feloopy_info: bool = True, extra_info: bool = False, math_info: bool = False, sys_info: bool = False, model_info: bool = True, sol_info: bool = True, obj_values: bool = True, dec_info: bool = True, metric_info: bool = True, ideal_pareto: Optional[np.ndarray] = [], ideal_point: Optional[np.array] = [], show_tensors = False, show_detailed_tensors=False, save=None):
 
         if not self.healthy():
             print()
             print()
             print('WARNING: Model is not healthy!')
             print()
             print()
-            
-            
+             
         self.interface_name = self.features['interface_name']
-        if self.solution_method_was==None:
+        if self.method_was==None:
             self.solution_method = self.features['solution_method']
         else:
-            self.solution_method = self.solution_method_was
+            self.solution_method = self.method_was
         self.model_name = self.features['model_name']
         self.solver_name = self.features['solver_name']
         self.model_constraints = self.features['constraints']
         self.model_objectives = self.features['objectives']
         self.objectives_directions = self.features['directions']
         self.pos_var_counter = self.features['positive_variable_counter']
         self.bin_var_counter = self.features['binary_variable_counter']
@@ -835,24 +1411,24 @@
 
         status = self.get_status()
         hour, min, sec = calculate_time_difference(length=self.get_time())
 
         if len(str(status)) == 0:
             status = ['infeasible (constrained)']
 
-        box_width = 80
+        box_width = 90
         vspace()
 
         if feloopy_info:
             
             import datetime
             now = datetime.datetime.now()
             date_str = now.strftime("Date: %Y-%m-%d")
             time_str = now.strftime("Time: %H:%M:%S")
-            tline_text("FelooPy v0.2.8")
+            tline_text("FelooPy v0.2.9")
             empty_line()
             two_column(date_str, time_str)
             two_column(f"Interface: {self.interface_name}", f"Solver: {self.solver_name}")
             empty_line()
             bline()
 
         if sys_info:
@@ -903,15 +1479,15 @@
                 ("Constraint       ", self.con_counter[0], self.con_counter[1]) ])
             empty_line()
             bline()
 
         if math_info:
             try:
                 import textwrap
-                tline_text('Math', box_width=80)
+                tline_text('Math', box_width=90)
                 empty_line()
                 obdirs = 0
                 for objective in self.features['objectives']:
                     wrapped_objective = textwrap.fill(str(objective), width=80)
                     boxed(str(f"obj: {self.features['directions'][obdirs]} {wrapped_objective}"))
                     obdirs += 1
                 left_align('s.t.')
@@ -980,97 +1556,155 @@
             try:
                 self.decision_information_print(status, show_tensors, show_detailed_tensors)
             except:
                 ""
             empty_line()
             bline()
 
+        if extra_info:
+            
+            tline_text("Extra")
+            empty_line()
+            try:
+                left_align("Slack:")
+                for i in self.features['constraint_labels']:
+                    left_align(str(i) + " = " + str(self.get_slack(i)))
+                empty_line()
+            except:
+                pass
+            try:
+                left_align("Dual:")
+                for i in self.features['constraint_labels']:
+                    left_align(str(i) + " = " + str(self.get_dual(i)))
+                empty_line()
+            except:
+                pass
+            bline()
+            
         if save is not None:
             sys.stdout.close()
             sys.stdout = stdout_origin
 
-    def get_numpy_var(self, var_name):
+    def get_numpy_var(self, var_name, dual=False, slack=False, reduced_cost=False):
 
-        for i,j in self.mainvars.keys():
-            if j==var_name:
-                if self.maindims[j]==0:
-                    output = self.get(self.mainvars[(i,j)])
-                elif len(self.maindims[j])==1:
-                    output = np.zeros(shape=len(fix_dims(self.maindims[j])[0]))
-                    for k in fix_dims(self.maindims[j])[0]:
-                        try:
-                            output[k] = self.get(self.mainvars[(i,j)][k])
-                        except:
-                            output[k] = self.get(self.mainvars[(i,j)])[k]
-                else:
-                    output = np.zeros(shape=tuple([len(dim) for dim in fix_dims(self.maindims[j])]))
-                    for k in it.product(*tuple(fix_dims(self.maindims[j]))):
-                        try:
-                            output[k] = self.get(self.mainvars[(i,j)][k])
-                        except:
-                            output[k] =  self.get(self.mainvars[(i,j)])[k]
+        if not dual and not slack:
+            for i,j in self.features['variables'].keys():
+                if j==var_name:
+                    if self.features['dimensions'][j]==0:
+                        output = self.get(self.features['variables'][(i,j)])
+                    elif len(self.features['dimensions'][j])==1:
+                        output = np.zeros(shape=len(fix_dims(self.features['dimensions'][j])[0]))
+                        for k in fix_dims(self.features['dimensions'][j])[0]:
+                            try:
+                                output[k] = self.get(self.features['variables'][(i,j)][k])
+                            except:
+                                output[k] = self.get(self.features['variables'][(i,j)])[k]
+                    else:
+                        output = np.zeros(shape=tuple([len(dim) for dim in fix_dims(self.features['dimensions'][j])]))
+                        for k in it.product(*tuple(fix_dims(self.features['dimensions'][j]))):
+                            try:
+                                output[k] = self.get(self.features['variables'][(i,j)][k])
+                            except:
+                                output[k] =  self.get(self.features['variables'][(i,j)])[k]
+        
+        if reduced_cost:
+            
+    
+            for i,j in self.features['variables'].keys():
+                if j==var_name:
+                    if self.features['dimensions'][j]==0:
+                        output = self.get_rc(self.features['variables'][(i,j)])
+                    elif len(self.features['dimensions'][j])==1:
+                        output = np.zeros(shape=len(fix_dims(self.features['dimensions'][j])[0]))
+                        for k in fix_dims(self.features['dimensions'][j])[0]:
+                            try:
+                                output[k] = self.get_rc(self.features['variables'][(i,j)][k])
+                            except:
+                                output[k] = self.get_rc(self.features['variables'][(i,j)])[k]
+                    else:
+                        output = np.zeros(shape=tuple([len(dim) for dim in fix_dims(self.features['dimensions'][j])]))
+                        for k in it.product(*tuple(fix_dims(self.features['dimensions'][j]))):
+                            try:
+                                output[k] = self.get_rc(self.features['variables'][(i,j)][k])
+                            except:
+                                output[k] =  self.get_rc(self.features['variables'][(i,j)])[k]            
+        if dual:
+            
+            output = []
+            for i in self.features['constraint_labels']:
+                if var_name in i:
+                    output.append(self.get_dual(i))
+            output = np.array(output)
+        
+        if slack:
+
+            output = []
+            for i in self.features['constraint_labels']:
+                if var_name in i:
+                    output.append(self.get_slack(i))
+            output = np.array(output)
+                        
         return output
 
-    def decision_information_print(self,status, show_tensors, show_detailed_tensors, box_width=80):
+    def decision_information_print(self,status, show_tensors, show_detailed_tensors, box_width=88):
         
         if show_detailed_tensors: show_tensors=True
         
         if not show_tensors:
 
-            for i,j in self.mainvars.keys():
+            for i,j in self.features['variables'].keys():
 
                 if i!='evar':
 
-                    if self.maindims[j] == 0:
+                    if self.features['dimensions'][j] == 0:
 
-                        if self.get(self.mainvars[(i,j)]) not in [0, None]:
+                        if self.get(self.features['variables'][(i,j)]) not in [0, None]:
+                            print(f"│ {j} =", self.get(self.features['variables'][(i,j)]), " "* (box_width-(len(f"│ {j} =") + len(str(self.get(self.features['variables'][(i,j)]))))-1) + "│")
 
-                            print(f"│ {j} =", self.get(self.mainvars[(i,j)]), " "* (box_width-(len(f"│ {j} =") + len(str(self.get(self.mainvars[(i,j)]))))-1) + "│")
-
-                    elif len(self.maindims[j])==1:
+                    elif len(self.features['dimensions'][j])==1:
                         try:
-                            for k in fix_dims(self.maindims[j])[0]:
-                                if self.get(self.mainvars[(i,j)][k]) not in [0, None]:
-                                    print(f"│ {j}[{k}] =", self.get(self.mainvars[(i,j)][k]), " "* (box_width-(len(f"│ {j}[{k}] =") + len(str(self.get(self.mainvars[(i,j)][k])))) - 1) + "│")
+                            for k in fix_dims(self.features['dimensions'][j])[0]:
+                                if self.get(self.features['variables'][(i,j)][k]) not in [0, None]:
+                                    print(f"│ {j}[{k}] =", self.get(self.features['variables'][(i,j)][k]), " "* (box_width-(len(f"│ {j}[{k}] =") + len(str(self.get(self.features['variables'][(i,j)][k])))) - 1) + "│")
                         except:
-                            for k in fix_dims(self.maindims[j])[0]:
-                                if self.get(self.mainvars[(i,j)])[k] not in [0, None]:
-                                    print(f"│ {j}[{k}] =", self.get(self.mainvars[(i,j)])[k], " "* (box_width-(len(f"│ {j}[{k}] =") + len(str(self.get(self.mainvars[(i,j)])[k]))) - 1) + "│")
+                            for k in fix_dims(self.features['dimensions'][j])[0]:
+                                if self.get(self.features['variables'][(i,j)])[k] not in [0, None]:
+                                    print(f"│ {j}[{k}] =", self.get(self.features['variables'][(i,j)])[k], " "* (box_width-(len(f"│ {j}[{k}] =") + len(str(self.get(self.features['variables'][(i,j)])[k]))) - 1) + "│")
                     else:
                         try:
-                            for k in it.product(*tuple(fix_dims(self.maindims[j]))):
-                                if self.get(self.mainvars[(i,j)][k]) not in [0, None]:
-                                    print(f"│ {j}[{k}] =".replace("(", "").replace(")", ""), self.get(self.mainvars[(i,j)][k]), " "* (box_width-(len(f"│ {j}[{k}] =".replace("(", "").replace(")", "")) + len(str(self.get(self.mainvars[(i,j)][k])))) - 1) + "│")
+                            for k in it.product(*tuple(fix_dims(self.features['dimensions'][j]))):
+                                if self.get(self.features['variables'][(i,j)][k]) not in [0, None]:
+                                    print(f"│ {j}[{k}] =".replace("(", "").replace(")", ""), self.get(self.features['variables'][(i,j)][k]), " "* (box_width-(len(f"│ {j}[{k}] =".replace("(", "").replace(")", "")) + len(str(self.get(self.features['variables'][(i,j)][k])))) - 1) + "│")
                         except:
-                            for k in it.product(*tuple(fix_dims(self.maindims[j]))):
-                                if self.get(self.mainvars[(i,j)])[k] not in [0, None]:
-                                    print(f"│ {j}[{k}] =".replace("(", "").replace(")", ""), self.get(self.mainvars[(i,j)])[k], " "* (box_width-(len(f"│ {j}[{k}] =".replace("(", "").replace(")", "")) + len(str(self.get(self.mainvars[(i,j)])[k]))) - 1) + "│")
+                            for k in it.product(*tuple(fix_dims(self.features['dimensions'][j]))):
+                                if self.get(self.features['variables'][(i,j)])[k] not in [0, None]:
+                                    print(f"│ {j}[{k}] =".replace("(", "").replace(")", ""), self.get(self.features['variables'][(i,j)])[k], " "* (box_width-(len(f"│ {j}[{k}] =".replace("(", "").replace(")", "")) + len(str(self.get(self.features['variables'][(i,j)])[k]))) - 1) + "│")
 
                 else:
 
-                    if self.maindims[j] == 0:
-                            if self.get_start(self.mainvars[(i,j)])!=None:
-                                print(f"│ {j} =", [self.get_start(self.mainvars[(i,j)]), self.get_end(self.mainvars[(i,j)])], " "* (box_width-(len(f"│ {j} =") + len(str([self.get_start(self.mainvars[(i,j)]), self.get_end(self.mainvars[(i,j)])])))-1) + "│")
+                    if self.features['dimensions'][j] == 0:
+                            if self.get_start(self.features['variables'][(i,j)])!=None:
+                                print(f"│ {j} =", [self.get_start(self.features['variables'][(i,j)]), self.get_end(self.features['variables'][(i,j)])], " "* (box_width-(len(f"│ {j} =") + len(str([self.get_start(self.features['variables'][(i,j)]), self.get_end(self.features['variables'][(i,j)])])))-1) + "│")
 
 
-                    elif len(self.maindims[j])==1:                    
-                        for k in fix_dims(self.maindims[j])[0]:
-                            if self.get_start(self.mainvars[(i,j)][k])!=None:
-                                print(f"│ {j}[{k}] =", [self.get_start(self.mainvars[(i,j)][k]), self.get_end(self.mainvars[(i,j)][k])], " "* (box_width-(len(f"│ {j} =") + len(str([self.get_start(self.mainvars[(i,j)][k]), self.get_end(self.mainvars[(i,j)][k])])))-1) + "│")
+                    elif len(self.features['dimensions'][j])==1:                    
+                        for k in fix_dims(self.features['dimensions'][j])[0]:
+                            if self.get_start(self.features['variables'][(i,j)][k])!=None:
+                                print(f"│ {j}[{k}] =", [self.get_start(self.features['variables'][(i,j)][k]), self.get_end(self.features['variables'][(i,j)][k])], " "* (box_width-(len(f"│ {j} =") + len(str([self.get_start(self.features['variables'][(i,j)][k]), self.get_end(self.features['variables'][(i,j)][k])])))-1) + "│")
 
                     else:                    
-                        for k in it.product(*tuple(fix_dims(self.maindims[j]))):
-                            if self.get_start(self.mainvars[(i,j)][k])!=None:
-                                print(f"│ {j}[{k}] =", [self.get_start(self.mainvars[(i,j)][k]), self.get_end(self.mainvars[(i,j)][k])], " "* (box_width-(len(f"│ {j} =") + len(str([self.get_start(self.mainvars[(i,j)][k]), self.get_end(self.mainvars[(i,j)][k])])))-1) + "│")
+                        for k in it.product(*tuple(fix_dims(self.features['dimensions'][j]))):
+                            if self.get_start(self.features['variables'][(i,j)][k])!=None:
+                                print(f"│ {j}[{k}] =", [self.get_start(self.features['variables'][(i,j)][k]), self.get_end(self.features['variables'][(i,j)][k])], " "* (box_width-(len(f"│ {j} =") + len(str([self.get_start(self.features['variables'][(i,j)][k]), self.get_end(self.features['variables'][(i,j)][k])])))-1) + "│")
                     
         else:
             
             if show_detailed_tensors: np.set_printoptions(threshold=np.inf)
             
-            for i,j in self.mainvars.keys():
+            for i,j in self.features['variables'].keys():
                 
                 if i!='evar':
                     
                     numpy_var = self.get_numpy_var(j) 
 
                     if type(numpy_var)==np.ndarray:
 
@@ -1083,27 +1717,27 @@
                             else:
                                 left_align(" "*(len(f"{j} =")-1)+row)
                     else:
                         left_align(f"{j} = {numpy_var}")
                         
                 else:
 
-                    if self.maindims[j] == 0:
-                            if self.get_start(self.mainvars[(i,j)])!=None:
-                                print(f"│ {j} =", [self.get_start(self.mainvars[(i,j)]), self.get_end(self.mainvars[(i,j)])], " "* (box_width-(len(f"│ {j} =") + len(str([self.get_start(self.mainvars[(i,j)]), self.get_end(self.mainvars[(i,j)])])))-1) + "│")
-
-                    elif len(self.maindims[j])==1:                    
-                        for k in fix_dims(self.maindims[j])[0]:
-                            if self.get_start(self.mainvars[(i,j)][k])!=None:
-                                print(f"│ {j}[{k}] =", [self.get_start(self.mainvars[(i,j)][k]), self.get_end(self.mainvars[(i,j)][k])], " "* (box_width-(len(f"│ {j} =") + len(str([self.get_start(self.mainvars[(i,j)][k]), self.get_end(self.mainvars[(i,j)][k])])))-1) + "│")
+                    if self.features['dimensions'][j] == 0:
+                            if self.get_start(self.features['variables'][(i,j)])!=None:
+                                print(f"│ {j} =", [self.get_start(self.features['variables'][(i,j)]), self.get_end(self.features['variables'][(i,j)])], " "* (box_width-(len(f"│ {j} =") + len(str([self.get_start(self.features['variables'][(i,j)]), self.get_end(self.features['variables'][(i,j)])])))-1) + "│")
+
+                    elif len(self.features['dimensions'][j])==1:                    
+                        for k in fix_dims(self.features['dimensions'][j])[0]:
+                            if self.get_start(self.features['variables'][(i,j)][k])!=None:
+                                print(f"│ {j}[{k}] =", [self.get_start(self.features['variables'][(i,j)][k]), self.get_end(self.features['variables'][(i,j)][k])], " "* (box_width-(len(f"│ {j} =") + len(str([self.get_start(self.features['variables'][(i,j)][k]), self.get_end(self.features['variables'][(i,j)][k])])))-1) + "│")
 
                     else:                    
-                        for k in it.product(*tuple(fix_dims(self.maindims[j]))):
-                            if self.get_start(self.mainvars[(i,j)][k])!=None:
-                                print(f"│ {j}[{k}] =", [self.get_start(self.mainvars[(i,j)][k]), self.get_end(self.mainvars[(i,j)][k])], " "* (box_width-(len(f"│ {j} =") + len(str([self.get_start(self.mainvars[(i,j)][k]), self.get_end(self.mainvars[(i,j)][k])])))-1) + "│")
+                        for k in it.product(*tuple(fix_dims(self.features['dimensions'][j]))):
+                            if self.get_start(self.features['variables'][(i,j)][k])!=None:
+                                print(f"│ {j}[{k}] =", [self.get_start(self.features['variables'][(i,j)][k]), self.get_end(self.features['variables'][(i,j)][k])], " "* (box_width-(len(f"│ {j} =") + len(str([self.get_start(self.features['variables'][(i,j)][k]), self.get_end(self.features['variables'][(i,j)][k])])))-1) + "│")
                             
     # Methods to work with input and output data.
 
     def max(self, *args):
 
         if self.features['interface_name'] == 'cplex_cp':
             return self.model.max(*args)
@@ -1130,14 +1764,18 @@
             The created set.
 
         Raises
         ------
         ValueError
             If neither bound nor index is provided.
         """
+        
+        if self.features['interface_name']=='gams':
+            from gamspy import Set
+            return Set(self.model, name=index, records=[f"{index}{i}" for i in range(bound[0],bound[1],step)])
 
         # Check if index is an empty string
         if index == '':
             if not to_list:
                 return set(range(bound[0], bound[1], step))
             else:
                 return list(range(bound[0], bound[1], step))
@@ -1162,27 +1800,29 @@
 
     def ambiguity_set(self,*args,**kwds):
         """
         Ambiguity set defintion
         """
         return self.model.ambiguity(*args,**kwds)
 
-    def sum(self, input):
+    def sum(self, input, domain_tuple=None):
         """
         Calculate the sum of all values in the input.
 
         :param input: List of values to be summed.
         :return: The sum of the input values.
         """
         if self.features['interface_name'] == 'cplex':
-            return self.model.Sum(input)
-        
+            return self.model.sum(input)
         elif self.features['interface_name'] == 'gurobi':
-            return self.model.quicksum(input)
-        
+            from gurobipy import quicksum
+            return quicksum(input)
+        elif self.features['interface_name'] == 'mip':
+            from mip import xsum
+            return xsum(input)
         else:
             return sum(input)
 
 
     def card(self, set):
         """
         Card Definition
@@ -1642,29 +2282,28 @@
 
             return self.model.round(x)
 
         else:
 
             return np.round(x)
 
-# Alternatives for defining this class:
-
-model = mdl = add_model = deterministic_model = certain_model = create_environment = env = feloopy = representor_model = learner_model = target_model = uncertain_target_model = uncertain_learner_model = uncertain_representor_model = optimizer = uncertain_model = stochastic_model = robust_model = possibilistic_model = Model
+# Aliases
 
 warnings.simplefilter(action='ignore', category=FutureWarning)
 
 class Implement:
 
     def __init__(self, ModelFunction):
         '''
         Creates and returns an implementor for the representor model.
         '''
 
         self.model_data = ModelFunction(['idle'])
         self.ModelFunction = ModelFunction
+        self.features = self.model_data.features
         self.interface_name = self.model_data.features['interface_name']
         self.solution_method = self.model_data.features['solution_method']
         self.model_name = self.model_data.features['model_name']
         self.solver_name = self.model_data.features['solver_name']
         self.model_constraints = self.model_data.features['constraints']
         self.model_objectives = self.model_data.features['objectives']
         self.objectives_directions = self.model_data.features['directions']
@@ -1683,15 +2322,16 @@
         self.VariablesDim = self.model_data.features['variable_dim']
         self.status = 'Not solved'
         self.response = None
         self.AgentProperties = [None, None, None, None]
         self.get_objective = self.get_obj
         self.get_var = self.get_variable = self.get
         self.search = self.solve = self.optimize = self.run = self.sol
-
+        self.get_tensor = self.get_numpy_var
+        
         match self.interface_name:
 
             case 'mealpy':
 
                 from .generators.model import mealpy_model_generator
                 self.ModelObject = mealpy_model_generator.generate_model(
                     self.solver_name, self.AlgOptions)
@@ -1809,15 +2449,16 @@
         def f6(X): return ObjectivesDirections[5]*self.Fitness(np.array(X))[5]
         my_list_of_functions = [f1, f2, f3, f4, f5, f6]
         parameters = dict()
         list_of_functions = []
         for i in range(len(ObjectivesDirections)): list_of_functions.append(my_list_of_functions[i])
         
         solution = np.concatenate((self.BestAgent, self.BestReward*ObjectivesDirections), axis=1)
-    
+
+   
         parameters = {
         'min_values': (0,)*self.tot_counter[1],
         'max_values': (1,)*self.tot_counter[1],
         'step': step*self.tot_counter[1],
         'solution': solution, 
         'show_pf': True,
         'show_pts': True,
@@ -2361,28 +3002,28 @@
                                     else:
                                         def var(*args):
                                             self.NewAgentProperties = np.round(self.VariablesBound[i[0]][0] + self.BestAgent[self.VariablesSpread[i[0]][0]:self.VariablesSpread[i[0]][1]] * (
                                                 self.VariablesBound[i[0]][1] - self.VariablesBound[i[0]][0]))
                                             return self.NewAgentProperties[sum(args[k]*mt.prod(len(self.VariablesDim[i[0]][j]) for j in range(k+1, len(self.VariablesDim[i[0]]))) for k in range(len(self.VariablesDim[i[0]])))]
                                         return var(*i[1])
                                 case 'svar':
-                                    return np.argsort(self.BestAgent[self.VariablesSpread[i[0]][0]:self.VariablesSpread[i[0]][1]])[i[1]]
+                                    return np.argsort(self.BestAgent[self.VariablesSpread[i[0]][0]:self.VariablesSpread[i[0]][1]])[i[1]].astype(np.int64)
 
                         else:
                             match self.VariablesType[i[0]]:
                                 case 'pvar':
                                     return (self.VariablesBound[i[0]][0] + self.BestAgent[self.VariablesSpread[i[0]][0]:self.VariablesSpread[i[0]][1]] * (self.VariablesBound[i[0]][1] - self.VariablesBound[i[0]][0]))[0]
                                 case 'fvar':
                                     return (self.VariablesBound[i[0]][0] + self.BestAgent[self.VariablesSpread[i[0]][0]:self.VariablesSpread[i[0]][1]] * (self.VariablesBound[i[0]][1] - self.VariablesBound[i[0]][0]))[0]
                                 case 'bvar':
                                     return np.round(self.VariablesBound[i[0]][0] + self.BestAgent[self.VariablesSpread[i[0]][0]:self.VariablesSpread[i[0]][1]] * (self.VariablesBound[i[0]][1] - self.VariablesBound[i[0]][0]))[0]
                                 case 'ivar':
                                     return np.round(self.VariablesBound[i[0]][0] + self.BestAgent[self.VariablesSpread[i[0]][0]:self.VariablesSpread[i[0]][1]] * (self.VariablesBound[i[0]][1] - self.VariablesBound[i[0]][0]))[0]
                                 case 'svar':
-                                    return np.argsort(self.BestAgent[self.VariablesSpread[i[0]][0]:self.VariablesSpread[i[0]][1]])
+                                    return np.argsort(self.BestAgent[self.VariablesSpread[i[0]][0]:self.VariablesSpread[i[0]][1]]).astype(np.int64)
                 case 'feloopy':
                     for i in args:
                         if len(i) >= 2:
                             match self.VariablesType[i[0]]:
                                 case 'pvar':
                                     if self.VariablesDim[i[0]] == 0:
                                         return (self.VariablesBound[i[0]][0] + self.BestAgent[self.VariablesSpread[i[0]][0]:self.VariablesSpread[i[0]][1]] * (self.VariablesBound[i[0]][1] - self.VariablesBound[i[0]][0]))
@@ -2424,29 +3065,29 @@
                                         def var(*args):
                                             self.NewAgentProperties = np.round(self.VariablesBound[i[0]][0] + self.BestAgent[self.VariablesSpread[i[0]][0]:self.VariablesSpread[i[0]][1]] * (
                                                 self.VariablesBound[i[0]][1] - self.VariablesBound[i[0]][0]))
                                             return self.NewAgentProperties[sum(args[k]*mt.prod(len(self.VariablesDim[i[0]][j]) for j in range(k+1, len(self.VariablesDim[i[0]]))) for k in range(len(self.VariablesDim[i[0]])))]
                                         return var(*i[1])
 
                                 case 'svar':
-                                    return np.argsort(self.BestAgent[self.VariablesSpread[i[0]][0]:self.VariablesSpread[i[0]][1]])[i[1]]
+                                    return np.argsort(self.BestAgent[self.VariablesSpread[i[0]][0]:self.VariablesSpread[i[0]][1]])[i[1]].astype(np.int64)
 
                         else:
                             match self.VariablesType[i[0]]:
 
                                 case 'pvar':
                                     return (self.VariablesBound[i[0]][0] + self.BestAgent[self.VariablesSpread[i[0]][0]:self.VariablesSpread[i[0]][1]] * (self.VariablesBound[i[0]][1] - self.VariablesBound[i[0]][0]))
                                 case 'fvar':
                                     return (self.VariablesBound[i[0]][0] + self.BestAgent[self.VariablesSpread[i[0]][0]:self.VariablesSpread[i[0]][1]] * (self.VariablesBound[i[0]][1] - self.VariablesBound[i[0]][0]))
                                 case 'bvar':
                                     return np.round(self.VariablesBound[i[0]][0] + self.BestAgent[self.VariablesSpread[i[0]][0]:self.VariablesSpread[i[0]][1]] * (self.VariablesBound[i[0]][1] - self.VariablesBound[i[0]][0]))
                                 case 'ivar':
                                     return np.round(self.VariablesBound[i[0]][0] + self.BestAgent[self.VariablesSpread[i[0]][0]:self.VariablesSpread[i[0]][1]] * (self.VariablesBound[i[0]][1] - self.VariablesBound[i[0]][0]))
                                 case 'svar':
-                                    return np.argsort(self.BestAgent[self.VariablesSpread[i[0]][0]:self.VariablesSpread[i[0]][1]])
+                                    return np.argsort(self.BestAgent[self.VariablesSpread[i[0]][0]:self.VariablesSpread[i[0]][1]]).astype(np.int64)
         else:
 
             for i in args:
                 if len(i) >= 2:
 
                     match self.VariablesType[i[0]]:
 
@@ -2494,29 +3135,29 @@
                                     self.NewAgentProperties = np.round(self.VariablesBound[i[0]][0] + self.BestAgent[:, self.VariablesSpread[i[0]][0]:self.VariablesSpread[i[0]][1]] * (
                                         self.VariablesBound[i[0]][1] - self.VariablesBound[i[0]][0]))
                                     return self.NewAgentProperties[sum(args[k]*mt.prod(len(self.VariablesDim[i[0]][j]) for j in range(k+1, len(self.VariablesDim[i[0]]))) for k in range(len(self.VariablesDim[i[0]])))]
                                 return var(*i[1])
 
                         case 'svar':
 
-                            return np.argsort(self.BestAgent[:, self.VariablesSpread[i[0]][0]:self.VariablesSpread[i[0]][1]])[i[1]]
+                            return np.argsort(self.BestAgent[:, self.VariablesSpread[i[0]][0]:self.VariablesSpread[i[0]][1]])[i[1]].astype(np.int64)
 
                 else:
 
                     match self.VariablesType[i[0]]:
                         case 'pvar':
                             return (self.VariablesBound[i[0]][0] + self.BestAgent[:, self.VariablesSpread[i[0]][0]:self.VariablesSpread[i[0]][1]] * (self.VariablesBound[i[0]][1] - self.VariablesBound[i[0]][0]))
                         case 'fvar':
                             return (self.VariablesBound[i[0]][0] + self.BestAgent[:, self.VariablesSpread[i[0]][0]:self.VariablesSpread[i[0]][1]] * (self.VariablesBound[i[0]][1] - self.VariablesBound[i[0]][0]))
                         case 'bvar':
                             return np.round(self.VariablesBound[i[0]][0] + self.BestAgent[:, self.VariablesSpread[i[0]][0]:self.VariablesSpread[i[0]][1]] * (self.VariablesBound[i[0]][1] - self.VariablesBound[i[0]][0]))
                         case 'ivar':
                             return np.round(self.VariablesBound[i[0]][0] + self.BestAgent[:, self.VariablesSpread[i[0]][0]:self.VariablesSpread[i[0]][1]] * (self.VariablesBound[i[0]][1] - self.VariablesBound[i[0]][0]))
                         case 'svar':
-                            return np.argsort(self.BestAgent[:, self.VariablesSpread[i[0]][0]:self.VariablesSpread[i[0]][1]])
+                            return np.argsort(self.BestAgent[:, self.VariablesSpread[i[0]][0]:self.VariablesSpread[i[0]][1]]).astype(np.int64)
 
     def dis_indicators(self, ideal_pareto: Optional[np.ndarray] = [], ideal_point: Optional[np.array] = [], step: Optional[tuple] = (0.1,), epsilon: float = 0.01, p: float = 2.0, n_clusters: int = 5, save_path: Optional[str] = None, show_log: Optional[bool] = False):
 
         """
         Calculates selected Pareto front metrics and displays the results in a tabulated format.
 
         :param ideal_pareto: An array of shape (n_samples, n_objectives) containing the ideal Pareto front. Default is None.
@@ -2731,14 +3372,20 @@
                 val = self.get_obj()[ind, :]
             elif self.objectives_directions[i] =='min':
                 ind = np.argmin(self.get_obj()[:, i])
                 val = self.get_obj()[ind, :]
             payoff.append(val)
         return np.array(payoff)
 
+    def clean_report(self):
+
+        command = "cls" if os.name == "nt" else "clear"
+        os.system(command)
+        self.report()
+        
     def report(self, all_metrics: bool = False, feloopy_info: bool = True, sys_info: bool = False, model_info: bool = True, sol_info: bool = True, obj_values: bool = True, dec_info: bool = True, metric_info: bool = True, ideal_pareto: Optional[np.ndarray] = [], ideal_point: Optional[np.array] = [], show_tensors = False, show_detailed_tensors=False, save=None):
 
         if not self.healthy():
             print()
             print()
             print('WARNING: Model is not healthy!')
             print()
@@ -2750,24 +3397,24 @@
 
         status = self.get_status()
         hour, min, sec = calculate_time_difference(self.start,self.end)
 
         if len(str(status)) == 0:
             status = ['infeasible (constrained)']
 
-        box_width = 80
+        box_width = 90
         vspace()
 
         if feloopy_info:
             
             import datetime
             now = datetime.datetime.now()
             date_str = now.strftime("Date: %Y-%m-%d")
             time_str = now.strftime("Time: %H:%M:%S")
-            tline_text("FelooPy v0.2.8")
+            tline_text("FelooPy v0.2.9")
             empty_line()
             two_column(date_str, time_str)
             two_column(f"Interface: {self.interface_name}", f"Solver: {self.solver_name}")
             empty_line()
             bline()
 
         if sys_info:
@@ -2854,48 +3501,43 @@
             bline()
 
         if save is not None:
             sys.stdout.close()
             sys.stdout = stdout_origin
 
     def get_numpy_var(self, var_name):
+        output = []
 
         for i in self.VariablesDim.keys():
-            if i==var_name:
-
+            if i == var_name:
                 if self.VariablesDim[i] == 0:
-
-                    output = self.get([i, (0,)])
-
+                    output.append(self.get([i, (0,)]))
                 elif len(self.VariablesDim[i]) == 1:
-
-                    output = np.zeros(shape=len(fix_dims(self.VariablesDim[i])[0]))
-
                     for k in fix_dims(self.VariablesDim[i])[0]:
-                        
-                        output[k] = self.get([i, (k,)])
-
+                        output.append(self.get([i, (k,)]))
                 else:
-                    output = np.zeros(shape=tuple([len(dim) for dim in fix_dims(self.VariablesDim[i])]))
                     for k in it.product(*tuple(fix_dims(self.VariablesDim[i]))):
+                        output.append(self.get([i, (*k,)]))
+        
 
-                        output[k] = self.get([i, (*k,)])
-
-        return output
-
+            
+        return np.array(output)
+    
     def healthy(self):
         try:
             status = self.get_status().lower()
             return ('optimal' in status or 'feasible' in status) and 'infeasible' not in status
         except:
-            status = self.get_status()[0].lower()
-            return ('feasible' in status or 'optimal' in status) and 'infeasible' not in status
-        
-    def decision_information_print(self, status, show_tensors, show_detailed_tensors, box_width=80):
-        
+            try:
+                status = self.get_status()[0].lower()
+                return ('feasible' in status or 'optimal' in status) and 'infeasible' not in status
+            except:
+                return False
+            
+    def decision_information_print(self, status, show_tensors, show_detailed_tensors, box_width=88):
         
         if show_detailed_tensors: show_tensors=True
         
         if not show_tensors:
         
             if type(status) == str:
                 for i in self.VariablesDim.keys():
@@ -2948,107 +3590,29 @@
                     else:
                         left_align(f"{i} = {numpy_var}")
                                             
 # Alternatives for defining this class:
             
 construct = make_model = implementor = implement = Implement
 
-
-WEIGHTING_ALGORITHMS = [
-    ['ahp_method','pydecision'],
-    ['fuzzy_ahp_method','pydecision'],
-    ['bw_method','pydecision'],
-    ['fuzzy_bw_method','pydecision'],
-    ['cilos_method', 'pydecision'],
-    ['critic_method', 'pydecision'],
-    ['entropy_method', 'pydecision'],
-    ['idocriw_method', 'pydecision'],
-    ['merec_method', 'pydecision'],
-    ['lp_method', 'feloopy'],
-    ]
-
-RANKING_ALGORITHMS = [
-    ['aras_method', 'pydecision'],
-    ['fuzzy_aras_method', 'pydecision'],
-    ['borda_method', 'pydecision'],
-    ['cocoso_method', 'pydecision'],
-    ['codas_method', 'pydecision'],
-    ['copeland_method', 'pydecision'],
-    ['copras_method', 'pydecision'],
-    ['fuzzy_copras_method', 'pydecision'],
-    ['cradis_method', 'pydecision'],
-    ['edas_method', 'pydecision'],
-    ['fuzzy_edas_method', 'pydecision'],
-    ['gra_method', 'pydecision'],
-    ['mabac_method', 'pydecision'],
-    ['macbeth_method', 'pydecision'],
-    ['mairca_method', 'pydecision'],
-    ['marcos_method', 'pydecision'],
-    ['maut_method', 'pydecision'],
-    ['moora_method', 'pydecision'],
-    ['fuzzy_moora_method', 'pydecision'],
-    ['moosra_method', 'pydecision'],
-    ['multimoora_method', 'pydecision'],
-    ['ocra_method', 'pydecision'],
-    ['fuzzy_ocra_method', 'pydecision'],
-    ['oreste_method', 'pydecision'],
-    ['piv_method', 'pydecision'],
-    ['promethee_ii', 'pydecision'],
-    ['promethee_iv', 'pydecision'],
-    ['promethee_vi', 'pydecision'],
-    ['psi_method', 'pydecision'],
-    ['regime_method', 'pydecision'],
-    ['rov_method', 'pydecision'],
-    ['saw_method', 'pydecision'],
-    ['smart_method', 'pydecision'],
-    ['spotis_method', 'pydecision'],
-    ['todim_method', 'pydecision'],
-    ['topsis_method', 'pydecision'],
-    ['fuzzy_topsis_method', 'pydecision'],
-    ['vikor_method', 'pydecision'],
-    ['fuzzy_vikor_method', 'pydecision'],
-    ['waspas_method', 'pydecision'],
-    ['fuzzy_waspas_method', 'pydecision'],
-    ['la_method', 'feloopy'],
-    ]
-
-SPECIAL_ALGORITHMS = [
-    ['dematel_method', 'pydecision'],
-    ['fuzzy_dematel_method', 'pydecision'],
-    ['electre_i', 'pydecision'],
-    ['electre_i_s', 'pydecision'],
-    ['electre_i_v', 'pydecision'],
-    ['electre_ii', 'pydecision'],
-    ['electre_iii', 'pydecision'],
-    ['electre_iv', 'pydecision'],
-    ['electre_tri_b', 'pydecision'],
-    ['promethee_i', 'pydecision'],
-    ['promethee_iii', 'pydecision'],
-    ['promethee_v', 'pydecision'],
-    ['promethee_gaia', 'pydecision'],
-    ['wings_method', 'pydecision'],
-    ['cwdea_method', 'feloopy']
-]
-
-# Missing: SWOT, BOCR, ANP
-
 class MADM:
 
     def __init__(self, solution_method, problem_name, interface_name):
         """
         Initializes an instance of MADM.
 
         Parameters:
         solution_method (str): The solution method to use.
         problem_name (str): The name of the problem.
         interface_name (str): The name of the interface.
 
         Returns:
         None
         """
+        
         self.model_name = problem_name
         self.interface_name = 'pyDecision.algorithm' if interface_name == 'pydecision' else interface_name
         self.madam_method = solution_method
 
         if self.interface_name == 'pyDecision.algorithm':
             if "_method" not in solution_method and 'auto' not in solution_method and 'electre' not in solution_method and 'promethee' not in solution_method:
                 self.madam_method = solution_method + "_method"
@@ -3061,14 +3625,16 @@
                 self.madam_method = solution_method + "_method"
 
         if solution_method == 'auto':
             self.madam_method = 'auto'
 
         self.solver_options = dict()
 
+        self.get_tensor = self.get_numpy_var
+
         self.features = {
             'weights_found': False,
             'ranks_found': False,
             'inconsistency_found': False,
             'dpr_found': False,
             'dmr_found': False,
             'rpc_found': False,
@@ -3085,14 +3651,17 @@
             'd_rank_found': False,
             'a_rank_found': False,
             'n_rank_found': False,
             'p_rank_found': False,
             'classification_found': False,
             'selection_found': False
         }
+        
+    def healthy(self):
+        return True
 
     def add_criteria_set(self, index='', bound=None, step=1, to_list=False):
         """
         Adds a criteria set.
 
         Parameters:
         index (str): The index of the criteria set.
@@ -3817,15 +4386,21 @@
     def get_crisp_weights(self):
 
         return self.crisp_weights
         
     def get_normalized_weights(self):
         
         return self.normalized_weights
-    
+
+    def clean_report(self):
+
+        command = "cls" if os.name == "nt" else "clear"
+        os.system(command)
+        self.report()
+        
     def report(self, all_metrics=False, feloopy_info=True, sys_info=False,
                         model_info=True, sol_info=True, metric_info=True,
                         ideal_pareto=None, ideal_point=None, show_tensors=False,
                         show_detailed_tensors=False, save=None, decimals = 4):
 
         self.show_tensor = show_tensors
         self.show_detailed_tensors = show_detailed_tensors
@@ -3845,14 +4420,20 @@
             self._generate_sol_info()
 
         if metric_info:
             self._generate_metric_info()
 
         self._generate_decision_info()
 
+    def clean_report(self):
+
+        command = "cls" if os.name == "nt" else "clear"
+        os.system(command)
+        self.report()
+        
     def display_as_tensor(self, name, numpy_var, detailed):
         if detailed:
             np.set_printoptions(threshold=np.inf)
 
         if isinstance(numpy_var, np.ndarray):
             tensor_str = np.array2string(numpy_var, separator=', ', prefix='│ ') #Style argument deprecated.
             rows = tensor_str.split('\n')
@@ -3868,15 +4449,15 @@
     def _generate_feloopy_info(self):
 
         import datetime
         now = datetime.datetime.now()
         date_str = now.strftime("Date: %Y-%m-%d")
         time_str = now.strftime("Time: %H:%M:%S")
 
-        tline_text("FelooPy v0.2.8")
+        tline_text("FelooPy v0.2.9")
         empty_line()
         two_column(date_str, time_str)
 
         if 'pydecision' in self.interface_name.lower():
             interface = 'pydecision'
             two_column(f"Interface: {interface}", f"Solver: {self.madam_method}")
 
@@ -3948,8 +4529,867 @@
         empty_line()
         left_align(f"Method: {self.madam_method}")
         left_align(f"Status: {self.status}")
 
         empty_line()
         bline()
     
-madm = MADM
+madm = MADM
+
+class feloop_model(model):
+    def __init__(self,name=None, agent=None):
+        if agent==None:
+            super().__init__('exact', name, 'feloopy')
+        else:
+            super().__init__('heuristic', name, 'feloopy', agent=agent)
+
+class copt_model(model):
+    def __init__(self,name='x'):
+        super().__init__('exact', name, 'copt')
+
+class cplex_cp_model(model):
+    def __init__(self,name='x'):
+        super().__init__('constraint', name, 'cplex_cp')
+
+class cplex_model(model):
+    def __init__(self,name='x'):
+        super().__init__('exact', name, 'cplex')
+
+class cylp_model(model):
+    def __init__(self,name='x'):
+        super().__init__('exact', name, 'cylp')
+
+class cvxpy_model(model):
+    def __init__(self,name='x'):
+        super().__init__('exact', name, 'cvxpy')
+
+class gekko_model(model):
+    def __init__(self,name='x'):
+        super().__init__('exact', name, 'gekko')
+
+class gurobi_model(model):
+    def __init__(self,name='x'):
+        super().__init__('exact', name, 'gurobi')
+
+class gams_model(model):
+    def __init__(self,name='x'):
+        super().__init__('exact', name, 'gams')
+
+class linopy_model(model):
+    def __init__(self,name='x'):
+        super().__init__('exact', name, 'linopy')
+
+class mip_model(model):
+    def __init__(self,name='x'):
+        super().__init__('exact', name, 'mip')
+
+class ortools_cp_model(model):
+    def __init__(self,name='x'):
+        super().__init__('constraint', name, 'ortools_cp')
+
+class ortools_model(model):
+    def __init__(self,name='x'):
+        super().__init__('exact', name, 'ortools')
+
+class picos_model(model):
+    def __init__(self,name='x'):
+        super().__init__('exact', name, 'picos')
+
+class pulp_model(model):
+    def __init__(self,name='x'):
+        super().__init__('exact', name, 'pulp')
+
+class pyomo_model(model):
+    def __init__(self,name='x'):
+        super().__init__('exact', name, 'pyomo')
+
+class pymprog_model(model):
+    def __init__(self,name='x'):
+        super().__init__('exact', name, 'pymprog')
+
+class rsome_dro_model(model):
+    def __init__(self,name='x'):
+        super().__init__('exact', name, 'rsome_dro')
+
+class rsome_ro_model(model):
+    def __init__(self,name='x'):
+        super().__init__('exact', name, 'rsome_ro')
+
+class seeker_model(model):
+    def __init__(self,name='x'):
+        super().__init__('exact', name, 'seeker')
+
+class xpress_model(model):
+    def __init__(self,name='x'):
+        super().__init__('exact', name, 'xpress')
+        
+class search(model,Implement):
+
+    def __init__(
+        self,
+        environment=None,
+        name="model_name",
+        method="exact",
+        approach = "nwsm",
+        interface="pymprog",
+        directions=["max"],
+        solver="glpk",
+        dataset = None,
+        key_params = [],
+        key_vars = [],
+        scenarios = [],
+        benchmark=None,
+        repeat=1,
+        verbose=False,
+        should_run=True,
+        memorize=True,
+        report=False,
+        control_scenario=0,
+        options={},
+        email=None,
+        time_limit=None,
+        cpu_threads=None,
+        absolute_gap=None,
+        relative_gap=None,
+        *args, **kwargs
+    ):
+
+        self.key_params = key_params
+        self.key_vars = key_vars
+        self.scenarios =  scenarios
+        self.email = email
+        self.cpu_threads = cpu_threads
+        self.time_limit = time_limit
+        self.absolute_gap = absolute_gap
+        self.relative_gap = relative_gap
+        self.args = args
+        self.kwargs = kwargs 
+        self.environment = environment
+        self.name = name
+        self.method = method
+        self.approach = approach
+        self.interface = interface
+        self.directions = directions
+        self.solver = solver
+        self.verbose = verbose
+        self.should_run = should_run
+        self.memorize = memorize
+        self.sensitivity_analyzed = False
+        self.options = options
+        self.should_benchmark = True if (type(benchmark)==str and benchmark=='all') or (type(benchmark)==list and len(benchmark)>=1) else False
+        self.data = {}
+        self.repeat = repeat
+        
+        self.number_of_objectives = len(self.directions)
+        
+        self.create_env(environment)
+            
+        if self.should_run:
+
+            if self.should_benchmark: 
+                self.benchmark_results = self.benchmark(algorithms=benchmark, repeat=self.repeat)
+                       
+            self.run(verbose=self.verbose)
+        
+        if len(self.key_params)!=0:
+            self.sensitivity(dataset, key_params, scenarios, environment,control_scenario)
+            
+        if report:
+            self.report()
+    
+    def clean_report(self):
+
+        command = "cls" if os.name == "nt" else "clear"
+        os.system(command)
+        self.report()
+        
+    def create_env(self, environment):
+        
+        self.penalty_coefficient=self.options.get("penalty_coefficient",0)
+        if "penalty_coefficient" in self.options.keys():
+            del self.options["penalty_coefficient"]
+    
+        if self.method in ["exact", "convex", "constraint", "uncertain"]:
+            self.em = model(method=self.method,name=self.name,interface=self.interface)
+            self.em = self.environment(self.em, *self.args, **self.kwargs)
+          
+        if self.method in ["heuristic"]:
+            if len(self.directions)==1:
+                def instance(X):
+                    lm = model(method=self.method, name=self.name, interface=self.interface, agent=X)
+                    lm = environment(lm)
+                    lm.sol(directions=self.directions,solver=self.solver,show_log=self.verbose, solver_options=self.options)
+                    return lm[X]
+                
+                self.em = Implement(instance)
+
+            else:
+                def instance(X):
+                    m = model(self.name,self.method, self.interface,X)
+                    m = self.environment(m, *self.args, **self.kwargs)
+                    m.sol(self.directions, self.solver, self.options, obj_id='all')
+                    return m[X]
+
+                self.em = implement(instance)
+
+        if self.method in ["madm"]:
+            self.em = madm(self.solver,self.name, self.interface)
+            self.em = self.environment(self.em, *self.args, **self.kwargs)
+
+    def healthy(self):
+        return self.em.healthy()
+    
+    def run(self, verbose):
+        
+        import sys
+        import threading
+        import time
+
+        solving_complete = False
+        
+        if not verbose:
+            """
+            def animate():
+                while not solving_complete:
+                    for frame in ['◴', '◷', '◶', '◵']:
+                        sys.stdout.write('\rSolving... ' + frame + ' ')
+                        sys.stdout.flush()
+                        time.sleep(0.1)
+
+            animate_thread = threading.Thread(target=animate)
+            animate_thread.daemon = True
+            animate_thread.start()
+            """
+            
+        if  self.number_of_objectives==1:
+            if self.method in ["exact", "convex", "constraint", "uncertain"]:
+                self.em.sol(directions=self.directions, solver=self.solver, show_log=verbose, email=self.email, time_limit=self.time_limit, cpu_threads=self.cpu_threads,absolute_gap=self.absolute_gap, relative_gap=self.relative_gap)
+                    
+            elif self.method == "heuristic":
+                self.em.sol(penalty_coefficient=self.penalty_coefficient, number_of_times=self.repeat)
+        else:
+            if self.method in ["exact", "convex", "constraint", "uncertain"]:
+                
+                try:
+                    from .extras.algorithms.exact.multiobjective import sol_multi
+                except:
+                    from .algorithms.exact.multiobjective import sol_multi
+                    
+                def instance():
+                    self.em = model(method=self.method, name=self.name, interface=self.interface)
+                    self.em = self.environment(self.em, *self.args, **self.kwargs)
+                    return self.em
+                
+                self.time_solve_begin = timeit.default_timer()
+                self.result = sol_multi(instance=instance,
+                                         directions=self.directions.copy(),
+                                         objective_id=self.approach,
+                                         solver_name=self.solver,
+                                         save_vars=True,
+                                         approach_options=self.options,
+                                         show_log=verbose, 
+                                         email=self.email, 
+                                         time_limit=self.time_limit, 
+                                         cpu_threads=self.cpu_threads,
+                                         absolute_gap=self.absolute_gap, 
+                                         relative_gap=self.relative_gap
+                                         )
+                self.time_solve_end = timeit.default_timer()
+            elif self.method == "heuristic":
+                self.em.solve(show_log=False, penalty_coefficient=self.penalty_coefficient)
+
+        if self.method == "madm":
+            self.time_solve_begin = timeit.default_timer()
+            self.em.sol()
+            self.time_solve_end = timeit.default_timer()
+        
+        if self.method in ["heuristic"]: self.cpt = self.em.get_time()
+            
+        if self.em.healthy():
+            if self.method not in ["madm"]:
+                if self.number_of_objectives != 1:
+                    if self.method not in ["heuristic"]:
+                        self.solutions = self.result[3]
+                    else:
+                        num_pareto = self.em.get_obj().shape[0]
+                        self.solutions = {i: {} for i in range(num_pareto)}
+                        for i in range(num_pareto):
+                            for j in self.em.VariablesDim.keys():
+                                self.solutions[i][j] = self.em.get_numpy_var(j)
+                else:
+                    self.solutions = {}
+                    if self.method not in ["heuristic"]:
+                        for typ, var in self.em.features['variables'].keys():
+                            self.solutions[var] = self.em.get_numpy_var(var)
+                    else:
+                        for j in self.em.VariablesDim.keys():
+                            self.solutions[j] = self.em.get_numpy_var(j)
+            else:
+                values_list = [
+                        'rv', 
+                        'wv', 
+                        'fwv', 
+                        'dmrv', 
+                        'dprv',
+                        'rmcv',
+                        'rpcv',
+                        'dominated',
+                        'concordance',
+                        'discordance',
+                        'kernel',
+                        'dominance',
+                        'dominance_s',
+                        'dominance_w',
+                        'global_concordance',
+                        'credibility',
+                        'rank_d',
+                        'rank_a',
+                        'classification'
+                    ]
+                self.solutions = {}
+                for key in values_list:
+                    try:
+                        self.solutions[key] = self.em.get_numpy_var(key)
+                    except:
+                        pass
+            
+            if self.memorize:
+                if self.number_of_objectives == 1:
+                    self.data.update(self.solutions)
+                else:
+                    self.data.update({"pareto": self.solutions})
+
+            if self.method != 'madm':
+                if self.number_of_objectives == 1:
+                    self.objective_values = np.array([[self.em.get_obj()]])
+                    self.num_objective_values = 1
+                    self.cpt = self.em.get_time()
+                else:
+                    if self.method == "heuristic":
+                        self.objective_values = self.em.get_obj()
+                        self.num_objective_values = self.objective_values.shape[0]
+                        self.cpt = self.em.get_time()
+                    else:
+                        self.objective_values = self.result[0]
+                        self.num_objective_values = self.objective_values.shape[0]
+                        self.cpt = self.time_solve_end - self.time_solve_begin
+            
+            if self.memorize:
+                if self.method != 'madm':
+                    self.data["obj"] = self.objective_values
+                    self.data["cpt"] = self.cpt
+                    self.data["healthy"] = self.em.healthy()
+                else:
+                    self.data["cpt"] = self.time_solve_end - self.time_solve_begin
+                    self.data["healthy"] = self.em.healthy()               
+            
+        solving_complete = True
+
+        if not verbose:
+            """
+            # Ensure the animation stops after solving is completed
+            sys.stdout.write('\rSolving... Done!    \n')
+            sys.stdout.flush()
+            """
+            
+    def get(self,input=None):
+        
+        if type(input)==str:
+            return self.em.get_tensor(input)
+
+    def get_obj(self):
+        if self.number_of_objectives==1:
+            return self.em.get_obj()
+        else:
+            if self.method=='heuristic':
+                return self.em.get_obj()
+            else:
+                return self.result[0]
+                
+        
+    def get_dual(self,input):
+        return self.em.get_dual(input)
+
+    def get_slack(self,input):
+        return self.em.get_slack(input)
+      
+    def sensitivity(self, dataset, parameter_names, parameter_values, environment=None,control_scenario=0):
+        
+        self.sensitivity_parameter_names = parameter_names
+        self.sensitivity_parameter_values = parameter_values
+        
+        if self.em.healthy():
+            
+            self.sensitivity_analyzed = True
+    
+            
+            self.sensitivity_memorize = False
+            self.sensitivity_verbose=False
+            if environment is None: 
+                environment = self.environment
+            
+            number_of_parameters = len(parameter_values)
+            number_of_names = len(parameter_names)
+            
+            if number_of_parameters != number_of_names:
+                raise ValueError("Number of parameter names and values do not match. It should be like ['a','b','c'] and [list_values_of_a (e.g., [1,2,3]), list_values_of_b (e.g., [1,2,3]), list_values_of_c (e.g., [1,2,3])]")
+        
+            sensitivity_keys = [
+                "sensitivtiy_values",
+                "sensitivtiy_of_health_to",
+                "sensitivtiy_of_cpt_to",
+                "sensitivtiy_of_objectives_to",
+                "sensitivtiy_of_solutions_to",
+            ]
+            
+            self.sensitivity_begin_timer = timeit.default_timer()
+            for parameter_name in parameter_names:
+                for key in sensitivity_keys:
+                    dataset.store(f"{key}_{parameter_name}", [])
+                previous_parameter_value = copy.deepcopy(dataset.data[parameter_name])
+                for parameter_value in parameter_values[parameter_names.index(parameter_name)]:
+                    dataset.data[f"sensitivtiy_values_{parameter_name}"].append(parameter_value)
+                    dataset.data[parameter_name] = parameter_value
+                    self.create_env(environment)
+                    with suppress(Exception):
+                        self.run(verbose=self.verbose)
+                    if self.method!='madm':
+                        if self.number_of_objectives==1:
+                            #Single-objective case extraction
+                            self.sensitivity_solutions = {}
+                            if self.method != "heuristic":
+                                for typ, var in self.em.features['variables'].keys():
+                                    self.sensitivity_solutions[var] = self.em.get_numpy_var(var) if self.em.healthy() else None
+                            else:
+                                for j in self.em.VariablesDim.keys():
+                                    self.sensitivity_solutions[j]=self.em.get_numpy_var(j) if self.em.healthy() else None
+                            self.sensitivity_objective_values = np.array([[self.em.get_obj()]])[0][0] if self.em.healthy() else None
+                            self.sensitivity_num_objective_values = 1
+                            self.sensitivity_cpt = self.em.get_time()
+                        else:
+                            #Multi-objective case extraction
+                            if self.method != "heuristic":
+                                self.sensitivity_solutions = self.result[3] if self.em.healthy() else None
+                                self.sensitivity_objective_values = self.result[0] if self.em.healthy() else np.array([[None for i in range(self.directions)]])
+                                self.sensitivity_num_objective_values = self.objective_values.shape[0]
+                                self.sensitivity_cpt = self.time_solve_end - self.time_solve_begin        
+                            else:
+                                self.sensitivity_num_objective_values = self.em.get_obj().shape[0] if self.em.healthy()  else 1
+                                self.sensitivity_solutions  = {i: {} for i in range(self.num_objective_values)}
+                                for i in range(self.sensitivity_num_objective_values):
+                                    for j in self.em.VariablesDim.keys():
+                                        self.sensitivity_solutions[i][j]=self.em.get_numpy_var(j) if self.em.healthy() else None
+                                self.sensitivity_objective_values = self.em.get_obj() if self.em.healthy() else None
+                                self.sensitivity_num_objective_values = self.objective_values.shape[0]
+                                self.sensitivity_cpt = self.time_solve_end - self.time_solve_begin
+                    dataset.data[f"sensitivtiy_of_health_to_{parameter_name}"].append(self.em.healthy())
+                    dataset.data[f"sensitivtiy_of_cpt_to_{parameter_name}"].append(self.sensitivity_cpt)
+                    dataset.data[f"sensitivtiy_of_objectives_to_{parameter_name}"].append(self.sensitivity_objective_values)
+                    dataset.data[f"sensitivtiy_of_solutions_to_{parameter_name}"].append(self.sensitivity_solutions)
+  
+                dataset.data[parameter_name] = previous_parameter_value
+            self.sensitivity_end_timer = timeit.default_timer()         
+            
+            if self.number_of_objectives==1:
+                for parameter_name in parameter_names:
+                    dataset.data[f"sensitivtiy_of_similarity_to_{parameter_name}"] = compute_similarity(dataset.data[f"sensitivtiy_of_solutions_to_{parameter_name}"],control_scenario_id=control_scenario)
+
+            self.sensitivity_data = copy.deepcopy(dataset.data)
+
+            return self.sensitivity_data
+
+    def benchmark(self, environment=None, algorithms=None, repeat=1, show_report=False):
+
+        if environment is None:
+            environment = self.environment        
+        
+        if algorithms is None:
+            if self.method=="exact":
+                algorithms=EXACT_ALGORITHMS
+            if self.method=="heuristic":
+                algorithms=HEURISTIC_ALGORITHMS
+        
+        columns = pd.MultiIndex.from_product([['time', 'obj'], ['ave', 'std', 'min', 'max']],names=['metric', 'stat'])
+        df = pd.DataFrame(columns=columns,index=[i+1 for i in range(len(algorithms))])
+        counter = 0
+        for interface, solver in progress_bar(algorithms, unit="alg", description="Benchmarking"):
+            objs = []
+            times = []
+            try:
+                for _ in range(repeat):
+                    self.create_env(environment)
+                    with suppress(Exception):
+                        self.run(verbose=self.verbose)
+                    objs.append(self.em.get_obj())
+                    times.append(self.em.get_time())
+                    
+                df.loc[counter+1, ('time', 'ave')] = pd.Series(times).mean()
+                df.loc[counter+1, ('time', 'std')] = pd.Series(times).std()
+                df.loc[counter+1, ('time', 'min')] = pd.Series(times).min()
+                df.loc[counter+1, ('time', 'max')] = pd.Series(times).max()
+                df.loc[counter+1, ('obj', 'ave')] = pd.Series(objs).mean()
+                df.loc[counter+1, ('obj', 'std')] = pd.Series(objs).std()
+                df.loc[counter+1, ('obj', 'min')] = pd.Series(objs).min()
+                df.loc[counter+1, ('obj', 'max')] = pd.Series(objs).max()
+                df.loc[counter+1, ('interface', '')] = interface
+                df.loc[counter+1, ('solver', '')] = solver
+                
+            except:
+                
+                df.loc[counter+1, ('interface', '')] = interface
+                df.loc[counter+1, ('solver', '')] = solver        
+                pass
+            
+            os.system('cls' if os.name == 'nt' else 'clear')
+            counter += 1
+            
+        df_cleaned = df.dropna(subset=[('time', 'ave'), ('obj', 'ave')]).reset_index(drop=True)
+        df_sorted = df_cleaned.sort_values(by=('time', 'ave'))
+        df_sorted = df_sorted.reset_index(drop=True)
+        
+        if show_report:
+            print(df_sorted.to_string())
+
+        self.ben_results = df_sorted
+
+        return self.ben_results
+
+    def clean_report(self,full=False):
+
+        command = "cls" if os.name == "nt" else "clear"
+        os.system(command)
+        self.report(full=full)
+
+    def report(self, skip_system_information=True,width=90,style=1,skip=False,full=False):
+        
+        # First box: FelooPy
+        print()
+        from colorama import init, Fore
+        init(autoreset=True)
+
+        phealthy = "Unknown"
+        if self.em.healthy() or self.method=="madm" or self.sensitivity_analyzed:
+            phealthy = f"{Fore.GREEN}{'√ Healthy'}"
+        else:
+            phealthy = f"{Fore.RED}{'X Unhealthy'}"
+
+        print(phealthy)
+        print()
+        
+        box = report(width=width, style=style)
+    
+        import datetime
+        current_datetime = datetime.datetime.now()
+        formatted_date = current_datetime.strftime("%Y-%m-%d")
+        formatted_time = current_datetime.strftime("%H:%M:%S")
+    
+        box.top(left="FelooPy v0.2.9", right="Released April 2024")
+        box.empty()
+        
+        box.clear_columns(list_of_strings=["", f"Interface: {self.interface}"], label=f"Date: {formatted_date}", max_space_between_elements=4)
+        box.clear_columns(list_of_strings=["", f"Solver: {self.solver}"], label=f"Time: {formatted_time}", max_space_between_elements=4)
+        box.clear_columns(list_of_strings=["",f"Method: {self.method}"], label= f"Name: {self.name}", max_space_between_elements=4)
+        
+        if self.method in ["exact", "convex", "constraint", "uncertain","heuristic"]:
+            if self.number_of_objectives==1:
+                ptype = "single-objective"
+            elif self.number_of_objectives<=3:
+                ptype = "multi-objective"
+            else:
+                ptype = "many-objective"
+        else:
+            ptype="multi-attribute"
+        
+        try:
+            if len(self.em.solver_options) >= 1:
+                pconfigurated = "√ Configured"
+            else:
+                pconfigurated = "X Unconfigured"
+        except:
+            try:
+                if len(self.em.features['solver_options']) >= 1:
+                    pconfigurated = "√ Configured"
+                else:
+                    pconfigurated = "X Unconfigured"
+            except:
+                pconfigurated = "N/A"
+    
+        import platform
+        import psutil
+        import cpuinfo
+        import GPUtil
+    
+        def get_system_characteristics():
+            os_info = platform.system()
+            ram_info = np.round(psutil.virtual_memory().total / (1024.0 ** 3))
+            cpu_info = cpuinfo.get_cpu_info()
+            cpu_generation = cpu_info['brand_raw'].split()[-1]
+            gpus = GPUtil.getGPUs()
+            gpu_memory = sum(gpu.memoryTotal for gpu in gpus)
+            gpu_memory_gb = np.round(gpu_memory / 1024)
+            system_characteristics = f"OS:{os_info} RAM:{ram_info}GB CPU:{cpu_generation} GPU:{gpu_memory_gb}GB"
+            return system_characteristics
+
+        box.clear_columns(list_of_strings=["",f"{pconfigurated}"], label= f"Type: {ptype}", max_space_between_elements=4)
+        
+        box.empty()
+                
+        if skip_system_information is False:
+            try: 
+                box.bottom(right=get_system_characteristics())
+            except:
+                box.bottom()
+        else:
+            box.bottom()
+        print()
+        
+        # Second box: Model
+        if self.method!='madm':
+            box.top(left="Model")
+            
+            values = [
+                format_string(self.em.features.get("binary_variable_counter",[0,0])[0],ensure_length=True), 
+                format_string(self.em.features.get("integer_variable_counter",[0,0])[0],ensure_length=True), 
+                format_string(self.em.features.get("positive_variable_counter",[0,0])[0],ensure_length=True), 
+                format_string(self.em.features.get("free_variable_counter",[0,0])[0],ensure_length=True), 
+                format_string(self.em.features.get("event_variable_counter",[0,0])[0],ensure_length=True), 
+                format_string(self.em.features.get("sequential_variable_counter",[0,0])[0],ensure_length=True), 
+                format_string(self.em.features.get("objective_counter",[0,0])[0],ensure_length=True), 
+                format_string(self.em.features.get("constraint_counter",[0,0])[0],ensure_length=True),
+                ]            
+
+            box.clear_columns(list_of_strings=["B"+" "*(len(values[0])-1), "I"+" "*(len(values[1])-1), "P"+" "*(len(values[2])-1), "F"+" "*(len(values[3])-1), "E"+" "*(len(values[4])-1), "S"+" "*(len(values[5])-1), "O"+" "*(len(values[6])-1), "C"+" "*(len(values[7])-1)], label="     ", max_space_between_elements=4)
+            box.middle()
+            box.clear_columns(list_of_strings=values, label=f"Class", max_space_between_elements=4)
+
+            values = [
+                format_string(self.em.features.get("binary_variable_counter",[0,0])[1],ensure_length=True), 
+                format_string(self.em.features.get("integer_variable_counter",[0,0])[1],ensure_length=True),
+                format_string(self.em.features.get("positive_variable_counter",[0,0])[1],ensure_length=True),  
+                format_string(self.em.features.get("free_variable_counter",[0,0])[1],ensure_length=True), 
+                format_string(self.em.features.get("event_variable_counter",[0,0])[1],ensure_length=True), 
+                format_string(self.em.features.get("sequential_variable_counter",[0,0])[1],ensure_length=True), 
+                format_string(self.em.features.get("objective_counter",[0,0])[1],ensure_length=True), 
+                format_string(self.em.features.get("constraint_counter",[0,0])[1],ensure_length=True),
+                ]
+        
+            box.clear_columns(list_of_strings=values, label=f"Size ", max_space_between_elements=4)
+            box.bottom()
+        else:
+            self.em._generate_metric_info()
+
+        # Mathematical Model
+        if full:
+            try:
+                import textwrap
+                tline_text('Math', box_width=90)
+                empty_line()
+                obdirs = 0
+                for objective in self.features['objectives']:
+                    wrapped_objective = textwrap.fill(str(objective), width=90)
+                    boxed(str(f"obj: {self.features['directions'][obdirs]} {wrapped_objective}"))
+                    obdirs += 1
+                left_align('s.t.')
+                if self.features['constraint_labels'][0] != None:
+                    for constraint in sorted(zip(self.features['constraint_labels'], self.features['constraints']), key=lambda x: x[0]):
+                        wrapped_constraint = textwrap.fill(str(constraint[1]), width=90)
+                        boxed(str(f"con {constraint[0]}: {wrapped_constraint}"))
+                else:
+                    counter = 0
+                    for constraint in self.features['constraints']:
+                        wrapped_constraint = textwrap.fill(str(constraint), width=90)
+                        boxed(str(f"con {counter}: {wrapped_constraint}"))
+                        counter += 1
+                empty_line()
+                bline()
+            except:
+                pass
+        
+            # Slack duual
+
+            tline_text("Extra")
+            empty_line()
+            try:
+                left_align("Slack:")
+                for i in self.em.features['constraint_labels']:
+                    left_align(str(i) + " = " + str(self.em.get_slack(i)))
+                empty_line()
+            except:
+                pass
+            try:
+                left_align("Dual:")
+                for i in self.em.features['constraint_labels']:
+                    left_align(str(i) + " = " + str(self.em.get_dual(i)))
+                empty_line()
+            except:
+                pass
+            bline()
+    
+
+        if self.healthy() == False:
+            tline_text("Debug")
+            empty_line()
+            try:
+                print(self.get_iis())
+            except:
+                ''
+            empty_line()
+            bline()
+                    
+        # Third box: Metrics
+        if self.method!='madm':                
+            print()
+            seconds_value = self.cpt
+            microseconds_value = seconds_value * 1e6
+            microseconds_scientific_notation = "{:.2e}".format(microseconds_value)
+            hours = int(microseconds_value // 3600e6)
+            minutes = int((microseconds_value % 3600e6) // 60e6)
+            seconds = int((microseconds_value % 60e6) / 1e6)
+            time_formatted = f"{hours:02d}:{minutes:02d}:{seconds:02d}"
+            box.top(left="Metric",right=f"{time_formatted} h:m:s" + f" {microseconds_scientific_notation} μs")
+            box.empty()
+            if self.number_of_objectives==1:
+                def show(i):
+                    return "Objective"
+            else:
+                def show(i):
+                    return f"Pareto point {i}"
+            
+            try:
+                for i in range(self.num_objective_values):
+                    k=None
+                    if skip==False:
+                        k = i
+                    else:
+                        if i%skip==0:
+                            k=i
+                    if k!=None:
+                        box.row(left= show(k), right=' '.join(format_string(j,ensure_length=True) for j in self.objective_values[k]))
+            except:
+                pass
+                            
+            box.empty()
+            box.bottom()
+            
+            # Fourth box: Decisions
+            print()
+            box.top(left="Decision")
+            try:
+                if self.method in ["constraint"]:
+                    box.empty()
+                    self.em.decision_information_print(self.em.status, 
+                                                       show_tensors=False, 
+                                                       show_detailed_tensors=False, 
+                                                       box_width=width-2)
+                    box.empty()
+                    box.bottom()
+                else:
+                    if self.number_of_objectives ==1:
+                        for key in self.solutions:
+                            box.empty()
+                            box.print_tesnor(key,self.solutions[key])
+                    else:
+                        box.empty()
+                        for i in range(self.objective_values.shape[0]):
+                            k=None
+                            if skip==False:
+                                k = i
+                            else:
+                                if i%skip==0:
+                                    k=i
+                            if k!=None:
+                                box.row(left=f"Pareto solution {k}")
+                                box.empty()
+                                for key in self.solutions[k]:
+                                    box.print_tesnor(key,self.solutions[k][key])
+                            if i!=self.objective_values.shape[0]-1:
+                                box.empty()
+                    box.empty()
+                    box.bottom()
+            except: 
+                box.empty()
+                box.empty()
+                box.bottom()
+                pass
+        else:
+            self.em.show_tensor=True
+            self.em.show_detailed_tensors=False
+            self.em.output_decimals=True
+            print()
+            self.em._generate_decision_info()
+        
+        # Benchmark
+        if self.should_benchmark:
+            print()
+            box.top(left="Benchmark")
+            box.empty()
+            box.print_pandas_df(label="Benchmark Results", df=self.ben_results[[('interface', ''), ('solver', ''), ('time', 'ave'), ('obj', 'ave')]])
+            box.empty()
+            box.bottom()
+        
+        # Sensitivity report
+        if self.sensitivity_analyzed:
+            print()
+            
+            for parameter_name in self.sensitivity_parameter_names:
+                if self.sensitivity_parameter_names.index(parameter_name)==0:
+                    box.top(left="Sensitivity")
+                
+                box.empty()
+                box.row(left=f"∞ Parameter {parameter_name}")
+                box.empty()
+                
+                for i in range(len(self.sensitivity_parameter_values[self.sensitivity_parameter_names.index(parameter_name)])):
+                    j=None
+                    if skip==False:
+                        j=i
+                    else:
+                        if i%skip ==0:
+                            j=i
+                    
+                    if j!=None:
+                        box.empty()                    
+                        
+                        seconds_value = self.sensitivity_data[f"sensitivtiy_of_cpt_to_{parameter_name}"][j]
+                        microseconds_value = seconds_value * 1e6
+                        microseconds_scientific_notation = "{:.2e}".format(microseconds_value)
+                        hours = int(microseconds_value // 3600e6)
+                        minutes = int((microseconds_value % 3600e6) // 60e6)
+                        seconds = int((microseconds_value % 60e6) / 1e6)
+                        time_formatted = f"{hours:02d}:{minutes:02d}:{seconds:02d}"
+
+                        box.empty()
+                        from colorama import init, Fore
+                        init(autoreset=True)
+                        
+                        if self.number_of_objectives==1:
+                            box.row(left=f"→ Scenario {j}", center=(f"{'√ Healthy'}" if self.sensitivity_data[f"sensitivtiy_of_health_to_{parameter_name}"][j] else f"{'X Unhealthy'}")+ f" (Objective: {format_string(self.sensitivity_data[f'sensitivtiy_of_objectives_to_{parameter_name}'][j])})", right=f"{time_formatted} h:m:s" + f" {microseconds_scientific_notation} μs")
+                        else:
+                            box.row(left=f"→ Scenario {j}", center=(f"{'√ Healthy'}" if self.sensitivity_data[f"sensitivtiy_of_health_to_{parameter_name}"][j] else f"{'X Unhealthy'}"), right=f"{time_formatted} h:m:s" + f" {microseconds_scientific_notation} μs")
+                            
+                        box.empty()
+                        for key in self.sensitivity_data[f"sensitivtiy_of_solutions_to_{parameter_name}"][j]:
+                            if key in self.key_vars:
+                                if self.number_of_objectives ==1:
+                                    box.print_tesnor(key,self.sensitivity_data[f"sensitivtiy_of_solutions_to_{parameter_name}"][j][key], "∆ " + format_string(self.sensitivity_data[f"sensitivtiy_of_similarity_to_{parameter_name}"][j][key])+"")
+                        
+                        if self.number_of_objectives !=1:
+                            for obj_id in range(self.number_of_objectives):
+                                box.print_tesnor(f"Objective {obj_id}",np.mean(self.sensitivity_data[f"sensitivtiy_of_objectives_to_{parameter_name}"][j][:,obj_id]))
+                    
+                        
+                    box.empty()
+                
+            seconds_value = self.sensitivity_end_timer - self.sensitivity_begin_timer
+            microseconds_value = seconds_value * 1e6
+            microseconds_scientific_notation = "{:.2e}".format(microseconds_value)
+            hours = int(microseconds_value // 3600e6)
+            minutes = int((microseconds_value % 3600e6) // 60e6)
+            seconds = int((microseconds_value % 60e6) / 1e6)
+            time_formatted = f"{hours:02d}:{minutes:02d}:{seconds:02d}"
+                        
+        
+            box.bottom(right=f"{time_formatted} h:m:s" + f" {microseconds_scientific_notation} μs")
+        
+            
+            
+            print()
```

### Comparing `feloopy-0.2.8/feloopy/generators/model/feloopy_model_generator.py` & `feloopy-0.2.9/feloopy/generators/model/feloopy_model_generator.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,9 @@
-'''
-+---------------------------------------------------------+
-|  Project: FelooPy (0.2.8)                               |
-|  Modified: Wednesday, 27th September 2023 09:03:26 pm   |
-|  Modified By: Keivan Tafakkori                          |
-|  Project: https://github.com/ktafakkori/feloopy         |
-|  Contact: https://www.linkedin.com/in/keivan-tafakkori/ |
-|  Copyright 2022 - 2023 Keivan Tafakkori, FELOOP         |
-+---------------------------------------------------------+
-'''
+# Copyright (c) 2022-2024, Keivan Tafakkori. All rights reserved.
+# See the file LICENSE file for licensing details.
 
 def generate_model(total_variables, directions, solver_name, solver_options):
     match solver_name:
         case 'hco':
             try:
                 from ...extras.algorithms.heuristic.HCO import HCO
             except ImportError:
```

### Comparing `feloopy-0.2.8/feloopy/generators/model/mealpy_model_generator.py` & `feloopy-0.2.9/feloopy/generators/model/mealpy_model_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,9 @@
-'''
-+---------------------------------------------------------+
-|  Project: FelooPy (0.2.8)                               |
-|  Modified: Wednesday, 27th September 2023 09:05:51 pm   |
-|  Modified By: Keivan Tafakkori                          |
-|  Project: https://github.com/ktafakkori/feloopy         |
-|  Contact: https://www.linkedin.com/in/keivan-tafakkori/ |
-|  Copyright 2022 - 2023 Keivan Tafakkori, FELOOP         |
-+---------------------------------------------------------+
-'''
+# Copyright (c) 2022-2024, Keivan Tafakkori. All rights reserved.
+# See the file LICENSE file for licensing details.
 
 def generate_model(solver_name, solver_options):
 
     module_mappings = {
 
         # Evolution-Inspired Heuristic Optimization Algorithms
         'orig-ep': ('mealpy.evolutionary_based', 'EP', 'OriginalEP'),
```

### Comparing `feloopy-0.2.8/feloopy/generators/model/niapy_model_generator.py` & `feloopy-0.2.9/feloopy/generators/model/niapy_model_generator.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,9 @@
-'''
-+---------------------------------------------------------+
-|  Project: FelooPy (0.2.8)                               |
-|  Modified: Wednesday, 27th September 2023 09:05:51 pm   |
-|  Modified By: Keivan Tafakkori                          |
-|  Project: https://github.com/ktafakkori/feloopy         |
-|  Contact: https://www.linkedin.com/in/keivan-tafakkori/ |
-|  Copyright 2022 - 2023 Keivan Tafakkori, FELOOP         |
-+---------------------------------------------------------+
-'''
+# Copyright (c) 2022-2024, Keivan Tafakkori. All rights reserved.
+# See the file LICENSE file for licensing details.
 
 def generate_model(solver_name, solver_options):
 
     module_mappings = {
 
         # Basic Heuristic Optimization Algorithms
```

### Comparing `feloopy-0.2.8/feloopy/generators/model_generator.py` & `feloopy-0.2.9/feloopy/generators/model_generator.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,19 +12,39 @@
             model_object = pulp_model_generator.generate_model(features)
 
         case 'pyomo':
 
             from .model import pyomo_model_generator
             model_object = pyomo_model_generator.generate_model(features)
 
+        case 'insideopt-demo':
+
+            from .model import seeker_model_generator
+            model_object = seeker_model_generator.generate_demo_model(features)
+
+        case 'insideopt':
+
+            from .model import seeker_model_generator
+            model_object = pyomo_model_generator.generate_model(features)
+
+        case 'gams':
+
+            from .model import gamspy_model_generator
+            model_object = gamspy_model_generator.generate_model(features)
+
         case 'ortools':
 
             from .model import ortools_model_generator
             model_object = ortools_model_generator.generate_model(features)
 
+        case 'highs':
+
+            from .model import highs_model_generator
+            model_object = highs_model_generator.generate_model(features)
+
         case 'ortools_cp':
 
             from .model import ortools_cp_model_generator
             model_object = ortools_cp_model_generator.generate_model(features)
 
         case 'gekko':
```

### Comparing `feloopy-0.2.8/feloopy/generators/result/copt_result_generator.py` & `feloopy-0.2.9/feloopy/generators/result/copt_result_generator.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.8/feloopy/generators/result/cplex_result_generator.py` & `feloopy-0.2.9/feloopy/generators/result/cplex_result_generator.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.8/feloopy/generators/result/cvxpy_result_generator.py` & `feloopy-0.2.9/feloopy/generators/result/cvxpy_result_generator.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.8/feloopy/generators/result/cylp_result_generator.py` & `feloopy-0.2.9/feloopy/generators/result/cylp_result_generator.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.8/feloopy/generators/result/gekko_result_generator.py` & `feloopy-0.2.9/feloopy/generators/result/gekko_result_generator.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.8/feloopy/generators/result/gurobi_result_generator.py` & `feloopy-0.2.9/feloopy/generators/result/gurobi_result_generator.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
 def Get(model_object, result, input1, input2=None):
     input1 = input1[0]
 
     match input1:
         case 'variable':
             return input2.X
-
+        
         case 'status':
             return gurobi_status_dict[model_object.status]
 
         case 'objective':
             return model_object.ObjVal
 
         case 'time':
```

### Comparing `feloopy-0.2.8/feloopy/generators/result/linopy_result_generator.py` & `feloopy-0.2.9/feloopy/generators/result/linopy_result_generator.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.8/feloopy/generators/result/ortools_cp_result_generator.py` & `feloopy-0.2.9/feloopy/generators/result/ortools_cp_result_generator.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.8/feloopy/generators/result/ortools_result_generator.py` & `feloopy-0.2.9/feloopy/generators/result/ortools_result_generator.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.8/feloopy/generators/result/picos_result_generator.py` & `feloopy-0.2.9/feloopy/generators/result/picos_result_generator.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.8/feloopy/generators/result/pulp_result_generator.py` & `feloopy-0.2.9/feloopy/generators/result/pulp_result_generator.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.8/feloopy/generators/result/pymprog_result_generator.py` & `feloopy-0.2.9/feloopy/generators/result/pymprog_result_generator.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.8/feloopy/generators/result/pyomo_result_generator.py` & `feloopy-0.2.9/feloopy/generators/result/pyomo_result_generator.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.8/feloopy/generators/result/rsome_dro_result_generator.py` & `feloopy-0.2.9/feloopy/generators/result/rsome_dro_result_generator.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.8/feloopy/generators/result/rsome_ro_result_generator.py` & `feloopy-0.2.9/feloopy/generators/result/rsome_ro_result_generator.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.8/feloopy/generators/result/xpress_result_generator.py` & `feloopy-0.2.9/feloopy/generators/result/xpress_result_generator.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.8/feloopy/generators/result_generator.py` & `feloopy-0.2.9/feloopy/generators/result_generator.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,14 +20,34 @@
                 return pulp_result_generator.Get(model_object, model_solution, indicator, variable_name_with_index)
 
             case 'pyomo':
 
                 from .result import pyomo_result_generator
                 return pyomo_result_generator.Get(model_object, model_solution, indicator, variable_name_with_index)
 
+            case 'insideopt':
+
+                from .result import seeker_result_generator
+                return seeker_result_generator.Get(model_object, model_solution, indicator, variable_name_with_index)
+
+            case 'gams':
+
+                from .result import gamspy_result_generator
+                return gamspy_result_generator.Get(model_object, model_solution, indicator, variable_name_with_index)
+
+            case 'highs':
+
+                from .result import highs_result_generator
+                return highs_result_generator.Get(model_object, model_solution, indicator, variable_name_with_index)
+
+            case 'insideopt-demo':
+
+                from .result import seeker_result_generator
+                return seeker_result_generator.Get(model_object, model_solution, indicator, variable_name_with_index)
+
             case 'ortools':
 
                 from .result import ortools_result_generator
                 return ortools_result_generator.Get(model_object, model_solution, indicator, variable_name_with_index)
 
             case 'ortools_cp':
 
@@ -114,14 +134,34 @@
                 return pulp_result_generator.Get(model_object, model_solution, indicator)
 
             case 'pyomo':
 
                 from .result import pyomo_result_generator
                 return pyomo_result_generator.Get(model_object, model_solution, indicator)
 
+            case 'gams':
+
+                from .result import gamspy_result_generator
+                return gamspy_result_generator.Get(model_object, model_solution, indicator)
+
+            case 'highs':
+
+                from .result import highs_result_generator
+                return highs_result_generator.Get(model_object, model_solution, indicator)
+                      
+            case 'insideopt':
+
+                from .result import seeker_result_generator
+                return seeker_result_generator.Get(model_object, model_solution, indicator)
+
+            case 'insideopt-demo':
+
+                from .result import seeker_result_generator
+                return seeker_result_generator.Get(model_object, model_solution, indicator)
+
             case 'ortools':
 
                 from .result import ortools_result_generator
                 return ortools_result_generator.Get(model_object, model_solution, indicator)
 
             case 'ortools_cp':
```

### Comparing `feloopy-0.2.8/feloopy/generators/solution/copt_solution_generator.py` & `feloopy-0.2.9/feloopy/generators/solution/copt_solution_generator.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.8/feloopy/generators/solution/cplex_cp_solution_generator.py` & `feloopy-0.2.9/feloopy/generators/solution/cplex_cp_solution_generator.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.8/feloopy/generators/solution/cplex_solution_generator.py` & `feloopy-0.2.9/feloopy/generators/solution/cplex_solution_generator.py`

 * *Files 6% similar despite different names*

```diff
@@ -83,19 +83,23 @@
                 case 'min':
                     model_object.set_objective(
                         'min', model_objectives[objective_id])
 
                 case 'max':
                     model_object.set_objective(
                         'max', model_objectives[objective_id])
-
+            
+            model_object.add_constraints(model_constraints, names=constraint_labels)
+            
+            """
             counter=0
             for constraint in model_constraints:
                 model_object.add_constraint(constraint, ctname=constraint_labels[counter])
                 counter+=1
+            """
 
             if save_model != False:
 
                 if '.lp' in save_model:
                     model_object.export_as_lp(path=save_model)
                 if '.mps' in save_model:
                     model_object.export_as_mps(path=save_model)
```

### Comparing `feloopy-0.2.8/feloopy/generators/solution/cvxpy_solution_generator.py` & `feloopy-0.2.9/feloopy/generators/solution/cvxpy_solution_generator.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.8/feloopy/generators/solution/cylp_solution_generator.py` & `feloopy-0.2.9/feloopy/generators/solution/cylp_solution_generator.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.8/feloopy/generators/solution/feloopy_solution_generator.py` & `feloopy-0.2.9/feloopy/generators/solution/feloopy_solution_generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,43 +35,44 @@
             Result[1] = Result[1].item()
             bestreward.append(best_reward)
             if directions*(Result[1]) >= directions*(best_reward_found):
                 best_agent_found = Result[0]
                 best_reward_found = Result[1]
         bestreward.pop(0)
 
-        print()
-        hour = []
-        min = []
-        sec = []
-        ave = []
-        for i in range(number_of_times):
-            tothour = round(
-                (time_solve_end[i] - time_solve_begin[i]), 3) % (24 * 3600) // 3600
-            totmin = round(
-                (time_solve_end[i] - time_solve_begin[i]), 3) % (24 * 3600) % 3600 // 60
-            totsec = round(
-                (time_solve_end[i] - time_solve_begin[i]), 3) % (24 * 3600) % 3600 % 60
-            hour.append(tothour)
-            min.append(totmin)
-            sec.append(totsec)
-            ave.append(round((time_solve_end[i]-time_solve_begin[i])*10**6))
+        if show_log:
+            print()
+            hour = []
+            min = []
+            sec = []
+            ave = []
+            for i in range(number_of_times):
+                tothour = round(
+                    (time_solve_end[i] - time_solve_begin[i]), 3) % (24 * 3600) // 3600
+                totmin = round(
+                    (time_solve_end[i] - time_solve_begin[i]), 3) % (24 * 3600) % 3600 // 60
+                totsec = round(
+                    (time_solve_end[i] - time_solve_begin[i]), 3) % (24 * 3600) % 3600 % 60
+                hour.append(tothour)
+                min.append(totmin)
+                sec.append(totsec)
+                ave.append(round((time_solve_end[i]-time_solve_begin[i])*10**6))
 
-        print("~~~~~~~\nTIME INFO\n~~~~~~~")
-        print(tb({
-            "cpt (ave)": [np.average(ave), "%02d:%02d:%02d" % (np.average(hour), np.average(min), np.average(sec))],
-            "cpt (std)": [np.std(ave), "%02d:%02d:%02d" % (np.std(hour), np.std(min), np.std(sec))],
-            "unit": ["micro sec", "h:m:s"]
-        }, headers="keys", tablefmt="github"))
-        print()
+            print("~~~~~~~\nTIME INFO\n~~~~~~~")
+            print(tb({
+                "cpt (ave)": [np.average(ave), "%02d:%02d:%02d" % (np.average(hour), np.average(min), np.average(sec))],
+                "cpt (std)": [np.std(ave), "%02d:%02d:%02d" % (np.std(hour), np.std(min), np.std(sec))],
+                "unit": ["micro sec", "h:m:s"]
+            }, headers="keys", tablefmt="github"))
+            print()
 
-        print("~~~~~~~\nOBJ INFO\n~~~~~~~")
-        print(tb({
-            "obj": [np.max(bestreward), np.average(bestreward), np.std(bestreward), np.min(bestreward)],
-            "unit": ["max", "average", "standard deviation", "min"]
-        }, headers="keys", tablefmt="github"))
-        print("~~~~~~~")
+            print("~~~~~~~\nOBJ INFO\n~~~~~~~")
+            print(tb({
+                "obj": [np.max(bestreward), np.average(bestreward), np.std(bestreward), np.min(bestreward)],
+                "unit": ["max", "average", "standard deviation", "min"]
+            }, headers="keys", tablefmt="github"))
+            print("~~~~~~~")
 
         best_agent = best_agent_found
         best_reward = best_reward_found
 
     return best_agent, best_reward, np.average(time_solve_begin), np.average(time_solve_end), status
```

### Comparing `feloopy-0.2.8/feloopy/generators/solution/gekko_solution_generator.py` & `feloopy-0.2.9/feloopy/generators/solution/gekko_solution_generator.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.8/feloopy/generators/solution/gurobi_solution_generator.py` & `feloopy-0.2.9/feloopy/generators/solution/gurobi_solution_generator.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,14 +75,15 @@
             for constraint, label in zip(model_constraints, constraint_labels):
                 if label:
                     model_object.addConstr(constraint, name=label)
                 else:
                     model_object.addConstr(constraint)
                 counter += 1
 
+            
             if save_model != False:
                 model_object.write(save_model)
 
             time_solve_begin = timeit.default_timer()
             result = model_object.optimize()
             time_solve_end = timeit.default_timer()
             generated_solution = result, [time_solve_begin, time_solve_end]
```

### Comparing `feloopy-0.2.8/feloopy/generators/solution/linopy_solution_generator.py` & `feloopy-0.2.9/feloopy/generators/solution/linopy_solution_generator.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 # Copyright (c) 2022-2024, Keivan Tafakkori. All rights reserved.
 # See the file LICENSE file for licensing details.
 
-
-
 from linopy import Model as LINOPYMODEL
 from linopy import LinearExpression
 import timeit
 
 linopy_solver_selector = {'cbc': 'cbc',
                           'glpk': 'glpk',
                           'highs': 'highs',
                           'gurobi': 'gurobi',
                           'xpress': 'xpress',
-                          'cplex': 'cplex'}
-
+                          'cplex': 'cplex',
+                          'copt', 'copt'}
 
 def generate_solution(features):
 
     model_object = features['model_object_before_solve']
     model_objectives = features['objectives']
     model_constraints = features['constraints']
     directions = features['directions']
@@ -31,34 +29,23 @@
     objective_id = features['objective_being_optimized']
     log = features['log']
     save = features['save_solver_log']
     save_model = features['write_model_file']
     email = features['email_address']
     max_iterations = features['max_iterations']
     solver_options = features['solver_options']
-
+    
     if solver_name not in linopy_solver_selector.keys():
-        raise RuntimeError(
-            "Using solver '%s' is not supported by 'linopy'! \nPossible fixes: \n1) Check the solver name. \n2) Use another interface. \n" % (solver_name))
-
+        raise RuntimeError("Using solver '%s' is not supported by 'linopy'! \nPossible fixes: \n1) Check the solver name. \n2) Use another interface. \n" % (solver_name))
     match debug:
-
         case False:
-
             match directions[objective_id]:
                 case "min":
-                    print(model_objectives[objective_id])
-                    print(type(model_objectives[objective_id]))
                     model_object.add_objective(model_objectives[objective_id])
-                    
                 case "max":
                     model_object.add_objective(-1*model_objectives[objective_id])
-
-            for constraint in model_constraints:
-                model_object.add_constraint(constraint)
-
+            for constraint in model_constraints: model_object.add_constraint(constraint)
             time_solve_begin = timeit.default_timer()
             result = model_object.solve(solver_name=solver_name)
             time_solve_end = timeit.default_timer()
             generated_solution = [result, [time_solve_begin, time_solve_end]]
-
     return generated_solution
```

### Comparing `feloopy-0.2.8/feloopy/generators/solution/mealpy_solution_generator.py` & `feloopy-0.2.9/feloopy/generators/solution/mealpy_solution_generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,16 +17,15 @@
         "log_to": "console" if show_log else None,
         "save_population": False,
     }
     if solver_options.get("mode", None)!=None:
 
         termination={
             "mode": solver_options.get("mode", "MG"), 
-            "quantity": solver_options.get("quantity", 100)
-            }
+            "quantity": solver_options.get("quantity", 100)}
 
     else:
         termination=None
         
     if number_of_times == 1:
         
         if solver_options.get("process_mode")!=None:
@@ -80,43 +79,44 @@
             Result[1] = Result[1].item()
             bestreward.append(best_reward)
             if directions*(Result[1]) >= directions*(best_reward_found):
                 best_agent_found = Result[0]
                 best_reward_found = Result[1]
         bestreward.pop(0)
 
-        print()
-        hour = []
-        min = []
-        sec = []
-        ave = []
-        for i in range(number_of_times):
-            tothour = round(
-                (time_solve_end[i] - time_solve_begin[i]), 3) % (24 * 3600) // 3600
-            totmin = round(
-                (time_solve_end[i] - time_solve_begin[i]), 3) % (24 * 3600) % 3600 // 60
-            totsec = round(
-                (time_solve_end[i] - time_solve_begin[i]), 3) % (24 * 3600) % 3600 % 60
-            hour.append(tothour)
-            min.append(totmin)
-            sec.append(totsec)
-            ave.append(round((time_solve_end[i]-time_solve_begin[i])*10**6))
-
-        print("~~~~~~~\nTIME INFO\n~~~~~~~")
-        print(tb({
-            "cpt (ave)": [np.average(ave), "%02d:%02d:%02d" % (np.average(hour), np.average(min), np.average(sec))],
-            "cpt (std)": [np.std(ave), "%02d:%02d:%02d" % (np.std(hour), np.std(min), np.std(sec))],
-            "unit": ["micro sec", "h:m:s"]
-        }, headers="keys", tablefmt="github"))
-        print("~~~~~~~")
-
-        print("~~~~~~~\nOBJ INFO\n~~~~~~~")
-        print(tb({
-            "obj": [np.max(bestreward), np.average(bestreward), np.std(bestreward), np.min(bestreward)],
-            "unit": ["max", "average", "standard deviation", "min"]
-        }, headers="keys", tablefmt="github"))
-        print("~~~~~~~")
+        if show_log:
+            print()
+            hour = []
+            min = []
+            sec = []
+            ave = []
+            for i in range(number_of_times):
+                tothour = round(
+                    (time_solve_end[i] - time_solve_begin[i]), 3) % (24 * 3600) // 3600
+                totmin = round(
+                    (time_solve_end[i] - time_solve_begin[i]), 3) % (24 * 3600) % 3600 // 60
+                totsec = round(
+                    (time_solve_end[i] - time_solve_begin[i]), 3) % (24 * 3600) % 3600 % 60
+                hour.append(tothour)
+                min.append(totmin)
+                sec.append(totsec)
+                ave.append(round((time_solve_end[i]-time_solve_begin[i])*10**6))
+
+            print("~~~~~~~\nTIME INFO\n~~~~~~~")
+            print(tb({
+                "cpt (ave)": [np.average(ave), "%02d:%02d:%02d" % (np.average(hour), np.average(min), np.average(sec))],
+                "cpt (std)": [np.std(ave), "%02d:%02d:%02d" % (np.std(hour), np.std(min), np.std(sec))],
+                "unit": ["micro sec", "h:m:s"]
+            }, headers="keys", tablefmt="github"))
+            print("~~~~~~~")
+
+            print("~~~~~~~\nOBJ INFO\n~~~~~~~")
+            print(tb({
+                "obj": [np.max(bestreward), np.average(bestreward), np.std(bestreward), np.min(bestreward)],
+                "unit": ["max", "average", "standard deviation", "min"]
+            }, headers="keys", tablefmt="github"))
+            print("~~~~~~~")
 
         best_agent = best_agent_found
         best_reward = best_reward_found
 
     return best_agent, best_reward, time_solve_begin, time_solve_end
```

### Comparing `feloopy-0.2.8/feloopy/generators/solution/mip_solution_generator.py` & `feloopy-0.2.9/feloopy/generators/solution/mip_solution_generator.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.8/feloopy/generators/solution/niapy_solution_generator.py` & `feloopy-0.2.9/feloopy/generators/solution/niapy_solution_generator.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.8/feloopy/generators/solution/ortools_cp_solution_generator.py` & `feloopy-0.2.9/feloopy/generators/solution/ortools_cp_solution_generator.py`

 * *Files 6% similar despite different names*

```diff
@@ -61,15 +61,21 @@
             for constraint in model_constraints:
                 model_object.Add(constraint)
 
             solver = cp_model.CpSolver()
 
             if time_limit != None:
                 solver.parameters.max_time_in_seconds = time_limit
-
+                
+            if 'enumerate' in solver_options.keys():
+                if solver_options['enumerate']:
+                    solver.parameters.enumerate_all_solutions = True
+                else:
+                    solver.parameters.enumerate_all_solutions = False
+                    
             time_solve_begin = timeit.default_timer()
             result = solver.Solve(model_object)
             time_solve_end = timeit.default_timer()
             generated_solution = [[result, solver],
                                   [time_solve_begin, time_solve_end]]
 
             if log:
```

### Comparing `feloopy-0.2.8/feloopy/generators/solution/ortools_solution_generator.py` & `feloopy-0.2.9/feloopy/generators/solution/ortools_solution_generator.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.8/feloopy/generators/solution/picos_solution_generator.py` & `feloopy-0.2.9/feloopy/generators/solution/picos_solution_generator.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.8/feloopy/generators/solution/pulp_solution_generator.py` & `feloopy-0.2.9/feloopy/generators/solution/rsome_ro_solution_generator.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,16 +1,12 @@
 # Copyright (c) 2022-2024, Keivan Tafakkori. All rights reserved.
 # See the file LICENSE file for licensing details.
 
-
-import pulp as pulp_interface
-
 import timeit
 
-
 def generate_solution(features):
 
     model_object = features['model_object_before_solve']
     model_objectives = features['objectives']
     model_constraints = features['constraints']
     directions = features['directions']
     constraint_labels = features['constraint_labels']
@@ -23,76 +19,82 @@
     objective_id = features['objective_being_optimized']
     log = features['log']
     save = features['save_solver_log']
     save_model = features['write_model_file']
     email = features['email_address']
     max_iterations = features['max_iterations']
     solver_options = features['solver_options']
-
-    if time_limit != None:
-        solver_options['timeLimit'] = time_limit
-
-    if thread_count != None:
-        solver_options['threads'] = thread_count
-
-    if relative_gap != None:
-        solver_options['gapRel'] = relative_gap
-
-    if absolute_gap != None:
-        solver_options['gapAbs'] = absolute_gap
+    obj_operators = features['obj_operators']
 
     if log:
-        solver_options['msg'] = 1
+        display=True
     else:
-        solver_options['msg'] = 0
-
-    if max_iterations != None:
-        "None"
-
-    pulp_solver_selector = {
-        'cbc': pulp_interface.PULP_CBC_CMD(**solver_options),
-        'choco': pulp_interface.CHOCO_CMD(**solver_options),
-        'coin': pulp_interface.COIN_CMD(**solver_options),
-        'coinmp_dll': pulp_interface.COINMP_DLL(**solver_options),
-        'cplex_py': pulp_interface.CPLEX_PY(**solver_options),
-        'cplex': pulp_interface.CPLEX_CMD(**solver_options),
-        'glpk': pulp_interface.GLPK_CMD(**solver_options),
-        'gurobi_cmd': pulp_interface.GUROBI_CMD(**solver_options),
-        'gurobi': pulp_interface.GUROBI(**solver_options),
-        'highs': pulp_interface.HiGHS_CMD(**solver_options),
-        'mipcl': pulp_interface.MIPCL_CMD(**solver_options),
-        'mosek': pulp_interface.MOSEK(**solver_options),
-        'pyglpk': pulp_interface.PYGLPK(**solver_options),
-        'scip': pulp_interface.SCIP_CMD(**solver_options),
-        'xpress_py': pulp_interface.XPRESS_PY(**solver_options),
-        'xpress': pulp_interface.XPRESS(**solver_options)
-    }
+        display=False
 
-    if solver_name not in pulp_solver_selector.keys():
+    if solver_name =='scipy':
+        from rsome import lpg_solver
+        solver = lpg_solver
+    
+    elif solver_name == 'cylp':
+        from rsome import clp_solver
+        solver = clp_solver
+    
+    elif solver_name == 'ortools':
+        from rsome import ort_solver
+        solver = ort_solver
+    
+    elif solver_name == 'ecos':
+        from rsome import eco_solver
+        solver = eco_solver
+
+    elif solver_name == 'gurobi':
+        from rsome import grb_solver
+        solver = grb_solver
+    
+    elif solver_name == 'cplex':
+        from rsome import cpx_solver
+        solver = cpx_solver
+    
+    elif solver_name == 'mosek':
+        from rsome import msk_solver
+        solver = msk_solver
+    
+    elif solver_name =='copt':
+        from rsome import cpt_solver
+        solver = cpt_solver
+
+    elif solver_name =='cvxpy':
+        from rsome import cvx_solver
+        solver = cvx_solver
+        
+    else:
         raise RuntimeError(
-            "Using solver '%s' is not supported by 'pulp'! \nPossible fixes: \n1) Check the solver name. \n2) Use another interface. \n" % (solver_name))
+            "Using solver '%s' is not supported by 'rsome_ro'! \nPossible fixes: \n1) Check the solver name. \n2) Use another interface. \n" % (solver_name))
 
     match debug:
 
         case False:
 
             match directions[objective_id]:
 
                 case "min":
-                    model_object += model_objectives[objective_id]
-
+                    if len(obj_operators)==0:                    
+                        model_object.min(model_objectives[objective_id])
+                    elif obj_operators[objective_id] == 'max':
+                        model_object.minmax(*model_objectives[objective_id])
                 case "max":
-                    model_object += -model_objectives[objective_id]
+                    if len(obj_operators)==0:
+                        model_object.max(model_objectives[objective_id])
+                    
+                    elif obj_operators[objective_id] == 'min':
+                        model_object.maxmin(*model_objectives[objective_id])
 
-            if len(model_constraints)!=0:
-                counter = 0
-                for constraint in model_constraints:
-                    model_object += (constraint, constraint_labels[counter])
-                    counter+=1
+            for constraint in model_constraints:
+                model_object.st(constraint)
 
             time_solve_begin = timeit.default_timer()
-            result = model_object.solve(
-                solver=pulp_solver_selector[solver_name])
+            result = model_object.solve(solver,display,solver_options)
             time_solve_end = timeit.default_timer()
             generated_solution = [result, [time_solve_begin, time_solve_end]]
 
     return generated_solution
+
```

### Comparing `feloopy-0.2.8/feloopy/generators/solution/pygad_solution_generator.py` & `feloopy-0.2.9/feloopy/generators/solution/pygad_solution_generator.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.8/feloopy/generators/solution/pymoo_solution_generator.py` & `feloopy-0.2.9/feloopy/generators/solution/pymoo_solution_generator.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.8/feloopy/generators/solution/pymprog_solution_generator.py` & `feloopy-0.2.9/feloopy/generators/solution/pymprog_solution_generator.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,14 +32,15 @@
     if log:
 
         ""
 
     else:
 
         msg_lev = pymprog_interface.glpk.GLP_MSG_OFF
+        
 
     if time_limit != None:
         tmlim = time_limit
     else:
         tmlim= None
 
     if solver_name not in pymprog_solver_selector.keys():
```

### Comparing `feloopy-0.2.8/feloopy/generators/solution/pymultiobjective_solution_generator.py` & `feloopy-0.2.9/feloopy/generators/solution/pymultiobjective_solution_generator.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.8/feloopy/generators/solution/pyomo_solution_generator.py` & `feloopy-0.2.9/feloopy/generators/solution/pyomo_solution_generator.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.8/feloopy/generators/solution/rsome_dro_solution_generator.py` & `feloopy-0.2.9/feloopy/generators/solution/rsome_dro_solution_generator.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.8/feloopy/generators/solution/rsome_ro_solution_generator.py` & `feloopy-0.2.9/feloopy/generators/solution/highs_solution_generator.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 # Copyright (c) 2022-2024, Keivan Tafakkori. All rights reserved.
 # See the file LICENSE file for licensing details.
 
+
+import highspy as highs_interface
 import timeit
 
+highs_solver_selector = {'highs': 'highs'}
+
 def generate_solution(features):
 
     model_object = features['model_object_before_solve']
     model_objectives = features['objectives']
     model_constraints = features['constraints']
     directions = features['directions']
     constraint_labels = features['constraint_labels']
@@ -19,82 +23,38 @@
     objective_id = features['objective_being_optimized']
     log = features['log']
     save = features['save_solver_log']
     save_model = features['write_model_file']
     email = features['email_address']
     max_iterations = features['max_iterations']
     solver_options = features['solver_options']
-    obj_operators = features['obj_operators']
 
-    if log:
-        display=True
-    else:
-        display=False
-
-    if solver_name =='scipy':
-        from rsome import lpg_solver
-        solver = lpg_solver
-    
-    elif solver_name == 'cylp':
-        from rsome import clp_solver
-        solver = clp_solver
-    
-    elif solver_name == 'ortools':
-        from rsome import ort_solver
-        solver = ort_solver
-    
-    elif solver_name == 'ecos':
-        from rsome import eco_solver
-        solver = eco_solver
-
-    elif solver_name == 'gurobi':
-        from rsome import grb_solver
-        solver = grb_solver
-    
-    elif solver_name == 'cplex':
-        from rsome import cpx_solver
-        solver = cpx_solver
-    
-    elif solver_name == 'mosek':
-        from rsome import msk_solver
-        solver = msk_solver
-    
-    elif solver_name =='copt':
-        from rsome import cpt_solver
-        solver = cpt_solver
-
-    elif solver_name =='cvxpy':
-        from rsome import cvx_solver
-        solver = cvx_solver
-        
-    else:
+    if solver_name not in highs_solver_selector.keys():
+
         raise RuntimeError(
-            "Using solver '%s' is not supported by 'rsome_ro'! \nPossible fixes: \n1) Check the solver name. \n2) Use another interface. \n" % (solver_name))
+            "Using solver '%s' is not supported by 'highs'! \nPossible fixes: \n1) Check the solver name. \n2) Use another interface. \n" % (solver_name))
 
     match debug:
 
         case False:
 
-            match directions[objective_id]:
+            counter = 0
+            for constraint, label in zip(model_constraints, constraint_labels):
+                if label:
+                    model_object.addConstr(constraint, name=label)
+                else:
+                    model_object.addConstr(constraint)
+                counter += 1
 
+            match directions[objective_id]:
                 case "min":
-                    if len(obj_operators)==0:                    
-                        model_object.min(model_objectives[objective_id])
-                    elif obj_operators[objective_id] == 'max':
-                        model_object.minmax(*model_objectives[objective_id])
+                    time_solve_begin = timeit.default_timer()
+                    result = model_object.minimize(model_objectives[objective_id])
+                    time_solve_end = timeit.default_timer()
                 case "max":
-                    if len(obj_operators)==0:
-                        model_object.max(model_objectives[objective_id])
-                    
-                    elif obj_operators[objective_id] == 'min':
-                        model_object.maxmin(*model_objectives[objective_id])
-
-            for constraint in model_constraints:
-                model_object.st(constraint)
-
-            time_solve_begin = timeit.default_timer()
-            result = model_object.solve(solver,display,solver_options)
-            time_solve_end = timeit.default_timer()
-            generated_solution = [result, [time_solve_begin, time_solve_end]]
+                    time_solve_begin = timeit.default_timer()
+                    result = model_object.maximize(model_objectives[objective_id])
+                    time_solve_end = timeit.default_timer()
+            
+            generated_solution = result, [time_solve_begin, time_solve_end]
 
     return generated_solution
-
```

### Comparing `feloopy-0.2.8/feloopy/generators/solution/xpress_solution_generator.py` & `feloopy-0.2.9/feloopy/generators/solution/xpress_solution_generator.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.8/feloopy/generators/solution_generator.py` & `feloopy-0.2.9/feloopy/generators/solution_generator.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,14 +13,34 @@
 
         case 'pyomo':
 
             from .solution import pyomo_solution_generator
             ModelSolution = pyomo_solution_generator.generate_solution(
                 features)
 
+        case 'insideopt':
+
+            from .solution import seeker_solution_generator
+            ModelSolution = seeker_solution_generator.generate_solution(features)
+
+        case 'insideopt-demo':
+
+            from .solution import seeker_solution_generator
+            ModelSolution = seeker_solution_generator.generate_solution(features)
+
+        case 'gams':
+
+            from .solution import gamspy_solution_generator
+            ModelSolution = gamspy_solution_generator.generate_solution(features)
+
+        case 'highs':
+
+            from .solution import highs_solution_generator
+            ModelSolution = highs_solution_generator.generate_solution(features)
+                                                   
         case 'ortools':
 
             from .solution import ortools_solution_generator
             ModelSolution = ortools_solution_generator.generate_solution(
                 features)
 
         case 'ortools_cp':
```

### Comparing `feloopy-0.2.8/feloopy/generators/variable/copt_variable_generator.py` & `feloopy-0.2.9/feloopy/generators/variable/copt_variable_generator.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.8/feloopy/generators/variable/cplex_cp_variable_generator.py` & `feloopy-0.2.9/feloopy/generators/variable/cplex_cp_variable_generator.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.8/feloopy/generators/variable/cplex_variable_generator.py` & `feloopy-0.2.9/feloopy/generators/variable/cplex_variable_generator.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # Copyright (c) 2022-2024, Keivan Tafakkori. All rights reserved.
 # See the file LICENSE file for licensing details.
 
 
-
 import cplex
 import itertools as it
 
 sets = it.product
 
 
 def generate_variable(model_object, variable_type, variable_name, variable_bound, variable_dim=0):
```

### Comparing `feloopy-0.2.8/feloopy/generators/variable/cvxpy_variable_generator.py` & `feloopy-0.2.9/feloopy/generators/variable/cvxpy_variable_generator.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,29 +19,29 @@
                 if len(variable_dim) == 1:
                     generated_variable = {key: VariableGenerator(1, integer=False, nonneg=True, name=f"{variable_name}_{key}") for key in variable_dim[0]}
                 else:
                     generated_variable = {key: VariableGenerator(1, integer=False, nonneg=True, name=f"{variable_name}_{key}") for key in sets(*variable_dim)}
 
         case 'bvar':
             if variable_dim == 0:
-                generated_variable = VariableGenerator(1, nonneg=True, integer=True, name=variable_name)
+                generated_variable = VariableGenerator(1, integer=True, name=variable_name)
             else:
                 if len(variable_dim) == 1:
-                    generated_variable = {key: VariableGenerator(1, integer=True, nonneg=True, name=f"{variable_name}_{key}") for key in variable_dim[0]}
+                    generated_variable = {key: VariableGenerator(1, integer=True, name=f"{variable_name}_{key}") for key in variable_dim[0]}
                 else:
-                    generated_variable = {key: VariableGenerator(1, integer=True, nonneg=True, name=f"{variable_name}_{key}") for key in sets(*variable_dim)}
+                    generated_variable = {key: VariableGenerator(1, integer=True, name=f"{variable_name}_{key}") for key in sets(*variable_dim)}
 
         case 'ivar':
             if variable_dim == 0:
-                generated_variable = VariableGenerator(1, nonneg=True, integer=True, name=variable_name)
+                generated_variable = VariableGenerator(1, integer=True, name=variable_name)
             else:
                 if len(variable_dim) == 1:
-                    generated_variable = {key: VariableGenerator(1, nonneg=True, integer=True, name=f"{variable_name}_{key}") for key in variable_dim[0]}
+                    generated_variable = {key: VariableGenerator(1, integer=True, name=f"{variable_name}_{key}") for key in variable_dim[0]}
                 else:
-                    generated_variable = {key: VariableGenerator(1, nonneg=True, integer=True, name=f"{variable_name}_{key}") for key in sets(*variable_dim)}
+                    generated_variable = {key: VariableGenerator(1, integer=True, name=f"{variable_name}_{key}") for key in sets(*variable_dim)}
 
         case 'fvar':
             if variable_dim == 0:
                 generated_variable = VariableGenerator(1, integer=False, nonneg=False, name=variable_name)
             else:
                 if len(variable_dim) == 1:
                     generated_variable = {key: VariableGenerator(1, integer=False, nonneg=False, name=f"{variable_name}_{key}") for key in variable_dim[0]}
@@ -61,20 +61,20 @@
                 generated_variable = VariableGenerator(1, integer=False, nonneg=True, name=variable_name)
             else:
                 dims = tuple(len(dim) for dim in variable_dim)
                 generated_variable = VariableGenerator(dims, integer=False, nonneg=True, name=variable_name)
 
         case 'itvar':
             if variable_dim ==0:
-                generated_variable = VariableGenerator(1, nonneg=True, integer=True, name=variable_name)
+                generated_variable = VariableGenerator(1, integer=True, name=variable_name)
             else:
                 dims = tuple(len(dim) for dim in variable_dim)
-                generated_variable = VariableGenerator(dims, integer=True, nonneg=True, name=variable_name)
+                generated_variable = VariableGenerator(dims, integer=True, name=variable_name)
 
         case 'btvar':
             if variable_dim ==0:
-                generated_variable = VariableGenerator(1, nonneg=True, integer=True, name=variable_name)
+                generated_variable = VariableGenerator(1, integer=True, name=variable_name)
             else:
                 dims = tuple(len(dim) for dim in variable_dim)
-                generated_variable = VariableGenerator(dims, integer=True, nonneg=True, name=variable_name)
+                generated_variable = VariableGenerator(dims, integer=True, name=variable_name)
 
     return generated_variable
```

### Comparing `feloopy-0.2.8/feloopy/generators/variable/cylp_variable_generator.py` & `feloopy-0.2.9/feloopy/generators/variable/cylp_variable_generator.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.8/feloopy/generators/variable/gekko_variable_generator.py` & `feloopy-0.2.9/feloopy/generators/variable/gekko_variable_generator.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.8/feloopy/generators/variable/gurobi_variable_generator.py` & `feloopy-0.2.9/feloopy/generators/variable/gurobi_variable_generator.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.8/feloopy/generators/variable/linopy_variable_generator.py` & `feloopy-0.2.9/feloopy/generators/variable/linopy_variable_generator.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,56 +1,58 @@
 # Copyright (c) 2022-2024, Keivan Tafakkori. All rights reserved.
 # See the file LICENSE file for licensing details.
 
 
 import itertools as it
 import pandas as pd
+import numpy as np
 
 def generate_variable(model_object, variable_type, variable_name, variable_bound, variable_dim=0):
 
     match variable_type:
 
         case 'pvar':
-
+            
+            if variable_bound[0] == None: variable_bound[0]=0
+            if variable_bound[1] == None: variable_bound[1]=np.inf
             if variable_dim == 0:
-                GeneratedVariable = model_object.add_variables(
-                    lower=variable_bound[0], upper=variable_bound[1], name=variable_name)
+                GeneratedVariable = model_object.add_variables(lower=variable_bound[0], upper=variable_bound[1], name=variable_name)
             else:
-                GeneratedVariable = model_object.add_variables(
-                    lower=variable_bound[0], upper=variable_bound[1], coords=pd.Index(variable_dim), name=variable_name)
+                GeneratedVariable = model_object.add_variables(lower=variable_bound[0], upper=variable_bound[1], coords=pd.Index(variable_dim), name=variable_name)
 
         case 'bvar':
-
+            if variable_bound[0] == None: variable_bound[0]=0
+            if variable_bound[1] == None: variable_bound[1]=1
+            
             if variable_dim == 0:
-                GeneratedVariable = model_object.add_variables(
-                    name=variable_name, binary=True)
+                GeneratedVariable = model_object.add_variables(name=variable_name, binary=True)
             else:
-                GeneratedVariable = model_object.add_variables(
-                    coords=pd.Index(variable_dim), name=variable_name, binary=True)
+                GeneratedVariable = model_object.add_variables(coords=pd.Index(variable_dim), name=variable_name, binary=True)
 
         case 'ivar':
-
+            if variable_bound[0] == None: variable_bound[0]=0
+            if variable_bound[1] == None: variable_bound[1]=np.inf
             if variable_dim == 0:
-                GeneratedVariable = model_object.add_variables(
-                    lower=variable_bound[0], upper=variable_bound[1], name=variable_name, binary=True)
+                GeneratedVariable = model_object.add_variables(lower=variable_bound[0], upper=variable_bound[1], name=variable_name, binary=True)
             else:
-                GeneratedVariable = model_object.add_variables(
-                    lower=variable_bound[0], upper=variable_bound[1], coords=pd.Index(variable_dim), name=variable_name, integer=True)
+                GeneratedVariable = model_object.add_variables(lower=variable_bound[0], upper=variable_bound[1], coords=pd.Index(variable_dim), name=variable_name, integer=True)
 
         case 'fvar':
 
+            if variable_bound[0] == None: variable_bound[0]=-np.inf
+            if variable_bound[1] == None: variable_bound[1]=np.inf
+            
             if variable_dim == 0:
-                GeneratedVariable = model_object.add_variables(
-                    lower=variable_bound[0], upper=variable_bound[1], name=variable_name)
+                GeneratedVariable = model_object.add_variables(lower=variable_bound[0], upper=variable_bound[1], name=variable_name)
             else:
-                GeneratedVariable = model_object.add_variables(
-                    lower=variable_bound[0], upper=variable_bound[1], coords=pd.Index(variable_dim), name=variable_name)
+                GeneratedVariable = model_object.add_variables(lower=variable_bound[0], upper=variable_bound[1], coords=pd.Index(variable_dim), name=variable_name)
 
         case 'ptvar':
-
+            
+            
             if variable_dim == 0:
                 GeneratedVariable = model_object.add_variables(
                     lower=variable_bound[0], upper=variable_bound[1], name=variable_name, positive=True)
             else:
                 GeneratedVariable = model_object.add_variables(
                     lower=variable_bound[0], upper=variable_bound[1], coords=pd.Index(variable_dim), name=variable_name, positive=True)
```

### Comparing `feloopy-0.2.8/feloopy/generators/variable/localsolver_variable_generator.py` & `feloopy-0.2.9/feloopy/generators/variable/ortools_variable_generator.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,67 +1,141 @@
-'''
-+---------------------------------------------------------+
-|  Project: FelooPy (0.2.8)                               |
-|  Modified: Wednesday, 27th September 2023 11:35:18 pm   |
-|  Modified By: Keivan Tafakkori                          |
-|  Project: https://github.com/ktafakkori/feloopy         |
-|  Contact: https://www.linkedin.com/in/keivan-tafakkori/ |
-|  Copyright 2022 - 2023 Keivan Tafakkori, FELOOP         |
-+---------------------------------------------------------+
-'''
+# Copyright (c) 2022-2024, Keivan Tafakkori. All rights reserved.
+# See the file LICENSE file for licensing details.
+
+
 
-import localsolver as ls
 import itertools as it
 
 sets = it.product
 
+
 def generate_variable(model_object, variable_type, variable_name, variable_bound, variable_dim=0):
+
+    if variable_bound[0] == None:
+        variable_bound[0] = -model_object.infinity()
+
+    if variable_bound[1] == None:
+        variable_bound[1] = model_object.infinity()
+
     match variable_type:
+
         case 'pvar':
+
             '''
+
             Positive Variable Generator
+
+
             '''
+
             if variable_dim == 0:
-                GeneratedVariable = model_object.Float(
-                    variable_bound[0], variable_bound[1], name=variable_name)
+
+                GeneratedVariable = model_object.NumVar(
+                    variable_bound[0], variable_bound[1], variable_name)
+
             else:
-                GeneratedVariable = generate_multi_dimensional_var(model_object, variable_bound, variable_name, variable_dim, 'Float')
-                
+
+                if len(variable_dim) == 1:
+
+                    GeneratedVariable = {key: model_object.NumVar(
+                        variable_bound[0], variable_bound[1], f"{variable_name}{key}") for key in variable_dim[0]}
+
+                else:
+
+                    GeneratedVariable = {key: model_object.NumVar(
+                        variable_bound[0], variable_bound[1], f"{variable_name}{key}") for key in it.product(*variable_dim)}
+
         case 'bvar':
+
             '''
+
             Binary Variable Generator
+
+
             '''
+
             if variable_dim == 0:
-                GeneratedVariable = model_object.Bool(name=variable_name)
+
+                GeneratedVariable = model_object.IntVar(
+                    variable_bound[0], variable_bound[1], variable_name)
+
             else:
-                GeneratedVariable = generate_multi_dimensional_var(model_object, variable_bound, variable_name, variable_dim, 'Bool')
+
+                if len(variable_dim) == 1:
+
+                    GeneratedVariable = {key: model_object.IntVar(
+                        variable_bound[0], variable_bound[1], f"{variable_name}{key}") for key in variable_dim[0]}
+
+                else:
+
+                    GeneratedVariable = {key: model_object.IntVar(
+                        variable_bound[0], variable_bound[1], f"{variable_name}{key}") for key in it.product(*variable_dim)}
 
         case 'ivar':
+
             '''
+
             Integer Variable Generator
+
+
             '''
+
+            if variable_bound[0] == 0:
+
+                variable_bound[0] = 0
+
+            if variable_bound[1] == None:
+
+                variable_bound[1] = model_object.infinity()
+
             if variable_dim == 0:
-                GeneratedVariable = model_object.Int(
-                    variable_bound[0], variable_bound[1], name=variable_name)
+
+                GeneratedVariable = model_object.IntVar(
+                    variable_bound[0], variable_bound[1], variable_name)
+
             else:
-                GeneratedVariable = generate_multi_dimensional_var(model_object, variable_bound, variable_name, variable_dim, 'Int')
+
+                if len(variable_dim) == 1:
+
+                    GeneratedVariable = {key: model_object.IntVar(
+                        variable_bound[0], variable_bound[1], f"{variable_name}{key}") for key in variable_dim[0]}
+
+                else:
+
+                    GeneratedVariable = {key: model_object.IntVar(
+                        variable_bound[0], variable_bound[1], f"{variable_name}{key}") for key in it.product(*variable_dim)}
 
         case 'fvar':
+
             '''
+
             Free Variable Generator
+
+
             '''
+
+            if variable_bound[0] == None:
+
+                variable_bound[0] = -model_object.infinity()
+
+            if variable_bound[1] == None:
+
+                variable_bound[1] = model_object.infinity()
+
             if variable_dim == 0:
-                GeneratedVariable = model_object.Float(
-                    variable_bound[0], variable_bound[1], name=variable_name)
+
+                GeneratedVariable = model_object.NumVar(
+                    variable_bound[0], variable_bound[1], variable_name)
+
             else:
-                GeneratedVariable = generate_multi_dimensional_var(model_object, variable_bound, variable_name, variable_dim, 'Float')
 
-    return GeneratedVariable
+                if len(variable_dim) == 1:
+
+                    GeneratedVariable = {key: model_object.NumVar(
+                        variable_bound[0], variable_bound[1], f"{variable_name}{key}") for key in variable_dim[0]}
+
+                else:
+
+                    GeneratedVariable = {key: model_object.NumVar(
+                        variable_bound[0], variable_bound[1], f"{variable_name}{key}") for key in it.product(*variable_dim)}
 
-def generate_multi_dimensional_var(model_object, variable_bound, variable_name, variable_dim, var_type):
-    if len(variable_dim) == 1:
-        GeneratedVariable = {key: getattr(model_object, var_type)(
-            variable_bound[0], variable_bound[1], name=f"{variable_name}{key}") for key in variable_dim[0]}
-    else:
-        GeneratedVariable = {key: getattr(model_object, var_type)(
-            variable_bound[0], variable_bound[1], name=f"{variable_name}{key}") for key in sets(*variable_dim)}
     return GeneratedVariable
```

### Comparing `feloopy-0.2.8/feloopy/generators/variable/mip_variable_generator.py` & `feloopy-0.2.9/feloopy/generators/variable/mip_variable_generator.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.8/feloopy/generators/variable/ortools_cp_variable_generator.py` & `feloopy-0.2.9/feloopy/generators/variable/ortools_cp_variable_generator.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.8/feloopy/generators/variable/picos_variable_generator.py` & `feloopy-0.2.9/feloopy/generators/variable/picos_variable_generator.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.8/feloopy/generators/variable/pulp_variable_generator.py` & `feloopy-0.2.9/feloopy/generators/variable/pulp_variable_generator.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.8/feloopy/generators/variable/pymprog_variable_generator.py` & `feloopy-0.2.9/feloopy/generators/variable/pymprog_variable_generator.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.8/feloopy/generators/variable/pyomo_variable_generator.py` & `feloopy-0.2.9/feloopy/generators/variable/pyomo_variable_generator.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.8/feloopy/generators/variable/rsome_dro_variable_generator.py` & `feloopy-0.2.9/feloopy/generators/variable/rsome_dro_variable_generator.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.8/feloopy/generators/variable/rsome_ro_variable_generator.py` & `feloopy-0.2.9/feloopy/generators/variable/rsome_ro_variable_generator.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.8/feloopy/generators/variable/xpress_variable_generator.py` & `feloopy-0.2.9/feloopy/generators/variable/xpress_variable_generator.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.8/feloopy/generators/variable_generator.py` & `feloopy-0.2.9/feloopy/generators/variable_generator.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,14 +19,34 @@
             return pulp_variable_generator.generate_variable(**inputs)
 
         case 'pyomo':
 
             from .variable import pyomo_variable_generator
             return pyomo_variable_generator.generate_variable(**inputs)
 
+        case 'insideopt':
+
+            from .variable import seeker_variable_generator
+            return seeker_variable_generator.generate_variable(**inputs)
+
+        case 'insideopt-demo':
+
+            from .variable import seeker_variable_generator
+            return seeker_variable_generator.generate_variable(**inputs)
+
+        case 'gams':
+
+            from .variable import gamspy_variable_generator
+            return gamspy_variable_generator.generate_variable(**inputs)
+
+        case 'highs':
+
+            from .variable import highs_variable_generator
+            return highs_variable_generator.generate_variable(**inputs)
+
         case 'ortools':
 
             from .variable import ortools_variable_generator
             return ortools_variable_generator.generate_variable(**inputs)
 
         case 'ortools_cp':
```

### Comparing `feloopy-0.2.8/feloopy/helpers/empty.py` & `feloopy-0.2.9/feloopy/helpers/empty.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,91 +9,91 @@
 
     def __init__(self, val):
 
         self.val = val
 
     def __call__(self, *args):
 
-        return 5
+        return 7
 
     def __getitem__(self, *args):
 
-        return 5
+        return 7
 
     def __setitem__(self, *args):
         'none'
 
     def __hash__(self):
 
-        return 5
+        return 7
 
     def __str__(self):
 
-        return 5
+        return 7
 
     def __repr__(self):
 
-        return 5
+        return 7
 
     def __neg__(self):
 
-        return 5
+        return 7
 
     def __pos__(self):
 
-        return 5
+        return 7
 
     def __pow__(self, other):
 
-        return 5
+        return 7
 
     def __bool__(self):
 
-        return 5
+        return 7
 
     def __add__(self, other):
 
-        return 5
+        return 7
 
     def __radd__(self, other):
 
-        return 5
+        return 7
 
     def __sub__(self, other):
 
-        return 5
+        return 7
 
     def __rsub__(self, other):
 
-        return 5
+        return 7
 
     def __mul__(self, other):
 
-        return 5
+        return 7
 
     def __rmul__(self, other):
 
-        return 5
+        return 7
 
     def __div__(self, other):
 
-        return 5
+        return 7
 
     def __rdiv__(self, other):
 
-        raise 5
+        raise 7
 
     def __le__(self, other):
 
-        return 5
+        return 7
 
     def __ge__(self, other):
 
-        return 5
+        return 7
 
     def __eq__(self, other):
 
-        return 5
+        return 7
 
     def __ne__(self, other):
 
-        return 5
+        return 7
```

### Comparing `feloopy-0.2.8/feloopy/operators/heuristic_operators.py` & `feloopy-0.2.9/feloopy/operators/heuristic_operators.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,115 +5,135 @@
 
 from ..helpers.empty import *
 from ..helpers.error import *
 import numpy as np
 import math as mt
 
 
+class NumpyVariable(np.ndarray):
+    def __new__(cls, input_array):
+        obj = np.asarray(input_array).view(cls)
+        return obj
+
+    def __array_finalize__(self, obj):
+        if obj is None: return
+
+    def __le__(self, other):       
+        return self - other
+
+    def __ge__(self, other):
+        return other - self
+
+    def __sub__(self, other):
+        return NumpyVariable(super().__sub__(other))
+    
 def generate_heuristic_variable(features, type, name, variable_dim, variable_bound, agent, no_agents):
 
     if no_agents==None:
         no_agents=100
-    
 
     if features['agent_status'] == 'idle':
 
         if features['vectorized']:
 
             if variable_dim == 0:
 
                 if type == 'pvar' or type == 'fvar':
-                    return variable_bound[0] + np.random.rand(no_agents,1)*(variable_bound[1]-variable_bound[0])
+                    return NumpyVariable(variable_bound[0] + np.random.rand(no_agents,1)*(variable_bound[1]-variable_bound[0]))
                 if type == 'bvar' or type == 'ivar':
-                    return np.round(variable_bound[0] + np.random.rand(no_agents,1)*(variable_bound[1]-variable_bound[0])).astype(int)
+                    return NumpyVariable(np.round(variable_bound[0] + np.random.rand(no_agents,1)*(variable_bound[1]-variable_bound[0])).astype(int))
                 if type == 'svar':
                     raise VariableDimError("Dimension is set to be 0 or not defined for a sequential variable.")
                 
             else:
 
                 if type == 'pvar' or type == 'fvar':
-                    return variable_bound[0] + np.random.rand(*tuple([no_agents]+[len(dims) for dims in variable_dim]))*(variable_bound[1]-variable_bound[0])
+                    return NumpyVariable(variable_bound[0] + np.random.rand(*tuple([no_agents]+[len(dims) for dims in variable_dim]))*(variable_bound[1]-variable_bound[0]))
                 if type == 'bvar' or type == 'ivar':
-                    return np.round(variable_bound[0] + np.random.rand(*tuple([no_agents]+[len(dims) for dims in variable_dim]))*(variable_bound[1]-variable_bound[0])).astype(int) 
+                    return NumpyVariable(np.round(variable_bound[0] + np.random.rand(*tuple([no_agents]+[len(dims) for dims in variable_dim]))*(variable_bound[1]-variable_bound[0])).astype(int) )
                 if type == 'svar':          
-                    return np.argsort(np.random.rand(*tuple([no_agents]+[len(dims) for dims in variable_dim])), axis=1)
+                    return NumpyVariable(np.argsort(np.random.rand(*tuple([no_agents]+[len(dims) for dims in variable_dim])), axis=1))
 
         else:
+            
+           
 
             if variable_dim == 0:
 
                 if type == 'pvar' or type == 'fvar':
-                    return variable_bound[0] + np.random.rand()*(variable_bound[1]-variable_bound[0])
+                    return NumpyVariable(variable_bound[0] + np.random.rand()*(variable_bound[1]-variable_bound[0]))
                 if type == 'bvar' or type == 'ivar':
-                    return np.round(variable_bound[0] + np.random.rand()*(variable_bound[1]-variable_bound[0])).astype(int)
+                    return NumpyVariable(np.round(variable_bound[0] + np.random.rand()*(variable_bound[1]-variable_bound[0])).astype(int))
                 if type == 'svar':
                     raise VariableDimError("Dimension is set to be 0 or not defined for a sequential variable.")
             
             else:
 
                 if type == 'pvar' or type == 'fvar':
-                    return variable_bound[0] + np.random.rand(*tuple([len(dims) for dims in variable_dim]))*(variable_bound[1]-variable_bound[0])
+                    return NumpyVariable(variable_bound[0] + np.random.rand(*tuple([len(dims) for dims in variable_dim]))*(variable_bound[1]-variable_bound[0]))
                 if type == 'bvar' or type == 'ivar':
-                    return np.round(variable_bound[0] + np.random.rand(*tuple([len(dims) for dims in variable_dim]))*(variable_bound[1]-variable_bound[0])).astype(int) 
+                    return NumpyVariable(np.round(variable_bound[0] + np.random.rand(*tuple([len(dims) for dims in variable_dim]))*(variable_bound[1]-variable_bound[0])).astype(int) )
                 if type == 'svar':          
-                    return np.argsort(np.random.rand(*tuple([len(dims) for dims in variable_dim])))
+                    return NumpyVariable(np.argsort(np.random.rand(*tuple([len(dims) for dims in variable_dim]))))
     else:
 
         spread = features['variable_spread'][name]
 
         if features['vectorized']:
             if variable_dim == 0:
                 if type == 'bvar' or type == 'ivar':
-                    return np.round(variable_bound[0] + agent[:, spread[0]:spread[1]] * (variable_bound[1] - variable_bound[0])).astype(int)
+                    return NumpyVariable(np.round(variable_bound[0] + agent[:, spread[0]:spread[1]] * (variable_bound[1] - variable_bound[0])).astype(int))
                 
                 elif type == 'pvar' or type == 'fvar':
-                    return variable_bound[0] + agent[:, spread[0]:spread[1]] * (variable_bound[1] - variable_bound[0])
+                    return NumpyVariable(variable_bound[0] + agent[:, spread[0]:spread[1]] * (variable_bound[1] - variable_bound[0]))
                 else:
-                    return np.argsort(agent[:, spread[0]:spread[1]])
+                    return NumpyVariable(np.argsort(agent[:, spread[0]:spread[1]]))
             else:
 
                 if type == 'bvar' or type == 'ivar':
 
-                    var = np.round(
-                        variable_bound[0] + agent[:, spread[0]:spread[1]] * (variable_bound[1] - variable_bound[0])).astype(int)
+                    var = NumpyVariable(np.round(variable_bound[0] + agent[:, spread[0]:spread[1]] * (variable_bound[1] - variable_bound[0])).astype(int))
 
-                    return np.reshape(var, [var.shape[0]]+[len(dims) for dims in variable_dim])
+                    return NumpyVariable(np.reshape(var, [var.shape[0]]+[len(dims) for dims in variable_dim]))
 
                 elif type == 'pvar' or type == 'fvar':
 
                     var = variable_bound[0] + agent[:, spread[0]:spread[1]
                                                     ] * (variable_bound[1] - variable_bound[0])
 
-                    return np.reshape(var, [var.shape[0]]+[len(dims) for dims in variable_dim])
+                    return NumpyVariable(np.reshape(var, [var.shape[0]]+[len(dims) for dims in variable_dim]))
 
                 else:
 
-                    return np.argsort(agent[:, spread[0]:spread[1]])
+                    return NumpyVariable(np.argsort(agent[:, spread[0]:spread[1]]))
         else:
 
             if variable_dim == 0:
 
                 if type == 'bvar' or type == 'ivar':
+                    
+                    
 
-                    return np.round(variable_bound[0] + agent[spread[0]:spread[1]] * (variable_bound[1] - variable_bound[0])).astype(int)
+                    return NumpyVariable(np.round(variable_bound[0] + agent[spread[0]:spread[1]] * (variable_bound[1] - variable_bound[0])).astype(int))
 
                 elif type == 'pvar' or type == 'fvar':
 
-                    return variable_bound[0] + agent[spread[0]:spread[1]] * (variable_bound[1] - variable_bound[0])
+                    return NumpyVariable(variable_bound[0] + agent[spread[0]:spread[1]] * (variable_bound[1] - variable_bound[0]))
 
                 else:
 
-                    return np.argsort(agent[spread[0]:spread[1]])
+                    return NumpyVariable(np.argsort(agent[spread[0]:spread[1]]))
 
             else:
 
                 if type == 'bvar' or type == 'ivar':
-
-                    return np.reshape(np.round(variable_bound[0] + agent[spread[0]:spread[1]] * (variable_bound[1] - variable_bound[0])), [len(dims) for dims in variable_dim]).astype(int)
+                    
+       
+                    return NumpyVariable(np.reshape(np.round(variable_bound[0] + agent[spread[0]:spread[1]] * (variable_bound[1] - variable_bound[0])), [len(dims) for dims in variable_dim]).astype(int))
 
                 elif type == 'pvar' or type == 'fvar':
 
-                    return np.reshape(variable_bound[0] + agent[spread[0]:spread[1]] * (variable_bound[1] - variable_bound[0]), [len(dims) for dims in variable_dim])
+                    return NumpyVariable(np.reshape(variable_bound[0] + agent[spread[0]:spread[1]] * (variable_bound[1] - variable_bound[0]), [len(dims) for dims in variable_dim]))
 
                 else:
 
-                    return np.argsort(agent[spread[0]:spread[1]])
+                    return NumpyVariable(np.argsort(agent[spread[0]:spread[1]]))
```

### Comparing `feloopy-0.2.8/feloopy/operators/math_operators.py` & `feloopy-0.2.9/feloopy/operators/math_operators.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.8/feloopy/operators/update_operators.py` & `feloopy-0.2.9/feloopy/operators/update_operators.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.8/feloopy.egg-info/SOURCES.txt` & `feloopy-0.2.9/feloopy.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 LICENSE
+README.md
 pyproject.toml
 setup.py
 feloopy/__init__.py
 feloopy/cli.py
 feloopy/feloopy.py
 feloopy.egg-info/PKG-INFO
 feloopy.egg-info/SOURCES.txt
@@ -10,137 +11,158 @@
 feloopy.egg-info/entry_points.txt
 feloopy.egg-info/requires.txt
 feloopy.egg-info/top_level.txt
 feloopy/algorithms/__init__.py
 feloopy/algorithms/constraint/__init__.py
 feloopy/algorithms/exact/__init__.py
 feloopy/algorithms/exact/benders.py
+feloopy/algorithms/exact/multiobjective.py
 feloopy/algorithms/heuristic/DE.py
 feloopy/algorithms/heuristic/GA.py
 feloopy/algorithms/heuristic/GWO.py
 feloopy/algorithms/heuristic/SA.py
 feloopy/algorithms/heuristic/TS.py
 feloopy/algorithms/heuristic/__init__.py
 feloopy/classes/__init__.py
 feloopy/classes/constraint_programming.py
 feloopy/classes/event_variable.py
 feloopy/classes/event_variable_collection.py
 feloopy/classes/linearization.py
 feloopy/classes/multidim_variable.py
 feloopy/classes/multidim_variable_collection.py
+feloopy/classes/normal_constraint.py
 feloopy/classes/special_constraint.py
 feloopy/classes/tensor_variable.py
 feloopy/classes/tensor_variable_collection.py
 feloopy/clitools/__init__.py
 feloopy/clitools/pkg_manager_detector.py
 feloopy/clitools/utils.py
 feloopy/generators/__init__.py
+feloopy/generators/init_generator.py
 feloopy/generators/model_generator.py
 feloopy/generators/result_generator.py
 feloopy/generators/solution_generator.py
 feloopy/generators/variable_generator.py
+feloopy/generators/init/__init__.py
+feloopy/generators/init/copt_init_generator.py
+feloopy/generators/init/cplex_init_generator.py
+feloopy/generators/init/gekko_init_generator.py
+feloopy/generators/init/gurobi_init_generator.py
+feloopy/generators/init/pulp_init_generator.py
+feloopy/generators/init/pyomo_init_generator.py
 feloopy/generators/model/__init__.py
 feloopy/generators/model/copt_model_generator.py
 feloopy/generators/model/cplex_cp_model_generator.py
 feloopy/generators/model/cplex_model_generator.py
 feloopy/generators/model/cvxpy_model_generator.py
 feloopy/generators/model/cylp_model_generator.py
 feloopy/generators/model/feloopy_model_generator.py
+feloopy/generators/model/gamspy_model_generator.py
 feloopy/generators/model/gekko_model_generator.py
 feloopy/generators/model/gurobi_model_generator.py
+feloopy/generators/model/highs_model_generator.py
 feloopy/generators/model/linopy_model_generator.py
-feloopy/generators/model/localsolver_model_generator.py
 feloopy/generators/model/mealpy_model_generator.py
 feloopy/generators/model/mip_model_generator.py
 feloopy/generators/model/niapy_model_generator.py
 feloopy/generators/model/ortools_cp_model_generator.py
 feloopy/generators/model/ortools_model_generator.py
 feloopy/generators/model/picos_model_generator.py
 feloopy/generators/model/pulp_model_generator.py
 feloopy/generators/model/pymprog_model_generator.py
 feloopy/generators/model/pyomo_model_generator.py
 feloopy/generators/model/rsome_dro_model_generator.py
 feloopy/generators/model/rsome_ro_model_generator.py
+feloopy/generators/model/seeker_model_generator.py
 feloopy/generators/model/xpress_model_generator.py
 feloopy/generators/result/__init__.py
 feloopy/generators/result/copt_result_generator.py
 feloopy/generators/result/cplex_cp_result_generator.py
 feloopy/generators/result/cplex_result_generator.py
 feloopy/generators/result/cvxpy_result_generator.py
 feloopy/generators/result/cylp_result_generator.py
+feloopy/generators/result/gamspy_result_generator.py
 feloopy/generators/result/gekko_result_generator.py
 feloopy/generators/result/gurobi_result_generator.py
+feloopy/generators/result/highs_result_generator.py
 feloopy/generators/result/linopy_result_generator.py
-feloopy/generators/result/localsolver_result_generator.py
 feloopy/generators/result/mip_result_generator.py
 feloopy/generators/result/ortools_cp_result_generator.py
 feloopy/generators/result/ortools_result_generator.py
 feloopy/generators/result/picos_result_generator.py
 feloopy/generators/result/pulp_result_generator.py
 feloopy/generators/result/pymprog_result_generator.py
 feloopy/generators/result/pyomo_result_generator.py
 feloopy/generators/result/rsome_dro_result_generator.py
 feloopy/generators/result/rsome_ro_result_generator.py
+feloopy/generators/result/seeker_result_generator.py
 feloopy/generators/result/xpress_result_generator.py
 feloopy/generators/solution/__init__.py
 feloopy/generators/solution/copt_solution_generator.py
 feloopy/generators/solution/cplex_cp_solution_generator.py
 feloopy/generators/solution/cplex_solution_generator.py
 feloopy/generators/solution/cvxpy_solution_generator.py
 feloopy/generators/solution/cylp_solution_generator.py
 feloopy/generators/solution/feloopy_solution_generator.py
+feloopy/generators/solution/gamspy_solution_generator.py
 feloopy/generators/solution/gekko_solution_generator.py
 feloopy/generators/solution/gurobi_solution_generator.py
+feloopy/generators/solution/highs_solution_generator.py
 feloopy/generators/solution/linopy_solution_generator.py
-feloopy/generators/solution/localsolver_solution_generator.py
 feloopy/generators/solution/mealpy_solution_generator.py
 feloopy/generators/solution/mip_solution_generator.py
 feloopy/generators/solution/niapy_solution_generator.py
 feloopy/generators/solution/ortools_cp_solution_generator.py
 feloopy/generators/solution/ortools_solution_generator.py
 feloopy/generators/solution/picos_solution_generator.py
 feloopy/generators/solution/pulp_solution_generator.py
 feloopy/generators/solution/pygad_solution_generator.py
 feloopy/generators/solution/pymoo_solution_generator.py
 feloopy/generators/solution/pymprog_solution_generator.py
 feloopy/generators/solution/pymultiobjective_solution_generator.py
 feloopy/generators/solution/pyomo_solution_generator.py
 feloopy/generators/solution/rsome_dro_solution_generator.py
 feloopy/generators/solution/rsome_ro_solution_generator.py
+feloopy/generators/solution/seeker_solution_generator.py
 feloopy/generators/solution/xpress_solution_generator.py
 feloopy/generators/variable/__init__.py
 feloopy/generators/variable/copt_variable_generator.py
 feloopy/generators/variable/cplex_cp_variable_generator.py
 feloopy/generators/variable/cplex_variable_generator.py
 feloopy/generators/variable/cvxpy_variable_generator.py
 feloopy/generators/variable/cylp_variable_generator.py
+feloopy/generators/variable/gamspy_variable_generator.py
 feloopy/generators/variable/gekko_variable_generator.py
 feloopy/generators/variable/gurobi_variable_generator.py
+feloopy/generators/variable/highs_variable_generator.py
 feloopy/generators/variable/linopy_variable_generator.py
-feloopy/generators/variable/localsolver_variable_generator.py
 feloopy/generators/variable/mip_variable_generator.py
 feloopy/generators/variable/ortools_cp_variable_generator.py
 feloopy/generators/variable/ortools_variable_generator.py
 feloopy/generators/variable/picos_variable_generator.py
 feloopy/generators/variable/pulp_variable_generator.py
 feloopy/generators/variable/pymprog_variable_generator.py
 feloopy/generators/variable/pyomo_variable_generator.py
 feloopy/generators/variable/rsome_dro_variable_generator.py
 feloopy/generators/variable/rsome_ro_variable_generator.py
+feloopy/generators/variable/seeker_variable_generator.py
 feloopy/generators/variable/xpress_variable_generator.py
 feloopy/helpers/__init__.py
+feloopy/helpers/context_manager.py
 feloopy/helpers/empty.py
 feloopy/helpers/error.py
 feloopy/helpers/formatter.py
 feloopy/operators/__init__.py
 feloopy/operators/common.py
 feloopy/operators/data_handler.py
 feloopy/operators/epsilon.py
 feloopy/operators/exact.py
 feloopy/operators/fix_operators.py
 feloopy/operators/heuristic.py
 feloopy/operators/heuristic_operators.py
 feloopy/operators/math_operators.py
+feloopy/operators/metrics.py
 feloopy/operators/pareto.py
 feloopy/operators/random_operators.py
 feloopy/operators/set_operators.py
-feloopy/operators/update_operators.py
+feloopy/operators/update_operators.py
+feloopy/operators/validator.py
```

### Comparing `feloopy-0.2.8/pyproject.toml` & `feloopy-0.2.9/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,142 +1,162 @@
 # Copyright (c) 2022-2024, Keivan Tafakkori. All rights reserved.
 # See the file LICENSE file for licensing details.
 
 [tool.poetry]
 name = "feloopy"
-version = "0.2.8"
-description = "FelooPy: An integrated optimization environment (IOE) for automated operations research (AutoOR) in Python."
+version = "0.2.9"
+description = "FelooPy: Efficient and feature-rich integrated decision environment"
 authors = ["Keivan Tafakkori <k.tafakkori@gmail.com>"]
 license = "MIT"
 
 [tool.poetry.dependencies]
 gputil = "1.4.0"
 infix = "1.2"
-matplotlib = "3.8.2"
+matplotlib = ""
 nbformat = "5.9.2"
-numba = "0.58.1"
-numpy = "1.26.2"
+numba = ""
+numpy = ""
 openpyxl = "3.1.2"
 pandas = "2.1.3"
-plotly = "5.18.0"
-polars = "0.19.19"
-psutil = "5.9.6"
+plotly = ""
+polars = ""
+psutil = ""
 py-cpuinfo = "9.0.0"
 python = ">=3.10,<3.12"
-scikit-learn = "1.3.2"
+scikit-learn = ""
 tabulate = "0.9.0"
 win-unicode-console = "0.5"
 xlsxwriter = "3.1.9"
-tqdm= "4.66.1"
+tqdm= ""
+colorama = ""
 
 [tool.poetry.group.pico.dependencies]
 
 [tool.poetry.group.nano.dependencies]
 pymprog = "1.1.2"
+highspy = ""
 
 [tool.poetry.group.micro.dependencies]
-gekko = "1.0.6"
+gekko = "1.1.0"
 mealpy = "3.0.1"
 pymprog = "1.1.2"
+highspy = ""
 
 [tool.poetry.group.mini.dependencies]
-cvxpy = "1.4.1"
-gekko = "1.0.6"
+cvxpy = "1.4.2"
+gekko = "1.1.0"
 mealpy = "3.0.1"
 ortools = "9.8.3296"
 pymprog = "1.1.2"
+highspy = ""
 
 [tool.poetry.group.full.dependencies]
-cvxpy = "1.4.1"
-gekko = "1.0.6"
+cvxpy = "1.4.2"
+gekko = "1.1.0"
 mealpy = "3.0.1"
 ortools = "9.8.3296"
 pydecision = "4.3.9"
 pymoo = "0.6.1.1"
 pymprog = "1.1.2"
+rsome = "1.2.5"
+highspy = ""
 
 [tool.poetry.group.stock.dependencies]
-cvxpy = "1.4.1"
-gekko = "1.0.6"
-linopy = "0.3.2"
+cvxpy = "1.4.2"
+gekko = "1.1.0"
+linopy = "0.3.8"
 mealpy = "3.0.1"
 mip = "1.15.0"
 niapy = "2.1.0"
 ortools = "9.8.3296"
 picos = "2.4.17"
-pulp = "2.7.0"
+pulp = "2.8.0"
 pydecision = "4.3.9"
 pygad = "3.2.0"
 pymoo = "0.6.1.1"
 pymprog = "1.1.2"
-pyomo = "6.7.0"
+pyomo = "6.7.1"
 rsome = "1.2.5"
+highspy = ""
 
 [tool.poetry.group.plus_gurobi.dependencies]
-gurobipy = "11.0.0"
+gurobipy = ""
 
 [tool.poetry.group.plus_cplex.dependencies]
-cplex = "22.1.1.1"
-docplex = "2.25.236"
+cplex = ""
+docplex = ""
 
 [tool.poetry.group.plus_xpress.dependencies]
 xpress = "9.2.5"
 
 [tool.poetry.group.plus_copt.dependencies]
-coptpy = "7.0.4"
+coptpy = ""
+
+[tool.poetry.group.plus_insideoptdemo.dependencies]
+insideopt-demo = ""
+
+[tool.poetry.group.plus_insideopt.dependencies]
+insideopt = ""
+
+[tool.poetry.group.plus_gams.dependencies]
+gampspy = ""
 
 [tool.poetry.group.hyper.dependencies]
-coptpy = "7.0.4"
-cplex = "22.1.1.1"
-cvxpy = "1.4.1"
-docplex = "2.25.236"
-gekko = "1.0.6"
-gurobipy = "11.0.0"
-linopy = "0.3.2"
+coptpy = ""
+cplex = ""
+cvxpy = "1.4.2"
+docplex = ""
+gekko = "1.1.0"
+gurobipy = ""
+linopy = "0.3.8"
 mealpy = "3.0.1"
 mip = "1.15.0"
 niapy = "2.1.0"
 ortools = "9.8.3296"
 picos = "2.4.17"
-pulp = "2.7.0"
+pulp = "2.8.0"
 pydecision = "4.3.9"
 pygad = "3.2.0"
 pymoo = "0.6.1.1"
 pymprog = "1.1.2"
-pyomo = "6.7.0"
+pyomo = "6.7.1"
 rsome = "1.2.5"
 xpress = "9.2.5"
+gampspy = ""
+highspy = ""
 
 [tool.poetry.group.only_cylp.dependencies]
 cylp = "0.92.2"
 
 [tool.poetry.group.only_linux.dependencies]
 pymultiobjective = "1.5.4"
 
 [tool.poetry.group.mega.dependencies]
-coptpy = "7.0.4"
-cplex = "22.1.1.1"
-cvxpy = "1.4.1"
+coptpy = ""
+cplex = ""
+cvxpy = "1.4.2"
 cylp = "0.92.2"
-docplex = "2.25.236"
-gekko = "1.0.6"
-gurobipy = "11.0.0"
-linopy = "0.3.2"
+docplex = ""
+gekko = "1.1.0"
+gurobipy = ""
+linopy = "0.3.8"
 mealpy = "3.0.1"
 mip = "1.15.0"
 niapy = "2.1.0"
 ortools = "9.8.3296"
 picos = "2.4.17"
-pulp = "2.7.0"
+pulp = "2.8.0"
 pydecision = "4.3.9"
 pygad = "3.2.0"
 pymoo = "0.6.1.1"
 pymprog = "1.1.2"
 pymultiobjective = "1.5.4"
-pyomo = "6.7.0"
+pyomo = "6.7.1"
 rsome = "1.2.5"
 xpress = "9.2.5"
+gampspy = ""
+highspy = ""
 
 [tool.poetry.scripts]
 feloopy = "feloopy.cli:main"
 flp = "feloopy.cli:main"
 fly = "feloopy.cli:main"
```

### Comparing `feloopy-0.2.8/setup.py` & `feloopy-0.2.9/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,87 +4,101 @@
 from setuptools import setup, find_packages
 
 # Common packages for all versions of FelooPy
 
 common = [
     'gputil==1.4.0',
     'infix==1.2',
-    'matplotlib==3.8.2',
+    'matplotlib',
     'nbformat==5.9.2',
-    'numba==0.58.1',
-    'numpy==1.26.2',
+    'numba',
+    'numpy',
     'openpyxl==3.1.2',
     'pandas==2.1.3',
-    'plotly==5.18.0',
-    'polars==0.19.19',
-    'psutil==5.9.6',
+    'plotly',
+    'polars',
+    'psutil',
     'py-cpuinfo==9.0.0',
-    'scikit-learn==1.3.2',
+    'scikit-learn',
     'tabulate==0.9.0',
     'win-unicode-console==0.5',
     'xlsxwriter==3.1.9',
-    'tqdm==4.66.1',
+    'tqdm',
+    'colorama',
 ]
 
 # Interfaces for optimization solvers or algorithms
 
 pico = [
     ''
 ]
 
 nano = pico + [
     'pymprog==1.1.2',
+    'highspy',
 ]
 
 micro = nano + [
-    'gekko==1.0.6',
+    'gekko==1.1.0',
     'mealpy==3.0.1',
 ]
 
 mini = micro + [
-    'cvxpy==1.4.1',
+    'cvxpy==1.4.2',
     'ortools==9.8.3296',
 ]
 
 full = mini + [
     'pydecision==4.3.9',
     'pymoo==0.6.1.1',
+    'rsome==1.2.5',
 ]
 
 stock = full + [
-    'linopy==0.3.2',
+    'linopy==0.3.8',
     'mip==1.15.0',
     'niapy==2.1.0',
     'picos==2.4.17',
-    'pulp==2.7.0',
+    'pulp==2.8.0',
     'pygad==3.2.0',
-    'pyomo==6.7.0',
-    'rsome==1.2.5',
+    'pyomo==6.7.1',
 ]
 
 # Solvers for optimization problems or algorithms
 
 plus_gurobi = [
-    'gurobipy==11.0.0',
+    'gurobipy',
 ]
 
 plus_cplex = [
-    'cplex==22.1.1.1',
-    'docplex==2.25.236',
+    'cplex',
+    'docplex',
 ]
 
 plus_xpress = [
-    'xpress==9.2.5',
+    'xpress',
 ]
 
 plus_copt = [
-    'coptpy==7.0.4',
+    'coptpy',
+]
+
+plus_insideoptdemo = [
+    'insideopt-demo',
+]
+
+plus_insideopt = [
+    'insideopt',
+]
+
+plus_gams = [
+    'gamspy',
 ]
 
-hyper = stock + plus_gurobi + plus_cplex + plus_xpress + plus_copt
+hyper = stock + plus_gurobi + plus_cplex + plus_xpress + plus_copt + plus_gams
 
 # Might have some os-dependent issues
 
 only_cylp = [
     'cylp==0.92.2',
 ]
 
@@ -102,14 +116,17 @@
     'full': full, 
     'stock': stock,
     'hyper': hyper,
     'plus_gurobi': plus_gurobi,
     'plus_cplex': plus_cplex,
     'plus_xpress': plus_xpress,
     'plus_copt': plus_copt,
+    'plus_insideopt': plus_insideopt,
+    'plus_insideoptdemo': plus_insideoptdemo,
+    'plus_gams': plus_gams,
     'only_cylp': only_cylp,
     'only_linux': only_linux,
     'mega': mega}
 
 keywords_list = [
     'computer science',
     'data science',
@@ -128,21 +145,21 @@
 
 if __name__ == '__main__':
 
     setup(
         
         name = 'feloopy',
         
-        version = '0.2.8',
+        version = '0.2.9',
         
-        description = 'FelooPy: An integrated optimization environment (IOE) for automated operations research (AutoOR) in Python.',
+        description = 'FelooPy: Efficient and feature-rich integrated decision environment',
         
         packages = find_packages(include=['feloopy', 'feloopy.*']),
         
-        long_description = open('./docs/README.md', encoding="utf8").read(),
+        long_description = open('./README.md', encoding="utf8").read(),
         
         long_description_content_type = 'text/markdown',
         
         keywords = keywords_list,
         
         author='Keivan Tafakkori',
```

