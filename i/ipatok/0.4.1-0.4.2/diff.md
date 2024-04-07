# Comparing `tmp/ipatok-0.4.1.tar.gz` & `tmp/ipatok-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipatok-0.4.1.tar", last modified: Sun Apr 17 14:02:45 2022, max compression
+gzip compressed data, was "ipatok-0.4.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `ipatok-0.4.1.tar` & `ipatok-0.4.2.tar`

### file list

```diff
@@ -1,19 +1,18 @@
--rw-r--r--   0        0        0      183 2022-04-17 09:55:58.405012 ipatok-0.4.1/.editorconfig
--rw-r--r--   0        0        0      251 2022-04-17 12:09:29.699298 ipatok-0.4.1/.flake8
--rw-r--r--   0        0        0       63 2022-04-17 12:23:33.725601 ipatok-0.4.1/.gitignore
--rw-r--r--   0        0        0      649 2022-04-17 13:52:48.090684 ipatok-0.4.1/CHANGELOG.rst
--rw-r--r--   0        0        0      818 2022-04-17 10:40:44.545960 ipatok-0.4.1/CONTRIBUTING.rst
--rw-r--r--   0        0        0     1072 2022-04-02 21:32:01.976617 ipatok-0.4.1/LICENSE
--rw-r--r--   0        0        0     5791 2022-04-17 13:55:23.278565 ipatok-0.4.1/README.rst
--rw-r--r--   0        0        0      128 2022-04-17 14:01:07.902294 ipatok-0.4.1/ipatok/__init__.py
--rw-r--r--   0        0        0     4543 2022-04-02 21:32:01.976617 ipatok-0.4.1/ipatok/data/ipa_2015.tsv
--rw-r--r--   0        0        0      232 2022-04-02 21:32:01.976617 ipatok-0.4.1/ipatok/data/replacements.tsv
--rw-r--r--   0        0        0     6143 2022-04-02 21:32:01.976617 ipatok-0.4.1/ipatok/ipa.py
--rw-r--r--   0        0        0        0 2022-04-02 21:32:01.976617 ipatok-0.4.1/ipatok/tests/__init__.py
--rw-r--r--   0        0        0     8116 2022-04-02 21:32:01.976617 ipatok-0.4.1/ipatok/tests/test_ipa.py
--rw-r--r--   0        0        0    12189 2022-04-17 13:24:27.683355 ipatok-0.4.1/ipatok/tests/test_tokens.py
--rw-r--r--   0        0        0     7531 2022-04-17 14:00:44.290313 ipatok-0.4.1/ipatok/tokens.py
--rw-r--r--   0        0        0      805 2022-04-17 10:30:44.463611 ipatok-0.4.1/pyproject.toml
--rw-r--r--   0        0        0       76 2022-04-17 10:36:32.910640 ipatok-0.4.1/requirements.in
--rw-r--r--   0        0        0      894 2022-04-17 10:36:41.734616 ipatok-0.4.1/requirements.txt
--rw-r--r--   0        0        0     6482 1970-01-01 00:00:00.000000 ipatok-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0      183 2023-05-20 05:52:57.708245 ipatok-0.4.2/.editorconfig
+-rw-r--r--   0        0        0       63 2023-05-20 05:52:57.708245 ipatok-0.4.2/.gitignore
+-rw-r--r--   0        0        0      809 2024-04-07 13:06:49.924909 ipatok-0.4.2/CHANGELOG.rst
+-rw-r--r--   0        0        0      866 2024-04-01 10:57:36.578478 ipatok-0.4.2/CONTRIBUTING.rst
+-rw-r--r--   0        0        0     1072 2023-05-20 05:52:57.708245 ipatok-0.4.2/LICENSE
+-rw-r--r--   0        0        0     5580 2024-04-07 12:43:36.462573 ipatok-0.4.2/README.rst
+-rw-r--r--   0        0        0      145 2024-04-07 13:07:24.244893 ipatok-0.4.2/ipatok/__init__.py
+-rw-r--r--   0        0        0     4543 2023-05-20 05:52:57.708245 ipatok-0.4.2/ipatok/data/ipa_2015.tsv
+-rw-r--r--   0        0        0      232 2023-05-20 05:52:57.708245 ipatok-0.4.2/ipatok/data/replacements.tsv
+-rw-r--r--   0        0        0     6162 2024-04-01 10:33:27.774234 ipatok-0.4.2/ipatok/ipa.py
+-rw-r--r--   0        0        0        0 2023-05-20 05:52:57.708245 ipatok-0.4.2/ipatok/tests/__init__.py
+-rw-r--r--   0        0        0     8148 2024-04-01 10:39:43.814083 ipatok-0.4.2/ipatok/tests/test_ipa.py
+-rw-r--r--   0        0        0    12200 2024-04-07 12:20:18.309954 ipatok-0.4.2/ipatok/tests/test_tokens.py
+-rw-r--r--   0        0        0     7554 2024-04-01 13:07:29.670065 ipatok-0.4.2/ipatok/tokens.py
+-rw-r--r--   0        0        0      878 2024-04-01 10:25:55.154398 ipatok-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0      100 2024-03-31 14:25:25.537438 ipatok-0.4.2/requirements.in
+-rw-r--r--   0        0        0      844 2024-03-31 14:25:57.007414 ipatok-0.4.2/requirements.txt
+-rw-r--r--   0        0        0     6271 1970-01-01 00:00:00.000000 ipatok-0.4.2/PKG-INFO
```

