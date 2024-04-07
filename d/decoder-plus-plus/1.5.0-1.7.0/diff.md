# Comparing `tmp/decoder-plus-plus-1.5.0.tar.gz` & `tmp/decoder-plus-plus-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/decoder-plus-plus-1.5.0.tar", last modified: Thu Sep 15 17:57:59 2022, max compression
+gzip compressed data, was "decoder-plus-plus-1.7.0.tar", last modified: Sun Apr  7 11:36:23 2024, max compression
```

## Comparing `decoder-plus-plus-1.5.0.tar` & `decoder-plus-plus-1.7.0.tar`

### file list

```diff
@@ -1,219 +1,310 @@
-drwxrwxr-x   0 tengel    (1000) tengel    (1000)        0 2022-09-15 17:57:59.330219 decoder-plus-plus-1.5.0/
--rw-rw-r--   0 tengel    (1000) tengel    (1000)    35147 2021-12-26 21:21:06.000000 decoder-plus-plus-1.5.0/LICENSE
--rw-rw-r--   0 tengel    (1000) tengel    (1000)       43 2021-12-26 21:21:06.000000 decoder-plus-plus-1.5.0/MANIFEST.in
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     7640 2022-09-15 17:57:59.330219 decoder-plus-plus-1.5.0/PKG-INFO
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     7093 2022-09-15 16:47:57.000000 decoder-plus-plus-1.5.0/README.md
-drwxrwxr-x   0 tengel    (1000) tengel    (1000)        0 2022-09-15 17:57:59.278219 decoder-plus-plus-1.5.0/data/
--rwxrwxr-x   0 tengel    (1000) tengel    (1000)      116 2021-12-26 21:21:06.000000 decoder-plus-plus-1.5.0/data/dpp.desktop
--rw-rw-r--   0 tengel    (1000) tengel    (1000)    10621 2021-12-26 21:21:06.000000 decoder-plus-plus-1.5.0/data/dpp.png
-drwxrwxr-x   0 tengel    (1000) tengel    (1000)        0 2022-09-15 17:57:59.278219 decoder-plus-plus-1.5.0/decoder_plus_plus.egg-info/
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     7640 2022-09-15 17:57:59.000000 decoder-plus-plus-1.5.0/decoder_plus_plus.egg-info/PKG-INFO
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     5981 2022-09-15 17:57:59.000000 decoder-plus-plus-1.5.0/decoder_plus_plus.egg-info/SOURCES.txt
--rw-rw-r--   0 tengel    (1000) tengel    (1000)        1 2022-09-15 17:57:59.000000 decoder-plus-plus-1.5.0/decoder_plus_plus.egg-info/dependency_links.txt
--rw-rw-r--   0 tengel    (1000) tengel    (1000)       40 2022-09-15 17:57:59.000000 decoder-plus-plus-1.5.0/decoder_plus_plus.egg-info/entry_points.txt
--rw-rw-r--   0 tengel    (1000) tengel    (1000)      350 2022-09-15 17:57:59.000000 decoder-plus-plus-1.5.0/decoder_plus_plus.egg-info/requires.txt
--rw-rw-r--   0 tengel    (1000) tengel    (1000)        4 2022-09-15 17:57:59.000000 decoder-plus-plus-1.5.0/decoder_plus_plus.egg-info/top_level.txt
-drwxrwxr-x   0 tengel    (1000) tengel    (1000)        0 2022-09-15 17:57:59.278219 decoder-plus-plus-1.5.0/dpp/
--rw-rw-r--   0 tengel    (1000) tengel    (1000)      850 2022-09-14 06:47:39.000000 decoder-plus-plus-1.5.0/dpp/__init__.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)      239 2021-12-26 21:21:06.000000 decoder-plus-plus-1.5.0/dpp/__main__.py
-drwxrwxr-x   0 tengel    (1000) tengel    (1000)        0 2022-09-15 17:57:59.282219 decoder-plus-plus-1.5.0/dpp/core/
--rw-rw-r--   0 tengel    (1000) tengel    (1000)      915 2021-12-26 21:21:06.000000 decoder-plus-plus-1.5.0/dpp/core/__init__.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     2353 2022-09-12 19:05:02.000000 decoder-plus-plus-1.5.0/dpp/core/argparse.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     2871 2022-09-12 21:57:24.000000 decoder-plus-plus-1.5.0/dpp/core/assertions.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     3279 2022-08-17 05:09:19.000000 decoder-plus-plus-1.5.0/dpp/core/config.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)    10219 2022-09-13 15:11:32.000000 decoder-plus-plus-1.5.0/dpp/core/context.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     2328 2022-09-12 17:32:16.000000 decoder-plus-plus-1.5.0/dpp/core/decoder_plus_plus.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)      906 2022-09-08 00:31:10.000000 decoder-plus-plus-1.5.0/dpp/core/exceptions.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     2806 2022-09-14 00:53:04.000000 decoder-plus-plus-1.5.0/dpp/core/icons.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     3699 2022-09-13 21:25:00.000000 decoder-plus-plus-1.5.0/dpp/core/listener.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     2200 2022-09-15 17:55:42.000000 decoder-plus-plus-1.5.0/dpp/core/logger.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     1329 2022-09-14 00:12:52.000000 decoder-plus-plus-1.5.0/dpp/core/math.py
-drwxrwxr-x   0 tengel    (1000) tengel    (1000)        0 2022-09-15 17:57:59.282219 decoder-plus-plus-1.5.0/dpp/core/plugin/
--rw-rw-r--   0 tengel    (1000) tengel    (1000)    12890 2022-09-15 16:19:03.000000 decoder-plus-plus-1.5.0/dpp/core/plugin/__init__.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     2288 2022-09-15 16:42:41.000000 decoder-plus-plus-1.5.0/dpp/core/plugin/builder.py
-drwxrwxr-x   0 tengel    (1000) tengel    (1000)        0 2022-09-15 17:57:59.282219 decoder-plus-plus-1.5.0/dpp/core/plugin/config/
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     8432 2022-09-13 14:39:30.000000 decoder-plus-plus-1.5.0/dpp/core/plugin/config/__init__.py
-drwxrwxr-x   0 tengel    (1000) tengel    (1000)        0 2022-09-15 17:57:59.282219 decoder-plus-plus-1.5.0/dpp/core/plugin/config/options/
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     2796 2022-09-14 07:38:39.000000 decoder-plus-plus-1.5.0/dpp/core/plugin/config/options/__init__.py
-drwxrwxr-x   0 tengel    (1000) tengel    (1000)        0 2022-09-15 17:57:59.282219 decoder-plus-plus-1.5.0/dpp/core/plugin/config/ui/
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     1572 2022-09-12 21:57:24.000000 decoder-plus-plus-1.5.0/dpp/core/plugin/config/ui/__init__.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)      858 2022-09-06 21:38:42.000000 decoder-plus-plus-1.5.0/dpp/core/plugin/config/ui/layouts.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     1957 2022-09-13 21:47:54.000000 decoder-plus-plus-1.5.0/dpp/core/plugin/config/ui/widgets.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     3048 2022-09-13 07:31:54.000000 decoder-plus-plus-1.5.0/dpp/core/plugin/loader.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     4301 2022-09-12 17:32:16.000000 decoder-plus-plus-1.5.0/dpp/core/plugin/manager.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     3878 2022-08-21 00:18:15.000000 decoder-plus-plus-1.5.0/dpp/core/shortcuts.py
-drwxrwxr-x   0 tengel    (1000) tengel    (1000)        0 2022-09-15 17:57:59.290219 decoder-plus-plus-1.5.0/dpp/images/
--rw-rw-r--   0 tengel    (1000) tengel    (1000)    22919 2021-12-26 21:21:06.000000 decoder-plus-plus-1.5.0/dpp/images/dpp.png
--rw-rw-r--   0 tengel    (1000) tengel    (1000)    10621 2021-12-26 21:21:06.000000 decoder-plus-plus-1.5.0/dpp/images/dpp_128.png
--rw-rw-r--   0 tengel    (1000) tengel    (1000)    22919 2021-12-26 21:21:06.000000 decoder-plus-plus-1.5.0/dpp/images/dpp_classic.png
--rw-rw-r--   0 tengel    (1000) tengel    (1000)    10621 2021-12-26 21:21:06.000000 decoder-plus-plus-1.5.0/dpp/images/dpp_classic_128.png
--rw-rw-r--   0 tengel    (1000) tengel    (1000)    90434 2022-09-06 22:45:08.000000 decoder-plus-plus-1.5.0/dpp/images/dpp_modern.png
--rw-rw-r--   0 tengel    (1000) tengel    (1000)    30058 2022-09-06 22:47:19.000000 decoder-plus-plus-1.5.0/dpp/images/dpp_modern_128.png
--rw-rw-r--   0 tengel    (1000) tengel    (1000)  1494359 2022-09-06 22:43:36.000000 decoder-plus-plus-1.5.0/dpp/images/dpp_modern_big.png
--rw-rw-r--   0 tengel    (1000) tengel    (1000)    25196 2021-12-26 21:21:06.000000 decoder-plus-plus-1.5.0/dpp/images/dpp_xmas.png
--rw-rw-r--   0 tengel    (1000) tengel    (1000)      258 2021-12-26 21:21:06.000000 decoder-plus-plus-1.5.0/dpp/images/hidden.png
--rw-rw-r--   0 tengel    (1000) tengel    (1000)      349 2022-09-13 21:04:47.000000 decoder-plus-plus-1.5.0/dpp/images/indicator_green.png
--rw-rw-r--   0 tengel    (1000) tengel    (1000)      417 2022-09-13 21:05:13.000000 decoder-plus-plus-1.5.0/dpp/images/indicator_grey.png
--rw-rw-r--   0 tengel    (1000) tengel    (1000)      319 2022-09-13 21:05:36.000000 decoder-plus-plus-1.5.0/dpp/images/indicator_red.png
--rw-rw-r--   0 tengel    (1000) tengel    (1000)    11652 2021-12-26 21:21:06.000000 decoder-plus-plus-1.5.0/dpp/images/keyboard.png
--rw-rw-r--   0 tengel    (1000) tengel    (1000)    27999 2021-12-26 21:21:06.000000 decoder-plus-plus-1.5.0/dpp/images/keyboard.svg
-drwxrwxr-x   0 tengel    (1000) tengel    (1000)        0 2022-09-15 17:57:59.314219 decoder-plus-plus-1.5.0/dpp/plugins/
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     1328 2022-09-12 17:32:16.000000 decoder-plus-plus-1.5.0/dpp/plugins/adler32_hasher.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     1393 2022-09-12 17:32:16.000000 decoder-plus-plus-1.5.0/dpp/plugins/apache_md5_hasher.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     1545 2022-09-12 17:32:16.000000 decoder-plus-plus-1.5.0/dpp/plugins/base16_decoder.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     1545 2022-09-12 17:32:16.000000 decoder-plus-plus-1.5.0/dpp/plugins/base16_encoder.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     1824 2022-09-12 17:32:16.000000 decoder-plus-plus-1.5.0/dpp/plugins/base32_decoder.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     1529 2022-09-12 17:32:16.000000 decoder-plus-plus-1.5.0/dpp/plugins/base32_encoder.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     1755 2022-09-12 17:32:16.000000 decoder-plus-plus-1.5.0/dpp/plugins/base45_decoder.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     1482 2022-09-12 17:32:16.000000 decoder-plus-plus-1.5.0/dpp/plugins/base45_encoder.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     2097 2022-09-12 17:32:16.000000 decoder-plus-plus-1.5.0/dpp/plugins/base64_decoder.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     1470 2022-09-12 17:32:16.000000 decoder-plus-plus-1.5.0/dpp/plugins/base64_encoder.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     2678 2022-09-12 17:32:16.000000 decoder-plus-plus-1.5.0/dpp/plugins/base64_url_decoder.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     1693 2022-09-12 17:32:16.000000 decoder-plus-plus-1.5.0/dpp/plugins/base64_url_encoder.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     1241 2022-09-12 17:32:16.000000 decoder-plus-plus-1.5.0/dpp/plugins/bin_int_decoder.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     1249 2022-09-12 17:32:16.000000 decoder-plus-plus-1.5.0/dpp/plugins/bin_int_encoder.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     1519 2022-09-12 17:32:16.000000 decoder-plus-plus-1.5.0/dpp/plugins/bin_str_decoder.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     1695 2022-09-12 17:32:16.000000 decoder-plus-plus-1.5.0/dpp/plugins/bin_str_encoder.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     5617 2022-09-14 07:12:50.000000 decoder-plus-plus-1.5.0/dpp/plugins/caesar_cipher_script.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     1065 2022-09-12 17:32:16.000000 decoder-plus-plus-1.5.0/dpp/plugins/clone_script.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     1320 2022-09-12 17:32:16.000000 decoder-plus-plus-1.5.0/dpp/plugins/crc32_hasher.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     1159 2022-09-12 17:32:16.000000 decoder-plus-plus-1.5.0/dpp/plugins/css_minify_script.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     1475 2022-09-12 17:32:16.000000 decoder-plus-plus-1.5.0/dpp/plugins/dec_str_decoder.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     1441 2022-09-12 17:32:16.000000 decoder-plus-plus-1.5.0/dpp/plugins/dec_str_encoder.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     1068 2022-09-12 17:32:16.000000 decoder-plus-plus-1.5.0/dpp/plugins/escape_string_script.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     1211 2022-09-12 17:32:16.000000 decoder-plus-plus-1.5.0/dpp/plugins/extract_urls_script.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     5143 2022-09-12 17:32:16.000000 decoder-plus-plus-1.5.0/dpp/plugins/filter_lines_script.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     1386 2022-09-12 17:32:16.000000 decoder-plus-plus-1.5.0/dpp/plugins/free_bsd_nt_hasher.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     1653 2022-09-12 17:32:16.000000 decoder-plus-plus-1.5.0/dpp/plugins/gzip_decoder.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     1408 2022-09-12 17:32:16.000000 decoder-plus-plus-1.5.0/dpp/plugins/gzip_encoder.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     1448 2022-09-12 17:32:16.000000 decoder-plus-plus-1.5.0/dpp/plugins/hex_int_decoder.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     1217 2022-09-12 17:32:16.000000 decoder-plus-plus-1.5.0/dpp/plugins/hex_int_encoder.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     2331 2022-09-12 17:32:16.000000 decoder-plus-plus-1.5.0/dpp/plugins/hex_shell_decoder.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     1980 2022-09-12 17:32:16.000000 decoder-plus-plus-1.5.0/dpp/plugins/hex_shell_encoder.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     1709 2022-09-12 17:32:16.000000 decoder-plus-plus-1.5.0/dpp/plugins/hex_str_decoder.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     1561 2022-09-12 17:32:16.000000 decoder-plus-plus-1.5.0/dpp/plugins/hex_str_encoder.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     1221 2022-09-12 17:32:16.000000 decoder-plus-plus-1.5.0/dpp/plugins/html_beautify_script.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     1783 2022-09-12 17:32:16.000000 decoder-plus-plus-1.5.0/dpp/plugins/html_decoder.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     1377 2022-09-12 17:32:16.000000 decoder-plus-plus-1.5.0/dpp/plugins/html_encoder.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     1138 2022-09-12 17:32:16.000000 decoder-plus-plus-1.5.0/dpp/plugins/html_minify_script.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     2539 2022-09-12 17:32:16.000000 decoder-plus-plus-1.5.0/dpp/plugins/http64_decoder.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     1841 2022-09-12 17:32:16.000000 decoder-plus-plus-1.5.0/dpp/plugins/http64_encoder.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     1300 2022-09-12 17:32:16.000000 decoder-plus-plus-1.5.0/dpp/plugins/identify_file_type_script.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     1332 2022-09-12 17:32:16.000000 decoder-plus-plus-1.5.0/dpp/plugins/identify_hash_format_script.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     2254 2022-09-12 17:32:16.000000 decoder-plus-plus-1.5.0/dpp/plugins/jq_script.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     1336 2022-09-12 17:32:16.000000 decoder-plus-plus-1.5.0/dpp/plugins/js_beautify_script.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     1131 2022-09-12 17:32:16.000000 decoder-plus-plus-1.5.0/dpp/plugins/js_minify_script.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     1171 2022-09-12 17:32:16.000000 decoder-plus-plus-1.5.0/dpp/plugins/js_to_xml_script.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)    15167 2022-09-15 00:43:43.000000 decoder-plus-plus-1.5.0/dpp/plugins/jsonify_script.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     2621 2022-09-12 17:32:16.000000 decoder-plus-plus-1.5.0/dpp/plugins/jsonpath_script.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     1612 2022-09-12 17:32:16.000000 decoder-plus-plus-1.5.0/dpp/plugins/jwt_decoder.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     1432 2022-09-15 16:34:02.000000 decoder-plus-plus-1.5.0/dpp/plugins/keccak224_hasher.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     1440 2022-09-12 17:32:16.000000 decoder-plus-plus-1.5.0/dpp/plugins/keccak256_hasher.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     1472 2022-09-12 17:32:16.000000 decoder-plus-plus-1.5.0/dpp/plugins/keccak384_hasher.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     1519 2022-09-12 17:32:16.000000 decoder-plus-plus-1.5.0/dpp/plugins/keccak512_hasher.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     1446 2022-09-12 17:32:16.000000 decoder-plus-plus-1.5.0/dpp/plugins/little_big_endian_script.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     1366 2022-09-12 17:32:16.000000 decoder-plus-plus-1.5.0/dpp/plugins/lm_hasher.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     1364 2022-09-12 17:32:16.000000 decoder-plus-plus-1.5.0/dpp/plugins/md2_hasher.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     1364 2022-09-12 17:32:16.000000 decoder-plus-plus-1.5.0/dpp/plugins/md4_hasher.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     1352 2022-09-12 17:32:16.000000 decoder-plus-plus-1.5.0/dpp/plugins/md5_hasher.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     1366 2022-09-12 17:32:16.000000 decoder-plus-plus-1.5.0/dpp/plugins/nt_hasher.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     1223 2022-09-12 17:32:16.000000 decoder-plus-plus-1.5.0/dpp/plugins/oct_int_decoder.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     1228 2022-09-12 17:32:16.000000 decoder-plus-plus-1.5.0/dpp/plugins/oct_int_encoder.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     1775 2022-09-12 17:32:16.000000 decoder-plus-plus-1.5.0/dpp/plugins/oct_str_decoder.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     1576 2022-09-12 17:32:16.000000 decoder-plus-plus-1.5.0/dpp/plugins/oct_str_encoder.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     1368 2022-09-12 17:32:16.000000 decoder-plus-plus-1.5.0/dpp/plugins/phpass_hasher.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     6634 2022-09-12 17:32:16.000000 decoder-plus-plus-1.5.0/dpp/plugins/reformat_text_script.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     1115 2022-09-12 17:32:16.000000 decoder-plus-plus-1.5.0/dpp/plugins/remove_newlines_script.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     1121 2022-09-12 17:32:16.000000 decoder-plus-plus-1.5.0/dpp/plugins/remove_whitespaces_script.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     1385 2022-09-12 17:32:16.000000 decoder-plus-plus-1.5.0/dpp/plugins/ripemd160_hasher.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     1398 2022-09-12 17:32:16.000000 decoder-plus-plus-1.5.0/dpp/plugins/rot13_decoder.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     1398 2022-09-12 17:32:16.000000 decoder-plus-plus-1.5.0/dpp/plugins/rot13_encoder.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     4534 2022-09-12 17:32:16.000000 decoder-plus-plus-1.5.0/dpp/plugins/search_and_replace_script.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     1363 2022-09-12 17:32:16.000000 decoder-plus-plus-1.5.0/dpp/plugins/sha1_hasher.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     1401 2022-09-12 17:32:16.000000 decoder-plus-plus-1.5.0/dpp/plugins/sha224_hasher.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     1409 2022-09-12 17:32:16.000000 decoder-plus-plus-1.5.0/dpp/plugins/sha256_hasher.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     1441 2022-09-12 17:32:16.000000 decoder-plus-plus-1.5.0/dpp/plugins/sha384_hasher.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     1382 2022-09-12 17:32:16.000000 decoder-plus-plus-1.5.0/dpp/plugins/sha3_224_hasher.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     1383 2022-09-12 17:32:16.000000 decoder-plus-plus-1.5.0/dpp/plugins/sha3_256_hasher.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     1415 2022-09-12 17:32:16.000000 decoder-plus-plus-1.5.0/dpp/plugins/sha3_384_hasher.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     1462 2022-09-12 17:32:16.000000 decoder-plus-plus-1.5.0/dpp/plugins/sha3_512_hasher.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     1474 2022-09-12 18:36:42.000000 decoder-plus-plus-1.5.0/dpp/plugins/sha512_hasher.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     5030 2022-09-12 18:36:42.000000 decoder-plus-plus-1.5.0/dpp/plugins/split_and_rejoin_script.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     1400 2022-09-12 18:36:42.000000 decoder-plus-plus-1.5.0/dpp/plugins/sun_md5_hasher.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     1107 2022-09-12 18:36:42.000000 decoder-plus-plus-1.5.0/dpp/plugins/unescape_string_script.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     1993 2022-09-12 18:36:42.000000 decoder-plus-plus-1.5.0/dpp/plugins/url_decoder.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     1487 2022-09-12 18:36:42.000000 decoder-plus-plus-1.5.0/dpp/plugins/url_encoder.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     1974 2022-09-12 18:36:42.000000 decoder-plus-plus-1.5.0/dpp/plugins/url_plus_decoder.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     1525 2022-09-12 18:36:42.000000 decoder-plus-plus-1.5.0/dpp/plugins/url_plus_encoder.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     2291 2022-09-12 18:36:42.000000 decoder-plus-plus-1.5.0/dpp/plugins/xpath_script.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     1821 2022-09-12 18:36:42.000000 decoder-plus-plus-1.5.0/dpp/plugins/zlib_decoder.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     1394 2022-09-12 18:36:42.000000 decoder-plus-plus-1.5.0/dpp/plugins/zlib_encoder.py
--rwxrwxr-x   0 tengel    (1000) tengel    (1000)    16774 2022-09-13 19:10:59.000000 decoder-plus-plus-1.5.0/dpp/runner.py
-drwxrwxr-x   0 tengel    (1000) tengel    (1000)        0 2022-09-15 17:57:59.314219 decoder-plus-plus-1.5.0/dpp/ui/
--rw-rw-r--   0 tengel    (1000) tengel    (1000)      967 2022-09-06 05:50:59.000000 decoder-plus-plus-1.5.0/dpp/ui/__init__.py
-drwxrwxr-x   0 tengel    (1000) tengel    (1000)        0 2022-09-15 17:57:59.318219 decoder-plus-plus-1.5.0/dpp/ui/builder/
--rw-rw-r--   0 tengel    (1000) tengel    (1000)        0 2021-12-26 21:21:06.000000 decoder-plus-plus-1.5.0/dpp/ui/builder/__init__.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     1962 2022-08-15 20:49:18.000000 decoder-plus-plus-1.5.0/dpp/ui/builder/action_builder.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     1769 2022-09-13 22:57:59.000000 decoder-plus-plus-1.5.0/dpp/ui/builder/plugin_config_widget_builder.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     9218 2022-09-15 00:32:48.000000 decoder-plus-plus-1.5.0/dpp/ui/builder/widget_builder.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     6202 2022-09-15 17:35:01.000000 decoder-plus-plus-1.5.0/dpp/ui/decoder_plus_plus_gui.py
-drwxrwxr-x   0 tengel    (1000) tengel    (1000)        0 2022-09-15 17:57:59.318219 decoder-plus-plus-1.5.0/dpp/ui/dialog/
--rw-rw-r--   0 tengel    (1000) tengel    (1000)      706 2021-12-26 21:21:06.000000 decoder-plus-plus-1.5.0/dpp/ui/dialog/__init__.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     5803 2022-09-12 17:32:16.000000 decoder-plus-plus-1.5.0/dpp/ui/dialog/config_dialog.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     5273 2022-09-10 21:34:51.000000 decoder-plus-plus-1.5.0/dpp/ui/dialog/keyboard_shortcut_dialog.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     6028 2022-09-13 22:57:59.000000 decoder-plus-plus-1.5.0/dpp/ui/dialog/plugin_config_dialog.py
-drwxrwxr-x   0 tengel    (1000) tengel    (1000)        0 2022-09-15 17:57:59.318219 decoder-plus-plus-1.5.0/dpp/ui/dock/
--rw-rw-r--   0 tengel    (1000) tengel    (1000)        0 2021-12-26 21:21:06.000000 decoder-plus-plus-1.5.0/dpp/ui/dock/__init__.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)    10606 2022-09-13 21:26:59.000000 decoder-plus-plus-1.5.0/dpp/ui/dock/hex_dock.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)    12701 2022-09-12 19:05:02.000000 decoder-plus-plus-1.5.0/dpp/ui/dock/log_dock.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     2564 2022-09-07 22:11:21.000000 decoder-plus-plus-1.5.0/dpp/ui/instance_handler.py
-drwxrwxr-x   0 tengel    (1000) tengel    (1000)        0 2022-09-15 17:57:59.318219 decoder-plus-plus-1.5.0/dpp/ui/view/
--rw-rw-r--   0 tengel    (1000) tengel    (1000)      706 2022-08-18 00:21:03.000000 decoder-plus-plus-1.5.0/dpp/ui/view/__init__.py
-drwxrwxr-x   0 tengel    (1000) tengel    (1000)        0 2022-09-15 17:57:59.322219 decoder-plus-plus-1.5.0/dpp/ui/view/classic/
--rw-rw-r--   0 tengel    (1000) tengel    (1000)      839 2022-08-20 19:51:05.000000 decoder-plus-plus-1.5.0/dpp/ui/view/classic/__init__.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)    10176 2022-09-15 01:57:25.000000 decoder-plus-plus-1.5.0/dpp/ui/view/classic/classic_main_window_widget.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)    15304 2022-09-15 16:12:53.000000 decoder-plus-plus-1.5.0/dpp/ui/view/classic/codec_frame.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)    13200 2022-09-15 16:14:00.000000 decoder-plus-plus-1.5.0/dpp/ui/view/classic/codec_frame_header.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)    17547 2022-09-14 00:10:13.000000 decoder-plus-plus-1.5.0/dpp/ui/view/classic/codec_frames.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     2346 2022-09-12 00:44:02.000000 decoder-plus-plus-1.5.0/dpp/ui/view/classic/codec_tab.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     8885 2022-09-15 16:27:26.000000 decoder-plus-plus-1.5.0/dpp/ui/view/classic/combo_box_frame.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)    10504 2022-09-15 01:57:25.000000 decoder-plus-plus-1.5.0/dpp/ui/view/main_window_widget.py
-drwxrwxr-x   0 tengel    (1000) tengel    (1000)        0 2022-09-15 17:57:59.322219 decoder-plus-plus-1.5.0/dpp/ui/view/modern/
--rw-rw-r--   0 tengel    (1000) tengel    (1000)      705 2022-08-20 19:51:05.000000 decoder-plus-plus-1.5.0/dpp/ui/view/modern/__init__.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     2448 2022-09-07 22:10:57.000000 decoder-plus-plus-1.5.0/dpp/ui/view/modern/modern_main_window_widget.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)      705 2022-09-12 17:32:16.000000 decoder-plus-plus-1.5.0/dpp/ui/view/modern/node_data.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     5229 2022-09-12 17:32:16.000000 decoder-plus-plus-1.5.0/dpp/ui/view/modern/node_data_models.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)      409 2022-08-30 00:07:08.000000 decoder-plus-plus-1.5.0/dpp/ui/view/modern/node_data_models_builder.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     2010 2022-09-12 00:44:03.000000 decoder-plus-plus-1.5.0/dpp/ui/view/modern/node_editor.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     1782 2022-09-12 17:32:16.000000 decoder-plus-plus-1.5.0/dpp/ui/view/modern/node_editor_tab.py
-drwxrwxr-x   0 tengel    (1000) tengel    (1000)        0 2022-09-15 17:57:59.330219 decoder-plus-plus-1.5.0/dpp/ui/widget/
--rw-rw-r--   0 tengel    (1000) tengel    (1000)      805 2022-08-16 19:35:20.000000 decoder-plus-plus-1.5.0/dpp/ui/widget/__init__.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     1367 2022-08-15 23:02:30.000000 decoder-plus-plus-1.5.0/dpp/ui/widget/clickable_label.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     3304 2022-09-13 21:57:04.000000 decoder-plus-plus-1.5.0/dpp/ui/widget/codec_preview_widget.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)    11187 2022-09-13 18:29:46.000000 decoder-plus-plus-1.5.0/dpp/ui/widget/collapsible_frame.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     2161 2022-09-10 22:00:08.000000 decoder-plus-plus-1.5.0/dpp/ui/widget/combo_box.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     4686 2022-09-12 17:32:16.000000 decoder-plus-plus-1.5.0/dpp/ui/widget/dock_tabs_widget.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     7690 2022-08-20 19:51:05.000000 decoder-plus-plus-1.5.0/dpp/ui/widget/dock_widget.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     1887 2022-08-15 20:48:14.000000 decoder-plus-plus-1.5.0/dpp/ui/widget/dyna_frame.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)      755 2022-08-15 20:44:52.000000 decoder-plus-plus-1.5.0/dpp/ui/widget/elided_label.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     2453 2022-09-13 19:28:49.000000 decoder-plus-plus-1.5.0/dpp/ui/widget/hover_label.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     1751 2022-09-13 19:04:34.000000 decoder-plus-plus-1.5.0/dpp/ui/widget/icon_label.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     4235 2022-09-14 01:04:28.000000 decoder-plus-plus-1.5.0/dpp/ui/widget/identify_format_button.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     3269 2022-09-12 19:34:03.000000 decoder-plus-plus-1.5.0/dpp/ui/widget/list_widget.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     1151 2022-08-21 00:18:15.000000 decoder-plus-plus-1.5.0/dpp/ui/widget/menu_bar.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     6687 2022-09-12 17:32:16.000000 decoder-plus-plus-1.5.0/dpp/ui/widget/message_widget.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     5355 2022-09-15 00:32:48.000000 decoder-plus-plus-1.5.0/dpp/ui/widget/option_widgets.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)    12432 2022-09-13 21:25:00.000000 decoder-plus-plus-1.5.0/dpp/ui/widget/plain_view.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     2621 2022-09-08 00:44:43.000000 decoder-plus-plus-1.5.0/dpp/ui/widget/plugin_frame.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     9593 2022-09-12 17:32:16.000000 decoder-plus-plus-1.5.0/dpp/ui/widget/plugin_tab.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     4396 2022-09-12 17:32:16.000000 decoder-plus-plus-1.5.0/dpp/ui/widget/search_field.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     1246 2022-09-12 17:32:16.000000 decoder-plus-plus-1.5.0/dpp/ui/widget/separater_widget.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     5000 2022-08-15 23:02:30.000000 decoder-plus-plus-1.5.0/dpp/ui/widget/shortcut_table.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     2846 2022-09-12 18:36:42.000000 decoder-plus-plus-1.5.0/dpp/ui/widget/slider_widget.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     4047 2022-09-14 01:04:28.000000 decoder-plus-plus-1.5.0/dpp/ui/widget/smart_decode_button.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     1442 2022-09-12 18:36:42.000000 decoder-plus-plus-1.5.0/dpp/ui/widget/spacers.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     2217 2022-08-15 20:47:17.000000 decoder-plus-plus-1.5.0/dpp/ui/widget/status_widget.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     3757 2022-08-20 19:51:05.000000 decoder-plus-plus-1.5.0/dpp/ui/widget/tab_bar.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     8075 2022-09-15 01:50:24.000000 decoder-plus-plus-1.5.0/dpp/ui/widget/tabs_widget.py
--rw-rw-r--   0 tengel    (1000) tengel    (1000)       38 2022-09-15 17:57:59.330219 decoder-plus-plus-1.5.0/setup.cfg
--rw-rw-r--   0 tengel    (1000) tengel    (1000)     2589 2022-09-15 15:02:19.000000 decoder-plus-plus-1.5.0/setup.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-07 11:36:23.990036 decoder-plus-plus-1.7.0/
+-rw-rw-r--   0 tom       (1000) tom       (1000)    35147 2021-12-26 21:21:06.000000 decoder-plus-plus-1.7.0/LICENSE
+-rw-rw-r--   0 tom       (1000) tom       (1000)       43 2021-12-26 21:21:06.000000 decoder-plus-plus-1.7.0/MANIFEST.in
+-rw-rw-r--   0 tom       (1000) tom       (1000)     7935 2024-04-07 11:36:23.990036 decoder-plus-plus-1.7.0/PKG-INFO
+-rw-rw-r--   0 tom       (1000) tom       (1000)     7367 2024-04-07 09:27:21.000000 decoder-plus-plus-1.7.0/README.md
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-07 11:36:23.938036 decoder-plus-plus-1.7.0/data/
+-rwxrwxr-x   0 tom       (1000) tom       (1000)      116 2021-12-26 21:21:06.000000 decoder-plus-plus-1.7.0/data/dpp.desktop
+-rw-rw-r--   0 tom       (1000) tom       (1000)    19277 2024-04-06 19:21:46.000000 decoder-plus-plus-1.7.0/data/dpp.png
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-07 11:36:23.938036 decoder-plus-plus-1.7.0/decoder_plus_plus.egg-info/
+-rw-rw-r--   0 tom       (1000) tom       (1000)     7935 2024-04-07 11:36:23.000000 decoder-plus-plus-1.7.0/decoder_plus_plus.egg-info/PKG-INFO
+-rw-rw-r--   0 tom       (1000) tom       (1000)     9070 2024-04-07 11:36:23.000000 decoder-plus-plus-1.7.0/decoder_plus_plus.egg-info/SOURCES.txt
+-rw-rw-r--   0 tom       (1000) tom       (1000)        1 2024-04-07 11:36:23.000000 decoder-plus-plus-1.7.0/decoder_plus_plus.egg-info/dependency_links.txt
+-rw-rw-r--   0 tom       (1000) tom       (1000)       40 2024-04-07 11:36:23.000000 decoder-plus-plus-1.7.0/decoder_plus_plus.egg-info/entry_points.txt
+-rw-rw-r--   0 tom       (1000) tom       (1000)      389 2024-04-07 11:36:23.000000 decoder-plus-plus-1.7.0/decoder_plus_plus.egg-info/requires.txt
+-rw-rw-r--   0 tom       (1000) tom       (1000)       10 2024-04-07 11:36:23.000000 decoder-plus-plus-1.7.0/decoder_plus_plus.egg-info/top_level.txt
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-07 11:36:23.942036 decoder-plus-plus-1.7.0/dpp/
+-rw-rw-r--   0 tom       (1000) tom       (1000)      850 2024-04-07 11:23:42.000000 decoder-plus-plus-1.7.0/dpp/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      239 2021-12-26 21:21:06.000000 decoder-plus-plus-1.7.0/dpp/__main__.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-07 11:36:23.942036 decoder-plus-plus-1.7.0/dpp/core/
+-rw-rw-r--   0 tom       (1000) tom       (1000)      915 2021-12-26 21:21:06.000000 decoder-plus-plus-1.7.0/dpp/core/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2353 2022-09-12 19:05:02.000000 decoder-plus-plus-1.7.0/dpp/core/argparse.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2871 2022-09-12 21:57:24.000000 decoder-plus-plus-1.7.0/dpp/core/assertions.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     3279 2022-08-17 05:09:19.000000 decoder-plus-plus-1.7.0/dpp/core/config.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)    10068 2024-04-05 20:12:39.000000 decoder-plus-plus-1.7.0/dpp/core/context.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2328 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.0/dpp/core/decoder_plus_plus.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      906 2022-09-18 10:36:35.000000 decoder-plus-plus-1.7.0/dpp/core/exceptions.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2860 2024-04-07 11:17:10.000000 decoder-plus-plus-1.7.0/dpp/core/icons.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     3650 2023-02-28 12:27:33.000000 decoder-plus-plus-1.7.0/dpp/core/listener.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     4546 2023-01-29 15:42:26.000000 decoder-plus-plus-1.7.0/dpp/core/logger.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1329 2022-09-14 00:12:52.000000 decoder-plus-plus-1.7.0/dpp/core/math.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-07 11:36:23.942036 decoder-plus-plus-1.7.0/dpp/core/plugin/
+-rw-rw-r--   0 tom       (1000) tom       (1000)    14067 2024-04-06 16:14:35.000000 decoder-plus-plus-1.7.0/dpp/core/plugin/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2324 2024-04-06 15:25:06.000000 decoder-plus-plus-1.7.0/dpp/core/plugin/builder.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-07 11:36:23.942036 decoder-plus-plus-1.7.0/dpp/core/plugin/config/
+-rw-rw-r--   0 tom       (1000) tom       (1000)     8387 2024-04-06 08:18:07.000000 decoder-plus-plus-1.7.0/dpp/core/plugin/config/__init__.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-07 11:36:23.942036 decoder-plus-plus-1.7.0/dpp/core/plugin/config/options/
+-rw-rw-r--   0 tom       (1000) tom       (1000)     3478 2024-04-06 16:14:35.000000 decoder-plus-plus-1.7.0/dpp/core/plugin/config/options/__init__.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-07 11:36:23.942036 decoder-plus-plus-1.7.0/dpp/core/plugin/config/ui/
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1572 2022-09-12 21:57:24.000000 decoder-plus-plus-1.7.0/dpp/core/plugin/config/ui/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      858 2022-09-06 21:38:42.000000 decoder-plus-plus-1.7.0/dpp/core/plugin/config/ui/layouts.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2111 2024-04-06 15:51:05.000000 decoder-plus-plus-1.7.0/dpp/core/plugin/config/ui/widgets.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     3048 2022-09-13 07:31:54.000000 decoder-plus-plus-1.7.0/dpp/core/plugin/loader.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     4301 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.0/dpp/core/plugin/manager.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     3878 2022-08-21 00:18:15.000000 decoder-plus-plus-1.7.0/dpp/core/shortcuts.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-07 11:36:23.950036 decoder-plus-plus-1.7.0/dpp/images/
+-rw-rw-r--   0 tom       (1000) tom       (1000)    22919 2021-12-26 21:21:06.000000 decoder-plus-plus-1.7.0/dpp/images/dpp.png
+-rw-rw-r--   0 tom       (1000) tom       (1000)    10621 2021-12-26 21:21:06.000000 decoder-plus-plus-1.7.0/dpp/images/dpp_128.png
+-rw-rw-r--   0 tom       (1000) tom       (1000)    22919 2021-12-26 21:21:06.000000 decoder-plus-plus-1.7.0/dpp/images/dpp_classic.png
+-rw-rw-r--   0 tom       (1000) tom       (1000)    10621 2021-12-26 21:21:06.000000 decoder-plus-plus-1.7.0/dpp/images/dpp_classic_128.png
+-rw-rw-r--   0 tom       (1000) tom       (1000)    90434 2022-09-06 22:45:08.000000 decoder-plus-plus-1.7.0/dpp/images/dpp_modern.png
+-rw-rw-r--   0 tom       (1000) tom       (1000)    30058 2022-09-06 22:47:19.000000 decoder-plus-plus-1.7.0/dpp/images/dpp_modern_128.png
+-rw-rw-r--   0 tom       (1000) tom       (1000)  1494359 2022-09-06 22:43:36.000000 decoder-plus-plus-1.7.0/dpp/images/dpp_modern_big.png
+-rw-rw-r--   0 tom       (1000) tom       (1000)    56153 2024-04-06 19:21:10.000000 decoder-plus-plus-1.7.0/dpp/images/dpp_stylized.png
+-rw-rw-r--   0 tom       (1000) tom       (1000)    19277 2024-04-06 19:21:46.000000 decoder-plus-plus-1.7.0/dpp/images/dpp_stylized_128.png
+-rw-rw-r--   0 tom       (1000) tom       (1000)    25196 2021-12-26 21:21:06.000000 decoder-plus-plus-1.7.0/dpp/images/dpp_xmas.png
+-rw-rw-r--   0 tom       (1000) tom       (1000)    52648 2024-04-06 19:39:41.000000 decoder-plus-plus-1.7.0/dpp/images/dpp_xmas_stylized.png
+-rw-rw-r--   0 tom       (1000) tom       (1000)      258 2021-12-26 21:21:06.000000 decoder-plus-plus-1.7.0/dpp/images/hidden.png
+-rw-rw-r--   0 tom       (1000) tom       (1000)      349 2022-09-13 21:04:47.000000 decoder-plus-plus-1.7.0/dpp/images/indicator_green.png
+-rw-rw-r--   0 tom       (1000) tom       (1000)      417 2022-09-13 21:05:13.000000 decoder-plus-plus-1.7.0/dpp/images/indicator_grey.png
+-rw-rw-r--   0 tom       (1000) tom       (1000)      319 2022-09-13 21:05:36.000000 decoder-plus-plus-1.7.0/dpp/images/indicator_red.png
+-rw-rw-r--   0 tom       (1000) tom       (1000)    11652 2021-12-26 21:21:06.000000 decoder-plus-plus-1.7.0/dpp/images/keyboard.png
+-rw-rw-r--   0 tom       (1000) tom       (1000)    27999 2021-12-26 21:21:06.000000 decoder-plus-plus-1.7.0/dpp/images/keyboard.svg
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-07 11:36:23.966036 decoder-plus-plus-1.7.0/dpp/plugins/
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1328 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.0/dpp/plugins/adler32_hasher.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1393 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.0/dpp/plugins/apache_md5_hasher.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1545 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.0/dpp/plugins/base16_decoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1545 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.0/dpp/plugins/base16_encoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1824 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.0/dpp/plugins/base32_decoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1529 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.0/dpp/plugins/base32_encoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1755 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.0/dpp/plugins/base45_decoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1482 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.0/dpp/plugins/base45_encoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2097 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.0/dpp/plugins/base64_decoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1470 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.0/dpp/plugins/base64_encoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2678 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.0/dpp/plugins/base64_url_decoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1693 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.0/dpp/plugins/base64_url_encoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1241 2022-09-17 09:11:33.000000 decoder-plus-plus-1.7.0/dpp/plugins/bin_int_decoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1249 2022-09-17 09:11:33.000000 decoder-plus-plus-1.7.0/dpp/plugins/bin_int_encoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1519 2022-09-17 09:11:33.000000 decoder-plus-plus-1.7.0/dpp/plugins/bin_str_decoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1695 2022-09-17 09:11:33.000000 decoder-plus-plus-1.7.0/dpp/plugins/bin_str_encoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     5641 2024-04-05 16:00:23.000000 decoder-plus-plus-1.7.0/dpp/plugins/caesar_cipher_script.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1065 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.0/dpp/plugins/clone_script.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1320 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.0/dpp/plugins/crc32_hasher.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1159 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.0/dpp/plugins/css_minify_script.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     5888 2024-04-06 15:56:04.000000 decoder-plus-plus-1.7.0/dpp/plugins/custom_code.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1475 2022-09-17 09:13:06.000000 decoder-plus-plus-1.7.0/dpp/plugins/dec_str_decoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1441 2022-09-17 09:13:12.000000 decoder-plus-plus-1.7.0/dpp/plugins/dec_str_encoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1068 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.0/dpp/plugins/escape_string_script.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1211 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.0/dpp/plugins/extract_urls_script.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     5143 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.0/dpp/plugins/filter_lines_script.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1386 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.0/dpp/plugins/free_bsd_nt_hasher.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1653 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.0/dpp/plugins/gzip_decoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1408 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.0/dpp/plugins/gzip_encoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2110 2022-11-01 18:01:29.000000 decoder-plus-plus-1.7.0/dpp/plugins/hex_char_decoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1582 2022-11-01 18:01:29.000000 decoder-plus-plus-1.7.0/dpp/plugins/hex_char_encoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1448 2022-11-01 18:01:29.000000 decoder-plus-plus-1.7.0/dpp/plugins/hex_int_decoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1217 2022-11-01 18:01:29.000000 decoder-plus-plus-1.7.0/dpp/plugins/hex_int_encoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2331 2022-11-01 18:01:29.000000 decoder-plus-plus-1.7.0/dpp/plugins/hex_shell_decoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1980 2022-11-01 18:01:29.000000 decoder-plus-plus-1.7.0/dpp/plugins/hex_shell_encoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1709 2022-11-01 18:01:29.000000 decoder-plus-plus-1.7.0/dpp/plugins/hex_str_decoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1561 2022-11-01 18:01:29.000000 decoder-plus-plus-1.7.0/dpp/plugins/hex_str_encoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1221 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.0/dpp/plugins/html_beautify_script.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1783 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.0/dpp/plugins/html_decoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1377 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.0/dpp/plugins/html_encoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1138 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.0/dpp/plugins/html_minify_script.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2539 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.0/dpp/plugins/http64_decoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1841 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.0/dpp/plugins/http64_encoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2265 2024-04-07 11:11:41.000000 decoder-plus-plus-1.7.0/dpp/plugins/identify_decoder_script.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1371 2024-04-07 11:16:17.000000 decoder-plus-plus-1.7.0/dpp/plugins/identify_file_type_filemagic_script.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1478 2024-04-07 11:16:17.000000 decoder-plus-plus-1.7.0/dpp/plugins/identify_file_type_magika_script.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1389 2024-04-07 11:03:59.000000 decoder-plus-plus-1.7.0/dpp/plugins/identify_hash_format_script.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2254 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.0/dpp/plugins/jq_script.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1336 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.0/dpp/plugins/js_beautify_script.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1131 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.0/dpp/plugins/js_minify_script.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1171 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.0/dpp/plugins/js_to_xml_script.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)    15185 2024-04-07 08:30:22.000000 decoder-plus-plus-1.7.0/dpp/plugins/jsonify_script.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2621 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.0/dpp/plugins/jsonpath_script.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1612 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.0/dpp/plugins/jwt_decoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1432 2022-09-15 16:34:02.000000 decoder-plus-plus-1.7.0/dpp/plugins/keccak224_hasher.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1440 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.0/dpp/plugins/keccak256_hasher.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1472 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.0/dpp/plugins/keccak384_hasher.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1519 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.0/dpp/plugins/keccak512_hasher.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1446 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.0/dpp/plugins/little_big_endian_script.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1366 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.0/dpp/plugins/lm_hasher.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1364 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.0/dpp/plugins/md2_hasher.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1364 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.0/dpp/plugins/md4_hasher.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1352 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.0/dpp/plugins/md5_hasher.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1366 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.0/dpp/plugins/nt_hasher.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1223 2022-09-17 09:11:33.000000 decoder-plus-plus-1.7.0/dpp/plugins/oct_int_decoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1228 2022-09-17 09:11:33.000000 decoder-plus-plus-1.7.0/dpp/plugins/oct_int_encoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1775 2022-09-17 09:11:33.000000 decoder-plus-plus-1.7.0/dpp/plugins/oct_str_decoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1576 2022-09-17 09:11:33.000000 decoder-plus-plus-1.7.0/dpp/plugins/oct_str_encoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1368 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.0/dpp/plugins/phpass_hasher.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     6590 2024-04-05 18:32:58.000000 decoder-plus-plus-1.7.0/dpp/plugins/reformat_text_script.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1115 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.0/dpp/plugins/remove_newlines_script.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1121 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.0/dpp/plugins/remove_whitespaces_script.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1693 2024-04-07 07:30:09.000000 decoder-plus-plus-1.7.0/dpp/plugins/ripemd160_hasher.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1398 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.0/dpp/plugins/rot13_decoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1398 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.0/dpp/plugins/rot13_encoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     4506 2024-04-05 18:32:58.000000 decoder-plus-plus-1.7.0/dpp/plugins/search_and_replace_script.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1363 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.0/dpp/plugins/sha1_hasher.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1401 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.0/dpp/plugins/sha224_hasher.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1409 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.0/dpp/plugins/sha256_hasher.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1441 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.0/dpp/plugins/sha384_hasher.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1382 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.0/dpp/plugins/sha3_224_hasher.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1383 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.0/dpp/plugins/sha3_256_hasher.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1415 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.0/dpp/plugins/sha3_384_hasher.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1462 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.0/dpp/plugins/sha3_512_hasher.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1474 2022-09-12 18:36:42.000000 decoder-plus-plus-1.7.0/dpp/plugins/sha512_hasher.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     4998 2024-04-05 18:32:58.000000 decoder-plus-plus-1.7.0/dpp/plugins/split_and_rejoin_script.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1400 2022-09-12 18:36:42.000000 decoder-plus-plus-1.7.0/dpp/plugins/sun_md5_hasher.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1107 2022-09-12 18:36:42.000000 decoder-plus-plus-1.7.0/dpp/plugins/unescape_string_script.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1993 2022-09-12 18:36:42.000000 decoder-plus-plus-1.7.0/dpp/plugins/url_decoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1487 2022-09-12 18:36:42.000000 decoder-plus-plus-1.7.0/dpp/plugins/url_encoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1974 2022-09-12 18:36:42.000000 decoder-plus-plus-1.7.0/dpp/plugins/url_plus_decoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1525 2022-09-12 18:36:42.000000 decoder-plus-plus-1.7.0/dpp/plugins/url_plus_encoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2291 2023-01-15 14:37:27.000000 decoder-plus-plus-1.7.0/dpp/plugins/xpath_script.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1821 2022-09-12 18:36:42.000000 decoder-plus-plus-1.7.0/dpp/plugins/zlib_decoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1394 2022-09-12 18:36:42.000000 decoder-plus-plus-1.7.0/dpp/plugins/zlib_encoder.py
+-rwxrwxr-x   0 tom       (1000) tom       (1000)    16769 2022-09-21 05:00:04.000000 decoder-plus-plus-1.7.0/dpp/runner.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-07 11:36:23.966036 decoder-plus-plus-1.7.0/dpp/ui/
+-rw-rw-r--   0 tom       (1000) tom       (1000)      967 2022-09-06 05:50:59.000000 decoder-plus-plus-1.7.0/dpp/ui/__init__.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-07 11:36:23.966036 decoder-plus-plus-1.7.0/dpp/ui/builder/
+-rw-rw-r--   0 tom       (1000) tom       (1000)        0 2021-12-26 21:21:06.000000 decoder-plus-plus-1.7.0/dpp/ui/builder/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1962 2022-08-15 20:49:18.000000 decoder-plus-plus-1.7.0/dpp/ui/builder/action_builder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1547 2023-03-07 03:42:36.000000 decoder-plus-plus-1.7.0/dpp/ui/builder/input_text_builder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1682 2024-04-05 15:27:20.000000 decoder-plus-plus-1.7.0/dpp/ui/builder/plugin_config_widget_builder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)    10393 2024-04-07 07:53:50.000000 decoder-plus-plus-1.7.0/dpp/ui/builder/widget_builder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     6388 2023-01-29 15:44:47.000000 decoder-plus-plus-1.7.0/dpp/ui/decoder_plus_plus_gui.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-07 11:36:23.970036 decoder-plus-plus-1.7.0/dpp/ui/dialog/
+-rw-rw-r--   0 tom       (1000) tom       (1000)      706 2021-12-26 21:21:06.000000 decoder-plus-plus-1.7.0/dpp/ui/dialog/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     5833 2024-04-06 19:42:04.000000 decoder-plus-plus-1.7.0/dpp/ui/dialog/config_dialog.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     5273 2022-09-10 21:34:51.000000 decoder-plus-plus-1.7.0/dpp/ui/dialog/keyboard_shortcut_dialog.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     6012 2024-04-06 09:24:31.000000 decoder-plus-plus-1.7.0/dpp/ui/dialog/plugin_config_dialog.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-07 11:36:23.970036 decoder-plus-plus-1.7.0/dpp/ui/dock/
+-rw-rw-r--   0 tom       (1000) tom       (1000)        0 2021-12-26 21:21:06.000000 decoder-plus-plus-1.7.0/dpp/ui/dock/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)    10582 2023-02-28 12:28:51.000000 decoder-plus-plus-1.7.0/dpp/ui/dock/hex_dock.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)    12701 2022-09-12 19:05:02.000000 decoder-plus-plus-1.7.0/dpp/ui/dock/log_dock.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2564 2022-09-07 22:11:21.000000 decoder-plus-plus-1.7.0/dpp/ui/instance_handler.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-07 11:36:23.970036 decoder-plus-plus-1.7.0/dpp/ui/view/
+-rw-rw-r--   0 tom       (1000) tom       (1000)      706 2022-08-18 00:21:03.000000 decoder-plus-plus-1.7.0/dpp/ui/view/__init__.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-07 11:36:23.970036 decoder-plus-plus-1.7.0/dpp/ui/view/classic/
+-rw-rw-r--   0 tom       (1000) tom       (1000)      839 2022-08-20 19:51:05.000000 decoder-plus-plus-1.7.0/dpp/ui/view/classic/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)    10186 2024-04-06 16:14:35.000000 decoder-plus-plus-1.7.0/dpp/ui/view/classic/classic_main_window_widget.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)    16982 2024-04-06 20:23:23.000000 decoder-plus-plus-1.7.0/dpp/ui/view/classic/codec_frame.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)    13200 2022-09-15 16:14:00.000000 decoder-plus-plus-1.7.0/dpp/ui/view/classic/codec_frame_header.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)    20241 2023-03-14 08:06:16.000000 decoder-plus-plus-1.7.0/dpp/ui/view/classic/codec_frames.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2401 2022-09-20 04:28:03.000000 decoder-plus-plus-1.7.0/dpp/ui/view/classic/codec_tab.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     9167 2023-01-30 13:35:51.000000 decoder-plus-plus-1.7.0/dpp/ui/view/classic/combo_box_frame.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)    10716 2022-09-21 05:00:04.000000 decoder-plus-plus-1.7.0/dpp/ui/view/main_window_widget.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-07 11:36:23.970036 decoder-plus-plus-1.7.0/dpp/ui/view/modern/
+-rw-rw-r--   0 tom       (1000) tom       (1000)      705 2022-08-20 19:51:05.000000 decoder-plus-plus-1.7.0/dpp/ui/view/modern/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2460 2022-09-17 10:02:26.000000 decoder-plus-plus-1.7.0/dpp/ui/view/modern/modern_main_window_widget.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      705 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.0/dpp/ui/view/modern/node_data.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     5229 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.0/dpp/ui/view/modern/node_data_models.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      409 2022-08-30 00:07:08.000000 decoder-plus-plus-1.7.0/dpp/ui/view/modern/node_data_models_builder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2001 2022-09-17 10:02:44.000000 decoder-plus-plus-1.7.0/dpp/ui/view/modern/node_editor.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1782 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.0/dpp/ui/view/modern/node_editor_tab.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-07 11:36:23.978036 decoder-plus-plus-1.7.0/dpp/ui/widget/
+-rw-rw-r--   0 tom       (1000) tom       (1000)      805 2022-08-16 19:35:20.000000 decoder-plus-plus-1.7.0/dpp/ui/widget/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1367 2022-08-15 23:02:30.000000 decoder-plus-plus-1.7.0/dpp/ui/widget/clickable_label.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     3507 2024-04-06 16:14:35.000000 decoder-plus-plus-1.7.0/dpp/ui/widget/code_editor_widget.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     3404 2024-04-07 09:41:34.000000 decoder-plus-plus-1.7.0/dpp/ui/widget/codec_preview_widget.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)    11051 2024-04-06 07:30:01.000000 decoder-plus-plus-1.7.0/dpp/ui/widget/collapsible_frame.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2161 2022-09-10 22:00:08.000000 decoder-plus-plus-1.7.0/dpp/ui/widget/combo_box.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     4686 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.0/dpp/ui/widget/dock_tabs_widget.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     7690 2022-08-20 19:51:05.000000 decoder-plus-plus-1.7.0/dpp/ui/widget/dock_widget.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1887 2022-08-15 20:48:14.000000 decoder-plus-plus-1.7.0/dpp/ui/widget/dyna_frame.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      755 2022-08-15 20:44:52.000000 decoder-plus-plus-1.7.0/dpp/ui/widget/elided_label.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2453 2024-04-06 20:17:41.000000 decoder-plus-plus-1.7.0/dpp/ui/widget/hover_label.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1793 2024-04-06 07:22:30.000000 decoder-plus-plus-1.7.0/dpp/ui/widget/icon_label.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     3270 2024-04-07 11:20:24.000000 decoder-plus-plus-1.7.0/dpp/ui/widget/identify_format_button.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     3269 2022-09-12 19:34:03.000000 decoder-plus-plus-1.7.0/dpp/ui/widget/list_widget.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1151 2022-08-21 00:18:15.000000 decoder-plus-plus-1.7.0/dpp/ui/widget/menu_bar.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2136 2024-04-06 09:24:31.000000 decoder-plus-plus-1.7.0/dpp/ui/widget/message_box_widget.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     6687 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.0/dpp/ui/widget/message_widget.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     6110 2024-04-06 15:44:53.000000 decoder-plus-plus-1.7.0/dpp/ui/widget/option_widgets.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)    16152 2023-03-14 08:16:41.000000 decoder-plus-plus-1.7.0/dpp/ui/widget/plain_view.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2621 2022-09-08 00:44:43.000000 decoder-plus-plus-1.7.0/dpp/ui/widget/plugin_frame.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     9593 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.0/dpp/ui/widget/plugin_tab.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     4396 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.0/dpp/ui/widget/search_field.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1246 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.0/dpp/ui/widget/separater_widget.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     5000 2022-08-15 23:02:30.000000 decoder-plus-plus-1.7.0/dpp/ui/widget/shortcut_table.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2846 2022-09-12 18:36:42.000000 decoder-plus-plus-1.7.0/dpp/ui/widget/slider_widget.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     4055 2022-09-20 10:34:13.000000 decoder-plus-plus-1.7.0/dpp/ui/widget/smart_decode_button.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1442 2022-09-12 18:36:42.000000 decoder-plus-plus-1.7.0/dpp/ui/widget/spacers.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2425 2023-01-30 12:23:56.000000 decoder-plus-plus-1.7.0/dpp/ui/widget/status_widget.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     3757 2022-08-20 19:51:05.000000 decoder-plus-plus-1.7.0/dpp/ui/widget/tab_bar.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     8075 2022-09-15 01:50:24.000000 decoder-plus-plus-1.7.0/dpp/ui/widget/tabs_widget.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     3210 2024-04-05 11:52:36.000000 decoder-plus-plus-1.7.0/dpp/ui/widget/text_widget.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)       38 2024-04-07 11:36:23.990036 decoder-plus-plus-1.7.0/setup.cfg
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2679 2024-04-07 10:39:21.000000 decoder-plus-plus-1.7.0/setup.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-07 11:36:23.978036 decoder-plus-plus-1.7.0/tests/
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1805 2023-01-15 14:31:34.000000 decoder-plus-plus-1.7.0/tests/__init__.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-07 11:36:23.990036 decoder-plus-plus-1.7.0/tests/plugins/
+-rw-rw-r--   0 tom       (1000) tom       (1000)        0 2022-11-01 13:33:59.000000 decoder-plus-plus-1.7.0/tests/plugins/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1113 2022-11-01 14:08:45.000000 decoder-plus-plus-1.7.0/tests/plugins/adler32_hasher_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1191 2022-11-01 18:50:27.000000 decoder-plus-plus-1.7.0/tests/plugins/apache_md5_hasher_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1295 2022-11-01 18:05:54.000000 decoder-plus-plus-1.7.0/tests/plugins/base16_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1680 2023-01-15 13:01:54.000000 decoder-plus-plus-1.7.0/tests/plugins/base32_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1287 2023-01-15 13:32:25.000000 decoder-plus-plus-1.7.0/tests/plugins/base45_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1288 2023-01-15 12:36:51.000000 decoder-plus-plus-1.7.0/tests/plugins/base64_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1474 2023-01-15 12:47:27.000000 decoder-plus-plus-1.7.0/tests/plugins/base64_url_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1229 2023-01-15 13:29:43.000000 decoder-plus-plus-1.7.0/tests/plugins/bin_int_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1040 2022-11-01 18:51:09.000000 decoder-plus-plus-1.7.0/tests/plugins/bin_str_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      992 2023-01-15 12:47:59.000000 decoder-plus-plus-1.7.0/tests/plugins/caesar_cipher_script_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1222 2022-11-01 18:35:38.000000 decoder-plus-plus-1.7.0/tests/plugins/clone_script_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1108 2023-01-15 12:37:31.000000 decoder-plus-plus-1.7.0/tests/plugins/crc32_hasher_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1183 2022-11-01 18:39:55.000000 decoder-plus-plus-1.7.0/tests/plugins/css_minify_script_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1401 2022-11-01 18:35:21.000000 decoder-plus-plus-1.7.0/tests/plugins/dec_str_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1245 2022-11-01 18:59:45.000000 decoder-plus-plus-1.7.0/tests/plugins/escape_string_script_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1123 2022-11-01 18:47:57.000000 decoder-plus-plus-1.7.0/tests/plugins/extract_urls_script_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1165 2022-11-01 18:40:22.000000 decoder-plus-plus-1.7.0/tests/plugins/filter_lines_script_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1189 2023-01-15 13:03:50.000000 decoder-plus-plus-1.7.0/tests/plugins/free_bsd_nt_hasher_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1253 2023-01-15 12:29:09.000000 decoder-plus-plus-1.7.0/tests/plugins/gzip_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1067 2022-11-01 18:47:18.000000 decoder-plus-plus-1.7.0/tests/plugins/hex_char_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1193 2023-01-15 13:10:42.000000 decoder-plus-plus-1.7.0/tests/plugins/hex_int_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1614 2022-11-01 18:43:06.000000 decoder-plus-plus-1.7.0/tests/plugins/hex_shell_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1313 2023-01-15 13:16:46.000000 decoder-plus-plus-1.7.0/tests/plugins/hex_str_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1173 2022-11-01 18:43:28.000000 decoder-plus-plus-1.7.0/tests/plugins/html_beautify_script_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1168 2022-11-01 18:48:47.000000 decoder-plus-plus-1.7.0/tests/plugins/html_minify_script_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1172 2023-01-15 12:22:31.000000 decoder-plus-plus-1.7.0/tests/plugins/html_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1219 2022-11-01 18:32:01.000000 decoder-plus-plus-1.7.0/tests/plugins/http64_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1004 2023-01-15 12:39:55.000000 decoder-plus-plus-1.7.0/tests/plugins/identify_file_type_script_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1108 2022-11-01 18:39:55.000000 decoder-plus-plus-1.7.0/tests/plugins/identify_hash_format_script_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1145 2023-01-15 13:26:35.000000 decoder-plus-plus-1.7.0/tests/plugins/jq_script_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      988 2023-01-15 12:41:00.000000 decoder-plus-plus-1.7.0/tests/plugins/js_beautify_script_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1164 2022-11-01 18:49:20.000000 decoder-plus-plus-1.7.0/tests/plugins/js_minify_script_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      977 2023-01-15 13:06:33.000000 decoder-plus-plus-1.7.0/tests/plugins/js_to_xml_script_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      981 2023-01-15 13:02:34.000000 decoder-plus-plus-1.7.0/tests/plugins/jsonify_script_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1163 2022-11-01 18:49:36.000000 decoder-plus-plus-1.7.0/tests/plugins/jsonpath_script_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      976 2023-01-15 12:39:55.000000 decoder-plus-plus-1.7.0/tests/plugins/jwt_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1163 2023-01-15 13:02:49.000000 decoder-plus-plus-1.7.0/tests/plugins/keccak224_hasher_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1171 2022-11-01 18:56:46.000000 decoder-plus-plus-1.7.0/tests/plugins/keccak256_hasher_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1203 2022-11-01 18:45:25.000000 decoder-plus-plus-1.7.0/tests/plugins/keccak384_hasher_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1235 2022-11-01 18:48:57.000000 decoder-plus-plus-1.7.0/tests/plugins/keccak512_hasher_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1245 2022-11-01 18:31:13.000000 decoder-plus-plus-1.7.0/tests/plugins/little_big_endian_script_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1124 2022-11-01 18:56:24.000000 decoder-plus-plus-1.7.0/tests/plugins/lm_hasher_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1126 2022-11-01 18:24:14.000000 decoder-plus-plus-1.7.0/tests/plugins/md2_hasher_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1126 2022-11-01 18:56:15.000000 decoder-plus-plus-1.7.0/tests/plugins/md4_hasher_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1126 2022-11-01 18:45:18.000000 decoder-plus-plus-1.7.0/tests/plugins/md5_hasher_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1124 2022-11-01 18:46:24.000000 decoder-plus-plus-1.7.0/tests/plugins/nt_hasher_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1193 2023-01-15 13:13:49.000000 decoder-plus-plus-1.7.0/tests/plugins/oct_int_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1405 2022-11-01 18:20:57.000000 decoder-plus-plus-1.7.0/tests/plugins/oct_str_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1181 2023-01-15 12:51:06.000000 decoder-plus-plus-1.7.0/tests/plugins/phpass_hasher_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1167 2022-11-01 18:57:07.000000 decoder-plus-plus-1.7.0/tests/plugins/reformat_text_script_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1187 2023-01-15 13:04:21.000000 decoder-plus-plus-1.7.0/tests/plugins/remove_newlines_script_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1064 2022-11-01 18:56:04.000000 decoder-plus-plus-1.7.0/tests/plugins/remove_whitespaces_script_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1146 2022-11-01 18:56:36.000000 decoder-plus-plus-1.7.0/tests/plugins/ripemd160_hasher_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1225 2022-11-01 18:26:44.000000 decoder-plus-plus-1.7.0/tests/plugins/rot13_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1503 2023-01-15 13:05:35.000000 decoder-plus-plus-1.7.0/tests/plugins/search_and_replace_script_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1136 2022-11-01 18:27:54.000000 decoder-plus-plus-1.7.0/tests/plugins/sha1_hasher_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1192 2022-11-01 18:29:14.000000 decoder-plus-plus-1.7.0/tests/plugins/sha224_hasher_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1200 2022-11-01 18:29:35.000000 decoder-plus-plus-1.7.0/tests/plugins/sha256_hasher_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1231 2022-11-01 18:29:59.000000 decoder-plus-plus-1.7.0/tests/plugins/sha384_hasher_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1160 2023-01-15 12:37:21.000000 decoder-plus-plus-1.7.0/tests/plugins/sha3_224_hasher_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1168 2022-11-01 18:53:45.000000 decoder-plus-plus-1.7.0/tests/plugins/sha3_256_hasher_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1200 2022-11-01 18:28:35.000000 decoder-plus-plus-1.7.0/tests/plugins/sha3_384_hasher_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1268 2022-11-01 18:28:57.000000 decoder-plus-plus-1.7.0/tests/plugins/sha3_512_hasher_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1263 2022-11-01 18:30:17.000000 decoder-plus-plus-1.7.0/tests/plugins/sha512_hasher_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1170 2022-11-01 18:57:46.000000 decoder-plus-plus-1.7.0/tests/plugins/split_and_rejoin_script_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      983 2023-01-15 12:39:55.000000 decoder-plus-plus-1.7.0/tests/plugins/sun_md5_hasher_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1247 2022-11-01 18:32:56.000000 decoder-plus-plus-1.7.0/tests/plugins/unescape_string_script_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1282 2022-11-01 18:45:08.000000 decoder-plus-plus-1.7.0/tests/plugins/url_plus_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1136 2022-11-01 18:53:35.000000 decoder-plus-plus-1.7.0/tests/plugins/url_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1136 2023-01-15 14:38:44.000000 decoder-plus-plus-1.7.0/tests/plugins/xpath_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1223 2023-01-15 13:12:30.000000 decoder-plus-plus-1.7.0/tests/plugins/zlib_test.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-07 11:36:23.990036 decoder-plus-plus-1.7.0/tests/ui/
+-rw-rw-r--   0 tom       (1000) tom       (1000)        0 2023-01-15 14:39:42.000000 decoder-plus-plus-1.7.0/tests/ui/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     8727 2024-04-06 20:29:29.000000 decoder-plus-plus-1.7.0/tests/ui/classic_mode_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      512 2023-01-15 15:28:09.000000 decoder-plus-plus-1.7.0/tests/utils.py
```

### Comparing `decoder-plus-plus-1.5.0/LICENSE` & `decoder-plus-plus-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.5.0/PKG-INFO` & `decoder-plus-plus-1.7.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,52 +1,36 @@
-Metadata-Version: 2.1
-Name: decoder-plus-plus
-Version: 1.5.0
-Summary: An extensible application for penetration testers and software developers to decode/encode data into various formats.
-Home-page: https://github.com/bytebutcher/decoder-plus-plus
-Author: bytebutcher
-Author-email: thomas.engel.web@gmail.com
-License: GPL-3.0
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-Provides-Extra: qt5
-Provides-Extra: qt6
-Provides-Extra: extras
-License-File: LICENSE
-
 ![Decoder++ Logo](https://raw.githubusercontent.com/bytebutcher/decoder-plus-plus/master/images/dpp.png)
 
 <a href="https://pypi.python.org/pypi/decoder-plus-plus"><img src="https://img.shields.io/pypi/v/decoder-plus-plus.svg"></a>
 <a href="https://pypi.python.org/pypi/decoder-plus-plus"><img src="https://img.shields.io/pypi/dm/decoder-plus-plus"></a>
 <a href="https://pypi.python.org/pypi/decoder-plus-plus"><img src="https://img.shields.io/pypi/pyversions/decoder-plus-plus.svg"></a>
 
 # Decoder++
 
-An extensible application for penetration testers and software developers to decode/encode data into various formats.
+Decoder++ is an extensible application designed for penetration testers, software developers, 
+and anyone in between looking to effortlessly decode and encode data across various formats. 
+It includes a wide range of preinstalled scripts and codecs, smart decoding and format identification, 
+and supports both graphical user interface (GUI) and command-line interface (CLI) operations.
 
-## Setup
+## Quick Start
 
-To install ```Decoder++``` simply use ```pip```:
+Get up and running with Decoder++ in just a few steps:
 
 ```bash
 # Install using pip (latest:qt6)
 pip3 install decoder-plus-plus[qt6]
 
-# Install using pip (backport:qt5)
+# Or, for a qt5 backport:
 pip3 install decoder-plus-plus[qt5]
-```
 
-Note, that this will install ```Decoder++``` and the most common plugins.
-In order to install and use all available plugins the package ```decoder-plus-plus[extras]``` needs to be installed:
-```
+# To leverage all features and plugins:
 pip3 install decoder-plus-plus[extras]
 ```
 
-Please refer to the [Installation Guide](docs/INSTALL.md) for more information regarding individual setups. 
+For a detailed installation guide, including platform-specific instructions, see the [Installation Guide](docs/INSTALL.md).
 
 ## Overview
 
 This section provides an overview about the individual ways of interacting with
 ```Decoder++```. For additional usage information check out the ```Advanced Usage``` section.
 
 ### Graphical User Interface
@@ -67,34 +51,40 @@
 
 In addition to the graphical user interface Decoder++ also provides a command line interface:
 ```bash
 $ dpp -e base64 -h sha1 "Hello, world!"
 e52d74c6d046c390345ae4343406b99587f2af0d
 ```
 
-### Features
+### Codecs and Scripts
+
+```Decoder++``` allows you to choose from a variety of codecs and scripts:
+
+* **Encode/Decode:**
+  - Base16, Base32, Base45, Base64, Base64 (URL-safe)
+  - Binary, Gzip, Hex, Html, JWT, HTTP64
+  - Octal, Url, Url+, Zlib
+* **Hashing:** 
+  - Adler-32, Apache-Md5, CRC32, FreeBSD-NT
+  - Keccak224, Keccak256, Keccak384, Keccak512
+  - LM, Md2, Md4, Md5, NT, PHPass
+  - RipeMd160, Sha1, Sha3 224, Sha3 256, Sha3 384, Sha3 512
+  - Sha224, Sha256, Sha348, Sha512, Sun Md5
+* **Scripts:**
+  - Caesar, CSS-Minify, Custom Code, Extract URLs, Filter-Lines
+  - Identify File Format, Identify Hash Format, JS-Beautifier, JS-to-XML, JQ
+  - JSONify, JSONPath, HTML-Beautifier
+  - Little/Big-Endian Transform, Reformat Text, Remove Newlines, Remove Whitespaces
+  - Search and Replace, Split and Rejoin, Unescape/Escape String, XPath
+
 
-* User Interfaces:
-    * Graphical User Interface
-    * Command Line Interface
-* Preinstalled Scripts and Codecs:
-    * **Encode/Decode:** Base16, Base32, Base45, Base64, Base64 (URL-safe), Binary, Gzip, Hex, Html, JWT, HTTP64, Octal, Url, Url+, Zlib
-    * **Hashing:** Adler-32, Apache-Md5, CRC32, FreeBSD-NT, Keccak224, Keccak256, Keccak384, Keccak512, LM, Md2, Md4,
-        Md5, NT, PHPass, RipeMd160, Sha1, Sha3 224, Sha3 256, Sha3 384, Sha3 512, Sha224, Sha256, Sha348, Sha512,
-        Sun Md5
-    * **Scripts:** CSS-Minify, Caesar, Extract URLs, Filter-Lines, Identify File Format, Identify Hash Format, JS-Beautifier, JS-to-XML, JQ, JSONify, JSONPath, HTML-Beautifier, Little/Big-Endian Transform, Reformat Text, Remove Newlines, Remove Whitespaces, Search and Replace, Split and Rejoin, Unescape/Escape String, XPath
-* Format-Identification
-* Smart-Decode
-* Plugin System
-* Load & Save Current Session
-* Supported Platforms:
-    * Windows
-    * Linux
-    * MAC
+In cases where you require a bit more flexibility ```Decoder++``` allows you to process your data with 
+custom scripts by using the ```Custom Code``` script:
 
+![Decoder++ Screenshot](https://raw.githubusercontent.com/bytebutcher/decoder-plus-plus/master/images/dpp-custom-code-script.png)
 
 ## Advanced Usage
 
 This section provides additional information about how the command line interface can be used.
 
 ### Command Line Interface
```

#### html2text {}

```diff
@@ -1,55 +1,51 @@
-Metadata-Version: 2.1 Name: decoder-plus-plus Version: 1.5.0 Summary: An
-extensible application for penetration testers and software developers to
-decode/encode data into various formats. Home-page: https://github.com/
-bytebutcher/decoder-plus-plus Author: bytebutcher Author-email:
-thomas.engel.web@gmail.com License: GPL-3.0 Classifier: Programming Language ::
-Python :: 3 Classifier: Operating System :: OS Independent Description-Content-
-Type: text/markdown Provides-Extra: qt5 Provides-Extra: qt6 Provides-Extra:
-extras License-File: LICENSE ![Decoder++ Logo](https://
-raw.githubusercontent.com/bytebutcher/decoder-plus-plus/master/images/dpp.png)
-_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_v_/_d_e_c_o_d_e_r_-_p_l_u_s_-_p_l_u_s_._s_v_g_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
-_p_y_p_i_/_d_m_/_d_e_c_o_d_e_r_-_p_l_u_s_-_p_l_u_s_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_p_y_v_e_r_s_i_o_n_s_/_d_e_c_o_d_e_r_-_p_l_u_s_-
-_p_l_u_s_._s_v_g_]# Decoder++ An extensible application for penetration testers and
-software developers to decode/encode data into various formats. ## Setup To
-install ```Decoder++``` simply use ```pip```: ```bash # Install using pip
-(latest:qt6) pip3 install decoder-plus-plus[qt6] # Install using pip (backport:
-qt5) pip3 install decoder-plus-plus[qt5] ``` Note, that this will install
-```Decoder++``` and the most common plugins. In order to install and use all
-available plugins the package ```decoder-plus-plus[extras]``` needs to be
-installed: ``` pip3 install decoder-plus-plus[extras] ``` Please refer to the
-[Installation Guide](docs/INSTALL.md) for more information regarding individual
-setups. ## Overview This section provides an overview about the individual ways
-of interacting with ```Decoder++```. For additional usage information check out
-the ```Advanced Usage``` section. ### Graphical User Interface The graphical
-user interface provides two distinct interaction modes: a ```main-window-
-mode``` and a ```dialog-mode```. ![Decoder++ Screenshot](https://
-raw.githubusercontent.com/bytebutcher/decoder-plus-plus/master/images/dpp-
-preview-001.png) While the ```main-window-mode``` supports tabbing, the
-```dialog-mode``` has the ability to return the transformed content to
-```stdout``` ready for further processing. As a result ```Decoder++``` can
-enhance other tools/scripts by providing a graphical user interface for
-flexible transformation of any input. ![Decoder++ Screenshot](https://
-raw.githubusercontent.com/bytebutcher/decoder-plus-plus/master/images/dpp-
-preview-dialog.png) ### Command Line In addition to the graphical user
+![Decoder++ Logo](https://raw.githubusercontent.com/bytebutcher/decoder-plus-
+plus/master/images/dpp.png) _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_v_/_d_e_c_o_d_e_r_-_p_l_u_s_-
+_p_l_u_s_._s_v_g_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_d_m_/_d_e_c_o_d_e_r_-_p_l_u_s_-_p_l_u_s_]_[_h_t_t_p_s_:_/_/
+_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_p_y_v_e_r_s_i_o_n_s_/_d_e_c_o_d_e_r_-_p_l_u_s_-_p_l_u_s_._s_v_g_]# Decoder++ Decoder++ is
+an extensible application designed for penetration testers, software
+developers, and anyone in between looking to effortlessly decode and encode
+data across various formats. It includes a wide range of preinstalled scripts
+and codecs, smart decoding and format identification, and supports both
+graphical user interface (GUI) and command-line interface (CLI) operations. ##
+Quick Start Get up and running with Decoder++ in just a few steps: ```bash #
+Install using pip (latest:qt6) pip3 install decoder-plus-plus[qt6] # Or, for a
+qt5 backport: pip3 install decoder-plus-plus[qt5] # To leverage all features
+and plugins: pip3 install decoder-plus-plus[extras] ``` For a detailed
+installation guide, including platform-specific instructions, see the
+[Installation Guide](docs/INSTALL.md). ## Overview This section provides an
+overview about the individual ways of interacting with ```Decoder++```. For
+additional usage information check out the ```Advanced Usage``` section. ###
+Graphical User Interface The graphical user interface provides two distinct
+interaction modes: a ```main-window-mode``` and a ```dialog-mode```. !
+[Decoder++ Screenshot](https://raw.githubusercontent.com/bytebutcher/decoder-
+plus-plus/master/images/dpp-preview-001.png) While the ```main-window-mode```
+supports tabbing, the ```dialog-mode``` has the ability to return the
+transformed content to ```stdout``` ready for further processing. As a result
+```Decoder++``` can enhance other tools/scripts by providing a graphical user
+interface for flexible transformation of any input. ![Decoder++ Screenshot]
+(https://raw.githubusercontent.com/bytebutcher/decoder-plus-plus/master/images/
+dpp-preview-dialog.png) ### Command Line In addition to the graphical user
 interface Decoder++ also provides a command line interface: ```bash $ dpp -
 e base64 -h sha1 "Hello, world!" e52d74c6d046c390345ae4343406b99587f2af0d ```
