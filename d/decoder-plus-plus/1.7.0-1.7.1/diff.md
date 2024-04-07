# Comparing `tmp/decoder-plus-plus-1.7.0.tar.gz` & `tmp/decoder-plus-plus-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "decoder-plus-plus-1.7.0.tar", last modified: Sun Apr  7 11:36:23 2024, max compression
+gzip compressed data, was "decoder-plus-plus-1.7.1.tar", last modified: Sun Apr  7 18:16:03 2024, max compression
```

## Comparing `decoder-plus-plus-1.7.0.tar` & `decoder-plus-plus-1.7.1.tar`

### file list

```diff
@@ -1,310 +1,311 @@
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-07 11:36:23.990036 decoder-plus-plus-1.7.0/
--rw-rw-r--   0 tom       (1000) tom       (1000)    35147 2021-12-26 21:21:06.000000 decoder-plus-plus-1.7.0/LICENSE
--rw-rw-r--   0 tom       (1000) tom       (1000)       43 2021-12-26 21:21:06.000000 decoder-plus-plus-1.7.0/MANIFEST.in
--rw-rw-r--   0 tom       (1000) tom       (1000)     7935 2024-04-07 11:36:23.990036 decoder-plus-plus-1.7.0/PKG-INFO
--rw-rw-r--   0 tom       (1000) tom       (1000)     7367 2024-04-07 09:27:21.000000 decoder-plus-plus-1.7.0/README.md
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-07 11:36:23.938036 decoder-plus-plus-1.7.0/data/
--rwxrwxr-x   0 tom       (1000) tom       (1000)      116 2021-12-26 21:21:06.000000 decoder-plus-plus-1.7.0/data/dpp.desktop
--rw-rw-r--   0 tom       (1000) tom       (1000)    19277 2024-04-06 19:21:46.000000 decoder-plus-plus-1.7.0/data/dpp.png
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-07 11:36:23.938036 decoder-plus-plus-1.7.0/decoder_plus_plus.egg-info/
--rw-rw-r--   0 tom       (1000) tom       (1000)     7935 2024-04-07 11:36:23.000000 decoder-plus-plus-1.7.0/decoder_plus_plus.egg-info/PKG-INFO
--rw-rw-r--   0 tom       (1000) tom       (1000)     9070 2024-04-07 11:36:23.000000 decoder-plus-plus-1.7.0/decoder_plus_plus.egg-info/SOURCES.txt
--rw-rw-r--   0 tom       (1000) tom       (1000)        1 2024-04-07 11:36:23.000000 decoder-plus-plus-1.7.0/decoder_plus_plus.egg-info/dependency_links.txt
--rw-rw-r--   0 tom       (1000) tom       (1000)       40 2024-04-07 11:36:23.000000 decoder-plus-plus-1.7.0/decoder_plus_plus.egg-info/entry_points.txt
--rw-rw-r--   0 tom       (1000) tom       (1000)      389 2024-04-07 11:36:23.000000 decoder-plus-plus-1.7.0/decoder_plus_plus.egg-info/requires.txt
--rw-rw-r--   0 tom       (1000) tom       (1000)       10 2024-04-07 11:36:23.000000 decoder-plus-plus-1.7.0/decoder_plus_plus.egg-info/top_level.txt
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-07 11:36:23.942036 decoder-plus-plus-1.7.0/dpp/
--rw-rw-r--   0 tom       (1000) tom       (1000)      850 2024-04-07 11:23:42.000000 decoder-plus-plus-1.7.0/dpp/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      239 2021-12-26 21:21:06.000000 decoder-plus-plus-1.7.0/dpp/__main__.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-07 11:36:23.942036 decoder-plus-plus-1.7.0/dpp/core/
--rw-rw-r--   0 tom       (1000) tom       (1000)      915 2021-12-26 21:21:06.000000 decoder-plus-plus-1.7.0/dpp/core/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     2353 2022-09-12 19:05:02.000000 decoder-plus-plus-1.7.0/dpp/core/argparse.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     2871 2022-09-12 21:57:24.000000 decoder-plus-plus-1.7.0/dpp/core/assertions.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     3279 2022-08-17 05:09:19.000000 decoder-plus-plus-1.7.0/dpp/core/config.py
--rw-rw-r--   0 tom       (1000) tom       (1000)    10068 2024-04-05 20:12:39.000000 decoder-plus-plus-1.7.0/dpp/core/context.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     2328 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.0/dpp/core/decoder_plus_plus.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      906 2022-09-18 10:36:35.000000 decoder-plus-plus-1.7.0/dpp/core/exceptions.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     2860 2024-04-07 11:17:10.000000 decoder-plus-plus-1.7.0/dpp/core/icons.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     3650 2023-02-28 12:27:33.000000 decoder-plus-plus-1.7.0/dpp/core/listener.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     4546 2023-01-29 15:42:26.000000 decoder-plus-plus-1.7.0/dpp/core/logger.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1329 2022-09-14 00:12:52.000000 decoder-plus-plus-1.7.0/dpp/core/math.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-07 11:36:23.942036 decoder-plus-plus-1.7.0/dpp/core/plugin/
--rw-rw-r--   0 tom       (1000) tom       (1000)    14067 2024-04-06 16:14:35.000000 decoder-plus-plus-1.7.0/dpp/core/plugin/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     2324 2024-04-06 15:25:06.000000 decoder-plus-plus-1.7.0/dpp/core/plugin/builder.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-07 11:36:23.942036 decoder-plus-plus-1.7.0/dpp/core/plugin/config/
--rw-rw-r--   0 tom       (1000) tom       (1000)     8387 2024-04-06 08:18:07.000000 decoder-plus-plus-1.7.0/dpp/core/plugin/config/__init__.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-07 11:36:23.942036 decoder-plus-plus-1.7.0/dpp/core/plugin/config/options/
--rw-rw-r--   0 tom       (1000) tom       (1000)     3478 2024-04-06 16:14:35.000000 decoder-plus-plus-1.7.0/dpp/core/plugin/config/options/__init__.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-07 11:36:23.942036 decoder-plus-plus-1.7.0/dpp/core/plugin/config/ui/
--rw-rw-r--   0 tom       (1000) tom       (1000)     1572 2022-09-12 21:57:24.000000 decoder-plus-plus-1.7.0/dpp/core/plugin/config/ui/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      858 2022-09-06 21:38:42.000000 decoder-plus-plus-1.7.0/dpp/core/plugin/config/ui/layouts.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     2111 2024-04-06 15:51:05.000000 decoder-plus-plus-1.7.0/dpp/core/plugin/config/ui/widgets.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     3048 2022-09-13 07:31:54.000000 decoder-plus-plus-1.7.0/dpp/core/plugin/loader.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     4301 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.0/dpp/core/plugin/manager.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     3878 2022-08-21 00:18:15.000000 decoder-plus-plus-1.7.0/dpp/core/shortcuts.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-07 11:36:23.950036 decoder-plus-plus-1.7.0/dpp/images/
--rw-rw-r--   0 tom       (1000) tom       (1000)    22919 2021-12-26 21:21:06.000000 decoder-plus-plus-1.7.0/dpp/images/dpp.png
--rw-rw-r--   0 tom       (1000) tom       (1000)    10621 2021-12-26 21:21:06.000000 decoder-plus-plus-1.7.0/dpp/images/dpp_128.png
--rw-rw-r--   0 tom       (1000) tom       (1000)    22919 2021-12-26 21:21:06.000000 decoder-plus-plus-1.7.0/dpp/images/dpp_classic.png
--rw-rw-r--   0 tom       (1000) tom       (1000)    10621 2021-12-26 21:21:06.000000 decoder-plus-plus-1.7.0/dpp/images/dpp_classic_128.png
--rw-rw-r--   0 tom       (1000) tom       (1000)    90434 2022-09-06 22:45:08.000000 decoder-plus-plus-1.7.0/dpp/images/dpp_modern.png
--rw-rw-r--   0 tom       (1000) tom       (1000)    30058 2022-09-06 22:47:19.000000 decoder-plus-plus-1.7.0/dpp/images/dpp_modern_128.png
--rw-rw-r--   0 tom       (1000) tom       (1000)  1494359 2022-09-06 22:43:36.000000 decoder-plus-plus-1.7.0/dpp/images/dpp_modern_big.png
--rw-rw-r--   0 tom       (1000) tom       (1000)    56153 2024-04-06 19:21:10.000000 decoder-plus-plus-1.7.0/dpp/images/dpp_stylized.png
--rw-rw-r--   0 tom       (1000) tom       (1000)    19277 2024-04-06 19:21:46.000000 decoder-plus-plus-1.7.0/dpp/images/dpp_stylized_128.png
--rw-rw-r--   0 tom       (1000) tom       (1000)    25196 2021-12-26 21:21:06.000000 decoder-plus-plus-1.7.0/dpp/images/dpp_xmas.png
--rw-rw-r--   0 tom       (1000) tom       (1000)    52648 2024-04-06 19:39:41.000000 decoder-plus-plus-1.7.0/dpp/images/dpp_xmas_stylized.png
--rw-rw-r--   0 tom       (1000) tom       (1000)      258 2021-12-26 21:21:06.000000 decoder-plus-plus-1.7.0/dpp/images/hidden.png
--rw-rw-r--   0 tom       (1000) tom       (1000)      349 2022-09-13 21:04:47.000000 decoder-plus-plus-1.7.0/dpp/images/indicator_green.png
--rw-rw-r--   0 tom       (1000) tom       (1000)      417 2022-09-13 21:05:13.000000 decoder-plus-plus-1.7.0/dpp/images/indicator_grey.png
--rw-rw-r--   0 tom       (1000) tom       (1000)      319 2022-09-13 21:05:36.000000 decoder-plus-plus-1.7.0/dpp/images/indicator_red.png
--rw-rw-r--   0 tom       (1000) tom       (1000)    11652 2021-12-26 21:21:06.000000 decoder-plus-plus-1.7.0/dpp/images/keyboard.png
--rw-rw-r--   0 tom       (1000) tom       (1000)    27999 2021-12-26 21:21:06.000000 decoder-plus-plus-1.7.0/dpp/images/keyboard.svg
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-07 11:36:23.966036 decoder-plus-plus-1.7.0/dpp/plugins/
--rw-rw-r--   0 tom       (1000) tom       (1000)     1328 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.0/dpp/plugins/adler32_hasher.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1393 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.0/dpp/plugins/apache_md5_hasher.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1545 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.0/dpp/plugins/base16_decoder.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1545 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.0/dpp/plugins/base16_encoder.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1824 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.0/dpp/plugins/base32_decoder.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1529 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.0/dpp/plugins/base32_encoder.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1755 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.0/dpp/plugins/base45_decoder.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1482 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.0/dpp/plugins/base45_encoder.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     2097 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.0/dpp/plugins/base64_decoder.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1470 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.0/dpp/plugins/base64_encoder.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     2678 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.0/dpp/plugins/base64_url_decoder.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1693 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.0/dpp/plugins/base64_url_encoder.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1241 2022-09-17 09:11:33.000000 decoder-plus-plus-1.7.0/dpp/plugins/bin_int_decoder.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1249 2022-09-17 09:11:33.000000 decoder-plus-plus-1.7.0/dpp/plugins/bin_int_encoder.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1519 2022-09-17 09:11:33.000000 decoder-plus-plus-1.7.0/dpp/plugins/bin_str_decoder.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1695 2022-09-17 09:11:33.000000 decoder-plus-plus-1.7.0/dpp/plugins/bin_str_encoder.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     5641 2024-04-05 16:00:23.000000 decoder-plus-plus-1.7.0/dpp/plugins/caesar_cipher_script.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1065 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.0/dpp/plugins/clone_script.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1320 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.0/dpp/plugins/crc32_hasher.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1159 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.0/dpp/plugins/css_minify_script.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     5888 2024-04-06 15:56:04.000000 decoder-plus-plus-1.7.0/dpp/plugins/custom_code.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1475 2022-09-17 09:13:06.000000 decoder-plus-plus-1.7.0/dpp/plugins/dec_str_decoder.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1441 2022-09-17 09:13:12.000000 decoder-plus-plus-1.7.0/dpp/plugins/dec_str_encoder.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1068 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.0/dpp/plugins/escape_string_script.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1211 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.0/dpp/plugins/extract_urls_script.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     5143 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.0/dpp/plugins/filter_lines_script.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1386 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.0/dpp/plugins/free_bsd_nt_hasher.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1653 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.0/dpp/plugins/gzip_decoder.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1408 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.0/dpp/plugins/gzip_encoder.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     2110 2022-11-01 18:01:29.000000 decoder-plus-plus-1.7.0/dpp/plugins/hex_char_decoder.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1582 2022-11-01 18:01:29.000000 decoder-plus-plus-1.7.0/dpp/plugins/hex_char_encoder.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1448 2022-11-01 18:01:29.000000 decoder-plus-plus-1.7.0/dpp/plugins/hex_int_decoder.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1217 2022-11-01 18:01:29.000000 decoder-plus-plus-1.7.0/dpp/plugins/hex_int_encoder.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     2331 2022-11-01 18:01:29.000000 decoder-plus-plus-1.7.0/dpp/plugins/hex_shell_decoder.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1980 2022-11-01 18:01:29.000000 decoder-plus-plus-1.7.0/dpp/plugins/hex_shell_encoder.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1709 2022-11-01 18:01:29.000000 decoder-plus-plus-1.7.0/dpp/plugins/hex_str_decoder.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1561 2022-11-01 18:01:29.000000 decoder-plus-plus-1.7.0/dpp/plugins/hex_str_encoder.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1221 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.0/dpp/plugins/html_beautify_script.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1783 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.0/dpp/plugins/html_decoder.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1377 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.0/dpp/plugins/html_encoder.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1138 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.0/dpp/plugins/html_minify_script.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     2539 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.0/dpp/plugins/http64_decoder.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1841 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.0/dpp/plugins/http64_encoder.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     2265 2024-04-07 11:11:41.000000 decoder-plus-plus-1.7.0/dpp/plugins/identify_decoder_script.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1371 2024-04-07 11:16:17.000000 decoder-plus-plus-1.7.0/dpp/plugins/identify_file_type_filemagic_script.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1478 2024-04-07 11:16:17.000000 decoder-plus-plus-1.7.0/dpp/plugins/identify_file_type_magika_script.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1389 2024-04-07 11:03:59.000000 decoder-plus-plus-1.7.0/dpp/plugins/identify_hash_format_script.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     2254 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.0/dpp/plugins/jq_script.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1336 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.0/dpp/plugins/js_beautify_script.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1131 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.0/dpp/plugins/js_minify_script.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1171 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.0/dpp/plugins/js_to_xml_script.py
--rw-rw-r--   0 tom       (1000) tom       (1000)    15185 2024-04-07 08:30:22.000000 decoder-plus-plus-1.7.0/dpp/plugins/jsonify_script.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     2621 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.0/dpp/plugins/jsonpath_script.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1612 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.0/dpp/plugins/jwt_decoder.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1432 2022-09-15 16:34:02.000000 decoder-plus-plus-1.7.0/dpp/plugins/keccak224_hasher.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1440 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.0/dpp/plugins/keccak256_hasher.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1472 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.0/dpp/plugins/keccak384_hasher.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1519 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.0/dpp/plugins/keccak512_hasher.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1446 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.0/dpp/plugins/little_big_endian_script.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1366 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.0/dpp/plugins/lm_hasher.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1364 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.0/dpp/plugins/md2_hasher.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1364 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.0/dpp/plugins/md4_hasher.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1352 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.0/dpp/plugins/md5_hasher.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1366 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.0/dpp/plugins/nt_hasher.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1223 2022-09-17 09:11:33.000000 decoder-plus-plus-1.7.0/dpp/plugins/oct_int_decoder.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1228 2022-09-17 09:11:33.000000 decoder-plus-plus-1.7.0/dpp/plugins/oct_int_encoder.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1775 2022-09-17 09:11:33.000000 decoder-plus-plus-1.7.0/dpp/plugins/oct_str_decoder.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1576 2022-09-17 09:11:33.000000 decoder-plus-plus-1.7.0/dpp/plugins/oct_str_encoder.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1368 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.0/dpp/plugins/phpass_hasher.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     6590 2024-04-05 18:32:58.000000 decoder-plus-plus-1.7.0/dpp/plugins/reformat_text_script.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1115 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.0/dpp/plugins/remove_newlines_script.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1121 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.0/dpp/plugins/remove_whitespaces_script.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1693 2024-04-07 07:30:09.000000 decoder-plus-plus-1.7.0/dpp/plugins/ripemd160_hasher.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1398 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.0/dpp/plugins/rot13_decoder.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1398 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.0/dpp/plugins/rot13_encoder.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     4506 2024-04-05 18:32:58.000000 decoder-plus-plus-1.7.0/dpp/plugins/search_and_replace_script.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1363 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.0/dpp/plugins/sha1_hasher.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1401 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.0/dpp/plugins/sha224_hasher.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1409 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.0/dpp/plugins/sha256_hasher.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1441 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.0/dpp/plugins/sha384_hasher.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1382 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.0/dpp/plugins/sha3_224_hasher.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1383 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.0/dpp/plugins/sha3_256_hasher.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1415 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.0/dpp/plugins/sha3_384_hasher.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1462 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.0/dpp/plugins/sha3_512_hasher.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1474 2022-09-12 18:36:42.000000 decoder-plus-plus-1.7.0/dpp/plugins/sha512_hasher.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     4998 2024-04-05 18:32:58.000000 decoder-plus-plus-1.7.0/dpp/plugins/split_and_rejoin_script.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1400 2022-09-12 18:36:42.000000 decoder-plus-plus-1.7.0/dpp/plugins/sun_md5_hasher.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1107 2022-09-12 18:36:42.000000 decoder-plus-plus-1.7.0/dpp/plugins/unescape_string_script.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1993 2022-09-12 18:36:42.000000 decoder-plus-plus-1.7.0/dpp/plugins/url_decoder.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1487 2022-09-12 18:36:42.000000 decoder-plus-plus-1.7.0/dpp/plugins/url_encoder.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1974 2022-09-12 18:36:42.000000 decoder-plus-plus-1.7.0/dpp/plugins/url_plus_decoder.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1525 2022-09-12 18:36:42.000000 decoder-plus-plus-1.7.0/dpp/plugins/url_plus_encoder.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     2291 2023-01-15 14:37:27.000000 decoder-plus-plus-1.7.0/dpp/plugins/xpath_script.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1821 2022-09-12 18:36:42.000000 decoder-plus-plus-1.7.0/dpp/plugins/zlib_decoder.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1394 2022-09-12 18:36:42.000000 decoder-plus-plus-1.7.0/dpp/plugins/zlib_encoder.py
--rwxrwxr-x   0 tom       (1000) tom       (1000)    16769 2022-09-21 05:00:04.000000 decoder-plus-plus-1.7.0/dpp/runner.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-07 11:36:23.966036 decoder-plus-plus-1.7.0/dpp/ui/
--rw-rw-r--   0 tom       (1000) tom       (1000)      967 2022-09-06 05:50:59.000000 decoder-plus-plus-1.7.0/dpp/ui/__init__.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-07 11:36:23.966036 decoder-plus-plus-1.7.0/dpp/ui/builder/
--rw-rw-r--   0 tom       (1000) tom       (1000)        0 2021-12-26 21:21:06.000000 decoder-plus-plus-1.7.0/dpp/ui/builder/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1962 2022-08-15 20:49:18.000000 decoder-plus-plus-1.7.0/dpp/ui/builder/action_builder.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1547 2023-03-07 03:42:36.000000 decoder-plus-plus-1.7.0/dpp/ui/builder/input_text_builder.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1682 2024-04-05 15:27:20.000000 decoder-plus-plus-1.7.0/dpp/ui/builder/plugin_config_widget_builder.py
--rw-rw-r--   0 tom       (1000) tom       (1000)    10393 2024-04-07 07:53:50.000000 decoder-plus-plus-1.7.0/dpp/ui/builder/widget_builder.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     6388 2023-01-29 15:44:47.000000 decoder-plus-plus-1.7.0/dpp/ui/decoder_plus_plus_gui.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-07 11:36:23.970036 decoder-plus-plus-1.7.0/dpp/ui/dialog/
--rw-rw-r--   0 tom       (1000) tom       (1000)      706 2021-12-26 21:21:06.000000 decoder-plus-plus-1.7.0/dpp/ui/dialog/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     5833 2024-04-06 19:42:04.000000 decoder-plus-plus-1.7.0/dpp/ui/dialog/config_dialog.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     5273 2022-09-10 21:34:51.000000 decoder-plus-plus-1.7.0/dpp/ui/dialog/keyboard_shortcut_dialog.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     6012 2024-04-06 09:24:31.000000 decoder-plus-plus-1.7.0/dpp/ui/dialog/plugin_config_dialog.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-07 11:36:23.970036 decoder-plus-plus-1.7.0/dpp/ui/dock/
--rw-rw-r--   0 tom       (1000) tom       (1000)        0 2021-12-26 21:21:06.000000 decoder-plus-plus-1.7.0/dpp/ui/dock/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)    10582 2023-02-28 12:28:51.000000 decoder-plus-plus-1.7.0/dpp/ui/dock/hex_dock.py
--rw-rw-r--   0 tom       (1000) tom       (1000)    12701 2022-09-12 19:05:02.000000 decoder-plus-plus-1.7.0/dpp/ui/dock/log_dock.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     2564 2022-09-07 22:11:21.000000 decoder-plus-plus-1.7.0/dpp/ui/instance_handler.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-07 11:36:23.970036 decoder-plus-plus-1.7.0/dpp/ui/view/
--rw-rw-r--   0 tom       (1000) tom       (1000)      706 2022-08-18 00:21:03.000000 decoder-plus-plus-1.7.0/dpp/ui/view/__init__.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-07 11:36:23.970036 decoder-plus-plus-1.7.0/dpp/ui/view/classic/
--rw-rw-r--   0 tom       (1000) tom       (1000)      839 2022-08-20 19:51:05.000000 decoder-plus-plus-1.7.0/dpp/ui/view/classic/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)    10186 2024-04-06 16:14:35.000000 decoder-plus-plus-1.7.0/dpp/ui/view/classic/classic_main_window_widget.py
--rw-rw-r--   0 tom       (1000) tom       (1000)    16982 2024-04-06 20:23:23.000000 decoder-plus-plus-1.7.0/dpp/ui/view/classic/codec_frame.py
--rw-rw-r--   0 tom       (1000) tom       (1000)    13200 2022-09-15 16:14:00.000000 decoder-plus-plus-1.7.0/dpp/ui/view/classic/codec_frame_header.py
--rw-rw-r--   0 tom       (1000) tom       (1000)    20241 2023-03-14 08:06:16.000000 decoder-plus-plus-1.7.0/dpp/ui/view/classic/codec_frames.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     2401 2022-09-20 04:28:03.000000 decoder-plus-plus-1.7.0/dpp/ui/view/classic/codec_tab.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     9167 2023-01-30 13:35:51.000000 decoder-plus-plus-1.7.0/dpp/ui/view/classic/combo_box_frame.py
--rw-rw-r--   0 tom       (1000) tom       (1000)    10716 2022-09-21 05:00:04.000000 decoder-plus-plus-1.7.0/dpp/ui/view/main_window_widget.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-07 11:36:23.970036 decoder-plus-plus-1.7.0/dpp/ui/view/modern/
--rw-rw-r--   0 tom       (1000) tom       (1000)      705 2022-08-20 19:51:05.000000 decoder-plus-plus-1.7.0/dpp/ui/view/modern/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     2460 2022-09-17 10:02:26.000000 decoder-plus-plus-1.7.0/dpp/ui/view/modern/modern_main_window_widget.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      705 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.0/dpp/ui/view/modern/node_data.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     5229 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.0/dpp/ui/view/modern/node_data_models.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      409 2022-08-30 00:07:08.000000 decoder-plus-plus-1.7.0/dpp/ui/view/modern/node_data_models_builder.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     2001 2022-09-17 10:02:44.000000 decoder-plus-plus-1.7.0/dpp/ui/view/modern/node_editor.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1782 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.0/dpp/ui/view/modern/node_editor_tab.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-07 11:36:23.978036 decoder-plus-plus-1.7.0/dpp/ui/widget/
--rw-rw-r--   0 tom       (1000) tom       (1000)      805 2022-08-16 19:35:20.000000 decoder-plus-plus-1.7.0/dpp/ui/widget/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1367 2022-08-15 23:02:30.000000 decoder-plus-plus-1.7.0/dpp/ui/widget/clickable_label.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     3507 2024-04-06 16:14:35.000000 decoder-plus-plus-1.7.0/dpp/ui/widget/code_editor_widget.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     3404 2024-04-07 09:41:34.000000 decoder-plus-plus-1.7.0/dpp/ui/widget/codec_preview_widget.py
--rw-rw-r--   0 tom       (1000) tom       (1000)    11051 2024-04-06 07:30:01.000000 decoder-plus-plus-1.7.0/dpp/ui/widget/collapsible_frame.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     2161 2022-09-10 22:00:08.000000 decoder-plus-plus-1.7.0/dpp/ui/widget/combo_box.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     4686 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.0/dpp/ui/widget/dock_tabs_widget.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     7690 2022-08-20 19:51:05.000000 decoder-plus-plus-1.7.0/dpp/ui/widget/dock_widget.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1887 2022-08-15 20:48:14.000000 decoder-plus-plus-1.7.0/dpp/ui/widget/dyna_frame.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      755 2022-08-15 20:44:52.000000 decoder-plus-plus-1.7.0/dpp/ui/widget/elided_label.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     2453 2024-04-06 20:17:41.000000 decoder-plus-plus-1.7.0/dpp/ui/widget/hover_label.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1793 2024-04-06 07:22:30.000000 decoder-plus-plus-1.7.0/dpp/ui/widget/icon_label.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     3270 2024-04-07 11:20:24.000000 decoder-plus-plus-1.7.0/dpp/ui/widget/identify_format_button.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     3269 2022-09-12 19:34:03.000000 decoder-plus-plus-1.7.0/dpp/ui/widget/list_widget.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1151 2022-08-21 00:18:15.000000 decoder-plus-plus-1.7.0/dpp/ui/widget/menu_bar.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     2136 2024-04-06 09:24:31.000000 decoder-plus-plus-1.7.0/dpp/ui/widget/message_box_widget.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     6687 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.0/dpp/ui/widget/message_widget.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     6110 2024-04-06 15:44:53.000000 decoder-plus-plus-1.7.0/dpp/ui/widget/option_widgets.py
--rw-rw-r--   0 tom       (1000) tom       (1000)    16152 2023-03-14 08:16:41.000000 decoder-plus-plus-1.7.0/dpp/ui/widget/plain_view.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     2621 2022-09-08 00:44:43.000000 decoder-plus-plus-1.7.0/dpp/ui/widget/plugin_frame.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     9593 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.0/dpp/ui/widget/plugin_tab.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     4396 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.0/dpp/ui/widget/search_field.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1246 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.0/dpp/ui/widget/separater_widget.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     5000 2022-08-15 23:02:30.000000 decoder-plus-plus-1.7.0/dpp/ui/widget/shortcut_table.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     2846 2022-09-12 18:36:42.000000 decoder-plus-plus-1.7.0/dpp/ui/widget/slider_widget.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     4055 2022-09-20 10:34:13.000000 decoder-plus-plus-1.7.0/dpp/ui/widget/smart_decode_button.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1442 2022-09-12 18:36:42.000000 decoder-plus-plus-1.7.0/dpp/ui/widget/spacers.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     2425 2023-01-30 12:23:56.000000 decoder-plus-plus-1.7.0/dpp/ui/widget/status_widget.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     3757 2022-08-20 19:51:05.000000 decoder-plus-plus-1.7.0/dpp/ui/widget/tab_bar.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     8075 2022-09-15 01:50:24.000000 decoder-plus-plus-1.7.0/dpp/ui/widget/tabs_widget.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     3210 2024-04-05 11:52:36.000000 decoder-plus-plus-1.7.0/dpp/ui/widget/text_widget.py
--rw-rw-r--   0 tom       (1000) tom       (1000)       38 2024-04-07 11:36:23.990036 decoder-plus-plus-1.7.0/setup.cfg
--rw-rw-r--   0 tom       (1000) tom       (1000)     2679 2024-04-07 10:39:21.000000 decoder-plus-plus-1.7.0/setup.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-07 11:36:23.978036 decoder-plus-plus-1.7.0/tests/
--rw-rw-r--   0 tom       (1000) tom       (1000)     1805 2023-01-15 14:31:34.000000 decoder-plus-plus-1.7.0/tests/__init__.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-07 11:36:23.990036 decoder-plus-plus-1.7.0/tests/plugins/
--rw-rw-r--   0 tom       (1000) tom       (1000)        0 2022-11-01 13:33:59.000000 decoder-plus-plus-1.7.0/tests/plugins/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1113 2022-11-01 14:08:45.000000 decoder-plus-plus-1.7.0/tests/plugins/adler32_hasher_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1191 2022-11-01 18:50:27.000000 decoder-plus-plus-1.7.0/tests/plugins/apache_md5_hasher_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1295 2022-11-01 18:05:54.000000 decoder-plus-plus-1.7.0/tests/plugins/base16_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1680 2023-01-15 13:01:54.000000 decoder-plus-plus-1.7.0/tests/plugins/base32_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1287 2023-01-15 13:32:25.000000 decoder-plus-plus-1.7.0/tests/plugins/base45_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1288 2023-01-15 12:36:51.000000 decoder-plus-plus-1.7.0/tests/plugins/base64_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1474 2023-01-15 12:47:27.000000 decoder-plus-plus-1.7.0/tests/plugins/base64_url_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1229 2023-01-15 13:29:43.000000 decoder-plus-plus-1.7.0/tests/plugins/bin_int_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1040 2022-11-01 18:51:09.000000 decoder-plus-plus-1.7.0/tests/plugins/bin_str_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      992 2023-01-15 12:47:59.000000 decoder-plus-plus-1.7.0/tests/plugins/caesar_cipher_script_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1222 2022-11-01 18:35:38.000000 decoder-plus-plus-1.7.0/tests/plugins/clone_script_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1108 2023-01-15 12:37:31.000000 decoder-plus-plus-1.7.0/tests/plugins/crc32_hasher_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1183 2022-11-01 18:39:55.000000 decoder-plus-plus-1.7.0/tests/plugins/css_minify_script_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1401 2022-11-01 18:35:21.000000 decoder-plus-plus-1.7.0/tests/plugins/dec_str_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1245 2022-11-01 18:59:45.000000 decoder-plus-plus-1.7.0/tests/plugins/escape_string_script_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1123 2022-11-01 18:47:57.000000 decoder-plus-plus-1.7.0/tests/plugins/extract_urls_script_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1165 2022-11-01 18:40:22.000000 decoder-plus-plus-1.7.0/tests/plugins/filter_lines_script_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1189 2023-01-15 13:03:50.000000 decoder-plus-plus-1.7.0/tests/plugins/free_bsd_nt_hasher_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1253 2023-01-15 12:29:09.000000 decoder-plus-plus-1.7.0/tests/plugins/gzip_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1067 2022-11-01 18:47:18.000000 decoder-plus-plus-1.7.0/tests/plugins/hex_char_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1193 2023-01-15 13:10:42.000000 decoder-plus-plus-1.7.0/tests/plugins/hex_int_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1614 2022-11-01 18:43:06.000000 decoder-plus-plus-1.7.0/tests/plugins/hex_shell_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1313 2023-01-15 13:16:46.000000 decoder-plus-plus-1.7.0/tests/plugins/hex_str_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1173 2022-11-01 18:43:28.000000 decoder-plus-plus-1.7.0/tests/plugins/html_beautify_script_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1168 2022-11-01 18:48:47.000000 decoder-plus-plus-1.7.0/tests/plugins/html_minify_script_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1172 2023-01-15 12:22:31.000000 decoder-plus-plus-1.7.0/tests/plugins/html_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1219 2022-11-01 18:32:01.000000 decoder-plus-plus-1.7.0/tests/plugins/http64_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1004 2023-01-15 12:39:55.000000 decoder-plus-plus-1.7.0/tests/plugins/identify_file_type_script_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1108 2022-11-01 18:39:55.000000 decoder-plus-plus-1.7.0/tests/plugins/identify_hash_format_script_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1145 2023-01-15 13:26:35.000000 decoder-plus-plus-1.7.0/tests/plugins/jq_script_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      988 2023-01-15 12:41:00.000000 decoder-plus-plus-1.7.0/tests/plugins/js_beautify_script_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1164 2022-11-01 18:49:20.000000 decoder-plus-plus-1.7.0/tests/plugins/js_minify_script_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      977 2023-01-15 13:06:33.000000 decoder-plus-plus-1.7.0/tests/plugins/js_to_xml_script_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      981 2023-01-15 13:02:34.000000 decoder-plus-plus-1.7.0/tests/plugins/jsonify_script_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1163 2022-11-01 18:49:36.000000 decoder-plus-plus-1.7.0/tests/plugins/jsonpath_script_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      976 2023-01-15 12:39:55.000000 decoder-plus-plus-1.7.0/tests/plugins/jwt_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1163 2023-01-15 13:02:49.000000 decoder-plus-plus-1.7.0/tests/plugins/keccak224_hasher_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1171 2022-11-01 18:56:46.000000 decoder-plus-plus-1.7.0/tests/plugins/keccak256_hasher_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1203 2022-11-01 18:45:25.000000 decoder-plus-plus-1.7.0/tests/plugins/keccak384_hasher_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1235 2022-11-01 18:48:57.000000 decoder-plus-plus-1.7.0/tests/plugins/keccak512_hasher_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1245 2022-11-01 18:31:13.000000 decoder-plus-plus-1.7.0/tests/plugins/little_big_endian_script_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1124 2022-11-01 18:56:24.000000 decoder-plus-plus-1.7.0/tests/plugins/lm_hasher_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1126 2022-11-01 18:24:14.000000 decoder-plus-plus-1.7.0/tests/plugins/md2_hasher_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1126 2022-11-01 18:56:15.000000 decoder-plus-plus-1.7.0/tests/plugins/md4_hasher_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1126 2022-11-01 18:45:18.000000 decoder-plus-plus-1.7.0/tests/plugins/md5_hasher_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1124 2022-11-01 18:46:24.000000 decoder-plus-plus-1.7.0/tests/plugins/nt_hasher_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1193 2023-01-15 13:13:49.000000 decoder-plus-plus-1.7.0/tests/plugins/oct_int_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1405 2022-11-01 18:20:57.000000 decoder-plus-plus-1.7.0/tests/plugins/oct_str_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1181 2023-01-15 12:51:06.000000 decoder-plus-plus-1.7.0/tests/plugins/phpass_hasher_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1167 2022-11-01 18:57:07.000000 decoder-plus-plus-1.7.0/tests/plugins/reformat_text_script_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1187 2023-01-15 13:04:21.000000 decoder-plus-plus-1.7.0/tests/plugins/remove_newlines_script_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1064 2022-11-01 18:56:04.000000 decoder-plus-plus-1.7.0/tests/plugins/remove_whitespaces_script_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1146 2022-11-01 18:56:36.000000 decoder-plus-plus-1.7.0/tests/plugins/ripemd160_hasher_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1225 2022-11-01 18:26:44.000000 decoder-plus-plus-1.7.0/tests/plugins/rot13_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1503 2023-01-15 13:05:35.000000 decoder-plus-plus-1.7.0/tests/plugins/search_and_replace_script_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1136 2022-11-01 18:27:54.000000 decoder-plus-plus-1.7.0/tests/plugins/sha1_hasher_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1192 2022-11-01 18:29:14.000000 decoder-plus-plus-1.7.0/tests/plugins/sha224_hasher_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1200 2022-11-01 18:29:35.000000 decoder-plus-plus-1.7.0/tests/plugins/sha256_hasher_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1231 2022-11-01 18:29:59.000000 decoder-plus-plus-1.7.0/tests/plugins/sha384_hasher_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1160 2023-01-15 12:37:21.000000 decoder-plus-plus-1.7.0/tests/plugins/sha3_224_hasher_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1168 2022-11-01 18:53:45.000000 decoder-plus-plus-1.7.0/tests/plugins/sha3_256_hasher_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1200 2022-11-01 18:28:35.000000 decoder-plus-plus-1.7.0/tests/plugins/sha3_384_hasher_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1268 2022-11-01 18:28:57.000000 decoder-plus-plus-1.7.0/tests/plugins/sha3_512_hasher_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1263 2022-11-01 18:30:17.000000 decoder-plus-plus-1.7.0/tests/plugins/sha512_hasher_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1170 2022-11-01 18:57:46.000000 decoder-plus-plus-1.7.0/tests/plugins/split_and_rejoin_script_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      983 2023-01-15 12:39:55.000000 decoder-plus-plus-1.7.0/tests/plugins/sun_md5_hasher_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1247 2022-11-01 18:32:56.000000 decoder-plus-plus-1.7.0/tests/plugins/unescape_string_script_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1282 2022-11-01 18:45:08.000000 decoder-plus-plus-1.7.0/tests/plugins/url_plus_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1136 2022-11-01 18:53:35.000000 decoder-plus-plus-1.7.0/tests/plugins/url_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1136 2023-01-15 14:38:44.000000 decoder-plus-plus-1.7.0/tests/plugins/xpath_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1223 2023-01-15 13:12:30.000000 decoder-plus-plus-1.7.0/tests/plugins/zlib_test.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-07 11:36:23.990036 decoder-plus-plus-1.7.0/tests/ui/
--rw-rw-r--   0 tom       (1000) tom       (1000)        0 2023-01-15 14:39:42.000000 decoder-plus-plus-1.7.0/tests/ui/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     8727 2024-04-06 20:29:29.000000 decoder-plus-plus-1.7.0/tests/ui/classic_mode_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      512 2023-01-15 15:28:09.000000 decoder-plus-plus-1.7.0/tests/utils.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-07 18:16:03.754202 decoder-plus-plus-1.7.1/
+-rw-rw-r--   0 tom       (1000) tom       (1000)    35147 2021-12-26 21:21:06.000000 decoder-plus-plus-1.7.1/LICENSE
+-rw-rw-r--   0 tom       (1000) tom       (1000)       43 2021-12-26 21:21:06.000000 decoder-plus-plus-1.7.1/MANIFEST.in
+-rw-rw-r--   0 tom       (1000) tom       (1000)     7935 2024-04-07 18:16:03.754202 decoder-plus-plus-1.7.1/PKG-INFO
+-rw-rw-r--   0 tom       (1000) tom       (1000)     7367 2024-04-07 09:27:21.000000 decoder-plus-plus-1.7.1/README.md
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-07 18:16:03.658201 decoder-plus-plus-1.7.1/data/
+-rwxrwxr-x   0 tom       (1000) tom       (1000)      116 2021-12-26 21:21:06.000000 decoder-plus-plus-1.7.1/data/dpp.desktop
+-rw-rw-r--   0 tom       (1000) tom       (1000)    19277 2024-04-06 19:21:46.000000 decoder-plus-plus-1.7.1/data/dpp.png
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-07 18:16:03.658201 decoder-plus-plus-1.7.1/decoder_plus_plus.egg-info/
+-rw-rw-r--   0 tom       (1000) tom       (1000)     7935 2024-04-07 18:16:03.000000 decoder-plus-plus-1.7.1/decoder_plus_plus.egg-info/PKG-INFO
+-rw-rw-r--   0 tom       (1000) tom       (1000)     9135 2024-04-07 18:16:03.000000 decoder-plus-plus-1.7.1/decoder_plus_plus.egg-info/SOURCES.txt
+-rw-rw-r--   0 tom       (1000) tom       (1000)        1 2024-04-07 18:16:03.000000 decoder-plus-plus-1.7.1/decoder_plus_plus.egg-info/dependency_links.txt
+-rw-rw-r--   0 tom       (1000) tom       (1000)       40 2024-04-07 18:16:03.000000 decoder-plus-plus-1.7.1/decoder_plus_plus.egg-info/entry_points.txt
+-rw-rw-r--   0 tom       (1000) tom       (1000)      389 2024-04-07 18:16:03.000000 decoder-plus-plus-1.7.1/decoder_plus_plus.egg-info/requires.txt
+-rw-rw-r--   0 tom       (1000) tom       (1000)       10 2024-04-07 18:16:03.000000 decoder-plus-plus-1.7.1/decoder_plus_plus.egg-info/top_level.txt
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-07 18:16:03.658201 decoder-plus-plus-1.7.1/dpp/
+-rw-rw-r--   0 tom       (1000) tom       (1000)      850 2024-04-07 18:09:02.000000 decoder-plus-plus-1.7.1/dpp/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      239 2021-12-26 21:21:06.000000 decoder-plus-plus-1.7.1/dpp/__main__.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-07 18:16:03.662201 decoder-plus-plus-1.7.1/dpp/core/
+-rw-rw-r--   0 tom       (1000) tom       (1000)      915 2021-12-26 21:21:06.000000 decoder-plus-plus-1.7.1/dpp/core/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2353 2022-09-12 19:05:02.000000 decoder-plus-plus-1.7.1/dpp/core/argparse.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2871 2022-09-12 21:57:24.000000 decoder-plus-plus-1.7.1/dpp/core/assertions.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     3279 2022-08-17 05:09:19.000000 decoder-plus-plus-1.7.1/dpp/core/config.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)    10068 2024-04-05 20:12:39.000000 decoder-plus-plus-1.7.1/dpp/core/context.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2328 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.1/dpp/core/decoder_plus_plus.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      906 2022-09-18 10:36:35.000000 decoder-plus-plus-1.7.1/dpp/core/exceptions.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2860 2024-04-07 11:17:10.000000 decoder-plus-plus-1.7.1/dpp/core/icons.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     3650 2023-02-28 12:27:33.000000 decoder-plus-plus-1.7.1/dpp/core/listener.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     4546 2023-01-29 15:42:26.000000 decoder-plus-plus-1.7.1/dpp/core/logger.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1329 2022-09-14 00:12:52.000000 decoder-plus-plus-1.7.1/dpp/core/math.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-07 18:16:03.662201 decoder-plus-plus-1.7.1/dpp/core/plugin/
+-rw-rw-r--   0 tom       (1000) tom       (1000)    14067 2024-04-06 16:14:35.000000 decoder-plus-plus-1.7.1/dpp/core/plugin/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2324 2024-04-06 15:25:06.000000 decoder-plus-plus-1.7.1/dpp/core/plugin/builder.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-07 18:16:03.662201 decoder-plus-plus-1.7.1/dpp/core/plugin/config/
+-rw-rw-r--   0 tom       (1000) tom       (1000)     8387 2024-04-06 08:18:07.000000 decoder-plus-plus-1.7.1/dpp/core/plugin/config/__init__.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-07 18:16:03.666201 decoder-plus-plus-1.7.1/dpp/core/plugin/config/options/
+-rw-rw-r--   0 tom       (1000) tom       (1000)     3478 2024-04-06 16:14:35.000000 decoder-plus-plus-1.7.1/dpp/core/plugin/config/options/__init__.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-07 18:16:03.666201 decoder-plus-plus-1.7.1/dpp/core/plugin/config/ui/
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1572 2022-09-12 21:57:24.000000 decoder-plus-plus-1.7.1/dpp/core/plugin/config/ui/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      858 2022-09-06 21:38:42.000000 decoder-plus-plus-1.7.1/dpp/core/plugin/config/ui/layouts.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2111 2024-04-06 15:51:05.000000 decoder-plus-plus-1.7.1/dpp/core/plugin/config/ui/widgets.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     3048 2022-09-13 07:31:54.000000 decoder-plus-plus-1.7.1/dpp/core/plugin/loader.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     4301 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.1/dpp/core/plugin/manager.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     3878 2022-08-21 00:18:15.000000 decoder-plus-plus-1.7.1/dpp/core/shortcuts.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-07 18:16:03.678201 decoder-plus-plus-1.7.1/dpp/images/
+-rw-rw-r--   0 tom       (1000) tom       (1000)    22919 2021-12-26 21:21:06.000000 decoder-plus-plus-1.7.1/dpp/images/dpp.png
+-rw-rw-r--   0 tom       (1000) tom       (1000)    10621 2021-12-26 21:21:06.000000 decoder-plus-plus-1.7.1/dpp/images/dpp_128.png
+-rw-rw-r--   0 tom       (1000) tom       (1000)    22919 2021-12-26 21:21:06.000000 decoder-plus-plus-1.7.1/dpp/images/dpp_classic.png
+-rw-rw-r--   0 tom       (1000) tom       (1000)    10621 2021-12-26 21:21:06.000000 decoder-plus-plus-1.7.1/dpp/images/dpp_classic_128.png
+-rw-rw-r--   0 tom       (1000) tom       (1000)    90434 2022-09-06 22:45:08.000000 decoder-plus-plus-1.7.1/dpp/images/dpp_modern.png
+-rw-rw-r--   0 tom       (1000) tom       (1000)    30058 2022-09-06 22:47:19.000000 decoder-plus-plus-1.7.1/dpp/images/dpp_modern_128.png
+-rw-rw-r--   0 tom       (1000) tom       (1000)  1494359 2022-09-06 22:43:36.000000 decoder-plus-plus-1.7.1/dpp/images/dpp_modern_big.png
+-rw-rw-r--   0 tom       (1000) tom       (1000)    56153 2024-04-06 19:21:10.000000 decoder-plus-plus-1.7.1/dpp/images/dpp_stylized.png
+-rw-rw-r--   0 tom       (1000) tom       (1000)    19277 2024-04-06 19:21:46.000000 decoder-plus-plus-1.7.1/dpp/images/dpp_stylized_128.png
+-rw-rw-r--   0 tom       (1000) tom       (1000)    25196 2021-12-26 21:21:06.000000 decoder-plus-plus-1.7.1/dpp/images/dpp_xmas.png
+-rw-rw-r--   0 tom       (1000) tom       (1000)    52648 2024-04-06 19:39:41.000000 decoder-plus-plus-1.7.1/dpp/images/dpp_xmas_stylized.png
+-rw-rw-r--   0 tom       (1000) tom       (1000)      258 2021-12-26 21:21:06.000000 decoder-plus-plus-1.7.1/dpp/images/hidden.png
+-rw-rw-r--   0 tom       (1000) tom       (1000)      349 2022-09-13 21:04:47.000000 decoder-plus-plus-1.7.1/dpp/images/indicator_green.png
+-rw-rw-r--   0 tom       (1000) tom       (1000)      417 2022-09-13 21:05:13.000000 decoder-plus-plus-1.7.1/dpp/images/indicator_grey.png
+-rw-rw-r--   0 tom       (1000) tom       (1000)      319 2022-09-13 21:05:36.000000 decoder-plus-plus-1.7.1/dpp/images/indicator_red.png
+-rw-rw-r--   0 tom       (1000) tom       (1000)    11652 2021-12-26 21:21:06.000000 decoder-plus-plus-1.7.1/dpp/images/keyboard.png
+-rw-rw-r--   0 tom       (1000) tom       (1000)    27999 2021-12-26 21:21:06.000000 decoder-plus-plus-1.7.1/dpp/images/keyboard.svg
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-07 18:16:03.706202 decoder-plus-plus-1.7.1/dpp/plugins/
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1328 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.1/dpp/plugins/adler32_hasher.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1393 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.1/dpp/plugins/apache_md5_hasher.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1545 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.1/dpp/plugins/base16_decoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1545 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.1/dpp/plugins/base16_encoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1824 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.1/dpp/plugins/base32_decoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1529 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.1/dpp/plugins/base32_encoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1755 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.1/dpp/plugins/base45_decoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1482 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.1/dpp/plugins/base45_encoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2097 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.1/dpp/plugins/base64_decoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1470 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.1/dpp/plugins/base64_encoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2678 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.1/dpp/plugins/base64_url_decoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1693 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.1/dpp/plugins/base64_url_encoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1241 2022-09-17 09:11:33.000000 decoder-plus-plus-1.7.1/dpp/plugins/bin_int_decoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1249 2022-09-17 09:11:33.000000 decoder-plus-plus-1.7.1/dpp/plugins/bin_int_encoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1519 2022-09-17 09:11:33.000000 decoder-plus-plus-1.7.1/dpp/plugins/bin_str_decoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1695 2022-09-17 09:11:33.000000 decoder-plus-plus-1.7.1/dpp/plugins/bin_str_encoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     5641 2024-04-05 16:00:23.000000 decoder-plus-plus-1.7.1/dpp/plugins/caesar_cipher_script.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1065 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.1/dpp/plugins/clone_script.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1320 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.1/dpp/plugins/crc32_hasher.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1159 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.1/dpp/plugins/css_minify_script.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     5888 2024-04-06 15:56:04.000000 decoder-plus-plus-1.7.1/dpp/plugins/custom_code.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1475 2022-09-17 09:13:06.000000 decoder-plus-plus-1.7.1/dpp/plugins/dec_str_decoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1441 2022-09-17 09:13:12.000000 decoder-plus-plus-1.7.1/dpp/plugins/dec_str_encoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1068 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.1/dpp/plugins/escape_string_script.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1211 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.1/dpp/plugins/extract_urls_script.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     5143 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.1/dpp/plugins/filter_lines_script.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1386 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.1/dpp/plugins/free_bsd_nt_hasher.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1653 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.1/dpp/plugins/gzip_decoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1408 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.1/dpp/plugins/gzip_encoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2110 2022-11-01 18:01:29.000000 decoder-plus-plus-1.7.1/dpp/plugins/hex_char_decoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1582 2022-11-01 18:01:29.000000 decoder-plus-plus-1.7.1/dpp/plugins/hex_char_encoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1448 2022-11-01 18:01:29.000000 decoder-plus-plus-1.7.1/dpp/plugins/hex_int_decoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1217 2022-11-01 18:01:29.000000 decoder-plus-plus-1.7.1/dpp/plugins/hex_int_encoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2331 2022-11-01 18:01:29.000000 decoder-plus-plus-1.7.1/dpp/plugins/hex_shell_decoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1980 2022-11-01 18:01:29.000000 decoder-plus-plus-1.7.1/dpp/plugins/hex_shell_encoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1709 2022-11-01 18:01:29.000000 decoder-plus-plus-1.7.1/dpp/plugins/hex_str_decoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1561 2022-11-01 18:01:29.000000 decoder-plus-plus-1.7.1/dpp/plugins/hex_str_encoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1221 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.1/dpp/plugins/html_beautify_script.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1783 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.1/dpp/plugins/html_decoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1377 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.1/dpp/plugins/html_encoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1138 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.1/dpp/plugins/html_minify_script.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2539 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.1/dpp/plugins/http64_decoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1841 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.1/dpp/plugins/http64_encoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2265 2024-04-07 11:11:41.000000 decoder-plus-plus-1.7.1/dpp/plugins/identify_decoder_script.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1371 2024-04-07 11:16:17.000000 decoder-plus-plus-1.7.1/dpp/plugins/identify_file_type_filemagic_script.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1478 2024-04-07 11:16:17.000000 decoder-plus-plus-1.7.1/dpp/plugins/identify_file_type_magika_script.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1389 2024-04-07 11:03:59.000000 decoder-plus-plus-1.7.1/dpp/plugins/identify_hash_format_script.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2254 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.1/dpp/plugins/jq_script.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1336 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.1/dpp/plugins/js_beautify_script.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1131 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.1/dpp/plugins/js_minify_script.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1171 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.1/dpp/plugins/js_to_xml_script.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)    15185 2024-04-07 08:30:22.000000 decoder-plus-plus-1.7.1/dpp/plugins/jsonify_script.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2621 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.1/dpp/plugins/jsonpath_script.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1612 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.1/dpp/plugins/jwt_decoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1432 2022-09-15 16:34:02.000000 decoder-plus-plus-1.7.1/dpp/plugins/keccak224_hasher.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1440 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.1/dpp/plugins/keccak256_hasher.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1472 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.1/dpp/plugins/keccak384_hasher.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1519 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.1/dpp/plugins/keccak512_hasher.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1446 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.1/dpp/plugins/little_big_endian_script.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1366 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.1/dpp/plugins/lm_hasher.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1364 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.1/dpp/plugins/md2_hasher.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1364 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.1/dpp/plugins/md4_hasher.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1352 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.1/dpp/plugins/md5_hasher.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1366 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.1/dpp/plugins/nt_hasher.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1223 2022-09-17 09:11:33.000000 decoder-plus-plus-1.7.1/dpp/plugins/oct_int_decoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1228 2022-09-17 09:11:33.000000 decoder-plus-plus-1.7.1/dpp/plugins/oct_int_encoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1775 2022-09-17 09:11:33.000000 decoder-plus-plus-1.7.1/dpp/plugins/oct_str_decoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1576 2022-09-17 09:11:33.000000 decoder-plus-plus-1.7.1/dpp/plugins/oct_str_encoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1368 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.1/dpp/plugins/phpass_hasher.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     6590 2024-04-05 18:32:58.000000 decoder-plus-plus-1.7.1/dpp/plugins/reformat_text_script.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1115 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.1/dpp/plugins/remove_newlines_script.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1121 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.1/dpp/plugins/remove_whitespaces_script.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1693 2024-04-07 07:30:09.000000 decoder-plus-plus-1.7.1/dpp/plugins/ripemd160_hasher.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1398 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.1/dpp/plugins/rot13_decoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1398 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.1/dpp/plugins/rot13_encoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     4506 2024-04-05 18:32:58.000000 decoder-plus-plus-1.7.1/dpp/plugins/search_and_replace_script.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1363 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.1/dpp/plugins/sha1_hasher.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1401 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.1/dpp/plugins/sha224_hasher.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1409 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.1/dpp/plugins/sha256_hasher.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1441 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.1/dpp/plugins/sha384_hasher.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1382 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.1/dpp/plugins/sha3_224_hasher.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1383 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.1/dpp/plugins/sha3_256_hasher.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1415 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.1/dpp/plugins/sha3_384_hasher.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1462 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.1/dpp/plugins/sha3_512_hasher.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1474 2022-09-12 18:36:42.000000 decoder-plus-plus-1.7.1/dpp/plugins/sha512_hasher.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     4998 2024-04-05 18:32:58.000000 decoder-plus-plus-1.7.1/dpp/plugins/split_and_rejoin_script.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1400 2022-09-12 18:36:42.000000 decoder-plus-plus-1.7.1/dpp/plugins/sun_md5_hasher.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1107 2022-09-12 18:36:42.000000 decoder-plus-plus-1.7.1/dpp/plugins/unescape_string_script.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1993 2022-09-12 18:36:42.000000 decoder-plus-plus-1.7.1/dpp/plugins/url_decoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1487 2022-09-12 18:36:42.000000 decoder-plus-plus-1.7.1/dpp/plugins/url_encoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1974 2022-09-12 18:36:42.000000 decoder-plus-plus-1.7.1/dpp/plugins/url_plus_decoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1525 2022-09-12 18:36:42.000000 decoder-plus-plus-1.7.1/dpp/plugins/url_plus_encoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2291 2023-01-15 14:37:27.000000 decoder-plus-plus-1.7.1/dpp/plugins/xpath_script.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1821 2022-09-12 18:36:42.000000 decoder-plus-plus-1.7.1/dpp/plugins/zlib_decoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1394 2022-09-12 18:36:42.000000 decoder-plus-plus-1.7.1/dpp/plugins/zlib_encoder.py
+-rwxrwxr-x   0 tom       (1000) tom       (1000)    16769 2022-09-21 05:00:04.000000 decoder-plus-plus-1.7.1/dpp/runner.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-07 18:16:03.706202 decoder-plus-plus-1.7.1/dpp/ui/
+-rw-rw-r--   0 tom       (1000) tom       (1000)      967 2022-09-06 05:50:59.000000 decoder-plus-plus-1.7.1/dpp/ui/__init__.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-07 18:16:03.706202 decoder-plus-plus-1.7.1/dpp/ui/builder/
+-rw-rw-r--   0 tom       (1000) tom       (1000)        0 2021-12-26 21:21:06.000000 decoder-plus-plus-1.7.1/dpp/ui/builder/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1962 2022-08-15 20:49:18.000000 decoder-plus-plus-1.7.1/dpp/ui/builder/action_builder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1547 2023-03-07 03:42:36.000000 decoder-plus-plus-1.7.1/dpp/ui/builder/input_text_builder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1682 2024-04-05 15:27:20.000000 decoder-plus-plus-1.7.1/dpp/ui/builder/plugin_config_widget_builder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)    10393 2024-04-07 07:53:50.000000 decoder-plus-plus-1.7.1/dpp/ui/builder/widget_builder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     6388 2023-01-29 15:44:47.000000 decoder-plus-plus-1.7.1/dpp/ui/decoder_plus_plus_gui.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-07 18:16:03.710202 decoder-plus-plus-1.7.1/dpp/ui/dialog/
+-rw-rw-r--   0 tom       (1000) tom       (1000)      706 2021-12-26 21:21:06.000000 decoder-plus-plus-1.7.1/dpp/ui/dialog/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     5833 2024-04-06 19:42:04.000000 decoder-plus-plus-1.7.1/dpp/ui/dialog/config_dialog.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     5273 2022-09-10 21:34:51.000000 decoder-plus-plus-1.7.1/dpp/ui/dialog/keyboard_shortcut_dialog.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     6012 2024-04-06 09:24:31.000000 decoder-plus-plus-1.7.1/dpp/ui/dialog/plugin_config_dialog.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-07 18:16:03.710202 decoder-plus-plus-1.7.1/dpp/ui/dock/
+-rw-rw-r--   0 tom       (1000) tom       (1000)        0 2021-12-26 21:21:06.000000 decoder-plus-plus-1.7.1/dpp/ui/dock/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)    10582 2023-02-28 12:28:51.000000 decoder-plus-plus-1.7.1/dpp/ui/dock/hex_dock.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)    12701 2022-09-12 19:05:02.000000 decoder-plus-plus-1.7.1/dpp/ui/dock/log_dock.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2564 2022-09-07 22:11:21.000000 decoder-plus-plus-1.7.1/dpp/ui/instance_handler.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-07 18:16:03.710202 decoder-plus-plus-1.7.1/dpp/ui/view/
+-rw-rw-r--   0 tom       (1000) tom       (1000)      706 2022-08-18 00:21:03.000000 decoder-plus-plus-1.7.1/dpp/ui/view/__init__.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-07 18:16:03.714202 decoder-plus-plus-1.7.1/dpp/ui/view/classic/
+-rw-rw-r--   0 tom       (1000) tom       (1000)      839 2022-08-20 19:51:05.000000 decoder-plus-plus-1.7.1/dpp/ui/view/classic/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)    10186 2024-04-06 16:14:35.000000 decoder-plus-plus-1.7.1/dpp/ui/view/classic/classic_main_window_widget.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)    16982 2024-04-07 13:12:43.000000 decoder-plus-plus-1.7.1/dpp/ui/view/classic/codec_frame.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)    13200 2022-09-15 16:14:00.000000 decoder-plus-plus-1.7.1/dpp/ui/view/classic/codec_frame_header.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)    20625 2024-04-07 18:07:00.000000 decoder-plus-plus-1.7.1/dpp/ui/view/classic/codec_frames.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2401 2022-09-20 04:28:03.000000 decoder-plus-plus-1.7.1/dpp/ui/view/classic/codec_tab.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     9167 2023-01-30 13:35:51.000000 decoder-plus-plus-1.7.1/dpp/ui/view/classic/combo_box_frame.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)    10716 2022-09-21 05:00:04.000000 decoder-plus-plus-1.7.1/dpp/ui/view/main_window_widget.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-07 18:16:03.722202 decoder-plus-plus-1.7.1/dpp/ui/view/modern/
+-rw-rw-r--   0 tom       (1000) tom       (1000)      705 2022-08-20 19:51:05.000000 decoder-plus-plus-1.7.1/dpp/ui/view/modern/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2460 2022-09-17 10:02:26.000000 decoder-plus-plus-1.7.1/dpp/ui/view/modern/modern_main_window_widget.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      705 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.1/dpp/ui/view/modern/node_data.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     5229 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.1/dpp/ui/view/modern/node_data_models.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      409 2022-08-30 00:07:08.000000 decoder-plus-plus-1.7.1/dpp/ui/view/modern/node_data_models_builder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2001 2022-09-17 10:02:44.000000 decoder-plus-plus-1.7.1/dpp/ui/view/modern/node_editor.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1782 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.1/dpp/ui/view/modern/node_editor_tab.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-07 18:16:03.730202 decoder-plus-plus-1.7.1/dpp/ui/widget/
+-rw-rw-r--   0 tom       (1000) tom       (1000)      805 2022-08-16 19:35:20.000000 decoder-plus-plus-1.7.1/dpp/ui/widget/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1367 2022-08-15 23:02:30.000000 decoder-plus-plus-1.7.1/dpp/ui/widget/clickable_label.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     3507 2024-04-06 16:14:35.000000 decoder-plus-plus-1.7.1/dpp/ui/widget/code_editor_widget.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     3404 2024-04-07 09:41:34.000000 decoder-plus-plus-1.7.1/dpp/ui/widget/codec_preview_widget.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)    11051 2024-04-06 07:30:01.000000 decoder-plus-plus-1.7.1/dpp/ui/widget/collapsible_frame.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2161 2022-09-10 22:00:08.000000 decoder-plus-plus-1.7.1/dpp/ui/widget/combo_box.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     4686 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.1/dpp/ui/widget/dock_tabs_widget.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     7690 2022-08-20 19:51:05.000000 decoder-plus-plus-1.7.1/dpp/ui/widget/dock_widget.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1887 2022-08-15 20:48:14.000000 decoder-plus-plus-1.7.1/dpp/ui/widget/dyna_frame.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      755 2022-08-15 20:44:52.000000 decoder-plus-plus-1.7.1/dpp/ui/widget/elided_label.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2453 2024-04-06 20:17:41.000000 decoder-plus-plus-1.7.1/dpp/ui/widget/hover_label.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1793 2024-04-06 07:22:30.000000 decoder-plus-plus-1.7.1/dpp/ui/widget/icon_label.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     3270 2024-04-07 11:20:24.000000 decoder-plus-plus-1.7.1/dpp/ui/widget/identify_format_button.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     3269 2022-09-12 19:34:03.000000 decoder-plus-plus-1.7.1/dpp/ui/widget/list_widget.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1151 2022-08-21 00:18:15.000000 decoder-plus-plus-1.7.1/dpp/ui/widget/menu_bar.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2136 2024-04-06 09:24:31.000000 decoder-plus-plus-1.7.1/dpp/ui/widget/message_box_widget.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     6687 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.1/dpp/ui/widget/message_widget.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     6110 2024-04-06 15:44:53.000000 decoder-plus-plus-1.7.1/dpp/ui/widget/option_widgets.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)    16152 2023-03-14 08:16:41.000000 decoder-plus-plus-1.7.1/dpp/ui/widget/plain_view.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2621 2022-09-08 00:44:43.000000 decoder-plus-plus-1.7.1/dpp/ui/widget/plugin_frame.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     9593 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.1/dpp/ui/widget/plugin_tab.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     4396 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.1/dpp/ui/widget/search_field.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1246 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.1/dpp/ui/widget/separater_widget.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     5000 2022-08-15 23:02:30.000000 decoder-plus-plus-1.7.1/dpp/ui/widget/shortcut_table.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2846 2022-09-12 18:36:42.000000 decoder-plus-plus-1.7.1/dpp/ui/widget/slider_widget.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     4055 2022-09-20 10:34:13.000000 decoder-plus-plus-1.7.1/dpp/ui/widget/smart_decode_button.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1442 2022-09-12 18:36:42.000000 decoder-plus-plus-1.7.1/dpp/ui/widget/spacers.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2425 2023-01-30 12:23:56.000000 decoder-plus-plus-1.7.1/dpp/ui/widget/status_widget.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     3757 2022-08-20 19:51:05.000000 decoder-plus-plus-1.7.1/dpp/ui/widget/tab_bar.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     8075 2022-09-15 01:50:24.000000 decoder-plus-plus-1.7.1/dpp/ui/widget/tabs_widget.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     3210 2024-04-05 11:52:36.000000 decoder-plus-plus-1.7.1/dpp/ui/widget/text_widget.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)       38 2024-04-07 18:16:03.754202 decoder-plus-plus-1.7.1/setup.cfg
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2679 2024-04-07 10:39:21.000000 decoder-plus-plus-1.7.1/setup.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-07 18:16:03.734202 decoder-plus-plus-1.7.1/tests/
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1805 2023-01-15 14:31:34.000000 decoder-plus-plus-1.7.1/tests/__init__.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-07 18:16:03.754202 decoder-plus-plus-1.7.1/tests/plugins/
+-rw-rw-r--   0 tom       (1000) tom       (1000)        0 2022-11-01 13:33:59.000000 decoder-plus-plus-1.7.1/tests/plugins/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1113 2022-11-01 14:08:45.000000 decoder-plus-plus-1.7.1/tests/plugins/adler32_hasher_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1191 2022-11-01 18:50:27.000000 decoder-plus-plus-1.7.1/tests/plugins/apache_md5_hasher_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1295 2022-11-01 18:05:54.000000 decoder-plus-plus-1.7.1/tests/plugins/base16_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1680 2023-01-15 13:01:54.000000 decoder-plus-plus-1.7.1/tests/plugins/base32_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1287 2023-01-15 13:32:25.000000 decoder-plus-plus-1.7.1/tests/plugins/base45_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1288 2023-01-15 12:36:51.000000 decoder-plus-plus-1.7.1/tests/plugins/base64_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1474 2023-01-15 12:47:27.000000 decoder-plus-plus-1.7.1/tests/plugins/base64_url_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1229 2023-01-15 13:29:43.000000 decoder-plus-plus-1.7.1/tests/plugins/bin_int_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1040 2022-11-01 18:51:09.000000 decoder-plus-plus-1.7.1/tests/plugins/bin_str_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      992 2023-01-15 12:47:59.000000 decoder-plus-plus-1.7.1/tests/plugins/caesar_cipher_script_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1222 2022-11-01 18:35:38.000000 decoder-plus-plus-1.7.1/tests/plugins/clone_script_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1108 2023-01-15 12:37:31.000000 decoder-plus-plus-1.7.1/tests/plugins/crc32_hasher_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1183 2022-11-01 18:39:55.000000 decoder-plus-plus-1.7.1/tests/plugins/css_minify_script_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1401 2022-11-01 18:35:21.000000 decoder-plus-plus-1.7.1/tests/plugins/dec_str_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1245 2022-11-01 18:59:45.000000 decoder-plus-plus-1.7.1/tests/plugins/escape_string_script_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1123 2022-11-01 18:47:57.000000 decoder-plus-plus-1.7.1/tests/plugins/extract_urls_script_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1165 2022-11-01 18:40:22.000000 decoder-plus-plus-1.7.1/tests/plugins/filter_lines_script_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1189 2023-01-15 13:03:50.000000 decoder-plus-plus-1.7.1/tests/plugins/free_bsd_nt_hasher_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1253 2023-01-15 12:29:09.000000 decoder-plus-plus-1.7.1/tests/plugins/gzip_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1067 2022-11-01 18:47:18.000000 decoder-plus-plus-1.7.1/tests/plugins/hex_char_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1193 2023-01-15 13:10:42.000000 decoder-plus-plus-1.7.1/tests/plugins/hex_int_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1614 2022-11-01 18:43:06.000000 decoder-plus-plus-1.7.1/tests/plugins/hex_shell_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1313 2023-01-15 13:16:46.000000 decoder-plus-plus-1.7.1/tests/plugins/hex_str_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1173 2022-11-01 18:43:28.000000 decoder-plus-plus-1.7.1/tests/plugins/html_beautify_script_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1168 2022-11-01 18:48:47.000000 decoder-plus-plus-1.7.1/tests/plugins/html_minify_script_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1172 2023-01-15 12:22:31.000000 decoder-plus-plus-1.7.1/tests/plugins/html_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1219 2022-11-01 18:32:01.000000 decoder-plus-plus-1.7.1/tests/plugins/http64_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1016 2024-04-07 12:31:43.000000 decoder-plus-plus-1.7.1/tests/plugins/identify_file_type_filemagic_script_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1019 2024-04-07 12:32:46.000000 decoder-plus-plus-1.7.1/tests/plugins/identify_file_type_magika_script_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1108 2022-11-01 18:39:55.000000 decoder-plus-plus-1.7.1/tests/plugins/identify_hash_format_script_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1145 2023-01-15 13:26:35.000000 decoder-plus-plus-1.7.1/tests/plugins/jq_script_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      988 2023-01-15 12:41:00.000000 decoder-plus-plus-1.7.1/tests/plugins/js_beautify_script_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1164 2022-11-01 18:49:20.000000 decoder-plus-plus-1.7.1/tests/plugins/js_minify_script_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      977 2023-01-15 13:06:33.000000 decoder-plus-plus-1.7.1/tests/plugins/js_to_xml_script_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      981 2023-01-15 13:02:34.000000 decoder-plus-plus-1.7.1/tests/plugins/jsonify_script_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1163 2022-11-01 18:49:36.000000 decoder-plus-plus-1.7.1/tests/plugins/jsonpath_script_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      976 2023-01-15 12:39:55.000000 decoder-plus-plus-1.7.1/tests/plugins/jwt_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1163 2023-01-15 13:02:49.000000 decoder-plus-plus-1.7.1/tests/plugins/keccak224_hasher_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1171 2022-11-01 18:56:46.000000 decoder-plus-plus-1.7.1/tests/plugins/keccak256_hasher_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1203 2022-11-01 18:45:25.000000 decoder-plus-plus-1.7.1/tests/plugins/keccak384_hasher_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1235 2022-11-01 18:48:57.000000 decoder-plus-plus-1.7.1/tests/plugins/keccak512_hasher_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1245 2022-11-01 18:31:13.000000 decoder-plus-plus-1.7.1/tests/plugins/little_big_endian_script_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1124 2022-11-01 18:56:24.000000 decoder-plus-plus-1.7.1/tests/plugins/lm_hasher_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1126 2022-11-01 18:24:14.000000 decoder-plus-plus-1.7.1/tests/plugins/md2_hasher_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1126 2022-11-01 18:56:15.000000 decoder-plus-plus-1.7.1/tests/plugins/md4_hasher_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1126 2022-11-01 18:45:18.000000 decoder-plus-plus-1.7.1/tests/plugins/md5_hasher_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1124 2022-11-01 18:46:24.000000 decoder-plus-plus-1.7.1/tests/plugins/nt_hasher_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1193 2023-01-15 13:13:49.000000 decoder-plus-plus-1.7.1/tests/plugins/oct_int_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1405 2022-11-01 18:20:57.000000 decoder-plus-plus-1.7.1/tests/plugins/oct_str_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1181 2023-01-15 12:51:06.000000 decoder-plus-plus-1.7.1/tests/plugins/phpass_hasher_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1167 2022-11-01 18:57:07.000000 decoder-plus-plus-1.7.1/tests/plugins/reformat_text_script_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1187 2023-01-15 13:04:21.000000 decoder-plus-plus-1.7.1/tests/plugins/remove_newlines_script_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1064 2022-11-01 18:56:04.000000 decoder-plus-plus-1.7.1/tests/plugins/remove_whitespaces_script_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1146 2022-11-01 18:56:36.000000 decoder-plus-plus-1.7.1/tests/plugins/ripemd160_hasher_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1225 2022-11-01 18:26:44.000000 decoder-plus-plus-1.7.1/tests/plugins/rot13_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1503 2023-01-15 13:05:35.000000 decoder-plus-plus-1.7.1/tests/plugins/search_and_replace_script_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1136 2022-11-01 18:27:54.000000 decoder-plus-plus-1.7.1/tests/plugins/sha1_hasher_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1192 2022-11-01 18:29:14.000000 decoder-plus-plus-1.7.1/tests/plugins/sha224_hasher_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1200 2022-11-01 18:29:35.000000 decoder-plus-plus-1.7.1/tests/plugins/sha256_hasher_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1231 2022-11-01 18:29:59.000000 decoder-plus-plus-1.7.1/tests/plugins/sha384_hasher_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1160 2023-01-15 12:37:21.000000 decoder-plus-plus-1.7.1/tests/plugins/sha3_224_hasher_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1168 2022-11-01 18:53:45.000000 decoder-plus-plus-1.7.1/tests/plugins/sha3_256_hasher_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1200 2022-11-01 18:28:35.000000 decoder-plus-plus-1.7.1/tests/plugins/sha3_384_hasher_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1268 2022-11-01 18:28:57.000000 decoder-plus-plus-1.7.1/tests/plugins/sha3_512_hasher_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1263 2022-11-01 18:30:17.000000 decoder-plus-plus-1.7.1/tests/plugins/sha512_hasher_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1170 2022-11-01 18:57:46.000000 decoder-plus-plus-1.7.1/tests/plugins/split_and_rejoin_script_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      983 2023-01-15 12:39:55.000000 decoder-plus-plus-1.7.1/tests/plugins/sun_md5_hasher_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1247 2022-11-01 18:32:56.000000 decoder-plus-plus-1.7.1/tests/plugins/unescape_string_script_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1282 2022-11-01 18:45:08.000000 decoder-plus-plus-1.7.1/tests/plugins/url_plus_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1136 2022-11-01 18:53:35.000000 decoder-plus-plus-1.7.1/tests/plugins/url_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1136 2023-01-15 14:38:44.000000 decoder-plus-plus-1.7.1/tests/plugins/xpath_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1223 2023-01-15 13:12:30.000000 decoder-plus-plus-1.7.1/tests/plugins/zlib_test.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-07 18:16:03.754202 decoder-plus-plus-1.7.1/tests/ui/
+-rw-rw-r--   0 tom       (1000) tom       (1000)        0 2023-01-15 14:39:42.000000 decoder-plus-plus-1.7.1/tests/ui/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)    10085 2024-04-07 18:07:00.000000 decoder-plus-plus-1.7.1/tests/ui/classic_mode_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      512 2023-01-15 15:28:09.000000 decoder-plus-plus-1.7.1/tests/utils.py
```

### Comparing `decoder-plus-plus-1.7.0/LICENSE` & `decoder-plus-plus-1.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/PKG-INFO` & `decoder-plus-plus-1.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: decoder-plus-plus
-Version: 1.7.0
+Version: 1.7.1
 Summary: An extensible application for penetration testers and software developers to decode/encode data into various formats.
 Home-page: https://github.com/bytebutcher/decoder-plus-plus
 Author: bytebutcher
 Author-email: thomas.engel.web@gmail.com
 License: GPL-3.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: decoder-plus-plus Version: 1.7.0 Summary: An
