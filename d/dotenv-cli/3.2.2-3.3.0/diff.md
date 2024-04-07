# Comparing `tmp/dotenv-cli-3.2.2.tar.gz` & `tmp/dotenv-cli-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dotenv-cli-3.2.2.tar", last modified: Fri Nov 10 20:44:47 2023, max compression
+gzip compressed data, was "dotenv-cli-3.3.0.tar", last modified: Sun Apr  7 12:55:48 2024, max compression
```

## Comparing `dotenv-cli-3.2.2.tar` & `dotenv-cli-3.3.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 venthur   (1000) venthur   (1000)        0 2023-11-10 20:44:47.462503 dotenv-cli-3.2.2/
--rw-r--r--   0 venthur   (1000) venthur   (1000)     1072 2018-10-14 16:13:37.000000 dotenv-cli-3.2.2/LICENSE
--rw-r--r--   0 venthur   (1000) venthur   (1000)       31 2019-04-28 11:56:54.000000 dotenv-cli-3.2.2/MANIFEST.in
--rw-r--r--   0 venthur   (1000) venthur   (1000)     4430 2023-11-10 20:44:47.462503 dotenv-cli-3.2.2/PKG-INFO
--rw-r--r--   0 venthur   (1000) venthur   (1000)     2347 2019-08-03 12:37:48.000000 dotenv-cli-3.2.2/README.md
-drwxr-xr-x   0 venthur   (1000) venthur   (1000)        0 2023-11-10 20:44:47.458503 dotenv-cli-3.2.2/completion/
-drwxr-xr-x   0 venthur   (1000) venthur   (1000)        0 2023-11-10 20:44:47.458503 dotenv-cli-3.2.2/completion/bash/
--rw-r--r--   0 venthur   (1000) venthur   (1000)      869 2019-04-28 11:56:54.000000 dotenv-cli-3.2.2/completion/bash/dotenv
-drwxr-xr-x   0 venthur   (1000) venthur   (1000)        0 2023-11-10 20:44:47.458503 dotenv-cli-3.2.2/dotenv_cli/
--rw-r--r--   0 venthur   (1000) venthur   (1000)       66 2023-07-01 11:21:02.000000 dotenv-cli-3.2.2/dotenv_cli/__init__.py
--rw-r--r--   0 venthur   (1000) venthur   (1000)     1248 2023-11-10 20:11:32.000000 dotenv-cli-3.2.2/dotenv_cli/cli.py
--rw-r--r--   0 venthur   (1000) venthur   (1000)     3121 2023-11-10 20:11:32.000000 dotenv-cli-3.2.2/dotenv_cli/core.py
--rw-r--r--   0 venthur   (1000) venthur   (1000)       78 2023-11-10 20:17:57.000000 dotenv-cli-3.2.2/dotenv_cli/version.py
-drwxr-xr-x   0 venthur   (1000) venthur   (1000)        0 2023-11-10 20:44:47.458503 dotenv-cli-3.2.2/dotenv_cli.egg-info/
--rw-r--r--   0 venthur   (1000) venthur   (1000)     4430 2023-11-10 20:44:47.000000 dotenv-cli-3.2.2/dotenv_cli.egg-info/PKG-INFO
--rw-r--r--   0 venthur   (1000) venthur   (1000)      414 2023-11-10 20:44:47.000000 dotenv-cli-3.2.2/dotenv_cli.egg-info/SOURCES.txt
--rw-r--r--   0 venthur   (1000) venthur   (1000)        1 2023-11-10 20:44:47.000000 dotenv-cli-3.2.2/dotenv_cli.egg-info/dependency_links.txt
--rw-r--r--   0 venthur   (1000) venthur   (1000)       47 2023-11-10 20:44:47.000000 dotenv-cli-3.2.2/dotenv_cli.egg-info/entry_points.txt
--rw-r--r--   0 venthur   (1000) venthur   (1000)       47 2023-11-10 20:44:47.000000 dotenv-cli-3.2.2/dotenv_cli.egg-info/requires.txt
--rw-r--r--   0 venthur   (1000) venthur   (1000)       11 2023-11-10 20:44:47.000000 dotenv-cli-3.2.2/dotenv_cli.egg-info/top_level.txt
--rw-r--r--   0 venthur   (1000) venthur   (1000)     1482 2023-11-10 20:11:32.000000 dotenv-cli-3.2.2/pyproject.toml
--rw-r--r--   0 venthur   (1000) venthur   (1000)       38 2023-11-10 20:44:47.462503 dotenv-cli-3.2.2/setup.cfg
-drwxr-xr-x   0 venthur   (1000) venthur   (1000)        0 2023-11-10 20:44:47.458503 dotenv-cli-3.2.2/tests/
--rw-r--r--   0 venthur   (1000) venthur   (1000)     1752 2023-11-10 20:11:32.000000 dotenv-cli-3.2.2/tests/test_cli.py
--rw-r--r--   0 venthur   (1000) venthur   (1000)     4069 2023-11-10 20:11:32.000000 dotenv-cli-3.2.2/tests/test_core.py
--rw-r--r--   0 venthur   (1000) venthur   (1000)      166 2023-11-10 20:11:32.000000 dotenv-cli-3.2.2/tests/test_version.py
+drwxrwxr-x   0 venthur   (1000) venthur   (1000)        0 2024-04-07 12:55:48.211474 dotenv-cli-3.3.0/
+-rw-r--r--   0 venthur   (1000) venthur   (1000)     1072 2018-10-14 16:13:37.000000 dotenv-cli-3.3.0/LICENSE
+-rw-r--r--   0 venthur   (1000) venthur   (1000)       31 2019-04-28 11:56:54.000000 dotenv-cli-3.3.0/MANIFEST.in
+-rw-r--r--   0 venthur   (1000) venthur   (1000)     4841 2024-04-07 12:55:48.211474 dotenv-cli-3.3.0/PKG-INFO
+-rw-rw-r--   0 venthur   (1000) venthur   (1000)     2610 2024-04-07 12:51:33.000000 dotenv-cli-3.3.0/README.md
+drwxrwxr-x   0 venthur   (1000) venthur   (1000)        0 2024-04-07 12:55:48.207474 dotenv-cli-3.3.0/completion/
+drwxrwxr-x   0 venthur   (1000) venthur   (1000)        0 2024-04-07 12:55:48.207474 dotenv-cli-3.3.0/completion/bash/
+-rw-r--r--   0 venthur   (1000) venthur   (1000)      869 2019-04-28 11:56:54.000000 dotenv-cli-3.3.0/completion/bash/dotenv
+drwxrwxr-x   0 venthur   (1000) venthur   (1000)        0 2024-04-07 12:55:48.207474 dotenv-cli-3.3.0/dotenv_cli/
+-rw-r--r--   0 venthur   (1000) venthur   (1000)       66 2023-07-01 11:21:02.000000 dotenv-cli-3.3.0/dotenv_cli/__init__.py
+-rw-rw-r--   0 venthur   (1000) venthur   (1000)     1661 2024-04-07 12:51:33.000000 dotenv-cli-3.3.0/dotenv_cli/cli.py
+-rw-rw-r--   0 venthur   (1000) venthur   (1000)     3311 2024-04-07 12:51:33.000000 dotenv-cli-3.3.0/dotenv_cli/core.py
+-rw-rw-r--   0 venthur   (1000) venthur   (1000)       78 2024-04-07 12:51:33.000000 dotenv-cli-3.3.0/dotenv_cli/version.py
+drwxrwxr-x   0 venthur   (1000) venthur   (1000)        0 2024-04-07 12:55:48.211474 dotenv-cli-3.3.0/dotenv_cli.egg-info/
+-rw-r--r--   0 venthur   (1000) venthur   (1000)     4841 2024-04-07 12:55:48.000000 dotenv-cli-3.3.0/dotenv_cli.egg-info/PKG-INFO
+-rw-rw-r--   0 venthur   (1000) venthur   (1000)      414 2024-04-07 12:55:48.000000 dotenv-cli-3.3.0/dotenv_cli.egg-info/SOURCES.txt
+-rw-rw-r--   0 venthur   (1000) venthur   (1000)        1 2024-04-07 12:55:48.000000 dotenv-cli-3.3.0/dotenv_cli.egg-info/dependency_links.txt
+-rw-rw-r--   0 venthur   (1000) venthur   (1000)       47 2024-04-07 12:55:48.000000 dotenv-cli-3.3.0/dotenv_cli.egg-info/entry_points.txt
+-rw-rw-r--   0 venthur   (1000) venthur   (1000)       70 2024-04-07 12:55:48.000000 dotenv-cli-3.3.0/dotenv_cli.egg-info/requires.txt
+-rw-rw-r--   0 venthur   (1000) venthur   (1000)       11 2024-04-07 12:55:48.000000 dotenv-cli-3.3.0/dotenv_cli.egg-info/top_level.txt
+-rw-rw-r--   0 venthur   (1000) venthur   (1000)     1581 2024-04-07 12:51:33.000000 dotenv-cli-3.3.0/pyproject.toml
+-rw-rw-r--   0 venthur   (1000) venthur   (1000)       38 2024-04-07 12:55:48.211474 dotenv-cli-3.3.0/setup.cfg
+drwxrwxr-x   0 venthur   (1000) venthur   (1000)        0 2024-04-07 12:55:48.211474 dotenv-cli-3.3.0/tests/
+-rw-rw-r--   0 venthur   (1000) venthur   (1000)     2577 2024-04-07 12:51:33.000000 dotenv-cli-3.3.0/tests/test_cli.py
+-rw-rw-r--   0 venthur   (1000) venthur   (1000)     4220 2024-04-07 12:51:33.000000 dotenv-cli-3.3.0/tests/test_core.py
+-rw-r--r--   0 venthur   (1000) venthur   (1000)      166 2023-11-10 20:11:32.000000 dotenv-cli-3.3.0/tests/test_version.py
```

### Comparing `dotenv-cli-3.2.2/LICENSE` & `dotenv-cli-3.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dotenv-cli-3.2.2/PKG-INFO` & `dotenv-cli-3.3.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dotenv-cli
-Version: 3.2.2
+Version: 3.3.0
 Summary: Simple dotenv CLI.
 Author-email: Bastian Venthur <mail@venthur.de>
 License: MIT License
         
         Copyright (c) 2018 Bastian Venthur
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -21,40 +21,47 @@
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
+Project-URL: Documentation, https://dotenv-cli.readthedocs.io/
 Project-URL: Source, https://github.com/venthur/dotenv-cli
 Project-URL: Changelog, https://github.com/venthur/dotenv-cli/blob/master/CHANGELOG.md
 Keywords: dotenv,cli,.env
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Provides-Extra: dev
+Requires-Dist: build; extra == "dev"
+Requires-Dist: mkdocs; extra == "dev"
+Requires-Dist: mkdocs-material; extra == "dev"
+Requires-Dist: mypy; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: ruff; extra == "dev"
-Requires-Dist: build; extra == "dev"
 Requires-Dist: twine; extra == "dev"
