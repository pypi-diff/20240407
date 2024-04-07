# Comparing `tmp/openapi_service_client-0.0.1.tar.gz` & `tmp/openapi_service_client-0.0.2.tar.gz`

## Comparing `openapi_service_client-0.0.1.tar` & `openapi_service_client-0.0.2.tar`

### file list

```diff
@@ -1,35 +1,36 @@
--rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 openapi_service_client-0.0.1/.github/workflows/pypi_release.yml
--rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 openapi_service_client-0.0.1/.github/workflows/tests.yml
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 openapi_service_client-0.0.1/src/openapi_service_client/__init__.py
--rw-r--r--   0        0        0     2309 2020-02-02 00:00:00.000000 openapi_service_client-0.0.1/src/openapi_service_client/client.py
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 openapi_service_client-0.0.1/src/openapi_service_client/config/__init__.py
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 openapi_service_client-0.0.1/src/openapi_service_client/config/auth_strategy.py
--rw-r--r--   0        0        0     3908 2020-02-02 00:00:00.000000 openapi_service_client-0.0.1/src/openapi_service_client/config/configuration.py
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 openapi_service_client-0.0.1/src/openapi_service_client/http_client/__init__.py
--rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 openapi_service_client-0.0.1/src/openapi_service_client/http_client/client.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 openapi_service_client-0.0.1/src/openapi_service_client/request_builder/__init__.py
--rw-r--r--   0        0        0     4090 2020-02-02 00:00:00.000000 openapi_service_client-0.0.1/src/openapi_service_client/request_builder/builder.py
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 openapi_service_client-0.0.1/src/openapi_service_client/spec/__init__.py
--rw-r--r--   0        0        0     3786 2020-02-02 00:00:00.000000 openapi_service_client-0.0.1/src/openapi_service_client/spec/open_api_spec.py
--rw-r--r--   0        0        0     2007 2020-02-02 00:00:00.000000 openapi_service_client-0.0.1/src/openapi_service_client/spec/operation.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openapi_service_client-0.0.1/tests/__init__.py
--rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 openapi_service_client-0.0.1/tests/conftest.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openapi_service_client-0.0.1/tests/client/__init__.py
--rw-r--r--   0        0        0     3711 2020-02-02 00:00:00.000000 openapi_service_client-0.0.1/tests/client/test_client.py
--rw-r--r--   0        0        0     7396 2020-02-02 00:00:00.000000 openapi_service_client-0.0.1/tests/client/test_client_auth.py
--rw-r--r--   0        0        0     2033 2020-02-02 00:00:00.000000 openapi_service_client-0.0.1/tests/client/test_client_complex_request_body.py
--rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 openapi_service_client-0.0.1/tests/client/test_client_edge_cases.py
--rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 openapi_service_client-0.0.1/tests/client/test_client_error_handling.py
--rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 openapi_service_client-0.0.1/tests/client/test_client_live.py
--rw-r--r--   0        0        0    12430 2020-02-02 00:00:00.000000 openapi_service_client-0.0.1/tests/test_files/github_compare.yml
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 openapi_service_client-0.0.1/tests/test_files/openapi_edge_cases.yml
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 openapi_service_client-0.0.1/tests/test_files/openapi_error_handling.yml
--rw-r--r--   0        0        0     5483 2020-02-02 00:00:00.000000 openapi_service_client-0.0.1/tests/test_files/openapi_greeting_service.yml
--rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 openapi_service_client-0.0.1/tests/test_files/openapi_order_service.json
--rw-r--r--   0        0        0     1412 2020-02-02 00:00:00.000000 openapi_service_client-0.0.1/tests/test_files/openapi_order_service.yml
--rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 openapi_service_client-0.0.1/tests/test_files/serper.yaml
--rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 openapi_service_client-0.0.1/.gitignore
--rw-r--r--   0        0        0    11356 2020-02-02 00:00:00.000000 openapi_service_client-0.0.1/LICENSE
--rw-r--r--   0        0        0     3999 2020-02-02 00:00:00.000000 openapi_service_client-0.0.1/README.md
--rw-r--r--   0        0        0     3793 2020-02-02 00:00:00.000000 openapi_service_client-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     4981 2020-02-02 00:00:00.000000 openapi_service_client-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 openapi_service_client-0.0.2/.github/workflows/pypi_release.yml
+-rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 openapi_service_client-0.0.2/.github/workflows/tests.yml
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 openapi_service_client-0.0.2/src/openapi_service_client/__init__.py
+-rw-r--r--   0        0        0     2978 2020-02-02 00:00:00.000000 openapi_service_client-0.0.2/src/openapi_service_client/auth_factory.py
+-rw-r--r--   0        0        0     2621 2020-02-02 00:00:00.000000 openapi_service_client-0.0.2/src/openapi_service_client/client.py
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 openapi_service_client-0.0.2/src/openapi_service_client/config/__init__.py
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 openapi_service_client-0.0.2/src/openapi_service_client/config/auth_strategy.py
+-rw-r--r--   0        0        0     3378 2020-02-02 00:00:00.000000 openapi_service_client-0.0.2/src/openapi_service_client/config/configuration.py
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 openapi_service_client-0.0.2/src/openapi_service_client/http_client/__init__.py
+-rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 openapi_service_client-0.0.2/src/openapi_service_client/http_client/client.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 openapi_service_client-0.0.2/src/openapi_service_client/request_builder/__init__.py
+-rw-r--r--   0        0        0     4090 2020-02-02 00:00:00.000000 openapi_service_client-0.0.2/src/openapi_service_client/request_builder/builder.py
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 openapi_service_client-0.0.2/src/openapi_service_client/spec/__init__.py
+-rw-r--r--   0        0        0     3786 2020-02-02 00:00:00.000000 openapi_service_client-0.0.2/src/openapi_service_client/spec/open_api_spec.py
+-rw-r--r--   0        0        0     2007 2020-02-02 00:00:00.000000 openapi_service_client-0.0.2/src/openapi_service_client/spec/operation.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openapi_service_client-0.0.2/tests/__init__.py
+-rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 openapi_service_client-0.0.2/tests/conftest.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openapi_service_client-0.0.2/tests/client/__init__.py
+-rw-r--r--   0        0        0     3711 2020-02-02 00:00:00.000000 openapi_service_client-0.0.2/tests/client/test_client.py
+-rw-r--r--   0        0        0     8804 2020-02-02 00:00:00.000000 openapi_service_client-0.0.2/tests/client/test_client_auth.py
+-rw-r--r--   0        0        0     2033 2020-02-02 00:00:00.000000 openapi_service_client-0.0.2/tests/client/test_client_complex_request_body.py
+-rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 openapi_service_client-0.0.2/tests/client/test_client_edge_cases.py
+-rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 openapi_service_client-0.0.2/tests/client/test_client_error_handling.py
+-rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 openapi_service_client-0.0.2/tests/client/test_client_live.py
+-rw-r--r--   0        0        0    12430 2020-02-02 00:00:00.000000 openapi_service_client-0.0.2/tests/test_files/github_compare.yml
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 openapi_service_client-0.0.2/tests/test_files/openapi_edge_cases.yml
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 openapi_service_client-0.0.2/tests/test_files/openapi_error_handling.yml
+-rw-r--r--   0        0        0     6359 2020-02-02 00:00:00.000000 openapi_service_client-0.0.2/tests/test_files/openapi_greeting_service.yml
+-rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 openapi_service_client-0.0.2/tests/test_files/openapi_order_service.json
+-rw-r--r--   0        0        0     1412 2020-02-02 00:00:00.000000 openapi_service_client-0.0.2/tests/test_files/openapi_order_service.yml
+-rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 openapi_service_client-0.0.2/tests/test_files/serper.yaml
+-rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 openapi_service_client-0.0.2/.gitignore
+-rw-r--r--   0        0        0    11356 2020-02-02 00:00:00.000000 openapi_service_client-0.0.2/LICENSE
+-rw-r--r--   0        0        0     5226 2020-02-02 00:00:00.000000 openapi_service_client-0.0.2/README.md
+-rw-r--r--   0        0        0     3769 2020-02-02 00:00:00.000000 openapi_service_client-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     6150 2020-02-02 00:00:00.000000 openapi_service_client-0.0.2/PKG-INFO
```

