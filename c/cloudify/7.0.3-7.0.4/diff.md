# Comparing `tmp/cloudify-7.0.3.tar.gz` & `tmp/cloudify-7.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudify-7.0.3.tar", last modified: Tue Nov 28 12:52:23 2023, max compression
+gzip compressed data, was "cloudify-7.0.4.tar", last modified: Sun Apr  7 14:35:41 2024, max compression
```

## Comparing `cloudify-7.0.3.tar` & `cloudify-7.0.4.tar`

### file list

```diff
@@ -1,79 +1,78 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-28 12:52:23.963725 cloudify-7.0.3/
--rw-r--r--   0 root         (0) root         (0)    11325 2023-11-28 12:52:05.000000 cloudify-7.0.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)      189 2023-11-28 12:52:23.963725 cloudify-7.0.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      591 2023-11-28 12:52:05.000000 cloudify-7.0.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-28 12:52:23.959725 cloudify-7.0.3/cloudify.egg-info/
--rw-r--r--   0 root         (0) root         (0)      189 2023-11-28 12:52:23.000000 cloudify-7.0.3/cloudify.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2162 2023-11-28 12:52:23.000000 cloudify-7.0.3/cloudify.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-11-28 12:52:23.000000 cloudify-7.0.3/cloudify.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       47 2023-11-28 12:52:23.000000 cloudify-7.0.3/cloudify.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      145 2023-11-28 12:52:23.000000 cloudify-7.0.3/cloudify.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-11-28 12:52:23.000000 cloudify-7.0.3/cloudify.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-28 12:52:23.959725 cloudify-7.0.3/cloudify_cli/
--rw-r--r--   0 root         (0) root         (0)      641 2023-11-28 12:52:05.000000 cloudify-7.0.3/cloudify_cli/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-28 12:52:23.959725 cloudify-7.0.3/cloudify_cli/async_commands/
--rw-r--r--   0 root         (0) root         (0)        0 2023-11-28 12:52:05.000000 cloudify-7.0.3/cloudify_cli/async_commands/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2275 2023-11-28 12:52:05.000000 cloudify-7.0.3/cloudify_cli/async_commands/audit_log.py
--rw-r--r--   0 root         (0) root         (0)     6759 2023-11-28 12:52:05.000000 cloudify-7.0.3/cloudify_cli/blueprint.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-28 12:52:23.959725 cloudify-7.0.3/cloudify_cli/cli/
--rw-r--r--   0 root         (0) root         (0)      641 2023-11-28 12:52:05.000000 cloudify-7.0.3/cloudify_cli/cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)    78946 2023-11-28 12:52:05.000000 cloudify-7.0.3/cloudify_cli/cli/cfy.py
--rw-r--r--   0 root         (0) root         (0)     1967 2023-11-28 12:52:05.000000 cloudify-7.0.3/cloudify_cli/cli/completion_utils.py
--rw-r--r--   0 root         (0) root         (0)    31948 2023-11-28 12:52:05.000000 cloudify-7.0.3/cloudify_cli/cli/helptexts.py
--rw-r--r--   0 root         (0) root         (0)     6054 2023-11-28 12:52:05.000000 cloudify-7.0.3/cloudify_cli/colorful_event.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-28 12:52:23.963725 cloudify-7.0.3/cloudify_cli/commands/
--rw-r--r--   0 root         (0) root         (0)      641 2023-11-28 12:52:05.000000 cloudify-7.0.3/cloudify_cli/commands/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16037 2023-11-28 12:52:05.000000 cloudify-7.0.3/cloudify_cli/commands/agents.py
--rw-r--r--   0 root         (0) root         (0)    10374 2023-11-28 12:52:05.000000 cloudify-7.0.3/cloudify_cli/commands/apply.py
--rw-r--r--   0 root         (0) root         (0)     5480 2023-11-28 12:52:05.000000 cloudify-7.0.3/cloudify_cli/commands/audit_log.py
--rw-r--r--   0 root         (0) root         (0)    31561 2023-11-28 12:52:05.000000 cloudify-7.0.3/cloudify_cli/commands/blueprints.py
--rw-r--r--   0 root         (0) root         (0)    14297 2023-11-28 12:52:05.000000 cloudify-7.0.3/cloudify_cli/commands/certificates.py
--rw-r--r--   0 root         (0) root         (0)    16691 2023-11-28 12:52:05.000000 cloudify-7.0.3/cloudify_cli/commands/cluster.py
--rw-r--r--   0 root         (0) root         (0)     1359 2023-11-28 12:52:05.000000 cloudify-7.0.3/cloudify_cli/commands/community.py
--rw-r--r--   0 root         (0) root         (0)     2404 2023-11-28 12:52:05.000000 cloudify-7.0.3/cloudify_cli/commands/config.py
--rw-r--r--   0 root         (0) root         (0)    72161 2023-11-28 12:52:05.000000 cloudify-7.0.3/cloudify_cli/commands/deployments.py
--rw-r--r--   0 root         (0) root         (0)    12209 2023-11-28 12:52:05.000000 cloudify-7.0.3/cloudify_cli/commands/events.py
--rw-r--r--   0 root         (0) root         (0)    33757 2023-11-28 12:52:05.000000 cloudify-7.0.3/cloudify_cli/commands/executions.py
--rw-r--r--   0 root         (0) root         (0)     2785 2023-11-28 12:52:05.000000 cloudify-7.0.3/cloudify_cli/commands/groups.py
--rw-r--r--   0 root         (0) root         (0)      383 2023-11-28 12:52:05.000000 cloudify-7.0.3/cloudify_cli/commands/idp.py
--rw-r--r--   0 root         (0) root         (0)     6587 2023-11-28 12:52:05.000000 cloudify-7.0.3/cloudify_cli/commands/init.py
--rw-r--r--   0 root         (0) root         (0)     8223 2023-11-28 12:52:05.000000 cloudify-7.0.3/cloudify_cli/commands/install.py
--rw-r--r--   0 root         (0) root         (0)     3166 2023-11-28 12:52:05.000000 cloudify-7.0.3/cloudify_cli/commands/ldap.py
--rw-r--r--   0 root         (0) root         (0)     4505 2023-11-28 12:52:05.000000 cloudify-7.0.3/cloudify_cli/commands/license.py
--rw-r--r--   0 root         (0) root         (0)     3984 2023-11-28 12:52:05.000000 cloudify-7.0.3/cloudify_cli/commands/log_bundles.py
--rw-r--r--   0 root         (0) root         (0)     5465 2023-11-28 12:52:05.000000 cloudify-7.0.3/cloudify_cli/commands/maintenance_mode.py
--rw-r--r--   0 root         (0) root         (0)    10411 2023-11-28 12:52:05.000000 cloudify-7.0.3/cloudify_cli/commands/node_instances.py
--rw-r--r--   0 root         (0) root         (0)     8827 2023-11-28 12:52:05.000000 cloudify-7.0.3/cloudify_cli/commands/nodes.py
--rw-r--r--   0 root         (0) root         (0)     1909 2023-11-28 12:52:05.000000 cloudify-7.0.3/cloudify_cli/commands/permissions.py
--rw-r--r--   0 root         (0) root         (0)    41310 2023-11-28 12:52:05.000000 cloudify-7.0.3/cloudify_cli/commands/plugins.py
--rw-r--r--   0 root         (0) root         (0)    27830 2023-11-28 12:52:05.000000 cloudify-7.0.3/cloudify_cli/commands/profiles.py
--rw-r--r--   0 root         (0) root         (0)    21581 2023-11-28 12:52:05.000000 cloudify-7.0.3/cloudify_cli/commands/secrets.py
--rw-r--r--   0 root         (0) root         (0)     5512 2023-11-28 12:52:05.000000 cloudify-7.0.3/cloudify_cli/commands/sites.py
--rw-r--r--   0 root         (0) root         (0)    10099 2023-11-28 12:52:05.000000 cloudify-7.0.3/cloudify_cli/commands/snapshots.py
--rw-r--r--   0 root         (0) root         (0)     2419 2023-11-28 12:52:05.000000 cloudify-7.0.3/cloudify_cli/commands/status.py
--rw-r--r--   0 root         (0) root         (0)     2264 2023-11-28 12:52:05.000000 cloudify-7.0.3/cloudify_cli/commands/summary.py
--rw-r--r--   0 root         (0) root         (0)    10822 2023-11-28 12:52:05.000000 cloudify-7.0.3/cloudify_cli/commands/tenants.py
--rw-r--r--   0 root         (0) root         (0)     2866 2023-11-28 12:52:05.000000 cloudify-7.0.3/cloudify_cli/commands/tokens.py
--rw-r--r--   0 root         (0) root         (0)     4293 2023-11-28 12:52:05.000000 cloudify-7.0.3/cloudify_cli/commands/uninstall.py
--rw-r--r--   0 root         (0) root         (0)     6937 2023-11-28 12:52:05.000000 cloudify-7.0.3/cloudify_cli/commands/user_groups.py
--rw-r--r--   0 root         (0) root         (0)     9355 2023-11-28 12:52:05.000000 cloudify-7.0.3/cloudify_cli/commands/users.py
--rw-r--r--   0 root         (0) root         (0)     5644 2023-11-28 12:52:05.000000 cloudify-7.0.3/cloudify_cli/commands/workflows.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-28 12:52:23.963725 cloudify-7.0.3/cloudify_cli/config/
--rw-r--r--   0 root         (0) root         (0)      641 2023-11-28 12:52:05.000000 cloudify-7.0.3/cloudify_cli/config/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4228 2023-11-28 12:52:05.000000 cloudify-7.0.3/cloudify_cli/config/config.py
--rw-r--r--   0 root         (0) root         (0)     2812 2023-11-28 12:52:05.000000 cloudify-7.0.3/cloudify_cli/constants.py
--rw-r--r--   0 root         (0) root         (0)    22806 2023-11-28 12:52:05.000000 cloudify-7.0.3/cloudify_cli/env.py
--rw-r--r--   0 root         (0) root         (0)     1498 2023-11-28 12:52:05.000000 cloudify-7.0.3/cloudify_cli/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     9183 2023-11-28 12:52:05.000000 cloudify-7.0.3/cloudify_cli/execution_events_fetcher.py
--rw-r--r--   0 root         (0) root         (0)    13653 2023-11-28 12:52:05.000000 cloudify-7.0.3/cloudify_cli/filters_utils.py
--rw-r--r--   0 root         (0) root         (0)     6006 2023-11-28 12:52:05.000000 cloudify-7.0.3/cloudify_cli/inputs.py
--rw-r--r--   0 root         (0) root         (0)     5989 2023-11-28 12:52:05.000000 cloudify-7.0.3/cloudify_cli/labels_utils.py
--rw-r--r--   0 root         (0) root         (0)     8492 2023-11-28 12:52:05.000000 cloudify-7.0.3/cloudify_cli/local.py
--rw-r--r--   0 root         (0) root         (0)     6868 2023-11-28 12:52:05.000000 cloudify-7.0.3/cloudify_cli/logger.py
--rw-r--r--   0 root         (0) root         (0)    13189 2023-11-28 12:52:05.000000 cloudify-7.0.3/cloudify_cli/main.py
--rw-r--r--   0 root         (0) root         (0)    54445 2023-11-28 12:52:05.000000 cloudify-7.0.3/cloudify_cli/prettytable.py
--rw-r--r--   0 root         (0) root         (0)    10905 2023-11-28 12:52:05.000000 cloudify-7.0.3/cloudify_cli/replace_certificates_config.py
--rw-r--r--   0 root         (0) root         (0)     6697 2023-11-28 12:52:05.000000 cloudify-7.0.3/cloudify_cli/table.py
--rw-r--r--   0 root         (0) root         (0)    16280 2023-11-28 12:52:05.000000 cloudify-7.0.3/cloudify_cli/utils.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-11-28 12:52:23.963725 cloudify-7.0.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1427 2023-11-28 12:52:05.000000 cloudify-7.0.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 14:35:41.403734 cloudify-7.0.4/
+-rw-r--r--   0 root         (0) root         (0)    11325 2024-04-07 14:32:13.000000 cloudify-7.0.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      189 2024-04-07 14:35:41.403734 cloudify-7.0.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      591 2024-04-07 14:32:13.000000 cloudify-7.0.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 14:35:41.395734 cloudify-7.0.4/cloudify.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      189 2024-04-07 14:35:41.000000 cloudify-7.0.4/cloudify.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2125 2024-04-07 14:35:41.000000 cloudify-7.0.4/cloudify.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-07 14:35:41.000000 cloudify-7.0.4/cloudify.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       47 2024-04-07 14:35:41.000000 cloudify-7.0.4/cloudify.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      145 2024-04-07 14:35:41.000000 cloudify-7.0.4/cloudify.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2024-04-07 14:35:41.000000 cloudify-7.0.4/cloudify.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 14:35:41.399734 cloudify-7.0.4/cloudify_cli/
+-rw-r--r--   0 root         (0) root         (0)      641 2024-04-07 14:32:13.000000 cloudify-7.0.4/cloudify_cli/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 14:35:41.399734 cloudify-7.0.4/cloudify_cli/async_commands/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-07 14:32:13.000000 cloudify-7.0.4/cloudify_cli/async_commands/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2275 2024-04-07 14:32:13.000000 cloudify-7.0.4/cloudify_cli/async_commands/audit_log.py
+-rw-r--r--   0 root         (0) root         (0)     6759 2024-04-07 14:32:13.000000 cloudify-7.0.4/cloudify_cli/blueprint.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 14:35:41.399734 cloudify-7.0.4/cloudify_cli/cli/
+-rw-r--r--   0 root         (0) root         (0)      641 2024-04-07 14:32:13.000000 cloudify-7.0.4/cloudify_cli/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    79115 2024-04-07 14:32:13.000000 cloudify-7.0.4/cloudify_cli/cli/cfy.py
+-rw-r--r--   0 root         (0) root         (0)    32455 2024-04-07 14:32:13.000000 cloudify-7.0.4/cloudify_cli/cli/helptexts.py
+-rw-r--r--   0 root         (0) root         (0)     6054 2024-04-07 14:32:13.000000 cloudify-7.0.4/cloudify_cli/colorful_event.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 14:35:41.403734 cloudify-7.0.4/cloudify_cli/commands/
+-rw-r--r--   0 root         (0) root         (0)      641 2024-04-07 14:32:13.000000 cloudify-7.0.4/cloudify_cli/commands/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16037 2024-04-07 14:32:13.000000 cloudify-7.0.4/cloudify_cli/commands/agents.py
+-rw-r--r--   0 root         (0) root         (0)    10374 2024-04-07 14:32:13.000000 cloudify-7.0.4/cloudify_cli/commands/apply.py
+-rw-r--r--   0 root         (0) root         (0)     5480 2024-04-07 14:32:13.000000 cloudify-7.0.4/cloudify_cli/commands/audit_log.py
+-rw-r--r--   0 root         (0) root         (0)    31561 2024-04-07 14:32:13.000000 cloudify-7.0.4/cloudify_cli/commands/blueprints.py
+-rw-r--r--   0 root         (0) root         (0)    14297 2024-04-07 14:32:13.000000 cloudify-7.0.4/cloudify_cli/commands/certificates.py
+-rw-r--r--   0 root         (0) root         (0)    16691 2024-04-07 14:32:13.000000 cloudify-7.0.4/cloudify_cli/commands/cluster.py
+-rw-r--r--   0 root         (0) root         (0)     1359 2024-04-07 14:32:13.000000 cloudify-7.0.4/cloudify_cli/commands/community.py
+-rw-r--r--   0 root         (0) root         (0)     2404 2024-04-07 14:32:13.000000 cloudify-7.0.4/cloudify_cli/commands/config.py
+-rw-r--r--   0 root         (0) root         (0)    72161 2024-04-07 14:32:13.000000 cloudify-7.0.4/cloudify_cli/commands/deployments.py
+-rw-r--r--   0 root         (0) root         (0)    12209 2024-04-07 14:32:13.000000 cloudify-7.0.4/cloudify_cli/commands/events.py
+-rw-r--r--   0 root         (0) root         (0)    33757 2024-04-07 14:32:13.000000 cloudify-7.0.4/cloudify_cli/commands/executions.py
+-rw-r--r--   0 root         (0) root         (0)     2785 2024-04-07 14:32:13.000000 cloudify-7.0.4/cloudify_cli/commands/groups.py
+-rw-r--r--   0 root         (0) root         (0)      383 2024-04-07 14:32:13.000000 cloudify-7.0.4/cloudify_cli/commands/idp.py
+-rw-r--r--   0 root         (0) root         (0)     6587 2024-04-07 14:32:13.000000 cloudify-7.0.4/cloudify_cli/commands/init.py
+-rw-r--r--   0 root         (0) root         (0)     8223 2024-04-07 14:32:13.000000 cloudify-7.0.4/cloudify_cli/commands/install.py
+-rw-r--r--   0 root         (0) root         (0)     3166 2024-04-07 14:32:13.000000 cloudify-7.0.4/cloudify_cli/commands/ldap.py
+-rw-r--r--   0 root         (0) root         (0)     4505 2024-04-07 14:32:13.000000 cloudify-7.0.4/cloudify_cli/commands/license.py
+-rw-r--r--   0 root         (0) root         (0)     3984 2024-04-07 14:32:13.000000 cloudify-7.0.4/cloudify_cli/commands/log_bundles.py
+-rw-r--r--   0 root         (0) root         (0)     5465 2024-04-07 14:32:13.000000 cloudify-7.0.4/cloudify_cli/commands/maintenance_mode.py
+-rw-r--r--   0 root         (0) root         (0)    10411 2024-04-07 14:32:13.000000 cloudify-7.0.4/cloudify_cli/commands/node_instances.py
+-rw-r--r--   0 root         (0) root         (0)     8827 2024-04-07 14:32:13.000000 cloudify-7.0.4/cloudify_cli/commands/nodes.py
+-rw-r--r--   0 root         (0) root         (0)     1909 2024-04-07 14:32:13.000000 cloudify-7.0.4/cloudify_cli/commands/permissions.py
+-rw-r--r--   0 root         (0) root         (0)    41310 2024-04-07 14:32:13.000000 cloudify-7.0.4/cloudify_cli/commands/plugins.py
+-rw-r--r--   0 root         (0) root         (0)    27830 2024-04-07 14:32:13.000000 cloudify-7.0.4/cloudify_cli/commands/profiles.py
+-rw-r--r--   0 root         (0) root         (0)    21581 2024-04-07 14:32:13.000000 cloudify-7.0.4/cloudify_cli/commands/secrets.py
+-rw-r--r--   0 root         (0) root         (0)     5512 2024-04-07 14:32:13.000000 cloudify-7.0.4/cloudify_cli/commands/sites.py
+-rw-r--r--   0 root         (0) root         (0)    10429 2024-04-07 14:32:13.000000 cloudify-7.0.4/cloudify_cli/commands/snapshots.py
+-rw-r--r--   0 root         (0) root         (0)     2419 2024-04-07 14:32:13.000000 cloudify-7.0.4/cloudify_cli/commands/status.py
+-rw-r--r--   0 root         (0) root         (0)     2264 2024-04-07 14:32:13.000000 cloudify-7.0.4/cloudify_cli/commands/summary.py
+-rw-r--r--   0 root         (0) root         (0)    10822 2024-04-07 14:32:13.000000 cloudify-7.0.4/cloudify_cli/commands/tenants.py
+-rw-r--r--   0 root         (0) root         (0)     2866 2024-04-07 14:32:13.000000 cloudify-7.0.4/cloudify_cli/commands/tokens.py
+-rw-r--r--   0 root         (0) root         (0)     4293 2024-04-07 14:32:13.000000 cloudify-7.0.4/cloudify_cli/commands/uninstall.py
+-rw-r--r--   0 root         (0) root         (0)     6937 2024-04-07 14:32:13.000000 cloudify-7.0.4/cloudify_cli/commands/user_groups.py
+-rw-r--r--   0 root         (0) root         (0)     9355 2024-04-07 14:32:13.000000 cloudify-7.0.4/cloudify_cli/commands/users.py
+-rw-r--r--   0 root         (0) root         (0)     5644 2024-04-07 14:32:13.000000 cloudify-7.0.4/cloudify_cli/commands/workflows.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 14:35:41.403734 cloudify-7.0.4/cloudify_cli/config/
+-rw-r--r--   0 root         (0) root         (0)      641 2024-04-07 14:32:13.000000 cloudify-7.0.4/cloudify_cli/config/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4228 2024-04-07 14:32:13.000000 cloudify-7.0.4/cloudify_cli/config/config.py
+-rw-r--r--   0 root         (0) root         (0)     2812 2024-04-07 14:32:13.000000 cloudify-7.0.4/cloudify_cli/constants.py
+-rw-r--r--   0 root         (0) root         (0)    22806 2024-04-07 14:32:13.000000 cloudify-7.0.4/cloudify_cli/env.py
+-rw-r--r--   0 root         (0) root         (0)     1498 2024-04-07 14:32:13.000000 cloudify-7.0.4/cloudify_cli/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     9183 2024-04-07 14:32:13.000000 cloudify-7.0.4/cloudify_cli/execution_events_fetcher.py
+-rw-r--r--   0 root         (0) root         (0)    13653 2024-04-07 14:32:13.000000 cloudify-7.0.4/cloudify_cli/filters_utils.py
+-rw-r--r--   0 root         (0) root         (0)     6006 2024-04-07 14:32:13.000000 cloudify-7.0.4/cloudify_cli/inputs.py
+-rw-r--r--   0 root         (0) root         (0)     5989 2024-04-07 14:32:13.000000 cloudify-7.0.4/cloudify_cli/labels_utils.py
+-rw-r--r--   0 root         (0) root         (0)     8492 2024-04-07 14:32:13.000000 cloudify-7.0.4/cloudify_cli/local.py
+-rw-r--r--   0 root         (0) root         (0)     6868 2024-04-07 14:32:13.000000 cloudify-7.0.4/cloudify_cli/logger.py
+-rw-r--r--   0 root         (0) root         (0)    13189 2024-04-07 14:32:13.000000 cloudify-7.0.4/cloudify_cli/main.py
+-rw-r--r--   0 root         (0) root         (0)    54445 2024-04-07 14:32:13.000000 cloudify-7.0.4/cloudify_cli/prettytable.py
+-rw-r--r--   0 root         (0) root         (0)    10905 2024-04-07 14:32:13.000000 cloudify-7.0.4/cloudify_cli/replace_certificates_config.py
+-rw-r--r--   0 root         (0) root         (0)     6697 2024-04-07 14:32:13.000000 cloudify-7.0.4/cloudify_cli/table.py
+-rw-r--r--   0 root         (0) root         (0)    16280 2024-04-07 14:32:13.000000 cloudify-7.0.4/cloudify_cli/utils.py
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-07 14:35:41.403734 cloudify-7.0.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1427 2024-04-07 14:32:13.000000 cloudify-7.0.4/setup.py
```

### Comparing `cloudify-7.0.3/LICENSE` & `cloudify-7.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `cloudify-7.0.3/README.md` & `cloudify-7.0.4/README.md`

 * *Files identical despite different names*

