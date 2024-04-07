# Comparing `tmp/pytest_yaml_sanmu-0.2.5.dev0-py3-none-any.whl.zip` & `tmp/pytest_yaml_sanmu-0.2.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 9363 bytes, number of entries: 12
+Zip file size: 9315 bytes, number of entries: 12
 -rw-r--r--  2.0 unx      174 b- defN 16-Jan-01 00:00 pytest_yaml/__init__.py
 -rw-r--r--  2.0 unx     1808 b- defN 16-Jan-01 00:00 pytest_yaml/_plugin.py
 -rw-r--r--  2.0 unx     7442 b- defN 16-Jan-01 00:00 pytest_yaml/file.py
 -rw-r--r--  2.0 unx      661 b- defN 16-Jan-01 00:00 pytest_yaml/hooks.py
 -rw-r--r--  2.0 unx      874 b- defN 16-Jan-01 00:00 pytest_yaml/models.py
 -rw-r--r--  2.0 unx     1425 b- defN 16-Jan-01 00:00 pytest_yaml/plugin.py
 -rw-r--r--  2.0 unx     2492 b- defN 16-Jan-01 00:00 pytest_yaml/templates.py
--rw-r--r--  2.0 unx     2726 b- defN 16-Jan-01 00:00 pytest_yaml/yaml_case.schema.yaml
-?rw-------  2.0 unx       36 b- defN 16-Jan-01 00:00 pytest_yaml_sanmu-0.2.5.dev0.dist-info/entry_points.txt
-?rw-------  2.0 unx       87 b- defN 16-Jan-01 00:00 pytest_yaml_sanmu-0.2.5.dev0.dist-info/WHEEL
-?rw-------  2.0 unx     1934 b- defN 16-Jan-01 00:00 pytest_yaml_sanmu-0.2.5.dev0.dist-info/METADATA
-?rw-------  2.0 unx      997 b- defN 16-Jan-01 00:00 pytest_yaml_sanmu-0.2.5.dev0.dist-info/RECORD
-12 files, 20656 bytes uncompressed, 7681 bytes compressed:  62.8%
+-rw-r--r--  2.0 unx     2732 b- defN 16-Jan-01 00:00 pytest_yaml/yaml_case.schema.yaml
+?rw-------  2.0 unx       36 b- defN 16-Jan-01 00:00 pytest_yaml_sanmu-0.2.6.dist-info/entry_points.txt
+?rw-------  2.0 unx       87 b- defN 16-Jan-01 00:00 pytest_yaml_sanmu-0.2.6.dist-info/WHEEL
+?rw-------  2.0 unx     1930 b- defN 16-Jan-01 00:00 pytest_yaml_sanmu-0.2.6.dist-info/METADATA
+?rw-------  2.0 unx      977 b- defN 16-Jan-01 00:00 pytest_yaml_sanmu-0.2.6.dist-info/RECORD
+12 files, 20638 bytes uncompressed, 7673 bytes compressed:  62.8%
```

## zipnote {}

```diff
@@ -18,20 +18,20 @@
 
 Filename: pytest_yaml/templates.py
 Comment: 
 
 Filename: pytest_yaml/yaml_case.schema.yaml
 Comment: 
 
-Filename: pytest_yaml_sanmu-0.2.5.dev0.dist-info/entry_points.txt
+Filename: pytest_yaml_sanmu-0.2.6.dist-info/entry_points.txt
 Comment: 
 
-Filename: pytest_yaml_sanmu-0.2.5.dev0.dist-info/WHEEL
+Filename: pytest_yaml_sanmu-0.2.6.dist-info/WHEEL
 Comment: 
 
-Filename: pytest_yaml_sanmu-0.2.5.dev0.dist-info/METADATA
+Filename: pytest_yaml_sanmu-0.2.6.dist-info/METADATA
 Comment: 
 
-Filename: pytest_yaml_sanmu-0.2.5.dev0.dist-info/RECORD
+Filename: pytest_yaml_sanmu-0.2.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pytest_yaml/yaml_case.schema.yaml

```diff
@@ -11,15 +11,15 @@
   mark:
     items:
       anyOf:
         - type: string
         - properties:
             order:
               type: integer
-            description: '用例排序，依赖插件: pytest-order'
+              description: '用例排序，依赖插件: pytest-order'
           required:
             - order
           type: object
         - properties:
             usefixtures:
               items:
                 type: string
@@ -43,22 +43,22 @@
               description: 跳过用例，并标注原因
           required:
             - skip
           type: object
         - properties:
             skipif:
               type: string
-            description: 满足条件时跳过用例
+              description: 满足条件时跳过用例
           required:
             - skipif
           type: object
         - properties:
             xfail:
               type: string
-            description: 预期本用例失败
+              description: 预期本用例失败
           required:
             - xfail
           type: object
         - properties:
             parametrize:
               properties:
                 keys:
```

