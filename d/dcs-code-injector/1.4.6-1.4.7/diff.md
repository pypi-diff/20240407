# Comparing `tmp/dcs-code-injector-1.4.6.tar.gz` & `tmp/dcs-code-injector-1.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcs-code-injector-1.4.6.tar", last modified: Sat Mar 30 13:12:39 2024, max compression
+gzip compressed data, was "dcs-code-injector-1.4.7.tar", last modified: Sun Apr  7 12:14:13 2024, max compression
```

## Comparing `dcs-code-injector-1.4.6.tar` & `dcs-code-injector-1.4.7.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxrwxrwx   0        0        0        0 2024-03-30 13:12:39.541647 dcs-code-injector-1.4.6/
--rw-rw-rw-   0        0        0    35823 2024-03-30 13:10:55.000000 dcs-code-injector-1.4.6/LICENSE
--rw-rw-rw-   0        0        0     9038 2024-03-30 13:12:39.541647 dcs-code-injector-1.4.6/PKG-INFO
--rw-rw-rw-   0        0        0     8474 2024-03-30 13:10:55.000000 dcs-code-injector-1.4.6/README.md
-drwxrwxrwx   0        0        0        0 2024-03-30 13:12:39.526026 dcs-code-injector-1.4.6/dcs_code_injector/
--rw-rw-rw-   0        0        0      253 2024-03-30 13:10:55.000000 dcs-code-injector-1.4.6/dcs_code_injector/__init__.py
--rw-rw-rw-   0        0        0     3128 2024-03-30 13:10:55.000000 dcs-code-injector-1.4.6/dcs_code_injector/app.py
--rw-rw-rw-   0        0        0    22855 2024-03-30 13:10:55.000000 dcs-code-injector-1.4.6/dcs_code_injector/code_editor.py
--rw-rw-rw-   0        0        0     2298 2024-03-30 13:10:55.000000 dcs-code-injector-1.4.6/dcs_code_injector/constants.py
--rw-rw-rw-   0        0        0    15193 2024-03-30 13:10:55.000000 dcs-code-injector-1.4.6/dcs_code_injector/dcs_code_injector_window.py
--rw-rw-rw-   0        0        0     3955 2024-03-30 13:10:55.000000 dcs-code-injector-1.4.6/dcs_code_injector/favorites.py
--rw-rw-rw-   0        0        0     2725 2024-03-30 13:10:55.000000 dcs-code-injector-1.4.6/dcs_code_injector/hook_string.py
--rw-rw-rw-   0        0        0     1748 2024-03-30 13:10:55.000000 dcs-code-injector-1.4.6/dcs_code_injector/log_highlighter.py
--rw-rw-rw-   0        0        0     5352 2024-03-30 13:10:55.000000 dcs-code-injector-1.4.6/dcs_code_injector/log_view.py
--rw-rw-rw-   0        0        0     1549 2024-03-30 13:10:55.000000 dcs-code-injector-1.4.6/dcs_code_injector/logger.py
--rw-rw-rw-   0        0        0     1003 2024-03-30 13:10:55.000000 dcs-code-injector-1.4.6/dcs_code_injector/lua_function_parser.py
--rw-rw-rw-   0        0        0    10005 2024-03-30 13:10:55.000000 dcs-code-injector-1.4.6/dcs_code_injector/lua_syntax_highlighter.py
--rw-rw-rw-   0        0        0     2862 2024-03-30 13:10:55.000000 dcs-code-injector-1.4.6/dcs_code_injector/server.py
--rw-rw-rw-   0        0        0     7414 2024-03-30 13:10:55.000000 dcs-code-injector-1.4.6/dcs_code_injector/settings_dialog.py
-drwxrwxrwx   0        0        0        0 2024-03-30 13:12:39.526026 dcs-code-injector-1.4.6/dcs_code_injector/ui/
--rw-rw-rw-   0        0        0        0 2024-03-30 13:10:55.000000 dcs-code-injector-1.4.6/dcs_code_injector/ui/__init__.py
--rw-rw-rw-   0        0        0     2602 2024-03-30 13:10:55.000000 dcs-code-injector-1.4.6/dcs_code_injector/ui/dcs_code_injector_search_ui.py
--rw-rw-rw-   0        0        0    11018 2024-03-30 13:10:55.000000 dcs-code-injector-1.4.6/dcs_code_injector/ui/dcs_code_injector_settings_ui.py
--rw-rw-rw-   0        0        0    11238 2024-03-30 13:10:55.000000 dcs-code-injector-1.4.6/dcs_code_injector/ui/dcs_code_injector_window_ui.py
-drwxrwxrwx   0        0        0        0 2024-03-30 13:12:39.526026 dcs-code-injector-1.4.6/dcs_code_injector/ui/icons/
--rw-rw-rw-   0        0        0        0 2024-03-30 13:10:55.000000 dcs-code-injector-1.4.6/dcs_code_injector/ui/icons/__init__.py
--rw-rw-rw-   0        0        0      855 2024-03-30 13:10:55.000000 dcs-code-injector-1.4.6/dcs_code_injector/ui/icons/cloud_done.png
--rw-rw-rw-   0        0        0     1126 2024-03-30 13:10:55.000000 dcs-code-injector-1.4.6/dcs_code_injector/ui/icons/cloud_off.png
--rw-rw-rw-   0        0        0     5569 2024-03-30 13:10:55.000000 dcs-code-injector-1.4.6/dcs_code_injector/ui/icons/icon.png
--rw-rw-rw-   0        0        0    95798 2024-03-30 13:10:55.000000 dcs-code-injector-1.4.6/dcs_code_injector/ui/icons/logo.png
-drwxrwxrwx   0        0        0        0 2024-03-30 13:12:39.541647 dcs-code-injector-1.4.6/dcs_code_injector/ui/splashscreens/
--rw-rw-rw-   0        0        0        0 2024-03-30 13:10:55.000000 dcs-code-injector-1.4.6/dcs_code_injector/ui/splashscreens/__init__.py
--rw-rw-rw-   0        0        0   629069 2024-03-30 13:10:55.000000 dcs-code-injector-1.4.6/dcs_code_injector/ui/splashscreens/splash_01.png
--rw-rw-rw-   0        0        0   831944 2024-03-30 13:10:55.000000 dcs-code-injector-1.4.6/dcs_code_injector/ui/splashscreens/splash_02.png
--rw-rw-rw-   0        0        0   927761 2024-03-30 13:10:55.000000 dcs-code-injector-1.4.6/dcs_code_injector/ui/splashscreens/splash_03.png
--rw-rw-rw-   0        0        0   932507 2024-03-30 13:10:55.000000 dcs-code-injector-1.4.6/dcs_code_injector/ui/splashscreens/splash_04.png
--rw-rw-rw-   0        0        0   723796 2024-03-30 13:10:55.000000 dcs-code-injector-1.4.6/dcs_code_injector/ui/splashscreens/splash_05.png
--rw-rw-rw-   0        0        0   916284 2024-03-30 13:10:55.000000 dcs-code-injector-1.4.6/dcs_code_injector/ui/splashscreens/splash_06.png
--rw-rw-rw-   0        0        0   968922 2024-03-30 13:10:55.000000 dcs-code-injector-1.4.6/dcs_code_injector/ui/splashscreens/splash_07.png
--rw-rw-rw-   0        0        0     2298 2024-03-30 13:10:55.000000 dcs-code-injector-1.4.6/dcs_code_injector/utils.py
--rw-rw-rw-   0        0        0     3188 2024-03-30 13:10:55.000000 dcs-code-injector-1.4.6/dcs_code_injector/variables_tree.py
--rw-rw-rw-   0        0        0      891 2024-03-30 13:10:55.000000 dcs-code-injector-1.4.6/dcs_code_injector/version_dialog.py
--rw-rw-rw-   0        0        0     6289 2024-03-30 13:10:55.000000 dcs-code-injector-1.4.6/dcs_code_injector/versioner.py
-drwxrwxrwx   0        0        0        0 2024-03-30 13:12:39.541647 dcs-code-injector-1.4.6/dcs_code_injector.egg-info/
--rw-rw-rw-   0        0        0     9038 2024-03-30 13:12:39.000000 dcs-code-injector-1.4.6/dcs_code_injector.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1653 2024-03-30 13:12:39.000000 dcs-code-injector-1.4.6/dcs_code_injector.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-30 13:12:39.000000 dcs-code-injector-1.4.6/dcs_code_injector.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       65 2024-03-30 13:12:39.000000 dcs-code-injector-1.4.6/dcs_code_injector.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       73 2024-03-30 13:12:39.000000 dcs-code-injector-1.4.6/dcs_code_injector.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-03-30 13:12:39.000000 dcs-code-injector-1.4.6/dcs_code_injector.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-30 13:12:39.541647 dcs-code-injector-1.4.6/setup.cfg
--rw-rw-rw-   0        0        0      970 2024-03-30 13:10:55.000000 dcs-code-injector-1.4.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-07 12:14:13.564144 dcs-code-injector-1.4.7/
+-rw-rw-rw-   0        0        0    35823 2024-04-07 12:12:34.000000 dcs-code-injector-1.4.7/LICENSE
+-rw-rw-rw-   0        0        0     9038 2024-04-07 12:14:13.564144 dcs-code-injector-1.4.7/PKG-INFO
+-rw-rw-rw-   0        0        0     8474 2024-04-07 12:12:34.000000 dcs-code-injector-1.4.7/README.md
+drwxrwxrwx   0        0        0        0 2024-04-07 12:14:13.548519 dcs-code-injector-1.4.7/dcs_code_injector/
+-rw-rw-rw-   0        0        0      253 2024-04-07 12:12:34.000000 dcs-code-injector-1.4.7/dcs_code_injector/__init__.py
+-rw-rw-rw-   0        0        0     3128 2024-04-07 12:12:34.000000 dcs-code-injector-1.4.7/dcs_code_injector/app.py
+-rw-rw-rw-   0        0        0    23577 2024-04-07 12:12:34.000000 dcs-code-injector-1.4.7/dcs_code_injector/code_editor.py
+-rw-rw-rw-   0        0        0     2298 2024-04-07 12:12:34.000000 dcs-code-injector-1.4.7/dcs_code_injector/constants.py
+-rw-rw-rw-   0        0        0    15193 2024-04-07 12:12:34.000000 dcs-code-injector-1.4.7/dcs_code_injector/dcs_code_injector_window.py
+-rw-rw-rw-   0        0        0     3955 2024-04-07 12:12:34.000000 dcs-code-injector-1.4.7/dcs_code_injector/favorites.py
+-rw-rw-rw-   0        0        0     2725 2024-04-07 12:12:34.000000 dcs-code-injector-1.4.7/dcs_code_injector/hook_string.py
+-rw-rw-rw-   0        0        0     1748 2024-04-07 12:12:34.000000 dcs-code-injector-1.4.7/dcs_code_injector/log_highlighter.py
+-rw-rw-rw-   0        0        0     5352 2024-04-07 12:12:34.000000 dcs-code-injector-1.4.7/dcs_code_injector/log_view.py
+-rw-rw-rw-   0        0        0     1549 2024-04-07 12:12:34.000000 dcs-code-injector-1.4.7/dcs_code_injector/logger.py
+-rw-rw-rw-   0        0        0     1003 2024-04-07 12:12:34.000000 dcs-code-injector-1.4.7/dcs_code_injector/lua_function_parser.py
+-rw-rw-rw-   0        0        0    10005 2024-04-07 12:12:34.000000 dcs-code-injector-1.4.7/dcs_code_injector/lua_syntax_highlighter.py
+-rw-rw-rw-   0        0        0     2862 2024-04-07 12:12:34.000000 dcs-code-injector-1.4.7/dcs_code_injector/server.py
+-rw-rw-rw-   0        0        0     7414 2024-04-07 12:12:34.000000 dcs-code-injector-1.4.7/dcs_code_injector/settings_dialog.py
+drwxrwxrwx   0        0        0        0 2024-04-07 12:14:13.548519 dcs-code-injector-1.4.7/dcs_code_injector/ui/
+-rw-rw-rw-   0        0        0        0 2024-04-07 12:12:34.000000 dcs-code-injector-1.4.7/dcs_code_injector/ui/__init__.py
+-rw-rw-rw-   0        0        0     2602 2024-04-07 12:12:34.000000 dcs-code-injector-1.4.7/dcs_code_injector/ui/dcs_code_injector_search_ui.py
+-rw-rw-rw-   0        0        0    11018 2024-04-07 12:12:34.000000 dcs-code-injector-1.4.7/dcs_code_injector/ui/dcs_code_injector_settings_ui.py
+-rw-rw-rw-   0        0        0    11238 2024-04-07 12:12:34.000000 dcs-code-injector-1.4.7/dcs_code_injector/ui/dcs_code_injector_window_ui.py
+drwxrwxrwx   0        0        0        0 2024-04-07 12:14:13.548519 dcs-code-injector-1.4.7/dcs_code_injector/ui/icons/
+-rw-rw-rw-   0        0        0        0 2024-04-07 12:12:34.000000 dcs-code-injector-1.4.7/dcs_code_injector/ui/icons/__init__.py
+-rw-rw-rw-   0        0        0      855 2024-04-07 12:12:34.000000 dcs-code-injector-1.4.7/dcs_code_injector/ui/icons/cloud_done.png
+-rw-rw-rw-   0        0        0     1126 2024-04-07 12:12:34.000000 dcs-code-injector-1.4.7/dcs_code_injector/ui/icons/cloud_off.png
+-rw-rw-rw-   0        0        0     5569 2024-04-07 12:12:34.000000 dcs-code-injector-1.4.7/dcs_code_injector/ui/icons/icon.png
+-rw-rw-rw-   0        0        0    95798 2024-04-07 12:12:34.000000 dcs-code-injector-1.4.7/dcs_code_injector/ui/icons/logo.png
+drwxrwxrwx   0        0        0        0 2024-04-07 12:14:13.564144 dcs-code-injector-1.4.7/dcs_code_injector/ui/splashscreens/
+-rw-rw-rw-   0        0        0        0 2024-04-07 12:12:34.000000 dcs-code-injector-1.4.7/dcs_code_injector/ui/splashscreens/__init__.py
+-rw-rw-rw-   0        0        0   629069 2024-04-07 12:12:34.000000 dcs-code-injector-1.4.7/dcs_code_injector/ui/splashscreens/splash_01.png
+-rw-rw-rw-   0        0        0   831944 2024-04-07 12:12:34.000000 dcs-code-injector-1.4.7/dcs_code_injector/ui/splashscreens/splash_02.png
+-rw-rw-rw-   0        0        0   927761 2024-04-07 12:12:34.000000 dcs-code-injector-1.4.7/dcs_code_injector/ui/splashscreens/splash_03.png
+-rw-rw-rw-   0        0        0   932507 2024-04-07 12:12:35.000000 dcs-code-injector-1.4.7/dcs_code_injector/ui/splashscreens/splash_04.png
+-rw-rw-rw-   0        0        0   723796 2024-04-07 12:12:35.000000 dcs-code-injector-1.4.7/dcs_code_injector/ui/splashscreens/splash_05.png
+-rw-rw-rw-   0        0        0   916284 2024-04-07 12:12:35.000000 dcs-code-injector-1.4.7/dcs_code_injector/ui/splashscreens/splash_06.png
+-rw-rw-rw-   0        0        0   968922 2024-04-07 12:12:35.000000 dcs-code-injector-1.4.7/dcs_code_injector/ui/splashscreens/splash_07.png
+-rw-rw-rw-   0        0        0     2298 2024-04-07 12:12:35.000000 dcs-code-injector-1.4.7/dcs_code_injector/utils.py
+-rw-rw-rw-   0        0        0     3188 2024-04-07 12:12:35.000000 dcs-code-injector-1.4.7/dcs_code_injector/variables_tree.py
+-rw-rw-rw-   0        0        0      891 2024-04-07 12:12:35.000000 dcs-code-injector-1.4.7/dcs_code_injector/version_dialog.py
+-rw-rw-rw-   0        0        0     6289 2024-04-07 12:12:35.000000 dcs-code-injector-1.4.7/dcs_code_injector/versioner.py
+drwxrwxrwx   0        0        0        0 2024-04-07 12:14:13.564144 dcs-code-injector-1.4.7/dcs_code_injector.egg-info/
+-rw-rw-rw-   0        0        0     9038 2024-04-07 12:14:13.000000 dcs-code-injector-1.4.7/dcs_code_injector.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1653 2024-04-07 12:14:13.000000 dcs-code-injector-1.4.7/dcs_code_injector.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-07 12:14:13.000000 dcs-code-injector-1.4.7/dcs_code_injector.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       65 2024-04-07 12:14:13.000000 dcs-code-injector-1.4.7/dcs_code_injector.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       73 2024-04-07 12:14:13.000000 dcs-code-injector-1.4.7/dcs_code_injector.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-04-07 12:14:13.000000 dcs-code-injector-1.4.7/dcs_code_injector.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-07 12:14:13.564144 dcs-code-injector-1.4.7/setup.cfg
+-rw-rw-rw-   0        0        0      970 2024-04-07 12:12:35.000000 dcs-code-injector-1.4.7/setup.py
```

### Comparing `dcs-code-injector-1.4.6/LICENSE` & `dcs-code-injector-1.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `dcs-code-injector-1.4.6/PKG-INFO` & `dcs-code-injector-1.4.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcs-code-injector
-Version: 1.4.6
+Version: 1.4.7
 Summary: A REPL to use with Digital Combat Simulator to execute code while a mission is running.
 Home-page: https://www.github.com/nielsvaes/dcs_code_injector
 Author: Niels Vaes
 Author-email: nielsvaes@gmail.com
 License: GNU v3
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `dcs-code-injector-1.4.6/README.md` & `dcs-code-injector-1.4.7/README.md`

 * *Files identical despite different names*

### Comparing `dcs-code-injector-1.4.6/dcs_code_injector/app.py` & `dcs-code-injector-1.4.7/dcs_code_injector/app.py`

 * *Files identical despite different names*

### Comparing `dcs-code-injector-1.4.6/dcs_code_injector/code_editor.py` & `dcs-code-injector-1.4.7/dcs_code_injector/code_editor.py`

 * *Files 2% similar despite different names*

```diff
@@ -359,14 +359,18 @@
             elif event.key() == Qt.Key_Tab:
                 self.handle_tab()
             elif event.key() == Qt.Key_Backtab:
                 self.handle_backtab()
             elif event.key() in (Qt.Key_Up, Qt.Key_Down):
                 super().keyPressEvent(event)
                 self.check_cursor_position()