### Comparing `cloudify-7.0.3/cloudify.egg-info/SOURCES.txt` & `cloudify-7.0.4/cloudify.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,14 @@
 cloudify_cli/replace_certificates_config.py
 cloudify_cli/table.py
 cloudify_cli/utils.py
 cloudify_cli/async_commands/__init__.py
 cloudify_cli/async_commands/audit_log.py
 cloudify_cli/cli/__init__.py
 cloudify_cli/cli/cfy.py
-cloudify_cli/cli/completion_utils.py
 cloudify_cli/cli/helptexts.py
 cloudify_cli/commands/__init__.py
 cloudify_cli/commands/agents.py
 cloudify_cli/commands/apply.py
 cloudify_cli/commands/audit_log.py
 cloudify_cli/commands/blueprints.py
 cloudify_cli/commands/certificates.py
```

### Comparing `cloudify-7.0.3/cloudify_cli/__init__.py` & `cloudify-7.0.4/cloudify_cli/__init__.py`

 * *Files identical despite different names*

### Comparing `cloudify-7.0.3/cloudify_cli/async_commands/audit_log.py` & `cloudify-7.0.4/cloudify_cli/async_commands/audit_log.py`

 * *Files identical despite different names*

### Comparing `cloudify-7.0.3/cloudify_cli/blueprint.py` & `cloudify-7.0.4/cloudify_cli/blueprint.py`

 * *Files identical despite different names*

### Comparing `cloudify-7.0.3/cloudify_cli/cli/__init__.py` & `cloudify-7.0.4/cloudify_cli/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `cloudify-7.0.3/cloudify_cli/cli/cfy.py` & `cloudify-7.0.4/cloudify_cli/cli/cfy.py`

 * *Files 0% similar despite different names*

