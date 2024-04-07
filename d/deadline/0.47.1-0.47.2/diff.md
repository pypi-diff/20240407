# Comparing `tmp/deadline-0.47.1.tar.gz` & `tmp/deadline-0.47.2.tar.gz`

## Comparing `deadline-0.47.1.tar` & `deadline-0.47.2.tar`

### file list

```diff
@@ -1,107 +1,107 @@
--rw-r--r--   0        0        0    50578 2020-02-02 00:00:00.000000 deadline-0.47.1/THIRD_PARTY_LICENSES
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 deadline-0.47.1/_version.py
--rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 deadline-0.47.1/src/deadline/__main__.py
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 deadline-0.47.1/src/deadline/client/__init__.py
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 deadline-0.47.1/src/deadline/client/_version.py
--rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 deadline-0.47.1/src/deadline/client/exceptions.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 deadline-0.47.1/src/deadline/client/py.typed
--rw-r--r--   0        0        0     2858 2020-02-02 00:00:00.000000 deadline-0.47.1/src/deadline/client/api/__init__.py
--rw-r--r--   0        0        0     3771 2020-02-02 00:00:00.000000 deadline-0.47.1/src/deadline/client/api/_list_apis.py
--rw-r--r--   0        0        0     6856 2020-02-02 00:00:00.000000 deadline-0.47.1/src/deadline/client/api/_loginout.py
--rw-r--r--   0        0        0     2999 2020-02-02 00:00:00.000000 deadline-0.47.1/src/deadline/client/api/_queue_parameters.py
--rw-r--r--   0        0        0    13355 2020-02-02 00:00:00.000000 deadline-0.47.1/src/deadline/client/api/_session.py
--rw-r--r--   0        0        0    17160 2020-02-02 00:00:00.000000 deadline-0.47.1/src/deadline/client/api/_submit_job_bundle.py
--rw-r--r--   0        0        0    14070 2020-02-02 00:00:00.000000 deadline-0.47.1/src/deadline/client/api/_telemetry.py
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 deadline-0.47.1/src/deadline/client/cli/__init__.py
--rw-r--r--   0        0        0     6214 2020-02-02 00:00:00.000000 deadline-0.47.1/src/deadline/client/cli/_common.py
--rw-r--r--   0        0        0     2408 2020-02-02 00:00:00.000000 deadline-0.47.1/src/deadline/client/cli/_deadline_cli.py
--rw-r--r--   0        0        0    11102 2020-02-02 00:00:00.000000 deadline-0.47.1/src/deadline/client/cli/_deadline_web_url.py
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 deadline-0.47.1/src/deadline/client/cli/deadline_cli_main.py
--rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 deadline-0.47.1/src/deadline/client/cli/deadline_dev_gui_main.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 deadline-0.47.1/src/deadline/client/cli/_groups/__init__.py
--rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 deadline-0.47.1/src/deadline/client/cli/_groups/_sigint_handler.py
--rw-r--r--   0        0        0     3967 2020-02-02 00:00:00.000000 deadline-0.47.1/src/deadline/client/cli/_groups/auth_group.py
--rw-r--r--   0        0        0    10522 2020-02-02 00:00:00.000000 deadline-0.47.1/src/deadline/client/cli/_groups/bundle_group.py
--rw-r--r--   0        0        0     3582 2020-02-02 00:00:00.000000 deadline-0.47.1/src/deadline/client/cli/_groups/config_group.py
--rw-r--r--   0        0        0     2023 2020-02-02 00:00:00.000000 deadline-0.47.1/src/deadline/client/cli/_groups/farm_group.py
--rw-r--r--   0        0        0     3717 2020-02-02 00:00:00.000000 deadline-0.47.1/src/deadline/client/cli/_groups/fleet_group.py
--rw-r--r--   0        0        0     4909 2020-02-02 00:00:00.000000 deadline-0.47.1/src/deadline/client/cli/_groups/handle_web_url_command.py
--rw-r--r--   0        0        0    39347 2020-02-02 00:00:00.000000 deadline-0.47.1/src/deadline/client/cli/_groups/job_group.py
--rw-r--r--   0        0        0     3370 2020-02-02 00:00:00.000000 deadline-0.47.1/src/deadline/client/cli/_groups/queue_group.py
--rw-r--r--   0        0        0     3050 2020-02-02 00:00:00.000000 deadline-0.47.1/src/deadline/client/cli/_groups/worker_group.py
--rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 deadline-0.47.1/src/deadline/client/config/__init__.py
--rw-r--r--   0        0        0    17510 2020-02-02 00:00:00.000000 deadline-0.47.1/src/deadline/client/config/config_file.py
--rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 deadline-0.47.1/src/deadline/client/job_bundle/__init__.py
--rw-r--r--   0        0        0     2257 2020-02-02 00:00:00.000000 deadline-0.47.1/src/deadline/client/job_bundle/_yaml.py
--rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 deadline-0.47.1/src/deadline/client/job_bundle/adaptors.py
--rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 deadline-0.47.1/src/deadline/client/job_bundle/job_template.py
--rw-r--r--   0        0        0     4771 2020-02-02 00:00:00.000000 deadline-0.47.1/src/deadline/client/job_bundle/loader.py
--rw-r--r--   0        0        0    32688 2020-02-02 00:00:00.000000 deadline-0.47.1/src/deadline/client/job_bundle/parameters.py
--rw-r--r--   0        0        0     6027 2020-02-02 00:00:00.000000 deadline-0.47.1/src/deadline/client/job_bundle/submission.py
--rw-r--r--   0        0        0     5933 2020-02-02 00:00:00.000000 deadline-0.47.1/src/deadline/client/ui/__init__.py
--rw-r--r--   0        0        0     7788 2020-02-02 00:00:00.000000 deadline-0.47.1/src/deadline/client/ui/cli_job_submitter.py
--rw-r--r--   0        0        0     8163 2020-02-02 00:00:00.000000 deadline-0.47.1/src/deadline/client/ui/deadline_authentication_status.py
--rw-r--r--   0        0        0     5306 2020-02-02 00:00:00.000000 deadline-0.47.1/src/deadline/client/ui/dev_application.py
--rw-r--r--   0        0        0     7159 2020-02-02 00:00:00.000000 deadline-0.47.1/src/deadline/client/ui/job_bundle_submitter.py
--rw-r--r--   0        0        0     1967 2020-02-02 00:00:00.000000 deadline-0.47.1/src/deadline/client/ui/dataclasses/__init__.py
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 deadline-0.47.1/src/deadline/client/ui/dialogs/__init__.py
--rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 deadline-0.47.1/src/deadline/client/ui/dialogs/_types.py
--rw-r--r--   0        0        0    34201 2020-02-02 00:00:00.000000 deadline-0.47.1/src/deadline/client/ui/dialogs/deadline_config_dialog.py
--rw-r--r--   0        0        0     6419 2020-02-02 00:00:00.000000 deadline-0.47.1/src/deadline/client/ui/dialogs/deadline_login_dialog.py
--rw-r--r--   0        0        0    25968 2020-02-02 00:00:00.000000 deadline-0.47.1/src/deadline/client/ui/dialogs/submit_job_progress_dialog.py
--rw-r--r--   0        0        0    20671 2020-02-02 00:00:00.000000 deadline-0.47.1/src/deadline/client/ui/dialogs/submit_job_to_deadline_dialog.py
--rw-r--r--   0        0        0     1899 2020-02-02 00:00:00.000000 deadline-0.47.1/src/deadline/client/ui/resources/deadline_logo.svg
--rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 deadline-0.47.1/src/deadline/client/ui/resources/info.svg
--rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 deadline-0.47.1/src/deadline/client/ui/resources/blender_example_bundle/template.yaml
--rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 deadline-0.47.1/src/deadline/client/ui/resources/cli_job_bundle/template.yaml
--rw-r--r--   0        0        0     6139 2020-02-02 00:00:00.000000 deadline-0.47.1/src/deadline/client/ui/resources/controls_demo_job_bundle/template.yaml
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 deadline-0.47.1/src/deadline/client/ui/widgets/__init__.py
--rw-r--r--   0        0        0     4289 2020-02-02 00:00:00.000000 deadline-0.47.1/src/deadline/client/ui/widgets/cli_job_settings_tab.py
--rw-r--r--   0        0        0     3958 2020-02-02 00:00:00.000000 deadline-0.47.1/src/deadline/client/ui/widgets/deadline_authentication_status_widget.py
--rw-r--r--   0        0        0    36343 2020-02-02 00:00:00.000000 deadline-0.47.1/src/deadline/client/ui/widgets/host_requirements_tab.py
--rw-r--r--   0        0        0    14402 2020-02-02 00:00:00.000000 deadline-0.47.1/src/deadline/client/ui/widgets/job_attachments_tab.py
--rw-r--r--   0        0        0     5340 2020-02-02 00:00:00.000000 deadline-0.47.1/src/deadline/client/ui/widgets/job_bundle_settings_tab.py
--rw-r--r--   0        0        0    31193 2020-02-02 00:00:00.000000 deadline-0.47.1/src/deadline/client/ui/widgets/openjd_parameters_widget.py
--rw-r--r--   0        0        0     8735 2020-02-02 00:00:00.000000 deadline-0.47.1/src/deadline/client/ui/widgets/path_widgets.py
--rw-r--r--   0        0        0    23261 2020-02-02 00:00:00.000000 deadline-0.47.1/src/deadline/client/ui/widgets/shared_job_settings_tab.py
--rw-r--r--   0        0        0     8687 2020-02-02 00:00:00.000000 deadline-0.47.1/src/deadline/client/ui/widgets/spinbox_widgets.py
--rw-r--r--   0        0        0     5998 2020-02-02 00:00:00.000000 deadline-0.47.1/src/deadline/job_attachments/README.md
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 deadline-0.47.1/src/deadline/job_attachments/__init__.py
--rw-r--r--   0        0        0     2796 2020-02-02 00:00:00.000000 deadline-0.47.1/src/deadline/job_attachments/_utils.py
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 deadline-0.47.1/src/deadline/job_attachments/_version.py
--rw-r--r--   0        0        0    26842 2020-02-02 00:00:00.000000 deadline-0.47.1/src/deadline/job_attachments/asset_sync.py
--rw-r--r--   0        0        0    46742 2020-02-02 00:00:00.000000 deadline-0.47.1/src/deadline/job_attachments/download.py
--rw-r--r--   0        0        0     4748 2020-02-02 00:00:00.000000 deadline-0.47.1/src/deadline/job_attachments/exceptions.py
--rw-r--r--   0        0        0    10861 2020-02-02 00:00:00.000000 deadline-0.47.1/src/deadline/job_attachments/models.py
--rw-r--r--   0        0        0     7308 2020-02-02 00:00:00.000000 deadline-0.47.1/src/deadline/job_attachments/os_file_permission.py
--rw-r--r--   0        0        0    15063 2020-02-02 00:00:00.000000 deadline-0.47.1/src/deadline/job_attachments/progress_tracker.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 deadline-0.47.1/src/deadline/job_attachments/py.typed
--rw-r--r--   0        0        0    50280 2020-02-02 00:00:00.000000 deadline-0.47.1/src/deadline/job_attachments/upload.py
--rw-r--r--   0        0        0    21984 2020-02-02 00:00:00.000000 deadline-0.47.1/src/deadline/job_attachments/vfs.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 deadline-0.47.1/src/deadline/job_attachments/_aws/__init__.py
--rw-r--r--   0        0        0     4423 2020-02-02 00:00:00.000000 deadline-0.47.1/src/deadline/job_attachments/_aws/aws_clients.py
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 deadline-0.47.1/src/deadline/job_attachments/_aws/aws_config.py
--rw-r--r--   0        0        0     5127 2020-02-02 00:00:00.000000 deadline-0.47.1/src/deadline/job_attachments/_aws/deadline.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 deadline-0.47.1/src/deadline/job_attachments/_windows/__init__.py
--rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 deadline-0.47.1/src/deadline/job_attachments/_windows/file.py
--rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 deadline-0.47.1/src/deadline/job_attachments/asset_manifests/__init__.py
--rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 deadline-0.47.1/src/deadline/job_attachments/asset_manifests/_canonical_json.py
--rw-r--r--   0        0        0     2471 2020-02-02 00:00:00.000000 deadline-0.47.1/src/deadline/job_attachments/asset_manifests/base_manifest.py
--rw-r--r--   0        0        0     2864 2020-02-02 00:00:00.000000 deadline-0.47.1/src/deadline/job_attachments/asset_manifests/decode.py
--rw-r--r--   0        0        0     1484 2020-02-02 00:00:00.000000 deadline-0.47.1/src/deadline/job_attachments/asset_manifests/hash_algorithms.py
--rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 deadline-0.47.1/src/deadline/job_attachments/asset_manifests/manifest_model.py
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 deadline-0.47.1/src/deadline/job_attachments/asset_manifests/versions.py
--rw-r--r--   0        0        0     1850 2020-02-02 00:00:00.000000 deadline-0.47.1/src/deadline/job_attachments/asset_manifests/schemas/2023-03-03.json
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 deadline-0.47.1/src/deadline/job_attachments/asset_manifests/v2023_03_03/__init__.py
--rw-r--r--   0        0        0     3321 2020-02-02 00:00:00.000000 deadline-0.47.1/src/deadline/job_attachments/asset_manifests/v2023_03_03/asset_manifest.py
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 deadline-0.47.1/src/deadline/job_attachments/caches/__init__.py
--rw-r--r--   0        0        0     3394 2020-02-02 00:00:00.000000 deadline-0.47.1/src/deadline/job_attachments/caches/cache_db.py
--rw-r--r--   0        0        0     3080 2020-02-02 00:00:00.000000 deadline-0.47.1/src/deadline/job_attachments/caches/hash_cache.py
--rw-r--r--   0        0        0     3070 2020-02-02 00:00:00.000000 deadline-0.47.1/src/deadline/job_attachments/caches/s3_check_cache.py
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 deadline-0.47.1/.gitignore
--rw-r--r--   0        0        0    10142 2020-02-02 00:00:00.000000 deadline-0.47.1/LICENSE
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 deadline-0.47.1/NOTICE
--rw-r--r--   0        0        0     6246 2020-02-02 00:00:00.000000 deadline-0.47.1/README.md
--rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 deadline-0.47.1/hatch.toml
--rw-r--r--   0        0        0     6717 2020-02-02 00:00:00.000000 deadline-0.47.1/pyproject.toml
--rw-r--r--   0        0        0     7927 2020-02-02 00:00:00.000000 deadline-0.47.1/PKG-INFO
+-rw-r--r--   0        0        0    50578 2020-02-02 00:00:00.000000 deadline-0.47.2/THIRD_PARTY_LICENSES
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 deadline-0.47.2/_version.py
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/__main__.py
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/client/__init__.py
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/client/_version.py
+-rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/client/exceptions.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/client/py.typed
+-rw-r--r--   0        0        0     2858 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/client/api/__init__.py
+-rw-r--r--   0        0        0     3771 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/client/api/_list_apis.py
+-rw-r--r--   0        0        0     6856 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/client/api/_loginout.py
+-rw-r--r--   0        0        0     2999 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/client/api/_queue_parameters.py
+-rw-r--r--   0        0        0    13355 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/client/api/_session.py
+-rw-r--r--   0        0        0    17160 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/client/api/_submit_job_bundle.py
+-rw-r--r--   0        0        0    14070 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/client/api/_telemetry.py
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/client/cli/__init__.py
+-rw-r--r--   0        0        0     6214 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/client/cli/_common.py
+-rw-r--r--   0        0        0     2408 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/client/cli/_deadline_cli.py
+-rw-r--r--   0        0        0    11102 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/client/cli/_deadline_web_url.py
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/client/cli/deadline_cli_main.py
+-rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/client/cli/deadline_dev_gui_main.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/client/cli/_groups/__init__.py
+-rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/client/cli/_groups/_sigint_handler.py
+-rw-r--r--   0        0        0     3967 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/client/cli/_groups/auth_group.py
+-rw-r--r--   0        0        0    10522 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/client/cli/_groups/bundle_group.py
+-rw-r--r--   0        0        0     3582 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/client/cli/_groups/config_group.py
+-rw-r--r--   0        0        0     2023 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/client/cli/_groups/farm_group.py
+-rw-r--r--   0        0        0     3717 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/client/cli/_groups/fleet_group.py
+-rw-r--r--   0        0        0     4909 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/client/cli/_groups/handle_web_url_command.py
+-rw-r--r--   0        0        0    39347 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/client/cli/_groups/job_group.py
+-rw-r--r--   0        0        0     3370 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/client/cli/_groups/queue_group.py
+-rw-r--r--   0        0        0     3050 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/client/cli/_groups/worker_group.py
+-rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/client/config/__init__.py
+-rw-r--r--   0        0        0    17510 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/client/config/config_file.py
+-rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/client/job_bundle/__init__.py
+-rw-r--r--   0        0        0     2257 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/client/job_bundle/_yaml.py
+-rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/client/job_bundle/adaptors.py
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/client/job_bundle/job_template.py
+-rw-r--r--   0        0        0     4771 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/client/job_bundle/loader.py
+-rw-r--r--   0        0        0    32688 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/client/job_bundle/parameters.py
+-rw-r--r--   0        0        0     6027 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/client/job_bundle/submission.py
+-rw-r--r--   0        0        0     6246 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/client/ui/__init__.py
+-rw-r--r--   0        0        0     7788 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/client/ui/cli_job_submitter.py
+-rw-r--r--   0        0        0     8163 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/client/ui/deadline_authentication_status.py
+-rw-r--r--   0        0        0     5306 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/client/ui/dev_application.py
+-rw-r--r--   0        0        0     7159 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/client/ui/job_bundle_submitter.py
+-rw-r--r--   0        0        0     1967 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/client/ui/dataclasses/__init__.py
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/client/ui/dialogs/__init__.py
+-rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/client/ui/dialogs/_types.py
+-rw-r--r--   0        0        0    34201 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/client/ui/dialogs/deadline_config_dialog.py
+-rw-r--r--   0        0        0     6419 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/client/ui/dialogs/deadline_login_dialog.py
+-rw-r--r--   0        0        0    25968 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/client/ui/dialogs/submit_job_progress_dialog.py
+-rw-r--r--   0        0        0    20671 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/client/ui/dialogs/submit_job_to_deadline_dialog.py
+-rw-r--r--   0        0        0     1899 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/client/ui/resources/deadline_logo.svg
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/client/ui/resources/info.svg
+-rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/client/ui/resources/blender_example_bundle/template.yaml
+-rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/client/ui/resources/cli_job_bundle/template.yaml
+-rw-r--r--   0        0        0     6139 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/client/ui/resources/controls_demo_job_bundle/template.yaml
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/client/ui/widgets/__init__.py
+-rw-r--r--   0        0        0     4289 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/client/ui/widgets/cli_job_settings_tab.py
+-rw-r--r--   0        0        0     3958 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/client/ui/widgets/deadline_authentication_status_widget.py
+-rw-r--r--   0        0        0    36343 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/client/ui/widgets/host_requirements_tab.py
+-rw-r--r--   0        0        0    14402 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/client/ui/widgets/job_attachments_tab.py
+-rw-r--r--   0        0        0     5340 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/client/ui/widgets/job_bundle_settings_tab.py
+-rw-r--r--   0        0        0    31193 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/client/ui/widgets/openjd_parameters_widget.py
+-rw-r--r--   0        0        0     8735 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/client/ui/widgets/path_widgets.py
+-rw-r--r--   0        0        0    23261 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/client/ui/widgets/shared_job_settings_tab.py
+-rw-r--r--   0        0        0     8687 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/client/ui/widgets/spinbox_widgets.py
+-rw-r--r--   0        0        0     5998 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/job_attachments/README.md
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/job_attachments/__init__.py
+-rw-r--r--   0        0        0     2796 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/job_attachments/_utils.py
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/job_attachments/_version.py
+-rw-r--r--   0        0        0    26842 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/job_attachments/asset_sync.py
+-rw-r--r--   0        0        0    46754 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/job_attachments/download.py
+-rw-r--r--   0        0        0     4748 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/job_attachments/exceptions.py
+-rw-r--r--   0        0        0    10861 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/job_attachments/models.py
+-rw-r--r--   0        0        0     7308 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/job_attachments/os_file_permission.py
+-rw-r--r--   0        0        0    15063 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/job_attachments/progress_tracker.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/job_attachments/py.typed
+-rw-r--r--   0        0        0    51260 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/job_attachments/upload.py
+-rw-r--r--   0        0        0    21984 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/job_attachments/vfs.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/job_attachments/_aws/__init__.py
+-rw-r--r--   0        0        0     4423 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/job_attachments/_aws/aws_clients.py
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/job_attachments/_aws/aws_config.py
+-rw-r--r--   0        0        0     5127 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/job_attachments/_aws/deadline.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/job_attachments/_windows/__init__.py
+-rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/job_attachments/_windows/file.py
+-rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/job_attachments/asset_manifests/__init__.py
+-rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/job_attachments/asset_manifests/_canonical_json.py
+-rw-r--r--   0        0        0     2471 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/job_attachments/asset_manifests/base_manifest.py
+-rw-r--r--   0        0        0     2864 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/job_attachments/asset_manifests/decode.py
+-rw-r--r--   0        0        0     1484 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/job_attachments/asset_manifests/hash_algorithms.py
+-rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/job_attachments/asset_manifests/manifest_model.py
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/job_attachments/asset_manifests/versions.py
+-rw-r--r--   0        0        0     1850 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/job_attachments/asset_manifests/schemas/2023-03-03.json
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/job_attachments/asset_manifests/v2023_03_03/__init__.py
+-rw-r--r--   0        0        0     3321 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/job_attachments/asset_manifests/v2023_03_03/asset_manifest.py
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/job_attachments/caches/__init__.py
+-rw-r--r--   0        0        0     3394 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/job_attachments/caches/cache_db.py
+-rw-r--r--   0        0        0     3080 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/job_attachments/caches/hash_cache.py
+-rw-r--r--   0        0        0     3070 2020-02-02 00:00:00.000000 deadline-0.47.2/src/deadline/job_attachments/caches/s3_check_cache.py
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 deadline-0.47.2/.gitignore
+-rw-r--r--   0        0        0    10142 2020-02-02 00:00:00.000000 deadline-0.47.2/LICENSE
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 deadline-0.47.2/NOTICE
+-rw-r--r--   0        0        0     6250 2020-02-02 00:00:00.000000 deadline-0.47.2/README.md
+-rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 deadline-0.47.2/hatch.toml
+-rw-r--r--   0        0        0     6717 2020-02-02 00:00:00.000000 deadline-0.47.2/pyproject.toml
+-rw-r--r--   0        0        0     7931 2020-02-02 00:00:00.000000 deadline-0.47.2/PKG-INFO
```

