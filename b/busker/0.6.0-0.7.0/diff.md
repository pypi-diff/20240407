# Comparing `tmp/busker-0.6.0.tar.gz` & `tmp/busker-0.7.0.tar.gz`

## Comparing `busker-0.6.0.tar` & `busker-0.7.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 busker-0.6.0/CHANGELOG.md
--rw-r--r--   0        0        0    49152 2020-02-02 00:00:00.000000 busker-0.6.0/busker/.gui.py.swp
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 busker-0.6.0/busker/__init__.py
--rw-r--r--   0        0        0     7127 2020-02-02 00:00:00.000000 busker-0.6.0/busker/executive.py
--rw-r--r--   0        0        0    19607 2020-02-02 00:00:00.000000 busker-0.6.0/busker/gui.py
--rw-r--r--   0        0        0     3373 2020-02-02 00:00:00.000000 busker-0.6.0/busker/history.py
--rw-r--r--   0        0        0     3548 2020-02-02 00:00:00.000000 busker-0.6.0/busker/main.py
--rw-r--r--   0        0        0     6730 2020-02-02 00:00:00.000000 busker-0.6.0/busker/runner.py
--rw-r--r--   0        0        0     4635 2020-02-02 00:00:00.000000 busker-0.6.0/busker/scraper.py
--rw-r--r--   0        0        0     1367 2020-02-02 00:00:00.000000 busker-0.6.0/busker/tagger.py
--rw-r--r--   0        0        0     1419 2020-02-02 00:00:00.000000 busker-0.6.0/busker/types.py
--rw-r--r--   0        0        0     5702 2020-02-02 00:00:00.000000 busker-0.6.0/busker/visitor.py
--rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 busker-0.6.0/busker/zone.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 busker-0.6.0/busker/test/__init__.py
--rw-r--r--   0        0        0     2271 2020-02-02 00:00:00.000000 busker-0.6.0/busker/test/test_executive.py
--rw-r--r--   0        0        0     2438 2020-02-02 00:00:00.000000 busker-0.6.0/busker/test/test_history.py
--rw-r--r--   0        0        0     2779 2020-02-02 00:00:00.000000 busker-0.6.0/busker/test/test_runner.py
--rw-r--r--   0        0        0     6933 2020-02-02 00:00:00.000000 busker-0.6.0/busker/test/test_scraper.py
--rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 busker-0.6.0/busker/test/test_zone.py
--rw-r--r--   0        0        0    35141 2020-02-02 00:00:00.000000 busker-0.6.0/LICENSE
--rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 busker-0.6.0/README.md
--rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 busker-0.6.0/pyproject.toml
--rw-r--r--   0        0        0    42031 2020-02-02 00:00:00.000000 busker-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 busker-0.7.0/CHANGELOG.md
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 busker-0.7.0/busker/__init__.py
+-rw-r--r--   0        0        0     7127 2020-02-02 00:00:00.000000 busker-0.7.0/busker/executive.py
+-rw-r--r--   0        0        0    20767 2020-02-02 00:00:00.000000 busker-0.7.0/busker/gui.py
+-rw-r--r--   0        0        0     3373 2020-02-02 00:00:00.000000 busker-0.7.0/busker/history.py
+-rw-r--r--   0        0        0     3641 2020-02-02 00:00:00.000000 busker-0.7.0/busker/main.py
+-rw-r--r--   0        0        0     6774 2020-02-02 00:00:00.000000 busker-0.7.0/busker/runner.py
+-rw-r--r--   0        0        0     4648 2020-02-02 00:00:00.000000 busker-0.7.0/busker/scraper.py
+-rw-r--r--   0        0        0     4324 2020-02-02 00:00:00.000000 busker-0.7.0/busker/tagger.py
+-rw-r--r--   0        0        0     1419 2020-02-02 00:00:00.000000 busker-0.7.0/busker/types.py
+-rw-r--r--   0        0        0     5867 2020-02-02 00:00:00.000000 busker-0.7.0/busker/visitor.py
+-rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 busker-0.7.0/busker/zone.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 busker-0.7.0/busker/test/__init__.py
+-rw-r--r--   0        0        0     2271 2020-02-02 00:00:00.000000 busker-0.7.0/busker/test/test_executive.py
+-rw-r--r--   0        0        0     2438 2020-02-02 00:00:00.000000 busker-0.7.0/busker/test/test_history.py
+-rw-r--r--   0        0        0     2779 2020-02-02 00:00:00.000000 busker-0.7.0/busker/test/test_runner.py
+-rw-r--r--   0        0        0     7241 2020-02-02 00:00:00.000000 busker-0.7.0/busker/test/test_scraper.py
+-rw-r--r--   0        0        0     2904 2020-02-02 00:00:00.000000 busker-0.7.0/busker/test/test_tagger.py
+-rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 busker-0.7.0/busker/test/test_zone.py
+-rw-r--r--   0        0        0    35141 2020-02-02 00:00:00.000000 busker-0.7.0/LICENSE
+-rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 busker-0.7.0/README.md
+-rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 busker-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0    42031 2020-02-02 00:00:00.000000 busker-0.7.0/PKG-INFO
```

### Comparing `busker-0.6.0/busker/executive.py` & `busker-0.7.0/busker/executive.py`

 * *Files identical despite different names*

### Comparing `busker-0.6.0/busker/gui.py` & `busker-0.7.0/busker/gui.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,20 +20,22 @@
 from collections import defaultdict
 from collections import deque
 import concurrent.futures
 import enum
 import importlib.metadata
 import logging
 import multiprocessing.context
