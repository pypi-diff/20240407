# Comparing `tmp/dotbackup-1.1.0.tar.gz` & `tmp/dotbackup-1.2.0.tar.gz`

## Comparing `dotbackup-1.1.0.tar` & `dotbackup-1.2.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     4772 2020-02-02 00:00:00.000000 dotbackup-1.1.0/dotbackup.1.adoc
--rw-r--r--   0        0        0     4773 2020-02-02 00:00:00.000000 dotbackup-1.1.0/dotsetup.1.adoc
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 dotbackup-1.1.0/requirements.txt
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 dotbackup-1.1.0/setup.cfg
--rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 dotbackup-1.1.0/.github/workflows/lint.yml
--rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 dotbackup-1.1.0/.github/workflows/release.yml
--rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 dotbackup-1.1.0/.github/workflows/style.yml
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 dotbackup-1.1.0/.github/workflows/test.yml
--rwxr-xr-x   0        0        0    12933 2020-02-02 00:00:00.000000 dotbackup-1.1.0/src/dotbackup.py
--rw-r--r--   0        0        0     4648 2020-02-02 00:00:00.000000 dotbackup-1.1.0/tests/helper.py
--rw-r--r--   0        0        0     1813 2020-02-02 00:00:00.000000 dotbackup-1.1.0/tests/misc_test.py
--rw-r--r--   0        0        0     4541 2020-02-02 00:00:00.000000 dotbackup-1.1.0/tests/test_basic.py
--rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 dotbackup-1.1.0/tests/test_complex_script.py
--rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 dotbackup-1.1.0/tests/test_ignore.py
--rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 dotbackup-1.1.0/tests/configs/basic.yml
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 dotbackup-1.1.0/tests/configs/complex_script.yml
--rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 dotbackup-1.1.0/tests/configs/ignore.yml
--rw-r--r--   0        0        0     3139 2020-02-02 00:00:00.000000 dotbackup-1.1.0/.gitignore
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 dotbackup-1.1.0/LICENSE
--rw-r--r--   0        0        0     2979 2020-02-02 00:00:00.000000 dotbackup-1.1.0/README.md
--rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 dotbackup-1.1.0/hatch_build.py
--rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 dotbackup-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     4132 2020-02-02 00:00:00.000000 dotbackup-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     4839 2020-02-02 00:00:00.000000 dotbackup-1.2.0/dotbackup.1.adoc
+-rw-r--r--   0        0        0     4840 2020-02-02 00:00:00.000000 dotbackup-1.2.0/dotsetup.1.adoc
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 dotbackup-1.2.0/requirements.txt
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 dotbackup-1.2.0/setup.cfg
+-rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 dotbackup-1.2.0/.github/workflows/lint.yml
+-rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 dotbackup-1.2.0/.github/workflows/release.yml
+-rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 dotbackup-1.2.0/.github/workflows/style.yml
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 dotbackup-1.2.0/.github/workflows/test.yml
+-rwxr-xr-x   0        0        0    12850 2020-02-02 00:00:00.000000 dotbackup-1.2.0/src/dotbackup.py
+-rw-r--r--   0        0        0     4648 2020-02-02 00:00:00.000000 dotbackup-1.2.0/tests/helper.py
+-rw-r--r--   0        0        0     1808 2020-02-02 00:00:00.000000 dotbackup-1.2.0/tests/misc_test.py
+-rw-r--r--   0        0        0     5318 2020-02-02 00:00:00.000000 dotbackup-1.2.0/tests/test_basic.py
+-rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 dotbackup-1.2.0/tests/test_complex_script.py
+-rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 dotbackup-1.2.0/tests/test_ignore.py
+-rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 dotbackup-1.2.0/tests/configs/basic.yml
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 dotbackup-1.2.0/tests/configs/complex_script.yml
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 dotbackup-1.2.0/tests/configs/ignore.yml
+-rw-r--r--   0        0        0     3139 2020-02-02 00:00:00.000000 dotbackup-1.2.0/.gitignore
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 dotbackup-1.2.0/LICENSE
+-rw-r--r--   0        0        0     2993 2020-02-02 00:00:00.000000 dotbackup-1.2.0/README.md
+-rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 dotbackup-1.2.0/hatch_build.py
+-rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 dotbackup-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     4241 2020-02-02 00:00:00.000000 dotbackup-1.2.0/PKG-INFO
```

### Comparing `dotbackup-1.1.0/dotbackup.1.adoc` & `dotbackup-1.2.0/dotbackup.1.adoc`

 * *Files 1% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 
 == Name
 
 dotbackup - YAML config based backup utility
 
 == Synopsis
 
-*dotbackup* [-h|--help] [-c|--config _CONFIG_] [-V|--version] [--clean]
-[--log-level _LOG_LEVEL_] [_APP_...]
+*dotbackup* [-h|--help] [-c|--config _CONFIG_] [-l|--list] [-V|--version]
+[--clean] [--log-level _LOG_LEVEL_] [_APP_...]
 
 == Description
 
 Usually people maintain backup and setup scripts along with their dotfiles. But
 these scripts always contain a lot of repeat codes, and writing them is not fun!
 dotbackup and dotsetup are here to help.
 
@@ -37,14 +37,17 @@
 
 *-c, --config*=_CONFIG_::
 	Set configuration file path (default: _~/.config/dotbackup/dotbackup.yml_).
 	Configuration files under _~/.config/dotbackup_ can also be specified by their
 	basenames, e.g., _~/.config/dotbackup/config.yml_ can be specified by
 	_config_. See _CONFIGURATION_ section for configuration definition.
 
+*-l, --list*::
+	List configured application and exit.
+
 *-V, --version*::
 	Print the version information and exit.
 
 *--clean*::
 	Do clean backup, i.e., delete old backup files before backup.
 
 *--log-level* _LOG_LEVEL_::
```

