# Comparing `tmp/responses_validator-0.1.0-cp312-cp312-win_amd64.whl.zip` & `tmp/responses_validator-0.1.1-cp312-cp312-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 58127 bytes, number of entries: 5
--rw-rw-rw-  2.0 fat     1280 b- defN 16-Jan-01 00:00 responses_validator/__init__.pyi
--rw-rw-rw-  2.0 fat   123904 b- defN 16-Jan-01 00:00 responses_validator/__init__.cp312-win_amd64.pyd
-?rw-------  2.0 fat       97 b- defN 16-Jan-01 00:00 responses_validator-0.1.0.dist-info/WHEEL
-?rw-------  2.0 fat     1902 b- defN 16-Jan-01 00:00 responses_validator-0.1.0.dist-info/METADATA
-?rw-------  2.0 fat      438 b- defN 16-Jan-01 00:00 responses_validator-0.1.0.dist-info/RECORD
-5 files, 127621 bytes uncompressed, 57311 bytes compressed:  55.1%
+Zip file size: 58413 bytes, number of entries: 5
+-rw-rw-rw-  2.0 fat     1254 b- defN 16-Jan-01 00:00 responses_validator/__init__.pyi
+-rw-rw-rw-  2.0 fat   124928 b- defN 16-Jan-01 00:00 responses_validator/__init__.cp312-win_amd64.pyd
+-rw-rw-rw-  2.0 fat     2433 b- defN 16-Jan-01 00:00 responses_validator-0.1.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      101 b- defN 16-Jan-01 00:00 responses_validator-0.1.1.dist-info/WHEEL
+?rw-------  2.0 fat      439 b- defN 16-Jan-01 00:00 responses_validator-0.1.1.dist-info/RECORD
+5 files, 129155 bytes uncompressed, 57597 bytes compressed:  55.4%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
 Filename: responses_validator/__init__.pyi
 Comment: 
 
 Filename: responses_validator/__init__.cp312-win_amd64.pyd
 Comment: 
 
-Filename: responses_validator-0.1.0.dist-info/WHEEL
+Filename: responses_validator-0.1.1.dist-info/METADATA
 Comment: 
 
-Filename: responses_validator-0.1.0.dist-info/METADATA
+Filename: responses_validator-0.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: responses_validator-0.1.0.dist-info/RECORD
+Filename: responses_validator-0.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## responses_validator/__init__.pyi

```diff
@@ -1,11 +1,9 @@
-from dataclasses import dataclass
-from dataclasses import field as field
-
 from _typeshed import Incomplete
+from dataclasses import dataclass, field as field
 
 logger: Incomplete
 
 @dataclass
 class JSONField:
     name: str | int
     value: dict
```

## Comparing `responses_validator-0.1.0.dist-info/METADATA` & `responses_validator-0.1.1.dist-info/METADATA`

 * *Files 24% similar despite different names*