-### Features * User Interfaces: * Graphical User Interface * Command Line
-Interface * Preinstalled Scripts and Codecs: * **Encode/Decode:** Base16,
-Base32, Base45, Base64, Base64 (URL-safe), Binary, Gzip, Hex, Html, JWT,
-HTTP64, Octal, Url, Url+, Zlib * **Hashing:** Adler-32, Apache-Md5, CRC32,
-FreeBSD-NT, Keccak224, Keccak256, Keccak384, Keccak512, LM, Md2, Md4, Md5, NT,
-PHPass, RipeMd160, Sha1, Sha3 224, Sha3 256, Sha3 384, Sha3 512, Sha224,
-Sha256, Sha348, Sha512, Sun Md5 * **Scripts:** CSS-Minify, Caesar, Extract
-URLs, Filter-Lines, Identify File Format, Identify Hash Format, JS-Beautifier,
-JS-to-XML, JQ, JSONify, JSONPath, HTML-Beautifier, Little/Big-Endian Transform,
-Reformat Text, Remove Newlines, Remove Whitespaces, Search and Replace, Split
-and Rejoin, Unescape/Escape String, XPath * Format-Identification * Smart-
-Decode * Plugin System * Load & Save Current Session * Supported Platforms: *
-Windows * Linux * MAC ## Advanced Usage This section provides additional
+### Codecs and Scripts ```Decoder++``` allows you to choose from a variety of
+codecs and scripts: * **Encode/Decode:** - Base16, Base32, Base45, Base64,
+Base64 (URL-safe) - Binary, Gzip, Hex, Html, JWT, HTTP64 - Octal, Url, Url+,
+Zlib * **Hashing:** - Adler-32, Apache-Md5, CRC32, FreeBSD-NT - Keccak224,
+Keccak256, Keccak384, Keccak512 - LM, Md2, Md4, Md5, NT, PHPass - RipeMd160,
+Sha1, Sha3 224, Sha3 256, Sha3 384, Sha3 512 - Sha224, Sha256, Sha348, Sha512,
+Sun Md5 * **Scripts:** - Caesar, CSS-Minify, Custom Code, Extract URLs, Filter-
+Lines - Identify File Format, Identify Hash Format, JS-Beautifier, JS-to-XML,
+JQ - JSONify, JSONPath, HTML-Beautifier - Little/Big-Endian Transform, Reformat
+Text, Remove Newlines, Remove Whitespaces - Search and Replace, Split and
+Rejoin, Unescape/Escape String, XPath In cases where you require a bit more
+flexibility ```Decoder++``` allows you to process your data with custom scripts
+by using the ```Custom Code``` script: ![Decoder++ Screenshot](https://
+raw.githubusercontent.com/bytebutcher/decoder-plus-plus/master/images/dpp-
+custom-code-script.png) ## Advanced Usage This section provides additional
 information about how the command line interface can be used. ### Command Line
 Interface The commandline interface gives easy access to all available codecs.
 To list them the ```-l``` argument can be used. To narrow down the search the
 ```-l``` argument accepts additional parameters which work as filter: ```bash $
 dpp -l base enc Codec Type ----- ---- base16 encoder base32 encoder base64
 encoder ``` ```Decoder++``` distinguishes between encoders, decoders, hashers
 and scripts. Like the graphical user interface the command line interface
