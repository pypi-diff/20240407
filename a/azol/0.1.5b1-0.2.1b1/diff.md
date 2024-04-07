# Comparing `tmp/azol-0.1.5b1.tar.gz` & `tmp/azol-0.2.1b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "azol-0.1.5b1.tar", last modified: Thu Mar 14 15:43:45 2024, max compression
+gzip compressed data, was "azol-0.2.1b1.tar", last modified: Sun Apr  7 16:39:05 2024, max compression
```

## Comparing `azol-0.1.5b1.tar` & `azol-0.2.1b1.tar`

### file list

```diff
@@ -1,53 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 15:43:45.355450 azol-0.1.5b1/
--rw-r--r--   0 runner    (1001) docker     (127)    35801 2024-03-14 15:43:33.000000 azol-0.1.5b1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-03-14 15:43:45.351450 azol-0.1.5b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      958 2024-03-14 15:43:33.000000 azol-0.1.5b1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 15:43:45.347450 azol-0.1.5b1/azol/
--rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-03-14 15:43:33.000000 azol-0.1.5b1/azol/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 15:43:45.347450 azol-0.1.5b1/azol/caches/
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-03-14 15:43:33.000000 azol-0.1.5b1/azol/caches/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5989 2024-03-14 15:43:33.000000 azol-0.1.5b1/azol/caches/azol_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-03-14 15:43:33.000000 azol-0.1.5b1/azol/caches/in_memory_token_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     2319 2024-03-14 15:43:33.000000 azol-0.1.5b1/azol/caches/local_token_cache.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 15:43:45.347450 azol-0.1.5b1/azol/clients/
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-03-14 15:43:33.000000 azol-0.1.5b1/azol/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    43193 2024-03-14 15:43:33.000000 azol-0.1.5b1/azol/clients/arm_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    29419 2024-03-14 15:43:33.000000 azol-0.1.5b1/azol/clients/graph_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3881 2024-03-14 15:43:33.000000 azol-0.1.5b1/azol/clients/key_vault_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    10939 2024-03-14 15:43:33.000000 azol-0.1.5b1/azol/clients/oauth_http_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    41448 2024-03-14 15:43:33.000000 azol-0.1.5b1/azol/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 15:43:45.351450 azol-0.1.5b1/azol/credentials/
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-03-14 15:43:33.000000 azol-0.1.5b1/azol/credentials/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-03-14 15:43:33.000000 azol-0.1.5b1/azol/credentials/access_token.py
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-03-14 15:43:33.000000 azol-0.1.5b1/azol/credentials/application_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-03-14 15:43:33.000000 azol-0.1.5b1/azol/credentials/credential.py
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-03-14 15:43:33.000000 azol-0.1.5b1/azol/credentials/entraid_credential.py
--rw-r--r--   0 runner    (1001) docker     (127)      841 2024-03-14 15:43:33.000000 azol-0.1.5b1/azol/credentials/service_principal.py
--rw-r--r--   0 runner    (1001) docker     (127)     2233 2024-03-14 15:43:33.000000 azol-0.1.5b1/azol/credentials/user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 15:43:45.351450 azol-0.1.5b1/azol/models/
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-03-14 15:43:33.000000 azol-0.1.5b1/azol/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-03-14 15:43:33.000000 azol-0.1.5b1/azol/models/generic_resource.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 15:43:45.351450 azol-0.1.5b1/azol/providers/
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-03-14 15:43:33.000000 azol-0.1.5b1/azol/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-03-14 15:43:33.000000 azol-0.1.5b1/azol/providers/file_secret_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-03-14 15:43:33.000000 azol-0.1.5b1/azol/providers/key_vault_secret_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 15:43:45.351450 azol-0.1.5b1/azol/resources/
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-03-14 15:43:33.000000 azol-0.1.5b1/azol/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   270913 2024-03-14 15:43:33.000000 azol-0.1.5b1/azol/resources/graph_delegated_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)   182559 2024-03-14 15:43:33.000000 azol-0.1.5b1/azol/resources/graph_permissions_map.py
--rw-r--r--   0 runner    (1001) docker     (127)    32330 2024-03-14 15:43:33.000000 azol-0.1.5b1/azol/resources/rbac_roles.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 15:43:45.351450 azol-0.1.5b1/azol/services/
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-03-14 15:43:33.000000 azol-0.1.5b1/azol/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20694 2024-03-14 15:43:33.000000 azol-0.1.5b1/azol/services/token_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 15:43:45.351450 azol-0.1.5b1/azol/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-03-14 15:43:33.000000 azol-0.1.5b1/azol/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2384 2024-03-14 15:43:33.000000 azol-0.1.5b1/azol/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 15:43:45.351450 azol-0.1.5b1/azol.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-03-14 15:43:45.000000 azol-0.1.5b1/azol.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-03-14 15:43:45.000000 azol-0.1.5b1/azol.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-14 15:43:45.000000 azol-0.1.5b1/azol.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-03-14 15:43:45.000000 azol-0.1.5b1/azol.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-03-14 15:43:45.000000 azol-0.1.5b1/azol.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-03-14 15:43:33.000000 azol-0.1.5b1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-14 15:43:45.355450 azol-0.1.5b1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-03-14 15:43:33.000000 azol-0.1.5b1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 16:39:05.706318 azol-0.2.1b1/
+-rw-r--r--   0 runner    (1001) docker     (127)    35801 2024-04-07 16:38:56.000000 azol-0.2.1b1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-04-07 16:39:05.706318 azol-0.2.1b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-04-07 16:38:56.000000 azol-0.2.1b1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 16:39:05.698318 azol-0.2.1b1/azol/
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-04-07 16:38:56.000000 azol-0.2.1b1/azol/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 16:39:05.698318 azol-0.2.1b1/azol/caches/
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-07 16:38:56.000000 azol-0.2.1b1/azol/caches/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5989 2024-04-07 16:38:56.000000 azol-0.2.1b1/azol/caches/azol_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-07 16:38:56.000000 azol-0.2.1b1/azol/caches/in_memory_token_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2319 2024-04-07 16:38:56.000000 azol-0.2.1b1/azol/caches/local_token_cache.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 16:39:05.702318 azol-0.2.1b1/azol/clients/
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-07 16:38:56.000000 azol-0.2.1b1/azol/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43193 2024-04-07 16:38:56.000000 azol-0.2.1b1/azol/clients/arm_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29419 2024-04-07 16:38:56.000000 azol-0.2.1b1/azol/clients/graph_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3881 2024-04-07 16:38:56.000000 azol-0.2.1b1/azol/clients/key_vault_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9083 2024-04-07 16:38:56.000000 azol-0.2.1b1/azol/clients/oauth_http_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41909 2024-04-07 16:38:56.000000 azol-0.2.1b1/azol/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 16:39:05.702318 azol-0.2.1b1/azol/credentials/
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-07 16:38:56.000000 azol-0.2.1b1/azol/credentials/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-04-07 16:38:56.000000 azol-0.2.1b1/azol/credentials/access_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-04-07 16:38:56.000000 azol-0.2.1b1/azol/credentials/application_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-04-07 16:38:56.000000 azol-0.2.1b1/azol/credentials/credential.py
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-07 16:38:56.000000 azol-0.2.1b1/azol/credentials/entraid_credential.py
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-04-07 16:38:56.000000 azol-0.2.1b1/azol/credentials/service_principal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-04-07 16:38:56.000000 azol-0.2.1b1/azol/credentials/user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 16:39:05.702318 azol-0.2.1b1/azol/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-07 16:38:56.000000 azol-0.2.1b1/azol/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-04-07 16:38:56.000000 azol-0.2.1b1/azol/models/generic_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-07 16:38:56.000000 azol-0.2.1b1/azol/models/sp_login_init_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 16:39:05.702318 azol-0.2.1b1/azol/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-07 16:38:56.000000 azol-0.2.1b1/azol/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-04-07 16:38:56.000000 azol-0.2.1b1/azol/providers/file_secret_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-04-07 16:38:56.000000 azol-0.2.1b1/azol/providers/key_vault_secret_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 16:39:05.706318 azol-0.2.1b1/azol/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-07 16:38:56.000000 azol-0.2.1b1/azol/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   270913 2024-04-07 16:38:56.000000 azol-0.2.1b1/azol/resources/graph_delegated_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)   182559 2024-04-07 16:38:56.000000 azol-0.2.1b1/azol/resources/graph_permissions_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32330 2024-04-07 16:38:56.000000 azol-0.2.1b1/azol/resources/rbac_roles.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 16:39:05.706318 azol-0.2.1b1/azol/services/
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-07 16:38:56.000000 azol-0.2.1b1/azol/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35337 2024-04-07 16:38:56.000000 azol-0.2.1b1/azol/services/token_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 16:39:05.706318 azol-0.2.1b1/azol/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-07 16:38:56.000000 azol-0.2.1b1/azol/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2279 2024-04-07 16:38:56.000000 azol-0.2.1b1/azol/utils/auth_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2659 2024-04-07 16:38:56.000000 azol-0.2.1b1/azol/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 16:39:05.706318 azol-0.2.1b1/azol.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-04-07 16:39:05.000000 azol-0.2.1b1/azol.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-04-07 16:39:05.000000 azol-0.2.1b1/azol.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 16:39:05.000000 azol-0.2.1b1/azol.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-07 16:39:05.000000 azol-0.2.1b1/azol.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-07 16:39:05.000000 azol-0.2.1b1/azol.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-07 16:38:56.000000 azol-0.2.1b1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 16:39:05.706318 azol-0.2.1b1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-07 16:38:56.000000 azol-0.2.1b1/setup.py
```

### Comparing `azol-0.1.5b1/LICENSE` & `azol-0.2.1b1/LICENSE`

 * *Files identical despite different names*

### Comparing `azol-0.1.5b1/PKG-INFO` & `azol-0.2.1b1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azol
-Version: 0.1.5b1
+Version: 0.2.1b1
 Summary: A python-based pentesting library for Azure and Entra ID
 Home-page: https://github.com/cdburkard/azol
 Author: Cody Burkard
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests==2.31.0
 Requires-Dist: dataclasses==0.6
