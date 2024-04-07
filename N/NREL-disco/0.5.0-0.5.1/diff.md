# Comparing `tmp/NREL-disco-0.5.0.tar.gz` & `tmp/NREL-disco-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/NREL-disco-0.5.0.tar", last modified: Wed Nov 22 23:51:03 2023, max compression
+gzip compressed data, was "dist/NREL-disco-0.5.1.tar", last modified: Sun Apr  7 21:28:11 2024, max compression
```

## Comparing `NREL-disco-0.5.0.tar` & `NREL-disco-0.5.1.tar`

### file list

```diff
@@ -1,173 +1,173 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-22 23:51:03.000000 NREL-disco-0.5.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-22 23:51:03.000000 NREL-disco-0.5.0/NREL_disco.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      623 2023-11-22 23:51:03.000000 NREL-disco-0.5.0/NREL_disco.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5350 2023-11-22 23:51:03.000000 NREL-disco-0.5.0/NREL_disco.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-22 23:51:03.000000 NREL-disco-0.5.0/NREL_disco.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       93 2023-11-22 23:51:03.000000 NREL-disco-0.5.0/NREL_disco.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-22 23:51:03.000000 NREL-disco-0.5.0/NREL_disco.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      391 2023-11-22 23:51:03.000000 NREL-disco-0.5.0/NREL_disco.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2023-11-22 23:51:03.000000 NREL-disco-0.5.0/NREL_disco.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      623 2023-11-22 23:51:03.000000 NREL-disco-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       83 2023-11-22 23:50:55.000000 NREL-disco-0.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-22 23:51:03.000000 NREL-disco-0.5.0/disco/
--rw-r--r--   0 runner    (1001) docker     (127)      201 2023-11-22 23:50:55.000000 NREL-disco-0.5.0/disco/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-22 23:51:03.000000 NREL-disco-0.5.0/disco/analysis/
--rw-r--r--   0 runner    (1001) docker     (127)      150 2023-11-22 23:50:55.000000 NREL-disco-0.5.0/disco/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6175 2023-11-22 23:50:55.000000 NREL-disco-0.5.0/disco/analysis/analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)      553 2023-11-22 23:50:55.000000 NREL-disco-0.5.0/disco/analysis/configure.py
--rw-r--r--   0 runner    (1001) docker     (127)     1000 2023-11-22 23:50:55.000000 NREL-disco-0.5.0/disco/analysis/input.py
--rw-r--r--   0 runner    (1001) docker     (127)      240 2023-11-22 23:50:55.000000 NREL-disco-0.5.0/disco/analysis/option.py
--rw-r--r--   0 runner    (1001) docker     (127)     7254 2023-11-22 23:50:55.000000 NREL-disco-0.5.0/disco/analysis/postprocess_time_series.py
--rw-r--r--   0 runner    (1001) docker     (127)    25140 2023-11-22 23:50:55.000000 NREL-disco-0.5.0/disco/analysis/snapshot_impact_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)      878 2023-11-22 23:50:55.000000 NREL-disco-0.5.0/disco/analysis/time_series_impact_analysis.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-22 23:51:03.000000 NREL-disco-0.5.0/disco/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-22 23:50:55.000000 NREL-disco-0.5.0/disco/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2334 2023-11-22 23:50:55.000000 NREL-disco-0.5.0/disco/cli/cba_post_process.py
--rw-r--r--   0 runner    (1001) docker     (127)     2231 2023-11-22 23:50:55.000000 NREL-disco-0.5.0/disco/cli/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     4070 2023-11-22 23:50:55.000000 NREL-disco-0.5.0/disco/cli/compute_cba.py
--rw-r--r--   0 runner    (1001) docker     (127)     3114 2023-11-22 23:50:55.000000 NREL-disco-0.5.0/disco/cli/compute_hosting_capacity.py
--rw-r--r--   0 runner    (1001) docker     (127)     5675 2023-11-22 23:50:55.000000 NREL-disco-0.5.0/disco/cli/compute_pv_swad.py
--rw-r--r--   0 runner    (1001) docker     (127)     5450 2023-11-22 23:50:55.000000 NREL-disco-0.5.0/disco/cli/compute_snapshot_hosting_capacity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1419 2023-11-22 23:50:55.000000 NREL-disco-0.5.0/disco/cli/compute_snapshot_impact_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2023-11-22 23:50:55.000000 NREL-disco-0.5.0/disco/cli/compute_time_series_hosting_capacity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1133 2023-11-22 23:50:55.000000 NREL-disco-0.5.0/disco/cli/compute_time_series_impact_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)      344 2023-11-22 23:50:55.000000 NREL-disco-0.5.0/disco/cli/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     9235 2023-11-22 23:50:55.000000 NREL-disco-0.5.0/disco/cli/config_generic_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     9581 2023-11-22 23:50:55.000000 NREL-disco-0.5.0/disco/cli/config_snapshot.py
--rw-r--r--   0 runner    (1001) docker     (127)    10675 2023-11-22 23:50:55.000000 NREL-disco-0.5.0/disco/cli/config_time_series.py
--rw-r--r--   0 runner    (1001) docker     (127)     2356 2023-11-22 23:50:55.000000 NREL-disco-0.5.0/disco/cli/config_upgrade.py
--rw-r--r--   0 runner    (1001) docker     (127)     2395 2023-11-22 23:50:55.000000 NREL-disco-0.5.0/disco/cli/configure_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     9550 2023-11-22 23:50:55.000000 NREL-disco-0.5.0/disco/cli/create_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     2051 2023-11-22 23:50:55.000000 NREL-disco-0.5.0/disco/cli/disco.py
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2023-11-22 23:50:55.000000 NREL-disco-0.5.0/disco/cli/disco_internal.py
--rw-r--r--   0 runner    (1001) docker     (127)      799 2023-11-22 23:50:55.000000 NREL-disco-0.5.0/disco/cli/download_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     2022 2023-11-22 23:50:55.000000 NREL-disco-0.5.0/disco/cli/ingest_tables.py
--rw-r--r--   0 runner    (1001) docker     (127)    10456 2023-11-22 23:50:55.000000 NREL-disco-0.5.0/disco/cli/make_cba_tables.py
--rw-r--r--   0 runner    (1001) docker     (127)    10771 2023-11-22 23:50:55.000000 NREL-disco-0.5.0/disco/cli/make_summary_tables.py
--rw-r--r--   0 runner    (1001) docker     (127)     4689 2023-11-22 23:50:55.000000 NREL-disco-0.5.0/disco/cli/make_upgrade_tables.py
--rw-r--r--   0 runner    (1001) docker     (127)      889 2023-11-22 23:50:55.000000 NREL-disco-0.5.0/disco/cli/plots.py
--rw-r--r--   0 runner    (1001) docker     (127)     5247 2023-11-22 23:50:55.000000 NREL-disco-0.5.0/disco/cli/prescreen_pv_penetration_levels.py
--rw-r--r--   0 runner    (1001) docker     (127)    10998 2023-11-22 23:50:55.000000 NREL-disco-0.5.0/disco/cli/pv_deployments.py
--rw-r--r--   0 runner    (1001) docker     (127)     1477 2023-11-22 23:50:55.000000 NREL-disco-0.5.0/disco/cli/pydss_hosting_capacity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1589 2023-11-22 23:50:55.000000 NREL-disco-0.5.0/disco/cli/simulation_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     6787 2023-11-22 23:50:55.000000 NREL-disco-0.5.0/disco/cli/summarize_hosting_capacity.py
--rw-r--r--   0 runner    (1001) docker     (127)     2601 2023-11-22 23:50:55.000000 NREL-disco-0.5.0/disco/cli/transform_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    13454 2023-11-22 23:50:55.000000 NREL-disco-0.5.0/disco/cli/upgrade_cost_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)      196 2023-11-22 23:50:55.000000 NREL-disco-0.5.0/disco/common.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-22 23:51:03.000000 NREL-disco-0.5.0/disco/distribution/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-22 23:50:55.000000 NREL-disco-0.5.0/disco/distribution/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3645 2023-11-22 23:50:55.000000 NREL-disco-0.5.0/disco/distribution/deployment_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)      670 2023-11-22 23:50:55.000000 NREL-disco-0.5.0/disco/distribution/distribution_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     4691 2023-11-22 23:50:55.000000 NREL-disco-0.5.0/disco/distribution/distribution_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4482 2023-11-22 23:50:55.000000 NREL-disco-0.5.0/disco/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)       83 2023-11-22 23:50:55.000000 NREL-disco-0.5.0/disco/events.py
--rw-r--r--   0 runner    (1001) docker     (127)     5678 2023-11-22 23:50:55.000000 NREL-disco-0.5.0/disco/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-22 23:51:03.000000 NREL-disco-0.5.0/disco/extensions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-22 23:50:55.000000 NREL-disco-0.5.0/disco/extensions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-22 23:51:03.000000 NREL-disco-0.5.0/disco/extensions/pydss_simulation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-22 23:50:55.000000 NREL-disco-0.5.0/disco/extensions/pydss_simulation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1670 2023-11-22 23:50:55.000000 NREL-disco-0.5.0/disco/extensions/pydss_simulation/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2904 2023-11-22 23:50:55.000000 NREL-disco-0.5.0/disco/extensions/pydss_simulation/estimate_run_minutes.py
--rw-r--r--   0 runner    (1001) docker     (127)     9764 2023-11-22 23:50:55.000000 NREL-disco-0.5.0/disco/extensions/pydss_simulation/pydss_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)      217 2023-11-22 23:50:55.000000 NREL-disco-0.5.0/disco/extensions/pydss_simulation/pydss_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     6685 2023-11-22 23:50:55.000000 NREL-disco-0.5.0/disco/extensions/pydss_simulation/pydss_simulation.py
--rw-r--r--   0 runner    (1001) docker     (127)      718 2023-11-22 23:50:55.000000 NREL-disco-0.5.0/disco/extensions/pydss_simulation/time_series_impact_analysis_configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-22 23:51:03.000000 NREL-disco-0.5.0/disco/extensions/upgrade_simulation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-22 23:50:55.000000 NREL-disco-0.5.0/disco/extensions/upgrade_simulation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3050 2023-11-22 23:50:55.000000 NREL-disco-0.5.0/disco/extensions/upgrade_simulation/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2469 2023-11-22 23:50:55.000000 NREL-disco-0.5.0/disco/extensions/upgrade_simulation/upgrade_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)      644 2023-11-22 23:50:55.000000 NREL-disco-0.5.0/disco/extensions/upgrade_simulation/upgrade_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)      293 2023-11-22 23:50:55.000000 NREL-disco-0.5.0/disco/extensions/upgrade_simulation/upgrade_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     7040 2023-11-22 23:50:55.000000 NREL-disco-0.5.0/disco/extensions/upgrade_simulation/upgrade_simulation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-22 23:51:03.000000 NREL-disco-0.5.0/disco/extensions/upgrade_simulation/upgrades/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-22 23:50:55.000000 NREL-disco-0.5.0/disco/extensions/upgrade_simulation/upgrades/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21649 2023-11-22 23:50:55.000000 NREL-disco-0.5.0/disco/extensions/upgrade_simulation/upgrades/automated_thermal_upgrades.py
--rw-r--r--   0 runner    (1001) docker     (127)    23549 2023-11-22 23:50:55.000000 NREL-disco-0.5.0/disco/extensions/upgrade_simulation/upgrades/automated_voltage_upgrades.py
--rw-r--r--   0 runner    (1001) docker     (127)    92378 2023-11-22 23:50:55.000000 NREL-disco-0.5.0/disco/extensions/upgrade_simulation/upgrades/common_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)    31891 2023-11-22 23:50:55.000000 NREL-disco-0.5.0/disco/extensions/upgrade_simulation/upgrades/cost_computation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1038 2023-11-22 23:50:55.000000 NREL-disco-0.5.0/disco/extensions/upgrade_simulation/upgrades/fixed_upgrade_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1475 2023-11-22 23:50:55.000000 NREL-disco-0.5.0/disco/extensions/upgrade_simulation/upgrades/pydss_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)    33131 2023-11-22 23:50:55.000000 NREL-disco-0.5.0/disco/extensions/upgrade_simulation/upgrades/thermal_upgrade_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)   129611 2023-11-22 23:50:55.000000 NREL-disco-0.5.0/disco/extensions/upgrade_simulation/upgrades/voltage_upgrade_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-22 23:51:03.000000 NREL-disco-0.5.0/disco/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-22 23:50:55.000000 NREL-disco-0.5.0/disco/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9698 2023-11-22 23:50:55.000000 NREL-disco-0.5.0/disco/models/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2036 2023-11-22 23:50:55.000000 NREL-disco-0.5.0/disco/models/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     5537 2023-11-22 23:50:55.000000 NREL-disco-0.5.0/disco/models/power_flow_generic_models.py
--rw-r--r--   0 runner    (1001) docker     (127)      595 2023-11-22 23:50:55.000000 NREL-disco-0.5.0/disco/models/snapshot_impact_analysis_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2037 2023-11-22 23:50:55.000000 NREL-disco-0.5.0/disco/models/time_series_analysis_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    15566 2023-11-22 23:50:55.000000 NREL-disco-0.5.0/disco/models/upgrade_cost_analysis_equipment_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    30076 2023-11-22 23:50:55.000000 NREL-disco-0.5.0/disco/models/upgrade_cost_analysis_generic_input_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    14951 2023-11-22 23:50:55.000000 NREL-disco-0.5.0/disco/models/upgrade_cost_analysis_generic_output_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2023-11-22 23:50:55.000000 NREL-disco-0.5.0/disco/models/upgrade_cost_analysis_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2684 2023-11-22 23:50:55.000000 NREL-disco-0.5.0/disco/models/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-22 23:51:03.000000 NREL-disco-0.5.0/disco/pipelines/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-22 23:50:55.000000 NREL-disco-0.5.0/disco/pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      741 2023-11-22 23:50:55.000000 NREL-disco-0.5.0/disco/pipelines/auto_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    13125 2023-11-22 23:50:55.000000 NREL-disco-0.5.0/disco/pipelines/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    13022 2023-11-22 23:50:55.000000 NREL-disco-0.5.0/disco/pipelines/creator.py
--rw-r--r--   0 runner    (1001) docker     (127)      378 2023-11-22 23:50:55.000000 NREL-disco-0.5.0/disco/pipelines/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)      983 2023-11-22 23:50:55.000000 NREL-disco-0.5.0/disco/pipelines/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)      531 2023-11-22 23:50:55.000000 NREL-disco-0.5.0/disco/pipelines/update_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1713 2023-11-22 23:50:55.000000 NREL-disco-0.5.0/disco/pipelines/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-22 23:51:03.000000 NREL-disco-0.5.0/disco/postprocess/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-22 23:50:55.000000 NREL-disco-0.5.0/disco/postprocess/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-22 23:51:03.000000 NREL-disco-0.5.0/disco/postprocess/config/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-22 23:50:55.000000 NREL-disco-0.5.0/disco/postprocess/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12196 2023-11-22 23:50:55.000000 NREL-disco-0.5.0/disco/postprocess/hosting_capacity.py
--rw-r--r--   0 runner    (1001) docker     (127)     6127 2023-11-22 23:50:55.000000 NREL-disco-0.5.0/disco/postprocess/hosting_capacity_from_pydss.py
--rw-r--r--   0 runner    (1001) docker     (127)     3866 2023-11-22 23:50:55.000000 NREL-disco-0.5.0/disco/postprocess/plots.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-22 23:51:03.000000 NREL-disco-0.5.0/disco/pydss/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-22 23:50:55.000000 NREL-disco-0.5.0/disco/pydss/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      548 2023-11-22 23:50:55.000000 NREL-disco-0.5.0/disco/pydss/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     4845 2023-11-22 23:50:55.000000 NREL-disco-0.5.0/disco/pydss/prescreen_pv_penetration_levels.py
--rw-r--r--   0 runner    (1001) docker     (127)     8148 2023-11-22 23:50:55.000000 NREL-disco-0.5.0/disco/pydss/pydss_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)    11329 2023-11-22 23:50:55.000000 NREL-disco-0.5.0/disco/pydss/pydss_configuration_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    12428 2023-11-22 23:50:55.000000 NREL-disco-0.5.0/disco/pydss/pydss_simulation_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      956 2023-11-22 23:50:55.000000 NREL-disco-0.5.0/disco/pydss/pydss_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-22 23:51:03.000000 NREL-disco-0.5.0/disco/sources/
--rw-r--r--   0 runner    (1001) docker     (127)      203 2023-11-22 23:50:55.000000 NREL-disco-0.5.0/disco/sources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21523 2023-11-22 23:50:55.000000 NREL-disco-0.5.0/disco/sources/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-22 23:51:03.000000 NREL-disco-0.5.0/disco/sources/epri/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2023-11-22 23:50:55.000000 NREL-disco-0.5.0/disco/sources/epri/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2503 2023-11-22 23:50:55.000000 NREL-disco-0.5.0/disco/sources/epri/download.py
--rw-r--r--   0 runner    (1001) docker     (127)     8356 2023-11-22 23:50:55.000000 NREL-disco-0.5.0/disco/sources/epri/epri_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2343 2023-11-22 23:50:55.000000 NREL-disco-0.5.0/disco/sources/factory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-22 23:51:03.000000 NREL-disco-0.5.0/disco/sources/gem/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2023-11-22 23:50:55.000000 NREL-disco-0.5.0/disco/sources/gem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      577 2023-11-22 23:50:55.000000 NREL-disco-0.5.0/disco/sources/gem/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     2598 2023-11-22 23:50:55.000000 NREL-disco-0.5.0/disco/sources/gem/gem_model.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    15311 2023-11-22 23:50:55.000000 NREL-disco-0.5.0/disco/sources/gem/make_element_bus_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)      507 2023-11-22 23:50:55.000000 NREL-disco-0.5.0/disco/sources/gem/model_input_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)    17044 2023-11-22 23:50:55.000000 NREL-disco-0.5.0/disco/sources/gem/open_dss_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-22 23:51:03.000000 NREL-disco-0.5.0/disco/sources/source_tree_1/
--rw-r--r--   0 runner    (1001) docker     (127)      113 2023-11-22 23:50:55.000000 NREL-disco-0.5.0/disco/sources/source_tree_1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    77557 2023-11-22 23:50:55.000000 NREL-disco-0.5.0/disco/sources/source_tree_1/pv_deployments.py
--rw-r--r--   0 runner    (1001) docker     (127)    30437 2023-11-22 23:50:55.000000 NREL-disco-0.5.0/disco/sources/source_tree_1/source_tree_1_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    11890 2023-11-22 23:50:55.000000 NREL-disco-0.5.0/disco/sources/source_tree_1/source_tree_1_model_inputs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-22 23:51:03.000000 NREL-disco-0.5.0/disco/sources/source_tree_2/
--rw-r--r--   0 runner    (1001) docker     (127)      113 2023-11-22 23:50:55.000000 NREL-disco-0.5.0/disco/sources/source_tree_2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12562 2023-11-22 23:50:55.000000 NREL-disco-0.5.0/disco/sources/source_tree_2/source_tree_2_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    12224 2023-11-22 23:50:55.000000 NREL-disco-0.5.0/disco/sources/source_tree_2/source_tree_2_model_inputs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-22 23:51:03.000000 NREL-disco-0.5.0/disco/storage/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-22 23:50:55.000000 NREL-disco-0.5.0/disco/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3787 2023-11-22 23:50:55.000000 NREL-disco-0.5.0/disco/storage/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    10406 2023-11-22 23:50:55.000000 NREL-disco-0.5.0/disco/storage/db.py
--rw-r--r--   0 runner    (1001) docker     (127)       72 2023-11-22 23:50:55.000000 NREL-disco-0.5.0/disco/storage/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    12088 2023-11-22 23:50:55.000000 NREL-disco-0.5.0/disco/storage/ingesters.py
--rw-r--r--   0 runner    (1001) docker     (127)     6942 2023-11-22 23:50:55.000000 NREL-disco-0.5.0/disco/storage/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    22410 2023-11-22 23:50:55.000000 NREL-disco-0.5.0/disco/storage/parsers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-22 23:51:03.000000 NREL-disco-0.5.0/disco/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-22 23:50:55.000000 NREL-disco-0.5.0/disco/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      582 2023-11-22 23:50:55.000000 NREL-disco-0.5.0/disco/utils/custom_encoders.py
--rw-r--r--   0 runner    (1001) docker     (127)     2776 2023-11-22 23:50:55.000000 NREL-disco-0.5.0/disco/utils/custom_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     2015 2023-11-22 23:50:55.000000 NREL-disco-0.5.0/disco/utils/dss_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2696 2023-11-22 23:50:55.000000 NREL-disco-0.5.0/disco/utils/failing_test_bisector.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2023-11-22 23:50:55.000000 NREL-disco-0.5.0/disco/version.py
--rw-r--r--   0 runner    (1001) docker     (127)       85 2023-11-22 23:50:55.000000 NREL-disco-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-22 23:51:03.000000 NREL-disco-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3957 2023-11-22 23:50:55.000000 NREL-disco-0.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-22 23:51:03.000000 NREL-disco-0.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-22 23:50:55.000000 NREL-disco-0.5.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2023-11-22 23:50:55.000000 NREL-disco-0.5.0/tests/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2023-11-22 23:50:55.000000 NREL-disco-0.5.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 21:28:11.000000 NREL-disco-0.5.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 21:28:11.000000 NREL-disco-0.5.1/NREL_disco.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-04-07 21:28:11.000000 NREL-disco-0.5.1/NREL_disco.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5350 2024-04-07 21:28:11.000000 NREL-disco-0.5.1/NREL_disco.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 21:28:11.000000 NREL-disco-0.5.1/NREL_disco.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-07 21:28:11.000000 NREL-disco-0.5.1/NREL_disco.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 21:28:11.000000 NREL-disco-0.5.1/NREL_disco.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-07 21:28:11.000000 NREL-disco-0.5.1/NREL_disco.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-07 21:28:11.000000 NREL-disco-0.5.1/NREL_disco.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-04-07 21:28:11.000000 NREL-disco-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-07 21:27:56.000000 NREL-disco-0.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 21:28:11.000000 NREL-disco-0.5.1/disco/
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-07 21:27:56.000000 NREL-disco-0.5.1/disco/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 21:28:11.000000 NREL-disco-0.5.1/disco/analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-07 21:27:56.000000 NREL-disco-0.5.1/disco/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6175 2024-04-07 21:27:56.000000 NREL-disco-0.5.1/disco/analysis/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-07 21:27:56.000000 NREL-disco-0.5.1/disco/analysis/configure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-04-07 21:27:56.000000 NREL-disco-0.5.1/disco/analysis/input.py
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-07 21:27:56.000000 NREL-disco-0.5.1/disco/analysis/option.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7254 2024-04-07 21:27:56.000000 NREL-disco-0.5.1/disco/analysis/postprocess_time_series.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25140 2024-04-07 21:27:56.000000 NREL-disco-0.5.1/disco/analysis/snapshot_impact_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-04-07 21:27:56.000000 NREL-disco-0.5.1/disco/analysis/time_series_impact_analysis.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 21:28:11.000000 NREL-disco-0.5.1/disco/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 21:27:56.000000 NREL-disco-0.5.1/disco/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2334 2024-04-07 21:27:56.000000 NREL-disco-0.5.1/disco/cli/cba_post_process.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2231 2024-04-07 21:27:56.000000 NREL-disco-0.5.1/disco/cli/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4070 2024-04-07 21:27:56.000000 NREL-disco-0.5.1/disco/cli/compute_cba.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3114 2024-04-07 21:27:56.000000 NREL-disco-0.5.1/disco/cli/compute_hosting_capacity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5675 2024-04-07 21:27:56.000000 NREL-disco-0.5.1/disco/cli/compute_pv_swad.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5450 2024-04-07 21:27:56.000000 NREL-disco-0.5.1/disco/cli/compute_snapshot_hosting_capacity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-04-07 21:27:56.000000 NREL-disco-0.5.1/disco/cli/compute_snapshot_impact_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-04-07 21:27:56.000000 NREL-disco-0.5.1/disco/cli/compute_time_series_hosting_capacity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-04-07 21:27:56.000000 NREL-disco-0.5.1/disco/cli/compute_time_series_impact_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-04-07 21:27:56.000000 NREL-disco-0.5.1/disco/cli/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9235 2024-04-07 21:27:56.000000 NREL-disco-0.5.1/disco/cli/config_generic_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9581 2024-04-07 21:27:56.000000 NREL-disco-0.5.1/disco/cli/config_snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10675 2024-04-07 21:27:56.000000 NREL-disco-0.5.1/disco/cli/config_time_series.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-04-07 21:27:56.000000 NREL-disco-0.5.1/disco/cli/config_upgrade.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2395 2024-04-07 21:27:56.000000 NREL-disco-0.5.1/disco/cli/configure_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9550 2024-04-07 21:27:56.000000 NREL-disco-0.5.1/disco/cli/create_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-04-07 21:27:56.000000 NREL-disco-0.5.1/disco/cli/disco.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-07 21:27:56.000000 NREL-disco-0.5.1/disco/cli/disco_internal.py
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-04-07 21:27:56.000000 NREL-disco-0.5.1/disco/cli/download_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-04-07 21:27:56.000000 NREL-disco-0.5.1/disco/cli/ingest_tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10456 2024-04-07 21:27:56.000000 NREL-disco-0.5.1/disco/cli/make_cba_tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10771 2024-04-07 21:27:56.000000 NREL-disco-0.5.1/disco/cli/make_summary_tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4689 2024-04-07 21:27:56.000000 NREL-disco-0.5.1/disco/cli/make_upgrade_tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2024-04-07 21:27:56.000000 NREL-disco-0.5.1/disco/cli/plots.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5247 2024-04-07 21:27:56.000000 NREL-disco-0.5.1/disco/cli/prescreen_pv_penetration_levels.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10998 2024-04-07 21:27:56.000000 NREL-disco-0.5.1/disco/cli/pv_deployments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-04-07 21:27:56.000000 NREL-disco-0.5.1/disco/cli/pydss_hosting_capacity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-04-07 21:27:56.000000 NREL-disco-0.5.1/disco/cli/simulation_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6787 2024-04-07 21:27:56.000000 NREL-disco-0.5.1/disco/cli/summarize_hosting_capacity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2601 2024-04-07 21:27:56.000000 NREL-disco-0.5.1/disco/cli/transform_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13454 2024-04-07 21:27:56.000000 NREL-disco-0.5.1/disco/cli/upgrade_cost_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-07 21:27:56.000000 NREL-disco-0.5.1/disco/common.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 21:28:11.000000 NREL-disco-0.5.1/disco/distribution/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 21:27:56.000000 NREL-disco-0.5.1/disco/distribution/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3645 2024-04-07 21:27:56.000000 NREL-disco-0.5.1/disco/distribution/deployment_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-07 21:27:56.000000 NREL-disco-0.5.1/disco/distribution/distribution_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4691 2024-04-07 21:27:56.000000 NREL-disco-0.5.1/disco/distribution/distribution_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4482 2024-04-07 21:27:56.000000 NREL-disco-0.5.1/disco/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-07 21:27:56.000000 NREL-disco-0.5.1/disco/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5678 2024-04-07 21:27:56.000000 NREL-disco-0.5.1/disco/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 21:28:11.000000 NREL-disco-0.5.1/disco/extensions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 21:27:56.000000 NREL-disco-0.5.1/disco/extensions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 21:28:11.000000 NREL-disco-0.5.1/disco/extensions/pydss_simulation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 21:27:56.000000 NREL-disco-0.5.1/disco/extensions/pydss_simulation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-04-07 21:27:56.000000 NREL-disco-0.5.1/disco/extensions/pydss_simulation/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2904 2024-04-07 21:27:56.000000 NREL-disco-0.5.1/disco/extensions/pydss_simulation/estimate_run_minutes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9764 2024-04-07 21:27:56.000000 NREL-disco-0.5.1/disco/extensions/pydss_simulation/pydss_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-07 21:27:56.000000 NREL-disco-0.5.1/disco/extensions/pydss_simulation/pydss_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6685 2024-04-07 21:27:56.000000 NREL-disco-0.5.1/disco/extensions/pydss_simulation/pydss_simulation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-07 21:27:56.000000 NREL-disco-0.5.1/disco/extensions/pydss_simulation/time_series_impact_analysis_configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 21:28:11.000000 NREL-disco-0.5.1/disco/extensions/upgrade_simulation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 21:27:56.000000 NREL-disco-0.5.1/disco/extensions/upgrade_simulation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3050 2024-04-07 21:27:56.000000 NREL-disco-0.5.1/disco/extensions/upgrade_simulation/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2469 2024-04-07 21:27:56.000000 NREL-disco-0.5.1/disco/extensions/upgrade_simulation/upgrade_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-07 21:27:56.000000 NREL-disco-0.5.1/disco/extensions/upgrade_simulation/upgrade_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-07 21:27:56.000000 NREL-disco-0.5.1/disco/extensions/upgrade_simulation/upgrade_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7040 2024-04-07 21:27:56.000000 NREL-disco-0.5.1/disco/extensions/upgrade_simulation/upgrade_simulation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 21:28:11.000000 NREL-disco-0.5.1/disco/extensions/upgrade_simulation/upgrades/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 21:27:56.000000 NREL-disco-0.5.1/disco/extensions/upgrade_simulation/upgrades/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21649 2024-04-07 21:27:56.000000 NREL-disco-0.5.1/disco/extensions/upgrade_simulation/upgrades/automated_thermal_upgrades.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23549 2024-04-07 21:27:56.000000 NREL-disco-0.5.1/disco/extensions/upgrade_simulation/upgrades/automated_voltage_upgrades.py
+-rw-r--r--   0 runner    (1001) docker     (127)    92378 2024-04-07 21:27:56.000000 NREL-disco-0.5.1/disco/extensions/upgrade_simulation/upgrades/common_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31891 2024-04-07 21:27:56.000000 NREL-disco-0.5.1/disco/extensions/upgrade_simulation/upgrades/cost_computation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-04-07 21:27:56.000000 NREL-disco-0.5.1/disco/extensions/upgrade_simulation/upgrades/fixed_upgrade_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-04-07 21:27:56.000000 NREL-disco-0.5.1/disco/extensions/upgrade_simulation/upgrades/pydss_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33131 2024-04-07 21:27:56.000000 NREL-disco-0.5.1/disco/extensions/upgrade_simulation/upgrades/thermal_upgrade_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)   129611 2024-04-07 21:27:56.000000 NREL-disco-0.5.1/disco/extensions/upgrade_simulation/upgrades/voltage_upgrade_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 21:28:11.000000 NREL-disco-0.5.1/disco/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 21:27:56.000000 NREL-disco-0.5.1/disco/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9698 2024-04-07 21:27:56.000000 NREL-disco-0.5.1/disco/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-04-07 21:27:56.000000 NREL-disco-0.5.1/disco/models/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5537 2024-04-07 21:27:56.000000 NREL-disco-0.5.1/disco/models/power_flow_generic_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-07 21:27:56.000000 NREL-disco-0.5.1/disco/models/snapshot_impact_analysis_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-04-07 21:27:56.000000 NREL-disco-0.5.1/disco/models/time_series_analysis_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15566 2024-04-07 21:27:56.000000 NREL-disco-0.5.1/disco/models/upgrade_cost_analysis_equipment_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30076 2024-04-07 21:27:56.000000 NREL-disco-0.5.1/disco/models/upgrade_cost_analysis_generic_input_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14951 2024-04-07 21:27:56.000000 NREL-disco-0.5.1/disco/models/upgrade_cost_analysis_generic_output_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-07 21:27:56.000000 NREL-disco-0.5.1/disco/models/upgrade_cost_analysis_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-04-07 21:27:56.000000 NREL-disco-0.5.1/disco/models/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 21:28:11.000000 NREL-disco-0.5.1/disco/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 21:27:56.000000 NREL-disco-0.5.1/disco/pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-04-07 21:27:56.000000 NREL-disco-0.5.1/disco/pipelines/auto_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13125 2024-04-07 21:27:56.000000 NREL-disco-0.5.1/disco/pipelines/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13022 2024-04-07 21:27:56.000000 NREL-disco-0.5.1/disco/pipelines/creator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-07 21:27:56.000000 NREL-disco-0.5.1/disco/pipelines/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-04-07 21:27:56.000000 NREL-disco-0.5.1/disco/pipelines/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-04-07 21:27:56.000000 NREL-disco-0.5.1/disco/pipelines/update_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-04-07 21:27:56.000000 NREL-disco-0.5.1/disco/pipelines/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 21:28:11.000000 NREL-disco-0.5.1/disco/postprocess/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 21:27:56.000000 NREL-disco-0.5.1/disco/postprocess/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 21:28:11.000000 NREL-disco-0.5.1/disco/postprocess/config/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 21:27:56.000000 NREL-disco-0.5.1/disco/postprocess/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12196 2024-04-07 21:27:56.000000 NREL-disco-0.5.1/disco/postprocess/hosting_capacity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6127 2024-04-07 21:27:56.000000 NREL-disco-0.5.1/disco/postprocess/hosting_capacity_from_pydss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3866 2024-04-07 21:27:56.000000 NREL-disco-0.5.1/disco/postprocess/plots.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 21:28:11.000000 NREL-disco-0.5.1/disco/pydss/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 21:27:56.000000 NREL-disco-0.5.1/disco/pydss/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-07 21:27:56.000000 NREL-disco-0.5.1/disco/pydss/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4845 2024-04-07 21:27:56.000000 NREL-disco-0.5.1/disco/pydss/prescreen_pv_penetration_levels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8148 2024-04-07 21:27:56.000000 NREL-disco-0.5.1/disco/pydss/pydss_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11329 2024-04-07 21:27:56.000000 NREL-disco-0.5.1/disco/pydss/pydss_configuration_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12428 2024-04-07 21:27:56.000000 NREL-disco-0.5.1/disco/pydss/pydss_simulation_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      956 2024-04-07 21:27:56.000000 NREL-disco-0.5.1/disco/pydss/pydss_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 21:28:11.000000 NREL-disco-0.5.1/disco/sources/
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-07 21:27:56.000000 NREL-disco-0.5.1/disco/sources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21523 2024-04-07 21:27:56.000000 NREL-disco-0.5.1/disco/sources/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 21:28:11.000000 NREL-disco-0.5.1/disco/sources/epri/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-07 21:27:56.000000 NREL-disco-0.5.1/disco/sources/epri/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2503 2024-04-07 21:27:56.000000 NREL-disco-0.5.1/disco/sources/epri/download.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8356 2024-04-07 21:27:56.000000 NREL-disco-0.5.1/disco/sources/epri/epri_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2343 2024-04-07 21:27:56.000000 NREL-disco-0.5.1/disco/sources/factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 21:28:11.000000 NREL-disco-0.5.1/disco/sources/gem/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-07 21:27:56.000000 NREL-disco-0.5.1/disco/sources/gem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-04-07 21:27:56.000000 NREL-disco-0.5.1/disco/sources/gem/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2598 2024-04-07 21:27:56.000000 NREL-disco-0.5.1/disco/sources/gem/gem_model.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    15311 2024-04-07 21:27:56.000000 NREL-disco-0.5.1/disco/sources/gem/make_element_bus_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-04-07 21:27:56.000000 NREL-disco-0.5.1/disco/sources/gem/model_input_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17044 2024-04-07 21:27:56.000000 NREL-disco-0.5.1/disco/sources/gem/open_dss_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 21:28:11.000000 NREL-disco-0.5.1/disco/sources/source_tree_1/
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-07 21:27:56.000000 NREL-disco-0.5.1/disco/sources/source_tree_1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    77557 2024-04-07 21:27:56.000000 NREL-disco-0.5.1/disco/sources/source_tree_1/pv_deployments.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30437 2024-04-07 21:27:56.000000 NREL-disco-0.5.1/disco/sources/source_tree_1/source_tree_1_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11890 2024-04-07 21:27:56.000000 NREL-disco-0.5.1/disco/sources/source_tree_1/source_tree_1_model_inputs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 21:28:11.000000 NREL-disco-0.5.1/disco/sources/source_tree_2/
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-07 21:27:56.000000 NREL-disco-0.5.1/disco/sources/source_tree_2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12562 2024-04-07 21:27:56.000000 NREL-disco-0.5.1/disco/sources/source_tree_2/source_tree_2_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12224 2024-04-07 21:27:56.000000 NREL-disco-0.5.1/disco/sources/source_tree_2/source_tree_2_model_inputs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 21:28:11.000000 NREL-disco-0.5.1/disco/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 21:27:56.000000 NREL-disco-0.5.1/disco/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3787 2024-04-07 21:27:56.000000 NREL-disco-0.5.1/disco/storage/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10406 2024-04-07 21:27:56.000000 NREL-disco-0.5.1/disco/storage/db.py
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-07 21:27:56.000000 NREL-disco-0.5.1/disco/storage/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12088 2024-04-07 21:27:56.000000 NREL-disco-0.5.1/disco/storage/ingesters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6942 2024-04-07 21:27:56.000000 NREL-disco-0.5.1/disco/storage/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22410 2024-04-07 21:27:56.000000 NREL-disco-0.5.1/disco/storage/parsers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 21:28:11.000000 NREL-disco-0.5.1/disco/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 21:27:56.000000 NREL-disco-0.5.1/disco/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-07 21:27:56.000000 NREL-disco-0.5.1/disco/utils/custom_encoders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2776 2024-04-07 21:27:56.000000 NREL-disco-0.5.1/disco/utils/custom_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-04-07 21:27:56.000000 NREL-disco-0.5.1/disco/utils/dss_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-04-07 21:27:56.000000 NREL-disco-0.5.1/disco/utils/failing_test_bisector.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-07 21:27:56.000000 NREL-disco-0.5.1/disco/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-07 21:27:56.000000 NREL-disco-0.5.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 21:28:11.000000 NREL-disco-0.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4067 2024-04-07 21:27:56.000000 NREL-disco-0.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 21:28:11.000000 NREL-disco-0.5.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 21:27:56.000000 NREL-disco-0.5.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-04-07 21:27:56.000000 NREL-disco-0.5.1/tests/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-04-07 21:27:56.000000 NREL-disco-0.5.1/tests/conftest.py
```

### Comparing `NREL-disco-0.5.0/NREL_disco.egg-info/PKG-INFO` & `NREL-disco-0.5.1/NREL_disco.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NREL-disco
-Version: 0.5.0
+Version: 0.5.1
 Summary: DISCO
 Home-page: https://github.com/NREL/disco
 Maintainer-email: daniel.thom@nrel.gov
 License: BSD license
 Description: # DISCO
         DISCO source code repository
