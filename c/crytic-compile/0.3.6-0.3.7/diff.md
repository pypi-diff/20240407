# Comparing `tmp/crytic-compile-0.3.6.tar.gz` & `tmp/crytic-compile-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crytic-compile-0.3.6.tar", last modified: Tue Jan 16 17:28:46 2024, max compression
+gzip compressed data, was "crytic-compile-0.3.7.tar", last modified: Sun Apr  7 20:56:00 2024, max compression
```

## Comparing `crytic-compile-0.3.6.tar` & `crytic-compile-0.3.7.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 17:28:46.149485 crytic-compile-0.3.6/
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-01-16 17:28:35.000000 crytic-compile-0.3.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3543 2024-01-16 17:28:46.149485 crytic-compile-0.3.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2704 2024-01-16 17:28:35.000000 crytic-compile-0.3.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 17:28:46.141485 crytic-compile-0.3.6/crytic_compile/
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-01-16 17:28:35.000000 crytic-compile-0.3.6/crytic_compile/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7834 2024-01-16 17:28:35.000000 crytic-compile-0.3.6/crytic_compile/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9788 2024-01-16 17:28:35.000000 crytic-compile-0.3.6/crytic_compile/compilation_unit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 17:28:46.141485 crytic-compile-0.3.6/crytic_compile/compiler/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-16 17:28:35.000000 crytic-compile-0.3.6/crytic_compile/compiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-01-16 17:28:35.000000 crytic-compile-0.3.6/crytic_compile/compiler/compiler.py
--rw-r--r--   0 runner    (1001) docker     (127)    27196 2024-01-16 17:28:35.000000 crytic-compile-0.3.6/crytic_compile/crytic_compile.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 17:28:46.141485 crytic-compile-0.3.6/crytic_compile/cryticparser/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-01-16 17:28:35.000000 crytic-compile-0.3.6/crytic_compile/cryticparser/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    16517 2024-01-16 17:28:35.000000 crytic-compile-0.3.6/crytic_compile/cryticparser/cryticparser.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1652 2024-01-16 17:28:35.000000 crytic-compile-0.3.6/crytic_compile/cryticparser/defaults.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 17:28:46.145485 crytic-compile-0.3.6/crytic_compile/platform/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-01-16 17:28:35.000000 crytic-compile-0.3.6/crytic_compile/platform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6326 2024-01-16 17:28:35.000000 crytic-compile-0.3.6/crytic_compile/platform/abstract_platform.py
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-01-16 17:28:35.000000 crytic-compile-0.3.6/crytic_compile/platform/all_export.py
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-01-16 17:28:35.000000 crytic-compile-0.3.6/crytic_compile/platform/all_platforms.py
--rw-r--r--   0 runner    (1001) docker     (127)     5145 2024-01-16 17:28:35.000000 crytic-compile-0.3.6/crytic_compile/platform/archive.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8496 2024-01-16 17:28:35.000000 crytic-compile-0.3.6/crytic_compile/platform/brownie.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9566 2024-01-16 17:28:35.000000 crytic-compile-0.3.6/crytic_compile/platform/buidler.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8641 2024-01-16 17:28:35.000000 crytic-compile-0.3.6/crytic_compile/platform/dapp.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    10118 2024-01-16 17:28:35.000000 crytic-compile-0.3.6/crytic_compile/platform/embark.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8281 2024-01-16 17:28:35.000000 crytic-compile-0.3.6/crytic_compile/platform/etherlime.py
--rw-r--r--   0 runner    (1001) docker     (127)    20885 2024-01-16 17:28:35.000000 crytic-compile-0.3.6/crytic_compile/platform/etherscan.py
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-01-16 17:28:35.000000 crytic-compile-0.3.6/crytic_compile/platform/exceptions.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5408 2024-01-16 17:28:35.000000 crytic-compile-0.3.6/crytic_compile/platform/foundry.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    12036 2024-01-16 17:28:35.000000 crytic-compile-0.3.6/crytic_compile/platform/hardhat.py
--rw-r--r--   0 runner    (1001) docker     (127)    29584 2024-01-16 17:28:35.000000 crytic-compile-0.3.6/crytic_compile/platform/solc.py
--rw-r--r--   0 runner    (1001) docker     (127)    16565 2024-01-16 17:28:35.000000 crytic-compile-0.3.6/crytic_compile/platform/solc_standard_json.py
--rw-r--r--   0 runner    (1001) docker     (127)    19951 2024-01-16 17:28:35.000000 crytic-compile-0.3.6/crytic_compile/platform/standard.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    18378 2024-01-16 17:28:35.000000 crytic-compile-0.3.6/crytic_compile/platform/truffle.py
--rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-01-16 17:28:35.000000 crytic-compile-0.3.6/crytic_compile/platform/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     7787 2024-01-16 17:28:35.000000 crytic-compile-0.3.6/crytic_compile/platform/vyper.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    13783 2024-01-16 17:28:35.000000 crytic-compile-0.3.6/crytic_compile/platform/waffle.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-16 17:28:35.000000 crytic-compile-0.3.6/crytic_compile/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    21891 2024-01-16 17:28:35.000000 crytic-compile-0.3.6/crytic_compile/source_unit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 17:28:46.149485 crytic-compile-0.3.6/crytic_compile/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-16 17:28:35.000000 crytic-compile-0.3.6/crytic_compile/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-16 17:28:35.000000 crytic-compile-0.3.6/crytic_compile/utils/name_collision.py
--rw-r--r--   0 runner    (1001) docker     (127)     5670 2024-01-16 17:28:35.000000 crytic-compile-0.3.6/crytic_compile/utils/naming.py
--rw-r--r--   0 runner    (1001) docker     (127)     5923 2024-01-16 17:28:35.000000 crytic-compile-0.3.6/crytic_compile/utils/natspec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-01-16 17:28:35.000000 crytic-compile-0.3.6/crytic_compile/utils/npm.py
--rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-01-16 17:28:35.000000 crytic-compile-0.3.6/crytic_compile/utils/subprocess.py
--rw-r--r--   0 runner    (1001) docker     (127)      953 2024-01-16 17:28:35.000000 crytic-compile-0.3.6/crytic_compile/utils/unit_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-01-16 17:28:35.000000 crytic-compile-0.3.6/crytic_compile/utils/zip.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 17:28:46.149485 crytic-compile-0.3.6/crytic_compile.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3543 2024-01-16 17:28:46.000000 crytic-compile-0.3.6/crytic_compile.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-01-16 17:28:46.000000 crytic-compile-0.3.6/crytic_compile.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-16 17:28:46.000000 crytic-compile-0.3.6/crytic_compile.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-01-16 17:28:46.000000 crytic-compile-0.3.6/crytic_compile.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-01-16 17:28:46.000000 crytic-compile-0.3.6/crytic_compile.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-01-16 17:28:46.000000 crytic-compile-0.3.6/crytic_compile.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-01-16 17:28:35.000000 crytic-compile-0.3.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-16 17:28:46.149485 crytic-compile-0.3.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-01-16 17:28:35.000000 crytic-compile-0.3.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 17:28:46.149485 crytic-compile-0.3.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-01-16 17:28:35.000000 crytic-compile-0.3.6/tests/test_library_linking.py
--rw-r--r--   0 runner    (1001) docker     (127)    17669 2024-01-16 17:28:35.000000 crytic-compile-0.3.6/tests/test_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-01-16 17:28:35.000000 crytic-compile-0.3.6/tests/test_zip_archive.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 20:56:00.962138 crytic-compile-0.3.7/
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-04-07 20:55:56.000000 crytic-compile-0.3.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3543 2024-04-07 20:56:00.958138 crytic-compile-0.3.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2704 2024-04-07 20:55:56.000000 crytic-compile-0.3.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 20:56:00.950138 crytic-compile-0.3.7/crytic_compile/
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-07 20:55:56.000000 crytic-compile-0.3.7/crytic_compile/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7834 2024-04-07 20:55:56.000000 crytic-compile-0.3.7/crytic_compile/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9788 2024-04-07 20:55:56.000000 crytic-compile-0.3.7/crytic_compile/compilation_unit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 20:56:00.954138 crytic-compile-0.3.7/crytic_compile/compiler/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 20:55:56.000000 crytic-compile-0.3.7/crytic_compile/compiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-04-07 20:55:56.000000 crytic-compile-0.3.7/crytic_compile/compiler/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27350 2024-04-07 20:55:56.000000 crytic-compile-0.3.7/crytic_compile/crytic_compile.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 20:56:00.954138 crytic-compile-0.3.7/crytic_compile/cryticparser/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-07 20:55:56.000000 crytic-compile-0.3.7/crytic_compile/cryticparser/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    16735 2024-04-07 20:55:56.000000 crytic-compile-0.3.7/crytic_compile/cryticparser/cryticparser.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1652 2024-04-07 20:55:56.000000 crytic-compile-0.3.7/crytic_compile/cryticparser/defaults.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 20:56:00.958138 crytic-compile-0.3.7/crytic_compile/platform/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-07 20:55:56.000000 crytic-compile-0.3.7/crytic_compile/platform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6326 2024-04-07 20:55:56.000000 crytic-compile-0.3.7/crytic_compile/platform/abstract_platform.py
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-07 20:55:56.000000 crytic-compile-0.3.7/crytic_compile/platform/all_export.py
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-04-07 20:55:56.000000 crytic-compile-0.3.7/crytic_compile/platform/all_platforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5145 2024-04-07 20:55:56.000000 crytic-compile-0.3.7/crytic_compile/platform/archive.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8496 2024-04-07 20:55:56.000000 crytic-compile-0.3.7/crytic_compile/platform/brownie.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9566 2024-04-07 20:55:56.000000 crytic-compile-0.3.7/crytic_compile/platform/buidler.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8641 2024-04-07 20:55:56.000000 crytic-compile-0.3.7/crytic_compile/platform/dapp.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10118 2024-04-07 20:55:56.000000 crytic-compile-0.3.7/crytic_compile/platform/embark.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8281 2024-04-07 20:55:56.000000 crytic-compile-0.3.7/crytic_compile/platform/etherlime.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21999 2024-04-07 20:55:56.000000 crytic-compile-0.3.7/crytic_compile/platform/etherscan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-07 20:55:56.000000 crytic-compile-0.3.7/crytic_compile/platform/exceptions.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5408 2024-04-07 20:55:56.000000 crytic-compile-0.3.7/crytic_compile/platform/foundry.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12036 2024-04-07 20:55:56.000000 crytic-compile-0.3.7/crytic_compile/platform/hardhat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29584 2024-04-07 20:55:56.000000 crytic-compile-0.3.7/crytic_compile/platform/solc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16565 2024-04-07 20:55:56.000000 crytic-compile-0.3.7/crytic_compile/platform/solc_standard_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19951 2024-04-07 20:55:56.000000 crytic-compile-0.3.7/crytic_compile/platform/standard.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    18378 2024-04-07 20:55:56.000000 crytic-compile-0.3.7/crytic_compile/platform/truffle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-04-07 20:55:56.000000 crytic-compile-0.3.7/crytic_compile/platform/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7787 2024-04-07 20:55:56.000000 crytic-compile-0.3.7/crytic_compile/platform/vyper.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    13783 2024-04-07 20:55:56.000000 crytic-compile-0.3.7/crytic_compile/platform/waffle.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 20:55:56.000000 crytic-compile-0.3.7/crytic_compile/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    21891 2024-04-07 20:55:56.000000 crytic-compile-0.3.7/crytic_compile/source_unit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 20:56:00.958138 crytic-compile-0.3.7/crytic_compile/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 20:55:56.000000 crytic-compile-0.3.7/crytic_compile/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 20:55:56.000000 crytic-compile-0.3.7/crytic_compile/utils/name_collision.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5917 2024-04-07 20:55:56.000000 crytic-compile-0.3.7/crytic_compile/utils/naming.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5923 2024-04-07 20:55:56.000000 crytic-compile-0.3.7/crytic_compile/utils/natspec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-04-07 20:55:56.000000 crytic-compile-0.3.7/crytic_compile/utils/npm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-04-07 20:55:56.000000 crytic-compile-0.3.7/crytic_compile/utils/subprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2024-04-07 20:55:56.000000 crytic-compile-0.3.7/crytic_compile/utils/unit_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-04-07 20:55:56.000000 crytic-compile-0.3.7/crytic_compile/utils/zip.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 20:56:00.958138 crytic-compile-0.3.7/crytic_compile.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3543 2024-04-07 20:56:00.000000 crytic-compile-0.3.7/crytic_compile.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-04-07 20:56:00.000000 crytic-compile-0.3.7/crytic_compile.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 20:56:00.000000 crytic-compile-0.3.7/crytic_compile.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-07 20:56:00.000000 crytic-compile-0.3.7/crytic_compile.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-07 20:56:00.000000 crytic-compile-0.3.7/crytic_compile.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-07 20:56:00.000000 crytic-compile-0.3.7/crytic_compile.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-07 20:55:56.000000 crytic-compile-0.3.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 20:56:00.962138 crytic-compile-0.3.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-04-07 20:55:56.000000 crytic-compile-0.3.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 20:56:00.958138 crytic-compile-0.3.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-04-07 20:55:56.000000 crytic-compile-0.3.7/tests/test_library_linking.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17669 2024-04-07 20:55:56.000000 crytic-compile-0.3.7/tests/test_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-04-07 20:55:56.000000 crytic-compile-0.3.7/tests/test_zip_archive.py
```

### Comparing `crytic-compile-0.3.6/LICENSE` & `crytic-compile-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `crytic-compile-0.3.6/PKG-INFO` & `crytic-compile-0.3.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crytic-compile
-Version: 0.3.6
+Version: 0.3.7
 Summary: Util to facilitate smart contracts compilation.
 Home-page: https://github.com/crytic/crytic-compile
 Author: Trail of Bits
 License: AGPL-3.0
 Requires-Python: >=3.8,!=3.12.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `crytic-compile-0.3.6/README.md` & `crytic-compile-0.3.7/README.md`

 * *Files identical despite different names*

### Comparing `crytic-compile-0.3.6/crytic_compile/__main__.py` & `crytic-compile-0.3.7/crytic_compile/__main__.py`

 * *Files identical despite different names*

### Comparing `crytic-compile-0.3.6/crytic_compile/compilation_unit.py` & `crytic-compile-0.3.7/crytic_compile/compilation_unit.py`

 * *Files identical despite different names*

### Comparing `crytic-compile-0.3.6/crytic_compile/compiler/compiler.py` & `crytic-compile-0.3.7/crytic_compile/compiler/compiler.py`

 * *Files identical despite different names*

### Comparing `crytic-compile-0.3.6/crytic_compile/crytic_compile.py` & `crytic-compile-0.3.7/crytic_compile/crytic_compile.py`

 * *Files 1% similar despite different names*

```diff
@@ -120,15 +120,15 @@
     def __init__(self, target: Union[str, AbstractPlatform], **kwargs: str) -> None:
         """See https://github.com/crytic/crytic-compile/wiki/Configuration
         Target is usually a file or a project directory. It can be an AbstractPlatform
         for custom setup
 
         Args:
             target (Union[str, AbstractPlatform]): Target
-            **kwargs: additional arguments
+            **kwargs: additional arguments. Used: "cwd"
         """
 
         # dependencies is needed for platform conversion
         self._dependencies: Set = set()
 
         self._src_content: Dict = {}
 
