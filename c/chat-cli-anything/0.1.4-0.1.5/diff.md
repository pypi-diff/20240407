# Comparing `tmp/chat_cli_anything-0.1.4.tar.gz` & `tmp/chat_cli_anything-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chat_cli_anything-0.1.4.tar", max compression
+gzip compressed data, was "chat_cli_anything-0.1.5.tar", max compression
```

## Comparing `chat_cli_anything-0.1.4.tar` & `chat_cli_anything-0.1.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    11357 2024-03-13 16:33:27.236056 chat_cli_anything-0.1.4/LICENSE
--rw-r--r--   0        0        0     7696 2024-04-03 09:54:05.392800 chat_cli_anything-0.1.4/README.md
--rw-r--r--   0        0        0        0 2024-03-20 12:50:07.078680 chat_cli_anything-0.1.4/chat_cli_anything/__init__.py
--rw-r--r--   0        0        0    28974 2024-04-03 09:59:28.022343 chat_cli_anything-0.1.4/chat_cli_anything/ask.py
--rw-r--r--   0        0        0     6896 2024-04-03 05:20:02.168901 chat_cli_anything-0.1.4/chat_cli_anything/config.py
--rw-r--r--   0        0        0     7876 2024-04-03 09:16:53.301015 chat_cli_anything-0.1.4/chat_cli_anything/db.py
--rw-r--r--   0        0        0     1621 2024-04-03 09:17:55.507727 chat_cli_anything-0.1.4/chat_cli_anything/embedding.py
--rw-r--r--   0        0        0     2798 2024-04-03 06:48:40.337190 chat_cli_anything-0.1.4/chat_cli_anything/loader.py
--rw-r--r--   0        0        0     2714 2024-04-03 07:17:55.368638 chat_cli_anything-0.1.4/chat_cli_anything/request.py
--rw-r--r--   0        0        0      729 2024-03-31 17:35:50.217211 chat_cli_anything-0.1.4/chat_cli_anything/rerank.py
--rw-r--r--   0        0        0     1868 2024-04-01 08:49:00.737620 chat_cli_anything-0.1.4/chat_cli_anything/service.py
--rw-r--r--   0        0        0     1050 2024-04-02 06:30:30.360008 chat_cli_anything-0.1.4/chat_cli_anything/util.py
--rw-r--r--   0        0        0     1465 2024-04-03 10:15:53.523917 chat_cli_anything-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     9237 1970-01-01 00:00:00.000000 chat_cli_anything-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-03-13 16:33:27.236056 chat_cli_anything-0.1.5/LICENSE
+-rw-r--r--   0        0        0     7930 2024-04-07 09:17:05.654963 chat_cli_anything-0.1.5/README.md
+-rw-r--r--   0        0        0        0 2024-03-20 12:50:07.078680 chat_cli_anything-0.1.5/chat_cli_anything/__init__.py
+-rw-r--r--   0        0        0    29932 2024-04-07 08:01:49.273506 chat_cli_anything-0.1.5/chat_cli_anything/ask.py
+-rw-r--r--   0        0        0     6896 2024-04-03 05:20:02.168901 chat_cli_anything-0.1.5/chat_cli_anything/config.py
+-rw-r--r--   0        0        0     7876 2024-04-03 09:16:53.301015 chat_cli_anything-0.1.5/chat_cli_anything/db.py
+-rw-r--r--   0        0        0     1621 2024-04-03 09:17:55.507727 chat_cli_anything-0.1.5/chat_cli_anything/embedding.py
+-rw-r--r--   0        0        0     2798 2024-04-03 06:48:40.337190 chat_cli_anything-0.1.5/chat_cli_anything/loader.py
+-rw-r--r--   0        0        0     2714 2024-04-03 07:17:55.368638 chat_cli_anything-0.1.5/chat_cli_anything/request.py
+-rw-r--r--   0        0        0      729 2024-03-31 17:35:50.217211 chat_cli_anything-0.1.5/chat_cli_anything/rerank.py
+-rw-r--r--   0        0        0     1868 2024-04-01 08:49:00.737620 chat_cli_anything-0.1.5/chat_cli_anything/service.py
+-rw-r--r--   0        0        0     1050 2024-04-02 06:30:30.360008 chat_cli_anything-0.1.5/chat_cli_anything/util.py
+-rw-r--r--   0        0        0     1466 2024-04-07 09:28:58.621285 chat_cli_anything-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     9464 1970-01-01 00:00:00.000000 chat_cli_anything-0.1.5/PKG-INFO
```

### Comparing `chat_cli_anything-0.1.4/LICENSE` & `chat_cli_anything-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `chat_cli_anything-0.1.4/README.md` & `chat_cli_anything-0.1.5/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -81,22 +81,22 @@
 Step 2: Ask a question
 
 ```
 # for open question, '-a/--advance' option would be helpful
 cc-ask -d d2light "DETR implementation" -a
 ```
 
-**Example 6**: Code review
+**Example 6**: Code explain
 
 ```
 # Explain line by line