```

### Comparing `NREL-disco-0.5.0/NREL_disco.egg-info/SOURCES.txt` & `NREL-disco-0.5.1/NREL_disco.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `NREL-disco-0.5.0/PKG-INFO` & `NREL-disco-0.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NREL-disco
-Version: 0.5.0
+Version: 0.5.1
 Summary: DISCO
 Home-page: https://github.com/NREL/disco
 Maintainer-email: daniel.thom@nrel.gov
 License: BSD license
 Description: # DISCO
         DISCO source code repository
```

### Comparing `NREL-disco-0.5.0/disco/analysis/analysis.py` & `NREL-disco-0.5.1/disco/analysis/analysis.py`

 * *Files identical despite different names*

### Comparing `NREL-disco-0.5.0/disco/analysis/configure.py` & `NREL-disco-0.5.1/disco/analysis/configure.py`

 * *Files identical despite different names*

### Comparing `NREL-disco-0.5.0/disco/analysis/input.py` & `NREL-disco-0.5.1/disco/analysis/input.py`

 * *Files identical despite different names*

### Comparing `NREL-disco-0.5.0/disco/analysis/postprocess_time_series.py` & `NREL-disco-0.5.1/disco/analysis/postprocess_time_series.py`

 * *Files identical despite different names*

### Comparing `NREL-disco-0.5.0/disco/analysis/snapshot_impact_analysis.py` & `NREL-disco-0.5.1/disco/analysis/snapshot_impact_analysis.py`

 * *Files identical despite different names*