```diff
@@ -1434,14 +1434,20 @@
         self.legacy = click.option(
             '--legacy/--no-legacy',
             is_flag=True,
             default=True,
             help=helptexts.LEGACY_SNAPSHOT
         )
 
+        self.listener_timeout = click.option(
+            '--listener-timeout',
+            type=float,
+            help=helptexts.SNAPSHOT_LISTENER_TIMEOUT,
+        )
+
         self.wait_for_status = click.option(
             '-w',
             '--wait-for-status',
             is_flag=True,
             default=False,
             help=helptexts.WAIT_FOR_STATUS
         )
```

### Comparing `cloudify-7.0.3/cloudify_cli/cli/helptexts.py` & `cloudify-7.0.4/cloudify_cli/cli/helptexts.py`

 * *Files 0% similar despite different names*

```diff
@@ -597,14 +597,21 @@
                'of the resource.'
 WORKER_NAMES = 'Show the worker name for each event'
 DRIFT_ONLY = 'Run update without changing anything. This will still check ' \
              'drift and run update operations as necessary'
 TEMPDIR_PATH = "Temporary location to be used for snapshot creation. If not " \
                "specified, /tmp will be used."
 LEGACY_SNAPSHOT = "Create legacy version of the snapshot (as opposed to 'new')"
+SNAPSHOT_LISTENER_TIMEOUT = "Changes the timeout for pending actions to " \
+                           "complete. As snapshot creation is a " \
+                           "non-blocking execution, it can be run " \
+                           "independently of others. System changes " \
+                           "occuring during snapshot creation are added " \
+                           "to the snapshot. This parameter specified the " \
+                           "additional waiting time (in seconds)."
 WAIT_FOR_STATUS = "Whether to wait for snapshot status [default: False]."
 SUMMARY_HELP = """
     Retrieve summary of {type}, e.g. a count of each {example}.
 
     `TARGET_FIELD` is the field to summarize {type} on. `SUB_FIELD` is an
     optional second field to summarize {type} on. Both can be chosen from
     [{fields}].
```

