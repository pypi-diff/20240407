# Comparing `tmp/protokolo-0.2.0.tar.gz` & `tmp/protokolo-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "protokolo-0.2.0.tar", max compression
+gzip compressed data, was "protokolo-0.3.0.tar", max compression
```

## Comparing `protokolo-0.2.0.tar` & `protokolo-0.3.0.tar`

### file list

```diff
@@ -1,27 +1,28 @@
--rw-r--r--   0        0        0     1106 2023-11-07 09:38:52.982639 protokolo-0.2.0/CHANGELOG.md
-drwxr-xr-x   0        0        0        0 2023-10-19 20:10:58.496541 protokolo-0.2.0/LICENSES/
--rw-r--r--   0        0        0    18375 2023-10-19 20:10:58.496541 protokolo-0.2.0/LICENSES/CC-BY-SA-4.0.txt
--rw-r--r--   0        0        0     7048 2023-10-19 20:10:57.776495 protokolo-0.2.0/LICENSES/CC0-1.0.txt
--rw-r--r--   0        0        0    34674 2023-10-19 20:10:58.188521 protokolo-0.2.0/LICENSES/GPL-3.0-or-later.txt
--rw-r--r--   0        0        0     4821 2023-11-07 10:08:49.503330 protokolo-0.2.0/README.md
--rw-r--r--   0        0        0     1758 2023-11-07 09:37:57.924839 protokolo-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      177 2023-11-07 09:38:14.953392 protokolo-0.2.0/src/protokolo/__init__.py
--rw-r--r--   0        0        0      288 2023-10-25 21:07:33.877601 protokolo-0.2.0/src/protokolo/__main__.py
--rw-r--r--   0        0        0     3841 2023-11-06 20:24:31.978893 protokolo-0.2.0/src/protokolo/_formatter.py
--rw-r--r--   0        0        0     4206 2023-11-07 07:28:04.278102 protokolo-0.2.0/src/protokolo/_util.py
--rw-r--r--   0        0        0     7539 2023-11-07 09:13:49.816178 protokolo-0.2.0/src/protokolo/cli.py
--rw-r--r--   0        0        0     9177 2023-11-01 18:50:36.036810 protokolo-0.2.0/src/protokolo/compile.py
--rw-r--r--   0        0        0    12601 2023-11-01 09:01:42.738824 protokolo-0.2.0/src/protokolo/config.py
--rw-r--r--   0        0        0     3169 2023-10-29 08:11:06.304880 protokolo-0.2.0/src/protokolo/exceptions.py
--rw-r--r--   0        0        0        0 2023-10-21 21:28:23.558911 protokolo-0.2.0/src/protokolo/py.typed
--rw-r--r--   0        0        0      890 2023-11-01 17:19:54.550000 protokolo-0.2.0/src/protokolo/replace.py
--rw-r--r--   0        0        0      788 2023-10-28 18:00:29.613284 protokolo-0.2.0/src/protokolo/types.py
--rw-r--r--   0        0        0     2224 2023-11-07 08:51:52.167259 protokolo-0.2.0/tests/conftest.py
--rw-r--r--   0        0        0    15497 2023-11-07 10:03:40.667838 protokolo-0.2.0/tests/test_cli.py
--rw-r--r--   0        0        0    13608 2023-10-31 07:20:13.415288 protokolo-0.2.0/tests/test_compile.py
--rw-r--r--   0        0        0    14442 2023-10-30 09:13:16.697582 protokolo-0.2.0/tests/test_config.py
--rw-r--r--   0        0        0     3592 2023-10-28 21:28:57.351824 protokolo-0.2.0/tests/test_exceptions.py
--rw-r--r--   0        0        0     6084 2023-11-06 20:18:08.391190 protokolo-0.2.0/tests/test_formatter.py
--rw-r--r--   0        0        0     3279 2023-11-01 17:52:44.244904 protokolo-0.2.0/tests/test_replace.py
--rw-r--r--   0        0        0     5868 1970-01-01 00:00:00.000000 protokolo-0.2.0/setup.py
--rw-r--r--   0        0        0     5372 1970-01-01 00:00:00.000000 protokolo-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1451 2024-04-07 11:37:00.007312 protokolo-0.3.0/CHANGELOG.md
+drwxr-xr-x   0        0        0        0 2023-10-19 20:10:58.496541 protokolo-0.3.0/LICENSES/
+-rw-r--r--   0        0        0    18375 2023-10-19 20:10:58.496541 protokolo-0.3.0/LICENSES/CC-BY-SA-4.0.txt
+-rw-r--r--   0        0        0     7048 2023-10-19 20:10:57.776495 protokolo-0.3.0/LICENSES/CC0-1.0.txt
+-rw-r--r--   0        0        0    34674 2023-10-19 20:10:58.188521 protokolo-0.3.0/LICENSES/GPL-3.0-or-later.txt
+-rw-r--r--   0        0        0     5698 2024-04-07 10:36:42.970478 protokolo-0.3.0/README.md
+-rw-r--r--   0        0        0     2452 2024-04-07 11:36:14.630847 protokolo-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      177 2024-04-07 11:36:14.630847 protokolo-0.3.0/src/protokolo/__init__.py
+-rw-r--r--   0        0        0      290 2024-04-07 10:30:16.712348 protokolo-0.3.0/src/protokolo/__main__.py
+-rw-r--r--   0        0        0     3874 2024-03-08 18:49:41.103198 protokolo-0.3.0/src/protokolo/_formatter.py
+-rw-r--r--   0        0        0     1435 2024-03-08 18:20:59.913097 protokolo-0.3.0/src/protokolo/_util.py
+-rw-r--r--   0        0        0     7950 2024-04-07 10:30:16.712348 protokolo-0.3.0/src/protokolo/cli.py
+-rw-r--r--   0        0        0     9904 2024-04-07 08:08:13.113594 protokolo-0.3.0/src/protokolo/compile.py
+-rw-r--r--   0        0        0    11710 2024-04-06 19:36:36.296945 protokolo-0.3.0/src/protokolo/config.py
+-rw-r--r--   0        0        0     3171 2023-11-07 12:34:47.189029 protokolo-0.3.0/src/protokolo/exceptions.py
+-rw-r--r--   0        0        0     3778 2024-03-29 20:30:44.665888 protokolo-0.3.0/src/protokolo/initialise.py
+-rw-r--r--   0        0        0        0 2023-10-21 21:28:23.558911 protokolo-0.3.0/src/protokolo/py.typed
+-rw-r--r--   0        0        0      890 2023-11-01 17:19:54.550000 protokolo-0.3.0/src/protokolo/replace.py
+-rw-r--r--   0        0        0      930 2024-03-29 19:44:07.379769 protokolo-0.3.0/src/protokolo/types.py
+-rw-r--r--   0        0        0     2224 2024-04-06 17:40:55.028923 protokolo-0.3.0/tests/conftest.py
+-rw-r--r--   0        0        0    18254 2024-04-07 10:30:16.712348 protokolo-0.3.0/tests/test_cli.py
+-rw-r--r--   0        0        0    14236 2024-04-07 08:08:13.113594 protokolo-0.3.0/tests/test_compile.py
+-rw-r--r--   0        0        0    11411 2024-03-29 19:44:07.383769 protokolo-0.3.0/tests/test_config.py
+-rw-r--r--   0        0        0     3592 2023-10-28 21:28:57.351824 protokolo-0.3.0/tests/test_exceptions.py
+-rw-r--r--   0        0        0     6089 2023-11-07 12:32:33.427701 protokolo-0.3.0/tests/test_formatter.py
+-rw-r--r--   0        0        0     3279 2023-11-01 17:52:44.244904 protokolo-0.3.0/tests/test_replace.py
+-rw-r--r--   0        0        0     6706 1970-01-01 00:00:00.000000 protokolo-0.3.0/setup.py
+-rw-r--r--   0        0        0     6281 1970-01-01 00:00:00.000000 protokolo-0.3.0/PKG-INFO
```

### Comparing `protokolo-0.2.0/CHANGELOG.md` & `protokolo-0.3.0/CHANGELOG.md`

 * *Files 26% similar despite different names*

```diff
@@ -14,14 +14,28 @@
 - `Deprecated` for soon-to-be removed features.
 - `Removed` for now removed features.
 - `Fixed` for any bug fixes.
 - `Security` in case of vulnerabilities.
 
 <!-- protokolo-section-tag -->
 
+## 0.3.0 - 2024-04-07
+
+### Added
+
+- Added `--dry-run` to `compile`.
+
+- Added `--format` to `compile`. This is primarily useful for doing something
+  like `protokolo compile --format version 1.0.0` to format the correct version
+  into the section heading.
+
+### Changed
+
+- Re-wrote the internals to use the `attrs` library for easier validation.
+
 ## 0.2.0 - 2023-11-07
 
 This is the prototype release of Protokolo. It contains the most basic
 functionality and limited documentation, but is a minimum viable product. You
 can:
 
 - Compile the `changelog.d` directory into a CHANGELOG file with
```

### Comparing `protokolo-0.2.0/LICENSES/CC-BY-SA-4.0.txt` & `protokolo-0.3.0/LICENSES/CC-BY-SA-4.0.txt`

 * *Files identical despite different names*

### Comparing `protokolo-0.2.0/LICENSES/CC0-1.0.txt` & `protokolo-0.3.0/LICENSES/CC0-1.0.txt`

 * *Files identical despite different names*

### Comparing `protokolo-0.2.0/LICENSES/GPL-3.0-or-later.txt` & `protokolo-0.3.0/LICENSES/GPL-3.0-or-later.txt`

 * *Files identical despite different names*

### Comparing `protokolo-0.2.0/pyproject.toml` & `protokolo-0.3.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # SPDX-FileCopyrightText: 2023 Carmen Bianca BAKKER <carmen@carmenbianca.eu>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 [tool.poetry]
 name = "protokolo"
-version = "0.2.0"
+version = "0.3.0"
 description = "Protokolo is a change log generator."
 authors = [
     "Carmen Bianca BAKKER <carmen@carmenbianca.eu>"
 ]
 maintainers = [
     "Carmen Bianca BAKKER <carmen@carmenbianca.eu>"
 ]
@@ -22,47 +22,82 @@
     { path = "tests", format = "sdist" },
     { path = "README.md", format = "sdist" },
     { path = "CHANGELOG.md", format = "sdist" },
     { path = "LICENSES", format = "sdist" },
 ]
 
 [tool.poetry.scripts]
-protokolo = 'protokolo.cli:cli'
+protokolo = 'protokolo.cli:main'
 
 [tool.poetry.dependencies]
 python = "^3.11"
 click = ">=8.0"
+attrs = ">=22.1.0"
 
 [tool.poetry.group.test.dependencies]
 pytest = ">=6.0.0"
 pytest-cov = ">=2.10.0"
 freezegun = "^1.0"
 
 [tool.poetry.group.dev.dependencies]
 black = ">=20"
 isort = "^5.0.0"
 pre-commit = "^2.9.0"
-bump2version = "^1.0.0"
-pylint = "^2.12.2"
+bumpver = ">=2023.1129"
+pylint = "^3.0"
 mypy = "^1.0"
+reuse = "^3.0"
+
+[tool.poetry.group.docs]
+optional = true
+
+[tool.poetry.group.docs.dependencies]
+Sphinx = ">=7.0.0"
+sphinxcontrib-apidoc = "^0.3.0"
+myst-parser = "^2.0.0"
+furo = ">=2023.3.27"
+
+[tool.poetry.group.lsp]
+optional = true
 
 [tool.poetry.group.lsp.dependencies]
 python-lsp-server = "*"
 pylsp-mypy = "*"
 pyls-isort = "*"
 python-lsp-black = "*"
 
+[build-system]
+requires = ["poetry-core>=1.1.0"]
+build-backend = "poetry.core.masonry.api"
+
 [tool.protokolo]
 changelog = "CHANGELOG.md"
 markup = "markdown"
 directory = "changelog.d"
 