### Comparing `NREL-disco-0.5.0/disco/analysis/time_series_impact_analysis.py` & `NREL-disco-0.5.1/disco/analysis/time_series_impact_analysis.py`

 * *Files identical despite different names*

### Comparing `NREL-disco-0.5.0/disco/cli/cba_post_process.py` & `NREL-disco-0.5.1/disco/cli/cba_post_process.py`

 * *Files identical despite different names*

### Comparing `NREL-disco-0.5.0/disco/cli/common.py` & `NREL-disco-0.5.1/disco/cli/common.py`

 * *Files identical despite different names*

### Comparing `NREL-disco-0.5.0/disco/cli/compute_cba.py` & `NREL-disco-0.5.1/disco/cli/compute_cba.py`

 * *Files identical despite different names*

### Comparing `NREL-disco-0.5.0/disco/cli/compute_hosting_capacity.py` & `NREL-disco-0.5.1/disco/cli/compute_hosting_capacity.py`

 * *Files identical despite different names*

### Comparing `NREL-disco-0.5.0/disco/cli/compute_pv_swad.py` & `NREL-disco-0.5.1/disco/cli/compute_pv_swad.py`

 * *Files identical despite different names*

### Comparing `NREL-disco-0.5.0/disco/cli/compute_snapshot_hosting_capacity.py` & `NREL-disco-0.5.1/disco/cli/compute_snapshot_hosting_capacity.py`

 * *Files identical despite different names*

