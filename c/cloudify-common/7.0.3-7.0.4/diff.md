# Comparing `tmp/cloudify-common-7.0.3.tar.gz` & `tmp/cloudify-common-7.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudify-common-7.0.3.tar", last modified: Tue Nov 28 12:56:21 2023, max compression
+gzip compressed data, was "cloudify-common-7.0.4.tar", last modified: Sun Apr  7 13:11:11 2024, max compression
```

## Comparing `cloudify-common-7.0.3.tar` & `cloudify-common-7.0.4.tar`

### file list

```diff
@@ -1,183 +1,183 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-28 12:56:21.801283 cloudify-common-7.0.3/
--rw-r--r--   0 root         (0) root         (0)    10273 2023-11-28 12:56:03.000000 cloudify-common-7.0.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)       39 2023-11-28 12:56:03.000000 cloudify-common-7.0.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      249 2023-11-28 12:56:21.801283 cloudify-common-7.0.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3034 2023-11-28 12:56:03.000000 cloudify-common-7.0.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-28 12:56:21.789283 cloudify-common-7.0.3/cloudify/
--rw-r--r--   0 root         (0) root         (0)     2286 2023-11-28 12:56:03.000000 cloudify-common-7.0.3/cloudify/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5056 2023-11-28 12:56:03.000000 cloudify-common-7.0.3/cloudify/agent_utils.py
--rw-r--r--   0 root         (0) root         (0)    23830 2023-11-28 12:56:03.000000 cloudify-common-7.0.3/cloudify/amqp_client.py
--rw-r--r--   0 root         (0) root         (0)     4028 2023-11-28 12:56:03.000000 cloudify-common-7.0.3/cloudify/cluster.py
--rw-r--r--   0 root         (0) root         (0)     1335 2023-11-28 12:56:03.000000 cloudify-common-7.0.3/cloudify/cluster_status.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-28 12:56:21.793283 cloudify-common-7.0.3/cloudify/compute/
--rw-r--r--   0 root         (0) root         (0)     4460 2023-11-28 12:56:03.000000 cloudify-common-7.0.3/cloudify/compute/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1302 2023-11-28 12:56:03.000000 cloudify-common-7.0.3/cloudify/conflict_handlers.py
--rw-r--r--   0 root         (0) root         (0)     4385 2023-11-28 12:56:03.000000 cloudify-common-7.0.3/cloudify/constants.py
--rw-r--r--   0 root         (0) root         (0)    47193 2023-11-28 12:56:03.000000 cloudify-common-7.0.3/cloudify/context.py
--rw-r--r--   0 root         (0) root         (0)     3855 2023-11-28 12:56:03.000000 cloudify-common-7.0.3/cloudify/cryptography_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-28 12:56:21.793283 cloudify-common-7.0.3/cloudify/ctx_wrappers/
--rw-r--r--   0 root         (0) root         (0)        0 2023-11-28 12:56:03.000000 cloudify-common-7.0.3/cloudify/ctx_wrappers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8328 2023-11-28 12:56:03.000000 cloudify-common-7.0.3/cloudify/ctx_wrappers/ctx-py.py
--rw-r--r--   0 root         (0) root         (0)     4271 2023-11-28 12:56:03.000000 cloudify-common-7.0.3/cloudify/decorators.py
--rw-r--r--   0 root         (0) root         (0)     3394 2023-11-28 12:56:03.000000 cloudify-common-7.0.3/cloudify/deployment_dependencies.py
--rw-r--r--   0 root         (0) root         (0)    18954 2023-11-28 12:56:03.000000 cloudify-common-7.0.3/cloudify/dispatch.py
--rw-r--r--   0 root         (0) root         (0)    19168 2023-11-28 12:56:03.000000 cloudify-common-7.0.3/cloudify/endpoint.py
--rw-r--r--   0 root         (0) root         (0)     3741 2023-11-28 12:56:03.000000 cloudify-common-7.0.3/cloudify/error_handling.py
--rw-r--r--   0 root         (0) root         (0)     4872 2023-11-28 12:56:03.000000 cloudify-common-7.0.3/cloudify/event.py
--rw-r--r--   0 root         (0) root         (0)     5918 2023-11-28 12:56:03.000000 cloudify-common-7.0.3/cloudify/exceptions.py
--rw-r--r--   0 root         (0) root         (0)    15865 2023-11-28 12:56:03.000000 cloudify-common-7.0.3/cloudify/logs.py
--rw-r--r--   0 root         (0) root         (0)    18303 2023-11-28 12:56:03.000000 cloudify-common-7.0.3/cloudify/manager.py
--rw-r--r--   0 root         (0) root         (0)     7829 2023-11-28 12:56:03.000000 cloudify-common-7.0.3/cloudify/mocks.py
--rw-r--r--   0 root         (0) root         (0)     4914 2023-11-28 12:56:03.000000 cloudify-common-7.0.3/cloudify/models_states.py
--rw-r--r--   0 root         (0) root         (0)    24914 2023-11-28 12:56:03.000000 cloudify-common-7.0.3/cloudify/plugin_installer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-28 12:56:21.793283 cloudify-common-7.0.3/cloudify/plugins/
--rw-r--r--   0 root         (0) root         (0)      643 2023-11-28 12:56:03.000000 cloudify-common-7.0.3/cloudify/plugins/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1213 2023-11-28 12:56:03.000000 cloudify-common-7.0.3/cloudify/plugins/install_utils.py
--rw-r--r--   0 root         (0) root         (0)    53945 2023-11-28 12:56:03.000000 cloudify-common-7.0.3/cloudify/plugins/lifecycle.py
--rw-r--r--   0 root         (0) root         (0)    59556 2023-11-28 12:56:03.000000 cloudify-common-7.0.3/cloudify/plugins/workflows.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-28 12:56:21.793283 cloudify-common-7.0.3/cloudify/proxy/
--rw-r--r--   0 root         (0) root         (0)      637 2023-11-28 12:56:03.000000 cloudify-common-7.0.3/cloudify/proxy/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3965 2023-11-28 12:56:03.000000 cloudify-common-7.0.3/cloudify/proxy/client.py
--rw-r--r--   0 root         (0) root         (0)     8157 2023-11-28 12:56:03.000000 cloudify-common-7.0.3/cloudify/proxy/server.py
--rw-r--r--   0 root         (0) root         (0)     6223 2023-11-28 12:56:03.000000 cloudify-common-7.0.3/cloudify/rabbitmq_client.py
--rw-r--r--   0 root         (0) root         (0)      782 2023-11-28 12:56:03.000000 cloudify-common-7.0.3/cloudify/snapshots.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-28 12:56:21.793283 cloudify-common-7.0.3/cloudify/snmp/
--rw-r--r--   0 root         (0) root         (0)     5393 2023-11-28 12:56:03.000000 cloudify-common-7.0.3/cloudify/snmp/CLOUDIFY-MIB.mib
--rw-r--r--   0 root         (0) root         (0)        0 2023-11-28 12:56:03.000000 cloudify-common-7.0.3/cloudify/snmp/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4934 2023-11-28 12:56:03.000000 cloudify-common-7.0.3/cloudify/snmp/snmp_trap.py
--rw-r--r--   0 root         (0) root         (0)     3054 2023-11-28 12:56:03.000000 cloudify-common-7.0.3/cloudify/state.py
--rw-r--r--   0 root         (0) root         (0)     2330 2023-11-28 12:56:03.000000 cloudify-common-7.0.3/cloudify/systemddbus.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-28 12:56:21.793283 cloudify-common-7.0.3/cloudify/test_utils/
--rw-r--r--   0 root         (0) root         (0)      751 2023-11-28 12:56:03.000000 cloudify-common-7.0.3/cloudify/test_utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)      999 2023-11-28 12:56:03.000000 cloudify-common-7.0.3/cloudify/test_utils/dispatch_helper.py
--rw-r--r--   0 root         (0) root         (0)    11243 2023-11-28 12:56:03.000000 cloudify-common-7.0.3/cloudify/test_utils/local_workflow_decorator.py
--rw-r--r--   0 root         (0) root         (0)     3892 2023-11-28 12:56:03.000000 cloudify-common-7.0.3/cloudify/test_utils/mock_rest_client.py
--rw-r--r--   0 root         (0) root         (0)    37803 2023-11-28 12:56:03.000000 cloudify-common-7.0.3/cloudify/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-28 12:56:21.793283 cloudify-common-7.0.3/cloudify/workflows/
--rw-r--r--   0 root         (0) root         (0)      848 2023-11-28 12:56:03.000000 cloudify-common-7.0.3/cloudify/workflows/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8618 2023-11-28 12:56:03.000000 cloudify-common-7.0.3/cloudify/workflows/amqp_dispatcher.py
--rw-r--r--   0 root         (0) root         (0)     5562 2023-11-28 12:56:03.000000 cloudify-common-7.0.3/cloudify/workflows/events.py
--rw-r--r--   0 root         (0) root         (0)    36444 2023-11-28 12:56:03.000000 cloudify-common-7.0.3/cloudify/workflows/local.py
--rw-r--r--   0 root         (0) root         (0)    40724 2023-11-28 12:56:03.000000 cloudify-common-7.0.3/cloudify/workflows/tasks.py
--rw-r--r--   0 root         (0) root         (0)    26098 2023-11-28 12:56:03.000000 cloudify-common-7.0.3/cloudify/workflows/tasks_graph.py
--rw-r--r--   0 root         (0) root         (0)     2782 2023-11-28 12:56:03.000000 cloudify-common-7.0.3/cloudify/workflows/workflow_api.py
--rw-r--r--   0 root         (0) root         (0)    80337 2023-11-28 12:56:03.000000 cloudify-common-7.0.3/cloudify/workflows/workflow_context.py
--rw-r--r--   0 root         (0) root         (0)     1746 2023-11-28 12:56:03.000000 cloudify-common-7.0.3/cloudify/zip_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-28 12:56:21.793283 cloudify-common-7.0.3/cloudify_async_client/
--rw-r--r--   0 root         (0) root         (0)       69 2023-11-28 12:56:03.000000 cloudify-common-7.0.3/cloudify_async_client/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1258 2023-11-28 12:56:03.000000 cloudify-common-7.0.3/cloudify_async_client/audit_log.py
--rw-r--r--   0 root         (0) root         (0)     1530 2023-11-28 12:56:03.000000 cloudify-common-7.0.3/cloudify_async_client/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-28 12:56:21.793283 cloudify-common-7.0.3/cloudify_common.egg-info/
--rw-r--r--   0 root         (0) root         (0)      249 2023-11-28 12:56:21.000000 cloudify-common-7.0.3/cloudify_common.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4997 2023-11-28 12:56:21.000000 cloudify-common-7.0.3/cloudify_common.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-11-28 12:56:21.000000 cloudify-common-7.0.3/cloudify_common.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       51 2023-11-28 12:56:21.000000 cloudify-common-7.0.3/cloudify_common.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-11-28 12:56:21.000000 cloudify-common-7.0.3/cloudify_common.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      205 2023-11-28 12:56:21.000000 cloudify-common-7.0.3/cloudify_common.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       77 2023-11-28 12:56:21.000000 cloudify-common-7.0.3/cloudify_common.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-28 12:56:21.797283 cloudify-common-7.0.3/cloudify_rest_client/
--rw-r--r--   0 root         (0) root         (0)      731 2023-11-28 12:56:03.000000 cloudify-common-7.0.3/cloudify_rest_client/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4122 2023-11-28 12:56:03.000000 cloudify-common-7.0.3/cloudify_rest_client/_datetime_compat.py
--rw-r--r--   0 root         (0) root         (0)     8814 2023-11-28 12:56:03.000000 cloudify-common-7.0.3/cloudify_rest_client/agents.py
--rw-r--r--   0 root         (0) root         (0)     3565 2023-11-28 12:56:03.000000 cloudify-common-7.0.3/cloudify_rest_client/audit_log.py
--rw-r--r--   0 root         (0) root         (0)    25807 2023-11-28 12:56:03.000000 cloudify-common-7.0.3/cloudify_rest_client/blueprints.py
--rw-r--r--   0 root         (0) root         (0)     3857 2023-11-28 12:56:03.000000 cloudify-common-7.0.3/cloudify_rest_client/bytes_stream_utils.py
--rw-r--r--   0 root         (0) root         (0)    22799 2023-11-28 12:56:03.000000 cloudify-common-7.0.3/cloudify_rest_client/client.py
--rw-r--r--   0 root         (0) root         (0)     1009 2023-11-28 12:56:03.000000 cloudify-common-7.0.3/cloudify_rest_client/cluster.py
--rw-r--r--   0 root         (0) root         (0)     1205 2023-11-28 12:56:03.000000 cloudify-common-7.0.3/cloudify_rest_client/community_contacts.py
--rw-r--r--   0 root         (0) root         (0)      435 2023-11-28 12:56:03.000000 cloudify-common-7.0.3/cloudify_rest_client/constants.py
--rw-r--r--   0 root         (0) root         (0)     6367 2023-11-28 12:56:03.000000 cloudify-common-7.0.3/cloudify_rest_client/deployment_modifications.py
--rw-r--r--   0 root         (0) root         (0)    10221 2023-11-28 12:56:03.000000 cloudify-common-7.0.3/cloudify_rest_client/deployment_updates.py
--rw-r--r--   0 root         (0) root         (0)    38732 2023-11-28 12:56:03.000000 cloudify-common-7.0.3/cloudify_rest_client/deployments.py
--rw-r--r--   0 root         (0) root         (0)     1963 2023-11-28 12:56:03.000000 cloudify-common-7.0.3/cloudify_rest_client/evaluate.py
--rw-r--r--   0 root         (0) root         (0)    11374 2023-11-28 12:56:03.000000 cloudify-common-7.0.3/cloudify_rest_client/events.py
--rw-r--r--   0 root         (0) root         (0)    10493 2023-11-28 12:56:03.000000 cloudify-common-7.0.3/cloudify_rest_client/exceptions.py
--rw-r--r--   0 root         (0) root         (0)    12947 2023-11-28 12:56:03.000000 cloudify-common-7.0.3/cloudify_rest_client/execution_schedules.py
--rw-r--r--   0 root         (0) root         (0)    22148 2023-11-28 12:56:03.000000 cloudify-common-7.0.3/cloudify_rest_client/executions.py
--rw-r--r--   0 root         (0) root         (0)     6266 2023-11-28 12:56:03.000000 cloudify-common-7.0.3/cloudify_rest_client/filters.py
--rw-r--r--   0 root         (0) root         (0)      284 2023-11-28 12:56:03.000000 cloudify-common-7.0.3/cloudify_rest_client/idp.py
--rw-r--r--   0 root         (0) root         (0)    10537 2023-11-28 12:56:03.000000 cloudify-common-7.0.3/cloudify_rest_client/inter_deployment_dependencies.py
--rw-r--r--   0 root         (0) root         (0)     1852 2023-11-28 12:56:03.000000 cloudify-common-7.0.3/cloudify_rest_client/labels.py
--rw-r--r--   0 root         (0) root         (0)     3760 2023-11-28 12:56:03.000000 cloudify-common-7.0.3/cloudify_rest_client/ldap.py
--rw-r--r--   0 root         (0) root         (0)     2886 2023-11-28 12:56:03.000000 cloudify-common-7.0.3/cloudify_rest_client/license.py
--rw-r--r--   0 root         (0) root         (0)     5149 2023-11-28 12:56:03.000000 cloudify-common-7.0.3/cloudify_rest_client/log_bundles.py
--rw-r--r--   0 root         (0) root         (0)     2947 2023-11-28 12:56:03.000000 cloudify-common-7.0.3/cloudify_rest_client/maintenance.py
--rw-r--r--   0 root         (0) root         (0)    15074 2023-11-28 12:56:03.000000 cloudify-common-7.0.3/cloudify_rest_client/manager.py
--rw-r--r--   0 root         (0) root         (0)    13494 2023-11-28 12:56:03.000000 cloudify-common-7.0.3/cloudify_rest_client/node_instances.py
--rw-r--r--   0 root         (0) root         (0)    13368 2023-11-28 12:56:03.000000 cloudify-common-7.0.3/cloudify_rest_client/nodes.py
--rw-r--r--   0 root         (0) root         (0)    10417 2023-11-28 12:56:03.000000 cloudify-common-7.0.3/cloudify_rest_client/operations.py
--rw-r--r--   0 root         (0) root         (0)     2489 2023-11-28 12:56:03.000000 cloudify-common-7.0.3/cloudify_rest_client/permissions.py
--rw-r--r--   0 root         (0) root         (0)    17819 2023-11-28 12:56:03.000000 cloudify-common-7.0.3/cloudify_rest_client/plugins.py
--rw-r--r--   0 root         (0) root         (0)     8930 2023-11-28 12:56:03.000000 cloudify-common-7.0.3/cloudify_rest_client/plugins_update.py
--rw-r--r--   0 root         (0) root         (0)    11395 2023-11-28 12:56:03.000000 cloudify-common-7.0.3/cloudify_rest_client/resources.py
--rw-r--r--   0 root         (0) root         (0)     2800 2023-11-28 12:56:03.000000 cloudify-common-7.0.3/cloudify_rest_client/responses.py
--rw-r--r--   0 root         (0) root         (0)     9516 2023-11-28 12:56:03.000000 cloudify-common-7.0.3/cloudify_rest_client/secrets.py
--rw-r--r--   0 root         (0) root         (0)     7514 2023-11-28 12:56:03.000000 cloudify-common-7.0.3/cloudify_rest_client/secrets_providers.py
--rw-r--r--   0 root         (0) root         (0)     5680 2023-11-28 12:56:03.000000 cloudify-common-7.0.3/cloudify_rest_client/sites.py
--rw-r--r--   0 root         (0) root         (0)     8391 2023-11-28 12:56:03.000000 cloudify-common-7.0.3/cloudify_rest_client/snapshots.py
--rw-r--r--   0 root         (0) root         (0)     1708 2023-11-28 12:56:03.000000 cloudify-common-7.0.3/cloudify_rest_client/summary.py
--rw-r--r--   0 root         (0) root         (0)     7510 2023-11-28 12:56:03.000000 cloudify-common-7.0.3/cloudify_rest_client/tenants.py
--rw-r--r--   0 root         (0) root         (0)     2891 2023-11-28 12:56:03.000000 cloudify-common-7.0.3/cloudify_rest_client/tokens.py
--rw-r--r--   0 root         (0) root         (0)     4578 2023-11-28 12:56:03.000000 cloudify-common-7.0.3/cloudify_rest_client/user_groups.py
--rw-r--r--   0 root         (0) root         (0)     6921 2023-11-28 12:56:03.000000 cloudify-common-7.0.3/cloudify_rest_client/users.py
--rw-r--r--   0 root         (0) root         (0)     4873 2023-11-28 12:56:03.000000 cloudify-common-7.0.3/cloudify_rest_client/utils.py
--rw-r--r--   0 root         (0) root         (0)     1851 2023-11-28 12:56:03.000000 cloudify-common-7.0.3/cloudify_rest_client/workflows.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-28 12:56:21.797283 cloudify-common-7.0.3/ctx_wrappers/
--rw-r--r--   0 root         (0) root         (0)       71 2023-11-28 12:56:03.000000 cloudify-common-7.0.3/ctx_wrappers/ctx-sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-28 12:56:21.797283 cloudify-common-7.0.3/dsl_parser/
--rw-r--r--   0 root         (0) root         (0)      637 2023-11-28 12:56:03.000000 cloudify-common-7.0.3/dsl_parser/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4856 2023-11-28 12:56:03.000000 cloudify-common-7.0.3/dsl_parser/constants.py
--rw-r--r--   0 root         (0) root         (0)    19171 2023-11-28 12:56:03.000000 cloudify-common-7.0.3/dsl_parser/constraints.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-28 12:56:21.801283 cloudify-common-7.0.3/dsl_parser/elements/
--rw-r--r--   0 root         (0) root         (0)      712 2023-11-28 12:56:03.000000 cloudify-common-7.0.3/dsl_parser/elements/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5669 2023-11-28 12:56:03.000000 cloudify-common-7.0.3/dsl_parser/elements/blueprint.py
--rw-r--r--   0 root         (0) root         (0)    10177 2023-11-28 12:56:03.000000 cloudify-common-7.0.3/dsl_parser/elements/data_types.py
--rw-r--r--   0 root         (0) root         (0)     4985 2023-11-28 12:56:03.000000 cloudify-common-7.0.3/dsl_parser/elements/deployment_schedules.py
--rw-r--r--   0 root         (0) root         (0)    31837 2023-11-28 12:56:03.000000 cloudify-common-7.0.3/dsl_parser/elements/imports.py
--rw-r--r--   0 root         (0) root         (0)     6358 2023-11-28 12:56:03.000000 cloudify-common-7.0.3/dsl_parser/elements/inputs.py
--rw-r--r--   0 root         (0) root         (0)     6044 2023-11-28 12:56:03.000000 cloudify-common-7.0.3/dsl_parser/elements/misc.py
--rw-r--r--   0 root         (0) root         (0)    25808 2023-11-28 12:56:03.000000 cloudify-common-7.0.3/dsl_parser/elements/node_templates.py
--rw-r--r--   0 root         (0) root         (0)     3767 2023-11-28 12:56:03.000000 cloudify-common-7.0.3/dsl_parser/elements/node_types.py
--rw-r--r--   0 root         (0) root         (0)    15763 2023-11-28 12:56:03.000000 cloudify-common-7.0.3/dsl_parser/elements/operation.py
--rw-r--r--   0 root         (0) root         (0)     5413 2023-11-28 12:56:03.000000 cloudify-common-7.0.3/dsl_parser/elements/plugins.py
--rw-r--r--   0 root         (0) root         (0)    19699 2023-11-28 12:56:03.000000 cloudify-common-7.0.3/dsl_parser/elements/policies.py
--rw-r--r--   0 root         (0) root         (0)     4018 2023-11-28 12:56:03.000000 cloudify-common-7.0.3/dsl_parser/elements/relationships.py
--rw-r--r--   0 root         (0) root         (0)     6098 2023-11-28 12:56:03.000000 cloudify-common-7.0.3/dsl_parser/elements/scalable.py
--rw-r--r--   0 root         (0) root         (0)     2359 2023-11-28 12:56:03.000000 cloudify-common-7.0.3/dsl_parser/elements/types.py
--rw-r--r--   0 root         (0) root         (0)     1485 2023-11-28 12:56:03.000000 cloudify-common-7.0.3/dsl_parser/elements/version.py
--rw-r--r--   0 root         (0) root         (0)     8400 2023-11-28 12:56:03.000000 cloudify-common-7.0.3/dsl_parser/elements/workflows.py
--rw-r--r--   0 root         (0) root         (0)     5578 2023-11-28 12:56:03.000000 cloudify-common-7.0.3/dsl_parser/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-28 12:56:21.801283 cloudify-common-7.0.3/dsl_parser/framework/
--rw-r--r--   0 root         (0) root         (0)      637 2023-11-28 12:56:03.000000 cloudify-common-7.0.3/dsl_parser/framework/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7859 2023-11-28 12:56:03.000000 cloudify-common-7.0.3/dsl_parser/framework/elements.py
--rw-r--r--   0 root         (0) root         (0)    31720 2023-11-28 12:56:03.000000 cloudify-common-7.0.3/dsl_parser/framework/parser.py
--rw-r--r--   0 root         (0) root         (0)     1684 2023-11-28 12:56:03.000000 cloudify-common-7.0.3/dsl_parser/framework/requirements.py
--rw-r--r--   0 root         (0) root         (0)    72247 2023-11-28 12:56:03.000000 cloudify-common-7.0.3/dsl_parser/functions.py
--rw-r--r--   0 root         (0) root         (0)     5031 2023-11-28 12:56:03.000000 cloudify-common-7.0.3/dsl_parser/holder.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-28 12:56:21.801283 cloudify-common-7.0.3/dsl_parser/import_resolver/
--rw-r--r--   0 root         (0) root         (0)      637 2023-11-28 12:56:03.000000 cloudify-common-7.0.3/dsl_parser/import_resolver/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5209 2023-11-28 12:56:03.000000 cloudify-common-7.0.3/dsl_parser/import_resolver/abstract_import_resolver.py
--rw-r--r--   0 root         (0) root         (0)     7670 2023-11-28 12:56:03.000000 cloudify-common-7.0.3/dsl_parser/import_resolver/default_import_resolver.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-28 12:56:21.801283 cloudify-common-7.0.3/dsl_parser/interfaces/
--rw-r--r--   0 root         (0) root         (0)        0 2023-11-28 12:56:03.000000 cloudify-common-7.0.3/dsl_parser/interfaces/__init__.py
--rw-r--r--   0 root         (0) root         (0)      813 2023-11-28 12:56:03.000000 cloudify-common-7.0.3/dsl_parser/interfaces/constants.py
--rw-r--r--   0 root         (0) root         (0)     3932 2023-11-28 12:56:03.000000 cloudify-common-7.0.3/dsl_parser/interfaces/interfaces_merger.py
--rw-r--r--   0 root         (0) root         (0)     2339 2023-11-28 12:56:03.000000 cloudify-common-7.0.3/dsl_parser/interfaces/interfaces_parser.py
--rw-r--r--   0 root         (0) root         (0)    10119 2023-11-28 12:56:03.000000 cloudify-common-7.0.3/dsl_parser/interfaces/operation_merger.py
--rw-r--r--   0 root         (0) root         (0)     3934 2023-11-28 12:56:03.000000 cloudify-common-7.0.3/dsl_parser/interfaces/utils.py
--rw-r--r--   0 root         (0) root         (0)     1710 2023-11-28 12:56:03.000000 cloudify-common-7.0.3/dsl_parser/models.py
--rw-r--r--   0 root         (0) root         (0)     4636 2023-11-28 12:56:03.000000 cloudify-common-7.0.3/dsl_parser/multi_instance.py
--rw-r--r--   0 root         (0) root         (0)     5834 2023-11-28 12:56:03.000000 cloudify-common-7.0.3/dsl_parser/parser.py
--rw-r--r--   0 root         (0) root         (0)    43420 2023-11-28 12:56:03.000000 cloudify-common-7.0.3/dsl_parser/rel_graph.py
--rw-r--r--   0 root         (0) root         (0)     8644 2023-11-28 12:56:03.000000 cloudify-common-7.0.3/dsl_parser/scan.py
--rw-r--r--   0 root         (0) root         (0)    12442 2023-11-28 12:56:03.000000 cloudify-common-7.0.3/dsl_parser/tasks.py
--rw-r--r--   0 root         (0) root         (0)    18600 2023-11-28 12:56:03.000000 cloudify-common-7.0.3/dsl_parser/utils.py
--rw-r--r--   0 root         (0) root         (0)     4288 2023-11-28 12:56:03.000000 cloudify-common-7.0.3/dsl_parser/version.py
--rw-r--r--   0 root         (0) root         (0)     5530 2023-11-28 12:56:03.000000 cloudify-common-7.0.3/dsl_parser/yaml_loader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-28 12:56:21.801283 cloudify-common-7.0.3/script_runner/
--rw-r--r--   0 root         (0) root         (0)      637 2023-11-28 12:56:03.000000 cloudify-common-7.0.3/script_runner/__init__.py
--rw-r--r--   0 root         (0) root         (0)      124 2023-11-28 12:56:03.000000 cloudify-common-7.0.3/script_runner/constants.py
--rw-r--r--   0 root         (0) root         (0)      984 2023-11-28 12:56:03.000000 cloudify-common-7.0.3/script_runner/eval_env.py
--rw-r--r--   0 root         (0) root         (0)    16145 2023-11-28 12:56:03.000000 cloudify-common-7.0.3/script_runner/tasks.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-11-28 12:56:21.801283 cloudify-common-7.0.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1340 2023-11-28 12:56:03.000000 cloudify-common-7.0.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 13:11:11.103052 cloudify-common-7.0.4/
+-rw-r--r--   0 root         (0) root         (0)    10273 2024-04-07 13:02:26.000000 cloudify-common-7.0.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       39 2024-04-07 13:02:26.000000 cloudify-common-7.0.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      249 2024-04-07 13:11:11.103052 cloudify-common-7.0.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3034 2024-04-07 13:02:26.000000 cloudify-common-7.0.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 13:11:11.079052 cloudify-common-7.0.4/cloudify/
+-rw-r--r--   0 root         (0) root         (0)     2286 2024-04-07 13:02:26.000000 cloudify-common-7.0.4/cloudify/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5056 2024-04-07 13:02:26.000000 cloudify-common-7.0.4/cloudify/agent_utils.py
+-rw-r--r--   0 root         (0) root         (0)    30777 2024-04-07 13:02:26.000000 cloudify-common-7.0.4/cloudify/amqp_client.py
+-rw-r--r--   0 root         (0) root         (0)     7373 2024-04-07 13:02:26.000000 cloudify-common-7.0.4/cloudify/cluster.py
+-rw-r--r--   0 root         (0) root         (0)     1335 2024-04-07 13:02:26.000000 cloudify-common-7.0.4/cloudify/cluster_status.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 13:11:11.079052 cloudify-common-7.0.4/cloudify/compute/
+-rw-r--r--   0 root         (0) root         (0)     4460 2024-04-07 13:02:26.000000 cloudify-common-7.0.4/cloudify/compute/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1302 2024-04-07 13:02:26.000000 cloudify-common-7.0.4/cloudify/conflict_handlers.py
+-rw-r--r--   0 root         (0) root         (0)     4385 2024-04-07 13:02:26.000000 cloudify-common-7.0.4/cloudify/constants.py
+-rw-r--r--   0 root         (0) root         (0)    47193 2024-04-07 13:02:26.000000 cloudify-common-7.0.4/cloudify/context.py
+-rw-r--r--   0 root         (0) root         (0)     3855 2024-04-07 13:02:26.000000 cloudify-common-7.0.4/cloudify/cryptography_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 13:11:11.079052 cloudify-common-7.0.4/cloudify/ctx_wrappers/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-07 13:02:26.000000 cloudify-common-7.0.4/cloudify/ctx_wrappers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8328 2024-04-07 13:02:26.000000 cloudify-common-7.0.4/cloudify/ctx_wrappers/ctx-py.py
+-rw-r--r--   0 root         (0) root         (0)     4271 2024-04-07 13:02:26.000000 cloudify-common-7.0.4/cloudify/decorators.py
+-rw-r--r--   0 root         (0) root         (0)     3394 2024-04-07 13:02:26.000000 cloudify-common-7.0.4/cloudify/deployment_dependencies.py
+-rw-r--r--   0 root         (0) root         (0)    19061 2024-04-07 13:02:26.000000 cloudify-common-7.0.4/cloudify/dispatch.py
+-rw-r--r--   0 root         (0) root         (0)    19168 2024-04-07 13:02:26.000000 cloudify-common-7.0.4/cloudify/endpoint.py
+-rw-r--r--   0 root         (0) root         (0)     3741 2024-04-07 13:02:26.000000 cloudify-common-7.0.4/cloudify/error_handling.py
+-rw-r--r--   0 root         (0) root         (0)     4872 2024-04-07 13:02:26.000000 cloudify-common-7.0.4/cloudify/event.py
+-rw-r--r--   0 root         (0) root         (0)     5918 2024-04-07 13:02:26.000000 cloudify-common-7.0.4/cloudify/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)    16107 2024-04-07 13:02:26.000000 cloudify-common-7.0.4/cloudify/logs.py
+-rw-r--r--   0 root         (0) root         (0)    18303 2024-04-07 13:02:26.000000 cloudify-common-7.0.4/cloudify/manager.py
+-rw-r--r--   0 root         (0) root         (0)     7829 2024-04-07 13:02:26.000000 cloudify-common-7.0.4/cloudify/mocks.py
+-rw-r--r--   0 root         (0) root         (0)     4914 2024-04-07 13:02:26.000000 cloudify-common-7.0.4/cloudify/models_states.py
+-rw-r--r--   0 root         (0) root         (0)    25048 2024-04-07 13:02:26.000000 cloudify-common-7.0.4/cloudify/plugin_installer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 13:11:11.079052 cloudify-common-7.0.4/cloudify/plugins/
+-rw-r--r--   0 root         (0) root         (0)      643 2024-04-07 13:02:26.000000 cloudify-common-7.0.4/cloudify/plugins/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1213 2024-04-07 13:02:26.000000 cloudify-common-7.0.4/cloudify/plugins/install_utils.py
+-rw-r--r--   0 root         (0) root         (0)    53945 2024-04-07 13:02:26.000000 cloudify-common-7.0.4/cloudify/plugins/lifecycle.py
+-rw-r--r--   0 root         (0) root         (0)    59556 2024-04-07 13:02:26.000000 cloudify-common-7.0.4/cloudify/plugins/workflows.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 13:11:11.083052 cloudify-common-7.0.4/cloudify/proxy/
+-rw-r--r--   0 root         (0) root         (0)      637 2024-04-07 13:02:26.000000 cloudify-common-7.0.4/cloudify/proxy/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3965 2024-04-07 13:02:26.000000 cloudify-common-7.0.4/cloudify/proxy/client.py
+-rw-r--r--   0 root         (0) root         (0)     8157 2024-04-07 13:02:26.000000 cloudify-common-7.0.4/cloudify/proxy/server.py
+-rw-r--r--   0 root         (0) root         (0)     6223 2024-04-07 13:02:26.000000 cloudify-common-7.0.4/cloudify/rabbitmq_client.py
+-rw-r--r--   0 root         (0) root         (0)      782 2024-04-07 13:02:26.000000 cloudify-common-7.0.4/cloudify/snapshots.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 13:11:11.083052 cloudify-common-7.0.4/cloudify/snmp/
+-rw-r--r--   0 root         (0) root         (0)     5393 2024-04-07 13:02:26.000000 cloudify-common-7.0.4/cloudify/snmp/CLOUDIFY-MIB.mib
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-07 13:02:26.000000 cloudify-common-7.0.4/cloudify/snmp/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4934 2024-04-07 13:02:26.000000 cloudify-common-7.0.4/cloudify/snmp/snmp_trap.py
+-rw-r--r--   0 root         (0) root         (0)     3054 2024-04-07 13:02:26.000000 cloudify-common-7.0.4/cloudify/state.py
+-rw-r--r--   0 root         (0) root         (0)     2330 2024-04-07 13:02:26.000000 cloudify-common-7.0.4/cloudify/systemddbus.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 13:11:11.083052 cloudify-common-7.0.4/cloudify/test_utils/
+-rw-r--r--   0 root         (0) root         (0)      751 2024-04-07 13:02:26.000000 cloudify-common-7.0.4/cloudify/test_utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      999 2024-04-07 13:02:26.000000 cloudify-common-7.0.4/cloudify/test_utils/dispatch_helper.py
+-rw-r--r--   0 root         (0) root         (0)    11243 2024-04-07 13:02:26.000000 cloudify-common-7.0.4/cloudify/test_utils/local_workflow_decorator.py
+-rw-r--r--   0 root         (0) root         (0)     3892 2024-04-07 13:02:26.000000 cloudify-common-7.0.4/cloudify/test_utils/mock_rest_client.py
+-rw-r--r--   0 root         (0) root         (0)    38891 2024-04-07 13:02:26.000000 cloudify-common-7.0.4/cloudify/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 13:11:11.083052 cloudify-common-7.0.4/cloudify/workflows/
+-rw-r--r--   0 root         (0) root         (0)      848 2024-04-07 13:02:26.000000 cloudify-common-7.0.4/cloudify/workflows/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8618 2024-04-07 13:02:26.000000 cloudify-common-7.0.4/cloudify/workflows/amqp_dispatcher.py
+-rw-r--r--   0 root         (0) root         (0)     5562 2024-04-07 13:02:26.000000 cloudify-common-7.0.4/cloudify/workflows/events.py
+-rw-r--r--   0 root         (0) root         (0)    36444 2024-04-07 13:02:26.000000 cloudify-common-7.0.4/cloudify/workflows/local.py
+-rw-r--r--   0 root         (0) root         (0)    40724 2024-04-07 13:02:26.000000 cloudify-common-7.0.4/cloudify/workflows/tasks.py
+-rw-r--r--   0 root         (0) root         (0)    26098 2024-04-07 13:02:26.000000 cloudify-common-7.0.4/cloudify/workflows/tasks_graph.py
+-rw-r--r--   0 root         (0) root         (0)     2782 2024-04-07 13:02:26.000000 cloudify-common-7.0.4/cloudify/workflows/workflow_api.py
+-rw-r--r--   0 root         (0) root         (0)    80337 2024-04-07 13:02:26.000000 cloudify-common-7.0.4/cloudify/workflows/workflow_context.py
+-rw-r--r--   0 root         (0) root         (0)     1746 2024-04-07 13:02:26.000000 cloudify-common-7.0.4/cloudify/zip_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 13:11:11.087052 cloudify-common-7.0.4/cloudify_async_client/
+-rw-r--r--   0 root         (0) root         (0)       69 2024-04-07 13:02:26.000000 cloudify-common-7.0.4/cloudify_async_client/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1258 2024-04-07 13:02:26.000000 cloudify-common-7.0.4/cloudify_async_client/audit_log.py
+-rw-r--r--   0 root         (0) root         (0)     1530 2024-04-07 13:02:26.000000 cloudify-common-7.0.4/cloudify_async_client/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 13:11:11.087052 cloudify-common-7.0.4/cloudify_common.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      249 2024-04-07 13:11:11.000000 cloudify-common-7.0.4/cloudify_common.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4997 2024-04-07 13:11:11.000000 cloudify-common-7.0.4/cloudify_common.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-07 13:11:11.000000 cloudify-common-7.0.4/cloudify_common.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       51 2024-04-07 13:11:11.000000 cloudify-common-7.0.4/cloudify_common.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-07 13:02:45.000000 cloudify-common-7.0.4/cloudify_common.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      225 2024-04-07 13:11:11.000000 cloudify-common-7.0.4/cloudify_common.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       77 2024-04-07 13:11:11.000000 cloudify-common-7.0.4/cloudify_common.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 13:11:11.095052 cloudify-common-7.0.4/cloudify_rest_client/
+-rw-r--r--   0 root         (0) root         (0)      731 2024-04-07 13:02:26.000000 cloudify-common-7.0.4/cloudify_rest_client/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4122 2024-04-07 13:02:26.000000 cloudify-common-7.0.4/cloudify_rest_client/_datetime_compat.py
+-rw-r--r--   0 root         (0) root         (0)     8814 2024-04-07 13:02:26.000000 cloudify-common-7.0.4/cloudify_rest_client/agents.py
+-rw-r--r--   0 root         (0) root         (0)     3565 2024-04-07 13:02:26.000000 cloudify-common-7.0.4/cloudify_rest_client/audit_log.py
+-rw-r--r--   0 root         (0) root         (0)    25807 2024-04-07 13:02:26.000000 cloudify-common-7.0.4/cloudify_rest_client/blueprints.py
+-rw-r--r--   0 root         (0) root         (0)     3857 2024-04-07 13:02:26.000000 cloudify-common-7.0.4/cloudify_rest_client/bytes_stream_utils.py
+-rw-r--r--   0 root         (0) root         (0)    22798 2024-04-07 13:02:26.000000 cloudify-common-7.0.4/cloudify_rest_client/client.py
+-rw-r--r--   0 root         (0) root         (0)     1009 2024-04-07 13:02:26.000000 cloudify-common-7.0.4/cloudify_rest_client/cluster.py
+-rw-r--r--   0 root         (0) root         (0)     1205 2024-04-07 13:02:26.000000 cloudify-common-7.0.4/cloudify_rest_client/community_contacts.py
+-rw-r--r--   0 root         (0) root         (0)      435 2024-04-07 13:02:26.000000 cloudify-common-7.0.4/cloudify_rest_client/constants.py
+-rw-r--r--   0 root         (0) root         (0)     6367 2024-04-07 13:02:26.000000 cloudify-common-7.0.4/cloudify_rest_client/deployment_modifications.py
+-rw-r--r--   0 root         (0) root         (0)    10221 2024-04-07 13:02:26.000000 cloudify-common-7.0.4/cloudify_rest_client/deployment_updates.py
+-rw-r--r--   0 root         (0) root         (0)    38732 2024-04-07 13:02:26.000000 cloudify-common-7.0.4/cloudify_rest_client/deployments.py
+-rw-r--r--   0 root         (0) root         (0)     1963 2024-04-07 13:02:26.000000 cloudify-common-7.0.4/cloudify_rest_client/evaluate.py
+-rw-r--r--   0 root         (0) root         (0)    11374 2024-04-07 13:02:26.000000 cloudify-common-7.0.4/cloudify_rest_client/events.py
+-rw-r--r--   0 root         (0) root         (0)    10493 2024-04-07 13:02:26.000000 cloudify-common-7.0.4/cloudify_rest_client/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)    12947 2024-04-07 13:02:26.000000 cloudify-common-7.0.4/cloudify_rest_client/execution_schedules.py
+-rw-r--r--   0 root         (0) root         (0)    22589 2024-04-07 13:02:26.000000 cloudify-common-7.0.4/cloudify_rest_client/executions.py
+-rw-r--r--   0 root         (0) root         (0)     6266 2024-04-07 13:02:26.000000 cloudify-common-7.0.4/cloudify_rest_client/filters.py
+-rw-r--r--   0 root         (0) root         (0)      284 2024-04-07 13:02:26.000000 cloudify-common-7.0.4/cloudify_rest_client/idp.py
+-rw-r--r--   0 root         (0) root         (0)    10537 2024-04-07 13:02:26.000000 cloudify-common-7.0.4/cloudify_rest_client/inter_deployment_dependencies.py
+-rw-r--r--   0 root         (0) root         (0)     1852 2024-04-07 13:02:26.000000 cloudify-common-7.0.4/cloudify_rest_client/labels.py
+-rw-r--r--   0 root         (0) root         (0)     3760 2024-04-07 13:02:26.000000 cloudify-common-7.0.4/cloudify_rest_client/ldap.py
+-rw-r--r--   0 root         (0) root         (0)     2886 2024-04-07 13:02:26.000000 cloudify-common-7.0.4/cloudify_rest_client/license.py
+-rw-r--r--   0 root         (0) root         (0)     5149 2024-04-07 13:02:26.000000 cloudify-common-7.0.4/cloudify_rest_client/log_bundles.py
+-rw-r--r--   0 root         (0) root         (0)     2947 2024-04-07 13:02:26.000000 cloudify-common-7.0.4/cloudify_rest_client/maintenance.py
+-rw-r--r--   0 root         (0) root         (0)    15074 2024-04-07 13:02:26.000000 cloudify-common-7.0.4/cloudify_rest_client/manager.py
+-rw-r--r--   0 root         (0) root         (0)    13494 2024-04-07 13:02:26.000000 cloudify-common-7.0.4/cloudify_rest_client/node_instances.py
+-rw-r--r--   0 root         (0) root         (0)    13368 2024-04-07 13:02:26.000000 cloudify-common-7.0.4/cloudify_rest_client/nodes.py
+-rw-r--r--   0 root         (0) root         (0)    10417 2024-04-07 13:02:26.000000 cloudify-common-7.0.4/cloudify_rest_client/operations.py
+-rw-r--r--   0 root         (0) root         (0)     2489 2024-04-07 13:02:26.000000 cloudify-common-7.0.4/cloudify_rest_client/permissions.py
+-rw-r--r--   0 root         (0) root         (0)    17819 2024-04-07 13:02:26.000000 cloudify-common-7.0.4/cloudify_rest_client/plugins.py
+-rw-r--r--   0 root         (0) root         (0)     8930 2024-04-07 13:02:26.000000 cloudify-common-7.0.4/cloudify_rest_client/plugins_update.py
+-rw-r--r--   0 root         (0) root         (0)    11395 2024-04-07 13:02:26.000000 cloudify-common-7.0.4/cloudify_rest_client/resources.py
+-rw-r--r--   0 root         (0) root         (0)     2800 2024-04-07 13:02:26.000000 cloudify-common-7.0.4/cloudify_rest_client/responses.py
+-rw-r--r--   0 root         (0) root         (0)     9516 2024-04-07 13:02:26.000000 cloudify-common-7.0.4/cloudify_rest_client/secrets.py
+-rw-r--r--   0 root         (0) root         (0)     7514 2024-04-07 13:02:26.000000 cloudify-common-7.0.4/cloudify_rest_client/secrets_providers.py
+-rw-r--r--   0 root         (0) root         (0)     5680 2024-04-07 13:02:26.000000 cloudify-common-7.0.4/cloudify_rest_client/sites.py
+-rw-r--r--   0 root         (0) root         (0)     8479 2024-04-07 13:02:26.000000 cloudify-common-7.0.4/cloudify_rest_client/snapshots.py
+-rw-r--r--   0 root         (0) root         (0)     1708 2024-04-07 13:02:26.000000 cloudify-common-7.0.4/cloudify_rest_client/summary.py
+-rw-r--r--   0 root         (0) root         (0)     7510 2024-04-07 13:02:26.000000 cloudify-common-7.0.4/cloudify_rest_client/tenants.py
+-rw-r--r--   0 root         (0) root         (0)     2891 2024-04-07 13:02:26.000000 cloudify-common-7.0.4/cloudify_rest_client/tokens.py
+-rw-r--r--   0 root         (0) root         (0)     4578 2024-04-07 13:02:26.000000 cloudify-common-7.0.4/cloudify_rest_client/user_groups.py
+-rw-r--r--   0 root         (0) root         (0)     6921 2024-04-07 13:02:26.000000 cloudify-common-7.0.4/cloudify_rest_client/users.py
+-rw-r--r--   0 root         (0) root         (0)     4880 2024-04-07 13:02:26.000000 cloudify-common-7.0.4/cloudify_rest_client/utils.py
+-rw-r--r--   0 root         (0) root         (0)     1851 2024-04-07 13:02:26.000000 cloudify-common-7.0.4/cloudify_rest_client/workflows.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 13:11:11.095052 cloudify-common-7.0.4/ctx_wrappers/
+-rw-r--r--   0 root         (0) root         (0)       71 2024-04-07 13:02:26.000000 cloudify-common-7.0.4/ctx_wrappers/ctx-sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 13:11:11.099052 cloudify-common-7.0.4/dsl_parser/
+-rw-r--r--   0 root         (0) root         (0)      637 2024-04-07 13:02:27.000000 cloudify-common-7.0.4/dsl_parser/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4856 2024-04-07 13:02:27.000000 cloudify-common-7.0.4/dsl_parser/constants.py
+-rw-r--r--   0 root         (0) root         (0)    19171 2024-04-07 13:02:27.000000 cloudify-common-7.0.4/dsl_parser/constraints.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 13:11:11.103052 cloudify-common-7.0.4/dsl_parser/elements/
+-rw-r--r--   0 root         (0) root         (0)      712 2024-04-07 13:02:27.000000 cloudify-common-7.0.4/dsl_parser/elements/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5669 2024-04-07 13:02:27.000000 cloudify-common-7.0.4/dsl_parser/elements/blueprint.py
+-rw-r--r--   0 root         (0) root         (0)    10177 2024-04-07 13:02:27.000000 cloudify-common-7.0.4/dsl_parser/elements/data_types.py
+-rw-r--r--   0 root         (0) root         (0)     4985 2024-04-07 13:02:27.000000 cloudify-common-7.0.4/dsl_parser/elements/deployment_schedules.py
+-rw-r--r--   0 root         (0) root         (0)    31837 2024-04-07 13:02:27.000000 cloudify-common-7.0.4/dsl_parser/elements/imports.py
+-rw-r--r--   0 root         (0) root         (0)     6358 2024-04-07 13:02:27.000000 cloudify-common-7.0.4/dsl_parser/elements/inputs.py
+-rw-r--r--   0 root         (0) root         (0)     6044 2024-04-07 13:02:27.000000 cloudify-common-7.0.4/dsl_parser/elements/misc.py
+-rw-r--r--   0 root         (0) root         (0)    25808 2024-04-07 13:02:27.000000 cloudify-common-7.0.4/dsl_parser/elements/node_templates.py
+-rw-r--r--   0 root         (0) root         (0)     3767 2024-04-07 13:02:27.000000 cloudify-common-7.0.4/dsl_parser/elements/node_types.py
+-rw-r--r--   0 root         (0) root         (0)    15763 2024-04-07 13:02:27.000000 cloudify-common-7.0.4/dsl_parser/elements/operation.py
+-rw-r--r--   0 root         (0) root         (0)     5413 2024-04-07 13:02:27.000000 cloudify-common-7.0.4/dsl_parser/elements/plugins.py
+-rw-r--r--   0 root         (0) root         (0)    19699 2024-04-07 13:02:27.000000 cloudify-common-7.0.4/dsl_parser/elements/policies.py
+-rw-r--r--   0 root         (0) root         (0)     4018 2024-04-07 13:02:27.000000 cloudify-common-7.0.4/dsl_parser/elements/relationships.py
+-rw-r--r--   0 root         (0) root         (0)     6098 2024-04-07 13:02:27.000000 cloudify-common-7.0.4/dsl_parser/elements/scalable.py
+-rw-r--r--   0 root         (0) root         (0)     2359 2024-04-07 13:02:27.000000 cloudify-common-7.0.4/dsl_parser/elements/types.py
+-rw-r--r--   0 root         (0) root         (0)     1485 2024-04-07 13:02:27.000000 cloudify-common-7.0.4/dsl_parser/elements/version.py
+-rw-r--r--   0 root         (0) root         (0)     8400 2024-04-07 13:02:27.000000 cloudify-common-7.0.4/dsl_parser/elements/workflows.py
+-rw-r--r--   0 root         (0) root         (0)     5578 2024-04-07 13:02:27.000000 cloudify-common-7.0.4/dsl_parser/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 13:11:11.103052 cloudify-common-7.0.4/dsl_parser/framework/
+-rw-r--r--   0 root         (0) root         (0)      637 2024-04-07 13:02:27.000000 cloudify-common-7.0.4/dsl_parser/framework/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7859 2024-04-07 13:02:27.000000 cloudify-common-7.0.4/dsl_parser/framework/elements.py
+-rw-r--r--   0 root         (0) root         (0)    31720 2024-04-07 13:02:27.000000 cloudify-common-7.0.4/dsl_parser/framework/parser.py
+-rw-r--r--   0 root         (0) root         (0)     1684 2024-04-07 13:02:27.000000 cloudify-common-7.0.4/dsl_parser/framework/requirements.py
+-rw-r--r--   0 root         (0) root         (0)    72247 2024-04-07 13:02:27.000000 cloudify-common-7.0.4/dsl_parser/functions.py
+-rw-r--r--   0 root         (0) root         (0)     5031 2024-04-07 13:02:27.000000 cloudify-common-7.0.4/dsl_parser/holder.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 13:11:11.103052 cloudify-common-7.0.4/dsl_parser/import_resolver/
+-rw-r--r--   0 root         (0) root         (0)      637 2024-04-07 13:02:27.000000 cloudify-common-7.0.4/dsl_parser/import_resolver/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5209 2024-04-07 13:02:27.000000 cloudify-common-7.0.4/dsl_parser/import_resolver/abstract_import_resolver.py
+-rw-r--r--   0 root         (0) root         (0)     7670 2024-04-07 13:02:27.000000 cloudify-common-7.0.4/dsl_parser/import_resolver/default_import_resolver.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 13:11:11.103052 cloudify-common-7.0.4/dsl_parser/interfaces/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-07 13:02:27.000000 cloudify-common-7.0.4/dsl_parser/interfaces/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      813 2024-04-07 13:02:27.000000 cloudify-common-7.0.4/dsl_parser/interfaces/constants.py
+-rw-r--r--   0 root         (0) root         (0)     3932 2024-04-07 13:02:27.000000 cloudify-common-7.0.4/dsl_parser/interfaces/interfaces_merger.py
+-rw-r--r--   0 root         (0) root         (0)     2339 2024-04-07 13:02:27.000000 cloudify-common-7.0.4/dsl_parser/interfaces/interfaces_parser.py
+-rw-r--r--   0 root         (0) root         (0)    10119 2024-04-07 13:02:27.000000 cloudify-common-7.0.4/dsl_parser/interfaces/operation_merger.py
+-rw-r--r--   0 root         (0) root         (0)     3934 2024-04-07 13:02:27.000000 cloudify-common-7.0.4/dsl_parser/interfaces/utils.py
+-rw-r--r--   0 root         (0) root         (0)     1710 2024-04-07 13:02:27.000000 cloudify-common-7.0.4/dsl_parser/models.py
+-rw-r--r--   0 root         (0) root         (0)     4636 2024-04-07 13:02:27.000000 cloudify-common-7.0.4/dsl_parser/multi_instance.py
+-rw-r--r--   0 root         (0) root         (0)     5834 2024-04-07 13:02:27.000000 cloudify-common-7.0.4/dsl_parser/parser.py
+-rw-r--r--   0 root         (0) root         (0)    43420 2024-04-07 13:02:27.000000 cloudify-common-7.0.4/dsl_parser/rel_graph.py
+-rw-r--r--   0 root         (0) root         (0)     8644 2024-04-07 13:02:27.000000 cloudify-common-7.0.4/dsl_parser/scan.py
+-rw-r--r--   0 root         (0) root         (0)    12442 2024-04-07 13:02:27.000000 cloudify-common-7.0.4/dsl_parser/tasks.py
+-rw-r--r--   0 root         (0) root         (0)    18600 2024-04-07 13:02:27.000000 cloudify-common-7.0.4/dsl_parser/utils.py
+-rw-r--r--   0 root         (0) root         (0)     4288 2024-04-07 13:02:27.000000 cloudify-common-7.0.4/dsl_parser/version.py
+-rw-r--r--   0 root         (0) root         (0)     5530 2024-04-07 13:02:27.000000 cloudify-common-7.0.4/dsl_parser/yaml_loader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 13:11:11.103052 cloudify-common-7.0.4/script_runner/
+-rw-r--r--   0 root         (0) root         (0)      637 2024-04-07 13:02:27.000000 cloudify-common-7.0.4/script_runner/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      124 2024-04-07 13:02:27.000000 cloudify-common-7.0.4/script_runner/constants.py
+-rw-r--r--   0 root         (0) root         (0)      984 2024-04-07 13:02:27.000000 cloudify-common-7.0.4/script_runner/eval_env.py
+-rw-r--r--   0 root         (0) root         (0)    16145 2024-04-07 13:02:27.000000 cloudify-common-7.0.4/script_runner/tasks.py
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-07 13:11:11.107052 cloudify-common-7.0.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1371 2024-04-07 13:02:27.000000 cloudify-common-7.0.4/setup.py
```

### Comparing `cloudify-common-7.0.3/LICENSE` & `cloudify-common-7.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.3/README.md` & `cloudify-common-7.0.4/README.md`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.3/cloudify/__init__.py` & `cloudify-common-7.0.4/cloudify/__init__.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.3/cloudify/agent_utils.py` & `cloudify-common-7.0.4/cloudify/agent_utils.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.3/cloudify/amqp_client.py` & `cloudify-common-7.0.4/cloudify/amqp_client.py`

 * *Files 12% similar despite different names*

