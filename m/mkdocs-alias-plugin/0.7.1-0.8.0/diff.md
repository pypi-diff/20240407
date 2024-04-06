# Comparing `tmp/mkdocs-alias-plugin-0.7.1.tar.gz` & `tmp/mkdocs-alias-plugin-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs-alias-plugin-0.7.1.tar", last modified: Thu Mar  7 16:55:45 2024, max compression
+gzip compressed data, was "mkdocs-alias-plugin-0.8.0.tar", last modified: Sat Apr  6 22:50:37 2024, max compression
```

## Comparing `mkdocs-alias-plugin-0.7.1.tar` & `mkdocs-alias-plugin-0.8.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 16:55:45.308763 mkdocs-alias-plugin-0.7.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-03-07 16:55:36.000000 mkdocs-alias-plugin-0.7.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     7432 2024-03-07 16:55:45.308763 mkdocs-alias-plugin-0.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6784 2024-03-07 16:55:36.000000 mkdocs-alias-plugin-0.7.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 16:55:45.308763 mkdocs-alias-plugin-0.7.1/alias/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 16:55:36.000000 mkdocs-alias-plugin-0.7.1/alias/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5804 2024-03-07 16:55:36.000000 mkdocs-alias-plugin-0.7.1/alias/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 16:55:45.308763 mkdocs-alias-plugin-0.7.1/mkdocs_alias_plugin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7432 2024-03-07 16:55:45.000000 mkdocs-alias-plugin-0.7.1/mkdocs_alias_plugin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-03-07 16:55:45.000000 mkdocs-alias-plugin-0.7.1/mkdocs_alias_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-07 16:55:45.000000 mkdocs-alias-plugin-0.7.1/mkdocs_alias_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-03-07 16:55:45.000000 mkdocs-alias-plugin-0.7.1/mkdocs_alias_plugin.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-07 16:55:45.000000 mkdocs-alias-plugin-0.7.1/mkdocs_alias_plugin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-07 16:55:45.000000 mkdocs-alias-plugin-0.7.1/mkdocs_alias_plugin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-07 16:55:45.308763 mkdocs-alias-plugin-0.7.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-03-07 16:55:36.000000 mkdocs-alias-plugin-0.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 22:50:37.365961 mkdocs-alias-plugin-0.8.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-06 22:50:32.000000 mkdocs-alias-plugin-0.8.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     8591 2024-04-06 22:50:37.365961 mkdocs-alias-plugin-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7741 2024-04-06 22:50:32.000000 mkdocs-alias-plugin-0.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 22:50:37.365961 mkdocs-alias-plugin-0.8.0/alias/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 22:50:32.000000 mkdocs-alias-plugin-0.8.0/alias/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8040 2024-04-06 22:50:32.000000 mkdocs-alias-plugin-0.8.0/alias/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 22:50:37.365961 mkdocs-alias-plugin-0.8.0/mkdocs_alias_plugin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8591 2024-04-06 22:50:37.000000 mkdocs-alias-plugin-0.8.0/mkdocs_alias_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-06 22:50:37.000000 mkdocs-alias-plugin-0.8.0/mkdocs_alias_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 22:50:37.000000 mkdocs-alias-plugin-0.8.0/mkdocs_alias_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-06 22:50:37.000000 mkdocs-alias-plugin-0.8.0/mkdocs_alias_plugin.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-06 22:50:37.000000 mkdocs-alias-plugin-0.8.0/mkdocs_alias_plugin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-06 22:50:37.000000 mkdocs-alias-plugin-0.8.0/mkdocs_alias_plugin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 22:50:37.365961 mkdocs-alias-plugin-0.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-04-06 22:50:32.000000 mkdocs-alias-plugin-0.8.0/setup.py
```

### Comparing `mkdocs-alias-plugin-0.7.1/LICENSE.md` & `mkdocs-alias-plugin-0.8.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `mkdocs-alias-plugin-0.7.1/PKG-INFO` & `mkdocs-alias-plugin-0.8.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,12 @@
-Metadata-Version: 2.1
-Name: mkdocs-alias-plugin
-Version: 0.7.1
-Summary: An MkDocs plugin allowing links to your pages using a custom alias
-Home-page: https://github.com/eddyluten/mkdocs-alias-plugin
-Author: Eddy Luten
-Author-email: eddyluten@gmail.com
-License: MIT
-Keywords: mkdocs python markdown alias link wiki
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.0
-Description-Content-Type: text/markdown
-License-File: LICENSE.md
-Requires-Dist: mkdocs
-
 # mkdocs-alias-plugin
 
 [![PyPI version](https://badge.fury.io/py/mkdocs-alias-plugin.svg)](https://pypi.org/project/mkdocs-alias-plugin/)  [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) ![example workflow](https://github.com/eddyluten/mkdocs-alias-plugin/actions/workflows/pylint.yml/badge.svg) [![Downloads](https://pepy.tech/badge/mkdocs-alias-plugin)](https://pepy.tech/project/mkdocs-alias-plugin) ![](https://github.com/eddyluten/mkdocs-alias-plugin/workflows/mkdocs-alias-plugin%20Tests/badge.svg)
 
-An MkDocs plugin allowing links to your pages using a custom alias such as `[[my-alias]]` or `[[my-alias|My Title]]`.
+The `mkdocs-alias-plugin` MkDocs plugin allows links to your pages using a custom alias such as `[[my-alias]]` or `[[my-alias|My Title]]`.
 
 The aliases are configured through the meta-sections of each page (see Usage below).
 
 If you like this plugin, you'll probably also like [mkdocs-categories-plugin](https://github.com/EddyLuten/mkdocs-categories-plugin) and [mkdocs-live-edit-plugin](https://github.com/EddyLuten/mkdocs-live-edit-plugin).
 
 ## Rationale
 
@@ -61,60 +43,62 @@
 
 ```md
 The song references [[wuthering-heights]].
 ```
 
 Which, after the page builds, renders as a regular link to your page.
 
-Or, a more advanced example by using the dictionary-style configuration instead to provide a different link title.
+A more advanced example would be to use the dictionary-style configuration instead of providing a different link title:
 
 ```yaml
 ---
 alias:
     name: wuthering-heights
     text: Wuthering Heights, a novel by Emily Brontë
 ---
 ```
 
-If you'd like to supply your own link text instead on a link-by-link basis, you can do so using a pipe to separate the title from the alias:
+If you'd like to supply a custom link text instead on a link-by-link basis, you can do so using a pipe to separate the title from the alias:
 
 ```md
 The song references [[wuthering-heights|Wuthering Heights]].
 ```
 
 As of version 0.6.0, you can also use link anchors in your aliases:
 
 ```md
 The song references [[wuthering-heights#references]].
 ```
 
-Or, also using a title:
+Or, using a custom title:
 
 ```md
 The song references [[wuthering-heights#references|Wuthering Heights]].
 ```
 
+As of version 0.8.0, you can enable the plugin option `use_anchor_titles` to replace anchor links with the text of the page heading that defined it. This behavior is opt-in to preserve backward compatibility.
+
 Please refer to the [MkDocs documentation](https://www.mkdocs.org/user-guide/writing-your-docs/#yaml-style-meta-data) for more information on how the meta-data block is used.
 
 ### Multiple Aliases
 
-As of version 0.3.0, it is possible to assign multiple aliases to a single page. This does come with the limitation that these aliases cannot define a per-alias title. The syntax for this is:
+As of version 0.3.0, assigning multiple aliases to a single page is possible. This feature does come with the limitation that these aliases cannot define a per-alias title and instead will use the page title. The syntax for this is:
 
 ```yaml
 ---
 alias:
     - wuthering-heights
     - wuthering
     - wh
 ---
 ```
 
 ### Escaping Aliases (Escape Syntax)
 
-As of version 0.4.0, it is possible to escape aliases to prevent them being parsed by the plugin. This is useful if you use a similar double-bracket markup for a different purpose (e.g. shell scripts). The syntax for this feature is a leading backslash:
+As of version 0.4.0, it is possible to escape aliases to prevent them being parsed by the plugin. This is useful if you use a similar double-bracket markup for a different purpose (e.g. shell scripts in code blocks). The syntax for this feature is a leading backslash:
 
 ```md
 \[[this text will remain untouched]]
 
 [[this text will be parsed as an alias]]
 ```
 
@@ -122,27 +106,32 @@
 
 You may customize the plugin by passing options into the plugin's configuration sections in `mkdocs.yml`:
 
 ```yaml
 plugins:
     - alias:
         verbose: true
+        use_anchor_titles: true
 ```
 
 ### `verbose`
 
-You may use the optional `verbose` option to print more information about which aliases were used and defined during build. The default value is `false`.
+You may use the optional `verbose` option to print more information about which aliases were used and defined during the build process. The default value is `false`.
+
+### `use_anchor_titles`
+
+Setting this flag to true causes the plugin to replace an alias containing an anchor (`[[my-page#sub-heading]]`) with the text of the header that defined it. You can still override the title of the link as usual.
 
 ## Troubleshooting
 
 ### The link text looks like a path or URL
 
 Your alias doesn't have link text defined *and* your page doesn't have a title H1 tag or a `title` attribute in its meta data section. Once you add this, your link will render with the appropriate text.
 
-### My alias is not being replaced
+### My alias is not replaced
 
 `WARNING  -  Alias 'my-alias' not found`
 
 The alias could not be found in the defined aliases, usually due to a typo. Enable verbose output in the plugin's configuration to display all of the found aliases.
 
 However, it is also possible that the plugin is trying to interpret another double-bracketed syntax as an alias. In this case, use the escape syntax to prevent the plugin from parsing it.
 
@@ -172,23 +161,27 @@
 
 ```zsh
 pylint $(git ls-files '*.py') && pytest -vv
 ```
 
 ## Changelog
 
+## 0.8.0
+
+This release adds functionality to replace the titles of aliases containing anchors with the text of the heading that defines them. Enable this feature by setting the plugin option `use_anchor_titles` to true. Feature request: [#8](https://github.com/EddyLuten/mkdocs-alias-plugin/issues/8).
+
 ### 0.7.1
 
-**Bug Fix:** fixes a bug where any alias with the word "text" would break the plugin due to faulty logic. Reported in [#7](https://github.com/EddyLuten/mkdocs-alias-plugin/issues/7)
+**Bug Fix:** fixes a bug where any alias with the word "text" would break the plugin due to faulty logic. Bug report: [#7](https://github.com/EddyLuten/mkdocs-alias-plugin/issues/7).
 
 ### 0.7.0
 
 2024-02-01
 
-Removed support for the `use_relative_link` option introduced in issue #3. As of 1.5.0, MkDocs prefers relative links to absolute links, which were the default of this package before. As of this version, all alias links generated are relative to the file they were linked from.
+This release removes support for the `use_relative_link` option introduced in issue [#3](https://github.com/EddyLuten/mkdocs-alias-plugin/issues/3). As of version 1.5.0, MkDocs prefers relative links to absolute links, which was this package's default before. As of this version, all alias links generated are relative to the file from where they were linked.
 
 ### 0.6.0
 
 2023-04-17
 
 Adds support for page anchor links from within an alias. E.g.:
```

### Comparing `mkdocs-alias-plugin-0.7.1/README.md` & `mkdocs-alias-plugin-0.8.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,35 @@
+Metadata-Version: 2.1
+Name: mkdocs-alias-plugin
+Version: 0.8.0
+Summary: An MkDocs plugin allowing links to your pages using a custom alias
+Home-page: https://github.com/eddyluten/mkdocs-alias-plugin
+Author: Eddy Luten
+Author-email: eddyluten@gmail.com
+License: MIT
+Keywords: mkdocs python markdown alias link wiki
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Documentation
+Classifier: Topic :: Text Processing
+Classifier: Topic :: Text Processing :: Markup
+Classifier: Topic :: Text Processing :: Markup :: Markdown
+Requires-Python: >=3.0
+Description-Content-Type: text/markdown
+License-File: LICENSE.md
+Requires-Dist: mkdocs
+Requires-Dist: markdown
+
 # mkdocs-alias-plugin
 
 [![PyPI version](https://badge.fury.io/py/mkdocs-alias-plugin.svg)](https://pypi.org/project/mkdocs-alias-plugin/)  [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) ![example workflow](https://github.com/eddyluten/mkdocs-alias-plugin/actions/workflows/pylint.yml/badge.svg) [![Downloads](https://pepy.tech/badge/mkdocs-alias-plugin)](https://pepy.tech/project/mkdocs-alias-plugin) ![](https://github.com/eddyluten/mkdocs-alias-plugin/workflows/mkdocs-alias-plugin%20Tests/badge.svg)
 
-An MkDocs plugin allowing links to your pages using a custom alias such as `[[my-alias]]` or `[[my-alias|My Title]]`.
+The `mkdocs-alias-plugin` MkDocs plugin allows links to your pages using a custom alias such as `[[my-alias]]` or `[[my-alias|My Title]]`.
 
 The aliases are configured through the meta-sections of each page (see Usage below).
 
 If you like this plugin, you'll probably also like [mkdocs-categories-plugin](https://github.com/EddyLuten/mkdocs-categories-plugin) and [mkdocs-live-edit-plugin](https://github.com/EddyLuten/mkdocs-live-edit-plugin).
 
 ## Rationale
 
@@ -43,60 +66,62 @@
 
 ```md
 The song references [[wuthering-heights]].
 ```
 
 Which, after the page builds, renders as a regular link to your page.
 
-Or, a more advanced example by using the dictionary-style configuration instead to provide a different link title.
+A more advanced example would be to use the dictionary-style configuration instead of providing a different link title:
 
 ```yaml
 ---
 alias:
     name: wuthering-heights
     text: Wuthering Heights, a novel by Emily Brontë
 ---
 ```
 
-If you'd like to supply your own link text instead on a link-by-link basis, you can do so using a pipe to separate the title from the alias:
+If you'd like to supply a custom link text instead on a link-by-link basis, you can do so using a pipe to separate the title from the alias:
 
 ```md
 The song references [[wuthering-heights|Wuthering Heights]].
 ```
 
 As of version 0.6.0, you can also use link anchors in your aliases:
 
 ```md
 The song references [[wuthering-heights#references]].
 ```
 
-Or, also using a title:
+Or, using a custom title:
 
 ```md
 The song references [[wuthering-heights#references|Wuthering Heights]].
 ```
 
+As of version 0.8.0, you can enable the plugin option `use_anchor_titles` to replace anchor links with the text of the page heading that defined it. This behavior is opt-in to preserve backward compatibility.
+
 Please refer to the [MkDocs documentation](https://www.mkdocs.org/user-guide/writing-your-docs/#yaml-style-meta-data) for more information on how the meta-data block is used.
 
 ### Multiple Aliases
 
-As of version 0.3.0, it is possible to assign multiple aliases to a single page. This does come with the limitation that these aliases cannot define a per-alias title. The syntax for this is:
+As of version 0.3.0, assigning multiple aliases to a single page is possible. This feature does come with the limitation that these aliases cannot define a per-alias title and instead will use the page title. The syntax for this is:
 
 ```yaml
 ---
 alias:
     - wuthering-heights
     - wuthering
     - wh
 ---
 ```
 
 ### Escaping Aliases (Escape Syntax)
 
-As of version 0.4.0, it is possible to escape aliases to prevent them being parsed by the plugin. This is useful if you use a similar double-bracket markup for a different purpose (e.g. shell scripts). The syntax for this feature is a leading backslash:
+As of version 0.4.0, it is possible to escape aliases to prevent them being parsed by the plugin. This is useful if you use a similar double-bracket markup for a different purpose (e.g. shell scripts in code blocks). The syntax for this feature is a leading backslash:
 
 ```md
 \[[this text will remain untouched]]
 
 [[this text will be parsed as an alias]]
 ```
 
@@ -104,27 +129,32 @@
 
 You may customize the plugin by passing options into the plugin's configuration sections in `mkdocs.yml`:
 
 ```yaml
 plugins:
     - alias:
         verbose: true
+        use_anchor_titles: true
 ```
 
 ### `verbose`
 
-You may use the optional `verbose` option to print more information about which aliases were used and defined during build. The default value is `false`.
+You may use the optional `verbose` option to print more information about which aliases were used and defined during the build process. The default value is `false`.
+
+### `use_anchor_titles`
+
+Setting this flag to true causes the plugin to replace an alias containing an anchor (`[[my-page#sub-heading]]`) with the text of the header that defined it. You can still override the title of the link as usual.
 
 ## Troubleshooting
 
 ### The link text looks like a path or URL
 
 Your alias doesn't have link text defined *and* your page doesn't have a title H1 tag or a `title` attribute in its meta data section. Once you add this, your link will render with the appropriate text.
 
-### My alias is not being replaced
+### My alias is not replaced
 
 `WARNING  -  Alias 'my-alias' not found`
 
 The alias could not be found in the defined aliases, usually due to a typo. Enable verbose output in the plugin's configuration to display all of the found aliases.
 
 However, it is also possible that the plugin is trying to interpret another double-bracketed syntax as an alias. In this case, use the escape syntax to prevent the plugin from parsing it.
 
@@ -154,23 +184,27 @@
 
 ```zsh
 pylint $(git ls-files '*.py') && pytest -vv
 ```
 
 ## Changelog
 
+## 0.8.0
+
+This release adds functionality to replace the titles of aliases containing anchors with the text of the heading that defines them. Enable this feature by setting the plugin option `use_anchor_titles` to true. Feature request: [#8](https://github.com/EddyLuten/mkdocs-alias-plugin/issues/8).
+
 ### 0.7.1
 
-**Bug Fix:** fixes a bug where any alias with the word "text" would break the plugin due to faulty logic. Reported in [#7](https://github.com/EddyLuten/mkdocs-alias-plugin/issues/7)
+**Bug Fix:** fixes a bug where any alias with the word "text" would break the plugin due to faulty logic. Bug report: [#7](https://github.com/EddyLuten/mkdocs-alias-plugin/issues/7).
 
 ### 0.7.0
 
 2024-02-01
 
-Removed support for the `use_relative_link` option introduced in issue #3. As of 1.5.0, MkDocs prefers relative links to absolute links, which were the default of this package before. As of this version, all alias links generated are relative to the file they were linked from.
+This release removes support for the `use_relative_link` option introduced in issue [#3](https://github.com/EddyLuten/mkdocs-alias-plugin/issues/3). As of version 1.5.0, MkDocs prefers relative links to absolute links, which was this package's default before. As of this version, all alias links generated are relative to the file from where they were linked.
 
 ### 0.6.0
 
 2023-04-17
 
 Adds support for page anchor links from within an alias. E.g.:
```

### Comparing `mkdocs-alias-plugin-0.7.1/alias/plugin.py` & `mkdocs-alias-plugin-0.8.0/alias/plugin.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,51 +1,89 @@
 """mkdocs-alias-plugin
 
 An MkDocs plugin allowing links to your pages using a custom alias.
 """
 
 import logging
 import re
-from typing import Match
-from mkdocs.structure.files import File
-from mkdocs.plugins import BasePlugin
-from mkdocs.utils import meta, get_markdown_title, get_relative_url
+from typing import Match, TypedDict
+
+from markdown import Markdown
 from mkdocs.config import config_options
+from mkdocs.plugins import BasePlugin
+from mkdocs.structure.files import File, Files
+from mkdocs.structure.pages import Page
+from mkdocs.utils import get_markdown_title, get_relative_url, meta
 
 # The Regular Expression used to find alias tags
+# group 1: escape character
+# group 2: alias name
+# group 3: alias text
 ALIAS_TAG_REGEX = r"([\\])?\[\[([^|\]]+)\|?([^\]]+)?\]\]"
 
+
+class MarkdownAnchor(TypedDict):
+    """A single entry in the table of contents. See the following link for more info:
+    https://python-markdown.github.io/extensions/toc/#syntax"""
+    level: int
+    id: str
+    name: str
+    children: list['MarkdownAnchor']
+
+
+def get_markdown_toc(markdown_source) -> list[MarkdownAnchor]:
+    """Parse the markdown source and return the table of contents tokens."""
+    md = Markdown(extensions=['toc'])
+    md.convert(markdown_source)
+    return getattr(md, 'toc_tokens', [])
+
+
+def find_anchor_by_id(anchors: list[MarkdownAnchor], anchor_id: str) -> MarkdownAnchor | None:
+    """Find an anchor by its ID in a list of anchors returned by get_markdown_toc."""
+    for anchor in anchors:
+        if anchor['id'] == anchor_id:
+            return anchor
+        if 'children' in anchor:
+            child = find_anchor_by_id(anchor['children'], anchor_id)
+            if child is not None:
+                return child
+    return None
+
+
 def get_page_title(page_src: str, meta_data: dict):
     """Returns the title of the page. The title in the meta data section
     will take precedence over the H1 markdown title if both are provided."""
     return (
         meta_data['title']
         if 'title' in meta_data and isinstance(meta_data['title'], str)
         else get_markdown_title(page_src)
     )
 
+
 def get_alias_names(meta_data: dict):
     """Returns the list of configured alias names."""
     if len(meta_data) <= 0 or 'alias' not in meta_data:
         return None
     aliases = meta_data['alias']
     if isinstance(aliases, list):
         # If the alias meta data is a list, ensure that they're strings
         return list(filter(lambda value: isinstance(value, str), aliases))
     if isinstance(aliases, dict) and 'name' in aliases:
-        return [ aliases['name'] ]
+        return [aliases['name']]
     if isinstance(aliases, str):
-        return [ aliases ]
+        return [aliases]
     return None
 
+
 def replace_tag(
     match: Match,
     aliases: dict,
     log: logging.Logger,
-    page_file: File
+    page_file: File,
+    use_anchor_titles: bool = False
 ):
     """Callback used in the sub function within on_page_markdown."""
     if match.group(1) is not None:
         # if the alias match was escaped, return the unescaped version
         return match.group(0)[1:]
     # split the tag up in case there's an anchor in the link
     tag_bits = ['']
@@ -54,44 +92,57 @@
     alias = aliases.get(tag_bits[0])
     if alias is None:
         log.warning(
             "Alias '%s' not found in '%s'",
             match.group(2),
             page_file.src_path
         )
-        return match.group(0) # return the input string
+        return match.group(0)  # return the input string
 
-    text = alias['text'] if match.group(3) is None else match.group(3)
+    text = None
+    anchor = tag_bits[1] if len(tag_bits) > 1 else None
+    # if the use_anchor_titles config option is set, replace the text with the
+    # anchor title, but only if the alias tag doesn't have a custom text
+    if use_anchor_titles and anchor is not None and match.group(3) is None:
+        anchor_tag = find_anchor_by_id(alias['anchors'], anchor)
+        if anchor_tag is not None:
+            text = anchor_tag['name']
+    if text is None:
+        # if the alias tag has a custom text, use that instead
+        text = alias['text'] if match.group(3) is None else match.group(3)
+    # if the alias tag has no text, use the alias URL
     if text is None:
         text = alias['url']
 
     url = get_relative_url(alias['url'], page_file.src_uri)
-    if len(tag_bits) > 1:
+    if anchor is not None:
         url = f"{url}#{tag_bits[1]}"
 
     log.info(
         "replaced alias '%s' with '%s' to '%s'",
         alias['alias'],
         text,
         url
     )
     return f"[{text}]({url})"
 
+
 class AliasPlugin(BasePlugin):
     """An extension of BasePlugin providing all of the aliasing logic.
 
     The plugin works by reading all of the markdown files before they are
     processed and parsing their meta sections.
 
     See on_files() for more info.
 
     For overridden BasePlugin methods, see the MkDocs source code.
     """
     config_scheme = (
         ('verbose', config_options.Type(bool, default=False)),
+        ('use_anchor_titles', config_options.Type(bool, default=False)),
     )
     aliases = {}
     log = logging.getLogger(f'mkdocs.plugins.{__name__}')
     current_page = None
 
     def on_config(self, _):
         """Set the log level if the verbose config option is set"""
@@ -102,39 +153,46 @@
     def on_post_build(self, **_):
         """Executed after the build has completed. Clears the aliases from
         memory and displays stats if the verbose option is configured.
         """
         self.log.info("Defined %s alias(es).", len(self.aliases))
         self.aliases.clear()
 
-    def on_page_markdown(self, markdown: str, *, page, **_):
+    def on_page_markdown(self, markdown: str, *, page: Page, **_):
         """Replaces any alias tags on the page with markdown links."""
         self.current_page = page
         return re.sub(
             ALIAS_TAG_REGEX,
             lambda match: replace_tag(
                 match,
                 self.aliases,
                 self.log,
-                self.current_page.file
+                self.current_page.file,
+                self.config['use_anchor_titles']
             ),
             markdown
         )
 
-    def on_files(self, files, **_):
+    def on_files(self, files: Files, **_):
         """When MkDocs loads its files, extract aliases from any Markdown files
         that were found.
         """
         for file in filter(lambda f: f.is_documentation_page(), files):
             with open(file.abs_src_path, encoding='utf-8-sig', errors='strict') as handle:
                 source, meta_data = meta.get_data(handle.read())
                 alias_names = get_alias_names(meta_data)
                 if alias_names is None or len(alias_names) < 1:
                     continue
 
+                # If the use_anchor_titles config option is set, parse the markdown
+                # and get the table of contents for the page
+                anchors: list[MarkdownAnchor] = []
+                if self.config['use_anchor_titles']:
+                    anchors = get_markdown_toc(source)
+
                 if len(alias_names) > 1:
                     self.log.info(
                         '%s defines %d aliases:', file.url, len(alias_names)
                     )
                 for alias in alias_names:
                     existing = self.aliases.get(alias)
                     if existing is not None:
@@ -151,14 +209,15 @@
                         'text': (
                             meta_data['alias']['text']
                             # if meta_data['alias'] is a dictionary and 'text' is a key
                             if isinstance(meta_data['alias'], dict) and 'text' in meta_data['alias']
                             else get_page_title(source, meta_data)
                         ),
                         'url': file.src_uri,
+                        'anchors': anchors,
                     }
                     self.log.info(
                         "Alias %s to %s",
                         alias,
                         new_alias['url']
                     )
                     self.aliases[alias] = new_alias
```

### Comparing `mkdocs-alias-plugin-0.7.1/mkdocs_alias_plugin.egg-info/PKG-INFO` & `mkdocs-alias-plugin-0.8.0/mkdocs_alias_plugin.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,35 @@
 Metadata-Version: 2.1
 Name: mkdocs-alias-plugin
-Version: 0.7.1
+Version: 0.8.0
 Summary: An MkDocs plugin allowing links to your pages using a custom alias
 Home-page: https://github.com/eddyluten/mkdocs-alias-plugin
 Author: Eddy Luten
 Author-email: eddyluten@gmail.com
 License: MIT
 Keywords: mkdocs python markdown alias link wiki
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Documentation
+Classifier: Topic :: Text Processing
+Classifier: Topic :: Text Processing :: Markup
+Classifier: Topic :: Text Processing :: Markup :: Markdown
 Requires-Python: >=3.0
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: mkdocs
+Requires-Dist: markdown
 
 # mkdocs-alias-plugin
 
 [![PyPI version](https://badge.fury.io/py/mkdocs-alias-plugin.svg)](https://pypi.org/project/mkdocs-alias-plugin/)  [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) ![example workflow](https://github.com/eddyluten/mkdocs-alias-plugin/actions/workflows/pylint.yml/badge.svg) [![Downloads](https://pepy.tech/badge/mkdocs-alias-plugin)](https://pepy.tech/project/mkdocs-alias-plugin) ![](https://github.com/eddyluten/mkdocs-alias-plugin/workflows/mkdocs-alias-plugin%20Tests/badge.svg)
 
-An MkDocs plugin allowing links to your pages using a custom alias such as `[[my-alias]]` or `[[my-alias|My Title]]`.
+The `mkdocs-alias-plugin` MkDocs plugin allows links to your pages using a custom alias such as `[[my-alias]]` or `[[my-alias|My Title]]`.
 
 The aliases are configured through the meta-sections of each page (see Usage below).
 
 If you like this plugin, you'll probably also like [mkdocs-categories-plugin](https://github.com/EddyLuten/mkdocs-categories-plugin) and [mkdocs-live-edit-plugin](https://github.com/EddyLuten/mkdocs-live-edit-plugin).
 
 ## Rationale
 
@@ -61,60 +66,62 @@
 
 ```md
 The song references [[wuthering-heights]].
 ```
 
 Which, after the page builds, renders as a regular link to your page.
 
-Or, a more advanced example by using the dictionary-style configuration instead to provide a different link title.
+A more advanced example would be to use the dictionary-style configuration instead of providing a different link title:
 
 ```yaml
 ---
 alias:
     name: wuthering-heights
     text: Wuthering Heights, a novel by Emily Brontë
 ---
 ```
 
-If you'd like to supply your own link text instead on a link-by-link basis, you can do so using a pipe to separate the title from the alias:
+If you'd like to supply a custom link text instead on a link-by-link basis, you can do so using a pipe to separate the title from the alias:
 
 ```md
 The song references [[wuthering-heights|Wuthering Heights]].
 ```
 
 As of version 0.6.0, you can also use link anchors in your aliases:
 
 ```md
 The song references [[wuthering-heights#references]].
 ```
 
-Or, also using a title:
+Or, using a custom title:
 
 ```md
 The song references [[wuthering-heights#references|Wuthering Heights]].
 ```
 
+As of version 0.8.0, you can enable the plugin option `use_anchor_titles` to replace anchor links with the text of the page heading that defined it. This behavior is opt-in to preserve backward compatibility.
+
 Please refer to the [MkDocs documentation](https://www.mkdocs.org/user-guide/writing-your-docs/#yaml-style-meta-data) for more information on how the meta-data block is used.
 
 ### Multiple Aliases
 
-As of version 0.3.0, it is possible to assign multiple aliases to a single page. This does come with the limitation that these aliases cannot define a per-alias title. The syntax for this is:
+As of version 0.3.0, assigning multiple aliases to a single page is possible. This feature does come with the limitation that these aliases cannot define a per-alias title and instead will use the page title. The syntax for this is:
 
 ```yaml
 ---
 alias:
     - wuthering-heights
     - wuthering
     - wh
 ---
 ```
 
 ### Escaping Aliases (Escape Syntax)
 
-As of version 0.4.0, it is possible to escape aliases to prevent them being parsed by the plugin. This is useful if you use a similar double-bracket markup for a different purpose (e.g. shell scripts). The syntax for this feature is a leading backslash:
+As of version 0.4.0, it is possible to escape aliases to prevent them being parsed by the plugin. This is useful if you use a similar double-bracket markup for a different purpose (e.g. shell scripts in code blocks). The syntax for this feature is a leading backslash:
 
 ```md
 \[[this text will remain untouched]]
 
 [[this text will be parsed as an alias]]
 ```
 
@@ -122,27 +129,32 @@
 
 You may customize the plugin by passing options into the plugin's configuration sections in `mkdocs.yml`:
 
 ```yaml
 plugins:
     - alias:
         verbose: true
+        use_anchor_titles: true
 ```
 
 ### `verbose`
 
-You may use the optional `verbose` option to print more information about which aliases were used and defined during build. The default value is `false`.
+You may use the optional `verbose` option to print more information about which aliases were used and defined during the build process. The default value is `false`.
+
+### `use_anchor_titles`
+
+Setting this flag to true causes the plugin to replace an alias containing an anchor (`[[my-page#sub-heading]]`) with the text of the header that defined it. You can still override the title of the link as usual.
 
 ## Troubleshooting
 
 ### The link text looks like a path or URL
 
 Your alias doesn't have link text defined *and* your page doesn't have a title H1 tag or a `title` attribute in its meta data section. Once you add this, your link will render with the appropriate text.
 
-### My alias is not being replaced
+### My alias is not replaced
 
 `WARNING  -  Alias 'my-alias' not found`
 
 The alias could not be found in the defined aliases, usually due to a typo. Enable verbose output in the plugin's configuration to display all of the found aliases.
 
 However, it is also possible that the plugin is trying to interpret another double-bracketed syntax as an alias. In this case, use the escape syntax to prevent the plugin from parsing it.
 
@@ -172,23 +184,27 @@
 
 ```zsh
 pylint $(git ls-files '*.py') && pytest -vv
 ```
 
 ## Changelog
 
+## 0.8.0
+
+This release adds functionality to replace the titles of aliases containing anchors with the text of the heading that defines them. Enable this feature by setting the plugin option `use_anchor_titles` to true. Feature request: [#8](https://github.com/EddyLuten/mkdocs-alias-plugin/issues/8).
+
 ### 0.7.1
 
-**Bug Fix:** fixes a bug where any alias with the word "text" would break the plugin due to faulty logic. Reported in [#7](https://github.com/EddyLuten/mkdocs-alias-plugin/issues/7)
+**Bug Fix:** fixes a bug where any alias with the word "text" would break the plugin due to faulty logic. Bug report: [#7](https://github.com/EddyLuten/mkdocs-alias-plugin/issues/7).
 
 ### 0.7.0
 
 2024-02-01
 
-Removed support for the `use_relative_link` option introduced in issue #3. As of 1.5.0, MkDocs prefers relative links to absolute links, which were the default of this package before. As of this version, all alias links generated are relative to the file they were linked from.
+This release removes support for the `use_relative_link` option introduced in issue [#3](https://github.com/EddyLuten/mkdocs-alias-plugin/issues/3). As of version 1.5.0, MkDocs prefers relative links to absolute links, which was this package's default before. As of this version, all alias links generated are relative to the file from where they were linked.
 
 ### 0.6.0
 
 2023-04-17
 
 Adds support for page anchor links from within an alias. E.g.:
```

### Comparing `mkdocs-alias-plugin-0.7.1/setup.py` & `mkdocs-alias-plugin-0.8.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,29 +3,33 @@
 from setuptools import setup, find_packages
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name='mkdocs-alias-plugin',
-    version='0.7.1',
+    version='0.8.0',
     description=
     'An MkDocs plugin allowing links to your pages using a custom alias',
     long_description=long_description,
     long_description_content_type='text/markdown',
     keywords='mkdocs python markdown alias link wiki',
     url='https://github.com/eddyluten/mkdocs-alias-plugin',
     author='Eddy Luten',
     author_email='eddyluten@gmail.com',
     license='MIT',
     python_requires='>=3.0',
-    install_requires=['mkdocs'],
+    install_requires=['mkdocs', 'markdown'],
     classifiers=[
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3 :: Only',
         'Topic :: Software Development :: Libraries :: Python Modules',
+        "Topic :: Documentation",
+        "Topic :: Text Processing",
+        "Topic :: Text Processing :: Markup",
+        "Topic :: Text Processing :: Markup :: Markdown",
     ],
     packages=find_packages(exclude=['*.tests']),
     entry_points={
         'mkdocs.plugins': ['alias = alias.plugin:AliasPlugin']
     })
```