### Comparing `ipatok-0.4.1/CHANGELOG.rst` & `ipatok-0.4.2/CHANGELOG.rst`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,19 @@
 =========
 changelog
 =========
 
 
+0.4.2 (2024-04-07)
+------------------
+
+- Fixed ``tokenise`` to handle underscores as unknown symbols (`#5
+  <https://github.com/pavelsof/ipatok/issues/5>`_).
+
+
 0.4.1 (2022-04-17)
 ------------------
 
 - Fixed ``clusterise`` to properly forward its keyword arguments to
   ``tokenise`` (`#4 <https://github.com/pavelsof/ipatok/pull/4>`_).
```

### Comparing `ipatok-0.4.1/CONTRIBUTING.rst` & `ipatok-0.4.2/CONTRIBUTING.rst`

 * *Files 14% similar despite different names*

```diff
@@ -23,16 +23,19 @@
     # you can also pip install -r requirements.txt
     pip install pip-tools
     pip-sync
 
     # run the tests
     python -m unittest
 
-    # check for PEP8 issues
-    flake8
+    # run the code linter
+    ruff check
+
+    # run the code formatter
+    ruff format
 
 
 conventions
 ===========
 
 For file encoding, newlines, indentation: please use the ``.editorconfig``
 rules (`take a look here <https://editorconfig.org/>`_ if this is new for you).
```

### Comparing `ipatok-0.4.1/LICENSE` & `ipatok-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ipatok-0.4.1/README.rst` & `ipatok-0.4.2/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -96,34 +96,27 @@
 together symbols separated by these characters, even though the latter are not
 included in the output.
 
 
 installation
 ============
 
-This is a standard Python 3 package without dependencies. It is offered at the
-`Cheese Shop`_, so you can install it with pip::
+This is a Python 3 package without dependencies and it is offered at the
+`Cheese Shop`_::
 
+    # usually within a virtual environment
     pip install ipatok
 
-or, alternatively, you can clone this repo (safe to delete afterwards) and do::
-
-    python setup.py test
-    python setup.py install
-
-Of course, this could be happening within a virtualenv/venv as well.
-
 
 other IPA packages
 ==================
 
 - lingpy_ is a historical linguistics suite that includes an ipa2tokens_
   function.
-- loanpy_ is another historical linguistics suite which uses ``ipatok`` as a
-  dependency.
+- loanpy_ is another historical linguistics suite which works with IPA strings.
 - ipapy_ is a package for working with IPA strings.
 - ipalint_ provides a command-line tool for checking IPA datasets for errors
   and inconsistencies.
 - asjp_ provides functions for converting between IPA and ASJP.
 
 
 licence