```

### Comparing `azol-0.1.5b1/README.md` & `azol-0.2.1b1/README.md`

 * *Files identical despite different names*

### Comparing `azol-0.1.5b1/azol/__init__.py` & `azol-0.2.1b1/azol/__init__.py`

 * *Files identical despite different names*

### Comparing `azol-0.1.5b1/azol/caches/azol_cache.py` & `azol-0.2.1b1/azol/caches/azol_cache.py`

 * *Files identical despite different names*

### Comparing `azol-0.1.5b1/azol/caches/local_token_cache.py` & `azol-0.2.1b1/azol/caches/local_token_cache.py`

 * *Files identical despite different names*

### Comparing `azol-0.1.5b1/azol/clients/arm_client.py` & `azol-0.2.1b1/azol/clients/arm_client.py`

 * *Files identical despite different names*

### Comparing `azol-0.1.5b1/azol/clients/graph_client.py` & `azol-0.2.1b1/azol/clients/graph_client.py`

 * *Files identical despite different names*

### Comparing `azol-0.1.5b1/azol/clients/key_vault_client.py` & `azol-0.2.1b1/azol/clients/key_vault_client.py`

 * *Files identical despite different names*

### Comparing `azol-0.1.5b1/azol/clients/oauth_http_client.py` & `azol-0.2.1b1/azol/clients/oauth_http_client.py`

 * *Files 17% similar despite different names*

```diff
@@ -182,34 +182,16 @@
 
             Returns:
                 OAuthHTTPClient subclass
         """
         self._current_token = None
         self.token_service.switch_client(client_id)
 
-    def switch_resource(self, oauth_resource):
-        """
-            Switch the oauth resource used by the HTTP Client. Used to abuse FOCI functionality.
-
-            nullifies current cached access token, but leaves refresh token in the client.
 
