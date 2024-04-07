# Comparing `tmp/py-libtrust-1.0.5.tar.gz` & `tmp/py_libtrust-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-libtrust-1.0.5.tar", max compression
+gzip compressed data, was "py_libtrust-2.0.0.tar", max compression
```

## Comparing `py-libtrust-1.0.5.tar` & `py_libtrust-2.0.0.tar`

### file list

```diff
@@ -1,14 +1,13 @@
--rw-r--r--   0        0        0    11357 2022-04-15 04:39:19.823217 py-libtrust-1.0.5/LICENSE
--rw-r--r--   0        0        0     1881 2022-04-15 04:39:19.823217 py-libtrust-1.0.5/README.md
--rw-r--r--   0        0        0      373 2022-04-15 04:39:19.823217 py-libtrust-1.0.5/libtrust/__init__.py
--rw-r--r--   0        0        0      137 2022-04-15 04:39:19.823217 py-libtrust-1.0.5/libtrust/exceptions.py
--rw-r--r--   0        0        0     9432 2022-04-15 04:39:19.823217 py-libtrust-1.0.5/libtrust/jsonsign.py
--rw-r--r--   0        0        0        0 2022-04-15 04:39:19.823217 py-libtrust-1.0.5/libtrust/keys/__init__.py
--rw-r--r--   0        0        0     8953 2022-04-15 04:39:19.823217 py-libtrust-1.0.5/libtrust/keys/ec_key.py
--rw-r--r--   0        0        0     3677 2022-04-15 04:39:19.823217 py-libtrust-1.0.5/libtrust/keys/protocol.py
--rw-r--r--   0        0        0     7331 2022-04-15 04:39:19.823217 py-libtrust-1.0.5/libtrust/keys/rs_key.py
--rw-r--r--   0        0        0     2601 2022-04-15 04:39:19.823217 py-libtrust-1.0.5/libtrust/keys/utils.py
--rw-r--r--   0        0        0     1409 2022-04-15 04:39:19.823217 py-libtrust-1.0.5/libtrust/utils.py
--rw-r--r--   0        0        0      815 2022-04-15 04:39:19.823217 py-libtrust-1.0.5/pyproject.toml
--rw-r--r--   0        0        0     2662 2022-04-15 04:39:28.113163 py-libtrust-1.0.5/setup.py
--rw-r--r--   0        0        0     2685 2022-04-15 04:39:28.113522 py-libtrust-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-07 07:13:33.594837 py_libtrust-2.0.0/LICENSE
+-rw-r--r--   0        0        0     1881 2024-04-07 07:13:33.594837 py_libtrust-2.0.0/README.md
+-rw-r--r--   0        0        0      373 2024-04-07 07:13:33.594837 py_libtrust-2.0.0/libtrust/__init__.py
+-rw-r--r--   0        0        0      137 2024-04-07 07:13:33.594837 py_libtrust-2.0.0/libtrust/exceptions.py
+-rw-r--r--   0        0        0     9432 2024-04-07 07:13:33.594837 py_libtrust-2.0.0/libtrust/jsonsign.py
+-rw-r--r--   0        0        0        0 2024-04-07 07:13:33.594837 py_libtrust-2.0.0/libtrust/keys/__init__.py
+-rw-r--r--   0        0        0     8898 2024-04-07 07:13:33.594837 py_libtrust-2.0.0/libtrust/keys/ec_key.py
+-rw-r--r--   0        0        0     3677 2024-04-07 07:13:33.594837 py_libtrust-2.0.0/libtrust/keys/protocol.py
+-rw-r--r--   0        0        0     7247 2024-04-07 07:13:33.594837 py_libtrust-2.0.0/libtrust/keys/rs_key.py
+-rw-r--r--   0        0        0     2601 2024-04-07 07:13:33.594837 py_libtrust-2.0.0/libtrust/keys/utils.py
+-rw-r--r--   0        0        0     1409 2024-04-07 07:13:33.594837 py_libtrust-2.0.0/libtrust/utils.py
+-rw-r--r--   0        0        0      812 2024-04-07 07:13:33.594837 py_libtrust-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     2784 1970-01-01 00:00:00.000000 py_libtrust-2.0.0/PKG-INFO
```

### Comparing `py-libtrust-1.0.5/LICENSE` & `py_libtrust-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `py-libtrust-1.0.5/README.md` & `py_libtrust-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `py-libtrust-1.0.5/libtrust/jsonsign.py` & `py_libtrust-2.0.0/libtrust/jsonsign.py`

 * *Files identical despite different names*

### Comparing `py-libtrust-1.0.5/libtrust/keys/ec_key.py` & `py_libtrust-2.0.0/libtrust/keys/ec_key.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,23 @@
 from typing import BinaryIO, Dict, Optional, Type, Union
 
 from cryptography.hazmat.backends import default_backend
 from cryptography.hazmat.primitives import hashes, serialization
 from cryptography.hazmat.primitives.asymmetric import ec
