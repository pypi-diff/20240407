# Comparing `tmp/phc-ingestion-0.7.4.tar.gz` & `tmp/phc-ingestion-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phc-ingestion-0.7.4.tar", last modified: Mon Apr  1 22:07:20 2024, max compression
+gzip compressed data, was "phc-ingestion-0.8.0.tar", last modified: Sun Apr  7 13:29:20 2024, max compression
```

## Comparing `phc-ingestion-0.7.4.tar` & `phc-ingestion-0.8.0.tar`

### file list

```diff
@@ -1,51 +1,54 @@
--rw-r--r--   0        0        0       16 2024-04-01 22:06:40.809031 phc-ingestion-0.7.4/PYPI.md
--rw-r--r--   0        0        0        0 2024-04-01 22:06:40.809031 phc-ingestion-0.7.4/ingestion/__init__.py
--rw-r--r--   0        0        0       61 2024-04-01 22:06:40.809031 phc-ingestion-0.7.4/ingestion/caris/__init__.py
--rw-r--r--   0        0        0     1636 2024-04-01 22:06:40.809031 phc-ingestion-0.7.4/ingestion/caris/process.py
--rw-r--r--   0        0        0        0 2024-04-01 22:06:40.809031 phc-ingestion-0.7.4/ingestion/caris/util/__init__.py
--rw-r--r--   0        0        0     4738 2024-04-01 22:06:40.809031 phc-ingestion-0.7.4/ingestion/caris/util/cnv.py
--rw-r--r--   0        0        0     1640 2024-04-01 22:06:40.809031 phc-ingestion-0.7.4/ingestion/caris/util/detect_genome_ref.py
--rw-r--r--   0        0        0      629 2024-04-01 22:06:40.809031 phc-ingestion-0.7.4/ingestion/caris/util/ga4gh.py
--rw-r--r--   0        0        0      747 2024-04-01 22:06:40.809031 phc-ingestion-0.7.4/ingestion/caris/util/hla.py
--rw-r--r--   0        0        0      555 2024-04-01 22:06:40.809031 phc-ingestion-0.7.4/ingestion/caris/util/interpretation.py
--rw-r--r--   0        0        0     4976 2024-04-01 22:06:40.809031 phc-ingestion-0.7.4/ingestion/caris/util/json.py
--rw-r--r--   0        0        0    23579 2024-04-01 22:06:40.809031 phc-ingestion-0.7.4/ingestion/caris/util/metadata.py
--rw-r--r--   0        0        0     5022 2024-04-01 22:06:40.809031 phc-ingestion-0.7.4/ingestion/caris/util/structural.py
--rw-r--r--   0        0        0      482 2024-04-01 22:06:40.809031 phc-ingestion-0.7.4/ingestion/caris/util/tar.py
--rw-r--r--   0        0        0     1771 2024-04-01 22:06:40.809031 phc-ingestion-0.7.4/ingestion/caris/util/tsv.py
--rw-r--r--   0        0        0     3324 2024-04-01 22:06:40.809031 phc-ingestion-0.7.4/ingestion/caris/util/vcf.py
--rw-r--r--   0        0        0       49 2024-04-01 22:06:40.809031 phc-ingestion-0.7.4/ingestion/foundation/__init__.py
--rw-r--r--   0        0        0     3151 2024-04-01 22:06:40.809031 phc-ingestion-0.7.4/ingestion/foundation/process.py
--rw-r--r--   0        0        0        0 2024-04-01 22:06:40.809031 phc-ingestion-0.7.4/ingestion/foundation/util/__init__.py
--rw-r--r--   0        0        0     4215 2024-04-01 22:06:40.809031 phc-ingestion-0.7.4/ingestion/foundation/util/cnv.py
--rw-r--r--   0        0        0     5937 2024-04-01 22:06:40.809031 phc-ingestion-0.7.4/ingestion/foundation/util/fnv.py
--rw-r--r--   0        0        0    10987 2024-04-01 22:06:40.809031 phc-ingestion-0.7.4/ingestion/foundation/util/ga4gh.py
--rw-r--r--   0        0        0      405 2024-04-01 22:06:40.809031 phc-ingestion-0.7.4/ingestion/foundation/util/interpretation.py
--rw-r--r--   0        0        0     2163 2024-04-01 22:06:40.809031 phc-ingestion-0.7.4/ingestion/foundation/util/vcf_etl.py
--rw-r--r--   0        0        0        0 2024-04-01 22:06:40.809031 phc-ingestion-0.7.4/ingestion/generic/__init__.py
--rw-r--r--   0        0        0     1548 2024-04-01 22:06:40.809031 phc-ingestion-0.7.4/ingestion/generic/process.py
--rw-r--r--   0        0        0     2814 2024-04-01 22:06:40.809031 phc-ingestion-0.7.4/ingestion/generic/utils.py
--rw-r--r--   0        0        0       46 2024-04-01 22:06:40.809031 phc-ingestion-0.7.4/ingestion/nextgen/__init__.py
--rw-r--r--   0        0        0     3074 2024-04-01 22:06:40.809031 phc-ingestion-0.7.4/ingestion/nextgen/process.py
--rw-r--r--   0        0        0      297 2024-04-01 22:06:40.809031 phc-ingestion-0.7.4/ingestion/nextgen/util/interpretation.py
--rw-r--r--   0        0        0     2284 2024-04-01 22:06:40.809031 phc-ingestion-0.7.4/ingestion/nextgen/util/process_cnv.py
--rw-r--r--   0        0        0     8522 2024-04-01 22:06:40.809031 phc-ingestion-0.7.4/ingestion/nextgen/util/process_manifest.py
--rw-r--r--   0        0        0     5451 2024-04-01 22:06:40.809031 phc-ingestion-0.7.4/ingestion/nextgen/util/process_structural.py
--rw-r--r--   0        0        0     7341 2024-04-01 22:06:40.809031 phc-ingestion-0.7.4/ingestion/nextgen/util/process_vcf.py
--rw-r--r--   0        0        0       22 2024-04-01 22:06:40.809031 phc-ingestion-0.7.4/ingestion/nextgen/util/types.py
--rw-r--r--   0        0        0     2047 2024-04-01 22:06:40.809031 phc-ingestion-0.7.4/ingestion/nextgen/util/variant_table.py
--rw-r--r--   0        0        0   408290 2024-04-01 22:06:40.809031 phc-ingestion-0.7.4/ingestion/resources/GRCh37_map.csv.gz
--rw-r--r--   0        0        0   612373 2024-04-01 22:06:40.813031 phc-ingestion-0.7.4/ingestion/resources/GRCh38_map.csv.gz
--rw-r--r--   0        0        0        0 2024-04-01 22:06:40.813031 phc-ingestion-0.7.4/ingestion/shared_util/__init__.py
--rw-r--r--   0        0        0     1669 2024-04-01 22:06:40.813031 phc-ingestion-0.7.4/ingestion/shared_util/coords_to_genes.py
--rw-r--r--   0        0        0      876 2024-04-01 22:06:40.813031 phc-ingestion-0.7.4/ingestion/shared_util/gene_to_coords.py
--rw-r--r--   0        0        0       68 2024-04-01 22:06:40.813031 phc-ingestion-0.7.4/ingestion/shared_util/types.py
--rw-r--r--   0        0        0     5398 2024-04-01 22:06:40.813031 phc-ingestion-0.7.4/ingestion/vcf_standardization/Variant.py
--rw-r--r--   0        0        0        0 2024-04-01 22:06:40.813031 phc-ingestion-0.7.4/ingestion/vcf_standardization/__init__.py
--rw-r--r--   0        0        0     2289 2024-04-01 22:06:40.813031 phc-ingestion-0.7.4/ingestion/vcf_standardization/standardize.py
--rw-r--r--   0        0        0        0 2024-04-01 22:06:40.813031 phc-ingestion-0.7.4/ingestion/vcf_standardization/util/__init__.py
--rw-r--r--   0        0        0     1061 2024-04-01 22:06:40.813031 phc-ingestion-0.7.4/ingestion/vcf_standardization/util/af_helpers.py
--rw-r--r--   0        0        0      823 2024-04-01 22:06:40.813031 phc-ingestion-0.7.4/ingestion/vcf_standardization/util/dp_helpers.py
--rw-r--r--   0        0        0     2471 2024-04-01 22:06:40.813031 phc-ingestion-0.7.4/ingestion/vcf_standardization/util/read_write.py
--rw-r--r--   0        0        0     1009 2024-04-01 22:06:40.813031 phc-ingestion-0.7.4/pyproject.toml
--rw-r--r--   0        0        0      268 1970-01-01 00:00:00.000000 phc-ingestion-0.7.4/PKG-INFO
+-rw-r--r--   0        0        0       16 2024-04-07 13:28:56.008269 phc-ingestion-0.8.0/PYPI.md
+-rw-r--r--   0        0        0        0 2024-04-07 13:28:56.008269 phc-ingestion-0.8.0/ingestion/__init__.py
+-rw-r--r--   0        0        0       61 2024-04-07 13:28:56.008269 phc-ingestion-0.8.0/ingestion/caris/__init__.py
+-rw-r--r--   0        0        0     1257 2024-04-07 13:28:56.008269 phc-ingestion-0.8.0/ingestion/caris/process.py
+-rw-r--r--   0        0        0        0 2024-04-07 13:28:56.008269 phc-ingestion-0.8.0/ingestion/caris/util/__init__.py
+-rw-r--r--   0        0        0     4199 2024-04-07 13:28:56.008269 phc-ingestion-0.8.0/ingestion/caris/util/cnv.py
+-rw-r--r--   0        0        0     1640 2024-04-07 13:28:56.008269 phc-ingestion-0.8.0/ingestion/caris/util/detect_genome_ref.py
+-rw-r--r--   0        0        0      507 2024-04-07 13:28:56.008269 phc-ingestion-0.8.0/ingestion/caris/util/ga4gh.py
+-rw-r--r--   0        0        0      747 2024-04-07 13:28:56.008269 phc-ingestion-0.8.0/ingestion/caris/util/hla.py
+-rw-r--r--   0        0        0    12312 2024-04-07 13:28:56.008269 phc-ingestion-0.8.0/ingestion/caris/util/ihc.py
+-rw-r--r--   0        0        0      555 2024-04-07 13:28:56.008269 phc-ingestion-0.8.0/ingestion/caris/util/interpretation.py
+-rw-r--r--   0        0        0     4706 2024-04-07 13:28:56.008269 phc-ingestion-0.8.0/ingestion/caris/util/json.py
+-rw-r--r--   0        0        0     9497 2024-04-07 13:28:56.008269 phc-ingestion-0.8.0/ingestion/caris/util/metadata.py
+-rw-r--r--   0        0        0     2051 2024-04-07 13:28:56.008269 phc-ingestion-0.8.0/ingestion/caris/util/specimen_details.py
+-rw-r--r--   0        0        0     4363 2024-04-07 13:28:56.008269 phc-ingestion-0.8.0/ingestion/caris/util/structural.py
+-rw-r--r--   0        0        0      482 2024-04-07 13:28:56.008269 phc-ingestion-0.8.0/ingestion/caris/util/tar.py
+-rw-r--r--   0        0        0     1027 2024-04-07 13:28:56.008269 phc-ingestion-0.8.0/ingestion/caris/util/tmb.py
+-rw-r--r--   0        0        0     1595 2024-04-07 13:28:56.008269 phc-ingestion-0.8.0/ingestion/caris/util/tsv.py
+-rw-r--r--   0        0        0     3298 2024-04-07 13:28:56.008269 phc-ingestion-0.8.0/ingestion/caris/util/vcf.py
+-rw-r--r--   0        0        0       49 2024-04-07 13:28:56.008269 phc-ingestion-0.8.0/ingestion/foundation/__init__.py
+-rw-r--r--   0        0        0     3151 2024-04-07 13:28:56.008269 phc-ingestion-0.8.0/ingestion/foundation/process.py
+-rw-r--r--   0        0        0        0 2024-04-07 13:28:56.008269 phc-ingestion-0.8.0/ingestion/foundation/util/__init__.py
+-rw-r--r--   0        0        0     4215 2024-04-07 13:28:56.008269 phc-ingestion-0.8.0/ingestion/foundation/util/cnv.py
+-rw-r--r--   0        0        0     5937 2024-04-07 13:28:56.008269 phc-ingestion-0.8.0/ingestion/foundation/util/fnv.py
+-rw-r--r--   0        0        0    10987 2024-04-07 13:28:56.008269 phc-ingestion-0.8.0/ingestion/foundation/util/ga4gh.py
+-rw-r--r--   0        0        0      405 2024-04-07 13:28:56.008269 phc-ingestion-0.8.0/ingestion/foundation/util/interpretation.py
+-rw-r--r--   0        0        0     2163 2024-04-07 13:28:56.008269 phc-ingestion-0.8.0/ingestion/foundation/util/vcf_etl.py
+-rw-r--r--   0        0        0        0 2024-04-07 13:28:56.008269 phc-ingestion-0.8.0/ingestion/generic/__init__.py
+-rw-r--r--   0        0        0     1548 2024-04-07 13:28:56.008269 phc-ingestion-0.8.0/ingestion/generic/process.py
+-rw-r--r--   0        0        0     2814 2024-04-07 13:28:56.008269 phc-ingestion-0.8.0/ingestion/generic/utils.py
+-rw-r--r--   0        0        0       46 2024-04-07 13:28:56.008269 phc-ingestion-0.8.0/ingestion/nextgen/__init__.py
+-rw-r--r--   0        0        0     3074 2024-04-07 13:28:56.008269 phc-ingestion-0.8.0/ingestion/nextgen/process.py
+-rw-r--r--   0        0        0      297 2024-04-07 13:28:56.008269 phc-ingestion-0.8.0/ingestion/nextgen/util/interpretation.py
+-rw-r--r--   0        0        0     2284 2024-04-07 13:28:56.008269 phc-ingestion-0.8.0/ingestion/nextgen/util/process_cnv.py
+-rw-r--r--   0        0        0     8522 2024-04-07 13:28:56.008269 phc-ingestion-0.8.0/ingestion/nextgen/util/process_manifest.py
+-rw-r--r--   0        0        0     5451 2024-04-07 13:28:56.008269 phc-ingestion-0.8.0/ingestion/nextgen/util/process_structural.py
+-rw-r--r--   0        0        0     7341 2024-04-07 13:28:56.008269 phc-ingestion-0.8.0/ingestion/nextgen/util/process_vcf.py
+-rw-r--r--   0        0        0       22 2024-04-07 13:28:56.008269 phc-ingestion-0.8.0/ingestion/nextgen/util/types.py
+-rw-r--r--   0        0        0     2047 2024-04-07 13:28:56.008269 phc-ingestion-0.8.0/ingestion/nextgen/util/variant_table.py
+-rw-r--r--   0        0        0   408290 2024-04-07 13:28:56.008269 phc-ingestion-0.8.0/ingestion/resources/GRCh37_map.csv.gz
+-rw-r--r--   0        0        0   612373 2024-04-07 13:28:56.012269 phc-ingestion-0.8.0/ingestion/resources/GRCh38_map.csv.gz
+-rw-r--r--   0        0        0        0 2024-04-07 13:28:56.012269 phc-ingestion-0.8.0/ingestion/shared_util/__init__.py
+-rw-r--r--   0        0        0     1669 2024-04-07 13:28:56.012269 phc-ingestion-0.8.0/ingestion/shared_util/coords_to_genes.py
+-rw-r--r--   0        0        0      876 2024-04-07 13:28:56.012269 phc-ingestion-0.8.0/ingestion/shared_util/gene_to_coords.py
+-rw-r--r--   0        0        0       68 2024-04-07 13:28:56.012269 phc-ingestion-0.8.0/ingestion/shared_util/types.py
+-rw-r--r--   0        0        0     5398 2024-04-07 13:28:56.012269 phc-ingestion-0.8.0/ingestion/vcf_standardization/Variant.py
+-rw-r--r--   0        0        0        0 2024-04-07 13:28:56.012269 phc-ingestion-0.8.0/ingestion/vcf_standardization/__init__.py
+-rw-r--r--   0        0        0     2289 2024-04-07 13:28:56.012269 phc-ingestion-0.8.0/ingestion/vcf_standardization/standardize.py
+-rw-r--r--   0        0        0        0 2024-04-07 13:28:56.012269 phc-ingestion-0.8.0/ingestion/vcf_standardization/util/__init__.py
+-rw-r--r--   0        0        0     1061 2024-04-07 13:28:56.012269 phc-ingestion-0.8.0/ingestion/vcf_standardization/util/af_helpers.py
+-rw-r--r--   0        0        0      823 2024-04-07 13:28:56.012269 phc-ingestion-0.8.0/ingestion/vcf_standardization/util/dp_helpers.py
+-rw-r--r--   0        0        0     2471 2024-04-07 13:28:56.012269 phc-ingestion-0.8.0/ingestion/vcf_standardization/util/read_write.py
+-rw-r--r--   0        0        0     1010 2024-04-07 13:28:56.012269 phc-ingestion-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0      269 1970-01-01 00:00:00.000000 phc-ingestion-0.8.0/PKG-INFO
```

### Comparing `phc-ingestion-0.7.4/ingestion/caris/process.py` & `phc-ingestion-0.8.0/ingestion/caris/process.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,34 +2,21 @@
 
 from ingestion.caris.util.json import process_caris_json
 from ingestion.caris.util.vcf import process_caris_vcf
 from lifeomic_logging import scoped_logger
 
 
 def process_caris(infile, outpath, file_name, source_file_id):
