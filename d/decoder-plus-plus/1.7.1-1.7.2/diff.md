# Comparing `tmp/decoder-plus-plus-1.7.1.tar.gz` & `tmp/decoder-plus-plus-1.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "decoder-plus-plus-1.7.1.tar", last modified: Sun Apr  7 18:16:03 2024, max compression
+gzip compressed data, was "decoder-plus-plus-1.7.2.tar", last modified: Sun Apr  7 19:02:44 2024, max compression
```

## Comparing `decoder-plus-plus-1.7.1.tar` & `decoder-plus-plus-1.7.2.tar`

### file list

```diff
@@ -1,311 +1,312 @@
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-07 18:16:03.754202 decoder-plus-plus-1.7.1/
--rw-rw-r--   0 tom       (1000) tom       (1000)    35147 2021-12-26 21:21:06.000000 decoder-plus-plus-1.7.1/LICENSE
--rw-rw-r--   0 tom       (1000) tom       (1000)       43 2021-12-26 21:21:06.000000 decoder-plus-plus-1.7.1/MANIFEST.in
--rw-rw-r--   0 tom       (1000) tom       (1000)     7935 2024-04-07 18:16:03.754202 decoder-plus-plus-1.7.1/PKG-INFO
--rw-rw-r--   0 tom       (1000) tom       (1000)     7367 2024-04-07 09:27:21.000000 decoder-plus-plus-1.7.1/README.md
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-07 18:16:03.658201 decoder-plus-plus-1.7.1/data/
--rwxrwxr-x   0 tom       (1000) tom       (1000)      116 2021-12-26 21:21:06.000000 decoder-plus-plus-1.7.1/data/dpp.desktop
--rw-rw-r--   0 tom       (1000) tom       (1000)    19277 2024-04-06 19:21:46.000000 decoder-plus-plus-1.7.1/data/dpp.png
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-07 18:16:03.658201 decoder-plus-plus-1.7.1/decoder_plus_plus.egg-info/
--rw-rw-r--   0 tom       (1000) tom       (1000)     7935 2024-04-07 18:16:03.000000 decoder-plus-plus-1.7.1/decoder_plus_plus.egg-info/PKG-INFO
--rw-rw-r--   0 tom       (1000) tom       (1000)     9135 2024-04-07 18:16:03.000000 decoder-plus-plus-1.7.1/decoder_plus_plus.egg-info/SOURCES.txt
--rw-rw-r--   0 tom       (1000) tom       (1000)        1 2024-04-07 18:16:03.000000 decoder-plus-plus-1.7.1/decoder_plus_plus.egg-info/dependency_links.txt
--rw-rw-r--   0 tom       (1000) tom       (1000)       40 2024-04-07 18:16:03.000000 decoder-plus-plus-1.7.1/decoder_plus_plus.egg-info/entry_points.txt
--rw-rw-r--   0 tom       (1000) tom       (1000)      389 2024-04-07 18:16:03.000000 decoder-plus-plus-1.7.1/decoder_plus_plus.egg-info/requires.txt
--rw-rw-r--   0 tom       (1000) tom       (1000)       10 2024-04-07 18:16:03.000000 decoder-plus-plus-1.7.1/decoder_plus_plus.egg-info/top_level.txt
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-07 18:16:03.658201 decoder-plus-plus-1.7.1/dpp/
--rw-rw-r--   0 tom       (1000) tom       (1000)      850 2024-04-07 18:09:02.000000 decoder-plus-plus-1.7.1/dpp/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      239 2021-12-26 21:21:06.000000 decoder-plus-plus-1.7.1/dpp/__main__.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-07 18:16:03.662201 decoder-plus-plus-1.7.1/dpp/core/
--rw-rw-r--   0 tom       (1000) tom       (1000)      915 2021-12-26 21:21:06.000000 decoder-plus-plus-1.7.1/dpp/core/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     2353 2022-09-12 19:05:02.000000 decoder-plus-plus-1.7.1/dpp/core/argparse.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     2871 2022-09-12 21:57:24.000000 decoder-plus-plus-1.7.1/dpp/core/assertions.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     3279 2022-08-17 05:09:19.000000 decoder-plus-plus-1.7.1/dpp/core/config.py
--rw-rw-r--   0 tom       (1000) tom       (1000)    10068 2024-04-05 20:12:39.000000 decoder-plus-plus-1.7.1/dpp/core/context.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     2328 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.1/dpp/core/decoder_plus_plus.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      906 2022-09-18 10:36:35.000000 decoder-plus-plus-1.7.1/dpp/core/exceptions.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     2860 2024-04-07 11:17:10.000000 decoder-plus-plus-1.7.1/dpp/core/icons.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     3650 2023-02-28 12:27:33.000000 decoder-plus-plus-1.7.1/dpp/core/listener.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     4546 2023-01-29 15:42:26.000000 decoder-plus-plus-1.7.1/dpp/core/logger.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1329 2022-09-14 00:12:52.000000 decoder-plus-plus-1.7.1/dpp/core/math.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-07 18:16:03.662201 decoder-plus-plus-1.7.1/dpp/core/plugin/
--rw-rw-r--   0 tom       (1000) tom       (1000)    14067 2024-04-06 16:14:35.000000 decoder-plus-plus-1.7.1/dpp/core/plugin/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     2324 2024-04-06 15:25:06.000000 decoder-plus-plus-1.7.1/dpp/core/plugin/builder.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-07 18:16:03.662201 decoder-plus-plus-1.7.1/dpp/core/plugin/config/
--rw-rw-r--   0 tom       (1000) tom       (1000)     8387 2024-04-06 08:18:07.000000 decoder-plus-plus-1.7.1/dpp/core/plugin/config/__init__.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-07 18:16:03.666201 decoder-plus-plus-1.7.1/dpp/core/plugin/config/options/
--rw-rw-r--   0 tom       (1000) tom       (1000)     3478 2024-04-06 16:14:35.000000 decoder-plus-plus-1.7.1/dpp/core/plugin/config/options/__init__.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-07 18:16:03.666201 decoder-plus-plus-1.7.1/dpp/core/plugin/config/ui/
--rw-rw-r--   0 tom       (1000) tom       (1000)     1572 2022-09-12 21:57:24.000000 decoder-plus-plus-1.7.1/dpp/core/plugin/config/ui/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      858 2022-09-06 21:38:42.000000 decoder-plus-plus-1.7.1/dpp/core/plugin/config/ui/layouts.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     2111 2024-04-06 15:51:05.000000 decoder-plus-plus-1.7.1/dpp/core/plugin/config/ui/widgets.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     3048 2022-09-13 07:31:54.000000 decoder-plus-plus-1.7.1/dpp/core/plugin/loader.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     4301 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.1/dpp/core/plugin/manager.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     3878 2022-08-21 00:18:15.000000 decoder-plus-plus-1.7.1/dpp/core/shortcuts.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-07 18:16:03.678201 decoder-plus-plus-1.7.1/dpp/images/
--rw-rw-r--   0 tom       (1000) tom       (1000)    22919 2021-12-26 21:21:06.000000 decoder-plus-plus-1.7.1/dpp/images/dpp.png
--rw-rw-r--   0 tom       (1000) tom       (1000)    10621 2021-12-26 21:21:06.000000 decoder-plus-plus-1.7.1/dpp/images/dpp_128.png
--rw-rw-r--   0 tom       (1000) tom       (1000)    22919 2021-12-26 21:21:06.000000 decoder-plus-plus-1.7.1/dpp/images/dpp_classic.png
--rw-rw-r--   0 tom       (1000) tom       (1000)    10621 2021-12-26 21:21:06.000000 decoder-plus-plus-1.7.1/dpp/images/dpp_classic_128.png
--rw-rw-r--   0 tom       (1000) tom       (1000)    90434 2022-09-06 22:45:08.000000 decoder-plus-plus-1.7.1/dpp/images/dpp_modern.png
--rw-rw-r--   0 tom       (1000) tom       (1000)    30058 2022-09-06 22:47:19.000000 decoder-plus-plus-1.7.1/dpp/images/dpp_modern_128.png
--rw-rw-r--   0 tom       (1000) tom       (1000)  1494359 2022-09-06 22:43:36.000000 decoder-plus-plus-1.7.1/dpp/images/dpp_modern_big.png
--rw-rw-r--   0 tom       (1000) tom       (1000)    56153 2024-04-06 19:21:10.000000 decoder-plus-plus-1.7.1/dpp/images/dpp_stylized.png
--rw-rw-r--   0 tom       (1000) tom       (1000)    19277 2024-04-06 19:21:46.000000 decoder-plus-plus-1.7.1/dpp/images/dpp_stylized_128.png
--rw-rw-r--   0 tom       (1000) tom       (1000)    25196 2021-12-26 21:21:06.000000 decoder-plus-plus-1.7.1/dpp/images/dpp_xmas.png
--rw-rw-r--   0 tom       (1000) tom       (1000)    52648 2024-04-06 19:39:41.000000 decoder-plus-plus-1.7.1/dpp/images/dpp_xmas_stylized.png
--rw-rw-r--   0 tom       (1000) tom       (1000)      258 2021-12-26 21:21:06.000000 decoder-plus-plus-1.7.1/dpp/images/hidden.png
--rw-rw-r--   0 tom       (1000) tom       (1000)      349 2022-09-13 21:04:47.000000 decoder-plus-plus-1.7.1/dpp/images/indicator_green.png
--rw-rw-r--   0 tom       (1000) tom       (1000)      417 2022-09-13 21:05:13.000000 decoder-plus-plus-1.7.1/dpp/images/indicator_grey.png
--rw-rw-r--   0 tom       (1000) tom       (1000)      319 2022-09-13 21:05:36.000000 decoder-plus-plus-1.7.1/dpp/images/indicator_red.png
--rw-rw-r--   0 tom       (1000) tom       (1000)    11652 2021-12-26 21:21:06.000000 decoder-plus-plus-1.7.1/dpp/images/keyboard.png
--rw-rw-r--   0 tom       (1000) tom       (1000)    27999 2021-12-26 21:21:06.000000 decoder-plus-plus-1.7.1/dpp/images/keyboard.svg
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-07 18:16:03.706202 decoder-plus-plus-1.7.1/dpp/plugins/
--rw-rw-r--   0 tom       (1000) tom       (1000)     1328 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.1/dpp/plugins/adler32_hasher.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1393 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.1/dpp/plugins/apache_md5_hasher.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1545 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.1/dpp/plugins/base16_decoder.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1545 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.1/dpp/plugins/base16_encoder.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1824 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.1/dpp/plugins/base32_decoder.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1529 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.1/dpp/plugins/base32_encoder.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1755 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.1/dpp/plugins/base45_decoder.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1482 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.1/dpp/plugins/base45_encoder.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     2097 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.1/dpp/plugins/base64_decoder.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1470 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.1/dpp/plugins/base64_encoder.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     2678 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.1/dpp/plugins/base64_url_decoder.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1693 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.1/dpp/plugins/base64_url_encoder.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1241 2022-09-17 09:11:33.000000 decoder-plus-plus-1.7.1/dpp/plugins/bin_int_decoder.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1249 2022-09-17 09:11:33.000000 decoder-plus-plus-1.7.1/dpp/plugins/bin_int_encoder.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1519 2022-09-17 09:11:33.000000 decoder-plus-plus-1.7.1/dpp/plugins/bin_str_decoder.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1695 2022-09-17 09:11:33.000000 decoder-plus-plus-1.7.1/dpp/plugins/bin_str_encoder.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     5641 2024-04-05 16:00:23.000000 decoder-plus-plus-1.7.1/dpp/plugins/caesar_cipher_script.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1065 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.1/dpp/plugins/clone_script.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1320 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.1/dpp/plugins/crc32_hasher.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1159 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.1/dpp/plugins/css_minify_script.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     5888 2024-04-06 15:56:04.000000 decoder-plus-plus-1.7.1/dpp/plugins/custom_code.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1475 2022-09-17 09:13:06.000000 decoder-plus-plus-1.7.1/dpp/plugins/dec_str_decoder.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1441 2022-09-17 09:13:12.000000 decoder-plus-plus-1.7.1/dpp/plugins/dec_str_encoder.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1068 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.1/dpp/plugins/escape_string_script.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1211 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.1/dpp/plugins/extract_urls_script.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     5143 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.1/dpp/plugins/filter_lines_script.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1386 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.1/dpp/plugins/free_bsd_nt_hasher.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1653 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.1/dpp/plugins/gzip_decoder.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1408 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.1/dpp/plugins/gzip_encoder.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     2110 2022-11-01 18:01:29.000000 decoder-plus-plus-1.7.1/dpp/plugins/hex_char_decoder.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1582 2022-11-01 18:01:29.000000 decoder-plus-plus-1.7.1/dpp/plugins/hex_char_encoder.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1448 2022-11-01 18:01:29.000000 decoder-plus-plus-1.7.1/dpp/plugins/hex_int_decoder.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1217 2022-11-01 18:01:29.000000 decoder-plus-plus-1.7.1/dpp/plugins/hex_int_encoder.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     2331 2022-11-01 18:01:29.000000 decoder-plus-plus-1.7.1/dpp/plugins/hex_shell_decoder.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1980 2022-11-01 18:01:29.000000 decoder-plus-plus-1.7.1/dpp/plugins/hex_shell_encoder.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1709 2022-11-01 18:01:29.000000 decoder-plus-plus-1.7.1/dpp/plugins/hex_str_decoder.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1561 2022-11-01 18:01:29.000000 decoder-plus-plus-1.7.1/dpp/plugins/hex_str_encoder.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1221 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.1/dpp/plugins/html_beautify_script.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1783 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.1/dpp/plugins/html_decoder.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1377 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.1/dpp/plugins/html_encoder.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1138 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.1/dpp/plugins/html_minify_script.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     2539 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.1/dpp/plugins/http64_decoder.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1841 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.1/dpp/plugins/http64_encoder.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     2265 2024-04-07 11:11:41.000000 decoder-plus-plus-1.7.1/dpp/plugins/identify_decoder_script.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1371 2024-04-07 11:16:17.000000 decoder-plus-plus-1.7.1/dpp/plugins/identify_file_type_filemagic_script.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1478 2024-04-07 11:16:17.000000 decoder-plus-plus-1.7.1/dpp/plugins/identify_file_type_magika_script.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1389 2024-04-07 11:03:59.000000 decoder-plus-plus-1.7.1/dpp/plugins/identify_hash_format_script.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     2254 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.1/dpp/plugins/jq_script.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1336 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.1/dpp/plugins/js_beautify_script.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1131 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.1/dpp/plugins/js_minify_script.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1171 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.1/dpp/plugins/js_to_xml_script.py
--rw-rw-r--   0 tom       (1000) tom       (1000)    15185 2024-04-07 08:30:22.000000 decoder-plus-plus-1.7.1/dpp/plugins/jsonify_script.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     2621 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.1/dpp/plugins/jsonpath_script.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1612 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.1/dpp/plugins/jwt_decoder.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1432 2022-09-15 16:34:02.000000 decoder-plus-plus-1.7.1/dpp/plugins/keccak224_hasher.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1440 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.1/dpp/plugins/keccak256_hasher.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1472 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.1/dpp/plugins/keccak384_hasher.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1519 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.1/dpp/plugins/keccak512_hasher.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1446 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.1/dpp/plugins/little_big_endian_script.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1366 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.1/dpp/plugins/lm_hasher.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1364 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.1/dpp/plugins/md2_hasher.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1364 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.1/dpp/plugins/md4_hasher.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1352 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.1/dpp/plugins/md5_hasher.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1366 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.1/dpp/plugins/nt_hasher.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1223 2022-09-17 09:11:33.000000 decoder-plus-plus-1.7.1/dpp/plugins/oct_int_decoder.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1228 2022-09-17 09:11:33.000000 decoder-plus-plus-1.7.1/dpp/plugins/oct_int_encoder.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1775 2022-09-17 09:11:33.000000 decoder-plus-plus-1.7.1/dpp/plugins/oct_str_decoder.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1576 2022-09-17 09:11:33.000000 decoder-plus-plus-1.7.1/dpp/plugins/oct_str_encoder.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1368 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.1/dpp/plugins/phpass_hasher.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     6590 2024-04-05 18:32:58.000000 decoder-plus-plus-1.7.1/dpp/plugins/reformat_text_script.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1115 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.1/dpp/plugins/remove_newlines_script.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1121 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.1/dpp/plugins/remove_whitespaces_script.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1693 2024-04-07 07:30:09.000000 decoder-plus-plus-1.7.1/dpp/plugins/ripemd160_hasher.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1398 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.1/dpp/plugins/rot13_decoder.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1398 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.1/dpp/plugins/rot13_encoder.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     4506 2024-04-05 18:32:58.000000 decoder-plus-plus-1.7.1/dpp/plugins/search_and_replace_script.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1363 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.1/dpp/plugins/sha1_hasher.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1401 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.1/dpp/plugins/sha224_hasher.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1409 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.1/dpp/plugins/sha256_hasher.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1441 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.1/dpp/plugins/sha384_hasher.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1382 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.1/dpp/plugins/sha3_224_hasher.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1383 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.1/dpp/plugins/sha3_256_hasher.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1415 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.1/dpp/plugins/sha3_384_hasher.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1462 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.1/dpp/plugins/sha3_512_hasher.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1474 2022-09-12 18:36:42.000000 decoder-plus-plus-1.7.1/dpp/plugins/sha512_hasher.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     4998 2024-04-05 18:32:58.000000 decoder-plus-plus-1.7.1/dpp/plugins/split_and_rejoin_script.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1400 2022-09-12 18:36:42.000000 decoder-plus-plus-1.7.1/dpp/plugins/sun_md5_hasher.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1107 2022-09-12 18:36:42.000000 decoder-plus-plus-1.7.1/dpp/plugins/unescape_string_script.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1993 2022-09-12 18:36:42.000000 decoder-plus-plus-1.7.1/dpp/plugins/url_decoder.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1487 2022-09-12 18:36:42.000000 decoder-plus-plus-1.7.1/dpp/plugins/url_encoder.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1974 2022-09-12 18:36:42.000000 decoder-plus-plus-1.7.1/dpp/plugins/url_plus_decoder.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1525 2022-09-12 18:36:42.000000 decoder-plus-plus-1.7.1/dpp/plugins/url_plus_encoder.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     2291 2023-01-15 14:37:27.000000 decoder-plus-plus-1.7.1/dpp/plugins/xpath_script.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1821 2022-09-12 18:36:42.000000 decoder-plus-plus-1.7.1/dpp/plugins/zlib_decoder.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1394 2022-09-12 18:36:42.000000 decoder-plus-plus-1.7.1/dpp/plugins/zlib_encoder.py
--rwxrwxr-x   0 tom       (1000) tom       (1000)    16769 2022-09-21 05:00:04.000000 decoder-plus-plus-1.7.1/dpp/runner.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-07 18:16:03.706202 decoder-plus-plus-1.7.1/dpp/ui/
--rw-rw-r--   0 tom       (1000) tom       (1000)      967 2022-09-06 05:50:59.000000 decoder-plus-plus-1.7.1/dpp/ui/__init__.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-07 18:16:03.706202 decoder-plus-plus-1.7.1/dpp/ui/builder/
--rw-rw-r--   0 tom       (1000) tom       (1000)        0 2021-12-26 21:21:06.000000 decoder-plus-plus-1.7.1/dpp/ui/builder/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1962 2022-08-15 20:49:18.000000 decoder-plus-plus-1.7.1/dpp/ui/builder/action_builder.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1547 2023-03-07 03:42:36.000000 decoder-plus-plus-1.7.1/dpp/ui/builder/input_text_builder.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1682 2024-04-05 15:27:20.000000 decoder-plus-plus-1.7.1/dpp/ui/builder/plugin_config_widget_builder.py
--rw-rw-r--   0 tom       (1000) tom       (1000)    10393 2024-04-07 07:53:50.000000 decoder-plus-plus-1.7.1/dpp/ui/builder/widget_builder.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     6388 2023-01-29 15:44:47.000000 decoder-plus-plus-1.7.1/dpp/ui/decoder_plus_plus_gui.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-07 18:16:03.710202 decoder-plus-plus-1.7.1/dpp/ui/dialog/
--rw-rw-r--   0 tom       (1000) tom       (1000)      706 2021-12-26 21:21:06.000000 decoder-plus-plus-1.7.1/dpp/ui/dialog/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     5833 2024-04-06 19:42:04.000000 decoder-plus-plus-1.7.1/dpp/ui/dialog/config_dialog.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     5273 2022-09-10 21:34:51.000000 decoder-plus-plus-1.7.1/dpp/ui/dialog/keyboard_shortcut_dialog.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     6012 2024-04-06 09:24:31.000000 decoder-plus-plus-1.7.1/dpp/ui/dialog/plugin_config_dialog.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-07 18:16:03.710202 decoder-plus-plus-1.7.1/dpp/ui/dock/
--rw-rw-r--   0 tom       (1000) tom       (1000)        0 2021-12-26 21:21:06.000000 decoder-plus-plus-1.7.1/dpp/ui/dock/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)    10582 2023-02-28 12:28:51.000000 decoder-plus-plus-1.7.1/dpp/ui/dock/hex_dock.py
--rw-rw-r--   0 tom       (1000) tom       (1000)    12701 2022-09-12 19:05:02.000000 decoder-plus-plus-1.7.1/dpp/ui/dock/log_dock.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     2564 2022-09-07 22:11:21.000000 decoder-plus-plus-1.7.1/dpp/ui/instance_handler.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-07 18:16:03.710202 decoder-plus-plus-1.7.1/dpp/ui/view/
--rw-rw-r--   0 tom       (1000) tom       (1000)      706 2022-08-18 00:21:03.000000 decoder-plus-plus-1.7.1/dpp/ui/view/__init__.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-07 18:16:03.714202 decoder-plus-plus-1.7.1/dpp/ui/view/classic/
--rw-rw-r--   0 tom       (1000) tom       (1000)      839 2022-08-20 19:51:05.000000 decoder-plus-plus-1.7.1/dpp/ui/view/classic/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)    10186 2024-04-06 16:14:35.000000 decoder-plus-plus-1.7.1/dpp/ui/view/classic/classic_main_window_widget.py
--rw-rw-r--   0 tom       (1000) tom       (1000)    16982 2024-04-07 13:12:43.000000 decoder-plus-plus-1.7.1/dpp/ui/view/classic/codec_frame.py
--rw-rw-r--   0 tom       (1000) tom       (1000)    13200 2022-09-15 16:14:00.000000 decoder-plus-plus-1.7.1/dpp/ui/view/classic/codec_frame_header.py
--rw-rw-r--   0 tom       (1000) tom       (1000)    20625 2024-04-07 18:07:00.000000 decoder-plus-plus-1.7.1/dpp/ui/view/classic/codec_frames.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     2401 2022-09-20 04:28:03.000000 decoder-plus-plus-1.7.1/dpp/ui/view/classic/codec_tab.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     9167 2023-01-30 13:35:51.000000 decoder-plus-plus-1.7.1/dpp/ui/view/classic/combo_box_frame.py
--rw-rw-r--   0 tom       (1000) tom       (1000)    10716 2022-09-21 05:00:04.000000 decoder-plus-plus-1.7.1/dpp/ui/view/main_window_widget.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-07 18:16:03.722202 decoder-plus-plus-1.7.1/dpp/ui/view/modern/
--rw-rw-r--   0 tom       (1000) tom       (1000)      705 2022-08-20 19:51:05.000000 decoder-plus-plus-1.7.1/dpp/ui/view/modern/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     2460 2022-09-17 10:02:26.000000 decoder-plus-plus-1.7.1/dpp/ui/view/modern/modern_main_window_widget.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      705 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.1/dpp/ui/view/modern/node_data.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     5229 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.1/dpp/ui/view/modern/node_data_models.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      409 2022-08-30 00:07:08.000000 decoder-plus-plus-1.7.1/dpp/ui/view/modern/node_data_models_builder.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     2001 2022-09-17 10:02:44.000000 decoder-plus-plus-1.7.1/dpp/ui/view/modern/node_editor.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1782 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.1/dpp/ui/view/modern/node_editor_tab.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-07 18:16:03.730202 decoder-plus-plus-1.7.1/dpp/ui/widget/
--rw-rw-r--   0 tom       (1000) tom       (1000)      805 2022-08-16 19:35:20.000000 decoder-plus-plus-1.7.1/dpp/ui/widget/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1367 2022-08-15 23:02:30.000000 decoder-plus-plus-1.7.1/dpp/ui/widget/clickable_label.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     3507 2024-04-06 16:14:35.000000 decoder-plus-plus-1.7.1/dpp/ui/widget/code_editor_widget.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     3404 2024-04-07 09:41:34.000000 decoder-plus-plus-1.7.1/dpp/ui/widget/codec_preview_widget.py
--rw-rw-r--   0 tom       (1000) tom       (1000)    11051 2024-04-06 07:30:01.000000 decoder-plus-plus-1.7.1/dpp/ui/widget/collapsible_frame.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     2161 2022-09-10 22:00:08.000000 decoder-plus-plus-1.7.1/dpp/ui/widget/combo_box.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     4686 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.1/dpp/ui/widget/dock_tabs_widget.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     7690 2022-08-20 19:51:05.000000 decoder-plus-plus-1.7.1/dpp/ui/widget/dock_widget.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1887 2022-08-15 20:48:14.000000 decoder-plus-plus-1.7.1/dpp/ui/widget/dyna_frame.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      755 2022-08-15 20:44:52.000000 decoder-plus-plus-1.7.1/dpp/ui/widget/elided_label.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     2453 2024-04-06 20:17:41.000000 decoder-plus-plus-1.7.1/dpp/ui/widget/hover_label.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1793 2024-04-06 07:22:30.000000 decoder-plus-plus-1.7.1/dpp/ui/widget/icon_label.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     3270 2024-04-07 11:20:24.000000 decoder-plus-plus-1.7.1/dpp/ui/widget/identify_format_button.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     3269 2022-09-12 19:34:03.000000 decoder-plus-plus-1.7.1/dpp/ui/widget/list_widget.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1151 2022-08-21 00:18:15.000000 decoder-plus-plus-1.7.1/dpp/ui/widget/menu_bar.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     2136 2024-04-06 09:24:31.000000 decoder-plus-plus-1.7.1/dpp/ui/widget/message_box_widget.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     6687 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.1/dpp/ui/widget/message_widget.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     6110 2024-04-06 15:44:53.000000 decoder-plus-plus-1.7.1/dpp/ui/widget/option_widgets.py
--rw-rw-r--   0 tom       (1000) tom       (1000)    16152 2023-03-14 08:16:41.000000 decoder-plus-plus-1.7.1/dpp/ui/widget/plain_view.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     2621 2022-09-08 00:44:43.000000 decoder-plus-plus-1.7.1/dpp/ui/widget/plugin_frame.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     9593 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.1/dpp/ui/widget/plugin_tab.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     4396 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.1/dpp/ui/widget/search_field.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1246 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.1/dpp/ui/widget/separater_widget.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     5000 2022-08-15 23:02:30.000000 decoder-plus-plus-1.7.1/dpp/ui/widget/shortcut_table.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     2846 2022-09-12 18:36:42.000000 decoder-plus-plus-1.7.1/dpp/ui/widget/slider_widget.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     4055 2022-09-20 10:34:13.000000 decoder-plus-plus-1.7.1/dpp/ui/widget/smart_decode_button.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1442 2022-09-12 18:36:42.000000 decoder-plus-plus-1.7.1/dpp/ui/widget/spacers.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     2425 2023-01-30 12:23:56.000000 decoder-plus-plus-1.7.1/dpp/ui/widget/status_widget.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     3757 2022-08-20 19:51:05.000000 decoder-plus-plus-1.7.1/dpp/ui/widget/tab_bar.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     8075 2022-09-15 01:50:24.000000 decoder-plus-plus-1.7.1/dpp/ui/widget/tabs_widget.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     3210 2024-04-05 11:52:36.000000 decoder-plus-plus-1.7.1/dpp/ui/widget/text_widget.py
--rw-rw-r--   0 tom       (1000) tom       (1000)       38 2024-04-07 18:16:03.754202 decoder-plus-plus-1.7.1/setup.cfg
--rw-rw-r--   0 tom       (1000) tom       (1000)     2679 2024-04-07 10:39:21.000000 decoder-plus-plus-1.7.1/setup.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-07 18:16:03.734202 decoder-plus-plus-1.7.1/tests/
--rw-rw-r--   0 tom       (1000) tom       (1000)     1805 2023-01-15 14:31:34.000000 decoder-plus-plus-1.7.1/tests/__init__.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-07 18:16:03.754202 decoder-plus-plus-1.7.1/tests/plugins/
--rw-rw-r--   0 tom       (1000) tom       (1000)        0 2022-11-01 13:33:59.000000 decoder-plus-plus-1.7.1/tests/plugins/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1113 2022-11-01 14:08:45.000000 decoder-plus-plus-1.7.1/tests/plugins/adler32_hasher_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1191 2022-11-01 18:50:27.000000 decoder-plus-plus-1.7.1/tests/plugins/apache_md5_hasher_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1295 2022-11-01 18:05:54.000000 decoder-plus-plus-1.7.1/tests/plugins/base16_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1680 2023-01-15 13:01:54.000000 decoder-plus-plus-1.7.1/tests/plugins/base32_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1287 2023-01-15 13:32:25.000000 decoder-plus-plus-1.7.1/tests/plugins/base45_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1288 2023-01-15 12:36:51.000000 decoder-plus-plus-1.7.1/tests/plugins/base64_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1474 2023-01-15 12:47:27.000000 decoder-plus-plus-1.7.1/tests/plugins/base64_url_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1229 2023-01-15 13:29:43.000000 decoder-plus-plus-1.7.1/tests/plugins/bin_int_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1040 2022-11-01 18:51:09.000000 decoder-plus-plus-1.7.1/tests/plugins/bin_str_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      992 2023-01-15 12:47:59.000000 decoder-plus-plus-1.7.1/tests/plugins/caesar_cipher_script_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1222 2022-11-01 18:35:38.000000 decoder-plus-plus-1.7.1/tests/plugins/clone_script_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1108 2023-01-15 12:37:31.000000 decoder-plus-plus-1.7.1/tests/plugins/crc32_hasher_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1183 2022-11-01 18:39:55.000000 decoder-plus-plus-1.7.1/tests/plugins/css_minify_script_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1401 2022-11-01 18:35:21.000000 decoder-plus-plus-1.7.1/tests/plugins/dec_str_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1245 2022-11-01 18:59:45.000000 decoder-plus-plus-1.7.1/tests/plugins/escape_string_script_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1123 2022-11-01 18:47:57.000000 decoder-plus-plus-1.7.1/tests/plugins/extract_urls_script_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1165 2022-11-01 18:40:22.000000 decoder-plus-plus-1.7.1/tests/plugins/filter_lines_script_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1189 2023-01-15 13:03:50.000000 decoder-plus-plus-1.7.1/tests/plugins/free_bsd_nt_hasher_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1253 2023-01-15 12:29:09.000000 decoder-plus-plus-1.7.1/tests/plugins/gzip_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1067 2022-11-01 18:47:18.000000 decoder-plus-plus-1.7.1/tests/plugins/hex_char_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1193 2023-01-15 13:10:42.000000 decoder-plus-plus-1.7.1/tests/plugins/hex_int_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1614 2022-11-01 18:43:06.000000 decoder-plus-plus-1.7.1/tests/plugins/hex_shell_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1313 2023-01-15 13:16:46.000000 decoder-plus-plus-1.7.1/tests/plugins/hex_str_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1173 2022-11-01 18:43:28.000000 decoder-plus-plus-1.7.1/tests/plugins/html_beautify_script_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1168 2022-11-01 18:48:47.000000 decoder-plus-plus-1.7.1/tests/plugins/html_minify_script_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1172 2023-01-15 12:22:31.000000 decoder-plus-plus-1.7.1/tests/plugins/html_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1219 2022-11-01 18:32:01.000000 decoder-plus-plus-1.7.1/tests/plugins/http64_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1016 2024-04-07 12:31:43.000000 decoder-plus-plus-1.7.1/tests/plugins/identify_file_type_filemagic_script_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1019 2024-04-07 12:32:46.000000 decoder-plus-plus-1.7.1/tests/plugins/identify_file_type_magika_script_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1108 2022-11-01 18:39:55.000000 decoder-plus-plus-1.7.1/tests/plugins/identify_hash_format_script_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1145 2023-01-15 13:26:35.000000 decoder-plus-plus-1.7.1/tests/plugins/jq_script_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      988 2023-01-15 12:41:00.000000 decoder-plus-plus-1.7.1/tests/plugins/js_beautify_script_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1164 2022-11-01 18:49:20.000000 decoder-plus-plus-1.7.1/tests/plugins/js_minify_script_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      977 2023-01-15 13:06:33.000000 decoder-plus-plus-1.7.1/tests/plugins/js_to_xml_script_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      981 2023-01-15 13:02:34.000000 decoder-plus-plus-1.7.1/tests/plugins/jsonify_script_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1163 2022-11-01 18:49:36.000000 decoder-plus-plus-1.7.1/tests/plugins/jsonpath_script_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      976 2023-01-15 12:39:55.000000 decoder-plus-plus-1.7.1/tests/plugins/jwt_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1163 2023-01-15 13:02:49.000000 decoder-plus-plus-1.7.1/tests/plugins/keccak224_hasher_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1171 2022-11-01 18:56:46.000000 decoder-plus-plus-1.7.1/tests/plugins/keccak256_hasher_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1203 2022-11-01 18:45:25.000000 decoder-plus-plus-1.7.1/tests/plugins/keccak384_hasher_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1235 2022-11-01 18:48:57.000000 decoder-plus-plus-1.7.1/tests/plugins/keccak512_hasher_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1245 2022-11-01 18:31:13.000000 decoder-plus-plus-1.7.1/tests/plugins/little_big_endian_script_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1124 2022-11-01 18:56:24.000000 decoder-plus-plus-1.7.1/tests/plugins/lm_hasher_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1126 2022-11-01 18:24:14.000000 decoder-plus-plus-1.7.1/tests/plugins/md2_hasher_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1126 2022-11-01 18:56:15.000000 decoder-plus-plus-1.7.1/tests/plugins/md4_hasher_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1126 2022-11-01 18:45:18.000000 decoder-plus-plus-1.7.1/tests/plugins/md5_hasher_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1124 2022-11-01 18:46:24.000000 decoder-plus-plus-1.7.1/tests/plugins/nt_hasher_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1193 2023-01-15 13:13:49.000000 decoder-plus-plus-1.7.1/tests/plugins/oct_int_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1405 2022-11-01 18:20:57.000000 decoder-plus-plus-1.7.1/tests/plugins/oct_str_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1181 2023-01-15 12:51:06.000000 decoder-plus-plus-1.7.1/tests/plugins/phpass_hasher_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1167 2022-11-01 18:57:07.000000 decoder-plus-plus-1.7.1/tests/plugins/reformat_text_script_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1187 2023-01-15 13:04:21.000000 decoder-plus-plus-1.7.1/tests/plugins/remove_newlines_script_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1064 2022-11-01 18:56:04.000000 decoder-plus-plus-1.7.1/tests/plugins/remove_whitespaces_script_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1146 2022-11-01 18:56:36.000000 decoder-plus-plus-1.7.1/tests/plugins/ripemd160_hasher_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1225 2022-11-01 18:26:44.000000 decoder-plus-plus-1.7.1/tests/plugins/rot13_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1503 2023-01-15 13:05:35.000000 decoder-plus-plus-1.7.1/tests/plugins/search_and_replace_script_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1136 2022-11-01 18:27:54.000000 decoder-plus-plus-1.7.1/tests/plugins/sha1_hasher_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1192 2022-11-01 18:29:14.000000 decoder-plus-plus-1.7.1/tests/plugins/sha224_hasher_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1200 2022-11-01 18:29:35.000000 decoder-plus-plus-1.7.1/tests/plugins/sha256_hasher_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1231 2022-11-01 18:29:59.000000 decoder-plus-plus-1.7.1/tests/plugins/sha384_hasher_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1160 2023-01-15 12:37:21.000000 decoder-plus-plus-1.7.1/tests/plugins/sha3_224_hasher_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1168 2022-11-01 18:53:45.000000 decoder-plus-plus-1.7.1/tests/plugins/sha3_256_hasher_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1200 2022-11-01 18:28:35.000000 decoder-plus-plus-1.7.1/tests/plugins/sha3_384_hasher_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1268 2022-11-01 18:28:57.000000 decoder-plus-plus-1.7.1/tests/plugins/sha3_512_hasher_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1263 2022-11-01 18:30:17.000000 decoder-plus-plus-1.7.1/tests/plugins/sha512_hasher_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1170 2022-11-01 18:57:46.000000 decoder-plus-plus-1.7.1/tests/plugins/split_and_rejoin_script_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      983 2023-01-15 12:39:55.000000 decoder-plus-plus-1.7.1/tests/plugins/sun_md5_hasher_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1247 2022-11-01 18:32:56.000000 decoder-plus-plus-1.7.1/tests/plugins/unescape_string_script_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1282 2022-11-01 18:45:08.000000 decoder-plus-plus-1.7.1/tests/plugins/url_plus_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1136 2022-11-01 18:53:35.000000 decoder-plus-plus-1.7.1/tests/plugins/url_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1136 2023-01-15 14:38:44.000000 decoder-plus-plus-1.7.1/tests/plugins/xpath_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1223 2023-01-15 13:12:30.000000 decoder-plus-plus-1.7.1/tests/plugins/zlib_test.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-07 18:16:03.754202 decoder-plus-plus-1.7.1/tests/ui/
--rw-rw-r--   0 tom       (1000) tom       (1000)        0 2023-01-15 14:39:42.000000 decoder-plus-plus-1.7.1/tests/ui/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)    10085 2024-04-07 18:07:00.000000 decoder-plus-plus-1.7.1/tests/ui/classic_mode_test.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      512 2023-01-15 15:28:09.000000 decoder-plus-plus-1.7.1/tests/utils.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-07 19:02:44.568739 decoder-plus-plus-1.7.2/
+-rw-rw-r--   0 tom       (1000) tom       (1000)    35147 2021-12-26 21:21:06.000000 decoder-plus-plus-1.7.2/LICENSE
+-rw-rw-r--   0 tom       (1000) tom       (1000)       43 2021-12-26 21:21:06.000000 decoder-plus-plus-1.7.2/MANIFEST.in
+-rw-rw-r--   0 tom       (1000) tom       (1000)     7935 2024-04-07 19:02:44.568739 decoder-plus-plus-1.7.2/PKG-INFO
+-rw-rw-r--   0 tom       (1000) tom       (1000)     7367 2024-04-07 09:27:21.000000 decoder-plus-plus-1.7.2/README.md
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-07 19:02:44.524738 decoder-plus-plus-1.7.2/data/
+-rwxrwxr-x   0 tom       (1000) tom       (1000)      116 2021-12-26 21:21:06.000000 decoder-plus-plus-1.7.2/data/dpp.desktop
+-rw-rw-r--   0 tom       (1000) tom       (1000)    19277 2024-04-06 19:21:46.000000 decoder-plus-plus-1.7.2/data/dpp.png
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-07 19:02:44.524738 decoder-plus-plus-1.7.2/decoder_plus_plus.egg-info/
+-rw-rw-r--   0 tom       (1000) tom       (1000)     7935 2024-04-07 19:02:44.000000 decoder-plus-plus-1.7.2/decoder_plus_plus.egg-info/PKG-INFO
+-rw-rw-r--   0 tom       (1000) tom       (1000)     9162 2024-04-07 19:02:44.000000 decoder-plus-plus-1.7.2/decoder_plus_plus.egg-info/SOURCES.txt
+-rw-rw-r--   0 tom       (1000) tom       (1000)        1 2024-04-07 19:02:44.000000 decoder-plus-plus-1.7.2/decoder_plus_plus.egg-info/dependency_links.txt
+-rw-rw-r--   0 tom       (1000) tom       (1000)       40 2024-04-07 19:02:44.000000 decoder-plus-plus-1.7.2/decoder_plus_plus.egg-info/entry_points.txt
+-rw-rw-r--   0 tom       (1000) tom       (1000)      391 2024-04-07 19:02:44.000000 decoder-plus-plus-1.7.2/decoder_plus_plus.egg-info/requires.txt
+-rw-rw-r--   0 tom       (1000) tom       (1000)       10 2024-04-07 19:02:44.000000 decoder-plus-plus-1.7.2/decoder_plus_plus.egg-info/top_level.txt
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-07 19:02:44.524738 decoder-plus-plus-1.7.2/dpp/
+-rw-rw-r--   0 tom       (1000) tom       (1000)      850 2024-04-07 18:59:53.000000 decoder-plus-plus-1.7.2/dpp/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      239 2021-12-26 21:21:06.000000 decoder-plus-plus-1.7.2/dpp/__main__.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-07 19:02:44.528739 decoder-plus-plus-1.7.2/dpp/core/
+-rw-rw-r--   0 tom       (1000) tom       (1000)      915 2021-12-26 21:21:06.000000 decoder-plus-plus-1.7.2/dpp/core/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2353 2022-09-12 19:05:02.000000 decoder-plus-plus-1.7.2/dpp/core/argparse.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2871 2022-09-12 21:57:24.000000 decoder-plus-plus-1.7.2/dpp/core/assertions.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     3279 2022-08-17 05:09:19.000000 decoder-plus-plus-1.7.2/dpp/core/config.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)    10068 2024-04-05 20:12:39.000000 decoder-plus-plus-1.7.2/dpp/core/context.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2328 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.2/dpp/core/decoder_plus_plus.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      906 2022-09-18 10:36:35.000000 decoder-plus-plus-1.7.2/dpp/core/exceptions.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2860 2024-04-07 11:17:10.000000 decoder-plus-plus-1.7.2/dpp/core/icons.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     3650 2023-02-28 12:27:33.000000 decoder-plus-plus-1.7.2/dpp/core/listener.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     4546 2023-01-29 15:42:26.000000 decoder-plus-plus-1.7.2/dpp/core/logger.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1329 2022-09-14 00:12:52.000000 decoder-plus-plus-1.7.2/dpp/core/math.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-07 19:02:44.528739 decoder-plus-plus-1.7.2/dpp/core/plugin/
+-rw-rw-r--   0 tom       (1000) tom       (1000)    14067 2024-04-06 16:14:35.000000 decoder-plus-plus-1.7.2/dpp/core/plugin/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2324 2024-04-06 15:25:06.000000 decoder-plus-plus-1.7.2/dpp/core/plugin/builder.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-07 19:02:44.528739 decoder-plus-plus-1.7.2/dpp/core/plugin/config/
+-rw-rw-r--   0 tom       (1000) tom       (1000)     8387 2024-04-06 08:18:07.000000 decoder-plus-plus-1.7.2/dpp/core/plugin/config/__init__.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-07 19:02:44.528739 decoder-plus-plus-1.7.2/dpp/core/plugin/config/options/
+-rw-rw-r--   0 tom       (1000) tom       (1000)     3478 2024-04-06 16:14:35.000000 decoder-plus-plus-1.7.2/dpp/core/plugin/config/options/__init__.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-07 19:02:44.528739 decoder-plus-plus-1.7.2/dpp/core/plugin/config/ui/
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1572 2022-09-12 21:57:24.000000 decoder-plus-plus-1.7.2/dpp/core/plugin/config/ui/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      858 2022-09-06 21:38:42.000000 decoder-plus-plus-1.7.2/dpp/core/plugin/config/ui/layouts.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2111 2024-04-06 15:51:05.000000 decoder-plus-plus-1.7.2/dpp/core/plugin/config/ui/widgets.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     3048 2022-09-13 07:31:54.000000 decoder-plus-plus-1.7.2/dpp/core/plugin/loader.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     4301 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.2/dpp/core/plugin/manager.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     3878 2022-08-21 00:18:15.000000 decoder-plus-plus-1.7.2/dpp/core/shortcuts.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-07 19:02:44.532739 decoder-plus-plus-1.7.2/dpp/images/
+-rw-rw-r--   0 tom       (1000) tom       (1000)    22919 2021-12-26 21:21:06.000000 decoder-plus-plus-1.7.2/dpp/images/dpp.png
+-rw-rw-r--   0 tom       (1000) tom       (1000)    10621 2021-12-26 21:21:06.000000 decoder-plus-plus-1.7.2/dpp/images/dpp_128.png
+-rw-rw-r--   0 tom       (1000) tom       (1000)    22919 2021-12-26 21:21:06.000000 decoder-plus-plus-1.7.2/dpp/images/dpp_classic.png
+-rw-rw-r--   0 tom       (1000) tom       (1000)    10621 2021-12-26 21:21:06.000000 decoder-plus-plus-1.7.2/dpp/images/dpp_classic_128.png
+-rw-rw-r--   0 tom       (1000) tom       (1000)    90434 2022-09-06 22:45:08.000000 decoder-plus-plus-1.7.2/dpp/images/dpp_modern.png
+-rw-rw-r--   0 tom       (1000) tom       (1000)    30058 2022-09-06 22:47:19.000000 decoder-plus-plus-1.7.2/dpp/images/dpp_modern_128.png
+-rw-rw-r--   0 tom       (1000) tom       (1000)  1494359 2022-09-06 22:43:36.000000 decoder-plus-plus-1.7.2/dpp/images/dpp_modern_big.png
+-rw-rw-r--   0 tom       (1000) tom       (1000)    56153 2024-04-06 19:21:10.000000 decoder-plus-plus-1.7.2/dpp/images/dpp_stylized.png
+-rw-rw-r--   0 tom       (1000) tom       (1000)    19277 2024-04-06 19:21:46.000000 decoder-plus-plus-1.7.2/dpp/images/dpp_stylized_128.png
+-rw-rw-r--   0 tom       (1000) tom       (1000)    25196 2021-12-26 21:21:06.000000 decoder-plus-plus-1.7.2/dpp/images/dpp_xmas.png
+-rw-rw-r--   0 tom       (1000) tom       (1000)    52648 2024-04-06 19:39:41.000000 decoder-plus-plus-1.7.2/dpp/images/dpp_xmas_stylized.png
+-rw-rw-r--   0 tom       (1000) tom       (1000)      258 2021-12-26 21:21:06.000000 decoder-plus-plus-1.7.2/dpp/images/hidden.png
+-rw-rw-r--   0 tom       (1000) tom       (1000)      349 2022-09-13 21:04:47.000000 decoder-plus-plus-1.7.2/dpp/images/indicator_green.png
+-rw-rw-r--   0 tom       (1000) tom       (1000)      417 2022-09-13 21:05:13.000000 decoder-plus-plus-1.7.2/dpp/images/indicator_grey.png
+-rw-rw-r--   0 tom       (1000) tom       (1000)      319 2022-09-13 21:05:36.000000 decoder-plus-plus-1.7.2/dpp/images/indicator_red.png
+-rw-rw-r--   0 tom       (1000) tom       (1000)    11652 2021-12-26 21:21:06.000000 decoder-plus-plus-1.7.2/dpp/images/keyboard.png
+-rw-rw-r--   0 tom       (1000) tom       (1000)    27999 2021-12-26 21:21:06.000000 decoder-plus-plus-1.7.2/dpp/images/keyboard.svg
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-07 19:02:44.548739 decoder-plus-plus-1.7.2/dpp/plugins/
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1328 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.2/dpp/plugins/adler32_hasher.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1393 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.2/dpp/plugins/apache_md5_hasher.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1545 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.2/dpp/plugins/base16_decoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1545 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.2/dpp/plugins/base16_encoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1824 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.2/dpp/plugins/base32_decoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1529 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.2/dpp/plugins/base32_encoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1755 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.2/dpp/plugins/base45_decoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1482 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.2/dpp/plugins/base45_encoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2097 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.2/dpp/plugins/base64_decoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1470 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.2/dpp/plugins/base64_encoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2678 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.2/dpp/plugins/base64_url_decoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1693 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.2/dpp/plugins/base64_url_encoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1241 2022-09-17 09:11:33.000000 decoder-plus-plus-1.7.2/dpp/plugins/bin_int_decoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1249 2022-09-17 09:11:33.000000 decoder-plus-plus-1.7.2/dpp/plugins/bin_int_encoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1519 2022-09-17 09:11:33.000000 decoder-plus-plus-1.7.2/dpp/plugins/bin_str_decoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1695 2022-09-17 09:11:33.000000 decoder-plus-plus-1.7.2/dpp/plugins/bin_str_encoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     5641 2024-04-05 16:00:23.000000 decoder-plus-plus-1.7.2/dpp/plugins/caesar_cipher_script.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1065 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.2/dpp/plugins/clone_script.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1320 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.2/dpp/plugins/crc32_hasher.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1159 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.2/dpp/plugins/css_minify_script.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     5888 2024-04-06 15:56:04.000000 decoder-plus-plus-1.7.2/dpp/plugins/custom_code.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1475 2022-09-17 09:13:06.000000 decoder-plus-plus-1.7.2/dpp/plugins/dec_str_decoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1441 2022-09-17 09:13:12.000000 decoder-plus-plus-1.7.2/dpp/plugins/dec_str_encoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1068 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.2/dpp/plugins/escape_string_script.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1211 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.2/dpp/plugins/extract_urls_script.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     5143 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.2/dpp/plugins/filter_lines_script.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1386 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.2/dpp/plugins/free_bsd_nt_hasher.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1653 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.2/dpp/plugins/gzip_decoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1408 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.2/dpp/plugins/gzip_encoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2110 2022-11-01 18:01:29.000000 decoder-plus-plus-1.7.2/dpp/plugins/hex_char_decoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1582 2022-11-01 18:01:29.000000 decoder-plus-plus-1.7.2/dpp/plugins/hex_char_encoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1448 2022-11-01 18:01:29.000000 decoder-plus-plus-1.7.2/dpp/plugins/hex_int_decoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1217 2022-11-01 18:01:29.000000 decoder-plus-plus-1.7.2/dpp/plugins/hex_int_encoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2331 2022-11-01 18:01:29.000000 decoder-plus-plus-1.7.2/dpp/plugins/hex_shell_decoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1980 2022-11-01 18:01:29.000000 decoder-plus-plus-1.7.2/dpp/plugins/hex_shell_encoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1709 2022-11-01 18:01:29.000000 decoder-plus-plus-1.7.2/dpp/plugins/hex_str_decoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1561 2022-11-01 18:01:29.000000 decoder-plus-plus-1.7.2/dpp/plugins/hex_str_encoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1221 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.2/dpp/plugins/html_beautify_script.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1783 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.2/dpp/plugins/html_decoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1377 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.2/dpp/plugins/html_encoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1138 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.2/dpp/plugins/html_minify_script.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2539 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.2/dpp/plugins/http64_decoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1841 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.2/dpp/plugins/http64_encoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2265 2024-04-07 11:11:41.000000 decoder-plus-plus-1.7.2/dpp/plugins/identify_decoder_script.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1371 2024-04-07 11:16:17.000000 decoder-plus-plus-1.7.2/dpp/plugins/identify_file_type_filemagic_script.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1478 2024-04-07 11:16:17.000000 decoder-plus-plus-1.7.2/dpp/plugins/identify_file_type_magika_script.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1389 2024-04-07 11:03:59.000000 decoder-plus-plus-1.7.2/dpp/plugins/identify_hash_format_script.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2254 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.2/dpp/plugins/jq_script.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1336 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.2/dpp/plugins/js_beautify_script.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1131 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.2/dpp/plugins/js_minify_script.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1171 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.2/dpp/plugins/js_to_xml_script.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)    15185 2024-04-07 08:30:22.000000 decoder-plus-plus-1.7.2/dpp/plugins/jsonify_script.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2621 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.2/dpp/plugins/jsonpath_script.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2568 2024-04-07 18:47:41.000000 decoder-plus-plus-1.7.2/dpp/plugins/jwt_decoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2345 2024-04-07 18:56:21.000000 decoder-plus-plus-1.7.2/dpp/plugins/jwt_encoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1432 2022-09-15 16:34:02.000000 decoder-plus-plus-1.7.2/dpp/plugins/keccak224_hasher.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1440 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.2/dpp/plugins/keccak256_hasher.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1472 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.2/dpp/plugins/keccak384_hasher.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1519 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.2/dpp/plugins/keccak512_hasher.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1446 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.2/dpp/plugins/little_big_endian_script.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1366 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.2/dpp/plugins/lm_hasher.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1364 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.2/dpp/plugins/md2_hasher.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1364 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.2/dpp/plugins/md4_hasher.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1352 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.2/dpp/plugins/md5_hasher.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1366 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.2/dpp/plugins/nt_hasher.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1223 2022-09-17 09:11:33.000000 decoder-plus-plus-1.7.2/dpp/plugins/oct_int_decoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1228 2022-09-17 09:11:33.000000 decoder-plus-plus-1.7.2/dpp/plugins/oct_int_encoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1775 2022-09-17 09:11:33.000000 decoder-plus-plus-1.7.2/dpp/plugins/oct_str_decoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1576 2022-09-17 09:11:33.000000 decoder-plus-plus-1.7.2/dpp/plugins/oct_str_encoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1368 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.2/dpp/plugins/phpass_hasher.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     6590 2024-04-05 18:32:58.000000 decoder-plus-plus-1.7.2/dpp/plugins/reformat_text_script.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1115 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.2/dpp/plugins/remove_newlines_script.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1121 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.2/dpp/plugins/remove_whitespaces_script.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1693 2024-04-07 07:30:09.000000 decoder-plus-plus-1.7.2/dpp/plugins/ripemd160_hasher.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1398 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.2/dpp/plugins/rot13_decoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1398 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.2/dpp/plugins/rot13_encoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     4506 2024-04-05 18:32:58.000000 decoder-plus-plus-1.7.2/dpp/plugins/search_and_replace_script.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1363 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.2/dpp/plugins/sha1_hasher.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1401 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.2/dpp/plugins/sha224_hasher.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1409 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.2/dpp/plugins/sha256_hasher.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1441 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.2/dpp/plugins/sha384_hasher.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1382 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.2/dpp/plugins/sha3_224_hasher.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1383 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.2/dpp/plugins/sha3_256_hasher.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1415 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.2/dpp/plugins/sha3_384_hasher.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1462 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.2/dpp/plugins/sha3_512_hasher.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1474 2022-09-12 18:36:42.000000 decoder-plus-plus-1.7.2/dpp/plugins/sha512_hasher.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     4998 2024-04-05 18:32:58.000000 decoder-plus-plus-1.7.2/dpp/plugins/split_and_rejoin_script.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1400 2022-09-12 18:36:42.000000 decoder-plus-plus-1.7.2/dpp/plugins/sun_md5_hasher.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1107 2022-09-12 18:36:42.000000 decoder-plus-plus-1.7.2/dpp/plugins/unescape_string_script.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1993 2022-09-12 18:36:42.000000 decoder-plus-plus-1.7.2/dpp/plugins/url_decoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1487 2022-09-12 18:36:42.000000 decoder-plus-plus-1.7.2/dpp/plugins/url_encoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1974 2022-09-12 18:36:42.000000 decoder-plus-plus-1.7.2/dpp/plugins/url_plus_decoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1525 2022-09-12 18:36:42.000000 decoder-plus-plus-1.7.2/dpp/plugins/url_plus_encoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2291 2023-01-15 14:37:27.000000 decoder-plus-plus-1.7.2/dpp/plugins/xpath_script.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1821 2022-09-12 18:36:42.000000 decoder-plus-plus-1.7.2/dpp/plugins/zlib_decoder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1394 2022-09-12 18:36:42.000000 decoder-plus-plus-1.7.2/dpp/plugins/zlib_encoder.py
+-rwxrwxr-x   0 tom       (1000) tom       (1000)    16769 2022-09-21 05:00:04.000000 decoder-plus-plus-1.7.2/dpp/runner.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-07 19:02:44.548739 decoder-plus-plus-1.7.2/dpp/ui/
+-rw-rw-r--   0 tom       (1000) tom       (1000)      967 2022-09-06 05:50:59.000000 decoder-plus-plus-1.7.2/dpp/ui/__init__.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-07 19:02:44.548739 decoder-plus-plus-1.7.2/dpp/ui/builder/
+-rw-rw-r--   0 tom       (1000) tom       (1000)        0 2021-12-26 21:21:06.000000 decoder-plus-plus-1.7.2/dpp/ui/builder/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1962 2022-08-15 20:49:18.000000 decoder-plus-plus-1.7.2/dpp/ui/builder/action_builder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1547 2023-03-07 03:42:36.000000 decoder-plus-plus-1.7.2/dpp/ui/builder/input_text_builder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1682 2024-04-05 15:27:20.000000 decoder-plus-plus-1.7.2/dpp/ui/builder/plugin_config_widget_builder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)    10393 2024-04-07 07:53:50.000000 decoder-plus-plus-1.7.2/dpp/ui/builder/widget_builder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     6388 2023-01-29 15:44:47.000000 decoder-plus-plus-1.7.2/dpp/ui/decoder_plus_plus_gui.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-07 19:02:44.548739 decoder-plus-plus-1.7.2/dpp/ui/dialog/
+-rw-rw-r--   0 tom       (1000) tom       (1000)      706 2021-12-26 21:21:06.000000 decoder-plus-plus-1.7.2/dpp/ui/dialog/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     5833 2024-04-06 19:42:04.000000 decoder-plus-plus-1.7.2/dpp/ui/dialog/config_dialog.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     5273 2022-09-10 21:34:51.000000 decoder-plus-plus-1.7.2/dpp/ui/dialog/keyboard_shortcut_dialog.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     5810 2024-04-07 18:45:09.000000 decoder-plus-plus-1.7.2/dpp/ui/dialog/plugin_config_dialog.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-07 19:02:44.552739 decoder-plus-plus-1.7.2/dpp/ui/dock/
+-rw-rw-r--   0 tom       (1000) tom       (1000)        0 2021-12-26 21:21:06.000000 decoder-plus-plus-1.7.2/dpp/ui/dock/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)    10582 2023-02-28 12:28:51.000000 decoder-plus-plus-1.7.2/dpp/ui/dock/hex_dock.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)    12701 2022-09-12 19:05:02.000000 decoder-plus-plus-1.7.2/dpp/ui/dock/log_dock.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2564 2022-09-07 22:11:21.000000 decoder-plus-plus-1.7.2/dpp/ui/instance_handler.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-07 19:02:44.552739 decoder-plus-plus-1.7.2/dpp/ui/view/
+-rw-rw-r--   0 tom       (1000) tom       (1000)      706 2022-08-18 00:21:03.000000 decoder-plus-plus-1.7.2/dpp/ui/view/__init__.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-07 19:02:44.552739 decoder-plus-plus-1.7.2/dpp/ui/view/classic/
+-rw-rw-r--   0 tom       (1000) tom       (1000)      839 2022-08-20 19:51:05.000000 decoder-plus-plus-1.7.2/dpp/ui/view/classic/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)    10186 2024-04-06 16:14:35.000000 decoder-plus-plus-1.7.2/dpp/ui/view/classic/classic_main_window_widget.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)    16982 2024-04-07 13:12:43.000000 decoder-plus-plus-1.7.2/dpp/ui/view/classic/codec_frame.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)    13200 2022-09-15 16:14:00.000000 decoder-plus-plus-1.7.2/dpp/ui/view/classic/codec_frame_header.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)    20625 2024-04-07 18:07:00.000000 decoder-plus-plus-1.7.2/dpp/ui/view/classic/codec_frames.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2401 2022-09-20 04:28:03.000000 decoder-plus-plus-1.7.2/dpp/ui/view/classic/codec_tab.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     9167 2023-01-30 13:35:51.000000 decoder-plus-plus-1.7.2/dpp/ui/view/classic/combo_box_frame.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)    10716 2022-09-21 05:00:04.000000 decoder-plus-plus-1.7.2/dpp/ui/view/main_window_widget.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-07 19:02:44.552739 decoder-plus-plus-1.7.2/dpp/ui/view/modern/
+-rw-rw-r--   0 tom       (1000) tom       (1000)      705 2022-08-20 19:51:05.000000 decoder-plus-plus-1.7.2/dpp/ui/view/modern/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2460 2022-09-17 10:02:26.000000 decoder-plus-plus-1.7.2/dpp/ui/view/modern/modern_main_window_widget.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      705 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.2/dpp/ui/view/modern/node_data.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     5229 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.2/dpp/ui/view/modern/node_data_models.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      409 2022-08-30 00:07:08.000000 decoder-plus-plus-1.7.2/dpp/ui/view/modern/node_data_models_builder.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2001 2022-09-17 10:02:44.000000 decoder-plus-plus-1.7.2/dpp/ui/view/modern/node_editor.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1782 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.2/dpp/ui/view/modern/node_editor_tab.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-07 19:02:44.556739 decoder-plus-plus-1.7.2/dpp/ui/widget/
+-rw-rw-r--   0 tom       (1000) tom       (1000)      805 2022-08-16 19:35:20.000000 decoder-plus-plus-1.7.2/dpp/ui/widget/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1367 2022-08-15 23:02:30.000000 decoder-plus-plus-1.7.2/dpp/ui/widget/clickable_label.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     3507 2024-04-06 16:14:35.000000 decoder-plus-plus-1.7.2/dpp/ui/widget/code_editor_widget.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     3404 2024-04-07 09:41:34.000000 decoder-plus-plus-1.7.2/dpp/ui/widget/codec_preview_widget.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)    11051 2024-04-06 07:30:01.000000 decoder-plus-plus-1.7.2/dpp/ui/widget/collapsible_frame.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2161 2022-09-10 22:00:08.000000 decoder-plus-plus-1.7.2/dpp/ui/widget/combo_box.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     4686 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.2/dpp/ui/widget/dock_tabs_widget.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     7690 2022-08-20 19:51:05.000000 decoder-plus-plus-1.7.2/dpp/ui/widget/dock_widget.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1887 2022-08-15 20:48:14.000000 decoder-plus-plus-1.7.2/dpp/ui/widget/dyna_frame.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      755 2022-08-15 20:44:52.000000 decoder-plus-plus-1.7.2/dpp/ui/widget/elided_label.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2453 2024-04-06 20:17:41.000000 decoder-plus-plus-1.7.2/dpp/ui/widget/hover_label.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1793 2024-04-06 07:22:30.000000 decoder-plus-plus-1.7.2/dpp/ui/widget/icon_label.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     3270 2024-04-07 11:20:24.000000 decoder-plus-plus-1.7.2/dpp/ui/widget/identify_format_button.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     3269 2022-09-12 19:34:03.000000 decoder-plus-plus-1.7.2/dpp/ui/widget/list_widget.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1151 2022-08-21 00:18:15.000000 decoder-plus-plus-1.7.2/dpp/ui/widget/menu_bar.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2136 2024-04-06 09:24:31.000000 decoder-plus-plus-1.7.2/dpp/ui/widget/message_box_widget.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     6687 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.2/dpp/ui/widget/message_widget.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     6110 2024-04-06 15:44:53.000000 decoder-plus-plus-1.7.2/dpp/ui/widget/option_widgets.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)    16152 2023-03-14 08:16:41.000000 decoder-plus-plus-1.7.2/dpp/ui/widget/plain_view.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2621 2022-09-08 00:44:43.000000 decoder-plus-plus-1.7.2/dpp/ui/widget/plugin_frame.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     9593 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.2/dpp/ui/widget/plugin_tab.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     4396 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.2/dpp/ui/widget/search_field.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1246 2022-09-12 17:32:16.000000 decoder-plus-plus-1.7.2/dpp/ui/widget/separater_widget.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     5000 2022-08-15 23:02:30.000000 decoder-plus-plus-1.7.2/dpp/ui/widget/shortcut_table.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2846 2022-09-12 18:36:42.000000 decoder-plus-plus-1.7.2/dpp/ui/widget/slider_widget.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     4055 2022-09-20 10:34:13.000000 decoder-plus-plus-1.7.2/dpp/ui/widget/smart_decode_button.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1442 2022-09-12 18:36:42.000000 decoder-plus-plus-1.7.2/dpp/ui/widget/spacers.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2425 2023-01-30 12:23:56.000000 decoder-plus-plus-1.7.2/dpp/ui/widget/status_widget.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     3757 2022-08-20 19:51:05.000000 decoder-plus-plus-1.7.2/dpp/ui/widget/tab_bar.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     8075 2022-09-15 01:50:24.000000 decoder-plus-plus-1.7.2/dpp/ui/widget/tabs_widget.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     3210 2024-04-05 11:52:36.000000 decoder-plus-plus-1.7.2/dpp/ui/widget/text_widget.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)       38 2024-04-07 19:02:44.568739 decoder-plus-plus-1.7.2/setup.cfg
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2681 2024-04-07 18:40:37.000000 decoder-plus-plus-1.7.2/setup.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-07 19:02:44.556739 decoder-plus-plus-1.7.2/tests/
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1805 2023-01-15 14:31:34.000000 decoder-plus-plus-1.7.2/tests/__init__.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-07 19:02:44.568739 decoder-plus-plus-1.7.2/tests/plugins/
+-rw-rw-r--   0 tom       (1000) tom       (1000)        0 2022-11-01 13:33:59.000000 decoder-plus-plus-1.7.2/tests/plugins/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1113 2022-11-01 14:08:45.000000 decoder-plus-plus-1.7.2/tests/plugins/adler32_hasher_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1191 2022-11-01 18:50:27.000000 decoder-plus-plus-1.7.2/tests/plugins/apache_md5_hasher_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1295 2022-11-01 18:05:54.000000 decoder-plus-plus-1.7.2/tests/plugins/base16_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1680 2023-01-15 13:01:54.000000 decoder-plus-plus-1.7.2/tests/plugins/base32_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1287 2023-01-15 13:32:25.000000 decoder-plus-plus-1.7.2/tests/plugins/base45_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1288 2023-01-15 12:36:51.000000 decoder-plus-plus-1.7.2/tests/plugins/base64_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1474 2023-01-15 12:47:27.000000 decoder-plus-plus-1.7.2/tests/plugins/base64_url_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1229 2023-01-15 13:29:43.000000 decoder-plus-plus-1.7.2/tests/plugins/bin_int_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1040 2022-11-01 18:51:09.000000 decoder-plus-plus-1.7.2/tests/plugins/bin_str_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      992 2023-01-15 12:47:59.000000 decoder-plus-plus-1.7.2/tests/plugins/caesar_cipher_script_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1222 2022-11-01 18:35:38.000000 decoder-plus-plus-1.7.2/tests/plugins/clone_script_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1108 2023-01-15 12:37:31.000000 decoder-plus-plus-1.7.2/tests/plugins/crc32_hasher_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1183 2022-11-01 18:39:55.000000 decoder-plus-plus-1.7.2/tests/plugins/css_minify_script_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1401 2022-11-01 18:35:21.000000 decoder-plus-plus-1.7.2/tests/plugins/dec_str_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1245 2022-11-01 18:59:45.000000 decoder-plus-plus-1.7.2/tests/plugins/escape_string_script_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1123 2022-11-01 18:47:57.000000 decoder-plus-plus-1.7.2/tests/plugins/extract_urls_script_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1165 2022-11-01 18:40:22.000000 decoder-plus-plus-1.7.2/tests/plugins/filter_lines_script_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1189 2023-01-15 13:03:50.000000 decoder-plus-plus-1.7.2/tests/plugins/free_bsd_nt_hasher_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1253 2023-01-15 12:29:09.000000 decoder-plus-plus-1.7.2/tests/plugins/gzip_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1067 2022-11-01 18:47:18.000000 decoder-plus-plus-1.7.2/tests/plugins/hex_char_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1193 2023-01-15 13:10:42.000000 decoder-plus-plus-1.7.2/tests/plugins/hex_int_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1614 2022-11-01 18:43:06.000000 decoder-plus-plus-1.7.2/tests/plugins/hex_shell_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1313 2023-01-15 13:16:46.000000 decoder-plus-plus-1.7.2/tests/plugins/hex_str_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1173 2022-11-01 18:43:28.000000 decoder-plus-plus-1.7.2/tests/plugins/html_beautify_script_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1168 2022-11-01 18:48:47.000000 decoder-plus-plus-1.7.2/tests/plugins/html_minify_script_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1172 2023-01-15 12:22:31.000000 decoder-plus-plus-1.7.2/tests/plugins/html_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1219 2022-11-01 18:32:01.000000 decoder-plus-plus-1.7.2/tests/plugins/http64_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1016 2024-04-07 12:31:43.000000 decoder-plus-plus-1.7.2/tests/plugins/identify_file_type_filemagic_script_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1019 2024-04-07 12:32:46.000000 decoder-plus-plus-1.7.2/tests/plugins/identify_file_type_magika_script_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1108 2022-11-01 18:39:55.000000 decoder-plus-plus-1.7.2/tests/plugins/identify_hash_format_script_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1145 2023-01-15 13:26:35.000000 decoder-plus-plus-1.7.2/tests/plugins/jq_script_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      988 2023-01-15 12:41:00.000000 decoder-plus-plus-1.7.2/tests/plugins/js_beautify_script_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1164 2022-11-01 18:49:20.000000 decoder-plus-plus-1.7.2/tests/plugins/js_minify_script_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      977 2023-01-15 13:06:33.000000 decoder-plus-plus-1.7.2/tests/plugins/js_to_xml_script_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      981 2023-01-15 13:02:34.000000 decoder-plus-plus-1.7.2/tests/plugins/jsonify_script_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1163 2022-11-01 18:49:36.000000 decoder-plus-plus-1.7.2/tests/plugins/jsonpath_script_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      976 2023-01-15 12:39:55.000000 decoder-plus-plus-1.7.2/tests/plugins/jwt_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1163 2023-01-15 13:02:49.000000 decoder-plus-plus-1.7.2/tests/plugins/keccak224_hasher_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1171 2022-11-01 18:56:46.000000 decoder-plus-plus-1.7.2/tests/plugins/keccak256_hasher_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1203 2022-11-01 18:45:25.000000 decoder-plus-plus-1.7.2/tests/plugins/keccak384_hasher_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1235 2022-11-01 18:48:57.000000 decoder-plus-plus-1.7.2/tests/plugins/keccak512_hasher_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1245 2022-11-01 18:31:13.000000 decoder-plus-plus-1.7.2/tests/plugins/little_big_endian_script_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1124 2022-11-01 18:56:24.000000 decoder-plus-plus-1.7.2/tests/plugins/lm_hasher_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1126 2022-11-01 18:24:14.000000 decoder-plus-plus-1.7.2/tests/plugins/md2_hasher_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1126 2022-11-01 18:56:15.000000 decoder-plus-plus-1.7.2/tests/plugins/md4_hasher_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1126 2022-11-01 18:45:18.000000 decoder-plus-plus-1.7.2/tests/plugins/md5_hasher_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1124 2022-11-01 18:46:24.000000 decoder-plus-plus-1.7.2/tests/plugins/nt_hasher_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1193 2023-01-15 13:13:49.000000 decoder-plus-plus-1.7.2/tests/plugins/oct_int_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1405 2022-11-01 18:20:57.000000 decoder-plus-plus-1.7.2/tests/plugins/oct_str_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1181 2023-01-15 12:51:06.000000 decoder-plus-plus-1.7.2/tests/plugins/phpass_hasher_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1167 2022-11-01 18:57:07.000000 decoder-plus-plus-1.7.2/tests/plugins/reformat_text_script_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1187 2023-01-15 13:04:21.000000 decoder-plus-plus-1.7.2/tests/plugins/remove_newlines_script_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1064 2022-11-01 18:56:04.000000 decoder-plus-plus-1.7.2/tests/plugins/remove_whitespaces_script_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1146 2022-11-01 18:56:36.000000 decoder-plus-plus-1.7.2/tests/plugins/ripemd160_hasher_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1225 2022-11-01 18:26:44.000000 decoder-plus-plus-1.7.2/tests/plugins/rot13_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1503 2023-01-15 13:05:35.000000 decoder-plus-plus-1.7.2/tests/plugins/search_and_replace_script_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1136 2022-11-01 18:27:54.000000 decoder-plus-plus-1.7.2/tests/plugins/sha1_hasher_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1192 2022-11-01 18:29:14.000000 decoder-plus-plus-1.7.2/tests/plugins/sha224_hasher_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1200 2022-11-01 18:29:35.000000 decoder-plus-plus-1.7.2/tests/plugins/sha256_hasher_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1231 2022-11-01 18:29:59.000000 decoder-plus-plus-1.7.2/tests/plugins/sha384_hasher_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1160 2023-01-15 12:37:21.000000 decoder-plus-plus-1.7.2/tests/plugins/sha3_224_hasher_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1168 2022-11-01 18:53:45.000000 decoder-plus-plus-1.7.2/tests/plugins/sha3_256_hasher_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1200 2022-11-01 18:28:35.000000 decoder-plus-plus-1.7.2/tests/plugins/sha3_384_hasher_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1268 2022-11-01 18:28:57.000000 decoder-plus-plus-1.7.2/tests/plugins/sha3_512_hasher_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1263 2022-11-01 18:30:17.000000 decoder-plus-plus-1.7.2/tests/plugins/sha512_hasher_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1170 2022-11-01 18:57:46.000000 decoder-plus-plus-1.7.2/tests/plugins/split_and_rejoin_script_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      983 2023-01-15 12:39:55.000000 decoder-plus-plus-1.7.2/tests/plugins/sun_md5_hasher_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1247 2022-11-01 18:32:56.000000 decoder-plus-plus-1.7.2/tests/plugins/unescape_string_script_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1282 2022-11-01 18:45:08.000000 decoder-plus-plus-1.7.2/tests/plugins/url_plus_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1136 2022-11-01 18:53:35.000000 decoder-plus-plus-1.7.2/tests/plugins/url_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1136 2023-01-15 14:38:44.000000 decoder-plus-plus-1.7.2/tests/plugins/xpath_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1223 2023-01-15 13:12:30.000000 decoder-plus-plus-1.7.2/tests/plugins/zlib_test.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-07 19:02:44.568739 decoder-plus-plus-1.7.2/tests/ui/
+-rw-rw-r--   0 tom       (1000) tom       (1000)        0 2023-01-15 14:39:42.000000 decoder-plus-plus-1.7.2/tests/ui/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)    10085 2024-04-07 18:07:00.000000 decoder-plus-plus-1.7.2/tests/ui/classic_mode_test.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      512 2023-01-15 15:28:09.000000 decoder-plus-plus-1.7.2/tests/utils.py
```

### Comparing `decoder-plus-plus-1.7.1/LICENSE` & `decoder-plus-plus-1.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/PKG-INFO` & `decoder-plus-plus-1.7.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: decoder-plus-plus
-Version: 1.7.1
+Version: 1.7.2
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
-Metadata-Version: 2.1 Name: decoder-plus-plus Version: 1.7.1 Summary: An
+Metadata-Version: 2.1 Name: decoder-plus-plus Version: 1.7.2 Summary: An
 extensible application for penetration testers and software developers to
 decode/encode data into various formats. Home-page: https://github.com/
 bytebutcher/decoder-plus-plus Author: bytebutcher Author-email:
 thomas.engel.web@gmail.com License: GPL-3.0 Classifier: Programming Language ::
 Python :: 3 Classifier: Operating System :: OS Independent Description-Content-
 Type: text/markdown Provides-Extra: qt5 Provides-Extra: qt6 Provides-Extra:
 extras Provides-Extra: test License-File: LICENSE ![Decoder++ Logo](https://
```

### Comparing `decoder-plus-plus-1.7.1/README.md` & `decoder-plus-plus-1.7.2/README.md`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/data/dpp.png` & `decoder-plus-plus-1.7.2/data/dpp.png`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/decoder_plus_plus.egg-info/PKG-INFO` & `decoder-plus-plus-1.7.2/decoder_plus_plus.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: decoder-plus-plus
-Version: 1.7.1
+Version: 1.7.2
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
-Metadata-Version: 2.1 Name: decoder-plus-plus Version: 1.7.1 Summary: An
+Metadata-Version: 2.1 Name: decoder-plus-plus Version: 1.7.2 Summary: An
 extensible application for penetration testers and software developers to
 decode/encode data into various formats. Home-page: https://github.com/
 bytebutcher/decoder-plus-plus Author: bytebutcher Author-email:
 thomas.engel.web@gmail.com License: GPL-3.0 Classifier: Programming Language ::
 Python :: 3 Classifier: Operating System :: OS Independent Description-Content-
 Type: text/markdown Provides-Extra: qt5 Provides-Extra: qt6 Provides-Extra:
 extras Provides-Extra: test License-File: LICENSE ![Decoder++ Logo](https://
```

### Comparing `decoder-plus-plus-1.7.1/decoder_plus_plus.egg-info/SOURCES.txt` & `decoder-plus-plus-1.7.2/decoder_plus_plus.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -101,14 +101,15 @@
 dpp/plugins/jq_script.py
 dpp/plugins/js_beautify_script.py
 dpp/plugins/js_minify_script.py
 dpp/plugins/js_to_xml_script.py
 dpp/plugins/jsonify_script.py
 dpp/plugins/jsonpath_script.py
 dpp/plugins/jwt_decoder.py
+dpp/plugins/jwt_encoder.py
 dpp/plugins/keccak224_hasher.py
 dpp/plugins/keccak256_hasher.py
 dpp/plugins/keccak384_hasher.py
 dpp/plugins/keccak512_hasher.py
 dpp/plugins/little_big_endian_script.py
 dpp/plugins/lm_hasher.py
 dpp/plugins/md2_hasher.py
```

### Comparing `decoder-plus-plus-1.7.1/dpp/__init__.py` & `decoder-plus-plus-1.7.2/dpp/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,12 +12,12 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 __name__ = 'decoder-plus-plus'
-__version__ = '1.7.1'
+__version__ = '1.7.2'
 __author__ = 'bytebutcher'
 
 import os
 app_path = os.path.dirname(os.path.abspath(__file__))
```

### Comparing `decoder-plus-plus-1.7.1/dpp/core/__init__.py` & `decoder-plus-plus-1.7.2/dpp/core/__init__.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/core/argparse.py` & `decoder-plus-plus-1.7.2/dpp/core/argparse.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/core/assertions.py` & `decoder-plus-plus-1.7.2/dpp/core/assertions.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/core/config.py` & `decoder-plus-plus-1.7.2/dpp/core/config.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/core/context.py` & `decoder-plus-plus-1.7.2/dpp/core/context.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/core/decoder_plus_plus.py` & `decoder-plus-plus-1.7.2/dpp/core/decoder_plus_plus.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/core/exceptions.py` & `decoder-plus-plus-1.7.2/dpp/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/core/icons.py` & `decoder-plus-plus-1.7.2/dpp/core/icons.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/core/listener.py` & `decoder-plus-plus-1.7.2/dpp/core/listener.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/core/logger.py` & `decoder-plus-plus-1.7.2/dpp/core/logger.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/core/math.py` & `decoder-plus-plus-1.7.2/dpp/core/math.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/core/plugin/__init__.py` & `decoder-plus-plus-1.7.2/dpp/core/plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/core/plugin/builder.py` & `decoder-plus-plus-1.7.2/dpp/core/plugin/builder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/core/plugin/config/__init__.py` & `decoder-plus-plus-1.7.2/dpp/core/plugin/config/__init__.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/core/plugin/config/options/__init__.py` & `decoder-plus-plus-1.7.2/dpp/core/plugin/config/options/__init__.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/core/plugin/config/ui/__init__.py` & `decoder-plus-plus-1.7.2/dpp/core/plugin/config/ui/__init__.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/core/plugin/config/ui/layouts.py` & `decoder-plus-plus-1.7.2/dpp/core/plugin/config/ui/layouts.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/core/plugin/config/ui/widgets.py` & `decoder-plus-plus-1.7.2/dpp/core/plugin/config/ui/widgets.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/core/plugin/loader.py` & `decoder-plus-plus-1.7.2/dpp/core/plugin/loader.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/core/plugin/manager.py` & `decoder-plus-plus-1.7.2/dpp/core/plugin/manager.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/core/shortcuts.py` & `decoder-plus-plus-1.7.2/dpp/core/shortcuts.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/images/dpp.png` & `decoder-plus-plus-1.7.2/dpp/images/dpp.png`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/images/dpp_128.png` & `decoder-plus-plus-1.7.2/dpp/images/dpp_128.png`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/images/dpp_classic.png` & `decoder-plus-plus-1.7.2/dpp/images/dpp_classic.png`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/images/dpp_classic_128.png` & `decoder-plus-plus-1.7.2/dpp/images/dpp_classic_128.png`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/images/dpp_modern.png` & `decoder-plus-plus-1.7.2/dpp/images/dpp_modern.png`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/images/dpp_modern_128.png` & `decoder-plus-plus-1.7.2/dpp/images/dpp_modern_128.png`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/images/dpp_modern_big.png` & `decoder-plus-plus-1.7.2/dpp/images/dpp_modern_big.png`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/images/dpp_stylized.png` & `decoder-plus-plus-1.7.2/dpp/images/dpp_stylized.png`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/images/dpp_stylized_128.png` & `decoder-plus-plus-1.7.2/dpp/images/dpp_stylized_128.png`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/images/dpp_xmas.png` & `decoder-plus-plus-1.7.2/dpp/images/dpp_xmas.png`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/images/dpp_xmas_stylized.png` & `decoder-plus-plus-1.7.2/dpp/images/dpp_xmas_stylized.png`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/images/keyboard.png` & `decoder-plus-plus-1.7.2/dpp/images/keyboard.png`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/images/keyboard.svg` & `decoder-plus-plus-1.7.2/dpp/images/keyboard.svg`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/plugins/adler32_hasher.py` & `decoder-plus-plus-1.7.2/dpp/plugins/adler32_hasher.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/plugins/apache_md5_hasher.py` & `decoder-plus-plus-1.7.2/dpp/plugins/apache_md5_hasher.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/plugins/base16_decoder.py` & `decoder-plus-plus-1.7.2/dpp/plugins/base16_decoder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/plugins/base16_encoder.py` & `decoder-plus-plus-1.7.2/dpp/plugins/base16_encoder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/plugins/base32_decoder.py` & `decoder-plus-plus-1.7.2/dpp/plugins/base32_decoder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/plugins/base32_encoder.py` & `decoder-plus-plus-1.7.2/dpp/plugins/base32_encoder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/plugins/base45_decoder.py` & `decoder-plus-plus-1.7.2/dpp/plugins/base45_decoder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/plugins/base45_encoder.py` & `decoder-plus-plus-1.7.2/dpp/plugins/base45_encoder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/plugins/base64_decoder.py` & `decoder-plus-plus-1.7.2/dpp/plugins/base64_decoder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/plugins/base64_encoder.py` & `decoder-plus-plus-1.7.2/dpp/plugins/base64_encoder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/plugins/base64_url_decoder.py` & `decoder-plus-plus-1.7.2/dpp/plugins/base64_url_decoder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/plugins/base64_url_encoder.py` & `decoder-plus-plus-1.7.2/dpp/plugins/base64_url_encoder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/plugins/bin_int_decoder.py` & `decoder-plus-plus-1.7.2/dpp/plugins/bin_int_decoder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/plugins/bin_int_encoder.py` & `decoder-plus-plus-1.7.2/dpp/plugins/bin_int_encoder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/plugins/bin_str_decoder.py` & `decoder-plus-plus-1.7.2/dpp/plugins/bin_str_decoder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/plugins/bin_str_encoder.py` & `decoder-plus-plus-1.7.2/dpp/plugins/bin_str_encoder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/plugins/caesar_cipher_script.py` & `decoder-plus-plus-1.7.2/dpp/plugins/caesar_cipher_script.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/plugins/clone_script.py` & `decoder-plus-plus-1.7.2/dpp/plugins/clone_script.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/plugins/crc32_hasher.py` & `decoder-plus-plus-1.7.2/dpp/plugins/crc32_hasher.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/plugins/css_minify_script.py` & `decoder-plus-plus-1.7.2/dpp/plugins/css_minify_script.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/plugins/custom_code.py` & `decoder-plus-plus-1.7.2/dpp/plugins/custom_code.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/plugins/dec_str_decoder.py` & `decoder-plus-plus-1.7.2/dpp/plugins/dec_str_decoder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/plugins/dec_str_encoder.py` & `decoder-plus-plus-1.7.2/dpp/plugins/dec_str_encoder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/plugins/escape_string_script.py` & `decoder-plus-plus-1.7.2/dpp/plugins/escape_string_script.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/plugins/extract_urls_script.py` & `decoder-plus-plus-1.7.2/dpp/plugins/extract_urls_script.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/plugins/filter_lines_script.py` & `decoder-plus-plus-1.7.2/dpp/plugins/filter_lines_script.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/plugins/free_bsd_nt_hasher.py` & `decoder-plus-plus-1.7.2/dpp/plugins/free_bsd_nt_hasher.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/plugins/gzip_decoder.py` & `decoder-plus-plus-1.7.2/dpp/plugins/gzip_decoder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/plugins/gzip_encoder.py` & `decoder-plus-plus-1.7.2/dpp/plugins/gzip_encoder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/plugins/hex_char_decoder.py` & `decoder-plus-plus-1.7.2/dpp/plugins/hex_char_decoder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/plugins/hex_char_encoder.py` & `decoder-plus-plus-1.7.2/dpp/plugins/hex_char_encoder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/plugins/hex_int_decoder.py` & `decoder-plus-plus-1.7.2/dpp/plugins/hex_int_decoder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/plugins/hex_int_encoder.py` & `decoder-plus-plus-1.7.2/dpp/plugins/hex_int_encoder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/plugins/hex_shell_decoder.py` & `decoder-plus-plus-1.7.2/dpp/plugins/hex_shell_decoder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/plugins/hex_shell_encoder.py` & `decoder-plus-plus-1.7.2/dpp/plugins/hex_shell_encoder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/plugins/hex_str_decoder.py` & `decoder-plus-plus-1.7.2/dpp/plugins/hex_str_decoder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/plugins/hex_str_encoder.py` & `decoder-plus-plus-1.7.2/dpp/plugins/hex_str_encoder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/plugins/html_beautify_script.py` & `decoder-plus-plus-1.7.2/dpp/plugins/html_beautify_script.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/plugins/html_decoder.py` & `decoder-plus-plus-1.7.2/dpp/plugins/html_decoder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/plugins/html_encoder.py` & `decoder-plus-plus-1.7.2/dpp/plugins/html_encoder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/plugins/html_minify_script.py` & `decoder-plus-plus-1.7.2/dpp/plugins/html_minify_script.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/plugins/http64_decoder.py` & `decoder-plus-plus-1.7.2/dpp/plugins/http64_decoder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/plugins/http64_encoder.py` & `decoder-plus-plus-1.7.2/dpp/plugins/http64_encoder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/plugins/identify_decoder_script.py` & `decoder-plus-plus-1.7.2/dpp/plugins/identify_decoder_script.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/plugins/identify_file_type_filemagic_script.py` & `decoder-plus-plus-1.7.2/dpp/plugins/identify_file_type_filemagic_script.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/plugins/identify_file_type_magika_script.py` & `decoder-plus-plus-1.7.2/dpp/plugins/identify_file_type_magika_script.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/plugins/identify_hash_format_script.py` & `decoder-plus-plus-1.7.2/dpp/plugins/identify_hash_format_script.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/plugins/jq_script.py` & `decoder-plus-plus-1.7.2/dpp/plugins/jq_script.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/plugins/js_beautify_script.py` & `decoder-plus-plus-1.7.2/dpp/plugins/js_beautify_script.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/plugins/js_minify_script.py` & `decoder-plus-plus-1.7.2/dpp/plugins/js_minify_script.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/plugins/js_to_xml_script.py` & `decoder-plus-plus-1.7.2/dpp/plugins/js_to_xml_script.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/plugins/jsonify_script.py` & `decoder-plus-plus-1.7.2/dpp/plugins/jsonify_script.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/plugins/jsonpath_script.py` & `decoder-plus-plus-1.7.2/dpp/plugins/jsonpath_script.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/plugins/jwt_decoder.py` & `decoder-plus-plus-1.7.2/dpp/plugins/sha512_hasher.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,39 +10,34 @@
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
-from dpp.core.plugin import DecoderPlugin
+from dpp.core.plugin import HasherPlugin
 
 
-class Plugin(DecoderPlugin):
+class Plugin(HasherPlugin):
     """
-    Decodes JSON Web Tokens.
+    Hashes a string using SHA512.
 
     Example:
 
         Input:
-            eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJzb21lIjoicGF5bG9hZCJ9.4twFt5NiznN84AWoo1d7KO1T_yoc0Z6XOpOVswacPZg
+            abcdefghijklmnopqrstuvwxyz
+            ^°!"§$%&/()=?´`<>| ,.-;:_#+'*~
+            0123456789
 
         Output:
-            {'some': 'payload'}
+            58cd501bee1ece7411a23b2e86bfb795b136f2aae5d8f94a59c551622d9a0d7e \\
+            293a04a8584244eadf1f9bedd34cbcb7e99f7bdedaac56591f88bb282c5146cd
+
     """
 
     def __init__(self, context: 'dpp.core.context.Context'):
         # Name, Author, Dependencies
-        super().__init__('JWT', "Thomas Engel", ["jwt"], context)
+        super().__init__('SHA512', "Thomas Engel", ["hashlib"], context)
 
     def run(self, input_text: str) -> str:
-        import jwt
-        return str(jwt.decode(input_text.encode('utf-8', errors='surrogateescape'), verify=False))
-
-    def can_decode_input(self, input_text: str) -> bool:
-        if input_text and input_text.startswith("ey"):
-            try:
-                self.run(input_text)
-                return True
-            except:
-                return False
-        return False
+        import hashlib
+        return hashlib.sha512(input_text.encode('utf-8', errors='surrogateescape')).hexdigest()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `decoder-plus-plus-1.7.1/dpp/plugins/keccak224_hasher.py` & `decoder-plus-plus-1.7.2/dpp/plugins/keccak224_hasher.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/plugins/keccak256_hasher.py` & `decoder-plus-plus-1.7.2/dpp/plugins/keccak256_hasher.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/plugins/keccak384_hasher.py` & `decoder-plus-plus-1.7.2/dpp/plugins/keccak384_hasher.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/plugins/keccak512_hasher.py` & `decoder-plus-plus-1.7.2/dpp/plugins/keccak512_hasher.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/plugins/little_big_endian_script.py` & `decoder-plus-plus-1.7.2/dpp/plugins/little_big_endian_script.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/plugins/lm_hasher.py` & `decoder-plus-plus-1.7.2/dpp/plugins/lm_hasher.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/plugins/md2_hasher.py` & `decoder-plus-plus-1.7.2/dpp/plugins/md2_hasher.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/plugins/md4_hasher.py` & `decoder-plus-plus-1.7.2/dpp/plugins/md4_hasher.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/plugins/md5_hasher.py` & `decoder-plus-plus-1.7.2/dpp/plugins/md5_hasher.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/plugins/nt_hasher.py` & `decoder-plus-plus-1.7.2/dpp/plugins/nt_hasher.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/plugins/oct_int_decoder.py` & `decoder-plus-plus-1.7.2/dpp/plugins/oct_int_decoder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/plugins/oct_int_encoder.py` & `decoder-plus-plus-1.7.2/dpp/plugins/oct_int_encoder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/plugins/oct_str_decoder.py` & `decoder-plus-plus-1.7.2/dpp/plugins/oct_str_decoder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/plugins/oct_str_encoder.py` & `decoder-plus-plus-1.7.2/dpp/plugins/oct_str_encoder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/plugins/phpass_hasher.py` & `decoder-plus-plus-1.7.2/dpp/plugins/phpass_hasher.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/plugins/reformat_text_script.py` & `decoder-plus-plus-1.7.2/dpp/plugins/reformat_text_script.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/plugins/remove_newlines_script.py` & `decoder-plus-plus-1.7.2/dpp/plugins/remove_newlines_script.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/plugins/remove_whitespaces_script.py` & `decoder-plus-plus-1.7.2/dpp/plugins/remove_whitespaces_script.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/plugins/ripemd160_hasher.py` & `decoder-plus-plus-1.7.2/dpp/plugins/ripemd160_hasher.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/plugins/rot13_decoder.py` & `decoder-plus-plus-1.7.2/dpp/plugins/rot13_decoder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/plugins/rot13_encoder.py` & `decoder-plus-plus-1.7.2/dpp/plugins/rot13_encoder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/plugins/search_and_replace_script.py` & `decoder-plus-plus-1.7.2/dpp/plugins/search_and_replace_script.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/plugins/sha1_hasher.py` & `decoder-plus-plus-1.7.2/dpp/plugins/sha1_hasher.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/plugins/sha224_hasher.py` & `decoder-plus-plus-1.7.2/dpp/plugins/sha224_hasher.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/plugins/sha256_hasher.py` & `decoder-plus-plus-1.7.2/dpp/plugins/sha256_hasher.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/plugins/sha384_hasher.py` & `decoder-plus-plus-1.7.2/dpp/plugins/sha384_hasher.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/plugins/sha3_224_hasher.py` & `decoder-plus-plus-1.7.2/dpp/plugins/sha3_224_hasher.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/plugins/sha3_256_hasher.py` & `decoder-plus-plus-1.7.2/dpp/plugins/sha3_256_hasher.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/plugins/sha3_384_hasher.py` & `decoder-plus-plus-1.7.2/dpp/plugins/sha3_384_hasher.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/plugins/sha3_512_hasher.py` & `decoder-plus-plus-1.7.2/dpp/plugins/sha3_512_hasher.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/plugins/sha512_hasher.py` & `decoder-plus-plus-1.7.2/dpp/plugins/url_encoder.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,34 +10,34 @@
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
-from dpp.core.plugin import HasherPlugin
+from dpp.core.plugin import EncoderPlugin
 
 
-class Plugin(HasherPlugin):
+class Plugin(EncoderPlugin):
     """
-    Hashes a string using SHA512.
+    Encodes a string to an URL.
 
     Example:
 
         Input:
             abcdefghijklmnopqrstuvwxyz
             ^°!"§$%&/()=?´`<>| ,.-;:_#+'*~
             0123456789
 
         Output:
-            58cd501bee1ece7411a23b2e86bfb795b136f2aae5d8f94a59c551622d9a0d7e \\
-            293a04a8584244eadf1f9bedd34cbcb7e99f7bdedaac56591f88bb282c5146cd
-
+            abcdefghijklmnopqrstuvwxyz \\
+            %0A%5E%C2%B0%21%22%C2%A7%24%25%26/%28%29%3D%3F%C2%B4%60%3C%3E%7C%20%2C.-%3B%3A_%23%2B%27%2A%7E%0A \\
+            0123456789
     """
 
     def __init__(self, context: 'dpp.core.context.Context'):
         # Name, Author, Dependencies
-        super().__init__('SHA512', "Thomas Engel", ["hashlib"], context)
+        super().__init__('URL', "Thomas Engel", ["urllib"], context)
 
     def run(self, input_text: str) -> str:
-        import hashlib
-        return hashlib.sha512(input_text.encode('utf-8', errors='surrogateescape')).hexdigest()
+        import urllib.parse
+        return urllib.parse.quote(input_text.encode('utf-8', errors='surrogateescape'))
```

### Comparing `decoder-plus-plus-1.7.1/dpp/plugins/split_and_rejoin_script.py` & `decoder-plus-plus-1.7.2/dpp/plugins/split_and_rejoin_script.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/plugins/sun_md5_hasher.py` & `decoder-plus-plus-1.7.2/dpp/plugins/sun_md5_hasher.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/plugins/unescape_string_script.py` & `decoder-plus-plus-1.7.2/dpp/plugins/unescape_string_script.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/plugins/url_decoder.py` & `decoder-plus-plus-1.7.2/dpp/plugins/url_decoder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/plugins/url_encoder.py` & `decoder-plus-plus-1.7.2/dpp/plugins/url_plus_encoder.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,29 +15,29 @@
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 from dpp.core.plugin import EncoderPlugin
 
 
 class Plugin(EncoderPlugin):
     """
-    Encodes a string to an URL.
+    Encodes a string to an URL. Spaces are encoded to plus-signs.
 
     Example:
 
         Input:
             abcdefghijklmnopqrstuvwxyz
             ^°!"§$%&/()=?´`<>| ,.-;:_#+'*~
             0123456789
 
         Output:
             abcdefghijklmnopqrstuvwxyz \\
-            %0A%5E%C2%B0%21%22%C2%A7%24%25%26/%28%29%3D%3F%C2%B4%60%3C%3E%7C%20%2C.-%3B%3A_%23%2B%27%2A%7E%0A \\
+            %0A%5E%C2%B0%21%22%C2%A7%24%25%26/%28%29%3D%3F%C2%B4%60%3C%3E%7C+%2C.-%3B%3A_%23%2B%27%2A%7E%0A \\
             0123456789
     """
 
     def __init__(self, context: 'dpp.core.context.Context'):
         # Name, Author, Dependencies
-        super().__init__('URL', "Thomas Engel", ["urllib"], context)
+        super().__init__('URL+', "Thomas Engel", ["urllib"], context)
 
     def run(self, input_text: str) -> str:
         import urllib.parse
-        return urllib.parse.quote(input_text.encode('utf-8', errors='surrogateescape'))
+        return urllib.parse.quote_plus(input_text.encode('utf-8', errors='surrogateescape'))
```

### Comparing `decoder-plus-plus-1.7.1/dpp/plugins/url_plus_decoder.py` & `decoder-plus-plus-1.7.2/dpp/plugins/url_plus_decoder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/plugins/url_plus_encoder.py` & `decoder-plus-plus-1.7.2/dpp/plugins/zlib_decoder.py`

 * *Files 22% similar despite different names*

```diff
@@ -10,34 +10,44 @@
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
-from dpp.core.plugin import EncoderPlugin
+from dpp.core.plugin import DecoderPlugin
 
 
-class Plugin(EncoderPlugin):
+class Plugin(DecoderPlugin):
     """
-    Encodes a string to an URL. Spaces are encoded to plus-signs.
+    Decodes bytes using ZLib.
 
     Example:
 
         Input:
-            abcdefghijklmnopqrstuvwxyz
-            ^°!"§$%&/()=?´`<>| ,.-;:_#+'*~
-            0123456789
+            [bytes]
 
         Output:
-            abcdefghijklmnopqrstuvwxyz \\
-            %0A%5E%C2%B0%21%22%C2%A7%24%25%26/%28%29%3D%3F%C2%B4%60%3C%3E%7C+%2C.-%3B%3A_%23%2B%27%2A%7E%0A \\
+            abcdefghijklmnopqrstuvwxyz
+            ^°!"§$%&/()=?´`<>| ,.-;:_#+'*~
             0123456789
     """
 
     def __init__(self, context: 'dpp.core.context.Context'):
         # Name, Author, Dependencies
-        super().__init__('URL+', "Thomas Engel", ["urllib"], context)
+        super().__init__('Zlib', "Thomas Engel", ["zlib"], context)
 
     def run(self, input_text: str) -> str:
-        import urllib.parse
-        return urllib.parse.quote_plus(input_text.encode('utf-8', errors='surrogateescape'))
+        import zlib
+        return zlib.decompress(input_text.encode('utf-8', errors='surrogateescape'))\
+            .decode('utf-8', errors='surrogateescape')
+
+    def can_decode_input(self, input_text: str) -> bool:
+        if input_text:
+            input_bytes = input_text.encode('utf-8', errors='surrogateescape')
+            if len(input_bytes) > 2:
+                return (input_bytes[0] == 0x78) and (input_bytes[1] in (
+                    0x01, # No Compression/Low
+                    0x9c, # Default Compression
+                    0xda  # Best Compression
+                ))
+        return False
```

### Comparing `decoder-plus-plus-1.7.1/dpp/plugins/xpath_script.py` & `decoder-plus-plus-1.7.2/dpp/plugins/xpath_script.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/plugins/zlib_decoder.py` & `decoder-plus-plus-1.7.2/dpp/plugins/zlib_encoder.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,44 +10,32 @@
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
-from dpp.core.plugin import DecoderPlugin
+from dpp.core.plugin import EncoderPlugin
 
 
-class Plugin(DecoderPlugin):
+class Plugin(EncoderPlugin):
     """
-    Decodes bytes using ZLib.
+        Encodes a string using ZLib.
 
-    Example:
+        Example:
 
-        Input:
-            [bytes]
-
-        Output:
-            abcdefghijklmnopqrstuvwxyz
-            ^°!"§$%&/()=?´`<>| ,.-;:_#+'*~
-            0123456789
-    """
+            Input:
+                abcdefghijklmnopqrstuvwxyz
+                ^°!"§$%&/()=?´`<>| ,.-;:_#+'*~
+                0123456789
+
+            Output:
+                [bytes]
+        """
 
     def __init__(self, context: 'dpp.core.context.Context'):
         # Name, Author, Dependencies
         super().__init__('Zlib', "Thomas Engel", ["zlib"], context)
 
     def run(self, input_text: str) -> str:
         import zlib
-        return zlib.decompress(input_text.encode('utf-8', errors='surrogateescape'))\
-            .decode('utf-8', errors='surrogateescape')
-
-    def can_decode_input(self, input_text: str) -> bool:
-        if input_text:
-            input_bytes = input_text.encode('utf-8', errors='surrogateescape')
-            if len(input_bytes) > 2:
-                return (input_bytes[0] == 0x78) and (input_bytes[1] in (
-                    0x01, # No Compression/Low
-                    0x9c, # Default Compression
-                    0xda  # Best Compression
-                ))
-        return False
+        return zlib.compress(input_text.encode('utf-8', errors='surrogateescape')).decode('utf-8', errors='surrogateescape')
```

### Comparing `decoder-plus-plus-1.7.1/dpp/plugins/zlib_encoder.py` & `decoder-plus-plus-1.7.2/tests/plugins/base32_test.py`

 * *Files 24% similar despite different names*

```diff
@@ -10,32 +10,33 @@
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
-from dpp.core.plugin import EncoderPlugin
+import unittest
 
+from dpp.core.plugin import PluginType
+from tests.utils import load_plugin
 
-class Plugin(EncoderPlugin):
-    """
-        Encodes a string using ZLib.
 
-        Example:
+class TestBase32Encoder(unittest.TestCase):
+    encoder = load_plugin("Base32", PluginType.ENCODER)
+    decoder = load_plugin("Base32", PluginType.DECODER)
 
-            Input:
-                abcdefghijklmnopqrstuvwxyz
-                ^°!"§$%&/()=?´`<>| ,.-;:_#+'*~
-                0123456789
+    def testEncoder(self):
+        input_text = 'abcdefghijklmnopqrstuvwxyz\n^°!"§$%&/()=?´`<>| ,.-;:_#+\'*~\n0123456789'
+        output_text = 'MFRGGZDFMZTWQ2LKNNWG23TPOBYXE43UOV3HO6DZPIFF5QVQEERMFJZEEUTC6KBJHU74FNDAHQ7HYIBMFYWTWOS7EMVSOKT6BIYDCMRTGQ2TMNZYHE======'
 
-            Output:
-                [bytes]
-        """
+        self.assertEqual(self.encoder.run(
+            input_text
+        ), output_text)
 
-    def __init__(self, context: 'dpp.core.context.Context'):
-        # Name, Author, Dependencies
-        super().__init__('Zlib', "Thomas Engel", ["zlib"], context)
 
-    def run(self, input_text: str) -> str:
-        import zlib
-        return zlib.compress(input_text.encode('utf-8', errors='surrogateescape')).decode('utf-8', errors='surrogateescape')
+    def testDecoder(self):
+        input_text = 'MFRGGZDFMZTWQ2LKNNWG23TPOBYXE43UOV3HO6DZPIFF5QVQEERMFJZEEUTC6KBJHU74FNDAHQ7HYIBMFYWTWOS7EMVSOKT6BIYDCMRTGQ2TMNZYHE======'
+        output_text = 'abcdefghijklmnopqrstuvwxyz\n^°!"§$%&/()=?´`<>| ,.-;:_#+\'*~\n0123456789'
+
+        self.assertEqual(self.decoder.run(
+            input_text
+        ), output_text)
```

### Comparing `decoder-plus-plus-1.7.1/dpp/runner.py` & `decoder-plus-plus-1.7.2/dpp/runner.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/ui/__init__.py` & `decoder-plus-plus-1.7.2/dpp/ui/__init__.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/ui/builder/action_builder.py` & `decoder-plus-plus-1.7.2/dpp/ui/builder/action_builder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/ui/builder/input_text_builder.py` & `decoder-plus-plus-1.7.2/dpp/ui/builder/input_text_builder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/ui/builder/plugin_config_widget_builder.py` & `decoder-plus-plus-1.7.2/dpp/ui/builder/plugin_config_widget_builder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/ui/builder/widget_builder.py` & `decoder-plus-plus-1.7.2/dpp/ui/builder/widget_builder.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/ui/decoder_plus_plus_gui.py` & `decoder-plus-plus-1.7.2/dpp/ui/decoder_plus_plus_gui.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/ui/dialog/__init__.py` & `decoder-plus-plus-1.7.2/dpp/ui/dialog/__init__.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/ui/dialog/config_dialog.py` & `decoder-plus-plus-1.7.2/dpp/ui/dialog/config_dialog.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/ui/dialog/keyboard_shortcut_dialog.py` & `decoder-plus-plus-1.7.2/dpp/ui/dialog/keyboard_shortcut_dialog.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/ui/dialog/plugin_config_dialog.py` & `decoder-plus-plus-1.7.2/dpp/ui/dialog/plugin_config_dialog.py`

 * *Files 6% similar despite different names*

```diff
@@ -103,35 +103,32 @@
         try:
             self._plugin_clone.validate_options(input_text, option_keys)
         except BaseException as err:
             self._show_error_message(str(err))
 
     def _hide_message_box(self):
         """ Hide message box and enable OK button. """
-        self._btn_box.button(QDialogButtonBox.Ok).setEnabled(True)
         self._message_box.setHidden(True)
 
     def _show_error_message(self, message):
         """ Shows an error message within a message-box. """
         if not message:
             self._hide_message_box()
             return
-        self._btn_box.button(QDialogButtonBox.Ok).setEnabled(False)
         self._message_box.setFrameStyle("background-color: black;")
         self._message_box.setTextStyle("QLabel { color: white }")
         self._message_box.setIcon(Icon.MSG_ERROR, color='red')
         self._message_box.setText(message)
         self._message_box.setHidden(False)
         self._context.logger.debug(message)
 
     def _show_success_message(self, message):
         """ Shows a success message within a message box. """
         if not message:
             self._hide_message_box()
             return
-        self._btn_box.button(QDialogButtonBox.Ok).setEnabled(True)
         self._message_box.setFrameStyle("background-color: white;")
         self._message_box.setTextStyle("QLabel { color: black }")
         self._message_box.setIcon(Icon.MSG_INFO, color='blue')
         self._message_box.setText(message)
         self._message_box.setHidden(False)
         self._context.logger.debug(message)
```

### Comparing `decoder-plus-plus-1.7.1/dpp/ui/dock/hex_dock.py` & `decoder-plus-plus-1.7.2/dpp/ui/dock/hex_dock.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/ui/dock/log_dock.py` & `decoder-plus-plus-1.7.2/dpp/ui/dock/log_dock.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/ui/instance_handler.py` & `decoder-plus-plus-1.7.2/dpp/ui/instance_handler.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/ui/view/__init__.py` & `decoder-plus-plus-1.7.2/dpp/ui/view/__init__.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/ui/view/classic/__init__.py` & `decoder-plus-plus-1.7.2/dpp/ui/view/classic/__init__.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/ui/view/classic/classic_main_window_widget.py` & `decoder-plus-plus-1.7.2/dpp/ui/view/classic/classic_main_window_widget.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/ui/view/classic/codec_frame.py` & `decoder-plus-plus-1.7.2/dpp/ui/view/classic/codec_frame.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/ui/view/classic/codec_frame_header.py` & `decoder-plus-plus-1.7.2/dpp/ui/view/classic/codec_frame_header.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/ui/view/classic/codec_frames.py` & `decoder-plus-plus-1.7.2/dpp/ui/view/classic/codec_frames.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/ui/view/classic/codec_tab.py` & `decoder-plus-plus-1.7.2/dpp/ui/view/classic/codec_tab.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/ui/view/classic/combo_box_frame.py` & `decoder-plus-plus-1.7.2/dpp/ui/view/classic/combo_box_frame.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/ui/view/main_window_widget.py` & `decoder-plus-plus-1.7.2/dpp/ui/view/main_window_widget.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/ui/view/modern/__init__.py` & `decoder-plus-plus-1.7.2/dpp/ui/view/modern/__init__.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/ui/view/modern/modern_main_window_widget.py` & `decoder-plus-plus-1.7.2/dpp/ui/view/modern/modern_main_window_widget.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/ui/view/modern/node_data.py` & `decoder-plus-plus-1.7.2/dpp/ui/view/modern/node_data.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/ui/view/modern/node_data_models.py` & `decoder-plus-plus-1.7.2/dpp/ui/view/modern/node_data_models.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/ui/view/modern/node_editor.py` & `decoder-plus-plus-1.7.2/dpp/ui/view/modern/node_editor.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/ui/view/modern/node_editor_tab.py` & `decoder-plus-plus-1.7.2/dpp/ui/view/modern/node_editor_tab.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/ui/widget/__init__.py` & `decoder-plus-plus-1.7.2/dpp/ui/widget/__init__.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/ui/widget/clickable_label.py` & `decoder-plus-plus-1.7.2/dpp/ui/widget/clickable_label.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/ui/widget/code_editor_widget.py` & `decoder-plus-plus-1.7.2/dpp/ui/widget/code_editor_widget.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/ui/widget/codec_preview_widget.py` & `decoder-plus-plus-1.7.2/dpp/ui/widget/codec_preview_widget.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/ui/widget/collapsible_frame.py` & `decoder-plus-plus-1.7.2/dpp/ui/widget/collapsible_frame.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/ui/widget/combo_box.py` & `decoder-plus-plus-1.7.2/dpp/ui/widget/combo_box.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/ui/widget/dock_tabs_widget.py` & `decoder-plus-plus-1.7.2/dpp/ui/widget/dock_tabs_widget.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/ui/widget/dock_widget.py` & `decoder-plus-plus-1.7.2/dpp/ui/widget/dock_widget.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/ui/widget/dyna_frame.py` & `decoder-plus-plus-1.7.2/dpp/ui/widget/dyna_frame.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/ui/widget/elided_label.py` & `decoder-plus-plus-1.7.2/dpp/ui/widget/elided_label.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/ui/widget/hover_label.py` & `decoder-plus-plus-1.7.2/dpp/ui/widget/hover_label.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/ui/widget/icon_label.py` & `decoder-plus-plus-1.7.2/dpp/ui/widget/icon_label.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/ui/widget/identify_format_button.py` & `decoder-plus-plus-1.7.2/dpp/ui/widget/identify_format_button.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/ui/widget/list_widget.py` & `decoder-plus-plus-1.7.2/dpp/ui/widget/list_widget.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/ui/widget/menu_bar.py` & `decoder-plus-plus-1.7.2/dpp/ui/widget/menu_bar.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/ui/widget/message_box_widget.py` & `decoder-plus-plus-1.7.2/dpp/ui/widget/message_box_widget.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/ui/widget/message_widget.py` & `decoder-plus-plus-1.7.2/dpp/ui/widget/message_widget.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/ui/widget/option_widgets.py` & `decoder-plus-plus-1.7.2/dpp/ui/widget/option_widgets.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/ui/widget/plain_view.py` & `decoder-plus-plus-1.7.2/dpp/ui/widget/plain_view.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/ui/widget/plugin_frame.py` & `decoder-plus-plus-1.7.2/dpp/ui/widget/plugin_frame.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/ui/widget/plugin_tab.py` & `decoder-plus-plus-1.7.2/dpp/ui/widget/plugin_tab.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/ui/widget/search_field.py` & `decoder-plus-plus-1.7.2/dpp/ui/widget/search_field.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/ui/widget/separater_widget.py` & `decoder-plus-plus-1.7.2/dpp/ui/widget/separater_widget.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/ui/widget/shortcut_table.py` & `decoder-plus-plus-1.7.2/dpp/ui/widget/shortcut_table.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/ui/widget/slider_widget.py` & `decoder-plus-plus-1.7.2/dpp/ui/widget/slider_widget.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/ui/widget/smart_decode_button.py` & `decoder-plus-plus-1.7.2/dpp/ui/widget/smart_decode_button.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/ui/widget/spacers.py` & `decoder-plus-plus-1.7.2/dpp/ui/widget/spacers.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/ui/widget/status_widget.py` & `decoder-plus-plus-1.7.2/dpp/ui/widget/status_widget.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/ui/widget/tab_bar.py` & `decoder-plus-plus-1.7.2/dpp/ui/widget/tab_bar.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/ui/widget/tabs_widget.py` & `decoder-plus-plus-1.7.2/dpp/ui/widget/tabs_widget.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/dpp/ui/widget/text_widget.py` & `decoder-plus-plus-1.7.2/dpp/ui/widget/text_widget.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/setup.py` & `decoder-plus-plus-1.7.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,15 @@
             'base45>=0.4.0',
             'css-html-js-minify>=2.5.0',
             'pycryptodome>=3.15.0',
             'jc>=1.21.0',
             'jsbeautifier>=1.14.0',
             'json2xml>=3.19.0',
             'jsonpath_ng>=1.5.0',
-            'jwt>=1.3.0',
+            'PyJWT>=2.8.0',
             'magika>=0.5.0',
             'passlib>=1.7.0',
             'pycryptodome>=3.15.0',
             'validators>=0.20.0'
         ],
         'test': [
             'pytest-qt>=4.2.0',
```

### Comparing `decoder-plus-plus-1.7.1/tests/__init__.py` & `decoder-plus-plus-1.7.2/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/tests/plugins/adler32_hasher_test.py` & `decoder-plus-plus-1.7.2/tests/plugins/adler32_hasher_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/tests/plugins/apache_md5_hasher_test.py` & `decoder-plus-plus-1.7.2/tests/plugins/apache_md5_hasher_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/tests/plugins/base16_test.py` & `decoder-plus-plus-1.7.2/tests/plugins/base16_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/tests/plugins/base32_test.py` & `decoder-plus-plus-1.7.2/tests/plugins/oct_str_test.py`

 * *Files 26% similar despite different names*

```diff
@@ -16,27 +16,24 @@
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 import unittest
 
 from dpp.core.plugin import PluginType
 from tests.utils import load_plugin
 
 
-class TestBase32Encoder(unittest.TestCase):
-    encoder = load_plugin("Base32", PluginType.ENCODER)
-    decoder = load_plugin("Base32", PluginType.DECODER)
+class TestOctStrEncoder(unittest.TestCase):
 
-    def testEncoder(self):
-        input_text = 'abcdefghijklmnopqrstuvwxyz\n^°!"§$%&/()=?´`<>| ,.-;:_#+\'*~\n0123456789'
-        output_text = 'MFRGGZDFMZTWQ2LKNNWG23TPOBYXE43UOV3HO6DZPIFF5QVQEERMFJZEEUTC6KBJHU74FNDAHQ7HYIBMFYWTWOS7EMVSOKT6BIYDCMRTGQ2TMNZYHE======'
+    plugin = load_plugin("Oct (str)", PluginType.ENCODER)
 
-        self.assertEqual(self.encoder.run(
-            input_text
-        ), output_text)
-
-
-    def testDecoder(self):
-        input_text = 'MFRGGZDFMZTWQ2LKNNWG23TPOBYXE43UOV3HO6DZPIFF5QVQEERMFJZEEUTC6KBJHU74FNDAHQ7HYIBMFYWTWOS7EMVSOKT6BIYDCMRTGQ2TMNZYHE======'
-        output_text = 'abcdefghijklmnopqrstuvwxyz\n^°!"§$%&/()=?´`<>| ,.-;:_#+\'*~\n0123456789'
-
-        self.assertEqual(self.decoder.run(
-            input_text
-        ), output_text)
+    def testPlugin(self):
+        self.assertEqual(self.plugin.run(
+            'abcdefghijklmnopqrstuvwxyz\n'
+            '^°!"§$%&/()=?´`<>| ,.-;:_#+\'*~\n'
+            '0123456789'
+        ),
+            '1411421431441451461471501511521531'
+            '5415515615716016116216316416516616'
+            '7170171172012136260041042247044045'
+            '0460570500510750772641400740761740'
+            '4005405605507307213704305304705217'
+            '6012060061062063064065066067070071'
+        )
```

### Comparing `decoder-plus-plus-1.7.1/tests/plugins/base45_test.py` & `decoder-plus-plus-1.7.2/tests/plugins/base45_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/tests/plugins/base64_test.py` & `decoder-plus-plus-1.7.2/tests/plugins/base64_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/tests/plugins/base64_url_test.py` & `decoder-plus-plus-1.7.2/tests/plugins/base64_url_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/tests/plugins/bin_int_test.py` & `decoder-plus-plus-1.7.2/tests/plugins/bin_int_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/tests/plugins/bin_str_test.py` & `decoder-plus-plus-1.7.2/tests/plugins/bin_str_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/tests/plugins/caesar_cipher_script_test.py` & `decoder-plus-plus-1.7.2/tests/plugins/caesar_cipher_script_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/tests/plugins/clone_script_test.py` & `decoder-plus-plus-1.7.2/tests/plugins/clone_script_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/tests/plugins/crc32_hasher_test.py` & `decoder-plus-plus-1.7.2/tests/plugins/crc32_hasher_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/tests/plugins/css_minify_script_test.py` & `decoder-plus-plus-1.7.2/tests/plugins/css_minify_script_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/tests/plugins/dec_str_test.py` & `decoder-plus-plus-1.7.2/tests/plugins/dec_str_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/tests/plugins/escape_string_script_test.py` & `decoder-plus-plus-1.7.2/tests/plugins/escape_string_script_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/tests/plugins/extract_urls_script_test.py` & `decoder-plus-plus-1.7.2/tests/plugins/extract_urls_script_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/tests/plugins/filter_lines_script_test.py` & `decoder-plus-plus-1.7.2/tests/plugins/filter_lines_script_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/tests/plugins/free_bsd_nt_hasher_test.py` & `decoder-plus-plus-1.7.2/tests/plugins/free_bsd_nt_hasher_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/tests/plugins/gzip_test.py` & `decoder-plus-plus-1.7.2/tests/plugins/gzip_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/tests/plugins/hex_char_test.py` & `decoder-plus-plus-1.7.2/tests/plugins/hex_char_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/tests/plugins/hex_int_test.py` & `decoder-plus-plus-1.7.2/tests/plugins/hex_int_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/tests/plugins/hex_shell_test.py` & `decoder-plus-plus-1.7.2/tests/plugins/hex_shell_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/tests/plugins/hex_str_test.py` & `decoder-plus-plus-1.7.2/tests/plugins/hex_str_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/tests/plugins/html_beautify_script_test.py` & `decoder-plus-plus-1.7.2/tests/plugins/html_beautify_script_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/tests/plugins/html_minify_script_test.py` & `decoder-plus-plus-1.7.2/tests/plugins/html_minify_script_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/tests/plugins/html_test.py` & `decoder-plus-plus-1.7.2/tests/plugins/html_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/tests/plugins/http64_test.py` & `decoder-plus-plus-1.7.2/tests/plugins/http64_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/tests/plugins/identify_file_type_filemagic_script_test.py` & `decoder-plus-plus-1.7.2/tests/plugins/identify_file_type_filemagic_script_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/tests/plugins/identify_file_type_magika_script_test.py` & `decoder-plus-plus-1.7.2/tests/plugins/identify_file_type_magika_script_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/tests/plugins/identify_hash_format_script_test.py` & `decoder-plus-plus-1.7.2/tests/plugins/identify_hash_format_script_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/tests/plugins/jq_script_test.py` & `decoder-plus-plus-1.7.2/tests/plugins/jq_script_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/tests/plugins/js_beautify_script_test.py` & `decoder-plus-plus-1.7.2/tests/plugins/js_beautify_script_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/tests/plugins/js_minify_script_test.py` & `decoder-plus-plus-1.7.2/tests/plugins/js_minify_script_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/tests/plugins/js_to_xml_script_test.py` & `decoder-plus-plus-1.7.2/tests/plugins/js_to_xml_script_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/tests/plugins/jsonify_script_test.py` & `decoder-plus-plus-1.7.2/tests/plugins/jsonify_script_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/tests/plugins/jsonpath_script_test.py` & `decoder-plus-plus-1.7.2/tests/plugins/jsonpath_script_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/tests/plugins/jwt_test.py` & `decoder-plus-plus-1.7.2/tests/plugins/jwt_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/tests/plugins/keccak224_hasher_test.py` & `decoder-plus-plus-1.7.2/tests/plugins/keccak224_hasher_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/tests/plugins/keccak256_hasher_test.py` & `decoder-plus-plus-1.7.2/tests/plugins/keccak256_hasher_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/tests/plugins/keccak384_hasher_test.py` & `decoder-plus-plus-1.7.2/tests/plugins/keccak384_hasher_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/tests/plugins/keccak512_hasher_test.py` & `decoder-plus-plus-1.7.2/tests/plugins/keccak512_hasher_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/tests/plugins/little_big_endian_script_test.py` & `decoder-plus-plus-1.7.2/tests/plugins/little_big_endian_script_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/tests/plugins/lm_hasher_test.py` & `decoder-plus-plus-1.7.2/tests/plugins/lm_hasher_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/tests/plugins/md2_hasher_test.py` & `decoder-plus-plus-1.7.2/tests/plugins/md2_hasher_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/tests/plugins/md4_hasher_test.py` & `decoder-plus-plus-1.7.2/tests/plugins/md4_hasher_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/tests/plugins/md5_hasher_test.py` & `decoder-plus-plus-1.7.2/tests/plugins/md5_hasher_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/tests/plugins/nt_hasher_test.py` & `decoder-plus-plus-1.7.2/tests/plugins/nt_hasher_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/tests/plugins/oct_int_test.py` & `decoder-plus-plus-1.7.2/tests/plugins/oct_int_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/tests/plugins/oct_str_test.py` & `decoder-plus-plus-1.7.2/tests/plugins/sha3_512_hasher_test.py`

 * *Files 25% similar despite different names*

```diff
@@ -16,24 +16,20 @@
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 import unittest
 
 from dpp.core.plugin import PluginType
 from tests.utils import load_plugin
 
 
-class TestOctStrEncoder(unittest.TestCase):
+class TestSHA3_512Hasher(unittest.TestCase):
 
-    plugin = load_plugin("Oct (str)", PluginType.ENCODER)
+    plugin = load_plugin("SHA3 512", PluginType.HASHER)
 
     def testPlugin(self):
         self.assertEqual(self.plugin.run(
             'abcdefghijklmnopqrstuvwxyz\n'
             '^°!"§$%&/()=?´`<>| ,.-;:_#+\'*~\n'
             '0123456789'
         ),
-            '1411421431441451461471501511521531'
-            '5415515615716016116216316416516616'
-            '7170171172012136260041042247044045'
-            '0460570500510750772641400740761740'
-            '4005405605507307213704305304705217'
-            '6012060061062063064065066067070071'
+            '82ca87f576cadb05d4c911f36c98ed2735f45cad359d6ef5f6d544f5a3210e3e'
+            'cf080be15e539e23c15e2eb23054677d8a015ee56be2d9673c9f187d290906ed'
         )
```

### Comparing `decoder-plus-plus-1.7.1/tests/plugins/phpass_hasher_test.py` & `decoder-plus-plus-1.7.2/tests/plugins/phpass_hasher_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/tests/plugins/reformat_text_script_test.py` & `decoder-plus-plus-1.7.2/tests/plugins/reformat_text_script_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/tests/plugins/remove_newlines_script_test.py` & `decoder-plus-plus-1.7.2/tests/plugins/remove_newlines_script_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/tests/plugins/remove_whitespaces_script_test.py` & `decoder-plus-plus-1.7.2/tests/plugins/remove_whitespaces_script_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/tests/plugins/ripemd160_hasher_test.py` & `decoder-plus-plus-1.7.2/tests/plugins/ripemd160_hasher_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/tests/plugins/rot13_test.py` & `decoder-plus-plus-1.7.2/tests/plugins/rot13_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/tests/plugins/search_and_replace_script_test.py` & `decoder-plus-plus-1.7.2/tests/plugins/search_and_replace_script_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/tests/plugins/sha1_hasher_test.py` & `decoder-plus-plus-1.7.2/tests/plugins/sha1_hasher_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/tests/plugins/sha224_hasher_test.py` & `decoder-plus-plus-1.7.2/tests/plugins/sha224_hasher_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/tests/plugins/sha256_hasher_test.py` & `decoder-plus-plus-1.7.2/tests/plugins/sha256_hasher_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/tests/plugins/sha384_hasher_test.py` & `decoder-plus-plus-1.7.2/tests/plugins/sha384_hasher_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/tests/plugins/sha3_224_hasher_test.py` & `decoder-plus-plus-1.7.2/tests/plugins/sha3_224_hasher_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/tests/plugins/sha3_256_hasher_test.py` & `decoder-plus-plus-1.7.2/tests/plugins/sha3_256_hasher_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/tests/plugins/sha3_384_hasher_test.py` & `decoder-plus-plus-1.7.2/tests/plugins/sha3_384_hasher_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/tests/plugins/sha3_512_hasher_test.py` & `decoder-plus-plus-1.7.2/tests/plugins/url_plus_test.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,20 +16,20 @@
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 import unittest
 
 from dpp.core.plugin import PluginType
 from tests.utils import load_plugin
 
 
-class TestSHA3_512Hasher(unittest.TestCase):
-
-    plugin = load_plugin("SHA3 512", PluginType.HASHER)
+class TestURLPlusDecoder(unittest.TestCase):
+    plugin = load_plugin("URL+", PluginType.DECODER)
 
     def testPlugin(self):
         self.assertEqual(self.plugin.run(
+            'abcdefghijklmnopqrstuvwxyz'
+            '%0A%5E%C2%B0%21%22%C2%A7%24%25%26/%28%29%3D%3F%C2%B4%60%3C%3E%7C+%2C.-%3B%3A_%23%2B%27%2A%7E%0A'
+            '0123456789'
+        ),
             'abcdefghijklmnopqrstuvwxyz\n'
             '^°!"§$%&/()=?´`<>| ,.-;:_#+\'*~\n'
             '0123456789'
-        ),
-            '82ca87f576cadb05d4c911f36c98ed2735f45cad359d6ef5f6d544f5a3210e3e'
-            'cf080be15e539e23c15e2eb23054677d8a015ee56be2d9673c9f187d290906ed'
         )
```

### Comparing `decoder-plus-plus-1.7.1/tests/plugins/sha512_hasher_test.py` & `decoder-plus-plus-1.7.2/tests/plugins/sha512_hasher_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/tests/plugins/split_and_rejoin_script_test.py` & `decoder-plus-plus-1.7.2/tests/plugins/split_and_rejoin_script_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/tests/plugins/sun_md5_hasher_test.py` & `decoder-plus-plus-1.7.2/tests/plugins/sun_md5_hasher_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/tests/plugins/unescape_string_script_test.py` & `decoder-plus-plus-1.7.2/tests/plugins/unescape_string_script_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/tests/plugins/url_plus_test.py` & `decoder-plus-plus-1.7.2/tests/plugins/url_test.py`

 * *Files 22% similar despite different names*

```diff
@@ -16,20 +16,17 @@
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 import unittest
 
 from dpp.core.plugin import PluginType
 from tests.utils import load_plugin
 
 
-class TestURLPlusDecoder(unittest.TestCase):
-    plugin = load_plugin("URL+", PluginType.DECODER)
+class TestURLEncoder(unittest.TestCase):
+
+    plugin = load_plugin("URL", PluginType.ENCODER)
 
     def testPlugin(self):
         self.assertEqual(self.plugin.run(
-            'abcdefghijklmnopqrstuvwxyz'
-            '%0A%5E%C2%B0%21%22%C2%A7%24%25%26/%28%29%3D%3F%C2%B4%60%3C%3E%7C+%2C.-%3B%3A_%23%2B%27%2A%7E%0A'
-            '0123456789'
+            '^°!"§$%&/()=?´`<>| ,.-;:_#+\'*~'
         ),
-            'abcdefghijklmnopqrstuvwxyz\n'
-            '^°!"§$%&/()=?´`<>| ,.-;:_#+\'*~\n'
-            '0123456789'
+            '%5E%C2%B0%21%22%C2%A7%24%25%26/%28%29%3D%3F%C2%B4%60%3C%3E%7C%20%2C.-%3B%3A_%23%2B%27%2A~'
         )
```

### Comparing `decoder-plus-plus-1.7.1/tests/plugins/url_test.py` & `decoder-plus-plus-1.7.2/tests/plugins/xpath_test.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,17 +16,18 @@
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 import unittest
 
 from dpp.core.plugin import PluginType
 from tests.utils import load_plugin
 
 
-class TestURLEncoder(unittest.TestCase):
-
-    plugin = load_plugin("URL", PluginType.ENCODER)
+class TestXPathScript(unittest.TestCase):
+    plugin = load_plugin("XPath", PluginType.SCRIPT)
 
+    @unittest.skip("Missing configuration")
     def testPlugin(self):
+        self.plugin.setup({
+            'xpath_expression', '//b'
+        })
         self.assertEqual(self.plugin.run(
-            '^°!"§$%&/()=?´`<>| ,.-;:_#+\'*~'
-        ),
-            '%5E%C2%B0%21%22%C2%A7%24%25%26/%28%29%3D%3F%C2%B4%60%3C%3E%7C%20%2C.-%3B%3A_%23%2B%27%2A~'
-        )
+            '<a><b>text</b></a>'
+        ), 'text')
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `decoder-plus-plus-1.7.1/tests/plugins/xpath_test.py` & `decoder-plus-plus-1.7.2/tests/plugins/zlib_test.py`

 * *Files 24% similar despite different names*