### Comparing `NREL-disco-0.5.0/disco/cli/compute_snapshot_impact_analysis.py` & `NREL-disco-0.5.1/disco/cli/compute_snapshot_impact_analysis.py`

 * *Files identical despite different names*

### Comparing `NREL-disco-0.5.0/disco/cli/compute_time_series_hosting_capacity.py` & `NREL-disco-0.5.1/disco/cli/compute_time_series_hosting_capacity.py`

 * *Files identical despite different names*

### Comparing `NREL-disco-0.5.0/disco/cli/compute_time_series_impact_analysis.py` & `NREL-disco-0.5.1/disco/cli/compute_time_series_impact_analysis.py`

 * *Files identical despite different names*

### Comparing `NREL-disco-0.5.0/disco/cli/config_generic_models.py` & `NREL-disco-0.5.1/disco/cli/config_generic_models.py`

 * *Files identical despite different names*

### Comparing `NREL-disco-0.5.0/disco/cli/config_snapshot.py` & `NREL-disco-0.5.1/disco/cli/config_snapshot.py`

 * *Files identical despite different names*

### Comparing `NREL-disco-0.5.0/disco/cli/config_time_series.py` & `NREL-disco-0.5.1/disco/cli/config_time_series.py`

 * *Files identical despite different names*