```diff
@@ -252,38 +252,38 @@
             try:
                 envelope = self._connection_tasks_queue.get_nowait()
             except queue.Empty:
                 return
 
             target_channel = envelope['channel'] or channel
             method = envelope['method']
-            # we use a separate queue to send any possible exceptions back
-            # to the calling thread - see the publish method
+            # we use a separate queue to send any possible results/exceptions
+            # back to the calling thread - see the publish method
             message = envelope['message']
-            err_queue = envelope.get('err_queue')
+            response_queue = envelope.get('response_queue')
 
             try:
                 if callable(method):
-                    method(self, channel, **message)
+                    result = method(self, channel, **message)
                 else:
-                    getattr(target_channel, method)(**message)
+                    result = getattr(target_channel, method)(**message)
             except pika.exceptions.ConnectionClosed:
                 if self._closed:
                     return
                 # if we couldn't send the message because the connection
                 # was down, requeue it to be sent again later
                 self._connection_tasks_queue.put(envelope)
                 raise
             except Exception as e:
-                if err_queue:
-                    err_queue.put(e)
+                if response_queue:
+                    response_queue.put(e)
                 raise
             else:
-                if err_queue:
-                    err_queue.put(None)
+                if response_queue:
+                    response_queue.put(result)
 
     def close(self, wait=True):
         self._closed = True
         if self._consumer_thread and wait:
             self._consumer_thread.join()
             self._consumer_thread = None
 
@@ -305,34 +305,37 @@
         Use this to schedule a channel method such as .publish or .basic_ack
         to be called from the connection thread.
         """
         if wait and self._consumer_thread \
                 and self._consumer_thread is threading.current_thread():
             # when sending from the connection thread, we can't wait because
             # then we wouldn't allow the actual send loop (._process_publish)
-            # to run, because we'd block on the err_queue here
+            # to run, because we'd block on the response_queue here
             raise RuntimeError(
                 'Cannot wait when sending from the connection thread')
 
         # the message is going to be sent from another thread (the .consume
-        # thread). If an error happens there, we must have a way to get it
-        # back out, so we pass a Queue together with the message, that will
-        # contain either an exception instance, or None
-        err_queue = queue.Queue() if wait else None
+        # thread). If operation has a result or an error happens there,
+        # we must have a way to get it back out, so we pass a Queue together
+        # with the message, that will contain operation result or
+        # an exception instance
+        response_queue = queue.Queue() if wait else None
         envelope = {
             'method': method,
             'message': kwargs,
-            'err_queue': err_queue,
+            'response_queue': response_queue,
             'channel': channel
         }
         self._connection_tasks_queue.put(envelope)
-        if err_queue:
-            err = err_queue.get(timeout=timeout)
-            if isinstance(err, Exception):
-                raise err
+        if response_queue:
+            response_or_err = response_queue.get(timeout=timeout)
+            if isinstance(response_or_err, Exception):
+                raise response_or_err
+            else:
+                return response_or_err
 
     def publish(self, message, wait=True, timeout=None):
         """Schedule a message to be sent.
 
         :param message: Kwargs for the pika basic_publish call. Should at
                         least contain the "body" and "exchange" keys, and
                         it might contain other keys such as "routing_key"
@@ -367,22 +370,152 @@
 STOP_AGENT = object()
 
 
 class TaskConsumer(object):
     routing_key = ''
     late_ack = False
 
-    def __init__(self, queue, threadpool_size=5, exchange_type='direct'):
+    def __init__(
+        self,
+        queue,
+        threadpool_size=5,
+        watchdog_period=180,
+        exchange_type='direct',
+    ):
         self.threadpool_size = threadpool_size
         self.exchange = queue
         self.queue = '{0}_{1}'.format(queue, self.routing_key)
         self._sem = threading.Semaphore(threadpool_size)
         self._connection = None
+        self._channel = None
         self.exchange_type = exchange_type
         self._tasks_buffer = deque()
+        self._last_processing_time_lock = threading.Lock()
+        self._last_processing_time = None
+        self._watchdog_period = watchdog_period
+        self._watchdog_thread = threading.Thread(
+            target=self._watch_tasks_processing
+        )
+        self._watchdog_thread.daemon = True
+        self._watchdog_thread.start()
+
+    def _set_last_processing_time(self, new_value):
+        with self._last_processing_time_lock:
+            self._last_processing_time = new_value
+
+    def _get_last_processing_time(self):
+        with self._last_processing_time_lock:
+            return self._last_processing_time
+
+    def _watch_tasks_processing(self):
+        """
+        This is the target function for the watchdog thread.
+        The purpose of this thread is to help prevent possible
+        deadlocks that could occur if a given task spawns more
+        tasks than the thread pool size can handle. To address this,
+        the watchdog will spawn additional worker thread(s) outside
+        the semaphore control, since threads from the pool could hang
+        while waiting for results of dependent tasks.
+
+        Watchdog algorithm:
+        1. Check the stamp of the last task execution.
+        2. If it is not older than the configured period, go idle.
+        3. If the task buffer is not empty, pick a task from the buffer,
+            spawn a worker thread for that task, then go idle.
+        4. If the task buffer was empty, attempt to pull a single message
+            directly from the RabbitMQ channel. If there are no pending
+            messages in RabbitMQ, go idle. It means there is no more
+            pending tasks. Otherwise, spawn a worker thread
+            for the task related to the pulled message and then go idle.
+        After any idle state, start again from point 1.
+
+        Unfortunately, it cannot distinguish deadlocks from long-running tasks.
+        In that case, the watchdog thread will gradually spawn threads for the
+        remaining pending tasks.
+        """
+        while True:
+            if self._is_watchdog_idle():
+                time.sleep(self._watchdog_period)
+                continue
+
+            buffered_task = self._get_task_from_buffer()
+            if buffered_task is not None:
+                self._run_task(buffered_task, threadpool_worker=False)
+                logger.info(
+                    '%s watchdog: Spawned thread for task %s and '
+                    'delivery tag %s based on message pulled from '
+                    'tasks buffer. Going idle for %s seconds',
+                    self.__class__.__name__, buffered_task[2],
+                    buffered_task[3], self._watchdog_period
+                )
+                time.sleep(self._watchdog_period)
+                continue
+
+            # despite tasks buffer being empty, we still have a deadlock e.g.
+            # when rabbitmq's prefetch_count is same (or smaller)
+            # comparing to threadpool size and late_ack is enabled, so
+            # rabbitmq won't send any new message before
+            # at least one ack happen
+
+            get_ok, properties, body = self._connection.channel_method(
+                'basic_get', channel=self._channel,
+                queue=self.queue, auto_ack=False,
+            )
+            if get_ok is None:
+                logger.debug(
+                    '%s watchdog: Going idle for %s seconds, '
+                    'rabbitmq channel was empty',
+                    self.__class__.__name__, self._watchdog_period
+                )
+                time.sleep(self._watchdog_period)
+                continue
+
+            full_task = json.loads(body.decode('utf-8'))
+            task_args = (
+                self._channel, properties, full_task, get_ok.delivery_tag
+            )
+            self._run_task(task_args, threadpool_worker=False)
+            logger.info(
+                '%s watchdog: Spawned thread for task %s and delivery tag %s'
+                ' based on message pulled directly from rabbitmq channel. '
+                'Going idle for %s seconds',
+                self.__class__.__name__, full_task,
+                get_ok.delivery_tag, self._watchdog_period
+            )
+            time.sleep(self._watchdog_period)
+
+    def _is_watchdog_idle(self):
+        if self._connection is None or self._channel is None:
+            logger.debug(
+                '%s watchdog: rabbitmq connection and/or channel '
+                'was not set up yet. Going idle for %s seconds',
+                self.__class__.__name__, self._watchdog_period
+            )
+            return True
+
+        last_time = self._get_last_processing_time()
+        if last_time is None:
+            logger.debug(
+                '%s watchdog: there was not task execution yet. '
+                'Going idle for %s seconds',
+                self.__class__.__name__, self._watchdog_period
+            )
+            return True
+
+        last_execution_ago = time.monotonic() - last_time
+        if last_execution_ago < self._watchdog_period:
+            logger.debug(
+                '%s watchdog: recent task execution took place %s '
+                'seconds ago. Going idle for %s seconds',
+                self.__class__.__name__, last_execution_ago,
+                self._watchdog_period
+            )
+            return True
+
+        return False
 
     def register(self, connection, channel):
         self._connection = connection
         channel.basic_qos(prefetch_count=self.threadpool_size)
         channel.confirm_delivery()
         channel.exchange_declare(exchange=self.exchange,
                                  auto_delete=False,
@@ -394,41 +527,85 @@
         channel.queue_bind(queue=self.queue,
                            exchange=self.exchange,
                            routing_key=self.routing_key)
         if OLD_PIKA:
             channel.basic_consume(self.process, self.queue)
         else:
             channel.basic_consume(self.queue, self.process)
+        self._channel = channel
 
     def process(self, channel, method, properties, body):
         try:
             full_task = json.loads(body.decode('utf-8'))
         except ValueError:
             logger.error('Error parsing task: {0}'.format(body))
             return
 
         task_args = (channel, properties, full_task, method.delivery_tag)
         if self._sem.acquire(blocking=False):
-            self._run_task(task_args)
+            self._run_task(task_args, threadpool_worker=True)
         else:
             self._tasks_buffer.append(task_args)
 
-    def _process_message(self, channel, properties, full_task, delivery_tag):
+    def _watchdog_worker(
+        self,
+        channel,
+        properties,
+        full_task,
+        delivery_tag,
+    ):
+        self._set_last_processing_time(time.monotonic())
+        self._process_message(channel, properties, full_task, delivery_tag)
+
+    def _threadpool_worker(
+        self,
+        channel,
+        properties,
+        full_task,
+        delivery_tag,
+    ):
+        self._set_last_processing_time(time.monotonic())
+        self._process_message(channel, properties, full_task, delivery_tag)
+        buffered_task = self._get_task_from_buffer()
+        if buffered_task is not None:
+            self._run_task(buffered_task, threadpool_worker=True)
+        else:
+            self._sem.release()
+
+    def _process_message(
+        self,
+        channel,
+        properties,
+        full_task,
+        delivery_tag,
+    ):
+        logger.debug(
+            '%s started processing task %s, delivery_tag: %s',
+            self.__class__.__name__, full_task, delivery_tag
+        )
         if not self.late_ack:
             self._connection.ack(channel, delivery_tag)
+            logger.debug(
+                '%s gave ACK on task %s delivery_tag: %s',
+                self.__class__.__name__, full_task, delivery_tag
+            )
         try:
             result = self.handle_task(full_task)
         except Exception as e:
             result = {'ok': False, 'error': repr(e)}
             logger.exception(
                 'ERROR - failed message processing: '
                 '{0!r}\nbody: {1}'.format(e, full_task)
             )
         if self.late_ack:
             self._connection.ack(channel, delivery_tag)
+            logger.debug(
+                '%s gave ACK on task %s delivery_tag: %s',
+                self.__class__.__name__, full_task, delivery_tag
+            )
         if properties.reply_to:
             if result is NO_RESPONSE:
                 self.delete_queue(properties.reply_to)
             else:
                 if result is STOP_AGENT:
                     body = json.dumps({'ok': True})
                 else:
@@ -439,33 +616,32 @@
                     'properties': pika.BasicProperties(
                         correlation_id=properties.correlation_id),
                     'body': body
                 })
         if result is STOP_AGENT:
             # the operation asked us to exit, so drop everything and exit
             os._exit(0)
-        if not self._maybe_run_next_task():
-            self._sem.release()
 
-    def _run_task(self, task_args):
+    def _run_task(self, task_args, threadpool_worker=True):
+        if threadpool_worker:
+            target = self._threadpool_worker
+        else:
+            target = self._watchdog_worker
         new_thread = threading.Thread(
-            target=self._process_message,
+            target=target,
             args=task_args
         )
         new_thread.daemon = True
         new_thread.start()
 
-    def _maybe_run_next_task(self):
+    def _get_task_from_buffer(self):
         try:
-            task_args = self._tasks_buffer.popleft()
+            return self._tasks_buffer.popleft()
         except IndexError:
-            return False
-        else:
-            self._run_task(task_args)
-            return True
+            return None
 
     def handle_task(self, full_task):
         raise NotImplementedError()
 
     def delete_queue(self, queue, if_empty=True, wait=True):
         self._connection.channel_method(
             'queue_delete', queue=queue, if_empty=if_empty, wait=wait)
```

