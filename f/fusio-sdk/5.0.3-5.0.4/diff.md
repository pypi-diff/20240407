# Comparing `tmp/fusio-sdk-5.0.3.tar.gz` & `tmp/fusio-sdk-5.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fusio-sdk-5.0.3.tar", last modified: Sat Apr  6 19:28:29 2024, max compression
+gzip compressed data, was "fusio-sdk-5.0.4.tar", last modified: Sat Apr  6 19:50:15 2024, max compression
```

## Comparing `fusio-sdk-5.0.3.tar` & `fusio-sdk-5.0.4.tar`

### file list

```diff
@@ -1,274 +1,274 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 19:28:29.866751 fusio-sdk-5.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2305 2024-04-06 19:28:29.866751 fusio-sdk-5.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-06 19:28:26.000000 fusio-sdk-5.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 19:28:29.866751 fusio-sdk-5.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 19:28:29.814751 fusio-sdk-5.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 19:28:29.866751 fusio-sdk-5.0.3/src/fusio_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2305 2024-04-06 19:28:29.000000 fusio-sdk-5.0.3/src/fusio_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8902 2024-04-06 19:28:29.000000 fusio-sdk-5.0.3/src/fusio_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 19:28:29.000000 fusio-sdk-5.0.3/src/fusio_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-06 19:28:29.000000 fusio-sdk-5.0.3/src/fusio_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-06 19:28:29.000000 fusio-sdk-5.0.3/src/fusio_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 19:28:29.862751 fusio-sdk-5.0.3/src/sdk/
--rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/authorization_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_account_change_password.py
--rw-r--r--   0 runner    (1001) docker     (127)     3957 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_account_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      902 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_action.py
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_action_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_action_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_action_create.py
--rw-r--r--   0 runner    (1001) docker     (127)      793 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_action_execute_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_action_execute_request_body.py
--rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_action_execute_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_action_execute_response_body.py
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_action_execute_response_headers.py
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_action_index.py
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_action_index_entry.py
--rw-r--r--   0 runner    (1001) docker     (127)    10435 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_action_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_action_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_app.py
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_app_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_app_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     8218 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_app_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_app_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_audit.py
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_audit_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_audit_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     3293 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_audit_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_category.py
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_category_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_category_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     7059 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_category_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_category_update.py
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_config_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     4508 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_config_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_config_update.py
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_connection_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_connection_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_connection_create.py
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_connection_index.py
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_connection_index_entry.py
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_connection_introspection_entities.py
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_connection_introspection_entity.py
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_connection_introspection_entity_row.py
--rw-r--r--   0 runner    (1001) docker     (127)    13073 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_connection_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_connection_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_cronjob.py
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_cronjob_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_cronjob_create.py
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_cronjob_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     7026 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_cronjob_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_cronjob_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_dashboard.py
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_dashboard_app.py
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_dashboard_apps.py
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_dashboard_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_dashboard_requests.py
--rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_dashboard_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      764 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_dashboard_transaction.py
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_dashboard_transactions.py
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_dashboard_user.py
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_dashboard_users.py
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_event.py
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_event_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_event_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     6960 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_event_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_event_update.py
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_generator_index_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_generator_index_providers.py
--rw-r--r--   0 runner    (1001) docker     (127)      714 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_generator_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)      742 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_generator_provider_changelog.py
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_generator_provider_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5223 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_generator_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      939 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_identity.py
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_identity_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_identity_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_identity_create.py
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_identity_index.py
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_identity_index_entry.py
--rw-r--r--   0 runner    (1001) docker     (127)     9180 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_identity_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_identity_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_log.py
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_log_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_log_error.py
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_log_error_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     5821 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_log_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_marketplace_app.py
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_marketplace_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_marketplace_collection_apps.py
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_marketplace_install.py
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_marketplace_local_app.py
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_marketplace_remote_app.py
--rw-r--r--   0 runner    (1001) docker     (127)     6622 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_marketplace_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_operation.py
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_operation_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_operation_create.py
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_operation_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_operation_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     7092 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_operation_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_operation_throws.py
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_operation_update.py
--rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_page.py
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_page_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_page_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     6927 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_page_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_page_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_plan.py
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_plan_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_plan_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     6927 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_plan_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_plan_update.py
--rw-r--r--   0 runner    (1001) docker     (127)      974 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_rate.py
--rw-r--r--   0 runner    (1001) docker     (127)      748 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_rate_allocation.py
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_rate_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_rate_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     6927 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_rate_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_rate_update.py
--rw-r--r--   0 runner    (1001) docker     (127)      583 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_role.py
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_role_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_role_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     6927 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_role_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_role_update.py
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_schema_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_schema_create.py
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_schema_form.py
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_schema_preview_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_schema_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     9668 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_schema_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_schema_update.py
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_scope.py
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_scope_categories.py
--rw-r--r--   0 runner    (1001) docker     (127)      606 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_scope_category.py
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_scope_category_scope.py
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_scope_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_scope_create.py
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_scope_operation.py
--rw-r--r--   0 runner    (1001) docker     (127)     8117 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_scope_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_scope_update.py
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_sdk_generate.py
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_sdk_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_sdk_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_sdk_types.py
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_statistic_chart.py
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_statistic_chart_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_statistic_count.py
--rw-r--r--   0 runner    (1001) docker     (127)    18570 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_statistic_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     6142 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     2959 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_tenant_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      820 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_token.py
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_token_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3183 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_token_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_transaction.py
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_transaction_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3409 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_transaction_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_trash_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_trash_data_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_trash_restore.py
--rw-r--r--   0 runner    (1001) docker     (127)     4059 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_trash_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_trash_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_user.py
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_user_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_user_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     6927 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_user_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_user_update.py
--rw-r--r--   0 runner    (1001) docker     (127)      825 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_webhook.py
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_webhook_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_webhook_create.py
--rw-r--r--   0 runner    (1001) docker     (127)      746 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_webhook_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     6919 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_webhook_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/backend_webhook_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/common_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)      751 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/common_form_container.py
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/common_form_element.py
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/common_form_element_input.py
--rw-r--r--   0 runner    (1001) docker     (127)      557 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/common_form_element_select.py
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/common_form_element_select_option.py
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/common_form_element_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/common_form_element_text_area.py
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/common_message.py
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/common_message_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/common_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)    14020 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/consumer_account_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/consumer_app.py
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/consumer_app_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/consumer_app_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     6915 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/consumer_app_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/consumer_app_update.py
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/consumer_authorize_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/consumer_authorize_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/consumer_authorize_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/consumer_authorize_response_token.py
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/consumer_event.py
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/consumer_event_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1647 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/consumer_event_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      538 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/consumer_grant.py
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/consumer_grant_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2939 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/consumer_grant_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/consumer_identity.py
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/consumer_identity_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3632 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/consumer_identity_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      928 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/consumer_log.py
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/consumer_log_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2901 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/consumer_log_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      680 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/consumer_page.py
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/consumer_page_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2909 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/consumer_page_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/consumer_payment_checkout_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/consumer_payment_checkout_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/consumer_payment_portal_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/consumer_payment_portal_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3122 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/consumer_payment_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/consumer_plan.py
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/consumer_plan_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2920 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/consumer_plan_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/consumer_scope.py
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/consumer_scope_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1647 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/consumer_scope_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     2963 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/consumer_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/consumer_token.py
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/consumer_token_access_token.py
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/consumer_token_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/consumer_token_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     7090 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/consumer_token_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/consumer_token_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/consumer_transaction.py
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/consumer_transaction_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3032 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/consumer_transaction_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/consumer_user_account.py
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/consumer_user_activate.py
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/consumer_user_email.py
--rw-r--r--   0 runner    (1001) docker     (127)      583 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/consumer_user_jwt.py
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/consumer_user_login.py
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/consumer_user_password_reset.py
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/consumer_user_plan.py
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/consumer_user_refresh.py
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/consumer_user_register.py
--rw-r--r--   0 runner    (1001) docker     (127)      824 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/consumer_webhook.py
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/consumer_webhook_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/consumer_webhook_create.py
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/consumer_webhook_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     7047 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/consumer_webhook_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/consumer_webhook_update.py
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/passthru.py
--rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/system_about.py
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/system_about_apps.py
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/system_about_link.py
--rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/system_connection_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/system_health_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     5655 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/system_meta_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      918 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/system_o_auth_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/system_payment_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/system_route.py
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/system_route_method.py
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/system_route_path.py
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/system_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/system_schema_form.py
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/system_schema_type_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-06 19:28:25.000000 fusio-sdk-5.0.3/src/sdk/system_tag.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 19:50:15.245665 fusio-sdk-5.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2305 2024-04-06 19:50:15.245665 fusio-sdk-5.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 19:50:15.245665 fusio-sdk-5.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 19:50:15.197665 fusio-sdk-5.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 19:50:15.245665 fusio-sdk-5.0.4/src/fusio_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2305 2024-04-06 19:50:15.000000 fusio-sdk-5.0.4/src/fusio_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8902 2024-04-06 19:50:15.000000 fusio-sdk-5.0.4/src/fusio_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 19:50:15.000000 fusio-sdk-5.0.4/src/fusio_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-06 19:50:15.000000 fusio-sdk-5.0.4/src/fusio_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-06 19:50:15.000000 fusio-sdk-5.0.4/src/fusio_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 19:50:15.245665 fusio-sdk-5.0.4/src/sdk/
+-rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/authorization_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_account_change_password.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3962 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_account_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_action_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_action_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_action_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_action_execute_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_action_execute_request_body.py
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_action_execute_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_action_execute_response_body.py
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_action_execute_response_headers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_action_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_action_index_entry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10445 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_action_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_action_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_app_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_app_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8224 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_app_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_app_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_audit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_audit_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_audit_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3296 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_audit_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_category.py
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_category_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_category_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7065 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_category_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_category_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_config_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4513 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_config_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_config_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_connection_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_connection_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_connection_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_connection_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_connection_index_entry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_connection_introspection_entities.py
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_connection_introspection_entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_connection_introspection_entity_row.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13083 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_connection_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_connection_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_cronjob.py
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_cronjob_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_cronjob_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_cronjob_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7032 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_cronjob_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_cronjob_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_dashboard_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_dashboard_apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_dashboard_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_dashboard_requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_dashboard_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_dashboard_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_dashboard_transactions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_dashboard_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_dashboard_users.py
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_event_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_event_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6966 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_event_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_event_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_generator_index_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      506 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_generator_index_providers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_generator_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_generator_provider_changelog.py
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_generator_provider_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5230 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_generator_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_identity.py
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_identity_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_identity_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_identity_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_identity_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_identity_index_entry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9188 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_identity_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_identity_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_log.py
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_log_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_log_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_log_error_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5826 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_log_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_marketplace_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_marketplace_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_marketplace_collection_apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_marketplace_install.py
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_marketplace_local_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_marketplace_remote_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6627 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_marketplace_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_operation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_operation_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_operation_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_operation_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_operation_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7098 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_operation_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_operation_throws.py
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_operation_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_page.py
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_page_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_page_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6933 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_page_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_page_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_plan_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_plan_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6933 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_plan_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_plan_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_rate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_rate_allocation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_rate_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_rate_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6933 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_rate_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_rate_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_role_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_role_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6933 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_role_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_role_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)      891 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_schema_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_schema_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_schema_form.py
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_schema_preview_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_schema_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9676 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_schema_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_schema_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_scope_categories.py
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_scope_category.py
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_scope_category_scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_scope_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_scope_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_scope_operation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8124 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_scope_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_scope_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_sdk_generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_sdk_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2597 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_sdk_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_sdk_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_statistic_chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_statistic_chart_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_statistic_count.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18573 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_statistic_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6171 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2961 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_tenant_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      820 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_token_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3186 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_token_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_transaction_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3412 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_transaction_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_trash_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_trash_data_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_trash_restore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4064 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_trash_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_trash_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_user_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_user_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6933 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_user_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_user_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_webhook.py
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_webhook_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_webhook_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_webhook_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6925 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_webhook_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/backend_webhook_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/common_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/common_form_container.py
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/common_form_element.py
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/common_form_element_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/common_form_element_select.py
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/common_form_element_select_option.py
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/common_form_element_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/common_form_element_text_area.py
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/common_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/common_message_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/common_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14034 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/consumer_account_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/consumer_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/consumer_app_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/consumer_app_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6921 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/consumer_app_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/consumer_app_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/consumer_authorize_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/consumer_authorize_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/consumer_authorize_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/consumer_authorize_response_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/consumer_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/consumer_event_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1649 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/consumer_event_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/consumer_grant.py
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/consumer_grant_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2942 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/consumer_grant_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/consumer_identity.py
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/consumer_identity_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3635 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/consumer_identity_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      928 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/consumer_log.py
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/consumer_log_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2904 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/consumer_log_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/consumer_page.py
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/consumer_page_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/consumer_page_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/consumer_payment_checkout_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/consumer_payment_checkout_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/consumer_payment_portal_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/consumer_payment_portal_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3127 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/consumer_payment_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/consumer_plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/consumer_plan_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2923 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/consumer_plan_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/consumer_scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/consumer_scope_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1649 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/consumer_scope_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2976 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/consumer_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/consumer_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/consumer_token_access_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/consumer_token_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/consumer_token_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7097 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/consumer_token_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/consumer_token_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/consumer_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/consumer_transaction_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3035 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/consumer_transaction_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/consumer_user_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/consumer_user_activate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/consumer_user_email.py
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/consumer_user_jwt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/consumer_user_login.py
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/consumer_user_password_reset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/consumer_user_plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/consumer_user_refresh.py
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/consumer_user_register.py
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/consumer_webhook.py
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/consumer_webhook_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/consumer_webhook_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/consumer_webhook_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7053 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/consumer_webhook_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/consumer_webhook_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/passthru.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/system_about.py
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/system_about_apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/system_about_link.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/system_connection_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/system_health_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5662 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/system_meta_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/system_o_auth_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/system_payment_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/system_route.py
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/system_route_method.py
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/system_route_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/system_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/system_schema_form.py
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/system_schema_type_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2024-04-06 19:50:11.000000 fusio-sdk-5.0.4/src/sdk/system_tag.py
```

### Comparing `fusio-sdk-5.0.3/LICENSE` & `fusio-sdk-5.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.3/PKG-INFO` & `fusio-sdk-5.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fusio-sdk
-Version: 5.0.3
+Version: 5.0.4
 Summary: SDK to talk to the Fusio REST API
 Author-email: Christoph Kappestein <christoph.kappestein@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/apioo/fusio-sdk-python
 Project-URL: Issues, https://github.com/apioo/fusio-sdk-sdkgen-python/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `fusio-sdk-5.0.3/README.md` & `fusio-sdk-5.0.4/README.md`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.3/pyproject.toml` & `fusio-sdk-5.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "fusio-sdk"
