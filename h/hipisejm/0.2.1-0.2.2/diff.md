# Comparing `tmp/hipisejm-0.2.1.tar.gz` & `tmp/hipisejm-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hipisejm-0.2.1.tar", last modified: Wed Mar  6 18:13:56 2024, max compression
+gzip compressed data, was "hipisejm-0.2.2.tar", last modified: Sun Apr  7 12:09:36 2024, max compression
```

## Comparing `hipisejm-0.2.1.tar` & `hipisejm-0.2.2.tar`

### file list

```diff
@@ -1,24 +1,21 @@
-drwxrwxr-x   0 walasiek  (1000) walasiek  (1000)        0 2024-03-06 18:13:56.351549 hipisejm-0.2.1/
--rw-rw-r--   0 walasiek  (1000) walasiek  (1000)     2742 2024-03-06 18:13:56.355549 hipisejm-0.2.1/PKG-INFO
--rw-rw-r--   0 walasiek  (1000) walasiek  (1000)     1919 2024-03-06 17:19:28.466075 hipisejm-0.2.1/README.md
-drwxrwxr-x   0 walasiek  (1000) walasiek  (1000)        0 2024-03-06 18:13:56.351549 hipisejm-0.2.1/bin/
--rwxrwxr-x   0 walasiek  (1000) walasiek  (1000)     1687 2024-03-02 14:14:10.686690 hipisejm-0.2.1/bin/parser-parse-pdf.py
--rw-rw-r--   0 walasiek  (1000) walasiek  (1000)     1626 2024-03-03 23:06:40.665682 hipisejm-0.2.1/dobre_przyklady_do_testow.txt
-drwxrwxr-x   0 walasiek  (1000) walasiek  (1000)        0 2024-03-06 18:13:56.351549 hipisejm-0.2.1/hipisejm/
--rw-rw-r--   0 walasiek  (1000) walasiek  (1000)       44 2024-03-06 18:07:34.184124 hipisejm-0.2.1/hipisejm/__init__.py
-drwxrwxr-x   0 walasiek  (1000) walasiek  (1000)        0 2024-03-06 18:13:56.351549 hipisejm-0.2.1/hipisejm/stenparser/
--rw-rw-r--   0 walasiek  (1000) walasiek  (1000)        0 2024-01-07 21:59:32.848211 hipisejm-0.2.1/hipisejm/stenparser/__init__.py
--rw-rw-r--   0 walasiek  (1000) walasiek  (1000)     4964 2024-03-04 00:10:58.221013 hipisejm-0.2.1/hipisejm/stenparser/raw_speech_parser.py
--rw-rw-r--   0 walasiek  (1000) walasiek  (1000)     2270 2024-03-04 23:46:54.134129 hipisejm-0.2.1/hipisejm/stenparser/sejm_parser.py
--rw-rw-r--   0 walasiek  (1000) walasiek  (1000)    14635 2024-03-06 18:07:08.272446 hipisejm-0.2.1/hipisejm/stenparser/session_file_parser.py
--rw-rw-r--   0 walasiek  (1000) walasiek  (1000)     7322 2024-03-04 23:49:53.156383 hipisejm-0.2.1/hipisejm/stenparser/transcript.py
-drwxrwxr-x   0 walasiek  (1000) walasiek  (1000)        0 2024-03-06 18:13:56.351549 hipisejm-0.2.1/hipisejm/utils/
--rw-rw-r--   0 walasiek  (1000) walasiek  (1000)        0 2024-02-17 11:30:03.021932 hipisejm-0.2.1/hipisejm/utils/__init__.py
--rw-rw-r--   0 walasiek  (1000) walasiek  (1000)     5631 2024-03-03 00:38:02.542925 hipisejm-0.2.1/hipisejm/utils/pdfminer_wrapper.py
--rw-rw-r--   0 walasiek  (1000) walasiek  (1000)     5080 2024-03-04 00:04:36.756566 hipisejm-0.2.1/hipisejm/utils/pdfminer_wrapper_helper.py
--rw-rw-r--   0 walasiek  (1000) walasiek  (1000)     1509 2024-03-04 22:27:01.201143 hipisejm-0.2.1/hipisejm/utils/polish_dates.py
--rw-rw-r--   0 walasiek  (1000) walasiek  (1000)      466 2024-03-04 21:55:33.045961 hipisejm-0.2.1/hipisejm/utils/roman_numbers.py
--rw-rw-r--   0 walasiek  (1000) walasiek  (1000)      119 2024-02-18 00:19:53.771024 hipisejm-0.2.1/requirements.txt
--rw-rw-r--   0 walasiek  (1000) walasiek  (1000)      603 2024-03-06 17:00:45.745160 hipisejm-0.2.1/setup.py
--rw-rw-r--   0 walasiek  (1000) walasiek  (1000)     9386 2024-03-03 00:38:04.574899 hipisejm-0.2.1/test-komisja-raw.txt
--rw-rw-r--   0 walasiek  (1000) walasiek  (1000)   244929 2024-03-03 00:49:37.947647 hipisejm-0.2.1/test-komisja2-raw.txt
+drwxrwxr-x   0 walasiek  (1000) walasiek  (1000)        0 2024-04-07 12:09:36.676554 hipisejm-0.2.2/
+-rw-rw-r--   0 walasiek  (1000) walasiek  (1000)     2742 2024-04-07 12:09:36.676554 hipisejm-0.2.2/PKG-INFO
+-rw-rw-r--   0 walasiek  (1000) walasiek  (1000)     1919 2024-03-06 17:19:28.466075 hipisejm-0.2.2/README.md
+drwxrwxr-x   0 walasiek  (1000) walasiek  (1000)        0 2024-04-07 12:09:36.676554 hipisejm-0.2.2/bin/
+-rwxrwxr-x   0 walasiek  (1000) walasiek  (1000)     1687 2024-03-02 14:14:10.686690 hipisejm-0.2.2/bin/parser-parse-pdf.py
+drwxrwxr-x   0 walasiek  (1000) walasiek  (1000)        0 2024-04-07 12:09:36.676554 hipisejm-0.2.2/hipisejm/
+-rw-rw-r--   0 walasiek  (1000) walasiek  (1000)       44 2024-04-07 12:03:20.842406 hipisejm-0.2.2/hipisejm/__init__.py
+drwxrwxr-x   0 walasiek  (1000) walasiek  (1000)        0 2024-04-07 12:09:36.676554 hipisejm-0.2.2/hipisejm/stenparser/
+-rw-rw-r--   0 walasiek  (1000) walasiek  (1000)        0 2024-01-07 21:59:32.848211 hipisejm-0.2.2/hipisejm/stenparser/__init__.py
+-rw-rw-r--   0 walasiek  (1000) walasiek  (1000)     5184 2024-04-07 11:52:59.100165 hipisejm-0.2.2/hipisejm/stenparser/raw_speech_parser.py
+-rw-rw-r--   0 walasiek  (1000) walasiek  (1000)     2270 2024-03-04 23:46:54.134129 hipisejm-0.2.2/hipisejm/stenparser/sejm_parser.py
+-rw-rw-r--   0 walasiek  (1000) walasiek  (1000)    14736 2024-04-07 11:14:35.066007 hipisejm-0.2.2/hipisejm/stenparser/session_file_parser.py
+-rw-rw-r--   0 walasiek  (1000) walasiek  (1000)     6753 2024-04-07 11:43:03.203286 hipisejm-0.2.2/hipisejm/stenparser/transcript.py
+drwxrwxr-x   0 walasiek  (1000) walasiek  (1000)        0 2024-04-07 12:09:36.676554 hipisejm-0.2.2/hipisejm/utils/
+-rw-rw-r--   0 walasiek  (1000) walasiek  (1000)        0 2024-02-17 11:30:03.021932 hipisejm-0.2.2/hipisejm/utils/__init__.py
+-rw-rw-r--   0 walasiek  (1000) walasiek  (1000)     5631 2024-03-03 00:38:02.542925 hipisejm-0.2.2/hipisejm/utils/pdfminer_wrapper.py
+-rw-rw-r--   0 walasiek  (1000) walasiek  (1000)     5175 2024-04-07 11:14:10.798434 hipisejm-0.2.2/hipisejm/utils/pdfminer_wrapper_helper.py
+-rw-rw-r--   0 walasiek  (1000) walasiek  (1000)     1509 2024-03-04 22:27:01.201143 hipisejm-0.2.2/hipisejm/utils/polish_dates.py
+-rw-rw-r--   0 walasiek  (1000) walasiek  (1000)      466 2024-03-04 21:55:33.045961 hipisejm-0.2.2/hipisejm/utils/roman_numbers.py
+-rw-rw-r--   0 walasiek  (1000) walasiek  (1000)      119 2024-02-18 00:19:53.771024 hipisejm-0.2.2/requirements.txt
+-rw-rw-r--   0 walasiek  (1000) walasiek  (1000)      603 2024-03-06 17:00:45.745160 hipisejm-0.2.2/setup.py
```

### Comparing `hipisejm-0.2.1/PKG-INFO` & `hipisejm-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: hipisejm
-Version: 0.2.1
+Version: 0.2.2
 Summary: Parse Polish Sejm transcripts to machine readable corpus
 Home-page: https://pypi.org/project/hipisejm/
 Author: Marcin Walas
 Author-email: kontakt@marcinwalas.pl
 License: LICENSE
 Description: # hipisejm
         # Author: Marcin Walas <kontakt@marcinwalas.pl>