@@ -141,15 +141,19 @@
         # Lines are indexed from 1
         self._cached_line_to_offset: Dict[Filename, Dict[int, int]] = defaultdict(dict)
 
         # Return the line from the line number
         # Note: line 1 is at index 0
         self._cached_line_to_code: Dict[Filename, List[bytes]] = {}
 
-        self._working_dir = Path.cwd()
+        custom_cwd = kwargs.get("cwd")
+        if custom_cwd is not None:
+            self._working_dir = Path(custom_cwd)
+        else:
+            self._working_dir = Path.cwd()
 
         # pylint: disable=too-many-nested-blocks
         if isinstance(target, str):
             platform = self._init_platform(target, **kwargs)
             # If the platform is Solc it means we are trying to compile a single
             # we try to see if we are in a known compilation framework to retrieve
             # information like remappings and solc version
```

### Comparing `crytic-compile-0.3.6/crytic_compile/cryticparser/cryticparser.py` & `crytic-compile-0.3.7/crytic_compile/cryticparser/cryticparser.py`

 * *Files 1% similar despite different names*

```diff
@@ -406,14 +406,22 @@
         help="zkEVM Polygonscan API key.",
         action="store",
         dest="polyzk_api_key",
         default=DEFAULTS_FLAG_IN_CONFIG["etherscan_api_key"],
     )
 
     group_etherscan.add_argument(
+        "--blast-apikey",
+        help="Blastscan API key.",
+        action="store",
+        dest="blast_api_key",
+        default=DEFAULTS_FLAG_IN_CONFIG["etherscan_api_key"],
+    )
+
+    group_etherscan.add_argument(
         "--etherscan-export-directory",
         help="Directory in which to save the analyzed contracts.",
         action="store",
         dest="etherscan_export_dir",
         default=DEFAULTS_FLAG_IN_CONFIG["etherscan_export_directory"],
     )