-version = "5.0.3"
+version = "5.0.4"
 authors = [
   { name="Christoph Kappestein", email="christoph.kappestein@gmail.com" },
 ]
 description = "SDK to talk to the Fusio REST API"
 readme = "README.md"
 requires-python = ">=3.8"
 license = {text = "MIT"}
```

### Comparing `fusio-sdk-5.0.3/src/fusio_sdk.egg-info/PKG-INFO` & `fusio-sdk-5.0.4/src/fusio_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fusio-sdk
-Version: 5.0.3
+Version: 5.0.4
 Summary: SDK to talk to the Fusio REST API
 Author-email: Christoph Kappestein <christoph.kappestein@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/apioo/fusio-sdk-python
 Project-URL: Issues, https://github.com/apioo/fusio-sdk-sdkgen-python/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `fusio-sdk-5.0.3/src/fusio_sdk.egg-info/SOURCES.txt` & `fusio-sdk-5.0.4/src/fusio_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.3/src/sdk/authorization_tag.py` & `fusio-sdk-5.0.4/src/sdk/authorization_tag.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 https://sdkgen.app
 """
 
 import requests
 import sdkgen
 from requests import RequestException
 
-from backend_user import BackendUser
-from common_message import CommonMessage
-from common_message_exception import CommonMessageException
+from .backend_user import BackendUser
+from .common_message import CommonMessage
+from .common_message_exception import CommonMessageException
 
 class AuthorizationTag(sdkgen.TagAbstract):
     def __init__(self, http_client: requests.Session, parser: sdkgen.Parser):
         super().__init__(http_client, parser)
 
     pass
```

### Comparing `fusio-sdk-5.0.3/src/sdk/backend_account_change_password.py` & `fusio-sdk-5.0.4/src/sdk/backend_account_change_password.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.3/src/sdk/backend_account_tag.py` & `fusio-sdk-5.0.4/src/sdk/backend_account_tag.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 https://sdkgen.app
 """
 
 import requests
 import sdkgen
 from requests import RequestException
 
-from backend_account_change_password import BackendAccountChangePassword
-from backend_user import BackendUser
-from backend_user_update import BackendUserUpdate
-from common_message import CommonMessage
-from common_message_exception import CommonMessageException
+from .backend_account_change_password import BackendAccountChangePassword
+from .backend_user import BackendUser
+from .backend_user_update import BackendUserUpdate
+from .common_message import CommonMessage
+from .common_message_exception import CommonMessageException
 
 class BackendAccountTag(sdkgen.TagAbstract):
     def __init__(self, http_client: requests.Session, parser: sdkgen.Parser):
         super().__init__(http_client, parser)
 
     pass
```

### Comparing `fusio-sdk-5.0.3/src/sdk/backend_action.py` & `fusio-sdk-5.0.4/src/sdk/backend_action.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """
 backend_action automatically generated by SDKgen please do not edit this file manually
 https://sdkgen.app
 """
 
 from dataclasses import dataclass, field
 from dataclasses_json import dataclass_json, config
-from backend_action_config import BackendActionConfig
-from common_metadata import CommonMetadata
+from .backend_action_config import BackendActionConfig
+from .common_metadata import CommonMetadata
 @dataclass_json
 @dataclass
 class BackendAction:
     id: int = field(default=None, metadata=config(field_name="id"))
     status: int = field(default=None, metadata=config(field_name="status"))
     name: str = field(default=None, metadata=config(field_name="name"))
     _class: str = field(default=None, metadata=config(field_name="class"))
```

### Comparing `fusio-sdk-5.0.3/src/sdk/backend_action_execute_request.py` & `fusio-sdk-5.0.4/src/sdk/backend_action_execute_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 backend_action_execute_request automatically generated by SDKgen please do not edit this file manually
 https://sdkgen.app
 """
 
 from dataclasses import dataclass, field
 from dataclasses_json import dataclass_json, config
-from backend_action_execute_request_body import BackendActionExecuteRequestBody
+from .backend_action_execute_request_body import BackendActionExecuteRequestBody
 @dataclass_json
 @dataclass
 class BackendActionExecuteRequest:
     method: str = field(default=None, metadata=config(field_name="method"))
     uri_fragments: str = field(default=None, metadata=config(field_name="uriFragments"))
     parameters: str = field(default=None, metadata=config(field_name="parameters"))
     headers: str = field(default=None, metadata=config(field_name="headers"))
```

### Comparing `fusio-sdk-5.0.3/src/sdk/backend_action_execute_response.py` & `fusio-sdk-5.0.4/src/sdk/backend_action_execute_response.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 backend_action_execute_response automatically generated by SDKgen please do not edit this file manually
 https://sdkgen.app
 """
 
 from dataclasses import dataclass, field
 from dataclasses_json import dataclass_json, config
-from backend_action_execute_response_headers import BackendActionExecuteResponseHeaders
-from backend_action_execute_response_body import BackendActionExecuteResponseBody
+from .backend_action_execute_response_headers import BackendActionExecuteResponseHeaders
+from .backend_action_execute_response_body import BackendActionExecuteResponseBody
 @dataclass_json
 @dataclass
 class BackendActionExecuteResponse:
     status_code: int = field(default=None, metadata=config(field_name="statusCode"))
     headers: BackendActionExecuteResponseHeaders = field(default=None, metadata=config(field_name="headers"))
     body: BackendActionExecuteResponseBody = field(default=None, metadata=config(field_name="body"))
```

### Comparing `fusio-sdk-5.0.3/src/sdk/backend_action_tag.py` & `fusio-sdk-5.0.4/src/sdk/backend_action_tag.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,24 +3,24 @@
 https://sdkgen.app
 """
 
 import requests
 import sdkgen
 from requests import RequestException
 
-from backend_action import BackendAction
-from backend_action_collection import BackendActionCollection
-from backend_action_create import BackendActionCreate
-from backend_action_execute_request import BackendActionExecuteRequest
-from backend_action_execute_response import BackendActionExecuteResponse
-from backend_action_index import BackendActionIndex
-from backend_action_update import BackendActionUpdate
-from common_form_container import CommonFormContainer
-from common_message import CommonMessage
-from common_message_exception import CommonMessageException
+from .backend_action import BackendAction
+from .backend_action_collection import BackendActionCollection
+from .backend_action_create import BackendActionCreate
+from .backend_action_execute_request import BackendActionExecuteRequest
+from .backend_action_execute_response import BackendActionExecuteResponse
+from .backend_action_index import BackendActionIndex
+from .backend_action_update import BackendActionUpdate
+from .common_form_container import CommonFormContainer
+from .common_message import CommonMessage
+from .common_message_exception import CommonMessageException
 
 class BackendActionTag(sdkgen.TagAbstract):
     def __init__(self, http_client: requests.Session, parser: sdkgen.Parser):
         super().__init__(http_client, parser)
 
     pass
```

### Comparing `fusio-sdk-5.0.3/src/sdk/backend_app.py` & `fusio-sdk-5.0.4/src/sdk/backend_app.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 backend_app automatically generated by SDKgen please do not edit this file manually
 https://sdkgen.app
 """
 
 from dataclasses import dataclass, field
 from dataclasses_json import dataclass_json, config
 from typing import List
-from common_metadata import CommonMetadata
-from backend_token import BackendToken
+from .common_metadata import CommonMetadata
+from .backend_token import BackendToken
 @dataclass_json
 @dataclass
 class BackendApp:
     id: int = field(default=None, metadata=config(field_name="id"))
     user_id: int = field(default=None, metadata=config(field_name="userId"))
     status: int = field(default=None, metadata=config(field_name="status"))
     name: str = field(default=None, metadata=config(field_name="name"))
```

### Comparing `fusio-sdk-5.0.3/src/sdk/backend_app_tag.py` & `fusio-sdk-5.0.4/src/sdk/backend_app_tag.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,20 +3,20 @@
 https://sdkgen.app
 """
 
 import requests
 import sdkgen
 from requests import RequestException
 
-from backend_app import BackendApp
-from backend_app_collection import BackendAppCollection
-from backend_app_create import BackendAppCreate
-from backend_app_update import BackendAppUpdate
-from common_message import CommonMessage
-from common_message_exception import CommonMessageException
+from .backend_app import BackendApp
+from .backend_app_collection import BackendAppCollection
+from .backend_app_create import BackendAppCreate
+from .backend_app_update import BackendAppUpdate
+from .common_message import CommonMessage
+from .common_message_exception import CommonMessageException
 
 class BackendAppTag(sdkgen.TagAbstract):
     def __init__(self, http_client: requests.Session, parser: sdkgen.Parser):
         super().__init__(http_client, parser)
 
     pass
```

### Comparing `fusio-sdk-5.0.3/src/sdk/backend_audit.py` & `fusio-sdk-5.0.4/src/sdk/backend_log.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 """
-backend_audit automatically generated by SDKgen please do not edit this file manually
+backend_log automatically generated by SDKgen please do not edit this file manually
 https://sdkgen.app
 """
 
 from dataclasses import dataclass, field
 from dataclasses_json import dataclass_json, config
-from backend_app import BackendApp
-from backend_user import BackendUser
-from backend_audit_object import BackendAuditObject
+from typing import List
+from .backend_log_error import BackendLogError
 @dataclass_json
 @dataclass
-class BackendAudit:
+class BackendLog:
     id: int = field(default=None, metadata=config(field_name="id"))
-    app: BackendApp = field(default=None, metadata=config(field_name="app"))
-    user: BackendUser = field(default=None, metadata=config(field_name="user"))
-    event: str = field(default=None, metadata=config(field_name="event"))
     ip: str = field(default=None, metadata=config(field_name="ip"))
-    message: str = field(default=None, metadata=config(field_name="message"))
-    content: BackendAuditObject = field(default=None, metadata=config(field_name="content"))
+    user_agent: str = field(default=None, metadata=config(field_name="userAgent"))
+    method: str = field(default=None, metadata=config(field_name="method"))
+    path: str = field(default=None, metadata=config(field_name="path"))
+    header: str = field(default=None, metadata=config(field_name="header"))
+    body: str = field(default=None, metadata=config(field_name="body"))
     date: datetime.datetime = field(default=None, metadata=config(field_name="date"))
+    errors: List[BackendLogError] = field(default=None, metadata=config(field_name="errors"))
```

### Comparing `fusio-sdk-5.0.3/src/sdk/backend_audit_tag.py` & `fusio-sdk-5.0.4/src/sdk/backend_audit_tag.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 https://sdkgen.app
 """
 
 import requests
 import sdkgen
 from requests import RequestException
 
-from backend_audit import BackendAudit
-from backend_audit_collection import BackendAuditCollection
-from common_message_exception import CommonMessageException
+from .backend_audit import BackendAudit
+from .backend_audit_collection import BackendAuditCollection
+from .common_message_exception import CommonMessageException
 
 class BackendAuditTag(sdkgen.TagAbstract):
     def __init__(self, http_client: requests.Session, parser: sdkgen.Parser):
         super().__init__(http_client, parser)
 
     pass
```

### Comparing `fusio-sdk-5.0.3/src/sdk/backend_category_tag.py` & `fusio-sdk-5.0.4/src/sdk/backend_category_tag.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,20 +3,20 @@
 https://sdkgen.app
 """
 
 import requests
 import sdkgen
 from requests import RequestException
 
-from backend_category import BackendCategory
-from backend_category_collection import BackendCategoryCollection
-from backend_category_create import BackendCategoryCreate
-from backend_category_update import BackendCategoryUpdate
-from common_message import CommonMessage
-from common_message_exception import CommonMessageException
+from .backend_category import BackendCategory
+from .backend_category_collection import BackendCategoryCollection
+from .backend_category_create import BackendCategoryCreate
+from .backend_category_update import BackendCategoryUpdate
+from .common_message import CommonMessage
+from .common_message_exception import CommonMessageException
 
 class BackendCategoryTag(sdkgen.TagAbstract):
     def __init__(self, http_client: requests.Session, parser: sdkgen.Parser):
         super().__init__(http_client, parser)
 
     pass
```

### Comparing `fusio-sdk-5.0.3/src/sdk/backend_config.py` & `fusio-sdk-5.0.4/src/sdk/backend_config.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.3/src/sdk/backend_config_tag.py` & `fusio-sdk-5.0.4/src/sdk/backend_config_tag.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 https://sdkgen.app
 """
 
 import requests
 import sdkgen
 from requests import RequestException
 
-from backend_config import BackendConfig
-from backend_config_collection import BackendConfigCollection
-from backend_config_update import BackendConfigUpdate
-from common_message import CommonMessage
-from common_message_exception import CommonMessageException
+from .backend_config import BackendConfig
+from .backend_config_collection import BackendConfigCollection
+from .backend_config_update import BackendConfigUpdate
+from .common_message import CommonMessage
+from .common_message_exception import CommonMessageException
 
 class BackendConfigTag(sdkgen.TagAbstract):
     def __init__(self, http_client: requests.Session, parser: sdkgen.Parser):
         super().__init__(http_client, parser)
 
     pass