### Comparing `openapi_service_client-0.0.1/.github/workflows/tests.yml` & `openapi_service_client-0.0.2/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `openapi_service_client-0.0.1/src/openapi_service_client/client.py` & `openapi_service_client-0.0.2/src/openapi_service_client/client.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import json
 import os
 from pathlib import Path
 from typing import Any, Dict, Optional, Union
 
+from openapi_service_client.auth_factory import AuthenticationFactoryRegistry
 from openapi_service_client.config import AuthenticationStrategy
 from openapi_service_client.http_client import (
     VALID_HTTP_METHODS,
     AbstractHttpClient,
     RequestsHttpClient,
 )
 from openapi_service_client.request_builder import RequestBuilder
@@ -14,25 +15,28 @@
 
 
 class OpenAPIServiceClient:
     def __init__(
         self,
         openapi_spec: Union[str, Dict[str, Any]],
         http_client: Optional[AbstractHttpClient] = None,
-        auth_config: Optional[AuthenticationStrategy] = None,
+        auth_config: Optional[Union[str, Dict[str, Any], AuthenticationStrategy]] = None,
     ):
         if isinstance(openapi_spec, (str, Path)) and os.path.isfile(openapi_spec):
             self.openapi_spec = OpenAPISpecification.from_file(openapi_spec)
         elif isinstance(openapi_spec, dict):
             self.openapi_spec = OpenAPISpecification.from_dict(openapi_spec)
         else:
             raise ValueError("Invalid OpenAPI specification format. Expected file path or dictionary.")
 
         self.http_client = http_client or RequestsHttpClient()
