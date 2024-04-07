# Comparing `tmp/dogma_rust-0.2.0.tar.gz` & `tmp/dogma_rust-0.2.1.tar.gz`

## Comparing `dogma_rust-0.2.0.tar` & `dogma_rust-0.2.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      412 1970-01-01 00:00:00.000000 dogma_rust-0.2.0/Cargo.toml
--rw-r--r--   0    23269      100     3526 2024-04-03 16:48:42.000000 dogma_rust-0.2.0/.github/workflows/CI.yml
--rw-r--r--   0    23269      100      686 2024-04-03 16:48:42.000000 dogma_rust-0.2.0/.gitignore
--rw-r--r--   0    23269      100      166 2024-04-04 19:31:45.000000 dogma_rust-0.2.0/README.md
--rw-r--r--   0    23269      100     2111 2024-04-04 01:54:29.000000 dogma_rust-0.2.0/src/data.rs
--rw-r--r--   0    23269      100     3416 2024-04-07 01:04:04.000000 dogma_rust-0.2.0/src/fasta.rs
--rw-r--r--   0    23269      100     3752 2024-04-05 03:46:03.000000 dogma_rust-0.2.0/src/lib.rs
--rw-r--r--   0    23269      100     2663 2024-04-03 20:34:57.000000 dogma_rust-0.2.0/src/parallel.rs
--rw-r--r--   0    23269      100    19296 2024-04-07 01:12:45.000000 dogma_rust-0.2.0/Cargo.lock
--rw-r--r--   0    23269      100      411 2024-04-04 19:30:55.000000 dogma_rust-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      495 1970-01-01 00:00:00.000000 dogma_rust-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      412 1970-01-01 00:00:00.000000 dogma_rust-0.2.1/Cargo.toml
+-rw-r--r--   0    23269      100     3526 2024-04-03 16:48:42.000000 dogma_rust-0.2.1/.github/workflows/CI.yml
+-rw-r--r--   0    23269      100      686 2024-04-03 16:48:42.000000 dogma_rust-0.2.1/.gitignore
+-rw-r--r--   0    23269      100      377 2024-04-07 01:19:19.000000 dogma_rust-0.2.1/README.md
+-rw-r--r--   0    23269      100     2111 2024-04-04 01:54:29.000000 dogma_rust-0.2.1/src/data.rs
+-rw-r--r--   0    23269      100     3416 2024-04-07 01:04:04.000000 dogma_rust-0.2.1/src/fasta.rs
+-rw-r--r--   0    23269      100     3752 2024-04-05 03:46:03.000000 dogma_rust-0.2.1/src/lib.rs
+-rw-r--r--   0    23269      100     2663 2024-04-03 20:34:57.000000 dogma_rust-0.2.1/src/parallel.rs
+-rw-r--r--   0    23269      100    19296 2024-04-07 01:21:35.000000 dogma_rust-0.2.1/Cargo.lock
+-rw-r--r--   0    23269      100      522 2024-04-07 01:22:40.000000 dogma_rust-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      706 1970-01-01 00:00:00.000000 dogma_rust-0.2.1/PKG-INFO
```

### Comparing `dogma_rust-0.2.0/.github/workflows/CI.yml` & `dogma_rust-0.2.1/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `dogma_rust-0.2.0/.gitignore` & `dogma_rust-0.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `dogma_rust-0.2.0/src/data.rs` & `dogma_rust-0.2.1/src/data.rs`

 * *Files identical despite different names*

### Comparing `dogma_rust-0.2.0/src/fasta.rs` & `dogma_rust-0.2.1/src/fasta.rs`

 * *Files identical despite different names*

### Comparing `dogma_rust-0.2.0/src/lib.rs` & `dogma_rust-0.2.1/src/lib.rs`

 * *Files identical despite different names*

### Comparing `dogma_rust-0.2.0/src/parallel.rs` & `dogma_rust-0.2.1/src/parallel.rs`

 * *Files identical despite different names*

### Comparing `dogma_rust-0.2.0/Cargo.lock` & `dogma_rust-0.2.1/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -96,15 +96,15 @@
 name = "crossbeam-utils"
 version = "0.8.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "248e3bacc7dc6baa3b21e405ee045c3047101a49145e7e9eca583ab4c2ca5345"
 
 [[package]]
 name = "dogma-rust"
-version = "0.2.0"
+version = "0.2.1"
 dependencies = [
  "anyhow",
  "chrono",
  "eyre",
  "num-bigint",
  "numpy",
  "pyo3",
```