### Comparing `cloudify-common-7.0.3/cloudify/cluster_status.py` & `cloudify-common-7.0.4/cloudify/cluster_status.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.3/cloudify/compute/__init__.py` & `cloudify-common-7.0.4/cloudify/compute/__init__.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.3/cloudify/conflict_handlers.py` & `cloudify-common-7.0.4/cloudify/conflict_handlers.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.3/cloudify/constants.py` & `cloudify-common-7.0.4/cloudify/constants.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.3/cloudify/context.py` & `cloudify-common-7.0.4/cloudify/context.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.3/cloudify/cryptography_utils.py` & `cloudify-common-7.0.4/cloudify/cryptography_utils.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.3/cloudify/ctx_wrappers/ctx-py.py` & `cloudify-common-7.0.4/cloudify/ctx_wrappers/ctx-py.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.3/cloudify/decorators.py` & `cloudify-common-7.0.4/cloudify/decorators.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.3/cloudify/deployment_dependencies.py` & `cloudify-common-7.0.4/cloudify/deployment_dependencies.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.3/cloudify/dispatch.py` & `cloudify-common-7.0.4/cloudify/dispatch.py`

 * *Files 2% similar despite different names*

```diff
@@ -442,28 +442,31 @@
     logs.setup_subprocess_logger()
     _update_logging_level()
 
 
 def _update_logging_level():
     if not os.path.isfile(LOGGING_CONFIG_FILE):
         return
-    with open(LOGGING_CONFIG_FILE, 'r') as config_file:
-        config_lines = config_file.readlines()
-    for line in config_lines:
-        if not line.strip() or line.startswith('#'):
-            continue
-        level_name, logger_name = line.split()
-        level_id = logging.getLevelName(level_name.upper())
-        if not isinstance(level_id, int):
-            continue
-        logging.getLogger(logger_name).setLevel(level_id)
+    with open(LOGGING_CONFIG_FILE) as config_file:
+        for line in config_file:
+            line = line.strip()
+            if not line or line.startswith('#'):
+                continue
+            parts = line.split()
+            if not len(parts) == 2:
+                continue
+            level_name, logger_name = parts
+            level_id = logging.getLevelName(level_name.upper())
+            if not isinstance(level_id, int):
+                continue
+            logging.getLogger(logger_name).setLevel(level_id)
 
 
 def main():
-    dispatch_dir = sys.argv[1]
+    dispatch_dir = os.path.abspath(sys.argv[1])
     with open(os.path.join(dispatch_dir, 'input.json')) as f:
         dispatch_inputs = json.load(f)
     cloudify_context = dispatch_inputs['cloudify_context']
     args = dispatch_inputs['args']
     kwargs = dispatch_inputs['kwargs']
     dispatch_type = cloudify_context['type']
     threading.current_thread().name = f'Dispatch-{dispatch_type}'
```

