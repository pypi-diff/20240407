# Comparing `tmp/rlotp-0.0.7.tar.gz` & `tmp/rlotp-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rlotp-0.0.7.tar", last modified: Tue Apr  2 08:24:22 2024, max compression
+gzip compressed data, was "rlotp-0.0.8.tar", last modified: Sun Apr  7 05:07:07 2024, max compression
```

## Comparing `rlotp-0.0.7.tar` & `rlotp-0.0.8.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 jahid     (1000) jahid     (1001)        0 2024-04-02 08:24:22.901250 rlotp-0.0.7/
--rw-r--r--   0 jahid     (1000) jahid     (1001)     1174 2024-03-31 05:37:56.000000 rlotp-0.0.7/LICENSE
--rw-r--r--   0 jahid     (1000) jahid     (1001)       51 2024-03-31 05:27:57.000000 rlotp-0.0.7/MANIFEST.in
--rw-r--r--   0 jahid     (1000) jahid     (1001)     9606 2024-04-02 08:24:22.901250 rlotp-0.0.7/PKG-INFO
--rw-r--r--   0 jahid     (1000) jahid     (1001)     8535 2024-03-31 05:38:54.000000 rlotp-0.0.7/README.rst
--rw-r--r--   0 jahid     (1000) jahid     (1001)      112 2024-03-31 05:27:57.000000 rlotp-0.0.7/pyproject.toml
--rw-r--r--   0 jahid     (1000) jahid     (1001)       38 2024-04-02 08:24:22.901250 rlotp-0.0.7/setup.cfg
--rwxr-xr-x   0 jahid     (1000) jahid     (1001)     2063 2024-03-31 13:41:58.000000 rlotp-0.0.7/setup.py
-drwxr-xr-x   0 jahid     (1000) jahid     (1001)        0 2024-04-02 08:24:22.897916 rlotp-0.0.7/src/
-drwxr-xr-x   0 jahid     (1000) jahid     (1001)        0 2024-04-02 08:24:22.901250 rlotp-0.0.7/src/rlotp/
--rw-r--r--   0 jahid     (1000) jahid     (1001)     4338 2024-04-02 08:24:13.000000 rlotp-0.0.7/src/rlotp/__init__.py
--rw-r--r--   0 jahid     (1000) jahid     (1001)      217 2024-03-31 13:41:58.000000 rlotp-0.0.7/src/rlotp/compat.py
--rw-r--r--   0 jahid     (1000) jahid     (1001)     1750 2024-04-02 08:24:13.000000 rlotp-0.0.7/src/rlotp/hotp.py
--rw-r--r--   0 jahid     (1000) jahid     (1001)     3300 2024-04-02 08:24:13.000000 rlotp-0.0.7/src/rlotp/otp.py
--rw-r--r--   0 jahid     (1000) jahid     (1001)        0 2024-03-31 13:41:58.000000 rlotp-0.0.7/src/rlotp/py.typed
--rw-r--r--   0 jahid     (1000) jahid     (1001)      122 2024-03-31 13:41:58.000000 rlotp-0.0.7/src/rlotp/steam.py
--rw-r--r--   0 jahid     (1000) jahid     (1001)     5579 2024-04-02 08:24:13.000000 rlotp-0.0.7/src/rlotp/totp.py
--rw-r--r--   0 jahid     (1000) jahid     (1001)     4114 2024-04-02 08:24:13.000000 rlotp-0.0.7/src/rlotp/utils.py
--rw-r--r--   0 jahid     (1000) jahid     (1001)       89 2024-04-02 08:24:13.000000 rlotp-0.0.7/src/rlotp/version.py
-drwxr-xr-x   0 jahid     (1000) jahid     (1001)        0 2024-04-02 08:24:22.901250 rlotp-0.0.7/src/rlotp.egg-info/
--rw-r--r--   0 jahid     (1000) jahid     (1001)     9606 2024-04-02 08:24:22.000000 rlotp-0.0.7/src/rlotp.egg-info/PKG-INFO
--rw-r--r--   0 jahid     (1000) jahid     (1001)      399 2024-04-02 08:24:22.000000 rlotp-0.0.7/src/rlotp.egg-info/SOURCES.txt
--rw-r--r--   0 jahid     (1000) jahid     (1001)        1 2024-04-02 08:24:22.000000 rlotp-0.0.7/src/rlotp.egg-info/dependency_links.txt
--rw-r--r--   0 jahid     (1000) jahid     (1001)        1 2024-04-02 08:24:22.000000 rlotp-0.0.7/src/rlotp.egg-info/not-zip-safe
--rw-r--r--   0 jahid     (1000) jahid     (1001)        6 2024-04-02 08:24:22.000000 rlotp-0.0.7/src/rlotp.egg-info/top_level.txt
--rwxr-xr-x   0 jahid     (1000) jahid     (1001)    20360 2024-04-02 08:24:13.000000 rlotp-0.0.7/test.py
+drwxr-xr-x   0 jahid     (1000) jahid     (1001)        0 2024-04-07 05:07:07.891113 rlotp-0.0.8/
+-rw-r--r--   0 jahid     (1000) jahid     (1001)     1174 2024-03-31 05:37:56.000000 rlotp-0.0.8/LICENSE
+-rw-r--r--   0 jahid     (1000) jahid     (1001)       51 2024-03-31 05:27:57.000000 rlotp-0.0.8/MANIFEST.in
+-rw-r--r--   0 jahid     (1000) jahid     (1001)     9606 2024-04-07 05:07:07.891113 rlotp-0.0.8/PKG-INFO
+-rw-r--r--   0 jahid     (1000) jahid     (1001)     8535 2024-03-31 05:38:54.000000 rlotp-0.0.8/README.rst
+-rw-r--r--   0 jahid     (1000) jahid     (1001)      112 2024-03-31 05:27:57.000000 rlotp-0.0.8/pyproject.toml
+-rw-r--r--   0 jahid     (1000) jahid     (1001)       38 2024-04-07 05:07:07.891113 rlotp-0.0.8/setup.cfg
+-rwxr-xr-x   0 jahid     (1000) jahid     (1001)     2063 2024-03-31 13:41:58.000000 rlotp-0.0.8/setup.py
+drwxr-xr-x   0 jahid     (1000) jahid     (1001)        0 2024-04-07 05:07:07.891113 rlotp-0.0.8/src/
+drwxr-xr-x   0 jahid     (1000) jahid     (1001)        0 2024-04-07 05:07:07.891113 rlotp-0.0.8/src/rlotp/
+-rw-r--r--   0 jahid     (1000) jahid     (1001)     4338 2024-04-02 08:24:13.000000 rlotp-0.0.8/src/rlotp/__init__.py
+-rw-r--r--   0 jahid     (1000) jahid     (1001)      217 2024-03-31 13:41:58.000000 rlotp-0.0.8/src/rlotp/compat.py
+-rw-r--r--   0 jahid     (1000) jahid     (1001)     1750 2024-04-02 08:24:13.000000 rlotp-0.0.8/src/rlotp/hotp.py
+-rw-r--r--   0 jahid     (1000) jahid     (1001)     3300 2024-04-02 08:24:13.000000 rlotp-0.0.8/src/rlotp/otp.py
+-rw-r--r--   0 jahid     (1000) jahid     (1001)        0 2024-03-31 13:41:58.000000 rlotp-0.0.8/src/rlotp/py.typed
+-rw-r--r--   0 jahid     (1000) jahid     (1001)      122 2024-03-31 13:41:58.000000 rlotp-0.0.8/src/rlotp/steam.py
+-rw-r--r--   0 jahid     (1000) jahid     (1001)     5581 2024-04-07 05:06:57.000000 rlotp-0.0.8/src/rlotp/totp.py
+-rw-r--r--   0 jahid     (1000) jahid     (1001)     4114 2024-04-07 05:05:46.000000 rlotp-0.0.8/src/rlotp/utils.py
+-rw-r--r--   0 jahid     (1000) jahid     (1001)       89 2024-04-07 05:06:57.000000 rlotp-0.0.8/src/rlotp/version.py
+drwxr-xr-x   0 jahid     (1000) jahid     (1001)        0 2024-04-07 05:07:07.891113 rlotp-0.0.8/src/rlotp.egg-info/
+-rw-r--r--   0 jahid     (1000) jahid     (1001)     9606 2024-04-07 05:07:07.000000 rlotp-0.0.8/src/rlotp.egg-info/PKG-INFO
+-rw-r--r--   0 jahid     (1000) jahid     (1001)      399 2024-04-07 05:07:07.000000 rlotp-0.0.8/src/rlotp.egg-info/SOURCES.txt
+-rw-r--r--   0 jahid     (1000) jahid     (1001)        1 2024-04-07 05:07:07.000000 rlotp-0.0.8/src/rlotp.egg-info/dependency_links.txt
+-rw-r--r--   0 jahid     (1000) jahid     (1001)        1 2024-04-07 05:07:07.000000 rlotp-0.0.8/src/rlotp.egg-info/not-zip-safe
+-rw-r--r--   0 jahid     (1000) jahid     (1001)        6 2024-04-07 05:07:07.000000 rlotp-0.0.8/src/rlotp.egg-info/top_level.txt
+-rwxr-xr-x   0 jahid     (1000) jahid     (1001)    20360 2024-04-02 08:24:13.000000 rlotp-0.0.8/test.py
```

### Comparing `rlotp-0.0.7/LICENSE` & `rlotp-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `rlotp-0.0.7/PKG-INFO` & `rlotp-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rlotp
-Version: 0.0.7
+Version: 0.0.8
 Summary: Random Length OTP Library in Python
 Home-page: https://github.com/rlotp/rlotp
 Author: Md. Jahidul Hamid & PyOTP contributors
 Author-email: jahidulhamid@yahoo.com
 License: MIT License
 Project-URL: Documentation, https://neurobin.github.io/rlotp
 Project-URL: Source Code, https://github.com/neurobin/rlotp
```

