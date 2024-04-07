# Comparing `tmp/hich_restrict-0.1.0-py3-none-any.whl.zip` & `tmp/hich_restrict-0.1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,12 @@
-Zip file size: 6101 bytes, number of entries: 9
+Zip file size: 6838 bytes, number of entries: 10
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 hich_restrict/__init__.py
--rw-r--r--  2.0 unx     3571 b- defN 80-Jan-01 00:00 hich_restrict/__main__.py
+-rw-r--r--  2.0 unx     1300 b- defN 80-Jan-01 00:00 hich_restrict/__main__.py
 -rw-r--r--  2.0 unx     4202 b- defN 80-Jan-01 00:00 hich_restrict/contacts.py
 -rw-r--r--  2.0 unx     4343 b- defN 80-Jan-01 00:00 hich_restrict/fragments.py
+-rw-r--r--  2.0 unx     3455 b- defN 80-Jan-01 00:00 hich_restrict/restrict_manager.py
 -rw-r--r--  2.0 unx     1289 b- defN 80-Jan-01 00:00 hich_restrict/timer.py
--rw-r--r--  2.0 unx      445 b- defN 80-Jan-01 00:00 hich_restrict-0.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 hich_restrict-0.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       60 b- defN 80-Jan-01 00:00 hich_restrict-0.1.0.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx      729 b- defN 16-Jan-01 00:00 hich_restrict-0.1.0.dist-info/RECORD
-9 files, 14727 bytes uncompressed, 4839 bytes compressed:  67.1%
+-rw-r--r--  2.0 unx      445 b- defN 80-Jan-01 00:00 hich_restrict-0.1.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 hich_restrict-0.1.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       60 b- defN 80-Jan-01 00:00 hich_restrict-0.1.1.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx      819 b- defN 16-Jan-01 00:00 hich_restrict-0.1.1.dist-info/RECORD
+10 files, 16001 bytes uncompressed, 5434 bytes compressed:  66.0%
```

## zipnote {}

```diff
@@ -6,23 +6,26 @@
 
 Filename: hich_restrict/contacts.py
 Comment: 
 
 Filename: hich_restrict/fragments.py
 Comment: 
 
+Filename: hich_restrict/restrict_manager.py
+Comment: 
+
 Filename: hich_restrict/timer.py
 Comment: 
 
-Filename: hich_restrict-0.1.0.dist-info/METADATA
+Filename: hich_restrict-0.1.1.dist-info/METADATA
 Comment: 
 
-Filename: hich_restrict-0.1.0.dist-info/WHEEL
+Filename: hich_restrict-0.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: hich_restrict-0.1.0.dist-info/entry_points.txt
+Filename: hich_restrict-0.1.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: hich_restrict-0.1.0.dist-info/RECORD
+Filename: hich_restrict-0.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## hich_restrict/__main__.py