```

### Comparing `decoder-plus-plus-1.5.0/README.md` & `decoder-plus-plus-1.7.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,36 +1,53 @@
+Metadata-Version: 2.1
+Name: decoder-plus-plus
+Version: 1.7.0
+Summary: An extensible application for penetration testers and software developers to decode/encode data into various formats.
+Home-page: https://github.com/bytebutcher/decoder-plus-plus
+Author: bytebutcher
+Author-email: thomas.engel.web@gmail.com
+License: GPL-3.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+Provides-Extra: qt5
+Provides-Extra: qt6
+Provides-Extra: extras
+Provides-Extra: test
+License-File: LICENSE
+
 ![Decoder++ Logo](https://raw.githubusercontent.com/bytebutcher/decoder-plus-plus/master/images/dpp.png)
 
 <a href="https://pypi.python.org/pypi/decoder-plus-plus"><img src="https://img.shields.io/pypi/v/decoder-plus-plus.svg"></a>
 <a href="https://pypi.python.org/pypi/decoder-plus-plus"><img src="https://img.shields.io/pypi/dm/decoder-plus-plus"></a>
 <a href="https://pypi.python.org/pypi/decoder-plus-plus"><img src="https://img.shields.io/pypi/pyversions/decoder-plus-plus.svg"></a>
 
 # Decoder++
 
-An extensible application for penetration testers and software developers to decode/encode data into various formats.
+Decoder++ is an extensible application designed for penetration testers, software developers, 
+and anyone in between looking to effortlessly decode and encode data across various formats. 
+It includes a wide range of preinstalled scripts and codecs, smart decoding and format identification, 
+and supports both graphical user interface (GUI) and command-line interface (CLI) operations.
 
-## Setup
+## Quick Start
 
-To install ```Decoder++``` simply use ```pip```:
+Get up and running with Decoder++ in just a few steps:
 
 ```bash
 # Install using pip (latest:qt6)
 pip3 install decoder-plus-plus[qt6]
 
-# Install using pip (backport:qt5)
+# Or, for a qt5 backport:
 pip3 install decoder-plus-plus[qt5]
-```
 
-Note, that this will install ```Decoder++``` and the most common plugins.
-In order to install and use all available plugins the package ```decoder-plus-plus[extras]``` needs to be installed:
-```
+# To leverage all features and plugins:
 pip3 install decoder-plus-plus[extras]
 ```
 
-Please refer to the [Installation Guide](docs/INSTALL.md) for more information regarding individual setups. 
+For a detailed installation guide, including platform-specific instructions, see the [Installation Guide](docs/INSTALL.md).
 
 ## Overview
 
 This section provides an overview about the individual ways of interacting with
 ```Decoder++```. For additional usage information check out the ```Advanced Usage``` section.
 
 ### Graphical User Interface
@@ -51,34 +68,40 @@
 
 In addition to the graphical user interface Decoder++ also provides a command line interface:
 ```bash
 $ dpp -e base64 -h sha1 "Hello, world!"
 e52d74c6d046c390345ae4343406b99587f2af0d
 ```
 
-### Features
+### Codecs and Scripts
+
+```Decoder++``` allows you to choose from a variety of codecs and scripts:
+
+* **Encode/Decode:**
+  - Base16, Base32, Base45, Base64, Base64 (URL-safe)
+  - Binary, Gzip, Hex, Html, JWT, HTTP64
+  - Octal, Url, Url+, Zlib
+* **Hashing:** 
+  - Adler-32, Apache-Md5, CRC32, FreeBSD-NT
+  - Keccak224, Keccak256, Keccak384, Keccak512
+  - LM, Md2, Md4, Md5, NT, PHPass
+  - RipeMd160, Sha1, Sha3 224, Sha3 256, Sha3 384, Sha3 512
+  - Sha224, Sha256, Sha348, Sha512, Sun Md5
+* **Scripts:**
+  - Caesar, CSS-Minify, Custom Code, Extract URLs, Filter-Lines
+  - Identify File Format, Identify Hash Format, JS-Beautifier, JS-to-XML, JQ
+  - JSONify, JSONPath, HTML-Beautifier
+  - Little/Big-Endian Transform, Reformat Text, Remove Newlines, Remove Whitespaces
+  - Search and Replace, Split and Rejoin, Unescape/Escape String, XPath
+
 
-* User Interfaces:
-    * Graphical User Interface
-    * Command Line Interface
-* Preinstalled Scripts and Codecs:
-    * **Encode/Decode:** Base16, Base32, Base45, Base64, Base64 (URL-safe), Binary, Gzip, Hex, Html, JWT, HTTP64, Octal, Url, Url+, Zlib
-    * **Hashing:** Adler-32, Apache-Md5, CRC32, FreeBSD-NT, Keccak224, Keccak256, Keccak384, Keccak512, LM, Md2, Md4,
-        Md5, NT, PHPass, RipeMd160, Sha1, Sha3 224, Sha3 256, Sha3 384, Sha3 512, Sha224, Sha256, Sha348, Sha512,
-        Sun Md5
-    * **Scripts:** CSS-Minify, Caesar, Extract URLs, Filter-Lines, Identify File Format, Identify Hash Format, JS-Beautifier, JS-to-XML, JQ, JSONify, JSONPath, HTML-Beautifier, Little/Big-Endian Transform, Reformat Text, Remove Newlines, Remove Whitespaces, Search and Replace, Split and Rejoin, Unescape/Escape String, XPath
-* Format-Identification
-* Smart-Decode
-* Plugin System
-* Load & Save Current Session
-* Supported Platforms:
-    * Windows
-    * Linux
-    * MAC
+In cases where you require a bit more flexibility ```Decoder++``` allows you to process your data with 
+custom scripts by using the ```Custom Code``` script:
 
+![Decoder++ Screenshot](https://raw.githubusercontent.com/bytebutcher/decoder-plus-plus/master/images/dpp-custom-code-script.png)
 
 ## Advanced Usage
 
 This section provides additional information about how the command line interface can be used.
 
 ### Command Line Interface
```

#### html2text {}

```diff
@@ -1,86 +1,98 @@
-![Decoder++ Logo](https://raw.githubusercontent.com/bytebutcher/decoder-plus-
-plus/master/images/dpp.png) _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_v_/_d_e_c_o_d_e_r_-_p_l_u_s_-
-_p_l_u_s_._s_v_g_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_d_m_/_d_e_c_o_d_e_r_-_p_l_u_s_-_p_l_u_s_]_[_h_t_t_p_s_:_/_/
-_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_p_y_v_e_r_s_i_o_n_s_/_d_e_c_o_d_e_r_-_p_l_u_s_-_p_l_u_s_._s_v_g_]# Decoder++ An extensible
-application for penetration testers and software developers to decode/encode
-data into various formats. ## Setup To install ```Decoder++``` simply use
-```pip```: ```bash # Install using pip (latest:qt6) pip3 install decoder-plus-
-plus[qt6] # Install using pip (backport:qt5) pip3 install decoder-plus-plus
-[qt5] ``` Note, that this will install ```Decoder++``` and the most common
-plugins. In order to install and use all available plugins the package
-```decoder-plus-plus[extras]``` needs to be installed: ``` pip3 install
-decoder-plus-plus[extras] ``` Please refer to the [Installation Guide](docs/
-INSTALL.md) for more information regarding individual setups. ## Overview This
-section provides an overview about the individual ways of interacting with
-```Decoder++```. For additional usage information check out the ```Advanced
-Usage``` section. ### Graphical User Interface The graphical user interface
-provides two distinct interaction modes: a ```main-window-mode``` and a
-```dialog-mode```. ![Decoder++ Screenshot](https://raw.githubusercontent.com/
-bytebutcher/decoder-plus-plus/master/images/dpp-preview-001.png) While the
-```main-window-mode``` supports tabbing, the ```dialog-mode``` has the ability
-to return the transformed content to ```stdout``` ready for further processing.
-As a result ```Decoder++``` can enhance other tools/scripts by providing a
-graphical user interface for flexible transformation of any input. ![Decoder++
-Screenshot](https://raw.githubusercontent.com/bytebutcher/decoder-plus-plus/
-master/images/dpp-preview-dialog.png) ### Command Line In addition to the
-graphical user interface Decoder++ also provides a command line interface:
-```bash $ dpp -e base64 -h sha1 "Hello, world!"
-e52d74c6d046c390345ae4343406b99587f2af0d ``` ### Features * User Interfaces: *
-Graphical User Interface * Command Line Interface * Preinstalled Scripts and
-Codecs: * **Encode/Decode:** Base16, Base32, Base45, Base64, Base64 (URL-safe),
-Binary, Gzip, Hex, Html, JWT, HTTP64, Octal, Url, Url+, Zlib * **Hashing:**
-Adler-32, Apache-Md5, CRC32, FreeBSD-NT, Keccak224, Keccak256, Keccak384,
-Keccak512, LM, Md2, Md4, Md5, NT, PHPass, RipeMd160, Sha1, Sha3 224, Sha3 256,
-Sha3 384, Sha3 512, Sha224, Sha256, Sha348, Sha512, Sun Md5 * **Scripts:** CSS-
-Minify, Caesar, Extract URLs, Filter-Lines, Identify File Format, Identify Hash
-Format, JS-Beautifier, JS-to-XML, JQ, JSONify, JSONPath, HTML-Beautifier,
-Little/Big-Endian Transform, Reformat Text, Remove Newlines, Remove
-Whitespaces, Search and Replace, Split and Rejoin, Unescape/Escape String,
-XPath * Format-Identification * Smart-Decode * Plugin System * Load & Save
-Current Session * Supported Platforms: * Windows * Linux * MAC ## Advanced
-Usage This section provides additional information about how the command line
-interface can be used. ### Command Line Interface The commandline interface
-gives easy access to all available codecs. To list them the ```-l``` argument
-can be used. To narrow down the search the ```-l``` argument accepts additional
-parameters which work as filter: ```bash $ dpp -l base enc Codec Type ----- ---
-- base16 encoder base32 encoder base64 encoder ``` ```Decoder++```
-distinguishes between encoders, decoders, hashers and scripts. Like the
-graphical user interface the command line interface allows the usage of
-multiple codecs in a row: ```bash $ dpp "H4sIAAXmeVsC//NIzcnJ11Eozy/
-KSVEEAObG5usNAAAA" -d base64 -d gzip Hello, world! ``` While encoders, decoders
-and hashers can be used right away, some scripts may require additional
-configuration. To show all available options of a specific script add the
-```help``` parameter: ``` $ dpp "Hello, world!" -s split_and_rejoin help Split
-& Rejoin ============== Name Value Group Required Description ---- ----- ----
-- -------- ----------- split_by_chars split_behaviour yes the chars used at
-which to split the text split_by_length 0 split_behaviour yes the length used
-at which to split the text rejoin_with_chars yes the chars used to join the
-splitted text ``` To configure a specific script the individual options need to
-be supplied as name-value pairs (e.g. ```search_term="Hello"```): ``` $ dpp
-"Hello, world!" -s search_and_replace search_term="Hello" replace_term="Hey"
-Hey, world! ``` ## Contribute Feel free to open a new ticket for requesting
-features or reporting bugs. Also don't hesitate to issue a pull-request for new
-features/plugins. More information regarding Decoder++ development can be found
-in the [Development Guide](docs/DEVELOPMENT.md). Thanks to * Tim Menapace
-(RIPEMD160, KECCAK256) * Robin Krumnow (ROT13) ## Troubleshooting ### Signals
-are not working on Mac OS When starting ```Decoder++``` in Mac OS signals are
-not working. This might happen when ```PyQt6``` is installed using homebrew.
-### Can not start Decoder++ in Windows using CygWin When starting
-```Decoder++``` in ```CygWin``` an error occurs: ``` ModuleNotFoundError: No
-module named 'PyQt6' ``` This might happen even if ```PyQt6``` is installed
-using pip. Currently there is no fix for that. Instead it is recommended to
-start ```Decoder++``` using the Windows command line. ### No Module PyQt6 When
-starting ```Decoder++``` the error ```No module named 'PyQt6.sig'``` is
-displayed on the console. This may happen when there are competing versions of
-PyQt6 installed. Reinstalling PyQt6 should fix this error. ``` $ sudo pip3
-uninstall PyQt6 $ sudo pip3 install PyQt6 ``` ### Missing Qt6 libraries At
-least in Ubuntu 22.04 it might be necessary to install the following packages
-using ```apt```: ``` apt install libqt6core6 libqt6network6
-libqt6openglwidgets6 libqt6widgets6 ``` ### X11-forwarding fails In order to
-run dpp inside a container/virtual machine you may need to install the ```qt6-
-qpa-plugins``` inside the container/virtual machine and configure the
-```QT_QPA_PLATFORM_PLUGIN_PATH``` accordingly: ``` apt install qt6-qpa-plugins
-export QT_QPA_PLATFORM_PLUGIN_PATH=/usr/lib/x86_64-linux-gnu/qt6/plugins/
-platforms/ ``` See the _D_o_c_k_e_r_ _b_u_i_l_d_ _a_n_d_ _r_u_n_ _s_c_r_i_p_t_s for more information
-regarding how to build and run a Decoder++ Docker container. ## Inspired By *
-PortSwigger's Burp Decoder ## Powered By * QtPy / PyQt5 / PyQt6 * QtAwesome
+Metadata-Version: 2.1 Name: decoder-plus-plus Version: 1.7.0 Summary: An
+extensible application for penetration testers and software developers to
+decode/encode data into various formats. Home-page: https://github.com/
+bytebutcher/decoder-plus-plus Author: bytebutcher Author-email:
+thomas.engel.web@gmail.com License: GPL-3.0 Classifier: Programming Language ::
+Python :: 3 Classifier: Operating System :: OS Independent Description-Content-
+Type: text/markdown Provides-Extra: qt5 Provides-Extra: qt6 Provides-Extra:
+extras Provides-Extra: test License-File: LICENSE ![Decoder++ Logo](https://
+raw.githubusercontent.com/bytebutcher/decoder-plus-plus/master/images/dpp.png)
+_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_v_/_d_e_c_o_d_e_r_-_p_l_u_s_-_p_l_u_s_._s_v_g_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
+_p_y_p_i_/_d_m_/_d_e_c_o_d_e_r_-_p_l_u_s_-_p_l_u_s_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_p_y_v_e_r_s_i_o_n_s_/_d_e_c_o_d_e_r_-_p_l_u_s_-
+_p_l_u_s_._s_v_g_]# Decoder++ Decoder++ is an extensible application designed for
+penetration testers, software developers, and anyone in between looking to
+effortlessly decode and encode data across various formats. It includes a wide
+range of preinstalled scripts and codecs, smart decoding and format
+identification, and supports both graphical user interface (GUI) and command-
+line interface (CLI) operations. ## Quick Start Get up and running with
+Decoder++ in just a few steps: ```bash # Install using pip (latest:qt6) pip3
+install decoder-plus-plus[qt6] # Or, for a qt5 backport: pip3 install decoder-
+plus-plus[qt5] # To leverage all features and plugins: pip3 install decoder-
+plus-plus[extras] ``` For a detailed installation guide, including platform-
+specific instructions, see the [Installation Guide](docs/INSTALL.md). ##
+Overview This section provides an overview about the individual ways of
+interacting with ```Decoder++```. For additional usage information check out
+the ```Advanced Usage``` section. ### Graphical User Interface The graphical
+user interface provides two distinct interaction modes: a ```main-window-
+mode``` and a ```dialog-mode```. ![Decoder++ Screenshot](https://
+raw.githubusercontent.com/bytebutcher/decoder-plus-plus/master/images/dpp-
+preview-001.png) While the ```main-window-mode``` supports tabbing, the
+```dialog-mode``` has the ability to return the transformed content to
+```stdout``` ready for further processing. As a result ```Decoder++``` can
+enhance other tools/scripts by providing a graphical user interface for
+flexible transformation of any input. ![Decoder++ Screenshot](https://
+raw.githubusercontent.com/bytebutcher/decoder-plus-plus/master/images/dpp-
+preview-dialog.png) ### Command Line In addition to the graphical user
+interface Decoder++ also provides a command line interface: ```bash $ dpp -
+e base64 -h sha1 "Hello, world!" e52d74c6d046c390345ae4343406b99587f2af0d ```
+### Codecs and Scripts ```Decoder++``` allows you to choose from a variety of
+codecs and scripts: * **Encode/Decode:** - Base16, Base32, Base45, Base64,
+Base64 (URL-safe) - Binary, Gzip, Hex, Html, JWT, HTTP64 - Octal, Url, Url+,
+Zlib * **Hashing:** - Adler-32, Apache-Md5, CRC32, FreeBSD-NT - Keccak224,
+Keccak256, Keccak384, Keccak512 - LM, Md2, Md4, Md5, NT, PHPass - RipeMd160,
+Sha1, Sha3 224, Sha3 256, Sha3 384, Sha3 512 - Sha224, Sha256, Sha348, Sha512,
+Sun Md5 * **Scripts:** - Caesar, CSS-Minify, Custom Code, Extract URLs, Filter-
+Lines - Identify File Format, Identify Hash Format, JS-Beautifier, JS-to-XML,
+JQ - JSONify, JSONPath, HTML-Beautifier - Little/Big-Endian Transform, Reformat
+Text, Remove Newlines, Remove Whitespaces - Search and Replace, Split and
+Rejoin, Unescape/Escape String, XPath In cases where you require a bit more
+flexibility ```Decoder++``` allows you to process your data with custom scripts
+by using the ```Custom Code``` script: ![Decoder++ Screenshot](https://
+raw.githubusercontent.com/bytebutcher/decoder-plus-plus/master/images/dpp-
+custom-code-script.png) ## Advanced Usage This section provides additional
+information about how the command line interface can be used. ### Command Line
+Interface The commandline interface gives easy access to all available codecs.
+To list them the ```-l``` argument can be used. To narrow down the search the
+```-l``` argument accepts additional parameters which work as filter: ```bash $
+dpp -l base enc Codec Type ----- ---- base16 encoder base32 encoder base64
+encoder ``` ```Decoder++``` distinguishes between encoders, decoders, hashers
+and scripts. Like the graphical user interface the command line interface
+allows the usage of multiple codecs in a row: ```bash $ dpp "H4sIAAXmeVsC//
+NIzcnJ11Eozy/KSVEEAObG5usNAAAA" -d base64 -d gzip Hello, world! ``` While
+encoders, decoders and hashers can be used right away, some scripts may require
+additional configuration. To show all available options of a specific script
+add the ```help``` parameter: ``` $ dpp "Hello, world!" -s split_and_rejoin
+help Split & Rejoin ============== Name Value Group Required Description ---- -
+---- ----- -------- ----------- split_by_chars split_behaviour yes the chars
+used at which to split the text split_by_length 0 split_behaviour yes the
+length used at which to split the text rejoin_with_chars yes the chars used to
+join the splitted text ``` To configure a specific script the individual
+options need to be supplied as name-value pairs (e.g.
+```search_term="Hello"```): ``` $ dpp "Hello, world!" -s search_and_replace
+search_term="Hello" replace_term="Hey" Hey, world! ``` ## Contribute Feel free
+to open a new ticket for requesting features or reporting bugs. Also don't
+hesitate to issue a pull-request for new features/plugins. More information
+regarding Decoder++ development can be found in the [Development Guide](docs/
+DEVELOPMENT.md). Thanks to * Tim Menapace (RIPEMD160, KECCAK256) * Robin
+Krumnow (ROT13) ## Troubleshooting ### Signals are not working on Mac OS When
+starting ```Decoder++``` in Mac OS signals are not working. This might happen
+when ```PyQt6``` is installed using homebrew. ### Can not start Decoder++ in
+Windows using CygWin When starting ```Decoder++``` in ```CygWin``` an error
+occurs: ``` ModuleNotFoundError: No module named 'PyQt6' ``` This might happen
+even if ```PyQt6``` is installed using pip. Currently there is no fix for that.
+Instead it is recommended to start ```Decoder++``` using the Windows command
+line. ### No Module PyQt6 When starting ```Decoder++``` the error ```No module
+named 'PyQt6.sig'``` is displayed on the console. This may happen when there
+are competing versions of PyQt6 installed. Reinstalling PyQt6 should fix this
+error. ``` $ sudo pip3 uninstall PyQt6 $ sudo pip3 install PyQt6 ``` ###
+Missing Qt6 libraries At least in Ubuntu 22.04 it might be necessary to install
+the following packages using ```apt```: ``` apt install libqt6core6
+libqt6network6 libqt6openglwidgets6 libqt6widgets6 ``` ### X11-forwarding fails
+In order to run dpp inside a container/virtual machine you may need to install
+the ```qt6-qpa-plugins``` inside the container/virtual machine and configure
+the ```QT_QPA_PLATFORM_PLUGIN_PATH``` accordingly: ``` apt install qt6-qpa-
+plugins export QT_QPA_PLATFORM_PLUGIN_PATH=/usr/lib/x86_64-linux-gnu/qt6/
+plugins/platforms/ ``` See the _D_o_c_k_e_r_ _b_u_i_l_d_ _a_n_d_ _r_u_n_ _s_c_r_i_p_t_s for more
+information regarding how to build and run a Decoder++ Docker container. ##
+Inspired By * PortSwigger's Burp Decoder ## Powered By * QtPy / PyQt5 / PyQt6 *
+QtAwesome
```

### Comparing `decoder-plus-plus-1.5.0/data/dpp.png` & `decoder-plus-plus-1.7.0/dpp/images/dpp_128.png`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.5.0/decoder_plus_plus.egg-info/PKG-INFO` & `decoder-plus-plus-1.7.0/decoder_plus_plus.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,52 +1,53 @@
 Metadata-Version: 2.1
 Name: decoder-plus-plus
-Version: 1.5.0
+Version: 1.7.0
 Summary: An extensible application for penetration testers and software developers to decode/encode data into various formats.
 Home-page: https://github.com/bytebutcher/decoder-plus-plus
 Author: bytebutcher
 Author-email: thomas.engel.web@gmail.com
 License: GPL-3.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Provides-Extra: qt5
 Provides-Extra: qt6
 Provides-Extra: extras
