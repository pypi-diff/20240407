# Comparing `tmp/gdmath-1.5.1.tar.gz` & `tmp/gdmath-1.5.2-cp310-cp310-musllinux_1_1_i686.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gdmath-1.5.1.tar", last modified: Sat Apr  6 07:14:06 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