```

### Comparing `fusio-sdk-5.0.3/src/sdk/backend_connection.py` & `fusio-sdk-5.0.4/src/sdk/backend_connection.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """
 backend_connection automatically generated by SDKgen please do not edit this file manually
 https://sdkgen.app
 """
 
 from dataclasses import dataclass, field
 from dataclasses_json import dataclass_json, config
-from backend_connection_config import BackendConnectionConfig
-from common_metadata import CommonMetadata
+from .backend_connection_config import BackendConnectionConfig
+from .common_metadata import CommonMetadata
 @dataclass_json
 @dataclass
 class BackendConnection:
     id: int = field(default=None, metadata=config(field_name="id"))
     name: str = field(default=None, metadata=config(field_name="name"))
     _class: str = field(default=None, metadata=config(field_name="class"))
     config: BackendConnectionConfig = field(default=None, metadata=config(field_name="config"))
```

### Comparing `fusio-sdk-5.0.3/src/sdk/backend_connection_introspection_entity.py` & `fusio-sdk-5.0.4/src/sdk/backend_connection_introspection_entity.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,14 @@
 backend_connection_introspection_entity automatically generated by SDKgen please do not edit this file manually
 https://sdkgen.app
 """
 
 from dataclasses import dataclass, field
 from dataclasses_json import dataclass_json, config
 from typing import List
-from backend_connection_introspection_entity_row import BackendConnectionIntrospectionEntityRow
+from .backend_connection_introspection_entity_row import BackendConnectionIntrospectionEntityRow
 @dataclass_json
 @dataclass
 class BackendConnectionIntrospectionEntity:
     name: str = field(default=None, metadata=config(field_name="name"))
     headers: List[str] = field(default=None, metadata=config(field_name="headers"))
     rows: List[BackendConnectionIntrospectionEntityRow] = field(default=None, metadata=config(field_name="rows"))
```

### Comparing `fusio-sdk-5.0.3/src/sdk/backend_connection_tag.py` & `fusio-sdk-5.0.4/src/sdk/backend_connection_tag.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,24 +3,24 @@
 https://sdkgen.app
 """
 
 import requests
 import sdkgen
 from requests import RequestException
 
-from backend_connection import BackendConnection
-from backend_connection_collection import BackendConnectionCollection
-from backend_connection_create import BackendConnectionCreate
-from backend_connection_index import BackendConnectionIndex
-from backend_connection_introspection_entities import BackendConnectionIntrospectionEntities
-from backend_connection_introspection_entity import BackendConnectionIntrospectionEntity
-from backend_connection_update import BackendConnectionUpdate
-from common_form_container import CommonFormContainer
-from common_message import CommonMessage
-from common_message_exception import CommonMessageException
+from .backend_connection import BackendConnection
+from .backend_connection_collection import BackendConnectionCollection
+from .backend_connection_create import BackendConnectionCreate
+from .backend_connection_index import BackendConnectionIndex
+from .backend_connection_introspection_entities import BackendConnectionIntrospectionEntities
+from .backend_connection_introspection_entity import BackendConnectionIntrospectionEntity
+from .backend_connection_update import BackendConnectionUpdate
+from .common_form_container import CommonFormContainer
+from .common_message import CommonMessage
+from .common_message_exception import CommonMessageException
 
 class BackendConnectionTag(sdkgen.TagAbstract):
     def __init__(self, http_client: requests.Session, parser: sdkgen.Parser):
         super().__init__(http_client, parser)
 
     pass
```

### Comparing `fusio-sdk-5.0.3/src/sdk/backend_cronjob.py` & `fusio-sdk-5.0.4/src/sdk/backend_cronjob.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 backend_cronjob automatically generated by SDKgen please do not edit this file manually
 https://sdkgen.app
 """
 
 from dataclasses import dataclass, field
 from dataclasses_json import dataclass_json, config
 from typing import List
-from common_metadata import CommonMetadata
-from backend_cronjob_error import BackendCronjobError
+from .common_metadata import CommonMetadata
+from .backend_cronjob_error import BackendCronjobError
 @dataclass_json
 @dataclass
 class BackendCronjob:
     id: int = field(default=None, metadata=config(field_name="id"))
     name: str = field(default=None, metadata=config(field_name="name"))
     cron: str = field(default=None, metadata=config(field_name="cron"))
     action: str = field(default=None, metadata=config(field_name="action"))
```

### Comparing `fusio-sdk-5.0.3/src/sdk/backend_cronjob_error.py` & `fusio-sdk-5.0.4/src/sdk/backend_cronjob_error.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.3/src/sdk/backend_cronjob_tag.py` & `fusio-sdk-5.0.4/src/sdk/backend_cronjob_tag.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,20 +3,20 @@
 https://sdkgen.app
 """
 
 import requests
 import sdkgen
 from requests import RequestException
 
-from backend_cronjob import BackendCronjob
-from backend_cronjob_collection import BackendCronjobCollection
-from backend_cronjob_create import BackendCronjobCreate
-from backend_cronjob_update import BackendCronjobUpdate
-from common_message import CommonMessage
-from common_message_exception import CommonMessageException
+from .backend_cronjob import BackendCronjob
+from .backend_cronjob_collection import BackendCronjobCollection
+from .backend_cronjob_create import BackendCronjobCreate
+from .backend_cronjob_update import BackendCronjobUpdate
+from .common_message import CommonMessage
+from .common_message_exception import CommonMessageException
 
 class BackendCronjobTag(sdkgen.TagAbstract):
     def __init__(self, http_client: requests.Session, parser: sdkgen.Parser):
         super().__init__(http_client, parser)
 
     pass
```

### Comparing `fusio-sdk-5.0.3/src/sdk/backend_dashboard.py` & `fusio-sdk-5.0.4/src/sdk/backend_dashboard.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 """
 backend_dashboard automatically generated by SDKgen please do not edit this file manually
 https://sdkgen.app
 """
 
 from dataclasses import dataclass, field
 from dataclasses_json import dataclass_json, config
-from backend_statistic_chart import BackendStatisticChart
-from backend_dashboard_apps import BackendDashboardApps
-from backend_dashboard_requests import BackendDashboardRequests
-from backend_dashboard_users import BackendDashboardUsers
-from backend_dashboard_transactions import BackendDashboardTransactions
+from .backend_statistic_chart import BackendStatisticChart
+from .backend_dashboard_apps import BackendDashboardApps
+from .backend_dashboard_requests import BackendDashboardRequests
+from .backend_dashboard_users import BackendDashboardUsers
+from .backend_dashboard_transactions import BackendDashboardTransactions
 @dataclass_json
 @dataclass
 class BackendDashboard:
     errors_per_operation: BackendStatisticChart = field(default=None, metadata=config(field_name="errorsPerOperation"))
     incoming_requests: BackendStatisticChart = field(default=None, metadata=config(field_name="incomingRequests"))
     incoming_transactions: BackendStatisticChart = field(default=None, metadata=config(field_name="incomingTransactions"))
     most_used_operations: BackendStatisticChart = field(default=None, metadata=config(field_name="mostUsedOperations"))
```

### Comparing `fusio-sdk-5.0.3/src/sdk/backend_dashboard_request.py` & `fusio-sdk-5.0.4/src/sdk/backend_dashboard_request.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.3/src/sdk/backend_dashboard_tag.py` & `fusio-sdk-5.0.4/src/sdk/backend_dashboard_tag.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 https://sdkgen.app
 """
 
 import requests
 import sdkgen
 from requests import RequestException
 
-from backend_dashboard import BackendDashboard
-from common_message_exception import CommonMessageException
+from .backend_dashboard import BackendDashboard
+from .common_message_exception import CommonMessageException
 
 class BackendDashboardTag(sdkgen.TagAbstract):
     def __init__(self, http_client: requests.Session, parser: sdkgen.Parser):
         super().__init__(http_client, parser)
 
     pass
```

### Comparing `fusio-sdk-5.0.3/src/sdk/backend_dashboard_transaction.py` & `fusio-sdk-5.0.4/src/sdk/backend_dashboard_transaction.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.3/src/sdk/backend_dashboard_user.py` & `fusio-sdk-5.0.4/src/sdk/backend_dashboard_user.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.3/src/sdk/backend_event.py` & `fusio-sdk-5.0.4/src/sdk/backend_event.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 backend_event automatically generated by SDKgen please do not edit this file manually
 https://sdkgen.app
 """
 
 from dataclasses import dataclass, field
 from dataclasses_json import dataclass_json, config
-from common_metadata import CommonMetadata
+from .common_metadata import CommonMetadata
 @dataclass_json
 @dataclass
 class BackendEvent:
     id: int = field(default=None, metadata=config(field_name="id"))
     name: str = field(default=None, metadata=config(field_name="name"))
     description: str = field(default=None, metadata=config(field_name="description"))
     schema: str = field(default=None, metadata=config(field_name="schema"))
```

### Comparing `fusio-sdk-5.0.3/src/sdk/backend_event_tag.py` & `fusio-sdk-5.0.4/src/sdk/backend_event_tag.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,20 +3,20 @@
 https://sdkgen.app
 """
 
 import requests
 import sdkgen
 from requests import RequestException
 
-from backend_event import BackendEvent
-from backend_event_collection import BackendEventCollection
-from backend_event_create import BackendEventCreate
-from backend_event_update import BackendEventUpdate
-from common_message import CommonMessage
-from common_message_exception import CommonMessageException
+from .backend_event import BackendEvent
+from .backend_event_collection import BackendEventCollection
+from .backend_event_create import BackendEventCreate
+from .backend_event_update import BackendEventUpdate
+from .common_message import CommonMessage
+from .common_message_exception import CommonMessageException
 
 class BackendEventTag(sdkgen.TagAbstract):
     def __init__(self, http_client: requests.Session, parser: sdkgen.Parser):
         super().__init__(http_client, parser)
 
     pass
```

### Comparing `fusio-sdk-5.0.3/src/sdk/backend_generator_provider.py` & `fusio-sdk-5.0.4/src/sdk/backend_generator_provider.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 backend_generator_provider automatically generated by SDKgen please do not edit this file manually
 https://sdkgen.app
 """
 
 from dataclasses import dataclass, field
 from dataclasses_json import dataclass_json, config
 from typing import List
-from backend_generator_provider_config import BackendGeneratorProviderConfig
+from .backend_generator_provider_config import BackendGeneratorProviderConfig
 @dataclass_json
 @dataclass
 class BackendGeneratorProvider:
     path: str = field(default=None, metadata=config(field_name="path"))
     scopes: List[str] = field(default=None, metadata=config(field_name="scopes"))
     public: bool = field(default=None, metadata=config(field_name="public"))
     config: BackendGeneratorProviderConfig = field(default=None, metadata=config(field_name="config"))
```

### Comparing `fusio-sdk-5.0.3/src/sdk/backend_generator_provider_changelog.py` & `fusio-sdk-5.0.4/src/sdk/backend_generator_provider_changelog.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 backend_generator_provider_changelog automatically generated by SDKgen please do not edit this file manually
 https://sdkgen.app
 """
 
 from dataclasses import dataclass, field
 from dataclasses_json import dataclass_json, config
 from typing import List
-from backend_schema import BackendSchema
-from backend_action import BackendAction
-from backend_operation import BackendOperation
+from .backend_schema import BackendSchema
+from .backend_action import BackendAction
+from .backend_operation import BackendOperation
 @dataclass_json
 @dataclass
 class BackendGeneratorProviderChangelog:
     schemas: List[BackendSchema] = field(default=None, metadata=config(field_name="schemas"))
     actions: List[BackendAction] = field(default=None, metadata=config(field_name="actions"))
     operations: List[BackendOperation] = field(default=None, metadata=config(field_name="operations"))
```

### Comparing `fusio-sdk-5.0.3/src/sdk/backend_generator_tag.py` & `fusio-sdk-5.0.4/src/sdk/backend_generator_tag.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,21 +3,21 @@
 https://sdkgen.app
 """
 
 import requests
 import sdkgen
 from requests import RequestException
 
-from backend_generator_index_providers import BackendGeneratorIndexProviders
-from backend_generator_provider import BackendGeneratorProvider
-from backend_generator_provider_changelog import BackendGeneratorProviderChangelog
-from backend_generator_provider_config import BackendGeneratorProviderConfig
-from common_form_container import CommonFormContainer
-from common_message import CommonMessage
-from common_message_exception import CommonMessageException
+from .backend_generator_index_providers import BackendGeneratorIndexProviders
+from .backend_generator_provider import BackendGeneratorProvider
+from .backend_generator_provider_changelog import BackendGeneratorProviderChangelog
+from .backend_generator_provider_config import BackendGeneratorProviderConfig
+from .common_form_container import CommonFormContainer
+from .common_message import CommonMessage
+from .common_message_exception import CommonMessageException
 
 class BackendGeneratorTag(sdkgen.TagAbstract):
     def __init__(self, http_client: requests.Session, parser: sdkgen.Parser):
         super().__init__(http_client, parser)
 
     pass
```

### Comparing `fusio-sdk-5.0.3/src/sdk/backend_identity.py` & `fusio-sdk-5.0.4/src/sdk/backend_identity.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 backend_identity automatically generated by SDKgen please do not edit this file manually
 https://sdkgen.app
 """
 
 from dataclasses import dataclass, field
 from dataclasses_json import dataclass_json, config
-from backend_identity_config import BackendIdentityConfig
+from .backend_identity_config import BackendIdentityConfig
 @dataclass_json
 @dataclass
 class BackendIdentity:
     id: int = field(default=None, metadata=config(field_name="id"))
     app_id: int = field(default=None, metadata=config(field_name="appId"))
     role_id: int = field(default=None, metadata=config(field_name="roleId"))
     name: str = field(default=None, metadata=config(field_name="name"))
```

### Comparing `fusio-sdk-5.0.3/src/sdk/backend_identity_tag.py` & `fusio-sdk-5.0.4/src/sdk/backend_identity_tag.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 https://sdkgen.app
 """
 
 import requests
 import sdkgen
 from requests import RequestException
 