### Comparing `cloudify-common-7.0.3/cloudify/endpoint.py` & `cloudify-common-7.0.4/cloudify/endpoint.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.3/cloudify/error_handling.py` & `cloudify-common-7.0.4/cloudify/error_handling.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.3/cloudify/event.py` & `cloudify-common-7.0.4/cloudify/event.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.3/cloudify/exceptions.py` & `cloudify-common-7.0.4/cloudify/exceptions.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.3/cloudify/logs.py` & `cloudify-common-7.0.4/cloudify/logs.py`

 * *Files 4% similar despite different names*

```diff
@@ -385,25 +385,35 @@
     # silence pika and http loggers so that even if the agent is logging on
     # DEBUG, we're not getting all the uninteresting AMQP/HTTP information
     logging.getLogger('pika').setLevel(logging.WARNING)
     logging.getLogger('cloudify.rest_client.http').setLevel(logging.INFO)
 
 
 def setup_subprocess_logger():
-    setup_logger_base(os.environ.get(ENV_AGENT_LOG_LEVEL) or 'DEBUG',
-                      os.environ.get(ENV_AGENT_LOG_DIR))
+    log_dir = os.environ.get(ENV_AGENT_LOG_DIR)
+    if log_dir and os.path.exists(log_dir):
+        log_dir = os.path.abspath(log_dir)
+    else:
+        log_dir = None
+
+    setup_logger_base(
+        os.environ.get(ENV_AGENT_LOG_LEVEL) or 'DEBUG',
+        log_dir,
+    )
 
 
 def setup_agent_logger(log_name, log_level=None, log_dir=None,
                        max_bytes=None, max_history=None):
     if log_level is None:
         log_level = os.environ.get(ENV_AGENT_LOG_LEVEL) or 'DEBUG'
 
     if log_dir is None:
         log_dir = os.environ.get(ENV_AGENT_LOG_DIR)
+        if log_dir:
+            log_dir = os.path.realpath(os.path.abspath(log_dir), strict=True)
 
     setup_logger_base(log_level, log_dir)
 
     worker_logger = logging.getLogger('worker')
     dispatch_logger = logging.getLogger('dispatch')
 
     for logger in [worker_logger, dispatch_logger]:
```