```

### Comparing `hipisejm-0.2.1/README.md` & `hipisejm-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `hipisejm-0.2.1/bin/parser-parse-pdf.py` & `hipisejm-0.2.2/bin/parser-parse-pdf.py`

 * *Files identical despite different names*

### Comparing `hipisejm-0.2.1/hipisejm/stenparser/raw_speech_parser.py` & `hipisejm-0.2.2/hipisejm/stenparser/raw_speech_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import logging
 import re
 from hipisejm.stenparser.transcript import SessionSpeech, SpeechInterruption, SpeechReaction
+from hipisejm.utils.pdfminer_wrapper_helper import remove_all_tags
 
 
 class RawSpeechParser:
     """
     Helper class to parse raw text speech
     """
     def __init__(self):
@@ -79,15 +80,15 @@
         match = re.match(r"^[(]<i>(?P<speaker>.*?)(?:</i>\s*:\s*|:\s*</i>|(?:</i>\s*(?P<broken_font>[A-Za-zĄŻŚŹĘĆÓŁŃ][a-zążśźęćółń]+)\s*:))(?P<text>.*)[)]$", part)
         if match:
             speaker = match.group('speaker')
             broken_font = match.group('broken_font')
             if broken_font:
                 speaker = speaker + ' ' + broken_font
 