-from backend_identity import BackendIdentity
-from backend_identity_collection import BackendIdentityCollection
-from backend_identity_create import BackendIdentityCreate
-from backend_identity_index import BackendIdentityIndex
-from backend_identity_update import BackendIdentityUpdate
-from common_form_container import CommonFormContainer
-from common_message import CommonMessage
-from common_message_exception import CommonMessageException
+from .backend_identity import BackendIdentity
+from .backend_identity_collection import BackendIdentityCollection
+from .backend_identity_create import BackendIdentityCreate
+from .backend_identity_index import BackendIdentityIndex
+from .backend_identity_update import BackendIdentityUpdate
+from .common_form_container import CommonFormContainer
+from .common_message import CommonMessage
+from .common_message_exception import CommonMessageException
 
 class BackendIdentityTag(sdkgen.TagAbstract):
     def __init__(self, http_client: requests.Session, parser: sdkgen.Parser):
         super().__init__(http_client, parser)
 
     pass
```

### Comparing `fusio-sdk-5.0.3/src/sdk/backend_log.py` & `fusio-sdk-5.0.4/src/sdk/consumer_log.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 """
-backend_log automatically generated by SDKgen please do not edit this file manually
+consumer_log automatically generated by SDKgen please do not edit this file manually
 https://sdkgen.app
 """
 
 from dataclasses import dataclass, field
 from dataclasses_json import dataclass_json, config
-from typing import List
-from backend_log_error import BackendLogError
 @dataclass_json
 @dataclass
-class BackendLog:
+class ConsumerLog:
     id: int = field(default=None, metadata=config(field_name="id"))
+    app_id: int = field(default=None, metadata=config(field_name="appId"))
     ip: str = field(default=None, metadata=config(field_name="ip"))
     user_agent: str = field(default=None, metadata=config(field_name="userAgent"))
     method: str = field(default=None, metadata=config(field_name="method"))
     path: str = field(default=None, metadata=config(field_name="path"))
     header: str = field(default=None, metadata=config(field_name="header"))
     body: str = field(default=None, metadata=config(field_name="body"))
     date: datetime.datetime = field(default=None, metadata=config(field_name="date"))
-    errors: List[BackendLogError] = field(default=None, metadata=config(field_name="errors"))
```

### Comparing `fusio-sdk-5.0.3/src/sdk/backend_log_error.py` & `fusio-sdk-5.0.4/src/sdk/backend_log_error.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.3/src/sdk/backend_log_tag.py` & `fusio-sdk-5.0.4/src/sdk/backend_log_tag.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 https://sdkgen.app
 """
 
 import requests
 import sdkgen
 from requests import RequestException
 
-from backend_log import BackendLog
-from backend_log_collection import BackendLogCollection
-from backend_log_error import BackendLogError
-from backend_log_error_collection import BackendLogErrorCollection
-from common_message_exception import CommonMessageException
+from .backend_log import BackendLog
+from .backend_log_collection import BackendLogCollection
+from .backend_log_error import BackendLogError
+from .backend_log_error_collection import BackendLogErrorCollection
+from .common_message_exception import CommonMessageException
 
 class BackendLogTag(sdkgen.TagAbstract):
     def __init__(self, http_client: requests.Session, parser: sdkgen.Parser):
         super().__init__(http_client, parser)
 
     pass
```

### Comparing `fusio-sdk-5.0.3/src/sdk/backend_marketplace_app.py` & `fusio-sdk-5.0.4/src/sdk/backend_marketplace_app.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.3/src/sdk/backend_marketplace_tag.py` & `fusio-sdk-5.0.4/src/sdk/backend_marketplace_tag.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 https://sdkgen.app
 """
 
 import requests
 import sdkgen
 from requests import RequestException
 
-from backend_marketplace_collection import BackendMarketplaceCollection
-from backend_marketplace_install import BackendMarketplaceInstall
-from backend_marketplace_local_app import BackendMarketplaceLocalApp
-from common_message import CommonMessage
-from common_message_exception import CommonMessageException
+from .backend_marketplace_collection import BackendMarketplaceCollection
+from .backend_marketplace_install import BackendMarketplaceInstall
+from .backend_marketplace_local_app import BackendMarketplaceLocalApp
+from .common_message import CommonMessage
+from .common_message_exception import CommonMessageException
 
 class BackendMarketplaceTag(sdkgen.TagAbstract):
     def __init__(self, http_client: requests.Session, parser: sdkgen.Parser):
         super().__init__(http_client, parser)
 
     pass
```

### Comparing `fusio-sdk-5.0.3/src/sdk/backend_operation.py` & `fusio-sdk-5.0.4/src/sdk/backend_operation.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 backend_operation automatically generated by SDKgen please do not edit this file manually
 https://sdkgen.app
 """
 
 from dataclasses import dataclass, field
 from dataclasses_json import dataclass_json, config
 from typing import List
-from backend_operation_parameters import BackendOperationParameters
-from backend_operation_throws import BackendOperationThrows
-from common_metadata import CommonMetadata
+from .backend_operation_parameters import BackendOperationParameters
+from .backend_operation_throws import BackendOperationThrows
+from .common_metadata import CommonMetadata
 @dataclass_json
 @dataclass
 class BackendOperation:
     id: int = field(default=None, metadata=config(field_name="id"))
     status: int = field(default=None, metadata=config(field_name="status"))
     active: bool = field(default=None, metadata=config(field_name="active"))
     public: bool = field(default=None, metadata=config(field_name="public"))
```

### Comparing `fusio-sdk-5.0.3/src/sdk/backend_operation_schema.py` & `fusio-sdk-5.0.4/src/sdk/backend_operation_schema.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.3/src/sdk/backend_operation_tag.py` & `fusio-sdk-5.0.4/src/sdk/backend_operation_tag.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,20 +3,20 @@
 https://sdkgen.app
 """
 
 import requests
 import sdkgen
 from requests import RequestException
 
-from backend_operation import BackendOperation
-from backend_operation_collection import BackendOperationCollection
-from backend_operation_create import BackendOperationCreate
-from backend_operation_update import BackendOperationUpdate
-from common_message import CommonMessage
-from common_message_exception import CommonMessageException
+from .backend_operation import BackendOperation
+from .backend_operation_collection import BackendOperationCollection
+from .backend_operation_create import BackendOperationCreate
+from .backend_operation_update import BackendOperationUpdate
+from .common_message import CommonMessage
+from .common_message_exception import CommonMessageException
 
 class BackendOperationTag(sdkgen.TagAbstract):
     def __init__(self, http_client: requests.Session, parser: sdkgen.Parser):
         super().__init__(http_client, parser)
 
     pass
```

### Comparing `fusio-sdk-5.0.3/src/sdk/backend_page.py` & `fusio-sdk-5.0.4/src/sdk/backend_page.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 backend_page automatically generated by SDKgen please do not edit this file manually
 https://sdkgen.app
 """
 
 from dataclasses import dataclass, field
 from dataclasses_json import dataclass_json, config
-from common_metadata import CommonMetadata
+from .common_metadata import CommonMetadata
 @dataclass_json
 @dataclass
 class BackendPage:
     id: int = field(default=None, metadata=config(field_name="id"))
     status: int = field(default=None, metadata=config(field_name="status"))
     title: str = field(default=None, metadata=config(field_name="title"))
     slug: str = field(default=None, metadata=config(field_name="slug"))
```

### Comparing `fusio-sdk-5.0.3/src/sdk/backend_page_tag.py` & `fusio-sdk-5.0.4/src/sdk/backend_page_tag.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,20 +3,20 @@
 https://sdkgen.app
 """
 
 import requests
 import sdkgen
 from requests import RequestException
 
-from backend_page import BackendPage
-from backend_page_collection import BackendPageCollection
-from backend_page_create import BackendPageCreate
-from backend_page_update import BackendPageUpdate
-from common_message import CommonMessage
-from common_message_exception import CommonMessageException
+from .backend_page import BackendPage
+from .backend_page_collection import BackendPageCollection
+from .backend_page_create import BackendPageCreate
+from .backend_page_update import BackendPageUpdate
+from .common_message import CommonMessage
+from .common_message_exception import CommonMessageException
 
 class BackendPageTag(sdkgen.TagAbstract):
     def __init__(self, http_client: requests.Session, parser: sdkgen.Parser):
         super().__init__(http_client, parser)
 
     pass
```

### Comparing `fusio-sdk-5.0.3/src/sdk/backend_plan.py` & `fusio-sdk-5.0.4/src/sdk/backend_plan.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 backend_plan automatically generated by SDKgen please do not edit this file manually
 https://sdkgen.app
 """
 
 from dataclasses import dataclass, field
 from dataclasses_json import dataclass_json, config
 from typing import List
-from common_metadata import CommonMetadata
+from .common_metadata import CommonMetadata
 @dataclass_json
 @dataclass
 class BackendPlan:
     id: int = field(default=None, metadata=config(field_name="id"))
     name: str = field(default=None, metadata=config(field_name="name"))
     description: str = field(default=None, metadata=config(field_name="description"))
     price: float = field(default=None, metadata=config(field_name="price"))
```

### Comparing `fusio-sdk-5.0.3/src/sdk/backend_plan_tag.py` & `fusio-sdk-5.0.4/src/sdk/backend_plan_tag.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,20 +3,20 @@
 https://sdkgen.app
 """
 
 import requests
 import sdkgen
 from requests import RequestException
 
-from backend_plan import BackendPlan
-from backend_plan_collection import BackendPlanCollection
-from backend_plan_create import BackendPlanCreate
-from backend_plan_update import BackendPlanUpdate
-from common_message import CommonMessage
-from common_message_exception import CommonMessageException
+from .backend_plan import BackendPlan
+from .backend_plan_collection import BackendPlanCollection
+from .backend_plan_create import BackendPlanCreate
+from .backend_plan_update import BackendPlanUpdate
+from .common_message import CommonMessage
+from .common_message_exception import CommonMessageException
 
 class BackendPlanTag(sdkgen.TagAbstract):
     def __init__(self, http_client: requests.Session, parser: sdkgen.Parser):
         super().__init__(http_client, parser)
 
     pass
```

### Comparing `fusio-sdk-5.0.3/src/sdk/backend_rate.py` & `fusio-sdk-5.0.4/src/sdk/backend_rate.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 backend_rate automatically generated by SDKgen please do not edit this file manually
 https://sdkgen.app
 """
 
 from dataclasses import dataclass, field
 from dataclasses_json import dataclass_json, config
 from typing import List
-from backend_rate_allocation import BackendRateAllocation
-from common_metadata import CommonMetadata
+from .backend_rate_allocation import BackendRateAllocation
+from .common_metadata import CommonMetadata
 @dataclass_json
 @dataclass
 class BackendRate:
     id: int = field(default=None, metadata=config(field_name="id"))
     priority: int = field(default=None, metadata=config(field_name="priority"))
     name: str = field(default=None, metadata=config(field_name="name"))
     rate_limit: int = field(default=None, metadata=config(field_name="rateLimit"))
```

### Comparing `fusio-sdk-5.0.3/src/sdk/backend_rate_allocation.py` & `fusio-sdk-5.0.4/src/sdk/backend_rate_allocation.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.3/src/sdk/backend_rate_tag.py` & `fusio-sdk-5.0.4/src/sdk/backend_rate_tag.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,20 +3,20 @@
 https://sdkgen.app
 """
 
 import requests
 import sdkgen
 from requests import RequestException
 
-from backend_rate import BackendRate
-from backend_rate_collection import BackendRateCollection
-from backend_rate_create import BackendRateCreate
-from backend_rate_update import BackendRateUpdate
-from common_message import CommonMessage
-from common_message_exception import CommonMessageException
+from .backend_rate import BackendRate
+from .backend_rate_collection import BackendRateCollection
+from .backend_rate_create import BackendRateCreate
+from .backend_rate_update import BackendRateUpdate
+from .common_message import CommonMessage
+from .common_message_exception import CommonMessageException
 
 class BackendRateTag(sdkgen.TagAbstract):
     def __init__(self, http_client: requests.Session, parser: sdkgen.Parser):
         super().__init__(http_client, parser)
 
     pass
```

### Comparing `fusio-sdk-5.0.3/src/sdk/backend_role.py` & `fusio-sdk-5.0.4/src/sdk/backend_role.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.3/src/sdk/backend_role_tag.py` & `fusio-sdk-5.0.4/src/sdk/backend_role_tag.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,20 +3,20 @@
 https://sdkgen.app
 """
 
 import requests
 import sdkgen
 from requests import RequestException
 
-from backend_role import BackendRole
-from backend_role_collection import BackendRoleCollection
-from backend_role_create import BackendRoleCreate
-from backend_role_update import BackendRoleUpdate
-from common_message import CommonMessage
-from common_message_exception import CommonMessageException
+from .backend_role import BackendRole
+from .backend_role_collection import BackendRoleCollection
+from .backend_role_create import BackendRoleCreate
+from .backend_role_update import BackendRoleUpdate
+from .common_message import CommonMessage
+from .common_message_exception import CommonMessageException
 
 class BackendRoleTag(sdkgen.TagAbstract):
     def __init__(self, http_client: requests.Session, parser: sdkgen.Parser):
         super().__init__(http_client, parser)
 
     pass
```

### Comparing `fusio-sdk-5.0.3/src/sdk/backend_schema.py` & `fusio-sdk-5.0.4/src/sdk/backend_schema.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """
 backend_schema automatically generated by SDKgen please do not edit this file manually
 https://sdkgen.app
 """
 
 from dataclasses import dataclass, field
 from dataclasses_json import dataclass_json, config
-from backend_schema_source import BackendSchemaSource
-from backend_schema_form import BackendSchemaForm
-from common_metadata import CommonMetadata
+from .backend_schema_source import BackendSchemaSource
+from .backend_schema_form import BackendSchemaForm
+from .common_metadata import CommonMetadata
 @dataclass_json
 @dataclass
 class BackendSchema:
     id: int = field(default=None, metadata=config(field_name="id"))
     status: int = field(default=None, metadata=config(field_name="status"))
     name: str = field(default=None, metadata=config(field_name="name"))
     source: BackendSchemaSource = field(default=None, metadata=config(field_name="source"))
```

### Comparing `fusio-sdk-5.0.3/src/sdk/backend_schema_tag.py` & `fusio-sdk-5.0.4/src/sdk/backend_schema_tag.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 https://sdkgen.app
 """
 
 import requests
 import sdkgen
 from requests import RequestException
 
