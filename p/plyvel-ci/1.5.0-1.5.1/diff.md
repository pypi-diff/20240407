# Comparing `tmp/plyvel-ci-1.5.0.tar.gz` & `tmp/plyvel_ci-1.5.1-cp39-cp39-macosx_10_9_universal2.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plyvel-ci-1.5.0.tar", last modified: Mon Apr  3 06:39:37 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