### Comparing `cloudify-common-7.0.3/cloudify/manager.py` & `cloudify-common-7.0.4/cloudify/manager.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.3/cloudify/mocks.py` & `cloudify-common-7.0.4/cloudify/mocks.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.3/cloudify/models_states.py` & `cloudify-common-7.0.4/cloudify/models_states.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.3/cloudify/plugin_installer.py` & `cloudify-common-7.0.4/cloudify/plugin_installer.py`

 * *Files 2% similar despite different names*

```diff
@@ -616,14 +616,18 @@
         executables = {
             self._main_version: sys.executable,
         }
         executable_filename = os.path.basename(sys.executable)
         # examine all directories in PATH for executables named the same
         # as the executable we're running, so either `python` or `Python.exe`
         for path in os.environ['PATH'].split(os.pathsep):
+            if path and os.path.exists(path):
+                path = os.path.abspath(path)
+            else:
+                continue
             target_executable = os.path.join(path, executable_filename)
             version = self._get_executable_version(target_executable)
             if not version or version in executables:
                 continue
             executables[version] = target_executable
         return executables
```

### Comparing `cloudify-common-7.0.3/cloudify/plugins/__init__.py` & `cloudify-common-7.0.4/cloudify/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.3/cloudify/plugins/install_utils.py` & `cloudify-common-7.0.4/cloudify/plugins/install_utils.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.3/cloudify/plugins/lifecycle.py` & `cloudify-common-7.0.4/cloudify/plugins/lifecycle.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.3/cloudify/plugins/workflows.py` & `cloudify-common-7.0.4/cloudify/plugins/workflows.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.3/cloudify/proxy/__init__.py` & `cloudify-common-7.0.4/cloudify/proxy/__init__.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.3/cloudify/proxy/client.py` & `cloudify-common-7.0.4/cloudify/proxy/client.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.3/cloudify/proxy/server.py` & `cloudify-common-7.0.4/cloudify/proxy/server.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.3/cloudify/rabbitmq_client.py` & `cloudify-common-7.0.4/cloudify/rabbitmq_client.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.3/cloudify/snapshots.py` & `cloudify-common-7.0.4/cloudify/snapshots.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.3/cloudify/snmp/CLOUDIFY-MIB.mib` & `cloudify-common-7.0.4/cloudify/snmp/CLOUDIFY-MIB.mib`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.3/cloudify/snmp/snmp_trap.py` & `cloudify-common-7.0.4/cloudify/snmp/snmp_trap.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.3/cloudify/state.py` & `cloudify-common-7.0.4/cloudify/state.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.3/cloudify/systemddbus.py` & `cloudify-common-7.0.4/cloudify/systemddbus.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.3/cloudify/test_utils/__init__.py` & `cloudify-common-7.0.4/cloudify/test_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.3/cloudify/test_utils/dispatch_helper.py` & `cloudify-common-7.0.4/cloudify/test_utils/dispatch_helper.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.3/cloudify/test_utils/local_workflow_decorator.py` & `cloudify-common-7.0.4/cloudify/test_utils/local_workflow_decorator.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.3/cloudify/test_utils/mock_rest_client.py` & `cloudify-common-7.0.4/cloudify/test_utils/mock_rest_client.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.3/cloudify/utils.py` & `cloudify-common-7.0.4/cloudify/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -252,29 +252,44 @@
     )
 
 
 def get_manager_rest_service_host():
     """
     Returns the host the manager REST service is running on.
     """