+            if event.key() == Qt.Key_X and event.modifiers() == Qt.ControlModifier:
+                self.delete_current_line()
+            if event.key() == Qt.Key_D and event.modifiers() == Qt.ControlModifier:
+                self.duplicate_current_line()
             elif event.key() == Qt.Key_Return or event.key() == Qt.Key_Enter and not event.modifiers() == Qt.ControlModifier:
                 cursor = self.textCursor()
                 current_line = cursor.block().text()
                 indentation = re.match(r"\s*", current_line).group()  # Capture leading whitespace
                 super().keyPressEvent(event)  # Call the parent method to insert the newline
                 self.insertPlainText(indentation)  # Insert the captured indentation
                 self.check_cursor_position()
@@ -508,14 +512,27 @@
             cursor.setPosition(end, QTextCursor.KeepAnchor)
             cursor.insertText("\n".join(unindented_lines))
 
             cursor.setPosition(start)
             cursor.setPosition(start + len("\n".join(unindented_lines)), QTextCursor.KeepAnchor)
             self.setTextCursor(cursor)
 
+    def delete_current_line(self):
+        cursor = self.textCursor()
+        cursor.select(QTextCursor.LineUnderCursor)
+        cursor.removeSelectedText()
+        cursor.deleteChar()
+
+    def duplicate_current_line(self):
+        cursor = self.textCursor()
+        cursor.select(QTextCursor.LineUnderCursor)
+        line_text = cursor.selectedText()
+        cursor.movePosition(QTextCursor.EndOfLine)
+        cursor.insertText('\n' + line_text)
+
     def resizeEvent(self, event):
         """
         Handles the resize event of the text editor to adjust the line number area accordingly.
 
         Parameters:
             event (QResizeEvent): The resize event.
         """