```

### Comparing `crytic-compile-0.3.6/crytic_compile/cryticparser/defaults.py` & `crytic-compile-0.3.7/crytic_compile/cryticparser/defaults.py`

 * *Files identical despite different names*

### Comparing `crytic-compile-0.3.6/crytic_compile/platform/abstract_platform.py` & `crytic-compile-0.3.7/crytic_compile/platform/abstract_platform.py`

 * *Files identical despite different names*

### Comparing `crytic-compile-0.3.6/crytic_compile/platform/all_platforms.py` & `crytic-compile-0.3.7/crytic_compile/platform/all_platforms.py`

 * *Files identical despite different names*

### Comparing `crytic-compile-0.3.6/crytic_compile/platform/archive.py` & `crytic-compile-0.3.7/crytic_compile/platform/archive.py`

 * *Files identical despite different names*

### Comparing `crytic-compile-0.3.6/crytic_compile/platform/brownie.py` & `crytic-compile-0.3.7/crytic_compile/platform/brownie.py`

 * *Files identical despite different names*

### Comparing `crytic-compile-0.3.6/crytic_compile/platform/buidler.py` & `crytic-compile-0.3.7/crytic_compile/platform/buidler.py`

 * *Files identical despite different names*

### Comparing `crytic-compile-0.3.6/crytic_compile/platform/dapp.py` & `crytic-compile-0.3.7/crytic_compile/platform/dapp.py`

 * *Files identical despite different names*

### Comparing `crytic-compile-0.3.6/crytic_compile/platform/embark.py` & `crytic-compile-0.3.7/crytic_compile/platform/embark.py`

 * *Files identical despite different names*

### Comparing `crytic-compile-0.3.6/crytic_compile/platform/etherlime.py` & `crytic-compile-0.3.7/crytic_compile/platform/etherlime.py`

 * *Files identical despite different names*

### Comparing `crytic-compile-0.3.6/crytic_compile/platform/etherscan.py` & `crytic-compile-0.3.7/crytic_compile/platform/etherscan.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,14 +47,15 @@
     "avax:": (".snowtrace.io", "snowtrace.io"),
     "testnet.avax:": ("-testnet.snowtrace.io", "testnet.snowtrace.io"),
     "ftm:": (".ftmscan.com", "ftmscan.com"),
     "goerli.base:": ("-goerli.basescan.org", "goerli.basescan.org"),
     "base:": (".basescan.org", "basescan.org"),
     "gno:": (".gnosisscan.io", "gnosisscan.io"),
     "polyzk:": ("-zkevm.polygonscan.com", "zkevm.polygonscan.com"),