-cc-code review /path/to/your/code.py -l
+cc-code explain /path/to/your/code.py -l
 
 # If the code is lengthy, continue generating
-cc-code review /path/to/your/code.py -l -c
+cc-code explain /path/to/your/code.py -l -c
 ```
 
 ## Command Explanation
 
 ### cc-config
 
 Configure LLM provider
@@ -245,66 +245,76 @@
 ```
 cc-code explain some_complex_scripts.py
 ```
 
 Example 2: Specify a particular function
 
 ```
-cc-code explain some_complex_scripts.py SomeClass::some_function
+cc-code explain some_complex_scripts.py -o SomeClass::some_function
 ```
 
 Example 3: Use pipe
 
 ```
 cat some_complex_scripts.py | cc-code explain
 ```
 
 #### Fix Issues
 
 ```
-cc-code fix [OPTIONS] [FILENAME] [OBJECT_NAME]
+```
+cc-code fix [OPTIONS] [FILENAME]
 
-Fix code.
+  Fix code.
 
 Options:
-  --help  Show this message and exit.
+  -o, --object-name TEXT
+  -c, --continue-generate
+  --help                   Show this message and exit.
+```
 ```
 
 #### Code Refactoring
 
 ```
-cc-code refactor [OPTIONS] [FILENAME] [OBJECT_NAME]
+cc-code refactor [OPTIONS] [FILENAME]
 
-Refactor code.
+  Refactor code.
 
 Options:
-  --help  Show this message and exit.
+  -o, --object-name TEXT
+  -c, --continue-generate
+  --help                   Show this message and exit.
 ```
 
 #### Code Review
 
 ```
-cc-code review [OPTIONS] [FILENAME] [OBJECT_NAME]
+cc-code review [OPTIONS] [FILENAME]
 
-Review code.
+  Review code.
 
 Options:
-  --help  Show this message and exit.
+  -o, --object-name TEXT
+  -c, --continue-generate
+  --help                   Show this message and exit.
 ```
 
 #### Code Translation
 
 ```
-cc-code translate [OPTIONS] [FILENAME] [OBJECT_NAME] LANGUAGE
+cc-code translate [OPTIONS] LANGUAGE [FILENAME]
 
-Translate code from one language to another. Supported languages include c++, cpp,
-c, rust, typescript, javascript, markdown, html.
+  Translate code from one language to another. Supported languages  c++, cpp,
+  c, rust, typescript, javascript, markdown, html.
 
 Options:
-  --help  Show this message and exit.
+  -o, --object-name TEXT
+  -c, --continue-generate
+  --help                   Show this message and exit.
 ```
 
 #### Select Code from Generated Results
 
 Used to select code snippets from the generated responses of the above commands.
 
 ```
@@ -410,8 +420,8 @@
 #### status:
 
 ```
 cc-service status [OPTIONS]
 
 Options:
   --help  Show this message and exit.
-```
+```
```

### Comparing `chat_cli_anything-0.1.4/chat_cli_anything/ask.py` & `chat_cli_anything-0.1.5/chat_cli_anything/ask.py`

 * *Files 3% similar despite different names*