+import os
 import pathlib
 import queue
 import subprocess
 import tempfile
 import tkinter as tk
 from tkinter import filedialog
+from tkinter import messagebox
 from tkinter import ttk
 from types import SimpleNamespace as Structure
 import sys
 import urllib.error
 import urllib.parse
 import venv
 
@@ -87,75 +89,84 @@
             self.log(f"{e!s}", level=logging.WARNING)
             return
         else:
             info.configure(text=node.text.strip())
 
         reader = busker.visitor.Read(url=host)
         node = reader.run(self.scraper)
-        writer = busker.visitor.Write(url=host, prior=node, choice=Choice(form=0))
+        writer = busker.visitor.Write(url=host, prior=node, choice=Choice(form="ballad-form-start"))
         self.registry["Transcript"].process_node(writer.run(self.scraper))
 
+
 class InteractiveZone(Zone):
 
     def __init__(self, parent, name="", **kwargs):
         self.assist = tk.BooleanVar(value=False)
         super().__init__(parent, name=name, **kwargs)
         self.scraper = Scraper()
         self.node = None
+        self.do_display()
 
     def build(self, frame: ttk.Frame):
         frame.rowconfigure(0, weight=30)
         frame.rowconfigure(1, weight=1)
         frame.columnconfigure(0, weight=1)
 
-        text_widget = tk.Text(frame, height=6)
+        text_widget = Tagger.configure(tk.Text(frame, height=6))
         scroll_bar = ttk.Scrollbar(frame, orient=tk.VERTICAL, command=text_widget.yview)
         text_widget.configure(yscrollcommand=scroll_bar.set)
-        text_widget.tag_configure("cite", background="yellow", font="TkFixedFont", relief="raised")
 
         yield "text", self.grid(text_widget, row=0, column=0, columnspan=3, padx=(10, 10), sticky=tk.W + tk.N + tk.E + tk.S)
         yield "scroll", self.grid(scroll_bar, row=0, column=3, pady=(10, 10), sticky=tk.N + tk.S)
 
         combo_box = ttk.Combobox(frame, justify=tk.LEFT)
         yield "entry", self.grid(
             combo_box, row=1, column=0,
             padx=(10, 10), pady=(2, 6), ipadx=6,
             sticky=tk.W + tk.N + tk.E + tk.S
         )
         combo_box.bind("<Return>", self.on_entry)
 
         yield "toggle", self.grid(
-            ttk.Checkbutton(frame, variable=self.assist, offvalue=False, onvalue=True),
+            ttk.Checkbutton(frame, variable=self.assist, offvalue=False, onvalue=True, command=self.do_display),
             row=1, column=1, padx=(10, 10), sticky=tk.W + tk.E
         )
         yield "label", self.grid(ttk.Label(frame, text="Assist"), row=1, column=2, columnspan=3, padx=(10, 10))
 
     def process_node(self, node: Node):
+        self.node = node
         tagger = Tagger(self.controls.text[0])
         for block in node.blocks:
             tagger.feed(block)
 
+    def do_display(self):
         if self.assist.get():
