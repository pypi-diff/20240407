# Comparing `tmp/ggun-0.1.3-py3-none-any.whl.zip` & `tmp/ggun-0.1.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 9515 bytes, number of entries: 12
+Zip file size: 9590 bytes, number of entries: 12
 -rw-rw-r--  2.0 unx       23 b- defN 24-Apr-05 13:04 ggun/__init__.py
 -rw-rw-r--  2.0 unx     5578 b- defN 24-Apr-07 15:01 ggun/main.py
 -rw-rw-r--  2.0 unx       20 b- defN 24-Mar-31 13:47 ggun/commands/__init__.py
 -rw-rw-r--  2.0 unx    14337 b- defN 24-Apr-07 15:13 ggun/commands/test.py
 -rw-rw-r--  2.0 unx        0 b- defN 24-Mar-31 13:35 utils/__init__.py
 -rw-rw-r--  2.0 unx     1480 b- defN 24-Apr-07 15:01 utils/api_call.py
--rw-rw-r--  2.0 unx     3315 b- defN 24-Apr-07 15:13 utils/list_files.py
--rw-rw-r--  2.0 unx      231 b- defN 24-Apr-07 15:14 ggun-0.1.3.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 24-Apr-07 15:14 ggun-0.1.3.dist-info/WHEEL
--rw-rw-r--  2.0 unx       35 b- defN 24-Apr-07 15:14 ggun-0.1.3.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx       11 b- defN 24-Apr-07 15:14 ggun-0.1.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      897 b- defN 24-Apr-07 15:14 ggun-0.1.3.dist-info/RECORD
-12 files, 26019 bytes uncompressed, 8021 bytes compressed:  69.2%
+-rw-rw-r--  2.0 unx     3537 b- defN 24-Apr-07 15:28 utils/list_files.py
+-rw-rw-r--  2.0 unx      231 b- defN 24-Apr-07 15:31 ggun-0.1.4.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 24-Apr-07 15:31 ggun-0.1.4.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       35 b- defN 24-Apr-07 15:31 ggun-0.1.4.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx       11 b- defN 24-Apr-07 15:31 ggun-0.1.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      897 b- defN 24-Apr-07 15:31 ggun-0.1.4.dist-info/RECORD
+12 files, 26241 bytes uncompressed, 8096 bytes compressed:  69.1%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: utils/api_call.py
 Comment: 
 
 Filename: utils/list_files.py
 Comment: 
 
-Filename: ggun-0.1.3.dist-info/METADATA
+Filename: ggun-0.1.4.dist-info/METADATA
 Comment: 
 
-Filename: ggun-0.1.3.dist-info/WHEEL
+Filename: ggun-0.1.4.dist-info/WHEEL
 Comment: 
 
-Filename: ggun-0.1.3.dist-info/entry_points.txt
+Filename: ggun-0.1.4.dist-info/entry_points.txt
 Comment: 
 
-Filename: ggun-0.1.3.dist-info/top_level.txt
+Filename: ggun-0.1.4.dist-info/top_level.txt
 Comment: 
 
-Filename: ggun-0.1.3.dist-info/RECORD
+Filename: ggun-0.1.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## utils/list_files.py