-Requires-Dist: mypy; extra == "dev"
 
 # dotenv CLI
 
-Dotenv-CLI is a simple package that provides the `dotenv` command. It reads the
-`.env` file from the current directory puts the contents in the environment and
-executes the given command.
+Dotenv-CLI provides the `dotenv` command. `dotenv` loads the `.env` file from
+the current directory, puts the contents in the environment by either changing
+existing- or adding new environment variables, and executes the given command.
 
 `dotenv` supports alternative `.env` files like `.env.development` via the `-e`
-or `--dotenv` parametes.
+or `--dotenv` parameters.
+
+With the `--replace` flag, `dotenv` also provides an option to completely
+replace the environment variables with the ones from the `.env` file, allowing
+you to control exactly which environment variables are set.
 
 `dotenv` provides bash completion, so you can use `dotenv` like this:
 
 ```bash
 $ dotenv make <TAB>
 all      clean    docs     lint     release  test
 ```
```

### Comparing `dotenv-cli-3.2.2/README.md` & `dotenv-cli-3.3.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 # dotenv CLI
 
-Dotenv-CLI is a simple package that provides the `dotenv` command. It reads the
-`.env` file from the current directory puts the contents in the environment and
-executes the given command.
+Dotenv-CLI provides the `dotenv` command. `dotenv` loads the `.env` file from
+the current directory, puts the contents in the environment by either changing
+existing- or adding new environment variables, and executes the given command.
 
 `dotenv` supports alternative `.env` files like `.env.development` via the `-e`