+    "blast:": (".blastscan.io", "blastscan.io"),
 }
 
 
 def _handle_bytecode(crytic_compile: "CryticCompile", target: str, result_b: bytes) -> None:
     """Parse the bytecode and populate CryticCompile info
 
     Args:
@@ -237,14 +238,15 @@
         avax_api_key = kwargs.get("avax_api_key", None)
         ftmscan_api_key = kwargs.get("ftmscan_api_key", None)
         bscan_api_key = kwargs.get("bscan_api_key", None)
         optim_api_key = kwargs.get("optim_api_key", None)
         base_api_key = kwargs.get("base_api_key", None)
         gno_api_key = kwargs.get("gno_api_key", None)
         polyzk_api_key = kwargs.get("polyzk_api_key", None)
+        blast_api_key = kwargs.get("blast_api_key", None)
 
         export_dir = kwargs.get("export_dir", "crytic-export")
         export_dir = os.path.join(
             export_dir, kwargs.get("etherscan_export_dir", "etherscan-contracts")
         )
 
         if etherscan_api_key and "etherscan" in etherscan_url:
@@ -276,14 +278,17 @@
             etherscan_bytecode_url += f"&apikey={base_api_key}"
         if gno_api_key and "gno" in etherscan_url:
             etherscan_url += f"&apikey={gno_api_key}"
             etherscan_bytecode_url += f"&apikey={gno_api_key}"
         if polyzk_api_key and "zkevm" in etherscan_url:
             etherscan_url += f"&apikey={polyzk_api_key}"
             etherscan_bytecode_url += f"&apikey={polyzk_api_key}"
+        if blast_api_key and "blast" in etherscan_url:
+            etherscan_url += f"&apikey={blast_api_key}"
+            etherscan_bytecode_url += f"&apikey={blast_api_key}"
 
         source_code: str = ""
         result: Dict[str, Union[bool, str, int]] = {}
         contract_name: str = ""
 
         if not only_bytecode:
             if "polygon" in etherscan_url or "basescan" in etherscan_url:
@@ -420,14 +425,36 @@
             compilation_unit,
             working_dir=working_dir,
             remappings=remappings,
             evm_version=evm_version,
             via_ir=via_ir_enabled,
         )
 
+        metadata_config = {
+            "solc_remaps": remappings if remappings else {},
+            "solc_solcs_select": compiler_version,
+            "solc_args": " ".join(
+                filter(
+                    None,
+                    [
+                        "--via-ir" if via_ir_enabled else "",
+                        "--optimize --optimize-runs " + str(optimize_runs) if optimize_runs else "",
+                        "--evm-version " + evm_version if evm_version else "",
+                    ],
+                )
+            ),
+        }
+
+        with open(
+            os.path.join(working_dir if working_dir else export_dir, "crytic_compile.config.json"),
+            "w",
+            encoding="utf-8",
+        ) as f:
+            json.dump(metadata_config, f)
+
     def clean(self, **_kwargs: str) -> None:
         pass
 
     @staticmethod
     def is_supported(target: str, **kwargs: str) -> bool:
         """Check if the target is a etherscan project
 