-            self.controls.entry[0].configure(values=node.options)
-        self.node = node
+            Tagger.show(self.controls.text[0], "cue")
+            if self.node:
+                self.controls.entry[0].configure(values=self.node.options)
+        else:
+            Tagger.hide(self.controls.text[0], "cue")
+            self.controls.entry[0].configure(values=[])
 
     def on_entry(self, evt):
         value = self.controls.entry[0].get().strip()
         writer = busker.visitor.Write(
             url=self.node.url,
             prior=self.node,
-            choice=Choice(form=0, input=0, value=value)
+            choice=Choice(form="ballad-command-form", input="ballad-command-form-input-text", value=value)
         )
         self.controls.entry[0].delete(0, tk.END)
-        self.controls.text[0].insert(tk.END, "> ", ("prompt"))
-        self.controls.text[0].insert(tk.END, f"{value}\n", ("command"))
+
+        Tagger.display_command(self.controls.text[0], cmd=value)
         try:
             self.process_node(writer.run(self.scraper))
         except urllib.error.HTTPError:
-            self.controls.text[0].insert(tk.END, "...\n", ("nudge"))
+            Tagger.display_message(self.controls.text[0])
+        finally:
+            self.do_display()
 
 
 class EnvironmentZone(Zone):
 
     def __init__(self, parent, name="", **kwargs):
         super().__init__(parent, name=name, **kwargs)
         self.executive = Executive()
@@ -180,20 +191,25 @@
 
         yield "button", self.grid(
             tk.Button(frame, text="Build", command=self.on_build),
             row=0, column=3, columnspan=2, padx=(10, 10), sticky=tk.W + tk.E
         )
 
     def on_select(self):
-        path = pathlib.Path(filedialog.askdirectory(
+        choice = filedialog.askdirectory(
             parent=self.frame,
             title="Select virtual environment",
             initialdir=pathlib.Path.cwd(),
             mustexist=True,
-        ))
+        )
+        if not choice:
+            return
+        else:
+            path = pathlib.Path(choice)
+
         if not self.executive.venv_cfg(path) and not path.name.startswith("busker_"):
             path = pathlib.Path(tempfile.mkdtemp(prefix="busker_", suffix="_venv", dir=path))
         self.controls.entry[0].delete(0, tk.END)
         self.controls.entry[0].insert(0, str(path))
         self.location = path
 
     def on_build(self):
@@ -299,14 +315,15 @@
         text_widget.see(tk.END)
 
         try:
             msg = runner.exenv.queue.get(block=False)
             if isinstance(msg, list):
                 msg = [str(i) for i in msg]
             text_widget.insert(tk.END, f"Runner: {msg}\n")
+            text_widget.see(tk.END)
         except queue.Empty:
             pass
 
         if runner.proc.poll() is None:
             self.frame.after(100, self.update_progress, runner)
         else:
             self.install_complete(runner)
@@ -328,22 +345,24 @@
         name = package_path.name.removesuffix("".join(package_path.suffixes))
         values = runner.sort_entry_points(entry_points, like=name)
 
         entry_widget = self.registry["Server"].controls.entry[0]
         entry_widget.configure(values=values)
         entry_widget.current(0)
         self.registry["Server"].controls.button[1]["state"] = tk.NORMAL
+        proc.terminate()
 
 
 class ServerZone(Zone):
 
     def __init__(self, parent, name="", **kwargs):
         super().__init__(parent, name=name, **kwargs)
         self.executive = Executive()
         self.running = None
+        parent._root().protocol('WM_DELETE_WINDOW', self.on_window)
 
     def build(self, frame: ttk.Frame):
         frame.rowconfigure(0, weight=1)
         frame.columnconfigure(0, minsize=12)
         frame.columnconfigure(1, weight=1)
         frame.columnconfigure(6, uniform="button")
         frame.columnconfigure(7, uniform="button")
@@ -371,60 +390,79 @@
             ),
             self.grid(
                 tk.Button(frame, text="Start", command=self.on_start),
                 row=0, column=7, padx=(10, 10), pady=(10, 10), sticky=tk.W + tk.E
             ),
         ]
         for button in buttons:
-            button["state"] = tk.DISABLED
+            # button["state"] = tk.DISABLED
             yield "button", button
 
+    def on_window(self):
+        if not self.running:
+            self.parent._root().destroy()
+        elif messagebox.askokcancel("Quit", "Quitting now will stop the server."):
+            self.on_stop()
+            self.parent._root().destroy()
+
     def on_stop(self):
-        if self.running:
-            self.running.terminate()
+        text_widget = self.registry["Output"].controls.text[0]
         self.controls.button[0]["state"] = tk.DISABLED
         self.controls.button[1]["state"] = tk.NORMAL
 