### Comparing `cloudify-7.0.3/cloudify_cli/colorful_event.py` & `cloudify-7.0.4/cloudify_cli/colorful_event.py`

 * *Files identical despite different names*

### Comparing `cloudify-7.0.3/cloudify_cli/commands/__init__.py` & `cloudify-7.0.4/cloudify_cli/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `cloudify-7.0.3/cloudify_cli/commands/agents.py` & `cloudify-7.0.4/cloudify_cli/commands/agents.py`

 * *Files identical despite different names*

### Comparing `cloudify-7.0.3/cloudify_cli/commands/apply.py` & `cloudify-7.0.4/cloudify_cli/commands/apply.py`

 * *Files identical despite different names*

### Comparing `cloudify-7.0.3/cloudify_cli/commands/audit_log.py` & `cloudify-7.0.4/cloudify_cli/commands/audit_log.py`

 * *Files identical despite different names*

### Comparing `cloudify-7.0.3/cloudify_cli/commands/blueprints.py` & `cloudify-7.0.4/cloudify_cli/commands/blueprints.py`

 * *Files identical despite different names*

### Comparing `cloudify-7.0.3/cloudify_cli/commands/certificates.py` & `cloudify-7.0.4/cloudify_cli/commands/certificates.py`

 * *Files identical despite different names*