### Comparing `deadline-0.47.1/THIRD_PARTY_LICENSES` & `deadline-0.47.2/THIRD_PARTY_LICENSES`

 * *Files identical despite different names*

### Comparing `deadline-0.47.1/src/deadline/client/exceptions.py` & `deadline-0.47.2/src/deadline/client/exceptions.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.1/src/deadline/client/api/__init__.py` & `deadline-0.47.2/src/deadline/client/api/__init__.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.1/src/deadline/client/api/_list_apis.py` & `deadline-0.47.2/src/deadline/client/api/_list_apis.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.1/src/deadline/client/api/_loginout.py` & `deadline-0.47.2/src/deadline/client/api/_loginout.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.1/src/deadline/client/api/_queue_parameters.py` & `deadline-0.47.2/src/deadline/client/api/_queue_parameters.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.1/src/deadline/client/api/_session.py` & `deadline-0.47.2/src/deadline/client/api/_session.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.1/src/deadline/client/api/_submit_job_bundle.py` & `deadline-0.47.2/src/deadline/client/api/_submit_job_bundle.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.1/src/deadline/client/api/_telemetry.py` & `deadline-0.47.2/src/deadline/client/api/_telemetry.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.1/src/deadline/client/cli/_common.py` & `deadline-0.47.2/src/deadline/client/cli/_common.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.1/src/deadline/client/cli/_deadline_cli.py` & `deadline-0.47.2/src/deadline/client/cli/_deadline_cli.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.1/src/deadline/client/cli/_deadline_web_url.py` & `deadline-0.47.2/src/deadline/client/cli/_deadline_web_url.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.1/src/deadline/client/cli/deadline_dev_gui_main.py` & `deadline-0.47.2/src/deadline/client/cli/deadline_dev_gui_main.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.1/src/deadline/client/cli/_groups/_sigint_handler.py` & `deadline-0.47.2/src/deadline/client/cli/_groups/_sigint_handler.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.1/src/deadline/client/cli/_groups/auth_group.py` & `deadline-0.47.2/src/deadline/client/cli/_groups/auth_group.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.1/src/deadline/client/cli/_groups/bundle_group.py` & `deadline-0.47.2/src/deadline/client/cli/_groups/bundle_group.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.1/src/deadline/client/cli/_groups/config_group.py` & `deadline-0.47.2/src/deadline/client/cli/_groups/config_group.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.1/src/deadline/client/cli/_groups/farm_group.py` & `deadline-0.47.2/src/deadline/client/cli/_groups/farm_group.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.1/src/deadline/client/cli/_groups/fleet_group.py` & `deadline-0.47.2/src/deadline/client/cli/_groups/fleet_group.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.1/src/deadline/client/cli/_groups/handle_web_url_command.py` & `deadline-0.47.2/src/deadline/client/cli/_groups/handle_web_url_command.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.1/src/deadline/client/cli/_groups/job_group.py` & `deadline-0.47.2/src/deadline/client/cli/_groups/job_group.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.1/src/deadline/client/cli/_groups/queue_group.py` & `deadline-0.47.2/src/deadline/client/cli/_groups/queue_group.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.1/src/deadline/client/cli/_groups/worker_group.py` & `deadline-0.47.2/src/deadline/client/cli/_groups/worker_group.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.1/src/deadline/client/config/__init__.py` & `deadline-0.47.2/src/deadline/client/config/__init__.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.1/src/deadline/client/config/config_file.py` & `deadline-0.47.2/src/deadline/client/config/config_file.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.1/src/deadline/client/job_bundle/__init__.py` & `deadline-0.47.2/src/deadline/client/job_bundle/__init__.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.1/src/deadline/client/job_bundle/_yaml.py` & `deadline-0.47.2/src/deadline/client/job_bundle/_yaml.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.1/src/deadline/client/job_bundle/adaptors.py` & `deadline-0.47.2/src/deadline/client/job_bundle/adaptors.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.1/src/deadline/client/job_bundle/job_template.py` & `deadline-0.47.2/src/deadline/client/job_bundle/job_template.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.1/src/deadline/client/job_bundle/loader.py` & `deadline-0.47.2/src/deadline/client/job_bundle/loader.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.1/src/deadline/client/job_bundle/parameters.py` & `deadline-0.47.2/src/deadline/client/job_bundle/parameters.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.1/src/deadline/client/job_bundle/submission.py` & `deadline-0.47.2/src/deadline/client/job_bundle/submission.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.1/src/deadline/client/ui/__init__.py` & `deadline-0.47.2/src/deadline/client/ui/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -56,25 +56,27 @@
         from deadline.client.ui.cli_job_submitter import show_cli_job_submitter
 
         show_cli_job_submitter()
 
         app.exec()
     """
     import importlib
+    import os
     from os.path import basename, dirname, join, normpath
     import shlex
     import shutil
     import subprocess
     import sys
     from pathlib import Path
 
     import click
 
-    has_pyside = importlib.util.find_spec("PySide6") or importlib.util.find_spec("PySide2")
-    if not has_pyside:
+    has_pyside6 = importlib.util.find_spec("PySide6")
+    has_pyside2 = importlib.util.find_spec("PySide2")
+    if not (has_pyside6 or has_pyside2):
         message = "Optional GUI components for deadline are unavailable. Would you like to install PySide?"
         will_install_gui = click.confirm(message, default=False)
         if not will_install_gui:
             click.echo("Unable to continue without GUI, exiting")
             sys.exit(1)
 
         # this should match what's in the pyproject.toml
@@ -116,14 +118,20 @@
                 sys.exit(1)
         else:
             # standard python sys.executable
             # TODO: swap to deadline[gui]==version once published and at the same
             # time consider local editables `pip install .[gui]`
             subprocess.run([sys.executable, "-m", "pip", "install", pyside6_pypi])
 
+    # set QT_API to inform qtpy which dependencies to look for.
+    # default to pyside6 and fallback to pyside2.
+    # Does not work with PyQt5 which is qtpy default
+    os.environ["QT_API"] = "pyside6"
+    if has_pyside2:
+        os.environ["QT_API"] = "pyside2"
     try:
         from qtpy.QtGui import QIcon
         from qtpy.QtWidgets import QApplication, QMessageBox
     except ImportError as e:
         click.echo(f"Failed to import qtpy/PySide/Qt, which is required to show the GUI:\n{e}")
         sys.exit(1)
```

### Comparing `deadline-0.47.1/src/deadline/client/ui/cli_job_submitter.py` & `deadline-0.47.2/src/deadline/client/ui/cli_job_submitter.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.1/src/deadline/client/ui/deadline_authentication_status.py` & `deadline-0.47.2/src/deadline/client/ui/deadline_authentication_status.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.1/src/deadline/client/ui/dev_application.py` & `deadline-0.47.2/src/deadline/client/ui/dev_application.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.1/src/deadline/client/ui/job_bundle_submitter.py` & `deadline-0.47.2/src/deadline/client/ui/job_bundle_submitter.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.1/src/deadline/client/ui/dataclasses/__init__.py` & `deadline-0.47.2/src/deadline/client/ui/dataclasses/__init__.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.1/src/deadline/client/ui/dialogs/deadline_config_dialog.py` & `deadline-0.47.2/src/deadline/client/ui/dialogs/deadline_config_dialog.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.1/src/deadline/client/ui/dialogs/deadline_login_dialog.py` & `deadline-0.47.2/src/deadline/client/ui/dialogs/deadline_login_dialog.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.1/src/deadline/client/ui/dialogs/submit_job_progress_dialog.py` & `deadline-0.47.2/src/deadline/client/ui/dialogs/submit_job_progress_dialog.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.1/src/deadline/client/ui/dialogs/submit_job_to_deadline_dialog.py` & `deadline-0.47.2/src/deadline/client/ui/dialogs/submit_job_to_deadline_dialog.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.1/src/deadline/client/ui/resources/deadline_logo.svg` & `deadline-0.47.2/src/deadline/client/ui/resources/deadline_logo.svg`

 * *Files identical despite different names*

### Comparing `deadline-0.47.1/src/deadline/client/ui/resources/blender_example_bundle/template.yaml` & `deadline-0.47.2/src/deadline/client/ui/resources/blender_example_bundle/template.yaml`

 * *Files identical despite different names*

### Comparing `deadline-0.47.1/src/deadline/client/ui/resources/cli_job_bundle/template.yaml` & `deadline-0.47.2/src/deadline/client/ui/resources/cli_job_bundle/template.yaml`

 * *Files identical despite different names*

### Comparing `deadline-0.47.1/src/deadline/client/ui/resources/controls_demo_job_bundle/template.yaml` & `deadline-0.47.2/src/deadline/client/ui/resources/controls_demo_job_bundle/template.yaml`

 * *Files identical despite different names*

### Comparing `deadline-0.47.1/src/deadline/client/ui/widgets/cli_job_settings_tab.py` & `deadline-0.47.2/src/deadline/client/ui/widgets/cli_job_settings_tab.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.1/src/deadline/client/ui/widgets/deadline_authentication_status_widget.py` & `deadline-0.47.2/src/deadline/client/ui/widgets/deadline_authentication_status_widget.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.1/src/deadline/client/ui/widgets/host_requirements_tab.py` & `deadline-0.47.2/src/deadline/client/ui/widgets/host_requirements_tab.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.1/src/deadline/client/ui/widgets/job_attachments_tab.py` & `deadline-0.47.2/src/deadline/client/ui/widgets/job_attachments_tab.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.1/src/deadline/client/ui/widgets/job_bundle_settings_tab.py` & `deadline-0.47.2/src/deadline/client/ui/widgets/job_bundle_settings_tab.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.1/src/deadline/client/ui/widgets/openjd_parameters_widget.py` & `deadline-0.47.2/src/deadline/client/ui/widgets/openjd_parameters_widget.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.1/src/deadline/client/ui/widgets/path_widgets.py` & `deadline-0.47.2/src/deadline/client/ui/widgets/path_widgets.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.1/src/deadline/client/ui/widgets/shared_job_settings_tab.py` & `deadline-0.47.2/src/deadline/client/ui/widgets/shared_job_settings_tab.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.1/src/deadline/client/ui/widgets/spinbox_widgets.py` & `deadline-0.47.2/src/deadline/client/ui/widgets/spinbox_widgets.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.1/src/deadline/job_attachments/README.md` & `deadline-0.47.2/src/deadline/job_attachments/README.md`

 * *Files identical despite different names*

### Comparing `deadline-0.47.1/src/deadline/job_attachments/_utils.py` & `deadline-0.47.2/src/deadline/job_attachments/_utils.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.1/src/deadline/job_attachments/asset_sync.py` & `deadline-0.47.2/src/deadline/job_attachments/asset_sync.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.1/src/deadline/job_attachments/download.py` & `deadline-0.47.2/src/deadline/job_attachments/download.py`

 * *Files 0% similar despite different names*

```diff
@@ -118,15 +118,15 @@
         ) from exc
     except BotoCoreError as bce:
         raise JobAttachmentS3BotoCoreError(
             action="downloading binary file",
             error_details=str(bce),
         ) from bce
     except Exception as e:
-        raise AssetSyncError from e
+        raise AssetSyncError(e) from e
 
 
 def _get_output_manifest_prefix(
     s3_settings: JobAttachmentS3Settings,
     farm_id: str,
     queue_id: str,
     job_id: str,
@@ -216,15 +216,15 @@
         raise JobAttachmentS3BotoCoreError(
             action="listing bucket contents",
             error_details=str(bce),
         ) from bce
     except JobAttachmentsError:
         raise  # pass along JobAttachmentsErrors if we get them
     except Exception as e:
-        raise AssetSyncError from e
+        raise AssetSyncError(e) from e
 
     # 2. Select all files in the last subfolder (alphabetically) under each "task-{any}" folder.
     for task_folder, files in task_prefixes.items():
         last_subfolder = sorted(
             set(f.split("/")[len(task_folder.split("/"))] for f in files), reverse=True
         )[0]
         manifests_keys += [f for f in files if f.startswith(f"{task_folder}/{last_subfolder}/")]
@@ -512,15 +512,15 @@
             process_client_error(exc, status_code)
     except BotoCoreError as bce:
         raise JobAttachmentS3BotoCoreError(
             action="downloading file",
             error_details=str(bce),
         ) from bce
     except Exception as e:
-        raise AssetSyncError from e
+        raise AssetSyncError(e) from e
 
     download_logger.debug(f"Downloaded {file.path} to {str(local_file_name)}")
     os.utime(local_file_name, (modified_time_override, modified_time_override))  # type: ignore[arg-type]
 
     return (file_bytes, local_file_name)
 
 
@@ -642,15 +642,15 @@
         ) from exc
     except BotoCoreError as bce:
         raise JobAttachmentS3BotoCoreError(
             action="checking for the existence of an object in the S3 bucket",
             error_details=str(bce),
         ) from bce
     except Exception as e:
-        raise AssetSyncError from e
+        raise AssetSyncError(e) from e
 
     return head["Metadata"].get("asset-root", None)
 
 
 def get_job_output_paths_by_asset_root(
     s3_settings: JobAttachmentS3Settings,
     farm_id: str,
```

### Comparing `deadline-0.47.1/src/deadline/job_attachments/exceptions.py` & `deadline-0.47.2/src/deadline/job_attachments/exceptions.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.1/src/deadline/job_attachments/models.py` & `deadline-0.47.2/src/deadline/job_attachments/models.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.1/src/deadline/job_attachments/os_file_permission.py` & `deadline-0.47.2/src/deadline/job_attachments/os_file_permission.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.1/src/deadline/job_attachments/progress_tracker.py` & `deadline-0.47.2/src/deadline/job_attachments/progress_tracker.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.1/src/deadline/job_attachments/upload.py` & `deadline-0.47.2/src/deadline/job_attachments/upload.py`

 * *Files 2% similar despite different names*

```diff
@@ -428,15 +428,15 @@
                 ) from exc
             except BotoCoreError as bce:
                 raise JobAttachmentS3BotoCoreError(
                     action="uploading file",
                     error_details=str(bce),
                 ) from bce
             except Exception as e:
-                raise AssetSyncError from e
+                raise AssetSyncError(e) from e
 
     @contextmanager
     def _open_non_symlink_file_binary(
         self, path: str
     ) -> Generator[Optional[BufferedReader], None, None]:
         """
         Open a file in binary mode after verifying that it is not a symbolic link.
