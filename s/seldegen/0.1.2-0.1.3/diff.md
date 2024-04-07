# Comparing `tmp/seldegen-0.1.2.tar.gz` & `tmp/seldegen-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seldegen-0.1.2.tar", max compression
+gzip compressed data, was "seldegen-0.1.3.tar", max compression
```

## Comparing `seldegen-0.1.2.tar` & `seldegen-0.1.3.tar`

### file list

```diff
@@ -1,59 +1,59 @@
--rw-r--r--   0        0        0     1063 2023-12-19 17:13:01.240843 seldegen-0.1.2/LICENSE
--rw-r--r--   0        0        0      570 2024-03-22 14:49:24.530143 seldegen-0.1.2/README.md
--rw-r--r--   0        0        0     1186 2024-04-05 18:34:27.055953 seldegen-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     6148 2024-03-28 21:36:21.502576 seldegen-0.1.2/seldegen/.DS_Store
--rw-r--r--   0        0        0      905 2024-03-10 14:15:32.069712 seldegen-0.1.2/seldegen/__init__.py
--rw-r--r--   0        0        0      271 2024-03-04 10:03:54.006477 seldegen-0.1.2/seldegen/abc/__init__.py
--rw-r--r--   0        0        0      565 2024-04-05 18:13:31.254714 seldegen-0.1.2/seldegen/abc/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     6039 2024-04-05 18:13:31.255567 seldegen-0.1.2/seldegen/abc/__pycache__/base_account.cpython-311.pyc
--rw-r--r--   0        0        0     5023 2024-04-05 18:13:31.267024 seldegen-0.1.2/seldegen/abc/__pycache__/browser_extension.cpython-311.pyc
--rw-r--r--   0        0        0     2380 2024-04-05 18:13:31.267310 seldegen-0.1.2/seldegen/abc/__pycache__/dapp.cpython-311.pyc
--rw-r--r--   0        0        0     6384 2024-04-05 18:13:31.267864 seldegen-0.1.2/seldegen/abc/__pycache__/wallet.cpython-311.pyc
--rw-r--r--   0        0        0     3708 2024-03-14 12:37:02.555958 seldegen-0.1.2/seldegen/abc/base_account.py
--rw-r--r--   0        0        0     3170 2024-03-10 14:15:32.060110 seldegen-0.1.2/seldegen/abc/browser_extension.py
--rw-r--r--   0        0        0     1289 2024-03-13 17:22:11.291732 seldegen-0.1.2/seldegen/abc/dapp.py
--rw-r--r--   0        0        0     4322 2024-03-18 21:16:58.614812 seldegen-0.1.2/seldegen/abc/wallet.py
--rw-r--r--   0        0        0     1048 2024-03-04 15:15:02.044620 seldegen-0.1.2/seldegen/captcha_solver.py
--rw-r--r--   0        0        0     5460 2024-03-10 13:56:26.849873 seldegen-0.1.2/seldegen/captcha_waiter.py
--rw-r--r--   0        0        0      588 2024-03-10 14:15:32.063197 seldegen-0.1.2/seldegen/context.py
--rw-r--r--   0        0        0       79 2024-03-18 21:20:50.195453 seldegen-0.1.2/seldegen/dapps/__init__.py
--rw-r--r--   0        0        0      330 2024-04-05 18:13:31.268539 seldegen-0.1.2/seldegen/dapps/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     6220 2024-04-05 18:13:31.269081 seldegen-0.1.2/seldegen/dapps/__pycache__/guild.cpython-311.pyc
--rw-r--r--   0        0        0     3263 2024-04-05 18:13:31.288079 seldegen-0.1.2/seldegen/dapps/__pycache__/lens.cpython-311.pyc
--rw-r--r--   0        0        0     4131 2024-04-05 18:13:31.287517 seldegen-0.1.2/seldegen/dapps/__pycache__/snapshot.cpython-311.pyc
--rw-r--r--   0        0        0     3924 2024-03-10 14:04:14.121204 seldegen-0.1.2/seldegen/dapps/guild.py
--rw-r--r--   0        0        0     1936 2024-03-18 21:16:58.632296 seldegen-0.1.2/seldegen/dapps/lens.py
--rw-r--r--   0        0        0     2632 2024-03-10 14:04:48.886701 seldegen-0.1.2/seldegen/dapps/snapshot.py
--rw-r--r--   0        0        0     3229 2024-03-10 14:15:32.055901 seldegen-0.1.2/seldegen/email.py
--rw-r--r--   0        0        0     1551 2024-03-19 17:16:42.207059 seldegen-0.1.2/seldegen/exceptions.py
--rw-r--r--   0        0        0      706 2023-12-19 15:19:41.201226 seldegen-0.1.2/seldegen/extensions/__init__.py
--rw-r--r--   0        0        0      958 2024-04-05 18:13:31.291274 seldegen-0.1.2/seldegen/extensions/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     7171 2024-04-05 18:13:31.291863 seldegen-0.1.2/seldegen/extensions/__pycache__/authenticator.cpython-311.pyc
--rw-r--r--   0        0        0     3542 2024-04-05 18:13:31.292195 seldegen-0.1.2/seldegen/extensions/__pycache__/capmonster.cpython-311.pyc
--rw-r--r--   0        0        0     4963 2024-03-10 14:03:08.164497 seldegen-0.1.2/seldegen/extensions/authenticator.py
--rw-r--r--   0        0        0     2195 2024-03-10 14:03:30.243674 seldegen-0.1.2/seldegen/extensions/capmonster.py
--rw-r--r--   0        0        0       69 2024-03-22 14:49:24.529615 seldegen-0.1.2/seldegen/globals.py
--rw-r--r--   0        0        0      359 2024-03-06 19:31:48.607513 seldegen-0.1.2/seldegen/socials/__init__.py
--rw-r--r--   0        0        0      735 2024-04-05 18:13:31.269317 seldegen-0.1.2/seldegen/socials/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     6903 2024-04-05 18:13:31.269998 seldegen-0.1.2/seldegen/socials/__pycache__/discord.cpython-311.pyc
--rw-r--r--   0        0        0     6561 2024-04-05 18:13:31.271881 seldegen-0.1.2/seldegen/socials/__pycache__/facebook.cpython-311.pyc
--rw-r--r--   0        0        0     6494 2024-04-05 18:13:31.275944 seldegen-0.1.2/seldegen/socials/__pycache__/github.cpython-311.pyc
--rw-r--r--   0        0        0     3314 2024-04-05 18:13:31.276243 seldegen-0.1.2/seldegen/socials/__pycache__/gmail.cpython-311.pyc
--rw-r--r--   0        0        0     7232 2024-04-05 18:13:31.276829 seldegen-0.1.2/seldegen/socials/__pycache__/google.cpython-311.pyc
--rw-r--r--   0        0        0     5998 2024-04-05 18:13:31.277360 seldegen-0.1.2/seldegen/socials/__pycache__/linkedin.cpython-311.pyc
--rw-r--r--   0        0        0    14532 2024-04-05 18:13:31.279192 seldegen-0.1.2/seldegen/socials/__pycache__/twitter.cpython-311.pyc
--rw-r--r--   0        0        0     4529 2024-03-19 17:21:41.167605 seldegen-0.1.2/seldegen/socials/discord.py
--rw-r--r--   0        0        0     4438 2024-03-14 12:16:40.439943 seldegen-0.1.2/seldegen/socials/facebook.py
--rw-r--r--   0        0        0     3982 2024-03-19 17:17:40.610882 seldegen-0.1.2/seldegen/socials/github.py
--rw-r--r--   0        0        0     2186 2024-03-10 14:00:33.245512 seldegen-0.1.2/seldegen/socials/gmail.py
--rw-r--r--   0        0        0     5086 2024-03-15 00:29:31.085041 seldegen-0.1.2/seldegen/socials/google.py
--rw-r--r--   0        0        0     4004 2024-03-19 17:08:22.151688 seldegen-0.1.2/seldegen/socials/linkedin.py
--rw-r--r--   0        0        0    10541 2024-03-19 17:24:12.014594 seldegen-0.1.2/seldegen/socials/twitter.py
--rw-r--r--   0        0        0      304 2024-03-14 21:45:11.803532 seldegen-0.1.2/seldegen/types.py
--rw-r--r--   0        0        0      224 2023-12-19 15:19:41.201564 seldegen-0.1.2/seldegen/wallets/__init__.py
--rw-r--r--   0        0        0      470 2024-04-05 18:13:31.292423 seldegen-0.1.2/seldegen/wallets/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0    15424 2024-04-05 18:31:22.639471 seldegen-0.1.2/seldegen/wallets/__pycache__/metamask.cpython-311.pyc
--rw-r--r--   0        0        0    10355 2024-04-05 18:13:31.536439 seldegen-0.1.2/seldegen/wallets/__pycache__/sui_wallet.cpython-311.pyc
--rw-r--r--   0        0        0    11176 2024-04-05 18:29:51.284321 seldegen-0.1.2/seldegen/wallets/metamask.py
--rw-r--r--   0        0        0     7258 2024-03-13 17:22:11.289963 seldegen-0.1.2/seldegen/wallets/sui_wallet.py
--rw-r--r--   0        0        0     1801 1970-01-01 00:00:00.000000 seldegen-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-12-19 17:13:01.240843 seldegen-0.1.3/LICENSE
+-rw-r--r--   0        0        0      570 2024-03-22 14:49:24.530143 seldegen-0.1.3/README.md
+-rw-r--r--   0        0        0     1186 2024-04-07 01:51:41.616145 seldegen-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     6148 2024-03-28 21:36:21.502576 seldegen-0.1.3/seldegen/.DS_Store
+-rw-r--r--   0        0        0      905 2024-03-10 14:15:32.069712 seldegen-0.1.3/seldegen/__init__.py
+-rw-r--r--   0        0        0      271 2024-03-04 10:03:54.006477 seldegen-0.1.3/seldegen/abc/__init__.py
+-rw-r--r--   0        0        0      565 2024-04-05 18:13:31.254714 seldegen-0.1.3/seldegen/abc/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     6039 2024-04-05 18:13:31.255567 seldegen-0.1.3/seldegen/abc/__pycache__/base_account.cpython-311.pyc
+-rw-r--r--   0        0        0     5023 2024-04-05 18:13:31.267024 seldegen-0.1.3/seldegen/abc/__pycache__/browser_extension.cpython-311.pyc
+-rw-r--r--   0        0        0     2380 2024-04-05 18:13:31.267310 seldegen-0.1.3/seldegen/abc/__pycache__/dapp.cpython-311.pyc
+-rw-r--r--   0        0        0     6384 2024-04-05 18:13:31.267864 seldegen-0.1.3/seldegen/abc/__pycache__/wallet.cpython-311.pyc
+-rw-r--r--   0        0        0     3708 2024-03-14 12:37:02.555958 seldegen-0.1.3/seldegen/abc/base_account.py
+-rw-r--r--   0        0        0     3170 2024-03-10 14:15:32.060110 seldegen-0.1.3/seldegen/abc/browser_extension.py
+-rw-r--r--   0        0        0     1289 2024-03-13 17:22:11.291732 seldegen-0.1.3/seldegen/abc/dapp.py
+-rw-r--r--   0        0        0     4322 2024-03-18 21:16:58.614812 seldegen-0.1.3/seldegen/abc/wallet.py
+-rw-r--r--   0        0        0     1048 2024-03-04 15:15:02.044620 seldegen-0.1.3/seldegen/captcha_solver.py
+-rw-r--r--   0        0        0     5460 2024-03-10 13:56:26.849873 seldegen-0.1.3/seldegen/captcha_waiter.py
+-rw-r--r--   0        0        0      588 2024-03-10 14:15:32.063197 seldegen-0.1.3/seldegen/context.py
+-rw-r--r--   0        0        0       79 2024-03-18 21:20:50.195453 seldegen-0.1.3/seldegen/dapps/__init__.py
+-rw-r--r--   0        0        0      330 2024-04-05 18:13:31.268539 seldegen-0.1.3/seldegen/dapps/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     6220 2024-04-05 18:13:31.269081 seldegen-0.1.3/seldegen/dapps/__pycache__/guild.cpython-311.pyc
+-rw-r--r--   0        0        0     3263 2024-04-05 18:13:31.288079 seldegen-0.1.3/seldegen/dapps/__pycache__/lens.cpython-311.pyc
+-rw-r--r--   0        0        0     4131 2024-04-05 18:13:31.287517 seldegen-0.1.3/seldegen/dapps/__pycache__/snapshot.cpython-311.pyc
+-rw-r--r--   0        0        0     3924 2024-03-10 14:04:14.121204 seldegen-0.1.3/seldegen/dapps/guild.py
+-rw-r--r--   0        0        0     1936 2024-03-18 21:16:58.632296 seldegen-0.1.3/seldegen/dapps/lens.py
+-rw-r--r--   0        0        0     2632 2024-03-10 14:04:48.886701 seldegen-0.1.3/seldegen/dapps/snapshot.py
+-rw-r--r--   0        0        0     3229 2024-03-10 14:15:32.055901 seldegen-0.1.3/seldegen/email.py
+-rw-r--r--   0        0        0     1551 2024-03-19 17:16:42.207059 seldegen-0.1.3/seldegen/exceptions.py
+-rw-r--r--   0        0        0      706 2023-12-19 15:19:41.201226 seldegen-0.1.3/seldegen/extensions/__init__.py
+-rw-r--r--   0        0        0      958 2024-04-05 18:13:31.291274 seldegen-0.1.3/seldegen/extensions/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     7171 2024-04-05 18:13:31.291863 seldegen-0.1.3/seldegen/extensions/__pycache__/authenticator.cpython-311.pyc
+-rw-r--r--   0        0        0     3542 2024-04-05 18:13:31.292195 seldegen-0.1.3/seldegen/extensions/__pycache__/capmonster.cpython-311.pyc
+-rw-r--r--   0        0        0     4963 2024-03-10 14:03:08.164497 seldegen-0.1.3/seldegen/extensions/authenticator.py
+-rw-r--r--   0        0        0     2195 2024-03-10 14:03:30.243674 seldegen-0.1.3/seldegen/extensions/capmonster.py
+-rw-r--r--   0        0        0       69 2024-03-22 14:49:24.529615 seldegen-0.1.3/seldegen/globals.py
+-rw-r--r--   0        0        0      359 2024-03-06 19:31:48.607513 seldegen-0.1.3/seldegen/socials/__init__.py
+-rw-r--r--   0        0        0      735 2024-04-05 18:13:31.269317 seldegen-0.1.3/seldegen/socials/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     6903 2024-04-05 18:13:31.269998 seldegen-0.1.3/seldegen/socials/__pycache__/discord.cpython-311.pyc
+-rw-r--r--   0        0        0     6561 2024-04-05 18:13:31.271881 seldegen-0.1.3/seldegen/socials/__pycache__/facebook.cpython-311.pyc
+-rw-r--r--   0        0        0     6494 2024-04-05 18:13:31.275944 seldegen-0.1.3/seldegen/socials/__pycache__/github.cpython-311.pyc
+-rw-r--r--   0        0        0     3314 2024-04-05 18:13:31.276243 seldegen-0.1.3/seldegen/socials/__pycache__/gmail.cpython-311.pyc
+-rw-r--r--   0        0        0     7232 2024-04-05 18:13:31.276829 seldegen-0.1.3/seldegen/socials/__pycache__/google.cpython-311.pyc
+-rw-r--r--   0        0        0     5998 2024-04-05 18:13:31.277360 seldegen-0.1.3/seldegen/socials/__pycache__/linkedin.cpython-311.pyc
+-rw-r--r--   0        0        0    14532 2024-04-05 18:13:31.279192 seldegen-0.1.3/seldegen/socials/__pycache__/twitter.cpython-311.pyc
+-rw-r--r--   0        0        0     4529 2024-03-19 17:21:41.167605 seldegen-0.1.3/seldegen/socials/discord.py
+-rw-r--r--   0        0        0     4438 2024-03-14 12:16:40.439943 seldegen-0.1.3/seldegen/socials/facebook.py
+-rw-r--r--   0        0        0     3982 2024-03-19 17:17:40.610882 seldegen-0.1.3/seldegen/socials/github.py
+-rw-r--r--   0        0        0     2186 2024-03-10 14:00:33.245512 seldegen-0.1.3/seldegen/socials/gmail.py
+-rw-r--r--   0        0        0     5086 2024-03-15 00:29:31.085041 seldegen-0.1.3/seldegen/socials/google.py
+-rw-r--r--   0        0        0     4004 2024-03-19 17:08:22.151688 seldegen-0.1.3/seldegen/socials/linkedin.py
+-rw-r--r--   0        0        0    10541 2024-03-19 17:24:12.014594 seldegen-0.1.3/seldegen/socials/twitter.py
+-rw-r--r--   0        0        0      304 2024-03-14 21:45:11.803532 seldegen-0.1.3/seldegen/types.py
+-rw-r--r--   0        0        0      224 2023-12-19 15:19:41.201564 seldegen-0.1.3/seldegen/wallets/__init__.py
+-rw-r--r--   0        0        0      470 2024-04-05 18:13:31.292423 seldegen-0.1.3/seldegen/wallets/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0    15424 2024-04-05 18:31:22.639471 seldegen-0.1.3/seldegen/wallets/__pycache__/metamask.cpython-311.pyc
+-rw-r--r--   0        0        0    10355 2024-04-05 18:13:31.536439 seldegen-0.1.3/seldegen/wallets/__pycache__/sui_wallet.cpython-311.pyc
+-rw-r--r--   0        0        0    11248 2024-04-07 01:47:03.066187 seldegen-0.1.3/seldegen/wallets/metamask.py
+-rw-r--r--   0        0        0     7258 2024-03-13 17:22:11.289963 seldegen-0.1.3/seldegen/wallets/sui_wallet.py
+-rw-r--r--   0        0        0     1801 1970-01-01 00:00:00.000000 seldegen-0.1.3/PKG-INFO
```

### Comparing `seldegen-0.1.2/LICENSE` & `seldegen-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `seldegen-0.1.2/README.md` & `seldegen-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `seldegen-0.1.2/pyproject.toml` & `seldegen-0.1.3/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = 'seldegen'
-version = '0.1.2'
+version = '0.1.3'
 description = 'The package containing tools to warm up Web3-based project using Selenium'
 authors = ['Alexey <axbelenkov@gmail.com>']
 license = 'MIT'
 readme = 'README.md'
 repository = 'https://github.com/blnkoff/seldegen'
 homepage = 'https://github.com/blnkoff/seldegen'
 classifiers = [
```

### Comparing `seldegen-0.1.2/seldegen/.DS_Store` & `seldegen-0.1.3/seldegen/.DS_Store`

 * *Files identical despite different names*

### Comparing `seldegen-0.1.2/seldegen/__init__.py` & `seldegen-0.1.3/seldegen/__init__.py`

 * *Files identical despite different names*

### Comparing `seldegen-0.1.2/seldegen/abc/__pycache__/__init__.cpython-311.pyc` & `seldegen-0.1.3/seldegen/abc/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `seldegen-0.1.2/seldegen/abc/__pycache__/base_account.cpython-311.pyc` & `seldegen-0.1.3/seldegen/abc/__pycache__/base_account.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `seldegen-0.1.2/seldegen/abc/__pycache__/browser_extension.cpython-311.pyc` & `seldegen-0.1.3/seldegen/abc/__pycache__/browser_extension.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `seldegen-0.1.2/seldegen/abc/__pycache__/dapp.cpython-311.pyc` & `seldegen-0.1.3/seldegen/abc/__pycache__/dapp.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `seldegen-0.1.2/seldegen/abc/__pycache__/wallet.cpython-311.pyc` & `seldegen-0.1.3/seldegen/abc/__pycache__/wallet.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `seldegen-0.1.2/seldegen/abc/base_account.py` & `seldegen-0.1.3/seldegen/abc/base_account.py`

 * *Files identical despite different names*

### Comparing `seldegen-0.1.2/seldegen/abc/browser_extension.py` & `seldegen-0.1.3/seldegen/abc/browser_extension.py`

 * *Files identical despite different names*

### Comparing `seldegen-0.1.2/seldegen/abc/dapp.py` & `seldegen-0.1.3/seldegen/abc/dapp.py`

 * *Files identical despite different names*

### Comparing `seldegen-0.1.2/seldegen/abc/wallet.py` & `seldegen-0.1.3/seldegen/abc/wallet.py`

 * *Files identical despite different names*

### Comparing `seldegen-0.1.2/seldegen/captcha_solver.py` & `seldegen-0.1.3/seldegen/captcha_solver.py`

 * *Files identical despite different names*

### Comparing `seldegen-0.1.2/seldegen/captcha_waiter.py` & `seldegen-0.1.3/seldegen/captcha_waiter.py`

 * *Files identical despite different names*

### Comparing `seldegen-0.1.2/seldegen/context.py` & `seldegen-0.1.3/seldegen/context.py`

 * *Files identical despite different names*

### Comparing `seldegen-0.1.2/seldegen/dapps/__pycache__/guild.cpython-311.pyc` & `seldegen-0.1.3/seldegen/dapps/__pycache__/guild.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `seldegen-0.1.2/seldegen/dapps/__pycache__/lens.cpython-311.pyc` & `seldegen-0.1.3/seldegen/dapps/__pycache__/lens.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `seldegen-0.1.2/seldegen/dapps/__pycache__/snapshot.cpython-311.pyc` & `seldegen-0.1.3/seldegen/dapps/__pycache__/snapshot.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `seldegen-0.1.2/seldegen/dapps/guild.py` & `seldegen-0.1.3/seldegen/dapps/guild.py`

 * *Files identical despite different names*

### Comparing `seldegen-0.1.2/seldegen/dapps/lens.py` & `seldegen-0.1.3/seldegen/dapps/lens.py`

 * *Files identical despite different names*

### Comparing `seldegen-0.1.2/seldegen/dapps/snapshot.py` & `seldegen-0.1.3/seldegen/dapps/snapshot.py`

 * *Files identical despite different names*

### Comparing `seldegen-0.1.2/seldegen/email.py` & `seldegen-0.1.3/seldegen/email.py`

 * *Files identical despite different names*

### Comparing `seldegen-0.1.2/seldegen/exceptions.py` & `seldegen-0.1.3/seldegen/exceptions.py`

 * *Files identical despite different names*

### Comparing `seldegen-0.1.2/seldegen/extensions/__init__.py` & `seldegen-0.1.3/seldegen/extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `seldegen-0.1.2/seldegen/extensions/__pycache__/__init__.cpython-311.pyc` & `seldegen-0.1.3/seldegen/extensions/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `seldegen-0.1.2/seldegen/extensions/__pycache__/authenticator.cpython-311.pyc` & `seldegen-0.1.3/seldegen/extensions/__pycache__/authenticator.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `seldegen-0.1.2/seldegen/extensions/__pycache__/capmonster.cpython-311.pyc` & `seldegen-0.1.3/seldegen/extensions/__pycache__/capmonster.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `seldegen-0.1.2/seldegen/extensions/authenticator.py` & `seldegen-0.1.3/seldegen/extensions/authenticator.py`

 * *Files identical despite different names*

### Comparing `seldegen-0.1.2/seldegen/extensions/capmonster.py` & `seldegen-0.1.3/seldegen/extensions/capmonster.py`

 * *Files identical despite different names*

### Comparing `seldegen-0.1.2/seldegen/socials/__pycache__/__init__.cpython-311.pyc` & `seldegen-0.1.3/seldegen/socials/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `seldegen-0.1.2/seldegen/socials/__pycache__/discord.cpython-311.pyc` & `seldegen-0.1.3/seldegen/socials/__pycache__/discord.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `seldegen-0.1.2/seldegen/socials/__pycache__/facebook.cpython-311.pyc` & `seldegen-0.1.3/seldegen/socials/__pycache__/facebook.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `seldegen-0.1.2/seldegen/socials/__pycache__/github.cpython-311.pyc` & `seldegen-0.1.3/seldegen/socials/__pycache__/github.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `seldegen-0.1.2/seldegen/socials/__pycache__/gmail.cpython-311.pyc` & `seldegen-0.1.3/seldegen/socials/__pycache__/gmail.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `seldegen-0.1.2/seldegen/socials/__pycache__/google.cpython-311.pyc` & `seldegen-0.1.3/seldegen/socials/__pycache__/google.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `seldegen-0.1.2/seldegen/socials/__pycache__/linkedin.cpython-311.pyc` & `seldegen-0.1.3/seldegen/socials/__pycache__/linkedin.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `seldegen-0.1.2/seldegen/socials/__pycache__/twitter.cpython-311.pyc` & `seldegen-0.1.3/seldegen/socials/__pycache__/twitter.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `seldegen-0.1.2/seldegen/socials/discord.py` & `seldegen-0.1.3/seldegen/socials/discord.py`

 * *Files identical despite different names*

### Comparing `seldegen-0.1.2/seldegen/socials/facebook.py` & `seldegen-0.1.3/seldegen/socials/facebook.py`

 * *Files identical despite different names*

### Comparing `seldegen-0.1.2/seldegen/socials/github.py` & `seldegen-0.1.3/seldegen/socials/github.py`

 * *Files identical despite different names*

### Comparing `seldegen-0.1.2/seldegen/socials/gmail.py` & `seldegen-0.1.3/seldegen/socials/gmail.py`

 * *Files identical despite different names*

### Comparing `seldegen-0.1.2/seldegen/socials/google.py` & `seldegen-0.1.3/seldegen/socials/google.py`

 * *Files identical despite different names*

### Comparing `seldegen-0.1.2/seldegen/socials/linkedin.py` & `seldegen-0.1.3/seldegen/socials/linkedin.py`

 * *Files identical despite different names*

### Comparing `seldegen-0.1.2/seldegen/socials/twitter.py` & `seldegen-0.1.3/seldegen/socials/twitter.py`

 * *Files identical despite different names*

### Comparing `seldegen-0.1.2/seldegen/wallets/__pycache__/metamask.cpython-311.pyc` & `seldegen-0.1.3/seldegen/wallets/__pycache__/metamask.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `seldegen-0.1.2/seldegen/wallets/__pycache__/sui_wallet.cpython-311.pyc` & `seldegen-0.1.3/seldegen/wallets/__pycache__/sui_wallet.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `seldegen-0.1.2/seldegen/wallets/metamask.py` & `seldegen-0.1.3/seldegen/wallets/metamask.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,14 +43,16 @@
             mnemonic,
             extension_url,
             extension_id,
             public_key=public_key,
             private_key=private_key
         )
 