-        self.request_builder = RequestBuilder(self.openapi_spec, self.http_client, auth_config=auth_config)
+
+        auth_factory_registry = AuthenticationFactoryRegistry.get_instance().get_factory()
+        created_auth_config = auth_factory_registry.create_authentication(self.openapi_spec, auth_config)
+        self.request_builder = RequestBuilder(self.openapi_spec, self.http_client, auth_config=created_auth_config)
 
     def get_operations(self) -> Dict[str, Dict[str, Operation]]:
         operations: Dict[str, Dict[str, Operation]] = {}
         for path, path_item in self.openapi_spec.get_paths().items():
             operations[path] = {}
             for method, operation in path_item.items():
                 if method in VALID_HTTP_METHODS:
```

### Comparing `openapi_service_client-0.0.1/src/openapi_service_client/http_client/client.py` & `openapi_service_client-0.0.2/src/openapi_service_client/http_client/client.py`

 * *Files identical despite different names*

### Comparing `openapi_service_client-0.0.1/src/openapi_service_client/request_builder/builder.py` & `openapi_service_client-0.0.2/src/openapi_service_client/request_builder/builder.py`

 * *Files identical despite different names*

### Comparing `openapi_service_client-0.0.1/src/openapi_service_client/spec/open_api_spec.py` & `openapi_service_client-0.0.2/src/openapi_service_client/spec/open_api_spec.py`

 * *Files identical despite different names*

### Comparing `openapi_service_client-0.0.1/src/openapi_service_client/spec/operation.py` & `openapi_service_client-0.0.2/src/openapi_service_client/spec/operation.py`

 * *Files identical despite different names*

### Comparing `openapi_service_client-0.0.1/tests/conftest.py` & `openapi_service_client-0.0.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `openapi_service_client-0.0.1/tests/client/test_client.py` & `openapi_service_client-0.0.2/tests/client/test_client.py`

 * *Files identical despite different names*

### Comparing `openapi_service_client-0.0.1/tests/client/test_client_auth.py` & `openapi_service_client-0.0.2/tests/client/test_client_auth.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,25 +8,27 @@
     HTTPBasic,
     HTTPBasicCredentials,
     HTTPBearer,
 )
 
 from openapi_service_client import OpenAPIServiceClient
 from openapi_service_client.config import ApiKeyAuthentication
-from openapi_service_client.config.configuration import HTTPAuthentication
+from openapi_service_client.config.configuration import HTTPAuthentication, OAuthAuthentication
 from tests.conftest import FastAPITestClient
 
 API_KEY = "secret_api_key"
 BASIC_AUTH_USERNAME = "admin"
 BASIC_AUTH_PASSWORD = "secret_password"
 
 API_KEY_QUERY = "secret_api_key_query"
 API_KEY_COOKIE = "secret_api_key_cookie"
 BEARER_TOKEN = "secret_bearer_token"
 