+        if self.running:
+            self.running.terminate()
+            text_widget.insert(tk.END, f"Server process terminated.\n")
+            text_widget.see(tk.END)
+            self.running = None
+
     def on_start(self):
+        text_widget = self.registry["Output"].controls.text[0]
         self.controls.button[0]["state"] = tk.NORMAL
         self.controls.button[1]["state"] = tk.DISABLED
 
         entry_point = self.controls.entry[0].get()
         host = self.controls.entry[1].get().strip()
         port = self.controls.entry[2].get()
+        text_widget.insert(tk.END, f"Starting {entry_point} on {host}:{port}.\n")
+        text_widget.see(tk.END)
 
         runner = Server(entry_point, host=host, port=port)
         self.running = next(self.executive.run(runner, interpreter=self.executive.active.interpreter))
+
         self.registry["Info"].controls.entry[0].delete(0, tk.END)
         self.registry["Info"].controls.entry[0].insert(0, runner.url)
-        self.registry["Output"].controls.text[0].insert(tk.END, f"Server process running.\n")
+        text_widget.insert(tk.END, f"Server process running.\n")
+        text_widget.see(tk.END)
+
+        os.set_blocking(self.running.stdout.fileno(), False)
+        os.set_blocking(self.running.stderr.fileno(), False)
         self.update_progress(runner)
 
     def update_progress(self, runner: Runner):
         text_widget = self.registry["Output"].controls.text[0]
 
         try:
             msg = runner.exenv.queue.get(block=False)
             if isinstance(msg, list):
                 msg = [str(i) for i in msg]
             text_widget.insert(tk.END, f"Runner: {msg}\n")
+            text_widget.see(tk.END)
         except queue.Empty:
             pass
 
-        try:
-            out, err = runner.proc.communicate(timeout=0.1)
-        except subprocess.TimeoutExpired:
+        for line in runner.proc.stdout:
+            text_widget.insert(tk.END, line)
+            text_widget.see(tk.END)
+        for line in runner.proc.stderr:
+            text_widget.insert(tk.END, line)
+            text_widget.see(tk.END)
+
+        if runner.proc.poll() is None:
             self.frame.after(100, self.update_progress, runner)
-        else:
-            for line in out.splitlines(keepends=True):
-                text_widget.insert(tk.END, line)
-                text_widget.see(tk.END)
-            for line in err.splitlines(keepends=True):
-                text_widget.insert(tk.END, line)
-                text_widget.see(tk.END)
 
 
 class OutputZone(Zone):
 
     def build(self, frame: ttk.Frame):
         frame.rowconfigure(0, weight=1)
         frame.columnconfigure(0, weight=30)
```

### Comparing `busker-0.6.0/busker/history.py` & `busker-0.7.0/busker/history.py`

 * *Files identical despite different names*

### Comparing `busker-0.6.0/busker/main.py` & `busker-0.7.0/busker/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -39,14 +39,36 @@
 )
 
 
 def main(args):
     history = SharedHistory(log_name="busker")
     history.log(f"Busker {busker.__version__}")
 
+    if args.with_automation:
+        witness = Counter()
+
+        n = 0
+        while n < args.number:
+            n += 1
+            history.log(f"Run: {n:03d}")
+            visitor = Visitor(args.url)
+            while visitor.tactics:
+                tactic = visitor.tactics.popleft()
+                node = visitor(tactic)
+                if node:
+                    history.log(f"Page: {node.title}")
+
+            witness[visitor.turns] += 1
+
+        history.log(f"{visitor.turns} done.")
+
+        print(*visitor.toml_lines(visitor.history), sep="\n")
+        print({k: witness[k] for k in sorted(witness.keys())})
+        return 0
+
     try:
         text = args.config.read_text()
         config = tomllib.loads(text)
     except FileNotFoundError:
         config = {}
     except tomllib.TOMLDecodeError as e:
         history.log(f"Error reading config file at {args.config}", level=logging.WARNING)
@@ -54,35 +76,14 @@
         return 2
 
     exclude = [] if args.with_automation else ["automation"]
     root = busker.gui.build(config, exclude=exclude)
     root.mainloop()
     return 0
 