### Comparing `NREL-disco-0.5.0/disco/cli/config_upgrade.py` & `NREL-disco-0.5.1/disco/cli/config_upgrade.py`

 * *Files identical despite different names*

### Comparing `NREL-disco-0.5.0/disco/cli/configure_analysis.py` & `NREL-disco-0.5.1/disco/cli/configure_analysis.py`

 * *Files identical despite different names*

### Comparing `NREL-disco-0.5.0/disco/cli/create_pipeline.py` & `NREL-disco-0.5.1/disco/cli/create_pipeline.py`

 * *Files identical despite different names*

### Comparing `NREL-disco-0.5.0/disco/cli/disco.py` & `NREL-disco-0.5.1/disco/cli/disco.py`

 * *Files identical despite different names*

### Comparing `NREL-disco-0.5.0/disco/cli/disco_internal.py` & `NREL-disco-0.5.1/disco/cli/disco_internal.py`

 * *Files identical despite different names*

### Comparing `NREL-disco-0.5.0/disco/cli/download_source.py` & `NREL-disco-0.5.1/disco/cli/download_source.py`

 * *Files identical despite different names*

### Comparing `NREL-disco-0.5.0/disco/cli/ingest_tables.py` & `NREL-disco-0.5.1/disco/cli/ingest_tables.py`

 * *Files identical despite different names*

