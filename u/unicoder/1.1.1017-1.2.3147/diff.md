# Comparing `tmp/unicoder-1.1.1017.tar.gz` & `tmp/unicoder-1.2.3147.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/unicoder-1.1.1017.tar", last modified: Sat Jan  8 15:43:46 2022, max compression
+gzip compressed data, was "dist/unicoder-1.2.3147.tar", last modified: Sun Apr  7 20:27:32 2024, max compression
```

## Comparing `unicoder-1.1.1017.tar` & `unicoder-1.2.3147.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 guidod    (1001) root         (0)        0 2022-01-08 15:43:46.000000 unicoder-1.1.1017/
--rw-r--r--   0 guidod    (1001) root         (0)    11351 2022-01-07 19:08:33.000000 unicoder-1.1.1017/LICENSE
--rw-r--r--   0 guidod    (1001) root         (0)     2702 2022-01-08 15:43:46.000000 unicoder-1.1.1017/PKG-INFO
--rw-r--r--   0 guidod    (1001) root         (0)     1870 2022-01-08 15:43:46.000000 unicoder-1.1.1017/README
--rw-r--r--   0 guidod    (1001) root         (0)     2497 2022-01-08 15:26:33.000000 unicoder-1.1.1017/README.md
--rw-r--r--   0 guidod    (1001) root         (0)     1116 2022-01-08 15:43:46.000000 unicoder-1.1.1017/setup.cfg
--rwxr-xr-x   0 guidod    (1001) root         (0)       60 2022-01-08 15:43:46.000000 unicoder-1.1.1017/setup.py
-drwxr-xr-x   0 guidod    (1001) root         (0)        0 2022-01-08 15:43:46.000000 unicoder-1.1.1017/unicoder.egg-info/
--rw-r--r--   0 guidod    (1001) root         (0)     2702 2022-01-08 15:43:46.000000 unicoder-1.1.1017/unicoder.egg-info/PKG-INFO
--rw-r--r--   0 guidod    (1001) root         (0)      204 2022-01-08 15:43:46.000000 unicoder-1.1.1017/unicoder.egg-info/SOURCES.txt
--rw-r--r--   0 guidod    (1001) root         (0)        1 2022-01-08 15:43:46.000000 unicoder-1.1.1017/unicoder.egg-info/dependency_links.txt
--rw-r--r--   0 guidod    (1001) root         (0)        1 2022-01-08 15:43:46.000000 unicoder-1.1.1017/unicoder.egg-info/top_level.txt
--rwxr-xr-x   0 guidod    (1001) root         (0)    30811 2022-01-08 15:43:37.000000 unicoder-1.1.1017/unicoder.py
--rwxr-xr-x   0 guidod    (1001) root         (0)    61276 2022-01-08 04:03:41.000000 unicoder-1.1.1017/unicoder.py.tests.py
+drwxr-xr-x   0 guidod    (1001) root         (0)        0 2024-04-07 20:27:32.000000 unicoder-1.2.3147/
+-rw-r--r--   0 guidod    (1001) root         (0)    11351 2022-01-07 19:08:33.000000 unicoder-1.2.3147/LICENSE
+-rw-r--r--   0 guidod    (1001) root         (0)     3106 2024-04-07 20:27:32.000000 unicoder-1.2.3147/PKG-INFO
+-rw-r--r--   0 guidod    (1001) root         (0)     2168 2024-04-07 20:27:31.000000 unicoder-1.2.3147/README
+-rw-r--r--   0 guidod    (1001) root         (0)     2956 2024-04-07 20:03:09.000000 unicoder-1.2.3147/README.md
+-rw-r--r--   0 guidod    (1001) root         (0)     1118 2024-04-07 20:27:32.000000 unicoder-1.2.3147/setup.cfg
+-rwxr-xr-x   0 guidod    (1001) root         (0)       60 2024-04-07 20:27:31.000000 unicoder-1.2.3147/setup.py
+drwxr-xr-x   0 guidod    (1001) root         (0)        0 2024-04-07 20:27:32.000000 unicoder-1.2.3147/unicoder.egg-info/
+-rw-r--r--   0 guidod    (1001) root         (0)     3106 2024-04-07 20:27:32.000000 unicoder-1.2.3147/unicoder.egg-info/PKG-INFO
+-rw-r--r--   0 guidod    (1001) root         (0)      204 2024-04-07 20:27:32.000000 unicoder-1.2.3147/unicoder.egg-info/SOURCES.txt
+-rw-r--r--   0 guidod    (1001) root         (0)        1 2024-04-07 20:27:32.000000 unicoder-1.2.3147/unicoder.egg-info/dependency_links.txt
+-rw-r--r--   0 guidod    (1001) root         (0)        1 2024-04-07 20:27:32.000000 unicoder-1.2.3147/unicoder.egg-info/top_level.txt
+-rwxr-xr-x   0 guidod    (1001) root         (0)    45156 2024-04-07 19:57:25.000000 unicoder-1.2.3147/unicoder.py
+-rwxr-xr-x   0 guidod    (1001) root         (0)    85812 2024-04-07 20:25:31.000000 unicoder-1.2.3147/unicoder.py.tests.py
```

### Comparing `unicoder-1.1.1017/LICENSE` & `unicoder-1.2.3147/LICENSE`

 * *Files identical despite different names*

### Comparing `unicoder-1.1.1017/PKG-INFO` & `unicoder-1.2.3147/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: unicoder
-Version: 1.1.1017
-Summary: allows to convert ascii to unicode specials including bold italic greek fraktur script
+Version: 1.2.3147
+Summary: unicode text generator to make bold italic greek fraktur cursive script from ascii input
 Home-page: https://github.com/gdraheim/unicoder
 Author: Guido U. Draheim
 Author-email: Guido.Draheim@gmx.de
 License: APL
 Description: 
         This script allows to convert ascii to unicode specials 
         including bold italic greek fraktur script.
@@ -24,17 +24,24 @@
             unicoder.py fraktur foobar
             unicoder.py boldfraktur foobar
             unicoder.py fract 15 1/4
             unicoder.py 15 1/4 km/h
             unicoder.py value 15 1/4 km/h
             unicoder.py thin 15 1/4 km/h
             unicoder.py nobr 15 1/4 km/h
+            unicoder.py power 15^3
+            unicoder.py index x_1
+            unicoder.py math X_1^3 +1/4
+            unicoder.py back answer
+            unicoder.py down answer
+            unicoder.py flip answer
         
         This script helps to bold or slanted text to various social media platforms.
         The nobr thin fract parts are particularly useful for Wikipedia.