-    witness = Counter()
-
-    n = 0
-    while n < args.number:
-        n += 1
-        history.log(f"Run: {n:03d}")
-        visitor = Visitor(args.url)
-        while visitor.tactics:
-            tactic = visitor.tactics.popleft()
-            node = visitor(tactic)
-            if node:
-                history.log(f"Page: {node.title}")
-
-        witness[visitor.turns] += 1
-
-    history.log(f"{visitor.turns} done.")
-
-    print(*visitor.toml_lines(visitor.history), sep="\n")
-    print({k: witness[k] for k in sorted(witness.keys())})
-    return 0
-
 
 def parser(defaults):
     rv = argparse.ArgumentParser(fromfile_prefix_chars="@")
 
     display_options = rv.add_argument_group("Display")
     packaging_options = rv.add_argument_group("Packaging")
     automation_options = rv.add_argument_group("Automation")
```

### Comparing `busker-0.6.0/busker/runner.py` & `busker-0.7.0/busker/runner.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,15 +98,15 @@
     def pip_command_args(
         interpreter: pathlib.Path,
         distribution: pathlib.Path,
         dependencies: list = ["test"],
         update=False,
     ) -> list[str]:
         specification = f"{distribution}" + ("[{0}]".format(",".join(dependencies)) if dependencies else "")
-        rv = [interpreter, "-m", "pip", "install", specification]
+        rv = [interpreter, "-m", "pip", "install", "--upgrade", "--upgrade-strategy", "eager", specification]
         if update:
             rv.insert(4, "--upgrade")
         return rv
 
     def __init__(self, distribution: pathlib.Path, read_interval: int = 0.5):
         super().__init__()
         self.distribution = distribution
```

### Comparing `busker-0.6.0/busker/scraper.py` & `busker-0.7.0/busker/scraper.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,31 +82,31 @@
 
 
 class Scraper(SharedHistory):
 
     @staticmethod
     @functools.cache
     def tag_matcher(tag: str):
-        return re.compile(f"<{tag}.*?>(.*?)<\\/{tag}>", re.DOTALL)
+        return re.compile(f"(<{tag}.*?>)(.*?)(<\\/{tag}>)", re.DOTALL)
 
     @staticmethod
     def find_forms(body: str):
         root = ET.fromstring(body)
         return root.findall(".//form")
 
     @staticmethod
     def find_blocks(body: str):
         matcher = Scraper.tag_matcher("blockquote")
-        return [i.strip() for i in matcher.findall(body, re.DOTALL)]
+        return ["".join(i).strip() for i in matcher.findall(body, re.DOTALL)]
 
     @staticmethod
     def find_title(doc: str):
         matcher = Scraper.tag_matcher("title")
         match = matcher.search(doc)