```

### Comparing `ipatok-0.4.1/ipatok/data/ipa_2015.tsv` & `ipatok-0.4.2/ipatok/data/ipa_2015.tsv`

 * *Files identical despite different names*

### Comparing `ipatok-0.4.1/ipatok/ipa.py` & `ipatok-0.4.2/ipatok/ipa.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,16 @@
             '# consonants (non-pulmonic)': self.consonants,
             '# other symbols': self.consonants,
             '# tie bars': self.tie_bars,
             '# vowels': self.vowels,
             '# diacritics': self.diacritics,
             '# suprasegmentals': self.suprasegmentals,
             '# lengths': self.lengths,
-            '# tones and word accents': self.tones}
+            '# tones and word accents': self.tones,
+        }
 
         curr_section = None
 
         with open(file_path, encoding='utf-8') as f:
             for line in map(lambda x: x.strip(), f):
                 if line.startswith('#'):
                     if line in sections:
@@ -74,21 +75,23 @@
 
 
 def ensure_single_char(func):
     """
     Decorator that ensures that the first argument of the decorated function is
     a single character, i.e. a string of length one.
     """
+
     @functools.wraps(func)
     def wrapper(*args, **kwargs):
         if not isinstance(args[0], str) or len(args[0]) != 1:
-            raise ValueError((
+            raise ValueError(
                 'This function should be invoked with a string of length one '
                 'as its first argument'
-            ))
+            )
+
         return func(*args, **kwargs)
 
     return wrapper
 
 
 @ensure_single_char
 def is_letter(char, strict=True):
@@ -134,18 +137,20 @@
 
     In strict mode return True only if the diacritic is part of the IPA spec.
     """
     if char in chart.diacritics:
         return True
 
     if not strict:
-        return (unicodedata.category(char) in ['Lm', 'Mn', 'Sk']) \
-                and (not is_suprasegmental(char)) \
-                and (not is_tie_bar(char)) \
-                and (not 0xA700 <= ord(char) <= 0xA71F)
+        return (
+            unicodedata.category(char) in ['Lm', 'Mn', 'Sk']
+            and not is_suprasegmental(char)
+            and not is_tie_bar(char)
+            and not 0xA700 <= ord(char) <= 0xA71F
+        )
 
     return False
 
 
 @ensure_single_char
 def is_suprasegmental(char, strict=True):
     """
@@ -189,17 +194,19 @@
 
 
 def get_precomposed_chars():
     """
     Return the set of IPA characters that are defined in normal form C in the
     spec. As of 2015, this is only the voiceless palatal fricative, ç.
     """
-    return set([
-        letter for letter in chart.consonants
-        if unicodedata.normalize('NFD', letter) != letter])
+    return set(
+        letter
+        for letter in chart.consonants
+        if unicodedata.normalize('NFD', letter) != letter
+    )
 
 
 def replace_substitutes(string):
     """
     Return the given string with all known common substitutes replaced with
     their IPA-compliant counterparts.
     """
```

### Comparing `ipatok-0.4.1/ipatok/tests/test_ipa.py` & `ipatok-0.4.2/ipatok/tests/test_ipa.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,25 @@
 from functools import partial
 from unittest import TestCase
 
 from ipatok.ipa import (
-    is_letter, is_vowel, is_tie_bar, is_diacritic, is_suprasegmental,
-    is_length, is_tone, get_precomposed_chars, replace_substitutes, chart
+    is_letter,
+    is_vowel,
+    is_tie_bar,
+    is_diacritic,
+    is_suprasegmental,
+    is_length,
+    is_tone,
+    get_precomposed_chars,
+    replace_substitutes,
+    chart,
 )
 
 
 class IpaTestCase(TestCase):
-
     def test_is_letter(self):
         """
         is_letter should always return True for IPA letters and False for other
         IPA symbols.
         """
         for strict in [True, False]:
             func = partial(is_letter, strict=strict)