+OAUTH_TOKEN = "secret-oauth-token"
+
 api_key_query = APIKeyQuery(name="api_key")
 api_key_cookie = APIKeyCookie(name="api_key")
 bearer_auth = HTTPBearer()
 
 api_key_header = APIKeyHeader(name="X-API-Key")
 basic_auth_http = HTTPBasic()
 
@@ -109,14 +111,30 @@
     def greet_basic_auth(name: str, username: str = Depends(basic_auth)):
         greeting = f"Hello, {name} from basic_auth, using {username}"
         return JSONResponse(content={"greeting": greeting})
 
     return app
 
 
+def create_greet_oauth_auth_app() -> FastAPI:
+    app = FastAPI()
+
+    def oauth_auth(token: HTTPAuthorizationCredentials = Depends(HTTPBearer())):  # noqa: B008
+        if token.credentials != OAUTH_TOKEN:
+            raise HTTPException(status_code=status.HTTP_401_UNAUTHORIZED, detail="Invalid token")
+        return token
+
+    @app.get("/greet-oauth/{name}")
+    def greet_oauth(name: str, token: HTTPAuthorizationCredentials = Depends(oauth_auth)):  # noqa: B008
+        greeting = f"Hello, {name} from oauth_auth, using {token}"
+        return JSONResponse(content={"greeting": greeting})
+
+    return app
+
+
 class TestOpenAPIAuth:
 
     def test_greet_api_key_auth(self, test_files_path):
         client = OpenAPIServiceClient(
             test_files_path / "openapi_greeting_service.yml",
             FastAPITestClient(create_greet_api_key_auth_app()),
             ApiKeyAuthentication(API_KEY),
@@ -195,7 +213,25 @@
                 "arguments": '{"name": "John"}',
                 "name": "greetBearerAuth",
             },
             "type": "function",
         }
         response = client.invoke(payload)
         assert response == {"greeting": "Hello, John from bearer_auth, using secret_bearer_token"}
+
+    def test_greet_oauth_auth(self, test_files_path):
+        client = OpenAPIServiceClient(
+            test_files_path / "openapi_greeting_service.yml",
+            FastAPITestClient(create_greet_oauth_auth_app()),
+            OAuthAuthentication(OAUTH_TOKEN),
+        )
+        payload = {
+            "id": "call_NJr1NBz2Th7iUWJpRIJZoJIA",
+            "function": {
+                "arguments": '{"name": "John"}',
+                "name": "greetOAuth",
+            },
+            "type": "function",
+        }
+        response = client.invoke(payload)
+        auth = HTTPAuthorizationCredentials(scheme="Bearer", credentials="secret-oauth-token")
+        assert response == {"greeting": f"Hello, John from oauth_auth, using {auth}"}
```

### Comparing `openapi_service_client-0.0.1/tests/client/test_client_complex_request_body.py` & `openapi_service_client-0.0.2/tests/client/test_client_complex_request_body.py`

 * *Files identical despite different names*

### Comparing `openapi_service_client-0.0.1/tests/client/test_client_edge_cases.py` & `openapi_service_client-0.0.2/tests/client/test_client_edge_cases.py`

 * *Files identical despite different names*

### Comparing `openapi_service_client-0.0.1/tests/client/test_client_error_handling.py` & `openapi_service_client-0.0.2/tests/client/test_client_error_handling.py`

 * *Files identical despite different names*

### Comparing `openapi_service_client-0.0.1/tests/client/test_client_live.py` & `openapi_service_client-0.0.2/tests/client/test_client_live.py`

 * *Files identical despite different names*

### Comparing `openapi_service_client-0.0.1/tests/test_files/github_compare.yml` & `openapi_service_client-0.0.2/tests/test_files/github_compare.yml`

 * *Files identical despite different names*

### Comparing `openapi_service_client-0.0.1/tests/test_files/openapi_greeting_service.yml` & `openapi_service_client-0.0.2/tests/test_files/openapi_greeting_service.yml`

 * *Files 9% similar despite different names*

```diff
@@ -181,14 +181,38 @@
         '401':
           description: Unauthorized
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/ErrorResponse'
 