-or `--dotenv` parametes.
+or `--dotenv` parameters.
+
+With the `--replace` flag, `dotenv` also provides an option to completely
+replace the environment variables with the ones from the `.env` file, allowing
+you to control exactly which environment variables are set.
 
 `dotenv` provides bash completion, so you can use `dotenv` like this:
 
 ```bash
 $ dotenv make <TAB>
 all      clean    docs     lint     release  test
 ```
```

### Comparing `dotenv-cli-3.2.2/completion/bash/dotenv` & `dotenv-cli-3.3.0/completion/bash/dotenv`

 * *Files identical despite different names*

### Comparing `dotenv-cli-3.2.2/dotenv_cli/cli.py` & `dotenv-cli-3.3.0/dotenv_cli/cli.py`

 * *Files 11% similar despite different names*

```diff
@@ -23,35 +23,50 @@
         This if for debugging only.
 
     Returns
     -------
     argparse.Namespace
 
     """
-    parser = argparse.ArgumentParser()
+    parser = argparse.ArgumentParser(
+        description=(
+            "dotenv executes a given command with environment variables "
+            "loaded from a .env file."
+        ),
+    )
 
     parser.add_argument(
         "-e",
         "--dotenv",
-        help="Alternative .env file",
+        help="alternative .env file",
         default=".env",
     )
 
     parser.add_argument(
         "command",
-        help="Shell command to execute",
+        help="shell command to execute",
         nargs=argparse.REMAINDER,
     )
 
     parser.add_argument(
         "--version",
         action="version",
         version=__VERSION__,
     )
 
+    parser.add_argument(
+        "-r",
+        "--replace",
+        action="store_true",
+        help=(
+            "completely replace all existing environment variables with the "
+            "ones loaded from the .env file"
+            )
+    )
+
     return parser.parse_args(args)
 
 
 def main() -> NoReturn | int:
     """Run dotenv.
 
     This function parses sys.argv and runs dotenv.