+        self.__popup_closed = False
+
     @staticmethod
     def __agree_to_terms(driver: WebDriver, signing_type: _SigningType) -> None:
         action_performer = ActionPerformer(driver)
 
         checkbox_xpath = '//*[@id="onboarding__terms-checkbox"]'
         action_performer.click(_DEFAULT_TIMEOUT, checkbox_xpath)
 
@@ -186,30 +188,36 @@
         cls.__agree_to_terms(driver, signing_type)
         cls.__create_password(driver, signing_type, password)
         mnemonic = cls.__get_mnemonic(driver)
         cls.__verify_mnemonic(driver, mnemonic)
         cls.__complete(driver)
         return cls(driver, password, ' '.join(mnemonic), extension_id)
 
+    def __close_pop_up(self) -> None:
+        action_performer = self._action_performer
+        if not self.__popup_closed:
+            action_performer.click(_DEFAULT_TIMEOUT, '//button[@data-testid="popover-close"]',
+                                   ignored_exceptions=TimeoutException)
+
     def import_account(self, private_key: str) -> None:
         """
         Imports an account using a private key
         :param private_key: A private key of Metamask wallet
         :return: None
         """
         driver = self.driver
         driver.get(self.extension_url)
         action_performer = self._action_performer
 
         account = Account.from_key(private_key)
         public_key = account.address
 
         time.sleep(2)
