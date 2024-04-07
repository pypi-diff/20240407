# Comparing `tmp/japanese_address_parser_py-0.1.0b11.tar.gz` & `tmp/japanese_address_parser_py-0.1.0b12.tar.gz`

## Comparing `japanese_address_parser_py-0.1.0b11.tar` & `japanese_address_parser_py-0.1.0b12.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0     1001      127      706 2024-03-31 08:00:39.000000 japanese_address_parser_py-0.1.0b11/core/Cargo.toml
--rw-r--r--   0     1001      127     1065 2024-03-31 08:00:39.000000 japanese_address_parser_py-0.1.0b11/core/LICENSE
--rw-r--r--   0     1001      127     4410 2024-03-31 08:00:39.000000 japanese_address_parser_py-0.1.0b11/core/src/api/city_master_api.rs
--rw-r--r--   0     1001      127     4915 2024-03-31 08:00:39.000000 japanese_address_parser_py-0.1.0b11/core/src/api/prefecture_master_api.rs
--rw-r--r--   0     1001      127     2775 2024-03-31 08:00:39.000000 japanese_address_parser_py-0.1.0b11/core/src/api.rs
--rw-r--r--   0     1001      127     1794 2024-03-31 08:00:39.000000 japanese_address_parser_py-0.1.0b11/core/src/entity.rs
--rw-r--r--   0     1001      127     1326 2024-03-31 08:00:39.000000 japanese_address_parser_py-0.1.0b11/core/src/err.rs
--rw-r--r--   0     1001      127       64 2024-03-31 08:00:39.000000 japanese_address_parser_py-0.1.0b11/core/src/lib.rs
--rw-r--r--   0     1001      127     3131 2024-03-31 08:00:39.000000 japanese_address_parser_py-0.1.0b11/core/src/parser/adapter/orthographical_variant_adapter.rs
--rw-r--r--   0     1001      127       40 2024-03-31 08:00:39.000000 japanese_address_parser_py-0.1.0b11/core/src/parser/adapter.rs
--rw-r--r--   0     1001      127      570 2024-03-31 08:00:39.000000 japanese_address_parser_py-0.1.0b11/core/src/parser/filter/fullwidth_character.rs
--rw-r--r--   0     1001      127     7292 2024-03-31 08:00:39.000000 japanese_address_parser_py-0.1.0b11/core/src/parser/filter/invalid_town_name_format.rs
--rw-r--r--   0     1001      127     3393 2024-03-31 08:00:39.000000 japanese_address_parser_py-0.1.0b11/core/src/parser/filter/non_kanji_block_number.rs
--rw-r--r--   0     1001      127      162 2024-03-31 08:00:39.000000 japanese_address_parser_py-0.1.0b11/core/src/parser/filter.rs
--rw-r--r--   0     1001      127     3078 2024-03-31 08:00:39.000000 japanese_address_parser_py-0.1.0b11/core/src/parser/read_city.rs
--rw-r--r--   0     1001      127     2293 2024-03-31 08:00:39.000000 japanese_address_parser_py-0.1.0b11/core/src/parser/read_house_number.rs
--rw-r--r--   0     1001      127     1739 2024-03-31 08:00:39.000000 japanese_address_parser_py-0.1.0b11/core/src/parser/read_prefecture.rs
--rw-r--r--   0     1001      127     7124 2024-03-31 08:00:39.000000 japanese_address_parser_py-0.1.0b11/core/src/parser/read_town.rs
--rw-r--r--   0     1001      127     9275 2024-03-31 08:00:39.000000 japanese_address_parser_py-0.1.0b11/core/src/parser.rs
--rw-r--r--   0     1001      127     3695 2024-03-31 08:00:39.000000 japanese_address_parser_py-0.1.0b11/core/src/util/converter.rs
--rw-r--r--   0     1001      127       19 2024-03-31 08:00:39.000000 japanese_address_parser_py-0.1.0b11/core/src/util.rs
--rw-r--r--   0     1001      127     2826 2024-03-31 08:00:39.000000 japanese_address_parser_py-0.1.0b11/README.md
--rw-r--r--   0        0        0      464 1970-01-01 00:00:00.000000 japanese_address_parser_py-0.1.0b11/python/Cargo.toml
--rw-r--r--   0     1001      127     3282 2024-03-31 08:00:39.000000 japanese_address_parser_py-0.1.0b11/python/README.md
--rw-r--r--   0     1001      127     1426 2024-03-31 08:00:39.000000 japanese_address_parser_py-0.1.0b11/python/src/lib.rs
--rw-r--r--   0     1001      127    35516 2024-03-31 08:00:54.000000 japanese_address_parser_py-0.1.0b11/Cargo.lock
--rw-r--r--   0        0        0      507 1970-01-01 00:00:00.000000 japanese_address_parser_py-0.1.0b11/Cargo.toml
--rw-r--r--   0        0        0      346 1970-01-01 00:00:00.000000 japanese_address_parser_py-0.1.0b11/pyproject.toml
--rw-r--r--   0        0        0     3785 1970-01-01 00:00:00.000000 japanese_address_parser_py-0.1.0b11/PKG-INFO
+-rw-r--r--   0     1001      127      729 2024-04-07 07:30:00.000000 japanese_address_parser_py-0.1.0b12/core/Cargo.toml
+-rw-r--r--   0     1001      127     1065 2024-04-07 07:30:00.000000 japanese_address_parser_py-0.1.0b12/core/LICENSE
+-rw-r--r--   0     1001      127     4410 2024-04-07 07:30:00.000000 japanese_address_parser_py-0.1.0b12/core/src/api/city_master_api.rs
+-rw-r--r--   0     1001      127     4915 2024-04-07 07:30:00.000000 japanese_address_parser_py-0.1.0b12/core/src/api/prefecture_master_api.rs
+-rw-r--r--   0     1001      127     2775 2024-04-07 07:30:00.000000 japanese_address_parser_py-0.1.0b12/core/src/api.rs
+-rw-r--r--   0     1001      127     1794 2024-04-07 07:30:00.000000 japanese_address_parser_py-0.1.0b12/core/src/entity.rs
+-rw-r--r--   0     1001      127     1326 2024-04-07 07:30:00.000000 japanese_address_parser_py-0.1.0b12/core/src/err.rs
+-rw-r--r--   0     1001      127       64 2024-04-07 07:30:00.000000 japanese_address_parser_py-0.1.0b12/core/src/lib.rs
+-rw-r--r--   0     1001      127     3131 2024-04-07 07:30:00.000000 japanese_address_parser_py-0.1.0b12/core/src/parser/adapter/orthographical_variant_adapter.rs
+-rw-r--r--   0     1001      127       40 2024-04-07 07:30:00.000000 japanese_address_parser_py-0.1.0b12/core/src/parser/adapter.rs
+-rw-r--r--   0     1001      127      570 2024-04-07 07:30:00.000000 japanese_address_parser_py-0.1.0b12/core/src/parser/filter/fullwidth_character.rs
+-rw-r--r--   0     1001      127     7292 2024-04-07 07:30:00.000000 japanese_address_parser_py-0.1.0b12/core/src/parser/filter/invalid_town_name_format.rs
+-rw-r--r--   0     1001      127     3393 2024-04-07 07:30:00.000000 japanese_address_parser_py-0.1.0b12/core/src/parser/filter/non_kanji_block_number.rs
+-rw-r--r--   0     1001      127      162 2024-04-07 07:30:00.000000 japanese_address_parser_py-0.1.0b12/core/src/parser/filter.rs
+-rw-r--r--   0     1001      127     3078 2024-04-07 07:30:00.000000 japanese_address_parser_py-0.1.0b12/core/src/parser/read_city.rs
+-rw-r--r--   0     1001      127     2293 2024-04-07 07:30:00.000000 japanese_address_parser_py-0.1.0b12/core/src/parser/read_house_number.rs
+-rw-r--r--   0     1001      127     1739 2024-04-07 07:30:00.000000 japanese_address_parser_py-0.1.0b12/core/src/parser/read_prefecture.rs
+-rw-r--r--   0     1001      127     7124 2024-04-07 07:30:00.000000 japanese_address_parser_py-0.1.0b12/core/src/parser/read_town.rs
+-rw-r--r--   0     1001      127     9275 2024-04-07 07:30:00.000000 japanese_address_parser_py-0.1.0b12/core/src/parser.rs
+-rw-r--r--   0     1001      127     3695 2024-04-07 07:30:00.000000 japanese_address_parser_py-0.1.0b12/core/src/util/converter.rs
+-rw-r--r--   0     1001      127       19 2024-04-07 07:30:00.000000 japanese_address_parser_py-0.1.0b12/core/src/util.rs
+-rw-r--r--   0     1001      127     2826 2024-04-07 07:30:00.000000 japanese_address_parser_py-0.1.0b12/README.md
+-rw-r--r--   0        0        0      464 1970-01-01 00:00:00.000000 japanese_address_parser_py-0.1.0b12/python/Cargo.toml
+-rw-r--r--   0     1001      127     3282 2024-04-07 07:30:00.000000 japanese_address_parser_py-0.1.0b12/python/README.md
+-rw-r--r--   0     1001      127     1426 2024-04-07 07:30:00.000000 japanese_address_parser_py-0.1.0b12/python/src/lib.rs
+-rw-r--r--   0     1001      127    35483 2024-04-07 07:30:05.000000 japanese_address_parser_py-0.1.0b12/Cargo.lock
+-rw-r--r--   0        0        0      507 1970-01-01 00:00:00.000000 japanese_address_parser_py-0.1.0b12/Cargo.toml
+-rw-r--r--   0        0        0      346 1970-01-01 00:00:00.000000 japanese_address_parser_py-0.1.0b12/pyproject.toml
+-rw-r--r--   0        0        0     3785 1970-01-01 00:00:00.000000 japanese_address_parser_py-0.1.0b12/PKG-INFO
```

### Comparing `japanese_address_parser_py-0.1.0b11/core/LICENSE` & `japanese_address_parser_py-0.1.0b12/core/LICENSE`

 * *Files identical despite different names*

### Comparing `japanese_address_parser_py-0.1.0b11/core/src/api/city_master_api.rs` & `japanese_address_parser_py-0.1.0b12/core/src/api/city_master_api.rs`

 * *Files identical despite different names*

### Comparing `japanese_address_parser_py-0.1.0b11/core/src/api/prefecture_master_api.rs` & `japanese_address_parser_py-0.1.0b12/core/src/api/prefecture_master_api.rs`

 * *Files identical despite different names*

### Comparing `japanese_address_parser_py-0.1.0b11/core/src/api.rs` & `japanese_address_parser_py-0.1.0b12/core/src/api.rs`

 * *Files identical despite different names*

### Comparing `japanese_address_parser_py-0.1.0b11/core/src/entity.rs` & `japanese_address_parser_py-0.1.0b12/core/src/entity.rs`

 * *Files identical despite different names*

### Comparing `japanese_address_parser_py-0.1.0b11/core/src/err.rs` & `japanese_address_parser_py-0.1.0b12/core/src/err.rs`

 * *Files identical despite different names*

### Comparing `japanese_address_parser_py-0.1.0b11/core/src/parser/adapter/orthographical_variant_adapter.rs` & `japanese_address_parser_py-0.1.0b12/core/src/parser/adapter/orthographical_variant_adapter.rs`

 * *Files identical despite different names*

### Comparing `japanese_address_parser_py-0.1.0b11/core/src/parser/filter/fullwidth_character.rs` & `japanese_address_parser_py-0.1.0b12/core/src/parser/filter/fullwidth_character.rs`

 * *Files identical despite different names*

### Comparing `japanese_address_parser_py-0.1.0b11/core/src/parser/filter/invalid_town_name_format.rs` & `japanese_address_parser_py-0.1.0b12/core/src/parser/filter/invalid_town_name_format.rs`

 * *Files identical despite different names*

### Comparing `japanese_address_parser_py-0.1.0b11/core/src/parser/filter/non_kanji_block_number.rs` & `japanese_address_parser_py-0.1.0b12/core/src/parser/filter/non_kanji_block_number.rs`

 * *Files identical despite different names*

### Comparing `japanese_address_parser_py-0.1.0b11/core/src/parser/read_city.rs` & `japanese_address_parser_py-0.1.0b12/core/src/parser/read_city.rs`

 * *Files identical despite different names*

### Comparing `japanese_address_parser_py-0.1.0b11/core/src/parser/read_house_number.rs` & `japanese_address_parser_py-0.1.0b12/core/src/parser/read_house_number.rs`

 * *Files identical despite different names*

### Comparing `japanese_address_parser_py-0.1.0b11/core/src/parser/read_prefecture.rs` & `japanese_address_parser_py-0.1.0b12/core/src/parser/read_prefecture.rs`

 * *Files identical despite different names*

### Comparing `japanese_address_parser_py-0.1.0b11/core/src/parser/read_town.rs` & `japanese_address_parser_py-0.1.0b12/core/src/parser/read_town.rs`

 * *Files identical despite different names*

### Comparing `japanese_address_parser_py-0.1.0b11/core/src/parser.rs` & `japanese_address_parser_py-0.1.0b12/core/src/parser.rs`

 * *Files identical despite different names*

### Comparing `japanese_address_parser_py-0.1.0b11/core/src/util/converter.rs` & `japanese_address_parser_py-0.1.0b12/core/src/util/converter.rs`

 * *Files identical despite different names*

### Comparing `japanese_address_parser_py-0.1.0b11/README.md` & `japanese_address_parser_py-0.1.0b12/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # japanese-address-parser
 
 [![Docs](https://docs.rs/japanese-address-parser/badge.svg)](https://docs.rs/japanese-address-parser)
 [![Crates.io (latest)](https://img.shields.io/crates/v/japanese-address-parser)](https://crates.io/crates/japanese-address-parser)
-![Rust Version](https://img.shields.io/badge/rust%20version-%3E%3D1.75.0-orange)
+![Rust Version](https://img.shields.io/badge/rust%20version-%3E%3D1.64.0-orange)
 [![Unit test & Code check](https://github.com/YuukiToriyama/japanese-address-parser/actions/workflows/code-check.yaml/badge.svg)](https://github.com/YuukiToriyama/japanese-address-parser/actions/workflows/code-check.yaml)
 
-A Rust Library to parse japanses addresses.
+A Rust Library to parse japanese addresses.
 
 ## Usage
 
 Add this to your `Cargo.toml`
 
 ```bash
 cargo add japanese-address-parser
```

### Comparing `japanese_address_parser_py-0.1.0b11/python/README.md` & `japanese_address_parser_py-0.1.0b12/python/README.md`

 * *Files identical despite different names*

### Comparing `japanese_address_parser_py-0.1.0b11/python/src/lib.rs` & `japanese_address_parser_py-0.1.0b12/python/src/lib.rs`

 * *Files identical despite different names*

### Comparing `japanese_address_parser_py-0.1.0b11/Cargo.lock` & `japanese_address_parser_py-0.1.0b12/Cargo.lock`

 * *Files 3% similar despite different names*

```diff
@@ -45,17 +45,17 @@
  "miniz_oxide",
  "object",
  "rustc-demangle",
 ]
 
 [[package]]
 name = "base64"
-version = "0.21.7"
+version = "0.22.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9d297deb1925b89f2ccc13d7635fa0714f12c87adce1c75356b39ca9b7178567"
+checksum = "9475866fec1451be56a3c2400fd081ff546538961565ccb5b7142cbd22bc7a51"
 
 [[package]]
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
@@ -90,30 +90,14 @@
 checksum = "a06aeb73f470f66dcdbf7223caeebb85984942f22f1adb2a088cf9668146bbbc"
 dependencies = [
  "cfg-if",
  "wasm-bindgen",
 ]
 
 [[package]]
-name = "core-foundation"
-version = "0.9.4"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "91e195e091a93c46f7102ec7818a2aa394e1e1771c3ab4825963fa03e45afb8f"
-dependencies = [
- "core-foundation-sys",
- "libc",
-]
-
-[[package]]
-name = "core-foundation-sys"
-version = "0.8.6"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "06ea2b9bc92be3c2baa9334a323ebca2d6f074ff852cd1d7b11064035cd3868f"
-
-[[package]]
 name = "csv"
 version = "1.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ac574ff4d437a7b5ad237ef331c17ccca63c46479e5b5453eb8e10bb99a759fe"
 dependencies = [
  "csv-core",
  "itoa",
@@ -133,29 +117,14 @@
 [[package]]
 name = "either"
 version = "1.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "11157ac094ffbdde99aa67b23417ebdd801842852b500e395a45a9c0aac03e4a"
 
 [[package]]
-name = "encoding_rs"
-version = "0.8.33"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7268b386296a025e474d5140678f75d6de9493ae55a5d709eeb9dd08149945e1"
-dependencies = [
- "cfg-if",
-]
-
-[[package]]
-name = "equivalent"
-version = "1.0.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5443807d6dff69373d433ab9ef5378ad8df50ca6298caf15de6e52e24aaf54d5"
-
-[[package]]
 name = "fnv"
 version = "1.0.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3f9eec918d3f24069decb9af1554cad7c880e2da24a9afd88aca000531ab82c1"
 
 [[package]]
 name = "form_urlencoded"
@@ -169,14 +138,15 @@
 [[package]]
 name = "futures-channel"
 version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "eac8f7d7865dcb88bd4373ab671c8cf4508703796caa2b1985a9ca867b3fcb78"
 dependencies = [
  "futures-core",
+ "futures-sink",
 ]
 
 [[package]]
 name = "futures-core"
 version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "dfc6580bb841c5a68e9ef15c77ccc837b40a7504914d52e47b8b0e9bbda25a1d"
@@ -203,159 +173,155 @@
 name = "futures-util"
 version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3d6401deb83407ab3da39eba7e33987a73c3df0c82b4bb5813ee871c19c41d48"
 dependencies = [
  "futures-core",
  "futures-io",
+ "futures-sink",
  "futures-task",
  "memchr",
  "pin-project-lite",
  "pin-utils",
  "slab",
 ]
 
 [[package]]
 name = "getrandom"
-version = "0.2.12"
+version = "0.2.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "190092ea657667030ac6a35e305e62fc4dd69fd98ac98631e5d3a2b1575a12b5"
+checksum = "a06fddc2749e0528d2813f95e050e87e52c8cbbae56223b9babf73b3e53b0cc6"
 dependencies = [
  "cfg-if",
  "libc",
  "wasi",
 ]
 
 [[package]]
 name = "gimli"
 version = "0.28.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4271d37baee1b8c7e4b708028c57d816cf9d2434acb33a549475f78c181f6253"
 
 [[package]]
-name = "h2"
-version = "0.3.25"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4fbd2820c5e49886948654ab546d0688ff24530286bdcf8fca3cefb16d4618eb"
-dependencies = [
- "bytes",
- "fnv",
- "futures-core",
- "futures-sink",
- "futures-util",
- "http",
- "indexmap",
- "slab",
- "tokio",
- "tokio-util",
- "tracing",
-]
-
-[[package]]
-name = "hashbrown"
-version = "0.14.3"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "290f1a1d9242c78d09ce40a5e87e7554ee637af1351968159f4952f028f75604"
-
-[[package]]
 name = "heck"
 version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "95505c38b4572b2d910cecb0281560f54b440a19336cbbcb27bf6ce6adc6f5a8"
 
 [[package]]
+name = "hermit-abi"
+version = "0.3.9"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d231dfb89cfffdbc30e7fc41579ed6066ad03abda9e567ccafae602b97ec5024"
+
+[[package]]
 name = "http"
-version = "0.2.12"
+version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "601cbb57e577e2f5ef5be8e7b83f0f63994f25aa94d673e54a92d5c516d101f1"
+checksum = "21b9ddb458710bc376481b842f5da65cdf31522de232c1ca8146abce2a358258"
 dependencies = [
  "bytes",
  "fnv",
  "itoa",
 ]
 
 [[package]]
 name = "http-body"
-version = "0.4.6"
+version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7ceab25649e9960c0311ea418d17bee82c0dcec1bd053b5f9a66e265a693bed2"
+checksum = "1cac85db508abc24a2e48553ba12a996e87244a0395ce011e62b37158745d643"
 dependencies = [
  "bytes",
  "http",
+]
+
+[[package]]
+name = "http-body-util"
+version = "0.1.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "0475f8b2ac86659c21b64320d5d653f9efe42acd2a4e560073ec61a155a34f1d"
+dependencies = [
+ "bytes",
+ "futures-core",
+ "http",
+ "http-body",
  "pin-project-lite",
 ]
 
 [[package]]
 name = "httparse"
 version = "1.8.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d897f394bad6a705d5f4104762e116a75639e470d80901eed05a860a95cb1904"
 
 [[package]]
-name = "httpdate"
-version = "1.0.3"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "df3b46402a9d5adb4c86a0cf463f42e19994e3ee891101b1841f30a545cb49a9"
-
-[[package]]
 name = "hyper"
-version = "0.14.28"
+version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bf96e135eb83a2a8ddf766e426a841d8ddd7449d5f00d34ea02b41d2f19eef80"
+checksum = "186548d73ac615b32a73aafe38fb4f56c0d340e110e5a200bcadbaf2e199263a"
 dependencies = [
  "bytes",
  "futures-channel",
- "futures-core",
  "futures-util",
- "h2",
  "http",
  "http-body",
  "httparse",
- "httpdate",
  "itoa",
  "pin-project-lite",
- "socket2",
+ "smallvec",
  "tokio",
- "tower-service",
- "tracing",
  "want",
 ]
 
 [[package]]
 name = "hyper-rustls"
-version = "0.24.2"
+version = "0.26.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ec3efd23720e2049821a693cbc7e65ea87c72f1c58ff2f9522ff332b1491e590"
+checksum = "a0bea761b46ae2b24eb4aef630d8d1c398157b6fc29e6350ecf090a0b70c952c"
 dependencies = [
  "futures-util",
  "http",
  "hyper",
+ "hyper-util",
  "rustls",
+ "rustls-pki-types",
  "tokio",
  "tokio-rustls",
+ "tower-service",
 ]
 
 [[package]]
-name = "idna"
-version = "0.5.0"
+name = "hyper-util"
+version = "0.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "634d9b1461af396cad843f47fdba5597a4f9e6ddd4bfb6ff5d85028c25cb12f6"
+checksum = "ca38ef113da30126bbff9cd1705f9273e15d45498615d138b0c20279ac7a76aa"
 dependencies = [
- "unicode-bidi",
- "unicode-normalization",
+ "bytes",
+ "futures-channel",
+ "futures-util",
+ "http",
+ "http-body",
+ "hyper",
+ "pin-project-lite",
+ "socket2",
+ "tokio",
+ "tower",
+ "tower-service",
+ "tracing",
 ]
 
 [[package]]
-name = "indexmap"
-version = "2.2.6"
+name = "idna"
+version = "0.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "168fb715dda47215e360912c096649d23d58bf392ac62f73919e831745e40f26"
+checksum = "634d9b1461af396cad843f47fdba5597a4f9e6ddd4bfb6ff5d85028c25cb12f6"
 dependencies = [
- "equivalent",
- "hashbrown",
+ "unicode-bidi",
+ "unicode-normalization",
 ]
 
 [[package]]
 name = "indoc"
 version = "2.0.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b248f5224d1d606005e02c97f5aa4e88eeb230488bcc03bc9ca4d7991399f2b5"
@@ -379,15 +345,15 @@
 name = "itoa"
 version = "1.0.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "49f1f14873335454500d59611f1cf4a4b0f786f9ac11f4312a78e4cf2566695b"
 
 [[package]]
 name = "japanese-address-parser"
-version = "0.1.0-beta.11"
+version = "0.1.0-beta.12"
 dependencies = [
  "itertools",
  "js-sys",
  "nom",
  "regex",
  "reqwest",
  "serde",
@@ -481,14 +447,24 @@
 checksum = "d273983c5a657a70a3e8f2a01329822f3b8c8172b73826411a55751e404a0a4a"
 dependencies = [
  "memchr",
  "minimal-lexical",
 ]
 
 [[package]]
+name = "num_cpus"
+version = "1.16.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "4161fcb6d602d4d2081af7c3a45852d875a03dd337a6bfdd6e06407b61342a43"
+dependencies = [
+ "hermit-abi",
+ "libc",
+]
+
+[[package]]
 name = "object"
 version = "0.32.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a6a622008b6e321afc04970976f62ee297fdbaa6f95318ca343e3eebb9648441"
 dependencies = [
  "memchr",
 ]
@@ -525,14 +501,34 @@
 [[package]]
 name = "percent-encoding"
 version = "2.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e3148f5046208a5d56bcfc03053e3ca6334e51da8dfb19b6cdc8b306fae3283e"
 
 [[package]]
+name = "pin-project"
+version = "1.1.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b6bf43b791c5b9e34c3d182969b4abb522f9343702850a2e57f460d00d09b4b3"
+dependencies = [
+ "pin-project-internal",
+]
+
+[[package]]
+name = "pin-project-internal"
+version = "1.1.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "2f38a4412a78282e09a2cf38d195ea5420d15ba0602cb375210efbc877243965"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "syn",
+]
+
+[[package]]
 name = "pin-project-lite"
 version = "0.2.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bda66fc9667c18cb2758a2ac84d1167245054bcf85d5d1aaa6923f45801bdd02"
 
 [[package]]
 name = "pin-utils"
@@ -553,17 +549,17 @@
 checksum = "e835ff2298f5721608eb1a980ecaee1aef2c132bf95ecc026a11b7bf3c01c02e"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
-version = "0.21.0"
+version = "0.21.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a02a88a17e74cadbc8ce77855e1d6c8ad0ab82901a4a9b5046bd01c1c0bd95cd"
+checksum = "a7a8b1990bd018761768d5e608a13df8bd1ac5f678456e0f301bb93e5f3ea16b"
 dependencies = [
  "cfg-if",
  "indoc",
  "libc",
  "memoffset",
  "parking_lot",
  "portable-atomic",
@@ -571,60 +567,60 @@
  "pyo3-ffi",
  "pyo3-macros",
  "unindent",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.21.0"
+version = "0.21.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a5eb0b6ecba38961f6f4bd6cd5906dfab3cd426ff37b2eed5771006aa31656f1"
+checksum = "650dca34d463b6cdbdb02b1d71bfd6eb6b6816afc708faebb3bac1380ff4aef7"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
-version = "0.21.0"
+version = "0.21.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ba8a6e48a29b5d22e4fdaf132d8ba8d3203ee9f06362d48f244346902a594ec3"
+checksum = "09a7da8fc04a8a2084909b59f29e1b8474decac98b951d77b80b26dc45f046ad"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.21.0"
+version = "0.21.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4e80493c5965f94a747d0782a607b2328a4eea5391327b152b00e2f3b001cede"
+checksum = "4b8a199fce11ebb28e3569387228836ea98110e43a804a530a9fd83ade36d513"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.21.0"
+version = "0.21.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fcd7d86f42004025200e12a6a8119bd878329e6fddef8178eaafa4e4b5906c5b"
+checksum = "93fbbfd7eb553d10036513cb122b888dcd362a945a00b06c165f2ab480d4cc3b"
 dependencies = [
  "heck",
  "proc-macro2",
  "pyo3-build-config",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "python"
-version = "0.1.0-beta.11"
+version = "0.1.0-beta.12"
 dependencies = [
  "japanese-address-parser",
  "pyo3",
 ]
 
 [[package]]
 name = "quote"
@@ -671,42 +667,43 @@
 name = "regex-syntax"
 version = "0.8.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "adad44e29e4c806119491a7f06f03de4d1af22c3a680dd47f1e6e179439d1f56"
 
 [[package]]
 name = "reqwest"
-version = "0.11.27"
+version = "0.12.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dd67538700a17451e7cba03ac727fb961abb7607553461627b97de0b89cf4a62"
+checksum = "3e6cc1e89e689536eb5aeede61520e874df5a4707df811cd5da4aa5fbb2aae19"
 dependencies = [
  "base64",
  "bytes",
- "encoding_rs",
+ "futures-channel",
  "futures-core",
  "futures-util",
- "h2",
  "http",
  "http-body",
+ "http-body-util",
  "hyper",
  "hyper-rustls",
+ "hyper-util",
  "ipnet",
  "js-sys",
  "log",
  "mime",
  "once_cell",
  "percent-encoding",
  "pin-project-lite",
  "rustls",
  "rustls-pemfile",
+ "rustls-pki-types",
  "serde",
  "serde_json",
  "serde_urlencoded",
  "sync_wrapper",
- "system-configuration",
  "tokio",
  "tokio-rustls",
  "tower-service",
  "url",
  "wasm-bindgen",
  "wasm-bindgen-futures",
  "web-sys",
@@ -733,40 +730,50 @@
 name = "rustc-demangle"
 version = "0.1.23"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d626bb9dae77e28219937af045c257c28bfd3f69333c512553507f5f9798cb76"
 
 [[package]]
 name = "rustls"
-version = "0.21.10"
+version = "0.22.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f9d5a6813c0759e4609cd494e8e725babae6a2ca7b62a5536a13daaec6fcb7ba"
+checksum = "99008d7ad0bbbea527ec27bddbc0e432c5b87d8175178cee68d2eec9c4a1813c"
 dependencies = [
  "log",
  "ring",
+ "rustls-pki-types",
  "rustls-webpki",
- "sct",
+ "subtle",
+ "zeroize",
 ]
 
 [[package]]
 name = "rustls-pemfile"
-version = "1.0.4"
+version = "2.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1c74cae0a4cf6ccbbf5f359f08efdf8ee7e1dc532573bf0db71968cb56b1448c"
+checksum = "29993a25686778eb88d4189742cd713c9bce943bc54251a33509dc63cbacf73d"
 dependencies = [
  "base64",
+ "rustls-pki-types",
 ]
 
 [[package]]
+name = "rustls-pki-types"
+version = "1.4.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ecd36cc4259e3e4514335c4a138c6b43171a8d61d8f5c9348f9fc7529416f247"
+
+[[package]]
 name = "rustls-webpki"
-version = "0.101.7"
+version = "0.102.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8b6275d1ee7a1cd780b64aca7726599a1dbc893b1e64144529e55c3c2f745765"
+checksum = "faaa0a62740bedb9b2ef5afa303da42764c012f743917351dc9a237ea1663610"
 dependencies = [
  "ring",
+ "rustls-pki-types",
  "untrusted",
 ]
 
 [[package]]
 name = "ryu"
 version = "1.0.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -781,24 +788,14 @@
 [[package]]
 name = "scopeguard"
 version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "94143f37725109f92c262ed2cf5e59bce7498c01bcc1502d7b9afe439a4e9f49"
 
 [[package]]
-name = "sct"
-version = "0.7.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "da046153aa2352493d6cb7da4b6e5c0c057d8a1d0a9aa8560baffdd945acd414"
-dependencies = [
- "ring",
- "untrusted",
-]
-
-[[package]]
 name = "serde"
 version = "1.0.197"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3fb1c873e1b9b056a4dc4c0c198b24c3ffa059243875552b2bd0933b1aee4ce2"
 dependencies = [
  "serde_derive",
 ]
@@ -876,52 +873,37 @@
 [[package]]
 name = "spin"
 version = "0.9.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6980e8d7511241f8acf4aebddbb1ff938df5eebe98691418c4468d0b72a96a67"
 
 [[package]]
+name = "subtle"
+version = "2.5.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "81cdd64d312baedb58e21336b31bc043b77e01cc99033ce76ef539f78e965ebc"
+
+[[package]]
 name = "syn"
-version = "2.0.57"
+version = "2.0.58"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "11a6ae1e52eb25aab8f3fb9fca13be982a373b8f1157ca14b897a825ba4a2d35"
+checksum = "44cfb93f38070beee36b3fef7d4f5a16f27751d94b187b666a5cc5e9b0d30687"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "sync_wrapper"
 version = "0.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2047c6ded9c721764247e62cd3b03c09ffc529b2ba5b10ec482ae507a4a70160"
 
 [[package]]
-name = "system-configuration"
-version = "0.5.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ba3a3adc5c275d719af8cb4272ea1c4a6d668a777f37e115f6d11ddbc1c8e0e7"
-dependencies = [
- "bitflags",
- "core-foundation",
- "system-configuration-sys",
-]
-
-[[package]]
-name = "system-configuration-sys"
-version = "0.5.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a75fb188eb626b924683e3b95e3a48e63551fcfb51949de2f06a9d91dbee93c9"
-dependencies = [
- "core-foundation-sys",
- "libc",
-]
-
-[[package]]
 name = "target-lexicon"
 version = "0.12.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e1fc403891a21bcfb7c37834ba66a547a8f402146eba7265b5a6d88059c9ff2f"
 
 [[package]]
 name = "test-case"
@@ -954,15 +936,15 @@
  "quote",
  "syn",
  "test-case-core",
 ]
 
 [[package]]
 name = "tests"
-version = "0.1.0-beta.11"
+version = "0.1.0-beta.12"
 dependencies = [
  "csv",
  "japanese-address-parser",
  "serde",
  "tokio",
 ]
 
@@ -987,14 +969,15 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1adbebffeca75fcfd058afa480fb6c0b81e165a0323f9c9d39c9697e37c46787"
 dependencies = [
  "backtrace",
  "bytes",
  "libc",
  "mio",
+ "num_cpus",
  "pin-project-lite",
  "socket2",
  "tokio-macros",
  "windows-sys 0.48.0",
 ]
 
 [[package]]
@@ -1006,48 +989,58 @@
  "proc-macro2",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "tokio-rustls"
-version = "0.24.1"
+version = "0.25.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c28327cf380ac148141087fbfb9de9d7bd4e84ab5d2c28fbc911d753de8a7081"
+checksum = "775e0c0f0adb3a2f22a00c4745d728b479985fc15ee7ca6a2608388c5569860f"
 dependencies = [
  "rustls",
+ "rustls-pki-types",
  "tokio",
 ]
 
 [[package]]
-name = "tokio-util"
-version = "0.7.10"
+name = "tower"
+version = "0.4.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5419f34732d9eb6ee4c3578b7989078579b7f039cbbb9ca2c4da015749371e15"
+checksum = "b8fa9be0de6cf49e536ce1851f987bd21a43b771b09473c3549a6c853db37c1c"
 dependencies = [
- "bytes",
  "futures-core",
- "futures-sink",
+ "futures-util",
+ "pin-project",
  "pin-project-lite",
  "tokio",
+ "tower-layer",
+ "tower-service",
  "tracing",
 ]
 
 [[package]]
+name = "tower-layer"
+version = "0.3.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "c20c8dbed6283a09604c3e69b4b7eeb54e298b8a600d4d5ecb5ad39de609f1d0"
+
+[[package]]
 name = "tower-service"
 version = "0.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b6bc1c9ce2b5135ac7f93c72918fc37feb872bdc6a5533a8b85eb4b86bfdae52"
 
 [[package]]
 name = "tracing"
 version = "0.1.40"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c3523ab5a71916ccf420eebdf5521fcef02141234bbc0b8a49f2fdc4544364ef"
 dependencies = [
+ "log",
  "pin-project-lite",
  "tracing-core",
 ]
 
 [[package]]
 name = "tracing-core"
 version = "0.1.32"
@@ -1120,15 +1113,15 @@
 name = "wasi"
 version = "0.11.0+wasi-snapshot-preview1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9c8d87e72b64a3b4db28d11ce29237c246188f4f51057d65a7eab63b7987e423"
 
 [[package]]
 name = "wasm"
-version = "0.1.0-beta.11"
+version = "0.1.0-beta.12"
 dependencies = [
  "console_error_panic_hook",
  "japanese-address-parser",
  "serde-wasm-bindgen",
  "wasm-bindgen",
  "wasm-bindgen-futures",
 ]
@@ -1232,17 +1225,20 @@
 dependencies = [
  "js-sys",
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "webpki-roots"
-version = "0.25.4"
+version = "0.26.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5f20c57d8d7db6d3b86154206ae5d8fba62dd39573114de97c2cb0578251f8e1"
+checksum = "b3de34ae270483955a94f4b21bdaaeb83d508bb84a01435f393818edb0012009"
+dependencies = [
+ "rustls-pki-types",
+]
 
 [[package]]
 name = "windows-sys"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "677d2418bec65e3338edb076e806bc1ec15693c5d0104683f2efe857f61056a9"
 dependencies = [
@@ -1370,14 +1366,20 @@
 name = "windows_x86_64_msvc"
 version = "0.52.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "32b752e52a2da0ddfbdbcc6fceadfeede4c939ed16d13e648833a61dfb611ed8"
 
 [[package]]
 name = "winreg"
-version = "0.50.0"
+version = "0.52.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "524e57b2c537c0f9b1e69f1965311ec12182b4122e45035b1508cd24d2adadb1"
+checksum = "a277a57398d4bfa075df44f501a17cfdf8542d224f0d36095a2adc7aee4ef0a5"
 dependencies = [
  "cfg-if",
  "windows-sys 0.48.0",
 ]
+
+[[package]]
+name = "zeroize"
+version = "1.7.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "525b4ec142c6b68a2d10f01f7bbf6755599ca3f81ea53b8431b7dd348f5fdb2d"
```

### Comparing `japanese_address_parser_py-0.1.0b11/PKG-INFO` & `japanese_address_parser_py-0.1.0b12/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: japanese-address-parser-py
-Version: 0.1.0b11
+Version: 0.1.0b12
 Classifier: Topic :: Text Processing
 Classifier: Programming Language :: Rust
 Summary: A Rust Library to parse japanses addresses.
 Keywords: converter,utility,geo,rust
 Author: Yuuki Toriyama <github@toriyama.dev>
 Author-email: Yuuki Toriyama <github@toriyama.dev>
 License: MIT
```