@@ -62,8 +77,8 @@
         the return value
 
     """
     args = parse_args()
     if not args.command:
         return 0
 
-    return run_dotenv(args.dotenv, args.command)
+    return run_dotenv(args.dotenv, args.command, args.replace)
```

### Comparing `dotenv-cli-3.2.2/dotenv_cli/core.py` & `dotenv-cli-3.3.0/dotenv_cli/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -69,40 +69,48 @@
             value = value[1:-1]
 
         res[key] = value
     logger.debug(res)
     return res
 
 
-def run_dotenv(filename: str, command: list[str]) -> NoReturn | int:
+def run_dotenv(
+    filename: str, command: list[str], replace: bool = False
+) -> NoReturn | int:
     """Run dotenv.
 
     This function executes the commands with the environment variables
     parsed from filename.
 
     Parameters
     ----------
     filename
         path to the .env file
     command
         command to execute
+    replace_env
+        Replace the current environment instead of updating it.
 
     Returns
     -------
     NoReturn | int
         The exit status code in Windows. In POSIX-compatible systems, the
         function does not return normally.
 
     """
     # read dotenv
     dotenv = read_dotenv(filename)
 
-    # update env
-    env = os.environ.copy()
-    env.update(dotenv)
+    if replace:
+        # replace env
+        env = dotenv
+    else:
+        # update env
+        env = os.environ.copy()
+        env.update(dotenv)
 
     # in POSIX, we replace the current process with the command, execvpe does
     # not return
     if os.name == "posix":
         os.execvpe(command[0], command, env)
 
     # in Windows, we spawn a new process
```

### Comparing `dotenv-cli-3.2.2/dotenv_cli.egg-info/PKG-INFO` & `dotenv-cli-3.3.0/dotenv_cli.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dotenv-cli
-Version: 3.2.2
+Version: 3.3.0
 Summary: Simple dotenv CLI.
 Author-email: Bastian Venthur <mail@venthur.de>
 License: MIT License
         
         Copyright (c) 2018 Bastian Venthur
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -21,40 +21,47 @@
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
+Project-URL: Documentation, https://dotenv-cli.readthedocs.io/
 Project-URL: Source, https://github.com/venthur/dotenv-cli
 Project-URL: Changelog, https://github.com/venthur/dotenv-cli/blob/master/CHANGELOG.md
 Keywords: dotenv,cli,.env
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Provides-Extra: dev
+Requires-Dist: build; extra == "dev"
+Requires-Dist: mkdocs; extra == "dev"
+Requires-Dist: mkdocs-material; extra == "dev"
+Requires-Dist: mypy; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: ruff; extra == "dev"
-Requires-Dist: build; extra == "dev"
 Requires-Dist: twine; extra == "dev"
-Requires-Dist: mypy; extra == "dev"
 
 # dotenv CLI
 
-Dotenv-CLI is a simple package that provides the `dotenv` command. It reads the
-`.env` file from the current directory puts the contents in the environment and
-executes the given command.
+Dotenv-CLI provides the `dotenv` command. `dotenv` loads the `.env` file from
+the current directory, puts the contents in the environment by either changing
+existing- or adding new environment variables, and executes the given command.
 
 `dotenv` supports alternative `.env` files like `.env.development` via the `-e`
-or `--dotenv` parametes.
+or `--dotenv` parameters.
+
+With the `--replace` flag, `dotenv` also provides an option to completely
+replace the environment variables with the ones from the `.env` file, allowing
+you to control exactly which environment variables are set.
 
 `dotenv` provides bash completion, so you can use `dotenv` like this:
 
 ```bash
 $ dotenv make <TAB>
 all      clean    docs     lint     release  test
 ```
```

### Comparing `dotenv-cli-3.2.2/pyproject.toml` & `dotenv-cli-3.3.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -20,25 +20,28 @@
     "Programming Language :: Python :: 3",
 ]
 
 [project.scripts]
 dotenv = "dotenv_cli.cli:main"
 
 [project.urls]
+'Documentation' = 'https://dotenv-cli.readthedocs.io/'
 'Source' = 'https://github.com/venthur/dotenv-cli'
 'Changelog' = 'https://github.com/venthur/dotenv-cli/blob/master/CHANGELOG.md'
 
 [project.optional-dependencies]
 dev = [
+    "build",
+    "mkdocs",
+    "mkdocs-material",
+    "mypy",
     "pytest",
     "pytest-cov",
     "ruff",
-    "build",
     "twine",
-    "mypy"
 ]
 
 [tool.setuptools.dynamic]
 version = { attr = "dotenv_cli.__VERSION__" }
 
 [tool.setuptools]
 packages = ["dotenv_cli"]
@@ -48,23 +51,24 @@
     "--cov=dotenv_cli",
     "--cov=tests",
     "--cov-report=html",
     "--cov-report=term-missing:skip-covered"
 ]
 
 [tool.ruff]
+line-length = 79
+target-version = "py38"
+
+[tool.ruff.lint]
 select = [
     "F",        # pyflakes
     "E", "W",   # pycodestyle
     "C90",      # mccabe
     "I",        # isort
     "D",        # pydocstyle
     "UP"        # pyupgrade
 ]
-line-length = 79
-target-version = "py38"
+pydocstyle.convention = "numpy"
 
-[tool.ruff.pydocstyle]
-convention = "numpy"
 [tool.mypy]
 files = ["dotenv_cli", "tests"]
 strict = true
```

### Comparing `dotenv-cli-3.2.2/tests/test_cli.py` & `dotenv-cli-3.3.0/tests/test_cli.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 import tempfile
 from pathlib import Path
 from subprocess import PIPE, run
 from typing import Iterator
 
 import pytest
 
+from dotenv_cli import __VERSION__
+
 DOTENV_FILE = """
 # comment=foo
 TEST=foo
 TWOLINES='foo\nbar'
 TEST_COMMENT=foo # bar
 LINE_WITH_EQUAL='foo=bar'
 """
@@ -22,14 +24,20 @@
     _file = Path.cwd() / ".env"
     with _file.open("w") as fh:
         fh.write(DOTENV_FILE)
     yield _file
     _file.unlink()
 
 
+def test_this_dotenv() -> None:
+    """Simple test for CI to assert we're running *our* dotenv."""
+    proc = run(["dotenv", "--version"], stdout=PIPE)
+    assert __VERSION__.encode() in proc.stdout
+
+
 def test_stdout(dotenvfile: Path) -> None:
     """Test stdout."""
     proc = run(["dotenv", "echo", "test"], stdout=PIPE)
     assert b"test" in proc.stdout
 
 
 def test_stderr(dotenvfile: Path) -> None:
@@ -66,7 +74,20 @@
     assert b"does not exist" in proc.stderr
 
 
 def test_no_command() -> None:
     """Test no command."""
     proc = run(["dotenv"])
     assert proc.returncode == 0
+
+
+def test_replace_environment(dotenvfile: Path) -> None:
+    """Test replace environment."""
+    proc = run(["dotenv", "-r", "env"], stdout=PIPE)
+    # the above .env file has exactly 4 lines, on some test platforms, the CI
+    # environment itself adds a few more environment variables into the shell,
+    # see:
+    # https://stackoverflow.com/questions/78226424/custom-environment-variables-with-popen-on-windows-on-github-actions
+    assert len(proc.stdout.splitlines()) < 10
+
+    proc = run(["dotenv", "--replace", "env"], stdout=PIPE)
+    assert len(proc.stdout.splitlines()) < 10
```

### Comparing `dotenv-cli-3.2.2/tests/test_core.py` & `dotenv-cli-3.3.0/tests/test_core.py`

 * *Files 4% similar despite different names*

```diff
@@ -168,7 +168,13 @@
     TEST = "export FOO=BAR"
 
     with tempfile.NamedTemporaryFile("w", delete=False) as f:
         f.write(TEST)
 
     env = core.read_dotenv(f.name)
     assert env["FOO"] == "BAR"
+
+
+def test_non_existing_dotenv() -> None:
+    """Non-existing dotenv file."""
+    env = core.read_dotenv("/tmp/i.dont.exist")
+    assert len(env) == 0
```