```diff
@@ -1,56 +1,89 @@
-Metadata-Version: 2.1
-Name: responses-validator
-Version: 0.1.0
-Summary: Write response validation scripts for requests using flexible YAML syntax, including: status_code, headers, text, and json()
-License: MIT
-Author-email: dongfangtianyu <7629022+dongfangtianyu@users.noreply.github.com>
-Requires-Python: ~=3.12
-Requires-Dist: genson~=1.2.2
-Requires-Dist: jsonpath~=0.82.2
-Requires-Dist: jsonschema~=4.21.1
-Requires-Dist: mypy~=1.8.0
-Description-Content-Type: text/markdown
-
-# responses-validator
-
-
-```python
-import logging
-
-import requests
-from responses_validator import ResponseValidator
-from yaml import safe_load
-
-logging.basicConfig(level=logging.DEBUG)
-resp = requests.get("http://www.baidu.com/404.html")
-
-yaml_text = """
-status_code: 200 | 204   # 状态码 等于200 或 204
-headers:
-  server: 'nginx/*' # 服务器是nginx
-  Content-Type: 'application/json' # 响应类型为JSON
-json: # 默认使用glob模式可以只提供部分数据
-  name: foo
-text: qqqqq
-"""
-
-validate = safe_load(yaml_text)  # 加载yaml格式的断言
-
-obj = ResponseValidator(**validate)  # 实例化断言
-
-ret = obj.is_valid(resp)  # 对响应执行断言
-
-```
-
-```python
-  File "src\\responses_validator\\__init__.py", line 150, in responses_validator.ResponseValidator.is_valid
-responses_validator.ResponseAssertionError:
-{
-    'status_code': "status_code is 404 and does not match the pattern '200 | 204'.", 
-    'headers': "headers.server is 'Apache' and does not match the pattern '{'name': 'server', 'value': 'nginx/*', 'mode': 'glob'}'.", 
-    'text': 'text is \'<!DOCTYPE HTML PUBLIC "-//IETF//DTD HTML 2.0//EN">\n<html><head>\n<title>404 Not Found</title>\n</head><body>\n<h1>Not Found</h1>\n<p>The requested URL /404.html was not found on this server.</p>\n</body></html>\n\' and does not match the pattern \'{\'name\': \'text\', \'value\': \'qqqqq\', \'mode\': \'glob\'}\'.'}
-
-
-```
-wx: python_sanmu
-
+Metadata-Version: 2.1
+Name: responses-validator
+Version: 0.1.1
+Summary: Write response validation scripts for requests using flexible YAML syntax, including: status_code, headers, text, and json()
+License: MIT
+Author-email: dongfangtianyu <7629022+dongfangtianyu@users.noreply.github.com>
+Requires-Python: ~=3.12
+Requires-Dist: genson~=1.2.2
+Requires-Dist: jsonpath~=0.82.2
+Requires-Dist: jsonschema~=4.21.1
+Requires-Dist: mypy~=1.8.0
+Description-Content-Type: text/markdown
+
+# responses-validator
+
+
+
+A more convenient response assertion tool suitable for requests(experimental ).
+
+Write response validation scripts for requests using flexible YAML syntax, including: status_code, headers, text, and json()
+
+## Install
+
+
+
+```
+pip install responses-validator
+```
+
+
+
+
+
+
+## Example
+
+```python
+import logging
+
+import requests
+from responses_validator import ResponseValidator
+from yaml import safe_load
+
+logging.basicConfig(level=logging.DEBUG)
+resp = requests.get("http://www.baidu.com/404.html")
+
+yaml_text = """
+status_code: 200 | 204   # 状态码 等于200 或 204
+headers:
+  server: 'nginx/*' # 服务器信息包含nginx
+  Content-Type: 'application/json' # 响应类型为JSON
+json: # 默认使用glob模式可以只提供部分数据
+  name: foo
+text: qqqqq
+"""
+
+validate = safe_load(yaml_text)  # 加载yaml格式的断言
+
+obj = ResponseValidator(**validate)  # 实例化验证器
+
+ret = obj.is_valid(resp)  # 对响应执行断言
+
+```
+
+
+## Result
+```python
+  File "src\\responses_validator\\__init__.py", line 150, in responses_validator.ResponseValidator.is_valid
+responses_validator.ResponseAssertionError: 
+{
+    'status_code': "status_code is 404 and does not match the pattern '200 | 204'.", 
+    
+    'headers': "headers.server is 'Apache' and does not match the pattern '{'name': 'server', 'value': 'nginx/*', 'mode': 'glob'}'.", 
+    
+    'text': 'text is \'<!DOCTYPE HTML PUBLIC "-//IETF//DTD HTML 2.0//EN">\n<html><head>\n<title>404 Not Found</title>\n</head><body>\n<h1>Not Found</h1>\n<p>The requested URL /404.html was not found on this server.</p>\n</body></html>\n\' and does not match the pattern \'{\'name\': \'text\', \'value\': \'qqqqq\', \'mode\': \'glob\'}\'.',
+    
+    'json': "resp.json() failed! It may not be a JSON type response, please use text to verify again'."
+}
+
+
+```
+
+
+## Feedback
+
+
+
+wx: python_sanmu
+
```

