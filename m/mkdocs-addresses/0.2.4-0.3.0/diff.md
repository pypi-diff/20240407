# Comparing `tmp/mkdocs_addresses-0.2.4.tar.gz` & `tmp/mkdocs_addresses-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs_addresses-0.2.4.tar", max compression
+gzip compressed data, was "mkdocs_addresses-0.3.0.tar", max compression
```

## Comparing `mkdocs_addresses-0.2.4.tar` & `mkdocs_addresses-0.3.0.tar`

### file list

```diff
@@ -1,25 +1,28 @@
--rw-r--r--   0        0        0   303056 2023-09-20 13:11:14.726464 mkdocs_addresses-0.2.4/LICENSE.md
--rw-r--r--   0        0        0     6883 2023-09-21 08:31:37.887971 mkdocs_addresses-0.2.4/README.md
--rwxr-xr-x   0        0        0      103 2023-07-31 20:53:55.753679 mkdocs_addresses-0.2.4/mkdocs_addresses/__init__.py
--rw-r--r--   0        0        0       22 2023-09-21 08:35:12.802294 mkdocs_addresses-0.2.4/mkdocs_addresses/__version__.py
--rw-r--r--   0        0        0    12869 2023-09-06 08:35:03.857149 mkdocs_addresses-0.2.4/mkdocs_addresses/addresses_checker.py
--rw-r--r--   0        0        0    35457 2023-09-20 13:11:14.890469 mkdocs_addresses-0.2.4/mkdocs_addresses/addresses_plugin.py
--rw-r--r--   0        0        0     5902 2023-09-20 13:11:14.898469 mkdocs_addresses-0.2.4/mkdocs_addresses/auto_completion_handler.py
--rw-r--r--   0        0        0    23008 2023-09-20 13:11:14.914470 mkdocs_addresses-0.2.4/mkdocs_addresses/config_plugin.py
--rw-r--r--   0        0        0     4482 2023-09-20 18:40:27.867386 mkdocs_addresses-0.2.4/mkdocs_addresses/exceptions.py
--rw-r--r--   0        0        0     7960 2023-08-27 13:53:48.856771 mkdocs_addresses-0.2.4/mkdocs_addresses/logger.py
--rw-r--r--   0        0        0        0 2023-08-27 13:53:48.856771 mkdocs_addresses-0.2.4/mkdocs_addresses/other_plugins_handling/__init__.py
--rw-r--r--   0        0        0     1683 2023-08-27 13:53:48.856771 mkdocs_addresses-0.2.4/mkdocs_addresses/other_plugins_handling/autorefs.py
--rw-r--r--   0        0        0     1897 2023-08-27 13:53:48.856771 mkdocs_addresses-0.2.4/mkdocs_addresses/path_manager.py
--rw-r--r--   0        0        0     5260 2023-08-27 13:53:48.856771 mkdocs_addresses-0.2.4/mkdocs_addresses/soup_excluding_codes.py
--rw-r--r--   0        0        0      692 2023-08-27 13:53:48.856771 mkdocs_addresses-0.2.4/mkdocs_addresses/static_handler/__init__.py
--rw-r--r--   0        0        0     1965 2023-08-27 13:53:48.856771 mkdocs_addresses-0.2.4/mkdocs_addresses/static_handler/files_tracker.py
--rw-r--r--   0        0        0    16977 2023-09-21 08:35:12.754292 mkdocs_addresses-0.2.4/mkdocs_addresses/static_handler/static_handler.py
--rw-r--r--   0        0        0     2525 2023-08-27 13:53:48.860771 mkdocs_addresses-0.2.4/mkdocs_addresses/static_handler/tracker_addresses_usage_pool.py
--rw-r--r--   0        0        0     5805 2023-08-27 13:53:48.860771 mkdocs_addresses-0.2.4/mkdocs_addresses/static_handler/tracker_data_pages.py
--rw-r--r--   0        0        0     2228 2023-09-20 13:11:14.914470 mkdocs_addresses-0.2.4/mkdocs_addresses/static_handler/tracker_errors_counter.py
--rw-r--r--   0        0        0     6171 2023-08-27 13:53:48.860771 mkdocs_addresses-0.2.4/mkdocs_addresses/static_handler/tracker_references.py
--rw-r--r--   0        0        0      712 2023-08-27 13:53:48.860771 mkdocs_addresses-0.2.4/mkdocs_addresses/static_handler/types_aliases.py
--rw-r--r--   0        0        0      629 2023-08-27 13:53:48.864771 mkdocs_addresses-0.2.4/mkdocs_addresses/toolbox.py
--rw-r--r--   0        0        0     2024 2023-09-21 08:35:12.754292 mkdocs_addresses-0.2.4/pyproject.toml
--rw-r--r--   0        0        0     8340 1970-01-01 00:00:00.000000 mkdocs_addresses-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0   303056 2024-04-07 13:02:30.042002 mkdocs_addresses-0.3.0/LICENSE.md
+-rw-r--r--   0        0        0     6870 2024-04-07 13:19:35.416233 mkdocs_addresses-0.3.0/README.md
+-rw-r--r--   0        0        0      141 2024-04-07 13:02:30.158005 mkdocs_addresses-0.3.0/mkdocs_addresses/__init__.py
+-rw-r--r--   0        0        0       22 2024-04-07 13:27:46.314691 mkdocs_addresses-0.3.0/mkdocs_addresses/__version__.py
+-rw-r--r--   0        0        0    12859 2024-04-07 13:02:30.158005 mkdocs_addresses-0.3.0/mkdocs_addresses/addresses_checker.py
+-rw-r--r--   0        0        0    35160 2024-04-07 13:02:30.178006 mkdocs_addresses-0.3.0/mkdocs_addresses/addresses_plugin.py
+-rw-r--r--   0        0        0     1826 2024-04-07 13:02:30.242007 mkdocs_addresses-0.3.0/mkdocs_addresses/auto_completion_handler/__init__.py
+-rw-r--r--   0        0        0     3851 2024-04-07 13:02:30.278009 mkdocs_addresses-0.3.0/mkdocs_addresses/auto_completion_handler/_base_handler.py
+-rw-r--r--   0        0        0     1273 2024-04-07 13:02:30.278009 mkdocs_addresses-0.3.0/mkdocs_addresses/auto_completion_handler/_no_completion_handler.py
+-rw-r--r--   0        0        0     4173 2024-04-07 13:02:30.290009 mkdocs_addresses-0.3.0/mkdocs_addresses/auto_completion_handler/_vsc_handlers.py
+-rw-r--r--   0        0        0    24827 2024-04-07 13:02:30.290009 mkdocs_addresses-0.3.0/mkdocs_addresses/config_plugin.py
+-rw-r--r--   0        0        0     4482 2023-09-21 08:35:25.358662 mkdocs_addresses-0.3.0/mkdocs_addresses/exceptions.py
+-rw-r--r--   0        0        0     8074 2024-04-07 13:02:30.298009 mkdocs_addresses-0.3.0/mkdocs_addresses/logger.py
+-rw-r--r--   0        0        0        0 2023-08-27 13:53:48.856771 mkdocs_addresses-0.3.0/mkdocs_addresses/other_plugins_handling/__init__.py
+-rw-r--r--   0        0        0     1663 2024-04-07 13:02:30.310009 mkdocs_addresses-0.3.0/mkdocs_addresses/other_plugins_handling/autorefs.py
+-rw-r--r--   0        0        0     1897 2023-08-27 13:53:48.856771 mkdocs_addresses-0.3.0/mkdocs_addresses/path_manager.py
+-rw-r--r--   0        0        0     5260 2023-08-27 13:53:48.856771 mkdocs_addresses-0.3.0/mkdocs_addresses/soup_excluding_codes.py
+-rw-r--r--   0        0        0      692 2023-08-27 13:53:48.856771 mkdocs_addresses-0.3.0/mkdocs_addresses/static_handler/__init__.py
+-rw-r--r--   0        0        0     1965 2023-08-27 13:53:48.856771 mkdocs_addresses-0.3.0/mkdocs_addresses/static_handler/files_tracker.py
+-rw-r--r--   0        0        0    17190 2024-04-07 13:27:46.270689 mkdocs_addresses-0.3.0/mkdocs_addresses/static_handler/static_handler.py
+-rw-r--r--   0        0        0     2525 2023-08-27 13:53:48.860771 mkdocs_addresses-0.3.0/mkdocs_addresses/static_handler/tracker_addresses_usage_pool.py
+-rw-r--r--   0        0        0     5805 2023-08-27 13:53:48.860771 mkdocs_addresses-0.3.0/mkdocs_addresses/static_handler/tracker_data_pages.py
+-rw-r--r--   0        0        0     2228 2023-09-20 13:11:14.914470 mkdocs_addresses-0.3.0/mkdocs_addresses/static_handler/tracker_errors_counter.py
+-rw-r--r--   0        0        0     5628 2024-04-07 13:02:30.342010 mkdocs_addresses-0.3.0/mkdocs_addresses/static_handler/tracker_references.py
+-rw-r--r--   0        0        0      712 2023-08-27 13:53:48.860771 mkdocs_addresses-0.3.0/mkdocs_addresses/static_handler/types_aliases.py
+-rw-r--r--   0        0        0      492 2024-04-07 13:02:30.342010 mkdocs_addresses-0.3.0/mkdocs_addresses/toolbox.py
+-rw-r--r--   0        0        0     2013 2024-04-07 13:22:55.886145 mkdocs_addresses-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     8327 1970-01-01 00:00:00.000000 mkdocs_addresses-0.3.0/PKG-INFO
```

### Comparing `mkdocs_addresses-0.2.4/LICENSE.md` & `mkdocs_addresses-0.3.0/LICENSE.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 mkdocs-addresses
-0.2.3
+0.3.0
 FreeBSD License
 Copyright (c) 2022 Frédéric Zinelli, All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are
 met:
```

### Comparing `mkdocs_addresses-0.2.4/README.md` & `mkdocs_addresses-0.3.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
-![coverage badge](https://gitlab.com/frederic.zinelli/mkdocs-addresses/badges/main/pipeline.svg) ![coverage badge](https://gitlab.com/frederic.zinelli/mkdocs-addresses/badges/main/coverage.svg)
+![coverage badge](https://gitlab.com/frederic-zinelli/mkdocs-addresses/badges/main/pipeline.svg) ![coverage badge](https://gitlab.com/frederic-zinelli/mkdocs-addresses/badges/main/coverage.svg)
 
 
 ## Links
 
-* [Project repository (GitLab)](https://gitlab.com/frederic.zinelli/mkdocs-addresses)
-* [Full online documentation](http://frederic.zinelli.gitlab.io/mkdocs-addresses/)
+* [Project repository (GitLab)](https://gitlab.com/frederic-zinelli/mkdocs-addresses)
+* [Full online documentation](http://frederic-zinelli.gitlab.io/mkdocs-addresses/)
 * [The project on PyPI](https://pypi.org/project/mkdocs-addresses/)
 
 
 
 ## Dependencies
 
 * Python 3.8+
@@ -60,18 +60,18 @@
 
 Identifiers still work after:
 - Changing header content
 - Moving sections from one file to another
 - Renaming files
 - Moving files
 
-![move-deeper](http://frederic.zinelli.gitlab.io/mkdocs-addresses/assets/move-deeper.png)
+![move-deeper](http://frederic-zinelli.gitlab.io/mkdocs-addresses/assets/move-deeper.png)
 
 
-### Provide [autocompletion helpers](http://frederic.zinelli.gitlab.io/mkdocs-addresses/autocompletion/) (_IDE dependent_)
+### Provide [autocompletion helpers](http://frederic-zinelli.gitlab.io/mkdocs-addresses/autocompletion/) (_IDE dependent_)
 
 _(Currently only available for VSC-like IDEs)_
 
 * All snippets are automatically kept up to date while working on the documentation.
 * They provide various markdown snippets, to get a quick and easy access to all the references defined in the documentation, and use them within the markdown code they are usual used for.
 
 | Kind | Suggestion completion | Inserted markdown |
@@ -82,37 +82,37 @@
 | Images in `assets/` | `Img.file_in_assets_jpg` | `![alt content](!!file_in_assets_jpg)` |
 | Other files links | `++file_path_in_docs_html` | `++file_path_in_docs_html` |
 | Other files links | `File.file_path_in_docs_html` | `[link to a file](++file_path_in_docs_html)` |
 | External Links <sup>\*</sup> | `Ext.global_ref` | `[global_ref][global_ref]` |
 | Code inclusions<sup>\*\*</sup> | `::md that_file_md` | `--<8-- "include/that_file.md"` |
 
 
-\*: requires an [external_links_file](http://frederic.zinelli.gitlab.io/mkdocs-addresses/configuration/#mkdocs_addresses.config_plugin.PluginOptions.external_links_file) for global references is configured.
+\*: requires an [external_links_file](http://frederic-zinelli.gitlab.io/mkdocs-addresses/configuration/#mkdocs_addresses.config_plugin.PluginOptions.external_links_file) for global references is configured.
 
-\*\*: requires the use of [inclusions](http://frederic.zinelli.gitlab.io/mkdocs-addresses/configuration/#mkdocs_addresses.config_plugin.PluginOptions.inclusions) directories.
+\*\*: requires the use of [inclusions](http://frederic-zinelli.gitlab.io/mkdocs-addresses/configuration/#mkdocs_addresses.config_plugin.PluginOptions.inclusions) directories.
 
 
 ![autocomplete](docs/assets/auto-completion-point-here.png)
 
 
 
 ### Tracking dead links or addresses in the docs
 
 The plugin also explores the documentation and warns you if it finds invalid addresses or identifiers. This works for:
 
 - Addresses in links
 - Addresses of images
 - Identifiers used by the plugin
 
-![errors-example](http://frederic.zinelli.gitlab.io/mkdocs-addresses/assets/errors-summary.png)
+![errors-example](http://frederic-zinelli.gitlab.io/mkdocs-addresses/assets/errors-summary.png)
 
 
 ### User handed configuration
 
-A lot of [options](http://frederic.zinelli.gitlab.io/mkdocs-addresses/configuration/) are available for the user to fine tune the plugin's behavior.
+A lot of [options](http://frederic-zinelli.gitlab.io/mkdocs-addresses/configuration/) are available for the user to fine tune the plugin's behavior.
 
 
 
 
 
 ## Installation
 
@@ -133,15 +133,15 @@
 Configure the plugin (see below).
 
 
 
 
 ### Recommended `mkdocs.yml` configuration
 
-See the [online documentation](http://frederic.zinelli.gitlab.io/mkdocs-addresses/#installation) for more details.
+See the [online documentation](http://frederic-zinelli.gitlab.io/mkdocs-addresses/#installation) for more details.
 
 #### Markdown extensions
 
 ```yaml
 markdown_extensions:
     - attr_list             # To define the identifiers in the markdown content
     - pymdownx.snippets:    # If you need inclusions code snippets
@@ -164,17 +164,17 @@
 
 Note that the default configuration also implies the following choices:
 
 ```yaml
         - dump_snippets_file: .vscode/links.code-snippets
         - fail_fast: false
         - ignore_auto_headers: true
-        - use_vsc: true
+        - ide: vsc
 ```
-So, if VSC isn't the utilized IDE, the [`use_vsc`](http://frederic.zinelli.gitlab.io/mkdocs-addresses/configuration/#mkdocs_addresses.config_plugin.PluginOptions.use_vsc) option should at the very least be modified.
+So, if VSC isn't the utilized IDE, the [`ide`](http://frederic-zinelli.gitlab.io/mkdocs-addresses/configuration/#mkdocs_addresses.config_plugin.PluginOptions.ide) option should at the very least be modified.
 
 
 #### When using mkdocs 1.5+
 
 Significant enhancements in address verification logic (which was notoriously lacking in earlier versions...) have been added in `mkdocs 1.5+`. But the plugin does more work, and the identifiers it is utilizing are generating warnings in the console.
 
 Hence, deactivate the default verification logic for mkdocs 1.5+:
@@ -184,16 +184,16 @@
     absolute_links: ignore
     unrecognized_links: ignore
 ```
 
 
 ## Links
 
-* [Project repository (GitLab)](https://gitlab.com/frederic.zinelli/mkdocs-addresses)
-* [Full online documentation](http://frederic.zinelli.gitlab.io/mkdocs-addresses/)
+* [Project repository (GitLab)](https://gitlab.com/frederic-zinelli/mkdocs-addresses)
+* [Full online documentation](http://frederic-zinelli.gitlab.io/mkdocs-addresses/)
 * [The project on PyPI](https://pypi.org/project/mkdocs-addresses/)
 
 
 ## License
 
 [Apache-2.0](https://www.tldrlegal.com/license/apache-license-2-0-apache-2-0)
 Copyright © 2023 Zinelli Frédéric
```

### Comparing `mkdocs_addresses-0.2.4/mkdocs_addresses/addresses_checker.py` & `mkdocs_addresses-0.3.0/mkdocs_addresses/addresses_checker.py`

 * *Files 0% similar despite different names*

```diff
@@ -210,15 +210,15 @@
         else:
             checker.__validate_with_docs_as_html()
 
 
 
     def __validate_anchor(self, anchor:str, is_bare):
 
-        completer  = AutoCompletion.get_completer_for(RefKind.Link)
+        completer  = AutoCompletion.get_for(RefKind.Link)
         identifier = completer.get_final_identifier(anchor)
         references = self.plugin.global_handler.references
         unknown_id = not references.has_id(identifier)
 
         # The id should always exist, except in one case: if ignore_auto_headers is true, the user
         # might be pointing at one of the unregistered anchors... In that case, and if the user
         # didn't ask for a strict check of anchors, just issue a warning in the console.
```

### Comparing `mkdocs_addresses-0.2.4/mkdocs_addresses/addresses_plugin.py` & `mkdocs_addresses-0.3.0/mkdocs_addresses/addresses_plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import json
 import re
 
-from typing import List, Literal, Set, NamedTuple, Union
+from typing import List, Literal, Set, NamedTuple, Type, Union
 from collections import Counter
 from pathlib import Path
 
 from bs4.element import Tag
 
 from mkdocs.structure.pages import Page
 from mkdocs.structure.files import Files, File
@@ -28,29 +28,32 @@
     InvalidIdentifierError,
     LeadingSlashAddressError,
     NonAbsoluteAddressError,
     OutdatedReferenceError,
     UnknownExternalLinkIdentifierError,
     UnknownIdentifierError,
 )
+from .auto_completion_handler import (
+    RefKind,
+    AutoCompletion,
+    IdeKind,
+    PLUGIN_MARK,
+)
 from .config_plugin import (
     AddressAddressesConfig,
     ConfigDescriptor,
     NO_DUMP,
     DUMP_ONLY,
-    PLUGIN_MARK,
 )
 from .static_handler import StaticHandler
 from .toolbox import (
-    build_other_snippet,
     extract_external_links_refs_in_md,
     plugin_dump_padder,
     fatal_if
 )
-from .auto_completion_handler import RefKind, AutoCompletion
 from .addresses_checker import AddressChecker, AddressKind
 from .logger import LogMessages, logger, addresses_auto_log_plugin_on
 
 
 
 
 
@@ -123,19 +126,19 @@
 
 #----------------------------------------
 
 
 def never_skip(*_,**__):
     return False
 
-def skip_if_no_vsc_or_no_snippets_file_or_wrong_extension(plugin:'AddressAddressesPlugin', *_, **__) -> bool:
-    no_vsc    = not plugin.use_vsc
-    no_file   = not plugin.dump_snippets_file.is_file()
-    wrong_ext = not plugin.dump_snippets_file.suffix == '.code-snippets'
-    return no_vsc or no_file or wrong_ext
+def skip_if_no_autocompletion_or_no_snippets_file_or_wrong_extension(plugin:'AddressAddressesPlugin', *_, **__) -> bool:
+    no_autocomp = not plugin.use_auto_completion
+    no_file     = not plugin.dump_snippets_file.is_file()
+    wrong_ext   = no_file or plugin.dump_snippets_file.suffix == '.txt'
+    return no_autocomp or wrong_ext
 
 def skip_if_no_external_links(plugin:'AddressAddressesPlugin', *_, **__) -> bool:
     return not plugin.external_links_file
 
 def skip_if_only_dump(plugin:'AddressAddressesPlugin', *_, **__) -> bool:
     """ Check special reasons to not apply the on_page_context event """
     return plugin.dump_action == DUMP_ONLY
@@ -175,14 +178,17 @@
     """ Relative to cwd """
 
     fail_fast: bool = ConfigDescriptor()
     """ If false, information about the exceptions raised by the plugin are logged to the console
         but are caught, to let the executions go.
     """
 
+    ide: IdeKind = ConfigDescriptor()
+    """ Ide to use for autocompletion """
+
     imgs_extension_pattern: re.Pattern = ConfigDescriptor()
     """ Regex pattern used to decide what should be considered a file or an image.
         This will decide the prefix used ('!!' for images and '++' for files)
     """
 
     ignore_auto_headers: bool = ConfigDescriptor()
     """ If true, the plugin will try to spot headers without specific id attribute and won't
@@ -218,43 +224,46 @@
 
     uni_docs_dir: PathCwd = ConfigDescriptor()
     """ Relative to cwd """
 
     use_directory_urls: bool = ConfigDescriptor()
     """ keep track of the config value """
 
-    use_vsc: bool = ConfigDescriptor()
-    # Note: if this needs to evolve further, to offer support for autocompletion with other
-    #       softwares, this should probably become "use_auto_completion" (to check it matches
-    #       every use case)
-
     strict_anchor_check: bool = ConfigDescriptor()
 
     verify_only: Set[UriDocsPathStr] = ConfigDescriptor()
     """ Set of files to verify during on_page_context. If empty, all (updated) files are checked,
         otherwise, only the files listed here are checked (if they have been updated, when the
         cache is activated).
     """
 
 
 
 
     # Plugin specific:
     global_handler: StaticHandler
+    completion: Type[AutoCompletion]
 
+    @property
+    def use_auto_completion(self) -> bool:
+        return self.ide != 'none'
 
 
     def __str__(self):
+        props_to_show = set(self.__class__.__annotations__.keys()) \
+                      - {'global_handler', 'completion'}
         plugin = {
-            prop: list(val) if isinstance((val:=getattr(self,prop)),set) else
-                  val.pattern if isinstance(val, re.Pattern) else
-                  ['...'] if prop=='global_handler' else
-                  str(val) if isinstance(val, Path) else
-                  val
-            for prop in sorted(self.__class__.__annotations__.keys())
+            prop: (
+                list(val) if isinstance((val:=getattr(self,prop)),set) else
+                val.pattern if isinstance(val, re.Pattern) else
+                ['...'] if prop=='global_handler' else
+                str(val) if isinstance(val, Path) else
+                val
+            )
+            for prop in sorted(props_to_show)
         }
         plugin.update({
             "references": dict(self.global_handler.references.id_to_data),
         })
         return f'{ self.__class__.__name__ }:\n{ json.dumps(plugin, indent=4) }'
 
 
@@ -329,15 +338,15 @@
         logger.debug(f'Gather all references used in page: { page.file.src_uri !r}')
         # Done first because og the soup.decompose_header_to_kebab step, which will mutate
         # the content of the html soup tree...
 
         soup = PluginSoupExcludingCodes(html, self)
 
         for tag, attr, _, identifier in soup.gen_targeted_addresses_data():
-            if AutoCompletion.href_is_possible_ref(identifier):
+            if self.completion.href_is_possible_ref(identifier):
                 logger.debug(f'  Reference used: <{ tag.name } { attr }="{ identifier }">')
                 self.global_handler.used_refs.add_id(page,identifier)
 
         all_external_refs = Counter(extract_external_links_refs_in_md(page.markdown))
         refs_in_code_tags = Counter( soup.get_external_refs_in_codes() )
         actual_refs       = all_external_refs - refs_in_code_tags
         for identifier in actual_refs:
@@ -571,28 +580,28 @@
 
 
 
 
 
     def _setup(self, config:MkDocsConfig):
         """ First inner step of on_config hook (helps with testing) """
-        self.config.validate_and_process(config)
+        self.completion = self.config.validate_and_process(config)
         self.global_handler = StaticHandler.inject(self, config)
                             # Inject ONLY after validation/preprocessing of the config
         self._update_watch_list(config)
 
 
 
     @addresses_auto_log_plugin_on(
         step_name="updating the watch list with inclusions and/or external link file",
         log_errors=False,
     )
     def _update_watch_list(self, config:MkDocsConfig):
 
-        has_includes       = self.use_vsc and self.inclusions
+        has_includes       = self.use_auto_completion and self.inclusions
         has_external_links = self.external_links_file
 
         if not has_includes and not has_external_links:
             return
 
         watching: List[str] = config['watch']
         uri_links = path_manager.to_uri(self.external_links_file) if has_external_links else None
@@ -623,45 +632,37 @@
 
     @addresses_auto_log_plugin_on(
         step_name="extracting the existing code snippets file",
         log_errors=False,
     )
     @StaticHandler.snippets_extraction_cached_with(
         plugin_file_prop_extractor('dump_snippets_file'),
-        skip_if_no_vsc_or_no_snippets_file_or_wrong_extension,
+        skip_if_no_autocompletion_or_no_snippets_file_or_wrong_extension,
     )
     def _extract_and_cleanup_current_snippets_file(self):
         """ If using VSC and a code snippets file is provided, extract it and check if the user
             added anything not related to the plugin. If so, store that for the next dump.
             Every entry related to the plugin is discarded.
         """
         self.log_more(LogMessages.setup_snippets)
         snippets = self.dump_snippets_file.read_text()
-
-        # Keep only things that weren't previously generated (just in case...)
-        json_as_dict = json.loads(snippets).items()
-        other_snippets = (
-            build_other_snippet(name, d)
-            for name,d in json_as_dict
-            if 'description' not in d or PLUGIN_MARK not in d['description']
-        )
-        self.global_handler.references.store_other_snippets(other_snippets)
+        self.completion.store_other_snippets(snippets)
 
 
 
 
     @addresses_auto_log_plugin_on(
         step_name="building files inclusions snippets",
         log_errors=False,
     )
     def _build_inclusions_snippets(self):
         """ Travel recursively through the content of each paths in the inclusions and build
             the related snippets.
         """
-        if self.use_vsc and self.inclusions:
+        if self.use_auto_completion and self.inclusions:
 
             self.log_more(LogMessages.build_inclusions)
 
             for root_include in self.inclusions:
                 for file in root_include.rglob('./*'):
                     if file.is_file():
                         self._gather_inclusions_in(file, root_include)
@@ -692,18 +693,18 @@
     @StaticHandler.external_links_cached_with(
         plugin_file_prop_extractor('external_links_file'),
         skip_if_no_external_links,
     )
     def _add_external_links_if_needed(self):
         """ Add external links
 
-            Note: the references of those links aren't stored, and only the autocompletion
-                  informations are actually interesting, because mkdocs will replace the
-                  identifiers on it's own. But the equivalent references are stored anyway
-                  so that the txt file dumped if use_vsc=false still contains everything.
+            Note: The references of those links aren't stored, and only the autocompletion
+                  informations are actually interesting, because mkdocs will replace the identifiers
+                  on it's own. But the equivalent references are stored anyway so that the txt file
+                  dumped when use_auto_completion=false still contains everything.
         """
         self.log_more(LogMessages.setup_links)
         code = self.external_links_file.read_text()
         self._add_external_links(code)
 
 
     def _add_external_links(self, code:str):
@@ -735,24 +736,24 @@
     def _build_identifiers_for_all_files_in_docs_dir_except_markdowns(self, files:Files):
         """ Add all fixed files in the docs directory:, except for markdown ones
             (let mkdocs build the urls for those, according to the user's settings)
         """
         self.log(LogMessages.setup_non_md_files)
 
         for file in files:
-            uri   = file.src_uri
+            cwd_path = self.uni_docs_dir / file.src_path
+            uri = file.src_uri
             is_md = uri.endswith('.md')
-            is_built = (
+            is_builtin = (
                 uri.startswith('assets/javascripts/')
                 or uri.startswith('assets/stylesheets/')
                 or uri == 'assets/images/favicon.png'       # mkdocs default config
             )
-            cwd_path = self.uni_docs_dir / file.src_path
-
-            if not is_built and not is_md:
+            is_to_skip = self.black_list_pattern.match(str(cwd_path))
+            if not is_builtin and not is_md and not is_to_skip:
                 self.add_file_infos(cwd_path, file)
 
 
 
 
     @StaticHandler.other_files_cached_with(
         cwd_path_arg_extractor_other_files,
@@ -814,18 +815,18 @@
             @identifier: Bare identifier that will be used to build the code snippet prefix
                          (for example: "plain-address" -> "--plain-address" for a RefKind.Link,
                          or "code_ex.py" -> "<<py code_ex.py" for a RefKind.Include, ...)
             @def_link:   Target document/link for the snippet(s) (as uri)
             @**extras:   Extra arguments that will be passed to the VscAutoCompletion.build_snippet
                          method.
         """
-        completer = AutoCompletion.get_completer_for(kind)
+        completer = self.completion.get_for(kind)
         final_id  = completer.get_final_identifier(identifier)
 
-        if self.use_vsc:
+        if self.use_auto_completion:
             logger.debug(f"Adding code snippet(s) for {identifier=!r}: {def_link=!r}")
             for json_id,snippet in completer.build_snippet(identifier, def_link, **extras):
                 self.global_handler.references.add_snippet(src, json_id, snippet)
 
         return final_id
 
 
@@ -904,15 +905,15 @@
             to_check and identifier.startswith('/'),
             f"No leading slash address allowed: {identifier!r}.\nIf you absolutely need it, "
             'mark it as ignored, one way or another (black_list_pattern, or '
             'ignored_identifiers_or_addresses).',
             LeadingSlashAddressError
         )
 
-        if AutoCompletion.href_is_possible_ref(identifier):
+        if self.completion.href_is_possible_ref(identifier):
             logger.debug(f"Build the correct relative path for \"{identifier}\"...")
             target    = self.__build_path_from_caller_to_id(page, identifier)
             tag[attr] = target
             logger.debug(f"\"{ identifier }\" built as: { target !r}")
             is_built_ref = True
 
 
@@ -928,27 +929,25 @@
         # Check the address only if it has not been built by the plugin (this is assuming
         # it will do a proper job... :p )
         if to_check and not is_built_ref:
             AddressChecker.check(self, page, target, kind)
 
 
 
+    def build_snippets_code(self):
+        """ Build all snippets """
+        code = self.completion.build_snippets_code(self)
+        return code
 
-    def _dump_snippets(self):
-        logger.debug(f"Building data to dump (use_vsc={ self.use_vsc })")
 
-        if self.use_vsc:
-            code = self.global_handler.references.build_json_snippets()
-        else:
-            items_gen = self.global_handler.references.gen_refs_items()
-            code = "Identifier | Target\n--------------------\n\n" + "".join(
-                f"{ plugin_dump_padder(identifier+':') } { file } \n"
-                for identifier,file in sorted(items_gen)
-            )
 
+    def _dump_snippets(self):
+        logger.debug(f"Building data to dump (ide={ self.ide })")
+
+        code = self.build_snippets_code()
         self.dump_snippets_file.parent.mkdir(exist_ok=True)
         self.dump_snippets_file.write_text(code)
         self.global_handler.files_tracker.mark_file(self.dump_snippets_file)
 
         self.log(LogMessages.on_post_build_out)
```

### Comparing `mkdocs_addresses-0.2.4/mkdocs_addresses/config_plugin.py` & `mkdocs_addresses-0.3.0/mkdocs_addresses/config_plugin.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,26 @@
 from argparse import Namespace
 import os
 from pathlib import Path
 import re
 
-from typing import Any, Callable, List, Literal, Optional, Tuple, TYPE_CHECKING
+from typing import Any, Callable, List, Literal, Optional, Tuple, TYPE_CHECKING, Union
 
 from mkdocs.config import config_options  as C
 from mkdocs.config.base import Config
 from mkdocs.config.defaults import MkDocsConfig
 
 from mkdocs_addresses import path_manager
+from mkdocs_addresses.exceptions import AddresserConfigError, InvalidOperationError
+from mkdocs_addresses.auto_completion_handler import (
+    AutoCompletion,
+    IDE_OPTIONS, VSC, IdeKind,
+    validate_config_and_get_auto_completion_handler,
+)
 
-from .exceptions import AddresserConfigError, InvalidOperationError
 
 if TYPE_CHECKING:
     from .addresses_plugin import AddressAddressesPlugin
 
 
 
 
@@ -69,34 +74,31 @@
       to stop serving.
 
         This option is useful when there's a need to regenerate code snippets while something
         in the addresses verifications steps causes a crash.
     """
 
 
-    dump_file_vsc: str = '.vscode/links.code-snippets'
-    dump_file_txt: str = 'addresses_identifiers.txt'
     dump_snippets_file: str = ''
     """
     Define the location, relative to the cwd, of the file where the information regarding all
-    the references (either code snippets configuration or plain text) will be stored.
+    the identifiers (either code snippets configuration or plain text) will be stored.
 
     There are restrictions about the name of this file:
 
     * The file cannot be in the `docs_dir` (it should never be anyway).
     * The extension of the file must be compatible with the value chosen for the
-    [`use_vsc`][mkdocs_addresses.config_plugin.PluginOptions.use_vsc]
-    option (see table below).
+    [`ide`][mkdocs_addresses.config_plugin.PluginOptions.ide] option (see table below).
     * If left undefined, the filename is automatically defined, depending on the value of the
-      [`use_vsc`](--mkdocs_addresses_config_plugin_PluginOptions_use_vsc) option:
+      [`ide`](--mkdocs_addresses_config_plugin_PluginOptions_ide) option:
 
-    | `use_vsc` | Default `dump_snippets_file` | Required file extension |
+    | `ide` | Default `dump_snippets_file` | Required file extension |
     |:-|:-|:-|
-    | `true` | `.vscode/links.code-snippets` | `.code-snippets` |
-    | `false` | `addresses_identifiers.txt` | `.txt` |
+    | `none` | `addresses_identifiers.txt` | `.txt` |
+    | `vsc` | `.vscode/links.code-snippets` | `.code-snippets` |
     """
 
 
     external_links_file: str = ''
     """
     Location of the file where are defined the global links/references, if any:
 
@@ -159,14 +161,33 @@
 
     Note that some errors will appear separately from these summaries. Specifically,
     [`OutDatedReferenceError`](--mkdocs_addresses_exceptions_OutdatedReferenceError), which is
     checked at a different point during the validation process.
     """
 
 
+    ide: IdeKind = VSC
+    """
+    Controls the kind of IDE used, for the autocompletion features. Possible values are:
+
+    * `none`: no autocompletion activated. A simple txt file with all the available identifiers will
+      be generated (see [`dump_snippets_file`][mkdocs_addresses.config_plugin.PluginOptions.dump_snippets_file]).
+
+    * In any other case, code snippets will be automatically generated and saved in the appropriate
+      [`dump_snippets_file`][mkdocs_addresses.config_plugin.PluginOptions.dump_snippets_file].
+
+    Note:
+        Remember that this option determines the kind of file used for the
+        [`dump_snippets_file`][mkdocs_addresses.config_plugin.PluginOptions.dump_snippets_file]
+        option: if a filename is assigned to it, its extension has to match with the chosen value
+        for `ide` (see the [`dump_snippets_file`][mkdocs_addresses.config_plugin.PluginOptions.dump_snippets_file]
+        section above).
+    """
+
+
     ignore_auto_headers: bool = True
     """
     Controls whether the "bare headers" will be taken into account when the plugin collects
     identifiers from the documentation.
     <br>Note that both options have their advantages and disadvantages. For more details, see the
     section about [handling automatic mkdocs headers](--identifiers-handling-headers).
 
@@ -331,34 +352,34 @@
         In summary:
 
         * Setting `strict_anchor_check` to false is not recommended, as it diminishes the
           reliability of the plugin's verifications.
         * But it might be useful to facilitate the integration of the plugin into older projects.
     """
 
+    # LEGACY:
+    use_vsc: Union[bool,None] = None
+    # """
+    # Controls the kind of file the plugin will generate with all the collected identifiers.
 
-    use_vsc: bool = True
-    """
-    Controls the kind of file the plugin will generate with all the collected identifiers.
-
-    * If true, a VSC `.code-snippets` file will be created, enabling autocompletion features.
-      This file is located at the value specified for the
-      [`dump_snippets_file`][mkdocs_addresses.config_plugin.PluginOptions.dump_snippets_file]
-      option.
-    * If false, the plugin overall behavior remains unchanged, but a simple `.txt` file is
-      generated instead, containing the identifiers and the related targeted address.
-
-    Note:
-        Remember that this option determines the kind of file used for the
-        [`dump_snippets_file`][mkdocs_addresses.config_plugin.PluginOptions.dump_snippets_file]
-        option. This means that if you assigned a filename to that option, its extension has
-        to match with the chosen value for `use_vsc` (see the
-        [`dump_snippets_file`][mkdocs_addresses.config_plugin.PluginOptions.dump_snippets_file]
-        section above).
-    """
+    # * If true, a VSC `.code-snippets` file will be created, enabling autocompletion features.
+    #   This file is located at the value specified for the
+    #   [`dump_snippets_file`][mkdocs_addresses.config_plugin.PluginOptions.dump_snippets_file]
+    #   option.
+    # * If false, the plugin overall behavior remains unchanged, but a simple `.txt` file is
+    #   generated instead, containing the identifiers and the related targeted address.
+
+    # Note:
+    #     Remember that this option determines the kind of file used for the
+    #     [`dump_snippets_file`][mkdocs_addresses.config_plugin.PluginOptions.dump_snippets_file]
+    #     option. This means that if you assigned a filename to that option, its extension has
+    #     to match with the chosen value for `use_vsc` (see the
+    #     [`dump_snippets_file`][mkdocs_addresses.config_plugin.PluginOptions.dump_snippets_file]
+    #     section above).
+    # """
 
 
     verify_only: List[str] = []
     """
     Each entry denotes the location of the only files (slash separated, and relative to the
     _^^`docs_dir`^^_) that will be validated by the plugin. All other operations proceed as usual.
 
@@ -376,17 +397,14 @@
 
 CONFIG_ANNOTATIONS = set(PluginOptions.__annotations__) - { "dump_file_vsc", "dump_file_txt" }
 
 
 
 
 
-PLUGIN_MARK = "VSC-REF"
-
-
 
 DUMP_OPTIONS = tuple('normal only none'.split())
 NORMAL, DUMP_ONLY, NO_DUMP = DUMP_OPTIONS
 assert PluginOptions.dump_action in DUMP_OPTIONS, "Invalid plugin setup"
 
 
 
@@ -409,14 +427,16 @@
 
     dump_snippets_file = C.Type(str, default='')      # Automatically overridden at validation time
 
     external_links_file = C.Type(str, default=PluginOptions.external_links_file)
 
     fail_fast = C.Type(bool, default=PluginOptions.fail_fast)
 
+    ide = C.Choice(IDE_OPTIONS, default=PluginOptions.ide)
+
     imgs_extension_pattern = C.Type(str, default=PluginOptions.imgs_extension_pattern)
 
     ignore_auto_headers = C.Type(bool, default=PluginOptions.ignore_auto_headers)
 
     ignored_identifiers_or_addresses = C.ListOfItems(C.Type(str), default=PluginOptions.ignored_identifiers_or_addresses)
 
     ignored_classes = C.ListOfItems(C.Type(str), default=PluginOptions.ignored_classes)
@@ -429,14 +449,15 @@
 
     more_verbose = C.Type(bool, default=PluginOptions.more_verbose)
 
     plugin_off = C.Type(bool, default=PluginOptions.plugin_off)
 
     strict_anchor_check = C.Type(bool, default=PluginOptions.strict_anchor_check)
 
+    # LEGACY:
     use_vsc = C.Type(bool, default=PluginOptions.use_vsc)
 
     verify_only = C.ListOfItems(C.File(exists=True), default=PluginOptions.verify_only)
 
 
 
     #----------------------------------------------
@@ -446,28 +467,35 @@
     def validate_and_process(self, config:MkDocsConfig):
         """ Performs the basic, then extras validations on each property, and also apply the
             post conversions to the data structures that need it.
             Add on the fly the needed fields from the mkdocs config.
         """
 
         # Enforce no unexpected option name (because this is boring AF...)
-        user_settings = set(self.user_configs[-1])
+        # Enforce no unexpected option name (because this is boring AF...)
+        if 'plugins' in config and 'mkdocs-addresses' in config.plugins:
+            settings = set(config.plugins['mkdocs-addresses'].config)
+            base_settings = set(dir(config.plugins['mkdocs-addresses'].__class__.mro()[1]))
+            user_settings = settings - base_settings
+        else:
+            # when testing in mkdocs-addresses, the plugin isn't in the yml file (must change
+            # that: see use of entry-points in pyodide-mkdocs-theme):
+            user_settings = set(self.user_configs[-1])
+
         nope          = user_settings - CONFIG_ANNOTATIONS
         if nope:
             nope    = ''.join( '\n   '+key for key in sorted(nope))
             options = ''.join( '\n   '+key for key in sorted(CONFIG_ANNOTATIONS))
             raise AddresserConfigError(
                 f"Unexpected option(s) name(s):{ nope }\n\n Available options are:{options}"
             )
 
-        # Pre-conversions:
-        #-----------------
-
-        if not self.dump_snippets_file:
-            self.dump_snippets_file = PluginOptions.dump_file_vsc if self.use_vsc else PluginOptions.dump_file_txt
+        # Extract completion handler class, handling use_vsc, ide and dump_snippets_file defaults
+        # (no validation):
+        completion_class = validate_config_and_get_auto_completion_handler(self)
 
 
         # Perform "post" conversions:       (yeah, "post"... lol...)
         #----------------------------
 
         maybe_abs = path_manager.to_os(config['docs_dir'])
         self.uni_docs_dir = maybe_abs.absolute().relative_to(Path.cwd())
@@ -488,87 +516,95 @@
                     setattr(self, prop, post)
                 except Exception as e:                              # pylint: disable=all
                     e.args = ( f"{ prop }: { e.args[0] }",)
                     raise
 
         self.ignored_classes.add('headerlink')      # this avoids to consider mkdocs permalinks in headers, when used
 
-        # More specific validations:
-        #---------------------------
+        # More specific validations and post conversions:
+        #------------------------------------------------
 
-        self.__validate_inclusions_dir()
-        self.__validate_black_list_pattern()
-        self.__validate_external_links_file()
-        self.__validate_dump_snippets_file()
-        self.__validate_verify_only_md_files()
-        self.__validate_vsc_and_dump_filename_consistency()
+        self._validate_inclusions_dir()
+        self._validate_black_list_pattern()
+        self._validate_external_links_file()
+        self._validate_verify_only_md_files()
+        self._validate_auto_completion_config(completion_class)
+        self._validate_dump_extension_vs_ide(completion_class)
 
+        return completion_class
 
 
     #----------------------------------------------
 
-    def __check_not_in_docs(self, prop:str, path:str):
+
+    def _check_not_in_docs(self, prop:str, path:str):
         rel = os.path.relpath(path, self.uni_docs_dir)
         if not rel.startswith('..'):
             raise AddresserConfigError(
                 f"{prop}: {path!r} should not be inside the docs_dir directory"
             )
 
 
-    def __validate_inclusions_dir(self):
+    #----------------------------------------------
+
+
+    def _validate_inclusions_dir(self):
         self.inclusions = sorted(map( path_manager.to_os, self.inclusions))
         oops = [location for location in self.inclusions if not location.is_dir() ]
         if oops:
             raise AddresserConfigError(
                 f"'inclusions' should be a list of directories, but found invalid paths: ({ oops !r})"
             )
 
         for path in self.inclusions:
-            self.__check_not_in_docs('inclusions', path)
+            self._check_not_in_docs('inclusions', path)
 
 
-    def __validate_black_list_pattern(self):
+
+    def _validate_black_list_pattern(self):
         if not self.black_list_pattern.pattern:      # this is now a pattern, not a string anymore!
             raise AddresserConfigError(
                 "black_list_pattern should never be an empty string. Note that not using at "
                 "least the default pattern will definitely cause problems..."
             )
 
 
-    def __validate_external_links_file(self):
+
+    def _validate_external_links_file(self):
         if not self.external_links_file:
             return
 
         self.external_links_file = p = path_manager.to_os(self.external_links_file)
         if not p.is_file() or not p.suffix=='.md':
             raise AddresserConfigError(
                 "'external_links_file' is configured, but is not an existing markdown file "
                 f'("{ self.external_links_file }")'
             )
-        self.__check_not_in_docs('external_links_file', self.external_links_file)
+        self._check_not_in_docs('external_links_file', self.external_links_file)
 
 
-    def __validate_dump_snippets_file(self):
+
+    def _validate_auto_completion_config(self, completion_class:AutoCompletion):
         self.dump_snippets_file = path_manager.to_os(self.dump_snippets_file)
-        self.__check_not_in_docs('dump_snippets_file', self.dump_snippets_file)
+        self._check_not_in_docs('dump_snippets_file', self.dump_snippets_file)
 
 
-    def __validate_vsc_and_dump_filename_consistency(self):
-        snip_file:Path   = self.dump_snippets_file
-        vsc_and_snippets = self.use_vsc and snip_file.suffix=='.code-snippets'
-        not_vsc_and_txt  = not self.use_vsc and snip_file.suffix=='.txt'
-        if not (vsc_and_snippets or not_vsc_and_txt):
+    def _validate_dump_extension_vs_ide(self, completion_class:AutoCompletion):
+        # Note: separated from _validate_auto_completion_config for testing purpose.
+        needed_suffix:str = path_manager.to_os(completion_class.filename).suffix
+        if self.dump_snippets_file.suffix != needed_suffix:
             raise AddresserConfigError(
                 "Inconsistent configuration:\n"
-                f"   use_vsc: {self.use_vsc}\n"
+                f"   ide: {self.ide}\n"
                 f"   dump_snippets_file: {self.dump_snippets_file}"
             )
 
 
-    def __validate_verify_only_md_files(self):
+
+    def _validate_verify_only_md_files(self):
         invalids = [ file for file in self.verify_only
                           if not path_manager.to_os(file).suffix=='.md']
         if invalids:
             raise AddresserConfigError(
                 "All options for `verify_only` should be valid markdown files, relative to the cwd.\n"
                 +"Invalid entries:" + "".join('\n    '+file for file in invalids)
             )
```

### Comparing `mkdocs_addresses-0.2.4/mkdocs_addresses/exceptions.py` & `mkdocs_addresses-0.3.0/mkdocs_addresses/exceptions.py`

 * *Files identical despite different names*

### Comparing `mkdocs_addresses-0.2.4/mkdocs_addresses/logger.py` & `mkdocs_addresses-0.3.0/mkdocs_addresses/logger.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 See: https://github.com/mkdocs/mkdocs/discussions/3241
 """
 from argparse import Namespace
+import platform
 import traceback
 import logging
 
 from typing import TYPE_CHECKING, Any, MutableMapping, Tuple
 from functools import wraps
 
 from mkdocs_addresses.exceptions import AbortError, AddresserError
@@ -55,14 +56,16 @@
 
         Arguments:
             prefix: The string to insert in front of every message.
             logger: The logger instance.
         """
         super().__init__(logger, {})
         self.prefix = prefix
+        if platform.system() != 'Windows':
+            self.prefix = f"\033[35m{ prefix }\033[0m"
 
     def process(self, msg: str, kwargs: MutableMapping[str, Any]) -> Tuple[str, Any]:
         """Process the message.
 
         Arguments:
             msg: The message:
             kwargs: Remaining arguments.
```

### Comparing `mkdocs_addresses-0.2.4/mkdocs_addresses/other_plugins_handling/autorefs.py` & `mkdocs_addresses-0.3.0/mkdocs_addresses/other_plugins_handling/autorefs.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,16 +21,16 @@
     a reference doesn't exist, while the others 'with existing ref) have already been replaced
 
     BUT these spans also appear in the html generated by mkdocstrings, and will be replaced with
     links only during a post processing step (I didn't search when exactly, but in on_page_context
     hooks, they are still present as <span>, and not <a>). So the invalid references must be searched
     for very carefully.
     """
-    external_links = AutoCompletion.get_completer_for(RefKind.Ext)
-    links          = AutoCompletion.get_completer_for(RefKind.Link)
+    external_links = AutoCompletion.get_for(RefKind.Ext)
+    links          = AutoCompletion.get_for(RefKind.Link)
     for span in soup.find_all('span'):
         if not span.has_attr("data-autorefs-identifier"):
             continue
         identifier = span['data-autorefs-identifier']
         link_id    = links.get_final_identifier(identifier)
         ext_id     = external_links.get_final_identifier(identifier)
         if not defined_refs.has_id(link_id) and not defined_refs.has_id(ext_id):
```

### Comparing `mkdocs_addresses-0.2.4/mkdocs_addresses/path_manager.py` & `mkdocs_addresses-0.3.0/mkdocs_addresses/path_manager.py`

 * *Files identical despite different names*

### Comparing `mkdocs_addresses-0.2.4/mkdocs_addresses/soup_excluding_codes.py` & `mkdocs_addresses-0.3.0/mkdocs_addresses/soup_excluding_codes.py`

 * *Files identical despite different names*

### Comparing `mkdocs_addresses-0.2.4/mkdocs_addresses/static_handler/__init__.py` & `mkdocs_addresses-0.3.0/mkdocs_addresses/static_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `mkdocs_addresses-0.2.4/mkdocs_addresses/static_handler/files_tracker.py` & `mkdocs_addresses-0.3.0/mkdocs_addresses/static_handler/files_tracker.py`

 * *Files identical despite different names*

### Comparing `mkdocs_addresses-0.2.4/mkdocs_addresses/static_handler/static_handler.py` & `mkdocs_addresses-0.3.0/mkdocs_addresses/static_handler/static_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 from typing import TYPE_CHECKING, Any, Callable
 
 from functools import wraps
 
 from mkdocs.structure.pages import Page
 from mkdocs.config.defaults import MkDocsConfig
+from mkdocs_addresses.auto_completion_handler import COMPLETION_CLASSES_CONFIG
 
 
 from mkdocs_addresses.logger import logger
 from mkdocs_addresses.exceptions import (
     NoStaticHandlerError,
 #    ConcurrentPluginError,                                 ##!LOCK
 )
@@ -53,17 +54,17 @@
 
 
 
 #---------------------------------------------------------
 
 
 
-def clear_other_snippets(*_,**__):
+def clear_other_snippets(_, plugin:'AddressAddressesPlugin', *ça,**_kw):
     logger.debug("Clear snippets unrelated to the plugin")
-    StaticHandler.HANDLER.references.clear_other_snippets()
+    plugin.completion.clear_other_snippets()
 
 
 def clear_references_from_src(cwd_path, *_,**__):
     logger.debug(f"Clear previous references for the file {cwd_path=!r}")
     StaticHandler.HANDLER.clear_file_related_data(cwd_path)
 
 
@@ -185,23 +186,28 @@
         Reset the internals of the global StaticHandler, but keeping the current global innstance
         alive (testing purpose, mostly)
         """
         if plugin:
             self._plugin = plugin
         if config:
             self._config = config
+
         self.used_refs          = AddressesUsagePool(uni_docs_dir=plugin.uni_docs_dir)
-        self.references         = References(uni_docs_dir=plugin.uni_docs_dir)
         self.exceptions_counter = ContextExceptionsTracker(uni_docs_dir=plugin.uni_docs_dir)
         self.files_tracker      = FilesTracker()
+        self.references         = References(uni_docs_dir=plugin.uni_docs_dir)
+
+        for TopClass,*_ in COMPLETION_CLASSES_CONFIG.values():
+            TopClass.clear_other_snippets()
+
         return self
 
 
     def rebuild_with(self, plugin:'AddressAddressesPlugin', config:MkDocsConfig):
-        """ On a new build, use the fresh instances, checking of a global rebuild of the
+        """ On a new build, use the fresh instances, checking if a global rebuild of the
             internal data must be made or note.
             This happens on_build only.
         """
         self._plugin = plugin
         self._config = config
         self.used_refs.archive_current(plugin.uni_docs_dir)
         self.references.archive_current(plugin.uni_docs_dir)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `mkdocs_addresses-0.2.4/mkdocs_addresses/static_handler/tracker_addresses_usage_pool.py` & `mkdocs_addresses-0.3.0/mkdocs_addresses/static_handler/tracker_addresses_usage_pool.py`

 * *Files identical despite different names*

### Comparing `mkdocs_addresses-0.2.4/mkdocs_addresses/static_handler/tracker_data_pages.py` & `mkdocs_addresses-0.3.0/mkdocs_addresses/static_handler/tracker_data_pages.py`

 * *Files identical despite different names*

### Comparing `mkdocs_addresses-0.2.4/mkdocs_addresses/static_handler/tracker_errors_counter.py` & `mkdocs_addresses-0.3.0/mkdocs_addresses/static_handler/tracker_errors_counter.py`

 * *Files identical despite different names*

### Comparing `mkdocs_addresses-0.2.4/mkdocs_addresses/static_handler/tracker_references.py` & `mkdocs_addresses-0.3.0/mkdocs_addresses/static_handler/tracker_references.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 
 
-from typing import Any, Dict, Iterable, List, Set
+from typing import Any, Dict, Set
 
 
 
 from mkdocs_addresses.exceptions import DuplicateIdentifierError
 from mkdocs_addresses.static_handler.tracker_data_pages import PageDataTracker
 from .types_aliases import Ref, PathCwd, SnipDescription, SourceRef
 
@@ -23,15 +23,15 @@
     """
     Keep track of each reference definition (headers, explicit ids, files, external links in a
     dedicated file):
         - identifier
         - associated source to point to when the identifier will be used
         - file location of the identifier (as "source uri")
           WARNING: the path is relative to the cwd.
-        - code snippets associated to each identifier, if use_vsc is True
+        - code snippets associated to each identifier, if use_auto_completion is True
         - ensure that all identifiers (references or those used for the code snippets) are
           unique, otherwise raise DuplicateIdentifierError
 
     Note about the external links: they are stored only to build the code snippets/info file
     about the available references? Mkdocs actually already handles their transformation into
     proper urls.
     """
@@ -43,48 +43,38 @@
         |:-|:-|
         | A link/img ref<br>(`--link`/`!!img`) | Url page/file in the rendered website, relative to the docs_dir |
         | A file ref (`++file`) | Url of the file in the rendered website, relative to the docs_dir |
         | An external link ref (`BusService`) | the url of the link |
         | Description of a snippet | complete code, as string, of the item for the snippet |
     """
 
-    other_entries:  List[Any]
-    """ List of any code snippet the user might have added in the target file (when using vsc) """
-
     snippets: Dict[SnipDescription,str]
     """ Dict "snippet description -> full snippet item code (as string)"
         The snippet description is the key used to identify a snippet in the final file.
     """
 
     _old_refs: Set[Ref]
     """ Registered references during the previous build """
 
 
     UNIQUE_SRC = True       # override
 
 
     def __init__(self, uni_docs_dir:PathCwd):
         super().__init__(uni_docs_dir)
-        self.id_to_data     = {}
-        self.snippets       = {}
-        self.other_entries  = []
-        self._old_refs      = set()
+        self.id_to_data = {}
+        self.snippets   = {}
+        self._old_refs  = set()
 
 
 
     #--------------------------------------------------------------
     # Snippets related logistic
 
 
-    def clear_other_snippets(self):
-        self.other_entries.clear()
-
-    def store_other_snippets(self, snippets:Iterable[str]):
-        self.other_entries.extend(snippets)
-
 
     def add_snippet(self, src:SourceRef, identifier:str, snippet:str):
         here = self.format_source(src)
         if identifier in self.snippets:
             there = next(iter(self.id_to_sources[identifier]))
             raise DuplicateIdentifierError(
                 f"{ identifier !r} is already used.\n"
@@ -95,21 +85,14 @@
 
         self.snippets[identifier] = snippet
         self.id_to_sources[identifier].add(here)
         self.source_to_ids[here].add(identifier)
 
 
 
-    def build_json_snippets(self):
-        snippets = sorted(( *self.other_entries,  *self.snippets.values() ))
-        code = "{\n" + ",\n".join(snippets) + "\n}"
-        return code
-
-
-
     #--------------------------------------------------------------
 
 
     def add_id(
         self,
         source:SourceRef,
         identifier:str,
```

### Comparing `mkdocs_addresses-0.2.4/mkdocs_addresses/static_handler/types_aliases.py` & `mkdocs_addresses-0.3.0/mkdocs_addresses/static_handler/types_aliases.py`

 * *Files identical despite different names*

### Comparing `mkdocs_addresses-0.2.4/pyproject.toml` & `mkdocs_addresses-0.3.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [tool.poetry]
 name = "mkdocs-addresses"
-version = "0.2.4"
+version = "0.3.0"
 description = "Mkdocs automatic paths/addresses building - auto-completion support (VSC)"
 authors = ["Frédéric Zinelli <frederic.zinelli@gmail.com>"]
 readme = "README.md"
-repository = "https://gitlab.com/frederic.zinelli/mkdocs-addresses"
-homepage = "http://frederic.zinelli.gitlab.io/mkdocs-addresses/"
+repository = "https://gitlab.com/frederic-zinelli/mkdocs-addresses"
+homepage = "http://frederic-zinelli.gitlab.io/mkdocs-addresses/"
 exclude = ["mkdocs_addresses/_test_data_extraction.py"]
 keywords = [
     "mkdocs", "mkdocs-plugin", "links", "autocompletion"
 ]
 classifiers = [
     "Environment :: Plugins",
     "Intended Audience :: Developers",
@@ -32,19 +32,19 @@
 [tool.poetry.dependencies]
 python = "^3.8"
 mkdocs = "^1.4"
 beautifulsoup4 = "^4.12"
 
 
 [tool.poetry.group.dev.dependencies]
-mkdocs-material = "^9.1.18"
-mkdocs-glightbox = "^0.3.4"
-pylint = "^2.17.4"
-pytest = "^7.4.0"
-pytest-cov = "^4.1.0"
+mkdocs-material = "^9.1"
+mkdocs-glightbox = "^0.3"
+pylint = "^2.17"
+pytest = "^7.4"
+pytest-cov = "^4.1"
 
 
 [tool.poetry.group.docs.dependencies]
 mkdocstrings = {version = "^0.22.0", extras = ["python"] }
 
 
 [tool.poetry.group.toxic.dependencies]
```

### Comparing `mkdocs_addresses-0.2.4/PKG-INFO` & `mkdocs_addresses-0.3.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: mkdocs-addresses
-Version: 0.2.4
+Version: 0.3.0
 Summary: Mkdocs automatic paths/addresses building - auto-completion support (VSC)
-Home-page: http://frederic.zinelli.gitlab.io/mkdocs-addresses/
+Home-page: http://frederic-zinelli.gitlab.io/mkdocs-addresses/
 Keywords: mkdocs,mkdocs-plugin,links,autocompletion
 Author: Frédéric Zinelli
 Author-email: frederic.zinelli@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Environment :: Plugins
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
@@ -24,25 +24,25 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Documentation
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Documentation
 Classifier: Topic :: Utilities
 Requires-Dist: beautifulsoup4 (>=4.12,<5.0)
 Requires-Dist: mkdocs (>=1.4,<2.0)
-Project-URL: Repository, https://gitlab.com/frederic.zinelli/mkdocs-addresses
+Project-URL: Repository, https://gitlab.com/frederic-zinelli/mkdocs-addresses
 Description-Content-Type: text/markdown
 
 
-![coverage badge](https://gitlab.com/frederic.zinelli/mkdocs-addresses/badges/main/pipeline.svg) ![coverage badge](https://gitlab.com/frederic.zinelli/mkdocs-addresses/badges/main/coverage.svg)
+![coverage badge](https://gitlab.com/frederic-zinelli/mkdocs-addresses/badges/main/pipeline.svg) ![coverage badge](https://gitlab.com/frederic-zinelli/mkdocs-addresses/badges/main/coverage.svg)
 
 
 ## Links
 
-* [Project repository (GitLab)](https://gitlab.com/frederic.zinelli/mkdocs-addresses)
-* [Full online documentation](http://frederic.zinelli.gitlab.io/mkdocs-addresses/)
+* [Project repository (GitLab)](https://gitlab.com/frederic-zinelli/mkdocs-addresses)
+* [Full online documentation](http://frederic-zinelli.gitlab.io/mkdocs-addresses/)
 * [The project on PyPI](https://pypi.org/project/mkdocs-addresses/)
 
 
 
 ## Dependencies
 
 * Python 3.8+
@@ -93,18 +93,18 @@
 
 Identifiers still work after:
 - Changing header content
 - Moving sections from one file to another
 - Renaming files
 - Moving files
 
-![move-deeper](http://frederic.zinelli.gitlab.io/mkdocs-addresses/assets/move-deeper.png)
+![move-deeper](http://frederic-zinelli.gitlab.io/mkdocs-addresses/assets/move-deeper.png)
 
 
-### Provide [autocompletion helpers](http://frederic.zinelli.gitlab.io/mkdocs-addresses/autocompletion/) (_IDE dependent_)
+### Provide [autocompletion helpers](http://frederic-zinelli.gitlab.io/mkdocs-addresses/autocompletion/) (_IDE dependent_)
 
 _(Currently only available for VSC-like IDEs)_
 
 * All snippets are automatically kept up to date while working on the documentation.
 * They provide various markdown snippets, to get a quick and easy access to all the references defined in the documentation, and use them within the markdown code they are usual used for.
 
 | Kind | Suggestion completion | Inserted markdown |
@@ -115,37 +115,37 @@
 | Images in `assets/` | `Img.file_in_assets_jpg` | `![alt content](!!file_in_assets_jpg)` |
 | Other files links | `++file_path_in_docs_html` | `++file_path_in_docs_html` |
 | Other files links | `File.file_path_in_docs_html` | `[link to a file](++file_path_in_docs_html)` |
 | External Links <sup>\*</sup> | `Ext.global_ref` | `[global_ref][global_ref]` |
 | Code inclusions<sup>\*\*</sup> | `::md that_file_md` | `--<8-- "include/that_file.md"` |
 
 
-\*: requires an [external_links_file](http://frederic.zinelli.gitlab.io/mkdocs-addresses/configuration/#mkdocs_addresses.config_plugin.PluginOptions.external_links_file) for global references is configured.
+\*: requires an [external_links_file](http://frederic-zinelli.gitlab.io/mkdocs-addresses/configuration/#mkdocs_addresses.config_plugin.PluginOptions.external_links_file) for global references is configured.
 
-\*\*: requires the use of [inclusions](http://frederic.zinelli.gitlab.io/mkdocs-addresses/configuration/#mkdocs_addresses.config_plugin.PluginOptions.inclusions) directories.
+\*\*: requires the use of [inclusions](http://frederic-zinelli.gitlab.io/mkdocs-addresses/configuration/#mkdocs_addresses.config_plugin.PluginOptions.inclusions) directories.
 
 
 ![autocomplete](docs/assets/auto-completion-point-here.png)
 
 
 
 ### Tracking dead links or addresses in the docs
 
 The plugin also explores the documentation and warns you if it finds invalid addresses or identifiers. This works for:
 
 - Addresses in links
 - Addresses of images
 - Identifiers used by the plugin
 
-![errors-example](http://frederic.zinelli.gitlab.io/mkdocs-addresses/assets/errors-summary.png)
+![errors-example](http://frederic-zinelli.gitlab.io/mkdocs-addresses/assets/errors-summary.png)
 
 
 ### User handed configuration
 
-A lot of [options](http://frederic.zinelli.gitlab.io/mkdocs-addresses/configuration/) are available for the user to fine tune the plugin's behavior.
+A lot of [options](http://frederic-zinelli.gitlab.io/mkdocs-addresses/configuration/) are available for the user to fine tune the plugin's behavior.
 
 
 
 
 
 ## Installation
 
@@ -166,15 +166,15 @@
 Configure the plugin (see below).
 
 
 
 
 ### Recommended `mkdocs.yml` configuration
 
-See the [online documentation](http://frederic.zinelli.gitlab.io/mkdocs-addresses/#installation) for more details.
+See the [online documentation](http://frederic-zinelli.gitlab.io/mkdocs-addresses/#installation) for more details.
 
 #### Markdown extensions
 
 ```yaml
 markdown_extensions:
     - attr_list             # To define the identifiers in the markdown content
     - pymdownx.snippets:    # If you need inclusions code snippets
@@ -197,17 +197,17 @@
 
 Note that the default configuration also implies the following choices:
 
 ```yaml
         - dump_snippets_file: .vscode/links.code-snippets
         - fail_fast: false
         - ignore_auto_headers: true
-        - use_vsc: true
+        - ide: vsc
 ```
-So, if VSC isn't the utilized IDE, the [`use_vsc`](http://frederic.zinelli.gitlab.io/mkdocs-addresses/configuration/#mkdocs_addresses.config_plugin.PluginOptions.use_vsc) option should at the very least be modified.
+So, if VSC isn't the utilized IDE, the [`ide`](http://frederic-zinelli.gitlab.io/mkdocs-addresses/configuration/#mkdocs_addresses.config_plugin.PluginOptions.ide) option should at the very least be modified.
 
 
 #### When using mkdocs 1.5+
 
 Significant enhancements in address verification logic (which was notoriously lacking in earlier versions...) have been added in `mkdocs 1.5+`. But the plugin does more work, and the identifiers it is utilizing are generating warnings in the console.
 
 Hence, deactivate the default verification logic for mkdocs 1.5+:
@@ -217,16 +217,16 @@
     absolute_links: ignore
     unrecognized_links: ignore
 ```
 
 
 ## Links
 
-* [Project repository (GitLab)](https://gitlab.com/frederic.zinelli/mkdocs-addresses)
-* [Full online documentation](http://frederic.zinelli.gitlab.io/mkdocs-addresses/)
+* [Project repository (GitLab)](https://gitlab.com/frederic-zinelli/mkdocs-addresses)
+* [Full online documentation](http://frederic-zinelli.gitlab.io/mkdocs-addresses/)
 * [The project on PyPI](https://pypi.org/project/mkdocs-addresses/)
 
 
 ## License
 
 [Apache-2.0](https://www.tldrlegal.com/license/apache-license-2-0-apache-2-0)
 Copyright © 2023 Zinelli Frédéric
```