-        action_performer.click(_DEFAULT_TIMEOUT, '//button[@data-testid="popover-close"]',
-                               ignored_exceptions=TimeoutException)
+
+        self.__close_pop_up()
         action_performer.click(_DEFAULT_TIMEOUT, '//button[@data-testid="account-menu-icon"]')
         action_performer.click(_DEFAULT_TIMEOUT, '//*[@id="popover-content"]/div/div/section/div[2]/div/div[2]/div[2]/button')
         action_performer.send_keys(_DEFAULT_TIMEOUT, '//input[@id="private-key-box"]', private_key)
         action_performer.click(_DEFAULT_TIMEOUT, '//button[@data-testid="import-account-confirm-button"]')
 
         self._private_key = private_key
         self._public_key = public_key
@@ -217,16 +225,15 @@
 
     @handle_in_new_tab()
     def switch_network(self, network: str):
         driver = self.driver
         driver.get(self.extension_url)
         action_performer = self._action_performer
 
-        action_performer.click(_DEFAULT_TIMEOUT, '//button[@data-testid="popover-close"]',
-                               ignored_exceptions=TimeoutException)
+        self.__close_pop_up()
 
         network_menu_xpath = '//button[contains(@class, "mm-picker-network")]'
         action_performer.click(_DEFAULT_TIMEOUT, network_menu_xpath)
 
         toogle_xpath = '//label[contains(@class, "toggle-button")]'
         toogle_element = action_performer.get_element(_DEFAULT_TIMEOUT, toogle_xpath)
         if 'off' in toogle_element.get_attribute('class'):
```

### Comparing `seldegen-0.1.2/seldegen/wallets/sui_wallet.py` & `seldegen-0.1.3/seldegen/wallets/sui_wallet.py`

 * *Files identical despite different names*

### Comparing `seldegen-0.1.2/PKG-INFO` & `seldegen-0.1.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seldegen
-Version: 0.1.2
+Version: 0.1.3
 Summary: The package containing tools to warm up Web3-based project using Selenium
 Home-page: https://github.com/blnkoff/seldegen
 License: MIT
 Author: Alexey
 Author-email: axbelenkov@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 4 - Beta
```