+Provides-Extra: test
 License-File: LICENSE
 
 ![Decoder++ Logo](https://raw.githubusercontent.com/bytebutcher/decoder-plus-plus/master/images/dpp.png)
 
 <a href="https://pypi.python.org/pypi/decoder-plus-plus"><img src="https://img.shields.io/pypi/v/decoder-plus-plus.svg"></a>
 <a href="https://pypi.python.org/pypi/decoder-plus-plus"><img src="https://img.shields.io/pypi/dm/decoder-plus-plus"></a>
 <a href="https://pypi.python.org/pypi/decoder-plus-plus"><img src="https://img.shields.io/pypi/pyversions/decoder-plus-plus.svg"></a>
 
 # Decoder++
 
-An extensible application for penetration testers and software developers to decode/encode data into various formats.
+Decoder++ is an extensible application designed for penetration testers, software developers, 
+and anyone in between looking to effortlessly decode and encode data across various formats. 
+It includes a wide range of preinstalled scripts and codecs, smart decoding and format identification, 
+and supports both graphical user interface (GUI) and command-line interface (CLI) operations.
 
-## Setup
+## Quick Start
 
-To install ```Decoder++``` simply use ```pip```:
+Get up and running with Decoder++ in just a few steps:
 
 ```bash
 # Install using pip (latest:qt6)
 pip3 install decoder-plus-plus[qt6]
 
-# Install using pip (backport:qt5)
+# Or, for a qt5 backport:
 pip3 install decoder-plus-plus[qt5]
-```
 
-Note, that this will install ```Decoder++``` and the most common plugins.
-In order to install and use all available plugins the package ```decoder-plus-plus[extras]``` needs to be installed:
-```
+# To leverage all features and plugins:
 pip3 install decoder-plus-plus[extras]
 ```
 
-Please refer to the [Installation Guide](docs/INSTALL.md) for more information regarding individual setups. 
+For a detailed installation guide, including platform-specific instructions, see the [Installation Guide](docs/INSTALL.md).
 
 ## Overview
 
 This section provides an overview about the individual ways of interacting with
 ```Decoder++```. For additional usage information check out the ```Advanced Usage``` section.
 
 ### Graphical User Interface
@@ -67,34 +68,40 @@
 
 In addition to the graphical user interface Decoder++ also provides a command line interface:
 ```bash
 $ dpp -e base64 -h sha1 "Hello, world!"
 e52d74c6d046c390345ae4343406b99587f2af0d
 ```
 
-### Features
+### Codecs and Scripts
+
+```Decoder++``` allows you to choose from a variety of codecs and scripts:
+
+* **Encode/Decode:**
+  - Base16, Base32, Base45, Base64, Base64 (URL-safe)
+  - Binary, Gzip, Hex, Html, JWT, HTTP64
+  - Octal, Url, Url+, Zlib
+* **Hashing:** 
+  - Adler-32, Apache-Md5, CRC32, FreeBSD-NT
+  - Keccak224, Keccak256, Keccak384, Keccak512
+  - LM, Md2, Md4, Md5, NT, PHPass
+  - RipeMd160, Sha1, Sha3 224, Sha3 256, Sha3 384, Sha3 512
+  - Sha224, Sha256, Sha348, Sha512, Sun Md5
+* **Scripts:**
+  - Caesar, CSS-Minify, Custom Code, Extract URLs, Filter-Lines
+  - Identify File Format, Identify Hash Format, JS-Beautifier, JS-to-XML, JQ
+  - JSONify, JSONPath, HTML-Beautifier
+  - Little/Big-Endian Transform, Reformat Text, Remove Newlines, Remove Whitespaces
+  - Search and Replace, Split and Rejoin, Unescape/Escape String, XPath
+
 
-* User Interfaces:
-    * Graphical User Interface
-    * Command Line Interface
-* Preinstalled Scripts and Codecs:
-    * **Encode/Decode:** Base16, Base32, Base45, Base64, Base64 (URL-safe), Binary, Gzip, Hex, Html, JWT, HTTP64, Octal, Url, Url+, Zlib
-    * **Hashing:** Adler-32, Apache-Md5, CRC32, FreeBSD-NT, Keccak224, Keccak256, Keccak384, Keccak512, LM, Md2, Md4,
-        Md5, NT, PHPass, RipeMd160, Sha1, Sha3 224, Sha3 256, Sha3 384, Sha3 512, Sha224, Sha256, Sha348, Sha512,
-        Sun Md5
-    * **Scripts:** CSS-Minify, Caesar, Extract URLs, Filter-Lines, Identify File Format, Identify Hash Format, JS-Beautifier, JS-to-XML, JQ, JSONify, JSONPath, HTML-Beautifier, Little/Big-Endian Transform, Reformat Text, Remove Newlines, Remove Whitespaces, Search and Replace, Split and Rejoin, Unescape/Escape String, XPath
-* Format-Identification
-* Smart-Decode
-* Plugin System
-* Load & Save Current Session
-* Supported Platforms:
-    * Windows
-    * Linux
-    * MAC
+In cases where you require a bit more flexibility ```Decoder++``` allows you to process your data with 
+custom scripts by using the ```Custom Code``` script:
 
+![Decoder++ Screenshot](https://raw.githubusercontent.com/bytebutcher/decoder-plus-plus/master/images/dpp-custom-code-script.png)
 
 ## Advanced Usage
 
 This section provides additional information about how the command line interface can be used.
 
 ### Command Line Interface
```

#### html2text {}

```diff
@@ -1,55 +1,59 @@
-Metadata-Version: 2.1 Name: decoder-plus-plus Version: 1.5.0 Summary: An
+Metadata-Version: 2.1 Name: decoder-plus-plus Version: 1.7.0 Summary: An
 extensible application for penetration testers and software developers to
 decode/encode data into various formats. Home-page: https://github.com/
 bytebutcher/decoder-plus-plus Author: bytebutcher Author-email:
 thomas.engel.web@gmail.com License: GPL-3.0 Classifier: Programming Language ::
 Python :: 3 Classifier: Operating System :: OS Independent Description-Content-
 Type: text/markdown Provides-Extra: qt5 Provides-Extra: qt6 Provides-Extra:
-extras License-File: LICENSE ![Decoder++ Logo](https://
+extras Provides-Extra: test License-File: LICENSE ![Decoder++ Logo](https://
 raw.githubusercontent.com/bytebutcher/decoder-plus-plus/master/images/dpp.png)
 _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_v_/_d_e_c_o_d_e_r_-_p_l_u_s_-_p_l_u_s_._s_v_g_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
 _p_y_p_i_/_d_m_/_d_e_c_o_d_e_r_-_p_l_u_s_-_p_l_u_s_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_p_y_v_e_r_s_i_o_n_s_/_d_e_c_o_d_e_r_-_p_l_u_s_-
-_p_l_u_s_._s_v_g_]# Decoder++ An extensible application for penetration testers and
-software developers to decode/encode data into various formats. ## Setup To
-install ```Decoder++``` simply use ```pip```: ```bash # Install using pip
-(latest:qt6) pip3 install decoder-plus-plus[qt6] # Install using pip (backport:
-qt5) pip3 install decoder-plus-plus[qt5] ``` Note, that this will install
-```Decoder++``` and the most common plugins. In order to install and use all
-available plugins the package ```decoder-plus-plus[extras]``` needs to be
-installed: ``` pip3 install decoder-plus-plus[extras] ``` Please refer to the
-[Installation Guide](docs/INSTALL.md) for more information regarding individual
-setups. ## Overview This section provides an overview about the individual ways
-of interacting with ```Decoder++```. For additional usage information check out
+_p_l_u_s_._s_v_g_]# Decoder++ Decoder++ is an extensible application designed for
+penetration testers, software developers, and anyone in between looking to
+effortlessly decode and encode data across various formats. It includes a wide
+range of preinstalled scripts and codecs, smart decoding and format
+identification, and supports both graphical user interface (GUI) and command-
+line interface (CLI) operations. ## Quick Start Get up and running with
+Decoder++ in just a few steps: ```bash # Install using pip (latest:qt6) pip3
+install decoder-plus-plus[qt6] # Or, for a qt5 backport: pip3 install decoder-
+plus-plus[qt5] # To leverage all features and plugins: pip3 install decoder-
+plus-plus[extras] ``` For a detailed installation guide, including platform-
+specific instructions, see the [Installation Guide](docs/INSTALL.md). ##
+Overview This section provides an overview about the individual ways of
+interacting with ```Decoder++```. For additional usage information check out
 the ```Advanced Usage``` section. ### Graphical User Interface The graphical
 user interface provides two distinct interaction modes: a ```main-window-
 mode``` and a ```dialog-mode```. ![Decoder++ Screenshot](https://
 raw.githubusercontent.com/bytebutcher/decoder-plus-plus/master/images/dpp-
 preview-001.png) While the ```main-window-mode``` supports tabbing, the
 ```dialog-mode``` has the ability to return the transformed content to
 ```stdout``` ready for further processing. As a result ```Decoder++``` can
 enhance other tools/scripts by providing a graphical user interface for
 flexible transformation of any input. ![Decoder++ Screenshot](https://
 raw.githubusercontent.com/bytebutcher/decoder-plus-plus/master/images/dpp-
 preview-dialog.png) ### Command Line In addition to the graphical user
 interface Decoder++ also provides a command line interface: ```bash $ dpp -
 e base64 -h sha1 "Hello, world!" e52d74c6d046c390345ae4343406b99587f2af0d ```
-### Features * User Interfaces: * Graphical User Interface * Command Line
-Interface * Preinstalled Scripts and Codecs: * **Encode/Decode:** Base16,
-Base32, Base45, Base64, Base64 (URL-safe), Binary, Gzip, Hex, Html, JWT,
-HTTP64, Octal, Url, Url+, Zlib * **Hashing:** Adler-32, Apache-Md5, CRC32,
-FreeBSD-NT, Keccak224, Keccak256, Keccak384, Keccak512, LM, Md2, Md4, Md5, NT,
-PHPass, RipeMd160, Sha1, Sha3 224, Sha3 256, Sha3 384, Sha3 512, Sha224,
-Sha256, Sha348, Sha512, Sun Md5 * **Scripts:** CSS-Minify, Caesar, Extract
-URLs, Filter-Lines, Identify File Format, Identify Hash Format, JS-Beautifier,
-JS-to-XML, JQ, JSONify, JSONPath, HTML-Beautifier, Little/Big-Endian Transform,
-Reformat Text, Remove Newlines, Remove Whitespaces, Search and Replace, Split
-and Rejoin, Unescape/Escape String, XPath * Format-Identification * Smart-
-Decode * Plugin System * Load & Save Current Session * Supported Platforms: *
-Windows * Linux * MAC ## Advanced Usage This section provides additional
+### Codecs and Scripts ```Decoder++``` allows you to choose from a variety of
+codecs and scripts: * **Encode/Decode:** - Base16, Base32, Base45, Base64,
+Base64 (URL-safe) - Binary, Gzip, Hex, Html, JWT, HTTP64 - Octal, Url, Url+,
+Zlib * **Hashing:** - Adler-32, Apache-Md5, CRC32, FreeBSD-NT - Keccak224,
+Keccak256, Keccak384, Keccak512 - LM, Md2, Md4, Md5, NT, PHPass - RipeMd160,
+Sha1, Sha3 224, Sha3 256, Sha3 384, Sha3 512 - Sha224, Sha256, Sha348, Sha512,
+Sun Md5 * **Scripts:** - Caesar, CSS-Minify, Custom Code, Extract URLs, Filter-
+Lines - Identify File Format, Identify Hash Format, JS-Beautifier, JS-to-XML,
+JQ - JSONify, JSONPath, HTML-Beautifier - Little/Big-Endian Transform, Reformat
+Text, Remove Newlines, Remove Whitespaces - Search and Replace, Split and
+Rejoin, Unescape/Escape String, XPath In cases where you require a bit more
+flexibility ```Decoder++``` allows you to process your data with custom scripts
+by using the ```Custom Code``` script: ![Decoder++ Screenshot](https://
+raw.githubusercontent.com/bytebutcher/decoder-plus-plus/master/images/dpp-
+custom-code-script.png) ## Advanced Usage This section provides additional
 information about how the command line interface can be used. ### Command Line
 Interface The commandline interface gives easy access to all available codecs.
 To list them the ```-l``` argument can be used. To narrow down the search the
 ```-l``` argument accepts additional parameters which work as filter: ```bash $
 dpp -l base enc Codec Type ----- ---- base16 encoder base32 encoder base64
 encoder ``` ```Decoder++``` distinguishes between encoders, decoders, hashers
 and scripts. Like the graphical user interface the command line interface
```

### Comparing `decoder-plus-plus-1.5.0/dpp/__init__.py` & `decoder-plus-plus-1.7.0/dpp/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,12 +12,12 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 __name__ = 'decoder-plus-plus'
-__version__ = '1.5.0'
+__version__ = '1.7.0'
 __author__ = 'bytebutcher'
 
 import os
 app_path = os.path.dirname(os.path.abspath(__file__))
```

### Comparing `decoder-plus-plus-1.5.0/dpp/core/__init__.py` & `decoder-plus-plus-1.7.0/dpp/core/__init__.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.5.0/dpp/core/argparse.py` & `decoder-plus-plus-1.7.0/dpp/core/argparse.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.5.0/dpp/core/assertions.py` & `decoder-plus-plus-1.7.0/dpp/core/assertions.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.5.0/dpp/core/config.py` & `decoder-plus-plus-1.7.0/dpp/core/config.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.5.0/dpp/core/context.py` & `decoder-plus-plus-1.7.0/dpp/core/context.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         TAB_RENAME = "tab_rename"
         TAB_DUPLICATE = "tab_duplicate"
         TAB_NEXT = "tab_next"
         TAB_PREVIOUS = "tab_previous"
         TAB_CLOSE = "tab_close"
         TAB_SELECT_ = "tab_select_{}"
         TAB_SELECT_1 = "tab_select_1"
-        TAB_SELECT_2= "tab_select_2"
+        TAB_SELECT_2 = "tab_select_2"
         TAB_SELECT_3 = "tab_select_3"
         TAB_SELECT_4 = "tab_select_4"
         TAB_SELECT_5 = "tab_select_5"
         TAB_SELECT_6 = "tab_select_6"
         TAB_SELECT_7 = "tab_select_7"
         TAB_SELECT_8 = "tab_select_8"
         TAB_SELECT_9 = "tab_select_9"
@@ -88,22 +88,21 @@
         SELECT_HEX_DOCK = "select_hex_dock"
         SELECT_LOG_DOCK = "select_log_dock"
         TOGGLE_SEARCH_FIELD = "toggle_search_field"
         SHOW_PLUGINS = "show_plugins"
         SHOW_KEYBOARD_SHORTCUTS = "show_keyboard_shortcuts"
         SHOW_ABOUT = "show_about"
 
-    def __init__(self, app_id, app_path, namespace):
+    def __init__(self, app_id, app_path):
         super(__class__, self).__init__()
         self._app_id = app_id
         self._app_path = app_path
-        self._namespace = namespace
         self._trace_mode = False
         self._debug_mode = self.config.isDebugModeEnabled()
-        self._logger = logger.init_logger(self.getLogLevel())
+        self._logger = logger.getLogger(name='dpp', level=self.getLogLevel())
         self._listener = Listener(self)
         self._plugins = None
         self._shortcuts = {}
         self._installed_packages = []
         self._mode = None
 
     @property
@@ -113,15 +112,15 @@
             from dpp.core.config import Config
             self._config = Config()
         return self._config
 
     @property
     def logger(self) -> logging.Logger:
         """ Returns the standard logger for this application. """
-        return logging.getLogger()
+        return self._logger
 
     def getAppName(self) -> str:
         """ Returns the name of the application. """
         return "Decoder++"
 
     def getAppVersion(self) -> str:
         """ Returns the version of the application. """
@@ -153,23 +152,23 @@
 
     def setDebugMode(self, status: bool, temporary=False):
         """ Enables/Disables debug mode. """
         if not temporary:
             self.config.setDebugMode(status)
         self._debug_mode = status
         self._trace_mode = False
-        logger.set_level(logging.DEBUG if status else logging.INFO)
+        self._logger.setLevel(logging.DEBUG if status else logging.INFO)
         status_string = "enabled" if status else "disabled"
         self._logger.info("Debug Mode: {} {}".format(status_string, " (temporary) " if temporary else ""))
 
     def setTraceMode(self, status: bool):
         """ Enables/Disables debug mode. """
         self._trace_mode = status
         self._debug_mode = False
-        logger.set_level(logging.TRACE if status else logging.INFO)
+        self._logger.setLevel(logging.TRACE if status else logging.INFO)
         status_string = 'enabled' if status else 'disabled'
         self._logger.info(f'Trace Mode: {status_string}')
 
     def toggleDebugMode(self):
         """ Toggles the debug-mode on/off. """
         self.setDebugMode(not self.config.isDebugModeEnabled())
 
@@ -257,14 +256,10 @@
             self._logger.error("Shortcut {} is not defined".format(id))
             return NullShortcut()
         return self._shortcuts[id]
 
     def getPluginByName(self, name: str, type: str) -> AbstractPlugin:
         return self.plugins().plugin(name, type)
 
-    def saveAsFile(self, filename: str, content: str):
-        with open(filename, "w") as f:
-            f.write(content)
-
     def __deepcopy__(self, memo):
         """ There shall be only one. """
         return self
```

### Comparing `decoder-plus-plus-1.5.0/dpp/core/decoder_plus_plus.py` & `decoder-plus-plus-1.7.0/dpp/core/decoder_plus_plus.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.5.0/dpp/core/exceptions.py` & `decoder-plus-plus-1.7.0/dpp/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.5.0/dpp/core/icons.py` & `decoder-plus-plus-1.7.0/dpp/core/icons.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 import os
 
 import qtawesome
 from qtpy.QtGui import QIcon
 
 from dpp import app_path
 
-logger = logging.getLogger()
+logger = logging.getLogger(__name__)
 
 
 class Icon:
     EDIT = 'awesome', 'fa.edit'
     FILTER = 'awesome', 'fa.filter'
     SEARCH = 'awesome', 'fa.search'
     CLOSE = 'awesome', 'fa.times'
@@ -41,15 +41,16 @@
     FRAME_REFRESH = 'awesome', 'fa.refresh'
     FRAME_UP = 'awesome', 'fa.chevron-up'
     FRAME_DOWN = 'awesome', 'fa.chevron-down'
     FRAME_RUN = 'awesome', 'fa.play'
     FRAME_PAUSE = 'awesome', 'fa.pause'
     FRAME_CONFIG = 'awesome', 'fa.cog'
     IDENTIFY_CODEC = 'awesome', 'ei.indent-left'
-    IDENTIFY_HASH = 'awesome', 'ei.align-justify'
+    IDENTIFY_HASH = 'awesome', 'fa.hashtag'
+    IDENTIFY_FORMAT = 'awesome', 'ei.align-justify'
     STATUS_ERROR = 'awesome', 'fa.exclamation'
     STATUS_INFO = 'awesome', 'fa.info'
     STATUS_READY = 'awesome', 'fa.check'
     SEPARATOR_H = 'awesome', 'fa.ellipsis-h'
     SEPARATOR_V = 'awesome', 'fa.ellipsis-v'
     TAB_NEW = 'awesome', 'fa.plus'
     INDICATOR_DEFAULT = 'file', os.path.join('images', 'indicator_grey.png')
```

### Comparing `decoder-plus-plus-1.5.0/dpp/core/listener.py` & `decoder-plus-plus-1.7.0/dpp/core/listener.py`

 * *Files 4% similar despite different names*

```diff
@@ -63,15 +63,15 @@
     # Signals that a new tab should be created with the specified input text
     newTabRequested = Signal(str, str)  # title, input_text
 
     # Signals that the selected frame changed (e.g. to update the hex view)
     selectedFrameChanged = Signal(str, str, str)  # tab_id, frame_id, input_text
 
     # Signals that the text inside the codec frame changed (e.g. to update the hex view)
-    textChanged = Signal(str, str, str, bool)  # tab_id, frame_id, input_text, interactive
+    textChanged = Signal(str, str, str)  # tab_id, frame_id, input_text
 
     # Signals that the text selection inside the codec frame changed (e.g. to update the hex view)
     textSelectionChanged = Signal(str, str, str)  # tab_id, frame_id, input_text
 
     # Signals that text of a codec frame should be changed to the specified text (e.g. when hex view was edited by user)
     textSubmitted = Signal(str, str, str)  # tab_id, frame_id, input_text
 
@@ -79,13 +79,13 @@
         super(__class__, self).__init__()
         # Logs each event when being triggered
         self.newTabRequested.connect(lambda title, input_text:
                                      context.logger.trace("newTabRequested({})".format(input_text)))
         self.selectedFrameChanged.connect(lambda tab_id, frame_id, input_text:
                                           context.logger.trace(
                                               "selectedFrameChanged({}, {}, {})".format(tab_id, frame_id, input_text)))
-        self.textChanged.connect(lambda tab_id, frame_id, input_text, interactive:
-            context.logger.trace("textChanged({}, {}, {}, {})".format(tab_id, frame_id, input_text, interactive)))
+        self.textChanged.connect(lambda tab_id, frame_id, input_text:
+            context.logger.trace("textChanged({}, {}, {})".format(tab_id, frame_id, input_text)))
         self.textSelectionChanged.connect(lambda tab_id, frame_id, input_text:
             context.logger.trace("textSelectionChanged({}, {}, {})".format(tab_id, frame_id, input_text)))
         self.textSubmitted.connect(lambda tab_id, frame_id, input_text:
             context.logger.trace("textSubmitted({}, {}, {})".format(tab_id, frame_id, input_text)))
```

### Comparing `decoder-plus-plus-1.5.0/dpp/core/math.py` & `decoder-plus-plus-1.7.0/dpp/core/math.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.5.0/dpp/core/plugin/__init__.py` & `decoder-plus-plus-1.7.0/dpp/core/plugin/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,33 +19,38 @@
 import importlib.util
 import logging
 import os
 import sys
 from typing import List
 
 from dpp.core.assertions import assert_type
+from dpp.core.listener import Signal
 from dpp.core.plugin import config
 from dpp.core.plugin.config import ui, PluginConfig
 from dpp.core.plugin.config import options
-from dpp.core.plugin.config.ui import Layout
-from dpp.core.plugin.config.ui.layouts import FormLayout
-from dpp.core.plugin.config.ui.widgets import Option
+from dpp.core.plugin.config.ui import Layout, Widget
+from dpp.core.plugin.config.ui.layouts import FormLayout, VBoxLayout
+from dpp.core.plugin.config.ui.widgets import Option, GroupBox, TextPreview
 
 
 class PluginType(object):
     DECODER = "Decoder"
     ENCODER = "Encoder"
     HASHER = "Hasher"
     SCRIPT = "Script"
     IDENTIFY = "Identify"
 
 
 class AbstractPlugin:
     """ Base-class to all plugins. Should not be used directly. Instead, use one of its abstract implementations. """
 
+    # Signals used to communicate error or success to the plugin configuration dialog.
+    onError = Signal('PyQt_PyObject')
+    onSuccess = Signal('PyQt_PyObject')
+
     def __init__(self, name: str, type: str, author: str, dependencies: List[str],
                  context: 'dpp.core.context.Context', icon: tuple = None):
         """ Initializes a plugin.
         :param name: the name of the plugin.
         :param type: the type of the plugin (either DECODER, ENCODER, HASHER, SCRIPT, IDENTIFY).
         :param author: the author of the plugin.
         :param dependencies: the dependencies of the plugin (either None or a list of strings).
@@ -56,17 +61,17 @@
         self._safe_name = None
         self._type = type
         self._author = author
         self._dependencies = dependencies
         self._config = PluginConfig(context)
         self._context = context
         self._icon = icon
-        self._logger = logging.getLogger()
+        self._logger = logging.getLogger(__name__)
 
-    def setup(self, config: dict):
+    def setup(self, config: dict, safe_mode: bool = False):
         """ Injects a given configuration into the plugin. """
         for name, value in config.items():
             self.config.add(value)
 
     def is_configurable(self) -> bool:
         """ :return: True, when plugin is configurable, otherwise False. """
         return self.config.count() > 0
@@ -174,14 +179,19 @@
         except Exception as e:
             return False
 
     def dependencies(self) -> List[str]:
         """ :returns all dependencies in a list. """
         return self._dependencies
 
+    def validate_options(self, input_text, option_keys=None):
+        if option_keys:
+            for option_key in option_keys:
+                self.config.validate(self.config.option(option_key), input_text)
+
     def run(self, text: str) -> str:
         """ The main method of the plugin which must be implemented by the plugin. """
         raise NotImplementedError('Method must be implemented by the upper class')
 
     def _run_lines(self, text: str, callback):
         """ Helper method which executes a callback for each line of text. """
         lines = []
@@ -189,17 +199,34 @@
             result = []
             for text_part in text_line.split(" "):
                 if text_part:
                     result.append(callback(text_part))
             lines.append(' '.join(result))
         return os.linesep.join(lines)
 
+    def _create_options_group_box(self, input_text) -> Widget:
+        return GroupBox(label='Options', layout=self._create_options_layout(input_text))
+
+    def _create_options_layout(self, input_text) -> Layout:
+        return FormLayout(widgets=[Option(option) for option in self._config.values()])
+
+    def _create_preview_group_box(self, input_text) -> Widget:
+        return GroupBox(label='Preview', layout=self._create_preview_layout(input_text))
+
+    def _create_preview_layout(self, input_text) -> Layout:
+        return VBoxLayout(widgets=[TextPreview(self, input_text)])
+
     def layout(self, input_text: str) -> Layout:
         """ Returns a layout containing all configuration entries. """
-        return FormLayout(widgets=[Option(option) for option in self._config.values()])
+        return VBoxLayout(
+            widgets=[
+                self._create_options_group_box(input_text),
+                self._create_preview_group_box(input_text)
+            ]
+        )
 
     def _join_options_as_human_readable_string(self, options: List[str]):
         """ Returns the list of options as human-readable string.
 
         Examples:
             [] => ''
             ['a'] => 'a'
```

### Comparing `decoder-plus-plus-1.5.0/dpp/core/plugin/builder.py` & `decoder-plus-plus-1.7.0/dpp/core/plugin/builder.py`

 * *Files 5% similar despite different names*

```diff
@@ -40,18 +40,18 @@
                 mod = __import__('dpp.core.plugin.config.options', fromlist=[clazz])
                 result[name] = getattr(mod, clazz)(**value)
             except:
                 raise Exception("Error while loading plugin configuration!")
 
         return result
 
-    def build(self, config) -> AbstractPlugin:
+    def build(self, config, safe_mode: bool = False) -> AbstractPlugin:
         """ Returns a plugin as specified within configuration item. Returns a NullPlugin on error. """
         try:
             plugin = self._context.getPluginByName(config["name"], config["type"])
-            plugin.setup(self._build_config(config['config']))
+            plugin.setup(self._build_config(config['config']), safe_mode)
             return plugin
         except Exception as err:
             self._context.logger.debug("Error building plugin:")
             self._context.logger.debug("> {}".format(config))
             self._context.logger.debug(err, exc_info=True)
             return NullPlugin(self._context)
```

### Comparing `decoder-plus-plus-1.5.0/dpp/core/plugin/config/__init__.py` & `decoder-plus-plus-1.7.0/dpp/core/plugin/config/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 import json
 from typing import List
 
 import dpp
 from dpp.core.exceptions import ValidationError
 from dpp.core.listener import Signal
 from dpp.core import plugin
+from dpp.core.logger import logmethod
 
 
 class Label:
 
     def __init__(self, key, name):
         self.key = key
         self.name = name
@@ -123,28 +124,28 @@
         """ Returns the individual configuration options in a list. """
         return self._config.values()
 
     def count(self) -> int:
         """ Returns the number of configuration options. """
         return len(self._config.keys())
 
+    @logmethod()
     def update(self, options):
         """
         Updates the value for each specified option.
         :param options: either a name-value-dictionary or an instance of PluginConfig.
 
         If options is a name-value dictionary the is_initialized attribute of the associated PluginConfigOption
         is set to True, to indicate that the option was manually configured.
 
         Example:
             update({"foo": "bar", "bar": "foo"})
             update(config.clone())
         """
         from dpp.core.plugin.config.options import Group
-        self._context.logger.trace('Updating plugin configuration ...')
         if isinstance(options, PluginConfig):
             # Adding/Removing config entries should not be possible during runtime.
             assert options.keys() == self._config.keys(), 'Invalid plugin config! Expected identical keys!'
             updated_keys = []
             for key in options.keys():
                 if options.value(key) != self.value(key):
                     # Only update when there is an actual change of value.
@@ -163,15 +164,15 @@
                 """ Unchecks every option within the specified group. """
                 for option in self._config.items():
                     if isinstance(option, Group) and option.group_name == group_name:
                         option.value = False
 
             updated_keys = []
             for key in options.keys():
-                if options[key] == self._config[key]:
+                if options[key] == self._config[key].value:
                     # Option did not change. Continue with next entry.
                     continue
 
                 original_option = self._config[key]
 
                 # When option is within a group, uncheck all.
                 if isinstance(key, plugin.config.options.Group):
@@ -189,19 +190,19 @@
     def clone(self) -> 'dpp.core.plugin.config.PluginConfig':
         """ Returns a deep copy of the plugin configuration. """
         plugin_config = PluginConfig(self._context)
         plugin_config._config = copy.deepcopy(self._config)
         plugin_config._validators = self._validators
         return plugin_config
 
-    def validate(self, option: Option, plugin: 'AbstractPlugin', input_text: str) -> str:
+    def validate(self, option: Option, input_text: str) -> str:
         """ Returns None if validation succeeded, else error message. """
         if option.key in self._validators and self._validators[option.key] is not None:
             try:
-                return self._validators[option.key](plugin, input_text)
+                return self._validators[option.key](input_text)
             except ValidationError as err:
                 return str(err)
             except Exception as err:
                 self._context.logger.critical(f'Programming Error: Expected ValidationError, got {type(err)}!')
                 return str(err)
 
     def __str__(self):
```

### Comparing `decoder-plus-plus-1.5.0/dpp/core/plugin/config/options/__init__.py` & `decoder-plus-plus-1.7.0/dpp/core/plugin/config/options/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -15,21 +15,32 @@
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 from dpp.core.plugin.config import Option
 
 
 class String(Option):
 
-    def __init__(self, label, value, description, is_required):
+    def __init__(self, label, value, description, is_required=True):
         """
         :param value: the string (e.g. "ab cd ef gh ij kl mn op qr st uv wx yz").
         """
         super(String, self).__init__(label, value, description, is_required)
 
 
+class Text(String):
+
+    def __init__(self, label, value, description, is_required=True, read_only=False, wrap_lines=False):
+        """
+        :param value: the text (e.g. "ab\ncd\nef\ngh\nij\nkl\nmn\nop\nqr\nst\nuv\nwx\nyz").
+        """
+        super(Text, self).__init__(label, value, description, is_required)
+        self.read_only = read_only
+        self.wrap_lines = wrap_lines
+
+
 class Integer(Option):
 
     def __init__(self, label, value, description, is_required, range=None):
         """
         :param value: the integer (e.g. ..., -2, -1, 0, 1, 2, ...).
         :param range: a list containing the minimum and maximum (e.g. [-2, 2])
         """
@@ -76,7 +87,16 @@
     def __init__(self, label, value, values, description, is_required):
         """
         :param value: the selected value.
         :param values: the available values to select.
         """
         super(ComboBox, self).__init__(label, value, description, is_required)
         self.values = values
+
+
+class CodeEditor(Option):
+
+    def __init__(self, label, value, description, is_required):
+        """
+        :param value: the source code (e.g. "def run(input_text):\n\treturn input_text").
+        """
+        super(CodeEditor, self).__init__(label, value, description, is_required)
```

### Comparing `decoder-plus-plus-1.5.0/dpp/core/plugin/config/ui/__init__.py` & `decoder-plus-plus-1.7.0/dpp/core/plugin/config/ui/__init__.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.5.0/dpp/core/plugin/config/ui/layouts.py` & `decoder-plus-plus-1.7.0/dpp/core/plugin/config/ui/layouts.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.5.0/dpp/core/plugin/config/ui/widgets.py` & `decoder-plus-plus-1.7.0/dpp/core/plugin/config/ui/widgets.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,22 +47,31 @@
 
     def __init__(self, label=None, layout=None, show_label=False):
         super().__init__(label=label, layout=layout, show_label=show_label)
 
 
 class Button(Widget):
 
-    def __init__(self, label, on_click, show_label=False):
+    def __init__(self, label, on_click, description="", show_label=False, icon=None):
         super().__init__(label=label, show_label=show_label)
         self.on_click = on_click
+        self.description = description
+        self.icon = icon
 
 
 class ToolButton(Button):
     ...
 
 
+class HSpace(Widget):
+    ...
+
+class VSpace(Widget):
+    ...
+
+
 class TextPreview(Widget):
 
     def __init__(self, plugin, input_text):
         super().__init__()
         self.plugin = plugin
         self.input_text = input_text
```

### Comparing `decoder-plus-plus-1.5.0/dpp/core/plugin/loader.py` & `decoder-plus-plus-1.7.0/dpp/core/plugin/loader.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.5.0/dpp/core/plugin/manager.py` & `decoder-plus-plus-1.7.0/dpp/core/plugin/manager.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.5.0/dpp/core/shortcuts.py` & `decoder-plus-plus-1.7.0/dpp/core/shortcuts.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.5.0/dpp/images/dpp.png` & `decoder-plus-plus-1.7.0/dpp/images/dpp.png`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.5.0/dpp/images/dpp_128.png` & `decoder-plus-plus-1.7.0/dpp/images/dpp_classic_128.png`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.5.0/dpp/images/dpp_classic.png` & `decoder-plus-plus-1.7.0/dpp/images/dpp_classic.png`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.5.0/dpp/images/dpp_modern.png` & `decoder-plus-plus-1.7.0/dpp/images/dpp_modern.png`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.5.0/dpp/images/dpp_modern_128.png` & `decoder-plus-plus-1.7.0/dpp/images/dpp_modern_128.png`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.5.0/dpp/images/dpp_modern_big.png` & `decoder-plus-plus-1.7.0/dpp/images/dpp_modern_big.png`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.5.0/dpp/images/dpp_xmas.png` & `decoder-plus-plus-1.7.0/dpp/images/dpp_xmas.png`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.5.0/dpp/images/keyboard.png` & `decoder-plus-plus-1.7.0/dpp/images/keyboard.png`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.5.0/dpp/images/keyboard.svg` & `decoder-plus-plus-1.7.0/dpp/images/keyboard.svg`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.5.0/dpp/plugins/adler32_hasher.py` & `decoder-plus-plus-1.7.0/dpp/plugins/adler32_hasher.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.5.0/dpp/plugins/apache_md5_hasher.py` & `decoder-plus-plus-1.7.0/dpp/plugins/apache_md5_hasher.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.5.0/dpp/plugins/base16_decoder.py` & `decoder-plus-plus-1.7.0/dpp/plugins/base16_decoder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.5.0/dpp/plugins/base16_encoder.py` & `decoder-plus-plus-1.7.0/dpp/plugins/base16_encoder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.5.0/dpp/plugins/base32_decoder.py` & `decoder-plus-plus-1.7.0/dpp/plugins/base32_decoder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.5.0/dpp/plugins/base32_encoder.py` & `decoder-plus-plus-1.7.0/dpp/plugins/base32_encoder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.5.0/dpp/plugins/base45_decoder.py` & `decoder-plus-plus-1.7.0/dpp/plugins/base45_decoder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.5.0/dpp/plugins/base45_encoder.py` & `decoder-plus-plus-1.7.0/dpp/plugins/base45_encoder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.5.0/dpp/plugins/base64_decoder.py` & `decoder-plus-plus-1.7.0/dpp/plugins/base64_decoder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.5.0/dpp/plugins/base64_encoder.py` & `decoder-plus-plus-1.7.0/dpp/plugins/base64_encoder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.5.0/dpp/plugins/base64_url_decoder.py` & `decoder-plus-plus-1.7.0/dpp/plugins/base64_url_decoder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.5.0/dpp/plugins/base64_url_encoder.py` & `decoder-plus-plus-1.7.0/dpp/plugins/base64_url_encoder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.5.0/dpp/plugins/bin_int_decoder.py` & `decoder-plus-plus-1.7.0/dpp/plugins/bin_int_decoder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.5.0/dpp/plugins/bin_int_encoder.py` & `decoder-plus-plus-1.7.0/dpp/plugins/bin_int_encoder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.5.0/dpp/plugins/bin_str_decoder.py` & `decoder-plus-plus-1.7.0/dpp/plugins/bin_str_decoder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.5.0/dpp/plugins/bin_str_encoder.py` & `decoder-plus-plus-1.7.0/dpp/plugins/bin_str_encoder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.5.0/dpp/plugins/caesar_cipher_script.py` & `decoder-plus-plus-1.7.0/dpp/plugins/caesar_cipher_script.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
             value=0,
             description="integer by which the value of the letters should be shifted.",
             is_required=True,
             range=[0, 26]
         ))
         self._codec = CaesarCipher()
 
-    def layout(self, input_text: str) -> Layout:
+    def _create_options_layout(self, input_text: str) -> Layout:
         return HBoxLayout(widgets=[
             Option(Plugin.Option.Shift),
             Button(
                 label="Calculate",
                 on_click=lambda event: self._calculate_shift(self._config, input_text)
             )
         ])
@@ -68,15 +68,15 @@
 class CaesarCipher:
     """
     Caesar cipher and offset calculator for Caesar cipher based on known frequency of english letters.
     Based on code from RobSpectre (see https://github.com/RobSpectre/Caesar-Cipher/)
     """
 
     def __init__(self):
-        self._logger = logging.getLogger()
+        self._logger = logging.getLogger(__name__)
         # Frequency of letters used in English, taken from Wikipedia.
         # http://en.wikipedia.org/wiki/Letter_frequency
         self.frequency = {
             'a': 0.08167,
             'b': 0.01492,
             'c': 0.02782,
             'd': 0.04253,
```

### Comparing `decoder-plus-plus-1.5.0/dpp/plugins/clone_script.py` & `decoder-plus-plus-1.7.0/dpp/plugins/clone_script.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.5.0/dpp/plugins/crc32_hasher.py` & `decoder-plus-plus-1.7.0/dpp/plugins/crc32_hasher.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.5.0/dpp/plugins/css_minify_script.py` & `decoder-plus-plus-1.7.0/dpp/plugins/css_minify_script.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.5.0/dpp/plugins/dec_str_decoder.py` & `decoder-plus-plus-1.7.0/dpp/plugins/dec_str_decoder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.5.0/dpp/plugins/dec_str_encoder.py` & `decoder-plus-plus-1.7.0/dpp/plugins/dec_str_encoder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.5.0/dpp/plugins/escape_string_script.py` & `decoder-plus-plus-1.7.0/dpp/plugins/escape_string_script.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.5.0/dpp/plugins/extract_urls_script.py` & `decoder-plus-plus-1.7.0/dpp/plugins/extract_urls_script.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.5.0/dpp/plugins/filter_lines_script.py` & `decoder-plus-plus-1.7.0/dpp/plugins/filter_lines_script.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.5.0/dpp/plugins/free_bsd_nt_hasher.py` & `decoder-plus-plus-1.7.0/dpp/plugins/free_bsd_nt_hasher.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.5.0/dpp/plugins/gzip_decoder.py` & `decoder-plus-plus-1.7.0/dpp/plugins/gzip_decoder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.5.0/dpp/plugins/gzip_encoder.py` & `decoder-plus-plus-1.7.0/dpp/plugins/gzip_encoder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.5.0/dpp/plugins/hex_int_decoder.py` & `decoder-plus-plus-1.7.0/dpp/plugins/hex_int_decoder.py`

 * *Files 11% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
         Output:
             123456789
     """
 
     def __init__(self, context: 'dpp.core.context.Context'):
         # Name, Author, Dependencies
-        super().__init__('HEX (int)', "Thomas Engel", [], context)
+        super().__init__('Hex (int)', "Thomas Engel", [], context)
 
     def run(self, input_text: str) -> str:
         return self._run_lines(input_text, lambda text_part: str(int(text_part, 16)))
 
     def can_decode_input(self, input_text):
         if len(input_text) % 2 == 0:
             hex = re.search(r'^(0x|0X)[a-fA-F0-9]+$', input_text)
```

### Comparing `decoder-plus-plus-1.5.0/dpp/plugins/hex_int_encoder.py` & `decoder-plus-plus-1.7.0/dpp/plugins/hex_int_encoder.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,11 +28,11 @@
 
         Output:
             0x75bcd15
     """
 
     def __init__(self, context: 'dpp.core.context.Context'):
         # Name, Author, Dependencies
-        super().__init__('HEX (int)', "Thomas Engel", [], context)
+        super().__init__('Hex (int)', "Thomas Engel", [], context)
 
     def run(self, input_text: str) -> str:
         return self._run_lines(input_text, lambda text_part: hex(int(text_part)))
```

### Comparing `decoder-plus-plus-1.5.0/dpp/plugins/hex_shell_decoder.py` & `decoder-plus-plus-1.7.0/dpp/plugins/hex_shell_decoder.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,15 +37,15 @@
             abcdefghijklmnopqrstuvwxyz
             ^°!"§$%&/()=?´`<>| ,.-;:_#+'*~
             0123456789
     """
 
     def __init__(self, context: 'dpp.core.context.Context'):
         # Name, Author, Dependencies
-        super().__init__('HEX (shell)', "Thomas Engel", ["codecs"], context)
+        super().__init__('Hex (shell)', "Thomas Engel", ["codecs"], context)
 
     def run(self, input_text: str) -> str:
         if input_text:
             import codecs
             import re
             output = input_text
             for hex_code in set(sorted(re.findall(r'\\[Xx][0-9a-fA-F][0-9a-fA-F]', input_text))):
```

### Comparing `decoder-plus-plus-1.5.0/dpp/plugins/hex_shell_encoder.py` & `decoder-plus-plus-1.7.0/dpp/plugins/hex_shell_encoder.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
             \\xc2\\xb4\\x60\\x3c\\x3e\\x7c\\x20\\x2c\\x2e\\x2d\\x3b\\x3a\\x5f\\x23 \\
             \\x2b\\x27\\x2a\\x7e\\x0a\\x30\\x31\\x32\\x33\\x34\\x35\\x36\\x37\\x38 \\
             \\x39
     """
 
     def __init__(self, context: 'dpp.core.context.Context'):
         # Name, Author, Dependencies
-        super().__init__('HEX (shell)', "Thomas Engel", ["codecs"], context)
+        super().__init__('Hex (shell)', "Thomas Engel", ["codecs"], context)
 
     def run(self, input_text: str) -> str:
         if input_text:
             import codecs
             output = codecs.encode(input_text.encode('utf-8', errors='surrogateescape'), 'hex') \
                 .decode('utf-8', errors='surrogateescape')
             return "\\x" + "\\x".join([i + j for i, j in zip(output[::2], output[1::2])])
```

### Comparing `decoder-plus-plus-1.5.0/dpp/plugins/hex_str_decoder.py` & `decoder-plus-plus-1.7.0/dpp/plugins/hex_str_decoder.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
             abcdefghijklmnopqrstuvwxyz
             ^°!"§$%&/()=?´`<>| ,.-;:_#+'*~
             0123456789
     """
 
     def __init__(self, context: 'dpp.core.context.Context'):
         # Name, Author, Dependencies
-        super().__init__('HEX (str)', "Thomas Engel", [], context)
+        super().__init__('Hex (str)', "Thomas Engel", [], context)
 
     def run(self, input_text: str) -> str:
         return self._run_lines(input_text, lambda text_part: bytes.fromhex(text_part).decode('ascii'))
 
     def can_decode_input(self, input_text: str) -> bool:
         if len(input_text) % 2 == 0:
             hex = re.search(r'^[a-fA-F0-9]+$', input_text)
```

### Comparing `decoder-plus-plus-1.5.0/dpp/plugins/hex_str_encoder.py` & `decoder-plus-plus-1.7.0/dpp/plugins/hex_str_encoder.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,13 +32,13 @@
             6162636465666768696a6b6c6d6e6f70717273747576777 \\
             8797a0a5ec2b02122c2a72425262f28293d3fc2b4603c3e \\
             7c202c2e2d3b3a5f232b272a7e0a30313233343536373839
     """
 
     def __init__(self, context: 'dpp.core.context.Context'):
         # Name, Author, Dependencies
-        super().__init__('HEX (str)', "Thomas Engel", ["codecs"], context)
+        super().__init__('Hex (str)', "Thomas Engel", ["codecs"], context)
 
     def run(self, input_text: str) -> str:
         import codecs
         return codecs.encode(input_text.encode('utf-8', errors='surrogateescape'), 'hex') \
             .decode('utf-8', errors='surrogateescape')
```

### Comparing `decoder-plus-plus-1.5.0/dpp/plugins/html_beautify_script.py` & `decoder-plus-plus-1.7.0/dpp/plugins/html_beautify_script.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.5.0/dpp/plugins/html_decoder.py` & `decoder-plus-plus-1.7.0/dpp/plugins/html_decoder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.5.0/dpp/plugins/html_encoder.py` & `decoder-plus-plus-1.7.0/dpp/plugins/html_encoder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.5.0/dpp/plugins/html_minify_script.py` & `decoder-plus-plus-1.7.0/dpp/plugins/html_minify_script.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.5.0/dpp/plugins/http64_decoder.py` & `decoder-plus-plus-1.7.0/dpp/plugins/http64_decoder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.5.0/dpp/plugins/http64_encoder.py` & `decoder-plus-plus-1.7.0/dpp/plugins/http64_encoder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.5.0/dpp/plugins/identify_file_type_script.py` & `decoder-plus-plus-1.7.0/dpp/plugins/identify_file_type_filemagic_script.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,25 +10,26 @@
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
+from dpp.core.icons import Icon
 from dpp.core.plugin import IdentifyPlugin
 
 
 class Plugin(IdentifyPlugin):
     """
     Detects the file type of the input text based on magic bytes.
     """
 
     def __init__(self, context: 'dpp.core.context.Context'):
         # Name, Author, Dependencies
-        super().__init__('Identify File Type', "Thomas Engel", ["filemagic"], context)
+        super().__init__('Identify File Type (filemagic)', "Thomas Engel", ["filemagic"], context, icon=Icon.IDENTIFY_FORMAT)
 
     def _detect_magic_bytes(self, input_text: str) -> str:
         import magic
         with magic.Magic() as m:
             return m.id_buffer(input_text)
 
     def run(self, input_text: str) -> str:
```

### Comparing `decoder-plus-plus-1.5.0/dpp/plugins/identify_hash_format_script.py` & `decoder-plus-plus-1.7.0/dpp/plugins/identify_hash_format_script.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,25 +10,26 @@
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
+from dpp.core.icons import Icon
 from dpp.core.plugin import IdentifyPlugin
 
 
 class Plugin(IdentifyPlugin):
     """
     Identifies the hash format of the input text based on structure.
     """
 
     def __init__(self, context: 'dpp.core.context.Context'):
         # Name, Author, Dependencies
-        super().__init__('Identify Hash Format', "Thomas Engel", ["hashid"], context)
+        super().__init__('Identify Hash Format', "Thomas Engel", ["hashid"], context, icon=Icon.IDENTIFY_HASH)
 
     def _detect_hash_format(self, input_text: str) -> str:
         from hashid import HashID
         return "\n".join(sorted([item.name for item in HashID().identifyHash(input_text)]))
 
     def run(self, input_text: str) -> str:
         return self._detect_hash_format(input_text)
```

### Comparing `decoder-plus-plus-1.5.0/dpp/plugins/jq_script.py` & `decoder-plus-plus-1.7.0/dpp/plugins/jq_script.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.5.0/dpp/plugins/js_beautify_script.py` & `decoder-plus-plus-1.7.0/dpp/plugins/js_beautify_script.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.5.0/dpp/plugins/js_minify_script.py` & `decoder-plus-plus-1.7.0/dpp/plugins/js_minify_script.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.5.0/dpp/plugins/js_to_xml_script.py` & `decoder-plus-plus-1.7.0/dpp/plugins/js_to_xml_script.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.5.0/dpp/plugins/jsonify_script.py` & `decoder-plus-plus-1.7.0/dpp/plugins/jsonify_script.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,22 +12,19 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 import json
 import logging
-import math
 import os.path
-import string
 from abc import abstractmethod
 from typing import Callable
 
 from lxml import etree
-from ruamel import yaml
 
 from dpp.core.exceptions import CodecException
 from dpp.core import plugin
 from dpp.core.icons import Icon
 from dpp.core.plugin.config import options
 from dpp.core.plugin.config.ui import Layout
 from dpp.core.plugin.config.ui.layouts import HBoxLayout
@@ -169,15 +166,15 @@
                 'zipinfo'
             ],
             description="the format of the input text.",
             is_required=True,
         ))
         self._codec = JC()
 