-from backend_schema import BackendSchema
-from backend_schema_collection import BackendSchemaCollection
-from backend_schema_create import BackendSchemaCreate
-from backend_schema_form import BackendSchemaForm
-from backend_schema_preview_response import BackendSchemaPreviewResponse
-from backend_schema_update import BackendSchemaUpdate
-from common_message import CommonMessage
-from common_message_exception import CommonMessageException
+from .backend_schema import BackendSchema
+from .backend_schema_collection import BackendSchemaCollection
+from .backend_schema_create import BackendSchemaCreate
+from .backend_schema_form import BackendSchemaForm
+from .backend_schema_preview_response import BackendSchemaPreviewResponse
+from .backend_schema_update import BackendSchemaUpdate
+from .common_message import CommonMessage
+from .common_message_exception import CommonMessageException
 
 class BackendSchemaTag(sdkgen.TagAbstract):
     def __init__(self, http_client: requests.Session, parser: sdkgen.Parser):
         super().__init__(http_client, parser)
 
     pass
```

### Comparing `fusio-sdk-5.0.3/src/sdk/backend_scope.py` & `fusio-sdk-5.0.4/src/sdk/backend_scope.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 backend_scope automatically generated by SDKgen please do not edit this file manually
 https://sdkgen.app
 """
 
 from dataclasses import dataclass, field
 from dataclasses_json import dataclass_json, config
 from typing import List
-from backend_scope_operation import BackendScopeOperation
-from common_metadata import CommonMetadata
+from .backend_scope_operation import BackendScopeOperation
+from .common_metadata import CommonMetadata
 @dataclass_json
 @dataclass
 class BackendScope:
     id: int = field(default=None, metadata=config(field_name="id"))
     name: str = field(default=None, metadata=config(field_name="name"))
     description: str = field(default=None, metadata=config(field_name="description"))
     operations: List[BackendScopeOperation] = field(default=None, metadata=config(field_name="operations"))
```

### Comparing `fusio-sdk-5.0.3/src/sdk/backend_scope_category.py` & `fusio-sdk-5.0.4/src/sdk/backend_scope_category.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,14 @@
 backend_scope_category automatically generated by SDKgen please do not edit this file manually
 https://sdkgen.app
 """
 
 from dataclasses import dataclass, field
 from dataclasses_json import dataclass_json, config
 from typing import List
-from backend_scope_category_scope import BackendScopeCategoryScope
+from .backend_scope_category_scope import BackendScopeCategoryScope
 @dataclass_json
 @dataclass
 class BackendScopeCategory:
     id: int = field(default=None, metadata=config(field_name="id"))
     name: str = field(default=None, metadata=config(field_name="name"))
     scopes: List[BackendScopeCategoryScope] = field(default=None, metadata=config(field_name="scopes"))
```

### Comparing `fusio-sdk-5.0.3/src/sdk/backend_scope_tag.py` & `fusio-sdk-5.0.4/src/sdk/backend_scope_tag.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,21 +3,21 @@
 https://sdkgen.app
 """
 
 import requests
 import sdkgen
 from requests import RequestException
 
-from backend_scope import BackendScope
-from backend_scope_categories import BackendScopeCategories
-from backend_scope_collection import BackendScopeCollection
-from backend_scope_create import BackendScopeCreate
-from backend_scope_update import BackendScopeUpdate
-from common_message import CommonMessage
-from common_message_exception import CommonMessageException
+from .backend_scope import BackendScope
+from .backend_scope_categories import BackendScopeCategories
+from .backend_scope_collection import BackendScopeCollection
+from .backend_scope_create import BackendScopeCreate
+from .backend_scope_update import BackendScopeUpdate
+from .common_message import CommonMessage
+from .common_message_exception import CommonMessageException
 
 class BackendScopeTag(sdkgen.TagAbstract):
     def __init__(self, http_client: requests.Session, parser: sdkgen.Parser):
         super().__init__(http_client, parser)
 
     pass
```

### Comparing `fusio-sdk-5.0.3/src/sdk/backend_sdk_tag.py` & `fusio-sdk-5.0.4/src/sdk/backend_sdk_tag.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 https://sdkgen.app
 """
 
 import requests
 import sdkgen
 from requests import RequestException
 
-from backend_sdk_generate import BackendSdkGenerate
-from backend_sdk_response import BackendSdkResponse
-from common_message import CommonMessage
-from common_message_exception import CommonMessageException
+from .backend_sdk_generate import BackendSdkGenerate
+from .backend_sdk_response import BackendSdkResponse
+from .common_message import CommonMessage
+from .common_message_exception import CommonMessageException
 
 class BackendSdkTag(sdkgen.TagAbstract):
     def __init__(self, http_client: requests.Session, parser: sdkgen.Parser):
         super().__init__(http_client, parser)
 
     pass
```

### Comparing `fusio-sdk-5.0.3/src/sdk/backend_statistic_chart.py` & `fusio-sdk-5.0.4/src/sdk/backend_statistic_chart.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,14 @@
 backend_statistic_chart automatically generated by SDKgen please do not edit this file manually
 https://sdkgen.app
 """
 
 from dataclasses import dataclass, field
 from dataclasses_json import dataclass_json, config
 from typing import List
-from backend_statistic_chart_data import BackendStatisticChartData
+from .backend_statistic_chart_data import BackendStatisticChartData
 @dataclass_json
 @dataclass
 class BackendStatisticChart:
     labels: List[str] = field(default=None, metadata=config(field_name="labels"))
     data: List[BackendStatisticChartData] = field(default=None, metadata=config(field_name="data"))
     series: List[str] = field(default=None, metadata=config(field_name="series"))
```

### Comparing `fusio-sdk-5.0.3/src/sdk/backend_statistic_count.py` & `fusio-sdk-5.0.4/src/sdk/backend_statistic_count.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.3/src/sdk/backend_statistic_tag.py` & `fusio-sdk-5.0.4/src/sdk/backend_statistic_tag.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 https://sdkgen.app
 """
 
 import requests
 import sdkgen
 from requests import RequestException
 
-from backend_statistic_chart import BackendStatisticChart
-from backend_statistic_count import BackendStatisticCount
-from common_message_exception import CommonMessageException
+from .backend_statistic_chart import BackendStatisticChart
+from .backend_statistic_count import BackendStatisticCount
+from .common_message_exception import CommonMessageException
 
 class BackendStatisticTag(sdkgen.TagAbstract):
     def __init__(self, http_client: requests.Session, parser: sdkgen.Parser):
         super().__init__(http_client, parser)
 
     pass
```

### Comparing `fusio-sdk-5.0.3/src/sdk/backend_tag.py` & `fusio-sdk-5.0.4/src/sdk/backend_tag.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,43 +3,43 @@
 https://sdkgen.app
 """
 
 import requests
 import sdkgen
 from requests import RequestException
 
-from backend_account_tag import BackendAccountTag
-from backend_action_tag import BackendActionTag
-from backend_app_tag import BackendAppTag
-from backend_audit_tag import BackendAuditTag
-from backend_category_tag import BackendCategoryTag
-from backend_config_tag import BackendConfigTag
-from backend_connection_tag import BackendConnectionTag
-from backend_cronjob_tag import BackendCronjobTag
-from backend_dashboard_tag import BackendDashboardTag
-from backend_event_tag import BackendEventTag
-from backend_generator_tag import BackendGeneratorTag
-from backend_identity_tag import BackendIdentityTag
-from backend_log_tag import BackendLogTag
-from backend_marketplace_tag import BackendMarketplaceTag
-from backend_operation_tag import BackendOperationTag
-from backend_page_tag import BackendPageTag
-from backend_plan_tag import BackendPlanTag
-from backend_rate_tag import BackendRateTag
-from backend_role_tag import BackendRoleTag
-from backend_schema_tag import BackendSchemaTag
-from backend_scope_tag import BackendScopeTag
-from backend_sdk_tag import BackendSdkTag
-from backend_statistic_tag import BackendStatisticTag
-from backend_tenant_tag import BackendTenantTag
-from backend_token_tag import BackendTokenTag
-from backend_transaction_tag import BackendTransactionTag
-from backend_trash_tag import BackendTrashTag
-from backend_user_tag import BackendUserTag
-from backend_webhook_tag import BackendWebhookTag
+from .backend_account_tag import BackendAccountTag
+from .backend_action_tag import BackendActionTag
+from .backend_app_tag import BackendAppTag
+from .backend_audit_tag import BackendAuditTag
+from .backend_category_tag import BackendCategoryTag
+from .backend_config_tag import BackendConfigTag
+from .backend_connection_tag import BackendConnectionTag
+from .backend_cronjob_tag import BackendCronjobTag
+from .backend_dashboard_tag import BackendDashboardTag
+from .backend_event_tag import BackendEventTag
+from .backend_generator_tag import BackendGeneratorTag
+from .backend_identity_tag import BackendIdentityTag
+from .backend_log_tag import BackendLogTag
+from .backend_marketplace_tag import BackendMarketplaceTag
+from .backend_operation_tag import BackendOperationTag
+from .backend_page_tag import BackendPageTag
+from .backend_plan_tag import BackendPlanTag
+from .backend_rate_tag import BackendRateTag
+from .backend_role_tag import BackendRoleTag
+from .backend_schema_tag import BackendSchemaTag
+from .backend_scope_tag import BackendScopeTag
+from .backend_sdk_tag import BackendSdkTag
+from .backend_statistic_tag import BackendStatisticTag
+from .backend_tenant_tag import BackendTenantTag
+from .backend_token_tag import BackendTokenTag
+from .backend_transaction_tag import BackendTransactionTag
+from .backend_trash_tag import BackendTrashTag
+from .backend_user_tag import BackendUserTag
+from .backend_webhook_tag import BackendWebhookTag
 
 class BackendTag(sdkgen.TagAbstract):
     def __init__(self, http_client: requests.Session, parser: sdkgen.Parser):
         super().__init__(http_client, parser)
 
     pass
```

### Comparing `fusio-sdk-5.0.3/src/sdk/backend_tenant_tag.py` & `fusio-sdk-5.0.4/src/sdk/backend_tenant_tag.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 https://sdkgen.app
 """
 
 import requests
 import sdkgen
 from requests import RequestException
 
-from common_message import CommonMessage
-from common_message_exception import CommonMessageException
+from .common_message import CommonMessage
+from .common_message_exception import CommonMessageException
 
 class BackendTenantTag(sdkgen.TagAbstract):
     def __init__(self, http_client: requests.Session, parser: sdkgen.Parser):
         super().__init__(http_client, parser)
 
     pass
```

### Comparing `fusio-sdk-5.0.3/src/sdk/backend_token.py` & `fusio-sdk-5.0.4/src/sdk/backend_token.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.3/src/sdk/backend_token_tag.py` & `fusio-sdk-5.0.4/src/sdk/backend_token_tag.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 https://sdkgen.app
 """
 
 import requests
 import sdkgen
 from requests import RequestException
 
-from backend_token import BackendToken
-from backend_token_collection import BackendTokenCollection
-from common_message_exception import CommonMessageException
+from .backend_token import BackendToken
+from .backend_token_collection import BackendTokenCollection
+from .common_message_exception import CommonMessageException
 
 class BackendTokenTag(sdkgen.TagAbstract):
     def __init__(self, http_client: requests.Session, parser: sdkgen.Parser):
         super().__init__(http_client, parser)
 
     pass
```

### Comparing `fusio-sdk-5.0.3/src/sdk/backend_transaction.py` & `fusio-sdk-5.0.4/src/sdk/backend_transaction.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.3/src/sdk/backend_transaction_tag.py` & `fusio-sdk-5.0.4/src/sdk/backend_transaction_tag.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 https://sdkgen.app
 """
 
 import requests
 import sdkgen
 from requests import RequestException
 
-from backend_transaction import BackendTransaction
-from backend_transaction_collection import BackendTransactionCollection
-from common_message_exception import CommonMessageException
+from .backend_transaction import BackendTransaction
+from .backend_transaction_collection import BackendTransactionCollection
+from .common_message_exception import CommonMessageException
 
 class BackendTransactionTag(sdkgen.TagAbstract):
     def __init__(self, http_client: requests.Session, parser: sdkgen.Parser):
         super().__init__(http_client, parser)
 
     pass