+  /greet-oauth/{name}:
+    get:
+      operationId: greetOAuth
+      security:
+        - OAuth2: [ ]
+      parameters:
+        - name: name
+          in: path
+          required: true
+          schema:
+            type: string
+      responses:
+        '200':
+          description: Successful response
+          content:
+            application/json:
+              schema:
+                $ref: '#/components/schemas/GreetingResponse'
+        '401':
+          description: Unauthorized
+          content:
+            application/json:
+              schema:
+                $ref: '#/components/schemas/ErrorResponse'
 components:
   securitySchemes:
     ApiKeyAuth:
       type: apiKey
       in: header
       name: X-API-Key
     BasicAuth:
@@ -201,14 +225,22 @@
     ApiKeyAuthCookie:
       type: apiKey
       in: cookie
       name: api_key
     BearerAuth:
       type: http
       scheme: bearer
+    OAuth2:
+      type: oauth2
+      flows:
+        authorizationCode:
+          authorizationUrl: https://example.com/oauth/authorize
+          tokenUrl: https://example.com/oauth/token
+          scopes:
+            read:greet: Read access to greeting service
 
   schemas:
     GreetBody:
       type: object
       properties:
         message:
           type: string
```

### Comparing `openapi_service_client-0.0.1/tests/test_files/openapi_order_service.json` & `openapi_service_client-0.0.2/tests/test_files/openapi_order_service.json`

 * *Files identical despite different names*

### Comparing `openapi_service_client-0.0.1/tests/test_files/openapi_order_service.yml` & `openapi_service_client-0.0.2/tests/test_files/openapi_order_service.yml`

 * *Files identical despite different names*

### Comparing `openapi_service_client-0.0.1/tests/test_files/serper.yaml` & `openapi_service_client-0.0.2/tests/test_files/serper.yaml`

 * *Files identical despite different names*

### Comparing `openapi_service_client-0.0.1/.gitignore` & `openapi_service_client-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `openapi_service_client-0.0.1/LICENSE` & `openapi_service_client-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `openapi_service_client-0.0.1/README.md` & `openapi_service_client-0.0.2/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -18,24 +18,26 @@
 You can install OpenAPI Service Client using pip:
 
 ```shell
 pip install openapi-service-client
 ```
 
 ## Usage
+To use the `OpenAPIServiceClient`, you need to have an OpenAPI specification file (in YAML or JSON format) that describes the API you want to interact with. Below are examples of how to use the library with both explicit and implicit authentication configurations.
 
-To use OpenAPI Service Client, you need to have an OpenAPI specification file (in YAML or JSON format) that describes the API you want to interact with. Here's an example of how to use the library:
+### Explicit Authentication
+In this example, we explicitly define the authentication mechanism by using ApiKeyAuthentication to provide the API key.
 
 ```python
 from openapi_service_client import OpenAPIServiceClient
 from openapi_service_client.config import ApiKeyAuthentication
 
 api = OpenAPIServiceClient(
     openapi_spec="/path/to/weather_service.yml",
-    auth_config=ApiKeyAuthentication("api_key")
+    auth_config=ApiKeyAuthentication(api_key="your_api_key")
 )
 
 payload = {
     "type": "function",
     "name": "weather_forecast",
     "arguments": {
         "location": "San Francisco, CA",
@@ -43,22 +45,48 @@
     }
 }
 
 response = api.invoke(payload)
 print(response)
 ```
 