-    if os.environ.get(constants.REST_HOST_KEY):
-        return os.environ[constants.REST_HOST_KEY].split(',')
+    environ_rest_host = os.environ.get(constants.REST_HOST_KEY)
+    # hostnames must be ascii, otherwise they're invalid
+    if environ_rest_host and environ_rest_host.isprintable():
+        hosts = []
+        for host in environ_rest_host.split(','):
+            host = host.strip()
+            # hostnames must not have spaces in them
+            if ' ' in host:
+                continue
+            hosts.append(host)
+        # if we seem to have 64 hosts, surely that's an invalid/malformed
+        # input, and we should not use that
+        if 0 < len(hosts) < 64:
+            return hosts
     try:
         # Context could be not available sometimes
         return _get_current_context().rest_host
     except RuntimeError:
         pass
 
 
 def get_manager_rest_service_port():
     """
     Returns the port the manager REST service is running on.
     """
-    if os.environ.get(constants.REST_PORT_KEY):
-        return int(os.environ[constants.REST_PORT_KEY])
+    environ_rest_port = os.environ.get(constants.REST_PORT_KEY)
+    if environ_rest_port and environ_rest_port.isdigit():
+        rest_port = int(environ_rest_port)
+        if 0 < rest_port < 65536:
+            return rest_port
     try:
         return _get_current_context().rest_port
     except RuntimeError:
         pass
 
 
 def get_broker_ssl_cert_path():