```diff
@@ -1,80 +1,11 @@
 import click
 import time
 import sys
-from .contacts import *
-from .fragments import *
-
-class RestrictManager:
-    
-    def setup(self, cmd, frag_file_format, output_pairs, frag_file, input_pairs):
-        self.output_pairs = output_pairs
-        reader = self.frag_reader(frag_file_format, frag_file)
-        self.frag_finder = FragFinder(reader)
-        self.contacts = PairsContactsReader(
-            input_pairs, 
-            extract_fields=["chrom1", "pos1", "chrom2", "pos2", "#"],
-            add_before_columns = f"#hichheader: @PG ID:hich-restrict CL: {cmd} PN:hich-restrict\n",
-            yield_line_with_item = True)
-
-        self.frag_finder.load()
-    
-    def tag(self):
-        file = None
-        if self.output_pairs:
-            file = open(self.output_pairs, 'w')
-
-        for fields, line in self.contacts:
-            if fields is not None:
-                frag1 = self.frag_finder.find(fields['chrom1'], int(fields['pos1']))
-                frag2 = self.frag_finder.find(fields['chrom2'], int(fields['pos2']))
-                frag_tag = "\t".join([str(s) for s in frag1+frag2])
-                new_line = f"{line.strip()}\t{frag_tag}\n"
-            else:
-                new_line = line
-            if not file:
-                click.echo(new_line.strip())
-            else:
-                file.write(new_line)
-        
-        if file:
-            file.close()
-        if self.output_pairs:
-            autodetect_compress(self.output_pairs)
-            
-
-    def frag_reader(self, frag_file_format, frag_file):
-        readers = self.frag_file_formats[frag_file_format]
-        reader = None
-        for reader_type in readers:
-            try_reader = reader_type(frag_file)
-            try:
-                for r in try_reader:
-                    break
-            except:
-                continue
-            else:
-                reader = try_reader
-                break
-        if reader is None:
-            raise Exception("Failed to autodetect fragment file format.")
-        reader.file.seek(0)
-        return reader
-
-
-
-    @classmethod
-    def frag_file_format_options(cls):
-        return list(cls.frag_file_formats)
-
-    frag_file_formats = {
-        "autodetect":[BedIntervalReader, ChromlinesIntervalReader],
-        "bed":[BedIntervalReader],
-        "chromlines":[ChromlinesIntervalReader]
-    }
+from .restrict_manager import *
 
 @click.command()
 @click.option("--frag-file-format",
     type=click.Choice(RestrictManager.frag_file_format_options()),
     show_default=True,
     default=RestrictManager.frag_file_format_options()[0],
     help="Whether lines of fragments file are in .bed format (chrom start end) "
```

## Comparing `hich_restrict-0.1.0.dist-info/RECORD` & `hich_restrict-0.1.1.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 hich_restrict/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-hich_restrict/__main__.py,sha256=i5YImeMx1AW1nvZuQpLeKqo9wuexQPFUuxVFc84lPPY,3571
+hich_restrict/__main__.py,sha256=E2qjk90I-smYKcc7z4aLFQSTHqS1enDBMjb3OpivV58,1300
 hich_restrict/contacts.py,sha256=088NMTKygzd43V2vPlkfj3_Fzybw04YIBInUoVWd0BM,4202
 hich_restrict/fragments.py,sha256=oY7ceSjTIYauV1gElRvKrnF1LCJqwfNr7VqcfIvmNZ8,4343
+hich_restrict/restrict_manager.py,sha256=uPMb7puIXRzl70zsJ9Rh06_7dRXxYztwFSB_u5zlKIs,3455
 hich_restrict/timer.py,sha256=VhkDub_yc5dQmXwHfKRQjFuFD_S64bpMl9akkSbNrOA,1289
-hich_restrict-0.1.0.dist-info/METADATA,sha256=4yeR61yeh8kzRTNVUBStlUCChkTOPEwt13L88FUzjgY,445
-hich_restrict-0.1.0.dist-info/WHEEL,sha256=FMvqSimYX_P7y0a7UY-_Mc83r5zkBZsCYPm7Lr0Bsq4,88
-hich_restrict-0.1.0.dist-info/entry_points.txt,sha256=gO9fXm7Uq94XUtbPUFzStNx2VxM8N-JfSK8hBqaBiZU,60
-hich_restrict-0.1.0.dist-info/RECORD,,
+hich_restrict-0.1.1.dist-info/METADATA,sha256=I0MQm3l6usqlDSsrA-PuwoRYJun-2fRnYaWQ_jE3tqg,445
+hich_restrict-0.1.1.dist-info/WHEEL,sha256=FMvqSimYX_P7y0a7UY-_Mc83r5zkBZsCYPm7Lr0Bsq4,88
+hich_restrict-0.1.1.dist-info/entry_points.txt,sha256=gO9fXm7Uq94XUtbPUFzStNx2VxM8N-JfSK8hBqaBiZU,60
+hich_restrict-0.1.1.dist-info/RECORD,,
```