```

### Comparing `ipatok-0.4.1/ipatok/tests/test_tokens.py` & `ipatok-0.4.2/ipatok/tests/test_tokens.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 from functools import partial
 from itertools import product
 from unittest import TestCase
 from unittest.mock import patch
 
 from ipatok.tokens import (
-    normalise, group, are_diphthong, tokenise, clusterise,
-    replace_digits_with_chao
+    normalise,
+    group,
+    are_diphthong,
+    tokenise,
+    clusterise,
+    replace_digits_with_chao,
 )
 
 
 class TokensTestCase(TestCase):
     """
     The IPA strings are sourced from NorthEuraLex (languages: ady, ava, bul,
     ckt, cmn, deu, eng, hun).
@@ -43,30 +47,34 @@
     def test_tokenise(self):
         """
         IPA-compliant strings should be correctly tokenised, regardless of the
         flag values.
         """
         for comb in product(*[[True, False]] * 5):
             func = partial(
-                tokenise, strict=comb[0], replace=comb[1], diphthongs=comb[2],
-                tones=comb[3], unknown=comb[4]
+                tokenise,
+                strict=comb[0],
+                replace=comb[1],
+                diphthongs=comb[2],
+                tones=comb[3],
+                unknown=comb[4],
             )
 
             self.assertEqual(func('miq͡χː'), ['m', 'i', 'q͡χː'])
             self.assertEqual(
                 func('ʃːjeq͡χːʼjer'),
-                ['ʃː', 'j', 'e', 'q͡χːʼ', 'j', 'e', 'r']
+                ['ʃː', 'j', 'e', 'q͡χːʼ', 'j', 'e', 'r'],
             )
             self.assertEqual(func('t͡ɬʼibil'), ['t͡ɬʼ', 'i', 'b', 'i', 'l'])
             self.assertEqual(func('ɬalkʼ'), ['ɬ', 'a', 'l', 'kʼ'])
 
             self.assertEqual(func('lit͡sɛ'), ['l', 'i', 't͡s', 'ɛ'])
             self.assertEqual(
                 func('t͡ʃɛʎust'),
-                ['t͡ʃ', 'ɛ', 'ʎ', 'u', 's', 't']
+                ['t͡ʃ', 'ɛ', 'ʎ', 'u', 's', 't'],
             )
             self.assertEqual(func('dirʲa'), ['d', 'i', 'rʲ', 'a'])
             self.assertEqual(func('ut͡ʃa sɛ'), ['u', 't͡ʃ', 'a', 's', 'ɛ'])
 
             self.assertEqual(func('nɪçt'), ['n', 'ɪ', 'ç', 't'])
 
             self.assertEqual(func('ˈd͡ʒɔɪ'), ['d͡ʒ', 'ɔ', 'ɪ'])
@@ -76,108 +84,109 @@
     def test_tokenise_non_ipa(self):
         """
         Tokenising non-compliant strings should raise ValueError unless strict
         is False, regardless of the other flags' values.
         """
         for comb in product(*[[True, False]] * 4):
             func = partial(
-                tokenise, replace=comb[0], diphthongs=comb[1], tones=comb[2],
-                unknown=comb[3]
+                tokenise,
+                replace=comb[0],
+                diphthongs=comb[1],
+                tones=comb[2],
+                unknown=comb[3],
             )
 
             with self.assertRaises(ValueError):
                 func('ʷəˈʁʷa', strict=True)
 
             self.assertEqual(
                 func('ʷəˈʁʷa', strict=False),
-                ['ʷ', 'ə', 'ʁʷ', 'a']
+                ['ʷ', 'ə', 'ʁʷ', 'a'],
             )
 
             with self.assertRaises(ValueError):
                 func('t͡ɕˀet͡ɕeŋ', strict=True)
 
             self.assertEqual(
                 func('t͡ɕˀet͡ɕeŋ', strict=False),
-                ['t͡ɕˀ', 'e', 't͡ɕ', 'e', 'ŋ']
+                ['t͡ɕˀ', 'e', 't͡ɕ', 'e', 'ŋ'],
             )
 
             with self.assertRaises(ValueError):
                 func('kat͡ɕˀaɹ', strict=True)
 
             self.assertEqual(
                 func('kat͡ɕˀaɹ', strict=False),
-                ['k', 'a', 't͡ɕˀ', 'a', 'ɹ']
+                ['k', 'a', 't͡ɕˀ', 'a', 'ɹ'],
             )
 
     def test_tokenise_replace(self):
         """
         Strings containing common substitutes but otherwise IPA-compliant
         should pass the strictness check only if replace is True.
         """
         for comb in product(*[[True, False]] * 3):
             func = partial(
-                tokenise, strict=True, diphthongs=comb[0], tones=comb[1],
-                unknown=comb[2]
+                tokenise,
+                strict=True,
+                diphthongs=comb[0],
+                tones=comb[1],
+                unknown=comb[2],
             )
 
             with self.assertRaises(ValueError):
                 func('t͡ʃɛɫɔ', replace=False)
 
             self.assertEqual(
                 func('t͡ʃɛɫɔ', replace=True), ['t͡ʃ', 'ɛ', 'l̴', 'ɔ']
             )
 
             with self.assertRaises(ValueError):
                 func('ɫuna', replace=False)
 
-            self.assertEqual(
-                func('ɫuna', replace=True), ['l̴', 'u', 'n', 'a']
-            )
+            self.assertEqual(func('ɫuna', replace=True), ['l̴', 'u', 'n', 'a'])
 
     def test_tokenise_diphthongs(self):
         """
         Diphthongs in IPA-compliant strings should be merged depending on the
         diphthongs flag, regardless of the other flags' values.
         """
         for comb in product(*[[True, False]] * 4):
             func = partial(
-                tokenise, strict=comb[0], replace=comb[1], tones=comb[2],
-                unknown=comb[3]
+                tokenise,
+                strict=comb[0],
+                replace=comb[1],
+                tones=comb[2],
+                unknown=comb[3],
             )
 
             self.assertEqual(
                 func('t͡saɪ̯çən', diphthongs=False),
-                ['t͡s', 'a', 'ɪ̯', 'ç', 'ə', 'n']
+                ['t͡s', 'a', 'ɪ̯', 'ç', 'ə', 'n'],
             )
             self.assertEqual(
                 func('t͡saɪ̯çən', diphthongs=True),
-                ['t͡s', 'aɪ̯', 'ç', 'ə', 'n']
+                ['t͡s', 'aɪ̯', 'ç', 'ə', 'n'],
             )
 
             self.assertEqual(
                 func('hɛɐ̯t͡s', diphthongs=False), ['h', 'ɛ', 'ɐ̯', 't͡s']
             )
-            self.assertEqual(
-                func('hɛɐ̯t͡s', diphthongs=True), ['h', 'ɛɐ̯', 't͡s']
-            )
+            self.assertEqual(func('hɛɐ̯t͡s', diphthongs=True), ['h', 'ɛɐ̯', 't͡s'])
 
-            self.assertEqual(
-                func('moːɐ̯', diphthongs=False), ['m', 'oː', 'ɐ̯']
-            )
-            self.assertEqual(
-                func('moːɐ̯', diphthongs=True), ['m', 'oːɐ̯']
-            )
+            self.assertEqual(func('moːɐ̯', diphthongs=False), ['m', 'oː', 'ɐ̯'])
+            self.assertEqual(func('moːɐ̯', diphthongs=True), ['m', 'oːɐ̯'])
 
             self.assertEqual(
                 func('aɪ̯çhœɐ̯nçən', diphthongs=False),
-                ['a', 'ɪ̯', 'ç', 'h', 'œ', 'ɐ̯', 'n', 'ç', 'ə', 'n']
+                ['a', 'ɪ̯', 'ç', 'h', 'œ', 'ɐ̯', 'n', 'ç', 'ə', 'n'],
             )
             self.assertEqual(
                 func('aɪ̯çhœɐ̯nçən', diphthongs=True),
-                ['aɪ̯', 'ç', 'h', 'œɐ̯', 'n', 'ç', 'ə', 'n']
+                ['aɪ̯', 'ç', 'h', 'œɐ̯', 'n', 'ç', 'ə', 'n'],
             )
 
             self.assertEqual(
                 func('klaʊ̯ə', diphthongs=False), ['k', 'l', 'a', 'ʊ̯', 'ə']
             )
             self.assertEqual(
                 func('klaʊ̯ə', diphthongs=True), ['k', 'l', 'aʊ̯', 'ə']
@@ -186,25 +195,28 @@
     def test_tokenise_tones(self):
         """
         Tones in IPA-compliant strings should be tokenised or ignored depending
         on the tones flag, regardless of other flags' values.
         """
         for comb in product(*[[True, False]] * 4):
             func = partial(
-                tokenise, strict=comb[0], replace=comb[1], diphthongs=comb[2],
-                unknown=comb[3]
+                tokenise,
+                strict=comb[0],
+                replace=comb[1],
+                diphthongs=comb[2],
+                unknown=comb[3],
             )
 
             self.assertEqual(
                 func('t͡sɯ˦ɕy˦', tones=True),
-                ['t͡s', 'ɯ', '˦', 'ɕ', 'y', '˦']
+                ['t͡s', 'ɯ', '˦', 'ɕ', 'y', '˦'],
             )
             self.assertEqual(
                 func('t͡sɯ˦ɕy˦', tones=False),
-                ['t͡s', 'ɯ', 'ɕ', 'y']
+                ['t͡s', 'ɯ', 'ɕ', 'y'],
             )
 
             self.assertEqual(func('˨˩˦', tones=True), ['˨˩˦'])
             self.assertEqual(func('˨˩˦', tones=False), [])
 
             self.assertEqual(func('ə̋ə̏', tones=True), ['ə̋', 'ə̏'])
             self.assertEqual(func('ə̋ə̏', tones=False), ['ə', 'ə'])
@@ -229,51 +241,49 @@
     def test_tokenise_unknown(self):
         """
         Unknown symbols should raise ValueError unless strict is False, in
         which case they should be ignored depending on the unknown flag.
         """
         for comb in product(*[[True, False]] * 3):
             func = partial(
-                tokenise, replace=comb[0], diphthongs=comb[1], tones=comb[2]
+                tokenise,
+                replace=comb[0],
+                diphthongs=comb[1],
+                tones=comb[2],
             )
 
             for unknown in [True, False]:
                 with self.assertRaises(ValueError):
-                    func('-/$', strict=True, unknown=unknown)
+                    func('_-/$', strict=True, unknown=unknown)
 
-            self.assertEqual(func('-/$', unknown=True), ['-', '/', '$'])
-            self.assertEqual(func('-/$', unknown=False), [])
+            self.assertEqual(func('_-/$', unknown=True), ['_', '-', '/', '$'])
+            self.assertEqual(func('_-/$', unknown=False), [])
 
-    def test_tokenise_splits_words(self):
+    def test_tokenise_whitespace(self):
         """