-            interrupted_by = self._fix_spaces(speaker)
+            interrupted_by = self._fix_interruption_by(speaker)
 
             interruption_text = self._fix_spaces(match.group('text'))
 
             # other italic tags should not occur in interruption
             # if there is italic tag, then maybe something is wrong with the parse
             if '<i>' in interruption_text:
                 return None
@@ -121,12 +122,17 @@
                 reaction_txt = f"{reaction_txt} {additional_non_italic}"
 
             reaction_txt = self._fix_spaces(reaction_txt)
             return SpeechReaction(reaction_txt)
 
         return None
 
+    def _fix_interruption_by(self, txt: str) -> str:
+        txt = remove_all_tags(txt)
+        txt = self._fix_spaces(txt)
+        return txt
+
     def _fix_spaces(self, txt):
         txt = re.sub(r"^\s+", "", txt)
         txt = re.sub(r"\s+$", "", txt)
         txt = re.sub(r"\s+", " ", txt)
         return txt
```

### Comparing `hipisejm-0.2.1/hipisejm/stenparser/sejm_parser.py` & `hipisejm-0.2.2/hipisejm/stenparser/sejm_parser.py`

 * *Files identical despite different names*

### Comparing `hipisejm-0.2.1/hipisejm/stenparser/session_file_parser.py` & `hipisejm-0.2.2/hipisejm/stenparser/session_file_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import math
 import re
 from hipisejm.stenparser.transcript import SessionTranscript
 from hipisejm.stenparser.raw_speech_parser import RawSpeechParser
 from hipisejm.utils.pdfminer_wrapper import PDFText, PDFLineBreak, PDFTextBoxBreak, PDFPageBreak
-from hipisejm.utils.pdfminer_wrapper_helper import get_first_text_box_from_index, get_first_page_from_index, extract_text_from_parsed_list
+from hipisejm.utils.pdfminer_wrapper_helper import get_first_text_box_from_index, get_first_page_from_index, extract_text_from_parsed_list, remove_all_tags
 from hipisejm.utils.roman_numbers import roman_to_arabic
 from hipisejm.utils.polish_dates import convert_polish_date_to_iso, find_polish_dates_in_text
 
 
 class SejmParseError(Exception):
     """Raised when parse is not possible"""
     def __init__(self, message="Sejm Parsing error"):