-[build-system]
-requires = ["poetry-core>=1.1.0"]
-build-backend = "poetry.core.masonry.api"
+[bumpver]
+current_version = "0.3.0"
+version_pattern = "MAJOR.MINOR.PATCH"
+commit_message = "Bump version to {new_version}"
+tag_message = "{new_version}"
+tag_scope = "default"
+pre_commit_hook = ""
+post_commit_hook = ""
+commit = true
+tag = false
+push = false
+
+[bumpver.file_patterns]
+"pyproject.toml" = [
+    '^version = "{version}"$',
+    '^current_version = "{version}"$',
+]
+"src/protokolo/__init__.py" = [
+    '^__version__ = "{version}"$',
+]
 
 [tool.black]
 line-length = 80
 
 [tool.isort]
 multi_line_output = 3
 include_trailing_comma = true
```

### Comparing `protokolo-0.2.0/src/protokolo/_formatter.py` & `protokolo-0.3.0/src/protokolo/_formatter.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,59 +7,58 @@
 from abc import ABC, abstractmethod
 from datetime import date
 from inspect import cleandoc
 from string import Template
 from typing import cast
 
 from .config import SectionAttributes
-from .exceptions import HeaderFormatError
+from .exceptions import HeadingFormatError
 
 # pylint: disable=too-few-public-methods
 
 
 class MarkupFormatter(ABC):
     """A simple formatter class."""
 
     @classmethod
     def format_section(cls, attrs: SectionAttributes) -> str:
-        """Format a title as a section header. For instance, a level-2 Markdown
+        """Format a title as a section heading. For instance, a level-2 Markdown
         section might look like this::
 
             ## Hello, world
 
         You can use ``$key`` (or ``${key}``) placeholders in the title to
         replace them with the values of the corresponding keys in *attrs*.
         ``$date`` is special in that it is replaced with today's date. ``$$`` is
         replaced by a single ``$``.
 
         Raises:
-            HeaderFormatError: could not format the header as given.
+            HeadingFormatError: could not format the heading as given.
 
         """
         cls._validate(attrs)
         title = cls._format_output(attrs)
         return cls._format_section(title, attrs)
 
     @classmethod
     def _validate(cls, attrs: SectionAttributes) -> None:
         """
         Raises:
-            HeaderFormatError: could not format the header as given.
+            HeadingFormatError: could not format the heading as given.
         """
         # This is technically invalid. Valid attrs do not have a non-positive
         # level.
         if attrs.level <= 0:
-            raise HeaderFormatError(f"Level {attrs.level} must be positive.")
+            raise HeadingFormatError(f"Level {attrs.level} must be positive.")
         if not attrs.title:
-            raise HeaderFormatError("title cannot be empty.")
+            raise HeadingFormatError("title cannot be empty.")
 
     @classmethod
     @abstractmethod
-    def _format_section(cls, title: str, attrs: SectionAttributes) -> str:
-        ...
+    def _format_section(cls, title: str, attrs: SectionAttributes) -> str: ...
 
     @classmethod
     def _format_output(cls, attrs: SectionAttributes) -> str:
         values = attrs.as_dict()
         # No recursive funny stuff.
         title = cast(str, values.pop("title"))
         # Don't render None.
@@ -82,29 +81,31 @@
 
 class ReStructuredTextFormatter(MarkupFormatter):
     """A reStructuredText formatter."""
 
     # TODO: Honestly this should be more flexible, but the amount of engineering
     # it would take to achieve that is beyond the scope of what I want to do.
     # What were the designers of reST thinking when they didn't define the
-    # header hierarchy?
+    # heading hierarchy?
     _levels = {
         1: "=",  # Special case.
         2: "=",
         3: "-",
         4: "~",
         5: "^",
         6: "'",
     }
 
     @classmethod
     def _validate(cls, attrs: SectionAttributes) -> None:
         super()._validate(attrs)
         if attrs.level > len(cls._levels):
-            raise HeaderFormatError(f"Header level {attrs.level} is too deep.")
+            raise HeadingFormatError(
+                f"Heading level {attrs.level} is too deep."
+            )
 
     @classmethod
     def _format_section(cls, title: str, attrs: SectionAttributes) -> str:
         sign = cls._levels[attrs.level]
         length = len(title)
         return cleandoc(
             f"""
```

### Comparing `protokolo-0.2.0/src/protokolo/cli.py` & `protokolo-0.3.0/src/protokolo/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,30 +8,34 @@
 import tomllib
 from io import TextIOWrapper
 from pathlib import Path
 
 import click
 
 from ._formatter import MARKUP_EXTENSION_MAPPING as _MARKUP_EXTENSION_MAPPING
-from ._util import create_changelog, create_keep_a_changelog
 from .compile import Section
 from .config import GlobalConfig
 from .exceptions import (
     AttributeNotPositiveError,
     DictTypeError,
-    HeaderFormatError,
+    HeadingFormatError,
+)
+from .initialise import (
+    create_changelog,
+    create_keep_a_changelog,
+    create_root_toml,
 )
 from .replace import find_first_occurrence, insert_into_str
 from .types import SupportedMarkup
 
 
 @click.group(name="protokolo")
 @click.version_option(package_name="protokolo")
 @click.pass_context
-def cli(ctx: click.Context) -> None:
+def main(ctx: click.Context) -> None:
     """Protokolo is a change log generator."""
     ctx.ensure_object(dict)
     if ctx.default_map is None:
         ctx.default_map = {}
 
     # Only load the global config if the subcommand needs it.
     if ctx.invoked_subcommand in ["compile", "init"]:
@@ -53,92 +57,109 @@
             ctx.default_map["init"] = {
                 "changelog": config.changelog,
                 "markup": config.markup,
                 "directory": config.directory,
             }
 
 
-@cli.command(name="compile")
+@main.command(name="compile")
 @click.option(
     "--changelog",
     show_default="determined by config",
     type=click.File("r+", encoding="utf-8", lazy=True),
     required=True,
     help="File into which to compile.",
 )
 @click.option(
     "--markup",
     default="markdown",
     show_default="determined by config, or markdown",
     type=click.Choice(SupportedMarkup.__args__),  # type: ignore
     help="Markup language.",
 )
+@click.option(
+    "--format",
+    "-f",
+    "format_",
+    type=(str, str),
+    metavar="<KEY VALUE>...",
+    multiple=True,
+    help="Use key-value pairs to string-format section headers.",
+)
+@click.option(
+    "--dry-run",
+    "-n",
+    is_flag=True,
+    help="Do not write to file system; print to STDOUT.",
+)
 @click.argument(
     "directory",
     type=click.Path(
         exists=True,
         file_okay=False,
         dir_okay=True,
         readable=True,
         path_type=Path,
     ),
     required=True,
 )
 def compile_(
     changelog: click.File,
     markup: SupportedMarkup,
+    format_: tuple[tuple[str, str], ...],
+    dry_run: bool,
     directory: Path,
 ) -> None:
-    """Compile a directory of change log entries into a CHANGELOG file.
-    Directories and subdirectories are analogous to sections and subsections,
-    and files are analogous to change log entries, typically list items in a
-    section.
+    """Aggregate all change log entries from files in a directory into a
+    CHANGELOG file.
 
     A change log directory should contain a '.protokolo.toml' file that defines
     some attributes of the section. This is an example file:
 
     \b
     [protokolo.section]
     title = "${version} - ${date}"
     level = 2
 
     When the section is compiled, it looks a little like this:
 
     ## 1.0.0 - 2023-11-08
 
-    The section header is followed by the contents of files in the section's
-    directory. The file contents are pasted as-is into the section, separated as
-    paragraphs. The entries are sorted alphabetically by file name. If you want
-    a file to go first or last, prefix it with '000_' or 'zzz_'. Only files with
-    your markup language's file extension (e.g. .md) are compiled as entries.
-
+    The heading is followed by the contents of files in the section's directory.
     If a section is empty (no change log entries), it is not compiled.
 
     The CHANGELOG file should contain the following comment, which is the
-    location in the file where compiled sections will be pasted:
+    location in the file after which the compiled section will be pasted:
 
+    \b
     <!-- protokolo-section-tag -->
 
     For more documentation and options, read the documentation at TODO.
     """
+    # TODO: Maybe split this up.
+    # pylint: disable=too-many-locals
+    format_pairs: dict[str, str] = dict(format_)
+
     # Create Section
     try:
-        section = Section.from_directory(directory, markup=markup)
+        section = Section.from_directory(
+            directory, markup=markup, section_format_pairs=format_pairs
+        )
     except (
         tomllib.TOMLDecodeError,
         DictTypeError,
         AttributeNotPositiveError,
         OSError,
     ) as error:
         raise click.UsageError(str(error)) from error
 
     # Compile Section
     try:
         new_section = section.compile()
-    except HeaderFormatError as error:
+    except HeadingFormatError as error:
         raise click.UsageError(str(error)) from error
 
     if not new_section:
         click.echo("There are no change log entries to compile.")
         return
 
     # Write to CHANGELOG
@@ -151,85 +172,92 @@
             lineno = find_first_occurrence("protokolo-section-tag", contents)
             if lineno is None:
                 raise click.UsageError(
                     f"There is no 'protokolo-section-tag' in"
                     f" {repr(changelog.name)}."
                 )
             new_contents = insert_into_str(f"\n{new_section}", contents, lineno)
-            fp.seek(0)
-            fp.write(new_contents)
-            fp.truncate()
+            if dry_run:
+                click.echo(new_contents)
+            else:
+                fp.seek(0)
+                fp.write(new_contents)
+                fp.truncate()
     except OSError as error:
         # TODO: This is a little tricky to test. click already exits early if
         # changelog isn't readable/writable.
         raise click.UsageError(str(error))
 
     # Delete change log entries
-    for dirpath, _, filenames in os.walk(directory):
-        for filename in filenames:
-            path = Path(dirpath) / filename
-            if path.suffix in _MARKUP_EXTENSION_MAPPING[markup]:
-                path.unlink()
+    if not dry_run:
+        for dirpath, _, filenames in os.walk(directory):
+            for filename in filenames:
+                path = Path(dirpath) / filename
+                if path.suffix in _MARKUP_EXTENSION_MAPPING[markup]:
+                    path.unlink()
 
 
-@cli.command(name="init")
+@main.command(name="init")
 @click.option(
     "--changelog",
     default="CHANGELOG.md",
     show_default="determined by config, or CHANGELOG.md",
     type=click.File("w", encoding="utf-8", lazy=True),
     help="CHANGELOG file to create.",
 )
 @click.option(
-    "--markup",
-    default="markdown",
-    show_default="determined by config, or markdown",
-    type=click.Choice(SupportedMarkup.__args__),  # type: ignore
-    help="Markup language.",
-)
-@click.option(
     "--directory",
     default="changelog.d",
     show_default="determined by config, or changelog.d",
     type=click.Path(
         file_okay=False,
         dir_okay=True,
         readable=True,
         path_type=Path,
     ),
     help="Directory of change log sections and entries.",
 )
+@click.option(
+    "--markup",
+    default="markdown",
+    show_default="determined by config, or markdown",
+    type=click.Choice(SupportedMarkup.__args__),  # type: ignore
+    help="Markup language.",
+)
 def init(
     changelog: click.File,
-    markup: SupportedMarkup,
     directory: Path,
+    markup: SupportedMarkup,
 ) -> None:
     """Set up your project to be ready to use Protokolo. It creates a
     CHANGELOG.md file, a changelog.d directory with subsections that match the
     Keep a Changelog recommendations, and .protokolo.toml files with metadata
     for those (sub)sections. The end result looks a little like this:
 
     \b
     .
     ├── changelog.d
-    │   ├── added
-    │   │   └── .protokolo.toml
-    │   ├── changed
-    │   │   └── .protokolo.toml
-    │   ├── deprecated
-    │   │   └── .protokolo.toml
-    │   ├── fixed
-    │   │   └── .protokolo.toml
-    │   ├── removed
-    │   │   └── .protokolo.toml
-    │   ├── security
-    │   │   └── .protokolo.toml
-    │   └── .protokolo.toml
-    └── CHANGELOG.md
+    │   ├── added
+    │   │   └── .protokolo.toml
+    │   ├── changed
+    │   │   └── .protokolo.toml
+    │   ├── deprecated
+    │   │   └── .protokolo.toml
+    │   ├── fixed
+    │   │   └── .protokolo.toml
+    │   ├── removed
+    │   │   └── .protokolo.toml
+    │   ├── security
+    │   │   └── .protokolo.toml
+    │   └── .protokolo.toml
+    ├── CHANGELOG.md
+    └── .protokolo.toml
 