### Comparing `rlotp-0.0.7/README.rst` & `rlotp-0.0.8/README.rst`

 * *Files identical despite different names*

### Comparing `rlotp-0.0.7/setup.py` & `rlotp-0.0.8/setup.py`

 * *Files identical despite different names*

### Comparing `rlotp-0.0.7/src/rlotp/__init__.py` & `rlotp-0.0.8/src/rlotp/__init__.py`

 * *Files identical despite different names*

### Comparing `rlotp-0.0.7/src/rlotp/hotp.py` & `rlotp-0.0.8/src/rlotp/hotp.py`

 * *Files identical despite different names*

### Comparing `rlotp-0.0.7/src/rlotp/otp.py` & `rlotp-0.0.8/src/rlotp/otp.py`

 * *Files identical despite different names*

### Comparing `rlotp-0.0.7/src/rlotp/totp.py` & `rlotp-0.0.8/src/rlotp/totp.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         :param issuer: issuer
         :param period: the time period in seconds for OTP. This defaults to 30.
         """
         self.rdigits = None
         if rdigits:
             if rdigits[0] < 6 or rdigits[1] > 10:
                 raise ValueError("rdigits must be between 6 and 10")
-            self.rdigits = (rdigits[0], rdigits[1] + 1)
+            self.rdigits = rdigits
         if digest is None:
             digest = hashlib.sha1
 
         self.secret = secret
         self.digits = digits
         self.digest = digest
         self.name = name or 'Secret'
@@ -63,15 +63,15 @@
             time_remaining = totp.period - datetime.datetime.now().timestamp() % totp.period
 
         :param for_time: the time to generate an OTP for
         :param counter_offset: the amount of ticks to add to the time counter
         :returns: OTP value
         """
         if self.rdigits:
-            ns = range(*self.rdigits)
+            ns = range(self.rdigits[0], self.rdigits[1] + 1)
             n = len(str(len(ns)))
             otp1 = OTP(self.secret, digits=n, digest=self.digest, name=self.name, issuer=self.issuer)
             digits = utils.normalize(int(otp1.generate_otp(self.timecode(for_time) + counter_offset) if for_time else counter_offset), ns)
         else:
             digits = self.digits
 
         otp = OTP(self.secret, digits=digits, digest=self.digest, name=self.name, issuer=self.issuer, chargroup=self.chargroup, encoder=self.encoder)
```

### Comparing `rlotp-0.0.7/src/rlotp/utils.py` & `rlotp-0.0.8/src/rlotp/utils.py`

 * *Files identical despite different names*

### Comparing `rlotp-0.0.7/src/rlotp.egg-info/PKG-INFO` & `rlotp-0.0.8/src/rlotp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rlotp
-Version: 0.0.7
+Version: 0.0.8
 Summary: Random Length OTP Library in Python
 Home-page: https://github.com/rlotp/rlotp
 Author: Md. Jahidul Hamid & PyOTP contributors
 Author-email: jahidulhamid@yahoo.com
 License: MIT License
 Project-URL: Documentation, https://neurobin.github.io/rlotp
 Project-URL: Source Code, https://github.com/neurobin/rlotp
```

### Comparing `rlotp-0.0.7/test.py` & `rlotp-0.0.8/test.py`

 * *Files identical despite different names*