```

### Comparing `fusio-sdk-5.0.3/src/sdk/backend_trash_tag.py` & `fusio-sdk-5.0.4/src/sdk/backend_trash_tag.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 https://sdkgen.app
 """
 
 import requests
 import sdkgen
 from requests import RequestException
 
-from backend_trash_data_collection import BackendTrashDataCollection
-from backend_trash_restore import BackendTrashRestore
-from backend_trash_types import BackendTrashTypes
-from common_message import CommonMessage
-from common_message_exception import CommonMessageException
+from .backend_trash_data_collection import BackendTrashDataCollection
+from .backend_trash_restore import BackendTrashRestore
+from .backend_trash_types import BackendTrashTypes
+from .common_message import CommonMessage
+from .common_message_exception import CommonMessageException
 
 class BackendTrashTag(sdkgen.TagAbstract):
     def __init__(self, http_client: requests.Session, parser: sdkgen.Parser):
         super().__init__(http_client, parser)
 
     pass
```

### Comparing `fusio-sdk-5.0.3/src/sdk/backend_user.py` & `fusio-sdk-5.0.4/src/sdk/consumer_app.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 """
-backend_user automatically generated by SDKgen please do not edit this file manually
+consumer_app automatically generated by SDKgen please do not edit this file manually
 https://sdkgen.app
 """
 
 from dataclasses import dataclass, field
 from dataclasses_json import dataclass_json, config
 from typing import List
-from backend_app import BackendApp
-from common_metadata import CommonMetadata
+from .common_metadata import CommonMetadata
 @dataclass_json
 @dataclass
-class BackendUser:
+class ConsumerApp:
     id: int = field(default=None, metadata=config(field_name="id"))
-    role_id: int = field(default=None, metadata=config(field_name="roleId"))
-    plan_id: int = field(default=None, metadata=config(field_name="planId"))
+    user_id: int = field(default=None, metadata=config(field_name="userId"))
     status: int = field(default=None, metadata=config(field_name="status"))
     name: str = field(default=None, metadata=config(field_name="name"))
-    email: str = field(default=None, metadata=config(field_name="email"))
-    points: int = field(default=None, metadata=config(field_name="points"))
+    url: str = field(default=None, metadata=config(field_name="url"))
+    app_key: str = field(default=None, metadata=config(field_name="appKey"))
+    app_secret: str = field(default=None, metadata=config(field_name="appSecret"))
+    date: str = field(default=None, metadata=config(field_name="date"))
     scopes: List[str] = field(default=None, metadata=config(field_name="scopes"))
-    apps: List[BackendApp] = field(default=None, metadata=config(field_name="apps"))
     metadata: CommonMetadata = field(default=None, metadata=config(field_name="metadata"))
-    date: datetime.datetime = field(default=None, metadata=config(field_name="date"))
```

### Comparing `fusio-sdk-5.0.3/src/sdk/backend_user_tag.py` & `fusio-sdk-5.0.4/src/sdk/backend_user_tag.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,20 +3,20 @@
 https://sdkgen.app
 """
 
 import requests
 import sdkgen
 from requests import RequestException
 
-from backend_user import BackendUser
-from backend_user_collection import BackendUserCollection
-from backend_user_create import BackendUserCreate
-from backend_user_update import BackendUserUpdate
-from common_message import CommonMessage
-from common_message_exception import CommonMessageException
+from .backend_user import BackendUser
+from .backend_user_collection import BackendUserCollection
+from .backend_user_create import BackendUserCreate
+from .backend_user_update import BackendUserUpdate
+from .common_message import CommonMessage
+from .common_message_exception import CommonMessageException
 
 class BackendUserTag(sdkgen.TagAbstract):
     def __init__(self, http_client: requests.Session, parser: sdkgen.Parser):
         super().__init__(http_client, parser)
 
     pass
```

### Comparing `fusio-sdk-5.0.3/src/sdk/backend_webhook.py` & `fusio-sdk-5.0.4/src/sdk/consumer_user_plan.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,15 @@
 """
-backend_webhook automatically generated by SDKgen please do not edit this file manually
+consumer_user_plan automatically generated by SDKgen please do not edit this file manually
 https://sdkgen.app
 """
 
 from dataclasses import dataclass, field
 from dataclasses_json import dataclass_json, config
-from typing import List
-from backend_webhook_response import BackendWebhookResponse
 @dataclass_json
 @dataclass
-class BackendWebhook:
+class ConsumerUserPlan:
     id: int = field(default=None, metadata=config(field_name="id"))
-    event_id: int = field(default=None, metadata=config(field_name="eventId"))
-    user_id: int = field(default=None, metadata=config(field_name="userId"))
     name: str = field(default=None, metadata=config(field_name="name"))
-    endpoint: str = field(default=None, metadata=config(field_name="endpoint"))
-    responses: List[BackendWebhookResponse] = field(default=None, metadata=config(field_name="responses"))
+    price: int = field(default=None, metadata=config(field_name="price"))
+    points: int = field(default=None, metadata=config(field_name="points"))
+    period: int = field(default=None, metadata=config(field_name="period"))
```

### Comparing `fusio-sdk-5.0.3/src/sdk/backend_webhook_response.py` & `fusio-sdk-5.0.4/src/sdk/backend_webhook_response.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.3/src/sdk/backend_webhook_tag.py` & `fusio-sdk-5.0.4/src/sdk/backend_webhook_tag.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,20 +3,20 @@
 https://sdkgen.app
 """
 
 import requests
 import sdkgen
 from requests import RequestException
 
-from backend_webhook import BackendWebhook
-from backend_webhook_collection import BackendWebhookCollection
-from backend_webhook_create import BackendWebhookCreate
-from backend_webhook_update import BackendWebhookUpdate
-from common_message import CommonMessage
-from common_message_exception import CommonMessageException
+from .backend_webhook import BackendWebhook
+from .backend_webhook_collection import BackendWebhookCollection
+from .backend_webhook_create import BackendWebhookCreate
+from .backend_webhook_update import BackendWebhookUpdate
+from .common_message import CommonMessage
+from .common_message_exception import CommonMessageException
 
 class BackendWebhookTag(sdkgen.TagAbstract):
     def __init__(self, http_client: requests.Session, parser: sdkgen.Parser):
         super().__init__(http_client, parser)
 
     pass
```

### Comparing `fusio-sdk-5.0.3/src/sdk/client.py` & `fusio-sdk-5.0.4/src/sdk/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 https://sdkgen.app
 """
 
 import requests
 import sdkgen
 from requests import RequestException
 
-from authorization_tag import AuthorizationTag
-from system_tag import SystemTag
-from consumer_tag import ConsumerTag
-from backend_tag import BackendTag
+from .authorization_tag import AuthorizationTag
+from .system_tag import SystemTag
+from .consumer_tag import ConsumerTag
+from .backend_tag import BackendTag
 
 class Client(sdkgen.ClientAbstract):
     def __init__(self, base_url: str, credentials: sdkgen.CredentialsInterface):
         super().__init__(base_url, credentials)
 
     pass
```

### Comparing `fusio-sdk-5.0.3/src/sdk/common_collection.py` & `fusio-sdk-5.0.4/src/sdk/common_collection.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.3/src/sdk/common_form_container.py` & `fusio-sdk-5.0.4/src/sdk/common_form_container.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 https://sdkgen.app
 """
 
 from dataclasses import dataclass, field
 from dataclasses_json import dataclass_json, config
 from typing import List
 from typing import Union
-from common_form_element_input import CommonFormElementInput
-from common_form_element_select import CommonFormElementSelect
-from common_form_element_tag import CommonFormElementTag
-from common_form_element_text_area import CommonFormElementTextArea
+from .common_form_element_input import CommonFormElementInput
+from .common_form_element_select import CommonFormElementSelect
+from .common_form_element_tag import CommonFormElementTag
+from .common_form_element_text_area import CommonFormElementTextArea
 @dataclass_json
 @dataclass
 class CommonFormContainer:
     element: List[Union[CommonFormElementInput, CommonFormElementSelect, CommonFormElementTag, CommonFormElementTextArea]] = field(default=None, metadata=config(field_name="element"))
```

### Comparing `fusio-sdk-5.0.3/src/sdk/common_form_element.py` & `fusio-sdk-5.0.4/src/sdk/common_form_element.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.3/src/sdk/common_form_element_select.py` & `fusio-sdk-5.0.4/src/sdk/common_form_element_select.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,13 +2,13 @@
 common_form_element_select automatically generated by SDKgen please do not edit this file manually
 https://sdkgen.app
 """
 
 from dataclasses import dataclass, field
 from dataclasses_json import dataclass_json, config
 from typing import List
-from common_form_element import CommonFormElement
-from common_form_element_select_option import CommonFormElementSelectOption
+from .common_form_element import CommonFormElement
+from .common_form_element_select_option import CommonFormElementSelectOption
 @dataclass_json
 @dataclass
 class CommonFormElementSelect(CommonFormElement):
     options: List[CommonFormElementSelectOption] = field(default=None, metadata=config(field_name="options"))
```

### Comparing `fusio-sdk-5.0.3/src/sdk/consumer_account_tag.py` & `fusio-sdk-5.0.4/src/sdk/consumer_account_tag.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,28 +3,28 @@
 https://sdkgen.app
 """
 
 import requests
 import sdkgen
 from requests import RequestException
 
-from backend_account_change_password import BackendAccountChangePassword
-from common_message import CommonMessage
-from common_message_exception import CommonMessageException
-from consumer_authorize_meta import ConsumerAuthorizeMeta
-from consumer_authorize_request import ConsumerAuthorizeRequest
-from consumer_authorize_response import ConsumerAuthorizeResponse
-from consumer_user_account import ConsumerUserAccount
-from consumer_user_activate import ConsumerUserActivate
-from consumer_user_email import ConsumerUserEmail
-from consumer_user_jwt import ConsumerUserJWT
-from consumer_user_login import ConsumerUserLogin
-from consumer_user_password_reset import ConsumerUserPasswordReset
-from consumer_user_refresh import ConsumerUserRefresh
-from consumer_user_register import ConsumerUserRegister
+from .backend_account_change_password import BackendAccountChangePassword
+from .common_message import CommonMessage
+from .common_message_exception import CommonMessageException
+from .consumer_authorize_meta import ConsumerAuthorizeMeta
+from .consumer_authorize_request import ConsumerAuthorizeRequest
+from .consumer_authorize_response import ConsumerAuthorizeResponse
+from .consumer_user_account import ConsumerUserAccount
+from .consumer_user_activate import ConsumerUserActivate
+from .consumer_user_email import ConsumerUserEmail
+from .consumer_user_jwt import ConsumerUserJWT
+from .consumer_user_login import ConsumerUserLogin
+from .consumer_user_password_reset import ConsumerUserPasswordReset
+from .consumer_user_refresh import ConsumerUserRefresh
+from .consumer_user_register import ConsumerUserRegister
 
 class ConsumerAccountTag(sdkgen.TagAbstract):
     def __init__(self, http_client: requests.Session, parser: sdkgen.Parser):
         super().__init__(http_client, parser)
 
     pass
```

### Comparing `fusio-sdk-5.0.3/src/sdk/consumer_app.py` & `fusio-sdk-5.0.4/src/sdk/backend_user.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 """
-consumer_app automatically generated by SDKgen please do not edit this file manually
+backend_user automatically generated by SDKgen please do not edit this file manually
 https://sdkgen.app
 """
 
 from dataclasses import dataclass, field
 from dataclasses_json import dataclass_json, config
 from typing import List
-from common_metadata import CommonMetadata
+from .backend_app import BackendApp
+from .common_metadata import CommonMetadata
 @dataclass_json
 @dataclass
-class ConsumerApp:
+class BackendUser:
     id: int = field(default=None, metadata=config(field_name="id"))
-    user_id: int = field(default=None, metadata=config(field_name="userId"))
+    role_id: int = field(default=None, metadata=config(field_name="roleId"))
+    plan_id: int = field(default=None, metadata=config(field_name="planId"))
     status: int = field(default=None, metadata=config(field_name="status"))
     name: str = field(default=None, metadata=config(field_name="name"))
-    url: str = field(default=None, metadata=config(field_name="url"))
-    app_key: str = field(default=None, metadata=config(field_name="appKey"))
-    app_secret: str = field(default=None, metadata=config(field_name="appSecret"))
-    date: str = field(default=None, metadata=config(field_name="date"))
+    email: str = field(default=None, metadata=config(field_name="email"))
+    points: int = field(default=None, metadata=config(field_name="points"))
     scopes: List[str] = field(default=None, metadata=config(field_name="scopes"))
+    apps: List[BackendApp] = field(default=None, metadata=config(field_name="apps"))
     metadata: CommonMetadata = field(default=None, metadata=config(field_name="metadata"))
+    date: datetime.datetime = field(default=None, metadata=config(field_name="date"))
```

### Comparing `fusio-sdk-5.0.3/src/sdk/consumer_app_create.py` & `fusio-sdk-5.0.4/src/sdk/consumer_app_create.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.3/src/sdk/consumer_app_tag.py` & `fusio-sdk-5.0.4/src/sdk/consumer_app_tag.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,20 +3,20 @@
 https://sdkgen.app
 """
 
 import requests
 import sdkgen
 from requests import RequestException
 
-from common_message import CommonMessage
-from common_message_exception import CommonMessageException
-from consumer_app import ConsumerApp
-from consumer_app_collection import ConsumerAppCollection
-from consumer_app_create import ConsumerAppCreate
-from consumer_app_update import ConsumerAppUpdate
+from .common_message import CommonMessage
+from .common_message_exception import CommonMessageException
+from .consumer_app import ConsumerApp
+from .consumer_app_collection import ConsumerAppCollection
+from .consumer_app_create import ConsumerAppCreate
+from .consumer_app_update import ConsumerAppUpdate
 
 class ConsumerAppTag(sdkgen.TagAbstract):
     def __init__(self, http_client: requests.Session, parser: sdkgen.Parser):
         super().__init__(http_client, parser)
 
     pass
```

### Comparing `fusio-sdk-5.0.3/src/sdk/consumer_app_update.py` & `fusio-sdk-5.0.4/src/sdk/consumer_app_update.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.3/src/sdk/consumer_authorize_meta.py` & `fusio-sdk-5.0.4/src/sdk/consumer_authorize_meta.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,14 @@
 consumer_authorize_meta automatically generated by SDKgen please do not edit this file manually
 https://sdkgen.app
 """
 
 from dataclasses import dataclass, field
 from dataclasses_json import dataclass_json, config
 from typing import List
-from consumer_scope import ConsumerScope
+from .consumer_scope import ConsumerScope
 @dataclass_json
 @dataclass
 class ConsumerAuthorizeMeta:
     name: str = field(default=None, metadata=config(field_name="name"))
     url: str = field(default=None, metadata=config(field_name="url"))
     scopes: List[ConsumerScope] = field(default=None, metadata=config(field_name="scopes"))
```

### Comparing `fusio-sdk-5.0.3/src/sdk/consumer_authorize_request.py` & `fusio-sdk-5.0.4/src/sdk/consumer_authorize_request.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.3/src/sdk/consumer_authorize_response.py` & `fusio-sdk-5.0.4/src/sdk/consumer_authorize_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 consumer_authorize_response automatically generated by SDKgen please do not edit this file manually
 https://sdkgen.app
 """
 
 from dataclasses import dataclass, field
 from dataclasses_json import dataclass_json, config