-            Note: this will not create a new HTTP client object. The resource id will be used to
-                  attempt to authenticate to the existing base_url of the current HTTP client.
-
-            Vars:
-                - oauth_resource - the new oauth resource id. for example, https://graph.microsoft.com/
-
-            Returns:
-                OAuthHTTPClient subclass
-        """
-        self._current_token = None
-        self._resource=oauth_resource
-        self.token_service.switch_resource(oauth_resource)
-
-    def refresh_to_new_resource(self, oauth_http_client_class, *args, **kwargs):
+    def refresh_to_new_resource(self, oauth_http_client_class):
         """
             Generate a new HTTP Client with a different OAuth Resource, using the current token.
 
             Use this class to switch from, for example, a GraphClient to an ArmClient.
             Nullifies current cached access token, but leaves refresh token in client.
 
             Vars:
@@ -219,41 +201,17 @@
                               or KeyVaultClient
 
             Returns:
                 OAuthHTTPClient subclass instance
         """
         rt = self.get_current_refresh_token()
         user = User(refresh_token=rt)
-        client = oauth_http_client_class(*args, tenant=self._tenant, cred=user, **kwargs)
+        client = oauth_http_client_class(tenant=self._tenant, cred=user)
         return client
 
-    @classmethod
-    def from_client(cls, client, *args, **kwargs):
-        """
-            Generate a new HTTP Client with a different OAuth Resource, using the current client class.
-
-            Use this class to switch from, for example, a GraphClient to an ArmClient.
-            Nullifies current cached access token, but leaves refresh token in client.
-
-            Note: alternative to "refresh_to_new_resource" of an active client, but results in the same.
-
-            Vars:
-                - client - OAuthHTTP child class that will be used to instantiate the 
-                              new class. Note that this must be a valid
-                              OAuth HTTP child class. For example, ArmClient, GraphClient,
-                              or KeyVaultClient
-
-            Returns:
-                OAuthHTTPClient subclass instance
-        """
-        rt = client.get_current_refresh_token()
-        user = User(refresh_token=rt)
-        newClass = cls(*args, tenant=client._tenant, cred=user, **kwargs)
-        return newClass
-
     def _set_current_token(self, token):
         """
             internal: Set the current token
 
             Returns:
                 None
         """
```

### Comparing `azol-0.1.5b1/azol/constants.py` & `azol-0.2.1b1/azol/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 class OAuthResourceIDs:
     """
         A data class containing constant strings for OAuth flow types
     """
     Arm="https://management.azure.com/"
     Graph="https://graph.microsoft.com/"
     KeyVault="https://vault.azure.net/"
-    CosmosDB="https://cosmos.azure.com/"
+    CosmosDB="https://cosmos.azure.com"
     AzureDataLake="https://datalake.azure.net/"
     AzureSQL="https://database.windows.net/"
     OneNote="https://onenote.com/"
     AzureDevOps="https://app.vssps.visualstudio.com/"
     StorageAccount="https://storage.azure.com/"
     Sharepoint="https://microsoft.sharepoint.com"
     PowerBI="https://analysis.windows.net/powerbi/api/"
@@ -48,22 +48,24 @@
     """
         A data class containing constant strings for OAuth flow types
     """
     CLIENT_CREDENTIALS="client_credentials"
     DEVICE_CODE="device_code"
     REFRESH_TOKEN="refresh_token"
     RAW_TOKEN="raw_token"
+    AUTHORIZATION_CODE="authorization_code"
 
 @dataclass(frozen=True)
 class FOCIClients:
     """
         A data class containing client IDs for FOCI Clients
 
         Taken from here: https://github.com/secureworks/family-of-client-ids-research/blob/main/known-foci-clients.csv
     """
+    AzurePortal="c44b4083-3bb0-49c1-b47d-974e53cbdf3c"
     Office365Management="00b41c95-dab0-4487-9791-b9d2c32c80f2"
     MicrosoftAzurePowershell="1950a258-227b-4e31-a9cf-717495945fc2"
     MicrosoftAzureCLI="04b07795-8ddb-461a-bbee-02f9e1bf7b46"
     MicrosoftTeams="1fec8e78-bce4-4aaf-ab1b-5451cc387264"
     WindowsSearch="26a7ee05-5602-4d76-a7ba-eae8b7b67941"
     OutlookMobile="27922004-5251-4030-b22d-91ecd9a37ea4"
     MicrosoftAuthenticatorApp="4813382a-8fa7-425e-ab75-3b753aab3abb"
@@ -94,14 +96,21 @@
     MicrosoftEdge3="f44b1140-bc5e-48c6-8dc0-5cf5a53c0e34"
     M365ComplianceDriveClient="be1918be-3fe3-4be9-b32b-b542fc27f02e"
     MicrosoftDefenderPlatform="cab96880-db5b-4e15-90a7-f3f1d62ffe39"
     MicrosoftEdgeEnterpriseNewTabPage="d7b530a4-7680-4c23-a8bf-c52c121d2e87"
     MicrosoftDefenderForMobile="dd47d17a-3194-4d86-bfd5-c6ae6f5651e3"
     OutlookLite="e9b154d0-7658-433b-bb25-6b8e0a8a7c59"
 
+known_client_redirect_uris={
+    "c44b4083-3bb0-49c1-b47d-974e53cbdf3c": "https://portal.azure.com/signin/index/",
+    "1fec8e78-bce4-4aaf-ab1b-5451cc387264":"https://login.microsoftonline.com/common/oauth2/nativeclient",
+    "1950a258-227b-4e31-a9cf-717495945fc2": "http://localhost:8400",
+    "04b07795-8ddb-461a-bbee-02f9e1bf7b46": "http://localhost:21282"
+}
+
 @dataclass(frozen=True)
 class GraphAPIPermissions:
     """
         All Entra RBAC Role names mapped to their ids in a frozen data class
     """
 
 @dataclass(frozen=True)
```

### Comparing `azol-0.1.5b1/azol/credentials/access_token.py` & `azol-0.2.1b1/azol/credentials/access_token.py`

 * *Files identical despite different names*

### Comparing `azol-0.1.5b1/azol/credentials/application_object.py` & `azol-0.2.1b1/azol/credentials/application_object.py`

 * *Files identical despite different names*

### Comparing `azol-0.1.5b1/azol/credentials/credential.py` & `azol-0.2.1b1/azol/credentials/credential.py`

 * *Files identical despite different names*

### Comparing `azol-0.1.5b1/azol/credentials/service_principal.py` & `azol-0.2.1b1/azol/credentials/service_principal.py`

 * *Files identical despite different names*

### Comparing `azol-0.1.5b1/azol/credentials/user.py` & `azol-0.2.1b1/azol/credentials/user.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 """A module containing the User credential class"""
 import logging
 
-from azol.constants import FOCIClients
+from azol.constants import FOCIClients, known_client_redirect_uris
 from azol.credentials.entraid_credential import EntraIdCredential
 
 class User( EntraIdCredential ):
     """
         A credential object that may be used when a refresh token is stolen, 
         or a username/password combo is stolen
     """
 
-    supportedOAuthFlows = [ "refresh_token", "device_code" ]
+    supportedOAuthFlows = [ "refresh_token", "device_code", "authorization_code" ]
     credentialType="user"
-    default_oauth_flow="device_code"
+    default_oauth_flow="authorization_code"
 
     def __init__( self, username=None, refresh_token=None,
-                  client_id=FOCIClients.MicrosoftAzurePowershell, *args, **kwargs ):
+                  client_id=FOCIClients.AzurePortal,
+                  redirect_uri=known_client_redirect_uris[FOCIClients.AzurePortal], 
+                  *args, **kwargs ):
         """
             User objects always have a username, pasword and refresh token. 
             However, sometimes some or all of these are unknown
             during a test. Accept any combo except for password only, 
             and if none are provided, ask the user.
         """
 
@@ -29,14 +31,15 @@
         if username:
             self._username=username.lower()
         else:
             self._username=username
         self._refresh_token=refresh_token
 
         self._client_id=client_id
+        self._redirect_uri=redirect_uri
 
     def username_is_known( self ):
         """
             Returns True if the username is set on the user object
     
             Returns: bool depending on whether the username is set or not
         """
@@ -54,14 +57,22 @@
         """
             Get the current refresh token of the user object
     
             Returns: string containing the raw refresh token, or None
         """
         return self._refresh_token
 
+    def get_username( self ):
+        """
+            Get the username of the user object
+
+            Returns: username (string)
+        """
+        return self._username
+
     def set_username( self, username ):
         """
             Set the username of the user object
 
             Args:
                 -username - (string) The username to set for the user object