-        Whitespace characters and underscores should serve as word boundaries,
-        regardless of the flag values.
+        Whitespace characters are expected to be used as word boundaries and
+        should be ignored regardless of the flag values.
         """
         for comb in product(*[[True, False]] * 5):
             func = partial(
-                tokenise, strict=comb[0], replace=comb[1], diphthongs=comb[2],
-                tones=comb[3], unknown=comb[4]
+                tokenise,
+                strict=comb[0],
+                replace=comb[1],
+                diphthongs=comb[2],
+                tones=comb[3],
+                unknown=comb[4],
             )
 
             self.assertEqual(
                 func('prɤst na krak'),
-                ['p', 'r', 'ɤ', 's', 't', 'n', 'a', 'k', 'r', 'a', 'k']
-            )
-            self.assertEqual(
-                func('prɤst_na_krak'),
-                ['p', 'r', 'ɤ', 's', 't', 'n', 'a', 'k', 'r', 'a', 'k']
+                ['p', 'r', 'ɤ', 's', 't', 'n', 'a', 'k', 'r', 'a', 'k'],
             )
-
             self.assertEqual(
                 func('etɬə tite'),
-                ['e', 't', 'ɬ', 'ə', 't', 'i', 't', 'e']
-            )
-            self.assertEqual(
-                func('etɬə_tite'),
-                ['e', 't', 'ɬ', 'ə', 't', 'i', 't', 'e']
+                ['e', 't', 'ɬ', 'ə', 't', 'i', 't', 'e'],
             )
 
     def test_replace_digits_with_chao(self):
         """
         Digits should be correctly replaced with Chao tone letters, regardless
         of the flag value and whether superscript or not.
         """
@@ -292,19 +302,19 @@
         )
         self.assertEqual(
             replace_digits_with_chao('ɕiŋ55ɕiŋ2', inverse=True), 'ɕiŋ˩ɕiŋ˦'
         )
 
         self.assertEqual(
             replace_digits_with_chao('ɕia⁵¹ɕyɛ²¹⁴', inverse=True),
-            'ɕia˩˥ɕyɛ˦˥˨'
+            'ɕia˩˥ɕyɛ˦˥˨',
         )
         self.assertEqual(
             replace_digits_with_chao('ɕia51ɕyɛ214', inverse=True),
-            'ɕia˩˥ɕyɛ˦˥˨'
+            'ɕia˩˥ɕyɛ˦˥˨',
         )
 
     def test_clusterise(self):
         self.assertEqual(
             clusterise('kiaːltaːʃ'), ['k', 'iaː', 'lt', 'aː', 'ʃ']
         )
         self.assertEqual(clusterise('sɫɤnt͡sɛ'), ['sɫ', 'ɤ', 'nt͡s', 'ɛ'])
```

### Comparing `ipatok-0.4.1/ipatok/tokens.py` & `ipatok-0.4.2/ipatok/tokens.py`

 * *Files 6% similar despite different names*

```diff
@@ -55,20 +55,21 @@
     Users who want more sophisticated diphthong detection should instead write
     their own function and do something like::
 
         tokenise(string, diphthong=False, merge=user_func)
 
     Helper for tokenise(string, ..).
     """