### Comparing `cloudify-7.0.3/cloudify_cli/commands/cluster.py` & `cloudify-7.0.4/cloudify_cli/commands/cluster.py`

 * *Files identical despite different names*

### Comparing `cloudify-7.0.3/cloudify_cli/commands/community.py` & `cloudify-7.0.4/cloudify_cli/commands/community.py`

 * *Files identical despite different names*

### Comparing `cloudify-7.0.3/cloudify_cli/commands/config.py` & `cloudify-7.0.4/cloudify_cli/commands/config.py`

 * *Files identical despite different names*

### Comparing `cloudify-7.0.3/cloudify_cli/commands/deployments.py` & `cloudify-7.0.4/cloudify_cli/commands/deployments.py`

 * *Files identical despite different names*

### Comparing `cloudify-7.0.3/cloudify_cli/commands/events.py` & `cloudify-7.0.4/cloudify_cli/commands/events.py`

 * *Files identical despite different names*

### Comparing `cloudify-7.0.3/cloudify_cli/commands/executions.py` & `cloudify-7.0.4/cloudify_cli/commands/executions.py`

 * *Files identical despite different names*

### Comparing `cloudify-7.0.3/cloudify_cli/commands/groups.py` & `cloudify-7.0.4/cloudify_cli/commands/groups.py`

 * *Files identical despite different names*

