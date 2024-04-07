# Comparing `tmp/swiftest-2024.3.4.tar.gz` & `tmp/swiftest-2024.4.0-cp312-cp312-macosx_12_0_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swiftest-2024.3.4.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