-In this example, we create an instance of `OpenAPIServiceClient` by providing the path to the OpenAPI specification file and an authentication configuration using `ApiKeyAuthentication`. We then define a function-calling payload that specifies the desired operation and its arguments. Finally, we invoke the API using the `invoke()` method and print the response.
+In this scenario, ApiKeyAuthentication is utilized to directly provide the API key as part of the authentication configuration. You might want to use this approach when you want to explicitly specify the authentication method and provide the necessary credentials.
+
+### Implicit Authentication
+Alternatively, you can pass your secret token directly, and `OpenAPIServiceClient` will deduce the appropriate authentication method based on the OpenAPI specification. This approach is useful when you want the library to automatically select the correct authentication strategy.
+
+```python
+
+from openapi_service_client import OpenAPIServiceClient
+
+api = OpenAPIServiceClient(
+    openapi_spec="/path/to/weather_service.yml",
+    auth_config="your_secret_token"
+)
+
+payload = {
+    "type": "function",
+    "name": "weather_forecast",
+    "arguments": {
+        "location": "San Francisco, CA",
+        "num_days": 3
+    }
+}
+
+response = api.invoke(payload)
+print(response)
+```
+In this example, by providing a secret token as a string to auth_config, the library examines the OpenAPI specification to identify and apply the necessary authentication method (e.g., API key, OAuth2 token). This flexibility allows for a more straightforward setup when the authentication strategy can be inferred from the OpenAPI spec and the provided token.
 
 ## How It Works
 `OpenAPIServiceClient` simplifies the process of invoking REST services defined by OpenAPI specifications. It takes care of the complexities involved in making HTTP requests, handling authentication, and processing responses.
 
 When you provide an OpenAPI specification file to the client, it parses the specification and sets up the necessary request payloads and configurations to interact with the API based on the provided specification. You can then invoke specific operations using the OpenAI function-calling JSON format, which specifies the operation name and its arguments.
 
-The client handles the REST invocation by constructing the appropriate HTTP request based on the OpenAPI specification. It takes care of parameter passing, payload formatting, authentication, and error handling. The response from the API is then returned to the caller for further processing.
+The client handles the REST invocation by constructing the appropriate HTTP request based on the OpenAPI specification. It takes care of parameter placing (path, query, requestBody etc.), payload formatting, authentication, and error handling. The response from the API is then returned to the caller for further processing.
 
 By leveraging the OpenAPI specification, `OpenAPIServiceClient` eliminates the need for manual request setup and simplifies the integration process. It allows you to focus on working with LLM-generated function calls and seamlessly invoke the underlying services.
 ## Configuration
 
 OpenAPI Service Client provides various configuration options to customize the behavior of the client. You can configure authentication, HTTP client settings, and more. Refer to the documentation for detailed information on the available configuration options.
 
 ## Contributing
```

### Comparing `openapi_service_client-0.0.1/pyproject.toml` & `openapi_service_client-0.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -13,24 +13,22 @@
 keywords = []
 authors = [
   { name = "Vladimir Blagojevic", email = "dovlex@gmail.com" },
 ]
 classifiers = [
   "Development Status :: 4 - Beta",
   "Programming Language :: Python",
+  "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
-  "Programming Language :: Python :: 3.12",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
   "pyyaml",
   "requests",
-  "pydantic",
-  "pydantic-settings",
 ]
 
 [project.urls]
 Documentation = "https://github.com/vblagoje/openapi-service-client/blob/main/README.md"
 Issues = "https://github.com/vblagoje/openapi-service-client/issues"
 Source = "https://github.com/vblagoje/openapi-service-client"
 