-from consumer_authorize_response_token import ConsumerAuthorizeResponseToken
+from .consumer_authorize_response_token import ConsumerAuthorizeResponseToken
 @dataclass_json
 @dataclass
 class ConsumerAuthorizeResponse:
     type: str = field(default=None, metadata=config(field_name="type"))
     token: ConsumerAuthorizeResponseToken = field(default=None, metadata=config(field_name="token"))
     code: str = field(default=None, metadata=config(field_name="code"))
     redirect_uri: str = field(default=None, metadata=config(field_name="redirectUri"))
```

### Comparing `fusio-sdk-5.0.3/src/sdk/consumer_authorize_response_token.py` & `fusio-sdk-5.0.4/src/sdk/consumer_authorize_response_token.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.3/src/sdk/consumer_event.py` & `fusio-sdk-5.0.4/src/sdk/consumer_event.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 consumer_event automatically generated by SDKgen please do not edit this file manually
 https://sdkgen.app
 """
 
 from dataclasses import dataclass, field
 from dataclasses_json import dataclass_json, config
-from common_metadata import CommonMetadata
+from .common_metadata import CommonMetadata
 @dataclass_json
 @dataclass
 class ConsumerEvent:
     id: int = field(default=None, metadata=config(field_name="id"))
     name: str = field(default=None, metadata=config(field_name="name"))
     description: str = field(default=None, metadata=config(field_name="description"))
     metadata: CommonMetadata = field(default=None, metadata=config(field_name="metadata"))
```

### Comparing `fusio-sdk-5.0.3/src/sdk/consumer_event_tag.py` & `fusio-sdk-5.0.4/src/sdk/consumer_event_tag.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 https://sdkgen.app
 """
 
 import requests
 import sdkgen
 from requests import RequestException
 
-from common_message_exception import CommonMessageException
-from consumer_event_collection import ConsumerEventCollection
+from .common_message_exception import CommonMessageException
+from .consumer_event_collection import ConsumerEventCollection
 
 class ConsumerEventTag(sdkgen.TagAbstract):
     def __init__(self, http_client: requests.Session, parser: sdkgen.Parser):
         super().__init__(http_client, parser)
 
     pass
```

### Comparing `fusio-sdk-5.0.3/src/sdk/consumer_grant.py` & `fusio-sdk-5.0.4/src/sdk/consumer_grant.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 consumer_grant automatically generated by SDKgen please do not edit this file manually
 https://sdkgen.app
 """
 
 from dataclasses import dataclass, field
 from dataclasses_json import dataclass_json, config
-from consumer_app import ConsumerApp
+from .consumer_app import ConsumerApp
 @dataclass_json
 @dataclass
 class ConsumerGrant:
     id: int = field(default=None, metadata=config(field_name="id"))
     app: ConsumerApp = field(default=None, metadata=config(field_name="app"))
     create_date: datetime.datetime = field(default=None, metadata=config(field_name="createDate"))
```

### Comparing `fusio-sdk-5.0.3/src/sdk/consumer_grant_tag.py` & `fusio-sdk-5.0.4/src/sdk/consumer_grant_tag.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 https://sdkgen.app
 """
 
 import requests
 import sdkgen
 from requests import RequestException
 
-from common_message import CommonMessage
-from common_message_exception import CommonMessageException
-from consumer_grant_collection import ConsumerGrantCollection
+from .common_message import CommonMessage
+from .common_message_exception import CommonMessageException
+from .consumer_grant_collection import ConsumerGrantCollection
 
 class ConsumerGrantTag(sdkgen.TagAbstract):
     def __init__(self, http_client: requests.Session, parser: sdkgen.Parser):
         super().__init__(http_client, parser)
 
     pass
```

### Comparing `fusio-sdk-5.0.3/src/sdk/consumer_identity.py` & `fusio-sdk-5.0.4/src/sdk/consumer_identity.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.3/src/sdk/consumer_identity_tag.py` & `fusio-sdk-5.0.4/src/sdk/consumer_identity_tag.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 https://sdkgen.app
 """
 
 import requests
 import sdkgen
 from requests import RequestException
 
-from common_message_exception import CommonMessageException
-from consumer_identity_collection import ConsumerIdentityCollection
-from passthru import Passthru
+from .common_message_exception import CommonMessageException
+from .consumer_identity_collection import ConsumerIdentityCollection
+from .passthru import Passthru
 
 class ConsumerIdentityTag(sdkgen.TagAbstract):
     def __init__(self, http_client: requests.Session, parser: sdkgen.Parser):
         super().__init__(http_client, parser)
 
     pass
```

### Comparing `fusio-sdk-5.0.3/src/sdk/consumer_log.py` & `fusio-sdk-5.0.4/src/sdk/consumer_token_access_token.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,15 @@
 """
-consumer_log automatically generated by SDKgen please do not edit this file manually
+consumer_token_access_token automatically generated by SDKgen please do not edit this file manually
 https://sdkgen.app
 """
 
 from dataclasses import dataclass, field
 from dataclasses_json import dataclass_json, config
 @dataclass_json
 @dataclass
-class ConsumerLog:
-    id: int = field(default=None, metadata=config(field_name="id"))
-    app_id: int = field(default=None, metadata=config(field_name="appId"))
-    ip: str = field(default=None, metadata=config(field_name="ip"))
-    user_agent: str = field(default=None, metadata=config(field_name="userAgent"))
-    method: str = field(default=None, metadata=config(field_name="method"))
-    path: str = field(default=None, metadata=config(field_name="path"))
-    header: str = field(default=None, metadata=config(field_name="header"))
-    body: str = field(default=None, metadata=config(field_name="body"))
-    date: datetime.datetime = field(default=None, metadata=config(field_name="date"))
+class ConsumerTokenAccessToken:
+    access_token: str = field(default=None, metadata=config(field_name="access_token"))
+    token_type: str = field(default=None, metadata=config(field_name="token_type"))
+    expires_in: int = field(default=None, metadata=config(field_name="expires_in"))
+    refresh_token: str = field(default=None, metadata=config(field_name="refresh_token"))
+    scope: str = field(default=None, metadata=config(field_name="scope"))
```

### Comparing `fusio-sdk-5.0.3/src/sdk/consumer_log_tag.py` & `fusio-sdk-5.0.4/src/sdk/consumer_log_tag.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 https://sdkgen.app
 """
 
 import requests
 import sdkgen
 from requests import RequestException
 
-from common_message_exception import CommonMessageException
-from consumer_log import ConsumerLog
-from consumer_log_collection import ConsumerLogCollection
+from .common_message_exception import CommonMessageException
+from .consumer_log import ConsumerLog
+from .consumer_log_collection import ConsumerLogCollection
 
 class ConsumerLogTag(sdkgen.TagAbstract):
     def __init__(self, http_client: requests.Session, parser: sdkgen.Parser):
         super().__init__(http_client, parser)
 
     pass
```

### Comparing `fusio-sdk-5.0.3/src/sdk/consumer_page.py` & `fusio-sdk-5.0.4/src/sdk/consumer_page.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 consumer_page automatically generated by SDKgen please do not edit this file manually
 https://sdkgen.app
 """
 
 from dataclasses import dataclass, field
 from dataclasses_json import dataclass_json, config
-from common_metadata import CommonMetadata
+from .common_metadata import CommonMetadata
 @dataclass_json
 @dataclass
 class ConsumerPage:
     id: int = field(default=None, metadata=config(field_name="id"))
     title: str = field(default=None, metadata=config(field_name="title"))
     slug: str = field(default=None, metadata=config(field_name="slug"))
     content: str = field(default=None, metadata=config(field_name="content"))
```

### Comparing `fusio-sdk-5.0.3/src/sdk/consumer_page_tag.py` & `fusio-sdk-5.0.4/src/sdk/consumer_page_tag.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 https://sdkgen.app
 """
 
 import requests
 import sdkgen
 from requests import RequestException
 
-from common_message_exception import CommonMessageException
-from consumer_page import ConsumerPage
-from consumer_page_collection import ConsumerPageCollection
+from .common_message_exception import CommonMessageException
+from .consumer_page import ConsumerPage
+from .consumer_page_collection import ConsumerPageCollection
 
 class ConsumerPageTag(sdkgen.TagAbstract):
     def __init__(self, http_client: requests.Session, parser: sdkgen.Parser):
         super().__init__(http_client, parser)
 
     pass
```

### Comparing `fusio-sdk-5.0.3/src/sdk/consumer_payment_tag.py` & `fusio-sdk-5.0.4/src/sdk/consumer_payment_tag.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 https://sdkgen.app
 """
 
 import requests
 import sdkgen
 from requests import RequestException
 
-from common_message_exception import CommonMessageException
-from consumer_payment_checkout_request import ConsumerPaymentCheckoutRequest
-from consumer_payment_checkout_response import ConsumerPaymentCheckoutResponse
-from consumer_payment_portal_request import ConsumerPaymentPortalRequest
-from consumer_payment_portal_response import ConsumerPaymentPortalResponse
+from .common_message_exception import CommonMessageException
+from .consumer_payment_checkout_request import ConsumerPaymentCheckoutRequest
+from .consumer_payment_checkout_response import ConsumerPaymentCheckoutResponse
+from .consumer_payment_portal_request import ConsumerPaymentPortalRequest
+from .consumer_payment_portal_response import ConsumerPaymentPortalResponse
 
 class ConsumerPaymentTag(sdkgen.TagAbstract):
     def __init__(self, http_client: requests.Session, parser: sdkgen.Parser):
         super().__init__(http_client, parser)
 
     pass
```

### Comparing `fusio-sdk-5.0.3/src/sdk/consumer_plan.py` & `fusio-sdk-5.0.4/src/sdk/consumer_plan.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 consumer_plan automatically generated by SDKgen please do not edit this file manually
 https://sdkgen.app
 """
 
 from dataclasses import dataclass, field
 from dataclasses_json import dataclass_json, config
-from common_metadata import CommonMetadata
+from .common_metadata import CommonMetadata
 @dataclass_json
 @dataclass
 class ConsumerPlan:
     id: int = field(default=None, metadata=config(field_name="id"))
     name: str = field(default=None, metadata=config(field_name="name"))
     description: str = field(default=None, metadata=config(field_name="description"))
     price: float = field(default=None, metadata=config(field_name="price"))
```

### Comparing `fusio-sdk-5.0.3/src/sdk/consumer_plan_tag.py` & `fusio-sdk-5.0.4/src/sdk/consumer_plan_tag.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 https://sdkgen.app
 """
 
 import requests
 import sdkgen
 from requests import RequestException
 
-from common_message_exception import CommonMessageException
-from consumer_plan import ConsumerPlan
-from consumer_plan_collection import ConsumerPlanCollection
+from .common_message_exception import CommonMessageException
+from .consumer_plan import ConsumerPlan
+from .consumer_plan_collection import ConsumerPlanCollection
 
 class ConsumerPlanTag(sdkgen.TagAbstract):
     def __init__(self, http_client: requests.Session, parser: sdkgen.Parser):
         super().__init__(http_client, parser)
 
     pass
```

### Comparing `fusio-sdk-5.0.3/src/sdk/consumer_scope.py` & `fusio-sdk-5.0.4/src/sdk/consumer_scope.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 consumer_scope automatically generated by SDKgen please do not edit this file manually
 https://sdkgen.app
 """
 
 from dataclasses import dataclass, field
 from dataclasses_json import dataclass_json, config
-from common_metadata import CommonMetadata
+from .common_metadata import CommonMetadata
 @dataclass_json
 @dataclass
 class ConsumerScope:
     id: int = field(default=None, metadata=config(field_name="id"))
     name: str = field(default=None, metadata=config(field_name="name"))
     description: str = field(default=None, metadata=config(field_name="description"))
     metadata: CommonMetadata = field(default=None, metadata=config(field_name="metadata"))
```

### Comparing `fusio-sdk-5.0.3/src/sdk/consumer_scope_tag.py` & `fusio-sdk-5.0.4/src/sdk/consumer_scope_tag.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 https://sdkgen.app
 """
 
 import requests
 import sdkgen
 from requests import RequestException
 
-from common_message_exception import CommonMessageException
-from consumer_scope_collection import ConsumerScopeCollection
+from .common_message_exception import CommonMessageException
+from .consumer_scope_collection import ConsumerScopeCollection
 
 class ConsumerScopeTag(sdkgen.TagAbstract):
     def __init__(self, http_client: requests.Session, parser: sdkgen.Parser):
         super().__init__(http_client, parser)
 
     pass
```

### Comparing `fusio-sdk-5.0.3/src/sdk/consumer_tag.py` & `fusio-sdk-5.0.4/src/sdk/consumer_tag.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,27 +3,27 @@
 https://sdkgen.app
 """
 
 import requests
 import sdkgen
 from requests import RequestException
 