@@ -470,15 +497,17 @@
 
     Args:
         version (str): original version
 
     Returns:
         str: converted version
     """
-    return version[1 : version.find("+")]
+    if "+" in version:
+        return version[1 : version.find("+")]
+    return version[1:]
 
 
 def _sanitize_remappings(
     remappings: Optional[List[str]], allowed_directory: str
 ) -> Optional[List[str]]:
     """Sanitize a list of remappings
```

### Comparing `crytic-compile-0.3.6/crytic_compile/platform/foundry.py` & `crytic-compile-0.3.7/crytic_compile/platform/foundry.py`

 * *Files identical despite different names*

### Comparing `crytic-compile-0.3.6/crytic_compile/platform/hardhat.py` & `crytic-compile-0.3.7/crytic_compile/platform/hardhat.py`

 * *Files identical despite different names*

### Comparing `crytic-compile-0.3.6/crytic_compile/platform/solc.py` & `crytic-compile-0.3.7/crytic_compile/platform/solc.py`

 * *Files identical despite different names*

### Comparing `crytic-compile-0.3.6/crytic_compile/platform/solc_standard_json.py` & `crytic-compile-0.3.7/crytic_compile/platform/solc_standard_json.py`

 * *Files identical despite different names*

### Comparing `crytic-compile-0.3.6/crytic_compile/platform/standard.py` & `crytic-compile-0.3.7/crytic_compile/platform/standard.py`

 * *Files identical despite different names*

### Comparing `crytic-compile-0.3.6/crytic_compile/platform/truffle.py` & `crytic-compile-0.3.7/crytic_compile/platform/truffle.py`

 * *Files identical despite different names*

### Comparing `crytic-compile-0.3.6/crytic_compile/platform/types.py` & `crytic-compile-0.3.7/crytic_compile/platform/types.py`

 * *Files identical despite different names*

### Comparing `crytic-compile-0.3.6/crytic_compile/platform/vyper.py` & `crytic-compile-0.3.7/crytic_compile/platform/vyper.py`

 * *Files identical despite different names*

### Comparing `crytic-compile-0.3.6/crytic_compile/platform/waffle.py` & `crytic-compile-0.3.7/crytic_compile/platform/waffle.py`

 * *Files identical despite different names*

### Comparing `crytic-compile-0.3.6/crytic_compile/source_unit.py` & `crytic-compile-0.3.7/crytic_compile/source_unit.py`

 * *Files identical despite different names*

### Comparing `crytic-compile-0.3.6/crytic_compile/utils/naming.py` & `crytic-compile-0.3.7/crytic_compile/utils/naming.py`

 * *Files 10% similar despite different names*

```diff
@@ -184,14 +184,15 @@
             short = relative.relative_to(cwd)
     except ValueError:
         short = relative
     except RuntimeError:
         short = relative
 
     short = relative_to_short(short)
