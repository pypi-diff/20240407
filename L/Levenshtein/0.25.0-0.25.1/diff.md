# Comparing `tmp/Levenshtein-0.25.0.tar.gz` & `tmp/Levenshtein-0.25.1-cp312-cp312-musllinux_1_1_ppc64le.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Levenshtein-0.25.0.tar", last modified: Sun Feb 11 16:44:02 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