+
     def is_short(token):
         return '◌̯'[1] in token
 
     subtokens = []
 
-    for char in tokenA+tokenB:
+    for char in tokenA + tokenB:
         if ipa.is_vowel(char):
             subtokens.append(char)
         elif ipa.is_diacritic(char) or ipa.is_length(char):
             if subtokens:
                 subtokens[-1] += char
             else:
                 break
@@ -77,16 +78,17 @@
     else:
         if len([x for x in subtokens if not is_short(x)]) < 2:
             return True
 
     return False
 
 
-def tokenise_word(string,
-                  strict=False, replace=False, tones=False, unknown=False):
+def tokenise_word(
+    string, strict=False, replace=False, tones=False, unknown=False
+):
     """
     Tokenise the string into a list of tokens or raise ValueError if it cannot
     be tokenised (relatively) unambiguously. The string should not include
     whitespace, i.e. it is assumed to be a single word.
 
     If strict=False, allow non-standard letters and diacritics, as well as
     initial diacritic-only tokens (e.g. pre-aspiration). If replace=True,
@@ -101,15 +103,15 @@
     if replace:
         string = ipa.replace_substitutes(string)
 
     tokens = []
 
     for index, char in enumerate(string):
         if ipa.is_letter(char, strict):
-            if tokens and ipa.is_tie_bar(string[index-1]):
+            if tokens and ipa.is_tie_bar(string[index - 1]):
                 tokens[-1] += char
             else:
                 tokens.append(char)
 
         elif ipa.is_tie_bar(char):
             if not tokens:
                 raise ValueError(f'The string starts with a tie bar: {string}')
@@ -150,30 +152,37 @@
                 tokens.append(char)
             else:
                 pass
 
     return tokens
 
 
-def tokenise(string, strict=False, replace=False,
-             diphthongs=False, tones=False, unknown=False, merge=None):
+def tokenise(
+    string,
+    strict=False,
+    replace=False,
+    diphthongs=False,
+    tones=False,
+    unknown=False,
+    merge=None,
+):
     """
     Tokenise an IPA string into a list of tokens. Raise ValueError if there is
     a problem; if strict=True, this includes the string not being compliant to
     the IPA spec.
 
     If replace=True, replace some common non-IPA symbols with their IPA
     counterparts. If diphthongs=True, try to group diphthongs into single
     tokens. If tones=True, do not ignore tone symbols. If unknown=True, do not
     ignore symbols that cannot be classified into a relevant category. If merge
     is not None, use it for within-word token grouping.
 
     Part of ipatok's public API.
     """
-    words = string.strip().replace('_', ' ').split()
+    words = string.strip().split()
     output = []
 
     for word in words:
         tokens = tokenise_word(word, strict, replace, tones, unknown)
 
         if diphthongs:
             tokens = group(are_diphthong, tokens)
@@ -182,24 +191,32 @@
             tokens = group(merge, tokens)
 
         output.extend(tokens)
 
     return output
 
 
-def clusterise(string, strict=False, replace=False,
-               diphthongs=False, tones=False, unknown=False, merge=None):
+def clusterise(
+    string,
+    strict=False,
+    replace=False,
+    diphthongs=False,
+    tones=False,
+    unknown=False,
+    merge=None,
+):
     """
     Tokenise an IPA string and return a list of consonant and vowel clusters.
     Raise ValueError if there is a problem.
 
     Forward the keyword arguments to tokenise.
 
     Part of ipatok's public API.
     """
+
     def groupit(ipalist):
         """Merge subsequent consonants and vowels to clusters."""
         tmp = []
         it = iter(ipalist)
         nextit = next(it)
         for char in ipalist:
             charcv = any(ipa.is_vowel(i) for i in char)
@@ -228,17 +245,19 @@
 
     if inverse:
         chao_letters = chao_letters[::-1]
 
     string = string.translate(str.maketrans('¹²³⁴⁵', '12345'))
     string = string.translate(str.maketrans('12345', chao_letters))
 
-    string = ''.join([
-        char for index, char in enumerate(string)
-        if not (index and char in chao_letters and string[index-1] == char)])
+    string = ''.join(
+        char
+        for index, char in enumerate(string)
+        if not (index and char in chao_letters and string[index - 1] == char)
+    )
 
     return string
 
 
 """
 Provide for the alternative spellings.
 """
```

### Comparing `ipatok-0.4.1/pyproject.toml` & `ipatok-0.4.2/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -26,7 +26,13 @@
 dynamic = ["version"]
 
 [project.urls]
 Home = "https://github.com/pavelsof/ipatok"
 Tracker = "https://github.com/pavelsof/ipatok/issues"
 Source = "https://github.com/pavelsof/ipatok"
 Changelog = "https://github.com/pavelsof/ipatok/blob/master/CHANGELOG.rst"
+
+[tool.ruff]
+line-length = 79
+
+[tool.ruff.format]
+quote-style = "single"
```

### Comparing `ipatok-0.4.1/PKG-INFO` & `ipatok-0.4.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipatok
-Version: 0.4.1
+Version: 0.4.2
 Summary: IPA tokeniser
 Keywords: IPA,tokeniser,tokenizer
 Author-email: pavelsof <mail@pavelsof.com>
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
@@ -113,34 +113,27 @@
 together symbols separated by these characters, even though the latter are not
 included in the output.
 
 
 installation
 ============
 
-This is a standard Python 3 package without dependencies. It is offered at the
-`Cheese Shop`_, so you can install it with pip::
+This is a Python 3 package without dependencies and it is offered at the
+`Cheese Shop`_::
 
+    # usually within a virtual environment
     pip install ipatok
 
-or, alternatively, you can clone this repo (safe to delete afterwards) and do::
-
-    python setup.py test
-    python setup.py install
-
-Of course, this could be happening within a virtualenv/venv as well.
-
 
 other IPA packages
 ==================
 
 - lingpy_ is a historical linguistics suite that includes an ipa2tokens_
   function.
-- loanpy_ is another historical linguistics suite which uses ``ipatok`` as a
-  dependency.
+- loanpy_ is another historical linguistics suite which works with IPA strings.
 - ipapy_ is a package for working with IPA strings.
 - ipalint_ provides a command-line tool for checking IPA datasets for errors
   and inconsistencies.
 - asjp_ provides functions for converting between IPA and ASJP.
 
 
 licence
```