```diff
@@ -16,18 +16,20 @@
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 import unittest
 
 from dpp.core.plugin import PluginType
 from tests.utils import load_plugin
 
 
-class TestXPathScript(unittest.TestCase):
-    plugin = load_plugin("XPath", PluginType.SCRIPT)
+class TestZLibDecoder(unittest.TestCase):
 
-    @unittest.skip("Missing configuration")
-    def testPlugin(self):
-        self.plugin.setup({
-            'xpath_expression', '//b'
-        })
-        self.assertEqual(self.plugin.run(
-            '<a><b>text</b></a>'
-        ), 'text')
+    encoder = load_plugin("ZLib", PluginType.DECODER)
+    decoder = load_plugin("ZLib", PluginType.DECODER)
+
+    @unittest.skip("decode(encode(text)) != text")
+    def testEncodeDecode(self):
+        input_text = 'abcdefghijklmnopqrstuvwxyz\n'
+        self.assertEqual(self.decoder.run(
+            self.encoder.run(
+                input_text
+            )
+        ), input_text)
```

### Comparing `decoder-plus-plus-1.7.1/tests/ui/classic_mode_test.py` & `decoder-plus-plus-1.7.2/tests/ui/classic_mode_test.py`

 * *Files identical despite different names*

### Comparing `decoder-plus-plus-1.7.1/tests/utils.py` & `decoder-plus-plus-1.7.2/tests/utils.py`

 * *Files identical despite different names*