@@ -586,15 +586,15 @@
             return False
         except BotoCoreError as bce:
             raise JobAttachmentS3BotoCoreError(
                 action="checking for the existence of an object in the S3 bucket",
                 error_details=str(bce),
             ) from bce
         except Exception as e:
-            raise AssetSyncError from e
+            raise AssetSyncError(e) from e
 
     def upload_bytes_to_s3(
         self,
         bytes: BytesIO,
         bucket: str,
         key: str,
         progress_handler: Optional[Callable[[int], None]] = None,
@@ -640,15 +640,15 @@
             ) from exc
         except BotoCoreError as bce:
             raise JobAttachmentS3BotoCoreError(
                 action="uploading binary file",
                 error_details=str(bce),
             ) from bce
         except Exception as e:
-            raise AssetSyncError from e
+            raise AssetSyncError(e) from e
 
 
 class S3AssetManager:
     """
     Asset handler that creates an asset manifest and uploads assets. Based on an S3 file system.
     """
 
@@ -828,15 +828,16 @@
             # If the path is relative to any of the File System Location of LOCAL type,
             # groups the files into a single group using the path of that location.
             matched_root = self._find_matched_root_from_local_type_locations(
                 groupings=groupings,
                 abs_path=abs_path,
                 local_type_locations=local_type_locations,
             )
