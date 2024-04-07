# Comparing `tmp/hex_renderer_py-0.1.1.tar.gz` & `tmp/hex_renderer_py-0.1.2-cp38-none-win32.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