### Comparing `cloudify-7.0.3/cloudify_cli/commands/init.py` & `cloudify-7.0.4/cloudify_cli/commands/init.py`

 * *Files identical despite different names*

### Comparing `cloudify-7.0.3/cloudify_cli/commands/install.py` & `cloudify-7.0.4/cloudify_cli/commands/install.py`

 * *Files identical despite different names*

### Comparing `cloudify-7.0.3/cloudify_cli/commands/ldap.py` & `cloudify-7.0.4/cloudify_cli/commands/ldap.py`

 * *Files identical despite different names*

### Comparing `cloudify-7.0.3/cloudify_cli/commands/license.py` & `cloudify-7.0.4/cloudify_cli/commands/license.py`

 * *Files identical despite different names*

### Comparing `cloudify-7.0.3/cloudify_cli/commands/log_bundles.py` & `cloudify-7.0.4/cloudify_cli/commands/log_bundles.py`

 * *Files identical despite different names*

### Comparing `cloudify-7.0.3/cloudify_cli/commands/maintenance_mode.py` & `cloudify-7.0.4/cloudify_cli/commands/maintenance_mode.py`

 * *Files identical despite different names*

### Comparing `cloudify-7.0.3/cloudify_cli/commands/node_instances.py` & `cloudify-7.0.4/cloudify_cli/commands/node_instances.py`

 * *Files identical despite different names*