### Comparing `dotbackup-1.1.0/dotsetup.1.adoc` & `dotbackup-1.2.0/dotsetup.1.adoc`

 * *Files 1% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 
 == Name
 
 dotsetup - YAML config based backup utility
 
 == Synopsis
 
-*dotsetup* [-h|--help] [-c|--config _CONFIG_] [-V|--version] [--clean]
-[--log-level _LOG_LEVEL_] [_APP_...]
+*dotsetup* [-h|--help] [-c|--config _CONFIG_] [-l|--list] [-V|--version]
+[--clean] [--log-level _LOG_LEVEL_] [_APP_...]
 
 == Description
 
 Usually people maintain backup and setup scripts along with their dotfiles. But
 these scripts always contain a lot of repeat codes, and writing them is not fun!
 dotbackup and dotsetup are here to help.
 
@@ -37,14 +37,17 @@
 
 *-c, --config*=_CONFIG_::
 	Set configuration file path (default: _~/.config/dotbackup/dotbackup.yml_).
 	Configuration files under _~/.config/dotbackup_ can also be specified by their
 	basenames, e.g., _~/.config/dotbackup/config.yml_ can be specified by
 	_config_. See _CONFIGURATION_ section for configuration definition.
 
+*-l, --list*::
+	List configured application and exit.
+
 *-V, --version*::
 	Print the version information and exit.
 
 *--clean*::
 	Do clean setup, i.e., delete old configuration files before setup.
 
 *--log-level* _LOG_LEVEL_::