```

### Comparing `dcs-code-injector-1.4.6/dcs_code_injector/constants.py` & `dcs-code-injector-1.4.7/dcs_code_injector/constants.py`

 * *Files identical despite different names*

### Comparing `dcs-code-injector-1.4.6/dcs_code_injector/dcs_code_injector_window.py` & `dcs-code-injector-1.4.7/dcs_code_injector/dcs_code_injector_window.py`

 * *Files identical despite different names*

### Comparing `dcs-code-injector-1.4.6/dcs_code_injector/favorites.py` & `dcs-code-injector-1.4.7/dcs_code_injector/favorites.py`

 * *Files identical despite different names*

### Comparing `dcs-code-injector-1.4.6/dcs_code_injector/hook_string.py` & `dcs-code-injector-1.4.7/dcs_code_injector/hook_string.py`

 * *Files identical despite different names*

### Comparing `dcs-code-injector-1.4.6/dcs_code_injector/log_highlighter.py` & `dcs-code-injector-1.4.7/dcs_code_injector/log_highlighter.py`

 * *Files identical despite different names*

### Comparing `dcs-code-injector-1.4.6/dcs_code_injector/log_view.py` & `dcs-code-injector-1.4.7/dcs_code_injector/log_view.py`

 * *Files identical despite different names*

### Comparing `dcs-code-injector-1.4.6/dcs_code_injector/logger.py` & `dcs-code-injector-1.4.7/dcs_code_injector/logger.py`

 * *Files identical despite different names*

### Comparing `dcs-code-injector-1.4.6/dcs_code_injector/lua_function_parser.py` & `dcs-code-injector-1.4.7/dcs_code_injector/lua_function_parser.py`

 * *Files identical despite different names*

### Comparing `dcs-code-injector-1.4.6/dcs_code_injector/lua_syntax_highlighter.py` & `dcs-code-injector-1.4.7/dcs_code_injector/lua_syntax_highlighter.py`

 * *Files identical despite different names*

### Comparing `dcs-code-injector-1.4.6/dcs_code_injector/server.py` & `dcs-code-injector-1.4.7/dcs_code_injector/server.py`

 * *Files identical despite different names*

### Comparing `dcs-code-injector-1.4.6/dcs_code_injector/settings_dialog.py` & `dcs-code-injector-1.4.7/dcs_code_injector/settings_dialog.py`

 * *Files identical despite different names*

### Comparing `dcs-code-injector-1.4.6/dcs_code_injector/ui/dcs_code_injector_search_ui.py` & `dcs-code-injector-1.4.7/dcs_code_injector/ui/dcs_code_injector_search_ui.py`

 * *Files identical despite different names*

### Comparing `dcs-code-injector-1.4.6/dcs_code_injector/ui/dcs_code_injector_settings_ui.py` & `dcs-code-injector-1.4.7/dcs_code_injector/ui/dcs_code_injector_settings_ui.py`

 * *Files identical despite different names*

### Comparing `dcs-code-injector-1.4.6/dcs_code_injector/ui/dcs_code_injector_window_ui.py` & `dcs-code-injector-1.4.7/dcs_code_injector/ui/dcs_code_injector_window_ui.py`

 * *Files identical despite different names*

### Comparing `dcs-code-injector-1.4.6/dcs_code_injector/ui/icons/cloud_done.png` & `dcs-code-injector-1.4.7/dcs_code_injector/ui/icons/cloud_done.png`

 * *Files identical despite different names*

### Comparing `dcs-code-injector-1.4.6/dcs_code_injector/ui/icons/cloud_off.png` & `dcs-code-injector-1.4.7/dcs_code_injector/ui/icons/cloud_off.png`

 * *Files identical despite different names*

### Comparing `dcs-code-injector-1.4.6/dcs_code_injector/ui/icons/icon.png` & `dcs-code-injector-1.4.7/dcs_code_injector/ui/icons/icon.png`

 * *Files identical despite different names*

### Comparing `dcs-code-injector-1.4.6/dcs_code_injector/ui/icons/logo.png` & `dcs-code-injector-1.4.7/dcs_code_injector/ui/icons/logo.png`

 * *Files identical despite different names*

### Comparing `dcs-code-injector-1.4.6/dcs_code_injector/ui/splashscreens/splash_01.png` & `dcs-code-injector-1.4.7/dcs_code_injector/ui/splashscreens/splash_01.png`

 * *Files identical despite different names*

### Comparing `dcs-code-injector-1.4.6/dcs_code_injector/ui/splashscreens/splash_02.png` & `dcs-code-injector-1.4.7/dcs_code_injector/ui/splashscreens/splash_02.png`

 * *Files identical despite different names*

### Comparing `dcs-code-injector-1.4.6/dcs_code_injector/ui/splashscreens/splash_03.png` & `dcs-code-injector-1.4.7/dcs_code_injector/ui/splashscreens/splash_03.png`

 * *Files identical despite different names*

### Comparing `dcs-code-injector-1.4.6/dcs_code_injector/ui/splashscreens/splash_04.png` & `dcs-code-injector-1.4.7/dcs_code_injector/ui/splashscreens/splash_04.png`

 * *Files identical despite different names*

### Comparing `dcs-code-injector-1.4.6/dcs_code_injector/ui/splashscreens/splash_05.png` & `dcs-code-injector-1.4.7/dcs_code_injector/ui/splashscreens/splash_05.png`

 * *Files identical despite different names*

### Comparing `dcs-code-injector-1.4.6/dcs_code_injector/ui/splashscreens/splash_06.png` & `dcs-code-injector-1.4.7/dcs_code_injector/ui/splashscreens/splash_06.png`

 * *Files identical despite different names*

### Comparing `dcs-code-injector-1.4.6/dcs_code_injector/ui/splashscreens/splash_07.png` & `dcs-code-injector-1.4.7/dcs_code_injector/ui/splashscreens/splash_07.png`

 * *Files identical despite different names*

### Comparing `dcs-code-injector-1.4.6/dcs_code_injector/utils.py` & `dcs-code-injector-1.4.7/dcs_code_injector/utils.py`

 * *Files identical despite different names*

### Comparing `dcs-code-injector-1.4.6/dcs_code_injector/variables_tree.py` & `dcs-code-injector-1.4.7/dcs_code_injector/variables_tree.py`

 * *Files identical despite different names*

### Comparing `dcs-code-injector-1.4.6/dcs_code_injector/version_dialog.py` & `dcs-code-injector-1.4.7/dcs_code_injector/version_dialog.py`

 * *Files identical despite different names*

### Comparing `dcs-code-injector-1.4.6/dcs_code_injector/versioner.py` & `dcs-code-injector-1.4.7/dcs_code_injector/versioner.py`

 * *Files identical despite different names*

### Comparing `dcs-code-injector-1.4.6/dcs_code_injector.egg-info/PKG-INFO` & `dcs-code-injector-1.4.7/dcs_code_injector.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcs-code-injector
-Version: 1.4.6
+Version: 1.4.7
 Summary: A REPL to use with Digital Combat Simulator to execute code while a mission is running.
 Home-page: https://www.github.com/nielsvaes/dcs_code_injector
 Author: Niels Vaes
 Author-email: nielsvaes@gmail.com
 License: GNU v3
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `dcs-code-injector-1.4.6/dcs_code_injector.egg-info/SOURCES.txt` & `dcs-code-injector-1.4.7/dcs_code_injector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dcs-code-injector-1.4.6/setup.py` & `dcs-code-injector-1.4.7/setup.py`

 * *Files identical despite different names*