-    ingest_status = {
-        "exome_performed": False,
-        "cnv_performed": False,
-        "ihc_performed": False,
-        "structural_performed": False,
-        "run_instructions": {
-            "som_vcf": False,
-            "germ_vcf": False,
-            "som_rna": False,
-            "som_structural": False,
-            "som_cnv": False,
-        },
-    }
 
     with scoped_logger(__name__) as log:
         os.makedirs(f"{outpath}", exist_ok=True)
         somatic_vcf_line_count = 0
         germline_vcf_line_count = 0
         result, germline_case_id, file_genome_references, json_data = process_caris_json(
-            infile, outpath, file_name, source_file_id, ingest_status, log
+            infile, outpath, file_name, source_file_id, log
         )
         if "somatic_vcf" in result:
             somatic_vcf_line_count = process_caris_vcf(
                 result["somatic_vcf"], json_data, outpath, file_name, log
             )
         if "germline_vcf" in result:
             germline_vcf_line_count = process_caris_vcf(
```

### Comparing `phc-ingestion-0.7.4/ingestion/caris/util/cnv.py` & `phc-ingestion-0.8.0/ingestion/caris/util/cnv.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,106 +1,100 @@
 from logging import Logger
 from ingestion.shared_util.gene_to_coords import gene_to_coords
 
 
-def extract_cnv(prefix, data, ingest_status, log: Logger):
+def extract_cnv(prefix, data, log: Logger):
     # Get all CNV calls into a csv
     caris_lo_keywords = {"intermediate": "gain", "amplified": "amplification", "deleted": "loss"}
-    if ingest_status["cnv_performed"]:
-        tests = []
-        for test in data["tests"]:
-            # We don't want to bring in "not detected" or wild type results
-            test_name = test["testName"]
-            if ("CNA" in test_name or "CND" in test_name) and "testResults" in test.keys():
-                test = test["testResults"]
-                if isinstance(test, dict):
-                    test = [test]
-                for cna in test:
-                    if "copyNumberAlteration" in cna.keys():
-                        results = cna["copyNumberAlteration"]
-                        if "result" in results.keys() and results["result_group"].lower() not in [
-                            "normal",
-                            "no result",
-                            "indeterminate",
-                            "wild type",
-                        ]:
-                            status = results["result"].lower()
-                            if status in caris_lo_keywords.keys():
-                                # We only accept 2 of their results and they have to match our PHC keywords to be searchable
-                                results["result"] = caris_lo_keywords[status]
-                                tests.append(results)
-                        elif (
-                            "Exome CNA Panel - Additional Genes" in test_name
-                            and "result" in results.keys()
-                            and "copyNumber" in results.keys()
-                        ):
-                            status = results["result"].lower()
-
-                            copy_number = 2
-                            if results["copyNumber"]:
-                                copy_number = float(results["copyNumber"])
-                                cn_status = ""
-                                # We only accept 2 of their results and they have to match our PHC keywords to be searchable
-                                if copy_number >= 4 and copy_number < 6:
-                                    cn_status = "gain"
-                                elif copy_number >= 6:
-                                    cn_status = "amplification"
-                                elif copy_number < 1.3:
-                                    cn_status = "loss"
-                                else:
-                                    continue
-                                results["result"] = cn_status
-                                tests.append(results)
+    tests = []
+    for test in data["tests"]:
+        # We don't want to bring in "not detected" or wild type results
+        test_name = test["testName"]
+        if ("CNA" in test_name or "CND" in test_name) and "testResults" in test.keys():
+            test = test["testResults"]
+            if isinstance(test, dict):
+                test = [test]
+            for cna in test:
+                if "copyNumberAlteration" in cna.keys():
+                    results = cna["copyNumberAlteration"]
+                    if "result" in results.keys() and results["result_group"].lower() not in [
+                        "normal",
+                        "no result",
+                        "indeterminate",
+                        "wild type",
+                    ]:
+                        status = results["result"].lower()
+                        if status in caris_lo_keywords.keys():
+                            # We only accept 2 of their results and they have to match our PHC keywords to be searchable
+                            results["result"] = caris_lo_keywords[status]
+                            tests.append(results)
+                    elif (
+                        "Exome CNA Panel - Additional Genes" in test_name
+                        and "result" in results.keys()
+                        and "copyNumber" in results.keys()
+                    ):
+                        status = results["result"].lower()
+
+                        copy_number = 2.0
+                        if results["copyNumber"]:
+                            copy_number = float(results["copyNumber"])
+                            cn_status = ""
+                            # We only accept 2 of their results and they have to match our PHC keywords to be searchable
+                            if copy_number >= 4 and copy_number < 6:
+                                cn_status = "gain"
+                            elif copy_number >= 6:
+                                cn_status = "amplification"
+                            elif copy_number < 1.3:
+                                cn_status = "loss"
+                            else:
+                                continue
+                            results["result"] = cn_status
+                            tests.append(results)
+
+    if not tests:
+        return None
+
+    # Save our results
+    with open(f"{prefix}.copynumber.csv", "w") as f:
+        f.write(
+            "sample_id,gene,copy_number,status,attributes,chromosome,start_position,end_position,interpretation\n"
+        )
+        for alt in tests:
+            if "genomicCoordinates" in alt.keys():
+                chrom = alt["genomicCoordinates"].split(":")[1]
+                coords = alt["genomicCoordinates"].split(":")[2].split("-")
+            else:
+                chrom, coords = gene_to_coords("GRCh37", alt["gene"])
+
+            # Get pathogenic result
+            if alt["result_group"].lower() in ["high", "mutated"]:
+                interpretation = "Pathogenic"
+            elif alt["result_group"].lower() in ["intermediate", "no result"]:
+                interpretation = "Uncertain significance"
+            else:
+                interpretation = "other"
 
-        if not tests:
-            return None
-
-        # Save our results
-        with open(f"{prefix}.copynumber.csv", "w") as f:
             f.write(
-                "sample_id,gene,copy_number,status,attributes,chromosome,start_position,end_position,interpretation\n"
+                ",".join(
+                    [
+                        prefix,
+                        alt["gene"],
+                        str(alt["copyNumber"]),
+                        alt["result"],
+                        "{}",
+                        chrom,
+                        coords[0],
+                        coords[1],
+                        f"{interpretation}\n",
+                    ]
+                ),
             )
-            for alt in tests:
-                if "genomicCoordinates" in alt.keys():
-                    chrom = alt["genomicCoordinates"].split(":")[1]
-                    coords = alt["genomicCoordinates"].split(":")[2].split("-")
-                else:
-                    chrom, coords = gene_to_coords("GRCh37", alt["gene"])
-
-                # Get pathogenic result
-                if alt["result_group"].lower() in ["high", "mutated"]:
-                    interpretation = "Pathogenic"
-                elif alt["result_group"].lower() in ["intermediate", "no result"]:
-                    interpretation = "Uncertain significance"
-                else:
-                    interpretation = "other"
-
-                f.write(
-                    ",".join(
-                        [
-                            prefix,
-                            alt["gene"],
-                            str(alt["copyNumber"]),
-                            alt["result"],
-                            "{}",
-                            chrom,
-                            coords[0],
-                            coords[1],
-                            f"{interpretation}\n",
-                        ]
-                    ),
-                )
-
-        ingest_status["run_instructions"]["som_cnv"] = True
-
-        # Hard-code genome reference for Caris CNVs only
-        genome_reference = "GRCh37"
-
-        return {
-            "fileName": f".lifeomic/caris/{prefix}/{prefix}.copynumber.csv",
-            "sequenceType": "somatic",
-            "type": "copyNumberVariant",
-            "reference": genome_reference,
-        }
 
-    # We can return none here because there will be no CNV file.
-    return None
+    # Hard-code genome reference for Caris CNVs only
+    genome_reference = "GRCh37"
+
+    return {
+        "fileName": f".lifeomic/caris/{prefix}/{prefix}.copynumber.csv",
+        "sequenceType": "somatic",
+        "type": "copyNumberVariant",
+        "reference": genome_reference,
+    }
```

### Comparing `phc-ingestion-0.7.4/ingestion/caris/util/detect_genome_ref.py` & `phc-ingestion-0.8.0/ingestion/caris/util/detect_genome_ref.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.7.4/ingestion/caris/util/hla.py` & `phc-ingestion-0.8.0/ingestion/caris/util/hla.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.7.4/ingestion/caris/util/interpretation.py` & `phc-ingestion-0.8.0/ingestion/caris/util/interpretation.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.7.4/ingestion/caris/util/json.py` & `phc-ingestion-0.8.0/ingestion/caris/util/json.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,84 +22,77 @@
     if not multiple_tsv or "Transformed" in file:
         return {
             "tsv": file,
         }
     return {}
 
 
-def process_caris_json(
-    infile: str, outpath: str, file_name: str, source_file_id: str, ingest_status: dict, log: Logger
-):
+def process_caris_json(infile: str, outpath: str, file_name: str, source_file_id: str, log: Logger):
     # Unpack tarball and go into the new directory
     unpack(infile, outpath)
     os.chdir(outpath)
-    # If we do this we need to make sure we communicate it well.
-    #  shutil.move(args.input, f'{outpath}/{os.path.basename(args.input)}')
+
     file_list = glob.glob("*")
     files: dict[str, str] = {}
 
     # if file_list has more than one file that starts with DNA_ then we need to throw an error
     if len([file for file in file_list if file.startswith("DNA_")]) > 1:
         raise Exception(f"More than one DNA file found in {file_name}\n")
 
     for file in file_list:
         extension = ".".join(file.split(".")[1:])
-        if file.lower().startswith("germline"):
+        if file.lower().startswith("germline") or file.startswith("gDNA"):
             files["germline.vcf"] = file
         elif file.endswith("vcf") and "germline" not in file:
             files["somatic.vcf"] = file
         elif file.endswith("tsv"):
             files.update(handle_tsv(file, file_list))
         else:
             files[extension] = file
 
     log.info(f"Files in tarball input: {file_list}")
 
     json_file = files["json"]
 
-    f = open(json_file, "rb")
-    all_data = json.load(f)
-    data = all_data
-    if "root" in all_data.keys():
-        data = all_data["root"]
-    f.close()
+    with open(json_file, "rb") as f:
+        data = json.load(f)
+    if "root" in data:
+        data = data["root"]
 
     somatic_filename = None
     germline_filename = None
     germline_case_id = None
 
     # Sometimes they don't come in gzipped
     for key in files.keys():
         if "somatic.vcf" in key:
             somatic_filename = files["somatic.vcf"].replace(".vcf", ".somatic.vcf") + ".gz"
             with open(files["somatic.vcf"], "rb") as f_in:
                 with gzip.open(somatic_filename, "wb") as f_out:
                     shutil.copyfileobj(f_in, f_out)
-            ingest_status["run_instructions"]["som_vcf"] = True
         if "germline.vcf" in key:
             germline_filename = (
                 files["germline.vcf"].replace("Germline_", "").replace(".vcf", ".germline.vcf")
                 + ".gz"
             )
             with open(files["germline.vcf"], "rb") as f_in:
                 with gzip.open(germline_filename, "wb") as f_out:
                     shutil.copyfileobj(f_in, f_out)
-            ingest_status["run_instructions"]["germ_vcf"] = True
-            germline_case_id = files["germline.vcf"].replace("Germline_", "")[
-                0:CARIS_CASE_ID_LENGTH
-            ]
-    if "tsv" in files.keys():
-        ingest_status["run_instructions"]["som_rna"] = True
+            # Liquid cases don't start with `Germline_` and follow a different pattern for germline
+            if "germline" in files["germline.vcf"].lower():
+                germline_case_id = files["germline.vcf"].replace("Germline_", "")[
+                    0:CARIS_CASE_ID_LENGTH
+                ]
 
     # Get patient
-    metadata = extract_metadata(data, file_name, files, source_file_id, ingest_status, log)
-    structural_results = extract_structural(file_name, data, ingest_status, log)
-    cnv_results = extract_cnv(file_name, data, ingest_status, log)
-    rgel_results = convert_tsv_to_rgel(file_name, files, ingest_status, log)
-    vcf_results = extract_sv(file_name, ingest_status)
+    metadata = extract_metadata(data, file_name, files, source_file_id, log)
+    structural_results = extract_structural(file_name, data, log)
+    cnv_results = extract_cnv(file_name, data, log)
+    rgel_results = convert_tsv_to_rgel(file_name, files, log)
+    vcf_results = extract_sv(file_name, bool(somatic_filename), bool(germline_filename))
 
     # We might not have any of these files but we need an empty json object here.
     file_genome_references = {}
     metadata["files"] = []
     if structural_results:
         metadata["files"].append(structural_results)
         file_genome_references["structural_genome_reference"] = structural_results["reference"]
@@ -111,15 +104,15 @@
         file_genome_references["cnv_genome_reference"] = cnv_results["reference"]
     if vcf_results:
         metadata["files"] = metadata["files"] + vcf_results
         for vcf in vcf_results:
             seq_type = vcf.get("sequenceType")
             file_genome_references[f"{seq_type}_genome_reference"] = vcf["reference"]
 
-    create_yaml(metadata, file_name, ingest_status)
+    create_yaml(metadata, file_name)
 
     # Return VCF files for immediate processing, and JSON data for adding vendsig
     result = {}
 
     if somatic_filename is not None:
         result["somatic_vcf"] = f"{outpath}/{somatic_filename}"
     if germline_filename is not None:
```

### Comparing `phc-ingestion-0.7.4/ingestion/caris/util/structural.py` & `phc-ingestion-0.8.0/ingestion/caris/util/structural.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,123 +1,113 @@
 import pandas as pd
 from logging import Logger
 
 from ingestion.caris.util.interpretation import calculate_interpretation
 from ingestion.caris.util.detect_genome_ref import detect_caris_gr
 
 
-def extract_structural(prefix, data, ingest_status, log: Logger):
+def extract_structural(prefix, data, log: Logger):
     log.info("Extracting fusion variants from json")
-    if ingest_status["structural_performed"]:
-        tests = []
-        for test in data["tests"]:
-            if (
-                test["platformTechnology"] in ["Transcriptome", "Hybrid Transcriptome"]
-                and "testResults" in test.keys()
-            ):
-                for test_result in test["testResults"]:
-                    this_result = test_result["translocation"]
-
-                    # Result_group values:
-                    #     - Mutated
-                    #     - Normal
-                    #     - No Result
-                    #
-                    # We only keep Mutated. Possible results:
-                    #     - Fusion Detected
-                    #     - Likely Pathogenic Fusion
-                    #     - Likely Pathogenic Isoform
-                    #     - Pathogenic Fusion
-                    if this_result["result_group"].lower() not in [
-                        "normal",
-                        "no result",
-                        "indeterminate",
-                        "wild type",
-                    ]:
-                        tests.append(this_result)
-        if not tests:
-            return None
-
-        df = pd.DataFrame(tests)
-
-        plus_delim = ":+/"
-        minus_delim = ":-/"
-
-        def split_coords(x):
-            return x.strip(":+").replace("+/", "").strip(":-").replace("-/", "")
-
-        df["genomicBreakpoint"] = df["genomicBreakpoint"].apply(split_coords)
-
-        df[["chromosome1", "start_position1", "chromosome2", "start_position2"]] = df[
-            "genomicBreakpoint"
-        ].str.split(":", expand=True)
-
-        # Structural Variant CSV fields found in documentation here:
-        # https://docs.us.lifeomic.com/user-guides/omics/data-processing/#structural-variants
-        df["sample_id"] = prefix  # required str
-        # df['gene1']                                 #already exists from JSON
-        # df['gene2']                                 #already exists from JSON
-        df[
-            "effect"
-        ] = "Fusion"  # "Fusion" if "Fusion" in df['result'] else ""                   #optional str
-        # df['chromosome1']     = ""#firstBreak[0]#""                   #optional str
-        # df['start_position1'] = ""#firstBreak[1]#""                   #optional str
-        df["end_position1"] = df["start_position1"]  # optional str
-        # df['chromosome2']     = ""                   #optional str
-        # df['start_position2'] = ""                   #optional str
-        df["end_position2"] = df["start_position2"]  # optional str
-        # df['interpretation']                        #already exists from JSON
-        df["sequence_type"] = df["genomicSource"]  # optional str
-
-        # Fusions are no longer described in depth from what I can see in the new json files...
-        df["in_frame"] = "Unknown"
-        # To explain below: https://stackoverflow.com/a/11531402/14708230
-        df.loc[df["interpretation"].str.contains("in-frame"), "in_frame"] = "Yes"
-
-        # Utilize "result" as the interpretation, mapped to approved values
-        # (if result_group is 'unclassifiedVD' we use that, because a result will not be present)
-        mapped_interpretation_list = []
-        for entry in zip(list(df.result_group), list(df.result)):
-            if entry[0].lower() == "unclassifiedvd":
-                mapped_interpretation_list.append("Uncertain significance")
-            else:
-                mapped_interpretation_list.append(calculate_interpretation(entry[1].lower(), log))
-
-        df["interpretation"] = mapped_interpretation_list
-
-        df["attributes"] = "{}"  # optional str containing JSON
-
-        # Select columns for output
-        df_out = df[
-            [
-                "sample_id",
-                "gene1",
-                "gene2",
-                "effect",
-                "chromosome1",
-                "start_position1",
-                "end_position1",
-                "chromosome2",
-                "start_position2",
-                "end_position2",
-                "interpretation",
-                "sequence_type",
-                "in_frame",
-                "attributes",
-            ]
+    tests = []
+    for test in data["tests"]:
+        if (
+            test["platformTechnology"] in ["Transcriptome", "Hybrid Transcriptome"]
+            and "testResults" in test.keys()
+        ):
+            for test_result in test["testResults"]:
+                this_result = test_result["translocation"]
+
+                # Result_group values:
+                #     - Mutated
+                #     - Normal
+                #     - No Result
+                #
+                # We only keep Mutated. Possible results:
+                #     - Fusion Detected
+                #     - Likely Pathogenic Fusion
+                #     - Likely Pathogenic Isoform
+                #     - Pathogenic Fusion
+                if this_result["result_group"].lower() not in [
+                    "normal",
+                    "no result",
+                    "indeterminate",
+                    "wild type",
+                ]:
+                    tests.append(this_result)
+    if not tests:
+        return None
+
+    df = pd.DataFrame(tests)
+
+    def split_coords(x):
+        return x.strip(":+").replace("+/", "").strip(":-").replace("-/", "")
+
+    df["genomicBreakpoint"] = df["genomicBreakpoint"].apply(split_coords)
+
+    df[["chromosome1", "start_position1", "chromosome2", "start_position2"]] = df[
+        "genomicBreakpoint"
+    ].str.split(":", expand=True)
+
+    # Structural Variant CSV fields found in documentation here:
+    # https://docs.us.lifeomic.com/user-guides/omics/data-processing/#structural-variants
+    df["sample_id"] = prefix  # required str
+    # df['gene1']                                 #already exists from JSON
+    # df['gene2']                                 #already exists from JSON
+    df["effect"] = (
+        "Fusion"  # "Fusion" if "Fusion" in df['result'] else ""                   #optional str
+    )
+    # df['chromosome1']     = ""#firstBreak[0]#""                   #optional str
+    # df['start_position1'] = ""#firstBreak[1]#""                   #optional str
+    df["end_position1"] = df["start_position1"]  # optional str
+    # df['chromosome2']     = ""                   #optional str
+    # df['start_position2'] = ""                   #optional str
+    df["end_position2"] = df["start_position2"]  # optional str
+    # df['interpretation']                        #already exists from JSON
+    df["sequence_type"] = df["genomicSource"]  # optional str
+
+    # Fusions are no longer described in depth from what I can see in the new json files...
+    df["in_frame"] = "Unknown"
+    # To explain below: https://stackoverflow.com/a/11531402/14708230
+    df.loc[df["interpretation"].str.contains("in-frame"), "in_frame"] = "Yes"
+
+    # Utilize "result" as the interpretation, mapped to approved values
+    # (if result_group is 'unclassifiedVD' we use that, because a result will not be present)
+    mapped_interpretation_list = []
+    for entry in zip(list(df.result_group), list(df.result)):
+        if entry[0].lower() == "unclassifiedvd":
+            mapped_interpretation_list.append("Uncertain significance")
+        else:
+            mapped_interpretation_list.append(calculate_interpretation(entry[1].lower(), log))
+
+    df["interpretation"] = mapped_interpretation_list
+
+    df["attributes"] = "{}"  # optional str containing JSON
+
+    # Select columns for output
+    df_out = df[
+        [
+            "sample_id",
+            "gene1",
+            "gene2",
+            "effect",
+            "chromosome1",
+            "start_position1",
+            "end_position1",
+            "chromosome2",
+            "start_position2",
+            "end_position2",
+            "interpretation",
+            "sequence_type",
+            "in_frame",
+            "attributes",
         ]
+    ]
 
-        ingest_status["run_instructions"]["som_structural"] = True
-        df_out.to_csv(f"{prefix}.structural.csv", na_rep="N/A", index=False)
+    df_out.to_csv(f"{prefix}.structural.csv", na_rep="N/A", index=False)
 
-        genome_reference = detect_caris_gr(tests, "structural", log)
-        return {
-            "fileName": f".lifeomic/caris/{prefix}/{prefix}.structural.csv",
-            "sequenceType": "somatic",
-            "type": "structuralVariant",
-            "reference": genome_reference,
-        }
-
-    ingest_status["run_instructions"]["som_structural"] = False
-
-    # Won't be in the manifest
-    return None
+    genome_reference = detect_caris_gr(tests, "structural", log)
+    return {
+        "fileName": f".lifeomic/caris/{prefix}/{prefix}.structural.csv",
+        "sequenceType": "somatic",
+        "type": "structuralVariant",
+        "reference": genome_reference,
+    }
```

### Comparing `phc-ingestion-0.7.4/ingestion/caris/util/tsv.py` & `phc-ingestion-0.8.0/ingestion/caris/util/tsv.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,54 +1,55 @@
 import pandas as pd
-import gzip
 
 from logging import Logger
 from ingestion.caris.util.detect_genome_ref import detect_caris_gr
 
+
 # Take the caris RNA information from the provided tsv for ingestion and input to TSO/pcann
 # We are not guaranteed rnaseq results FYI
-def convert_tsv_to_rgel(prefix, files, ingest_status, log: Logger):
-    if ingest_status["run_instructions"]["som_rna"]:
-        tsv_file = files["tsv"]
-        log.info(f"RNA TPM file found. Converting to RGEL: {tsv_file}")
-
-        df = pd.read_table(tsv_file, comment="#", header=None)
-        df.rename(columns={0: "gene_id", 1: "expression"}, inplace=True)
-
-        df["sample_id"] = prefix
-        df["gene_name"] = df["gene_id"]
-        df["raw_count"] = ""
-        df["attributes"] = "{}"
-        df["is_normalized"] = "True"
-        df["expression_unit"] = "tpm"
-
-        df.drop_duplicates(inplace=True)
-        # Select columns for output
-        df_out = df[
-            [
-                "sample_id",
-                "gene_id",
-                "gene_name",
-                "expression",
-                "raw_count",
-                "attributes",
-                "is_normalized",
-                "expression_unit",
-            ]
+def convert_tsv_to_rgel(prefix, files, log: Logger):
+    if not "tsv" in files:
+        return None
+    tsv_file = files["tsv"]
+    log.info(f"RNA TPM file found. Converting to RGEL: {tsv_file}")
+
+    df = pd.read_table(tsv_file, comment="#", header=None)
+    df.rename(columns={0: "gene_id", 1: "expression"}, inplace=True)
+
+    df["sample_id"] = prefix
+    df["gene_name"] = df["gene_id"]
+    df["raw_count"] = ""
+    df["attributes"] = "{}"
+    df["is_normalized"] = "True"
+    df["expression_unit"] = "tpm"
+
+    df.drop_duplicates(inplace=True)
+    # Select columns for output
+    df_out = df[
+        [
+            "sample_id",
+            "gene_id",
+            "gene_name",
+            "expression",
+            "raw_count",
+            "attributes",
+            "is_normalized",
+            "expression_unit",
         ]
+    ]
 
-        df_out.to_csv(f"{prefix}.expression.rgel.gz", compression="gzip", na_rep="", index=False)
+    df_out.to_csv(f"{prefix}.expression.rgel.gz", compression="gzip", na_rep="", index=False)
 
-        headers = []
-        with open(tsv_file) as f:
-            for line in f.readlines()[:10]:
-                headers.append(line.strip())
-        genome_reference = detect_caris_gr(headers, "expression", log)
-
-        return {
-            "fileName": f".lifeomic/caris/{prefix}/{prefix}.expression.rgel.gz",
-            "sequenceType": "somatic",
-            "type": "expression",
-            "reference": genome_reference,
-        }
+    headers = []
+    with open(tsv_file) as f:
+        for line in f.readlines()[:10]:
+            headers.append(line.strip())
+    genome_reference = detect_caris_gr(headers, "expression", log)
+
+    return {
+        "fileName": f".lifeomic/caris/{prefix}/{prefix}.expression.rgel.gz",
+        "sequenceType": "somatic",
+        "type": "expression",
+        "reference": genome_reference,
+    }
 
     return None
```

### Comparing `phc-ingestion-0.7.4/ingestion/caris/util/vcf.py` & `phc-ingestion-0.8.0/ingestion/caris/util/vcf.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,31 +9,31 @@
 
 from logging import Logger
 
 from ingestion.vcf_standardization.standardize import standardize_vcf
 
 
 # This is done in next step, we are just adding to yaml
-def extract_sv(prefix, ingest_status):
+def extract_sv(prefix, include_somatic: bool, include_germline: bool):
     vcfs = []
 
     # Hard-code genome reference for Caris VCFs
     genome_reference = "GRCh38"
 
-    if ingest_status["run_instructions"]["som_vcf"]:
+    if include_somatic:
         vcfs.append(
             {
                 "fileName": f".lifeomic/caris/{prefix}/{prefix}.modified.somatic.nrm.filtered.vcf.gz",
                 "sequenceType": "somatic",
                 "type": "shortVariant",
                 "reference": genome_reference,
             }
         )
 
-    if ingest_status["run_instructions"]["germ_vcf"]:
+    if include_germline:
         vcfs.append(
             {
                 "fileName": f".lifeomic/caris/{prefix}/{prefix}.modified.germline.nrm.filtered.vcf.gz",
                 "sequenceType": "germline",
                 "type": "shortVariant",
                 "reference": genome_reference,
             }
```

### Comparing `phc-ingestion-0.7.4/ingestion/foundation/process.py` & `phc-ingestion-0.8.0/ingestion/foundation/process.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.7.4/ingestion/foundation/util/cnv.py` & `phc-ingestion-0.8.0/ingestion/foundation/util/cnv.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.7.4/ingestion/foundation/util/fnv.py` & `phc-ingestion-0.8.0/ingestion/foundation/util/fnv.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.7.4/ingestion/foundation/util/ga4gh.py` & `phc-ingestion-0.8.0/ingestion/foundation/util/ga4gh.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.7.4/ingestion/foundation/util/vcf_etl.py` & `phc-ingestion-0.8.0/ingestion/foundation/util/vcf_etl.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.7.4/ingestion/generic/process.py` & `phc-ingestion-0.8.0/ingestion/generic/process.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.7.4/ingestion/generic/utils.py` & `phc-ingestion-0.8.0/ingestion/generic/utils.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.7.4/ingestion/nextgen/process.py` & `phc-ingestion-0.8.0/ingestion/nextgen/process.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.7.4/ingestion/nextgen/util/process_cnv.py` & `phc-ingestion-0.8.0/ingestion/nextgen/util/process_cnv.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.7.4/ingestion/nextgen/util/process_manifest.py` & `phc-ingestion-0.8.0/ingestion/nextgen/util/process_manifest.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.7.4/ingestion/nextgen/util/process_structural.py` & `phc-ingestion-0.8.0/ingestion/nextgen/util/process_structural.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.7.4/ingestion/nextgen/util/process_vcf.py` & `phc-ingestion-0.8.0/ingestion/nextgen/util/process_vcf.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.7.4/ingestion/nextgen/util/variant_table.py` & `phc-ingestion-0.8.0/ingestion/nextgen/util/variant_table.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.7.4/ingestion/resources/GRCh37_map.csv.gz` & `phc-ingestion-0.8.0/ingestion/resources/GRCh37_map.csv.gz`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.7.4/ingestion/resources/GRCh38_map.csv.gz` & `phc-ingestion-0.8.0/ingestion/resources/GRCh38_map.csv.gz`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.7.4/ingestion/shared_util/coords_to_genes.py` & `phc-ingestion-0.8.0/ingestion/shared_util/coords_to_genes.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.7.4/ingestion/shared_util/gene_to_coords.py` & `phc-ingestion-0.8.0/ingestion/shared_util/gene_to_coords.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.7.4/ingestion/vcf_standardization/Variant.py` & `phc-ingestion-0.8.0/ingestion/vcf_standardization/Variant.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.7.4/ingestion/vcf_standardization/standardize.py` & `phc-ingestion-0.8.0/ingestion/vcf_standardization/standardize.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.7.4/ingestion/vcf_standardization/util/af_helpers.py` & `phc-ingestion-0.8.0/ingestion/vcf_standardization/util/af_helpers.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.7.4/ingestion/vcf_standardization/util/dp_helpers.py` & `phc-ingestion-0.8.0/ingestion/vcf_standardization/util/dp_helpers.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.7.4/ingestion/vcf_standardization/util/read_write.py` & `phc-ingestion-0.8.0/ingestion/vcf_standardization/util/read_write.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.7.4/pyproject.toml` & `phc-ingestion-0.8.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,49 +1,49 @@
 [project]
 name = "phc-ingestion"
-version = "0.7.4"
+version = "0.8.0"
 description = "Functions for LifeOmic PHC genomic ingestions"
 authors = [
     { name = "LifeOmic Development", email = "development@lifeomic.com" },
 ]
 dependencies = [
     "lifeomic-logging>=0.3.2,<0.4.0",
     "xmltodict==0.13.0",
     "natsort==7.1.1",
     "ruamel.yaml==0.17.21",
     "pandas>=1.5.0,<1.6.0",
     "jsonschema>=4.16.0,<5.0.0",
     "schema>=0.7.5",
     "packaging>=23.1",
 ]
-requires-python = ">=3.9"
+requires-python = ">=3.10"
 readme = "PYPI.md"
 
 [project.license]
 text = "MIT"
 
+[build-system]
+requires = [
+    "pdm-pep517>=0.12.0",
+]
+build-backend = "pdm.pep517.api"
+
+[tool.black]
+line-length = 100
+
 [tool.pdm.dev-dependencies]
 dev = [
-    "black==22.3.0",
+    "black==24.3.0",
     "pytest==7.1.2",
     "pytest-cov==2.10.1",
     "coverage==6.4.1",
 ]
 
 [tool.pdm.build]
 excludes = [
     "tests/",
 ]
 
 [tool.pdm.scripts]
 test = "python3 -m pytest -v --cov-report term-missing --cov=ingestion --log-level=INFO tests/"
 lint = "black --check tests/ ingestion/"
 lint-fix = "black tests/ ingestion/"
-
-[tool.black]
-line-length = 100
-
-[build-system]
-requires = [
-    "pdm-pep517>=0.12.0",
-]
-build-backend = "pdm.pep517.api"
```