+        The flip or turn allows to provide a pun on a text.
         
         ### RESULT
         
         Just for amusement, this is the result when running the commands shown above. 
         Note that the bold and italic text snippets do not rely on \<i\> \<b\> \<font\> hints
         or some similar style markup, instead they use different codepoints from the 
         [Mathematical Alphanumeric Symbols](https://en.wikipedia.org/wiki/Mathematical_Alphanumeric_Symbols)
@@ -52,21 +59,27 @@
             𝔣𝔬𝔬𝔟𝔞𝔯
             𝖋𝖔𝖔𝖇𝖆𝖗
             15¼
             15¼ km/h
             15¼ km/h
             15 1/4 km/h
             15 1/4 km/h
+            15³
+            x₁
+            Ξ₁³ +¼
+            rewsna
+            ɐusʍǝɹ
+            ɹǝʍsuɐ
         
         ### TESTSUITE
         
         Yes, there is a testsuite with more than a hundred unittests for the functions.
         The module can also be imported as helper to other scripts.
         
-        For developers, please use "make tests" for the testsuite and do run also
-        the "make type" for mypy typehints checks and "make pep" for pep8 style checks.
+        For developers, please run "make tests" for the testsuite. Please do also
+        run "make type" for mypy typehints checks and "make pep" for pep8 style checks.
         
         
         
         
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `unicoder-1.1.1017/README` & `unicoder-1.2.3147/README`

 * *Files 16% similar despite different names*

```diff
@@ -16,17 +16,24 @@
     unicoder.py fraktur foobar
     unicoder.py boldfraktur foobar
     unicoder.py fract 15 1/4
     unicoder.py 15 1/4 km/h
     unicoder.py value 15 1/4 km/h
     unicoder.py thin 15 1/4 km/h
     unicoder.py nobr 15 1/4 km/h
+    unicoder.py power 15^3
+    unicoder.py index x_1
+    unicoder.py math X_1^3 +1/4
+    unicoder.py back answer
+    unicoder.py down answer
+    unicoder.py flip answer
 
 This script helps to bold or slanted text to various social media platforms.
 The nobr thin fract parts are particularly useful for Wikipedia.
+The flip or turn allows to provide a pun on a text.
 
 ### RESULT
 
 Just for amusement, this is the result when running the commands shown above. 
 Note that the bold and italic text snippets do not rely on \<i\> \<b\> \<font\> hints
 or some similar style markup, instead they use different codepoints from the 
 [Mathematical Alphanumeric Symbols](https://en.wikipedia.org/wiki/Mathematical_Alphanumeric_Symbols)
@@ -44,18 +51,24 @@
     𝔣𝔬𝔬𝔟𝔞𝔯
     𝖋𝖔𝖔𝖇𝖆𝖗
     15¼
     15¼ km/h
     15¼ km/h
     15 1/4 km/h
     15 1/4 km/h
+    15³
+    x₁
+    Ξ₁³ +¼
+    rewsna
+    ɐusʍǝɹ
+    ɹǝʍsuɐ
 
 ### TESTSUITE
 
 Yes, there is a testsuite with more than a hundred unittests for the functions.
 The module can also be imported as helper to other scripts.
 
-For developers, please use "make tests" for the testsuite and do run also
-the "make type" for mypy typehints checks and "make pep" for pep8 style checks.
+For developers, please run "make tests" for the testsuite. Please do also
+run "make type" for mypy typehints checks and "make pep" for pep8 style checks.
```

### Comparing `unicoder-1.1.1017/README.md` & `unicoder-1.2.3147/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 [![Style Check](https://github.com/gdraheim/unicoder/actions/workflows/stylecheck.yml/badge.svg?event=push)](https://github.com/gdraheim/unicoder/actions/workflows/stylecheck.yml)
 [![Type Check](https://github.com/gdraheim/unicoder/actions/workflows/typecheck.yml/badge.svg?event=push)](https://github.com/gdraheim/unicoder/actions/workflows/typecheck.yml)
 [![Unit Tests](https://github.com/gdraheim/unicoder/actions/workflows/unittests.yml/badge.svg?event=push)](https://github.com/gdraheim/unicoder/actions/workflows/unittests.yml)
+[![Code Coverage](https://img.shields.io/badge/311%20test-100%25%20coverage-brightgreen)](https://github.com/gdraheim/unicoder/blob/master/unicoder.py.tests.py)
 [![PyPI version](https://badge.fury.io/py/unicoder.svg)](https://pypi.org/project/unicoder/)
 
 This script allows to convert ascii to unicode specials 
 including bold italic greek fraktur script.
 
 
 Examples:
@@ -20,17 +21,24 @@
     unicoder.py fraktur foobar
     unicoder.py boldfraktur foobar
     unicoder.py fract 15 1/4
     unicoder.py 15 1/4 km/h
     unicoder.py value 15 1/4 km/h
     unicoder.py thin 15 1/4 km/h
     unicoder.py nobr 15 1/4 km/h
+    unicoder.py power 15^3
+    unicoder.py index x_1
+    unicoder.py math X_1^3 +1/4
+    unicoder.py back answer
+    unicoder.py down answer
+    unicoder.py flip answer
 
 This script helps to bold or slanted text to various social media platforms.
 The nobr thin fract parts are particularly useful for Wikipedia.
+The flip or turn allows to provide a pun on a text.
 
 ### RESULT
 
 Just for amusement, this is the result when running the commands shown above. 
 Note that the bold and italic text snippets do not rely on \<i\> \<b\> \<font\> hints
 or some similar style markup, instead they use different codepoints from the 
 [Mathematical Alphanumeric Symbols](https://en.wikipedia.org/wiki/Mathematical_Alphanumeric_Symbols)
@@ -48,18 +56,24 @@
     𝔣𝔬𝔬𝔟𝔞𝔯
     𝖋𝖔𝖔𝖇𝖆𝖗
     15¼
     15¼ km/h
     15¼ km/h
     15 1/4 km/h
     15 1/4 km/h
+    15³
+    x₁
+    Ξ₁³ +¼
+    rewsna
+    ɐusʍǝɹ
+    ɹǝʍsuɐ
 
 ### TESTSUITE
 
 Yes, there is a testsuite with more than a hundred unittests for the functions.
 The module can also be imported as helper to other scripts.
 
-For developers, please use "make tests" for the testsuite and do run also
-the "make type" for mypy typehints checks and "make pep" for pep8 style checks.
+For developers, please run "make tests" for the testsuite. Please do also
+run "make type" for mypy typehints checks and "make pep" for pep8 style checks.
```

### Comparing `unicoder-1.1.1017/setup.cfg` & `unicoder-1.2.3147/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [metadata]
 name = unicoder
-version = 1.1.1017
+version = 1.2.3147
 license = APL
 license_files = 
 	LICENSE
 author = Guido U. Draheim
 author-email = Guido.Draheim@gmx.de
 home-page = https://github.com/gdraheim/unicoder
-description = allows to convert ascii to unicode specials including bold italic greek fraktur script
+description = unicode text generator to make bold italic greek fraktur cursive script from ascii input
 long-description = file: README
 long-description-content-type = text/markdown
 requires-dist = setuptools
 
 [options]
 include_package_data = True
 scripts =
```

### Comparing `unicoder-1.1.1017/unicoder.egg-info/PKG-INFO` & `unicoder-1.2.3147/unicoder.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: unicoder
-Version: 1.1.1017
-Summary: allows to convert ascii to unicode specials including bold italic greek fraktur script
+Version: 1.2.3147
+Summary: unicode text generator to make bold italic greek fraktur cursive script from ascii input
 Home-page: https://github.com/gdraheim/unicoder
 Author: Guido U. Draheim
 Author-email: Guido.Draheim@gmx.de
 License: APL
 Description: 
         This script allows to convert ascii to unicode specials 
         including bold italic greek fraktur script.
@@ -24,17 +24,24 @@
             unicoder.py fraktur foobar
             unicoder.py boldfraktur foobar
             unicoder.py fract 15 1/4
             unicoder.py 15 1/4 km/h
             unicoder.py value 15 1/4 km/h
             unicoder.py thin 15 1/4 km/h
             unicoder.py nobr 15 1/4 km/h
+            unicoder.py power 15^3
+            unicoder.py index x_1
+            unicoder.py math X_1^3 +1/4
+            unicoder.py back answer
+            unicoder.py down answer
+            unicoder.py flip answer
         
         This script helps to bold or slanted text to various social media platforms.
         The nobr thin fract parts are particularly useful for Wikipedia.
+        The flip or turn allows to provide a pun on a text.
         
         ### RESULT
         
         Just for amusement, this is the result when running the commands shown above. 
         Note that the bold and italic text snippets do not rely on \<i\> \<b\> \<font\> hints
         or some similar style markup, instead they use different codepoints from the 
         [Mathematical Alphanumeric Symbols](https://en.wikipedia.org/wiki/Mathematical_Alphanumeric_Symbols)
@@ -52,21 +59,27 @@
             𝔣𝔬𝔬𝔟𝔞𝔯
             𝖋𝖔𝖔𝖇𝖆𝖗
             15¼
             15¼ km/h
             15¼ km/h
             15 1/4 km/h
             15 1/4 km/h
+            15³
+            x₁
+            Ξ₁³ +¼
+            rewsna
+            ɐusʍǝɹ
+            ɹǝʍsuɐ
         
         ### TESTSUITE
         
         Yes, there is a testsuite with more than a hundred unittests for the functions.
         The module can also be imported as helper to other scripts.
         
-        For developers, please use "make tests" for the testsuite and do run also
-        the "make type" for mypy typehints checks and "make pep" for pep8 style checks.
+        For developers, please run "make tests" for the testsuite. Please do also
+        run "make type" for mypy typehints checks and "make pep" for pep8 style checks.
         
         
         
         
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `unicoder-1.1.1017/unicoder.py` & `unicoder-1.2.3147/unicoder.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #! /usr/bin/python3
 from __future__ import print_function
 
-__copyright__ = "(C) 2021-2022 Guido U. Draheim, licensed under the APLv2"
-__version__ = "1.1.1017"
+__copyright__ = "(C) 2021-2024 Guido U. Draheim, licensed under the APLv2"
+__version__ = "1.2.3147"
 
 from typing import List, Dict, Generator, Tuple
 from io import StringIO
 import sys
 import logging
 
 logg = logging.getLogger("UNICODER")
@@ -67,18 +67,18 @@
     norm_fraktur_Y = 0x1D51C
     norm_fraktur_a = 0x1D51E
     norm_fraktur_z = 0x1D537
     bold_fraktur_A = 0x1D56C
     bold_fraktur_Z = 0x1D585
     bold_fraktur_a = 0x1D586
     bold_fraktur_z = 0x1D59F
-    ital_fraktur_A = 0x1D56C
-    ital_fraktur_Z = 0x1D585
-    ital_fraktur_a = 0x1D586
-    ital_fraktur_z = 0x1D59F
+    # ital_fraktur_A = 0x1D56C
+    # ital_fraktur_Z = 0x1D585
+    # ital_fraktur_a = 0x1D586
+    # ital_fraktur_z = 0x1D59F
     # bold_ital_fraktur_A = n/a
     # bold_ital_fraktur_Z = n/a
     # bold_ital_fraktur_a = n/a
     # bold_ital_fraktur_z = n/a
     #
     norm_script_A = 0x1D49C
     norm_script_Z = 0x1D4B5
@@ -97,20 +97,68 @@
     norm_double_9 = 0x1D7E1
     norm_mono_A = 0x1D670
     norm_mono_Z = 0x1D689
     norm_mono_a = 0x1D68A
     norm_mono_z = 0x1D6A3
     norm_mono_0 = 0x1D7F6
     norm_mono_9 = 0x1D7FF
+    norm_parens_A = 0x1F110   # PARENTHESIZED CAPITAL
+    norm_parens_O = 0x1F11E   # PARENTHESIZED CAPITAL
+    norm_parens_Z = 0x1F129   # PARENTHESIZED CAPITAL
+    norm_parens_a = 0x249C    # PARENTHESIZED SMALL
+    norm_parens_o = 0x24AA    # PARENTHESIZED SMALL
+    norm_parens_z = 0x24B5    # PARENTHESIZED SMALL
+    norm_parens_1 = 0x2472    # PARENTHESIZED DIGIT
+    norm_parens_9 = 0x247A    # PARENTHESIZED DIGIT
+    norm_parens_20 = 0x2485   # PARENTHESIZED DIGIT
+    #
+    norm_circled_A = 0x24B6  # CIRCLED DIGIT
+    norm_circled_O = 0x24C4  # CIRCLED DIGIT
+    norm_circled_Z = 0x24CF  # CIRCLED DIGIT
+    norm_circled_a = 0x24D0  # CIRCLED DIGIT
+    norm_circled_z = 0x24E9  # CIRCLED DIGIT
+    norm_circled_0 = 0x24EA  # CIRCLED DIGIT
+    norm_circled_1 = 0x245E  # CIRCLED DIGIT
+    norm_circled_9 = 0x2466  # CIRCLED DIGIT
+    norm_circled_20 = 0x2471  # CIRCLED DIGIT
+    norm_circled_sans_1 = 0x2780    # NEGATIVE CIRCLED SANS-SERIF DIGIT (dingbats)
+    norm_circled_sans_9 = 0x2788    # NEGATIVE CIRCLED SANS-SERIF DIGIT (dingbats)
+    norm_circled_sans_10 = 0x2789   # NEGATIVE CIRCLED SANS-SERIF DIGIT (dingbats)
+    #
+    norm_button_A = 0x1F150  # NEGATIVE CIRCLED CAPITAL
+    norm_button_O = 0x1F15E  # NEGATIVE CIRCLED CAPITAL
+    norm_button_Z = 0x1F169  # NEGATIVE CIRCLED CAPITAL
+    norm_button_1 = 0x2774   # NEGATIVE CIRCLED DIGIT (dingbats)
+    norm_button_9 = 0x277E   # NEGATIVE CIRCLED DIGIT (dingbats)
+    norm_button_10 = 0x277F   # NEGATIVE CIRCLED DIGIT (dingbats)
+    norm_button_11 = 0x24EB   # NEGATIVE CIRCLED DIGIT
+    norm_button_20 = 0x24F4   # NEGATIVE CIRCLED DIGIT
+    norm_button_0 = 0x24FF   # NEGATIVE CIRCLED DIGIT
+    norm_button_sans_1 = 0x278A   # NEGATIVE CIRCLED SANS-SERIF DIGIT (dingbats)
+    norm_button_sans_9 = 0x2792   # NEGATIVE CIRCLED SANS-SERIF DIGIT (dingbats)
+    norm_button_sans_10 = 0x2793   # NEGATIVE CIRCLED SANS-SERIF DIGIT (dingbats)
+    norm_signum_A = 0x1F170  # NEGATIVE SQUARED CAPITAL
+    norm_signum_O = 0x1F17E  # NEGATIVE SQUARED CAPITAL
+    norm_signum_Z = 0x1F189  # NEGATIVE SQUARED CAPITAL
+    #
+    norm_dbutton_1 = 0x24F5   # DOUBLE CIRCLED DIGIT (dingbats)
+    norm_dbutton_9 = 0x24FE   # DOUBLE CIRCLED DIGIT (dingbats)
+    norm_squared_A = 0x1F130  # SQUARED CAPITAL
+    norm_squared_O = 0x1F13E  # SQUARED CAPITAL
+    norm_squared_Z = 0x1F149  # SQUARED CAPITAL
+    norm_dice_1 = 0x2680
+    norm_dice_6 = 0x2685
+    norm_regional_A = 0x1F1E6  # REGIONAL INDICATOR 
+    norm_regional_Z = 0x1F1FF  # REGIONAL INDICATOR 
     #
     norm_greek_A = 0x391
     norm_greek_O = 0x3A9
     norm_greek_a = 0x3B1
     norm_greek_o = 0x3C9
-    norm_greek_nabla = 0x8711
+    norm_greek_nabla = 0x2207
     norm_greek_diffs = 0x2202
     bold_greek_A = 0x1D6A8
     bold_greek_O = 0x1D6C0
     bold_greek_nabla = 0x1D6C1
     bold_greek_a = 0x1D6C2
     bold_greek_o = 0x1D6DA
     bold_greek_diffs = 0x1D6DB
@@ -147,14 +195,111 @@
     norm_frac_7_8 = 0x215E
     norm_frac_1_x = 0x215F
     norm_frac_0_3 = 0x2189
     norm_base_space = 0x20
     norm_nobr_space = 0x00A0
     norm_thin_space = 0x202F
     norm_numm_space = 0x2007
+    #
+    norm_super_0 = 0x2070
+    norm_super_1 = 0x00B9
+    norm_super_2 = 0x00B2
+    norm_super_3 = 0x00B3
+    norm_super_4 = 0x2074
+    norm_super_5 = 0x2075
+    norm_super_6 = 0x2076
+    norm_super_7 = 0x2077
+    norm_super_8 = 0x2078
+    norm_super_9 = 0x2079
+    norm_super_plus = 0x207A
+    norm_super_minus = 0x207B
+    norm_super_leftparen = 0x207D
+    norm_super_rightparen = 0x0207E
+    norm_super_equals = 0x207C
+    norm_super_n = 0x207F
+    norm_sub_0 = 0x2080
+    norm_sub_1 = 0x2081
+    norm_sub_2 = 0x2082
+    norm_sub_3 = 0x2083
+    norm_sub_4 = 0x2084
+    norm_sub_5 = 0x2085
+    norm_sub_6 = 0x2086
+    norm_sub_7 = 0x2087
+    norm_sub_8 = 0x2088
+    norm_sub_9 = 0x2089
+    norm_sub_plus = 0x208A
+    norm_sub_minus = 0x208B
+    norm_sub_equals = 0x208C
+    norm_sub_leftparen = 0x208D
+    norm_sub_rightparen = 0x0208E
+    norm_sub_a =  0x2090
+    norm_sub_e =  0x2091
+    norm_sub_o =  0x2092
+    norm_sub_x =  0x2093
+    norm_sub_i =  0x1D62
+    norm_sub_r =  0x1D63
+    norm_sub_u =  0x1D64
+    norm_sub_v =  0x1D65
+    #
+    norm_turned_a = 0x0250
+    norm_turned_b = ord('q')
+    norm_turned_c = 0x0254
+    norm_turned_d = ord('p')
+    norm_turned_e = 0x01DD
+    norm_turned_f = 0x025F
+    norm_turned_g = 0x1D77 # 0x0183
+    norm_turned_h = 0x0265
+    norm_turned_i = 0x1D09 # 0x0131
+    norm_turned_j = 0x027E
+    norm_turned_k = 0x029E
+    norm_turned_l = ord('l')
+    norm_turned_m = 0x026F
+    norm_turned_n = ord('u')
+    norm_turned_o = ord('o')
+    norm_turned_p = ord('d')
+    norm_turned_q = ord('b')
+    norm_turned_r = 0x0279
+    norm_turned_s = ord('s')
+    norm_turned_t = 0x0287
+    norm_turned_u = ord('n')
+    norm_turned_v = 0x028C
+    norm_turned_w = 0x028D
+    norm_turned_x = ord('x')
+    norm_turned_y = 0x028E
+    norm_turned_z = ord('z')
+    norm_turned_amp = 0x214B
+    norm_turned_dot = 0x02D9
+    norm_turned_comma = 0x02BB
+    norm_turned_bang = 0x00A1
+    norm_turned_question = 0x00BF
+    norm_turned_A = 0x2200 # 0x2C6F
+    norm_turned_C = 0x0186
+    norm_turned_E = 0x018E
+    norm_turned_F = 0x2132
+    norm_turned_G = 0x2141 # 0x05E4
+    norm_turned_J = 0x017F
+    norm_turned_M = 0x019C
+    norm_turned_L = 0x2142
+    norm_turned_R = 0x1D1A
+    norm_turned_T = 0xA7B1 # 0x2534
+    norm_turned_U = 0x2229
+    norm_turned_V = 0x039B
+    norm_turned_W = ord('M')
+    norm_turned_Y = 0x2144
+    norm_turned_1 = 0x21C2
+    norm_turned_3 = 0x0190
+    norm_turned_6 = ord('9')
+    norm_turned_9 = ord('6')
+    norm_turned_ue = 0x1E49 # n with under line
+    norm_turned_UE = 0x1E4B # n with under hacek
+    norm_turned_AE = 0x1E7E # V with ring under
+    norm_turned_OE = 0x1ECC # O with dot under
+    norm_turned_ae = 0x1D02 # ae turned
+    norm_turned_oe = 0x1ECD # o with dot under # 0x1D14 # oe turned
+    norm_turned_sz = 0x00FE # thorn # 0x025B # open e # 0x0D93 # open e with retroflex
 
 def nobrspace(text: str) -> str:
     """replace base space by thin nobreak space """
     out = StringIO()
     last_ch = 0
     for c in text:
         ch = ord(c)
@@ -266,14 +411,141 @@
                 out.write(space + item[:-1])
                 space = item[-1]
             else:
                 out.write(space + item)
                 space = ""
     return out.getvalue()
 
+norm_super_numbers: Dict[str, int] = {
+    "0": norm_super_0,
+    "1": norm_super_1,
+    "2": norm_super_2,
+    "3": norm_super_3,
+    "4": norm_super_4,
+    "5": norm_super_5,
+    "6": norm_super_6,
+    "7": norm_super_7,
+    "8": norm_super_8,
+    "9": norm_super_9,
+    "+": norm_super_plus,
+    "-": norm_super_minus,
+}
+
+norm_super_before: Dict[str, int] = {
+    "=": norm_super_equals,
+    "(": norm_super_leftparen,
+}
+norm_super_after: Dict[str, int] = {
+    ")": norm_super_rightparen,
+    "n": norm_super_n,
+}
+
+def superscript(text: str) -> str:
+    out = StringIO()
+    for x, c in enumerate(text):
+        if c in norm_super_numbers:
+            out.write(chr(norm_super_numbers[c]))
+        elif c in norm_super_after and x > 0 and text[x-1] in norm_super_numbers:
+            out.write(chr(norm_super_after[c]))
+        elif c in norm_super_before and x+1 < len(text) and text[x+1] in norm_super_numbers:
+            out.write(chr(norm_super_before[c]))
+        else:
+            out.write(c)
+    return out.getvalue()
+
+norm_power_signs = "^"
+def power(text: str) -> str:
+    out = StringIO()
+    power = False
+    for x, c in enumerate(text):
+        if c in norm_power_signs and x+1 < len(text) and (text[x+1] in norm_super_numbers or text[x+1] in norm_super_before):
+            power = True
+            continue # drop the power sign
+        if power:
+            if c in norm_super_numbers:
+                out.write(chr(norm_super_numbers[c]))
+            elif c in norm_super_before:
+                out.write(chr(norm_super_before[c]))
+            elif c in norm_super_after:
+                out.write(chr(norm_super_after[c]))
+            else:
+                power = False
+                out.write(c)
+        else:
+            out.write(c)
+    return out.getvalue()
+
+norm_sub_numbers: Dict[str, int] = {
+    "0": norm_sub_0,
+    "1": norm_sub_1,
+    "2": norm_sub_2,
+    "3": norm_sub_3,
+    "4": norm_sub_4,
+    "5": norm_sub_5,
+    "6": norm_sub_6,
+    "7": norm_sub_7,
+    "8": norm_sub_8,
+    "9": norm_sub_9,
+    "+": norm_sub_plus,
+    "-": norm_sub_minus,
+}
+
+norm_sub_before: Dict[str, int] = {
+    "=": norm_sub_equals,
+    "(": norm_sub_leftparen,
+}
+norm_sub_after: Dict[str, int] = {
+    ")": norm_sub_rightparen,
+    "a": norm_sub_a,
+    "e": norm_sub_e,
+    "i": norm_sub_i,
+    "o": norm_sub_o,
+    "u": norm_sub_u,
+    "v": norm_sub_v,
+    "x": norm_sub_x,
+    "r": norm_sub_r,
+}
+
+def subscript(text: str) -> str:
+    out = StringIO()
+    for x, c in enumerate(text):
+        if c in norm_sub_numbers:
+            out.write(chr(norm_sub_numbers[c]))
+        elif c in norm_sub_after and x > 0 and text[x-1] in norm_sub_numbers:
+            out.write(chr(norm_sub_after[c]))
+        elif c in norm_sub_before and x+1 < len(text) and text[x+1] in norm_sub_numbers:
+            out.write(chr(norm_sub_before[c]))
+        else:
+            out.write(c)
+    return out.getvalue()
+
+norm_indexed_signs = "_"
+def indexed(text: str) -> str:
+    out = StringIO()
+    indexed = False
+    for x, c in enumerate(text):
+        if c in norm_indexed_signs and x+1 < len(text) and (text[x+1] in norm_sub_numbers or text[x+1] in norm_sub_before):
+            indexed = True
+            continue # drop the indexed sign
+        if indexed:
+            if c in norm_sub_numbers:
+                out.write(chr(norm_sub_numbers[c]))
+            elif c in norm_sub_before:
+                out.write(chr(norm_sub_before[c]))
+            elif c in norm_sub_after:
+                out.write(chr(norm_sub_after[c]))
+            else:
+                indexed = False
+                out.write(c)
+        else:
+            out.write(c)
+    return out.getvalue()
+
+
+
 norm_greek_upper: Dict[str, Tuple[int, ...]] = {
     "A": (0x391,),  # Alpha
     "B": (0x392,),  # Beta
     "G": (0x393,),  # Gamma
     "D": (0x394,),  # Delta
     "E": (0x395,),  # Epsilon
     "Z": (0x396,),  # Zeta
@@ -300,15 +572,15 @@
     "W": (0x3A8,),  # Psi
     "U": (0x3A9,),  # Omega
     "OO": (0x3A9,),  # Omega
     #
     "J": (0x399,),  # Iota
     "Q": (0x39A,),  # Kappa
     "QU": (0x39A,),  # Kappa
-    "V": (0x2207,),  # Nabla Operatur
+    "V": (norm_greek_nabla,),  # Nabla Operator
 }
 
 norm_greek_lower: Dict[str, Tuple[int, ...]] = {
     "a": (0x3B1,),  # Alpha
     "b": (0x3B2,),  # Beta
     "g": (0x3B3,),  # Gamma
     "d": (0x3B4,),  # Delta
@@ -336,15 +608,15 @@
     "w": (0x3C8,),  # Psi
     "u": (0x3C9,),  # Omega
     "oo": (0x3C9,),  # Omega
     #
     "j": (0x3B9,),  # Iota
     "q": (0x3BA,),  # Kappa
     "qu": (0x3BA,),  # Kappa
-    "v": (0x2202,),  # Differential
+    "v": (norm_greek_diffs,),  # Differential
 }
 
 def greek(text: str) -> str:
     def as_norm(text: str) -> str:
         return text
     def as_ital(text: str) -> str:
         return ital(text)
@@ -393,15 +665,15 @@
             d = text[i + 1]
         else:
             d = " "
         # orig_d = d
         dh = ord(d)
         if ital_base_A <= dh and dh <= ital_base_Z:
             d = chr(norm_base_A + (dh - ital_base_A))
-        if ch in ital_base_lower:
+        if dh in ital_base_lower:
             d = chr(ital_base_lower[dh])
         if ital_base_a <= dh and dh <= ital_base_z:
             d = chr(norm_base_a + (dh - ital_base_a))
         if bold_base_A <= dh and dh <= bold_base_Z:
             d = chr(norm_base_A + (dh - bold_base_A))
         if bold_base_a <= dh and dh <= bold_base_z:
             d = chr(norm_base_a + (dh - bold_base_a))
@@ -499,14 +771,15 @@
                     out.write(chr(n))
                 skip = True
             elif c in norm_rune_lower:
                 for n in norm_rune_lower[c]:
                     out.write(chr(n))
             else:
                 logg.error("did not find rune for '%s'", c)
+                out.write(c)
         else:
             out.write(c)
     return out.getvalue()
 
 norm_fraktur__C = 0x212D  # Complex Numbers
 norm_fraktur__H = 0x210C  # Hamilton Numbers
 norm_fraktur__I = 0x2111
@@ -537,14 +810,92 @@
             out.write(chr(norm_fraktur_a + (ch - norm_base_a)))
         # elif norm_base_0 <= ch and ch <= norm_base_9:
         #     out.write(chr(bold_base_0+(ch-norm_base_0)))
         else:
             out.write(c)
     return out.getvalue()
 
+norm_turned_encode: Dict[str, int] = {
+    'a': norm_turned_a,
+    'b': norm_turned_b,
+    'c': norm_turned_c,
+    'd': norm_turned_d,
+    'e': norm_turned_e,
+    'f': norm_turned_f,
+    'g': norm_turned_g,
+    'h': norm_turned_h,
+    'i': norm_turned_i,
+    'j': norm_turned_j,
+    'k': norm_turned_k,
+    'l': norm_turned_l,
+    'm': norm_turned_m,
+    'n': norm_turned_n,
+    'p': norm_turned_p,
+    'q': norm_turned_q,
+    'r': norm_turned_r,
+    't': norm_turned_t,
+    'u': norm_turned_u,
+    'v': norm_turned_v,
+    'w': norm_turned_w,
+    'y': norm_turned_y,
+    '&': norm_turned_amp,
+    ',': norm_turned_comma,
+    '.': norm_turned_dot,
+    '!': norm_turned_bang,
+    '?': norm_turned_question,
+    'A': norm_turned_A,
+    'C': norm_turned_C,
+    'E': norm_turned_E,
+    'F': norm_turned_F,
+    'G': norm_turned_G,
+    'J': norm_turned_J,
+    'L': norm_turned_L,
+    'M': norm_turned_M,
+    'P': ord('d'),
+    'R': norm_turned_R,
+    'T': norm_turned_T,
+    'U': norm_turned_U,
+    'V': norm_turned_V,
+    'W': norm_turned_W,
+    'Y': norm_turned_Y,
+    chr(0xE4): norm_turned_ae,
+    chr(0xF6): norm_turned_oe,
+    chr(0xFC): norm_turned_ue,
+    chr(0xC4): norm_turned_AE,
+    chr(0xD6): norm_turned_OE,
+    chr(0xDC): norm_turned_UE,
+    chr(0xDF): norm_turned_sz,
+    }
+
+def turned(text: str) -> str:  # characters flipped upside down
+    out = StringIO()
+    for c in text:
+        ch = ord(c)
+        if c in norm_turned_encode:
+            out.write(chr(norm_turned_encode[c]))
+        else:
+            out.write(c)
+    return out.getvalue()
+
+def backlines(text: str) -> str:  # lines right-left inversed
+    out = StringIO()
+    line = StringIO()
+    for c in text:
+        if c in '\r\n\f':
+            out.write(line.getvalue()[::-1])
+            out.write(c)
+            line = StringIO()
+        else:
+            line.write(c)
+    out.write(line.getvalue()[::-1])
+    return out.getvalue()
+
+def turnlines(text: str) -> str:
+    return turned(backlines(text))
+
 norm_script__B = 0x212C
 norm_script__E = 0x2130
 norm_script__F = 0x2131
 norm_script__H = 0x210B
 norm_script__I = 0x2110
 norm_script__L = 0x2112
 norm_script__M = 0x2133
@@ -616,15 +967,15 @@
     norm_double__H: ord('H'),
     norm_double__N: ord('N'),
     norm_double__P: ord('P'),
     norm_double__Q: ord('Q'),
     norm_double__R: ord('R'),
     norm_double__Z: ord('Z')}
 
-def double(text: str) -> str:  # gothic, blackletter
+def doubled(text: str) -> str:  # gothic, blackletter
     out = StringIO()
     for c in text:
         ch = ord(c)
         if c in norm_double_encode:
             out.write(chr(norm_double_encode[c]))
         elif norm_base_A <= ch and ch <= norm_base_Z:
             out.write(chr(norm_double_A + (ch - norm_base_A)))
@@ -632,35 +983,90 @@
             out.write(chr(norm_double_a + (ch - norm_base_a)))
         elif norm_base_0 <= ch and ch <= norm_base_9:
             out.write(chr(norm_double_0 + (ch - norm_base_0)))
         else:
             out.write(c)
     return out.getvalue()
 
+def button(text: str) -> str:  # squred
+    # only ABO for bloodgroup are common, digit 0 is different than 9
+    out = StringIO()
+    for c in text:
+        ch = ord(c)
+        if norm_base_A <= ch and ch <= norm_base_Z:
+            out.write(chr(norm_signum_A + (ch - norm_base_A)))
+        elif norm_base_a <= ch and ch <= norm_base_z:
+            out.write(chr(norm_button_A + (ch - norm_base_a)))
+        elif norm_base_0+1 <= ch and ch <= norm_base_9:
+            out.write(chr(norm_button_1 + (ch - norm_base_0+1)))
+        elif norm_base_0 == ch and ch:
+            out.write(chr(norm_button_0))
+        else:
+            out.write(c)
+    return out.getvalue()
+
+def circled(text: str) -> str:  # squred
+    # most fonts have that inconsistent - found M to be blue
+    out = StringIO()
+    for c in text:
+        ch = ord(c)
+        if norm_base_A <= ch and ch <= norm_base_Z:
+            out.write(chr(norm_circled_A + (ch - norm_base_A)))
+        elif norm_base_a <= ch and ch <= norm_base_z:
+            out.write(chr(norm_circled_a + (ch - norm_base_a)))
+        elif norm_base_0+1 <= ch and ch <= norm_base_9:
+            out.write(chr(norm_circled_1 + (ch - norm_base_0+1)))
+        elif norm_base_0 == ch and ch:
+            out.write(chr(norm_circled_0))
+        else:
+            out.write(c)
+    return out.getvalue()
+
+def parens(text: str) -> str:  # squred
+    # most fonts have that incomplete - only lowercase and digts are common
+    out = StringIO()
+    for c in text:
+        ch = ord(c)
+        if norm_base_A <= ch and ch <= norm_base_Z:
+            out.write(chr(norm_parens_A + (ch - norm_base_A)))
+        elif norm_base_a <= ch and ch <= norm_base_z:
+            out.write(chr(norm_parens_a + (ch - norm_base_a)))
+        elif norm_base_0+1 <= ch and ch <= norm_base_9:
+            out.write(chr(norm_parens_1 + (ch - norm_base_0+1)))
+        elif norm_base_0 == ch and ch:
+            out.write(chr(norm_parens_o))
+        else:
+            out.write(c)
+    return out.getvalue()
+
 def courier(text: str) -> str:  # gothic, blackletter
     out = StringIO()
     for c in text:
         ch = ord(c)
         if norm_base_A <= ch and ch <= norm_base_Z:
             out.write(chr(norm_mono_A + (ch - norm_base_A)))
         elif norm_base_a <= ch and ch <= norm_base_z:
             out.write(chr(norm_mono_a + (ch - norm_base_a)))
         elif norm_base_0 <= ch and ch <= norm_base_9:
             out.write(chr(norm_mono_0 + (ch - norm_base_0)))
         else:
             out.write(c)
     return out.getvalue()
 
-def uppercasedouble(text: str) -> str:  # gothic, blackletter
+def initial(text: str) -> str:
     out = StringIO()
+    newline = True
     for c in text:
         ch = ord(c)
-        if norm_base_A <= ch and ch <= norm_base_Z:
-            out.write(chr(norm_double_A + (ch - norm_base_A)))
+        if newline and norm_base_A <= ch and ch <= norm_base_Z:
+            out.write(doubled(c))
+            newline = False
         else:
+            if c in "\r\n":
+                newline = True
             out.write(c)
     return out.getvalue()
 
 def sans(text: str) -> str:
     out = StringIO()
     for c in text:
         ch = ord(c)
@@ -717,26 +1123,22 @@
             out.write(chr(ital_sans_A + (ch - norm_sans_A)))
         elif norm_sans_a <= ch and ch <= norm_sans_z:
             out.write(chr(ital_sans_a + (ch - norm_sans_a)))
         elif bold_sans_A <= ch and ch <= bold_sans_Z:
             out.write(chr(bold_ital_sans_A + (ch - bold_sans_A)))
         elif bold_sans_a <= ch and ch <= bold_sans_z:
             out.write(chr(bold_ital_sans_a + (ch - bold_sans_a)))
-        elif norm_fraktur_A <= ch and ch <= norm_fraktur_Y:
-            out.write(chr(ital_fraktur_A + (ch - norm_fraktur_A)))
-        elif norm_fraktur_a <= ch and ch <= norm_fraktur_z:
-            out.write(chr(ital_fraktur_a + (ch - norm_fraktur_a)))
-        elif norm_greek_A <= ch and ch <= norm_greek_O:
-            out.write(chr(ital_greek_A + (ch - norm_greek_A)))
-        elif norm_greek_a <= ch and ch <= norm_greek_o:
-            out.write(chr(ital_greek_a + (ch - norm_greek_a)))
         elif norm_greek_nabla == ch:
             out.write(chr(ital_greek_nabla))
         elif norm_greek_diffs == ch:
             out.write(chr(ital_greek_diffs))
+        elif norm_greek_A <= ch and ch <= norm_greek_O:
+            out.write(chr(ital_greek_A + (ch - norm_greek_A)))
+        elif norm_greek_a <= ch and ch <= norm_greek_o:
+            out.write(chr(ital_greek_a + (ch - norm_greek_a)))
         elif bold_greek_A <= ch and ch <= bold_greek_O + 1:
             out.write(chr(bold_ital_greek_A + (ch - bold_greek_A)))
         elif bold_greek_a <= ch and ch <= bold_greek_o + 1:
             out.write(chr(bold_ital_greek_a + (ch - bold_greek_a)))
         else:
             out.write(c)
     return out.getvalue()
@@ -780,22 +1182,22 @@
             out.write(chr(bold_script_A + (norm_script_upper[ch] - norm_base_A)))
         elif ch in norm_script_lower:
             out.write(chr(bold_script_a + (norm_script_lower[ch] - norm_base_a)))
         elif norm_script_A <= ch and ch <= norm_script_Z:
             out.write(chr(bold_script_A + (ch - norm_script_A)))
         elif norm_script_a <= ch and ch <= norm_script_z:
             out.write(chr(bold_script_a + (ch - norm_script_a)))
-        elif norm_greek_A <= ch and ch <= norm_greek_O:
-            out.write(chr(bold_greek_A + (ch - norm_greek_A)))
-        elif norm_greek_a <= ch and ch <= norm_greek_o:
-            out.write(chr(bold_greek_a + (ch - norm_greek_a)))
         elif norm_greek_nabla == ch:
             out.write(chr(bold_greek_nabla))
         elif norm_greek_diffs == ch:
             out.write(chr(bold_greek_diffs))
+        elif norm_greek_A <= ch and ch <= norm_greek_O:
+            out.write(chr(bold_greek_A + (ch - norm_greek_A)))
+        elif norm_greek_a <= ch and ch <= norm_greek_o:
+            out.write(chr(bold_greek_a + (ch - norm_greek_a)))
         elif ital_greek_A <= ch and ch <= ital_greek_O + 1:
             out.write(chr(bold_ital_greek_A + (ch - ital_greek_A)))
         elif ital_greek_a <= ch and ch <= ital_greek_o + 1:
             out.write(chr(bold_ital_greek_a + (ch - ital_greek_a)))
         else:
             out.write(c)
     return out.getvalue()
@@ -841,20 +1243,45 @@
         text = cmd + " " + text
         cmd = "value"
     logg.debug("cmd = '%s'", cmd)
     if "nobr" in cmd or "word" in cmd:
         text = nobrspace(text)
     if "thin" in cmd or "value" in cmd:
         text = thinspace(text)
+    if "button" in cmd or "button" in cmd:
+        text = button(text)
+    if "circ" in cmd or "circled" in cmd:
+        text = circled(text)
+    if "parens" in cmd or "parent" in cmd:
+        text = parens(text)
     if "frac" in cmd or "value" in cmd:
         text = fractions(text)
+    if "subi" in cmd or "below" in cmd:
+        text = subscript(text)
+    if "super" in cmd or "above" in cmd:
+        text = superscript(text)
+    if "power" in cmd or "dim" in cmd:
+        text = power(text)
+    if "index" in cmd or "idx" in cmd:
+        text = indexed(text)
+    if "math" in cmd:
+        text = indexed(power(fractions(nobrspace(text))))
     if "doub" in cmd or "wide" in cmd:
-        text = double(text)
+        text = doubled(text)
     if "caps" in cmd or "init" in cmd:
-        text = uppercasedouble(text)
+        text = initial(text)
+    if "turned" in cmd or "down" in cmd:
+        text = turned(text)
+    if "flip" in cmd or "ambi" in cmd or "turnlines" in cmd:
+        text = turnlines(text) # turned(backlines(text))
+    if "back" in cmd or "swap" in cmd:
+        text = backlines(text)
+    if "turn" in cmd and "turned" not in cmd and "turnlines" not in cmd:
+        logg.warning("use 'flip' to turnlines")
+        text = turned(backlines(text))
     if "rune" in cmd or "futark" in cmd:
         text = rune(text)
     if "greek" in cmd or "math" in cmd:
         text = greek(text)
     if "black" in cmd or "frak" in cmd:
         text = fraktur(text)
     if "round" in cmd or "script" in cmd or "writ" in cmd:
@@ -878,30 +1305,38 @@
      *fat*  *bold*    convert to math fat symbols
      *ital* *name*    convert to math slanted symbols
      *round* *script* convert to math writing symbols
      *greek* *math*   convert to math greek
      *frak* *black*   convert to math fraktur 
      *doub* *wide*    convert to math double stroke
      *cour* *type*    convert to math courier monospace
-     *caps* *init*    uppercase chars to double stroke
+     *rune* *futark*  transliterate to runic script
+     *caps* *init*    initial uppercase char to double stroke
      *nobr* *word*    using base nobr spaces
      *thin* *value*   using thin nobr spaces
      *fract* *vect*   convert fractional values
-     *rune* *futark*  transliterate to runic script
+     *subi* *below*   convert numbers to subscript (and +/-)
+     *super* *above*  convert numbers to superscript (and +/-)
+     *power* *dim*    convert numbers after ^ to superscript
+     *index* *idx*    convert numbers after _ to subscript
+     *math*           nobr+frac+power+index
+     *turned* *down*  turn each character (upside-down)
+     *swap* *back*    reverse each line
+     *flip* *ambi*    turned (upside-down and reversed)
     some combinations provide different codepoints:
       italboldbase
       italgreek
       boldgreek
       italboldgreek
       italsans
       boldsans
       italboldsans
       boldfrak
     """
 
-if __name__ == "__main__":
+if __name__ == "__main__":  # pragma: no cover
     __opt = scan(sys.argv[1:])
     logging.basicConfig(level=max(0, logging.WARNING - __opt.verbose * 10))
     if __opt.helpinfo:
         print(helpinfo())
     else:
         print(convert(__opt.cmd, __opt.text))
```

### Comparing `unicoder-1.1.1017/unicoder.py.tests.py` & `unicoder-1.2.3147/unicoder.py.tests.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,19 @@
 """ testing the unicoder.py functions """
 
 import sys, os
 import unittest
 import logging
 from fnmatch import fnmatchcase as fnmatch
 
-import unicoder
+try:
+    from . import unicoder # mypy
+except ImportError:
+    sys.path.insert(0, ".")
+    import unicoder # type: ignore[no-redef]
 
 logg = logging.getLogger("TEST")
 
 base_abcdefghijklmnopqrstuvwxyz = ":abcdefghijklmnopqrstuvwxyz"
 base_ABCDEFGHIJKLMNOPQRSTUVWXYZ = ":ABCDEFGHIJKLMNOPQRSTUVWXYZ"
 mono_abcdefghijklmnopqrstuvwxyz = ":𝚊𝚋𝚌𝚍𝚎𝚏𝚐𝚑𝚒𝚓𝚔𝚕𝚖𝚗𝚘𝚙𝚚𝚛𝚜𝚝𝚞𝚟𝚠𝚡𝚢𝚣"
 mono_ABCDEFGHIJKLMNOPQRSTUVWXYZ = ":𝙰𝙱𝙲𝙳𝙴𝙵𝙶𝙷𝙸𝙹𝙺𝙻𝙼𝙽𝙾𝙿𝚀𝚁𝚂𝚃𝚄𝚅𝚆𝚇𝚈𝚉"
@@ -36,14 +40,73 @@
         self.assertEqual(opt.verbose, 1)
     def test_002_opt_scan(self) -> None:
         opt = unicoder.scan(["-vv"])
         self.assertEqual(opt.verbose, 2)
     def test_003_opt_scan(self) -> None:
         opt = unicoder.scan(["-v", "-vv"])
         self.assertEqual(opt.verbose, 3)
+    def test_005_opt_scan(self) -> None:
+        opt = unicoder.scan(["--verbose"])
+        self.assertEqual(opt.verbose, 1)
+    def test_006_opt_scan(self) -> None:
+        opt = unicoder.scan(["--verbose", "--verbose"])
+        self.assertEqual(opt.verbose, 2)
+    def test_007_opt_scan(self) -> None:
+        opt = unicoder.scan(["--verbose", "--verbose", "-vv"])
+        self.assertEqual(opt.verbose, 4)
+    def test_008_opt_scan(self) -> None:
+        opt = unicoder.scan(["--verbose", "-vv", "--verbose"])
+        self.assertEqual(opt.verbose, 4)
+    def test_009_opt_scan(self) -> None:
+        opt = unicoder.scan(["-vv", "--verbose", "--verbose"])
+        self.assertEqual(opt.verbose, 4)
+    def test_011_opt_scan(self) -> None:
+        opt = unicoder.scan(["-h"])
+        self.assertEqual(opt.helpinfo, 1)
+    def test_012_opt_scan(self) -> None:
+        opt = unicoder.scan(["-hh"])
+        self.assertEqual(opt.helpinfo, 2)
+    def test_013_opt_scan(self) -> None:
+        opt = unicoder.scan(["-hh", "--help"])
+        self.assertEqual(opt.helpinfo, 3)
+    def test_014_opt_scan(self) -> None:
+        opt = unicoder.scan(["-hh", "--help", "arg1"])
+        self.assertEqual(opt.helpinfo, 3)
+        self.assertEqual(opt.cmd, "arg1")
+        self.assertEqual(opt.text, "")
+    def test_015_opt_scan(self) -> None:
+        opt = unicoder.scan(["-hh", "--help", "arg1", "arg2"])
+        self.assertEqual(opt.helpinfo, 3)
+        self.assertEqual(opt.cmd, "arg1")
+        self.assertEqual(opt.text, "arg2")
+    def test_016_opt_scan(self) -> None:
+        opt = unicoder.scan(["-hh", "--help", "arg1", "arg2", "--arg3"])
+        self.assertEqual(opt.helpinfo, 3)
+        self.assertEqual(opt.cmd, "arg1")
+        self.assertEqual(opt.text, "arg2 --arg3")
+    def test_017_opt_scan(self) -> None:
+        opt = unicoder.scan(["-hh", "--help", "arg1", "--arg2", "arg3"])
+        self.assertEqual(opt.helpinfo, 3)
+        self.assertEqual(opt.cmd, "arg1")
+        self.assertEqual(opt.text, "--arg2 arg3")
+    def test_018_opt_scan(self) -> None:
+        opt = unicoder.scan(["-hh", "--help", "--arg1", "arg2", "arg3"])
+        self.assertEqual(opt.helpinfo, 3)
+        self.assertEqual(opt.cmd, "arg2")
+        self.assertEqual(opt.text, "arg3")
+    def test_019_opt_scan(self) -> None:
+        opt = unicoder.scan(["-hh", "--help", "-&", "arg2", "arg3"])
+        self.assertEqual(opt.helpinfo, 3)
+        self.assertEqual(opt.cmd, "arg2")
+        self.assertEqual(opt.text, "arg3")
+    def test_051_helpinfo(self) -> None:
+        text = unicoder.helpinfo()
+        self.assertIn("futark", text)
+        self.assertIn("italboldgreek", text)
+    #
     def test_110_bold_base(self) -> None:
         uni = unicoder.convert("fix", base_abcdefghijklmnopqrstuvwxyz)
         self.assertEqual(uni, base_abcdefghijklmnopqrstuvwxyz)
     def test_111_bold_base(self) -> None:
         uni = unicoder.convert("fat", base_abcdefghijklmnopqrstuvwxyz)
         self.assertEqual(uni, ":𝐚𝐛𝐜𝐝𝐞𝐟𝐠𝐡𝐢𝐣𝐤𝐥𝐦𝐧𝐨𝐩𝐪𝐫𝐬𝐭𝐮𝐯𝐰𝐱𝐲𝐳")
     def test_112_bold_base(self) -> None:
@@ -211,54 +274,54 @@
         self.assertEqual(uni, ":𝔸𝔹ℂ𝔻𝔼𝔽𝔾ℍ𝕀𝕁𝕂𝕃𝕄ℕ𝕆ℙℚℝ𝕊𝕋𝕌𝕍𝕎𝕏𝕐ℤ")
     def test_204_norm_double(self) -> None:
         uni = unicoder.convert("wide", ":AB-DEFG-IJKLM-O---STUVWXY-")
         self.assertEqual(uni, ":𝔸𝔹-𝔻𝔼𝔽𝔾-𝕀𝕁𝕂𝕃𝕄-𝕆---𝕊𝕋𝕌𝕍𝕎𝕏𝕐-")
         uni = unicoder.convert("wide", base_ABCDEFGHIJKLMNOPQRSTUVWXYZ)
         self.assertEqual(uni, ":𝔸𝔹ℂ𝔻𝔼𝔽𝔾ℍ𝕀𝕁𝕂𝕃𝕄ℕ𝕆ℙℚℝ𝕊𝕋𝕌𝕍𝕎𝕏𝕐ℤ")
     def test_205_norm_double(self) -> None:
-        uni = unicoder.double(base_abcdefghijklmnopqrstuvwxyz)
+        uni = unicoder.doubled(base_abcdefghijklmnopqrstuvwxyz)
         self.assertEqual(uni, ":𝕒𝕓𝕔𝕕𝕖𝕗𝕘𝕙𝕚𝕛𝕜𝕝𝕞𝕟𝕠𝕡𝕢𝕣𝕤𝕥𝕦𝕧𝕨𝕩𝕪𝕫")
     def test_206_norm_double(self) -> None:
-        uni = unicoder.double(base_abcdefghijklmnopqrstuvwxyz)
+        uni = unicoder.doubled(base_abcdefghijklmnopqrstuvwxyz)
         self.assertEqual(uni, ":𝕒𝕓𝕔𝕕𝕖𝕗𝕘𝕙𝕚𝕛𝕜𝕝𝕞𝕟𝕠𝕡𝕢𝕣𝕤𝕥𝕦𝕧𝕨𝕩𝕪𝕫")
     def test_207_norm_double(self) -> None:
-        uni = unicoder.double(base_ABCDEFGHIJKLMNOPQRSTUVWXYZ)
+        uni = unicoder.doubled(base_ABCDEFGHIJKLMNOPQRSTUVWXYZ)
         self.assertEqual(uni, ":𝔸𝔹ℂ𝔻𝔼𝔽𝔾ℍ𝕀𝕁𝕂𝕃𝕄ℕ𝕆ℙℚℝ𝕊𝕋𝕌𝕍𝕎𝕏𝕐ℤ")
     def test_208_norm_double(self) -> None:
-        uni = unicoder.double(base_ABCDEFGHIJKLMNOPQRSTUVWXYZ)
+        uni = unicoder.doubled(base_ABCDEFGHIJKLMNOPQRSTUVWXYZ)
         self.assertEqual(uni, ":𝔸𝔹ℂ𝔻𝔼𝔽𝔾ℍ𝕀𝕁𝕂𝕃𝕄ℕ𝕆ℙℚℝ𝕊𝕋𝕌𝕍𝕎𝕏𝕐ℤ")
     def test_210_bold_double(self) -> None:
         uni = unicoder.convert("fix", ":abcxyzABXY")
         self.assertEqual(uni, ":abcxyzABXY")
     def test_211_bold_double(self) -> None:
         uni = unicoder.convert("fatdouble", ":abcxyzABXY")
         self.assertEqual(uni, ":𝕒𝕓𝕔𝕩𝕪𝕫𝔸𝔹𝕏𝕐")
     def test_212_bold_double(self) -> None:
         uni = unicoder.convert("boldwide", ":abcxyzABXY")
         self.assertEqual(uni, ":𝕒𝕓𝕔𝕩𝕪𝕫𝔸𝔹𝕏𝕐")
     def test_215_bold_double(self) -> None:
-        uni = unicoder.bold(unicoder.double(":abcxyzABXY"))
+        uni = unicoder.bold(unicoder.doubled(":abcxyzABXY"))
         self.assertEqual(uni, ":𝕒𝕓𝕔𝕩𝕪𝕫𝔸𝔹𝕏𝕐")
     def test_216_bold_double(self) -> None:
-        uni = unicoder.bold(unicoder.double(":abcxyzABXY"))
+        uni = unicoder.bold(unicoder.doubled(":abcxyzABXY"))
         self.assertEqual(uni, ":𝕒𝕓𝕔𝕩𝕪𝕫𝔸𝔹𝕏𝕐")
     def test_240_numm_double(self) -> None:
         uni = unicoder.convert("fix", base_0123456789)
         self.assertEqual(uni, base_0123456789)
     def test_241_numm_double(self) -> None:
         uni = unicoder.convert("double", base_0123456789)
         self.assertEqual(uni, ":𝟘𝟙𝟚𝟛𝟜𝟝𝟞𝟟𝟠𝟡")
     def test_242_numm_double(self) -> None:
         uni = unicoder.convert("wide", base_0123456789)
         self.assertEqual(uni, ":𝟘𝟙𝟚𝟛𝟜𝟝𝟞𝟟𝟠𝟡")
     def test_245_numm_double(self) -> None:
-        uni = unicoder.double(base_0123456789)
+        uni = unicoder.doubled(base_0123456789)
         self.assertEqual(uni, ":𝟘𝟙𝟚𝟛𝟜𝟝𝟞𝟟𝟠𝟡")
     def test_246_numm_double(self) -> None:
-        uni = unicoder.double(base_0123456789)
+        uni = unicoder.doubled(base_0123456789)
         self.assertEqual(uni, ":𝟘𝟙𝟚𝟛𝟜𝟝𝟞𝟟𝟠𝟡")
     #
     def test_250_norm_script(self) -> None:
         uni = unicoder.convert("fix", ":abcxyzABCXYZ")
         self.assertEqual(uni, ":abcxyzABCXYZ")
     def test_251_norm_script(self) -> None:
         uni = unicoder.convert("script", ":abcd-f-hijklmn-pqrstuvwxyz")
@@ -385,14 +448,120 @@
         self.assertEqual(uni, mono_0123456789)
     def test_345_numm_courier(self) -> None:
         uni = unicoder.courier(base_0123456789)
         self.assertEqual(uni, mono_0123456789)
     def test_346_numm_courier(self) -> None:
         uni = unicoder.courier(base_0123456789)
         self.assertEqual(uni, mono_0123456789)
+    def test_350_norm_initial(self) -> None:
+        uni = unicoder.convert("init", "Hello world")
+        self.assertEqual(uni, "ℍello world")
+    def test_351_norm_initial(self) -> None:
+        uni = unicoder.convert("caps", "Hello world")
+        self.assertEqual(uni, "ℍello world")
+    def test_352_norm_initial(self) -> None:
+        uni = unicoder.convert("init", "say Hello world")
+        self.assertEqual(uni, "say ℍello world")
+    def test_353_norm_initial(self) -> None:
+        uni = unicoder.convert("caps", "say Hello world")
+        self.assertEqual(uni, "say ℍello world")
+    def test_354_norm_initial(self) -> None:
+        uni = unicoder.convert("init", "Say Hello world")
+        self.assertEqual(uni, "𝕊ay Hello world")
+    def test_355_norm_initial(self) -> None:
+        uni = unicoder.convert("caps", "Say Hello world")
+        self.assertEqual(uni, "𝕊ay Hello world")
+    def test_360_norm_initial(self) -> None:
+        uni = unicoder.initial("Hello world")
+        self.assertEqual(uni, "ℍello world")
+    def test_361_norm_initial(self) -> None:
+        uni = unicoder.initial("say Hello world")
+        self.assertEqual(uni, "say ℍello world")
+    def test_362_norm_initial(self) -> None:
+        uni = unicoder.initial("Say Hello world")
+        self.assertEqual(uni, "𝕊ay Hello world")
+    def test_363_norm_initial(self) -> None:
+        uni = unicoder.initial("Say Hello world.\nYes, I will do.")
+        self.assertEqual(uni, "𝕊ay Hello world.\n𝕐es, I will do.")
+
+
+
+    def test_370_norm_back(self) -> None:
+        uni = unicoder.convert("back", ":abcxyzABXY\nmnoPQ")
+        self.assertEqual(uni, "YXBAzyxcba:\nQPonm")
+    def test_371_norm_back(self) -> None:
+        uni = unicoder.convert("swap", ":abcxyzABXY\nmnoPQ")
+        self.assertEqual(uni, "YXBAzyxcba:\nQPonm")
+    def test_372_norm_back(self) -> None:
+        uni = unicoder.convert("back", base_ABCDEFGHIJKLMNOPQRSTUVWXYZ)
+        self.assertEqual(uni, "ZYXWVUTSRQPONMLKJIHGFEDCBA:")
+    def test_373_norm_back(self) -> None:
+        uni = unicoder.convert("swap", base_ABCDEFGHIJKLMNOPQRSTUVWXYZ)
+        self.assertEqual(uni, "ZYXWVUTSRQPONMLKJIHGFEDCBA:")
+    def test_374_norm_back(self) -> None:
+        uni = unicoder.convert("back", base_abcdefghijklmnopqrstuvwxyz)
+        self.assertEqual(uni, "zyxwvutsrqponmlkjihgfedcba:")
+    def test_375_norm_back(self) -> None:
+        uni = unicoder.convert("swap", base_abcdefghijklmnopqrstuvwxyz)
+        self.assertEqual(uni, "zyxwvutsrqponmlkjihgfedcba:")
+    def test_376_norm_back(self) -> None:
+        uni = unicoder.backlines(base_ABCDEFGHIJKLMNOPQRSTUVWXYZ)
+        self.assertEqual(uni, "ZYXWVUTSRQPONMLKJIHGFEDCBA:")
+    def test_377_norm_back(self) -> None:
+        uni = unicoder.backlines(base_abcdefghijklmnopqrstuvwxyz)
+        self.assertEqual(uni, "zyxwvutsrqponmlkjihgfedcba:")
+    def test_380_norm_turned(self) -> None:
+        uni = unicoder.convert("turned", ":abcxyzABXY\nmnoPQ")
+        self.assertEqual(uni, ":ɐqɔxʎz∀BX⅄\nɯuodQ")
+    def test_381_norm_turned(self) -> None:
+        uni = unicoder.convert("down", ":abcxyzABXY\nmnoPQ")
+        self.assertEqual(uni, ":ɐqɔxʎz∀BX⅄\nɯuodQ")
+    def test_382_norm_turned(self) -> None:
+        uni = unicoder.convert("turned", base_ABCDEFGHIJKLMNOPQRSTUVWXYZ)
+        self.assertEqual(uni, ":∀BƆDƎℲ⅁HIſK⅂ƜNOdQᴚSꞱ∩ΛMX⅄Z")
+    def test_383_norm_turned(self) -> None:
+        uni = unicoder.convert("down", base_ABCDEFGHIJKLMNOPQRSTUVWXYZ)
+        self.assertEqual(uni, ":∀BƆDƎℲ⅁HIſK⅂ƜNOdQᴚSꞱ∩ΛMX⅄Z")
+    def test_384_norm_turned(self) -> None:
+        uni = unicoder.convert("turned", base_abcdefghijklmnopqrstuvwxyz)
+        self.assertEqual(uni, ":ɐqɔpǝɟᵷɥᴉɾʞlɯuodbɹsʇnʌʍxʎz")
+    def test_385_norm_turned(self) -> None:
+        uni = unicoder.convert("down", base_abcdefghijklmnopqrstuvwxyz)
+        self.assertEqual(uni, ":ɐqɔpǝɟᵷɥᴉɾʞlɯuodbɹsʇnʌʍxʎz")
+    def test_386_norm_turned(self) -> None:
+        uni = unicoder.turned(base_ABCDEFGHIJKLMNOPQRSTUVWXYZ)
+        self.assertEqual(uni, ":∀BƆDƎℲ⅁HIſK⅂ƜNOdQᴚSꞱ∩ΛMX⅄Z")
+    def test_387_norm_turned(self) -> None:
+        uni = unicoder.turned(base_abcdefghijklmnopqrstuvwxyz)
+        self.assertEqual(uni, ":ɐqɔpǝɟᵷɥᴉɾʞlɯuodbɹsʇnʌʍxʎz")
+    def test_390_norm_flip(self) -> None:
+        uni = unicoder.convert("flip", ":abcxyzABXY\nmnoPQ")
+        self.assertEqual(uni, "⅄XB∀zʎxɔqɐ:\nQdouɯ")
+    def test_391_norm_flip(self) -> None:
+        uni = unicoder.convert("ambi", ":abcxyzABXY\nmnoPQ")
+        self.assertEqual(uni, "⅄XB∀zʎxɔqɐ:\nQdouɯ")
+    def test_392_norm_flip(self) -> None:
+        uni = unicoder.convert("flip", base_ABCDEFGHIJKLMNOPQRSTUVWXYZ)
+        self.assertEqual(uni, "Z⅄XMΛ∩ꞱSᴚQdONƜ⅂KſIH⅁ℲƎDƆB∀:")
+    def test_393_norm_flip(self) -> None:
+        uni = unicoder.convert("ambi", base_ABCDEFGHIJKLMNOPQRSTUVWXYZ)
+        self.assertEqual(uni, "Z⅄XMΛ∩ꞱSᴚQdONƜ⅂KſIH⅁ℲƎDƆB∀:")
+    def test_394_norm_flip(self) -> None:
+        uni = unicoder.convert("flip", base_abcdefghijklmnopqrstuvwxyz)
+        self.assertEqual(uni, "zʎxʍʌnʇsɹbdouɯlʞɾᴉɥᵷɟǝpɔqɐ:")
+    def test_395_norm_flip(self) -> None:
+        uni = unicoder.convert("ambi", base_abcdefghijklmnopqrstuvwxyz)
+        self.assertEqual(uni, "zʎxʍʌnʇsɹbdouɯlʞɾᴉɥᵷɟǝpɔqɐ:")
+    def test_396_norm_flip(self) -> None:
+        uni = unicoder.turnlines(base_ABCDEFGHIJKLMNOPQRSTUVWXYZ)
+        self.assertEqual(uni, "Z⅄XMΛ∩ꞱSᴚQdONƜ⅂KſIH⅁ℲƎDƆB∀:")
+    def test_397_norm_flip(self) -> None:
+        uni = unicoder.turnlines(base_abcdefghijklmnopqrstuvwxyz)
+        self.assertEqual(uni, "zʎxʍʌnʇsɹbdouɯlʞɾᴉɥᵷɟǝpɔqɐ:")
+
     #
     def test_400_norm_sans(self) -> None:
         uni = unicoder.convert("fix", base_abcdefghijklmnopqrstuvwxyz)
         self.assertEqual(uni, base_abcdefghijklmnopqrstuvwxyz)
         self.assertNotEqual(base_abcdefghijklmnopqrstuvwxyz,
                             sans_abcdefghijklmnopqrstuvwxyz)
         self.assertNotEqual(mono_abcdefghijklmnopqrstuvwxyz,
@@ -529,45 +698,62 @@
         uni = unicoder.convert("fatslantvect", base_ABCDEFGHIJKLMNOPQRSTUVWXYZ)
         self.assertEqual(uni, bold_ital_sans_ABCDEFGHIJKLMNOPQRSTUVWXYZ)
     def test_465_bold_ital_sans(self) -> None:
         uni = unicoder.bold(unicoder.ital(
             unicoder.sans(base_abcdefghijklmnopqrstuvwxyz)))
         self.assertEqual(uni, bold_ital_sans_abcdefghijklmnopqrstuvwxyz)
     def test_466_bold_ital_sans(self) -> None:
-        uni = unicoder.sans(
-            unicoder.bold(unicoder.ital(base_abcdefghijklmnopqrstuvwxyz)))
+        uni = unicoder.ital(unicoder.bold(
+            unicoder.sans(base_abcdefghijklmnopqrstuvwxyz)))
         self.assertEqual(uni, bold_ital_sans_abcdefghijklmnopqrstuvwxyz)
     def test_467_bold_ital_sans(self) -> None:
+        uni = unicoder.sans(
+            unicoder.bold(unicoder.ital(base_abcdefghijklmnopqrstuvwxyz)))
+    def test_468_bold_ital_sans(self) -> None:
+        uni = unicoder.bold(
+            unicoder.sans(unicoder.ital(base_abcdefghijklmnopqrstuvwxyz)))
+    def test_469_bold_ital_sans(self) -> None:
+        uni = unicoder.ital(
+            unicoder.sans(unicoder.bold(base_abcdefghijklmnopqrstuvwxyz)))
+    def test_470_bold_ital_sans(self) -> None:
         uni = unicoder.bold(unicoder.ital(
             unicoder.sans(base_ABCDEFGHIJKLMNOPQRSTUVWXYZ)))
         self.assertEqual(uni, bold_ital_sans_ABCDEFGHIJKLMNOPQRSTUVWXYZ)
-    def test_468_bold_ital_sans(self) -> None:
+    def test_471_bold_ital_sans(self) -> None:
         uni = unicoder.ital(unicoder.bold(
             unicoder.sans(base_ABCDEFGHIJKLMNOPQRSTUVWXYZ)))
         self.assertEqual(uni, bold_ital_sans_ABCDEFGHIJKLMNOPQRSTUVWXYZ)
-    def test_469_bold_ital_sans(self) -> None:
+    def test_472_bold_ital_sans(self) -> None:
         uni = unicoder.sans(
             unicoder.bold(unicoder.ital(base_ABCDEFGHIJKLMNOPQRSTUVWXYZ)))
         self.assertEqual(uni, bold_ital_sans_ABCDEFGHIJKLMNOPQRSTUVWXYZ)
-    def test_470_numm_bold_ital_sans(self) -> None:
+    def test_473_bold_ital_sans(self) -> None:
+        uni = unicoder.bold(
+            unicoder.sans(unicoder.ital(base_ABCDEFGHIJKLMNOPQRSTUVWXYZ)))
+        self.assertEqual(uni, bold_ital_sans_ABCDEFGHIJKLMNOPQRSTUVWXYZ)
+    def test_474_bold_ital_sans(self) -> None:
+        uni = unicoder.ital(
+            unicoder.sans(unicoder.bold(base_ABCDEFGHIJKLMNOPQRSTUVWXYZ)))
+        self.assertEqual(uni, bold_ital_sans_ABCDEFGHIJKLMNOPQRSTUVWXYZ)
+    def test_480_numm_bold_ital_sans(self) -> None:
         uni = unicoder.convert("fix", base_0123456789)
         self.assertEqual(uni, base_0123456789)
-    def test_471_numm_bold_ital_sans(self) -> None:
+    def test_481_numm_bold_ital_sans(self) -> None:
         uni = unicoder.convert("bolditalsans", base_0123456789)
         self.assertEqual(uni, bold_ital_sans_0123456789)
-    def test_472_numm_bold_ital_sans(self) -> None:
+    def test_482_numm_bold_ital_sans(self) -> None:
         uni = unicoder.convert("fatslantvect", base_0123456789)
         self.assertEqual(uni, bold_ital_sans_0123456789)
-    def test_475_numm_bold_ital_sans(self) -> None:
+    def test_485_numm_bold_ital_sans(self) -> None:
         uni = unicoder.bold(unicoder.ital(unicoder.sans(base_0123456789)))
         self.assertEqual(uni, bold_ital_sans_0123456789)
-    def test_476_numm_bold_ital_sans(self) -> None:
+    def test_486_numm_bold_ital_sans(self) -> None:
         uni = unicoder.sans(unicoder.bold(unicoder.ital(base_0123456789)))
         self.assertEqual(uni, bold_ital_sans_0123456789)
-    def test_479_numm_bold_ital_sans(self) -> None:
+    def test_489_numm_bold_ital_sans(self) -> None:
         self.assertEqual(bold_ital_sans_0123456789, bold_sans_0123456789)
     #
     def test_500_norm_frak(self) -> None:
         uni = unicoder.convert("fix", base_abcdefghijklmnopqrstuvwxyz)
         self.assertEqual(uni, base_abcdefghijklmnopqrstuvwxyz)
     def test_501_norm_frak(self) -> None:
         uni = unicoder.convert("frak", base_abcdefghijklmnopqrstuvwxyz)
@@ -621,14 +807,78 @@
     def test_517_bold_frak(self) -> None:
         uni = unicoder.bold(unicoder.fraktur(base_ABCDEFGHIJKLMNOPQRSTUVWXYZ))
         self.assertEqual(uni, ":𝕬𝕭𝕮𝕯𝕰𝕱𝕲𝕳𝕴𝕵𝕶𝕷𝕸𝕹𝕺𝕻𝕼𝕽𝕾𝕿𝖀𝖁𝖂𝖃𝖄𝖅")
     def test_518_bold_frak(self) -> None:
         uni = unicoder.bold(unicoder.fraktur(base_ABCDEFGHIJKLMNOPQRSTUVWXYZ))
         self.assertEqual(uni, ":𝕬𝕭𝕮𝕯𝕰𝕱𝕲𝕳𝕴𝕵𝕶𝕷𝕸𝕹𝕺𝕻𝕼𝕽𝕾𝕿𝖀𝖁𝖂𝖃𝖄𝖅")
     #
+    def test_550_norm_button(self) -> None:
+        uni = unicoder.convert("fix", base_abcdefghijklmnopqrstuvwxyz)
+        self.assertEqual(uni, base_abcdefghijklmnopqrstuvwxyz)
+    def test_551_norm_button(self) -> None:
+        uni = unicoder.convert("button", base_abcdefghijklmnopqrstuvwxyz)
+        self.assertEqual(uni, ":🅐🅑🅒🅓🅔🅕🅖🅗🅘🅙🅚🅛🅜🅝🅞🅟🅠🅡🅢🅣🅤🅥🅦🅧🅨🅩")
+    def test_552_norm_button(self) -> None:
+        uni = unicoder.convert("button", base_ABCDEFGHIJKLMNOPQRSTUVWXYZ)
+        self.assertEqual(uni, ":🅰🅱🅲🅳🅴🅵🅶🅷🅸🅹🅺🅻🅼🅽🅾🅿🆀🆁🆂🆃🆄🆅🆆🆇🆈🆉")
+    def test_553_numm_button(self) -> None:
+        uni = unicoder.convert("button", base_0123456789)
+        self.assertEqual(uni, ":⓿❶❷❸❹❺❻❼❽❾")
+    def test_555_norm_button(self) -> None:
+        uni = unicoder.button(base_abcdefghijklmnopqrstuvwxyz)
+        self.assertEqual(uni, ":🅐🅑🅒🅓🅔🅕🅖🅗🅘🅙🅚🅛🅜🅝🅞🅟🅠🅡🅢🅣🅤🅥🅦🅧🅨🅩")
+    def test_556_norm_button(self) -> None:
+        uni = unicoder.button(base_ABCDEFGHIJKLMNOPQRSTUVWXYZ)
+        self.assertEqual(uni, ":🅰🅱🅲🅳🅴🅵🅶🅷🅸🅹🅺🅻🅼🅽🅾🅿🆀🆁🆂🆃🆄🆅🆆🆇🆈🆉")
+    def test_557_numm_button(self) -> None:
+        uni = unicoder.button(base_0123456789)
+        self.assertEqual(uni, ":⓿❶❷❸❹❺❻❼❽❾")
+    def test_560_norm_circled(self) -> None:
+        uni = unicoder.convert("fix", base_abcdefghijklmnopqrstuvwxyz)
+        self.assertEqual(uni, base_abcdefghijklmnopqrstuvwxyz)
+    def test_561_norm_circled(self) -> None:
+        uni = unicoder.convert("circ", base_abcdefghijklmnopqrstuvwxyz)
+        self.assertEqual(uni, ":ⓐⓑⓒⓓⓔⓕⓖⓗⓘⓙⓚⓛⓜⓝⓞⓟⓠⓡⓢⓣⓤⓥⓦⓧⓨⓩ")
+    def test_562_norm_circled(self) -> None:
+        uni = unicoder.convert("circ", base_ABCDEFGHIJKLMNOPQRSTUVWXYZ)
+        self.assertEqual(uni, ":ⒶⒷⒸⒹⒺⒻⒼⒽⒾⒿⓀⓁⓂⓃⓄⓅⓆⓇⓈⓉⓊⓋⓌⓍⓎⓏ")
+    def test_563_numm_circled(self) -> None:
+        uni = unicoder.convert("circ", base_0123456789)
+        self.assertEqual(uni, ":⓪①②③④⑤⑥⑦⑧⑨")
+    def test_565_norm_circled(self) -> None:
+        uni = unicoder.circled(base_abcdefghijklmnopqrstuvwxyz)
+        self.assertEqual(uni, ":ⓐⓑⓒⓓⓔⓕⓖⓗⓘⓙⓚⓛⓜⓝⓞⓟⓠⓡⓢⓣⓤⓥⓦⓧⓨⓩ")
+    def test_566_norm_circled(self) -> None:
+        uni = unicoder.circled(base_ABCDEFGHIJKLMNOPQRSTUVWXYZ)
+        self.assertEqual(uni, ":ⒶⒷⒸⒹⒺⒻⒼⒽⒾⒿⓀⓁⓂⓃⓄⓅⓆⓇⓈⓉⓊⓋⓌⓍⓎⓏ")
+    def test_567_numm_circled(self) -> None:
+        uni = unicoder.circled(base_0123456789)
+        self.assertEqual(uni, ":⓪①②③④⑤⑥⑦⑧⑨")
+    def test_570_norm_parens(self) -> None:
+        uni = unicoder.convert("fix", base_abcdefghijklmnopqrstuvwxyz)
+        self.assertEqual(uni, base_abcdefghijklmnopqrstuvwxyz)
+    def test_571_norm_parens(self) -> None:
+        uni = unicoder.convert("parens", base_abcdefghijklmnopqrstuvwxyz)
+        self.assertEqual(uni, ":⒜⒝⒞⒟⒠⒡⒢⒣⒤⒥⒦⒧⒨⒩⒪⒫⒬⒭⒮⒯⒰⒱⒲⒳⒴⒵")
+    def test_572_norm_parens(self) -> None:
+        uni = unicoder.convert("parens", base_ABCDEFGHIJKLMNOPQRSTUVWXYZ)
+        self.assertEqual(uni, ":🄐🄑🄒🄓🄔🄕🄖🄗🄘🄙🄚🄛🄜🄝🄞🄟🄠🄡🄢🄣🄤🄥🄦🄧🄨🄩")
+    def test_573_numm_parens(self) -> None:
+        uni = unicoder.convert("parens", base_0123456789)
+        self.assertEqual(uni, ":⒪⑴⑵⑶⑷⑸⑹⑺⑻⑼")
+    def test_575_norm_parens(self) -> None:
+        uni = unicoder.parens(base_abcdefghijklmnopqrstuvwxyz)
+        self.assertEqual(uni, ":⒜⒝⒞⒟⒠⒡⒢⒣⒤⒥⒦⒧⒨⒩⒪⒫⒬⒭⒮⒯⒰⒱⒲⒳⒴⒵")
+    def test_576_norm_parens(self) -> None:
+        uni = unicoder.parens(base_ABCDEFGHIJKLMNOPQRSTUVWXYZ)
+        self.assertEqual(uni, ":🄐🄑🄒🄓🄔🄕🄖🄗🄘🄙🄚🄛🄜🄝🄞🄟🄠🄡🄢🄣🄤🄥🄦🄧🄨🄩")
+    def test_577_numm_parens(self) -> None:
+        uni = unicoder.parens(base_0123456789)
+        self.assertEqual(uni, ":⒪⑴⑵⑶⑷⑸⑹⑺⑻⑼")
+    #
     def test_600_norm_greek(self) -> None:
         uni = unicoder.convert("fix", base_abcdefghijklmnopqrstuvwxyz)
         self.assertEqual(uni, base_abcdefghijklmnopqrstuvwxyz)
     def test_601_norm_greek(self) -> None:
         uni = unicoder.convert("greek", base_abcdefghijklmnopqrstuvwxyz)
         self.assertEqual(uni, ":αβχδεφγηιικλμνοπκρστω∂ψξυζ")
     def test_602_norm_greek(self) -> None:
@@ -656,86 +906,172 @@
         uni = unicoder.convert("boldgreek", base_abcdefghijklmnopqrstuvwxyz)
         self.assertEqual(uni, ":𝛂𝛃𝛘𝛅𝛆𝛗𝛄𝛈𝛊𝛊𝛋𝛌𝛍𝛎𝛐𝛑𝛋𝛒𝛔𝛕𝛚𝛛𝛙𝛏𝛖𝛇")
     def test_622_bold_greek(self) -> None:
         uni = unicoder.convert("fatmath", base_abcdefghijklmnopqrstuvwxyz)
         self.assertEqual(uni, ":𝛂𝛃𝛘𝛅𝛆𝛗𝛄𝛈𝛊𝛊𝛋𝛌𝛍𝛎𝛐𝛑𝛋𝛒𝛔𝛕𝛚𝛛𝛙𝛏𝛖𝛇")
     def test_623_bold_greek(self) -> None:
         uni = unicoder.convert("boldgreek", base_ABCDEFGHIJKLMNOPQRSTUVWXYZ)
-        self.assertEqual(uni, ":𝚨𝚩𝚾𝚫𝚬𝚽𝚪𝚮𝚰𝚰𝚱𝚲𝚳𝚴𝚶𝚷𝚱𝚸𝚺𝚻𝛀∇𝚿𝚵𝚼𝚭")
+        self.assertEqual(uni, ":𝚨𝚩𝚾𝚫𝚬𝚽𝚪𝚮𝚰𝚰𝚱𝚲𝚳𝚴𝚶𝚷𝚱𝚸𝚺𝚻𝛀𝛁𝚿𝚵𝚼𝚭")
     def test_624_bold_greek(self) -> None:
         uni = unicoder.convert("fatmath", base_ABCDEFGHIJKLMNOPQRSTUVWXYZ)
-        self.assertEqual(uni, ":𝚨𝚩𝚾𝚫𝚬𝚽𝚪𝚮𝚰𝚰𝚱𝚲𝚳𝚴𝚶𝚷𝚱𝚸𝚺𝚻𝛀∇𝚿𝚵𝚼𝚭")
+        self.assertEqual(uni, ":𝚨𝚩𝚾𝚫𝚬𝚽𝚪𝚮𝚰𝚰𝚱𝚲𝚳𝚴𝚶𝚷𝚱𝚸𝚺𝚻𝛀𝛁𝚿𝚵𝚼𝚭")
     def test_625_bold_greek(self) -> None:
         uni = unicoder.bold(unicoder.greek(base_abcdefghijklmnopqrstuvwxyz))
         self.assertEqual(uni, ":𝛂𝛃𝛘𝛅𝛆𝛗𝛄𝛈𝛊𝛊𝛋𝛌𝛍𝛎𝛐𝛑𝛋𝛒𝛔𝛕𝛚𝛛𝛙𝛏𝛖𝛇")
     def test_626_bold_greek(self) -> None:
         uni = unicoder.greek(unicoder.bold(base_abcdefghijklmnopqrstuvwxyz))
         self.assertEqual(uni, ":𝛂𝛃𝛘𝛅𝛆𝛗𝛄𝛈𝛊𝛊𝛋𝛌𝛍𝛎𝛐𝛑𝛋𝛒𝛔𝛕𝛚𝛛𝛙𝛏𝛖𝛇")
     def test_627_bold_greek(self) -> None:
         uni = unicoder.bold(unicoder.greek(base_ABCDEFGHIJKLMNOPQRSTUVWXYZ))
-        self.assertEqual(uni, ":𝚨𝚩𝚾𝚫𝚬𝚽𝚪𝚮𝚰𝚰𝚱𝚲𝚳𝚴𝚶𝚷𝚱𝚸𝚺𝚻𝛀∇𝚿𝚵𝚼𝚭")
+        self.assertEqual(uni, ":𝚨𝚩𝚾𝚫𝚬𝚽𝚪𝚮𝚰𝚰𝚱𝚲𝚳𝚴𝚶𝚷𝚱𝚸𝚺𝚻𝛀𝛁𝚿𝚵𝚼𝚭")
     def test_628_bold_greek(self) -> None:
         uni = unicoder.greek(unicoder.bold(base_ABCDEFGHIJKLMNOPQRSTUVWXYZ))
-        self.assertEqual(uni, ":𝚨𝚩𝚾𝚫𝚬𝚽𝚪𝚮𝚰𝚰𝚱𝚲𝚳𝚴𝚶𝚷𝚱𝚸𝚺𝚻𝛀∇𝚿𝚵𝚼𝚭")
+        self.assertEqual(uni, ":𝚨𝚩𝚾𝚫𝚬𝚽𝚪𝚮𝚰𝚰𝚱𝚲𝚳𝚴𝚶𝚷𝚱𝚸𝚺𝚻𝛀𝛁𝚿𝚵𝚼𝚭")
     def test_641_ital_greek(self) -> None:
         uni = unicoder.convert("italgreek", base_abcdefghijklmnopqrstuvwxyz)
         self.assertEqual(uni, ":𝛼𝛽𝜒𝛿𝜀𝜑𝛾𝜂𝜄𝜄𝜅𝜆𝜇𝜈𝜊𝜋𝜅𝜌𝜎𝜏𝜔𝜕𝜓𝜉𝜐𝜁")
     def test_642_ital_greek(self) -> None:
         uni = unicoder.convert("slantmath", base_abcdefghijklmnopqrstuvwxyz)
         self.assertEqual(uni, ":𝛼𝛽𝜒𝛿𝜀𝜑𝛾𝜂𝜄𝜄𝜅𝜆𝜇𝜈𝜊𝜋𝜅𝜌𝜎𝜏𝜔𝜕𝜓𝜉𝜐𝜁")
     def test_643_ital_greek(self) -> None:
         uni = unicoder.convert("italgreek", base_ABCDEFGHIJKLMNOPQRSTUVWXYZ)
-        self.assertEqual(uni, ":𝛢𝛣𝛸𝛥𝛦𝛷𝛤𝛨𝛪𝛪𝛫𝛬𝛭𝛮𝛰𝛱𝛫𝛲𝛴𝛵𝛺∇𝛹𝛯𝛶𝛧")
+        self.assertEqual(uni, ":𝛢𝛣𝛸𝛥𝛦𝛷𝛤𝛨𝛪𝛪𝛫𝛬𝛭𝛮𝛰𝛱𝛫𝛲𝛴𝛵𝛺𝛻𝛹𝛯𝛶𝛧")
     def test_644_ital_greek(self) -> None:
         uni = unicoder.convert("slantmath", base_ABCDEFGHIJKLMNOPQRSTUVWXYZ)
-        self.assertEqual(uni, ":𝛢𝛣𝛸𝛥𝛦𝛷𝛤𝛨𝛪𝛪𝛫𝛬𝛭𝛮𝛰𝛱𝛫𝛲𝛴𝛵𝛺∇𝛹𝛯𝛶𝛧")
+        self.assertEqual(uni, ":𝛢𝛣𝛸𝛥𝛦𝛷𝛤𝛨𝛪𝛪𝛫𝛬𝛭𝛮𝛰𝛱𝛫𝛲𝛴𝛵𝛺𝛻𝛹𝛯𝛶𝛧")
     def test_645_ital_greek(self) -> None:
         uni = unicoder.ital(unicoder.greek(base_abcdefghijklmnopqrstuvwxyz))
         self.assertEqual(uni, ":𝛼𝛽𝜒𝛿𝜀𝜑𝛾𝜂𝜄𝜄𝜅𝜆𝜇𝜈𝜊𝜋𝜅𝜌𝜎𝜏𝜔𝜕𝜓𝜉𝜐𝜁")
     def test_646_ital_greek(self) -> None:
         uni = unicoder.greek(unicoder.ital(base_abcdefghijklmnopqrstuvwxyz))
         self.assertEqual(uni, ":𝛼𝛽𝜒𝛿𝜀𝜑𝛾𝜂𝜄𝜄𝜅𝜆𝜇𝜈𝜊𝜋𝜅𝜌𝜎𝜏𝜔𝜕𝜓𝜉𝜐𝜁")
     def test_647_ital_greek(self) -> None:
         uni = unicoder.ital(unicoder.greek(base_ABCDEFGHIJKLMNOPQRSTUVWXYZ))
-        self.assertEqual(uni, ":𝛢𝛣𝛸𝛥𝛦𝛷𝛤𝛨𝛪𝛪𝛫𝛬𝛭𝛮𝛰𝛱𝛫𝛲𝛴𝛵𝛺∇𝛹𝛯𝛶𝛧")
+        self.assertEqual(uni, ":𝛢𝛣𝛸𝛥𝛦𝛷𝛤𝛨𝛪𝛪𝛫𝛬𝛭𝛮𝛰𝛱𝛫𝛲𝛴𝛵𝛺𝛻𝛹𝛯𝛶𝛧")
     def test_648_ital_greek(self) -> None:
         uni = unicoder.greek(unicoder.ital(base_ABCDEFGHIJKLMNOPQRSTUVWXYZ))
-        self.assertEqual(uni, ":𝛢𝛣𝛸𝛥𝛦𝛷𝛤𝛨𝛪𝛪𝛫𝛬𝛭𝛮𝛰𝛱𝛫𝛲𝛴𝛵𝛺∇𝛹𝛯𝛶𝛧")
+        self.assertEqual(uni, ":𝛢𝛣𝛸𝛥𝛦𝛷𝛤𝛨𝛪𝛪𝛫𝛬𝛭𝛮𝛰𝛱𝛫𝛲𝛴𝛵𝛺𝛻𝛹𝛯𝛶𝛧")
     def test_661_bold_ital_greek(self) -> None:
         uni = unicoder.convert("bolditalgreek", base_abcdefghijklmnopqrstuvwxyz)
         self.assertEqual(uni, ":𝜶𝜷𝝌𝜹𝜺𝝋𝜸𝜼𝜾𝜾𝜿𝝀𝝁𝝂𝝄𝝅𝜿𝝆𝝈𝝉𝝎𝝏𝝍𝝃𝝊𝜻")
     def test_662_bold_ital_greek(self) -> None:
         uni = unicoder.convert("fatslantmath", base_abcdefghijklmnopqrstuvwxyz)
         self.assertEqual(uni, ":𝜶𝜷𝝌𝜹𝜺𝝋𝜸𝜼𝜾𝜾𝜿𝝀𝝁𝝂𝝄𝝅𝜿𝝆𝝈𝝉𝝎𝝏𝝍𝝃𝝊𝜻")
     def test_663_bold_ital_greek(self) -> None:
         uni = unicoder.convert("bolditalgreek", base_ABCDEFGHIJKLMNOPQRSTUVWXYZ)
-        self.assertEqual(uni, ":𝜜𝜝𝜲𝜟𝜠𝜱𝜞𝜢𝜤𝜤𝜥𝜦𝜧𝜨𝜪𝜫𝜥𝜬𝜮𝜯𝜴∇𝜳𝜩𝜰𝜡")
+        self.assertEqual(uni, ":𝜜𝜝𝜲𝜟𝜠𝜱𝜞𝜢𝜤𝜤𝜥𝜦𝜧𝜨𝜪𝜫𝜥𝜬𝜮𝜯𝜴𝜵𝜳𝜩𝜰𝜡")
     def test_664_bold_ital_greek(self) -> None:
         uni = unicoder.convert("fatslantmath", base_ABCDEFGHIJKLMNOPQRSTUVWXYZ)
-        self.assertEqual(uni, ":𝜜𝜝𝜲𝜟𝜠𝜱𝜞𝜢𝜤𝜤𝜥𝜦𝜧𝜨𝜪𝜫𝜥𝜬𝜮𝜯𝜴∇𝜳𝜩𝜰𝜡")
+        self.assertEqual(uni, ":𝜜𝜝𝜲𝜟𝜠𝜱𝜞𝜢𝜤𝜤𝜥𝜦𝜧𝜨𝜪𝜫𝜥𝜬𝜮𝜯𝜴𝜵𝜳𝜩𝜰𝜡")
     def test_665_bold_ital_greek(self) -> None:
         uni = unicoder.bold(unicoder.ital(
             unicoder.greek(base_abcdefghijklmnopqrstuvwxyz)))
         self.assertEqual(uni, ":𝜶𝜷𝝌𝜹𝜺𝝋𝜸𝜼𝜾𝜾𝜿𝝀𝝁𝝂𝝄𝝅𝜿𝝆𝝈𝝉𝝎𝝏𝝍𝝃𝝊𝜻")
     def test_666_bold_ital_greek(self) -> None:
         uni = unicoder.greek(
             unicoder.bold(unicoder.ital(base_abcdefghijklmnopqrstuvwxyz)))
         self.assertEqual(uni, ":𝜶𝜷𝝌𝜹𝜺𝝋𝜸𝜼𝜾𝜾𝜿𝝀𝝁𝝂𝝄𝝅𝜿𝝆𝝈𝝉𝝎𝝏𝝍𝝃𝝊𝜻")
     def test_667_bold_ital_greek(self) -> None:
         uni = unicoder.bold(unicoder.ital(
             unicoder.greek(base_ABCDEFGHIJKLMNOPQRSTUVWXYZ)))
-        self.assertEqual(uni, ":𝜜𝜝𝜲𝜟𝜠𝜱𝜞𝜢𝜤𝜤𝜥𝜦𝜧𝜨𝜪𝜫𝜥𝜬𝜮𝜯𝜴∇𝜳𝜩𝜰𝜡")
+        self.assertEqual(uni, ":𝜜𝜝𝜲𝜟𝜠𝜱𝜞𝜢𝜤𝜤𝜥𝜦𝜧𝜨𝜪𝜫𝜥𝜬𝜮𝜯𝜴𝜵𝜳𝜩𝜰𝜡")
     def test_668_bold_ital_greek(self) -> None:
         uni = unicoder.ital(unicoder.bold(
             unicoder.greek(base_ABCDEFGHIJKLMNOPQRSTUVWXYZ)))
-        self.assertEqual(uni, ":𝜜𝜝𝜲𝜟𝜠𝜱𝜞𝜢𝜤𝜤𝜥𝜦𝜧𝜨𝜪𝜫𝜥𝜬𝜮𝜯𝜴∇𝜳𝜩𝜰𝜡")
+        self.assertEqual(uni, ":𝜜𝜝𝜲𝜟𝜠𝜱𝜞𝜢𝜤𝜤𝜥𝜦𝜧𝜨𝜪𝜫𝜥𝜬𝜮𝜯𝜴𝜵𝜳𝜩𝜰𝜡")
     def test_669_bold_ital_greek(self) -> None:
         uni = unicoder.greek(
             unicoder.bold(unicoder.ital(base_ABCDEFGHIJKLMNOPQRSTUVWXYZ)))
-        self.assertEqual(uni, ":𝜜𝜝𝜲𝜟𝜠𝜱𝜞𝜢𝜤𝜤𝜥𝜦𝜧𝜨𝜪𝜫𝜥𝜬𝜮𝜯𝜴∇𝜳𝜩𝜰𝜡")
+        self.assertEqual(uni, ":𝜜𝜝𝜲𝜟𝜠𝜱𝜞𝜢𝜤𝜤𝜥𝜦𝜧𝜨𝜪𝜫𝜥𝜬𝜮𝜯𝜴𝜵𝜳𝜩𝜰𝜡")
+
+    def test_670_bold_ital_greek(self) -> None:
+        uni = unicoder.bold(
+            unicoder.greek(unicoder.ital(base_ABCDEFGHIJKLMNOPQRSTUVWXYZ)))
+        self.assertEqual(uni, ":𝜜𝜝𝜲𝜟𝜠𝜱𝜞𝜢𝜤𝜤𝜥𝜦𝜧𝜨𝜪𝜫𝜥𝜬𝜮𝜯𝜴𝜵𝜳𝜩𝜰𝜡")
+    def test_671_bold_ital_greek(self) -> None:
+        uni = unicoder.ital(
+            unicoder.greek(unicoder.bold(base_ABCDEFGHIJKLMNOPQRSTUVWXYZ)))
+        self.assertEqual(uni, ":𝜜𝜝𝜲𝜟𝜠𝜱𝜞𝜢𝜤𝜤𝜥𝜦𝜧𝜨𝜪𝜫𝜥𝜬𝜮𝜯𝜴𝜵𝜳𝜩𝜰𝜡")
+    def test_672_bold_ital_greek(self) -> None:
+        uni = unicoder.bold(
+            unicoder.ital(unicoder.greek(base_ABCDEFGHIJKLMNOPQRSTUVWXYZ)))
+        self.assertEqual(uni, ":𝜜𝜝𝜲𝜟𝜠𝜱𝜞𝜢𝜤𝜤𝜥𝜦𝜧𝜨𝜪𝜫𝜥𝜬𝜮𝜯𝜴𝜵𝜳𝜩𝜰𝜡")
+    def test_673_bold_ital_greek(self) -> None:
+        uni = unicoder.bold(
+            unicoder.greek(unicoder.ital(base_abcdefghijklmnopqrstuvwxyz)))
+        self.assertEqual(uni, ":𝜶𝜷𝝌𝜹𝜺𝝋𝜸𝜼𝜾𝜾𝜿𝝀𝝁𝝂𝝄𝝅𝜿𝝆𝝈𝝉𝝎𝝏𝝍𝝃𝝊𝜻")
+    def test_674_bold_ital_greek(self) -> None:
+        uni = unicoder.ital(
+            unicoder.greek(unicoder.bold(base_abcdefghijklmnopqrstuvwxyz)))
+        self.assertEqual(uni, ":𝜶𝜷𝝌𝜹𝜺𝝋𝜸𝜼𝜾𝜾𝜿𝝀𝝁𝝂𝝄𝝅𝜿𝝆𝝈𝝉𝝎𝝏𝝍𝝃𝝊𝜻")
+    def test_675_bold_ital_greek(self) -> None:
+        uni = unicoder.bold(
+            unicoder.ital(unicoder.greek(base_abcdefghijklmnopqrstuvwxyz)))
+        self.assertEqual(uni, ":𝜶𝜷𝝌𝜹𝜺𝝋𝜸𝜼𝜾𝜾𝜿𝝀𝝁𝝂𝝄𝝅𝜿𝝆𝝈𝝉𝝎𝝏𝝍𝝃𝝊𝜻")
+
+    def test_680_norm_greek(self) -> None:
+        uni = unicoder.convert("greek", ":foobar")
+        self.assertEqual(uni, ":φωβαρ")
+    def test_681_norm_greek(self) -> None:
+        uni = unicoder.convert("greek", ":FOOBAR")
+        self.assertEqual(uni, ":ΦΩΒΑΡ")
+    def test_682_norm_greek(self) -> None:
+        uni = unicoder.convert("boldgreek", ":foobar")
+        self.assertEqual(uni, ":𝛗𝛚𝛃𝛂𝛒")
+    def test_683_norm_greek(self) -> None:
+        uni = unicoder.convert("boldgreek", ":FOOBAR")
+        self.assertEqual(uni, ":𝚽𝛀𝚩𝚨𝚸")
+    def test_684_norm_greek(self) -> None:
+        uni = unicoder.convert("italgreek", ":foobar")
+        self.assertEqual(uni, ":𝜑𝜔𝛽𝛼𝜌")
+    def test_685_norm_greek(self) -> None:
+        uni = unicoder.convert("italgreek", ":FOOBAR")
+        self.assertEqual(uni, ":𝛷𝛺𝛣𝛢𝛲")
+    def test_686_norm_greek(self) -> None:
+        uni = unicoder.convert("italboldgreek", ":foobar")
+        self.assertEqual(uni, ":𝝋𝝎𝜷𝜶𝝆")
+    def test_687_norm_greek(self) -> None:
+        uni = unicoder.convert("italboldgreek", ":FOOBAR")
+        self.assertEqual(uni, ":𝜱𝜴𝜝𝜜𝜬")
+    def test_690_norm_greek(self) -> None:
+        uni = unicoder.greek(":foobar")
+        self.assertEqual(uni, ":φωβαρ")
+    def test_691_norm_greek(self) -> None:
+        uni = unicoder.greek(":FOOBAR")
+        self.assertEqual(uni, ":ΦΩΒΑΡ")
+    def test_692_norm_greek(self) -> None:
+        uni = unicoder.greek(unicoder.bold(":foobar"))
+        self.assertEqual(uni, ":𝛗𝛚𝛃𝛂𝛒")
+    def test_693_norm_greek(self) -> None:
+        uni = unicoder.greek(unicoder.bold(":FOOBAR"))
+        self.assertEqual(uni, ":𝚽𝛀𝚩𝚨𝚸")
+    def test_694_norm_greek(self) -> None:
+        uni = unicoder.greek(unicoder.ital(":foobar"))
+        self.assertEqual(uni, ":𝜑𝜔𝛽𝛼𝜌")
+    def test_695_norm_greek(self) -> None:
+        uni = unicoder.greek(unicoder.ital(":FOOBAR"))
+        self.assertEqual(uni, ":𝛷𝛺𝛣𝛢𝛲")
+    def test_696_norm_greek(self) -> None:
+        uni = unicoder.greek(unicoder.ital(unicoder.bold(":foobar")))
+        self.assertEqual(uni, ":𝝋𝝎𝜷𝜶𝝆")
+    def test_697_norm_greek(self) -> None:
+        uni = unicoder.greek(unicoder.ital(unicoder.bold(":FOOBAR")))
+        self.assertEqual(uni, ":𝜱𝜴𝜝𝜜𝜬")
+    def test_698_norm_greek_notfound(self) -> None:
+        old = unicoder.norm_greek_upper
+        unicoder.norm_greek_upper = unicoder.norm_greek_lower
+        uni = unicoder.greek(":FOOBAR")
+        unicoder.norm_greek_upper = old
+        self.assertEqual(uni, ":FOOBAR")
+    def test_699_norm_greek_notfound(self) -> None:
+        old = unicoder.norm_greek_lower
+        unicoder.norm_greek_lower = unicoder.norm_greek_upper
+        uni = unicoder.greek(unicoder.bold(":foobar"))
+        unicoder.norm_greek_lower = old
+        self.assertEqual(uni, ":foobar")
     #
     def test_700_norm_rune(self) -> None:
         uni = unicoder.convert("fix", base_abcdefghijklmnopqrstuvwxyz)
         self.assertEqual(uni, base_abcdefghijklmnopqrstuvwxyz)
     def test_701_norm_rune(self) -> None:
         uni = unicoder.convert("rune", base_abcdefghijklmnopqrstuvwxyz)
         self.assertEqual(uni, ":ᚨᛒᚳᛞᛖᚠᚷᚺᛁᛡᚳᛚᛗᚾᛟᛈᚳᚱᛋᛏᚹᚹᛕᚳᛋᛇᛉ")
@@ -753,14 +1089,32 @@
         self.assertEqual(uni, ":ᚨᛒᚳᛞᛖᚠᚷᚺᛁᛡᚳᛚᛗᚾᛟᛈᚳᚱᛋᛏᚹᚹᛕᚳᛋᛇᛉ")
     def test_706_norm_rune(self) -> None:
         uni = unicoder.rune(base_abcdefghijklmnopqrstuvwxyz)
         self.assertEqual(uni, ":ᚨᛒᚳᛞᛖᚠᚷᚺᛁᛡᚳᛚᛗᚾᛟᛈᚳᚱᛋᛏᚹᚹᛕᚳᛋᛇᛉ")
     def test_707_norm_rune(self) -> None:
         uni = unicoder.rune(base_ABCDEFGHIJKLMNOPQRSTUVWXYZ)
         self.assertEqual(uni, ":ᚨᛒᚳᛞᛖᚠᚷᚺᛁᛡᚳᛚᛗᚾᛟᛈᚳᚱᛋᛏᚹᚹᛕᚳᛋᛇᛉ")
+    def test_741_norm_rune_quaengeln(self) -> None:
+        uni = unicoder.rune(":quaengeln")
+        self.assertEqual(uni, ":ᚳᚨᛖᛜᛖᛚᚾ")
+    def test_742_norm_rune_quaengeln(self) -> None:
+        uni = unicoder.rune(":QUAENGELN")
+        self.assertEqual(uni, ":ᚳᚨᛖᛜᛖᛚᚾ")
+    def test_748_norm_rune_notfound(self) -> None:
+        old = unicoder.norm_rune_lower
+        unicoder.norm_rune_lower = unicoder.norm_greek_upper
+        uni = unicoder.rune(":FOOBAR")
+        unicoder.norm_rune_lower = old
+        self.assertEqual(uni, ":foobar")
+    def test_749_norm_rune_notfound(self) -> None:
+        old = unicoder.norm_rune_lower
+        unicoder.norm_rune_lower = unicoder.norm_greek_upper
+        uni = unicoder.rune(":foobar")
+        unicoder.norm_rune_lower = old
+        self.assertEqual(uni, ":foobar")
     #
     def test_800_norm_value(self) -> None:
         txt = "15 km/h more"
         uni = unicoder.convert("fix", txt)
         self.assertEqual(uni, "15 km/h more")
         self.assertEqual(uni, txt)
     def test_801_thin_value(self) -> None:
@@ -779,14 +1133,132 @@
     def test_803_thin_nobr_value(self) -> None:
         txt = "15 km/h more"
         thin = unicoder.convert("thin", txt)
         nobr = unicoder.convert("nobr", txt)
         self.assertEqual(thin, "15 km/h more")
         self.assertEqual(nobr, "15 km/h more")
         self.assertNotEqual(thin, nobr)
+    def test_809_thin_value_command(self) -> None:
+        txt = "15 km/h more"
+        uni = unicoder.convert("1+", txt)
+        self.assertEqual(uni, "1+ 15 km/h more")
+        self.assertNotEqual(uni, txt)
+    def test_850_superscript(self) -> None:
+        txt = "+-0123456789"
+        uni = unicoder.convert("super", txt)
+        self.assertEqual(uni, "⁺⁻⁰¹²³⁴⁵⁶⁷⁸⁹")
+        self.assertNotEqual(uni, txt)
+    def test_851_superscript(self) -> None:
+        txt = "+-0123456789"
+        uni = unicoder.superscript(txt)
+        self.assertEqual(uni, "⁺⁻⁰¹²³⁴⁵⁶⁷⁸⁹")
+        self.assertNotEqual(uni, txt)
+    def test_854_superscript(self) -> None:
+        txt = "(-20)(X)"
+        uni = unicoder.convert("super", txt)
+        self.assertEqual(uni, "⁽⁻²⁰⁾(X)")
+        self.assertNotEqual(uni, txt)
+    def test_855_superscript(self) -> None:
+        txt = "(-20)(X)"
+        uni = unicoder.superscript(txt)
+        self.assertEqual(uni, "⁽⁻²⁰⁾(X)")
+        self.assertNotEqual(uni, txt)
+    def test_860_power(self) -> None:
+        txt = "+-0123456789"
+        uni = unicoder.convert("power", txt)
+        self.assertEqual(uni, txt)
+    def test_861_power(self) -> None:
+        txt = "+-0123456789"
+        uni = unicoder.power(txt)
+        self.assertEqual(uni, txt)
+    def test_862_power(self) -> None:
+        txt = "^+-0123456789"
+        uni = unicoder.convert("power", txt)
+        self.assertEqual(uni, "⁺⁻⁰¹²³⁴⁵⁶⁷⁸⁹")
+        self.assertNotEqual(uni, txt)
+    def test_863_power(self) -> None:
+        txt = "^+-0123456789"
+        uni = unicoder.power(txt)
+        self.assertEqual(uni, "⁺⁻⁰¹²³⁴⁵⁶⁷⁸⁹")
+        self.assertNotEqual(uni, txt)
+    def test_864_power(self) -> None:
+        txt = "(-20)(X)"
+        uni = unicoder.convert("power", txt)
+        self.assertEqual(uni, txt)
+    def test_865_power(self) -> None:
+        txt = "(-20)(X)"
+        uni = unicoder.power(txt)
+        self.assertEqual(uni, txt)
+    def test_866_power(self) -> None:
+        txt = "^(-20) (X)"
+        uni = unicoder.convert("power", txt)
+        self.assertEqual(uni, "⁽⁻²⁰⁾ (X)")
+        self.assertNotEqual(uni, txt)
+    def test_867_power(self) -> None:
+        txt = "^(-20) (X)"
+        uni = unicoder.power(txt)
+        self.assertEqual(uni, "⁽⁻²⁰⁾ (X)")
+        self.assertNotEqual(uni, txt)
+    def test_870_subscript(self) -> None:
+        txt = "+-0123456789"
+        uni = unicoder.convert("subi", txt)
+        self.assertEqual(uni, "₊₋₀₁₂₃₄₅₆₇₈₉")
+        self.assertNotEqual(uni, txt)
+    def test_871_subscript(self) -> None:
+        txt = "+-0123456789"
+        uni = unicoder.subscript(txt)
+        self.assertEqual(uni, "₊₋₀₁₂₃₄₅₆₇₈₉")
+        self.assertNotEqual(uni, txt)
+    def test_874_subscript(self) -> None:
+        txt = "(-20)(X)"
+        uni = unicoder.convert("subi", txt)
+        self.assertEqual(uni, "₍₋₂₀₎(X)")
+        self.assertNotEqual(uni, txt)
+    def test_875_subscript(self) -> None:
+        txt = "(-20)(X)"
+        uni = unicoder.subscript(txt)
+        self.assertEqual(uni, "₍₋₂₀₎(X)")
+        self.assertNotEqual(uni, txt)
+    def test_880_index(self) -> None:
+        txt = "+-0123456789"
+        uni = unicoder.convert("index", txt)
+        self.assertEqual(uni, txt)
+    def test_881_index(self) -> None:
+        txt = "+-0123456789"
+        uni = unicoder.indexed(txt)
+        self.assertEqual(uni, txt)
+    def test_882_index(self) -> None:
+        txt = "_+-0123456789"
+        uni = unicoder.convert("index", txt)
+        self.assertEqual(uni, "₊₋₀₁₂₃₄₅₆₇₈₉")
+        self.assertNotEqual(uni, txt)
+    def test_883_index(self) -> None:
+        txt = "_+-0123456789"
+        uni = unicoder.indexed(txt)
+        self.assertEqual(uni, "₊₋₀₁₂₃₄₅₆₇₈₉")
+        self.assertNotEqual(uni, txt)
+    def test_884_index(self) -> None:
+        txt = "(-20)(X)"
+        uni = unicoder.convert("index", txt)
+        self.assertEqual(uni, txt)
+    def test_885_index(self) -> None:
+        txt = "(-20)(X)"
+        uni = unicoder.indexed(txt)
+        self.assertEqual(uni, txt)
+    def test_886_index(self) -> None:
+        txt = "_(-20) (X)"
+        uni = unicoder.convert("index", txt)
+        self.assertEqual(uni, "₍₋₂₀₎ (X)")
+        self.assertNotEqual(uni, txt)
+    def test_887_index(self) -> None:
+        txt = "_(-20) (X)"
+        uni = unicoder.indexed(txt)
+        self.assertEqual(uni, "₍₋₂₀₎ (X)")
+        self.assertNotEqual(uni, txt)
+
     def test_900_norm_1_8(self) -> None:
         txt = "15 1/8 km/h more"
         uni = unicoder.convert("fix", txt)
         self.assertEqual(uni, "15 1/8 km/h more")
         self.assertEqual(uni, txt)
     def test_901_norm_1_8(self) -> None:
         txt = "15 1/8 km/h more"
@@ -885,41 +1357,48 @@
         self.assertNotEqual(uni, txt)
     def test_932_norm_2_3(self) -> None:
         txt = "15 2/3 km/h more"
         uni = unicoder.convert("fract", txt)
         self.assertEqual(uni, "15⅔ km/h more")
         self.assertNotEqual(uni, txt)
     def test_941_norm_1_5(self) -> None:
-        txt = "15 1/5 km/h more"
+        txt = "go 15 1/5 km/h more"
         uni = unicoder.convert("fract", txt)
-        self.assertEqual(uni, "15⅕ km/h more")
+        self.assertEqual(uni, "go 15⅕ km/h more")
         self.assertNotEqual(uni, txt)
     def test_942_norm_2_5(self) -> None:
-        txt = "15 2/5 km/h more"
+        txt = "go 15 2/5 km/h more"
         uni = unicoder.convert("fract", txt)
-        self.assertEqual(uni, "15⅖ km/h more")
+        self.assertEqual(uni, "go 15⅖ km/h more")
         self.assertNotEqual(uni, txt)
     def test_943_norm_3_5(self) -> None:
-        txt = "15 3/5 km/h more"
+        txt = "go 15 3/5 km/h more"
         uni = unicoder.convert("fract", txt)
-        self.assertEqual(uni, "15⅗ km/h more")
+        self.assertEqual(uni, "go 15⅗ km/h more")
         self.assertNotEqual(uni, txt)
     def test_944_norm_4_5(self) -> None:
-        txt = "15 4/5 km/h more"
+        txt = "go 15 4/5 km/h more"
         uni = unicoder.convert("fract", txt)
-        self.assertEqual(uni, "15⅘ km/h more")
+        self.assertEqual(uni, "go 15⅘ km/h more")
+        self.assertNotEqual(uni, txt)
+    def test_990_math(self) -> None:
+        txt = "A_1^2 + 1/4"
+        uni = unicoder.convert("math", txt)
+        self.assertEqual(uni, "Α₁² +¼")
         self.assertNotEqual(uni, txt)
 
 
 if __name__ == "__main__":
     from optparse import OptionParser
     _o = OptionParser("%prog [options] test*",
                       epilog=__doc__.strip().split("\n")[0])
     _o.add_option("-v", "--verbose", action="count", default=0,
                   help="increase logging level [%default]")
+    _o.add_option("--failfast", action="store_true", default=False,
+                  help="Stop the test run on the first error or failure. [%default]")
     _o.add_option("--xmlresults", metavar="FILE", default=None,
                   help="capture results as a junit xml file [%default]")
     _o.add_option("-l", "--logfile", metavar="FILE", default="",
                   help="additionally save the output log to a file [%default]")
     opt, args = _o.parse_args()
     logging.basicConfig(level=logging.WARNING - opt.verbose * 5)
     #
@@ -954,15 +1433,15 @@
     if not logfile:
         if xmlresults:
             import xmlrunner  # type: ignore
             Runner = xmlrunner.XMLTestRunner
             result = Runner(xmlresults).run(suite)
         else:
             Runner = unittest.TextTestRunner
-            result = Runner(verbosity=opt.verbose).run(suite)
+            result = Runner(verbosity=opt.verbose, failfast=opt.failfast).run(suite)
     else:
         Runner = unittest.TextTestRunner
         if xmlresults:
             import xmlrunner
             Runner = xmlrunner.XMLTestRunner
         result = Runner(logfile.stream, verbosity=opt.verbose).run(suite)  # type: ignore
     if not result.wasSuccessful():
```