```diff
@@ -82,21 +82,39 @@
                 self.last_query = self.history.get('last_query', '')
         else:
             self.diag_history = []
             self.last_output = '' 
             self.last_query = '' 
 
         self.pipeline_input = self._read_from_pipeline_input()
-        self.active_config = self.config['providers'][self.config['active']]
-        self.client = build_client(
-            self.active_config['base_url'],
-            self.active_config['api_key'],
-            self.active_config['proxy'],
-        )
+        if 'providers' in self.config and 'active' in self.config:
+                self.active_config = self.config['providers'][self.config['active']]
+                self.client = build_client(
+                    self.active_config['base_url'],
+                    self.active_config['api_key'],
+                    self.active_config['proxy'],
+                )
+    
+    def _check_providers(self):
+        if 'providers' not in self.config:
+            click.secho('No provider has been add.', fg='bright_red')
+            return False
+        return True
+
+    def _check_active_config(self):
+        if 'active' not in self.config:
+            click.secho('No provider has been set active.', fg='bright_red')
+            return False
+        return True
 
+    def check_active_config_exists(self):
+        """"""
+        if self._check_providers() and self._check_active_config():
+            return
+        sys.exit(1)
 
     def _read_from_pipeline_input(self):
         import sys
         # check whether there is a pipeline input
         lines: List[str] = []
         if not sys.stdin.isatty():
             # read data from pipeline
@@ -135,15 +153,15 @@
 
         if as_system:
             self.diag_history.insert(0, {'role': 'system', 'content': prompt})
         else:
             self.diag_history.append({'role': 'user', 'content': prompt})
 
     def load_file(self, filename: str):
-        from loader import SUPPORTED_FILES, load_file
+        from chat_cli_anything.loader import SUPPORTED_FILES, load_file
         ext = os.path.splitext(filename)
         if ext[1] and ext[1] in SUPPORTED_FILES: 
             pages = load_file(filename)
             content = ''.join(page.page_content for page in pages)
         else:
             click.secho(click.style('Not supported file extension. ' + f' currrent supported format: {",".join(SUPPORTED_FILES)}', fg='orange') + 'It will be loaded as plain text')
             with open(filename, 'r', encoding='utf-8') as f:
@@ -469,15 +487,15 @@
     config = Config()
     config.switch(name)
 
 
 @config.command()
 @click.argument('name', required=True)
 def ping(name: str):
-    """Switch to a different configuration and save the change."""
+    """Ping provider."""
     config = Config()
     config.ping(name)
 
 
 @config.command()
 @click.argument('path', required=True)
 @click.option('-o', '--override', is_flag=True, help='Whether override existing file.')
@@ -500,14 +518,16 @@
 @click.option('-f', '--filename', type=str, help='Name of file.')
 @click.option('-r', '--rerank', is_flag=True, default=False, help='Whether to rerank the results.')
 @click.option('-s', '--show-chunks', is_flag=True, help='Whether to show the related chunks retrieved from database.')
 @click.option('-a', '--advance', is_flag=True, help='Whether to use advance RAG.')
 def ask(query: str, db: Any, filename: str, rerank: bool, show_chunks: bool, advance: bool):
     """Start a chat session with the given query."""
     interface = Interface()
+    interface.check_active_config_exists()
+
     if db is not None:
         from chat_cli_anything.db import load_vectorstore
         _db = db
         status, db = load_vectorstore(db)
         if status:
             check_and_start_service()
         else:
@@ -527,14 +547,16 @@
          filename: str='',
          db: Any='',
          not_interactive: bool=False,
          show_history: bool=False,
          clear: bool=False):
     """Interactive chat. Enter '/quit' to exit"""
     interface = Interface()
+    interface.check_active_config_exists()
+
     if db is not None:
         from chat_cli_anything.db import load_vectorstore
         _db = db
         status, db = load_vectorstore(db)
         if status:
             check_and_start_service()
         else:
@@ -558,75 +580,86 @@
 @filename
 @object_name
 @continue_generate
 def refactor(filename: str, object_name: str, continue_generate: bool):
     """Refactor code."""
     check_has_context(filename)
     interface = Interface()
+    interface.check_active_config_exists()
+
     interface.refactor(filename, object_name, continue_generate)
 
 
 @code.command()
 @click.argument('language')
 @filename
 @object_name
 @continue_generate
 def translate(filename: str, object_name: str, language: str, continue_generate: bool):
     """Translate code from one language to another. Supported languages 
     c++, cpp, c, rust, typescript, javascript, markdown, html.
     """
     check_has_context(filename)
     interface = Interface()
+    interface.check_active_config_exists()
+
     interface.translate(filename, object_name, language, continue_generate)
 
 
 @code.command()
 @filename
 @object_name
 @continue_generate
 def fix(filename: str, object_name: str, continue_generate: bool):
     """Fix code."""
     check_has_context(filename)
     interface = Interface()
+    interface.check_active_config_exists()
+
     interface.fix(filename, object_name, continue_generate)
 
 
 @code.command()
 @filename
 @object_name
 @continue_generate
 def review(filename: str, object_name: str, continue_generate: bool):
     """Review code."""
     check_has_context(filename)
     interface = Interface()
+    interface.check_active_config_exists()
+
     interface.review(filename, object_name, continue_generate)
 
 
 @code.command()
 @filename
 @object_name
 @click.option('-l', '--line', is_flag=True, help='Line by line.')
 @continue_generate
 def explain(filename: str, object_name: str, line: bool, continue_generate: bool):
     """Explain code."""
     check_has_context(filename)
     interface = Interface()
+    interface.check_active_config_exists()
+
     interface.explain(filename, object_name, line_by_line=line, continue_generate=continue_generate)
 
 
 @code.command()
 @click.argument('index', required=False, default='')
 @click.option('-c', '--count', is_flag=True, help='get number of code snippets')
 def select(index: str, count: bool):
     """Select code snippet from last output.
 
     Argument:
         index: code snippet index
     """
     interface = Interface()
+
     interface.select_code_snippet(index, count)
 
 
 @db.command(name='ingest')
 @click.argument('files', nargs=-1)
 @click.option('-n', '--name', help='The name of the knowledge base.')
 @click.option('-m', '--comment', default='', help='Add comment to info')
```