+Metadata-Version: 2.1 Name: decoder-plus-plus Version: 1.7.1 Summary: An
 extensible application for penetration testers and software developers to
 decode/encode data into various formats. Home-page: https://github.com/
 bytebutcher/decoder-plus-plus Author: bytebutcher Author-email:
 thomas.engel.web@gmail.com License: GPL-3.0 Classifier: Programming Language ::
 Python :: 3 Classifier: Operating System :: OS Independent Description-Content-
 Type: text/markdown Provides-Extra: qt5 Provides-Extra: qt6 Provides-Extra:
 extras Provides-Extra: test License-File: LICENSE ![Decoder++ Logo](https://
```

### Comparing `decoder-plus-plus-1.7.0/README.md` & `decoder-plus-plus-1.7.1/README.md`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/data/dpp.png` & `decoder-plus-plus-1.7.1/data/dpp.png`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/decoder_plus_plus.egg-info/PKG-INFO` & `decoder-plus-plus-1.7.1/decoder_plus_plus.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: decoder-plus-plus
-Version: 1.7.0
+Version: 1.7.1
 Summary: An extensible application for penetration testers and software developers to decode/encode data into various formats.
 Home-page: https://github.com/bytebutcher/decoder-plus-plus
 Author: bytebutcher
 Author-email: thomas.engel.web@gmail.com
 License: GPL-3.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: decoder-plus-plus Version: 1.7.0 Summary: An
+Metadata-Version: 2.1 Name: decoder-plus-plus Version: 1.7.1 Summary: An
 extensible application for penetration testers and software developers to
 decode/encode data into various formats. Home-page: https://github.com/
 bytebutcher/decoder-plus-plus Author: bytebutcher Author-email:
 thomas.engel.web@gmail.com License: GPL-3.0 Classifier: Programming Language ::
 Python :: 3 Classifier: Operating System :: OS Independent Description-Content-
 Type: text/markdown Provides-Extra: qt5 Provides-Extra: qt6 Provides-Extra:
 extras Provides-Extra: test License-File: LICENSE ![Decoder++ Logo](https://
```

### Comparing `decoder-plus-plus-1.7.0/decoder_plus_plus.egg-info/SOURCES.txt` & `decoder-plus-plus-1.7.1/decoder_plus_plus.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -234,15 +234,16 @@
 tests/plugins/hex_int_test.py
 tests/plugins/hex_shell_test.py
 tests/plugins/hex_str_test.py
 tests/plugins/html_beautify_script_test.py
 tests/plugins/html_minify_script_test.py
 tests/plugins/html_test.py
 tests/plugins/http64_test.py
-tests/plugins/identify_file_type_script_test.py
+tests/plugins/identify_file_type_filemagic_script_test.py
+tests/plugins/identify_file_type_magika_script_test.py
 tests/plugins/identify_hash_format_script_test.py
 tests/plugins/jq_script_test.py
 tests/plugins/js_beautify_script_test.py
 tests/plugins/js_minify_script_test.py
 tests/plugins/js_to_xml_script_test.py
 tests/plugins/jsonify_script_test.py
 tests/plugins/jsonpath_script_test.py
```

### Comparing `decoder-plus-plus-1.7.0/dpp/__init__.py` & `decoder-plus-plus-1.7.1/dpp/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,12 +12,12 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 __name__ = 'decoder-plus-plus'
-__version__ = '1.7.0'
+__version__ = '1.7.1'
 __author__ = 'bytebutcher'
 
 import os
 app_path = os.path.dirname(os.path.abspath(__file__))
```

### Comparing `decoder-plus-plus-1.7.0/dpp/core/__init__.py` & `decoder-plus-plus-1.7.1/dpp/core/__init__.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/core/argparse.py` & `decoder-plus-plus-1.7.1/dpp/core/argparse.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/core/assertions.py` & `decoder-plus-plus-1.7.1/dpp/core/assertions.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/core/config.py` & `decoder-plus-plus-1.7.1/dpp/core/config.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/core/context.py` & `decoder-plus-plus-1.7.1/dpp/core/context.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/core/decoder_plus_plus.py` & `decoder-plus-plus-1.7.1/dpp/core/decoder_plus_plus.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/core/exceptions.py` & `decoder-plus-plus-1.7.1/dpp/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/core/icons.py` & `decoder-plus-plus-1.7.1/dpp/core/icons.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/core/listener.py` & `decoder-plus-plus-1.7.1/dpp/core/listener.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/core/logger.py` & `decoder-plus-plus-1.7.1/dpp/core/logger.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/core/math.py` & `decoder-plus-plus-1.7.1/dpp/core/math.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/core/plugin/__init__.py` & `decoder-plus-plus-1.7.1/dpp/core/plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/core/plugin/builder.py` & `decoder-plus-plus-1.7.1/dpp/core/plugin/builder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/core/plugin/config/__init__.py` & `decoder-plus-plus-1.7.1/dpp/core/plugin/config/__init__.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/core/plugin/config/options/__init__.py` & `decoder-plus-plus-1.7.1/dpp/core/plugin/config/options/__init__.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/core/plugin/config/ui/__init__.py` & `decoder-plus-plus-1.7.1/dpp/core/plugin/config/ui/__init__.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/core/plugin/config/ui/layouts.py` & `decoder-plus-plus-1.7.1/dpp/core/plugin/config/ui/layouts.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/core/plugin/config/ui/widgets.py` & `decoder-plus-plus-1.7.1/dpp/core/plugin/config/ui/widgets.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/core/plugin/loader.py` & `decoder-plus-plus-1.7.1/dpp/core/plugin/loader.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/core/plugin/manager.py` & `decoder-plus-plus-1.7.1/dpp/core/plugin/manager.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/core/shortcuts.py` & `decoder-plus-plus-1.7.1/dpp/core/shortcuts.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/images/dpp.png` & `decoder-plus-plus-1.7.1/dpp/images/dpp.png`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/images/dpp_128.png` & `decoder-plus-plus-1.7.1/dpp/images/dpp_128.png`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/images/dpp_classic.png` & `decoder-plus-plus-1.7.1/dpp/images/dpp_classic.png`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/images/dpp_classic_128.png` & `decoder-plus-plus-1.7.1/dpp/images/dpp_classic_128.png`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/images/dpp_modern.png` & `decoder-plus-plus-1.7.1/dpp/images/dpp_modern.png`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/images/dpp_modern_128.png` & `decoder-plus-plus-1.7.1/dpp/images/dpp_modern_128.png`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/images/dpp_modern_big.png` & `decoder-plus-plus-1.7.1/dpp/images/dpp_modern_big.png`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/images/dpp_stylized.png` & `decoder-plus-plus-1.7.1/dpp/images/dpp_stylized.png`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/images/dpp_stylized_128.png` & `decoder-plus-plus-1.7.1/dpp/images/dpp_stylized_128.png`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/images/dpp_xmas.png` & `decoder-plus-plus-1.7.1/dpp/images/dpp_xmas.png`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/images/dpp_xmas_stylized.png` & `decoder-plus-plus-1.7.1/dpp/images/dpp_xmas_stylized.png`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/images/keyboard.png` & `decoder-plus-plus-1.7.1/dpp/images/keyboard.png`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/images/keyboard.svg` & `decoder-plus-plus-1.7.1/dpp/images/keyboard.svg`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/plugins/adler32_hasher.py` & `decoder-plus-plus-1.7.1/dpp/plugins/adler32_hasher.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/plugins/apache_md5_hasher.py` & `decoder-plus-plus-1.7.1/dpp/plugins/apache_md5_hasher.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/plugins/base16_decoder.py` & `decoder-plus-plus-1.7.1/dpp/plugins/base16_decoder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/plugins/base16_encoder.py` & `decoder-plus-plus-1.7.1/dpp/plugins/base16_encoder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/plugins/base32_decoder.py` & `decoder-plus-plus-1.7.1/dpp/plugins/base32_decoder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/plugins/base32_encoder.py` & `decoder-plus-plus-1.7.1/dpp/plugins/base32_encoder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/plugins/base45_decoder.py` & `decoder-plus-plus-1.7.1/dpp/plugins/base45_decoder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/plugins/base45_encoder.py` & `decoder-plus-plus-1.7.1/dpp/plugins/base45_encoder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/plugins/base64_decoder.py` & `decoder-plus-plus-1.7.1/dpp/plugins/base64_decoder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/plugins/base64_encoder.py` & `decoder-plus-plus-1.7.1/dpp/plugins/base64_encoder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/plugins/base64_url_decoder.py` & `decoder-plus-plus-1.7.1/dpp/plugins/base64_url_decoder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/plugins/base64_url_encoder.py` & `decoder-plus-plus-1.7.1/dpp/plugins/base64_url_encoder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/plugins/bin_int_decoder.py` & `decoder-plus-plus-1.7.1/dpp/plugins/bin_int_decoder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/plugins/bin_int_encoder.py` & `decoder-plus-plus-1.7.1/dpp/plugins/bin_int_encoder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/plugins/bin_str_decoder.py` & `decoder-plus-plus-1.7.1/dpp/plugins/bin_str_decoder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/plugins/bin_str_encoder.py` & `decoder-plus-plus-1.7.1/dpp/plugins/bin_str_encoder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/plugins/caesar_cipher_script.py` & `decoder-plus-plus-1.7.1/dpp/plugins/caesar_cipher_script.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/plugins/clone_script.py` & `decoder-plus-plus-1.7.1/dpp/plugins/clone_script.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/plugins/crc32_hasher.py` & `decoder-plus-plus-1.7.1/dpp/plugins/crc32_hasher.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/plugins/css_minify_script.py` & `decoder-plus-plus-1.7.1/dpp/plugins/css_minify_script.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/plugins/custom_code.py` & `decoder-plus-plus-1.7.1/dpp/plugins/custom_code.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/plugins/dec_str_decoder.py` & `decoder-plus-plus-1.7.1/dpp/plugins/dec_str_decoder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/plugins/dec_str_encoder.py` & `decoder-plus-plus-1.7.1/dpp/plugins/dec_str_encoder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/plugins/escape_string_script.py` & `decoder-plus-plus-1.7.1/dpp/plugins/escape_string_script.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/plugins/extract_urls_script.py` & `decoder-plus-plus-1.7.1/dpp/plugins/extract_urls_script.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/plugins/filter_lines_script.py` & `decoder-plus-plus-1.7.1/dpp/plugins/filter_lines_script.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/plugins/free_bsd_nt_hasher.py` & `decoder-plus-plus-1.7.1/dpp/plugins/free_bsd_nt_hasher.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/plugins/gzip_decoder.py` & `decoder-plus-plus-1.7.1/dpp/plugins/gzip_decoder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/plugins/gzip_encoder.py` & `decoder-plus-plus-1.7.1/dpp/plugins/gzip_encoder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/plugins/hex_char_decoder.py` & `decoder-plus-plus-1.7.1/dpp/plugins/hex_char_decoder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/plugins/hex_char_encoder.py` & `decoder-plus-plus-1.7.1/dpp/plugins/hex_char_encoder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/plugins/hex_int_decoder.py` & `decoder-plus-plus-1.7.1/dpp/plugins/hex_int_decoder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/plugins/hex_int_encoder.py` & `decoder-plus-plus-1.7.1/dpp/plugins/hex_int_encoder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/plugins/hex_shell_decoder.py` & `decoder-plus-plus-1.7.1/dpp/plugins/hex_shell_decoder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/plugins/hex_shell_encoder.py` & `decoder-plus-plus-1.7.1/dpp/plugins/hex_shell_encoder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/plugins/hex_str_decoder.py` & `decoder-plus-plus-1.7.1/dpp/plugins/hex_str_decoder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/plugins/hex_str_encoder.py` & `decoder-plus-plus-1.7.1/dpp/plugins/hex_str_encoder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/plugins/html_beautify_script.py` & `decoder-plus-plus-1.7.1/dpp/plugins/html_beautify_script.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/plugins/html_decoder.py` & `decoder-plus-plus-1.7.1/dpp/plugins/html_decoder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/plugins/html_encoder.py` & `decoder-plus-plus-1.7.1/dpp/plugins/html_encoder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/plugins/html_minify_script.py` & `decoder-plus-plus-1.7.1/dpp/plugins/html_minify_script.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/plugins/http64_decoder.py` & `decoder-plus-plus-1.7.1/dpp/plugins/http64_decoder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/plugins/http64_encoder.py` & `decoder-plus-plus-1.7.1/dpp/plugins/http64_encoder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/plugins/identify_decoder_script.py` & `decoder-plus-plus-1.7.1/dpp/plugins/identify_decoder_script.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/plugins/identify_file_type_filemagic_script.py` & `decoder-plus-plus-1.7.1/dpp/plugins/identify_file_type_filemagic_script.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/plugins/identify_file_type_magika_script.py` & `decoder-plus-plus-1.7.1/dpp/plugins/identify_file_type_magika_script.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/plugins/identify_hash_format_script.py` & `decoder-plus-plus-1.7.1/dpp/plugins/identify_hash_format_script.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/plugins/jq_script.py` & `decoder-plus-plus-1.7.1/dpp/plugins/jq_script.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/plugins/js_beautify_script.py` & `decoder-plus-plus-1.7.1/dpp/plugins/js_beautify_script.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/plugins/js_minify_script.py` & `decoder-plus-plus-1.7.1/dpp/plugins/js_minify_script.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/plugins/js_to_xml_script.py` & `decoder-plus-plus-1.7.1/dpp/plugins/js_to_xml_script.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/plugins/jsonify_script.py` & `decoder-plus-plus-1.7.1/dpp/plugins/jsonify_script.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/plugins/jsonpath_script.py` & `decoder-plus-plus-1.7.1/dpp/plugins/jsonpath_script.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/plugins/jwt_decoder.py` & `decoder-plus-plus-1.7.1/dpp/plugins/jwt_decoder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/plugins/keccak224_hasher.py` & `decoder-plus-plus-1.7.1/dpp/plugins/keccak224_hasher.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/plugins/keccak256_hasher.py` & `decoder-plus-plus-1.7.1/dpp/plugins/keccak256_hasher.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/plugins/keccak384_hasher.py` & `decoder-plus-plus-1.7.1/dpp/plugins/keccak384_hasher.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/plugins/keccak512_hasher.py` & `decoder-plus-plus-1.7.1/dpp/plugins/keccak512_hasher.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/plugins/little_big_endian_script.py` & `decoder-plus-plus-1.7.1/dpp/plugins/little_big_endian_script.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/plugins/lm_hasher.py` & `decoder-plus-plus-1.7.1/dpp/plugins/lm_hasher.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/plugins/md2_hasher.py` & `decoder-plus-plus-1.7.1/dpp/plugins/md2_hasher.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/plugins/md4_hasher.py` & `decoder-plus-plus-1.7.1/dpp/plugins/md4_hasher.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/plugins/md5_hasher.py` & `decoder-plus-plus-1.7.1/dpp/plugins/md5_hasher.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/plugins/nt_hasher.py` & `decoder-plus-plus-1.7.1/dpp/plugins/nt_hasher.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/plugins/oct_int_decoder.py` & `decoder-plus-plus-1.7.1/dpp/plugins/oct_int_decoder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/plugins/oct_int_encoder.py` & `decoder-plus-plus-1.7.1/dpp/plugins/oct_int_encoder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/plugins/oct_str_decoder.py` & `decoder-plus-plus-1.7.1/dpp/plugins/oct_str_decoder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/plugins/oct_str_encoder.py` & `decoder-plus-plus-1.7.1/dpp/plugins/oct_str_encoder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/plugins/phpass_hasher.py` & `decoder-plus-plus-1.7.1/dpp/plugins/phpass_hasher.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/plugins/reformat_text_script.py` & `decoder-plus-plus-1.7.1/dpp/plugins/reformat_text_script.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/plugins/remove_newlines_script.py` & `decoder-plus-plus-1.7.1/dpp/plugins/remove_newlines_script.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/plugins/remove_whitespaces_script.py` & `decoder-plus-plus-1.7.1/dpp/plugins/remove_whitespaces_script.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/plugins/ripemd160_hasher.py` & `decoder-plus-plus-1.7.1/dpp/plugins/ripemd160_hasher.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/plugins/rot13_decoder.py` & `decoder-plus-plus-1.7.1/dpp/plugins/rot13_decoder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/plugins/rot13_encoder.py` & `decoder-plus-plus-1.7.1/dpp/plugins/rot13_encoder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/plugins/search_and_replace_script.py` & `decoder-plus-plus-1.7.1/dpp/plugins/search_and_replace_script.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/plugins/sha1_hasher.py` & `decoder-plus-plus-1.7.1/dpp/plugins/sha1_hasher.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/plugins/sha224_hasher.py` & `decoder-plus-plus-1.7.1/dpp/plugins/sha224_hasher.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/plugins/sha256_hasher.py` & `decoder-plus-plus-1.7.1/dpp/plugins/sha256_hasher.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/plugins/sha384_hasher.py` & `decoder-plus-plus-1.7.1/dpp/plugins/sha384_hasher.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/plugins/sha3_224_hasher.py` & `decoder-plus-plus-1.7.1/dpp/plugins/sha3_224_hasher.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/plugins/sha3_256_hasher.py` & `decoder-plus-plus-1.7.1/dpp/plugins/sha3_256_hasher.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/plugins/sha3_384_hasher.py` & `decoder-plus-plus-1.7.1/dpp/plugins/sha3_384_hasher.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/plugins/sha3_512_hasher.py` & `decoder-plus-plus-1.7.1/dpp/plugins/sha3_512_hasher.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/plugins/sha512_hasher.py` & `decoder-plus-plus-1.7.1/dpp/plugins/sha512_hasher.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/plugins/split_and_rejoin_script.py` & `decoder-plus-plus-1.7.1/dpp/plugins/split_and_rejoin_script.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/plugins/sun_md5_hasher.py` & `decoder-plus-plus-1.7.1/dpp/plugins/sun_md5_hasher.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/plugins/unescape_string_script.py` & `decoder-plus-plus-1.7.1/dpp/plugins/unescape_string_script.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/plugins/url_decoder.py` & `decoder-plus-plus-1.7.1/dpp/plugins/url_decoder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/plugins/url_encoder.py` & `decoder-plus-plus-1.7.1/dpp/plugins/url_encoder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/plugins/url_plus_decoder.py` & `decoder-plus-plus-1.7.1/dpp/plugins/url_plus_decoder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/plugins/url_plus_encoder.py` & `decoder-plus-plus-1.7.1/dpp/plugins/url_plus_encoder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/plugins/xpath_script.py` & `decoder-plus-plus-1.7.1/dpp/plugins/xpath_script.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/plugins/zlib_decoder.py` & `decoder-plus-plus-1.7.1/dpp/plugins/zlib_decoder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/plugins/zlib_encoder.py` & `decoder-plus-plus-1.7.1/dpp/plugins/zlib_encoder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/runner.py` & `decoder-plus-plus-1.7.1/dpp/runner.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/ui/__init__.py` & `decoder-plus-plus-1.7.1/dpp/ui/__init__.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/ui/builder/action_builder.py` & `decoder-plus-plus-1.7.1/dpp/ui/builder/action_builder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/ui/builder/input_text_builder.py` & `decoder-plus-plus-1.7.1/dpp/ui/builder/input_text_builder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/ui/builder/plugin_config_widget_builder.py` & `decoder-plus-plus-1.7.1/dpp/ui/builder/plugin_config_widget_builder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/ui/builder/widget_builder.py` & `decoder-plus-plus-1.7.1/dpp/ui/builder/widget_builder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/ui/decoder_plus_plus_gui.py` & `decoder-plus-plus-1.7.1/dpp/ui/decoder_plus_plus_gui.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/ui/dialog/__init__.py` & `decoder-plus-plus-1.7.1/dpp/ui/dialog/__init__.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/ui/dialog/config_dialog.py` & `decoder-plus-plus-1.7.1/dpp/ui/dialog/config_dialog.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/ui/dialog/keyboard_shortcut_dialog.py` & `decoder-plus-plus-1.7.1/dpp/ui/dialog/keyboard_shortcut_dialog.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/ui/dialog/plugin_config_dialog.py` & `decoder-plus-plus-1.7.1/dpp/ui/dialog/plugin_config_dialog.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/ui/dock/hex_dock.py` & `decoder-plus-plus-1.7.1/dpp/ui/dock/hex_dock.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/ui/dock/log_dock.py` & `decoder-plus-plus-1.7.1/dpp/ui/dock/log_dock.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/ui/instance_handler.py` & `decoder-plus-plus-1.7.1/dpp/ui/instance_handler.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/ui/view/__init__.py` & `decoder-plus-plus-1.7.1/dpp/ui/view/__init__.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/ui/view/classic/__init__.py` & `decoder-plus-plus-1.7.1/dpp/ui/view/classic/__init__.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/ui/view/classic/classic_main_window_widget.py` & `decoder-plus-plus-1.7.1/dpp/ui/view/classic/classic_main_window_widget.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/ui/view/classic/codec_frame.py` & `decoder-plus-plus-1.7.1/dpp/ui/view/classic/codec_frame.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/ui/view/classic/codec_frame_header.py` & `decoder-plus-plus-1.7.1/dpp/ui/view/classic/codec_frame_header.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/ui/view/classic/codec_frames.py` & `decoder-plus-plus-1.7.1/dpp/ui/view/classic/codec_frames.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,15 +111,17 @@
         return self.newFrame(output, plugin.title, new_frame_index, status=status, msg=error)
 
     @logmethod()
     def _update_frames(self, frame_id, is_user_action=True, do_preserve_state=False):
         """
         Updates all frames starting from the given frame_id.
         @param frame_id: the frame id to start updating from.
-        @param is_user_action: defines whether the update is triggered by a user action or not.
+        @param is_user_action: defines whether the update was triggered by a user action.
+                               If True, the method marks the starting frame with a "DEFAULT" status to denote
+                               that the user has modified the input. Defaults to True.
         @param do_preserve_state: defines whether the state of the frame should be preserved or not.
         """
         frame_index = self.getFrameIndex(frame_id)
         frame = self.getFrameById(frame_id)
         if is_user_action:
             frame.setStatus(StatusWidget.DEFAULT, '')
         while frame:
@@ -182,27 +184,29 @@
     def _on_plugin_selected(self, frame_id: str, plugin: AbstractPlugin):
         if plugin:
             frame = self.getFrameById(frame_id)
             if not self._configure_plugin(frame_id, frame.getInputText(), plugin):
                 # Abort if user cancels configuration.
                 return
 
-            if frame.getFrameIndex() > 0 and not frame.hasNextFrame():
-                # Auto-collapse when current frame is last frame (except if current frame is the first frame).
+            # Do only auto-collapse, when we are creating a new frame. But never auto-collapse the first frame.
+            if frame.getFrameIndex() == self.getFramesCount() - 1 and frame.getFrameIndex() > 0:
                 frame.setCollapsed(True)
 
-            # TODO: #53 Allow multiple codecs on input
-            #       Computation should be done within in the frame.
-            #       (Old) frames store information how input is processed.
-            frame = self._new_frame(frame)
-
-            # Focus the input text of the newly created frame.
-            # If frame already existed make sure it is not collapsed.
-            frame.setCollapsed(False)
-            frame.focusInputText()
+            # Iteratively execute codecs starting with the current frame and continuing to the last frame,
+            # stopping if any codec encounters a failure.
+            self._update_frames(frame.id(), is_user_action=False)
+
+            # Focus input text of next frame which is not collapsed.
+            next_frame = frame
+            while next_frame.hasNextFrame():
+                next_frame: CodecFrame = next_frame.getNextFrame()
+                if not next_frame.isCollapsed():
+                    next_frame.focusInputText()
+                    break
         else:
             self._deselect_plugin(frame_id)
 
     @logmethod()
     def _on_frame_close_button_clicked(self, frame_id):
         """ Closes/Removes the frame with the specified frame-id. """
         _frame_index = self.getFrameIndex(frame_id)
@@ -399,16 +403,17 @@
                 self._context.listener().textSelectionChanged.emit(tab_id, frame_id, input_text)
 
         new_frame.textSelectionChanged.connect(on_text_selection_changed)
 
         def selected_frame_changed(tab_id, frame_id, input_text):
             # Always remember the currently focused frame (e.g. used for finding the currently selected frame when
             # using keyboard-shortcuts)
-            self._focused_frame = self.getFrameById(frame_id)
-            self._context.listener().selectedFrameChanged.emit(tab_id, frame_id, input_text)
+            if self._tab_id == tab_id:
+                self._focused_frame = self.getFrameById(frame_id)
+                self._context.listener().selectedFrameChanged.emit(tab_id, frame_id, input_text)
 
         new_frame.selectedFrameChanged.connect(selected_frame_changed)
 
         def textChanged(tab_id, frame_id, text):
             if self._tab_id == tab_id:
                 self._update_frames(frame_id)
                 self._context.listener().textChanged.emit(tab_id, frame_id, text)
```

### Comparing `decoder-plus-plus-1.7.0/dpp/ui/view/classic/codec_tab.py` & `decoder-plus-plus-1.7.1/dpp/ui/view/classic/codec_tab.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/ui/view/classic/combo_box_frame.py` & `decoder-plus-plus-1.7.1/dpp/ui/view/classic/combo_box_frame.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/ui/view/main_window_widget.py` & `decoder-plus-plus-1.7.1/dpp/ui/view/main_window_widget.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/ui/view/modern/__init__.py` & `decoder-plus-plus-1.7.1/dpp/ui/view/modern/__init__.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/ui/view/modern/modern_main_window_widget.py` & `decoder-plus-plus-1.7.1/dpp/ui/view/modern/modern_main_window_widget.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/ui/view/modern/node_data.py` & `decoder-plus-plus-1.7.1/dpp/ui/view/modern/node_data.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/ui/view/modern/node_data_models.py` & `decoder-plus-plus-1.7.1/dpp/ui/view/modern/node_data_models.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/ui/view/modern/node_editor.py` & `decoder-plus-plus-1.7.1/dpp/ui/view/modern/node_editor.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/ui/view/modern/node_editor_tab.py` & `decoder-plus-plus-1.7.1/dpp/ui/view/modern/node_editor_tab.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/ui/widget/__init__.py` & `decoder-plus-plus-1.7.1/dpp/ui/widget/__init__.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/ui/widget/clickable_label.py` & `decoder-plus-plus-1.7.1/dpp/ui/widget/clickable_label.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/ui/widget/code_editor_widget.py` & `decoder-plus-plus-1.7.1/dpp/ui/widget/code_editor_widget.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/ui/widget/codec_preview_widget.py` & `decoder-plus-plus-1.7.1/dpp/ui/widget/codec_preview_widget.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/ui/widget/collapsible_frame.py` & `decoder-plus-plus-1.7.1/dpp/ui/widget/collapsible_frame.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/ui/widget/combo_box.py` & `decoder-plus-plus-1.7.1/dpp/ui/widget/combo_box.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/ui/widget/dock_tabs_widget.py` & `decoder-plus-plus-1.7.1/dpp/ui/widget/dock_tabs_widget.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/ui/widget/dock_widget.py` & `decoder-plus-plus-1.7.1/dpp/ui/widget/dock_widget.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/ui/widget/dyna_frame.py` & `decoder-plus-plus-1.7.1/dpp/ui/widget/dyna_frame.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/ui/widget/elided_label.py` & `decoder-plus-plus-1.7.1/dpp/ui/widget/elided_label.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/ui/widget/hover_label.py` & `decoder-plus-plus-1.7.1/dpp/ui/widget/hover_label.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/ui/widget/icon_label.py` & `decoder-plus-plus-1.7.1/dpp/ui/widget/icon_label.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/ui/widget/identify_format_button.py` & `decoder-plus-plus-1.7.1/dpp/ui/widget/identify_format_button.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/ui/widget/list_widget.py` & `decoder-plus-plus-1.7.1/dpp/ui/widget/list_widget.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/ui/widget/menu_bar.py` & `decoder-plus-plus-1.7.1/dpp/ui/widget/menu_bar.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/ui/widget/message_box_widget.py` & `decoder-plus-plus-1.7.1/dpp/ui/widget/message_box_widget.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/ui/widget/message_widget.py` & `decoder-plus-plus-1.7.1/dpp/ui/widget/message_widget.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/ui/widget/option_widgets.py` & `decoder-plus-plus-1.7.1/dpp/ui/widget/option_widgets.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/ui/widget/plain_view.py` & `decoder-plus-plus-1.7.1/dpp/ui/widget/plain_view.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/ui/widget/plugin_frame.py` & `decoder-plus-plus-1.7.1/dpp/ui/widget/plugin_frame.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/ui/widget/plugin_tab.py` & `decoder-plus-plus-1.7.1/dpp/ui/widget/plugin_tab.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/ui/widget/search_field.py` & `decoder-plus-plus-1.7.1/dpp/ui/widget/search_field.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/ui/widget/separater_widget.py` & `decoder-plus-plus-1.7.1/dpp/ui/widget/separater_widget.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/ui/widget/shortcut_table.py` & `decoder-plus-plus-1.7.1/dpp/ui/widget/shortcut_table.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/ui/widget/slider_widget.py` & `decoder-plus-plus-1.7.1/dpp/ui/widget/slider_widget.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/ui/widget/smart_decode_button.py` & `decoder-plus-plus-1.7.1/dpp/ui/widget/smart_decode_button.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/ui/widget/spacers.py` & `decoder-plus-plus-1.7.1/dpp/ui/widget/spacers.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/ui/widget/status_widget.py` & `decoder-plus-plus-1.7.1/dpp/ui/widget/status_widget.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/ui/widget/tab_bar.py` & `decoder-plus-plus-1.7.1/dpp/ui/widget/tab_bar.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/ui/widget/tabs_widget.py` & `decoder-plus-plus-1.7.1/dpp/ui/widget/tabs_widget.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/dpp/ui/widget/text_widget.py` & `decoder-plus-plus-1.7.1/dpp/ui/widget/text_widget.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/setup.py` & `decoder-plus-plus-1.7.1/setup.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/tests/__init__.py` & `decoder-plus-plus-1.7.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/tests/plugins/adler32_hasher_test.py` & `decoder-plus-plus-1.7.1/tests/plugins/adler32_hasher_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/tests/plugins/apache_md5_hasher_test.py` & `decoder-plus-plus-1.7.1/tests/plugins/apache_md5_hasher_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/tests/plugins/base16_test.py` & `decoder-plus-plus-1.7.1/tests/plugins/base16_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/tests/plugins/base32_test.py` & `decoder-plus-plus-1.7.1/tests/plugins/base32_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/tests/plugins/base45_test.py` & `decoder-plus-plus-1.7.1/tests/plugins/base45_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/tests/plugins/base64_test.py` & `decoder-plus-plus-1.7.1/tests/plugins/base64_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/tests/plugins/base64_url_test.py` & `decoder-plus-plus-1.7.1/tests/plugins/base64_url_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/tests/plugins/bin_int_test.py` & `decoder-plus-plus-1.7.1/tests/plugins/bin_int_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/tests/plugins/bin_str_test.py` & `decoder-plus-plus-1.7.1/tests/plugins/bin_str_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/tests/plugins/caesar_cipher_script_test.py` & `decoder-plus-plus-1.7.1/tests/plugins/caesar_cipher_script_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/tests/plugins/clone_script_test.py` & `decoder-plus-plus-1.7.1/tests/plugins/clone_script_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/tests/plugins/crc32_hasher_test.py` & `decoder-plus-plus-1.7.1/tests/plugins/crc32_hasher_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/tests/plugins/css_minify_script_test.py` & `decoder-plus-plus-1.7.1/tests/plugins/css_minify_script_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/tests/plugins/dec_str_test.py` & `decoder-plus-plus-1.7.1/tests/plugins/dec_str_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/tests/plugins/escape_string_script_test.py` & `decoder-plus-plus-1.7.1/tests/plugins/escape_string_script_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/tests/plugins/extract_urls_script_test.py` & `decoder-plus-plus-1.7.1/tests/plugins/extract_urls_script_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/tests/plugins/filter_lines_script_test.py` & `decoder-plus-plus-1.7.1/tests/plugins/filter_lines_script_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/tests/plugins/free_bsd_nt_hasher_test.py` & `decoder-plus-plus-1.7.1/tests/plugins/free_bsd_nt_hasher_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/tests/plugins/gzip_test.py` & `decoder-plus-plus-1.7.1/tests/plugins/gzip_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/tests/plugins/hex_char_test.py` & `decoder-plus-plus-1.7.1/tests/plugins/hex_char_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/tests/plugins/hex_int_test.py` & `decoder-plus-plus-1.7.1/tests/plugins/hex_int_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/tests/plugins/hex_shell_test.py` & `decoder-plus-plus-1.7.1/tests/plugins/hex_shell_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/tests/plugins/hex_str_test.py` & `decoder-plus-plus-1.7.1/tests/plugins/hex_str_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/tests/plugins/html_beautify_script_test.py` & `decoder-plus-plus-1.7.1/tests/plugins/html_beautify_script_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/tests/plugins/html_minify_script_test.py` & `decoder-plus-plus-1.7.1/tests/plugins/html_minify_script_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/tests/plugins/html_test.py` & `decoder-plus-plus-1.7.1/tests/plugins/html_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/tests/plugins/http64_test.py` & `decoder-plus-plus-1.7.1/tests/plugins/http64_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/tests/plugins/identify_file_type_script_test.py` & `decoder-plus-plus-1.7.1/tests/plugins/identify_file_type_filemagic_script_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,12 +18,12 @@
 
 from dpp.core.plugin import PluginType
 from tests.utils import load_plugin
 
 
 class TestIdentifyFileTypeScript(unittest.TestCase):
 
-    plugin = load_plugin("Identify File Type", PluginType.IDENTIFY)
+    plugin = load_plugin("Identify File Type (filemagic)", PluginType.IDENTIFY)
 
     @unittest.skip("Missing configuration")
     def testPlugin(self):
         ...
```

### Comparing `decoder-plus-plus-1.7.0/tests/plugins/identify_hash_format_script_test.py` & `decoder-plus-plus-1.7.1/tests/plugins/identify_hash_format_script_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/tests/plugins/jq_script_test.py` & `decoder-plus-plus-1.7.1/tests/plugins/jq_script_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/tests/plugins/js_beautify_script_test.py` & `decoder-plus-plus-1.7.1/tests/plugins/js_beautify_script_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/tests/plugins/js_minify_script_test.py` & `decoder-plus-plus-1.7.1/tests/plugins/js_minify_script_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/tests/plugins/js_to_xml_script_test.py` & `decoder-plus-plus-1.7.1/tests/plugins/js_to_xml_script_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/tests/plugins/jsonify_script_test.py` & `decoder-plus-plus-1.7.1/tests/plugins/jsonify_script_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/tests/plugins/jsonpath_script_test.py` & `decoder-plus-plus-1.7.1/tests/plugins/jsonpath_script_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/tests/plugins/jwt_test.py` & `decoder-plus-plus-1.7.1/tests/plugins/jwt_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/tests/plugins/keccak224_hasher_test.py` & `decoder-plus-plus-1.7.1/tests/plugins/keccak224_hasher_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/tests/plugins/keccak256_hasher_test.py` & `decoder-plus-plus-1.7.1/tests/plugins/keccak256_hasher_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/tests/plugins/keccak384_hasher_test.py` & `decoder-plus-plus-1.7.1/tests/plugins/keccak384_hasher_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/tests/plugins/keccak512_hasher_test.py` & `decoder-plus-plus-1.7.1/tests/plugins/keccak512_hasher_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/tests/plugins/little_big_endian_script_test.py` & `decoder-plus-plus-1.7.1/tests/plugins/little_big_endian_script_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/tests/plugins/lm_hasher_test.py` & `decoder-plus-plus-1.7.1/tests/plugins/lm_hasher_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/tests/plugins/md2_hasher_test.py` & `decoder-plus-plus-1.7.1/tests/plugins/md2_hasher_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/tests/plugins/md4_hasher_test.py` & `decoder-plus-plus-1.7.1/tests/plugins/md4_hasher_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/tests/plugins/md5_hasher_test.py` & `decoder-plus-plus-1.7.1/tests/plugins/md5_hasher_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/tests/plugins/nt_hasher_test.py` & `decoder-plus-plus-1.7.1/tests/plugins/nt_hasher_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/tests/plugins/oct_int_test.py` & `decoder-plus-plus-1.7.1/tests/plugins/oct_int_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/tests/plugins/oct_str_test.py` & `decoder-plus-plus-1.7.1/tests/plugins/oct_str_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/tests/plugins/phpass_hasher_test.py` & `decoder-plus-plus-1.7.1/tests/plugins/phpass_hasher_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/tests/plugins/reformat_text_script_test.py` & `decoder-plus-plus-1.7.1/tests/plugins/reformat_text_script_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/tests/plugins/remove_newlines_script_test.py` & `decoder-plus-plus-1.7.1/tests/plugins/remove_newlines_script_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/tests/plugins/remove_whitespaces_script_test.py` & `decoder-plus-plus-1.7.1/tests/plugins/remove_whitespaces_script_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/tests/plugins/ripemd160_hasher_test.py` & `decoder-plus-plus-1.7.1/tests/plugins/ripemd160_hasher_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/tests/plugins/rot13_test.py` & `decoder-plus-plus-1.7.1/tests/plugins/rot13_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/tests/plugins/search_and_replace_script_test.py` & `decoder-plus-plus-1.7.1/tests/plugins/search_and_replace_script_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/tests/plugins/sha1_hasher_test.py` & `decoder-plus-plus-1.7.1/tests/plugins/sha1_hasher_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/tests/plugins/sha224_hasher_test.py` & `decoder-plus-plus-1.7.1/tests/plugins/sha224_hasher_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/tests/plugins/sha256_hasher_test.py` & `decoder-plus-plus-1.7.1/tests/plugins/sha256_hasher_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/tests/plugins/sha384_hasher_test.py` & `decoder-plus-plus-1.7.1/tests/plugins/sha384_hasher_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/tests/plugins/sha3_224_hasher_test.py` & `decoder-plus-plus-1.7.1/tests/plugins/sha3_224_hasher_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/tests/plugins/sha3_256_hasher_test.py` & `decoder-plus-plus-1.7.1/tests/plugins/sha3_256_hasher_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/tests/plugins/sha3_384_hasher_test.py` & `decoder-plus-plus-1.7.1/tests/plugins/sha3_384_hasher_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/tests/plugins/sha3_512_hasher_test.py` & `decoder-plus-plus-1.7.1/tests/plugins/sha3_512_hasher_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/tests/plugins/sha512_hasher_test.py` & `decoder-plus-plus-1.7.1/tests/plugins/sha512_hasher_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/tests/plugins/split_and_rejoin_script_test.py` & `decoder-plus-plus-1.7.1/tests/plugins/split_and_rejoin_script_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/tests/plugins/sun_md5_hasher_test.py` & `decoder-plus-plus-1.7.1/tests/plugins/sun_md5_hasher_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/tests/plugins/unescape_string_script_test.py` & `decoder-plus-plus-1.7.1/tests/plugins/unescape_string_script_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/tests/plugins/url_plus_test.py` & `decoder-plus-plus-1.7.1/tests/plugins/url_plus_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/tests/plugins/url_test.py` & `decoder-plus-plus-1.7.1/tests/plugins/url_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/tests/plugins/xpath_test.py` & `decoder-plus-plus-1.7.1/tests/plugins/xpath_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/tests/plugins/zlib_test.py` & `decoder-plus-plus-1.7.1/tests/plugins/zlib_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.0/tests/ui/classic_mode_test.py` & `decoder-plus-plus-1.7.1/tests/ui/classic_mode_test.py`

 * *Files 12% similar despite different names*

```diff
@@ -85,31 +85,41 @@
         plugin = load_plugin("Sha256", PluginType.HASHER)
         codec_frames.frame(1).setPlugin(plugin, block_signals=False)
         self.assertEqual(codec_frames.count(), 3)
         self.assertFrame(codec_frames.frame(0), "Hello, world!", "SGVsbG8sIHdvcmxkIQ==", ("DEFAULT", None), False)
         self.assertFrame(codec_frames.frame(1), "SGVsbG8sIHdvcmxkIQ==", "f978b1667208cc537def3f71a79f69475474d3f0bd2773f1f2428e73d31dc5ee", ("SUCCESS", None), True)
         self.assertFrame(codec_frames.frame(2), "f978b1667208cc537def3f71a79f69475474d3f0bd2773f1f2428e73d31dc5ee", "", ("SUCCESS", None), False)
 
-    def XtestMoveCodecUp(self):
+    def testChangingCodecDoesExecuteAllCodecsBelow(self):
+        # Changing Codec does not execute codecs below #61
+        idx, codec_tab = self.dpp.newTab("Hello, world!")
+        codec_frames = codec_tab.frames()
+        plugin = load_plugin("Base64", PluginType.ENCODER)
+        codec_frames.frame(0).setPlugin(plugin, block_signals=False)
+        plugin = load_plugin("Base45", PluginType.ENCODER)
+        codec_frames.frame(1).setPlugin(plugin, block_signals=False)
+        self.assertEqual(codec_frames.count(), 3)
+        self.assertFrame(codec_frames.frame(0), "Hello, world!", "SGVsbG8sIHdvcmxkIQ==", ("DEFAULT", None), False)
+        self.assertFrame(codec_frames.frame(1), "SGVsbG8sIHdvcmxkIQ==", "YNA -A4JC667+B9NVCSPC2AF4C9HX7", ("SUCCESS", None), True)
+        self.assertFrame(codec_frames.frame(2), "YNA -A4JC667+B9NVCSPC2AF4C9HX7", "", ("SUCCESS", None), False)
+        plugin = load_plugin("Base45", PluginType.ENCODER)
+        codec_frames.frame(0).setPlugin(plugin, block_signals=False)
+        self.assertEqual(codec_frames.count(), 3)
+        self.assertFrame(codec_frames.frame(0), "Hello, world!", "%69 VDK2EV4404ESVDX0", ("DEFAULT", None), False)
+        self.assertFrame(codec_frames.frame(1), "%69 VDK2EV4404ESVDX0", "VV4:97Y+AZM9KY8:Q6A46HY8Y+AV6B", ("SUCCESS", None), True)
+        self.assertFrame(codec_frames.frame(2), "VV4:97Y+AZM9KY8:Q6A46HY8Y+AV6B", "", ("SUCCESS", None), False)
+
+    def testMoveCodecUp(self):
         """
         # Example:
         #
         #   1. "Hello, world" - Base64 - open
         #   2. "<base64> of hello world" - Sha256 - collapsed
         #   3. "<sha256> of base64 hello world" - <> - open
-        #
-        #   Case 1. Press up on Frame 1
-        #
-        #       First frame can not be moved.
-        #
-        #   Case 2. Press down on Frame 2
-        #
-        #       Second frame can not be moved.
-        #
-        #   Case 3. Press up on Frame 3
+        #   4. Press up on Frame 3
         #
         #       Switching the codec of the previous frame with Frame 3 results in:
         #
         #       1. "Hello, world" - Sha256 - open
         #       2. "<sha256> of hello world" - Base64 - collapsed
         #       3. "<base64> of <sha256> of hello world" - open
         #
@@ -121,46 +131,34 @@
 
         def clickMoveUpButton(frame_index):
             QTest.mouseClick(codec_frames.frame(frame_index).getMoveUpButton().centralWidget(), Qt.LeftButton)
 
         def clickMoveDownButton(frame_index):
             QTest.mouseClick(codec_frames.frame(frame_index).getMoveDownButton().centralWidget(), Qt.LeftButton)
 
-
-        # Case 1 - First frame can not be moved.
-        #clickMoveDownButton(0)
-        #clickMoveUpButton(0)
-        #with self.assertRaises(AssertionError):
-        #    clickMoveUpButton(0)
-
-        #with self.assertRaises(AssertionError):
-        #    clickMoveDownButton(0)
-
-        # Case 2
-        try:
-            clickMoveDownButton(1)
-            pass
-        except AssertionError:
-            pass
-        #clickMoveUpButton(1)
-        self.assertEqual(codec_frames.count(), 3)
+        # 1. "Hello, world" - Base64 - open
+        idx, codec_tab = self.dpp.newTab("Hello, world!")
+        codec_frames = codec_tab.frames()
+        # 2. "<base64> of hello world" - Sha256 - collapsed
+        plugin = load_plugin("Base64", PluginType.ENCODER)
+        codec_frames.frame(0).setPlugin(plugin, block_signals=False)
+        # 3. "<sha256> of base64 hello world" - <> - open
+        plugin = load_plugin("Sha256", PluginType.HASHER)
+        codec_frames.frame(1).setPlugin(plugin, block_signals=False)
+        # Assert precondition
         self.assertFrame(codec_frames.frame(0), "Hello, world!", "SGVsbG8sIHdvcmxkIQ==", ("DEFAULT", None), False)
         self.assertFrame(codec_frames.frame(1), "SGVsbG8sIHdvcmxkIQ==", "f978b1667208cc537def3f71a79f69475474d3f0bd2773f1f2428e73d31dc5ee", ("SUCCESS", None), True)
         self.assertFrame(codec_frames.frame(2), "f978b1667208cc537def3f71a79f69475474d3f0bd2773f1f2428e73d31dc5ee", "", ("SUCCESS", None), False)
 
-        # Case 3
-        #clickMoveDownButton(2)
-        #clickMoveUpButton(2)
+        # 4. Press up on Frame 3
+        clickMoveUpButton(2)
         self.assertEqual(codec_frames.count(), 3)
-        self.assertFrame(codec_frames.frame(0), "Hello, world!", "SGVsbG8sIHdvcmxkIQ==", ("DEFAULT", None), False)
-        self.assertFrame(codec_frames.frame(1), "SGVsbG8sIHdvcmxkIQ==", "f978b1667208cc537def3f71a79f69475474d3f0bd2773f1f2428e73d31dc5ee", ("SUCCESS", None), True)
-        self.assertFrame(codec_frames.frame(2), "f978b1667208cc537def3f71a79f69475474d3f0bd2773f1f2428e73d31dc5ee", "", ("SUCCESS", None), False)
-
-
-
+        self.assertFrame(codec_frames.frame(0), "Hello, world!", "315f5bdb76d078c43b8ac0064e4a0164612b1fce77c869345bfc94c75894edd3", ("DEFAULT", None), False)
+        self.assertFrame(codec_frames.frame(1), "315f5bdb76d078c43b8ac0064e4a0164612b1fce77c869345bfc94c75894edd3", "MzE1ZjViZGI3NmQwNzhjNDNiOGFjMDA2NGU0YTAxNjQ2MTJiMWZjZTc3Yzg2OTM0NWJmYzk0Yzc1ODk0ZWRkMw==", ("SUCCESS", None), True)
+        self.assertFrame(codec_frames.frame(2), "MzE1ZjViZGI3NmQwNzhjNDNiOGFjMDA2NGU0YTAxNjQ2MTJiMWZjZTc3Yzg2OTM0NWJmYzk0Yzc1ODk0ZWRkMw==", "", ("SUCCESS", None), False)
 
     def testMoveCodecDown(self):
         """
         # Example:
         #
         #   1. "Hello, world" - Base64 - open
         #   2. "<base64> of hello world" - Sha256 - collapsed
```

### Comparing `decoder-plus-plus-1.7.0/tests/utils.py` & `decoder-plus-plus-1.7.1/tests/utils.py`

 * *Files identical despite different names*