-
+    # Starting with v0.8.8 (https://github.com/ethereum/solidity/pull/11545), solc normalizes the paths to not include the drive on Windows,
+    # so it's important we use posix path here to avoid issues with the path comparison.
     return Filename(
-        absolute=str(absolute),
+        absolute=absolute.as_posix(),
         relative=relative.as_posix(),
         short=short.as_posix(),
-        used=str(used_filename),
+        used=Path(used_filename).as_posix(),
     )
```

### Comparing `crytic-compile-0.3.6/crytic_compile/utils/natspec.py` & `crytic-compile-0.3.7/crytic_compile/utils/natspec.py`

 * *Files identical despite different names*

### Comparing `crytic-compile-0.3.6/crytic_compile/utils/npm.py` & `crytic-compile-0.3.7/crytic_compile/utils/npm.py`

 * *Files identical despite different names*

### Comparing `crytic-compile-0.3.6/crytic_compile/utils/subprocess.py` & `crytic-compile-0.3.7/crytic_compile/utils/subprocess.py`

 * *Files identical despite different names*

### Comparing `crytic-compile-0.3.6/crytic_compile/utils/unit_tests.py` & `crytic-compile-0.3.7/crytic_compile/utils/unit_tests.py`

 * *Files identical despite different names*

### Comparing `crytic-compile-0.3.6/crytic_compile/utils/zip.py` & `crytic-compile-0.3.7/crytic_compile/utils/zip.py`

 * *Files identical despite different names*

### Comparing `crytic-compile-0.3.6/crytic_compile.egg-info/PKG-INFO` & `crytic-compile-0.3.7/crytic_compile.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crytic-compile
-Version: 0.3.6
+Version: 0.3.7
 Summary: Util to facilitate smart contracts compilation.
 Home-page: https://github.com/crytic/crytic-compile
 Author: Trail of Bits
 License: AGPL-3.0
 Requires-Python: >=3.8,!=3.12.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `crytic-compile-0.3.6/crytic_compile.egg-info/SOURCES.txt` & `crytic-compile-0.3.7/crytic_compile.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `crytic-compile-0.3.6/pyproject.toml` & `crytic-compile-0.3.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `crytic-compile-0.3.6/setup.py` & `crytic-compile-0.3.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     long_description = f.read()
 
 setup(
     name="crytic-compile",
     description="Util to facilitate smart contracts compilation.",
     url="https://github.com/crytic/crytic-compile",
     author="Trail of Bits",
-    version="0.3.6",
+    version="0.3.7",
     packages=find_packages(),
     # Python 3.12.0 on Windows suffers from https://github.com/python/cpython/issues/109590
     # breaking some of our integrations. The issue is fixed in 3.12.1
     python_requires=">=3.8,!=3.12.0",
     install_requires=["pycryptodome>=3.4.6", "cbor2", "solc-select>=v1.0.4"],
     extras_require={
         "test": [
```

### Comparing `crytic-compile-0.3.6/tests/test_library_linking.py` & `crytic-compile-0.3.7/tests/test_library_linking.py`

 * *Files identical despite different names*

### Comparing `crytic-compile-0.3.6/tests/test_metadata.py` & `crytic-compile-0.3.7/tests/test_metadata.py`

 * *Files identical despite different names*

### Comparing `crytic-compile-0.3.6/tests/test_zip_archive.py` & `crytic-compile-0.3.7/tests/test_zip_archive.py`

 * *Files identical despite different names*