### Comparing `chat_cli_anything-0.1.4/chat_cli_anything/config.py` & `chat_cli_anything-0.1.5/chat_cli_anything/config.py`

 * *Files identical despite different names*

### Comparing `chat_cli_anything-0.1.4/chat_cli_anything/db.py` & `chat_cli_anything-0.1.5/chat_cli_anything/db.py`

 * *Files identical despite different names*

### Comparing `chat_cli_anything-0.1.4/chat_cli_anything/embedding.py` & `chat_cli_anything-0.1.5/chat_cli_anything/embedding.py`

 * *Files identical despite different names*

### Comparing `chat_cli_anything-0.1.4/chat_cli_anything/loader.py` & `chat_cli_anything-0.1.5/chat_cli_anything/loader.py`

 * *Files identical despite different names*

### Comparing `chat_cli_anything-0.1.4/chat_cli_anything/request.py` & `chat_cli_anything-0.1.5/chat_cli_anything/request.py`

 * *Files identical despite different names*

### Comparing `chat_cli_anything-0.1.4/chat_cli_anything/rerank.py` & `chat_cli_anything-0.1.5/chat_cli_anything/rerank.py`

 * *Files identical despite different names*

### Comparing `chat_cli_anything-0.1.4/chat_cli_anything/service.py` & `chat_cli_anything-0.1.5/chat_cli_anything/service.py`

 * *Files identical despite different names*

### Comparing `chat_cli_anything-0.1.4/chat_cli_anything/util.py` & `chat_cli_anything-0.1.5/chat_cli_anything/util.py`

 * *Files identical despite different names*

### Comparing `chat_cli_anything-0.1.4/pyproject.toml` & `chat_cli_anything-0.1.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "chat-cli-anything"
-version = "0.1.4"
+version = "0.1.5"
 description = "Chat with anything on cli."
 authors = ["liuping <liuping@shukun.net>"]
 license = "Apache"
 readme = "README.md"
 keywords = ["chatgpt", "cli", "chat"]
 packages = [{ include = "chat_cli_anything" }]
 
@@ -21,15 +21,15 @@
 tabulate = "^0.9.0"
 rich = "^13.7.1"
 langchain-core = "^0.1.36"
 uvicorn = "^0.29.0"
 langchain-community = {version = "^0.0.29", optional = true}
 langchain = {version = "^0.1.13", optional = true}
 flagembedding = {version = "^1.2.8", optional = true}
-torch = {version = "^2.2.2", optional = true}
+torch = {version = ">=2.1.0", optional = true}
 langchain-openai = {version = "^0.1.1", optional = true}
 langchain-text-splitters = {version = "^0.0.1", optional = true}
 tiktoken = "^0.6.0"
 tqdm = "^4.66.2"
 
 [tool.poetry.group.dev.dependencies]
 openai = "^1.13.3"