-    def layout(self, input_text: str) -> Layout:
+    def _create_options_layout(self, input_text: str) -> Layout:
         return HBoxLayout(widgets=[
             Option(Plugin.Option.Format),
             Button(
                 label="Auto-Detect",
                 on_click=lambda event: self._auto_detect_format(self._config, input_text)
             )
         ])
@@ -197,15 +194,15 @@
 
 class JC:
     """ Codec for transforming various file formats into JSON using jc. """
 
     class ParserBase:
 
         def __init__(self, input_format: str, input_text: str):
-            self._logger = logging.getLogger()
+            self._logger = logging.getLogger(__name__)
             self._input_format = input_format
             self._input_text = input_text
             self._output_text = ""
 
         def pre_check(self) -> bool:
             """ Checks the input text whether it conforms to a specific format. """
             try:
@@ -323,20 +320,21 @@
 
         def pre_check(self) -> bool:
             return self._check_true(lambda: etree.fromstring(self._input_text) != None)
 
     class YamlParser(ParserBase):
 
         def pre_check(self) -> bool:
+            from ruamel import yaml
             return self._check_true(lambda: yaml.safe_dump(self._input_text) != None)
 
 
     def __init__(self):
         import validators
-        self._logger = logging.getLogger()
+        self._logger = logging.getLogger(__name__)
         self._auto_detect_skip_list = [
             'airport-s',
             'asciitable',
             'gpg',
             'hash',
             'pip-list',
             'systemctl',
```

### Comparing `decoder-plus-plus-1.5.0/dpp/plugins/jsonpath_script.py` & `decoder-plus-plus-1.7.0/dpp/plugins/jsonpath_script.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.5.0/dpp/plugins/jwt_decoder.py` & `decoder-plus-plus-1.7.0/dpp/plugins/jwt_decoder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.5.0/dpp/plugins/keccak224_hasher.py` & `decoder-plus-plus-1.7.0/dpp/plugins/keccak224_hasher.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.5.0/dpp/plugins/keccak256_hasher.py` & `decoder-plus-plus-1.7.0/dpp/plugins/keccak256_hasher.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.5.0/dpp/plugins/keccak384_hasher.py` & `decoder-plus-plus-1.7.0/dpp/plugins/keccak384_hasher.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.5.0/dpp/plugins/keccak512_hasher.py` & `decoder-plus-plus-1.7.0/dpp/plugins/keccak512_hasher.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.5.0/dpp/plugins/little_big_endian_script.py` & `decoder-plus-plus-1.7.0/dpp/plugins/little_big_endian_script.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.5.0/dpp/plugins/lm_hasher.py` & `decoder-plus-plus-1.7.0/dpp/plugins/lm_hasher.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.5.0/dpp/plugins/md2_hasher.py` & `decoder-plus-plus-1.7.0/dpp/plugins/md2_hasher.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.5.0/dpp/plugins/md4_hasher.py` & `decoder-plus-plus-1.7.0/dpp/plugins/md4_hasher.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.5.0/dpp/plugins/md5_hasher.py` & `decoder-plus-plus-1.7.0/dpp/plugins/md5_hasher.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.5.0/dpp/plugins/nt_hasher.py` & `decoder-plus-plus-1.7.0/dpp/plugins/nt_hasher.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.5.0/dpp/plugins/oct_int_decoder.py` & `decoder-plus-plus-1.7.0/dpp/plugins/oct_int_decoder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.5.0/dpp/plugins/oct_int_encoder.py` & `decoder-plus-plus-1.7.0/dpp/plugins/oct_int_encoder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.5.0/dpp/plugins/oct_str_decoder.py` & `decoder-plus-plus-1.7.0/dpp/plugins/oct_str_decoder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.5.0/dpp/plugins/oct_str_encoder.py` & `decoder-plus-plus-1.7.0/dpp/plugins/oct_str_encoder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.5.0/dpp/plugins/phpass_hasher.py` & `decoder-plus-plus-1.7.0/dpp/plugins/phpass_hasher.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.5.0/dpp/plugins/reformat_text_script.py` & `decoder-plus-plus-1.7.0/dpp/plugins/reformat_text_script.py`

 * *Files 10% similar despite different names*

```diff
@@ -58,32 +58,32 @@
         IsRegex = Label("is_regex", "Regex")
         HandleNewlines = Label("handle_newlines", "Handle Newlines")
 
     def __init__(self, context: 'dpp.core.context.Context'):
         # Name, Author, Dependencies, Icon
         super().__init__('Reformat Text', "Thomas Engel", [], context, Icon.EDIT)
 
-        def _validate_split_chars(plugin: 'AbstractPlugin', input_text: str):
+        def _validate_split_chars(input_text: str):
 
             def _validate_regex():
                 try:
-                    re.compile(plugin.config.value(Plugin.Option.SplitChars))
+                    re.compile(self.config.value(Plugin.Option.SplitChars))
                     return True
                 except:
                     return False
 
-            if not plugin.config.value(Plugin.Option.SplitChars):
+            if not self.config.value(Plugin.Option.SplitChars):
                 raise ValidationError("Split by should not be empty!")
 
-            if plugin.config.value(Plugin.Option.IsRegex) and not _validate_regex():
+            if self.config.value(Plugin.Option.IsRegex) and not _validate_regex():
                 raise ValidationError("Invalid regular expression!")
 
-        def _validate_format(plugin: 'AbstractPlugin', input_text: str):
+        def _validate_format(input_text: str):
             try:
-                plugin.run(input_text)
+                self.run(input_text)
             except:
                 raise ValidationError("Invalid format string!")
 
         self.config.add(String(
             label=Plugin.Option.Format,
             value="",
             description="the format string to be used",
@@ -105,15 +105,15 @@
             label=Plugin.Option.HandleNewlines,
             value=True,
             description="defines whether the operation should be applied for each individual line (default=True)",
             is_required=False
         ))
         self._codec = ReformatCodec()
 
-    def layout(self, input_text: str) -> Layout:
+    def _create_options_layout(self, input_text: str) -> Layout:
         return FormLayout(
             widgets=[
                 Frame(
                     label=Plugin.Option.Format.name,
                     layout=HBoxLayout(
                         widgets=[
                             Option(self._config.option(Plugin.Option.Format), show_label=False),
```

### Comparing `decoder-plus-plus-1.5.0/dpp/plugins/remove_newlines_script.py` & `decoder-plus-plus-1.7.0/dpp/plugins/remove_newlines_script.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.5.0/dpp/plugins/remove_whitespaces_script.py` & `decoder-plus-plus-1.7.0/dpp/plugins/remove_whitespaces_script.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.5.0/dpp/plugins/ripemd160_hasher.py` & `decoder-plus-plus-1.7.0/dpp/plugins/unescape_string_script.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,32 +10,21 @@
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
-from dpp.core.plugin import HasherPlugin
+from dpp.core.plugin import ScriptPlugin
 
 
-class Plugin(HasherPlugin):
+class Plugin(ScriptPlugin):
     """
-    Hashes a string using RIPEMD160.
-
-    Example:
-
-        Input:
-            abcdefghijklmnopqrstuvwxyz
-            ^°!"§$%&/()=?´`<>| ,.-;:_#+'*~
-            0123456789
-
-        Output:
-            1b63bae30eb8be665459c3f2021293811ac2d63b
+    Unescapes the input string.
     """
 
     def __init__(self, context: 'dpp.core.context.Context'):
         # Name, Author, Dependencies
-        super().__init__('RIPEMD160', "Tim Menapace", ["hashlib"], context)
+        super().__init__('Unescape String', "Thomas Engel", [], context)
 
     def run(self, input_text: str) -> str:
-        import hashlib
-        return hashlib.new('ripemd160', input_text.encode('utf-8', errors='surrogateescape')).hexdigest()
+        return input_text.encode('utf-8').decode('unicode_escape')
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `decoder-plus-plus-1.5.0/dpp/plugins/rot13_decoder.py` & `decoder-plus-plus-1.7.0/dpp/plugins/rot13_decoder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.5.0/dpp/plugins/rot13_encoder.py` & `decoder-plus-plus-1.7.0/dpp/plugins/rot13_encoder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.5.0/dpp/plugins/search_and_replace_script.py` & `decoder-plus-plus-1.7.0/dpp/plugins/search_and_replace_script.py`

 * *Files 4% similar despite different names*

```diff
@@ -54,16 +54,16 @@
     def __init__(self, context: 'dpp.core.context.Context'):
         # Name, Author, Dependencies, Icon
         super().__init__('Search & Replace', "Thomas Engel", [], context, Icon.SEARCH)
         self._codec = Plugin.SearchAndReplaceCodec()
         self._init_config()
 
     def _init_config(self):
-        def _validate_search_term(plugin: 'AbstractPlugin', input_text: str):
-            if not plugin.config.value(Plugin.Option.SearchTerm):
+        def _validate_search_term(input_text: str):
+            if not self.config.value(Plugin.Option.SearchTerm):
                 raise ValidationError("Search term should not be empty.")
 
         self.config.add(String(
             label=Plugin.Option.SearchTerm,
             value="",
             description="the word or phrase to replace",
             is_required=True
```

### Comparing `decoder-plus-plus-1.5.0/dpp/plugins/sha1_hasher.py` & `decoder-plus-plus-1.7.0/dpp/plugins/sha1_hasher.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.5.0/dpp/plugins/sha224_hasher.py` & `decoder-plus-plus-1.7.0/dpp/plugins/sha224_hasher.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.5.0/dpp/plugins/sha256_hasher.py` & `decoder-plus-plus-1.7.0/dpp/plugins/sha256_hasher.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.5.0/dpp/plugins/sha384_hasher.py` & `decoder-plus-plus-1.7.0/dpp/plugins/sha384_hasher.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.5.0/dpp/plugins/sha3_224_hasher.py` & `decoder-plus-plus-1.7.0/dpp/plugins/sha3_224_hasher.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.5.0/dpp/plugins/sha3_256_hasher.py` & `decoder-plus-plus-1.7.0/dpp/plugins/sha3_256_hasher.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.5.0/dpp/plugins/sha3_384_hasher.py` & `decoder-plus-plus-1.7.0/dpp/plugins/sha3_384_hasher.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.5.0/dpp/plugins/sha3_512_hasher.py` & `decoder-plus-plus-1.7.0/dpp/plugins/sha3_512_hasher.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.5.0/dpp/plugins/sha512_hasher.py` & `decoder-plus-plus-1.7.0/dpp/plugins/sha512_hasher.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.5.0/dpp/plugins/split_and_rejoin_script.py` & `decoder-plus-plus-1.7.0/dpp/plugins/split_and_rejoin_script.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,20 +68,20 @@
     def __init__(self, context: 'dpp.core.context.Context'):
         # Name, Author, Dependencies, Icon
         super().__init__('Split & Rejoin', "Thomas Engel", [], context, Icon.EDIT)
         self._init_config()
         self._codec = Plugin.SplitAndRejoinCodec()
 
     def _init_config(self):
-        def _validate_split_text(plugin: 'AbstractPlugin', input_text: str):
-            if not plugin.config.value(Plugin.Option.SplitText):
+        def _validate_split_text(input_text: str):
+            if not self.config.value(Plugin.Option.SplitText):
                 raise ValidationError("Split by should not be empty.")
-            if plugin.config.value(Plugin.Option.SplitByLength):
+            if self.config.value(Plugin.Option.SplitByLength):
                 try:
-                    length = int(plugin.config.value(Plugin.Option.SplitText))
+                    length = int(self.config.value(Plugin.Option.SplitText))
                     if length <= 0:
                         raise ValidationError("Split by should be greater than 0.")
                 except:
                     raise ValidationError("Split by should be an integer.")
 
         self.config.add(String(
             label=Plugin.Option.SplitText,
```

### Comparing `decoder-plus-plus-1.5.0/dpp/plugins/sun_md5_hasher.py` & `decoder-plus-plus-1.7.0/dpp/plugins/sun_md5_hasher.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.5.0/dpp/plugins/unescape_string_script.py` & `decoder-plus-plus-1.7.0/tests/plugins/extract_urls_script_test.py`

 * *Files 17% similar despite different names*

```diff
@@ -10,21 +10,23 @@
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
-from dpp.core.plugin import ScriptPlugin
+import unittest
 
+from dpp.core.plugin import PluginType
+from tests.utils import load_plugin
 
-class Plugin(ScriptPlugin):
-    """
-    Unescapes the input string.
-    """
 
-    def __init__(self, context: 'dpp.core.context.Context'):
-        # Name, Author, Dependencies
-        super().__init__('Unescape String', "Thomas Engel", [], context)
+class TestExtractURLsScript(unittest.TestCase):
 
-    def run(self, input_text: str) -> str:
-        return input_text.encode('utf-8').decode('unicode_escape')
+    plugin = load_plugin("Extract URLs", PluginType.SCRIPT)
+
+    def testPlugin(self):
+        self.assertEqual(self.plugin.run(
+            'abcdefghijklmnopqrstuvwxyz\n'
+            'dcba http://example.com abcd\n'
+            '0123456789'
+        ), 'http://example.com')
```

### Comparing `decoder-plus-plus-1.5.0/dpp/plugins/url_decoder.py` & `decoder-plus-plus-1.7.0/dpp/plugins/url_decoder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.5.0/dpp/plugins/url_encoder.py` & `decoder-plus-plus-1.7.0/dpp/plugins/url_encoder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.5.0/dpp/plugins/url_plus_decoder.py` & `decoder-plus-plus-1.7.0/dpp/plugins/url_plus_decoder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.5.0/dpp/plugins/url_plus_encoder.py` & `decoder-plus-plus-1.7.0/dpp/plugins/url_plus_encoder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.5.0/dpp/plugins/xpath_script.py` & `decoder-plus-plus-1.7.0/dpp/plugins/xpath_script.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.5.0/dpp/plugins/zlib_decoder.py` & `decoder-plus-plus-1.7.0/dpp/plugins/zlib_decoder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.5.0/dpp/plugins/zlib_encoder.py` & `decoder-plus-plus-1.7.0/dpp/plugins/zlib_encoder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.5.0/dpp/runner.py` & `decoder-plus-plus-1.7.0/dpp/runner.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
+import logging
 import os
 import signal
 import sys
 import argparse
 from collections import namedtuple
 from typing import List
 
@@ -254,15 +255,15 @@
 
 
 def main():
     # Abort program execution on ctrl+c
     signal.signal(signal.SIGINT, signal.SIG_DFL)
 
     # Loads logger, config and plugins.
-    context = Context('net.bytebutcher.decoder_plus_plus', app_path, namespace=locals())
+    context = Context('net.bytebutcher.decoder_plus_plus', app_path)
 
     # Enable debug mode for current session.
     if '--debug' in sys.argv:
         context.setDebugMode(True, temporary=True)
 
     if '--trace' in sys.argv:
         context.setTraceMode(True)
```

### Comparing `decoder-plus-plus-1.5.0/dpp/ui/__init__.py` & `decoder-plus-plus-1.7.0/dpp/ui/__init__.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.5.0/dpp/ui/builder/action_builder.py` & `decoder-plus-plus-1.7.0/dpp/ui/builder/action_builder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.5.0/dpp/ui/builder/plugin_config_widget_builder.py` & `decoder-plus-plus-1.7.0/dpp/ui/builder/plugin_config_widget_builder.py`

 * *Files 20% similar despite different names*

```diff
@@ -23,23 +23,22 @@
 
 class PluginConfigWidgetBuilder:
 
     def __init__(self, parent, plugin, input_text):
         self._parent = parent
         self._plugin = plugin
         self._input_text = input_text
-        self._layout_callback = lambda layout_spec: layout_spec
 
     def layout(self, callback: Callable) -> 'PluginConfigWidgetBuilder':
         self._layout_callback = callback
         return self
 
     def build(self) -> QFrame:
         """ Builds the widget based on the layout specification. """
         frame = QFrame(self._parent)
-        layout_spec = self._layout_callback(self._plugin.layout(self._input_text))
+        layout_spec = self._plugin.layout(self._input_text)
         assert layout_spec, 'Illegal layout specification! Expected object, got None!'
         layout = LayoutBuilder().build(self._plugin, self._input_text, layout_spec)
         assert layout, 'Illegal layout! Expected object, got None!'
         layout.setContentsMargins(0, 0, 0, 0)
         frame.setLayout(layout)
         return frame
```

### Comparing `decoder-plus-plus-1.5.0/dpp/ui/builder/widget_builder.py` & `decoder-plus-plus-1.7.0/dpp/ui/builder/widget_builder.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,28 +17,32 @@
 import logging
 from typing import Union
 
 from qtpy.QtWidgets import QPushButton, QToolButton, QGroupBox, QLabel, QFrame, QWidget, QFormLayout, QLayout, \
     QHBoxLayout, QVBoxLayout
 
 from dpp.core.assertions import assert_type, assert_instance
+from dpp.core.icons import icon
 from dpp.core.plugin import AbstractPlugin
-from dpp.core.plugin.config.options import Boolean, Slider, String, Integer, Group, ComboBox
+from dpp.core.plugin.config.options import Boolean, Slider, String, Integer, Group, ComboBox, CodeEditor, Text
 from dpp.core.plugin.config.ui import Widget, Layout
-from dpp.core.plugin.config.ui.widgets import ToolButton, Button, GroupBox, TextPreview, Frame, Option, Label
+from dpp.core.plugin.config.ui.widgets import ToolButton, Button, GroupBox, TextPreview, Frame, Option, Label, HSpace, \
+    VSpace
 from dpp.core.plugin.config.ui.layouts import FormLayout, VBoxLayout, HBoxLayout
+from dpp.ui import VSpacer, HSpacer
 from dpp.ui.widget.codec_preview_widget import CodecPreviewWidget
+from dpp.ui.widget.code_editor_widget import CodeEditorWidget
 from dpp.ui.widget.option_widgets import SliderOptionWidget, StringOptionWidget, GroupOptionWidget, \
-    BooleanOptionWidget, OptionWidget, ComboBoxOptionWidget
+    BooleanOptionWidget, OptionWidget, ComboBoxOptionWidget, CodeEditorOptionWidget, TextOptionWidget
 
 
 class BuilderBase:
 
     def __init__(self):
-        self._logger = logging.getLogger()
+        self._logger = logging.getLogger(__name__)
 
 
 class LayoutBuilder(BuilderBase):
 
     def __init__(self, widget_builder: 'WidgetBuilder' = None):
         super().__init__()
         self._widget_builder = WidgetBuilder(layout_builder=self) if not widget_builder else widget_builder
@@ -78,20 +82,22 @@
 
 
 class OptionWidgetBuilder(BuilderBase):
 
     def __init__(self):
         super().__init__()
         self._widgets = {
+            Boolean: BooleanOptionWidget,
+            CodeEditor: CodeEditorOptionWidget,
+            ComboBox: ComboBoxOptionWidget,
+            Group: GroupOptionWidget,
+            Integer: StringOptionWidget,
             Slider: SliderOptionWidget,
             String: StringOptionWidget,
-            Integer: StringOptionWidget,
-            Group: GroupOptionWidget,
-            Boolean: BooleanOptionWidget,
-            ComboBox: ComboBoxOptionWidget
+            Text: TextOptionWidget,
         }
 
     def _build(self, plugin: AbstractPlugin, input_text: str, widget_spec: Option):
         # Note: We are using type() instead of instanceof since we really want to check whether the object is a
         #       specific type rather than checking whether the object inherits from some class.
         if type(widget_spec) is Option:
             widget = self._build(plugin, input_text, plugin.config.option(widget_spec.key))
@@ -103,53 +109,70 @@
             return widget
 
         if type(widget_spec) not in self._widgets:
             raise Exception(f'Can not build widget! Unknown widget specification {type(widget_spec)}!')
 
         widget = self._widgets[type(widget_spec)](plugin.config, widget_spec)
 
-        # Update config, when option widget value changes.
+        # Update config, when option widget value is changes by user.
         widget.onChange.connect(
             lambda option_widget: plugin.config.update({option_widget.getKey(): option_widget.getValue()}))
 
-        # TODO: This should be part of the widget.
-        widget.onChange.connect(lambda option_widget: widget.validate(plugin, input_text))
-
         return widget
 
     def build(self, plugin: AbstractPlugin, input_text: str, widget_spec: Option) -> OptionWidget:
         """ Automatically builds the widget for this option. """
         return self._build(plugin, input_text, widget_spec).getWidget()
 
 
 class ToolButtonWidgetBuilder(BuilderBase):
 
     def build(self, plugin: AbstractPlugin, input_text: str, widget_spec: ToolButton) -> QWidget:
         widget = QToolButton()
         widget.setText(widget_spec.label)
+        widget.setToolTip(widget_spec.description)
         widget.clicked.connect(widget_spec.on_click)
+        if widget_spec.icon:
+            widget.setIcon(icon(widget_spec.icon))
         return widget
 
 
 class ButtonWidgetBuilder(BuilderBase):
 
     def build(self, plugin: AbstractPlugin, input_text: str, widget_spec: Button) -> QWidget:
         widget = QPushButton(widget_spec.label)
         widget.setText(widget_spec.label)
+        widget.setToolTip(widget_spec.description)
         widget.clicked.connect(widget_spec.on_click)
+        if widget_spec.icon:
+            widget.setIcon(icon(widget_spec.icon))
         return widget
 
 
 class LabelWidgetBuilder(BuilderBase):
     """ Builds a label from a widget specification. """
 
     def build(self, plugin: AbstractPlugin, input_text: str, widget_spec: Label) -> QWidget:
         return QLabel(widget_spec.label)
 
 
+class HSpaceWidgetBuilder(BuilderBase):
+    """ Builds a horizontal spacer from a widget specification. """
+
+    def build(self, plugin: AbstractPlugin, input_text: str, widget_spec: Label) -> QWidget:
+        return HSpacer()
+
+
+class VSpaceWidgetBuilder(BuilderBase):
+    """ Builds a vertical spacer from a widget specification. """
+
+    def build(self, plugin: AbstractPlugin, input_text: str, widget_spec: Label) -> QWidget:
+        return VSpacer()
+
+
 class GroupBoxWidgetBuilder(BuilderBase):
 
     def build(self, plugin: AbstractPlugin, input_text: str, widget_spec: GroupBox) -> QWidget:
         group_box = QGroupBox(widget_spec.label)
         group_box.setStyleSheet("""
         QGroupBox {
             border: 1px solid silver;
@@ -179,14 +202,20 @@
 
 class TextPreviewWidgetBuilder(BuilderBase):
 
     def build(self, plugin: AbstractPlugin, input_text: str, widget_spec: TextPreview) -> QWidget:
         return CodecPreviewWidget(plugin, input_text)
 
 
+class CodeEditorWidgetBuilder(BuilderBase):
+
+    def build(self, plugin: AbstractPlugin, input_text: str, widget_spec: CodeEditor) -> QWidget:
+        return CodeEditorWidget(plugin, input_text)
+
+
 class LabelBuilder(BuilderBase):
 
     def build(self, plugin: AbstractPlugin, input_text: str, widget_spec: Widget) -> QWidget:
         label = None
         if widget_spec.label and widget_spec.show_label:
             assert_type(widget_spec.label, str)
             label = QLabel()
@@ -197,21 +226,23 @@
 class WidgetBuilder(BuilderBase):
 
     def __init__(self, label_builder: LabelBuilder = None, layout_builder: LayoutBuilder = None):
         super().__init__()
         self._label_builder = LabelBuilder() if not label_builder else label_builder
         self._layout_builder = LayoutBuilder(widget_builder=self) if not layout_builder else layout_builder
         self._widget_builders = {
-            ToolButton: ToolButtonWidgetBuilder(),
             Button: ButtonWidgetBuilder(),
-            Label: LabelWidgetBuilder(),
-            GroupBox: GroupBoxWidgetBuilder(),
             Frame: FrameWidgetBuilder(),
+            GroupBox: GroupBoxWidgetBuilder(),
+            HSpace: HSpaceWidgetBuilder(),
+            Label: LabelWidgetBuilder(),
+            Option: OptionWidgetBuilder(),
             TextPreview: TextPreviewWidgetBuilder(),
-            Option: OptionWidgetBuilder()
+            ToolButton: ToolButtonWidgetBuilder(),
+            VSpace: VSpaceWidgetBuilder(),
         }
 
     def build(self, plugin: AbstractPlugin, input_text: str, widget_spec) -> Union[str, QWidget]:
         if type(widget_spec) not in self._widget_builders:
             raise Exception(f'Can not build widget! Unknown widget specification {type(widget_spec)}!')
 
         widget = self._widget_builders[type(widget_spec)].build(plugin, input_text, widget_spec)
```

### Comparing `decoder-plus-plus-1.5.0/dpp/ui/decoder_plus_plus_gui.py` & `decoder-plus-plus-1.7.0/dpp/ui/decoder_plus_plus_gui.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,19 +17,21 @@
 import os
 
 from qtpy.QtCore import Qt
 from qtpy.QtGui import QIcon
 from qtpy.QtWidgets import QMainWindow, QFrame, QDialogButtonBox, QShortcut, QVBoxLayout
 
 from dpp.core import Context
+from dpp.core.logger import logmethod
 from dpp.core.shortcuts import KeySequence
 from dpp.ui.dock.hex_dock import HexDock
 from dpp.ui.dock.log_dock import LogDock
 from dpp.ui.view.classic.classic_main_window_widget import ClassicMainWindowWidget
 from dpp.ui.view.classic import CodecTab
+from dpp.ui.view.modern.modern_main_window_widget import ModernMainWindowWidget
 from dpp.ui.widget.dock_tabs_widget import DockTabsWidget
 
 
 class DecoderPlusPlusGui(QMainWindow):
 
     def __init__(self, context: 'core.context.Context'):
         super().__init__()
@@ -55,22 +57,22 @@
         :param context: the application context.
         :param input_text: the user input.
         """
         super().__init__(context)
         self.setCentralWidget(ClassicMainWindowWidget(self, self._context, input_text))
         self.show()
 
-    def newTab(self, input_text: str):
+    def newTab(self, input_text: str) -> (int, CodecTab):
         """
         Opens a new tab with the specified input as content for the first codec frame.
         This function is used when user runs Decoder++ when it is already running and the --new-instance switch
         was not used.
         """
         self._context.logger.info("Opening input in new tab...")
-        self.centralWidget().tabsWidget().onTabAddButtonClick.emit(None, input_text)
+        return self.centralWidget().newTab(input_text=input_text)
 
 
 class DecoderPlusPlusDialog(DecoderPlusPlusGui):
     """
     The DecoderPlusPlusDialog with OK- and Cancel button.
     When the OK-button is triggered the transformed text is printed to stdout.
     When the Cancel-button is triggered or the user exist the application in any other way the initial input is
@@ -109,40 +111,44 @@
 
         # Do not show statusbar in dialog mode.
         self.statusBar().hide()
 
         # Show dialog.
         self.show()
 
+    @logmethod()
     def _setup_shortcuts(self):
         """ Setup shortcuts to allow user to quickly hit the accept button. """
         ctrl_return_shortcut = QShortcut(KeySequence(Qt.CTRL, Qt.Key_Return), self)
         ctrl_return_shortcut.activated.connect(self.onAccept)
         alt_return_shortcut = QShortcut(KeySequence(Qt.ALT, Qt.Key_Return), self)
         alt_return_shortcut.activated.connect(self.onAccept)
         alt_o_shortcut = QShortcut(KeySequence(Qt.ALT, Qt.Key_O), self)
         alt_o_shortcut.activated.connect(self.onAccept)
 
+    @logmethod()
     def _init_button_box(self):
         """ Initialize the central dialog buttons.  """
         button_box = QDialogButtonBox(QDialogButtonBox.Ok | QDialogButtonBox.Cancel)
         button_box.accepted.connect(self.onAccept)
         button_box.rejected.connect(self.onReject)
         button_box.setContentsMargins(0, 35, 0, 0)
         return button_box
 
     def docksWidget(self) -> DockTabsWidget:
         if not hasattr(self, '_docks_widget'):
             self._docks_widget = DockTabsWidget(self, self._context)
         return self._docks_widget
 
+    @logmethod()
     def onAccept(self):
         # Return the transformed input when user triggered the OK-button.
         codec_frames = self._codec_tab_widget.frames().getFrames()
         print(codec_frames[-1].getInputText(), end='')
         self._application_was_canceled = False
         self.close()
 
+    @logmethod()
     def onReject(self):
         # Return the initial user input (here: no change) when user cancelled application.
         print(self._user_input, end='')
         self.close()
```

### Comparing `decoder-plus-plus-1.5.0/dpp/ui/dialog/__init__.py` & `decoder-plus-plus-1.7.0/dpp/ui/dialog/__init__.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.5.0/dpp/ui/dialog/config_dialog.py` & `decoder-plus-plus-1.7.0/dpp/ui/dialog/config_dialog.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 class ConfigDialog(QDialog):
     TAB_ABOUT = "About"
     TAB_PLUGINS = "Plugins"
     TAB_KEYBOARD_SHORTCUTS = "Keyboard Shortcuts"
 
     def __init__(self, parent, context: 'core.context.Context', select_tab_name: str = None):
         """
-        Initializes the hidden dialog.
+        Initializes the config dialog.
         :param parent: the widget which is calling the dialog.
         :param context: the context of the application.
         :param select_tab_name: the tab name which should be selcted.
         """
         super().__init__(parent)
         self._context = context
         layout = QHBoxLayout()
@@ -55,31 +55,31 @@
 
         self._init_tab_selection(tabs, select_tab_name)
 
         layout.addWidget(tabs)
 
         self.setLayout(layout)
         self.setMinimumWidth(640)
-        self.setWindowTitle(" ")
+        self.setWindowTitle("Configuration")
 
     def _init_tab_selection(self, tabs: QTabWidget, tab_name: str):
         """ Selects the tab with the specified name. """
         for tab_index in range(len(tabs)):
             text = tabs.tabText(tab_index)
             if text == tab_name:
                 tabs.setCurrentIndex(tab_index)
 
     def _init_about_tab(self):
         tab = QWidget(self)
         base_layout = QHBoxLayout()
         base_layout.setAlignment(QtCore.Qt.AlignVCenter)
         if datetime.now().month == 12:
-            logo = os.path.join(self._context.getAppPath(), 'images', 'dpp_xmas.png')
+            logo = os.path.join(self._context.getAppPath(), 'images', 'dpp_xmas_stylized.png')
         else:
-            logo = os.path.join(self._context.getAppPath(), 'images', 'dpp.png')
+            logo = os.path.join(self._context.getAppPath(), 'images', 'dpp_stylized.png')
         icon_frame = QFrame()
         icon_layout = QHBoxLayout()
         icon_label = IconLabel(self, QIcon(logo))
         icon_label.mouseDoubleClickEvent = lambda evt: self._context.toggleDebugMode()
         icon_label.setFixedSize(QSize(180, 180))
         icon_layout.setAlignment(QtCore.Qt.AlignLeft)
         icon_layout.setContentsMargins(10, 10, 10, 10)
```

### Comparing `decoder-plus-plus-1.5.0/dpp/ui/dialog/keyboard_shortcut_dialog.py` & `decoder-plus-plus-1.7.0/dpp/ui/dialog/keyboard_shortcut_dialog.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.5.0/dpp/ui/dialog/plugin_config_dialog.py` & `decoder-plus-plus-1.7.0/dpp/ui/dialog/plugin_config_dialog.py`

 * *Files 27% similar despite different names*

```diff
@@ -11,133 +11,127 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 from qtpy.QtCore import Qt
-from qtpy.QtWidgets import QHBoxLayout, QSizePolicy, QFrame, QLabel, QDialog, QDialogButtonBox, QVBoxLayout, QShortcut
+from qtpy.QtWidgets import QFrame, QDialog, QDialogButtonBox, QVBoxLayout, QShortcut
 
 from dpp.core.icons import icon, Icon
 from dpp.core.plugin import AbstractPlugin
-from dpp.core.plugin.config.ui.layouts import VBoxLayout
-from dpp.core.plugin.config.ui.widgets import TextPreview, GroupBox
 from dpp.core.shortcuts import KeySequence
-from dpp.ui import IconLabel
 from dpp.ui.builder.plugin_config_widget_builder import PluginConfigWidgetBuilder
+from dpp.ui.widget.message_box_widget import MessageBox
 
 
 class PluginConfigDialog(QDialog):
 
     def __init__(self, context, plugin: AbstractPlugin, input_text: str):
         super(PluginConfigDialog, self).__init__()
         self._context = context
         self._input_text = input_text
 
         # Dialog operates on a copy of the plugin and its configuration. This allows that configuration changes made
         # in the dialog do not have an immediate effect to the real configuration. Synchronization with original
         # configuration occurs when the accept button is pressed.
         self._plugin_clone = plugin.clone()
-        self._plugin_clone.config.onChange.connect(lambda keys: self._on_config_change())
 
-        self._widget = PluginConfigWidgetBuilder(self, self._plugin_clone, input_text).layout(
-            lambda layout_spec: VBoxLayout(
-                widgets=[
-                    GroupBox(label='Options', layout=layout_spec),
-                    GroupBox(label='Preview', layout=VBoxLayout(
-                        widgets=[TextPreview(self._plugin_clone, self._input_text)]
-                    ))
-                ]
-            )
-        ).build()
+        self._widget = PluginConfigWidgetBuilder(self, self._plugin_clone, input_text).build()
 
         self._main_layout = self._init_main_layout(self._widget)
         self._init_shortcuts()
-        self._validate_options()
+        self._validate_options(input_text)
         self.setLayout(self._main_layout)
         self.setWindowTitle(plugin.name)
         if plugin.icon:
             self.setWindowIcon(icon(plugin.icon))
 
         # Synchronize cloned configuration with the original one.
         self.accepted.connect(lambda: plugin.config.update(self._plugin_clone.config))
 
+        # Handle success and error on plugin run.
+        # Remember: onSuccess/onError is usually being run by the preview window.
+        self._plugin_clone.onSuccess.connect(self._show_success_message)
+        self._plugin_clone.onError.connect(self._show_error_message)
+
     def _init_main_layout(self, widget):
         main_layout = QVBoxLayout()
         main_layout.addWidget(self._init_input_frame(widget))
-        main_layout.addWidget(self._init_error_frame())
+        main_layout.addWidget(self._init_message_box(widget))
         main_layout.addWidget(self._init_button_box())
         return main_layout
 
     def _init_input_frame(self, widget) -> QFrame:
         input_frame = QFrame()
         input_frame_layout = QVBoxLayout()
         input_frame_layout.addWidget(widget)
         input_frame.setLayout(input_frame_layout)
         return input_frame
 
-    def _init_error_frame(self):
-        frm = QFrame()
-        frm_layout = QVBoxLayout()
-        self._error_frame = QFrame()
-        self._error_frame.setStyleSheet("background-color: black;")
-        layout = QHBoxLayout()
-        layout.setContentsMargins(15, 15, 15, 15)
-        lbl_error = IconLabel(self, icon(Icon.MSG_ERROR, color='red'))
-        layout.addWidget(lbl_error)
-        self._error_text = QLabel("")
-        self._error_text.setStyleSheet('QLabel { color: white }')
-        self._error_text.setSizePolicy(QSizePolicy.Expanding, QSizePolicy.Fixed)
-        layout.addWidget(self._error_text)
-        self._error_frame.setLayout(layout)
-        self._error_frame.setHidden(True)
-        frm_layout.addWidget(self._error_frame)
-        frm_layout.setContentsMargins(10, 0, 10, 10)
-        frm.setLayout(frm_layout)
-        return frm
-
     def _init_button_box(self):
         frm = QFrame()
         frm_layout = QVBoxLayout()
         self._btn_box = QDialogButtonBox(QDialogButtonBox.Ok | QDialogButtonBox.Cancel)
         self._btn_box.accepted.connect(self.accept)
         self._btn_box.rejected.connect(self.reject)
         frm_layout.addWidget(self._btn_box)
         frm.setLayout(frm_layout)
         return frm
 
+    def _init_message_box(self, parent):
+        self._message_box = MessageBox(self)
+        self._message_box.hide()
+        return self._message_box
+
     def _init_shortcuts(self):
-        def _accept(self):
-            if self._btn_box(QDialogButtonBox.Ok).isEnabled():
+        def _accept():
+            if self._btn_box.button(QDialogButtonBox.Ok).isEnabled():
                 self.accept()
 
         ctrl_return_shortcut = QShortcut(KeySequence(Qt.CTRL, Qt.Key_Return), self)
         ctrl_return_shortcut.activated.connect(_accept)
         alt_return_shortcut = QShortcut(KeySequence(Qt.ALT, Qt.Key_Return), self)
         alt_return_shortcut.activated.connect(_accept)
         alt_o_shortcut = QShortcut(KeySequence(Qt.ALT, Qt.Key_O), self)
         alt_o_shortcut.activated.connect(_accept)
 
-    def _on_config_change(self):
-        """ Update and validate options when change occurred. """
-        self._validate_options()
-
-    def _validate_options(self):
+    def _validate_options(self, input_text, option_keys=None):
         """ Update and validate options. """
+        # TODO: Indicate error on the individual widgets instead.
+        #       This method has the disadvantage that we can only show one error message at a time.
+        #       In addition the error message might not indicate directly which widget/field is responsible.
         try:
-            self._plugin_clone.run(self._input_text)
-            self._reset_errors()
+            self._plugin_clone.validate_options(input_text, option_keys)
         except BaseException as err:
             self._show_error_message(str(err))
 
-    def _reset_errors(self):
-        """ Hides error message box and resets any error indicators. """
+    def _hide_message_box(self):
+        """ Hide message box and enable OK button. """
         self._btn_box.button(QDialogButtonBox.Ok).setEnabled(True)
-        self._error_frame.setHidden(True)
-        self._error_text.setText("")
+        self._message_box.setHidden(True)
 
     def _show_error_message(self, message):
-        """ Shows an error message within a error-box. """
+        """ Shows an error message within a message-box. """
+        if not message:
+            self._hide_message_box()
+            return
         self._btn_box.button(QDialogButtonBox.Ok).setEnabled(False)
+        self._message_box.setFrameStyle("background-color: black;")
+        self._message_box.setTextStyle("QLabel { color: white }")
+        self._message_box.setIcon(Icon.MSG_ERROR, color='red')
+        self._message_box.setText(message)
+        self._message_box.setHidden(False)
+        self._context.logger.debug(message)
+
+    def _show_success_message(self, message):
+        """ Shows a success message within a message box. """
+        if not message:
+            self._hide_message_box()
+            return
+        self._btn_box.button(QDialogButtonBox.Ok).setEnabled(True)
+        self._message_box.setFrameStyle("background-color: white;")
+        self._message_box.setTextStyle("QLabel { color: black }")
+        self._message_box.setIcon(Icon.MSG_INFO, color='blue')
+        self._message_box.setText(message)
+        self._message_box.setHidden(False)
         self._context.logger.debug(message)
-        self._error_frame.setHidden(False)
-        self._error_text.setText(message)
```

### Comparing `decoder-plus-plus-1.5.0/dpp/ui/dock/hex_dock.py` & `decoder-plus-plus-1.7.0/dpp/ui/dock/hex_dock.py`

 * *Files 0% similar despite different names*

```diff
@@ -243,15 +243,15 @@
                                                     bytearray.fromhex(hex_string).decode('utf-8',
                                                                                          errors='surrogateescape'))
         self.blockSignals(False)
 
     def _on_selection_change(self, tab_id: str, frame_id: str, input_text: str):
         self._update_view(tab_id, frame_id, input_text)
 
-    def _on_text_change(self, tab_id: str, frame_id: str, input_text: str, user_interaction: bool):
+    def _on_text_change(self, tab_id: str, frame_id: str, input_text: str):
         self._update_view(tab_id, frame_id, input_text)
 
     def _on_selected_frame_change(self, tab_id: str, frame_id: str, input_text: str):
         self._frame_id = frame_id
         self._update_view(tab_id, frame_id, input_text)
 
     #############################################
```

### Comparing `decoder-plus-plus-1.5.0/dpp/ui/dock/log_dock.py` & `decoder-plus-plus-1.7.0/dpp/ui/dock/log_dock.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.5.0/dpp/ui/instance_handler.py` & `decoder-plus-plus-1.7.0/dpp/ui/instance_handler.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.5.0/dpp/ui/view/__init__.py` & `decoder-plus-plus-1.7.0/dpp/ui/view/__init__.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.5.0/dpp/ui/view/classic/__init__.py` & `decoder-plus-plus-1.7.0/dpp/ui/view/classic/__init__.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.5.0/dpp/ui/view/classic/classic_main_window_widget.py` & `decoder-plus-plus-1.7.0/dpp/ui/view/classic/classic_main_window_widget.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 #
 import json
 
 from qtpy.QtWidgets import QFileDialog, QWidget
 
+from dpp.core.logger import logmethod
 from dpp.core.plugin import PluginType
 from dpp.ui.view.classic import CodecTab
 from dpp.ui.view.classic.codec_frame import CodecFrame
 from dpp.ui.view.main_window_widget import MainWindowWidget, menu, MenuItem
 
 
 class ClassicMainWindowWidget(MainWindowWidget):
@@ -83,51 +84,48 @@
 
     @menu.register_menu_item(id=MenuItem.FOCUS_INPUT_TEXT, text="Select &Text Field", shortcut_key="Alt+Shift+I")
     def _select_text_field_action(self):
         self._call_focused_frame(lambda focused_frame: focused_frame.focusInputText())
 
     @menu.register_menu_item(id=MenuItem.FOCUS_INPUT_TEXT_NEXT, text="Select &Next Text Field", shortcut_key="Alt+Down")
     def _focus_next_input_text_action(self):
-        self._focus_input_text(lambda frame: frame.getNextFrame())
+        focused_frame = self._get_focused_frame()
+        if focused_frame and focused_frame.hasNextFrame():
+            self._focus_input_text(focused_frame.getNextFrame())
 
     @menu.register_menu_item(id=MenuItem.FOCUS_INPUT_TEXT_PREVIOUS, text="Select &Previous Text Field",
                              shortcut_key="Alt+Up")
     def _focus_previous_input_text_action(self):
-        self._focus_input_text(lambda frame: frame.getPreviousFrame())
+        focused_frame = self._get_focused_frame()
+        if focused_frame and focused_frame.hasPreviousFrame():
+            self._focus_input_text(focused_frame.getPreviousFrame())
 
     #############################################
     # Helper functions
     #############################################
 
     def _call_focused_frame(self, callback):
         focused_frame = self._get_focused_frame()
         if focused_frame:
             callback(focused_frame)
 
     def _get_focused_frame(self) -> CodecFrame:
         return self.tabsWidget().currentWidget().frames().getFocusedFrame()
 
-    def _focus_input_text(self, callback):
-        frame = self._get_focused_frame()
-        if frame:
-            future_frame = callback(frame) or frame
-            future_frame.focusInputText()
-            # Collapse/Uncollapse frames automatically.
-            if self.tabsWidget().currentWidget().frames().getFramesCount() > 2:
-                if frame != future_frame:
-                    if future_frame.isCollapsed():
-                        if future_frame.hasPreviousFrame():
-                            # Toggle frame, except the first frame which does not have a header
-                            future_frame.toggleCollapsed()
-                    if not frame.wasCollapseStateChangedByUser():
-                        if frame.hasPreviousFrame():
-                            # Collapse frame, except the first frame which does not have a header
-                            frame.toggleCollapsed()
-
-            self.tabsWidget().currentWidget().ensureWidgetVisible(future_frame)
+    def _focus_input_text(self, future_frame: CodecFrame):
+        focused_frame = self._get_focused_frame()
+        # Only collapse if frame was not manually collapsed by user and is not first or last frame
+        if not focused_frame.wasCollapseStateChangedByUser():
+            is_first_or_last_frame = not focused_frame.hasPreviousFrame() or not focused_frame.hasNextFrame()
+            if not is_first_or_last_frame:
+                focused_frame.setCollapsed(True)
+
+        future_frame.focusInputText()
+        future_frame.setCollapsed(False)
+        self.tabsWidget().currentWidget().ensureWidgetVisible(future_frame)
 
     #############################################
     # Connector functions
     #############################################
 
     @menu.register_menu_item(id=MenuItem.OPEN_FILE, text="&Open File...", shortcut_key="Ctrl+O")
     def _open_file_action(self):
@@ -149,44 +147,48 @@
                             frame.setStatus(frame_config["status"]["type"], frame_config["status"]["message"])
                         else:
                             frame = tab.frames().newFrame(frame_config["text"],
                                                           frame_config["title"],
                                                           frame_index,
                                                           frame_config["status"]["type"],
                                                           frame_config["status"]["message"])
-                        frame.fromDict(frame_config)
+                        frame.fromDict(frame_config, safe_mode=True)
                         frame_index = frame_index + 1
             self._context.logger.info("Successfully loaded {}!".format(filename))
         except Exception as e:
             self._context.logger.error("Unexpected error loading file. {}".format(e))
 
     @menu.register_menu_item(id=MenuItem.SAVE_AS_FILE, text="&Save As...", shortcut_key="Ctrl+S")
     def _save_as_file_action(self):
         filename, _ = QFileDialog.getSaveFileName(self, 'Save As File')
         if not filename:
             return
 
         try:
-            self._context.saveAsFile(filename, str(json.dumps(self.toDict(), default=lambda x: x.__dict__)))
+            content = str(json.dumps(self.toDict(), default=lambda x: x.__dict__))
+            with open(filename, "w") as f:
+                f.write(content)
             self._context.logger.info("Successfully saved session in {}!".format(filename))
         except Exception as e:
             self._context.logger.error("Unexpected error saving file. {}".format(e))
 
     #############################################
     # Public functions
     #############################################
 
+    @logmethod()
     def newTab(self, title: str = None, input_text: str = None, widget: QWidget = None) -> (int, QWidget):
         tab = CodecTab(self, self._context, self._plugins)
         tab.frames().getFocusedFrame().setInputText(input_text)
         # BUG: Input-text of newly added codec-tab is not focused correctly.
         # FIX: Refocus input-text.
         tab.frames().getFocusedFrame().focusInputText()
         return super().newTab(title, input_text, tab)
 
+    @logmethod()
     def duplicateTab(self, title, src_tab):
         tab_index, dst_tab = self.newTab(title=title)
         frame_index = 0
         for src_frame in src_tab.frames().getFrames():
             status_type, status_message = src_frame.status()
             if frame_index == 0:
                 # New tabs already contain one empty frame
@@ -198,12 +200,13 @@
                                           src_frame.title(),
                                           frame_index,
                                           status_type,
                                           status_message)
             dst_tab.frames().getFrameByIndex(frame_index).fromDict(src_frame.toDict())
             frame_index = frame_index + 1
 
+    @logmethod()
     def toDict(self):
         return [{
             "name": self.tabsWidget().tabBar().tabText(tabIndex),
             "frames": self.tabsWidget().tab(tabIndex).toDict()
         } for tabIndex in range(0, self.tabsWidget().tabCount())]
```

### Comparing `decoder-plus-plus-1.5.0/dpp/ui/view/classic/codec_frame.py` & `decoder-plus-plus-1.7.0/dpp/ui/view/classic/codec_frame.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,50 +10,68 @@
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
+import dataclasses
 import uuid
+from typing import List
 
 from qtpy import QtCore
 from qtpy.QtCore import Signal
 from qtpy.QtWidgets import QFrame, QVBoxLayout
 
 from dpp.core import Context
+from dpp.core.logger import logmethod
 from dpp.core.plugin import PluginType, AbstractPlugin, NullPlugin
 from dpp.core.plugin.manager import PluginManager
 from dpp.core.plugin.builder import PluginBuilder
 from dpp.ui import VSpacer
 from dpp.ui.view.classic.codec_frame_header import CodecFrameHeader
 from dpp.ui.view.classic.combo_box_frame import ComboBoxFrame
 from dpp.ui.widget.plain_view import PlainView
 from dpp.ui.widget.collapsible_frame import CollapsibleFrame
 from dpp.ui.widget.identify_format_button import IdentifyFormatButton
 from dpp.ui.widget.smart_decode_button import SmartDecodeButton
 from dpp.ui.widget.status_widget import StatusWidget
 
 
 class CodecFrame(CollapsibleFrame):
-    # frame_id
-    refreshButtonClicked = Signal(str)
-    # frame_id
-    upButtonClicked = Signal(str)
-    # frame_id
-    downButtonClicked = Signal(str)
-    # frame_id
-    configButtonClicked = Signal(str)
-    # frame_id
-    closeButtonClicked = Signal(str)
-    # frame_id, input_text, combo_box_type, combo_box_index, plugin
-    pluginSelected = Signal(str, str, str, int, 'PyQt_PyObject')
-    # frame_id, combo_box_type
-    pluginDeselected = Signal(str, str)
 
+    # Signals that the frame was focused
+    selectedFrameChanged = Signal(str, str, str)  # tab_id, frame_id, input_text
+
+    # Signals that the text inside the codec frame changed
+    textChanged = Signal(str, str, str)  # tab_id, frame_id, input_text
+
+    # Signals that the text selection inside the codec frame changed
+    textSelectionChanged = Signal(str, str, str)  # tab_id, frame_id, input_text
+
+    # Signals that the text inside the codec frame should be updated
+    refreshButtonClicked = Signal(str)  # frame_id
+
+    # Signals that the frame should be repositioned
+    upButtonClicked = Signal(str)  # frame_id
+    downButtonClicked = Signal(str)  # frame_id
+    configButtonClicked = Signal(str)  # frame_id
+    closeButtonClicked = Signal(str)  # frame_id
+
+    # Signals that the selected plugin changed
+    pluginSelected = Signal(str, 'PyQt_PyObject')  # frame_id, plugin
+
+    @dataclasses.dataclass
+    class TextSelection:
+        start: int
+        end: int
+        color: str
+        plugin: AbstractPlugin
+
+    @logmethod()
     def __init__(self, parent, context: Context, tab_id: str, codec_frames, plugins: PluginManager, text):
         super().__init__(parent, context, uuid.uuid4().hex)
 
         self._tab_id = tab_id
         self._codec_frames = codec_frames
         self._context.shortcutUpdated.connect(self._shortcut_updated_event)
         self._plugins = plugins
@@ -64,14 +82,17 @@
         self.addWidget(self._init_input_frame(text))
         self.addWidget(self._init_button_frame())
 
         self._init_header()
 
         self.show()
 
+    # ------------------------------------------------------------------------------------------------------------------
+
+    @logmethod(prefix_callback=lambda self: f'{self.getFrameId()}::')
     def _init_header(self):
 
         self._header_frame.addWidget(CodecFrameHeader.IndicatorHeaderItem(self))
         self._header_frame.addWidget(CodecFrameHeader.ContentPreviewHeaderItem(self))
 
         self._header_frame.addWidget(CollapsibleFrame.HeaderFrame.VSepItem(self))
         self._header_frame.addWidget(CodecFrameHeader.TitleHeaderItem(self))
@@ -84,60 +105,66 @@
         self._header_frame.addWidget(CodecFrameHeader.EntropyInfoHeaderItem(self))
         self._header_frame.addWidget(CollapsibleFrame.HeaderFrame.VSepItem(self))
 
         def button_clicked_event(event, signal):
             if event.button() == QtCore.Qt.LeftButton:
                 signal.emit(self.id())
 
-        up_button_header_item = CodecFrameHeader.UpButtonHeaderItem(self)
-        up_button_header_item.clicked.connect(lambda evt: button_clicked_event(evt, self.upButtonClicked))
-        self._header_frame.addWidget(up_button_header_item)
-
-        down_button_header_item = CodecFrameHeader.DownButtonHeaderItem(self)
-        down_button_header_item.clicked.connect(lambda evt: button_clicked_event(evt, self.downButtonClicked))
-        self._header_frame.addWidget(down_button_header_item)
-
-        refresh_button_header_item = CodecFrameHeader.RefreshButtonHeaderItem(self)
-        refresh_button_header_item.clicked.connect(lambda evt: button_clicked_event(evt, self.refreshButtonClicked))
-        self._header_frame.addWidget(refresh_button_header_item)
-
-        config_button_header_item = CodecFrameHeader.ConfigButtonHeaderItem(self)
-        config_button_header_item.clicked.connect(lambda evt: button_clicked_event(evt, self.configButtonClicked))
-        self._header_frame.addWidget(config_button_header_item)
-
-        close_button_header_item = CodecFrameHeader.CloseButtonHeaderItem(self)
-        close_button_header_item.clicked.connect(lambda evt: button_clicked_event(evt, self.closeButtonClicked))
-        self._header_frame.addWidget(close_button_header_item)
+        def init_button(button, signal):
+            button.clicked.connect(lambda evt: button_clicked_event(evt, signal))
+            self._header_frame.addWidget(button)
+            return button
+
+        self._move_up_button = init_button(CodecFrameHeader.UpButtonHeaderItem(self), self.upButtonClicked)
+        self._move_down_button = init_button(CodecFrameHeader.DownButtonHeaderItem(self), self.downButtonClicked)
+        self._refresh_button = init_button(CodecFrameHeader.RefreshButtonHeaderItem(self), self.refreshButtonClicked)
+        self._config_button = init_button(CodecFrameHeader.ConfigButtonHeaderItem(self), self.configButtonClicked)
+        self._close_button = init_button(CodecFrameHeader.CloseButtonHeaderItem(self), self.closeButtonClicked)
+
+    def getMoveUpButton(self) -> CodecFrameHeader.ClickableCodecFrameHeaderItem:
+        return self._move_up_button
+
+    def getMoveDownButton(self) -> CodecFrameHeader.ClickableCodecFrameHeaderItem:
+        return self._move_down_button
+
+    def getRefreshButton(self) -> CodecFrameHeader.ClickableCodecFrameHeaderItem:
+        return self._refresh_button
+
+    def getConfigButton(self) -> CodecFrameHeader.ClickableCodecFrameHeaderItem:
+        return self._config_button
+
+    def getCloseButton(self) -> CodecFrameHeader.ClickableCodecFrameHeaderItem:
+        return self._close_button
 
+    # ------------------------------------------------------------------------------------------------------------------
+
+    @logmethod(prefix_callback=lambda self: f'{self.getFrameId()}::')
     def _init_input_frame(self, text):
         input_frame = QFrame(self)
         frame_layout = QVBoxLayout()
         self._plain_view_widget = PlainView(self._tab_id, self._frame_id, text, self._context, self)
+        self._plain_view_widget.selectedFrameChanged.connect(self.selectedFrameChanged.emit)
+        self._plain_view_widget.textSelectionChanged.connect(self.textSelectionChanged.emit)
+        self._plain_view_widget.textChanged.connect(self.textChanged.emit)
+
         frame_layout.addWidget(self._plain_view_widget)
         frame_layout.setContentsMargins(0, 6, 6, 6)
         input_frame.setLayout(frame_layout)
         return input_frame
 
+    @logmethod(prefix_callback=lambda self: f'{self.getFrameId()}::')
     def _init_button_frame(self):
         button_frame = QFrame(self)
         button_frame_layout = QVBoxLayout()
         self._combo_box_frame = ComboBoxFrame(self, self._context)
-        self._combo_box_frame.pluginSelected.connect(lambda combo_box_type, combo_box_index, plugin:
+        self._combo_box_frame.pluginSelected.connect(lambda plugin:
                                                      self.pluginSelected.emit(
                                                          self.id(),
-                                                         self.getInputText(),
-                                                         combo_box_type,
-                                                         combo_box_index,
                                                          plugin
                                                      ))
-        self._combo_box_frame.pluginDeselected.connect(lambda combo_box_type:
-                                                       self.pluginDeselected.emit(
-                                                           self.id(),
-                                                           combo_box_type
-                                                       ))
         button_frame_layout.addWidget(self._combo_box_frame)
         self._smart_decode_button = SmartDecodeButton(self,
                                                       self._plugins.filter(type=PluginType.DECODER),
                                                       self._plain_view_widget.toPlainText,
                                                       self.selectComboBoxEntryByPlugin)
         button_frame_layout.addWidget(self._smart_decode_button)
         self._identify_format_button = IdentifyFormatButton(self,
@@ -146,14 +173,15 @@
                                                             self._plain_view_widget.toPlainText,
                                                             self.selectComboBoxEntryByPlugin)
         button_frame_layout.addWidget(self._identify_format_button)
         button_frame_layout.addWidget(VSpacer(self))
         button_frame.setLayout(button_frame_layout)
         return button_frame
 
+    @logmethod(prefix_callback=lambda self: f'{self.getFrameId()}::')
     def _shortcut_updated_event(self, shortcut):
         tooltip = self._get_tooltip_by_shortcut(shortcut)
         combo_box_type = self._get_combo_box_type_by_shortcut(shortcut)
         self._combo_box_frame.setToolTip(tooltip, combo_box_type)
 
     def _get_combo_box_type_by_shortcut(self, shortcut) -> str:
         combo_box_shortcut_map = {
@@ -169,82 +197,97 @@
 
     def id(self) -> str:
         return self._frame_id
 
     def getPlugin(self) -> AbstractPlugin:
         """ Returns the currently selected plugin. Might return a NullPlugin when nothing is selected. """
         # A bit dirty, but might be called before initialization (see Frame::isConfigurable)
-        if hasattr(self,'_combo_box_frame'):
+        if hasattr(self, '_combo_box_frame'):
             return self._combo_box_frame.selectedPlugin()
         else:
             return NullPlugin(self._context)
 
     def hasStatus(self, status_name: str) -> bool:
         return self._status_widget.hasStatus(status_name)
 
-    def status(self):
+    def status(self) -> (str, str):
         return self._status_widget.status()
 
+    @logmethod(prefix_callback=lambda self: f'{self.getFrameId()}::')
     def setStatus(self, type, message):
-        self._logger.trace(f'{self.getFrameId()}::statusChanged({type}, {message})')
         self._header_frame.setStatus(type, message)
         self._status_widget.setStatus(type, message)
 
+    # ------------------------------------------------------------------------------------------------------------------
+
+    def hasTextSelected(self) -> bool:
+        return self._plain_view_widget.hasTextSelected()
+
+    def getTextSelections(self) -> List[TextSelection]:
+        # TODO:
+        ...
+
+    def getSelectedText(self) -> TextSelection:
+        # TODO:
+        ...
+
+    # ------------------------------------------------------------------------------------------------------------------
+
+    @logmethod(prefix_callback=lambda self: f'{self.getFrameId()}::')
     def selectComboBoxEntryByPlugin(self, plugin, block_signals=False):
-        self._logger.trace(f'{self.getFrameId()}::selectComboBoxEntryByPlugin({plugin.name}, {str(block_signals)})')
-        self._combo_box_frame.selectItem(plugin.type, plugin.name, block_signals=True)
-        if not block_signals:
-            combo_box_type = plugin.type
-            combo_box_index = self._combo_box_frame.index(combo_box_type)
-            self.pluginSelected.emit(self.id(), self.getInputText(), combo_box_type, combo_box_index, plugin)
+        self._combo_box_frame.selectItem(plugin.type, plugin.name, block_signals=block_signals)
 
+    @logmethod(prefix_callback=lambda self: f'{self.getFrameId()}::')
     def toggleSearchField(self):
-        self._logger.trace(f'{self.getFrameId()}::toggleSearchField()')
         self._plain_view_widget.toggleSearchField()
 
+    @logmethod(prefix_callback=lambda self: f'{self.getFrameId()}::')
     def setInputText(self, text):
-        self._logger.trace(f'{self.getFrameId()}::setInputText({text})')
-        self._plain_view_widget.blockSignals(True)
         self._plain_view_widget.setPlainText(text)
-        self._plain_view_widget.blockSignals(False)
         self.header().refresh()
 
     def getInputText(self) -> str:
         return self._plain_view_widget.toPlainText()
 
+    def getOutputText(self) -> str:
+        return self.getPlugin().run(self.getInputText())
+
     def getComboBoxes(self):
         return self._combo_box_frame
 
+    @logmethod(prefix_callback=lambda self: f'{self.getFrameId()}::')
     def cutSelectedInputText(self):
-        self._logger.trace(f'{self.getFrameId()}::cutSelectedInputText()')
         self._plain_view_widget.cutSelectedInputText()
 
+    @logmethod(prefix_callback=lambda self: f'{self.getFrameId()}::')
     def copySelectedInputText(self):
-        self._logger.trace(f'{self.getFrameId()}::copySelectedInputText()')
         self._plain_view_widget.copySelectedInputText()
 
+    @logmethod(prefix_callback=lambda self: f'{self.getFrameId()}::')
     def pasteSelectedInputText(self):
-        self._logger.trace(f'{self.getFrameId()}::pasteSelectedInputText()')
         self._plain_view_widget.pasteSelectedInputText()
 
+    @logmethod(prefix_callback=lambda self: f'{self.getFrameId()}::')
     def focusInputText(self):
-        self._logger.trace(f'{self.getFrameId()}::focusInputText()')
         self._plain_view_widget.setFocus()
 
     def hasFocus(self):
         return self._plain_view_widget.hasFocus()
 
+    @logmethod(prefix_callback=lambda self: f'{self.getFrameId()}::')
     def focusComboBox(self, type):
         self._combo_box_frame.focusType(type)
 
+    @logmethod(prefix_callback=lambda self: f'{self.getFrameId()}::')
     def setPlugin(self, plugin: AbstractPlugin, block_signals=True):
         if plugin:
+            assert isinstance(plugin, AbstractPlugin), "Plugin must be of type AbstractPlugin"
             self.selectComboBoxEntryByPlugin(plugin, block_signals=block_signals)
             self.getPlugin().setup(plugin.config.toDict())
-            self.frameChanged.emit(self.id())
+            self.selectedFrameChanged.emit(self._tab_id, self.id(), self.getInputText())
 
     def title(self) -> str:
         """ Returns the title of the current frame which is either the title of the previous plugin or None. """
         if self.hasPreviousFrame():
             return self.getPreviousFrame().getPlugin().title
 
     def name(self) -> str:
@@ -277,18 +320,14 @@
         """ Returns the index of the codec frame. """
         return self._codec_frames.getFrameIndex(self._frame_id)
 
     def getFrameId(self) -> str:
         """ Returns the id of the codec frame. """
         return self._frame_id
 
-    def getFrame(self) -> 'dpp.ui.codec_frame.CodecFrame':
-        """ Returns the current frame if exists, otherwise an exception is thrown. """
-        return self._codec_frames.getFrameByIndex(self.getFrameIndex())
-
     def hasPreviousFrame(self) -> bool:
         """ Checks whether there is a previous frame. Returns either True or False. """
         return self._codec_frames.hasPreviousFrame(self.getFrameIndex())
 
     def getPreviousFrame(self) -> 'dpp.ui.codec_frame.CodecFrame':
         """ Returns the previous frame if any, otherwise an exception is thrown. """
         return self._codec_frames.getFrameByIndex(self.getFrameIndex() - 1)
@@ -297,24 +336,33 @@
         """ Checks whether there is a next frame. Returns either True or False. """
         return self._codec_frames.hasNextFrame(self.getFrameIndex())
 
     def getNextFrame(self) -> 'dpp.ui.codec_frame.CodecFrame':
         """ Returns the next frame if any, otherwise an exception is thrown. """
         return self._codec_frames.getFrameByIndex(self.getFrameIndex() + 1)
 
-    def fromDict(self, frame_config):
+    # ------------------------------------------------------------------------------------------------------------------
+
+    @logmethod(prefix_callback=lambda self: f'{self.getFrameId()}::')
+    def fromDict(self, frame_config, safe_mode: bool = False):
+        """ Setups a tab from a given configuration.
+        @param frame_config: configuration of a frame. See toDict method for more information.
+        @param safe_mode: dictates how potentially dangerous plugins are handled.
+        """
         self.setInputText(frame_config["text"])
         self.setStatus(frame_config["status"]["type"], frame_config["status"]["message"])
-        if frame_config["plugin"]["name"] and frame_config["plugin"]["type"]:
+        plugin = frame_config["plugin"]
+        if plugin["name"] and plugin["type"]:
             # Configure plugin if any. Last frame does not have a plugin configured, yet.
-            self.selectComboBoxEntryByPlugin(PluginBuilder(self._context).build(frame_config["plugin"]),
+            self.selectComboBoxEntryByPlugin(PluginBuilder(self._context).build(plugin, safe_mode),
                                              block_signals=True)
         self.header().refresh()
         self.setCollapsed(frame_config["is_collapsed"])
 
+    @logmethod(prefix_callback=lambda self: f'{self.getFrameId()}::')
     def toDict(self):
         status_type, status_message = self._status_widget.status()
         return {
             "title": self.title,
             "text": self.getInputText(),
             "is_collapsed": self.isCollapsed(),
             "status": {
```

### Comparing `decoder-plus-plus-1.5.0/dpp/ui/view/classic/codec_frame_header.py` & `decoder-plus-plus-1.7.0/dpp/ui/view/classic/codec_frame_header.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.5.0/dpp/ui/view/classic/codec_frames.py` & `decoder-plus-plus-1.7.0/dpp/ui/view/classic/codec_frames.py`

 * *Files 27% similar despite different names*

```diff
@@ -10,18 +10,19 @@
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
-from typing import List
+from typing import List, Tuple, Dict
 
 from qtpy.QtWidgets import QDialog, QFrame, QVBoxLayout
 
+from dpp.core.logger import logmethod
 from dpp.core.plugin import AbstractPlugin
 from dpp.ui.dialog.plugin_config_dialog import PluginConfigDialog
 from dpp.ui.view.classic.codec_frame import CodecFrame
 from dpp.ui.widget.status_widget import StatusWidget
 
 
 class CodecFrames(QFrame):
@@ -30,257 +31,220 @@
         super(__class__, self).__init__(parent)
         self._context = context
         self._tab_id = tab_id
         self._plugins = plugins
         self._frames_layout = QVBoxLayout()
         self.setLayout(self._frames_layout)
         self._frames_layout.setContentsMargins(0, 0, 0, 0)
-        self._init_listener(context)
         self._focused_frame = None
 
     # ------------------------------------------------------------------------------------------------------------------
-
-    def _init_listener(self, context):
-        self._listener = context.listener()
-
-        def selected_frame_changed(tab_id, frame_id, input_text):
-            # Always remember the currently focused frame (e.g. used for finding the currently selected frame when
-            # using keyboard-shortcuts)
-            if self._tab_id == tab_id:
-                self._focused_frame = self.getFrameById(frame_id)
-
-        self._listener.selectedFrameChanged.connect(selected_frame_changed)
-        self._listener.textChanged.connect(lambda tab_id, frame_id, text, interactive:
-            self._tab_id == tab_id and self._text_changed_event(frame_id, text, interactive))
-
+    # Private helper functions
     # ------------------------------------------------------------------------------------------------------------------
 
-    def _text_changed_event(self, frame_id, text, is_user_action=True, do_preserve_state=False):
-        frame_index = self.getFrameIndex(frame_id)
-        frame = self.getFrameById(frame_id)
-        if is_user_action:
-            frame.setStatus(StatusWidget.DEFAULT, '')
-        while frame:
-            if do_preserve_state and self.hasNextFrame(frame_index) and \
-                    self.getFrameByIndex(frame_index + 1).status() == StatusWidget.DEFAULT:
-                # Do not overwrite content of frames which are in default-state.
-                # Usually done when moving frames to a new position whereby custom user-input should not be
-                # overwritten.
-                frame = self.getFrameByIndex(frame_index + 1)
-                continue
-
-            input_text = frame.getInputText()
-            frame.header().refresh()
-            plugin = frame._combo_box_frame.selectedPlugin()
-            if not plugin.is_runnable():
-                break
-
-            frame = self._execute_plugin_run(frame.id(), input_text, plugin)
-
-    def _on_plugin_selected(self, frame_id: str, input_text: str,
-                            combo_box_type: str, combo_box_index: int, plugin: AbstractPlugin):
-        frame = self.getFrameById(frame_id)
-        if self._show_plugin_config(frame_id, input_text, plugin) != QDialog.Accepted:
-            # User clicked the cancel-button within the plugin config dialog.
-            # BUG: Item gets selected although dialog was canceled.
-            # FIX: Reselect last item prior to current selection.
-            frame.getComboBoxes().reselectLastItem(block_signals=True)
-        else:
-            # BUG: Item gets deselected when running dialogs.
-            # FIX: Reselect Item
-            frame.getComboBoxes().reselectItem(combo_box_index, combo_box_type)
-
-        # ------------------------------------------------------------------------------------------------------------------
-
-    def _execute_plugin_run(self, frame_id, input_text, plugin) -> CodecFrame:
-        frame_index = self.getFrameIndex(frame_id) + 1
-        output_text = ""
-        status = StatusWidget.SUCCESS
-        error = None
-        try:
-            output_text = plugin.run(input_text)
-        except BaseException as e:
-            status = StatusWidget.ERROR
-            error = str(e)
-            self._context.logger.error('{} {}: {}'.format(plugin.name, plugin.type, error))
-
-        return self.newFrame(output_text, plugin.title, frame_index, status=status, msg=error)
-
-    def _show_plugin_config(self, frame_id, input_text, plugin) -> int:
-        new_frame_index = self.getFrameIndex(frame_id) + 1
+    @logmethod()
+    def _configure_plugin(self, frame_id, input_text, plugin) -> bool:
+        if plugin.is_configurable():
+            if PluginConfigDialog(self._context, plugin, input_text).exec_() != QDialog.Accepted:
+                # User clicked the cancel-button within the plugin config dialog.
+                # BUG: Item gets selected although dialog was canceled.
+                # FIX: Reselect last item prior to current selection.
+                self.getFrameById(frame_id).getComboBoxes().reselectLastItem(block_signals=True)
+                return False
+        return True
+
+    @logmethod()
+    def _run_plugin(self, input_text: str, plugin: AbstractPlugin) -> Tuple[str, str, str]:
+        """
+        Runs the plugin using the input text on the frame.
+        @param input_text: the input text for the plugin.
+        @param plugin: the plugin to run.
+        @return: the new CodecFrame or None if plugin configuration failed.
+        """
         output = ""
         error = None
         try:
-            if plugin.is_configurable():
-                result = PluginConfigDialog(self._context, plugin, input_text).exec_()
-                if result != QDialog.Accepted:
-                    return result
             output = plugin.run(input_text)
             status = StatusWidget.SUCCESS
         except BaseException as err:
             status = StatusWidget.ERROR
-            self._context.logger.error(f'{plugin.name} {plugin.type}: {str(err)}')
+            error = str(err)
+            self._context.logger.error(f'{plugin.name} {plugin.type}: {error}')
             self._context.logger.debug(str(err), exc_info=True)
+        return output, status, error
 
-        self.newFrame(output, plugin.title, new_frame_index, status=status, msg=error).focusInputText()
-        return QDialog.Accepted
-
+    @logmethod()
     def _refill_frame(self, text, title, frame_index, status, msg=None):
-        self._context.logger.trace(f'Refill frame at index {frame_index}')
         if status == StatusWidget.ERROR:
             # ERROR usually indicates that codec execution failed and there is no text to display.
             # However, we indicate to the user that there is an error (setStatus) for this frame and any
             # following frame.
             frame = self.getFrameByIndex(frame_index)
             while frame_index < self.getFramesCount():
                 _frame = self.getFrameByIndex(frame_index)
                 _frame.setStatus(status, msg)
                 _frame.header().refresh()
                 # Display error only for the first frame.
                 msg = None
                 frame_index = frame_index + 1
         else:
-            # Display status and insert text into frame when there was no error.
-            # Note that setInputText may result into another call to newFrame with frame_index + 1.
             frame = self.getFrameByIndex(frame_index)
             frame.setInputText(text)
             frame.header().refresh()
             frame.setStatus(status, msg)
 
         return frame
 
-    def _on_plugin_deselected(self, frame_id):
+    @logmethod()
+    def _deselect_plugin(self, frame_id: str):
+        """ When the first combo box entry gets selected all further frames are going to be removed. """
         _frame_index = self.getFrameIndex(frame_id)
         self._context.logger.debug(f'Reset frames after index {_frame_index} up until {self.getFramesCount() - 1}')
         for frame_index in range(self.getFramesCount() - 1, _frame_index, -1):
             self._context.logger.debug(f'Reset frame with index {frame_index}')
             self.getFrameByIndex(frame_index).deleteLater()
 
-    # ------------------------------------------------------------------------------------------------------------------
+    @logmethod()
+    def _new_frame(self, frame: CodecFrame) -> CodecFrame:
+        plugin = frame.getPlugin()
+        output, status, error = self._run_plugin(frame.getInputText(), plugin)
+        new_frame_index = frame.getFrameIndex() + 1
+        return self.newFrame(output, plugin.title, new_frame_index, status=status, msg=error)
+
+    @logmethod()
+    def _update_frames(self, frame_id, is_user_action=True, do_preserve_state=False):
+        """
+        Updates all frames starting from the given frame_id.
+        @param frame_id: the frame id to start updating from.
+        @param is_user_action: defines whether the update is triggered by a user action or not.
+        @param do_preserve_state: defines whether the state of the frame should be preserved or not.
+        """
+        frame_index = self.getFrameIndex(frame_id)
+        frame = self.getFrameById(frame_id)
+        if is_user_action:
+            frame.setStatus(StatusWidget.DEFAULT, '')
+        while frame:
+            if do_preserve_state and self.hasNextFrame(frame_index) and \
+                    self.getFrameByIndex(frame_index + 1).status() == StatusWidget.DEFAULT:
+                # Do not overwrite content of frames which are in default-state.
+                # Usually done when moving frames to a new position whereby custom user-input should not be
+                # overwritten.
+                frame = self.getFrameByIndex(frame_index + 1)
+                continue
 
-    def getFrameIndex(self, frame_id) -> int:
-        frame = None
-        index = 0
-        for current_frame in self.getFrames():
-            if current_frame.id() == frame_id:
-                frame = current_frame
+            frame.header().refresh()
+            plugin = frame.getPlugin()
+            if not plugin.is_runnable():
                 break
-            index = index + 1
-        return index if frame else -1
 
-    def getFrameById(self, frame_id) -> CodecFrame:
-        for frame in self.getFrames():
-            if frame.id() == frame_id:
-                return frame
-
-    def getFrameByIndex(self, index) -> CodecFrame:
-        if self.layout().itemAt(index):
-            return self.layout().itemAt(index).widget()
-
-    def getFramesCount(self) -> int:
-        return self.layout().count()
-
-    def getFocusedFrame(self) -> CodecFrame:
-        widget = self.focusWidget()
-        while widget:
-            if isinstance(widget, CodecFrame):
-                return widget
-            widget = widget.parent()
-        return self.layout().itemAt(0).widget()
+            frame = self._update_frame(frame)
 
-    def getFrames(self) -> List[CodecFrame]:
-        frames = []
-        for frameIndex in range(0, self.layout().count()):
-            frames.append(self.layout().itemAt(frameIndex).widget())
-        return frames
+    @logmethod()
+    def _replace_input_text(self, input_text: str, replacements: Dict[str, Tuple[str, str, str]]) -> str:
+        """
+        Replaces text at the specified positions in the input text.
+        @param input_text: a string.
+        @param replacements: a dictionary of tuples. key contains the starting index, value/tuple contains the
+                             starting position (duplicate), ending position and replacement text.
+        @return: The output text with the specified replacements.
+        """
+        output_text = []
+        end_index = -1
+        for index, element in enumerate(input_text):
+            if index in replacements:
+                start_index, end_index, replacement_text = replacements[index]
+                output_text.extend(list(replacement_text))
+                continue
+            if index >= end_index:
+                output_text.append(element)
+        return ''.join(output_text)
 
-    def hasNextFrame(self, frame_index: int, frame_id: str = None) -> bool:
-        assert frame_index is not None or frame_id is not None, \
-            'Illegal operation! Expected either frame_index or frame_id!'
-        if frame_index is not None:
-            return frame_index < (self.getFramesCount() - 1)
-        if frame_id is not None:
-            return self.hasNextFrame(frame_index=self.getFrameIndex(frame_id))
+    @logmethod()
+    def _switch_frames(self, index1, index2):
+        frame1 = self.getFrameByIndex(index1)
+        plugin1 = frame1.getPlugin()
+        frame2 = self.getFrameByIndex(index2)
+        plugin2 = frame2.getPlugin()
+        frame2.setPlugin(plugin1)
+        frame1.setPlugin(plugin2)
 
-    def hasPreviousFrame(self, frame_index: int = None, frame_id: str = None) -> bool:
-        assert frame_index is not None or frame_id is not None, \
-            'Illegal operation! Expected either frame_index or frame_id!'
-        if frame_index is not None:
-            return frame_index > 0
-        if frame_id is not None:
-            return self.hasPreviousFrame(frame_index=self.getFrameIndex(frame_id))
+    @logmethod()
+    def _update_frame(self, frame: CodecFrame) -> CodecFrame:
+        plugin = frame.getPlugin()
+        output, status, error = self._run_plugin(frame.getInputText(), plugin)
+        new_frame_index = frame.getFrameIndex() + 1
+        return self.newFrame(output, plugin.title, new_frame_index, status=status, msg=error)
 
     # ------------------------------------------------------------------------------------------------------------------
+    # Event handlers
+    # ------------------------------------------------------------------------------------------------------------------
 
-    def newFrame(self, text, title, frame_index, status, msg=None) -> CodecFrame:
-        if frame_index < self.getFramesCount():
-            return self._refill_frame(text, title, frame_index, status, msg)
-
-        self._context.logger.debug(f'Adding new codec frame {title} at {frame_index} ...')
-        previous_frame = self.getFrameByIndex(frame_index - 1)
-        new_frame = CodecFrame(self, self._context, self._tab_id, self, self._plugins, text)
-        self.layout().addWidget(new_frame)
-
-        new_frame.pluginSelected.connect(self._on_plugin_selected)
-        new_frame.pluginDeselected.connect(self._on_plugin_deselected)
-        new_frame.configButtonClicked.connect(self._on_frame_config_button_clicked)
-        new_frame.refreshButtonClicked.connect(self._on_frame_refresh_button_clicked)
-        new_frame.upButtonClicked.connect(self._on_frame_up_button_clicked)
-        new_frame.downButtonClicked.connect(self._on_frame_down_button_clicked)
-        new_frame.closeButtonClicked.connect(self._on_frame_close_button_clicked)
-
-        if frame_index > 0:
-            # Every new frame (except the first frame) should signal success/error.
-            new_frame.setStatus(status, msg)
-
-        if previous_frame and frame_index > 1:
-            # Auto-collapse frame where plugin was selected (except first frame and when this frame had focus).
-            previous_frame.setCollapsed(not (self._focused_frame and self._focused_frame == previous_frame))
-
-        new_frame.setContentsMargins(0, 0, 0, 0)
-        new_frame.layout().setContentsMargins(0, 0, 0, 0)
-        new_frame.header().refresh()
-        if previous_frame: previous_frame.header().refresh()
-        return new_frame
+    @logmethod()
+    def _on_plugin_selected(self, frame_id: str, plugin: AbstractPlugin):
+        if plugin:
+            frame = self.getFrameById(frame_id)
+            if not self._configure_plugin(frame_id, frame.getInputText(), plugin):
+                # Abort if user cancels configuration.
+                return
+
+            if frame.getFrameIndex() > 0 and not frame.hasNextFrame():
+                # Auto-collapse when current frame is last frame (except if current frame is the first frame).
+                frame.setCollapsed(True)
+
+            # TODO: #53 Allow multiple codecs on input
+            #       Computation should be done within in the frame.
+            #       (Old) frames store information how input is processed.
+            frame = self._new_frame(frame)
+
+            # Focus the input text of the newly created frame.
+            # If frame already existed make sure it is not collapsed.
+            frame.setCollapsed(False)
+            frame.focusInputText()
+        else:
+            self._deselect_plugin(frame_id)
 
+    @logmethod()
     def _on_frame_close_button_clicked(self, frame_id):
         """ Closes/Removes the frame with the specified frame-id. """
         _frame_index = self.getFrameIndex(frame_id)
         self._context.logger.debug(f'Close frame {_frame_index}:{frame_id}')
         assert _frame_index > 0, 'Illegal operation! Can not close first or invalid frame!'
         frame = self.getFrameByIndex(_frame_index)
         previous_frame = self.getFrameByIndex(_frame_index - 1)
 
         if not self.hasNextFrame(_frame_index):
             # If this is the last frame the combo-boxes of the previous frame needs to reset.
-            self.layout().removeWidget(frame) # remove frame from layout to avoid side-effects with header refresh
+            self.layout().removeWidget(frame)  # remove frame from layout to avoid side-effects with header refresh
             frame.deleteLater()
             previous_frame.getComboBoxes().resetAll()
             # Usability: Always show the content of the last frame.
             previous_frame.setCollapsed(False)
             # Update headings since some buttons may need to be en-/disabled.
             previous_frame.header().refresh()
         else:
             # Otherwise the selected plugin of the previous frame needs to be executed.
             next_frame = self.getFrameByIndex(_frame_index + 1)
-            self.layout().removeWidget(frame) # remove frame from layout to avoid side-effects with header refresh
+            self.layout().removeWidget(frame)  # remove frame from layout to avoid side-effects with header refresh
             frame.deleteLater()
-            self._execute_plugin_run(previous_frame.id(), previous_frame.getInputText(), previous_frame.getPlugin())
+            self._update_frame(previous_frame)
+
             # Update headings since some buttons may need to be en-/disabled.
             next_frame.header().refresh()
             previous_frame.header().refresh()
 
+    @logmethod()
     def _on_frame_refresh_button_clicked(self, frame_id: str):
         _frame_index = self.getFrameIndex(frame_id)
         self._context.logger.debug(f'Refreshing frame {_frame_index}:{frame_id}')
         assert self.hasPreviousFrame(_frame_index), 'Illegal operation! No previous frame!'
         previous_frame = self.getFrameByIndex(_frame_index - 1)
         self._context.listener().textChanged.emit(
-            self._tab_id, previous_frame.getFrameId(), previous_frame.getInputText(), False)
+            self._tab_id, previous_frame.getFrameId(), previous_frame.getInputText())
 
+    @logmethod()
     def _on_frame_up_button_clicked(self, frame_id: str):
         # Example:
         #
         #   1. "Hello, world" - Base64 - open
         #   2. "<base64> of hello world" - Sha256 - collapsed
         #   3. "<sha256> of base64 hello world" - <> - open
         #
@@ -301,19 +265,20 @@
         #       3. "<base64> of <sha256> of hello world" - open
         #
         #       Note that the text of the first frame is not touched. More precisely any frame which is in default
         #       state should not be touched. However, frames which contain an error can be overwritten.
         #
         frame_index = self.getFrameIndex(frame_id)
         codec_frame = self.getFrameByIndex(frame_index)
-        assert not codec_frame or frame_index < 2, f'Illegal operation! moveFrameUp({frame_index}:{frame_id})'
+        assert codec_frame and frame_index > 1, f'Illegal operation! moveFrameUp({frame_index}:{frame_id})'
         self._switch_frames(frame_index - 2, frame_index - 1)
         codec_frame = self.getFrameByIndex(frame_index - 2)
-        self._text_changed_event(codec_frame.id(), codec_frame.getInputText(), is_user_action=False, do_preserve_state=True)
+        self._update_frames(codec_frame.id(), is_user_action=False, do_preserve_state=True)
 
+    @logmethod()
     def _on_frame_down_button_clicked(self, frame_id: str):
         # Example:
         #
         #   1. "Hello, world" - Base64 - open
         #   2. "<base64> of hello world" - Sha256 - collapsed
         #   3. "<sha256> of base64 hello world" - <> - open
         #
@@ -334,34 +299,143 @@
         #
         #   Case 3. Press down on Frame 3
         #
         #       Last frame can not be moved.
         #
         frame_index = self.getFrameIndex(frame_id)
         codec_frame = self.getFrameByIndex(frame_index)
-        assert not codec_frame or frame_index == 0 or frame_index == self.getFramesCount() - 1, \
-            f'Illegal operation! moveFrameDown({frame_index}:{frame_id})'
+        assert codec_frame and frame_index > 0 or frame_index < self.getFramesCount() - 1, \
+            f'Illegal operation! moveFrameDown({frame_index}:{frame_id}) with {self.getFramesCount()} frames'
         self._switch_frames(frame_index - 1, frame_index)
         codec_frame = self.getFrameByIndex(frame_index - 1)
-        self._text_changed_event(codec_frame.id(), codec_frame.getInputText(), is_user_action=False, do_preserve_state=True)
-
-    def _switch_frames(self, index1, index2):
-        frame1 = self.getFrameByIndex(index1)
-        plugin1 = frame1.getPlugin()
-        frame2 = self.getFrameByIndex(index2)
-        plugin2 = frame2.getPlugin()
-        frame2.setPlugin(plugin1)
-        frame1.setPlugin(plugin2)
+        self._update_frames(codec_frame.id(), is_user_action=False, do_preserve_state=True)
 
+    @logmethod()
     def _on_frame_config_button_clicked(self, frame_id: str):
         # Remember: We press the config-button of a frame, but want to show the plugin-config of the previous frame ...
         frame_index = self.getFrameIndex(frame_id)
         previous_frame = self.getFrameByIndex(frame_index - 1)
         if previous_frame:
-            plugin = previous_frame.getPlugin()
-            input_text = previous_frame.getInputText()
-            self._show_plugin_config(previous_frame.id(), input_text, plugin)
+            if not self._configure_plugin(frame_id, previous_frame.getInputText(), previous_frame.getPlugin()):
+                # Abort if the user cancels the configuration
+                return
+            self._new_frame(previous_frame)
 
     # ------------------------------------------------------------------------------------------------------------------
+    # Public functions
+    # ------------------------------------------------------------------------------------------------------------------
+
+    def getFrameIndex(self, frame_id) -> int:
+        frame = None
+        index = 0
+        for current_frame in self.getFrames():
+            if current_frame.getFrameId() == frame_id:
+                frame = current_frame
+                break
+            index = index + 1
+        return index if frame else -1
+
+    def getFrameById(self, frame_id) -> CodecFrame:
+        for frame in self.getFrames():
+            if frame.id() == frame_id:
+                return frame
+
+    def getFrameByIndex(self, index) -> CodecFrame:
+        if self.layout().itemAt(index):
+            return self.layout().itemAt(index).widget()
+
+    def getFramesCount(self) -> int:
+        return self.layout().count()
+
+    def getFocusedFrame(self) -> CodecFrame:
+        widget = self.focusWidget()
+        while widget:
+            if isinstance(widget, CodecFrame):
+                return widget
+            widget = widget.parent()
+        return self.layout().itemAt(0).widget()
+
+    def getFrames(self) -> List[CodecFrame]:
+        frames = []
+        for frameIndex in range(0, self.layout().count()):
+            frames.append(self.layout().itemAt(frameIndex).widget())
+        return frames
+
+    def hasNextFrame(self, frame_index: int, frame_id: str = None) -> bool:
+        assert frame_index is not None or frame_id is not None, \
+            'Illegal operation! Expected either frame_index or frame_id!'
+        if frame_index is not None:
+            return frame_index < (self.getFramesCount() - 1)
+        if frame_id is not None:
+            return self.hasNextFrame(frame_index=self.getFrameIndex(frame_id))
+
+    def hasPreviousFrame(self, frame_index: int = None, frame_id: str = None) -> bool:
+        assert frame_index is not None or frame_id is not None, \
+            'Illegal operation! Expected either frame_index or frame_id!'
+        if frame_index is not None:
+            return frame_index > 0
+        if frame_id is not None:
+            return self.hasPreviousFrame(frame_index=self.getFrameIndex(frame_id))
+
+    @logmethod()
+    def newFrame(self, input_text: str, title: str, frame_index: int, status, msg=None) -> CodecFrame:
+        if frame_index < self.getFramesCount():
+            # if frame already exists, refill frame.
+            return self._refill_frame(input_text, title, frame_index, status, msg)
+
+        self._context.logger.debug(f'Adding new codec frame {title} at {frame_index} ...')
+        previous_frame = self.getFrameByIndex(frame_index - 1)
+        new_frame = CodecFrame(self, self._context, self._tab_id, self, self._plugins, input_text)
+        self.layout().addWidget(new_frame)
+
+        new_frame.pluginSelected.connect(self._on_plugin_selected)
+        new_frame.configButtonClicked.connect(self._on_frame_config_button_clicked)
+        new_frame.refreshButtonClicked.connect(self._on_frame_refresh_button_clicked)
+        new_frame.upButtonClicked.connect(self._on_frame_up_button_clicked)
+        new_frame.downButtonClicked.connect(self._on_frame_down_button_clicked)
+        new_frame.closeButtonClicked.connect(self._on_frame_close_button_clicked)
+
+        def on_text_selection_changed(tab_id, frame_id, input_text):
+            if self._tab_id == tab_id:
+                self._context.listener().textSelectionChanged.emit(tab_id, frame_id, input_text)
+
+        new_frame.textSelectionChanged.connect(on_text_selection_changed)
+
+        def selected_frame_changed(tab_id, frame_id, input_text):
+            # Always remember the currently focused frame (e.g. used for finding the currently selected frame when
+            # using keyboard-shortcuts)
+            self._focused_frame = self.getFrameById(frame_id)
+            self._context.listener().selectedFrameChanged.emit(tab_id, frame_id, input_text)
+
+        new_frame.selectedFrameChanged.connect(selected_frame_changed)
+
+        def textChanged(tab_id, frame_id, text):
+            if self._tab_id == tab_id:
+                self._update_frames(frame_id)
+                self._context.listener().textChanged.emit(tab_id, frame_id, text)
+
+        new_frame.textChanged.connect(textChanged)
+        if frame_index > 0:
+            # Every new frame (except the first frame) should signal success/error.
+            new_frame.setStatus(status, msg)
+
+        def on_text_submitted(tab_id: str, frame_id: str, text: str):
+            if tab_id == self._tab_id and frame_id == new_frame.id():
+                new_frame.setInputText(text)
+
+        self._context.listener().textSubmitted.connect(on_text_submitted)
+
+        new_frame.setContentsMargins(0, 0, 0, 0)
+        new_frame.layout().setContentsMargins(0, 0, 0, 0)
+        new_frame.header().refresh()
+        if previous_frame: previous_frame.header().refresh()
+        return new_frame
+
+    def frame(self, index: int) -> CodecFrame:
+        return self.layout().itemAt(index).widget()
+
+    def count(self) -> int:
+        return self.layout().count()
 
+    @logmethod()
     def toDict(self) -> List[dict]:
         return [frame.toDict() for frame in self.getFrames()]
```

### Comparing `decoder-plus-plus-1.5.0/dpp/ui/view/classic/codec_tab.py` & `decoder-plus-plus-1.7.0/dpp/ui/view/classic/codec_tab.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,22 +17,24 @@
 import uuid
 from typing import List
 
 from qtpy.QtCore import Qt
 from qtpy.QtWidgets import QScrollArea, QFrame, QVBoxLayout
 
 from dpp.core import Context
+from dpp.core.logger import logmethod
 from dpp.core.plugin.manager import PluginManager
 from dpp.ui.view.classic.codec_frames import CodecFrames
 from dpp.ui.widget.spacers import VSpacer
 from dpp.ui.widget.status_widget import StatusWidget
 
 
 class CodecTab(QScrollArea):
 
+    @logmethod()
     def __init__(self, parent, context: Context, plugins: PluginManager):
         super(__class__, self).__init__(parent)
         self._context = context
         self._tab_id = uuid.uuid4().hex
         self._plugins = plugins
         self._frames = CodecFrames(self, context, self._tab_id, plugins)
         self._main_frame = QFrame(self)
```

### Comparing `decoder-plus-plus-1.5.0/dpp/ui/view/classic/combo_box_frame.py` & `decoder-plus-plus-1.7.0/dpp/ui/view/classic/combo_box_frame.py`

 * *Files 17% similar despite different names*

```diff
@@ -17,23 +17,24 @@
 import copy
 
 from qtpy.QtCore import QTimer, Signal
 from qtpy.QtGui import QStandardItemModel, QStandardItem
 from qtpy.QtWidgets import QFrame, QComboBox, QVBoxLayout
 
 import dpp
+from dpp.core.logger import logmethod
 from dpp.core.plugin import NullPlugin
 from dpp.core.plugin import PluginType
 from dpp.ui.widget.combo_box import ComboBox
 
 
 class ComboBoxFrame(QFrame):
-    pluginDeselected = Signal(str)  # combo_box_type
-    pluginSelected = Signal(str, int, 'PyQt_PyObject')  # combo_box_type, combo_box_index, plugin
+    pluginSelected = Signal('PyQt_PyObject')  # plugin
 
+    @logmethod()
     def __init__(self, parent, context):
         super(ComboBoxFrame, self).__init__(parent)
         self._context = context
         self._plugins = context.plugins()
 
         # Cache for remembering configurations of selected plugins.
         self._plugin_cache = {}
@@ -49,14 +50,15 @@
         for codec_combo_box in self._combo_boxes.values():
             layout.addWidget(codec_combo_box)
 
         layout.setContentsMargins(0, 0, 0, 0)
         self.setLayout(layout)
         self._combo_box_selection_history = []
 
+    @logmethod()
     def _init_combo_box(self, combo_box_title: str, combo_box_type: str):
         combo_box = ComboBox()
         combo_box.setEditable(True)
         combo_box.setInsertPolicy(QComboBox.NoInsert)
         model = QStandardItemModel()
 
         model.setItem(0, 0, QStandardItem(combo_box_title))
@@ -72,49 +74,54 @@
         # FIX: Delay select-all for a few milliseconds.
         combo_box.focusInEvent = lambda e: QTimer.singleShot(100, lambda: combo_box.lineEdit().selectAll())
         # BUG: combo_box.lineEdit().deselect does not work correctly when loosing focus.
         # FIX: Delay deselect for a few milliseconds.
         combo_box.focusOutEvent = lambda e: QTimer.singleShot(100, lambda: combo_box.lineEdit().deselect())
         combo_box.setModel(model)
         combo_box.setModelColumn(0)
-        combo_box.activated.connect(
-            lambda i: self._combo_box_item_selected_event(combo_box_type, combo_box.currentIndex()))
+        combo_box.currentIndexChanged.connect(
+            lambda i: self._combo_box_item_selected_event(combo_box_type, combo_box.currentIndex())
+        )
         return combo_box
 
+    @logmethod()
     def _combo_box_enter_pressed_event(self, combo_box_type: str):
         combo_box = self._combo_boxes[combo_box_type]
         current_text = combo_box.currentText()
         self._combo_box_selection_history.append([combo_box_type, combo_box.index()])
         self.selectItem(combo_box_type, current_text, block_signals=False)
 
+    @logmethod()
     def _combo_box_item_selected_event(self, combo_box_type: str, combo_box_index: int):
         self.resetExceptType(combo_box_type)
         if combo_box_index == 0:
             # Remove frames below when title element was selected
             # Note: It does not matter which combo box is the source, since all combo boxes are going to reset
             # to index 0.
-            self.pluginDeselected.emit(combo_box_type)
+            self.pluginSelected.emit(None)
             return
 
         self._combo_box_selection_history.append([combo_box_type, combo_box_index])
         plugin = self.getPluginByTypeAndIndex(combo_box_type, combo_box_index)
-        self.pluginSelected.emit(combo_box_type, combo_box_index, plugin)
+        self.pluginSelected.emit(plugin)
 
+    @logmethod()
     def reselectLastItem(self, block_signals=True):
         # Always reset everything first.
         self.resetAll()
         if len(self._combo_box_selection_history) > 1:
             # Reselect previous item if any.
             type, index = self._combo_box_selection_history[-2]
             self.reselectItem(index, type, block_signals)
 
     def index(self, combo_box_type: str) -> int:
-        """ Returns the """
+        """ Returns the index of the currently selected item in the given combo box. """
         return self._combo_boxes[combo_box_type].currentIndex()
 
+    @logmethod()
     def reselectItem(self, index: int, combo_box_type: str, block_signals=True):
         combo_box = self._combo_boxes[combo_box_type]
         combo_box.blockSignals(block_signals)
         combo_box.setCurrentIndex(index)
         combo_box.blockSignals(False)
 
     def getPluginByTypeAndIndex(self, combo_box_type: str, index: int) -> dpp.core.plugin.AbstractPlugin:
@@ -138,50 +145,58 @@
             selected_plugin_type = selected_plugin_types[0]
             selected_combo_box = self._combo_boxes[selected_plugin_type]
             selected_index = selected_combo_box.currentIndex()
             return self.getPluginByTypeAndIndex(selected_plugin_type, selected_index)
         else:
             return NullPlugin(self._context)
 
+    @logmethod()
     def selectItem(self, combo_box_type: str, plugin_name: str, block_signals=False):
         if not combo_box_type and not plugin_name:
+            # Signals are blocked during this call.
             self.resetAll()
             return
 
+        # Signals are blocked during this call.
         self.resetExceptType(combo_box_type)
         combo_box = self._combo_boxes[combo_box_type]
         for i in range(combo_box.count()):
             if combo_box.itemText(i) == plugin_name:
                 combo_box.blockSignals(block_signals)
                 combo_box.setCurrentIndex(i)
                 combo_box.blockSignals(False)
                 break
 
+    @logmethod()
     def focusType(self, combo_box_type: str):
-        """ Focues the combo-box associated with the specified type (e.g. PluginType.DECODER, ...). """
+        """ Focuses the combo-box associated with the specified type (e.g. PluginType.DECODER, ...). """
         self._combo_boxes[combo_box_type].setFocus()
 
+    @logmethod()
     def _reset(self, *combo_boxes, **kwargs):
         """ Resets a list of combo-boxes. """
         for combo_box in combo_boxes:
             combo_box.blockSignals(True)
             combo_box.setCurrentIndex(0)
             combo_box.blockSignals(False)
 
+    @logmethod()
     def resetExceptType(self, combo_box_type: str):
         """ Resets all combo-boxes except the specified type (e.g. PluginType.DECODER, ...). """
         for _combo_box_type in self._combo_boxes.keys():
             if _combo_box_type != combo_box_type:
                 self._reset(self._combo_boxes[_combo_box_type])
 
+    @logmethod()
     def resetAll(self):
         """ Resets all combo-boxes to show the first element. """
         self._context.logger.debug("ComboBoxFrame:ResetAll")
         self._reset(*self._combo_boxes.values())
 
+    @logmethod()
     def setToolTip(self, tooltip: str, combo_box_type: str = None):
         """ Setup's the tooltip of the combo-box associated with the specified plugin-type.
         :param tooltip: the tooltip to show.
         :param combo_box_type: the plugin-type which is associated with the combo-box (e.g. PluginType.DECODER, ...).
         """
         assert combo_box_type is not None, 'No combo box type was specified!'
         assert combo_box_type in self._combo_boxes.keys(), 'Illegal combo box type!'
```

### Comparing `decoder-plus-plus-1.5.0/dpp/ui/view/main_window_widget.py` & `decoder-plus-plus-1.7.0/dpp/ui/view/main_window_widget.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,16 +15,17 @@
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 import os
 from typing import List, Union
 
 from qtpy.QtCore import QEvent
 from qtpy.QtGui import QIcon
-from qtpy.QtWidgets import QMainWindow, QAction, QVBoxLayout, QFileDialog, QMenu, QWidget
+from qtpy.QtWidgets import QMainWindow, QAction, QVBoxLayout, QMenu, QWidget
 
+from dpp.core.logger import logmethod
 from dpp.core.shortcuts import MenuRegistry
 from dpp.ui import IconLabel
 from dpp.ui.dock.hex_dock import HexDock
 from dpp.ui.dock.log_dock import LogDock
 from dpp.ui.widget.dock_tabs_widget import DockTabsWidget
 
 from dpp.core import Context
@@ -34,14 +35,15 @@
 
 menu = MenuRegistry()
 MenuItem = Context.Shortcut
 
 
 class MainWindowWidget(QWidget):
 
+    @logmethod()
     def __init__(self, parent: QMainWindow, context: 'core.context.Context', input_text: str):
         super().__init__(parent)
         self._context = context
         self._plugins = context.plugins()
         self._parent = parent
 
         # Initialize docks
@@ -62,14 +64,15 @@
         self.tabsWidget().onTabDuplicateButtonClick.connect(self.duplicateTab)
         self.newTab(input_text=input_text)
 
     #############################################
     # Menu
     #############################################
 
+    @logmethod()
     def _init_menu_items(self):
         self._register_shortcuts('&File', [
             [Context.Shortcut.TAB_NEW, Context.Shortcut.TAB_CLOSE],
             [Context.Shortcut.OPEN_FILE, Context.Shortcut.SAVE_AS_FILE],
             [Context.Shortcut.SHOW_PLUGINS],
             [Context.Shortcut.FILE_EXIT]
         ])
@@ -79,14 +82,15 @@
         self._init_tabs_menu()
         self._register_shortcuts('&Help', [
             [
                 Context.Shortcut.SHOW_KEYBOARD_SHORTCUTS, Context.Shortcut.SHOW_ABOUT
             ]
         ])
 
+    @logmethod()
     def _init_tabs_menu(self):
         tab_menu = self._register_shortcuts('&Tabs', [
             [
                 Context.Shortcut.TAB_NEW, Context.Shortcut.TAB_RENAME, Context.Shortcut.TAB_DUPLICATE,
                 Context.Shortcut.TAB_NEXT, Context.Shortcut.TAB_PREVIOUS
             ]
         ])
@@ -159,14 +163,15 @@
     def _select_modern_gui_action(self):
         pass
 
     #############################################
     # Helpers
     #############################################
 
+    @logmethod()
     def _register_shortcuts(self, menu_item: Union[str, QMenu], items: List[List]):
         def register_shortcut(id, text, shortcut_key, callback, menu_widget):
             """ This method is required in order to get the callback working. """
             self._register_shortcut(id, text, shortcut_key, lambda: callback(self), menu_widget)
 
         if isinstance(menu_item, str):
             if self.menuBar().hasMenu(menu_item):
@@ -185,31 +190,36 @@
                 text, shortcut_key, callback = menu.registry[shortcut_key_id]
                 register_shortcut(shortcut_key_id, text, shortcut_key, callback, menu_widget)
             if index < len(items):
                 # Add a separator inbetween items
                 menu_widget.addSeparator()
         return menu_widget
 
+    @logmethod()
     def _register_shortcut(self, id, text, shortcut_key, callback, menu) -> QAction:
         action = self._context.registerShortcut(id, text, shortcut_key, callback, self)
         menu.addAction(action)
         return action
 
+    @logmethod()
     def _show_hidden_dialog(self, tab_select: str = None):
         """ Shows the hidden dialog. """
         ConfigDialog(self, self._context, tab_select).exec_()
 
+    @logmethod()
     def _tab_added_event(self, index, title, tab, input_text):
         if 0 <= index < len(self._tabs_select_action):
             self._tabs_select_action[index].setVisible(True)
 
+    @logmethod()
     def _tab_closed_event(self, index, title):
         for index in range(0, len(self._tabs_select_action)):
             self._tabs_select_action[index].setVisible(index < self.tabsWidget().tabCount())
 
+    @logmethod()
     def _init_hidden_dialog(self):
         """ Inits the icon which opens the hidden dialog on mouse press. """
         about_label = IconLabel(self, QIcon(os.path.join(self._context.getAppPath(), 'images', 'hidden.png')))
         about_label.mousePressEvent = lambda e: self._show_hidden_dialog()
         return about_label
 
     #############################################
@@ -232,20 +242,22 @@
         return self._parent.statusBar()
 
     def docksWidget(self) -> DockTabsWidget:
         if not hasattr(self, '_docks_widget'):
             self._docks_widget = DockTabsWidget(self._parent, self._context)
         return self._docks_widget
 
+    @logmethod()
     def closeEvent(self, e: QEvent):
         """ Closes the main window and saves window-size and -position. """
         self._context.config.setSize(self.size())
         self._context.config.setPosition(self.pos())
         e.accept()
 
+    @logmethod()
     def newTab(self, title: str = None, input_text: str = None, widget: QWidget = None) -> (int, QWidget):
         """
         Opens a new tab and writes input.
         :param title: The title of the tab.
         :param input_text: The input which should be written into the tab.
         """
         index, tab = self.tabsWidget().newTab(widget, title=title, input_text=input_text)
```

### Comparing `decoder-plus-plus-1.5.0/dpp/ui/view/modern/__init__.py` & `decoder-plus-plus-1.7.0/dpp/ui/view/modern/__init__.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.5.0/dpp/ui/view/modern/modern_main_window_widget.py` & `decoder-plus-plus-1.7.0/dpp/ui/view/modern/modern_main_window_widget.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 from dpp.ui.view.main_window_widget import MainWindowWidget
 from dpp.ui.view.modern.node_editor_tab import NodeEditorTab
 
 
 class ModernMainWindowWidget(MainWindowWidget):
 
     def __init__(self, parent, context: 'dpp.core.context.Context', input_text: str):
-        super().__init__(parent, context)
+        super().__init__(parent, context, input_text)
 
     #############################################
     # Menu items
     #############################################
 
     def _init_menu_items(self):
         self._register_shortcuts('&File', [])
```

### Comparing `decoder-plus-plus-1.5.0/dpp/ui/view/modern/node_data.py` & `decoder-plus-plus-1.7.0/dpp/ui/view/modern/node_data.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.5.0/dpp/ui/view/modern/node_data_models.py` & `decoder-plus-plus-1.7.0/dpp/ui/view/modern/node_data_models.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.5.0/dpp/ui/view/modern/node_editor.py` & `decoder-plus-plus-1.7.0/dpp/ui/view/modern/node_editor.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
     def __init__(self, parent, context, tab_id, plugins, input_text: str):
         super(__class__, self).__init__(parent)
         self._context = context
         self._tab_id = tab_id
         self._plugins = plugins
         self._layout = QVBoxLayout()
-        self._node_data_models_builder = NodeDataModelsBuilder(context, plugins)
+        self._node_data_models_builder = NodeDataModelsBuilder(context)
         node_editor_view = self._init_node_editor_view(input_text)
         self._layout.addWidget(node_editor_view)
         self.setLayout(self._layout)
         self._layout.setContentsMargins(0, 0, 0, 0)
 
     def _init_node_editor_view(self, input: str):
```

### Comparing `decoder-plus-plus-1.5.0/dpp/ui/view/modern/node_editor_tab.py` & `decoder-plus-plus-1.7.0/dpp/ui/view/modern/node_editor_tab.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.5.0/dpp/ui/widget/__init__.py` & `decoder-plus-plus-1.7.0/dpp/ui/widget/__init__.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.5.0/dpp/ui/widget/clickable_label.py` & `decoder-plus-plus-1.7.0/dpp/ui/widget/clickable_label.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.5.0/dpp/ui/widget/codec_preview_widget.py` & `decoder-plus-plus-1.7.0/dpp/ui/widget/codec_preview_widget.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 from qtpy.QtWidgets import QFrame, QPlainTextEdit, QHBoxLayout, QAction
 
 
 class CodecPreviewWidget(QFrame):
 
     def __init__(self, plugin, input_text):
         super().__init__()
-        self._logger = logging.getLogger()
+        self._logger = logging.getLogger(__name__)
         view_frame_layout = QHBoxLayout()
         view_frame_layout.setContentsMargins(0, 5, 0, 5)
         self._txt_preview = QPlainTextEdit(self)
         self._txt_preview.setPlainText(input_text)
         self._txt_preview.setReadOnly(True)
         self._txt_preview.setLineWrapMode(QPlainTextEdit.NoWrap)
         self._txt_preview.customContextMenuRequested.connect(self._show_preview_frame_context_menu)
@@ -43,16 +43,18 @@
         self._plugin.config.onChange.connect(lambda keys: self._do_preview())
 
     def _do_preview(self):
         try:
             self._txt_preview.setStyleSheet('')
             result = self._plugin.run(self._input_text)
             self._txt_preview.setPlainText(result)
+            self._plugin.onSuccess.emit("")
         except BaseException as err:
             self._txt_preview.setStyleSheet('border: 1px solid red;')
+            self._plugin.onError.emit(str(err))
             self._logger.debug(err, exc_info=False)
 
     def _show_preview_frame_context_menu(self, point: QPoint = None):
         """ Displays a customized context menu for the plain view. """
 
         def _on_plain_text_context_menu_wrap_lines(e: QEvent):
             """ Un-/wraps lines when user clicks the wrap-lines action within the plain views context-menu. """
```

### Comparing `decoder-plus-plus-1.5.0/dpp/ui/widget/collapsible_frame.py` & `decoder-plus-plus-1.7.0/dpp/ui/widget/collapsible_frame.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,16 +26,14 @@
 
 
 class CollapsibleFrame(QFrame):
     """
     Frame with ability to un-/collapse content via clickable arrow-handles.
     """
 
-    frameChanged = Signal(str)
-
     arrowClicked = Signal()
     upButtonClicked = Signal()
     downButtonClicked = Signal()
     configButtonClicked = Signal()
     closeButtonClicked = Signal()
 
     def __init__(self, parent, context: Context, frame_id: str):
@@ -92,27 +90,25 @@
         content_layout.setAlignment(Qt.AlignTop)
         content.setLayout(content_layout)
         content.setVisible(not collapsed)
         return content
 
     def _arrow_clicked_event(self):
         self.toggleCollapsed()
-        self._was_collapse_state_changed_by_user = True
+        # Remember, when user uncollapses the frame manually. This is used to determine whether the
+        # frame should be collapsed automatically under certain conditions.
+        self._was_collapse_state_changed_by_user = not self.isCollapsed()
 
     def addWidget(self, widget):
         """
         Adds an widget to the content.
         :param widget: the widget to be added.
         """
         self._content.layout().addWidget(widget)
 
-    def setContentDirection(self, direction: int):
-        """ Sets the direction of the content (e.g. LeftToRight, RightToLeft, TopToBottom, BottomToTop). """
-        self._content.layout().setDirection(direction)
-
     def toggleCollapsed(self):
         """ Toggles collapsing of the frame. """
         self._content.setVisible(self._is_collasped)
         self._is_collasped = not self._is_collasped
         self._header_frame._arrow.setArrow(int(self._is_collasped))
 
     def setCollapsed(self, status):
@@ -127,18 +123,14 @@
     def wasCollapseStateChangedByUser(self):
         """ Returns whether the collapse state was changed by the user. """
         return self._was_collapse_state_changed_by_user
 
     def header(self) -> 'dpp.ui.collapsible_frame.CollapsibleFrame.HeaderFrame':
         return self._header_frame
 
-    def indicateError(self, status: bool):
-        """ Indicates that there was an error during encoding/decoding/hashing/scripting. """
-        self._header_frame.indicateError(status)
-
     def getContentHeight(self) -> int:
         """ Returns the height of the content when uncollapsed. """
         return self._content.height()
 
     def setContentHeight(self, height: int):
         """ Sets the height of the content when uncollapsed. """
         self._content.setFixedHeight(height)
@@ -161,14 +153,17 @@
                     if child.widget():
                         child.widget().deleteLater()
 
             def setCentralWidget(self, widget: QWidget):
                 self.clearLayout()
                 self.layout().addWidget(widget)
 
+            def centralWidget(self) -> QWidget:
+                return self.layout().itemAt(0).widget()
+
             def setStatus(self, status: str, message: str):
                 """ Sets a status.
                 :param status: The status to set. Either "DEFAULT", "SUCCESS", or "ERROR".
                 :param message: The message to set.
                 """
                 ...
```

### Comparing `decoder-plus-plus-1.5.0/dpp/ui/widget/combo_box.py` & `decoder-plus-plus-1.7.0/dpp/ui/widget/combo_box.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.5.0/dpp/ui/widget/dock_tabs_widget.py` & `decoder-plus-plus-1.7.0/dpp/ui/widget/dock_tabs_widget.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.5.0/dpp/ui/widget/dock_widget.py` & `decoder-plus-plus-1.7.0/dpp/ui/widget/dock_widget.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.5.0/dpp/ui/widget/dyna_frame.py` & `decoder-plus-plus-1.7.0/dpp/ui/widget/dyna_frame.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.5.0/dpp/ui/widget/elided_label.py` & `decoder-plus-plus-1.7.0/dpp/ui/widget/elided_label.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.5.0/dpp/ui/widget/hover_label.py` & `decoder-plus-plus-1.7.0/dpp/ui/widget/hover_label.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.5.0/dpp/ui/widget/icon_label.py` & `decoder-plus-plus-1.7.0/dpp/ui/widget/icon_label.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,23 +18,24 @@
 
 from dpp.ui.widget.hover_label import HoverLabel
 
 
 class IconLabel(HoverLabel):
     """ A widget for showing an icon. """
 
-    def __init__(self, parent, icon):
+    def __init__(self, parent, icon: QIcon = None):
         super(IconLabel, self).__init__(parent)
         self._icon = None
         self._do_repaint = None
         self._last_height = None
-        self.setIcon(icon)
+        if icon:
+            self.setIcon(icon)
         self.setHoverEffect(False)
 
-    def setIcon(self, icon):
+    def setIcon(self, icon: QIcon):
         """ Sets the icon. """
         assert isinstance(icon, QIcon), f'Illegal type! Expected QIcon, got {type(icon)}!'
         self._do_repaint = True
         self._icon = icon
         self.repaint()
 
     def paintEvent(self, event=None):
```

### Comparing `decoder-plus-plus-1.5.0/dpp/ui/widget/list_widget.py` & `decoder-plus-plus-1.7.0/dpp/ui/widget/list_widget.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.5.0/dpp/ui/widget/menu_bar.py` & `decoder-plus-plus-1.7.0/dpp/ui/widget/menu_bar.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.5.0/dpp/ui/widget/message_widget.py` & `decoder-plus-plus-1.7.0/dpp/ui/widget/message_widget.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.5.0/dpp/ui/widget/option_widgets.py` & `decoder-plus-plus-1.7.0/dpp/ui/widget/option_widgets.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,15 +15,17 @@
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 from typing import List
 
 from qtpy.QtCore import Signal, QObject
 from qtpy.QtWidgets import QCheckBox, QComboBox, QLineEdit, QRadioButton
 
+from dpp.ui.widget.code_editor_widget import CodeEditorWidget
 from dpp.ui.widget.slider_widget import SliderWidget
+from dpp.ui.widget.text_widget import TextWidget
 
 
 class OptionWidget(QObject):
     """ Wraps a widget (e.g. QLineEdit, QCheckBox) representing a configuration option (e.g. String, Boolean). """
 
     onChange = Signal('PyQt_PyObject')  # option
 
@@ -43,16 +45,17 @@
         self._name = option.name
         self._config = config
         self._widget = widget
         self._set_value_callback = set_value_callback
         self._get_value_callback = get_value_callback
         self.setValue(option.value)
         self._config.onChange.connect(self._on_config_change)
-        on_change_signal.connect(lambda event: self.onChange.emit(self))
         self.show_label = show_label
+        widget.setToolTip(option.description)
+        on_change_signal.connect(lambda event: self.onChange.emit(self))
 
     def getKey(self):
         """ Returns the configuration key/id. """
         return self._key
 
     def getName(self):
         """ Returns the human-readable name of the option. """
@@ -76,37 +79,45 @@
 
     def getOption(self):
         """ Returns the configuration option. """
         return self._option
 
     def _on_config_change(self, keys: List[str]):
         """ Checks whether this widget is affected by the configuration change and updates the value accordingly. """
-        if self.getKey() in keys:
+        if self.getKey() in keys and self.getValue() != self._config.value(self.getKey()):
             self.setValue(self._config.value(self.getKey()))
 
-    def validate(self, plugin, input_text) -> str:
+    def validate(self, input_text) -> str:
         """ Validates the configuration entry in association with the input text. """
-        return self._config.validate(self._option, plugin, input_text)
+        return self._config.validate(self._option, input_text)
 
 
 class StringOptionWidget(OptionWidget):
 
     def __init__(self, config, option):
         widget = QLineEdit(str(option.value))
         super().__init__(widget, option, config, lambda text: widget.setText(str(text)), widget.text,
                          widget.textChanged, show_label=True)
 
-    def validate(self, plugin, input_text) -> str:
+    def validate(self, input_text) -> str:
         """ Validates the configuration entry in association with the input text. """
-        if super().validate(plugin, input_text):
+        if super().validate(input_text):
             self._widget.setStyleSheet('QLineEdit { color: red }')
         else:
             self._widget.setStyleSheet('')
 
 
+class TextOptionWidget(OptionWidget):
+
+    def __init__(self, config, option):
+        widget = TextWidget(option.value, read_only=option.read_only, wrap_lines=option.wrap_lines)
+        super().__init__(widget, option, config, widget.setText, widget.text,
+                         widget.textChanged, show_label=False)
+
+
 class BooleanOptionWidget(OptionWidget):
 
     def __init__(self, config, option):
         widget = QCheckBox(option.name)
         super().__init__(widget, option, config, widget.setChecked, widget.isChecked, widget.clicked, show_label=False)
 
 
@@ -128,7 +139,14 @@
 
 
 class SliderOptionWidget(OptionWidget):
 
     def __init__(self, config, option):
         widget = SliderWidget(option.value, option.range)
         super().__init__(widget, option, config, widget.setValue, widget.value, widget.valueChanged, show_label=True)
+
+
+class CodeEditorOptionWidget(OptionWidget):
+
+    def __init__(self, config, option):
+        widget = CodeEditorWidget(option.value)
+        super().__init__(widget, option, config, widget.setText, widget.text, widget.textChanged, show_label=False)
```

### Comparing `decoder-plus-plus-1.5.0/dpp/ui/widget/plain_view.py` & `decoder-plus-plus-1.7.0/dpp/ui/widget/plain_view.py`

 * *Files 21% similar despite different names*

```diff
@@ -10,29 +10,87 @@
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
+import copy
+
 from qtpy import QtCore
-from qtpy.QtCore import QRegularExpression, QPoint, QEvent
+from qtpy.QtCore import QRegularExpression, QPoint, QEvent, Signal
 from qtpy.QtGui import QColor, QBrush, QTextCharFormat, QTextCursor, QCursor
 from qtpy.QtWidgets import QAction, QFrame, QVBoxLayout, QPlainTextEdit
 
 from dpp.core import Context
 from dpp.core.icons import icon, Icon
 from dpp.ui import SearchField
 
 
 class PlainView(QFrame):
     """
     Represents the plain-view of the Decoder++ application.
     """
 
+    selectedFrameChanged = Signal(str, str, str)  # tab_id, frame_id, input_text
+    textSelectionChanged = Signal(str, str, str)  # tab_id, frame_id, input_text
+    textChanged = Signal(str, str, str)  # tab_id, frame_id, input_text
+
+    # Color index
+    color_codes = [
+        '#800000',
+        '#008000',
+        '#000080',
+        '#808000',
+        '#800080',
+        '#008080',
+        '#C0C0C0',
+        '#808080',
+        '#9999FF',
+        '#993366',
+        '#FFFFCC',
+        '#CCFFFF',
+        '#660066',
+        '#FF8080',
+        '#0066CC',
+        '#CCCCFF',
+        '#000080',
+        '#FF00FF',
+        '#FFFF00',
+        '#00FFFF',
+        '#800080',
+        '#800000',
+        '#008080',
+        '#0000FF',
+        '#00CCFF',
+        '#CCFFFF',
+        '#CCFFCC',
+        '#FFFF99',
+        '#99CCFF',
+        '#FF99CC',
+        '#CC99FF',
+        '#FFCC99',
+        '#3366FF',
+        '#33CCCC',
+        '#99CC00',
+        '#FFCC00',
+        '#FF9900',
+        '#FF6600',
+        '#666699',
+        '#969696',
+        '#003366',
+        '#339966',
+        '#003300',
+        '#333300',
+        '#993300',
+        '#993366',
+        '#333399',
+        '#333333'
+    ]
+
     class EventFilter(QtCore.QObject):
 
         def __init__(self, parent, context: 'core.context.Context', callback):
             QtCore.QObject.__init__(self, parent)
             self._context = context
             self._callback = callback
 
@@ -47,54 +105,52 @@
         """
         super(__class__, self).__init__(parent)
         self._context = context
         self._listener = context.listener()
         self._tab_id = tab_id
         self._frame_id = frame_id
 
+        # TODO: How to persist selections and reload them from file?
+        self._selections = []
+
         self._plain_text = QPlainTextEdit()
         self.setPlainText(text)
         self._plain_text.setLineWrapMode(QPlainTextEdit.NoWrap)
         self._plain_text.dragEnterEvent = self._on_plain_text_drag_enter_event
         self._plain_text.dropEvent = self._on_plain_text_drop_event
         self._plain_text.textChanged.connect(self._on_plain_text_changed_event)
         self._plain_text.selectionChanged.connect(self._on_plain_text_selection_changed_event)
         self._plain_text.setContextMenuPolicy(QtCore.Qt.CustomContextMenu)
         self._plain_text.customContextMenuRequested.connect(self.showContextMenu)
         self._plain_text.installEventFilter(
             PlainView.EventFilter(self, self._context, self._on_plain_text_focus_changed_event))
 
-        self._listener.textSubmitted.connect(self._on_plain_text_submitted_event)
-
         self._last_plain_text = self.toPlainText()
         self._last_selected_plain_text = self.toPlainText()
 
         self._search_field = SearchField(self)
         self._search_field.setClosable(True)
         self._search_field.setIcon(icon(Icon.SEARCH))
         self._search_field.setPlaceholderText("Search text")
         self._search_field.escapePressed.connect(self._on_search_field_escape_pressed_event)
         self._search_field.textChanged.connect(self._do_highlight_text)
         self._search_field.closeEvent.connect(self._do_close_search_field)
         self._search_field.setVisible(False)
 
-        # Propagate that a new frame was loaded
-        self._context.listener().selectedFrameChanged.emit(self._tab_id, self._frame_id, self.toPlainText())
-
         layout = QVBoxLayout()
         layout.addWidget(self._plain_text)
         layout.addWidget(self._search_field)
         layout.setContentsMargins(0, 0, 0, 0)
 
         self.setLayout(layout)
 
     def id(self) -> str:
         return self._frame_id
 
-    def showContextMenu(self, point: QPoint=None):
+    def showContextMenu(self, point: QPoint = None):
         """ Displays a customized context menu for the plain view. """
         if not point:
             point = QCursor.pos()
         context_menu = self._plain_text.createStandardContextMenu()
 
         textSelected = len(self._plain_text.textCursor().selectedText()) > 0
 
@@ -148,44 +204,43 @@
         """ Catches the drop-event which is triggered when media is dropped into the plain text area. """
         data = e.mimeData()
         if data.hasUrls():
             file_path = data.urls()[0].toLocalFile()
             try:
                 with open(file_path, mode='rb') as f:
                     # Drops text within (binary) file into plain text area.
-                    self._plain_text.setPlainText(f.read().decode('utf-8', errors='surrogateescape'))
+                    self.setPlainText(f.read().decode('utf-8', errors='surrogateescape'))
             except Exception as e:
                 self._context.logger.error("Error reading file: " + str(e))
         elif data.hasText():
             # Drops text into text field.
-            self._plain_text.setPlainText(data.text())
+            self.setPlainText(data.text())
 
     def _on_plain_text_changed_event(self):
         """ Signals that text has changed and highlights text when search field is active. """
         if self._last_plain_text != self.toPlainText():
             self._last_plain_text = self.toPlainText()
             if self._search_field.isVisible():
                 self._do_highlight_text()
-        self._context.listener().textChanged.emit(self._tab_id, self._frame_id, self.toPlainText(), True)
+            self.textChanged.emit(self._tab_id, self._frame_id, self.toPlainText())
 
     def _on_plain_text_selection_changed_event(self):
         cursor = self._plain_text.textCursor()
         selected_text = cursor.selectedText()
-        if selected_text and selected_text != self._last_selected_plain_text:
+        if selected_text != self._last_selected_plain_text:
+            if not selected_text:
+                # If no text is selected, everything is selected.
+                selected_text = self.toPlainText()
             self._last_selected_plain_text = selected_text
-            self._context.listener().textSelectionChanged.emit(self._tab_id, self._frame_id, selected_text)
+            self.textSelectionChanged.emit(self._tab_id, self._frame_id, selected_text)
 
     def _on_plain_text_focus_changed_event(self, obj, event):
         if event.type() == QtCore.QEvent.FocusIn and event.reason() == QtCore.Qt.MouseFocusReason:
             if self._plain_text.hasFocus():
-                self._context.listener().selectedFrameChanged.emit(self._tab_id, self._frame_id, self.toPlainText())
-
-    def _on_plain_text_submitted_event(self, tab_id: str, frame_id: str, text: str):
-        if tab_id == self._tab_id and frame_id == self._frame_id:
-            self._plain_text.setPlainText(text)
+                self.selectedFrameChanged.emit(self._tab_id, self._frame_id, self.toPlainText())
 
     def _on_search_field_escape_pressed_event(self):
         """ Closes the search field when search field is focused. """
         if self._search_field.hasFocus() and self._search_field.isVisible():
             self._do_close_search_field()
 
     def _do_highlight_clear(self):
@@ -241,27 +296,83 @@
 
     def copySelectedInputText(self):
         self._plain_text.copy()
 
     def pasteSelectedInputText(self):
         self._plain_text.paste()
 
+    # ------------------------------------------------------------------------------------------------------------------
+
+    def _do_clear_selections_highlighting(self):
+        self._selections = []
+        self._plain_text.blockSignals(True)
+        format = QTextCharFormat()
+        format.setBackground(QBrush(QColor("white")))
+        cursor = self._plain_text.textCursor()
+        cursor.setPosition(0)
+        cursor.movePosition(QTextCursor.End, QTextCursor.KeepAnchor, 1)
+        cursor.mergeCharFormat(format)
+        self._plain_text.blockSignals(False)
+
+    def _apply_selections_highlighting(self, selections):
+        cursor = self._plain_text.textCursor()
+        self._do_clear_selections_highlighting()
+        self._plain_text.blockSignals(True)
+        for start, end, color in selections:
+            format = QTextCharFormat()
+            format.setBackground(QBrush(QColor(color)))
+            cursor.setPosition(start)
+            cursor.movePosition(QTextCursor.NextCharacter, QTextCursor.KeepAnchor, end - start)
+            cursor.mergeCharFormat(format)
+        self._plain_text.blockSignals(False)
+        self._selections = selections
+
+    def storeSelection(self):
+        cursor = self._plain_text.textCursor()
+        cur_sel_start = cursor.selectionStart()
+        cur_sel_end = cursor.selectionEnd()
+        tmp_selections = []
+        for stor_sel_start, stor_sel_end, stor_sel_color in self._selections:
+            cur_sel_before_stor_sel = cur_sel_start < stor_sel_start and cur_sel_end < stor_sel_end
+            cur_sel_after_stor_sel = cur_sel_start > stor_sel_end
+            does_selection_overlap = cur_sel_before_stor_sel or cur_sel_after_stor_sel
+            if does_selection_overlap:
+                # Restore stored selections which are not overlapping.
+                tmp_selections.append((stor_sel_start, stor_sel_end, stor_sel_color))
+
+        available_colors = copy.copy(self.color_codes)
+        for stor_sel_start, stor_sel_end, stor_sel_color in tmp_selections:
+            available_colors.remove(stor_sel_color)
+
+        tmp_selections.append((cur_sel_start, cur_sel_end, self.color_codes[0]))
+        self._apply_selections_highlighting(tmp_selections)
+
+    def hastTextSelected(self) -> bool:
+        """ Returns whether there are current and stored text selections. """
+        cursor = self._plain_text.textCursor()
+        selected_text = cursor.selectedText()
+        return selected_text or self._selections
+
+    # ------------------------------------------------------------------------------------------------------------------
+
     def toggleSearchField(self):
         """ Toggles the search field. """
         if self._search_field.hasFocus() and self._search_field.isVisible():
             self._do_close_search_field()
         else:
             self._do_open_search_field()
 
     def toPlainText(self):
         """ Returns the plain text of the plain text area. """
         return self._plain_text.toPlainText()
 
     def setPlainText(self, text):
         """ Sets the text of the text area. """
+        # TODO: Try to restore selections instead of cleaning them.
+        self._selections = []
         # Avoid triggering textChanged-event when setting text manually
         self._plain_text.blockSignals(True)
         self._plain_text.setPlainText(text)
         # Bug: When setting text the cursor position is set to beginning of plain text field.
         # Fix: Manually set cursor position to end of plain text field when setting text.
         self.setCursorPosition(QTextCursor.End)
         self._plain_text.blockSignals(False)
@@ -271,7 +382,8 @@
         plain_text_cursor = self._plain_text.textCursor()
         plain_text_cursor.movePosition(cursor_position)
         self._plain_text.setTextCursor(plain_text_cursor)
 
     def setFocus(self, Qt_FocusReason=None):
         """ Sets the focus to the plain text area. """
         self._plain_text.setFocus()
+        self.selectedFrameChanged.emit(self._tab_id, self._frame_id, self._plain_text.toPlainText())
```

### Comparing `decoder-plus-plus-1.5.0/dpp/ui/widget/plugin_frame.py` & `decoder-plus-plus-1.7.0/dpp/ui/widget/plugin_frame.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.5.0/dpp/ui/widget/plugin_tab.py` & `decoder-plus-plus-1.7.0/dpp/ui/widget/plugin_tab.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.5.0/dpp/ui/widget/search_field.py` & `decoder-plus-plus-1.7.0/dpp/ui/widget/search_field.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.5.0/dpp/ui/widget/separater_widget.py` & `decoder-plus-plus-1.7.0/dpp/ui/widget/separater_widget.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.5.0/dpp/ui/widget/shortcut_table.py` & `decoder-plus-plus-1.7.0/dpp/ui/widget/shortcut_table.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.5.0/dpp/ui/widget/slider_widget.py` & `decoder-plus-plus-1.7.0/dpp/ui/widget/slider_widget.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.5.0/dpp/ui/widget/smart_decode_button.py` & `decoder-plus-plus-1.7.0/dpp/ui/widget/smart_decode_button.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 
 class SmartDecodeButton(QFrame):
     """ A button which provides a smart-decode functionality. """
 
     def __init__(self, parent, plugins: List[DecoderPlugin], get_input_callback, select_decoder_callback):
         super(__class__, self).__init__(parent)
-        self._logger = logging.getLogger()
+        self._logger = logging.getLogger(__name__)
         self._plugins = plugins
         self._get_input = get_input_callback
         self._select_decoder = select_decoder_callback
         layout = QHBoxLayout()
         layout.setContentsMargins(0, 6, 0, 0)
         self._button = self._init_button()
         layout.addWidget(self._button)
```

### Comparing `decoder-plus-plus-1.5.0/dpp/ui/widget/spacers.py` & `decoder-plus-plus-1.7.0/dpp/ui/widget/spacers.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.5.0/dpp/ui/widget/status_widget.py` & `decoder-plus-plus-1.7.0/dpp/ui/widget/status_widget.py`

 * *Files 23% similar despite different names*

```diff
@@ -16,16 +16,21 @@
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 from qtpy.QtWidgets import QWidget, QHBoxLayout
 
 
 class StatusWidget(QWidget):
 
+    # Indicates that the input text was manually edited by the user.
     DEFAULT = "DEFAULT"
+
+    # Indicates that the plugin has been successfully executed.
     SUCCESS = "SUCCESS"
+
+    # Indicates that the plugin has been executed but an error occurred.
     ERROR = "ERROR"
 
     def __init__(self, parent=None, status="DEFAULT", width=15, height=None):
         super(__class__, self).__init__(parent)
         layout = QHBoxLayout()
         self._widget = QWidget(self)
         if width is not None: self._widget.setFixedWidth(width)
```

### Comparing `decoder-plus-plus-1.5.0/dpp/ui/widget/tab_bar.py` & `decoder-plus-plus-1.7.0/dpp/ui/widget/tab_bar.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.5.0/dpp/ui/widget/tabs_widget.py` & `decoder-plus-plus-1.7.0/dpp/ui/widget/tabs_widget.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.5.0/setup.py` & `decoder-plus-plus-1.7.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,17 +60,21 @@
             'css-html-js-minify>=2.5.0',
             'pycryptodome>=3.15.0',
             'jc>=1.21.0',
             'jsbeautifier>=1.14.0',
             'json2xml>=3.19.0',
             'jsonpath_ng>=1.5.0',
             'jwt>=1.3.0',
+            'magika>=0.5.0',
             'passlib>=1.7.0',
             'pycryptodome>=3.15.0',
             'validators>=0.20.0'
+        ],
+        'test': [
+            'pytest-qt>=4.2.0',
         ]
     },
     data_files=[
         ('share/icons/hicolor/scalable/apps', ['data/dpp.png']),
         ('share/applications', ['data/dpp.desktop'])
     ],
     include_package_data=True,
```

