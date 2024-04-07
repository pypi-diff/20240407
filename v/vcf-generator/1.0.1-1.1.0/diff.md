# Comparing `tmp/vcf_generator-1.0.1.tar.gz` & `tmp/vcf_generator-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vcf_generator-1.0.1.tar", max compression
+gzip compressed data, was "vcf_generator-1.1.0.tar", max compression
```

## Comparing `vcf_generator-1.0.1.tar` & `vcf_generator-1.1.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1062 2024-04-02 06:27:52.338006 vcf_generator-1.0.1/LICENSE
--rw-r--r--   0        0        0     3157 2024-04-02 06:27:52.338006 vcf_generator-1.0.1/README.md
--rw-r--r--   0        0        0      894 2024-04-02 06:27:52.338006 vcf_generator-1.0.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-02 06:27:52.338006 vcf_generator-1.0.1/tests/__init__.py
--rw-r--r--   0        0        0      896 2024-04-02 06:27:52.338006 vcf_generator-1.0.1/tests/addres_test.py
--rw-r--r--   0        0        0     3193 2024-04-02 06:27:52.338006 vcf_generator-1.0.1/tests/contact_test.py
--rw-r--r--   0        0        0      175 2024-04-02 06:27:52.338006 vcf_generator-1.0.1/tests/email_test.py
--rw-r--r--   0        0        0     4872 2024-04-02 06:27:52.338006 vcf_generator-1.0.1/tests/gen_contacts_test.py
--rw-r--r--   0        0        0     3844 2024-04-02 06:27:52.338006 vcf_generator-1.0.1/tests/gen_vcards_test.py
--rw-r--r--   0        0        0      321 2024-04-02 06:27:52.338006 vcf_generator-1.0.1/tests/phone_number_test.py
--rw-r--r--   0        0        0       21 2024-04-02 06:27:52.338006 vcf_generator-1.0.1/vcf_generator/__init__.py
--rw-r--r--   0        0        0     1725 2024-04-02 06:27:52.338006 vcf_generator-1.0.1/vcf_generator/__main__.py
--rw-r--r--   0        0        0      619 2024-04-02 06:27:52.338006 vcf_generator-1.0.1/vcf_generator/address.py
--rw-r--r--   0        0        0     1694 2024-04-02 06:27:52.338006 vcf_generator-1.0.1/vcf_generator/contact.py
--rw-r--r--   0        0        0      258 2024-04-02 06:27:52.338006 vcf_generator-1.0.1/vcf_generator/email.py
--rw-r--r--   0        0        0     3515 2024-04-02 06:27:52.338006 vcf_generator-1.0.1/vcf_generator/gen_contacts.py
--rw-r--r--   0        0        0     2655 2024-04-02 06:27:52.338006 vcf_generator-1.0.1/vcf_generator/gen_vcards.py
--rw-r--r--   0        0        0      623 2024-04-02 06:27:52.338006 vcf_generator-1.0.1/vcf_generator/phone_number.py
--rw-r--r--   0        0        0     4008 1970-01-01 00:00:00.000000 vcf_generator-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1062 2024-04-07 15:31:43.843531 vcf_generator-1.1.0/LICENSE
+-rw-r--r--   0        0        0     3067 2024-04-07 15:31:43.843531 vcf_generator-1.1.0/README.md
+-rw-r--r--   0        0        0      906 2024-04-07 15:31:43.847531 vcf_generator-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-07 15:31:43.847531 vcf_generator-1.1.0/tests/__init__.py
+-rw-r--r--   0        0        0      896 2024-04-07 15:31:43.847531 vcf_generator-1.1.0/tests/addres_test.py
+-rw-r--r--   0        0        0     3196 2024-04-07 15:31:43.847531 vcf_generator-1.1.0/tests/contact_test.py
+-rw-r--r--   0        0        0      175 2024-04-07 15:31:43.847531 vcf_generator-1.1.0/tests/email_test.py
+-rw-r--r--   0        0        0     4872 2024-04-07 15:31:43.847531 vcf_generator-1.1.0/tests/gen_contacts_test.py
+-rw-r--r--   0        0        0     3844 2024-04-07 15:31:43.847531 vcf_generator-1.1.0/tests/gen_vcards_test.py
+-rw-r--r--   0        0        0      323 2024-04-07 15:31:43.847531 vcf_generator-1.1.0/tests/phone_number_test.py
+-rw-r--r--   0        0        0       90 2024-04-07 15:31:43.847531 vcf_generator-1.1.0/vcf_generator/__init__.py
+-rw-r--r--   0        0        0     1526 2024-04-07 15:31:43.847531 vcf_generator-1.1.0/vcf_generator/__main__.py
+-rw-r--r--   0        0        0      619 2024-04-07 15:31:43.847531 vcf_generator-1.1.0/vcf_generator/address.py
+-rw-r--r--   0        0        0     1694 2024-04-07 15:31:43.847531 vcf_generator-1.1.0/vcf_generator/contact.py
+-rw-r--r--   0        0        0      258 2024-04-07 15:31:43.847531 vcf_generator-1.1.0/vcf_generator/email.py
+-rw-r--r--   0        0        0     3515 2024-04-07 15:31:43.847531 vcf_generator-1.1.0/vcf_generator/gen_contacts.py
+-rw-r--r--   0        0        0     2655 2024-04-07 15:31:43.847531 vcf_generator-1.1.0/vcf_generator/gen_vcards.py
+-rw-r--r--   0        0        0      754 2024-04-07 15:31:43.847531 vcf_generator-1.1.0/vcf_generator/phone_number.py
+-rw-r--r--   0        0        0     3918 1970-01-01 00:00:00.000000 vcf_generator-1.1.0/PKG-INFO
```

### Comparing `vcf_generator-1.0.1/LICENSE` & `vcf_generator-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vcf_generator-1.0.1/README.md` & `vcf_generator-1.1.0/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-[![build status](https://github.com/talk2bryan/vcf-generator/actions/workflows/ci.yaml/badge.svg)](https://github.com/talk2bryan/vcf-generator/actions/workflows/ci.yaml)
+[![build status](https://github.com/talk2bryan/vcf-generator/actions/workflows/ci.yml/badge.svg)](https://github.com/talk2bryan/vcf-generator/actions/workflows/ci.yml)
 [![codecov](https://codecov.io/gh/talk2bryan/vcf-generator/graph/badge.svg?token=IHS7IJ3RPN)](https://codecov.io/gh/talk2bryan/vcf-generator)
 [![PyPI version](https://badge.fury.io/py/vcf-generator.svg)](https://badge.fury.io/py/vcf-generator)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/vcf-generator)](https://pypi.org/project/vcf-generator/)
 [![PyPI - License](https://img.shields.io/pypi/l/vcf-generator)](https://pypi.org/project/vcf-generator/)
 [![PyPI - Format](https://img.shields.io/pypi/format/vcf-generator)](https://pypi.org/project/vcf-generator/)
 [![PyPI - Wheel](https://img.shields.io/pypi/wheel/vcf-generator)](https://pypi.org/project/vcf-generator/)
 
@@ -47,46 +47,46 @@
 
 ## Examples
 ### Generate VCF data with 1 contact
 ```bash
 $ vcf-generator vcards
 ```
 
-The above command will generate a VCF file with 1 contact and print the content to the console:
+The above command will generate 1 contact as a VCF string and print the content to the console:
 
 ```bash
 BEGIN:VCARD
 VERSION:4.0
-N:None;Caroline;None;;None
-FN:Caroline
-ORG:None Co.
-TITLE:None
-TEL;TYPE#HOME,voice;VALUE#uri:tel:+72-665-5131092
-TEL;TYPE#HOME,voice;VALUE#uri:tel:+63-689-8521227
-TEL;TYPE#WORK,voice;VALUE#uri:tel:+594-235-6973654
-ADR;TYPE#OTHER;PREF#1;LABEL#922 Williams Grove Apt. 408
-Debbieside, NE 58214
-Trinidad and Tobago:;;922 Williams Grove Apt. 408;Debbieside;NE;58214;Trinidad and Tobago
-ADR;TYPE#WORK;PREF#2;LABEL#987 Middleton Shoals
-Lake Amyview, OK 67042
-Hungary:;;987 Middleton Shoals;Lake Amyview;OK;67042;Hungary
-BDAY:1965-02-22
-EMAIL:rebeccabrady@example.com
-EMAIL:michaeljordan@example.com
-EMAIL:campbellrodney@example.com
+N:None;Laura;Valerie;;Miss
+FN:Laura Valerie
+ORG:Miss Co.
+TITLE:Miss
+TEL;TYPE#HOME,voice;VALUE#uri:tel:+859-422-5863580
+TEL;TYPE#MOBILE,voice;VALUE#uri:tel:+528-463-7642962
+TEL;TYPE#MOBILE,voice;VALUE#uri:tel:+51-666-1415776
+ADR;TYPE#WORK;PREF#1;LABEL#13962 Casey Spring Suite 931
+Xavierfurt, VT 65391
+Suriname:;;13962 Casey Spring Suite 931;Xavierfurt;VT;65391;Suriname
+ADR;TYPE#OTHER;PREF#2;LABEL#33446 Deanna Prairie Apt. 140
+Mcguireport, NJ 64518
+Tokelau:;;33446 Deanna Prairie Apt. 140;Mcguireport;NJ;64518;Tokelau
+BDAY:1959-08-06
+EMAIL:caleb93@example.org
+EMAIL:christopherblankenship@example.org
+EMAIL:michaelwhite@example.org
 END:VCARD
 ```
 
 ### Generate 1 contact as string
 ```bash
 $ vcf-generator contacts_str
 ```
 
-The above command will generate a contact as string and print the content to the console:
+The above command will generate 1 contact information and print the content to the console:
 
 ```bash
-Name: Latoya (Jenna) - Mrs.
-DOB: 1953-04-23
-Phone Numbers: MOBILE: +111 (747) 3381349, OTHER: +220 (470) 7413364
-Emails: PERSONAL: jameswillis@example.org, OTHER: haasbrenda@example.com
-Addresses: OTHER: 86137 Julie Neck Apt. 623, 745 East Eugenefort, MD 06582 Marshall Islands, WORK: 751 Michael Crossroad, 7971 New Andreaton, NM 31536 Israel
+Name: Charles Rebekah - Ind.
+DOB: 1953-11-18
+Phone Numbers: HOME: +738 (250) 705-2590. OTHER: +432 (509) 404-8152. MOBILE: +601 (647) 746-1060
+Emails: OTHER: daniel03@example.org
+Addresses: OTHER: 557 Ruiz Avenue, 7934 Westmouth, KY 56508 Guyana
 ```
```

### Comparing `vcf_generator-1.0.1/pyproject.toml` & `vcf_generator-1.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "vcf-generator"
-version = "1.0.1"
+version = "1.1.0"
 description = "A simple VCF generator. Generate VCF files with random data."
 authors = ["Bryan Wodi <pypi.envy443@dralias.com>"]
 readme = "README.md"
 license = "MIT"
 repository = "https://github.com/talk2bryan/vcf-generator"
 keywords = ["vcf", "generator", "vcard", "contacts", "faker", "python"]
 include = [
@@ -24,13 +24,13 @@
 faker = "^24.4.0"
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "^3.7.0"
 pytest = "^8.1.1"
 pytest-cov = "^5.0.0"
 
-[tool.pytest]
+[tool.pytest.ini_options]
 filterwarnings = ["ignore::DeprecationWarning"]
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `vcf_generator-1.0.1/tests/addres_test.py` & `vcf_generator-1.1.0/tests/addres_test.py`

 * *Files identical despite different names*

### Comparing `vcf_generator-1.0.1/tests/contact_test.py` & `vcf_generator-1.1.0/tests/contact_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,15 +95,15 @@
 
 
 def test_contact_full_name_w_middlename(contact_full_name):
     assert contact_full_name.full_name == "John Nicholas Doe"
 
 
 def test_contact_phone_number(contact):
-    assert str(contact.phone_numbers[0]) == "HOME: +1 (123) 4567890"
+    assert str(contact.phone_numbers[0]) == "HOME: +1 (123) 456-7890"
 
 
 def test_contact_email(contact):
     assert contact.emails[0].address == "test@example.com"
 
 
 def test_contact_address(contact):
@@ -112,12 +112,12 @@
     )
 
 
 def test_contact_str(contact_full_name):
     expected_output = (
         "Name: John Nicholas Doe (JD) - Mr.\n"
         + "DOB: 1990-01-01\n"
-        + "Phone Numbers: HOME: +1 (123) 4567890, WORK: +1 (198) 7654321\n"
+        + "Phone Numbers: HOME: +1 (123) 456-7890. WORK: +1 (198) 765-4321\n"
         + "Emails: HOME: email@address.com\n"
-        + "Addresses: HOME: 123 Main St, Anytown, Anystate 12345 USA, WORK: 456 Oak St, Othertown, Otherstate 54321 USA\n"
+        + "Addresses: HOME: 123 Main St, Anytown, Anystate 12345 USA. WORK: 456 Oak St, Othertown, Otherstate 54321 USA\n"
     )
     assert str(contact_full_name) == expected_output
```

### Comparing `vcf_generator-1.0.1/tests/gen_contacts_test.py` & `vcf_generator-1.1.0/tests/gen_contacts_test.py`

 * *Files identical despite different names*

### Comparing `vcf_generator-1.0.1/tests/gen_vcards_test.py` & `vcf_generator-1.1.0/tests/gen_vcards_test.py`

 * *Files identical despite different names*

### Comparing `vcf_generator-1.0.1/vcf_generator/__main__.py` & `vcf_generator-1.1.0/vcf_generator/__main__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,8 @@
-"""CLI module for vcf_generator package.
-
-The user can either call the gen_contacts module or the gen_vcards module as follows:
-
-$ python -m vcf_generator contacts_str [--num_contacts NUM_CONTACTS] [--output_file OUTPUT_FILE]
-$ python -m vcf_generator vcards [--num_contacts NUM_CONTACTS] [--output_file OUTPUT_FILE]
-"""
+"""CLI module for vcf_generator package."""
 
 import fire
 
 from vcf_generator import MIN_NUM_CONTACTS
 from vcf_generator.gen_contacts import main as gen_contacts
 from vcf_generator.gen_vcards import main as gen_vcards
 
@@ -42,12 +36,14 @@
             num_contacts (int, optional): Number of contacts to generate. Defaults to MIN_NUM_CONTACTS.
             output_file (str | None, optional): Output file path. Defaults to None.
         """
         gen_vcards(num_contacts=num_contacts, output_file=output_file)
 
 
 def main():
+    """CLI module for vcf_generator package."""
+    # Fire up the CLI module.
     fire.Fire(Contacts)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `vcf_generator-1.0.1/vcf_generator/address.py` & `vcf_generator-1.1.0/vcf_generator/address.py`

 * *Files identical despite different names*

### Comparing `vcf_generator-1.0.1/vcf_generator/contact.py` & `vcf_generator-1.1.0/vcf_generator/contact.py`

 * *Files 14% similar despite different names*

```diff
@@ -33,25 +33,25 @@
             f"Name: {self.full_name}"
             + (f" ({self.nickname})" if self.nickname else "")
             + (f" - {self.title}" if self.title else "")
             + "\n"
             + (f"DOB: {self.birth_date}" if self.birth_date else "")
             + "\n"
             + (
-                f"Phone Numbers: {', '.join([str(p) for p in self.phone_numbers])}"
+                f"Phone Numbers: {'. '.join([str(p) for p in self.phone_numbers])}"
                 if self.phone_numbers
                 else ""
             )
             + "\n"
             + (
-                f"Emails: {', '.join([str(e) for e in self.emails])}"
+                f"Emails: {'. '.join([str(e) for e in self.emails])}"
                 if self.emails
                 else ""
             )
             + "\n"
             + (
-                f"Addresses: {', '.join([str(a) for a in self.addresses])}"
+                f"Addresses: {'. '.join([str(a) for a in self.addresses])}"
                 if self.addresses
                 else ""
             )
             + "\n"
         )
```

### Comparing `vcf_generator-1.0.1/vcf_generator/gen_contacts.py` & `vcf_generator-1.1.0/vcf_generator/gen_contacts.py`

 * *Files identical despite different names*

### Comparing `vcf_generator-1.0.1/vcf_generator/gen_vcards.py` & `vcf_generator-1.1.0/vcf_generator/gen_vcards.py`

 * *Files identical despite different names*

### Comparing `vcf_generator-1.0.1/PKG-INFO` & `vcf_generator-1.1.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vcf-generator
-Version: 1.0.1
+Version: 1.1.0
 Summary: A simple VCF generator. Generate VCF files with random data.
 Home-page: https://github.com/talk2bryan/vcf-generator
 License: MIT
 Keywords: vcf,generator,vcard,contacts,faker,python
 Author: Bryan Wodi
 Author-email: pypi.envy443@dralias.com
 Requires-Python: >=3.10,<4.0
@@ -15,15 +15,15 @@
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: faker (>=24.4.0,<25.0.0)
 Requires-Dist: fire (>=0.6.0,<0.7.0)
 Project-URL: Bug Tracker, https://github.com/talk2bryan/vcf-generator/issues
 Project-URL: Repository, https://github.com/talk2bryan/vcf-generator
 Description-Content-Type: text/markdown
 
-[![build status](https://github.com/talk2bryan/vcf-generator/actions/workflows/ci.yaml/badge.svg)](https://github.com/talk2bryan/vcf-generator/actions/workflows/ci.yaml)
+[![build status](https://github.com/talk2bryan/vcf-generator/actions/workflows/ci.yml/badge.svg)](https://github.com/talk2bryan/vcf-generator/actions/workflows/ci.yml)
 [![codecov](https://codecov.io/gh/talk2bryan/vcf-generator/graph/badge.svg?token=IHS7IJ3RPN)](https://codecov.io/gh/talk2bryan/vcf-generator)
 [![PyPI version](https://badge.fury.io/py/vcf-generator.svg)](https://badge.fury.io/py/vcf-generator)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/vcf-generator)](https://pypi.org/project/vcf-generator/)
 [![PyPI - License](https://img.shields.io/pypi/l/vcf-generator)](https://pypi.org/project/vcf-generator/)
 [![PyPI - Format](https://img.shields.io/pypi/format/vcf-generator)](https://pypi.org/project/vcf-generator/)
 [![PyPI - Wheel](https://img.shields.io/pypi/wheel/vcf-generator)](https://pypi.org/project/vcf-generator/)
 
@@ -68,47 +68,47 @@
 
 ## Examples
 ### Generate VCF data with 1 contact
 ```bash
 $ vcf-generator vcards
 ```
 
-The above command will generate a VCF file with 1 contact and print the content to the console:
+The above command will generate 1 contact as a VCF string and print the content to the console:
 
 ```bash
 BEGIN:VCARD
 VERSION:4.0
-N:None;Caroline;None;;None
-FN:Caroline
-ORG:None Co.
-TITLE:None
-TEL;TYPE#HOME,voice;VALUE#uri:tel:+72-665-5131092
-TEL;TYPE#HOME,voice;VALUE#uri:tel:+63-689-8521227
-TEL;TYPE#WORK,voice;VALUE#uri:tel:+594-235-6973654
-ADR;TYPE#OTHER;PREF#1;LABEL#922 Williams Grove Apt. 408
-Debbieside, NE 58214
-Trinidad and Tobago:;;922 Williams Grove Apt. 408;Debbieside;NE;58214;Trinidad and Tobago
-ADR;TYPE#WORK;PREF#2;LABEL#987 Middleton Shoals
-Lake Amyview, OK 67042
-Hungary:;;987 Middleton Shoals;Lake Amyview;OK;67042;Hungary
-BDAY:1965-02-22
-EMAIL:rebeccabrady@example.com
-EMAIL:michaeljordan@example.com
-EMAIL:campbellrodney@example.com
+N:None;Laura;Valerie;;Miss
+FN:Laura Valerie
+ORG:Miss Co.
+TITLE:Miss
+TEL;TYPE#HOME,voice;VALUE#uri:tel:+859-422-5863580
+TEL;TYPE#MOBILE,voice;VALUE#uri:tel:+528-463-7642962
+TEL;TYPE#MOBILE,voice;VALUE#uri:tel:+51-666-1415776
+ADR;TYPE#WORK;PREF#1;LABEL#13962 Casey Spring Suite 931
+Xavierfurt, VT 65391
+Suriname:;;13962 Casey Spring Suite 931;Xavierfurt;VT;65391;Suriname
+ADR;TYPE#OTHER;PREF#2;LABEL#33446 Deanna Prairie Apt. 140
+Mcguireport, NJ 64518
+Tokelau:;;33446 Deanna Prairie Apt. 140;Mcguireport;NJ;64518;Tokelau
+BDAY:1959-08-06
+EMAIL:caleb93@example.org
+EMAIL:christopherblankenship@example.org
+EMAIL:michaelwhite@example.org
 END:VCARD
 ```
 
 ### Generate 1 contact as string
 ```bash
 $ vcf-generator contacts_str
 ```
 
-The above command will generate a contact as string and print the content to the console:
+The above command will generate 1 contact information and print the content to the console:
 
 ```bash
-Name: Latoya (Jenna) - Mrs.
-DOB: 1953-04-23
-Phone Numbers: MOBILE: +111 (747) 3381349, OTHER: +220 (470) 7413364
-Emails: PERSONAL: jameswillis@example.org, OTHER: haasbrenda@example.com
-Addresses: OTHER: 86137 Julie Neck Apt. 623, 745 East Eugenefort, MD 06582 Marshall Islands, WORK: 751 Michael Crossroad, 7971 New Andreaton, NM 31536 Israel
+Name: Charles Rebekah - Ind.
+DOB: 1953-11-18
+Phone Numbers: HOME: +738 (250) 705-2590. OTHER: +432 (509) 404-8152. MOBILE: +601 (647) 746-1060
+Emails: OTHER: daniel03@example.org
+Addresses: OTHER: 557 Ruiz Avenue, 7934 Westmouth, KY 56508 Guyana
 ```
```