### Comparing `NREL-disco-0.5.0/disco/cli/make_cba_tables.py` & `NREL-disco-0.5.1/disco/cli/make_cba_tables.py`

 * *Files identical despite different names*

### Comparing `NREL-disco-0.5.0/disco/cli/make_summary_tables.py` & `NREL-disco-0.5.1/disco/cli/make_summary_tables.py`

 * *Files identical despite different names*

### Comparing `NREL-disco-0.5.0/disco/cli/make_upgrade_tables.py` & `NREL-disco-0.5.1/disco/cli/make_upgrade_tables.py`

 * *Files identical despite different names*

### Comparing `NREL-disco-0.5.0/disco/cli/plots.py` & `NREL-disco-0.5.1/disco/cli/plots.py`

 * *Files identical despite different names*

### Comparing `NREL-disco-0.5.0/disco/cli/prescreen_pv_penetration_levels.py` & `NREL-disco-0.5.1/disco/cli/prescreen_pv_penetration_levels.py`

 * *Files identical despite different names*

### Comparing `NREL-disco-0.5.0/disco/cli/pv_deployments.py` & `NREL-disco-0.5.1/disco/cli/pv_deployments.py`

 * *Files identical despite different names*

### Comparing `NREL-disco-0.5.0/disco/cli/pydss_hosting_capacity.py` & `NREL-disco-0.5.1/disco/cli/pydss_hosting_capacity.py`

 * *Files identical despite different names*

### Comparing `NREL-disco-0.5.0/disco/cli/simulation_models.py` & `NREL-disco-0.5.1/disco/cli/simulation_models.py`

 * *Files identical despite different names*

### Comparing `NREL-disco-0.5.0/disco/cli/summarize_hosting_capacity.py` & `NREL-disco-0.5.1/disco/cli/summarize_hosting_capacity.py`

 * *Files identical despite different names*

### Comparing `NREL-disco-0.5.0/disco/cli/transform_model.py` & `NREL-disco-0.5.1/disco/cli/transform_model.py`

 * *Files identical despite different names*

### Comparing `NREL-disco-0.5.0/disco/cli/upgrade_cost_analysis.py` & `NREL-disco-0.5.1/disco/cli/upgrade_cost_analysis.py`

 * *Files identical despite different names*

### Comparing `NREL-disco-0.5.0/disco/distribution/deployment_parameters.py` & `NREL-disco-0.5.1/disco/distribution/deployment_parameters.py`

 * *Files identical despite different names*

### Comparing `NREL-disco-0.5.0/disco/distribution/distribution_configuration.py` & `NREL-disco-0.5.1/disco/distribution/distribution_configuration.py`

 * *Files identical despite different names*