```

### Comparing `chat_cli_anything-0.1.4/PKG-INFO` & `chat_cli_anything-0.1.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chat-cli-anything
-Version: 0.1.4
+Version: 0.1.5
 Summary: Chat with anything on cli.
 License: Apache
 Keywords: chatgpt,cli,chat
 Author: liuping
 Author-email: liuping@shukun.net
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
@@ -26,15 +26,15 @@
 Requires-Dist: openai (>=1.13.3,<2.0.0)
 Requires-Dist: psutil (>=5.9.8,<6.0.0)
 Requires-Dist: pypdf (>=4.1.0,<5.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: rich (>=13.7.1,<14.0.0)
 Requires-Dist: tabulate (>=0.9.0,<0.10.0)
 Requires-Dist: tiktoken (>=0.6.0,<0.7.0)
-Requires-Dist: torch (>=2.2.2,<3.0.0) ; extra == "all"
+Requires-Dist: torch (>=2.1.0) ; extra == "all"
 Requires-Dist: tqdm (>=4.66.2,<5.0.0)
 Requires-Dist: uvicorn (>=0.29.0,<0.30.0)
 Requires-Dist: xonsh (>=0.15.1,<0.16.0)
 Description-Content-Type: text/markdown
 
 ![chat-cli-anything](./logo.png)
 
@@ -119,22 +119,22 @@
 Step 2: Ask a question
 
 ```
 # for open question, '-a/--advance' option would be helpful
 cc-ask -d d2light "DETR implementation" -a
 ```
 
-**Example 6**: Code review
+**Example 6**: Code explain
 
 ```
 # Explain line by line
-cc-code review /path/to/your/code.py -l
+cc-code explain /path/to/your/code.py -l
 
 # If the code is lengthy, continue generating
-cc-code review /path/to/your/code.py -l -c
+cc-code explain /path/to/your/code.py -l -c
 ```
 
 ## Command Explanation
 
 ### cc-config
 
 Configure LLM provider
@@ -283,66 +283,76 @@
 ```
 cc-code explain some_complex_scripts.py
 ```
 
 Example 2: Specify a particular function
 
 ```
-cc-code explain some_complex_scripts.py SomeClass::some_function
+cc-code explain some_complex_scripts.py -o SomeClass::some_function
 ```
 
 Example 3: Use pipe
 
 ```
 cat some_complex_scripts.py | cc-code explain
 ```
 
 #### Fix Issues
 
 ```
-cc-code fix [OPTIONS] [FILENAME] [OBJECT_NAME]
+```
+cc-code fix [OPTIONS] [FILENAME]
 
-Fix code.
+  Fix code.
 
 Options:
-  --help  Show this message and exit.
+  -o, --object-name TEXT
+  -c, --continue-generate
+  --help                   Show this message and exit.
+```
 ```
 
 #### Code Refactoring
 
 ```
-cc-code refactor [OPTIONS] [FILENAME] [OBJECT_NAME]
+cc-code refactor [OPTIONS] [FILENAME]
 
-Refactor code.
+  Refactor code.
 
 Options:
-  --help  Show this message and exit.
+  -o, --object-name TEXT
+  -c, --continue-generate
+  --help                   Show this message and exit.
 ```
 
 #### Code Review
 
 ```
-cc-code review [OPTIONS] [FILENAME] [OBJECT_NAME]
+cc-code review [OPTIONS] [FILENAME]
 
-Review code.
+  Review code.
 
 Options:
-  --help  Show this message and exit.
+  -o, --object-name TEXT
+  -c, --continue-generate
+  --help                   Show this message and exit.
 ```
 
 #### Code Translation
 
 ```
-cc-code translate [OPTIONS] [FILENAME] [OBJECT_NAME] LANGUAGE
+cc-code translate [OPTIONS] LANGUAGE [FILENAME]
 
-Translate code from one language to another. Supported languages include c++, cpp,
-c, rust, typescript, javascript, markdown, html.
+  Translate code from one language to another. Supported languages  c++, cpp,
+  c, rust, typescript, javascript, markdown, html.
 
 Options:
-  --help  Show this message and exit.
+  -o, --object-name TEXT
+  -c, --continue-generate
+  --help                   Show this message and exit.
 ```
 
 #### Select Code from Generated Results
 
 Used to select code snippets from the generated responses of the above commands.
 
 ```
@@ -449,7 +459,8 @@
 
 ```
 cc-service status [OPTIONS]
 
 Options:
   --help  Show this message and exit.
 ```
+
```

