# Comparing `tmp/pypdf-4.1.0.tar.gz` & `tmp/pypdf-4.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypdf-4.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pypdf-4.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pypdf-4.1.0.tar` & `pypdf-4.2.0.tar`

### file list

```diff
@@ -1,62 +1,62 @@
--rw-r--r--   0        0        0      488 2024-03-03 11:49:51.414962 pypdf-4.1.0/.git-blame-ignore-revs
--rw-r--r--   0        0        0      542 2024-03-03 11:49:51.414962 pypdf-4.1.0/.readthedocs.yaml
--rw-r--r--   0        0        0    48963 2024-03-03 11:49:51.414962 pypdf-4.1.0/CHANGELOG.md
--rw-r--r--   0        0        0      896 2024-03-03 11:49:51.414962 pypdf-4.1.0/CONTRIBUTING.md
--rw-r--r--   0        0        0     4607 2024-03-03 11:49:51.414962 pypdf-4.1.0/CONTRIBUTORS.md
--rw-r--r--   0        0        0     1605 2024-03-03 11:49:51.414962 pypdf-4.1.0/LICENSE
--rw-r--r--   0        0        0       34 2024-03-03 11:49:51.414962 pypdf-4.1.0/MANIFEST.in
--rw-r--r--   0        0        0     4947 2024-03-03 11:49:51.418962 pypdf-4.1.0/README.md
--rw-r--r--   0        0        0     1292 2024-03-03 11:49:51.442962 pypdf-4.1.0/pypdf/__init__.py
--rw-r--r--   0        0        0    17997 2024-03-03 11:49:51.442962 pypdf-4.1.0/pypdf/_cmap.py
--rw-r--r--   0        0        0     1674 2024-03-03 11:49:51.442962 pypdf-4.1.0/pypdf/_codecs/__init__.py
--rw-r--r--   0        0        0   447237 2024-03-03 11:49:51.446961 pypdf-4.1.0/pypdf/_codecs/adobe_glyphs.py
--rw-r--r--   0        0        0     4269 2024-03-03 11:49:51.446961 pypdf-4.1.0/pypdf/_codecs/pdfdoc.py
--rw-r--r--   0        0        0     2630 2024-03-03 11:49:51.446961 pypdf-4.1.0/pypdf/_codecs/std.py
--rw-r--r--   0        0        0     3734 2024-03-03 11:49:51.446961 pypdf-4.1.0/pypdf/_codecs/symbol.py
--rw-r--r--   0        0        0     3742 2024-03-03 11:49:51.446961 pypdf-4.1.0/pypdf/_codecs/zapfding.py
--rw-r--r--   0        0        0     3054 2024-03-03 11:49:51.446961 pypdf-4.1.0/pypdf/_crypt_providers/__init__.py
--rw-r--r--   0        0        0     1711 2024-03-03 11:49:51.446961 pypdf-4.1.0/pypdf/_crypt_providers/_base.py
--rw-r--r--   0        0        0     4329 2024-03-03 11:49:51.446961 pypdf-4.1.0/pypdf/_crypt_providers/_cryptography.py
--rw-r--r--   0        0        0     3345 2024-03-03 11:49:51.446961 pypdf-4.1.0/pypdf/_crypt_providers/_fallback.py
--rw-r--r--   0        0        0     3381 2024-03-03 11:49:51.446961 pypdf-4.1.0/pypdf/_crypt_providers/_pycryptodome.py
--rw-r--r--   0        0        0    48920 2024-03-03 11:49:51.446961 pypdf-4.1.0/pypdf/_encryption.py
--rw-r--r--   0        0        0    24442 2024-03-03 11:49:51.446961 pypdf-4.1.0/pypdf/_merger.py
--rw-r--r--   0        0        0    93641 2024-03-03 11:49:51.450961 pypdf-4.1.0/pypdf/_page.py
--rw-r--r--   0        0        0     7186 2024-03-03 11:49:51.450961 pypdf-4.1.0/pypdf/_page_labels.py
--rw-r--r--   0        0        0     1897 2024-03-03 11:49:51.450961 pypdf-4.1.0/pypdf/_protocols.py
--rw-r--r--   0        0        0    81593 2024-03-03 11:49:51.450961 pypdf-4.1.0/pypdf/_reader.py
--rw-r--r--   0        0        0    10373 2024-03-03 11:49:51.450961 pypdf-4.1.0/pypdf/_text_extraction/__init__.py
--rw-r--r--   0        0        0      338 2024-03-03 11:49:51.450961 pypdf-4.1.0/pypdf/_text_extraction/_layout_mode/__init__.py
--rw-r--r--   0        0        0    14782 2024-03-03 11:49:51.450961 pypdf-4.1.0/pypdf/_text_extraction/_layout_mode/_fixed_width_page.py
--rw-r--r--   0        0        0     5099 2024-03-03 11:49:51.450961 pypdf-4.1.0/pypdf/_text_extraction/_layout_mode/_font.py
--rw-r--r--   0        0        0     4264 2024-03-03 11:49:51.450961 pypdf-4.1.0/pypdf/_text_extraction/_layout_mode/_font_widths.py
--rw-r--r--   0        0        0     8012 2024-03-03 11:49:51.450961 pypdf-4.1.0/pypdf/_text_extraction/_layout_mode/_text_state_manager.py
--rw-r--r--   0        0        0     5316 2024-03-03 11:49:51.450961 pypdf-4.1.0/pypdf/_text_extraction/_layout_mode/_text_state_params.py
--rw-r--r--   0        0        0    20090 2024-03-03 11:49:51.450961 pypdf-4.1.0/pypdf/_utils.py
--rw-r--r--   0        0        0       22 2024-03-03 11:49:51.450961 pypdf-4.1.0/pypdf/_version.py
--rw-r--r--   0        0        0   119479 2024-03-03 11:49:51.450961 pypdf-4.1.0/pypdf/_writer.py
--rw-r--r--   0        0        0    10925 2024-03-03 11:49:51.450961 pypdf-4.1.0/pypdf/_xobj_image_helpers.py
--rw-r--r--   0        0        0     1118 2024-03-03 11:49:51.450961 pypdf-4.1.0/pypdf/annotations/__init__.py
--rw-r--r--   0        0        0      910 2024-03-03 11:49:51.450961 pypdf-4.1.0/pypdf/annotations/_base.py
--rw-r--r--   0        0        0    11608 2024-03-03 11:49:51.450961 pypdf-4.1.0/pypdf/annotations/_markup_annotations.py
--rw-r--r--   0        0        0     1278 2024-03-03 11:49:51.450961 pypdf-4.1.0/pypdf/annotations/_non_markup_annotations.py
--rw-r--r--   0        0        0    19217 2024-03-03 11:49:51.450961 pypdf-4.1.0/pypdf/constants.py
--rw-r--r--   0        0        0     1632 2024-03-03 11:49:51.450961 pypdf-4.1.0/pypdf/errors.py
--rw-r--r--   0        0        0    30533 2024-03-03 11:49:51.450961 pypdf-4.1.0/pypdf/filters.py
--rw-r--r--   0        0        0    15097 2024-03-03 11:49:51.450961 pypdf-4.1.0/pypdf/generic/__init__.py
--rw-r--r--   0        0        0    24281 2024-03-03 11:49:51.450961 pypdf-4.1.0/pypdf/generic/_base.py
--rw-r--r--   0        0        0    55915 2024-03-03 11:49:51.450961 pypdf-4.1.0/pypdf/generic/_data_structures.py
--rw-r--r--   0        0        0     5427 2024-03-03 11:49:51.450961 pypdf-4.1.0/pypdf/generic/_fit.py
--rw-r--r--   0        0        0     1090 2024-03-03 11:49:51.450961 pypdf-4.1.0/pypdf/generic/_outline.py
--rw-r--r--   0        0        0     3808 2024-03-03 11:49:51.450961 pypdf-4.1.0/pypdf/generic/_rectangle.py
--rw-r--r--   0        0        0     6420 2024-03-03 11:49:51.450961 pypdf-4.1.0/pypdf/generic/_utils.py
--rw-r--r--   0        0        0     6327 2024-03-03 11:49:51.450961 pypdf-4.1.0/pypdf/generic/_viewerpref.py
--rw-r--r--   0        0        0     6880 2024-03-03 11:49:51.454961 pypdf-4.1.0/pypdf/pagerange.py
--rw-r--r--   0        0        0     1367 2024-03-03 11:49:51.454961 pypdf-4.1.0/pypdf/papersizes.py
--rw-r--r--   0        0        0        0 2024-03-03 11:49:51.454961 pypdf-4.1.0/pypdf/py.typed
--rw-r--r--   0        0        0     2085 2024-03-03 11:49:51.454961 pypdf-4.1.0/pypdf/types.py
--rw-r--r--   0        0        0    14192 2024-03-03 11:49:51.454961 pypdf-4.1.0/pypdf/xmp.py
--rw-r--r--   0        0        0     8953 2024-03-03 11:49:51.454961 pypdf-4.1.0/pyproject.toml
-drwxr-xr-x   0        0        0        0 2024-03-03 11:49:51.506961 pypdf-4.1.0/sample-files/
--rw-r--r--   0        0        0      156 2024-03-03 11:49:51.506961 pypdf-4.1.0/setup.cfg
--rw-r--r--   0        0        0     7407 1970-01-01 00:00:00.000000 pypdf-4.1.0/PKG-INFO
+-rw-r--r--   0        0        0      488 2023-06-30 15:52:13.172911 pypdf-4.2.0/.git-blame-ignore-revs
+-rw-r--r--   0        0        0      544 2024-04-07 14:19:40.262299 pypdf-4.2.0/.readthedocs.yaml
+-rw-r--r--   0        0        0    51243 2024-04-07 14:21:22.168216 pypdf-4.2.0/CHANGELOG.md
+-rw-r--r--   0        0        0      896 2024-04-03 20:23:02.489414 pypdf-4.2.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0     4607 2024-04-03 20:23:02.493413 pypdf-4.2.0/CONTRIBUTORS.md
+-rw-r--r--   0        0        0     1605 2023-06-30 15:52:13.172911 pypdf-4.2.0/LICENSE
+-rw-r--r--   0        0        0       34 2023-06-30 15:52:13.172911 pypdf-4.2.0/MANIFEST.in
+-rw-r--r--   0        0        0     4947 2024-04-03 20:23:02.493413 pypdf-4.2.0/README.md
+-rw-r--r--   0        0        0     1316 2024-04-07 14:19:40.266300 pypdf-4.2.0/pypdf/__init__.py
+-rw-r--r--   0        0        0    17997 2024-04-03 20:23:02.529412 pypdf-4.2.0/pypdf/_cmap.py
+-rw-r--r--   0        0        0     1674 2024-04-03 20:23:02.529412 pypdf-4.2.0/pypdf/_codecs/__init__.py
+-rw-r--r--   0        0        0   447237 2024-04-03 20:23:02.533412 pypdf-4.2.0/pypdf/_codecs/adobe_glyphs.py
+-rw-r--r--   0        0        0     4269 2024-04-03 20:23:02.533412 pypdf-4.2.0/pypdf/_codecs/pdfdoc.py
+-rw-r--r--   0        0        0     2630 2024-04-03 20:23:02.533412 pypdf-4.2.0/pypdf/_codecs/std.py
+-rw-r--r--   0        0        0     3734 2024-04-03 20:23:02.533412 pypdf-4.2.0/pypdf/_codecs/symbol.py
+-rw-r--r--   0        0        0     3742 2024-04-03 20:23:02.533412 pypdf-4.2.0/pypdf/_codecs/zapfding.py
+-rw-r--r--   0        0        0     3054 2024-04-03 20:23:02.533412 pypdf-4.2.0/pypdf/_crypt_providers/__init__.py
+-rw-r--r--   0        0        0     1711 2024-04-03 20:23:02.533412 pypdf-4.2.0/pypdf/_crypt_providers/_base.py
+-rw-r--r--   0        0        0     4329 2024-04-03 20:23:02.533412 pypdf-4.2.0/pypdf/_crypt_providers/_cryptography.py
+-rw-r--r--   0        0        0     3345 2024-04-03 20:23:02.533412 pypdf-4.2.0/pypdf/_crypt_providers/_fallback.py
+-rw-r--r--   0        0        0     3381 2024-04-03 20:23:02.533412 pypdf-4.2.0/pypdf/_crypt_providers/_pycryptodome.py
+-rw-r--r--   0        0        0    48730 2024-04-07 14:19:40.266300 pypdf-4.2.0/pypdf/_doc_common.py
+-rw-r--r--   0        0        0    48920 2024-04-03 20:23:02.533412 pypdf-4.2.0/pypdf/_encryption.py
+-rw-r--r--   0        0        0    24468 2024-04-07 14:19:40.266300 pypdf-4.2.0/pypdf/_merger.py
+-rw-r--r--   0        0        0    93557 2024-04-07 14:19:40.266300 pypdf-4.2.0/pypdf/_page.py
+-rw-r--r--   0        0        0     8326 2024-04-07 14:19:40.266300 pypdf-4.2.0/pypdf/_page_labels.py
+-rw-r--r--   0        0        0     2260 2024-04-07 14:19:40.266300 pypdf-4.2.0/pypdf/_protocols.py
+-rw-r--r--   0        0        0    45843 2024-04-07 14:19:40.266300 pypdf-4.2.0/pypdf/_reader.py
+-rw-r--r--   0        0        0    10373 2024-04-03 20:23:02.537412 pypdf-4.2.0/pypdf/_text_extraction/__init__.py
+-rw-r--r--   0        0        0      338 2024-04-03 20:23:02.537412 pypdf-4.2.0/pypdf/_text_extraction/_layout_mode/__init__.py
+-rw-r--r--   0        0        0    14782 2024-04-03 20:23:02.537412 pypdf-4.2.0/pypdf/_text_extraction/_layout_mode/_fixed_width_page.py
+-rw-r--r--   0        0        0     5099 2024-04-03 20:23:02.537412 pypdf-4.2.0/pypdf/_text_extraction/_layout_mode/_font.py
+-rw-r--r--   0        0        0     4264 2024-04-03 20:23:02.537412 pypdf-4.2.0/pypdf/_text_extraction/_layout_mode/_font_widths.py
+-rw-r--r--   0        0        0     8012 2024-04-07 14:19:40.266300 pypdf-4.2.0/pypdf/_text_extraction/_layout_mode/_text_state_manager.py
+-rw-r--r--   0        0        0     5316 2024-04-03 20:23:02.537412 pypdf-4.2.0/pypdf/_text_extraction/_layout_mode/_text_state_params.py
+-rw-r--r--   0        0        0    20078 2024-04-07 14:19:40.266300 pypdf-4.2.0/pypdf/_utils.py
+-rw-r--r--   0        0        0       22 2024-04-07 14:19:58.318639 pypdf-4.2.0/pypdf/_version.py
+-rw-r--r--   0        0        0   114540 2024-04-07 14:19:40.270300 pypdf-4.2.0/pypdf/_writer.py
+-rw-r--r--   0        0        0    10923 2024-04-07 14:19:40.270300 pypdf-4.2.0/pypdf/_xobj_image_helpers.py
+-rw-r--r--   0        0        0     1118 2024-04-03 20:23:02.541412 pypdf-4.2.0/pypdf/annotations/__init__.py
+-rw-r--r--   0        0        0      910 2024-04-03 20:23:02.541412 pypdf-4.2.0/pypdf/annotations/_base.py
+-rw-r--r--   0        0        0    11608 2024-04-03 20:23:02.541412 pypdf-4.2.0/pypdf/annotations/_markup_annotations.py
+-rw-r--r--   0        0        0     1278 2024-04-03 20:23:02.541412 pypdf-4.2.0/pypdf/annotations/_non_markup_annotations.py
+-rw-r--r--   0        0        0    21006 2024-04-07 14:19:40.270300 pypdf-4.2.0/pypdf/constants.py
+-rw-r--r--   0        0        0     1632 2024-04-03 20:23:02.541412 pypdf-4.2.0/pypdf/errors.py
+-rw-r--r--   0        0        0    30896 2024-04-07 14:19:40.270300 pypdf-4.2.0/pypdf/filters.py
+-rw-r--r--   0        0        0    15097 2024-04-07 14:19:40.270300 pypdf-4.2.0/pypdf/generic/__init__.py
+-rw-r--r--   0        0        0    24567 2024-04-07 14:19:40.270300 pypdf-4.2.0/pypdf/generic/_base.py
+-rw-r--r--   0        0        0    58626 2024-04-07 14:19:40.270300 pypdf-4.2.0/pypdf/generic/_data_structures.py
+-rw-r--r--   0        0        0     5427 2024-04-03 20:23:02.541412 pypdf-4.2.0/pypdf/generic/_fit.py
+-rw-r--r--   0        0        0     1090 2024-04-03 20:23:02.545412 pypdf-4.2.0/pypdf/generic/_outline.py
+-rw-r--r--   0        0        0     3808 2024-04-03 20:23:02.545412 pypdf-4.2.0/pypdf/generic/_rectangle.py
+-rw-r--r--   0        0        0     6420 2024-04-03 20:23:02.545412 pypdf-4.2.0/pypdf/generic/_utils.py
+-rw-r--r--   0        0        0     6642 2024-04-03 20:23:02.545412 pypdf-4.2.0/pypdf/generic/_viewerpref.py
+-rw-r--r--   0        0        0     6880 2024-04-03 20:23:02.545412 pypdf-4.2.0/pypdf/pagerange.py
+-rw-r--r--   0        0        0     1367 2024-04-03 20:23:02.545412 pypdf-4.2.0/pypdf/papersizes.py
+-rw-r--r--   0        0        0        0 2024-04-03 20:23:02.545412 pypdf-4.2.0/pypdf/py.typed
+-rw-r--r--   0        0        0     2085 2024-04-03 20:23:02.545412 pypdf-4.2.0/pypdf/types.py
+-rw-r--r--   0        0        0    14192 2024-04-03 20:23:02.545412 pypdf-4.2.0/pypdf/xmp.py
+-rw-r--r--   0        0        0     8949 2024-04-03 20:23:02.545412 pypdf-4.2.0/pyproject.toml
+-rw-r--r--   0        0        0      156 2024-04-03 20:23:02.557412 pypdf-4.2.0/setup.cfg
+-rw-r--r--   0        0        0     7403 1970-01-01 00:00:00.000000 pypdf-4.2.0/PKG-INFO
```

### Comparing `pypdf-4.1.0/CHANGELOG.md` & `pypdf-4.2.0/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,66 @@
 # CHANGELOG
 