@@ -326,14 +326,17 @@
         raw_name = re.sub(r"[:]+", "", raw_name)
         raw_name = re.sub(r"\s+", " ", raw_name)
 
         if raw_name == 'Marszałek':
             sejm_speaker_names = self.parse_cache['transcript'].session_officials.get_by_role('speaker')
             if len(sejm_speaker_names) > 0:
                 raw_name = 'Marszałek ' + sejm_speaker_names[0][1]
+
+        # remove tags if any are left
+        raw_name = remove_all_tags(raw_name)
         return raw_name
 
     def _start_new_speech(self):
         self.parse_cache['new_speaker_entries'] = []
         self.parse_cache['current_speech_entries'] = []
 
     def _add_entry_to_current_speech(self, entry):
```

### Comparing `hipisejm-0.2.1/hipisejm/stenparser/transcript.py` & `hipisejm-0.2.2/hipisejm/stenparser/transcript.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from collections import defaultdict
 import xml.etree.ElementTree as ET
+from xml.dom import minidom
 
 
 class SessionOfficials:
     """
     This class represents officials of the sessions like Marszałek, Marszałek senior and Wicemarszałek
     """
     def __init__(self):
@@ -17,21 +18,17 @@
 
     def __str__(self):
         chunks = ["Session officials:"]
         for entry in self.officials_list:
             chunks.append(f"  {entry[0]}: {entry[1]}")
         return "\n".join(chunks)
 
-    def to_xml(self) -> str:
-        chunks = []
+    def to_xml(self, parent_tag):
         for official in self.officials_list:
-            chunk = '<official title="' + official[0] + '" name="' + official[1] + '"/>'
-            chunks.append(chunk)
-
-        return "\n".join(chunks)
+            ET.SubElement(parent_tag, "official", title=official[0], name=official[1])
 
     def get_by_role(self, role_name: str):
         """
         Returns list of entries for persons with given role on the session.
         If there is no such role during the session then returns empty list.
         """
         return self.role_to_officials.get(role_name, [])
@@ -41,29 +38,29 @@
     """
     Reactions are spontanous interruptions of the speech without particular speaker
     Can be something like appluase, noise, laugh, etc...
     """
     def __init__(self, reaction_text: str):
         self.reaction_text = reaction_text
 
-    def to_xml(self) -> str:
-        return '<utt t="reaction">' + self.reaction_text + '</utt>'
+    def to_xml(self, parent_tag):
+        ET.SubElement(parent_tag, "utt", t="reaction").text = self.reaction_text
 
 
 class SpeechInterruption:
     """
     Interruptions are from the audience and particular speaker
     Sometimes the speaker is unknown ("Głos z sali") or refers to multiple persons speaking
     """
     def __init__(self, interrupted_by_speaker: str, text: str):
         self.interrupted_by_speaker = interrupted_by_speaker
         self.text = text
 