```diff
@@ -5,34 +5,38 @@
 
 
 def list_forge_test_strace_files(directory, show_tree, exclude_file_types=[]):
     """
     List all files in a directory that are being used by forge test.
     """
     # Define the command to be executed
-    command = "strace -f -e trace=%file -e read=none -e write=none forge test 2>&1 | grep -E 'openat\\(.*\\.sol'"
-
+    command = (
+        "strace -f -e trace=%file -e read=none -e write=none forge test 2>&1"
+        " | grep -E 'openat\\(.*\\.sol'"
+    )
     # Change the current working directory to ~/Test_Ggun/vanilla
-    cwd = expanduser("~/Test_Ggun/vanilla")
+    cwd = expanduser(directory)
 
     # Run the command
     process = subprocess.Popen(
         command,
         shell=True,
         stdout=subprocess.PIPE,
         stderr=subprocess.STDOUT,
         cwd=cwd,
         text=True,
     )
 
     # Read the output
     output, _ = process.communicate()
 
-    # Find all paths in the output
-    paths = re.findall(r"\"(.+\.sol)\"", output)
+    # Find all paths in the output and convert them to relative paths
+    absolute_paths = re.findall(r"\"(.+\.sol)\"", output)
+    paths = [os.path.relpath(path, cwd) for path in absolute_paths]
+    paths = ["./" + path for path in paths]
 
     return paths
 
 
 
 
 def list_git_files(directory, show_tree, exclude_file_types=[]):
@@ -79,23 +83,23 @@
 
 
 def test_list_git_files():
     """
     Test the list_git_files function with a known directory structure.
     """
     # Assuming the current directory has a .git and it's not empty
-    directory = "."
+    directory = "../Test_Ggun/vanilla"    
     print("Testing list_git_files with show_tree=False")
     file_list = list_git_files(directory, show_tree=False)
     print(file_list)
 
     print("\nTesting list_git_files with show_tree=True")
     file_list = list_git_files(directory, show_tree=True)
     print(file_list)
 
 
 if __name__ == "__main__":
-    # test_list_git_files()
     directory = "~/Test_Ggun/vanilla"
+
+    # files = list_git_files(directory, show_tree=False)
     files = list_forge_test_strace_files(directory, show_tree=True)
     print(files)
-
```

## Comparing `ggun-0.1.3.dist-info/RECORD` & `ggun-0.1.4.dist-info/RECORD`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 ggun/__init__.py,sha256=ZuXHO-b9d-MyvTiU9PSfWItKChRjKMqjHD15a7a9pZk,23
 ggun/main.py,sha256=ZBQsiscSFbRb6ZlIHPRg0C0nRu72hB2YZxyyzBYj4ac,5578
 ggun/commands/__init__.py,sha256=NN4uHMI_a8xSJCUbzuPTfd14fY-t0vPGHwWjrmzgSL4,20
 ggun/commands/test.py,sha256=L0DmY7pafTisWmdDgYfVKCZZJC5rbbQWCcu96LYPcCI,14337
 utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 utils/api_call.py,sha256=3Ms1Q8J-Ugj5_d2t0mHIeG81QbVmWJGLG4Z4vnKEyv4,1480
-utils/list_files.py,sha256=gr4cvixgtb10f3aW--NTOMY11BxJFJ-KGQ4KBvOPC2g,3315
-ggun-0.1.3.dist-info/METADATA,sha256=JQsCs-QkBW-roLIhNTXxL5jRTsDyc6ki_6-nWOu3-fI,231
-ggun-0.1.3.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-ggun-0.1.3.dist-info/entry_points.txt,sha256=YdLq3ka3RZvTQrtNCRK17TS8pXpWX4-tNzRL-uEpTC0,35
-ggun-0.1.3.dist-info/top_level.txt,sha256=7KfY85D4hwH5PHyWRel9YWjQzZNDVOugwhYxA64r0Qs,11
-ggun-0.1.3.dist-info/RECORD,,
+utils/list_files.py,sha256=Nayz2SWi7IalXlr2pGEasFT1j72JZW_ljEp1kKpD0MY,3537
+ggun-0.1.4.dist-info/METADATA,sha256=N0jFsbwezH6gtwnXdMeTcMxB4mQUNF1U4fdnUMdP6hE,231
+ggun-0.1.4.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+ggun-0.1.4.dist-info/entry_points.txt,sha256=YdLq3ka3RZvTQrtNCRK17TS8pXpWX4-tNzRL-uEpTC0,35
+ggun-0.1.4.dist-info/top_level.txt,sha256=7KfY85D4hwH5PHyWRel9YWjQzZNDVOugwhYxA64r0Qs,11
+ggun-0.1.4.dist-info/RECORD,,
```

