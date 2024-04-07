# Comparing `tmp/tui_dsmt-202404071539.tar.gz` & `tmp/tui_dsmt-202404071540-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tui_dsmt-202404071539.tar", last modified: Sun Apr  7 15:39:57 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

