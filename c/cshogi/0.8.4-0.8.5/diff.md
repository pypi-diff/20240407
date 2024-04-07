# Comparing `tmp/cshogi-0.8.4.tar.gz` & `tmp/cshogi-0.8.5-cp39-cp39-win_amd64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cshogi-0.8.4.tar", last modified: Wed Feb 14 05:09:46 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