```

### Comparing `azol-0.1.5b1/azol/models/generic_resource.py` & `azol-0.2.1b1/azol/models/generic_resource.py`

 * *Files identical despite different names*

### Comparing `azol-0.1.5b1/azol/providers/file_secret_provider.py` & `azol-0.2.1b1/azol/providers/file_secret_provider.py`

 * *Files identical despite different names*

### Comparing `azol-0.1.5b1/azol/providers/key_vault_secret_provider.py` & `azol-0.2.1b1/azol/providers/key_vault_secret_provider.py`

 * *Files identical despite different names*

### Comparing `azol-0.1.5b1/azol/resources/graph_delegated_permissions.py` & `azol-0.2.1b1/azol/resources/graph_delegated_permissions.py`

 * *Files identical despite different names*

### Comparing `azol-0.1.5b1/azol/resources/graph_permissions_map.py` & `azol-0.2.1b1/azol/resources/graph_permissions_map.py`

 * *Files identical despite different names*

### Comparing `azol-0.1.5b1/azol/resources/rbac_roles.py` & `azol-0.2.1b1/azol/resources/rbac_roles.py`

 * *Files identical despite different names*

### Comparing `azol-0.1.5b1/azol/utils/utils.py` & `azol-0.2.1b1/azol/utils/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,22 @@
 """Module that contains functions that are useful when working with Entra ID and Azure"""
 import logging
 import json
 import base64
 import time
 import requests
 