```

### Comparing `dotbackup-1.1.0/.github/workflows/lint.yml` & `dotbackup-1.2.0/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `dotbackup-1.1.0/.github/workflows/release.yml` & `dotbackup-1.2.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `dotbackup-1.1.0/.github/workflows/test.yml` & `dotbackup-1.2.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `dotbackup-1.1.0/src/dotbackup.py` & `dotbackup-1.2.0/src/dotbackup.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import sys
 from argparse import ArgumentParser
 from logging import Formatter, Logger, LogRecord
 from pathlib import Path
 
 from ruamel.yaml import YAML
 
-__VERSION__ = "1.1.0"
+__VERSION__ = "1.2.0"
 
 
 class ColorFormatter(Formatter):
     def format(self, record: LogRecord) -> str:  # pragma: no cover
         template = "\x1b[%dm{}\x1b[00m"
 
         if record.levelno == logging.INFO:
@@ -80,24 +80,33 @@
 
     @classmethod
     def parse_args(cls, args):
         """Return a new Config object based on the parsed CLI arguments."""
 
         cls._LOGGER.setLevel(args.log_level)
 
+        if args.version:
+            cls.print_version()
+            sys.exit()
+
         if (
             args.config.endswith(".yml")
             or "/" in args.config
             or os.path.isfile(args.config)
         ):
             config_file = args.config
         else:
             config_file = f"{cls._CONFIG_DIR}/{args.config}.yml"
 
         config = cls.fromfile(config_file)
+
+        if args.list:
+            config._list_apps()
+            sys.exit()
+
         if args.clean:
             config._dict["clean"] = True
         config._dict["selected_apps"] = list(args.app)
 
         return config
 
     @classmethod
@@ -109,14 +118,20 @@
         parser.add_argument(
             "-c",
             "--config",
             default=cls._DEFAULT_CONFIG_FILE,
             help=f"Configuration file (default: {cls._DEFAULT_CONFIG_FILE}).",
         )
         parser.add_argument(
+            "-l",
+            "--list",
+            action="store_true",
+            help="List configured applications and exit.",
+        )
+        parser.add_argument(
             "-V",
             "--version",
             action="store_true",
             help="Print the version number of dotbackup and exit.",
         )
         parser.add_argument(
             "--clean",
@@ -142,26 +157,14 @@
     @classmethod
     def main_parser(cls):
         """Return argument parser for dotbackup.py."""
 
         parser = ArgumentParser(
             prog="dotbackup.py", description="YAML config based backup utility."
         )
-        parser.add_argument(
-            "-V",
-            "--version",
-            action="store_true",
-            help="Print the version number of dotbackup and exit.",
-        )
-        parser.add_argument(
-            "--log-level",
-            default="INFO",
-            choices=("DEBUG", "INFO", "WARNING", "ERROR", "CRITICAL"),
-            help="Set the log level (default: INFO).",
-        )
         subparsers = parser.add_subparsers(
             title="subcommands",
             dest="command",
             help="Sub-command to be executed.",
         )
         backup_parser = subparsers.add_parser(
             "backup", help="Do backup based on the YAML configuration."
@@ -329,14 +332,18 @@
                 dest_path.parent.mkdir(parents=True, exist_ok=True)
                 shutil.copy2(src_path, dest_path)
 
     def _set_env(self) -> None:
         """Set environment variable."""
         os.environ["BACKUP_DIR"] = self._backup_dir
 
+    def _list_apps(self) -> None:
+        """List configured applications."""
+        print("\n".join(self._apps_dict.keys()))
+
     def backup(self) -> int:
         """Do backup."""
 
         if not self._check_apps():
             return 1
 
         self._set_env()
@@ -395,18 +402,14 @@
 
     if args is None:
         args = sys.argv[1:]
 
     parser = Config.dotbackup_parser()
     args = parser.parse_args(args)
 
-    if args.version:
-        Config.print_version()
-        return 0
-
     try:
         return Config.parse_args(args).backup()
     except RuntimeError as e:
         logger.error(" ".join(e.args))
         return 1
 
 
@@ -417,18 +420,14 @@
 
     if args is None:
         args = sys.argv[1:]
 
     parser = Config.dotsetup_parser()
     args = parser.parse_args(args)
 
-    if args.version:
-        Config.print_version()
-        return 0
-
     try:
         return Config.parse_args(args).setup()
     except RuntimeError as e:
         logger.error(" ".join(e.args))
         return 1
 
 
@@ -439,17 +438,17 @@
 
     if args is None:
         args = sys.argv[1:]
 
     parser = Config.main_parser()
     args = parser.parse_args(args)
 
-    if args.version:
-        Config.print_version()
-        return 0
+    if not args.command:
+        parser.print_help()
+        return 1
 
     try:
         config = Config.parse_args(args)
     except RuntimeError as e:
         logger.error(" ".join(e.args))
         return 1
```