### Comparing `NREL-disco-0.5.0/disco/distribution/distribution_inputs.py` & `NREL-disco-0.5.1/disco/distribution/distribution_inputs.py`

 * *Files identical despite different names*

### Comparing `NREL-disco-0.5.0/disco/enums.py` & `NREL-disco-0.5.1/disco/enums.py`

 * *Files identical despite different names*

### Comparing `NREL-disco-0.5.0/disco/exceptions.py` & `NREL-disco-0.5.1/disco/exceptions.py`

 * *Files identical despite different names*

### Comparing `NREL-disco-0.5.0/disco/extensions/pydss_simulation/cli.py` & `NREL-disco-0.5.1/disco/extensions/pydss_simulation/cli.py`

 * *Files identical despite different names*

### Comparing `NREL-disco-0.5.0/disco/extensions/pydss_simulation/estimate_run_minutes.py` & `NREL-disco-0.5.1/disco/extensions/pydss_simulation/estimate_run_minutes.py`

 * *Files identical despite different names*

### Comparing `NREL-disco-0.5.0/disco/extensions/pydss_simulation/pydss_configuration.py` & `NREL-disco-0.5.1/disco/extensions/pydss_simulation/pydss_configuration.py`

 * *Files identical despite different names*

### Comparing `NREL-disco-0.5.0/disco/extensions/pydss_simulation/pydss_simulation.py` & `NREL-disco-0.5.1/disco/extensions/pydss_simulation/pydss_simulation.py`

 * *Files identical despite different names*

### Comparing `NREL-disco-0.5.0/disco/extensions/pydss_simulation/time_series_impact_analysis_configuration.py` & `NREL-disco-0.5.1/disco/extensions/pydss_simulation/time_series_impact_analysis_configuration.py`

 * *Files identical despite different names*

### Comparing `NREL-disco-0.5.0/disco/extensions/upgrade_simulation/cli.py` & `NREL-disco-0.5.1/disco/extensions/upgrade_simulation/cli.py`

 * *Files identical despite different names*

### Comparing `NREL-disco-0.5.0/disco/extensions/upgrade_simulation/upgrade_configuration.py` & `NREL-disco-0.5.1/disco/extensions/upgrade_simulation/upgrade_configuration.py`

 * *Files identical despite different names*

### Comparing `NREL-disco-0.5.0/disco/extensions/upgrade_simulation/upgrade_inputs.py` & `NREL-disco-0.5.1/disco/extensions/upgrade_simulation/upgrade_inputs.py`

 * *Files identical despite different names*

### Comparing `NREL-disco-0.5.0/disco/extensions/upgrade_simulation/upgrade_simulation.py` & `NREL-disco-0.5.1/disco/extensions/upgrade_simulation/upgrade_simulation.py`

 * *Files identical despite different names*

### Comparing `NREL-disco-0.5.0/disco/extensions/upgrade_simulation/upgrades/automated_thermal_upgrades.py` & `NREL-disco-0.5.1/disco/extensions/upgrade_simulation/upgrades/automated_thermal_upgrades.py`

 * *Files identical despite different names*

### Comparing `NREL-disco-0.5.0/disco/extensions/upgrade_simulation/upgrades/automated_voltage_upgrades.py` & `NREL-disco-0.5.1/disco/extensions/upgrade_simulation/upgrades/automated_voltage_upgrades.py`

 * *Files identical despite different names*

### Comparing `NREL-disco-0.5.0/disco/extensions/upgrade_simulation/upgrades/common_functions.py` & `NREL-disco-0.5.1/disco/extensions/upgrade_simulation/upgrades/common_functions.py`

 * *Files identical despite different names*

### Comparing `NREL-disco-0.5.0/disco/extensions/upgrade_simulation/upgrades/cost_computation.py` & `NREL-disco-0.5.1/disco/extensions/upgrade_simulation/upgrades/cost_computation.py`

 * *Files identical despite different names*

### Comparing `NREL-disco-0.5.0/disco/extensions/upgrade_simulation/upgrades/fixed_upgrade_parameters.py` & `NREL-disco-0.5.1/disco/extensions/upgrade_simulation/upgrades/fixed_upgrade_parameters.py`

 * *Files identical despite different names*

### Comparing `NREL-disco-0.5.0/disco/extensions/upgrade_simulation/upgrades/pydss_parameters.py` & `NREL-disco-0.5.1/disco/extensions/upgrade_simulation/upgrades/pydss_parameters.py`

 * *Files identical despite different names*

### Comparing `NREL-disco-0.5.0/disco/extensions/upgrade_simulation/upgrades/thermal_upgrade_functions.py` & `NREL-disco-0.5.1/disco/extensions/upgrade_simulation/upgrades/thermal_upgrade_functions.py`

 * *Files identical despite different names*

### Comparing `NREL-disco-0.5.0/disco/extensions/upgrade_simulation/upgrades/voltage_upgrade_functions.py` & `NREL-disco-0.5.1/disco/extensions/upgrade_simulation/upgrades/voltage_upgrade_functions.py`

 * *Files identical despite different names*

### Comparing `NREL-disco-0.5.0/disco/models/base.py` & `NREL-disco-0.5.1/disco/models/base.py`

 * *Files identical despite different names*

### Comparing `NREL-disco-0.5.0/disco/models/factory.py` & `NREL-disco-0.5.1/disco/models/factory.py`

 * *Files identical despite different names*

### Comparing `NREL-disco-0.5.0/disco/models/power_flow_generic_models.py` & `NREL-disco-0.5.1/disco/models/power_flow_generic_models.py`

 * *Files identical despite different names*

### Comparing `NREL-disco-0.5.0/disco/models/snapshot_impact_analysis_model.py` & `NREL-disco-0.5.1/disco/models/snapshot_impact_analysis_model.py`

 * *Files identical despite different names*

### Comparing `NREL-disco-0.5.0/disco/models/time_series_analysis_model.py` & `NREL-disco-0.5.1/disco/models/time_series_analysis_model.py`

 * *Files identical despite different names*

### Comparing `NREL-disco-0.5.0/disco/models/upgrade_cost_analysis_equipment_model.py` & `NREL-disco-0.5.1/disco/models/upgrade_cost_analysis_equipment_model.py`

 * *Files identical despite different names*

### Comparing `NREL-disco-0.5.0/disco/models/upgrade_cost_analysis_generic_input_model.py` & `NREL-disco-0.5.1/disco/models/upgrade_cost_analysis_generic_input_model.py`

 * *Files identical despite different names*

### Comparing `NREL-disco-0.5.0/disco/models/upgrade_cost_analysis_generic_output_model.py` & `NREL-disco-0.5.1/disco/models/upgrade_cost_analysis_generic_output_model.py`

 * *Files identical despite different names*

### Comparing `NREL-disco-0.5.0/disco/models/upgrade_cost_analysis_model.py` & `NREL-disco-0.5.1/disco/models/upgrade_cost_analysis_model.py`

 * *Files identical despite different names*

### Comparing `NREL-disco-0.5.0/disco/models/utils.py` & `NREL-disco-0.5.1/disco/models/utils.py`

 * *Files identical despite different names*

### Comparing `NREL-disco-0.5.0/disco/pipelines/auto_config.py` & `NREL-disco-0.5.1/disco/pipelines/auto_config.py`

 * *Files identical despite different names*

### Comparing `NREL-disco-0.5.0/disco/pipelines/base.py` & `NREL-disco-0.5.1/disco/pipelines/base.py`

 * *Files identical despite different names*

### Comparing `NREL-disco-0.5.0/disco/pipelines/creator.py` & `NREL-disco-0.5.1/disco/pipelines/creator.py`

 * *Files identical despite different names*

### Comparing `NREL-disco-0.5.0/disco/pipelines/factory.py` & `NREL-disco-0.5.1/disco/pipelines/factory.py`

 * *Files identical despite different names*

### Comparing `NREL-disco-0.5.0/disco/pipelines/update_config.py` & `NREL-disco-0.5.1/disco/pipelines/update_config.py`

 * *Files identical despite different names*