### Comparing `cloudify-7.0.3/cloudify_cli/commands/nodes.py` & `cloudify-7.0.4/cloudify_cli/commands/nodes.py`

 * *Files identical despite different names*

### Comparing `cloudify-7.0.3/cloudify_cli/commands/permissions.py` & `cloudify-7.0.4/cloudify_cli/commands/permissions.py`

 * *Files identical despite different names*

### Comparing `cloudify-7.0.3/cloudify_cli/commands/plugins.py` & `cloudify-7.0.4/cloudify_cli/commands/plugins.py`

 * *Files identical despite different names*

### Comparing `cloudify-7.0.3/cloudify_cli/commands/profiles.py` & `cloudify-7.0.4/cloudify_cli/commands/profiles.py`

 * *Files identical despite different names*

### Comparing `cloudify-7.0.3/cloudify_cli/commands/secrets.py` & `cloudify-7.0.4/cloudify_cli/commands/secrets.py`

 * *Files identical despite different names*

### Comparing `cloudify-7.0.3/cloudify_cli/commands/sites.py` & `cloudify-7.0.4/cloudify_cli/commands/sites.py`

 * *Files identical despite different names*

### Comparing `cloudify-7.0.3/cloudify_cli/commands/snapshots.py` & `cloudify-7.0.4/cloudify_cli/commands/snapshots.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 ############
 
 from cloudify.snapshots import STATES
 
 from cloudify_cli import utils
 from cloudify_cli.table import print_data
 from cloudify_cli.cli import helptexts, cfy
+from cloudify_cli.exceptions import CloudifyCliError
 from cloudify_cli.execution_events_fetcher import wait_for_execution
 
 SNAPSHOT_COLUMNS = ['id', 'created_at', 'status', 'error',
                     'visibility', 'tenant_name', 'created_by']
 
 SNAPSHOT_STATUSES = {
     STATES.RUNNING: 'Snapshot restore in progress... This may take a while, '
@@ -93,44 +94,51 @@
 @cfy.options.exclude_credentials
 @cfy.options.exclude_logs
 @cfy.options.exclude_events
 @cfy.options.common_options
 @cfy.options.queue_snapshot
 @cfy.options.tempdir_path
 @cfy.options.legacy
+@cfy.options.listener_timeout
 @cfy.options.wait_for_status
 @cfy.pass_client()
 @cfy.pass_logger
 def create(snapshot_id,
            exclude_credentials,
            exclude_logs,
            exclude_events,
            queue,
            tempdir_path,
            legacy,
+           listener_timeout,
            wait_for_status,
            logger,
            client):
     """Create a snapshot on the manager
 
     The snapshot will contain the relevant data to restore a manager to
     its previous state.
 
     `SNAPSHOT_ID` is the id to attach to the snapshot.
     """
+    if legacy and listener_timeout:
+        raise CloudifyCliError(
+            'Listener timeout can be set only for non-legacy snapshots.')
+
     snapshot_id = snapshot_id or utils.generate_suffixed_id('snapshot')
     logger.info('Creating snapshot {0}...'.format(snapshot_id))
 
     execution = client.snapshots.create(snapshot_id,
                                         not exclude_credentials,
                                         not exclude_logs,
                                         not exclude_events,
                                         queue,
                                         tempdir_path=tempdir_path,
-                                        legacy=legacy)
+                                        legacy=legacy,
+                                        listener_timeout=listener_timeout)
     started_log_msg = "Started workflow execution. The execution's id is" \
                       " {0}.".format(execution.id)
     queued_log_msg = '`queue` flag was passed, snapshot creation will start' \
                      ' automatically when possible. Execution id:' \
                      ' {0}'.format(execution.id)
     queued = True if execution.status == 'queued' else False
     logger.info(queued_log_msg) if queued else logger.info(started_log_msg)