### Comparing `dotbackup-1.1.0/tests/helper.py` & `dotbackup-1.2.0/tests/helper.py`

 * *Files identical despite different names*

### Comparing `dotbackup-1.1.0/tests/misc_test.py` & `dotbackup-1.2.0/tests/misc_test.py`

 * *Files 20% similar despite different names*

```diff
@@ -21,24 +21,26 @@
     assert dotbackup.dotsetup() == 1
     assert dotbackup.main(["backup"]) == 1
     assert dotbackup.main(["setup"]) == 1
 
 
 @pytest.mark.parametrize("option", ["-V", "--version"])
 def test_version(option, capfd):
-    assert dotbackup.dotbackup([option]) == 0
+    with pytest.raises(SystemExit):
+        dotbackup.dotbackup([option])
     assert capfd.readouterr().out == f"dotbackup {dotbackup.__VERSION__}\n"
-    assert dotbackup.dotsetup([option]) == 0
+    with pytest.raises(SystemExit):
+        dotbackup.dotsetup([option])
     assert capfd.readouterr().out == f"dotbackup {dotbackup.__VERSION__}\n"
 
-    assert dotbackup.main([option]) == 0
+    with pytest.raises(SystemExit):
+        dotbackup.main(["backup", option])
     assert capfd.readouterr().out == f"dotbackup {dotbackup.__VERSION__}\n"
-    assert dotbackup.main(["backup", option]) == 0
-    assert capfd.readouterr().out == f"dotbackup {dotbackup.__VERSION__}\n"
-    assert dotbackup.main(["setup", option]) == 0
+    with pytest.raises(SystemExit):
+        dotbackup.main(["setup", option])
     assert capfd.readouterr().out == f"dotbackup {dotbackup.__VERSION__}\n"
 
 
 def test_shortcut(monkeypatch):
     """Test configuration shortcut."""
 
     parser = Config.dotsetup_parser()
```

### Comparing `dotbackup-1.1.0/tests/test_basic.py` & `dotbackup-1.2.0/tests/test_basic.py`

 * *Files 18% similar despite different names*

```diff
@@ -127,7 +127,26 @@
 
         helper.mkdir("~/backup/.config/app_a")
 
         assert dotbackup.dotsetup(["--clean"]) == 0
         assert helper.validate_setup(self._config)
         for file in self._files:
             assert not os.path.isfile(file)
+
+    @pytest.mark.parametrize("option", ["-l", "--list"])
+    def test_list(self, option, capfd):
+        """Test -l, --list option."""
+        expected_output = "\n".join(self._config._apps_dict.keys()) + "\n"
+
+        with pytest.raises(SystemExit):
+            dotbackup.dotbackup([option])
+        assert capfd.readouterr().out == expected_output
+        with pytest.raises(SystemExit):
+            dotbackup.dotsetup([option])
+        assert capfd.readouterr().out == expected_output
+
+        with pytest.raises(SystemExit):
+            dotbackup.main(["backup", option])
+        assert capfd.readouterr().out == expected_output
+        with pytest.raises(SystemExit):
+            dotbackup.main(["setup", option])
+        assert capfd.readouterr().out == expected_output
```

### Comparing `dotbackup-1.1.0/tests/test_ignore.py` & `dotbackup-1.2.0/tests/test_ignore.py`

 * *Files identical despite different names*

### Comparing `dotbackup-1.1.0/tests/configs/basic.yml` & `dotbackup-1.2.0/tests/configs/basic.yml`

 * *Files identical despite different names*