-from consumer_account_tag import ConsumerAccountTag
-from consumer_app_tag import ConsumerAppTag
-from consumer_event_tag import ConsumerEventTag
-from consumer_grant_tag import ConsumerGrantTag
-from consumer_identity_tag import ConsumerIdentityTag
-from consumer_log_tag import ConsumerLogTag
-from consumer_page_tag import ConsumerPageTag
-from consumer_payment_tag import ConsumerPaymentTag
-from consumer_plan_tag import ConsumerPlanTag
-from consumer_scope_tag import ConsumerScopeTag
-from consumer_token_tag import ConsumerTokenTag
-from consumer_transaction_tag import ConsumerTransactionTag
-from consumer_webhook_tag import ConsumerWebhookTag
+from .consumer_account_tag import ConsumerAccountTag
+from .consumer_app_tag import ConsumerAppTag
+from .consumer_event_tag import ConsumerEventTag
+from .consumer_grant_tag import ConsumerGrantTag
+from .consumer_identity_tag import ConsumerIdentityTag
+from .consumer_log_tag import ConsumerLogTag
+from .consumer_page_tag import ConsumerPageTag
+from .consumer_payment_tag import ConsumerPaymentTag
+from .consumer_plan_tag import ConsumerPlanTag
+from .consumer_scope_tag import ConsumerScopeTag
+from .consumer_token_tag import ConsumerTokenTag
+from .consumer_transaction_tag import ConsumerTransactionTag
+from .consumer_webhook_tag import ConsumerWebhookTag
 
 class ConsumerTag(sdkgen.TagAbstract):
     def __init__(self, http_client: requests.Session, parser: sdkgen.Parser):
         super().__init__(http_client, parser)
 
     pass
```

### Comparing `fusio-sdk-5.0.3/src/sdk/consumer_token.py` & `fusio-sdk-5.0.4/src/sdk/consumer_token.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.3/src/sdk/consumer_token_create.py` & `fusio-sdk-5.0.4/src/sdk/consumer_token_create.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.3/src/sdk/consumer_token_tag.py` & `fusio-sdk-5.0.4/src/sdk/consumer_token_tag.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,21 +3,21 @@
 https://sdkgen.app
 """
 
 import requests
 import sdkgen
 from requests import RequestException
 
-from common_message import CommonMessage
-from common_message_exception import CommonMessageException
-from consumer_token import ConsumerToken
-from consumer_token_access_token import ConsumerTokenAccessToken
-from consumer_token_collection import ConsumerTokenCollection
-from consumer_token_create import ConsumerTokenCreate
-from consumer_token_update import ConsumerTokenUpdate
+from .common_message import CommonMessage
+from .common_message_exception import CommonMessageException
+from .consumer_token import ConsumerToken
+from .consumer_token_access_token import ConsumerTokenAccessToken
+from .consumer_token_collection import ConsumerTokenCollection
+from .consumer_token_create import ConsumerTokenCreate
+from .consumer_token_update import ConsumerTokenUpdate
 
 class ConsumerTokenTag(sdkgen.TagAbstract):
     def __init__(self, http_client: requests.Session, parser: sdkgen.Parser):
         super().__init__(http_client, parser)
 
     pass
```

### Comparing `fusio-sdk-5.0.3/src/sdk/consumer_transaction.py` & `fusio-sdk-5.0.4/src/sdk/consumer_transaction.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 consumer_transaction automatically generated by SDKgen please do not edit this file manually
 https://sdkgen.app
 """
 
 from dataclasses import dataclass, field
 from dataclasses_json import dataclass_json, config
-from consumer_plan import ConsumerPlan
+from .consumer_plan import ConsumerPlan
 @dataclass_json
 @dataclass
 class ConsumerTransaction:
     id: int = field(default=None, metadata=config(field_name="id"))
     user_id: int = field(default=None, metadata=config(field_name="userId"))
     plan_id: int = field(default=None, metadata=config(field_name="planId"))
     plan: ConsumerPlan = field(default=None, metadata=config(field_name="plan"))
```

### Comparing `fusio-sdk-5.0.3/src/sdk/consumer_transaction_tag.py` & `fusio-sdk-5.0.4/src/sdk/consumer_transaction_tag.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 https://sdkgen.app
 """
 
 import requests
 import sdkgen
 from requests import RequestException
 
-from common_message_exception import CommonMessageException
-from consumer_transaction import ConsumerTransaction
-from consumer_transaction_collection import ConsumerTransactionCollection
+from .common_message_exception import CommonMessageException
+from .consumer_transaction import ConsumerTransaction
+from .consumer_transaction_collection import ConsumerTransactionCollection
 
 class ConsumerTransactionTag(sdkgen.TagAbstract):
     def __init__(self, http_client: requests.Session, parser: sdkgen.Parser):
         super().__init__(http_client, parser)
 
     pass
```

### Comparing `fusio-sdk-5.0.3/src/sdk/consumer_user_account.py` & `fusio-sdk-5.0.4/src/sdk/consumer_user_account.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 consumer_user_account automatically generated by SDKgen please do not edit this file manually
 https://sdkgen.app
 """
 
 from dataclasses import dataclass, field
 from dataclasses_json import dataclass_json, config
 from typing import List
-from consumer_user_plan import ConsumerUserPlan
-from common_metadata import CommonMetadata
+from .consumer_user_plan import ConsumerUserPlan
+from .common_metadata import CommonMetadata
 @dataclass_json
 @dataclass
 class ConsumerUserAccount:
     id: int = field(default=None, metadata=config(field_name="id"))
     plan_id: int = field(default=None, metadata=config(field_name="planId"))
     status: int = field(default=None, metadata=config(field_name="status"))
     name: str = field(default=None, metadata=config(field_name="name"))
```

### Comparing `fusio-sdk-5.0.3/src/sdk/consumer_user_jwt.py` & `fusio-sdk-5.0.4/src/sdk/consumer_user_jwt.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.3/src/sdk/consumer_user_login.py` & `fusio-sdk-5.0.4/src/sdk/consumer_user_login.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.3/src/sdk/consumer_user_plan.py` & `fusio-sdk-5.0.4/src/sdk/consumer_webhook.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 """
-consumer_user_plan automatically generated by SDKgen please do not edit this file manually
+consumer_webhook automatically generated by SDKgen please do not edit this file manually
 https://sdkgen.app
 """
 
 from dataclasses import dataclass, field
 from dataclasses_json import dataclass_json, config
+from typing import List
+from .consumer_webhook_response import ConsumerWebhookResponse
 @dataclass_json
 @dataclass
-class ConsumerUserPlan:
+class ConsumerWebhook:
     id: int = field(default=None, metadata=config(field_name="id"))
+    status: int = field(default=None, metadata=config(field_name="status"))
+    event: str = field(default=None, metadata=config(field_name="event"))
     name: str = field(default=None, metadata=config(field_name="name"))
-    price: int = field(default=None, metadata=config(field_name="price"))
-    points: int = field(default=None, metadata=config(field_name="points"))
-    period: int = field(default=None, metadata=config(field_name="period"))
+    endpoint: str = field(default=None, metadata=config(field_name="endpoint"))
+    responses: List[ConsumerWebhookResponse] = field(default=None, metadata=config(field_name="responses"))
```

### Comparing `fusio-sdk-5.0.3/src/sdk/consumer_user_register.py` & `fusio-sdk-5.0.4/src/sdk/consumer_user_register.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.3/src/sdk/consumer_webhook.py` & `fusio-sdk-5.0.4/src/sdk/backend_webhook.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """
-consumer_webhook automatically generated by SDKgen please do not edit this file manually
+backend_webhook automatically generated by SDKgen please do not edit this file manually
 https://sdkgen.app
 """
 
 from dataclasses import dataclass, field
 from dataclasses_json import dataclass_json, config
 from typing import List
-from consumer_webhook_response import ConsumerWebhookResponse
+from .backend_webhook_response import BackendWebhookResponse
 @dataclass_json
 @dataclass
-class ConsumerWebhook:
+class BackendWebhook:
     id: int = field(default=None, metadata=config(field_name="id"))
-    status: int = field(default=None, metadata=config(field_name="status"))
-    event: str = field(default=None, metadata=config(field_name="event"))
+    event_id: int = field(default=None, metadata=config(field_name="eventId"))
+    user_id: int = field(default=None, metadata=config(field_name="userId"))
     name: str = field(default=None, metadata=config(field_name="name"))
     endpoint: str = field(default=None, metadata=config(field_name="endpoint"))
-    responses: List[ConsumerWebhookResponse] = field(default=None, metadata=config(field_name="responses"))
+    responses: List[BackendWebhookResponse] = field(default=None, metadata=config(field_name="responses"))
```

### Comparing `fusio-sdk-5.0.3/src/sdk/consumer_webhook_response.py` & `fusio-sdk-5.0.4/src/sdk/consumer_webhook_response.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.3/src/sdk/consumer_webhook_tag.py` & `fusio-sdk-5.0.4/src/sdk/consumer_webhook_tag.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,20 +3,20 @@
 https://sdkgen.app
 """
 
 import requests
 import sdkgen
 from requests import RequestException
 
-from common_message import CommonMessage
-from common_message_exception import CommonMessageException
-from consumer_webhook import ConsumerWebhook
-from consumer_webhook_collection import ConsumerWebhookCollection
-from consumer_webhook_create import ConsumerWebhookCreate
-from consumer_webhook_update import ConsumerWebhookUpdate
+from .common_message import CommonMessage
+from .common_message_exception import CommonMessageException
+from .consumer_webhook import ConsumerWebhook
+from .consumer_webhook_collection import ConsumerWebhookCollection
+from .consumer_webhook_create import ConsumerWebhookCreate
+from .consumer_webhook_update import ConsumerWebhookUpdate
 
 class ConsumerWebhookTag(sdkgen.TagAbstract):
     def __init__(self, http_client: requests.Session, parser: sdkgen.Parser):
         super().__init__(http_client, parser)
 
     pass
```

### Comparing `fusio-sdk-5.0.3/src/sdk/system_about.py` & `fusio-sdk-5.0.4/src/sdk/system_about.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 system_about automatically generated by SDKgen please do not edit this file manually
 https://sdkgen.app
 """
 
 from dataclasses import dataclass, field
 from dataclasses_json import dataclass_json, config
 from typing import List
-from system_about_apps import SystemAboutApps
-from system_about_link import SystemAboutLink
+from .system_about_apps import SystemAboutApps
+from .system_about_link import SystemAboutLink
 @dataclass_json
 @dataclass
 class SystemAbout:
     api_version: str = field(default=None, metadata=config(field_name="apiVersion"))
     title: str = field(default=None, metadata=config(field_name="title"))
     description: str = field(default=None, metadata=config(field_name="description"))
     terms_of_service: str = field(default=None, metadata=config(field_name="termsOfService"))
```

### Comparing `fusio-sdk-5.0.3/src/sdk/system_connection_tag.py` & `fusio-sdk-5.0.4/src/sdk/system_connection_tag.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 https://sdkgen.app
 """
 
 import requests
 import sdkgen
 from requests import RequestException
 
-from common_message import CommonMessage
+from .common_message import CommonMessage
 
 class SystemConnectionTag(sdkgen.TagAbstract):
     def __init__(self, http_client: requests.Session, parser: sdkgen.Parser):
         super().__init__(http_client, parser)
 
     pass
```

### Comparing `fusio-sdk-5.0.3/src/sdk/system_meta_tag.py` & `fusio-sdk-5.0.4/src/sdk/system_meta_tag.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,21 +3,21 @@
 https://sdkgen.app
 """
 
 import requests
 import sdkgen
 from requests import RequestException
 
-from common_message_exception import CommonMessageException
-from passthru import Passthru
-from system_about import SystemAbout
-from system_health_check import SystemHealthCheck
-from system_o_auth_configuration import SystemOAuthConfiguration
-from system_route import SystemRoute
-from system_schema import SystemSchema
+from .common_message_exception import CommonMessageException
+from .passthru import Passthru
+from .system_about import SystemAbout
+from .system_health_check import SystemHealthCheck
+from .system_o_auth_configuration import SystemOAuthConfiguration
+from .system_route import SystemRoute
+from .system_schema import SystemSchema
 
 class SystemMetaTag(sdkgen.TagAbstract):
     def __init__(self, http_client: requests.Session, parser: sdkgen.Parser):
         super().__init__(http_client, parser)
 
     pass
```

### Comparing `fusio-sdk-5.0.3/src/sdk/system_o_auth_configuration.py` & `fusio-sdk-5.0.4/src/sdk/system_o_auth_configuration.py`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.3/src/sdk/system_payment_tag.py` & `fusio-sdk-5.0.4/src/sdk/system_payment_tag.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 https://sdkgen.app
 """
 
 import requests
 import sdkgen
 from requests import RequestException
 
-from common_message import CommonMessage
-from common_message_exception import CommonMessageException
+from .common_message import CommonMessage
+from .common_message_exception import CommonMessageException
 
 class SystemPaymentTag(sdkgen.TagAbstract):
     def __init__(self, http_client: requests.Session, parser: sdkgen.Parser):
         super().__init__(http_client, parser)
 
     pass
```

### Comparing `fusio-sdk-5.0.3/src/sdk/system_schema.py` & `fusio-sdk-5.0.4/src/sdk/system_schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 system_schema automatically generated by SDKgen please do not edit this file manually
 https://sdkgen.app
 """
 
 from dataclasses import dataclass, field
 from dataclasses_json import dataclass_json, config
-from system_schema_type_schema import SystemSchemaTypeSchema
-from system_schema_form import SystemSchemaForm
+from .system_schema_type_schema import SystemSchemaTypeSchema
+from .system_schema_form import SystemSchemaForm
 @dataclass_json
 @dataclass
 class SystemSchema:
     schema: SystemSchemaTypeSchema = field(default=None, metadata=config(field_name="schema"))
     form: SystemSchemaForm = field(default=None, metadata=config(field_name="form"))
```

### Comparing `fusio-sdk-5.0.3/src/sdk/system_tag.py` & `fusio-sdk-5.0.4/src/sdk/system_tag.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 https://sdkgen.app
 """
 
 import requests
 import sdkgen
 from requests import RequestException
 
-from system_connection_tag import SystemConnectionTag
-from system_meta_tag import SystemMetaTag
-from system_payment_tag import SystemPaymentTag
+from .system_connection_tag import SystemConnectionTag
+from .system_meta_tag import SystemMetaTag
+from .system_payment_tag import SystemPaymentTag
 
 class SystemTag(sdkgen.TagAbstract):
     def __init__(self, http_client: requests.Session, parser: sdkgen.Parser):
         super().__init__(http_client, parser)
 
     pass
```