-        return match and match[1]
+        return match and match[2]
 
     def get_forms(self, body: str):
         root = ET.fromstring(body)
         for form_node in root.findall(".//form"):
             inputs = tuple(
                 Input(**dict(
                     {k: v for k, v in node.attrib.items() if k in Input._fields},
```

### Comparing `busker-0.6.0/busker/types.py` & `busker-0.7.0/busker/types.py`

 * *Files identical despite different names*

### Comparing `busker-0.6.0/busker/visitor.py` & `busker-0.7.0/busker/visitor.py`

 * *Files 7% similar despite different names*

```diff
@@ -59,49 +59,50 @@
         url = self.prior.url if self.prior else self.url
         node = scraper.get(url, **kwargs)
 
         body_re = scraper.tag_matcher("body")
         body_match = body_re.search(node.text)
 
         title_match = scraper.find_title(node.text)
-        forms = body_match and tuple(scraper.get_forms(body_match[0])) or []
-        blocks = body_match and tuple(scraper.find_blocks(body_match[0])) or []
+        forms = body_match and tuple(scraper.get_forms(body_match[0])) or tuple()
+        blocks = body_match and tuple(scraper.find_blocks(body_match[0])) or tuple()
 
         return node._replace(
             tactic=self.__class__.__name__,
             params=tuple(kwargs.items()),
             title=title_match and title_match.group(),
             blocks=blocks,
             options=tuple(v for f in forms for i in f.inputs for v in i.values),
             actions=forms,
         )
         return node
 
 
 class Write(Tactic):
     def run(self, scraper: Scraper, **kwargs) -> Node:
-        form = self.prior.actions[self.choice.form]
+        form = {i.name: i for i in self.prior.actions}.get(self.choice.form, next(iter(self.prior.actions)))
         if form and form.method.lower() == "post":
             parts = urllib.parse.urlparse(form.action)
             if not parts.scheme:
                 parts = urllib.parse.urlparse(f"{self.prior.url}{form.action}")
             self.url = urllib.parse.urlunparse(parts)
 
             if self.choice.input is None:
                 data = dict()
             else:
-                data = {form.inputs[self.choice.input].name: self.choice.value}
+                input_ = {i.name: i for i in form.inputs}.get(self.choice.input, next(iter(form.inputs)))
+                data = {input_.name: self.choice.value}
 
             rv = scraper.post(self.url, data)
 
             body_re = scraper.tag_matcher("body")
             body_match = body_re.search(rv.text)
 
-            forms = body_match and tuple(scraper.get_forms(body_match[0]))
-            blocks = body_match and tuple(scraper.find_blocks(body_match[0])) or []
+            forms = body_match and tuple(scraper.get_forms(body_match[0])) or tuple()
+            blocks = body_match and tuple(scraper.find_blocks(body_match[0])) or tuple()
 
             rv = rv._replace(
                 tactic=self.__class__.__name__,
                 params=tuple(kwargs.items()),
                 title = scraper.find_title(rv.text),
                 blocks=blocks,
                 options=tuple(v for f in forms for i in f.inputs for v in i.values),
```

### Comparing `busker-0.6.0/busker/zone.py` & `busker-0.7.0/busker/zone.py`

 * *Files identical despite different names*

### Comparing `busker-0.6.0/busker/test/test_executive.py` & `busker-0.7.0/busker/test/test_executive.py`

 * *Files identical despite different names*

### Comparing `busker-0.6.0/busker/test/test_history.py` & `busker-0.7.0/busker/test/test_history.py`

 * *Files identical despite different names*

### Comparing `busker-0.6.0/busker/test/test_runner.py` & `busker-0.7.0/busker/test/test_runner.py`

 * *Files identical despite different names*

### Comparing `busker-0.6.0/busker/test/test_scraper.py` & `busker-0.7.0/busker/test/test_scraper.py`

 * *Files 3% similar despite different names*

```diff
@@ -166,14 +166,21 @@
             with self.subTest(n=n, text=text):
                 title = scraper.find_title(text)
                 if n == 0:
                     self.assertIsNone(title)
                 else:
                     self.assertEqual(title, "Story", title)
 
+    def test_find_blocks(self):
+        scraper = Scraper()
+        blocks = scraper.find_blocks(self.fixtures.Session)
+        self.assertEqual(len(blocks), 2)
+        self.assertTrue(all(i.startswith("<blockquote") for i in blocks))
+        self.assertTrue(all(i.endswith("blockquote>") for i in blocks))
+
     def test_get_forms_from_session(self):
         scraper = Scraper()
         for n, text in enumerate((self.fixtures.Home, self.fixtures.Session)):
             with self.subTest(n=n, text=text):
                 body_re = scraper.tag_matcher("body")
                 match = body_re.search(text)
                 form = next(scraper.get_forms(match[0]), None)
```

### Comparing `busker-0.6.0/busker/test/test_zone.py` & `busker-0.7.0/busker/test/test_zone.py`

 * *Files identical despite different names*

### Comparing `busker-0.6.0/LICENSE` & `busker-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `busker-0.6.0/README.md` & `busker-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `busker-0.6.0/pyproject.toml` & `busker-0.7.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # For possible options see https://peps.python.org/pep-0621/
  
 [project]
 name = "busker"
-version = "0.6.0"
+version = "0.7.0"
 description = "A utility for testing Balladeer projects."
 readme = "README.md"
 requires-python = ">=3.11"
 license = {file = "LICENSE"}
 keywords = ["interactive fiction", "balladeer"]
 authors = [
     {name = "D E Haynes", email = "tundish@gigeconomy.org.uk"}
@@ -29,15 +29,24 @@
 busker-cli = "busker.main:run"
 
 [build-system]
 # requires = ["hatchling == 1.21.1"]
 requires = ["hatchling >= 1.22.4"]
 build-backend = "hatchling.build"
 
-[tool.hatch.build]
+[tool.hatch.build.targets.sdist]
+include = [
+"*.md",
+"busker/*",
+]
+exclude = [
+"busker_*",
+]
+
+[tool.hatch.build.targets.wheel]
 include = [
 "*.md",
 "busker/*",
 ]
 exclude = [
 "busker_*",
 ]
```

### Comparing `busker-0.6.0/PKG-INFO` & `busker-0.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: busker
-Version: 0.6.0
+Version: 0.7.0
 Summary: A utility for testing Balladeer projects.
 Author-email: D E Haynes <tundish@gigeconomy.org.uk>
 Maintainer-email: Tundish <tundish@gigeconomy.org.uk>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
```