### Comparing `dotbackup-1.1.0/.gitignore` & `dotbackup-1.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `dotbackup-1.1.0/LICENSE` & `dotbackup-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dotbackup-1.1.0/README.md` & `dotbackup-1.2.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -31,16 +31,16 @@
 
 - [PyPI](https://pypi.org/project/dotbackup)
 - [AUR](https://aur.archlinux.org/packages/dotbackup)
 
 Installing from a package manager gives you the two commands - `dotbackup` and
 `dotsetup`, and the manpages. But you can also download this single script:
 [dotbackup.py](./src/dotbackup.py). In fact, `dotbackup` and `dotsetup` are just
-shortcut commands of `dotbackup.py`, which means that `dotbackup` equals to
-`dotbackup.py backup` and `dotsetup` equals to `dotbackup.py setup`.
+shortcut commands of `dotbackup.py`, which means that `dotbackup` is equivalent
+to `dotbackup.py backup` and `dotsetup` is equivalent to `dotbackup.py setup`.
 
 ## Quick Start
 
 Write a simple configuration and place it to `~/.config/dotbackup/dotbackup.yml`:
 
 ```yml
 backup_dir: ~/backup
```

### Comparing `dotbackup-1.1.0/hatch_build.py` & `dotbackup-1.2.0/hatch_build.py`

 * *Files identical despite different names*

### Comparing `dotbackup-1.1.0/pyproject.toml` & `dotbackup-1.2.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -18,15 +18,17 @@
 	"Programming Language :: Python :: 3.8",
 	"Programming Language :: Python :: 3.9",
 	"Programming Language :: Python :: 3.10",
 	"Programming Language :: Python :: 3.11",
 	"Programming Language :: Python :: 3.12",
 	"License :: OSI Approved :: MIT License",
 	"Operating System :: POSIX",
-	"Development Status :: 5 - Production/Stable"
+	"Development Status :: 5 - Production/Stable",
+	"Topic :: System :: Archiving :: Backup",
+	"Intended Audience :: Developers",
 ]
 
 [project.scripts]
 dotbackup = "dotbackup:dotbackup"
 dotsetup = "dotbackup:dotsetup"
 
 [project.urls]
```

### Comparing `dotbackup-1.1.0/PKG-INFO` & `dotbackup-1.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 Metadata-Version: 2.3
 Name: dotbackup
-Version: 1.1.0
+Version: 1.2.0
 Summary: YAML config based backup utility. Easy to use yet flexible. With a primary focus on dotfile backup & setup, but not limited to dotfiles.
 Project-URL: Homepage, https://github.com/jaxvanyang/dotbackup
 Project-URL: Source, https://github.com/jaxvanyang/dotbackup
 Project-URL: Repository, https://github.com/jaxvanyang/dotbackup.git
 Project-URL: Issues, https://github.com/jaxvanyang/dotbackup/issues
 Author-email: Jax Young <jaxvanyang@gmail.com>
 License-File: LICENSE
 Keywords: YAML,backup,dotfiles
 Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Classifier: Topic :: System :: Archiving :: Backup
 Requires-Python: >=3.8
 Requires-Dist: ruamel-yaml
 Description-Content-Type: text/markdown
 
 # dotbackup
 
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/dotbackup)
@@ -56,16 +58,16 @@
 
 - [PyPI](https://pypi.org/project/dotbackup)
 - [AUR](https://aur.archlinux.org/packages/dotbackup)
 
 Installing from a package manager gives you the two commands - `dotbackup` and
 `dotsetup`, and the manpages. But you can also download this single script:
 [dotbackup.py](./src/dotbackup.py). In fact, `dotbackup` and `dotsetup` are just
-shortcut commands of `dotbackup.py`, which means that `dotbackup` equals to
-`dotbackup.py backup` and `dotsetup` equals to `dotbackup.py setup`.
+shortcut commands of `dotbackup.py`, which means that `dotbackup` is equivalent
+to `dotbackup.py backup` and `dotsetup` is equivalent to `dotbackup.py setup`.
 
 ## Quick Start
 
 Write a simple configuration and place it to `~/.config/dotbackup/dotbackup.yml`:
 
 ```yml
 backup_dir: ~/backup
```

