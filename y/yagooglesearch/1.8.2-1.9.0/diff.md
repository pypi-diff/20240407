# Comparing `tmp/yagooglesearch-1.8.2.tar.gz` & `tmp/yagooglesearch-1.9.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yagooglesearch-1.8.2.tar", last modified: Mon Dec 11 13:43:40 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