```

### Comparing `cloudify-7.0.3/cloudify_cli/commands/status.py` & `cloudify-7.0.4/cloudify_cli/commands/status.py`

 * *Files identical despite different names*

### Comparing `cloudify-7.0.3/cloudify_cli/commands/summary.py` & `cloudify-7.0.4/cloudify_cli/commands/summary.py`

 * *Files identical despite different names*

### Comparing `cloudify-7.0.3/cloudify_cli/commands/tenants.py` & `cloudify-7.0.4/cloudify_cli/commands/tenants.py`

 * *Files identical despite different names*

### Comparing `cloudify-7.0.3/cloudify_cli/commands/tokens.py` & `cloudify-7.0.4/cloudify_cli/commands/tokens.py`

 * *Files identical despite different names*

### Comparing `cloudify-7.0.3/cloudify_cli/commands/uninstall.py` & `cloudify-7.0.4/cloudify_cli/commands/uninstall.py`

 * *Files identical despite different names*

### Comparing `cloudify-7.0.3/cloudify_cli/commands/user_groups.py` & `cloudify-7.0.4/cloudify_cli/commands/user_groups.py`

 * *Files identical despite different names*

### Comparing `cloudify-7.0.3/cloudify_cli/commands/users.py` & `cloudify-7.0.4/cloudify_cli/commands/users.py`

 * *Files identical despite different names*

### Comparing `cloudify-7.0.3/cloudify_cli/commands/workflows.py` & `cloudify-7.0.4/cloudify_cli/commands/workflows.py`

 * *Files identical despite different names*

### Comparing `cloudify-7.0.3/cloudify_cli/config/__init__.py` & `cloudify-7.0.4/cloudify_cli/config/__init__.py`

 * *Files identical despite different names*

### Comparing `cloudify-7.0.3/cloudify_cli/config/config.py` & `cloudify-7.0.4/cloudify_cli/config/config.py`

 * *Files identical despite different names*

### Comparing `cloudify-7.0.3/cloudify_cli/constants.py` & `cloudify-7.0.4/cloudify_cli/constants.py`

 * *Files identical despite different names*

### Comparing `cloudify-7.0.3/cloudify_cli/env.py` & `cloudify-7.0.4/cloudify_cli/env.py`

 * *Files identical despite different names*

### Comparing `cloudify-7.0.3/cloudify_cli/exceptions.py` & `cloudify-7.0.4/cloudify_cli/exceptions.py`

 * *Files identical despite different names*

### Comparing `cloudify-7.0.3/cloudify_cli/execution_events_fetcher.py` & `cloudify-7.0.4/cloudify_cli/execution_events_fetcher.py`

 * *Files identical despite different names*

### Comparing `cloudify-7.0.3/cloudify_cli/filters_utils.py` & `cloudify-7.0.4/cloudify_cli/filters_utils.py`

 * *Files identical despite different names*

### Comparing `cloudify-7.0.3/cloudify_cli/inputs.py` & `cloudify-7.0.4/cloudify_cli/inputs.py`

 * *Files identical despite different names*

### Comparing `cloudify-7.0.3/cloudify_cli/labels_utils.py` & `cloudify-7.0.4/cloudify_cli/labels_utils.py`

 * *Files identical despite different names*

### Comparing `cloudify-7.0.3/cloudify_cli/local.py` & `cloudify-7.0.4/cloudify_cli/local.py`

 * *Files identical despite different names*

### Comparing `cloudify-7.0.3/cloudify_cli/logger.py` & `cloudify-7.0.4/cloudify_cli/logger.py`

 * *Files identical despite different names*

### Comparing `cloudify-7.0.3/cloudify_cli/main.py` & `cloudify-7.0.4/cloudify_cli/main.py`

 * *Files identical despite different names*

### Comparing `cloudify-7.0.3/cloudify_cli/prettytable.py` & `cloudify-7.0.4/cloudify_cli/prettytable.py`

 * *Files identical despite different names*

### Comparing `cloudify-7.0.3/cloudify_cli/replace_certificates_config.py` & `cloudify-7.0.4/cloudify_cli/replace_certificates_config.py`

 * *Files identical despite different names*

### Comparing `cloudify-7.0.3/cloudify_cli/table.py` & `cloudify-7.0.4/cloudify_cli/table.py`

 * *Files identical despite different names*

### Comparing `cloudify-7.0.3/cloudify_cli/utils.py` & `cloudify-7.0.4/cloudify_cli/utils.py`

 * *Files identical despite different names*

### Comparing `cloudify-7.0.3/setup.py` & `cloudify-7.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     'cloudify_cli.commands',
     'cloudify_cli.config',
     'cloudify_cli.async_commands',
 ]
 
 setup(
     name='cloudify',
-    version='7.0.3',
+    version='7.0.4',
     author='Cloudify',
     author_email='cosmo-admin@cloudify.co',
     packages=packages,
     license='LICENSE',
     description="Cloudify's Command Line Interface",
     entry_points={
         'console_scripts': [
```