-    def to_xml(self) -> str:
-        return '<utt t="interrupt" by="' + self.interrupted_by_speaker + '">' + f"{self.text}</utt>"
+    def to_xml(self, parent_tag):
+        ET.SubElement(parent_tag, "utt", t="interrupt", by=self.interrupted_by_speaker).text = self.text
 
 
 class SessionSpeech:
     """
     Speech is the one uninterrupted sequence of utterance of the given person.
     Speech consists of:
     - utterances of the speaker
@@ -91,26 +88,22 @@
 
     def add_interruption(self, interruption: SpeechInterruption):
         self.content.append(interruption)
 
     def add_reaction(self, reaction: SpeechReaction):
         self.content.append(reaction)
 
-    def to_xml(self) -> str:
-        result = []
+    def to_xml(self, parent_tag):
 
-        result.append('<speech speaker="' + self.speaker + '">')
+        speech_tag = ET.SubElement(parent_tag, "speech", speaker=self.speaker)
         for entry in self.content:
             if isinstance(entry, str):
-                result.append('<utt t="norm">' + entry + '</utt>')
+                ET.SubElement(speech_tag, "utt", t="norm").text = entry
             else:
-                result.append(entry.to_xml())
-        result.append("</speech>")
-
-        return "\n".join(result)
+                entry.to_xml(speech_tag)
 
 
 class SessionTranscript:
     """
     Session Transcript stores all speeches from the given session.
     """
     def __init__(self):
@@ -118,38 +111,36 @@
         self.session_content = []
         self.session_no = None
         self.term_no = None
         self.session_date = None
         self.source_filename = None
 
     def dump_to_xml(self, filepath: str= None):
-        with open(filepath, "w") as f:
-            f.write('<?xml version="1.0" encoding="UTF-8"?>\n')
-            f.write("""<session xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
-                    xsi:noNamespaceSchemaLocation="hipisejm-transcript-schema.xsd" """)
-            if self.source_filename is not None:
-                f.write('source="' + self.source_filename + '"')
-            f.write(">\n")
-
-            f.write("<meta>\n")
-            f.write(f"<session_no>{self.session_no}</session_no>\n")
-            f.write(f"<term_no>{self.term_no}</term_no>\n")
-            f.write(f"<session_date>{self.session_date}</session_date>\n")
-            f.write("</meta>\n")
+        session_tag = ET.Element("session", source=self.source_filename)
 
-            f.write('<session_officials>\n')
-            f.write(self.session_officials.to_xml())
-            f.write("\n")
-            f.write('</session_officials>\n')
+        meta_tag = ET.SubElement(session_tag, "meta")
+
+        ET.SubElement(meta_tag, "session_no").text = str(self.session_no)
+        ET.SubElement(meta_tag, "term_no").text = str(self.term_no)
+        ET.SubElement(meta_tag, "session_date").text = self.session_date
 
-            f.write('<content>\n')
-            self._dump_session_content_to_xml(f)
-            f.write('</content>\n')
+        session_officials_tag = ET.SubElement(session_tag, "session_officials")
+        self.session_officials.to_xml(session_officials_tag)
+
+        content_tag = ET.SubElement(session_tag, "content")
+        for speech in self.session_content:
+            speech.to_xml(content_tag)
 
-            f.write('</session>\n')
+        tree_str = ET.tostring(session_tag, 'utf-8')
+        pretty_xml = minidom.parseString(tree_str).toprettyxml(indent="  ")
+
+        with open(filepath, "w") as f:
+            f.write(pretty_xml)
+            f.write("\n")
+        return
 
     def load_from_xml(self, filepath: str):
         xml_tree = ET.parse(filepath)
 
         session_tag = xml_tree.getroot()
 
         self.source_filename = session_tag.get("source")
@@ -165,24 +156,14 @@
         chunks = []
         chunks.append(str(self.session_officials))
         return "\n".join(chunks)
 
     def add_speech(self, speech: SessionSpeech):
         self.session_content.append(speech)
 
-    def _dump_officials_to_xml(self, f):
-        for session_official in self.session_officials:
-            f.write(session_official.to_xml())
-            f.write("\n")
-
-    def _dump_session_content_to_xml(self, f):
-        for speech in self.session_content:
-            f.write(speech.to_xml())
-            f.write("\n")
-
     def _load_xml_meta_tag(self, meta_tag):
         session_no_tag = meta_tag.find("session_no")
         if session_no_tag is not None:
             self.session_no = int(session_no_tag.text)
         session_date_tag = meta_tag.find("session_date")
         if session_date_tag is not None:
             self.session_date = session_date_tag.text
```

### Comparing `hipisejm-0.2.1/hipisejm/utils/pdfminer_wrapper.py` & `hipisejm-0.2.2/hipisejm/utils/pdfminer_wrapper.py`

 * *Files identical despite different names*

### Comparing `hipisejm-0.2.1/hipisejm/utils/pdfminer_wrapper_helper.py` & `hipisejm-0.2.2/hipisejm/utils/pdfminer_wrapper_helper.py`

 * *Files 3% similar despite different names*

```diff
@@ -112,7 +112,12 @@
         result = re.sub("</b></i><i><b>", "", result)
         result = re.sub("</i><i>", "", result)
         result = re.sub("</b><b>", "", result)
 
     # fix spaces
     result = re.sub(r"[ ][\n]", "\n", result)
     return result
+
+
+def remove_all_tags(text: str) -> str:
+    text = re.sub(r"<.*?>", "", text)
+    return text
```

### Comparing `hipisejm-0.2.1/hipisejm/utils/polish_dates.py` & `hipisejm-0.2.2/hipisejm/utils/polish_dates.py`

 * *Files identical despite different names*

### Comparing `hipisejm-0.2.1/setup.py` & `hipisejm-0.2.2/setup.py`

 * *Files identical despite different names*

