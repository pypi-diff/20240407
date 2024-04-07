# Comparing `tmp/aind-slurm-rest-0.0.1.tar.gz` & `tmp/aind-slurm-rest-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aind-slurm-rest-0.0.1.tar", last modified: Sun Mar 24 21:16:07 2024, max compression
+gzip compressed data, was "aind-slurm-rest-0.1.0.tar", last modified: Sun Apr  7 21:45:51 2024, max compression
```

## Comparing `aind-slurm-rest-0.0.1.tar` & `aind-slurm-rest-0.1.0.tar`

### file list

```diff
@@ -1,430 +1,432 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 21:16:07.931152 aind-slurm-rest-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-03-24 21:15:50.000000 aind-slurm-rest-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-03-24 21:16:07.931152 aind-slurm-rest-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    28486 2024-03-24 21:15:58.000000 aind-slurm-rest-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 21:16:07.867152 aind-slurm-rest-0.0.1/aind_slurm_rest/
--rw-r--r--   0 runner    (1001) docker     (127)    17265 2024-03-24 21:15:58.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 21:16:07.867152 aind-slurm-rest-0.0.1/aind_slurm_rest/api/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-03-24 21:15:58.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   144779 2024-03-24 21:15:58.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/api/default_api.py
--rw-r--r--   0 runner    (1001) docker     (127)   861002 2024-03-24 21:15:58.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/api/slurm_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    26248 2024-03-24 21:15:58.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/api_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-03-24 21:15:58.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/api_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    15600 2024-03-24 21:15:58.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     5937 2024-03-24 21:15:58.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 21:16:07.899152 aind-slurm-rest-0.0.1/aind_slurm_rest/models/
--rw-r--r--   0 runner    (1001) docker     (127)    16606 2024-03-24 21:15:58.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4437 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0036_account.py
--rw-r--r--   0 runner    (1001) docker     (127)     3602 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0036_account_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2999 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0036_account_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     5372 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0036_association.py
--rw-r--r--   0 runner    (1001) docker     (127)     3622 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0036_association_max.py
--rw-r--r--   0 runner    (1001) docker     (127)     2826 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0036_association_max_jobs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3929 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0036_association_max_tres.py
--rw-r--r--   0 runner    (1001) docker     (127)     3516 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0036_association_max_tres_minutes.py
--rw-r--r--   0 runner    (1001) docker     (127)     3063 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0036_association_max_tres_minutes_per.py
--rw-r--r--   0 runner    (1001) docker     (127)     3570 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0036_association_max_tres_per.py
--rw-r--r--   0 runner    (1001) docker     (127)     2995 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0036_association_short_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     3679 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0036_associations_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     4755 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0036_cluster_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2858 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0036_cluster_info_associations.py
--rw-r--r--   0 runner    (1001) docker     (127)     6817 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0036_config_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2995 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0036_config_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2795 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0036_coordinator_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     5021 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0036_diag.py
--rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0036_error.py
--rw-r--r--   0 runner    (1001) docker     (127)    10498 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0036_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     3154 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0036_job_exit_code.py
--rw-r--r--   0 runner    (1001) docker     (127)     3531 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0036_job_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2701 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0036_job_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     6490 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0036_job_step.py
--rw-r--r--   0 runner    (1001) docker     (127)     3881 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0036_job_step_tres.py
--rw-r--r--   0 runner    (1001) docker     (127)     4667 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0036_job_step_tres_requested.py
--rw-r--r--   0 runner    (1001) docker     (127)     3619 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0036_job_tres.py
--rw-r--r--   0 runner    (1001) docker     (127)     4144 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0036_qos.py
--rw-r--r--   0 runner    (1001) docker     (127)     3521 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0036_qos_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     3142 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0036_qos_limits.py
--rw-r--r--   0 runner    (1001) docker     (127)     4153 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0036_qos_limits_max.py
--rw-r--r--   0 runner    (1001) docker     (127)     2819 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0036_qos_limits_max_jobs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0036_qos_limits_max_jobs_per.py
--rw-r--r--   0 runner    (1001) docker     (127)     3274 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0036_qos_limits_max_tres.py
--rw-r--r--   0 runner    (1001) docker     (127)     2871 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0036_qos_limits_max_tres_minutes.py
--rw-r--r--   0 runner    (1001) docker     (127)     4156 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0036_qos_limits_max_tres_minutes_per.py
--rw-r--r--   0 runner    (1001) docker     (127)     4663 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0036_qos_limits_max_tres_per.py
--rw-r--r--   0 runner    (1001) docker     (127)     3007 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0036_qos_limits_min.py
--rw-r--r--   0 runner    (1001) docker     (127)     2813 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0036_qos_limits_min_tres.py
--rw-r--r--   0 runner    (1001) docker     (127)     3028 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0036_qos_limits_min_tres_per.py
--rw-r--r--   0 runner    (1001) docker     (127)     3023 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0036_response_account_delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     3039 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0036_response_association_delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     3011 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0036_response_cluster_add.py
--rw-r--r--   0 runner    (1001) docker     (127)     3023 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0036_response_cluster_delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     3007 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0036_response_qos_delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     2987 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0036_response_tres.py
--rw-r--r--   0 runner    (1001) docker     (127)     3011 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0036_response_user_delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     3011 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0036_response_user_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     3003 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0036_response_wckey_add.py
--rw-r--r--   0 runner    (1001) docker     (127)     3015 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0036_response_wckey_delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     3789 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0036_tres_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     4303 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0036_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     2828 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0036_user_associations.py
--rw-r--r--   0 runner    (1001) docker     (127)     3549 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0036_user_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     3214 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0036_wckey.py
--rw-r--r--   0 runner    (1001) docker     (127)     3566 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0036_wckey_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     4437 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_account.py
--rw-r--r--   0 runner    (1001) docker     (127)     3602 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_account_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2999 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_account_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     5531 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_association.py
--rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_association_default.py
--rw-r--r--   0 runner    (1001) docker     (127)     3622 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_association_max.py
--rw-r--r--   0 runner    (1001) docker     (127)     3307 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_association_max_jobs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2596 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_association_max_jobs_per.py
--rw-r--r--   0 runner    (1001) docker     (127)     2870 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_association_max_per.py
--rw-r--r--   0 runner    (1001) docker     (127)     2615 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_association_max_per_account.py
--rw-r--r--   0 runner    (1001) docker     (127)     4374 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_association_max_tres.py
--rw-r--r--   0 runner    (1001) docker     (127)     3627 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_association_max_tres_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     3516 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_association_max_tres_minutes.py
--rw-r--r--   0 runner    (1001) docker     (127)     3063 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_association_max_tres_minutes_per.py
--rw-r--r--   0 runner    (1001) docker     (127)     3570 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_association_max_tres_per.py
--rw-r--r--   0 runner    (1001) docker     (127)     2599 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_association_min.py
--rw-r--r--   0 runner    (1001) docker     (127)     2995 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_association_short_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     4352 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_association_usage.py
--rw-r--r--   0 runner    (1001) docker     (127)     3679 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_associations_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     4755 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_cluster_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2858 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_cluster_info_associations.py
--rw-r--r--   0 runner    (1001) docker     (127)     2701 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_cluster_info_controller.py
--rw-r--r--   0 runner    (1001) docker     (127)     6817 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_config_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2995 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_config_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2795 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_coordinator_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     3407 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_diag.py
--rw-r--r--   0 runner    (1001) docker     (127)     4483 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_diag_statistics.py
--rw-r--r--   0 runner    (1001) docker     (127)     3391 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_diag_statistics_rollups_inner.py
--rw-r--r--   0 runner    (1001) docker     (127)     3157 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_diag_statistics_rpcs_inner.py
--rw-r--r--   0 runner    (1001) docker     (127)     2772 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_diag_statistics_rpcs_inner_time.py
--rw-r--r--   0 runner    (1001) docker     (127)     3170 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_diag_statistics_users_inner.py
--rw-r--r--   0 runner    (1001) docker     (127)     2775 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_diag_statistics_users_inner_time.py
--rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_error.py
--rw-r--r--   0 runner    (1001) docker     (127)    10498 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     3230 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_job_array.py
--rw-r--r--   0 runner    (1001) docker     (127)     2805 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_job_array_limits.py
--rw-r--r--   0 runner    (1001) docker     (127)     2879 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_job_array_limits_max.py
--rw-r--r--   0 runner    (1001) docker     (127)     2609 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_job_array_limits_max_running.py
--rw-r--r--   0 runner    (1001) docker     (127)     2837 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_job_comment.py
--rw-r--r--   0 runner    (1001) docker     (127)     3154 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_job_exit_code.py
--rw-r--r--   0 runner    (1001) docker     (127)     2743 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_job_exit_code_signal.py
--rw-r--r--   0 runner    (1001) docker     (127)     2709 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_job_het.py
--rw-r--r--   0 runner    (1001) docker     (127)     3531 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_job_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_job_mcs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2709 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_job_required.py
--rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_job_reservation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2693 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_job_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     6490 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_job_step.py
--rw-r--r--   0 runner    (1001) docker     (127)     3137 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_job_step_cpu.py
--rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_job_step_cpu_requested_frequency.py
--rw-r--r--   0 runner    (1001) docker     (127)     2689 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_job_step_nodes.py
--rw-r--r--   0 runner    (1001) docker     (127)     3313 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_job_step_statistics.py
--rw-r--r--   0 runner    (1001) docker     (127)     2627 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_job_step_statistics_cpu.py
--rw-r--r--   0 runner    (1001) docker     (127)     2599 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_job_step_statistics_energy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3169 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_job_step_step.py
--rw-r--r--   0 runner    (1001) docker     (127)     2580 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_job_step_step_het.py
--rw-r--r--   0 runner    (1001) docker     (127)     2569 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_job_step_task.py
--rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_job_step_tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     4196 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_job_step_time.py
--rw-r--r--   0 runner    (1001) docker     (127)     3881 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_job_step_tres.py
--rw-r--r--   0 runner    (1001) docker     (127)     4667 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_job_step_tres_requested.py
--rw-r--r--   0 runner    (1001) docker     (127)     4649 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_job_time.py
--rw-r--r--   0 runner    (1001) docker     (127)     2886 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_job_time_system.py
--rw-r--r--   0 runner    (1001) docker     (127)     2793 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_job_time_total.py
--rw-r--r--   0 runner    (1001) docker     (127)     2819 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_job_time_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     3619 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_job_tres.py
--rw-r--r--   0 runner    (1001) docker     (127)     2673 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_job_wckey.py
--rw-r--r--   0 runner    (1001) docker     (127)     4144 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_qos.py
--rw-r--r--   0 runner    (1001) docker     (127)     3521 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_qos_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     3382 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_qos_limits.py
--rw-r--r--   0 runner    (1001) docker     (127)     4153 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_qos_limits_max.py
--rw-r--r--   0 runner    (1001) docker     (127)     2851 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_qos_limits_max_accruing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2757 2024-03-24 21:15:58.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_qos_limits_max_accruing_per.py
--rw-r--r--   0 runner    (1001) docker     (127)     2920 2024-03-24 21:15:58.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_qos_limits_max_jobs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2898 2024-03-24 21:15:58.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_qos_limits_max_jobs_active_jobs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2750 2024-03-24 21:15:58.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_qos_limits_max_jobs_active_jobs_per.py
--rw-r--r--   0 runner    (1001) docker     (127)     3274 2024-03-24 21:15:58.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_qos_limits_max_tres.py
--rw-r--r--   0 runner    (1001) docker     (127)     2871 2024-03-24 21:15:58.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_qos_limits_max_tres_minutes.py
--rw-r--r--   0 runner    (1001) docker     (127)     4156 2024-03-24 21:15:58.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_qos_limits_max_tres_minutes_per.py
--rw-r--r--   0 runner    (1001) docker     (127)     4663 2024-03-24 21:15:58.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_qos_limits_max_tres_per.py
--rw-r--r--   0 runner    (1001) docker     (127)     2859 2024-03-24 21:15:58.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_qos_limits_max_wall_clock.py
--rw-r--r--   0 runner    (1001) docker     (127)     2717 2024-03-24 21:15:58.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_qos_limits_max_wall_clock_per.py
--rw-r--r--   0 runner    (1001) docker     (127)     3007 2024-03-24 21:15:58.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_qos_limits_min.py
--rw-r--r--   0 runner    (1001) docker     (127)     2813 2024-03-24 21:15:58.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_qos_limits_min_tres.py
--rw-r--r--   0 runner    (1001) docker     (127)     3028 2024-03-24 21:15:58.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_qos_limits_min_tres_per.py
--rw-r--r--   0 runner    (1001) docker     (127)     2882 2024-03-24 21:15:58.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_qos_preempt.py
--rw-r--r--   0 runner    (1001) docker     (127)     3023 2024-03-24 21:15:58.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_response_account_delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     3039 2024-03-24 21:15:58.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_response_association_delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     3019 2024-03-24 21:15:58.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_response_associations.py
--rw-r--r--   0 runner    (1001) docker     (127)     3011 2024-03-24 21:15:58.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_response_cluster_add.py
--rw-r--r--   0 runner    (1001) docker     (127)     3023 2024-03-24 21:15:58.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_response_cluster_delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     3007 2024-03-24 21:15:58.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_response_qos_delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     2987 2024-03-24 21:15:58.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_response_tres.py
--rw-r--r--   0 runner    (1001) docker     (127)     3011 2024-03-24 21:15:58.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_response_user_delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     3011 2024-03-24 21:15:58.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_response_user_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     3003 2024-03-24 21:15:58.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_response_wckey_add.py
--rw-r--r--   0 runner    (1001) docker     (127)     3015 2024-03-24 21:15:58.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_response_wckey_delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     3789 2024-03-24 21:15:58.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_tres_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2925 2024-03-24 21:15:58.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_tres_list_inner.py
--rw-r--r--   0 runner    (1001) docker     (127)     4303 2024-03-24 21:15:58.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     2828 2024-03-24 21:15:58.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_user_associations.py
--rw-r--r--   0 runner    (1001) docker     (127)     2678 2024-03-24 21:15:58.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_user_default.py
--rw-r--r--   0 runner    (1001) docker     (127)     3549 2024-03-24 21:15:58.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_user_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     3214 2024-03-24 21:15:58.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_wckey.py
--rw-r--r--   0 runner    (1001) docker     (127)     3566 2024-03-24 21:15:58.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_wckey_info.py
--rw-r--r--   0 runner    (1001) docker     (127)    18713 2024-03-24 21:15:58.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/job_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)     5470 2024-03-24 21:15:58.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/job_properties_exclusive.py
--rw-r--r--   0 runner    (1001) docker     (127)     5579 2024-03-24 21:15:58.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/job_properties_nodes.py
--rw-r--r--   0 runner    (1001) docker     (127)     5229 2024-03-24 21:15:58.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/signal.py
--rw-r--r--   0 runner    (1001) docker     (127)     3383 2024-03-24 21:15:58.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/v0036_diag.py
--rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-03-24 21:15:58.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/v0036_error.py
--rw-r--r--   0 runner    (1001) docker     (127)    18677 2024-03-24 21:15:58.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/v0036_job_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)     3098 2024-03-24 21:15:58.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/v0036_job_resources.py
--rw-r--r--   0 runner    (1001) docker     (127)    21473 2024-03-24 21:15:58.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/v0036_job_response_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)     3465 2024-03-24 21:15:58.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/v0036_job_submission.py
--rw-r--r--   0 runner    (1001) docker     (127)     3511 2024-03-24 21:15:58.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/v0036_job_submission_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3604 2024-03-24 21:15:58.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/v0036_jobs_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     7945 2024-03-24 21:15:58.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/v0036_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     3541 2024-03-24 21:15:58.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/v0036_nodes_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     7502 2024-03-24 21:15:58.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/v0036_partition.py
--rw-r--r--   0 runner    (1001) docker     (127)     3630 2024-03-24 21:15:58.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/v0036_partitions_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3261 2024-03-24 21:15:58.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/v0036_ping.py
--rw-r--r--   0 runner    (1001) docker     (127)     3521 2024-03-24 21:15:58.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/v0036_pings.py
--rw-r--r--   0 runner    (1001) docker     (127)      937 2024-03-24 21:15:58.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/v0036_signal.py
--rw-r--r--   0 runner    (1001) docker     (127)     3383 2024-03-24 21:15:58.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/v0037_diag.py
--rw-r--r--   0 runner    (1001) docker     (127)     9695 2024-03-24 21:15:58.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/v0037_diag_statistics.py
--rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-03-24 21:15:58.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/v0037_error.py
--rw-r--r--   0 runner    (1001) docker     (127)    18701 2024-03-24 21:15:58.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/v0037_job_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)     3623 2024-03-24 21:15:58.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/v0037_job_resources.py
--rw-r--r--   0 runner    (1001) docker     (127)    21433 2024-03-24 21:15:58.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/v0037_job_response_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)     3465 2024-03-24 21:15:58.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/v0037_job_submission.py
--rw-r--r--   0 runner    (1001) docker     (127)     3511 2024-03-24 21:15:58.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/v0037_job_submission_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3604 2024-03-24 21:15:58.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/v0037_jobs_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     9234 2024-03-24 21:15:58.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/v0037_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     3042 2024-03-24 21:15:58.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/v0037_node_allocation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3541 2024-03-24 21:15:58.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/v0037_nodes_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     7466 2024-03-24 21:15:58.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/v0037_partition.py
--rw-r--r--   0 runner    (1001) docker     (127)     3630 2024-03-24 21:15:58.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/v0037_partitions_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3261 2024-03-24 21:15:58.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/v0037_ping.py
--rw-r--r--   0 runner    (1001) docker     (127)     3521 2024-03-24 21:15:58.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/v0037_pings.py
--rw-r--r--   0 runner    (1001) docker     (127)     5799 2024-03-24 21:15:58.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/v0037_reservation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2702 2024-03-24 21:15:58.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/v0037_reservation_purge_completed.py
--rw-r--r--   0 runner    (1001) docker     (127)     3666 2024-03-24 21:15:58.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/v0037_reservations_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      937 2024-03-24 21:15:58.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/models/v0037_signal.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 21:15:58.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     9374 2024-03-24 21:15:58.000000 aind-slurm-rest-0.0.1/aind_slurm_rest/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 21:16:07.931152 aind-slurm-rest-0.0.1/aind_slurm_rest.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-03-24 21:16:07.000000 aind-slurm-rest-0.0.1/aind_slurm_rest.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    18236 2024-03-24 21:16:07.000000 aind-slurm-rest-0.0.1/aind_slurm_rest.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-24 21:16:07.000000 aind-slurm-rest-0.0.1/aind_slurm_rest.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-03-24 21:16:07.000000 aind-slurm-rest-0.0.1/aind_slurm_rest.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-03-24 21:16:07.000000 aind-slurm-rest-0.0.1/aind_slurm_rest.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-03-24 21:15:58.000000 aind-slurm-rest-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-03-24 21:16:07.931152 aind-slurm-rest-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-03-24 21:15:58.000000 aind-slurm-rest-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 21:16:07.931152 aind-slurm-rest-0.0.1/test/
--rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/test/test_dbv0036_account.py
--rw-r--r--   0 runner    (1001) docker     (127)     2570 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/test/test_dbv0036_account_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/test/test_dbv0036_account_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3867 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/test/test_dbv0036_association.py
--rw-r--r--   0 runner    (1001) docker     (127)     3086 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/test/test_dbv0036_association_max.py
--rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/test/test_dbv0036_association_max_jobs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3423 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/test/test_dbv0036_association_max_tres.py
--rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/test/test_dbv0036_association_max_tres_minutes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/test/test_dbv0036_association_max_tres_minutes_per.py
--rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/test/test_dbv0036_association_max_tres_per.py
--rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/test/test_dbv0036_association_short_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     4639 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/test/test_dbv0036_associations_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2538 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/test/test_dbv0036_cluster_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/test/test_dbv0036_cluster_info_associations.py
--rw-r--r--   0 runner    (1001) docker     (127)     9618 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/test/test_dbv0036_config_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     1604 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/test/test_dbv0036_config_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/test/test_dbv0036_coordinator_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2872 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/test/test_dbv0036_diag.py
--rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/test/test_dbv0036_error.py
--rw-r--r--   0 runner    (1001) docker     (127)    10757 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/test/test_dbv0036_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/test/test_dbv0036_job_exit_code.py
--rw-r--r--   0 runner    (1001) docker     (127)     9529 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/test/test_dbv0036_job_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/test/test_dbv0036_job_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     5365 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/test/test_dbv0036_job_step.py
--rw-r--r--   0 runner    (1001) docker     (127)     3296 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/test/test_dbv0036_job_step_tres.py
--rw-r--r--   0 runner    (1001) docker     (127)     2631 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/test/test_dbv0036_job_step_tres_requested.py
--rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/test/test_dbv0036_job_tres.py
--rw-r--r--   0 runner    (1001) docker     (127)     3033 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/test/test_dbv0036_qos.py
--rw-r--r--   0 runner    (1001) docker     (127)     3635 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/test/test_dbv0036_qos_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     3034 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/test/test_dbv0036_qos_limits.py
--rw-r--r--   0 runner    (1001) docker     (127)     3768 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/test/test_dbv0036_qos_limits_max.py
--rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/test/test_dbv0036_qos_limits_max_jobs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/test/test_dbv0036_qos_limits_max_jobs_per.py
--rw-r--r--   0 runner    (1001) docker     (127)     3232 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/test/test_dbv0036_qos_limits_max_tres.py
--rw-r--r--   0 runner    (1001) docker     (127)     2312 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/test/test_dbv0036_qos_limits_max_tres_minutes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/test/test_dbv0036_qos_limits_max_tres_minutes_per.py
--rw-r--r--   0 runner    (1001) docker     (127)     2620 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/test/test_dbv0036_qos_limits_max_tres_per.py
--rw-r--r--   0 runner    (1001) docker     (127)     1995 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/test/test_dbv0036_qos_limits_min.py
--rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/test/test_dbv0036_qos_limits_min_tres.py
--rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/test/test_dbv0036_qos_limits_min_tres_per.py
--rw-r--r--   0 runner    (1001) docker     (127)     1689 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/test/test_dbv0036_response_account_delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/test/test_dbv0036_response_association_delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/test/test_dbv0036_response_cluster_add.py
--rw-r--r--   0 runner    (1001) docker     (127)     1689 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/test/test_dbv0036_response_cluster_delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/test/test_dbv0036_response_qos_delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     1580 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/test/test_dbv0036_response_tres.py
--rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/test/test_dbv0036_response_user_delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/test/test_dbv0036_response_user_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/test/test_dbv0036_response_wckey_add.py
--rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/test/test_dbv0036_response_wckey_delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/test/test_dbv0036_tres_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2134 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/test/test_dbv0036_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/test/test_dbv0036_user_associations.py
--rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/test/test_dbv0036_user_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/test/test_dbv0036_wckey.py
--rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/test/test_dbv0036_wckey_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/test/test_dbv0037_account.py
--rw-r--r--   0 runner    (1001) docker     (127)     2570 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/test/test_dbv0037_account_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/test/test_dbv0037_account_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     4588 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/test/test_dbv0037_association.py
--rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/test/test_dbv0037_association_default.py
--rw-r--r--   0 runner    (1001) docker     (127)     3391 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/test/test_dbv0037_association_max.py
--rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/test/test_dbv0037_association_max_jobs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/test/test_dbv0037_association_max_jobs_per.py
--rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/test/test_dbv0037_association_max_per.py
--rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/test/test_dbv0037_association_max_per_account.py
--rw-r--r--   0 runner    (1001) docker     (127)     4186 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/test/test_dbv0037_association_max_tres.py
--rw-r--r--   0 runner    (1001) docker     (127)     2094 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/test/test_dbv0037_association_max_tres_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/test/test_dbv0037_association_max_tres_minutes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/test/test_dbv0037_association_max_tres_minutes_per.py
--rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/test/test_dbv0037_association_max_tres_per.py
--rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/test/test_dbv0037_association_min.py
--rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/test/test_dbv0037_association_short_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/test/test_dbv0037_association_usage.py
--rw-r--r--   0 runner    (1001) docker     (127)     5465 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/test/test_dbv0037_associations_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2538 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/test/test_dbv0037_cluster_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/test/test_dbv0037_cluster_info_associations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/test/test_dbv0037_cluster_info_controller.py
--rw-r--r--   0 runner    (1001) docker     (127)    10650 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/test/test_dbv0037_config_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     1604 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/test/test_dbv0037_config_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/test/test_dbv0037_coordinator_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2847 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/test/test_dbv0037_diag.py
--rw-r--r--   0 runner    (1001) docker     (127)     2792 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/test/test_dbv0037_diag_statistics.py
--rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/test/test_dbv0037_diag_statistics_rollups_inner.py
--rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/test/test_dbv0037_diag_statistics_rpcs_inner.py
--rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/test/test_dbv0037_diag_statistics_rpcs_inner_time.py
--rw-r--r--   0 runner    (1001) docker     (127)     1783 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/test/test_dbv0037_diag_statistics_users_inner.py
--rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/test/test_dbv0037_diag_statistics_users_inner_time.py
--rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/test/test_dbv0037_error.py
--rw-r--r--   0 runner    (1001) docker     (127)    10755 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/test/test_dbv0037_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/test/test_dbv0037_job_array.py
--rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/test/test_dbv0037_job_array_limits.py
--rw-r--r--   0 runner    (1001) docker     (127)     1604 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/test/test_dbv0037_job_array_limits_max.py
--rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/test/test_dbv0037_job_array_limits_max_running.py
--rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/test/test_dbv0037_job_comment.py
--rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/test/test_dbv0037_job_exit_code.py
--rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/test/test_dbv0037_job_exit_code_signal.py
--rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/test/test_dbv0037_job_het.py
--rw-r--r--   0 runner    (1001) docker     (127)     9527 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/test/test_dbv0037_job_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/test/test_dbv0037_job_mcs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/test/test_dbv0037_job_required.py
--rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/test/test_dbv0037_job_reservation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/test/test_dbv0037_job_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     5365 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/test/test_dbv0037_job_step.py
--rw-r--r--   0 runner    (1001) docker     (127)     1643 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/test/test_dbv0037_job_step_cpu.py
--rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/test/test_dbv0037_job_step_cpu_requested_frequency.py
--rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/test/test_dbv0037_job_step_nodes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/test/test_dbv0037_job_step_statistics.py
--rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/test/test_dbv0037_job_step_statistics_cpu.py
--rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/test/test_dbv0037_job_step_statistics_energy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/test/test_dbv0037_job_step_step.py
--rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/test/test_dbv0037_job_step_step_het.py
--rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/test/test_dbv0037_job_step_task.py
--rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/test/test_dbv0037_job_step_tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2009 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/test/test_dbv0037_job_step_time.py
--rw-r--r--   0 runner    (1001) docker     (127)     3296 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/test/test_dbv0037_job_step_tres.py
--rw-r--r--   0 runner    (1001) docker     (127)     2631 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/test/test_dbv0037_job_step_tres_requested.py
--rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/test/test_dbv0037_job_time.py
--rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/test/test_dbv0037_job_time_system.py
--rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/test/test_dbv0037_job_time_total.py
--rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/test/test_dbv0037_job_time_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/test/test_dbv0037_job_tres.py
--rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/test/test_dbv0037_job_wckey.py
--rw-r--r--   0 runner    (1001) docker     (127)     3223 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/test/test_dbv0037_qos.py
--rw-r--r--   0 runner    (1001) docker     (127)     3841 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/test/test_dbv0037_qos_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     3215 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/test/test_dbv0037_qos_limits.py
--rw-r--r--   0 runner    (1001) docker     (127)     3949 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/test/test_dbv0037_qos_limits_max.py
--rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-03-24 21:15:57.000000 aind-slurm-rest-0.0.1/test/test_dbv0037_qos_limits_max_accruing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-03-24 21:15:58.000000 aind-slurm-rest-0.0.1/test/test_dbv0037_qos_limits_max_accruing_per.py
--rw-r--r--   0 runner    (1001) docker     (127)     1789 2024-03-24 21:15:58.000000 aind-slurm-rest-0.0.1/test/test_dbv0037_qos_limits_max_jobs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-03-24 21:15:58.000000 aind-slurm-rest-0.0.1/test/test_dbv0037_qos_limits_max_jobs_active_jobs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-03-24 21:15:58.000000 aind-slurm-rest-0.0.1/test/test_dbv0037_qos_limits_max_jobs_active_jobs_per.py
--rw-r--r--   0 runner    (1001) docker     (127)     3232 2024-03-24 21:15:58.000000 aind-slurm-rest-0.0.1/test/test_dbv0037_qos_limits_max_tres.py
--rw-r--r--   0 runner    (1001) docker     (127)     2312 2024-03-24 21:15:58.000000 aind-slurm-rest-0.0.1/test/test_dbv0037_qos_limits_max_tres_minutes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-03-24 21:15:58.000000 aind-slurm-rest-0.0.1/test/test_dbv0037_qos_limits_max_tres_minutes_per.py
--rw-r--r--   0 runner    (1001) docker     (127)     2620 2024-03-24 21:15:58.000000 aind-slurm-rest-0.0.1/test/test_dbv0037_qos_limits_max_tres_per.py
--rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-03-24 21:15:58.000000 aind-slurm-rest-0.0.1/test/test_dbv0037_qos_limits_max_wall_clock.py
--rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-03-24 21:15:58.000000 aind-slurm-rest-0.0.1/test/test_dbv0037_qos_limits_max_wall_clock_per.py
--rw-r--r--   0 runner    (1001) docker     (127)     1995 2024-03-24 21:15:58.000000 aind-slurm-rest-0.0.1/test/test_dbv0037_qos_limits_min.py
--rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-03-24 21:15:58.000000 aind-slurm-rest-0.0.1/test/test_dbv0037_qos_limits_min_tres.py
--rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-03-24 21:15:58.000000 aind-slurm-rest-0.0.1/test/test_dbv0037_qos_limits_min_tres_per.py
--rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-03-24 21:15:58.000000 aind-slurm-rest-0.0.1/test/test_dbv0037_qos_preempt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1689 2024-03-24 21:15:58.000000 aind-slurm-rest-0.0.1/test/test_dbv0037_response_account_delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-03-24 21:15:58.000000 aind-slurm-rest-0.0.1/test/test_dbv0037_response_association_delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-03-24 21:15:58.000000 aind-slurm-rest-0.0.1/test/test_dbv0037_response_associations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-03-24 21:15:58.000000 aind-slurm-rest-0.0.1/test/test_dbv0037_response_cluster_add.py
--rw-r--r--   0 runner    (1001) docker     (127)     1689 2024-03-24 21:15:58.000000 aind-slurm-rest-0.0.1/test/test_dbv0037_response_cluster_delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-03-24 21:15:58.000000 aind-slurm-rest-0.0.1/test/test_dbv0037_response_qos_delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     1580 2024-03-24 21:15:58.000000 aind-slurm-rest-0.0.1/test/test_dbv0037_response_tres.py
--rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-03-24 21:15:58.000000 aind-slurm-rest-0.0.1/test/test_dbv0037_response_user_delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-03-24 21:15:58.000000 aind-slurm-rest-0.0.1/test/test_dbv0037_response_user_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-03-24 21:15:58.000000 aind-slurm-rest-0.0.1/test/test_dbv0037_response_wckey_add.py
--rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-03-24 21:15:58.000000 aind-slurm-rest-0.0.1/test/test_dbv0037_response_wckey_delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-03-24 21:15:58.000000 aind-slurm-rest-0.0.1/test/test_dbv0037_tres_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-03-24 21:15:58.000000 aind-slurm-rest-0.0.1/test/test_dbv0037_tres_list_inner.py
--rw-r--r--   0 runner    (1001) docker     (127)     2134 2024-03-24 21:15:58.000000 aind-slurm-rest-0.0.1/test/test_dbv0037_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-03-24 21:15:58.000000 aind-slurm-rest-0.0.1/test/test_dbv0037_user_associations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-03-24 21:15:58.000000 aind-slurm-rest-0.0.1/test/test_dbv0037_user_default.py
--rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-03-24 21:15:58.000000 aind-slurm-rest-0.0.1/test/test_dbv0037_user_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-03-24 21:15:58.000000 aind-slurm-rest-0.0.1/test/test_dbv0037_wckey.py
--rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-03-24 21:15:58.000000 aind-slurm-rest-0.0.1/test/test_dbv0037_wckey_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-03-24 21:15:58.000000 aind-slurm-rest-0.0.1/test/test_default_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3854 2024-03-24 21:15:58.000000 aind-slurm-rest-0.0.1/test/test_job_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-03-24 21:15:58.000000 aind-slurm-rest-0.0.1/test/test_job_properties_exclusive.py
--rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-03-24 21:15:58.000000 aind-slurm-rest-0.0.1/test/test_job_properties_nodes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-03-24 21:15:58.000000 aind-slurm-rest-0.0.1/test/test_signal.py
--rw-r--r--   0 runner    (1001) docker     (127)    12922 2024-03-24 21:15:58.000000 aind-slurm-rest-0.0.1/test/test_slurm_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3271 2024-03-24 21:15:58.000000 aind-slurm-rest-0.0.1/test/test_v0036_diag.py
--rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-03-24 21:15:58.000000 aind-slurm-rest-0.0.1/test/test_v0036_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     4079 2024-03-24 21:15:58.000000 aind-slurm-rest-0.0.1/test/test_v0036_job_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-03-24 21:15:58.000000 aind-slurm-rest-0.0.1/test/test_v0036_job_resources.py
--rw-r--r--   0 runner    (1001) docker     (127)     5681 2024-03-24 21:15:58.000000 aind-slurm-rest-0.0.1/test/test_v0036_job_response_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)     7964 2024-03-24 21:15:58.000000 aind-slurm-rest-0.0.1/test/test_v0036_job_submission.py
--rw-r--r--   0 runner    (1001) docker     (127)     1762 2024-03-24 21:15:58.000000 aind-slurm-rest-0.0.1/test/test_v0036_job_submission_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     6985 2024-03-24 21:15:58.000000 aind-slurm-rest-0.0.1/test/test_v0036_jobs_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2413 2024-03-24 21:15:58.000000 aind-slurm-rest-0.0.1/test/test_v0036_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     3154 2024-03-24 21:15:58.000000 aind-slurm-rest-0.0.1/test/test_v0036_nodes_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2395 2024-03-24 21:15:58.000000 aind-slurm-rest-0.0.1/test/test_v0036_partition.py
--rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-03-24 21:15:58.000000 aind-slurm-rest-0.0.1/test/test_v0036_partitions_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-03-24 21:15:58.000000 aind-slurm-rest-0.0.1/test/test_v0036_ping.py
--rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-03-24 21:15:58.000000 aind-slurm-rest-0.0.1/test/test_v0036_pings.py
--rw-r--r--   0 runner    (1001) docker     (127)      656 2024-03-24 21:15:58.000000 aind-slurm-rest-0.0.1/test/test_v0036_signal.py
--rw-r--r--   0 runner    (1001) docker     (127)     3271 2024-03-24 21:15:58.000000 aind-slurm-rest-0.0.1/test/test_v0037_diag.py
--rw-r--r--   0 runner    (1001) docker     (127)     2897 2024-03-24 21:15:58.000000 aind-slurm-rest-0.0.1/test/test_v0037_diag_statistics.py
--rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-03-24 21:15:58.000000 aind-slurm-rest-0.0.1/test/test_v0037_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     4085 2024-03-24 21:15:58.000000 aind-slurm-rest-0.0.1/test/test_v0037_job_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-03-24 21:15:58.000000 aind-slurm-rest-0.0.1/test/test_v0037_job_resources.py
--rw-r--r--   0 runner    (1001) docker     (127)     6016 2024-03-24 21:15:58.000000 aind-slurm-rest-0.0.1/test/test_v0037_job_response_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)     7976 2024-03-24 21:15:58.000000 aind-slurm-rest-0.0.1/test/test_v0037_job_submission.py
--rw-r--r--   0 runner    (1001) docker     (127)     1762 2024-03-24 21:15:58.000000 aind-slurm-rest-0.0.1/test/test_v0037_job_submission_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     7368 2024-03-24 21:15:58.000000 aind-slurm-rest-0.0.1/test/test_v0037_jobs_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2805 2024-03-24 21:15:58.000000 aind-slurm-rest-0.0.1/test/test_v0037_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-03-24 21:15:58.000000 aind-slurm-rest-0.0.1/test/test_v0037_node_allocation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3657 2024-03-24 21:15:58.000000 aind-slurm-rest-0.0.1/test/test_v0037_nodes_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2432 2024-03-24 21:15:58.000000 aind-slurm-rest-0.0.1/test/test_v0037_partition.py
--rw-r--r--   0 runner    (1001) docker     (127)     3157 2024-03-24 21:15:58.000000 aind-slurm-rest-0.0.1/test/test_v0037_partitions_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-03-24 21:15:58.000000 aind-slurm-rest-0.0.1/test/test_v0037_ping.py
--rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-03-24 21:15:58.000000 aind-slurm-rest-0.0.1/test/test_v0037_pings.py
--rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-03-24 21:15:58.000000 aind-slurm-rest-0.0.1/test/test_v0037_reservation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-03-24 21:15:58.000000 aind-slurm-rest-0.0.1/test/test_v0037_reservation_purge_completed.py
--rw-r--r--   0 runner    (1001) docker     (127)     2755 2024-03-24 21:15:58.000000 aind-slurm-rest-0.0.1/test/test_v0037_reservations_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      656 2024-03-24 21:15:58.000000 aind-slurm-rest-0.0.1/test/test_v0037_signal.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 21:45:51.749913 aind-slurm-rest-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-07 21:45:33.000000 aind-slurm-rest-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-07 21:45:51.749913 aind-slurm-rest-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    28528 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 21:45:51.677913 aind-slurm-rest-0.1.0/aind_slurm_rest/
+-rw-r--r--   0 runner    (1001) docker     (127)    17330 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 21:45:51.677913 aind-slurm-rest-0.1.0/aind_slurm_rest/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   144779 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/api/default_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)   861002 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/api/slurm_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26248 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/api_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15600 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5937 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 21:45:51.709913 aind-slurm-rest-0.1.0/aind_slurm_rest/models/
+-rw-r--r--   0 runner    (1001) docker     (127)    16671 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4437 2024-04-07 21:45:40.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0036_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3602 2024-04-07 21:45:40.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0036_account_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2999 2024-04-07 21:45:40.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0036_account_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5372 2024-04-07 21:45:40.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0036_association.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3622 2024-04-07 21:45:40.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0036_association_max.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2826 2024-04-07 21:45:40.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0036_association_max_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3929 2024-04-07 21:45:40.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0036_association_max_tres.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3516 2024-04-07 21:45:40.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0036_association_max_tres_minutes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3063 2024-04-07 21:45:40.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0036_association_max_tres_minutes_per.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3570 2024-04-07 21:45:40.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0036_association_max_tres_per.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2995 2024-04-07 21:45:40.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0036_association_short_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3679 2024-04-07 21:45:40.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0036_associations_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4755 2024-04-07 21:45:40.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0036_cluster_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2858 2024-04-07 21:45:40.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0036_cluster_info_associations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6817 2024-04-07 21:45:40.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0036_config_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2995 2024-04-07 21:45:40.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0036_config_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2795 2024-04-07 21:45:40.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0036_coordinator_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5021 2024-04-07 21:45:40.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0036_diag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-04-07 21:45:40.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0036_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10498 2024-04-07 21:45:40.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0036_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3154 2024-04-07 21:45:40.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0036_job_exit_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2715 2024-04-07 21:45:40.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0036_job_het.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3531 2024-04-07 21:45:40.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0036_job_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2701 2024-04-07 21:45:40.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0036_job_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6490 2024-04-07 21:45:40.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0036_job_step.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3881 2024-04-07 21:45:40.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0036_job_step_tres.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4667 2024-04-07 21:45:40.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0036_job_step_tres_requested.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3619 2024-04-07 21:45:40.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0036_job_tres.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4144 2024-04-07 21:45:40.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0036_qos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3521 2024-04-07 21:45:40.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0036_qos_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3142 2024-04-07 21:45:40.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0036_qos_limits.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4153 2024-04-07 21:45:40.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0036_qos_limits_max.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2819 2024-04-07 21:45:40.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0036_qos_limits_max_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-04-07 21:45:40.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0036_qos_limits_max_jobs_per.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3274 2024-04-07 21:45:40.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0036_qos_limits_max_tres.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2871 2024-04-07 21:45:40.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0036_qos_limits_max_tres_minutes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4156 2024-04-07 21:45:40.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0036_qos_limits_max_tres_minutes_per.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4663 2024-04-07 21:45:40.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0036_qos_limits_max_tres_per.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3007 2024-04-07 21:45:40.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0036_qos_limits_min.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2813 2024-04-07 21:45:40.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0036_qos_limits_min_tres.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3028 2024-04-07 21:45:40.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0036_qos_limits_min_tres_per.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3023 2024-04-07 21:45:40.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0036_response_account_delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3039 2024-04-07 21:45:40.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0036_response_association_delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3011 2024-04-07 21:45:40.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0036_response_cluster_add.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3023 2024-04-07 21:45:40.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0036_response_cluster_delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3007 2024-04-07 21:45:40.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0036_response_qos_delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2987 2024-04-07 21:45:40.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0036_response_tres.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3011 2024-04-07 21:45:40.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0036_response_user_delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3011 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0036_response_user_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3003 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0036_response_wckey_add.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3015 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0036_response_wckey_delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3789 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0036_tres_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4303 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0036_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2828 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0036_user_associations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3549 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0036_user_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3214 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0036_wckey.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3566 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0036_wckey_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4437 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3602 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_account_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2999 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_account_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5531 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_association.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_association_default.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3622 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_association_max.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3307 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_association_max_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2596 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_association_max_jobs_per.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2870 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_association_max_per.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2615 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_association_max_per_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4374 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_association_max_tres.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3627 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_association_max_tres_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3516 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_association_max_tres_minutes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3063 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_association_max_tres_minutes_per.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3570 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_association_max_tres_per.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2599 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_association_min.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2995 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_association_short_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4352 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_association_usage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3679 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_associations_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4755 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_cluster_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2858 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_cluster_info_associations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2701 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_cluster_info_controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6817 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_config_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2995 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_config_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2795 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_coordinator_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3407 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_diag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4483 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_diag_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3391 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_diag_statistics_rollups_inner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3157 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_diag_statistics_rpcs_inner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2772 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_diag_statistics_rpcs_inner_time.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3170 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_diag_statistics_users_inner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2775 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_diag_statistics_users_inner_time.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10498 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3230 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_job_array.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2805 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_job_array_limits.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2879 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_job_array_limits_max.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2609 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_job_array_limits_max_running.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2837 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_job_comment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3154 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_job_exit_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2743 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_job_exit_code_signal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2709 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_job_het.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3531 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_job_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_job_mcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2709 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_job_required.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_job_reservation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2693 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_job_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6490 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_job_step.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3137 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_job_step_cpu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_job_step_cpu_requested_frequency.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2689 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_job_step_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3313 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_job_step_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2627 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_job_step_statistics_cpu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2599 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_job_step_statistics_energy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3169 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_job_step_step.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2580 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_job_step_step_het.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2569 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_job_step_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_job_step_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4196 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_job_step_time.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3881 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_job_step_tres.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4667 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_job_step_tres_requested.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4649 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_job_time.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2886 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_job_time_system.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2793 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_job_time_total.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2819 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_job_time_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3619 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_job_tres.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2673 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_job_wckey.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4144 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_qos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3521 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_qos_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3382 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_qos_limits.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4153 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_qos_limits_max.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2851 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_qos_limits_max_accruing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2757 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_qos_limits_max_accruing_per.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2920 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_qos_limits_max_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2898 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_qos_limits_max_jobs_active_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2750 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_qos_limits_max_jobs_active_jobs_per.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3274 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_qos_limits_max_tres.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2871 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_qos_limits_max_tres_minutes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4156 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_qos_limits_max_tres_minutes_per.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4663 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_qos_limits_max_tres_per.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2859 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_qos_limits_max_wall_clock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2717 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_qos_limits_max_wall_clock_per.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3007 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_qos_limits_min.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2813 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_qos_limits_min_tres.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3028 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_qos_limits_min_tres_per.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2882 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_qos_preempt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3023 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_response_account_delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3039 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_response_association_delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3019 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_response_associations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3011 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_response_cluster_add.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3023 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_response_cluster_delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3007 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_response_qos_delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2987 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_response_tres.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3011 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_response_user_delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3011 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_response_user_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3003 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_response_wckey_add.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3015 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_response_wckey_delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3789 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_tres_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2925 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_tres_list_inner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4303 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2828 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_user_associations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2678 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_user_default.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3549 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_user_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3214 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_wckey.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3566 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_wckey_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18713 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/job_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5470 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/job_properties_exclusive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5579 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/job_properties_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5229 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/signal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3383 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/v0036_diag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/v0036_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18677 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/v0036_job_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3098 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/v0036_job_resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21473 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/v0036_job_response_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3465 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/v0036_job_submission.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3511 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/v0036_job_submission_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3604 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/v0036_jobs_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7945 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/v0036_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3541 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/v0036_nodes_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7502 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/v0036_partition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3630 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/v0036_partitions_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3261 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/v0036_ping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3521 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/v0036_pings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/v0036_signal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3383 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/v0037_diag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9695 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/v0037_diag_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/v0037_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18701 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/v0037_job_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3623 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/v0037_job_resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21433 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/v0037_job_response_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3465 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/v0037_job_submission.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3511 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/v0037_job_submission_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3604 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/v0037_jobs_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9234 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/v0037_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3042 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/v0037_node_allocation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3541 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/v0037_nodes_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7466 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/v0037_partition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3630 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/v0037_partitions_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3261 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/v0037_ping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3521 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/v0037_pings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5799 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/v0037_reservation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2702 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/v0037_reservation_purge_completed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3666 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/v0037_reservations_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/models/v0037_signal.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     9374 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/aind_slurm_rest/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 21:45:51.749913 aind-slurm-rest-0.1.0/aind_slurm_rest.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-07 21:45:51.000000 aind-slurm-rest-0.1.0/aind_slurm_rest.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    18307 2024-04-07 21:45:51.000000 aind-slurm-rest-0.1.0/aind_slurm_rest.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 21:45:51.000000 aind-slurm-rest-0.1.0/aind_slurm_rest.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-07 21:45:51.000000 aind-slurm-rest-0.1.0/aind_slurm_rest.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-07 21:45:51.000000 aind-slurm-rest-0.1.0/aind_slurm_rest.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-07 21:45:51.749913 aind-slurm-rest-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 21:45:51.749913 aind-slurm-rest-0.1.0/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-04-07 21:45:40.000000 aind-slurm-rest-0.1.0/test/test_dbv0036_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2570 2024-04-07 21:45:40.000000 aind-slurm-rest-0.1.0/test/test_dbv0036_account_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-04-07 21:45:40.000000 aind-slurm-rest-0.1.0/test/test_dbv0036_account_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3867 2024-04-07 21:45:40.000000 aind-slurm-rest-0.1.0/test/test_dbv0036_association.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3086 2024-04-07 21:45:40.000000 aind-slurm-rest-0.1.0/test/test_dbv0036_association_max.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-04-07 21:45:40.000000 aind-slurm-rest-0.1.0/test/test_dbv0036_association_max_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3423 2024-04-07 21:45:40.000000 aind-slurm-rest-0.1.0/test/test_dbv0036_association_max_tres.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-04-07 21:45:40.000000 aind-slurm-rest-0.1.0/test/test_dbv0036_association_max_tres_minutes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-04-07 21:45:40.000000 aind-slurm-rest-0.1.0/test/test_dbv0036_association_max_tres_minutes_per.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-04-07 21:45:40.000000 aind-slurm-rest-0.1.0/test/test_dbv0036_association_max_tres_per.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-04-07 21:45:40.000000 aind-slurm-rest-0.1.0/test/test_dbv0036_association_short_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4639 2024-04-07 21:45:40.000000 aind-slurm-rest-0.1.0/test/test_dbv0036_associations_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2538 2024-04-07 21:45:40.000000 aind-slurm-rest-0.1.0/test/test_dbv0036_cluster_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-04-07 21:45:40.000000 aind-slurm-rest-0.1.0/test/test_dbv0036_cluster_info_associations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9618 2024-04-07 21:45:40.000000 aind-slurm-rest-0.1.0/test/test_dbv0036_config_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1604 2024-04-07 21:45:40.000000 aind-slurm-rest-0.1.0/test/test_dbv0036_config_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-04-07 21:45:40.000000 aind-slurm-rest-0.1.0/test/test_dbv0036_coordinator_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2872 2024-04-07 21:45:40.000000 aind-slurm-rest-0.1.0/test/test_dbv0036_diag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-04-07 21:45:40.000000 aind-slurm-rest-0.1.0/test/test_dbv0036_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10721 2024-04-07 21:45:40.000000 aind-slurm-rest-0.1.0/test/test_dbv0036_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-04-07 21:45:40.000000 aind-slurm-rest-0.1.0/test/test_dbv0036_job_exit_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-04-07 21:45:40.000000 aind-slurm-rest-0.1.0/test/test_dbv0036_job_het.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9493 2024-04-07 21:45:40.000000 aind-slurm-rest-0.1.0/test/test_dbv0036_job_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-04-07 21:45:40.000000 aind-slurm-rest-0.1.0/test/test_dbv0036_job_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5365 2024-04-07 21:45:40.000000 aind-slurm-rest-0.1.0/test/test_dbv0036_job_step.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3296 2024-04-07 21:45:40.000000 aind-slurm-rest-0.1.0/test/test_dbv0036_job_step_tres.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2631 2024-04-07 21:45:40.000000 aind-slurm-rest-0.1.0/test/test_dbv0036_job_step_tres_requested.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-04-07 21:45:40.000000 aind-slurm-rest-0.1.0/test/test_dbv0036_job_tres.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3033 2024-04-07 21:45:40.000000 aind-slurm-rest-0.1.0/test/test_dbv0036_qos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3635 2024-04-07 21:45:40.000000 aind-slurm-rest-0.1.0/test/test_dbv0036_qos_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3034 2024-04-07 21:45:40.000000 aind-slurm-rest-0.1.0/test/test_dbv0036_qos_limits.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3768 2024-04-07 21:45:40.000000 aind-slurm-rest-0.1.0/test/test_dbv0036_qos_limits_max.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-04-07 21:45:40.000000 aind-slurm-rest-0.1.0/test/test_dbv0036_qos_limits_max_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-04-07 21:45:40.000000 aind-slurm-rest-0.1.0/test/test_dbv0036_qos_limits_max_jobs_per.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3232 2024-04-07 21:45:40.000000 aind-slurm-rest-0.1.0/test/test_dbv0036_qos_limits_max_tres.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2312 2024-04-07 21:45:40.000000 aind-slurm-rest-0.1.0/test/test_dbv0036_qos_limits_max_tres_minutes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-04-07 21:45:40.000000 aind-slurm-rest-0.1.0/test/test_dbv0036_qos_limits_max_tres_minutes_per.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2620 2024-04-07 21:45:40.000000 aind-slurm-rest-0.1.0/test/test_dbv0036_qos_limits_max_tres_per.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1995 2024-04-07 21:45:40.000000 aind-slurm-rest-0.1.0/test/test_dbv0036_qos_limits_min.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-04-07 21:45:40.000000 aind-slurm-rest-0.1.0/test/test_dbv0036_qos_limits_min_tres.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-04-07 21:45:40.000000 aind-slurm-rest-0.1.0/test/test_dbv0036_qos_limits_min_tres_per.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1689 2024-04-07 21:45:40.000000 aind-slurm-rest-0.1.0/test/test_dbv0036_response_account_delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-04-07 21:45:40.000000 aind-slurm-rest-0.1.0/test/test_dbv0036_response_association_delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-04-07 21:45:40.000000 aind-slurm-rest-0.1.0/test/test_dbv0036_response_cluster_add.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1689 2024-04-07 21:45:40.000000 aind-slurm-rest-0.1.0/test/test_dbv0036_response_cluster_delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-04-07 21:45:40.000000 aind-slurm-rest-0.1.0/test/test_dbv0036_response_qos_delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1580 2024-04-07 21:45:40.000000 aind-slurm-rest-0.1.0/test/test_dbv0036_response_tres.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/test/test_dbv0036_response_user_delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/test/test_dbv0036_response_user_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/test/test_dbv0036_response_wckey_add.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/test/test_dbv0036_response_wckey_delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/test/test_dbv0036_tres_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2134 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/test/test_dbv0036_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/test/test_dbv0036_user_associations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/test/test_dbv0036_user_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/test/test_dbv0036_wckey.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/test/test_dbv0036_wckey_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/test/test_dbv0037_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2570 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/test/test_dbv0037_account_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/test/test_dbv0037_account_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4588 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/test/test_dbv0037_association.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/test/test_dbv0037_association_default.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3391 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/test/test_dbv0037_association_max.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/test/test_dbv0037_association_max_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/test/test_dbv0037_association_max_jobs_per.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/test/test_dbv0037_association_max_per.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/test/test_dbv0037_association_max_per_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4186 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/test/test_dbv0037_association_max_tres.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2094 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/test/test_dbv0037_association_max_tres_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/test/test_dbv0037_association_max_tres_minutes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/test/test_dbv0037_association_max_tres_minutes_per.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/test/test_dbv0037_association_max_tres_per.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/test/test_dbv0037_association_min.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/test/test_dbv0037_association_short_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/test/test_dbv0037_association_usage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5465 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/test/test_dbv0037_associations_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2538 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/test/test_dbv0037_cluster_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/test/test_dbv0037_cluster_info_associations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/test/test_dbv0037_cluster_info_controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10650 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/test/test_dbv0037_config_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1604 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/test/test_dbv0037_config_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/test/test_dbv0037_coordinator_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2847 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/test/test_dbv0037_diag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2792 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/test/test_dbv0037_diag_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/test/test_dbv0037_diag_statistics_rollups_inner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/test/test_dbv0037_diag_statistics_rpcs_inner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/test/test_dbv0037_diag_statistics_rpcs_inner_time.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1783 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/test/test_dbv0037_diag_statistics_users_inner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/test/test_dbv0037_diag_statistics_users_inner_time.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/test/test_dbv0037_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10755 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/test/test_dbv0037_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/test/test_dbv0037_job_array.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/test/test_dbv0037_job_array_limits.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1604 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/test/test_dbv0037_job_array_limits_max.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/test/test_dbv0037_job_array_limits_max_running.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/test/test_dbv0037_job_comment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/test/test_dbv0037_job_exit_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/test/test_dbv0037_job_exit_code_signal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/test/test_dbv0037_job_het.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9527 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/test/test_dbv0037_job_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/test/test_dbv0037_job_mcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/test/test_dbv0037_job_required.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/test/test_dbv0037_job_reservation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/test/test_dbv0037_job_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5365 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/test/test_dbv0037_job_step.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1643 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/test/test_dbv0037_job_step_cpu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/test/test_dbv0037_job_step_cpu_requested_frequency.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/test/test_dbv0037_job_step_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/test/test_dbv0037_job_step_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/test/test_dbv0037_job_step_statistics_cpu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/test/test_dbv0037_job_step_statistics_energy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/test/test_dbv0037_job_step_step.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/test/test_dbv0037_job_step_step_het.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/test/test_dbv0037_job_step_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/test/test_dbv0037_job_step_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2009 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/test/test_dbv0037_job_step_time.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3296 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/test/test_dbv0037_job_step_tres.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2631 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/test/test_dbv0037_job_step_tres_requested.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/test/test_dbv0037_job_time.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/test/test_dbv0037_job_time_system.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/test/test_dbv0037_job_time_total.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/test/test_dbv0037_job_time_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/test/test_dbv0037_job_tres.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/test/test_dbv0037_job_wckey.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3223 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/test/test_dbv0037_qos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3841 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/test/test_dbv0037_qos_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3215 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/test/test_dbv0037_qos_limits.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3949 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/test/test_dbv0037_qos_limits_max.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/test/test_dbv0037_qos_limits_max_accruing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/test/test_dbv0037_qos_limits_max_accruing_per.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1789 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/test/test_dbv0037_qos_limits_max_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/test/test_dbv0037_qos_limits_max_jobs_active_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/test/test_dbv0037_qos_limits_max_jobs_active_jobs_per.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3232 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/test/test_dbv0037_qos_limits_max_tres.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2312 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/test/test_dbv0037_qos_limits_max_tres_minutes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/test/test_dbv0037_qos_limits_max_tres_minutes_per.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2620 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/test/test_dbv0037_qos_limits_max_tres_per.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/test/test_dbv0037_qos_limits_max_wall_clock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/test/test_dbv0037_qos_limits_max_wall_clock_per.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1995 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/test/test_dbv0037_qos_limits_min.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/test/test_dbv0037_qos_limits_min_tres.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/test/test_dbv0037_qos_limits_min_tres_per.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/test/test_dbv0037_qos_preempt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1689 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/test/test_dbv0037_response_account_delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/test/test_dbv0037_response_association_delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/test/test_dbv0037_response_associations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/test/test_dbv0037_response_cluster_add.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1689 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/test/test_dbv0037_response_cluster_delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/test/test_dbv0037_response_qos_delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1580 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/test/test_dbv0037_response_tres.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/test/test_dbv0037_response_user_delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/test/test_dbv0037_response_user_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/test/test_dbv0037_response_wckey_add.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/test/test_dbv0037_response_wckey_delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/test/test_dbv0037_tres_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/test/test_dbv0037_tres_list_inner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2134 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/test/test_dbv0037_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/test/test_dbv0037_user_associations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/test/test_dbv0037_user_default.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/test/test_dbv0037_user_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/test/test_dbv0037_wckey.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/test/test_dbv0037_wckey_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/test/test_default_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3854 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/test/test_job_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/test/test_job_properties_exclusive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/test/test_job_properties_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/test/test_signal.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12922 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/test/test_slurm_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3271 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/test/test_v0036_diag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/test/test_v0036_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4079 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/test/test_v0036_job_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/test/test_v0036_job_resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5681 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/test/test_v0036_job_response_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7964 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/test/test_v0036_job_submission.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1762 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/test/test_v0036_job_submission_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6985 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/test/test_v0036_jobs_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2413 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/test/test_v0036_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3154 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/test/test_v0036_nodes_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2395 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/test/test_v0036_partition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/test/test_v0036_partitions_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/test/test_v0036_ping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/test/test_v0036_pings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/test/test_v0036_signal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3271 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/test/test_v0037_diag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2897 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/test/test_v0037_diag_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/test/test_v0037_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4085 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/test/test_v0037_job_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/test/test_v0037_job_resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6016 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/test/test_v0037_job_response_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7976 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/test/test_v0037_job_submission.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1762 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/test/test_v0037_job_submission_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7368 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/test/test_v0037_jobs_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2805 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/test/test_v0037_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/test/test_v0037_node_allocation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3657 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/test/test_v0037_nodes_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2432 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/test/test_v0037_partition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3157 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/test/test_v0037_partitions_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/test/test_v0037_ping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/test/test_v0037_pings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/test/test_v0037_reservation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/test/test_v0037_reservation_purge_completed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2755 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/test/test_v0037_reservations_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-04-07 21:45:41.000000 aind-slurm-rest-0.1.0/test/test_v0037_signal.py
```

### Comparing `aind-slurm-rest-0.0.1/LICENSE` & `aind-slurm-rest-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/README.md` & `aind-slurm-rest-0.1.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # aind-slurm-rest
 API to access and control Slurm.
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 - API version: 0.0.37
-- Package version: 0.0.1
+- Package version: 0.1.0
 - Generator version: 7.5.0-SNAPSHOT
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 For more information, please visit [https://www.schedmd.com/](https://www.schedmd.com/)
 
 ## Requirements.
 
 Python 3.7+
@@ -218,14 +218,15 @@
  - [Dbv0036ConfigInfo](docs/Dbv0036ConfigInfo.md)
  - [Dbv0036ConfigResponse](docs/Dbv0036ConfigResponse.md)
  - [Dbv0036CoordinatorInfo](docs/Dbv0036CoordinatorInfo.md)
  - [Dbv0036Diag](docs/Dbv0036Diag.md)
  - [Dbv0036Error](docs/Dbv0036Error.md)
  - [Dbv0036Job](docs/Dbv0036Job.md)
  - [Dbv0036JobExitCode](docs/Dbv0036JobExitCode.md)
+ - [Dbv0036JobHet](docs/Dbv0036JobHet.md)
  - [Dbv0036JobInfo](docs/Dbv0036JobInfo.md)
  - [Dbv0036JobState](docs/Dbv0036JobState.md)
  - [Dbv0036JobStep](docs/Dbv0036JobStep.md)
  - [Dbv0036JobStepTres](docs/Dbv0036JobStepTres.md)
  - [Dbv0036JobStepTresRequested](docs/Dbv0036JobStepTresRequested.md)
  - [Dbv0036JobTres](docs/Dbv0036JobTres.md)
  - [Dbv0036Qos](docs/Dbv0036Qos.md)
```

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/__init__.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     Contact: sales@schedmd.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
-__version__ = "0.0.1"
+__version__ = "0.1.0"
 
 # import apis into sdk package
 from aind_slurm_rest.api.default_api import DefaultApi
 from aind_slurm_rest.api.slurm_api import SlurmApi
 
 # import ApiClient
 from aind_slurm_rest.api_response import ApiResponse
@@ -50,14 +50,15 @@
 from aind_slurm_rest.models.dbv0036_config_info import Dbv0036ConfigInfo
 from aind_slurm_rest.models.dbv0036_config_response import Dbv0036ConfigResponse
 from aind_slurm_rest.models.dbv0036_coordinator_info import Dbv0036CoordinatorInfo
 from aind_slurm_rest.models.dbv0036_diag import Dbv0036Diag
 from aind_slurm_rest.models.dbv0036_error import Dbv0036Error
 from aind_slurm_rest.models.dbv0036_job import Dbv0036Job
 from aind_slurm_rest.models.dbv0036_job_exit_code import Dbv0036JobExitCode
+from aind_slurm_rest.models.dbv0036_job_het import Dbv0036JobHet
 from aind_slurm_rest.models.dbv0036_job_info import Dbv0036JobInfo
 from aind_slurm_rest.models.dbv0036_job_state import Dbv0036JobState
 from aind_slurm_rest.models.dbv0036_job_step import Dbv0036JobStep
 from aind_slurm_rest.models.dbv0036_job_step_tres import Dbv0036JobStepTres
 from aind_slurm_rest.models.dbv0036_job_step_tres_requested import Dbv0036JobStepTresRequested
 from aind_slurm_rest.models.dbv0036_job_tres import Dbv0036JobTres
 from aind_slurm_rest.models.dbv0036_qos import Dbv0036Qos
```

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/api/default_api.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/api/default_api.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/api/slurm_api.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/api/slurm_api.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/api_client.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -85,15 +85,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/0.0.1/python'
+        self.user_agent = 'OpenAPI-Generator/0.1.0/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         pass
```

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/api_response.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/api_response.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/configuration.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -405,15 +405,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: 0.0.37\n"\
-               "SDK Package Version: 0.0.1".\
+               "SDK Package Version: 0.1.0".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/exceptions.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/exceptions.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/__init__.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 from aind_slurm_rest.models.dbv0036_config_info import Dbv0036ConfigInfo
 from aind_slurm_rest.models.dbv0036_config_response import Dbv0036ConfigResponse
 from aind_slurm_rest.models.dbv0036_coordinator_info import Dbv0036CoordinatorInfo
 from aind_slurm_rest.models.dbv0036_diag import Dbv0036Diag
 from aind_slurm_rest.models.dbv0036_error import Dbv0036Error
 from aind_slurm_rest.models.dbv0036_job import Dbv0036Job
 from aind_slurm_rest.models.dbv0036_job_exit_code import Dbv0036JobExitCode
+from aind_slurm_rest.models.dbv0036_job_het import Dbv0036JobHet
 from aind_slurm_rest.models.dbv0036_job_info import Dbv0036JobInfo
 from aind_slurm_rest.models.dbv0036_job_state import Dbv0036JobState
 from aind_slurm_rest.models.dbv0036_job_step import Dbv0036JobStep
 from aind_slurm_rest.models.dbv0036_job_step_tres import Dbv0036JobStepTres
 from aind_slurm_rest.models.dbv0036_job_step_tres_requested import Dbv0036JobStepTresRequested
 from aind_slurm_rest.models.dbv0036_job_tres import Dbv0036JobTres
 from aind_slurm_rest.models.dbv0036_qos import Dbv0036Qos
```

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0036_account.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0036_account.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0036_account_info.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0036_account_info.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0036_account_response.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0036_account_response.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0036_association.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0036_association.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0036_association_max.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0036_association_max.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0036_association_max_jobs.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0036_association_max_jobs.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0036_association_max_tres.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0036_association_max_tres.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0036_association_max_tres_minutes.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0036_association_max_tres_minutes.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0036_association_max_tres_minutes_per.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0036_association_max_tres_minutes_per.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0036_association_max_tres_per.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0036_association_max_tres_per.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0036_association_short_info.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0036_association_short_info.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0036_associations_info.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0036_associations_info.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0036_cluster_info.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0036_cluster_info.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0036_cluster_info_associations.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0036_cluster_info_associations.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0036_config_info.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0036_config_info.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0036_config_response.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0036_config_response.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0036_coordinator_info.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0036_coordinator_info.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0036_diag.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0036_diag.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0036_error.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0036_error.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0036_job.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0036_job.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,45 +18,45 @@
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, ConfigDict, Field, StrictInt, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
 from aind_slurm_rest.models.dbv0036_association_short_info import Dbv0036AssociationShortInfo
 from aind_slurm_rest.models.dbv0036_job_exit_code import Dbv0036JobExitCode
+from aind_slurm_rest.models.dbv0036_job_het import Dbv0036JobHet
 from aind_slurm_rest.models.dbv0036_job_state import Dbv0036JobState
 from aind_slurm_rest.models.dbv0036_job_step import Dbv0036JobStep
 from aind_slurm_rest.models.dbv0036_job_tres import Dbv0036JobTres
 from aind_slurm_rest.models.dbv0037_job_array import Dbv0037JobArray
 from aind_slurm_rest.models.dbv0037_job_comment import Dbv0037JobComment
-from aind_slurm_rest.models.dbv0037_job_het import Dbv0037JobHet
 from aind_slurm_rest.models.dbv0037_job_mcs import Dbv0037JobMcs
 from aind_slurm_rest.models.dbv0037_job_required import Dbv0037JobRequired
 from aind_slurm_rest.models.dbv0037_job_reservation import Dbv0037JobReservation
 from aind_slurm_rest.models.dbv0037_job_time import Dbv0037JobTime
 from aind_slurm_rest.models.dbv0037_job_wckey import Dbv0037JobWckey
 from typing import Optional, Set
 from typing_extensions import Self
 
 class Dbv0036Job(BaseModel):
     """
     Single job description
     """ # noqa: E501
     account: Optional[StrictStr] = Field(default=None, description="Account charged by job")
     comment: Optional[Dbv0037JobComment] = None
-    allocation_nodes: Optional[StrictStr] = Field(default=None, description="Nodes allocated to job")
+    allocation_nodes: Optional[StrictInt] = Field(default=None, description="Nodes allocated to job")
     array: Optional[Dbv0037JobArray] = None
     time: Optional[Dbv0037JobTime] = None
     association: Optional[Dbv0036AssociationShortInfo] = None
     cluster: Optional[StrictStr] = Field(default=None, description="Assigned cluster")
     constraints: Optional[StrictStr] = Field(default=None, description="Constraints on job")
     derived_exit_code: Optional[Dbv0036JobExitCode] = None
     exit_code: Optional[Dbv0036JobExitCode] = None
     flags: Optional[List[StrictStr]] = Field(default=None, description="List of properties of job")
     group: Optional[StrictStr] = Field(default=None, description="User's group to run job")
-    het: Optional[Dbv0037JobHet] = None
+    het: Optional[Dbv0036JobHet] = None
     job_id: Optional[StrictInt] = Field(default=None, description="Job id")
     name: Optional[StrictStr] = Field(default=None, description="Assigned job name")
     mcs: Optional[Dbv0037JobMcs] = None
     nodes: Optional[StrictStr] = Field(default=None, description="List of nodes allocated for job")
     partition: Optional[StrictStr] = Field(default=None, description="Assigned job's partition")
     priority: Optional[StrictInt] = Field(default=None, description="Priority")
     qos: Optional[StrictStr] = Field(default=None, description="Assigned qos name")
@@ -176,15 +176,15 @@
             "association": Dbv0036AssociationShortInfo.from_dict(obj["association"]) if obj.get("association") is not None else None,
             "cluster": obj.get("cluster"),
             "constraints": obj.get("constraints"),
             "derived_exit_code": Dbv0036JobExitCode.from_dict(obj["derived_exit_code"]) if obj.get("derived_exit_code") is not None else None,
             "exit_code": Dbv0036JobExitCode.from_dict(obj["exit_code"]) if obj.get("exit_code") is not None else None,
             "flags": obj.get("flags"),
             "group": obj.get("group"),
-            "het": Dbv0037JobHet.from_dict(obj["het"]) if obj.get("het") is not None else None,
+            "het": Dbv0036JobHet.from_dict(obj["het"]) if obj.get("het") is not None else None,
             "job_id": obj.get("job_id"),
             "name": obj.get("name"),
             "mcs": Dbv0037JobMcs.from_dict(obj["mcs"]) if obj.get("mcs") is not None else None,
             "nodes": obj.get("nodes"),
             "partition": obj.get("partition"),
             "priority": obj.get("priority"),
             "qos": obj.get("qos"),
```

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0036_job_exit_code.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0036_job_exit_code.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0036_job_info.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0036_job_info.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0036_job_state.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0036_job_state.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0036_job_step.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0036_job_step.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0036_job_step_tres.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0036_job_step_tres.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0036_job_step_tres_requested.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0036_job_step_tres_requested.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0036_job_tres.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0036_job_tres.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0036_qos.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0036_qos.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0036_qos_info.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0036_qos_info.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0036_qos_limits.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0036_qos_limits.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0036_qos_limits_max.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0036_qos_limits_max.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0036_qos_limits_max_jobs.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0036_qos_limits_max_jobs.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0036_qos_limits_max_jobs_per.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0036_qos_limits_max_jobs_per.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0036_qos_limits_max_tres.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0036_qos_limits_max_tres.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0036_qos_limits_max_tres_minutes.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0036_qos_limits_max_tres_minutes.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0036_qos_limits_max_tres_minutes_per.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0036_qos_limits_max_tres_minutes_per.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0036_qos_limits_max_tres_per.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0036_qos_limits_max_tres_per.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0036_qos_limits_min.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0036_qos_limits_min.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0036_qos_limits_min_tres.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0036_qos_limits_min_tres.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0036_qos_limits_min_tres_per.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0036_qos_limits_min_tres_per.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0036_response_account_delete.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0036_response_account_delete.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0036_response_association_delete.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0036_response_association_delete.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0036_response_cluster_add.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0036_response_cluster_add.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0036_response_cluster_delete.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0036_response_cluster_delete.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0036_response_qos_delete.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0036_response_qos_delete.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0036_response_tres.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0036_response_tres.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0036_response_user_delete.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0036_response_user_delete.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0036_response_user_update.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0036_response_user_update.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0036_response_wckey_add.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0036_response_wckey_add.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0036_response_wckey_delete.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0036_response_wckey_delete.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0036_tres_info.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0036_tres_info.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0036_user.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0036_user.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0036_user_associations.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0036_user_associations.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0036_user_info.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0036_user_info.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0036_wckey.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0036_wckey.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0036_wckey_info.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0036_wckey_info.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_account.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_account.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_account_info.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_account_info.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_account_response.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_account_response.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_association.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_association.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_association_default.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_association_default.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_association_max.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_association_max.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_association_max_jobs.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_association_max_jobs.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_association_max_jobs_per.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_association_max_jobs_per.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_association_max_per.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_association_max_per.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_association_max_per_account.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_association_max_per_account.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_association_max_tres.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_association_max_tres.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_association_max_tres_group.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_association_max_tres_group.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_association_max_tres_minutes.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_association_max_tres_minutes.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_association_max_tres_minutes_per.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_association_max_tres_minutes_per.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_association_max_tres_per.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_association_max_tres_per.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_association_min.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_association_min.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_association_short_info.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_association_short_info.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_association_usage.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_association_usage.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_associations_info.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_associations_info.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_cluster_info.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_cluster_info.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_cluster_info_associations.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_cluster_info_associations.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_cluster_info_controller.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_cluster_info_controller.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_config_info.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_config_info.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_config_response.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_config_response.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_coordinator_info.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_coordinator_info.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_diag.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_diag.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_diag_statistics.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_diag_statistics.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_diag_statistics_rollups_inner.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_diag_statistics_rollups_inner.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_diag_statistics_rpcs_inner.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_diag_statistics_rpcs_inner.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_diag_statistics_rpcs_inner_time.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_diag_statistics_rpcs_inner_time.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_diag_statistics_users_inner.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_diag_statistics_users_inner.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_diag_statistics_users_inner_time.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_diag_statistics_users_inner_time.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_error.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_error.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_job.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_job.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_job_array.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_job_array.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_job_array_limits.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_job_array_limits.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_job_array_limits_max.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_job_array_limits_max.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_job_array_limits_max_running.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_job_array_limits_max_running.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_job_comment.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_job_comment.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_job_exit_code.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_job_exit_code.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_job_exit_code_signal.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_job_exit_code_signal.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_job_het.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_job_het.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_job_info.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_job_info.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_job_mcs.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_job_mcs.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_job_required.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_job_required.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_job_reservation.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_job_reservation.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_job_state.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_job_state.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_job_step.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_job_step.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_job_step_cpu.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_job_step_cpu.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_job_step_cpu_requested_frequency.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_job_step_cpu_requested_frequency.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_job_step_nodes.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_job_step_nodes.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_job_step_statistics.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_job_step_statistics.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_job_step_statistics_cpu.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_job_step_statistics_cpu.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_job_step_statistics_energy.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_job_step_statistics_energy.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_job_step_step.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_job_step_step.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_job_step_step_het.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_job_step_step_het.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_job_step_task.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_job_step_task.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_job_step_tasks.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_job_step_tasks.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_job_step_time.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_job_step_time.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_job_step_tres.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_job_step_tres.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_job_step_tres_requested.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_job_step_tres_requested.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_job_time.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_job_time.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_job_time_system.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_job_time_system.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_job_time_total.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_job_time_total.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_job_time_user.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_job_time_user.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_job_tres.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_job_tres.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_job_wckey.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_job_wckey.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_qos.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_qos.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_qos_info.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_qos_info.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_qos_limits.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_qos_limits.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_qos_limits_max.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_qos_limits_max.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_qos_limits_max_accruing.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_qos_limits_max_accruing.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_qos_limits_max_accruing_per.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_qos_limits_max_accruing_per.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_qos_limits_max_jobs.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_qos_limits_max_jobs.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_qos_limits_max_jobs_active_jobs.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_qos_limits_max_jobs_active_jobs.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_qos_limits_max_jobs_active_jobs_per.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_qos_limits_max_jobs_active_jobs_per.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_qos_limits_max_tres.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_qos_limits_max_tres.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_qos_limits_max_tres_minutes.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_qos_limits_max_tres_minutes.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_qos_limits_max_tres_minutes_per.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_qos_limits_max_tres_minutes_per.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_qos_limits_max_tres_per.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_qos_limits_max_tres_per.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_qos_limits_max_wall_clock.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_qos_limits_max_wall_clock.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_qos_limits_max_wall_clock_per.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_qos_limits_max_wall_clock_per.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_qos_limits_min.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_qos_limits_min.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_qos_limits_min_tres.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_qos_limits_min_tres.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_qos_limits_min_tres_per.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_qos_limits_min_tres_per.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_qos_preempt.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_qos_preempt.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_response_account_delete.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_response_account_delete.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_response_association_delete.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_response_association_delete.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_response_associations.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_response_associations.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_response_cluster_add.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_response_cluster_add.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_response_cluster_delete.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_response_cluster_delete.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_response_qos_delete.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_response_qos_delete.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_response_tres.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_response_tres.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_response_user_delete.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_response_user_delete.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_response_user_update.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_response_user_update.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_response_wckey_add.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_response_wckey_add.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_response_wckey_delete.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_response_wckey_delete.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_tres_info.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_tres_info.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_tres_list_inner.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_tres_list_inner.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_user.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_user.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_user_associations.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_user_associations.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_user_default.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_user_default.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_user_info.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_user_info.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_wckey.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_wckey.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/dbv0037_wckey_info.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/dbv0037_wckey_info.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/job_properties.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/job_properties.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/job_properties_exclusive.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/job_properties_exclusive.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/job_properties_nodes.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/job_properties_nodes.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/signal.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/signal.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/v0036_diag.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/v0036_diag.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/v0036_error.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/v0036_error.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/v0036_job_properties.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/v0036_job_properties.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/v0036_job_resources.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/v0036_job_resources.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/v0036_job_response_properties.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/v0036_job_response_properties.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/v0036_job_submission.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/v0036_job_submission.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/v0036_job_submission_response.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/v0036_job_submission_response.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/v0036_jobs_response.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/v0036_jobs_response.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/v0036_node.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/v0036_node.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/v0036_nodes_response.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/v0036_nodes_response.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/v0036_partition.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/v0036_partition.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/v0036_partitions_response.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/v0036_partitions_response.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/v0036_ping.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/v0036_ping.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/v0036_pings.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/v0036_pings.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/v0036_signal.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/v0036_signal.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/v0037_diag.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/v0037_diag.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/v0037_diag_statistics.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/v0037_diag_statistics.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/v0037_error.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/v0037_error.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/v0037_job_properties.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/v0037_job_properties.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/v0037_job_resources.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/v0037_job_resources.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/v0037_job_response_properties.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/v0037_job_response_properties.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/v0037_job_submission.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/v0037_job_submission.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/v0037_job_submission_response.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/v0037_job_submission_response.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/v0037_jobs_response.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/v0037_jobs_response.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/v0037_node.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/v0037_node.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/v0037_node_allocation.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/v0037_node_allocation.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/v0037_nodes_response.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/v0037_nodes_response.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/v0037_partition.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/v0037_partition.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/v0037_partitions_response.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/v0037_partitions_response.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/v0037_ping.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/v0037_ping.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/v0037_pings.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/v0037_pings.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/v0037_reservation.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/v0037_reservation.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/v0037_reservation_purge_completed.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/v0037_reservation_purge_completed.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/v0037_reservations_response.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/v0037_reservations_response.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/models/v0037_signal.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/models/v0037_signal.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest/rest.py` & `aind-slurm-rest-0.1.0/aind_slurm_rest/rest.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/aind_slurm_rest.egg-info/SOURCES.txt` & `aind-slurm-rest-0.1.0/aind_slurm_rest.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 aind_slurm_rest/models/dbv0036_config_info.py
 aind_slurm_rest/models/dbv0036_config_response.py
 aind_slurm_rest/models/dbv0036_coordinator_info.py
 aind_slurm_rest/models/dbv0036_diag.py
 aind_slurm_rest/models/dbv0036_error.py
 aind_slurm_rest/models/dbv0036_job.py
 aind_slurm_rest/models/dbv0036_job_exit_code.py
+aind_slurm_rest/models/dbv0036_job_het.py
 aind_slurm_rest/models/dbv0036_job_info.py
 aind_slurm_rest/models/dbv0036_job_state.py
 aind_slurm_rest/models/dbv0036_job_step.py
 aind_slurm_rest/models/dbv0036_job_step_tres.py
 aind_slurm_rest/models/dbv0036_job_step_tres_requested.py
 aind_slurm_rest/models/dbv0036_job_tres.py
 aind_slurm_rest/models/dbv0036_qos.py
@@ -236,14 +237,15 @@
 test/test_dbv0036_config_info.py
 test/test_dbv0036_config_response.py
 test/test_dbv0036_coordinator_info.py
 test/test_dbv0036_diag.py
 test/test_dbv0036_error.py
 test/test_dbv0036_job.py
 test/test_dbv0036_job_exit_code.py
+test/test_dbv0036_job_het.py
 test/test_dbv0036_job_info.py
 test/test_dbv0036_job_state.py
 test/test_dbv0036_job_step.py
 test/test_dbv0036_job_step_tres.py
 test/test_dbv0036_job_step_tres_requested.py
 test/test_dbv0036_job_tres.py
 test/test_dbv0036_qos.py
```

### Comparing `aind-slurm-rest-0.0.1/pyproject.toml` & `aind-slurm-rest-0.1.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aind_slurm_rest"
-version = "0.0.1"
+version = "0.1.0"
 description = "Slurm Rest API"
 authors = ["SchedMD LLC <sales@schedmd.com>"]
 license = "Apache 2.0"
 readme = "README.md"
 repository = "https://github.com/GIT_USER_ID/GIT_REPO_ID"
 keywords = ["OpenAPI", "OpenAPI-Generator", "Slurm Rest API"]
 include = ["aind_slurm_rest/py.typed"]
```

### Comparing `aind-slurm-rest-0.0.1/setup.py` & `aind-slurm-rest-0.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
 NAME = "aind-slurm-rest"
-VERSION = "0.0.1"
+VERSION = "0.1.0"
 PYTHON_REQUIRES = ">=3.7"
 REQUIRES = [
     "urllib3 >= 1.25.3, < 2.1.0",
     "python-dateutil",
     "pydantic >= 2",
     "typing-extensions >= 4.7.1",
 ]
```

### Comparing `aind-slurm-rest-0.0.1/test/test_dbv0036_account.py` & `aind-slurm-rest-0.1.0/test/test_dbv0036_account.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_dbv0036_account_info.py` & `aind-slurm-rest-0.1.0/test/test_dbv0036_account_info.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_dbv0036_account_response.py` & `aind-slurm-rest-0.1.0/test/test_dbv0036_account_response.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_dbv0036_association.py` & `aind-slurm-rest-0.1.0/test/test_dbv0036_association.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_dbv0036_association_max.py` & `aind-slurm-rest-0.1.0/test/test_dbv0036_association_max.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_dbv0036_association_max_jobs.py` & `aind-slurm-rest-0.1.0/test/test_dbv0036_association_max_jobs.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_dbv0036_association_max_tres.py` & `aind-slurm-rest-0.1.0/test/test_dbv0036_association_max_tres.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_dbv0036_association_max_tres_minutes.py` & `aind-slurm-rest-0.1.0/test/test_dbv0036_association_max_tres_minutes.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_dbv0036_association_max_tres_minutes_per.py` & `aind-slurm-rest-0.1.0/test/test_dbv0036_association_max_tres_minutes_per.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_dbv0036_association_max_tres_per.py` & `aind-slurm-rest-0.1.0/test/test_dbv0036_association_max_tres_per.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_dbv0036_association_short_info.py` & `aind-slurm-rest-0.1.0/test/test_dbv0036_association_short_info.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_dbv0036_associations_info.py` & `aind-slurm-rest-0.1.0/test/test_dbv0036_associations_info.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_dbv0036_cluster_info.py` & `aind-slurm-rest-0.1.0/test/test_dbv0036_cluster_info.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_dbv0036_cluster_info_associations.py` & `aind-slurm-rest-0.1.0/test/test_dbv0036_cluster_info_associations.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_dbv0036_config_info.py` & `aind-slurm-rest-0.1.0/test/test_dbv0036_config_info.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_dbv0036_config_response.py` & `aind-slurm-rest-0.1.0/test/test_dbv0036_config_response.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_dbv0036_coordinator_info.py` & `aind-slurm-rest-0.1.0/test/test_dbv0036_coordinator_info.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_dbv0036_diag.py` & `aind-slurm-rest-0.1.0/test/test_dbv0036_diag.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_dbv0036_error.py` & `aind-slurm-rest-0.1.0/test/test_dbv0036_error.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_dbv0036_job.py` & `aind-slurm-rest-0.1.0/test/test_dbv0036_job.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
         if include_optional:
             return Dbv0036Job(
                 account = '',
                 comment = aind_slurm_rest.models.dbv0_0_37_job_comment.dbv0_0_37_job_comment(
                     administrator = '', 
                     job = '', 
                     system = '', ),
-                allocation_nodes = '',
+                allocation_nodes = 56,
                 array = aind_slurm_rest.models.dbv0_0_37_job_array.dbv0_0_37_job_array(
                     job_id = 56, 
                     limits = aind_slurm_rest.models.dbv0_0_37_job_array_limits.dbv0_0_37_job_array_limits(
                         max = aind_slurm_rest.models.dbv0_0_37_job_array_limits_max.dbv0_0_37_job_array_limits_max(
                             running = aind_slurm_rest.models.dbv0_0_37_job_array_limits_max_running.dbv0_0_37_job_array_limits_max_running(
                                 tasks = 56, ), ), ), 
                     task = '', 
@@ -86,16 +86,16 @@
                     signal = aind_slurm_rest.models.dbv0_0_37_job_exit_code_signal.dbv0_0_37_job_exit_code_signal(
                         signal_id = 56, 
                         name = '', ), ),
                 flags = [
                     ''
                     ],
                 group = '',
-                het = aind_slurm_rest.models.dbv0_0_37_job_het.dbv0_0_37_job_het(
-                    job_id = aind_slurm_rest.models.job_id.job_id(), 
+                het = aind_slurm_rest.models.dbv0_0_36_job_het.dbv0_0_36_job_het(
+                    job_id = 56, 
                     job_offset = aind_slurm_rest.models.job_offset.job_offset(), ),
                 job_id = 56,
                 name = '',
                 mcs = aind_slurm_rest.models.dbv0_0_37_job_mcs.dbv0_0_37_job_mcs(
                     label = '', ),
                 nodes = '',
                 partition = '',
```

### Comparing `aind-slurm-rest-0.0.1/test/test_dbv0036_job_exit_code.py` & `aind-slurm-rest-0.1.0/test/test_dbv0036_job_exit_code.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_dbv0036_job_info.py` & `aind-slurm-rest-0.1.0/test/test_dbv0036_job_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
                 jobs = [
                     aind_slurm_rest.models.dbv0/0/36_job.dbv0.0.36_job(
                         account = '', 
                         comment = aind_slurm_rest.models.dbv0_0_37_job_comment.dbv0_0_37_job_comment(
                             administrator = '', 
                             job = '', 
                             system = '', ), 
-                        allocation_nodes = '', 
+                        allocation_nodes = 56, 
                         array = aind_slurm_rest.models.dbv0_0_37_job_array.dbv0_0_37_job_array(
                             job_id = 56, 
                             limits = aind_slurm_rest.models.dbv0_0_37_job_array_limits.dbv0_0_37_job_array_limits(
                                 max = aind_slurm_rest.models.dbv0_0_37_job_array_limits_max.dbv0_0_37_job_array_limits_max(
                                     running = aind_slurm_rest.models.dbv0_0_37_job_array_limits_max_running.dbv0_0_37_job_array_limits_max_running(
                                         tasks = 56, ), ), ), 
                             task = '', 
@@ -89,16 +89,16 @@
                         exit_code = aind_slurm_rest.models.dbv0/0/36_job_exit_code.dbv0.0.36_job_exit_code(
                             status = '', 
                             return_code = 56, ), 
                         flags = [
                             ''
                             ], 
                         group = '', 
-                        het = aind_slurm_rest.models.dbv0_0_37_job_het.dbv0_0_37_job_het(
-                            job_id = aind_slurm_rest.models.job_id.job_id(), 
+                        het = aind_slurm_rest.models.dbv0_0_36_job_het.dbv0_0_36_job_het(
+                            job_id = 56, 
                             job_offset = aind_slurm_rest.models.job_offset.job_offset(), ), 
                         job_id = 56, 
                         name = '', 
                         mcs = aind_slurm_rest.models.dbv0_0_37_job_mcs.dbv0_0_37_job_mcs(
                             label = '', ), 
                         nodes = '', 
                         partition = '',
```

### Comparing `aind-slurm-rest-0.0.1/test/test_dbv0036_job_state.py` & `aind-slurm-rest-0.1.0/test/test_dbv0036_job_state.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_dbv0036_job_step.py` & `aind-slurm-rest-0.1.0/test/test_dbv0036_job_step.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_dbv0036_job_step_tres.py` & `aind-slurm-rest-0.1.0/test/test_dbv0036_job_step_tres.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_dbv0036_job_step_tres_requested.py` & `aind-slurm-rest-0.1.0/test/test_dbv0036_job_step_tres_requested.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_dbv0036_job_tres.py` & `aind-slurm-rest-0.1.0/test/test_dbv0036_job_tres.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_dbv0036_qos.py` & `aind-slurm-rest-0.1.0/test/test_dbv0036_qos.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_dbv0036_qos_info.py` & `aind-slurm-rest-0.1.0/test/test_dbv0036_qos_info.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_dbv0036_qos_limits.py` & `aind-slurm-rest-0.1.0/test/test_dbv0036_qos_limits.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_dbv0036_qos_limits_max.py` & `aind-slurm-rest-0.1.0/test/test_dbv0036_qos_limits_max.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_dbv0036_qos_limits_max_jobs.py` & `aind-slurm-rest-0.1.0/test/test_dbv0036_qos_limits_max_jobs.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_dbv0036_qos_limits_max_jobs_per.py` & `aind-slurm-rest-0.1.0/test/test_dbv0036_qos_limits_max_jobs_per.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_dbv0036_qos_limits_max_tres.py` & `aind-slurm-rest-0.1.0/test/test_dbv0036_qos_limits_max_tres.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_dbv0036_qos_limits_max_tres_minutes.py` & `aind-slurm-rest-0.1.0/test/test_dbv0036_qos_limits_max_tres_minutes.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_dbv0036_qos_limits_max_tres_minutes_per.py` & `aind-slurm-rest-0.1.0/test/test_dbv0036_qos_limits_max_tres_minutes_per.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_dbv0036_qos_limits_max_tres_per.py` & `aind-slurm-rest-0.1.0/test/test_dbv0036_qos_limits_max_tres_per.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_dbv0036_qos_limits_min.py` & `aind-slurm-rest-0.1.0/test/test_dbv0036_qos_limits_min.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_dbv0036_qos_limits_min_tres.py` & `aind-slurm-rest-0.1.0/test/test_dbv0036_qos_limits_min_tres.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_dbv0036_qos_limits_min_tres_per.py` & `aind-slurm-rest-0.1.0/test/test_dbv0036_qos_limits_min_tres_per.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_dbv0036_response_account_delete.py` & `aind-slurm-rest-0.1.0/test/test_dbv0036_response_account_delete.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_dbv0036_response_association_delete.py` & `aind-slurm-rest-0.1.0/test/test_dbv0036_response_association_delete.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_dbv0036_response_cluster_add.py` & `aind-slurm-rest-0.1.0/test/test_dbv0036_response_cluster_add.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_dbv0036_response_cluster_delete.py` & `aind-slurm-rest-0.1.0/test/test_dbv0036_response_cluster_delete.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_dbv0036_response_qos_delete.py` & `aind-slurm-rest-0.1.0/test/test_dbv0036_response_qos_delete.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_dbv0036_response_tres.py` & `aind-slurm-rest-0.1.0/test/test_dbv0036_response_tres.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_dbv0036_response_user_delete.py` & `aind-slurm-rest-0.1.0/test/test_dbv0036_response_user_delete.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_dbv0036_response_user_update.py` & `aind-slurm-rest-0.1.0/test/test_dbv0036_response_user_update.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_dbv0036_response_wckey_add.py` & `aind-slurm-rest-0.1.0/test/test_dbv0036_response_wckey_add.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_dbv0036_response_wckey_delete.py` & `aind-slurm-rest-0.1.0/test/test_dbv0036_response_wckey_delete.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_dbv0036_tres_info.py` & `aind-slurm-rest-0.1.0/test/test_dbv0036_tres_info.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_dbv0036_user.py` & `aind-slurm-rest-0.1.0/test/test_dbv0036_user.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_dbv0036_user_associations.py` & `aind-slurm-rest-0.1.0/test/test_dbv0036_user_associations.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_dbv0036_user_info.py` & `aind-slurm-rest-0.1.0/test/test_dbv0036_user_info.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_dbv0036_wckey.py` & `aind-slurm-rest-0.1.0/test/test_dbv0036_wckey.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_dbv0036_wckey_info.py` & `aind-slurm-rest-0.1.0/test/test_dbv0036_wckey_info.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_dbv0037_account.py` & `aind-slurm-rest-0.1.0/test/test_dbv0037_account.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_dbv0037_account_info.py` & `aind-slurm-rest-0.1.0/test/test_dbv0037_account_info.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_dbv0037_account_response.py` & `aind-slurm-rest-0.1.0/test/test_dbv0037_account_response.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_dbv0037_association.py` & `aind-slurm-rest-0.1.0/test/test_dbv0037_association.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_dbv0037_association_default.py` & `aind-slurm-rest-0.1.0/test/test_dbv0037_association_default.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_dbv0037_association_max.py` & `aind-slurm-rest-0.1.0/test/test_dbv0037_association_max.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_dbv0037_association_max_jobs.py` & `aind-slurm-rest-0.1.0/test/test_dbv0037_association_max_jobs.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_dbv0037_association_max_jobs_per.py` & `aind-slurm-rest-0.1.0/test/test_dbv0037_association_max_jobs_per.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_dbv0037_association_max_per.py` & `aind-slurm-rest-0.1.0/test/test_dbv0037_association_max_per.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_dbv0037_association_max_per_account.py` & `aind-slurm-rest-0.1.0/test/test_dbv0037_association_max_per_account.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_dbv0037_association_max_tres.py` & `aind-slurm-rest-0.1.0/test/test_dbv0037_association_max_tres.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_dbv0037_association_max_tres_group.py` & `aind-slurm-rest-0.1.0/test/test_dbv0037_association_max_tres_group.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_dbv0037_association_max_tres_minutes.py` & `aind-slurm-rest-0.1.0/test/test_dbv0037_association_max_tres_minutes.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_dbv0037_association_max_tres_minutes_per.py` & `aind-slurm-rest-0.1.0/test/test_dbv0037_association_max_tres_minutes_per.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_dbv0037_association_max_tres_per.py` & `aind-slurm-rest-0.1.0/test/test_dbv0037_association_max_tres_per.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_dbv0037_association_min.py` & `aind-slurm-rest-0.1.0/test/test_dbv0037_association_min.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_dbv0037_association_short_info.py` & `aind-slurm-rest-0.1.0/test/test_dbv0037_association_short_info.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_dbv0037_association_usage.py` & `aind-slurm-rest-0.1.0/test/test_dbv0037_association_usage.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_dbv0037_associations_info.py` & `aind-slurm-rest-0.1.0/test/test_dbv0037_associations_info.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_dbv0037_cluster_info.py` & `aind-slurm-rest-0.1.0/test/test_dbv0037_cluster_info.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_dbv0037_cluster_info_associations.py` & `aind-slurm-rest-0.1.0/test/test_dbv0037_cluster_info_associations.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_dbv0037_cluster_info_controller.py` & `aind-slurm-rest-0.1.0/test/test_dbv0037_cluster_info_controller.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_dbv0037_config_info.py` & `aind-slurm-rest-0.1.0/test/test_dbv0037_config_info.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_dbv0037_config_response.py` & `aind-slurm-rest-0.1.0/test/test_dbv0037_config_response.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_dbv0037_coordinator_info.py` & `aind-slurm-rest-0.1.0/test/test_dbv0037_coordinator_info.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_dbv0037_diag.py` & `aind-slurm-rest-0.1.0/test/test_dbv0037_diag.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_dbv0037_diag_statistics.py` & `aind-slurm-rest-0.1.0/test/test_dbv0037_diag_statistics.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_dbv0037_diag_statistics_rollups_inner.py` & `aind-slurm-rest-0.1.0/test/test_dbv0037_diag_statistics_rollups_inner.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_dbv0037_diag_statistics_rpcs_inner.py` & `aind-slurm-rest-0.1.0/test/test_dbv0037_diag_statistics_rpcs_inner.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_dbv0037_diag_statistics_rpcs_inner_time.py` & `aind-slurm-rest-0.1.0/test/test_dbv0037_diag_statistics_rpcs_inner_time.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_dbv0037_diag_statistics_users_inner.py` & `aind-slurm-rest-0.1.0/test/test_dbv0037_diag_statistics_users_inner.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_dbv0037_diag_statistics_users_inner_time.py` & `aind-slurm-rest-0.1.0/test/test_dbv0037_diag_statistics_users_inner_time.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_dbv0037_error.py` & `aind-slurm-rest-0.1.0/test/test_dbv0037_error.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_dbv0037_job.py` & `aind-slurm-rest-0.1.0/test/test_dbv0037_job.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_dbv0037_job_array.py` & `aind-slurm-rest-0.1.0/test/test_dbv0037_job_array.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_dbv0037_job_array_limits.py` & `aind-slurm-rest-0.1.0/test/test_dbv0037_job_array_limits.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_dbv0037_job_array_limits_max.py` & `aind-slurm-rest-0.1.0/test/test_dbv0037_job_array_limits_max.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_dbv0037_job_array_limits_max_running.py` & `aind-slurm-rest-0.1.0/test/test_dbv0037_job_array_limits_max_running.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_dbv0037_job_comment.py` & `aind-slurm-rest-0.1.0/test/test_dbv0037_job_comment.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_dbv0037_job_exit_code.py` & `aind-slurm-rest-0.1.0/test/test_dbv0037_job_exit_code.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_dbv0037_job_exit_code_signal.py` & `aind-slurm-rest-0.1.0/test/test_dbv0037_job_exit_code_signal.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_dbv0037_job_het.py` & `aind-slurm-rest-0.1.0/test/test_dbv0037_job_het.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_dbv0037_job_info.py` & `aind-slurm-rest-0.1.0/test/test_dbv0037_job_info.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_dbv0037_job_mcs.py` & `aind-slurm-rest-0.1.0/test/test_dbv0037_job_mcs.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_dbv0037_job_required.py` & `aind-slurm-rest-0.1.0/test/test_dbv0037_job_required.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_dbv0037_job_reservation.py` & `aind-slurm-rest-0.1.0/test/test_dbv0037_job_reservation.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_dbv0037_job_state.py` & `aind-slurm-rest-0.1.0/test/test_dbv0037_job_state.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_dbv0037_job_step.py` & `aind-slurm-rest-0.1.0/test/test_dbv0037_job_step.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_dbv0037_job_step_cpu.py` & `aind-slurm-rest-0.1.0/test/test_dbv0037_job_step_cpu.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_dbv0037_job_step_cpu_requested_frequency.py` & `aind-slurm-rest-0.1.0/test/test_dbv0037_job_step_cpu_requested_frequency.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_dbv0037_job_step_nodes.py` & `aind-slurm-rest-0.1.0/test/test_dbv0037_job_step_nodes.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_dbv0037_job_step_statistics.py` & `aind-slurm-rest-0.1.0/test/test_dbv0037_job_step_statistics.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_dbv0037_job_step_statistics_cpu.py` & `aind-slurm-rest-0.1.0/test/test_dbv0037_job_step_statistics_cpu.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_dbv0037_job_step_statistics_energy.py` & `aind-slurm-rest-0.1.0/test/test_dbv0037_job_step_statistics_energy.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_dbv0037_job_step_step.py` & `aind-slurm-rest-0.1.0/test/test_dbv0037_job_step_step.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_dbv0037_job_step_step_het.py` & `aind-slurm-rest-0.1.0/test/test_dbv0037_job_step_step_het.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_dbv0037_job_step_task.py` & `aind-slurm-rest-0.1.0/test/test_dbv0037_job_step_task.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_dbv0037_job_step_tasks.py` & `aind-slurm-rest-0.1.0/test/test_dbv0037_job_step_tasks.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_dbv0037_job_step_time.py` & `aind-slurm-rest-0.1.0/test/test_dbv0037_job_step_time.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_dbv0037_job_step_tres.py` & `aind-slurm-rest-0.1.0/test/test_dbv0037_job_step_tres.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_dbv0037_job_step_tres_requested.py` & `aind-slurm-rest-0.1.0/test/test_dbv0037_job_step_tres_requested.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_dbv0037_job_time.py` & `aind-slurm-rest-0.1.0/test/test_dbv0037_job_time.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_dbv0037_job_time_system.py` & `aind-slurm-rest-0.1.0/test/test_dbv0037_job_time_system.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_dbv0037_job_time_total.py` & `aind-slurm-rest-0.1.0/test/test_dbv0037_job_time_total.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_dbv0037_job_time_user.py` & `aind-slurm-rest-0.1.0/test/test_dbv0037_job_time_user.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_dbv0037_job_tres.py` & `aind-slurm-rest-0.1.0/test/test_dbv0037_job_tres.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_dbv0037_job_wckey.py` & `aind-slurm-rest-0.1.0/test/test_dbv0037_job_wckey.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_dbv0037_qos.py` & `aind-slurm-rest-0.1.0/test/test_dbv0037_qos.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_dbv0037_qos_info.py` & `aind-slurm-rest-0.1.0/test/test_dbv0037_qos_info.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_dbv0037_qos_limits.py` & `aind-slurm-rest-0.1.0/test/test_dbv0037_qos_limits.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_dbv0037_qos_limits_max.py` & `aind-slurm-rest-0.1.0/test/test_dbv0037_qos_limits_max.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_dbv0037_qos_limits_max_accruing.py` & `aind-slurm-rest-0.1.0/test/test_dbv0037_qos_limits_max_accruing.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_dbv0037_qos_limits_max_accruing_per.py` & `aind-slurm-rest-0.1.0/test/test_dbv0037_qos_limits_max_accruing_per.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_dbv0037_qos_limits_max_jobs.py` & `aind-slurm-rest-0.1.0/test/test_dbv0037_qos_limits_max_jobs.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_dbv0037_qos_limits_max_jobs_active_jobs.py` & `aind-slurm-rest-0.1.0/test/test_dbv0037_qos_limits_max_jobs_active_jobs.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_dbv0037_qos_limits_max_jobs_active_jobs_per.py` & `aind-slurm-rest-0.1.0/test/test_dbv0037_qos_limits_max_jobs_active_jobs_per.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_dbv0037_qos_limits_max_tres.py` & `aind-slurm-rest-0.1.0/test/test_dbv0037_qos_limits_max_tres.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_dbv0037_qos_limits_max_tres_minutes.py` & `aind-slurm-rest-0.1.0/test/test_dbv0037_qos_limits_max_tres_minutes.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_dbv0037_qos_limits_max_tres_minutes_per.py` & `aind-slurm-rest-0.1.0/test/test_dbv0037_qos_limits_max_tres_minutes_per.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_dbv0037_qos_limits_max_tres_per.py` & `aind-slurm-rest-0.1.0/test/test_dbv0037_qos_limits_max_tres_per.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_dbv0037_qos_limits_max_wall_clock.py` & `aind-slurm-rest-0.1.0/test/test_dbv0037_qos_limits_max_wall_clock.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_dbv0037_qos_limits_max_wall_clock_per.py` & `aind-slurm-rest-0.1.0/test/test_dbv0037_qos_limits_max_wall_clock_per.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_dbv0037_qos_limits_min.py` & `aind-slurm-rest-0.1.0/test/test_dbv0037_qos_limits_min.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_dbv0037_qos_limits_min_tres.py` & `aind-slurm-rest-0.1.0/test/test_dbv0037_qos_limits_min_tres.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_dbv0037_qos_limits_min_tres_per.py` & `aind-slurm-rest-0.1.0/test/test_dbv0037_qos_limits_min_tres_per.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_dbv0037_qos_preempt.py` & `aind-slurm-rest-0.1.0/test/test_dbv0037_qos_preempt.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_dbv0037_response_account_delete.py` & `aind-slurm-rest-0.1.0/test/test_dbv0037_response_account_delete.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_dbv0037_response_association_delete.py` & `aind-slurm-rest-0.1.0/test/test_dbv0037_response_association_delete.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_dbv0037_response_associations.py` & `aind-slurm-rest-0.1.0/test/test_dbv0037_response_associations.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_dbv0037_response_cluster_add.py` & `aind-slurm-rest-0.1.0/test/test_dbv0037_response_cluster_add.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_dbv0037_response_cluster_delete.py` & `aind-slurm-rest-0.1.0/test/test_dbv0037_response_cluster_delete.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_dbv0037_response_qos_delete.py` & `aind-slurm-rest-0.1.0/test/test_dbv0037_response_qos_delete.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_dbv0037_response_tres.py` & `aind-slurm-rest-0.1.0/test/test_dbv0037_response_tres.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_dbv0037_response_user_delete.py` & `aind-slurm-rest-0.1.0/test/test_dbv0037_response_user_delete.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_dbv0037_response_user_update.py` & `aind-slurm-rest-0.1.0/test/test_dbv0037_response_user_update.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_dbv0037_response_wckey_add.py` & `aind-slurm-rest-0.1.0/test/test_dbv0037_response_wckey_add.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_dbv0037_response_wckey_delete.py` & `aind-slurm-rest-0.1.0/test/test_dbv0037_response_wckey_delete.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_dbv0037_tres_info.py` & `aind-slurm-rest-0.1.0/test/test_dbv0037_tres_info.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_dbv0037_tres_list_inner.py` & `aind-slurm-rest-0.1.0/test/test_dbv0037_tres_list_inner.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_dbv0037_user.py` & `aind-slurm-rest-0.1.0/test/test_dbv0037_user.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_dbv0037_user_associations.py` & `aind-slurm-rest-0.1.0/test/test_dbv0037_user_associations.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_dbv0037_user_default.py` & `aind-slurm-rest-0.1.0/test/test_dbv0037_user_default.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_dbv0037_user_info.py` & `aind-slurm-rest-0.1.0/test/test_dbv0037_user_info.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_dbv0037_wckey.py` & `aind-slurm-rest-0.1.0/test/test_dbv0037_wckey.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_dbv0037_wckey_info.py` & `aind-slurm-rest-0.1.0/test/test_dbv0037_wckey_info.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_default_api.py` & `aind-slurm-rest-0.1.0/test/test_default_api.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_job_properties.py` & `aind-slurm-rest-0.1.0/test/test_job_properties.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_job_properties_exclusive.py` & `aind-slurm-rest-0.1.0/test/test_job_properties_exclusive.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_job_properties_nodes.py` & `aind-slurm-rest-0.1.0/test/test_job_properties_nodes.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_signal.py` & `aind-slurm-rest-0.1.0/test/test_signal.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_slurm_api.py` & `aind-slurm-rest-0.1.0/test/test_slurm_api.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_v0036_diag.py` & `aind-slurm-rest-0.1.0/test/test_v0036_diag.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_v0036_error.py` & `aind-slurm-rest-0.1.0/test/test_v0036_error.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_v0036_job_properties.py` & `aind-slurm-rest-0.1.0/test/test_v0036_job_properties.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_v0036_job_resources.py` & `aind-slurm-rest-0.1.0/test/test_v0036_job_resources.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_v0036_job_response_properties.py` & `aind-slurm-rest-0.1.0/test/test_v0036_job_response_properties.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_v0036_job_submission.py` & `aind-slurm-rest-0.1.0/test/test_v0036_job_submission.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_v0036_job_submission_response.py` & `aind-slurm-rest-0.1.0/test/test_v0036_job_submission_response.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_v0036_jobs_response.py` & `aind-slurm-rest-0.1.0/test/test_v0036_jobs_response.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_v0036_node.py` & `aind-slurm-rest-0.1.0/test/test_v0036_node.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_v0036_nodes_response.py` & `aind-slurm-rest-0.1.0/test/test_v0036_nodes_response.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_v0036_partition.py` & `aind-slurm-rest-0.1.0/test/test_v0036_partition.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_v0036_partitions_response.py` & `aind-slurm-rest-0.1.0/test/test_v0036_partitions_response.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_v0036_ping.py` & `aind-slurm-rest-0.1.0/test/test_v0036_ping.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_v0036_pings.py` & `aind-slurm-rest-0.1.0/test/test_v0036_pings.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_v0036_signal.py` & `aind-slurm-rest-0.1.0/test/test_v0036_signal.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_v0037_diag.py` & `aind-slurm-rest-0.1.0/test/test_v0037_diag.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_v0037_diag_statistics.py` & `aind-slurm-rest-0.1.0/test/test_v0037_diag_statistics.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_v0037_error.py` & `aind-slurm-rest-0.1.0/test/test_v0037_error.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_v0037_job_properties.py` & `aind-slurm-rest-0.1.0/test/test_v0037_job_properties.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_v0037_job_resources.py` & `aind-slurm-rest-0.1.0/test/test_v0037_job_resources.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_v0037_job_response_properties.py` & `aind-slurm-rest-0.1.0/test/test_v0037_job_response_properties.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_v0037_job_submission.py` & `aind-slurm-rest-0.1.0/test/test_v0037_job_submission.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_v0037_job_submission_response.py` & `aind-slurm-rest-0.1.0/test/test_v0037_job_submission_response.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_v0037_jobs_response.py` & `aind-slurm-rest-0.1.0/test/test_v0037_jobs_response.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_v0037_node.py` & `aind-slurm-rest-0.1.0/test/test_v0037_node.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_v0037_node_allocation.py` & `aind-slurm-rest-0.1.0/test/test_v0037_node_allocation.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_v0037_nodes_response.py` & `aind-slurm-rest-0.1.0/test/test_v0037_nodes_response.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_v0037_partition.py` & `aind-slurm-rest-0.1.0/test/test_v0037_partition.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_v0037_partitions_response.py` & `aind-slurm-rest-0.1.0/test/test_v0037_partitions_response.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_v0037_ping.py` & `aind-slurm-rest-0.1.0/test/test_v0037_ping.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_v0037_pings.py` & `aind-slurm-rest-0.1.0/test/test_v0037_pings.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_v0037_reservation.py` & `aind-slurm-rest-0.1.0/test/test_v0037_reservation.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_v0037_reservation_purge_completed.py` & `aind-slurm-rest-0.1.0/test/test_v0037_reservation_purge_completed.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_v0037_reservations_response.py` & `aind-slurm-rest-0.1.0/test/test_v0037_reservations_response.py`

 * *Files identical despite different names*

### Comparing `aind-slurm-rest-0.0.1/test/test_v0037_signal.py` & `aind-slurm-rest-0.1.0/test/test_v0037_signal.py`

 * *Files identical despite different names*