-            groupings[matched_root].inputs.add(abs_path)
+            matched_group = self._get_matched_group(matched_root, groupings)
+            matched_group.inputs.add(abs_path)
 
         for _path in output_paths:
             abs_path = Path(os.path.normpath(Path(_path).absolute()))
 
             # Skips the upload if the path is relative to any of the File System Location
             # of SHARED type that was set in the Job.
             if any(_is_relative_to(abs_path, shared) for shared in shared_type_locations):
@@ -845,15 +846,16 @@
             # If the path is relative to any of the File System Location of LOCAL type,
             # groups the files into a single group using the path of that location.
             matched_root = self._find_matched_root_from_local_type_locations(
                 groupings=groupings,
                 abs_path=abs_path,
                 local_type_locations=local_type_locations,
             )
-            groupings[matched_root].outputs.add(abs_path)
+            matched_group = self._get_matched_group(matched_root, groupings)
+            matched_group.outputs.add(abs_path)
 
         for _path in referenced_paths:
             abs_path = Path(os.path.normpath(Path(_path).absolute()))
 
             # Skips the reference if the path is relative to any of the File System Location
             # of SHARED type that was set in the Job.
             if any(_is_relative_to(abs_path, shared) for shared in shared_type_locations):
@@ -861,29 +863,44 @@
             # If the path is relative to any of the File System Location of LOCAL type,
             # groups the references into a single group using the path of that location.
             matched_root = self._find_matched_root_from_local_type_locations(
                 groupings=groupings,
                 abs_path=abs_path,
                 local_type_locations=local_type_locations,
             )