-    Files that already exist are never overwritten.
+    Files that already exist are never overwritten, except the root
+    .protokolo.toml file, which is always (re-)generated.
     """
     try:
         create_changelog(changelog.name, markup)
         create_keep_a_changelog(directory)
+        create_root_toml(changelog.name, markup, directory)
     except OSError as error:
         raise click.UsageError(str(error))
```

### Comparing `protokolo-0.2.0/src/protokolo/compile.py` & `protokolo-0.3.0/src/protokolo/compile.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,105 +9,108 @@
 from io import StringIO
 from itertools import chain
 from operator import attrgetter
 from os import strerror
 from pathlib import Path
 from typing import Iterator, Self, cast
 
+import attrs as attrs_
+from attrs.converters import optional
+
 from ._formatter import MARKUP_EXTENSION_MAPPING as _MARKUP_EXTENSION_MAPPING
 from ._formatter import MARKUP_FORMATTER_MAPPING as _MARKUP_FORMATTER_MAPPING
 from .config import SectionAttributes, parse_toml
 from .exceptions import (
     AttributeNotPositiveError,
-    HeaderFormatError,
+    HeadingFormatError,
     ProtokoloTOMLIsADirectoryError,
     ProtokoloTOMLNotFoundError,
 )
 from .types import StrPath, SupportedMarkup
 
 # pylint: disable=too-few-public-methods
 
 
+@attrs_.define(frozen=True)
 class Entry:
     """An entry, analogous to a file."""
 
-    def __init__(
-        self,
-        text: str,
-        source: StrPath | None = None,
-    ):
-        self.text: str = text
-        if source is not None:
-            source = Path(source)
-        self.source: Path | None = source
+    text: str
+    source: Path | None = attrs_.field(default=None, converter=optional(Path))
 
     def compile(self) -> str:
         """Compile the entry. For the time being, this just means stripping the
         newline characters around the text.
         """
         return self.text.strip("\n")
 
 
+@attrs_.define(eq=False)
 class Section:
     """A section, analogous to a directory."""
 
-    def __init__(
-        self,
-        attrs: SectionAttributes | None = None,
-        markup: SupportedMarkup = "markdown",
-        source: StrPath | None = None,
-    ):
-        if attrs is None:
-            attrs = SectionAttributes()
-        self.attrs: SectionAttributes = attrs
-        self.markup = markup
-        if source is not None:
-            source = Path(source)
-        self.source: Path | None = source
-        self.entries: set[Entry] = set()
-        self.subsections: set[Self] = set()
+    attrs: SectionAttributes = attrs_.field(factory=SectionAttributes)
+    markup: SupportedMarkup = "markdown"
+    source: Path | None = attrs_.field(default=None, converter=optional(Path))
+
+    entries: set[Entry] = attrs_.field(factory=set, init=False)
+    subsections: set[Self] = attrs_.field(factory=set, init=False)
 
     @classmethod
     def from_directory(
         cls,
         directory: StrPath,
         level: int = 1,
         markup: SupportedMarkup = "markdown",
+        section_format_pairs: dict[str, str] | None = None,
     ) -> Self:
-        """Factory method to recursively create a Section from a directory.
+        """Factory method to recursively create a :class:`Section` from a
+        directory.
 
-        The *level* keyword argument is overridden by the level value in
-        .protokolo.toml.
+        Args:
+            directory: The changelog.d directory.
+            level: The level of the root :class:`Section`. This is overridden by
+                the level value in ``.protokolo.toml``, if any.
+            markup: The markup language.
+            section_format_pairs: Additional key-value pairs used to format the
+                section headings, applied recursively to all subsections.
 
         Raises:
             OSError: input/output error.
-            ProtokoloTOMLNotFoundError: .protokolo.toml doesn't exist.
-            ProtokoloTOMLIsADirectoryError: .protokolo.toml is not a file.
-            TOMLDecodeError: .protokolo.toml couldn't be parsed.
-            DictTypeError: .protokolo.toml fields have the wrong type.
-            AttributeNotPositiveError: value in .protokolo.toml should be a
+            ProtokoloTOMLNotFoundError: ``.protokolo.toml`` doesn't exist.
+            ProtokoloTOMLIsADirectoryError: ``.protokolo.toml`` is not a file.
+            tomllib.TOMLDecodeError: ``.protokolo.toml`` couldn't be parsed.
+            DictTypeError: ``.protokolo.toml`` fields have the wrong type.
+            AttributeNotPositiveError: value in ``.protokolo.toml`` should be a
                 positive integer.
         """
+        if section_format_pairs is None:
+            section_format_pairs = {}
+
         directory = Path(directory)
         section = cls(markup=markup, source=directory)
 
-        section._load_section_attributes(directory, level)
-        section._load_subsections_and_entries(directory, section.attrs.level)
+        section._load_section_attributes(directory, level, section_format_pairs)
+        section._load_subsections_and_entries(
+            directory, section.attrs.level, section_format_pairs
+        )
 
         return section
 
-    def _load_section_attributes(self, directory: Path, level: int) -> None:
-        """Locate .protokolo.toml and create a SectionAttributes object from it,
-        then set that object on self.
+    def _load_section_attributes(
+        self, directory: Path, level: int, section_format_pairs: dict[str, str]
+    ) -> None:
+        """Locate ``.protokolo.toml`` and create a :class:`SectionAttributes`
+        object from it, then set that object on self.
 
         Raises:
             OSError: input/output error.
-            ProtokoloTOMLNotFoundError: .protokolo.toml doesn't exist.
-            ProtokoloTOMLIsADirectoryError: .protokolo.toml is not a file.
-            TOMLDecodeError: .protokolo.toml couldn't be parsed.
+            ProtokoloTOMLNotFoundError: ``.protokolo.toml`` doesn't exist.
+            ProtokoloTOMLIsADirectoryError: ``.protokolo.toml`` is not a file.
+            tomllib.TOMLDecodeError: ``.protokolo.toml`` couldn't be parsed.
         """
         protokolo_toml = directory / ".protokolo.toml"
         if not protokolo_toml.exists():
             raise ProtokoloTOMLNotFoundError(
                 errno.ENOENT, strerror(errno.ENOENT), str(protokolo_toml)
             )
         if not protokolo_toml.is_file():
@@ -127,38 +130,43 @@
             raise AttributeNotPositiveError(
                 f"Wrong value in '{fp.name}': {error}"
             ) from error
         # The level of the current section is determined first by the value
         # in the toml, second by the level value.
         level = values.get("level") or level
         attrs.level = level
+        for key, val in section_format_pairs.items():
+            attrs[key] = val
         self.attrs = attrs
 
     def _load_subsections_and_entries(
-        self, directory: Path, level: int
+        self, directory: Path, level: int, section_format_pairs: dict[str, str]
     ) -> None:
         """Locate subsections and entries. Load entries onto self, and
         recursively create subsections to also load them onto self.
 
         Raises:
             OSError: input/output error.
-            ProtokoloTOMLNotFoundError: .protokolo.toml doesn't exist.
-            ProtokoloTOMLIsADirectoryError: .protokolo.toml is not a file.
-            TOMLDecodeError: .protokolo.toml couldn't be parsed.
-            DictTypeError: .protokolo.toml fields have the wrong type.
-            AttributeNotPositiveError: value in .protokolo.toml should be a
+            ProtokoloTOMLNotFoundError: ``.protokolo.toml`` doesn't exist.
+            ProtokoloTOMLIsADirectoryError: ``.protokolo.toml`` is not a file.
+            tomllib.TOMLDecodeError: ``.protokolo.toml`` couldn't be parsed.
+            DictTypeError: ``.protokolo.toml`` fields have the wrong type.
+            AttributeNotPositiveError: value in ``.protokolo.toml`` should be a
                 positive integer.
         """
         subsections = set()
         entries = set()
         for path in directory.iterdir():
             if path.is_dir():
                 subsections.add(
                     self.from_directory(
-                        path, level=level + 1, markup=self.markup
+                        path,
+                        level=level + 1,
+                        markup=self.markup,
+                        section_format_pairs=section_format_pairs,
                     )
                 )
             elif (
                 path.is_file()
                 and path.suffix in _MARKUP_EXTENSION_MAPPING[self.markup]
             ):
                 with path.open("r", encoding="utf-8") as fp_:
@@ -170,57 +178,57 @@
     def compile(self) -> str:
         """Compile the entire section recursively, first printing the entries in
         order, then the subsections.
 
         Empty sections are not compiled.
 
         Raises:
-            HeaderFormatError: could not format header of section.
+            HeadingFormatError: could not format heading of section.
         """
         buffer = self.write_to_buffer()
         return buffer.getvalue()
 
     def write_to_buffer(self, buffer: StringIO | None = None) -> StringIO:
-        """Like compile, but writing to a StringIO buffer.
+        """Like compile, but writing to a :class:`StringIO` buffer.
 
         Raises:
-            HeaderFormatError: could not format header of section.
+            HeadingFormatError: could not format heading of section.
         """
         if buffer is None:
             buffer = StringIO()
 
         if self.is_empty():
             return buffer
 
         try:
-            header = _MARKUP_FORMATTER_MAPPING[self.markup].format_section(
+            heading = _MARKUP_FORMATTER_MAPPING[self.markup].format_section(
                 self.attrs,
             )
-        except HeaderFormatError as error:
-            raise HeaderFormatError(
-                f"Failed to format section header of {repr(str(self.source))}:"
+        except HeadingFormatError as error:
+            raise HeadingFormatError(
+                f"Failed to format section heading of {repr(str(self.source))}:"
                 f" {str(error)}"
             ) from error
-        buffer.write(header)
+        buffer.write(heading)
 
         for entry in self.sorted_entries():
             buffer.write("\n\n")
             buffer.write(entry.compile())
 
         for subsection in self.sorted_subsections():
             if not subsection.is_empty():
                 buffer.write("\n\n")
             subsection.write_to_buffer(buffer=buffer)
 
         return buffer
 
     def is_empty(self) -> bool:
-        """A Section is empty if it contains neither entries nor subsections. If
-        it contains no entries, and its subsections are empty, then it is also
-        considered empty.
+        """A :class:`Section` is empty if it contains neither entries nor
+        subsections. If it contains no entries, and its subsections are empty,
+        then it is also considered empty.
         """
         if self.entries:
             return False
         if not self.subsections:
             return True
         for subsection in self.subsections:
             if not subsection.is_empty():
```

### Comparing `protokolo-0.2.0/src/protokolo/config.py` & `protokolo-0.3.0/src/protokolo/config.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 # SPDX-FileCopyrightText: 2023 Carmen Bianca BAKKER <carmen@carmenbianca.eu>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 """The global configuration of Protokolo."""
 
-import contextlib
 import tomllib
 from collections.abc import Sequence
 from copy import deepcopy
 from pathlib import Path
 from types import UnionType
 from typing import IO, Any, Self, cast
 
+import attrs
+
 from ._util import nested_itemgetter, type_in_expected_type
 from .exceptions import (
     AttributeNotPositiveError,
     DictTypeError,
     DictTypeListError,
 )
-from .types import NestedTypeDict, StrPath, TOMLValue, TOMLValueType
-
-# pylint: disable=too-many-arguments
+from .types import StrPath, TOMLValue, TOMLValueType
 
 
 def parse_toml(
     toml: str | IO[bytes],
     section: Sequence[str] | None = None,
 ) -> dict[str, Any]:
     """
     Args:
         toml: A TOML string or binary file object.
         sections: A list of nested sections, for example
-            ["protokolo", "section"] to return the values of [protokolo.section]
+            ``["protokolo", "section"]`` to return the values of
+            ``[protokolo.section]``
 
     Raises:
         TypeError: *toml* is not a valid type.
         tomllib.TOMLDecodeError: not valid TOML.
     """
     if isinstance(toml, str):
         values = tomllib.loads(toml)
@@ -50,126 +50,84 @@
         return values
     try:
         return nested_itemgetter(*section)(values)
     except KeyError:
         return {}
 
 
+@attrs.define
 class TOMLConfig:
     """A utility class to hold data parsed from a TOML file."""
 
-    expected_types: NestedTypeDict = {}
+    _values: dict[str, TOMLValue] = attrs.field(factory=dict)
+    source: str | None = attrs.field(converter=str, default=None)
 
-    def __init__(
-        self,
-        values: dict[str, TOMLValue] | None = None,
-        source: StrPath | None = None,
-    ):
-        if source is not None:
-            source = Path(source)
-        self.source: Path | None = source
-        if values is None:
-            values = {}
-        self._config: dict[str, TOMLValue] = deepcopy(values)
+    def __attrs_post_init__(self) -> None:
+        self._values = deepcopy(self._values)
+        # Can't use validator on the attribute itself because the validation
+        # depends on `self`. So we do the validation here.
         self.validate()
 
     @classmethod
     def from_dict(
         cls, values: dict[str, Any], source: StrPath | None = None
     ) -> Self:
-        """Generate TOMLConfig from a dictionary containing the keys and values.
-        This is useless for the TOMLConfig base class, but potentially useful
-        for subclasses that change the ``__init__`` signature.
+        """Generate :class:`TOMLConfig` from a dictionary containing the keys
+        and values. This is useless for the :class:`TOMLConfig` base class, but
+        potentially useful for subclasses that change the ``__init__``
+        signature.
 
         Raises:
             DictTypeError: value isn't an expected/supported type.
             DictTypeListError: if a list contains elements other than a dict.
         """
-        return cls(values=values, source=source)
+        return cls(values=values, source=str(source))
 
     def __getitem__(self, key: str | Sequence[str]) -> TOMLValue:
         if isinstance(key, str):
             keys = [key]
         else:
             keys = list(key)
-        return nested_itemgetter(*keys)(self._config)
+        return nested_itemgetter(*keys)(self._values)
 
     def __setitem__(self, key: str | Sequence[str], value: TOMLValue) -> None:
         if isinstance(key, str):
             final_key = key
             keys = []
         else:
             copied = list(key)
             final_key = copied.pop()
             keys = copied
-        # Technically this can fail because self._config is a Mapping instead of
-        # a MutableMapping.
-        nested_itemgetter(*keys)(self._config)[final_key] = value
+        nested_itemgetter(*keys)(self._values)[final_key] = value
 
     def as_dict(self) -> dict[str, TOMLValue]:
-        """Return a mapping of the TOMLConfig."""
-        return deepcopy(self._config)
+        """Return a mapping of the :class:`TOMLConfig`."""
+        return deepcopy(self._values)
 
     def validate(self) -> None:
         """Verify that all keys contain valid TOML types. This is automatically
         run on object instantiation.
 
-        The *expected_values* (class) attribute can contain a dictionary
-        describing the expected type of each key. For example:
-
-        >>> toml = '''
-        ...     [foo]
-        ...     hello = "world"
-        ...     [[foo.bar]]
-        ...     baz = 1
-        ...     [[foo.bar]]
-        ...     baz = 2
-        ...     '''
-        ...
-        >>> config = TOMLConfig(parse_toml(toml))
-        >>> config.expected_types = {
-        ...     "foo": dict,
-        ...     "foo+dict": {
-        ...         "hello": str,
-        ...         "bar": list,
-        ...         "bar+list": {
-        ...             "baz": int,
-        ...         }
-        ...     }
-        ... }
-        ...
-        >>> config.validate()
-
         Raises:
             DictTypeError: value isn't an expected/supported type.
             DictTypeListError: if a list contains elements other than a dict.
         """
-        self._validate(cast(dict[str, Any], self._config))
+        self._validate(cast(dict[str, Any], self._values))
 
-    def _validate(
-        self, values: dict[str, Any], path: Sequence[str] | None = None
-    ) -> None:
-        if path is None:
-            path = []
+    def _validate(self, values: dict[str, Any]) -> None:
         for name, value in values.items():
-            expected_type: UnionType = TOMLValueType
-            with contextlib.suppress(KeyError):
-                expected_type = nested_itemgetter(*(list(path) + [name]))(
-                    self.expected_types
-                )
+            # Use typed annotations to expect a very specific type. If not,
+            # allow any valid TOML type.
+            # pylint: disable=no-member
+            expected_type = self.__annotations__.get(f"_{name}", TOMLValueType)
             self._validate_item(value, name, expected_type=expected_type)
             if isinstance(value, dict):
-                self._validate(value, path=list(path) + [f"{name}+dict"])
+                self._validate(value)
             elif isinstance(value, list):
-                for item in value:
-                    if not isinstance(item, dict):
-                        raise DictTypeListError(
-                            name, dict, item, str(self.source)
-                        )
-                    self._validate(item, path=list(path) + [f"{name}+list"])
+                self._validate_list(value, name)
 
     def _validate_item(
         self,
         item: Any,
         name: str,
         expected_type: type | UnionType = TOMLValueType,
     ) -> None:
@@ -179,51 +137,65 @@
         if isinstance(item, bool) and not type_in_expected_type(
             bool, expected_type
         ):
             bool_err = True
         if bool_err or not isinstance(item, expected_type):
             raise DictTypeError(name, expected_type, item, str(self.source))
 
+    def _validate_list(
+        self,
+        values: list[Any],
+        name: str,
+    ) -> None:
+        for item in values:
+            if isinstance(item, dict):
+                self._validate(item)
+            elif isinstance(item, list):
+                self._validate_list(item, name)
+            else:
+                try:
+                    self._validate_item(item, name)
+                except DictTypeError as error:
+                    raise DictTypeListError(
+                        name, TOMLValueType, item, self.source
+                    ) from error
 
-class SectionAttributes(TOMLConfig):
-    """A data container to hold some metadata for a Section."""
 
-    expected_types = {"title": str, "level": int, "order": int | None}
+@attrs.define
+class SectionAttributes(TOMLConfig):
+    """A data container to hold some metadata for a :class:`.compile.Section`
+    object.
+    """
 
-    def __init__(
-        self,
-        title: str | None = None,
-        level: int = 1,
-        order: int | None = None,
-        values: dict[str, TOMLValue] | None = None,
-        source: StrPath | None = None,
-    ):
-        """If *title*, *level*, or *order* also occur as keys in *values*, then
-        *values* takes precedence.
-        """
-        if values is None:
-            values = {}
-        else:
-            values = deepcopy(values)
-        # Make sure these items exist in the dictionary.
-        values.setdefault("title", title)
-        values.setdefault("level", level)
-        values.setdefault("order", order)
-        if values.get("title") is None:
-            values["title"] = "TODO: No section title defined"
-        if values.get("level") is None:
-            values["level"] = 1
-        super().__init__(values, source=source)
+    _title: str = attrs.field(
+        default="TODO: No section title defined",
+        repr=False,
+        eq=False,
+        order=False,
+    )
+    _level: int = attrs.field(default=1, repr=False, eq=False, order=False)
+    _order: int | None = attrs.field(
+        default=None, repr=False, eq=False, order=False
+    )
+
+    def __attrs_post_init__(self) -> None:
+        self._values = deepcopy(self._values)
+        # The private variables are no longer used after they are written to
+        # _values.
+        self._values.setdefault("title", self._title)
+        self._values.setdefault("level", self._level)
+        self._values.setdefault("order", self._order)
+        super().__attrs_post_init__()
 
     @classmethod
     def from_dict(
         cls, values: dict[str, Any], source: StrPath | None = None
     ) -> Self:
-        """Generate SectionAttributes from a dictionary containing the keys and
-        values.
+        """Generate :class:`SectionAttributes` from a dictionary containing the
+        keys and values.
 
         Raises:
             AttributeNotPositiveError: one of the values should have been
                 positive.
             DictTypeError: value isn't an expected/supported type.
             DictTypeListError: if a list contains elements other than a dict.
         """
@@ -257,82 +229,77 @@
 
     @title.setter
     def title(self, value: str) -> None:
         self["title"] = value
 
     @property
     def level(self) -> int:
-        """The level of the section header, which must not be zero or lower."""
+        """The level of the section heading, which must not be zero or lower."""
         return cast(int, self["level"])
 
     @level.setter
     def level(self, value: int) -> None:
         self["level"] = value
 
     @property
     def order(self) -> int | None:
         """The order of the section in relation to others. It must not be zero
-        or lower, and may be None, in which case it is alphabetically sorted
-        after all sections that do have an order.
+        or lower, and may be :const:`None`, in which case it is alphabetically
+        sorted after all sections that do have an order.
         """
         return cast(int | None, self["order"])
 
     @order.setter
     def order(self, value: int | None) -> None:
         self["order"] = value
 
 
+@attrs.define
 class GlobalConfig(TOMLConfig):
-    """A container object for config values of the global .protokolo.toml."""
+    """A container object for config values of the global ``.protokolo.toml``
+    file.
+    """
 
-    expected_types = {
-        "changelog": str | None,
-        "markup": str | None,
-        "directory": str | None,
-    }
+    _changelog: str | None = attrs.field(
+        default=None, repr=False, eq=False, order=False
+    )
+    _markup: str | None = attrs.field(
+        default=None, repr=False, eq=False, order=False
+    )
+    _directory: str | None = attrs.field(
+        default=None, repr=False, eq=False, order=False
+    )
 
-    _file_section = {
+    _FILE_SECTION = {
         ".protokolo.toml": ["protokolo"],
         "pyproject.toml": ["tool", "protokolo"],
     }
 
-    def __init__(
-        self,
-        changelog: str | None = None,
-        markup: str | None = None,
-        directory: str | None = None,
-        values: dict[str, TOMLValue] | None = None,
-        source: StrPath | None = None,
-    ):
-        """If *changelog*, *markup*, or *directory* also occur as keys in
-        *values*, then *values* takes precedence.
-        """
-        if values is None:
-            values = {}
-        else:
-            values = deepcopy(values)
-        values.setdefault("changelog", changelog)
-        values.setdefault("markup", markup)
-        values.setdefault("directory", directory)
-        super().__init__(values, source=source)
+    def __attrs_post_init__(self) -> None:
+        self._values = deepcopy(self._values)
+        self._values.setdefault("changelog", self._changelog)
+        self._values.setdefault("markup", self._markup)
+        self._values.setdefault("directory", self._directory)
+        super().__attrs_post_init__()
 
     @classmethod
     def from_file(cls, path: StrPath) -> Self:
-        """Factory method to create a GlobalConfig from a path. The exact table
-        that is loaded from the file depends on the file name. In
-        pyproject.toml, the table [tool.protokolo] is loaded, whereas
-        [protokolo] is loaded everywhere else.
+        """Factory method to create a :class:`GlobalConfig` from a path. The
+        exact table that is loaded from the file depends on the file name. In
+        ``pyproject.toml``, the table ``[tool.protokolo]`` is loaded, whereas
+        ``[protokolo]`` is loaded everywhere else.
 
         Raises:
+            OSError: if the file could not be opened.
             tomllib.TOMLDecodeError: if the file could not be decoded.
             DictTypeError: value isn't an expected/supported type.
             DictTypeListError: if a list contains elements other than a dict.
         """
         path = Path(path)
-        section = cls._file_section.get(path.name, ["protokolo"])
+        section = cls._FILE_SECTION.get(path.name, ["protokolo"])
         with path.open("rb") as fp:
             try:
                 values = parse_toml(fp, section=section)
             except tomllib.TOMLDecodeError as error:
                 raise tomllib.TOMLDecodeError(
                     f"Invalid TOML in '{fp.name}': {error}"
                 ) from error
@@ -340,19 +307,19 @@
 
     @classmethod
     def find_config(cls, directory: StrPath) -> Path | None:
         """In *directory*, find the config file.
 
         The order of precedence (highest to lowest) is:
 
-        - .protokolo.toml
-        - pyproject.toml
+        - ``.protokolo.toml``
+        - ``pyproject.toml``
         """
         directory = Path(directory)
-        for name in cls._file_section:
+        for name in cls._FILE_SECTION:
             target = directory / name
             if target.exists() and target.is_file():
                 return target
         return None
 
     @property
     def changelog(self) -> str | None:
```

### Comparing `protokolo-0.2.0/src/protokolo/exceptions.py` & `protokolo-0.3.0/src/protokolo/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,9 +92,9 @@
     """Couldn't find a .protokolo.toml file."""
 
 
 class ProtokoloTOMLIsADirectoryError(IsADirectoryError, ProtokoloTOMLError):
     """.protokolo.toml is not a file."""
 
 
-class HeaderFormatError(ValueError, ProtokoloError):
-    """Could not create header."""
+class HeadingFormatError(ValueError, ProtokoloError):
+    """Could not create heading."""
```

### Comparing `protokolo-0.2.0/src/protokolo/replace.py` & `protokolo-0.3.0/src/protokolo/replace.py`

 * *Files identical despite different names*

### Comparing `protokolo-0.2.0/src/protokolo/types.py` & `protokolo-0.3.0/src/protokolo/types.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,32 +3,35 @@
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 """Some typing definitions."""
 
 from datetime import date, datetime
 from os import PathLike
 from types import UnionType
-from typing import Literal, Mapping
+from typing import Literal, Mapping, TypeAlias
 
-StrPath = str | PathLike
+# pylint: disable=invalid-name
 
-SupportedMarkup = Literal["markdown", "restructuredtext"]
+#: Anything that looks like a path.
+StrPath: TypeAlias = str | PathLike
 
-TOMLType = Mapping[str, "TOMLValue"]
-TOMLValue = (
+#: The supported markup languages.
+SupportedMarkup: TypeAlias = Literal["markdown", "restructuredtext"]
+
+#: A TOML dictionary.
+TOMLType: TypeAlias = Mapping[str, "TOMLValue"]
+#: All possible types for a value in a TOML dictionary.
+TOMLValue: TypeAlias = (
     str
     | int
     | float
     | bool
     | datetime
     | date
     | None
     | TOMLType
     | list["TOMLType"]
 )
-# Like TOMLValue, but using only Python primitives.
+#: Like :ref:`TOMLValue`, but using only Python primitives.
 TOMLValueType: UnionType = (
     str | int | float | bool | datetime | date | None | dict | list
 )
-
-NestedTypeDict = Mapping[str, "NestedTypeValue"]
-NestedTypeValue = type | UnionType | NestedTypeDict
```

### Comparing `protokolo-0.2.0/tests/conftest.py` & `protokolo-0.3.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `protokolo-0.2.0/tests/test_cli.py` & `protokolo-0.3.0/tests/test_cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,73 +1,72 @@
 # SPDX-FileCopyrightText: 2023 Carmen Bianca BAKKER <carmen@carmenbianca.eu>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 """Test the formatting code."""
 
-from contextlib import contextmanager, suppress
+import errno
 from inspect import cleandoc
 from pathlib import Path
-from typing import Generator
 
 from freezegun import freeze_time
 
 import protokolo
-from protokolo.cli import cli
+from protokolo import cli
+from protokolo.cli import main
+from protokolo.config import GlobalConfig, SectionAttributes
 
 # pylint: disable=unspecified-encoding
 
 
-@contextmanager
-def chmod(path: str | Path, mode: int) -> Generator[None, None, None]:
-    """chmod as a context manager."""
-    path = Path(path)
-    try:
-        old_mode = path.stat().st_mode
-        path.chmod(mode)
-        yield
-    finally:
-        with suppress(Exception):
-            path.chmod(old_mode)  # pylint: disable=used-before-assignment
+def raise_permission(filename):
+    """A context manager for a function that raises a permission error on
+    *filename*.
+    """
 
+    def inner(*args, **kwargs):
+        raise PermissionError(errno.EACCES, "Permission denied", filename)
 
-class TestCli:
-    """Collect all tests for cli."""
+    return inner
+
+
+class TestMain:
+    """Collect all tests for main."""
 
     def test_help_is_default(self, runner):
         """--help is optional."""
-        without_help = runner.invoke(cli, [])
-        with_help = runner.invoke(cli, ["--help"])
+        without_help = runner.invoke(main, [])
+        with_help = runner.invoke(main, ["--help"])
         assert without_help.output == with_help.output
         assert without_help.exit_code == with_help.exit_code == 0
         assert with_help.output.startswith("Usage: protokolo")
 
     def test_version(self, runner):
         """--version returns the correct version."""
-        result = runner.invoke(cli, ["--version"])
+        result = runner.invoke(main, ["--version"])
         assert result.output == f"protokolo, version {protokolo.__version__}\n"
 
 
 class TestCompile:
     """Collect all tests for compile."""
 
     def test_help_is_not_default(self, runner):
         """--help is not the default action."""
-        without_help = runner.invoke(cli, ["compile"])
-        with_help = runner.invoke(cli, ["compile", "--help"])
+        without_help = runner.invoke(main, ["compile"])
+        with_help = runner.invoke(main, ["compile", "--help"])
         assert without_help.output != with_help.output
         assert without_help.exit_code != 0
         assert with_help.exit_code == 0
 
     @freeze_time("2023-11-08")
     def test_simple(self, runner):
         """The absolute simplest case without any configuration."""
         Path("changelog.d/foo.md").write_text("Foo")
         result = runner.invoke(
-            cli,
+            main,
             [
                 "compile",
                 "--changelog",
                 "CHANGELOG.md",
                 "--markup",
                 "markdown",
                 "changelog.d",
@@ -90,19 +89,58 @@
                 ## 0.1.0 - 2020-01-01
                 """
             )
             in changelog
         )
         assert not Path("changelog.d/foo.md").exists()
 
+    @freeze_time("2023-11-08")
+    def test_with_format(self, runner):
+        """The simple case, but using --format."""
+        Path("changelog.d/foo.md").write_text("Foo")
+        result = runner.invoke(
+            main,
+            [
+                "compile",
+                "--changelog",
+                "CHANGELOG.md",
+                "--markup",
+                "markdown",
+                "--format",
+                "version",
+                "0.2.0",
+                "changelog.d",
+            ],
+        )
+        assert result.exit_code == 0
+        changelog = Path("CHANGELOG.md").read_text()
+
+        assert (
+            cleandoc(
+                """
+                Lorem ipsum.
+
+                <!-- protokolo-section-tag -->
+
+                ## 0.2.0 - 2023-11-08
+
+                Foo
+
+                ## 0.1.0 - 2020-01-01
+                """
+            )
+            in changelog
+        )
+        assert not Path("changelog.d/foo.md").exists()
+
     def test_global_config_parse_error(self, runner):
         """.protokolo.toml cannot be parsed."""
         Path(".protokolo.toml").write_text("{'Foo")
         result = runner.invoke(
-            cli,
+            main,
             [
                 "compile",
                 "--changelog",
                 "CHANGELOG.md",
                 "--markup",
                 "markdown",
                 "changelog.d",
@@ -118,15 +156,15 @@
                 """
                 [protokolo]
                 changelog = 1
                 """
             )
         )
         result = runner.invoke(
-            cli,
+            main,
             [
                 "compile",
                 "--changelog",
                 "CHANGELOG.md",
                 "--markup",
                 "markdown",
                 "changelog.d",
@@ -134,20 +172,22 @@
         )
         assert result.exit_code != 0
         assert (
             "Error: .protokolo.toml: 'changelog' does not have the correct"
             " type. Expected str | None. Got 1."
         ) in result.output
 
-    def test_global_config_not_readable(self, runner):
-        """.protokolo.toml is not readable (or any other OSError, really)."""
+    def test_global_config_not_readable(self, runner, monkeypatch):
+        """.protokolo.toml is not accessible (or any other OSError, really)."""
         Path(".protokolo.toml").touch()
-        Path(".protokolo.toml").chmod(0o100)  # write-only
+        monkeypatch.setattr(
+            GlobalConfig, "from_file", raise_permission(".protokolo.toml")
+        )
         result = runner.invoke(
-            cli,
+            main,
             [
                 "compile",
                 "--changelog",
                 "CHANGELOG.md",
                 "--markup",
                 "markdown",
                 "changelog.d",
@@ -156,15 +196,15 @@
         assert result.exit_code != 0
         assert "Permission denied" in result.output
 
     def test_section_config_parse_error(self, runner):
         """.protokolo.toml cannot be parsed."""
         Path("changelog.d/.protokolo.toml").write_text("{'Foo")
         result = runner.invoke(
-            cli,
+            main,
             [
                 "compile",
                 "--changelog",
                 "CHANGELOG.md",
                 "--markup",
                 "markdown",
                 "changelog.d",
@@ -183,15 +223,15 @@
                 """
                 [protokolo.section]
                 title = 1
                 """
             )
         )
         result = runner.invoke(
-            cli,
+            main,
             [
                 "compile",
                 "--changelog",
                 "CHANGELOG.md",
                 "--markup",
                 "markdown",
                 "changelog.d",
@@ -210,15 +250,15 @@
                 """
                 [protokolo.section]
                 level = -1
                 """
             )
         )
         result = runner.invoke(
-            cli,
+            main,
             [
                 "compile",
                 "--changelog",
                 "CHANGELOG.md",
                 "--markup",
                 "markdown",
                 "changelog.d",
@@ -226,65 +266,69 @@
         )
         assert result.exit_code != 0
         assert (
             "Error: Wrong value in 'changelog.d/.protokolo.toml': level must be"
             " a positive integer, got -1" in result.output
         )
 
-    def test_section_config_not_readable(self, runner):
-        """.protokolo.toml is not readable (or any other OSError, really)."""
+    def test_section_config_not_readable(self, runner, monkeypatch):
+        """.protokolo.toml is not accessible (or any other OSError, really)."""
         Path("changelog.d/.protokolo.toml").touch()
-        Path("changelog.d/.protokolo.toml").chmod(0o100)  # write-only
+        monkeypatch.setattr(
+            SectionAttributes,
+            "__init__",
+            raise_permission("changelog.d/.protokolo.toml"),
+        )
         result = runner.invoke(
-            cli,
+            main,
             [
                 "compile",
                 "--changelog",
                 "CHANGELOG.md",
                 "--markup",
                 "markdown",
                 "changelog.d",
             ],
         )
         assert result.exit_code != 0
         assert "Permission denied" in result.output
 
-    def test_header_format_error(self, runner):
-        """Could not format a header."""
+    def test_heading_format_error(self, runner):
+        """Could not format a heading."""
         Path("changelog.d/.protokolo.toml").write_text(
             cleandoc(
                 """
                 [protokolo.section]
                 level = 10
                 """
             )
         )
         Path("changelog.d/foo.rst").write_text("Foo")
         result = runner.invoke(
-            cli,
+            main,
             [
                 "compile",
                 "--changelog",
                 "CHANGELOG.rst",
                 "--markup",
                 "restructuredtext",
                 "changelog.d",
             ],
         )
         assert result.exit_code != 0
         assert (
-            "Error: Failed to format section header of 'changelog.d': Header"
+            "Error: Failed to format section heading of 'changelog.d': Heading"
             " level 10 is too deep." in result.output
         )
 
     def test_nothing_to_compile(self, runner):
         """There are no change log entries."""
         changelog = Path("CHANGELOG.md").read_text()
         result = runner.invoke(
-            cli,
+            main,
             [
                 "compile",
                 "--changelog",
                 "CHANGELOG.md",
                 "--markup",
                 "markdown",
                 "changelog.d",
@@ -295,15 +339,15 @@
         assert Path("CHANGELOG.md").read_text() == changelog
 
     def test_no_replacement_tag(self, runner):
         """There is no protokolo-section-tag in CHANGELOG."""
         Path("CHANGELOG.md").write_text("Hello, world!")
         Path("changelog.d/foo.md").write_text("Foo")
         result = runner.invoke(
-            cli,
+            main,
             [
                 "compile",
                 "--changelog",
                 "CHANGELOG.md",
                 "--markup",
                 "markdown",
                 "changelog.d",
@@ -319,15 +363,15 @@
     def test_nested_entries_deleted(self, runner):
         """Entries in nested sections are also deleted, but other files are
         not.
         """
         Path("changelog.d/feature/foo.md").write_text("Foo")
         Path("changelog.d/feature/bar.txt").write_text("Bar")
         result = runner.invoke(
-            cli,
+            main,
             [
                 "compile",
                 "--changelog",
                 "CHANGELOG.md",
                 "--markup",
                 "markdown",
                 "changelog.d",
@@ -359,15 +403,15 @@
 
     @freeze_time("2023-11-08")
     def test_restructuredtext(self, runner):
         """A simple test, but for restructuredtext."""
         Path("changelog.d/foo.rst").write_text("Foo")
         Path("changelog.d/feature/bar.rst").write_text("Bar")
         result = runner.invoke(
-            cli,
+            main,
             [
                 "compile",
                 "--changelog",
                 "CHANGELOG.rst",
                 "--markup",
                 "restructuredtext",
                 "changelog.d",
@@ -399,29 +443,69 @@
                 """
             )
             in changelog
         )
         assert not Path("changelog.d/feature/bar.rst").exists()
         assert not Path("changelog.d/foo.rst").exists()
 
+    @freeze_time("2023-11-08")
+    def test_dry_run(self, runner):
+        """Test that no filesystem changes are made during dry run."""
+        Path("changelog.d/foo.md").write_text("Foo")
+        changelog_text = Path("CHANGELOG.md").read_text()
+
+        result = runner.invoke(
+            main,
+            [
+                "compile",
+                "--changelog",
+                "CHANGELOG.md",
+                "--dry-run",
+                "changelog.d",
+            ],
+        )
+        assert result.exit_code == 0
+        assert Path("CHANGELOG.md").read_text() == changelog_text
+        assert Path("changelog.d/foo.md").exists()
+        assert Path("changelog.d/foo.md").read_text() == "Foo"
+
+        assert result.stdout.strip() == cleandoc(
+            """
+            # Change log
+
+            Lorem ipsum.
+
+            <!-- protokolo-section-tag -->
+
+            ## ${version} - 2023-11-08
+
+            Foo
+
+            ## 0.1.0 - 2020-01-01
+
+            First release.
+            """
+        )
+        assert result.stdout.endswith("\n")
+
 
 class TestInit:
     """Collect all tests for init."""
 
     def test_help_is_not_default(self, runner):
         """--help is not the default action."""
-        without_help = runner.invoke(cli, ["init"])
-        with_help = runner.invoke(cli, ["init", "--help"])
+        without_help = runner.invoke(main, ["init"])
+        with_help = runner.invoke(main, ["init", "--help"])
         assert without_help.output != with_help.output
         assert without_help.exit_code == 0
         assert with_help.exit_code == 0
 
     def test_simple(self, empty_runner):
         """Use without any parameters; correctly set up files."""
-        result = empty_runner.invoke(cli, ["init"])
+        result = empty_runner.invoke(main, ["init"])
         assert result.exit_code == 0
         assert "# Change log" in Path("CHANGELOG.md").read_text()
         main_section_toml = Path("changelog.d/.protokolo.toml").read_text()
         assert "[protokolo.section]" in main_section_toml
         assert "title =" in main_section_toml
         assert "level = 2" in main_section_toml
         sections = [
@@ -436,60 +520,75 @@
             assert path.name in sections + [".protokolo.toml"]
         subsection_toml = Path("changelog.d/added/.protokolo.toml").read_text()
         assert "[protokolo.section]" in subsection_toml
         assert 'title = "Added"' in subsection_toml
         assert "order = 1" in subsection_toml
         for section in sections:
             assert Path(f"changelog.d/{section}/.protokolo.toml").is_file()
+        assert Path(".protokolo.toml").exists()
+        root_toml = Path(".protokolo.toml").read_text()
+        assert 'changelog = "CHANGELOG.md"' in root_toml
+        assert 'markup = "markdown"' in root_toml
+        assert 'directory = "changelog.d"' in root_toml
 
     def test_changelog_option(self, empty_runner):
         """Use with --changelog option."""
-        result = empty_runner.invoke(cli, ["init", "--changelog", "CHANGELOG"])
+        result = empty_runner.invoke(main, ["init", "--changelog", "CHANGELOG"])
         assert result.exit_code == 0
         assert "# Change log" in Path("CHANGELOG").read_text()
         assert not Path("CHANGELOG.md").exists()
+        assert (
+            'changelog = "CHANGELOG"\n' in Path(".protokolo.toml").read_text()
+        )
 
     def test_markup_option(self, empty_runner):
         """Use with --markup option."""
         result = empty_runner.invoke(
-            cli, ["init", "--markup", "restructuredtext"]
+            main, ["init", "--markup", "restructuredtext"]
         )
         assert result.exit_code == 0
         assert (
             "==========\nChange log\n=========="
             in Path("CHANGELOG.md").read_text()
         )
+        assert (
+            'markup = "restructuredtext"' in Path(".protokolo.toml").read_text()
+        )
 
     def test_directory_option(self, empty_runner):
         """Use with --directory option."""
-        result = empty_runner.invoke(cli, ["init", "--directory", "foo"])
+        result = empty_runner.invoke(main, ["init", "--directory", "foo"])
         assert result.exit_code == 0
         assert Path("foo").is_dir()
         assert Path("foo/.protokolo.toml").exists()
         assert not Path("changelog.d").exists()
+        assert 'directory = "foo"' in Path(".protokolo.toml").read_text()
 
     def test_run_twice(self, empty_runner):
         """Invoke twice without problems."""
-        empty_runner.invoke(cli, ["init"])
-        result = empty_runner.invoke(cli, ["init"])
+        empty_runner.invoke(main, ["init"])
+        result = empty_runner.invoke(main, ["init"])
         assert result.exit_code == 0
 
     def test_do_not_override(self, empty_runner):
         """Do not override contents of files."""
-        empty_runner.invoke(cli, ["init"])
+        empty_runner.invoke(main, ["init"])
         Path("CHANGELOG.md").write_text("foo")
         Path("changelog.d/.protokolo.toml").write_text("foo")
         Path("changelog.d/added/.protokolo.toml").write_text("foo")
-        result = empty_runner.invoke(cli, ["init"])
+        result = empty_runner.invoke(main, ["init"])
         assert result.exit_code == 0
         assert Path("CHANGELOG.md").read_text() == "foo"
         assert Path("changelog.d/.protokolo.toml").read_text() == "foo"
         assert Path("changelog.d/added/.protokolo.toml").read_text() == "foo"
 
-    def test_oserror(self, empty_runner):
+    def test_oserror(self, empty_runner, monkeypatch):
         """Handle OSErrors"""
-        empty_runner.invoke(cli, ["init"])
-        Path("changelog.d/added/.protokolo.toml").unlink()
-        with chmod("changelog.d/added", 0o000):
-            result = empty_runner.invoke(cli, ["init"])
+        empty_runner.invoke(main, ["init"])
+        monkeypatch.setattr(
+            cli,
+            "create_keep_a_changelog",
+            raise_permission("changelog.d"),
+        )
+        result = empty_runner.invoke(main, ["init"])
         assert result.exit_code != 0
         assert "Permission denied" in result.output
```

### Comparing `protokolo-0.2.0/tests/test_compile.py` & `protokolo-0.3.0/tests/test_compile.py`

 * *Files 2% similar despite different names*

```diff
@@ -306,15 +306,19 @@
             "Hello, world!"
         )
         (project_dir / "changelog.d/feature/feature_1.md").write_text(
             "- Added feature."
         )
         section = Section.from_directory(project_dir / "changelog.d")
         assert section.attrs.level == 2
-        assert section.attrs.title == "${version} - ${date}"
+        assert (
+            # Strange pylint false positive here.
+            section.attrs.title  # pylint: disable=no-member
+            == "${version} - ${date}"
+        )
         assert len(section.entries) == 1
         announcement = next(iter(section.entries))
         assert announcement.text == "Hello, world!"
         assert (
             announcement.source == project_dir / "changelog.d/announcement.md"
         )
         assert len(section.subsections) == 1
@@ -324,14 +328,26 @@
         assert len(subsection.entries) == 1
         feature = next(iter(subsection.entries))
         assert feature.text == "- Added feature."
         assert (
             feature.source == project_dir / "changelog.d/feature/feature_1.md"
         )
 
+    def test_from_directory_additional_format_pairs(self, project_dir):
+        """Provide additional section format pairs to Section, and make sure
+        they are set on the SectionAttributes.
+        """
+        section = Section.from_directory(
+            project_dir / "changelog.d",
+            section_format_pairs={"version": "0.2.0"},
+        )
+        assert section.attrs["version"] == "0.2.0"
+        for subsection in section.subsections:
+            assert subsection.attrs["version"] == "0.2.0"
+
     def test_from_directory_decode_error(self, project_dir):
         """Raise TOMLDecodeError if there is invalid TOML."""
         (project_dir / "changelog.d/.protokolo.toml").write_text(
             "{'hello': 'world'}"
         )
         with pytest.raises(tomllib.TOMLDecodeError) as exc_info:
             Section.from_directory(project_dir / "changelog.d")
```

### Comparing `protokolo-0.2.0/tests/test_config.py` & `protokolo-0.3.0/tests/test_config.py`

 * *Files 18% similar despite different names*

```diff
@@ -101,46 +101,39 @@
             "float": 3.14,
             "bool": True,
             "datetime": now_datetime,
             "date": now_date,
             "none": None,
             "dict": {"foo": "bar"},
             "list": [{"foo": "bar"}, {"baz": "quz"}],
+            "list-primitive": [1, 2],
         }
         config = TOMLConfig.from_dict(values)
         assert config["str"] == "foo"
         assert config["int"] == 100
         assert config["float"] == 3.14
         assert config["bool"] is True
         assert config["datetime"] == now_datetime
         assert config["date"] == now_date
         assert config["none"] is None
         assert config["dict"] == {"foo": "bar"}
         assert config["list"] == [{"foo": "bar"}, {"baz": "quz"}]
+        assert config["list-primitive"] == [1, 2]
 
     def test_from_dict_unsupported_type(self):
         """Many complex types are not supported."""
         value = object()
         with pytest.raises(DictTypeError) as exc_info:
             TOMLConfig.from_dict({"foo": value})
         error = exc_info.value
         assert error.key == "foo"
         assert error.expected_type == TOMLValueType
         # TODO: This is not true because error.got is a (deep)copy of value.
         # assert error.got == value
 
-    def test_from_dict_list_no_dict_inside(self):
-        """A list is always a list of dicts."""
-        with pytest.raises(DictTypeListError) as exc_info:
-            TOMLConfig.from_dict({"foo": [1]})
-        error = exc_info.value
-        assert error.key == "foo"
-        assert error.expected_type == dict
-        assert error.got == 1
-
     def test_setitem(self):
         """You can set an item on the TOMLConfig object."""
         config = TOMLConfig.from_dict({"foo": "bar"})
         config["foo"] = "baz"
         assert config["foo"] == "baz"
 
     def test_setitem_doesnt_exist(self):
@@ -166,112 +159,41 @@
         with pytest.raises(DictTypeError) as exc_info:
             config.validate()
         error = exc_info.value
         assert error.key == "foo"
         assert error.expected_type == TOMLValueType
         assert error.got == value
 
-    def test_validate_simple_expected(self):
-        """No error when validating a valid expected type."""
-        config = TOMLConfig.from_dict({"foo": "bar"})
-        config.expected_types = {"foo": str}
-        config.validate()
-
-    def test_validate_nested_expected(self):
-        """No error when validating a valid nested expected type."""
-        config = TOMLConfig.from_dict({"foo": {"bar": "baz"}})
-        config.expected_types = {"foo": dict, "foo+dict": {"bar": str}}
-        config.validate()
-
-    def test_validate_simple_not_expected(self):
-        """Error when validating an invalid expected type."""
-        config = TOMLConfig.from_dict({"foo": "bar"})
-        config.expected_types = {"foo": int}
-        with pytest.raises(DictTypeError) as exc_info:
-            config.validate()
-        error = exc_info.value
-        assert error.key == "foo"
-        assert error.expected_type == int
-        assert error.got == "bar"
-
-    def test_validate_list_wrong_type(self):
-        """If a value is a list instead of the expected type, raise an error."""
-        config = TOMLConfig.from_dict({"foo": [{"bar": "baz"}]})
-        config.expected_types = {"foo": str}
-        with pytest.raises(DictTypeError) as exc_info:
-            config.validate()
-        error = exc_info.value
-        assert error.key == "foo"
-        assert error.expected_type == str
-        assert error.got == [{"bar": "baz"}]
-
-    def test_validate_dict_wrong_type(self):
-        """If a value is a dict instead of the expected type, raise an error."""
-        config = TOMLConfig.from_dict({"foo": {"bar": "baz"}})
-        config.expected_types = {"foo": str}
-        with pytest.raises(DictTypeError) as exc_info:
+    def test_validate_list_item(self):
+        """List items get a special exception DictTypeListError."""
+        config = TOMLConfig()
+        value = object()
+        config["foo"] = [value]  # type: ignore
+        with pytest.raises(DictTypeListError) as exc_info:
             config.validate()
         error = exc_info.value
         assert error.key == "foo"
-        assert error.expected_type == str
-        assert error.got == {"bar": "baz"}
-
-    def test_validate_item_of_list(self):
-        """Validate the items of lists."""
-        config = TOMLConfig.from_dict({"foo": [{"bar": "baz"}, {"bar": "quz"}]})
-        config.expected_types = {"foo": list, "foo+list": {"bar": str}}
-        config.validate()
-
-    def test_validate_very_nested(self):
-        """A rather complex nesting test."""
-        config = TOMLConfig.from_dict(
-            {
-                "foo": {
-                    "bar": {
-                        "baz": [
-                            {"quz": 1},
-                            {"quz": 2},
-                        ]
-                    }
-                }
-            }
-        )
-        config.expected_types = {
-            "foo": dict,
-            "foo+dict": {
-                "bar": dict,
-                "bar+dict": {
-                    "baz": list,
-                    "baz+list": {
-                        "quz": int,
-                    },
-                },
-            },
-        }
-        config.validate()
+        assert error.expected_type == TOMLValueType
+        assert error.got == value
 
 
 class TestSectionAttributes:
     """Collect all tests for SectionAttributes."""
 
     def test_level_positive(self):
         """level must be a positive integer."""
         SectionAttributes(level=1)
-        # Automagically fix unexpected type
-        attrs = SectionAttributes(level=None)  # type: ignore
-        assert attrs.level == 1
         with pytest.raises(AttributeNotPositiveError):
             SectionAttributes(level=0)
         with pytest.raises(AttributeNotPositiveError):
             SectionAttributes(level=-1)
 
     def test_order_positive(self):
         """order must be a positive integer."""
         SectionAttributes(order=1)
-        SectionAttributes(order=None)
         with pytest.raises(AttributeNotPositiveError):
             SectionAttributes(order=0)
         with pytest.raises(AttributeNotPositiveError):
             SectionAttributes(order=-1)
 
     def test_from_dict_simple(self):
         """Provide all values."""
@@ -298,45 +220,42 @@
         assert from_dict.level == empty.level == 1
         assert from_dict.order == empty.order == None
 
     def test_from_dict_wrong_type_level(self):
         """If the level is not an int, expect an error."""
         # No errors
         SectionAttributes.from_dict({"level": 1})
-        SectionAttributes.from_dict({"level": None})
         # Errors
         wrong_values = {"1", 1.1, "1.1", "Foo", True}
         for value in wrong_values:
             with pytest.raises(DictTypeError) as exc_info:
                 SectionAttributes.from_dict({"level": value})
             error = exc_info.value
             assert error.key == "level"
             assert error.expected_type == int
             assert error.got == value
 
     def test_from_dict_wrong_type_order(self):
         """If the order is not an int, expect an error."""
         # No errors
         SectionAttributes.from_dict({"order": 1})
-        SectionAttributes.from_dict({"order": None})
         # Errors
         wrong_values = {"1", 1.1, "1.1", "Foo", True}
         for value in wrong_values:
             with pytest.raises(DictTypeError) as exc_info:
                 SectionAttributes.from_dict({"order": value})
             error = exc_info.value
             assert error.key == "order"
             assert error.expected_type == int | None
             assert error.got == value
 
     def test_from_dict_wrong_type_title(self):
         """If the title is not a str, expect an error."""
         # No errors
         SectionAttributes.from_dict({"title": "Foo"})
-        SectionAttributes.from_dict({"title": None})
         # Errors
         wrong_values = {1, 1.1, False}
         for value in wrong_values:
             with pytest.raises(DictTypeError) as exc_info:
                 SectionAttributes.from_dict({"title": value})
             error = exc_info.value
             assert error.key == "title"
```

### Comparing `protokolo-0.2.0/tests/test_exceptions.py` & `protokolo-0.3.0/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `protokolo-0.2.0/tests/test_formatter.py` & `protokolo-0.3.0/tests/test_formatter.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from inspect import cleandoc
 
 import pytest
 from freezegun import freeze_time
 
 from protokolo._formatter import MarkdownFormatter, ReStructuredTextFormatter
 from protokolo.config import SectionAttributes
-from protokolo.exceptions import HeaderFormatError
+from protokolo.exceptions import HeadingFormatError
 
 
 class TestMarkdownFormatter:
     """Collect all tests for MarkdownFormatter."""
 
     def test_format_section_one_level(self):
         """Format an h1 section."""
@@ -44,31 +44,31 @@
                     SectionAttributes(title="Foo", level=i)
                 )
                 == "#" * i + " Foo"
             )
 
     def test_format_section_no_title(self):
         """Cannot format a section without a title."""
-        with pytest.raises(HeaderFormatError):
+        with pytest.raises(HeadingFormatError):
             MarkdownFormatter.format_section(
                 SectionAttributes(title="", level=1)
             )
 
     def test_format_section_zero_level(self):
         """A section must have a level."""
         attrs = SectionAttributes(title="Foo", level=1)
         attrs.level = 0
-        with pytest.raises(HeaderFormatError):
+        with pytest.raises(HeadingFormatError):
             MarkdownFormatter.format_section(attrs)
 
     def test_format_section_negative_level(self):
         """Level cannot be negative."""
         attrs = SectionAttributes(title="Foo", level=1)
         attrs.level = -1
-        with pytest.raises(HeaderFormatError):
+        with pytest.raises(HeadingFormatError):
             MarkdownFormatter.format_section(attrs)
 
     def test_format_section_format_simple(self):
         """Do additional formatting in the title."""
         assert (
             MarkdownFormatter.format_section(
                 SectionAttributes(
@@ -175,15 +175,15 @@
             Hello, world
             ------------
             """
         )
 
     def test_format_section_level_too_deep(self):
         """Very deep sections are not supported."""
-        with pytest.raises(HeaderFormatError):
+        with pytest.raises(HeadingFormatError):
             ReStructuredTextFormatter.format_section(
                 SectionAttributes(title="Foo", level=10)
             )
 
     def test_format_with_replacement(self):
         """The length of the section symbols adjusts to the rendered text."""
         assert ReStructuredTextFormatter.format_section(
```

### Comparing `protokolo-0.2.0/tests/test_replace.py` & `protokolo-0.3.0/tests/test_replace.py`

 * *Files identical despite different names*

### Comparing `protokolo-0.2.0/setup.py` & `protokolo-0.3.0/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -7,24 +7,24 @@
 packages = \
 ['protokolo']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['click>=8.0']
+['attrs>=22.1.0', 'click>=8.0']
 
 entry_points = \
-{'console_scripts': ['protokolo = protokolo.cli:cli']}
+{'console_scripts': ['protokolo = protokolo.cli:main']}
 
 setup_kwargs = {
     'name': 'protokolo',
-    'version': '0.2.0',
+    'version': '0.3.0',
     'description': 'Protokolo is a change log generator.',
-    'long_description': "<!--\nSPDX-FileCopyrightText: 2023 Carmen Bianca BAKKER <carmen@carmenbianca.eu>\n\nSPDX-License-Identifier: CC-BY-SA-4.0 OR GPL-3.0-or-later\n-->\n\n# Protokolo\n\nProtokolo is a change log generator.\n\nProtokolo allows you to maintain your change log entries in separate files, and\nthen finally aggregate them into a new section in CHANGELOG just before release.\n\n## Table of Contents\n\n- [Background](#background)\n- [Install](#install)\n- [Usage](#usage)\n- [Maintainers](#maintainers)\n- [Contributing](#contributing)\n- [License](#license)\n\n## Background\n\nChange logs are [a really good idea](https://keepachangelog.com/).\nUnfortunately, they are also a bit of a pain when combined with version control:\n\n- If two pull requests edit CHANGELOG, there is a non-zero chance that you'll\n  need to resolve a conflict when trying to merge them both.\n- Just after you make a release, you need to create a new section in CHANGELOG\n  for your next release. If you forget this busywork, new feature branches will\n  need to create this section, which increases the chance of merge conflicts.\n- If a feature branch adds a change log entry to the section for the next v1.2.3\n  release, and v1.2.3 subsequently releases without merging that feature branch,\n  then merging that feature branch afterwards would still add the change log\n  entry to the v1.2.3 section, even though it should now go to the v1.3.0\n  section.\n\nLife would be a lot easier if you didn't have to deal with these problems.\n\nEnter Protokolo. The idea is very simple: For every change log entry, create a\nnew file. Finally, just before release, compile the contents of those files into\na new section in CHANGELOG, and delete the files.\n\n## Install\n\nProtokolo is a regular Python package. You can install it using\n`pipx install protokolo`. Make sure that `~/.local/share/bin` is in your `$PATH`\nwith `pipx ensurepath`.\n\n## Usage\n\nTo set up your project for use with Protokolo, run `protokolo init`. This will\ncreate a `CHANGELOG.md` file (if one did not already exist) and a directory\nstructure under `changelog.d`. The directory structure uses the\n[Keep a Changelog](https://keepachangelog.com/) sections, and ends up looking\nlike this:\n\n```\n.\n├── changelog.d\n│\xa0\xa0 ├── added\n│\xa0\xa0 │\xa0\xa0 └── .protokolo.toml\n│\xa0\xa0 ├── changed\n│\xa0\xa0 │\xa0\xa0 └── .protokolo.toml\n│\xa0\xa0 ├── deprecated\n│\xa0\xa0 │\xa0\xa0 └── .protokolo.toml\n│\xa0\xa0 ├── fixed\n│\xa0\xa0 │\xa0\xa0 └── .protokolo.toml\n│\xa0\xa0 ├── removed\n│\xa0\xa0 │\xa0\xa0 └── .protokolo.toml\n│\xa0\xa0 ├── security\n│\xa0\xa0 │\xa0\xa0 └── .protokolo.toml\n│\xa0\xa0 └── .protokolo.toml\n└── CHANGELOG.md\n```\n\nThe `.protokolo.toml` files contain metadata for their respective sections; the\nsection title, header level, and order. Their inclusion is mandatory.\n\nTo add a change log entry, create the file `changelog.d/added/my_feature.md`,\nand write something like:\n\n```markdown\n- Added `--my-new-feature` option.\n```\n\nNote the item dash at the start; Protokolo does not add them for you. What you\nwrite is exactly what you get.\n\nYou can add more files. Change log entries in the same section (read: directory)\nare sorted alphabetically by their file name. If you want to make certain that\nsome change log entries go first or last, prefix the file with `000_` or `zzz_`.\nFor example, you can create `changelog.d/added/000_important_feature.md` to make\nit appear first.\n\nFinally, compile your change log with\n`protokolo compile --changelog CHANGELOG.md changelog.d`. This will take all\nchange log entries from `changelog.d` and put them in your `CHANGELOG.md`. If we\nrun it now, the following section is added after the\n`<!-- protokolo-section-tag -->` comment:\n\n```markdown\n## ${version} - 2023-11-08\n\n### Added\n\n- Added important feature.\n\n- Added `--my-new-feature` option.\n```\n\nThe Markdown files in `changelog.d/added/` are deleted. You can manually replace\n`${version}` with a release version, or you can pass the option\n`--format version=1.0.0` to `protokolo compile` to format the header at compile\ntime (TODO: not implemented yet).\n\nFor more documentation and options, read the documentation at TODO.\n\n## Maintainers\n\n- Carmen Bianca BAKKER <carmen@carmenbianca.eu>\n\n## Contributing\n\nThe code and issue tracker is hosted at\n<https://codeberg.org/carmenbianca/protokolo>. You are welcome to open any\nissues. For pull requests, bug fixes are always welcome, but new features should\nprobably be discussed in any issue first.\n\n## License\n\nAll code is licensed under GPL-3.0-or-later.\n\nAll documentation is licensed under CC-BY-SA-4.0 OR GPL-3.0-or-later.\n\nSome configuration files are licensed under CC0-1.0 OR GPL-3.0-or-later.\n\nThe repository is [REUSE](https://reuse.software)-compliant. Check the\nindividual files for their exact licensing.\n",
+    'long_description': "<!--\nSPDX-FileCopyrightText: 2023 Carmen Bianca BAKKER <carmen@carmenbianca.eu>\n\nSPDX-License-Identifier: CC-BY-SA-4.0 OR GPL-3.0-or-later\n-->\n\n# Protokolo\n\n[![Latest Protokolo version](https://img.shields.io/pypi/v/protokolo.svg)](https://pypi.python.org/pypi/protokolo)\n[![Supported Python versions](https://img.shields.io/pypi/pyversions/protokolo.svg)](https://pypi.python.org/pypi/protokolo)\n[![REUSE status](https://api.reuse.software/badge/codeberg.org/carmenbianca/protokolo)](https://api.reuse.software/info/codeberg.org/carmenbianca/protokolo)\n[![standard-readme compliant](https://img.shields.io/badge/readme%20style-standard-brightgreen.svg)](https://github.com/RichardLitt/standard-readme)\n\nProtokolo is a change log generator.\n\nProtokolo allows you to maintain your change log entries in separate files, and\nthen finally aggregate them into a new section in CHANGELOG just before release.\n\n## Table of Contents\n\n- [Background](#background)\n- [Install](#install)\n- [Usage](#usage)\n- [Maintainers](#maintainers)\n- [Contributing](#contributing)\n- [License](#license)\n\n## Background\n\nChange logs are [a really good idea](https://keepachangelog.com/).\nUnfortunately, they are also a bit of a pain when combined with version control:\n\n- If two pull requests edit CHANGELOG, there is a non-zero chance that you'll\n  need to resolve a conflict when trying to merge them both.\n- Just after you make a release, you need to create a new section in CHANGELOG\n  for your next release. If you forget this busywork, new feature branches will\n  need to create this section, which increases the chance of merge conflicts.\n- If a feature branch adds a change log entry to the section for the next v1.2.3\n  release, and v1.2.3 subsequently releases without merging that feature branch,\n  then merging that feature branch afterwards would still add the change log\n  entry to the v1.2.3 section, even though it should now go to the v1.3.0\n  section.\n\nLife would be a lot easier if you didn't have to deal with these problems.\n\nEnter Protokolo. The idea is very simple: For every change log entry, create a\nnew file. Finally, just before release, compile the contents of those files into\na new section in CHANGELOG, and delete the files.\n\n## Install\n\nProtokolo is a regular Python package. You can install it using\n`pipx install protokolo`. Make sure that `~/.local/share/bin` is in your `$PATH`\nwith `pipx ensurepath`.\n\n## Usage\n\nFor full documentation and options, read the documentation at TODO.\n\n### Initial set-up\n\nTo set up your project for use with Protokolo, run `protokolo init`. This will\ncreate a `CHANGELOG.md` file (if one did not already exist) and a directory\nstructure under `changelog.d`. The directory structure uses the\n[Keep a Changelog](https://keepachangelog.com/) sections, and ends up looking\nlike this:\n\n```\n.\n├── changelog.d\n│   ├── added\n│   │   └── .protokolo.toml\n│   ├── changed\n│   │   └── .protokolo.toml\n│   ├── deprecated\n│   │   └── .protokolo.toml\n│   ├── fixed\n│   │   └── .protokolo.toml\n│   ├── removed\n│   │   └── .protokolo.toml\n│   ├── security\n│   │   └── .protokolo.toml\n│   └── .protokolo.toml\n├── CHANGELOG.md\n└── .protokolo.toml\n```\n\nThe `.protokolo.toml` files in `changelog.d` contain metadata for their\nrespective sections; the section title, heading level, and order. Their\ninclusion is mandatory.\n\nThe `.protokolo.toml` file in the root of the project contains configurations\nfor Protokolo that reduce the amount of typing you need to do when running\ncommands.\n\nIf a `CHANGELOG.md` file already existed, make sure to add a line containing\n`<!-- protokolo-section-tag -->` just before the heading of the latest release.\n\n### Adding entries\n\nTo add a change log entry, create the file `changelog.d/added/my_feature.md`,\nand write something like:\n\n```markdown\n- Added `--my-new-feature` option.\n```\n\nNote the item dash at the start; Protokolo does not add them for you. What you\nwrite is exactly what you get.\n\nYou can add more files. Change log entries in the same section (read: directory)\nare sorted alphabetically by their file name. If you want to make certain that\nsome change log entries go first or last, prefix the file with `000_` or `zzz_`.\nFor example, you can create `changelog.d/added/000_important_feature.md` to make\nit appear first.\n\n### Compiling your change log\n\nYou compile your change log with `protokolo compile`. This will take all change\nlog entries from `changelog.d` and put them in your `CHANGELOG.md`. If we run it\nnow, the following section is added after the `<!-- protokolo-section-tag -->`\ncomment:\n\n```markdown\n## ${version} - 2023-11-08\n\n### Added\n\n- Added important feature.\n\n- Added `--my-new-feature` option.\n```\n\nThe Markdown files in `changelog.d/added/` are deleted. You can manually replace\n`${version}` with a release version, or you can pass the option\n`--format version 1.0.0` to `protokolo compile` to format the heading at compile\ntime.\n\n## Maintainers\n\n- Carmen Bianca BAKKER <carmen@carmenbianca.eu>\n\n## Contributing\n\nThe code and issue tracker is hosted at\n<https://codeberg.org/carmenbianca/protokolo>. You are welcome to open any\nissues. For pull requests, bug fixes are always welcome, but new features should\nprobably be discussed in any issue first.\n\n## License\n\nAll code is licensed under GPL-3.0-or-later.\n\nAll documentation is licensed under CC-BY-SA-4.0 OR GPL-3.0-or-later.\n\nSome configuration files are licensed under CC0-1.0 OR GPL-3.0-or-later.\n\nThe repository is [REUSE](https://reuse.software)-compliant. Check the\nindividual files for their exact licensing.\n",
     'author': 'Carmen Bianca BAKKER',
     'author_email': 'carmen@carmenbianca.eu',
     'maintainer': 'Carmen Bianca BAKKER',
     'maintainer_email': 'carmen@carmenbianca.eu',
     'url': 'None',
     'package_dir': package_dir,
     'packages': packages,
```

### Comparing `protokolo-0.2.0/PKG-INFO` & `protokolo-0.3.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,20 @@
-Metadata-Version: 2.1
-Name: protokolo
-Version: 0.2.0
-Summary: Protokolo is a change log generator.
-License: GPL-3.0-or-later
-Author: Carmen Bianca BAKKER
-Author-email: carmen@carmenbianca.eu
-Maintainer: Carmen Bianca BAKKER
-Maintainer-email: carmen@carmenbianca.eu
-Requires-Python: >=3.11,<4.0
-Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: click (>=8.0)
-Description-Content-Type: text/markdown
-
 <!--
 SPDX-FileCopyrightText: 2023 Carmen Bianca BAKKER <carmen@carmenbianca.eu>
 
 SPDX-License-Identifier: CC-BY-SA-4.0 OR GPL-3.0-or-later
 -->
 
 # Protokolo
 
+[![Latest Protokolo version](https://img.shields.io/pypi/v/protokolo.svg)](https://pypi.python.org/pypi/protokolo)
+[![Supported Python versions](https://img.shields.io/pypi/pyversions/protokolo.svg)](https://pypi.python.org/pypi/protokolo)
+[![REUSE status](https://api.reuse.software/badge/codeberg.org/carmenbianca/protokolo)](https://api.reuse.software/info/codeberg.org/carmenbianca/protokolo)
+[![standard-readme compliant](https://img.shields.io/badge/readme%20style-standard-brightgreen.svg)](https://github.com/RichardLitt/standard-readme)
+
 Protokolo is a change log generator.
 
 Protokolo allows you to maintain your change log entries in separate files, and
 then finally aggregate them into a new section in CHANGELOG just before release.
 
 ## Table of Contents
 
@@ -62,41 +51,56 @@
 
 Protokolo is a regular Python package. You can install it using
 `pipx install protokolo`. Make sure that `~/.local/share/bin` is in your `$PATH`
 with `pipx ensurepath`.
 
 ## Usage
 
+For full documentation and options, read the documentation at TODO.
+
+### Initial set-up
+
 To set up your project for use with Protokolo, run `protokolo init`. This will
 create a `CHANGELOG.md` file (if one did not already exist) and a directory
 structure under `changelog.d`. The directory structure uses the
 [Keep a Changelog](https://keepachangelog.com/) sections, and ends up looking
 like this:
 
 ```
 .
 ├── changelog.d
-│   ├── added
-│   │   └── .protokolo.toml
-│   ├── changed
-│   │   └── .protokolo.toml
-│   ├── deprecated
-│   │   └── .protokolo.toml
-│   ├── fixed
-│   │   └── .protokolo.toml
-│   ├── removed
-│   │   └── .protokolo.toml
-│   ├── security
-│   │   └── .protokolo.toml
-│   └── .protokolo.toml
-└── CHANGELOG.md
+│   ├── added
+│   │   └── .protokolo.toml
+│   ├── changed
+│   │   └── .protokolo.toml
+│   ├── deprecated
+│   │   └── .protokolo.toml
+│   ├── fixed
+│   │   └── .protokolo.toml
+│   ├── removed
+│   │   └── .protokolo.toml
+│   ├── security
+│   │   └── .protokolo.toml
+│   └── .protokolo.toml
+├── CHANGELOG.md
+└── .protokolo.toml
 ```
 
-The `.protokolo.toml` files contain metadata for their respective sections; the
-section title, header level, and order. Their inclusion is mandatory.
+The `.protokolo.toml` files in `changelog.d` contain metadata for their
+respective sections; the section title, heading level, and order. Their
+inclusion is mandatory.
+
+The `.protokolo.toml` file in the root of the project contains configurations
+for Protokolo that reduce the amount of typing you need to do when running
+commands.
+
+If a `CHANGELOG.md` file already existed, make sure to add a line containing
+`<!-- protokolo-section-tag -->` just before the heading of the latest release.
+
+### Adding entries
 
 To add a change log entry, create the file `changelog.d/added/my_feature.md`,
 and write something like:
 
 ```markdown
 - Added `--my-new-feature` option.
 ```
@@ -106,36 +110,35 @@
 
 You can add more files. Change log entries in the same section (read: directory)
 are sorted alphabetically by their file name. If you want to make certain that
 some change log entries go first or last, prefix the file with `000_` or `zzz_`.
 For example, you can create `changelog.d/added/000_important_feature.md` to make
 it appear first.
 
-Finally, compile your change log with
-`protokolo compile --changelog CHANGELOG.md changelog.d`. This will take all
-change log entries from `changelog.d` and put them in your `CHANGELOG.md`. If we
-run it now, the following section is added after the
-`<!-- protokolo-section-tag -->` comment:
+### Compiling your change log
+
+You compile your change log with `protokolo compile`. This will take all change
+log entries from `changelog.d` and put them in your `CHANGELOG.md`. If we run it
+now, the following section is added after the `<!-- protokolo-section-tag -->`
+comment:
 
 ```markdown
 ## ${version} - 2023-11-08
 
 ### Added
 
 - Added important feature.
 
 - Added `--my-new-feature` option.
 ```
 
 The Markdown files in `changelog.d/added/` are deleted. You can manually replace
 `${version}` with a release version, or you can pass the option
-`--format version=1.0.0` to `protokolo compile` to format the header at compile
-time (TODO: not implemented yet).
-
-For more documentation and options, read the documentation at TODO.
+`--format version 1.0.0` to `protokolo compile` to format the heading at compile
+time.
 
 ## Maintainers
 
 - Carmen Bianca BAKKER <carmen@carmenbianca.eu>
 
 ## Contributing
 
@@ -150,8 +153,7 @@
 
 All documentation is licensed under CC-BY-SA-4.0 OR GPL-3.0-or-later.
 
 Some configuration files are licensed under CC0-1.0 OR GPL-3.0-or-later.
 
 The repository is [REUSE](https://reuse.software)-compliant. Check the
 individual files for their exact licensing.
-
```