### Comparing `NREL-disco-0.5.0/disco/pipelines/utils.py` & `NREL-disco-0.5.1/disco/pipelines/utils.py`

 * *Files identical despite different names*

### Comparing `NREL-disco-0.5.0/disco/postprocess/hosting_capacity.py` & `NREL-disco-0.5.1/disco/postprocess/hosting_capacity.py`

 * *Files identical despite different names*

### Comparing `NREL-disco-0.5.0/disco/postprocess/hosting_capacity_from_pydss.py` & `NREL-disco-0.5.1/disco/postprocess/hosting_capacity_from_pydss.py`

 * *Files identical despite different names*

### Comparing `NREL-disco-0.5.0/disco/postprocess/plots.py` & `NREL-disco-0.5.1/disco/postprocess/plots.py`

 * *Files identical despite different names*

### Comparing `NREL-disco-0.5.0/disco/pydss/common.py` & `NREL-disco-0.5.1/disco/pydss/common.py`

 * *Files identical despite different names*

### Comparing `NREL-disco-0.5.0/disco/pydss/prescreen_pv_penetration_levels.py` & `NREL-disco-0.5.1/disco/pydss/prescreen_pv_penetration_levels.py`

 * *Files identical despite different names*

### Comparing `NREL-disco-0.5.0/disco/pydss/pydss_analysis.py` & `NREL-disco-0.5.1/disco/pydss/pydss_analysis.py`

 * *Files identical despite different names*

### Comparing `NREL-disco-0.5.0/disco/pydss/pydss_configuration_base.py` & `NREL-disco-0.5.1/disco/pydss/pydss_configuration_base.py`

 * *Files identical despite different names*

### Comparing `NREL-disco-0.5.0/disco/pydss/pydss_simulation_base.py` & `NREL-disco-0.5.1/disco/pydss/pydss_simulation_base.py`

 * *Files identical despite different names*

### Comparing `NREL-disco-0.5.0/disco/pydss/pydss_utils.py` & `NREL-disco-0.5.1/disco/pydss/pydss_utils.py`

 * *Files identical despite different names*

### Comparing `NREL-disco-0.5.0/disco/sources/base.py` & `NREL-disco-0.5.1/disco/sources/base.py`

 * *Files identical despite different names*

### Comparing `NREL-disco-0.5.0/disco/sources/epri/download.py` & `NREL-disco-0.5.1/disco/sources/epri/download.py`

 * *Files identical despite different names*

### Comparing `NREL-disco-0.5.0/disco/sources/epri/epri_model.py` & `NREL-disco-0.5.1/disco/sources/epri/epri_model.py`

 * *Files identical despite different names*

### Comparing `NREL-disco-0.5.0/disco/sources/factory.py` & `NREL-disco-0.5.1/disco/sources/factory.py`

 * *Files identical despite different names*

### Comparing `NREL-disco-0.5.0/disco/sources/gem/factory.py` & `NREL-disco-0.5.1/disco/sources/gem/factory.py`

 * *Files identical despite different names*

### Comparing `NREL-disco-0.5.0/disco/sources/gem/gem_model.py` & `NREL-disco-0.5.1/disco/sources/gem/gem_model.py`

 * *Files identical despite different names*

### Comparing `NREL-disco-0.5.0/disco/sources/gem/make_element_bus_mapping.py` & `NREL-disco-0.5.1/disco/sources/gem/make_element_bus_mapping.py`

 * *Files identical despite different names*

### Comparing `NREL-disco-0.5.0/disco/sources/gem/open_dss_generator.py` & `NREL-disco-0.5.1/disco/sources/gem/open_dss_generator.py`

 * *Files identical despite different names*

### Comparing `NREL-disco-0.5.0/disco/sources/source_tree_1/pv_deployments.py` & `NREL-disco-0.5.1/disco/sources/source_tree_1/pv_deployments.py`

 * *Files identical despite different names*

### Comparing `NREL-disco-0.5.0/disco/sources/source_tree_1/source_tree_1_model.py` & `NREL-disco-0.5.1/disco/sources/source_tree_1/source_tree_1_model.py`

 * *Files identical despite different names*

### Comparing `NREL-disco-0.5.0/disco/sources/source_tree_1/source_tree_1_model_inputs.py` & `NREL-disco-0.5.1/disco/sources/source_tree_1/source_tree_1_model_inputs.py`

 * *Files identical despite different names*

### Comparing `NREL-disco-0.5.0/disco/sources/source_tree_2/source_tree_2_model.py` & `NREL-disco-0.5.1/disco/sources/source_tree_2/source_tree_2_model.py`

 * *Files identical despite different names*

### Comparing `NREL-disco-0.5.0/disco/sources/source_tree_2/source_tree_2_model_inputs.py` & `NREL-disco-0.5.1/disco/sources/source_tree_2/source_tree_2_model_inputs.py`

 * *Files identical despite different names*

### Comparing `NREL-disco-0.5.0/disco/storage/core.py` & `NREL-disco-0.5.1/disco/storage/core.py`

 * *Files identical despite different names*

### Comparing `NREL-disco-0.5.0/disco/storage/db.py` & `NREL-disco-0.5.1/disco/storage/db.py`

 * *Files identical despite different names*

### Comparing `NREL-disco-0.5.0/disco/storage/ingesters.py` & `NREL-disco-0.5.1/disco/storage/ingesters.py`

 * *Files identical despite different names*

### Comparing `NREL-disco-0.5.0/disco/storage/outputs.py` & `NREL-disco-0.5.1/disco/storage/outputs.py`

 * *Files identical despite different names*

### Comparing `NREL-disco-0.5.0/disco/storage/parsers.py` & `NREL-disco-0.5.1/disco/storage/parsers.py`

 * *Files identical despite different names*

### Comparing `NREL-disco-0.5.0/disco/utils/custom_encoders.py` & `NREL-disco-0.5.1/disco/utils/custom_encoders.py`

 * *Files identical despite different names*

### Comparing `NREL-disco-0.5.0/disco/utils/custom_type.py` & `NREL-disco-0.5.1/disco/utils/custom_type.py`

 * *Files identical despite different names*

### Comparing `NREL-disco-0.5.0/disco/utils/dss_utils.py` & `NREL-disco-0.5.1/disco/utils/dss_utils.py`

 * *Files identical despite different names*

### Comparing `NREL-disco-0.5.0/disco/utils/failing_test_bisector.py` & `NREL-disco-0.5.1/disco/utils/failing_test_bisector.py`

 * *Files identical despite different names*

### Comparing `NREL-disco-0.5.0/setup.py` & `NREL-disco-0.5.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -59,24 +59,24 @@
 
 version = lines[0].split()[2].strip('"').strip("'")
 
 install_requires = [
     "NREL-jade~=0.10.0",
     "chevron~=0.14.0",
     "click~=8.0",
-    "dsspy~=3.0.0",
+    "dsspy==3.0.2",  # 3.0.4 has a breaking change
     "filelock~=3.8",
     "matplotlib~=3.6",
     "networkx~=2.8",
     "opendssdirect.py~=0.8.4",
     "openpyxl~=3.0",
-    "pandas~=1.5.0",
+    "pandas >= 2, < 3",
     "pydantic~=2.5.2",
     "seaborn~=0.12.1",
-    "scikit-learn~=1.1",
+    "scikit-learn >= 1.1, < 1.4",  # 1.4 removes the parameter affinity from AgglomerativeClustering
     "sqlalchemy~=1.4",
     "toml~=0.10.0",
 ]
 dev_requires = [
     "flake8",
     "ghp-import",
     "mock>=3.0.0",
```

### Comparing `NREL-disco-0.5.0/tests/common.py` & `NREL-disco-0.5.1/tests/common.py`

 * *Files identical despite different names*

### Comparing `NREL-disco-0.5.0/tests/conftest.py` & `NREL-disco-0.5.1/tests/conftest.py`

 * *Files identical despite different names*