@@ -288,31 +303,36 @@
 get_manager_ip = get_manager_rest_service_host
 
 
 def get_local_rest_certificate():
     """
     Returns the path to the local copy of the server's public certificate
     """
+    ssl_cert_key_path = os.environ[constants.LOCAL_REST_CERT_FILE_KEY]
+    if not os.path.isfile(ssl_cert_key_path):
+        raise RuntimeError(f'Local REST certificate file not found, is '
+                           f'{constants.LOCAL_REST_CERT_FILE_KEY} environment '
+                           f'variable set?')
+
     ssl_cert_path = os.path.join(
-        os.path.dirname(os.environ[constants.LOCAL_REST_CERT_FILE_KEY]),
+        os.path.dirname(ssl_cert_key_path),
         'tmp_cloudify_internal_cert.pem'
     )
     ssl_cert_content = None
     try:
         ssl_cert_content = \
             _get_current_context().rest_ssl_cert if \
             hasattr(_get_current_context(), 'rest_ssl_cert') else None
     except RuntimeError:
         pass
     if ssl_cert_content:
         with open(ssl_cert_path, 'w') as f:
             f.write(ssl_cert_content)
 
-    return ssl_cert_path if ssl_cert_content \
-        else os.environ[constants.LOCAL_REST_CERT_FILE_KEY]
+    return ssl_cert_path if ssl_cert_content else ssl_cert_key_path
 
 
 def _get_current_context():
     for context in [ctx, workflow_ctx]:
         try:
             return context._get_current_object()
         except RuntimeError:
@@ -406,15 +426,18 @@
 def get_exec_tempdir():
     """
     Returns the directory to use for temporary files, when the intention
     is to place an executable file there.
     This is needed because some production systems disallow executions from
     the default temporary directory.
     """
-    return os.environ.get(ENV_CFY_EXEC_TEMPDIR) or tempfile.gettempdir()
+    exec_tempdir = os.environ.get(ENV_CFY_EXEC_TEMPDIR)
+    if exec_tempdir and os.path.exists(exec_tempdir):
+        return os.path.abspath(exec_tempdir)
+    return tempfile.gettempdir()
 
 
 def create_temp_folder():
     """
     Create a temporary folder.
     """
     path_join = os.path.join(get_exec_tempdir(), id_generator(5))
@@ -886,15 +909,18 @@
 
 
 def _plugins_base_dir():
     """The directory where plugins/ and source_plugins/ are stored.
 
     Default to sys.prefix, which is going to be in the mgmtworker/agent venv.
     """
-    return os.environ.get('CFY_PLUGINS_ROOT') or sys.prefix
+    plugins_root = os.environ.get('CFY_PLUGINS_ROOT')
+    if plugins_root and os.path.exists(plugins_root):
+        return os.path.abspath(plugins_root)
+    return sys.prefix
 
 
 def plugin_prefix(name, tenant_name, version=None, deployment_id=None):
     """Virtualenv for the specified plugin.
 
     If version is not provided, the highest version is used.
```

### Comparing `cloudify-common-7.0.3/cloudify/workflows/__init__.py` & `cloudify-common-7.0.4/cloudify/workflows/__init__.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.3/cloudify/workflows/amqp_dispatcher.py` & `cloudify-common-7.0.4/cloudify/workflows/amqp_dispatcher.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.3/cloudify/workflows/events.py` & `cloudify-common-7.0.4/cloudify/workflows/events.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.3/cloudify/workflows/local.py` & `cloudify-common-7.0.4/cloudify/workflows/local.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.3/cloudify/workflows/tasks.py` & `cloudify-common-7.0.4/cloudify/workflows/tasks.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.3/cloudify/workflows/tasks_graph.py` & `cloudify-common-7.0.4/cloudify/workflows/tasks_graph.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.3/cloudify/workflows/workflow_api.py` & `cloudify-common-7.0.4/cloudify/workflows/workflow_api.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.3/cloudify/workflows/workflow_context.py` & `cloudify-common-7.0.4/cloudify/workflows/workflow_context.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.3/cloudify/zip_utils.py` & `cloudify-common-7.0.4/cloudify/zip_utils.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.3/cloudify_async_client/audit_log.py` & `cloudify-common-7.0.4/cloudify_async_client/audit_log.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.3/cloudify_async_client/client.py` & `cloudify-common-7.0.4/cloudify_async_client/client.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.3/cloudify_common.egg-info/SOURCES.txt` & `cloudify-common-7.0.4/cloudify_common.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.3/cloudify_rest_client/__init__.py` & `cloudify-common-7.0.4/cloudify_rest_client/__init__.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.3/cloudify_rest_client/_datetime_compat.py` & `cloudify-common-7.0.4/cloudify_rest_client/_datetime_compat.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.3/cloudify_rest_client/agents.py` & `cloudify-common-7.0.4/cloudify_rest_client/agents.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.3/cloudify_rest_client/audit_log.py` & `cloudify-common-7.0.4/cloudify_rest_client/audit_log.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.3/cloudify_rest_client/blueprints.py` & `cloudify-common-7.0.4/cloudify_rest_client/blueprints.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.3/cloudify_rest_client/bytes_stream_utils.py` & `cloudify-common-7.0.4/cloudify_rest_client/bytes_stream_utils.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.3/cloudify_rest_client/client.py` & `cloudify-common-7.0.4/cloudify_rest_client/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,15 +89,15 @@
                  username=None, password=None, token=None, tenant=None,
                  kerberos_env=None, timeout=None, session=None):
         self.port = port
         self.host = ipv6_url_compat(host)
         self.protocol = protocol
         self.api_version = api_version
         self.kerberos_env = kerberos_env
-        self.default_timeout_sec = timeout or (5, None)
+        self.default_timeout_sec = timeout or (5, 300)
 
         self.headers = headers.copy() if headers else {}
         if not self.headers.get('Content-type'):
             self.headers['Content-type'] = 'application/json'
         self.query_params = query_params.copy() if query_params else {}
         self.logger = logging.getLogger('cloudify.rest_client.http')
         self.cert = cert
@@ -436,15 +436,15 @@
         :param trust_all: if `False`, the server's certificate
                           (self-signed or not) will be verified.
         :param username: Cloudify User username.
         :param password: Cloudify User password.
         :param token: Cloudify User token.
         :param tenant: Cloudify Tenant name.
         :param timeout: Requests timeout value. If not set, will default to
-                        (5, None)- 5 seconds connect timeout, no read timeout.
+                        (5, 300)- 5 seconds connect timeout, 300 read timeout.
         :param session: a requests.Session to use for all HTTP calls
         :return: Cloudify client instance.
         """
 
         if not port:
             if protocol == SECURED_PROTOCOL:
                 # SSL
```

### Comparing `cloudify-common-7.0.3/cloudify_rest_client/cluster.py` & `cloudify-common-7.0.4/cloudify_rest_client/cluster.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.3/cloudify_rest_client/community_contacts.py` & `cloudify-common-7.0.4/cloudify_rest_client/community_contacts.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.3/cloudify_rest_client/deployment_modifications.py` & `cloudify-common-7.0.4/cloudify_rest_client/deployment_modifications.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.3/cloudify_rest_client/deployment_updates.py` & `cloudify-common-7.0.4/cloudify_rest_client/deployment_updates.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.3/cloudify_rest_client/deployments.py` & `cloudify-common-7.0.4/cloudify_rest_client/deployments.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.3/cloudify_rest_client/evaluate.py` & `cloudify-common-7.0.4/cloudify_rest_client/evaluate.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.3/cloudify_rest_client/events.py` & `cloudify-common-7.0.4/cloudify_rest_client/events.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.3/cloudify_rest_client/exceptions.py` & `cloudify-common-7.0.4/cloudify_rest_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.3/cloudify_rest_client/execution_schedules.py` & `cloudify-common-7.0.4/cloudify_rest_client/execution_schedules.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.3/cloudify_rest_client/executions.py` & `cloudify-common-7.0.4/cloudify_rest_client/executions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import warnings
 
+from cloudify.models_states import ExecutionState
 from cloudify_rest_client import utils
 from cloudify_rest_client.exceptions import CloudifyClientError
 from cloudify_rest_client.responses import ListResponse
 
 
 class Execution(dict):
     """Cloudify workflow execution."""