## Comparing `pytest_yaml_sanmu-0.2.5.dev0.dist-info/METADATA` & `pytest_yaml_sanmu-0.2.6.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: pytest-yaml-sanmu
-Version: 0.2.5.dev
+Version: 0.2.6
 Summary: pytest plugin for generating test cases by yaml
 License: Apache-2.0
 Author-email: dongfangtianyu <7629022+dongfangtianyu@users.noreply.github.com>
 Requires-Python: >=3.10
 Requires-Dist: allure-pytest>=2.13.0
 Requires-Dist: jsonschema>=4.20.0
 Requires-Dist: pydantic<3,>=2.0
 Requires-Dist: pytest>=7.4.0
-Requires-Dist: pyyaml-include>=1.3.1
+Requires-Dist: pyyaml-include~=1.3.1
 Requires-Dist: pyyaml>=6.0
 Project-URL: Homepage, https://github.com/dongfangtianyu/pytest-yaml-sanmul
 Description-Content-Type: text/markdown
 
 # pytest-yml
 
 pytest plugin for generating test cases by yaml
```

## Comparing `pytest_yaml_sanmu-0.2.5.dev0.dist-info/RECORD` & `pytest_yaml_sanmu-0.2.6.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 pytest_yaml/__init__.py,sha256=DGKoLcZrOO_Q1R-uNFCgvO_hhgM6cBMMaJJ_zufaWDo,174
 pytest_yaml/_plugin.py,sha256=0f_8bkaORTtcEn8HAoyMy-J1E5yULjA0CP1i4ExVs24,1808
 pytest_yaml/file.py,sha256=dxsuQUlKFPkmGJrpYO4AoqPfhliTUEkPD9IYJViWNgE,7442
 pytest_yaml/hooks.py,sha256=cclZKDIxTpWoRFZHqXzukmSwPjpmx8aH1iSWhs0Io8o,661
 pytest_yaml/models.py,sha256=ZeBqFcCSx6y7sZn6dSR5-PT0Z3icZx95v_vjA7Hil78,874
 pytest_yaml/plugin.py,sha256=Z69brEVc5wZVvFYMUfqd1iAUt_RmaBtHN8C1kLYzmwM,1425
 pytest_yaml/templates.py,sha256=MECMa6K_EZk9dD3enOSfG4nxoaFqCm7SdnZe0iu2K3E,2492
-pytest_yaml/yaml_case.schema.yaml,sha256=pM7NOxe_Y3gdzktzIjOXodyuPaeyLpr_y080aNItJeM,2726
-pytest_yaml_sanmu-0.2.5.dev0.dist-info/entry_points.txt,sha256=pEQ-BthnhQfWoRegIMd3s8W8oR9tMHZz_soP_RAGXTs,36
-pytest_yaml_sanmu-0.2.5.dev0.dist-info/WHEEL,sha256=B19PGBCYhWaz2p_UjAoRVh767nYQfk14Sn4TpIZ-nfU,87
-pytest_yaml_sanmu-0.2.5.dev0.dist-info/METADATA,sha256=BPq0Lth2A-8tHa9_QthqveGUDQ9t_JH5KbG03wWqO94,1934
-pytest_yaml_sanmu-0.2.5.dev0.dist-info/RECORD,,
+pytest_yaml/yaml_case.schema.yaml,sha256=wy9BG1miWAQxFOMAcJkmbHg-nk7J0QsEDJTFduSEydc,2732
+pytest_yaml_sanmu-0.2.6.dist-info/entry_points.txt,sha256=pEQ-BthnhQfWoRegIMd3s8W8oR9tMHZz_soP_RAGXTs,36
+pytest_yaml_sanmu-0.2.6.dist-info/WHEEL,sha256=B19PGBCYhWaz2p_UjAoRVh767nYQfk14Sn4TpIZ-nfU,87
+pytest_yaml_sanmu-0.2.6.dist-info/METADATA,sha256=3Vx7A655OWuxVo1E-XnQJjyFs_CxvVZTr4CxDYS6jaM,1930
+pytest_yaml_sanmu-0.2.6.dist-info/RECORD,,
```