-            groupings[matched_root].references.add(abs_path)
+            matched_group = self._get_matched_group(matched_root, groupings)
+            matched_group.references.add(abs_path)
 
         # Finally, build the list of asset root groups
         for asset_group in groupings.values():
             common_path: Path = Path(
                 os.path.commonpath(
                     list(asset_group.inputs | asset_group.outputs | asset_group.references)
                 )
             )
             if common_path.is_file():
                 common_path = common_path.parent
             asset_group.root_path = str(common_path)
 
         return list(groupings.values())
 
+    def _get_matched_group(
+        self, root_path: str, groupings: dict[str, AssetRootGroup]
+    ) -> AssetRootGroup:
+        root_normcase = os.path.normcase(root_path)
+        matched_group = next(
+            (group for key, group in groupings.items() if os.path.normcase(key) == root_normcase),
+            None,
+        )
+        if matched_group is None:
+            raise ValueError(
+                f"No group found for the root path '{root_path}' in the groupings dictionary: {groupings}"
+            )
+        return matched_group
+
     def _find_matched_root_from_local_type_locations(
         self,
         groupings: dict[str, AssetRootGroup],
         abs_path: Path,
         local_type_locations: dict[str, str] = {},
     ) -> str:
         """
@@ -902,17 +919,21 @@
         if matched_root is not None:
             if matched_root not in groupings:
                 groupings[matched_root] = AssetRootGroup(
                     file_system_location_name=local_type_locations[matched_root],
                 )
             return matched_root
         else:
+            keys_normcase = [os.path.normcase(key) for key in groupings.keys()]
             top_directory = PurePath(abs_path).parts[0]
-            if top_directory not in groupings:
+            top_directory_normcase = os.path.normcase(top_directory)
+            if top_directory_normcase not in keys_normcase:
                 groupings[top_directory] = AssetRootGroup()
+            else:
+                return top_directory_normcase
             return top_directory
 
     def _get_total_size_of_files(self, paths: list[str]) -> int:
         total_bytes = 0
         try:
             for path in paths:
                 total_bytes += Path(path).resolve().stat().st_size
```

### Comparing `deadline-0.47.1/src/deadline/job_attachments/vfs.py` & `deadline-0.47.2/src/deadline/job_attachments/vfs.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.1/src/deadline/job_attachments/_aws/aws_clients.py` & `deadline-0.47.2/src/deadline/job_attachments/_aws/aws_clients.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.1/src/deadline/job_attachments/_aws/deadline.py` & `deadline-0.47.2/src/deadline/job_attachments/_aws/deadline.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.1/src/deadline/job_attachments/_windows/file.py` & `deadline-0.47.2/src/deadline/job_attachments/_windows/file.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.1/src/deadline/job_attachments/asset_manifests/__init__.py` & `deadline-0.47.2/src/deadline/job_attachments/asset_manifests/__init__.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.1/src/deadline/job_attachments/asset_manifests/_canonical_json.py` & `deadline-0.47.2/src/deadline/job_attachments/asset_manifests/_canonical_json.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.1/src/deadline/job_attachments/asset_manifests/base_manifest.py` & `deadline-0.47.2/src/deadline/job_attachments/asset_manifests/base_manifest.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.1/src/deadline/job_attachments/asset_manifests/decode.py` & `deadline-0.47.2/src/deadline/job_attachments/asset_manifests/decode.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.1/src/deadline/job_attachments/asset_manifests/hash_algorithms.py` & `deadline-0.47.2/src/deadline/job_attachments/asset_manifests/hash_algorithms.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.1/src/deadline/job_attachments/asset_manifests/manifest_model.py` & `deadline-0.47.2/src/deadline/job_attachments/asset_manifests/manifest_model.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.1/src/deadline/job_attachments/asset_manifests/schemas/2023-03-03.json` & `deadline-0.47.2/src/deadline/job_attachments/asset_manifests/schemas/2023-03-03.json`

 * *Files identical despite different names*

### Comparing `deadline-0.47.1/src/deadline/job_attachments/asset_manifests/v2023_03_03/asset_manifest.py` & `deadline-0.47.2/src/deadline/job_attachments/asset_manifests/v2023_03_03/asset_manifest.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.1/src/deadline/job_attachments/caches/cache_db.py` & `deadline-0.47.2/src/deadline/job_attachments/caches/cache_db.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.1/src/deadline/job_attachments/caches/hash_cache.py` & `deadline-0.47.2/src/deadline/job_attachments/caches/hash_cache.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.1/src/deadline/job_attachments/caches/s3_check_cache.py` & `deadline-0.47.2/src/deadline/job_attachments/caches/s3_check_cache.py`

 * *Files identical despite different names*

### Comparing `deadline-0.47.1/LICENSE` & `deadline-0.47.2/LICENSE`

 * *Files identical despite different names*

### Comparing `deadline-0.47.1/README.md` & `deadline-0.47.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 The AWS Deadline Cloud client can be installed by the standard python packaging mechanisms:
 ```sh
 $ pip install deadline
 ```
 
 or if you want the optional gui dependencies:
 ```sh
-pip install deadline[gui]
+$ pip install "deadline[gui]"
 ```
 
 ## Usage
 
 After installation it can then be used as a command line tool:
 ```sh
 $ deadline farm list
```

### Comparing `deadline-0.47.1/hatch.toml` & `deadline-0.47.2/hatch.toml`

 * *Files identical despite different names*

### Comparing `deadline-0.47.1/pyproject.toml` & `deadline-0.47.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `deadline-0.47.1/PKG-INFO` & `deadline-0.47.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: deadline
-Version: 0.47.1
+Version: 0.47.2
 Summary: Multi-purpose library and command line tool that implements functionality to support applications using AWS Deadline Cloud.
 Project-URL: Homepage, https://github.com/aws-deadline/deadline-cloud
 Project-URL: Source, https://github.com/aws-deadline/deadline-cloud
 Author: Amazon Web Services
 License-Expression: Apache-2.0
 License-File: LICENSE
 License-File: NOTICE
@@ -68,15 +68,15 @@
 The AWS Deadline Cloud client can be installed by the standard python packaging mechanisms:
 ```sh
 $ pip install deadline
 ```
 
 or if you want the optional gui dependencies:
 ```sh
-pip install deadline[gui]
+$ pip install "deadline[gui]"
 ```
 
 ## Usage
 
 After installation it can then be used as a command line tool:
 ```sh
 $ deadline farm list
```

