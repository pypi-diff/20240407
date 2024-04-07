# Comparing `tmp/syft-0.8.6b1.tar.gz` & `tmp/syft-0.8.7b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syft-0.8.6b1.tar", last modified: Fri Mar 22 16:28:17 2024, max compression
+gzip compressed data, was "syft-0.8.7b1.tar", last modified: Sun Apr  7 12:41:40 2024, max compression
```

## Comparing `syft-0.8.6b1.tar` & `syft-0.8.7b1.tar`

### file list

```diff
@@ -1,311 +1,305 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:28:17.068658 syft-0.8.6b1/
--rw-r--r--   0 runner    (1001) docker     (127)    11843 2024-03-22 16:25:00.000000 syft-0.8.6b1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-03-22 16:25:00.000000 syft-0.8.6b1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    22992 2024-03-22 16:28:17.068658 syft-0.8.6b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    18569 2024-03-22 16:26:03.000000 syft-0.8.6b1/PYPI.md
--rw-r--r--   0 runner    (1001) docker     (127)    17399 2024-03-22 16:25:00.000000 syft-0.8.6b1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-03-22 16:25:00.000000 syft-0.8.6b1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     3346 2024-03-22 16:28:17.072658 syft-0.8.6b1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-03-22 16:25:00.000000 syft-0.8.6b1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:28:17.004657 syft-0.8.6b1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:28:17.012657 syft-0.8.6b1/src/syft/
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-03-22 16:25:31.000000 syft-0.8.6b1/src/syft/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)     6312 2024-03-22 16:25:31.000000 syft-0.8.6b1/src/syft/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/abstract_node.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:28:17.016657 syft-0.8.6b1/src/syft/capnp/
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/capnp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/capnp/iterable.capnp
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/capnp/kv_iterable.capnp
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/capnp/recursive_serde.capnp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:28:17.016657 syft-0.8.6b1/src/syft/client/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    36986 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/client/api.py
--rw-r--r--   0 runner    (1001) docker     (127)    46083 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/client/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/client/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/client/deploy.py
--rw-r--r--   0 runner    (1001) docker     (127)    18906 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/client/domain_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     7795 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/client/enclave_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     6359 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/client/gateway_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/client/protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)    14936 2024-03-22 16:27:15.000000 syft-0.8.6b1/src/syft/client/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/client/search.py
--rw-r--r--   0 runner    (1001) docker     (127)     8876 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/client/syncing.py
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/client/user_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:28:17.020657 syft-0.8.6b1/src/syft/custom_worker/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/custom_worker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4253 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/custom_worker/builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/custom_worker/builder_docker.py
--rw-r--r--   0 runner    (1001) docker     (127)    13892 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/custom_worker/builder_k8s.py
--rw-r--r--   0 runner    (1001) docker     (127)      998 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/custom_worker/builder_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     5478 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/custom_worker/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     7955 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/custom_worker/k8s.py
--rw-r--r--   0 runner    (1001) docker     (127)     7535 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/custom_worker/runner_k8s.py
--rw-r--r--   0 runner    (1001) docker     (127)      951 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/custom_worker/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:28:17.020657 syft-0.8.6b1/src/syft/exceptions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      863 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/exceptions/exception.py
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/exceptions/user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:28:17.020657 syft-0.8.6b1/src/syft/external/
--rw-r--r--   0 runner    (1001) docker     (127)     2017 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/external/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:28:17.020657 syft-0.8.6b1/src/syft/external/oblv/
--rw-r--r--   0 runner    (1001) docker     (127)      860 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/external/oblv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/external/oblv/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/external/oblv/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     4750 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/external/oblv/deployment.py
--rw-r--r--   0 runner    (1001) docker     (127)    12614 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/external/oblv/deployment_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/external/oblv/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/external/oblv/oblv_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/external/oblv/oblv_keys_stash.py
--rw-r--r--   0 runner    (1001) docker     (127)     7524 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/external/oblv/oblv_proxy.py
--rw-r--r--   0 runner    (1001) docker     (127)    13721 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/external/oblv/oblv_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/gevent_patch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:28:17.024657 syft-0.8.6b1/src/syft/img/
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/img/base64.py
--rw-r--r--   0 runner    (1001) docker     (127)    25535 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/img/logo.png
--rw-r--r--   0 runner    (1001) docker     (127)    41764 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/img/small-grid-symbol-logo.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:28:17.024657 syft-0.8.6b1/src/syft/node/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/node/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/node/credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/node/domain.py
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/node/enclave.py
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/node/gateway.py
--rw-r--r--   0 runner    (1001) docker     (127)    60531 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/node/node.py
--rw-r--r--   0 runner    (1001) docker     (127)     7319 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/node/routes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/node/run.py
--rw-r--r--   0 runner    (1001) docker     (127)     8758 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/node/server.py
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/node/worker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/node/worker_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:28:17.024657 syft-0.8.6b1/src/syft/protocol/
--rw-r--r--   0 runner    (1001) docker     (127)    22541 2024-03-22 16:27:14.000000 syft-0.8.6b1/src/syft/protocol/data_protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/protocol/protocol_version.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:28:17.024657 syft-0.8.6b1/src/syft/protocol/releases/
--rw-r--r--   0 runner    (1001) docker     (127)    21316 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/protocol/releases/0.8.2.json
--rw-r--r--   0 runner    (1001) docker     (127)     5405 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/protocol/releases/0.8.3.json
--rw-r--r--   0 runner    (1001) docker     (127)     6868 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/protocol/releases/0.8.4.json
--rw-r--r--   0 runner    (1001) docker     (127)    50490 2024-03-22 16:27:36.000000 syft-0.8.6b1/src/syft/protocol/releases/0.8.5.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:28:17.028658 syft-0.8.6b1/src/syft/serde/
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/serde/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3597 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/serde/array.py
--rw-r--r--   0 runner    (1001) docker     (127)     4068 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/serde/arrow.py
--rw-r--r--   0 runner    (1001) docker     (127)      404 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/serde/capnp.py
--rw-r--r--   0 runner    (1001) docker     (127)      722 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/serde/deserialize.py
--rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/serde/lib_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)    11491 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/serde/lib_service_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/serde/mock.py
--rw-r--r--   0 runner    (1001) docker     (127)    11818 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/serde/recursive.py
--rw-r--r--   0 runner    (1001) docker     (127)    11583 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/serde/recursive_primitives.py
--rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/serde/serializable.py
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/serde/serialize.py
--rw-r--r--   0 runner    (1001) docker     (127)     4937 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/serde/signature.py
--rw-r--r--   0 runner    (1001) docker     (127)     5904 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/serde/third_party.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:28:17.028658 syft-0.8.6b1/src/syft/service/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:28:17.032657 syft-0.8.6b1/src/syft/service/action/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/action/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      979 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/action/action_data_empty.py
--rw-r--r--   0 runner    (1001) docker     (127)    16790 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/action/action_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     6947 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/action/action_graph_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    71240 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/action/action_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     3148 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/action/action_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)    37785 2024-03-22 16:27:14.000000 syft-0.8.6b1/src/syft/service/action/action_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    13954 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/action/action_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/action/action_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     4167 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/action/numpy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2200 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/action/pandas.py
--rw-r--r--   0 runner    (1001) docker     (127)     3611 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/action/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)     4875 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/action/verification.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:28:17.032657 syft-0.8.6b1/src/syft/service/blob_storage/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/blob_storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/blob_storage/remote_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)    12866 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/blob_storage/service.py
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/blob_storage/stash.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:28:17.036658 syft-0.8.6b1/src/syft/service/code/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/code/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/code/code_parse.py
--rw-r--r--   0 runner    (1001) docker     (127)     3166 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/code/status_service.py
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/code/unparse.py
--rw-r--r--   0 runner    (1001) docker     (127)    55680 2024-03-22 16:27:14.000000 syft-0.8.6b1/src/syft/service/code/user_code.py
--rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/code/user_code_parse.py
--rw-r--r--   0 runner    (1001) docker     (127)    24350 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/code/user_code_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/code/user_code_stash.py
--rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/code/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:28:17.036658 syft-0.8.6b1/src/syft/service/code_history/
--rw-r--r--   0 runner    (1001) docker     (127)     4854 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/code_history/code_history.py
--rw-r--r--   0 runner    (1001) docker     (127)     9177 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/code_history/code_history_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/code_history/code_history_stash.py
--rw-r--r--   0 runner    (1001) docker     (127)     3218 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/context.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:28:17.036658 syft-0.8.6b1/src/syft/service/data_subject/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/data_subject/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4260 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/data_subject/data_subject.py
--rw-r--r--   0 runner    (1001) docker     (127)      908 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/data_subject/data_subject_member.py
--rw-r--r--   0 runner    (1001) docker     (127)     3120 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/data_subject/data_subject_member_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     5121 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/data_subject/data_subject_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:28:17.036658 syft-0.8.6b1/src/syft/service/dataset/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28883 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/dataset/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     7503 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/dataset/dataset_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1911 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/dataset/dataset_stash.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:28:17.036658 syft-0.8.6b1/src/syft/service/enclave/
--rw-r--r--   0 runner    (1001) docker     (127)     6597 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/enclave/enclave_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:28:17.036658 syft-0.8.6b1/src/syft/service/job/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/job/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9191 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/job/job_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    22622 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/job/job_stash.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:28:17.036658 syft-0.8.6b1/src/syft/service/log/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/log/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      844 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/log/log.py
--rw-r--r--   0 runner    (1001) docker     (127)     4493 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/log/log_service.py
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/log/log_stash.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:28:17.040658 syft-0.8.6b1/src/syft/service/metadata/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/metadata/metadata_service.py
--rw-r--r--   0 runner    (1001) docker     (127)      941 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/metadata/migrations.py
--rw-r--r--   0 runner    (1001) docker     (127)     4427 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/metadata/node_metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:28:17.040658 syft-0.8.6b1/src/syft/service/network/
--rw-r--r--   0 runner    (1001) docker     (127)    19533 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/network/network_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     6564 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/network/node_peer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6027 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/network/routes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:28:17.040658 syft-0.8.6b1/src/syft/service/notification/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/notification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14659 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/notification/email_templates.py
--rw-r--r--   0 runner    (1001) docker     (127)    10068 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/notification/notification_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     4542 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/notification/notification_stash.py
--rw-r--r--   0 runner    (1001) docker     (127)     5211 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/notification/notifications.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:28:17.040658 syft-0.8.6b1/src/syft/service/notifier/
--rw-r--r--   0 runner    (1001) docker     (127)     7052 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/notifier/notifier.py
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/notifier/notifier_enums.py
--rw-r--r--   0 runner    (1001) docker     (127)    11728 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/notifier/notifier_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     2981 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/notifier/notifier_stash.py
--rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/notifier/smtp_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:28:17.040658 syft-0.8.6b1/src/syft/service/object_search/
--rw-r--r--   0 runner    (1001) docker     (127)     2342 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/object_search/migration_state_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/object_search/object_migration_state.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:28:17.040658 syft-0.8.6b1/src/syft/service/output/
--rw-r--r--   0 runner    (1001) docker     (127)     9891 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/output/output_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:28:17.044658 syft-0.8.6b1/src/syft/service/policy/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/policy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27196 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/policy/policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/policy/policy_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/policy/user_policy_stash.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:28:17.044658 syft-0.8.6b1/src/syft/service/project/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    49644 2024-03-22 16:27:14.000000 syft-0.8.6b1/src/syft/service/project/project.py
--rw-r--r--   0 runner    (1001) docker     (127)    15911 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/project/project_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/project/project_stash.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:28:17.044658 syft-0.8.6b1/src/syft/service/queue/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/queue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2619 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/queue/base_queue.py
--rw-r--r--   0 runner    (1001) docker     (127)    11250 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/queue/queue.py
--rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/queue/queue_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     5354 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/queue/queue_stash.py
--rw-r--r--   0 runner    (1001) docker     (127)    33929 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/queue/zmq_queue.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:28:17.044658 syft-0.8.6b1/src/syft/service/request/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/request/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    49952 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/request/request.py
--rw-r--r--   0 runner    (1001) docker     (127)    11568 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/request/request_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/request/request_stash.py
--rw-r--r--   0 runner    (1001) docker     (127)     3614 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/response.py
--rw-r--r--   0 runner    (1001) docker     (127)    17295 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:28:17.048658 syft-0.8.6b1/src/syft/service/settings/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/settings/migrations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/settings/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     5127 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/settings/settings_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/settings/settings_stash.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:28:17.048658 syft-0.8.6b1/src/syft/service/sync/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/sync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    29637 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/sync/diff_state.py
--rw-r--r--   0 runner    (1001) docker     (127)    11131 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/sync/sync_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/sync/sync_stash.py
--rw-r--r--   0 runner    (1001) docker     (127)     4700 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/sync/sync_state.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:28:17.048658 syft-0.8.6b1/src/syft/service/user/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/user/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/user/roles.py
--rw-r--r--   0 runner    (1001) docker     (127)    11013 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/user/user.py
--rw-r--r--   0 runner    (1001) docker     (127)     3483 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/user/user_roles.py
--rw-r--r--   0 runner    (1001) docker     (127)    20699 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/user/user_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     4968 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/user/user_stash.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:28:17.052658 syft-0.8.6b1/src/syft/service/veilid/
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/veilid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/veilid/veilid_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (127)     3109 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/veilid/veilid_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     5655 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/warnings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:28:17.052658 syft-0.8.6b1/src/syft/service/worker/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/worker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/worker/image_identifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/worker/image_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     3663 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/worker/image_registry_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/worker/image_registry_stash.py
--rw-r--r--   0 runner    (1001) docker     (127)    22317 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/worker/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/worker/worker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/worker/worker_image.py
--rw-r--r--   0 runner    (1001) docker     (127)    10314 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/worker/worker_image_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     2463 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/worker/worker_image_stash.py
--rw-r--r--   0 runner    (1001) docker     (127)     9700 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/worker/worker_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)    25667 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/worker/worker_pool_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     2324 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/worker/worker_pool_stash.py
--rw-r--r--   0 runner    (1001) docker     (127)    11381 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/worker/worker_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     3029 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/worker/worker_stash.py
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/stable_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:28:17.056658 syft-0.8.6b1/src/syft/store/
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/store/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:28:17.056658 syft-0.8.6b1/src/syft/store/blob_storage/
--rw-r--r--   0 runner    (1001) docker     (127)     8101 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/store/blob_storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3497 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/store/blob_storage/on_disk.py
--rw-r--r--   0 runner    (1001) docker     (127)    10785 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/store/blob_storage/seaweedfs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3371 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/store/dict_document_store.py
--rw-r--r--   0 runner    (1001) docker     (127)    25674 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/store/document_store.py
--rw-r--r--   0 runner    (1001) docker     (127)    25135 2024-03-22 16:27:14.000000 syft-0.8.6b1/src/syft/store/kv_document_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     4972 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/store/linked_obj.py
--rw-r--r--   0 runner    (1001) docker     (127)    11659 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/store/locks.py
--rw-r--r--   0 runner    (1001) docker     (127)    10005 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/store/mongo_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      909 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/store/mongo_codecs.py
--rw-r--r--   0 runner    (1001) docker     (127)    31590 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/store/mongo_document_store.py
--rw-r--r--   0 runner    (1001) docker     (127)    15863 2024-03-22 16:27:14.000000 syft-0.8.6b1/src/syft/store/sqlite_document_store.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:28:17.060658 syft-0.8.6b1/src/syft/types/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/types/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    11865 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/types/blob_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/types/cache_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/types/datetime.py
--rw-r--r--   0 runner    (1001) docker     (127)     7492 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/types/dicttuple.py
--rw-r--r--   0 runner    (1001) docker     (127)     5271 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/types/grid_url.py
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/types/identity.py
--rw-r--r--   0 runner    (1001) docker     (127)      971 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/types/syft_metaclass.py
--rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/types/syft_migration.py
--rw-r--r--   0 runner    (1001) docker     (127)    37205 2024-03-22 16:27:14.000000 syft-0.8.6b1/src/syft/types/syft_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/types/syncable_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     8877 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/types/transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)     2839 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/types/twin_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     8245 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/types/uid.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:28:17.064658 syft-0.8.6b1/src/syft/util/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9797 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/util/_std_stream_capture.py
--rw-r--r--   0 runner    (1001) docker     (127)      978 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/util/autoreload.py
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/util/colors.py
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/util/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/util/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/util/env.py
--rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/util/experimental_flags.py
--rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/util/filterwarnings.py
--rw-r--r--   0 runner    (1001) docker     (127)     2940 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/util/fonts.py
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/util/jax_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     3765 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/util/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)      857 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/util/markdown.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:28:17.064658 syft-0.8.6b1/src/syft/util/notebook_ui/
--rw-r--r--   0 runner    (1001) docker     (127)    28420 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/util/notebook_ui/notebook_addons.py
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/util/options.py
--rw-r--r--   0 runner    (1001) docker     (127)     5301 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/util/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     2601 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/util/telemetry.py
--rw-r--r--   0 runner    (1001) docker     (127)     6681 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/util/trace_decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)    24446 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/util/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3110 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/util/version_compare.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:28:17.064658 syft-0.8.6b1/src/syft.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    22992 2024-03-22 16:28:16.000000 syft-0.8.6b1/src/syft.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9149 2024-03-22 16:28:17.000000 syft-0.8.6b1/src/syft.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-22 16:28:16.000000 syft-0.8.6b1/src/syft.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-03-22 16:28:16.000000 syft-0.8.6b1/src/syft.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-22 16:25:32.000000 syft-0.8.6b1/src/syft.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-03-22 16:28:16.000000 syft-0.8.6b1/src/syft.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-03-22 16:28:16.000000 syft-0.8.6b1/src/syft.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:41:40.201675 syft-0.8.7b1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11843 2024-04-07 12:37:49.000000 syft-0.8.7b1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-07 12:37:49.000000 syft-0.8.7b1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    23134 2024-04-07 12:41:40.201675 syft-0.8.7b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    18678 2024-04-07 12:39:28.000000 syft-0.8.7b1/PYPI.md
+-rw-r--r--   0 runner    (1001) docker     (127)    17508 2024-04-07 12:37:49.000000 syft-0.8.7b1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-07 12:37:49.000000 syft-0.8.7b1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     3365 2024-04-07 12:41:40.201675 syft-0.8.7b1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-07 12:37:49.000000 syft-0.8.7b1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:41:40.141673 syft-0.8.7b1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:41:40.149673 syft-0.8.7b1/src/syft/
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-07 12:38:47.000000 syft-0.8.7b1/src/syft/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)     6371 2024-04-07 12:38:47.000000 syft-0.8.7b1/src/syft/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/abstract_node.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:41:40.149673 syft-0.8.7b1/src/syft/capnp/
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/capnp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/capnp/iterable.capnp
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/capnp/kv_iterable.capnp
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/capnp/recursive_serde.capnp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:41:40.153673 syft-0.8.7b1/src/syft/client/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41720 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/client/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46245 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/client/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/client/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/client/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18511 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/client/domain_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7793 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/client/enclave_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6357 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/client/gateway_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/client/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16212 2024-04-07 12:40:41.000000 syft-0.8.7b1/src/syft/client/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3661 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/client/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/client/sync_decision.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12864 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/client/syncing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/client/user_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:41:40.153673 syft-0.8.7b1/src/syft/custom_worker/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/custom_worker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4253 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/custom_worker/builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/custom_worker/builder_docker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13892 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/custom_worker/builder_k8s.py
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/custom_worker/builder_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5478 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/custom_worker/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7955 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/custom_worker/k8s.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7535 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/custom_worker/runner_k8s.py
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/custom_worker/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:41:40.153673 syft-0.8.7b1/src/syft/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/exceptions/exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/exceptions/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/gevent_patch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:41:40.153673 syft-0.8.7b1/src/syft/img/
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/img/base64.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25535 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/img/logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)    41764 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/img/small-grid-symbol-logo.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:41:40.157673 syft-0.8.7b1/src/syft/node/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/node/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/node/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/node/domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/node/enclave.py
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/node/gateway.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59372 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/node/node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7319 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/node/routes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/node/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8758 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/node/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/node/worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/node/worker_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:41:40.157673 syft-0.8.7b1/src/syft/protocol/
+-rw-r--r--   0 runner    (1001) docker     (127)    24381 2024-04-07 12:40:41.000000 syft-0.8.7b1/src/syft/protocol/data_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3102 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/protocol/protocol_version.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:41:40.157673 syft-0.8.7b1/src/syft/protocol/releases/
+-rw-r--r--   0 runner    (1001) docker     (127)    21316 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/protocol/releases/0.8.2.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5405 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/protocol/releases/0.8.3.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6868 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/protocol/releases/0.8.4.json
+-rw-r--r--   0 runner    (1001) docker     (127)    50490 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/protocol/releases/0.8.6.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:41:40.161673 syft-0.8.7b1/src/syft/serde/
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/serde/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3597 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/serde/array.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4068 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/serde/arrow.py
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/serde/capnp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      722 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/serde/deserialize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/serde/lib_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11491 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/serde/lib_service_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/serde/mock.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11818 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/serde/recursive.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11583 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/serde/recursive_primitives.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/serde/serializable.py
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/serde/serialize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4937 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/serde/signature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6976 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/serde/third_party.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:41:40.161673 syft-0.8.7b1/src/syft/service/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:41:40.165674 syft-0.8.7b1/src/syft/service/action/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/action/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/action/action_data_empty.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/action/action_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16790 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/action/action_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6947 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/action/action_graph_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    72779 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/action/action_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3164 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/action/action_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39060 2024-04-07 12:40:41.000000 syft-0.8.7b1/src/syft/service/action/action_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14084 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/action/action_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/action/action_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4167 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/action/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2200 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/action/pandas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3611 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/action/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4875 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/action/verification.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:41:40.165674 syft-0.8.7b1/src/syft/service/api/
+-rw-r--r--   0 runner    (1001) docker     (127)    19755 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/api/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12425 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/api/api_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2259 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/api/api_stash.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:41:40.165674 syft-0.8.7b1/src/syft/service/blob_storage/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/blob_storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/blob_storage/remote_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12511 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/blob_storage/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/blob_storage/stash.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:41:40.165674 syft-0.8.7b1/src/syft/service/code/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/code/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/code/code_parse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3614 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/code/status_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/code/unparse.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55843 2024-04-07 12:40:41.000000 syft-0.8.7b1/src/syft/service/code/user_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/code/user_code_parse.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25074 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/code/user_code_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/code/user_code_stash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/code/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:41:40.169674 syft-0.8.7b1/src/syft/service/code_history/
+-rw-r--r--   0 runner    (1001) docker     (127)     4854 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/code_history/code_history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8832 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/code_history/code_history_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/code_history/code_history_stash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3102 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:41:40.169674 syft-0.8.7b1/src/syft/service/data_subject/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/data_subject/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4260 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/data_subject/data_subject.py
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/data_subject/data_subject_member.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3120 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/data_subject/data_subject_member_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4943 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/data_subject/data_subject_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:41:40.169674 syft-0.8.7b1/src/syft/service/dataset/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28880 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/dataset/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7230 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/dataset/dataset_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1911 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/dataset/dataset_stash.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:41:40.169674 syft-0.8.7b1/src/syft/service/enclave/
+-rw-r--r--   0 runner    (1001) docker     (127)     5324 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/enclave/enclave_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:41:40.169674 syft-0.8.7b1/src/syft/service/job/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/job/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9408 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/job/job_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24816 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/job/job_stash.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:41:40.169674 syft-0.8.7b1/src/syft/service/log/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/log/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/log/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4876 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/log/log_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/log/log_stash.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:41:40.173674 syft-0.8.7b1/src/syft/service/metadata/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/metadata/metadata_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)      941 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/metadata/migrations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4427 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/metadata/node_metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:41:40.173674 syft-0.8.7b1/src/syft/service/network/
+-rw-r--r--   0 runner    (1001) docker     (127)    18970 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/network/network_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6457 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/network/node_peer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5836 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/network/routes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:41:40.173674 syft-0.8.7b1/src/syft/service/notification/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/notification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14281 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/notification/email_templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9667 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/notification/notification_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4542 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/notification/notification_stash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5211 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/notification/notifications.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:41:40.173674 syft-0.8.7b1/src/syft/service/notifier/
+-rw-r--r--   0 runner    (1001) docker     (127)     6925 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/notifier/notifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/notifier/notifier_enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11477 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/notifier/notifier_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2981 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/notifier/notifier_stash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/notifier/smtp_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:41:40.173674 syft-0.8.7b1/src/syft/service/object_search/
+-rw-r--r--   0 runner    (1001) docker     (127)     2342 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/object_search/migration_state_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/object_search/object_migration_state.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:41:40.173674 syft-0.8.7b1/src/syft/service/output/
+-rw-r--r--   0 runner    (1001) docker     (127)    11222 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/output/output_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:41:40.177674 syft-0.8.7b1/src/syft/service/policy/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/policy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27118 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/policy/policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/policy/policy_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/policy/user_policy_stash.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:41:40.177674 syft-0.8.7b1/src/syft/service/project/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49644 2024-04-07 12:40:41.000000 syft-0.8.7b1/src/syft/service/project/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15401 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/project/project_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/project/project_stash.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:41:40.177674 syft-0.8.7b1/src/syft/service/queue/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/queue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2619 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/queue/base_queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11250 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/queue/queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/queue/queue_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5354 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/queue/queue_stash.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33929 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/queue/zmq_queue.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:41:40.177674 syft-0.8.7b1/src/syft/service/request/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/request/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49704 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/request/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11273 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/request/request_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/request/request_stash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3614 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17295 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:41:40.181674 syft-0.8.7b1/src/syft/service/settings/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/settings/migrations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/settings/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4839 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/settings/settings_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/settings/settings_stash.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:41:40.181674 syft-0.8.7b1/src/syft/service/sync/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/sync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48845 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/sync/diff_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21598 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/sync/resolve_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13157 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/sync/sync_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/sync/sync_stash.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11570 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/sync/sync_state.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:41:40.181674 syft-0.8.7b1/src/syft/service/user/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/user/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/user/roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11013 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/user/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3483 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/user/user_roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20579 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/user/user_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4968 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/user/user_stash.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:41:40.185674 syft-0.8.7b1/src/syft/service/veilid/
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/veilid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/veilid/veilid_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3109 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/veilid/veilid_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5655 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/warnings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:41:40.185674 syft-0.8.7b1/src/syft/service/worker/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/worker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/worker/image_identifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/worker/image_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3663 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/worker/image_registry_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/worker/image_registry_stash.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22317 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/worker/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/worker/worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/worker/worker_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10135 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/worker/worker_image_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2463 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/worker/worker_image_stash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9698 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/worker/worker_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25273 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/worker/worker_pool_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2324 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/worker/worker_pool_stash.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11229 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/worker/worker_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3029 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/worker/worker_stash.py
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/stable_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:41:40.189674 syft-0.8.7b1/src/syft/store/
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/store/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:41:40.189674 syft-0.8.7b1/src/syft/store/blob_storage/
+-rw-r--r--   0 runner    (1001) docker     (127)     8101 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/store/blob_storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3497 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/store/blob_storage/on_disk.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10785 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/store/blob_storage/seaweedfs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3371 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/store/dict_document_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26359 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/store/document_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25265 2024-04-07 12:40:41.000000 syft-0.8.7b1/src/syft/store/kv_document_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4972 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/store/linked_obj.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11659 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/store/locks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10902 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/store/mongo_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      909 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/store/mongo_codecs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35722 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/store/mongo_document_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15863 2024-04-07 12:40:41.000000 syft-0.8.7b1/src/syft/store/sqlite_document_store.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:41:40.193674 syft-0.8.7b1/src/syft/types/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/types/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11865 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/types/blob_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/types/cache_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/types/datetime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7492 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/types/dicttuple.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5271 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/types/grid_url.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/types/identity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/types/syft_metaclass.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/types/syft_migration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36866 2024-04-07 12:40:41.000000 syft-0.8.7b1/src/syft/types/syft_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/types/syncable_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8877 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/types/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2839 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/types/twin_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8245 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/types/uid.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:41:40.197674 syft-0.8.7b1/src/syft/util/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9797 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/util/_std_stream_capture.py
+-rw-r--r--   0 runner    (1001) docker     (127)      978 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/util/autoreload.py
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/util/colors.py
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/util/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/util/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/util/env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/util/experimental_flags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/util/filterwarnings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2939 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/util/fonts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/util/jax_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3765 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/util/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      857 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/util/markdown.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:41:40.197674 syft-0.8.7b1/src/syft/util/notebook_ui/
+-rw-r--r--   0 runner    (1001) docker     (127)    32438 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/util/notebook_ui/notebook_addons.py
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/util/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5301 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/util/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2601 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/util/telemetry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6681 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/util/trace_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24531 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/util/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3110 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/util/version_compare.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:41:40.197674 syft-0.8.7b1/src/syft.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    23134 2024-04-07 12:41:40.000000 syft-0.8.7b1/src/syft.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8959 2024-04-07 12:41:40.000000 syft-0.8.7b1/src/syft.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 12:41:40.000000 syft-0.8.7b1/src/syft.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-07 12:41:40.000000 syft-0.8.7b1/src/syft.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 12:38:48.000000 syft-0.8.7b1/src/syft.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)     1660 2024-04-07 12:41:40.000000 syft-0.8.7b1/src/syft.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-07 12:41:40.000000 syft-0.8.7b1/src/syft.egg-info/top_level.txt
```

### Comparing `syft-0.8.6b1/LICENSE` & `syft-0.8.7b1/LICENSE`

 * *Files identical despite different names*

### Comparing `syft-0.8.6b1/PKG-INFO` & `syft-0.8.7b1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syft
-Version: 0.8.6b1
+Version: 0.8.7b1
 Summary: Perform numpy-like analysis on data that remains in someone elses server
 Home-page: https://openmined.github.io/PySyft/
 Author: OpenMined
 Author-email: info@openmined.org
 License: Apache-2.0
 Project-URL: Source, https://github.com/OpenMined/PySyft
 Project-URL: Tracker, https://github.com/OpenMined/PySyft/issues
@@ -48,14 +48,15 @@
 Requires-Dist: numpy<=1.24.4,>=1.23.5; python_version < "3.12"
 Requires-Dist: numpy<1.27,>=1.26.4; python_version >= "3.12"
 Requires-Dist: pandas==2.2.1
 Requires-Dist: docker==6.1.3
 Requires-Dist: kr8s==0.13.5
 Requires-Dist: PyYAML==6.0.1
 Requires-Dist: azure-storage-blob==12.19.1
+Requires-Dist: ipywidgets==8.1.2
 Provides-Extra: data-science
 Requires-Dist: transformers==4.38.2; extra == "data-science"
 Requires-Dist: opendp==0.9.2; extra == "data-science"
 Requires-Dist: evaluate==0.4.1; extra == "data-science"
 Requires-Dist: recordlinkage==0.16; extra == "data-science"
 Requires-Dist: dm-haiku==0.0.10; extra == "data-science"
 Requires-Dist: torch[cpu]==2.2.1; extra == "data-science"
@@ -101,15 +102,15 @@
 Requires-Dist: coverage; extra == "test-plugins"
 Requires-Dist: faker; extra == "test-plugins"
 Requires-Dist: distro; extra == "test-plugins"
 
 <div align="left"> <a href="https://pypi.org/project/syft/"><img src="https://static.pepy.tech/badge/pysyft" /></a> <a href="https://pypi.org/project/syft/"><img src="https://badge.fury.io/py/syft.svg" /></a> <a href="https://hub.docker.com/u/openmined"><img src="https://img.shields.io/badge/docker-images-blue?logo=docker" /></a> <a href="https://github.com/OpenMined/PySyft/actions/workflows/nightlies.yml"><img src="https://github.com/OpenMined/PySyft/actions/workflows/nightlies.yml/badge.svg?branch=dev" /></a> <a href="https://slack.openmined.org/"><img src="https://img.shields.io/badge/chat-on%20slack-purple?logo=slack" /></a> <a href="https://openmined.github.io/PySyft/"><img src="https://img.shields.io/badge/read-docs-yellow?logo=mdbook" /></a>
 <br /><br /></div>
 
-<img alt="Syft Logo" src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.6/docs/img/title_syft_light.png" width="200px" />
+<img alt="Syft Logo" src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.7/docs/img/title_syft_light.png" width="200px" />
 
 Perform data science on `data` that remains in `someone else's` server
 
 # Quickstart
 
 ✅ `Linux` ✅ `macOS` ✅ `Windows` ✅ `Docker` ✅ `Podman` ✅ `Kubernetes`
 
@@ -120,49 +121,49 @@
 ```
 
 ## Launch Server
 
 ```python
 # from Jupyter / Python
 import syft as sy
-sy.requires(">=0.8.5,<0.8.6")
+sy.requires(">=0.8.6,<0.8.7")
 node = sy.orchestra.launch(name="my-domain", port=8080, dev_mode=True, reset=True)
 ```
 
 ```bash
 # or from the command line
 $ syft launch --name=my-domain --port=8080 --reset=True
 
 Starting syft-node server on 0.0.0.0:8080
 ```
 
 ## Launch Client
 
 ```python
 import syft as sy
-sy.requires(">=0.8.5,<0.8.6")
+sy.requires(">=0.8.6,<0.8.7")
 domain_client = sy.login(port=8080, email="info@openmined.org", password="changethis")
 ```
 
 ## PySyft in 10 minutes
 
-📝 <a href="https://github.com/OpenMined/PySyft/tree/0.8.6/notebooks/api">API Example Notebooks</a>
+📝 <a href="https://github.com/OpenMined/PySyft/tree/0.8.7/notebooks/api">API Example Notebooks</a>
 
-- <a href="https://github.com/OpenMined/PySyft/tree/0.8.6/notebooks/api/0.8/00-load-data.ipynb">00-load-data.ipynb</a>
-- <a href="https://github.com/OpenMined/PySyft/tree/0.8.6/notebooks/api/0.8/01-submit-code.ipynb">01-submit-code.ipynb</a>
-- <a href="https://github.com/OpenMined/PySyft/tree/0.8.6/notebooks/api/0.8/02-review-code-and-approve.ipynb">02-review-code-and-approve.ipynb</a>
-- <a href="https://github.com/OpenMined/PySyft/tree/0.8.6/notebooks/api/0.8/03-data-scientist-download-result.ipynb">03-data-scientist-download-result.ipynb</a>
-- <a href="https://github.com/OpenMined/PySyft/tree/0.8.6/notebooks/api/0.8/04-jax-example.ipynb">04-jax-example.ipynb</a>
-- <a href="https://github.com/OpenMined/PySyft/tree/0.8.6/notebooks/api/0.8/05-custom-policy.ipynb">05-custom-policy.ipynb</a>
-- <a href="https://github.com/OpenMined/PySyft/tree/0.8.6/notebooks/api/0.8/06-multiple-code-requests.ipynb">06-multiple-code-requests.ipynb</a>
-- <a href="https://github.com/OpenMined/PySyft/tree/0.8.6/notebooks/api/0.8/07-domain-register-control-flow.ipynb">07-domain-register-control-flow.ipynb</a>
-- <a href="https://github.com/OpenMined/PySyft/tree/0.8.6/notebooks/api/0.8/08-code-version.ipynb">08-code-version.ipynb</a>
-- <a href="https://github.com/OpenMined/PySyft/tree/0.8.6/notebooks/api/0.8/09-blob-storage.ipynb">09-blob-storage.ipynb</a>
-- <a href="https://github.com/OpenMined/PySyft/tree/0.8.6/notebooks/api/0.8/10-container-images.ipynb">10-container-images.ipynb</a>
-- <a href="https://github.com/OpenMined/PySyft/tree/0.8.6/notebooks/api/0.8/11-container-images-k8s.ipynb">11-container-images-k8s.ipynb</a>
+- <a href="https://github.com/OpenMined/PySyft/tree/0.8.7/notebooks/api/0.8/00-load-data.ipynb">00-load-data.ipynb</a>
+- <a href="https://github.com/OpenMined/PySyft/tree/0.8.7/notebooks/api/0.8/01-submit-code.ipynb">01-submit-code.ipynb</a>
+- <a href="https://github.com/OpenMined/PySyft/tree/0.8.7/notebooks/api/0.8/02-review-code-and-approve.ipynb">02-review-code-and-approve.ipynb</a>
+- <a href="https://github.com/OpenMined/PySyft/tree/0.8.7/notebooks/api/0.8/03-data-scientist-download-result.ipynb">03-data-scientist-download-result.ipynb</a>
+- <a href="https://github.com/OpenMined/PySyft/tree/0.8.7/notebooks/api/0.8/04-jax-example.ipynb">04-jax-example.ipynb</a>
+- <a href="https://github.com/OpenMined/PySyft/tree/0.8.7/notebooks/api/0.8/05-custom-policy.ipynb">05-custom-policy.ipynb</a>
+- <a href="https://github.com/OpenMined/PySyft/tree/0.8.7/notebooks/api/0.8/06-multiple-code-requests.ipynb">06-multiple-code-requests.ipynb</a>
+- <a href="https://github.com/OpenMined/PySyft/tree/0.8.7/notebooks/api/0.8/07-domain-register-control-flow.ipynb">07-domain-register-control-flow.ipynb</a>
+- <a href="https://github.com/OpenMined/PySyft/tree/0.8.7/notebooks/api/0.8/08-code-version.ipynb">08-code-version.ipynb</a>
+- <a href="https://github.com/OpenMined/PySyft/tree/0.8.7/notebooks/api/0.8/09-blob-storage.ipynb">09-blob-storage.ipynb</a>
+- <a href="https://github.com/OpenMined/PySyft/tree/0.8.7/notebooks/api/0.8/10-container-images.ipynb">10-container-images.ipynb</a>
+- <a href="https://github.com/OpenMined/PySyft/tree/0.8.7/notebooks/api/0.8/11-container-images-k8s.ipynb">11-container-images-k8s.ipynb</a>
 
 ## Deploy Kubernetes Helm Chart
 
 **Note**: Assuming we have a Kubernetes cluster already setup.
 
 #### 1. Add and update Helm repo for Syft
 
@@ -233,19 +234,20 @@
 - Interactive Install 🧙🏽‍♂️ Wizard<sup>BETA</sup> Requires 🛵 `hagrid`: - Run: `hagrid quickstart`
 - PySyft 0.8.1 Requires: 🐍 `python 3.10 - 3.12` - Run: `pip install -U syft`
 - PyGrid Requires: 🐳 `docker`, 🦦 `podman` or ☸️ `kubernetes` - Run: `hagrid launch ...`
 
 # Versions
 
 `0.9.0` - Coming soon...  
-`0.8.6` (Beta) - `dev` branch 👈🏽 <a href="https://github.com/OpenMined/PySyft/tree/dev/notebooks/api/0.8">API</a> - Coming soon...  
-`0.8.5` (Stable) - <a href="https://github.com/OpenMined/PySyft/tree/0.8.5/notebooks/api/0.8">API</a>
+`0.8.7` (Beta) - `dev` branch 👈🏽 <a href="https://github.com/OpenMined/PySyft/tree/dev/notebooks/api/0.8">API</a> - Coming soon...  
+`0.8.6` (Stable) - <a href="https://github.com/OpenMined/PySyft/tree/0.8.6/notebooks/api/0.8">API</a>
 
 Deprecated:
 
+- `0.8.5-post.2` - <a href="https://github.com/OpenMined/PySyft/tree/0.8.5-post.2/notebooks/api/0.8">API</a>
 - `0.8.4` - <a href="https://github.com/OpenMined/PySyft/tree/0.8.4/notebooks/api/0.8">API</a>
 - `0.8.3` - <a href="https://github.com/OpenMined/PySyft/tree/0.8.3/notebooks/api/0.8">API</a>
 - `0.8.2` - <a href="https://github.com/OpenMined/PySyft/tree/0.8.2/notebooks/api/0.8">API</a>
 - `0.8.1` - <a href="https://github.com/OpenMined/PySyft/tree/0.8.1/notebooks/api/0.8">API</a>
 - `0.8.0` - <a href="https://github.com/OpenMined/PySyft/tree/0.8/notebooks/api/0.8">API</a>
 - `0.7.0` - <a href="https://github.com/OpenMined/courses/tree/introduction-to-remote-data-science-dev">Course 3 Updated</a>
 - `0.6.0` - <a href="https://github.com/OpenMined/courses/tree/introduction-to-remote-data-science">Course 3</a>
@@ -260,15 +262,15 @@
 PySyft (Beta): `pip install -U syft --pre`  
 PyGrid (Beta): `hagrid launch ... tag=beta`
 
 HAGrid is a cli / deployment tool so the latest version of `hagrid` is usually the best.
 
 # What is Syft?
 
-<img align="right" src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.6/docs/img/logo_big.png" alt="Syft" height="250" style="padding-left:30px;">
+<img align="right" src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.7/docs/img/logo_big.png" alt="Syft" height="250" style="padding-left:30px;">
 
 `Syft` is OpenMined's `open source` stack that provides `secure` and `private` Data Science in Python. Syft decouples `private data` from model training, using techniques like [Federated Learning](https://ai.googleblog.com/2017/04/federated-learning-collaborative.html), [Differential Privacy](https://en.wikipedia.org/wiki/Differential_privacy), and [Encrypted Computation](https://en.wikipedia.org/wiki/Homomorphic_encryption). This is done with a `numpy`-like interface and integration with `Deep Learning` frameworks, so that you as a `Data Scientist` can maintain your current workflow while using these new `privacy-enhancing techniques`.
 
 ### Why should I use Syft?
 
 `Syft` allows a `Data Scientist` to ask `questions` about a `dataset` and, within `privacy limits` set by the `data owner`, get `answers` to those `questions`, all without obtaining a `copy` of the data itself. We call this process `Remote Data Science`. It means in a wide variety of `domains` across society, the current `risks` of sharing information (`copying` data) with someone such as, privacy invasion, IP theft and blackmail will no longer prevent the vast `benefits` such as innovation, insights and scientific discovery which secure access will provide.
 
@@ -278,39 +280,39 @@
 # Tutorials
 
 <table border="5" bordercolor="grey">
 <tr>
 <th align="center">
 <img width="441" height="1">
 <div align="center">
-<img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.6/docs/img/personas_image/dataowner.png" alt="" width="100" height="100" align="center">
+<img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.7/docs/img/personas_image/dataowner.png" alt="" width="100" height="100" align="center">
 <p>Data Owner</p></div>
 </th>
 <th align="center">
 <img width="441" height="1">
-<div align="center"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.6/docs/img/personas_image/datascientist.png" alt="" width="100" height="100" align="center">
+<div align="center"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.7/docs/img/personas_image/datascientist.png" alt="" width="100" height="100" align="center">
 <p>Data Scientist</p></div>
 
 </th>
 <th align="center">
 <img width="441" height="1">
 <div align="center">
-<img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.6/docs/img/personas_image/dataengineer.png" alt="" width="100" height="100" align="center">
+<img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.7/docs/img/personas_image/dataengineer.png" alt="" width="100" height="100" align="center">
 <p>Data Engineer</p>
 </div>
 </th>
 </tr>
 <tr>
 <td valign="top">
 
-- <a href="https://github.com/OpenMined/PySyft/tree/0.8.6/notebooks/quickstart/data-owner/00-deploy-domain.ipynb">Deploy a Domain Server</a>
-- <a href="https://github.com/OpenMined/PySyft/tree/0.8.6/notebooks/quickstart/data-owner/01-upload-data.ipynb">Upload Private Data</a>
-- <a href="https://github.com/OpenMined/PySyft/tree/0.8.6/notebooks/quickstart/data-owner/02-create-account-configure-pb.ipynb">Create Accounts</a>
+- <a href="https://github.com/OpenMined/PySyft/tree/0.8.7/notebooks/quickstart/data-owner/00-deploy-domain.ipynb">Deploy a Domain Server</a>
+- <a href="https://github.com/OpenMined/PySyft/tree/0.8.7/notebooks/quickstart/data-owner/01-upload-data.ipynb">Upload Private Data</a>
+- <a href="https://github.com/OpenMined/PySyft/tree/0.8.7/notebooks/quickstart/data-owner/02-create-account-configure-pb.ipynb">Create Accounts</a>
 - Manage Privacy Budget</a>
-- <a href="https://github.com/OpenMined/PySyft/tree/0.8.6/notebooks/quickstart/data-owner/03-join-network.ipynb">Join a Network</a>
+- <a href="https://github.com/OpenMined/PySyft/tree/0.8.7/notebooks/quickstart/data-owner/03-join-network.ipynb">Join a Network</a>
 - Learn how PETs streamline Data Policies
 
 </td>
 <td valign="top">
 
 - Install Syft</a>
 - Connect to a Domain</a>
@@ -390,25 +392,25 @@
 
 <table border="5" bordercolor="grey">
 <tr>
 <th align="center" valign="top">
 <img width="441" height="1">
 <div align="center">
 
-<img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.6/docs/img/panel_slack_title_light.png" alt="" width="100%" align="center" />
+<img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.7/docs/img/panel_slack_title_light.png" alt="" width="100%" align="center" />
 
-<a href="https://slack.openmined.org/"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.6/docs/img/panel_slack.png" alt="" width="100%" align="center" /></a>
+<a href="https://slack.openmined.org/"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.7/docs/img/panel_slack.png" alt="" width="100%" align="center" /></a>
 
 </div>
 </th>
 <th align="center" valign="top">
 <img width="441" height="1">
 <div align="center">
 
-<img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.6/docs/img/panel_title_videos_papers_light.png" alt="" width="100%" align="center" />
+<img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.7/docs/img/panel_title_videos_papers_light.png" alt="" width="100%" align="center" />
 
 <p align="left"><sub><sup>
 🎥 <a href="https://www.youtube.com/watch?v=qVf0tPBzr2k">PETs: Remote Data Science Unleashed - R gov 2021</a><br />
 🎥 <a href="https://youtu.be/sCoDWKTbh3s?list=PL_lsbAsL_o2BQKXG7mkGFA8LSApCnhljL">Introduction to Remote Data Science - PyTorch 2021</a><br />
 🎥 <a href="https://youtu.be/kzLeTz_vIeQ?list=PL_lsbAsL_o2BtOz6KUfUI_Zla6Rg5dmyc">The Future of AI Tools - PyTorch 2020</a><br />
 🎥 <a href="https://www.youtube.com/watch?v=4zrU54VIK6k&t=1s">Privacy Preserving AI - MIT Deep Learning Series</a><br />
 🎥 <a href="https://www.youtube.com/watch?v=Pr4erdusiW0">Privacy-Preserving Data Science - TWiML Talk #241</a><br />
@@ -419,106 +421,106 @@
 </sup></sup></p>
 </div>
 </th>
 <th align="center" valign="top">
 <img width="441" height="1">
 <div align="center">
 
-<img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.6/docs/img/panel_padawan_title_light.png" alt="" width="100%" align="center" />
+<img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.7/docs/img/panel_padawan_title_light.png" alt="" width="100%" align="center" />
 
-<a href="https://blog.openmined.org/work-on-ais-most-exciting-frontier-no-phd-required/"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.6/docs/img/panel_padawan.png" alt="" width="100%" align="center"></a>
+<a href="https://blog.openmined.org/work-on-ais-most-exciting-frontier-no-phd-required/"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.7/docs/img/panel_padawan.png" alt="" width="100%" align="center"></a>
 
 </div>
 </th>
 </tr>
 </table>
 
 # Courses
 
 <table border="5" bordercolor="grey">
 <tr>
 <th align="center">
 <img width="441" height="1">
 <div align="center">
-<a href="https://courses.openmined.org/courses/our-privacy-opportunity"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.6/docs/img/course_privacy.png" alt="" width="100%" align="center" /></a>
+<a href="https://courses.openmined.org/courses/our-privacy-opportunity"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.7/docs/img/course_privacy.png" alt="" width="100%" align="center" /></a>
 </th>
 <th align="center">
 <img width="441" height="1">
 <div align="center">
-<a href="https://courses.openmined.org/courses/foundations-of-private-computation"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.6/docs/img/course_foundations.png" alt="" width="100%" align="center" /></a>
+<a href="https://courses.openmined.org/courses/foundations-of-private-computation"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.7/docs/img/course_foundations.png" alt="" width="100%" align="center" /></a>
 </div>
 </th>
 <th align="center">
 <img width="441" height="1">
 <div align="center">
-<a href="https://courses.openmined.org/courses/introduction-to-remote-data-science"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.6/docs/img/course_introduction.png" alt="" width="100%" align="center"></a>
+<a href="https://courses.openmined.org/courses/introduction-to-remote-data-science"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.7/docs/img/course_introduction.png" alt="" width="100%" align="center"></a>
 </div>
 </th>
 </tr>
 </table>
 
 # Contributors
 
 OpenMined and Syft appreciates all contributors, if you would like to fix a bug or suggest a new feature, please see our [guidelines](https://openmined.github.io/PySyft/developer_guide/index.html).<br />
 
-<img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.6/docs/img/contributors_light.jpg" alt="Contributors" width="100%" />
+<img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.7/docs/img/contributors_light.jpg" alt="Contributors" width="100%" />
 
 # Supporters
 
 <table border="0">
 <tr>
 <th align="center">
-<a href="https://sloan.org/"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.6/docs/img/logo_sloan.png" /></a>
+<a href="https://sloan.org/"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.7/docs/img/logo_sloan.png" /></a>
 </th>
 <th align="center">
-<a href="https://opensource.fb.com/"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.6/docs/img/logo_meta.png" /></a>
+<a href="https://opensource.fb.com/"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.7/docs/img/logo_meta.png" /></a>
 </th>
 <th align="center">
-<a href="https://pytorch.org/"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.6/docs/img/logo_torch.png" /></a>
+<a href="https://pytorch.org/"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.7/docs/img/logo_torch.png" /></a>
 </th>
 <th align="center">
 <a href="https://www.dpmc.govt.nz/">
-<img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.6/docs/img/logo_nz_light.png" />
+<img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.7/docs/img/logo_nz_light.png" />
 </a>
 </th>
 <th align="center">
-<a href="https://twitter.com/"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.6/docs/img/logo_twitter.png" /></a>
+<a href="https://twitter.com/"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.7/docs/img/logo_twitter.png" /></a>
 </th>
 <th align="center">
-<a href="https://google.com/"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.6/docs/img/logo_google.png" /></a>
+<a href="https://google.com/"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.7/docs/img/logo_google.png" /></a>
 </th>
 <th align="center">
-<a href="https://microsoft.com/"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.6/docs/img/logo_microsoft.png" /></a>
+<a href="https://microsoft.com/"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.7/docs/img/logo_microsoft.png" /></a>
 </th>
 <th align="center">
-<a href="https://omidyar.com/"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.6/docs/img/logo_on.png" /></a>
+<a href="https://omidyar.com/"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.7/docs/img/logo_on.png" /></a>
 </th>
 <th align="center">
-<a href="https://www.udacity.com/"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.6/docs/img/logo_udacity.png" /></a>
+<a href="https://www.udacity.com/"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.7/docs/img/logo_udacity.png" /></a>
 </th>
 <th align="center">
 <a href="https://www.centerfordigitalhealthinnovation.org/">
 
-<img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.6/docs/img/logo_cdhi_light.png" />
+<img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.7/docs/img/logo_cdhi_light.png" />
 
 </a>
 </th>
 <th align="center">
 <a href="https://arkhn.org/">
-<img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.6/docs/img/logo_arkhn_light.png" />
+<img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.7/docs/img/logo_arkhn_light.png" />
 </a>
 </th>
 </tr>
 </table>
 
 # Open Collective
 
 `OpenMined` is a fiscally sponsored `501(c)(3)` in the USA. We are funded by our generous supporters on <a href="https://opencollective.com/openmined">Open Collective</a>. <br /><br />
 
-<img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.6/docs/img/opencollective_light.png" alt="Contributors" width="100%" />
+<img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.7/docs/img/opencollective_light.png" alt="Contributors" width="100%" />
 
 # Disclaimer
 
 Syft is under active development and is not yet ready for pilots on private data without our assistance. As early access participants, please contact us via [Slack](https://slack.openmined.org/) or email if you would like to ask a question or have a use case that you would like to discuss.
 
 # License
```

### Comparing `syft-0.8.6b1/PYPI.md` & `syft-0.8.7b1/PYPI.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 <div align="left"> <a href="https://pypi.org/project/syft/"><img src="https://static.pepy.tech/badge/pysyft" /></a> <a href="https://pypi.org/project/syft/"><img src="https://badge.fury.io/py/syft.svg" /></a> <a href="https://hub.docker.com/u/openmined"><img src="https://img.shields.io/badge/docker-images-blue?logo=docker" /></a> <a href="https://github.com/OpenMined/PySyft/actions/workflows/nightlies.yml"><img src="https://github.com/OpenMined/PySyft/actions/workflows/nightlies.yml/badge.svg?branch=dev" /></a> <a href="https://slack.openmined.org/"><img src="https://img.shields.io/badge/chat-on%20slack-purple?logo=slack" /></a> <a href="https://openmined.github.io/PySyft/"><img src="https://img.shields.io/badge/read-docs-yellow?logo=mdbook" /></a>
 <br /><br /></div>
 
-<img alt="Syft Logo" src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.6/docs/img/title_syft_light.png" width="200px" />
+<img alt="Syft Logo" src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.7/docs/img/title_syft_light.png" width="200px" />
 
 Perform data science on `data` that remains in `someone else's` server
 
 # Quickstart
 
 ✅ `Linux` ✅ `macOS` ✅ `Windows` ✅ `Docker` ✅ `Podman` ✅ `Kubernetes`
 
@@ -16,49 +16,49 @@
 ```
 
 ## Launch Server
 
 ```python
 # from Jupyter / Python
 import syft as sy
-sy.requires(">=0.8.5,<0.8.6")
+sy.requires(">=0.8.6,<0.8.7")
 node = sy.orchestra.launch(name="my-domain", port=8080, dev_mode=True, reset=True)
 ```
 
 ```bash
 # or from the command line
 $ syft launch --name=my-domain --port=8080 --reset=True
 
 Starting syft-node server on 0.0.0.0:8080
 ```
 
 ## Launch Client
 
 ```python
 import syft as sy
-sy.requires(">=0.8.5,<0.8.6")
+sy.requires(">=0.8.6,<0.8.7")
 domain_client = sy.login(port=8080, email="info@openmined.org", password="changethis")
 ```
 
 ## PySyft in 10 minutes
 
-📝 <a href="https://github.com/OpenMined/PySyft/tree/0.8.6/notebooks/api">API Example Notebooks</a>
+📝 <a href="https://github.com/OpenMined/PySyft/tree/0.8.7/notebooks/api">API Example Notebooks</a>
 
-- <a href="https://github.com/OpenMined/PySyft/tree/0.8.6/notebooks/api/0.8/00-load-data.ipynb">00-load-data.ipynb</a>
-- <a href="https://github.com/OpenMined/PySyft/tree/0.8.6/notebooks/api/0.8/01-submit-code.ipynb">01-submit-code.ipynb</a>
-- <a href="https://github.com/OpenMined/PySyft/tree/0.8.6/notebooks/api/0.8/02-review-code-and-approve.ipynb">02-review-code-and-approve.ipynb</a>
-- <a href="https://github.com/OpenMined/PySyft/tree/0.8.6/notebooks/api/0.8/03-data-scientist-download-result.ipynb">03-data-scientist-download-result.ipynb</a>
-- <a href="https://github.com/OpenMined/PySyft/tree/0.8.6/notebooks/api/0.8/04-jax-example.ipynb">04-jax-example.ipynb</a>
-- <a href="https://github.com/OpenMined/PySyft/tree/0.8.6/notebooks/api/0.8/05-custom-policy.ipynb">05-custom-policy.ipynb</a>
-- <a href="https://github.com/OpenMined/PySyft/tree/0.8.6/notebooks/api/0.8/06-multiple-code-requests.ipynb">06-multiple-code-requests.ipynb</a>
-- <a href="https://github.com/OpenMined/PySyft/tree/0.8.6/notebooks/api/0.8/07-domain-register-control-flow.ipynb">07-domain-register-control-flow.ipynb</a>
-- <a href="https://github.com/OpenMined/PySyft/tree/0.8.6/notebooks/api/0.8/08-code-version.ipynb">08-code-version.ipynb</a>
-- <a href="https://github.com/OpenMined/PySyft/tree/0.8.6/notebooks/api/0.8/09-blob-storage.ipynb">09-blob-storage.ipynb</a>
-- <a href="https://github.com/OpenMined/PySyft/tree/0.8.6/notebooks/api/0.8/10-container-images.ipynb">10-container-images.ipynb</a>
-- <a href="https://github.com/OpenMined/PySyft/tree/0.8.6/notebooks/api/0.8/11-container-images-k8s.ipynb">11-container-images-k8s.ipynb</a>
+- <a href="https://github.com/OpenMined/PySyft/tree/0.8.7/notebooks/api/0.8/00-load-data.ipynb">00-load-data.ipynb</a>
+- <a href="https://github.com/OpenMined/PySyft/tree/0.8.7/notebooks/api/0.8/01-submit-code.ipynb">01-submit-code.ipynb</a>
+- <a href="https://github.com/OpenMined/PySyft/tree/0.8.7/notebooks/api/0.8/02-review-code-and-approve.ipynb">02-review-code-and-approve.ipynb</a>
+- <a href="https://github.com/OpenMined/PySyft/tree/0.8.7/notebooks/api/0.8/03-data-scientist-download-result.ipynb">03-data-scientist-download-result.ipynb</a>
+- <a href="https://github.com/OpenMined/PySyft/tree/0.8.7/notebooks/api/0.8/04-jax-example.ipynb">04-jax-example.ipynb</a>
+- <a href="https://github.com/OpenMined/PySyft/tree/0.8.7/notebooks/api/0.8/05-custom-policy.ipynb">05-custom-policy.ipynb</a>
+- <a href="https://github.com/OpenMined/PySyft/tree/0.8.7/notebooks/api/0.8/06-multiple-code-requests.ipynb">06-multiple-code-requests.ipynb</a>
+- <a href="https://github.com/OpenMined/PySyft/tree/0.8.7/notebooks/api/0.8/07-domain-register-control-flow.ipynb">07-domain-register-control-flow.ipynb</a>
+- <a href="https://github.com/OpenMined/PySyft/tree/0.8.7/notebooks/api/0.8/08-code-version.ipynb">08-code-version.ipynb</a>
+- <a href="https://github.com/OpenMined/PySyft/tree/0.8.7/notebooks/api/0.8/09-blob-storage.ipynb">09-blob-storage.ipynb</a>
+- <a href="https://github.com/OpenMined/PySyft/tree/0.8.7/notebooks/api/0.8/10-container-images.ipynb">10-container-images.ipynb</a>
+- <a href="https://github.com/OpenMined/PySyft/tree/0.8.7/notebooks/api/0.8/11-container-images-k8s.ipynb">11-container-images-k8s.ipynb</a>
 
 ## Deploy Kubernetes Helm Chart
 
 **Note**: Assuming we have a Kubernetes cluster already setup.
 
 #### 1. Add and update Helm repo for Syft
 
@@ -129,19 +129,20 @@
 - Interactive Install 🧙🏽‍♂️ Wizard<sup>BETA</sup> Requires 🛵 `hagrid`: - Run: `hagrid quickstart`
 - PySyft 0.8.1 Requires: 🐍 `python 3.10 - 3.12` - Run: `pip install -U syft`
 - PyGrid Requires: 🐳 `docker`, 🦦 `podman` or ☸️ `kubernetes` - Run: `hagrid launch ...`
 
 # Versions
 
 `0.9.0` - Coming soon...  
-`0.8.6` (Beta) - `dev` branch 👈🏽 <a href="https://github.com/OpenMined/PySyft/tree/dev/notebooks/api/0.8">API</a> - Coming soon...  
-`0.8.5` (Stable) - <a href="https://github.com/OpenMined/PySyft/tree/0.8.5/notebooks/api/0.8">API</a>
+`0.8.7` (Beta) - `dev` branch 👈🏽 <a href="https://github.com/OpenMined/PySyft/tree/dev/notebooks/api/0.8">API</a> - Coming soon...  
+`0.8.6` (Stable) - <a href="https://github.com/OpenMined/PySyft/tree/0.8.6/notebooks/api/0.8">API</a>
 
 Deprecated:
 
+- `0.8.5-post.2` - <a href="https://github.com/OpenMined/PySyft/tree/0.8.5-post.2/notebooks/api/0.8">API</a>
 - `0.8.4` - <a href="https://github.com/OpenMined/PySyft/tree/0.8.4/notebooks/api/0.8">API</a>
 - `0.8.3` - <a href="https://github.com/OpenMined/PySyft/tree/0.8.3/notebooks/api/0.8">API</a>
 - `0.8.2` - <a href="https://github.com/OpenMined/PySyft/tree/0.8.2/notebooks/api/0.8">API</a>
 - `0.8.1` - <a href="https://github.com/OpenMined/PySyft/tree/0.8.1/notebooks/api/0.8">API</a>
 - `0.8.0` - <a href="https://github.com/OpenMined/PySyft/tree/0.8/notebooks/api/0.8">API</a>
 - `0.7.0` - <a href="https://github.com/OpenMined/courses/tree/introduction-to-remote-data-science-dev">Course 3 Updated</a>
 - `0.6.0` - <a href="https://github.com/OpenMined/courses/tree/introduction-to-remote-data-science">Course 3</a>
@@ -156,15 +157,15 @@
 PySyft (Beta): `pip install -U syft --pre`  
 PyGrid (Beta): `hagrid launch ... tag=beta`
 
 HAGrid is a cli / deployment tool so the latest version of `hagrid` is usually the best.
 
 # What is Syft?
 
-<img align="right" src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.6/docs/img/logo_big.png" alt="Syft" height="250" style="padding-left:30px;">
+<img align="right" src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.7/docs/img/logo_big.png" alt="Syft" height="250" style="padding-left:30px;">
 
 `Syft` is OpenMined's `open source` stack that provides `secure` and `private` Data Science in Python. Syft decouples `private data` from model training, using techniques like [Federated Learning](https://ai.googleblog.com/2017/04/federated-learning-collaborative.html), [Differential Privacy](https://en.wikipedia.org/wiki/Differential_privacy), and [Encrypted Computation](https://en.wikipedia.org/wiki/Homomorphic_encryption). This is done with a `numpy`-like interface and integration with `Deep Learning` frameworks, so that you as a `Data Scientist` can maintain your current workflow while using these new `privacy-enhancing techniques`.
 
 ### Why should I use Syft?
 
 `Syft` allows a `Data Scientist` to ask `questions` about a `dataset` and, within `privacy limits` set by the `data owner`, get `answers` to those `questions`, all without obtaining a `copy` of the data itself. We call this process `Remote Data Science`. It means in a wide variety of `domains` across society, the current `risks` of sharing information (`copying` data) with someone such as, privacy invasion, IP theft and blackmail will no longer prevent the vast `benefits` such as innovation, insights and scientific discovery which secure access will provide.
 
@@ -174,39 +175,39 @@
 # Tutorials
 
 <table border="5" bordercolor="grey">
 <tr>
 <th align="center">
 <img width="441" height="1">
 <div align="center">
-<img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.6/docs/img/personas_image/dataowner.png" alt="" width="100" height="100" align="center">
+<img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.7/docs/img/personas_image/dataowner.png" alt="" width="100" height="100" align="center">
 <p>Data Owner</p></div>
 </th>
 <th align="center">
 <img width="441" height="1">
-<div align="center"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.6/docs/img/personas_image/datascientist.png" alt="" width="100" height="100" align="center">
+<div align="center"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.7/docs/img/personas_image/datascientist.png" alt="" width="100" height="100" align="center">
 <p>Data Scientist</p></div>
 
 </th>
 <th align="center">
 <img width="441" height="1">
 <div align="center">
-<img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.6/docs/img/personas_image/dataengineer.png" alt="" width="100" height="100" align="center">
+<img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.7/docs/img/personas_image/dataengineer.png" alt="" width="100" height="100" align="center">
 <p>Data Engineer</p>
 </div>
 </th>
 </tr>
 <tr>
 <td valign="top">
 
-- <a href="https://github.com/OpenMined/PySyft/tree/0.8.6/notebooks/quickstart/data-owner/00-deploy-domain.ipynb">Deploy a Domain Server</a>
-- <a href="https://github.com/OpenMined/PySyft/tree/0.8.6/notebooks/quickstart/data-owner/01-upload-data.ipynb">Upload Private Data</a>
-- <a href="https://github.com/OpenMined/PySyft/tree/0.8.6/notebooks/quickstart/data-owner/02-create-account-configure-pb.ipynb">Create Accounts</a>
+- <a href="https://github.com/OpenMined/PySyft/tree/0.8.7/notebooks/quickstart/data-owner/00-deploy-domain.ipynb">Deploy a Domain Server</a>
+- <a href="https://github.com/OpenMined/PySyft/tree/0.8.7/notebooks/quickstart/data-owner/01-upload-data.ipynb">Upload Private Data</a>
+- <a href="https://github.com/OpenMined/PySyft/tree/0.8.7/notebooks/quickstart/data-owner/02-create-account-configure-pb.ipynb">Create Accounts</a>
 - Manage Privacy Budget</a>
-- <a href="https://github.com/OpenMined/PySyft/tree/0.8.6/notebooks/quickstart/data-owner/03-join-network.ipynb">Join a Network</a>
+- <a href="https://github.com/OpenMined/PySyft/tree/0.8.7/notebooks/quickstart/data-owner/03-join-network.ipynb">Join a Network</a>
 - Learn how PETs streamline Data Policies
 
 </td>
 <td valign="top">
 
 - Install Syft</a>
 - Connect to a Domain</a>
@@ -286,25 +287,25 @@
 
 <table border="5" bordercolor="grey">
 <tr>
 <th align="center" valign="top">
 <img width="441" height="1">
 <div align="center">
 
-<img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.6/docs/img/panel_slack_title_light.png" alt="" width="100%" align="center" />
+<img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.7/docs/img/panel_slack_title_light.png" alt="" width="100%" align="center" />
 
-<a href="https://slack.openmined.org/"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.6/docs/img/panel_slack.png" alt="" width="100%" align="center" /></a>
+<a href="https://slack.openmined.org/"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.7/docs/img/panel_slack.png" alt="" width="100%" align="center" /></a>
 
 </div>
 </th>
 <th align="center" valign="top">
 <img width="441" height="1">
 <div align="center">
 
-<img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.6/docs/img/panel_title_videos_papers_light.png" alt="" width="100%" align="center" />
+<img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.7/docs/img/panel_title_videos_papers_light.png" alt="" width="100%" align="center" />
 
 <p align="left"><sub><sup>
 🎥 <a href="https://www.youtube.com/watch?v=qVf0tPBzr2k">PETs: Remote Data Science Unleashed - R gov 2021</a><br />
 🎥 <a href="https://youtu.be/sCoDWKTbh3s?list=PL_lsbAsL_o2BQKXG7mkGFA8LSApCnhljL">Introduction to Remote Data Science - PyTorch 2021</a><br />
 🎥 <a href="https://youtu.be/kzLeTz_vIeQ?list=PL_lsbAsL_o2BtOz6KUfUI_Zla6Rg5dmyc">The Future of AI Tools - PyTorch 2020</a><br />
 🎥 <a href="https://www.youtube.com/watch?v=4zrU54VIK6k&t=1s">Privacy Preserving AI - MIT Deep Learning Series</a><br />
 🎥 <a href="https://www.youtube.com/watch?v=Pr4erdusiW0">Privacy-Preserving Data Science - TWiML Talk #241</a><br />
@@ -315,106 +316,106 @@
 </sup></sup></p>
 </div>
 </th>
 <th align="center" valign="top">
 <img width="441" height="1">
 <div align="center">
 
-<img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.6/docs/img/panel_padawan_title_light.png" alt="" width="100%" align="center" />
+<img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.7/docs/img/panel_padawan_title_light.png" alt="" width="100%" align="center" />
 
-<a href="https://blog.openmined.org/work-on-ais-most-exciting-frontier-no-phd-required/"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.6/docs/img/panel_padawan.png" alt="" width="100%" align="center"></a>
+<a href="https://blog.openmined.org/work-on-ais-most-exciting-frontier-no-phd-required/"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.7/docs/img/panel_padawan.png" alt="" width="100%" align="center"></a>
 
 </div>
 </th>
 </tr>
 </table>
 
 # Courses
 
 <table border="5" bordercolor="grey">
 <tr>
 <th align="center">
 <img width="441" height="1">
 <div align="center">
-<a href="https://courses.openmined.org/courses/our-privacy-opportunity"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.6/docs/img/course_privacy.png" alt="" width="100%" align="center" /></a>
+<a href="https://courses.openmined.org/courses/our-privacy-opportunity"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.7/docs/img/course_privacy.png" alt="" width="100%" align="center" /></a>
 </th>
 <th align="center">
 <img width="441" height="1">
 <div align="center">
-<a href="https://courses.openmined.org/courses/foundations-of-private-computation"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.6/docs/img/course_foundations.png" alt="" width="100%" align="center" /></a>
+<a href="https://courses.openmined.org/courses/foundations-of-private-computation"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.7/docs/img/course_foundations.png" alt="" width="100%" align="center" /></a>
 </div>
 </th>
 <th align="center">
 <img width="441" height="1">
 <div align="center">
-<a href="https://courses.openmined.org/courses/introduction-to-remote-data-science"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.6/docs/img/course_introduction.png" alt="" width="100%" align="center"></a>
+<a href="https://courses.openmined.org/courses/introduction-to-remote-data-science"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.7/docs/img/course_introduction.png" alt="" width="100%" align="center"></a>
 </div>
 </th>
 </tr>
 </table>
 
 # Contributors
 
 OpenMined and Syft appreciates all contributors, if you would like to fix a bug or suggest a new feature, please see our [guidelines](https://openmined.github.io/PySyft/developer_guide/index.html).<br />
 
-<img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.6/docs/img/contributors_light.jpg" alt="Contributors" width="100%" />
+<img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.7/docs/img/contributors_light.jpg" alt="Contributors" width="100%" />
 
 # Supporters
 
 <table border="0">
 <tr>
 <th align="center">
-<a href="https://sloan.org/"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.6/docs/img/logo_sloan.png" /></a>
+<a href="https://sloan.org/"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.7/docs/img/logo_sloan.png" /></a>
 </th>
 <th align="center">
-<a href="https://opensource.fb.com/"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.6/docs/img/logo_meta.png" /></a>
+<a href="https://opensource.fb.com/"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.7/docs/img/logo_meta.png" /></a>
 </th>
 <th align="center">
-<a href="https://pytorch.org/"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.6/docs/img/logo_torch.png" /></a>
+<a href="https://pytorch.org/"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.7/docs/img/logo_torch.png" /></a>
 </th>
 <th align="center">
 <a href="https://www.dpmc.govt.nz/">
-<img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.6/docs/img/logo_nz_light.png" />
+<img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.7/docs/img/logo_nz_light.png" />
 </a>
 </th>
 <th align="center">
-<a href="https://twitter.com/"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.6/docs/img/logo_twitter.png" /></a>
+<a href="https://twitter.com/"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.7/docs/img/logo_twitter.png" /></a>
 </th>
 <th align="center">
-<a href="https://google.com/"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.6/docs/img/logo_google.png" /></a>
+<a href="https://google.com/"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.7/docs/img/logo_google.png" /></a>
 </th>
 <th align="center">
-<a href="https://microsoft.com/"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.6/docs/img/logo_microsoft.png" /></a>
+<a href="https://microsoft.com/"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.7/docs/img/logo_microsoft.png" /></a>
 </th>
 <th align="center">
-<a href="https://omidyar.com/"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.6/docs/img/logo_on.png" /></a>
+<a href="https://omidyar.com/"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.7/docs/img/logo_on.png" /></a>
 </th>
 <th align="center">
-<a href="https://www.udacity.com/"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.6/docs/img/logo_udacity.png" /></a>
+<a href="https://www.udacity.com/"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.7/docs/img/logo_udacity.png" /></a>
 </th>
 <th align="center">
 <a href="https://www.centerfordigitalhealthinnovation.org/">
 
-<img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.6/docs/img/logo_cdhi_light.png" />
+<img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.7/docs/img/logo_cdhi_light.png" />
 
 </a>
 </th>
 <th align="center">
 <a href="https://arkhn.org/">
-<img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.6/docs/img/logo_arkhn_light.png" />
+<img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.7/docs/img/logo_arkhn_light.png" />
 </a>
 </th>
 </tr>
 </table>
 
 # Open Collective
 
 `OpenMined` is a fiscally sponsored `501(c)(3)` in the USA. We are funded by our generous supporters on <a href="https://opencollective.com/openmined">Open Collective</a>. <br /><br />
 
-<img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.6/docs/img/opencollective_light.png" alt="Contributors" width="100%" />
+<img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.7/docs/img/opencollective_light.png" alt="Contributors" width="100%" />
 
 # Disclaimer
 
 Syft is under active development and is not yet ready for pilots on private data without our assistance. As early access participants, please contact us via [Slack](https://slack.openmined.org/) or email if you would like to ask a question or have a use case that you would like to discuss.
 
 # License
```

#### html2text {}

```diff
@@ -4,19 +4,19 @@
 _b_a_d_g_e_._s_v_g_?_b_r_a_n_c_h_=_d_e_v_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_c_h_a_t_-_o_n_%_2_0_s_l_a_c_k_-
 _p_u_r_p_l_e_?_l_o_g_o_=_s_l_a_c_k_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_r_e_a_d_-_d_o_c_s_-_y_e_l_l_o_w_?_l_o_g_o_=_m_d_b_o_o_k_]
 
 [Syft Logo]Perform data science on `data` that remains in `someone else's`
 server # Quickstart â `Linux` â `macOS` â `Windows` â `Docker` â
 `Podman` â `Kubernetes` ## Install Client ```bash $ pip install -U syft
 [data_science] ``` ## Launch Server ```python # from Jupyter / Python import
-syft as sy sy.requires(">=0.8.5,<0.8.6") node = sy.orchestra.launch(name="my-
+syft as sy sy.requires(">=0.8.6,<0.8.7") node = sy.orchestra.launch(name="my-
 domain", port=8080, dev_mode=True, reset=True) ``` ```bash # or from the
 command line $ syft launch --name=my-domain --port=8080 --reset=True Starting
 syft-node server on 0.0.0.0:8080 ``` ## Launch Client ```python import syft as
-sy sy.requires(">=0.8.5,<0.8.6") domain_client = sy.login(port=8080,
+sy sy.requires(">=0.8.6,<0.8.7") domain_client = sy.login(port=8080,
 email="info@openmined.org", password="changethis") ``` ## PySyft in 10 minutes
 ð _A_P_I_ _E_x_a_m_p_l_e_ _N_o_t_e_b_o_o_k_s - _0_0_-_l_o_a_d_-_d_a_t_a_._i_p_y_n_b - _0_1_-_s_u_b_m_i_t_-_c_o_d_e_._i_p_y_n_b - _0_2_-
 _r_e_v_i_e_w_-_c_o_d_e_-_a_n_d_-_a_p_p_r_o_v_e_._i_p_y_n_b - _0_3_-_d_a_t_a_-_s_c_i_e_n_t_i_s_t_-_d_o_w_n_l_o_a_d_-_r_e_s_u_l_t_._i_p_y_n_b - _0_4_-
 _j_a_x_-_e_x_a_m_p_l_e_._i_p_y_n_b - _0_5_-_c_u_s_t_o_m_-_p_o_l_i_c_y_._i_p_y_n_b - _0_6_-_m_u_l_t_i_p_l_e_-_c_o_d_e_-_r_e_q_u_e_s_t_s_._i_p_y_n_b -
 _0_7_-_d_o_m_a_i_n_-_r_e_g_i_s_t_e_r_-_c_o_n_t_r_o_l_-_f_l_o_w_._i_p_y_n_b - _0_8_-_c_o_d_e_-_v_e_r_s_i_o_n_._i_p_y_n_b - _0_9_-_b_l_o_b_-
 _s_t_o_r_a_g_e_._i_p_y_n_b - _1_0_-_c_o_n_t_a_i_n_e_r_-_i_m_a_g_e_s_._i_p_y_n_b - _1_1_-_c_o_n_t_a_i_n_e_r_-_i_m_a_g_e_s_-_k_8_s_._i_p_y_n_b ##
 Deploy Kubernetes Helm Chart **Note**: Assuming we have a Kubernetes cluster
@@ -41,44 +41,45 @@
 `PyGrid` = our ð³ `docker` / ð§ `vm` `Domain` & `Gateway` Servers where
 `private data` lives ## Docs and Support - ð _D_o_c_s - `#support` on _S_l_a_c_k #
 Install Notes - HAGrid 0.3 Requires: ð `python` ð `git` - Run: `pip
 install -U hagrid` - Interactive Install ð§ð½ââï¸ WizardBETA Requires
 ðµ `hagrid`: - Run: `hagrid quickstart` - PySyft 0.8.1 Requires: ð `python
 3.10 - 3.12` - Run: `pip install -U syft` - PyGrid Requires: ð³ `docker`,
 ð¦¦ `podman` or â¸ï¸ `kubernetes` - Run: `hagrid launch ...` # Versions
-`0.9.0` - Coming soon... `0.8.6` (Beta) - `dev` branch ðð½ _A_P_I - Coming
-soon... `0.8.5` (Stable) - _A_P_I Deprecated: - `0.8.4` - _A_P_I - `0.8.3` - _A_P_I -
-`0.8.2` - _A_P_I - `0.8.1` - _A_P_I - `0.8.0` - _A_P_I - `0.7.0` - _C_o_u_r_s_e_ _3_ _U_p_d_a_t_e_d -
-`0.6.0` - _C_o_u_r_s_e_ _3 - `0.5.1` - _C_o_u_r_s_e_ _2 + M1 Hotfix - `0.2.0` - `0.5.0` PySyft
-and PyGrid use the same `version` and its best to match them up where possible.
-We release weekly betas which can be used in each context: PySyft (Stable):
-`pip install -U syft` PyGrid (Stable) `hagrid launch ... tag=latest` PySyft
-(Beta): `pip install -U syft --pre` PyGrid (Beta): `hagrid launch ... tag=beta`
-HAGrid is a cli / deployment tool so the latest version of `hagrid` is usually
-the best. # What is Syft? [Syft]`Syft` is OpenMined's `open source` stack that
-provides `secure` and `private` Data Science in Python. Syft decouples `private
-data` from model training, using techniques like [Federated Learning](https://
-ai.googleblog.com/2017/04/federated-learning-collaborative.html), [Differential
-Privacy](https://en.wikipedia.org/wiki/Differential_privacy), and [Encrypted
-Computation](https://en.wikipedia.org/wiki/Homomorphic_encryption). This is
-done with a `numpy`-like interface and integration with `Deep Learning`
-frameworks, so that you as a `Data Scientist` can maintain your current
-workflow while using these new `privacy-enhancing techniques`. ### Why should I
-use Syft? `Syft` allows a `Data Scientist` to ask `questions` about a `dataset`
-and, within `privacy limits` set by the `data owner`, get `answers` to those
-`questions`, all without obtaining a `copy` of the data itself. We call this
-process `Remote Data Science`. It means in a wide variety of `domains` across
-society, the current `risks` of sharing information (`copying` data) with
-someone such as, privacy invasion, IP theft and blackmail will no longer
-prevent the vast `benefits` such as innovation, insights and scientific
-discovery which secure access will provide. No more cold calls to get `access`
-to a dataset. No more weeks of `wait times` to get a `result` on your `query`.
-It also means `1000x more data` in every domain. PySyft opens the doors to a
-streamlined Data Scientist `workflow`, all with the individual's `privacy` at
-its heart. # Terminology
+`0.9.0` - Coming soon... `0.8.7` (Beta) - `dev` branch ðð½ _A_P_I - Coming
+soon... `0.8.6` (Stable) - _A_P_I Deprecated: - `0.8.5-post.2` - _A_P_I - `0.8.4` -
+_A_P_I - `0.8.3` - _A_P_I - `0.8.2` - _A_P_I - `0.8.1` - _A_P_I - `0.8.0` - _A_P_I - `0.7.0` -
+_C_o_u_r_s_e_ _3_ _U_p_d_a_t_e_d - `0.6.0` - _C_o_u_r_s_e_ _3 - `0.5.1` - _C_o_u_r_s_e_ _2 + M1 Hotfix -
+`0.2.0` - `0.5.0` PySyft and PyGrid use the same `version` and its best to
+match them up where possible. We release weekly betas which can be used in each
+context: PySyft (Stable): `pip install -U syft` PyGrid (Stable) `hagrid launch
+... tag=latest` PySyft (Beta): `pip install -U syft --pre` PyGrid (Beta):
+`hagrid launch ... tag=beta` HAGrid is a cli / deployment tool so the latest
+version of `hagrid` is usually the best. # What is Syft? [Syft]`Syft` is
+OpenMined's `open source` stack that provides `secure` and `private` Data
+Science in Python. Syft decouples `private data` from model training, using
+techniques like [Federated Learning](https://ai.googleblog.com/2017/04/
+federated-learning-collaborative.html), [Differential Privacy](https://
+en.wikipedia.org/wiki/Differential_privacy), and [Encrypted Computation](https:
+//en.wikipedia.org/wiki/Homomorphic_encryption). This is done with a `numpy`-
+like interface and integration with `Deep Learning` frameworks, so that you as
+a `Data Scientist` can maintain your current workflow while using these new
+`privacy-enhancing techniques`. ### Why should I use Syft? `Syft` allows a
+`Data Scientist` to ask `questions` about a `dataset` and, within `privacy
+limits` set by the `data owner`, get `answers` to those `questions`, all
+without obtaining a `copy` of the data itself. We call this process `Remote
+Data Science`. It means in a wide variety of `domains` across society, the
+current `risks` of sharing information (`copying` data) with someone such as,
+privacy invasion, IP theft and blackmail will no longer prevent the vast
+`benefits` such as innovation, insights and scientific discovery which secure
+access will provide. No more cold calls to get `access` to a dataset. No more
+weeks of `wait times` to get a `result` on your `query`. It also means `1000x
+more data` in every domain. PySyft opens the doors to a streamlined Data
+Scientist `workflow`, all with the individual's `privacy` at its heart. #
+Terminology
  _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ 
 |                  [[IImmaaggee]]             |                 [[IImmaaggee]]              |
 |_ _ _ _ _ _ _ _ _?ð_?_?_?¨_?ð_?_?_?»_?â_?_?_?ð_?_?_?¼_ _DD_aa_tt_aa_ _OO_ww_nn_ee_rr_ss_ _ _ _|_ _ _ _ _ _?ð_?_?_?©_?ð_?_?_?½_?â_?_?_?ð_?_?_?¬_ _DD_aa_tt_aa_ _SS_cc_ii_ee_nn_tt_ii_ss_tt_ss_ _ |
 |Provide `datasets` which they would   |Are end `users` who desire to perform |
 |like to make available for `study` by |`computations` or `answer` a specific |
 |an `outside party` they may or may not|`question` using one or more data     |
 |_`_f_u_l_l_y_ _t_r_u_s_t_`_ _h_a_s_ _g_o_o_d_ _i_n_t_e_n_t_i_o_n_s_._ _ _ _ _|_o_w_n_e_r_s_'_ _`_d_a_t_a_s_e_t_s_`_._ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ |
@@ -111,15 +112,15 @@
 |_[[_II_mm_aa_gg_ee_]]_|_[[_II_mm_aa_gg_ee_]]_|_[[_II_mm_aa_gg_ee_]]|
 # Contributors OpenMined and Syft appreciates all contributors, if you would
 like to fix a bug or suggest a new feature, please see our [guidelines](https:/
 /openmined.github.io/PySyft/developer_guide/index.html).
 [Contributors]# Supporters
         _[[_hh_tt_tt_pp_ss_::_//_//                  _[[_hh_tt_tt_pp_ss_::_//_//                  _[[_hh_tt_tt_pp_ss_::_//_//                  _[[_hh_tt_tt_pp_ss_::_//_//                  _[[_hh_tt_tt_pp_ss_::_//_//                  _[[_hh_tt_tt_pp_ss_::_//_//                  _[[_hh_tt_tt_pp_ss_::_//_//                  _[[_hh_tt_tt_pp_ss_::_//_//                  _[[_hh_tt_tt_pp_ss_::_//_//                  _[[_hh_tt_tt_pp_ss_::_//_//                  _[[_hh_tt_tt_pp_ss_::_//_//
 _rr_aa_ww_.._gg_ii_tt_hh_uu_bb_uu_ss_ee_rr_cc_oo_nn_tt_ee_nn_tt_.._cc_oo_mm_// _rr_aa_ww_.._gg_ii_tt_hh_uu_bb_uu_ss_ee_rr_cc_oo_nn_tt_ee_nn_tt_.._cc_oo_mm_// _rr_aa_ww_.._gg_ii_tt_hh_uu_bb_uu_ss_ee_rr_cc_oo_nn_tt_ee_nn_tt_.._cc_oo_mm_// _rr_aa_ww_.._gg_ii_tt_hh_uu_bb_uu_ss_ee_rr_cc_oo_nn_tt_ee_nn_tt_.._cc_oo_mm_// _rr_aa_ww_.._gg_ii_tt_hh_uu_bb_uu_ss_ee_rr_cc_oo_nn_tt_ee_nn_tt_.._cc_oo_mm_// _rr_aa_ww_.._gg_ii_tt_hh_uu_bb_uu_ss_ee_rr_cc_oo_nn_tt_ee_nn_tt_.._cc_oo_mm_// _rr_aa_ww_.._gg_ii_tt_hh_uu_bb_uu_ss_ee_rr_cc_oo_nn_tt_ee_nn_tt_.._cc_oo_mm_// _rr_aa_ww_.._gg_ii_tt_hh_uu_bb_uu_ss_ee_rr_cc_oo_nn_tt_ee_nn_tt_.._cc_oo_mm_// _rr_aa_ww_.._gg_ii_tt_hh_uu_bb_uu_ss_ee_rr_cc_oo_nn_tt_ee_nn_tt_.._cc_oo_mm_// _rr_aa_ww_.._gg_ii_tt_hh_uu_bb_uu_ss_ee_rr_cc_oo_nn_tt_ee_nn_tt_.._cc_oo_mm_// _rr_aa_ww_.._gg_ii_tt_hh_uu_bb_uu_ss_ee_rr_cc_oo_nn_tt_ee_nn_tt_.._cc_oo_mm_//
- _OO_pp_ee_nn_MM_ii_nn_ee_dd_//_PP_yy_SS_yy_ff_tt_//_00_.._88_.._66_//    _OO_pp_ee_nn_MM_ii_nn_ee_dd_//_PP_yy_SS_yy_ff_tt_//_00_.._88_.._66_//    _OO_pp_ee_nn_MM_ii_nn_ee_dd_//_PP_yy_SS_yy_ff_tt_//_00_.._88_.._66_//    _OO_pp_ee_nn_MM_ii_nn_ee_dd_//_PP_yy_SS_yy_ff_tt_//_00_.._88_.._66_//    _OO_pp_ee_nn_MM_ii_nn_ee_dd_//_PP_yy_SS_yy_ff_tt_//_00_.._88_.._66_//    _OO_pp_ee_nn_MM_ii_nn_ee_dd_//_PP_yy_SS_yy_ff_tt_//_00_.._88_.._66_//    _OO_pp_ee_nn_MM_ii_nn_ee_dd_//_PP_yy_SS_yy_ff_tt_//_00_.._88_.._66_//    _OO_pp_ee_nn_MM_ii_nn_ee_dd_//_PP_yy_SS_yy_ff_tt_//_00_.._88_.._66_//    _OO_pp_ee_nn_MM_ii_nn_ee_dd_//_PP_yy_SS_yy_ff_tt_//_00_.._88_.._66_//    _OO_pp_ee_nn_MM_ii_nn_ee_dd_//_PP_yy_SS_yy_ff_tt_//_00_.._88_.._66_//    _OO_pp_ee_nn_MM_ii_nn_ee_dd_//_PP_yy_SS_yy_ff_tt_//_00_.._88_.._66_//
+ _OO_pp_ee_nn_MM_ii_nn_ee_dd_//_PP_yy_SS_yy_ff_tt_//_00_.._88_.._77_//    _OO_pp_ee_nn_MM_ii_nn_ee_dd_//_PP_yy_SS_yy_ff_tt_//_00_.._88_.._77_//    _OO_pp_ee_nn_MM_ii_nn_ee_dd_//_PP_yy_SS_yy_ff_tt_//_00_.._88_.._77_//    _OO_pp_ee_nn_MM_ii_nn_ee_dd_//_PP_yy_SS_yy_ff_tt_//_00_.._88_.._77_//    _OO_pp_ee_nn_MM_ii_nn_ee_dd_//_PP_yy_SS_yy_ff_tt_//_00_.._88_.._77_//    _OO_pp_ee_nn_MM_ii_nn_ee_dd_//_PP_yy_SS_yy_ff_tt_//_00_.._88_.._77_//    _OO_pp_ee_nn_MM_ii_nn_ee_dd_//_PP_yy_SS_yy_ff_tt_//_00_.._88_.._77_//    _OO_pp_ee_nn_MM_ii_nn_ee_dd_//_PP_yy_SS_yy_ff_tt_//_00_.._88_.._77_//    _OO_pp_ee_nn_MM_ii_nn_ee_dd_//_PP_yy_SS_yy_ff_tt_//_00_.._88_.._77_//    _OO_pp_ee_nn_MM_ii_nn_ee_dd_//_PP_yy_SS_yy_ff_tt_//_00_.._88_.._77_//    _OO_pp_ee_nn_MM_ii_nn_ee_dd_//_PP_yy_SS_yy_ff_tt_//_00_.._88_.._77_//
  _dd_oo_cc_ss_//_ii_mm_gg_//_ll_oo_gg_oo____ss_ll_oo_aa_nn_.._pp_nn_gg_]]   _dd_oo_cc_ss_//_ii_mm_gg_//_ll_oo_gg_oo____mm_ee_tt_aa_.._pp_nn_gg_]]    _dd_oo_cc_ss_//_ii_mm_gg_//_ll_oo_gg_oo____tt_oo_rr_cc_hh_.._pp_nn_gg_]]          _dd_oo_cc_ss_//_ii_mm_gg_//          _dd_oo_cc_ss_//_ii_mm_gg_//_ll_oo_gg_oo____tt_ww_ii_tt_tt_ee_rr_.._pp_nn_gg_]] _dd_oo_cc_ss_//_ii_mm_gg_//_ll_oo_gg_oo____gg_oo_oo_gg_ll_ee_.._pp_nn_gg_]]          _dd_oo_cc_ss_//_ii_mm_gg_//            _dd_oo_cc_ss_//_ii_mm_gg_//_ll_oo_gg_oo____oo_nn_.._pp_nn_gg_]]    _dd_oo_cc_ss_//_ii_mm_gg_//_ll_oo_gg_oo____uu_dd_aa_cc_ii_tt_yy_.._pp_nn_gg_]]         _dd_oo_cc_ss_//_ii_mm_gg_//                  _dd_oo_cc_ss_//_ii_mm_gg_//
                                                                                      _ll_oo_gg_oo____nn_zz____ll_ii_gg_hh_tt_.._pp_nn_gg_]]                                                              _ll_oo_gg_oo____mm_ii_cc_rr_oo_ss_oo_ff_tt_.._pp_nn_gg_]]                                                              _ll_oo_gg_oo____cc_dd_hh_ii____ll_ii_gg_hh_tt_.._pp_nn_gg_]]      _ll_oo_gg_oo____aa_rr_kk_hh_nn____ll_ii_gg_hh_tt_.._pp_nn_gg_]]
 # Open Collective `OpenMined` is a fiscally sponsored `501(c)(3)` in the USA.
 We are funded by our generous supporters on _O_p_e_n_ _C_o_l_l_e_c_t_i_v_e.
 
 [Contributors]# Disclaimer Syft is under active development and is not yet
 ready for pilots on private data without our assistance. As early access
```

### Comparing `syft-0.8.6b1/README.md` & `syft-0.8.7b1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -19,30 +19,30 @@
 ```
 
 ## Launch Server
 
 ```python
 # from Jupyter / Python
 import syft as sy
-sy.requires(">=0.8.5,<0.8.6")
+sy.requires(">=0.8.6,<0.8.7")
 node = sy.orchestra.launch(name="my-domain", port=8080, dev_mode=True, reset=True)
 ```
 
 ```bash
 # or from the command line
 $ syft launch --name=my-domain --port=8080 --reset=True
 
 Starting syft-node server on 0.0.0.0:8080
 ```
 
 ## Launch Client
 
 ```python
 import syft as sy
-sy.requires(">=0.8.5,<0.8.6")
+sy.requires(">=0.8.6,<0.8.7")
 domain_client = sy.login(port=8080, email="info@openmined.org", password="changethis")
 ```
 
 ## PySyft in 10 minutes
 
 📝 <a href="notebooks/api">API Example Notebooks</a>
 
@@ -132,19 +132,20 @@
 - Interactive Install 🧙🏽‍♂️ Wizard<sup>BETA</sup> Requires 🛵 `hagrid`: - Run: `hagrid quickstart`
 - PySyft 0.8.1 Requires: 🐍 `python 3.10 - 3.12` - Run: `pip install -U syft`
 - PyGrid Requires: 🐳 `docker`, 🦦 `podman` or ☸️ `kubernetes` - Run: `hagrid launch ...`
 
 # Versions
 
 `0.9.0` - Coming soon...  
-`0.8.6` (Beta) - `dev` branch 👈🏽 <a href="https://github.com/OpenMined/PySyft/tree/dev/notebooks/api/0.8">API</a> - Coming soon...  
-`0.8.5` (Stable) - <a href="https://github.com/OpenMined/PySyft/tree/0.8.5/notebooks/api/0.8">API</a>
+`0.8.7` (Beta) - `dev` branch 👈🏽 <a href="https://github.com/OpenMined/PySyft/tree/dev/notebooks/api/0.8">API</a> - Coming soon...  
+`0.8.6` (Stable) - <a href="https://github.com/OpenMined/PySyft/tree/0.8.6/notebooks/api/0.8">API</a>
 
 Deprecated:
 
+- `0.8.5-post.2` - <a href="https://github.com/OpenMined/PySyft/tree/0.8.5-post.2/notebooks/api/0.8">API</a>
 - `0.8.4` - <a href="https://github.com/OpenMined/PySyft/tree/0.8.4/notebooks/api/0.8">API</a>
 - `0.8.3` - <a href="https://github.com/OpenMined/PySyft/tree/0.8.3/notebooks/api/0.8">API</a>
 - `0.8.2` - <a href="https://github.com/OpenMined/PySyft/tree/0.8.2/notebooks/api/0.8">API</a>
 - `0.8.1` - <a href="https://github.com/OpenMined/PySyft/tree/0.8.1/notebooks/api/0.8">API</a>
 - `0.8.0` - <a href="https://github.com/OpenMined/PySyft/tree/0.8/notebooks/api/0.8">API</a>
 - `0.7.0` - <a href="https://github.com/OpenMined/courses/tree/introduction-to-remote-data-science-dev">Course 3 Updated</a>
 - `0.6.0` - <a href="https://github.com/OpenMined/courses/tree/introduction-to-remote-data-science">Course 3</a>
```

#### html2text {}

```diff
@@ -4,19 +4,19 @@
 _b_a_d_g_e_._s_v_g_?_b_r_a_n_c_h_=_d_e_v_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_c_h_a_t_-_o_n_%_2_0_s_l_a_c_k_-
 _p_u_r_p_l_e_?_l_o_g_o_=_s_l_a_c_k_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_r_e_a_d_-_d_o_c_s_-_y_e_l_l_o_w_?_l_o_g_o_=_m_d_b_o_o_k_]
 
 [Syft Logo]Perform data science on `data` that remains in `someone else's`
 server # Quickstart â `Linux` â `macOS` â `Windows` â `Docker` â
 `Podman` â `Kubernetes` ## Install Client ```bash $ pip install -U syft
 [data_science] ``` ## Launch Server ```python # from Jupyter / Python import
-syft as sy sy.requires(">=0.8.5,<0.8.6") node = sy.orchestra.launch(name="my-
+syft as sy sy.requires(">=0.8.6,<0.8.7") node = sy.orchestra.launch(name="my-
 domain", port=8080, dev_mode=True, reset=True) ``` ```bash # or from the
 command line $ syft launch --name=my-domain --port=8080 --reset=True Starting
 syft-node server on 0.0.0.0:8080 ``` ## Launch Client ```python import syft as
-sy sy.requires(">=0.8.5,<0.8.6") domain_client = sy.login(port=8080,
+sy sy.requires(">=0.8.6,<0.8.7") domain_client = sy.login(port=8080,
 email="info@openmined.org", password="changethis") ``` ## PySyft in 10 minutes
 ð _A_P_I_ _E_x_a_m_p_l_e_ _N_o_t_e_b_o_o_k_s - _0_0_-_l_o_a_d_-_d_a_t_a_._i_p_y_n_b - _0_1_-_s_u_b_m_i_t_-_c_o_d_e_._i_p_y_n_b - _0_2_-
 _r_e_v_i_e_w_-_c_o_d_e_-_a_n_d_-_a_p_p_r_o_v_e_._i_p_y_n_b - _0_3_-_d_a_t_a_-_s_c_i_e_n_t_i_s_t_-_d_o_w_n_l_o_a_d_-_r_e_s_u_l_t_._i_p_y_n_b - _0_4_-
 _j_a_x_-_e_x_a_m_p_l_e_._i_p_y_n_b - _0_5_-_c_u_s_t_o_m_-_p_o_l_i_c_y_._i_p_y_n_b - _0_6_-_m_u_l_t_i_p_l_e_-_c_o_d_e_-_r_e_q_u_e_s_t_s_._i_p_y_n_b -
 _0_7_-_d_o_m_a_i_n_-_r_e_g_i_s_t_e_r_-_c_o_n_t_r_o_l_-_f_l_o_w_._i_p_y_n_b - _0_8_-_c_o_d_e_-_v_e_r_s_i_o_n_._i_p_y_n_b - _0_9_-_b_l_o_b_-
 _s_t_o_r_a_g_e_._i_p_y_n_b - _1_0_-_c_o_n_t_a_i_n_e_r_-_i_m_a_g_e_s_._i_p_y_n_b - _1_1_-_c_o_n_t_a_i_n_e_r_-_i_m_a_g_e_s_-_k_8_s_._i_p_y_n_b ##
 Deploy Kubernetes Helm Chart **Note**: Assuming we have a Kubernetes cluster
@@ -41,44 +41,45 @@
 `PyGrid` = our ð³ `docker` / ð§ `vm` `Domain` & `Gateway` Servers where
 `private data` lives ## Docs and Support - ð _D_o_c_s - `#support` on _S_l_a_c_k #
 Install Notes - HAGrid 0.3 Requires: ð `python` ð `git` - Run: `pip
 install -U hagrid` - Interactive Install ð§ð½ââï¸ WizardBETA Requires
 ðµ `hagrid`: - Run: `hagrid quickstart` - PySyft 0.8.1 Requires: ð `python
 3.10 - 3.12` - Run: `pip install -U syft` - PyGrid Requires: ð³ `docker`,
 ð¦¦ `podman` or â¸ï¸ `kubernetes` - Run: `hagrid launch ...` # Versions
-`0.9.0` - Coming soon... `0.8.6` (Beta) - `dev` branch ðð½ _A_P_I - Coming
-soon... `0.8.5` (Stable) - _A_P_I Deprecated: - `0.8.4` - _A_P_I - `0.8.3` - _A_P_I -
-`0.8.2` - _A_P_I - `0.8.1` - _A_P_I - `0.8.0` - _A_P_I - `0.7.0` - _C_o_u_r_s_e_ _3_ _U_p_d_a_t_e_d -
-`0.6.0` - _C_o_u_r_s_e_ _3 - `0.5.1` - _C_o_u_r_s_e_ _2 + M1 Hotfix - `0.2.0` - `0.5.0` PySyft
-and PyGrid use the same `version` and its best to match them up where possible.
-We release weekly betas which can be used in each context: PySyft (Stable):
-`pip install -U syft` PyGrid (Stable) `hagrid launch ... tag=latest` PySyft
-(Beta): `pip install -U syft --pre` PyGrid (Beta): `hagrid launch ... tag=beta`
-HAGrid is a cli / deployment tool so the latest version of `hagrid` is usually
-the best. # What is Syft? [Syft]`Syft` is OpenMined's `open source` stack that
-provides `secure` and `private` Data Science in Python. Syft decouples `private
-data` from model training, using techniques like [Federated Learning](https://
-ai.googleblog.com/2017/04/federated-learning-collaborative.html), [Differential
-Privacy](https://en.wikipedia.org/wiki/Differential_privacy), and [Encrypted
-Computation](https://en.wikipedia.org/wiki/Homomorphic_encryption). This is
-done with a `numpy`-like interface and integration with `Deep Learning`
-frameworks, so that you as a `Data Scientist` can maintain your current
-workflow while using these new `privacy-enhancing techniques`. ### Why should I
-use Syft? `Syft` allows a `Data Scientist` to ask `questions` about a `dataset`
-and, within `privacy limits` set by the `data owner`, get `answers` to those
-`questions`, all without obtaining a `copy` of the data itself. We call this
-process `Remote Data Science`. It means in a wide variety of `domains` across
-society, the current `risks` of sharing information (`copying` data) with
-someone such as, privacy invasion, IP theft and blackmail will no longer
-prevent the vast `benefits` such as innovation, insights and scientific
-discovery which secure access will provide. No more cold calls to get `access`
-to a dataset. No more weeks of `wait times` to get a `result` on your `query`.
-It also means `1000x more data` in every domain. PySyft opens the doors to a
-streamlined Data Scientist `workflow`, all with the individual's `privacy` at
-its heart. # Terminology
+`0.9.0` - Coming soon... `0.8.7` (Beta) - `dev` branch ðð½ _A_P_I - Coming
+soon... `0.8.6` (Stable) - _A_P_I Deprecated: - `0.8.5-post.2` - _A_P_I - `0.8.4` -
+_A_P_I - `0.8.3` - _A_P_I - `0.8.2` - _A_P_I - `0.8.1` - _A_P_I - `0.8.0` - _A_P_I - `0.7.0` -
+_C_o_u_r_s_e_ _3_ _U_p_d_a_t_e_d - `0.6.0` - _C_o_u_r_s_e_ _3 - `0.5.1` - _C_o_u_r_s_e_ _2 + M1 Hotfix -
+`0.2.0` - `0.5.0` PySyft and PyGrid use the same `version` and its best to
+match them up where possible. We release weekly betas which can be used in each
+context: PySyft (Stable): `pip install -U syft` PyGrid (Stable) `hagrid launch
+... tag=latest` PySyft (Beta): `pip install -U syft --pre` PyGrid (Beta):
+`hagrid launch ... tag=beta` HAGrid is a cli / deployment tool so the latest
+version of `hagrid` is usually the best. # What is Syft? [Syft]`Syft` is
+OpenMined's `open source` stack that provides `secure` and `private` Data
+Science in Python. Syft decouples `private data` from model training, using
+techniques like [Federated Learning](https://ai.googleblog.com/2017/04/
+federated-learning-collaborative.html), [Differential Privacy](https://
+en.wikipedia.org/wiki/Differential_privacy), and [Encrypted Computation](https:
+//en.wikipedia.org/wiki/Homomorphic_encryption). This is done with a `numpy`-
+like interface and integration with `Deep Learning` frameworks, so that you as
+a `Data Scientist` can maintain your current workflow while using these new
+`privacy-enhancing techniques`. ### Why should I use Syft? `Syft` allows a
+`Data Scientist` to ask `questions` about a `dataset` and, within `privacy
+limits` set by the `data owner`, get `answers` to those `questions`, all
+without obtaining a `copy` of the data itself. We call this process `Remote
+Data Science`. It means in a wide variety of `domains` across society, the
+current `risks` of sharing information (`copying` data) with someone such as,
+privacy invasion, IP theft and blackmail will no longer prevent the vast
+`benefits` such as innovation, insights and scientific discovery which secure
+access will provide. No more cold calls to get `access` to a dataset. No more
+weeks of `wait times` to get a `result` on your `query`. It also means `1000x
+more data` in every domain. PySyft opens the doors to a streamlined Data
+Scientist `workflow`, all with the individual's `privacy` at its heart. #
+Terminology
  _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ 
 |                  [[IImmaaggee]]             |                 [[IImmaaggee]]              |
 |_ _ _ _ _ _ _ _ _?ð_?_?_?¨_?ð_?_?_?»_?â_?_?_?ð_?_?_?¼_ _DD_aa_tt_aa_ _OO_ww_nn_ee_rr_ss_ _ _ _|_ _ _ _ _ _?ð_?_?_?©_?ð_?_?_?½_?â_?_?_?ð_?_?_?¬_ _DD_aa_tt_aa_ _SS_cc_ii_ee_nn_tt_ii_ss_tt_ss_ _ |
 |Provide `datasets` which they would   |Are end `users` who desire to perform |
 |like to make available for `study` by |`computations` or `answer` a specific |
 |an `outside party` they may or may not|`question` using one or more data     |
 |_`_f_u_l_l_y_ _t_r_u_s_t_`_ _h_a_s_ _g_o_o_d_ _i_n_t_e_n_t_i_o_n_s_._ _ _ _ _|_o_w_n_e_r_s_'_ _`_d_a_t_a_s_e_t_s_`_._ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ |
```

### Comparing `syft-0.8.6b1/setup.cfg` & `syft-0.8.7b1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = syft
-version = attr: "0.8.6-beta.1"
+version = attr: "0.8.7-beta.1"
 description = Perform numpy-like analysis on data that remains in someone elses server
 author = OpenMined
 author_email = info@openmined.org
 license = Apache-2.0
 long_description = file: PYPI.md
 long_description_content_type = text/markdown; charset=UTF-8; variant=GFM
 url = https://openmined.github.io/PySyft/
@@ -57,14 +57,15 @@
 	numpy>=1.23.5,<=1.24.4; python_version<"3.12"
 	numpy>=1.26.4,<1.27; python_version>="3.12"
 	pandas==2.2.1
 	docker==6.1.3
 	kr8s==0.13.5
 	PyYAML==6.0.1
 	azure-storage-blob==12.19.1
+	ipywidgets==8.1.2
 install_requires = 
 	%(syft)s
 python_requires = >=3.10
 
 [options.packages.find]
 where = src
 exclude =
```

### Comparing `syft-0.8.6b1/src/syft/VERSION` & `syft-0.8.7b1/src/syft/VERSION`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Mono Repo Global Version
-__version__ = "0.8.6-beta.1"
+__version__ = "0.8.7-beta.1"
 # elsewhere we can call this file: `python VERSION` and simply take the stdout
 
 # stdlib
 import os
 import subprocess
 import sys
```

### Comparing `syft-0.8.6b1/src/syft/__init__.py` & `syft-0.8.7b1/src/syft/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.8.6-beta.1"
+__version__ = "0.8.7-beta.1"
 
 # stdlib
 from collections.abc import Callable
 import pathlib
 from pathlib import Path
 import sys
 from typing import Any
@@ -22,16 +22,14 @@
 from .client.registry import EnclaveRegistry  # noqa: F401
 from .client.registry import NetworkRegistry  # noqa: F401
 from .client.search import Search  # noqa: F401
 from .client.search import SearchResults  # noqa: F401
 from .client.user_settings import UserSettings  # noqa: F401
 from .client.user_settings import settings  # noqa: F401
 from .custom_worker.config import DockerWorkerConfig  # noqa: F401
-from .external import OBLV_ENABLED  # noqa: F401
-from .external import enable_external_lib  # noqa: F401
 from .node.credentials import SyftSigningKey  # noqa: F401
 from .node.domain import Domain  # noqa: F401
 from .node.enclave import Enclave  # noqa: F401
 from .node.gateway import Gateway  # noqa: F401
 from .node.server import serve_node  # noqa: F401
 from .node.server import serve_node as bind_worker  # noqa: F401
 from .node.worker import Worker  # noqa: F401
@@ -43,14 +41,18 @@
 from .serde.deserialize import _deserialize as deserialize  # noqa: F401
 from .serde.serializable import serializable  # noqa: F401
 from .serde.serialize import _serialize as serialize  # noqa: F401
 from .service.action.action_data_empty import ActionDataEmpty  # noqa: F401
 from .service.action.action_object import ActionObject  # noqa: F401
 from .service.action.plan import Plan  # noqa: F401
 from .service.action.plan import planify  # noqa: F401
+from .service.api.api import api_endpoint  # noqa: F401
+from .service.api.api import create_new_api_endpoint as TwinAPIEndpoint  # noqa: F401
+from .service.api.api import mock_api_endpoint  # noqa: F401
+from .service.api.api import private_api_endpoint  # noqa: F401
 from .service.code.user_code import UserCodeStatus  # noqa: F401; noqa: F401
 from .service.code.user_code import syft_function  # noqa: F401; noqa: F401
 from .service.code.user_code import syft_function_single_use  # noqa: F401; noqa: F401
 from .service.data_subject import DataSubjectCreate as DataSubject  # noqa: F401
 from .service.dataset.dataset import Contributor  # noqa: F401
 from .service.dataset.dataset import CreateAsset as Asset  # noqa: F401
 from .service.dataset.dataset import CreateDataset as Dataset  # noqa: F401
@@ -103,18 +105,14 @@
     #         "\nWarning: syft is imported in light mode by default. \
     #     \nTo switch to dark mode, please run `sy.options.color_theme = 'dark'`"
     #     )
     # )
 except:  # noqa: E722
     pass  # nosec
 
-# For server-side, to enable by environment variable
-if OBLV_ENABLED:
-    enable_external_lib("oblv")
-
 
 def module_property(func: Any) -> Callable:
     """Decorator to turn module functions into properties.
     Function names must be prefixed with an underscore."""
     module = sys.modules[func.__module__]
 
     def base_getattr(name: str) -> None:
```

### Comparing `syft-0.8.6b1/src/syft/abstract_node.py` & `syft-0.8.7b1/src/syft/abstract_node.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6b1/src/syft/client/api.py` & `syft-0.8.7b1/src/syft/client/api.py`

 * *Files 9% similar despite different names*

```diff
@@ -51,14 +51,15 @@
 from ..types.syft_object import SYFT_OBJECT_VERSION_2
 from ..types.syft_object import SyftBaseObject
 from ..types.syft_object import SyftMigrationRegistry
 from ..types.syft_object import SyftObject
 from ..types.uid import LineageID
 from ..types.uid import UID
 from ..util.autoreload import autoreload_enabled
+from ..util.markdown import as_markdown_python_code
 from ..util.telemetry import instrument
 from ..util.util import prompt_warning_message
 from .connection import NodeConnection
 
 if TYPE_CHECKING:
     # relative
     from ..node import Node
@@ -227,14 +228,15 @@
     node_uid: UID
     signature: Signature
     path: str
     make_call: Callable
     pre_kwargs: dict[str, Any] | None = None
     communication_protocol: PROTOCOL_TYPE
     warning: APIEndpointWarning | None = None
+    custom_function: bool = False
 
     @property
     def __ipython_inspector_signature_override__(self) -> Signature | None:
         return self.signature
 
     def prepare_args_and_kwargs(
         self, args: list | tuple, kwargs: dict[str, Any]
@@ -247,15 +249,17 @@
 
         args, kwargs = migrate_args_and_kwargs(
             to_protocol=self.communication_protocol, args=args, kwargs=kwargs
         )
 
         return args, kwargs
 
-    def __call__(self, *args: Any, **kwargs: Any) -> Any:
+    def __function_call(
+        self, path: str, *args: Any, cache_result: bool = True, **kwargs: Any
+    ) -> Any:
         if "blocking" in self.signature.parameters:
             raise Exception(
                 f"Signature {self.signature} can't have 'blocking' kwarg because it's reserved"
             )
 
         blocking = True
         if "blocking" in kwargs:
@@ -270,31 +274,97 @@
         if self.pre_kwargs:
             _valid_kwargs.update(self.pre_kwargs)
 
         _valid_kwargs["communication_protocol"] = self.communication_protocol
 
         api_call = SyftAPICall(
             node_uid=self.node_uid,
-            path=self.path,
+            path=path,
             args=list(_valid_args),
             kwargs=_valid_kwargs,
             blocking=blocking,
         )
 
         allowed = self.warning.show() if self.warning else True
         if not allowed:
             return
-        result = self.make_call(api_call=api_call)
+        result = self.make_call(api_call=api_call, cache_result=cache_result)
 
         result, _ = migrate_args_and_kwargs(
             [result], kwargs={}, to_latest_protocol=True
         )
         result = result[0]
         return result
 
+    def __call__(self, *args: Any, **kwargs: Any) -> Any:
+        return self.__function_call(self.path, *args, **kwargs)
+
+    def mock(self, *args: Any, **kwargs: Any) -> Any:
+        if self.custom_function:
+            return self.__function_call("api.call_public", *args, **kwargs)
+        return SyftError(
+            message="This function doesn't support public/private calls as it's not custom."
+        )
+
+    def private(self, *args: Any, **kwargs: Any) -> Any:
+        if self.custom_function:
+            return self.__function_call("api.call_private", *args, **kwargs)
+        return SyftError(
+            message="This function doesn't support public/private calls as it's not custom."
+        )
+
+    def custom_function_id(self) -> UID | SyftError:
+        if self.custom_function and self.pre_kwargs is not None:
+            custom_path = self.pre_kwargs.get("path", "")
+            api_call = SyftAPICall(
+                node_uid=self.node_uid,
+                path="api.view",
+                args=[custom_path],
+                kwargs={},
+            )
+            endpoint = self.make_call(api_call=api_call)
+            if isinstance(endpoint, SyftError):
+                return endpoint
+            return endpoint.id
+        return SyftError(message="This function is not a custom function")
+
+    def _repr_markdown_(self, wrap_as_python: bool = False, indent: int = 0) -> str:
+        if self.custom_function and self.pre_kwargs is not None:
+            custom_path = self.pre_kwargs.get("path", "")
+            api_call = SyftAPICall(
+                node_uid=self.node_uid,
+                path="api.view",
+                args=[custom_path],
+                kwargs={},
+            )
+            endpoint = self.make_call(api_call=api_call)
+            if isinstance(endpoint, SyftError):
+                return endpoint._repr_html_()
+
+            str_repr = "## API: " + custom_path + "\n"
+            str_repr += (
+                "### Description: "
+                + f'<span style="font-weight: normal;">{endpoint.description}</span><br>'
+                + "\n"
+            )
+            str_repr += "#### Private Code:\n"
+            str_repr += as_markdown_python_code(endpoint.private_function) + "\n"
+            if endpoint.private_helper_functions:
+                str_repr += "##### Helper Functions:\n"
+                for helper_function in endpoint.private_helper_functions:
+                    str_repr += as_markdown_python_code(helper_function) + "\n"
+            str_repr += "#### Public Code:\n"
+            str_repr += as_markdown_python_code(endpoint.mock_function) + "\n"
+            if endpoint.mock_helper_functions:
+                str_repr += "##### Helper Functions:\n"
+                for helper_function in endpoint.mock_helper_functions:
+                    str_repr += as_markdown_python_code(helper_function) + "\n"
+            return str_repr
+        return super()._repr_markdown_()
+
 
 class RemoteUserCodeFunction(RemoteFunction):
     __canonical_name__ = "RemoteUserFunction"
     __version__ = SYFT_OBJECT_VERSION_2
     __repr_attrs__ = RemoteFunction.__repr_attrs__ + ["user_code_id"]
 
     api: SyftAPI
@@ -307,14 +377,24 @@
 
         # Validate and migrate args and kwargs
         res = validate_callable_args_and_kwargs(args, kwargs, self.signature)
         if isinstance(res, SyftError):
             return res
         args, kwargs = res
 
+        # Check remote function type to avoid function/method serialization
+        # We can recover the function/method pointer by its UID in server side.
+        for i in range(len(args)):
+            if isinstance(args[i], RemoteFunction) and args[i].custom_function:
+                args[i] = args[i].custom_function_id()
+
+        for k, v in kwargs.items():
+            if isinstance(v, RemoteFunction) and v.custom_function:
+                kwargs[k] = v.custom_function_id()
+
         args, kwargs = convert_to_pointers(
             api=self.api,
             node_uid=self.node_uid,
             args=args,
             kwargs=kwargs,
         )
 
@@ -370,22 +450,24 @@
             make_call=make_call,
             pre_kwargs=pre_kwargs,
             communication_protocol=communication_protocol,
             warning=warning,
             user_code_id=pre_kwargs["uid"],
         )
     else:
+        custom_function = bool(path == "api.call")
         remote_function = RemoteFunction(
             node_uid=node_uid,
             signature=signature,
             path=path,
             make_call=make_call,
             pre_kwargs=pre_kwargs,
             communication_protocol=communication_protocol,
             warning=warning,
+            custom_function=custom_function,
         )
 
     return remote_function
 
 
 def generate_remote_lib_function(
     api: SyftAPI,
@@ -633,14 +715,16 @@
     @staticmethod
     def for_user(
         node: AbstractNode,
         communication_protocol: PROTOCOL_TYPE,
         user_verify_key: SyftVerifyKey | None = None,
     ) -> SyftAPI:
         # relative
+        from ..service.api.api_service import APIService
+
         # TODO: Maybe there is a possibility of merging ServiceConfig and APIEndpoint
         from ..service.code.user_code_service import UserCodeService
 
         # find user role by verify_key
         # TODO: we should probably not allow empty verify keys but instead make user always register
         role = node.get_role_for_credentials(user_verify_key)
         _user_service_config_registry = UserServiceConfigRegistry.from_role(role)
@@ -729,42 +813,66 @@
                 doc_string=f"Users custom func {code_item.service_func_name}",
                 signature=code_item.signature,
                 has_self=False,
                 pre_kwargs={"uid": code_item.id},
             )
             endpoints[unique_path] = endpoint
 
+        # get admin defined custom api endpoints
+        method = node.get_method_with_context(APIService.get_endpoints, context)
+        custom_endpoints = method()
+        for custom_endpoint in custom_endpoints:
+            pre_kwargs = {"path": custom_endpoint.path}
+            service_path = "api.call"
+            path = custom_endpoint.path
+            api_end = custom_endpoint.path.split(".")[-1]
+            endpoint = APIEndpoint(
+                service_path=service_path,
+                module_path=path,
+                name=api_end,
+                description="",
+                doc_string="",
+                signature=custom_endpoint.signature,
+                has_self=False,
+                pre_kwargs=pre_kwargs,
+            )
+            endpoints[path] = endpoint
+
         return SyftAPI(
             node_name=node.name,
             node_uid=node.id,
             endpoints=endpoints,
             lib_endpoints=lib_endpoints,
             __user_role=role,
             communication_protocol=communication_protocol,
         )
 
     @property
     def user_role(self) -> ServiceRole:
         return self.__user_role
 
-    def make_call(self, api_call: SyftAPICall) -> Result:
+    def make_call(self, api_call: SyftAPICall, cache_result: bool = True) -> Result:
         signed_call = api_call.sign(credentials=self.signing_key)
         if self.connection is not None:
             signed_result = self.connection.make_call(signed_call)
         else:
             return SyftError(message="API connection is None")
 
         result = debox_signed_syftapicall_response(signed_result=signed_result)
 
         if isinstance(result, CachedSyftObject):
             if result.error_msg is not None:
-                prompt_warning_message(
-                    message=f"{result.error_msg}. Loading results from cache."
-                )
-            result = result.result
+                if cache_result:
+                    prompt_warning_message(
+                        message=f"{result.error_msg}. Loading results from cache."
+                    )
+                else:
+                    result = SyftError(message=result.error_msg)
+            if cache_result:
+                result = result.result
 
         if isinstance(result, OkErr):
             if result.is_ok():
                 result = result.ok()
             else:
                 result = result.err()
         # we update the api when we create objects that change it
```

### Comparing `syft-0.8.6b1/src/syft/client/client.py` & `syft-0.8.7b1/src/syft/client/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -905,14 +905,20 @@
     @property
     def users(self) -> APIModule | None:
         if self.api.has_service("user"):
             return self.api.services.user
         return None
 
     @property
+    def custom_api(self) -> APIModule | None:
+        if self.api.has_service("api"):
+            return self.api.services.api
+        return None
+
+    @property
     def numpy(self) -> APIModule | None:
         if self.api.has_lib("numpy"):
             return self.api.lib.numpy
         return None
 
     @property
     def settings(self) -> APIModule | None:
```

### Comparing `syft-0.8.6b1/src/syft/client/connection.py` & `syft-0.8.7b1/src/syft/client/connection.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6b1/src/syft/client/deploy.py` & `syft-0.8.7b1/src/syft/client/deploy.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6b1/src/syft/client/domain_client.py` & `syft-0.8.7b1/src/syft/client/domain_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 from ..service.sync.diff_state import ResolvedSyncState
 from ..service.sync.sync_state import SyncState
 from ..service.user.roles import Roles
 from ..service.user.user import UserView
 from ..service.user.user_roles import ServiceRole
 from ..types.blob_storage import BlobFile
 from ..types.uid import UID
-from ..util.fonts import fonts_css
+from ..util.fonts import FONT_CSS
 from ..util.util import get_mb_size
 from ..util.util import prompt_warning_message
 from .api import APIModule
 from .client import SyftClient
 from .client import login
 from .client import login_as_guest
 from .connection import NodeConnection
@@ -164,60 +164,53 @@
     #             raise ValueError(
     #                 f"Can't access the api. Please log in to {item.syft_node_location}"
     #             )
     #         return api.services.sync.get_permissions(items)
     #     else:
     #         return {}
 
+    def refresh(self) -> None:
+        if self._api and self._api.refresh_api_callback:
+            self._api.refresh_api_callback()
+
     def get_sync_state(self) -> SyncState | SyftError:
         state: SyncState = self.api.services.sync._get_state()
+        if isinstance(state, SyftError):
+            return state
+
         for uid, obj in state.objects.items():
             if isinstance(obj, ActionObject):
-                state.objects[uid] = obj.refresh_object()
+                obj = obj.refresh_object(resolve_nested=False)
+                obj.reload_cache()
+                state.objects[uid] = obj
         return state
 
     def apply_state(self, resolved_state: ResolvedSyncState) -> SyftSuccess | SyftError:
         if len(resolved_state.delete_objs):
             raise NotImplementedError("TODO implement delete")
         items = resolved_state.create_objs + resolved_state.update_objs
 
         action_objects = [x for x in items if isinstance(x, ActionObject)]
-        # permissions = self.get_permissions_for_other_node(items)
-
-        permissions: dict[UID, set[str]] = {}
-        for p in resolved_state.new_permissions:
-            if p.uid in permissions:
-                permissions[p.uid].add(p.permission_string)
-            else:
-                permissions[p.uid] = {p.permission_string}
-
-        storage_permissions: dict[UID, set[UID]] = {}
-        for sp in resolved_state.new_storage_permissions:
-            if sp.uid in storage_permissions:
-                storage_permissions[sp.uid].add(sp.node_uid)
-            else:
-                storage_permissions[sp.uid] = {sp.node_uid}
 
         for action_object in action_objects:
             # NOTE permissions are added separately server side
             action_object._send(self, add_storage_permission=False)
 
+        ignored_batches = resolved_state.ignored_batches
+
         res = self.api.services.sync.sync_items(
             items,
-            permissions,
-            storage_permissions,
+            resolved_state.new_permissions,
+            resolved_state.new_storage_permissions,
+            ignored_batches,
+            unignored_batches=resolved_state.unignored_batches,
         )
         if isinstance(res, SyftError):
             return res
 
-        # Add updated node state to store to have a previous_state for next sync
-        new_state = self.api.services.sync._get_state(add_to_store=True)
-        if isinstance(new_state, SyftError):
-            return new_state
-
         self._fetch_api(self.credentials)
         return res
 
     def upload_files(
         self,
         file_list: BlobFile | list[BlobFile] | str | list[str] | Path | list[Path],
         allow_recursive: bool = False,
@@ -487,15 +480,15 @@
             node_details += f"<strong>Node Side Type:</strong> {node_side_type}<br />"
             node_details += (
                 f"<strong>Syft Version:</strong> {self.metadata.syft_version}<br />"
             )
 
         return f"""
         <style>
-            {fonts_css}
+            {FONT_CSS}
 
             .syft-container {{
                 padding: 5px;
                 font-family: 'Open Sans';
             }}
             .syft-alert-info {{
                 color: #1F567A;
```

### Comparing `syft-0.8.6b1/src/syft/client/enclave_client.py` & `syft-0.8.7b1/src/syft/client/enclave_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from ..service.metadata.node_metadata import NodeMetadataJSON
 from ..service.network.routes import NodeRouteType
 from ..service.response import SyftError
 from ..service.response import SyftSuccess
 from ..types.syft_object import SYFT_OBJECT_VERSION_2
 from ..types.syft_object import SyftObject
 from ..types.uid import UID
-from ..util.fonts import fonts_css
+from ..util.fonts import FONT_CSS
 from .api import APIModule
 from .client import SyftClient
 from .client import login
 from .client import login_as_guest
 from .protocol import SyftProtocol
 
 if TYPE_CHECKING:
@@ -178,15 +178,15 @@
             node_details += f"<strong>Node Side Type:</strong> {node_side_type}<br />"
             node_details += (
                 f"<strong>Syft Version:</strong> {self.metadata.syft_version}<br />"
             )
 
         return f"""
         <style>
-            {fonts_css}
+            {FONT_CSS}
 
             .syft-container {{
                 padding: 5px;
                 font-family: 'Open Sans';
             }}
             .syft-alert-info {{
                 color: #1F567A;
```

### Comparing `syft-0.8.6b1/src/syft/client/gateway_client.py` & `syft-0.8.7b1/src/syft/client/gateway_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from ..node.credentials import SyftSigningKey
 from ..serde.serializable import serializable
 from ..service.network.node_peer import NodePeer
 from ..service.response import SyftError
 from ..service.response import SyftException
 from ..types.syft_object import SYFT_OBJECT_VERSION_2
 from ..types.syft_object import SyftObject
-from ..util.fonts import fonts_css
+from ..util.fonts import FONT_CSS
 from .client import SyftClient
 
 
 @serializable()
 class GatewayClient(SyftClient):
     # TODO: add widget repr for gateway client
 
@@ -101,15 +101,15 @@
             node_details += f"<strong>Node Side Type:</strong> {node_side_type}<br />"
             node_details += (
                 f"<strong>Syft Version:</strong> {self.metadata.syft_version}<br />"
             )
 
         return f"""
         <style>
-            {fonts_css}
+            {FONT_CSS}
 
             .syft-container {{
                 padding: 5px;
                 font-family: 'Open Sans';
             }}
             .syft-alert-info {{
                 color: #1F567A;
```

### Comparing `syft-0.8.6b1/src/syft/client/registry.py` & `syft-0.8.7b1/src/syft/client/registry.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 # future
 from __future__ import annotations
 
 # stdlib
 from concurrent import futures
+import json
+import os
 from typing import Any
 
 # third party
 import pandas as pd
 import requests
 
 # relative
@@ -18,28 +20,56 @@
 from ..util.logger import error
 from ..util.logger import warning
 from .client import SyftClient as Client
 
 NETWORK_REGISTRY_URL = (
     "https://raw.githubusercontent.com/OpenMined/NetworkRegistry/main/gateways.json"
 )
+
 NETWORK_REGISTRY_REPO = "https://github.com/OpenMined/NetworkRegistry"
 
 
+def _get_all_networks(network_json: dict, version: str) -> list[dict]:
+    return network_json.get(version, {}).get("gateways", [])
+
+
 class NetworkRegistry:
     def __init__(self) -> None:
         self.all_networks: list[dict] = []
+
         try:
-            response = requests.get(NETWORK_REGISTRY_URL)  # nosec
-            network_json = response.json()
-            self.all_networks = network_json["2.0.0"]["gateways"]
+            network_json = self.load_network_registry_json()
+            self.all_networks = _get_all_networks(
+                network_json=network_json, version="2.0.0"
+            )
+        except Exception as e:
+            warning(
+                f"Failed to get Network Registry, go checkout: {NETWORK_REGISTRY_REPO}. Exception: {e}"
+            )
+
+    @staticmethod
+    def load_network_registry_json() -> dict:
+        try:
+            # Get the environment variable
+            network_registry_json = os.getenv("NETWORK_REGISTRY_JSON")
+            # If the environment variable exists, use it
+            if network_registry_json is not None:
+                network_json: dict = json.loads(network_registry_json)
+            else:
+                # Load the network registry from the NETWORK_REGISTRY_URL
+                response = requests.get(NETWORK_REGISTRY_URL, timeout=10)  # nosec
+                network_json = response.json()
+
+            return network_json
+
         except Exception as e:
             warning(
                 f"Failed to get Network Registry, go checkout: {NETWORK_REGISTRY_REPO}. {e}"
             )
+            return {}
 
     @property
     def online_networks(self) -> list[dict]:
         networks = self.all_networks
 
         def check_network(network: dict) -> dict[Any, Any] | None:
             url = "http://" + network["host_or_ip"] + ":" + str(network["port"]) + "/"
@@ -79,30 +109,26 @@
         # We can use a with statement to ensure threads are cleaned up promptly
         with futures.ThreadPoolExecutor(max_workers=20) as executor:
             # map
             _online_networks = list(
                 executor.map(lambda network: check_network(network), networks)
             )
 
-        online_networks = []
-        for each in _online_networks:
-            if each is not None:
-                online_networks.append(each)
-        return online_networks
+        return [network for network in _online_networks if network is not None]
 
     def _repr_html_(self) -> str:
         on = self.online_networks
         if len(on) == 0:
-            return "(no gateways online - try syft.gateways.all_gateways to see offline gateways)"
+            return "(no gateways online - try syft.gateways.all_networks to see offline gateways)"
         return pd.DataFrame(on)._repr_html_()  # type: ignore
 
     def __repr__(self) -> str:
         on = self.online_networks
         if len(on) == 0:
-            return "(no gateways online - try syft.gateways.all_gateways to see offline gateways)"
+            return "(no gateways online - try syft.gateways.all_networks to see offline gateways)"
         return pd.DataFrame(on).to_string()
 
     @staticmethod
     def create_client(network: dict[str, Any]) -> Client:
         # relative
         from ..client.client import connect
 
@@ -127,24 +153,33 @@
                     return self.create_client(network=network)
         raise KeyError(f"Invalid key: {key} for {on}")
 
 
 class DomainRegistry:
     def __init__(self) -> None:
         self.all_networks: list[dict] = []
-        self.all_domains: list = []
+        self.all_domains: dict[str, NodePeer] = {}
         try:
-            response = requests.get(NETWORK_REGISTRY_URL)  # nosec
-            network_json = response.json()
-            self.all_networks = network_json["2.0.0"]["gateways"]
+            network_json = NetworkRegistry.load_network_registry_json()
+            self.all_networks = _get_all_networks(
+                network_json=network_json, version="2.0.0"
+            )
+            self._get_all_domains()
         except Exception as e:
             warning(
                 f"Failed to get Network Registry, go checkout: {NETWORK_REGISTRY_REPO}. {e}"
             )
 
+    def _get_all_domains(self) -> None:
+        for network in self.all_networks:
+            network_client = NetworkRegistry.create_client(network)
+            domains: list[NodePeer] = network_client.domains.retrieve_nodes()
+            for domain in domains:
+                self.all_domains[str(domain.id)] = domain
+
     @property
     def online_networks(self) -> list[dict]:
         networks = self.all_networks
 
         def check_network(network: dict) -> dict[Any, Any] | None:
             url = "http://" + network["host_or_ip"] + ":" + str(network["port"]) + "/"
             try:
@@ -174,91 +209,85 @@
                         if res.status_code == 200:
                             network["version"] = res.json()["syft_version"]
                         else:
                             network["version"] = "unknown"
                     except Exception:
                         network["version"] = "unknown"
                 return network
+
             return None
 
         # We can use a with statement to ensure threads are cleaned up promptly
         with futures.ThreadPoolExecutor(max_workers=20) as executor:
             # map
             _online_networks = list(
                 executor.map(lambda network: check_network(network), networks)
             )
 
-        online_networks = []
-        for each in _online_networks:
-            if each is not None:
-                online_networks.append(each)
-        return online_networks
+        return [network for network in _online_networks if network is not None]
 
     @property
     def online_domains(self) -> list[tuple[NodePeer, NodeMetadataJSON | None]]:
         def check_domain(
             peer: NodePeer,
         ) -> tuple[NodePeer, NodeMetadataJSON | None] | None:
             try:
                 guest_client = peer.guest_client
                 metadata = guest_client.metadata
                 return peer, metadata
-            except Exception:  # nosec
-                pass
+            except Exception as e:  # nosec
+                print(f"Error in checking domain with exception {e}")
             return None
 
         networks = self.online_networks
 
-        self.all_domains = []
         # We can use a with statement to ensure threads are cleaned up promptly
         with futures.ThreadPoolExecutor(max_workers=20) as executor:
             # map
             _all_online_domains = []
             for network in networks:
                 network_client = NetworkRegistry.create_client(network)
-                domains = network_client.domains
-                self.all_domains += domains
+                domains: list[NodePeer] = network_client.domains.retrieve_nodes()
+                for domain in domains:
+                    self.all_domains[str(domain.id)] = domain
                 _online_domains = list(
                     executor.map(lambda domain: check_domain(domain), domains)
                 )
                 _all_online_domains += _online_domains
 
-        online_domains = []
-        for each in _all_online_domains:
-            if each is not None:
-                online_domains.append(each)
-        return online_domains
+        return [domain for domain in _all_online_domains if domain is not None]
 
     def __make_dict__(self) -> list[dict[str, Any]]:
         on = self.online_domains
-        domains = []
-        domain_dict: dict[str, Any] = {}
+        domains: list[dict[str, Any]] = []
         for domain, metadata in on:
+            domain_dict: dict[str, Any] = {}
             domain_dict["name"] = domain.name
             if metadata is not None:
                 domain_dict["organization"] = metadata.organization
                 domain_dict["version"] = metadata.syft_version
             route = None
             if len(domain.node_routes) > 0:
                 route = domain.pick_highest_priority_route()
             domain_dict["host_or_ip"] = route.host_or_ip if route else "-"
             domain_dict["protocol"] = route.protocol if route else "-"
             domain_dict["port"] = route.port if route else "-"
             domain_dict["id"] = domain.id
             domains.append(domain_dict)
+
         return domains
 
     def _repr_html_(self) -> str:
-        on = self.__make_dict__()
+        on: list[dict[str, Any]] = self.__make_dict__()
         if len(on) == 0:
             return "(no domains online - try syft.domains.all_domains to see offline domains)"
         return pd.DataFrame(on)._repr_html_()  # type: ignore
 
     def __repr__(self) -> str:
-        on = self.__make_dict__()
+        on: list[dict[str, Any]] = self.__make_dict__()
         if len(on) == 0:
             return "(no domains online - try syft.domains.all_domains to see offline domains)"
         return pd.DataFrame(on).to_string()
 
     def create_client(self, peer: NodePeer) -> Client:
         try:
             return peer.guest_client
```

### Comparing `syft-0.8.6b1/src/syft/client/syncing.py` & `syft-0.8.7b1/src/syft/client/syncing.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,127 +1,215 @@
 # stdlib
+from collections.abc import Callable
 from time import sleep
 
 # relative
+from ..abstract_node import NodeSideType
 from ..service.action.action_permissions import ActionObjectPermission
 from ..service.action.action_permissions import ActionPermission
 from ..service.action.action_permissions import StoragePermission
 from ..service.code.user_code import UserCode
 from ..service.job.job_stash import Job
 from ..service.sync.diff_state import NodeDiff
 from ..service.sync.diff_state import ObjectDiff
 from ..service.sync.diff_state import ObjectDiffBatch
 from ..service.sync.diff_state import ResolvedSyncState
-from ..service.sync.diff_state import SyncDecision
+from ..service.sync.diff_state import SyncInstruction
+from ..service.sync.resolve_widget import ResolveWidget
 from ..service.sync.sync_state import SyncState
+from .client import SyftClient
+from .sync_decision import SyncDecision
+from .sync_decision import SyncDirection
+
+
+def compare_states(state1: SyncState, state2: SyncState) -> NodeDiff:
+    # NodeDiff
+    if (
+        state1.node_side_type == NodeSideType.LOW_SIDE
+        and state2.node_side_type == NodeSideType.HIGH_SIDE
+    ):
+        low_state = state1
+        high_state = state2
+        direction = SyncDirection.LOW_TO_HIGH
+    elif (
+        state1.node_side_type == NodeSideType.HIGH_SIDE
+        and state2.node_side_type == NodeSideType.LOW_SIDE
+    ):
+        low_state = state2
+        high_state = state1
+        direction = SyncDirection.HIGH_TO_LOW
+    else:
+        raise ValueError("Invalid SyncStates")
+    return NodeDiff.from_sync_state(
+        low_state=low_state, high_state=high_state, direction=direction
+    )
 
 
-def compare_states(low_state: SyncState, high_state: SyncState) -> NodeDiff:
-    return NodeDiff.from_sync_state(low_state=low_state, high_state=high_state)
+def compare_clients(low_client: SyftClient, high_client: SyftClient) -> NodeDiff:
+    return compare_states(low_client.get_sync_state(), high_client.get_sync_state())
 
 
-def get_user_input_for_resolve() -> str | None:
-    print(
-        "Do you want to keep the low state or the high state for these objects? choose 'low' or 'high'"
-    )
+def get_user_input_for_resolve() -> SyncDecision:
+    options = [x.value for x in SyncDecision]
+    options_str = ", ".join(options[:-1]) + f" or {options[-1]}"
+    print(f"How do you want to sync these objects? choose between {options_str}")
 
     while True:
         decision = input()
         decision = decision.lower()
 
-        if decision in ["low", "high"]:
-            return decision
-        else:
-            print("Please choose between `low` or `high`")
+        try:
+            return SyncDecision(decision)
+        except ValueError:
+            print(f"Please choose between {options_str}")
+
+
+def handle_ignore_skip(
+    batch: ObjectDiffBatch, decision: SyncDecision, other_batches: list[ObjectDiffBatch]
+) -> None:
+    # make sure type is SyncDecision at runtime
+    decision = SyncDecision(decision)
+
+    if decision == SyncDecision.skip or decision == SyncDecision.ignore:
+        skipped_or_ignored_ids = {
+            x.object_id for x in batch.get_dependents(include_roots=False)
+        }
+        for other_batch in other_batches:
+            if other_batch.decision != decision:
+                # Currently, this is not recursive, in the future it might be
+                other_batch_ids = {
+                    d.object_id
+                    for d in other_batch.get_dependencies(include_roots=True)
+                }
+                if len(other_batch_ids & skipped_or_ignored_ids) != 0:
+                    other_batch.decision = decision
+                    skipped_or_ignored_ids.update(other_batch_ids)
+                    action = "Skipping" if decision == SyncDecision.skip else "Ignoring"
+                    print(
+                        f"\n{action} other batch with root {other_batch.root_type.__name__}\n"
+                    )
+
+
+def resolve_single(obj_diff_batch: ObjectDiffBatch) -> ResolveWidget:
+    widget = ResolveWidget(obj_diff_batch)
+    return widget
 
 
 def resolve(
     state: NodeDiff,
     decision: str | None = None,
+    decision_callback: Callable[[ObjectDiffBatch], SyncDecision] | None = None,
     share_private_objects: bool = False,
     ask_for_input: bool = True,
 ) -> tuple[ResolvedSyncState, ResolvedSyncState]:
+    # TODO: fix this
+    previously_ignored_batches = state.low_state.ignored_batches
     # TODO: only add permissions for objects where we manually give permission
     # Maybe default read permission for some objects (high -> low)
     resolved_state_low = ResolvedSyncState(node_uid=state.low_node_uid, alias="low")
     resolved_state_high = ResolvedSyncState(node_uid=state.high_node_uid, alias="high")
 
-    for batch_diff in state.hierarchies:
-        batch_decision = decision
-        if all(diff.status == "SAME" for diff in batch_diff.diffs):
+    for batch_diff in state.batches:
+        if batch_diff.is_unchanged:
             # Hierarchy has no diffs
             continue
 
-        print(batch_diff.__repr__())
-
-        if batch_decision is None:
+        if batch_diff.decision is not None:
+            # handles ignores
+            batch_decision = batch_diff.decision
+        elif decision is not None:
+            print(batch_diff.__repr__())
+            batch_decision = SyncDecision(decision)
+        elif decision_callback is not None:
+            batch_decision = decision_callback(batch_diff)
+        else:
+            print(batch_diff.__repr__())
             batch_decision = get_user_input_for_resolve()
 
-        sync_decisions: list[SyncDecision] = get_sync_decisions_for_batch_items(
-            batch_diff,
-            batch_decision,
-            share_private_objects=share_private_objects,
-            ask_for_input=ask_for_input,
-        )
+        batch_diff.decision = batch_decision
 
-        print(f"Decision: Syncing {len(batch_diff)} objects from {batch_decision} side")
+        other_batches = [b for b in state.batches if b is not batch_diff]
+        handle_ignore_skip(batch_diff, batch_decision, other_batches)
 
-        for sync_decision in sync_decisions:
-            resolved_state_low.add_sync_decision(sync_decision)
-            resolved_state_high.add_sync_decision(sync_decision)
+        if batch_decision not in [SyncDecision.skip, SyncDecision.ignore]:
+            sync_instructions = get_sync_instructions_for_batch_items_for_add(
+                batch_diff,
+                batch_decision,
+                share_private_objects=share_private_objects,
+                ask_for_input=ask_for_input,
+            )
+        else:
+            sync_instructions = []
+            if batch_decision == SyncDecision.ignore:
+                resolved_state_high.add_ignored(batch_diff)
+                resolved_state_low.add_ignored(batch_diff)
+
+        if (
+            batch_diff.root_id in previously_ignored_batches
+            and batch_diff.decision != SyncDecision.ignore
+        ):
+            resolved_state_high.add_unignored(batch_diff.root_id)
+            resolved_state_low.add_unignored(batch_diff.root_id)
+
+        print(f"Decision: Syncing {len(sync_instructions)} objects")
+
+        for sync_instruction in sync_instructions:
+            resolved_state_low.add_sync_instruction(sync_instruction)
+            resolved_state_high.add_sync_instruction(sync_instruction)
 
         print()
         print("=" * 100)
         print()
 
     return resolved_state_low, resolved_state_high
 
 
-def get_sync_decisions_for_batch_items(
+def get_sync_instructions_for_batch_items_for_add(
     batch_diff: ObjectDiffBatch,
-    decision: str,
+    decision: SyncDecision,
     share_private_objects: bool = False,
     ask_for_input: bool = True,
-) -> list[SyncDecision]:
-    sync_decisions: list[SyncDecision] = []
+) -> list[SyncInstruction]:
+    sync_decisions: list[SyncInstruction] = []
 
     unpublished_private_high_diffs: list[ObjectDiff] = []
-    for diff in batch_diff.diffs:
+    for diff in batch_diff.get_dependents(include_roots=False):
         is_high_private_object = (
             diff.high_obj is not None and diff.high_obj._has_private_sync_attrs()
         )
         is_low_published_object = diff.low_node_uid in diff.low_storage_permissions
         if is_high_private_object and not is_low_published_object:
             unpublished_private_high_diffs.append(diff)
 
     user_codes_high: list[UserCode] = [
         diff.high_obj
-        for diff in batch_diff.diffs
+        for diff in batch_diff.get_dependencies(include_roots=True)
         if isinstance(diff.high_obj, UserCode)
     ]
-    if len(user_codes_high) > 1:
-        raise ValueError("too many user codes")
+
     if len(user_codes_high) == 0:
         user_code_high = None
     else:
+        # NOTE we can always assume the first usercode is
+        # not a nested code, because diffs are sorted in depth-first order
         user_code_high = user_codes_high[0]
 
     if user_code_high is None and len(unpublished_private_high_diffs):
         raise ValueError("Found unpublished private objects without user code")
 
     if share_private_objects:
         private_high_diffs_to_share = unpublished_private_high_diffs
     elif ask_for_input:
         private_high_diffs_to_share = ask_user_input_permission(
             user_code_high, unpublished_private_high_diffs
         )
     else:
         private_high_diffs_to_share = []
 
-    for diff in batch_diff.diffs:
+    for diff in batch_diff.get_dependencies(include_roots=False):
         is_unpublished_private_diff = diff in unpublished_private_high_diffs
         has_share_decision = diff in private_high_diffs_to_share
 
         if isinstance(diff.high_obj, Job):
             if user_code_high is None:
                 raise ValueError("Job without user code")
             # Jobs are always shared
@@ -157,24 +245,27 @@
 
         new_storage_permissions_lowside = []
         if not mockify:
             new_storage_permissions_lowside = [
                 StoragePermission(uid=diff.object_id, node_uid=diff.low_node_uid)
             ]
 
-        # Always share to high_side
-        if diff.status == "NEW" and diff.high_obj is None:
+        if (
+            diff.status == "NEW"
+            and diff.high_obj is None
+            and decision == SyncDecision.low
+        ):
             new_storage_permissions_highside = [
                 StoragePermission(uid=diff.object_id, node_uid=diff.high_node_uid)
             ]
         else:
             new_storage_permissions_highside = []
 
         sync_decisions.append(
-            SyncDecision(
+            SyncInstruction(
                 diff=diff,
                 decision=decision,
                 new_permissions_lowside=new_permissions_low_side,
                 new_storage_permissions_lowside=new_storage_permissions_lowside,
                 new_storage_permissions_highside=new_storage_permissions_highside,
                 mockify=mockify,
             )
@@ -184,15 +275,16 @@
 
 
 QUESTION_SHARE_PRIVATE_OBJS = """You currently have the following private objects:
 
 {objects_str}
 
 Do you want to share some of these private objects? If so type the first 3 characters of the id e.g. 'abc'.
-If you dont want to share any more private objects, type "no"
+If you want to share all private objects, type "all".
+If you dont want to share any more private objects, type "no".
 """
 
 CONFIRMATION_SHARE_PRIVATE_OBJ = """Setting permissions for {object_type} #{object_id} to share with {user_verify_key},
 this will become effective when you call client.apply_state(<resolved_state>))
 """
 
 
@@ -219,14 +311,18 @@
         )
         print(QUESTION_SHARE_PRIVATE_OBJS.format(objects_str=objects_str), flush=True)
 
         sleep(0.1)
         res = input()
         if res == "no":
             break
+
+        if res == "all":
+            private_high_diffs_to_share.extend(remaining_private_high_diffs)
+            remaining_private_high_diffs = []
         elif len(res) >= 3:
             matches = [
                 diff
                 for diff in remaining_private_high_diffs
                 if str(diff.object_id).startswith(res)
             ]
             if len(matches) == 0:
```

### Comparing `syft-0.8.6b1/src/syft/client/user_settings.py` & `syft-0.8.7b1/src/syft/client/user_settings.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6b1/src/syft/custom_worker/builder.py` & `syft-0.8.7b1/src/syft/custom_worker/builder.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6b1/src/syft/custom_worker/builder_docker.py` & `syft-0.8.7b1/src/syft/custom_worker/builder_docker.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6b1/src/syft/custom_worker/builder_k8s.py` & `syft-0.8.7b1/src/syft/custom_worker/builder_k8s.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6b1/src/syft/custom_worker/builder_types.py` & `syft-0.8.7b1/src/syft/custom_worker/builder_types.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6b1/src/syft/custom_worker/config.py` & `syft-0.8.7b1/src/syft/custom_worker/config.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6b1/src/syft/custom_worker/k8s.py` & `syft-0.8.7b1/src/syft/custom_worker/k8s.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6b1/src/syft/custom_worker/runner_k8s.py` & `syft-0.8.7b1/src/syft/custom_worker/runner_k8s.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6b1/src/syft/custom_worker/utils.py` & `syft-0.8.7b1/src/syft/custom_worker/utils.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6b1/src/syft/exceptions/exception.py` & `syft-0.8.7b1/src/syft/exceptions/exception.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6b1/src/syft/external/oblv/deployment_client.py` & `syft-0.8.7b1/src/syft/service/user/user.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,374 +1,361 @@
-# future
-from __future__ import annotations
-
 # stdlib
 from collections.abc import Callable
-from datetime import datetime
-import os
-from signal import SIGTERM
-import subprocess  # nosec
-import sys
-import time
+from getpass import getpass
 from typing import Any
-from typing import TYPE_CHECKING
 
 # third party
-from oblv_ctl import OblvClient
+from bcrypt import checkpw
+from bcrypt import gensalt
+from bcrypt import hashpw
+from pydantic import EmailStr
+from pydantic import ValidationError
 from pydantic import field_validator
-import requests
 
 # relative
-from ...client.api import SyftAPI
-from ...client.client import SyftClient
-from ...client.client import login
-from ...client.client import login_as_guest
-from ...client.enclave_client import EnclaveMetadata
+from ...client.api import APIRegistry
 from ...node.credentials import SyftSigningKey
+from ...node.credentials import SyftVerifyKey
 from ...serde.serializable import serializable
-from ...service.response import SyftError
+from ...types.syft_metaclass import Empty
+from ...types.syft_object import PartialSyftObject
+from ...types.syft_object import SYFT_OBJECT_VERSION_2
+from ...types.syft_object import SYFT_OBJECT_VERSION_3
+from ...types.syft_object import SyftObject
+from ...types.transforms import TransformContext
+from ...types.transforms import drop
+from ...types.transforms import generate_id
+from ...types.transforms import keep
+from ...types.transforms import make_set_default
+from ...types.transforms import transform
+from ...types.transforms import validate_email
 from ...types.uid import UID
-from ...util.util import bcolors
-from .constants import LOCAL_MODE
-from .exceptions import OblvEnclaveError
-from .exceptions import OblvUnAuthorizedError
-from .oblv_proxy import check_oblv_proxy_installation_status
-
-if TYPE_CHECKING:
-    # relative
-    from ...service.code.user_code import SubmitUserCode
+from ..notifier.notifier_enums import NOTIFIERS
+from ..response import SyftError
+from ..response import SyftSuccess
+from .user_roles import ServiceRole
 
 
 @serializable()
-class OblvMetadata(EnclaveMetadata):
-    """Contains Metadata to connect to Oblivious Enclave"""
+class User(SyftObject):
+    # version
+    __canonical_name__ = "User"
+    __version__ = SYFT_OBJECT_VERSION_3
+
+    id: UID | None = None  # type: ignore[assignment]
+
+    # fields
+    notifications_enabled: dict[NOTIFIERS, bool] = {
+        NOTIFIERS.EMAIL: True,
+        NOTIFIERS.SMS: False,
+        NOTIFIERS.SLACK: False,
+        NOTIFIERS.APP: False,
+    }
+    email: EmailStr | None = None
+    name: str | None = None
+    hashed_password: str | None = None
+    salt: str | None = None
+    signing_key: SyftSigningKey | None = None
+    verify_key: SyftVerifyKey | None = None
+    role: ServiceRole | None = None
+    institution: str | None = None
+    website: str | None = None
+    created_at: str | None = None
+    # TODO where do we put this flag?
+    mock_execution_permission: bool = False
+
+    # serde / storage rules
+    __attr_searchable__ = ["name", "email", "verify_key", "role"]
+    __attr_unique__ = ["email", "signing_key", "verify_key"]
+    __repr_attrs__ = ["name", "email"]
+
+
+def default_role(role: ServiceRole) -> Callable:
+    return make_set_default(key="role", value=role)
+
+
+def hash_password(context: TransformContext) -> TransformContext:
+    if context.output is None:
+        return context
+
+    if context.output["password"] is not None and (
+        (context.output["password_verify"] is None)
+        or context.output["password"] == context.output["password_verify"]
+    ):
+        salt, hashed = salt_and_hash_password(context.output["password"], 12)
+        context.output["hashed_password"] = hashed
+        context.output["salt"] = salt
 
-    deployment_id: str | None = None
-    oblv_client: OblvClient | None = None
+    return context
 
-    @field_validator("deployment_id")
-    @classmethod
-    def check_valid_deployment_id(cls, deployment_id: str) -> str:
-        if not deployment_id and not LOCAL_MODE:
-            raise ValueError(
-                f"Deployment ID should be a valid string: {deployment_id}"
-                + "in cloud deployment of enclave"
-                + "For testing set the LOCAL_MODE variable in constants.py"
-            )
-        return deployment_id
 
-    @field_validator("oblv_client")
+def generate_key(context: TransformContext) -> TransformContext:
+    if context.output is not None:
+        signing_key = SyftSigningKey.generate()
+        context.output["signing_key"] = signing_key
+        context.output["verify_key"] = signing_key.verify_key
+
+    return context
+
+
+def salt_and_hash_password(password: str, rounds: int) -> tuple[str, str]:
+    bytes_pass = password.encode("UTF-8")
+    salt = gensalt(rounds=rounds)
+    hashed = hashpw(bytes_pass, salt)
+    hashed_bytes = hashed.decode("UTF-8")
+    salt_bytes = salt.decode("UTF-8")
+    return salt_bytes, hashed_bytes
+
+
+def check_pwd(password: str, hashed_password: str) -> bool:
+    return checkpw(
+        password=password.encode("utf-8"),
+        hashed_password=hashed_password.encode("utf-8"),
+    )
+
+
+@serializable()
+class UserUpdate(PartialSyftObject):
+    __canonical_name__ = "UserUpdate"
+    __version__ = SYFT_OBJECT_VERSION_3
+
+    @field_validator("role", mode="before")
     @classmethod
-    def check_valid_oblv_client(cls, oblv_client: OblvClient) -> OblvClient:
-        if not oblv_client and not LOCAL_MODE:
-            raise ValueError(
-                f"Oblivious Client should be a valid client: {oblv_client}"
-                + "in cloud deployment of enclave"
-                + "For testing set the LOCAL_MODE variable in constants.py"
-            )
-        return oblv_client
-
-
-class DeploymentClient:
-    deployment_id: str
-    key_name: str
-    domain_clients: list[SyftClient]  # List of domain client objects
-    oblv_client: OblvClient = None
-    __conn_string: str
-    __logs: Any
-    __process: Any
-    __enclave_client: SyftClient | None
+    def str_to_role(cls, v: Any) -> Any:
+        if isinstance(v, str) and hasattr(ServiceRole, v.upper()):
+            return getattr(ServiceRole, v.upper())
+        return v
+
+    email: EmailStr
+    name: str
+    role: ServiceRole  # make sure role cant be set without uid
+    password: str
+    password_verify: str
+    verify_key: SyftVerifyKey
+    institution: str
+    website: str
+    mock_execution_permission: bool
 
-    def __init__(
-        self,
-        domain_clients: list[SyftClient],
-        deployment_id: str,
-        oblv_client: OblvClient | None = None,
-        key_name: str | None = None,
-        api: SyftAPI | None = None,
-    ):
-        if not domain_clients:
-            raise Exception(
-                "domain_clients should be populated with valid domain nodes"
-            )
-        self.deployment_id = deployment_id
-        self.key_name: str | None = key_name
-        self.oblv_client = oblv_client
-        self.domain_clients = domain_clients
-        self.__conn_string = ""
-        self.__process = None
-        self.__logs = None
-        self._api = api
-        self.__enclave_client: SyftClient | None = None
 
-    def make_request_to_enclave(
-        self,
-        request_method: Callable,
-        connection_string: str,
-        params: dict | None = None,
-        files: dict | None = None,
-        data: dict | None = None,
-        json: dict | None = None,
-    ) -> Any:
-        header = {}
-        if LOCAL_MODE:
-            header["x-oblv-user-name"] = "enclave_test"
-            header["x-oblv-user-role"] = "user"
-        else:
-            depl = self.oblv_client.deployment_info(self.deployment_id)
-            if depl.is_deleted:
-                raise Exception(
-                    "User cannot connect to this deployment, as it is no longer available."
-                )
-        return request_method(
-            connection_string,
-            headers=header,
-            params=params,
-            files=files,
-            data=data,
-            json=json,
-        )
+@serializable()
+class UserCreate(SyftObject):
+    __canonical_name__ = "UserCreate"
+    __version__ = SYFT_OBJECT_VERSION_3
+
+    email: EmailStr
+    name: str
+    role: ServiceRole | None = None  # type: ignore[assignment]
+    password: str
+    password_verify: str | None = None  # type: ignore[assignment]
+    verify_key: SyftVerifyKey | None = None  # type: ignore[assignment]
+    institution: str | None = ""  # type: ignore[assignment]
+    website: str | None = ""  # type: ignore[assignment]
+    created_by: SyftSigningKey | None = None  # type: ignore[assignment]
+    mock_execution_permission: bool = False
+
+    __repr_attrs__ = ["name", "email"]
 
-    def set_conn_string(self, url: str) -> None:
-        self.__conn_string = url
 
-    def initiate_connection(self, connection_port: int = 3030) -> None:
-        if LOCAL_MODE:
-            self.__conn_string = f"http://127.0.0.1:{connection_port}"
-            return
-        check_oblv_proxy_installation_status()
-        self.close_connection()  # To close any existing connections
-        public_file_name = os.path.join(
-            os.path.expanduser("~"),
-            ".ssh",
-            self.key_name,
-            self.key_name + "_public.der",
+@serializable()
+class UserSearch(PartialSyftObject):
+    __canonical_name__ = "UserSearch"
+    __version__ = SYFT_OBJECT_VERSION_2
+
+    id: UID
+    email: EmailStr
+    verify_key: SyftVerifyKey
+    name: str
+
+
+@serializable()
+class UserView(SyftObject):
+    __canonical_name__ = "UserView"
+    __version__ = SYFT_OBJECT_VERSION_3
+
+    notifications_enabled: dict[NOTIFIERS, bool] = {
+        NOTIFIERS.EMAIL: True,
+        NOTIFIERS.SMS: False,
+        NOTIFIERS.SLACK: False,
+        NOTIFIERS.APP: False,
+    }
+    email: EmailStr
+    name: str
+    role: ServiceRole  # make sure role cant be set without uid
+    institution: str | None = None
+    website: str | None = None
+    mock_execution_permission: bool
+
+    __repr_attrs__ = [
+        "name",
+        "email",
+        "institution",
+        "website",
+        "role",
+        "notifications_enabled",
+    ]
+
+    def _coll_repr_(self) -> dict[str, Any]:
+        return {
+            "Name": self.name,
+            "Email": self.email,
+            "Institute": self.institution,
+            "Website": self.website,
+            "Role": self.role.name.capitalize(),
+            "Notifications": "Email: "
+            + (
+                "Enabled" if self.notifications_enabled[NOTIFIERS.EMAIL] else "Disabled"
+            ),
+        }
+
+    def _set_password(self, new_password: str) -> SyftError | SyftSuccess:
+        api = APIRegistry.api_for(
+            node_uid=self.syft_node_location,
+            user_verify_key=self.syft_client_verify_key,
         )
-        private_file_name = os.path.join(
-            os.path.expanduser("~"),
-            ".ssh",
-            self.key_name,
-            self.key_name + "_private.der",
+        if api is None:
+            return SyftError(message=f"You must login to {self.node_uid}")
+
+        api.services.user.update(
+            uid=self.id, user_update=UserUpdate(password=new_password)
         )
-        log_file_name = os.path.join(
-            os.path.expanduser("~"),
-            ".oblv_syft_logs",
-            "proxy_logs_" + datetime.now().strftime("%d_%m_%Y_%H_%M_%S") + ".log",
+        return SyftSuccess(
+            message=f"Successfully updated password for "
+            f"user '{self.name}' with email '{self.email}'."
         )
-        # Creating directory if not exist
-        os.makedirs(os.path.dirname(log_file_name), exist_ok=True)
-        log_file = open(log_file_name, "wb")
-        depl = self.oblv_client.deployment_info(self.deployment_id)
-        if depl.is_deleted:
-            raise Exception(
-                "User cannot connect to this deployment, as it is no longer available."
-            )
+
+    def set_password(
+        self, new_password: str | None = None, confirm: bool = True
+    ) -> SyftError | SyftSuccess:
+        """Set a new password interactively with confirmed password from user input"""
+        # TODO: Add password validation for special characters
+        if not new_password:
+            new_password = getpass("New Password: ")
+
+        if confirm:
+            confirmed_password: str = getpass("Please confirm your password: ")
+            if confirmed_password != new_password:
+                return SyftError(message="Passwords do not match !")
+        return self._set_password(new_password)
+
+    def set_email(self, email: str) -> SyftSuccess | SyftError:
+        # validate email address
+        api = APIRegistry.api_for(
+            node_uid=self.syft_node_location,
+            user_verify_key=self.syft_client_verify_key,
+        )
+        if api is None:
+            return SyftError(message=f"You must login to {self.node_uid}")
+
         try:
-            if depl.is_dev_env:
-                process = subprocess.Popen(  # nosec
-                    [
-                        "oblv",
-                        "connect",
-                        "--private-key",
-                        private_file_name,
-                        "--public-key",
-                        public_file_name,
-                        "--url",
-                        depl.instance.service_url,
-                        "--pcr0",
-                        depl.pcr_codes[0],
-                        "--pcr1",
-                        depl.pcr_codes[1],
-                        "--pcr2",
-                        depl.pcr_codes[2],
-                        "--port",
-                        "443",
-                        "--lport",
-                        str(connection_port),
-                        "--disable-pcr-check",
-                    ],
-                    stdout=log_file,
-                    stderr=log_file,
-                )
-            else:
-                process = subprocess.Popen(  # nosec
-                    [
-                        "oblv",
-                        "connect",
-                        "--private-key",
-                        private_file_name,
-                        "--public-key",
-                        public_file_name,
-                        "--url",
-                        depl.instance.service_url,
-                        "--pcr0",
-                        depl.pcr_codes[0],
-                        "--pcr1",
-                        depl.pcr_codes[1],
-                        "--pcr2",
-                        depl.pcr_codes[2],
-                        "--port",
-                        "443",
-                        "--lport",
-                        str(connection_port),
-                    ],
-                    stdout=log_file,
-                    stderr=log_file,
-                )
-            with open(log_file_name) as log_file_read:
-                while True:
-                    log_line = log_file_read.readline()
-                    if "Error:  Invalid PCR Values" in log_line:
-                        raise Exception("PCR Validation Failed")
-                    if "Only one usage of each socket address" in log_line:
-                        raise Exception(
-                            "Another oblv proxy instance running. Either close that connection"
-                            + "or change the *connection_port*"
-                        )
-                    elif "error" in log_line.lower():
-                        raise Exception(log_line)
-                    elif "listening on" in log_line:
-                        break
-        except Exception as e:
-            raise e
-        else:
-            print(
-                f"Successfully connected to proxy on port {connection_port}. The logs can be found at {log_file_name}"
-            )
-        self.__conn_string = f"http://127.0.0.1:{connection_port}"
-        self.__logs = log_file_name
-        self.__process = process
-        return
+            user_update = UserUpdate(email=email)
+        except ValidationError:
+            return SyftError(message="{email} is not a valid email address.")
+
+        result = api.services.user.update(uid=self.id, user_update=user_update)
+
+        if isinstance(result, SyftError):
+            return result
+
+        self.email = email
+        return SyftSuccess(
+            message=f"Successfully updated email for the user "
+            f"'{self.name}' to '{self.email}'."
+        )
 
-    def register(
+    def update(
         self,
-        name: str,
-        email: str,
-        password: str,
-        institution: str | None = None,
-        website: str | None = None,
-    ) -> SyftError | SyftSigningKey | None:
-        self.check_connection_string()
-        guest_client = login_as_guest(url=self.__conn_string)
-        return guest_client.register(
+        name: type[Empty] | str = Empty,
+        institution: type[Empty] | str = Empty,
+        website: type[Empty] | str = Empty,
+        role: type[Empty] | str = Empty,
+        mock_execution_permission: type[Empty] | bool = Empty,
+    ) -> SyftSuccess | SyftError:
+        """Used to update name, institution, website of a user."""
+        api = APIRegistry.api_for(
+            node_uid=self.syft_node_location,
+            user_verify_key=self.syft_client_verify_key,
+        )
+        if api is None:
+            return SyftError(message=f"You must login to {self.node_uid}")
+        user_update = UserUpdate(
             name=name,
-            email=email,
-            password=password,
             institution=institution,
             website=website,
+            role=role,
+            mock_execution_permission=mock_execution_permission,
         )
+        result = api.services.user.update(uid=self.id, user_update=user_update)
 
-    def login(
-        self,
-        email: str,
-        password: str,
-    ) -> None:
-        self.check_connection_string()
-        self.__enclave_client = login(
-            url=self.__conn_string, email=email, password=password
-        )
+        if isinstance(result, SyftError):
+            return result
+
+        for attr, val in result.to_dict(exclude_empty=True).items():
+            setattr(self, attr, val)
+
+        return SyftSuccess(message="User details successfully updated.")
 
-    def check_connection_string(self) -> None:
-        if not self.__conn_string:
-            raise Exception(
-                "Either proxy not running or not initiated using syft."
-                + " Run the method initiate_connection to initiate the proxy connection"
-            )
-
-    def sanity_check_oblv_response(self, req: requests.Response) -> str:
-        if req.status_code == 401:
-            raise OblvUnAuthorizedError()
-        elif req.status_code == 400:
-            raise OblvEnclaveError(req.json()["detail"])
-        elif req.status_code == 422:
-            print(req.text)
-            # ToDo - Update here
-        elif req.status_code != 200:
-            raise OblvEnclaveError(
-                f"Failed to perform the operation  with status {req.status_code}, {req.content!r}"
-            )
-        return "Failed"
-
-    def request_code_execution(self, code: SubmitUserCode) -> Any:
-        # relative
-        from ...service.code.user_code import SubmitUserCode
-
-        if not isinstance(code, SubmitUserCode):
-            raise Exception(
-                f"The input code should be of type: {SubmitUserCode} got:{type(code)}"
-            )
+    def allow_mock_execution(self, allow: bool = True) -> SyftSuccess | SyftError:
+        return self.update(mock_execution_permission=allow)
 
-        enclave_metadata = OblvMetadata(
-            deployment_id=self.deployment_id, oblv_client=self.oblv_client
+
+@serializable()
+class UserViewPage(SyftObject):
+    __canonical_name__ = "UserViewPage"
+    __version__ = SYFT_OBJECT_VERSION_2
+
+    users: list[UserView]
+    total: int
+
+
+@transform(UserUpdate, User)
+def user_update_to_user() -> list[Callable]:
+    return [
+        validate_email,
+        hash_password,
+        drop(["password", "password_verify"]),
+    ]
+
+
+@transform(UserCreate, User)
+def user_create_to_user() -> list[Callable]:
+    return [
+        generate_id,
+        validate_email,
+        hash_password,
+        generate_key,
+        drop(["password", "password_verify", "created_by"]),
+        # TODO: Fix this by passing it from client & verifying it at server
+        default_role(ServiceRole.DATA_SCIENTIST),
+    ]
+
+
+@transform(User, UserView)
+def user_to_view_user() -> list[Callable]:
+    return [
+        keep(
+            [
+                "id",
+                "email",
+                "name",
+                "role",
+                "institution",
+                "website",
+                "mock_execution_permission",
+                "notifications_enabled",
+            ]
         )
+    ]
 
-        code_id = UID()
-        code.id = code_id
-        code.enclave_metadata = enclave_metadata
-
-        for domain_client in self.domain_clients:
-            domain_client.code.request_code_execution(code=code)
-            print(f"Sent code execution request to {domain_client.name}")
-
-        res = self.api.services.code.request_code_execution(code=code)
-        print(f"Execution will be done on {self.__enclave_client.name}")
-
-        return res
-
-    @property
-    def api(self) -> SyftAPI:
-        if not self.__enclave_client:
-            raise Exception("Kindly login or register with the enclave")
-
-        return self.__enclave_client.api
-
-    def close_connection(self) -> str | None:
-        if self.check_proxy_running():
-            os.kill(self.__process.pid, SIGTERM)
-            return None
-        else:
-            return "No Proxy Connection Running"
-
-    def check_proxy_running(self) -> bool:
-        if self.__process is not None:
-            if self.__process.poll() is not None:
-                return False
-            else:
-                return True
-        return False
-
-    def fetch_current_proxy_logs(
-        self, follow: bool = False, tail: bool = False
-    ) -> None:
-        """Returns the logs of the running enclave instance
-
-        Args:
-            follow (bool, optional): To follow the logs as they grow. Defaults to False.
-            tail (bool, optional): Only show the new generated logs.
-                To be used only when follow is True. Defaults to False.
-        """
-        if self.__logs is None:
-            print(
-                bcolors.RED
-                + bcolors.BOLD
-                + "Exception"
-                + bcolors.BLACK
-                + bcolors.ENDC
-                + ": Logs not initiated",
-                file=sys.stderr,
-            )
-        log_file = open(self.__logs)
-        if not follow:
-            print(log_file.read())
-        else:
-            if tail:
-                log_file.seek(0, 2)
-            while True:
-                line = log_file.readline()
-                if not line:
-                    time.sleep(0.1)
-                    continue
-                print(line)
+
+@serializable()
+class UserPrivateKey(SyftObject):
+    __canonical_name__ = "UserPrivateKey"
+    __version__ = SYFT_OBJECT_VERSION_2
+
+    email: str
+    signing_key: SyftSigningKey
+    role: ServiceRole
 
 
-# Todo - Method to check if proxy is running
-# Todo
+@transform(User, UserPrivateKey)
+def user_to_user_verify() -> list[Callable]:
+    return [keep(["email", "signing_key", "id", "role"])]
```

### Comparing `syft-0.8.6b1/src/syft/external/oblv/oblv_keys_stash.py` & `syft-0.8.7b1/src/syft/service/notifier/notifier_stash.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,68 +1,83 @@
 # stdlib
-from typing import Any
 
 # third party
 from result import Err
 from result import Ok
 from result import Result
 
 # relative
 from ...node.credentials import SyftVerifyKey
 from ...serde.serializable import serializable
-from ...service.response import SyftError
 from ...store.document_store import BaseStash
 from ...store.document_store import DocumentStore
+from ...store.document_store import PartitionKey
 from ...store.document_store import PartitionSettings
-from ...store.document_store import QueryKeys
-from ...store.document_store import UIDPartitionKey
 from ...types.uid import UID
-from .oblv_keys import OblvKeys
+from ...util.telemetry import instrument
+from ..action.action_permissions import ActionObjectPermission
+from .notifier import NotifierSettings
 
+NamePartitionKey = PartitionKey(key="name", type_=str)
+ActionIDsPartitionKey = PartitionKey(key="action_ids", type_=list[UID])
 
+
+@instrument
 @serializable()
-class OblvKeysStash(BaseStash):
-    object_type = OblvKeys
+class NotifierStash(BaseStash):
+    object_type = NotifierSettings
     settings: PartitionSettings = PartitionSettings(
-        name=OblvKeys.__canonical_name__, object_type=OblvKeys, db_name="app"
+        name=NotifierSettings.__canonical_name__, object_type=NotifierSettings
     )
 
     def __init__(self, store: DocumentStore) -> None:
         super().__init__(store=store)
 
-    def check_type(self, obj: Any, type_: type) -> Result[Any, str]:
-        return (
-            Ok(obj)
-            if isinstance(obj, type_)
-            else Err(f"{type(obj)} does not match required type: {type_}")
-        )
-
-    def set(
-        self, credentials: SyftVerifyKey, oblv_keys: OblvKeys
-    ) -> Result[OblvKeys, Err]:
-        if not len(self):
-            valid = self.check_type(oblv_keys, self.object_type)
-            if valid.is_err():
-                return SyftError(message=valid.err())
+    def admin_verify_key(self) -> SyftVerifyKey:
+        return self.partition.root_verify_key
 
-            return super().set(credentials, oblv_keys)
+    # TODO: should this method behave like a singleton?
+    def get(self, credentials: SyftVerifyKey) -> Result[NotifierSettings, Err]:
+        """Get Settings"""
+        result = self.get_all(credentials)
+        if result.is_ok():
+            settings = result.ok()
+            if len(settings) == 0:
+                return Ok(
+                    None
+                )  # TODO: Stash shouldn't be empty after init. Return Err instead?
+            result = settings[
+                0
+            ]  # TODO: Should we check if theres more than one? => Report corruption
+            return Ok(result)
         else:
-            return Err("Domain Node already has an existing public/private key pair")
+            return Err(message=result.err())
 
-    def get_by_uid(
-        self, credentials: SyftVerifyKey, uid: UID
-    ) -> Result[OblvKeys | None, str]:
-        qks = QueryKeys(qks=[UIDPartitionKey.with_obj(uid)])
-        return Ok(self.query_one(credentials=credentials, qks=qks))
-
-    def delete_by_uid(self, credentials: SyftVerifyKey, uid: UID) -> Result[bool, str]:
-        qk = UIDPartitionKey.with_obj(uid)
-        return super().delete(qk=qk)
+    def set(
+        self,
+        credentials: SyftVerifyKey,
+        settings: NotifierSettings,
+        add_permissions: list[ActionObjectPermission] | None = None,
+        add_storage_permission: bool = True,
+        ignore_duplicates: bool = False,
+    ) -> Result[NotifierSettings, Err]:
+        result = self.check_type(settings, self.object_type)
+        # we dont use and_then logic here as it is hard because of the order of the arguments
+        if result.is_err():
+            return Err(message=result.err())
+        return super().set(
+            credentials=credentials, obj=result.ok()
+        )  # TODO check if result isInstance(Ok)
 
     def update(
-        self, credentials: SyftVerifyKey, task: OblvKeys
-    ) -> Result[OblvKeys, str]:
-        valid = self.check_type(task, self.object_type)
-        if valid.is_err():
-            return SyftError(message=valid.err())
-
-        return super().update(credentials, task)
+        self,
+        credentials: SyftVerifyKey,
+        settings: NotifierSettings,
+        has_permission: bool = False,
+    ) -> Result[NotifierSettings, Err]:
+        result = self.check_type(settings, self.object_type)
+        # we dont use and_then logic here as it is hard because of the order of the arguments
+        if result.is_err():
+            return Err(message=result.err())
+        return super().update(
+            credentials=credentials, obj=result.ok()
+        )  # TODO check if result isInstance(Ok)
```

### Comparing `syft-0.8.6b1/src/syft/gevent_patch.py` & `syft-0.8.7b1/src/syft/gevent_patch.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6b1/src/syft/img/logo.png` & `syft-0.8.7b1/src/syft/img/logo.png`

 * *Files identical despite different names*

### Comparing `syft-0.8.6b1/src/syft/img/small-grid-symbol-logo.png` & `syft-0.8.7b1/src/syft/img/small-grid-symbol-logo.png`

 * *Files identical despite different names*

### Comparing `syft-0.8.6b1/src/syft/node/credentials.py` & `syft-0.8.7b1/src/syft/node/credentials.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6b1/src/syft/node/node.py` & `syft-0.8.7b1/src/syft/node/node.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,24 +30,24 @@
 from ..client.api import SignedSyftAPICall
 from ..client.api import SyftAPI
 from ..client.api import SyftAPICall
 from ..client.api import SyftAPIData
 from ..client.api import debox_signed_syftapicall_response
 from ..client.client import SyftClient
 from ..exceptions.exception import PySyftException
-from ..external import OblvServiceProvider
 from ..protocol.data_protocol import PROTOCOL_TYPE
 from ..protocol.data_protocol import get_data_protocol
 from ..service.action.action_object import Action
 from ..service.action.action_object import ActionObject
 from ..service.action.action_service import ActionService
 from ..service.action.action_store import ActionStore
 from ..service.action.action_store import DictActionStore
 from ..service.action.action_store import MongoActionStore
 from ..service.action.action_store import SQLiteActionStore
+from ..service.api.api_service import APIService
 from ..service.blob_storage.service import BlobStorageService
 from ..service.code.status_service import UserCodeStatusService
 from ..service.code.user_code_service import UserCodeService
 from ..service.code.user_code_stash import UserCodeStash
 from ..service.code_history.code_history_service import CodeHistoryService
 from ..service.context import AuthedServiceContext
 from ..service.context import NodeServiceContext
@@ -117,14 +117,15 @@
 from ..store.sqlite_document_store import SQLiteStoreClientConfig
 from ..store.sqlite_document_store import SQLiteStoreConfig
 from ..types.syft_object import SYFT_OBJECT_VERSION_2
 from ..types.syft_object import SyftObject
 from ..types.uid import UID
 from ..util.experimental_flags import flags
 from ..util.telemetry import instrument
+from ..util.util import get_dev_mode
 from ..util.util import get_env
 from ..util.util import get_queue_address
 from ..util.util import random_name
 from ..util.util import str_to_bool
 from ..util.util import thread_ident
 from .credentials import SyftSigningKey
 from .credentials import SyftVerifyKey
@@ -174,18 +175,14 @@
     return get_env(DEFAULT_ROOT_USERNAME, "Jane Doe")
 
 
 def get_default_root_password() -> str | None:
     return get_env(DEFAULT_ROOT_PASSWORD, "changethis")  # nosec
 
 
-def get_dev_mode() -> bool:
-    return str_to_bool(get_env("DEV_MODE", "False"))
-
-
 def get_enable_warnings() -> bool:
     return str_to_bool(get_env("ENABLE_WARNINGS", "False"))
 
 
 def get_container_host() -> str | None:
     return get_env("CONTAINER_HOST")
 
@@ -855,14 +852,15 @@
             {"svc": SettingsService},
             {"svc": DatasetService},
             {"svc": UserCodeService},
             {"svc": LogService},
             {"svc": RequestService},
             {"svc": QueueService},
             {"svc": JobService},
+            {"svc": APIService},
             {"svc": DataSubjectService},
             {"svc": NetworkService},
             {"svc": PolicyService},
             {"svc": NotifierService},
             {"svc": NotificationService},
             {"svc": DataSubjectMemberService},
             {"svc": ProjectService},
@@ -874,15 +872,14 @@
             {"svc": SyftWorkerImageService},
             {"svc": SyftWorkerPoolService},
             {"svc": SyftImageRegistryService},
             {"svc": SyncService},
             {"svc": OutputService},
             {"svc": UserCodeStatusService},
             {"svc": VeilidServiceProvider},  # this is lazy
-            {"svc": OblvServiceProvider},  # this is lazy
         ]
 
         for svc_kwargs in default_services:
             ServiceCls = svc_kwargs.pop("svc")
             svc_kwargs.setdefault("store", self.document_store)
 
             svc_instance = ServiceCls(**svc_kwargs)
@@ -1280,15 +1277,15 @@
 
         # 🟡 TODO 36: Needs distributed lock
         self.queue_stash.set_placeholder(credentials, queue_item)
         self.job_stash.set(credentials, job)
 
         log_service = self.get_service("logservice")
 
-        result = log_service.add(context, log_id)
+        result = log_service.add(context, log_id, queue_item.job_id)
         if isinstance(result, SyftError):
             return result
         return job
 
     def _get_existing_user_code_jobs(
         self, context: AuthedServiceContext, user_code_id: UID
     ) -> list[Job] | SyftError:
@@ -1423,16 +1420,14 @@
 
     def get_unauthed_context(
         self, login_credentials: UserLoginCredentials
     ) -> NodeServiceContext:
         return UnauthedServiceContext(node=self, login_credentials=login_credentials)
 
     def create_initial_settings(self, admin_email: str) -> NodeSettingsV2 | None:
-        if self.name is None:
-            self.name = random_name()
         try:
             settings_stash = SettingsStash(store=self.document_store)
             if self.signing_key is None:
                 print("create_initial_settings failed as there is no signing key")
                 return None
             settings_exists = settings_stash.get_all(self.signing_key.verify_key).ok()
             if settings_exists:
@@ -1502,41 +1497,14 @@
                 raise Exception(f"Could not create user: {result}")
     except Exception as e:
         print("Unable to create new admin", e)
 
     return None
 
 
-# def create_oblv_key_pair(
-#     worker: Node,
-# ) -> str | None:
-#     try:
-#         # relative
-#         from ..external.oblv.oblv_keys_stash import OblvKeys
-#         from ..external.oblv.oblv_keys_stash import OblvKeysStash
-#         from ..external.oblv.oblv_service import generate_oblv_key
-
-#         oblv_keys_stash = OblvKeysStash(store=worker.document_store)
-
-#         if not len(oblv_keys_stash) and worker.signing_key:
-#             public_key, private_key = generate_oblv_key(oblv_key_name=worker.name)
-#             oblv_keys = OblvKeys(public_key=public_key, private_key=private_key)
-#             res = oblv_keys_stash.set(worker.signing_key.verify_key, oblv_keys)
-#             if res.is_ok():
-#                 print("Successfully generated Oblv Key pair at startup")
-#             return res.err()
-#         else:
-#             print(f"Using Existing Public/Private Key pair: {len(oblv_keys_stash)}")
-#     except Exception as e:
-#         print("Unable to create Oblv Keys.", e)
-#         return None
-
-#     return None
-
-
 class NodeRegistry:
     __node_registry__: dict[UID, Node] = {}
 
     @classmethod
     def set_node_for(
         cls,
         node_uid: UID | str,
```

### Comparing `syft-0.8.6b1/src/syft/node/routes.py` & `syft-0.8.7b1/src/syft/node/routes.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6b1/src/syft/node/run.py` & `syft-0.8.7b1/src/syft/node/run.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6b1/src/syft/node/server.py` & `syft-0.8.7b1/src/syft/node/server.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6b1/src/syft/node/worker_settings.py` & `syft-0.8.7b1/src/syft/node/worker_settings.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6b1/src/syft/protocol/data_protocol.py` & `syft-0.8.7b1/src/syft/protocol/data_protocol.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,29 +5,33 @@
 from collections.abc import MutableSequence
 import hashlib
 import json
 from operator import itemgetter
 import os
 from pathlib import Path
 import re
+from types import UnionType
+import typing
 from typing import Any
+import warnings
 
 # third party
 from packaging.version import parse
 from result import OkErr
 from result import Result
 
 # relative
 from .. import __version__
 from ..serde.recursive import TYPE_BANK
 from ..service.response import SyftError
 from ..service.response import SyftException
 from ..service.response import SyftSuccess
 from ..types.dicttuple import DictTuple
 from ..types.syft_object import SyftBaseObject
+from ..util.util import get_dev_mode
 
 PROTOCOL_STATE_FILENAME = "protocol_version.json"
 PROTOCOL_TYPE = str | int
 
 
 def natural_key(key: PROTOCOL_TYPE) -> list[int | str | Any]:
     """Define key for natural ordering of strings."""
@@ -49,30 +53,61 @@
     return Path(os.path.abspath(str(Path(__file__).parent)))
 
 
 def protocol_release_dir() -> Path:
     return data_protocol_dir() / "releases"
 
 
+def handle_union_type_klass_name(type_klass_name: str) -> str:
+    if type_klass_name == typing.Union.__name__:
+        return UnionType.__name__
+    return type_klass_name
+
+
+def handle_annotation_repr_(annotation: type) -> str:
+    """Handle typing representation."""
+    origin = typing.get_origin(annotation)
+    args = typing.get_args(annotation)
+    if origin and args:
+        args_repr = ", ".join(getattr(arg, "__name__", str(arg)) for arg in args)
+        origin_repr = getattr(origin, "__name__", str(origin))
+
+        # Handle typing.Union and types.UnionType
+        origin_repr = handle_union_type_klass_name(origin_repr)
+        return f"{origin_repr}: [{args_repr}]"
+    elif args:
+        args_repr = ", ".join(
+            getattr(arg, "__name__", str(arg)) for arg in sorted(args)
+        )
+        return args_repr
+    else:
+        return repr(annotation)
+
+
 class DataProtocol:
-    def __init__(self, filename: str) -> None:
+    def __init__(self, filename: str, raise_exception: bool = False) -> None:
         self.file_path = data_protocol_dir() / filename
+        self.raise_exception = raise_exception
         self.load_state()
 
     def load_state(self) -> None:
         self.protocol_history = self.read_history()
         self.state = self.build_state()
         self.diff, self.current = self.diff_state(self.state)
         self.protocol_support = self.calculate_supported_protocols()
 
     @staticmethod
     def _calculate_object_hash(klass: type[SyftBaseObject]) -> str:
         # TODO: this depends on what is marked as serde
+
+        # Rebuild the model to ensure that the fields are up to date
+        # and any ForwardRef are resolved
+        klass.model_rebuild()
         field_data = {
-            field: repr(field_info.annotation)
+            field: handle_annotation_repr_(field_info.rebuild_annotation())
             for field, field_info in sorted(
                 klass.model_fields.items(), key=itemgetter(0)
             )
         }
         obj_meta_info = {
             "canonical_name": klass.__canonical_name__,
             "version": klass.__version__,
@@ -207,22 +242,29 @@
                         object_diff[canonical_name][str(version)]["version"] = int(
                             version
                         )
                         object_diff[canonical_name][str(version)]["hash"] = hash_str
                         object_diff[canonical_name][str(version)]["action"] = "add"
                         continue
 
-                    raise Exception(
+                    error_msg = (
                         f"{canonical_name} for class {cls.__name__} fqn {cls} "
                         + f"version {version} hash has changed. "
                         + f"{hash_str} not in {versions.values()}. "
                         + "Is a unique __canonical_name__ for this subclass missing? "
                         + "If the class has changed you will need to define a new class with the changes, "
                         + "with same __canonical_name__ and bump the __version__ number."
+                        + f"{cls.model_fields}"
                     )
+
+                    if get_dev_mode() or self.raise_exception:
+                        raise Exception(error_msg)
+                    else:
+                        warnings.warn(error_msg, stacklevel=1, category=UserWarning)
+                        break
                 else:
                     # new object so its an add
                     object_diff[canonical_name][str(version)] = {}
                     object_diff[canonical_name][str(version)]["version"] = int(version)
                     object_diff[canonical_name][str(version)]["hash"] = hash_str
                     object_diff[canonical_name][str(version)]["action"] = "add"
                     continue
@@ -412,14 +454,15 @@
 
         # Delete the current released protocol
         protocol_history.pop(latest_protocol)
         protocol_file_path.unlink()
 
         # Save history
         self.save_history(protocol_history)
+        self.load_state()
 
     def check_protocol(self) -> Result[SyftSuccess, SyftError]:
         if len(self.diff) != 0:
             return SyftError(message="Protocol Changes Unstaged")
         else:
             return SyftSuccess(message="Protocol Stable")
 
@@ -458,26 +501,34 @@
 
     @property
     def has_dev(self) -> bool:
         if "dev" in self.protocol_history.keys():
             return True
         return False
 
+    def reset_dev_protocol(self) -> None:
+        if self.has_dev:
+            del self.protocol_history["dev"]
+            self.save_history(self.protocol_history)
+
 
-def get_data_protocol() -> DataProtocol:
-    return DataProtocol(filename=data_protocol_file_name())
+def get_data_protocol(raise_exception: bool = False) -> DataProtocol:
+    return DataProtocol(
+        filename=data_protocol_file_name(),
+        raise_exception=raise_exception,
+    )
 
 
 def stage_protocol_changes() -> Result[SyftSuccess, SyftError]:
-    data_protocol = get_data_protocol()
+    data_protocol = get_data_protocol(raise_exception=True)
     return data_protocol.stage_protocol_changes()
 
 
 def bump_protocol_version() -> Result[SyftSuccess, SyftError]:
-    data_protocol = get_data_protocol()
+    data_protocol = get_data_protocol(raise_exception=True)
     return data_protocol.bump_protocol_version()
 
 
 def check_or_stage_protocol() -> Result[SyftSuccess, SyftError]:
     data_protocol = get_data_protocol()
     return data_protocol.check_or_stage_protocol()
```

### Comparing `syft-0.8.6b1/src/syft/protocol/releases/0.8.2.json` & `syft-0.8.7b1/src/syft/protocol/releases/0.8.2.json`

 * *Files identical despite different names*

### Comparing `syft-0.8.6b1/src/syft/protocol/releases/0.8.3.json` & `syft-0.8.7b1/src/syft/protocol/releases/0.8.3.json`

 * *Files identical despite different names*

### Comparing `syft-0.8.6b1/src/syft/protocol/releases/0.8.4.json` & `syft-0.8.7b1/src/syft/protocol/releases/0.8.4.json`

 * *Files identical despite different names*

### Comparing `syft-0.8.6b1/src/syft/protocol/releases/0.8.5.json` & `syft-0.8.7b1/src/syft/protocol/releases/0.8.6.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9948050213675219%*

 * *Differences: {"'4'": "{'object_versions': {'ActionObject': {'3': {'hash': "*

 * *        "'d5303167b1048c1b956781c6daeaa93ec792bea5181c076c93da74dfec0a6127'}}, 'AnyActionObject': "*

 * *        "{'3': {'hash': '22568b8c3d700b7eaa3291b9f3d014dda3d6dbe20f1f8eab87210ccb2f035bbc'}}, "*

 * *        "'BlobFileOBject': {'2': {'hash': "*

 * *        "'f8d75c274f7ae4138e85bb936c3f27241cc0f7dd011ba237396733c53e5a1b0d'}}, 'JobInfo': {'2': "*

 * *        "{'hash': '89dbd4a810586b49498be1f5299b565a19871487e14a120433b0a4cf607b6dee'}}, "*

 * *        "'ExecutionOu […]*

```diff
@@ -5,15 +5,15 @@
                 "1": {
                     "action": "remove",
                     "hash": "c0e83867b107113e6fed06364ba364c24b2f4af35b15a3869b176318d3be7989",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "1264dca857f7d5c8d1aa92791726a2e17567aba82538b64d357b988d1ae3a8c9",
+                    "hash": "1be1f6793478cd2e4a0cc84713426b2d5586969e98058f4e8b91fc19293cf445",
                     "version": 2
                 }
             },
             "Action": {
                 "1": {
                     "action": "remove",
                     "hash": "5cf71ee35097f17fbb1dd05096f875211d71cf07161205d7f6a9c11fd49d5272",
@@ -22,39 +22,39 @@
                 "2": {
                     "action": "remove",
                     "hash": "a13b50c4d23bd6deb7896e394f2a20e6cef4c33c5e6f4ee30f19eaffab708f21",
                     "version": 2
                 },
                 "3": {
                     "action": "add",
-                    "hash": "18525c0610aea0aa62fe496a739b0ca7fb828617b4fca73840807d3c7b1477a7",
+                    "hash": "8b9957c26b2fa6513d6a07cdde6a4fab003693cf4b787e8bda0ecc2503ae9d54",
                     "version": 3
                 }
             },
             "ActionDataEmpty": {
                 "1": {
                     "action": "remove",
                     "hash": "89b5912fe5416f922051b8068be6071a03c87a4ab264959de524f1b86e95f028",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "2bea14a344a82a10725a9e933bb1838ffbe2d28771ee4f54f40b4d5663840a7c",
+                    "hash": "1fd3a1d3b3d97c8fe4ff2e51567c026830e6c1489f82caa4c6e3ca24a11e1da0",
                     "version": 2
                 }
             },
             "ActionDataLink": {
                 "1": {
                     "action": "remove",
                     "hash": "10bf94e99637695f1ba283f0b10e70743a4ebcb9ee75aefb1a05e6d6e1d21a71",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "4551f22ea68af0d0943f9aa239b4fd468cf9f4da43589b536651fc3d27d99f12",
+                    "hash": "59756e8b5729df61217f8bcf53f54e99c7fcc715594488779e19296dec582951",
                     "version": 2
                 }
             },
             "ActionObject": {
                 "1": {
                     "action": "remove",
                     "hash": "632446f1415102490c93fafb56dd9eb29d79623bcc5e9f2e6e37c4f63c2c51c3",
@@ -63,15 +63,15 @@
                 "2": {
                     "action": "remove",
                     "hash": "577aa1f010b90194958a18ec38ee21db3718bd96d9e036501c6ddeefabedf432",
                     "version": 2
                 },
                 "3": {
                     "action": "add",
-                    "hash": "37bb8f0f87b1da2525da8f6873e6257dff4a732f2dba293b62931ad0b85ef9e2",
+                    "hash": "d5303167b1048c1b956781c6daeaa93ec792bea5181c076c93da74dfec0a6127",
                     "version": 3
                 }
             },
             "ActionQueueItem": {
                 "1": {
                     "action": "remove",
                     "hash": "11a43caf9164eb2a5a21f4bcb0ca361d0a5d134bf3c60173f2c502d0d80219de",
@@ -80,39 +80,39 @@
                 "2": {
                     "action": "remove",
                     "hash": "6413ed01e949cac169299a43ce40651f9bf8053e408b6942853f8afa8a693b3d",
                     "version": 2
                 },
                 "3": {
                     "action": "add",
-                    "hash": "4159d6ea45bc82577828bc19d668196422ff29bb8cc298b84623e6f4f476aaf3",
+                    "hash": "5bcda9c7df78ded9ea4b53710191f37054d3046ea01125b755afc8c30dd9eed2",
                     "version": 3
                 }
             },
             "ActionStoreChange": {
                 "1": {
                     "action": "remove",
                     "hash": "17b865e75eb3fb2693924fb00ba87a25260be45d55a4eb2184c4ead22d787cbe",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "3a1c8f10afb4c4d10a4096a1371e4780b2cb40bb2253193bfced6c250d3e8547",
+                    "hash": "0d97c83b6a355eaa6c351cd50c36ba58c0f0e08e63e16af1c44cba76c61af834",
                     "version": 2
                 }
             },
             "AnswerProjectPoll": {
                 "1": {
                     "action": "remove",
                     "hash": "ff2e1ac7bb764c99d646b96eb3ebfbf9311599b7e3be07aa4a4eb4810bb6dd12",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "fff1a7e5ca30b76132cf8b6225cb576467d9727349b9dc54d4131fede03c10f3",
+                    "hash": "7467766e01c8afadb1b2dbe548c9f540a7d6869fed4e98db96c2705bb6f3f3c2",
                     "version": 2
                 }
             },
             "AnyActionObject": {
                 "1": {
                     "action": "remove",
                     "hash": "bcb31f847907edc9c95d2d120dc5427854604f40940e3f41cd0474a1820ac65e",
@@ -121,75 +121,75 @@
                 "2": {
                     "action": "remove",
                     "hash": "002d8be821140befebbc0503e6bc1ef8779094e24e46305e5da5af6eecb56b13",
                     "version": 2
                 },
                 "3": {
                     "action": "add",
-                    "hash": "7c55461e3c6ba36ff999c64eb1b97a65b5a1f27193a973b1355ee2675f14c313",
+                    "hash": "22568b8c3d700b7eaa3291b9f3d014dda3d6dbe20f1f8eab87210ccb2f035bbc",
                     "version": 3
                 }
             },
             "Asset": {
                 "1": {
                     "action": "remove",
                     "hash": "24350b8d9597df49999918ad42e0eece1328ea30389311f1e0a420be8f39b8a1",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "64661b3bc84a2df81ce631641a0fe3f0d969618b6855971f5e51e5770c278bba",
+                    "hash": "b5ce972e6b0341da041f457660eca873bd9bb4f93e73158767f951cb93b53d10",
                     "version": 2
                 }
             },
             "AzureRemoteConfig": {
                 "1": {
                     "action": "remove",
                     "hash": "c05c6caa27db4e385c642536d4b0ecabc0c71e91220d2e6ce21a2761ca68a673",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "2f820aa55e6476b455fec7774346a4c0dad212bde1400f1f53f42c8864b7ded4",
+                    "hash": "56ab4455e8182d3c300efb31ae019a2211ecb9e579ec1a41a087c98ee8e9f317",
                     "version": 2
                 }
             },
             "AzureSecureFilePathLocation": {
                 "1": {
                     "action": "remove",
                     "hash": "1bb15f3f9d7082779f1c9f58de94011487924cb8a8c9c2ec18fd7c161c27fd0e",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "29a0c01a59d8632037c6d18d6fce1512b651e1aa8493b302746ff294c7bd331d",
+                    "hash": "b05c5b759d43d9aa13e2a11087d13ff78cbec946768e3ff130fcac83a4216117",
                     "version": 2
                 }
             },
             "BaseConfig": {
                 "1": {
                     "action": "remove",
                     "hash": "4e5257080ce615aa4122b02bad8487e4c7d6d0f171ff77abbc9e8cd3e33df89a",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "45e4480e6fbb5183e36cbe3bd18e21d65c43cc5809028a13ab49270e0a565da6",
+                    "hash": "383d9ce8873520c9224e00797a96d6dc2e64f054795e3b1de2ac7cd8ce68df86",
                     "version": 2
                 }
             },
             "BlobDeposit": {
                 "1": {
                     "action": "remove",
                     "hash": "c98e6da658a3be01ead4ea6ee6a4c10046879f0ce0f5fc5f946346671579b229",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "87dd601b58f31ccf8e3001e8723d8d251f84bd7ab9a2f87ff7c6cf05b074d41f",
+                    "hash": "7b0709298f6a6bd1e33244f655dc4f3bb95645f9e474f2de331869071e3ab384",
                     "version": 2
                 }
             },
             "BlobFile": {
                 "1": {
                     "action": "remove",
                     "hash": "47ed55183d619c6c624e35412360a41de42833e2c24223c1de1ad12a84fdafc2",
@@ -198,27 +198,27 @@
                 "3": {
                     "action": "remove",
                     "hash": "8f1710c754bb3b39f546b97fd69c4826291398b247976bbc41fa873af431bca9",
                     "version": 3
                 },
                 "4": {
                     "action": "add",
-                    "hash": "05ef86582c6b8967499eb0f57d048676e15390ce74891409fada522226563754",
+                    "hash": "c74d6f9899d928430a38bd4585069b557de8e985a13f82f166479bd7f32d5a85",
                     "version": 4
                 }
             },
             "BlobFileOBject": {
                 "1": {
                     "action": "remove",
                     "hash": "8da2c80ced4f0414c671313c4b63d05846df1e397c763d99d803be86c29755bb",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "1ab941c7669572a41067a17e0e3f2d9c7056f7a4df8f899e87ae2358d9113b02",
+                    "hash": "f8d75c274f7ae4138e85bb936c3f27241cc0f7dd011ba237396733c53e5a1b0d",
                     "version": 2
                 }
             },
             "BlobRetrieval": {
                 "1": {
                     "action": "remove",
                     "hash": "a8d7e1d6483e7a9b5a130e837fa398862aa6cbb316cc5f4470450d835755fdd9",
@@ -227,27 +227,27 @@
                 "2": {
                     "action": "remove",
                     "hash": "4c4fbdb6df5bb9fcbe914a9890bd1c1b6a1b3f382a04cbc8752a5a1b03130111",
                     "version": 2
                 },
                 "3": {
                     "action": "add",
-                    "hash": "ab0f1f06c57b3cd8bd362514d662b170a888a2487dbb1e9f880f611ce47a2b2c",
+                    "hash": "609daef405c4606f61b76df23c91ae75a97788a4e99f3e1ee7faa5a35eab8748",
                     "version": 3
                 }
             },
             "BlobRetrievalByURL": {
                 "3": {
                     "action": "remove",
                     "hash": "0b664100ea08413ca4ef04665ca910c2cf9535539617ea4ba33687d05cdfe747",
                     "version": 3
                 },
                 "4": {
                     "action": "add",
-                    "hash": "3fadedaf8e4ba97db9d4ddf1cf954338113cbb88d016253c008b11f0dfe19c59",
+                    "hash": "3a82ec6220eda51289931689db2f598e5e44a610b0a229113c4695f897cc9f2b",
                     "version": 4
                 }
             },
             "BlobStorageEntry": {
                 "1": {
                     "action": "remove",
                     "hash": "9f1b027cce390ee6f71c7a81e7420bb71a477b29c6c62ba74e781a97bc5434e6",
@@ -256,15 +256,15 @@
                 "2": {
                     "action": "remove",
                     "hash": "5472bdd5bdce6d0b561543a6bac70d47bf0c05c141a21450751460cc538d6b55",
                     "version": 2
                 },
                 "3": {
                     "action": "add",
-                    "hash": "136b0fb4908eb0c065a7ba6644ff5377a3c22ce8d97b3e48de1eb241101d4806",
+                    "hash": "0a5cf4058b330727a2d617a99d56070a7a6977b7d10f532fbb35cd4fe97b7678",
                     "version": 3
                 }
             },
             "BlobStorageMetadata": {
                 "1": {
                     "action": "remove",
                     "hash": "6888943be3f97186190dd26d7eefbdf29b15c6f2fa459e13608065ebcdb799e2",
@@ -273,322 +273,322 @@
                 "2": {
                     "action": "remove",
                     "hash": "674f4c52a8444289d5ef389b919008860e2b0e7acbaafa774d58e492d5b6741a",
                     "version": 2
                 },
                 "3": {
                     "action": "add",
-                    "hash": "643065504ecfabd283c736c794cfb41fb85156879940488d6ea851bb2ac3c16a",
+                    "hash": "b4b222dc8a994b5ff6d685818973516d89b615e2321d122edc28d1c30479a9fb",
                     "version": 3
                 }
             },
             "Change": {
                 "1": {
                     "action": "remove",
                     "hash": "aefebd1601cf5bfd4817b0db75300a78299cc4949ead735a90873cbd22c8d4bc",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "b661753ae9187feb92751edb4a38066c9c14aba73e3639d44ac5fe7aee8b2ab9",
+                    "hash": "9784905430b48d60be31b89d5fdbf559f8f7cc0a3be3428a3ba4b17b0db06330",
                     "version": 2
                 }
             },
             "ChangeStatus": {
                 "1": {
                     "action": "remove",
                     "hash": "627f6f8e42cc285336aa6fd4916285d796140f4ff901487b7cb3907ef0f116a6",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "8a62d5bcde312e7b9efd1d0b26cab6de7affa1e3ffe9182f8598137340408084",
+                    "hash": "37e33e685081a3e45155ffe8f02371a5dde82841ebb3d1b60c0ff06031622ccd",
                     "version": 2
                 }
             },
             "CodeHistoriesDict": {
                 "1": {
                     "action": "remove",
                     "hash": "95288411cd5843834f3273a2fd66a7df2e603e980f4ab1d329f9ab17d5d2f643",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "36175742343fdb2c9ea54809c08857cf1f30451245ebdca45b13020f6c7c0e2e",
+                    "hash": "9ebf38ad3f12b1ec397bd977cf1013fb8703e02562a6e74b7d17ea2debfcb4a1",
                     "version": 2
                 }
             },
             "CodeHistory": {
                 "1": {
                     "action": "remove",
                     "hash": "a7baae93862ae0aa67675f1617574e31aafb15a9ebff633eb817278a3a867161",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "54793b2909c70303c58fb720e431752547e29e56a616e544b6a103b2bfd2f73b",
+                    "hash": "f9a3e33bb89c72612b2c5ea501ca16bdbac832a94af1f373c76458f2a5a96614",
                     "version": 2
                 }
             },
             "CodeHistoryView": {
                 "1": {
                     "action": "remove",
                     "hash": "0ed1a2a04a962ecbcfa38b0b8a03c1e51e8946a4b80f6bf2557148ce658671ce",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "3d5f79f8367c229f163ab746ef8c7069bec5a1478a19812dbac735fc333e41c3",
+                    "hash": "91f1c8b4d9f8e8be517cda487615ae2e3a9df6fd4bdd2c7be51836b851f429f0",
                     "version": 2
                 }
             },
             "Contributor": {
                 "1": {
                     "action": "remove",
                     "hash": "d1d4f25bb87e59c0414501d3335097de66815c164c9ed5a7850ff8bec69fbcdc",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "55259f1e4f1b9da4ac83b032adb86eb4a1322a06584790d1300131777212dbaa",
+                    "hash": "7beef331ac6ea90632adc81a96bd99a656467ab8f2334007c624c64ea8a4b886",
                     "version": 2
                 }
             },
             "CreateAsset": {
                 "1": {
                     "action": "remove",
                     "hash": "1b4c71569b8da64258672483bd36dc4aa99a32d4cb519659241d15bc898041a6",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "93c75b45b9b74c69243cc2f2ef2d661e11eef5c23ecf71692ffdbd467d11efe6",
+                    "hash": "954da64a48165139f585e9e5a9526aa43a73a0709c1c1bf58e937e8c3e0f184f",
                     "version": 2
                 }
             },
             "CreateBlobStorageEntry": {
                 "1": {
                     "action": "remove",
                     "hash": "61a373336e83645f1b6d78a320323d9ea4ee91b3d87b730cb0608fbfa0072262",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "9046843fba39e5700aeb8c442a7e4ac5e772b12f6ac502367b2e5decbb26761f",
+                    "hash": "b252fe14bd22f92866c20bfffbdab1a839c8648c7b2cda81500cbeb9a5d85c57",
                     "version": 2
                 }
             },
             "CreateCustomImageChange": {
                 "1": {
                     "action": "remove",
                     "hash": "bc09dca7995938f3b3a2bd9c8b3c2feffc8484df466144a425cb69cadb2ab635",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "6569fb11bccd100cd4b6050084656e7e7c46b9405ff76589b870402b26a6927b",
+                    "hash": "91d2333291eb43c9814eb1d3ad1f736d5c1ccb9370de6734e506f0463fa92159",
                     "version": 2
                 }
             },
             "CreateCustomWorkerPoolChange": {
                 "1": {
                     "action": "remove",
                     "hash": "86894f8ccc037de61f44f9698fd113ba02c3cf3870a3048c00a46e15dcd1941c",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "e2a223a65461b502f097f06453f878b54175b4055dad3ec9b09c1eb9458a575e",
+                    "hash": "84cb18e884dfb1509d78d8775110314278444af2b2dd5370cb2621d28f8d1aaa",
                     "version": 2
                 }
             },
             "CreateDataset": {
                 "1": {
                     "action": "remove",
                     "hash": "3b020d9b8928cbd7e91f41c749ab4c932e19520696a183f2c7cd1312ebb640d1",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "83c6142c99da6667260e0d6df258b6e173beb18e399d60209b6ffccb5547f1e7",
+                    "hash": "67d45b8e93be3c95cdc5c5c2ff8d7e181e0c3200badc279d56be4f51f5e78ce7",
                     "version": 2
                 }
             },
             "CreateNotification": {
                 "1": {
                     "action": "remove",
                     "hash": "b1f459de374fe674f873a4a5f3fb8a8aabe0d83faad84a933f0a77dd1141159a",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "32d046bda4d978fb8e839e2c2c4994b86a60843311b74330e307e6e3e422176f",
+                    "hash": "657edc0de0b93399006f9c911de2cd212244acc192ff052abf7215bb41fe83aa",
                     "version": 2
                 }
             },
             "DataSubject": {
                 "1": {
                     "action": "remove",
                     "hash": "0b8b049d4627727b444c419f5d6a97b7cb97a433088ebf744c854b6a470dadf1",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "6d9d65d2723aed8cc4cfce9b5ee4a005ab84f8a24372dc47ce856cb6516835a9",
+                    "hash": "4385b12c582d711cfadf08f6d9254d2b95652d8aeedbeb350c5dcbf57dab1fea",
                     "version": 2
                 }
             },
             "DataSubjectCreate": {
                 "1": {
                     "action": "remove",
                     "hash": "5a94f9fcba75c50d78d71222f0235c5fd4d8003ae0db4d74bdbc4d56a99de3aa",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "b35897295822f061fbc70522ca8967cd2be53a5c01b19e24c587cd7b0c4aa3e8",
+                    "hash": "f33811ae53332a54323cd64772776d0fdf95623f5ee7e3f5759dd36ba9e0397d",
                     "version": 2
                 }
             },
             "DataSubjectMemberRelationship": {
                 "1": {
                     "action": "remove",
                     "hash": "0a820edc9f1a87387acc3c611fe852752fcb3dab7608058f2bc48211be7bfbd2",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "159d4e4f2463b213a65082b270acbb57ae84c5f0dbc897fda75486290b3148f1",
+                    "hash": "6f03ee3c35cd02973210c25ce99f50effdaa6156211329bddf763272d9d32585",
                     "version": 2
                 }
             },
             "Dataset": {
                 "1": {
                     "action": "remove",
                     "hash": "99ca2fa3e46fd9810222d269fac6accb546f632e94d5d57529016ba5e55af5a8",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "0bbae6e3665e61e97eeb328400efc678dfb26409616c66bf48f3f34bbf102721",
+                    "hash": "5e108228813bda478de1d6496fffc888f2f1bbaa7ae11ccce100987ee935c5ce",
                     "version": 2
                 }
             },
             "DatasetPageView": {
                 "1": {
                     "action": "remove",
                     "hash": "b1de14bb9b6a259648dfc59b6a48fa526116afe50a689c24b8bb36fd0e6a97f8",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "c7494afa0ae27326c4521a918eb234ba74eb2c0494ea448255ff310201a16c88",
+                    "hash": "f7652573278f762788f4ec3d39c3ec14179061429589714ff49210b015d57d0f",
                     "version": 2
                 }
             },
             "DateTime": {
                 "1": {
                     "action": "remove",
                     "hash": "7e9d89309a10d2110a7ae4f97d8f25a7914853269e8fa0c531630790c1253f17",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "c353b8edfa13250507942a3134f0ec9db8fb1d85f4f7a029fe4ad5665614bf5a",
+                    "hash": "92daa79cc211b880d7c492e32b22fa4b7cce78ef1606a9be4461324f68fb8cd3",
                     "version": 2
                 }
             },
             "DictStoreConfig": {
                 "1": {
                     "action": "remove",
                     "hash": "256e9c623ce0becd555ddd2a55a0c15514e162786b1549388cef98a92a9b18c9",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "6cef5c61f567c75c969827fabaf5bd4f4409a399f33b6b2623fbed3c7a597a41",
+                    "hash": "071e31e8bf4fdf894b03e0490549be4c40fcb0f0cdecff34866c5d2eded2944f",
                     "version": 2
                 }
             },
             "EnclaveMetadata": {
                 "1": {
                     "action": "remove",
                     "hash": "39f85e475015e6f860ddcc5fea819423eba2db8f4b7d8e004c05a44d6f8444c6",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "5103272305abd2bcf23c616bd9014be986a92c40dc37b6238680114036451852",
+                    "hash": "6dcc26695abc6a9ecd9d7d1e6507a9f1a92cc5ccd10987e92419bf984245f9a1",
                     "version": 2
                 }
             },
             "EnumMutation": {
                 "1": {
                     "action": "remove",
                     "hash": "4c02f956ec9b973064972cc57fc8dd9c525e683f93f804642b4e1bfee1b62e57",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "6d2e2f64c00dcda74a2545c77abbcf1630c56c26014987038feab174d15bd9d7",
+                    "hash": "13275f41942fa8eaa359fe3b0d5ba9f7c8c73564dad6d661441c29beef19a049",
                     "version": 2
                 }
             },
             "ExactMatch": {
                 "1": {
                     "action": "remove",
                     "hash": "e497e2e2380db72766c5e219e8afd13136d8953933d6f1eaf83b14001e887cde",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "f752dfdec6b30e1c849e483ac88ab6f0c71a286199415e4f7bc33c8c2502fc1f",
+                    "hash": "8767689e0b6acdc42ed558645ce641098e63094300225e2c8b9e4758abf80104",
                     "version": 2
                 }
             },
             "ExecutionOutput": {
                 "1": {
                     "action": "add",
-                    "hash": "201c8abcb6595a64140ad0c3b058557229c7790a25fb55ed229ae0efcb63ad07",
+                    "hash": "c2337099eba14767ead75fcc1b1fa265c1898461ede0b5e7758a0e8d11d1757d",
                     "version": 1
                 }
             },
             "HTTPConnection": {
                 "1": {
                     "action": "remove",
                     "hash": "5ee19eaf55ecbe7945ea45924c036ec0f500114a2f64176620961a8c2ec94cdb",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "c05bfaf9ca6b5f47cd20c52fd7961bf9f372196713c2333fc9bfed8e0383acf1",
+                    "hash": "68409295f8916ceb22a8cf4abf89f5e4bcff0d75dc37e16ede37250ada28df59",
                     "version": 2
                 }
             },
             "HTTPNodeRoute": {
                 "1": {
                     "action": "remove",
                     "hash": "1901b9f53f9970ce2bd8307ba9f7cafc0e7eba1d2ec82e4014c6120e605e3741",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "b7ee63d7b47d2fab46a62d8e7d8277c03f872524457f4fe128cc9759eac72795",
+                    "hash": "2134ea812f7c6ea41522727ae087245c4b1195ffbad554db638070861cd9eb1c",
                     "version": 2
                 }
             },
             "JobInfo": {
                 "1": {
                     "action": "remove",
                     "hash": "cf26eeac3d9254dfa439917493b816341f8a379a77d182bbecba3b7ed2c1d00a",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "058a7fc0c63e0bcb399088e7fcde9b8522522e269b00cee2d093d1c890550ce8",
+                    "hash": "89dbd4a810586b49498be1f5299b565a19871487e14a120433b0a4cf607b6dee",
                     "version": 2
                 }
             },
             "JobItem": {
                 "1": {
                     "action": "remove",
                     "hash": "7b8723861837b0b7e948b2cf9244159d232185f3407dd6bef108346f941ddf6e",
@@ -602,87 +602,87 @@
                 "3": {
                     "action": "remove",
                     "hash": "5b93a59e28574691339d22826d5650969336a2e930b93d6b3fe6d5409ca0cfc4",
                     "version": 3
                 },
                 "4": {
                     "action": "add",
-                    "hash": "dae431b87cadacfd30613519b5dd25d2e4ff59d2a971e21a31d56901103b9420",
+                    "hash": "6a7cc7c2bb4dd234c1508b0af4d3b403cd3b7b427578a775bf80dc36891923ed",
                     "version": 4
                 }
             },
             "LibConfig": {
                 "1": {
                     "action": "remove",
                     "hash": "c6ff229aea16874c5d9ae4d1f9e500d13f5cf984bbcee7abd16c5841707a2f78",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "0fc4586bc939a15426ba2315f2457c77eea262c9d34756f0ee6b0198c001cf47",
+                    "hash": "48924a4e5c9dfbc22ef7f2449ca82c7c8d6ae6f6eae070b87747e8a971bd1cb4",
                     "version": 2
                 }
             },
             "LibEndpoint": {
                 "1": {
                     "action": "remove",
                     "hash": "153eac6d8990774eebfffaa75a9895e7c4e1a0e09465d5da0baf4c3a3b03369d",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "c845900e729bef87be1a0efe69a7059055199eb5a5b9b9e8bd730dd16e18ed7a",
+                    "hash": "74916f7c9bbca213b70fcdb5212eae9eb5d3c9fddf4aa35e1fb9a7158fd2d97f",
                     "version": 2
                 }
             },
             "LinkedObject": {
                 "1": {
                     "action": "remove",
                     "hash": "824567c6933c095d0e2f6995c8de3581c0fbd2e9e4ead35c8159f7964709c28e",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "0c52ad9a259358652f7c78f73ab041185a59b24534cee9f0802313ff4b4d4781",
+                    "hash": "08ba9bab178011c723f84bdc64ea879a369f4e6fb32d60020ae123e64b19ec42",
                     "version": 2
                 }
             },
             "MarkdownDescription": {
                 "1": {
                     "action": "remove",
                     "hash": "519328a3952049f57004013e4fb00840695b24b8575cad983056412c9c9d9ba6",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "3416f899b925ba0636edd1ac01bf5c6f4f5533eae4f0a825f112bbf89dcd232a",
+                    "hash": "3c4990cee7cc0b9e86c4b1aa6120476d3d7154d4047d8f4a80a10b6ad1415be4",
                     "version": 2
                 }
             },
             "MongoDict": {
                 "1": {
                     "action": "remove",
                     "hash": "640734396edae801e1601fe7777710e67685e552acb0244ad8b4f689599baca9",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "c83245be5997362196ee7fe2afd2b7ec7a2cf67aed5efe4bde16c7e83dc530b0",
+                    "hash": "47da755ee2c572f719f9c4624120142f0e3c411aeb03278a9eea5fdd92ad2bad",
                     "version": 2
                 }
             },
             "MongoStoreConfig": {
                 "1": {
                     "action": "remove",
                     "hash": "e52aa382e300b0b69aaa2d80aadb4e3a9a3c02b3c741b71d56f959c4d3891ce5",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "f27e70c1c074de2d921f8f0cca02bec90d359cf0a1f255fe77d84455e5daa966",
+                    "hash": "ab2a664a0b3c6f5e0d8323aa26c399c7810462f1a8178f5e5f5021b95a40570c",
                     "version": 2
                 }
             },
             "NodeMetadata": {
                 "1": {
                     "action": "remove",
                     "hash": "6bee018894dfdf697ea624740d0bf051750e0b0d8470ced59646f6d8812068ac",
@@ -696,39 +696,39 @@
                 "3": {
                     "action": "remove",
                     "hash": "3cc67abf394a805066a88aef0bea15bde609b9ecbe7ec15172eac5e7a0b7ef7c",
                     "version": 3
                 },
                 "4": {
                     "action": "add",
-                    "hash": "9501017d54d67c987bf62a37891e9e2ceaa0f741ff6cc502ea1db7bdf26b98da",
+                    "hash": "6d0dd9f388728bb8532ca775587cc7eb9889e111bad8f0b4ba17464140479f9f",
                     "version": 4
                 }
             },
             "NodeMetadataUpdate": {
                 "1": {
                     "action": "remove",
                     "hash": "569d124c23590360bda240c19b53314ccc6204c5d1ab0d2898976a028e002191",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "cfe5400a5440de50e9a413f84c2aa05bad33135f46b16d21496534973145e93c",
+                    "hash": "520ae8ffc0c057ffa827cb7b267a19fb6b92e3cf3c0a3666ac34e271b6dd0aed",
                     "version": 2
                 }
             },
             "NodePeer": {
                 "1": {
                     "action": "remove",
                     "hash": "7b88de7e38490e2d69f31295137673e7ddabc16ab0e2272ff491f6cea1835d63",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "14cf8b9bb7c95c20caec8606ae5dddb882832f00fba2326352e7a0f2444dbc9f",
+                    "hash": "840d11498095c02d3de9bfe48ea8960c81017c4af45cb8af7e12dc9a18ebd2da",
                     "version": 2
                 }
             },
             "NodeSettings": {
                 "1": {
                     "action": "remove",
                     "hash": "b662047bb278f4f5db77c102f94b733c3a929839271b3d6b82ea174a60e2aaf0",
@@ -737,53 +737,53 @@
                 "2": {
                     "action": "remove",
                     "hash": "29a82afcb006a044b6ae04c6ea8a067d145d28b4210bb038ea9fa86ebde108c8",
                     "version": 2
                 },
                 "3": {
                     "action": "add",
-                    "hash": "ea0a9336358fc24988e2e157912f1898a9f770d9520b73a34ce2320b0565f99c",
+                    "hash": "2d5f6e79f074f75b5cfc2357eac7cf635b8f083421009a513240b4dbbd5a0fc1",
                     "version": 3
                 }
             },
             "NodeSettingsUpdate": {
                 "1": {
                     "action": "remove",
                     "hash": "b6ddc66ff270a3c2c4760e31e1a55d72ed04ccae2d0115ebe2fba6f2bf9bd119",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "3f66c4c8a21d63b6dba2ad27c452a01aae6b827ca5c161580312dfb850a0d821",
+                    "hash": "e1dc9d2f30c4aae1f7359eb3fd44de5537788cd3c69be5f30c36fb019f07c261",
                     "version": 2
                 }
             },
             "Notification": {
                 "1": {
                     "action": "remove",
                     "hash": "d13981f721fe2b3e2717640ee07dc716c596e4ecd442461665c3fdab0b85bf0e",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "3814065d869d10444d7413302101c720bc6dd1a105dd7c29eccf38f32351e322",
+                    "hash": "848bdbdbfc655c8cbb6274d3158fad7d3fcdaf77bf0389031dff0d8cedcdbd24",
                     "version": 2
                 }
             },
             "NotificationPreferences": {
                 "1": {
                     "action": "add",
-                    "hash": "127206b9c72d353d9f1b73fb10d8ecd57f28f9bfbfdc2f7648894cb0d2ad2522",
+                    "hash": "e0be3fb928a3e05ba309fc4d59e8eba1e61c6ea09aeb68f25230a5e9446cfcfd",
                     "version": 1
                 }
             },
             "NotifierSettings": {
                 "1": {
                     "action": "add",
-                    "hash": "8505ded16432d1741ee16b0eada22da7c6e36ae7b414cfb59168ac846f3e9f54",
+                    "hash": "efa20280a24d48f583d1e21875a9c195466c7df1239cebbce6016fd6c15c02ad",
                     "version": 1
                 }
             },
             "NumpyArrayObject": {
                 "1": {
                     "action": "remove",
                     "hash": "dcc7b44fa5ad22ae0bc576948f856c172dac1e9de2bc8e2a302e428f3309a278",
@@ -792,15 +792,15 @@
                 "2": {
                     "action": "remove",
                     "hash": "2c631121d9211006edab5620b214dea83e2398bee92244d822227ee316647e22",
                     "version": 2
                 },
                 "3": {
                     "action": "add",
-                    "hash": "709dc84a946267444a3f9968acf4a5e9807d6aa5143626c3fb635c9282108cc1",
+                    "hash": "ff3e9e57df17d6027581ae1aa177199751d8685a3b0cb4359e7e55ace3514041",
                     "version": 3
                 }
             },
             "NumpyBoolObject": {
                 "1": {
                     "action": "remove",
                     "hash": "a5c822a6a3ca9eefd6a2b68f7fd0bc614fba7995f6bcc30bdc9dc882296b9b16",
@@ -809,15 +809,15 @@
                 "2": {
                     "action": "remove",
                     "hash": "24839ba1c88ed833a134124750d5f299abcdf318670315028ed87b254f4578b3",
                     "version": 2
                 },
                 "3": {
                     "action": "add",
-                    "hash": "bf936c1923ceee4def4cded06d41766998ea472322b0738bade7b85298e469da",
+                    "hash": "808a042ea9bca5b621417296824bf2a0b170e66c1f714f91ec3feccace41e2a3",
                     "version": 3
                 }
             },
             "NumpyScalarObject": {
                 "1": {
                     "action": "remove",
                     "hash": "5c1b6b6e8ba88bc79e76646d621489b889fe8f9b9fd59f117d594be18a409633",
@@ -826,87 +826,87 @@
                 "2": {
                     "action": "remove",
                     "hash": "0d5d81b9d45c140f6e07b43ed68d31e0ef060d6b4d0431c9b4795997bb35c69d",
                     "version": 2
                 },
                 "3": {
                     "action": "add",
-                    "hash": "5e84c9905a1816d51c0dfb1eedbfb4d831095ca6c89956c6fe200c2a193cbb8f",
+                    "hash": "9cc5eca915280827de912d66fbb345f43f80787de309613f3fc53130df5fa7d8",
                     "version": 3
                 }
             },
             "ObjectMutation": {
                 "1": {
                     "action": "remove",
                     "hash": "0ee3dd38d6df0fe9a19d848e8f3aaaf13a6ba86afe3406c239caed6da185651a",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "24b7c302f9821afe073534d4ed02c377bd4f7cb691f66ca92b94c38c92dc78c2",
+                    "hash": "4d77ee2650ea29a50e60cf0dcb6cac932b7e6f1aa1e8a927a791ca088e1d07d0",
                     "version": 2
                 }
             },
             "ObjectNotReady": {
                 "1": {
                     "action": "remove",
                     "hash": "88207988639b11eaca686b6e079616d9caecc3dbc2a8112258e0f39ee5c3e113",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "be7001fea1c819ced4c14e6b3a32b59ee11f773d8b23cf42c2f228e782b631b8",
+                    "hash": "07cad6b7fbf4dc9f02ec5857dd4ab4c224fc2da540062a55835eb85df31e7fe8",
                     "version": 2
                 }
             },
             "OnDiskBlobDeposit": {
                 "1": {
                     "action": "remove",
                     "hash": "5efc230c1ee65c4626d334aa69ed458c796c45265e546a333844c6c2bcd0e6b0",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "adc890e6c70334b46f49fff6b4f22d6aa9f13981b4f6ecd16a0f2910ed69da1b",
+                    "hash": "6f8f03f6bf76407b8f34aba12970d037c2a59ec3858feee8f8a3234ebe3a744d",
                     "version": 2
                 }
             },
             "OutputHistory": {
                 "1": {
                     "action": "remove",
                     "hash": "4ec6e6efd86a972b474251885151bdfe4ef262562174605e8ab6a8abba1aa867",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "425ad1c14348e51a2ec0eb82f1ef86b8fbc63e282e4c511023d6c2d644e3bd83",
+                    "hash": "b6e3d6ca02441af981df1c83bb3ccf05e8221e8da3fb369596190c32ee547f12",
                     "version": 2
                 }
             },
             "OutputPolicyExecuteCount": {
                 "1": {
                     "action": "remove",
                     "hash": "6bb24b3b35e19564c43b838ca3f46ccdeadb6596511917f2d220681a378e439d",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "5bce0120ba3b7cbbe08b28bb92bf035215e66232c36899637b8a3f84300747e3",
+                    "hash": "124e48961e0a2ffe9b8ce2aca7244e5c87d3a31debaedfc03c4edc721bb1a86c",
                     "version": 2
                 }
             },
             "OutputPolicyExecuteOnce": {
                 "1": {
                     "action": "remove",
                     "hash": "32a40fc9966b277528eebc61c01041f3a5447417731954abdaffbb14dabc76bb",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "11e2ed5f7fc4bfc701c592352c5377911b0496454c42995c428333ca7ce635c5",
+                    "hash": "429110a31e6a1b91e228e1ce9006607bf6ca3e8ce4c4005c82754b089492ec80",
                     "version": 2
                 }
             },
             "PandasDataframeObject": {
                 "1": {
                     "action": "remove",
                     "hash": "35058924b3de2e0a604a92f91f4dd2e3cc0dac80c219d34f360e7cedd52f5f4c",
@@ -915,15 +915,15 @@
                 "2": {
                     "action": "remove",
                     "hash": "66729d4ba7a92210d45c5a5c24fbdb4c8e58138a515a7bdb71ac8f6e8b868544",
                     "version": 2
                 },
                 "3": {
                     "action": "add",
-                    "hash": "daf3629fb7d26f41f96cd7f9200d7327a4b74d800b3e02afa75454d11bd47d78",
+                    "hash": "30e79bc3df2f7d99d8bca7e58f2d93ab24fc766ce723d985142cf7adee4cc57a",
                     "version": 3
                 }
             },
             "PandasSeriesObject": {
                 "1": {
                     "action": "remove",
                     "hash": "2a0d8a55f1c27bd8fccd276cbe01bf272c40cab10417d7027273983fed423caa",
@@ -932,147 +932,147 @@
                 "2": {
                     "action": "remove",
                     "hash": "cb05a714f75b1140a943f56a3622fcc0477b3a1f504cd545a98510959ffe1528",
                     "version": 2
                 },
                 "3": {
                     "action": "add",
-                    "hash": "4747a220d1587e99e6ac076496a2aa7217e2700205ac80fc24fe4768a313da78",
+                    "hash": "96942949c5a7be48891f84f95b046148bf3e5213b586012071f637c488115ac0",
                     "version": 3
                 }
             },
             "PartialSyftObject": {
                 "1": {
                     "action": "remove",
                     "hash": "008917584d8e1c09015cdbef02f59c0622f48e0618877c1b44425c8846befc13",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "385ef254e4a0c9e68fd750f2bb47f8f9c46dbd2ac9f00f535f843f19f1cf6032",
+                    "hash": "1254e629e855f017511f60a10f249bd266a018c446b8533b58fcbbb7bb63c29e",
                     "version": 2
                 }
             },
             "Plan": {
                 "1": {
                     "action": "remove",
                     "hash": "a0bba2b7792c9e08c453e9e256f0ac6e6185610726566bcd50b057ae83b42d9a",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "67be9b8933b5bec20090727a7b1a03216f874dcc254975481ac62a5a1e9c0c1e",
+                    "hash": "f8e623e1887df2c0051caf9e06820e6603148e8ae688460e10a6f4b2dd405e9d",
                     "version": 2
                 }
             },
             "Project": {
                 "1": {
                     "action": "remove",
                     "hash": "ec5b7ac1c92808e266f06b175c6ebcd50be81777ad120c02ce8c6074d0004788",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "4b7f5d0bec9a1ba7863679b85425f1918745e9dad21476078c19f7257d5f38a3",
+                    "hash": "7a874f5d00996d9781f1e448c1a6fb766aa236fb9b468e8f0f5fdee76a047791",
                     "version": 2
                 }
             },
             "ProjectMessage": {
                 "1": {
                     "action": "remove",
                     "hash": "55a3a5171b6949372b4125cc461bf39bc998565e07703804fca6c7ef99695ae4",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "086513fa450d185b5040b75dc034f4e219c3214677674efa4b4263fda140ce2a",
+                    "hash": "283dd47bd664db581928ffe33e7f93d81100351461976a7d662541837b8490b9",
                     "version": 2
                 }
             },
             "ProjectPoll": {
                 "1": {
                     "action": "remove",
                     "hash": "b0ac8f1d9c06997374ddbc33fdf1d0af0da15fdb6899f52d91a8574106558964",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "90522301ab056881d79a066d824dcce6d7836f2555ac4182bbafe75bea5a5fa7",
+                    "hash": "900f51fcd1cdac2b34f74038a33229273446e211a310138f8af7ac3683094e92",
                     "version": 2
                 }
             },
             "ProjectRequest": {
                 "1": {
                     "action": "remove",
                     "hash": "514d189df335c68869eea36befcdcafec74bdc682eaf18871fe879e26da4dbb6",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "7d7f74f39333bef10ac37f49b5783dc9ba9b5783d2bec814d7de2d2025bcce01",
+                    "hash": "4051700e64dd28f6a928fd3e4cbaf989abf0e2345b7c086f3aa8917e30c756b2",
                     "version": 2
                 }
             },
             "ProjectRequestResponse": {
                 "1": {
                     "action": "remove",
                     "hash": "d4c360e845697a0b24695143d0781626cd344cfde43162c90ae90fe67e00ae21",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "b29309054cd9f9e6a3f00724453f90510076de0bf03ff300fc83670a1721b272",
+                    "hash": "31c346849ab131d6eddb109054a19118c6937b20586fe54f5c7a0a50ecc017e4",
                     "version": 2
                 }
             },
             "ProjectSubmit": {
                 "1": {
                     "action": "remove",
                     "hash": "0374b37779497d7e0b2ffeabc38d35bfbae2ee762a7674a5a8af75e7c5545e61",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "0af1abb9ac899c0bc133971f75d17be8260b80a2df9fe191965db431bb6fd910",
+                    "hash": "70fa24856ecb0df109736e0cb8478cac335801413ca191aa9ced34f5ea3e5189",
                     "version": 2
                 }
             },
             "ProjectThreadMessage": {
                 "1": {
                     "action": "remove",
                     "hash": "1118e935792e8e54103dbf91fa33edbf192a7767d2b1d4526dfa7d4a643cde2e",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "319007e1173c1558917cbdf25171da70514fe0afaae49c7d099aca6f2ec87015",
+                    "hash": "a7454aace740674583226e4f1c1e48284d4ffbc125c196c919d449e2fe8b52a7",
                     "version": 2
                 }
             },
             "PythonConnection": {
                 "1": {
                     "action": "remove",
                     "hash": "011946fc9af0a6987f5c7bc9b0208b2fae9d65217531430bced7ba542788da1a",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "b7bb677f60333d3ab1e927d0be44725667ce75620c2861c706cbca022cfae1fc",
+                    "hash": "eb479c671fc112b2acbedb88bc5624dfdc9592856c04c22c66410f6c863e1708",
                     "version": 2
                 }
             },
             "PythonNodeRoute": {
                 "1": {
                     "action": "remove",
                     "hash": "15711e6e7a1ef726c8e8b5c35a6cb2d30b56ba5213cba489524bf63489e136cf",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "375b36756047fa0e926e5461320960a5c48546ef8cc0c6bb4ff620c7084dc4fc",
+                    "hash": "3eca5767ae4a8fbe67744509e58c6d9fb78f38fa0a0f7fcf5960ab4250acc1f0",
                     "version": 2
                 }
             },
             "QueueItem": {
                 "1": {
                     "action": "remove",
                     "hash": "5aa94681d9d0715d5b605f9625a54e114927271378cf2ea7245f85c488035e0b",
@@ -1086,87 +1086,87 @@
                 "3": {
                     "action": "remove",
                     "hash": "3495f406d2c97050ce86be80c230f49b6b846c63b9a9230cbd6631952f2bad0f",
                     "version": 3
                 },
                 "4": {
                     "action": "add",
-                    "hash": "c37bc1c6303c467050ce4f8faa088a2f66ef1781437ffe34f15aadf5477ac25b",
+                    "hash": "96b0ab4ae935558cd391b86e923f8c7e172b3c27b288c0133197bdc41bd7e19f",
                     "version": 4
                 }
             },
             "RemoteConfig": {
                 "1": {
                     "action": "remove",
                     "hash": "ad7bc4780a8ad52e14ce68601852c93d2fe07bda489809cad7cae786d2461754",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "9d6b8ddb258815b5660f2288164a3a87f68a0e6849493eb48c87da1509b6ab27",
+                    "hash": "0269311d0a524c1f2c565ffd1c9d0da4a4cb4880f98b44cb7d3b76312f5c9f98",
                     "version": 2
                 }
             },
             "ReplyNotification": {
                 "1": {
                     "action": "remove",
                     "hash": "34b2ad522f7406c2486573467d9c7acef5c1063a0d9f2177c3bda2d8c4f87572",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "7bea00170bce350ea1c3a1a16cfb31264e70da9da2fd6f2128852c479e793b60",
+                    "hash": "bc3a15f754ea23a1b6dfe1612ee47a361864c820c507b5644b3fada92bd266e7",
                     "version": 2
                 }
             },
             "Request": {
                 "1": {
                     "action": "remove",
                     "hash": "e054307eeb7f13683cde9ce7613d5ca2925a13fff7c345b1c9f729a12c955f90",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "72bb2fcf520d8ca31fc5fd9b1730a8839648b7f446bcc9f2b6d80e4c635feb59",
+                    "hash": "b8be498ac1e0a7df5e683540ed2a62778faff11404f45f660b3e092e9ed0e37d",
                     "version": 2
                 }
             },
             "RequestInfo": {
                 "1": {
                     "action": "remove",
                     "hash": "b76075c138afc0563ce9ac7f6b1131f048951f7486cd516c02736dc1a2a23639",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "fd127bb4f64b4d04122d31b27b46f712a6f3c9518b2e6df0b140247bab115789",
+                    "hash": "836d768fe0d3d5e134dbcafdff8542a97242ded1b4df1c76dff2ca0f87b28d71",
                     "version": 2
                 }
             },
             "RequestInfoFilter": {
                 "1": {
                     "action": "remove",
                     "hash": "7103abdc464ae71bb746410f5730f55dd8ed82268aa32bbb0a69e0070488a669",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "c8773edca83f068b5a7b7ebe7f5e70ff8df65915564cead695b4528203f750a3",
+                    "hash": "8dabbabdac26c5223579dabe54f7b1b4220b0e49fa6e401fdb09768bca6b49d5",
                     "version": 2
                 }
             },
             "SQLiteStoreConfig": {
                 "1": {
                     "action": "remove",
                     "hash": "b656b26c14cf4e97aba702dd62a0927aec7f860c12eed512c2c688e1b7109aa5",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "e2027eacb8db772fadc506e5bbe797a3fd24175c18b98f79f412cc86ee300f2e",
+                    "hash": "194391d5e90030ad2fe46e7a810ee55dddaa9a1f831667bcdad6e2363c1996fa",
                     "version": 2
                 }
             },
             "SeaweedFSBlobDeposit": {
                 "1": {
                     "action": "remove",
                     "hash": "382a9ac178deed2a9591e1ebbb39f265cbe67027fb93a420d473a4c26b7fda11",
@@ -1175,15 +1175,15 @@
                 "2": {
                     "action": "remove",
                     "hash": "07d84a95324d95d9c868cd7d1c33c908f77aa468671d76c144586aab672bcbb5",
                     "version": 2
                 },
                 "3": {
                     "action": "add",
-                    "hash": "ba3715305ea320413ca5a8780d0d02aeeb5cf3be2445aa274496c539ac787425",
+                    "hash": "05e61e6328b085b738e5d41c0781d87852d44d218894cb3008f5be46e337f6d8",
                     "version": 3
                 }
             },
             "SeaweedSecureFilePathLocation": {
                 "1": {
                     "action": "remove",
                     "hash": "5724a38b1a92b8a55da3d9cc34a720365a6d0c32683acda630fc44067173e201",
@@ -1192,75 +1192,75 @@
                 "2": {
                     "action": "remove",
                     "hash": "5fd63fed2a4efba8c2b6c7a7b5e9b5939181781c331230896aa130b6fd558739",
                     "version": 2
                 },
                 "3": {
                     "action": "add",
-                    "hash": "a986f0e990db9c7ada326b2cca828fa146349a303e674fa48ee4b45702bedc14",
+                    "hash": "12547e03e48b48c44f13720792db9302726c92f33ecc5374bd92ff6f2d733adf",
                     "version": 3
                 }
             },
             "SecureFilePathLocation": {
                 "1": {
                     "action": "remove",
                     "hash": "7febc066e2ee5a3a4a891720afede3f5c155cacc0557662ac4d04bf67b964c6d",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "f1a9510992d60e037c0016574225b8f61433b87bb65bc3320800b1c70e54982c",
+                    "hash": "e4e18e793f25c1ba8eb32849dafc3b85aa1572ebd9a7339ea8776452777d5b7c",
                     "version": 2
                 }
             },
             "ServiceConfig": {
                 "1": {
                     "action": "remove",
                     "hash": "ca91f59bf045d949d82860f7d52655bfbede4cf6bdc5bae8f847f08a16f05d74",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "5945f4f7347baeae0a7f5386d71982a16d6be8ab0c1caa2b10c28d282e66b1ea",
+                    "hash": "4c79a399bbbd8571b712bdb957ff3bc4903aae59cc06bd584c248860dfdab9fe",
                     "version": 2
                 }
             },
             "SignedSyftAPICall": {
                 "1": {
                     "action": "remove",
                     "hash": "e66a116de2fa44ebdd0d4c2d7d5a047dedb555fd201a0f431cd8017d9d33a61d",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "6cd89ed24027ed94b3e2bb7a07e8932060e07e481ceb35eb7ee4d2d0b6e34f43",
+                    "hash": "7a3bdede247c347196d5ced8217d2d3849e91a02dc5fd1c98c4a8bcac98480e4",
                     "version": 2
                 }
             },
             "StoreConfig": {
                 "1": {
                     "action": "remove",
                     "hash": "17de8875cf590311ddb042140347ffc79d4a85028e504dad178ca4e1237ec861",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "3f6c9a967a43557bf88caab87e5d1b9b14ea240bfd5bd6a1a313798e4ee2552b",
+                    "hash": "6df61455f637affc477cf7ded7206009b414269b497a586b5d3374368e9ea602",
                     "version": 2
                 }
             },
             "SubmitRequest": {
                 "1": {
                     "action": "remove",
                     "hash": "96b4ec12beafd9d8a7c97399cb8a23dade4db16d8f521be3fe7b8fec99db5161",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "796b297342793995b8dd87e8feb420e8601dee3b704b7a21a93326661b227ea8",
+                    "hash": "33c6aa318e2d7f3d56897e61c7370a5483bf5a37f25cfa0041ff3bf84949aee2",
                     "version": 2
                 }
             },
             "SubmitUserCode": {
                 "2": {
                     "action": "remove",
                     "hash": "9b29e060973a3de8d3564a2b7d2bb5c53745aa445bf257576994b613505d7194",
@@ -1269,75 +1269,75 @@
                 "3": {
                     "action": "remove",
                     "hash": "a29160c16d2e2620800d42cdcd9f3637d063a570c477a5d05217a2e64b4bb396",
                     "version": 3
                 },
                 "4": {
                     "action": "add",
-                    "hash": "755721313ee8a7148c513c1d0b85324cfcbec14297887daf84ac4c0c5f468a4f",
+                    "hash": "3c5c8627e4f7cca64c1249eea52e7c46171fd4882f76c83e9fa8a1ea7e828b9c",
                     "version": 4
                 }
             },
             "SubmitUserPolicy": {
                 "1": {
                     "action": "remove",
                     "hash": "96f7f39279fadc70c569b8d48ed4d6420a8132db51e37466d272fda19953554b",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "971f4aa69bf68e7a876b0b1cb85ba7d4213212baf7eeaa24bab0a70f18841497",
+                    "hash": "354df4734594f6bc3b58b26c0b60592f454c750e49c00781fc15448dd65a4fb4",
                     "version": 2
                 }
             },
             "SyftAPI": {
                 "1": {
                     "action": "remove",
                     "hash": "2bba1d9fcf677a58e35bf903de3da22ee4913af138aa3012af9c46b3609579cd",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "8f3ff426794df07cbeab441ff545fb896f27897df88b11ec949ec05726a41747",
+                    "hash": "8d24945c5d62c9a910dbe6b925064532db4f351ab7f3eabf1fb454a9e460f7ab",
                     "version": 2
                 }
             },
             "SyftAPICall": {
                 "1": {
                     "action": "remove",
                     "hash": "014bd1d0933f6070888a313edba239170759de24eae49bf2374c1be4dbe2b4d7",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "bc686b6399e058b21472d61fe56df1f0de0785219f52c7306dd5ab8bae863d89",
+                    "hash": "f18183e178a0b5709a2800a7d88f9eef25afefe64d6c646938fec6c5aacd296f",
                     "version": 2
                 }
             },
             "SyftAPIData": {
                 "1": {
                     "action": "remove",
                     "hash": "db101a75227e34750d7056785a1e87bb2e8ad6604f19c372d0cb6aa437243bf5",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "b303d322c7e6da6e003e5d92a27d86acce512228a9dd62c1ab48824702055bf0",
+                    "hash": "931f6019fe66e35eebfe2e0b3c20d7354e2222b4e51a7b60ae9a54c581a77d6e",
                     "version": 2
                 }
             },
             "SyftImageRegistry": {
                 "1": {
                     "action": "remove",
                     "hash": "dc83910c91947e3d9eaa3e6f8592237448f0408668c7cca80450b5fcd54722e1",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "3ceacaa164246323be86ccde0881dd42ee6275684e147095e1d0de7b007ae066",
+                    "hash": "862410fcf514a41ee13273d9540a245ed79e26bb82a0acfe2ad48accc3af1bef",
                     "version": 2
                 }
             },
             "SyftLog": {
                 "1": {
                     "action": "remove",
                     "hash": "bd3f62b8fe4b2718a6380c8f05a93c5c40169fc4ab174db291929298e588429e",
@@ -1346,27 +1346,27 @@
                 "2": {
                     "action": "remove",
                     "hash": "d3ce45794da2e6c4b0cef63b98a553525af50c5d9db42d3d64caef3e7d22b4a9",
                     "version": 2
                 },
                 "3": {
                     "action": "add",
-                    "hash": "6417108288ab4cf090ee2d548fb44b7de7f60b20a33876e5333ab4cabcc5b5df",
+                    "hash": "8964d48238672e0e5d5db6b932cda4ee8eb77581949ab3f7a38a05b1efec13b7",
                     "version": 3
                 }
             },
             "SyftObjectMigrationState": {
                 "1": {
                     "action": "remove",
                     "hash": "d3c8126bc15dae4dd243bb035530e3f56cd9e433d403dd6b5f3b45face6d281f",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "187e6b6619f56fdaf2fbe150a0ec561b1d6a7dbfbc6132257951844206319c79",
+                    "hash": "0b00b9236ae35820733041dc0f4f3956d85d75108a94dba0653aa5948436bd8a",
                     "version": 2
                 }
             },
             "SyftObjectRetrieval": {
                 "2": {
                     "action": "remove",
                     "hash": "d9d7a7e1b8843145c9687fd013c9223700285886073547734267e91ac53e0996",
@@ -1375,77 +1375,77 @@
                 "3": {
                     "action": "remove",
                     "hash": "952958e9afae007bef3cb89aa15be95dddc4c310e3a8ce4191576f90ac6fcbc8",
                     "version": 3
                 },
                 "4": {
                     "action": "add",
-                    "hash": "dd6527e200e7d21e5f4166b2874daf6aeb0b41fafeb8f07f96b675c8625d4cf7",
+                    "hash": "fe151e6fceaafc71c9189d07aed077dc0477bea6a8d7f3c3ace9098ed3161f6b",
                     "version": 4
                 }
             },
             "SyftWorker": {
                 "1": {
                     "action": "remove",
                     "hash": "0d5b367162f3ce55ab090cc1b49bd30e50d4eb144e8431eadc679bd0e743aa70",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "257395af556b1b2972089150c0e3280479a5ba12779d012651eee2f6870e7133",
+                    "hash": "ad19971aabbdf6d032fba708357eb0f0d0bd59f993c58b3e36a1b7ca04332453",
                     "version": 2
                 }
             },
             "SyftWorkerImage": {
                 "1": {
                     "action": "remove",
                     "hash": "2a9585b6a286e24f1a9f3f943d0128730cf853edc549184dc1809d19e1eec54b",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "4a6169ba1f50fdb73ac45500dd02b9d164ef239f13800c0da0ed5f8aed7cde1a",
+                    "hash": "1063e826436e24707eef3f37dbc15f8008ca038fc3f02ad489a49248c8666ba3",
                     "version": 2
                 }
             },
             "SyncState": {
                 "1": {
                     "action": "add",
-                    "hash": "b91ed9a9eb8ac7e2fadafd9376d8adefc83845d2f29939b30e95ebe94dc78cd9",
+                    "hash": "a0616775ec8ef0629e2d91e0df9cc4237ea3674727eda1ce367f1897ee35767d",
                     "version": 1
                 }
             },
             "SyncStateItem": {
                 "1": {
                     "action": "add",
-                    "hash": "cde09be2cfeca4246d001f3f28c00d8647a4506641104e5dc647f136a64fd06e",
+                    "hash": "4dbfa0813f5a3f7be0b36249ff2d67e395ad7c9e138c5a122fc7342b8dcc4b92",
                     "version": 1
                 }
             },
             "TwinObject": {
                 "1": {
                     "action": "remove",
                     "hash": "c42455586b43724a7421becd99122b787a129798daf6081e96954ecaea228099",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "937fded2210d9b792cbe7a99879180e396902fe7b684cd6a14a651db8b9ca2c9",
+                    "hash": "c863c24d4ec1989ce2a0547f9b9152a2a61b24386b38ccd37f0aeae91ce80e41",
                     "version": 2
                 }
             },
             "User": {
                 "2": {
                     "action": "remove",
                     "hash": "ded970c92f202716ed33a2117cf541789f35fad66bd4b1db39da5026b1d7d0e7",
                     "version": 2
                 },
                 "3": {
                     "action": "add",
-                    "hash": "7f5e148674564f2c9c75e19fd2ea17001fbef9e2ba5e49a7e92a8b8b6098f340",
+                    "hash": "ac5179da4b09332cade6aeedd1c59b506ddfe932ee79b9bb2c087dca24391342",
                     "version": 3
                 }
             },
             "UserCode": {
                 "1": {
                     "action": "remove",
                     "hash": "e14c22686cdc7d1fb2b0d01c0aebdea37e62a61b051677c1d30234214f05cd42",
@@ -1459,34 +1459,34 @@
                 "3": {
                     "action": "remove",
                     "hash": "90fcae0f556f375ba1e91d2e345f57241660695c6e2b84c8e311df89d09e6c66",
                     "version": 3
                 },
                 "4": {
                     "action": "add",
-                    "hash": "84ef96946a18e2028d71e125a7a4b8bed2c9cba3c5a2612634509790506e5b9c",
+                    "hash": "0a7181cd5f76800b6566175ffa7276d0cf38c4ddc5110114430147dfc8bfdb2a",
                     "version": 4
                 }
             },
             "UserCodeExecutionOutput": {
                 "1": {
                     "action": "add",
-                    "hash": "d20e83362df8a5d2d2e7eb26a2c5723739f9cfbe4c0272d3ae7e37a34bbe5317",
+                    "hash": "deafafb72d07d724690aaa2fe742379f8e9b3531d9c33f6a8683ee90b462e353",
                     "version": 1
                 }
             },
             "UserCodeExecutionResult": {
                 "1": {
                     "action": "remove",
                     "hash": "49c32e85e78b7b189a7f13b7e26115ef94fcb0b60b578adcbe2b95e289f63a6e",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "05c457f502f7a257a4d5287633d18bbd3cb4ba565afb6a69ac0822c55408a55e",
+                    "hash": "0f4b96ae01b360b7b5ba99f6bd34aaf2da368ff56075bee8137d8c9a82bcec02",
                     "version": 2
                 }
             },
             "UserCodeStatusChange": {
                 "1": {
                     "action": "remove",
                     "hash": "4f5b405cc2b3976ed8f7018df82e873435d9187dff15fa5a23bc85a738969f3f",
@@ -1495,144 +1495,144 @@
                 "2": {
                     "action": "remove",
                     "hash": "d83e0905ae882c824ba8fbbf455cd3881906bf8b2ebbfff07bcf471ef869cedc",
                     "version": 2
                 },
                 "3": {
                     "action": "add",
-                    "hash": "dd79f0f4d8cc7c95120911a0a5d9264cc6e65813bd4ad39f81b756b40c1463e9",
+                    "hash": "6a743ac25193006491f53e0ab697a1391a8f19441d6fa6d6b67d4d5745808b12",
                     "version": 3
                 }
             },
             "UserCodeStatusCollection": {
                 "1": {
                     "action": "add",
-                    "hash": "8d8bae10ee1733464272031e7de6fc783668885206fa448c9f7cd8e8cfc7486a",
+                    "hash": "07481d543ec3131e759822710ab1714d525c0a16b20ebe4a2119f558ba22c125",
                     "version": 1
                 }
             },
             "UserCreate": {
                 "2": {
                     "action": "remove",
                     "hash": "2540188c5aaea866914dccff459df6e0f4727108a503414bb1567ff6297d4646",
                     "version": 2
                 },
                 "3": {
                     "action": "add",
-                    "hash": "26f9467d60b9b642e0a754e9fc028c66a139925fa7d9fac52e5a1e9afdf1387b",
+                    "hash": "70a0d3a701aca47f58009d48c94e314adc464e5429af6794b5770a1163ddfdda",
                     "version": 3
                 }
             },
             "UserPolicy": {
                 "1": {
                     "action": "remove",
                     "hash": "c69b17b1d96cace8b45da6d9639165f2da4aa7ff156b6fd922ac217bf7856d8a",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "6f201caff6457bd036e614a58aedb9fad6a3947b7d4d7965ccfdb788b6385262",
+                    "hash": "9a5ef3d6ece1321ad59c20f2dda08564696e1dd8d017b268ffd70c2958671cad",
                     "version": 2
                 }
             },
             "UserPrivateKey": {
                 "1": {
                     "action": "remove",
                     "hash": "7cb196587887f0f3bffb298dd9f3b88509e9b2748792bf8dc03bdd0d6b98714a",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "0917d22c7cbd3531be6365570952557aed054332d1ec89720213f218e4202ae0",
+                    "hash": "7e99d928122dd7546c94893314f393956c29b8c8d605f62bc99429972f2ffd8e",
                     "version": 2
                 }
             },
             "UserSearch": {
                 "1": {
                     "action": "remove",
                     "hash": "69d1e10b81c8a4143cf70e4f911d8562732af2458ebbc455ca64542f11373dd1",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "6fd7bc05cfad5724d81b1122ddf70c6ea09e6fa77fa374c0b68e0d42e0781088",
+                    "hash": "78d4149c8b1af8510755341fc369eae83d7f67c6b771b50af7f9b3c9b6e7b7aa",
                     "version": 2
                 }
             },
             "UserUpdate": {
                 "2": {
                     "action": "remove",
                     "hash": "32cba8fbd786c575f92e26c31384d282e68e3ebfe5c4b0a0e793820b1228d246",
                     "version": 2
                 },
                 "3": {
                     "action": "add",
-                    "hash": "fd73429a86cc4fe4db51198ae380a18b9a7e42885701efad42bc2ef1b28c04de",
+                    "hash": "a7333af6252bf92ccd913bb23ddc4c0b0c63f8838277d7ebad406be92fa019d2",
                     "version": 3
                 }
             },
             "UserView": {
                 "2": {
                     "action": "remove",
                     "hash": "e410de583bb15bc5af57acef7be55ea5fc56b5b0fc169daa3869f4203c4d7473",
                     "version": 2
                 },
                 "3": {
                     "action": "add",
-                    "hash": "4487e0e96c6cdef771d751bca4e14afac48a17ba7aa03d956521e3d757ab95f5",
+                    "hash": "ac21f70f7bcbc6cadd7b07949e66b66bca31aa5c1fb28196ae38d22dc05eb444",
                     "version": 3
                 }
             },
             "UserViewPage": {
                 "1": {
                     "action": "remove",
                     "hash": "16dac6209b19a934d286ef1efa874379e0040c324e71023c57d1bc6d2d367171",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "0f9d54e606f9a4af73249dd4012baa11fcb7c1e60cce70c01ee48bb63411d6fe",
+                    "hash": "1383d83f202e53490d03049685c1052385ecde4ea6d4b34d4917d08749e02e44",
                     "version": 2
                 }
             },
             "UsersCodeHistoriesDict": {
                 "1": {
                     "action": "remove",
                     "hash": "5e1f389c4565ee8558386dd5c934d81e0c68ab1434f86bb9065976b587ef44d1",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "9cb9a7e1e5c5e294cd019bdb9824180fa399810e7d57db285823157c91ee7d76",
+                    "hash": "863280e2a39de8f50293d54dd9798a0568a2204418fe0bd776b5ea3dcc43e99a",
                     "version": 2
                 }
             },
             "VeilidConnection": {
                 "1": {
                     "action": "add",
-                    "hash": "c5ed1cfa9b7b146dbce7f1057f6e81e89715b5addfd4d4c4d53c415e450373a5",
+                    "hash": "c1796e7b01c9eae0dbf59cfd5c2c2f0e7eba593e0cea615717246572b27aae4b",
                     "version": 1
                 }
             },
             "VeilidNodeRoute": {
                 "1": {
                     "action": "add",
-                    "hash": "4797413e3144fce7bccc290db64f1750e8c09f75d5e1aba6e19d29f921a21074",
+                    "hash": "eadf99eac62574cdda61290c44c564a3ba22faebf27a661da4fc4a2643760376",
                     "version": 1
                 }
             },
             "WorkerPool": {
                 "1": {
                     "action": "remove",
                     "hash": "250699eb4c452fc427995353d5c5ad6245fb3e9fdac8814f8348784816a0733b",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "3fa999bb789b9557939dea820ddcb6c68224822581971a3c3861da3b781d6c25",
+                    "hash": "1b81621b7c03eacfe8369c30bbc97967acef6b5d29a3c67d5f8ad81b49556dac",
                     "version": 2
                 }
             },
             "WorkerSettings": {
                 "1": {
                     "action": "remove",
                     "hash": "0dcd95422ec8a7c74e45ee68a125084c08f898dc94a13d25fe5a5fd0e4fc5027",
@@ -1641,15 +1641,15 @@
                 "2": {
                     "action": "remove",
                     "hash": "d623a8a0d6c83b26ba49686bd8be10eccb126f54626fef334a85396c3b8a8ed6",
                     "version": 2
                 },
                 "3": {
                     "action": "add",
-                    "hash": "d42ed88ba674e8e1ceefa61b0f9fd76400d965e52ab000b2c7f0ae5f9d26d109",
+                    "hash": "20c9e19d8084a87130e173d09d3e9ebaecd3127c455702471eac764d37912a43",
                     "version": 3
                 }
             },
             "ZMQClientConfig": {
                 "1": {
                     "action": "remove",
                     "hash": "e6054969b495791569caaf33239039beae3d116e1fe74e9575467c48b9007c45",
@@ -1658,14 +1658,14 @@
                 "3": {
                     "action": "remove",
                     "hash": "91ce5953cced58e12c576aa5174d5ca0c91981b01cf42edd5283d347baa3390b",
                     "version": 3
                 },
                 "4": {
                     "action": "add",
-                    "hash": "94f4243442d5aa7d2eb48e661a2cbf9d7c1d6a22035a3783977bdfae4a571142",
+                    "hash": "d8761747473ef2af59a7889ab0ea0f69f78a841a9f0cf9fad8260e9c570211d5",
                     "version": 4
                 }
             }
         }
     }
 }
```

### Comparing `syft-0.8.6b1/src/syft/serde/array.py` & `syft-0.8.7b1/src/syft/serde/array.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6b1/src/syft/serde/arrow.py` & `syft-0.8.7b1/src/syft/serde/arrow.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6b1/src/syft/serde/deserialize.py` & `syft-0.8.7b1/src/syft/serde/deserialize.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6b1/src/syft/serde/lib_permissions.py` & `syft-0.8.7b1/src/syft/serde/lib_permissions.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6b1/src/syft/serde/lib_service_registry.py` & `syft-0.8.7b1/src/syft/serde/lib_service_registry.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6b1/src/syft/serde/mock.py` & `syft-0.8.7b1/src/syft/serde/mock.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6b1/src/syft/serde/recursive.py` & `syft-0.8.7b1/src/syft/serde/recursive.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6b1/src/syft/serde/recursive_primitives.py` & `syft-0.8.7b1/src/syft/serde/recursive_primitives.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6b1/src/syft/serde/serializable.py` & `syft-0.8.7b1/src/syft/serde/serializable.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6b1/src/syft/serde/signature.py` & `syft-0.8.7b1/src/syft/serde/signature.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6b1/src/syft/serde/third_party.py` & `syft-0.8.7b1/src/syft/serde/third_party.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # stdlib
 from datetime import date
 from datetime import datetime
 from datetime import time
 import functools
+from importlib.util import find_spec
 from io import BytesIO
 
 # third party
 from dateutil import parser
 from jax import numpy as jnp
 from jaxlib.xla_extension import ArrayImpl
 from nacl.signing import SigningKey
@@ -223,7 +224,37 @@
 
 
 recursive_serde_register(
     DiGraph,
     serialize=serialize_networkx_graph,
     deserialize=deserialize_networkx_graph,
 )
+
+try:
+    # Just register these serializers if the google.cloud.bigquery & db_dtypes module are available
+    # third party
+    from google.cloud.bigquery.job.query import QueryJob
+    from google.cloud.bigquery.table import RowIterator
+
+    # Checking db_dtypes availability this way to avoid unused ruff issues, but this package is used internally
+    if not find_spec("db_dtypes"):
+        raise ImportError("db_dtypes module not found")
+
+    def convert_to_dataframe(obj: RowIterator) -> bytes:
+        dataframe = obj.to_dataframe()
+        return serialize_dataframe(dataframe)
+
+    def convert_from_dataframe(blob: bytes) -> DataFrame:
+        dataframe = deserialize_dataframe(blob)
+        return dataframe
+
+    recursive_serde_register(
+        RowIterator, serialize=convert_to_dataframe, deserialize=convert_from_dataframe
+    )
+
+    recursive_serde_register(
+        QueryJob,
+        serialize=lambda obj: convert_to_dataframe(obj.result()),
+        deserialize=convert_from_dataframe,
+    )
+except ImportError:
+    pass
```

### Comparing `syft-0.8.6b1/src/syft/service/action/action_data_empty.py` & `syft-0.8.7b1/src/syft/service/action/action_data_empty.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6b1/src/syft/service/action/action_graph.py` & `syft-0.8.7b1/src/syft/service/action/action_graph.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6b1/src/syft/service/action/action_graph_service.py` & `syft-0.8.7b1/src/syft/service/action/action_graph_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6b1/src/syft/service/action/action_object.py` & `syft-0.8.7b1/src/syft/service/action/action_object.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,14 +41,16 @@
 from ...types.syft_object import SYFT_OBJECT_VERSION_3
 from ...types.syft_object import SyftBaseObject
 from ...types.syft_object import SyftObject
 from ...types.syncable_object import SyncableSyftObject
 from ...types.uid import LineageID
 from ...types.uid import UID
 from ...util.logger import debug
+from ...util.util import prompt_warning_message
+from ..context import AuthedServiceContext
 from ..response import SyftException
 from ..service import from_api_or_context
 from .action_data_empty import ActionDataEmpty
 from .action_data_empty import ActionDataLink
 from .action_data_empty import ObjectNotReady
 from .action_permissions import ActionPermission
 from .action_types import action_type_for_object
@@ -251,14 +253,15 @@
     "syft_action_data",  # syft
     "syft_resolved",  # syft
     "syft_action_data_node_id",
     "node_uid",
     "migrate_to",  # syft
     "to_dict",  # syft
     "dict",  # syft
+    "has_storage_permission",  # syft
     "_iter",  # pydantic
     "__exclude_fields__",  # pydantic
     "__include_fields__",  # pydantic
     "_calculate_keys",  # pydantic
     "_get_value",  # pydantic
     "__pydantic_validator__",  # pydantic
     "__class_vars__",  # pydantic
@@ -294,35 +297,40 @@
     "model_validate_json",  # pydantic
     "copy",  # pydantic
     "__sha256__",  # syft
     "__hash_exclude_attrs__",  # syft
     "__private_sync_attr_mocks__",  # syft
     "__exclude_sync_diff_attrs__",  # syft
     "__repr_attrs__",  # syft
+    "get_sync_dependencies",
+    "_data_repr",
 ]
 dont_wrap_output_attrs = [
     "__repr__",
     "__str__",
+    "__repr_attrs__",
     "_repr_html_",
     "_repr_markdown_",
     "_repr_latex_",
     "__array_struct__",
     "__array_prepare__",
     "__array_wrap__",
     "__bool__",
     "__len__",
     "syft_resolved",  # syft
     "node_uid",
     "syft_action_data_node_id",
     "__sha256__",
     "__hash_exclude_attrs__",
     "__exclude_sync_diff_attrs__",  # syft
-    "__repr_attrs__",
+    "__repr_attrs__",  # syft
+    "get_sync_dependencies",  # syft
 ]
 dont_make_side_effects = [
+    "__repr_attrs__",
     "_repr_html_",
     "_repr_markdown_",
     "_repr_latex_",
     "__repr__",
     "__getitem__",
     "__setitem__",
     "__len__",
@@ -330,14 +338,15 @@
     "syft_resolved",  # syft
     "node_uid",
     "syft_action_data_node_id",
     "__sha256__",
     "__hash_exclude_attrs__",
     "__exclude_sync_diff_attrs__",  # syft
     "__repr_attrs__",
+    "get_sync_dependencies",
 ]
 action_data_empty_must_run = [
     "__repr__",
     "__str__",
 ]
 
 
@@ -610,14 +619,16 @@
     "__sha256__",
     "__hash_exclude_attrs__",
     "__hash__",
     "create_shareable_sync_copy",
     "_has_private_sync_attrs",
     "__exclude_sync_diff_attrs__",
     "__repr_attrs__",
+    "get_sync_dependencies",
+    "_data_repr",
 ]
 
 
 @serializable(without=["syft_pre_hooks__", "syft_post_hooks__"])
 class ActionObject(SyncableSyftObject):
     """Action object for remote execution."""
 
@@ -1076,14 +1087,29 @@
             op=op,
             remote_self=self.syft_lineage_id,
             args=args,
             kwargs=kwargs,
             action_type=action_type,
         )
 
+    def get_sync_dependencies(
+        self, context: AuthedServiceContext, **kwargs: dict
+    ) -> list[UID]:  # type: ignore
+        # relative
+        from ..job.job_stash import Job
+
+        job_service = context.node.get_service("jobservice")  # type: ignore
+        job: Job | None | SyftError = job_service.get_by_result_id(context, self.id.id)  # type: ignore
+        if isinstance(job, SyftError):
+            return job
+        elif job is not None:
+            return [job.id]
+        else:
+            return []
+
     def syft_get_path(self) -> str:
         """Get the type path of the underlying object"""
         if (
             isinstance(self, AnyActionObject)
             and self.syft_internal_type
             and self.syft_action_data_type is not None
         ):
@@ -1131,42 +1157,57 @@
         """Get the object from a Syft Client"""
         res = client.api.services.action.get(self.id)
         if not isinstance(res, ActionObject):
             return SyftError(message=f"{res}")
         else:
             return res.syft_action_data
 
-    def refresh_object(self) -> ActionObject:
+    def refresh_object(self, resolve_nested: bool = True) -> ActionObject:
         # relative
         from ...client.api import APIRegistry
 
         api = APIRegistry.api_for(
             node_uid=self.syft_node_location,
             user_verify_key=self.syft_client_verify_key,
         )
         if api is None:
             return SyftError(
                 message=f"api is None. You must login to {self.syft_node_location}"
             )
 
-        res = api.services.action.get(self.id)
+        res = api.services.action.get(self.id, resolve_nested=resolve_nested)
         return res
 
+    def has_storage_permission(self) -> bool:
+        api = APIRegistry.api_for(
+            node_uid=self.syft_node_location,
+            user_verify_key=self.syft_client_verify_key,
+        )
+
+        if api is None:
+            return False
+
+        return api.services.action.has_storage_permission(self.id)
+
     def get(self, block: bool = False) -> Any:
         """Get the object from a Syft Client"""
         # relative
 
         if block:
             self.wait()
 
         res = self.refresh_object()
 
         if not isinstance(res, ActionObject):
             return SyftError(message=f"{res}")  # type: ignore
         else:
+            if not self.has_storage_permission():
+                prompt_warning_message(
+                    message="This is a placeholder object, the real data lives on a different node and is not synced."
+                )
             nested_res = res.syft_action_data
             if isinstance(nested_res, ActionObject):
                 nested_res.syft_node_location = res.syft_node_location
                 nested_res.syft_client_verify_key = res.syft_client_verify_key
             return nested_res
 
     def as_empty(self) -> ActionObject:
@@ -1815,29 +1856,33 @@
                         and hasattr(self.syft_action_data_cache, "_repr_markdown_")
                     )
                     else self.syft_action_data_cache.__repr__()
                 )
 
         return f"```python\n{res}\n```\n{data_repr_}"
 
+    def _data_repr(self) -> str | None:
+        if isinstance(self.syft_action_data_cache, ActionDataEmpty):
+            data_repr = self.syft_action_data_repr_
+        elif inspect.isclass(self.syft_action_data_cache):
+            data_repr = repr_cls(self.syft_action_data_cache)
+        else:
+            data_repr = self.syft_action_data_cache.__repr__()
+
+        return data_repr
+
     def __repr__(self) -> str:
         if self.is_mock:
             res = "TwinPointer(Mock)"
         elif self.is_real:
             res = "TwinPointer(Real)"
         if not self.is_twin:
             res = "Pointer"
-        if isinstance(self.syft_action_data_cache, ActionDataEmpty):
-            data_repr_ = self.syft_action_data_repr_
-        else:
-            if inspect.isclass(self.syft_action_data_cache):
-                data_repr_ = repr_cls(self.syft_action_data_cache)
-            else:
-                data_repr_ = self.syft_action_data_cache.__repr__()
-        return f"{res}:\n{data_repr_}"
+        data_repr = self._data_repr()
+        return f"{res}:\n{data_repr}"
 
     def __call__(self, *args: Any, **kwds: Any) -> Any:
         return self.__call__(*args, **kwds)
 
     def __str__(self) -> str:
         if not inspect.isclass(self):
             return self.__str__()
```

### Comparing `syft-0.8.6b1/src/syft/service/action/action_permissions.py` & `syft-0.8.7b1/src/syft/service/action/action_permissions.py`

 * *Files 4% similar despite different names*

```diff
@@ -90,14 +90,15 @@
 class ActionObjectEXECUTE(ActionObjectPermission):
     def __init__(self, uid: UID, credentials: SyftVerifyKey):
         self.uid = uid
         self.credentials = credentials
         self.permission = ActionPermission.EXECUTE
 
 
+@serializable()
 class StoragePermission:
     def __init__(self, uid: UID, node_uid: UID):
         self.uid = uid
         self.node_uid = node_uid
 
     def __repr__(self) -> str:
         return f"StoragePermission: {self.uid} on {self.node_uid}"
```

### Comparing `syft-0.8.6b1/src/syft/service/action/action_service.py` & `syft-0.8.7b1/src/syft/service/action/action_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 # stdlib
 import importlib
 from typing import Any
-from typing import cast
 
 # third party
 import numpy as np
 from result import Err
 from result import Ok
 from result import Result
 
 # relative
-from ...abstract_node import AbstractNode
 from ...node.credentials import SyftVerifyKey
 from ...serde.serializable import serializable
 from ...types.datetime import DateTime
 from ...types.syft_object import SyftObject
 from ...types.twin_object import TwinObject
 from ...types.uid import UID
 from ..blob_storage.service import BlobStorageService
@@ -55,15 +53,15 @@
         self.store = store
 
     @service_method(path="action.np_array", name="np_array")
     def np_array(self, context: AuthedServiceContext, data: Any) -> Any:
         if not isinstance(data, np.ndarray):
             data = np.array(data)
         # cast here since we are sure that AuthedServiceContext has a node
-        context.node = cast(AbstractNode, context.node)
+
         np_obj = NumpyArrayObject(
             dtype=data.dtype,
             shape=data.shape,
             syft_action_data_cache=data,
             syft_node_location=context.node.id,
             syft_client_verify_key=context.credentials,
         )
@@ -123,15 +121,15 @@
         )
         if result.is_ok():
             if isinstance(action_object, TwinObject):
                 if has_result_read_permission:
                     action_object = action_object.private
                 else:
                     action_object = action_object.mock
-            context.node = cast(AbstractNode, context.node)
+
             action_object.syft_point_to(context.node.id)
             return Ok(action_object)
         return result.err()
 
     @service_method(
         path="action.is_resolved", name="is_resolved", roles=GUEST_ROLE_LEVEL
     )
@@ -263,15 +261,15 @@
     @service_method(
         path="action.get_pointer", name="get_pointer", roles=GUEST_ROLE_LEVEL
     )
     def get_pointer(
         self, context: AuthedServiceContext, uid: UID
     ) -> Result[ActionObjectPointer, str]:
         """Get a pointer from the action store"""
-        context.node = cast(AbstractNode, context.node)
+
         result = self.store.get_pointer(
             uid=uid, credentials=context.credentials, node_uid=context.node.id
         )
         if result.is_ok():
             obj = result.ok()
             obj._set_obj_location_(
                 context.node.id,
@@ -286,27 +284,38 @@
     ) -> Result[SyftError, SyftObject]:
         """Get a pointer from the action store"""
         result = self.store.get_mock(uid=uid)
         if result.is_ok():
             return result.ok()
         return SyftError(message=result.err())
 
+    @service_method(
+        path="action.has_storage_permission",
+        name="has_storage_permission",
+        roles=GUEST_ROLE_LEVEL,
+    )
+    def has_storage_permission(self, context: AuthedServiceContext, uid: UID) -> bool:
+        return self.store.has_storage_permission(uid)
+
     # not a public service endpoint
     def _user_code_execute(
         self,
         context: AuthedServiceContext,
         code_item: UserCode,
         kwargs: dict[str, Any],
         result_id: UID | None = None,
     ) -> Result[ActionObjectPointer, Err]:
         override_execution_permission = (
             context.has_execute_permissions or context.role == ServiceRole.ADMIN
         )
+        if context.node:
+            user_code_service = context.node.get_service("usercodeservice")
 
         input_policy = code_item.get_input_policy(context)
+        output_policy = code_item.get_output_policy(context)
 
         if not override_execution_permission:
             if input_policy is None:
                 if not code_item.output_policy_approved:
                     return Err("Execution denied: Your code is waiting for approval")
                 return Err(f"No input policy defined for user code: {code_item.id}")
 
@@ -323,15 +332,18 @@
                 context=context,
                 usr_input_kwargs=kwargs,
                 code_item_id=code_item.id,
             )
             if is_approved.is_err():
                 return is_approved
         else:
-            filtered_kwargs = retrieve_from_db(code_item.id, kwargs, context).ok()
+            result = retrieve_from_db(code_item.id, kwargs, context)
+            if isinstance(result, SyftError):
+                return Err(result.message)
+            filtered_kwargs = result.ok()
         # update input policy to track any input state
 
         has_twin_inputs = False
 
         real_kwargs = {}
         for key, kwarg_value in filtered_kwargs.items():
             if isinstance(kwarg_value, TwinObject):
@@ -343,42 +355,62 @@
         try:
             if not has_twin_inputs:
                 # no twins
                 filtered_kwargs = filter_twin_kwargs(
                     real_kwargs, twin_mode=TwinMode.NONE
                 )
                 exec_result = execute_byte_code(code_item, filtered_kwargs, context)
+                if output_policy:
+                    exec_result.result = output_policy.apply_to_output(
+                        context,
+                        exec_result.result,
+                        update_policy=not override_execution_permission,
+                    )
+                code_item.output_policy = output_policy
+                user_code_service.update_code_state(context, code_item)
                 if isinstance(exec_result.result, ActionObject):
                     result_action_object = ActionObject.link(
                         result_id=result_id, pointer_id=exec_result.result.id
                     )
                 else:
                     result_action_object = wrap_result(result_id, exec_result.result)
             else:
                 # twins
                 private_kwargs = filter_twin_kwargs(
                     real_kwargs, twin_mode=TwinMode.PRIVATE
                 )
                 private_exec_result = execute_byte_code(
                     code_item, private_kwargs, context
                 )
+                if output_policy:
+                    private_exec_result.result = output_policy.apply_to_output(
+                        context,
+                        private_exec_result.result,
+                        update_policy=not override_execution_permission,
+                    )
+                code_item.output_policy = output_policy
+                user_code_service.update_code_state(context, code_item)
                 result_action_object_private = wrap_result(
                     result_id, private_exec_result.result
                 )
 
                 mock_kwargs = filter_twin_kwargs(real_kwargs, twin_mode=TwinMode.MOCK)
                 # relative
                 from .action_data_empty import ActionDataEmpty
 
                 if any(isinstance(v, ActionDataEmpty) for v in mock_kwargs.values()):
                     mock_exec_result_obj = ActionDataEmpty()
                 else:
                     mock_exec_result = execute_byte_code(
                         code_item, mock_kwargs, context
                     )
+                    if output_policy:
+                        mock_exec_result.result = output_policy.apply_to_output(
+                            context, mock_exec_result.result, update_policy=False
+                        )
                     mock_exec_result_obj = mock_exec_result.result
 
                 result_action_object_mock = wrap_result(result_id, mock_exec_result_obj)
 
                 result_action_object = TwinObject(
                     id=result_id,
                     private_obj=result_action_object_private,
@@ -391,36 +423,36 @@
         return Ok(result_action_object)
 
     def set_result_to_store(
         self,
         result_action_object: ActionObject | TwinObject,
         context: AuthedServiceContext,
         output_policy: OutputPolicy | None = None,
-    ) -> Result[ActionObject, str] | SyftError:
+    ) -> Result[ActionObject, str]:
         result_id = result_action_object.id
         # result_blob_id = result_action_object.syft_blob_storage_entry_id
 
         if output_policy is not None:
             output_readers = (
                 output_policy.output_readers
                 if not context.has_execute_permissions
                 else []
             )
         else:
             output_readers = []
 
         read_permission = ActionPermission.READ
-        context.node = cast(AbstractNode, context.node)
+
         result_action_object._set_obj_location_(
             context.node.id,
             context.credentials,
         )
         blob_store_result = result_action_object._save_to_blob_storage()
         if isinstance(blob_store_result, SyftError):
-            return blob_store_result
+            return Err(blob_store_result.message)
 
         # IMPORTANT: DO THIS ONLY AFTER ._save_to_blob_storage
         if isinstance(result_action_object, TwinObject):
             result_blob_id = result_action_object.private.syft_blob_storage_entry_id
         else:
             result_blob_id = result_action_object.syft_blob_storage_entry_id  # type: ignore[unreachable]
 
@@ -621,15 +653,14 @@
     def execute(
         self, context: AuthedServiceContext, action: Action
     ) -> Result[ActionObject, Err]:
         """Execute an operation on objects in the action store"""
         # relative
         from .plan import Plan
 
-        context.node = cast(AbstractNode, context.node)
         if action.action_type == ActionType.CREATEOBJECT:
             result_action_object = Ok(action.create_object)
             # print(action.create_object, "already in blob storage")
         elif action.action_type == ActionType.SYFTFUNCTION:
             usercode_service = context.node.get_service("usercodeservice")
             kwarg_ids = {}
             for k, v in action.kwargs.items():
```

### Comparing `syft-0.8.6b1/src/syft/service/action/action_store.py` & `syft-0.8.7b1/src/syft/service/action/action_store.py`

 * *Files 0% similar despite different names*

```diff
@@ -279,15 +279,18 @@
             self.add_storage_permission(permission)
 
     def remove_storage_permission(self, permission: StoragePermission) -> None:
         permissions = self.storage_permissions[permission.uid]
         permissions.remove(permission.node_uid)
         self.storage_permissions[permission.uid] = permissions
 
-    def has_storage_permission(self, permission: StoragePermission) -> bool:
+    def has_storage_permission(self, permission: StoragePermission | UID) -> bool:
+        if isinstance(permission, UID):
+            permission = StoragePermission(uid=permission, node_uid=self.node_uid)
+
         if permission.uid in self.storage_permissions:
             return permission.node_uid in self.storage_permissions[permission.uid]
         return False
 
     def migrate_data(
         self, to_klass: SyftObject, credentials: SyftVerifyKey
     ) -> Result[bool, str]:
```

### Comparing `syft-0.8.6b1/src/syft/service/action/action_types.py` & `syft-0.8.7b1/src/syft/service/action/action_types.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6b1/src/syft/service/action/numpy.py` & `syft-0.8.7b1/src/syft/service/action/numpy.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6b1/src/syft/service/action/pandas.py` & `syft-0.8.7b1/src/syft/service/action/pandas.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6b1/src/syft/service/action/plan.py` & `syft-0.8.7b1/src/syft/service/action/plan.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6b1/src/syft/service/action/verification.py` & `syft-0.8.7b1/src/syft/service/action/verification.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6b1/src/syft/service/blob_storage/remote_profile.py` & `syft-0.8.7b1/src/syft/service/blob_storage/remote_profile.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6b1/src/syft/service/blob_storage/service.py` & `syft-0.8.7b1/src/syft/service/blob_storage/service.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 # stdlib
 from pathlib import Path
-from typing import cast
 
 # third party
 import requests
 
 # relative
-from ...abstract_node import AbstractNode
 from ...serde.serializable import serializable
 from ...service.action.action_object import ActionObject
 from ...store.blob_storage import BlobRetrieval
 from ...store.blob_storage.on_disk import OnDiskBlobDeposit
 from ...store.blob_storage.seaweedfs import SeaweedFSBlobDeposit
 from ...store.document_store import DocumentStore
 from ...store.document_store import UIDPartitionKey
@@ -84,16 +82,14 @@
             container_name=container_name,
         )
         res = self.remote_profile_stash.set(context.credentials, new_profile)
         if res.is_err():
             return SyftError(message=res.value)
         remote_profile = res.ok()
 
-        context.node = cast(AbstractNode, context.node)
-
         seaweed_config = context.node.blob_storage_client.config
         # we cache this here such that we can use it when reading a file from azure
         # from the remote_name
         seaweed_config.remote_profiles[remote_name] = remote_profile
 
         # TODO: possible wrap this in try catch
         cfg = context.node.blob_store_config.client_config
@@ -200,15 +196,14 @@
         if result.is_ok():
             obj: BlobStorageEntry | None = result.ok()
             if obj is None:
                 return SyftError(
                     message=f"No blob storage entry exists for uid: {uid}, or you have no permissions to read it"
                 )
 
-            context.node = cast(AbstractNode, context.node)
             with context.node.blob_storage_client.connect() as conn:
                 res: BlobRetrieval = conn.read(
                     obj.location, obj.type_, bucket_name=obj.bucket_name
                 )
                 res.syft_blob_storage_entry_id = uid
                 res.file_size = obj.file_size
                 return res
@@ -218,15 +213,14 @@
         path="blob_storage.allocate",
         name="allocate",
         roles=GUEST_ROLE_LEVEL,
     )
     def allocate(
         self, context: AuthedServiceContext, obj: CreateBlobStorageEntry
     ) -> BlobDepositType | SyftError:
-        context.node = cast(AbstractNode, context.node)
         with context.node.blob_storage_client.connect() as conn:
             secure_location = conn.allocate(obj)
 
             if isinstance(secure_location, SyftError):
                 return secure_location
 
             blob_storage_entry = BlobStorageEntry(
@@ -301,15 +295,15 @@
         obj.no_lines = no_lines
         result = self.stash.update(
             credentials=context.credentials,
             obj=obj,
         )
         if result.is_err():
             return SyftError(message=f"{result.err()}")
-        context.node = cast(AbstractNode, context.node)
+
         with context.node.blob_storage_client.connect() as conn:
             result = conn.complete_multipart_upload(obj, etags)
 
         return result
 
     @service_method(path="blob_storage.delete", name="delete")
     def delete(
@@ -320,16 +314,14 @@
             obj = result.ok()
 
             if obj is None:
                 return SyftError(
                     message=f"No blob storage entry exists for uid: {uid}, or you have no permissions to read it"
                 )
 
-            context.node = cast(AbstractNode, context.node)
-
             try:
                 with context.node.blob_storage_client.connect() as conn:
                     file_unlinked_result = conn.delete(obj.location)
             except Exception as e:
                 return SyftError(message=f"Failed to delete file: {e}")
 
             if isinstance(file_unlinked_result, SyftError):
```

### Comparing `syft-0.8.6b1/src/syft/service/blob_storage/stash.py` & `syft-0.8.7b1/src/syft/service/blob_storage/stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6b1/src/syft/service/code/code_parse.py` & `syft-0.8.7b1/src/syft/service/code/code_parse.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6b1/src/syft/service/code/status_service.py` & `syft-0.8.7b1/src/syft/service/code/status_service.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from ...store.document_store import PartitionSettings
 from ...store.document_store import QueryKeys
 from ...store.document_store import UIDPartitionKey
 from ...types.uid import UID
 from ...util.telemetry import instrument
 from ..context import AuthedServiceContext
 from ..response import SyftError
+from ..response import SyftSuccess
 from ..service import AbstractService
 from ..service import TYPE_TO_SERVICE
 from ..service import service_method
 from ..user.user_roles import ADMIN_ROLE_LEVEL
 from ..user.user_roles import GUEST_ROLE_LEVEL
 from .user_code import UserCodeStatusCollection
 
@@ -87,9 +88,19 @@
     ) -> list[UserCodeStatusCollection] | SyftError:
         """Get all user code item statuses"""
         result = self.stash.get_all(context.credentials)
         if result.is_ok():
             return result.ok()
         return SyftError(message=result.err())
 
+    @service_method(path="code_status.remove", name="remove", roles=ADMIN_ROLE_LEVEL)
+    def remove(
+        self, context: AuthedServiceContext, uid: UID
+    ) -> SyftSuccess | SyftError:
+        """Remove a user code item status"""
+        result = self.stash.delete_by_uid(context.credentials, uid=uid)
+        if result.is_ok():
+            return result.ok()
+        return SyftError(message=result.err())
+
 
 TYPE_TO_SERVICE[UserCodeStatusCollection] = UserCodeStatusService
```

### Comparing `syft-0.8.6b1/src/syft/service/code/user_code.py` & `syft-0.8.7b1/src/syft/service/code/user_code.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,14 @@
 # third party
 from IPython.display import display
 from pydantic import field_validator
 from result import Err
 from typing_extensions import Self
 
 # relative
-from ...abstract_node import AbstractNode
 from ...abstract_node import NodeType
 from ...client.api import APIRegistry
 from ...client.api import NodeIdentity
 from ...client.enclave_client import EnclaveMetadata
 from ...node.credentials import SyftVerifyKey
 from ...serde.deserialize import _deserialize
 from ...serde.serializable import serializable
@@ -52,14 +51,15 @@
 from ...types.transforms import generate_id
 from ...types.transforms import transform
 from ...types.uid import UID
 from ...util import options
 from ...util.colors import SURFACE
 from ...util.markdown import CodeMarkdown
 from ...util.markdown import as_markdown_code
+from ..action.action_endpoint import CustomEndpointActionObject
 from ..action.action_object import Action
 from ..action.action_object import ActionObject
 from ..context import AuthedServiceContext
 from ..dataset.dataset import Asset
 from ..job.job_stash import Job
 from ..output.output_service import ExecutionOutput
 from ..output.output_service import OutputService
@@ -194,15 +194,14 @@
     def denied(self) -> bool:
         for status, _ in self.status_dict.values():
             if status == UserCodeStatus.DENIED:
                 return True
         return False
 
     def for_user_context(self, context: AuthedServiceContext) -> UserCodeStatus:
-        context.node = cast(AbstractNode, context.node)
         if context.node.node_type == NodeType.ENCLAVE:
             keys = {status for status, _ in self.status_dict.values()}
             if len(keys) == 1 and UserCodeStatus.APPROVED in keys:
                 return UserCodeStatus.APPROVED
             elif UserCodeStatus.PENDING in keys and UserCodeStatus.DENIED not in keys:
                 return UserCodeStatus.PENDING
             elif UserCodeStatus.DENIED in keys:
@@ -243,15 +242,15 @@
             self.status_dict = status_dict
             return self
         else:
             return SyftError(
                 message="Cannot Modify Status as the Domain's data is not included in the request"
             )
 
-    def get_sync_dependencies(self, api: Any = None) -> list[UID]:
+    def get_sync_dependencies(self, context: AuthedServiceContext) -> list[UID]:
         return [self.user_code_link.object_uid]
 
 
 @serializable()
 class UserCode(SyncableSyftObject):
     # version
     __canonical_name__ = "UserCode"
@@ -456,20 +455,14 @@
         if isinstance(value, InputPolicy):
             self.input_policy_state = _serialize(value, to_bytes=True)
         elif (isinstance(value, bytes) and len(value) == 0) or value is None:
             self.input_policy_state = b""
         else:
             raise Exception(f"You can't set {type(value)} as input_policy_state")
 
-    @property
-    def output_policy(self) -> OutputPolicy | None:  # type: ignore
-        if not self.status.approved:
-            return None
-        return self._get_output_policy()
-
     def get_output_policy(self, context: AuthedServiceContext) -> OutputPolicy | None:
         if not self.get_status(context).approved:
             return None
         return self._get_output_policy()
 
     def _get_output_policy(self) -> OutputPolicy | None:
         # if not self.status.approved:
@@ -502,14 +495,20 @@
 
         try:
             return _deserialize(self.output_policy_state, from_bytes=True)
         except Exception as e:
             print(f"Failed to deserialize custom output policy state. {e}")
             return None
 
+    @property
+    def output_policy(self) -> OutputPolicy | None:  # type: ignore
+        if not self.status.approved:
+            return None
+        return self._get_output_policy()
+
     @output_policy.setter  # type: ignore
     def output_policy(self, value: Any) -> None:  # type: ignore
         if isinstance(value, OutputPolicy):
             self.output_policy_state = _serialize(value, to_bytes=True)
         elif (isinstance(value, bytes) and len(value) == 0) or value is None:
             self.output_policy_state = b""
         else:
@@ -527,33 +526,33 @@
     def get_output_history(
         self, context: AuthedServiceContext
     ) -> list[ExecutionOutput] | SyftError:
         if not self.get_status(context).approved:
             return SyftError(
                 message="Execution denied, Please wait for the code to be approved"
             )
-        node = cast(AbstractNode, context.node)
-        output_service = cast(OutputService, node.get_service("outputservice"))
+
+        output_service = cast(OutputService, context.node.get_service("outputservice"))
         return output_service.get_by_user_code_id(context, self.id)
 
-    def apply_output(
+    def store_as_history(
         self,
         context: AuthedServiceContext,
         outputs: Any,
         job_id: UID | None = None,
         input_ids: dict[str, UID] | None = None,
     ) -> ExecutionOutput | SyftError:
         output_policy = self.get_output_policy(context)
         if output_policy is None:
             return SyftError(
                 message="You must wait for the output policy to be approved"
             )
 
         output_ids = filter_only_uids(outputs)
-        context.node = cast(AbstractNode, context.node)
+
         output_service = context.node.get_service("outputservice")
         output_service = cast(OutputService, output_service)
         execution_result = output_service.create(
             context,
             user_code_id=self.id,
             output_ids=output_ids,
             executing_user_verify_key=self.user_verify_key,
@@ -604,21 +603,27 @@
                 assets = api.services.dataset.get_assets_by_action_id(uid)
                 if not isinstance(assets, list):
                     return assets
 
                 all_assets += assets
         return all_assets
 
-    def get_sync_dependencies(self, api: Any = None) -> list[UID] | SyftError:
+    def get_sync_dependencies(
+        self, context: AuthedServiceContext
+    ) -> list[UID] | SyftError:
         dependencies = []
 
         if self.nested_codes is not None:
-            nested_code_ids = [link.object_uid for link in self.nested_codes.values()]
+            nested_code_ids = [
+                link.object_uid for link, _ in self.nested_codes.values()
+            ]
             dependencies.extend(nested_code_ids)
 
+        dependencies.append(self.status_link.object_uid)
+
         return dependencies
 
     @property
     def unsafe_function(self) -> Callable | None:
         warning = SyftWarning(
             message="This code was submitted by a User and could be UNSAFE."
         )
@@ -1434,14 +1439,18 @@
 
         else:
             print = original_print
 
         if code_item.uses_domain:
             kwargs["domain"] = LocalDomainClient()
 
+        for k, v in kwargs.items():
+            if isinstance(v, CustomEndpointActionObject):
+                kwargs[k] = v.add_context(context=context)
+
         stdout = StringIO()
         stderr = StringIO()
 
         # statisfy lint checker
         result = None
 
         # We only need access to local kwargs
```

### Comparing `syft-0.8.6b1/src/syft/service/code/user_code_parse.py` & `syft-0.8.7b1/src/syft/service/code/user_code_parse.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6b1/src/syft/service/code/user_code_service.py` & `syft-0.8.7b1/src/syft/service/code/user_code_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 
 # third party
 from result import Err
 from result import Ok
 from result import Result
 
 # relative
-from ...abstract_node import AbstractNode
 from ...abstract_node import NodeType
 from ...client.enclave_client import EnclaveClient
 from ...serde.serializable import serializable
 from ...store.document_store import DocumentStore
 from ...store.linked_obj import LinkedObject
 from ...types.cache_object import CachedSyftObject
 from ...types.twin_object import TwinObject
@@ -105,22 +104,33 @@
     def _request_code_execution(
         self,
         context: AuthedServiceContext,
         code: SubmitUserCode,
         reason: str | None = "",
     ) -> Request | SyftError:
         user_code: UserCode = code.to(UserCode, context=context)
-        return self._request_code_execution_inner(context, user_code, reason)
+        result = self._validate_request_code_execution(context, user_code)
+        if isinstance(result, SyftError):
+            # if the validation fails, we should remove the user code status
+            # and code version to prevent dangling status
+            root_context = AuthedServiceContext(
+                credentials=context.node.verify_key, node=context.node
+            )
+            _ = context.node.get_service("usercodestatusservice").remove(
+                root_context, user_code.status_link.object_uid
+            )
+            return result
+        result = self._request_code_execution_inner(context, user_code, reason)
+        return result
 
-    def _request_code_execution_inner(
+    def _validate_request_code_execution(
         self,
         context: AuthedServiceContext,
         user_code: UserCode,
-        reason: str | None = "",
-    ) -> Request | SyftError:
+    ) -> SyftSuccess | SyftError:
         if user_code.output_readers is None:
             return SyftError(
                 message=f"there is no verified output readers for {user_code}"
             )
         if user_code.input_owner_verify_keys is None:
             return SyftError(
                 message=f"there is no verified input owners for {user_code}"
@@ -140,16 +150,14 @@
         find_results = find_results.ok()
 
         if find_results is not None:
             return SyftError(
                 message="The code to be submitted (name and content) already exists"
             )
 
-        context.node = cast(AbstractNode, context.node)
-
         worker_pool_service = context.node.get_service("SyftWorkerPoolService")
         pool_result = worker_pool_service._get_worker_pool(
             context,
             pool_name=user_code.worker_pool_name,
         )
 
         if isinstance(pool_result, SyftError):
@@ -161,14 +169,22 @@
 
         # Create a code history
         code_history_service = context.node.get_service("codehistoryservice")
         result = code_history_service.submit_version(context=context, code=user_code)
         if isinstance(result, SyftError):
             return result
 
+        return SyftSuccess(message="")
+
+    def _request_code_execution_inner(
+        self,
+        context: AuthedServiceContext,
+        user_code: UserCode,
+        reason: str | None = "",
+    ) -> Request | SyftError:
         # Users that have access to the output also have access to the code item
         if user_code.output_readers is not None:
             self.stash.add_permissions(
                 [
                     ActionObjectPermission(user_code.id, ActionPermission.READ, x)
                     for x in user_code.output_readers
                 ]
@@ -224,28 +240,33 @@
             user_code = result.ok()
             if user_code and user_code.input_policy_state and context.node is not None:
                 # TODO replace with LinkedObject Context
                 user_code.node_uid = context.node.id
             return user_code
         return SyftError(message=result.err())
 
-    @service_method(path="code.get_all_for_user", name="get_all_for_user")
+    @service_method(
+        path="code.get_all_for_user",
+        name="get_all_for_user",
+        roles=DATA_SCIENTIST_ROLE_LEVEL,
+    )
     def get_all_for_user(
         self, context: AuthedServiceContext
     ) -> SyftSuccess | SyftError:
         """Get All User Code Items for User's VerifyKey"""
         # TODO: replace with incoming user context and key
         result = self.stash.get_all(context.credentials)
         if result.is_ok():
             return result.ok()
         return SyftError(message=result.err())
 
     def update_code_state(
         self, context: AuthedServiceContext, code_item: UserCode
     ) -> SyftSuccess | SyftError:
+        context = context.as_root_context()
         result = self.stash.update(context.credentials, code_item)
         if result.is_ok():
             return SyftSuccess(message="Code State Updated")
         return SyftError(message="Unable to Update Code State")
 
     def load_user_code(self, context: AuthedServiceContext) -> None:
         result = self.stash.get_all(credentials=context.credentials)
@@ -253,15 +274,14 @@
             user_code_items = result.ok()
             load_approved_policy_code(user_code_items=user_code_items, context=context)
 
     @service_method(path="code.get_results", name="get_results", roles=GUEST_ROLE_LEVEL)
     def get_results(
         self, context: AuthedServiceContext, inp: UID | UserCode
     ) -> list[UserCode] | SyftError:
-        context.node = cast(AbstractNode, context.node)
         uid = inp.id if isinstance(inp, UserCode) else inp
         code_result = self.stash.get_by_uid(context.credentials, uid=uid)
 
         if code_result.is_err():
             return SyftError(message=code_result.err())
         code = code_result.ok()
 
@@ -331,24 +351,23 @@
             return True
 
     def is_execution_on_owned_args_allowed(
         self, context: AuthedServiceContext
     ) -> bool | SyftError:
         if context.role == ServiceRole.ADMIN:
             return True
-        context.node = cast(AbstractNode, context.node)
+
         user_service = context.node.get_service("userservice")
         current_user = user_service.get_current_user(context=context)
         return current_user.mock_execution_permission
 
     def keep_owned_kwargs(
         self, kwargs: dict[str, Any], context: AuthedServiceContext
     ) -> dict[str, Any] | SyftError:
         """Return only the kwargs that are owned by the user"""
-        context.node = cast(AbstractNode, context.node)
 
         action_service = context.node.get_service("actionservice")
 
         mock_kwargs = {}
         for k, v in kwargs.items():
             if isinstance(v, UID):
                 # Jobs have UID kwargs instead of ActionObject
@@ -465,15 +484,14 @@
                                 )
                             )
                         else:
                             return cast(Err, is_valid.to_result())
                     return can_execute.to_result()  # type: ignore
 
             # Execute the code item
-            context.node = cast(AbstractNode, context.node)
 
             action_service = context.node.get_service("actionservice")
 
             result_action_object: Result[ActionObject | TwinObject, str] = (
                 action_service._user_code_execute(
                     context, code, kwarg2id, result_id=result_id
                 )
@@ -492,22 +510,28 @@
             result = output_result.ok()
 
             # Apply Output Policy to the results and update the OutputPolicyState
 
             # this currently only works for nested syft_functions
             # and admins executing on high side (TODO, decide if we want to increment counter)
             if not skip_fill_cache and output_policy is not None:
-                res = code.apply_output(
+                res = code.store_as_history(
                     context=context,
                     outputs=result,
                     job_id=context.job_id,
                     input_ids=kwarg2id,
                 )
                 if isinstance(res, SyftError):
                     return Err(res.message)
+
+            # output_policy.update_policy(context, result)
+            # code.output_policy = output_policy
+            # res = self.update_code_state(context, code)
+            # print(res)
+
             has_result_read_permission = context.extra_kwargs.get(
                 "has_result_read_permission", False
             )
             if isinstance(result, TwinObject):
                 if has_result_read_permission:
                     return Ok(result.private)
                 else:
@@ -526,28 +550,27 @@
             import traceback
 
             return Err(value=f"Failed to run. {e}, {traceback.format_exc()}")
 
     def has_code_permission(
         self, code_item: UserCode, context: AuthedServiceContext
     ) -> SyftSuccess | SyftError:
-        context.node = cast(AbstractNode, context.node)
         if not (
             context.credentials == context.node.verify_key
             or context.credentials == code_item.user_verify_key
         ):
             return SyftError(
                 message=f"Code Execution Permission: {context.credentials} denied"
             )
         return SyftSuccess(message="you have permission")
 
     @service_method(
-        path="code.apply_output", name="apply_output", roles=GUEST_ROLE_LEVEL
+        path="code.store_as_history", name="store_as_history", roles=GUEST_ROLE_LEVEL
     )
-    def apply_output(
+    def store_as_history(
         self,
         context: AuthedServiceContext,
         user_code_id: UID,
         outputs: Any,
         input_ids: dict[str, UID] | None = None,
         job_id: UID | None = None,
     ) -> ExecutionOutput | SyftError:
@@ -555,15 +578,15 @@
         if code_result.is_err():
             return SyftError(message=code_result.err())
 
         code: UserCode = code_result.ok()
         if not code.get_status(context).approved:
             return SyftError(message="Code is not approved")
 
-        res = code.apply_output(
+        res = code.store_as_history(
             context=context,
             outputs=outputs,
             job_id=job_id,
             input_ids=input_ids,
         )
         return res
```

### Comparing `syft-0.8.6b1/src/syft/service/code/user_code_stash.py` & `syft-0.8.7b1/src/syft/service/code/user_code_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6b1/src/syft/service/code/utils.py` & `syft-0.8.7b1/src/syft/service/code/utils.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6b1/src/syft/service/code_history/code_history.py` & `syft-0.8.7b1/src/syft/service/code_history/code_history.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6b1/src/syft/service/code_history/code_history_service.py` & `syft-0.8.7b1/src/syft/service/code_history/code_history_service.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 # stdlib
-from typing import cast
 
 # relative
-from ...abstract_node import AbstractNode
 from ...node.credentials import SyftVerifyKey
 from ...serde.serializable import serializable
 from ...store.document_store import DocumentStore
 from ...types.uid import UID
 from ...util.telemetry import instrument
 from ..code.user_code import SubmitUserCode
 from ..code.user_code import UserCode
@@ -41,15 +39,14 @@
     )
     def submit_version(
         self,
         context: AuthedServiceContext,
         code: SubmitUserCode | UserCode,
         comment: str | None = None,
     ) -> SyftSuccess | SyftError:
-        context.node = cast(AbstractNode, context.node)
         user_code_service = context.node.get_service("usercodeservice")
         if isinstance(code, SubmitUserCode):
             result = user_code_service._submit(context=context, code=code)
             if result.is_err():
                 return SyftError(message=str(result.err()))
             code = result.ok()
         elif isinstance(code, UserCode):  # type: ignore[unreachable]
@@ -122,15 +119,15 @@
 
     def fetch_histories_for_user(
         self, context: AuthedServiceContext, user_verify_key: SyftVerifyKey
     ) -> CodeHistoriesDict | SyftError:
         result = self.stash.get_by_verify_key(
             credentials=context.credentials, user_verify_key=user_verify_key
         )
-        context.node = cast(AbstractNode, context.node)
+
         user_code_service = context.node.get_service("usercodeservice")
 
         def get_code(uid: UID) -> UserCode | SyftError:
             return user_code_service.get_by_uid(context=context, uid=uid)
 
         if result.is_ok():
             code_histories = result.ok()
@@ -166,15 +163,14 @@
         path="code_history.get_history_for_user",
         name="get_history_for_user",
         roles=DATA_OWNER_ROLE_LEVEL,
     )
     def get_history_for_user(
         self, context: AuthedServiceContext, email: str
     ) -> CodeHistoriesDict | SyftError:
-        context.node = cast(AbstractNode, context.node)
         user_service = context.node.get_service("userservice")
         result = user_service.stash.get_by_email(
             credentials=context.credentials, email=email
         )
         if result.is_ok():
             user = result.ok()
             return self.fetch_histories_for_user(
@@ -191,15 +187,14 @@
         self, context: AuthedServiceContext
     ) -> UsersCodeHistoriesDict | SyftError:
         result = self.stash.get_all(credentials=context.credentials)
         if result.is_err():
             return SyftError(message=result.err())
         code_histories: list[CodeHistory] = result.ok()
 
-        context.node = cast(AbstractNode, context.node)
         user_service = context.node.get_service("userservice")
         result = user_service.stash.get_all(context.credentials)
         if result.is_err():
             return SyftError(message=result.err())
         users = result.ok()
 
         user_code_histories = UsersCodeHistoriesDict(node_uid=context.node.id)
@@ -224,15 +219,14 @@
     def get_by_func_name_and_user_email(
         self,
         context: AuthedServiceContext,
         service_func_name: str,
         user_email: str,
         user_id: UID,
     ) -> list[CodeHistory] | SyftError:
-        context.node = cast(AbstractNode, context.node)
         user_service = context.node.get_service("userservice")
         user_verify_key = user_service.user_verify_key(user_email)
 
         if isinstance(user_verify_key, SyftError):
             return user_verify_key
 
         kwargs = {
```

### Comparing `syft-0.8.6b1/src/syft/service/code_history/code_history_stash.py` & `syft-0.8.7b1/src/syft/service/code_history/code_history_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6b1/src/syft/service/context.py` & `syft-0.8.7b1/src/syft/service/context.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 # stdlib
 from typing import Any
-from typing import cast
 
 # third party
 from typing_extensions import Self
 
 # relative
 from ..abstract_node import AbstractNode
 from ..node.credentials import SyftVerifyKey
@@ -20,15 +19,15 @@
 
 
 class NodeServiceContext(Context, SyftObject):
     __canonical_name__ = "NodeServiceContext"
     __version__ = SYFT_OBJECT_VERSION_2
 
     id: UID | None = None  # type: ignore[assignment]
-    node: AbstractNode | None = None
+    node: AbstractNode
 
 
 class AuthedServiceContext(NodeServiceContext):
     __canonical_name__ = "AuthedServiceContext"
     __version__ = SYFT_OBJECT_VERSION_2
 
     credentials: SyftVerifyKey
@@ -44,15 +43,14 @@
     def capabilities(self) -> list[ServiceRoleCapability]:
         return ROLE_TO_CAPABILITIES.get(self.role, [])
 
     def with_credentials(self, credentials: SyftVerifyKey, role: ServiceRole) -> Self:
         return AuthedServiceContext(credentials=credentials, role=role, node=self.node)
 
     def as_root_context(self) -> Self:
-        self.node = cast(AbstractNode, self.node)
         return AuthedServiceContext(
             credentials=self.node.verify_key, role=ServiceRole.ADMIN, node=self.node
         )
 
     @property
     def job(self):  # type: ignore
         # TODO: fix the mypy issue. The return type is Optional[Job].
@@ -67,23 +65,23 @@
 
 
 class UnauthedServiceContext(NodeServiceContext):
     __canonical_name__ = "UnauthedServiceContext"
     __version__ = SYFT_OBJECT_VERSION_2
 
     login_credentials: UserLoginCredentials
-    node: AbstractNode | None = None
+    node: AbstractNode
     role: ServiceRole = ServiceRole.NONE
 
 
 class ChangeContext(SyftBaseObject):
     __canonical_name__ = "ChangeContext"
     __version__ = SYFT_OBJECT_VERSION_2
 
-    node: AbstractNode | None = None
+    node: AbstractNode
     approving_user_credentials: SyftVerifyKey | None = None
     requesting_user_credentials: SyftVerifyKey | None = None
     extra_kwargs: dict = {}
 
     @classmethod
     def from_service(cls, context: AuthedServiceContext) -> Self:
         return cls(
```

### Comparing `syft-0.8.6b1/src/syft/service/data_subject/data_subject.py` & `syft-0.8.7b1/src/syft/service/data_subject/data_subject.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6b1/src/syft/service/data_subject/data_subject_member.py` & `syft-0.8.7b1/src/syft/service/data_subject/data_subject_member.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6b1/src/syft/service/data_subject/data_subject_member_service.py` & `syft-0.8.7b1/src/syft/service/data_subject/data_subject_member_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6b1/src/syft/service/data_subject/data_subject_service.py` & `syft-0.8.7b1/src/syft/service/data_subject/data_subject_service.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 # stdlib
-from typing import cast
 
 # third party
 from result import Result
 
 # relative
-from ...abstract_node import AbstractNode
 from ...node.credentials import SyftVerifyKey
 from ...serde.serializable import serializable
 from ...store.document_store import BaseUIDStoreStash
 from ...store.document_store import DocumentStore
 from ...store.document_store import PartitionSettings
 from ...store.document_store import QueryKeys
 from ...util.telemetry import instrument
@@ -68,15 +66,14 @@
 
     @service_method(path="data_subject.add", name="add_data_subject")
     def add(
         self, context: AuthedServiceContext, data_subject: DataSubjectCreate
     ) -> SyftSuccess | SyftError:
         """Register a data subject."""
 
-        context.node = cast(AbstractNode, context.node)
         member_relationship_add = context.node.get_service_method(
             DataSubjectMemberService.add
         )
 
         member_relationships = data_subject.member_relationships
         for member_relationship in member_relationships:
             parent_ds, child_ds = member_relationship
@@ -105,15 +102,14 @@
             return data_subjects
         return SyftError(message=result.err())
 
     @service_method(path="data_subject.get_members", name="members_for")
     def get_members(
         self, context: AuthedServiceContext, data_subject_name: str
     ) -> list[DataSubject] | SyftError:
-        context.node = cast(AbstractNode, context.node)
         get_relatives = context.node.get_service_method(
             DataSubjectMemberService.get_relatives
         )
 
         relatives = get_relatives(context, data_subject_name)
 
         if isinstance(relatives, SyftError):
```

### Comparing `syft-0.8.6b1/src/syft/service/dataset/dataset.py` & `syft-0.8.7b1/src/syft/service/dataset/dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,16 +29,16 @@
 from ...types.transforms import transform
 from ...types.transforms import validate_url
 from ...types.uid import UID
 from ...util import options
 from ...util.colors import ON_SURFACE_HIGHEST
 from ...util.colors import SURFACE
 from ...util.colors import SURFACE_SURFACE
+from ...util.fonts import FONT_CSS
 from ...util.fonts import ITABLES_CSS
-from ...util.fonts import fonts_css
 from ...util.markdown import as_markdown_python_code
 from ...util.notebook_ui.notebook_addons import FOLDER_ICON
 from ...util.util import get_mb_size
 from ..data_subject.data_subject import DataSubject
 from ..data_subject.data_subject import DataSubjectCreate
 from ..data_subject.data_subject_service import DataSubjectService
 from ..response import SyftError
@@ -178,15 +178,15 @@
         else:
             mock_table_line = self.mock
             if isinstance(mock_table_line, SyftError):
                 mock_table_line = mock_table_line.message
 
         return f"""
             <style>
-            {fonts_css}
+            {FONT_CSS}
             .syft-asset {{color: {SURFACE[options.color_theme]};}}
             .syft-asset h3,
             .syft-asset p
               {{font-family: 'Open Sans'}}
             {ITABLES_CSS}
             </style>
 
@@ -487,15 +487,15 @@
             )
             if self.uploader
             else ""
         )
         description_text: str = self.description.text if self.description else ""
         return f"""
             <style>
-            {fonts_css}
+            {FONT_CSS}
             .syft-dataset {{color: {SURFACE[options.color_theme]};}}
             .syft-dataset h3,
             .syft-dataset p
               {{font-family: 'Open Sans';}}
               {ITABLES_CSS}
             </style>
             <div class='syft-dataset'>
```

### Comparing `syft-0.8.6b1/src/syft/service/dataset/dataset_service.py` & `syft-0.8.7b1/src/syft/service/dataset/dataset_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,24 +92,18 @@
                 ActionObjectPermission(
                     uid=dataset.id, permission=ActionPermission.ALL_READ
                 ),
             ],
         )
         if result.is_err():
             return SyftError(message=str(result.err()))
-        if context.node is not None:
-            return SyftSuccess(
-                message=f"Dataset uploaded to '{context.node.name}'. "
-                f"To see the datasets uploaded by a client on this node, use command `[your_client].datasets`"
-            )
-        else:
-            return SyftSuccess(
-                message="Dataset uploaded not to a node."
-                "To see the datasets uploaded by a client on this node, use command `[your_client].datasets`"
-            )
+        return SyftSuccess(
+            message=f"Dataset uploaded to '{context.node.name}'. "
+            f"To see the datasets uploaded by a client on this node, use command `[your_client].datasets`"
+        )
 
     @service_method(
         path="dataset.get_all",
         name="get_all",
         roles=GUEST_ROLE_LEVEL,
         warning=CRUDReminder(),
     )
@@ -130,17 +124,15 @@
             if context.node is not None:
                 dataset.node_uid = context.node.id
 
         return _paginate_dataset_collection(
             datasets=datasets, page_size=page_size, page_index=page_index
         )
 
-    @service_method(
-        path="dataset.search", name="search", roles=DATA_SCIENTIST_ROLE_LEVEL
-    )
+    @service_method(path="dataset.search", name="search", roles=GUEST_ROLE_LEVEL)
     def search(
         self,
         context: AuthedServiceContext,
         name: str,
         page_size: int | None = 0,
         page_index: int | None = 0,
     ) -> DatasetPageView | SyftError:
@@ -203,16 +195,17 @@
                         assets.append(asset)
             return assets
         elif isinstance(datasets, SyftError):
             return datasets
         return []
 
     @service_method(
-        path="dataset.delete_by_id",
-        name="dataset_delete_by_id",
+        path="dataset.delete_by_uid",
+        name="delete_by_uid",
+        roles=DATA_OWNER_ROLE_LEVEL,
         warning=HighSideCRUDWarning(confirmation=True),
     )
     def delete_dataset(
         self, context: AuthedServiceContext, uid: UID
     ) -> SyftSuccess | SyftError:
         result = self.stash.delete_by_uid(context.credentials, uid)
         if result.is_ok():
```

### Comparing `syft-0.8.6b1/src/syft/service/dataset/dataset_stash.py` & `syft-0.8.7b1/src/syft/service/dataset/dataset_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6b1/src/syft/service/enclave/enclave_service.py` & `syft-0.8.7b1/src/syft/service/enclave/enclave_service.py`

 * *Files 17% similar despite different names*

```diff
@@ -90,55 +90,18 @@
                 return SyftError(
                     message=f"Error while fetching the object on Enclave: {res.err()}"
                 )
 
         return SyftSuccess(message="Enclave Code Status Updated Successfully")
 
 
-def get_oblv_service() -> type[AbstractService] | SyftError:
-    # relative
-    from ...external import OBLV_ENABLED
-
-    if OBLV_ENABLED:
-        # relative
-        from ...external.oblv.oblv_service import OblvService
-
-        return OblvService
-    else:
-        return SyftError(
-            message="Oblivious is not enabled."
-            "To enable oblivious package, set sy.enable_external_lib('oblv') "
-            "on the client side"
-            "Or add --oblv when launching by hagrid"
-        )
-
-
-# Checks if the given user code would  propogate value to enclave on acceptance
+# Checks if the given user code would propogate value to enclave on acceptance
 def propagate_inputs_to_enclave(
     user_code: UserCode, context: ChangeContext
 ) -> SyftSuccess | SyftError:
-    # Temporarily disable Oblivious Enclave
-    # from ...external.oblv.deployment_client import OblvMetadata
-
-    # if isinstance(user_code.enclave_metadata, OblvMetadata):
-    #     # relative
-    #     oblv_service_class = get_oblv_service()
-    #     if isinstance(oblv_service_class, SyftError):
-    #         return oblv_service_class
-    #     method = context.node.get_service_method(oblv_service_class.get_api_for)
-
-    #     api = method(
-    #         user_code.enclave_metadata,
-    #         context.node.signing_key,
-    #         worker_name=context.node.name,
-    #     )
-    #     send_method = api.services.oblv.send_user_code_inputs_to_enclave
-    if context.node is None:
-        return SyftError(message=f"context {context}'s node is None")
-
     if isinstance(user_code.enclave_metadata, EnclaveMetadata):
         # TODO 🟣 Restructure url it work for local mode host.docker.internal
 
         connection = route_to_connection(user_code.enclave_metadata.route)
         enclave_client = EnclaveClient(
             connection=connection,
             credentials=context.node.signing_key,
```

### Comparing `syft-0.8.6b1/src/syft/service/job/job_service.py` & `syft-0.8.7b1/src/syft/service/job/job_service.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # stdlib
 from typing import Any
 from typing import cast
 
 # relative
-from ...abstract_node import AbstractNode
 from ...node.worker_settings import WorkerSettings
 from ...serde.serializable import serializable
 from ...store.document_store import DocumentStore
 from ...types.uid import UID
 from ...util.telemetry import instrument
 from ..action.action_permissions import ActionObjectPermission
 from ..action.action_permissions import ActionPermission
@@ -89,27 +88,38 @@
     ) -> SyftSuccess | SyftError:
         res = self.stash.delete_by_uid(context.credentials, uid)
         if res.is_err():
             return SyftError(message=res.err())
         return SyftSuccess(message="Great Success!")
 
     @service_method(
+        path="job.get_by_result_id",
+        name="get_by_result_id",
+        roles=ADMIN_ROLE_LEVEL,
+    )
+    def get_by_result_id(
+        self, context: AuthedServiceContext, result_id: UID
+    ) -> Job | None | SyftError:
+        res = self.stash.get_by_result_id(context.credentials, result_id)
+        if res.is_err():
+            return SyftError(message=res.err())
+        return res.ok()
+
+    @service_method(
         path="job.restart",
         name="restart",
         roles=DATA_SCIENTIST_ROLE_LEVEL,
     )
     def restart(
         self, context: AuthedServiceContext, uid: UID
     ) -> SyftSuccess | SyftError:
         res = self.stash.get_by_uid(context.credentials, uid=uid)
         if res.is_err():
             return SyftError(message=res.err())
 
-        context.node = cast(AbstractNode, context.node)
-
         job = res.ok()
         job.status = JobStatus.CREATED
         self.update(context=context, job=job)
 
         task_uid = UID()
         worker_settings = WorkerSettings.from_node(context.node)
 
@@ -211,15 +221,14 @@
         path="job.add_read_permission_log_for_code_owner",
         name="add_read_permission_log_for_code_owner",
         roles=DATA_OWNER_ROLE_LEVEL,
     )
     def add_read_permission_log_for_code_owner(
         self, context: AuthedServiceContext, log_id: UID, user_code: UserCode
     ) -> Any:
-        context.node = cast(AbstractNode, context.node)
         log_service = context.node.get_service("logservice")
         log_service = cast(LogService, log_service)
         return log_service.stash.add_permission(
             ActionObjectPermission(
                 log_id, ActionPermission.READ, user_code.user_verify_key
             )
         )
@@ -228,15 +237,14 @@
         path="job.create_job_for_user_code_id",
         name="create_job_for_user_code_id",
         roles=DATA_OWNER_ROLE_LEVEL,
     )
     def create_job_for_user_code_id(
         self, context: AuthedServiceContext, user_code_id: UID
     ) -> Job | SyftError:
-        context.node = cast(AbstractNode, context.node)
         job = Job(
             id=UID(),
             node_uid=context.node.id,
             action=None,
             result_id=None,
             parent_id=None,
             log_id=UID(),
@@ -249,15 +257,15 @@
             return user_code
 
         # The owner of the code should be able to read the job
         self.stash.set(context.credentials, job)
         self.add_read_permission_job_for_code_owner(context, job, user_code)
 
         log_service = context.node.get_service("logservice")
-        res = log_service.add(context, job.log_id)
+        res = log_service.add(context, job.log_id, job.id)
         if isinstance(res, SyftError):
             return res
         # The owner of the code should be able to read the job log
         self.add_read_permission_log_for_code_owner(context, job.log_id, user_code)
         # log_service.stash.add_permission(
         #     ActionObjectPermission(
         #         job.log_id, ActionPermission.READ, user_code.user_verify_key
```

### Comparing `syft-0.8.6b1/src/syft/service/job/job_stash.py` & `syft-0.8.7b1/src/syft/service/job/job_stash.py`

 * *Files 15% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from typing_extensions import Self
 
 # relative
 from ...client.api import APIRegistry
 from ...client.api import SyftAPICall
 from ...node.credentials import SyftVerifyKey
 from ...serde.serializable import serializable
-from ...service.queue.queue_stash import QueueItem
+from ...service.context import AuthedServiceContext
 from ...service.worker.worker_pool import SyftWorker
 from ...store.document_store import BaseStash
 from ...store.document_store import DocumentStore
 from ...store.document_store import PartitionKey
 from ...store.document_store import PartitionSettings
 from ...store.document_store import QueryKeys
 from ...store.document_store import UIDPartitionKey
@@ -32,14 +32,15 @@
 from ...types.syft_object import short_uid
 from ...types.syncable_object import SyncableSyftObject
 from ...types.uid import UID
 from ...util import options
 from ...util.colors import SURFACE
 from ...util.markdown import as_markdown_code
 from ...util.telemetry import instrument
+from ...util.util import prompt_warning_message
 from ..action.action_data_empty import ActionDataLink
 from ..action.action_object import Action
 from ..action.action_object import ActionObject
 from ..action.action_permissions import ActionObjectPermission
 from ..response import SyftError
 from ..response import SyftNotReady
 from ..response import SyftSuccess
@@ -73,15 +74,22 @@
     action: Action | None = None
     job_pid: int | None = None
     job_worker_id: UID | None = None
     updated_at: DateTime | None = None
     user_code_id: UID | None = None
 
     __attr_searchable__ = ["parent_job_id", "job_worker_id", "status", "user_code_id"]
-    __repr_attrs__ = ["id", "result", "resolved", "progress", "creation_time"]
+    __repr_attrs__ = [
+        "id",
+        "result",
+        "resolved",
+        "progress",
+        "creation_time",
+        "user_code_name",
+    ]
     __exclude_sync_diff_attrs__ = ["action"]
 
     @field_validator("creation_time")
     @classmethod
     def check_time(cls, time: Any) -> Any:
         return str(datetime.now()) if time is None else time
 
@@ -105,14 +113,27 @@
         else:
             # hacky
             self.action.syft_node_location = self.syft_node_location
             self.action.syft_client_verify_key = self.syft_client_verify_key
             return self.action.job_display_name
 
     @property
+    def user_code_name(self) -> str | None:
+        if self.user_code_id is not None:
+            api = APIRegistry.api_for(
+                node_uid=self.syft_node_location,
+                user_verify_key=self.syft_client_verify_key,
+            )
+            if api is None:
+                return None
+            user_code = api.services.code.get_by_id(self.user_code_id)
+            return user_code.service_func_name
+        return None
+
+    @property
     def time_remaining_string(self) -> str | None:
         # update state
         self.fetch()
         if (
             self.current_iter is not None
             and self.n_iters is not None
             and self.n_iters != 0
@@ -290,15 +311,15 @@
             self.result = job.result
 
         self.status = job.status
         self.n_iters = job.n_iters
         self.current_iter = job.current_iter
 
     @property
-    def subjobs(self) -> list[QueueItem] | SyftError:
+    def subjobs(self) -> list["Job"] | SyftError:
         api = APIRegistry.api_for(
             node_uid=self.syft_node_location,
             user_verify_key=self.syft_client_verify_key,
         )
         if api is None:
             return SyftError(
                 message=f"Can't access Syft API. You must login to {self.syft_node_location}"
@@ -331,35 +352,52 @@
     ) -> str | None:
         api = APIRegistry.api_for(
             node_uid=self.syft_node_location,
             user_verify_key=self.syft_client_verify_key,
         )
         if api is None:
             return f"Can't access Syft API. You must login to {self.syft_node_location}"
+
+        has_permissions = True
+
         results = []
         if stdout:
             stdout_log = api.services.log.get_stdout(self.log_id)
             if isinstance(stdout_log, SyftError):
                 results.append(f"Log {self.log_id} not available")
+                has_permissions = False
             else:
                 results.append(stdout_log)
 
         if stderr:
             try:
                 std_err_log = api.services.log.get_error(self.log_id)
-                results.append(std_err_log)
+                if isinstance(std_err_log, SyftError):
+                    results.append(f"Error log {self.log_id} not available")
+                    has_permissions = False
+                else:
+                    results.append(std_err_log)
             except Exception:
                 # no access
                 if isinstance(self.result, Err):
                     results.append(self.result.value)
         else:
             # add short error
             if isinstance(self.result, Err):
                 results.append(self.result.value)
 
+        if has_permissions:
+            has_storage_permission = api.services.log.has_storage_permission(
+                self.log_id
+            )
+            if not has_storage_permission:
+                prompt_warning_message(
+                    message="This is a placeholder object, the real data lives on a different node and is not synced."
+                )
+
         results_str = "\n".join(results)
         if not _print:
             return results_str
         else:
             print(results_str)
             return None
 
@@ -467,28 +505,40 @@
         if not self.resolved:
             self.fetch()
 
         if self.resolved:
             return self.result
         return SyftNotReady(message=f"{self.id} not ready yet.")
 
-    def get_sync_dependencies(self, **kwargs: dict) -> list[UID]:  # type: ignore
+    def get_sync_dependencies(self, context: AuthedServiceContext) -> list[UID]:  # type: ignore
         dependencies = []
         if self.result is not None:
             dependencies.append(self.result.id.id)
 
         if self.log_id:
             dependencies.append(self.log_id)
 
+        subjobs = self.subjobs
+        if isinstance(subjobs, SyftError):
+            return subjobs
+
         subjob_ids = [subjob.id for subjob in self.subjobs]
         dependencies.extend(subjob_ids)
 
         if self.user_code_id is not None:
             dependencies.append(self.user_code_id)
 
+        output = context.node.get_service("outputservice").get_by_job_id(  # type: ignore
+            context, self.id
+        )
+        if isinstance(output, SyftError):
+            return output
+        elif output is not None:
+            dependencies.append(output.id)
+
         return dependencies
 
 
 @serializable()
 class JobInfo(SyftObject):
     __canonical_name__ = "JobInfo"
     __version__ = SYFT_OBJECT_VERSION_2
@@ -591,14 +641,33 @@
         add_permissions: list[ActionObjectPermission] | None = None,
     ) -> Result[Job | None, str]:
         valid = self.check_type(item, self.object_type)
         if valid.is_err():
             return SyftError(message=valid.err())
         return super().update(credentials, item, add_permissions)
 
+    def get_by_result_id(
+        self,
+        credentials: SyftVerifyKey,
+        res_id: UID,
+    ) -> Result[Job | None, str]:
+        res = self.get_all(credentials)
+        if res.is_err():
+            return res
+        else:
+            res = res.ok()
+            # beautiful query
+            res = [x for x in res if x.result is not None and x.result.id.id == res_id]
+            if len(res) == 0:
+                return Ok(None)
+            elif len(res) > 1:
+                return Err(message="multiple Jobs found")
+            else:
+                return Ok(res[0])
+
     def set_placeholder(
         self,
         credentials: SyftVerifyKey,
         item: Job,
         add_permissions: list[ActionObjectPermission] | None = None,
     ) -> Result[Job, str]:
         # 🟡 TODO 36: Needs distributed lock
```

### Comparing `syft-0.8.6b1/src/syft/service/log/log_service.py` & `syft-0.8.7b1/src/syft/service/log/log_service.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,16 +27,18 @@
     stash: LogStash
 
     def __init__(self, store: DocumentStore) -> None:
         self.store = store
         self.stash = LogStash(store=store)
 
     @service_method(path="log.add", name="add", roles=DATA_SCIENTIST_ROLE_LEVEL)
-    def add(self, context: AuthedServiceContext, uid: UID) -> SyftSuccess | SyftError:
-        new_log = SyftLog(id=uid)
+    def add(
+        self, context: AuthedServiceContext, uid: UID, job_id: UID
+    ) -> SyftSuccess | SyftError:
+        new_log = SyftLog(id=uid, job_id=job_id)
         result = self.stash.set(context.credentials, new_log)
         if result.is_err():
             return SyftError(message=str(result.err()))
         return result
 
     @service_method(path="log.append", name="append", roles=DATA_SCIENTIST_ROLE_LEVEL)
     def append(
@@ -60,14 +62,15 @@
         if result.is_err():
             return SyftError(message=str(result.err()))
         return SyftSuccess(message="Log Append successful!")
 
     @service_method(path="log.get", name="get", roles=DATA_SCIENTIST_ROLE_LEVEL)
     def get(self, context: AuthedServiceContext, uid: UID) -> SyftSuccess | SyftError:
         result = self.stash.get_by_uid(context.credentials, uid)
+
         if result.is_err():
             return SyftError(message=str(result.err()))
 
         return result
 
     @service_method(
         path="log.get_stdout", name="get_stdout", roles=DATA_SCIENTIST_ROLE_LEVEL
@@ -121,9 +124,21 @@
     ) -> SyftSuccess | SyftError:
         result = self.stash.delete_by_uid(context.credentials, uid)
         if result.is_ok():
             return result.ok()
         else:
             return SyftError(message=result.err())
 
+    @service_method(
+        path="log.has_storage_permission",
+        name="has_storage_permission",
+        roles=DATA_SCIENTIST_ROLE_LEVEL,
+    )
+    def has_storage_permission(self, context: AuthedServiceContext, uid: UID) -> bool:
+        result = self.stash.has_storage_permission(
+            uid,
+        )
+
+        return result
+
 
 TYPE_TO_SERVICE[SyftLog] = LogService
```

### Comparing `syft-0.8.6b1/src/syft/service/log/log_stash.py` & `syft-0.8.7b1/src/syft/service/log/log_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6b1/src/syft/service/metadata/metadata_service.py` & `syft-0.8.7b1/src/syft/service/metadata/metadata_service.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 # stdlib
-from typing import cast
 
 # relative
-from ...abstract_node import AbstractNode
 from ...serde.serializable import serializable
 from ...store.document_store import DocumentStore
 from ...util.telemetry import instrument
 from ..context import AuthedServiceContext
 from ..service import AbstractService
 from ..service import service_method
 from ..user.user_roles import GUEST_ROLE_LEVEL
@@ -19,20 +17,18 @@
     def __init__(self, store: DocumentStore) -> None:
         self.store = store
 
     @service_method(
         path="metadata.get_metadata", name="get_metadata", roles=GUEST_ROLE_LEVEL
     )
     def get_metadata(self, context: AuthedServiceContext) -> NodeMetadataV3:
-        context.node = cast(AbstractNode, context.node)
         return context.node.metadata  # type: ignore
 
     # @service_method(path="metadata.get_admin", name="get_admin", roles=GUEST_ROLE_LEVEL)
     # def get_admin(self, context: AuthedServiceContext):
     #     user_service = context.node.get_service("userservice")
     #     admin_user = user_service.get_all(context=context)[0]
     #     return admin_user
 
     @service_method(path="metadata.get_env", name="get_env", roles=GUEST_ROLE_LEVEL)
     def get_env(self, context: AuthedServiceContext) -> str:
-        context.node = cast(AbstractNode, context.node)
         return context.node.packages
```

### Comparing `syft-0.8.6b1/src/syft/service/metadata/migrations.py` & `syft-0.8.7b1/src/syft/service/metadata/migrations.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6b1/src/syft/service/metadata/node_metadata.py` & `syft-0.8.7b1/src/syft/service/metadata/node_metadata.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6b1/src/syft/service/network/network_service.py` & `syft-0.8.7b1/src/syft/service/network/network_service.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 # stdlib
 from collections.abc import Callable
 import secrets
 from typing import Any
-from typing import cast
 
 # third party
 from result import Result
 
 # relative
-from ...abstract_node import AbstractNode
 from ...abstract_node import NodeType
 from ...client.client import HTTPConnection
 from ...client.client import PythonConnection
 from ...client.client import SyftClient
 from ...client.client import VeilidConnection
 from ...node.credentials import SyftVerifyKey
 from ...node.worker_settings import WorkerSettings
@@ -173,15 +171,15 @@
             remote_node_verify_key.verify_key.verify(
                 random_challenge, challenge_signature
             )
         except Exception as e:
             return SyftError(message=str(e))
 
         # save the remote peer for later
-        context.node = cast(AbstractNode, context.node)
+
         result = self.stash.update_peer(
             context.node.verify_key,
             remote_node_peer,
         )
         if result.is_err():
             return SyftError(message=str(result.err()))
 
@@ -203,15 +201,14 @@
             return SyftError(
                 message=(
                     f"The {type(peer)}.verify_key: "
                     f"{peer.verify_key} does not match the signature of the message"
                 )
             )
 
-        context.node = cast(AbstractNode, context.node)
         if verify_key != context.node.verify_key:
             return SyftError(
                 message="verify_key does not match the remote node's verify_key for add_peer"
             )
 
         try:
             remote_client: SyftClient = peer.client_with_context(context=context)
@@ -260,15 +257,15 @@
 
         # # Only the root user can ping the node to check its state
         # if context.node.verify_key != context.credentials:
         #     return SyftError(message=("Only the root user can access ping endpoint"))
 
         # this way they can match up who we are with who they think we are
         # Sending a signed messages for the peer to verify
-        context.node = cast(AbstractNode, context.node)
+
         challenge_signature = context.node.signing_key.signing_key.sign(
             challenge
         ).signature
 
         return challenge_signature
 
     @service_method(path="network.add_route_for", name="add_route_for")
@@ -291,15 +288,15 @@
         path="network.verify_route", name="verify_route", roles=GUEST_ROLE_LEVEL
     )
     def verify_route(
         self, context: AuthedServiceContext, route: NodeRoute
     ) -> SyftSuccess | SyftError:
         """Add a Network Node Route"""
         # get the peer asking for route verification from its verify_key
-        context.node = cast(AbstractNode, context.node)
+
         peer = self.stash.get_for_verify_key(
             context.node.verify_key,
             context.credentials,
         )
         if peer.is_err():
             return SyftError(message=peer.err())
         peer = peer.ok()
@@ -320,15 +317,15 @@
     @service_method(
         path="network.get_all_peers", name="get_all_peers", roles=GUEST_ROLE_LEVEL
     )
     def get_all_peers(
         self, context: AuthedServiceContext
     ) -> list[NodePeer] | SyftError:
         """Get all Peers"""
-        context.node = cast(AbstractNode, context.node)
+
         result = self.stash.get_all(
             credentials=context.node.verify_key,
             order_by=OrderByNamePartitionKey,
         )
         if result.is_ok():
             peers = result.ok()
             return peers
@@ -337,15 +334,15 @@
     @service_method(
         path="network.get_peer_by_name", name="get_peer_by_name", roles=GUEST_ROLE_LEVEL
     )
     def get_peer_by_name(
         self, context: AuthedServiceContext, name: str
     ) -> NodePeer | None | SyftError:
         """Get Peer by Name"""
-        context.node = cast(AbstractNode, context.node)
+
         result = self.stash.get_by_name(
             credentials=context.node.verify_key,
             name=name,
         )
         if result.is_ok():
             peer = result.ok()
             return peer
@@ -355,15 +352,14 @@
         path="network.get_peers_by_type",
         name="get_peers_by_type",
         roles=GUEST_ROLE_LEVEL,
     )
     def get_peers_by_type(
         self, context: AuthedServiceContext, node_type: NodeType
     ) -> list[NodePeer] | SyftError:
-        context.node = cast(AbstractNode, context.node)
         result = self.stash.get_by_node_type(
             credentials=context.node.verify_key,
             node_type=node_type,
         )
 
         if result.is_err():
             return SyftError(message=str(result.err()))
@@ -392,15 +388,15 @@
     )
     def exchange_veilid_route(
         self,
         context: AuthedServiceContext,
         remote_node_route: NodeRoute,
     ) -> SyftSuccess | SyftError:
         """Exchange Route With Another Node"""
-        context.node = cast(AbstractNode, context.node)
+
         # Step 1: Get our own Veilid Node Peer to send to the remote node
         self_node_peer: NodePeer = context.node.settings.to(NodePeer)
 
         veilid_service = context.node.get_service("veilidservice")
         veilid_route = veilid_service.get_veilid_route(context=context)
 
         if isinstance(veilid_route, SyftError):
@@ -435,15 +431,15 @@
     )
     def add_veilid_peer(
         self,
         context: AuthedServiceContext,
         peer: NodePeer,
     ) -> NodePeer | SyftError:
         """Add a Veilid Node Peer"""
-        context.node = cast(AbstractNode, context.node)
+
         # Step 1: Using the verify_key of the peer to verify the signature
         # It is also our single source of truth for the peer
         if peer.verify_key != context.credentials:
             return SyftError(
                 message=(
                     f"The {type(peer)}.verify_key: "
                     f"{peer.verify_key} does not match the signature of the message"
```

### Comparing `syft-0.8.6b1/src/syft/service/network/node_peer.py` & `syft-0.8.7b1/src/syft/service/network/node_peer.py`

 * *Files 1% similar despite different names*

```diff
@@ -128,16 +128,14 @@
         # select the latest added route
         final_route = self.pick_highest_priority_route()
         connection = route_to_connection(route=final_route)
 
         client_type = connection.get_client_type()
         if isinstance(client_type, SyftError):
             return client_type
-        if context.node is None:
-            return SyftError(message=f"context {context}'s node is None")
         return client_type(connection=connection, credentials=context.node.signing_key)
 
     def client_with_key(self, credentials: SyftSigningKey) -> SyftClient:
         if len(self.node_routes) < 1:
             raise Exception(f"No routes to peer: {self}")
         # select the latest added route
         final_route = self.pick_highest_priority_route()
```

### Comparing `syft-0.8.6b1/src/syft/service/network/routes.py` & `syft-0.8.7b1/src/syft/service/network/routes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # future
 from __future__ import annotations
 
 # stdlib
 import secrets
 from typing import Any
 from typing import TYPE_CHECKING
-from typing import cast
 
 # third party
 from typing_extensions import Self
 
 # relative
 from ...abstract_node import AbstractNode
 from ...client.client import HTTPConnection
@@ -35,16 +34,14 @@
 
 class NodeRoute:
     def client_with_context(self, context: NodeServiceContext) -> SyftClient:
         connection = route_to_connection(route=self, context=context)
         client_type = connection.get_client_type()
         if isinstance(client_type, SyftError):
             return client_type
-        if context.node is None:
-            return SyftError(message=f"context {context}'s node is None")
         return client_type(connection=connection, credentials=context.node.signing_key)
 
     def validate_with_context(self, context: AuthedServiceContext) -> NodePeer:
         # relative
         from .node_peer import NodePeer
 
         # Step 1: Check if the given route is able to reach the given node
@@ -55,15 +52,14 @@
         random_challenge = secrets.token_bytes(16)
         challenge_signature = self_client.api.services.network.ping(random_challenge)
 
         if isinstance(challenge_signature, SyftError):
             return challenge_signature
 
         try:
-            context.node = cast(AbstractNode, context.node)
             # Verifying if the challenge is valid
             context.node.verify_key.verify_key.verify(
                 random_challenge, challenge_signature
             )
         except Exception:
             return SyftError(message="Signature Verification Failed in ping")
```

### Comparing `syft-0.8.6b1/src/syft/service/notification/email_templates.py` & `syft-0.8.7b1/src/syft/service/notification/email_templates.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # stdlib
 from typing import TYPE_CHECKING
 from typing import cast
 
 # relative
-from ...abstract_node import AbstractNode
 from ...store.linked_obj import LinkedObject
 from ..context import AuthedServiceContext
 
 if TYPE_CHECKING:
     # relative
     from .notifications import Notification
 
@@ -21,20 +20,18 @@
     def email_body(notification: "Notification", context: AuthedServiceContext) -> str:
         return ""
 
 
 class OnBoardEmailTemplate(EmailTemplate):
     @staticmethod
     def email_title(notification: "Notification", context: AuthedServiceContext) -> str:
-        context.node = cast(AbstractNode, context.node)
         return f"Welcome to {context.node.name} node!"
 
     @staticmethod
     def email_body(notification: "Notification", context: AuthedServiceContext) -> str:
-        context.node = cast(AbstractNode, context.node)
         user_service = context.node.get_service("userservice")
         admin_name = user_service.get_by_verify_key(
             user_service.admin_verify_key()
         ).name
 
         head = (
             f"""
@@ -109,23 +106,21 @@
         """
         return f"""<html>{head} {body}</html>"""
 
 
 class RequestEmailTemplate(EmailTemplate):
     @staticmethod
     def email_title(notification: "Notification", context: AuthedServiceContext) -> str:
-        context.node = cast(AbstractNode, context.node)
         notification.linked_obj = cast(LinkedObject, notification.linked_obj)
         request_obj = notification.linked_obj.resolve_with_context(context=context).ok()
 
         return f"Domain {context.node.name}: A New Request ({str(request_obj.id)[:4]}) has been received!"
 
     @staticmethod
     def email_body(notification: "Notification", context: AuthedServiceContext) -> str:
-        context.node = cast(AbstractNode, context.node)
         notification.linked_obj = cast(LinkedObject, notification.linked_obj)
         request_obj = notification.linked_obj.resolve_with_context(context=context).ok()
 
         head = """
         <head>
             <title>Access Request Notification</title>
             <style>
@@ -258,20 +253,18 @@
         """
         return f"""<html>{head} {body}</html>"""
 
 
 class RequestUpdateEmailTemplate(EmailTemplate):
     @staticmethod
     def email_title(notification: "Notification", context: AuthedServiceContext) -> str:
-        context.node = cast(AbstractNode, context.node)
         return f"Domain {context.node.name}: {notification.subject}"
 
     @staticmethod
     def email_body(notification: "Notification", context: AuthedServiceContext) -> str:
-        context.node = cast(AbstractNode, context.node)
         notification.linked_obj = cast(LinkedObject, notification.linked_obj)
         request_obj = notification.linked_obj.resolve_with_context(context=context).ok()
         badge_color = "red" if request_obj.status.name == "REJECTED" else "green"
         head = """
         <head>
             <title>Access Request Notification</title>
             <style>
```

### Comparing `syft-0.8.6b1/src/syft/service/notification/notification_service.py` & `syft-0.8.7b1/src/syft/service/notification/notification_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 # stdlib
-from typing import cast
 
 # relative
-from ...abstract_node import AbstractNode
 from ...serde.serializable import serializable
 from ...store.document_store import DocumentStore
 from ...types.uid import UID
 from ...util.telemetry import instrument
 from ..action.action_permissions import ActionObjectREAD
 from ..context import AuthedServiceContext
 from ..notifier.notifier import NotifierSettings
@@ -50,15 +48,15 @@
                 uid=new_notification.id, credentials=new_notification.to_user_verify_key
             )
         ]
 
         result = self.stash.set(
             context.credentials, new_notification, add_permissions=permissions
         )
-        context.node = cast(AbstractNode, context.node)
+
         notifier_service = context.node.get_service("notifierservice")
 
         res = notifier_service.dispatch_notification(context, new_notification)
         if isinstance(res, SyftError):
             return res
 
         if result.is_err():
@@ -94,56 +92,52 @@
         path="notifications.user_settings",
         name="user_settings",
     )
     def user_settings(
         self,
         context: AuthedServiceContext,
     ) -> NotifierSettings | SyftError:
-        context.node = cast(AbstractNode, context.node)
         notifier_service = context.node.get_service("notifierservice")
         return notifier_service.user_settings(context)
 
     @service_method(
         path="notifications.settings",
         name="settings",
         roles=ADMIN_ROLE_LEVEL,
     )
     def settings(
         self,
         context: AuthedServiceContext,
     ) -> NotifierSettings | SyftError:
-        context.node = cast(AbstractNode, context.node)
         notifier_service = context.node.get_service("notifierservice")
         result = notifier_service.settings(context)
         return result
 
     @service_method(
         path="notifications.activate",
         name="activate",
         roles=DATA_SCIENTIST_ROLE_LEVEL,
     )
     def activate(
         self,
         context: AuthedServiceContext,
     ) -> Notification | SyftError:
-        context.node = cast(AbstractNode, context.node)
         notifier_service = context.node.get_service("notifierservice")
         result = notifier_service.activate(context)
         return result
 
     @service_method(
         path="notifications.deactivate",
         name="deactivate",
         roles=DATA_SCIENTIST_ROLE_LEVEL,
     )
     def deactivate(
         self,
         context: AuthedServiceContext,
     ) -> Notification | SyftError:
-        context.node = cast(AbstractNode, context.node)
         notifier_service = context.node.get_service("notifierservice")
         result = notifier_service.deactivate(context)
         return result
 
     @service_method(
         path="notifications.get_all",
         name="get_all",
@@ -248,15 +242,14 @@
         path="notifications.resolve_object",
         name="resolve_object",
         roles=DATA_SCIENTIST_ROLE_LEVEL,
     )
     def resolve_object(
         self, context: AuthedServiceContext, linked_obj: LinkedObject
     ) -> Notification | SyftError:
-        context.node = cast(AbstractNode, context.node)
         service = context.node.get_service(linked_obj.service_type)
         result = service.resolve_link(context=context, linked_obj=linked_obj)
         if result.is_err():
             return SyftError(message=str(result.err()))
         return result.ok()
 
     @service_method(path="notifications.clear", name="clear")
```

### Comparing `syft-0.8.6b1/src/syft/service/notification/notification_stash.py` & `syft-0.8.7b1/src/syft/service/notification/notification_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6b1/src/syft/service/notification/notifications.py` & `syft-0.8.7b1/src/syft/service/notification/notifications.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6b1/src/syft/service/notifier/notifier.py` & `syft-0.8.7b1/src/syft/service/notifier/notifier.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 # stdlib
 
 # stdlib
 from typing import TypeVar
-from typing import cast
 
 # third party
 from result import Err
 from result import Ok
 from result import Result
 
 # relative
-from ...abstract_node import AbstractNode
 from ...node.credentials import SyftVerifyKey
 from ...serde.serializable import serializable
 from ...types.syft_object import SYFT_OBJECT_VERSION_1
 from ...types.syft_object import SyftObject
 from ..context import AuthedServiceContext
 from ..notification.notifications import Notification
 from ..response import SyftError
@@ -68,16 +66,14 @@
             password=password,
         )
 
     def send(
         self, context: AuthedServiceContext, notification: Notification
     ) -> Result[Ok, Err]:
         try:
-            context.node = cast(AbstractNode, context.node)
-
             user_service = context.node.get_service("userservice")
 
             receiver = user_service.get_by_verify_key(notification.to_user_verify_key)
 
             if not receiver.notifications_enabled[NOTIFIERS.EMAIL]:
                 return Ok(
                     "Email notifications are disabled for this user."
```

### Comparing `syft-0.8.6b1/src/syft/service/notifier/notifier_service.py` & `syft-0.8.7b1/src/syft/service/notifier/notifier_service.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 # stdlib
 
 # stdlib
-from typing import cast
 
 # third party
 from pydantic import EmailStr
 from result import Err
 from result import Ok
 from result import Result
 
@@ -50,15 +49,14 @@
 
         return result.ok()
 
     def user_settings(
         self,
         context: AuthedServiceContext,
     ) -> NotificationPreferences:
-        context.node = cast(AbstractNode, context.node)
         user_service = context.node.get_service("userservice")
         user_view = user_service.get_current_user(context)
         notifications = user_view.notifications_enabled
         return NotificationPreferences(
             email=notifications[NOTIFIERS.EMAIL],
             sms=notifications[NOTIFIERS.SMS],
             slack=notifications[NOTIFIERS.SLACK],
@@ -195,25 +193,25 @@
     def activate(
         self, context: AuthedServiceContext, notifier_type: NOTIFIERS = NOTIFIERS.EMAIL
     ) -> SyftSuccess | SyftError:
         """
         Activate email notifications for the authenticated user.
         This will only work if the domain owner has enabled notifications.
         """
-        context.node = cast(AbstractNode, context.node)
+
         user_service = context.node.get_service("userservice")
         return user_service.enable_notifications(context, notifier_type=notifier_type)
 
     def deactivate(
         self, context: AuthedServiceContext, notifier_type: NOTIFIERS = NOTIFIERS.EMAIL
     ) -> SyftSuccess | SyftError:
         """Deactivate email notifications for the authenticated user
         This will only work if the domain owner has enabled notifications.
         """
-        context.node = cast(AbstractNode, context.node)
+
         user_service = context.node.get_service("userservice")
         return user_service.disable_notifications(context, notifier_type=notifier_type)
 
     @staticmethod
     def init_notifier(
         node: AbstractNode,
         email_username: str | None = None,
@@ -268,29 +266,28 @@
                     )
                     notifier.active = False
                 else:
                     notifier.email_password = email_password
                     notifier.email_username = email_username
                     notifier.email_sender = email_sender
                     notifier.email_server = smtp_host
-                    notifier.email_port = int(smtp_port)
+                    notifier.email_port = smtp_port
                     notifier.active = True
 
             notifier_stash.set(node.signing_key.verify_key, notifier)
             return Ok("Notifier initialized successfully")
 
         except Exception as e:
             raise Exception(f"Error initializing notifier. \n {e}")
 
     # This is not a public API.
     # This method is used by other services to dispatch notifications internally
     def dispatch_notification(
         self, context: AuthedServiceContext, notification: Notification
     ) -> SyftError:
-        context.node = cast(AbstractNode, context.node)
         admin_key = context.node.get_service("userservice").admin_verify_key()
         notifier = self.stash.get(admin_key)
         if notifier.is_err():
             return SyftError(
                 message="The mail service ran out of quota or some notifications failed to be delivered.\n"
                 + "Please check the health of the mailing server."
             )
```

### Comparing `syft-0.8.6b1/src/syft/service/notifier/notifier_stash.py` & `syft-0.8.7b1/src/syft/service/settings/settings_stash.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,83 +1,57 @@
 # stdlib
 
 # third party
-from result import Err
-from result import Ok
 from result import Result
 
 # relative
 from ...node.credentials import SyftVerifyKey
 from ...serde.serializable import serializable
-from ...store.document_store import BaseStash
+from ...store.document_store import BaseUIDStoreStash
 from ...store.document_store import DocumentStore
 from ...store.document_store import PartitionKey
 from ...store.document_store import PartitionSettings
 from ...types.uid import UID
 from ...util.telemetry import instrument
 from ..action.action_permissions import ActionObjectPermission
-from .notifier import NotifierSettings
+from .settings import NodeSettingsV2
 
 NamePartitionKey = PartitionKey(key="name", type_=str)
 ActionIDsPartitionKey = PartitionKey(key="action_ids", type_=list[UID])
 
 
 @instrument
 @serializable()
-class NotifierStash(BaseStash):
-    object_type = NotifierSettings
+class SettingsStash(BaseUIDStoreStash):
+    object_type = NodeSettingsV2
     settings: PartitionSettings = PartitionSettings(
-        name=NotifierSettings.__canonical_name__, object_type=NotifierSettings
+        name=NodeSettingsV2.__canonical_name__, object_type=NodeSettingsV2
     )
 
     def __init__(self, store: DocumentStore) -> None:
         super().__init__(store=store)
 
-    def admin_verify_key(self) -> SyftVerifyKey:
-        return self.partition.root_verify_key
-
-    # TODO: should this method behave like a singleton?
-    def get(self, credentials: SyftVerifyKey) -> Result[NotifierSettings, Err]:
-        """Get Settings"""
-        result = self.get_all(credentials)
-        if result.is_ok():
-            settings = result.ok()
-            if len(settings) == 0:
-                return Ok(
-                    None
-                )  # TODO: Stash shouldn't be empty after init. Return Err instead?
-            result = settings[
-                0
-            ]  # TODO: Should we check if theres more than one? => Report corruption
-            return Ok(result)
-        else:
-            return Err(message=result.err())
-
     def set(
         self,
         credentials: SyftVerifyKey,
-        settings: NotifierSettings,
-        add_permissions: list[ActionObjectPermission] | None = None,
+        settings: NodeSettingsV2,
+        add_permission: list[ActionObjectPermission] | None = None,
         add_storage_permission: bool = True,
         ignore_duplicates: bool = False,
-    ) -> Result[NotifierSettings, Err]:
-        result = self.check_type(settings, self.object_type)
+    ) -> Result[NodeSettingsV2, str]:
+        res = self.check_type(settings, self.object_type)
         # we dont use and_then logic here as it is hard because of the order of the arguments
-        if result.is_err():
-            return Err(message=result.err())
-        return super().set(
-            credentials=credentials, obj=result.ok()
-        )  # TODO check if result isInstance(Ok)
+        if res.is_err():
+            return res
+        return super().set(credentials=credentials, obj=res.ok())
 
     def update(
         self,
         credentials: SyftVerifyKey,
-        settings: NotifierSettings,
+        settings: NodeSettingsV2,
         has_permission: bool = False,
-    ) -> Result[NotifierSettings, Err]:
-        result = self.check_type(settings, self.object_type)
+    ) -> Result[NodeSettingsV2, str]:
+        res = self.check_type(settings, self.object_type)
         # we dont use and_then logic here as it is hard because of the order of the arguments
-        if result.is_err():
-            return Err(message=result.err())
-        return super().update(
-            credentials=credentials, obj=result.ok()
-        )  # TODO check if result isInstance(Ok)
+        if res.is_err():
+            return res
+        return super().update(credentials=credentials, obj=res.ok())
```

### Comparing `syft-0.8.6b1/src/syft/service/notifier/smtp_client.py` & `syft-0.8.7b1/src/syft/service/notifier/smtp_client.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6b1/src/syft/service/object_search/migration_state_service.py` & `syft-0.8.7b1/src/syft/service/object_search/migration_state_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6b1/src/syft/service/object_search/object_migration_state.py` & `syft-0.8.7b1/src/syft/service/object_search/object_migration_state.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6b1/src/syft/service/output/output_service.py` & `syft-0.8.7b1/src/syft/service/output/output_service.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,78 +1,85 @@
 # stdlib
-from typing import Any
 from typing import ClassVar
 
 # third party
 from pydantic import model_validator
+from result import Err
+from result import Ok
 from result import Result
 
 # relative
 from ...client.api import APIRegistry
 from ...node.credentials import SyftVerifyKey
 from ...serde.serializable import serializable
 from ...store.document_store import BaseUIDStoreStash
 from ...store.document_store import DocumentStore
 from ...store.document_store import PartitionKey
 from ...store.document_store import PartitionSettings
 from ...store.document_store import QueryKeys
 from ...store.linked_obj import LinkedObject
 from ...types.datetime import DateTime
-from ...types.syft_object import SYFT_OBJECT_VERSION_1
+from ...types.syft_object import SYFT_OBJECT_VERSION_2
 from ...types.syncable_object import SyncableSyftObject
 from ...types.uid import UID
 from ...util.telemetry import instrument
 from ..action.action_object import ActionObject
 from ..context import AuthedServiceContext
 from ..response import SyftError
 from ..service import AbstractService
 from ..service import TYPE_TO_SERVICE
 from ..service import service_method
+from ..user.user_roles import ADMIN_ROLE_LEVEL
 from ..user.user_roles import GUEST_ROLE_LEVEL
 
 CreatedAtPartitionKey = PartitionKey(key="created_at", type_=DateTime)
 UserCodeIdPartitionKey = PartitionKey(key="user_code_id", type_=UID)
+JobIdPartitionKey = PartitionKey(key="job_id", type_=UID)
 OutputPolicyIdPartitionKey = PartitionKey(key="output_policy_id", type_=UID)
 
 
 @serializable()
 class ExecutionOutput(SyncableSyftObject):
     __canonical_name__ = "ExecutionOutput"
-    __version__ = SYFT_OBJECT_VERSION_1
+    __version__ = SYFT_OBJECT_VERSION_2
 
     executing_user_verify_key: SyftVerifyKey
     user_code_link: LinkedObject
     output_ids: list[UID] | dict[str, UID] | None = None
     job_link: LinkedObject | None = None
     created_at: DateTime = DateTime.now()
     input_ids: dict[str, UID] | None = None
 
     # Required for __attr_searchable__, set by model_validator
     user_code_id: UID
+    job_id: UID | None = None
 
     # Output policy is not a linked object because its saved on the usercode
     output_policy_id: UID | None = None
 
     __attr_searchable__: ClassVar[list[str]] = [
         "user_code_id",
         "created_at",
         "output_policy_id",
+        "job_id",
     ]
     __repr_attrs__: ClassVar[list[str]] = [
         "created_at",
         "user_code_id",
         "job_id",
         "output_ids",
     ]
 
     @model_validator(mode="before")
     @classmethod
-    def add_user_code_id(cls, values: dict) -> dict:
+    def add_searchable_link_ids(cls, values: dict) -> dict:
         if "user_code_link" in values:
             values["user_code_id"] = values["user_code_link"].object_uid
+        if values.get("job_link"):
+            values["job_id"] = values["job_link"].object_uid
         return values
 
     @classmethod
     def from_ids(
         cls: type["ExecutionOutput"],
         output_ids: UID | list[UID] | dict[str, UID],
         user_code_id: UID,
@@ -165,19 +172,15 @@
         if not self.input_ids:
             return True
         for key, value in kwargs.items():  # Iterate over items of kwargs dictionary
             if key not in self.input_ids or self.input_ids[key] != value:
                 return False
         return True
 
-    @property
-    def job_id(self) -> UID | None:
-        return self.job_link.object_uid if self.job_link else None
-
-    def get_sync_dependencies(self, api: Any = None) -> list[UID]:
+    def get_sync_dependencies(self, context: AuthedServiceContext) -> list[UID]:
         # Output ids, user code id, job id
         res = []
 
         res.extend(self.output_id_list)
         res.append(self.user_code_id)
         if self.job_id:
             res.append(self.job_id)
@@ -205,14 +208,34 @@
         qks = QueryKeys(
             qks=[UserCodeIdPartitionKey.with_obj(user_code_id)],
         )
         return self.query_all(
             credentials=credentials, qks=qks, order_by=CreatedAtPartitionKey
         )
 
+    def get_by_job_id(
+        self, credentials: SyftVerifyKey, user_code_id: UID
+    ) -> Result[ExecutionOutput | None, str]:
+        qks = QueryKeys(
+            qks=[JobIdPartitionKey.with_obj(user_code_id)],
+        )
+        res = self.query_all(
+            credentials=credentials, qks=qks, order_by=CreatedAtPartitionKey
+        )
+        if res.is_err():
+            return res
+        else:
+            res = res.ok()
+            if len(res) == 0:
+                return Ok(None)
+            elif len(res) > 1:
+                return Err(message="Too many outputs found")
+            else:
+                return Ok(res[0])
+
     def get_by_output_policy_id(
         self, credentials: SyftVerifyKey, output_policy_id: UID
     ) -> Result[list[ExecutionOutput], str]:
         qks = QueryKeys(
             qks=[OutputPolicyIdPartitionKey.with_obj(output_policy_id)],
         )
         return self.query_all(
@@ -270,14 +293,30 @@
             credentials=context.node.verify_key,  # type: ignore
             user_code_id=user_code_id,
         )
         if result.is_ok():
             return result.ok()
         return SyftError(message=result.err())
 
+    @service_method(
+        path="output.get_by_job_id",
+        name="get_by_job_id",
+        roles=ADMIN_ROLE_LEVEL,
+    )
+    def get_by_job_id(
+        self, context: AuthedServiceContext, user_code_id: UID
+    ) -> ExecutionOutput | None | SyftError:
+        result = self.stash.get_by_job_id(
+            credentials=context.node.verify_key,  # type: ignore
+            user_code_id=user_code_id,
+        )
+        if result.is_ok():
+            return result.ok()
+        return SyftError(message=result.err())
+
     @service_method(
         path="output.get_by_output_policy_id",
         name="get_by_output_policy_id",
         roles=GUEST_ROLE_LEVEL,
     )
     def get_by_output_policy_id(
         self, context: AuthedServiceContext, output_policy_id: UID
```

### Comparing `syft-0.8.6b1/src/syft/service/policy/policy.py` & `syft-0.8.7b1/src/syft/service/policy/policy.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,24 +10,22 @@
 import inspect
 from inspect import Parameter
 from inspect import Signature
 from io import StringIO
 import sys
 import types
 from typing import Any
-from typing import cast
 
 # third party
 from RestrictedPython import compile_restricted
 from result import Err
 from result import Ok
 from result import Result
 
 # relative
-from ...abstract_node import AbstractNode
 from ...abstract_node import NodeType
 from ...client.api import APIRegistry
 from ...client.api import NodeIdentity
 from ...node.credentials import SyftVerifyKey
 from ...serde.recursive_primitives import recursive_serde_register_type
 from ...serde.serializable import serializable
 from ...store.document_store import PartitionKey
@@ -127,26 +125,29 @@
     APPROVED = "approved"
 
 
 def partition_by_node(kwargs: dict[str, Any]) -> dict[NodeIdentity, dict[str, UID]]:
     # relative
     from ...client.api import APIRegistry
     from ...client.api import NodeIdentity
+    from ...client.api import RemoteFunction
     from ...types.twin_object import TwinObject
     from ..action.action_object import ActionObject
 
     # fetches the all the current api's connected
     api_list = APIRegistry.get_all_api()
     output_kwargs = {}
     for k, v in kwargs.items():
         uid = v
         if isinstance(v, ActionObject):
             uid = v.id
         if isinstance(v, TwinObject):
             uid = v.id
+        if isinstance(v, RemoteFunction):
+            uid = v.custom_function_id()
         if isinstance(v, Asset):
             uid = v.action_id
         if not isinstance(uid, UID):
             raise Exception(f"Input {k} must have a UID not {type(v)}")
 
         _obj_exists = False
         for api in api_list:
@@ -198,16 +199,14 @@
     @property
     def inputs(self) -> dict[NodeIdentity, Any]:
         return self.init_kwargs
 
     def _inputs_for_context(self, context: ChangeContext) -> dict | SyftError:
         user_node_view = NodeIdentity.from_change_context(context)
         inputs = self.inputs[user_node_view]
-        if context.node is None:
-            return SyftError(f"context {context}'s node is None")
         root_context = AuthedServiceContext(
             node=context.node, credentials=context.approving_user_credentials
         ).as_root_context()
 
         action_service = context.node.get_service("actionservice")
         for var_name, uid in inputs.items():
             action_object = action_service.get(uid=uid, context=root_context)
@@ -226,16 +225,14 @@
 
 def retrieve_from_db(
     code_item_id: UID, allowed_inputs: dict[str, UID], context: AuthedServiceContext
 ) -> Result[dict[str, Any], str]:
     # relative
     from ...service.action.action_object import TwinMode
 
-    context.node = cast(AbstractNode, context.node)
-
     action_service = context.node.get_service("actionservice")
     code_inputs = {}
 
     # When we are retrieving the code from the database, we need to use the node's
     # verify key as the credentials. This is because when we approve the code, we
     # we allow the private data to be used only for this specific code.
     # but we are not modifying the permissions of the private data
@@ -270,15 +267,14 @@
 
 
 def allowed_ids_only(
     allowed_inputs: dict[NodeIdentity, Any],
     kwargs: dict[str, Any],
     context: AuthedServiceContext,
 ) -> dict[str, UID]:
-    context.node = cast(AbstractNode, context.node)
     if context.node.node_type == NodeType.DOMAIN:
         node_identity = NodeIdentity(
             node_name=context.node.name,
             node_id=context.node.id,
             verify_key=context.node.signing_key.verify_key,
         )
         allowed_inputs = allowed_inputs.get(node_identity, {})
@@ -382,18 +378,19 @@
     __canonical_name__ = "OutputPolicy"
     __version__ = SYFT_OBJECT_VERSION_2
 
     output_kwargs: list[str] = []
     node_uid: UID | None = None
     output_readers: list[SyftVerifyKey] = []
 
-    def apply_output(
+    def apply_to_output(
         self,
         context: NodeServiceContext,
         outputs: Any,
+        update_policy: bool = True,
     ) -> Any:
         # output_uids: Union[Dict[str, Any], list] = filter_only_uids(outputs)
         # if isinstance(output_uids, UID):
         #     output_uids = [output_uids]
         # history = OutputHistory(
         #     output_time=DateTime.now(),
         #     outputs=output_uids,
@@ -436,15 +433,14 @@
                 message=f"Policy is still valid. count: {execution_count} < limit: {self.limit}"
             )
         return SyftError(
             message=f"Policy is no longer valid. count: {execution_count} >= limit: {self.limit}"
         )
 
     def _is_valid(self, context: AuthedServiceContext) -> SyftSuccess | SyftError:
-        context.node = cast(AbstractNode, context.node)
         output_service = context.node.get_service("outputservice")
         output_history = output_service.get_by_output_policy_id(context, self.id)
         if isinstance(output_history, SyftError):
             return output_history
         execution_count = len(output_history)
 
         is_valid = execution_count < self.limit
@@ -481,18 +477,19 @@
 
 
 recursive_serde_register_type(CustomPolicy)
 
 
 @serializable()
 class CustomOutputPolicy(metaclass=CustomPolicy):
-    def apply_output(
+    def apply_to_output(
         self,
         context: NodeServiceContext,
         outputs: Any,
+        update_policy: bool = True,
     ) -> Any | None:
         return outputs
 
 
 class UserOutputPolicy(OutputPolicy):
     __canonical_name__ = "UserOutputPolicy"
 
@@ -538,18 +535,19 @@
     def byte_code(self) -> PyCodeObject | None:
         return compile_byte_code(self.parsed_code)
 
     @property
     def policy_code(self) -> str:
         return self.raw_code
 
-    def apply_output(
+    def apply_to_output(
         self,
         context: NodeServiceContext,
         outputs: Any,
+        update_policy: bool = True,
     ) -> Any | None:
         return outputs
 
 
 def new_getfile(object: Any) -> Any:  # TODO: fix the mypy issue
     if not inspect.isclass(object):
         return inspect.getfile(object)
@@ -724,15 +722,15 @@
         print("failed to unparse", e)
         raise e
 
 
 def check_class_code(context: TransformContext) -> TransformContext:
     # TODO: define the proper checking for this case based on the ideas from UserCode
     # check for no globals
-    # check for Policy template -> __init__, apply_output, public_state
+    # check for Policy template -> __init__, apply_to_output, public_state
     # parse init signature
     # check dangerous libraries, maybe compile_restricted already does that
     if context.output is None:
         return context
 
     try:
         processed_code = process_class_code(
```

### Comparing `syft-0.8.6b1/src/syft/service/policy/policy_service.py` & `syft-0.8.7b1/src/syft/service/policy/policy_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6b1/src/syft/service/policy/user_policy_stash.py` & `syft-0.8.7b1/src/syft/service/policy/user_policy_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6b1/src/syft/service/project/project.py` & `syft-0.8.7b1/src/syft/service/project/project.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6b1/src/syft/service/project/project_service.py` & `syft-0.8.7b1/src/syft/service/project/project_service.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 # stdlib
-from typing import cast
 
 # relative
-from ...abstract_node import AbstractNode
 from ...serde.serializable import serializable
 from ...store.document_store import DocumentStore
 from ...store.linked_obj import LinkedObject
 from ...types.uid import UID
 from ...util.telemetry import instrument
 from ..context import AuthedServiceContext
 from ..notification.notification_service import NotificationService
@@ -41,15 +39,14 @@
 
     @service_method(
         path="project.can_create_project",
         name="can_create_project",
         roles=ONLY_DATA_SCIENTIST_ROLE_LEVEL,
     )
     def can_create_project(self, context: AuthedServiceContext) -> bool | SyftError:
-        context.node = cast(AbstractNode, context.node)
         user_service = context.node.get_service("userservice")
         role = user_service.get_role_for_credentials(credentials=context.credentials)
         if role == ServiceRole.DATA_SCIENTIST:
             return True
         return SyftError(message="User cannot create projects")
 
     @service_method(
@@ -62,16 +59,14 @@
     ) -> SyftSuccess | SyftError:
         """Start a Project"""
 
         check_role = self.can_create_project(context)
         if isinstance(check_role, SyftError):
             return check_role
 
-        context.node = cast(AbstractNode, context.node)
-
         try:
             # Check if the project with given id already exists
             project_id_check = self.stash.get_by_uid(
                 credentials=context.node.verify_key, uid=project.id
             )
 
             if project_id_check.is_err():
@@ -147,15 +142,15 @@
         name="add_event",
         roles=GUEST_ROLE_LEVEL,
     )
     def add_event(
         self, context: AuthedServiceContext, project_event: ProjectEvent
     ) -> SyftSuccess | SyftError:
         """To add events to a projects"""
-        context.node = cast(AbstractNode, context.node)
+
         # Event object should be received from the leader of the project
 
         # retrieve the project object by node verify key
         project_obj = self.stash.get_by_uid(
             context.node.verify_key, uid=project_event.project_id
         )
         if project_obj.is_err():
@@ -193,15 +188,15 @@
     def broadcast_event(
         self, context: AuthedServiceContext, project_event: ProjectEvent
     ) -> SyftSuccess | SyftError:
         """To add events to a projects"""
         # Only the leader of the project could add events to the projects
         # Any Event to be added to the project should be sent to the leader of the project
         # The leader broadcasts the event to all the members of the project
-        context.node = cast(AbstractNode, context.node)
+
         project_obj = self.stash.get_by_uid(
             context.node.verify_key, uid=project_event.project_id
         )
 
         if project_obj.is_err():
             return SyftError(message=str(project_obj.err()))
 
@@ -260,15 +255,15 @@
         name="sync",
         roles=GUEST_ROLE_LEVEL,
     )
     def sync(
         self, context: AuthedServiceContext, project_id: UID, seq_no: int
     ) -> list[ProjectEvent] | SyftError:
         """To fetch unsynced events from the project"""
-        context.node = cast(AbstractNode, context.node)
+
         # Event object should be received from the leader of the project
 
         # retrieve the project object by node verify key
         project_obj = self.stash.get_by_uid(context.node.verify_key, uid=project_id)
         if project_obj.is_err():
             return SyftError(message=str(project_obj.err()))
 
@@ -325,15 +320,14 @@
         path="project.get_by_uid",
         name="get_by_uid",
         roles=GUEST_ROLE_LEVEL,
     )
     def get_by_uid(
         self, context: AuthedServiceContext, uid: UID
     ) -> Project | SyftError:
-        context.node = cast(AbstractNode, context.node)
         result = self.stash.get_by_uid(
             credentials=context.node.verify_key,
             uid=uid,
         )
         if result.is_err():
             return SyftError(message=str(result.err()))
         elif result.ok():
@@ -341,15 +335,15 @@
         return SyftError(message=f'Project(id="{uid}") does not exist')
 
     def add_signing_key_to_project(
         self, context: AuthedServiceContext, project: Project
     ) -> Project | SyftError:
         # Automatically infuse signing key of user
         # requesting get_all() or creating the project object
-        context.node = cast(AbstractNode, context.node)
+
         user_service = context.node.get_service("userservice")
         user = user_service.stash.get_by_verify_key(
             credentials=context.credentials, verify_key=context.credentials
         )
         if user.is_err():
             return SyftError(message=str(user.err()))
 
@@ -373,15 +367,15 @@
             project (Project): Project object
             project_event (ProjectEvent): Project event object
             context (AuthedServiceContext): Context of the node
 
         Returns:
             Union[SyftSuccess, SyftError]: SyftSuccess if message is created else SyftError
         """
-        context.node = cast(AbstractNode, context.node)
+
         if (
             isinstance(project_event, ProjectRequest)
             and project_event.linked_request.node_uid == context.node.id
         ):
             link = LinkedObject.with_context(project, context=context)
             message = CreateNotification(
                 subject=f"A new request has been added to the Project: {project.name}.",
```

### Comparing `syft-0.8.6b1/src/syft/service/project/project_stash.py` & `syft-0.8.7b1/src/syft/service/project/project_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6b1/src/syft/service/queue/base_queue.py` & `syft-0.8.7b1/src/syft/service/queue/base_queue.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6b1/src/syft/service/queue/queue.py` & `syft-0.8.7b1/src/syft/service/queue/queue.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6b1/src/syft/service/queue/queue_service.py` & `syft-0.8.7b1/src/syft/service/queue/queue_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6b1/src/syft/service/queue/queue_stash.py` & `syft-0.8.7b1/src/syft/service/queue/queue_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6b1/src/syft/service/queue/zmq_queue.py` & `syft-0.8.7b1/src/syft/service/queue/zmq_queue.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6b1/src/syft/service/request/request.py` & `syft-0.8.7b1/src/syft/service/request/request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 # stdlib
 from collections.abc import Callable
 from enum import Enum
 import hashlib
 import inspect
 from typing import Any
-from typing import cast
 
 # third party
 from result import Err
 from result import Ok
 from result import Result
 from typing_extensions import Self
 
 # relative
-from ...abstract_node import AbstractNode
 from ...abstract_node import NodeSideType
 from ...client.api import APIRegistry
 from ...client.client import SyftClient
 from ...custom_worker.config import WorkerConfig
 from ...custom_worker.k8s import IN_KUBERNETES
 from ...node.credentials import SyftVerifyKey
 from ...serde.serializable import serializable
@@ -50,14 +48,15 @@
 from ..code.user_code import UserCodeStatusCollection
 from ..context import AuthedServiceContext
 from ..context import ChangeContext
 from ..job.job_stash import Job
 from ..job.job_stash import JobInfo
 from ..job.job_stash import JobStatus
 from ..notification.notifications import Notification
+from ..policy.policy import UserPolicy
 from ..response import SyftError
 from ..response import SyftSuccess
 from ..user.user import UserView
 
 
 @serializable()
 class RequestStatus(Enum):
@@ -101,16 +100,14 @@
 
     __repr_attrs__ = ["linked_obj", "apply_permission_type"]
 
     def _run(
         self, context: ChangeContext, apply: bool
     ) -> Result[SyftSuccess, SyftError]:
         try:
-            if context.node is None:
-                return Err(SyftError(message=f"context {context}'s node is None"))
             action_service: ActionService = context.node.get_service(ActionService)  # type: ignore[assignment]
             blob_storage_service = context.node.get_service(BlobStorageService)
             action_store = action_service.store
 
             # can we ever have a lineage ID in the store?
             obj_uid = self.linked_obj.object_uid
             obj_uid = obj_uid.id if isinstance(obj_uid, LineageID) else obj_uid
@@ -201,17 +198,14 @@
 
     __repr_attrs__ = ["config", "tag"]
 
     def _run(
         self, context: ChangeContext, apply: bool
     ) -> Result[SyftSuccess, SyftError]:
         try:
-            if context.node is None:
-                return Err(SyftError(message=f"context {context}'s node is None"))
-
             worker_image_service = context.node.get_service("SyftWorkerImageService")
 
             service_context = context.to_service_ctx()
             result = worker_image_service.submit_dockerfile(
                 service_context, docker_config=self.config
             )
 
@@ -289,16 +283,14 @@
         This function is run when the DO approves (apply=True)
         or deny (apply=False) the request.
         """
         # TODO: refactor the returned Err(SyftError) or Ok(SyftSuccess) to just
         # SyftError or SyftSuccess
         if apply:
             # get the worker pool service and try to launch a pool
-            if context.node is None:
-                return Err(SyftError(message=f"context {context}'s node is None"))
             worker_pool_service = context.node.get_service("SyftWorkerPoolService")
             service_context: AuthedServiceContext = context.to_service_ctx()
 
             if self.config is not None:
                 result = worker_pool_service.image_stash.get_by_docker_config(
                     service_context.credentials, self.config
                 )
@@ -363,14 +355,15 @@
     __repr_attrs__ = [
         "request_time",
         "updated_at",
         "status",
         "changes",
         "requesting_user_verify_key",
     ]
+    __exclude_sync_diff_attrs__ = ["node_uid"]
 
     def _repr_html_(self) -> Any:
         # add changes
         updated_at_line = ""
         if self.updated_at is not None:
             updated_at_line += (
                 f"<p><strong>Created by: </strong>{self.requesting_user_name}</p>"
@@ -633,15 +626,14 @@
         self = result
         return Ok(SyftSuccess(message=f"Request {self.id} changes undone."))
 
     def save(self, context: AuthedServiceContext) -> Result[SyftSuccess, SyftError]:
         # relative
         from .request_service import RequestService
 
-        context.node = cast(AbstractNode, context.node)
         save_method = context.node.get_service_method(RequestService.save)
         return save_method(context=context, request=self)
 
     def _get_latest_or_create_job(self) -> Job | SyftError:
         """Get the latest job for this requests user_code, or creates one if no jobs exist"""
         api = APIRegistry.api_for(self.node_uid, self.syft_client_verify_key)
         if api is None:
@@ -708,14 +700,26 @@
                 includes_metadata=True,
                 includes_result=True,
                 status=JobStatus.COMPLETED,
                 resolved=True,
             )
 
         user_code_status_change: UserCodeStatusChange = self.changes[0]
+        code = user_code_status_change.code
+        output_history = code.output_history
+        if isinstance(output_history, SyftError):
+            return output_history
+        output_policy = code.output_policy
+        if isinstance(output_policy, SyftError):
+            return output_policy
+        if isinstance(user_code_status_change.code.output_policy_type, UserPolicy):
+            return SyftError(
+                message="UserCode uses an user-submitted custom policy. Please use .approve()"
+            )
+
         if not user_code_status_change.change_object_is_type(UserCodeStatusCollection):
             raise TypeError(
                 f"accept_by_depositing_result can only be run on {UserCodeStatusCollection} not "
                 f"{user_code_status_change.linked_obj.object_type}"
             )
         if not type(user_code_status_change) == UserCodeStatusChange:
             raise TypeError(
@@ -732,21 +736,14 @@
             raise ValueError(f"{api}'s signing key is None")
         is_approved = user_code_status_change.approved
 
         permission_request = self.approve(approve_nested=True)
         if isinstance(permission_request, SyftError):
             return permission_request
 
-        code = user_code_status_change.code
-        output_history = code.output_history
-        if isinstance(output_history, SyftError):
-            return output_history
-        output_policy = code.output_policy
-        if isinstance(output_policy, SyftError):
-            return output_policy
         job = self._get_latest_or_create_job()
         if isinstance(job, SyftError):
             return job
 
         # This weird order is due to the fact that state is None before calling approve
         # we could fix it in a future release
         if is_approved:
@@ -838,15 +835,15 @@
                 return approved
 
             input_ids = {}
             if code.input_policy is not None:
                 for inps in code.input_policy.inputs.values():
                     input_ids.update(inps)
 
-            res = api.services.code.apply_output(
+            res = api.services.code.store_as_history(
                 user_code_id=code.id,
                 outputs=result,
                 job_id=job.id,
                 input_ids=input_ids,
             )
             if isinstance(res, SyftError):
                 return res
@@ -881,15 +878,17 @@
             return SyftError(message=f"api is None. You must login to {self.node_uid}")
         job_service = api.services.job
 
         job = self._get_latest_or_create_job()
         job.apply_info(job_info)
         return job_service.update(job)
 
-    def get_sync_dependencies(self, api: Any = None) -> list[UID] | SyftError:
+    def get_sync_dependencies(
+        self, context: AuthedServiceContext
+    ) -> list[UID] | SyftError:
         dependencies = []
 
         code_id = self.code_id
         if isinstance(code_id, SyftError):
             return code_id
 
         dependencies.append(code_id)
@@ -1248,16 +1247,14 @@
 
     def mutate(
         self,
         status: UserCodeStatusCollection,
         context: ChangeContext,
         undo: bool,
     ) -> UserCodeStatusCollection | SyftError:
-        if context.node is None:
-            return SyftError(message=f"context {context}'s node is None")
         reason: str = context.extra_kwargs.get("reason", "")
 
         if not undo:
             res = status.mutate(
                 value=(self.value, reason),
                 node_name=context.node.name,
                 node_id=context.node.id,
```

### Comparing `syft-0.8.6b1/src/syft/service/request/request_service.py` & `syft-0.8.7b1/src/syft/service/request/request_service.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 # stdlib
-from typing import cast
 
 # third party
 from result import Err
 from result import Ok
 
 # relative
-from ...abstract_node import AbstractNode
 from ...serde.serializable import serializable
 from ...store.document_store import DocumentStore
 from ...store.linked_obj import LinkedObject
 from ...types.uid import UID
 from ...util.telemetry import instrument
 from ..action.action_permissions import ActionObjectPermission
 from ..action.action_permissions import ActionPermission
@@ -69,15 +67,15 @@
                         uid=req.id, permission=ActionPermission.ALL_READ
                     ),
                 ],
             )
             if result.is_ok():
                 request = result.ok()
                 link = LinkedObject.with_context(request, context=context)
-                context.node = cast(AbstractNode, context.node)
+
                 admin_verify_key = context.node.get_service_method(
                     UserService.admin_verify_key
                 )
 
                 root_verify_key = admin_verify_key()
                 if send_message:
                     subject_msg = f"Result to request {str(request.id)[:4]}...{str(request.id)[-3:]}\
@@ -121,15 +119,15 @@
     def get_all_info(
         self,
         context: AuthedServiceContext,
         page_index: int | None = 0,
         page_size: int | None = 0,
     ) -> list[list[RequestInfo]] | list[RequestInfo] | SyftError:
         """Get the information of all requests"""
-        context.node = cast(AbstractNode, context.node)
+
         result = self.stash.get_all(context.credentials)
         if result.is_err():
             return SyftError(message=result.err())
 
         method = context.node.get_service_method(UserService.get_by_verify_key)
         get_message = context.node.get_service_method(NotificationService.filter_by_obj)
 
@@ -196,15 +194,14 @@
     )
     def apply(
         self,
         context: AuthedServiceContext,
         uid: UID,
         **kwargs: dict,
     ) -> SyftSuccess | SyftError:
-        context.node = cast(AbstractNode, context.node)
         request = self.stash.get_by_uid(context.credentials, uid)
         if request.is_ok():
             request = request.ok()
 
             context.extra_kwargs = kwargs
             result = request.apply(context=context)
 
@@ -271,15 +268,15 @@
             subject=message_subject,
             from_user_verify_key=context.credentials,
             to_user_verify_key=request.requesting_user_verify_key,
             linked_obj=link,
             notifier_types=[NOTIFIERS.EMAIL],
             email_template=RequestUpdateEmailTemplate,
         )
-        context.node = cast(AbstractNode, context.node)
+
         send_notification = context.node.get_service_method(NotificationService.send)
         send_notification(context=context, notification=notification)
 
         return SyftSuccess(message=f"Request {uid} successfully denied !")
 
     def save(
         self, context: AuthedServiceContext, request: Request
```

### Comparing `syft-0.8.6b1/src/syft/service/request/request_stash.py` & `syft-0.8.7b1/src/syft/service/request/request_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6b1/src/syft/service/response.py` & `syft-0.8.7b1/src/syft/service/response.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6b1/src/syft/service/service.py` & `syft-0.8.7b1/src/syft/service/service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6b1/src/syft/service/settings/settings.py` & `syft-0.8.7b1/src/syft/service/settings/settings.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6b1/src/syft/service/settings/settings_service.py` & `syft-0.8.7b1/src/syft/service/settings/settings_service.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 # stdlib
 
 # stdlib
-from typing import cast
 
 # third party
 from result import Err
 from result import Ok
 from result import Result
 
 # relative
-from ...abstract_node import AbstractNode
 from ...serde.serializable import serializable
 from ...store.document_store import DocumentStore
 from ...util.experimental_flags import flags
 from ..context import AuthedServiceContext
 from ..context import UnauthedServiceContext
 from ..response import SyftError
 from ..response import SyftSuccess
@@ -34,15 +32,15 @@
     def __init__(self, store: DocumentStore) -> None:
         self.store = store
         self.stash = SettingsStash(store=store)
 
     @service_method(path="settings.get", name="get")
     def get(self, context: UnauthedServiceContext) -> Result[Ok, Err]:
         """Get Settings"""
-        context.node = cast(AbstractNode, context.node)
+
         result = self.stash.get_all(context.node.signing_key.verify_key)
         if result.is_ok():
             settings = result.ok()
             # check if the settings list is empty
             if len(settings) == 0:
                 return SyftError(message="No settings found")
             result = settings[0]
@@ -93,15 +91,14 @@
         context: AuthedServiceContext,
         email_username: str | None = None,
         email_password: str | None = None,
         email_sender: str | None = None,
         email_server: str | None = None,
         email_port: str | None = None,
     ) -> SyftSuccess | SyftError:
-        context.node = cast(AbstractNode, context.node)
         notifier_service = context.node.get_service("notifierservice")
         return notifier_service.turn_on(
             context=context,
             email_username=email_username,
             email_password=email_password,
             email_sender=email_sender,
             email_server=email_server,
@@ -113,29 +110,28 @@
         name="disable_notifications",
         roles=ADMIN_ROLE_LEVEL,
     )
     def disable_notifications(
         self,
         context: AuthedServiceContext,
     ) -> SyftSuccess | SyftError:
-        context.node = cast(AbstractNode, context.node)
         notifier_service = context.node.get_service("notifierservice")
         return notifier_service.turn_off(context=context)
 
     @service_method(
         path="settings.allow_guest_signup",
         name="allow_guest_signup",
         warning=HighSideCRUDWarning(confirmation=True),
     )
     def allow_guest_signup(
         self, context: AuthedServiceContext, enable: bool
     ) -> SyftSuccess | SyftError:
         """Enable/Disable Registration for Data Scientist or Guest Users."""
         flags.CAN_REGISTER = enable
-        context.node = cast(AbstractNode, context.node)
+
         method = context.node.get_service_method(SettingsService.update)
         settings = NodeSettingsUpdate(signup_enabled=enable)
 
         result = method(context=context, settings=settings)
 
         if result.is_err():
             return SyftError(message=f"Failed to update settings: {result.err()}")
```

### Comparing `syft-0.8.6b1/src/syft/service/settings/settings_stash.py` & `syft-0.8.7b1/src/syft/service/worker/worker_pool_stash.py`

 * *Files 19% similar despite different names*

```diff
@@ -6,52 +6,60 @@
 # relative
 from ...node.credentials import SyftVerifyKey
 from ...serde.serializable import serializable
 from ...store.document_store import BaseUIDStoreStash
 from ...store.document_store import DocumentStore
 from ...store.document_store import PartitionKey
 from ...store.document_store import PartitionSettings
+from ...store.document_store import QueryKeys
 from ...types.uid import UID
-from ...util.telemetry import instrument
 from ..action.action_permissions import ActionObjectPermission
-from .settings import NodeSettingsV2
+from ..action.action_permissions import ActionPermission
+from .worker_pool import WorkerPool
 
-NamePartitionKey = PartitionKey(key="name", type_=str)
-ActionIDsPartitionKey = PartitionKey(key="action_ids", type_=list[UID])
+PoolNamePartitionKey = PartitionKey(key="name", type_=str)
+PoolImageIDPartitionKey = PartitionKey(key="image_id", type_=UID)
 
 
-@instrument
 @serializable()
-class SettingsStash(BaseUIDStoreStash):
-    object_type = NodeSettingsV2
+class SyftWorkerPoolStash(BaseUIDStoreStash):
+    object_type = WorkerPool
     settings: PartitionSettings = PartitionSettings(
-        name=NodeSettingsV2.__canonical_name__, object_type=NodeSettingsV2
+        name=WorkerPool.__canonical_name__,
+        object_type=WorkerPool,
     )
 
     def __init__(self, store: DocumentStore) -> None:
         super().__init__(store=store)
 
+    def get_by_name(
+        self, credentials: SyftVerifyKey, pool_name: str
+    ) -> Result[WorkerPool | None, str]:
+        qks = QueryKeys(qks=[PoolNamePartitionKey.with_obj(pool_name)])
+        return self.query_one(credentials=credentials, qks=qks)
+
     def set(
         self,
         credentials: SyftVerifyKey,
-        settings: NodeSettingsV2,
-        add_permission: list[ActionObjectPermission] | None = None,
+        obj: WorkerPool,
+        add_permissions: list[ActionObjectPermission] | None = None,
         add_storage_permission: bool = True,
         ignore_duplicates: bool = False,
-    ) -> Result[NodeSettingsV2, str]:
-        res = self.check_type(settings, self.object_type)
-        # we dont use and_then logic here as it is hard because of the order of the arguments
-        if res.is_err():
-            return res
-        return super().set(credentials=credentials, obj=res.ok())
-
-    def update(
-        self,
-        credentials: SyftVerifyKey,
-        settings: NodeSettingsV2,
-        has_permission: bool = False,
-    ) -> Result[NodeSettingsV2, str]:
-        res = self.check_type(settings, self.object_type)
-        # we dont use and_then logic here as it is hard because of the order of the arguments
-        if res.is_err():
-            return res
-        return super().update(credentials=credentials, obj=res.ok())
+    ) -> Result[WorkerPool, str]:
+        # By default all worker pools have all read permission
+        add_permissions = [] if add_permissions is None else add_permissions
+        add_permissions.append(
+            ActionObjectPermission(uid=obj.id, permission=ActionPermission.ALL_READ)
+        )
+        return super().set(
+            credentials,
+            obj,
+            add_permissions=add_permissions,
+            add_storage_permission=add_storage_permission,
+            ignore_duplicates=ignore_duplicates,
+        )
+
+    def get_by_image_uid(
+        self, credentials: SyftVerifyKey, image_uid: UID
+    ) -> list[WorkerPool]:
+        qks = QueryKeys(qks=[PoolImageIDPartitionKey.with_obj(image_uid)])
+        return self.query_all(credentials=credentials, qks=qks)
```

### Comparing `syft-0.8.6b1/src/syft/service/sync/diff_state.py` & `syft-0.8.7b1/src/syft/store/document_store.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,864 +1,803 @@
-"""
-How to check differences between two objects:
-    * by default merge every attr
-    * check if there is a custom implementation of the check function
-    * check if there are exceptions we do not want to merge
-    * check if there are some restrictions on the attr set
-"""
+# future
+from __future__ import annotations
 
 # stdlib
-import html
-import textwrap
+from collections.abc import Callable
+import types
+import typing
 from typing import Any
-from typing import ClassVar
 
 # third party
-from pydantic import model_validator
-from rich import box
-from rich.console import Console
-from rich.console import Group
-from rich.markdown import Markdown
-from rich.padding import Padding
-from rich.panel import Panel
-from typing_extensions import Self
+from pydantic import BaseModel
+from pydantic import Field
+from result import Err
+from result import Ok
+from result import Result
+from typeguard import check_type
 
 # relative
-from ...types.syft_object import SYFT_OBJECT_VERSION_2
-from ...types.syft_object import SyftObject
-from ...types.syncable_object import SyncableSyftObject
-from ...types.uid import LineageID
-from ...types.uid import UID
-from ...util import options
-from ...util.colors import SURFACE
-from ...util.fonts import ITABLES_CSS
-from ...util.fonts import fonts_css
-from ..action.action_object import ActionObject
-from ..action.action_permissions import ActionObjectPermission
-from ..action.action_permissions import StoragePermission
-from ..code.user_code import UserCode
-from ..code.user_code import UserCodeStatusCollection
-from ..job.job_stash import Job
-from ..log.log import SyftLog
-from ..output.output_service import ExecutionOutput
-from ..request.request import Request
-from ..response import SyftError
-from .sync_state import SyncState
-
-sketchy_tab = "‎ " * 4
-
-
-class AttrDiff(SyftObject):
-    # version
-    __canonical_name__ = "AttrDiff"
-    __version__ = SYFT_OBJECT_VERSION_2
-    attr_name: str
-    low_attr: Any = None
-    high_attr: Any = None
-
-    def _repr_html_(self) -> str:
-        return f"""{self.attr_name}:
-    Low Side value: {self.low_attr}
-    High Side value: {self.high_attr}
+from ..node.credentials import SyftSigningKey
+from ..node.credentials import SyftVerifyKey
+from ..serde.serializable import serializable
+from ..service.action.action_permissions import ActionObjectPermission
+from ..service.action.action_permissions import StoragePermission
+from ..service.context import AuthedServiceContext
+from ..service.response import SyftSuccess
+from ..types.base import SyftBaseModel
+from ..types.syft_object import SYFT_OBJECT_VERSION_2
+from ..types.syft_object import SyftBaseObject
+from ..types.syft_object import SyftObject
+from ..types.uid import UID
+from ..util.telemetry import instrument
+from .locks import LockingConfig
+from .locks import NoLockingConfig
+from .locks import SyftLock
+
+
+@serializable()
+class BasePartitionSettings(SyftBaseModel):
+    """Basic Partition Settings
+
+    Parameters:
+        name: str
+            Identifier to be used as prefix by stores and for partitioning
     """
 
-    def __repr_side__(self, side: str) -> str:
-        if side == "low":
-            return recursive_attr_repr(self.low_attr)
-        else:
-            return recursive_attr_repr(self.high_attr)
+    name: str
 
-    def _coll_repr_(self) -> dict[str, Any]:
-        return {
-            "attr name": self.attr_name,
-            "low attr": html.escape(f"{self.low_attr}"),
-            "high attr": html.escape(str(self.high_attr)),
-        }
 
+def first_or_none(result: Any) -> Ok:
+    if hasattr(result, "__len__") and len(result) > 0:
+        return Ok(result[0])
+    return Ok(None)
 
-class ListDiff(AttrDiff):
-    # version
-    __canonical_name__ = "ListDiff"
-    __version__ = SYFT_OBJECT_VERSION_2
-    diff_ids: list[int] = []
-    new_low_ids: list[int] = []
-    new_high_ids: list[int] = []
 
-    @property
-    def is_empty(self) -> bool:
-        return (
-            len(self.diff_ids) == 0
-            and len(self.new_low_ids) == 0
-            and len(self.new_high_ids) == 0
-        )
+def is_generic_alias(t: type) -> bool:
+    return isinstance(t, types.GenericAlias | typing._GenericAlias)
 
-    @classmethod
-    def from_lists(cls, attr_name: str, low_list: list, high_list: list) -> "ListDiff":
-        diff_ids = []
-        new_low_ids = []
-        new_high_ids = []
-        if len(low_list) != len(high_list):
-            if len(low_list) > len(high_list):
-                common_length = len(high_list)
-                new_low_ids = list(range(common_length, len(low_list)))
-            else:
-                common_length = len(low_list)
-                new_high_ids = list(range(common_length, len(high_list)))
-        else:
-            common_length = len(low_list)
 
-        for i in range(common_length):
-            # if hasattr(low_list[i], 'syft_eq'):
-            #     if not low_list[i].syft_eq(high_list[i]):
-            #         diff_ids.append(i)
-            if low_list[i] != high_list[i]:
-                diff_ids.append(i)
-
-        change_diff = ListDiff(
-            attr_name=attr_name,
-            low_attr=low_list,
-            high_attr=high_list,
-            diff_ids=diff_ids,
-            new_low_ids=new_low_ids,
-            new_high_ids=new_high_ids,
-        )
-        return change_diff
-
-
-def recursive_attr_repr(value_attr: list | dict | bytes, num_tabs: int = 0) -> str:
-    new_num_tabs = num_tabs + 1
-
-    if isinstance(value_attr, list):
-        list_repr = "[\n"
-        for elem in value_attr:
-            list_repr += recursive_attr_repr(elem, num_tabs=num_tabs + 1) + "\n"
-        list_repr += "]"
-        return list_repr
-
-    elif isinstance(value_attr, dict):
-        dict_repr = "{\n"
-        for key, elem in value_attr.items():
-            dict_repr += f"{sketchy_tab * new_num_tabs}{key}: {str(elem)}\n"
-        dict_repr += "}"
-        return dict_repr
-
-    elif isinstance(value_attr, bytes):
-        value_attr = repr(value_attr)  # type: ignore
-        if len(value_attr) > 50:
-            value_attr = value_attr[:50] + "..."  # type: ignore
-    return f"{sketchy_tab*num_tabs}{str(value_attr)}"
-
-
-class ObjectDiff(SyftObject):  # StateTuple (compare 2 objects)
-    # version
-    __canonical_name__ = "ObjectDiff"
-    __version__ = SYFT_OBJECT_VERSION_2
-    low_obj: SyncableSyftObject | None = None
-    high_obj: SyncableSyftObject | None = None
-    low_node_uid: UID
-    high_node_uid: UID
-    low_permissions: list[str] = []
-    high_permissions: list[str] = []
-    low_storage_permissions: set[UID] = set()
-    high_storage_permissions: set[UID] = set()
-
-    obj_type: type
-    diff_list: list[AttrDiff] = []
-
-    __repr_attrs__ = [
-        "low_state",
-        "high_state",
-    ]
-
-    def is_mock(self, side: str) -> bool:
-        # An object is a mock object if it exists on both sides,
-        # and has no storage permissions on `side`
-        # NOTE both sides must have the objects, else it is a new object.
-        # New+mock objects do not appear naturally, but if they do we
-        # want them to show up.
-        if side == "low":
-            obj = self.low_obj
-            other_obj = self.high_obj
-            permissions = self.low_storage_permissions
-            node_uid = self.low_node_uid
-        elif side == "high":
-            obj = self.high_obj
-            other_obj = self.low_obj
-            permissions = self.high_storage_permissions
-            node_uid = self.high_node_uid
-        else:
-            raise ValueError("Invalid side")
+class StoreClientConfig(BaseModel):
+    """Base Client specific configuration"""
 
-        if obj is None or other_obj is None:
-            return False
+    pass
 
-        return node_uid not in permissions
 
-    @classmethod
-    def from_objects(
-        cls,
-        low_obj: SyncableSyftObject | None,
-        high_obj: SyncableSyftObject | None,
-        low_permissions: set[str],
-        high_permissions: set[str],
-        low_storage_permissions: set[UID],
-        high_storage_permissions: set[UID],
-        low_node_uid: UID,
-        high_node_uid: UID,
-    ) -> "ObjectDiff":
-        if low_obj is None and high_obj is None:
-            raise ValueError("Both low and high objects are None")
-        obj_type = type(low_obj if low_obj is not None else high_obj)
-
-        res = cls(
-            low_obj=low_obj,
-            high_obj=high_obj,
-            obj_type=obj_type,
-            low_node_uid=low_node_uid,
-            high_node_uid=high_node_uid,
-            low_permissions=low_permissions,
-            high_permissions=high_permissions,
-            low_storage_permissions=low_storage_permissions,
-            high_storage_permissions=high_storage_permissions,
-        )
-
-        if (
-            low_obj is None
-            or high_obj is None
-            or res.is_mock("low")
-            or res.is_mock("high")
-        ):
-            diff_list = []
-        else:
-            diff_list = low_obj.syft_get_diffs(high_obj)
+@serializable()
+class PartitionKey(BaseModel):
+    key: str
+    type_: type | object
 
-        res.diff_list = diff_list
-        return res
+    def __eq__(self, other: Any) -> bool:
+        return (
+            type(other) == type(self)
+            and self.key == other.key
+            and self.type_ == other.type_
+        )
 
-    def __hash__(self) -> int:
-        return hash(self.id) + hash(self.low_obj) + hash(self.high_obj)
+    def with_obj(self, obj: Any) -> QueryKey:
+        return QueryKey.from_obj(partition_key=self, obj=obj)
 
-    @property
-    def status(self) -> str:
-        if self.low_obj is None or self.high_obj is None:
-            return "NEW"
-        if len(self.diff_list) == 0:
-            return "SAME"
-        return "DIFF"
+    def extract_list(self, obj: Any) -> list:
+        # not a list and matches the internal list type of the _GenericAlias
+        if not isinstance(obj, list):
+            if not isinstance(obj, typing.get_args(self.type_)):
+                obj = getattr(obj, self.key)
+                if isinstance(obj, types.FunctionType | types.MethodType):
+                    obj = obj()
 
-    @property
-    def object_id(self) -> UID:
-        uid: UID | LineageID = (
-            self.low_obj.id if self.low_obj is not None else self.high_obj.id  # type: ignore
-        )
-        if isinstance(uid, LineageID):
-            return uid.id
-        return uid
+            if not isinstance(obj, list) and isinstance(
+                obj, typing.get_args(self.type_)
+            ):
+                # still not a list but the right type
+                obj = [obj]
 
-    @property
-    def non_empty_object(self) -> SyftObject | None:
-        return self.low_obj or self.high_obj
+        # is a list type so lets compare directly
+        check_type(obj, self.type_)
+        return obj
 
     @property
-    def object_type(self) -> str:
-        return self.obj_type.__name__
+    def type_list(self) -> bool:
+        return is_generic_alias(self.type_) and self.type_.__origin__ == list
 
-    @property
-    def high_state(self) -> str:
-        return self.state_str("high")
 
-    @property
-    def low_state(self) -> str:
-        return self.state_str("low")
+@serializable()
+class PartitionKeys(BaseModel):
+    pks: PartitionKey | tuple[PartitionKey, ...] | list[PartitionKey]
 
     @property
-    def object_uid(self) -> UID:
-        return self.low_obj.id if self.low_obj is not None else self.high_obj.id  # type: ignore
+    def all(self) -> tuple[PartitionKey, ...] | list[PartitionKey]:
+        # make sure we always return a list even if there's a single value
+        return self.pks if isinstance(self.pks, tuple | list) else [self.pks]
 
-    def diff_attributes_str(self, side: str) -> str:
-        obj = self.low_obj if side == "low" else self.high_obj
+    def with_obj(self, obj: Any) -> QueryKeys:
+        return QueryKeys.from_obj(partition_keys=self, obj=obj)
 
-        if obj is None:
-            return ""
+    def with_tuple(self, *args: Any) -> QueryKeys:
+        return QueryKeys.from_tuple(partition_keys=self, args=args)
 
-        repr_attrs = getattr(obj, "__repr_attrs__", [])
-        if self.status == "SAME":
-            repr_attrs = repr_attrs[:3]
+    def add(self, pk: PartitionKey) -> PartitionKeys:
+        return PartitionKeys(pks=list(self.all) + [pk])
 
-        if self.status in {"SAME", "NEW"}:
-            attrs_str = ""
-            for attr in repr_attrs:
-                value = getattr(obj, attr)
-                attrs_str += f"{attr}: {recursive_attr_repr(value)}\n"
-            return attrs_str
+    @staticmethod
+    def from_dict(cks_dict: dict[str, type]) -> PartitionKeys:
+        pks = []
+        for k, t in cks_dict.items():
+            pks.append(PartitionKey(key=k, type_=t))
+        return PartitionKeys(pks=pks)
 
-        elif self.status == "DIFF":
-            attrs_str = ""
-            for diff in self.diff_list:
-                attrs_str += f"{diff.attr_name}: {diff.__repr_side__(side)}\n"
-            return attrs_str
-        else:
-            raise ValueError("")
 
-    def diff_side_str(self, side: str) -> str:
-        obj = self.low_obj if side == "low" else self.high_obj
-        if obj is None:
-            return ""
-        res = f"{self.obj_type.__name__.upper()} #{obj.id}:\n"
-        res += self.diff_attributes_str(side)
-        return res
-
-    def state_str(self, side: str) -> str:
-        other_obj: SyftObject | None = None
-        if side == "high":
-            obj = self.high_obj
-            other_obj = self.low_obj
-        else:
-            obj = self.low_obj
-            other_obj = self.high_obj
+@serializable()
+class QueryKey(PartitionKey):
+    value: Any = None
 
-        if obj is None:
-            return "-"
-        if self.status == "SAME":
-            return f"SAME\n{self.obj_type.__name__}"
-
-        if isinstance(obj, ActionObject):
-            return obj.__repr__()
-
-        if other_obj is None:  # type: ignore[unreachable]
-            attrs_str = ""
-            attrs = getattr(obj, "__repr_attrs__", [])
-            for attr in attrs:
-                value = getattr(obj, attr)
-                attrs_str += f"{sketchy_tab}{attr} = {recursive_attr_repr(value)}\n"
-            attrs_str = attrs_str[:-1]
-            return f"NEW\n\nclass {self.object_type}:\n{attrs_str}"
-
-        attr_text = f"DIFF\nclass {self.object_type}:\n"
-        for diff in self.diff_list:
-            # TODO
-            attr_text += (
-                f"{sketchy_tab}{diff.attr_name}={diff.__repr_side__(side)}," + "\n"
-            )
-        if len(self.diff_list) > 0:
-            attr_text = attr_text[:-2]
+    def __eq__(self, other: Any) -> bool:
+        return (
+            type(other) == type(self)
+            and self.key == other.key
+            and self.type_ == other.type_
+            and self.value == other.value
+        )
+
+    @property
+    def partition_key(self) -> PartitionKey:
+        return PartitionKey(key=self.key, type_=self.type_)
 
-        return attr_text
+    @staticmethod
+    def from_obj(partition_key: PartitionKey, obj: Any) -> QueryKey:
+        pk_key = partition_key.key
+        pk_type = partition_key.type_
 
-    def get_obj(self) -> SyftObject | None:
-        if self.status == "NEW":
-            return self.low_obj if self.low_obj is not None else self.high_obj
+        # 🟡 TODO: support more advanced types than List[type]
+        if partition_key.type_list:
+            pk_value = partition_key.extract_list(obj)
         else:
-            raise ValueError("ERROR")
-
-    def _coll_repr_(self) -> dict[str, Any]:
-        low_state = f"{self.status}\n{self.diff_side_str('low')}"
-        high_state = f"{self.status}\n{self.diff_side_str('high')}"
-        return {
-            "low_state": html.escape(low_state),
-            "high_state": html.escape(high_state),
-        }
-
-    def _repr_html_(self) -> str:
-        if self.low_obj is None and self.high_obj is None:
-            return SyftError(message="Something broke")
-
-        base_str = f"""
-        <style>
-        {fonts_css}
-        .syft-dataset {{color: {SURFACE[options.color_theme]};}}
-        .syft-dataset h3,
-        .syft-dataset p
-            {{font-family: 'Open Sans';}}
-            {ITABLES_CSS}
-        </style>
-        <div class='syft-diff'>
-        """
-
-        obj_repr: str
-        attr_text: str
-        if self.low_obj is None:
-            if hasattr(self.high_obj, "_repr_html_"):
-                obj_repr = self.high_obj._repr_html_()  # type: ignore
-            elif hasattr(self.high_obj, "_inner_repr"):
-                obj_repr = self.high_obj._inner_repr()  # type: ignore
+            if isinstance(obj, pk_type):
+                pk_value = obj
             else:
-                obj_repr = self.__repr__()
-            attr_text = (
-                f"""
-    <h3>{self.object_type} ObjectDiff (New {self.object_type}  on the High Side):</h3>
-    """
-                + obj_repr
-            )
+                pk_value = getattr(obj, pk_key)
+                # object has a method for getting these types
+                # we can't use properties because we don't seem to be able to get the
+                # return types
+                # TODO: fix the mypy issue
+                if isinstance(pk_value, types.FunctionType | types.MethodType):  # type: ignore[unreachable]
+                    pk_value = pk_value()  # type: ignore[unreachable]
+
+            if pk_value and not isinstance(pk_value, pk_type):
+                raise Exception(
+                    f"PartitionKey {pk_value} of type {type(pk_value)} must be {pk_type}."
+                )
+        return QueryKey(key=pk_key, type_=pk_type, value=pk_value)
 
-        elif self.high_obj is None:
-            if hasattr(self.low_obj, "_repr_html_"):
-                obj_repr = self.low_obj._repr_html_()  # type: ignore
-            elif hasattr(self.low_obj, "_inner_repr"):
-                obj_repr = self.low_obj._inner_repr()  # type: ignore
-            else:
-                obj_repr = self.__repr__()
-            attr_text = (
-                f"""
-    <h3>{self.object_type} ObjectDiff (New {self.object_type}  on the High Side):</h3>
-    """
-                + obj_repr
-            )
+    @property
+    def as_dict(self) -> dict[str, Any]:
+        return {self.key: self.value}
 
-        elif self.status == "SAME":
-            obj_repr = "No changes between low side and high side"
-        else:
-            obj_repr = ""
-            for diff in self.diff_list:
-                obj_repr += diff.__repr__() + "<br>"
-
-            obj_repr = obj_repr.replace("\n", "<br>")
-            # print("New lines", res)
-
-        attr_text = f"<h3>{self.object_type} ObjectDiff:</h3>\n{obj_repr}"
-        return base_str + attr_text
-
-
-def _wrap_text(text: str, width: int, indent: int = 4) -> str:
-    """Wrap text, preserving existing line breaks"""
-    return "\n".join(
-        [
-            "\n".join(
-                textwrap.wrap(
-                    line,
-                    width,
-                    break_long_words=False,
-                    replace_whitespace=False,
-                    subsequent_indent=" " * indent,
+    @property
+    def as_dict_mongo(self) -> dict[str, Any]:
+        key = self.key
+        if key == "id":
+            key = "_id"
+        if self.type_list:
+            # We want to search inside the list of values
+            return {key: {"$in": self.value}}
+        return {key: self.value}
+
+
+@serializable()
+class PartitionKeysWithUID(PartitionKeys):
+    uid_pk: PartitionKey
+
+    @property
+    def all(self) -> tuple[PartitionKey, ...] | list[PartitionKey]:
+        all_keys = list(self.pks) if isinstance(self.pks, tuple | list) else [self.pks]
+        if self.uid_pk not in all_keys:
+            all_keys.insert(0, self.uid_pk)
+        return all_keys
+
+
+@serializable()
+class QueryKeys(SyftBaseModel):
+    qks: QueryKey | tuple[QueryKey, ...] | list[QueryKey]
+
+    @property
+    def all(self) -> tuple[QueryKey, ...] | list[QueryKey]:
+        # make sure we always return a list even if there's a single value
+        return self.qks if isinstance(self.qks, tuple | list) else [self.qks]
+
+    @staticmethod
+    def from_obj(partition_keys: PartitionKeys, obj: SyftObject) -> QueryKeys:
+        qks = []
+        for partition_key in partition_keys.all:
+            pk_key = partition_key.key
+            pk_type = partition_key.type_
+            pk_value = getattr(obj, pk_key)
+            # object has a method for getting these types
+            # we can't use properties because we don't seem to be able to get the
+            # return types
+            if isinstance(pk_value, types.FunctionType | types.MethodType):
+                pk_value = pk_value()
+            if partition_key.type_list:
+                pk_value = partition_key.extract_list(obj)
+            else:
+                if pk_value and not isinstance(pk_value, pk_type):
+                    raise Exception(
+                        f"PartitionKey {pk_value} of type {type(pk_value)} must be {pk_type}."
+                    )
+            qk = QueryKey(key=pk_key, type_=pk_type, value=pk_value)
+            qks.append(qk)
+        return QueryKeys(qks=qks)
+
+    @staticmethod
+    def from_tuple(partition_keys: PartitionKeys, args: tuple) -> QueryKeys:
+        qks = []
+        for partition_key, pk_value in zip(partition_keys.all, args):
+            pk_key = partition_key.key
+            pk_type = partition_key.type_
+            if not isinstance(pk_value, pk_type):
+                raise Exception(
+                    f"PartitionKey {pk_value} of type {type(pk_value)} must be {pk_type}."
                 )
-            )
-            for line in text.splitlines()
-            if line.strip() != ""
-        ]
-    )
+            qk = QueryKey(key=pk_key, type_=pk_type, value=pk_value)
+            qks.append(qk)
+        return QueryKeys(qks=qks)
+
+    @staticmethod
+    def from_dict(qks_dict: dict[str, Any]) -> QueryKeys:
+        qks = []
+        for k, v in qks_dict.items():
+            qks.append(QueryKey(key=k, type_=type(v), value=v))
+        return QueryKeys(qks=qks)
+
+    @property
+    def as_dict(self) -> dict:
+        qk_dict = {}
+        for qk in self.all:
+            qk_key = qk.key
+            qk_value = qk.value
+            qk_dict[qk_key] = qk_value
+        return qk_dict
+
+    @property
+    def as_dict_mongo(self) -> dict:
+        qk_dict = {}
+        for qk in self.all:
+            qk_key = qk.key
+            qk_value = qk.value
+            if qk_key == "id":
+                qk_key = "_id"
+            if qk.type_list:
+                # We want to search inside the list of values
+                qk_dict[qk_key] = {"$in": qk_value}
+            else:
+                qk_dict[qk_key] = qk_value
+        return qk_dict
 
 
-class ObjectDiffBatch(SyftObject):
-    __canonical_name__ = "DiffHierarchy"
-    __version__ = SYFT_OBJECT_VERSION_2
-    LINE_LENGTH: ClassVar[int] = 100
-    INDENT: ClassVar[int] = 4
-    ORDER: ClassVar[dict] = {"low": 0, "high": 1}
-
-    # Diffs are ordered in depth-first order,
-    # the first diff is the root of the hierarchy
-    diffs: list[ObjectDiff]
-    hierarchy_levels: list[int]
-    dependencies: dict[UID, list[UID]] = {}
-    dependents: dict[UID, list[UID]] = {}
-
-    @property
-    def visual_hierarchy(self) -> tuple[type, dict]:
-        # Returns
-        root_obj: Request | UserCodeStatusCollection | ExecutionOutput | Any = (
-            self.root.low_obj if self.root.low_obj is not None else self.root.high_obj
-        )
-        if isinstance(root_obj, Request):
-            return Request, {
-                Request: [UserCode],
-                UserCode: [UserCode],
-            }
-        if isinstance(root_obj, UserCodeStatusCollection):
-            return UserCode, {
-                UserCode: [UserCodeStatusCollection],
-            }
-        if isinstance(root_obj, ExecutionOutput):
-            return UserCode, {
-                UserCode: [Job],
-                Job: [ExecutionOutput, SyftLog, Job],
-                ExecutionOutput: [ActionObject],
-            }
-        raise ValueError(f"Unknown root type: {self.root.obj_type}")
-
-    @model_validator(mode="after")
-    def make_dependents(self) -> Self:
-        dependents: dict = {}
-        for parent, children in self.dependencies.items():
-            for child in children:
-                dependents[child] = dependents.get(child, []) + [parent]
-        self.dependents = dependents
-        return self
+UIDPartitionKey = PartitionKey(key="id", type_=UID)
 
-    @property
-    def root(self) -> ObjectDiff:
-        return self.diffs[0]
 
-    def __len__(self) -> int:
-        return len(self.diffs)
+@serializable()
+class PartitionSettings(BasePartitionSettings):
+    object_type: type
+    store_key: PartitionKey = UIDPartitionKey
 
-    def __repr__(self) -> str:
-        return f"""{self.hierarchy_str('low')}
+    @property
+    def unique_keys(self) -> PartitionKeys:
+        unique_keys = PartitionKeys.from_dict(self.object_type._syft_unique_keys_dict())
+        return unique_keys.add(self.store_key)
 
-{self.hierarchy_str('high')}
-"""
+    @property
+    def searchable_keys(self) -> PartitionKeys:
+        return PartitionKeys.from_dict(self.object_type._syft_searchable_keys_dict())
 
-    def _repr_markdown_(self, wrap_as_python: bool = True, indent: int = 0) -> str:
-        return ""  # Turns off the _repr_markdown_ of SyftObject
-
-    def _get_visual_hierarchy(self, node: ObjectDiff) -> dict[ObjectDiff, dict]:
-        _, child_types_map = self.visual_hierarchy
-        child_types = child_types_map.get(node.obj_type, [])
-        dep_ids = self.dependencies.get(node.object_id, []) + self.dependents.get(
-            node.object_id, []
-        )
-
-        result = {}
-        for child_type in child_types:
-            children = [
-                n
-                for n in self.diffs
-                if n.object_id in dep_ids
-                and isinstance(n.low_obj or n.high_obj, child_type)
-            ]
-            for child in children:
-                result[child] = self._get_visual_hierarchy(child)
 
-        return result
+@instrument
+@serializable(attrs=["settings", "store_config", "unique_cks", "searchable_cks"])
+class StorePartition:
+    """Base StorePartition
 
-    def get_visual_hierarchy(self) -> "ObjectDiffBatch":
-        visual_root_type = self.visual_hierarchy[0]
-        # First diff with a visual root type is the visual root
-        # because diffs are in depth-first order
-        visual_root = [
-            diff
-            for diff in self.diffs
-            if isinstance(diff.low_obj or diff.high_obj, visual_root_type)
-        ][0]
-        return {visual_root: self._get_visual_hierarchy(visual_root)}  # type: ignore
-
-    def _get_obj_str(self, diff_obj: ObjectDiff, level: int, side: str) -> str:
-        obj = diff_obj.low_obj if side == "low" else diff_obj.high_obj
-        if obj is None:
-            return ""
-        indent = " " * level * self.INDENT
-        obj_str = diff_obj.diff_side_str(side)
-        obj_str = _wrap_text(obj_str, width=self.LINE_LENGTH - len(indent))
-
-        line_prefix = indent + f"―――― {diff_obj.status} "
-        line = "―" * (self.LINE_LENGTH - len(line_prefix))
-        return f"""{line_prefix}{line}
-
-{textwrap.indent(obj_str, indent)}
-
-"""
-
-    def hierarchy_str(self, side: str) -> str:
-        def _hierarchy_str_recursive(tree: dict, level: int) -> str:
-            result = ""
-            for node, children in tree.items():
-                result += self._get_obj_str(node, level, side)
-                result += _hierarchy_str_recursive(children, level + 1)
-            return result
-
-        visual_hierarchy = self.get_visual_hierarchy()
-        res = _hierarchy_str_recursive(visual_hierarchy, 0)
-        if res == "":
-            res = f"No {side} side changes."
-        return f"""{side.upper()} SIDE STATE:
+    Parameters:
+        settings: PartitionSettings
+            PySyft specific settings
+        store_config: StoreConfig
+            Backend specific configuration
+    """
 
-{res}"""
+    def __init__(
+        self,
+        node_uid: UID,
+        root_verify_key: SyftVerifyKey | None,
+        settings: PartitionSettings,
+        store_config: StoreConfig,
+    ) -> None:
+        if root_verify_key is None:
+            root_verify_key = SyftSigningKey.generate().verify_key
+        self.node_uid = node_uid
+        self.root_verify_key = root_verify_key
+        self.settings = settings
+        self.store_config = store_config
+        self.init_store()
+
+        store_config.locking_config.lock_name = f"StorePartition-{settings.name}"
+        self.lock = SyftLock(store_config.locking_config)
+
+    def init_store(self) -> Result[Ok, Err]:
+        try:
+            self.unique_cks = self.settings.unique_keys.all
+            self.searchable_cks = self.settings.searchable_keys.all
+        except BaseException as e:
+            return Err(str(e))
+
+        return Ok(True)
+
+    def matches_unique_cks(self, partition_key: PartitionKey) -> bool:
+        return partition_key in self.unique_cks
+
+    def matches_searchable_cks(self, partition_key: PartitionKey) -> bool:
+        return partition_key in self.searchable_cks
+
+    def store_query_key(self, obj: Any) -> QueryKey:
+        return self.settings.store_key.with_obj(obj)
+
+    def store_query_keys(self, objs: Any) -> QueryKeys:
+        return QueryKeys(qks=[self.store_query_key(obj) for obj in objs])
+
+    # Thread-safe methods
+    def _thread_safe_cbk(self, cbk: Callable, *args: Any, **kwargs: Any) -> Any | Err:
+        locked = self.lock.acquire(blocking=True)
+        if not locked:
+            print("FAILED TO LOCK")
+            return Err(
+                f"Failed to acquire lock for the operation {self.lock.lock_name} ({self.lock._lock})"
+            )
 
+        try:
+            result = cbk(*args, **kwargs)
+        except BaseException as e:
+            result = Err(str(e))
+        self.lock.release()
 
-class NodeDiff(SyftObject):
-    __canonical_name__ = "NodeDiff"
-    __version__ = SYFT_OBJECT_VERSION_2
+        return result
 
-    low_node_uid: UID
-    high_node_uid: UID
-    obj_uid_to_diff: dict[UID, ObjectDiff] = {}
-    dependencies: dict[UID, list[UID]] = {}
-
-    @classmethod
-    def from_sync_state(
-        cls: type["NodeDiff"], low_state: SyncState, high_state: SyncState
-    ) -> "NodeDiff":
-        obj_uid_to_diff = {}
-        for obj_id in set(low_state.objects.keys()) | set(high_state.objects.keys()):
-            low_obj = low_state.objects.get(obj_id, None)
-            low_permissions = low_state.permissions.get(obj_id, set())
-            low_storage_permissions = low_state.storage_permissions.get(obj_id, set())
-            high_obj = high_state.objects.get(obj_id, None)
-            high_permissions = high_state.permissions.get(obj_id, set())
-            high_storage_permissions = high_state.storage_permissions.get(obj_id, set())
-            diff = ObjectDiff.from_objects(
-                low_obj=low_obj,
-                high_obj=high_obj,
-                low_permissions=low_permissions,
-                high_permissions=high_permissions,
-                low_storage_permissions=low_storage_permissions,
-                high_storage_permissions=high_storage_permissions,
-                low_node_uid=low_state.node_uid,
-                high_node_uid=high_state.node_uid,
-            )
-            obj_uid_to_diff[diff.object_id] = diff
+    def set(
+        self,
+        credentials: SyftVerifyKey,
+        obj: SyftObject,
+        add_permissions: list[ActionObjectPermission] | None = None,
+        add_storage_permission: bool = True,
+        ignore_duplicates: bool = False,
+    ) -> Result[SyftObject, str]:
+        return self._thread_safe_cbk(
+            self._set,
+            credentials=credentials,
+            obj=obj,
+            add_permissions=add_permissions,
+            add_storage_permission=add_storage_permission,
+            ignore_duplicates=ignore_duplicates,
+        )
+
+    def get(
+        self,
+        credentials: SyftVerifyKey,
+        uid: UID,
+    ) -> Result[SyftObject, str]:
+        return self._thread_safe_cbk(
+            self._get,
+            uid=uid,
+            credentials=credentials,
+        )
+
+    def find_index_or_search_keys(
+        self,
+        credentials: SyftVerifyKey,
+        index_qks: QueryKeys,
+        search_qks: QueryKeys,
+        order_by: PartitionKey | None = None,
+    ) -> Result[list[SyftObject], str]:
+        return self._thread_safe_cbk(
+            self._find_index_or_search_keys,
+            credentials,
+            index_qks=index_qks,
+            search_qks=search_qks,
+            order_by=order_by,
+        )
+
+    def remove_keys(
+        self,
+        unique_query_keys: QueryKeys,
+        searchable_query_keys: QueryKeys,
+    ) -> None:
+        self._thread_safe_cbk(
+            self._remove_keys,
+            unique_query_keys=unique_query_keys,
+            searchable_query_keys=searchable_query_keys,
+        )
+
+    def update(
+        self,
+        credentials: SyftVerifyKey,
+        qk: QueryKey,
+        obj: SyftObject,
+        has_permission: bool = False,
+    ) -> Result[SyftObject, str]:
+        return self._thread_safe_cbk(
+            self._update,
+            credentials=credentials,
+            qk=qk,
+            obj=obj,
+            has_permission=has_permission,
+        )
+
+    def get_all_from_store(
+        self,
+        credentials: SyftVerifyKey,
+        qks: QueryKeys,
+        order_by: PartitionKey | None = None,
+    ) -> Result[list[SyftObject], str]:
+        return self._thread_safe_cbk(
+            self._get_all_from_store, credentials, qks, order_by
+        )
+
+    def delete(
+        self, credentials: SyftVerifyKey, qk: QueryKey, has_permission: bool = False
+    ) -> Result[SyftSuccess, Err]:
+        return self._thread_safe_cbk(
+            self._delete, credentials, qk, has_permission=has_permission
+        )
+
+    def all(
+        self,
+        credentials: SyftVerifyKey,
+        order_by: PartitionKey | None = None,
+        has_permission: bool | None = False,
+    ) -> Result[list[BaseStash.object_type], str]:
+        return self._thread_safe_cbk(self._all, credentials, order_by, has_permission)
+
+    def migrate_data(
+        self,
+        to_klass: SyftObject,
+        context: AuthedServiceContext,
+        has_permission: bool | None = False,
+    ) -> Result[bool, str]:
+        return self._thread_safe_cbk(
+            self._migrate_data, to_klass, context, has_permission
+        )
+
+    # Potentially thread-unsafe methods.
+    # CAUTION:
+    #       * Don't use self.lock here.
+    #       * Do not call the public thread-safe methods here(with locking).
+    # These methods are called from the public thread-safe API, and will hang the process.
+    def _set(
+        self,
+        credentials: SyftVerifyKey,
+        obj: SyftObject,
+        add_permissions: list[ActionObjectPermission] | None = None,
+        add_storage_permission: bool = True,
+        ignore_duplicates: bool = False,
+    ) -> Result[SyftObject, str]:
+        raise NotImplementedError
+
+    def _update(
+        self,
+        credentials: SyftVerifyKey,
+        qk: QueryKey,
+        obj: SyftObject,
+        has_permission: bool = False,
+        overwrite: bool = False,
+    ) -> Result[SyftObject, str]:
+        raise NotImplementedError
+
+    def _get_all_from_store(
+        self,
+        credentials: SyftVerifyKey,
+        qks: QueryKeys,
+        order_by: PartitionKey | None = None,
+    ) -> Result[list[SyftObject], str]:
+        raise NotImplementedError
+
+    def _delete(
+        self, credentials: SyftVerifyKey, qk: QueryKey, has_permission: bool = False
+    ) -> Result[SyftSuccess, Err]:
+        raise NotImplementedError
+
+    def _all(
+        self,
+        credentials: SyftVerifyKey,
+        order_by: PartitionKey | None = None,
+        has_permission: bool | None = False,
+    ) -> Result[list[BaseStash.object_type], str]:
+        raise NotImplementedError
+
+    def add_permission(self, permission: ActionObjectPermission) -> None:
+        raise NotImplementedError
+
+    def add_permissions(self, permissions: list[ActionObjectPermission]) -> None:
+        raise NotImplementedError
+
+    def remove_permission(self, permission: ActionObjectPermission) -> None:
+        raise NotImplementedError
+
+    def has_permission(self, permission: ActionObjectPermission) -> bool:
+        raise NotImplementedError
+
+    def add_storage_permission(self, permission: StoragePermission) -> None:
+        raise NotImplementedError
+
+    def add_storage_permissions(self, permissions: list[StoragePermission]) -> None:
+        raise NotImplementedError
+
+    def remove_storage_permission(self, permission: StoragePermission) -> None:
+        raise NotImplementedError
+
+    def has_storage_permission(self, permission: StoragePermission | UID) -> bool:
+        raise NotImplementedError
+
+    def _migrate_data(
+        self,
+        to_klass: SyftObject,
+        context: AuthedServiceContext,
+        has_permission: bool,
+    ) -> Result[bool, str]:
+        raise NotImplementedError
+
+
+@instrument
+@serializable()
+class DocumentStore:
+    """Base Document Store
+
+    Parameters:
+        store_config: StoreConfig
+            Store specific configuration.
+    """
 
-        node_diff = cls(
-            low_node_uid=low_state.node_uid,
-            high_node_uid=high_state.node_uid,
-            obj_uid_to_diff=obj_uid_to_diff,
-        )
-
-        node_diff._init_dependencies(low_state, high_state)
-        return node_diff
-
-    def _init_dependencies(self, low_state: SyncState, high_state: SyncState) -> None:
-        all_parents = set(low_state.dependencies.keys()) | set(
-            high_state.dependencies.keys()
-        )
-        for parent in all_parents:
-            low_deps = low_state.dependencies.get(parent, [])
-            high_deps = high_state.dependencies.get(parent, [])
-            self.dependencies[parent] = list(set(low_deps) | set(high_deps))
-
-    @property
-    def diffs(self) -> list[ObjectDiff]:
-        diffs_depthfirst = [
-            diff for hierarchy in self.hierarchies for diff in hierarchy.diffs
-        ]
-        # deduplicate
-        diffs = []
-        ids = set()
-        for diff in diffs_depthfirst:
-            if diff.object_id not in ids:
-                diffs.append(diff)
-                ids.add(diff.object_id)
-        return diffs
-
-    def _repr_html_(self) -> Any:
-        return self.diffs._repr_html_()
-
-    def _sort_hierarchies(
-        self, hierarchies: list[ObjectDiffBatch]
-    ) -> list[ObjectDiffBatch]:
-        without_usercode = []
-        grouped_by_usercode: dict[UID, list[ObjectDiffBatch]] = {}
-        for hierarchy in hierarchies:
-            has_usercode = False
-            for diff in hierarchy.diffs:
-                obj = diff.low_obj if diff.low_obj is not None else diff.high_obj
-                if isinstance(obj, UserCode):
-                    usercode_id = obj.id
-                    if usercode_id not in grouped_by_usercode:
-                        grouped_by_usercode[usercode_id] = []
-                    grouped_by_usercode[usercode_id].append(hierarchy)
-                    has_usercode = True
-                    break
-            if not has_usercode:
-                without_usercode.append(hierarchy)
-
-        # Order of hierarchies, by root object type
-        hierarchy_order = [UserCodeStatusCollection, Request, ExecutionOutput]
-        # Sort group by hierarchy_order, then by root object id
-        for hierarchy_group in grouped_by_usercode.values():
-            hierarchy_group.sort(
-                key=lambda x: (
-                    hierarchy_order.index(x.root.obj_type),
-                    x.root.object_id,
-                )
-            )
+    partitions: dict[str, StorePartition]
+    partition_type: type[StorePartition]
 
-        # sorted = sorted groups + without_usercode
-        sorted_hierarchies = []
-        for grp in grouped_by_usercode.values():
-            sorted_hierarchies.extend(grp)
-        sorted_hierarchies.extend(without_usercode)
-        return sorted_hierarchies
-
-    @property
-    def hierarchies(self) -> list[ObjectDiffBatch]:
-        # Returns a list of hierarchies, where each hierarchy is a list of tuples (ObjectDiff, level),
-        # in depth-first order.
-
-        # Each hierarchy only contains one root, at the first position
-        # Example: [(Diff1, 0), (Diff2, 1), (Diff3, 2), (Diff4, 1)]
-        # Diff1
-        # -- Diff2
-        # ---- Diff3
-        # -- Diff4
-
-        def _build_hierarchy_helper(
-            uid: UID, level: int = 0, visited: set | None = None
-        ) -> list:
-            visited = visited if visited is not None else set()
-
-            if uid in visited:
-                return []
-
-            result = [(uid, level)]
-            visited.add(uid)
-            if uid in self.dependencies:
-                deps = self.dependencies[uid]
-                for dep_uid in self.dependencies[uid]:
-                    if dep_uid not in visited:
-                        # NOTE we pass visited + deps to recursive calls, to have
-                        # all objects at the highest level in the hierarchy
-                        # Example:
-                        # ExecutionOutput
-                        # -- Job
-                        # ---- Result
-                        # -- Result
-                        # We want to omit Job.Result, because it's already in ExecutionOutput.Result
-                        result.extend(
-                            _build_hierarchy_helper(
-                                uid=dep_uid,
-                                level=level + 1,
-                                visited=visited | set(deps) - {dep_uid},
-                            )
-                        )
-            return result
-
-        hierarchies = []
-        all_ids = set(self.obj_uid_to_diff.keys())
-        child_ids = {child for deps in self.dependencies.values() for child in deps}
-        # Root ids are object ids with no parents
-        root_ids = list(all_ids - child_ids)
-
-        for root_uid in root_ids:
-            uid_hierarchy = _build_hierarchy_helper(root_uid)
-            diffs = [self.obj_uid_to_diff[uid] for uid, _ in uid_hierarchy]
-            levels = [level for _, level in uid_hierarchy]
-
-            batch_uids = {uid for uid, _ in uid_hierarchy}
-            dependencies = {
-                uid: [d for d in self.dependencies.get(uid, []) if d in batch_uids]
-                for uid in batch_uids
-            }
-
-            batch = ObjectDiffBatch(
-                diffs=diffs,
-                hierarchy_levels=levels,
-                dependencies=dependencies,
+    def __init__(
+        self,
+        node_uid: UID,
+        root_verify_key: SyftVerifyKey | None,
+        store_config: StoreConfig,
+    ) -> None:
+        if store_config is None:
+            raise Exception("must have store config")
+        self.partitions = {}
+        self.store_config = store_config
+        self.node_uid = node_uid
+        self.root_verify_key = root_verify_key
+
+    def partition(self, settings: PartitionSettings) -> StorePartition:
+        if settings.name not in self.partitions:
+            self.partitions[settings.name] = self.partition_type(
+                node_uid=self.node_uid,
+                root_verify_key=self.root_verify_key,
+                settings=settings,
+                store_config=self.store_config,
             )
-            hierarchies.append(batch)
+        return self.partitions[settings.name]
 
-        hierarchies_sorted = self._sort_hierarchies(hierarchies)
-        return hierarchies_sorted
 
-    def objs_to_sync(self) -> list[SyftObject]:
-        objs: list[SyftObject] = []
-        for diff in self.diffs:
-            if diff.status == "NEW":
-                objs.append(diff.get_obj())
-        return objs
+@instrument
+class BaseStash:
+    object_type: type[SyftObject]
+    settings: PartitionSettings
+    partition: StorePartition
 
+    def __init__(self, store: DocumentStore) -> None:
+        self.store = store
+        self.partition = store.partition(type(self).settings)
 
-class SyncDecision(SyftObject):
-    __canonical_name__ = "SyncDecision"
-    __version__ = SYFT_OBJECT_VERSION_2
+    def check_type(self, obj: Any, type_: type) -> Result[Any, str]:
+        return (
+            Ok(obj)
+            if isinstance(obj, type_)
+            else Err(f"{type(obj)} does not match required type: {type_}")
+        )
 
-    diff: ObjectDiff
-    decision: str | None
-    new_permissions_lowside: list[ActionObjectPermission]
-    new_storage_permissions_lowside: list[StoragePermission]
-    new_storage_permissions_highside: list[StoragePermission]
-    mockify: bool
+    def get_all(
+        self,
+        credentials: SyftVerifyKey,
+        order_by: PartitionKey | None = None,
+        has_permission: bool = False,
+    ) -> Result[list[BaseStash.object_type], str]:
+        return self.partition.all(credentials, order_by, has_permission)
 
+    def add_permissions(self, permissions: list[ActionObjectPermission]) -> None:
+        self.partition.add_permissions(permissions)
 
-class ResolvedSyncState(SyftObject):
-    __canonical_name__ = "SyncUpdate"
-    __version__ = SYFT_OBJECT_VERSION_2
+    def add_permission(self, permission: ActionObjectPermission) -> None:
+        self.partition.add_permission(permission)
 
-    node_uid: UID
-    create_objs: list[SyncableSyftObject] = []
-    update_objs: list[SyncableSyftObject] = []
-    delete_objs: list[SyftObject] = []
-    new_permissions: list[ActionObjectPermission] = []
-    new_storage_permissions: list[StoragePermission] = []
-    alias: str
-
-    def add_sync_decision(self, sync_decision: SyncDecision) -> None:
-        diff = sync_decision.diff
-
-        if diff.status == "SAME":
-            return
-
-        my_obj = diff.low_obj if self.alias == "low" else diff.high_obj
-        other_obj = diff.low_obj if self.alias == "high" else diff.high_obj
-
-        if other_obj is not None and sync_decision.mockify:
-            other_obj = other_obj.create_shareable_sync_copy(mock=True)
-
-        if sync_decision.decision != self.alias:  # chose for the other
-            if diff.status == "DIFF":
-                # keep IDs comparison here, otherwise it will break with actionobjects
-                if other_obj.id not in [x.id for x in self.update_objs]:  # type: ignore
-                    self.update_objs.append(other_obj)
-
-            elif diff.status == "NEW":
-                if my_obj is None:
-                    # keep IDs comparison here, otherwise it will break with actionobjects
-                    if other_obj.id not in [x.id for x in self.create_objs]:  # type: ignore
-                        self.create_objs.append(other_obj)
-
-                elif other_obj is None:
-                    # keep IDs comparison here, otherwise it will break with actionobjects
-                    if my_obj.id not in [x.id for x in self.delete_objs]:
-                        self.delete_objs.append(my_obj)
-
-        if self.alias == "low":
-            self.new_permissions.extend(sync_decision.new_permissions_lowside)
-            self.new_storage_permissions.extend(
-                sync_decision.new_storage_permissions_lowside
-            )
-        elif self.alias == "high":
-            self.new_storage_permissions.extend(
-                sync_decision.new_storage_permissions_highside
-            )
-        else:
-            raise ValueError("Invalid alias")
+    def remove_permission(self, permission: ActionObjectPermission) -> None:
+        self.partition.remove_permission(permission)
 
-    def __repr__(self) -> str:
-        return (
-            f"ResolvedSyncState(\n"
-            f"  create_objs={self.create_objs},\n"
-            f"  update_objs={self.update_objs},\n"
-            f"  delete_objs={self.delete_objs}\n"
-            f"  new_permissions={self.new_permissions}\n"
-            f")"
-        )
+    def has_permission(self, permission: ActionObjectPermission) -> bool:
+        return self.partition.has_permission(permission=permission)
 
+    def has_storage_permission(self, permission: StoragePermission) -> bool:
+        return self.partition.has_storage_permission(permission=permission)
 
-def display_diff_object(obj_state: str | None) -> Panel:
-    if obj_state is None:
-        return Panel(Markdown("None"), box=box.ROUNDED, expand=False)
-    return Panel(
-        Markdown(f"```python\n{obj_state}\n```", code_theme="default"),
-        box=box.ROUNDED,
-        expand=False,
-    )
+    def __len__(self) -> int:
+        return len(self.partition)
 
+    def set(
+        self,
+        credentials: SyftVerifyKey,
+        obj: BaseStash.object_type,
+        add_permissions: list[ActionObjectPermission] | None = None,
+        add_storage_permission: bool = True,
+        ignore_duplicates: bool = False,
+    ) -> Result[BaseStash.object_type, str]:
+        return self.partition.set(
+            credentials=credentials,
+            obj=obj,
+            ignore_duplicates=ignore_duplicates,
+            add_permissions=add_permissions,
+            add_storage_permission=add_storage_permission,
+        )
+
+    def query_all(
+        self,
+        credentials: SyftVerifyKey,
+        qks: QueryKey | QueryKeys,
+        order_by: PartitionKey | None = None,
+    ) -> Result[list[BaseStash.object_type], str]:
+        if isinstance(qks, QueryKey):
+            qks = QueryKeys(qks=qks)
+
+        unique_keys = []
+        searchable_keys = []
+
+        for qk in qks.all:
+            pk = qk.partition_key
+            if self.partition.matches_unique_cks(pk):
+                unique_keys.append(qk)
+            elif self.partition.matches_searchable_cks(pk):
+                searchable_keys.append(qk)
+            else:
+                return Err(
+                    f"{qk} not in {type(self.partition)} unique or searchable keys"
+                )
 
-def display_diff_hierarchy(diff_hierarchy: list[tuple[ObjectDiff, int]]) -> None:
-    console = Console()
+        index_qks = QueryKeys(qks=unique_keys)
+        search_qks = QueryKeys(qks=searchable_keys)
 
-    for diff, level in diff_hierarchy:
-        title = f"{diff.obj_type.__name__}({diff.object_id}) - State: {diff.status}"
+        return self.partition.find_index_or_search_keys(
+            credentials=credentials,
+            index_qks=index_qks,
+            search_qks=search_qks,
+            order_by=order_by,
+        )
+
+    def query_all_kwargs(
+        self,
+        credentials: SyftVerifyKey,
+        **kwargs: dict[str, Any],
+    ) -> Result[list[BaseStash.object_type], str]:
+        order_by = kwargs.pop("order_by", None)
+        qks = QueryKeys.from_dict(kwargs)
+        return self.query_all(credentials=credentials, qks=qks, order_by=order_by)
+
+    def query_one(
+        self,
+        credentials: SyftVerifyKey,
+        qks: QueryKey | QueryKeys,
+        order_by: PartitionKey | None = None,
+    ) -> Result[BaseStash.object_type | None, str]:
+        return self.query_all(
+            credentials=credentials, qks=qks, order_by=order_by
+        ).and_then(first_or_none)
+
+    def query_one_kwargs(
+        self,
+        credentials: SyftVerifyKey,
+        **kwargs: dict[str, Any],
+    ) -> Result[BaseStash.object_type | None, str]:
+        return self.query_all_kwargs(credentials, **kwargs).and_then(first_or_none)
+
+    def find_all(
+        self, credentials: SyftVerifyKey, **kwargs: dict[str, Any]
+    ) -> Result[list[BaseStash.object_type], str]:
+        return self.query_all_kwargs(credentials=credentials, **kwargs)
+
+    def find_one(
+        self, credentials: SyftVerifyKey, **kwargs: dict[str, Any]
+    ) -> Result[BaseStash.object_type | None, str]:
+        return self.query_one_kwargs(credentials=credentials, **kwargs)
+
+    def find_and_delete(
+        self, credentials: SyftVerifyKey, **kwargs: dict[str, Any]
+    ) -> Result[SyftSuccess, Err]:
+        obj = self.query_one_kwargs(credentials=credentials, **kwargs)
+        if obj.is_err():
+            return obj
+        else:
+            obj = obj.ok()
 
-        low_side_panel = display_diff_object(diff.low_state if diff.low_obj else None)
-        low_side_panel.title = "Low side"
-        low_side_panel.title_align = "left"
-        high_side_panel = display_diff_object(
-            diff.high_state if diff.high_obj is not None else None
+        if not obj:
+            return Err(f"Object does not exists with kwargs: {kwargs}")
+        qk = self.partition.store_query_key(obj)
+        return self.delete(credentials=credentials, qk=qk)
+
+    def delete(
+        self, credentials: SyftVerifyKey, qk: QueryKey, has_permission: bool = False
+    ) -> Result[SyftSuccess, Err]:
+        return self.partition.delete(
+            credentials=credentials, qk=qk, has_permission=has_permission
+        )
+
+    def update(
+        self,
+        credentials: SyftVerifyKey,
+        obj: BaseStash.object_type,
+        has_permission: bool = False,
+    ) -> Result[BaseStash.object_type, str]:
+        qk = self.partition.store_query_key(obj)
+        return self.partition.update(
+            credentials=credentials, qk=qk, obj=obj, has_permission=has_permission
         )
-        high_side_panel.title = "High side"
-        high_side_panel.title_align = "left"
 
-        grouped_panels = Group(low_side_panel, high_side_panel)
 
-        diff_panel = Panel(
-            grouped_panels,
-            title=title,
-            title_align="left",
-            box=box.ROUNDED,
-            expand=False,
-            padding=(1, 2),
+@instrument
+class BaseUIDStoreStash(BaseStash):
+    def delete_by_uid(
+        self, credentials: SyftVerifyKey, uid: UID
+    ) -> Result[SyftSuccess, str]:
+        qk = UIDPartitionKey.with_obj(uid)
+        result = super().delete(credentials=credentials, qk=qk)
+        if result.is_ok():
+            return Ok(SyftSuccess(message=f"ID: {uid} deleted"))
+        return result
+
+    def get_by_uid(
+        self, credentials: SyftVerifyKey, uid: UID
+    ) -> Result[BaseUIDStoreStash.object_type | None, str]:
+        qks = QueryKeys(qks=[UIDPartitionKey.with_obj(uid)])
+        return self.query_one(credentials=credentials, qks=qks)
+
+    def set(
+        self,
+        credentials: SyftVerifyKey,
+        obj: BaseUIDStoreStash.object_type,
+        add_permissions: list[ActionObjectPermission] | None = None,
+        add_storage_permission: bool = True,
+        ignore_duplicates: bool = False,
+    ) -> Result[BaseUIDStoreStash.object_type, str]:
+        res = self.check_type(obj, self.object_type)
+        # we dont use and_then logic here as it is hard because of the order of the arguments
+        if res.is_err():
+            return res
+        return super().set(
+            credentials=credentials,
+            obj=res.ok(),
+            ignore_duplicates=ignore_duplicates,
+            add_permissions=add_permissions,
+            add_storage_permission=add_storage_permission,
         )
 
-        if level > 0:
-            diff_panel = Padding(diff_panel, (0, 0, 0, 5 * level))
 
-        console.print(diff_panel)
+@serializable()
+class StoreConfig(SyftBaseObject):
+    """Base Store configuration
+
+    Parameters:
+        store_type: Type
+            Document Store type
+        client_config: Optional[StoreClientConfig]
+            Backend-specific config
+        locking_config: LockingConfig
+            The config used for store locking. Available options:
+                * NoLockingConfig: no locking, ideal for single-thread stores.
+                * ThreadingLockingConfig: threading-based locking, ideal for same-process in-memory stores.
+                * FileLockingConfig: file based locking, ideal for same-device different-processes/threads stores.
+            Defaults to NoLockingConfig.
+    """
+
+    __canonical_name__ = "StoreConfig"
+    __version__ = SYFT_OBJECT_VERSION_2
+
+    store_type: type[DocumentStore]
+    client_config: StoreClientConfig | None = None
+    locking_config: LockingConfig = Field(default_factory=NoLockingConfig)
```

### Comparing `syft-0.8.6b1/src/syft/service/sync/sync_service.py` & `syft-0.8.7b1/src/syft/service/sync/sync_service.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 # stdlib
 from collections import defaultdict
 from typing import Any
-from typing import cast
 
 # third party
+from result import Ok
 from result import Result
 
 # relative
-from ...abstract_node import AbstractNode
 from ...client.api import NodeIdentity
-from ...node.credentials import SyftVerifyKey
 from ...serde.serializable import serializable
 from ...store.document_store import BaseStash
 from ...store.document_store import DocumentStore
 from ...store.linked_obj import LinkedObject
+from ...types.datetime import DateTime
 from ...types.syft_object import SyftObject
 from ...types.syncable_object import SyncableSyftObject
 from ...types.uid import UID
 from ...util.telemetry import instrument
 from ..action.action_object import ActionObject
 from ..action.action_permissions import ActionObjectPermission
 from ..action.action_permissions import ActionPermission
@@ -54,36 +53,31 @@
         self.store = store
         self.stash = SyncStash(store=store)
 
     def add_actionobject_read_permissions(
         self,
         context: AuthedServiceContext,
         action_object: ActionObject,
-        permissions_other: list[str],
+        new_permissions: list[ActionObjectPermission],
     ) -> None:
-        read_permissions = [x for x in permissions_other if "READ" in x]
-
-        _id = action_object.id.id
         blob_id = action_object.syft_blob_storage_entry_id
 
         store_to = context.node.get_service("actionservice").store  # type: ignore
         store_to_blob = context.node.get_service("blobstorageservice").stash.partition  # type: ignore
 
-        for read_permission in read_permissions:
-            creds, perm_str = read_permission.split("_")
-            perm = ActionPermission[perm_str]
-            permission = ActionObjectPermission(
-                uid=_id, permission=perm, credentials=SyftVerifyKey(creds)
-            )
-            store_to.add_permission(permission)
-
-            permission_blob = ActionObjectPermission(
-                uid=blob_id, permission=perm, credentials=SyftVerifyKey(creds)
-            )
-            store_to_blob.add_permission(permission_blob)
+        for permission in new_permissions:
+            if permission.permission == ActionPermission.READ:
+                store_to.add_permission(permission)
+
+                permission_blob = ActionObjectPermission(
+                    uid=blob_id,
+                    permission=permission.permission,
+                    credentials=permission.credentials,
+                )
+                store_to_blob.add_permission(permission_blob)
 
     def set_obj_ids(self, context: AuthedServiceContext, x: Any) -> None:
         if hasattr(x, "__dict__") and isinstance(x, SyftObject):
             for val in x.__dict__.values():
                 if isinstance(val, list | tuple):
                     for v in val:
                         self.set_obj_ids(context, v)
@@ -94,15 +88,17 @@
                     self.set_obj_ids(context, val)
             x.syft_node_location = context.node.id  # type: ignore
             x.syft_client_verify_key = context.credentials
             if hasattr(x, "node_uid"):
                 x.node_uid = context.node.id  # type: ignore
 
     def transform_item(
-        self, context: AuthedServiceContext, item: SyftObject
+        self,
+        context: AuthedServiceContext,
+        item: SyncableSyftObject,
     ) -> SyftObject:
         if isinstance(item, UserCodeStatusCollection):
             identity = NodeIdentity.from_node(context.node)
             res = {}
             for key in item.status_dict.keys():
                 # todo, check if they are actually only two nodes
                 res[identity] = item.status_dict[key]
@@ -124,41 +120,32 @@
         stash = all_stashes.get(type(item), None)
         return stash
 
     def add_permissions_for_item(
         self,
         context: AuthedServiceContext,
         item: SyftObject,
-        permissions_other: set[ActionObjectPermission],
+        new_permissions: list[ActionObjectPermission],
     ) -> None:
-        if isinstance(item, Job) and context.node.node_side_type.value == "low":  # type: ignore
-            _id = item.id
-            read_permissions = [x for x in permissions_other if "READ" in x]  # type: ignore
-            job_store = context.node.get_service("jobservice").stash.partition  # type: ignore
-            for read_permission in read_permissions:
-                creds, perm_str = read_permission.split("_")
-                perm = ActionPermission[perm_str]
-                permission = ActionObjectPermission(
-                    uid=_id, permission=perm, credentials=SyftVerifyKey(creds)
-                )
-                job_store.add_permission(permission)
+        if isinstance(item, ActionObject):
+            raise ValueError("ActionObject permissions should be added separately")
+        else:
+            store = get_store(context, item)  # type: ignore
+            for permission in new_permissions:
+                if permission.permission == ActionPermission.READ:
+                    store.add_permission(permission)
 
     def add_storage_permissions_for_item(
         self,
         context: AuthedServiceContext,
         item: SyftObject,
-        permissions_other: set[UID],
+        new_permissions: list[StoragePermission],
     ) -> None:
-        _id = item.id.id
-        permissions = [
-            StoragePermission(uid=_id, node_uid=p) for p in permissions_other
-        ]
-
         store = get_store(context, item)
-        store.add_storage_permissions(permissions)
+        store.add_storage_permissions(new_permissions)
 
     def set_object(
         self, context: AuthedServiceContext, item: SyncableSyftObject
     ) -> Result[SyftObject, str]:
         stash = self.get_stash_for_item(context, item)
         creds = context.credentials
 
@@ -179,23 +166,31 @@
         path="sync.sync_items",
         name="sync_items",
         roles=ADMIN_ROLE_LEVEL,
     )
     def sync_items(
         self,
         context: AuthedServiceContext,
-        items: list[ActionObject | SyftObject],
-        permissions: dict[UID, set[str]],
-        storage_permissions: dict[UID, set[UID]],
+        items: list[SyncableSyftObject],
+        permissions: list[ActionObjectPermission],
+        storage_permissions: list[StoragePermission],
+        ignored_batches: dict[UID, int],
+        unignored_batches: set[UID],
     ) -> SyftSuccess | SyftError:
-        permissions = defaultdict(set, permissions)
-        storage_permissions = defaultdict(set, storage_permissions)
+        permissions_dict = defaultdict(list)
+        for permission in permissions:
+            permissions_dict[permission.uid].append(permission)
+
+        storage_permissions_dict = defaultdict(list)
+        for storage_permission in storage_permissions:
+            storage_permissions_dict[storage_permission.uid].append(storage_permission)
+
         for item in items:
-            new_permissions = permissions[item.id.id]
-            new_storage_permissions = storage_permissions[item.id.id]
+            new_permissions = permissions_dict[item.id.id]
+            new_storage_permissions = storage_permissions_dict[item.id.id]
             if isinstance(item, ActionObject):
                 self.add_actionobject_read_permissions(context, item, new_permissions)
                 self.add_storage_permissions_for_item(
                     context, item, new_storage_permissions
                 )
             else:
                 item = self.transform_item(context, item)  # type: ignore[unreachable]
@@ -204,15 +199,31 @@
                 if res.is_ok():
                     self.add_permissions_for_item(context, item, new_permissions)
                     self.add_storage_permissions_for_item(
                         context, item, new_storage_permissions
                     )
                 else:
                     return SyftError(message=f"Failed to sync {res.err()}")
-        return SyftSuccess(message=f"Synced {len(items)} items")
+
+        res = self.build_current_state(
+            context,
+            new_items=items,
+            new_ignored_batches=ignored_batches,
+            new_unignored_batches=unignored_batches,
+        )
+
+        if res.is_err():
+            return SyftError(message=res.message)
+        else:
+            new_state = res.ok()
+            res = self.stash.set(context.credentials, new_state)
+            if res.is_err():
+                return SyftError(message=res.message)
+            else:
+                return SyftSuccess(message=f"Synced {len(items)} items")
 
     @service_method(
         path="sync.get_permissions",
         name="get_permissions",
         roles=ADMIN_ROLE_LEVEL,
     )
     def get_permissions(
@@ -227,71 +238,126 @@
             store = get_store(context, item)
             if store is not None:
                 _id = item.id.id
                 permissions[_id] = store.permissions[_id]
                 storage_permissions[_id] = store.storage_permissions[_id]
         return permissions, storage_permissions
 
-    @service_method(
-        path="sync._get_state",
-        name="_get_state",
-        roles=ADMIN_ROLE_LEVEL,
-    )
-    def _get_state(
-        self, context: AuthedServiceContext, add_to_store: bool = False
-    ) -> SyncState | SyftError:
-        node = cast(AbstractNode, context.node)
-
-        new_state = SyncState(node_uid=node.id)
+    def get_all_syncable_items(
+        self, context: AuthedServiceContext
+    ) -> Result[list[SyncableSyftObject], str]:
+        all_items = []
 
         services_to_sync = [
             "requestservice",
             "usercodeservice",
             "jobservice",
             "logservice",
             "outputservice",
             "usercodestatusservice",
         ]
 
         for service_name in services_to_sync:
-            service = node.get_service(service_name)
+            service = context.node.get_service(service_name)
             items = service.get_all(context)
-            new_state.add_objects(items, api=node.root_client.api)  # type: ignore
+            if isinstance(items, SyftError):
+                return items
+            all_items.extend(items)
 
-        # TODO workaround, we only need action objects from outputs for now
+        # NOTE we only need action objects from outputs for now
         action_object_ids = set()
-        for obj in new_state.objects.values():
+        for obj in all_items:
             if isinstance(obj, ExecutionOutput):
                 action_object_ids |= set(obj.output_id_list)
             elif isinstance(obj, Job) and obj.result is not None:
                 if isinstance(obj.result, ActionObject):
                     obj.result = obj.result.as_empty()
                 action_object_ids.add(obj.result.id)
 
-        action_objects = []
         for uid in action_object_ids:
-            action_object = node.get_service("actionservice").get(context, uid)  # type: ignore
+            action_object = context.node.get_service("actionservice").get(
+                context, uid, resolve_nested=False
+            )  # type: ignore
             if action_object.is_err():
-                return SyftError(message=action_object.err())
-            action_objects.append(action_object.ok())
-        new_state.add_objects(action_objects)
+                return action_object
+            all_items.append(action_object.ok())
 
-        new_state._build_dependencies(api=node.root_client.api)  # type: ignore
+        return Ok(all_items)
 
-        permissions, storage_permissions = self.get_permissions(
-            context, new_state.objects.values()
+    def build_current_state(
+        self,
+        context: AuthedServiceContext,
+        new_items: list[SyncableSyftObject] | None = None,
+        new_ignored_batches: dict[UID, int] | None = None,
+        new_unignored_batches: set[UID] | None = None,
+    ) -> Result[SyncState, str]:
+        new_items = new_items if new_items is not None else []
+        new_ignored_batches = (
+            new_ignored_batches if new_ignored_batches is not None else {}
+        )
+        unignored_batches: set[UID] = (
+            new_unignored_batches if new_unignored_batches is not None else set()
         )
-        new_state.permissions = permissions
-        new_state.storage_permissions = storage_permissions
+        objects_res = self.get_all_syncable_items(context)
+        if objects_res.is_err():
+            return objects_res
+        else:
+            objects = objects_res.ok()
+        permissions, storage_permissions = self.get_permissions(context, objects)
 
         previous_state = self.stash.get_latest(context=context)
+        if previous_state.is_err():
+            return previous_state
+        previous_state = previous_state.ok()
+
         if previous_state is not None:
-            new_state.previous_state_link = LinkedObject.from_obj(
+            previous_state_link = LinkedObject.from_obj(
                 obj=previous_state,
                 service_type=SyncService,
                 node_uid=context.node.id,  # type: ignore
             )
+            previous_ignored_batches = previous_state.ignored_batches
+        else:
+            previous_state_link = None
+            previous_ignored_batches = {}
 
-        if add_to_store:
-            self.stash.set(context.credentials, new_state)
+        ignored_batches = {
+            **previous_ignored_batches,
+            **new_ignored_batches,
+        }
+
+        ignored_batches = {
+            k: v for k, v in ignored_batches.items() if k not in unignored_batches
+        }
+
+        object_sync_dates = (
+            previous_state.object_sync_dates.copy() if previous_state else {}
+        )
+        for obj in new_items:
+            object_sync_dates[obj.id.id] = DateTime.now()
 
-        return new_state
+        new_state = SyncState(
+            node_uid=context.node.id,  # type: ignore
+            node_name=context.node.name,  # type: ignore
+            node_side_type=context.node.node_side_type,  # type: ignore
+            previous_state_link=previous_state_link,
+            permissions=permissions,
+            storage_permissions=storage_permissions,
+            ignored_batches=ignored_batches,
+            object_sync_dates=object_sync_dates,
+        )
+
+        new_state.add_objects(objects, context)
+
+        return Ok(new_state)
+
+    @service_method(
+        path="sync._get_state",
+        name="_get_state",
+        roles=ADMIN_ROLE_LEVEL,
+    )
+    def _get_state(self, context: AuthedServiceContext) -> SyncState | SyftError:
+        res = self.build_current_state(context)
+        if res.is_err():
+            return SyftError(message=res.value)
+        else:
+            return res.ok()
```

### Comparing `syft-0.8.6b1/src/syft/service/sync/sync_stash.py` & `syft-0.8.7b1/src/syft/service/sync/sync_stash.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,24 @@
 # stdlib
 
+# stdlib
+
+# third party
+from result import Ok
+from result import Result
+
 # relative
 from ...serde.serializable import serializable
 from ...store.document_store import BaseUIDStoreStash
 from ...store.document_store import DocumentStore
 from ...store.document_store import PartitionKey
 from ...store.document_store import PartitionSettings
 from ...types.datetime import DateTime
 from ...util.telemetry import instrument
 from ..context import AuthedServiceContext
-from ..response import SyftError
 from .sync_state import SyncState
 
 OrderByDatePartitionKey = PartitionKey(key="created_at", type_=DateTime)
 
 
 @instrument
 @serializable()
@@ -26,20 +31,22 @@
 
     def __init__(self, store: DocumentStore):
         super().__init__(store)
         self.store = store
         self.settings = self.settings
         self._object_type = self.object_type
 
-    def get_latest(self, context: AuthedServiceContext) -> SyncState | None | SyftError:
+    def get_latest(
+        self, context: AuthedServiceContext
+    ) -> Result[SyncState | None, str]:
         all_states = self.get_all(
             credentials=context.node.verify_key,  # type: ignore
             order_by=OrderByDatePartitionKey,
         )
 
         if all_states.is_err():
-            return SyftError(message=all_states.err())
+            return all_states
 
         all_states = all_states.ok()
         if len(all_states) > 0:
-            return all_states[-1]
-        return None
+            return Ok(all_states[-1])
+        return Ok(None)
```

### Comparing `syft-0.8.6b1/src/syft/service/user/user.py` & `syft-0.8.7b1/src/syft/store/blob_storage/seaweedfs.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,361 +1,303 @@
 # stdlib
-from collections.abc import Callable
-from getpass import getpass
+from collections.abc import Generator
+from io import BytesIO
+import math
+from queue import Queue
+import threading
 from typing import Any
 
 # third party
-from bcrypt import checkpw
-from bcrypt import gensalt
-from bcrypt import hashpw
-from pydantic import EmailStr
-from pydantic import ValidationError
-from pydantic import field_validator
+import boto3
+from botocore.client import BaseClient as S3BaseClient
+from botocore.client import ClientError as BotoClientError
+from botocore.client import Config
+import requests
+from tqdm import tqdm
+from typing_extensions import Self
 
 # relative
-from ...client.api import APIRegistry
-from ...node.credentials import SyftSigningKey
-from ...node.credentials import SyftVerifyKey
+from . import BlobDeposit
+from . import BlobRetrieval
+from . import BlobStorageClient
+from . import BlobStorageClientConfig
+from . import BlobStorageConfig
+from . import BlobStorageConnection
 from ...serde.serializable import serializable
-from ...types.syft_metaclass import Empty
-from ...types.syft_object import PartialSyftObject
-from ...types.syft_object import SYFT_OBJECT_VERSION_2
+from ...service.blob_storage.remote_profile import AzureRemoteProfile
+from ...service.response import SyftError
+from ...service.response import SyftSuccess
+from ...service.service import from_api_or_context
+from ...types.blob_storage import BlobStorageEntry
+from ...types.blob_storage import CreateBlobStorageEntry
+from ...types.blob_storage import SeaweedSecureFilePathLocation
+from ...types.blob_storage import SecureFilePathLocation
+from ...types.grid_url import GridURL
 from ...types.syft_object import SYFT_OBJECT_VERSION_3
-from ...types.syft_object import SyftObject
-from ...types.transforms import TransformContext
-from ...types.transforms import drop
-from ...types.transforms import generate_id
-from ...types.transforms import keep
-from ...types.transforms import make_set_default
-from ...types.transforms import transform
-from ...types.transforms import validate_email
-from ...types.uid import UID
-from ..notifier.notifier_enums import NOTIFIERS
-from ..response import SyftError
-from ..response import SyftSuccess
-from .user_roles import ServiceRole
+from ...util.constants import DEFAULT_TIMEOUT
+
+WRITE_EXPIRATION_TIME = 900  # seconds
+DEFAULT_FILE_PART_SIZE = (1024**3) * 5  # 5GB
+DEFAULT_UPLOAD_CHUNK_SIZE = 819200
 
 
 @serializable()
-class User(SyftObject):
-    # version
-    __canonical_name__ = "User"
+class SeaweedFSBlobDeposit(BlobDeposit):
+    __canonical_name__ = "SeaweedFSBlobDeposit"
     __version__ = SYFT_OBJECT_VERSION_3
 
-    id: UID | None = None  # type: ignore[assignment]
-
-    # fields
-    notifications_enabled: dict[NOTIFIERS, bool] = {
-        NOTIFIERS.EMAIL: True,
-        NOTIFIERS.SMS: False,
-        NOTIFIERS.SLACK: False,
-        NOTIFIERS.APP: False,
-    }
-    email: EmailStr | None = None
-    name: str | None = None
-    hashed_password: str | None = None
-    salt: str | None = None
-    signing_key: SyftSigningKey | None = None
-    verify_key: SyftVerifyKey | None = None
-    role: ServiceRole | None = None
-    institution: str | None = None
-    website: str | None = None
-    created_at: str | None = None
-    # TODO where do we put this flag?
-    mock_execution_permission: bool = False
-
-    # serde / storage rules
-    __attr_searchable__ = ["name", "email", "verify_key", "role"]
-    __attr_unique__ = ["email", "signing_key", "verify_key"]
-    __repr_attrs__ = ["name", "email"]
-
-
-def default_role(role: ServiceRole) -> Callable:
-    return make_set_default(key="role", value=role)
-
-
-def hash_password(context: TransformContext) -> TransformContext:
-    if context.output is None:
-        return context
-
-    if context.output["password"] is not None and (
-        (context.output["password_verify"] is None)
-        or context.output["password"] == context.output["password_verify"]
-    ):
-        salt, hashed = salt_and_hash_password(context.output["password"], 12)
-        context.output["hashed_password"] = hashed
-        context.output["salt"] = salt
-
-    return context
+    urls: list[GridURL]
+    size: int
 
+    def write(self, data: BytesIO) -> SyftSuccess | SyftError:
+        # relative
+        from ...client.api import APIRegistry
 
-def generate_key(context: TransformContext) -> TransformContext:
-    if context.output is not None:
-        signing_key = SyftSigningKey.generate()
-        context.output["signing_key"] = signing_key
-        context.output["verify_key"] = signing_key.verify_key
-
-    return context
-
-
-def salt_and_hash_password(password: str, rounds: int) -> tuple[str, str]:
-    bytes_pass = password.encode("UTF-8")
-    salt = gensalt(rounds=rounds)
-    hashed = hashpw(bytes_pass, salt)
-    hashed_bytes = hashed.decode("UTF-8")
-    salt_bytes = salt.decode("UTF-8")
-    return salt_bytes, hashed_bytes
+        api = APIRegistry.api_for(
+            node_uid=self.syft_node_location,
+            user_verify_key=self.syft_client_verify_key,
+        )
 
+        etags = []
 
-def check_pwd(password: str, hashed_password: str) -> bool:
-    return checkpw(
-        password=password.encode("utf-8"),
-        hashed_password=hashed_password.encode("utf-8"),
-    )
+        try:
+            no_lines = 0
+            # this loops over the parts, we have multiple parts to allow for
+            # concurrent uploads of a single file. (We are currently not using that)
+            # a part may for instance be 5GB
+            # parts are then splitted into chunks which are MBs (order of magnitude)
+            part_size = math.ceil(self.size / len(self.urls))
+            chunk_size = DEFAULT_UPLOAD_CHUNK_SIZE
+
+            # this is the total nr of chunks in all parts
+            total_iterations = math.ceil(part_size / chunk_size) * len(self.urls)
+
+            with tqdm(
+                total=total_iterations,
+                desc=f"Uploading progress",  # noqa
+            ) as pbar:
+                for part_no, url in enumerate(
+                    self.urls,
+                    start=1,
+                ):
+                    if api is not None and api.connection is not None:
+                        blob_url = api.connection.to_blob_route(
+                            url.url_path, host=url.host_or_ip
+                        )
+                    else:
+                        blob_url = url
+
+                    # read a chunk untill we have read part_size
+                    class PartGenerator:
+                        def __init__(self) -> None:
+                            self.no_lines = 0
+
+                        def async_generator(
+                            self, chunk_size: int = DEFAULT_UPLOAD_CHUNK_SIZE
+                        ) -> Generator:
+                            item_queue: Queue = Queue()
+                            threading.Thread(
+                                target=self.add_chunks_to_queue,
+                                kwargs={"queue": item_queue, "chunk_size": chunk_size},
+                                daemon=True,
+                            ).start()
+                            item = item_queue.get()
+                            while item != 0:
+                                yield item
+                                pbar.update(1)
+                                item = item_queue.get()
+
+                        def add_chunks_to_queue(
+                            self,
+                            queue: Queue,
+                            chunk_size: int = DEFAULT_UPLOAD_CHUNK_SIZE,
+                        ) -> None:
+                            """Creates a data geneator for the part"""
+                            n = 0
+
+                            while n * chunk_size <= part_size:
+                                try:
+                                    chunk = data.read(chunk_size)
+                                    self.no_lines += chunk.count(b"\n")
+                                    n += 1
+                                    queue.put(chunk)
+                                except BlockingIOError:
+                                    # if end of file, stop
+                                    queue.put(0)
+                            # if end of part, stop
+                            queue.put(0)
+
+                    gen = PartGenerator()
+
+                    response = requests.put(
+                        url=str(blob_url),
+                        data=gen.async_generator(chunk_size),
+                        timeout=DEFAULT_TIMEOUT,
+                        stream=True,
+                    )
+
+                    response.raise_for_status()
+                    no_lines += gen.no_lines
+                    etag = response.headers["ETag"]
+                    etags.append({"ETag": etag, "PartNumber": part_no})
+
+        except requests.RequestException as e:
+            print(e)
+            return SyftError(message=str(e))
+
+        mark_write_complete_method = from_api_or_context(
+            func_or_path="blob_storage.mark_write_complete",
+            syft_node_location=self.syft_node_location,
+            syft_client_verify_key=self.syft_client_verify_key,
+        )
+        if mark_write_complete_method is None:
+            return SyftError(message="mark_write_complete_method is None")
+        return mark_write_complete_method(
+            etags=etags, uid=self.blob_storage_entry_id, no_lines=no_lines
+        )
 
 
 @serializable()
-class UserUpdate(PartialSyftObject):
-    __canonical_name__ = "UserUpdate"
-    __version__ = SYFT_OBJECT_VERSION_3
-
-    @field_validator("role", mode="before")
-    @classmethod
-    def str_to_role(cls, v: Any) -> Any:
-        if isinstance(v, str) and hasattr(ServiceRole, v.upper()):
-            return getattr(ServiceRole, v.upper())
-        return v
-
-    email: EmailStr
-    name: str
-    role: ServiceRole  # make sure role cant be set without uid
-    password: str
-    password_verify: str
-    verify_key: SyftVerifyKey
-    institution: str
-    website: str
-    mock_execution_permission: bool
+class SeaweedFSClientConfig(BlobStorageClientConfig):
+    host: str
+    port: int
+    mount_port: int | None = None
+    access_key: str
+    secret_key: str
+    region: str
+    default_bucket_name: str = "defaultbucket"
+    remote_profiles: dict[str, AzureRemoteProfile] = {}
+
+    @property
+    def endpoint_url(self) -> str:
+        grid_url = GridURL(host_or_ip=self.host, port=self.port)
+        return grid_url.url
+
+    @property
+    def mount_url(self) -> str:
+        if self.mount_port is None:
+            raise ValueError("Seaweed should be configured with a mount port to mount")
+        return f"http://{self.host}:{self.mount_port}/configure_azure"
 
 
 @serializable()
-class UserCreate(SyftObject):
-    __canonical_name__ = "UserCreate"
-    __version__ = SYFT_OBJECT_VERSION_3
+class SeaweedFSClient(BlobStorageClient):
+    config: SeaweedFSClientConfig
 
-    email: EmailStr
-    name: str
-    role: ServiceRole | None = None  # type: ignore[assignment]
-    password: str
-    password_verify: str | None = None  # type: ignore[assignment]
-    verify_key: SyftVerifyKey | None = None  # type: ignore[assignment]
-    institution: str | None = ""  # type: ignore[assignment]
-    website: str | None = ""  # type: ignore[assignment]
-    created_by: SyftSigningKey | None = None  # type: ignore[assignment]
-    mock_execution_permission: bool = False
-
-    __repr_attrs__ = ["name", "email"]
+    def connect(self) -> BlobStorageConnection:
+        return SeaweedFSConnection(
+            client=boto3.client(
+                "s3",
+                endpoint_url=self.config.endpoint_url,
+                aws_access_key_id=self.config.access_key,
+                aws_secret_access_key=self.config.secret_key,
+                config=Config(signature_version="s3v4"),
+                region_name=self.config.region,
+            ),
+            default_bucket_name=self.config.default_bucket_name,
+            config=self.config,
+        )
 
 
 @serializable()
-class UserSearch(PartialSyftObject):
-    __canonical_name__ = "UserSearch"
-    __version__ = SYFT_OBJECT_VERSION_2
-
-    id: UID
-    email: EmailStr
-    verify_key: SyftVerifyKey
-    name: str
+class SeaweedFSConnection(BlobStorageConnection):
+    client: S3BaseClient
+    default_bucket_name: str
+    config: SeaweedFSClientConfig
 
+    def __init__(
+        self,
+        client: S3BaseClient,
+        default_bucket_name: str,
+        config: SeaweedFSClientConfig,
+    ):
+        self.client = client
+        self.default_bucket_name = default_bucket_name
+        self.config = config
 
-@serializable()
-class UserView(SyftObject):
-    __canonical_name__ = "UserView"
-    __version__ = SYFT_OBJECT_VERSION_3
+    def __enter__(self) -> Self:
+        return self
 
-    notifications_enabled: dict[NOTIFIERS, bool] = {
-        NOTIFIERS.EMAIL: True,
-        NOTIFIERS.SMS: False,
-        NOTIFIERS.SLACK: False,
-        NOTIFIERS.APP: False,
-    }
-    email: EmailStr
-    name: str
-    role: ServiceRole  # make sure role cant be set without uid
-    institution: str | None = None
-    website: str | None = None
-    mock_execution_permission: bool
-
-    __repr_attrs__ = [
-        "name",
-        "email",
-        "institution",
-        "website",
-        "role",
-        "notifications_enabled",
-    ]
-
-    def _coll_repr_(self) -> dict[str, Any]:
-        return {
-            "Name": self.name,
-            "Email": self.email,
-            "Institute": self.institution,
-            "Website": self.website,
-            "Role": self.role.name.capitalize(),
-            "Notifications": "Email: "
-            + (
-                "Enabled" if self.notifications_enabled[NOTIFIERS.EMAIL] else "Disabled"
-            ),
-        }
+    def __exit__(self, *exc: Any) -> None:
+        self.client.close()
 
-    def _set_password(self, new_password: str) -> SyftError | SyftSuccess:
-        api = APIRegistry.api_for(
-            node_uid=self.syft_node_location,
-            user_verify_key=self.syft_client_verify_key,
-        )
-        if api is None:
-            return SyftError(message=f"You must login to {self.node_uid}")
-
-        api.services.user.update(
-            uid=self.id, user_update=UserUpdate(password=new_password)
-        )
-        return SyftSuccess(
-            message=f"Successfully updated password for "
-            f"user '{self.name}' with email '{self.email}'."
+    def read(
+        self,
+        fp: SecureFilePathLocation,
+        type_: type | None,
+        bucket_name: str | None = None,
+    ) -> BlobRetrieval:
+        if bucket_name is None:
+            bucket_name = self.default_bucket_name
+        # this will generate the url, the SecureFilePathLocation also handles the logic
+        # that decides whether to use a direct connection to azure/aws/gcp or via seaweed
+        return fp.generate_url(self, type_, bucket_name)
+
+    def allocate(
+        self, obj: CreateBlobStorageEntry
+    ) -> SecureFilePathLocation | SyftError:
+        try:
+            file_name = obj.file_name
+            result = self.client.create_multipart_upload(
+                Bucket=self.default_bucket_name,
+                Key=file_name,
+            )
+            upload_id = result["UploadId"]
+            return SeaweedSecureFilePathLocation(upload_id=upload_id, path=file_name)
+        except BotoClientError as e:
+            return SyftError(
+                message=f"Failed to allocate space for {obj} with error: {e}"
+            )
+
+    def write(self, obj: BlobStorageEntry) -> BlobDeposit:
+        total_parts = math.ceil(obj.file_size / DEFAULT_FILE_PART_SIZE)
+
+        urls = [
+            GridURL.from_url(
+                self.client.generate_presigned_url(
+                    ClientMethod="upload_part",
+                    Params={
+                        "Bucket": self.default_bucket_name,
+                        "Key": obj.location.path,
+                        "UploadId": obj.location.upload_id,
+                        "PartNumber": i + 1,
+                    },
+                    ExpiresIn=WRITE_EXPIRATION_TIME,
+                )
+            )
+            for i in range(total_parts)
+        ]
+        return SeaweedFSBlobDeposit(
+            blob_storage_entry_id=obj.id, urls=urls, size=obj.file_size
         )
 
-    def set_password(
-        self, new_password: str | None = None, confirm: bool = True
+    def complete_multipart_upload(
+        self,
+        blob_entry: BlobStorageEntry,
+        etags: list,
     ) -> SyftError | SyftSuccess:
-        """Set a new password interactively with confirmed password from user input"""
-        # TODO: Add password validation for special characters
-        if not new_password:
-            new_password = getpass("New Password: ")
-
-        if confirm:
-            confirmed_password: str = getpass("Please confirm your password: ")
-            if confirmed_password != new_password:
-                return SyftError(message="Passwords do not match !")
-        return self._set_password(new_password)
-
-    def set_email(self, email: str) -> SyftSuccess | SyftError:
-        # validate email address
-        api = APIRegistry.api_for(
-            node_uid=self.syft_node_location,
-            user_verify_key=self.syft_client_verify_key,
-        )
-        if api is None:
-            return SyftError(message=f"You must login to {self.node_uid}")
-
         try:
-            user_update = UserUpdate(email=email)
-        except ValidationError:
-            return SyftError(message="{email} is not a valid email address.")
-
-        result = api.services.user.update(uid=self.id, user_update=user_update)
-
-        if isinstance(result, SyftError):
-            return result
-
-        self.email = email
-        return SyftSuccess(
-            message=f"Successfully updated email for the user "
-            f"'{self.name}' to '{self.email}'."
-        )
+            self.client.complete_multipart_upload(
+                Bucket=self.default_bucket_name,
+                Key=blob_entry.location.path,
+                MultipartUpload={"Parts": etags},
+                UploadId=blob_entry.location.upload_id,
+            )
+            return SyftSuccess(message="Successfully saved file.")
+        except BotoClientError as e:
+            return SyftError(message=str(e))
 
-    def update(
+    def delete(
         self,
-        name: type[Empty] | str = Empty,
-        institution: type[Empty] | str = Empty,
-        website: type[Empty] | str = Empty,
-        role: type[Empty] | str = Empty,
-        mock_execution_permission: type[Empty] | bool = Empty,
+        fp: SecureFilePathLocation,
     ) -> SyftSuccess | SyftError:
-        """Used to update name, institution, website of a user."""
-        api = APIRegistry.api_for(
-            node_uid=self.syft_node_location,
-            user_verify_key=self.syft_client_verify_key,
-        )
-        if api is None:
-            return SyftError(message=f"You must login to {self.node_uid}")
-        user_update = UserUpdate(
-            name=name,
-            institution=institution,
-            website=website,
-            role=role,
-            mock_execution_permission=mock_execution_permission,
-        )
-        result = api.services.user.update(uid=self.id, user_update=user_update)
-
-        if isinstance(result, SyftError):
-            return result
-
-        for attr, val in result.to_dict(exclude_empty=True).items():
-            setattr(self, attr, val)
-
-        return SyftSuccess(message="User details successfully updated.")
-
-    def allow_mock_execution(self, allow: bool = True) -> SyftSuccess | SyftError:
-        return self.update(mock_execution_permission=allow)
-
-
-@serializable()
-class UserViewPage(SyftObject):
-    __canonical_name__ = "UserViewPage"
-    __version__ = SYFT_OBJECT_VERSION_2
-
-    users: list[UserView]
-    total: int
-
-
-@transform(UserUpdate, User)
-def user_update_to_user() -> list[Callable]:
-    return [
-        validate_email,
-        hash_password,
-        drop(["password", "password_verify"]),
-    ]
-
-
-@transform(UserCreate, User)
-def user_create_to_user() -> list[Callable]:
-    return [
-        generate_id,
-        validate_email,
-        hash_password,
-        generate_key,
-        drop(["password", "password_verify", "created_by"]),
-        # TODO: Fix this by passing it from client & verifying it at server
-        default_role(ServiceRole.DATA_SCIENTIST),
-    ]
-
-
-@transform(User, UserView)
-def user_to_view_user() -> list[Callable]:
-    return [
-        keep(
-            [
-                "id",
-                "email",
-                "name",
-                "role",
-                "institution",
-                "website",
-                "mock_execution_permission",
-                "notifications_enabled",
-            ]
-        )
-    ]
+        try:
+            self.client.delete_object(Bucket=self.default_bucket_name, Key=fp.path)
+            return SyftSuccess(message="Successfully deleted file.")
+        except BotoClientError as e:
+            return SyftError(message=str(e))
 
 
 @serializable()
-class UserPrivateKey(SyftObject):
-    __canonical_name__ = "UserPrivateKey"
-    __version__ = SYFT_OBJECT_VERSION_2
-
-    email: str
-    signing_key: SyftSigningKey
-    role: ServiceRole
-
-
-@transform(User, UserPrivateKey)
-def user_to_user_verify() -> list[Callable]:
-    return [keep(["email", "signing_key", "id", "role"])]
+class SeaweedFSConfig(BlobStorageConfig):
+    client_type: type[BlobStorageClient] = SeaweedFSClient
+    client_config: SeaweedFSClientConfig
```

### Comparing `syft-0.8.6b1/src/syft/service/user/user_roles.py` & `syft-0.8.7b1/src/syft/service/user/user_roles.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6b1/src/syft/service/user/user_service.py` & `syft-0.8.7b1/src/syft/service/user/user_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 # stdlib
-from typing import cast
 
 # relative
-from ...abstract_node import AbstractNode
 from ...abstract_node import NodeType
 from ...exceptions.user import UserAlreadyExistsException
 from ...node.credentials import SyftSigningKey
 from ...node.credentials import SyftVerifyKey
 from ...node.credentials import UserLoginCredentials
 from ...serde.serializable import serializable
 from ...store.document_store import DocumentStore
@@ -269,15 +267,15 @@
             else:
                 return SyftError(
                     message=f"As a {context.role}, you are not allowed to edit {user.role} to {user_update.role}"
                 )
 
         edits_non_role_attrs = any(
             getattr(user_update, attr) is not Empty
-            for attr in user_update.dict()
+            for attr in user_update.to_dict()
             if attr != "role"
         )
 
         if (
             edits_non_role_attrs
             and user.verify_key != context.credentials
             and ServiceRoleCapability.CAN_MANAGE_USERS not in context.capabilities()
@@ -411,16 +409,14 @@
             return SyftError(message=str(e))
 
     def register(
         self, context: NodeServiceContext, new_user: UserCreate
     ) -> tuple[SyftSuccess, UserPrivateKey] | SyftError:
         """Register new user"""
 
-        context.node = cast(AbstractNode, context.node)
-
         request_user_role = (
             ServiceRole.GUEST
             if new_user.created_by is None
             else self.get_role_for_credentials(new_user.created_by)
         )
 
         can_user_register = (
```

### Comparing `syft-0.8.6b1/src/syft/service/user/user_stash.py` & `syft-0.8.7b1/src/syft/service/user/user_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6b1/src/syft/service/veilid/veilid_service.py` & `syft-0.8.7b1/src/syft/service/veilid/veilid_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6b1/src/syft/service/warnings.py` & `syft-0.8.7b1/src/syft/service/warnings.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6b1/src/syft/service/worker/image_identifier.py` & `syft-0.8.7b1/src/syft/service/worker/image_identifier.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6b1/src/syft/service/worker/image_registry.py` & `syft-0.8.7b1/src/syft/service/worker/image_registry.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6b1/src/syft/service/worker/image_registry_service.py` & `syft-0.8.7b1/src/syft/service/worker/image_registry_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6b1/src/syft/service/worker/image_registry_stash.py` & `syft-0.8.7b1/src/syft/service/worker/image_registry_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6b1/src/syft/service/worker/utils.py` & `syft-0.8.7b1/src/syft/service/worker/utils.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6b1/src/syft/service/worker/worker.py` & `syft-0.8.7b1/src/syft/service/worker/worker.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6b1/src/syft/service/worker/worker_image.py` & `syft-0.8.7b1/src/syft/service/worker/worker_image.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6b1/src/syft/service/worker/worker_image_service.py` & `syft-0.8.7b1/src/syft/service/worker/worker_image_service.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 # stdlib
 import contextlib
-from typing import cast
 
 # third party
 import docker
 import pydantic
 
 # relative
-from ...abstract_node import AbstractNode
 from ...custom_worker.config import DockerWorkerConfig
 from ...custom_worker.k8s import IN_KUBERNETES
 from ...serde.serializable import serializable
 from ...store.document_store import DocumentStore
 from ...types.datetime import DateTime
 from ...types.dicttuple import DictTuple
 from ...types.uid import UID
@@ -72,16 +70,14 @@
         image_uid: UID,
         tag: str,
         registry_uid: UID | None = None,
         pull: bool = True,
     ) -> SyftSuccess | SyftError:
         registry: SyftImageRegistry | None = None
 
-        context.node = cast(AbstractNode, context.node)
-
         if IN_KUBERNETES and registry_uid is None:
             return SyftError(message="Registry UID is required in Kubernetes mode.")
 
         result = self.stash.get_by_uid(credentials=context.credentials, uid=image_uid)
         if result.is_err():
             return SyftError(
                 message=f"Failed to get image for uid: {image_uid}. Error: {result.err()}"
@@ -226,15 +222,14 @@
     ) -> SyftSuccess | SyftError:
         #  Delete Docker image given image tag
         res = self.stash.get_by_uid(credentials=context.credentials, uid=uid)
         if res.is_err():
             return SyftError(message=f"{res.err()}")
         image: SyftWorkerImage = res.ok()
 
-        context.node = cast(AbstractNode, context.node)
         if context.node.in_memory_workers:
             pass
         elif IN_KUBERNETES:
             # TODO: Implement image deletion in kubernetes
             return SyftError(
                 message="Image Deletion is not yet implemented in Kubernetes !!"
             )
```

### Comparing `syft-0.8.6b1/src/syft/service/worker/worker_image_stash.py` & `syft-0.8.7b1/src/syft/service/worker/worker_image_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6b1/src/syft/service/worker/worker_pool.py` & `syft-0.8.7b1/src/syft/service/worker/worker_pool.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,16 +15,16 @@
 from ...types.datetime import DateTime
 from ...types.syft_object import SYFT_OBJECT_VERSION_2
 from ...types.syft_object import SyftObject
 from ...types.syft_object import short_uid
 from ...types.uid import UID
 from ...util import options
 from ...util.colors import SURFACE
+from ...util.fonts import FONT_CSS
 from ...util.fonts import ITABLES_CSS
-from ...util.fonts import fonts_css
 from ..response import SyftError
 from .worker_image import SyftWorkerImage
 
 
 @serializable()
 class WorkerStatus(Enum):
     PENDING = "Pending"
@@ -212,15 +212,15 @@
             "Image": image_name_with_tag,
             "Created at": str(self.created_at),
         }
 
     def _repr_html_(self) -> Any:
         return f"""
             <style>
-            {fonts_css}
+            {FONT_CSS}
             .syft-dataset {{color: {SURFACE[options.color_theme]};}}
             .syft-dataset h3,
             .syft-dataset p
               {{font-family: 'Open Sans';}}
               {ITABLES_CSS}
             </style>
             <div class='syft-dataset'>
```

### Comparing `syft-0.8.6b1/src/syft/service/worker/worker_pool_service.py` & `syft-0.8.7b1/src/syft/service/worker/worker_pool_service.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 # stdlib
 from typing import Any
-from typing import cast
 
 # third party
 import pydantic
 from result import OkErr
 
 # relative
-from ...abstract_node import AbstractNode
 from ...custom_worker.config import CustomWorkerConfig
 from ...custom_worker.config import WorkerConfig
 from ...custom_worker.k8s import IN_KUBERNETES
 from ...custom_worker.runner_k8s import KubernetesRunner
 from ...serde.serializable import serializable
 from ...store.document_store import DocumentStore
 from ...store.linked_obj import LinkedObject
@@ -108,15 +106,15 @@
         )
         if result.is_err():
             return SyftError(
                 message=f"Failed to retrieve Worker Image with id: {image_uid}. Error: {result.err()}"
             )
 
         worker_image: SyftWorkerImage = result.ok()
-        context.node = cast(AbstractNode, context.node)
+
         worker_service: AbstractService = context.node.get_service("WorkerService")
         worker_stash = worker_service.stash
 
         # Create worker pool from given image, with the given worker pool
         # and with the desired number of workers
         result = _create_workers_in_pool(
             context=context,
@@ -214,15 +212,15 @@
         )
 
         changes: list[Change] = [create_worker_pool_change]
 
         # Create a the request object with the changes and submit it
         # for approval.
         request = SubmitRequest(changes=changes)
-        context.node = cast(AbstractNode, context.node)
+
         method = context.node.get_service_method(RequestService.submit)
         result = method(context=context, request=request, reason=reason)
 
         return result
 
     @service_method(
         path="worker_pool.create_image_and_pool_request",
@@ -314,15 +312,15 @@
             num_workers=num_workers,
             config=config,
         )
         changes += [create_custom_image_change, create_worker_pool_change]
 
         # Create a request object and submit a request for approval
         request = SubmitRequest(changes=changes)
-        context.node = cast(AbstractNode, context.node)
+
         method = context.node.get_service_method(RequestService.submit)
         result = method(context=context, request=request, reason=reason)
 
         return result
 
     @service_method(
         path="worker_pool.get_all",
@@ -399,15 +397,14 @@
         if result.is_err():
             return SyftError(
                 message=f"Failed to retrieve image for worker pool: {worker_pool.name}"
             )
 
         worker_image: SyftWorkerImage = result.ok()
 
-        context.node = cast(AbstractNode, context.node)
         worker_service: AbstractService = context.node.get_service("WorkerService")
         worker_stash = worker_service.stash
 
         # Add workers to given pool from the given image
         result = _create_workers_in_pool(
             context=context,
             pool_name=worker_pool.name,
@@ -449,15 +446,15 @@
         pool_id: UID | None = None,
         pool_name: str | None = None,
     ) -> SyftError | SyftSuccess:
         """
         Scale the worker pool to the given number of workers in Kubernetes.
         Allows both scaling up and down the worker pool.
         """
-        context.node = cast(AbstractNode, context.node)
+
         if not IN_KUBERNETES:
             return SyftError(message="Scaling is only supported in Kubernetes mode")
         elif number < 0:
             # zero is a valid scale down
             return SyftError(message=f"Invalid number of workers: {number}")
 
         result: Any = self._get_worker_pool(context, pool_id, pool_name)
@@ -645,15 +642,14 @@
     existing_worker_cnt: int,
     worker_cnt: int,
     worker_image: SyftWorkerImage,
     worker_stash: WorkerStash,
     reg_username: str | None = None,
     reg_password: str | None = None,
 ) -> tuple[list[LinkedObject], list[ContainerSpawnStatus]] | SyftError:
-    context.node = cast(AbstractNode, context.node)
     queue_port = context.node.queue_config.client_config.queue_port
 
     # Check if workers needs to be run in memory or as containers
     start_workers_in_memory = context.node.in_memory_workers
 
     if start_workers_in_memory:
         # Run in-memory workers in threads
```

### Comparing `syft-0.8.6b1/src/syft/service/worker/worker_pool_stash.py` & `syft-0.8.7b1/src/syft/service/worker/worker_stash.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,65 +1,81 @@
 # stdlib
 
 # third party
+from result import Err
+from result import Ok
 from result import Result
 
 # relative
 from ...node.credentials import SyftVerifyKey
 from ...serde.serializable import serializable
 from ...store.document_store import BaseUIDStoreStash
 from ...store.document_store import DocumentStore
 from ...store.document_store import PartitionKey
 from ...store.document_store import PartitionSettings
 from ...store.document_store import QueryKeys
 from ...types.uid import UID
+from ...util.telemetry import instrument
 from ..action.action_permissions import ActionObjectPermission
 from ..action.action_permissions import ActionPermission
-from .worker_pool import WorkerPool
+from .worker_pool import ConsumerState
+from .worker_pool import SyftWorker
 
-PoolNamePartitionKey = PartitionKey(key="name", type_=str)
-PoolImageIDPartitionKey = PartitionKey(key="image_id", type_=UID)
+WorkerContainerNamePartitionKey = PartitionKey(key="container_name", type_=str)
 
 
+@instrument
 @serializable()
-class SyftWorkerPoolStash(BaseUIDStoreStash):
-    object_type = WorkerPool
+class WorkerStash(BaseUIDStoreStash):
+    object_type = SyftWorker
     settings: PartitionSettings = PartitionSettings(
-        name=WorkerPool.__canonical_name__,
-        object_type=WorkerPool,
+        name=SyftWorker.__canonical_name__, object_type=SyftWorker
     )
 
     def __init__(self, store: DocumentStore) -> None:
         super().__init__(store=store)
 
-    def get_by_name(
-        self, credentials: SyftVerifyKey, pool_name: str
-    ) -> Result[WorkerPool | None, str]:
-        qks = QueryKeys(qks=[PoolNamePartitionKey.with_obj(pool_name)])
-        return self.query_one(credentials=credentials, qks=qks)
-
     def set(
         self,
         credentials: SyftVerifyKey,
-        obj: WorkerPool,
+        obj: SyftWorker,
         add_permissions: list[ActionObjectPermission] | None = None,
         add_storage_permission: bool = True,
         ignore_duplicates: bool = False,
-    ) -> Result[WorkerPool, str]:
+    ) -> Result[SyftWorker, str]:
         # By default all worker pools have all read permission
         add_permissions = [] if add_permissions is None else add_permissions
         add_permissions.append(
             ActionObjectPermission(uid=obj.id, permission=ActionPermission.ALL_READ)
         )
         return super().set(
             credentials,
             obj,
             add_permissions=add_permissions,
-            add_storage_permission=add_storage_permission,
             ignore_duplicates=ignore_duplicates,
+            add_storage_permission=add_storage_permission,
         )
 
-    def get_by_image_uid(
-        self, credentials: SyftVerifyKey, image_uid: UID
-    ) -> list[WorkerPool]:
-        qks = QueryKeys(qks=[PoolImageIDPartitionKey.with_obj(image_uid)])
-        return self.query_all(credentials=credentials, qks=qks)
+    def get_worker_by_name(
+        self, credentials: SyftVerifyKey, worker_name: str
+    ) -> Result[SyftWorker | None, str]:
+        qks = QueryKeys(qks=[WorkerContainerNamePartitionKey.with_obj(worker_name)])
+        return self.query_one(credentials=credentials, qks=qks)
+
+    def update_consumer_state(
+        self, credentials: SyftVerifyKey, worker_uid: UID, consumer_state: ConsumerState
+    ) -> Result[str, str]:
+        res = self.get_by_uid(credentials=credentials, uid=worker_uid)
+        if res.is_err():
+            return Err(
+                f"Failed to retrieve Worker with id: {worker_uid}. Error: {res.err()}"
+            )
+        worker: SyftWorker | None = res.ok()
+        if worker is None:
+            return Err(f"Worker with id: {worker_uid} not found")
+        worker.consumer_state = consumer_state
+        update_res = self.update(credentials=credentials, obj=worker)
+        if update_res.is_err():
+            return Err(
+                f"Failed to update Worker with id: {worker_uid}. Error: {update_res.err()}"
+            )
+        return Ok(f"Successfully updated Worker with id: {worker_uid}")
```

### Comparing `syft-0.8.6b1/src/syft/service/worker/worker_service.py` & `syft-0.8.7b1/src/syft/service/worker/worker_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 from typing import cast
 
 # third party
 import docker
 from docker.models.containers import Container
 
 # relative
-from ...abstract_node import AbstractNode
 from ...custom_worker.k8s import IN_KUBERNETES
 from ...custom_worker.k8s import PodStatus
 from ...custom_worker.runner_k8s import KubernetesRunner
 from ...node.credentials import SyftVerifyKey
 from ...serde.serializable import serializable
 from ...store.document_store import DocumentStore
 from ...store.document_store import SyftSuccess
@@ -52,15 +51,15 @@
         name="start_workers",
         roles=ADMIN_ROLE_LEVEL,
     )
     def start_workers(
         self, context: AuthedServiceContext, n: int = 1
     ) -> list[ContainerSpawnStatus] | SyftError:
         """Add a Container Image."""
-        context.node = cast(AbstractNode, context.node)
+
         worker_pool_service = context.node.get_service("SyftWorkerPoolService")
         return worker_pool_service.add_workers(
             context, number=n, pool_name=DEFAULT_WORKER_POOL_NAME
         )
 
     @service_method(
         path="worker.get_all", name="get_all", roles=DATA_SCIENTIST_ROLE_LEVEL
@@ -157,15 +156,15 @@
         context: AuthedServiceContext,
         uid: UID,
         force: bool = False,
     ) -> SyftSuccess | SyftError:
         worker = self._get_worker(context=context, uid=uid)
         if isinstance(worker, SyftError):
             return worker
-        context.node = cast(AbstractNode, context.node)
+
         worker_pool_name = worker.worker_pool_name
 
         # relative
         from .worker_pool_service import SyftWorkerPoolService
 
         worker_pool_service: AbstractService = context.node.get_service(
             SyftWorkerPoolService
```

### Comparing `syft-0.8.6b1/src/syft/store/blob_storage/__init__.py` & `syft-0.8.7b1/src/syft/store/blob_storage/__init__.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6b1/src/syft/store/blob_storage/on_disk.py` & `syft-0.8.7b1/src/syft/store/blob_storage/on_disk.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6b1/src/syft/store/blob_storage/seaweedfs.py` & `syft-0.8.7b1/src/syft/types/blob_storage.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,303 +1,371 @@
 # stdlib
-from collections.abc import Generator
-from io import BytesIO
-import math
+from collections.abc import Callable
+from collections.abc import Iterator
+from datetime import datetime
+from datetime import timedelta
+import mimetypes
+from pathlib import Path
 from queue import Queue
+import sys
 import threading
+from time import sleep
 from typing import Any
+from typing import ClassVar
+from typing import TYPE_CHECKING
 
 # third party
-import boto3
-from botocore.client import BaseClient as S3BaseClient
+from azure.storage.blob import BlobSasPermissions
+from azure.storage.blob import generate_blob_sas
 from botocore.client import ClientError as BotoClientError
-from botocore.client import Config
-import requests
-from tqdm import tqdm
 from typing_extensions import Self
 
 # relative
-from . import BlobDeposit
-from . import BlobRetrieval
-from . import BlobStorageClient
-from . import BlobStorageClientConfig
-from . import BlobStorageConfig
-from . import BlobStorageConnection
-from ...serde.serializable import serializable
-from ...service.blob_storage.remote_profile import AzureRemoteProfile
-from ...service.response import SyftError
-from ...service.response import SyftSuccess
-from ...service.service import from_api_or_context
-from ...types.blob_storage import BlobStorageEntry
-from ...types.blob_storage import CreateBlobStorageEntry
-from ...types.blob_storage import SeaweedSecureFilePathLocation
-from ...types.blob_storage import SecureFilePathLocation
-from ...types.grid_url import GridURL
-from ...types.syft_object import SYFT_OBJECT_VERSION_3
-from ...util.constants import DEFAULT_TIMEOUT
-
-WRITE_EXPIRATION_TIME = 900  # seconds
-DEFAULT_FILE_PART_SIZE = (1024**3) * 5  # 5GB
-DEFAULT_UPLOAD_CHUNK_SIZE = 819200
+from ..client.api import SyftAPI
+from ..client.client import SyftClient
+from ..node.credentials import SyftVerifyKey
+from ..serde import serialize
+from ..serde.serializable import serializable
+from ..service.action.action_object import ActionObject
+from ..service.action.action_object import ActionObjectPointer
+from ..service.action.action_object import BASE_PASSTHROUGH_ATTRS
+from ..service.action.action_types import action_types
+from ..service.response import SyftError
+from ..service.response import SyftException
+from ..service.service import from_api_or_context
+from ..types.grid_url import GridURL
+from ..types.transforms import keep
+from ..types.transforms import transform
+from .datetime import DateTime
+from .syft_object import SYFT_OBJECT_VERSION_2
+from .syft_object import SYFT_OBJECT_VERSION_3
+from .syft_object import SYFT_OBJECT_VERSION_4
+from .syft_object import SyftObject
+from .uid import UID
+
+if TYPE_CHECKING:
+    # relative
+    from ..store.blob_storage import BlobRetrievalByURL
+    from ..store.blob_storage import BlobStorageConnection
 
 
-@serializable()
-class SeaweedFSBlobDeposit(BlobDeposit):
-    __canonical_name__ = "SeaweedFSBlobDeposit"
-    __version__ = SYFT_OBJECT_VERSION_3
+READ_EXPIRATION_TIME = 1800  # seconds
+DEFAULT_CHUNK_SIZE = 10000 * 1024
 
-    urls: list[GridURL]
-    size: int
 
-    def write(self, data: BytesIO) -> SyftSuccess | SyftError:
-        # relative
-        from ...client.api import APIRegistry
+@serializable()
+class BlobFile(SyftObject):
+    __canonical_name__ = "BlobFile"
+    __version__ = SYFT_OBJECT_VERSION_4
+
+    file_name: str
+    syft_blob_storage_entry_id: UID | None = None
+    file_size: int | None = None
+    path: Path | None = None
+    uploaded: bool = False
 
-        api = APIRegistry.api_for(
-            node_uid=self.syft_node_location,
-            user_verify_key=self.syft_client_verify_key,
+    __repr_attrs__ = ["id", "file_name"]
+
+    def read(
+        self,
+        stream: bool = False,
+        chunk_size: int = DEFAULT_CHUNK_SIZE,
+        force: bool = False,
+    ) -> Any:
+        # get blob retrieval object from api + syft_blob_storage_entry_id
+        read_method = from_api_or_context(
+            "blob_storage.read", self.syft_node_location, self.syft_client_verify_key
         )
+        if read_method is not None:
+            blob_retrieval_object = read_method(self.syft_blob_storage_entry_id)
+            return blob_retrieval_object._read_data(
+                stream=stream, chunk_size=chunk_size, _deserialize=False
+            )
+        else:
+            return None
 
-        etags = []
+    @classmethod
+    def upload_from_path(cls, path: str | Path, client: SyftClient) -> Any:
+        # syft absolute
+        import syft as sy
+
+        return sy.ActionObject.from_path(path=path).send(client).syft_action_data
+
+    def _upload_to_blobstorage_from_api(self, api: SyftAPI) -> SyftError | None:
+        if self.path is None:
+            raise ValueError("cannot upload BlobFile, no path specified")
+        storage_entry = CreateBlobStorageEntry.from_path(self.path)
+
+        blob_deposit_object = api.services.blob_storage.allocate(storage_entry)
+
+        if isinstance(blob_deposit_object, SyftError):
+            return blob_deposit_object
+
+        with open(self.path, "rb") as f:
+            result = blob_deposit_object.write(f)
+
+        if isinstance(result, SyftError):
+            return result
+
+        self.syft_blob_storage_entry_id = blob_deposit_object.blob_storage_entry_id
+        self.uploaded = True
+
+        return None
+
+    def upload_to_blobstorage(self, client: SyftClient) -> SyftError | None:
+        self.syft_node_location = client.id
+        self.syft_client_verify_key = client.verify_key
+        return self._upload_to_blobstorage_from_api(client.api)
+
+    def _iter_lines(self, chunk_size: int = DEFAULT_CHUNK_SIZE) -> Iterator[bytes]:
+        """Synchronous version of the async iter_lines. This implementation
+        is also optimized in terms of splitting chunks, making it faster for
+        larger lines"""
+        pending = None
+        for chunk in self.read(stream=True, chunk_size=chunk_size):
+            if b"\n" in chunk:
+                if pending is not None:
+                    chunk = pending + chunk  # type: ignore[unreachable]
+                lines = chunk.splitlines()
+                if lines and lines[-1] and chunk and lines[-1][-1] == chunk[-1]:
+                    pending = lines.pop()
+                else:
+                    pending = None
+                yield from lines
+            else:
+                if pending is None:
+                    pending = chunk
+                else:
+                    pending = pending + chunk
 
-        try:
-            no_lines = 0
-            # this loops over the parts, we have multiple parts to allow for
-            # concurrent uploads of a single file. (We are currently not using that)
-            # a part may for instance be 5GB
-            # parts are then splitted into chunks which are MBs (order of magnitude)
-            part_size = math.ceil(self.size / len(self.urls))
-            chunk_size = DEFAULT_UPLOAD_CHUNK_SIZE
-
-            # this is the total nr of chunks in all parts
-            total_iterations = math.ceil(part_size / chunk_size) * len(self.urls)
-
-            with tqdm(
-                total=total_iterations,
-                desc=f"Uploading progress",  # noqa
-            ) as pbar:
-                for part_no, url in enumerate(
-                    self.urls,
-                    start=1,
-                ):
-                    if api is not None and api.connection is not None:
-                        blob_url = api.connection.to_blob_route(
-                            url.url_path, host=url.host_or_ip
-                        )
-                    else:
-                        blob_url = url
-
-                    # read a chunk untill we have read part_size
-                    class PartGenerator:
-                        def __init__(self) -> None:
-                            self.no_lines = 0
-
-                        def async_generator(
-                            self, chunk_size: int = DEFAULT_UPLOAD_CHUNK_SIZE
-                        ) -> Generator:
-                            item_queue: Queue = Queue()
-                            threading.Thread(
-                                target=self.add_chunks_to_queue,
-                                kwargs={"queue": item_queue, "chunk_size": chunk_size},
-                                daemon=True,
-                            ).start()
-                            item = item_queue.get()
-                            while item != 0:
-                                yield item
-                                pbar.update(1)
-                                item = item_queue.get()
-
-                        def add_chunks_to_queue(
-                            self,
-                            queue: Queue,
-                            chunk_size: int = DEFAULT_UPLOAD_CHUNK_SIZE,
-                        ) -> None:
-                            """Creates a data geneator for the part"""
-                            n = 0
-
-                            while n * chunk_size <= part_size:
-                                try:
-                                    chunk = data.read(chunk_size)
-                                    self.no_lines += chunk.count(b"\n")
-                                    n += 1
-                                    queue.put(chunk)
-                                except BlockingIOError:
-                                    # if end of file, stop
-                                    queue.put(0)
-                            # if end of part, stop
-                            queue.put(0)
-
-                    gen = PartGenerator()
-
-                    response = requests.put(
-                        url=str(blob_url),
-                        data=gen.async_generator(chunk_size),
-                        timeout=DEFAULT_TIMEOUT,
-                        stream=True,
-                    )
-
-                    response.raise_for_status()
-                    no_lines += gen.no_lines
-                    etag = response.headers["ETag"]
-                    etags.append({"ETag": etag, "PartNumber": part_no})
-
-        except requests.RequestException as e:
-            print(e)
-            return SyftError(message=str(e))
-
-        mark_write_complete_method = from_api_or_context(
-            func_or_path="blob_storage.mark_write_complete",
-            syft_node_location=self.syft_node_location,
-            syft_client_verify_key=self.syft_client_verify_key,
-        )
-        if mark_write_complete_method is None:
-            return SyftError(message="mark_write_complete_method is None")
-        return mark_write_complete_method(
-            etags=etags, uid=self.blob_storage_entry_id, no_lines=no_lines
-        )
+        if pending is not None:
+            yield pending
 
+    def read_queue(
+        self,
+        queue: Queue,
+        chunk_size: int,
+        progress: bool = False,
+        buffer_lines: int = 10000,
+    ) -> None:
+        total_read = 0
+        for _i, line in enumerate(self._iter_lines(chunk_size=chunk_size)):
+            line_size = len(line) + 1  # add byte for \n
+            if self.file_size is not None:
+                total_read = min(self.file_size, total_read + line_size)
+            else:
+                # naive way of doing this, max be 1 byte off because the last
+                # byte can also be a \n
+                total_read += line_size
+            if progress:
+                queue.put((total_read, line))
+            else:
+                queue.put(line)
+            while queue.qsize() > buffer_lines:
+                sleep(0.1)
+        # Put anything not a string at the end
+        queue.put(0)
+
+    def iter_lines(
+        self, chunk_size: int = DEFAULT_CHUNK_SIZE, progress: bool = False
+    ) -> Iterator[str]:
+        item_queue: Queue = Queue()
+        threading.Thread(
+            target=self.read_queue,
+            args=(item_queue, chunk_size, progress),
+            daemon=True,
+        ).start()
+        item = item_queue.get()
+        while item != 0:
+            yield item
+            item = item_queue.get()
+
+    def _coll_repr_(self) -> dict[str, str]:
+        return {"file_name": self.file_name}
 
-@serializable()
-class SeaweedFSClientConfig(BlobStorageClientConfig):
-    host: str
-    port: int
-    mount_port: int | None = None
-    access_key: str
-    secret_key: str
-    region: str
-    default_bucket_name: str = "defaultbucket"
-    remote_profiles: dict[str, AzureRemoteProfile] = {}
 
-    @property
-    def endpoint_url(self) -> str:
-        grid_url = GridURL(host_or_ip=self.host, port=self.port)
-        return grid_url.url
+class BlobFileType(type):
+    pass
 
-    @property
-    def mount_url(self) -> str:
-        if self.mount_port is None:
-            raise ValueError("Seaweed should be configured with a mount port to mount")
-        return f"http://{self.host}:{self.mount_port}/configure_azure"
 
+class BlobFileObjectPointer(ActionObjectPointer):
+    pass
 
-@serializable()
-class SeaweedFSClient(BlobStorageClient):
-    config: SeaweedFSClientConfig
 
-    def connect(self) -> BlobStorageConnection:
-        return SeaweedFSConnection(
-            client=boto3.client(
-                "s3",
-                endpoint_url=self.config.endpoint_url,
-                aws_access_key_id=self.config.access_key,
-                aws_secret_access_key=self.config.secret_key,
-                config=Config(signature_version="s3v4"),
-                region_name=self.config.region,
-            ),
-            default_bucket_name=self.config.default_bucket_name,
-            config=self.config,
-        )
+@serializable()
+class BlobFileObject(ActionObject):
+    __canonical_name__ = "BlobFileOBject"
+    __version__ = SYFT_OBJECT_VERSION_2
+
+    syft_internal_type: ClassVar[type[Any]] = BlobFile
+    syft_pointer_type: ClassVar[type[ActionObjectPointer]] = BlobFileObjectPointer
+    syft_passthrough_attrs: list[str] = BASE_PASSTHROUGH_ATTRS
 
 
 @serializable()
-class SeaweedFSConnection(BlobStorageConnection):
-    client: S3BaseClient
-    default_bucket_name: str
-    config: SeaweedFSClientConfig
+class SecureFilePathLocation(SyftObject):
+    __canonical_name__ = "SecureFilePathLocation"
+    __version__ = SYFT_OBJECT_VERSION_2
+
+    id: UID
+    path: str
 
-    def __init__(
+    def __repr__(self) -> str:
+        return f"{self.path}"
+
+    def generate_url(
         self,
-        client: S3BaseClient,
-        default_bucket_name: str,
-        config: SeaweedFSClientConfig,
-    ):
-        self.client = client
-        self.default_bucket_name = default_bucket_name
-        self.config = config
+        connection: "BlobStorageConnection",
+        type_: type | None,
+        bucket_name: str | None,
+        *args: Any,
+    ) -> "BlobRetrievalByURL":
+        raise NotImplementedError
 
-    def __enter__(self) -> Self:
-        return self
 
-    def __exit__(self, *exc: Any) -> None:
-        self.client.close()
+@serializable()
+class SeaweedSecureFilePathLocation(SecureFilePathLocation):
+    __canonical_name__ = "SeaweedSecureFilePathLocation"
+    __version__ = SYFT_OBJECT_VERSION_3
 
-    def read(
+    upload_id: str | None = None
+
+    def generate_url(
         self,
-        fp: SecureFilePathLocation,
+        connection: "BlobStorageConnection",
         type_: type | None,
-        bucket_name: str | None = None,
-    ) -> BlobRetrieval:
-        if bucket_name is None:
-            bucket_name = self.default_bucket_name
-        # this will generate the url, the SecureFilePathLocation also handles the logic
-        # that decides whether to use a direct connection to azure/aws/gcp or via seaweed
-        return fp.generate_url(self, type_, bucket_name)
-
-    def allocate(
-        self, obj: CreateBlobStorageEntry
-    ) -> SecureFilePathLocation | SyftError:
+        bucket_name: str | None,
+        *args: Any,
+    ) -> "BlobRetrievalByURL":
         try:
-            file_name = obj.file_name
-            result = self.client.create_multipart_upload(
-                Bucket=self.default_bucket_name,
-                Key=file_name,
-            )
-            upload_id = result["UploadId"]
-            return SeaweedSecureFilePathLocation(upload_id=upload_id, path=file_name)
-        except BotoClientError as e:
-            return SyftError(
-                message=f"Failed to allocate space for {obj} with error: {e}"
+            url = connection.client.generate_presigned_url(
+                ClientMethod="get_object",
+                Params={"Bucket": bucket_name, "Key": self.path},
+                ExpiresIn=READ_EXPIRATION_TIME,
             )
 
-    def write(self, obj: BlobStorageEntry) -> BlobDeposit:
-        total_parts = math.ceil(obj.file_size / DEFAULT_FILE_PART_SIZE)
+            # relative
+            from ..store.blob_storage import BlobRetrievalByURL
 
-        urls = [
-            GridURL.from_url(
-                self.client.generate_presigned_url(
-                    ClientMethod="upload_part",
-                    Params={
-                        "Bucket": self.default_bucket_name,
-                        "Key": obj.location.path,
-                        "UploadId": obj.location.upload_id,
-                        "PartNumber": i + 1,
-                    },
-                    ExpiresIn=WRITE_EXPIRATION_TIME,
-                )
+            return BlobRetrievalByURL(
+                url=GridURL.from_url(url), file_name=Path(self.path).name, type_=type_
             )
-            for i in range(total_parts)
-        ]
-        return SeaweedFSBlobDeposit(
-            blob_storage_entry_id=obj.id, urls=urls, size=obj.file_size
+        except BotoClientError as e:
+            raise SyftException(e)
+
+
+@serializable()
+class AzureSecureFilePathLocation(SecureFilePathLocation):
+    __canonical_name__ = "AzureSecureFilePathLocation"
+    __version__ = SYFT_OBJECT_VERSION_2
+
+    # upload_id: str
+    azure_profile_name: str  # Used by Seaweedfs to refer to a remote config
+    bucket_name: str
+
+    def generate_url(
+        self, connection: "BlobStorageConnection", type_: type | None, *args: Any
+    ) -> "BlobRetrievalByURL":
+        # SAS is almost the same thing as the presigned url
+        config = connection.config.remote_profiles[self.azure_profile_name]
+        account_name = config.account_name
+        container_name = config.container_name
+        blob_name = self.path
+        sas_blob = generate_blob_sas(
+            account_name=account_name,
+            container_name=container_name,
+            blob_name=blob_name,
+            account_key=config.account_key,
+            permission=BlobSasPermissions(read=True),
+            expiry=datetime.utcnow() + timedelta(hours=48),
         )
+        url = f"https://{config.account_name}.blob.core.windows.net/{container_name}/{blob_name}?{sas_blob}"
 
-    def complete_multipart_upload(
-        self,
-        blob_entry: BlobStorageEntry,
-        etags: list,
-    ) -> SyftError | SyftSuccess:
-        try:
-            self.client.complete_multipart_upload(
-                Bucket=self.default_bucket_name,
-                Key=blob_entry.location.path,
-                MultipartUpload={"Parts": etags},
-                UploadId=blob_entry.location.upload_id,
-            )
-            return SyftSuccess(message="Successfully saved file.")
-        except BotoClientError as e:
-            return SyftError(message=str(e))
+        # relative
+        from ..store.blob_storage import BlobRetrievalByURL
 
-    def delete(
-        self,
-        fp: SecureFilePathLocation,
-    ) -> SyftSuccess | SyftError:
-        try:
-            self.client.delete_object(Bucket=self.default_bucket_name, Key=fp.path)
-            return SyftSuccess(message="Successfully deleted file.")
-        except BotoClientError as e:
-            return SyftError(message=str(e))
+        return BlobRetrievalByURL(url=url, file_name=Path(self.path).name, type_=type_)
+
+
+@serializable()
+class BlobStorageEntry(SyftObject):
+    __canonical_name__ = "BlobStorageEntry"
+    __version__ = SYFT_OBJECT_VERSION_3
+
+    id: UID
+    location: SecureFilePathLocation | SeaweedSecureFilePathLocation
+    type_: type | None = None
+    mimetype: str = "bytes"
+    file_size: int
+    no_lines: int | None = 0
+    uploaded_by: SyftVerifyKey
+    created_at: DateTime = DateTime.now()
+    bucket_name: str | None = None
+
+    __attr_searchable__ = ["bucket_name"]
+
+
+@serializable()
+class BlobStorageMetadata(SyftObject):
+    __canonical_name__ = "BlobStorageMetadata"
+    __version__ = SYFT_OBJECT_VERSION_3
+
+    type_: type[SyftObject] | None = None
+    mimetype: str = "bytes"
+    file_size: int
+    no_lines: int | None = 0
 
 
 @serializable()
-class SeaweedFSConfig(BlobStorageConfig):
-    client_type: type[BlobStorageClient] = SeaweedFSClient
-    client_config: SeaweedFSClientConfig
+class CreateBlobStorageEntry(SyftObject):
+    __canonical_name__ = "CreateBlobStorageEntry"
+    __version__ = SYFT_OBJECT_VERSION_2
+
+    id: UID
+    type_: type | None = None
+    mimetype: str = "bytes"
+    file_size: int
+    extensions: list[str] = []
+
+    @classmethod
+    def from_obj(cls, obj: SyftObject) -> Self:
+        file_size = sys.getsizeof(serialize._serialize(obj=obj, to_bytes=True))
+        return cls(file_size=file_size, type_=type(obj))
+
+    @classmethod
+    def from_path(cls, fp: str | Path, mimetype: str | None = None) -> Self:
+        path = Path(fp)
+        if not path.exists():
+            raise SyftException(f"{fp} does not exist.")
+        if not path.is_file():
+            raise SyftException(f"{fp} is not a file.")
+
+        if path.suffix.lower() == ".jsonl":
+            mimetype = "application/json-lines"
+        if mimetype is None:
+            mime_types = mimetypes.guess_type(fp)
+            if len(mime_types) > 0 and mime_types[0] is not None:
+                mimetype = mime_types[0]
+            else:
+                raise SyftException(
+                    "mimetype could not be identified.\n"
+                    "Please specify mimetype manually `from_path(..., mimetype = ...)`."
+                )
+
+        return cls(
+            mimetype=mimetype,
+            file_size=path.stat().st_size,
+            extensions=path.suffixes,
+            type_=BlobFileType,
+        )
+
+    @property
+    def file_name(self) -> str:
+        return str(self.id) + "".join(self.extensions)
+
+
+@transform(BlobStorageEntry, BlobStorageMetadata)
+def storage_entry_to_metadata() -> list[Callable]:
+    return [keep(["id", "type_", "mimetype", "file_size"])]
+
+
+action_types[BlobFile] = BlobFileObject
```

### Comparing `syft-0.8.6b1/src/syft/store/dict_document_store.py` & `syft-0.8.7b1/src/syft/store/dict_document_store.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6b1/src/syft/store/document_store.py` & `syft-0.8.7b1/src/syft/store/kv_document_store.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,787 +1,682 @@
 # future
 from __future__ import annotations
 
 # stdlib
-from collections.abc import Callable
-import types
-import typing
+from collections import defaultdict
+from enum import Enum
 from typing import Any
 
 # third party
-from pydantic import BaseModel
-from pydantic import Field
 from result import Err
 from result import Ok
 from result import Result
-from typeguard import check_type
+from typing_extensions import Self
 
 # relative
-from ..node.credentials import SyftSigningKey
 from ..node.credentials import SyftVerifyKey
 from ..serde.serializable import serializable
+from ..service.action.action_permissions import ActionObjectEXECUTE
+from ..service.action.action_permissions import ActionObjectOWNER
 from ..service.action.action_permissions import ActionObjectPermission
+from ..service.action.action_permissions import ActionObjectREAD
+from ..service.action.action_permissions import ActionObjectWRITE
+from ..service.action.action_permissions import ActionPermission
+from ..service.action.action_permissions import StoragePermission
 from ..service.context import AuthedServiceContext
 from ..service.response import SyftSuccess
-from ..types.base import SyftBaseModel
-from ..types.syft_object import SYFT_OBJECT_VERSION_2
-from ..types.syft_object import SyftBaseObject
 from ..types.syft_object import SyftObject
 from ..types.uid import UID
-from ..util.telemetry import instrument
-from .locks import LockingConfig
-from .locks import NoLockingConfig
-from .locks import SyftLock
+from .document_store import BaseStash
+from .document_store import PartitionKey
+from .document_store import QueryKey
+from .document_store import QueryKeys
+from .document_store import StorePartition
 
 
 @serializable()
-class BasePartitionSettings(SyftBaseModel):
-    """Basic Partition Settings
+class UniqueKeyCheck(Enum):
+    EMPTY = 0
+    MATCHES = 1
+    ERROR = 2
 
-    Parameters:
-        name: str
-            Identifier to be used as prefix by stores and for partitioning
-    """
-
-    name: str
-
-
-def first_or_none(result: Any) -> Ok:
-    if hasattr(result, "__len__") and len(result) > 0:
-        return Ok(result[0])
-    return Ok(None)
-
-
-def is_generic_alias(t: type) -> bool:
-    return isinstance(t, types.GenericAlias | typing._GenericAlias)
-
-
-class StoreClientConfig(BaseModel):
-    """Base Client specific configuration"""
-
-    pass
-
-
-@serializable()
-class PartitionKey(BaseModel):
-    key: str
-    type_: type | object
-
-    def __eq__(self, other: Any) -> bool:
-        return (
-            type(other) == type(self)
-            and self.key == other.key
-            and self.type_ == other.type_
-        )
-
-    def with_obj(self, obj: Any) -> QueryKey:
-        return QueryKey.from_obj(partition_key=self, obj=obj)
-
-    def extract_list(self, obj: Any) -> list:
-        # not a list and matches the internal list type of the _GenericAlias
-        if not isinstance(obj, list):
-            if not isinstance(obj, typing.get_args(self.type_)):
-                obj = getattr(obj, self.key)
-                if isinstance(obj, types.FunctionType | types.MethodType):
-                    obj = obj()
-
-            if not isinstance(obj, list) and isinstance(
-                obj, typing.get_args(self.type_)
-            ):
-                # still not a list but the right type
-                obj = [obj]
 
-        # is a list type so lets compare directly
-        check_type(obj, self.type_)
-        return obj
-
-    @property
-    def type_list(self) -> bool:
-        return is_generic_alias(self.type_) and self.type_.__origin__ == list
-
-
-@serializable()
-class PartitionKeys(BaseModel):
-    pks: PartitionKey | tuple[PartitionKey, ...] | list[PartitionKey]
-
-    @property
-    def all(self) -> tuple[PartitionKey, ...] | list[PartitionKey]:
-        # make sure we always return a list even if there's a single value
-        return self.pks if isinstance(self.pks, tuple | list) else [self.pks]
-
-    def with_obj(self, obj: Any) -> QueryKeys:
-        return QueryKeys.from_obj(partition_keys=self, obj=obj)
-
-    def with_tuple(self, *args: Any) -> QueryKeys:
-        return QueryKeys.from_tuple(partition_keys=self, args=args)
-
-    def add(self, pk: PartitionKey) -> PartitionKeys:
-        return PartitionKeys(pks=list(self.all) + [pk])
-
-    @staticmethod
-    def from_dict(cks_dict: dict[str, type]) -> PartitionKeys:
-        pks = []
-        for k, t in cks_dict.items():
-            pks.append(PartitionKey(key=k, type_=t))
-        return PartitionKeys(pks=pks)
+class KeyValueBackingStore:
+    """Key-Value store core logic."""
 
+    def __setitem__(self, key: Any, value: Any) -> None:
+        raise NotImplementedError
 
-@serializable()
-class QueryKey(PartitionKey):
-    value: Any = None
+    def __getitem__(self, key: Any) -> Self:
+        raise NotImplementedError
 
-    def __eq__(self, other: Any) -> bool:
-        return (
-            type(other) == type(self)
-            and self.key == other.key
-            and self.type_ == other.type_
-            and self.value == other.value
-        )
+    def __repr__(self) -> str:
+        raise NotImplementedError
 
-    @property
-    def partition_key(self) -> PartitionKey:
-        return PartitionKey(key=self.key, type_=self.type_)
-
-    @staticmethod
-    def from_obj(partition_key: PartitionKey, obj: Any) -> QueryKey:
-        pk_key = partition_key.key
-        pk_type = partition_key.type_
-
-        # 🟡 TODO: support more advanced types than List[type]
-        if partition_key.type_list:
-            pk_value = partition_key.extract_list(obj)
-        else:
-            if isinstance(obj, pk_type):
-                pk_value = obj
-            else:
-                pk_value = getattr(obj, pk_key)
-                # object has a method for getting these types
-                # we can't use properties because we don't seem to be able to get the
-                # return types
-                # TODO: fix the mypy issue
-                if isinstance(pk_value, types.FunctionType | types.MethodType):  # type: ignore[unreachable]
-                    pk_value = pk_value()  # type: ignore[unreachable]
+    def __len__(self) -> int:
+        raise NotImplementedError
 
-            if pk_value and not isinstance(pk_value, pk_type):
-                raise Exception(
-                    f"PartitionKey {pk_value} of type {type(pk_value)} must be {pk_type}."
-                )
-        return QueryKey(key=pk_key, type_=pk_type, value=pk_value)
+    def __delitem__(self, key: str) -> None:
+        raise NotImplementedError
 
-    @property
-    def as_dict(self) -> dict[str, Any]:
-        return {self.key: self.value}
-
-    @property
-    def as_dict_mongo(self) -> dict[str, Any]:
-        key = self.key
-        if key == "id":
-            key = "_id"
-        if self.type_list:
-            # We want to search inside the list of values
-            return {key: {"$in": self.value}}
-        return {key: self.value}
+    def clear(self) -> None:
+        raise NotImplementedError
 
+    def copy(self) -> Self:
+        raise NotImplementedError
 
-@serializable()
-class PartitionKeysWithUID(PartitionKeys):
-    uid_pk: PartitionKey
+    def update(self, *args: Any, **kwargs: Any) -> None:
+        raise NotImplementedError
 
-    @property
-    def all(self) -> tuple[PartitionKey, ...] | list[PartitionKey]:
-        all_keys = list(self.pks) if isinstance(self.pks, tuple | list) else [self.pks]
-        if self.uid_pk not in all_keys:
-            all_keys.insert(0, self.uid_pk)
-        return all_keys
+    def keys(self) -> Any:
+        raise NotImplementedError
 
+    def values(self) -> Any:
+        raise NotImplementedError
 
-@serializable()
-class QueryKeys(SyftBaseModel):
-    qks: QueryKey | tuple[QueryKey, ...] | list[QueryKey]
+    def items(self) -> Any:
+        raise NotImplementedError
 
-    @property
-    def all(self) -> tuple[QueryKey, ...] | list[QueryKey]:
-        # make sure we always return a list even if there's a single value
-        return self.qks if isinstance(self.qks, tuple | list) else [self.qks]
-
-    @staticmethod
-    def from_obj(partition_keys: PartitionKeys, obj: SyftObject) -> QueryKeys:
-        qks = []
-        for partition_key in partition_keys.all:
-            pk_key = partition_key.key
-            pk_type = partition_key.type_
-            pk_value = getattr(obj, pk_key)
-            # object has a method for getting these types
-            # we can't use properties because we don't seem to be able to get the
-            # return types
-            if isinstance(pk_value, types.FunctionType | types.MethodType):
-                pk_value = pk_value()
-            if partition_key.type_list:
-                pk_value = partition_key.extract_list(obj)
-            else:
-                if pk_value and not isinstance(pk_value, pk_type):
-                    raise Exception(
-                        f"PartitionKey {pk_value} of type {type(pk_value)} must be {pk_type}."
-                    )
-            qk = QueryKey(key=pk_key, type_=pk_type, value=pk_value)
-            qks.append(qk)
-        return QueryKeys(qks=qks)
-
-    @staticmethod
-    def from_tuple(partition_keys: PartitionKeys, args: tuple) -> QueryKeys:
-        qks = []
-        for partition_key, pk_value in zip(partition_keys.all, args):
-            pk_key = partition_key.key
-            pk_type = partition_key.type_
-            if not isinstance(pk_value, pk_type):
-                raise Exception(
-                    f"PartitionKey {pk_value} of type {type(pk_value)} must be {pk_type}."
-                )
-            qk = QueryKey(key=pk_key, type_=pk_type, value=pk_value)
-            qks.append(qk)
-        return QueryKeys(qks=qks)
-
-    @staticmethod
-    def from_dict(qks_dict: dict[str, Any]) -> QueryKeys:
-        qks = []
-        for k, v in qks_dict.items():
-            qks.append(QueryKey(key=k, type_=type(v), value=v))
-        return QueryKeys(qks=qks)
-
-    @property
-    def as_dict(self) -> dict:
-        qk_dict = {}
-        for qk in self.all:
-            qk_key = qk.key
-            qk_value = qk.value
-            qk_dict[qk_key] = qk_value
-        return qk_dict
-
-    @property
-    def as_dict_mongo(self) -> dict:
-        qk_dict = {}
-        for qk in self.all:
-            qk_key = qk.key
-            qk_value = qk.value
-            if qk_key == "id":
-                qk_key = "_id"
-            if qk.type_list:
-                # We want to search inside the list of values
-                qk_dict[qk_key] = {"$in": qk_value}
-            else:
-                qk_dict[qk_key] = qk_value
-        return qk_dict
+    def pop(self, *args: Any) -> Self:
+        raise NotImplementedError
 
+    def __contains__(self, item: Any) -> bool:
+        raise NotImplementedError
 
-UIDPartitionKey = PartitionKey(key="id", type_=UID)
+    def __iter__(self) -> Any:
+        raise NotImplementedError
 
 
-@serializable()
-class PartitionSettings(BasePartitionSettings):
-    object_type: type
-    store_key: PartitionKey = UIDPartitionKey
-
-    @property
-    def unique_keys(self) -> PartitionKeys:
-        unique_keys = PartitionKeys.from_dict(self.object_type._syft_unique_keys_dict())
-        return unique_keys.add(self.store_key)
-
-    @property
-    def searchable_keys(self) -> PartitionKeys:
-        return PartitionKeys.from_dict(self.object_type._syft_searchable_keys_dict())
-
-
-@instrument
-@serializable(attrs=["settings", "store_config", "unique_cks", "searchable_cks"])
-class StorePartition:
-    """Base StorePartition
+class KeyValueStorePartition(StorePartition):
+    """Key-Value StorePartition
 
     Parameters:
-        settings: PartitionSettings
+        `settings`: PartitionSettings
             PySyft specific settings
-        store_config: StoreConfig
+        `store_config`: StoreConfig
             Backend specific configuration
     """
 
-    def __init__(
-        self,
-        node_uid: UID,
-        root_verify_key: SyftVerifyKey | None,
-        settings: PartitionSettings,
-        store_config: StoreConfig,
-    ) -> None:
-        if root_verify_key is None:
-            root_verify_key = SyftSigningKey.generate().verify_key
-        self.node_uid = node_uid
-        self.root_verify_key = root_verify_key
-        self.settings = settings
-        self.store_config = store_config
-        self.init_store()
-
-        store_config.locking_config.lock_name = f"StorePartition-{settings.name}"
-        self.lock = SyftLock(store_config.locking_config)
-
     def init_store(self) -> Result[Ok, Err]:
-        try:
-            self.unique_cks = self.settings.unique_keys.all
-            self.searchable_cks = self.settings.searchable_keys.all
-        except BaseException as e:
-            return Err(str(e))
+        store_status = super().init_store()
+        if store_status.is_err():
+            return store_status
 
-        return Ok(True)
-
-    def matches_unique_cks(self, partition_key: PartitionKey) -> bool:
-        return partition_key in self.unique_cks
-
-    def matches_searchable_cks(self, partition_key: PartitionKey) -> bool:
-        return partition_key in self.searchable_cks
-
-    def store_query_key(self, obj: Any) -> QueryKey:
-        return self.settings.store_key.with_obj(obj)
+        try:
+            self.data = self.store_config.backing_store(
+                "data", self.settings, self.store_config
+            )
+            self.unique_keys = self.store_config.backing_store(
+                "unique_keys", self.settings, self.store_config
+            )
+            self.searchable_keys = self.store_config.backing_store(
+                "searchable_keys", self.settings, self.store_config
+            )
+            # uid -> set['<uid>_permission']
+            self.permissions: dict[UID, set[str]] = self.store_config.backing_store(
+                "permissions", self.settings, self.store_config, ddtype=set
+            )
 
-    def store_query_keys(self, objs: Any) -> QueryKeys:
-        return QueryKeys(qks=[self.store_query_key(obj) for obj in objs])
-
-    # Thread-safe methods
-    def _thread_safe_cbk(self, cbk: Callable, *args: Any, **kwargs: Any) -> Any | Err:
-        locked = self.lock.acquire(blocking=True)
-        if not locked:
-            print("FAILED TO LOCK")
-            return Err(
-                f"Failed to acquire lock for the operation {self.lock.lock_name} ({self.lock._lock})"
+            # uid -> set['<node_uid>']
+            self.storage_permissions: dict[UID, set[UID]] = (
+                self.store_config.backing_store(
+                    "storage_permissions",
+                    self.settings,
+                    self.store_config,
+                    ddtype=set,
+                )
             )
 
-        try:
-            result = cbk(*args, **kwargs)
+            for partition_key in self.unique_cks:
+                pk_key = partition_key.key
+                if pk_key not in self.unique_keys:
+                    self.unique_keys[pk_key] = {}
+
+            for partition_key in self.searchable_cks:
+                pk_key = partition_key.key
+                if pk_key not in self.searchable_keys:
+                    self.searchable_keys[pk_key] = defaultdict(list)
         except BaseException as e:
-            result = Err(str(e))
-        self.lock.release()
+            return Err(str(e))
 
-        return result
+        return Ok(True)
 
-    def set(
-        self,
-        credentials: SyftVerifyKey,
-        obj: SyftObject,
-        add_permissions: list[ActionObjectPermission] | None = None,
-        add_storage_permission: bool = True,
-        ignore_duplicates: bool = False,
-    ) -> Result[SyftObject, str]:
-        return self._thread_safe_cbk(
-            self._set,
-            credentials=credentials,
-            obj=obj,
-            add_permissions=add_permissions,
-            add_storage_permission=add_storage_permission,
-            ignore_duplicates=ignore_duplicates,
-        )
+    def __len__(self) -> int:
+        return len(self.data)
 
-    def get(
+    def _get(
         self,
-        credentials: SyftVerifyKey,
         uid: UID,
-    ) -> Result[SyftObject, str]:
-        return self._thread_safe_cbk(
-            self._get,
-            uid=uid,
-            credentials=credentials,
-        )
-
-    def find_index_or_search_keys(
-        self,
-        credentials: SyftVerifyKey,
-        index_qks: QueryKeys,
-        search_qks: QueryKeys,
-        order_by: PartitionKey | None = None,
-    ) -> Result[list[SyftObject], str]:
-        return self._thread_safe_cbk(
-            self._find_index_or_search_keys,
-            credentials,
-            index_qks=index_qks,
-            search_qks=search_qks,
-            order_by=order_by,
-        )
-
-    def remove_keys(
-        self,
-        unique_query_keys: QueryKeys,
-        searchable_query_keys: QueryKeys,
-    ) -> None:
-        self._thread_safe_cbk(
-            self._remove_keys,
-            unique_query_keys=unique_query_keys,
-            searchable_query_keys=searchable_query_keys,
-        )
-
-    def update(
-        self,
         credentials: SyftVerifyKey,
-        qk: QueryKey,
-        obj: SyftObject,
-        has_permission: bool = False,
+        has_permission: bool | None = False,
     ) -> Result[SyftObject, str]:
-        return self._thread_safe_cbk(
-            self._update,
-            credentials=credentials,
-            qk=qk,
-            obj=obj,
-            has_permission=has_permission,
-        )
+        # relative
+        from ..service.action.action_store import ActionObjectREAD
 
-    def get_all_from_store(
-        self,
-        credentials: SyftVerifyKey,
-        qks: QueryKeys,
-        order_by: PartitionKey | None = None,
-    ) -> Result[list[SyftObject], str]:
-        return self._thread_safe_cbk(
-            self._get_all_from_store, credentials, qks, order_by
-        )
-
-    def delete(
-        self, credentials: SyftVerifyKey, qk: QueryKey, has_permission: bool = False
-    ) -> Result[SyftSuccess, Err]:
-        return self._thread_safe_cbk(
-            self._delete, credentials, qk, has_permission=has_permission
-        )
-
-    def all(
-        self,
-        credentials: SyftVerifyKey,
-        order_by: PartitionKey | None = None,
-        has_permission: bool | None = False,
-    ) -> Result[list[BaseStash.object_type], str]:
-        return self._thread_safe_cbk(self._all, credentials, order_by, has_permission)
+        # if you get something you need READ permission
+        read_permission = ActionObjectREAD(uid=uid, credentials=credentials)
 
-    def migrate_data(
-        self,
-        to_klass: SyftObject,
-        context: AuthedServiceContext,
-        has_permission: bool | None = False,
-    ) -> Result[bool, str]:
-        return self._thread_safe_cbk(
-            self._migrate_data, to_klass, context, has_permission
-        )
+        if self.has_permission(read_permission) or has_permission:
+            syft_object = self.data[uid]
+            return Ok(syft_object)
+        return Err(f"Permission: {read_permission} denied")
 
     # Potentially thread-unsafe methods.
     # CAUTION:
     #       * Don't use self.lock here.
     #       * Do not call the public thread-safe methods here(with locking).
     # These methods are called from the public thread-safe API, and will hang the process.
+
     def _set(
         self,
         credentials: SyftVerifyKey,
         obj: SyftObject,
         add_permissions: list[ActionObjectPermission] | None = None,
         add_storage_permission: bool = True,
         ignore_duplicates: bool = False,
     ) -> Result[SyftObject, str]:
-        raise NotImplementedError
+        try:
+            # if obj.id is None:
+            # obj.id = UID()
+            store_query_key: QueryKey = self.settings.store_key.with_obj(obj)
+            uid = store_query_key.value
+            write_permission = ActionObjectWRITE(uid=uid, credentials=credentials)
+            can_write = self.has_permission(write_permission)
+            unique_query_keys: QueryKeys = self.settings.unique_keys.with_obj(obj)
+            store_key_exists = store_query_key.value in self.data
+            searchable_query_keys = self.settings.searchable_keys.with_obj(obj)
 
-    def _update(
-        self,
-        credentials: SyftVerifyKey,
-        qk: QueryKey,
-        obj: SyftObject,
-        has_permission: bool = False,
-        overwrite: bool = False,
-    ) -> Result[SyftObject, str]:
-        raise NotImplementedError
+            ck_check = self._check_partition_keys_unique(
+                unique_query_keys=unique_query_keys
+            )
 
-    def _get_all_from_store(
-        self,
-        credentials: SyftVerifyKey,
-        qks: QueryKeys,
-        order_by: PartitionKey | None = None,
-    ) -> Result[list[SyftObject], str]:
-        raise NotImplementedError
+            if not store_key_exists and ck_check == UniqueKeyCheck.EMPTY:
+                # attempt to claim it for writing
+                ownership_result = self.take_ownership(uid=uid, credentials=credentials)
+                can_write = ownership_result.is_ok()
+            elif not ignore_duplicates:
+                keys = ", ".join(f"`{key.key}`" for key in unique_query_keys.all)
+                return Err(
+                    f"Duplication Key Error for {obj}.\n"
+                    f"The fields that should be unique are {keys}."
+                )
+            else:
+                # we are not throwing an error, because we are ignoring duplicates
+                # we are also not writing though
+                return Ok(obj)
+
+            if can_write:
+                self._set_data_and_keys(
+                    store_query_key=store_query_key,
+                    unique_query_keys=unique_query_keys,
+                    searchable_query_keys=searchable_query_keys,
+                    obj=obj,
+                )
+                self.data[uid] = obj
 
-    def _delete(
-        self, credentials: SyftVerifyKey, qk: QueryKey, has_permission: bool = False
-    ) -> Result[SyftSuccess, Err]:
-        raise NotImplementedError
+                # Add default permissions
+                if uid not in self.permissions:
+                    self.permissions[uid] = set()
+                self.add_permission(ActionObjectREAD(uid=uid, credentials=credentials))
+                if add_permissions is not None:
+                    self.add_permissions(add_permissions)
+
+                if uid not in self.storage_permissions:
+                    self.storage_permissions[uid] = set()
+                if add_storage_permission:
+                    self.add_storage_permission(
+                        StoragePermission(
+                            uid=uid,
+                            node_uid=self.node_uid,
+                        )
+                    )
 
-    def _all(
-        self,
-        credentials: SyftVerifyKey,
-        order_by: PartitionKey | None = None,
-        has_permission: bool | None = False,
-    ) -> Result[list[BaseStash.object_type], str]:
-        raise NotImplementedError
+                return Ok(obj)
+            else:
+                return Err(f"Permission: {write_permission} denied")
+        except Exception as e:
+            return Err(f"Failed to write obj {obj}. {e}")
 
-    def add_permission(self, permission: ActionObjectPermission) -> None:
-        raise NotImplementedError
+    def take_ownership(
+        self, uid: UID, credentials: SyftVerifyKey
+    ) -> Result[SyftSuccess, str]:
+        # first person using this UID can claim ownership
+        if uid not in self.permissions and uid not in self.data:
+            self.add_permissions(
+                [
+                    ActionObjectOWNER(uid=uid, credentials=credentials),
+                    ActionObjectWRITE(uid=uid, credentials=credentials),
+                    ActionObjectREAD(uid=uid, credentials=credentials),
+                    ActionObjectEXECUTE(uid=uid, credentials=credentials),
+                ]
+            )
+            return Ok(SyftSuccess(message=f"Ownership of ID: {uid} taken."))
+        return Err(f"UID: {uid} already owned.")
 
-    def add_permissions(self, permissions: list[ActionObjectPermission]) -> None:
-        raise NotImplementedError
+    def add_permission(self, permission: ActionObjectPermission) -> None:
+        permissions = self.permissions[permission.uid]
+        permissions.add(permission.permission_string)
+        self.permissions[permission.uid] = permissions
 
     def remove_permission(self, permission: ActionObjectPermission) -> None:
-        raise NotImplementedError
+        permissions = self.permissions[permission.uid]
+        permissions.remove(permission.permission_string)
+        self.permissions[permission.uid] = permissions
+
+    def add_permissions(self, permissions: list[ActionObjectPermission]) -> None:
+        for permission in permissions:
+            self.add_permission(permission)
 
     def has_permission(self, permission: ActionObjectPermission) -> bool:
-        raise NotImplementedError
+        if not isinstance(permission.permission, ActionPermission):
+            raise Exception(f"ObjectPermission type: {permission.permission} not valid")
 
-    def _migrate_data(
-        self,
-        to_klass: SyftObject,
-        context: AuthedServiceContext,
-        has_permission: bool,
-    ) -> Result[bool, str]:
-        raise NotImplementedError
+        # TODO: fix for other admins
+        if (
+            permission.credentials
+            and self.root_verify_key.verify == permission.credentials.verify
+        ):
+            return True
+
+        if (
+            permission.uid in self.permissions
+            and permission.permission_string in self.permissions[permission.uid]
+        ):
+            return True
+
+        # 🟡 TODO 14: add ALL_READ, ALL_EXECUTE etc
+        # third party
+        if permission.permission == ActionPermission.OWNER:
+            pass
+        elif (
+            permission.permission == ActionPermission.READ
+            and ActionObjectPermission(
+                permission.uid, ActionPermission.ALL_READ
+            ).permission_string
+            in self.permissions[permission.uid]
+        ):
+            return True
+        elif permission.permission == ActionPermission.WRITE:
+            pass
+        elif permission.permission == ActionPermission.EXECUTE:
+            pass
+
+        return False
+
+    def add_storage_permission(self, permission: StoragePermission) -> None:
+        permissions = self.storage_permissions[permission.uid]
+        permissions.add(permission.node_uid)
+        self.storage_permissions[permission.uid] = permissions
+
+    def add_storage_permissions(self, permissions: list[StoragePermission]) -> None:
+        for permission in permissions:
+            self.add_storage_permission(permission)
+
+    def remove_storage_permission(self, permission: StoragePermission) -> None:
+        permissions = self.storage_permissions[permission.uid]
+        permissions.remove(permission.node_uid)
+        self.storage_permissions[permission.uid] = permissions
+
+    def has_storage_permission(self, permission: StoragePermission | UID) -> bool:
+        if isinstance(permission, UID):
+            permission = StoragePermission(uid=permission, node_uid=self.node_uid)
+
+        if permission.uid in self.storage_permissions:
+            return permission.node_uid in self.storage_permissions[permission.uid]
+        return False
 
+    def _all(
+        self,
+        credentials: SyftVerifyKey,
+        order_by: PartitionKey | None = None,
+        has_permission: bool | None = False,
+    ) -> Result[list[BaseStash.object_type], str]:
+        # this checks permissions
+        res = [self._get(uid, credentials, has_permission) for uid in self.data.keys()]
+        result = [x.ok() for x in res if x.is_ok()]
+        if order_by is not None:
+            result = sorted(result, key=lambda x: getattr(x, order_by.key, ""))
+        return Ok(result)
 
-@instrument
-@serializable()
-class DocumentStore:
-    """Base Document Store
+    def _remove_keys(
+        self,
+        store_key: QueryKey,
+        unique_query_keys: QueryKeys,
+        searchable_query_keys: QueryKeys,
+    ) -> None:
+        uqks = unique_query_keys.all
+        for qk in uqks:
+            pk_key, pk_value = qk.key, qk.value
+            ck_col = self.unique_keys[pk_key]
+            ck_col.pop(store_key.value, None)
+            self.unique_keys[pk_key] = ck_col
+
+        sqks = searchable_query_keys.all
+        for qk in sqks:
+            pk_key, pk_value = qk.key, qk.value
+            ck_col = self.searchable_keys[pk_key]
+            if pk_value in ck_col and (store_key.value in ck_col[pk_value]):
+                ck_col[pk_value].remove(store_key.value)
+            self.searchable_keys[pk_key] = ck_col
 
-    Parameters:
-        store_config: StoreConfig
-            Store specific configuration.
-    """
+    def _find_index_or_search_keys(
+        self,
+        credentials: SyftVerifyKey,
+        index_qks: QueryKeys,
+        search_qks: QueryKeys,
+        order_by: PartitionKey | None = None,
+    ) -> Result[list[SyftObject], str]:
+        ids: set | None = None
+        errors = []
+        # third party
+        if len(index_qks.all) > 0:
+            index_results = self._get_keys_index(qks=index_qks)
+            if index_results.is_ok():
+                if ids is None:
+                    ids = index_results.ok()
+                ids = ids.intersection(index_results.ok())
+            else:
+                errors.append(index_results.err())
 
-    partitions: dict[str, StorePartition]
-    partition_type: type[StorePartition]
+        search_results = None
+        if len(search_qks.all) > 0:
+            search_results = self._find_keys_search(qks=search_qks)
+
+            if search_results.is_ok():
+                if ids is None:
+                    ids = search_results.ok()
+                ids = ids.intersection(search_results.ok())
+            else:
+                errors.append(search_results.err())
 
-    def __init__(
-        self,
-        node_uid: UID,
-        root_verify_key: SyftVerifyKey | None,
-        store_config: StoreConfig,
-    ) -> None:
-        if store_config is None:
-            raise Exception("must have store config")
-        self.partitions = {}
-        self.store_config = store_config
-        self.node_uid = node_uid
-        self.root_verify_key = root_verify_key
-
-    def partition(self, settings: PartitionSettings) -> StorePartition:
-        if settings.name not in self.partitions:
-            self.partitions[settings.name] = self.partition_type(
-                node_uid=self.node_uid,
-                root_verify_key=self.root_verify_key,
-                settings=settings,
-                store_config=self.store_config,
-            )
-        return self.partitions[settings.name]
+        if len(errors) > 0:
+            return Err(" ".join(errors))
 
+        if ids is None:
+            return Ok([])
 
-@instrument
-class BaseStash:
-    object_type: type[SyftObject]
-    settings: PartitionSettings
-    partition: StorePartition
-
-    def __init__(self, store: DocumentStore) -> None:
-        self.store = store
-        self.partition = store.partition(type(self).settings)
-
-    def check_type(self, obj: Any, type_: type) -> Result[Any, str]:
-        return (
-            Ok(obj)
-            if isinstance(obj, type_)
-            else Err(f"{type(obj)} does not match required type: {type_}")
+        qks: QueryKeys = self.store_query_keys(ids)
+        return self._get_all_from_store(
+            credentials=credentials, qks=qks, order_by=order_by
         )
 
-    def get_all(
+    def _update(
         self,
         credentials: SyftVerifyKey,
-        order_by: PartitionKey | None = None,
+        qk: QueryKey,
+        obj: SyftObject,
         has_permission: bool = False,
-    ) -> Result[list[BaseStash.object_type], str]:
-        return self.partition.all(credentials, order_by, has_permission)
+        overwrite: bool = False,
+    ) -> Result[SyftObject, str]:
+        try:
+            if qk.value not in self.data:
+                return Err(f"No object exists for query key: {qk}")
 
-    def add_permissions(self, permissions: list[ActionObjectPermission]) -> None:
-        self.partition.add_permissions(permissions)
+            if has_permission or self.has_permission(
+                ActionObjectWRITE(uid=qk.value, credentials=credentials)
+            ):
+                _original_obj = self.data[qk.value]
+                _original_unique_keys = self.settings.unique_keys.with_obj(
+                    _original_obj
+                )
+                _original_searchable_keys = self.settings.searchable_keys.with_obj(
+                    _original_obj
+                )
 
-    def add_permission(self, permission: ActionObjectPermission) -> None:
-        self.partition.add_permission(permission)
+                store_query_key = self.settings.store_key.with_obj(_original_obj)
 
-    def remove_permission(self, permission: ActionObjectPermission) -> None:
-        self.partition.remove_permission(permission)
+                # remove old keys
+                self._remove_keys(
+                    store_key=store_query_key,
+                    unique_query_keys=_original_unique_keys,
+                    searchable_query_keys=_original_searchable_keys,
+                )
 
-    def has_permission(self, permission: ActionObjectPermission) -> bool:
-        return self.partition.has_permission(permission=permission)
+                # update the object with new data
+                if overwrite:
+                    # Overwrite existing object and their values
+                    _original_obj = obj
+                else:
+                    for key, value in obj.to_dict(exclude_empty=True).items():
+                        if key == "id":
+                            # protected field
+                            continue
+                        setattr(_original_obj, key, value)
+
+                # update data and keys
+                self._set_data_and_keys(
+                    store_query_key=store_query_key,
+                    unique_query_keys=self.settings.unique_keys.with_obj(_original_obj),
+                    searchable_query_keys=self.settings.searchable_keys.with_obj(
+                        _original_obj
+                    ),
+                    # has been updated
+                    obj=_original_obj,
+                )
 
-    def __len__(self) -> int:
-        return len(self.partition)
+                # 🟡 TODO 28: Add locking in this transaction
 
-    def set(
-        self,
-        credentials: SyftVerifyKey,
-        obj: BaseStash.object_type,
-        add_permissions: list[ActionObjectPermission] | None = None,
-        add_storage_permission: bool = True,
-        ignore_duplicates: bool = False,
-    ) -> Result[BaseStash.object_type, str]:
-        return self.partition.set(
-            credentials=credentials,
-            obj=obj,
-            ignore_duplicates=ignore_duplicates,
-            add_permissions=add_permissions,
-            add_storage_permission=add_storage_permission,
-        )
+                return Ok(_original_obj)
+            else:
+                return Err(f"Failed to update obj {obj}, you have no permission")
+
+        except Exception as e:
+            return Err(f"Failed to update obj {obj} with error: {e}")
 
-    def query_all(
+    def _get_all_from_store(
         self,
         credentials: SyftVerifyKey,
-        qks: QueryKey | QueryKeys,
+        qks: QueryKeys,
         order_by: PartitionKey | None = None,
-    ) -> Result[list[BaseStash.object_type], str]:
-        if isinstance(qks, QueryKey):
-            qks = QueryKeys(qks=qks)
+    ) -> Result[list[SyftObject], str]:
+        matches = []
+        for qk in qks.all:
+            if qk.value in self.data:
+                if self.has_permission(
+                    ActionObjectREAD(uid=qk.value, credentials=credentials)
+                ):
+                    matches.append(self.data[qk.value])
+        if order_by is not None:
+            matches = sorted(matches, key=lambda x: getattr(x, order_by.key, ""))
+        return Ok(matches)
 
-        unique_keys = []
-        searchable_keys = []
+    def create(self, obj: SyftObject) -> Result[SyftObject, str]:
+        pass
 
-        for qk in qks.all:
-            pk = qk.partition_key
-            if self.partition.matches_unique_cks(pk):
-                unique_keys.append(qk)
-            elif self.partition.matches_searchable_cks(pk):
-                searchable_keys.append(qk)
+    def _delete(
+        self, credentials: SyftVerifyKey, qk: QueryKey, has_permission: bool = False
+    ) -> Result[SyftSuccess, Err]:
+        try:
+            if has_permission or self.has_permission(
+                ActionObjectWRITE(uid=qk.value, credentials=credentials)
+            ):
+                _obj = self.data.pop(qk.value)
+                self.permissions.pop(qk.value)
+                self.storage_permissions.pop(qk.value)
+                self._delete_unique_keys_for(_obj)
+                self._delete_search_keys_for(_obj)
+                return Ok(SyftSuccess(message="Deleted"))
             else:
                 return Err(
-                    f"{qk} not in {type(self.partition)} unique or searchable keys"
+                    f"Failed to delete with query key {qk}, you have no permission"
                 )
+        except Exception as e:
+            return Err(f"Failed to delete with query key {qk} with error: {e}")
 
-        index_qks = QueryKeys(qks=unique_keys)
-        search_qks = QueryKeys(qks=searchable_keys)
-
-        return self.partition.find_index_or_search_keys(
-            credentials=credentials,
-            index_qks=index_qks,
-            search_qks=search_qks,
-            order_by=order_by,
-        )
-
-    def query_all_kwargs(
-        self,
-        credentials: SyftVerifyKey,
-        **kwargs: dict[str, Any],
-    ) -> Result[list[BaseStash.object_type], str]:
-        order_by = kwargs.pop("order_by", None)
-        qks = QueryKeys.from_dict(kwargs)
-        return self.query_all(credentials=credentials, qks=qks, order_by=order_by)
-
-    def query_one(
-        self,
-        credentials: SyftVerifyKey,
-        qks: QueryKey | QueryKeys,
-        order_by: PartitionKey | None = None,
-    ) -> Result[BaseStash.object_type | None, str]:
-        return self.query_all(
-            credentials=credentials, qks=qks, order_by=order_by
-        ).and_then(first_or_none)
-
-    def query_one_kwargs(
-        self,
-        credentials: SyftVerifyKey,
-        **kwargs: dict[str, Any],
-    ) -> Result[BaseStash.object_type | None, str]:
-        return self.query_all_kwargs(credentials, **kwargs).and_then(first_or_none)
+    def _delete_unique_keys_for(self, obj: SyftObject) -> Result[SyftSuccess, str]:
+        for _unique_ck in self.unique_cks:
+            qk = _unique_ck.with_obj(obj)
+            unique_keys = self.unique_keys[qk.key]
+            unique_keys.pop(qk.value, None)
+            self.unique_keys[qk.key] = unique_keys
+        return Ok(SyftSuccess(message="Deleted"))
+
+    def _delete_search_keys_for(self, obj: SyftObject) -> Result[SyftSuccess, str]:
+        for _search_ck in self.searchable_cks:
+            qk = _search_ck.with_obj(obj)
+            search_keys = self.searchable_keys[qk.key]
+            search_keys.pop(qk.value, None)
+            self.searchable_keys[qk.key] = search_keys
+        return Ok(SyftSuccess(message="Deleted"))
 
-    def find_all(
-        self, credentials: SyftVerifyKey, **kwargs: dict[str, Any]
-    ) -> Result[list[BaseStash.object_type], str]:
-        return self.query_all_kwargs(credentials=credentials, **kwargs)
+    def _get_keys_index(self, qks: QueryKeys) -> Result[set[Any], str]:
+        try:
+            # match AND
+            subsets: list = []
+            for qk in qks.all:
+                subset: set = set()
+                pk_key, pk_value = qk.key, qk.value
+                if pk_key not in self.unique_keys:
+                    return Err(f"Failed to query index with {qk}")
+                ck_col = self.unique_keys[pk_key]
+                if pk_value not in ck_col.keys():
+                    # must be at least one in all query keys
+                    continue
+                store_value = ck_col[pk_value]
+                subsets.append({store_value})
+
+            if len(subsets) == 0:
+                return Ok(set())
+            # AND
+            subset = subsets.pop()
+            for s in subsets:
+                subset = subset.intersection(s)
+
+            return Ok(subset)
+        except Exception as e:
+            return Err(f"Failed to query with {qks}. {e}")
 
-    def find_one(
-        self, credentials: SyftVerifyKey, **kwargs: dict[str, Any]
-    ) -> Result[BaseStash.object_type | None, str]:
-        return self.query_one_kwargs(credentials=credentials, **kwargs)
+    def _find_keys_search(self, qks: QueryKeys) -> Result[set[QueryKey], str]:
+        try:
+            # match AND
+            subsets = []
+            for qk in qks.all:
+                subset: set = set()
+                pk_key, pk_value = qk.key, qk.value
+                if pk_key not in self.searchable_keys:
+                    return Err(f"Failed to search with {qk}")
+                ck_col = self.searchable_keys[pk_key]
+                if qk.type_list:
+                    # 🟡 TODO: change this hacky way to do on to many relationships
+                    # this is when you search a QueryKey which is a list of items
+                    # at the moment its mostly just a List[UID]
+                    # match OR against all keys for this col
+                    # the values of the list will be turned into strings in a single key
+                    matches = set()
+                    for item in pk_value:
+                        for col_key in ck_col.keys():
+                            if str(item) in col_key:
+                                store_values = ck_col[col_key]
+                                for value in store_values:
+                                    matches.add(value)
+                    if len(matches):
+                        subsets.append(matches)
+                else:
+                    # this is the normal path
+                    if pk_value not in ck_col.keys():
+                        # must be at least one in all query keys
+                        subsets.append(set())
+                        continue
+                    store_values = ck_col[pk_value]
+                    subsets.append(set(store_values))
+
+            if len(subsets) == 0:
+                return Ok(set())
+            # AND
+            subset = subsets.pop()
+            for s in subsets:
+                subset = subset.intersection(s)
+            return Ok(subset)
+        except Exception as e:
+            return Err(f"Failed to query with {qks}. {e}")
+
+    def _check_partition_keys_unique(
+        self, unique_query_keys: QueryKeys
+    ) -> UniqueKeyCheck:
+        # dont check the store key
+        qks = [
+            x
+            for x in unique_query_keys.all
+            if x.partition_key != self.settings.store_key
+        ]
+        matches = []
+        for qk in qks:
+            pk_key, pk_value = qk.key, qk.value
+            if pk_key not in self.unique_keys:
+                raise Exception(
+                    f"pk_key: {pk_key} not in unique_keys: {self.unique_keys.keys()}"
+                )
+            ck_col = self.unique_keys[pk_key]
+            if pk_value in ck_col:
+                matches.append(pk_key)
 
-    def find_and_delete(
-        self, credentials: SyftVerifyKey, **kwargs: dict[str, Any]
-    ) -> Result[SyftSuccess, Err]:
-        obj = self.query_one_kwargs(credentials=credentials, **kwargs)
-        if obj.is_err():
-            return obj
-        else:
-            obj = obj.ok()
-
-        if not obj:
-            return Err(f"Object does not exists with kwargs: {kwargs}")
-        qk = self.partition.store_query_key(obj)
-        return self.delete(credentials=credentials, qk=qk)
+        if len(matches) == 0:
+            return UniqueKeyCheck.EMPTY
+        elif len(matches) == len(qks):
+            return UniqueKeyCheck.MATCHES
 
-    def delete(
-        self, credentials: SyftVerifyKey, qk: QueryKey, has_permission: bool = False
-    ) -> Result[SyftSuccess, Err]:
-        return self.partition.delete(
-            credentials=credentials, qk=qk, has_permission=has_permission
-        )
+        return UniqueKeyCheck.ERROR
 
-    def update(
+    def _set_data_and_keys(
         self,
-        credentials: SyftVerifyKey,
-        obj: BaseStash.object_type,
-        has_permission: bool = False,
-    ) -> Result[BaseStash.object_type, str]:
-        qk = self.partition.store_query_key(obj)
-        return self.partition.update(
-            credentials=credentials, qk=qk, obj=obj, has_permission=has_permission
-        )
+        store_query_key: QueryKey,
+        unique_query_keys: QueryKeys,
+        searchable_query_keys: QueryKeys,
+        obj: SyftObject,
+    ) -> None:
+        uqks = unique_query_keys.all
 
+        for qk in uqks:
+            pk_key, pk_value = qk.key, qk.value
+            ck_col = self.unique_keys[pk_key]
+            ck_col[pk_value] = store_query_key.value
+            self.unique_keys[pk_key] = ck_col
+
+        self.unique_keys[store_query_key.key][store_query_key.value] = (
+            store_query_key.value
+        )
+
+        sqks = searchable_query_keys.all
+        for qk in sqks:
+            pk_key, pk_value = qk.key, qk.value
+            ck_col = self.searchable_keys[pk_key]
+            if qk.type_list:
+                # coerce the list of objects to strings for a single key
+                pk_value = " ".join([str(obj) for obj in pk_value])
 
-@instrument
-class BaseUIDStoreStash(BaseStash):
-    def delete_by_uid(
-        self, credentials: SyftVerifyKey, uid: UID
-    ) -> Result[SyftSuccess, str]:
-        qk = UIDPartitionKey.with_obj(uid)
-        result = super().delete(credentials=credentials, qk=qk)
-        if result.is_ok():
-            return Ok(SyftSuccess(message=f"ID: {uid} deleted"))
-        return result
-
-    def get_by_uid(
-        self, credentials: SyftVerifyKey, uid: UID
-    ) -> Result[BaseUIDStoreStash.object_type | None, str]:
-        qks = QueryKeys(qks=[UIDPartitionKey.with_obj(uid)])
-        return self.query_one(credentials=credentials, qks=qks)
+            # check if key is present, then add to existing key
+            if pk_value in ck_col:
+                ck_col[pk_value].append(store_query_key.value)
+            else:
+                # else create the key with a list
+                ck_col[pk_value] = [store_query_key.value]
 
-    def set(
-        self,
-        credentials: SyftVerifyKey,
-        obj: BaseUIDStoreStash.object_type,
-        add_permissions: list[ActionObjectPermission] | None = None,
-        add_storage_permission: bool = True,
-        ignore_duplicates: bool = False,
-    ) -> Result[BaseUIDStoreStash.object_type, str]:
-        res = self.check_type(obj, self.object_type)
-        # we dont use and_then logic here as it is hard because of the order of the arguments
-        if res.is_err():
-            return res
-        return super().set(
-            credentials=credentials,
-            obj=res.ok(),
-            ignore_duplicates=ignore_duplicates,
-            add_permissions=add_permissions,
-            add_storage_permission=add_storage_permission,
-        )
+            self.searchable_keys[pk_key] = ck_col
 
+        self.data[store_query_key.value] = obj
 
-@serializable()
-class StoreConfig(SyftBaseObject):
-    """Base Store configuration
+    def _migrate_data(
+        self, to_klass: SyftObject, context: AuthedServiceContext, has_permission: bool
+    ) -> Result[bool, str]:
+        credentials = context.credentials
+        has_permission = (credentials == self.root_verify_key) or has_permission
+        if has_permission:
+            for key, value in self.data.items():
+                try:
+                    migrated_value = value.migrate_to(to_klass.__version__, context)
+                except Exception:
+                    return Err(f"Failed to migrate data to {to_klass} for qk: {key}")
+                qk = self.settings.store_key.with_obj(key)
+                result = self._update(
+                    credentials,
+                    qk=qk,
+                    obj=migrated_value,
+                    has_permission=has_permission,
+                    overwrite=True,
+                )
 
-    Parameters:
-        store_type: Type
-            Document Store type
-        client_config: Optional[StoreClientConfig]
-            Backend-specific config
-        locking_config: LockingConfig
-            The config used for store locking. Available options:
-                * NoLockingConfig: no locking, ideal for single-thread stores.
-                * ThreadingLockingConfig: threading-based locking, ideal for same-process in-memory stores.
-                * FileLockingConfig: file based locking, ideal for same-device different-processes/threads stores.
-            Defaults to NoLockingConfig.
-    """
+                if result.is_err():
+                    return result.err()
 
-    __canonical_name__ = "StoreConfig"
-    __version__ = SYFT_OBJECT_VERSION_2
+            return Ok(True)
 
-    store_type: type[DocumentStore]
-    client_config: StoreClientConfig | None = None
-    locking_config: LockingConfig = Field(default_factory=NoLockingConfig)
+        return Err("You don't have permissions to migrate data.")
```

### Comparing `syft-0.8.6b1/src/syft/store/linked_obj.py` & `syft-0.8.7b1/src/syft/store/linked_obj.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6b1/src/syft/store/locks.py` & `syft-0.8.7b1/src/syft/store/locks.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6b1/src/syft/store/mongo_client.py` & `syft-0.8.7b1/src/syft/store/mongo_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -232,10 +232,35 @@
                 name=collection_permissions_name, codec_options=SYFT_CODEC_OPTIONS
             )
         except BaseException as e:
             return Err(str(e))
 
         return Ok(collection_permissions)
 
+    def with_collection_storage_permissions(
+        self, collection_settings: PartitionSettings, store_config: StoreConfig
+    ) -> Result[MongoCollection, Err]:
+        """
+        For each collection, create a corresponding collection
+        that store the permissions to the data in that collection
+        """
+        res = self.with_db(db_name=store_config.db_name)
+        if res.is_err():
+            return res
+        db = res.ok()
+
+        try:
+            collection_storage_permissions_name: str = (
+                collection_settings.name + "_storage_permissions"
+            )
+            storage_permissons_collection = db.get_collection(
+                name=collection_storage_permissions_name,
+                codec_options=SYFT_CODEC_OPTIONS,
+            )
+        except BaseException as e:
+            return Err(str(e))
+
+        return Ok(storage_permissons_collection)
+
     def close(self) -> None:
         self.client.close()
         MongoClientCache.__client_cache__.pop(hash(str(self.config)), None)
```

### Comparing `syft-0.8.6b1/src/syft/store/mongo_codecs.py` & `syft-0.8.7b1/src/syft/store/mongo_codecs.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6b1/src/syft/store/mongo_document_store.py` & `syft-0.8.7b1/src/syft/store/mongo_document_store.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 from ..serde.serialize import _serialize
 from ..service.action.action_permissions import ActionObjectEXECUTE
 from ..service.action.action_permissions import ActionObjectOWNER
 from ..service.action.action_permissions import ActionObjectPermission
 from ..service.action.action_permissions import ActionObjectREAD
 from ..service.action.action_permissions import ActionObjectWRITE
 from ..service.action.action_permissions import ActionPermission
+from ..service.action.action_permissions import StoragePermission
 from ..service.context import AuthedServiceContext
 from ..service.response import SyftSuccess
 from ..types.syft_object import SYFT_OBJECT_VERSION_2
 from ..types.syft_object import StorableObjectType
 from ..types.syft_object import SyftBaseObject
 from ..types.syft_object import SyftObject
 from ..types.transforms import TransformContext
@@ -144,16 +145,26 @@
 
         collection_permissions_status = client.with_collection_permissions(
             collection_settings=self.settings, store_config=self.store_config
         )
         if collection_permissions_status.is_err():
             return collection_permissions_status
 
+        collection_storage_permissions_status = (
+            client.with_collection_storage_permissions(
+                collection_settings=self.settings, store_config=self.store_config
+            )
+        )
+
+        if collection_storage_permissions_status.is_err():
+            return collection_storage_permissions_status
+
         self._collection = collection_status.ok()
         self._permissions = collection_permissions_status.ok()
+        self._storage_permissions = collection_storage_permissions_status.ok()
 
         return self._create_update_index()
 
     # Potentially thread-unsafe methods.
     #
     # CAUTION:
     #       * Don't use self.lock here.
@@ -229,14 +240,23 @@
         if not hasattr(self, "_permissions"):
             res = self.init_store()
             if res.is_err():
                 return res
 
         return Ok(self._permissions)
 
+    @property
+    def storage_permissions(self) -> Result[MongoCollection, Err]:
+        if not hasattr(self, "_storage_permissions"):
+            res = self.init_store()
+            if res.is_err():
+                return res
+
+        return Ok(self._storage_permissions)
+
     def set(self, *args: Any, **kwargs: Any) -> Result[SyftObject, str]:
         return self._set(*args, **kwargs)
 
     def _set(
         self,
         credentials: SyftVerifyKey,
         obj: SyftObject,
@@ -287,16 +307,20 @@
             )
             self.add_permission(read_permission)
 
             if add_permissions is not None:
                 self.add_permissions(add_permissions)
 
             if add_storage_permission:
-                # TODO: add storage permissions to Mongo store
-                pass
+                self.add_storage_permission(
+                    StoragePermission(
+                        uid=obj.id,
+                        node_uid=self.node_uid,
+                    )
+                )
 
             return Ok(obj)
         else:
             return Err(f"No permission to write object with id {obj.id}")
 
     def item_keys_exist(self, obj: SyftObject, collection: MongoCollection) -> bool:
         qks: QueryKeys = self.settings.unique_keys.with_obj(obj)
@@ -529,14 +553,90 @@
                     {"$set": {"permissions": permissions_strings}},
                 )
             else:
                 collection_permissions.delete_one({"_id": permission.uid})
         else:
             return Err(f"the permission {permission.permission_string} does not exist!")
 
+    def add_storage_permission(self, storage_permission: StoragePermission) -> None:
+        storage_permissions_or_err = self.storage_permissions
+        if storage_permissions_or_err.is_err():
+            return storage_permissions_or_err
+        storage_permissions_collection: MongoCollection = (
+            storage_permissions_or_err.ok()
+        )
+
+        storage_permissions: dict | None = storage_permissions_collection.find_one(
+            {"_id": storage_permission.uid}
+        )
+        if storage_permissions is None:
+            # Permission doesn't exist, add a new one
+            storage_permissions_collection.insert_one(
+                {
+                    "_id": storage_permission.uid,
+                    "node_uids": {storage_permission.node_uid},
+                }
+            )
+        else:
+            # update the permissions with the new permission string
+            node_uids: set = storage_permissions["node_uids"]
+            node_uids.add(storage_permission.node_uid)
+            storage_permissions_collection.update_one(
+                {"_id": storage_permission.uid},
+                {"$set": {"node_uids": node_uids}},
+            )
+
+    def add_storage_permissions(self, permissions: list[StoragePermission]) -> None:
+        for permission in permissions:
+            self.add_storage_permission(permission)
+
+    def has_storage_permission(self, permission: StoragePermission) -> bool:  # type: ignore
+        """Check if the storage_permission is inside the storage_permission collection"""
+        storage_permissions_or_err = self.storage_permissions
+        if storage_permissions_or_err.is_err():
+            return storage_permissions_or_err
+        storage_permissions_collection: MongoCollection = (
+            storage_permissions_or_err.ok()
+        )
+        storage_permissions: dict | None = storage_permissions_collection.find_one(
+            {"_id": permission.uid}
+        )
+
+        if storage_permissions is None or "node_uids" not in storage_permissions:
+            return False
+
+        return permission.node_uid in storage_permissions["node_uids"]
+
+    def remove_storage_permission(
+        self, storage_permission: StoragePermission
+    ) -> Result[None, Err]:
+        storage_permissions_or_err = self.storage_permissions
+        if storage_permissions_or_err.is_err():
+            return storage_permissions_or_err
+        storage_permissions_collection = storage_permissions_or_err.ok()
+
+        storage_permissions: dict | None = storage_permissions_collection.find_one(
+            {"_id": storage_permission.uid}
+        )
+        if storage_permissions is None:
+            return Err(
+                f"storage permission with UID {storage_permission.uid} not found!"
+            )
+        node_uids: set = storage_permissions["node_uids"]
+        if storage_permission.node_uid in node_uids:
+            node_uids.remove(storage_permission.node_uid)
+            storage_permissions_collection.update_one(
+                {"_id": storage_permission.uid},
+                {"$set": {"node_uids": node_uids}},
+            )
+        else:
+            return Err(
+                f"the node_uid {storage_permission.node_uid} does not exist in the storage permission!"
+            )
+
     def take_ownership(
         self, uid: UID, credentials: SyftVerifyKey
     ) -> Result[SyftSuccess, str]:
         collection_permissions_status = self.permissions
         if collection_permissions_status.is_err():
             return collection_permissions_status
         collection_permissions: MongoCollection = collection_permissions_status.ok()
```

### Comparing `syft-0.8.6b1/src/syft/store/sqlite_document_store.py` & `syft-0.8.7b1/src/syft/store/sqlite_document_store.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6b1/src/syft/types/datetime.py` & `syft-0.8.7b1/src/syft/types/datetime.py`

 * *Files 15% similar despite different names*

```diff
@@ -29,14 +29,18 @@
     def __str__(self) -> str:
         utc_datetime = datetime.utcfromtimestamp(self.utc_timestamp)
         return utc_datetime.strftime("%Y-%m-%d %H:%M:%S")
 
     def __hash__(self) -> int:
         return hash(self.utc_timestamp)
 
+    def __sub__(self, other: "DateTime") -> "DateTime":
+        res = self.utc_timestamp - other.utc_timestamp
+        return DateTime(utc_timestamp=res)
+
     def __eq__(self, other: Any) -> bool:
         if other is None:
             return False
         return self.utc_timestamp == other.utc_timestamp
 
     def __lt__(self, other: Self) -> bool:
         return self.utc_timestamp < other.utc_timestamp
```

### Comparing `syft-0.8.6b1/src/syft/types/dicttuple.py` & `syft-0.8.7b1/src/syft/types/dicttuple.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6b1/src/syft/types/grid_url.py` & `syft-0.8.7b1/src/syft/types/grid_url.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6b1/src/syft/types/identity.py` & `syft-0.8.7b1/src/syft/types/identity.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6b1/src/syft/types/syft_metaclass.py` & `syft-0.8.7b1/src/syft/types/syft_metaclass.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 # stdlib
 from typing import Any
-from typing import TypeVar
 from typing import final
 
 # third party
 from pydantic import BaseModel
 from pydantic._internal._model_construction import ModelMetaclass
 
 # relative
 from ..serde.serializable import serializable
 
-_T = TypeVar("_T", bound=BaseModel)
-
 
 class EmptyType(type):
     def __repr__(self) -> str:
         return self.__name__
 
     def __bool__(self) -> bool:
         return False
@@ -24,16 +21,26 @@
 @serializable()
 @final
 class Empty(metaclass=EmptyType):
     pass
 
 
 class PartialModelMetaclass(ModelMetaclass):
-    def __call__(cls: type[_T], *args: Any, **kwargs: Any) -> _T:
-        for field_info in cls.model_fields.values():
-            if field_info.annotation is not None and field_info.is_required():
-                field_info.annotation = field_info.annotation | EmptyType
-                field_info.default = Empty
+    def __new__(
+        mcs,
+        cls_name: str,
+        bases: tuple[type[Any], ...],
+        namespace: dict[str, Any],
+        *args: Any,
+        **kwargs: Any,
+    ) -> type:
+        cls = super().__new__(mcs, cls_name, bases, namespace, *args, **kwargs)
+
+        if issubclass(cls, BaseModel):
+            for field_info in cls.model_fields.values():
+                if field_info.annotation is not None and field_info.is_required():
+                    field_info.annotation = field_info.annotation | EmptyType
+                    field_info.default = Empty
 
-        cls.model_rebuild(force=True)
+            cls.model_rebuild(force=True)
 
-        return super().__call__(*args, **kwargs)  # type: ignore[misc]
+        return cls
```

### Comparing `syft-0.8.6b1/src/syft/types/syft_migration.py` & `syft-0.8.7b1/src/syft/types/syft_migration.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6b1/src/syft/types/syft_object.py` & `syft-0.8.7b1/src/syft/types/syft_object.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 from typing import Any
 from typing import ClassVar
 from typing import Optional
 from typing import TYPE_CHECKING
 from typing import Union
 from typing import get_args
 from typing import get_origin
-import warnings
 
 # third party
 import pandas as pd
 import pydantic
 from pydantic import ConfigDict
 from pydantic import EmailStr
 from pydantic import Field
@@ -550,43 +549,35 @@
         # 🟡 TODO 19: Could we do an mro style inheritence conversion? Risky?
         transform = SyftObjectRegistry.get_transform(type(self), projection)
         return transform(self, context)
 
     def to_dict(
         self, exclude_none: bool = False, exclude_empty: bool = False
     ) -> dict[str, Any]:
-        warnings.warn(
-            "`SyftObject.to_dict` is deprecated and will be removed in a future version",
-            PendingDeprecationWarning,
-            stacklevel=2,
-        )
-        # 🟡 TODO 18: Remove to_dict and replace usage with transforms etc
-        if not exclude_none and not exclude_empty:
-            return self.dict()
-        else:
-            new_dict = {}
-            for k, v in dict(self).items():
-                # exclude dynamically added syft attributes
-                if k in DYNAMIC_SYFT_ATTRIBUTES:
-                    continue
-                if exclude_empty and v is not Empty:
-                    new_dict[k] = v
-                if exclude_none and v is not None:
-                    new_dict[k] = v
-            return new_dict
+        new_dict = {}
+        for k, v in dict(self).items():
+            # exclude dynamically added syft attributes
+            if k in DYNAMIC_SYFT_ATTRIBUTES:
+                continue
+            if exclude_empty and v is Empty:
+                continue
+            if exclude_none and v is None:
+                continue
+            new_dict[k] = v
+        return new_dict
 
     def __post_init__(self) -> None:
         pass
 
     def _syft_set_validate_private_attrs_(self, **kwargs: Any) -> None:
         if not self.__validate_private_attrs__:
             return
         # Validate and set private attributes
         # https://github.com/pydantic/pydantic/issues/2105
-        annotations = typing.get_type_hints(self.__class__, localns=locals())
+        annotations = typing.get_type_hints(self.__class__)
         for attr, decl in self.__private_attributes__.items():
             value = kwargs.get(attr, decl.get_default())
             var_annotation = annotations.get(attr)
             if value is not PydanticUndefined:
                 if var_annotation is not None:
                     # Otherwise validate value against the variable annotation
                     check_type(value, var_annotation)
@@ -783,29 +774,31 @@
         # unpack dict
         if isinstance(_self, Mapping):
             key, item = item
             cols["key"].append(key)
 
         # get id
         id_ = getattr(item, "id", None)
-        if id_ is not None:
+        include_id = getattr(item, "__syft_include_id_coll_repr__", True)
+        if id_ is not None and include_id:
             cols["id"].append({"value": str(id_), "type": "clipboard"})
 
         if type(item) == type:
             t = full_name_with_qualname(item)
         else:
             try:
                 t = item.__class__.__name__
             except Exception:
                 t = item.__repr__()
 
         if not is_homogenous:
             cols["type"].append(t)
 
         # if has _coll_repr_
+
         if hasattr(item, "_coll_repr_"):
             ret_val = item._coll_repr_()
             if "id" in ret_val:
                 del ret_val["id"]
             for key in ret_val.keys():
                 cols[key].append(ret_val[key])
         else:
```

### Comparing `syft-0.8.6b1/src/syft/types/syncable_object.py` & `syft-0.8.7b1/src/syft/types/syncable_object.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from typing import Any
 from typing import ClassVar
 
 # third party
 from typing_extensions import Self
 
 # relative
+from ..service.context import AuthedServiceContext
 from ..service.response import SyftError
 from .syft_object import SYFT_OBJECT_VERSION_1
 from .syft_object import SyftObject
 from .uid import UID
 
 
 class SyncableSyftObject(SyftObject):
@@ -25,9 +26,11 @@
 
     def create_shareable_sync_copy(self, mock: bool) -> Self:
         update: dict[str, Any] = {}
         if mock and self._has_private_sync_attrs():
             update |= copy.deepcopy(self.__private_sync_attr_mocks__)
         return self.model_copy(update=update, deep=True)
 
-    def get_sync_dependencies(self, api: Any = None) -> list[UID] | SyftError:
+    def get_sync_dependencies(
+        self, context: AuthedServiceContext
+    ) -> list[UID] | SyftError:
         return []
```

### Comparing `syft-0.8.6b1/src/syft/types/transforms.py` & `syft-0.8.7b1/src/syft/types/transforms.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6b1/src/syft/types/twin_object.py` & `syft-0.8.7b1/src/syft/types/twin_object.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6b1/src/syft/types/uid.py` & `syft-0.8.7b1/src/syft/types/uid.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6b1/src/syft/util/_std_stream_capture.py` & `syft-0.8.7b1/src/syft/util/_std_stream_capture.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6b1/src/syft/util/autoreload.py` & `syft-0.8.7b1/src/syft/util/autoreload.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6b1/src/syft/util/decorators.py` & `syft-0.8.7b1/src/syft/util/decorators.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6b1/src/syft/util/experimental_flags.py` & `syft-0.8.7b1/src/syft/util/experimental_flags.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6b1/src/syft/util/filterwarnings.py` & `syft-0.8.7b1/src/syft/util/filterwarnings.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6b1/src/syft/util/fonts.py` & `syft-0.8.7b1/src/syft/util/fonts.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ruff: noqa
-fonts_css = """
+FONT_CSS = """
 /* cyrillic-ext */
 @font-face {
   font-family: 'Open Sans';
   font-style: normal;
   font-weight: 300 800;
   font-stretch: 100%;
   src: url(https://fonts.gstatic.com/s/opensans/v35/memvYaGs126MiZpBA-UvWbX2vVnXBbObj2OVTSKmu0SC55K5gw.woff2) format('woff2');
```

### Comparing `syft-0.8.6b1/src/syft/util/logger.py` & `syft-0.8.7b1/src/syft/util/logger.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6b1/src/syft/util/markdown.py` & `syft-0.8.7b1/src/syft/util/markdown.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6b1/src/syft/util/notebook_ui/notebook_addons.py` & `syft-0.8.7b1/src/syft/util/notebook_ui/notebook_addons.py`

 * *Files 5% similar despite different names*

```diff
@@ -254,19 +254,116 @@
         padding: 6px 4px;
         overflow: hidden;
         border: 1px solid #CFCDD6;
         background-color: var(--primary-color);
         color: var(--tertiary-color);
     }
 
+
+    .syncstate-col-footer {
+        font-family: 'DejaVu Sans Mono', 'Open Sans';
+        font-size: 12px;
+        font-weight: 400;
+        line-height: 16.8px;
+        text-align: left;
+        color: #5E5A72;
+    }
+
+    .syncstate-description {
+        font-family: Open Sans;
+        font-size: 14px;
+        font-weight: 600;
+        line-height: 19.6px;
+        text-align: left;
+    }
+
+    .diff-state-orange-text{
+        color: #B8520A;
+    }
+
+    .diff-state-no-obj{
+        font-family: 'DejaVu Sans Mono', 'Open Sans';
+        font-size: 12px;
+        font-weight: 400;
+        line-height: 16.8px;
+        text-align: left;
+        color: #5E5A72;
+    }
+
+    .diff-state-intro{
+        font-family: Open Sans;
+        font-size: 14px;
+        font-weight: 400;
+        line-height: 19.6px;
+        text-align: left;
+        color: #B4B0BF;
+    }
+
+    .diff-state-header{
+        font-family: Open Sans;
+        font-size: 22px;
+        font-weight: 600;
+        line-height: 30.8px;
+        text-align: left;
+        color: #353243;
+        display: flex; gap: 8px;
+    }
+
+    .diff-state-sub-header{
+        font-family: Open Sans;
+        font-size: 14px;
+        font-weight: 400;
+        line-height: 19.6px;
+        text-align: left;
+        color: #5E5A72;
+    }
+
     .badge {
         code-text;
         border-radius: 30px;
     }
 
+    .label {
+        code-text;
+        border-radius: 4px;
+        padding: 0px 4px;
+
+    }
+
+    .label-light-purple {
+        label;
+        background-color: #C9CFE8;
+        color: #373B7B;
+    }
+
+    .label-light-blue {
+        label;
+        background-color: #C2DEF0;
+        color: #1F567A;
+
+    }
+
+    .label-orange {
+        badge;
+        background-color: #FEE9CD;
+        color: #B8520A;
+    }
+
+    .label-gray {
+        badge;
+        background-color: #ECEBEF;
+        color: #353243;
+    }
+
+    .label-green {
+        badge;
+        background-color: #D5F1D5;
+        color: #256B24;
+    }
+
     .badge-blue {
         badge;
         background-color: #C2DEF0;
         color: #1F567A;
     }
 
     .badge-purple {
@@ -449,14 +546,21 @@
     " 7.79313L7.29313 9H4.70687L3.5 7.79313C3.40748 7.69986 3.29734 7.62592 3.17599"
     " 7.5756C3.05464 7.52528 2.9245 7.49958 2.79313 7.5H1V1H11ZM11 11H1V8.5H2.79313L4"
     " 9.70687C4.09252 9.80014 4.20266 9.87408 4.32401 9.9244C4.44536 9.97472 4.5755"
     " 10.0004 4.70687 10H7.29313C7.4245 10.0004 7.55464 9.97472 7.67599 9.9244C7.79734"
     ' 9.87408 7.90748 9.80014 8 9.70687L9.20687 8.5H11V11Z" fill="#343330"/></svg>'
 )
 
+ARROW_ICON = (
+    '<svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">'
+    '<rect x="0.5" y="0.5" width="23" height="23" rx="1.5" fill="#ECEBEF"/>'
+    '<rect x="0.5" y="0.5" width="23" height="23" rx="1.5" stroke="#B4B0BF"/>'
+    '<path d="M17.8538 12.3538L13.3538 16.8538C13.2599 16.9476 13.1327 17.0003 13 17.0003C12.8673 17.0003 12.7401 16.9476 12.6462 16.8538C12.5524 16.76 12.4997 16.6327 12.4997 16.5C12.4997 16.3674 12.5524 16.2401 12.6462 16.1463L16.2931 12.5H6.5C6.36739 12.5 6.24021 12.4474 6.14645 12.3536C6.05268 12.2598 6 12.1326 6 12C6 11.8674 6.05268 11.7402 6.14645 11.6465C6.24021 11.5527 6.36739 11.5 6.5 11.5H16.2931L12.6462 7.85378C12.5524 7.75996 12.4997 7.63272 12.4997 7.50003C12.4997 7.36735 12.5524 7.2401 12.6462 7.14628C12.7401 7.05246 12.8673 6.99976 13 6.99976C13.1327 6.99976 13.2599 7.05246 13.3538 7.14628L17.8538 11.6463C17.9002 11.6927 17.9371 11.7479 17.9623 11.8086C17.9874 11.8693 18.0004 11.9343 18.0004 12C18.0004 12.0657 17.9874 12.1308 17.9623 12.1915C17.9371 12.2522 17.9002 12.3073 17.8538 12.3538Z" fill="#5E5A72"/></svg>'  # noqa: E501
+)
+
 
 custom_code = """
     <div style='margin-top:15px;'>
         <div class='flex gap-10' style='align-items: center;'>
             <div class='folder-icon'>${icon}</div>
             <div><p class='header-3'>${list_name}</p></div>
         </div>
@@ -606,14 +710,20 @@
                                                 && item[attr].hasOwnProperty('type')) {
                                                 if (item[attr].type.includes('badge')){
                                                     let badge_div = document.createElement("div");
                                                     badge_div.classList.add('badge',item[attr].type)
                                                     badge_div.innerText = String(item[attr].value).toUpperCase();
                                                     div.appendChild(badge_div);
                                                     div.classList.add('grid-row','grid-std-cells');
+                                                } else if (item[attr].type.includes('label')){
+                                                    let label_div = document.createElement("div");
+                                                    label_div.classList.add('label',item[attr].type)
+                                                    label_div.innerText = String(item[attr].value).toUpperCase();
+                                                    div.appendChild(label_div);
+                                                    div.classList.add('grid-row','grid-std-cells');
                                                 } else if (item[attr].type === "clipboard") {
                                                     div.classList.add('grid-row','grid-std-cells');
 
                                                     // Create clipboard div
                                                     let clipboard_div = document.createElement('div');
                                                     clipboard_div.style.display= 'flex';
                                                     clipboard_div.classList.add("gap-10")
@@ -681,14 +791,20 @@
                     }
 
                     function setPage${uid}(newPage){
                         pageIndex = newPage
                         resetById${uid}('table${uid}')
                         buildGrid${uid}(paginatedElements${uid}, pageIndex)
                     }
+                    (async function() {
+                        const myFont = new FontFace('DejaVu Sans', 'url(https://cdn.jsdelivr.net/npm/dejavu-sans@1.0.0/css/dejavu-sans.min.css)');
+                        await myFont.load();
+                        document.fonts.add(myFont);
+                        document.getElementsByTagName('h1')[0].style.fontFamily = "DejaVu Sans";
+                    })();
 
                     buildPaginationContainer${uid}(paginatedElements${uid})
                 </script>
             </div>
         </div>
 """
```

### Comparing `syft-0.8.6b1/src/syft/util/schema.py` & `syft-0.8.7b1/src/syft/util/schema.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6b1/src/syft/util/telemetry.py` & `syft-0.8.7b1/src/syft/util/telemetry.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6b1/src/syft/util/trace_decorator.py` & `syft-0.8.7b1/src/syft/util/trace_decorator.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6b1/src/syft/util/util.py` & `syft-0.8.7b1/src/syft/util/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -906,7 +906,11 @@
 
     container_host = os.getenv("CONTAINER_HOST", None)
     if container_host == "k8s":
         return f"tcp://backend:{port}"
     elif container_host == "docker":
         return f"tcp://{socket.gethostname()}:{port}"
     return f"tcp://localhost:{port}"
+
+
+def get_dev_mode() -> bool:
+    return str_to_bool(os.getenv("DEV_MODE", "False"))
```

### Comparing `syft-0.8.6b1/src/syft/util/version_compare.py` & `syft-0.8.7b1/src/syft/util/version_compare.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6b1/src/syft.egg-info/PKG-INFO` & `syft-0.8.7b1/src/syft.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syft
-Version: 0.8.6b1
+Version: 0.8.7b1
 Summary: Perform numpy-like analysis on data that remains in someone elses server
 Home-page: https://openmined.github.io/PySyft/
 Author: OpenMined
 Author-email: info@openmined.org
 License: Apache-2.0
 Project-URL: Source, https://github.com/OpenMined/PySyft
 Project-URL: Tracker, https://github.com/OpenMined/PySyft/issues
@@ -48,14 +48,15 @@
 Requires-Dist: numpy<=1.24.4,>=1.23.5; python_version < "3.12"
 Requires-Dist: numpy<1.27,>=1.26.4; python_version >= "3.12"
 Requires-Dist: pandas==2.2.1
 Requires-Dist: docker==6.1.3
 Requires-Dist: kr8s==0.13.5
 Requires-Dist: PyYAML==6.0.1
 Requires-Dist: azure-storage-blob==12.19.1
+Requires-Dist: ipywidgets==8.1.2
 Provides-Extra: data-science
 Requires-Dist: transformers==4.38.2; extra == "data-science"
 Requires-Dist: opendp==0.9.2; extra == "data-science"
 Requires-Dist: evaluate==0.4.1; extra == "data-science"
 Requires-Dist: recordlinkage==0.16; extra == "data-science"
 Requires-Dist: dm-haiku==0.0.10; extra == "data-science"
 Requires-Dist: torch[cpu]==2.2.1; extra == "data-science"
@@ -101,15 +102,15 @@
 Requires-Dist: coverage; extra == "test-plugins"
 Requires-Dist: faker; extra == "test-plugins"
 Requires-Dist: distro; extra == "test-plugins"
 
 <div align="left"> <a href="https://pypi.org/project/syft/"><img src="https://static.pepy.tech/badge/pysyft" /></a> <a href="https://pypi.org/project/syft/"><img src="https://badge.fury.io/py/syft.svg" /></a> <a href="https://hub.docker.com/u/openmined"><img src="https://img.shields.io/badge/docker-images-blue?logo=docker" /></a> <a href="https://github.com/OpenMined/PySyft/actions/workflows/nightlies.yml"><img src="https://github.com/OpenMined/PySyft/actions/workflows/nightlies.yml/badge.svg?branch=dev" /></a> <a href="https://slack.openmined.org/"><img src="https://img.shields.io/badge/chat-on%20slack-purple?logo=slack" /></a> <a href="https://openmined.github.io/PySyft/"><img src="https://img.shields.io/badge/read-docs-yellow?logo=mdbook" /></a>
 <br /><br /></div>
 
-<img alt="Syft Logo" src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.6/docs/img/title_syft_light.png" width="200px" />
+<img alt="Syft Logo" src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.7/docs/img/title_syft_light.png" width="200px" />
 
 Perform data science on `data` that remains in `someone else's` server
 
 # Quickstart
 
 ✅ `Linux` ✅ `macOS` ✅ `Windows` ✅ `Docker` ✅ `Podman` ✅ `Kubernetes`
 
@@ -120,49 +121,49 @@
 ```
 
 ## Launch Server
 
 ```python
 # from Jupyter / Python
 import syft as sy
-sy.requires(">=0.8.5,<0.8.6")
+sy.requires(">=0.8.6,<0.8.7")
 node = sy.orchestra.launch(name="my-domain", port=8080, dev_mode=True, reset=True)
 ```
 
 ```bash
 # or from the command line
 $ syft launch --name=my-domain --port=8080 --reset=True
 
 Starting syft-node server on 0.0.0.0:8080
 ```
 
 ## Launch Client
 
 ```python
 import syft as sy
-sy.requires(">=0.8.5,<0.8.6")
+sy.requires(">=0.8.6,<0.8.7")
 domain_client = sy.login(port=8080, email="info@openmined.org", password="changethis")
 ```
 
 ## PySyft in 10 minutes
 
-📝 <a href="https://github.com/OpenMined/PySyft/tree/0.8.6/notebooks/api">API Example Notebooks</a>
+📝 <a href="https://github.com/OpenMined/PySyft/tree/0.8.7/notebooks/api">API Example Notebooks</a>
 
-- <a href="https://github.com/OpenMined/PySyft/tree/0.8.6/notebooks/api/0.8/00-load-data.ipynb">00-load-data.ipynb</a>
-- <a href="https://github.com/OpenMined/PySyft/tree/0.8.6/notebooks/api/0.8/01-submit-code.ipynb">01-submit-code.ipynb</a>
-- <a href="https://github.com/OpenMined/PySyft/tree/0.8.6/notebooks/api/0.8/02-review-code-and-approve.ipynb">02-review-code-and-approve.ipynb</a>
-- <a href="https://github.com/OpenMined/PySyft/tree/0.8.6/notebooks/api/0.8/03-data-scientist-download-result.ipynb">03-data-scientist-download-result.ipynb</a>
-- <a href="https://github.com/OpenMined/PySyft/tree/0.8.6/notebooks/api/0.8/04-jax-example.ipynb">04-jax-example.ipynb</a>
-- <a href="https://github.com/OpenMined/PySyft/tree/0.8.6/notebooks/api/0.8/05-custom-policy.ipynb">05-custom-policy.ipynb</a>
-- <a href="https://github.com/OpenMined/PySyft/tree/0.8.6/notebooks/api/0.8/06-multiple-code-requests.ipynb">06-multiple-code-requests.ipynb</a>
-- <a href="https://github.com/OpenMined/PySyft/tree/0.8.6/notebooks/api/0.8/07-domain-register-control-flow.ipynb">07-domain-register-control-flow.ipynb</a>
-- <a href="https://github.com/OpenMined/PySyft/tree/0.8.6/notebooks/api/0.8/08-code-version.ipynb">08-code-version.ipynb</a>
-- <a href="https://github.com/OpenMined/PySyft/tree/0.8.6/notebooks/api/0.8/09-blob-storage.ipynb">09-blob-storage.ipynb</a>
-- <a href="https://github.com/OpenMined/PySyft/tree/0.8.6/notebooks/api/0.8/10-container-images.ipynb">10-container-images.ipynb</a>
-- <a href="https://github.com/OpenMined/PySyft/tree/0.8.6/notebooks/api/0.8/11-container-images-k8s.ipynb">11-container-images-k8s.ipynb</a>
+- <a href="https://github.com/OpenMined/PySyft/tree/0.8.7/notebooks/api/0.8/00-load-data.ipynb">00-load-data.ipynb</a>
+- <a href="https://github.com/OpenMined/PySyft/tree/0.8.7/notebooks/api/0.8/01-submit-code.ipynb">01-submit-code.ipynb</a>
+- <a href="https://github.com/OpenMined/PySyft/tree/0.8.7/notebooks/api/0.8/02-review-code-and-approve.ipynb">02-review-code-and-approve.ipynb</a>
+- <a href="https://github.com/OpenMined/PySyft/tree/0.8.7/notebooks/api/0.8/03-data-scientist-download-result.ipynb">03-data-scientist-download-result.ipynb</a>
+- <a href="https://github.com/OpenMined/PySyft/tree/0.8.7/notebooks/api/0.8/04-jax-example.ipynb">04-jax-example.ipynb</a>
+- <a href="https://github.com/OpenMined/PySyft/tree/0.8.7/notebooks/api/0.8/05-custom-policy.ipynb">05-custom-policy.ipynb</a>
+- <a href="https://github.com/OpenMined/PySyft/tree/0.8.7/notebooks/api/0.8/06-multiple-code-requests.ipynb">06-multiple-code-requests.ipynb</a>
+- <a href="https://github.com/OpenMined/PySyft/tree/0.8.7/notebooks/api/0.8/07-domain-register-control-flow.ipynb">07-domain-register-control-flow.ipynb</a>
+- <a href="https://github.com/OpenMined/PySyft/tree/0.8.7/notebooks/api/0.8/08-code-version.ipynb">08-code-version.ipynb</a>
+- <a href="https://github.com/OpenMined/PySyft/tree/0.8.7/notebooks/api/0.8/09-blob-storage.ipynb">09-blob-storage.ipynb</a>
+- <a href="https://github.com/OpenMined/PySyft/tree/0.8.7/notebooks/api/0.8/10-container-images.ipynb">10-container-images.ipynb</a>
+- <a href="https://github.com/OpenMined/PySyft/tree/0.8.7/notebooks/api/0.8/11-container-images-k8s.ipynb">11-container-images-k8s.ipynb</a>
 
 ## Deploy Kubernetes Helm Chart
 
 **Note**: Assuming we have a Kubernetes cluster already setup.
 
 #### 1. Add and update Helm repo for Syft
 
@@ -233,19 +234,20 @@
 - Interactive Install 🧙🏽‍♂️ Wizard<sup>BETA</sup> Requires 🛵 `hagrid`: - Run: `hagrid quickstart`
 - PySyft 0.8.1 Requires: 🐍 `python 3.10 - 3.12` - Run: `pip install -U syft`
 - PyGrid Requires: 🐳 `docker`, 🦦 `podman` or ☸️ `kubernetes` - Run: `hagrid launch ...`
 
 # Versions
 
 `0.9.0` - Coming soon...  
-`0.8.6` (Beta) - `dev` branch 👈🏽 <a href="https://github.com/OpenMined/PySyft/tree/dev/notebooks/api/0.8">API</a> - Coming soon...  
-`0.8.5` (Stable) - <a href="https://github.com/OpenMined/PySyft/tree/0.8.5/notebooks/api/0.8">API</a>
+`0.8.7` (Beta) - `dev` branch 👈🏽 <a href="https://github.com/OpenMined/PySyft/tree/dev/notebooks/api/0.8">API</a> - Coming soon...  
+`0.8.6` (Stable) - <a href="https://github.com/OpenMined/PySyft/tree/0.8.6/notebooks/api/0.8">API</a>
 
 Deprecated:
 
+- `0.8.5-post.2` - <a href="https://github.com/OpenMined/PySyft/tree/0.8.5-post.2/notebooks/api/0.8">API</a>
 - `0.8.4` - <a href="https://github.com/OpenMined/PySyft/tree/0.8.4/notebooks/api/0.8">API</a>
 - `0.8.3` - <a href="https://github.com/OpenMined/PySyft/tree/0.8.3/notebooks/api/0.8">API</a>
 - `0.8.2` - <a href="https://github.com/OpenMined/PySyft/tree/0.8.2/notebooks/api/0.8">API</a>
 - `0.8.1` - <a href="https://github.com/OpenMined/PySyft/tree/0.8.1/notebooks/api/0.8">API</a>
 - `0.8.0` - <a href="https://github.com/OpenMined/PySyft/tree/0.8/notebooks/api/0.8">API</a>
 - `0.7.0` - <a href="https://github.com/OpenMined/courses/tree/introduction-to-remote-data-science-dev">Course 3 Updated</a>
 - `0.6.0` - <a href="https://github.com/OpenMined/courses/tree/introduction-to-remote-data-science">Course 3</a>
@@ -260,15 +262,15 @@
 PySyft (Beta): `pip install -U syft --pre`  
 PyGrid (Beta): `hagrid launch ... tag=beta`
 
 HAGrid is a cli / deployment tool so the latest version of `hagrid` is usually the best.
 
 # What is Syft?
 
-<img align="right" src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.6/docs/img/logo_big.png" alt="Syft" height="250" style="padding-left:30px;">
+<img align="right" src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.7/docs/img/logo_big.png" alt="Syft" height="250" style="padding-left:30px;">
 
 `Syft` is OpenMined's `open source` stack that provides `secure` and `private` Data Science in Python. Syft decouples `private data` from model training, using techniques like [Federated Learning](https://ai.googleblog.com/2017/04/federated-learning-collaborative.html), [Differential Privacy](https://en.wikipedia.org/wiki/Differential_privacy), and [Encrypted Computation](https://en.wikipedia.org/wiki/Homomorphic_encryption). This is done with a `numpy`-like interface and integration with `Deep Learning` frameworks, so that you as a `Data Scientist` can maintain your current workflow while using these new `privacy-enhancing techniques`.
 
 ### Why should I use Syft?
 
 `Syft` allows a `Data Scientist` to ask `questions` about a `dataset` and, within `privacy limits` set by the `data owner`, get `answers` to those `questions`, all without obtaining a `copy` of the data itself. We call this process `Remote Data Science`. It means in a wide variety of `domains` across society, the current `risks` of sharing information (`copying` data) with someone such as, privacy invasion, IP theft and blackmail will no longer prevent the vast `benefits` such as innovation, insights and scientific discovery which secure access will provide.
 
@@ -278,39 +280,39 @@
 # Tutorials
 
 <table border="5" bordercolor="grey">
 <tr>
 <th align="center">
 <img width="441" height="1">
 <div align="center">
-<img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.6/docs/img/personas_image/dataowner.png" alt="" width="100" height="100" align="center">
+<img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.7/docs/img/personas_image/dataowner.png" alt="" width="100" height="100" align="center">
 <p>Data Owner</p></div>
 </th>
 <th align="center">
 <img width="441" height="1">
-<div align="center"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.6/docs/img/personas_image/datascientist.png" alt="" width="100" height="100" align="center">
+<div align="center"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.7/docs/img/personas_image/datascientist.png" alt="" width="100" height="100" align="center">
 <p>Data Scientist</p></div>
 
 </th>
 <th align="center">
 <img width="441" height="1">
 <div align="center">
-<img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.6/docs/img/personas_image/dataengineer.png" alt="" width="100" height="100" align="center">
+<img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.7/docs/img/personas_image/dataengineer.png" alt="" width="100" height="100" align="center">
 <p>Data Engineer</p>
 </div>
 </th>
 </tr>
 <tr>
 <td valign="top">
 
-- <a href="https://github.com/OpenMined/PySyft/tree/0.8.6/notebooks/quickstart/data-owner/00-deploy-domain.ipynb">Deploy a Domain Server</a>
-- <a href="https://github.com/OpenMined/PySyft/tree/0.8.6/notebooks/quickstart/data-owner/01-upload-data.ipynb">Upload Private Data</a>
-- <a href="https://github.com/OpenMined/PySyft/tree/0.8.6/notebooks/quickstart/data-owner/02-create-account-configure-pb.ipynb">Create Accounts</a>
+- <a href="https://github.com/OpenMined/PySyft/tree/0.8.7/notebooks/quickstart/data-owner/00-deploy-domain.ipynb">Deploy a Domain Server</a>
+- <a href="https://github.com/OpenMined/PySyft/tree/0.8.7/notebooks/quickstart/data-owner/01-upload-data.ipynb">Upload Private Data</a>
+- <a href="https://github.com/OpenMined/PySyft/tree/0.8.7/notebooks/quickstart/data-owner/02-create-account-configure-pb.ipynb">Create Accounts</a>
 - Manage Privacy Budget</a>
-- <a href="https://github.com/OpenMined/PySyft/tree/0.8.6/notebooks/quickstart/data-owner/03-join-network.ipynb">Join a Network</a>
+- <a href="https://github.com/OpenMined/PySyft/tree/0.8.7/notebooks/quickstart/data-owner/03-join-network.ipynb">Join a Network</a>
 - Learn how PETs streamline Data Policies
 
 </td>
 <td valign="top">
 
 - Install Syft</a>
 - Connect to a Domain</a>
@@ -390,25 +392,25 @@
 
 <table border="5" bordercolor="grey">
 <tr>
 <th align="center" valign="top">
 <img width="441" height="1">
 <div align="center">
 
-<img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.6/docs/img/panel_slack_title_light.png" alt="" width="100%" align="center" />
+<img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.7/docs/img/panel_slack_title_light.png" alt="" width="100%" align="center" />
 
-<a href="https://slack.openmined.org/"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.6/docs/img/panel_slack.png" alt="" width="100%" align="center" /></a>
+<a href="https://slack.openmined.org/"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.7/docs/img/panel_slack.png" alt="" width="100%" align="center" /></a>
 
 </div>
 </th>
 <th align="center" valign="top">
 <img width="441" height="1">
 <div align="center">
 
-<img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.6/docs/img/panel_title_videos_papers_light.png" alt="" width="100%" align="center" />
+<img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.7/docs/img/panel_title_videos_papers_light.png" alt="" width="100%" align="center" />
 
 <p align="left"><sub><sup>
 🎥 <a href="https://www.youtube.com/watch?v=qVf0tPBzr2k">PETs: Remote Data Science Unleashed - R gov 2021</a><br />
 🎥 <a href="https://youtu.be/sCoDWKTbh3s?list=PL_lsbAsL_o2BQKXG7mkGFA8LSApCnhljL">Introduction to Remote Data Science - PyTorch 2021</a><br />
 🎥 <a href="https://youtu.be/kzLeTz_vIeQ?list=PL_lsbAsL_o2BtOz6KUfUI_Zla6Rg5dmyc">The Future of AI Tools - PyTorch 2020</a><br />
 🎥 <a href="https://www.youtube.com/watch?v=4zrU54VIK6k&t=1s">Privacy Preserving AI - MIT Deep Learning Series</a><br />
 🎥 <a href="https://www.youtube.com/watch?v=Pr4erdusiW0">Privacy-Preserving Data Science - TWiML Talk #241</a><br />
@@ -419,106 +421,106 @@
 </sup></sup></p>
 </div>
 </th>
 <th align="center" valign="top">
 <img width="441" height="1">
 <div align="center">
 
-<img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.6/docs/img/panel_padawan_title_light.png" alt="" width="100%" align="center" />
+<img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.7/docs/img/panel_padawan_title_light.png" alt="" width="100%" align="center" />
 
-<a href="https://blog.openmined.org/work-on-ais-most-exciting-frontier-no-phd-required/"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.6/docs/img/panel_padawan.png" alt="" width="100%" align="center"></a>
+<a href="https://blog.openmined.org/work-on-ais-most-exciting-frontier-no-phd-required/"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.7/docs/img/panel_padawan.png" alt="" width="100%" align="center"></a>
 
 </div>
 </th>
 </tr>
 </table>
 
 # Courses
 
 <table border="5" bordercolor="grey">
 <tr>
 <th align="center">
 <img width="441" height="1">
 <div align="center">
-<a href="https://courses.openmined.org/courses/our-privacy-opportunity"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.6/docs/img/course_privacy.png" alt="" width="100%" align="center" /></a>
+<a href="https://courses.openmined.org/courses/our-privacy-opportunity"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.7/docs/img/course_privacy.png" alt="" width="100%" align="center" /></a>
 </th>
 <th align="center">
 <img width="441" height="1">
 <div align="center">
-<a href="https://courses.openmined.org/courses/foundations-of-private-computation"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.6/docs/img/course_foundations.png" alt="" width="100%" align="center" /></a>
+<a href="https://courses.openmined.org/courses/foundations-of-private-computation"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.7/docs/img/course_foundations.png" alt="" width="100%" align="center" /></a>
 </div>
 </th>
 <th align="center">
 <img width="441" height="1">
 <div align="center">
-<a href="https://courses.openmined.org/courses/introduction-to-remote-data-science"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.6/docs/img/course_introduction.png" alt="" width="100%" align="center"></a>
+<a href="https://courses.openmined.org/courses/introduction-to-remote-data-science"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.7/docs/img/course_introduction.png" alt="" width="100%" align="center"></a>
 </div>
 </th>
 </tr>
 </table>
 
 # Contributors
 
 OpenMined and Syft appreciates all contributors, if you would like to fix a bug or suggest a new feature, please see our [guidelines](https://openmined.github.io/PySyft/developer_guide/index.html).<br />
 
-<img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.6/docs/img/contributors_light.jpg" alt="Contributors" width="100%" />
+<img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.7/docs/img/contributors_light.jpg" alt="Contributors" width="100%" />
 
 # Supporters
 
 <table border="0">
 <tr>
 <th align="center">
-<a href="https://sloan.org/"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.6/docs/img/logo_sloan.png" /></a>
+<a href="https://sloan.org/"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.7/docs/img/logo_sloan.png" /></a>
 </th>
 <th align="center">
-<a href="https://opensource.fb.com/"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.6/docs/img/logo_meta.png" /></a>
+<a href="https://opensource.fb.com/"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.7/docs/img/logo_meta.png" /></a>
 </th>
 <th align="center">
-<a href="https://pytorch.org/"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.6/docs/img/logo_torch.png" /></a>
+<a href="https://pytorch.org/"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.7/docs/img/logo_torch.png" /></a>
 </th>
 <th align="center">
 <a href="https://www.dpmc.govt.nz/">
-<img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.6/docs/img/logo_nz_light.png" />
+<img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.7/docs/img/logo_nz_light.png" />
 </a>
 </th>
 <th align="center">
-<a href="https://twitter.com/"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.6/docs/img/logo_twitter.png" /></a>
+<a href="https://twitter.com/"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.7/docs/img/logo_twitter.png" /></a>
 </th>
 <th align="center">
-<a href="https://google.com/"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.6/docs/img/logo_google.png" /></a>
+<a href="https://google.com/"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.7/docs/img/logo_google.png" /></a>
 </th>
 <th align="center">
-<a href="https://microsoft.com/"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.6/docs/img/logo_microsoft.png" /></a>
+<a href="https://microsoft.com/"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.7/docs/img/logo_microsoft.png" /></a>
 </th>
 <th align="center">
-<a href="https://omidyar.com/"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.6/docs/img/logo_on.png" /></a>
+<a href="https://omidyar.com/"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.7/docs/img/logo_on.png" /></a>
 </th>
 <th align="center">
-<a href="https://www.udacity.com/"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.6/docs/img/logo_udacity.png" /></a>
+<a href="https://www.udacity.com/"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.7/docs/img/logo_udacity.png" /></a>
 </th>
 <th align="center">
 <a href="https://www.centerfordigitalhealthinnovation.org/">
 
-<img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.6/docs/img/logo_cdhi_light.png" />
+<img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.7/docs/img/logo_cdhi_light.png" />
 
 </a>
 </th>
 <th align="center">
 <a href="https://arkhn.org/">
-<img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.6/docs/img/logo_arkhn_light.png" />
+<img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.7/docs/img/logo_arkhn_light.png" />
 </a>
 </th>
 </tr>
 </table>
 
 # Open Collective
 
 `OpenMined` is a fiscally sponsored `501(c)(3)` in the USA. We are funded by our generous supporters on <a href="https://opencollective.com/openmined">Open Collective</a>. <br /><br />
 
-<img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.6/docs/img/opencollective_light.png" alt="Contributors" width="100%" />
+<img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.7/docs/img/opencollective_light.png" alt="Contributors" width="100%" />
 
 # Disclaimer
 
 Syft is under active development and is not yet ready for pilots on private data without our assistance. As early access participants, please contact us via [Slack](https://slack.openmined.org/) or email if you would like to ask a question or have a use case that you would like to discuss.
 
 # License
```

### Comparing `syft-0.8.6b1/src/syft.egg-info/SOURCES.txt` & `syft-0.8.7b1/src/syft.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -29,39 +29,29 @@
 src/syft/client/deploy.py
 src/syft/client/domain_client.py
 src/syft/client/enclave_client.py
 src/syft/client/gateway_client.py
 src/syft/client/protocol.py
 src/syft/client/registry.py
 src/syft/client/search.py
+src/syft/client/sync_decision.py
 src/syft/client/syncing.py
 src/syft/client/user_settings.py
 src/syft/custom_worker/__init__.py
 src/syft/custom_worker/builder.py
 src/syft/custom_worker/builder_docker.py
 src/syft/custom_worker/builder_k8s.py
 src/syft/custom_worker/builder_types.py
 src/syft/custom_worker/config.py
 src/syft/custom_worker/k8s.py
 src/syft/custom_worker/runner_k8s.py
 src/syft/custom_worker/utils.py
 src/syft/exceptions/__init__.py
 src/syft/exceptions/exception.py
 src/syft/exceptions/user.py
-src/syft/external/__init__.py
-src/syft/external/oblv/__init__.py
-src/syft/external/oblv/auth.py
-src/syft/external/oblv/constants.py
-src/syft/external/oblv/deployment.py
-src/syft/external/oblv/deployment_client.py
-src/syft/external/oblv/exceptions.py
-src/syft/external/oblv/oblv_keys.py
-src/syft/external/oblv/oblv_keys_stash.py
-src/syft/external/oblv/oblv_proxy.py
-src/syft/external/oblv/oblv_service.py
 src/syft/img/base64.py
 src/syft/img/logo.png
 src/syft/img/small-grid-symbol-logo.png
 src/syft/node/__init__.py
 src/syft/node/credentials.py
 src/syft/node/domain.py
 src/syft/node/enclave.py
@@ -73,15 +63,15 @@
 src/syft/node/worker.py
 src/syft/node/worker_settings.py
 src/syft/protocol/data_protocol.py
 src/syft/protocol/protocol_version.json
 src/syft/protocol/releases/0.8.2.json
 src/syft/protocol/releases/0.8.3.json
 src/syft/protocol/releases/0.8.4.json
-src/syft/protocol/releases/0.8.5.json
+src/syft/protocol/releases/0.8.6.json
 src/syft/serde/__init__.py
 src/syft/serde/array.py
 src/syft/serde/arrow.py
 src/syft/serde/capnp.py
 src/syft/serde/deserialize.py
 src/syft/serde/lib_permissions.py
 src/syft/serde/lib_service_registry.py
@@ -95,25 +85,29 @@
 src/syft/service/__init__.py
 src/syft/service/context.py
 src/syft/service/response.py
 src/syft/service/service.py
 src/syft/service/warnings.py
 src/syft/service/action/__init__.py
 src/syft/service/action/action_data_empty.py
+src/syft/service/action/action_endpoint.py
 src/syft/service/action/action_graph.py
 src/syft/service/action/action_graph_service.py
 src/syft/service/action/action_object.py
 src/syft/service/action/action_permissions.py
 src/syft/service/action/action_service.py
 src/syft/service/action/action_store.py
 src/syft/service/action/action_types.py
 src/syft/service/action/numpy.py
 src/syft/service/action/pandas.py
 src/syft/service/action/plan.py
 src/syft/service/action/verification.py
+src/syft/service/api/api.py
+src/syft/service/api/api_service.py
+src/syft/service/api/api_stash.py
 src/syft/service/blob_storage/__init__.py
 src/syft/service/blob_storage/remote_profile.py
 src/syft/service/blob_storage/service.py
 src/syft/service/blob_storage/stash.py
 src/syft/service/code/__init__.py
 src/syft/service/code/code_parse.py
 src/syft/service/code/status_service.py
@@ -184,14 +178,15 @@
 src/syft/service/settings/__init__.py
 src/syft/service/settings/migrations.py
 src/syft/service/settings/settings.py
 src/syft/service/settings/settings_service.py
 src/syft/service/settings/settings_stash.py
 src/syft/service/sync/__init__.py
 src/syft/service/sync/diff_state.py
+src/syft/service/sync/resolve_widget.py
 src/syft/service/sync/sync_service.py
 src/syft/service/sync/sync_stash.py
 src/syft/service/sync/sync_state.py
 src/syft/service/user/__init__.py
 src/syft/service/user/roles.py
 src/syft/service/user/user.py
 src/syft/service/user/user_roles.py
```

### Comparing `syft-0.8.6b1/src/syft.egg-info/requires.txt` & `syft-0.8.7b1/src/syft.egg-info/requires.txt`

 * *Files 6% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 jaxlib==0.4.20
 jax==0.4.20
 pandas==2.2.1
 docker==6.1.3
 kr8s==0.13.5
 PyYAML==6.0.1
 azure-storage-blob==12.19.1
+ipywidgets==8.1.2
 
 [:python_version < "3.12"]
 numpy<=1.24.4,>=1.23.5
 
 [:python_version >= "3.12"]
 numpy<1.27,>=1.26.4
```