+## Version 4.2.0, 2024-04-07
+
+### New Features (ENH)
+- Allow multiple charsets for NameObject.read_from_stream (#2585)
+- Add support for /Kids in page labels (#2562)
+- Allow to update fields on many pages (#2571)
+- Tolerate PDF with invalid xref pointed objects (#2335)
+- Add Enforce from PDF2.0 in viewer_preferences (#2511)
+- Add += and -= operators to ArrayObject (#2510)
+
+### Bug Fixes (BUG)
+- Fix merge_page sometimes generating unknown operator 'QQ' (#2588)
+- Fix fields update where annotations are kids of field (#2570)
+- Process CMYK images without a filter correctly (#2557)
+- Extract text in layout mode without finding resources (#2555)
+- Prevent recursive loop in some PDF files (#2505)
+
+### Robustness (ROB)
+- Tolerate "truncated" xref (#2580)
+- Replace error by warning for EOD in RunLengthDecode/ASCIIHexDecode (#2334)
+- Rebuild xref table if one entry is invalid (#2528)
+- Robustify stream extraction (#2526)
+
+### Documentation (DOC)
+- Update release process for latest changes (#2564)
+- Encryption/decryption: Clone document instead of copying all pages (#2546)
+- Minor improvements (#2542)
+- Update annotation list (#2534)
+- Update references and formatting (#2529)
+- Correct threads reference, plus minor changes (#2521)
+- Minor readability increases (#2515)
+- Simplify PaperSize examples (#2504)
+- Minor improvements (#2501)
+
+### Developer Experience (DEV)
+- Remove unused dependencies (#2572)
+- Remove page labels PR link from message (#2561)
+- Fix changelog generator regarding whitespace and handling of "Other" group (#2492)
+- Add REL to known PR prefixes (#2554)
+- Release using the REL commit instead of git tag (#2500)
+- Unify code between PdfReader and PdfWriter (#2497)
+- Bump softprops/action-gh-release from 1 to 2 (#2514)
+
+### Maintenance (MAINT)
+- Ressources → Resources (and internal name childs) (#2550)
+- Fix typos found by codespell (#2549)
+- Update Read the Docs configuration (#2538)
+- Add root_object, _info and _ID to PdfReader (#2495)
+
+### Testing (TST)
+- Allow loading truncated images if required (#2586)
+- Fix download issues from #2562 (#2578)
+- Improve test_get_contents_from_nullobject to show real use-case (#2524)
+- Add missing test annotations (#2507)
+
+[Full Changelog](https://github.com/py-pdf/pypdf/compare/4.1.0...4.2.0)
+
 ## Version 4.1.0, 2024-03-03
 
 Generating name objects (`NameObject`) without a leading slash
 is considered deprecated now. Previously, just a plain warning
 would be logged, leading to possibly invalid PDF files. According
 to our deprecation policy, this will log a *DeprecationWarning*
 for now.
@@ -239,15 +296,15 @@
 
 ## Version 3.15.2, 2023-08-20
 
 ### Security (SEC)
 -  Avoid endless recursion of reading damaged PDF file (#2093)
 
 ### Performance Improvements (PI)
--  Re-use content stream (#2101)
+-  Reuse content stream (#2101)
 
 ### Maintenance (MAINT)
 -  Make ParseError inherit from PyPdfError (#2097)
 
 [Full Changelog](https://github.com/py-pdf/pypdf/compare/3.15.1...3.15.2)
 
 ## Version 3.15.1, 2023-08-13
@@ -407,15 +464,15 @@
 
 [Full Changelog](https://github.com/py-pdf/pypdf/compare/3.9.0...3.9.1)
 
 ## Version 3.9.0, 2023-05-21
 
 ### New Features (ENH)
 -  Simplify metadata input (Document Information Dictionary) (#1851)
--  Extend cmap compatibilty to GBK_EUC_H/V (#1812)
+-  Extend cmap compatibility to GBK_EUC_H/V (#1812)
 
 ### Bug Fixes (BUG)
 -  Prevent infinite loop when no character follows after a comment (#1828)
 -  get_contents does not return ContentStream (#1847)
 -  Accept XYZ destination with zoom missing (default to zoom=0.0) (#1844)
 -  Cope with 1 Bit images (#1815)
 
@@ -428,15 +485,15 @@
 -  Clarify that PyPDF2 is dead (#1827)
 -  Add Hunter King as Contributor for #1806
 
 ### Maintenance (MAINT)
 -  Refactor internal Encryption class (#1821)
 -  Add R parameter to generate_values (#1820)
 -  Make encryption_key parameter of write_to_stream optional (#1819)
--  Prepare for adding AES enryption support (#1818)
+-  Prepare for adding AES encryption support (#1818)
 
 [Full Changelog](https://github.com/py-pdf/pypdf/compare/3.8.1...3.9.0)
 
 
 ## Version 3.8.1, 2023-04-23
 
 ### Bug Fixes (BUG)
@@ -661,15 +718,15 @@
 
 ### Developer Experience (DEV)
 -  Update docs config (#1535)
 
 ## Version 3.2.0, 2022-12-31
 
 ### Performance Improvement (PI)
--  Help the specializing adpative interpreter (#1522)
+-  Help the specializing adaptive interpreter (#1522)
 
 ### New Features (ENH)
 -  Add support for page labels (#1519)
 
 ### Bug Fixes (BUG)
 -  upgrade clone_document_root (#1520)
 
@@ -995,20 +1052,20 @@
 
 ### Bug Fixes (BUG)
 -  Named Dest in PDF1.1 (#1174)
 -  Incomplete Graphic State save/restore (#1172)
 
 ### Documentation (DOC)
 -  Update changelog url in package metadata (#1180)
--  Mantion camelot for table extraction (#1179)
+-  Mention camelot for table extraction (#1179)
 -  Mention pyHanko for signing PDF documents (#1178)
 -  Weow have CMAP support since a while (#1177)
 
 ### Maintenance (MAINT)
--  Consistant usage of warnings / log messages (#1164)
+-  Consistent usage of warnings / log messages (#1164)
 -  Consistent terminology for outline items (#1156)
 
 
 [Full Changelog](https://github.com/py-pdf/PyPDF2/compare/2.8.1...2.9.0)
 
 ## Version 2.8.1, 2022-07-25
 
@@ -1078,15 +1135,15 @@
 -  Fix type in signature of PdfWriter.add_uri (#1131)
 
 ### Developer Experience (DEV)
 -  Add .git-blame-ignore-revs (#1141)
 
 ### Code Style (STY)
 -  Fixing typos (#1137)
--  Re-use code via get_outlines_property in tests (#1130)
+-  Reuse code via get_outlines_property in tests (#1130)
 
 [Full Changelog](https://github.com/py-pdf/PyPDF2/compare/2.6.0...2.7.0)
 
 ## Version 2.6.0, 2022-07-17
 
 ### New Features (ENH)
 -  Add color and font_format to PdfReader.outlines[i] (#1104)
@@ -1242,15 +1299,15 @@
 -  Adjust string formatting to be able to use mutmut (#1020)
 -  Update Bug report template
 
 [Full Changelog](https://github.com/py-pdf/PyPDF2/compare/2.3.1...2.4.0)
 
 ## Version 2.3.1, 2022-06-19
 
-BUG: Forgot to add the interal `_codecs` subpackage.
+BUG: Forgot to add the internal `_codecs` subpackage.
 
 [Full Changelog](https://github.com/py-pdf/PyPDF2/compare/2.3.0...2.3.1)
 
 ## Version 2.3.0, 2022-06-19
 
 The highlight of this release is improved support for file encryption
 (AES-128 and AES-256, R5 only). See #749 for the amazing work of
@@ -1281,15 +1338,15 @@
 ### New Features (ENH)
 -  Add decrypt support for V5 and AES-128, AES-256 (R5 only) (#749)
 
 ### Robustness (ROB)
 -  Fix corrupted (wrongly) linear PDF (#1008)
 
 ### Maintenance (MAINT)
--  Move PDF_Samples folder into ressources
+-  Move PDF_Samples folder into resources
 -  Fix typos (#1007)
 
 ### Testing (TST)
 -  Improve encryption/decryption test (#1009)
 -  Add merger test cases with real PDFs (#1006)
 -  Add mutmut config
```

### Comparing `pypdf-4.1.0/CONTRIBUTING.md` & `pypdf-4.2.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pypdf-4.1.0/CONTRIBUTORS.md` & `pypdf-4.2.0/CONTRIBUTORS.md`

 * *Files identical despite different names*

### Comparing `pypdf-4.1.0/LICENSE` & `pypdf-4.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pypdf-4.1.0/README.md` & `pypdf-4.2.0/README.md`

 * *Files identical despite different names*

### Comparing `pypdf-4.1.0/pypdf/__init__.py` & `pypdf-4.2.0/pypdf/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,18 +4,19 @@
 custom data, viewing options, and passwords to PDF files. pypdf can retrieve
 text and metadata from PDFs as well.
 
 You can read the full docs at https://pypdf.readthedocs.io/.
 """
 
 from ._crypt_providers import crypt_provider
+from ._doc_common import DocumentInformation
 from ._encryption import PasswordType
 from ._merger import PdfMerger
 from ._page import PageObject, Transformation, mult
-from ._reader import DocumentInformation, PdfReader
+from ._reader import PdfReader
 from ._version import __version__
 from ._writer import ObjectDeletionFlag, PdfWriter
 from .constants import ImageType
 from .pagerange import PageRange, parse_filename_page_ranges
 from .papersizes import PaperSize
 
 try:
```

### Comparing `pypdf-4.1.0/pypdf/_cmap.py` & `pypdf-4.2.0/pypdf/_cmap.py`

 * *Files identical despite different names*

### Comparing `pypdf-4.1.0/pypdf/_codecs/__init__.py` & `pypdf-4.2.0/pypdf/_codecs/__init__.py`

 * *Files identical despite different names*

### Comparing `pypdf-4.1.0/pypdf/_codecs/adobe_glyphs.py` & `pypdf-4.2.0/pypdf/_codecs/adobe_glyphs.py`

 * *Files identical despite different names*

### Comparing `pypdf-4.1.0/pypdf/_codecs/pdfdoc.py` & `pypdf-4.2.0/pypdf/_codecs/pdfdoc.py`

 * *Files identical despite different names*

### Comparing `pypdf-4.1.0/pypdf/_codecs/std.py` & `pypdf-4.2.0/pypdf/_codecs/std.py`

 * *Files identical despite different names*

### Comparing `pypdf-4.1.0/pypdf/_codecs/symbol.py` & `pypdf-4.2.0/pypdf/_codecs/symbol.py`

 * *Files identical despite different names*

### Comparing `pypdf-4.1.0/pypdf/_codecs/zapfding.py` & `pypdf-4.2.0/pypdf/_codecs/zapfding.py`

 * *Files identical despite different names*

### Comparing `pypdf-4.1.0/pypdf/_crypt_providers/__init__.py` & `pypdf-4.2.0/pypdf/_crypt_providers/__init__.py`

 * *Files identical despite different names*

### Comparing `pypdf-4.1.0/pypdf/_crypt_providers/_base.py` & `pypdf-4.2.0/pypdf/_crypt_providers/_base.py`

 * *Files identical despite different names*

### Comparing `pypdf-4.1.0/pypdf/_crypt_providers/_cryptography.py` & `pypdf-4.2.0/pypdf/_crypt_providers/_cryptography.py`

 * *Files identical despite different names*

### Comparing `pypdf-4.1.0/pypdf/_crypt_providers/_fallback.py` & `pypdf-4.2.0/pypdf/_crypt_providers/_fallback.py`

 * *Files identical despite different names*

### Comparing `pypdf-4.1.0/pypdf/_crypt_providers/_pycryptodome.py` & `pypdf-4.2.0/pypdf/_crypt_providers/_pycryptodome.py`

 * *Files identical despite different names*

### Comparing `pypdf-4.1.0/pypdf/_encryption.py` & `pypdf-4.2.0/pypdf/_encryption.py`

 * *Files identical despite different names*

### Comparing `pypdf-4.1.0/pypdf/_merger.py` & `pypdf-4.2.0/pypdf/_merger.py`

 * *Files 0% similar despite different names*

```diff
@@ -302,16 +302,16 @@
 
         if my_file:
             ret_fileobj.close()
 
     def close(self) -> None:
         """Shut all file descriptors (input and output) and clear all memory usage."""
         self.pages = []
-        for fo, _reader in self.inputs:
-            fo.close()
+        for file_descriptor, _reader in self.inputs:
+            file_descriptor.close()
 
         self.inputs = []
         self.output = None
 
     def add_metadata(self, infos: Dict[str, Any]) -> None:
         """
         Add custom metadata to the output.
```

### Comparing `pypdf-4.1.0/pypdf/_page.py` & `pypdf-4.2.0/pypdf/_page.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     Tuple,
     Union,
     cast,
     overload,
 )
 
 from ._cmap import build_char_map, unknown_char_map
-from ._protocols import PdfReaderProtocol, PdfWriterProtocol
+from ._protocols import PdfCommonDocProtocol
 from ._text_extraction import (
     OrientationNotFoundError,
     _layout_mode,
     crlf_space_check,
     handle_tj,
     mult,
 )
@@ -65,15 +65,15 @@
     TransformationMatrixType,
     logger_warning,
     matrix_multiply,
 )
 from .constants import AnnotationDictionaryAttributes as ADA
 from .constants import ImageAttributes as IA
 from .constants import PageAttributes as PG
-from .constants import Ressources as RES
+from .constants import Resources as RES
 from .errors import PageSizeNotDefinedError, PdfReadError
 from .filters import _xobj_to_image
 from .generic import (
     ArrayObject,
     ContentStream,
     DictionaryObject,
     EncodedStreamObject,
@@ -324,19 +324,19 @@
             this object in its source PDF
     """
 
     original_page: "PageObject"  # very local use in writer when appending
 
     def __init__(
         self,
-        pdf: Union[None, PdfReaderProtocol, PdfWriterProtocol] = None,
+        pdf: Optional[PdfCommonDocProtocol] = None,
         indirect_reference: Optional[IndirectObject] = None,
     ) -> None:
         DictionaryObject.__init__(self)
-        self.pdf: Union[None, PdfReaderProtocol, PdfWriterProtocol] = pdf
+        self.pdf = pdf
         self.inline_images: Optional[Dict[str, ImageFile]] = None
         # below Union for mypy but actually Optional[List[str]]
         self.inline_images_keys: Optional[List[Union[str, List[str]]]] = None
         self.indirect_reference = indirect_reference
 
     def hash_value_data(self) -> bytes:
         data = super().hash_value_data()
@@ -352,15 +352,15 @@
         space unit is 1/72 inch, and a value of 3 means that a user
         space unit is 3/72 inch.
         """
         return self.get(PG.USER_UNIT, 1)
 
     @staticmethod
     def create_blank_page(
-        pdf: Union[None, PdfReaderProtocol, PdfWriterProtocol] = None,
+        pdf: Optional[PdfCommonDocProtocol] = None,
         width: Union[float, Decimal, None] = None,
         height: Union[float, Decimal, None] = None,
     ) -> "PageObject":
         """
         Return a new blank page.
 
         If ``width`` or ``height`` is ``None``, try to get the page size
@@ -793,15 +793,15 @@
                 new_res[el[0]] = el[1]
         return new_res, rename_res
 
     @staticmethod
     def _content_stream_rename(
         stream: ContentStream,
         rename: Dict[Any, Any],
-        pdf: Union[None, PdfReaderProtocol, PdfWriterProtocol],
+        pdf: Optional[PdfCommonDocProtocol],
     ) -> ContentStream:
         if not rename:
             return stream
         stream = ContentStream(stream, pdf)
         for operands, _operator in stream.operations:
             if isinstance(operands, list):
                 for i, op in enumerate(operands):
@@ -814,15 +814,15 @@
             else:
                 raise KeyError(f"type of operands is {type(operands)}")
         return stream
 
     @staticmethod
     def _add_transformation_matrix(
         contents: Any,
-        pdf: Union[None, PdfReaderProtocol, PdfWriterProtocol],
+        pdf: Optional[PdfCommonDocProtocol],
         ctm: CompressedTransformationMatrix,
     ) -> ContentStream:
         """Add transformation matrix at the beginning of the given contents stream."""
         a, b, c, d, e, f = ctm
         contents = ContentStream(contents, pdf)
         contents.operations.insert(
             0,
@@ -920,15 +920,15 @@
                 # applies at least for page not in writer
                 # as a backup solution, we put content as an object although not in accordance with pdf ref
                 # this will be fixed with the _add_object
                 self[NameObject(PG.CONTENTS)] = content
         else:
             content.indirect_reference = self[
                 PG.CONTENTS
-            ].indirect_reference  # TODO: in a future may required generation managment
+            ].indirect_reference  # TODO: in a future may required generation management
             try:
                 self.indirect_reference.pdf._objects[
                     content.indirect_reference.idnum - 1  # type: ignore
                 ] = content
             except AttributeError:
                 # applies at least for page not in writer
                 # as a backup solution, we put content as an object although not in accordance with pdf ref
@@ -1578,15 +1578,15 @@
         ] = {}
         try:
             objr = obj
             while NameObject(PG.RESOURCES) not in objr:
                 # /Resources can be inherited sometimes so we look to parents
                 objr = objr["/Parent"].get_object()
                 # if no parents we will have no /Resources will be available
-                # => an exception wil be raised
+                # => an exception will be raised
             resources_dict = cast(DictionaryObject, objr[PG.RESOURCES])
         except Exception:
             # no resources means no text is possible (no font) we consider the
             # file as not damaged, no need to check for TJ or Tj
             return ""
         if "/Font" in resources_dict:
             for f in cast(DictionaryObject, resources_dict["/Font"]):
@@ -1887,36 +1887,38 @@
         Get fonts formatted for "layout" mode text extraction.
 
         Returns:
             Dict[str, Font]: dictionary of _layout_mode.Font instances keyed by font name
         """
         # Font retrieval logic adapted from pypdf.PageObject._extract_text()
         objr: Any = self
-        while NameObject(PG.RESOURCES) not in objr:
-            objr = objr["/Parent"].get_object()
-        resources_dict: Any = objr[PG.RESOURCES]
         fonts: Dict[str, _layout_mode.Font] = {}
-        if "/Font" in resources_dict and self.pdf is not None:
-            for font_name in resources_dict["/Font"]:
-                *cmap, font_dict_obj = build_char_map(font_name, 200.0, self)
-                font_dict = {
-                    k: self.pdf.get_object(v)
-                    if isinstance(v, IndirectObject)
-                    else [
-                        self.pdf.get_object(_v)
-                        if isinstance(_v, IndirectObject)
-                        else _v
-                        for _v in v
-                    ]
-                    if isinstance(v, ArrayObject)
-                    else v
-                    for k, v in font_dict_obj.items()
-                }
-                # mypy really sucks at unpacking
-                fonts[font_name] = _layout_mode.Font(*cmap, font_dict)  # type: ignore[call-arg,arg-type]
+        while objr is not None:
+            try:
+                resources_dict: Any = objr[PG.RESOURCES]
+            except KeyError:
+                resources_dict = {}
+            if "/Font" in resources_dict and self.pdf is not None:
+                for font_name in resources_dict["/Font"]:
+                    *cmap, font_dict_obj = build_char_map(font_name, 200.0, self)
+                    font_dict = {
+                        k: v.get_object()
+                        if isinstance(v, IndirectObject)
+                        else [_v.get_object() for _v in v]
+                        if isinstance(v, ArrayObject)
+                        else v
+                        for k, v in font_dict_obj.items()
+                    }
+                    # mypy really sucks at unpacking
+                    fonts[font_name] = _layout_mode.Font(*cmap, font_dict)  # type: ignore[call-arg,arg-type]
+            try:
+                objr = objr["/Parent"].get_object()
+            except KeyError:
+                objr = None
+
         return fonts
 
     def _layout_mode_text(
         self,
         space_vertically: bool = True,
         scale_weight: float = 1.25,
         strip_rotated: bool = True,
@@ -2233,15 +2235,15 @@
     def __delitem__(self, index: Union[int, slice]) -> None:
         if isinstance(index, slice):
             r = list(range(*index.indices(len(self))))
             # pages have to be deleted from last to first
             r.sort()
             r.reverse()
             for p in r:
-                del self[p]
+                del self[p]  # recursive call
             return
         if not isinstance(index, int):
             raise TypeError("index must be integers")
         len_self = len(self)
         if index < 0:
             # support negative indexes
             index = len_self + index
@@ -2254,15 +2256,15 @@
             parent = cast(DictionaryObject, parent.get_object())
             try:
                 i = parent["/Kids"].index(ind)
                 del parent["/Kids"][i]
                 try:
                     assert ind is not None
                     del ind.pdf.flattened_pages[index]  # case of page in a Reader
-                except AttributeError:
+                except Exception:  # pragma: no cover
                     pass
                 if "/Count" in parent:
                     parent[NameObject("/Count")] = NumberObject(parent["/Count"] - 1)
                 if len(parent["/Kids"]) == 0:
                     # No more objects in this part of this sub tree
                     ind = parent.indirect_reference
                     parent = cast(DictionaryObject, parent.get("/Parent", None))
```

### Comparing `pypdf-4.1.0/pypdf/_page_labels.py` & `pypdf-4.2.0/pypdf/_page_labels.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,20 +7,20 @@
 
 However, the title page and the table of contents might have roman numerals as
 page label. This makes things more complicated.
 
 Example 1
 ---------
 
->>> reader.trailer["/Root"]["/PageLabels"]["/Nums"]
+>>> reader.root_object["/PageLabels"]["/Nums"]
 [0, IndirectObject(18, 0, 139929798197504),
  8, IndirectObject(19, 0, 139929798197504)]
->>> reader.get_object(reader.trailer["/Root"]["/PageLabels"]["/Nums"][1])
+>>> reader.get_object(reader.root_object["/PageLabels"]["/Nums"][1])
 {'/S': '/r'}
->>> reader.get_object(reader.trailer["/Root"]["/PageLabels"]["/Nums"][3])
+>>> reader.get_object(reader.root_object["/PageLabels"]["/Nums"][3])
 {'/S': '/D'}
 
 Example 2
 ---------
 The following example shows a document with pages labeled
 i, ii, iii, iv, 1, 2, 3, A-8, A-9, ...
 
@@ -53,19 +53,19 @@
 r       Lowercase roman numerals
 A       Uppercase letters (A to Z for the first 26 pages,
                            AA to ZZ for the next 26, and so on)
 a       Lowercase letters (a to z for the first 26 pages,
                            aa to zz for the next 26, and so on)
 """
 
-from typing import Iterator, Optional, Tuple
+from typing import Iterator, List, Optional, Tuple, cast
 
-from ._protocols import PdfReaderProtocol
+from ._protocols import PdfCommonDocProtocol
 from ._utils import logger_warning
-from .generic import ArrayObject, DictionaryObject, NumberObject
+from .generic import ArrayObject, DictionaryObject, NullObject, NumberObject
 
 
 def number2uppercase_roman_numeral(num: int) -> str:
     roman = [
         (1000, "M"),
         (900, "CM"),
         (500, "D"),
@@ -112,74 +112,97 @@
     return rep
 
 
 def number2lowercase_letter(number: int) -> str:
     return number2uppercase_letter(number).lower()
 
 
-def index2label(reader: PdfReaderProtocol, index: int) -> str:
+def get_label_from_nums(dictionary_object: DictionaryObject, index: int) -> str:
+    # [Nums] shall be an array of the form
+    #   [ key 1 value 1 key 2 value 2 ... key n value n ]
+    # where each key_i is an integer and the corresponding
+    # value_i shall be the object associated with that key.
+    # The keys shall be sorted in numerical order,
+    # analogously to the arrangement of keys in a name tree
+    # as described in 7.9.6, "Name Trees."
+    nums = cast(ArrayObject, dictionary_object["/Nums"])
+    i = 0
+    value = None
+    start_index = 0
+    while i < len(nums):
+        start_index = nums[i]
+        value = nums[i + 1].get_object()
+        if i + 2 == len(nums):
+            break
+        if nums[i + 2] > index:
+            break
+        i += 2
+    m = {
+        None: lambda n: "",
+        "/D": lambda n: str(n),
+        "/R": number2uppercase_roman_numeral,
+        "/r": number2lowercase_roman_numeral,
+        "/A": number2uppercase_letter,
+        "/a": number2lowercase_letter,
+    }
+    # if /Nums array is not following the specification or if /Nums is empty
+    if not isinstance(value, dict):
+        return str(index + 1)  # Fallback
+    start = value.get("/St", 1)
+    prefix = value.get("/P", "")
+    return prefix + m[value.get("/S")](index - start_index + start)
+
+
+def index2label(reader: PdfCommonDocProtocol, index: int) -> str:
     """
     See 7.9.7 "Number Trees".
 
     Args:
         reader: The PdfReader
         index: The index of the page
 
     Returns:
         The label of the page, e.g. "iv" or "4".
     """
-    root = reader.trailer["/Root"]
+    root = cast(DictionaryObject, reader.root_object)
     if "/PageLabels" not in root:
         return str(index + 1)  # Fallback
-    number_tree = root["/PageLabels"]
+    number_tree = cast(DictionaryObject, root["/PageLabels"].get_object())
     if "/Nums" in number_tree:
-        # [Nums] shall be an array of the form
-        #   [ key 1 value 1 key 2 value 2 ... key n value n ]
-        # where each key_i is an integer and the corresponding
-        # value_i shall be the object associated with that key.
-        # The keys shall be sorted in numerical order,
-        # analogously to the arrangement of keys in a name tree
-        # as described in 7.9.6, "Name Trees."
-        nums = number_tree["/Nums"]
-        i = 0
-        value = None
-        start_index = 0
-        while i < len(nums):
-            start_index = nums[i]
-            value = nums[i + 1].get_object()
-            if i + 2 == len(nums):
+        return get_label_from_nums(number_tree, index)
+    if "/Kids" in number_tree and not isinstance(number_tree["/Kids"], NullObject):
+        # number_tree = {'/Kids': [IndirectObject(7333, 0, 140132998195856), ...]}
+        # Limit maximum depth.
+        level = 0
+        while level < 100:
+            kids = cast(List[DictionaryObject], number_tree["/Kids"])
+            for kid in kids:
+                # kid = {'/Limits': [0, 63], '/Nums': [0, {'/P': 'C1'}, ...]}
+                limits = cast(List[int], kid["/Limits"])
+                if limits[0] <= index <= limits[1]:
+                    if kid.get("/Kids", None) is not None:
+                        # Recursive definition.
+                        level += 1
+                        if level == 100:  # pragma: no cover
+                            raise NotImplementedError("Too deep nesting is not supported.")
+                        number_tree = kid
+                        # Exit the inner `for` loop and continue at the next level with the
+                        # next iteration of the `while` loop.
+                        break
+                    return get_label_from_nums(kid, index)
+            else:
+                # When there are no kids, make sure to exit the `while` loop directly
+                # and continue with the fallback.
                 break
-            if nums[i + 2] > index:
-                break
-            i += 2
-        m = {
-            None: lambda n: "",
-            "/D": lambda n: str(n),
-            "/R": number2uppercase_roman_numeral,
-            "/r": number2lowercase_roman_numeral,
-            "/A": number2uppercase_letter,
-            "/a": number2lowercase_letter,
-        }
-        # if /Nums array is not following the specification or if /Nums is empty
-        if not isinstance(value, dict):
-            return str(index + 1)  # Fallback
-        start = value.get("/St", 1)
-        prefix = value.get("/P", "")
-        return prefix + m[value.get("/S")](index - start_index + start)
-    if "/Kids" in number_tree or "/Limits" in number_tree:
-        logger_warning(
-            (
-                "/Kids or /Limits found in PageLabels. "
-                "Please share this PDF with pypdf: "
-                "https://github.com/py-pdf/pypdf/pull/1519"
-            ),
-            __name__,
-        )
-    # TODO: Implement /Kids and /Limits for number tree
-    return str(index + 1)  # Fallback if /Nums is not in the number_tree
+
+    logger_warning(
+        f"Could not reliably determine page label for {index}.",
+        __name__
+    )
+    return str(index + 1)  # Fallback if neither /Nums nor /Kids is in the number_tree
 
 
 def nums_insert(
     key: NumberObject,
     value: DictionaryObject,
     nums: ArrayObject,
 ) -> None:
```

### Comparing `pypdf-4.1.0/pypdf/_reader.py` & `pypdf-4.2.0/pypdf/_writer.py`

 * *Files 25% similar despite different names*

```diff
@@ -23,346 +23,283 @@
 # CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
 # SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
 # INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
 # CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
 # ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
 # POSSIBILITY OF SUCH DAMAGE.
 
-import os
+import codecs
+import collections
+import decimal
+import enum
+import hashlib
 import re
-import struct
-import zlib
-from datetime import datetime
-from io import BytesIO, UnsupportedOperation
+import uuid
+from io import BytesIO, FileIO, IOBase
 from pathlib import Path
+from types import TracebackType
 from typing import (
+    IO,
     Any,
     Callable,
+    Deque,
     Dict,
     Iterable,
-    Iterator,
     List,
-    Mapping,
     Optional,
+    Pattern,
     Tuple,
+    Type,
     Union,
     cast,
 )
 
-from ._encryption import Encryption, PasswordType
-from ._page import PageObject, _VirtualList
-from ._page_labels import index2label as page_index2page_label
+from ._cmap import build_char_map_from_dict
+from ._doc_common import PdfDocCommon
+from ._encryption import EncryptAlgorithm, Encryption
+from ._page import PageObject
+from ._page_labels import nums_clear_range, nums_insert, nums_next
+from ._reader import PdfReader
 from ._utils import (
     StrByteType,
     StreamType,
+    _get_max_pdf_version_header,
     b_,
-    deprecate_with_replacement,
     logger_warning,
-    parse_iso8824_date,
-    read_non_whitespace,
-    read_previous_line,
-    read_until_whitespace,
-    skip_over_comment,
-    skip_over_whitespace,
 )
+from .constants import AnnotationDictionaryAttributes as AA
 from .constants import CatalogAttributes as CA
-from .constants import CatalogDictionary as CD
 from .constants import (
-    CheckboxRadioButtonAttributes,
+    CatalogDictionary,
+    FieldFlag,
+    FileSpecificationDictionaryEntries,
     GoToActionArguments,
+    ImageType,
+    InteractiveFormDictEntries,
+    PageLabelStyle,
+    TypFitArguments,
     UserAccessPermissions,
 )
+from .constants import CatalogDictionary as CD
 from .constants import Core as CO
-from .constants import DocumentInformationAttributes as DI
-from .constants import FieldDictionaryAttributes as FA
+from .constants import (
+    FieldDictionaryAttributes as FA,
+)
 from .constants import PageAttributes as PG
 from .constants import PagesAttributes as PA
 from .constants import TrailerKeys as TK
-from .errors import (
-    EmptyFileError,
-    FileNotDecryptedError,
-    PdfReadError,
-    PdfStreamError,
-    WrongPasswordError,
-)
+from .errors import PyPdfError
 from .generic import (
+    PAGE_FIT,
     ArrayObject,
     BooleanObject,
+    ByteStringObject,
     ContentStream,
     DecodedStreamObject,
     Destination,
     DictionaryObject,
-    EncodedStreamObject,
-    Field,
     Fit,
     FloatObject,
     IndirectObject,
     NameObject,
     NullObject,
     NumberObject,
     PdfObject,
+    RectangleObject,
+    StreamObject,
     TextStringObject,
     TreeObject,
     ViewerPreferences,
-    read_object,
+    create_string_object,
+    hex_to_rgb,
+)
+from .pagerange import PageRange, PageRangeSpec
+from .types import (
+    AnnotationSubtype,
+    BorderArrayType,
+    LayoutType,
+    OutlineItemType,
+    OutlineType,
+    PagemodeType,
 )
-from .types import OutlineType, PagemodeType
 from .xmp import XmpInformation
 
+OPTIONAL_READ_WRITE_FIELD = FieldFlag(0)
+ALL_DOCUMENT_PERMISSIONS = UserAccessPermissions.all()
 
-def convert_to_int(d: bytes, size: int) -> Union[int, Tuple[Any, ...]]:
-    if size > 8:
-        raise PdfReadError("invalid size in convert_to_int")
-    d = b"\x00\x00\x00\x00\x00\x00\x00\x00" + d
-    d = d[-8:]
-    return struct.unpack(">q", d)[0]
 
+class ObjectDeletionFlag(enum.IntFlag):
+    NONE = 0
+    TEXT = enum.auto()
+    LINKS = enum.auto()
+    ATTACHMENTS = enum.auto()
+    OBJECTS_3D = enum.auto()
+    ALL_ANNOTATIONS = enum.auto()
+    XOBJECT_IMAGES = enum.auto()
+    INLINE_IMAGES = enum.auto()
+    DRAWING_IMAGES = enum.auto()
+    IMAGES = XOBJECT_IMAGES | INLINE_IMAGES | DRAWING_IMAGES
+
+
+def _rolling_checksum(stream: BytesIO, blocksize: int = 65536) -> str:
+    hash = hashlib.md5()
+    for block in iter(lambda: stream.read(blocksize), b""):
+        hash.update(block)
+    return hash.hexdigest()
 
-class DocumentInformation(DictionaryObject):
-    """
-    A class representing the basic document metadata provided in a PDF File.
-    This class is accessible through
-    :py:class:`PdfReader.metadata<pypdf.PdfReader.metadata>`.
-
-    All text properties of the document metadata have
-    *two* properties, eg. author and author_raw. The non-raw property will
-    always return a ``TextStringObject``, making it ideal for a case where
-    the metadata is being displayed. The raw property can sometimes return
-    a ``ByteStringObject``, if pypdf was unable to decode the string's
-    text encoding; this requires additional safety in the caller and
-    therefore is not as commonly accessed.
-    """
-
-    def __init__(self) -> None:
-        DictionaryObject.__init__(self)
-
-    def _get_text(self, key: str) -> Optional[str]:
-        retval = self.get(key, None)
-        if isinstance(retval, TextStringObject):
-            return retval
-        return None
-
-    @property
-    def title(self) -> Optional[str]:
-        """
-        Read-only property accessing the document's title.
 
-        Returns a ``TextStringObject`` or ``None`` if the title is not
-        specified.
-        """
-        return (
-            self._get_text(DI.TITLE) or self.get(DI.TITLE).get_object()  # type: ignore
-            if self.get(DI.TITLE)
-            else None
-        )
+class PdfWriter(PdfDocCommon):
+    """
+    Write a PDF file out, given pages produced by another class or through
+    cloning a PDF file during initialization.
 
-    @property
-    def title_raw(self) -> Optional[str]:
-        """The "raw" version of title; can return a ``ByteStringObject``."""
-        return self.get(DI.TITLE)
+    Typically data is added from a :class:`PdfReader<pypdf.PdfReader>`.
+    """
 
+    # for commonality
     @property
-    def author(self) -> Optional[str]:
-        """
-        Read-only property accessing the document's author.
-
-        Returns a ``TextStringObject`` or ``None`` if the author is not
-        specified.
+    def is_encrypted(self) -> bool:
         """
-        return self._get_text(DI.AUTHOR)
-
-    @property
-    def author_raw(self) -> Optional[str]:
-        """The "raw" version of author; can return a ``ByteStringObject``."""
-        return self.get(DI.AUTHOR)
+        Read-only boolean property showing whether this PDF file is encrypted.
 
-    @property
-    def subject(self) -> Optional[str]:
+        Note that this property, if true, will remain true even after the
+        :meth:`decrypt()<pypdf.PdfReader.decrypt>` method is called.
         """
-        Read-only property accessing the document's subject.
+        return False
 
-        Returns a ``TextStringObject`` or ``None`` if the subject is not
-        specified.
-        """
-        return self._get_text(DI.SUBJECT)
+    def __init__(
+        self,
+        fileobj: StrByteType = "",
+        clone_from: Union[None, PdfReader, StrByteType, Path] = None,
+    ) -> None:
+        self._header = b"%PDF-1.3"
+        self._objects: List[PdfObject] = []
+        """The indirect objects in the PDF."""
+
+        self._idnum_hash: Dict[bytes, IndirectObject] = {}
+        """Maps hash values of indirect objects to their IndirectObject instances."""
+
+        self._id_translated: Dict[int, Dict[int, int]] = {}
+
+        # The root of our page tree node.
+        pages = DictionaryObject()
+        pages.update(
+            {
+                NameObject(PA.TYPE): NameObject("/Pages"),
+                NameObject(PA.COUNT): NumberObject(0),
+                NameObject(PA.KIDS): ArrayObject(),
+            }
+        )
+        self._pages = self._add_object(pages)
+        self.flattened_pages = []
 
-    @property
-    def subject_raw(self) -> Optional[str]:
-        """The "raw" version of subject; can return a ``ByteStringObject``."""
-        return self.get(DI.SUBJECT)
+        # info object
+        info = DictionaryObject()
+        info.update(
+            {
+                NameObject("/Producer"): create_string_object(
+                    codecs.BOM_UTF16_BE + "pypdf".encode("utf-16be")
+                )
+            }
+        )
+        self._info_obj: PdfObject = self._add_object(info)
 
-    @property
-    def creator(self) -> Optional[str]:
-        """
-        Read-only property accessing the document's creator.
+        # root object
+        self._root_object = DictionaryObject()
+        self._root_object.update(
+            {
+                NameObject(PA.TYPE): NameObject(CO.CATALOG),
+                NameObject(CO.PAGES): self._pages,
+            }
+        )
+        self._root = self._add_object(self._root_object)
 
-        If the document was converted to PDF from another format, this is the
-        name of the application (e.g. OpenOffice) that created the original
-        document from which it was converted. Returns a ``TextStringObject`` or
-        ``None`` if the creator is not specified.
-        """
-        return self._get_text(DI.CREATOR)
+        if clone_from is not None:
+            if not isinstance(clone_from, PdfReader):
+                clone_from = PdfReader(clone_from)
+            self.clone_document_from_reader(clone_from)
+        self.fileobj = fileobj
+        self.with_as_usage = False
 
-    @property
-    def creator_raw(self) -> Optional[str]:
-        """The "raw" version of creator; can return a ``ByteStringObject``."""
-        return self.get(DI.CREATOR)
+        self._encryption: Optional[Encryption] = None
+        self._encrypt_entry: Optional[DictionaryObject] = None
+        self._ID: Union[ArrayObject, None] = None
 
     @property
-    def producer(self) -> Optional[str]:
+    def root_object(self) -> DictionaryObject:
         """
-        Read-only property accessing the document's producer.
+        Provide direct access to Pdf Structure.
 
-        If the document was converted to PDF from another format, this is the
-        name of the application (for example, OSX Quartz) that converted it to
-        PDF. Returns a ``TextStringObject`` or ``None`` if the producer is not
-        specified.
+        Note:
+            Recommended be used only for read access.
         """
-        return self._get_text(DI.PRODUCER)
+        return self._root_object
 
     @property
-    def producer_raw(self) -> Optional[str]:
-        """The "raw" version of producer; can return a ``ByteStringObject``."""
-        return self.get(DI.PRODUCER)
-
-    @property
-    def creation_date(self) -> Optional[datetime]:
-        """Read-only property accessing the document's creation date."""
-        return parse_iso8824_date(self._get_text(DI.CREATION_DATE))
-
-    @property
-    def creation_date_raw(self) -> Optional[str]:
-        """
-        The "raw" version of creation date; can return a ``ByteStringObject``.
-
-        Typically in the format ``D:YYYYMMDDhhmmss[+Z-]hh'mm`` where the suffix
-        is the offset from UTC.
+    def _info(self) -> Optional[DictionaryObject]:
         """
-        return self.get(DI.CREATION_DATE)
+        Provide access to "/Info". standardized with PdfWriter.
 
-    @property
-    def modification_date(self) -> Optional[datetime]:
+        Returns:
+            /Info Dictionary ; None if the entry does not exists
         """
-        Read-only property accessing the document's modification date.
+        return cast(DictionaryObject, self._info_obj.get_object())
 
-        The date and time the document was most recently modified.
-        """
-        return parse_iso8824_date(self._get_text(DI.MOD_DATE))
+    @_info.setter
+    def _info(self, value: Union[IndirectObject, DictionaryObject]) -> None:
+        obj = cast(DictionaryObject, self._info_obj.get_object())
+        obj.clear()
+        obj.update(cast(DictionaryObject, value.get_object()))
 
     @property
-    def modification_date_raw(self) -> Optional[str]:
-        """
-        The "raw" version of modification date; can return a
-        ``ByteStringObject``.
-
-        Typically in the format ``D:YYYYMMDDhhmmss[+Z-]hh'mm`` where the suffix
-        is the offset from UTC.
-        """
-        return self.get(DI.MOD_DATE)
-
-
-class PdfReader:
-    """
-    Initialize a PdfReader object.
+    def xmp_metadata(self) -> Optional[XmpInformation]:
+        """XMP (Extensible Metadata Platform) data."""
+        return cast(XmpInformation, self.root_object.xmp_metadata)
 
-    This operation can take some time, as the PDF stream's cross-reference
-    tables are read into memory.
+    @xmp_metadata.setter
+    def xmp_metadata(self, value: Optional[XmpInformation]) -> None:
+        """XMP (Extensible Metadata Platform) data."""
+        if value is None:
+            if "/Metadata" in self.root_object:
+                del self.root_object["/Metadata"]
+        else:
+            self.root_object[NameObject("/Metadata")] = value
 
-    Args:
-        stream: A File object or an object that supports the standard read
-            and seek methods similar to a File object. Could also be a
-            string representing a path to a PDF file.
-        strict: Determines whether user should be warned of all
-            problems and also causes some correctable problems to be fatal.
-            Defaults to ``False``.
-        password: Decrypt PDF file at initialization. If the
-            password is None, the file will not be decrypted.
-            Defaults to ``None``
-    """
+        return self.root_object.xmp_metadata  # type: ignore
 
-    @property
-    def viewer_preferences(self) -> Optional[ViewerPreferences]:
-        """Returns the existing ViewerPreferences as an overloaded dictionary."""
-        o = cast(DictionaryObject, self.trailer["/Root"]).get(
-            CD.VIEWER_PREFERENCES, None
-        )
-        if o is None:
-            return None
-        o = o.get_object()
-        if not isinstance(o, ViewerPreferences):
-            o = ViewerPreferences(o)
-        return o
+    def __enter__(self) -> "PdfWriter":
+        """Store that writer is initialized by 'with'."""
+        self.with_as_usage = True
+        return self
 
-    def __init__(
+    def __exit__(
         self,
-        stream: Union[StrByteType, Path],
-        strict: bool = False,
-        password: Union[None, str, bytes] = None,
-    ) -> None:
-        self.strict = strict
-        self.flattened_pages: Optional[List[PageObject]] = None
-        #: Storage of parsed PDF objects.
-        self.resolved_objects: Dict[Tuple[Any, Any], Optional[PdfObject]] = {}
-        self.xref_index = 0
-        self._page_id2num: Optional[
-            Dict[Any, Any]
-        ] = None  # map page indirect_reference number to Page Number
-        if hasattr(stream, "mode") and "b" not in stream.mode:
-            logger_warning(
-                "PdfReader stream/file object is not in binary mode. "
-                "It may not be read correctly.",
-                __name__,
-            )
-        if isinstance(stream, (str, Path)):
-            with open(stream, "rb") as fh:
-                stream = BytesIO(fh.read())
-        self.read(stream)
-        self.stream = stream
-
-        self._override_encryption = False
-        self._encryption: Optional[Encryption] = None
-        if self.is_encrypted:
-            self._override_encryption = True
-            # Some documents may not have a /ID, use two empty
-            # byte strings instead. Solves
-            # https://github.com/py-pdf/pypdf/issues/608
-            id_entry = self.trailer.get(TK.ID)
-            id1_entry = id_entry[0].get_object().original_bytes if id_entry else b""
-            encrypt_entry = cast(
-                DictionaryObject, self.trailer[TK.ENCRYPT].get_object()
-            )
-            self._encryption = Encryption.read(encrypt_entry, id1_entry)
-
-            # try empty password if no password provided
-            pwd = password if password is not None else b""
-            if (
-                self._encryption.verify(pwd) == PasswordType.NOT_DECRYPTED
-                and password is not None
-            ):
-                # raise if password provided
-                raise WrongPasswordError("Wrong password")
-            self._override_encryption = False
-        elif password is not None:
-            raise PdfReadError("Not encrypted file")
+        exc_type: Optional[Type[BaseException]],
+        exc: Optional[BaseException],
+        traceback: Optional[TracebackType],
+    ) -> None:
+        """Write data to the fileobj."""
+        if self.fileobj:
+            self.write(self.fileobj)
 
     def _repr_mimebundle_(
         self,
         include: Union[None, Iterable[str]] = None,
         exclude: Union[None, Iterable[str]] = None,
     ) -> Dict[str, Any]:
         """
         Integration into Jupyter Notebooks.
 
         This method returns a dictionary that maps a mime-type to it's
         representation.
 
         See https://ipython.readthedocs.io/en/stable/config/integrating.html
         """
-        self.stream.seek(0)
-        pdf_data = self.stream.read()
+        pdf_data = BytesIO()
+        self.write(pdf_data)
         data = {
             "application/pdf": pdf_data,
         }
 
         if include is not None:
             # Filter representations based on include list
             data = {k: v for k, v in data.items() if k in include}
@@ -372,690 +309,1750 @@
             data = {k: v for k, v in data.items() if k not in exclude}
 
         return data
 
     @property
     def pdf_header(self) -> str:
         """
-        The first 8 bytes of the file.
+        Read/Write Property
+        Header of the PDF document that is written.
 
-        This is typically something like ``'%PDF-1.6'`` and can be used to
-        detect if the file is actually a PDF file and which version it is.
-        """
-        # TODO: Make this return a bytes object for consistency
-        #       but that needs a deprecation
-        loc = self.stream.tell()
-        self.stream.seek(0, 0)
-        pdf_file_version = self.stream.read(8).decode("utf-8", "backslashreplace")
-        self.stream.seek(loc, 0)  # return to where it was
-        return pdf_file_version
+        This should be something like ``'%PDF-1.5'``. It is recommended to set
+        the lowest version that supports all features which are used within the
+        PDF file.
 
-    @property
-    def metadata(self) -> Optional[DocumentInformation]:
+        Note: `pdf_header` returns a string but accepts bytes or str for writing
         """
-        Retrieve the PDF file's document information dictionary, if it exists.
+        return self._header.decode()
+
+    @pdf_header.setter
+    def pdf_header(self, new_header: Union[str, bytes]) -> None:
+        if isinstance(new_header, str):
+            new_header = new_header.encode()
+        self._header = new_header
+
+    def _add_object(self, obj: PdfObject) -> IndirectObject:
+        if (
+            getattr(obj, "indirect_reference", None) is not None
+            and obj.indirect_reference.pdf == self  # type: ignore
+        ):
+            return obj.indirect_reference  # type: ignore
+        # check for /Contents in Pages (/Contents in annotation are strings)
+        if isinstance(obj, DictionaryObject) and isinstance(
+            obj.get(PG.CONTENTS, None), (ArrayObject, DictionaryObject)
+        ):
+            obj[NameObject(PG.CONTENTS)] = self._add_object(obj[PG.CONTENTS])
+        self._objects.append(obj)
+        obj.indirect_reference = IndirectObject(len(self._objects), 0, self)
+        return obj.indirect_reference
+
+    def get_object(
+        self,
+        indirect_reference: Union[int, IndirectObject],
+    ) -> PdfObject:
+        if isinstance(indirect_reference, int):
+            return self._objects[indirect_reference - 1]
+        if indirect_reference.pdf != self:
+            raise ValueError("pdf must be self")
+        return self._objects[indirect_reference.idnum - 1]
 
-        Note that some PDF files use metadata streams instead of docinfo
-        dictionaries, and these metadata streams will not be accessed by this
-        function.
+    def _replace_object(
+        self,
+        indirect_reference: Union[int, IndirectObject],
+        obj: PdfObject,
+    ) -> PdfObject:
+        if isinstance(indirect_reference, IndirectObject):
+            if indirect_reference.pdf != self:
+                raise ValueError("pdf must be self")
+            indirect_reference = indirect_reference.idnum
+        gen = self._objects[indirect_reference - 1].indirect_reference.generation  # type: ignore
+        if (
+            getattr(obj, "indirect_reference", None) is not None
+            and obj.indirect_reference.pdf != self  # type: ignore
+        ):
+            obj = obj.clone(self)
+        self._objects[indirect_reference - 1] = obj
+        obj.indirect_reference = IndirectObject(indirect_reference, gen, self)
+        return self._objects[indirect_reference - 1]
+
+    def _add_page(
+        self,
+        page: PageObject,
+        action: Callable[[Any, Union[PageObject, IndirectObject]], None],
+        excluded_keys: Iterable[str] = (),
+    ) -> PageObject:
+        assert cast(str, page[PA.TYPE]) == CO.PAGE
+        page_org = page
+        excluded_keys = list(excluded_keys)
+        excluded_keys += [PA.PARENT, "/StructParents"]
+        # acrobat does not accept to have two indirect ref pointing on the same
+        # page; therefore in order to add easily multiple copies of the same
+        # page, we need to create a new dictionary for the page, however the
+        # objects below (including content) are not duplicated:
+        try:  # delete an already existing page
+            del self._id_translated[id(page_org.indirect_reference.pdf)][  # type: ignore
+                page_org.indirect_reference.idnum  # type: ignore
+            ]
+        except Exception:
+            pass
+        page = cast("PageObject", page_org.clone(self, False, excluded_keys))
+        if page_org.pdf is not None:
+            other = page_org.pdf.pdf_header
+            self.pdf_header = _get_max_pdf_version_header(self.pdf_header, other)
+        page[NameObject(PA.PARENT)] = self._pages
+        pages = cast(DictionaryObject, self.get_object(self._pages))
+        assert page.indirect_reference is not None
+        action(pages[PA.KIDS], page.indirect_reference)
+        action(self.flattened_pages, page)
+        page_count = cast(int, pages[PA.COUNT])
+        pages[NameObject(PA.COUNT)] = NumberObject(page_count + 1)
+        return page
+
+    def set_need_appearances_writer(self, state: bool = True) -> None:
+        """
+        Sets the "NeedAppearances" flag in the PDF writer.
+
+        The "NeedAppearances" flag indicates whether the appearance dictionary
+        for form fields should be automatically generated by the PDF viewer or
+        if the embedded appearance should be used.
+
+        Args:
+            state: The actual value of the NeedAppearances flag.
+
+        Returns:
+            None
         """
-        if TK.INFO not in self.trailer:
-            return None
-        obj = self.trailer[TK.INFO]
-        retval = DocumentInformation()
-        if isinstance(obj, type(None)):
-            raise PdfReadError(
-                "trailer not found or does not point to document information directory"
+        # See 12.7.2 and 7.7.2 for more information:
+        # https://opensource.adobe.com/dc-acrobat-sdk-docs/pdfstandards/PDF32000_2008.pdf
+        try:
+            # get the AcroForm tree
+            if CatalogDictionary.ACRO_FORM not in self._root_object:
+                self._root_object[
+                    NameObject(CatalogDictionary.ACRO_FORM)
+                ] = self._add_object(DictionaryObject())
+
+            need_appearances = NameObject(InteractiveFormDictEntries.NeedAppearances)
+            cast(DictionaryObject, self._root_object[CatalogDictionary.ACRO_FORM])[
+                need_appearances
+            ] = BooleanObject(state)
+        except Exception as exc:  # pragma: no cover
+            logger_warning(
+                f"set_need_appearances_writer({state}) catch : {exc}", __name__
             )
-        retval.update(obj)  # type: ignore
-        return retval
 
-    @property
-    def xmp_metadata(self) -> Optional[XmpInformation]:
-        """XMP (Extensible Metadata Platform) data."""
-        try:
-            self._override_encryption = True
-            return self.trailer[TK.ROOT].xmp_metadata  # type: ignore
-        finally:
-            self._override_encryption = False
+    def create_viewer_preferences(self) -> ViewerPreferences:
+        o = ViewerPreferences()
+        self._root_object[NameObject(CD.VIEWER_PREFERENCES)] = self._add_object(o)
+        return o
+
+    def add_page(
+        self,
+        page: PageObject,
+        excluded_keys: Iterable[str] = (),
+    ) -> PageObject:
+        """
+        Add a page to this PDF file.
+
+        Recommended for advanced usage including the adequate excluded_keys.
 
-    def _get_num_pages(self) -> int:
+        The page is usually acquired from a :class:`PdfReader<pypdf.PdfReader>`
+        instance.
+
+        Args:
+            page: The page to add to the document. Should be
+                an instance of :class:`PageObject<pypdf._page.PageObject>`
+            excluded_keys:
+
+        Returns:
+            The added PageObject.
+        """
+        return self._add_page(page, list.append, excluded_keys)
+
+    def insert_page(
+        self,
+        page: PageObject,
+        index: int = 0,
+        excluded_keys: Iterable[str] = (),
+    ) -> PageObject:
         """
-        Calculate the number of pages in this PDF file.
+        Insert a page in this PDF file. The page is usually acquired from a
+        :class:`PdfReader<pypdf.PdfReader>` instance.
+
+        Args:
+            page: The page to add to the document.
+            index: Position at which the page will be inserted.
+            excluded_keys:
 
         Returns:
-            The number of pages of the parsed PDF file
+            The added PageObject.
+        """
+        return self._add_page(page, lambda kids, p: kids.insert(index, p))
+
+    def _get_page_number_by_indirect(
+        self, indirect_reference: Union[None, int, NullObject, IndirectObject]
+    ) -> Optional[int]:
+        """
+        Generate _page_id2num.
+
+        Args:
+            indirect_reference:
+
+        Returns:
+            The page number or None
+        """
+        # to provide same function as in PdfReader
+        if indirect_reference is None or isinstance(indirect_reference, NullObject):
+            return None
+        if isinstance(indirect_reference, int):
+            indirect_reference = IndirectObject(indirect_reference, 0, self)
+        obj = indirect_reference.get_object()
+        if isinstance(obj, PageObject):
+            return obj.page_number
+        return None
+
+    def add_blank_page(
+        self, width: Optional[float] = None, height: Optional[float] = None
+    ) -> PageObject:
+        """
+        Append a blank page to this PDF file and return it.
+
+        If no page size is specified, use the size of the last page.
+
+        Args:
+            width: The width of the new page expressed in default user
+                space units.
+            height: The height of the new page expressed in default
+                user space units.
+
+        Returns:
+            The newly appended page
 
         Raises:
-            PdfReadError: if file is encrypted and restrictions prevent
-                this action.
+            PageSizeNotDefinedError: if width and height are not defined
+                and previous page does not exist.
         """
-        # Flattened pages will not work on an Encrypted PDF;
-        # the PDF file's page count is used in this case. Otherwise,
-        # the original method (flattened page count) is used.
-        if self.is_encrypted:
-            return self.trailer[TK.ROOT]["/Pages"]["/Count"]  # type: ignore
-        else:
-            if self.flattened_pages is None:
-                self._flatten()
-            return len(self.flattened_pages)  # type: ignore
+        page = PageObject.create_blank_page(self, width, height)
+        return self.add_page(page)
 
-    def _get_page(self, page_number: int) -> PageObject:
+    def insert_blank_page(
+        self,
+        width: Optional[Union[float, decimal.Decimal]] = None,
+        height: Optional[Union[float, decimal.Decimal]] = None,
+        index: int = 0,
+    ) -> PageObject:
         """
-        Retrieve a page by number from this PDF file.
+        Insert a blank page to this PDF file and return it.
+
+        If no page size is specified, use the size of the last page.
 
         Args:
-            page_number: The page number to retrieve
-                (pages begin at zero)
+            width: The width of the new page expressed in default user
+                space units.
+            height: The height of the new page expressed in default
+                user space units.
+            index: Position to add the page.
 
         Returns:
-            A :class:`PageObject<pypdf._page.PageObject>` instance.
+            The newly appended page.
+
+        Raises:
+            PageSizeNotDefinedError: if width and height are not defined
+                and previous page does not exist.
         """
-        if self.flattened_pages is None:
-            self._flatten()
-        assert self.flattened_pages is not None, "hint for mypy"
-        return self.flattened_pages[page_number]
+        if width is None or height is None and (self.get_num_pages() - 1) >= index:
+            oldpage = self.pages[index]
+            width = oldpage.mediabox.width
+            height = oldpage.mediabox.height
+        page = PageObject.create_blank_page(self, width, height)
+        self.insert_page(page, index)
+        return page
 
     @property
-    def named_destinations(self) -> Dict[str, Any]:
+    def open_destination(
+        self,
+    ) -> Union[None, Destination, TextStringObject, ByteStringObject]:
+        return super().open_destination
+
+    @open_destination.setter
+    def open_destination(self, dest: Union[None, str, Destination, PageObject]) -> None:
+        if dest is None:
+            try:
+                del self._root_object["/OpenAction"]
+            except KeyError:
+                pass
+        elif isinstance(dest, str):
+            self._root_object[NameObject("/OpenAction")] = TextStringObject(dest)
+        elif isinstance(dest, Destination):
+            self._root_object[NameObject("/OpenAction")] = dest.dest_array
+        elif isinstance(dest, PageObject):
+            self._root_object[NameObject("/OpenAction")] = Destination(
+                "Opening",
+                dest.indirect_reference
+                if dest.indirect_reference is not None
+                else NullObject(),
+                PAGE_FIT,
+            ).dest_array
+
+    def add_js(self, javascript: str) -> None:
         """
-        A read-only dictionary which maps names to
-        :class:`Destinations<pypdf.generic.Destination>`
+        Add JavaScript which will launch upon opening this PDF.
+
+        Args:
+            javascript: Your Javascript.
+
+        >>> output.add_js("this.print({bUI:true,bSilent:false,bShrinkToFit:true});")
+        # Example: This will launch the print window when the PDF is opened.
+        """
+        # Names / JavaScript preferred to be able to add multiple scripts
+        if "/Names" not in self._root_object:
+            self._root_object[NameObject(CA.NAMES)] = DictionaryObject()
+        names = cast(DictionaryObject, self._root_object[CA.NAMES])
+        if "/JavaScript" not in names:
+            names[NameObject("/JavaScript")] = DictionaryObject(
+                {NameObject("/Names"): ArrayObject()}
+            )
+        js_list = cast(
+            ArrayObject, cast(DictionaryObject, names["/JavaScript"])["/Names"]
+        )
+
+        js = DictionaryObject()
+        js.update(
+            {
+                NameObject(PA.TYPE): NameObject("/Action"),
+                NameObject("/S"): NameObject("/JavaScript"),
+                NameObject("/JS"): TextStringObject(f"{javascript}"),
+            }
+        )
+        # We need a name for parameterized javascript in the pdf file,
+        # but it can be anything.
+        js_list.append(create_string_object(str(uuid.uuid4())))
+        js_list.append(self._add_object(js))
+
+    def add_attachment(self, filename: str, data: Union[str, bytes]) -> None:
+        """
+        Embed a file inside the PDF.
+
+        Reference:
+        https://opensource.adobe.com/dc-acrobat-sdk-docs/pdfstandards/PDF32000_2008.pdf
+        Section 7.11.3
+
+        Args:
+            filename: The filename to display.
+            data: The data in the file.
         """
-        return self._get_named_destinations()
+        # We need three entries:
+        # * The file's data
+        # * The /Filespec entry
+        # * The file's name, which goes in the Catalog
+
+        # The entry for the file
+        # Sample:
+        # 8 0 obj
+        # <<
+        #  /Length 12
+        #  /Type /EmbeddedFile
+        # >>
+        # stream
+        # Hello world!
+        # endstream
+        # endobj
+
+        file_entry = DecodedStreamObject()
+        file_entry.set_data(b_(data))
+        file_entry.update({NameObject(PA.TYPE): NameObject("/EmbeddedFile")})
+
+        # The Filespec entry
+        # Sample:
+        # 7 0 obj
+        # <<
+        #  /Type /Filespec
+        #  /F (hello.txt)
+        #  /EF << /F 8 0 R >>
+        # >>
 
-    # A select group of relevant field attributes. For the complete list,
-    # see section 8.6.2 of the PDF 1.7 reference.
+        ef_entry = DictionaryObject()
+        ef_entry.update({NameObject("/F"): self._add_object(file_entry)})
 
-    def get_fields(
+        filespec = DictionaryObject()
+        filespec.update(
+            {
+                NameObject(PA.TYPE): NameObject("/Filespec"),
+                NameObject(FileSpecificationDictionaryEntries.F): create_string_object(
+                    filename
+                ),  # Perhaps also try TextStringObject
+                NameObject(FileSpecificationDictionaryEntries.EF): ef_entry,
+            }
+        )
+
+        # Then create the entry for the root, as it needs
+        # a reference to the Filespec
+        # Sample:
+        # 1 0 obj
+        # <<
+        #  /Type /Catalog
+        #  /Outlines 2 0 R
+        #  /Pages 3 0 R
+        #  /Names << /EmbeddedFiles << /Names [(hello.txt) 7 0 R] >> >>
+        # >>
+        # endobj
+
+        if CA.NAMES not in self._root_object:
+            self._root_object[NameObject(CA.NAMES)] = self._add_object(
+                DictionaryObject()
+            )
+        if "/EmbeddedFiles" not in cast(DictionaryObject, self._root_object[CA.NAMES]):
+            embedded_files_names_dictionary = DictionaryObject(
+                {NameObject(CA.NAMES): ArrayObject()}
+            )
+            cast(DictionaryObject, self._root_object[CA.NAMES])[
+                NameObject("/EmbeddedFiles")
+            ] = self._add_object(embedded_files_names_dictionary)
+        else:
+            embedded_files_names_dictionary = cast(
+                DictionaryObject,
+                cast(DictionaryObject, self._root_object[CA.NAMES])["/EmbeddedFiles"],
+            )
+        cast(ArrayObject, embedded_files_names_dictionary[CA.NAMES]).extend(
+            [create_string_object(filename), filespec]
+        )
+
+    def append_pages_from_reader(
         self,
-        tree: Optional[TreeObject] = None,
-        retval: Optional[Dict[Any, Any]] = None,
-        fileobj: Optional[Any] = None,
-    ) -> Optional[Dict[str, Any]]:
+        reader: PdfReader,
+        after_page_append: Optional[Callable[[PageObject], None]] = None,
+    ) -> None:
         """
-        Extract field data if this PDF contains interactive form fields.
+        Copy pages from reader to writer. Includes an optional callback
+        parameter which is invoked after pages are appended to the writer.
 
-        The *tree* and *retval* parameters are for recursive use.
+        ``append`` should be preferred.
 
         Args:
-            tree:
-            retval:
-            fileobj: A file object (usually a text file) to write
-                a report to on all interactive form fields found.
+            reader: a PdfReader object from which to copy page
+                annotations to this writer object.  The writer's annots
+                will then be updated.
+            after_page_append:
+                Callback function that is invoked after each page is appended to
+                the writer. Signature includes a reference to the appended page
+                (delegates to append_pages_from_reader). The single parameter of
+                the callback is a reference to the page just appended to the
+                document.
+        """
+        # Get page count from writer and reader
+        reader_num_pages = len(reader.pages)
+        # Copy pages from reader to writer
+        for reader_page_number in range(reader_num_pages):
+            reader_page = reader.pages[reader_page_number]
+            writer_page = self.add_page(reader_page)
+            # Trigger callback, pass writer page as parameter
+            if callable(after_page_append):
+                after_page_append(writer_page)
 
-        Returns:
-            A dictionary where each key is a field name, and each
-            value is a :class:`Field<pypdf.generic.Field>` object. By
-            default, the mapping name is used for keys.
-            ``None`` if form data could not be located.
-        """
-        field_attributes = FA.attributes_dict()
-        field_attributes.update(CheckboxRadioButtonAttributes.attributes_dict())
-        if retval is None:
-            retval = {}
-            catalog = cast(DictionaryObject, self.trailer[TK.ROOT])
-            # get the AcroForm tree
-            if CD.ACRO_FORM in catalog:
-                tree = cast(Optional[TreeObject], catalog[CD.ACRO_FORM])
-            else:
-                return None
-        if tree is None:
-            return retval
-        self._check_kids(tree, retval, fileobj)
-        for attr in field_attributes:
-            if attr in tree:
-                # Tree is a field
-                self._build_field(tree, retval, fileobj, field_attributes)
-                break
-
-        if "/Fields" in tree:
-            fields = cast(ArrayObject, tree["/Fields"])
-            for f in fields:
-                field = f.get_object()
-                self._build_field(field, retval, fileobj, field_attributes)
-
-        return retval
-
-    def _get_qualified_field_name(self, parent: DictionaryObject) -> str:
-        if "/TM" in parent:
-            return cast(str, parent["/TM"])
-        elif "/Parent" in parent:
-            return (
-                self._get_qualified_field_name(
-                    cast(DictionaryObject, parent["/Parent"])
-                )
-                + "."
-                + cast(str, parent["/T"])
+    def _update_field_annotation(
+        self, field: DictionaryObject, anno: DictionaryObject
+    ) -> None:
+        # Calculate rectangle dimensions
+        _rct = cast(RectangleObject, anno[AA.Rect])
+        rct = RectangleObject((0, 0, _rct[2] - _rct[0], _rct[3] - _rct[1]))
+
+        # Extract font information
+        da = anno.get_inherited(
+            AA.DA,
+            cast(DictionaryObject, self.root_object[CatalogDictionary.ACRO_FORM]).get(
+                AA.DA, None
+            ),
+        )
+        if da is None:
+            da = TextStringObject("/Helv 0 Tf 0 g")
+        else:
+            da = da.get_object()
+        font_properties = da.replace("\n", " ").replace("\r", " ").split(" ")
+        font_properties = [x for x in font_properties if x != ""]
+        font_name = font_properties[font_properties.index("Tf") - 2]
+        font_height = float(font_properties[font_properties.index("Tf") - 1])
+        if font_height == 0:
+            font_height = rct.height - 2
+            font_properties[font_properties.index("Tf") - 1] = str(font_height)
+            da = " ".join(font_properties)
+        y_offset = rct.height - 1 - font_height
+
+        # Retrieve font information from local DR ...
+        dr: Any = cast(
+            DictionaryObject,
+            cast(
+                DictionaryObject,
+                anno.get_inherited(
+                    "/DR",
+                    cast(
+                        DictionaryObject, self.root_object[CatalogDictionary.ACRO_FORM]
+                    ).get("/DR", DictionaryObject()),
+                ),
+            ).get_object(),
+        )
+        dr = dr.get("/Font", DictionaryObject()).get_object()
+        if font_name not in dr:
+            # ...or AcroForm dictionary
+            dr = cast(
+                Dict[Any, Any],
+                cast(
+                    DictionaryObject, self.root_object[CatalogDictionary.ACRO_FORM]
+                ).get("/DR", {}),
             )
+            dr = dr.get_object().get("/Font", DictionaryObject()).get_object()
+        font_res = dr.get(font_name, None)
+        if font_res is not None:
+            font_res = cast(DictionaryObject, font_res.get_object())
+            font_subtype, _, font_encoding, font_map = build_char_map_from_dict(
+                200, font_res
+            )
+            try:  # get rid of width stored in -1 key
+                del font_map[-1]
+            except KeyError:
+                pass
+            font_full_rev: Dict[str, bytes]
+            if isinstance(font_encoding, str):
+                font_full_rev = {
+                    v: k.encode(font_encoding) for k, v in font_map.items()
+                }
+            else:
+                font_full_rev = {v: bytes((k,)) for k, v in font_encoding.items()}
+                font_encoding_rev = {v: bytes((k,)) for k, v in font_encoding.items()}
+                for kk, v in font_map.items():
+                    font_full_rev[v] = font_encoding_rev.get(kk, kk)
         else:
-            return cast(str, parent["/T"])
+            logger_warning(f"Font dictionary for {font_name} not found.", __name__)
+            font_full_rev = {}
+
+        # Retrieve field text and selected values
+        field_flags = field.get(FA.Ff, 0)
+        if field.get(FA.FT, "/Tx") == "/Ch" and field_flags & FA.FfBits.Combo == 0:
+            txt = "\n".join(anno.get_inherited(FA.Opt, []))
+            sel = field.get("/V", [])
+            if not isinstance(sel, list):
+                sel = [sel]
+        else:  # /Tx
+            txt = field.get("/V", "")
+            sel = []
+        # Escape parentheses (pdf 1.7 reference, table 3.2  Literal Strings)
+        txt = txt.replace("\\", "\\\\").replace("(", r"\(").replace(")", r"\)")
+        # Generate appearance stream
+        ap_stream = f"q\n/Tx BMC \nq\n1 1 {rct.width - 1} {rct.height - 1} re\nW\nBT\n{da}\n".encode()
+        for line_number, line in enumerate(txt.replace("\n", "\r").split("\r")):
+            if line in sel:
+                # may be improved but can not find how get fill working => replaced with lined box
+                ap_stream += (
+                    f"1 {y_offset - (line_number * font_height * 1.4) - 1} {rct.width - 2} {font_height + 2} re\n"
+                    f"0.5 0.5 0.5 rg s\n{da}\n"
+                ).encode()
+            if line_number == 0:
+                ap_stream += f"2 {y_offset} Td\n".encode()
+            else:
+                # Td is a relative translation
+                ap_stream += f"0 {- font_height * 1.4} Td\n".encode()
+            enc_line: List[bytes] = [
+                font_full_rev.get(c, c.encode("utf-16-be")) for c in line
+            ]
+            if any(len(c) >= 2 for c in enc_line):
+                ap_stream += b"<" + (b"".join(enc_line)).hex().encode() + b"> Tj\n"
+            else:
+                ap_stream += b"(" + b"".join(enc_line) + b") Tj\n"
+        ap_stream += b"ET\nQ\nEMC\nQ\n"
+
+        # Create appearance dictionary
+        dct = DecodedStreamObject.initialize_from_dictionary(
+            {
+                NameObject("/Type"): NameObject("/XObject"),
+                NameObject("/Subtype"): NameObject("/Form"),
+                NameObject("/BBox"): rct,
+                "__streamdata__": ByteStringObject(ap_stream),
+                "/Length": 0,
+            }
+        )
 
-    def _build_field(
+        # Update Resources with font information if necessary
+        if font_res is not None:
+            dct[NameObject("/Resources")] = DictionaryObject(
+                {
+                    NameObject("/Font"): DictionaryObject(
+                        {
+                            NameObject(font_name): getattr(
+                                font_res, "indirect_reference", font_res
+                            )
+                        }
+                    )
+                }
+            )
+        if AA.AP not in anno:
+            anno[NameObject(AA.AP)] = DictionaryObject(
+                {NameObject("/N"): self._add_object(dct)}
+            )
+        elif "/N" not in cast(DictionaryObject, anno[AA.AP]):
+            cast(DictionaryObject, anno[NameObject(AA.AP)])[
+                NameObject("/N")
+            ] = self._add_object(dct)
+        else:  # [/AP][/N] exists
+            n = anno[AA.AP]["/N"].indirect_reference.idnum  # type: ignore
+            self._objects[n - 1] = dct
+            dct.indirect_reference = IndirectObject(n, 0, self)
+
+    def update_page_form_field_values(
         self,
-        field: Union[TreeObject, DictionaryObject],
-        retval: Dict[Any, Any],
-        fileobj: Any,
-        field_attributes: Any,
+        page: Union[PageObject, List[PageObject], None],
+        fields: Dict[str, Any],
+        flags: FieldFlag = OPTIONAL_READ_WRITE_FIELD,
+        auto_regenerate: Optional[bool] = True,
     ) -> None:
-        self._check_kids(field, retval, fileobj)
+        """
+        Update the form field values for a given page from a fields dictionary.
+
+        Copy field texts and values from fields to page.
+        If the field links to a parent object, add the information to the parent.
+
+        Args:
+            page: `PageObject` - references **PDF writer's page** where the
+                annotations and field data will be updated.
+                `List[Pageobject]` - provides list of page to be processsed.
+                `None` - all pages.
+            fields: a Python dictionary of field names (/T) and text
+                values (/V).
+            flags: An integer (0 to 7). The first bit sets ReadOnly, the
+                second bit sets Required, the third bit sets NoExport. See
+                PDF Reference Table 8.70 for details.
+            auto_regenerate: set/unset the need_appearances flag ;
+                the flag is unchanged if auto_regenerate is None.
+        """
+        if CatalogDictionary.ACRO_FORM not in self._root_object:
+            raise PyPdfError("No /AcroForm dictionary in PdfWriter Object")
+        af = cast(DictionaryObject, self._root_object[CatalogDictionary.ACRO_FORM])
+        if InteractiveFormDictEntries.Fields not in af:
+            raise PyPdfError("No /Fields dictionary in Pdf in PdfWriter Object")
+        if isinstance(auto_regenerate, bool):
+            self.set_need_appearances_writer(auto_regenerate)
+        # Iterate through pages, update field values
+        if page is None:
+            page = list(self.pages)
+        if isinstance(page, list):
+            for p in page:
+                if PG.ANNOTS in p:  # just to prevent warnings
+                    self.update_page_form_field_values(p, fields, flags, None)
+            return None
+        if PG.ANNOTS not in page:
+            logger_warning("No fields to update on this page", __name__)
+            return
+        for writer_annot in page[PG.ANNOTS]:  # type: ignore
+            writer_annot = cast(DictionaryObject, writer_annot.get_object())
+            if writer_annot.get("/Subtype", "") != "/Widget":
+                continue
+            if "/FT" in writer_annot and "/T" in writer_annot:
+                writer_parent_annot = writer_annot
+            else:
+                writer_parent_annot = writer_annot.get(
+                    PG.PARENT, DictionaryObject()
+                ).get_object()
+
+            for field, value in fields.items():
+                if not (
+                    self._get_qualified_field_name(writer_parent_annot) == field
+                    or writer_parent_annot.get("/T", None) == field
+                ):
+                    continue
+                if flags:
+                    writer_annot[NameObject(FA.Ff)] = NumberObject(flags)
+                if isinstance(value, list):
+                    lst = ArrayObject(TextStringObject(v) for v in value)
+                    writer_parent_annot[NameObject(FA.V)] = lst
+                else:
+                    writer_parent_annot[NameObject(FA.V)] = TextStringObject(value)
+                if writer_parent_annot.get(FA.FT) in ("/Btn"):
+                    # case of Checkbox button (no /FT found in Radio widgets
+                    v = NameObject(value)
+                    if v not in writer_annot[NameObject(AA.AP)][NameObject("/N")]:
+                        v = NameObject("/Off")
+                    # other cases will be updated through the for loop
+                    writer_annot[NameObject(AA.AS)] = v
+                elif (
+                    writer_parent_annot.get(FA.FT) == "/Tx"
+                    or writer_parent_annot.get(FA.FT) == "/Ch"
+                ):
+                    # textbox
+                    self._update_field_annotation(writer_parent_annot, writer_annot)
+                elif (
+                    writer_annot.get(FA.FT) == "/Sig"
+                ):  # deprecated  # not implemented yet
+                    # signature
+                    logger_warning("Signature forms not implemented yet", __name__)
+
+    def reattach_fields(
+        self, page: Optional[PageObject] = None
+    ) -> List[DictionaryObject]:
+        """
+        Parse annotations within the page looking for orphan fields and
+        reattach then into the Fields Structure.
+
+        Args:
+            page: page to analyze.
+                  If none is provided, all pages will be analyzed.
+
+        Returns:
+            list of reattached fields.
+        """
+        lst = []
+        if page is None:
+            for p in self.pages:
+                lst += self.reattach_fields(p)
+            return lst
+
         try:
-            key = cast(str, field["/TM"])
+            af = cast(DictionaryObject, self._root_object[CatalogDictionary.ACRO_FORM])
         except KeyError:
-            try:
-                if "/Parent" in field:
-                    key = (
-                        self._get_qualified_field_name(
-                            cast(DictionaryObject, field["/Parent"])
-                        )
-                        + "."
-                    )
-                else:
-                    key = ""
-                key += cast(str, field["/T"])
-            except KeyError:
-                # Ignore no-name field for now
-                return
-        if fileobj:
-            self._write_field(fileobj, field, field_attributes)
-            fileobj.write("\n")
-        retval[key] = Field(field)
-        obj = retval[key].indirect_reference.get_object()  # to get the full object
-        if obj.get(FA.FT, "") == "/Ch":
-            retval[key][NameObject("/_States_")] = obj[NameObject(FA.Opt)]
-        if obj.get(FA.FT, "") == "/Btn" and "/AP" in obj:
-            #  Checkbox
-            retval[key][NameObject("/_States_")] = ArrayObject(
-                list(obj["/AP"]["/N"].keys())
-            )
-            if "/Off" not in retval[key]["/_States_"]:
-                retval[key][NameObject("/_States_")].append(NameObject("/Off"))
-        elif obj.get(FA.FT, "") == "/Btn" and obj.get(FA.Ff, 0) & FA.FfBits.Radio != 0:
-            states: List[str] = []
-            retval[key][NameObject("/_States_")] = ArrayObject(states)
-            for k in obj.get(FA.Kids, {}):
-                k = k.get_object()
-                for s in list(k["/AP"]["/N"].keys()):
-                    if s not in states:
-                        states.append(s)
-                retval[key][NameObject("/_States_")] = ArrayObject(states)
-            if (
-                obj.get(FA.Ff, 0) & FA.FfBits.NoToggleToOff != 0
-                and "/Off" in retval[key]["/_States_"]
-            ):
-                del retval[key]["/_States_"][retval[key]["/_States_"].index("/Off")]
+            af = DictionaryObject()
+            self._root_object[NameObject(CatalogDictionary.ACRO_FORM)] = af
+        try:
+            fields = cast(ArrayObject, af[InteractiveFormDictEntries.Fields])
+        except KeyError:
+            fields = ArrayObject()
+            af[NameObject(InteractiveFormDictEntries.Fields)] = fields
 
-    def _check_kids(
-        self, tree: Union[TreeObject, DictionaryObject], retval: Any, fileobj: Any
+        if "/Annots" not in page:
+            return lst
+        annots = cast(ArrayObject, page["/Annots"])
+        for idx in range(len(annots)):
+            ano = annots[idx]
+            indirect = isinstance(ano, IndirectObject)
+            ano = cast(DictionaryObject, ano.get_object())
+            if ano.get("/Subtype", "") == "/Widget" and "/FT" in ano:
+                if (
+                    "indirect_reference" in ano.__dict__
+                    and ano.indirect_reference in fields
+                ):
+                    continue
+                if not indirect:
+                    annots[idx] = self._add_object(ano)
+                fields.append(ano.indirect_reference)
+                lst.append(ano)
+        return lst
+
+    def clone_reader_document_root(self, reader: PdfReader) -> None:
+        """
+        Copy the reader document root to the writer and all sub elements,
+        including pages, threads, outlines,... For partial insertion, ``append``
+        should be considered.
+
+        Args:
+            reader: PdfReader from the document root should be copied.
+        """
+        self._objects.clear()
+        self._root_object = reader.root_object.clone(self)
+        self._root = self._root_object.indirect_reference  # type: ignore[assignment]
+        self._pages = self._root_object.raw_get("/Pages")
+        self._flatten()
+        assert self.flattened_pages is not None
+        for p in self.flattened_pages:
+            p[NameObject("/Parent")] = self._pages
+            self._objects[cast(IndirectObject, p.indirect_reference).idnum - 1] = p
+        cast(DictionaryObject, self._pages.get_object())[
+            NameObject("/Kids")
+        ] = ArrayObject([p.indirect_reference for p in self.flattened_pages])
+
+    def clone_document_from_reader(
+        self,
+        reader: PdfReader,
+        after_page_append: Optional[Callable[[PageObject], None]] = None,
     ) -> None:
-        if PA.KIDS in tree:
-            # recurse down the tree
-            for kid in tree[PA.KIDS]:  # type: ignore
-                self.get_fields(kid.get_object(), retval, fileobj)
-
-    def _write_field(self, fileobj: Any, field: Any, field_attributes: Any) -> None:
-        field_attributes_tuple = FA.attributes()
-        field_attributes_tuple = (
-            field_attributes_tuple + CheckboxRadioButtonAttributes.attributes()
-        )
-
-        for attr in field_attributes_tuple:
-            if attr in (
-                FA.Kids,
-                FA.AA,
+        """
+        Create a copy (clone) of a document from a PDF file reader cloning
+        section '/Root' and '/Info' and '/ID' of the pdf.
+
+        Args:
+            reader: PDF file reader instance from which the clone
+                should be created.
+            after_page_append:
+                Callback function that is invoked after each page is appended to
+                the writer. Signature includes a reference to the appended page
+                (delegates to append_pages_from_reader). The single parameter of
+                the callback is a reference to the page just appended to the
+                document.
+        """
+        self.clone_reader_document_root(reader)
+        self._info_obj = self._add_object(DictionaryObject())
+        if TK.INFO in reader.trailer:
+            self._info = reader._info  # actually copy fields
+        try:
+            self._ID = cast(ArrayObject, reader._ID).clone(self)
+        except AttributeError:
+            pass
+        if callable(after_page_append):
+            for page in cast(
+                ArrayObject, cast(DictionaryObject, self._pages.get_object())["/Kids"]
             ):
-                continue
-            attr_name = field_attributes[attr]
-            try:
-                if attr == FA.FT:
-                    # Make the field type value more clear
-                    types = {
-                        "/Btn": "Button",
-                        "/Tx": "Text",
-                        "/Ch": "Choice",
-                        "/Sig": "Signature",
-                    }
-                    if field[attr] in types:
-                        fileobj.write(f"{attr_name}: {types[field[attr]]}\n")
-                elif attr == FA.Parent:
-                    # Let's just write the name of the parent
-                    try:
-                        name = field[attr][FA.TM]
-                    except KeyError:
-                        name = field[attr][FA.T]
-                    fileobj.write(f"{attr_name}: {name}\n")
-                else:
-                    fileobj.write(f"{attr_name}: {field[attr]}\n")
-            except KeyError:
-                # Field attribute is N/A or unknown, so don't write anything
-                pass
+                after_page_append(page.get_object())
+
+    def _compute_document_identifier(self) -> ByteStringObject:
+        stream = BytesIO()
+        self._write_pdf_structure(stream)
+        stream.seek(0)
+        return ByteStringObject(_rolling_checksum(stream).encode("utf8"))
+
+    def generate_file_identifiers(self) -> None:
+        """
+        Generate an identifier for the PDF that will be written.
+
+        The only point of this is ensuring uniqueness. Reproducibility is not
+        required.
+        When a file is first written, both identifiers shall be set to the same value.
+        If both identifiers match when a file reference is resolved, it is very
+        likely that the correct and unchanged file has been found. If only the first
+        identifier matches, a different version of the correct file has been found.
+        see 14.4 "File Identifiers".
+        """
+        if self._ID:
+            id1 = self._ID[0]
+            id2 = self._compute_document_identifier()
+        else:
+            id1 = self._compute_document_identifier()
+            id2 = id1
+        self._ID = ArrayObject((id1, id2))
 
-    def get_form_text_fields(self, full_qualified_name: bool = False) -> Dict[str, Any]:
+    def encrypt(
+        self,
+        user_password: str,
+        owner_password: Optional[str] = None,
+        use_128bit: bool = True,
+        permissions_flag: UserAccessPermissions = ALL_DOCUMENT_PERMISSIONS,
+        *,
+        algorithm: Optional[str] = None,
+    ) -> None:
         """
-        Retrieve form fields from the document with textual data.
+        Encrypt this PDF file with the PDF Standard encryption handler.
 
         Args:
-            full_qualified_name: to get full name
+            user_password: The password which allows for opening
+                and reading the PDF file with the restrictions provided.
+            owner_password: The password which allows for
+                opening the PDF files without any restrictions.  By default,
+                the owner password is the same as the user password.
+            use_128bit: flag as to whether to use 128bit
+                encryption.  When false, 40bit encryption will be used.
+                By default, this flag is on.
+            permissions_flag: permissions as described in
+                TABLE 3.20 of the PDF 1.7 specification. A bit value of 1 means
+                the permission is grantend.
+                Hence an integer value of -1 will set all flags.
+                Bit position 3 is for printing, 4 is for modifying content,
+                5 and 6 control annotations, 9 for form fields,
+                10 for extraction of text and graphics.
+            algorithm: encrypt algorithm. Values may be one of "RC4-40", "RC4-128",
+                "AES-128", "AES-256-R5", "AES-256". If it is valid,
+                `use_128bit` will be ignored.
+        """
+        if owner_password is None:
+            owner_password = user_password
 
-        Returns:
-            A dictionary. The key is the name of the form field,
-            the value is the content of the field.
+        if algorithm is not None:
+            try:
+                alg = getattr(EncryptAlgorithm, algorithm.replace("-", "_"))
+            except AttributeError:
+                raise ValueError(f"algorithm '{algorithm}' NOT supported")
+        else:
+            alg = EncryptAlgorithm.RC4_128
+            if not use_128bit:
+                alg = EncryptAlgorithm.RC4_40
+        self.generate_file_identifiers()
+        assert self._ID
+        self._encryption = Encryption.make(alg, permissions_flag, self._ID[0])
+        # in case call `encrypt` again
+        entry = self._encryption.write_entry(user_password, owner_password)
+        if self._encrypt_entry:
+            # replace old encrypt_entry
+            assert self._encrypt_entry.indirect_reference is not None
+            entry.indirect_reference = self._encrypt_entry.indirect_reference
+            self._objects[entry.indirect_reference.idnum - 1] = entry
+        else:
+            self._add_object(entry)
+        self._encrypt_entry = entry
 
-            If the document contains multiple form fields with the same name, the
-            second and following will get the suffix .2, .3, ...
-        """
+    def write_stream(self, stream: StreamType) -> None:
+        if hasattr(stream, "mode") and "b" not in stream.mode:
+            logger_warning(
+                f"File <{stream.name}> to write to is not in binary mode. "
+                "It may not be written to correctly.",
+                __name__,
+            )
 
-        def indexed_key(k: str, fields: Dict[Any, Any]) -> str:
-            if k not in fields:
-                return k
-            else:
-                return (
-                    k
-                    + "."
-                    + str(sum([1 for kk in fields if kk.startswith(k + ".")]) + 2)
-                )
+        if not self._root:
+            self._root = self._add_object(self._root_object)
 
-        # Retrieve document form fields
-        formfields = self.get_fields()
-        if formfields is None:
-            return {}
-        ff = {}
-        for field, value in formfields.items():
-            if value.get("/FT") == "/Tx":
-                if full_qualified_name:
-                    ff[field] = value.get("/V")
-                else:
-                    ff[indexed_key(cast(str, value["/T"]), ff)] = value.get("/V")
-        return ff
+        self._sweep_indirect_references(self._root)
+
+        object_positions = self._write_pdf_structure(stream)
+        xref_location = self._write_xref_table(stream, object_positions)
+        self._write_trailer(stream, xref_location)
 
-    def get_pages_showing_field(
-        self, field: Union[Field, PdfObject, IndirectObject]
-    ) -> List[PageObject]:
+    def write(self, stream: Union[Path, StrByteType]) -> Tuple[bool, IO[Any]]:
         """
-        Provides list of pages where the field is called.
+        Write the collection of pages added to this object out as a PDF file.
 
         Args:
-            field: Field Object, PdfObject or IndirectObject referencing a Field
+            stream: An object to write the file to. The object can support
+                the write method and the tell method, similar to a file object, or
+                be a file path, just like the fileobj, just named it stream to keep
+                existing workflow.
 
         Returns:
-            List of pages:
-                - Empty list:
-                    The field has no widgets attached
-                    (either hidden field or ancestor field).
-                - Single page list:
-                    Page where the widget is present
-                    (most common).
-                - Multi-page list:
-                    Field with multiple kids widgets
-                    (example: radio buttons, field repeated on multiple pages).
-        """
-
-        def _get_inherited(obj: DictionaryObject, key: str) -> Any:
-            if key in obj:
-                return obj[key]
-            elif "/Parent" in obj:
-                return _get_inherited(
-                    cast(DictionaryObject, obj["/Parent"].get_object()), key
-                )
-            else:
-                return None
+            A tuple (bool, IO)
+        """
+        my_file = False
 
-        try:
-            # to cope with all types
-            field = cast(DictionaryObject, field.indirect_reference.get_object())  # type: ignore
-        except Exception as exc:
-            raise ValueError("field type is invalid") from exc
-        if _get_inherited(field, "/FT") is None:
-            raise ValueError("field is not valid")
-        ret = []
-        if field.get("/Subtype", "") == "/Widget":
-            if "/P" in field:
-                ret = [field["/P"].get_object()]
-            else:
-                ret = [
-                    p
-                    for p in self.pages
-                    if field.indirect_reference in p.get("/Annots", "")
-                ]
-        else:
-            kids = field.get("/Kids", ())
-            for k in kids:
-                k = k.get_object()
-                if (k.get("/Subtype", "") == "/Widget") and ("/T" not in k):
-                    # Kid that is just a widget, not a field:
-                    if "/P" in k:
-                        ret += [k["/P"].get_object()]
-                    else:
-                        ret += [
-                            p
-                            for p in self.pages
-                            if k.indirect_reference in p.get("/Annots", "")
-                        ]
-        return [
-            x
-            if isinstance(x, PageObject)
-            else (self.pages[self._get_page_number_by_indirect(x.indirect_reference)])  # type: ignore
-            for x in ret
-        ]
+        if stream == "":
+            raise ValueError(f"Output(stream={stream}) is empty.")
 
-    def _get_named_destinations(
-        self,
-        tree: Union[TreeObject, None] = None,
-        retval: Optional[Any] = None,
-    ) -> Dict[str, Any]:
+        if isinstance(stream, (str, Path)):
+            stream = FileIO(stream, "wb")
+            self.with_as_usage = True  #
+            my_file = True
+
+        self.write_stream(stream)
+
+        if self.with_as_usage:
+            stream.close()
+
+        return my_file, stream
+
+    def _write_pdf_structure(self, stream: StreamType) -> List[int]:
+        object_positions = []
+        stream.write(self.pdf_header.encode() + b"\n")
+        stream.write(b"%\xE2\xE3\xCF\xD3\n")
+
+        for i, obj in enumerate(self._objects):
+            if obj is not None:
+                idnum = i + 1
+                object_positions.append(stream.tell())
+                stream.write(f"{idnum} 0 obj\n".encode())
+                if self._encryption and obj != self._encrypt_entry:
+                    obj = self._encryption.encrypt_object(obj, idnum, 0)
+                obj.write_to_stream(stream)
+                stream.write(b"\nendobj\n")
+        return object_positions
+
+    def _write_xref_table(self, stream: StreamType, object_positions: List[int]) -> int:
+        xref_location = stream.tell()
+        stream.write(b"xref\n")
+        stream.write(f"0 {len(self._objects) + 1}\n".encode())
+        stream.write(f"{0:0>10} {65535:0>5} f \n".encode())
+        for offset in object_positions:
+            stream.write(f"{offset:0>10} {0:0>5} n \n".encode())
+        return xref_location
+
+    def _write_trailer(self, stream: StreamType, xref_location: int) -> None:
+        """
+        Write the PDF trailer to the stream.
+
+        To quote the PDF specification:
+            [The] trailer [gives] the location of the cross-reference table and
+            of certain special objects within the body of the file.
+        """
+        stream.write(b"trailer\n")
+        trailer = DictionaryObject()
+        trailer.update(
+            {
+                NameObject(TK.SIZE): NumberObject(len(self._objects) + 1),
+                NameObject(TK.ROOT): self._root,
+                NameObject(TK.INFO): self._info_obj,
+            }
+        )
+        if self._ID:
+            trailer[NameObject(TK.ID)] = self._ID
+        if self._encrypt_entry:
+            trailer[NameObject(TK.ENCRYPT)] = self._encrypt_entry.indirect_reference
+        trailer.write_to_stream(stream)
+        stream.write(f"\nstartxref\n{xref_location}\n%%EOF\n".encode())  # eof
+
+    def add_metadata(self, infos: Dict[str, Any]) -> None:
         """
-        Retrieve the named destinations present in the document.
+        Add custom metadata to the output.
 
         Args:
-            tree:
-            retval:
+            infos: a Python dictionary where each key is a field
+                and each value is your new metadata.
+        """
+        args = {}
+        if isinstance(infos, PdfObject):
+            infos = cast(DictionaryObject, infos.get_object())
+        for key, value in list(infos.items()):
+            if isinstance(value, PdfObject):
+                value = value.get_object()
+            args[NameObject(key)] = create_string_object(str(value))
+        assert isinstance(self._info, DictionaryObject)
+        self._info.update(args)
 
-        Returns:
-            A dictionary which maps names to
-            :class:`Destinations<pypdf.generic.Destination>`.
+    def _sweep_indirect_references(
+        self,
+        root: Union[
+            ArrayObject,
+            BooleanObject,
+            DictionaryObject,
+            FloatObject,
+            IndirectObject,
+            NameObject,
+            PdfObject,
+            NumberObject,
+            TextStringObject,
+            NullObject,
+        ],
+    ) -> None:
         """
-        if retval is None:
-            retval = {}
-            catalog = cast(DictionaryObject, self.trailer[TK.ROOT])
-
-            # get the name tree
-            if CA.DESTS in catalog:
-                tree = cast(TreeObject, catalog[CA.DESTS])
-            elif CA.NAMES in catalog:
-                names = cast(DictionaryObject, catalog[CA.NAMES])
-                if CA.DESTS in names:
-                    tree = cast(TreeObject, names[CA.DESTS])
-
-        if tree is None:
-            return retval
-
-        if PA.KIDS in tree:
-            # recurse down the tree
-            for kid in cast(ArrayObject, tree[PA.KIDS]):
-                self._get_named_destinations(kid.get_object(), retval)
-        # TABLE 3.33 Entries in a name tree node dictionary (PDF 1.7 specs)
-        elif CA.NAMES in tree:  # KIDS and NAMES are exclusives (PDF 1.7 specs p 162)
-            names = cast(DictionaryObject, tree[CA.NAMES])
-            i = 0
-            while i < len(names):
-                key = cast(str, names[i].get_object())
-                i += 1
-                if not isinstance(key, str):
-                    continue
-                try:
-                    value = names[i].get_object()
-                except IndexError:
-                    break
-                i += 1
-                if isinstance(value, DictionaryObject):
-                    if "/D" in value:
-                        value = value["/D"]
-                    else:
-                        continue
-                dest = self._build_destination(key, value)  # type: ignore
-                if dest is not None:
-                    retval[key] = dest
-        else:  # case where Dests is in root catalog (PDF 1.7 specs, §2 about PDF1.1
-            for k__, v__ in tree.items():
-                val = v__.get_object()
-                if isinstance(val, DictionaryObject):
-                    if "/D" in val:
-                        val = val["/D"].get_object()
-                    else:
-                        continue
-                dest = self._build_destination(k__, val)
-                if dest is not None:
-                    retval[k__] = dest
-        return retval
+        Resolving any circular references to Page objects.
 
-    @property
-    def outline(self) -> OutlineType:
+        Circular references to Page objects can arise when objects such as
+        annotations refer to their associated page. If these references are not
+        properly handled, the PDF file will contain multiple copies of the same
+        Page object. To address this problem, Page objects store their original
+        object reference number. This method adds the reference number of any
+        circularly referenced Page objects to an external reference map. This
+        ensures that self-referencing trees reference the correct new object
+        location, rather than copying in a new copy of the Page object.
+
+        Args:
+            root: The root of the PDF object tree to sweep.
         """
-        Read-only property for the outline present in the document.
+        stack: Deque[
+            Tuple[
+                Any,
+                Optional[Any],
+                Any,
+                List[PdfObject],
+            ]
+        ] = collections.deque()
+        discovered = []
+        parent = None
+        grant_parents: List[PdfObject] = []
+        key_or_id = None
+
+        # Start from root
+        stack.append((root, parent, key_or_id, grant_parents))
+
+        while len(stack):
+            data, parent, key_or_id, grant_parents = stack.pop()
+
+            # Build stack for a processing depth-first
+            if isinstance(data, (ArrayObject, DictionaryObject)):
+                for key, value in data.items():
+                    stack.append(
+                        (
+                            value,
+                            data,
+                            key,
+                            grant_parents + [parent] if parent is not None else [],
+                        )
+                    )
+            elif isinstance(data, IndirectObject) and data.pdf != self:
+                data = self._resolve_indirect_object(data)
+
+                if str(data) not in discovered:
+                    discovered.append(str(data))
+                    stack.append((data.get_object(), None, None, []))
+
+            # Check if data has a parent and if it is a dict or
+            # an array update the value
+            if isinstance(parent, (DictionaryObject, ArrayObject)):
+                if isinstance(data, StreamObject):
+                    # a dictionary value is a stream.  streams must be indirect
+                    # objects, so we need to change this value.
+                    data = self._resolve_indirect_object(self._add_object(data))
+
+                update_hashes = []
+
+                # Data changed and thus the hash value changed
+                if parent[key_or_id] != data:
+                    update_hashes = [parent.hash_value()] + [
+                        grant_parent.hash_value() for grant_parent in grant_parents
+                    ]
+                    parent[key_or_id] = data
+
+                # Update old hash value to new hash value
+                for old_hash in update_hashes:
+                    indirect_reference = self._idnum_hash.pop(old_hash, None)
+
+                    if indirect_reference is not None:
+                        indirect_reference_obj = indirect_reference.get_object()
+
+                        if indirect_reference_obj is not None:
+                            self._idnum_hash[
+                                indirect_reference_obj.hash_value()
+                            ] = indirect_reference
+
+    def _resolve_indirect_object(self, data: IndirectObject) -> IndirectObject:
+        """
+        Resolves an indirect object to an indirect object in this PDF file.
+
+        If the input indirect object already belongs to this PDF file, it is
+        returned directly. Otherwise, the object is retrieved from the input
+        object's PDF file using the object's ID number and generation number. If
+        the object cannot be found, a warning is logged and a `NullObject` is
+        returned.
+
+        If the object is not already in this PDF file, it is added to the file's
+        list of objects and assigned a new ID number and generation number of 0.
+        The hash value of the object is then added to the `_idnum_hash`
+        dictionary, with the corresponding `IndirectObject` reference as the
+        value.
+
+        Args:
+            data: The `IndirectObject` to resolve.
+
+        Returns:
+            The resolved `IndirectObject` in this PDF file.
 
-        (i.e., a collection of 'outline items' which are also known as
-        'bookmarks')
+        Raises:
+            ValueError: If the input stream is closed.
         """
-        return self._get_outline()
+        if hasattr(data.pdf, "stream") and data.pdf.stream.closed:
+            raise ValueError(f"I/O operation on closed file: {data.pdf.stream.name}")
+
+        if data.pdf == self:
+            return data
 
-    def _get_outline(
-        self, node: Optional[DictionaryObject] = None, outline: Optional[Any] = None
-    ) -> OutlineType:
-        if outline is None:
-            outline = []
-            catalog = cast(DictionaryObject, self.trailer[TK.ROOT])
+        # Get real object indirect object
+        real_obj = data.pdf.get_object(data)
 
-            # get the outline dictionary and named destinations
-            if CO.OUTLINES in catalog:
-                lines = cast(DictionaryObject, catalog[CO.OUTLINES])
+        if real_obj is None:
+            logger_warning(
+                f"Unable to resolve [{data.__class__.__name__}: {data}], "
+                "returning NullObject instead",
+                __name__,
+            )
+            real_obj = NullObject()
 
-                if isinstance(lines, NullObject):
-                    return outline
+        hash_value = real_obj.hash_value()
 
-                # TABLE 8.3 Entries in the outline dictionary
-                if lines is not None and "/First" in lines:
-                    node = cast(DictionaryObject, lines["/First"])
-            self._namedDests = self._get_named_destinations()
+        # Check if object is handled
+        if hash_value in self._idnum_hash:
+            return self._idnum_hash[hash_value]
 
-        if node is None:
-            return outline
+        if data.pdf == self:
+            self._idnum_hash[hash_value] = IndirectObject(data.idnum, 0, self)
+        # This is new object in this pdf
+        else:
+            self._idnum_hash[hash_value] = self._add_object(real_obj)
+
+        return self._idnum_hash[hash_value]
 
-        # see if there are any more outline items
-        while True:
-            outline_obj = self._build_outline_item(node)
-            if outline_obj:
-                outline.append(outline_obj)
-
-            # check for sub-outline
-            if "/First" in node:
-                sub_outline: List[Any] = []
-                self._get_outline(cast(DictionaryObject, node["/First"]), sub_outline)
-                if sub_outline:
-                    outline.append(sub_outline)
-
-            if "/Next" not in node:
-                break
-            node = cast(DictionaryObject, node["/Next"])
+    def get_reference(self, obj: PdfObject) -> IndirectObject:
+        idnum = self._objects.index(obj) + 1
+        ref = IndirectObject(idnum, 0, self)
+        assert ref.get_object() == obj
+        return ref
+
+    def get_outline_root(self) -> TreeObject:
+        if CO.OUTLINES in self._root_object:
+            # TABLE 3.25 Entries in the catalog dictionary
+            outline = cast(TreeObject, self._root_object[CO.OUTLINES])
+            if not isinstance(outline, TreeObject):
+                t = TreeObject(outline)
+                self._replace_object(outline.indirect_reference.idnum, t)
+                outline = t
+            idnum = self._objects.index(outline) + 1
+            outline_ref = IndirectObject(idnum, 0, self)
+            assert outline_ref.get_object() == outline
+        else:
+            outline = TreeObject()
+            outline.update({})
+            outline_ref = self._add_object(outline)
+            self._root_object[NameObject(CO.OUTLINES)] = outline_ref
 
         return outline
 
+    def get_threads_root(self) -> ArrayObject:
+        """
+        The list of threads.
+
+        See §12.4.3 of the PDF 1.7 or PDF 2.0 specification.
+
+        Returns:
+            An array (possibly empty) of Dictionaries with ``/F`` and
+            ``/I`` properties.
+        """
+        if CO.THREADS in self._root_object:
+            # TABLE 3.25 Entries in the catalog dictionary
+            threads = cast(ArrayObject, self._root_object[CO.THREADS])
+        else:
+            threads = ArrayObject()
+            self._root_object[NameObject(CO.THREADS)] = threads
+        return threads
+
     @property
-    def threads(self) -> Optional[ArrayObject]:
+    def threads(self) -> ArrayObject:
         """
         Read-only property for the list of threads.
 
         See §8.3.2 from PDF 1.7 spec.
 
-        It's an array of dictionaries with "/F" and "/I" properties or
-        None if there are no articles.
+        Each element is a dictionaries with ``/F`` and ``/I`` keys.
         """
-        catalog = cast(DictionaryObject, self.trailer[TK.ROOT])
-        if CO.THREADS in catalog:
-            return cast("ArrayObject", catalog[CO.THREADS])
-        else:
-            return None
+        return self.get_threads_root()
 
-    def _get_page_number_by_indirect(
-        self, indirect_reference: Union[None, int, NullObject, IndirectObject]
-    ) -> Optional[int]:
+    def add_outline_item_destination(
+        self,
+        page_destination: Union[IndirectObject, PageObject, TreeObject],
+        parent: Union[None, TreeObject, IndirectObject] = None,
+        before: Union[None, TreeObject, IndirectObject] = None,
+        is_open: bool = True,
+    ) -> IndirectObject:
+        page_destination = cast(PageObject, page_destination.get_object())
+        if isinstance(page_destination, PageObject):
+            return self.add_outline_item_destination(
+                Destination(
+                    f"page #{page_destination.page_number}",
+                    cast(IndirectObject, page_destination.indirect_reference),
+                    Fit.fit(),
+                )
+            )
+
+        if parent is None:
+            parent = self.get_outline_root()
+
+        page_destination[NameObject("/%is_open%")] = BooleanObject(is_open)
+        parent = cast(TreeObject, parent.get_object())
+        page_destination_ref = self._add_object(page_destination)
+        if before is not None:
+            before = before.indirect_reference
+        parent.insert_child(
+            page_destination_ref,
+            before,
+            self,
+            page_destination.inc_parent_counter_outline
+            if is_open
+            else (lambda x, y: 0),
+        )
+        if "/Count" not in page_destination:
+            page_destination[NameObject("/Count")] = NumberObject(0)
+
+        return page_destination_ref
+
+    def add_outline_item_dict(
+        self,
+        outline_item: OutlineItemType,
+        parent: Union[None, TreeObject, IndirectObject] = None,
+        before: Union[None, TreeObject, IndirectObject] = None,
+        is_open: bool = True,
+    ) -> IndirectObject:
+        outline_item_object = TreeObject()
+        outline_item_object.update(outline_item)
+
+        if "/A" in outline_item:
+            action = DictionaryObject()
+            a_dict = cast(DictionaryObject, outline_item["/A"])
+            for k, v in list(a_dict.items()):
+                action[NameObject(str(k))] = v
+            action_ref = self._add_object(action)
+            outline_item_object[NameObject("/A")] = action_ref
+
+        return self.add_outline_item_destination(
+            outline_item_object, parent, before, is_open
+        )
+
+    def add_outline_item(
+        self,
+        title: str,
+        page_number: Union[None, PageObject, IndirectObject, int],
+        parent: Union[None, TreeObject, IndirectObject] = None,
+        before: Union[None, TreeObject, IndirectObject] = None,
+        color: Optional[Union[Tuple[float, float, float], str]] = None,
+        bold: bool = False,
+        italic: bool = False,
+        fit: Fit = PAGE_FIT,
+        is_open: bool = True,
+    ) -> IndirectObject:
         """
-        Generate _page_id2num.
+        Add an outline item (commonly referred to as a "Bookmark") to the PDF file.
 
         Args:
-            indirect_reference:
+            title: Title to use for this outline item.
+            page_number: Page number this outline item will point to.
+            parent: A reference to a parent outline item to create nested
+                outline items.
+            before:
+            color: Color of the outline item's font as a red, green, blue tuple
+                from 0.0 to 1.0 or as a Hex String (#RRGGBB)
+            bold: Outline item font is bold
+            italic: Outline item font is italic
+            fit: The fit of the destination page.
 
         Returns:
-            The page number or None
+            The added outline item as an indirect object.
         """
-        if self._page_id2num is None:
-            self._page_id2num = {
-                x.indirect_reference.idnum: i for i, x in enumerate(self.pages)  # type: ignore
+        page_ref: Union[None, NullObject, IndirectObject, NumberObject]
+        if isinstance(italic, Fit):  # it means that we are on the old params
+            if fit is not None and page_number is None:
+                page_number = fit  # type: ignore
+            return self.add_outline_item(
+                title, page_number, parent, None, before, color, bold, italic, is_open=is_open  # type: ignore
+            )
+        if page_number is None:
+            action_ref = None
+        else:
+            if isinstance(page_number, IndirectObject):
+                page_ref = page_number
+            elif isinstance(page_number, PageObject):
+                page_ref = page_number.indirect_reference
+            elif isinstance(page_number, int):
+                try:
+                    page_ref = self.pages[page_number].indirect_reference
+                except IndexError:
+                    page_ref = NumberObject(page_number)
+            if page_ref is None:
+                logger_warning(
+                    f"can not find reference of page {page_number}",
+                    __name__,
+                )
+                page_ref = NullObject()
+            dest = Destination(
+                NameObject("/" + title + " outline item"),
+                page_ref,
+                fit,
+            )
+
+            action_ref = self._add_object(
+                DictionaryObject(
+                    {
+                        NameObject(GoToActionArguments.D): dest.dest_array,
+                        NameObject(GoToActionArguments.S): NameObject("/GoTo"),
+                    }
+                )
+            )
+        outline_item = self._add_object(
+            _create_outline_item(action_ref, title, color, italic, bold)
+        )
+
+        if parent is None:
+            parent = self.get_outline_root()
+        return self.add_outline_item_destination(outline_item, parent, before, is_open)
+
+    def add_outline(self) -> None:
+        raise NotImplementedError(
+            "This method is not yet implemented. Use :meth:`add_outline_item` instead."
+        )
+
+    def add_named_destination_array(
+        self, title: TextStringObject, destination: Union[IndirectObject, ArrayObject]
+    ) -> None:
+        named_dest = self.get_named_dest_root()
+        i = 0
+        while i < len(named_dest):
+            if title < named_dest[i]:
+                named_dest.insert(i, destination)
+                named_dest.insert(i, TextStringObject(title))
+                return
+            else:
+                i += 2
+        named_dest.extend([TextStringObject(title), destination])
+        return
+
+    def add_named_destination_object(
+        self,
+        page_destination: PdfObject,
+    ) -> IndirectObject:
+        page_destination_ref = self._add_object(page_destination.dest_array)  # type: ignore
+        self.add_named_destination_array(
+            cast("TextStringObject", page_destination["/Title"]), page_destination_ref  # type: ignore
+        )
+
+        return page_destination_ref
+
+    def add_named_destination(
+        self,
+        title: str,
+        page_number: int,
+    ) -> IndirectObject:
+        page_ref = self.get_object(self._pages)[PA.KIDS][page_number]  # type: ignore
+        dest = DictionaryObject()
+        dest.update(
+            {
+                NameObject(GoToActionArguments.D): ArrayObject(
+                    [page_ref, NameObject(TypFitArguments.FIT_H), NumberObject(826)]
+                ),
+                NameObject(GoToActionArguments.S): NameObject("/GoTo"),
             }
+        )
 
-        if indirect_reference is None or isinstance(indirect_reference, NullObject):
-            return None
-        if isinstance(indirect_reference, int):
-            idnum = indirect_reference
-        else:
-            idnum = indirect_reference.idnum
-        assert self._page_id2num is not None, "hint for mypy"
-        ret = self._page_id2num.get(idnum, None)
-        return ret
+        dest_ref = self._add_object(dest)
+        if not isinstance(title, TextStringObject):
+            title = TextStringObject(str(title))
+
+        self.add_named_destination_array(title, dest_ref)
+        return dest_ref
+
+    def remove_links(self) -> None:
+        """Remove links and annotations from this output."""
+        for page in self.pages:
+            self.remove_objects_from_page(page, ObjectDeletionFlag.ALL_ANNOTATIONS)
 
-    def get_page_number(self, page: PageObject) -> Optional[int]:
+    def remove_annotations(
+        self, subtypes: Optional[Union[AnnotationSubtype, Iterable[AnnotationSubtype]]]
+    ) -> None:
         """
-        Retrieve page number of a given PageObject.
+        Remove annotations by annotation subtype.
 
         Args:
-            page: The page to get page number. Should be
-                an instance of :class:`PageObject<pypdf._page.PageObject>`
-
-        Returns:
-            The page number or None if page is not found
+            subtypes: SubType or list of SubTypes to be removed.
+                Examples are: "/Link", "/FileAttachment", "/Sound",
+                "/Movie", "/Screen", ...
+                If you want to remove all annotations, use subtypes=None.
         """
-        return self._get_page_number_by_indirect(page.indirect_reference)
+        for page in self.pages:
+            self._remove_annots_from_page(page, subtypes)
+
+    def _remove_annots_from_page(
+        self,
+        page: Union[IndirectObject, PageObject, DictionaryObject],
+        subtypes: Optional[Iterable[str]],
+    ) -> None:
+        page = cast(DictionaryObject, page.get_object())
+        if PG.ANNOTS in page:
+            i = 0
+            while i < len(cast(ArrayObject, page[PG.ANNOTS])):
+                an = cast(ArrayObject, page[PG.ANNOTS])[i]
+                obj = cast(DictionaryObject, an.get_object())
+                if subtypes is None or cast(str, obj["/Subtype"]) in subtypes:
+                    if isinstance(an, IndirectObject):
+                        self._objects[an.idnum - 1] = NullObject()  # to reduce PDF size
+                    del page[PG.ANNOTS][i]  # type:ignore
+                else:
+                    i += 1
 
-    def get_destination_page_number(self, destination: Destination) -> Optional[int]:
+    def remove_objects_from_page(
+        self,
+        page: Union[PageObject, DictionaryObject],
+        to_delete: Union[ObjectDeletionFlag, Iterable[ObjectDeletionFlag]],
+    ) -> None:
         """
-        Retrieve page number of a given Destination object.
+        Remove objects specified by ``to_delete`` from the given page.
 
         Args:
-            destination: The destination to get page number.
+            page: Page object to clean up.
+            to_delete: Objects to be deleted; can be a ``ObjectDeletionFlag``
+                or a list of ObjectDeletionFlag
+        """
+        if isinstance(to_delete, (list, tuple)):
+            for to_d in to_delete:
+                self.remove_objects_from_page(page, to_d)
+            return
+        assert isinstance(to_delete, ObjectDeletionFlag)
+
+        if to_delete & ObjectDeletionFlag.LINKS:
+            return self._remove_annots_from_page(page, ("/Link",))
+        if to_delete & ObjectDeletionFlag.ATTACHMENTS:
+            return self._remove_annots_from_page(
+                page, ("/FileAttachment", "/Sound", "/Movie", "/Screen")
+            )
+        if to_delete & ObjectDeletionFlag.OBJECTS_3D:
+            return self._remove_annots_from_page(page, ("/3D",))
+        if to_delete & ObjectDeletionFlag.ALL_ANNOTATIONS:
+            return self._remove_annots_from_page(page, None)
+
+        jump_operators = []
+        if to_delete & ObjectDeletionFlag.DRAWING_IMAGES:
+            jump_operators = (
+                [b"w", b"J", b"j", b"M", b"d", b"i"]
+                + [b"W", b"W*"]
+                + [b"b", b"b*", b"B", b"B*", b"S", b"s", b"f", b"f*", b"F", b"n"]
+                + [b"m", b"l", b"c", b"v", b"y", b"h", b"re"]
+                + [b"sh"]
+            )
+        if to_delete & ObjectDeletionFlag.TEXT:
+            jump_operators = [b"Tj", b"TJ", b"'", b'"']
 
-        Returns:
-            The page number or None if page is not found
+        def clean(content: ContentStream, images: List[str], forms: List[str]) -> None:
+            nonlocal jump_operators, to_delete
+            i = 0
+            while i < len(content.operations):
+                operands, operator = content.operations[i]
+                if (
+                    (
+                        operator == b"INLINE IMAGE"
+                        and (to_delete & ObjectDeletionFlag.INLINE_IMAGES)
+                    )
+                    or (operator in jump_operators)
+                    or (
+                        operator == b"Do"
+                        and (to_delete & ObjectDeletionFlag.XOBJECT_IMAGES)
+                        and (operands[0] in images)
+                    )
+                ):
+                    del content.operations[i]
+                else:
+                    i += 1
+            content.get_data()  # this ensures ._data is rebuilt from the .operations
+
+        def clean_forms(
+            elt: DictionaryObject, stack: List[DictionaryObject]
+        ) -> Tuple[List[str], List[str]]:
+            nonlocal to_delete
+            # elt in recursive call is a new ContentStream object, so we have to check the indirect_reference
+            if (elt in stack) or (
+                hasattr(elt, "indirect_reference")
+                and any(
+                    elt.indirect_reference == getattr(x, "indirect_reference", -1)
+                    for x in stack
+                )
+            ):
+                # to prevent infinite looping
+                return [], []  # pragma: no cover
+            try:
+                d = cast(
+                    Dict[Any, Any],
+                    cast(DictionaryObject, elt["/Resources"])["/XObject"],
+                )
+            except KeyError:
+                d = {}
+            images = []
+            forms = []
+            for k, v in d.items():
+                o = v.get_object()
+                try:
+                    content: Any = None
+                    if (
+                        to_delete & ObjectDeletionFlag.XOBJECT_IMAGES
+                        and o["/Subtype"] == "/Image"
+                    ):
+                        content = NullObject()  # to delete the image keeping the entry
+                        images.append(k)
+                    if o["/Subtype"] == "/Form":
+                        forms.append(k)
+                        if isinstance(o, ContentStream):
+                            content = o
+                        else:
+                            content = ContentStream(o, self)
+                            content.update(
+                                {
+                                    k1: v1
+                                    for k1, v1 in o.items()
+                                    if k1 not in ["/Length", "/Filter", "/DecodeParms"]
+                                }
+                            )
+                            try:
+                                content.indirect_reference = o.indirect_reference
+                            except AttributeError:  # pragma: no cover
+                                pass
+                        stack.append(elt)
+                        clean_forms(content, stack)  # clean subforms
+                    if content is not None:
+                        if isinstance(v, IndirectObject):
+                            self._objects[v.idnum - 1] = content
+                        else:
+                            # should only occur with pdf not respecting pdf spec
+                            # where streams must be indirected.
+                            d[k] = self._add_object(content)  # pragma: no cover
+                except (TypeError, KeyError):
+                    pass
+            for im in images:
+                del d[im]  # for clean-up
+            if isinstance(elt, StreamObject):  # for /Form
+                if not isinstance(elt, ContentStream):  # pragma: no cover
+                    e = ContentStream(elt, self)
+                    e.update(elt.items())
+                    elt = e
+                clean(elt, images, forms)  # clean the content
+            return images, forms
+
+        if not isinstance(page, PageObject):
+            page = PageObject(self, page.indirect_reference)  # pragma: no cover
+        if "/Contents" in page:
+            content = cast(ContentStream, page.get_contents())
+
+            images, forms = clean_forms(page, [])
+
+            clean(content, images, forms)
+            page.replace_contents(content)
+
+    def remove_images(
+        self,
+        to_delete: ImageType = ImageType.ALL,
+    ) -> None:
+        """
+        Remove images from this output.
+
+        Args:
+            to_delete : The type of images to be deleted
+                (default = all images types)
         """
-        return self._get_page_number_by_indirect(destination.page)
+        if isinstance(to_delete, bool):
+            to_delete = ImageType.ALL
+        i = (
+            (
+                ObjectDeletionFlag.XOBJECT_IMAGES
+                if to_delete & ImageType.XOBJECT_IMAGES
+                else ObjectDeletionFlag.NONE
+            )
+            | (
+                ObjectDeletionFlag.INLINE_IMAGES
+                if to_delete & ImageType.INLINE_IMAGES
+                else ObjectDeletionFlag.NONE
+            )
+            | (
+                ObjectDeletionFlag.DRAWING_IMAGES
+                if to_delete & ImageType.DRAWING_IMAGES
+                else ObjectDeletionFlag.NONE
+            )
+        )
+        for page in self.pages:
+            self.remove_objects_from_page(page, i)
+
+    def remove_text(self) -> None:
+        """Remove text from this output."""
+        for page in self.pages:
+            self.remove_objects_from_page(page, ObjectDeletionFlag.TEXT)
 
-    def _build_destination(
+    def add_uri(
         self,
-        title: str,
-        array: Optional[
-            List[
-                Union[NumberObject, IndirectObject, None, NullObject, DictionaryObject]
-            ]
-        ],
-    ) -> Destination:
-        page, typ = None, None
-        # handle outline items with missing or invalid destination
-        if (
-            isinstance(array, (NullObject, str))
-            or (isinstance(array, ArrayObject) and len(array) == 0)
-            or array is None
-        ):
-            page = NullObject()
-            return Destination(title, page, Fit.fit())
+        page_number: int,
+        uri: str,
+        rect: RectangleObject,
+        border: Optional[ArrayObject] = None,
+    ) -> None:
+        """
+        Add an URI from a rectangular area to the specified page.
+
+        Args:
+            page_number: index of the page on which to place the URI action.
+            uri: URI of resource to link to.
+            rect: :class:`RectangleObject<pypdf.generic.RectangleObject>` or
+                array of four integers specifying the clickable rectangular area
+                ``[xLL, yLL, xUR, yUR]``, or string in the form
+                ``"[ xLL yLL xUR yUR ]"``.
+            border: if provided, an array describing border-drawing
+                properties. See the PDF spec for details. No border will be
+                drawn if this argument is omitted.
+        """
+        page_link = self.get_object(self._pages)[PA.KIDS][page_number]  # type: ignore
+        page_ref = cast(Dict[str, Any], self.get_object(page_link))
+
+        border_arr: BorderArrayType
+        if border is not None:
+            border_arr = [NumberObject(n) for n in border[:3]]
+            if len(border) == 4:
+                dash_pattern = ArrayObject([NumberObject(n) for n in border[3]])
+                border_arr.append(dash_pattern)
         else:
-            page, typ = array[0:2]  # type: ignore
-            array = array[2:]
-            try:
-                return Destination(title, page, Fit(fit_type=typ, fit_args=array))  # type: ignore
-            except PdfReadError:
-                logger_warning(f"Unknown destination: {title} {array}", __name__)
-                if self.strict:
-                    raise
-                # create a link to first Page
-                tmp = self.pages[0].indirect_reference
-                indirect_reference = NullObject() if tmp is None else tmp
-                return Destination(title, indirect_reference, Fit.fit())  # type: ignore
+            border_arr = [NumberObject(2), NumberObject(2), NumberObject(2)]
+
+        if isinstance(rect, str):
+            rect = NumberObject(rect)
+        elif isinstance(rect, RectangleObject):
+            pass
+        else:
+            rect = RectangleObject(rect)
+
+        lnk2 = DictionaryObject()
+        lnk2.update(
+            {
+                NameObject("/S"): NameObject("/URI"),
+                NameObject("/URI"): TextStringObject(uri),
+            }
+        )
+        lnk = DictionaryObject()
+        lnk.update(
+            {
+                NameObject(AA.Type): NameObject("/Annot"),
+                NameObject(AA.Subtype): NameObject("/Link"),
+                NameObject(AA.P): page_link,
+                NameObject(AA.Rect): rect,
+                NameObject("/H"): NameObject("/I"),
+                NameObject(AA.Border): ArrayObject(border_arr),
+                NameObject("/A"): lnk2,
+            }
+        )
+        lnk_ref = self._add_object(lnk)
+
+        if PG.ANNOTS in page_ref:
+            page_ref[PG.ANNOTS].append(lnk_ref)
+        else:
+            page_ref[NameObject(PG.ANNOTS)] = ArrayObject([lnk_ref])
 
-    def _build_outline_item(self, node: DictionaryObject) -> Optional[Destination]:
-        dest, title, outline_item = None, None, None
+    _valid_layouts = (
+        "/NoLayout",
+        "/SinglePage",
+        "/OneColumn",
+        "/TwoColumnLeft",
+        "/TwoColumnRight",
+        "/TwoPageLeft",
+        "/TwoPageRight",
+    )
 
-        # title required for valid outline
-        # PDF Reference 1.7: TABLE 8.4 Entries in an outline item dictionary
+    def _get_page_layout(self) -> Optional[LayoutType]:
         try:
-            title = cast("str", node["/Title"])
+            return cast(LayoutType, self._root_object["/PageLayout"])
         except KeyError:
-            if self.strict:
-                raise PdfReadError(f"Outline Entry Missing /Title attribute: {node!r}")
-            title = ""
-
-        if "/A" in node:
-            # Action, PDFv1.7 Section 12.6 (only type GoTo supported)
-            action = cast(DictionaryObject, node["/A"])
-            action_type = cast(NameObject, action[GoToActionArguments.S])
-            if action_type == "/GoTo":
-                dest = action[GoToActionArguments.D]
-        elif "/Dest" in node:
-            # Destination, PDFv1.7 Section 12.3.2
-            dest = node["/Dest"]
-            # if array was referenced in another object, will be a dict w/ key "/D"
-            if isinstance(dest, DictionaryObject) and "/D" in dest:
-                dest = dest["/D"]
+            return None
 
-        if isinstance(dest, ArrayObject):
-            outline_item = self._build_destination(title, dest)
-        elif isinstance(dest, str):
-            # named destination, addresses NameObject Issue #193
-            # TODO : keep named destination instead of replacing it ?
-            try:
-                outline_item = self._build_destination(
-                    title, self._namedDests[dest].dest_array
-                )
-            except KeyError:
-                # named destination not found in Name Dict
-                outline_item = self._build_destination(title, None)
-        elif dest is None:
-            # outline item not required to have destination or action
-            # PDFv1.7 Table 153
-            outline_item = self._build_destination(title, dest)
-        else:
-            if self.strict:
-                raise PdfReadError(f"Unexpected destination {dest!r}")
-            else:
+    def _set_page_layout(self, layout: Union[NameObject, LayoutType]) -> None:
+        """
+        Set the page layout.
+
+        Args:
+            layout: The page layout to be used.
+
+        .. list-table:: Valid ``layout`` arguments
+           :widths: 50 200
+
+           * - /NoLayout
+             - Layout explicitly not specified
+           * - /SinglePage
+             - Show one page at a time
+           * - /OneColumn
+             - Show one column at a time
+           * - /TwoColumnLeft
+             - Show pages in two columns, odd-numbered pages on the left
+           * - /TwoColumnRight
+             - Show pages in two columns, odd-numbered pages on the right
+           * - /TwoPageLeft
+             - Show two pages at a time, odd-numbered pages on the left
+           * - /TwoPageRight
+             - Show two pages at a time, odd-numbered pages on the right
+        """
+        if not isinstance(layout, NameObject):
+            if layout not in self._valid_layouts:
                 logger_warning(
-                    f"Removed unexpected destination {dest!r} from destination",
+                    f"Layout should be one of: {'', ''.join(self._valid_layouts)}",
                     __name__,
                 )
-            outline_item = self._build_destination(title, None)
+            layout = NameObject(layout)
+        self._root_object.update({NameObject("/PageLayout"): layout})
 
-        # if outline item created, add color, format, and child count if present
-        if outline_item:
-            if "/C" in node:
-                # Color of outline item font in (R, G, B) with values ranging 0.0-1.0
-                outline_item[NameObject("/C")] = ArrayObject(FloatObject(c) for c in node["/C"])  # type: ignore
-            if "/F" in node:
-                # specifies style characteristics bold and/or italic
-                # with 1=italic, 2=bold, 3=both
-                outline_item[NameObject("/F")] = node["/F"]
-            if "/Count" in node:
-                # absolute value = num. visible children
-                # with positive = open/unfolded, negative = closed/folded
-                outline_item[NameObject("/Count")] = node["/Count"]
-            #  if count is 0 we will consider it as open ( in order to have always an is_open to simplify
-            outline_item[NameObject("/%is_open%")] = BooleanObject(
-                node.get("/Count", 0) >= 0
-            )
-        outline_item.node = node
-        try:
-            outline_item.indirect_reference = node.indirect_reference
-        except AttributeError:
-            pass
-        return outline_item
+    def set_page_layout(self, layout: LayoutType) -> None:
+        """
+        Set the page layout.
 
-    @property
-    def pages(self) -> List[PageObject]:
-        """Read-only property that emulates a list of :py:class:`PageObject<pypdf._page.PageObject>` objects."""
-        return _VirtualList(self._get_num_pages, self._get_page)  # type: ignore
+        Args:
+            layout: The page layout to be used
 
-    @property
-    def page_labels(self) -> List[str]:
-        """
-        A list of labels for the pages in this document.
+        .. list-table:: Valid ``layout`` arguments
+           :widths: 50 200
 
-        This property is read-only. The labels are in the order that the pages
-        appear in the document.
+           * - /NoLayout
+             - Layout explicitly not specified
+           * - /SinglePage
+             - Show one page at a time
+           * - /OneColumn
+             - Show one column at a time
+           * - /TwoColumnLeft
+             - Show pages in two columns, odd-numbered pages on the left
+           * - /TwoColumnRight
+             - Show pages in two columns, odd-numbered pages on the right
+           * - /TwoPageLeft
+             - Show two pages at a time, odd-numbered pages on the left
+           * - /TwoPageRight
+             - Show two pages at a time, odd-numbered pages on the right
         """
-        return [page_index2page_label(self, i) for i in range(len(self.pages))]
+        self._set_page_layout(layout)
 
     @property
-    def page_layout(self) -> Optional[str]:
+    def page_layout(self) -> Optional[LayoutType]:
         """
-        Get the page layout currently being used.
+        Page layout property.
 
         .. list-table:: Valid ``layout`` values
            :widths: 50 200
 
            * - /NoLayout
              - Layout explicitly not specified
            * - /SinglePage
@@ -1067,23 +2064,39 @@
            * - /TwoColumnRight
              - Show pages in two columns, odd-numbered pages on the right
            * - /TwoPageLeft
              - Show two pages at a time, odd-numbered pages on the left
            * - /TwoPageRight
              - Show two pages at a time, odd-numbered pages on the right
         """
-        trailer = cast(DictionaryObject, self.trailer[TK.ROOT])
-        if CD.PAGE_LAYOUT in trailer:
-            return cast(NameObject, trailer[CD.PAGE_LAYOUT])
-        return None
+        return self._get_page_layout()
+
+    @page_layout.setter
+    def page_layout(self, layout: LayoutType) -> None:
+        self._set_page_layout(layout)
+
+    _valid_modes = (
+        "/UseNone",
+        "/UseOutlines",
+        "/UseThumbs",
+        "/FullScreen",
+        "/UseOC",
+        "/UseAttachments",
+    )
+
+    def _get_page_mode(self) -> Optional[PagemodeType]:
+        try:
+            return cast(PagemodeType, self._root_object["/PageMode"])
+        except KeyError:
+            return None
 
     @property
     def page_mode(self) -> Optional[PagemodeType]:
         """
-        Get the page mode currently being used.
+        Page mode property.
 
         .. list-table:: Valid ``mode`` values
            :widths: 50 200
 
            * - /UseNone
              - Do not show outline or thumbnails panels
            * - /UseOutlines
@@ -1093,1025 +2106,876 @@
            * - /FullScreen
              - Fullscreen view
            * - /UseOC
              - Show Optional Content Group (OCG) panel
            * - /UseAttachments
              - Show attachments panel
         """
-        try:
-            return self.trailer[TK.ROOT]["/PageMode"]  # type: ignore
-        except KeyError:
-            return None
-
-    def _flatten(
-        self,
-        pages: Union[None, DictionaryObject, PageObject] = None,
-        inherit: Optional[Dict[str, Any]] = None,
-        indirect_reference: Optional[IndirectObject] = None,
-    ) -> None:
-        inheritable_page_attributes = (
-            NameObject(PG.RESOURCES),
-            NameObject(PG.MEDIABOX),
-            NameObject(PG.CROPBOX),
-            NameObject(PG.ROTATE),
-        )
-        if inherit is None:
-            inherit = {}
-        if pages is None:
-            # Fix issue 327: set flattened_pages attribute only for
-            # decrypted file
-            catalog = self.trailer[TK.ROOT].get_object()
-            pages = catalog["/Pages"].get_object()  # type: ignore
-            self.flattened_pages = []
-
-        if PA.TYPE in pages:
-            t = pages[PA.TYPE]
-        # if pdf has no type, considered as a page if /Kids is missing
-        elif PA.KIDS not in pages:
-            t = "/Page"
-        else:
-            t = "/Pages"
-
-        if t == "/Pages":
-            for attr in inheritable_page_attributes:
-                if attr in pages:
-                    inherit[attr] = pages[attr]
-            for page in pages[PA.KIDS]:  # type: ignore
-                addt = {}
-                if isinstance(page, IndirectObject):
-                    addt["indirect_reference"] = page
-                obj = page.get_object()
-                if obj:
-                    # damaged file may have invalid child in /Pages
-                    self._flatten(obj, inherit, **addt)
-        elif t == "/Page":
-            for attr_in, value in list(inherit.items()):
-                # if the page has it's own value, it does not inherit the
-                # parent's value:
-                if attr_in not in pages:
-                    pages[attr_in] = value
-            page_obj = PageObject(self, indirect_reference)
-            page_obj.update(pages)
-
-            # TODO: Could flattened_pages be None at this point?
-            self.flattened_pages.append(page_obj)  # type: ignore
-
-    def _get_object_from_stream(
-        self, indirect_reference: IndirectObject
-    ) -> Union[int, PdfObject, str]:
-        # indirect reference to object in object stream
-        # read the entire object stream into memory
-        stmnum, idx = self.xref_objStm[indirect_reference.idnum]
-        obj_stm: EncodedStreamObject = IndirectObject(stmnum, 0, self).get_object()  # type: ignore
-        # This is an xref to a stream, so its type better be a stream
-        assert cast(str, obj_stm["/Type"]) == "/ObjStm"
-        # /N is the number of indirect objects in the stream
-        assert idx < obj_stm["/N"]
-        stream_data = BytesIO(b_(obj_stm.get_data()))
-        for i in range(obj_stm["/N"]):  # type: ignore
-            read_non_whitespace(stream_data)
-            stream_data.seek(-1, 1)
-            objnum = NumberObject.read_from_stream(stream_data)
-            read_non_whitespace(stream_data)
-            stream_data.seek(-1, 1)
-            offset = NumberObject.read_from_stream(stream_data)
-            read_non_whitespace(stream_data)
-            stream_data.seek(-1, 1)
-            if objnum != indirect_reference.idnum:
-                # We're only interested in one object
-                continue
-            if self.strict and idx != i:
-                raise PdfReadError("Object is in wrong index.")
-            stream_data.seek(int(obj_stm["/First"] + offset), 0)  # type: ignore
-
-            # to cope with some case where the 'pointer' is on a white space
-            read_non_whitespace(stream_data)
-            stream_data.seek(-1, 1)
+        return self._get_page_mode()
 
-            try:
-                obj = read_object(stream_data, self)
-            except PdfStreamError as exc:
-                # Stream object cannot be read. Normally, a critical error, but
-                # Adobe Reader doesn't complain, so continue (in strict mode?)
+    @page_mode.setter
+    def page_mode(self, mode: PagemodeType) -> None:
+        if isinstance(mode, NameObject):
+            mode_name: NameObject = mode
+        else:
+            if mode not in self._valid_modes:
                 logger_warning(
-                    f"Invalid stream (index {i}) within object "
-                    f"{indirect_reference.idnum} {indirect_reference.generation}: "
-                    f"{exc}",
-                    __name__,
+                    f"Mode should be one of: {', '.join(self._valid_modes)}", __name__
                 )
+            mode_name = NameObject(mode)
+        self._root_object.update({NameObject("/PageMode"): mode_name})
 
-                if self.strict:
-                    raise PdfReadError(f"Can't read object stream: {exc}")
-                # Replace with null. Hopefully it's nothing important.
-                obj = NullObject()
-            return obj
+    def add_annotation(
+        self,
+        page_number: Union[int, PageObject],
+        annotation: Dict[str, Any],
+    ) -> DictionaryObject:
+        """
+        Add a single annotation to the page.
+        The added annotation must be a new annotation.
+        It can not be recycled.
 
-        if self.strict:
-            raise PdfReadError("This is a fatal error in strict mode.")
-        return NullObject()
+        Args:
+            page_number: PageObject or page index.
+            annotation: Annotation to be added (created with annotation).
 
-    def _get_indirect_object(self, num: int, gen: int) -> Optional[PdfObject]:
+        Returns:
+            The inserted object
+            This can be used for pop-up creation, for example
         """
-        Used to ease development.
+        page = page_number
+        if isinstance(page, int):
+            page = self.pages[page]
+        elif not isinstance(page, PageObject):
+            raise TypeError("page: invalid type")
+
+        to_add = cast(DictionaryObject, _pdf_objectify(annotation))
+        to_add[NameObject("/P")] = page.indirect_reference
+
+        if page.annotations is None:
+            page[NameObject("/Annots")] = ArrayObject()
+        assert page.annotations is not None
+
+        # Internal link annotations need the correct object type for the
+        # destination
+        if to_add.get("/Subtype") == "/Link" and "/Dest" in to_add:
+            tmp = cast(Dict[Any, Any], to_add[NameObject("/Dest")])
+            dest = Destination(
+                NameObject("/LinkName"),
+                tmp["target_page_index"],
+                Fit(
+                    fit_type=tmp["fit"], fit_args=dict(tmp)["fit_args"]
+                ),  # I have no clue why this dict-hack is necessary
+            )
+            to_add[NameObject("/Dest")] = dest.dest_array
+
+        page.annotations.append(self._add_object(to_add))
 
-        This is equivalent to generic.IndirectObject(num,gen,self).get_object()
+        if to_add.get("/Subtype") == "/Popup" and NameObject("/Parent") in to_add:
+            cast(DictionaryObject, to_add["/Parent"].get_object())[
+                NameObject("/Popup")
+            ] = to_add.indirect_reference
+
+        return to_add
+
+    def clean_page(self, page: Union[PageObject, IndirectObject]) -> PageObject:
+        """
+        Perform some clean up in the page.
+        Currently: convert NameObject nameddestination to TextStringObject
+        (required for names/dests list)
 
         Args:
-            num: The object number of the indirect object.
-            gen: The generation number of the indirect object.
+            page:
 
         Returns:
-            A PdfObject
+            The cleaned PageObject
         """
-        return IndirectObject(num, gen, self).get_object()
-
-    def get_object(
-        self, indirect_reference: Union[int, IndirectObject]
-    ) -> Optional[PdfObject]:
-        if isinstance(indirect_reference, int):
-            indirect_reference = IndirectObject(indirect_reference, 0, self)
-        retval = self.cache_get_indirect_object(
-            indirect_reference.generation, indirect_reference.idnum
-        )
-        if retval is not None:
-            return retval
-        if (
-            indirect_reference.generation == 0
-            and indirect_reference.idnum in self.xref_objStm
-        ):
-            retval = self._get_object_from_stream(indirect_reference)  # type: ignore
-        elif (
-            indirect_reference.generation in self.xref
-            and indirect_reference.idnum in self.xref[indirect_reference.generation]
-        ):
-            if self.xref_free_entry.get(indirect_reference.generation, {}).get(
-                indirect_reference.idnum, False
-            ):
-                return NullObject()
-            start = self.xref[indirect_reference.generation][indirect_reference.idnum]
-            self.stream.seek(start, 0)
-            try:
-                idnum, generation = self.read_object_header(self.stream)
-            except Exception:
-                if hasattr(self.stream, "getbuffer"):
-                    buf = bytes(self.stream.getbuffer())
-                else:
-                    p = self.stream.tell()
-                    self.stream.seek(0, 0)
-                    buf = self.stream.read(-1)
-                    self.stream.seek(p, 0)
-                m = re.search(
-                    rf"\s{indirect_reference.idnum}\s+{indirect_reference.generation}\s+obj".encode(),
-                    buf,
-                )
-                if m is not None:
-                    logger_warning(
-                        f"Object ID {indirect_reference.idnum},{indirect_reference.generation} ref repaired",
-                        __name__,
-                    )
-                    self.xref[indirect_reference.generation][
-                        indirect_reference.idnum
-                    ] = (m.start(0) + 1)
-                    self.stream.seek(m.start(0) + 1)
-                    idnum, generation = self.read_object_header(self.stream)
-                else:
-                    idnum = -1  # exception will be raised below
-            if idnum != indirect_reference.idnum and self.xref_index:
-                # Xref table probably had bad indexes due to not being zero-indexed
-                if self.strict:
-                    raise PdfReadError(
-                        f"Expected object ID ({indirect_reference.idnum} {indirect_reference.generation}) "
-                        f"does not match actual ({idnum} {generation}); "
-                        "xref table not zero-indexed."
-                    )
-                # xref table is corrected in non-strict mode
-            elif idnum != indirect_reference.idnum and self.strict:
-                # some other problem
-                raise PdfReadError(
-                    f"Expected object ID ({indirect_reference.idnum} "
-                    f"{indirect_reference.generation}) does not match actual "
-                    f"({idnum} {generation})."
-                )
-            if self.strict:
-                assert generation == indirect_reference.generation
-            retval = read_object(self.stream, self)  # type: ignore
-
-            # override encryption is used for the /Encrypt dictionary
-            if not self._override_encryption and self._encryption is not None:
-                # if we don't have the encryption key:
-                if not self._encryption.is_decrypted():
-                    raise FileNotDecryptedError("File has not been decrypted")
-                # otherwise, decrypt here...
-                retval = cast(PdfObject, retval)
-                retval = self._encryption.decrypt_object(
-                    retval, indirect_reference.idnum, indirect_reference.generation
-                )
+        page = cast("PageObject", page.get_object())
+        for a in page.get("/Annots", []):
+            a_obj = a.get_object()
+            d = a_obj.get("/Dest", None)
+            act = a_obj.get("/A", None)
+            if isinstance(d, NameObject):
+                a_obj[NameObject("/Dest")] = TextStringObject(d)
+            elif act is not None:
+                act = act.get_object()
+                d = act.get("/D", None)
+                if isinstance(d, NameObject):
+                    act[NameObject("/D")] = TextStringObject(d)
+        return page
+
+    def _create_stream(
+        self, fileobj: Union[Path, StrByteType, PdfReader]
+    ) -> Tuple[IOBase, Optional[Encryption]]:
+        # If the fileobj parameter is a string, assume it is a path
+        # and create a file object at that location. If it is a file,
+        # copy the file's contents into a BytesIO stream object; if
+        # it is a PdfReader, copy that reader's stream into a
+        # BytesIO stream.
+        # If fileobj is none of the above types, it is not modified
+        encryption_obj = None
+        stream: IOBase
+        if isinstance(fileobj, (str, Path)):
+            with FileIO(fileobj, "rb") as f:
+                stream = BytesIO(f.read())
+        elif isinstance(fileobj, PdfReader):
+            if fileobj._encryption:
+                encryption_obj = fileobj._encryption
+            orig_tell = fileobj.stream.tell()
+            fileobj.stream.seek(0)
+            stream = BytesIO(fileobj.stream.read())
+
+            # reset the stream to its original location
+            fileobj.stream.seek(orig_tell)
+        elif hasattr(fileobj, "seek") and hasattr(fileobj, "read"):
+            fileobj.seek(0)
+            filecontent = fileobj.read()
+            stream = BytesIO(filecontent)
         else:
-            if hasattr(self.stream, "getbuffer"):
-                buf = bytes(self.stream.getbuffer())
-            else:
-                p = self.stream.tell()
-                self.stream.seek(0, 0)
-                buf = self.stream.read(-1)
-                self.stream.seek(p, 0)
-            m = re.search(
-                rf"\s{indirect_reference.idnum}\s+{indirect_reference.generation}\s+obj".encode(),
-                buf,
+            raise NotImplementedError(
+                "PdfMerger.merge requires an object that PdfReader can parse. "
+                "Typically, that is a Path or a string representing a Path, "
+                "a file object, or an object implementing .seek and .read. "
+                "Passing a PdfReader directly works as well."
             )
-            if m is not None:
-                logger_warning(
-                    f"Object {indirect_reference.idnum} {indirect_reference.generation} found",
-                    __name__,
-                )
-                if indirect_reference.generation not in self.xref:
-                    self.xref[indirect_reference.generation] = {}
-                self.xref[indirect_reference.generation][indirect_reference.idnum] = (
-                    m.start(0) + 1
-                )
-                self.stream.seek(m.end(0) + 1)
-                skip_over_whitespace(self.stream)
-                self.stream.seek(-1, 1)
-                retval = read_object(self.stream, self)  # type: ignore
-
-                # override encryption is used for the /Encrypt dictionary
-                if not self._override_encryption and self._encryption is not None:
-                    # if we don't have the encryption key:
-                    if not self._encryption.is_decrypted():
-                        raise FileNotDecryptedError("File has not been decrypted")
-                    # otherwise, decrypt here...
-                    retval = cast(PdfObject, retval)
-                    retval = self._encryption.decrypt_object(
-                        retval, indirect_reference.idnum, indirect_reference.generation
-                    )
-            else:
-                logger_warning(
-                    f"Object {indirect_reference.idnum} {indirect_reference.generation} not defined.",
-                    __name__,
-                )
-                if self.strict:
-                    raise PdfReadError("Could not find object.")
-        self.cache_indirect_object(
-            indirect_reference.generation, indirect_reference.idnum, retval
-        )
-        return retval
-
-    def read_object_header(self, stream: StreamType) -> Tuple[int, int]:
-        # Should never be necessary to read out whitespace, since the
-        # cross-reference table should put us in the right spot to read the
-        # object header.  In reality... some files have stupid cross reference
-        # tables that are off by whitespace bytes.
-        extra = False
-        skip_over_comment(stream)
-        extra |= skip_over_whitespace(stream)
-        stream.seek(-1, 1)
-        idnum = read_until_whitespace(stream)
-        extra |= skip_over_whitespace(stream)
-        stream.seek(-1, 1)
-        generation = read_until_whitespace(stream)
-        extra |= skip_over_whitespace(stream)
-        stream.seek(-1, 1)
-
-        # although it's not used, it might still be necessary to read
-        _obj = stream.read(3)
-
-        read_non_whitespace(stream)
-        stream.seek(-1, 1)
-        if extra and self.strict:
-            logger_warning(
-                f"Superfluous whitespace found in object header {idnum} {generation}",  # type: ignore
-                __name__,
-            )
-        return int(idnum), int(generation)
-
-    def cache_get_indirect_object(
-        self, generation: int, idnum: int
-    ) -> Optional[PdfObject]:
-        return self.resolved_objects.get((generation, idnum))
-
-    def cache_indirect_object(
-        self, generation: int, idnum: int, obj: Optional[PdfObject]
-    ) -> Optional[PdfObject]:
-        if (generation, idnum) in self.resolved_objects:
-            msg = f"Overwriting cache for {generation} {idnum}"
-            if self.strict:
-                raise PdfReadError(msg)
-            logger_warning(msg, __name__)
-        self.resolved_objects[(generation, idnum)] = obj
-        if obj is not None:
-            obj.indirect_reference = IndirectObject(idnum, generation, self)
-        return obj
+        return stream, encryption_obj
 
-    def read(self, stream: StreamType) -> None:
-        self._basic_validation(stream)
-        self._find_eof_marker(stream)
-        startxref = self._find_startxref_pos(stream)
-
-        # check and eventually correct the startxref only in not strict
-        xref_issue_nr = self._get_xref_issues(stream, startxref)
-        if xref_issue_nr != 0:
-            if self.strict and xref_issue_nr:
-                raise PdfReadError("Broken xref table")
-            logger_warning(f"incorrect startxref pointer({xref_issue_nr})", __name__)
-
-        # read all cross reference tables and their trailers
-        self._read_xref_tables_and_trailers(stream, startxref, xref_issue_nr)
-
-        # if not zero-indexed, verify that the table is correct; change it if necessary
-        if self.xref_index and not self.strict:
-            loc = stream.tell()
-            for gen, xref_entry in self.xref.items():
-                if gen == 65535:
-                    continue
-                xref_k = sorted(
-                    xref_entry.keys()
-                )  # must ensure ascendant to prevent damage
-                for id in xref_k:
-                    stream.seek(xref_entry[id], 0)
-                    try:
-                        pid, _pgen = self.read_object_header(stream)
-                    except ValueError:
-                        break
-                    if pid == id - self.xref_index:
-                        # fixing index item per item is required for revised PDF.
-                        self.xref[gen][pid] = self.xref[gen][id]
-                        del self.xref[gen][id]
-                    # if not, then either it's just plain wrong, or the
-                    # non-zero-index is actually correct
-            stream.seek(loc, 0)  # return to where it was
-
-    def _basic_validation(self, stream: StreamType) -> None:
-        """Ensure file is not empty. Read at most 5 bytes."""
-        stream.seek(0, os.SEEK_SET)
-        try:
-            header_byte = stream.read(5)
-        except UnicodeDecodeError:
-            raise UnsupportedOperation("cannot read header")
-        if header_byte == b"":
-            raise EmptyFileError("Cannot read an empty file")
-        elif header_byte != b"%PDF-":
-            if self.strict:
-                raise PdfReadError(
-                    f"PDF starts with '{header_byte.decode('utf8')}', "
-                    "but '%PDF-' expected"
-                )
-            else:
-                logger_warning(f"invalid pdf header: {header_byte}", __name__)
-        stream.seek(0, os.SEEK_END)
-
-    def _find_eof_marker(self, stream: StreamType) -> None:
+    def append(
+        self,
+        fileobj: Union[StrByteType, PdfReader, Path],
+        outline_item: Union[
+            str, None, PageRange, Tuple[int, int], Tuple[int, int, int], List[int]
+        ] = None,
+        pages: Union[
+            None,
+            PageRange,
+            Tuple[int, int],
+            Tuple[int, int, int],
+            List[int],
+            List[PageObject],
+        ] = None,
+        import_outline: bool = True,
+        excluded_fields: Optional[Union[List[str], Tuple[str, ...]]] = None,
+    ) -> None:
         """
-        Jump to the %%EOF marker.
+        Identical to the :meth:`merge()<merge>` method, but assumes you want to
+        concatenate all pages onto the end of the file instead of specifying a
+        position.
 
-        According to the specs, the %%EOF marker should be at the very end of
-        the file. Hence for standard-compliant PDF documents this function will
-        read only the last part (DEFAULT_BUFFER_SIZE).
-        """
-        HEADER_SIZE = 8  # to parse whole file, Header is e.g. '%PDF-1.6'
-        line = b""
-        while line[:5] != b"%%EOF":
-            if stream.tell() < HEADER_SIZE:
-                if self.strict:
-                    raise PdfReadError("EOF marker not found")
-                else:
-                    logger_warning("EOF marker not found", __name__)
-            line = read_previous_line(stream)
+        Args:
+            fileobj: A File Object or an object that supports the standard
+                read and seek methods similar to a File Object. Could also be a
+                string representing a path to a PDF file.
+            outline_item: Optionally, you may specify a string to build an
+                outline (aka 'bookmark') to identify the beginning of the
+                included file.
+            pages: Can be a :class:`PageRange<pypdf.pagerange.PageRange>`
+                or a ``(start, stop[, step])`` tuple
+                or a list of pages to be processed
+                to merge only the specified range of pages from the source
+                document into the output document.
+            import_outline: You may prevent the source document's
+                outline (collection of outline items, previously referred to as
+                'bookmarks') from being imported by specifying this as ``False``.
+            excluded_fields: Provide the list of fields/keys to be ignored
+                if ``/Annots`` is part of the list, the annotation will be ignored
+                if ``/B`` is part of the list, the articles will be ignored
+        """
+        if excluded_fields is None:
+            excluded_fields = ()
+        if isinstance(outline_item, (tuple, list, PageRange)):
+            if isinstance(pages, bool):
+                if not isinstance(import_outline, bool):
+                    excluded_fields = import_outline
+                import_outline = pages
+            pages = outline_item
+            self.merge(
+                None,
+                fileobj,
+                None,
+                pages,
+                import_outline,
+                excluded_fields,
+            )
+        else:  # if isinstance(outline_item,str):
+            self.merge(
+                None,
+                fileobj,
+                outline_item,
+                pages,
+                import_outline,
+                excluded_fields,
+            )
 
-    def _find_startxref_pos(self, stream: StreamType) -> int:
+    def merge(
+        self,
+        position: Optional[int],
+        fileobj: Union[Path, StrByteType, PdfReader],
+        outline_item: Optional[str] = None,
+        pages: Optional[Union[PageRangeSpec, List[PageObject]]] = None,
+        import_outline: bool = True,
+        excluded_fields: Optional[Union[List[str], Tuple[str, ...]]] = (),
+    ) -> None:
         """
-        Find startxref entry - the location of the xref table.
+        Merge the pages from the given file into the output file at the
+        specified page number.
 
         Args:
-            stream:
+            position: The *page number* to insert this file. File will
+                be inserted after the given number.
+            fileobj: A File Object or an object that supports the standard
+                read and seek methods similar to a File Object. Could also be a
+                string representing a path to a PDF file.
+            outline_item: Optionally, you may specify a string to build an outline
+                (aka 'bookmark') to identify the
+                beginning of the included file.
+            pages: can be a :class:`PageRange<pypdf.pagerange.PageRange>`
+                or a ``(start, stop[, step])`` tuple
+                or a list of pages to be processed
+                to merge only the specified range of pages from the source
+                document into the output document.
+            import_outline: You may prevent the source document's
+                outline (collection of outline items, previously referred to as
+                'bookmarks') from being imported by specifying this as ``False``.
+            excluded_fields: provide the list of fields/keys to be ignored
+                if ``/Annots`` is part of the list, the annotation will be ignored
+                if ``/B`` is part of the list, the articles will be ignored
 
-        Returns:
-            The bytes offset
+        Raises:
+            TypeError: The pages attribute is not configured properly
         """
-        line = read_previous_line(stream)
-        try:
-            startxref = int(line)
-        except ValueError:
-            # 'startxref' may be on the same line as the location
-            if not line.startswith(b"startxref"):
-                raise PdfReadError("startxref not found")
-            startxref = int(line[9:].strip())
-            logger_warning("startxref on same line as offset", __name__)
-        else:
-            line = read_previous_line(stream)
-            if line[:9] != b"startxref":
-                raise PdfReadError("startxref not found")
-        return startxref
-
-    def _read_standard_xref_table(self, stream: StreamType) -> None:
-        # standard cross-reference table
-        ref = stream.read(3)
-        if ref != b"ref":
-            raise PdfReadError("xref table read error")
-        read_non_whitespace(stream)
-        stream.seek(-1, 1)
-        first_time = True  # check if the first time looking at the xref table
-        while True:
-            num = cast(int, read_object(stream, self))
-            if first_time and num != 0:
-                self.xref_index = num
-                if self.strict:
-                    logger_warning(
-                        "Xref table not zero-indexed. ID numbers for objects will be corrected.",
-                        __name__,
-                    )
-                    # if table not zero indexed, could be due to error from when PDF was created
-                    # which will lead to mismatched indices later on, only warned and corrected if self.strict==True
-            first_time = False
-            read_non_whitespace(stream)
-            stream.seek(-1, 1)
-            size = cast(int, read_object(stream, self))
-            read_non_whitespace(stream)
-            stream.seek(-1, 1)
-            cnt = 0
-            while cnt < size:
-                line = stream.read(20)
-
-                # It's very clear in section 3.4.3 of the PDF spec
-                # that all cross-reference table lines are a fixed
-                # 20 bytes (as of PDF 1.7). However, some files have
-                # 21-byte entries (or more) due to the use of \r\n
-                # (CRLF) EOL's. Detect that case, and adjust the line
-                # until it does not begin with a \r (CR) or \n (LF).
-                while line[0] in b"\x0D\x0A":
-                    stream.seek(-20 + 1, 1)
-                    line = stream.read(20)
-
-                # On the other hand, some malformed PDF files
-                # use a single character EOL without a preceding
-                # space.  Detect that case, and seek the stream
-                # back one character.  (0-9 means we've bled into
-                # the next xref entry, t means we've bled into the
-                # text "trailer"):
-                if line[-1] in b"0123456789t":
-                    stream.seek(-1, 1)
-
-                try:
-                    offset_b, generation_b = line[:16].split(b" ")
-                    entry_type_b = line[17:18]
-
-                    offset, generation = int(offset_b), int(generation_b)
-                except Exception:
-                    # if something wrong occurred
-                    if hasattr(stream, "getbuffer"):
-                        buf = bytes(stream.getbuffer())
-                    else:
-                        p = stream.tell()
-                        stream.seek(0, 0)
-                        buf = stream.read(-1)
-                        stream.seek(p)
-
-                    f = re.search(f"{num}\\s+(\\d+)\\s+obj".encode(), buf)
-                    if f is None:
-                        logger_warning(
-                            f"entry {num} in Xref table invalid; object not found",
-                            __name__,
-                        )
-                        generation = 65535
-                        offset = -1
-                    else:
-                        logger_warning(
-                            f"entry {num} in Xref table invalid but object found",
-                            __name__,
-                        )
-                        generation = int(f.group(1))
-                        offset = f.start()
+        if isinstance(fileobj, PdfDocCommon):
+            reader = fileobj
+        else:
+            stream, encryption_obj = self._create_stream(fileobj)
+            # Create a new PdfReader instance using the stream
+            # (either file or BytesIO or StringIO) created above
+            reader = PdfReader(stream, strict=False)  # type: ignore[arg-type]
+
+        if excluded_fields is None:
+            excluded_fields = ()
+        # Find the range of pages to merge.
+        if pages is None:
+            pages = list(range(len(reader.pages)))
+        elif isinstance(pages, PageRange):
+            pages = list(range(*pages.indices(len(reader.pages))))
+        elif isinstance(pages, list):
+            pass  # keep unchanged
+        elif isinstance(pages, tuple) and len(pages) <= 3:
+            pages = list(range(*pages))
+        elif not isinstance(pages, tuple):
+            raise TypeError(
+                '"pages" must be a tuple of (start, stop[, step]) or a list'
+            )
 
-                if generation not in self.xref:
-                    self.xref[generation] = {}
-                    self.xref_free_entry[generation] = {}
-                if num in self.xref[generation]:
-                    # It really seems like we should allow the last
-                    # xref table in the file to override previous
-                    # ones. Since we read the file backwards, assume
-                    # any existing key is already set correctly.
-                    pass
-                else:
-                    self.xref[generation][num] = offset
-                    try:
-                        self.xref_free_entry[generation][num] = entry_type_b == b"f"
-                    except Exception:
-                        pass
-                    try:
-                        self.xref_free_entry[65535][num] = entry_type_b == b"f"
-                    except Exception:
-                        pass
-                cnt += 1
-                num += 1
-            read_non_whitespace(stream)
-            stream.seek(-1, 1)
-            trailer_tag = stream.read(7)
-            if trailer_tag != b"trailer":
-                # more xrefs!
-                stream.seek(-7, 1)
+        srcpages = {}
+        for page in pages:
+            if isinstance(page, PageObject):
+                pg = page
             else:
-                break
-
-    def _read_xref_tables_and_trailers(
-        self, stream: StreamType, startxref: Optional[int], xref_issue_nr: int
-    ) -> None:
-        self.xref: Dict[int, Dict[Any, Any]] = {}
-        self.xref_free_entry: Dict[int, Dict[Any, Any]] = {}
-        self.xref_objStm: Dict[int, Tuple[Any, Any]] = {}
-        self.trailer = DictionaryObject()
-        while startxref is not None:
-            # load the xref table
-            stream.seek(startxref, 0)
-            x = stream.read(1)
-            if x in b"\r\n":
-                x = stream.read(1)
-            if x == b"x":
-                startxref = self._read_xref(stream)
-            elif xref_issue_nr:
-                try:
-                    self._rebuild_xref_table(stream)
-                    break
-                except Exception:
-                    xref_issue_nr = 0
-            elif x.isdigit():
-                try:
-                    xrefstream = self._read_pdf15_xref_stream(stream)
-                except Exception as e:
-                    if TK.ROOT in self.trailer:
-                        logger_warning(
-                            f"Previous trailer can not be read {e.args}",
-                            __name__,
-                        )
-                        break
-                    else:
-                        raise PdfReadError(f"trailer can not be read {e.args}")
-                trailer_keys = TK.ROOT, TK.ENCRYPT, TK.INFO, TK.ID, TK.SIZE
-                for key in trailer_keys:
-                    if key in xrefstream and key not in self.trailer:
-                        self.trailer[NameObject(key)] = xrefstream.raw_get(key)
-                if "/XRefStm" in xrefstream:
-                    p = stream.tell()
-                    stream.seek(cast(int, xrefstream["/XRefStm"]) + 1, 0)
-                    self._read_pdf15_xref_stream(stream)
-                    stream.seek(p, 0)
-                if "/Prev" in xrefstream:
-                    startxref = cast(int, xrefstream["/Prev"])
-                else:
-                    break
+                pg = reader.pages[page]
+            assert pg.indirect_reference is not None
+            if position is None:
+                # numbers in the exclude list identifies that the exclusion is
+                # only applicable to 1st level of cloning
+                srcpages[pg.indirect_reference.idnum] = self.add_page(
+                    pg, list(excluded_fields) + [1, "/B", 1, "/Annots"]  # type: ignore
+                )
             else:
-                startxref = self._read_xref_other_error(stream, startxref)
-
-    def _read_xref(self, stream: StreamType) -> Optional[int]:
-        self._read_standard_xref_table(stream)
-        read_non_whitespace(stream)
-        stream.seek(-1, 1)
-        new_trailer = cast(Dict[str, Any], read_object(stream, self))
-        for key, value in new_trailer.items():
-            if key not in self.trailer:
-                self.trailer[key] = value
-        if "/XRefStm" in new_trailer:
-            p = stream.tell()
-            stream.seek(cast(int, new_trailer["/XRefStm"]) + 1, 0)
-            try:
-                self._read_pdf15_xref_stream(stream)
-            except Exception:
-                logger_warning(
-                    f"XRef object at {new_trailer['/XRefStm']} can not be read, some object may be missing",
-                    __name__,
+                srcpages[pg.indirect_reference.idnum] = self.insert_page(
+                    pg, position, list(excluded_fields) + [1, "/B", 1, "/Annots"]  # type: ignore
                 )
-            stream.seek(p, 0)
-        if "/Prev" in new_trailer:
-            startxref = new_trailer["/Prev"]
-            return startxref
-        else:
-            return None
+                position += 1
+            srcpages[pg.indirect_reference.idnum].original_page = pg
 
-    def _read_xref_other_error(
-        self, stream: StreamType, startxref: int
-    ) -> Optional[int]:
-        # some PDFs have /Prev=0 in the trailer, instead of no /Prev
-        if startxref == 0:
-            if self.strict:
-                raise PdfReadError(
-                    "/Prev=0 in the trailer (try opening with strict=False)"
-                )
-            logger_warning(
-                "/Prev=0 in the trailer - assuming there is no previous xref table",
-                __name__,
+        reader._namedDests = (
+            reader.named_destinations
+        )  # need for the outline processing below
+        for dest in reader._namedDests.values():
+            arr = dest.dest_array
+            if "/Names" in self._root_object and dest["/Title"] in cast(
+                List[Any],
+                cast(
+                    DictionaryObject,
+                    cast(DictionaryObject, self._root_object["/Names"])["/Dests"],
+                )["/Names"],
+            ):
+                # already exists : should not duplicate it
+                pass
+            elif isinstance(dest["/Page"], NullObject):
+                pass
+            elif isinstance(dest["/Page"], int):
+                # the page reference is a page number normally not iaw Pdf Reference
+                # page numbers as int are normally accepted only in external goto
+                p = reader.pages[dest["/Page"]]
+                assert p.indirect_reference is not None
+                try:
+                    arr[NumberObject(0)] = NumberObject(
+                        srcpages[p.indirect_reference.idnum].page_number
+                    )
+                    self.add_named_destination_array(dest["/Title"], arr)
+                except KeyError:
+                    pass
+            elif dest["/Page"].indirect_reference.idnum in srcpages:
+                arr[NumberObject(0)] = srcpages[
+                    dest["/Page"].indirect_reference.idnum
+                ].indirect_reference
+                self.add_named_destination_array(dest["/Title"], arr)
+
+        outline_item_typ: TreeObject
+        if outline_item is not None:
+            outline_item_typ = cast(
+                "TreeObject",
+                self.add_outline_item(
+                    TextStringObject(outline_item),
+                    next(iter(srcpages.values())).indirect_reference,
+                    fit=PAGE_FIT,
+                ).get_object(),
             )
-            return None
-        # bad xref character at startxref.  Let's see if we can find
-        # the xref table nearby, as we've observed this error with an
-        # off-by-one before.
-        stream.seek(-11, 1)
-        tmp = stream.read(20)
-        xref_loc = tmp.find(b"xref")
-        if xref_loc != -1:
-            startxref -= 10 - xref_loc
-            return startxref
-        # No explicit xref table, try finding a cross-reference stream.
-        stream.seek(startxref, 0)
-        for look in range(25):  # value extended to cope with more linearized files
-            if stream.read(1).isdigit():
-                # This is not a standard PDF, consider adding a warning
-                startxref += look
-                return startxref
-        # no xref table found at specified location
-        if "/Root" in self.trailer and not self.strict:
-            # if Root has been already found, just raise warning
-            logger_warning("Invalid parent xref., rebuild xref", __name__)
-            try:
-                self._rebuild_xref_table(stream)
-                return None
-            except Exception:
-                raise PdfReadError("can not rebuild xref")
-        raise PdfReadError("Could not find xref table at specified location")
+        else:
+            outline_item_typ = self.get_outline_root()
 
-    def _read_pdf15_xref_stream(
-        self, stream: StreamType
-    ) -> Union[ContentStream, EncodedStreamObject, DecodedStreamObject]:
-        # PDF 1.5+ Cross-Reference Stream
-        stream.seek(-1, 1)
-        idnum, generation = self.read_object_header(stream)
-        xrefstream = cast(ContentStream, read_object(stream, self))
-        assert cast(str, xrefstream["/Type"]) == "/XRef"
-        self.cache_indirect_object(generation, idnum, xrefstream)
-        stream_data = BytesIO(b_(xrefstream.get_data()))
-        # Index pairs specify the subsections in the dictionary. If
-        # none create one subsection that spans everything.
-        idx_pairs = xrefstream.get("/Index", [0, xrefstream.get("/Size")])
-        entry_sizes = cast(Dict[Any, Any], xrefstream.get("/W"))
-        assert len(entry_sizes) >= 3
-        if self.strict and len(entry_sizes) > 3:
-            raise PdfReadError(f"Too many entry sizes: {entry_sizes}")
-
-        def get_entry(i: int) -> Union[int, Tuple[int, ...]]:
-            # Reads the correct number of bytes for each entry. See the
-            # discussion of the W parameter in PDF spec table 17.
-            if entry_sizes[i] > 0:
-                d = stream_data.read(entry_sizes[i])
-                return convert_to_int(d, entry_sizes[i])
-
-            # PDF Spec Table 17: A value of zero for an element in the
-            # W array indicates...the default value shall be used
-            if i == 0:
-                return 1  # First value defaults to 1
+        _ro = reader.root_object
+        if import_outline and CO.OUTLINES in _ro:
+            outline = self._get_filtered_outline(
+                _ro.get(CO.OUTLINES, None), srcpages, reader
+            )
+            self._insert_filtered_outline(
+                outline, outline_item_typ, None
+            )  # TODO : use before parameter
+
+        if "/Annots" not in excluded_fields:
+            for pag in srcpages.values():
+                lst = self._insert_filtered_annotations(
+                    pag.original_page.get("/Annots", ()), pag, srcpages, reader
+                )
+                if len(lst) > 0:
+                    pag[NameObject("/Annots")] = lst
+                self.clean_page(pag)
+
+        if "/AcroForm" in _ro and _ro["/AcroForm"] is not None:
+            if "/AcroForm" not in self._root_object:
+                self._root_object[NameObject("/AcroForm")] = self._add_object(
+                    cast(
+                        DictionaryObject,
+                        reader.root_object["/AcroForm"],
+                    ).clone(self, False, ("/Fields",))
+                )
+                arr = ArrayObject()
             else:
-                return 0
-
-        def used_before(num: int, generation: Union[int, Tuple[int, ...]]) -> bool:
-            # We move backwards through the xrefs, don't replace any.
-            return num in self.xref.get(generation, []) or num in self.xref_objStm  # type: ignore
+                arr = cast(
+                    ArrayObject,
+                    cast(DictionaryObject, self._root_object["/AcroForm"])["/Fields"],
+                )
+            trslat = self._id_translated[id(reader)]
+            try:
+                for f in reader.root_object["/AcroForm"]["/Fields"]:  # type: ignore
+                    try:
+                        ind = IndirectObject(trslat[f.idnum], 0, self)
+                        if ind not in arr:
+                            arr.append(ind)
+                    except KeyError:
+                        # for trslat[] which mean the field has not be copied
+                        # through the page
+                        pass
+            except KeyError:  # for /Acroform or /Fields are not existing
+                arr = self._add_object(ArrayObject())
+            cast(DictionaryObject, self._root_object["/AcroForm"])[
+                NameObject("/Fields")
+            ] = arr
 
-        # Iterate through each subsection
-        self._read_xref_subsections(idx_pairs, get_entry, used_before)
-        return xrefstream
+        if "/B" not in excluded_fields:
+            self.add_filtered_articles("", srcpages, reader)
 
-    @staticmethod
-    def _get_xref_issues(stream: StreamType, startxref: int) -> int:
+    def _add_articles_thread(
+        self,
+        thread: DictionaryObject,  # thread entry from the reader's array of threads
+        pages: Dict[int, PageObject],
+        reader: PdfReader,
+    ) -> IndirectObject:
         """
-        Return an int which indicates an issue. 0 means there is no issue.
+        Clone the thread with only the applicable articles.
 
         Args:
-            stream:
-            startxref:
+            thread:
+            pages:
+            reader:
 
         Returns:
-            0 means no issue, other values represent specific issues.
+            The added thread as an indirect reference
         """
-        stream.seek(startxref - 1, 0)  # -1 to check character before
-        line = stream.read(1)
-        if line == b"j":
-            line = stream.read(1)
-        if line not in b"\r\n \t":
-            return 1
-        line = stream.read(4)
-        if line != b"xref":
-            # not an xref so check if it is an XREF object
-            line = b""
-            while line in b"0123456789 \t":
-                line = stream.read(1)
-                if line == b"":
-                    return 2
-            line += stream.read(2)  # 1 char already read, +2 to check "obj"
-            if line.lower() != b"obj":
-                return 3
-        return 0
-
-    def _rebuild_xref_table(self, stream: StreamType) -> None:
-        self.xref = {}
-        stream.seek(0, 0)
-        f_ = stream.read(-1)
-
-        for m in re.finditer(rb"[\r\n \t][ \t]*(\d+)[ \t]+(\d+)[ \t]+obj", f_):
-            idnum = int(m.group(1))
-            generation = int(m.group(2))
-            if generation not in self.xref:
-                self.xref[generation] = {}
-            self.xref[generation][idnum] = m.start(1)
-        stream.seek(0, 0)
-        for m in re.finditer(rb"[\r\n \t][ \t]*trailer[\r\n \t]*(<<)", f_):
-            stream.seek(m.start(1), 0)
-            new_trailer = cast(Dict[Any, Any], read_object(stream, self))
-            # Here, we are parsing the file from start to end, the new data have to erase the existing.
-            for key, value in list(new_trailer.items()):
-                self.trailer[key] = value
-
-    def _read_xref_subsections(
-        self,
-        idx_pairs: List[int],
-        get_entry: Callable[[int], Union[int, Tuple[int, ...]]],
-        used_before: Callable[[int, Union[int, Tuple[int, ...]]], bool],
-    ) -> None:
-        for start, size in self._pairs(idx_pairs):
-            # The subsections must increase
-            for num in range(start, start + size):
-                # The first entry is the type
-                xref_type = get_entry(0)
-                # The rest of the elements depend on the xref_type
-                if xref_type == 0:
-                    # linked list of free objects
-                    next_free_object = get_entry(1)  # noqa: F841
-                    next_generation = get_entry(2)  # noqa: F841
-                elif xref_type == 1:
-                    # objects that are in use but are not compressed
-                    byte_offset = get_entry(1)
-                    generation = get_entry(2)
-                    if generation not in self.xref:
-                        self.xref[generation] = {}  # type: ignore
-                    if not used_before(num, generation):
-                        self.xref[generation][num] = byte_offset  # type: ignore
-                elif xref_type == 2:
-                    # compressed objects
-                    objstr_num = get_entry(1)
-                    obstr_idx = get_entry(2)
-                    generation = 0  # PDF spec table 18, generation is 0
-                    if not used_before(num, generation):
-                        self.xref_objStm[num] = (objstr_num, obstr_idx)
-                elif self.strict:
-                    raise PdfReadError(f"Unknown xref type: {xref_type}")
-
-    def _pairs(self, array: List[int]) -> Iterable[Tuple[int, int]]:
-        i = 0
-        while True:
-            yield array[i], array[i + 1]
-            i += 2
-            if (i + 1) >= len(array):
-                break
-
-    def decrypt(self, password: Union[str, bytes]) -> PasswordType:
-        """
-        When using an encrypted / secured PDF file with the PDF Standard
-        encryption handler, this function will allow the file to be decrypted.
-        It checks the given password against the document's user password and
-        owner password, and then stores the resulting decryption key if either
-        password is correct.
-
-        It does not matter which password was matched.  Both passwords provide
-        the correct decryption key that will allow the document to be used with
-        this library.
-
-        Args:
-            password: The password to match.
+        nthread = thread.clone(
+            self, force_duplicate=True, ignore_fields=("/F",)
+        )  # use of clone to keep link between reader and writer
+        self.threads.append(nthread.indirect_reference)
+        first_article = cast("DictionaryObject", thread["/F"])
+        current_article: Optional[DictionaryObject] = first_article
+        new_article: Optional[DictionaryObject] = None
+        while current_article is not None:
+            pag = self._get_cloned_page(
+                cast("PageObject", current_article["/P"]), pages, reader
+            )
+            if pag is not None:
+                if new_article is None:
+                    new_article = cast(
+                        "DictionaryObject",
+                        self._add_object(DictionaryObject()).get_object(),
+                    )
+                    new_first = new_article
+                    nthread[NameObject("/F")] = new_article.indirect_reference
+                else:
+                    new_article2 = cast(
+                        "DictionaryObject",
+                        self._add_object(
+                            DictionaryObject(
+                                {NameObject("/V"): new_article.indirect_reference}
+                            )
+                        ).get_object(),
+                    )
+                    new_article[NameObject("/N")] = new_article2.indirect_reference
+                    new_article = new_article2
+                new_article[NameObject("/P")] = pag
+                new_article[NameObject("/T")] = nthread.indirect_reference
+                new_article[NameObject("/R")] = current_article["/R"]
+                pag_obj = cast("PageObject", pag.get_object())
+                if "/B" not in pag_obj:
+                    pag_obj[NameObject("/B")] = ArrayObject()
+                cast("ArrayObject", pag_obj["/B"]).append(
+                    new_article.indirect_reference
+                )
+            current_article = cast("DictionaryObject", current_article["/N"])
+            if current_article == first_article:
+                new_article[NameObject("/N")] = new_first.indirect_reference  # type: ignore
+                new_first[NameObject("/V")] = new_article.indirect_reference  # type: ignore
+                current_article = None
+        assert nthread.indirect_reference is not None
+        return nthread.indirect_reference
 
-        Returns:
-            An indicator if the document was decrypted and weather it was the
-            owner password or the user password.
+    def add_filtered_articles(
+        self,
+        fltr: Union[
+            Pattern[Any], str
+        ],  # thread entry from the reader's array of threads
+        pages: Dict[int, PageObject],
+        reader: PdfReader,
+    ) -> None:
         """
-        if not self._encryption:
-            raise PdfReadError("Not encrypted file")
-        # TODO: raise Exception for wrong password
-        return self._encryption.verify(password)
-
-    def decode_permissions(self, permissions_code: int) -> Dict[str, bool]:
-        """Take the permissions as an integer, return the allowed access."""
-        deprecate_with_replacement(
-            old_name="decode_permissions",
-            new_name="user_access_permissions",
-            removed_in="5.0.0",
-        )
-
-        permissions_mapping = {
-            "print": UserAccessPermissions.PRINT,
-            "modify": UserAccessPermissions.MODIFY,
-            "copy": UserAccessPermissions.EXTRACT,
-            "annotations": UserAccessPermissions.ADD_OR_MODIFY,
-            "forms": UserAccessPermissions.FILL_FORM_FIELDS,
-            "accessability": UserAccessPermissions.EXTRACT_TEXT_AND_GRAPHICS,
-            "assemble": UserAccessPermissions.ASSEMBLE_DOC,
-            "print_high_quality": UserAccessPermissions.PRINT_TO_REPRESENTATION,
-        }
+        Add articles matching the defined criteria.
 
-        return {
-            key: permissions_code & flag != 0
-            for key, flag in permissions_mapping.items()
-        }
+        Args:
+            fltr:
+            pages:
+            reader:
+        """
+        if isinstance(fltr, str):
+            fltr = re.compile(fltr)
+        elif not isinstance(fltr, Pattern):
+            fltr = re.compile("")
+        for p in pages.values():
+            pp = p.original_page
+            for a in pp.get("/B", ()):
+                thr = a.get_object().get("/T")
+                if thr is None:
+                    continue
+                else:
+                    thr = thr.get_object()
+                if thr.indirect_reference.idnum not in self._id_translated[
+                    id(reader)
+                ] and fltr.search((thr["/I"] if "/I" in thr else {}).get("/Title", "")):
+                    self._add_articles_thread(thr, pages, reader)
 
-    @property
-    def user_access_permissions(self) -> Optional[UserAccessPermissions]:
-        """Get the user access permissions for encrypted documents. Returns None if not encrypted."""
-        if self._encryption is None:
+    def _get_cloned_page(
+        self,
+        page: Union[None, int, IndirectObject, PageObject, NullObject],
+        pages: Dict[int, PageObject],
+        reader: PdfReader,
+    ) -> Optional[IndirectObject]:
+        if isinstance(page, NullObject):
             return None
-        return UserAccessPermissions(self._encryption.P)
-
-    @property
-    def is_encrypted(self) -> bool:
-        """
-        Read-only boolean property showing whether this PDF file is encrypted.
-
-        Note that this property, if true, will remain true even after the
-        :meth:`decrypt()<pypdf.PdfReader.decrypt>` method is called.
-        """
-        return TK.ENCRYPT in self.trailer
-
-    @property
-    def xfa(self) -> Optional[Dict[str, Any]]:
-        tree: Optional[TreeObject] = None
-        retval: Dict[str, Any] = {}
-        catalog = cast(DictionaryObject, self.trailer[TK.ROOT])
-
-        if "/AcroForm" not in catalog or not catalog["/AcroForm"]:
+        if isinstance(page, int):
+            _i = reader.pages[page].indirect_reference
+        elif isinstance(page, DictionaryObject) and page.get("/Type", "") == "/Page":
+            _i = page.indirect_reference
+        elif isinstance(page, IndirectObject):
+            _i = page
+        try:
+            return pages[_i.idnum].indirect_reference  # type: ignore
+        except Exception:
             return None
 
-        tree = cast(TreeObject, catalog["/AcroForm"])
-
-        if "/XFA" in tree:
-            fields = cast(ArrayObject, tree["/XFA"])
-            i = iter(fields)
-            for f in i:
-                tag = f
-                f = next(i)
-                if isinstance(f, IndirectObject):
-                    field = cast(Optional[EncodedStreamObject], f.get_object())
-                    if field:
-                        es = zlib.decompress(b_(field._data))
-                        retval[tag] = es
-        return retval
+    def _insert_filtered_annotations(
+        self,
+        annots: Union[IndirectObject, List[DictionaryObject]],
+        page: PageObject,
+        pages: Dict[int, PageObject],
+        reader: PdfReader,
+    ) -> List[Destination]:
+        outlist = ArrayObject()
+        if isinstance(annots, IndirectObject):
+            annots = cast("List[Any]", annots.get_object())
+        for an in annots:
+            ano = cast("DictionaryObject", an.get_object())
+            if (
+                ano["/Subtype"] != "/Link"
+                or "/A" not in ano
+                or cast("DictionaryObject", ano["/A"])["/S"] != "/GoTo"
+                or "/Dest" in ano
+            ):
+                if "/Dest" not in ano:
+                    outlist.append(self._add_object(ano.clone(self)))
+                else:
+                    d = ano["/Dest"]
+                    if isinstance(d, str):
+                        # it is a named dest
+                        if str(d) in self.get_named_dest_root():
+                            outlist.append(ano.clone(self).indirect_reference)
+                    else:
+                        d = cast("ArrayObject", d)
+                        p = self._get_cloned_page(d[0], pages, reader)
+                        if p is not None:
+                            anc = ano.clone(self, ignore_fields=("/Dest",))
+                            anc[NameObject("/Dest")] = ArrayObject([p] + d[1:])
+                            outlist.append(self._add_object(anc))
+            else:
+                d = cast("DictionaryObject", ano["/A"])["/D"]
+                if isinstance(d, str):
+                    # it is a named dest
+                    if str(d) in self.get_named_dest_root():
+                        outlist.append(ano.clone(self).indirect_reference)
+                else:
+                    d = cast("ArrayObject", d)
+                    p = self._get_cloned_page(d[0], pages, reader)
+                    if p is not None:
+                        anc = ano.clone(self, ignore_fields=("/D",))
+                        cast("DictionaryObject", anc["/A"])[
+                            NameObject("/D")
+                        ] = ArrayObject([p] + d[1:])
+                        outlist.append(self._add_object(anc))
+        return outlist
 
-    def add_form_topname(self, name: str) -> Optional[DictionaryObject]:
+    def _get_filtered_outline(
+        self,
+        node: Any,
+        pages: Dict[int, PageObject],
+        reader: PdfReader,
+    ) -> List[Destination]:
         """
-        Add a top level form that groups all form fields below it.
+        Extract outline item entries that are part of the specified page set.
 
         Args:
-            name: text string of the "/T" Attribute of the created object
+            node:
+            pages:
+            reader:
 
         Returns:
-            The created object. ``None`` means no object was created.
+            A list of destination objects.
         """
-        catalog = cast(DictionaryObject, self.trailer[TK.ROOT])
+        new_outline = []
+        if node is None:
+            node = NullObject()
+        node = node.get_object()
+        if node is None or isinstance(node, NullObject):
+            node = DictionaryObject()
+        if node.get("/Type", "") == "/Outlines" or "/Title" not in node:
+            node = node.get("/First", None)
+            if node is not None:
+                node = node.get_object()
+                new_outline += self._get_filtered_outline(node, pages, reader)
+        else:
+            v: Union[None, IndirectObject, NullObject]
+            while node is not None:
+                node = node.get_object()
+                o = cast("Destination", reader._build_outline_item(node))
+                v = self._get_cloned_page(cast("PageObject", o["/Page"]), pages, reader)
+                if v is None:
+                    v = NullObject()
+                o[NameObject("/Page")] = v
+                if "/First" in node:
+                    o._filtered_children = self._get_filtered_outline(
+                        node["/First"], pages, reader
+                    )
+                else:
+                    o._filtered_children = []
+                if (
+                    not isinstance(o["/Page"], NullObject)
+                    or len(o._filtered_children) > 0
+                ):
+                    new_outline.append(o)
+                node = node.get("/Next", None)
+        return new_outline
+
+    def _clone_outline(self, dest: Destination) -> TreeObject:
+        n_ol = TreeObject()
+        self._add_object(n_ol)
+        n_ol[NameObject("/Title")] = TextStringObject(dest["/Title"])
+        if not isinstance(dest["/Page"], NullObject):
+            if dest.node is not None and "/A" in dest.node:
+                n_ol[NameObject("/A")] = dest.node["/A"].clone(self)
+            else:
+                n_ol[NameObject("/Dest")] = dest.dest_array
+        # TODO: /SE
+        if dest.node is not None:
+            n_ol[NameObject("/F")] = NumberObject(dest.node.get("/F", 0))
+            n_ol[NameObject("/C")] = ArrayObject(
+                dest.node.get(
+                    "/C", [FloatObject(0.0), FloatObject(0.0), FloatObject(0.0)]
+                )
+            )
+        return n_ol
 
-        if "/AcroForm" not in catalog or not isinstance(
-            catalog["/AcroForm"], DictionaryObject
-        ):
-            return None
-        acroform = cast(DictionaryObject, catalog[NameObject("/AcroForm")])
-        if "/Fields" not in acroform:
-            # TODO: :No error returns but may be extended for XFA Forms
-            return None
+    def _insert_filtered_outline(
+        self,
+        outlines: List[Destination],
+        parent: Union[TreeObject, IndirectObject],
+        before: Union[None, TreeObject, IndirectObject] = None,
+    ) -> None:
+        for dest in outlines:
+            # TODO  : can be improved to keep A and SE entries (ignored for the moment)
+            # with np=self.add_outline_item_destination(dest,parent,before)
+            if dest.get("/Type", "") == "/Outlines" or "/Title" not in dest:
+                np = parent
+            else:
+                np = self._clone_outline(dest)
+                cast(TreeObject, parent.get_object()).insert_child(np, before, self)
+            self._insert_filtered_outline(dest._filtered_children, np, None)
+
+    def close(self) -> None:
+        """To match the functions from Merger."""
+        return
 
-        interim = DictionaryObject()
-        interim[NameObject("/T")] = TextStringObject(name)
-        interim[NameObject("/Kids")] = acroform[NameObject("/Fields")]
-        self.cache_indirect_object(
-            0,
-            max([i for (g, i) in self.resolved_objects if g == 0]) + 1,
-            interim,
-        )
-        arr = ArrayObject()
-        arr.append(interim.indirect_reference)
-        acroform[NameObject("/Fields")] = arr
-        for o in cast(ArrayObject, interim["/Kids"]):
-            obj = o.get_object()
-            if "/Parent" in obj:
-                logger_warning(
-                    f"Top Level Form Field {obj.indirect_reference} have a non-expected parent",
-                    __name__,
+    def find_outline_item(
+        self,
+        outline_item: Dict[str, Any],
+        root: Optional[OutlineType] = None,
+    ) -> Optional[List[int]]:
+        if root is None:
+            o = self.get_outline_root()
+        else:
+            o = cast("TreeObject", root)
+
+        i = 0
+        while o is not None:
+            if (
+                o.indirect_reference == outline_item
+                or o.get("/Title", None) == outline_item
+            ):
+                return [i]
+            elif "/First" in o:
+                res = self.find_outline_item(
+                    outline_item, cast(OutlineType, o["/First"])
                 )
-            obj[NameObject("/Parent")] = interim.indirect_reference
-        return interim
+                if res:
+                    return ([i] if "/Title" in o else []) + res
+            if "/Next" in o:
+                i += 1
+                o = cast(TreeObject, o["/Next"])
+            else:
+                return None
+
+    def find_bookmark(
+        self,
+        outline_item: Dict[str, Any],
+        root: Optional[OutlineType] = None,
+    ) -> Optional[List[int]]:  # deprecated
+        """
+        .. deprecated:: 2.9.0
+            Use :meth:`find_outline_item` instead.
+        """
+        return self.find_outline_item(outline_item, root)
 
-    def rename_form_topname(self, name: str) -> Optional[DictionaryObject]:
+    def reset_translation(
+        self, reader: Union[None, PdfReader, IndirectObject] = None
+    ) -> None:
         """
-        Rename top level form field that all form fields below it.
+        Reset the translation table between reader and the writer object.
+
+        Late cloning will create new independent objects.
 
         Args:
-            name: text string of the "/T" field of the created object
+            reader: PdfReader or IndirectObject referencing a PdfReader object.
+                if set to None or omitted, all tables will be reset.
+        """
+        if reader is None:
+            self._id_translated = {}
+        elif isinstance(reader, PdfReader):
+            try:
+                del self._id_translated[id(reader)]
+            except Exception:
+                pass
+        elif isinstance(reader, IndirectObject):
+            try:
+                del self._id_translated[id(reader.pdf)]
+            except Exception:
+                pass
+        else:
+            raise Exception("invalid parameter {reader}")
 
-        Returns:
-            The modified object. ``None`` means no object was modified.
+    def set_page_label(
+        self,
+        page_index_from: int,
+        page_index_to: int,
+        style: Optional[PageLabelStyle] = None,
+        prefix: Optional[str] = None,
+        start: Optional[int] = 0,
+    ) -> None:
         """
-        catalog = cast(DictionaryObject, self.trailer[TK.ROOT])
+        Set a page label to a range of pages.
 
-        if "/AcroForm" not in catalog or not isinstance(
-            catalog["/AcroForm"], DictionaryObject
-        ):
-            return None
-        acroform = cast(DictionaryObject, catalog[NameObject("/AcroForm")])
-        if "/Fields" not in acroform:
-            return None
+        Page indexes must be given starting from 0.
+        Labels must have a style, a prefix or both.
+        If to a range is not assigned any page label a decimal label starting from 1 is applied.
 
-        interim = cast(
-            DictionaryObject,
-            cast(ArrayObject, acroform[NameObject("/Fields")])[0].get_object(),
-        )
-        interim[NameObject("/T")] = TextStringObject(name)
-        return interim
+        Args:
+            page_index_from: page index of the beginning of the range starting from 0
+            page_index_to: page index of the beginning of the range starting from 0
+            style: The numbering style to be used for the numeric portion of each page label:
+
+                       * ``/D`` Decimal arabic numerals
+                       * ``/R`` Uppercase roman numerals
+                       * ``/r`` Lowercase roman numerals
+                       * ``/A`` Uppercase letters (A to Z for the first 26 pages,
+                         AA to ZZ for the next 26, and so on)
+                       * ``/a`` Lowercase letters (a to z for the first 26 pages,
+                         aa to zz for the next 26, and so on)
+
+            prefix: The label prefix for page labels in this range.
+            start:  The value of the numeric portion for the first page label
+                    in the range.
+                    Subsequent pages are numbered sequentially from this value,
+                    which must be greater than or equal to 1.
+                    Default value: 1.
+        """
+        if style is None and prefix is None:
+            raise ValueError("at least one between style and prefix must be given")
+        if page_index_from < 0:
+            raise ValueError("page_index_from must be equal or greater then 0")
+        if page_index_to < page_index_from:
+            raise ValueError(
+                "page_index_to must be equal or greater then page_index_from"
+            )
+        if page_index_to >= len(self.pages):
+            raise ValueError("page_index_to exceeds number of pages")
+        if start is not None and start != 0 and start < 1:
+            raise ValueError("if given, start must be equal or greater than one")
 
-    @property
-    def attachments(self) -> Mapping[str, List[bytes]]:
-        return LazyDict(
-            {
-                name: (self._get_attachment_list, name)
-                for name in self._list_attachments()
-            }
-        )
+        self._set_page_label(page_index_from, page_index_to, style, prefix, start)
 
-    def _list_attachments(self) -> List[str]:
+    def _set_page_label(
+        self,
+        page_index_from: int,
+        page_index_to: int,
+        style: Optional[PageLabelStyle] = None,
+        prefix: Optional[str] = None,
+        start: Optional[int] = 0,
+    ) -> None:
         """
-        Retrieves the list of filenames of file attachments.
+        Set a page label to a range of pages.
 
-        Returns:
-            list of filenames
-        """
-        catalog = cast(DictionaryObject, self.trailer["/Root"])
-        # From the catalog get the embedded file names
-        try:
-            filenames = cast(
-                ArrayObject,
-                cast(
-                    DictionaryObject,
-                    cast(DictionaryObject, catalog["/Names"])["/EmbeddedFiles"],
-                )["/Names"],
-            )
-        except KeyError:
-            return []
-        attachments_names = [f for f in filenames if isinstance(f, str)]
-        return attachments_names
-
-    def _get_attachment_list(self, name: str) -> List[bytes]:
-        out = self._get_attachments(name)[name]
-        if isinstance(out, list):
-            return out
-        return [out]
-
-    def _get_attachments(
-        self, filename: Optional[str] = None
-    ) -> Dict[str, Union[bytes, List[bytes]]]:
-        """
-        Retrieves all or selected file attachments of the PDF as a dictionary of file names
-        and the file data as a bytestring.
-
-        Args:
-            filename: If filename is None, then a dictionary of all attachments
-                will be returned, where the key is the filename and the value
-                is the content. Otherwise, a dictionary with just a single key
-                - the filename - and its content will be returned.
+        Page indexes must be given
+        starting from 0. Labels must have a style, a prefix or both. If to a
+        range is not assigned any page label a decimal label starting from 1 is
+        applied.
 
-        Returns:
-            dictionary of filename -> Union[bytestring or List[ByteString]]
-            if the filename exists multiple times a List of the different version will be provided
-        """
-        catalog = cast(DictionaryObject, self.trailer["/Root"])
-        # From the catalog get the embedded file names
-        try:
-            filenames = cast(
-                ArrayObject,
-                cast(
-                    DictionaryObject,
-                    cast(DictionaryObject, catalog["/Names"])["/EmbeddedFiles"],
-                )["/Names"],
-            )
-        except KeyError:
-            return {}
-        attachments: Dict[str, Union[bytes, List[bytes]]] = {}
-        # Loop through attachments
-        for i in range(len(filenames)):
-            f = filenames[i]
-            if isinstance(f, str):
-                if filename is not None and f != filename:
-                    continue
-                name = f
-                f_dict = filenames[i + 1].get_object()
-                f_data = f_dict["/EF"]["/F"].get_data()
-                if name in attachments:
-                    if not isinstance(attachments[name], list):
-                        attachments[name] = [attachments[name]]  # type:ignore
-                    attachments[name].append(f_data)  # type:ignore
-                else:
-                    attachments[name] = f_data
-        return attachments
+        Args:
+            page_index_from: page index of the beginning of the range starting from 0
+            page_index_to: page index of the beginning of the range starting from 0
+            style:  The numbering style to be used for the numeric portion of each page label:
+                        /D Decimal arabic numerals
+                        /R Uppercase roman numerals
+                        /r Lowercase roman numerals
+                        /A Uppercase letters (A to Z for the first 26 pages,
+                           AA to ZZ for the next 26, and so on)
+                        /a Lowercase letters (a to z for the first 26 pages,
+                           aa to zz for the next 26, and so on)
+            prefix: The label prefix for page labels in this range.
+            start:  The value of the numeric portion for the first page label
+                    in the range.
+                    Subsequent pages are numbered sequentially from this value,
+                    which must be greater than or equal to 1. Default value: 1.
+        """
+        default_page_label = DictionaryObject()
+        default_page_label[NameObject("/S")] = NameObject("/D")
+
+        new_page_label = DictionaryObject()
+        if style is not None:
+            new_page_label[NameObject("/S")] = NameObject(style)
+        if prefix is not None:
+            new_page_label[NameObject("/P")] = TextStringObject(prefix)
+        if start != 0:
+            new_page_label[NameObject("/St")] = NumberObject(start)
+
+        if NameObject(CatalogDictionary.PAGE_LABELS) not in self._root_object:
+            nums = ArrayObject()
+            nums_insert(NumberObject(0), default_page_label, nums)
+            page_labels = TreeObject()
+            page_labels[NameObject("/Nums")] = nums
+            self._root_object[NameObject(CatalogDictionary.PAGE_LABELS)] = page_labels
 
+        page_labels = cast(
+            TreeObject, self._root_object[NameObject(CatalogDictionary.PAGE_LABELS)]
+        )
+        nums = cast(ArrayObject, page_labels[NameObject("/Nums")])
 
-class LazyDict(Mapping[Any, Any]):
-    def __init__(self, *args: Any, **kw: Any) -> None:
-        self._raw_dict = dict(*args, **kw)
+        nums_insert(NumberObject(page_index_from), new_page_label, nums)
+        nums_clear_range(NumberObject(page_index_from), page_index_to, nums)
+        next_label_pos, *_ = nums_next(NumberObject(page_index_from), nums)
+        if next_label_pos != page_index_to + 1 and page_index_to + 1 < len(self.pages):
+            nums_insert(NumberObject(page_index_to + 1), default_page_label, nums)
 
-    def __getitem__(self, key: str) -> Any:
-        func, arg = self._raw_dict.__getitem__(key)
-        return func(arg)
+        page_labels[NameObject("/Nums")] = nums
+        self._root_object[NameObject(CatalogDictionary.PAGE_LABELS)] = page_labels
 
-    def __iter__(self) -> Iterator[Any]:
-        return iter(self._raw_dict)
 
-    def __len__(self) -> int:
-        return len(self._raw_dict)
+def _pdf_objectify(obj: Union[Dict[str, Any], str, int, List[Any]]) -> PdfObject:
+    if isinstance(obj, PdfObject):
+        return obj
+    if isinstance(obj, dict):
+        to_add = DictionaryObject()
+        for key, value in obj.items():
+            name_key = NameObject(key)
+            casted_value = _pdf_objectify(value)
+            to_add[name_key] = casted_value
+        return to_add
+    elif isinstance(obj, list):
+        return ArrayObject(_pdf_objectify(el) for el in obj)
+    elif isinstance(obj, str):
+        if obj.startswith("/"):
+            return NameObject(obj)
+        else:
+            return TextStringObject(obj)
+    elif isinstance(obj, (int, float)):
+        return FloatObject(obj)
+    else:
+        raise NotImplementedError(
+            f"type(obj)={type(obj)} could not be casted to PdfObject"
+        )
+
 
-    def __str__(self) -> str:
-        return f"LazyDict(keys={list(self.keys())})"
+def _create_outline_item(
+    action_ref: Union[None, IndirectObject],
+    title: str,
+    color: Union[Tuple[float, float, float], str, None],
+    italic: bool,
+    bold: bool,
+) -> TreeObject:
+    outline_item = TreeObject()
+    if action_ref is not None:
+        outline_item[NameObject("/A")] = action_ref
+    outline_item.update(
+        {
+            NameObject("/Title"): create_string_object(title),
+        }
+    )
+    if color:
+        if isinstance(color, str):
+            color = hex_to_rgb(color)
+        outline_item.update(
+            {NameObject("/C"): ArrayObject([FloatObject(c) for c in color])}
+        )
+    if italic or bold:
+        format_flag = 0
+        if italic:
+            format_flag += 1
+        if bold:
+            format_flag += 2
+        outline_item.update({NameObject("/F"): NumberObject(format_flag)})
+    return outline_item
```

### Comparing `pypdf-4.1.0/pypdf/_text_extraction/__init__.py` & `pypdf-4.2.0/pypdf/_text_extraction/__init__.py`

 * *Files identical despite different names*

### Comparing `pypdf-4.1.0/pypdf/_text_extraction/_layout_mode/_fixed_width_page.py` & `pypdf-4.2.0/pypdf/_text_extraction/_layout_mode/_fixed_width_page.py`

 * *Files identical despite different names*

### Comparing `pypdf-4.1.0/pypdf/_text_extraction/_layout_mode/_font.py` & `pypdf-4.2.0/pypdf/_text_extraction/_layout_mode/_font.py`

 * *Files identical despite different names*

### Comparing `pypdf-4.1.0/pypdf/_text_extraction/_layout_mode/_font_widths.py` & `pypdf-4.2.0/pypdf/_text_extraction/_layout_mode/_font_widths.py`

 * *Files identical despite different names*

### Comparing `pypdf-4.1.0/pypdf/_text_extraction/_layout_mode/_text_state_manager.py` & `pypdf-4.2.0/pypdf/_text_extraction/_layout_mode/_text_state_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,15 @@
     def set_state_param(self, op: bytes, value: Union[float, List[Any]]) -> None:
         """
         Set a text state parameter. Supports Tc, Tz, Tw, TL, and Ts operators.
 
         Args:
             op: operator read from PDF stream as bytes. No action is taken
                 for unsupported operators (see supported operators above).
-            value (float | List[Any]): new paramater value. If a list,
+            value (float | List[Any]): new parameter value. If a list,
                 value[0] is used.
         """
         if op not in [b"Tc", b"Tz", b"Tw", b"TL", b"Ts"]:
             return
         self.__setattr__(op.decode(), value[0] if isinstance(value, list) else value)
 
     def set_font(self, font: Font, size: float) -> None:
```

### Comparing `pypdf-4.1.0/pypdf/_text_extraction/_layout_mode/_text_state_params.py` & `pypdf-4.2.0/pypdf/_text_extraction/_layout_mode/_text_state_params.py`

 * *Files identical despite different names*

### Comparing `pypdf-4.1.0/pypdf/_utils.py` & `pypdf-4.2.0/pypdf/_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,22 +107,22 @@
         else:
             if text[-5:] == "+0000":
                 d = d.replace(tzinfo=timezone.utc)
             return d
     raise ValueError(f"Can not convert date: {orgtext}")
 
 
-def _get_max_pdf_version_header(header1: bytes, header2: bytes) -> bytes:
+def _get_max_pdf_version_header(header1: str, header2: str) -> str:
     versions = (
-        b"%PDF-1.3",
-        b"%PDF-1.4",
-        b"%PDF-1.5",
-        b"%PDF-1.6",
-        b"%PDF-1.7",
-        b"%PDF-2.0",
+        "%PDF-1.3",
+        "%PDF-1.4",
+        "%PDF-1.5",
+        "%PDF-1.6",
+        "%PDF-1.7",
+        "%PDF-2.0",
     )
     pdf_header_indices = []
     if header1 in versions:
         pdf_header_indices.append(versions.index(header1))
     if header2 in versions:
         pdf_header_indices.append(versions.index(header2))
     if len(pdf_header_indices) == 0:
```

### Comparing `pypdf-4.1.0/pypdf/_xobj_image_helpers.py` & `pypdf-4.2.0/pypdf/_xobj_image_helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,15 @@
         )
     if isinstance(color_space, NullObject):
         return "", False
     if isinstance(color_space, str):
         pass
     elif not isinstance(color_space, list):
         raise PdfReadError(
-            "can not interprete colorspace", color_space
+            "Cannot interpret colorspace", color_space
         )  # pragma: no cover
     elif color_space[0].startswith("/Cal"):  # /CalRGB and /CalGray
         color_space = "/Device" + color_space[0][4:]
     elif color_space[0] == "/ICCBased":
         icc_profile = color_space[1].get_object()
         color_components = cast(int, icc_profile["/N"])
         color_space = icc_profile.get("/Alternate", "")
```

### Comparing `pypdf-4.1.0/pypdf/annotations/__init__.py` & `pypdf-4.2.0/pypdf/annotations/__init__.py`

 * *Files identical despite different names*

### Comparing `pypdf-4.1.0/pypdf/annotations/_base.py` & `pypdf-4.2.0/pypdf/annotations/_base.py`

 * *Files identical despite different names*

### Comparing `pypdf-4.1.0/pypdf/annotations/_markup_annotations.py` & `pypdf-4.2.0/pypdf/annotations/_markup_annotations.py`

 * *Files identical despite different names*

### Comparing `pypdf-4.1.0/pypdf/annotations/_non_markup_annotations.py` & `pypdf-4.2.0/pypdf/annotations/_non_markup_annotations.py`

 * *Files identical despite different names*

### Comparing `pypdf-4.1.0/pypdf/constants.py` & `pypdf-4.2.0/pypdf/constants.py`

 * *Files 17% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 
 PDF Reference, sixth edition, Version 1.7, 2006.
 """
 
 from enum import IntFlag, auto
 from typing import Dict, Tuple
 
+from ._utils import deprecate_with_replacement
+
 
 class Core:
     """Keywords that don't quite belong anywhere else."""
 
     OUTLINES = "/Outlines"
     THREADS = "/Threads"
     PAGE = "/Page"
@@ -123,27 +125,86 @@
         return result
 
     @classmethod
     def all(cls) -> "UserAccessPermissions":
         return cls((2**32 - 1) - cls.R1 - cls.R2)
 
 
-class Ressources:
-    """TABLE 3.30 Entries in a resource dictionary."""
+class Resources:
+    """
+    TABLE 3.30 Entries in a resource dictionary.
+    used to be Ressources
+    """
 
     EXT_G_STATE = "/ExtGState"  # dictionary, optional
     COLOR_SPACE = "/ColorSpace"  # dictionary, optional
     PATTERN = "/Pattern"  # dictionary, optional
     SHADING = "/Shading"  # dictionary, optional
     XOBJECT = "/XObject"  # dictionary, optional
     FONT = "/Font"  # dictionary, optional
     PROC_SET = "/ProcSet"  # array, optional
     PROPERTIES = "/Properties"  # dictionary, optional
 
 
+class Ressources:  # deprecated
+    """
+    Use :class: `Resources` instead.
+
+    .. deprecated:: 5.0.0
+    """
+
+    @classmethod  # type: ignore
+    @property
+    def EXT_G_STATE(cls) -> str:
+        deprecate_with_replacement("Ressources", "Resources", "5.0.0")
+        return "/ExtGState"  # dictionary, optional
+
+    @classmethod  # type: ignore
+    @property
+    def COLOR_SPACE(cls) -> str:
+        deprecate_with_replacement("Ressources", "Resources", "5.0.0")
+        return "/ColorSpace"  # dictionary, optional
+
+    @classmethod  # type: ignore
+    @property
+    def PATTERN(cls) -> str:
+        deprecate_with_replacement("Ressources", "Resources", "5.0.0")
+        return "/Pattern"  # dictionary, optional
+
+    @classmethod  # type: ignore
+    @property
+    def SHADING(cls) -> str:
+        deprecate_with_replacement("Ressources", "Resources", "5.0.0")
+        return "/Shading"  # dictionary, optional
+
+    @classmethod  # type: ignore
+    @property
+    def XOBJECT(cls) -> str:
+        deprecate_with_replacement("Ressources", "Resources", "5.0.0")
+        return "/XObject"  # dictionary, optional
+
+    @classmethod  # type: ignore
+    @property
+    def FONT(cls) -> str:
+        deprecate_with_replacement("Ressources", "Resources", "5.0.0")
+        return "/Font"  # dictionary, optional
+
+    @classmethod  # type: ignore
+    @property
+    def PROC_SET(cls) -> str:
+        deprecate_with_replacement("Ressources", "Resources", "5.0.0")
+        return "/ProcSet"  # array, optional
+
+    @classmethod  # type: ignore
+    @property
+    def PROPERTIES(cls) -> str:
+        deprecate_with_replacement("Ressources", "Resources", "5.0.0")
+        return "/Properties"  # dictionary, optional
+
+
 class PagesAttributes:
     """Page Attributes, Table 6.2, Page 52."""
 
     TYPE = "/Type"  # name, required; must be /Pages
     KIDS = "/Kids"  # array, required; List of indirect references
     COUNT = "/Count"  # integer, required; the number of all nodes und this node
     PARENT = "/Parent"  # dictionary, required; indirect reference to pages object
@@ -625,15 +686,15 @@
     GraphicsStateParameters,
     ImageAttributes,
     FileSpecificationDictionaryEntries,
     LzwFilterParameters,
     PageAttributes,
     PageLayouts,
     PagesAttributes,
-    Ressources,
+    Resources,
     StreamAttributes,
     TrailerKeys,
     TypArguments,
     TypFitArguments,
 )
```

### Comparing `pypdf-4.1.0/pypdf/errors.py` & `pypdf-4.2.0/pypdf/errors.py`

 * *Files identical despite different names*

### Comparing `pypdf-4.1.0/pypdf/filters.py` & `pypdf-4.2.0/pypdf/filters.py`

 * *Files 2% similar despite different names*

```diff
@@ -281,15 +281,16 @@
         if isinstance(data, str):
             data = data.encode()
         retval = b""
         hex_pair = b""
         index = 0
         while True:
             if index >= len(data):
-                raise PdfStreamError("Unexpected EOD in ASCIIHexDecode")
+                logger_warning("missing EOD in ASCIIHexDecode, check if output is OK", __name__)
+                break  # reach End Of String even if no EOD
             char = data[index : index + 1]
             if char == b">":
                 break
             elif char.isspace():
                 index += 1
                 continue
             hex_pair += char
@@ -336,15 +337,16 @@
         """
         # decode_parms is unused here
 
         lst = []
         index = 0
         while True:
             if index >= len(data):
-                raise PdfStreamError("Unexpected EOD in RunLengthDecode")
+                logger_warning("missing EOD in RunLengthDecode, check if output is OK", __name__)
+                break  # reach End Of String even if no EOD
             length = data[index]
             index += 1
             if length == 128:
                 if index < len(data):
                     raise PdfStreamError("early EOD in RunLengthDecode")
                 else:
                     break
@@ -593,54 +595,54 @@
         if "decodeParms" in kwargs:  # deprecated
             deprecate_with_replacement("decodeParms", "parameters", "4.0.0")
             decode_parms = kwargs["decodeParms"]
         if isinstance(decode_parms, ArrayObject):  # deprecated
             deprecation_no_replacement(
                 "decode_parms being an ArrayObject", removed_in="3.15.5"
             )
-        parms = CCITTFaxDecode._get_parameters(decode_parms, height)
+        params = CCITTFaxDecode._get_parameters(decode_parms, height)
 
         img_size = len(data)
         tiff_header_struct = "<2shlh" + "hhll" * 8 + "h"
         tiff_header = struct.pack(
             tiff_header_struct,
             b"II",  # Byte order indication: Little endian
             42,  # Version number (always 42)
             8,  # Offset to first IFD
             8,  # Number of tags in IFD
             256,
             4,
             1,
-            parms.columns,  # ImageWidth, LONG, 1, width
+            params.columns,  # ImageWidth, LONG, 1, width
             257,
             4,
             1,
-            parms.rows,  # ImageLength, LONG, 1, length
+            params.rows,  # ImageLength, LONG, 1, length
             258,
             3,
             1,
             1,  # BitsPerSample, SHORT, 1, 1
             259,
             3,
             1,
-            parms.group,  # Compression, SHORT, 1, 4 = CCITT Group 4 fax encoding
+            params.group,  # Compression, SHORT, 1, 4 = CCITT Group 4 fax encoding
             262,
             3,
             1,
             0,  # Thresholding, SHORT, 1, 0 = WhiteIsZero
             273,
             4,
             1,
             struct.calcsize(
                 tiff_header_struct
             ),  # StripOffsets, LONG, 1, length of header
             278,
             4,
             1,
-            parms.rows,  # RowsPerStrip, LONG, 1, length
+            params.rows,  # RowsPerStrip, LONG, 1, length
             279,
             4,
             1,
             img_size,  # StripByteCounts, LONG, 1, size of image
             0,  # last IFD
         )
 
@@ -811,17 +813,24 @@
     elif lfilters == FT.CCITT_FAX_DECODE:
         img, image_format, extension, invert_color = (
             Image.open(BytesIO(data), formats=("TIFF",)),
             "TIFF",
             ".tiff",
             False,
         )
+    elif mode == "CMYK":
+        img, image_format, extension, invert_color = (
+            Image.frombytes(mode, size, data),
+            "TIFF",
+            ".tif",
+            False,
+        )
+    elif mode == "":
+        raise PdfReadError(f"ColorSpace field not found in {x_object_obj}")
     else:
-        if mode == "":
-            raise PdfReadError(f"ColorSpace field not found in {x_object_obj}")
         img, image_format, extension, invert_color = (
             Image.frombytes(mode, size, data),
             "PNG",
             ".png",
             False,
         )
     # CMYK image and other colorspaces without decode
```

### Comparing `pypdf-4.1.0/pypdf/generic/__init__.py` & `pypdf-4.2.0/pypdf/generic/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -314,15 +314,15 @@
         Add a highlight annotation to the document.
 
         Args:
             rect: Array of four integers ``[xLL, yLL, xUR, yUR]``
                 specifying the highlighted area
             quad_points: An ArrayObject of 8 FloatObjects. Must match a word or
                 a group of words, otherwise no highlight will be shown.
-            highlight_color: The color used for the hightlight
+            highlight_color: The color used for the highlight.
 
         Returns:
             A dictionary object representing the annotation.
         """
         deprecate_with_replacement(
             "AnnotationBuilder.highlight", "pypdf.annotations.Highlight", "4.0.0"
         )
```

### Comparing `pypdf-4.1.0/pypdf/generic/_base.py` & `pypdf-4.2.0/pypdf/generic/_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -611,15 +611,18 @@
                 "the encryption_key parameter of write_to_stream", "5.0.0"
             )
         stream.write(self.renumber())
 
     def renumber(self) -> bytes:
         out = self[0].encode("utf-8")
         if out != b"/":
-            deprecate_no_replacement(f"Incorrect first char in NameObject, should start with '/': ({self})", "6.0.0")
+            deprecate_no_replacement(
+                f"Incorrect first char in NameObject, should start with '/': ({self})",
+                "6.0.0",
+            )
         for c in self[1:]:
             if c > "~":
                 for x in c.encode("utf-8"):
                     out += f"#{x:02X}".encode()
             else:
                 try:
                     out += self.renumber_table[c]
@@ -636,38 +639,45 @@
                 i = sin.find(b"#", i + 1)
             except ValueError:
                 # if the 2 characters after # can not be converted to hex
                 # we change nothing and carry on
                 i = i + 1
         return sin
 
+    CHARSETS = ("utf-8", "gbk", "latin1")
+
     @staticmethod
     def read_from_stream(stream: StreamType, pdf: Any) -> "NameObject":  # PdfReader
         name = stream.read(1)
         if name != NameObject.surfix:
             raise PdfReadError("name read error")
         name += read_until_regex(stream, NameObject.delimiter_pattern)
         try:
             # Name objects should represent irregular characters
             # with a '#' followed by the symbol's hex number
             name = NameObject.unnumber(name)
-            for enc in ("utf-8", "gbk"):
+            for enc in NameObject.CHARSETS:
                 try:
                     ret = name.decode(enc)
                     return NameObject(ret)
                 except Exception:
                     pass
             raise UnicodeDecodeError("", name, 0, 0, "Code Not Found")
         except (UnicodeEncodeError, UnicodeDecodeError) as e:
             if not pdf.strict:
-                logger_warning(f"Illegal character in Name Object ({name!r})", __name__)
+                logger_warning(
+                    f"Illegal character in NameObject ({name!r}), "
+                    "you may need to adjust NameObject.CHARSETS",
+                    __name__,
+                )
                 return NameObject(name.decode("charmap"))
             else:
                 raise PdfReadError(
-                    f"Illegal character in Name Object ({name!r})"
+                    f"Illegal character in NameObject ({name!r}). "
+                    "You may need to adjust NameObject.CHARSETS.",
                 ) from e
 
 
 def encode_pdfdocencoding(unicode_string: str) -> bytes:
     retval = bytearray()
     for c in unicode_string:
         try:
```

### Comparing `pypdf-4.1.0/pypdf/generic/_data_structures.py` & `pypdf-4.2.0/pypdf/generic/_data_structures.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 
 
 __author__ = "Mathieu Fenniak"
 __author_email__ = "biziqe@mathieu.fenniak.net"
 
 import logging
 import re
+import sys
 from io import BytesIO
 from typing import (
     Any,
     Callable,
     Dict,
     Iterable,
     List,
@@ -42,15 +43,15 @@
     Sequence,
     Set,
     Tuple,
     Union,
     cast,
 )
 
-from .._protocols import PdfReaderProtocol, PdfWriterProtocol
+from .._protocols import PdfReaderProtocol, PdfWriterProtocol, XmpInformationProtocol
 from .._utils import (
     WHITESPACES,
     StreamType,
     b_,
     deprecate_no_replacement,
     deprecate_with_replacement,
     logger_warning,
@@ -66,25 +67,31 @@
 from ..constants import FilterTypes as FT
 from ..constants import StreamAttributes as SA
 from ..constants import TypArguments as TA
 from ..constants import TypFitArguments as TF
 from ..errors import STREAM_TRUNCATED_PREMATURELY, PdfReadError, PdfStreamError
 from ._base import (
     BooleanObject,
+    ByteStringObject,
     FloatObject,
     IndirectObject,
     NameObject,
     NullObject,
     NumberObject,
     PdfObject,
     TextStringObject,
 )
 from ._fit import Fit
 from ._utils import read_hex_string_from_stream, read_string_from_stream
 
+if sys.version_info >= (3, 11):
+    from typing import Self
+else:
+    from typing_extensions import Self
+
 logger = logging.getLogger(__name__)
 NumberSigns = b"+-"
 IndirectPattern = re.compile(rb"[+-]?(\d+)\s+(\d+)\s+R[^a-zA-Z]")
 
 
 class ArrayObject(List[Any], PdfObject):
     def clone(
@@ -117,14 +124,73 @@
                 arr.append(data)
         return arr
 
     def items(self) -> Iterable[Any]:
         """Emulate DictionaryObject.items for a list (index, object)."""
         return enumerate(self)
 
+    def _to_lst(self, lst: Any) -> List[Any]:
+        # Convert to list, internal
+        if isinstance(lst, (list, tuple, set)):
+            pass
+        elif isinstance(lst, PdfObject):
+            lst = [lst]
+        elif isinstance(lst, str):
+            if lst[0] == "/":
+                lst = [NameObject(lst)]
+            else:
+                lst = [TextStringObject(lst)]
+        elif isinstance(lst, bytes):
+            lst = [ByteStringObject(lst)]
+        else:  # for numbers,...
+            lst = [lst]
+        return lst
+
+    def __add__(self, lst: Any) -> "ArrayObject":
+        """
+        Allow extension by adding list or add one element only
+
+        Args:
+            lst: any list, tuples are extended the list.
+            other types(numbers,...) will be appended.
+            if str is passed it will be converted into TextStringObject
+            or NameObject (if starting with "/")
+            if bytes is passed it will be converted into ByteStringObject
+
+        Returns:
+            ArrayObject with all elements
+        """
+        temp = ArrayObject(self)
+        temp.extend(self._to_lst(lst))
+        return temp
+
+    def __iadd__(self, lst: Any) -> Self:
+        """
+         Allow extension by adding list or add one element only
+
+        Args:
+            lst: any list, tuples are extended the list.
+            other types(numbers,...) will be appended.
+            if str is passed it will be converted into TextStringObject
+            or NameObject (if starting with "/")
+            if bytes is passed it will be converted into ByteStringObject
+        """
+        self.extend(self._to_lst(lst))
+        return self
+
+    def __isub__(self, lst: Any) -> Self:
+        """Allow to remove items"""
+        for x in self._to_lst(lst):
+            try:
+                x = self.index(x)
+                del self[x]
+            except ValueError:
+                pass
+        return self
+
     def write_to_stream(
         self, stream: StreamType, encryption_key: Union[None, str, bytes] = None
     ) -> None:
         if encryption_key is not None:  # deprecated
             deprecate_no_replacement(
                 "the encryption_key parameter of write_to_stream", "5.0.0"
             )
@@ -297,14 +363,38 @@
                         if hasattr(v, "clone")
                         else v
                     )
 
     def raw_get(self, key: Any) -> Any:
         return dict.__getitem__(self, key)
 
+    def get_inherited(self, key: str, default: Any = None) -> Any:
+        """
+        Returns the value of a key or from the parent if not found.
+        If not found returns default.
+
+        Args:
+            key: string identifying the field to return
+
+            default: default value to return
+
+        Returns:
+            Current key or inherited one, otherwise default value.
+        """
+        if key in self:
+            return self[key]
+        try:
+            if "/Parent" not in self:
+                return default
+            raise KeyError("not present")
+        except KeyError:
+            return cast("DictionaryObject", self["/Parent"].get_object()).get_inherited(
+                key, default
+            )
+
     def __setitem__(self, key: Any, value: Any) -> Any:
         if not isinstance(key, PdfObject):
             raise ValueError("key must be PdfObject")
         if not isinstance(value, PdfObject):
             raise ValueError("value must be PdfObject")
         return dict.__setitem__(self, key, value)
 
@@ -315,24 +405,23 @@
             raise ValueError("value must be PdfObject")
         return dict.setdefault(self, key, value)  # type: ignore
 
     def __getitem__(self, key: Any) -> PdfObject:
         return dict.__getitem__(self, key).get_object()
 
     @property
-    def xmp_metadata(self) -> Optional[PdfObject]:
+    def xmp_metadata(self) -> Optional[XmpInformationProtocol]:
         """
         Retrieve XMP (Extensible Metadata Platform) data relevant to the this
         object, if available.
 
-        Stability: Added in v1.12, will exist for all future v1.x releases.
-        See Table 315 – Additional entries in a metadata stream dictionary
+        See Table 347 — Additional entries in a metadata stream dictionary.
 
         Returns:
-          Returns a {@link #xmp.XmpInformation XmlInformation} instance
+          Returns a :class:`~pypdf.xmp.XmpInformation` instance
           that can be used to access XMP metadata from the document.  Can also
           return None if no metadata was found on the document root.
         """
         from ..xmp import XmpInformation
 
         metadata = self.get("/Metadata", None)
         if metadata is None:
@@ -366,22 +455,22 @@
         stream: StreamType,
         pdf: Optional[PdfReaderProtocol],
         forced_encoding: Union[None, str, List[str], Dict[int, str]] = None,
     ) -> "DictionaryObject":
         def get_next_obj_pos(
             p: int, p1: int, rem_gens: List[int], pdf: PdfReaderProtocol
         ) -> int:
-            loc = pdf.xref[rem_gens[0]]
-            for o in loc:
-                if p1 > loc[o] and p < loc[o]:
-                    p1 = loc[o]
-            if len(rem_gens) == 1:
-                return p1
-            else:
-                return get_next_obj_pos(p, p1, rem_gens[1:], pdf)
+            out = p1
+            for gen in rem_gens:
+                loc = pdf.xref[gen]
+                try:
+                    out = min(out, min([x for x in loc.values() if p < x <= p1]))
+                except ValueError:
+                    pass
+            return out
 
         def read_unsized_from_stream(
             stream: StreamType, pdf: PdfReaderProtocol
         ) -> bytes:
             # we are just pointing at beginning of the stream
             eon = get_next_obj_pos(stream.tell(), 2**32, list(pdf.xref), pdf) - 1
             curr = stream.tell()
@@ -830,35 +919,35 @@
         from ..filters import FlateDecode
 
         if SA.FILTER in self:
             f = self[SA.FILTER]
             if isinstance(f, ArrayObject):
                 f = ArrayObject([NameObject(FT.FLATE_DECODE), *f])
                 try:
-                    parms = ArrayObject(
+                    params = ArrayObject(
                         [NullObject(), *self.get(SA.DECODE_PARMS, ArrayObject())]
                     )
                 except TypeError:
                     # case of error where the * operator is not working (not an array
-                    parms = ArrayObject(
+                    params = ArrayObject(
                         [NullObject(), self.get(SA.DECODE_PARMS, ArrayObject())]
                     )
             else:
                 f = ArrayObject([NameObject(FT.FLATE_DECODE), f])
-                parms = ArrayObject(
+                params = ArrayObject(
                     [NullObject(), self.get(SA.DECODE_PARMS, NullObject())]
                 )
         else:
             f = NameObject(FT.FLATE_DECODE)
-            parms = None
+            params = None
         retval = EncodedStreamObject()
         retval.update(self)
         retval[NameObject(SA.FILTER)] = f
-        if parms is not None:
-            retval[NameObject(SA.DECODE_PARMS)] = parms
+        if params is not None:
+            retval[NameObject(SA.DECODE_PARMS)] = params
         retval._data = FlateDecode.encode(b_(self._data), level)
         return retval
 
 
 class DecodedStreamObject(StreamObject):
     pass
 
@@ -899,28 +988,31 @@
             raise PdfReadError(
                 "Streams encoded with different filter from only FlateDecode is not supported"
             )
 
 
 class ContentStream(DecodedStreamObject):
     """
-    In order to be fast, this datastructure can contain either:
+    In order to be fast, this data structure can contain either:
+
     * raw data in ._data
-    * parsed stream operations in ._operations
+    * parsed stream operations in ._operations.
 
-    At any time, ContentStream object can either have one or both of those fields defined,
-    and zero or one of those fields set to None.
+    At any time, ContentStream object can either have both of those fields defined,
+    or one field defined and the other set to None.
 
-    Those fields are "rebuilt" lazily, when accessed:
-    * when .get_data() is called, if ._data is None, it is rebuilt from ._operations
-    * when .operations is called, if ._operations is None, it is rebuilt from ._data
-
-    On the other side, those fields can be invalidated:
-    * when .set_data() is called, ._operations is set to None
-    * when .operations is set, ._data is set to None
+    These fields are "rebuilt" lazily, when accessed:
+
+    * when .get_data() is called, if ._data is None, it is rebuilt from ._operations.
+    * when .operations is called, if ._operations is None, it is rebuilt from ._data.
+
+    Conversely, these fields can be invalidated:
+
+    * when .set_data() is called, ._operations is set to None.
+    * when .operations is set, ._data is set to None.
     """
 
     def __init__(
         self,
         stream: Any,
         pdf: Any,
         forced_encoding: Union[None, str, List[str], Dict[int, str]] = None,
@@ -1160,15 +1252,15 @@
         self._data = b""
 
     def isolate_graphics_state(self) -> None:
         if self._operations:
             self._operations.insert(0, ([], "q"))
             self._operations.append(([], "Q"))
         elif self._data:
-            self._data = b"q\n" + b_(self._data) + b"Q\n"
+            self._data = b"q\n" + b_(self._data) + b"\nQ\n"
 
     # This overrides the parent method:
     def write_to_stream(
         self, stream: StreamType, encryption_key: Union[None, str, bytes] = None
     ) -> None:
         if not self._data and self._operations:
             self.get_data()  # this ensures ._data is rebuilt
@@ -1344,24 +1436,23 @@
     Raises:
         PdfReadError: If destination type is invalid.
     """
 
     node: Optional[
         DictionaryObject
     ] = None  # node provide access to the original Object
-    childs: List[
-        Any
-    ] = []  # used in PdfWriter - TODO: should be children  # noqa: RUF012
 
     def __init__(
         self,
         title: str,
         page: Union[NumberObject, IndirectObject, NullObject, DictionaryObject],
         fit: Fit,
     ) -> None:
+        self._filtered_children: List[Any] = []  # used in PdfWriter
+
         typ = fit.fit_type
         args = fit.fit_args
 
         DictionaryObject.__init__(self)
         self[NameObject("/Title")] = TextStringObject(title)
         self[NameObject("/Page")] = page
         self[NameObject("/Type")] = typ
```

### Comparing `pypdf-4.1.0/pypdf/generic/_fit.py` & `pypdf-4.2.0/pypdf/generic/_fit.py`

 * *Files identical despite different names*

### Comparing `pypdf-4.1.0/pypdf/generic/_outline.py` & `pypdf-4.2.0/pypdf/generic/_outline.py`

 * *Files identical despite different names*

### Comparing `pypdf-4.1.0/pypdf/generic/_rectangle.py` & `pypdf-4.2.0/pypdf/generic/_rectangle.py`

 * *Files identical despite different names*

### Comparing `pypdf-4.1.0/pypdf/generic/_utils.py` & `pypdf-4.2.0/pypdf/generic/_utils.py`

 * *Files identical despite different names*

### Comparing `pypdf-4.1.0/pypdf/generic/_viewerpref.py` & `pypdf-4.2.0/pypdf/generic/_viewerpref.py`

 * *Files 6% similar despite different names*

```diff
@@ -55,24 +55,34 @@
             raise ValueError(f"{v} is not par of acceptable values")
         self[NameObject(key)] = NameObject(v)
 
     def _get_arr(self, key: str, deft: Optional[List[Any]]) -> NumberObject:
         return self.get(key, None if deft is None else ArrayObject(deft))
 
     def _set_arr(self, key: str, v: Optional[ArrayObject]) -> None:
+        if v is None:
+            try:
+                del self[NameObject(key)]
+            except KeyError:
+                pass
+            return
         if not isinstance(v, ArrayObject):
             raise ValueError("ArrayObject is expected")
         self[NameObject(key)] = v
 
     def _get_int(self, key: str, deft: Optional[NumberObject]) -> NumberObject:
         return self.get(key, deft)
 
     def _set_int(self, key: str, v: int) -> None:
         self[NameObject(key)] = NumberObject(v)
 
+    @property
+    def PRINT_SCALING(self) -> NameObject:
+        return NameObject("/PrintScaling")
+
     def __new__(cls: Any, value: Any = None) -> "ViewerPreferences":
         def _add_prop_bool(key: str, deft: Optional[BooleanObject]) -> property:
             return property(
                 lambda self: self._get_bool(key, deft),
                 lambda self, v: self._set_bool(key, v),
                 None,
                 f"""
@@ -136,14 +146,16 @@
         cls.duplex = _add_prop_name(
             "/Duplex", ["/Simplex", "/DuplexFlipShortEdge", "/DuplexFlipLongEdge"], None
         )
         cls.pick_tray_by_pdfsize = _add_prop_bool("/PickTrayByPDFSize", None)
         cls.print_pagerange = _add_prop_arr("/PrintPageRange", None)
         cls.num_copies = _add_prop_int("/NumCopies", None)
 
+        cls.enforce = _add_prop_arr("/Enforce", ArrayObject())
+
         return DictionaryObject.__new__(cls)
 
     def __init__(self, obj: Optional[DictionaryObject] = None) -> None:
         super().__init__(self)
         if obj is not None:
             self.update(obj.items())
         try:
```

### Comparing `pypdf-4.1.0/pypdf/pagerange.py` & `pypdf-4.2.0/pypdf/pagerange.py`

 * *Files identical despite different names*

### Comparing `pypdf-4.1.0/pypdf/papersizes.py` & `pypdf-4.2.0/pypdf/papersizes.py`

 * *Files identical despite different names*

### Comparing `pypdf-4.1.0/pypdf/types.py` & `pypdf-4.2.0/pypdf/types.py`

 * *Files identical despite different names*

### Comparing `pypdf-4.1.0/pypdf/xmp.py` & `pypdf-4.2.0/pypdf/xmp.py`

 * *Files identical despite different names*

### Comparing `pypdf-4.1.0/pyproject.toml` & `pypdf-4.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     "Programming Language :: Python :: 3.12",
     "Operating System :: OS Independent",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Typing :: Typed",
 ]
 
 dependencies = [
-    "typing_extensions >= 3.7.4.3; python_version < '3.10'",
+    "typing_extensions >= 4.0; python_version < '3.11'",
     "dataclasses; python_version < '3.7'",
 ]
 
 [project.urls]
 Documentation = "https://pypdf.readthedocs.io/en/latest/"
 Source = "https://github.com/py-pdf/pypdf"
 "Bug Reports" = "https://github.com/py-pdf/pypdf/issues"
```

### Comparing `pypdf-4.1.0/PKG-INFO` & `pypdf-4.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypdf
-Version: 4.1.0
+Version: 4.2.0
 Summary: A pure-python PDF library capable of splitting, merging, cropping, and transforming PDF files
 Author-email: Mathieu Fenniak <biziqe@mathieu.fenniak.net>
 Maintainer-email: Martin Thoma <info@martin-thoma.de>
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
-Requires-Dist: typing_extensions >= 3.7.4.3; python_version < '3.10'
+Requires-Dist: typing_extensions >= 4.0; python_version < '3.11'
 Requires-Dist: dataclasses; python_version < '3.7'
 Requires-Dist: cryptography ; extra == "crypto" and ( python_version >= '3.7')
 Requires-Dist: PyCryptodome ; extra == "crypto" and ( python_version == '3.6')
 Requires-Dist: black ; extra == "dev"
 Requires-Dist: pip-tools ; extra == "dev"
 Requires-Dist: pre-commit<2.18.0 ; extra == "dev"
 Requires-Dist: pytest-cov ; extra == "dev"
```