@@ -595,15 +596,28 @@
 
         :param entities: An iterable (e.g. a list) of dictionaries describing
          executions to be restored.
         :param logger: A logger instance.
         """
         for entity in entities:
             entity['execution_id'] = entity.pop('id')
-            entity['force_status'] = entity.pop('status')
+            entity['force_status'], entity['error'] = \
+                restore_status_error_mapped(
+                    entity.pop('status'),
+                    entity.pop('error'),
+                )
             entity['dry_run'] = entity.pop('is_dry_run')
             entity['deployment_id'] = entity['deployment_id'] or ''
             try:
                 self.create(**entity)
             except CloudifyClientError as exc:
                 logger.error("Error restoring execution "
                              f"{entity['execution_id']}: {exc}")
+
+
+def restore_status_error_mapped(status, error):
+    if status in ExecutionState.IN_PROGRESS_STATES:
+        return (
+            ExecutionState.CANCELLED,
+            "Marked as cancelled by snapshot restore",
+        )
+    return status, error
```

### Comparing `cloudify-common-7.0.3/cloudify_rest_client/filters.py` & `cloudify-common-7.0.4/cloudify_rest_client/filters.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.3/cloudify_rest_client/inter_deployment_dependencies.py` & `cloudify-common-7.0.4/cloudify_rest_client/inter_deployment_dependencies.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.3/cloudify_rest_client/labels.py` & `cloudify-common-7.0.4/cloudify_rest_client/labels.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.3/cloudify_rest_client/ldap.py` & `cloudify-common-7.0.4/cloudify_rest_client/ldap.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.3/cloudify_rest_client/license.py` & `cloudify-common-7.0.4/cloudify_rest_client/license.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.3/cloudify_rest_client/log_bundles.py` & `cloudify-common-7.0.4/cloudify_rest_client/log_bundles.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.3/cloudify_rest_client/maintenance.py` & `cloudify-common-7.0.4/cloudify_rest_client/maintenance.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.3/cloudify_rest_client/manager.py` & `cloudify-common-7.0.4/cloudify_rest_client/manager.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.3/cloudify_rest_client/node_instances.py` & `cloudify-common-7.0.4/cloudify_rest_client/node_instances.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.3/cloudify_rest_client/nodes.py` & `cloudify-common-7.0.4/cloudify_rest_client/nodes.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.3/cloudify_rest_client/operations.py` & `cloudify-common-7.0.4/cloudify_rest_client/operations.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.3/cloudify_rest_client/permissions.py` & `cloudify-common-7.0.4/cloudify_rest_client/permissions.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.3/cloudify_rest_client/plugins.py` & `cloudify-common-7.0.4/cloudify_rest_client/plugins.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.3/cloudify_rest_client/plugins_update.py` & `cloudify-common-7.0.4/cloudify_rest_client/plugins_update.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.3/cloudify_rest_client/resources.py` & `cloudify-common-7.0.4/cloudify_rest_client/resources.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.3/cloudify_rest_client/responses.py` & `cloudify-common-7.0.4/cloudify_rest_client/responses.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.3/cloudify_rest_client/secrets.py` & `cloudify-common-7.0.4/cloudify_rest_client/secrets.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.3/cloudify_rest_client/secrets_providers.py` & `cloudify-common-7.0.4/cloudify_rest_client/secrets_providers.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.3/cloudify_rest_client/sites.py` & `cloudify-common-7.0.4/cloudify_rest_client/sites.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.3/cloudify_rest_client/snapshots.py` & `cloudify-common-7.0.4/cloudify_rest_client/snapshots.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,15 +110,16 @@
     def create(self,
                snapshot_id,
                include_credentials,
                include_logs=True,
                include_events=True,
                queue=False,
                tempdir_path=None,
-               legacy=True):
+               legacy=True,
+               listener_timeout=None):
         """
         Creates a new snapshot.
 
         :param snapshot_id: Snapshot id of the snapshot that will be created.
         :return: The created snapshot.
         """
         assert snapshot_id
@@ -126,14 +127,15 @@
         params = {
             'include_credentials': include_credentials,
             'include_logs': include_logs,
             'include_events': include_events,
             'queue': queue,
             'tempdir_path': tempdir_path,
             'legacy': legacy,
+            'listener_timeout': listener_timeout,
         }
         response = self.api.put(uri, data=params, expected_status_code=201)
         return Execution(response)
 
     def delete(self, snapshot_id):
         """
         Deletes the snapshot whose id matches the provided snapshot id.
```

### Comparing `cloudify-common-7.0.3/cloudify_rest_client/summary.py` & `cloudify-common-7.0.4/cloudify_rest_client/summary.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.3/cloudify_rest_client/tenants.py` & `cloudify-common-7.0.4/cloudify_rest_client/tenants.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.3/cloudify_rest_client/tokens.py` & `cloudify-common-7.0.4/cloudify_rest_client/tokens.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.3/cloudify_rest_client/user_groups.py` & `cloudify-common-7.0.4/cloudify_rest_client/user_groups.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.3/cloudify_rest_client/users.py` & `cloudify-common-7.0.4/cloudify_rest_client/users.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.3/cloudify_rest_client/utils.py` & `cloudify-common-7.0.4/cloudify_rest_client/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,17 +87,18 @@
 # Copied verbatim from distutils.spawn, since we don't always ship distutils.
 def find_executable(executable, path=None):
     """Tries to find 'executable' in the directories listed in 'path'.
 
     A string listing directories separated by 'os.pathsep'; defaults to
     os.environ['PATH'].  Returns the complete filename or None if not found.
     """
-    if path is None:
-        path = os.environ['PATH']
-    paths = path.split(os.pathsep)
+    if path:
+        paths = path.split(os.pathsep)
+    else:
+        paths = os.get_exec_path()
     base, ext = os.path.splitext(executable)
     if (sys.platform == 'win32') and (ext != '.exe'):
         executable = executable + '.exe'
     if not os.path.isfile(executable):
         for p in paths:
             f = os.path.join(p, executable)
             if os.path.isfile(f):
```

### Comparing `cloudify-common-7.0.3/cloudify_rest_client/workflows.py` & `cloudify-common-7.0.4/cloudify_rest_client/workflows.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.3/dsl_parser/__init__.py` & `cloudify-common-7.0.4/dsl_parser/__init__.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.3/dsl_parser/constants.py` & `cloudify-common-7.0.4/dsl_parser/constants.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.3/dsl_parser/constraints.py` & `cloudify-common-7.0.4/dsl_parser/constraints.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.3/dsl_parser/elements/__init__.py` & `cloudify-common-7.0.4/dsl_parser/elements/__init__.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.3/dsl_parser/elements/blueprint.py` & `cloudify-common-7.0.4/dsl_parser/elements/blueprint.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.3/dsl_parser/elements/data_types.py` & `cloudify-common-7.0.4/dsl_parser/elements/data_types.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.3/dsl_parser/elements/deployment_schedules.py` & `cloudify-common-7.0.4/dsl_parser/elements/deployment_schedules.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.3/dsl_parser/elements/imports.py` & `cloudify-common-7.0.4/dsl_parser/elements/imports.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.3/dsl_parser/elements/inputs.py` & `cloudify-common-7.0.4/dsl_parser/elements/inputs.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.3/dsl_parser/elements/misc.py` & `cloudify-common-7.0.4/dsl_parser/elements/misc.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.3/dsl_parser/elements/node_templates.py` & `cloudify-common-7.0.4/dsl_parser/elements/node_templates.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.3/dsl_parser/elements/node_types.py` & `cloudify-common-7.0.4/dsl_parser/elements/node_types.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.3/dsl_parser/elements/operation.py` & `cloudify-common-7.0.4/dsl_parser/elements/operation.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.3/dsl_parser/elements/plugins.py` & `cloudify-common-7.0.4/dsl_parser/elements/plugins.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.3/dsl_parser/elements/policies.py` & `cloudify-common-7.0.4/dsl_parser/elements/policies.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.3/dsl_parser/elements/relationships.py` & `cloudify-common-7.0.4/dsl_parser/elements/relationships.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.3/dsl_parser/elements/scalable.py` & `cloudify-common-7.0.4/dsl_parser/elements/scalable.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.3/dsl_parser/elements/types.py` & `cloudify-common-7.0.4/dsl_parser/elements/types.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.3/dsl_parser/elements/version.py` & `cloudify-common-7.0.4/dsl_parser/elements/version.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.3/dsl_parser/elements/workflows.py` & `cloudify-common-7.0.4/dsl_parser/elements/workflows.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.3/dsl_parser/exceptions.py` & `cloudify-common-7.0.4/dsl_parser/exceptions.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.3/dsl_parser/framework/__init__.py` & `cloudify-common-7.0.4/dsl_parser/framework/__init__.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.3/dsl_parser/framework/elements.py` & `cloudify-common-7.0.4/dsl_parser/framework/elements.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.3/dsl_parser/framework/parser.py` & `cloudify-common-7.0.4/dsl_parser/framework/parser.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.3/dsl_parser/framework/requirements.py` & `cloudify-common-7.0.4/dsl_parser/framework/requirements.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.3/dsl_parser/functions.py` & `cloudify-common-7.0.4/dsl_parser/functions.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.3/dsl_parser/holder.py` & `cloudify-common-7.0.4/dsl_parser/holder.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.3/dsl_parser/import_resolver/__init__.py` & `cloudify-common-7.0.4/dsl_parser/import_resolver/__init__.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.3/dsl_parser/import_resolver/abstract_import_resolver.py` & `cloudify-common-7.0.4/dsl_parser/import_resolver/abstract_import_resolver.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.3/dsl_parser/import_resolver/default_import_resolver.py` & `cloudify-common-7.0.4/dsl_parser/import_resolver/default_import_resolver.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.3/dsl_parser/interfaces/constants.py` & `cloudify-common-7.0.4/dsl_parser/interfaces/constants.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.3/dsl_parser/interfaces/interfaces_merger.py` & `cloudify-common-7.0.4/dsl_parser/interfaces/interfaces_merger.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.3/dsl_parser/interfaces/interfaces_parser.py` & `cloudify-common-7.0.4/dsl_parser/interfaces/interfaces_parser.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.3/dsl_parser/interfaces/operation_merger.py` & `cloudify-common-7.0.4/dsl_parser/interfaces/operation_merger.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.3/dsl_parser/interfaces/utils.py` & `cloudify-common-7.0.4/dsl_parser/interfaces/utils.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.3/dsl_parser/models.py` & `cloudify-common-7.0.4/dsl_parser/models.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.3/dsl_parser/multi_instance.py` & `cloudify-common-7.0.4/dsl_parser/multi_instance.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.3/dsl_parser/parser.py` & `cloudify-common-7.0.4/dsl_parser/parser.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.3/dsl_parser/rel_graph.py` & `cloudify-common-7.0.4/dsl_parser/rel_graph.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.3/dsl_parser/scan.py` & `cloudify-common-7.0.4/dsl_parser/scan.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.3/dsl_parser/tasks.py` & `cloudify-common-7.0.4/dsl_parser/tasks.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.3/dsl_parser/utils.py` & `cloudify-common-7.0.4/dsl_parser/utils.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.3/dsl_parser/version.py` & `cloudify-common-7.0.4/dsl_parser/version.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.3/dsl_parser/yaml_loader.py` & `cloudify-common-7.0.4/dsl_parser/yaml_loader.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.3/script_runner/__init__.py` & `cloudify-common-7.0.4/script_runner/__init__.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.3/script_runner/eval_env.py` & `cloudify-common-7.0.4/script_runner/eval_env.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.3/script_runner/tasks.py` & `cloudify-common-7.0.4/script_runner/tasks.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.3/setup.py` & `cloudify-common-7.0.4/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name='cloudify-common',
-    version='7.0.3',
+    version='7.0.4',
     author='Cloudify',
     author_email='cosmo-admin@cloudify.co',
     packages=find_packages(
         exclude=(
             'cloudify.tests*',
             'cloudify_rest_client.tests*',
             'dsl_parser.tests*',
@@ -15,23 +15,24 @@
         )
     ),
     include_package_data=True,
     license='LICENSE',
     description='Cloudify Common',
     zip_safe=False,
     install_requires=[
-        'aiohttp>=3.8.5,<4',
+        'aiohttp>=3.9.1,<4',
         'bottle<1',
         'distro>=1.7.0,<2',
         'fasteners<1',
         'jinja2>3,<4',
         'pika<2',
         'proxy_tools<1',
         'pytz',
-        'requests<3',
+        'urllib3>=2.0.7',
+        'requests>=2.31.0,<3',
         'requests_toolbelt>=1,<2',
         'wagon>=1,<2',
     ],
     python_requires='>=3.6',
     entry_points={
         'console_scripts': [
             'ctx = cloudify.proxy.client:main',
@@ -41,15 +42,15 @@
     scripts=[
         'ctx_wrappers/ctx-sh',
     ],
     extras_require={
         # for running workflows (in the mgmtworker and the cli), as opposed
         # to e.g. just executing operations (in the agent)
         'dispatcher': [
-            'PyYAML==6.0.1',
+            'PyYAML>6,<7',
             'networkx>2,<3',
         ],
         'snmp': [
-            'pysnmp==4.4.5',
+            'pysnmp>4,<5',
         ]
     }
 )
```