@@ -39,14 +37,15 @@
 
 [tool.hatch.envs.default]
 dependencies = [
   "httpx",
   "fastapi",
   "coverage[toml]>=6.5",
   "pytest",
+  "pydantic",
 ]
 [tool.hatch.envs.default.scripts]
 test = "pytest {args:tests}"
 test-cov = "coverage run -m pytest {args:tests}"
 cov-report = [
   "- coverage combine",
   "coverage report",
```

### Comparing `openapi_service_client-0.0.1/PKG-INFO` & `openapi_service_client-0.0.2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 Metadata-Version: 2.3
 Name: openapi-service-client
-Version: 0.0.1
+Version: 0.0.2
 Summary: A client library for invoking APIs based on provided OpenAPI specifications
 Project-URL: Documentation, https://github.com/vblagoje/openapi-service-client/blob/main/README.md
 Project-URL: Issues, https://github.com/vblagoje/openapi-service-client/issues
 Project-URL: Source, https://github.com/vblagoje/openapi-service-client
 Author-email: Vladimir Blagojevic <dovlex@gmail.com>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.8
-Requires-Dist: pydantic
-Requires-Dist: pydantic-settings
 Requires-Dist: pyyaml
 Requires-Dist: requests
 Description-Content-Type: text/markdown
 
 # OpenAPI Service Client
 [![PyPI - Version](https://img.shields.io/pypi/v/openapi-service-client.svg)](https://pypi.org/project/openapi-service-client)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/openapi-service-client.svg)](https://pypi.org/project/openapi-service-client)
@@ -41,24 +39,26 @@
 You can install OpenAPI Service Client using pip:
 
 ```shell
 pip install openapi-service-client
 ```
 
 ## Usage
+To use the `OpenAPIServiceClient`, you need to have an OpenAPI specification file (in YAML or JSON format) that describes the API you want to interact with. Below are examples of how to use the library with both explicit and implicit authentication configurations.
 
-To use OpenAPI Service Client, you need to have an OpenAPI specification file (in YAML or JSON format) that describes the API you want to interact with. Here's an example of how to use the library:
+### Explicit Authentication
+In this example, we explicitly define the authentication mechanism by using ApiKeyAuthentication to provide the API key.
 
 ```python
 from openapi_service_client import OpenAPIServiceClient
 from openapi_service_client.config import ApiKeyAuthentication
 
 api = OpenAPIServiceClient(
     openapi_spec="/path/to/weather_service.yml",
-    auth_config=ApiKeyAuthentication("api_key")
+    auth_config=ApiKeyAuthentication(api_key="your_api_key")
 )
 
 payload = {
     "type": "function",
     "name": "weather_forecast",
     "arguments": {
         "location": "San Francisco, CA",
@@ -66,22 +66,48 @@
     }
 }
 
 response = api.invoke(payload)
 print(response)
 ```
 
-In this example, we create an instance of `OpenAPIServiceClient` by providing the path to the OpenAPI specification file and an authentication configuration using `ApiKeyAuthentication`. We then define a function-calling payload that specifies the desired operation and its arguments. Finally, we invoke the API using the `invoke()` method and print the response.
+In this scenario, ApiKeyAuthentication is utilized to directly provide the API key as part of the authentication configuration. You might want to use this approach when you want to explicitly specify the authentication method and provide the necessary credentials.
+
+### Implicit Authentication
+Alternatively, you can pass your secret token directly, and `OpenAPIServiceClient` will deduce the appropriate authentication method based on the OpenAPI specification. This approach is useful when you want the library to automatically select the correct authentication strategy.
+
+```python
+
+from openapi_service_client import OpenAPIServiceClient
+
+api = OpenAPIServiceClient(
+    openapi_spec="/path/to/weather_service.yml",
+    auth_config="your_secret_token"
+)
+
+payload = {
+    "type": "function",
+    "name": "weather_forecast",
+    "arguments": {
+        "location": "San Francisco, CA",
+        "num_days": 3
+    }
+}
+
+response = api.invoke(payload)
+print(response)
+```
+In this example, by providing a secret token as a string to auth_config, the library examines the OpenAPI specification to identify and apply the necessary authentication method (e.g., API key, OAuth2 token). This flexibility allows for a more straightforward setup when the authentication strategy can be inferred from the OpenAPI spec and the provided token.
 
 ## How It Works
 `OpenAPIServiceClient` simplifies the process of invoking REST services defined by OpenAPI specifications. It takes care of the complexities involved in making HTTP requests, handling authentication, and processing responses.
 
 When you provide an OpenAPI specification file to the client, it parses the specification and sets up the necessary request payloads and configurations to interact with the API based on the provided specification. You can then invoke specific operations using the OpenAI function-calling JSON format, which specifies the operation name and its arguments.
 
-The client handles the REST invocation by constructing the appropriate HTTP request based on the OpenAPI specification. It takes care of parameter passing, payload formatting, authentication, and error handling. The response from the API is then returned to the caller for further processing.
+The client handles the REST invocation by constructing the appropriate HTTP request based on the OpenAPI specification. It takes care of parameter placing (path, query, requestBody etc.), payload formatting, authentication, and error handling. The response from the API is then returned to the caller for further processing.
 
 By leveraging the OpenAPI specification, `OpenAPIServiceClient` eliminates the need for manual request setup and simplifies the integration process. It allows you to focus on working with LLM-generated function calls and seamlessly invoke the underlying services.
 ## Configuration
 
 OpenAPI Service Client provides various configuration options to customize the behavior of the client. You can configure authentication, HTTP client settings, and more. Refer to the documentation for detailed information on the available configuration options.
 
 ## Contributing
```