+def string_between(whole_string, start_string, end_string, include_start=False):
+    i=whole_string.index(start_string)
+    z=whole_string[i:].index(end_string)+i
+    if not include_start:
+        i=i+len(start_string)
+    sub_string=whole_string[i:z]
+    return sub_string
+
 def get_tenant_id( tenant_name ):
     """
         Call the openid-configuration of a domain name to check if it exists in Entra ID as a tenant
 
         Returns: (string) tenant ID if the domain name is registered, or None
     """
     response = requests.get(f"https://login.microsoftonline.com/{tenant_name}/"
```

### Comparing `azol-0.1.5b1/azol.egg-info/PKG-INFO` & `azol-0.2.1b1/azol.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azol
-Version: 0.1.5b1
+Version: 0.2.1b1
 Summary: A python-based pentesting library for Azure and Entra ID
 Home-page: https://github.com/cdburkard/azol
 Author: Cody Burkard
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests==2.31.0
 Requires-Dist: dataclasses==0.6
```

### Comparing `azol-0.1.5b1/azol.egg-info/SOURCES.txt` & `azol-0.2.1b1/azol.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -23,18 +23,20 @@
 azol/credentials/application_object.py
 azol/credentials/credential.py
 azol/credentials/entraid_credential.py
 azol/credentials/service_principal.py
 azol/credentials/user.py
 azol/models/__init__.py
 azol/models/generic_resource.py
+azol/models/sp_login_init_model.py
 azol/providers/__init__.py
 azol/providers/file_secret_provider.py
 azol/providers/key_vault_secret_provider.py
 azol/resources/__init__.py
 azol/resources/graph_delegated_permissions.py
 azol/resources/graph_permissions_map.py
 azol/resources/rbac_roles.py
 azol/services/__init__.py
 azol/services/token_service.py
 azol/utils/__init__.py
+azol/utils/auth_utils.py
 azol/utils/utils.py
```

### Comparing `azol-0.1.5b1/setup.py` & `azol-0.2.1b1/setup.py`

 * *Files identical despite different names*

