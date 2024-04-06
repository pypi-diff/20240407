# Comparing `tmp/pymssql-2.2.9.tar.gz` & `tmp/pymssql-2.3.0-cp36-cp36m-macosx_10_14_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymssql-2.2.9.tar", last modified: Sat Oct 14 04:24:59 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