-from cryptography.hazmat.primitives.asymmetric.utils import decode_dss_signature, encode_dss_signature
+from cryptography.hazmat.primitives.asymmetric.utils import (
+    decode_dss_signature,
+    encode_dss_signature,
+)
 from cryptography.utils import int_to_bytes
 
-from libtrust.keys.utils import decode_ec_coordinate, encode_ec_coordinate, encode_key_id_from_crypto_key
+from libtrust.keys.utils import (
+    decode_ec_coordinate,
+    encode_ec_coordinate,
+    encode_key_id_from_crypto_key,
+)
 
 __all__ = ["ECPublicKey", "ECPrivateKey", "generate_private_key"]
 
 
 class ECPublicKey:
     """Usage for ECPublicKey:
     call ``verify`` to verify the signature for data in buffer.
@@ -22,15 +29,18 @@
         if not isinstance(key, ec.EllipticCurvePublicKey):
             raise ValueError("`key` is not a EllipticCurvePublicKey")
         self._public_key = key
 
     def __eq__(self, other):
         if not isinstance(other, ECPublicKey):
             return False
-        return self.crypto_public_key().public_numbers() == other.crypto_public_key().public_numbers()
+        return (
+            self.crypto_public_key().public_numbers()
+            == other.crypto_public_key().public_numbers()
+        )
 
     @classmethod
     def key_type(cls) -> str:
         return "EC"
 
     def key_id(self) -> str:
         return encode_key_id_from_crypto_key(self.crypto_public_key())
@@ -73,15 +83,17 @@
         if crv not in _curve_names_map_to_curves:
             raise Exception(f"JWK EC Public Key curve identifier not supported: {crv}")
 
         curve = _curve_names_map_to_curves[crv]()
         x = decode_ec_coordinate(jwk["x"], curve)
         y = decode_ec_coordinate(jwk["y"], curve)
 
-        return cls(ec.EllipticCurvePublicNumbers(x, y, curve).public_key(default_backend()))
+        return cls(
+            ec.EllipticCurvePublicNumbers(x, y, curve).public_key(default_backend())
+        )
 
     def verify(
         self,
         buffer: BinaryIO,
         alg: str,
         signature: bytes,
         *,
@@ -93,33 +105,29 @@
             raise Exception(
                 f"unable to verify signature: "
                 f"EC Public Key with curve {curve_name} does not support signature algorithm {alg}"
             )
 
         expected_octet_length = 2 * ((crypto_public_key.curve.key_size + 7) >> 3)
         if expected_octet_length != len(signature):
-            raise Exception(f"signature length is {len(signature)} octets long, should be {expected_octet_length}")
+            raise Exception(
+                f"signature length is {len(signature)} octets long, should be {expected_octet_length}"
+            )
 
         sig_length = len(signature)
         r_bytes, s_bytes = signature[: sig_length // 2], signature[sig_length // 2 :]
 
         r = int.from_bytes(r_bytes, "big")
         s = int.from_bytes(s_bytes, "big")
 
         signature = encode_dss_signature(r, s)
         hash_algorithm = _hash_algorithm_maps[_curve_names_map_to_alg[curve_name]]
-        verifier = crypto_public_key.verifier(signature, ec.ECDSA(hash_algorithm))
-        while True:
-            d = buffer.read(1024)
-            if not d:
-                break
-            verifier.update(d)
 
         try:
-            verifier.verify()
+            crypto_public_key.verify(signature, buffer.read(), ec.ECDSA(hash_algorithm))
             return True
         except Exception:
             if raise_exception:
                 raise
             return False
 
     def curve_name(self) -> str:
@@ -139,15 +147,18 @@
             raise ValueError("`key` is not a EllipticCurvePrivateKeyWithSerialization")
         super(ECPrivateKey, self).__init__(key.public_key())
         self._private_key = key
 
     def __eq__(self, other):
         if not isinstance(other, ECPrivateKey):
             return False
-        return self.crypto_private_key().private_numbers() == other.crypto_private_key().private_numbers()
+        return (
+            self.crypto_private_key().private_numbers()
+            == other.crypto_private_key().private_numbers()
+        )
 
     def public_key(self) -> ECPublicKey:
         return ECPublicKey(self.crypto_public_key())
 
     def crypto_private_key(self) -> ec.EllipticCurvePrivateKeyWithSerialization:
         return self._private_key
 
@@ -159,15 +170,17 @@
                 serialization.PrivateFormat.PKCS8,
                 serialization.NoEncryption(),
             )
             .decode()
         )
 
     @classmethod
-    def from_pem(cls, pem: Union[str, bytes], password: Optional[bytes] = None) -> "ECPrivateKey":
+    def from_pem(
+        cls, pem: Union[str, bytes], password: Optional[bytes] = None
+    ) -> "ECPrivateKey":
         if isinstance(pem, str):
             pem = pem.encode()
         return cls(serialization.load_pem_private_key(pem, password, default_backend()))
 
     def to_jwk(self) -> Dict:
         jwk = super().to_jwk()
         jwk["d"] = encode_ec_coordinate(
@@ -186,32 +199,30 @@
 
         curve = _curve_names_map_to_curves[crv]()
         x = decode_ec_coordinate(jwk["x"], curve)
         y = decode_ec_coordinate(jwk["y"], curve)
         d = decode_ec_coordinate(jwk["d"], curve)
 
         return cls(
-            ec.EllipticCurvePrivateNumbers(d, ec.EllipticCurvePublicNumbers(x, y, curve)).private_key(
-                default_backend()
-            )
+            ec.EllipticCurvePrivateNumbers(
+                d, ec.EllipticCurvePublicNumbers(x, y, curve)
+            ).private_key(default_backend())
         )
 
     def sign(self, buffer: BinaryIO, hash_id: hashes.HashAlgorithm):
         crypto_private_key = self.crypto_private_key()
         crypto_algorithm = _curve_names_map_to_alg[self.curve_name()]
         hash_algorithm = _hash_algorithm_maps[crypto_algorithm]
-        signer = crypto_private_key.signer(ec.ECDSA(hash_algorithm))
 
-        while True:
-            d = buffer.read(1024)
-            if not d:
-                break
-            signer.update(d)
+        dss_signature = crypto_private_key.sign(
+            buffer.read(),
+            ec.ECDSA(hash_algorithm),
+        )
 
-        r, s = decode_dss_signature(signer.finalize())
+        r, s = decode_dss_signature(dss_signature)
         r_bytes = int_to_bytes(r)
         s_bytes = int_to_bytes(s)
         octet_length = (crypto_private_key.curve.key_size + 7) >> 3
 
         r_bytes = b"\x00" * (octet_length - len(r_bytes)) + r_bytes
         s_bytes = b"\x00" * (octet_length - len(s_bytes)) + s_bytes
         signature = r_bytes + s_bytes
@@ -219,15 +230,17 @@
 
 
 _curves_map_to_curve_names: Dict[Type[ec.EllipticCurve], str] = {
     ec.SECP256R1: "P-256",
     ec.SECP384R1: "P-384",
     ec.SECP521R1: "P-521",
 }
-_curve_names_map_to_curves: Dict[str, Type[ec.EllipticCurve]] = {v: k for k, v in _curves_map_to_curve_names.items()}
+_curve_names_map_to_curves: Dict[str, Type[ec.EllipticCurve]] = {
+    v: k for k, v in _curves_map_to_curve_names.items()
+}
 
 _curve_names_map_to_alg: Dict[str, str] = {
     "P-256": "ES256",
     "P-384": "ES384",
     "P-521": "ES521",
 }
 _alg_map_to_curve_names = {v: k for k, v in _curve_names_map_to_alg.items()}
```

### Comparing `py-libtrust-1.0.5/libtrust/keys/protocol.py` & `py_libtrust-2.0.0/libtrust/keys/protocol.py`

 * *Files identical despite different names*

### Comparing `py-libtrust-1.0.5/libtrust/keys/rs_key.py` & `py_libtrust-2.0.0/libtrust/keys/rs_key.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,18 @@
         if not isinstance(key, rsa.RSAPublicKey):
             raise ValueError("`key` is not a RSAPublicKey")
         self._public_key = key
 
     def __eq__(self, other):
         if not isinstance(other, RSAPublicKey):
             return False
-        return self.crypto_public_key().public_numbers() == other.crypto_public_key().public_numbers()
+        return (
+            self.crypto_public_key().public_numbers()
+            == other.crypto_public_key().public_numbers()
+        )
 
     @classmethod
     def key_type(cls) -> str:
         return "RSA"
 
     def key_id(self) -> str:
         return encode_key_id_from_crypto_key(self.crypto_public_key())
@@ -79,27 +82,21 @@
         *,
         raise_exception: bool = True,
     ) -> bool:
         hash_algorithm = _hash_algorithm_maps.get(alg, None)
         if hash_algorithm is None:
             raise Exception(f"RSA Digital Signature Algorithm {alg} not supported")
 
-        verifier = self.crypto_public_key().verifier(
-            signature,
-            padding.PKCS1v15(),
-            hash_algorithm,
-        )
-        while True:
-            d = buffer.read(1024)
-            if not d:
-                break
-            verifier.update(d)
-
         try:
-            verifier.verify()
+            self.crypto_public_key().verify(
+                signature,
+                buffer.read(),
+                padding.PKCS1v15(),
+                hash_algorithm,
+            )
             return True
         except Exception:
             if raise_exception:
                 raise
             return False
 
 
@@ -116,15 +113,18 @@
             raise ValueError("`key` is not a RSAPrivateKey")
         super().__init__(key.public_key())
         self._private_key = key
 
     def __eq__(self, other):
         if not isinstance(other, RSAPrivateKey):
             return False
-        return self.crypto_private_key().private_numbers() == other.crypto_private_key().private_numbers()
+        return (
+            self.crypto_private_key().private_numbers()
+            == other.crypto_private_key().private_numbers()
+        )
 
     def public_key(self) -> RSAPublicKey:
         return RSAPublicKey(self.crypto_public_key())
 
     def crypto_private_key(self) -> rsa.RSAPrivateKeyWithSerialization:
         return self._private_key
 
@@ -136,15 +136,17 @@
                 serialization.PrivateFormat.PKCS8,
                 serialization.NoEncryption(),
             )
             .decode()
         )
 
     @classmethod
-    def from_pem(cls, pem: Union[str, bytes], password: Optional[bytes] = None) -> "RSAPrivateKey":
+    def from_pem(
+        cls, pem: Union[str, bytes], password: Optional[bytes] = None
+    ) -> "RSAPrivateKey":
         if isinstance(pem, str):
             pem = pem.encode()
         return cls(serialization.load_pem_private_key(pem, password, default_backend()))
 
     def to_jwk(self) -> Dict:
         jwk = super().to_jwk()
         private_numbers = self.crypto_private_key().private_numbers()
@@ -166,28 +168,26 @@
         p = int.from_bytes(jose_base64_url_decode(jwk["p"]), "big")
         q = int.from_bytes(jose_base64_url_decode(jwk["q"]), "big")
         dmp1 = int.from_bytes(jose_base64_url_decode(jwk["dp"]), "big")
         dmq1 = int.from_bytes(jose_base64_url_decode(jwk["dq"]), "big")
         iqmp = int.from_bytes(jose_base64_url_decode(jwk["qi"]), "big")
 
         return cls(
-            rsa.RSAPrivateNumbers(p, q, d, dmp1, dmq1, iqmp, rsa.RSAPublicNumbers(e, n)).private_key(default_backend())
+            rsa.RSAPrivateNumbers(
+                p, q, d, dmp1, dmq1, iqmp, rsa.RSAPublicNumbers(e, n)
+            ).private_key(default_backend())
         )
 
     def sign(self, buffer, hash_id):
         crypto_algorithm = _alg_maps.get(hash_id, "RS256")
         hash_algorithm = _hash_algorithm_maps[crypto_algorithm]
-        signer = self.crypto_private_key().signer(padding.PKCS1v15(), hash_algorithm)
-        while True:
-            d = buffer.read(1024)
-            if not d:
-                break
-            signer.update(d)
-
-        return signer.finalize(), crypto_algorithm
+        signature = self.crypto_private_key().sign(
+            buffer.read(), padding.PKCS1v15(), hash_algorithm
+        )
+        return signature, crypto_algorithm
 
 
 _alg_maps: Dict[Type[hashes.HashAlgorithm], str] = {
     hashes.SHA256: "RS256",
     hashes.SHA384: "RS384",
     hashes.SHA512: "RS512",
 }
@@ -196,9 +196,13 @@
 _hash_algorithm_maps: Dict[str, hashes.HashAlgorithm] = {
     "RS256": hashes.SHA256(),
     "RS384": hashes.SHA384(),
     "RS512": hashes.SHA512(),
 }
 
 
-def generate_private_key(key_size: int = 2048, public_exponent: int = 65537) -> RSAPrivateKey:
-    return RSAPrivateKey(rsa.generate_private_key(public_exponent, key_size, default_backend()))
+def generate_private_key(
+    key_size: int = 2048, public_exponent: int = 65537
+) -> RSAPrivateKey:
+    return RSAPrivateKey(
+        rsa.generate_private_key(public_exponent, key_size, default_backend())
+    )
```

### Comparing `py-libtrust-1.0.5/libtrust/keys/utils.py` & `py_libtrust-2.0.0/libtrust/keys/utils.py`

 * *Files identical despite different names*

### Comparing `py-libtrust-1.0.5/libtrust/utils.py` & `py_libtrust-2.0.0/libtrust/utils.py`

 * *Files identical despite different names*

### Comparing `py-libtrust-1.0.5/pyproject.toml` & `py_libtrust-2.0.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "py-libtrust"
-version = "1.0.5"
+version = "2.0.0"
 description = "Yet another docker/libtrust implement by python."
 license = "Apache-2.0"
 authors = ["shabbywu <shabbywu@qq.com>"]
 
 readme = "README.md"
 repository = "https://github.com/shabbywu/py-libtrust"
 homepage = "https://github.com/shabbywu/py-libtrust"
 
 packages = [
     {include = "libtrust"}
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.6"
-cryptography = ">= 3.0.0"
+cryptography = ">= 37"
 typing-extensions = ">= 3.6.5"
 
 [tool.poetry.dev-dependencies]
 pytest = "^6.2.5"
 pytest-cov = "^3.0.0"
 
 [build-system]
```

### Comparing `py-libtrust-1.0.5/setup.py` & `py_libtrust-2.0.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,30 +1,103 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: py-libtrust
+Version: 2.0.0
+Summary: Yet another docker/libtrust implement by python.
+Home-page: https://github.com/shabbywu/py-libtrust
+License: Apache-2.0
+Author: shabbywu
+Author-email: shabbywu@qq.com
+Requires-Python: >=3.6
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: cryptography (>=37)
+Requires-Dist: typing-extensions (>=3.6.5)
+Project-URL: Repository, https://github.com/shabbywu/py-libtrust
+Description-Content-Type: text/markdown
+
+# py-libtrust - Yet another docker/libtrust implement by python.
+
+Libtrust is library for managing authentication and authorization using public key cryptography.
+
+Works for Python 3.6+.
+
+## Usage
+
+### Install
+You can install from PyPi.
+
+```bash
+❯ pip install py-libtrust
+```
+
+### Example
+#### Sign/Verify a jose-json-web-signature
+```python
+import datetime
+from libtrust.keys.ec_key import generate_private_key
+from libtrust.jsonsign import JSONSignature
 
-packages = \
-['libtrust', 'libtrust.keys']
+# Generate a EC P256 private key
+ec_key = generate_private_key("P-256")
 
-package_data = \
-{'': ['*']}
+your_content = {
+    "author": "shabbywu(shabbywu@qq.com)"
+}
+
+# New a JSONSignature
+js = JSONSignature.new(your_content)
+
+# signature
+js.sign(ec_key, dt=datetime.datetime.utcfromtimestamp(0))
+
+jws = js.to_jws()
+
+loaded_js = JSONSignature.from_jws(jws)
+
+assert js == loaded_js
+assert js.verify() == loaded_js.verify()
+```
+
+#### Serialize/Deserialize a self-signed JSON signature
+```python
+import json
+import datetime
+from libtrust.keys.ec_key import generate_private_key
+from libtrust.jsonsign import JSONSignature
+
+# Generate a EC P256 private key
+ec_key = generate_private_key("P-256")
 
-install_requires = \
-['cryptography>=3.0.0', 'typing-extensions>=3.6.5']
-
-setup_kwargs = {
-    'name': 'py-libtrust',
-    'version': '1.0.5',
-    'description': 'Yet another docker/libtrust implement by python.',
-    'long_description': '# py-libtrust - Yet another docker/libtrust implement by python.\n\nLibtrust is library for managing authentication and authorization using public key cryptography.\n\nWorks for Python 3.6+.\n\n## Usage\n\n### Install\nYou can install from PyPi.\n\n```bash\n❯ pip install py-libtrust\n```\n\n### Example\n#### Sign/Verify a jose-json-web-signature\n```python\nimport datetime\nfrom libtrust.keys.ec_key import generate_private_key\nfrom libtrust.jsonsign import JSONSignature\n\n# Generate a EC P256 private key\nec_key = generate_private_key("P-256")\n\nyour_content = {\n    "author": "shabbywu(shabbywu@qq.com)"\n}\n\n# New a JSONSignature\njs = JSONSignature.new(your_content)\n\n# signature\njs.sign(ec_key, dt=datetime.datetime.utcfromtimestamp(0))\n\njws = js.to_jws()\n\nloaded_js = JSONSignature.from_jws(jws)\n\nassert js == loaded_js\nassert js.verify() == loaded_js.verify()\n```\n\n#### Serialize/Deserialize a self-signed JSON signature\n```python\nimport json\nimport datetime\nfrom libtrust.keys.ec_key import generate_private_key\nfrom libtrust.jsonsign import JSONSignature\n\n# Generate a EC P256 private key\nec_key = generate_private_key("P-256")\n\nyour_content = {\n    "author": "shabbywu(shabbywu@qq.com)"\n}\n\n# New a JSONSignature\njs = JSONSignature.new(your_content)\n\n# signature\njs.sign(ec_key, dt=datetime.datetime.utcfromtimestamp(0))\n\npretty_signature = js.to_pretty_signature("signatures")\nloaded_js = js.from_pretty_signature(pretty_signature)\n\nassert js.verify() == loaded_js.verify()\nassert json.loads(pretty_signature)["author"] == "shabbywu(shabbywu@qq.com)"\n```\n\n## Copyright and license\n\nCode and documentation copyright 2021 shabbywu(shabbywu@qq.com).   \nCode released under the Apache 2.0 license.\n\n## Reference\n\n- [docker/libtrust](https://github.com/distribution/distribution/tree/main/vendor/github.com/docker/libtrust)\n- [realityone/libtrust-py](https://github.com/realityone/libtrust-py)\n',
-    'author': 'shabbywu',
-    'author_email': 'shabbywu@qq.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/shabbywu/py-libtrust',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.6',
+your_content = {
+    "author": "shabbywu(shabbywu@qq.com)"
 }
 
+# New a JSONSignature
+js = JSONSignature.new(your_content)
+
+# signature
+js.sign(ec_key, dt=datetime.datetime.utcfromtimestamp(0))
+
+pretty_signature = js.to_pretty_signature("signatures")
+loaded_js = js.from_pretty_signature(pretty_signature)
+
+assert js.verify() == loaded_js.verify()
+assert json.loads(pretty_signature)["author"] == "shabbywu(shabbywu@qq.com)"
+```
+
+## Copyright and license
+
+Code and documentation copyright 2021 shabbywu(shabbywu@qq.com).   
+Code released under the Apache 2.0 license.
+
+## Reference
+
+- [docker/libtrust](https://github.com/distribution/distribution/tree/main/vendor/github.com/docker/libtrust)
+- [realityone/libtrust-py](https://github.com/realityone/libtrust-py)
 
-setup(**setup_kwargs)
```

